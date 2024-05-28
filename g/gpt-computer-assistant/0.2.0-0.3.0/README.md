# Comparing `tmp/gpt_computer_assistant-0.2.0.tar.gz` & `tmp/gpt_computer_assistant-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_computer_assistant-0.2.0.tar", last modified: Mon May 27 19:32:17 2024, max compression
+gzip compressed data, was "gpt_computer_assistant-0.3.0.tar", last modified: Tue May 28 07:56:34 2024, max compression
```

## Comparing `gpt_computer_assistant-0.2.0.tar` & `gpt_computer_assistant-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.061683 gpt_computer_assistant-0.2.0/gpt_computer_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/background.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/proccess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/gpt_computer_assistant/audio/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/audio/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/audio/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/gpt_computer_assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/gpt_computer_assistant/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/gui/button.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/gui/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/gpt_computer_assistant/screen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/screen/shot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/gpt_computer_assistant/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant/utils/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-27 19:32:16.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-27 19:32:17.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:32:16.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-27 19:32:16.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:32:16.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 19:32:16.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 19:32:16.000000 gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:32:17.065683 gpt_computer_assistant-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-27 19:32:07.000000 gpt_computer_assistant-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.961009 gpt_computer_assistant-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.949009 gpt_computer_assistant-0.3.0/.git/
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.953009 gpt_computer_assistant-0.3.0/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4726 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1649 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1374 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4898 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1492 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2783 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2308 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.953009 gpt_computer_assistant-0.3.0/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-05-28 07:56:19.000000 gpt_computer_assistant-0.3.0/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.953009 gpt_computer_assistant-0.3.0/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.945009 gpt_computer_assistant-0.3.0/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.953009 gpt_computer_assistant-0.3.0/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/logs/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.945009 gpt_computer_assistant-0.3.0/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.953009 gpt_computer_assistant-0.3.0/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/logs/refs/remotes/origin/Added-icon
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/logs/refs/remotes/origin/Added-input-box-and-button
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/logs/refs/remotes/origin/Added-reset-system
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/logs/refs/remotes/origin/Added-splitting-long-audios
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/logs/refs/remotes/origin/master
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.945009 gpt_computer_assistant-0.3.0/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.953009 gpt_computer_assistant-0.3.0/.git/objects/pack/
+-r--r--r--   0 runner    (1001) docker     (127)     5524 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/objects/pack/pack-2e24be27c35a7458f07908a63134ed37c2af0880.idx
+-r--r--r--   0 runner    (1001) docker     (127)    44598 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/objects/pack/pack-2e24be27c35a7458f07908a63134ed37c2af0880.pack
+-r--r--r--   0 runner    (1001) docker     (127)      688 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/objects/pack/pack-2e24be27c35a7458f07908a63134ed37c2af0880.rev
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.945009 gpt_computer_assistant-0.3.0/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.953009 gpt_computer_assistant-0.3.0/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.945009 gpt_computer_assistant-0.3.0/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.953009 gpt_computer_assistant-0.3.0/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/refs/remotes/origin/Added-icon
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/refs/remotes/origin/Added-input-box-and-button
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/refs/remotes/origin/Added-reset-system
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/refs/remotes/origin/Added-splitting-long-audios
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/refs/remotes/origin/master
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.957009 gpt_computer_assistant-0.3.0/.git/refs/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/refs/tags/v0.1.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/refs/tags/v0.1.1
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/refs/tags/v0.1.2
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/refs/tags/v0.2.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.git/refs/tags/v0.3.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.945009 gpt_computer_assistant-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.957009 gpt_computer_assistant-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.github/workflows/deploys.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.github/workflows/release_generation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-28 07:56:34.961009 gpt_computer_assistant-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/bump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.957009 gpt_computer_assistant-0.3.0/gpt_computer_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.957009 gpt_computer_assistant-0.3.0/gpt_computer_assistant/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/agent/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/agent/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/agent/chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/agent/proccess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.961009 gpt_computer_assistant-0.3.0/gpt_computer_assistant/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/audio/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/audio/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/audio/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/gpt_computer_assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.961009 gpt_computer_assistant-0.3.0/gpt_computer_assistant/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/gui/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/gui/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.961009 gpt_computer_assistant-0.3.0/gpt_computer_assistant/screen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/screen/shot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.961009 gpt_computer_assistant-0.3.0/gpt_computer_assistant/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/utils/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.961009 gpt_computer_assistant-0.3.0/gpt_computer_assistant/utils/media/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/utils/media/icon_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/utils/media/icon_24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/utils/media/icon_256.png
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/utils/media/icon_32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant/utils/media/icon_48.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:56:34.957009 gpt_computer_assistant-0.3.0/gpt_computer_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-28 07:56:34.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-28 07:56:34.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:56:34.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-28 07:56:34.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:56:34.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-28 07:56:34.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 07:56:34.000000 gpt_computer_assistant-0.3.0/gpt_computer_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 07:56:34.961009 gpt_computer_assistant-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-28 07:56:20.000000 gpt_computer_assistant-0.3.0/setup.py
```

### Comparing `gpt_computer_assistant-0.2.0/LICENSE` & `gpt_computer_assistant-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.2.0/PKG-INFO` & `gpt_computer_assistant-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_computer_assistant
-Version: 0.2.0
+Version: 0.3.0
 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # GPT Computer Assistant
         Hi, this is an unofficial work for providing ChatGPT MacOS app to Windows and Linux. In this way this is a fresh and stable work. You can easily install as Python library for this time but we will prepare a pipeline to providing native install scripts (.exe).
