# Comparing `tmp/anemoi_utils-0.1.9.tar.gz` & `tmp/anemoi_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemoi_utils-0.1.9.tar", last modified: Fri May 17 13:44:30 2024, max compression
+gzip compressed data, was "anemoi_utils-0.2.0.tar", last modified: Tue May 28 09:25:30 2024, max compression
```

## Comparing `anemoi_utils-0.1.9.tar` & `anemoi_utils-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.853158 anemoi_utils-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.841158 anemoi_utils-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.845158 anemoi_utils-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-05-17 13:44:30.853158 anemoi_utils-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.845158 anemoi_utils-0.1.9/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.845158 anemoi_utils-0.1.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.845158 anemoi_utils-0.1.9/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/installing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.845158 anemoi_utils-0.1.9/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/checkpoints.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/dates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/grib.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/humanize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/provenance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/modules/text.rst
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 13:44:30.853158 anemoi_utils-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.845158 anemoi_utils-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.841158 anemoi_utils-0.1.9/src/anemoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.849158 anemoi_utils-0.1.9/src/anemoi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 13:44:30.000000 anemoi_utils-0.1.9/src/anemoi/utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/grib.py
--rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/humanize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.849158 anemoi_utils-0.1.9/src/anemoi/utils/mars/
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/mars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/mars/mars.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/src/anemoi/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.849158 anemoi_utils-0.1.9/src/anemoi_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-05-17 13:44:30.000000 anemoi_utils-0.1.9/src/anemoi_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-17 13:44:30.000000 anemoi_utils-0.1.9/src/anemoi_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:44:30.000000 anemoi_utils-0.1.9/src/anemoi_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 13:44:30.000000 anemoi_utils-0.1.9/src/anemoi_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 13:44:30.000000 anemoi_utils-0.1.9/src/anemoi_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:44:30.849158 anemoi_utils-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/tests/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-17 13:44:21.000000 anemoi_utils-0.1.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.625761 anemoi_utils-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.613761 anemoi_utils-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.617761 anemoi_utils-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-05-28 09:25:30.625761 anemoi_utils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.617761 anemoi_utils-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.617761 anemoi_utils-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.617761 anemoi_utils-0.2.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/installing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.621761 anemoi_utils-0.2.0/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/modules/checkpoints.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/modules/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/modules/dates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/modules/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/modules/humanize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/modules/provenance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/modules/text.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:25:30.625761 anemoi_utils-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.617761 anemoi_utils-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.613761 anemoi_utils-0.2.0/src/anemoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.621761 anemoi_utils-0.2.0/src/anemoi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 09:25:30.000000 anemoi_utils-0.2.0/src/anemoi/utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/checkpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.621761 anemoi_utils-0.2.0/src/anemoi/utils/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/commands/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/humanize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.621761 anemoi_utils-0.2.0/src/anemoi/utils/mars/
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/mars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/mars/mars.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/src/anemoi/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.625761 anemoi_utils-0.2.0/src/anemoi_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-05-28 09:25:30.000000 anemoi_utils-0.2.0/src/anemoi_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-28 09:25:30.000000 anemoi_utils-0.2.0/src/anemoi_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:25:30.000000 anemoi_utils-0.2.0/src/anemoi_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 09:25:30.000000 anemoi_utils-0.2.0/src/anemoi_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 09:25:30.000000 anemoi_utils-0.2.0/src/anemoi_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 09:25:30.000000 anemoi_utils-0.2.0/src/anemoi_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:25:30.625761 anemoi_utils-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/tests/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-28 09:25:19.000000 anemoi_utils-0.2.0/tests/test_utils.py
```

### Comparing `anemoi_utils-0.1.9/.github/workflows/python-publish.yml` & `anemoi_utils-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/.gitignore` & `anemoi_utils-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/.pre-commit-config.yaml` & `anemoi_utils-0.2.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -57,13 +57,14 @@
     - id: sphinx-lint
 
 # For now, we use it. But it does not support a lot of sphinx features
 - repo: https://github.com/dzhu/rstfmt
   rev: v0.0.14
   hooks:
     - id: rstfmt
+      exclude: 'cli/.*' # Because we use argparse
 
 - repo: https://github.com/b8raoult/pre-commit-docconvert
   rev: "0.1.4"
   hooks:
   - id: docconvert
     args: ["numpy"]
