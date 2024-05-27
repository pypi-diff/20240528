# Comparing `tmp/gypsum_client-0.1.2.tar.gz` & `tmp/gypsum_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gypsum_client-0.1.2.tar", last modified: Sun May 26 01:12:41 2024, max compression
+gzip compressed data, was "gypsum_client-0.1.3.tar", last modified: Mon May 27 23:52:21 2024, max compression
```

## Comparing `gypsum_client-0.1.2.tar` & `gypsum_client-0.1.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.464810 gypsum_client-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.448810 gypsum_client-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.452810 gypsum_client-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-26 01:12:41.464810 gypsum_client-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.456810 gypsum_client-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.456810 gypsum_client-0.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-26 01:12:41.468810 gypsum_client-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.452810 gypsum_client-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.460810 gypsum_client-0.1.2/src/gypsum_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/cache_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/clone_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/create_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/fetch_metadata_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/fetch_metadata_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/fetch_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/list_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/prepare_directory_for_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/probation_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/refresh_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/remove_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/resolve_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/rest_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/s3_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/save_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/search_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/set_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/upload_api_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/upload_file_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/validate_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.464810 gypsum_client-0.1.2/src/gypsum_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-26 01:12:41.000000 gypsum_client-0.1.2/src/gypsum_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-26 01:12:41.000000 gypsum_client-0.1.2/src/gypsum_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:12:41.000000 gypsum_client-0.1.2/src/gypsum_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:12:41.000000 gypsum_client-0.1.2/src/gypsum_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-26 01:12:41.000000 gypsum_client-0.1.2/src/gypsum_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 01:12:41.000000 gypsum_client-0.1.2/src/gypsum_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.464810 gypsum_client-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_fetch_metadata_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_fetch_metadata_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_latest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_prepare_dir_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_probation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_quota.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:52:21.382556 gypsum_client-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:52:21.366556 gypsum_client-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:52:21.370555 gypsum_client-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-27 23:52:21.382556 gypsum_client-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:52:21.374556 gypsum_client-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:52:21.374556 gypsum_client-0.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-27 23:52:21.382556 gypsum_client-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:52:21.366556 gypsum_client-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:52:21.378556 gypsum_client-0.1.3/src/gypsum_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/cache_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/clone_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/create_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/fetch_metadata_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/fetch_metadata_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/fetch_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/list_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/prepare_directory_for_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/probation_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/refresh_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/remove_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/resolve_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/rest_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/s3_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/save_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/search_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/set_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/upload_api_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/upload_file_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/src/gypsum_client/validate_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:52:21.382556 gypsum_client-0.1.3/src/gypsum_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-27 23:52:21.000000 gypsum_client-0.1.3/src/gypsum_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-27 23:52:21.000000 gypsum_client-0.1.3/src/gypsum_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 23:52:21.000000 gypsum_client-0.1.3/src/gypsum_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 23:52:21.000000 gypsum_client-0.1.3/src/gypsum_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-27 23:52:21.000000 gypsum_client-0.1.3/src/gypsum_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 23:52:21.000000 gypsum_client-0.1.3/src/gypsum_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:52:21.382556 gypsum_client-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_fetch_metadata_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_fetch_metadata_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_latest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_prepare_dir_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_probation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-27 23:50:55.000000 gypsum_client-0.1.3/tox.ini
```

### Comparing `gypsum_client-0.1.2/.coveragerc` & `gypsum_client-0.1.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/.github/workflows/pypi-publish.yml` & `gypsum_client-0.1.3/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/.github/workflows/pypi-test.yml` & `gypsum_client-0.1.3/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/.gitignore` & `gypsum_client-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/.pre-commit-config.yaml` & `gypsum_client-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/.readthedocs.yml` & `gypsum_client-0.1.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/CONTRIBUTING.md` & `gypsum_client-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/LICENSE.txt` & `gypsum_client-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/PKG-INFO` & `gypsum_client-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gypsum-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client to gypsum REST API
 Home-page: https://github.com/ArtifactDB/gypsum-py
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/gypsum-py
 Platform: any
