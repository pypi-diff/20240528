# Comparing `tmp/synapse_super_invites-0.8.2.tar.gz` & `tmp/synapse_super_invites-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapse_super_invites-0.8.2.tar", last modified: Sat May 11 20:32:12 2024, max compression
+gzip compressed data, was "synapse_super_invites-0.8.3.tar", last modified: Tue May 28 17:25:57 2024, max compression
```

## Comparing `synapse_super_invites-0.8.2.tar` & `synapse_super_invites-0.8.3.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.052097 synapse_super_invites-0.8.2/
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.045431 synapse_super_invites-0.8.2/.github/
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/.github/workflows/
--rw-r--r--   0 ben       (1001) ben       (1001)     1094 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.2/.github/workflows/ci.yml
--rw-r--r--   0 ben       (1001) ben       (1001)     1786 2023-11-17 16:09:10.000000 synapse_super_invites-0.8.2/.github/workflows/release.yml
--rw-r--r--   0 ben       (1001) ben       (1001)      105 2023-11-17 14:46:55.000000 synapse_super_invites-0.8.2/.gitignore
--rw-r--r--   0 ben       (1001) ben       (1001)      805 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.2/.gitlab-ci.yml
--rw-r--r--   0 ben       (1001) ben       (1001)     4107 2024-05-11 20:32:12.052097 synapse_super_invites-0.8.2/PKG-INFO
--rw-r--r--   0 ben       (1001) ben       (1001)     3230 2024-05-11 20:28:53.000000 synapse_super_invites-0.8.2/README.md
--rw-r--r--   0 ben       (1001) ben       (1001)     3628 2023-11-17 16:04:33.000000 synapse_super_invites-0.8.2/alembic.ini
--rw-r--r--   0 ben       (1001) ben       (1001)      351 2023-11-15 22:30:55.000000 synapse_super_invites-0.8.2/example_server.py
--rw-r--r--   0 ben       (1001) ben       (1001)     1909 2024-05-11 20:11:27.000000 synapse_super_invites-0.8.2/pyproject.toml
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/scripts-dev/
--rwxr-xr-x   0 ben       (1001) ben       (1001)      354 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.2/scripts-dev/lint.sh
--rw-r--r--   0 ben       (1001) ben       (1001)       38 2024-05-11 20:32:12.052097 synapse_super_invites-0.8.2/setup.cfg
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites/
--rw-r--r--   0 ben       (1001) ben       (1001)     1986 2024-05-11 20:22:14.000000 synapse_super_invites-0.8.2/synapse_super_invites/__init__.py
--rw-r--r--   0 ben       (1001) ben       (1001)     3641 2023-11-17 16:04:48.000000 synapse_super_invites-0.8.2/synapse_super_invites/alembic.ini
--rw-r--r--   0 ben       (1001) ben       (1001)      681 2023-11-17 16:03:47.000000 synapse_super_invites-0.8.2/synapse_super_invites/config.py
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites/migration/
--rw-r--r--   0 ben       (1001) ben       (1001)     2302 2023-11-17 13:28:20.000000 synapse_super_invites-0.8.2/synapse_super_invites/migration/env.py
--rw-r--r--   0 ben       (1001) ben       (1001)      635 2023-11-14 17:03:24.000000 synapse_super_invites-0.8.2/synapse_super_invites/migration/script.py.mako
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites/migration/versions/
--rw-r--r--   0 ben       (1001) ben       (1001)     3218 2023-11-15 17:11:42.000000 synapse_super_invites-0.8.2/synapse_super_invites/migration/versions/25e4ec3cea32_added_token_table.py
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites/model/
--rw-r--r--   0 ben       (1001) ben       (1001)     2275 2023-11-15 17:11:42.000000 synapse_super_invites-0.8.2/synapse_super_invites/model/__init__.py
--rw-r--r--   0 ben       (1001) ben       (1001)        0 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.2/synapse_super_invites/py.typed
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites/resource/
--rw-r--r--   0 ben       (1001) ben       (1001)      238 2024-05-11 20:20:17.000000 synapse_super_invites-0.8.2/synapse_super_invites/resource/__init__.py
--rw-r--r--   0 ben       (1001) ben       (1001)     1227 2024-05-11 20:21:11.000000 synapse_super_invites-0.8.2/synapse_super_invites/resource/base.py
--rw-r--r--   0 ben       (1001) ben       (1001)     1998 2024-05-11 19:52:25.000000 synapse_super_invites-0.8.2/synapse_super_invites/resource/info.py
--rw-r--r--   0 ben       (1001) ben       (1001)     2475 2024-05-11 19:52:03.000000 synapse_super_invites-0.8.2/synapse_super_invites/resource/redeem.py
--rw-r--r--   0 ben       (1001) ben       (1001)     4790 2024-05-11 20:20:17.000000 synapse_super_invites-0.8.2/synapse_super_invites/resource/tokens.py
--rw-r--r--   0 ben       (1001) ben       (1001)     2034 2024-05-11 20:20:17.000000 synapse_super_invites-0.8.2/synapse_super_invites/resource/web_access.py
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites/static/
--rw-r--r--   0 ben       (1001) ben       (1001)      556 2023-11-15 23:09:11.000000 synapse_super_invites-0.8.2/synapse_super_invites/static/index.html
--rw-r--r--   0 ben       (1001) ben       (1001)    15721 2023-11-15 22:50:38.000000 synapse_super_invites-0.8.2/synapse_super_invites/static/pure-min.css
--rw-r--r--   0 ben       (1001) ben       (1001)       57 2023-11-15 23:06:08.000000 synapse_super_invites-0.8.2/synapse_super_invites/static/script.js
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites.egg-info/
--rw-r--r--   0 ben       (1001) ben       (1001)     4107 2024-05-11 20:32:12.000000 synapse_super_invites-0.8.2/synapse_super_invites.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1001) ben       (1001)     1198 2024-05-11 20:32:12.000000 synapse_super_invites-0.8.2/synapse_super_invites.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1001) ben       (1001)        1 2024-05-11 20:32:12.000000 synapse_super_invites-0.8.2/synapse_super_invites.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1001) ben       (1001)      135 2024-05-11 20:32:12.000000 synapse_super_invites-0.8.2/synapse_super_invites.egg-info/requires.txt
--rw-r--r--   0 ben       (1001) ben       (1001)       22 2024-05-11 20:32:12.000000 synapse_super_invites-0.8.2/synapse_super_invites.egg-info/top_level.txt
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/tests/
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/tests/.local/
--rw-r--r--   0 ben       (1001) ben       (1001)        0 2023-11-15 22:24:54.000000 synapse_super_invites-0.8.2/tests/.local/.gitkeep
--rw-r--r--   0 ben       (1001) ben       (1001)     1739 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.2/tests/__init__.py
--rw-r--r--   0 ben       (1001) ben       (1001)      844 2023-11-15 23:09:33.000000 synapse_super_invites-0.8.2/tests/example_cfg.yml
--rw-r--r--   0 ben       (1001) ben       (1001)      865 2023-11-17 13:28:20.000000 synapse_super_invites-0.8.2/tests/test_config.py
--rw-r--r--   0 ben       (1001) ben       (1001)    29983 2024-05-11 20:20:17.000000 synapse_super_invites-0.8.2/tests/test_integrations.py
--rw-r--r--   0 ben       (1001) ben       (1001)      866 2024-05-11 14:59:11.000000 synapse_super_invites-0.8.2/tox.ini
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.323228 synapse_super_invites-0.8.3/
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.316561 synapse_super_invites-0.8.3/.github/
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.316561 synapse_super_invites-0.8.3/.github/workflows/
+-rw-r--r--   0 ben       (1001) ben       (1001)     1094 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.3/.github/workflows/ci.yml
+-rw-r--r--   0 ben       (1001) ben       (1001)     1786 2023-11-17 16:09:10.000000 synapse_super_invites-0.8.3/.github/workflows/release.yml
+-rw-r--r--   0 ben       (1001) ben       (1001)      105 2023-11-17 14:46:55.000000 synapse_super_invites-0.8.3/.gitignore
+-rw-r--r--   0 ben       (1001) ben       (1001)      805 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.3/.gitlab-ci.yml
+-rw-r--r--   0 ben       (1001) ben       (1001)     4517 2024-05-28 17:25:57.323228 synapse_super_invites-0.8.3/PKG-INFO
+-rw-r--r--   0 ben       (1001) ben       (1001)     3640 2024-05-28 17:23:37.000000 synapse_super_invites-0.8.3/README.md
+-rw-r--r--   0 ben       (1001) ben       (1001)     3642 2024-05-28 16:37:05.000000 synapse_super_invites-0.8.3/alembic.ini
+-rw-r--r--   0 ben       (1001) ben       (1001)      351 2023-11-15 22:30:55.000000 synapse_super_invites-0.8.3/example_server.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     1909 2024-05-11 20:11:27.000000 synapse_super_invites-0.8.3/pyproject.toml
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.316561 synapse_super_invites-0.8.3/scripts-dev/
+-rwxr-xr-x   0 ben       (1001) ben       (1001)      354 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.3/scripts-dev/lint.sh
+-rw-r--r--   0 ben       (1001) ben       (1001)       38 2024-05-28 17:25:57.323228 synapse_super_invites-0.8.3/setup.cfg
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.316561 synapse_super_invites-0.8.3/synapse_super_invites/
+-rw-r--r--   0 ben       (1001) ben       (1001)     1986 2024-05-28 17:24:54.000000 synapse_super_invites-0.8.3/synapse_super_invites/__init__.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     3641 2023-11-17 16:04:48.000000 synapse_super_invites-0.8.3/synapse_super_invites/alembic.ini
+-rw-r--r--   0 ben       (1001) ben       (1001)      681 2023-11-17 16:03:47.000000 synapse_super_invites-0.8.3/synapse_super_invites/config.py
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.319894 synapse_super_invites-0.8.3/synapse_super_invites/migration/
+-rw-r--r--   0 ben       (1001) ben       (1001)     2302 2023-11-17 13:28:20.000000 synapse_super_invites-0.8.3/synapse_super_invites/migration/env.py
+-rw-r--r--   0 ben       (1001) ben       (1001)      635 2023-11-14 17:03:24.000000 synapse_super_invites-0.8.3/synapse_super_invites/migration/script.py.mako
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.319894 synapse_super_invites-0.8.3/synapse_super_invites/migration/versions/
+-rw-r--r--   0 ben       (1001) ben       (1001)     3218 2023-11-15 17:11:42.000000 synapse_super_invites-0.8.3/synapse_super_invites/migration/versions/25e4ec3cea32_added_token_table.py
+-rw-r--r--   0 ben       (1001) ben       (1001)      822 2024-05-28 16:39:39.000000 synapse_super_invites-0.8.3/synapse_super_invites/migration/versions/8c8c90d89eac_add_error_logs_to_acceptance.py
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.319894 synapse_super_invites-0.8.3/synapse_super_invites/model/
+-rw-r--r--   0 ben       (1001) ben       (1001)     2344 2024-05-28 16:38:47.000000 synapse_super_invites-0.8.3/synapse_super_invites/model/__init__.py
+-rw-r--r--   0 ben       (1001) ben       (1001)        0 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.3/synapse_super_invites/py.typed
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.319894 synapse_super_invites-0.8.3/synapse_super_invites/resource/
+-rw-r--r--   0 ben       (1001) ben       (1001)      238 2024-05-11 20:20:17.000000 synapse_super_invites-0.8.3/synapse_super_invites/resource/__init__.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     1227 2024-05-11 20:21:11.000000 synapse_super_invites-0.8.3/synapse_super_invites/resource/base.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     1998 2024-05-11 19:52:25.000000 synapse_super_invites-0.8.3/synapse_super_invites/resource/info.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     3281 2024-05-28 17:18:15.000000 synapse_super_invites-0.8.3/synapse_super_invites/resource/redeem.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     4790 2024-05-11 20:20:17.000000 synapse_super_invites-0.8.3/synapse_super_invites/resource/tokens.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     2034 2024-05-11 20:20:17.000000 synapse_super_invites-0.8.3/synapse_super_invites/resource/web_access.py
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.319894 synapse_super_invites-0.8.3/synapse_super_invites/static/
+-rw-r--r--   0 ben       (1001) ben       (1001)      556 2023-11-15 23:09:11.000000 synapse_super_invites-0.8.3/synapse_super_invites/static/index.html
+-rw-r--r--   0 ben       (1001) ben       (1001)    15721 2023-11-15 22:50:38.000000 synapse_super_invites-0.8.3/synapse_super_invites/static/pure-min.css
+-rw-r--r--   0 ben       (1001) ben       (1001)       57 2023-11-15 23:06:08.000000 synapse_super_invites-0.8.3/synapse_super_invites/static/script.js
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.319894 synapse_super_invites-0.8.3/synapse_super_invites.egg-info/
+-rw-r--r--   0 ben       (1001) ben       (1001)     4517 2024-05-28 17:25:57.000000 synapse_super_invites-0.8.3/synapse_super_invites.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1001) ben       (1001)     1284 2024-05-28 17:25:57.000000 synapse_super_invites-0.8.3/synapse_super_invites.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1001) ben       (1001)        1 2024-05-28 17:25:57.000000 synapse_super_invites-0.8.3/synapse_super_invites.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1001) ben       (1001)      135 2024-05-28 17:25:57.000000 synapse_super_invites-0.8.3/synapse_super_invites.egg-info/requires.txt
+-rw-r--r--   0 ben       (1001) ben       (1001)       22 2024-05-28 17:25:57.000000 synapse_super_invites-0.8.3/synapse_super_invites.egg-info/top_level.txt
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.319894 synapse_super_invites-0.8.3/tests/
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-28 17:25:57.319894 synapse_super_invites-0.8.3/tests/.local/
+-rw-r--r--   0 ben       (1001) ben       (1001)        0 2024-05-28 17:19:58.000000 synapse_super_invites-0.8.3/tests/.local/.gitkeep
+-rw-r--r--   0 ben       (1001) ben       (1001)     1739 2024-05-28 17:14:42.000000 synapse_super_invites-0.8.3/tests/__init__.py
+-rw-r--r--   0 ben       (1001) ben       (1001)      844 2023-11-15 23:09:33.000000 synapse_super_invites-0.8.3/tests/example_cfg.yml
+-rw-r--r--   0 ben       (1001) ben       (1001)      865 2023-11-17 13:28:20.000000 synapse_super_invites-0.8.3/tests/test_config.py
+-rw-r--r--   0 ben       (1001) ben       (1001)    34034 2024-05-28 17:18:33.000000 synapse_super_invites-0.8.3/tests/test_integrations.py
+-rw-r--r--   0 ben       (1001) ben       (1001)      866 2024-05-28 17:11:31.000000 synapse_super_invites-0.8.3/tox.ini
```

### Comparing `synapse_super_invites-0.8.2/.github/workflows/ci.yml` & `synapse_super_invites-0.8.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/.github/workflows/release.yml` & `synapse_super_invites-0.8.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/.gitlab-ci.yml` & `synapse_super_invites-0.8.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/PKG-INFO` & `synapse_super_invites-0.8.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapse_super_invites
-Version: 0.8.2
+Version: 0.8.3
 Summary: Provides extended support for users to invite other users to rooms via an inventation token
 Project-URL: Homepage, https://www.acter.global/
 Project-URL: Repository, https://github.com/acterglobal/synapse-super-invites/
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matrix-synapse
@@ -19,14 +19,16 @@
 Requires-Dist: black==23.10.0; extra == "dev"
 Requires-Dist: ruff==0.1.1; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # Super Invitation flow for Synapse Matrix Homeserver
 