```

### Comparing `anemoi_utils-0.1.9/LICENSE` & `anemoi_utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/PKG-INFO` & `anemoi_utils-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-utils
-Version: 0.1.9
+Version: 0.2.0
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -220,34 +220,36 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: tomli
 Requires-Dist: pyyaml
+Requires-Dist: tqdm
 Provides-Extra: provenance
 Requires-Dist: GitPython; extra == "provenance"
 Requires-Dist: nvsmi; extra == "provenance"
 Provides-Extra: text
 Requires-Dist: termcolor; extra == "text"
 Provides-Extra: grib
 Requires-Dist: requests; extra == "grib"
 Provides-Extra: docs
 Requires-Dist: tomli; extra == "docs"
 Requires-Dist: termcolor; extra == "docs"
 Requires-Dist: requests; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: pandoc; extra == "docs"
+Requires-Dist: sphinx_argparse; extra == "docs"
 Provides-Extra: all
 Requires-Dist: tomli; extra == "all"
 Requires-Dist: GitPython; extra == "all"
 Requires-Dist: nvsmi; extra == "all"
 Requires-Dist: termcolor; extra == "all"
 Requires-Dist: requests; extra == "all"
 Provides-Extra: dev
 Requires-Dist: tomli; extra == "dev"
 Requires-Dist: GitPython; extra == "dev"
 Requires-Dist: nvsmi; extra == "dev"
 Requires-Dist: termcolor; extra == "dev"
 Requires-Dist: requests; extra == "dev"
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: sphinx_rtd_theme; extra == "dev"
-Requires-Dist: nbsphinx; extra == "dev"
-Requires-Dist: pandoc; extra == "dev"
```

### Comparing `anemoi_utils-0.1.9/README.md` & `anemoi_utils-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/docs/Makefile` & `anemoi_utils-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/docs/_static/logo.png` & `anemoi_utils-0.2.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/docs/_static/style.css` & `anemoi_utils-0.2.0/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/docs/conf.py` & `anemoi_utils-0.2.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,48 +10,43 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import datetime
 import os
 import sys
 
-sys.path.insert(0, os.path.join(os.path.abspath(".."), "src"))
-
-
 read_the_docs_build = os.environ.get("READTHEDOCS", None) == "True"
 
-# top = os.path.realpath(os.path.dirname(os.path.dirname(__file__)))
-# sys.path.insert(0, top)
-
+sys.path.insert(0, os.path.join(os.path.abspath(".."), "src"))
 
 source_suffix = ".rst"
 master_doc = "index"
 pygments_style = "sphinx"
 html_theme_options = {"logo_only": True}
 html_logo = "_static/logo.png"
 
 
 # -- Project information -----------------------------------------------------
 
-project = "Anemoi"
+project = "Anemoi Utils"
 
 author = "ECMWF"
 
 year = datetime.datetime.now().year
 if year == 2024:
     years = "2024"
 else:
     years = "2024-%s" % (year,)
 
 copyright = "%s, ECMWF" % (years,)
 
 try:
-    import anemoi.utils
+    from anemoi.utils._version import __version__
 
-    release = anemoi.utils.__version__
+    release = __version__
 except ImportError:
     release = "0.0.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
@@ -61,14 +56,15 @@
     "sphinx.ext.todo",
     "sphinx_rtd_theme",
     "nbsphinx",
     "sphinx.ext.graphviz",
     "sphinx.ext.intersphinx",
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
+    "sphinxarg.ext",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
```

### Comparing `anemoi_utils-0.1.9/docs/index.rst` & `anemoi_utils-0.2.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. _anemoi-utils:
 
 .. _index-page:
 
-####################################
- Welcome to Anemoi's documentation!
-####################################
+##########################################
+ Welcome to `anemoi-utils` documentation!
+##########################################
 
 .. warning::
 
    This documentation is work in progress.
 
 *Anemoi* is a framework for developing machine learning weather
 forecasting models. It comprises of components or packages for preparing
```

### Comparing `anemoi_utils-0.1.9/docs/installing.rst` & `anemoi_utils-0.2.0/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/pyproject.toml` & `anemoi_utils-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -36,31 +36,37 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "tomli", # Only needed before 3.11
+    "tomli",  # Only needed before 3.11
     "pyyaml",