@@ -28,15 +28,16 @@
          - Writing and Running Scripts
          - Using your Telegram Account
          - Knowledge Management
         
         
         #### Todo
         - [x] Reset Option
-        - [ ] Splitting long audios. (Whisper api just support <20mb)
+        - [x] Splitting long audios. (Whisper api just support <20mb)
+        - [x] Text input area
         - [ ] More Effect
         
         - [ ] Windows .exe
         - [ ] Linux native
         - [ ] MacOS native
         
         
@@ -51,15 +52,16 @@
             <td><img src="https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/10b69a18-033c-4d81-8ac9-f4e3c65b59c3" alt="Read Docs" width="500"/></td>
             <td><img src="https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/0f483bae-ffaf-4311-8653-c0dc64fb5ebe" alt="Coding Assistant" width="500"/></td>   
         
           </tr>
         </table>
         
         ## Usage
-        ![options](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/317143b3-e1c4-427f-9295-b219950d755a)
+        ![options](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/9a1d53b8-b41b-47a9-bac7-341441b7d1fc)
+        
         
         ** After first click to an option that include microphone or system audio you need to stop with another click to same option.
         
         ## Installation && Run
         
         ```console
         pip3 install gpt-computer-assistant
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: gpt_computer_assistant Version: 0.2.0 Summary: GPT
+Metadata-Version: 2.1 Name: gpt_computer_assistant Version: 0.3.0 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant Author: Onur
 Atakan ULUSOY Author-email: atadogan06@gmail.com License: MIT Description: #
 GPT Computer Assistant Hi, this is an unofficial work for providing ChatGPT
 MacOS app to Windows and Linux. In this way this is a fresh and stable work.
 You can easily install as Python library for this time but we will prepare a
 pipeline to providing native install scripts (.exe). ![intro](https://
 github.com/onuratakan/gpt-computer-assistant/assets/41792982/d44d0efd-7354-
 4139-bae5-5fcfa97c48a2) ## Capabilities At this time we have many
 infrastructure element. We just aim to provide whole thinks that already in
 ChatGPT app. - **Screen Read** - Microphone - **System Audio** - Memory -- -
 **Clipboard** - Search Engines - **Python and SH Interpreters** - Writing and
 Running Scripts - Using your Telegram Account - Knowledge Management #### Todo
-- [x] Reset Option - [ ] Splitting long audios. (Whisper api just support
-<20mb) - [ ] More Effect - [ ] Windows .exe - [ ] Linux native - [ ] MacOS
-native ## Use cases
+- [x] Reset Option - [x] Splitting long audios. (Whisper api just support
+<20mb) - [x] Text input area - [ ] More Effect - [ ] Windows .exe - [ ] Linux
+native - [ ] MacOS native ## Use cases
 [Take Meeting Notes] [Daily Assistant]
 [Read Docs]          [Coding Assistant]
 ## Usage ![options](https://github.com/onuratakan/gpt-computer-assistant/
-assets/41792982/317143b3-e1c4-427f-9295-b219950d755a) ** After first click to
+assets/41792982/9a1d53b8-b41b-47a9-bac7-341441b7d1fc) ** After first click to
 an option that include microphone or system audio you need to stop with another
 click to same option. ## Installation && Run ```console pip3 install gpt-
 computer-assistant ``` ```console computerassistant ``` Platform: UNKNOWN
 Requires-Python: >= 3 Description-Content-Type: text/markdown
```