+![GitHub CI status main](https://img.shields.io/github/checks-status/acterglobal/synapse-super-invites/main) ![PyPI - Version](https://img.shields.io/pypi/v/synapse_super_invites)
+
 Provides extended support for users to invite other users to rooms via an invitation token
 
 ## Installation
 
 From the virtual environment that you use for Synapse, install this module with:
 
 ```shell
@@ -73,14 +75,18 @@
 
 You can confirm the installation went well by trying to access the path `/_synapse/client/super_invites/tokens` on your matrix server. If the module is available this will return with a `401` with `errCode: M_MISSING_TOKEN`. If it isn't available you will get a `404` with `"errcode: "M_UNRECOGNIZED"`.
 
 ## Usage
 
 ## Changelog
 
+**0.8.3** - 2024-05-28:
+
+- [Fix] Skip room if adding fails, but continue with adding to the others, track errors in db
+
 **0.8.2** - 2024-05-11:
 
 - Support for receiving info about a token without redeeming it, #2
 - Fix to mark DMs as direct (includes tests), #7
 - Fix for pyproject URLs, #1, thanks to @HarHarLinks
 - Allow API caller to not disable registration token creation
 - Clean up types
@@ -123,14 +129,16 @@
 
 To run the unit tests, you can either use:
 
 ```shell
 tox -e py
 ```
 
-or
+To run the linters and `mypy` type checker, use `./scripts-dev/lint.sh`.
 
-```shell
-trial tests
-```
+### Generating new db version
 
-To run the linters and `mypy` type checker, use `./scripts-dev/lint.sh`.
+Make your changes in `model/`, then run:
+
+```
+alembic revision --autogenerate -m "Description message"
+```
```

### Comparing `synapse_super_invites-0.8.2/README.md` & `synapse_super_invites-0.8.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Super Invitation flow for Synapse Matrix Homeserver
 
+![GitHub CI status main](https://img.shields.io/github/checks-status/acterglobal/synapse-super-invites/main) ![PyPI - Version](https://img.shields.io/pypi/v/synapse_super_invites)
+
 Provides extended support for users to invite other users to rooms via an invitation token
 
 ## Installation
 
 From the virtual environment that you use for Synapse, install this module with:
 
 ```shell
@@ -50,14 +52,18 @@
 
 You can confirm the installation went well by trying to access the path `/_synapse/client/super_invites/tokens` on your matrix server. If the module is available this will return with a `401` with `errCode: M_MISSING_TOKEN`. If it isn't available you will get a `404` with `"errcode: "M_UNRECOGNIZED"`.
 
 ## Usage
 
 ## Changelog
 
+**0.8.3** - 2024-05-28:
+
+- [Fix] Skip room if adding fails, but continue with adding to the others, track errors in db
+
 **0.8.2** - 2024-05-11:
 
 - Support for receiving info about a token without redeeming it, #2
 - Fix to mark DMs as direct (includes tests), #7
 - Fix for pyproject URLs, #1, thanks to @HarHarLinks
 - Allow API caller to not disable registration token creation
 - Clean up types
@@ -100,14 +106,16 @@
 
 To run the unit tests, you can either use:
 
 ```shell
 tox -e py
 ```
 
-or
+To run the linters and `mypy` type checker, use `./scripts-dev/lint.sh`.
 
-```shell
-trial tests
-```
+### Generating new db version
 
-To run the linters and `mypy` type checker, use `./scripts-dev/lint.sh`.
+Make your changes in `model/`, then run:
+
+```
+alembic revision --autogenerate -m "Description message"
+```
```

### Comparing `synapse_super_invites-0.8.2/alembic.ini` & `synapse_super_invites-0.8.3/alembic.ini`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 # new in Alembic version 1.10
 # recursive_version_locations = false
 
 # the output encoding used when revision files
 # are written from script.py.mako
 # output_encoding = utf-8
 
-sqlalchemy.url = sqlite:///
+sqlalchemy.url = sqlite:///build/local.db
 
 
 [post_write_hooks]
 # post_write_hooks defines scripts or Python functions that are run
 # on newly generated revision scripts.  See the documentation for further
 # detail and examples
```

### Comparing `synapse_super_invites-0.8.2/pyproject.toml` & `synapse_super_invites-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/__init__.py` & `synapse_super_invites-0.8.3/synapse_super_invites/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .resource import (
     RedeemResource,
     TokenInfoResource,
     TokensResource,
     WebAccessResource,
 )
 
-__version__ = "0.8.2"
+__version__ = "0.8.3"
 
 PKG_DIR = os.path.dirname(os.path.realpath(__file__))
 
 
 class SynapseSuperInvites:
     def __init__(self, config: SynapseSuperInvitesConfig, api: ModuleApi):
         # Keep a reference to the config and Module API
```

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/alembic.ini` & `synapse_super_invites-0.8.3/synapse_super_invites/alembic.ini`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/config.py` & `synapse_super_invites-0.8.3/synapse_super_invites/config.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/migration/env.py` & `synapse_super_invites-0.8.3/synapse_super_invites/migration/env.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/migration/script.py.mako` & `synapse_super_invites-0.8.3/synapse_super_invites/migration/script.py.mako`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/migration/versions/25e4ec3cea32_added_token_table.py` & `synapse_super_invites-0.8.3/synapse_super_invites/migration/versions/25e4ec3cea32_added_token_table.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/model/__init__.py` & `synapse_super_invites-0.8.3/synapse_super_invites/model/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     )
 
 
 class Accepted(Base):
     __tablename__ = "accepted"
     id: Mapped[int] = mapped_column(primary_key=True)
     user: Mapped[str] = mapped_column(String(255))
+    errors: Mapped[str] = mapped_column(String(1024), nullable=True)
 
     token_id = mapped_column(ForeignKey("tokens.token"))
     token = relationship("Token", back_populates="accepted")
 
     # meta
     created_at = mapped_column(DateTime(timezone=True), server_default=func.now())
     updated_at = mapped_column(
```

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/resource/base.py` & `synapse_super_invites-0.8.3/synapse_super_invites/resource/base.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/resource/info.py` & `synapse_super_invites-0.8.3/synapse_super_invites/resource/info.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/resource/redeem.py` & `synapse_super_invites-0.8.3/synapse_super_invites/resource/redeem.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+
+import logging
+
 from sqlalchemy import select
 from synapse.http.servlet import parse_string
 from synapse.http.site import SynapseRequest
 from synapse.types import JsonDict, Tuple  # type: ignore[attr-defined]
 
 from synapse_super_invites.model import Accepted
 
 from .base import SuperInviteResourceBase, token_query
 
+logger = logging.getLogger(__name__)
 
 class RedeemResource(SuperInviteResourceBase):
     async def _async_render_POST(self, request: SynapseRequest) -> Tuple[int, JsonDict]:
         requester = await self.api.get_user_by_req(request, allow_guest=False)
         my_id = str(requester.user)
         token_id = parse_string(request, "token", required=True)
         invited_rooms = []
+        errors = []
         with self.db.begin() as session:
             token = session.scalar(token_query(token_id))
             if not token:
                 return 404, {"error": "Token not found", "errcode": "NOT_FOUND"}
 
             if session.scalar(
                 select(Accepted).where(Accepted.user == my_id, Accepted.token == token)
@@ -31,38 +36,54 @@
                 return 400, {
                     "error": "Can't redeem your own token",
                     "errcode": "CANT_REDEEM",
                 }
 
             owner = token.owner
             for room in token.rooms:
-                await self.api.update_room_membership(
-                    sender=owner,
-                    target=my_id,
-                    room_id=room.nameOrAlias,
-                    new_membership="invite",
-                )
-
-                await self.api.update_room_membership(
-                    sender=my_id,
-                    target=my_id,
-                    room_id=room.nameOrAlias,
-                    new_membership="join",
-                )
-                invited_rooms.append(room.nameOrAlias)
+                try:
+                    await self.api.update_room_membership(
+                        sender=owner,
+                        target=my_id,
+                        room_id=room.nameOrAlias,
+                        new_membership="invite",
+                    )
+
+                    await self.api.update_room_membership(
+                        sender=my_id,
+                        target=my_id,
+                        room_id=room.nameOrAlias,
+                        new_membership="join",
+                    )
+                    invited_rooms.append(room.nameOrAlias)
+                except Exception as e:
+                    errors.append("{room_id} skipped: '{error}'".format(
+                        room_id=room.nameOrAlias,
+                        error=e))
+                    logger.warning(
+                        "Skipping super invite{token}: Failed to add {user_id} to {room_id}: {error}".format(
+                        token=token_id,
+                        user_id=my_id,
+                        room_id=room.nameOrAlias,
+                        error=e)
+                    )
 
             if token.create_dm:
                 dm_data = await self.api.create_room(
                     my_id,
                     config={
                         "preset": "trusted_private_chat",
                         "invite": [owner],
                         "is_direct": True,
                     },
                 )
                 invited_rooms.append(dm_data[0])
 
+            error_msg = None
+            if len(errors) > 0:
+                error_msg = '\n'.join(errors)[:1024]
+
             # keep the accepted record
-            session.add(Accepted(token=token, user=my_id))
+            session.add(Accepted(token=token, user=my_id, errors=error_msg))
             session.flush()
 
         return 200, {"rooms": invited_rooms}
```

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/resource/tokens.py` & `synapse_super_invites-0.8.3/synapse_super_invites/resource/tokens.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/resource/web_access.py` & `synapse_super_invites-0.8.3/synapse_super_invites/resource/web_access.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/static/index.html` & `synapse_super_invites-0.8.3/synapse_super_invites/static/index.html`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites/static/pure-min.css` & `synapse_super_invites-0.8.3/synapse_super_invites/static/pure-min.css`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites.egg-info/PKG-INFO` & `synapse_super_invites-0.8.3/synapse_super_invites.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapse_super_invites
-Version: 0.8.2
+Version: 0.8.3
 Summary: Provides extended support for users to invite other users to rooms via an inventation token
 Project-URL: Homepage, https://www.acter.global/
 Project-URL: Repository, https://github.com/acterglobal/synapse-super-invites/
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matrix-synapse
@@ -19,14 +19,16 @@
 Requires-Dist: black==23.10.0; extra == "dev"
 Requires-Dist: ruff==0.1.1; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # Super Invitation flow for Synapse Matrix Homeserver
 
+![GitHub CI status main](https://img.shields.io/github/checks-status/acterglobal/synapse-super-invites/main) ![PyPI - Version](https://img.shields.io/pypi/v/synapse_super_invites)
+
 Provides extended support for users to invite other users to rooms via an invitation token
 
 ## Installation
 
 From the virtual environment that you use for Synapse, install this module with:
 
 ```shell
@@ -73,14 +75,18 @@
 
 You can confirm the installation went well by trying to access the path `/_synapse/client/super_invites/tokens` on your matrix server. If the module is available this will return with a `401` with `errCode: M_MISSING_TOKEN`. If it isn't available you will get a `404` with `"errcode: "M_UNRECOGNIZED"`.
 
 ## Usage
 
 ## Changelog
 
+**0.8.3** - 2024-05-28:
+
+- [Fix] Skip room if adding fails, but continue with adding to the others, track errors in db
+
 **0.8.2** - 2024-05-11:
 
 - Support for receiving info about a token without redeeming it, #2
 - Fix to mark DMs as direct (includes tests), #7
 - Fix for pyproject URLs, #1, thanks to @HarHarLinks
 - Allow API caller to not disable registration token creation
 - Clean up types
@@ -123,14 +129,16 @@
 
 To run the unit tests, you can either use:
 
 ```shell
 tox -e py
 ```
 
-or
+To run the linters and `mypy` type checker, use `./scripts-dev/lint.sh`.
 
-```shell
-trial tests
-```
+### Generating new db version
 
-To run the linters and `mypy` type checker, use `./scripts-dev/lint.sh`.
+Make your changes in `model/`, then run:
+
+```
+alembic revision --autogenerate -m "Description message"
+```
```

### Comparing `synapse_super_invites-0.8.2/synapse_super_invites.egg-info/SOURCES.txt` & `synapse_super_invites-0.8.3/synapse_super_invites.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 synapse_super_invites.egg-info/SOURCES.txt
 synapse_super_invites.egg-info/dependency_links.txt
 synapse_super_invites.egg-info/requires.txt
 synapse_super_invites.egg-info/top_level.txt
 synapse_super_invites/migration/env.py
 synapse_super_invites/migration/script.py.mako
 synapse_super_invites/migration/versions/25e4ec3cea32_added_token_table.py
+synapse_super_invites/migration/versions/8c8c90d89eac_add_error_logs_to_acceptance.py
 synapse_super_invites/model/__init__.py
 synapse_super_invites/resource/__init__.py
 synapse_super_invites/resource/base.py
 synapse_super_invites/resource/info.py
 synapse_super_invites/resource/redeem.py
 synapse_super_invites/resource/tokens.py
 synapse_super_invites/resource/web_access.py
```

### Comparing `synapse_super_invites-0.8.2/tests/__init__.py` & `synapse_super_invites-0.8.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/tests/example_cfg.yml` & `synapse_super_invites-0.8.3/tests/example_cfg.yml`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/tests/test_config.py` & `synapse_super_invites-0.8.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.2/tests/test_integrations.py` & `synapse_super_invites-0.8.3/tests/test_integrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,21 @@
     # create a room with the given access_token, return the roomId
     def create_room(self, user_id: str) -> str:
         room_id: str = self.get_success(
             self.module_api.create_room(user_id=user_id, config={}, ratelimit=False)
         )[0]
         return room_id
 
+
+    # leave a room with the given access_token
+    def leave_room(self, user_id: str, room_id: str):
+        self.get_success(
+            self.module_api.update_room_membership(sender=user_id, target=user_id, room_id=room_id, new_membership='leave')
+        )
+
     # create a room with the given access_token, return the roomId
     def create_public_room(self, user_id: str) -> str:
         room_id: str = self.get_success(
             self.module_api.create_room(
                 user_id=user_id,
                 config={"preset": "public_chat", "visibility": "public"},
                 ratelimit=False,
@@ -227,14 +234,111 @@
         )
         self.assertEqual(channel.code, 200, msg=channel.result)
         self.assertEqual(channel.json_body["rooms"].get("invite"), None)
         self.assertCountEqual(
             channel.json_body["rooms"]["join"].keys(), rooms_to_invite
         )
 
+
+    @override_config(DEFAULT_CONFIG)  # type: ignore[misc]
+    def test_skip_if_broken_now(self) -> None:
+        m_id = self.register_user("meeko", "password")
+        m_access_token = self.login("meeko", "password")
+
+        # this is our new backend.
+        channel = self.make_request(
+            "GET", "/_synapse/client/super_invites/tokens", access_token=m_access_token
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        self.assertEqual(channel.json_body["tokens"], [])
+
+        # creating five channel
+        roomB = self.create_room(m_id)
+        roomC = self.create_room(m_id)
+        roomD = self.create_room(m_id)
+
+        rooms_to_invite = [
+            roomB,
+            roomC,
+            roomD,
+        ]
+        # create a new one for testing.
+        channel = self.make_request(
+            "POST",
+            "/_synapse/client/super_invites/tokens",
+            access_token=m_access_token,
+            content={"rooms": rooms_to_invite},
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        token_data = channel.json_body["token"]
+        self.assertCountEqual(token_data["rooms"], rooms_to_invite)
+        self.assertEquals(token_data["accepted_count"], 0)
+        self.assertFalse(token_data["create_dm"])
+        token = token_data["token"]
+
+        room_left_after = rooms_to_invite.pop(0)
+        self.leave_room(m_id, room_left_after)
+
+        # redeem the new token
+
+        _f_id = self.register_user("flit", "flit")
+        f_access_token = self.login("flit", "flit")
+
+        channel = self.make_request(
+            "GET",
+            "/_synapse/client/super_invites/info?token={token}".format(token=token),
+            access_token=f_access_token,
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        # list the rooms we were invited to
+
+        self.assertEqual(channel.json_body["rooms_count"], 3) # info shows 3
+        self.assertEqual(channel.json_body["create_dm"], False)
+        self.assertEqual(channel.json_body["has_redeemed"], False)
+        self.assertEqual(channel.json_body["inviter"]["user_id"], "@meeko:test")
+        self.assertEqual(channel.json_body["inviter"]["display_name"], "meeko")
+
+        channel = self.make_request(
+            "POST",
+            "/_synapse/client/super_invites/redeem?token={token}".format(token=token),
+            access_token=f_access_token,
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        # list the rooms we were invited to
+        self.assertCountEqual(channel.json_body["rooms"], rooms_to_invite) # but working are only two
+
+        # we see it has been redeemed
+        channel = self.make_request(
+            "GET",
+            "/_synapse/client/super_invites/tokens?token={token}".format(token=token),
+            access_token=m_access_token,
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        token_data = channel.json_body["token"]
+        self.assertEquals(token_data["accepted_count"], 1)
+
+        channel = self.make_request(
+            "GET",
+            "/_synapse/client/super_invites/info?token={token}".format(token=token),
+            access_token=f_access_token,
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        self.assertEqual(channel.json_body["has_redeemed"], True)
+
+        # and flit was invited to these, too:
+        channel = self.make_request(
+            "GET", "/_matrix/client/v3/sync", access_token=f_access_token
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        self.assertEqual(channel.json_body["rooms"].get("invite"), None)
+        self.assertCountEqual(
+            channel.json_body["rooms"]["join"].keys(), rooms_to_invite
+        )
+
+
     @override_config(DEFAULT_CONFIG)  # type: ignore[misc]
     def test_simple_can_join_public_room_test(self) -> None:
         m_id = self.register_user("meeko", "password")
         m_access_token = self.login("meeko", "password")
 
         # this is our new backend.
         channel = self.make_request(
```

### Comparing `synapse_super_invites-0.8.2/tox.ini` & `synapse_super_invites-0.8.3/tox.ini`

 * *Files identical despite different names*