+    "tqdm",
 ]
 
 [project.optional-dependencies]
 provenance = ["GitPython", "nvsmi"]
 
 text = ["termcolor"]
 
 grib = ["requests"]
 
 # Loaded by read-the-docs
 # `pip install .[docs]`
 docs = [
-    "tomli",     # Only needed before 3.11
+    "tomli",            # Only needed before 3.11
     "termcolor",
     "requests",
+    "sphinx",
+    "sphinx_rtd_theme",
+    "nbsphinx",
+    "pandoc",
+    "sphinx_argparse",
 ]
 
 all = [
     "tomli",     # Only needed before 3.11
     "GitPython",
     "nvsmi",
     "termcolor",
@@ -69,26 +75,24 @@
 
 dev = [
     "tomli",     # Only needed before 3.11
     "GitPython",
     "nvsmi",
     "termcolor",
     "requests",
-    "sphinx",
-    "sphinx_rtd_theme",
-    "nbsphinx",
-    "pandoc",
 ]
 
 [project.urls]
 Homepage = "https://github.com/ecmwf/anemoi-utils/"
 Documentation = "https://anemoi-utils.readthedocs.io/"
 Repository = "https://github.com/ecmwf/anemoi-utils/"
 Issues = "https://github.com/ecmwf/anemoi-utils/issues"
 # Changelog = "https://github.com/ecmwf/anemoi-utils/CHANGELOG.md"
 
+[project.scripts]
+anemoi-utils = "anemoi.utils.__main__:main"
 
 [tool.setuptools_scm]
 version_file = "src/anemoi/utils/_version.py"
 
 [tool.setuptools.package-data]
 "anemoi.utils.mars" = ["*.yaml"]
```

### Comparing `anemoi_utils-0.1.9/src/anemoi/utils/caching.py` & `anemoi_utils-0.2.0/src/anemoi/utils/caching.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/src/anemoi/utils/config.py` & `anemoi_utils-0.2.0/src/anemoi/utils/config.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/src/anemoi/utils/dates.py` & `anemoi_utils-0.2.0/src/anemoi/utils/dates.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/src/anemoi/utils/grib.py` & `anemoi_utils-0.2.0/src/anemoi/utils/grib.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/src/anemoi/utils/humanize.py` & `anemoi_utils-0.2.0/src/anemoi/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/src/anemoi/utils/mars/__init__.py` & `anemoi_utils-0.2.0/src/anemoi/utils/mars/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/src/anemoi/utils/provenance.py` & `anemoi_utils-0.2.0/src/anemoi/utils/provenance.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/src/anemoi/utils/text.py` & `anemoi_utils-0.2.0/src/anemoi/utils/text.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/src/anemoi_utils.egg-info/PKG-INFO` & `anemoi_utils-0.2.0/src/anemoi_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-utils
-Version: 0.1.9
+Version: 0.2.0
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -220,34 +220,36 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: tomli
 Requires-Dist: pyyaml
+Requires-Dist: tqdm
 Provides-Extra: provenance
 Requires-Dist: GitPython; extra == "provenance"
 Requires-Dist: nvsmi; extra == "provenance"
 Provides-Extra: text
 Requires-Dist: termcolor; extra == "text"
 Provides-Extra: grib
 Requires-Dist: requests; extra == "grib"
 Provides-Extra: docs
 Requires-Dist: tomli; extra == "docs"
 Requires-Dist: termcolor; extra == "docs"
 Requires-Dist: requests; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: pandoc; extra == "docs"
+Requires-Dist: sphinx_argparse; extra == "docs"
 Provides-Extra: all
 Requires-Dist: tomli; extra == "all"
 Requires-Dist: GitPython; extra == "all"
 Requires-Dist: nvsmi; extra == "all"
 Requires-Dist: termcolor; extra == "all"
 Requires-Dist: requests; extra == "all"
 Provides-Extra: dev
 Requires-Dist: tomli; extra == "dev"
 Requires-Dist: GitPython; extra == "dev"
 Requires-Dist: nvsmi; extra == "dev"
 Requires-Dist: termcolor; extra == "dev"
 Requires-Dist: requests; extra == "dev"
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: sphinx_rtd_theme; extra == "dev"
-Requires-Dist: nbsphinx; extra == "dev"
-Requires-Dist: pandoc; extra == "dev"
```

### Comparing `anemoi_utils-0.1.9/tests/test_dates.py` & `anemoi_utils-0.2.0/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.9/tests/test_utils.py` & `anemoi_utils-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