### Comparing `gpt_computer_assistant-0.2.0/README.md` & `gpt_computer_assistant-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,16 @@
  - Writing and Running Scripts
  - Using your Telegram Account
  - Knowledge Management
 
 
 #### Todo
 - [x] Reset Option
-- [ ] Splitting long audios. (Whisper api just support <20mb)
+- [x] Splitting long audios. (Whisper api just support <20mb)
+- [x] Text input area
 - [ ] More Effect
 
 - [ ] Windows .exe
 - [ ] Linux native
 - [ ] MacOS native
 
 
@@ -43,15 +44,16 @@
     <td><img src="https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/10b69a18-033c-4d81-8ac9-f4e3c65b59c3" alt="Read Docs" width="500"/></td>
     <td><img src="https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/0f483bae-ffaf-4311-8653-c0dc64fb5ebe" alt="Coding Assistant" width="500"/></td>   
 
   </tr>
 </table>
 
 ## Usage
-![options](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/317143b3-e1c4-427f-9295-b219950d755a)
+![options](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/9a1d53b8-b41b-47a9-bac7-341441b7d1fc)
+
 
 ** After first click to an option that include microphone or system audio you need to stop with another click to same option.
 
 ## Installation && Run
 
 ```console
 pip3 install gpt-computer-assistant
```

#### html2text {}

```diff
@@ -4,17 +4,17 @@
 pipeline to providing native install scripts (.exe). ![intro](https://
 github.com/onuratakan/gpt-computer-assistant/assets/41792982/d44d0efd-7354-
 4139-bae5-5fcfa97c48a2) ## Capabilities At this time we have many
 infrastructure element. We just aim to provide whole thinks that already in
 ChatGPT app. - **Screen Read** - Microphone - **System Audio** - Memory -- -
 **Clipboard** - Search Engines - **Python and SH Interpreters** - Writing and
 Running Scripts - Using your Telegram Account - Knowledge Management #### Todo
-- [x] Reset Option - [ ] Splitting long audios. (Whisper api just support
-<20mb) - [ ] More Effect - [ ] Windows .exe - [ ] Linux native - [ ] MacOS
-native ## Use cases
+- [x] Reset Option - [x] Splitting long audios. (Whisper api just support
+<20mb) - [x] Text input area - [ ] More Effect - [ ] Windows .exe - [ ] Linux
+native - [ ] MacOS native ## Use cases
 [Take Meeting Notes] [Daily Assistant]
 [Read Docs]          [Coding Assistant]
 ## Usage ![options](https://github.com/onuratakan/gpt-computer-assistant/
-assets/41792982/317143b3-e1c4-427f-9295-b219950d755a) ** After first click to
+assets/41792982/9a1d53b8-b41b-47a9-bac7-341441b7d1fc) ** After first click to
 an option that include microphone or system audio you need to stop with another
 click to same option. ## Installation && Run ```console pip3 install gpt-
 computer-assistant ``` ```console computerassistant ```
```

### Comparing `gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/agent.py` & `gpt_computer_assistant-0.3.0/gpt_computer_assistant/agent/agent.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/assistant.py` & `gpt_computer_assistant-0.3.0/gpt_computer_assistant/agent/assistant.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/background.py` & `gpt_computer_assistant-0.3.0/gpt_computer_assistant/agent/background.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.2.0/gpt_computer_assistant/agent/proccess.py` & `gpt_computer_assistant-0.3.0/gpt_computer_assistant/agent/proccess.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from ..llm import *
 from .assistant import *
 
 from .chat_history import *
 
 from ..audio.tts import text_to_speech
+from ..audio.stt import speech_to_text
 
 from ..audio.record import audio_data
 
 
 from ..gui.signal import signal_handler
 
 import threading
