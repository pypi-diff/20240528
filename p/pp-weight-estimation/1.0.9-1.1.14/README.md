# Comparing `tmp/pp_weight_estimation-1.0.9.tar.gz` & `tmp/pp_weight_estimation-1.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pp_weight_estimation-1.0.9.tar", last modified: Wed May 22 13:34:55 2024, max compression
+gzip compressed data, was "pp_weight_estimation-1.1.14.tar", last modified: Tue May 28 14:06:03 2024, max compression
```

## Comparing `pp_weight_estimation-1.0.9.tar` & `pp_weight_estimation-1.1.14.tar`

### file list

```diff
@@ -1,17 +1,29 @@
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-22 13:34:55.690183 pp_weight_estimation-1.0.9/
--rw-r--r--   0 malav     (1000) malav     (1000)      245 2024-05-22 13:34:55.690183 pp_weight_estimation-1.0.9/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-17 03:44:16.000000 pp_weight_estimation-1.0.9/README.md
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-22 13:34:55.686183 pp_weight_estimation-1.0.9/pp_weight_estimation/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.0.9/pp_weight_estimation/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      206 2024-05-22 13:34:45.000000 pp_weight_estimation-1.0.9/pp_weight_estimation/version.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-22 13:34:55.686183 pp_weight_estimation-1.0.9/pp_weight_estimation.egg-info/
--rw-r--r--   0 malav     (1000) malav     (1000)      245 2024-05-22 13:34:55.000000 pp_weight_estimation-1.0.9/pp_weight_estimation.egg-info/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)      342 2024-05-22 13:34:55.000000 pp_weight_estimation-1.0.9/pp_weight_estimation.egg-info/SOURCES.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-22 13:34:55.000000 pp_weight_estimation-1.0.9/pp_weight_estimation.egg-info/dependency_links.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-22 13:34:55.000000 pp_weight_estimation-1.0.9/pp_weight_estimation.egg-info/requires.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-05-22 13:34:55.000000 pp_weight_estimation-1.0.9/pp_weight_estimation.egg-info/top_level.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.0.9/pyproject.toml
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-22 13:34:55.686183 pp_weight_estimation-1.0.9/scripts/
--rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-22 13:34:30.000000 pp_weight_estimation-1.0.9/scripts/weight_pred.py
--rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-22 13:34:55.690183 pp_weight_estimation-1.0.9/setup.cfg
--rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-17 03:44:16.000000 pp_weight_estimation-1.0.9/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.14/README.md
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/pp_weight_estimation/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/pp_weight_estimation/core/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/core/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     7871 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/core/function_test.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     6680 2024-05-26 03:01:35.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/core/get_weight.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/core/gpt_support.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1643 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/core/s3_io.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/pp_weight_estimation/utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/utils/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1000 2024-05-23 00:53:12.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/utils/slack_connect.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/utils/visulizer.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-28 14:05:49.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/version.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-28 14:06:03.000000 pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-05-28 14:06:03.000000 pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/SOURCES.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-28 14:06:03.000000 pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/dependency_links.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-28 14:06:03.000000 pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/requires.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-05-28 14:06:03.000000 pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/top_level.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.14/pyproject.toml
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.094194 pp_weight_estimation-1.1.14/scripts/
+-rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.14/scripts/weight_pred.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/setup.cfg
+-rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.14/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/tests/
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.14/tests/test_function_test.py
```

### Comparing `pp_weight_estimation-1.0.9/setup.py` & `pp_weight_estimation-1.1.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup,find_packages
 import os
 
 VERSION_FILE = os.path.join(os.path.dirname(__file__), "VERSION.txt")
 print(VERSION_FILE)
+
 setup(
     name="pp_weight_estimation",
     description="Production planning weight estimation functions",
     author=["Malav Bateriwala"],
     packages=find_packages(),
     #packages=find_packages(),
     scripts=['./scripts/weight_pred.py'],
@@ -17,14 +18,14 @@
         "mb_base",
         "mb_utils",
         "mb_pandas",],
     setup_requires=["setuptools-git-versioning<2"],
     python_requires='>=3.8',
     setuptools_git_versioning={
         "enabled": True,
-        "version_file": VERSION_FILE,
+       "version_file": VERSION_FILE,
         "count_commits_from_version_file": True,
         "template": "{tag}",
         "dev_template": "{tag}.dev{ccount}+{branch}",
         "dirty_template": "{tag}.post{ccount}",
     },
 )
```

