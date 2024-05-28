# Comparing `tmp/wi1-bot-1.4.4.tar.gz` & `tmp/wi1-bot-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wi1-bot-1.4.4.tar", last modified: Sun May 26 05:31:28 2024, max compression
+gzip compressed data, was "wi1-bot-1.4.5.tar", last modified: Tue May 28 02:08:36 2024, max compression
```

## Comparing `wi1-bot-1.4.4.tar` & `wi1-bot-1.4.5.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.758413 wi1-bot-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.750413 wi1-bot-1.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.750413 wi1-bot-1.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-26 05:31:28.758413 wi1-bot-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/compose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/config.yaml.template
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 05:31:28.758413 wi1-bot-1.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/tests/movie_downloaded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-26 05:31:27.000000 wi1-bot-1.4.4/wi1_bot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot/arr/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/arr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/arr/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/arr/episode.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/arr/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/arr/radarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/arr/sonarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot/discord/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/discord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot/discord/cogs/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/discord/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/discord/cogs/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/discord/cogs/series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/discord/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/push.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/scripts/add_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/scripts/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/scripts/transcode_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot/transcoder/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/transcoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/transcoder/transcode_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/transcoder/transcoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-26 05:31:28.000000 wi1-bot-1.4.4/wi1_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-26 05:31:28.000000 wi1-bot-1.4.4/wi1_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 05:31:28.000000 wi1-bot-1.4.4/wi1_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-26 05:31:28.000000 wi1-bot-1.4.4/wi1_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-26 05:31:28.000000 wi1-bot-1.4.4/wi1_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-26 05:31:28.000000 wi1-bot-1.4.4/wi1_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.836720 wi1-bot-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.828720 wi1-bot-1.4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.828720 wi1-bot-1.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.828720 wi1-bot-1.4.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-28 02:08:36.836720 wi1-bot-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/config.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 02:08:36.836720 wi1-bot-1.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.828720 wi1-bot-1.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/tests/movie_downloaded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.828720 wi1-bot-1.4.5/wi1_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 02:08:35.000000 wi1-bot-1.4.5/wi1_bot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.832720 wi1-bot-1.4.5/wi1_bot/arr/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/arr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/arr/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/arr/episode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/arr/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/arr/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/arr/sonarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.832720 wi1-bot-1.4.5/wi1_bot/discord/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/discord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.832720 wi1-bot-1.4.5/wi1_bot/discord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/discord/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/discord/cogs/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/discord/cogs/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/discord/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/push.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.832720 wi1-bot-1.4.5/wi1_bot/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/scripts/add_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/scripts/rescan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/scripts/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/scripts/transcode_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.832720 wi1-bot-1.4.5/wi1_bot/transcoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/transcoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/transcoder/transcode_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/transcoder/transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.832720 wi1-bot-1.4.5/wi1_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-28 02:08:36.000000 wi1-bot-1.4.5/wi1_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 02:08:36.000000 wi1-bot-1.4.5/wi1_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 02:08:36.000000 wi1-bot-1.4.5/wi1_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 02:08:36.000000 wi1-bot-1.4.5/wi1_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-28 02:08:36.000000 wi1-bot-1.4.5/wi1_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 02:08:36.000000 wi1-bot-1.4.5/wi1_bot.egg-info/top_level.txt
```

### Comparing `wi1-bot-1.4.4/.github/workflows/pypi-publish.yml` & `wi1-bot-1.4.5/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/LICENSE` & `wi1-bot-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/PKG-INFO` & `wi1-bot-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.4.4
+Version: 1.4.5
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
```

### Comparing `wi1-bot-1.4.4/README.md` & `wi1-bot-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/config.yaml.template` & `wi1-bot-1.4.5/config.yaml.template`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/pyproject.toml` & `wi1-bot-1.4.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 [project.urls]
 Homepage = "https://github.com/wthueb/wi1-bot"
 
 [project.scripts]
 wi1-bot = "wi1_bot.scripts.start:main"
 transcode-item = "wi1_bot.scripts.transcode_item:main"
 add-tag = "wi1_bot.scripts.add_tag:main"
+rescan = "wi1_bot.scripts.rescan:main"
 
 [project.optional-dependencies]
 dev = [
     "mongo-types==0.15.1",
     "mypy==1.3.0",
     "pre-commit==3.6.2",
     "ruff==0.3.0",
```