```

### Comparing `gypsum_client-0.1.2/README.md` & `gypsum_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/docs/Makefile` & `gypsum_client-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/docs/conf.py` & `gypsum_client-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/docs/index.md` & `gypsum_client-0.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/docs/tutorial.md` & `gypsum_client-0.1.3/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/setup.cfg` & `gypsum_client-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/setup.py` & `gypsum_client-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/__init__.py` & `gypsum_client-0.1.3/src/gypsum_client/__init__.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/_github.py` & `gypsum_client-0.1.3/src/gypsum_client/_github.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/_utils.py` & `gypsum_client-0.1.3/src/gypsum_client/_utils.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/auth.py` & `gypsum_client-0.1.3/src/gypsum_client/auth.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/cache_directory.py` & `gypsum_client-0.1.3/src/gypsum_client/cache_directory.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/clone_operations.py` & `gypsum_client-0.1.3/src/gypsum_client/clone_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/create_operations.py` & `gypsum_client-0.1.3/src/gypsum_client/create_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/fetch_metadata_database.py` & `gypsum_client-0.1.3/src/gypsum_client/fetch_metadata_database.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/fetch_metadata_schema.py` & `gypsum_client-0.1.3/src/gypsum_client/fetch_metadata_schema.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/fetch_operations.py` & `gypsum_client-0.1.3/src/gypsum_client/fetch_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/list_operations.py` & `gypsum_client-0.1.3/src/gypsum_client/list_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/prepare_directory_for_upload.py` & `gypsum_client-0.1.3/src/gypsum_client/prepare_directory_for_upload.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/probation_operations.py` & `gypsum_client-0.1.3/src/gypsum_client/probation_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/refresh_operations.py` & `gypsum_client-0.1.3/src/gypsum_client/refresh_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/remove_operations.py` & `gypsum_client-0.1.3/src/gypsum_client/remove_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/resolve_links.py` & `gypsum_client-0.1.3/src/gypsum_client/resolve_links.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/rest_url.py` & `gypsum_client-0.1.3/src/gypsum_client/rest_url.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/s3_config.py` & `gypsum_client-0.1.3/src/gypsum_client/s3_config.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/save_operations.py` & `gypsum_client-0.1.3/src/gypsum_client/save_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/search_metadata.py` & `gypsum_client-0.1.3/src/gypsum_client/search_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     def __invert__(self):
         return GypsumSearchClause(type="not", child=self)
 
 
 def search_metadata_text(
     path: str,
-    query: Union[str, GypsumSearchClause],
+    query: Union[str, List[str], GypsumSearchClause],
     latest: bool = True,
     include_metadata: bool = True,
 ) -> List[Dict]:
     """Text search on the metadata database.
 
     Perform a text search on a SQLite database containing
     metadata from the gypsum backend. This is based on a precomputed
@@ -165,16 +165,18 @@
         stmt += " FROM paths LEFT JOIN versions ON paths.vid = versions.vid"
 
         if latest:
             cond.append("versions.latest = 1")
 
         if cond:
             stmt += " WHERE " + " AND ".join(cond)
+            cursor = conn.execute(stmt, params)
+        else:
+            cursor = conn.execute(stmt)
 
-        cursor = conn.execute(stmt, params)
         results = [dict(row) for row in cursor.fetchall()]
         if include_metadata:
             for result in results:
                 result["metadata"] = json.loads(result["metadata"])
 
         return results
     finally:
@@ -203,39 +205,42 @@
     Returns:
         `GypsumSearchClause` defining the search.
     """
     return GypsumSearchClause(type="text", text=text, field=field, partial=partial)
 
 
 def search_metadata_text_filter(
-    query: Union[str, GypsumSearchClause], pid_name: str = "paths.pid"
+    query: Union[str, List[str], GypsumSearchClause], pid_name: str = "paths.pid"
 ) -> Dict[str, Union[str, List]]:
     query = sanitize_query(query)
 
     if query is None:
         return {"where": [], "parameters": {}}
 
     env = {"parameters": {}}
     cond = build_query(query, pid_name, env)
     return {"where": cond, "parameters": env["parameters"]}
 
 
 def sanitize_query(
-    query: Union[str, GypsumSearchClause],
+    query: Union[str, List[str], GypsumSearchClause],
 ) -> Optional[GypsumSearchClause]:
     if isinstance(query, list):
         if len(query) > 1:
             query = GypsumSearchClause(
                 type="and", children=[define_text_query(q) for q in query]
             )
         elif len(query) == 1:
             query = define_text_query(query[0])
         else:
             raise ValueError("'query' must have atleast 1 element.")
 