@@ -25,26 +26,19 @@
 
 
 def process_audio(take_screenshot=True, take_system_audio=False):
     global audio_data
 
     
 
-    audio_file = open(mic_record_location, "rb")
-    transcription = get_client().audio.transcriptions.create(
-        model="whisper-1",
-        file=audio_file
-    )
+    transcription = speech_to_text(mic_record_location)
 
     if take_system_audio:
-        audio_file2 = open(system_sound_location, "rb")
-        transcription2 = get_client().audio.transcriptions.create(
-            model="whisper-1",
-            file=audio_file2
-        )
+
+        transcription2 = speech_to_text(system_sound_location)
 
     
     llm_input = "USER: "+transcription.text
 
     if take_system_audio:
         llm_input += " \n Other of USER: "+transcription2.text
 
@@ -106,7 +100,44 @@
         mixer.music.play()
         while mixer.music.get_busy():
             time.sleep(0.1)
         signal_handler.assistant_response_stopped.emit()
     
     playback_thread = threading.Thread(target=play_audio)
     playback_thread.start()
+
+
+
+
+def process_text(text):
+
+
+    
+    llm_input = "USER: "+text
+
+
+
+    llm_output = assistant(llm_input, chat_message_history.messages, get_client(), screenshot_path=None)
+
+
+
+
+
+    chat_message_history.add_message(llm_output[-1])
+    llm_output = llm_output[-1].content
+
+
+    response_path = text_to_speech(llm_output)
+
+
+    signal_handler.assistant_response_ready.emit()
+
+    def play_audio():
+        mixer.init()
+        mixer.music.load(response_path)
+        mixer.music.play()
+        while mixer.music.get_busy():
+            time.sleep(0.1)
+        signal_handler.assistant_response_stopped.emit()
+    
+    playback_thread = threading.Thread(target=play_audio)
+    playback_thread.start()
```

### Comparing `gpt_computer_assistant-0.2.0/gpt_computer_assistant/audio/record.py` & `gpt_computer_assistant-0.3.0/gpt_computer_assistant/audio/record.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.2.0/gpt_computer_assistant/audio/tts.py` & `gpt_computer_assistant-0.3.0/gpt_computer_assistant/audio/tts.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.2.0/gpt_computer_assistant/gpt_computer_assistant.py` & `gpt_computer_assistant-0.3.0/gpt_computer_assistant/gpt_computer_assistant.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from .llm import *
 from .agent.agent import *
 from .agent.background import *
 
 from .gui.signal import *
 from .gui.button import *
 
+from .utils.db import *
+
 import hashlib
 import sys
 import threading
 import base64
 import time
 import random
 import numpy as np
@@ -27,36 +29,39 @@
 from PyQt5.QtWidgets import QShortcut
 import os
 import scipy.io.wavfile as wavfile
 
 from PyQt5.QtWidgets import QApplication, QMainWindow, QVBoxLayout, QWidget, QPushButton, QLabel, QHBoxLayout
 from PyQt5.QtCore import Qt, QPoint
 
-
-
-
+from PyQt5.QtWidgets import QDialog, QVBoxLayout, QLabel, QLineEdit, QPushButton
+from PyQt5 import QtWidgets, QtGui
+from PyQt5.QtGui import QIcon
 
 
 
 
 
 
 print("Imported all libraries")
 
 
 
+from PyQt5 import QtCore
 
 
 
 
 
-
-
-
-
+try:
+    import ctypes
+    myappid = 'onuratakan.gpt_computer_assistant.gui.1' # arbitrary string
+    ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
+except:
+    pass
 
 
 
 class MainWindow(QMainWindow):
     def __init__(self):
         super().__init__()
         self.setWindowFlags(Qt.FramelessWindowHint | Qt.WindowStaysOnTopHint)  # Remove title bar and set window to always on top
@@ -64,42 +69,54 @@
         self.state = 'idle'  # Possible states: 'idle', 'talking', 'thinking'
         self.pulse_timer = None
         self.initUI()
         self.button_handler = ButtonHandler(self)  # Pass the whole MainWindow object
         self.old_position = self.pos()  # For moving window
 
     def initUI(self):