### Comparing `wi1-bot-1.4.4/wi1_bot/arr/download.py` & `wi1-bot-1.4.5/wi1_bot/arr/download.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/arr/episode.py` & `wi1-bot-1.4.5/wi1_bot/arr/episode.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/arr/movie.py` & `wi1-bot-1.4.5/wi1_bot/arr/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/arr/radarr.py` & `wi1-bot-1.4.5/wi1_bot/arr/radarr.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,18 +145,18 @@
                 name = profile["name"]
                 assert isinstance(name, str)
                 return name
 
         raise ValueError(f"no quality profile with the id {profile_id}")
 
     def rescan_movie(self, movie_id: int) -> None:
-        self._radarr.post_command("RescanMovie", movieId=movie_id)  # type: ignore
+        self._radarr.post_command("RescanMovie", movieId=movie_id)
 
     def refresh_movie(self, movie_id: int) -> None:
-        self._radarr.post_command("RefreshMovie", movieIds=[movie_id])  # type: ignore
+        self._radarr.post_command("RefreshMovie", movieIds=[movie_id])
 
     def search_missing(self) -> None:
         self._radarr.post_command(name="MissingMoviesSearch")
 
     def _get_quality_profile_id(self, name: str) -> int:
         profiles = self._radarr.get_quality_profile()
```

### Comparing `wi1-bot-1.4.4/wi1_bot/arr/sonarr.py` & `wi1-bot-1.4.5/wi1_bot/arr/sonarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/config.py` & `wi1-bot-1.4.5/wi1_bot/config.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/discord/bot.py` & `wi1-bot-1.4.5/wi1_bot/discord/bot.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/discord/cogs/movie.py` & `wi1-bot-1.4.5/wi1_bot/discord/cogs/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/discord/cogs/series.py` & `wi1-bot-1.4.5/wi1_bot/discord/cogs/series.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/discord/helpers.py` & `wi1-bot-1.4.5/wi1_bot/discord/helpers.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/push.py` & `wi1-bot-1.4.5/wi1_bot/push.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/scripts/add_tag.py` & `wi1-bot-1.4.5/wi1_bot/scripts/add_tag.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/scripts/start.py` & `wi1-bot-1.4.5/wi1_bot/scripts/start.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/scripts/transcode_item.py` & `wi1-bot-1.4.5/wi1_bot/scripts/transcode_item.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/transcoder/transcode_queue.py` & `wi1-bot-1.4.5/wi1_bot/transcoder/transcode_queue.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot/transcoder/transcoder.py` & `wi1-bot-1.4.5/wi1_bot/transcoder/transcoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,40 +42,33 @@
             item = queue.get_one()
 
             if item is None:
                 sleep(3)
                 continue
 
             try:
-                self._do_transcode(item)
-                queue.remove(item)
-            except SignalInterrupt:
-                # retry when restarted
-                pass
-            except FileNotFoundError:
-                # don't retry
-                queue.remove(item)
-            except UnknownError:
-                # don't retry
-                queue.remove(item)
+                remove = self._do_transcode(item)
+
+                if remove:
+                    queue.remove(item)
             except Exception:
                 self.logger.warning(
                     "got exception when trying to transcode", exc_info=True
                 )
 
             sleep(3)
 
-    def _do_transcode(self, item: TranscodeItem) -> None:
+    def _do_transcode(self, item: TranscodeItem) -> bool:
         path = pathlib.Path(item.path)
 
-        self.logger.debug(f"attempting to transcode {path.name}")
+        self.logger.info(f"attempting to transcode {path.name}")
 
         if path.suffix == ".avi":
-            self.logger.debug(f"cannot transcode {path.name}: .avi not supported")
-            return
+            self.logger.info(f"cannot transcode {path.name}: .avi not supported")
+            return True
 
         # push.send(f"{basename}", title="starting transcode")
 
         # TODO: calculate compression amount
         # 1 - (video bitrate + audio bitrate) * duration / size
         # if compression amount > config value, transcode
         # else, don't transcode