+    if isinstance(query, str):
+        query = define_text_query(query)
+
     if query.type == "not":
         query.child = sanitize_query(query.child)
         if query.child is None:
             return None
         return query
 
     if query.type != "text":
```

### Comparing `gypsum_client-0.1.2/src/gypsum_client/set_operations.py` & `gypsum_client-0.1.3/src/gypsum_client/set_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/upload_api_operations.py` & `gypsum_client-0.1.3/src/gypsum_client/upload_api_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/upload_file_actions.py` & `gypsum_client-0.1.3/src/gypsum_client/upload_file_actions.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client/validate_metadata.py` & `gypsum_client-0.1.3/src/gypsum_client/validate_metadata.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/src/gypsum_client.egg-info/PKG-INFO` & `gypsum_client-0.1.3/src/gypsum_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gypsum-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client to gypsum REST API
 Home-page: https://github.com/ArtifactDB/gypsum-py
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/gypsum-py
 Platform: any
```

### Comparing `gypsum_client-0.1.2/src/gypsum_client.egg-info/SOURCES.txt` & `gypsum_client-0.1.3/src/gypsum_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_auth.py` & `gypsum_client-0.1.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_clone.py` & `gypsum_client-0.1.3/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_fetch.py` & `gypsum_client-0.1.3/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_fetch_metadata_database.py` & `gypsum_client-0.1.3/tests/test_fetch_metadata_database.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_fetch_metadata_schema.py` & `gypsum_client-0.1.3/tests/test_fetch_metadata_schema.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_latest.py` & `gypsum_client-0.1.3/tests/test_latest.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_list.py` & `gypsum_client-0.1.3/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_permissions.py` & `gypsum_client-0.1.3/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_prepare_dir_upload.py` & `gypsum_client-0.1.3/tests/test_prepare_dir_upload.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_probation.py` & `gypsum_client-0.1.3/tests/test_probation.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_quota.py` & `gypsum_client-0.1.3/tests/test_quota.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_remove.py` & `gypsum_client-0.1.3/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_save.py` & `gypsum_client-0.1.3/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tests/test_search.py` & `gypsum_client-0.1.3/tests/test_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,20 @@
     result = search_metadata_text(
         sqlite_path, ["mikoto"], include_metadata=False, latest=False
     )
 
     assert len(result) == 1
     assert result[0]["path"] == "mikoto.txt"
 
+    result1 = search_metadata_text(
+        sqlite_path, "mikoto", include_metadata=False, latest=False
+    )
+    assert len(result1) == 1
+    assert result1[0]["path"] == "mikoto.txt"
+
     result = search_metadata_text(
         sqlite_path, ["kuroko"], include_metadata=False, latest=False
     )
     assert len(result) == 1
     assert result[0]["path"] == "kuroko.txt"
 
     result = search_metadata_text(
```

### Comparing `gypsum_client-0.1.2/tests/test_upload.py` & `gypsum_client-0.1.3/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.2/tox.ini` & `gypsum_client-0.1.3/tox.ini`

 * *Files identical despite different names*