-        self.setWindowTitle('GPT-4o Assistant')
-        self.setGeometry(100, 100, 200, 135)  # Adjust the size as needed
+        self.setWindowTitle('GPT-4o')
+        self.setGeometry(100, 100, 200, 200)  # Adjust the size as needed
+        
+
+        app_icon = QtGui.QIcon()
+        app_icon.addFile(icon_16_path, QtCore.QSize(16,16))
+        app_icon.addFile(icon_24_path, QtCore.QSize(24,24))
+        app_icon.addFile(icon_32_path, QtCore.QSize(32,32))
+        app_icon.addFile(icon_48_path, QtCore.QSize(48,48))
+        app_icon.addFile(icon_256_path, QtCore.QSize(256,256))
+        self.setWindowIcon(app_icon)
+
         central_widget = QWidget(self)
         self.setCentralWidget(central_widget)
         layout = QVBoxLayout(central_widget)
 
         # Custom title bar
         self.title_bar = QWidget(self)
         self.title_bar.setFixedHeight(20)  # Set a fixed height for the title bar
         self.title_bar_layout = QHBoxLayout(self.title_bar)
         self.title_bar_layout.setContentsMargins(0, 0, 0, 0)
         self.title_bar_layout.setSpacing(0)
 
-        self.title_label = QLabel("GPT-4o Assistant", self)
+        self.title_label = QLabel("GPT-4o", self)
         self.title_bar_layout.addWidget(self.title_label)
 
         self.close_button = QPushButton("X", self)
         self.close_button.setFixedSize(20, 20)
         self.close_button.clicked.connect(self.close)
         self.title_bar_layout.addWidget(self.close_button)
 
 
         layout.addWidget(self.title_bar)
 
         # Add other UI elements below the title bar
         self.other_widget = QWidget(self)
         layout.addWidget(self.other_widget)
 
+        self.layout = layout
+
         self.setLayout(layout)
 
         # Add keyboard shortcuts
         self.shortcut_screenshot = QShortcut(QKeySequence("Ctrl+1"), self)
         self.shortcut_screenshot.activated.connect(lambda: self.button_handler.just_screenshot())        
         self.shortcut_screenshot = QShortcut(QKeySequence("Ctrl+2"), self)
         self.shortcut_screenshot.activated.connect(lambda: self.button_handler.toggle_recording(take_system_audio=True))
@@ -107,14 +124,43 @@
         self.shortcut_no_screenshot = QShortcut(QKeySequence("Ctrl+e"), self)
         self.shortcut_no_screenshot.activated.connect(lambda: self.button_handler.toggle_recording(take_system_audio=True))
 
         self.shortcut_no_screenshot = QShortcut(QKeySequence("Ctrl+3"), self)
         self.shortcut_no_screenshot.activated.connect(lambda: self.button_handler.toggle_recording(no_screenshot=True))
 
 
+
+        # I want to create a input box to bottom left and a send button to bottom right
+
+        input_box = QLineEdit(self)
+        input_box.setPlaceholderText("Type here")
+        input_box.setGeometry(30, self.height() - 60, 200, 30)
+
+        send_button = QPushButton("Send", self)
+        send_button.setGeometry(self.width() - 100, self.height() - 60, 70, 30)
+
+        def input_box_send():
+            if input_box.text() != "":
+                self.button_handler.input_text(input_box.text())
+                input_box.setText("")
+                
+
+
+        # send button should trig button handler input_text function
+        send_button.clicked.connect(input_box_send)
+
+        self.layout.addWidget(input_box)
+        self.layout.addWidget(send_button)
+
+        # Also if the input box is not empty and enter is pressed, it should also trigger the send button
+        input_box.returnPressed.connect(input_box_send)
+
+
+
+
         self.show()
 
     def mousePressEvent(self, event: QMouseEvent):
         if event.button() == Qt.LeftButton:
             self.old_position = event.globalPos()
 
     def mouseMoveEvent(self, event: QMouseEvent):
@@ -147,25 +193,25 @@
             radius = 70
             painter.drawEllipse(int(center_x - radius / 2), int(center_y - radius / 2), int(radius), int(radius))
         
         self.circle_rect = QRect(int(center_x - radius / 2), int(center_y - radius / 2), int(radius), int(radius))
 
         # Draw second smaller circle button at bottom right
         small_center_x = self.width() - 30