@@ -99,76 +92,82 @@
             bufsize=1,
         ) as proc:
             last_output = ""
 
             tmp_log_path = tmp_folder / "wi1_bot.transcoder.log"
 
             with open(tmp_log_path, "w") as ffmpeg_log_file:
-                for line in proc.stdout:  # type: ignore
+                assert proc.stdout is not None
+                for line in proc.stdout:
                     ffmpeg_log_file.write(line)
                     last_output = line.strip()
 
             status = proc.wait()
 
             if status != 0:
-                self.logger.error(f"ffmpeg failed (status {status}): {last_output}")
-
-                if (
-                    "No such file or directory" in last_output
-                    and "shared object file" not in last_output
-                ):
-                    self.logger.debug(
+                if "Error opening input files" in last_output:
+                    self.logger.info(
                         f"file does not exist: {path}, skipping transcoding"
                     )
-                    raise FileNotFoundError
+                    return True
 
                 if "received signal 15" in last_output:
-                    self.logger.debug(
+                    self.logger.info(
                         f"transcoding interrupted by signal: {path}, will retry"
                     )
-                    raise SignalInterrupt
+                    return False
+
+                if "cannot open shared object file" in last_output:
+                    self.logger.error(
+                        "ffmpeg error: missing shared object file, will retry"
+                    )
+                    push.send(f"ffmpeg error: {last_output}", title="ffmpeg error")
+                    return False
 
                 perm_log_path = tmp_folder / f"{path.stem}.log"
 
                 if "general" in config and "log_dir" in config["general"]:
                     log_dir = pathlib.Path(config["general"]["log_dir"]).resolve()
 
                     perm_log_path = log_dir / "transcoder-errors" / f"{path.stem}.log"
                     perm_log_path.parent.mkdir(parents=True, exist_ok=True)
 
                 shutil.copy(tmp_log_path, perm_log_path)
+
+                self.logger.error(f"ffmpeg failed (status {status}): {last_output}")
                 self.logger.error(f"log file: {perm_log_path}")
 
                 push.send(
                     f"{path.name} has failed to transcode, log: {perm_log_path}",
                     title="transcoding error",
                 )
 
-                raise UnknownError
+                return True
 
         new_path = path.parent / transcode_to.name
 
         if not path.exists():
             self.logger.debug(
                 f"file doesn't exist: {item.path}, deleting transcoded file"
             )
 
             transcode_to.unlink()
-            return
+            return True
 
         shutil.move(transcode_to, new_path)
         path.unlink()
 
         self._rescan_content(item, str(new_path))
 
         self.logger.info(f"transcoded: {path.name} -> {new_path.name}")
         # push.send(f"{path.name} -> {new_path.name}", title="file transcoded")
 
+        return True
+
     def _rescan_content(self, item: TranscodeItem, new_path: str) -> None:
-        # FIXME: don't hardcode library paths (config)
         if item.content_id is not None:
             if new_path.startswith(config["radarr"]["root_folder"]):
                 self.radarr.rescan_movie(item.content_id)
                 # radarr bug that it doesn't see the deleted file and the new file
                 # in one rescan?
                 # have to sleep in between to ensure initial command finishes
                 # or use pyarr.get_command() to see command status
```

### Comparing `wi1-bot-1.4.4/wi1_bot/webhook.py` & `wi1-bot-1.4.5/wi1_bot/webhook.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.4/wi1_bot.egg-info/PKG-INFO` & `wi1-bot-1.4.5/wi1_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.4.4
+Version: 1.4.5
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
```

### Comparing `wi1-bot-1.4.4/wi1_bot.egg-info/SOURCES.txt` & `wi1-bot-1.4.5/wi1_bot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,12 +33,13 @@
 wi1_bot/discord/bot.py
 wi1_bot/discord/helpers.py
 wi1_bot/discord/cogs/__init__.py
 wi1_bot/discord/cogs/movie.py
 wi1_bot/discord/cogs/series.py
 wi1_bot/scripts/__init__.py
 wi1_bot/scripts/add_tag.py
+wi1_bot/scripts/rescan.py
 wi1_bot/scripts/start.py
 wi1_bot/scripts/transcode_item.py
 wi1_bot/transcoder/__init__.py
 wi1_bot/transcoder/transcode_queue.py
 wi1_bot/transcoder/transcoder.py
```