-        small_center_y = self.height() - 30
+        small_center_y = self.height() - 90
         small_radius = 25
         painter.drawEllipse(int(small_center_x - small_radius / 2), int(small_center_y - small_radius / 2), int(small_radius), int(small_radius))
         
         self.small_circle_rect = QRect(int(small_center_x - small_radius / 2), int(small_center_y - small_radius / 2), int(small_radius), int(small_radius))
 
 
 
         # Draw second smaller circle button at bottom left
         small_center_x = 30  # Adjust this line
-        small_center_y = self.height() - 30
+        small_center_y = self.height() - 90
         small_radius = 25
         painter.drawEllipse(int(small_center_x - small_radius / 2), int(small_center_y - small_radius / 2), int(small_radius), int(small_radius))
 
         self.small_circle_left = QRect(int(small_center_x - small_radius / 2), int(small_center_y - small_radius / 2), int(small_radius), int(small_radius))
 
 
         # Draw second smaller circle button at top left
@@ -184,14 +230,15 @@
         painter.drawRect(int(small_center_x - small_radius / 2), int(small_center_y - small_radius / 2), int(small_radius), int(small_radius))
 
         self.small_rect_right_top = QRect(int(small_center_x - small_radius / 2), int(small_center_y - small_radius / 2), int(small_radius), int(small_radius))
         
 
 
 
+
     def update_state(self, new_state):
         self.state = new_state
         print(f"State updated: {new_state}")
         if new_state == 'talking':
             self.pulse_frame = 0
             if self.pulse_timer:
                 self.pulse_timer.stop()
```

### Comparing `gpt_computer_assistant-0.2.0/gpt_computer_assistant/gui/button.py` & `gpt_computer_assistant-0.3.0/gpt_computer_assistant/gui/button.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,7 +117,16 @@
         reset_memory_button.clicked.connect(clear_chat_history)
         settings_dialog.layout().addWidget(reset_memory_button)
 
 
         settings_dialog.exec_()
         settings_dialog.show()
 
+
+
+    def input_text(self, text):
+        
+        self.main_window.update_state('thinking')
+        if self.process_audio_thread is None or not self.process_audio_thread.is_alive():
+            signal_handler.assistant_thinking.emit()
+            self.process_audio_thread = threading.Thread(target=process_text, args=(text,))
+            self.process_audio_thread.start()
```

### Comparing `gpt_computer_assistant-0.2.0/gpt_computer_assistant/utils/db.py` & `gpt_computer_assistant-0.3.0/gpt_computer_assistant/utils/db.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from dotenv import load_dotenv
 load_dotenv(".env")
 
 currently_dir  = os.path.dirname(os.path.abspath(__file__))
 
 artifacts_dir = os.path.join(currently_dir, "artifacts")
+media_dir = os.path.join(currently_dir, "media")
 
 if not os.path.exists(artifacts_dir):
     os.makedirs(artifacts_dir)
 
 mic_record_location = os.path.join(artifacts_dir, "mic_record.wav")
 
 system_sound_location = os.path.join(artifacts_dir, "system_sound.wav")
@@ -36,8 +37,15 @@
             env = os.getenv("OPENAI_API_KEY")
             if env:
                 save_api_key(env)
                 return env
             else:
                 return "CHANGE_ME"
         with open(openaikey, 'r') as f:
-            return f.read()
+            return f.read()
+        
+
+icon_16_path = os.path.join(media_dir, "icon_16.png")
+icon_24_path = os.path.join(media_dir, "icon_24.png")
+icon_32_path = os.path.join(media_dir, "icon_32.png")
+icon_48_path = os.path.join(media_dir, "icon_48.png")
+icon_256_path = os.path.join(media_dir, "icon_256.png")
```

### Comparing `gpt_computer_assistant-0.2.0/gpt_computer_assistant.egg-info/PKG-INFO` & `gpt_computer_assistant-0.3.0/gpt_computer_assistant.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-computer-assistant
-Version: 0.2.0
+Version: 0.3.0
 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # GPT Computer Assistant
         Hi, this is an unofficial work for providing ChatGPT MacOS app to Windows and Linux. In this way this is a fresh and stable work. You can easily install as Python library for this time but we will prepare a pipeline to providing native install scripts (.exe).
@@ -28,15 +28,16 @@
          - Writing and Running Scripts
          - Using your Telegram Account
          - Knowledge Management
         
         
         #### Todo
         - [x] Reset Option
-        - [ ] Splitting long audios. (Whisper api just support <20mb)
+        - [x] Splitting long audios. (Whisper api just support <20mb)
+        - [x] Text input area
         - [ ] More Effect
         
         - [ ] Windows .exe
         - [ ] Linux native
         - [ ] MacOS native
         
         
@@ -51,15 +52,16 @@
             <td><img src="https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/10b69a18-033c-4d81-8ac9-f4e3c65b59c3" alt="Read Docs" width="500"/></td>
             <td><img src="https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/0f483bae-ffaf-4311-8653-c0dc64fb5ebe" alt="Coding Assistant" width="500"/></td>   
         
           </tr>
         </table>
         
         ## Usage
-        ![options](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/317143b3-e1c4-427f-9295-b219950d755a)
+        ![options](https://github.com/onuratakan/gpt-computer-assistant/assets/41792982/9a1d53b8-b41b-47a9-bac7-341441b7d1fc)
+        
         
         ** After first click to an option that include microphone or system audio you need to stop with another click to same option.
         
         ## Installation && Run
         
         ```console
         pip3 install gpt-computer-assistant
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: gpt-computer-assistant Version: 0.2.0 Summary: GPT
+Metadata-Version: 2.1 Name: gpt-computer-assistant Version: 0.3.0 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant Author: Onur
 Atakan ULUSOY Author-email: atadogan06@gmail.com License: MIT Description: #
 GPT Computer Assistant Hi, this is an unofficial work for providing ChatGPT
 MacOS app to Windows and Linux. In this way this is a fresh and stable work.
 You can easily install as Python library for this time but we will prepare a
 pipeline to providing native install scripts (.exe). ![intro](https://
 github.com/onuratakan/gpt-computer-assistant/assets/41792982/d44d0efd-7354-
 4139-bae5-5fcfa97c48a2) ## Capabilities At this time we have many
 infrastructure element. We just aim to provide whole thinks that already in
 ChatGPT app. - **Screen Read** - Microphone - **System Audio** - Memory -- -
 **Clipboard** - Search Engines - **Python and SH Interpreters** - Writing and
 Running Scripts - Using your Telegram Account - Knowledge Management #### Todo
-- [x] Reset Option - [ ] Splitting long audios. (Whisper api just support
-<20mb) - [ ] More Effect - [ ] Windows .exe - [ ] Linux native - [ ] MacOS
-native ## Use cases
+- [x] Reset Option - [x] Splitting long audios. (Whisper api just support
+<20mb) - [x] Text input area - [ ] More Effect - [ ] Windows .exe - [ ] Linux
+native - [ ] MacOS native ## Use cases
 [Take Meeting Notes] [Daily Assistant]
 [Read Docs]          [Coding Assistant]
 ## Usage ![options](https://github.com/onuratakan/gpt-computer-assistant/
-assets/41792982/317143b3-e1c4-427f-9295-b219950d755a) ** After first click to
+assets/41792982/9a1d53b8-b41b-47a9-bac7-341441b7d1fc) ** After first click to
 an option that include microphone or system audio you need to stop with another
 click to same option. ## Installation && Run ```console pip3 install gpt-
 computer-assistant ``` ```console computerassistant ``` Platform: UNKNOWN
 Requires-Python: >= 3 Description-Content-Type: text/markdown
```

### Comparing `gpt_computer_assistant-0.2.0/setup.py` & `gpt_computer_assistant-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 with open('requirements.txt') as fp:
     install_requires = fp.read()
 setup(
     name="gpt_computer_assistant",
-    version="0.2.0",
+    version="0.3.0",
     description="""GPT""",
     long_description="".join(open("README.md", encoding="utf-8").readlines()),
     long_description_content_type="text/markdown",
     url="https://github.com/onuratakan/gpt-computer-assistant",
     author="Onur Atakan ULUSOY",
     author_email="atadogan06@gmail.com",
     license="MIT",
```

