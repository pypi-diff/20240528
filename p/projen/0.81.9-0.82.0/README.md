# Comparing `tmp/projen-0.81.9.tar.gz` & `tmp/projen-0.82.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.81.9.tar", last modified: Fri May 10 08:52:21 2024, max compression
+gzip compressed data, was "projen-0.82.0.tar", last modified: Tue May 28 11:15:29 2024, max compression
```

## Comparing `projen-0.81.9.tar` & `projen-0.82.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.862256 projen-0.81.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-10 08:52:11.000000 projen-0.81.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 08:52:11.000000 projen-0.81.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-10 08:52:21.862256 projen-0.81.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-05-10 08:52:11.000000 projen-0.81.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 08:52:11.000000 projen-0.81.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:52:21.862256 projen-0.81.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-10 08:52:11.000000 projen-0.81.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.842256 projen-0.81.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.846256 projen-0.81.9/src/projen/
--rw-r--r--   0 runner    (1001) docker     (127)   653934 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.846256 projen-0.81.9/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.850256 projen-0.81.9/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (127)  2641567 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/_jsii/projen@0.81.9.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.850256 projen-0.81.9/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.850256 projen-0.81.9/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (127)   409613 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)   202810 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.858256 projen-0.81.9/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)   844523 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.858256 projen-0.81.9/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.858256 projen-0.81.9/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.858256 projen-0.81.9/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.858256 projen-0.81.9/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.858256 projen-0.81.9/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.846256 projen-0.81.9/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-10 08:52:21.000000 projen-0.81.9/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-10 08:52:21.000000 projen-0.81.9/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:52:21.000000 projen-0.81.9/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-10 08:52:21.000000 projen-0.81.9/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 08:52:21.000000 projen-0.81.9/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.804165 projen-0.82.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-28 11:15:19.000000 projen-0.82.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 11:15:19.000000 projen-0.82.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-28 11:15:29.804165 projen-0.82.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-05-28 11:15:19.000000 projen-0.82.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-28 11:15:19.000000 projen-0.82.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:15:29.804165 projen-0.82.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-28 11:15:19.000000 projen-0.82.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.788165 projen-0.82.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.792165 projen-0.82.0/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (127)   653934 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.792165 projen-0.82.0/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.796165 projen-0.82.0/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (127)  2649232 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/_jsii/projen@0.82.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.796165 projen-0.82.0/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.796165 projen-0.82.0/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.796165 projen-0.82.0/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.796165 projen-0.82.0/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.800166 projen-0.82.0/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.800166 projen-0.82.0/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.800166 projen-0.82.0/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (127)   425340 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.800166 projen-0.82.0/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.800166 projen-0.82.0/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)   202836 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.800166 projen-0.82.0/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.800166 projen-0.82.0/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)   844517 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.800166 projen-0.82.0/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.804165 projen-0.82.0/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.804165 projen-0.82.0/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.804165 projen-0.82.0/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.804165 projen-0.82.0/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-05-28 11:15:19.000000 projen-0.82.0/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:15:29.792165 projen-0.82.0/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-28 11:15:29.000000 projen-0.82.0/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-28 11:15:29.000000 projen-0.82.0/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:15:29.000000 projen-0.82.0/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-28 11:15:29.000000 projen-0.82.0/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 11:15:29.000000 projen-0.82.0/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.81.9/LICENSE` & `projen-0.82.0/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/PKG-INFO` & `projen-0.82.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.81.9
+Version: 0.82.0
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.81.9/README.md` & `projen-0.82.0/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/setup.py` & `projen-0.82.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.81.9",
+    "version": "0.82.0",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.81.9.jsii.tgz"
+            "projen@0.82.0.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `projen-0.81.9/src/projen/__init__.py` & `projen-0.82.0/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/awscdk/__init__.py` & `projen-0.82.0/src/projen/awscdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/build/__init__.py` & `projen-0.82.0/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/cdk/__init__.py` & `projen-0.82.0/src/projen/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/cdk8s/__init__.py` & `projen-0.82.0/src/projen/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/cdktf/__init__.py` & `projen-0.82.0/src/projen/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/circleci/__init__.py` & `projen-0.82.0/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/github/__init__.py` & `projen-0.82.0/src/projen/github/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import constructs as _constructs_77d1e7e8
 from .. import (
     Component as _Component_2b0ad27f,
     GitOptions as _GitOptions_a65916a3,
     Gitpod as _Gitpod_5d9b9d87,
     GroupRunnerOptions as _GroupRunnerOptions_148c59c1,
     IgnoreFileOptions as _IgnoreFileOptions_86c48b91,
+    JsonFile as _JsonFile_fa8164db,
     LoggerOptions as _LoggerOptions_eb0f6309,
     Project as _Project_57d89203,
     ProjectOptions as _ProjectOptions_0d5b93c6,
     ProjectType as _ProjectType_fd80c725,
     ProjenrcJsonOptions as _ProjenrcJsonOptions_9c40dd4f,
     RenovatebotOptions as _RenovatebotOptions_18e6b8a1,
     SampleReadmeProps as _SampleReadmeProps_3518b03b,
@@ -2313,25 +2314,29 @@
         project: _Project_57d89203,
         *,
         download_lfs: typing.Optional[builtins.bool] = None,
         mergify: typing.Optional[builtins.bool] = None,
         mergify_options: typing.Optional[typing.Union["MergifyOptions", typing.Dict[builtins.str, typing.Any]]] = None,
         projen_credentials: typing.Optional["GithubCredentials"] = None,
         projen_token_secret: typing.Optional[builtins.str] = None,
+        pull_request_backport: typing.Optional[builtins.bool] = None,
+        pull_request_backport_options: typing.Optional[typing.Union["PullRequestBackportOptions", typing.Dict[builtins.str, typing.Any]]] = None,
         pull_request_lint: typing.Optional[builtins.bool] = None,
         pull_request_lint_options: typing.Optional[typing.Union["PullRequestLintOptions", typing.Dict[builtins.str, typing.Any]]] = None,
         workflows: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param project: -
         :param download_lfs: (experimental) Download files in LFS in workflows. Default: true if the associated project has ``lfsPatterns``, ``false`` otherwise
         :param mergify: (experimental) Whether mergify should be enabled on this repository or not. Default: true
         :param mergify_options: (experimental) Options for Mergify. Default: - default options
         :param projen_credentials: (experimental) Choose a method of providing GitHub API access for projen workflows. Default: - use a personal access token named PROJEN_GITHUB_TOKEN
         :param projen_token_secret: (deprecated) The name of a secret which includes a GitHub Personal Access Token to be used by projen workflows. This token needs to have the ``repo``, ``workflows`` and ``packages`` scope. Default: "PROJEN_GITHUB_TOKEN"
+        :param pull_request_backport: (experimental) Add a workflow that allows backport of PRs to other branches using labels. When opening a new PR add a backport label to it, and the PR will be backported to the target branches once the PR is merged. Should not be used together with mergify. Default: false
+        :param pull_request_backport_options: (experimental) Options for configuring pull request backport. Default: - see defaults in ``PullRequestBackportOptions``
         :param pull_request_lint: (experimental) Add a workflow that performs basic checks for pull requests, like validating that PRs follow Conventional Commits. Default: true
         :param pull_request_lint_options: (experimental) Options for configuring a pull request linter. Default: - see defaults in ``PullRequestLintOptions``
         :param workflows: (experimental) Enables GitHub workflows. If this is set to ``false``, workflows will not be created. Default: true
 
         :stability: experimental
         '''
         if __debug__:
@@ -2339,14 +2344,16 @@
             check_type(argname="argument project", value=project, expected_type=type_hints["project"])
         options = GitHubOptions(
             download_lfs=download_lfs,
             mergify=mergify,
             mergify_options=mergify_options,
             projen_credentials=projen_credentials,
             projen_token_secret=projen_token_secret,
+            pull_request_backport=pull_request_backport,
+            pull_request_backport_options=pull_request_backport_options,
             pull_request_lint=pull_request_lint,
             pull_request_lint_options=pull_request_lint_options,
             workflows=workflows,
         )
 
         jsii.create(self.__class__, self, [project, options])
 
@@ -2582,69 +2589,83 @@
     jsii_struct_bases=[],
     name_mapping={
         "download_lfs": "downloadLfs",
         "mergify": "mergify",
         "mergify_options": "mergifyOptions",
         "projen_credentials": "projenCredentials",
         "projen_token_secret": "projenTokenSecret",
+        "pull_request_backport": "pullRequestBackport",
+        "pull_request_backport_options": "pullRequestBackportOptions",
         "pull_request_lint": "pullRequestLint",
         "pull_request_lint_options": "pullRequestLintOptions",
         "workflows": "workflows",
     },
 )
 class GitHubOptions:
     def __init__(
         self,
         *,
         download_lfs: typing.Optional[builtins.bool] = None,
         mergify: typing.Optional[builtins.bool] = None,
         mergify_options: typing.Optional[typing.Union["MergifyOptions", typing.Dict[builtins.str, typing.Any]]] = None,
         projen_credentials: typing.Optional["GithubCredentials"] = None,
         projen_token_secret: typing.Optional[builtins.str] = None,
+        pull_request_backport: typing.Optional[builtins.bool] = None,
+        pull_request_backport_options: typing.Optional[typing.Union["PullRequestBackportOptions", typing.Dict[builtins.str, typing.Any]]] = None,
         pull_request_lint: typing.Optional[builtins.bool] = None,
         pull_request_lint_options: typing.Optional[typing.Union["PullRequestLintOptions", typing.Dict[builtins.str, typing.Any]]] = None,
         workflows: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param download_lfs: (experimental) Download files in LFS in workflows. Default: true if the associated project has ``lfsPatterns``, ``false`` otherwise
         :param mergify: (experimental) Whether mergify should be enabled on this repository or not. Default: true
         :param mergify_options: (experimental) Options for Mergify. Default: - default options
         :param projen_credentials: (experimental) Choose a method of providing GitHub API access for projen workflows. Default: - use a personal access token named PROJEN_GITHUB_TOKEN
         :param projen_token_secret: (deprecated) The name of a secret which includes a GitHub Personal Access Token to be used by projen workflows. This token needs to have the ``repo``, ``workflows`` and ``packages`` scope. Default: "PROJEN_GITHUB_TOKEN"
+        :param pull_request_backport: (experimental) Add a workflow that allows backport of PRs to other branches using labels. When opening a new PR add a backport label to it, and the PR will be backported to the target branches once the PR is merged. Should not be used together with mergify. Default: false
+        :param pull_request_backport_options: (experimental) Options for configuring pull request backport. Default: - see defaults in ``PullRequestBackportOptions``
         :param pull_request_lint: (experimental) Add a workflow that performs basic checks for pull requests, like validating that PRs follow Conventional Commits. Default: true
         :param pull_request_lint_options: (experimental) Options for configuring a pull request linter. Default: - see defaults in ``PullRequestLintOptions``
         :param workflows: (experimental) Enables GitHub workflows. If this is set to ``false``, workflows will not be created. Default: true
 
         :stability: experimental
         '''
         if isinstance(mergify_options, dict):
             mergify_options = MergifyOptions(**mergify_options)
+        if isinstance(pull_request_backport_options, dict):
+            pull_request_backport_options = PullRequestBackportOptions(**pull_request_backport_options)
         if isinstance(pull_request_lint_options, dict):
             pull_request_lint_options = PullRequestLintOptions(**pull_request_lint_options)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c22e66f011c96f13a6f4e5b07bb676bf98b477678e968ee61f79ee107a7d2bd7)
             check_type(argname="argument download_lfs", value=download_lfs, expected_type=type_hints["download_lfs"])
             check_type(argname="argument mergify", value=mergify, expected_type=type_hints["mergify"])
             check_type(argname="argument mergify_options", value=mergify_options, expected_type=type_hints["mergify_options"])
             check_type(argname="argument projen_credentials", value=projen_credentials, expected_type=type_hints["projen_credentials"])
             check_type(argname="argument projen_token_secret", value=projen_token_secret, expected_type=type_hints["projen_token_secret"])
+            check_type(argname="argument pull_request_backport", value=pull_request_backport, expected_type=type_hints["pull_request_backport"])
+            check_type(argname="argument pull_request_backport_options", value=pull_request_backport_options, expected_type=type_hints["pull_request_backport_options"])
             check_type(argname="argument pull_request_lint", value=pull_request_lint, expected_type=type_hints["pull_request_lint"])
             check_type(argname="argument pull_request_lint_options", value=pull_request_lint_options, expected_type=type_hints["pull_request_lint_options"])
             check_type(argname="argument workflows", value=workflows, expected_type=type_hints["workflows"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if download_lfs is not None:
             self._values["download_lfs"] = download_lfs
         if mergify is not None:
             self._values["mergify"] = mergify
         if mergify_options is not None:
             self._values["mergify_options"] = mergify_options
         if projen_credentials is not None:
             self._values["projen_credentials"] = projen_credentials
         if projen_token_secret is not None:
             self._values["projen_token_secret"] = projen_token_secret
+        if pull_request_backport is not None:
+            self._values["pull_request_backport"] = pull_request_backport
+        if pull_request_backport_options is not None:
+            self._values["pull_request_backport_options"] = pull_request_backport_options
         if pull_request_lint is not None:
             self._values["pull_request_lint"] = pull_request_lint
         if pull_request_lint_options is not None:
             self._values["pull_request_lint_options"] = pull_request_lint_options
         if workflows is not None:
             self._values["workflows"] = workflows
 
@@ -2705,14 +2726,43 @@
 
         :stability: deprecated
         '''
         result = self._values.get("projen_token_secret")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def pull_request_backport(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Add a workflow that allows backport of PRs to other branches using labels.
+
+        When opening a new PR add a backport label to it,
+        and the PR will be backported to the target branches once the PR is merged.
+
+        Should not be used together with mergify.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("pull_request_backport")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def pull_request_backport_options(
+        self,
+    ) -> typing.Optional["PullRequestBackportOptions"]:
+        '''(experimental) Options for configuring pull request backport.
+
+        :default: - see defaults in ``PullRequestBackportOptions``
+
+        :stability: experimental
+        '''
+        result = self._values.get("pull_request_backport_options")
+        return typing.cast(typing.Optional["PullRequestBackportOptions"], result)
+
+    @builtins.property
     def pull_request_lint(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Add a workflow that performs basic checks for pull requests, like validating that PRs follow Conventional Commits.
 
         :default: true
 
         :stability: experimental
         '''
@@ -4596,14 +4646,234 @@
 
     def __repr__(self) -> str:
         return "MergifyRule(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class PullRequestBackport(
+    _Component_2b0ad27f,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="projen.github.PullRequestBackport",
+):
+    '''
+    :stability: experimental
+    '''
+
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.IConstruct,
+        *,
+        auto_approve_backport: typing.Optional[builtins.bool] = None,
+        backport_branch_name_prefix: typing.Optional[builtins.str] = None,
+        backport_pr_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
+        branches: typing.Optional[typing.Sequence[builtins.str]] = None,
+        create_with_conflicts: typing.Optional[builtins.bool] = None,
+        label_prefix: typing.Optional[builtins.str] = None,
+        workflow_name: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param scope: -
+        :param auto_approve_backport: (experimental) Automatically approve backport PRs if the 'auto approve' workflow is available. Default: true
+        :param backport_branch_name_prefix: (experimental) The prefix used to name backport branches. Make sure to include a separator at the end like ``/`` or ``_``. Default: "backport/"
+        :param backport_pr_labels: (experimental) The labels added to the created backport PR. Default: ["backport"]
+        :param branches: (experimental) List of branches that can be a target for backports. Default: - allow backports to all release branches
+        :param create_with_conflicts: (experimental) Should this created Backport PRs with conflicts. Conflicts will have to be resolved manually, but a PR is always created. Set to ``false`` to prevent the backport PR from being created if there are conflicts. Default: true
+        :param label_prefix: (experimental) The prefix used to detect PRs that should be backported. Default: "backport-to-"
+        :param workflow_name: (experimental) The name of the workflow. Default: "backport"
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a321227b5ffc19f1220367db19ad9a6c84aec3e2bf74ba19db5a89f3ee8c9ce4)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+        options = PullRequestBackportOptions(
+            auto_approve_backport=auto_approve_backport,
+            backport_branch_name_prefix=backport_branch_name_prefix,
+            backport_pr_labels=backport_pr_labels,
+            branches=branches,
+            create_with_conflicts=create_with_conflicts,
+            label_prefix=label_prefix,
+            workflow_name=workflow_name,
+        )
+
+        jsii.create(self.__class__, self, [scope, options])
+
+    @builtins.property
+    @jsii.member(jsii_name="file")
+    def file(self) -> _JsonFile_fa8164db:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(_JsonFile_fa8164db, jsii.get(self, "file"))
+
+    @builtins.property
+    @jsii.member(jsii_name="workflow")
+    def workflow(self) -> GithubWorkflow:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(GithubWorkflow, jsii.get(self, "workflow"))
+
+
+@jsii.data_type(
+    jsii_type="projen.github.PullRequestBackportOptions",
+    jsii_struct_bases=[],
+    name_mapping={
+        "auto_approve_backport": "autoApproveBackport",
+        "backport_branch_name_prefix": "backportBranchNamePrefix",
+        "backport_pr_labels": "backportPRLabels",
+        "branches": "branches",
+        "create_with_conflicts": "createWithConflicts",
+        "label_prefix": "labelPrefix",
+        "workflow_name": "workflowName",
+    },
+)
+class PullRequestBackportOptions:
+    def __init__(
+        self,
+        *,
+        auto_approve_backport: typing.Optional[builtins.bool] = None,
+        backport_branch_name_prefix: typing.Optional[builtins.str] = None,
+        backport_pr_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
+        branches: typing.Optional[typing.Sequence[builtins.str]] = None,
+        create_with_conflicts: typing.Optional[builtins.bool] = None,
+        label_prefix: typing.Optional[builtins.str] = None,
+        workflow_name: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param auto_approve_backport: (experimental) Automatically approve backport PRs if the 'auto approve' workflow is available. Default: true
+        :param backport_branch_name_prefix: (experimental) The prefix used to name backport branches. Make sure to include a separator at the end like ``/`` or ``_``. Default: "backport/"
+        :param backport_pr_labels: (experimental) The labels added to the created backport PR. Default: ["backport"]
+        :param branches: (experimental) List of branches that can be a target for backports. Default: - allow backports to all release branches
+        :param create_with_conflicts: (experimental) Should this created Backport PRs with conflicts. Conflicts will have to be resolved manually, but a PR is always created. Set to ``false`` to prevent the backport PR from being created if there are conflicts. Default: true
+        :param label_prefix: (experimental) The prefix used to detect PRs that should be backported. Default: "backport-to-"
+        :param workflow_name: (experimental) The name of the workflow. Default: "backport"
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__066696cdba0d516ea035e9580a9e5c79c5a552ca23f78e5291d21811124a2a62)
+            check_type(argname="argument auto_approve_backport", value=auto_approve_backport, expected_type=type_hints["auto_approve_backport"])
+            check_type(argname="argument backport_branch_name_prefix", value=backport_branch_name_prefix, expected_type=type_hints["backport_branch_name_prefix"])
+            check_type(argname="argument backport_pr_labels", value=backport_pr_labels, expected_type=type_hints["backport_pr_labels"])
+            check_type(argname="argument branches", value=branches, expected_type=type_hints["branches"])
+            check_type(argname="argument create_with_conflicts", value=create_with_conflicts, expected_type=type_hints["create_with_conflicts"])
+            check_type(argname="argument label_prefix", value=label_prefix, expected_type=type_hints["label_prefix"])
+            check_type(argname="argument workflow_name", value=workflow_name, expected_type=type_hints["workflow_name"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if auto_approve_backport is not None:
+            self._values["auto_approve_backport"] = auto_approve_backport
+        if backport_branch_name_prefix is not None:
+            self._values["backport_branch_name_prefix"] = backport_branch_name_prefix
+        if backport_pr_labels is not None:
+            self._values["backport_pr_labels"] = backport_pr_labels
+        if branches is not None:
+            self._values["branches"] = branches
+        if create_with_conflicts is not None:
+            self._values["create_with_conflicts"] = create_with_conflicts
+        if label_prefix is not None:
+            self._values["label_prefix"] = label_prefix
+        if workflow_name is not None:
+            self._values["workflow_name"] = workflow_name
+
+    @builtins.property
+    def auto_approve_backport(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Automatically approve backport PRs if the 'auto approve' workflow is available.
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("auto_approve_backport")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def backport_branch_name_prefix(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The prefix used to name backport branches.
+
+        Make sure to include a separator at the end like ``/`` or ``_``.
+
+        :default: "backport/"
+
+        :stability: experimental
+        '''
+        result = self._values.get("backport_branch_name_prefix")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def backport_pr_labels(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''(experimental) The labels added to the created backport PR.
+
+        :default: ["backport"]
+
+        :stability: experimental
+        '''
+        result = self._values.get("backport_pr_labels")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
+    def branches(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''(experimental) List of branches that can be a target for backports.
+
+        :default: - allow backports to all release branches
+
+        :stability: experimental
+        '''
+        result = self._values.get("branches")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
+    def create_with_conflicts(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Should this created Backport PRs with conflicts.
+
+        Conflicts will have to be resolved manually, but a PR is always created.
+        Set to ``false`` to prevent the backport PR from being created if there are conflicts.
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("create_with_conflicts")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def label_prefix(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The prefix used to detect PRs that should be backported.
+
+        :default: "backport-to-"
+
+        :stability: experimental
+        '''
+        result = self._values.get("label_prefix")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def workflow_name(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The name of the workflow.
+
+        :default: "backport"
+
+        :stability: experimental
+        '''
+        result = self._values.get("workflow_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "PullRequestBackportOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 @jsii.data_type(
     jsii_type="projen.github.PullRequestFromPatchOptions",
     jsii_struct_bases=[CreatePullRequestOptions],
     name_mapping={
         "pull_request_description": "pullRequestDescription",
         "pull_request_title": "pullRequestTitle",
         "workflow_name": "workflowName",
@@ -7892,14 +8162,16 @@
     "GithubWorkflowOptions",
     "IAddConditionsLater",
     "Mergify",
     "MergifyConditionalOperator",
     "MergifyOptions",
     "MergifyQueue",
     "MergifyRule",
+    "PullRequestBackport",
+    "PullRequestBackportOptions",
     "PullRequestFromPatchOptions",
     "PullRequestLint",
     "PullRequestLintOptions",
     "PullRequestPatchSource",
     "PullRequestTemplate",
     "PullRequestTemplateOptions",
     "SemanticTitleOptions",
@@ -8163,14 +8435,16 @@
     project: _Project_57d89203,
     *,
     download_lfs: typing.Optional[builtins.bool] = None,
     mergify: typing.Optional[builtins.bool] = None,
     mergify_options: typing.Optional[typing.Union[MergifyOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     projen_credentials: typing.Optional[GithubCredentials] = None,
     projen_token_secret: typing.Optional[builtins.str] = None,
+    pull_request_backport: typing.Optional[builtins.bool] = None,
+    pull_request_backport_options: typing.Optional[typing.Union[PullRequestBackportOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     pull_request_lint: typing.Optional[builtins.bool] = None,
     pull_request_lint_options: typing.Optional[typing.Union[PullRequestLintOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     workflows: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -8214,14 +8488,16 @@
 def _typecheckingstub__c22e66f011c96f13a6f4e5b07bb676bf98b477678e968ee61f79ee107a7d2bd7(
     *,
     download_lfs: typing.Optional[builtins.bool] = None,
     mergify: typing.Optional[builtins.bool] = None,
     mergify_options: typing.Optional[typing.Union[MergifyOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     projen_credentials: typing.Optional[GithubCredentials] = None,
     projen_token_secret: typing.Optional[builtins.str] = None,
+    pull_request_backport: typing.Optional[builtins.bool] = None,
+    pull_request_backport_options: typing.Optional[typing.Union[PullRequestBackportOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     pull_request_lint: typing.Optional[builtins.bool] = None,
     pull_request_lint_options: typing.Optional[typing.Union[PullRequestLintOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     workflows: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -8392,14 +8668,41 @@
     actions: typing.Mapping[builtins.str, typing.Any],
     conditions: typing.Sequence[typing.Union[builtins.str, typing.Union[MergifyConditionalOperator, typing.Dict[builtins.str, typing.Any]]]],
     name: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__a321227b5ffc19f1220367db19ad9a6c84aec3e2bf74ba19db5a89f3ee8c9ce4(
+    scope: _constructs_77d1e7e8.IConstruct,
+    *,
+    auto_approve_backport: typing.Optional[builtins.bool] = None,
+    backport_branch_name_prefix: typing.Optional[builtins.str] = None,
+    backport_pr_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
+    branches: typing.Optional[typing.Sequence[builtins.str]] = None,
+    create_with_conflicts: typing.Optional[builtins.bool] = None,
+    label_prefix: typing.Optional[builtins.str] = None,
+    workflow_name: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__066696cdba0d516ea035e9580a9e5c79c5a552ca23f78e5291d21811124a2a62(
+    *,
+    auto_approve_backport: typing.Optional[builtins.bool] = None,
+    backport_branch_name_prefix: typing.Optional[builtins.str] = None,
+    backport_pr_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
+    branches: typing.Optional[typing.Sequence[builtins.str]] = None,
+    create_with_conflicts: typing.Optional[builtins.bool] = None,
+    label_prefix: typing.Optional[builtins.str] = None,
+    workflow_name: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__0c1e5279fc8c18480c3113cc60b389aa13938b2052436bbdcb3069cfe669fa47(
     *,
     pull_request_description: builtins.str,
     pull_request_title: builtins.str,
     workflow_name: builtins.str,
     assignees: typing.Optional[typing.Sequence[builtins.str]] = None,
     base_branch: typing.Optional[builtins.str] = None,
```

### Comparing `projen-0.81.9/src/projen/github/workflows/__init__.py` & `projen-0.82.0/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/gitlab/__init__.py` & `projen-0.82.0/src/projen/gitlab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11138,1539 +11138,1541 @@
 0002b810: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
 0002b820: 672e 4d61 7070 696e 675b 6275 696c 7469  g.Mapping[builti
 0002b830: 6e73 2e73 7472 2c20 7479 7069 6e67 2e55  ns.str, typing.U
 0002b840: 6e69 6f6e 5b62 7569 6c74 696e 732e 7374  nion[builtins.st
 0002b850: 722c 206a 7369 692e 4e75 6d62 6572 5d5d  r, jsii.Number]]
 0002b860: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
 0002b870: 2020 7768 656e 3a20 7479 7069 6e67 2e4f    when: typing.O
-0002b880: 7074 696f 6e61 6c5b 4a6f 6257 6865 6e5d  ptional[JobWhen]
-0002b890: 203d 204e 6f6e 652c 0a20 2020 2029 202d   = None,.    ) -
-0002b8a0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0002b8b0: 2727 2728 6578 7065 7269 6d65 6e74 616c  '''(experimental
-0002b8c0: 2920 5573 6564 2074 6f20 636f 6e74 726f  ) Used to contro
-0002b8d0: 6c20 7768 6574 6865 7220 6f72 206e 6f74  l whether or not
-0002b8e0: 2061 2077 686f 6c65 2070 6970 656c 696e   a whole pipelin
-0002b8f0: 6520 6973 2063 7265 6174 6564 2e0a 0a20  e is created... 
-0002b900: 2020 2020 2020 203a 7061 7261 6d20 6368         :param ch
-0002b910: 616e 6765 733a 200a 2020 2020 2020 2020  anges: .        
-0002b920: 3a70 6172 616d 2065 7869 7374 733a 200a  :param exists: .
-0002b930: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-0002b940: 665f 3a20 0a20 2020 2020 2020 203a 7061  f_: .        :pa
-0002b950: 7261 6d20 7661 7269 6162 6c65 733a 200a  ram variables: .
-0002b960: 2020 2020 2020 2020 3a70 6172 616d 2077          :param w
-0002b970: 6865 6e3a 200a 0a20 2020 2020 2020 203a  hen: ..        :
-0002b980: 7365 653a 2068 7474 7073 3a2f 2f64 6f63  see: https://doc
-0002b990: 732e 6769 746c 6162 2e63 6f6d 2f65 652f  s.gitlab.com/ee/
-0002b9a0: 6369 2f79 616d 6c2f 2377 6f72 6b66 6c6f  ci/yaml/#workflo
-0002b9b0: 7772 756c 6573 0a20 2020 2020 2020 203a  wrules.        :
-0002b9c0: 7374 6162 696c 6974 793a 2065 7870 6572  stability: exper
-0002b9d0: 696d 656e 7461 6c0a 2020 2020 2020 2020  imental.        
-0002b9e0: 2727 270a 2020 2020 2020 2020 6966 205f  '''.        if _
-0002b9f0: 5f64 6562 7567 5f5f 3a0a 2020 2020 2020  _debug__:.      
-0002ba00: 2020 2020 2020 7479 7065 5f68 696e 7473        type_hints
-0002ba10: 203d 2074 7970 696e 672e 6765 745f 7479   = typing.get_ty
-0002ba20: 7065 5f68 696e 7473 285f 7479 7065 6368  pe_hints(_typech
-0002ba30: 6563 6b69 6e67 7374 7562 5f5f 3031 6132  eckingstub__01a2
-0002ba40: 6366 3463 3261 3938 3261 3734 3964 3132  cf4c2a982a749d12
-0002ba50: 3531 3164 3965 3433 3436 3866 3362 3461  511d9e43468f3b4a
-0002ba60: 3963 6361 3136 6436 6335 3664 3961 3263  9cca16d6c56d9a2c
-0002ba70: 6664 3131 3534 3732 3064 3633 290a 2020  fd1154720d63).  
-0002ba80: 2020 2020 2020 2020 2020 6368 6563 6b5f            check_
-0002ba90: 7479 7065 2861 7267 6e61 6d65 3d22 6172  type(argname="ar
-0002baa0: 6775 6d65 6e74 2063 6861 6e67 6573 222c  gument changes",
-0002bab0: 2076 616c 7565 3d63 6861 6e67 6573 2c20   value=changes, 
-0002bac0: 6578 7065 6374 6564 5f74 7970 653d 7479  expected_type=ty
-0002bad0: 7065 5f68 696e 7473 5b22 6368 616e 6765  pe_hints["change
-0002bae0: 7322 5d29 0a20 2020 2020 2020 2020 2020  s"]).           
-0002baf0: 2063 6865 636b 5f74 7970 6528 6172 676e   check_type(argn
-0002bb00: 616d 653d 2261 7267 756d 656e 7420 6578  ame="argument ex
-0002bb10: 6973 7473 222c 2076 616c 7565 3d65 7869  ists", value=exi
-0002bb20: 7374 732c 2065 7870 6563 7465 645f 7479  sts, expected_ty
-0002bb30: 7065 3d74 7970 655f 6869 6e74 735b 2265  pe=type_hints["e
-0002bb40: 7869 7374 7322 5d29 0a20 2020 2020 2020  xists"]).       
-0002bb50: 2020 2020 2063 6865 636b 5f74 7970 6528       check_type(
-0002bb60: 6172 676e 616d 653d 2261 7267 756d 656e  argname="argumen
-0002bb70: 7420 6966 5f22 2c20 7661 6c75 653d 6966  t if_", value=if
-0002bb80: 5f2c 2065 7870 6563 7465 645f 7479 7065  _, expected_type
-0002bb90: 3d74 7970 655f 6869 6e74 735b 2269 665f  =type_hints["if_
-0002bba0: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
-0002bbb0: 6368 6563 6b5f 7479 7065 2861 7267 6e61  check_type(argna
-0002bbc0: 6d65 3d22 6172 6775 6d65 6e74 2076 6172  me="argument var
-0002bbd0: 6961 626c 6573 222c 2076 616c 7565 3d76  iables", value=v
-0002bbe0: 6172 6961 626c 6573 2c20 6578 7065 6374  ariables, expect
-0002bbf0: 6564 5f74 7970 653d 7479 7065 5f68 696e  ed_type=type_hin
-0002bc00: 7473 5b22 7661 7269 6162 6c65 7322 5d29  ts["variables"])
-0002bc10: 0a20 2020 2020 2020 2020 2020 2063 6865  .            che
-0002bc20: 636b 5f74 7970 6528 6172 676e 616d 653d  ck_type(argname=
-0002bc30: 2261 7267 756d 656e 7420 7768 656e 222c  "argument when",
-0002bc40: 2076 616c 7565 3d77 6865 6e2c 2065 7870   value=when, exp
-0002bc50: 6563 7465 645f 7479 7065 3d74 7970 655f  ected_type=type_
-0002bc60: 6869 6e74 735b 2277 6865 6e22 5d29 0a20  hints["when"]). 
-0002bc70: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
-0002bc80: 7565 733a 2074 7970 696e 672e 4469 6374  ues: typing.Dict
-0002bc90: 5b62 7569 6c74 696e 732e 7374 722c 2074  [builtins.str, t
-0002bca0: 7970 696e 672e 416e 795d 203d 207b 7d0a  yping.Any] = {}.
-0002bcb0: 2020 2020 2020 2020 6966 2063 6861 6e67          if chang
-0002bcc0: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
-0002bcd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002bce0: 2e5f 7661 6c75 6573 5b22 6368 616e 6765  ._values["change
-0002bcf0: 7322 5d20 3d20 6368 616e 6765 730a 2020  s"] = changes.  
-0002bd00: 2020 2020 2020 6966 2065 7869 7374 7320        if exists 
-0002bd10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002bd20: 2020 2020 2020 2020 2073 656c 662e 5f76           self._v
-0002bd30: 616c 7565 735b 2265 7869 7374 7322 5d20  alues["exists"] 
-0002bd40: 3d20 6578 6973 7473 0a20 2020 2020 2020  = exists.       
-0002bd50: 2069 6620 6966 5f20 6973 206e 6f74 204e   if if_ is not N
-0002bd60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002bd70: 2073 656c 662e 5f76 616c 7565 735b 2269   self._values["i
-0002bd80: 665f 225d 203d 2069 665f 0a20 2020 2020  f_"] = if_.     
-0002bd90: 2020 2069 6620 7661 7269 6162 6c65 7320     if variables 
-0002bda0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002bdb0: 2020 2020 2020 2020 2073 656c 662e 5f76           self._v
-0002bdc0: 616c 7565 735b 2276 6172 6961 626c 6573  alues["variables
-0002bdd0: 225d 203d 2076 6172 6961 626c 6573 0a20  "] = variables. 
-0002bde0: 2020 2020 2020 2069 6620 7768 656e 2069         if when i
-0002bdf0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002be00: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
-0002be10: 6c75 6573 5b22 7768 656e 225d 203d 2077  lues["when"] = w
-0002be20: 6865 6e0a 0a20 2020 2040 6275 696c 7469  hen..    @builti
-0002be30: 6e73 2e70 726f 7065 7274 790a 2020 2020  ns.property.    
-0002be40: 6465 6620 6368 616e 6765 7328 7365 6c66  def changes(self
-0002be50: 2920 2d3e 2074 7970 696e 672e 4f70 7469  ) -> typing.Opti
-0002be60: 6f6e 616c 5b74 7970 696e 672e 4c69 7374  onal[typing.List
-0002be70: 5b62 7569 6c74 696e 732e 7374 725d 5d3a  [builtins.str]]:
-0002be80: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-0002be90: 2020 2020 203a 7374 6162 696c 6974 793a       :stability:
-0002bea0: 2065 7870 6572 696d 656e 7461 6c0a 2020   experimental.  
-0002beb0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0002bec0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-0002bed0: 5f76 616c 7565 732e 6765 7428 2263 6861  _values.get("cha
-0002bee0: 6e67 6573 2229 0a20 2020 2020 2020 2072  nges").        r
-0002bef0: 6574 7572 6e20 7479 7069 6e67 2e63 6173  eturn typing.cas
-0002bf00: 7428 7479 7069 6e67 2e4f 7074 696f 6e61  t(typing.Optiona
-0002bf10: 6c5b 7479 7069 6e67 2e4c 6973 745b 6275  l[typing.List[bu
-0002bf20: 696c 7469 6e73 2e73 7472 5d5d 2c20 7265  iltins.str]], re
-0002bf30: 7375 6c74 290a 0a20 2020 2040 6275 696c  sult)..    @buil
-0002bf40: 7469 6e73 2e70 726f 7065 7274 790a 2020  tins.property.  
-0002bf50: 2020 6465 6620 6578 6973 7473 2873 656c    def exists(sel
-0002bf60: 6629 202d 3e20 7479 7069 6e67 2e4f 7074  f) -> typing.Opt
-0002bf70: 696f 6e61 6c5b 7479 7069 6e67 2e4c 6973  ional[typing.Lis
-0002bf80: 745b 6275 696c 7469 6e73 2e73 7472 5d5d  t[builtins.str]]
-0002bf90: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-0002bfa0: 2020 2020 2020 3a73 7461 6269 6c69 7479        :stability
-0002bfb0: 3a20 6578 7065 7269 6d65 6e74 616c 0a20  : experimental. 
-0002bfc0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-0002bfd0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-0002bfe0: 2e5f 7661 6c75 6573 2e67 6574 2822 6578  ._values.get("ex
-0002bff0: 6973 7473 2229 0a20 2020 2020 2020 2072  ists").        r
-0002c000: 6574 7572 6e20 7479 7069 6e67 2e63 6173  eturn typing.cas
-0002c010: 7428 7479 7069 6e67 2e4f 7074 696f 6e61  t(typing.Optiona
-0002c020: 6c5b 7479 7069 6e67 2e4c 6973 745b 6275  l[typing.List[bu
-0002c030: 696c 7469 6e73 2e73 7472 5d5d 2c20 7265  iltins.str]], re
-0002c040: 7375 6c74 290a 0a20 2020 2040 6275 696c  sult)..    @buil
-0002c050: 7469 6e73 2e70 726f 7065 7274 790a 2020  tins.property.  
-0002c060: 2020 6465 6620 6966 5f28 7365 6c66 2920    def if_(self) 
-0002c070: 2d3e 2074 7970 696e 672e 4f70 7469 6f6e  -> typing.Option
-0002c080: 616c 5b62 7569 6c74 696e 732e 7374 725d  al[builtins.str]
-0002c090: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-0002c0a0: 2020 2020 2020 3a73 7461 6269 6c69 7479        :stability
-0002c0b0: 3a20 6578 7065 7269 6d65 6e74 616c 0a20  : experimental. 
-0002c0c0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-0002c0d0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-0002c0e0: 2e5f 7661 6c75 6573 2e67 6574 2822 6966  ._values.get("if
-0002c0f0: 5f22 290a 2020 2020 2020 2020 7265 7475  _").        retu
-0002c100: 726e 2074 7970 696e 672e 6361 7374 2874  rn typing.cast(t
-0002c110: 7970 696e 672e 4f70 7469 6f6e 616c 5b62  yping.Optional[b
-0002c120: 7569 6c74 696e 732e 7374 725d 2c20 7265  uiltins.str], re
-0002c130: 7375 6c74 290a 0a20 2020 2040 6275 696c  sult)..    @buil
-0002c140: 7469 6e73 2e70 726f 7065 7274 790a 2020  tins.property.  
-0002c150: 2020 6465 6620 7661 7269 6162 6c65 7328    def variables(
-0002c160: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0002c170: 2020 2029 202d 3e20 7479 7069 6e67 2e4f     ) -> typing.O
-0002c180: 7074 696f 6e61 6c5b 7479 7069 6e67 2e4d  ptional[typing.M
-0002c190: 6170 7069 6e67 5b62 7569 6c74 696e 732e  apping[builtins.
-0002c1a0: 7374 722c 2074 7970 696e 672e 556e 696f  str, typing.Unio
-0002c1b0: 6e5b 6275 696c 7469 6e73 2e73 7472 2c20  n[builtins.str, 
-0002c1c0: 6a73 6969 2e4e 756d 6265 725d 5d5d 3a0a  jsii.Number]]]:.
-0002c1d0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0002c1e0: 2020 2020 3a73 7461 6269 6c69 7479 3a20      :stability: 
-0002c1f0: 6578 7065 7269 6d65 6e74 616c 0a20 2020  experimental.   
-0002c200: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-0002c210: 2072 6573 756c 7420 3d20 7365 6c66 2e5f   result = self._
-0002c220: 7661 6c75 6573 2e67 6574 2822 7661 7269  values.get("vari
-0002c230: 6162 6c65 7322 290a 2020 2020 2020 2020  ables").        
-0002c240: 7265 7475 726e 2074 7970 696e 672e 6361  return typing.ca
-0002c250: 7374 2874 7970 696e 672e 4f70 7469 6f6e  st(typing.Option
-0002c260: 616c 5b74 7970 696e 672e 4d61 7070 696e  al[typing.Mappin
-0002c270: 675b 6275 696c 7469 6e73 2e73 7472 2c20  g[builtins.str, 
-0002c280: 7479 7069 6e67 2e55 6e69 6f6e 5b62 7569  typing.Union[bui
-0002c290: 6c74 696e 732e 7374 722c 206a 7369 692e  ltins.str, jsii.
-0002c2a0: 4e75 6d62 6572 5d5d 5d2c 2072 6573 756c  Number]]], resul
-0002c2b0: 7429 0a0a 2020 2020 4062 7569 6c74 696e  t)..    @builtin
-0002c2c0: 732e 7072 6f70 6572 7479 0a20 2020 2064  s.property.    d
-0002c2d0: 6566 2077 6865 6e28 7365 6c66 2920 2d3e  ef when(self) ->
-0002c2e0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0002c2f0: 5b4a 6f62 5768 656e 5d3a 0a20 2020 2020  [JobWhen]:.     
-0002c300: 2020 2027 2727 0a20 2020 2020 2020 203a     '''.        :
-0002c310: 7374 6162 696c 6974 793a 2065 7870 6572  stability: exper
-0002c320: 696d 656e 7461 6c0a 2020 2020 2020 2020  imental.        
-0002c330: 2727 270a 2020 2020 2020 2020 7265 7375  '''.        resu
-0002c340: 6c74 203d 2073 656c 662e 5f76 616c 7565  lt = self._value
-0002c350: 732e 6765 7428 2277 6865 6e22 290a 2020  s.get("when").  
-0002c360: 2020 2020 2020 7265 7475 726e 2074 7970        return typ
-0002c370: 696e 672e 6361 7374 2874 7970 696e 672e  ing.cast(typing.
-0002c380: 4f70 7469 6f6e 616c 5b4a 6f62 5768 656e  Optional[JobWhen
-0002c390: 5d2c 2072 6573 756c 7429 0a0a 2020 2020  ], result)..    
-0002c3a0: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
-0002c3b0: 2072 6873 3a20 7479 7069 6e67 2e41 6e79   rhs: typing.Any
-0002c3c0: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
-0002c3d0: 6f6c 3a0a 2020 2020 2020 2020 7265 7475  ol:.        retu
-0002c3e0: 726e 2069 7369 6e73 7461 6e63 6528 7268  rn isinstance(rh
-0002c3f0: 732c 2073 656c 662e 5f5f 636c 6173 735f  s, self.__class_
-0002c400: 5f29 2061 6e64 2072 6873 2e5f 7661 6c75  _) and rhs._valu
-0002c410: 6573 203d 3d20 7365 6c66 2e5f 7661 6c75  es == self._valu
-0002c420: 6573 0a0a 2020 2020 6465 6620 5f5f 6e65  es..    def __ne
-0002c430: 5f5f 2873 656c 662c 2072 6873 3a20 7479  __(self, rhs: ty
-0002c440: 7069 6e67 2e41 6e79 2920 2d3e 2062 7569  ping.Any) -> bui
-0002c450: 6c74 696e 732e 626f 6f6c 3a0a 2020 2020  ltins.bool:.    
-0002c460: 2020 2020 7265 7475 726e 206e 6f74 2028      return not (
-0002c470: 7268 7320 3d3d 2073 656c 6629 0a0a 2020  rhs == self)..  
-0002c480: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
-0002c490: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
-0002c4a0: 2020 2020 2072 6574 7572 6e20 2257 6f72       return "Wor
-0002c4b0: 6b66 6c6f 7752 756c 6528 2573 2922 2025  kflowRule(%s)" %
-0002c4c0: 2022 2c20 222e 6a6f 696e 280a 2020 2020   ", ".join(.    
-0002c4d0: 2020 2020 2020 2020 6b20 2b20 223d 2220          k + "=" 
-0002c4e0: 2b20 7265 7072 2876 2920 666f 7220 6b2c  + repr(v) for k,
-0002c4f0: 2076 2069 6e20 7365 6c66 2e5f 7661 6c75   v in self._valu
-0002c500: 6573 2e69 7465 6d73 2829 0a20 2020 2020  es.items().     
-0002c510: 2020 2029 0a0a 0a40 6a73 6969 2e65 6e75     )...@jsii.enu
-0002c520: 6d28 6a73 6969 5f74 7970 653d 2270 726f  m(jsii_type="pro
-0002c530: 6a65 6e2e 6769 746c 6162 2e57 6f72 6b66  jen.gitlab.Workf
-0002c540: 6c6f 7757 6865 6e22 290a 636c 6173 7320  lowWhen").class 
-0002c550: 576f 726b 666c 6f77 5768 656e 2865 6e75  WorkflowWhen(enu
-0002c560: 6d2e 456e 756d 293a 0a20 2020 2027 2727  m.Enum):.    '''
-0002c570: 2865 7870 6572 696d 656e 7461 6c29 2044  (experimental) D
-0002c580: 6573 6372 6962 6573 2074 6865 2063 6f6e  escribes the con
-0002c590: 6469 7469 6f6e 7320 666f 7220 7768 656e  ditions for when
-0002c5a0: 2074 6f20 7275 6e20 7468 6520 6a6f 622e   to run the job.
-0002c5b0: 0a0a 2020 2020 4465 6661 756c 7473 2074  ..    Defaults t
-0002c5c0: 6f20 276f 6e5f 7375 6363 6573 7327 2e0a  o 'on_success'..
-0002c5d0: 2020 2020 5468 6520 7661 6c75 6520 6361      The value ca
-0002c5e0: 6e20 6f6e 6c79 2062 6520 2761 6c77 6179  n only be 'alway
-0002c5f0: 7327 206f 7220 276e 6576 6572 2720 7768  s' or 'never' wh
-0002c600: 656e 2075 7365 6420 7769 7468 2077 6f72  en used with wor
-0002c610: 6b66 6c6f 772e 0a0a 2020 2020 3a73 6565  kflow...    :see
-0002c620: 3a20 6874 7470 733a 2f2f 646f 6373 2e67  : https://docs.g
-0002c630: 6974 6c61 622e 636f 6d2f 6565 2f63 692f  itlab.com/ee/ci/
-0002c640: 7961 6d6c 2f23 776f 726b 666c 6f77 7275  yaml/#workflowru
-0002c650: 6c65 730a 2020 2020 3a73 7461 6269 6c69  les.    :stabili
-0002c660: 7479 3a20 6578 7065 7269 6d65 6e74 616c  ty: experimental
-0002c670: 0a20 2020 2027 2727 0a0a 2020 2020 414c  .    '''..    AL
-0002c680: 5741 5953 203d 2022 414c 5741 5953 220a  WAYS = "ALWAYS".
-0002c690: 2020 2020 2727 270a 2020 2020 3a73 7461      '''.    :sta
-0002c6a0: 6269 6c69 7479 3a20 6578 7065 7269 6d65  bility: experime
-0002c6b0: 6e74 616c 0a20 2020 2027 2727 0a20 2020  ntal.    '''.   
-0002c6c0: 204e 4556 4552 203d 2022 4e45 5645 5222   NEVER = "NEVER"
-0002c6d0: 0a20 2020 2027 2727 0a20 2020 203a 7374  .    '''.    :st
-0002c6e0: 6162 696c 6974 793a 2065 7870 6572 696d  ability: experim
-0002c6f0: 656e 7461 6c0a 2020 2020 2727 270a 0a0a  ental.    '''...
-0002c700: 5f5f 616c 6c5f 5f20 3d20 5b0a 2020 2020  __all__ = [.    
-0002c710: 2241 6374 696f 6e22 2c0a 2020 2020 2241  "Action",.    "A
-0002c720: 6c6c 6f77 4661 696c 7572 6522 2c0a 2020  llowFailure",.  
-0002c730: 2020 2241 7274 6966 6163 7473 222c 0a20    "Artifacts",. 
-0002c740: 2020 2022 4173 7365 7473 222c 0a20 2020     "Assets",.   
-0002c750: 2022 4361 6368 6522 2c0a 2020 2020 2243   "Cache",.    "C
-0002c760: 6163 6865 4b65 7946 696c 6573 222c 0a20  acheKeyFiles",. 
-0002c770: 2020 2022 4361 6368 6550 6f6c 6963 7922     "CachePolicy"
-0002c780: 2c0a 2020 2020 2243 6163 6865 5768 656e  ,.    "CacheWhen
-0002c790: 222c 0a20 2020 2022 4369 436f 6e66 6967  ",.    "CiConfig
-0002c7a0: 7572 6174 696f 6e22 2c0a 2020 2020 2243  uration",.    "C
-0002c7b0: 6943 6f6e 6669 6775 7261 7469 6f6e 4f70  iConfigurationOp
-0002c7c0: 7469 6f6e 7322 2c0a 2020 2020 2243 6f76  tions",.    "Cov
-0002c7d0: 6572 6167 6552 6570 6f72 7422 2c0a 2020  erageReport",.  
-0002c7e0: 2020 2244 6566 6175 6c74 222c 0a20 2020    "Default",.   
-0002c7f0: 2022 4465 6661 756c 7445 6c65 6d65 6e74   "DefaultElement
-0002c800: 222c 0a20 2020 2022 4465 706c 6f79 6d65  ",.    "Deployme
-0002c810: 6e74 5469 6572 222c 0a20 2020 2022 456e  ntTier",.    "En
-0002c820: 6769 6e65 222c 0a20 2020 2022 456e 7669  gine",.    "Envi
-0002c830: 726f 6e6d 656e 7422 2c0a 2020 2020 2246  ronment",.    "F
-0002c840: 696c 7465 7222 2c0a 2020 2020 2247 6974  ilter",.    "Git
-0002c850: 6c61 6243 6f6e 6669 6775 7261 7469 6f6e  labConfiguration
-0002c860: 222c 0a20 2020 2022 4944 546f 6b65 6e22  ",.    "IDToken"
-0002c870: 2c0a 2020 2020 2249 6d61 6765 222c 0a20  ,.    "Image",. 
-0002c880: 2020 2022 496e 636c 7564 6522 2c0a 2020     "Include",.  
-0002c890: 2020 2249 6e63 6c75 6465 5275 6c65 222c    "IncludeRule",
-0002c8a0: 0a20 2020 2022 496e 6865 7269 7422 2c0a  .    "Inherit",.
-0002c8b0: 2020 2020 224a 6f62 222c 0a20 2020 2022      "Job",.    "
-0002c8c0: 4a6f 6257 6865 6e22 2c0a 2020 2020 224b  JobWhen",.    "K
-0002c8d0: 7562 6572 6e65 7465 7343 6f6e 6669 6722  ubernetesConfig"
-0002c8e0: 2c0a 2020 2020 224b 7562 6572 6e65 7465  ,.    "Kubernete
-0002c8f0: 7345 6e75 6d22 2c0a 2020 2020 224c 696e  sEnum",.    "Lin
-0002c900: 6b22 2c0a 2020 2020 224c 696e 6b54 7970  k",.    "LinkTyp
-0002c910: 6522 2c0a 2020 2020 224e 6565 6422 2c0a  e",.    "Need",.
-0002c920: 2020 2020 224e 6573 7465 6443 6f6e 6669      "NestedConfi
-0002c930: 6775 7261 7469 6f6e 222c 0a20 2020 2022  guration",.    "
-0002c940: 5061 7261 6c6c 656c 222c 0a20 2020 2022  Parallel",.    "
-0002c950: 5075 6c6c 506f 6c69 6379 222c 0a20 2020  PullPolicy",.   
-0002c960: 2022 5265 6c65 6173 6522 2c0a 2020 2020   "Release",.    
-0002c970: 2252 6570 6f72 7473 222c 0a20 2020 2022  "Reports",.    "
-0002c980: 5265 7472 7922 2c0a 2020 2020 2253 6563  Retry",.    "Sec
-0002c990: 7265 7422 2c0a 2020 2020 2253 6572 7669  ret",.    "Servi
-0002c9a0: 6365 222c 0a20 2020 2022 5374 7261 7465  ce",.    "Strate
-0002c9b0: 6779 222c 0a20 2020 2022 5472 6967 6765  gy",.    "Trigge
-0002c9c0: 7222 2c0a 2020 2020 2254 7269 6767 6572  r",.    "Trigger
-0002c9d0: 496e 636c 7564 6522 2c0a 2020 2020 2256  Include",.    "V
-0002c9e0: 6172 6961 626c 6543 6f6e 6669 6722 2c0a  ariableConfig",.
-0002c9f0: 2020 2020 2256 6175 6c74 436f 6e66 6967      "VaultConfig
-0002ca00: 222c 0a20 2020 2022 576f 726b 666c 6f77  ",.    "Workflow
-0002ca10: 222c 0a20 2020 2022 576f 726b 666c 6f77  ",.    "Workflow
-0002ca20: 5275 6c65 222c 0a20 2020 2022 576f 726b  Rule",.    "Work
-0002ca30: 666c 6f77 5768 656e 222c 0a5d 0a0a 7075  flowWhen",.]..pu
-0002ca40: 626c 6963 6174 696f 6e2e 7075 626c 6973  blication.publis
-0002ca50: 6828 290a 0a64 6566 205f 7479 7065 6368  h()..def _typech
-0002ca60: 6563 6b69 6e67 7374 7562 5f5f 3333 6632  eckingstub__33f2
-0002ca70: 6333 3063 6465 3161 6562 6161 3833 6465  c30cde1aebaa83de
-0002ca80: 3039 3732 3433 3731 3761 6438 6464 3664  097243717ad8dd6d
-0002ca90: 3163 3236 3137 6234 3761 3433 3532 6362  1c2617b47a4352cb
-0002caa0: 6537 6533 6633 3531 6538 6232 280a 2020  e7e3f351e8b2(.  
-0002cab0: 2020 2a2c 0a20 2020 2065 7869 745f 636f    *,.    exit_co
-0002cac0: 6465 733a 2074 7970 696e 672e 556e 696f  des: typing.Unio
-0002cad0: 6e5b 6a73 6969 2e4e 756d 6265 722c 2074  n[jsii.Number, t
-0002cae0: 7970 696e 672e 5365 7175 656e 6365 5b6a  yping.Sequence[j
-0002caf0: 7369 692e 4e75 6d62 6572 5d5d 2c0a 2920  sii.Number]],.) 
-0002cb00: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
-0002cb10: 5479 7065 2063 6865 636b 696e 6720 7374  Type checking st
-0002cb20: 7562 7322 2222 0a20 2020 2070 6173 730a  ubs""".    pass.
-0002cb30: 0a64 6566 205f 7479 7065 6368 6563 6b69  .def _typechecki
-0002cb40: 6e67 7374 7562 5f5f 3136 6438 3463 3638  ngstub__16d84c68
-0002cb50: 3931 3066 6630 6432 6166 3138 6265 3533  910ff0d2af18be53
-0002cb60: 3439 3166 3563 6266 6430 6265 3838 3634  491f5cbfd0be8864
-0002cb70: 3861 6365 3264 6365 3130 6333 3563 3531  8ace2dce10c35c51
-0002cb80: 3064 3439 3861 6363 280a 2020 2020 2a2c  0d498acc(.    *,
-0002cb90: 0a20 2020 2065 7863 6c75 6465 3a20 7479  .    exclude: ty
-0002cba0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-0002cbb0: 7069 6e67 2e53 6571 7565 6e63 655b 6275  ping.Sequence[bu
-0002cbc0: 696c 7469 6e73 2e73 7472 5d5d 203d 204e  iltins.str]] = N
-0002cbd0: 6f6e 652c 0a20 2020 2065 7870 6972 655f  one,.    expire_
-0002cbe0: 696e 3a20 7479 7069 6e67 2e4f 7074 696f  in: typing.Optio
-0002cbf0: 6e61 6c5b 6275 696c 7469 6e73 2e73 7472  nal[builtins.str
-0002cc00: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6578  ] = None,.    ex
-0002cc10: 706f 7365 5f61 733a 2074 7970 696e 672e  pose_as: typing.
-0002cc20: 4f70 7469 6f6e 616c 5b62 7569 6c74 696e  Optional[builtin
-0002cc30: 732e 7374 725d 203d 204e 6f6e 652c 0a20  s.str] = None,. 
-0002cc40: 2020 206e 616d 653a 2074 7970 696e 672e     name: typing.
-0002cc50: 4f70 7469 6f6e 616c 5b62 7569 6c74 696e  Optional[builtin
-0002cc60: 732e 7374 725d 203d 204e 6f6e 652c 0a20  s.str] = None,. 
-0002cc70: 2020 2070 6174 6873 3a20 7479 7069 6e67     paths: typing
-0002cc80: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-0002cc90: 2e53 6571 7565 6e63 655b 6275 696c 7469  .Sequence[builti
-0002cca0: 6e73 2e73 7472 5d5d 203d 204e 6f6e 652c  ns.str]] = None,
-0002ccb0: 0a20 2020 2072 6570 6f72 7473 3a20 7479  .    reports: ty
-0002ccc0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-0002ccd0: 7069 6e67 2e55 6e69 6f6e 5b52 6570 6f72  ping.Union[Repor
-0002cce0: 7473 2c20 7479 7069 6e67 2e44 6963 745b  ts, typing.Dict[
-0002ccf0: 6275 696c 7469 6e73 2e73 7472 2c20 7479  builtins.str, ty
-0002cd00: 7069 6e67 2e41 6e79 5d5d 5d20 3d20 4e6f  ping.Any]]] = No
-0002cd10: 6e65 2c0a 2020 2020 756e 7472 6163 6b65  ne,.    untracke
-0002cd20: 643a 2074 7970 696e 672e 4f70 7469 6f6e  d: typing.Option
-0002cd30: 616c 5b62 7569 6c74 696e 732e 626f 6f6c  al[builtins.bool
-0002cd40: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 7768  ] = None,.    wh
-0002cd50: 656e 3a20 7479 7069 6e67 2e4f 7074 696f  en: typing.Optio
-0002cd60: 6e61 6c5b 4361 6368 6557 6865 6e5d 203d  nal[CacheWhen] =
-0002cd70: 204e 6f6e 652c 0a29 202d 3e20 4e6f 6e65   None,.) -> None
-0002cd80: 3a0a 2020 2020 2222 2254 7970 6520 6368  :.    """Type ch
-0002cd90: 6563 6b69 6e67 2073 7475 6273 2222 220a  ecking stubs""".
-0002cda0: 2020 2020 7061 7373 0a0a 6465 6620 5f74      pass..def _t
-0002cdb0: 7970 6563 6865 636b 696e 6773 7475 625f  ypecheckingstub_
-0002cdc0: 5f38 6164 3135 6338 3730 6665 3439 3238  _8ad15c870fe4928
-0002cdd0: 3862 6461 3161 3938 6531 6266 6339 6462  8bda1a98e1bfc9db
-0002cde0: 3566 3836 3232 3839 6465 3261 6435 6164  5f862289de2ad5ad
-0002cdf0: 3632 6534 6335 3963 6534 6161 6234 6337  62e4c59ce4aab4c7
-0002ce00: 3328 0a20 2020 202a 2c0a 2020 2020 6c69  3(.    *,.    li
-0002ce10: 6e6b 733a 2074 7970 696e 672e 5365 7175  nks: typing.Sequ
-0002ce20: 656e 6365 5b74 7970 696e 672e 556e 696f  ence[typing.Unio
-0002ce30: 6e5b 4c69 6e6b 2c20 7479 7069 6e67 2e44  n[Link, typing.D
-0002ce40: 6963 745b 6275 696c 7469 6e73 2e73 7472  ict[builtins.str
-0002ce50: 2c20 7479 7069 6e67 2e41 6e79 5d5d 5d2c  , typing.Any]]],
-0002ce60: 0a29 202d 3e20 4e6f 6e65 3a0a 2020 2020  .) -> None:.    
-0002ce70: 2222 2254 7970 6520 6368 6563 6b69 6e67  """Type checking
-0002ce80: 2073 7475 6273 2222 220a 2020 2020 7061   stubs""".    pa
-0002ce90: 7373 0a0a 6465 6620 5f74 7970 6563 6865  ss..def _typeche
-0002cea0: 636b 696e 6773 7475 625f 5f62 3766 3034  ckingstub__b7f04
-0002ceb0: 3936 3831 6466 3364 6363 6633 3536 3533  9681df3dccf35653
-0002cec0: 3834 3363 3534 3465 3036 3235 3832 3731  843c544e06258271
-0002ced0: 3532 3064 6231 3234 3933 6534 3861 6339  520db12493e48ac9
-0002cee0: 3336 6139 3665 6365 6461 6428 0a20 2020  36a96ecedad(.   
-0002cef0: 202a 2c0a 2020 2020 6661 6c6c 6261 636b   *,.    fallback
-0002cf00: 5f6b 6579 733a 2074 7970 696e 672e 4f70  _keys: typing.Op
-0002cf10: 7469 6f6e 616c 5b74 7970 696e 672e 5365  tional[typing.Se
-0002cf20: 7175 656e 6365 5b62 7569 6c74 696e 732e  quence[builtins.
-0002cf30: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
-0002cf40: 2020 6b65 793a 2074 7970 696e 672e 4f70    key: typing.Op
-0002cf50: 7469 6f6e 616c 5b74 7970 696e 672e 556e  tional[typing.Un
-0002cf60: 696f 6e5b 6275 696c 7469 6e73 2e73 7472  ion[builtins.str
-0002cf70: 2c20 7479 7069 6e67 2e55 6e69 6f6e 5b43  , typing.Union[C
-0002cf80: 6163 6865 4b65 7946 696c 6573 2c20 7479  acheKeyFiles, ty
-0002cf90: 7069 6e67 2e44 6963 745b 6275 696c 7469  ping.Dict[builti
-0002cfa0: 6e73 2e73 7472 2c20 7479 7069 6e67 2e41  ns.str, typing.A
-0002cfb0: 6e79 5d5d 5d5d 203d 204e 6f6e 652c 0a20  ny]]]] = None,. 
-0002cfc0: 2020 2070 6174 6873 3a20 7479 7069 6e67     paths: typing
-0002cfd0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-0002cfe0: 2e53 6571 7565 6e63 655b 6275 696c 7469  .Sequence[builti
-0002cff0: 6e73 2e73 7472 5d5d 203d 204e 6f6e 652c  ns.str]] = None,
-0002d000: 0a20 2020 2070 6f6c 6963 793a 2074 7970  .    policy: typ
-0002d010: 696e 672e 4f70 7469 6f6e 616c 5b43 6163  ing.Optional[Cac
-0002d020: 6865 506f 6c69 6379 5d20 3d20 4e6f 6e65  hePolicy] = None
-0002d030: 2c0a 2020 2020 756e 7472 6163 6b65 643a  ,.    untracked:
-0002d040: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0002d050: 5b62 7569 6c74 696e 732e 626f 6f6c 5d20  [builtins.bool] 
-0002d060: 3d20 4e6f 6e65 2c0a 2020 2020 7768 656e  = None,.    when
-0002d070: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0002d080: 6c5b 4361 6368 6557 6865 6e5d 203d 204e  l[CacheWhen] = N
-0002d090: 6f6e 652c 0a29 202d 3e20 4e6f 6e65 3a0a  one,.) -> None:.
-0002d0a0: 2020 2020 2222 2254 7970 6520 6368 6563      """Type chec
-0002d0b0: 6b69 6e67 2073 7475 6273 2222 220a 2020  king stubs""".  
-0002d0c0: 2020 7061 7373 0a0a 6465 6620 5f74 7970    pass..def _typ
-0002d0d0: 6563 6865 636b 696e 6773 7475 625f 5f65  echeckingstub__e
-0002d0e0: 3866 6137 3662 6331 6532 3235 3366 6439  8fa76bc1e2253fd9
-0002d0f0: 3564 6638 3166 6237 6239 3339 3832 3035  5df81fb7b9398205
-0002d100: 3162 3234 3063 6561 3933 6561 6435 3264  1b240cea93ead52d
-0002d110: 3964 3935 3533 3565 6562 3666 3736 3028  9d95535eeb6f760(
-0002d120: 0a20 2020 202a 2c0a 2020 2020 6669 6c65  .    *,.    file
-0002d130: 733a 2074 7970 696e 672e 5365 7175 656e  s: typing.Sequen
-0002d140: 6365 5b62 7569 6c74 696e 732e 7374 725d  ce[builtins.str]
-0002d150: 2c0a 2020 2020 7072 6566 6978 3a20 7479  ,.    prefix: ty
-0002d160: 7069 6e67 2e4f 7074 696f 6e61 6c5b 6275  ping.Optional[bu
-0002d170: 696c 7469 6e73 2e73 7472 5d20 3d20 4e6f  iltins.str] = No
-0002d180: 6e65 2c0a 2920 2d3e 204e 6f6e 653a 0a20  ne,.) -> None:. 
-0002d190: 2020 2022 2222 5479 7065 2063 6865 636b     """Type check
-0002d1a0: 696e 6720 7374 7562 7322 2222 0a20 2020  ing stubs""".   
-0002d1b0: 2070 6173 730a 0a64 6566 205f 7479 7065   pass..def _type
-0002d1c0: 6368 6563 6b69 6e67 7374 7562 5f5f 3233  checkingstub__23
-0002d1d0: 3163 3330 6263 3531 3366 3865 3039 6533  1c30bc513f8e09e3
-0002d1e0: 3435 6464 3633 3339 3265 3763 3530 6634  45dd63392e7c50f4
-0002d1f0: 3739 6466 3966 3438 3066 6333 3665 3033  79df9f480fc36e03
-0002d200: 6538 3866 6334 6135 6538 6364 3638 280a  e88fc4a5e8cd68(.
-0002d210: 2020 2020 7072 6f6a 6563 743a 205f 5072      project: _Pr
-0002d220: 6f6a 6563 745f 3537 6438 3932 3033 2c0a  oject_57d89203,.
-0002d230: 2020 2020 6e61 6d65 3a20 6275 696c 7469      name: builti
-0002d240: 6e73 2e73 7472 2c0a 2020 2020 2a2c 0a20  ns.str,.    *,. 
-0002d250: 2020 2064 6566 6175 6c74 3a20 7479 7069     default: typi
-0002d260: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-0002d270: 6e67 2e55 6e69 6f6e 5b44 6566 6175 6c74  ng.Union[Default
-0002d280: 2c20 7479 7069 6e67 2e44 6963 745b 6275  , typing.Dict[bu
-0002d290: 696c 7469 6e73 2e73 7472 2c20 7479 7069  iltins.str, typi
-0002d2a0: 6e67 2e41 6e79 5d5d 5d20 3d20 4e6f 6e65  ng.Any]]] = None
-0002d2b0: 2c0a 2020 2020 6a6f 6273 3a20 7479 7069  ,.    jobs: typi
-0002d2c0: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-0002d2d0: 6e67 2e4d 6170 7069 6e67 5b62 7569 6c74  ng.Mapping[built
-0002d2e0: 696e 732e 7374 722c 2074 7970 696e 672e  ins.str, typing.
-0002d2f0: 556e 696f 6e5b 4a6f 622c 2074 7970 696e  Union[Job, typin
-0002d300: 672e 4469 6374 5b62 7569 6c74 696e 732e  g.Dict[builtins.
-0002d310: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
-0002d320: 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ]]] = None,.    
-0002d330: 7061 6765 733a 2074 7970 696e 672e 4f70  pages: typing.Op
-0002d340: 7469 6f6e 616c 5b74 7970 696e 672e 556e  tional[typing.Un
-0002d350: 696f 6e5b 4a6f 622c 2074 7970 696e 672e  ion[Job, typing.
-0002d360: 4469 6374 5b62 7569 6c74 696e 732e 7374  Dict[builtins.st
-0002d370: 722c 2074 7970 696e 672e 416e 795d 5d5d  r, typing.Any]]]
-0002d380: 203d 204e 6f6e 652c 0a20 2020 2073 7461   = None,.    sta
-0002d390: 6765 733a 2074 7970 696e 672e 4f70 7469  ges: typing.Opti
-0002d3a0: 6f6e 616c 5b74 7970 696e 672e 5365 7175  onal[typing.Sequ
-0002d3b0: 656e 6365 5b62 7569 6c74 696e 732e 7374  ence[builtins.st
-0002d3c0: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
-0002d3d0: 7661 7269 6162 6c65 733a 2074 7970 696e  variables: typin
-0002d3e0: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-0002d3f0: 672e 4d61 7070 696e 675b 6275 696c 7469  g.Mapping[builti
-0002d400: 6e73 2e73 7472 2c20 7479 7069 6e67 2e41  ns.str, typing.A
-0002d410: 6e79 5d5d 203d 204e 6f6e 652c 0a20 2020  ny]] = None,.   
-0002d420: 2077 6f72 6b66 6c6f 773a 2074 7970 696e   workflow: typin
-0002d430: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-0002d440: 672e 556e 696f 6e5b 576f 726b 666c 6f77  g.Union[Workflow
-0002d450: 2c20 7479 7069 6e67 2e44 6963 745b 6275  , typing.Dict[bu
-0002d460: 696c 7469 6e73 2e73 7472 2c20 7479 7069  iltins.str, typi
-0002d470: 6e67 2e41 6e79 5d5d 5d20 3d20 4e6f 6e65  ng.Any]]] = None
-0002d480: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
-0002d490: 2022 2222 5479 7065 2063 6865 636b 696e   """Type checkin
-0002d4a0: 6720 7374 7562 7322 2222 0a20 2020 2070  g stubs""".    p
-0002d4b0: 6173 730a 0a64 6566 205f 7479 7065 6368  ass..def _typech
-0002d4c0: 6563 6b69 6e67 7374 7562 5f5f 6263 3864  eckingstub__bc8d
-0002d4d0: 6338 3366 3665 6432 6333 3932 3765 6163  c83f6ed2c3927eac
-0002d4e0: 3435 3839 3363 3836 3330 3530 3834 3362  45893c863050843b
-0002d4f0: 6465 6136 6139 3139 6463 6564 6130 6165  dea6a919dceda0ae
-0002d500: 6238 3131 6161 6236 6230 3361 280a 2020  b811aab6b03a(.  
-0002d510: 2020 6361 6368 6573 3a20 7479 7069 6e67    caches: typing
-0002d520: 2e53 6571 7565 6e63 655b 7479 7069 6e67  .Sequence[typing
-0002d530: 2e55 6e69 6f6e 5b43 6163 6865 2c20 7479  .Union[Cache, ty
-0002d540: 7069 6e67 2e44 6963 745b 6275 696c 7469  ping.Dict[builti
-0002d550: 6e73 2e73 7472 2c20 7479 7069 6e67 2e41  ns.str, typing.A
-0002d560: 6e79 5d5d 5d2c 0a29 202d 3e20 4e6f 6e65  ny]]],.) -> None
-0002d570: 3a0a 2020 2020 2222 2254 7970 6520 6368  :.    """Type ch
-0002d580: 6563 6b69 6e67 2073 7475 6273 2222 220a  ecking stubs""".
-0002d590: 2020 2020 7061 7373 0a0a 6465 6620 5f74      pass..def _t
-0002d5a0: 7970 6563 6865 636b 696e 6773 7475 625f  ypecheckingstub_
-0002d5b0: 5f61 3533 3262 3964 3362 6563 6264 6365  _a532b9d3becbdce
-0002d5c0: 6330 6132 3932 3533 3861 3036 3766 3364  c0a292538a067f3d
-0002d5d0: 6463 3661 3033 3761 6264 6635 3233 3530  dc6a037abdf52350
-0002d5e0: 3034 3835 6463 3533 3034 3138 3235 6330  0485dc53041825c0
-0002d5f0: 3328 0a20 2020 2076 6172 6961 626c 6573  3(.    variables
-0002d600: 3a20 7479 7069 6e67 2e4d 6170 7069 6e67  : typing.Mapping
-0002d610: 5b62 7569 6c74 696e 732e 7374 722c 2074  [builtins.str, t
-0002d620: 7970 696e 672e 416e 795d 2c0a 2920 2d3e  yping.Any],.) ->
-0002d630: 204e 6f6e 653a 0a20 2020 2022 2222 5479   None:.    """Ty
-0002d640: 7065 2063 6865 636b 696e 6720 7374 7562  pe checking stub
-0002d650: 7322 2222 0a20 2020 2070 6173 730a 0a64  s""".    pass..d
-0002d660: 6566 205f 7479 7065 6368 6563 6b69 6e67  ef _typechecking
-0002d670: 7374 7562 5f5f 3962 6361 3331 3839 6164  stub__9bca3189ad
-0002d680: 3533 6262 3461 3236 3539 6133 6334 6265  53bb4a2659a3c4be
-0002d690: 3763 3233 3337 3838 6466 6430 6436 6430  7c233788dfd0d6d0
-0002d6a0: 6533 3232 3535 6535 3264 3665 3664 3436  e32255e52d6e6d46
-0002d6b0: 3236 3165 6264 280a 2020 2020 2a69 6e63  261ebd(.    *inc
-0002d6c0: 6c75 6465 733a 2049 6e63 6c75 6465 2c0a  ludes: Include,.
-0002d6d0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
-0002d6e0: 2222 5479 7065 2063 6865 636b 696e 6720  ""Type checking 
-0002d6f0: 7374 7562 7322 2222 0a20 2020 2070 6173  stubs""".    pas
-0002d700: 730a 0a64 6566 205f 7479 7065 6368 6563  s..def _typechec
-0002d710: 6b69 6e67 7374 7562 5f5f 6634 3236 6464  kingstub__f426dd
-0002d720: 6330 6331 3235 6161 6265 3734 6130 3865  c0c125aabe74a08e
-0002d730: 6363 3461 6430 3038 6332 6432 6235 6234  cc4ad008c2d2b5b4
-0002d740: 3465 6639 3234 3066 3061 3065 3939 6330  4ef9240f0a0e99c0
-0002d750: 3461 3936 3830 6165 3138 280a 2020 2020  4a9680ae18(.    
-0002d760: 6a6f 6273 3a20 7479 7069 6e67 2e4d 6170  jobs: typing.Map
-0002d770: 7069 6e67 5b62 7569 6c74 696e 732e 7374  ping[builtins.st
-0002d780: 722c 2074 7970 696e 672e 556e 696f 6e5b  r, typing.Union[
-0002d790: 4a6f 622c 2074 7970 696e 672e 4469 6374  Job, typing.Dict
-0002d7a0: 5b62 7569 6c74 696e 732e 7374 722c 2074  [builtins.str, t
-0002d7b0: 7970 696e 672e 416e 795d 5d5d 2c0a 2920  yping.Any]]],.) 
-0002d7c0: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
-0002d7d0: 5479 7065 2063 6865 636b 696e 6720 7374  Type checking st
-0002d7e0: 7562 7322 2222 0a20 2020 2070 6173 730a  ubs""".    pass.
-0002d7f0: 0a64 6566 205f 7479 7065 6368 6563 6b69  .def _typechecki
-0002d800: 6e67 7374 7562 5f5f 6565 3838 3661 6236  ngstub__ee886ab6
-0002d810: 3633 3538 6363 3235 6637 3565 6166 6635  6358cc25f75eaff5
-0002d820: 6463 6265 6261 3265 3033 6435 6637 3264  dcbeba2e03d5f72d
-0002d830: 6238 6437 6432 3939 3336 3061 6638 3134  b8d7d299360af814
-0002d840: 3533 3432 3866 3962 280a 2020 2020 2a73  53428f9b(.    *s
-0002d850: 6572 7669 6365 733a 2053 6572 7669 6365  ervices: Service
-0002d860: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
-0002d870: 2022 2222 5479 7065 2063 6865 636b 696e   """Type checkin
-0002d880: 6720 7374 7562 7322 2222 0a20 2020 2070  g stubs""".    p
-0002d890: 6173 730a 0a64 6566 205f 7479 7065 6368  ass..def _typech
-0002d8a0: 6563 6b69 6e67 7374 7562 5f5f 6333 3732  eckingstub__c372
-0002d8b0: 3536 3731 3362 6238 6433 3631 3936 3666  56713bb8d361966f
-0002d8c0: 3062 3339 6634 6462 6138 6161 6334 3436  0b39f4dba8aac446
-0002d8d0: 6631 6565 6137 6461 3237 6661 6264 3865  f1eea7da27fabd8e
-0002d8e0: 3965 6136 3833 3339 3333 6336 280a 2020  9ea6833933c6(.  
-0002d8f0: 2020 2a73 7461 6765 733a 2062 7569 6c74    *stages: built
-0002d900: 696e 732e 7374 722c 0a29 202d 3e20 4e6f  ins.str,.) -> No
-0002d910: 6e65 3a0a 2020 2020 2222 2254 7970 6520  ne:.    """Type 
-0002d920: 6368 6563 6b69 6e67 2073 7475 6273 2222  checking stubs""
-0002d930: 220a 2020 2020 7061 7373 0a0a 6465 6620  ".    pass..def 
-0002d940: 5f74 7970 6563 6865 636b 696e 6773 7475  _typecheckingstu
-0002d950: 625f 5f63 6164 3632 3034 6439 3434 3231  b__cad6204d94421
-0002d960: 6132 3439 3365 3434 6336 3133 3165 3434  a2493e44c6131e44
-0002d970: 6539 6163 3231 3735 3534 3662 6537 3264  e9ac2175546be72d
-0002d980: 3065 3635 3564 6637 3632 3532 3036 3733  0e655df762520673
-0002d990: 6339 6528 0a20 2020 202a 2c0a 2020 2020  c9e(.    *,.    
-0002d9a0: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
-0002d9b0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-0002d9c0: 556e 696f 6e5b 4465 6661 756c 742c 2074  Union[Default, t
-0002d9d0: 7970 696e 672e 4469 6374 5b62 7569 6c74  yping.Dict[built
-0002d9e0: 696e 732e 7374 722c 2074 7970 696e 672e  ins.str, typing.
-0002d9f0: 416e 795d 5d5d 203d 204e 6f6e 652c 0a20  Any]]] = None,. 
-0002da00: 2020 206a 6f62 733a 2074 7970 696e 672e     jobs: typing.
-0002da10: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-0002da20: 4d61 7070 696e 675b 6275 696c 7469 6e73  Mapping[builtins
-0002da30: 2e73 7472 2c20 7479 7069 6e67 2e55 6e69  .str, typing.Uni
-0002da40: 6f6e 5b4a 6f62 2c20 7479 7069 6e67 2e44  on[Job, typing.D
-0002da50: 6963 745b 6275 696c 7469 6e73 2e73 7472  ict[builtins.str
-0002da60: 2c20 7479 7069 6e67 2e41 6e79 5d5d 5d5d  , typing.Any]]]]
-0002da70: 203d 204e 6f6e 652c 0a20 2020 2070 6167   = None,.    pag
-0002da80: 6573 3a20 7479 7069 6e67 2e4f 7074 696f  es: typing.Optio
-0002da90: 6e61 6c5b 7479 7069 6e67 2e55 6e69 6f6e  nal[typing.Union
-0002daa0: 5b4a 6f62 2c20 7479 7069 6e67 2e44 6963  [Job, typing.Dic
-0002dab0: 745b 6275 696c 7469 6e73 2e73 7472 2c20  t[builtins.str, 
-0002dac0: 7479 7069 6e67 2e41 6e79 5d5d 5d20 3d20  typing.Any]]] = 
-0002dad0: 4e6f 6e65 2c0a 2020 2020 7374 6167 6573  None,.    stages
-0002dae0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0002daf0: 6c5b 7479 7069 6e67 2e53 6571 7565 6e63  l[typing.Sequenc
-0002db00: 655b 6275 696c 7469 6e73 2e73 7472 5d5d  e[builtins.str]]
-0002db10: 203d 204e 6f6e 652c 0a20 2020 2076 6172   = None,.    var
-0002db20: 6961 626c 6573 3a20 7479 7069 6e67 2e4f  iables: typing.O
-0002db30: 7074 696f 6e61 6c5b 7479 7069 6e67 2e4d  ptional[typing.M
-0002db40: 6170 7069 6e67 5b62 7569 6c74 696e 732e  apping[builtins.
-0002db50: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
-0002db60: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 776f  ] = None,.    wo
-0002db70: 726b 666c 6f77 3a20 7479 7069 6e67 2e4f  rkflow: typing.O
-0002db80: 7074 696f 6e61 6c5b 7479 7069 6e67 2e55  ptional[typing.U
-0002db90: 6e69 6f6e 5b57 6f72 6b66 6c6f 772c 2074  nion[Workflow, t
-0002dba0: 7970 696e 672e 4469 6374 5b62 7569 6c74  yping.Dict[built
-0002dbb0: 696e 732e 7374 722c 2074 7970 696e 672e  ins.str, typing.
-0002dbc0: 416e 795d 5d5d 203d 204e 6f6e 652c 0a29  Any]]] = None,.)
-0002dbd0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
-0002dbe0: 2254 7970 6520 6368 6563 6b69 6e67 2073  "Type checking s
-0002dbf0: 7475 6273 2222 220a 2020 2020 7061 7373  tubs""".    pass
-0002dc00: 0a0a 6465 6620 5f74 7970 6563 6865 636b  ..def _typecheck
-0002dc10: 696e 6773 7475 625f 5f63 3466 6238 3436  ingstub__c4fb846
-0002dc20: 6461 6163 3030 3063 6463 6236 3337 3461  daac000cdcb6374a
-0002dc30: 6364 3730 6562 6337 3332 3366 3836 3736  cd70ebc7323f8676
-0002dc40: 3161 3331 6332 6562 6232 6566 3064 3162  1a31c2ebb2ef0d1b
-0002dc50: 3439 6133 6630 3635 3228 0a20 2020 202a  49a3f0652(.    *
-0002dc60: 2c0a 2020 2020 636f 7665 7261 6765 5f66  ,.    coverage_f
-0002dc70: 6f72 6d61 743a 2062 7569 6c74 696e 732e  ormat: builtins.
-0002dc80: 7374 722c 0a20 2020 2070 6174 683a 2062  str,.    path: b
-0002dc90: 7569 6c74 696e 732e 7374 722c 0a29 202d  uiltins.str,.) -
-0002dca0: 3e20 4e6f 6e65 3a0a 2020 2020 2222 2254  > None:.    """T
-0002dcb0: 7970 6520 6368 6563 6b69 6e67 2073 7475  ype checking stu
-0002dcc0: 6273 2222 220a 2020 2020 7061 7373 0a0a  bs""".    pass..
-0002dcd0: 6465 6620 5f74 7970 6563 6865 636b 696e  def _typecheckin
-0002dce0: 6773 7475 625f 5f63 3865 3731 6430 3165  gstub__c8e71d01e
-0002dcf0: 6461 3930 3239 3764 6236 6166 3637 3566  da90297db6af675f
-0002dd00: 3531 3033 3334 3134 3534 3632 3132 6230  51033414546212b0
-0002dd10: 3664 3439 6330 3063 3231 3864 6565 3230  6d49c00c218dee20
-0002dd20: 3731 6431 6564 3128 0a20 2020 202a 2c0a  71d1ed1(.    *,.
-0002dd30: 2020 2020 6166 7465 725f 7363 7269 7074      after_script
-0002dd40: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0002dd50: 6c5b 7479 7069 6e67 2e53 6571 7565 6e63  l[typing.Sequenc
-0002dd60: 655b 6275 696c 7469 6e73 2e73 7472 5d5d  e[builtins.str]]
-0002dd70: 203d 204e 6f6e 652c 0a20 2020 2061 7274   = None,.    art
-0002dd80: 6966 6163 7473 3a20 7479 7069 6e67 2e4f  ifacts: typing.O
-0002dd90: 7074 696f 6e61 6c5b 7479 7069 6e67 2e55  ptional[typing.U
-0002dda0: 6e69 6f6e 5b41 7274 6966 6163 7473 2c20  nion[Artifacts, 
-0002ddb0: 7479 7069 6e67 2e44 6963 745b 6275 696c  typing.Dict[buil
-0002ddc0: 7469 6e73 2e73 7472 2c20 7479 7069 6e67  tins.str, typing
-0002ddd0: 2e41 6e79 5d5d 5d20 3d20 4e6f 6e65 2c0a  .Any]]] = None,.
-0002dde0: 2020 2020 6265 666f 7265 5f73 6372 6970      before_scrip
-0002ddf0: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
-0002de00: 616c 5b74 7970 696e 672e 5365 7175 656e  al[typing.Sequen
-0002de10: 6365 5b62 7569 6c74 696e 732e 7374 725d  ce[builtins.str]
-0002de20: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6361  ] = None,.    ca
-0002de30: 6368 653a 2074 7970 696e 672e 4f70 7469  che: typing.Opti
-0002de40: 6f6e 616c 5b74 7970 696e 672e 5365 7175  onal[typing.Sequ
-0002de50: 656e 6365 5b74 7970 696e 672e 556e 696f  ence[typing.Unio
-0002de60: 6e5b 4361 6368 652c 2074 7970 696e 672e  n[Cache, typing.
-0002de70: 4469 6374 5b62 7569 6c74 696e 732e 7374  Dict[builtins.st
-0002de80: 722c 2074 7970 696e 672e 416e 795d 5d5d  r, typing.Any]]]
-0002de90: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 696d  ] = None,.    im
-0002dea0: 6167 653a 2074 7970 696e 672e 4f70 7469  age: typing.Opti
-0002deb0: 6f6e 616c 5b74 7970 696e 672e 556e 696f  onal[typing.Unio
-0002dec0: 6e5b 496d 6167 652c 2074 7970 696e 672e  n[Image, typing.
-0002ded0: 4469 6374 5b62 7569 6c74 696e 732e 7374  Dict[builtins.st
-0002dee0: 722c 2074 7970 696e 672e 416e 795d 5d5d  r, typing.Any]]]
-0002def0: 203d 204e 6f6e 652c 0a20 2020 2069 6e74   = None,.    int
-0002df00: 6572 7275 7074 6962 6c65 3a20 7479 7069  erruptible: typi
-0002df10: 6e67 2e4f 7074 696f 6e61 6c5b 6275 696c  ng.Optional[buil
-0002df20: 7469 6e73 2e62 6f6f 6c5d 203d 204e 6f6e  tins.bool] = Non
-0002df30: 652c 0a20 2020 2072 6574 7279 3a20 7479  e,.    retry: ty
-0002df40: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-0002df50: 7069 6e67 2e55 6e69 6f6e 5b52 6574 7279  ping.Union[Retry
-0002df60: 2c20 7479 7069 6e67 2e44 6963 745b 6275  , typing.Dict[bu
-0002df70: 696c 7469 6e73 2e73 7472 2c20 7479 7069  iltins.str, typi
-0002df80: 6e67 2e41 6e79 5d5d 5d20 3d20 4e6f 6e65  ng.Any]]] = None
-0002df90: 2c0a 2020 2020 7365 7276 6963 6573 3a20  ,.    services: 
-0002dfa0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0002dfb0: 7479 7069 6e67 2e53 6571 7565 6e63 655b  typing.Sequence[
-0002dfc0: 7479 7069 6e67 2e55 6e69 6f6e 5b53 6572  typing.Union[Ser
-0002dfd0: 7669 6365 2c20 7479 7069 6e67 2e44 6963  vice, typing.Dic
-0002dfe0: 745b 6275 696c 7469 6e73 2e73 7472 2c20  t[builtins.str, 
-0002dff0: 7479 7069 6e67 2e41 6e79 5d5d 5d5d 203d  typing.Any]]]] =
-0002e000: 204e 6f6e 652c 0a20 2020 2074 6167 733a   None,.    tags:
-0002e010: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0002e020: 5b74 7970 696e 672e 5365 7175 656e 6365  [typing.Sequence
-0002e030: 5b62 7569 6c74 696e 732e 7374 725d 5d20  [builtins.str]] 
-0002e040: 3d20 4e6f 6e65 2c0a 2020 2020 7469 6d65  = None,.    time
-0002e050: 6f75 743a 2074 7970 696e 672e 4f70 7469  out: typing.Opti
-0002e060: 6f6e 616c 5b62 7569 6c74 696e 732e 7374  onal[builtins.st
-0002e070: 725d 203d 204e 6f6e 652c 0a29 202d 3e20  r] = None,.) -> 
-0002e080: 4e6f 6e65 3a0a 2020 2020 2222 2254 7970  None:.    """Typ
-0002e090: 6520 6368 6563 6b69 6e67 2073 7475 6273  e checking stubs
-0002e0a0: 2222 220a 2020 2020 7061 7373 0a0a 6465  """.    pass..de
-0002e0b0: 6620 5f74 7970 6563 6865 636b 696e 6773  f _typecheckings
-0002e0c0: 7475 625f 5f34 3537 3464 6562 3530 6366  tub__4574deb50cf
-0002e0d0: 3930 3139 6531 3133 6336 3764 3731 3464  9019e113c67d714d
-0002e0e0: 6132 3936 3835 3134 3333 3234 6663 3465  a29685143324fc4e
-0002e0f0: 3164 6630 3663 3565 6130 3861 3837 3464  1df06c5ea08a874d
-0002e100: 6538 3232 3328 0a20 2020 202a 2c0a 2020  e8223(.    *,.  
-0002e110: 2020 6e61 6d65 3a20 6275 696c 7469 6e73    name: builtins
-0002e120: 2e73 7472 2c0a 2020 2020 7061 7468 3a20  .str,.    path: 
-0002e130: 6275 696c 7469 6e73 2e73 7472 2c0a 2920  builtins.str,.) 
-0002e140: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
-0002e150: 5479 7065 2063 6865 636b 696e 6720 7374  Type checking st
-0002e160: 7562 7322 2222 0a20 2020 2070 6173 730a  ubs""".    pass.
-0002e170: 0a64 6566 205f 7479 7065 6368 6563 6b69  .def _typechecki
-0002e180: 6e67 7374 7562 5f5f 3764 6163 6630 3636  ngstub__7dacf066
-0002e190: 3532 3065 6465 6263 6166 3139 3134 6366  520edebcaf1914cf
-0002e1a0: 3862 3437 6135 3339 6433 3262 3630 3163  8b47a539d32b601c
-0002e1b0: 3732 3863 3734 3561 3938 3231 6461 3138  728c745a9821da18
-0002e1c0: 6663 3631 6333 3131 280a 2020 2020 2a2c  fc61c311(.    *,
-0002e1d0: 0a20 2020 206e 616d 653a 2062 7569 6c74  .    name: built
-0002e1e0: 696e 732e 7374 722c 0a20 2020 2061 6374  ins.str,.    act
-0002e1f0: 696f 6e3a 2074 7970 696e 672e 4f70 7469  ion: typing.Opti
-0002e200: 6f6e 616c 5b41 6374 696f 6e5d 203d 204e  onal[Action] = N
-0002e210: 6f6e 652c 0a20 2020 2061 7574 6f5f 7374  one,.    auto_st
-0002e220: 6f70 5f69 6e3a 2074 7970 696e 672e 4f70  op_in: typing.Op
-0002e230: 7469 6f6e 616c 5b62 7569 6c74 696e 732e  tional[builtins.
-0002e240: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0002e250: 2064 6570 6c6f 796d 656e 745f 7469 6572   deployment_tier
-0002e260: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0002e270: 6c5b 4465 706c 6f79 6d65 6e74 5469 6572  l[DeploymentTier
-0002e280: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6b75  ] = None,.    ku
-0002e290: 6265 726e 6574 6573 3a20 7479 7069 6e67  bernetes: typing
-0002e2a0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-0002e2b0: 2e55 6e69 6f6e 5b4b 7562 6572 6e65 7465  .Union[Kubernete
-0002e2c0: 7343 6f6e 6669 672c 2074 7970 696e 672e  sConfig, typing.
-0002e2d0: 4469 6374 5b62 7569 6c74 696e 732e 7374  Dict[builtins.st
-0002e2e0: 722c 2074 7970 696e 672e 416e 795d 5d5d  r, typing.Any]]]
-0002e2f0: 203d 204e 6f6e 652c 0a20 2020 206f 6e5f   = None,.    on_
-0002e300: 7374 6f70 3a20 7479 7069 6e67 2e4f 7074  stop: typing.Opt
-0002e310: 696f 6e61 6c5b 6275 696c 7469 6e73 2e73  ional[builtins.s
-0002e320: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0002e330: 7572 6c3a 2074 7970 696e 672e 4f70 7469  url: typing.Opti
-0002e340: 6f6e 616c 5b62 7569 6c74 696e 732e 7374  onal[builtins.st
-0002e350: 725d 203d 204e 6f6e 652c 0a29 202d 3e20  r] = None,.) -> 
-0002e360: 4e6f 6e65 3a0a 2020 2020 2222 2254 7970  None:.    """Typ
-0002e370: 6520 6368 6563 6b69 6e67 2073 7475 6273  e checking stubs
-0002e380: 2222 220a 2020 2020 7061 7373 0a0a 6465  """.    pass..de
-0002e390: 6620 5f74 7970 6563 6865 636b 696e 6773  f _typecheckings
-0002e3a0: 7475 625f 5f64 6238 3935 6536 3732 3838  tub__db895e67288
-0002e3b0: 3736 6465 3562 6537 3536 3235 6466 3862  76de5be75625df8b
-0002e3c0: 6539 3461 3863 3836 3834 3633 3237 6232  e94a8c86846327b2
-0002e3d0: 3434 3366 6631 6664 3763 3863 3039 6463  443ff1fd7c8c09dc
-0002e3e0: 3464 3666 3228 0a20 2020 202a 2c0a 2020  4d6f2(.    *,.  
-0002e3f0: 2020 6368 616e 6765 733a 2074 7970 696e    changes: typin
-0002e400: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-0002e410: 672e 5365 7175 656e 6365 5b62 7569 6c74  g.Sequence[built
-0002e420: 696e 732e 7374 725d 5d20 3d20 4e6f 6e65  ins.str]] = None
-0002e430: 2c0a 2020 2020 6b75 6265 726e 6574 6573  ,.    kubernetes
-0002e440: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0002e450: 6c5b 4b75 6265 726e 6574 6573 456e 756d  l[KubernetesEnum
-0002e460: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 7265  ] = None,.    re
-0002e470: 6673 3a20 7479 7069 6e67 2e4f 7074 696f  fs: typing.Optio
-0002e480: 6e61 6c5b 7479 7069 6e67 2e53 6571 7565  nal[typing.Seque
-0002e490: 6e63 655b 6275 696c 7469 6e73 2e73 7472  nce[builtins.str
-0002e4a0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2076  ]] = None,.    v
-0002e4b0: 6172 6961 626c 6573 3a20 7479 7069 6e67  ariables: typing
-0002e4c0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-0002e4d0: 2e53 6571 7565 6e63 655b 6275 696c 7469  .Sequence[builti
-0002e4e0: 6e73 2e73 7472 5d5d 203d 204e 6f6e 652c  ns.str]] = None,
-0002e4f0: 0a29 202d 3e20 4e6f 6e65 3a0a 2020 2020  .) -> None:.    
-0002e500: 2222 2254 7970 6520 6368 6563 6b69 6e67  """Type checking
-0002e510: 2073 7475 6273 2222 220a 2020 2020 7061   stubs""".    pa
-0002e520: 7373 0a0a 6465 6620 5f74 7970 6563 6865  ss..def _typeche
-0002e530: 636b 696e 6773 7475 625f 5f39 6237 6332  ckingstub__9b7c2
-0002e540: 3262 3735 3238 3337 6435 6334 3139 3837  2b752837d5c41987
-0002e550: 3736 3131 6333 3636 3463 6161 3838 3635  7611c3664caa8865
-0002e560: 3339 6162 3532 3039 3436 3562 6266 6532  39ab5209465bbfe2
-0002e570: 3733 3732 6235 3165 3731 3428 0a20 2020  7372b51e714(.   
-0002e580: 2070 726f 6a65 6374 3a20 5f50 726f 6a65   project: _Proje
-0002e590: 6374 5f35 3764 3839 3230 332c 0a20 2020  ct_57d89203,.   
-0002e5a0: 202a 2c0a 2020 2020 6465 6661 756c 743a   *,.    default:
-0002e5b0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0002e5c0: 5b74 7970 696e 672e 556e 696f 6e5b 4465  [typing.Union[De
-0002e5d0: 6661 756c 742c 2074 7970 696e 672e 4469  fault, typing.Di
-0002e5e0: 6374 5b62 7569 6c74 696e 732e 7374 722c  ct[builtins.str,
-0002e5f0: 2074 7970 696e 672e 416e 795d 5d5d 203d   typing.Any]]] =
-0002e600: 204e 6f6e 652c 0a20 2020 206a 6f62 733a   None,.    jobs:
-0002e610: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0002e620: 5b74 7970 696e 672e 4d61 7070 696e 675b  [typing.Mapping[
-0002e630: 6275 696c 7469 6e73 2e73 7472 2c20 7479  builtins.str, ty
-0002e640: 7069 6e67 2e55 6e69 6f6e 5b4a 6f62 2c20  ping.Union[Job, 
-0002e650: 7479 7069 6e67 2e44 6963 745b 6275 696c  typing.Dict[buil
-0002e660: 7469 6e73 2e73 7472 2c20 7479 7069 6e67  tins.str, typing
-0002e670: 2e41 6e79 5d5d 5d5d 203d 204e 6f6e 652c  .Any]]]] = None,
-0002e680: 0a20 2020 2070 6167 6573 3a20 7479 7069  .    pages: typi
-0002e690: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-0002e6a0: 6e67 2e55 6e69 6f6e 5b4a 6f62 2c20 7479  ng.Union[Job, ty
-0002e6b0: 7069 6e67 2e44 6963 745b 6275 696c 7469  ping.Dict[builti
-0002e6c0: 6e73 2e73 7472 2c20 7479 7069 6e67 2e41  ns.str, typing.A
-0002e6d0: 6e79 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020  ny]]] = None,.  
-0002e6e0: 2020 7374 6167 6573 3a20 7479 7069 6e67    stages: typing
-0002e6f0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-0002e700: 2e53 6571 7565 6e63 655b 6275 696c 7469  .Sequence[builti
-0002e710: 6e73 2e73 7472 5d5d 203d 204e 6f6e 652c  ns.str]] = None,
-0002e720: 0a20 2020 2076 6172 6961 626c 6573 3a20  .    variables: 
-0002e730: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0002e740: 7479 7069 6e67 2e4d 6170 7069 6e67 5b62  typing.Mapping[b
-0002e750: 7569 6c74 696e 732e 7374 722c 2074 7970  uiltins.str, typ
-0002e760: 696e 672e 416e 795d 5d20 3d20 4e6f 6e65  ing.Any]] = None
-0002e770: 2c0a 2020 2020 776f 726b 666c 6f77 3a20  ,.    workflow: 
-0002e780: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0002e790: 7479 7069 6e67 2e55 6e69 6f6e 5b57 6f72  typing.Union[Wor
-0002e7a0: 6b66 6c6f 772c 2074 7970 696e 672e 4469  kflow, typing.Di
-0002e7b0: 6374 5b62 7569 6c74 696e 732e 7374 722c  ct[builtins.str,
-0002e7c0: 2074 7970 696e 672e 416e 795d 5d5d 203d   typing.Any]]] =
-0002e7d0: 204e 6f6e 652c 0a29 202d 3e20 4e6f 6e65   None,.) -> None
-0002e7e0: 3a0a 2020 2020 2222 2254 7970 6520 6368  :.    """Type ch
-0002e7f0: 6563 6b69 6e67 2073 7475 6273 2222 220a  ecking stubs""".
-0002e800: 2020 2020 7061 7373 0a0a 6465 6620 5f74      pass..def _t
-0002e810: 7970 6563 6865 636b 696e 6773 7475 625f  ypecheckingstub_
-0002e820: 5f61 3065 3839 6330 3034 6461 6535 6463  _a0e89c004dae5dc
-0002e830: 3861 3636 3437 3766 3965 3035 6434 3230  8a66477f9e05d420
-0002e840: 3265 3264 6532 3562 3339 3761 6435 3834  2e2de25b397ad584
-0002e850: 3339 3135 3864 3464 3065 3331 3166 6134  39158d4d0e311fa4
-0002e860: 3628 0a20 2020 2063 6f6e 6669 673a 2074  6(.    config: t
-0002e870: 7970 696e 672e 4d61 7070 696e 675b 6275  yping.Mapping[bu
-0002e880: 696c 7469 6e73 2e73 7472 2c20 7479 7069  iltins.str, typi
-0002e890: 6e67 2e55 6e69 6f6e 5b43 6943 6f6e 6669  ng.Union[CiConfi
-0002e8a0: 6775 7261 7469 6f6e 4f70 7469 6f6e 732c  gurationOptions,
-0002e8b0: 2074 7970 696e 672e 4469 6374 5b62 7569   typing.Dict[bui
-0002e8c0: 6c74 696e 732e 7374 722c 2074 7970 696e  ltins.str, typin
-0002e8d0: 672e 416e 795d 5d5d 2c0a 2920 2d3e 204e  g.Any]]],.) -> N
-0002e8e0: 6f6e 653a 0a20 2020 2022 2222 5479 7065  one:.    """Type
-0002e8f0: 2063 6865 636b 696e 6720 7374 7562 7322   checking stubs"
-0002e900: 2222 0a20 2020 2070 6173 730a 0a64 6566  "".    pass..def
-0002e910: 205f 7479 7065 6368 6563 6b69 6e67 7374   _typecheckingst
-0002e920: 7562 5f5f 6139 6536 6262 6437 6331 6433  ub__a9e6bbd7c1d3
-0002e930: 6531 3666 6661 3832 3336 3763 6464 3563  e16ffa82367cdd5c
-0002e940: 6131 3663 6530 3661 3432 3732 3666 3431  a16ce06a42726f41
-0002e950: 3933 3633 3937 3930 6133 3962 6232 6561  93639790a39bb2ea
-0002e960: 6465 6639 280a 2020 2020 7661 6c75 653a  def9(.    value:
-0002e970: 2074 7970 696e 672e 556e 696f 6e5b 6275   typing.Union[bu
-0002e980: 696c 7469 6e73 2e73 7472 2c20 7479 7069  iltins.str, typi
-0002e990: 6e67 2e4c 6973 745b 6275 696c 7469 6e73  ng.List[builtins
-0002e9a0: 2e73 7472 5d5d 2c0a 2920 2d3e 204e 6f6e  .str]],.) -> Non
-0002e9b0: 653a 0a20 2020 2022 2222 5479 7065 2063  e:.    """Type c
-0002e9c0: 6865 636b 696e 6720 7374 7562 7322 2222  hecking stubs"""
-0002e9d0: 0a20 2020 2070 6173 730a 0a64 6566 205f  .    pass..def _
-0002e9e0: 7479 7065 6368 6563 6b69 6e67 7374 7562  typecheckingstub
-0002e9f0: 5f5f 3164 6230 3433 6465 3162 6664 3937  __1db043de1bfd97
-0002ea00: 3163 6633 3632 6131 6435 3031 3564 3339  1cf362a1d5015d39
-0002ea10: 6663 6665 6339 6365 3132 6138 3536 3465  fcfec9ce12a8564e
-0002ea20: 3132 6233 6463 3833 6332 3736 3666 3565  12b3dc83c2766f5e
-0002ea30: 3766 280a 2020 2020 2a2c 0a20 2020 206e  7f(.    *,.    n
-0002ea40: 616d 653a 2062 7569 6c74 696e 732e 7374  ame: builtins.st
-0002ea50: 722c 0a20 2020 2065 6e74 7279 706f 696e  r,.    entrypoin
-0002ea60: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
-0002ea70: 616c 5b74 7970 696e 672e 5365 7175 656e  al[typing.Sequen
-0002ea80: 6365 5b74 7970 696e 672e 416e 795d 5d20  ce[typing.Any]] 
-0002ea90: 3d20 4e6f 6e65 2c0a 2920 2d3e 204e 6f6e  = None,.) -> Non
-0002eaa0: 653a 0a20 2020 2022 2222 5479 7065 2063  e:.    """Type c
-0002eab0: 6865 636b 696e 6720 7374 7562 7322 2222  hecking stubs"""
-0002eac0: 0a20 2020 2070 6173 730a 0a64 6566 205f  .    pass..def _
-0002ead0: 7479 7065 6368 6563 6b69 6e67 7374 7562  typecheckingstub
-0002eae0: 5f5f 6636 6234 6233 3366 3832 3464 6564  __f6b4b33f824ded
-0002eaf0: 6533 6335 3166 3834 3931 6632 3363 3162  e3c51f8491f23c1b
-0002eb00: 3234 6161 3939 6465 3839 3032 6162 3262  24aa99de8902ab2b
-0002eb10: 3061 6462 3739 3266 6263 3133 6464 6638  0adb792fbc13ddf8
-0002eb20: 6665 280a 2020 2020 2a2c 0a20 2020 2066  fe(.    *,.    f
-0002eb30: 696c 653a 2074 7970 696e 672e 4f70 7469  ile: typing.Opti
-0002eb40: 6f6e 616c 5b74 7970 696e 672e 5365 7175  onal[typing.Sequ
-0002eb50: 656e 6365 5b62 7569 6c74 696e 732e 7374  ence[builtins.st
-0002eb60: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
-0002eb70: 6c6f 6361 6c3a 2074 7970 696e 672e 4f70  local: typing.Op
-0002eb80: 7469 6f6e 616c 5b62 7569 6c74 696e 732e  tional[builtins.
-0002eb90: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0002eba0: 2070 726f 6a65 6374 3a20 7479 7069 6e67   project: typing
-0002ebb0: 2e4f 7074 696f 6e61 6c5b 6275 696c 7469  .Optional[builti
-0002ebc0: 6e73 2e73 7472 5d20 3d20 4e6f 6e65 2c0a  ns.str] = None,.
-0002ebd0: 2020 2020 7265 663a 2074 7970 696e 672e      ref: typing.
-0002ebe0: 4f70 7469 6f6e 616c 5b62 7569 6c74 696e  Optional[builtin
-0002ebf0: 732e 7374 725d 203d 204e 6f6e 652c 0a20  s.str] = None,. 
-0002ec00: 2020 2072 656d 6f74 653a 2074 7970 696e     remote: typin
-0002ec10: 672e 4f70 7469 6f6e 616c 5b62 7569 6c74  g.Optional[built
-0002ec20: 696e 732e 7374 725d 203d 204e 6f6e 652c  ins.str] = None,
-0002ec30: 0a20 2020 2072 756c 6573 3a20 7479 7069  .    rules: typi
-0002ec40: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-0002ec50: 6e67 2e53 6571 7565 6e63 655b 7479 7069  ng.Sequence[typi
-0002ec60: 6e67 2e55 6e69 6f6e 5b49 6e63 6c75 6465  ng.Union[Include
-0002ec70: 5275 6c65 2c20 7479 7069 6e67 2e44 6963  Rule, typing.Dic
-0002ec80: 745b 6275 696c 7469 6e73 2e73 7472 2c20  t[builtins.str, 
-0002ec90: 7479 7069 6e67 2e41 6e79 5d5d 5d5d 203d  typing.Any]]]] =
-0002eca0: 204e 6f6e 652c 0a20 2020 2074 656d 706c   None,.    templ
-0002ecb0: 6174 653a 2074 7970 696e 672e 4f70 7469  ate: typing.Opti
-0002ecc0: 6f6e 616c 5b62 7569 6c74 696e 732e 7374  onal[builtins.st
-0002ecd0: 725d 203d 204e 6f6e 652c 0a29 202d 3e20  r] = None,.) -> 
-0002ece0: 4e6f 6e65 3a0a 2020 2020 2222 2254 7970  None:.    """Typ
-0002ecf0: 6520 6368 6563 6b69 6e67 2073 7475 6273  e checking stubs
-0002ed00: 2222 220a 2020 2020 7061 7373 0a0a 6465  """.    pass..de
-0002ed10: 6620 5f74 7970 6563 6865 636b 696e 6773  f _typecheckings
-0002ed20: 7475 625f 5f35 3534 3730 3235 6262 6534  tub__5547025bbe4
-0002ed30: 3232 3132 3466 3539 6537 3832 6237 3134  22124f59e782b714
-0002ed40: 3138 3934 6261 3337 6462 6630 3034 3930  1894ba37dbf00490
-0002ed50: 3730 6337 3362 3137 6633 3964 6531 6431  70c73b17f39de1d1
-0002ed60: 3834 3361 3128 0a20 2020 202a 2c0a 2020  843a1(.    *,.  
-0002ed70: 2020 616c 6c6f 775f 6661 696c 7572 653a    allow_failure:
-0002ed80: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0002ed90: 5b74 7970 696e 672e 556e 696f 6e5b 6275  [typing.Union[bu
-0002eda0: 696c 7469 6e73 2e62 6f6f 6c2c 2074 7970  iltins.bool, typ
-0002edb0: 696e 672e 556e 696f 6e5b 416c 6c6f 7746  ing.Union[AllowF
-0002edc0: 6169 6c75 7265 2c20 7479 7069 6e67 2e44  ailure, typing.D
-0002edd0: 6963 745b 6275 696c 7469 6e73 2e73 7472  ict[builtins.str
-0002ede0: 2c20 7479 7069 6e67 2e41 6e79 5d5d 5d5d  , typing.Any]]]]
-0002edf0: 203d 204e 6f6e 652c 0a20 2020 2063 6861   = None,.    cha
-0002ee00: 6e67 6573 3a20 7479 7069 6e67 2e4f 7074  nges: typing.Opt
-0002ee10: 696f 6e61 6c5b 7479 7069 6e67 2e53 6571  ional[typing.Seq
-0002ee20: 7565 6e63 655b 6275 696c 7469 6e73 2e73  uence[builtins.s
-0002ee30: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
-0002ee40: 2065 7869 7374 733a 2074 7970 696e 672e   exists: typing.
-0002ee50: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-0002ee60: 5365 7175 656e 6365 5b62 7569 6c74 696e  Sequence[builtin
-0002ee70: 732e 7374 725d 5d20 3d20 4e6f 6e65 2c0a  s.str]] = None,.
-0002ee80: 2020 2020 6966 5f3a 2074 7970 696e 672e      if_: typing.
-0002ee90: 4f70 7469 6f6e 616c 5b62 7569 6c74 696e  Optional[builtin
-0002eea0: 732e 7374 725d 203d 204e 6f6e 652c 0a20  s.str] = None,. 
-0002eeb0: 2020 2073 7461 7274 5f69 6e3a 2074 7970     start_in: typ
-0002eec0: 696e 672e 4f70 7469 6f6e 616c 5b62 7569  ing.Optional[bui
-0002eed0: 6c74 696e 732e 7374 725d 203d 204e 6f6e  ltins.str] = Non
-0002eee0: 652c 0a20 2020 2076 6172 6961 626c 6573  e,.    variables
-0002eef0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0002ef00: 6c5b 7479 7069 6e67 2e4d 6170 7069 6e67  l[typing.Mapping
-0002ef10: 5b62 7569 6c74 696e 732e 7374 722c 2062  [builtins.str, b
-0002ef20: 7569 6c74 696e 732e 7374 725d 5d20 3d20  uiltins.str]] = 
-0002ef30: 4e6f 6e65 2c0a 2020 2020 7768 656e 3a20  None,.    when: 
-0002ef40: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0002ef50: 4a6f 6257 6865 6e5d 203d 204e 6f6e 652c  JobWhen] = None,
-0002ef60: 0a29 202d 3e20 4e6f 6e65 3a0a 2020 2020  .) -> None:.    
-0002ef70: 2222 2254 7970 6520 6368 6563 6b69 6e67  """Type checking
-0002ef80: 2073 7475 6273 2222 220a 2020 2020 7061   stubs""".    pa
-0002ef90: 7373 0a0a 6465 6620 5f74 7970 6563 6865  ss..def _typeche
-0002efa0: 636b 696e 6773 7475 625f 5f37 3865 3230  ckingstub__78e20
-0002efb0: 3230 3536 6638 6430 6565 3034 3634 3135  2056f8d0ee046415
-0002efc0: 6364 6430 6565 6261 3762 3033 6434 3134  cdd0eeba7b03d414
-0002efd0: 6262 6433 3866 6333 3637 3930 3930 3230  bbd38fc367909020
-0002efe0: 6334 6432 6432 3736 3663 6628 0a20 2020  c4d2d2766cf(.   
-0002eff0: 202a 2c0a 2020 2020 6465 6661 756c 743a   *,.    default:
-0002f000: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0002f010: 5b74 7970 696e 672e 556e 696f 6e5b 6275  [typing.Union[bu
-0002f020: 696c 7469 6e73 2e62 6f6f 6c2c 2074 7970  iltins.bool, typ
-0002f030: 696e 672e 5365 7175 656e 6365 5b44 6566  ing.Sequence[Def
-0002f040: 6175 6c74 456c 656d 656e 745d 5d5d 203d  aultElement]]] =
-0002f050: 204e 6f6e 652c 0a20 2020 2076 6172 6961   None,.    varia
-0002f060: 626c 6573 3a20 7479 7069 6e67 2e4f 7074  bles: typing.Opt
-0002f070: 696f 6e61 6c5b 7479 7069 6e67 2e55 6e69  ional[typing.Uni
-0002f080: 6f6e 5b62 7569 6c74 696e 732e 626f 6f6c  on[builtins.bool
-0002f090: 2c20 7479 7069 6e67 2e53 6571 7565 6e63  , typing.Sequenc
-0002f0a0: 655b 6275 696c 7469 6e73 2e73 7472 5d5d  e[builtins.str]]
-0002f0b0: 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e 204e  ] = None,.) -> N
-0002f0c0: 6f6e 653a 0a20 2020 2022 2222 5479 7065  one:.    """Type
-0002f0d0: 2063 6865 636b 696e 6720 7374 7562 7322   checking stubs"
-0002f0e0: 2222 0a20 2020 2070 6173 730a 0a64 6566  "".    pass..def
-0002f0f0: 205f 7479 7065 6368 6563 6b69 6e67 7374   _typecheckingst
-0002f100: 7562 5f5f 3438 3561 6662 3863 6134 6366  ub__485afb8ca4cf
-0002f110: 3132 6264 6161 6233 6333 3435 3563 3762  12bdaab3c3455c7b
-0002f120: 3930 6633 6561 3964 3534 3965 6238 3765  90f3ea9d549eb87e
-0002f130: 6336 6664 3035 6561 6530 3436 6633 6633  c6fd05eae046f3f3
-0002f140: 3862 6436 280a 2020 2020 2a2c 0a20 2020  8bd6(.    *,.   
-0002f150: 2061 6674 6572 5f73 6372 6970 743a 2074   after_script: t
-0002f160: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-0002f170: 7970 696e 672e 5365 7175 656e 6365 5b62  yping.Sequence[b
-0002f180: 7569 6c74 696e 732e 7374 725d 5d20 3d20  uiltins.str]] = 
-0002f190: 4e6f 6e65 2c0a 2020 2020 616c 6c6f 775f  None,.    allow_
-0002f1a0: 6661 696c 7572 653a 2074 7970 696e 672e  failure: typing.
-0002f1b0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-0002f1c0: 556e 696f 6e5b 6275 696c 7469 6e73 2e62  Union[builtins.b
-0002f1d0: 6f6f 6c2c 2074 7970 696e 672e 556e 696f  ool, typing.Unio
-0002f1e0: 6e5b 416c 6c6f 7746 6169 6c75 7265 2c20  n[AllowFailure, 
-0002f1f0: 7479 7069 6e67 2e44 6963 745b 6275 696c  typing.Dict[buil
-0002f200: 7469 6e73 2e73 7472 2c20 7479 7069 6e67  tins.str, typing
-0002f210: 2e41 6e79 5d5d 5d5d 203d 204e 6f6e 652c  .Any]]]] = None,
-0002f220: 0a20 2020 2061 7274 6966 6163 7473 3a20  .    artifacts: 
-0002f230: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0002f240: 7479 7069 6e67 2e55 6e69 6f6e 5b41 7274  typing.Union[Art
-0002f250: 6966 6163 7473 2c20 7479 7069 6e67 2e44  ifacts, typing.D
-0002f260: 6963 745b 6275 696c 7469 6e73 2e73 7472  ict[builtins.str
-0002f270: 2c20 7479 7069 6e67 2e41 6e79 5d5d 5d20  , typing.Any]]] 
-0002f280: 3d20 4e6f 6e65 2c0a 2020 2020 6265 666f  = None,.    befo
-0002f290: 7265 5f73 6372 6970 743a 2074 7970 696e  re_script: typin
-0002f2a0: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-0002f2b0: 672e 5365 7175 656e 6365 5b62 7569 6c74  g.Sequence[built
-0002f2c0: 696e 732e 7374 725d 5d20 3d20 4e6f 6e65  ins.str]] = None
-0002f2d0: 2c0a 2020 2020 6361 6368 653a 2074 7970  ,.    cache: typ
-0002f2e0: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
-0002f2f0: 696e 672e 5365 7175 656e 6365 5b74 7970  ing.Sequence[typ
-0002f300: 696e 672e 556e 696f 6e5b 4361 6368 652c  ing.Union[Cache,
-0002f310: 2074 7970 696e 672e 4469 6374 5b62 7569   typing.Dict[bui
-0002f320: 6c74 696e 732e 7374 722c 2074 7970 696e  ltins.str, typin
-0002f330: 672e 416e 795d 5d5d 5d20 3d20 4e6f 6e65  g.Any]]]] = None
-0002f340: 2c0a 2020 2020 636f 7665 7261 6765 3a20  ,.    coverage: 
-0002f350: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0002f360: 6275 696c 7469 6e73 2e73 7472 5d20 3d20  builtins.str] = 
-0002f370: 4e6f 6e65 2c0a 2020 2020 6465 7065 6e64  None,.    depend
-0002f380: 656e 6369 6573 3a20 7479 7069 6e67 2e4f  encies: typing.O
-0002f390: 7074 696f 6e61 6c5b 7479 7069 6e67 2e53  ptional[typing.S
-0002f3a0: 6571 7565 6e63 655b 6275 696c 7469 6e73  equence[builtins
-0002f3b0: 2e73 7472 5d5d 203d 204e 6f6e 652c 0a20  .str]] = None,. 
-0002f3c0: 2020 2065 6e76 6972 6f6e 6d65 6e74 3a20     environment: 
-0002f3d0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0002f3e0: 7479 7069 6e67 2e55 6e69 6f6e 5b62 7569  typing.Union[bui
-0002f3f0: 6c74 696e 732e 7374 722c 2074 7970 696e  ltins.str, typin
-0002f400: 672e 556e 696f 6e5b 456e 7669 726f 6e6d  g.Union[Environm
-0002f410: 656e 742c 2074 7970 696e 672e 4469 6374  ent, typing.Dict
-0002f420: 5b62 7569 6c74 696e 732e 7374 722c 2074  [builtins.str, t
-0002f430: 7970 696e 672e 416e 795d 5d5d 5d20 3d20  yping.Any]]]] = 
-0002f440: 4e6f 6e65 2c0a 2020 2020 6578 6365 7074  None,.    except
-0002f450: 5f3a 2074 7970 696e 672e 4f70 7469 6f6e  _: typing.Option
-0002f460: 616c 5b74 7970 696e 672e 556e 696f 6e5b  al[typing.Union[
-0002f470: 7479 7069 6e67 2e53 6571 7565 6e63 655b  typing.Sequence[
-0002f480: 6275 696c 7469 6e73 2e73 7472 5d2c 2074  builtins.str], t
-0002f490: 7970 696e 672e 556e 696f 6e5b 4669 6c74  yping.Union[Filt
-0002f4a0: 6572 2c20 7479 7069 6e67 2e44 6963 745b  er, typing.Dict[
-0002f4b0: 6275 696c 7469 6e73 2e73 7472 2c20 7479  builtins.str, ty
-0002f4c0: 7069 6e67 2e41 6e79 5d5d 5d5d 203d 204e  ping.Any]]]] = N
-0002f4d0: 6f6e 652c 0a20 2020 2065 7874 656e 6473  one,.    extends
-0002f4e0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0002f4f0: 6c5b 7479 7069 6e67 2e53 6571 7565 6e63  l[typing.Sequenc
-0002f500: 655b 6275 696c 7469 6e73 2e73 7472 5d5d  e[builtins.str]]
-0002f510: 203d 204e 6f6e 652c 0a20 2020 2069 645f   = None,.    id_
-0002f520: 746f 6b65 6e73 3a20 7479 7069 6e67 2e4f  tokens: typing.O
-0002f530: 7074 696f 6e61 6c5b 7479 7069 6e67 2e4d  ptional[typing.M
-0002f540: 6170 7069 6e67 5b62 7569 6c74 696e 732e  apping[builtins.
-0002f550: 7374 722c 2049 4454 6f6b 656e 5d5d 203d  str, IDToken]] =
-0002f560: 204e 6f6e 652c 0a20 2020 2069 6d61 6765   None,.    image
-0002f570: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0002f580: 6c5b 7479 7069 6e67 2e55 6e69 6f6e 5b49  l[typing.Union[I
-0002f590: 6d61 6765 2c20 7479 7069 6e67 2e44 6963  mage, typing.Dic
-0002f5a0: 745b 6275 696c 7469 6e73 2e73 7472 2c20  t[builtins.str, 
-0002f5b0: 7479 7069 6e67 2e41 6e79 5d5d 5d20 3d20  typing.Any]]] = 
-0002f5c0: 4e6f 6e65 2c0a 2020 2020 696e 6865 7269  None,.    inheri
-0002f5d0: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
-0002f5e0: 616c 5b74 7970 696e 672e 556e 696f 6e5b  al[typing.Union[
-0002f5f0: 496e 6865 7269 742c 2074 7970 696e 672e  Inherit, typing.
-0002f600: 4469 6374 5b62 7569 6c74 696e 732e 7374  Dict[builtins.st
-0002f610: 722c 2074 7970 696e 672e 416e 795d 5d5d  r, typing.Any]]]
-0002f620: 203d 204e 6f6e 652c 0a20 2020 2069 6e74   = None,.    int
-0002f630: 6572 7275 7074 6962 6c65 3a20 7479 7069  erruptible: typi
-0002f640: 6e67 2e4f 7074 696f 6e61 6c5b 6275 696c  ng.Optional[buil
-0002f650: 7469 6e73 2e62 6f6f 6c5d 203d 204e 6f6e  tins.bool] = Non
-0002f660: 652c 0a20 2020 206e 6565 6473 3a20 7479  e,.    needs: ty
-0002f670: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-0002f680: 7069 6e67 2e53 6571 7565 6e63 655b 7479  ping.Sequence[ty
-0002f690: 7069 6e67 2e55 6e69 6f6e 5b62 7569 6c74  ping.Union[built
-0002f6a0: 696e 732e 7374 722c 2074 7970 696e 672e  ins.str, typing.
-0002f6b0: 556e 696f 6e5b 4e65 6564 2c20 7479 7069  Union[Need, typi
-0002f6c0: 6e67 2e44 6963 745b 6275 696c 7469 6e73  ng.Dict[builtins
-0002f6d0: 2e73 7472 2c20 7479 7069 6e67 2e41 6e79  .str, typing.Any
-0002f6e0: 5d5d 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020  ]]]]] = None,.  
-0002f6f0: 2020 6f6e 6c79 3a20 7479 7069 6e67 2e4f    only: typing.O
-0002f700: 7074 696f 6e61 6c5b 7479 7069 6e67 2e55  ptional[typing.U
-0002f710: 6e69 6f6e 5b74 7970 696e 672e 5365 7175  nion[typing.Sequ
-0002f720: 656e 6365 5b62 7569 6c74 696e 732e 7374  ence[builtins.st
-0002f730: 725d 2c20 7479 7069 6e67 2e55 6e69 6f6e  r], typing.Union
-0002f740: 5b46 696c 7465 722c 2074 7970 696e 672e  [Filter, typing.
-0002f750: 4469 6374 5b62 7569 6c74 696e 732e 7374  Dict[builtins.st
-0002f760: 722c 2074 7970 696e 672e 416e 795d 5d5d  r, typing.Any]]]
-0002f770: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 7061  ] = None,.    pa
-0002f780: 7261 6c6c 656c 3a20 7479 7069 6e67 2e4f  rallel: typing.O
-0002f790: 7074 696f 6e61 6c5b 7479 7069 6e67 2e55  ptional[typing.U
-0002f7a0: 6e69 6f6e 5b6a 7369 692e 4e75 6d62 6572  nion[jsii.Number
-0002f7b0: 2c20 7479 7069 6e67 2e55 6e69 6f6e 5b50  , typing.Union[P
-0002f7c0: 6172 616c 6c65 6c2c 2074 7970 696e 672e  arallel, typing.
-0002f7d0: 4469 6374 5b62 7569 6c74 696e 732e 7374  Dict[builtins.st
-0002f7e0: 722c 2074 7970 696e 672e 416e 795d 5d5d  r, typing.Any]]]
-0002f7f0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 7265  ] = None,.    re
-0002f800: 6c65 6173 653a 2074 7970 696e 672e 4f70  lease: typing.Op
-0002f810: 7469 6f6e 616c 5b74 7970 696e 672e 556e  tional[typing.Un
-0002f820: 696f 6e5b 5265 6c65 6173 652c 2074 7970  ion[Release, typ
-0002f830: 696e 672e 4469 6374 5b62 7569 6c74 696e  ing.Dict[builtin
-0002f840: 732e 7374 722c 2074 7970 696e 672e 416e  s.str, typing.An
-0002f850: 795d 5d5d 203d 204e 6f6e 652c 0a20 2020  y]]] = None,.   
-0002f860: 2072 6573 6f75 7263 655f 6772 6f75 703a   resource_group:
-0002f870: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0002f880: 5b62 7569 6c74 696e 732e 7374 725d 203d  [builtins.str] =
-0002f890: 204e 6f6e 652c 0a20 2020 2072 6574 7279   None,.    retry
-0002f8a0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0002f8b0: 6c5b 7479 7069 6e67 2e55 6e69 6f6e 5b52  l[typing.Union[R
-0002f8c0: 6574 7279 2c20 7479 7069 6e67 2e44 6963  etry, typing.Dic
-0002f8d0: 745b 6275 696c 7469 6e73 2e73 7472 2c20  t[builtins.str, 
-0002f8e0: 7479 7069 6e67 2e41 6e79 5d5d 5d20 3d20  typing.Any]]] = 
-0002f8f0: 4e6f 6e65 2c0a 2020 2020 7275 6c65 733a  None,.    rules:
-0002f900: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0002f910: 5b74 7970 696e 672e 5365 7175 656e 6365  [typing.Sequence
-0002f920: 5b74 7970 696e 672e 556e 696f 6e5b 496e  [typing.Union[In
-0002f930: 636c 7564 6552 756c 652c 2074 7970 696e  cludeRule, typin
-0002f940: 672e 4469 6374 5b62 7569 6c74 696e 732e  g.Dict[builtins.
-0002f950: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
-0002f960: 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ]]] = None,.    
-0002f970: 7363 7269 7074 3a20 7479 7069 6e67 2e4f  script: typing.O
-0002f980: 7074 696f 6e61 6c5b 7479 7069 6e67 2e53  ptional[typing.S
-0002f990: 6571 7565 6e63 655b 6275 696c 7469 6e73  equence[builtins
-0002f9a0: 2e73 7472 5d5d 203d 204e 6f6e 652c 0a20  .str]] = None,. 
-0002f9b0: 2020 2073 6563 7265 7473 3a20 7479 7069     secrets: typi
-0002f9c0: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-0002f9d0: 6e67 2e4d 6170 7069 6e67 5b62 7569 6c74  ng.Mapping[built
-0002f9e0: 696e 732e 7374 722c 2074 7970 696e 672e  ins.str, typing.
-0002f9f0: 4d61 7070 696e 675b 6275 696c 7469 6e73  Mapping[builtins
-0002fa00: 2e73 7472 2c20 7479 7069 6e67 2e55 6e69  .str, typing.Uni
-0002fa10: 6f6e 5b53 6563 7265 742c 2074 7970 696e  on[Secret, typin
-0002fa20: 672e 4469 6374 5b62 7569 6c74 696e 732e  g.Dict[builtins.
-0002fa30: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
-0002fa40: 5d5d 5d5d 203d 204e 6f6e 652c 0a20 2020  ]]]] = None,.   
-0002fa50: 2073 6572 7669 6365 733a 2074 7970 696e   services: typin
-0002fa60: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-0002fa70: 672e 5365 7175 656e 6365 5b74 7970 696e  g.Sequence[typin
-0002fa80: 672e 556e 696f 6e5b 5365 7276 6963 652c  g.Union[Service,
-0002fa90: 2074 7970 696e 672e 4469 6374 5b62 7569   typing.Dict[bui
-0002faa0: 6c74 696e 732e 7374 722c 2074 7970 696e  ltins.str, typin
-0002fab0: 672e 416e 795d 5d5d 5d20 3d20 4e6f 6e65  g.Any]]]] = None
-0002fac0: 2c0a 2020 2020 7374 6167 653a 2074 7970  ,.    stage: typ
-0002fad0: 696e 672e 4f70 7469 6f6e 616c 5b62 7569  ing.Optional[bui
-0002fae0: 6c74 696e 732e 7374 725d 203d 204e 6f6e  ltins.str] = Non
-0002faf0: 652c 0a20 2020 2073 7461 7274 5f69 6e3a  e,.    start_in:
-0002fb00: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0002fb10: 5b62 7569 6c74 696e 732e 7374 725d 203d  [builtins.str] =
-0002fb20: 204e 6f6e 652c 0a20 2020 2074 6167 733a   None,.    tags:
-0002fb30: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0002fb40: 5b74 7970 696e 672e 5365 7175 656e 6365  [typing.Sequence
-0002fb50: 5b62 7569 6c74 696e 732e 7374 725d 5d20  [builtins.str]] 
-0002fb60: 3d20 4e6f 6e65 2c0a 2020 2020 7469 6d65  = None,.    time
-0002fb70: 6f75 743a 2074 7970 696e 672e 4f70 7469  out: typing.Opti
-0002fb80: 6f6e 616c 5b62 7569 6c74 696e 732e 7374  onal[builtins.st
-0002fb90: 725d 203d 204e 6f6e 652c 0a20 2020 2074  r] = None,.    t
-0002fba0: 7269 6767 6572 3a20 7479 7069 6e67 2e4f  rigger: typing.O
-0002fbb0: 7074 696f 6e61 6c5b 7479 7069 6e67 2e55  ptional[typing.U
-0002fbc0: 6e69 6f6e 5b62 7569 6c74 696e 732e 7374  nion[builtins.st
-0002fbd0: 722c 2074 7970 696e 672e 556e 696f 6e5b  r, typing.Union[
-0002fbe0: 5472 6967 6765 722c 2074 7970 696e 672e  Trigger, typing.
-0002fbf0: 4469 6374 5b62 7569 6c74 696e 732e 7374  Dict[builtins.st
-0002fc00: 722c 2074 7970 696e 672e 416e 795d 5d5d  r, typing.Any]]]
-0002fc10: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 7661  ] = None,.    va
-0002fc20: 7269 6162 6c65 733a 2074 7970 696e 672e  riables: typing.
-0002fc30: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-0002fc40: 4d61 7070 696e 675b 6275 696c 7469 6e73  Mapping[builtins
-0002fc50: 2e73 7472 2c20 6275 696c 7469 6e73 2e73  .str, builtins.s
-0002fc60: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
-0002fc70: 2077 6865 6e3a 2074 7970 696e 672e 4f70   when: typing.Op
-0002fc80: 7469 6f6e 616c 5b4a 6f62 5768 656e 5d20  tional[JobWhen] 
-0002fc90: 3d20 4e6f 6e65 2c0a 2920 2d3e 204e 6f6e  = None,.) -> Non
-0002fca0: 653a 0a20 2020 2022 2222 5479 7065 2063  e:.    """Type c
-0002fcb0: 6865 636b 696e 6720 7374 7562 7322 2222  hecking stubs"""
-0002fcc0: 0a20 2020 2070 6173 730a 0a64 6566 205f  .    pass..def _
-0002fcd0: 7479 7065 6368 6563 6b69 6e67 7374 7562  typecheckingstub
-0002fce0: 5f5f 3362 3531 3335 6531 3232 6230 6662  __3b5135e122b0fb
-0002fcf0: 3930 6335 6165 3564 3863 3635 3632 3637  90c5ae5d8c656267
-0002fd00: 3135 6332 3739 6261 3663 3862 6234 3130  15c279ba6c8bb410
-0002fd10: 3364 3462 6437 6131 3239 3639 6431 6635  3d4bd7a12969d1f5
-0002fd20: 6164 280a 2020 2020 2a2c 0a20 2020 206e  ad(.    *,.    n
-0002fd30: 616d 6573 7061 6365 3a20 7479 7069 6e67  amespace: typing
-0002fd40: 2e4f 7074 696f 6e61 6c5b 6275 696c 7469  .Optional[builti
-0002fd50: 6e73 2e73 7472 5d20 3d20 4e6f 6e65 2c0a  ns.str] = None,.
-0002fd60: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
-0002fd70: 2222 5479 7065 2063 6865 636b 696e 6720  ""Type checking 
-0002fd80: 7374 7562 7322 2222 0a20 2020 2070 6173  stubs""".    pas
-0002fd90: 730a 0a64 6566 205f 7479 7065 6368 6563  s..def _typechec
-0002fda0: 6b69 6e67 7374 7562 5f5f 3030 3336 3737  kingstub__003677
-0002fdb0: 6533 3837 3465 6432 3637 3437 6630 3438  e3874ed26747f048
-0002fdc0: 6538 6235 6330 3861 3332 6238 3766 3032  e8b5c08a32b87f02
-0002fdd0: 3236 6633 3532 3263 3130 6230 3834 3461  26f3522c10b0844a
-0002fde0: 6465 3235 3231 3936 3663 280a 2020 2020  de2521966c(.    
-0002fdf0: 2a2c 0a20 2020 206e 616d 653a 2062 7569  *,.    name: bui
-0002fe00: 6c74 696e 732e 7374 722c 0a20 2020 2075  ltins.str,.    u
-0002fe10: 726c 3a20 6275 696c 7469 6e73 2e73 7472  rl: builtins.str
-0002fe20: 2c0a 2020 2020 6669 6c65 7061 7468 3a20  ,.    filepath: 
-0002fe30: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0002fe40: 6275 696c 7469 6e73 2e73 7472 5d20 3d20  builtins.str] = 
-0002fe50: 4e6f 6e65 2c0a 2020 2020 6c69 6e6b 5f74  None,.    link_t
-0002fe60: 7970 653a 2074 7970 696e 672e 4f70 7469  ype: typing.Opti
-0002fe70: 6f6e 616c 5b4c 696e 6b54 7970 655d 203d  onal[LinkType] =
-0002fe80: 204e 6f6e 652c 0a29 202d 3e20 4e6f 6e65   None,.) -> None
-0002fe90: 3a0a 2020 2020 2222 2254 7970 6520 6368  :.    """Type ch
-0002fea0: 6563 6b69 6e67 2073 7475 6273 2222 220a  ecking stubs""".
-0002feb0: 2020 2020 7061 7373 0a0a 6465 6620 5f74      pass..def _t
-0002fec0: 7970 6563 6865 636b 696e 6773 7475 625f  ypecheckingstub_
-0002fed0: 5f63 3632 6138 6235 6435 3964 6532 3064  _c62a8b5d59de20d
-0002fee0: 3038 3131 6136 6562 3261 6538 6566 3561  0811a6eb2ae8ef5a
-0002fef0: 3338 3039 3964 3261 3964 6130 6562 6664  38099d2a9da0ebfd
-0002ff00: 3963 3963 6538 6431 3430 3663 6534 6638  9c9ce8d1406ce4f8
-0002ff10: 6528 0a20 2020 202a 2c0a 2020 2020 6a6f  e(.    *,.    jo
-0002ff20: 623a 2062 7569 6c74 696e 732e 7374 722c  b: builtins.str,
-0002ff30: 0a20 2020 2061 7274 6966 6163 7473 3a20  .    artifacts: 
-0002ff40: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0002ff50: 6275 696c 7469 6e73 2e62 6f6f 6c5d 203d  builtins.bool] =
-0002ff60: 204e 6f6e 652c 0a20 2020 206f 7074 696f   None,.    optio
-0002ff70: 6e61 6c3a 2074 7970 696e 672e 4f70 7469  nal: typing.Opti
-0002ff80: 6f6e 616c 5b62 7569 6c74 696e 732e 626f  onal[builtins.bo
-0002ff90: 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ol] = None,.    
-0002ffa0: 7069 7065 6c69 6e65 3a20 7479 7069 6e67  pipeline: typing
-0002ffb0: 2e4f 7074 696f 6e61 6c5b 6275 696c 7469  .Optional[builti
-0002ffc0: 6e73 2e73 7472 5d20 3d20 4e6f 6e65 2c0a  ns.str] = None,.
-0002ffd0: 2020 2020 7072 6f6a 6563 743a 2074 7970      project: typ
-0002ffe0: 696e 672e 4f70 7469 6f6e 616c 5b62 7569  ing.Optional[bui
-0002fff0: 6c74 696e 732e 7374 725d 203d 204e 6f6e  ltins.str] = Non
-00030000: 652c 0a20 2020 2072 6566 3a20 7479 7069  e,.    ref: typi
-00030010: 6e67 2e4f 7074 696f 6e61 6c5b 6275 696c  ng.Optional[buil
-00030020: 7469 6e73 2e73 7472 5d20 3d20 4e6f 6e65  tins.str] = None
-00030030: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
-00030040: 2022 2222 5479 7065 2063 6865 636b 696e   """Type checkin
-00030050: 6720 7374 7562 7322 2222 0a20 2020 2070  g stubs""".    p
-00030060: 6173 730a 0a64 6566 205f 7479 7065 6368  ass..def _typech
-00030070: 6563 6b69 6e67 7374 7562 5f5f 3233 6437  eckingstub__23d7
-00030080: 6631 6438 6432 3433 6662 3765 3237 3561  f1d8d243fb7e275a
-00030090: 3065 6562 6133 6631 3431 3938 3232 6266  0eeba3f1419822bf
-000300a0: 3263 3237 3465 3437 3634 3165 3535 3361  2c274e47641e553a
-000300b0: 3536 3735 6330 3032 6134 3337 280a 2020  5675c002a437(.  
-000300c0: 2020 7072 6f6a 6563 743a 205f 5072 6f6a    project: _Proj
-000300d0: 6563 745f 3537 6438 3932 3033 2c0a 2020  ect_57d89203,.  
-000300e0: 2020 7061 7265 6e74 3a20 4769 746c 6162    parent: Gitlab
-000300f0: 436f 6e66 6967 7572 6174 696f 6e2c 0a20  Configuration,. 
-00030100: 2020 206e 616d 653a 2062 7569 6c74 696e     name: builtin
-00030110: 732e 7374 722c 0a20 2020 202a 2c0a 2020  s.str,.    *,.  
-00030120: 2020 6465 6661 756c 743a 2074 7970 696e    default: typin
-00030130: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-00030140: 672e 556e 696f 6e5b 4465 6661 756c 742c  g.Union[Default,
-00030150: 2074 7970 696e 672e 4469 6374 5b62 7569   typing.Dict[bui
-00030160: 6c74 696e 732e 7374 722c 2074 7970 696e  ltins.str, typin
-00030170: 672e 416e 795d 5d5d 203d 204e 6f6e 652c  g.Any]]] = None,
-00030180: 0a20 2020 206a 6f62 733a 2074 7970 696e  .    jobs: typin
-00030190: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-000301a0: 672e 4d61 7070 696e 675b 6275 696c 7469  g.Mapping[builti
-000301b0: 6e73 2e73 7472 2c20 7479 7069 6e67 2e55  ns.str, typing.U
-000301c0: 6e69 6f6e 5b4a 6f62 2c20 7479 7069 6e67  nion[Job, typing
-000301d0: 2e44 6963 745b 6275 696c 7469 6e73 2e73  .Dict[builtins.s
-000301e0: 7472 2c20 7479 7069 6e67 2e41 6e79 5d5d  tr, typing.Any]]
-000301f0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2070  ]] = None,.    p
-00030200: 6167 6573 3a20 7479 7069 6e67 2e4f 7074  ages: typing.Opt
-00030210: 696f 6e61 6c5b 7479 7069 6e67 2e55 6e69  ional[typing.Uni
-00030220: 6f6e 5b4a 6f62 2c20 7479 7069 6e67 2e44  on[Job, typing.D
-00030230: 6963 745b 6275 696c 7469 6e73 2e73 7472  ict[builtins.str
-00030240: 2c20 7479 7069 6e67 2e41 6e79 5d5d 5d20  , typing.Any]]] 
-00030250: 3d20 4e6f 6e65 2c0a 2020 2020 7374 6167  = None,.    stag
-00030260: 6573 3a20 7479 7069 6e67 2e4f 7074 696f  es: typing.Optio
-00030270: 6e61 6c5b 7479 7069 6e67 2e53 6571 7565  nal[typing.Seque
-00030280: 6e63 655b 6275 696c 7469 6e73 2e73 7472  nce[builtins.str
-00030290: 5d5d 203d 204e 6f6e 652c 0a20 2020 2076  ]] = None,.    v
-000302a0: 6172 6961 626c 6573 3a20 7479 7069 6e67  ariables: typing
-000302b0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-000302c0: 2e4d 6170 7069 6e67 5b62 7569 6c74 696e  .Mapping[builtin
-000302d0: 732e 7374 722c 2074 7970 696e 672e 416e  s.str, typing.An
-000302e0: 795d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  y]] = None,.    
-000302f0: 776f 726b 666c 6f77 3a20 7479 7069 6e67  workflow: typing
-00030300: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-00030310: 2e55 6e69 6f6e 5b57 6f72 6b66 6c6f 772c  .Union[Workflow,
-00030320: 2074 7970 696e 672e 4469 6374 5b62 7569   typing.Dict[bui
-00030330: 6c74 696e 732e 7374 722c 2074 7970 696e  ltins.str, typin
-00030340: 672e 416e 795d 5d5d 203d 204e 6f6e 652c  g.Any]]] = None,
-00030350: 0a29 202d 3e20 4e6f 6e65 3a0a 2020 2020  .) -> None:.    
-00030360: 2222 2254 7970 6520 6368 6563 6b69 6e67  """Type checking
-00030370: 2073 7475 6273 2222 220a 2020 2020 7061   stubs""".    pa
-00030380: 7373 0a0a 6465 6620 5f74 7970 6563 6865  ss..def _typeche
-00030390: 636b 696e 6773 7475 625f 5f32 3738 3337  ckingstub__27837
-000303a0: 6165 3563 3965 3035 3865 6230 3830 3664  ae5c9e058eb0806d
-000303b0: 3161 6264 3635 3537 6333 6661 3336 3265  1abd6557c3fa362e
-000303c0: 3264 6635 3964 6361 6238 6365 3164 6235  2df59dcab8ce1db5
-000303d0: 3431 3663 3030 3532 3565 3128 0a20 2020  416c00525e1(.   
-000303e0: 202a 2c0a 2020 2020 6d61 7472 6978 3a20   *,.    matrix: 
-000303f0: 7479 7069 6e67 2e53 6571 7565 6e63 655b  typing.Sequence[
-00030400: 7479 7069 6e67 2e4d 6170 7069 6e67 5b62  typing.Mapping[b
-00030410: 7569 6c74 696e 732e 7374 722c 2074 7970  uiltins.str, typ
-00030420: 696e 672e 5365 7175 656e 6365 5b74 7970  ing.Sequence[typ
-00030430: 696e 672e 416e 795d 5d5d 2c0a 2920 2d3e  ing.Any]]],.) ->
-00030440: 204e 6f6e 653a 0a20 2020 2022 2222 5479   None:.    """Ty
-00030450: 7065 2063 6865 636b 696e 6720 7374 7562  pe checking stub
-00030460: 7322 2222 0a20 2020 2070 6173 730a 0a64  s""".    pass..d
-00030470: 6566 205f 7479 7065 6368 6563 6b69 6e67  ef _typechecking
-00030480: 7374 7562 5f5f 6333 3865 3735 3435 6361  stub__c38e7545ca
-00030490: 6632 3136 3530 6433 6664 3864 3963 3836  f21650d3fd8d9c86
-000304a0: 3732 6637 6163 3439 3937 3865 3133 3033  72f7ac49978e1303
-000304b0: 3038 6566 6637 3231 6432 3632 6635 6361  08eff721d262f5ca
-000304c0: 3836 3164 3933 280a 2020 2020 2a2c 0a20  861d93(.    *,. 
-000304d0: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-000304e0: 6275 696c 7469 6e73 2e73 7472 2c0a 2020  builtins.str,.  
-000304f0: 2020 7461 675f 6e61 6d65 3a20 6275 696c    tag_name: buil
-00030500: 7469 6e73 2e73 7472 2c0a 2020 2020 6173  tins.str,.    as
-00030510: 7365 7473 3a20 7479 7069 6e67 2e4f 7074  sets: typing.Opt
-00030520: 696f 6e61 6c5b 7479 7069 6e67 2e55 6e69  ional[typing.Uni
-00030530: 6f6e 5b41 7373 6574 732c 2074 7970 696e  on[Assets, typin
-00030540: 672e 4469 6374 5b62 7569 6c74 696e 732e  g.Dict[builtins.
-00030550: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
-00030560: 5d5d 203d 204e 6f6e 652c 0a20 2020 206d  ]] = None,.    m
-00030570: 696c 6573 746f 6e65 733a 2074 7970 696e  ilestones: typin
-00030580: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-00030590: 672e 5365 7175 656e 6365 5b62 7569 6c74  g.Sequence[built
-000305a0: 696e 732e 7374 725d 5d20 3d20 4e6f 6e65  ins.str]] = None
-000305b0: 2c0a 2020 2020 6e61 6d65 3a20 7479 7069  ,.    name: typi
-000305c0: 6e67 2e4f 7074 696f 6e61 6c5b 6275 696c  ng.Optional[buil
-000305d0: 7469 6e73 2e73 7472 5d20 3d20 4e6f 6e65  tins.str] = None
-000305e0: 2c0a 2020 2020 7265 663a 2074 7970 696e  ,.    ref: typin
-000305f0: 672e 4f70 7469 6f6e 616c 5b62 7569 6c74  g.Optional[built
-00030600: 696e 732e 7374 725d 203d 204e 6f6e 652c  ins.str] = None,
-00030610: 0a20 2020 2072 656c 6561 7365 645f 6174  .    released_at
-00030620: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00030630: 6c5b 6275 696c 7469 6e73 2e73 7472 5d20  l[builtins.str] 
-00030640: 3d20 4e6f 6e65 2c0a 2920 2d3e 204e 6f6e  = None,.) -> Non
-00030650: 653a 0a20 2020 2022 2222 5479 7065 2063  e:.    """Type c
-00030660: 6865 636b 696e 6720 7374 7562 7322 2222  hecking stubs"""
-00030670: 0a20 2020 2070 6173 730a 0a64 6566 205f  .    pass..def _
-00030680: 7479 7065 6368 6563 6b69 6e67 7374 7562  typecheckingstub
-00030690: 5f5f 3263 3966 3430 3330 6364 3665 3664  __2c9f4030cd6e6d
-000306a0: 3963 3839 3838 3038 3061 6665 3132 3334  9c8988080afe1234
-000306b0: 3164 3637 3461 3664 3037 3531 6461 3163  1d674a6d0751da1c
-000306c0: 3739 3337 6464 3339 3031 6339 6436 3036  7937dd3901c9d606
-000306d0: 3263 280a 2020 2020 2a2c 0a20 2020 2063  2c(.    *,.    c
-000306e0: 6f62 6572 7475 7261 3a20 7479 7069 6e67  obertura: typing
-000306f0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-00030700: 2e53 6571 7565 6e63 655b 6275 696c 7469  .Sequence[builti
-00030710: 6e73 2e73 7472 5d5d 203d 204e 6f6e 652c  ns.str]] = None,
-00030720: 0a20 2020 2063 6f64 6571 7561 6c69 7479  .    codequality
-00030730: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00030740: 6c5b 7479 7069 6e67 2e53 6571 7565 6e63  l[typing.Sequenc
-00030750: 655b 6275 696c 7469 6e73 2e73 7472 5d5d  e[builtins.str]]
-00030760: 203d 204e 6f6e 652c 0a20 2020 2063 6f6e   = None,.    con
-00030770: 7461 696e 6572 5f73 6361 6e6e 696e 673a  tainer_scanning:
-00030780: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00030790: 5b74 7970 696e 672e 5365 7175 656e 6365  [typing.Sequence
-000307a0: 5b62 7569 6c74 696e 732e 7374 725d 5d20  [builtins.str]] 
-000307b0: 3d20 4e6f 6e65 2c0a 2020 2020 636f 7665  = None,.    cove
-000307c0: 7261 6765 5f72 6570 6f72 743a 2074 7970  rage_report: typ
-000307d0: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
-000307e0: 696e 672e 556e 696f 6e5b 436f 7665 7261  ing.Union[Covera
-000307f0: 6765 5265 706f 7274 2c20 7479 7069 6e67  geReport, typing
-00030800: 2e44 6963 745b 6275 696c 7469 6e73 2e73  .Dict[builtins.s
-00030810: 7472 2c20 7479 7069 6e67 2e41 6e79 5d5d  tr, typing.Any]]
-00030820: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6461  ] = None,.    da
-00030830: 7374 3a20 7479 7069 6e67 2e4f 7074 696f  st: typing.Optio
-00030840: 6e61 6c5b 7479 7069 6e67 2e53 6571 7565  nal[typing.Seque
-00030850: 6e63 655b 6275 696c 7469 6e73 2e73 7472  nce[builtins.str
-00030860: 5d5d 203d 204e 6f6e 652c 0a20 2020 2064  ]] = None,.    d
-00030870: 6570 656e 6465 6e63 795f 7363 616e 6e69  ependency_scanni
-00030880: 6e67 3a20 7479 7069 6e67 2e4f 7074 696f  ng: typing.Optio
-00030890: 6e61 6c5b 7479 7069 6e67 2e53 6571 7565  nal[typing.Seque
-000308a0: 6e63 655b 6275 696c 7469 6e73 2e73 7472  nce[builtins.str
-000308b0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2064  ]] = None,.    d
-000308c0: 6f74 656e 763a 2074 7970 696e 672e 4f70  otenv: typing.Op
-000308d0: 7469 6f6e 616c 5b74 7970 696e 672e 5365  tional[typing.Se
-000308e0: 7175 656e 6365 5b62 7569 6c74 696e 732e  quence[builtins.
-000308f0: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
-00030900: 2020 6a75 6e69 743a 2074 7970 696e 672e    junit: typing.
-00030910: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-00030920: 5365 7175 656e 6365 5b62 7569 6c74 696e  Sequence[builtin
-00030930: 732e 7374 725d 5d20 3d20 4e6f 6e65 2c0a  s.str]] = None,.
-00030940: 2020 2020 6c69 6365 6e73 655f 6d61 6e61      license_mana
-00030950: 6765 6d65 6e74 3a20 7479 7069 6e67 2e4f  gement: typing.O
-00030960: 7074 696f 6e61 6c5b 7479 7069 6e67 2e53  ptional[typing.S
-00030970: 6571 7565 6e63 655b 6275 696c 7469 6e73  equence[builtins
-00030980: 2e73 7472 5d5d 203d 204e 6f6e 652c 0a20  .str]] = None,. 
-00030990: 2020 206c 6963 656e 7365 5f73 6361 6e6e     license_scann
-000309a0: 696e 673a 2074 7970 696e 672e 4f70 7469  ing: typing.Opti
-000309b0: 6f6e 616c 5b74 7970 696e 672e 5365 7175  onal[typing.Sequ
-000309c0: 656e 6365 5b62 7569 6c74 696e 732e 7374  ence[builtins.st
-000309d0: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
-000309e0: 6c73 6966 3a20 7479 7069 6e67 2e4f 7074  lsif: typing.Opt
-000309f0: 696f 6e61 6c5b 7479 7069 6e67 2e53 6571  ional[typing.Seq
-00030a00: 7565 6e63 655b 6275 696c 7469 6e73 2e73  uence[builtins.s
-00030a10: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
-00030a20: 206d 6574 7269 6373 3a20 7479 7069 6e67   metrics: typing
-00030a30: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-00030a40: 2e53 6571 7565 6e63 655b 6275 696c 7469  .Sequence[builti
-00030a50: 6e73 2e73 7472 5d5d 203d 204e 6f6e 652c  ns.str]] = None,
-00030a60: 0a20 2020 2070 6572 666f 726d 616e 6365  .    performance
-00030a70: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00030a80: 6c5b 7479 7069 6e67 2e53 6571 7565 6e63  l[typing.Sequenc
-00030a90: 655b 6275 696c 7469 6e73 2e73 7472 5d5d  e[builtins.str]]
-00030aa0: 203d 204e 6f6e 652c 0a20 2020 2072 6571   = None,.    req
-00030ab0: 7569 7265 6d65 6e74 733a 2074 7970 696e  uirements: typin
-00030ac0: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-00030ad0: 672e 5365 7175 656e 6365 5b62 7569 6c74  g.Sequence[built
-00030ae0: 696e 732e 7374 725d 5d20 3d20 4e6f 6e65  ins.str]] = None
-00030af0: 2c0a 2020 2020 7361 7374 3a20 7479 7069  ,.    sast: typi
-00030b00: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-00030b10: 6e67 2e53 6571 7565 6e63 655b 6275 696c  ng.Sequence[buil
-00030b20: 7469 6e73 2e73 7472 5d5d 203d 204e 6f6e  tins.str]] = Non
-00030b30: 652c 0a20 2020 2073 6563 7265 745f 6465  e,.    secret_de
-00030b40: 7465 6374 696f 6e3a 2074 7970 696e 672e  tection: typing.
-00030b50: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-00030b60: 5365 7175 656e 6365 5b62 7569 6c74 696e  Sequence[builtin
-00030b70: 732e 7374 725d 5d20 3d20 4e6f 6e65 2c0a  s.str]] = None,.
-00030b80: 2020 2020 7465 7272 6166 6f72 6d3a 2074      terraform: t
-00030b90: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-00030ba0: 7970 696e 672e 5365 7175 656e 6365 5b62  yping.Sequence[b
-00030bb0: 7569 6c74 696e 732e 7374 725d 5d20 3d20  uiltins.str]] = 
-00030bc0: 4e6f 6e65 2c0a 2920 2d3e 204e 6f6e 653a  None,.) -> None:
-00030bd0: 0a20 2020 2022 2222 5479 7065 2063 6865  .    """Type che
-00030be0: 636b 696e 6720 7374 7562 7322 2222 0a20  cking stubs""". 
-00030bf0: 2020 2070 6173 730a 0a64 6566 205f 7479     pass..def _ty
-00030c00: 7065 6368 6563 6b69 6e67 7374 7562 5f5f  pecheckingstub__
-00030c10: 6563 6262 3537 6330 6339 3134 6433 6665  ecbb57c0c914d3fe
-00030c20: 3631 6164 3066 6333 3063 3636 6231 6661  61ad0fc30c66b1fa
-00030c30: 3839 3234 3232 3537 6165 3265 3766 6264  89242257ae2e7fbd
-00030c40: 3330 3965 3538 3139 3235 3061 6332 3565  309e5819250ac25e
-00030c50: 280a 2020 2020 2a2c 0a20 2020 206d 6178  (.    *,.    max
-00030c60: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00030c70: 6c5b 6a73 6969 2e4e 756d 6265 725d 203d  l[jsii.Number] =
-00030c80: 204e 6f6e 652c 0a20 2020 2077 6865 6e3a   None,.    when:
-00030c90: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
-00030ca0: 6e65 2c0a 2920 2d3e 204e 6f6e 653a 0a20  ne,.) -> None:. 
-00030cb0: 2020 2022 2222 5479 7065 2063 6865 636b     """Type check
-00030cc0: 696e 6720 7374 7562 7322 2222 0a20 2020  ing stubs""".   
-00030cd0: 2070 6173 730a 0a64 6566 205f 7479 7065   pass..def _type
-00030ce0: 6368 6563 6b69 6e67 7374 7562 5f5f 3738  checkingstub__78
-00030cf0: 3961 6238 3761 3933 3766 3735 3239 3132  9ab87a937f752912
-00030d00: 3366 3764 6665 3135 6634 3733 3166 6232  3f7dfe15f4731fb2
-00030d10: 6261 3263 6433 3532 3936 3831 6131 6335  ba2cd3529681a1c5
-00030d20: 6237 6332 3736 3661 6335 3138 6564 280a  b7c2766ac518ed(.
-00030d30: 2020 2020 2a2c 0a20 2020 2076 6175 6c74      *,.    vault
-00030d40: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b56  : typing.Union[V
-00030d50: 6175 6c74 436f 6e66 6967 2c20 7479 7069  aultConfig, typi
-00030d60: 6e67 2e44 6963 745b 6275 696c 7469 6e73  ng.Dict[builtins
-00030d70: 2e73 7472 2c20 7479 7069 6e67 2e41 6e79  .str, typing.Any
-00030d80: 5d5d 2c0a 2920 2d3e 204e 6f6e 653a 0a20  ]],.) -> None:. 
-00030d90: 2020 2022 2222 5479 7065 2063 6865 636b     """Type check
-00030da0: 696e 6720 7374 7562 7322 2222 0a20 2020  ing stubs""".   
-00030db0: 2070 6173 730a 0a64 6566 205f 7479 7065   pass..def _type
-00030dc0: 6368 6563 6b69 6e67 7374 7562 5f5f 3165  checkingstub__1e
-00030dd0: 3230 3934 3638 6133 6639 6161 6236 6630  209468a3f9aab6f0
-00030de0: 3534 3236 3131 6263 3565 3262 3735 3662  542611bc5e2b756b
-00030df0: 6163 3432 3436 3134 3133 6561 6561 6431  ac42461413eaead1
-00030e00: 3738 3661 3162 3833 6564 3364 3237 280a  786a1b83ed3d27(.
-00030e10: 2020 2020 2a2c 0a20 2020 206e 616d 653a      *,.    name:
-00030e20: 2062 7569 6c74 696e 732e 7374 722c 0a20   builtins.str,. 
-00030e30: 2020 2061 6c69 6173 3a20 7479 7069 6e67     alias: typing
-00030e40: 2e4f 7074 696f 6e61 6c5b 6275 696c 7469  .Optional[builti
-00030e50: 6e73 2e73 7472 5d20 3d20 4e6f 6e65 2c0a  ns.str] = None,.
-00030e60: 2020 2020 636f 6d6d 616e 643a 2074 7970      command: typ
-00030e70: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
-00030e80: 696e 672e 5365 7175 656e 6365 5b62 7569  ing.Sequence[bui
-00030e90: 6c74 696e 732e 7374 725d 5d20 3d20 4e6f  ltins.str]] = No
-00030ea0: 6e65 2c0a 2020 2020 656e 7472 7970 6f69  ne,.    entrypoi
-00030eb0: 6e74 3a20 7479 7069 6e67 2e4f 7074 696f  nt: typing.Optio
-00030ec0: 6e61 6c5b 7479 7069 6e67 2e53 6571 7565  nal[typing.Seque
-00030ed0: 6e63 655b 6275 696c 7469 6e73 2e73 7472  nce[builtins.str
-00030ee0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2070  ]] = None,.    p
-00030ef0: 756c 6c5f 706f 6c69 6379 3a20 7479 7069  ull_policy: typi
-00030f00: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-00030f10: 6e67 2e53 6571 7565 6e63 655b 5075 6c6c  ng.Sequence[Pull
-00030f20: 506f 6c69 6379 5d5d 203d 204e 6f6e 652c  Policy]] = None,
-00030f30: 0a20 2020 2076 6172 6961 626c 6573 3a20  .    variables: 
-00030f40: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00030f50: 7479 7069 6e67 2e4d 6170 7069 6e67 5b62  typing.Mapping[b
-00030f60: 7569 6c74 696e 732e 7374 722c 2062 7569  uiltins.str, bui
-00030f70: 6c74 696e 732e 7374 725d 5d20 3d20 4e6f  ltins.str]] = No
-00030f80: 6e65 2c0a 2920 2d3e 204e 6f6e 653a 0a20  ne,.) -> None:. 
-00030f90: 2020 2022 2222 5479 7065 2063 6865 636b     """Type check
-00030fa0: 696e 6720 7374 7562 7322 2222 0a20 2020  ing stubs""".   
-00030fb0: 2070 6173 730a 0a64 6566 205f 7479 7065   pass..def _type
-00030fc0: 6368 6563 6b69 6e67 7374 7562 5f5f 3738  checkingstub__78
-00030fd0: 6165 6336 6136 6334 3632 3333 3163 6666  aec6a6c462331cff
-00030fe0: 6238 6438 6166 3531 3161 3761 3034 6561  b8d8af511a7a04ea
-00030ff0: 3936 6137 6532 3630 6530 3366 3864 3835  96a7e260e03f8d85
-00031000: 3762 6135 3731 3033 6236 6338 3966 280a  7ba57103b6c89f(.
-00031010: 2020 2020 2a2c 0a20 2020 2062 7261 6e63      *,.    branc
-00031020: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
-00031030: 616c 5b62 7569 6c74 696e 732e 7374 725d  al[builtins.str]
-00031040: 203d 204e 6f6e 652c 0a20 2020 2069 6e63   = None,.    inc
-00031050: 6c75 6465 3a20 7479 7069 6e67 2e4f 7074  lude: typing.Opt
-00031060: 696f 6e61 6c5b 7479 7069 6e67 2e53 6571  ional[typing.Seq
-00031070: 7565 6e63 655b 7479 7069 6e67 2e55 6e69  uence[typing.Uni
-00031080: 6f6e 5b54 7269 6767 6572 496e 636c 7564  on[TriggerInclud
-00031090: 652c 2074 7970 696e 672e 4469 6374 5b62  e, typing.Dict[b
-000310a0: 7569 6c74 696e 732e 7374 722c 2074 7970  uiltins.str, typ
-000310b0: 696e 672e 416e 795d 5d5d 5d20 3d20 4e6f  ing.Any]]]] = No
-000310c0: 6e65 2c0a 2020 2020 7072 6f6a 6563 743a  ne,.    project:
-000310d0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-000310e0: 5b62 7569 6c74 696e 732e 7374 725d 203d  [builtins.str] =
-000310f0: 204e 6f6e 652c 0a20 2020 2073 7472 6174   None,.    strat
-00031100: 6567 793a 2074 7970 696e 672e 4f70 7469  egy: typing.Opti
-00031110: 6f6e 616c 5b53 7472 6174 6567 795d 203d  onal[Strategy] =
-00031120: 204e 6f6e 652c 0a29 202d 3e20 4e6f 6e65   None,.) -> None
-00031130: 3a0a 2020 2020 2222 2254 7970 6520 6368  :.    """Type ch
-00031140: 6563 6b69 6e67 2073 7475 6273 2222 220a  ecking stubs""".
-00031150: 2020 2020 7061 7373 0a0a 6465 6620 5f74      pass..def _t
-00031160: 7970 6563 6865 636b 696e 6773 7475 625f  ypecheckingstub_
-00031170: 5f62 6366 3439 6538 6363 6265 3331 3534  _bcf49e8ccbe3154
-00031180: 6337 3432 6636 6631 3064 6636 3065 3339  c742f6f10df60e39
-00031190: 3236 3666 6239 3438 3162 3063 3236 3538  266fb9481b0c2658
-000311a0: 3234 3236 3539 3062 6638 6364 3033 6534  2426590bf8cd03e4
-000311b0: 6228 0a20 2020 202a 2c0a 2020 2020 6172  b(.    *,.    ar
-000311c0: 7469 6661 6374 3a20 7479 7069 6e67 2e4f  tifact: typing.O
-000311d0: 7074 696f 6e61 6c5b 6275 696c 7469 6e73  ptional[builtins
-000311e0: 2e73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  .str] = None,.  
-000311f0: 2020 6669 6c65 3a20 7479 7069 6e67 2e4f    file: typing.O
-00031200: 7074 696f 6e61 6c5b 6275 696c 7469 6e73  ptional[builtins
-00031210: 2e73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  .str] = None,.  
-00031220: 2020 6a6f 623a 2074 7970 696e 672e 4f70    job: typing.Op
-00031230: 7469 6f6e 616c 5b62 7569 6c74 696e 732e  tional[builtins.
-00031240: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00031250: 206c 6f63 616c 3a20 7479 7069 6e67 2e4f   local: typing.O
-00031260: 7074 696f 6e61 6c5b 6275 696c 7469 6e73  ptional[builtins
-00031270: 2e73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  .str] = None,.  
-00031280: 2020 7072 6f6a 6563 743a 2074 7970 696e    project: typin
-00031290: 672e 4f70 7469 6f6e 616c 5b62 7569 6c74  g.Optional[built
-000312a0: 696e 732e 7374 725d 203d 204e 6f6e 652c  ins.str] = None,
-000312b0: 0a20 2020 2072 6566 3a20 7479 7069 6e67  .    ref: typing
-000312c0: 2e4f 7074 696f 6e61 6c5b 6275 696c 7469  .Optional[builti
-000312d0: 6e73 2e73 7472 5d20 3d20 4e6f 6e65 2c0a  ns.str] = None,.
-000312e0: 2020 2020 7465 6d70 6c61 7465 3a20 7479      template: ty
-000312f0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 6275  ping.Optional[bu
-00031300: 696c 7469 6e73 2e73 7472 5d20 3d20 4e6f  iltins.str] = No
-00031310: 6e65 2c0a 2920 2d3e 204e 6f6e 653a 0a20  ne,.) -> None:. 
-00031320: 2020 2022 2222 5479 7065 2063 6865 636b     """Type check
-00031330: 696e 6720 7374 7562 7322 2222 0a20 2020  ing stubs""".   
-00031340: 2070 6173 730a 0a64 6566 205f 7479 7065   pass..def _type
-00031350: 6368 6563 6b69 6e67 7374 7562 5f5f 3237  checkingstub__27
-00031360: 3064 3334 3432 6432 6335 6239 6631 3865  0d3442d2c5b9f18e
-00031370: 3437 3562 6132 6339 3435 6361 3537 3635  475ba2c945ca5765
-00031380: 6565 3631 6564 3934 6335 6561 3238 6434  ee61ed94c5ea28d4
-00031390: 3339 3562 3963 3339 3532 6466 3538 280a  395b9c3952df58(.
-000313a0: 2020 2020 2a2c 0a20 2020 2064 6573 6372      *,.    descr
-000313b0: 6970 7469 6f6e 3a20 7479 7069 6e67 2e4f  iption: typing.O
-000313c0: 7074 696f 6e61 6c5b 6275 696c 7469 6e73  ptional[builtins
-000313d0: 2e73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  .str] = None,.  
-000313e0: 2020 7661 6c75 653a 2074 7970 696e 672e    value: typing.
-000313f0: 4f70 7469 6f6e 616c 5b62 7569 6c74 696e  Optional[builtin
-00031400: 732e 7374 725d 203d 204e 6f6e 652c 0a29  s.str] = None,.)
-00031410: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
-00031420: 2254 7970 6520 6368 6563 6b69 6e67 2073  "Type checking s
-00031430: 7475 6273 2222 220a 2020 2020 7061 7373  tubs""".    pass
-00031440: 0a0a 6465 6620 5f74 7970 6563 6865 636b  ..def _typecheck
-00031450: 696e 6773 7475 625f 5f38 6266 3862 3838  ingstub__8bf8b88
-00031460: 3939 3565 3762 3233 3665 3035 3438 6166  995e7b236e0548af
-00031470: 6435 3630 3034 3166 6338 6465 3638 3363  d560041fc8de683c
-00031480: 3731 3730 3832 3138 6365 3161 6632 3831  71708218ce1af281
-00031490: 3865 6664 3362 3234 3828 0a20 2020 202a  8efd3b248(.    *
-000314a0: 2c0a 2020 2020 656e 6769 6e65 3a20 7479  ,.    engine: ty
-000314b0: 7069 6e67 2e55 6e69 6f6e 5b45 6e67 696e  ping.Union[Engin
-000314c0: 652c 2074 7970 696e 672e 4469 6374 5b62  e, typing.Dict[b
-000314d0: 7569 6c74 696e 732e 7374 722c 2074 7970  uiltins.str, typ
-000314e0: 696e 672e 416e 795d 5d2c 0a20 2020 2066  ing.Any]],.    f
-000314f0: 6965 6c64 3a20 6275 696c 7469 6e73 2e73  ield: builtins.s
-00031500: 7472 2c0a 2020 2020 7061 7468 3a20 6275  tr,.    path: bu
-00031510: 696c 7469 6e73 2e73 7472 2c0a 2920 2d3e  iltins.str,.) ->
-00031520: 204e 6f6e 653a 0a20 2020 2022 2222 5479   None:.    """Ty
-00031530: 7065 2063 6865 636b 696e 6720 7374 7562  pe checking stub
-00031540: 7322 2222 0a20 2020 2070 6173 730a 0a64  s""".    pass..d
-00031550: 6566 205f 7479 7065 6368 6563 6b69 6e67  ef _typechecking
-00031560: 7374 7562 5f5f 6530 6237 3530 3437 6636  stub__e0b75047f6
-00031570: 6266 3765 6237 3838 6230 3866 6330 3037  bf7eb788b08fc007
-00031580: 6136 3635 3733 3438 3061 3338 6539 3133  a66573480a38e913
-00031590: 6264 6533 3531 6163 6161 6330 3533 3437  bde351acaac05347
-000315a0: 6434 3637 6231 280a 2020 2020 2a2c 0a20  d467b1(.    *,. 
-000315b0: 2020 2072 756c 6573 3a20 7479 7069 6e67     rules: typing
-000315c0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-000315d0: 2e53 6571 7565 6e63 655b 7479 7069 6e67  .Sequence[typing
-000315e0: 2e55 6e69 6f6e 5b57 6f72 6b66 6c6f 7752  .Union[WorkflowR
-000315f0: 756c 652c 2074 7970 696e 672e 4469 6374  ule, typing.Dict
-00031600: 5b62 7569 6c74 696e 732e 7374 722c 2074  [builtins.str, t
-00031610: 7970 696e 672e 416e 795d 5d5d 5d20 3d20  yping.Any]]]] = 
-00031620: 4e6f 6e65 2c0a 2920 2d3e 204e 6f6e 653a  None,.) -> None:
-00031630: 0a20 2020 2022 2222 5479 7065 2063 6865  .    """Type che
-00031640: 636b 696e 6720 7374 7562 7322 2222 0a20  cking stubs""". 
-00031650: 2020 2070 6173 730a 0a64 6566 205f 7479     pass..def _ty
-00031660: 7065 6368 6563 6b69 6e67 7374 7562 5f5f  pecheckingstub__
-00031670: 3031 6132 6366 3463 3261 3938 3261 3734  01a2cf4c2a982a74
-00031680: 3964 3132 3531 3164 3965 3433 3436 3866  9d12511d9e43468f
-00031690: 3362 3461 3963 6361 3136 6436 6335 3664  3b4a9cca16d6c56d
-000316a0: 3961 3263 6664 3131 3534 3732 3064 3633  9a2cfd1154720d63
-000316b0: 280a 2020 2020 2a2c 0a20 2020 2063 6861  (.    *,.    cha
-000316c0: 6e67 6573 3a20 7479 7069 6e67 2e4f 7074  nges: typing.Opt
-000316d0: 696f 6e61 6c5b 7479 7069 6e67 2e53 6571  ional[typing.Seq
-000316e0: 7565 6e63 655b 6275 696c 7469 6e73 2e73  uence[builtins.s
-000316f0: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
-00031700: 2065 7869 7374 733a 2074 7970 696e 672e   exists: typing.
-00031710: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-00031720: 5365 7175 656e 6365 5b62 7569 6c74 696e  Sequence[builtin
-00031730: 732e 7374 725d 5d20 3d20 4e6f 6e65 2c0a  s.str]] = None,.
-00031740: 2020 2020 6966 5f3a 2074 7970 696e 672e      if_: typing.
-00031750: 4f70 7469 6f6e 616c 5b62 7569 6c74 696e  Optional[builtin
-00031760: 732e 7374 725d 203d 204e 6f6e 652c 0a20  s.str] = None,. 
-00031770: 2020 2076 6172 6961 626c 6573 3a20 7479     variables: ty
-00031780: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-00031790: 7069 6e67 2e4d 6170 7069 6e67 5b62 7569  ping.Mapping[bui
-000317a0: 6c74 696e 732e 7374 722c 2074 7970 696e  ltins.str, typin
-000317b0: 672e 556e 696f 6e5b 6275 696c 7469 6e73  g.Union[builtins
-000317c0: 2e73 7472 2c20 6a73 6969 2e4e 756d 6265  .str, jsii.Numbe
-000317d0: 725d 5d5d 203d 204e 6f6e 652c 0a20 2020  r]]] = None,.   
-000317e0: 2077 6865 6e3a 2074 7970 696e 672e 4f70   when: typing.Op
-000317f0: 7469 6f6e 616c 5b4a 6f62 5768 656e 5d20  tional[JobWhen] 
-00031800: 3d20 4e6f 6e65 2c0a 2920 2d3e 204e 6f6e  = None,.) -> Non
-00031810: 653a 0a20 2020 2022 2222 5479 7065 2063  e:.    """Type c
-00031820: 6865 636b 696e 6720 7374 7562 7322 2222  hecking stubs"""
-00031830: 0a20 2020 2070 6173 730a                 .    pass.
+0002b880: 7074 696f 6e61 6c5b 2257 6f72 6b66 6c6f  ptional["Workflo
+0002b890: 7757 6865 6e22 5d20 3d20 4e6f 6e65 2c0a  wWhen"] = None,.
+0002b8a0: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
+0002b8b0: 2020 2020 2020 2027 2727 2865 7870 6572         '''(exper
+0002b8c0: 696d 656e 7461 6c29 2055 7365 6420 746f  imental) Used to
+0002b8d0: 2063 6f6e 7472 6f6c 2077 6865 7468 6572   control whether
+0002b8e0: 206f 7220 6e6f 7420 6120 7768 6f6c 6520   or not a whole 
+0002b8f0: 7069 7065 6c69 6e65 2069 7320 6372 6561  pipeline is crea
+0002b900: 7465 642e 0a0a 2020 2020 2020 2020 3a70  ted...        :p
+0002b910: 6172 616d 2063 6861 6e67 6573 3a20 0a20  aram changes: . 
+0002b920: 2020 2020 2020 203a 7061 7261 6d20 6578         :param ex
+0002b930: 6973 7473 3a20 0a20 2020 2020 2020 203a  ists: .        :
+0002b940: 7061 7261 6d20 6966 5f3a 200a 2020 2020  param if_: .    
+0002b950: 2020 2020 3a70 6172 616d 2076 6172 6961      :param varia
+0002b960: 626c 6573 3a20 0a20 2020 2020 2020 203a  bles: .        :
+0002b970: 7061 7261 6d20 7768 656e 3a20 0a0a 2020  param when: ..  
+0002b980: 2020 2020 2020 3a73 6565 3a20 6874 7470        :see: http
+0002b990: 733a 2f2f 646f 6373 2e67 6974 6c61 622e  s://docs.gitlab.
+0002b9a0: 636f 6d2f 6565 2f63 692f 7961 6d6c 2f23  com/ee/ci/yaml/#
+0002b9b0: 776f 726b 666c 6f77 7275 6c65 730a 2020  workflowrules.  
+0002b9c0: 2020 2020 2020 3a73 7461 6269 6c69 7479        :stability
+0002b9d0: 3a20 6578 7065 7269 6d65 6e74 616c 0a20  : experimental. 
+0002b9e0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0002b9f0: 2020 2069 6620 5f5f 6465 6275 675f 5f3a     if __debug__:
+0002ba00: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
+0002ba10: 655f 6869 6e74 7320 3d20 7479 7069 6e67  e_hints = typing
+0002ba20: 2e67 6574 5f74 7970 655f 6869 6e74 7328  .get_type_hints(
+0002ba30: 5f74 7970 6563 6865 636b 696e 6773 7475  _typecheckingstu
+0002ba40: 625f 5f30 3161 3263 6634 6332 6139 3832  b__01a2cf4c2a982
+0002ba50: 6137 3439 6431 3235 3131 6439 6534 3334  a749d12511d9e434
+0002ba60: 3638 6633 6234 6139 6363 6131 3664 3663  68f3b4a9cca16d6c
+0002ba70: 3536 6439 6132 6366 6431 3135 3437 3230  56d9a2cfd1154720
+0002ba80: 6436 3329 0a20 2020 2020 2020 2020 2020  d63).           
+0002ba90: 2063 6865 636b 5f74 7970 6528 6172 676e   check_type(argn
+0002baa0: 616d 653d 2261 7267 756d 656e 7420 6368  ame="argument ch
+0002bab0: 616e 6765 7322 2c20 7661 6c75 653d 6368  anges", value=ch
+0002bac0: 616e 6765 732c 2065 7870 6563 7465 645f  anges, expected_
+0002bad0: 7479 7065 3d74 7970 655f 6869 6e74 735b  type=type_hints[
+0002bae0: 2263 6861 6e67 6573 225d 290a 2020 2020  "changes"]).    
+0002baf0: 2020 2020 2020 2020 6368 6563 6b5f 7479          check_ty
+0002bb00: 7065 2861 7267 6e61 6d65 3d22 6172 6775  pe(argname="argu
+0002bb10: 6d65 6e74 2065 7869 7374 7322 2c20 7661  ment exists", va
+0002bb20: 6c75 653d 6578 6973 7473 2c20 6578 7065  lue=exists, expe
+0002bb30: 6374 6564 5f74 7970 653d 7479 7065 5f68  cted_type=type_h
+0002bb40: 696e 7473 5b22 6578 6973 7473 225d 290a  ints["exists"]).
+0002bb50: 2020 2020 2020 2020 2020 2020 6368 6563              chec
+0002bb60: 6b5f 7479 7065 2861 7267 6e61 6d65 3d22  k_type(argname="
+0002bb70: 6172 6775 6d65 6e74 2069 665f 222c 2076  argument if_", v
+0002bb80: 616c 7565 3d69 665f 2c20 6578 7065 6374  alue=if_, expect
+0002bb90: 6564 5f74 7970 653d 7479 7065 5f68 696e  ed_type=type_hin
+0002bba0: 7473 5b22 6966 5f22 5d29 0a20 2020 2020  ts["if_"]).     
+0002bbb0: 2020 2020 2020 2063 6865 636b 5f74 7970         check_typ
+0002bbc0: 6528 6172 676e 616d 653d 2261 7267 756d  e(argname="argum
+0002bbd0: 656e 7420 7661 7269 6162 6c65 7322 2c20  ent variables", 
+0002bbe0: 7661 6c75 653d 7661 7269 6162 6c65 732c  value=variables,
+0002bbf0: 2065 7870 6563 7465 645f 7479 7065 3d74   expected_type=t
+0002bc00: 7970 655f 6869 6e74 735b 2276 6172 6961  ype_hints["varia
+0002bc10: 626c 6573 225d 290a 2020 2020 2020 2020  bles"]).        
+0002bc20: 2020 2020 6368 6563 6b5f 7479 7065 2861      check_type(a
+0002bc30: 7267 6e61 6d65 3d22 6172 6775 6d65 6e74  rgname="argument
+0002bc40: 2077 6865 6e22 2c20 7661 6c75 653d 7768   when", value=wh
+0002bc50: 656e 2c20 6578 7065 6374 6564 5f74 7970  en, expected_typ
+0002bc60: 653d 7479 7065 5f68 696e 7473 5b22 7768  e=type_hints["wh
+0002bc70: 656e 225d 290a 2020 2020 2020 2020 7365  en"]).        se
+0002bc80: 6c66 2e5f 7661 6c75 6573 3a20 7479 7069  lf._values: typi
+0002bc90: 6e67 2e44 6963 745b 6275 696c 7469 6e73  ng.Dict[builtins
+0002bca0: 2e73 7472 2c20 7479 7069 6e67 2e41 6e79  .str, typing.Any
+0002bcb0: 5d20 3d20 7b7d 0a20 2020 2020 2020 2069  ] = {}.        i
+0002bcc0: 6620 6368 616e 6765 7320 6973 206e 6f74  f changes is not
+0002bcd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002bce0: 2020 2073 656c 662e 5f76 616c 7565 735b     self._values[
+0002bcf0: 2263 6861 6e67 6573 225d 203d 2063 6861  "changes"] = cha
+0002bd00: 6e67 6573 0a20 2020 2020 2020 2069 6620  nges.        if 
+0002bd10: 6578 6973 7473 2069 7320 6e6f 7420 4e6f  exists is not No
+0002bd20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002bd30: 7365 6c66 2e5f 7661 6c75 6573 5b22 6578  self._values["ex
+0002bd40: 6973 7473 225d 203d 2065 7869 7374 730a  ists"] = exists.
+0002bd50: 2020 2020 2020 2020 6966 2069 665f 2069          if if_ i
+0002bd60: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002bd70: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
+0002bd80: 6c75 6573 5b22 6966 5f22 5d20 3d20 6966  lues["if_"] = if
+0002bd90: 5f0a 2020 2020 2020 2020 6966 2076 6172  _.        if var
+0002bda0: 6961 626c 6573 2069 7320 6e6f 7420 4e6f  iables is not No
+0002bdb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002bdc0: 7365 6c66 2e5f 7661 6c75 6573 5b22 7661  self._values["va
+0002bdd0: 7269 6162 6c65 7322 5d20 3d20 7661 7269  riables"] = vari
+0002bde0: 6162 6c65 730a 2020 2020 2020 2020 6966  ables.        if
+0002bdf0: 2077 6865 6e20 6973 206e 6f74 204e 6f6e   when is not Non
+0002be00: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002be10: 656c 662e 5f76 616c 7565 735b 2277 6865  elf._values["whe
+0002be20: 6e22 5d20 3d20 7768 656e 0a0a 2020 2020  n"] = when..    
+0002be30: 4062 7569 6c74 696e 732e 7072 6f70 6572  @builtins.proper
+0002be40: 7479 0a20 2020 2064 6566 2063 6861 6e67  ty.    def chang
+0002be50: 6573 2873 656c 6629 202d 3e20 7479 7069  es(self) -> typi
+0002be60: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
+0002be70: 6e67 2e4c 6973 745b 6275 696c 7469 6e73  ng.List[builtins
+0002be80: 2e73 7472 5d5d 3a0a 2020 2020 2020 2020  .str]]:.        
+0002be90: 2727 270a 2020 2020 2020 2020 3a73 7461  '''.        :sta
+0002bea0: 6269 6c69 7479 3a20 6578 7065 7269 6d65  bility: experime
+0002beb0: 6e74 616c 0a20 2020 2020 2020 2027 2727  ntal.        '''
+0002bec0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0002bed0: 3d20 7365 6c66 2e5f 7661 6c75 6573 2e67  = self._values.g
+0002bee0: 6574 2822 6368 616e 6765 7322 290a 2020  et("changes").  
+0002bef0: 2020 2020 2020 7265 7475 726e 2074 7970        return typ
+0002bf00: 696e 672e 6361 7374 2874 7970 696e 672e  ing.cast(typing.
+0002bf10: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+0002bf20: 4c69 7374 5b62 7569 6c74 696e 732e 7374  List[builtins.st
+0002bf30: 725d 5d2c 2072 6573 756c 7429 0a0a 2020  r]], result)..  
+0002bf40: 2020 4062 7569 6c74 696e 732e 7072 6f70    @builtins.prop
+0002bf50: 6572 7479 0a20 2020 2064 6566 2065 7869  erty.    def exi
+0002bf60: 7374 7328 7365 6c66 2920 2d3e 2074 7970  sts(self) -> typ
+0002bf70: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0002bf80: 696e 672e 4c69 7374 5b62 7569 6c74 696e  ing.List[builtin
+0002bf90: 732e 7374 725d 5d3a 0a20 2020 2020 2020  s.str]]:.       
+0002bfa0: 2027 2727 0a20 2020 2020 2020 203a 7374   '''.        :st
+0002bfb0: 6162 696c 6974 793a 2065 7870 6572 696d  ability: experim
+0002bfc0: 656e 7461 6c0a 2020 2020 2020 2020 2727  ental.        ''
+0002bfd0: 270a 2020 2020 2020 2020 7265 7375 6c74  '.        result
+0002bfe0: 203d 2073 656c 662e 5f76 616c 7565 732e   = self._values.
+0002bff0: 6765 7428 2265 7869 7374 7322 290a 2020  get("exists").  
+0002c000: 2020 2020 2020 7265 7475 726e 2074 7970        return typ
+0002c010: 696e 672e 6361 7374 2874 7970 696e 672e  ing.cast(typing.
+0002c020: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+0002c030: 4c69 7374 5b62 7569 6c74 696e 732e 7374  List[builtins.st
+0002c040: 725d 5d2c 2072 6573 756c 7429 0a0a 2020  r]], result)..  
+0002c050: 2020 4062 7569 6c74 696e 732e 7072 6f70    @builtins.prop
+0002c060: 6572 7479 0a20 2020 2064 6566 2069 665f  erty.    def if_
+0002c070: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
+0002c080: 2e4f 7074 696f 6e61 6c5b 6275 696c 7469  .Optional[builti
+0002c090: 6e73 2e73 7472 5d3a 0a20 2020 2020 2020  ns.str]:.       
+0002c0a0: 2027 2727 0a20 2020 2020 2020 203a 7374   '''.        :st
+0002c0b0: 6162 696c 6974 793a 2065 7870 6572 696d  ability: experim
+0002c0c0: 656e 7461 6c0a 2020 2020 2020 2020 2727  ental.        ''
+0002c0d0: 270a 2020 2020 2020 2020 7265 7375 6c74  '.        result
+0002c0e0: 203d 2073 656c 662e 5f76 616c 7565 732e   = self._values.
+0002c0f0: 6765 7428 2269 665f 2229 0a20 2020 2020  get("if_").     
+0002c100: 2020 2072 6574 7572 6e20 7479 7069 6e67     return typing
+0002c110: 2e63 6173 7428 7479 7069 6e67 2e4f 7074  .cast(typing.Opt
+0002c120: 696f 6e61 6c5b 6275 696c 7469 6e73 2e73  ional[builtins.s
+0002c130: 7472 5d2c 2072 6573 756c 7429 0a0a 2020  tr], result)..  
+0002c140: 2020 4062 7569 6c74 696e 732e 7072 6f70    @builtins.prop
+0002c150: 6572 7479 0a20 2020 2064 6566 2076 6172  erty.    def var
+0002c160: 6961 626c 6573 280a 2020 2020 2020 2020  iables(.        
+0002c170: 7365 6c66 2c0a 2020 2020 2920 2d3e 2074  self,.    ) -> t
+0002c180: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+0002c190: 7970 696e 672e 4d61 7070 696e 675b 6275  yping.Mapping[bu
+0002c1a0: 696c 7469 6e73 2e73 7472 2c20 7479 7069  iltins.str, typi
+0002c1b0: 6e67 2e55 6e69 6f6e 5b62 7569 6c74 696e  ng.Union[builtin
+0002c1c0: 732e 7374 722c 206a 7369 692e 4e75 6d62  s.str, jsii.Numb
+0002c1d0: 6572 5d5d 5d3a 0a20 2020 2020 2020 2027  er]]]:.        '
+0002c1e0: 2727 0a20 2020 2020 2020 203a 7374 6162  ''.        :stab
+0002c1f0: 696c 6974 793a 2065 7870 6572 696d 656e  ility: experimen
+0002c200: 7461 6c0a 2020 2020 2020 2020 2727 270a  tal.        '''.
+0002c210: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0002c220: 2073 656c 662e 5f76 616c 7565 732e 6765   self._values.ge
+0002c230: 7428 2276 6172 6961 626c 6573 2229 0a20  t("variables"). 
+0002c240: 2020 2020 2020 2072 6574 7572 6e20 7479         return ty
+0002c250: 7069 6e67 2e63 6173 7428 7479 7069 6e67  ping.cast(typing
+0002c260: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0002c270: 2e4d 6170 7069 6e67 5b62 7569 6c74 696e  .Mapping[builtin
+0002c280: 732e 7374 722c 2074 7970 696e 672e 556e  s.str, typing.Un
+0002c290: 696f 6e5b 6275 696c 7469 6e73 2e73 7472  ion[builtins.str
+0002c2a0: 2c20 6a73 6969 2e4e 756d 6265 725d 5d5d  , jsii.Number]]]
+0002c2b0: 2c20 7265 7375 6c74 290a 0a20 2020 2040  , result)..    @
+0002c2c0: 6275 696c 7469 6e73 2e70 726f 7065 7274  builtins.propert
+0002c2d0: 790a 2020 2020 6465 6620 7768 656e 2873  y.    def when(s
+0002c2e0: 656c 6629 202d 3e20 7479 7069 6e67 2e4f  elf) -> typing.O
+0002c2f0: 7074 696f 6e61 6c5b 2257 6f72 6b66 6c6f  ptional["Workflo
+0002c300: 7757 6865 6e22 5d3a 0a20 2020 2020 2020  wWhen"]:.       
+0002c310: 2027 2727 0a20 2020 2020 2020 203a 7374   '''.        :st
+0002c320: 6162 696c 6974 793a 2065 7870 6572 696d  ability: experim
+0002c330: 656e 7461 6c0a 2020 2020 2020 2020 2727  ental.        ''
+0002c340: 270a 2020 2020 2020 2020 7265 7375 6c74  '.        result
+0002c350: 203d 2073 656c 662e 5f76 616c 7565 732e   = self._values.
+0002c360: 6765 7428 2277 6865 6e22 290a 2020 2020  get("when").    
+0002c370: 2020 2020 7265 7475 726e 2074 7970 696e      return typin
+0002c380: 672e 6361 7374 2874 7970 696e 672e 4f70  g.cast(typing.Op
+0002c390: 7469 6f6e 616c 5b22 576f 726b 666c 6f77  tional["Workflow
+0002c3a0: 5768 656e 225d 2c20 7265 7375 6c74 290a  When"], result).
+0002c3b0: 0a20 2020 2064 6566 205f 5f65 715f 5f28  .    def __eq__(
+0002c3c0: 7365 6c66 2c20 7268 733a 2074 7970 696e  self, rhs: typin
+0002c3d0: 672e 416e 7929 202d 3e20 6275 696c 7469  g.Any) -> builti
+0002c3e0: 6e73 2e62 6f6f 6c3a 0a20 2020 2020 2020  ns.bool:.       
+0002c3f0: 2072 6574 7572 6e20 6973 696e 7374 616e   return isinstan
+0002c400: 6365 2872 6873 2c20 7365 6c66 2e5f 5f63  ce(rhs, self.__c
+0002c410: 6c61 7373 5f5f 2920 616e 6420 7268 732e  lass__) and rhs.
+0002c420: 5f76 616c 7565 7320 3d3d 2073 656c 662e  _values == self.
+0002c430: 5f76 616c 7565 730a 0a20 2020 2064 6566  _values..    def
+0002c440: 205f 5f6e 655f 5f28 7365 6c66 2c20 7268   __ne__(self, rh
+0002c450: 733a 2074 7970 696e 672e 416e 7929 202d  s: typing.Any) -
+0002c460: 3e20 6275 696c 7469 6e73 2e62 6f6f 6c3a  > builtins.bool:
+0002c470: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002c480: 6e6f 7420 2872 6873 203d 3d20 7365 6c66  not (rhs == self
+0002c490: 290a 0a20 2020 2064 6566 205f 5f72 6570  )..    def __rep
+0002c4a0: 725f 5f28 7365 6c66 2920 2d3e 2073 7472  r__(self) -> str
+0002c4b0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0002c4c0: 2022 576f 726b 666c 6f77 5275 6c65 2825   "WorkflowRule(%
+0002c4d0: 7329 2220 2520 222c 2022 2e6a 6f69 6e28  s)" % ", ".join(
+0002c4e0: 0a20 2020 2020 2020 2020 2020 206b 202b  .            k +
+0002c4f0: 2022 3d22 202b 2072 6570 7228 7629 2066   "=" + repr(v) f
+0002c500: 6f72 206b 2c20 7620 696e 2073 656c 662e  or k, v in self.
+0002c510: 5f76 616c 7565 732e 6974 656d 7328 290a  _values.items().
+0002c520: 2020 2020 2020 2020 290a 0a0a 406a 7369          )...@jsi
+0002c530: 692e 656e 756d 286a 7369 695f 7479 7065  i.enum(jsii_type
+0002c540: 3d22 7072 6f6a 656e 2e67 6974 6c61 622e  ="projen.gitlab.
+0002c550: 576f 726b 666c 6f77 5768 656e 2229 0a63  WorkflowWhen").c
+0002c560: 6c61 7373 2057 6f72 6b66 6c6f 7757 6865  lass WorkflowWhe
+0002c570: 6e28 656e 756d 2e45 6e75 6d29 3a0a 2020  n(enum.Enum):.  
+0002c580: 2020 2727 2728 6578 7065 7269 6d65 6e74    '''(experiment
+0002c590: 616c 2920 4465 7363 7269 6265 7320 7468  al) Describes th
+0002c5a0: 6520 636f 6e64 6974 696f 6e73 2066 6f72  e conditions for
+0002c5b0: 2077 6865 6e20 746f 2072 756e 2074 6865   when to run the
+0002c5c0: 206a 6f62 2e0a 0a20 2020 2044 6566 6175   job...    Defau
+0002c5d0: 6c74 7320 746f 2027 6f6e 5f73 7563 6365  lts to 'on_succe
+0002c5e0: 7373 272e 0a20 2020 2054 6865 2076 616c  ss'..    The val
+0002c5f0: 7565 2063 616e 206f 6e6c 7920 6265 2027  ue can only be '
+0002c600: 616c 7761 7973 2720 6f72 2027 6e65 7665  always' or 'neve
+0002c610: 7227 2077 6865 6e20 7573 6564 2077 6974  r' when used wit
+0002c620: 6820 776f 726b 666c 6f77 2e0a 0a20 2020  h workflow...   
+0002c630: 203a 7365 653a 2068 7474 7073 3a2f 2f64   :see: https://d
+0002c640: 6f63 732e 6769 746c 6162 2e63 6f6d 2f65  ocs.gitlab.com/e
+0002c650: 652f 6369 2f79 616d 6c2f 2377 6f72 6b66  e/ci/yaml/#workf
+0002c660: 6c6f 7772 756c 6573 0a20 2020 203a 7374  lowrules.    :st
+0002c670: 6162 696c 6974 793a 2065 7870 6572 696d  ability: experim
+0002c680: 656e 7461 6c0a 2020 2020 2727 270a 0a20  ental.    '''.. 
+0002c690: 2020 2041 4c57 4159 5320 3d20 2241 4c57     ALWAYS = "ALW
+0002c6a0: 4159 5322 0a20 2020 2027 2727 0a20 2020  AYS".    '''.   
+0002c6b0: 203a 7374 6162 696c 6974 793a 2065 7870   :stability: exp
+0002c6c0: 6572 696d 656e 7461 6c0a 2020 2020 2727  erimental.    ''
+0002c6d0: 270a 2020 2020 4e45 5645 5220 3d20 224e  '.    NEVER = "N
+0002c6e0: 4556 4552 220a 2020 2020 2727 270a 2020  EVER".    '''.  
+0002c6f0: 2020 3a73 7461 6269 6c69 7479 3a20 6578    :stability: ex
+0002c700: 7065 7269 6d65 6e74 616c 0a20 2020 2027  perimental.    '
+0002c710: 2727 0a0a 0a5f 5f61 6c6c 5f5f 203d 205b  ''...__all__ = [
+0002c720: 0a20 2020 2022 4163 7469 6f6e 222c 0a20  .    "Action",. 
+0002c730: 2020 2022 416c 6c6f 7746 6169 6c75 7265     "AllowFailure
+0002c740: 222c 0a20 2020 2022 4172 7469 6661 6374  ",.    "Artifact
+0002c750: 7322 2c0a 2020 2020 2241 7373 6574 7322  s",.    "Assets"
+0002c760: 2c0a 2020 2020 2243 6163 6865 222c 0a20  ,.    "Cache",. 
+0002c770: 2020 2022 4361 6368 654b 6579 4669 6c65     "CacheKeyFile
+0002c780: 7322 2c0a 2020 2020 2243 6163 6865 506f  s",.    "CachePo
+0002c790: 6c69 6379 222c 0a20 2020 2022 4361 6368  licy",.    "Cach
+0002c7a0: 6557 6865 6e22 2c0a 2020 2020 2243 6943  eWhen",.    "CiC
+0002c7b0: 6f6e 6669 6775 7261 7469 6f6e 222c 0a20  onfiguration",. 
+0002c7c0: 2020 2022 4369 436f 6e66 6967 7572 6174     "CiConfigurat
+0002c7d0: 696f 6e4f 7074 696f 6e73 222c 0a20 2020  ionOptions",.   
+0002c7e0: 2022 436f 7665 7261 6765 5265 706f 7274   "CoverageReport
+0002c7f0: 222c 0a20 2020 2022 4465 6661 756c 7422  ",.    "Default"
+0002c800: 2c0a 2020 2020 2244 6566 6175 6c74 456c  ,.    "DefaultEl
+0002c810: 656d 656e 7422 2c0a 2020 2020 2244 6570  ement",.    "Dep
+0002c820: 6c6f 796d 656e 7454 6965 7222 2c0a 2020  loymentTier",.  
+0002c830: 2020 2245 6e67 696e 6522 2c0a 2020 2020    "Engine",.    
+0002c840: 2245 6e76 6972 6f6e 6d65 6e74 222c 0a20  "Environment",. 
+0002c850: 2020 2022 4669 6c74 6572 222c 0a20 2020     "Filter",.   
+0002c860: 2022 4769 746c 6162 436f 6e66 6967 7572   "GitlabConfigur
+0002c870: 6174 696f 6e22 2c0a 2020 2020 2249 4454  ation",.    "IDT
+0002c880: 6f6b 656e 222c 0a20 2020 2022 496d 6167  oken",.    "Imag
+0002c890: 6522 2c0a 2020 2020 2249 6e63 6c75 6465  e",.    "Include
+0002c8a0: 222c 0a20 2020 2022 496e 636c 7564 6552  ",.    "IncludeR
+0002c8b0: 756c 6522 2c0a 2020 2020 2249 6e68 6572  ule",.    "Inher
+0002c8c0: 6974 222c 0a20 2020 2022 4a6f 6222 2c0a  it",.    "Job",.
+0002c8d0: 2020 2020 224a 6f62 5768 656e 222c 0a20      "JobWhen",. 
+0002c8e0: 2020 2022 4b75 6265 726e 6574 6573 436f     "KubernetesCo
+0002c8f0: 6e66 6967 222c 0a20 2020 2022 4b75 6265  nfig",.    "Kube
+0002c900: 726e 6574 6573 456e 756d 222c 0a20 2020  rnetesEnum",.   
+0002c910: 2022 4c69 6e6b 222c 0a20 2020 2022 4c69   "Link",.    "Li
+0002c920: 6e6b 5479 7065 222c 0a20 2020 2022 4e65  nkType",.    "Ne
+0002c930: 6564 222c 0a20 2020 2022 4e65 7374 6564  ed",.    "Nested
+0002c940: 436f 6e66 6967 7572 6174 696f 6e22 2c0a  Configuration",.
+0002c950: 2020 2020 2250 6172 616c 6c65 6c22 2c0a      "Parallel",.
+0002c960: 2020 2020 2250 756c 6c50 6f6c 6963 7922      "PullPolicy"
+0002c970: 2c0a 2020 2020 2252 656c 6561 7365 222c  ,.    "Release",
+0002c980: 0a20 2020 2022 5265 706f 7274 7322 2c0a  .    "Reports",.
+0002c990: 2020 2020 2252 6574 7279 222c 0a20 2020      "Retry",.   
+0002c9a0: 2022 5365 6372 6574 222c 0a20 2020 2022   "Secret",.    "
+0002c9b0: 5365 7276 6963 6522 2c0a 2020 2020 2253  Service",.    "S
+0002c9c0: 7472 6174 6567 7922 2c0a 2020 2020 2254  trategy",.    "T
+0002c9d0: 7269 6767 6572 222c 0a20 2020 2022 5472  rigger",.    "Tr
+0002c9e0: 6967 6765 7249 6e63 6c75 6465 222c 0a20  iggerInclude",. 
+0002c9f0: 2020 2022 5661 7269 6162 6c65 436f 6e66     "VariableConf
+0002ca00: 6967 222c 0a20 2020 2022 5661 756c 7443  ig",.    "VaultC
+0002ca10: 6f6e 6669 6722 2c0a 2020 2020 2257 6f72  onfig",.    "Wor
+0002ca20: 6b66 6c6f 7722 2c0a 2020 2020 2257 6f72  kflow",.    "Wor
+0002ca30: 6b66 6c6f 7752 756c 6522 2c0a 2020 2020  kflowRule",.    
+0002ca40: 2257 6f72 6b66 6c6f 7757 6865 6e22 2c0a  "WorkflowWhen",.
+0002ca50: 5d0a 0a70 7562 6c69 6361 7469 6f6e 2e70  ]..publication.p
+0002ca60: 7562 6c69 7368 2829 0a0a 6465 6620 5f74  ublish()..def _t
+0002ca70: 7970 6563 6865 636b 696e 6773 7475 625f  ypecheckingstub_
+0002ca80: 5f33 3366 3263 3330 6364 6531 6165 6261  _33f2c30cde1aeba
+0002ca90: 6138 3364 6530 3937 3234 3337 3137 6164  a83de097243717ad
+0002caa0: 3864 6436 6431 6332 3631 3762 3437 6134  8dd6d1c2617b47a4
+0002cab0: 3335 3263 6265 3765 3366 3335 3165 3862  352cbe7e3f351e8b
+0002cac0: 3228 0a20 2020 202a 2c0a 2020 2020 6578  2(.    *,.    ex
+0002cad0: 6974 5f63 6f64 6573 3a20 7479 7069 6e67  it_codes: typing
+0002cae0: 2e55 6e69 6f6e 5b6a 7369 692e 4e75 6d62  .Union[jsii.Numb
+0002caf0: 6572 2c20 7479 7069 6e67 2e53 6571 7565  er, typing.Seque
+0002cb00: 6e63 655b 6a73 6969 2e4e 756d 6265 725d  nce[jsii.Number]
+0002cb10: 5d2c 0a29 202d 3e20 4e6f 6e65 3a0a 2020  ],.) -> None:.  
+0002cb20: 2020 2222 2254 7970 6520 6368 6563 6b69    """Type checki
+0002cb30: 6e67 2073 7475 6273 2222 220a 2020 2020  ng stubs""".    
+0002cb40: 7061 7373 0a0a 6465 6620 5f74 7970 6563  pass..def _typec
+0002cb50: 6865 636b 696e 6773 7475 625f 5f31 3664  heckingstub__16d
+0002cb60: 3834 6336 3839 3130 6666 3064 3261 6631  84c68910ff0d2af1
+0002cb70: 3862 6535 3334 3931 6635 6362 6664 3062  8be53491f5cbfd0b
+0002cb80: 6538 3836 3438 6163 6532 6463 6531 3063  e88648ace2dce10c
+0002cb90: 3335 6335 3130 6434 3938 6163 6328 0a20  35c510d498acc(. 
+0002cba0: 2020 202a 2c0a 2020 2020 6578 636c 7564     *,.    exclud
+0002cbb0: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
+0002cbc0: 616c 5b74 7970 696e 672e 5365 7175 656e  al[typing.Sequen
+0002cbd0: 6365 5b62 7569 6c74 696e 732e 7374 725d  ce[builtins.str]
+0002cbe0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6578  ] = None,.    ex
+0002cbf0: 7069 7265 5f69 6e3a 2074 7970 696e 672e  pire_in: typing.
+0002cc00: 4f70 7469 6f6e 616c 5b62 7569 6c74 696e  Optional[builtin
+0002cc10: 732e 7374 725d 203d 204e 6f6e 652c 0a20  s.str] = None,. 
+0002cc20: 2020 2065 7870 6f73 655f 6173 3a20 7479     expose_as: ty
+0002cc30: 7069 6e67 2e4f 7074 696f 6e61 6c5b 6275  ping.Optional[bu
+0002cc40: 696c 7469 6e73 2e73 7472 5d20 3d20 4e6f  iltins.str] = No
+0002cc50: 6e65 2c0a 2020 2020 6e61 6d65 3a20 7479  ne,.    name: ty
+0002cc60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 6275  ping.Optional[bu
+0002cc70: 696c 7469 6e73 2e73 7472 5d20 3d20 4e6f  iltins.str] = No
+0002cc80: 6e65 2c0a 2020 2020 7061 7468 733a 2074  ne,.    paths: t
+0002cc90: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+0002cca0: 7970 696e 672e 5365 7175 656e 6365 5b62  yping.Sequence[b
+0002ccb0: 7569 6c74 696e 732e 7374 725d 5d20 3d20  uiltins.str]] = 
+0002ccc0: 4e6f 6e65 2c0a 2020 2020 7265 706f 7274  None,.    report
+0002ccd0: 733a 2074 7970 696e 672e 4f70 7469 6f6e  s: typing.Option
+0002cce0: 616c 5b74 7970 696e 672e 556e 696f 6e5b  al[typing.Union[
+0002ccf0: 5265 706f 7274 732c 2074 7970 696e 672e  Reports, typing.
+0002cd00: 4469 6374 5b62 7569 6c74 696e 732e 7374  Dict[builtins.st
+0002cd10: 722c 2074 7970 696e 672e 416e 795d 5d5d  r, typing.Any]]]
+0002cd20: 203d 204e 6f6e 652c 0a20 2020 2075 6e74   = None,.    unt
+0002cd30: 7261 636b 6564 3a20 7479 7069 6e67 2e4f  racked: typing.O
+0002cd40: 7074 696f 6e61 6c5b 6275 696c 7469 6e73  ptional[builtins
+0002cd50: 2e62 6f6f 6c5d 203d 204e 6f6e 652c 0a20  .bool] = None,. 
+0002cd60: 2020 2077 6865 6e3a 2074 7970 696e 672e     when: typing.
+0002cd70: 4f70 7469 6f6e 616c 5b43 6163 6865 5768  Optional[CacheWh
+0002cd80: 656e 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e  en] = None,.) ->
+0002cd90: 204e 6f6e 653a 0a20 2020 2022 2222 5479   None:.    """Ty
+0002cda0: 7065 2063 6865 636b 696e 6720 7374 7562  pe checking stub
+0002cdb0: 7322 2222 0a20 2020 2070 6173 730a 0a64  s""".    pass..d
+0002cdc0: 6566 205f 7479 7065 6368 6563 6b69 6e67  ef _typechecking
+0002cdd0: 7374 7562 5f5f 3861 6431 3563 3837 3066  stub__8ad15c870f
+0002cde0: 6534 3932 3838 6264 6131 6139 3865 3162  e49288bda1a98e1b
+0002cdf0: 6663 3964 6235 6638 3632 3238 3964 6532  fc9db5f862289de2
+0002ce00: 6164 3561 6436 3265 3463 3539 6365 3461  ad5ad62e4c59ce4a
+0002ce10: 6162 3463 3733 280a 2020 2020 2a2c 0a20  ab4c73(.    *,. 
+0002ce20: 2020 206c 696e 6b73 3a20 7479 7069 6e67     links: typing
+0002ce30: 2e53 6571 7565 6e63 655b 7479 7069 6e67  .Sequence[typing
+0002ce40: 2e55 6e69 6f6e 5b4c 696e 6b2c 2074 7970  .Union[Link, typ
+0002ce50: 696e 672e 4469 6374 5b62 7569 6c74 696e  ing.Dict[builtin
+0002ce60: 732e 7374 722c 2074 7970 696e 672e 416e  s.str, typing.An
+0002ce70: 795d 5d5d 2c0a 2920 2d3e 204e 6f6e 653a  y]]],.) -> None:
+0002ce80: 0a20 2020 2022 2222 5479 7065 2063 6865  .    """Type che
+0002ce90: 636b 696e 6720 7374 7562 7322 2222 0a20  cking stubs""". 
+0002cea0: 2020 2070 6173 730a 0a64 6566 205f 7479     pass..def _ty
+0002ceb0: 7065 6368 6563 6b69 6e67 7374 7562 5f5f  pecheckingstub__
+0002cec0: 6237 6630 3439 3638 3164 6633 6463 6366  b7f049681df3dccf
+0002ced0: 3335 3635 3338 3433 6335 3434 6530 3632  35653843c544e062
+0002cee0: 3538 3237 3135 3230 6462 3132 3439 3365  58271520db12493e
+0002cef0: 3438 6163 3933 3661 3936 6563 6564 6164  48ac936a96ecedad
+0002cf00: 280a 2020 2020 2a2c 0a20 2020 2066 616c  (.    *,.    fal
+0002cf10: 6c62 6163 6b5f 6b65 7973 3a20 7479 7069  lback_keys: typi
+0002cf20: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
+0002cf30: 6e67 2e53 6571 7565 6e63 655b 6275 696c  ng.Sequence[buil
+0002cf40: 7469 6e73 2e73 7472 5d5d 203d 204e 6f6e  tins.str]] = Non
+0002cf50: 652c 0a20 2020 206b 6579 3a20 7479 7069  e,.    key: typi
+0002cf60: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
+0002cf70: 6e67 2e55 6e69 6f6e 5b62 7569 6c74 696e  ng.Union[builtin
+0002cf80: 732e 7374 722c 2074 7970 696e 672e 556e  s.str, typing.Un
+0002cf90: 696f 6e5b 4361 6368 654b 6579 4669 6c65  ion[CacheKeyFile
+0002cfa0: 732c 2074 7970 696e 672e 4469 6374 5b62  s, typing.Dict[b
+0002cfb0: 7569 6c74 696e 732e 7374 722c 2074 7970  uiltins.str, typ
+0002cfc0: 696e 672e 416e 795d 5d5d 5d20 3d20 4e6f  ing.Any]]]] = No
+0002cfd0: 6e65 2c0a 2020 2020 7061 7468 733a 2074  ne,.    paths: t
+0002cfe0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+0002cff0: 7970 696e 672e 5365 7175 656e 6365 5b62  yping.Sequence[b
+0002d000: 7569 6c74 696e 732e 7374 725d 5d20 3d20  uiltins.str]] = 
+0002d010: 4e6f 6e65 2c0a 2020 2020 706f 6c69 6379  None,.    policy
+0002d020: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+0002d030: 6c5b 4361 6368 6550 6f6c 6963 795d 203d  l[CachePolicy] =
+0002d040: 204e 6f6e 652c 0a20 2020 2075 6e74 7261   None,.    untra
+0002d050: 636b 6564 3a20 7479 7069 6e67 2e4f 7074  cked: typing.Opt
+0002d060: 696f 6e61 6c5b 6275 696c 7469 6e73 2e62  ional[builtins.b
+0002d070: 6f6f 6c5d 203d 204e 6f6e 652c 0a20 2020  ool] = None,.   
+0002d080: 2077 6865 6e3a 2074 7970 696e 672e 4f70   when: typing.Op
+0002d090: 7469 6f6e 616c 5b43 6163 6865 5768 656e  tional[CacheWhen
+0002d0a0: 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e 204e  ] = None,.) -> N
+0002d0b0: 6f6e 653a 0a20 2020 2022 2222 5479 7065  one:.    """Type
+0002d0c0: 2063 6865 636b 696e 6720 7374 7562 7322   checking stubs"
+0002d0d0: 2222 0a20 2020 2070 6173 730a 0a64 6566  "".    pass..def
+0002d0e0: 205f 7479 7065 6368 6563 6b69 6e67 7374   _typecheckingst
+0002d0f0: 7562 5f5f 6538 6661 3736 6263 3165 3232  ub__e8fa76bc1e22
+0002d100: 3533 6664 3935 6466 3831 6662 3762 3933  53fd95df81fb7b93
+0002d110: 3938 3230 3531 6232 3430 6365 6139 3365  982051b240cea93e
+0002d120: 6164 3532 6439 6439 3535 3335 6565 6236  ad52d9d95535eeb6
+0002d130: 6637 3630 280a 2020 2020 2a2c 0a20 2020  f760(.    *,.   
+0002d140: 2066 696c 6573 3a20 7479 7069 6e67 2e53   files: typing.S
+0002d150: 6571 7565 6e63 655b 6275 696c 7469 6e73  equence[builtins
+0002d160: 2e73 7472 5d2c 0a20 2020 2070 7265 6669  .str],.    prefi
+0002d170: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
+0002d180: 616c 5b62 7569 6c74 696e 732e 7374 725d  al[builtins.str]
+0002d190: 203d 204e 6f6e 652c 0a29 202d 3e20 4e6f   = None,.) -> No
+0002d1a0: 6e65 3a0a 2020 2020 2222 2254 7970 6520  ne:.    """Type 
+0002d1b0: 6368 6563 6b69 6e67 2073 7475 6273 2222  checking stubs""
+0002d1c0: 220a 2020 2020 7061 7373 0a0a 6465 6620  ".    pass..def 
+0002d1d0: 5f74 7970 6563 6865 636b 696e 6773 7475  _typecheckingstu
+0002d1e0: 625f 5f32 3331 6333 3062 6335 3133 6638  b__231c30bc513f8
+0002d1f0: 6530 3965 3334 3564 6436 3333 3932 6537  e09e345dd63392e7
+0002d200: 6335 3066 3437 3964 6639 6634 3830 6663  c50f479df9f480fc
+0002d210: 3336 6530 3365 3838 6663 3461 3565 3863  36e03e88fc4a5e8c
+0002d220: 6436 3828 0a20 2020 2070 726f 6a65 6374  d68(.    project
+0002d230: 3a20 5f50 726f 6a65 6374 5f35 3764 3839  : _Project_57d89
+0002d240: 3230 332c 0a20 2020 206e 616d 653a 2062  203,.    name: b
+0002d250: 7569 6c74 696e 732e 7374 722c 0a20 2020  uiltins.str,.   
+0002d260: 202a 2c0a 2020 2020 6465 6661 756c 743a   *,.    default:
+0002d270: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0002d280: 5b74 7970 696e 672e 556e 696f 6e5b 4465  [typing.Union[De
+0002d290: 6661 756c 742c 2074 7970 696e 672e 4469  fault, typing.Di
+0002d2a0: 6374 5b62 7569 6c74 696e 732e 7374 722c  ct[builtins.str,
+0002d2b0: 2074 7970 696e 672e 416e 795d 5d5d 203d   typing.Any]]] =
+0002d2c0: 204e 6f6e 652c 0a20 2020 206a 6f62 733a   None,.    jobs:
+0002d2d0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0002d2e0: 5b74 7970 696e 672e 4d61 7070 696e 675b  [typing.Mapping[
+0002d2f0: 6275 696c 7469 6e73 2e73 7472 2c20 7479  builtins.str, ty
+0002d300: 7069 6e67 2e55 6e69 6f6e 5b4a 6f62 2c20  ping.Union[Job, 
+0002d310: 7479 7069 6e67 2e44 6963 745b 6275 696c  typing.Dict[buil
+0002d320: 7469 6e73 2e73 7472 2c20 7479 7069 6e67  tins.str, typing
+0002d330: 2e41 6e79 5d5d 5d5d 203d 204e 6f6e 652c  .Any]]]] = None,
+0002d340: 0a20 2020 2070 6167 6573 3a20 7479 7069  .    pages: typi
+0002d350: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
+0002d360: 6e67 2e55 6e69 6f6e 5b4a 6f62 2c20 7479  ng.Union[Job, ty
+0002d370: 7069 6e67 2e44 6963 745b 6275 696c 7469  ping.Dict[builti
+0002d380: 6e73 2e73 7472 2c20 7479 7069 6e67 2e41  ns.str, typing.A
+0002d390: 6e79 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020  ny]]] = None,.  
+0002d3a0: 2020 7374 6167 6573 3a20 7479 7069 6e67    stages: typing
+0002d3b0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0002d3c0: 2e53 6571 7565 6e63 655b 6275 696c 7469  .Sequence[builti
+0002d3d0: 6e73 2e73 7472 5d5d 203d 204e 6f6e 652c  ns.str]] = None,
+0002d3e0: 0a20 2020 2076 6172 6961 626c 6573 3a20  .    variables: 
+0002d3f0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0002d400: 7479 7069 6e67 2e4d 6170 7069 6e67 5b62  typing.Mapping[b
+0002d410: 7569 6c74 696e 732e 7374 722c 2074 7970  uiltins.str, typ
+0002d420: 696e 672e 416e 795d 5d20 3d20 4e6f 6e65  ing.Any]] = None
+0002d430: 2c0a 2020 2020 776f 726b 666c 6f77 3a20  ,.    workflow: 
+0002d440: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0002d450: 7479 7069 6e67 2e55 6e69 6f6e 5b57 6f72  typing.Union[Wor
+0002d460: 6b66 6c6f 772c 2074 7970 696e 672e 4469  kflow, typing.Di
+0002d470: 6374 5b62 7569 6c74 696e 732e 7374 722c  ct[builtins.str,
+0002d480: 2074 7970 696e 672e 416e 795d 5d5d 203d   typing.Any]]] =
+0002d490: 204e 6f6e 652c 0a29 202d 3e20 4e6f 6e65   None,.) -> None
+0002d4a0: 3a0a 2020 2020 2222 2254 7970 6520 6368  :.    """Type ch
+0002d4b0: 6563 6b69 6e67 2073 7475 6273 2222 220a  ecking stubs""".
+0002d4c0: 2020 2020 7061 7373 0a0a 6465 6620 5f74      pass..def _t
+0002d4d0: 7970 6563 6865 636b 696e 6773 7475 625f  ypecheckingstub_
+0002d4e0: 5f62 6338 6463 3833 6636 6564 3263 3339  _bc8dc83f6ed2c39
+0002d4f0: 3237 6561 6334 3538 3933 6338 3633 3035  27eac45893c86305
+0002d500: 3038 3433 6264 6561 3661 3931 3964 6365  0843bdea6a919dce
+0002d510: 6461 3061 6562 3831 3161 6162 3662 3033  da0aeb811aab6b03
+0002d520: 6128 0a20 2020 2063 6163 6865 733a 2074  a(.    caches: t
+0002d530: 7970 696e 672e 5365 7175 656e 6365 5b74  yping.Sequence[t
+0002d540: 7970 696e 672e 556e 696f 6e5b 4361 6368  yping.Union[Cach
+0002d550: 652c 2074 7970 696e 672e 4469 6374 5b62  e, typing.Dict[b
+0002d560: 7569 6c74 696e 732e 7374 722c 2074 7970  uiltins.str, typ
+0002d570: 696e 672e 416e 795d 5d5d 2c0a 2920 2d3e  ing.Any]]],.) ->
+0002d580: 204e 6f6e 653a 0a20 2020 2022 2222 5479   None:.    """Ty
+0002d590: 7065 2063 6865 636b 696e 6720 7374 7562  pe checking stub
+0002d5a0: 7322 2222 0a20 2020 2070 6173 730a 0a64  s""".    pass..d
+0002d5b0: 6566 205f 7479 7065 6368 6563 6b69 6e67  ef _typechecking
+0002d5c0: 7374 7562 5f5f 6135 3332 6239 6433 6265  stub__a532b9d3be
+0002d5d0: 6362 6463 6563 3061 3239 3235 3338 6130  cbdcec0a292538a0
+0002d5e0: 3637 6633 6464 6336 6130 3337 6162 6466  67f3ddc6a037abdf
+0002d5f0: 3532 3335 3030 3438 3564 6335 3330 3431  523500485dc53041
+0002d600: 3832 3563 3033 280a 2020 2020 7661 7269  825c03(.    vari
+0002d610: 6162 6c65 733a 2074 7970 696e 672e 4d61  ables: typing.Ma
+0002d620: 7070 696e 675b 6275 696c 7469 6e73 2e73  pping[builtins.s
+0002d630: 7472 2c20 7479 7069 6e67 2e41 6e79 5d2c  tr, typing.Any],
+0002d640: 0a29 202d 3e20 4e6f 6e65 3a0a 2020 2020  .) -> None:.    
+0002d650: 2222 2254 7970 6520 6368 6563 6b69 6e67  """Type checking
+0002d660: 2073 7475 6273 2222 220a 2020 2020 7061   stubs""".    pa
+0002d670: 7373 0a0a 6465 6620 5f74 7970 6563 6865  ss..def _typeche
+0002d680: 636b 696e 6773 7475 625f 5f39 6263 6133  ckingstub__9bca3
+0002d690: 3138 3961 6435 3362 6234 6132 3635 3961  189ad53bb4a2659a
+0002d6a0: 3363 3462 6537 6332 3333 3738 3864 6664  3c4be7c233788dfd
+0002d6b0: 3064 3664 3065 3332 3235 3565 3532 6436  0d6d0e32255e52d6
+0002d6c0: 6536 6434 3632 3631 6562 6428 0a20 2020  e6d46261ebd(.   
+0002d6d0: 202a 696e 636c 7564 6573 3a20 496e 636c   *includes: Incl
+0002d6e0: 7564 652c 0a29 202d 3e20 4e6f 6e65 3a0a  ude,.) -> None:.
+0002d6f0: 2020 2020 2222 2254 7970 6520 6368 6563      """Type chec
+0002d700: 6b69 6e67 2073 7475 6273 2222 220a 2020  king stubs""".  
+0002d710: 2020 7061 7373 0a0a 6465 6620 5f74 7970    pass..def _typ
+0002d720: 6563 6865 636b 696e 6773 7475 625f 5f66  echeckingstub__f
+0002d730: 3432 3664 6463 3063 3132 3561 6162 6537  426ddc0c125aabe7
+0002d740: 3461 3038 6563 6334 6164 3030 3863 3264  4a08ecc4ad008c2d
+0002d750: 3262 3562 3434 6566 3932 3430 6630 6130  2b5b44ef9240f0a0
+0002d760: 6539 3963 3034 6139 3638 3061 6531 3828  e99c04a9680ae18(
+0002d770: 0a20 2020 206a 6f62 733a 2074 7970 696e  .    jobs: typin
+0002d780: 672e 4d61 7070 696e 675b 6275 696c 7469  g.Mapping[builti
+0002d790: 6e73 2e73 7472 2c20 7479 7069 6e67 2e55  ns.str, typing.U
+0002d7a0: 6e69 6f6e 5b4a 6f62 2c20 7479 7069 6e67  nion[Job, typing
+0002d7b0: 2e44 6963 745b 6275 696c 7469 6e73 2e73  .Dict[builtins.s
+0002d7c0: 7472 2c20 7479 7069 6e67 2e41 6e79 5d5d  tr, typing.Any]]
+0002d7d0: 5d2c 0a29 202d 3e20 4e6f 6e65 3a0a 2020  ],.) -> None:.  
+0002d7e0: 2020 2222 2254 7970 6520 6368 6563 6b69    """Type checki
+0002d7f0: 6e67 2073 7475 6273 2222 220a 2020 2020  ng stubs""".    
+0002d800: 7061 7373 0a0a 6465 6620 5f74 7970 6563  pass..def _typec
+0002d810: 6865 636b 696e 6773 7475 625f 5f65 6538  heckingstub__ee8
+0002d820: 3836 6162 3636 3335 3863 6332 3566 3735  86ab66358cc25f75
+0002d830: 6561 6666 3564 6362 6562 6132 6530 3364  eaff5dcbeba2e03d
+0002d840: 3566 3732 6462 3864 3764 3239 3933 3630  5f72db8d7d299360
+0002d850: 6166 3831 3435 3334 3238 6639 6228 0a20  af81453428f9b(. 
+0002d860: 2020 202a 7365 7276 6963 6573 3a20 5365     *services: Se
+0002d870: 7276 6963 652c 0a29 202d 3e20 4e6f 6e65  rvice,.) -> None
+0002d880: 3a0a 2020 2020 2222 2254 7970 6520 6368  :.    """Type ch
+0002d890: 6563 6b69 6e67 2073 7475 6273 2222 220a  ecking stubs""".
+0002d8a0: 2020 2020 7061 7373 0a0a 6465 6620 5f74      pass..def _t
+0002d8b0: 7970 6563 6865 636b 696e 6773 7475 625f  ypecheckingstub_
+0002d8c0: 5f63 3337 3235 3637 3133 6262 3864 3336  _c37256713bb8d36
+0002d8d0: 3139 3636 6630 6233 3966 3464 6261 3861  1966f0b39f4dba8a
+0002d8e0: 6163 3434 3666 3165 6561 3764 6132 3766  ac446f1eea7da27f
+0002d8f0: 6162 6438 6539 6561 3638 3333 3933 3363  abd8e9ea6833933c
+0002d900: 3628 0a20 2020 202a 7374 6167 6573 3a20  6(.    *stages: 
+0002d910: 6275 696c 7469 6e73 2e73 7472 2c0a 2920  builtins.str,.) 
+0002d920: 2d3e 204e 6f6e 653a 0a20 2020 2022 2222  -> None:.    """
+0002d930: 5479 7065 2063 6865 636b 696e 6720 7374  Type checking st
+0002d940: 7562 7322 2222 0a20 2020 2070 6173 730a  ubs""".    pass.
+0002d950: 0a64 6566 205f 7479 7065 6368 6563 6b69  .def _typechecki
+0002d960: 6e67 7374 7562 5f5f 6361 6436 3230 3464  ngstub__cad6204d
+0002d970: 3934 3432 3161 3234 3933 6534 3463 3631  94421a2493e44c61
+0002d980: 3331 6534 3465 3961 6332 3137 3535 3436  31e44e9ac2175546
+0002d990: 6265 3732 6430 6536 3535 6466 3736 3235  be72d0e655df7625
+0002d9a0: 3230 3637 3363 3965 280a 2020 2020 2a2c  20673c9e(.    *,
+0002d9b0: 0a20 2020 2064 6566 6175 6c74 3a20 7479  .    default: ty
+0002d9c0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+0002d9d0: 7069 6e67 2e55 6e69 6f6e 5b44 6566 6175  ping.Union[Defau
+0002d9e0: 6c74 2c20 7479 7069 6e67 2e44 6963 745b  lt, typing.Dict[
+0002d9f0: 6275 696c 7469 6e73 2e73 7472 2c20 7479  builtins.str, ty
+0002da00: 7069 6e67 2e41 6e79 5d5d 5d20 3d20 4e6f  ping.Any]]] = No
+0002da10: 6e65 2c0a 2020 2020 6a6f 6273 3a20 7479  ne,.    jobs: ty
+0002da20: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+0002da30: 7069 6e67 2e4d 6170 7069 6e67 5b62 7569  ping.Mapping[bui
+0002da40: 6c74 696e 732e 7374 722c 2074 7970 696e  ltins.str, typin
+0002da50: 672e 556e 696f 6e5b 4a6f 622c 2074 7970  g.Union[Job, typ
+0002da60: 696e 672e 4469 6374 5b62 7569 6c74 696e  ing.Dict[builtin
+0002da70: 732e 7374 722c 2074 7970 696e 672e 416e  s.str, typing.An
+0002da80: 795d 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020  y]]]] = None,.  
+0002da90: 2020 7061 6765 733a 2074 7970 696e 672e    pages: typing.
+0002daa0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+0002dab0: 556e 696f 6e5b 4a6f 622c 2074 7970 696e  Union[Job, typin
+0002dac0: 672e 4469 6374 5b62 7569 6c74 696e 732e  g.Dict[builtins.
+0002dad0: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
+0002dae0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2073  ]] = None,.    s
+0002daf0: 7461 6765 733a 2074 7970 696e 672e 4f70  tages: typing.Op
+0002db00: 7469 6f6e 616c 5b74 7970 696e 672e 5365  tional[typing.Se
+0002db10: 7175 656e 6365 5b62 7569 6c74 696e 732e  quence[builtins.
+0002db20: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+0002db30: 2020 7661 7269 6162 6c65 733a 2074 7970    variables: typ
+0002db40: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0002db50: 696e 672e 4d61 7070 696e 675b 6275 696c  ing.Mapping[buil
+0002db60: 7469 6e73 2e73 7472 2c20 7479 7069 6e67  tins.str, typing
+0002db70: 2e41 6e79 5d5d 203d 204e 6f6e 652c 0a20  .Any]] = None,. 
+0002db80: 2020 2077 6f72 6b66 6c6f 773a 2074 7970     workflow: typ
+0002db90: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0002dba0: 696e 672e 556e 696f 6e5b 576f 726b 666c  ing.Union[Workfl
+0002dbb0: 6f77 2c20 7479 7069 6e67 2e44 6963 745b  ow, typing.Dict[
+0002dbc0: 6275 696c 7469 6e73 2e73 7472 2c20 7479  builtins.str, ty
+0002dbd0: 7069 6e67 2e41 6e79 5d5d 5d20 3d20 4e6f  ping.Any]]] = No
+0002dbe0: 6e65 2c0a 2920 2d3e 204e 6f6e 653a 0a20  ne,.) -> None:. 
+0002dbf0: 2020 2022 2222 5479 7065 2063 6865 636b     """Type check
+0002dc00: 696e 6720 7374 7562 7322 2222 0a20 2020  ing stubs""".   
+0002dc10: 2070 6173 730a 0a64 6566 205f 7479 7065   pass..def _type
+0002dc20: 6368 6563 6b69 6e67 7374 7562 5f5f 6334  checkingstub__c4
+0002dc30: 6662 3834 3664 6161 6330 3030 6364 6362  fb846daac000cdcb
+0002dc40: 3633 3734 6163 6437 3065 6263 3733 3233  6374acd70ebc7323
+0002dc50: 6638 3637 3631 6133 3163 3265 6262 3265  f86761a31c2ebb2e
+0002dc60: 6630 6431 6234 3961 3366 3036 3532 280a  f0d1b49a3f0652(.
+0002dc70: 2020 2020 2a2c 0a20 2020 2063 6f76 6572      *,.    cover
+0002dc80: 6167 655f 666f 726d 6174 3a20 6275 696c  age_format: buil
+0002dc90: 7469 6e73 2e73 7472 2c0a 2020 2020 7061  tins.str,.    pa
+0002dca0: 7468 3a20 6275 696c 7469 6e73 2e73 7472  th: builtins.str
+0002dcb0: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
+0002dcc0: 2022 2222 5479 7065 2063 6865 636b 696e   """Type checkin
+0002dcd0: 6720 7374 7562 7322 2222 0a20 2020 2070  g stubs""".    p
+0002dce0: 6173 730a 0a64 6566 205f 7479 7065 6368  ass..def _typech
+0002dcf0: 6563 6b69 6e67 7374 7562 5f5f 6338 6537  eckingstub__c8e7
+0002dd00: 3164 3031 6564 6139 3032 3937 6462 3661  1d01eda90297db6a
+0002dd10: 6636 3735 6635 3130 3333 3431 3435 3436  f675f51033414546
+0002dd20: 3231 3262 3036 6434 3963 3030 6332 3138  212b06d49c00c218
+0002dd30: 6465 6532 3037 3164 3165 6431 280a 2020  dee2071d1ed1(.  
+0002dd40: 2020 2a2c 0a20 2020 2061 6674 6572 5f73    *,.    after_s
+0002dd50: 6372 6970 743a 2074 7970 696e 672e 4f70  cript: typing.Op
+0002dd60: 7469 6f6e 616c 5b74 7970 696e 672e 5365  tional[typing.Se
+0002dd70: 7175 656e 6365 5b62 7569 6c74 696e 732e  quence[builtins.
+0002dd80: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+0002dd90: 2020 6172 7469 6661 6374 733a 2074 7970    artifacts: typ
+0002dda0: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0002ddb0: 696e 672e 556e 696f 6e5b 4172 7469 6661  ing.Union[Artifa
+0002ddc0: 6374 732c 2074 7970 696e 672e 4469 6374  cts, typing.Dict
+0002ddd0: 5b62 7569 6c74 696e 732e 7374 722c 2074  [builtins.str, t
+0002dde0: 7970 696e 672e 416e 795d 5d5d 203d 204e  yping.Any]]] = N
+0002ddf0: 6f6e 652c 0a20 2020 2062 6566 6f72 655f  one,.    before_
+0002de00: 7363 7269 7074 3a20 7479 7069 6e67 2e4f  script: typing.O
+0002de10: 7074 696f 6e61 6c5b 7479 7069 6e67 2e53  ptional[typing.S
+0002de20: 6571 7565 6e63 655b 6275 696c 7469 6e73  equence[builtins
+0002de30: 2e73 7472 5d5d 203d 204e 6f6e 652c 0a20  .str]] = None,. 
+0002de40: 2020 2063 6163 6865 3a20 7479 7069 6e67     cache: typing
+0002de50: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0002de60: 2e53 6571 7565 6e63 655b 7479 7069 6e67  .Sequence[typing
+0002de70: 2e55 6e69 6f6e 5b43 6163 6865 2c20 7479  .Union[Cache, ty
+0002de80: 7069 6e67 2e44 6963 745b 6275 696c 7469  ping.Dict[builti
+0002de90: 6e73 2e73 7472 2c20 7479 7069 6e67 2e41  ns.str, typing.A
+0002dea0: 6e79 5d5d 5d5d 203d 204e 6f6e 652c 0a20  ny]]]] = None,. 
+0002deb0: 2020 2069 6d61 6765 3a20 7479 7069 6e67     image: typing
+0002dec0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0002ded0: 2e55 6e69 6f6e 5b49 6d61 6765 2c20 7479  .Union[Image, ty
+0002dee0: 7069 6e67 2e44 6963 745b 6275 696c 7469  ping.Dict[builti
+0002def0: 6e73 2e73 7472 2c20 7479 7069 6e67 2e41  ns.str, typing.A
+0002df00: 6e79 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020  ny]]] = None,.  
+0002df10: 2020 696e 7465 7272 7570 7469 626c 653a    interruptible:
+0002df20: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0002df30: 5b62 7569 6c74 696e 732e 626f 6f6c 5d20  [builtins.bool] 
+0002df40: 3d20 4e6f 6e65 2c0a 2020 2020 7265 7472  = None,.    retr
+0002df50: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
+0002df60: 616c 5b74 7970 696e 672e 556e 696f 6e5b  al[typing.Union[
+0002df70: 5265 7472 792c 2074 7970 696e 672e 4469  Retry, typing.Di
+0002df80: 6374 5b62 7569 6c74 696e 732e 7374 722c  ct[builtins.str,
+0002df90: 2074 7970 696e 672e 416e 795d 5d5d 203d   typing.Any]]] =
+0002dfa0: 204e 6f6e 652c 0a20 2020 2073 6572 7669   None,.    servi
+0002dfb0: 6365 733a 2074 7970 696e 672e 4f70 7469  ces: typing.Opti
+0002dfc0: 6f6e 616c 5b74 7970 696e 672e 5365 7175  onal[typing.Sequ
+0002dfd0: 656e 6365 5b74 7970 696e 672e 556e 696f  ence[typing.Unio
+0002dfe0: 6e5b 5365 7276 6963 652c 2074 7970 696e  n[Service, typin
+0002dff0: 672e 4469 6374 5b62 7569 6c74 696e 732e  g.Dict[builtins.
+0002e000: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
+0002e010: 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ]]] = None,.    
+0002e020: 7461 6773 3a20 7479 7069 6e67 2e4f 7074  tags: typing.Opt
+0002e030: 696f 6e61 6c5b 7479 7069 6e67 2e53 6571  ional[typing.Seq
+0002e040: 7565 6e63 655b 6275 696c 7469 6e73 2e73  uence[builtins.s
+0002e050: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
+0002e060: 2074 696d 656f 7574 3a20 7479 7069 6e67   timeout: typing
+0002e070: 2e4f 7074 696f 6e61 6c5b 6275 696c 7469  .Optional[builti
+0002e080: 6e73 2e73 7472 5d20 3d20 4e6f 6e65 2c0a  ns.str] = None,.
+0002e090: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
+0002e0a0: 2222 5479 7065 2063 6865 636b 696e 6720  ""Type checking 
+0002e0b0: 7374 7562 7322 2222 0a20 2020 2070 6173  stubs""".    pas
+0002e0c0: 730a 0a64 6566 205f 7479 7065 6368 6563  s..def _typechec
+0002e0d0: 6b69 6e67 7374 7562 5f5f 3435 3734 6465  kingstub__4574de
+0002e0e0: 6235 3063 6639 3031 3965 3131 3363 3637  b50cf9019e113c67
+0002e0f0: 6437 3134 6461 3239 3638 3531 3433 3332  d714da2968514332
+0002e100: 3466 6334 6531 6466 3036 6335 6561 3038  4fc4e1df06c5ea08
+0002e110: 6138 3734 6465 3832 3233 280a 2020 2020  a874de8223(.    
+0002e120: 2a2c 0a20 2020 206e 616d 653a 2062 7569  *,.    name: bui
+0002e130: 6c74 696e 732e 7374 722c 0a20 2020 2070  ltins.str,.    p
+0002e140: 6174 683a 2062 7569 6c74 696e 732e 7374  ath: builtins.st
+0002e150: 722c 0a29 202d 3e20 4e6f 6e65 3a0a 2020  r,.) -> None:.  
+0002e160: 2020 2222 2254 7970 6520 6368 6563 6b69    """Type checki
+0002e170: 6e67 2073 7475 6273 2222 220a 2020 2020  ng stubs""".    
+0002e180: 7061 7373 0a0a 6465 6620 5f74 7970 6563  pass..def _typec
+0002e190: 6865 636b 696e 6773 7475 625f 5f37 6461  heckingstub__7da
+0002e1a0: 6366 3036 3635 3230 6564 6562 6361 6631  cf066520edebcaf1
+0002e1b0: 3931 3463 6638 6234 3761 3533 3964 3332  914cf8b47a539d32
+0002e1c0: 6236 3031 6337 3238 6337 3435 6139 3832  b601c728c745a982
+0002e1d0: 3164 6131 3866 6336 3163 3331 3128 0a20  1da18fc61c311(. 
+0002e1e0: 2020 202a 2c0a 2020 2020 6e61 6d65 3a20     *,.    name: 
+0002e1f0: 6275 696c 7469 6e73 2e73 7472 2c0a 2020  builtins.str,.  
+0002e200: 2020 6163 7469 6f6e 3a20 7479 7069 6e67    action: typing
+0002e210: 2e4f 7074 696f 6e61 6c5b 4163 7469 6f6e  .Optional[Action
+0002e220: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6175  ] = None,.    au
+0002e230: 746f 5f73 746f 705f 696e 3a20 7479 7069  to_stop_in: typi
+0002e240: 6e67 2e4f 7074 696f 6e61 6c5b 6275 696c  ng.Optional[buil
+0002e250: 7469 6e73 2e73 7472 5d20 3d20 4e6f 6e65  tins.str] = None
+0002e260: 2c0a 2020 2020 6465 706c 6f79 6d65 6e74  ,.    deployment
+0002e270: 5f74 6965 723a 2074 7970 696e 672e 4f70  _tier: typing.Op
+0002e280: 7469 6f6e 616c 5b44 6570 6c6f 796d 656e  tional[Deploymen
+0002e290: 7454 6965 725d 203d 204e 6f6e 652c 0a20  tTier] = None,. 
+0002e2a0: 2020 206b 7562 6572 6e65 7465 733a 2074     kubernetes: t
+0002e2b0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+0002e2c0: 7970 696e 672e 556e 696f 6e5b 4b75 6265  yping.Union[Kube
+0002e2d0: 726e 6574 6573 436f 6e66 6967 2c20 7479  rnetesConfig, ty
+0002e2e0: 7069 6e67 2e44 6963 745b 6275 696c 7469  ping.Dict[builti
+0002e2f0: 6e73 2e73 7472 2c20 7479 7069 6e67 2e41  ns.str, typing.A
+0002e300: 6e79 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020  ny]]] = None,.  
+0002e310: 2020 6f6e 5f73 746f 703a 2074 7970 696e    on_stop: typin
+0002e320: 672e 4f70 7469 6f6e 616c 5b62 7569 6c74  g.Optional[built
+0002e330: 696e 732e 7374 725d 203d 204e 6f6e 652c  ins.str] = None,
+0002e340: 0a20 2020 2075 726c 3a20 7479 7069 6e67  .    url: typing
+0002e350: 2e4f 7074 696f 6e61 6c5b 6275 696c 7469  .Optional[builti
+0002e360: 6e73 2e73 7472 5d20 3d20 4e6f 6e65 2c0a  ns.str] = None,.
+0002e370: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
+0002e380: 2222 5479 7065 2063 6865 636b 696e 6720  ""Type checking 
+0002e390: 7374 7562 7322 2222 0a20 2020 2070 6173  stubs""".    pas
+0002e3a0: 730a 0a64 6566 205f 7479 7065 6368 6563  s..def _typechec
+0002e3b0: 6b69 6e67 7374 7562 5f5f 6462 3839 3565  kingstub__db895e
+0002e3c0: 3637 3238 3837 3664 6535 6265 3735 3632  6728876de5be7562
+0002e3d0: 3564 6638 6265 3934 6138 6338 3638 3436  5df8be94a8c86846
+0002e3e0: 3332 3762 3234 3433 6666 3166 6437 6338  327b2443ff1fd7c8
+0002e3f0: 6330 3964 6334 6436 6632 280a 2020 2020  c09dc4d6f2(.    
+0002e400: 2a2c 0a20 2020 2063 6861 6e67 6573 3a20  *,.    changes: 
+0002e410: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0002e420: 7479 7069 6e67 2e53 6571 7565 6e63 655b  typing.Sequence[
+0002e430: 6275 696c 7469 6e73 2e73 7472 5d5d 203d  builtins.str]] =
+0002e440: 204e 6f6e 652c 0a20 2020 206b 7562 6572   None,.    kuber
+0002e450: 6e65 7465 733a 2074 7970 696e 672e 4f70  netes: typing.Op
+0002e460: 7469 6f6e 616c 5b4b 7562 6572 6e65 7465  tional[Kubernete
+0002e470: 7345 6e75 6d5d 203d 204e 6f6e 652c 0a20  sEnum] = None,. 
+0002e480: 2020 2072 6566 733a 2074 7970 696e 672e     refs: typing.
+0002e490: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+0002e4a0: 5365 7175 656e 6365 5b62 7569 6c74 696e  Sequence[builtin
+0002e4b0: 732e 7374 725d 5d20 3d20 4e6f 6e65 2c0a  s.str]] = None,.
+0002e4c0: 2020 2020 7661 7269 6162 6c65 733a 2074      variables: t
+0002e4d0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+0002e4e0: 7970 696e 672e 5365 7175 656e 6365 5b62  yping.Sequence[b
+0002e4f0: 7569 6c74 696e 732e 7374 725d 5d20 3d20  uiltins.str]] = 
+0002e500: 4e6f 6e65 2c0a 2920 2d3e 204e 6f6e 653a  None,.) -> None:
+0002e510: 0a20 2020 2022 2222 5479 7065 2063 6865  .    """Type che
+0002e520: 636b 696e 6720 7374 7562 7322 2222 0a20  cking stubs""". 
+0002e530: 2020 2070 6173 730a 0a64 6566 205f 7479     pass..def _ty
+0002e540: 7065 6368 6563 6b69 6e67 7374 7562 5f5f  pecheckingstub__
+0002e550: 3962 3763 3232 6237 3532 3833 3764 3563  9b7c22b752837d5c
+0002e560: 3431 3938 3737 3631 3163 3336 3634 6361  419877611c3664ca
+0002e570: 6138 3836 3533 3961 6235 3230 3934 3635  a886539ab5209465
+0002e580: 6262 6665 3237 3337 3262 3531 6537 3134  bbfe27372b51e714
+0002e590: 280a 2020 2020 7072 6f6a 6563 743a 205f  (.    project: _
+0002e5a0: 5072 6f6a 6563 745f 3537 6438 3932 3033  Project_57d89203
+0002e5b0: 2c0a 2020 2020 2a2c 0a20 2020 2064 6566  ,.    *,.    def
+0002e5c0: 6175 6c74 3a20 7479 7069 6e67 2e4f 7074  ault: typing.Opt
+0002e5d0: 696f 6e61 6c5b 7479 7069 6e67 2e55 6e69  ional[typing.Uni
+0002e5e0: 6f6e 5b44 6566 6175 6c74 2c20 7479 7069  on[Default, typi
+0002e5f0: 6e67 2e44 6963 745b 6275 696c 7469 6e73  ng.Dict[builtins
+0002e600: 2e73 7472 2c20 7479 7069 6e67 2e41 6e79  .str, typing.Any
+0002e610: 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ]]] = None,.    
+0002e620: 6a6f 6273 3a20 7479 7069 6e67 2e4f 7074  jobs: typing.Opt
+0002e630: 696f 6e61 6c5b 7479 7069 6e67 2e4d 6170  ional[typing.Map
+0002e640: 7069 6e67 5b62 7569 6c74 696e 732e 7374  ping[builtins.st
+0002e650: 722c 2074 7970 696e 672e 556e 696f 6e5b  r, typing.Union[
+0002e660: 4a6f 622c 2074 7970 696e 672e 4469 6374  Job, typing.Dict
+0002e670: 5b62 7569 6c74 696e 732e 7374 722c 2074  [builtins.str, t
+0002e680: 7970 696e 672e 416e 795d 5d5d 5d20 3d20  yping.Any]]]] = 
+0002e690: 4e6f 6e65 2c0a 2020 2020 7061 6765 733a  None,.    pages:
+0002e6a0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0002e6b0: 5b74 7970 696e 672e 556e 696f 6e5b 4a6f  [typing.Union[Jo
+0002e6c0: 622c 2074 7970 696e 672e 4469 6374 5b62  b, typing.Dict[b
+0002e6d0: 7569 6c74 696e 732e 7374 722c 2074 7970  uiltins.str, typ
+0002e6e0: 696e 672e 416e 795d 5d5d 203d 204e 6f6e  ing.Any]]] = Non
+0002e6f0: 652c 0a20 2020 2073 7461 6765 733a 2074  e,.    stages: t
+0002e700: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+0002e710: 7970 696e 672e 5365 7175 656e 6365 5b62  yping.Sequence[b
+0002e720: 7569 6c74 696e 732e 7374 725d 5d20 3d20  uiltins.str]] = 
+0002e730: 4e6f 6e65 2c0a 2020 2020 7661 7269 6162  None,.    variab
+0002e740: 6c65 733a 2074 7970 696e 672e 4f70 7469  les: typing.Opti
+0002e750: 6f6e 616c 5b74 7970 696e 672e 4d61 7070  onal[typing.Mapp
+0002e760: 696e 675b 6275 696c 7469 6e73 2e73 7472  ing[builtins.str
+0002e770: 2c20 7479 7069 6e67 2e41 6e79 5d5d 203d  , typing.Any]] =
+0002e780: 204e 6f6e 652c 0a20 2020 2077 6f72 6b66   None,.    workf
+0002e790: 6c6f 773a 2074 7970 696e 672e 4f70 7469  low: typing.Opti
+0002e7a0: 6f6e 616c 5b74 7970 696e 672e 556e 696f  onal[typing.Unio
+0002e7b0: 6e5b 576f 726b 666c 6f77 2c20 7479 7069  n[Workflow, typi
+0002e7c0: 6e67 2e44 6963 745b 6275 696c 7469 6e73  ng.Dict[builtins
+0002e7d0: 2e73 7472 2c20 7479 7069 6e67 2e41 6e79  .str, typing.Any
+0002e7e0: 5d5d 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e  ]]] = None,.) ->
+0002e7f0: 204e 6f6e 653a 0a20 2020 2022 2222 5479   None:.    """Ty
+0002e800: 7065 2063 6865 636b 696e 6720 7374 7562  pe checking stub
+0002e810: 7322 2222 0a20 2020 2070 6173 730a 0a64  s""".    pass..d
+0002e820: 6566 205f 7479 7065 6368 6563 6b69 6e67  ef _typechecking
+0002e830: 7374 7562 5f5f 6130 6538 3963 3030 3464  stub__a0e89c004d
+0002e840: 6165 3564 6338 6136 3634 3737 6639 6530  ae5dc8a66477f9e0
+0002e850: 3564 3432 3032 6532 6465 3235 6233 3937  5d4202e2de25b397
+0002e860: 6164 3538 3433 3931 3538 6434 6430 6533  ad58439158d4d0e3
+0002e870: 3131 6661 3436 280a 2020 2020 636f 6e66  11fa46(.    conf
+0002e880: 6967 3a20 7479 7069 6e67 2e4d 6170 7069  ig: typing.Mappi
+0002e890: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
+0002e8a0: 2074 7970 696e 672e 556e 696f 6e5b 4369   typing.Union[Ci
+0002e8b0: 436f 6e66 6967 7572 6174 696f 6e4f 7074  ConfigurationOpt
+0002e8c0: 696f 6e73 2c20 7479 7069 6e67 2e44 6963  ions, typing.Dic
+0002e8d0: 745b 6275 696c 7469 6e73 2e73 7472 2c20  t[builtins.str, 
+0002e8e0: 7479 7069 6e67 2e41 6e79 5d5d 5d2c 0a29  typing.Any]]],.)
+0002e8f0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
+0002e900: 2254 7970 6520 6368 6563 6b69 6e67 2073  "Type checking s
+0002e910: 7475 6273 2222 220a 2020 2020 7061 7373  tubs""".    pass
+0002e920: 0a0a 6465 6620 5f74 7970 6563 6865 636b  ..def _typecheck
+0002e930: 696e 6773 7475 625f 5f61 3965 3662 6264  ingstub__a9e6bbd
+0002e940: 3763 3164 3365 3136 6666 6138 3233 3637  7c1d3e16ffa82367
+0002e950: 6364 6435 6361 3136 6365 3036 6134 3237  cdd5ca16ce06a427
+0002e960: 3236 6634 3139 3336 3339 3739 3061 3339  26f4193639790a39
+0002e970: 6262 3265 6164 6566 3928 0a20 2020 2076  bb2eadef9(.    v
+0002e980: 616c 7565 3a20 7479 7069 6e67 2e55 6e69  alue: typing.Uni
+0002e990: 6f6e 5b62 7569 6c74 696e 732e 7374 722c  on[builtins.str,
+0002e9a0: 2074 7970 696e 672e 4c69 7374 5b62 7569   typing.List[bui
+0002e9b0: 6c74 696e 732e 7374 725d 5d2c 0a29 202d  ltins.str]],.) -
+0002e9c0: 3e20 4e6f 6e65 3a0a 2020 2020 2222 2254  > None:.    """T
+0002e9d0: 7970 6520 6368 6563 6b69 6e67 2073 7475  ype checking stu
+0002e9e0: 6273 2222 220a 2020 2020 7061 7373 0a0a  bs""".    pass..
+0002e9f0: 6465 6620 5f74 7970 6563 6865 636b 696e  def _typecheckin
+0002ea00: 6773 7475 625f 5f31 6462 3034 3364 6531  gstub__1db043de1
+0002ea10: 6266 6439 3731 6366 3336 3261 3164 3530  bfd971cf362a1d50
+0002ea20: 3135 6433 3966 6366 6563 3963 6531 3261  15d39fcfec9ce12a
+0002ea30: 3835 3634 6531 3262 3364 6338 3363 3237  8564e12b3dc83c27
+0002ea40: 3636 6635 6537 6628 0a20 2020 202a 2c0a  66f5e7f(.    *,.
+0002ea50: 2020 2020 6e61 6d65 3a20 6275 696c 7469      name: builti
+0002ea60: 6e73 2e73 7472 2c0a 2020 2020 656e 7472  ns.str,.    entr
+0002ea70: 7970 6f69 6e74 3a20 7479 7069 6e67 2e4f  ypoint: typing.O
+0002ea80: 7074 696f 6e61 6c5b 7479 7069 6e67 2e53  ptional[typing.S
+0002ea90: 6571 7565 6e63 655b 7479 7069 6e67 2e41  equence[typing.A
+0002eaa0: 6e79 5d5d 203d 204e 6f6e 652c 0a29 202d  ny]] = None,.) -
+0002eab0: 3e20 4e6f 6e65 3a0a 2020 2020 2222 2254  > None:.    """T
+0002eac0: 7970 6520 6368 6563 6b69 6e67 2073 7475  ype checking stu
+0002ead0: 6273 2222 220a 2020 2020 7061 7373 0a0a  bs""".    pass..
+0002eae0: 6465 6620 5f74 7970 6563 6865 636b 696e  def _typecheckin
+0002eaf0: 6773 7475 625f 5f66 3662 3462 3333 6638  gstub__f6b4b33f8
+0002eb00: 3234 6465 6465 3363 3531 6638 3439 3166  24dede3c51f8491f
+0002eb10: 3233 6331 6232 3461 6139 3964 6538 3930  23c1b24aa99de890
+0002eb20: 3261 6232 6230 6164 6237 3932 6662 6331  2ab2b0adb792fbc1
+0002eb30: 3364 6466 3866 6528 0a20 2020 202a 2c0a  3ddf8fe(.    *,.
+0002eb40: 2020 2020 6669 6c65 3a20 7479 7069 6e67      file: typing
+0002eb50: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0002eb60: 2e53 6571 7565 6e63 655b 6275 696c 7469  .Sequence[builti
+0002eb70: 6e73 2e73 7472 5d5d 203d 204e 6f6e 652c  ns.str]] = None,
+0002eb80: 0a20 2020 206c 6f63 616c 3a20 7479 7069  .    local: typi
+0002eb90: 6e67 2e4f 7074 696f 6e61 6c5b 6275 696c  ng.Optional[buil
+0002eba0: 7469 6e73 2e73 7472 5d20 3d20 4e6f 6e65  tins.str] = None
+0002ebb0: 2c0a 2020 2020 7072 6f6a 6563 743a 2074  ,.    project: t
+0002ebc0: 7970 696e 672e 4f70 7469 6f6e 616c 5b62  yping.Optional[b
+0002ebd0: 7569 6c74 696e 732e 7374 725d 203d 204e  uiltins.str] = N
+0002ebe0: 6f6e 652c 0a20 2020 2072 6566 3a20 7479  one,.    ref: ty
+0002ebf0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 6275  ping.Optional[bu
+0002ec00: 696c 7469 6e73 2e73 7472 5d20 3d20 4e6f  iltins.str] = No
+0002ec10: 6e65 2c0a 2020 2020 7265 6d6f 7465 3a20  ne,.    remote: 
+0002ec20: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0002ec30: 6275 696c 7469 6e73 2e73 7472 5d20 3d20  builtins.str] = 
+0002ec40: 4e6f 6e65 2c0a 2020 2020 7275 6c65 733a  None,.    rules:
+0002ec50: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0002ec60: 5b74 7970 696e 672e 5365 7175 656e 6365  [typing.Sequence
+0002ec70: 5b74 7970 696e 672e 556e 696f 6e5b 496e  [typing.Union[In
+0002ec80: 636c 7564 6552 756c 652c 2074 7970 696e  cludeRule, typin
+0002ec90: 672e 4469 6374 5b62 7569 6c74 696e 732e  g.Dict[builtins.
+0002eca0: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
+0002ecb0: 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ]]] = None,.    
+0002ecc0: 7465 6d70 6c61 7465 3a20 7479 7069 6e67  template: typing
+0002ecd0: 2e4f 7074 696f 6e61 6c5b 6275 696c 7469  .Optional[builti
+0002ece0: 6e73 2e73 7472 5d20 3d20 4e6f 6e65 2c0a  ns.str] = None,.
+0002ecf0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
+0002ed00: 2222 5479 7065 2063 6865 636b 696e 6720  ""Type checking 
+0002ed10: 7374 7562 7322 2222 0a20 2020 2070 6173  stubs""".    pas
+0002ed20: 730a 0a64 6566 205f 7479 7065 6368 6563  s..def _typechec
+0002ed30: 6b69 6e67 7374 7562 5f5f 3535 3437 3032  kingstub__554702
+0002ed40: 3562 6265 3432 3231 3234 6635 3965 3738  5bbe422124f59e78
+0002ed50: 3262 3731 3431 3839 3462 6133 3764 6266  2b7141894ba37dbf
+0002ed60: 3030 3439 3037 3063 3733 6231 3766 3339  0049070c73b17f39
+0002ed70: 6465 3164 3138 3433 6131 280a 2020 2020  de1d1843a1(.    
+0002ed80: 2a2c 0a20 2020 2061 6c6c 6f77 5f66 6169  *,.    allow_fai
+0002ed90: 6c75 7265 3a20 7479 7069 6e67 2e4f 7074  lure: typing.Opt
+0002eda0: 696f 6e61 6c5b 7479 7069 6e67 2e55 6e69  ional[typing.Uni
+0002edb0: 6f6e 5b62 7569 6c74 696e 732e 626f 6f6c  on[builtins.bool
+0002edc0: 2c20 7479 7069 6e67 2e55 6e69 6f6e 5b41  , typing.Union[A
+0002edd0: 6c6c 6f77 4661 696c 7572 652c 2074 7970  llowFailure, typ
+0002ede0: 696e 672e 4469 6374 5b62 7569 6c74 696e  ing.Dict[builtin
+0002edf0: 732e 7374 722c 2074 7970 696e 672e 416e  s.str, typing.An
+0002ee00: 795d 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020  y]]]] = None,.  
+0002ee10: 2020 6368 616e 6765 733a 2074 7970 696e    changes: typin
+0002ee20: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+0002ee30: 672e 5365 7175 656e 6365 5b62 7569 6c74  g.Sequence[built
+0002ee40: 696e 732e 7374 725d 5d20 3d20 4e6f 6e65  ins.str]] = None
+0002ee50: 2c0a 2020 2020 6578 6973 7473 3a20 7479  ,.    exists: ty
+0002ee60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+0002ee70: 7069 6e67 2e53 6571 7565 6e63 655b 6275  ping.Sequence[bu
+0002ee80: 696c 7469 6e73 2e73 7472 5d5d 203d 204e  iltins.str]] = N
+0002ee90: 6f6e 652c 0a20 2020 2069 665f 3a20 7479  one,.    if_: ty
+0002eea0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 6275  ping.Optional[bu
+0002eeb0: 696c 7469 6e73 2e73 7472 5d20 3d20 4e6f  iltins.str] = No
+0002eec0: 6e65 2c0a 2020 2020 7374 6172 745f 696e  ne,.    start_in
+0002eed0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+0002eee0: 6c5b 6275 696c 7469 6e73 2e73 7472 5d20  l[builtins.str] 
+0002eef0: 3d20 4e6f 6e65 2c0a 2020 2020 7661 7269  = None,.    vari
+0002ef00: 6162 6c65 733a 2074 7970 696e 672e 4f70  ables: typing.Op
+0002ef10: 7469 6f6e 616c 5b74 7970 696e 672e 4d61  tional[typing.Ma
+0002ef20: 7070 696e 675b 6275 696c 7469 6e73 2e73  pping[builtins.s
+0002ef30: 7472 2c20 6275 696c 7469 6e73 2e73 7472  tr, builtins.str
+0002ef40: 5d5d 203d 204e 6f6e 652c 0a20 2020 2077  ]] = None,.    w
+0002ef50: 6865 6e3a 2074 7970 696e 672e 4f70 7469  hen: typing.Opti
+0002ef60: 6f6e 616c 5b4a 6f62 5768 656e 5d20 3d20  onal[JobWhen] = 
+0002ef70: 4e6f 6e65 2c0a 2920 2d3e 204e 6f6e 653a  None,.) -> None:
+0002ef80: 0a20 2020 2022 2222 5479 7065 2063 6865  .    """Type che
+0002ef90: 636b 696e 6720 7374 7562 7322 2222 0a20  cking stubs""". 
+0002efa0: 2020 2070 6173 730a 0a64 6566 205f 7479     pass..def _ty
+0002efb0: 7065 6368 6563 6b69 6e67 7374 7562 5f5f  pecheckingstub__
+0002efc0: 3738 6532 3032 3035 3666 3864 3065 6530  78e202056f8d0ee0
+0002efd0: 3436 3431 3563 6464 3065 6562 6137 6230  46415cdd0eeba7b0
+0002efe0: 3364 3431 3462 6264 3338 6663 3336 3739  3d414bbd38fc3679
+0002eff0: 3039 3032 3063 3464 3264 3237 3636 6366  09020c4d2d2766cf
+0002f000: 280a 2020 2020 2a2c 0a20 2020 2064 6566  (.    *,.    def
+0002f010: 6175 6c74 3a20 7479 7069 6e67 2e4f 7074  ault: typing.Opt
+0002f020: 696f 6e61 6c5b 7479 7069 6e67 2e55 6e69  ional[typing.Uni
+0002f030: 6f6e 5b62 7569 6c74 696e 732e 626f 6f6c  on[builtins.bool
+0002f040: 2c20 7479 7069 6e67 2e53 6571 7565 6e63  , typing.Sequenc
+0002f050: 655b 4465 6661 756c 7445 6c65 6d65 6e74  e[DefaultElement
+0002f060: 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ]]] = None,.    
+0002f070: 7661 7269 6162 6c65 733a 2074 7970 696e  variables: typin
+0002f080: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+0002f090: 672e 556e 696f 6e5b 6275 696c 7469 6e73  g.Union[builtins
+0002f0a0: 2e62 6f6f 6c2c 2074 7970 696e 672e 5365  .bool, typing.Se
+0002f0b0: 7175 656e 6365 5b62 7569 6c74 696e 732e  quence[builtins.
+0002f0c0: 7374 725d 5d5d 203d 204e 6f6e 652c 0a29  str]]] = None,.)
+0002f0d0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2222   -> None:.    ""
+0002f0e0: 2254 7970 6520 6368 6563 6b69 6e67 2073  "Type checking s
+0002f0f0: 7475 6273 2222 220a 2020 2020 7061 7373  tubs""".    pass
+0002f100: 0a0a 6465 6620 5f74 7970 6563 6865 636b  ..def _typecheck
+0002f110: 696e 6773 7475 625f 5f34 3835 6166 6238  ingstub__485afb8
+0002f120: 6361 3463 6631 3262 6461 6162 3363 3334  ca4cf12bdaab3c34
+0002f130: 3535 6337 6239 3066 3365 6139 6435 3439  55c7b90f3ea9d549
+0002f140: 6562 3837 6563 3666 6430 3565 6165 3034  eb87ec6fd05eae04
+0002f150: 3666 3366 3338 6264 3628 0a20 2020 202a  6f3f38bd6(.    *
+0002f160: 2c0a 2020 2020 6166 7465 725f 7363 7269  ,.    after_scri
+0002f170: 7074 3a20 7479 7069 6e67 2e4f 7074 696f  pt: typing.Optio
+0002f180: 6e61 6c5b 7479 7069 6e67 2e53 6571 7565  nal[typing.Seque
+0002f190: 6e63 655b 6275 696c 7469 6e73 2e73 7472  nce[builtins.str
+0002f1a0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2061  ]] = None,.    a
+0002f1b0: 6c6c 6f77 5f66 6169 6c75 7265 3a20 7479  llow_failure: ty
+0002f1c0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+0002f1d0: 7069 6e67 2e55 6e69 6f6e 5b62 7569 6c74  ping.Union[built
+0002f1e0: 696e 732e 626f 6f6c 2c20 7479 7069 6e67  ins.bool, typing
+0002f1f0: 2e55 6e69 6f6e 5b41 6c6c 6f77 4661 696c  .Union[AllowFail
+0002f200: 7572 652c 2074 7970 696e 672e 4469 6374  ure, typing.Dict
+0002f210: 5b62 7569 6c74 696e 732e 7374 722c 2074  [builtins.str, t
+0002f220: 7970 696e 672e 416e 795d 5d5d 5d20 3d20  yping.Any]]]] = 
+0002f230: 4e6f 6e65 2c0a 2020 2020 6172 7469 6661  None,.    artifa
+0002f240: 6374 733a 2074 7970 696e 672e 4f70 7469  cts: typing.Opti
+0002f250: 6f6e 616c 5b74 7970 696e 672e 556e 696f  onal[typing.Unio
+0002f260: 6e5b 4172 7469 6661 6374 732c 2074 7970  n[Artifacts, typ
+0002f270: 696e 672e 4469 6374 5b62 7569 6c74 696e  ing.Dict[builtin
+0002f280: 732e 7374 722c 2074 7970 696e 672e 416e  s.str, typing.An
+0002f290: 795d 5d5d 203d 204e 6f6e 652c 0a20 2020  y]]] = None,.   
+0002f2a0: 2062 6566 6f72 655f 7363 7269 7074 3a20   before_script: 
+0002f2b0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0002f2c0: 7479 7069 6e67 2e53 6571 7565 6e63 655b  typing.Sequence[
+0002f2d0: 6275 696c 7469 6e73 2e73 7472 5d5d 203d  builtins.str]] =
+0002f2e0: 204e 6f6e 652c 0a20 2020 2063 6163 6865   None,.    cache
+0002f2f0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+0002f300: 6c5b 7479 7069 6e67 2e53 6571 7565 6e63  l[typing.Sequenc
+0002f310: 655b 7479 7069 6e67 2e55 6e69 6f6e 5b43  e[typing.Union[C
+0002f320: 6163 6865 2c20 7479 7069 6e67 2e44 6963  ache, typing.Dic
+0002f330: 745b 6275 696c 7469 6e73 2e73 7472 2c20  t[builtins.str, 
+0002f340: 7479 7069 6e67 2e41 6e79 5d5d 5d5d 203d  typing.Any]]]] =
+0002f350: 204e 6f6e 652c 0a20 2020 2063 6f76 6572   None,.    cover
+0002f360: 6167 653a 2074 7970 696e 672e 4f70 7469  age: typing.Opti
+0002f370: 6f6e 616c 5b62 7569 6c74 696e 732e 7374  onal[builtins.st
+0002f380: 725d 203d 204e 6f6e 652c 0a20 2020 2064  r] = None,.    d
+0002f390: 6570 656e 6465 6e63 6965 733a 2074 7970  ependencies: typ
+0002f3a0: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0002f3b0: 696e 672e 5365 7175 656e 6365 5b62 7569  ing.Sequence[bui
+0002f3c0: 6c74 696e 732e 7374 725d 5d20 3d20 4e6f  ltins.str]] = No
+0002f3d0: 6e65 2c0a 2020 2020 656e 7669 726f 6e6d  ne,.    environm
+0002f3e0: 656e 743a 2074 7970 696e 672e 4f70 7469  ent: typing.Opti
+0002f3f0: 6f6e 616c 5b74 7970 696e 672e 556e 696f  onal[typing.Unio
+0002f400: 6e5b 6275 696c 7469 6e73 2e73 7472 2c20  n[builtins.str, 
+0002f410: 7479 7069 6e67 2e55 6e69 6f6e 5b45 6e76  typing.Union[Env
+0002f420: 6972 6f6e 6d65 6e74 2c20 7479 7069 6e67  ironment, typing
+0002f430: 2e44 6963 745b 6275 696c 7469 6e73 2e73  .Dict[builtins.s
+0002f440: 7472 2c20 7479 7069 6e67 2e41 6e79 5d5d  tr, typing.Any]]
+0002f450: 5d5d 203d 204e 6f6e 652c 0a20 2020 2065  ]] = None,.    e
+0002f460: 7863 6570 745f 3a20 7479 7069 6e67 2e4f  xcept_: typing.O
+0002f470: 7074 696f 6e61 6c5b 7479 7069 6e67 2e55  ptional[typing.U
+0002f480: 6e69 6f6e 5b74 7970 696e 672e 5365 7175  nion[typing.Sequ
+0002f490: 656e 6365 5b62 7569 6c74 696e 732e 7374  ence[builtins.st
+0002f4a0: 725d 2c20 7479 7069 6e67 2e55 6e69 6f6e  r], typing.Union
+0002f4b0: 5b46 696c 7465 722c 2074 7970 696e 672e  [Filter, typing.
+0002f4c0: 4469 6374 5b62 7569 6c74 696e 732e 7374  Dict[builtins.st
+0002f4d0: 722c 2074 7970 696e 672e 416e 795d 5d5d  r, typing.Any]]]
+0002f4e0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6578  ] = None,.    ex
+0002f4f0: 7465 6e64 733a 2074 7970 696e 672e 4f70  tends: typing.Op
+0002f500: 7469 6f6e 616c 5b74 7970 696e 672e 5365  tional[typing.Se
+0002f510: 7175 656e 6365 5b62 7569 6c74 696e 732e  quence[builtins.
+0002f520: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+0002f530: 2020 6964 5f74 6f6b 656e 733a 2074 7970    id_tokens: typ
+0002f540: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0002f550: 696e 672e 4d61 7070 696e 675b 6275 696c  ing.Mapping[buil
+0002f560: 7469 6e73 2e73 7472 2c20 4944 546f 6b65  tins.str, IDToke
+0002f570: 6e5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  n]] = None,.    
+0002f580: 696d 6167 653a 2074 7970 696e 672e 4f70  image: typing.Op
+0002f590: 7469 6f6e 616c 5b74 7970 696e 672e 556e  tional[typing.Un
+0002f5a0: 696f 6e5b 496d 6167 652c 2074 7970 696e  ion[Image, typin
+0002f5b0: 672e 4469 6374 5b62 7569 6c74 696e 732e  g.Dict[builtins.
+0002f5c0: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
+0002f5d0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2069  ]] = None,.    i
+0002f5e0: 6e68 6572 6974 3a20 7479 7069 6e67 2e4f  nherit: typing.O
+0002f5f0: 7074 696f 6e61 6c5b 7479 7069 6e67 2e55  ptional[typing.U
+0002f600: 6e69 6f6e 5b49 6e68 6572 6974 2c20 7479  nion[Inherit, ty
+0002f610: 7069 6e67 2e44 6963 745b 6275 696c 7469  ping.Dict[builti
+0002f620: 6e73 2e73 7472 2c20 7479 7069 6e67 2e41  ns.str, typing.A
+0002f630: 6e79 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020  ny]]] = None,.  
+0002f640: 2020 696e 7465 7272 7570 7469 626c 653a    interruptible:
+0002f650: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0002f660: 5b62 7569 6c74 696e 732e 626f 6f6c 5d20  [builtins.bool] 
+0002f670: 3d20 4e6f 6e65 2c0a 2020 2020 6e65 6564  = None,.    need
+0002f680: 733a 2074 7970 696e 672e 4f70 7469 6f6e  s: typing.Option
+0002f690: 616c 5b74 7970 696e 672e 5365 7175 656e  al[typing.Sequen
+0002f6a0: 6365 5b74 7970 696e 672e 556e 696f 6e5b  ce[typing.Union[
+0002f6b0: 6275 696c 7469 6e73 2e73 7472 2c20 7479  builtins.str, ty
+0002f6c0: 7069 6e67 2e55 6e69 6f6e 5b4e 6565 642c  ping.Union[Need,
+0002f6d0: 2074 7970 696e 672e 4469 6374 5b62 7569   typing.Dict[bui
+0002f6e0: 6c74 696e 732e 7374 722c 2074 7970 696e  ltins.str, typin
+0002f6f0: 672e 416e 795d 5d5d 5d5d 203d 204e 6f6e  g.Any]]]]] = Non
+0002f700: 652c 0a20 2020 206f 6e6c 793a 2074 7970  e,.    only: typ
+0002f710: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0002f720: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
+0002f730: 2e53 6571 7565 6e63 655b 6275 696c 7469  .Sequence[builti
+0002f740: 6e73 2e73 7472 5d2c 2074 7970 696e 672e  ns.str], typing.
+0002f750: 556e 696f 6e5b 4669 6c74 6572 2c20 7479  Union[Filter, ty
+0002f760: 7069 6e67 2e44 6963 745b 6275 696c 7469  ping.Dict[builti
+0002f770: 6e73 2e73 7472 2c20 7479 7069 6e67 2e41  ns.str, typing.A
+0002f780: 6e79 5d5d 5d5d 203d 204e 6f6e 652c 0a20  ny]]]] = None,. 
+0002f790: 2020 2070 6172 616c 6c65 6c3a 2074 7970     parallel: typ
+0002f7a0: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0002f7b0: 696e 672e 556e 696f 6e5b 6a73 6969 2e4e  ing.Union[jsii.N
+0002f7c0: 756d 6265 722c 2074 7970 696e 672e 556e  umber, typing.Un
+0002f7d0: 696f 6e5b 5061 7261 6c6c 656c 2c20 7479  ion[Parallel, ty
+0002f7e0: 7069 6e67 2e44 6963 745b 6275 696c 7469  ping.Dict[builti
+0002f7f0: 6e73 2e73 7472 2c20 7479 7069 6e67 2e41  ns.str, typing.A
+0002f800: 6e79 5d5d 5d5d 203d 204e 6f6e 652c 0a20  ny]]]] = None,. 
+0002f810: 2020 2072 656c 6561 7365 3a20 7479 7069     release: typi
+0002f820: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
+0002f830: 6e67 2e55 6e69 6f6e 5b52 656c 6561 7365  ng.Union[Release
+0002f840: 2c20 7479 7069 6e67 2e44 6963 745b 6275  , typing.Dict[bu
+0002f850: 696c 7469 6e73 2e73 7472 2c20 7479 7069  iltins.str, typi
+0002f860: 6e67 2e41 6e79 5d5d 5d20 3d20 4e6f 6e65  ng.Any]]] = None
+0002f870: 2c0a 2020 2020 7265 736f 7572 6365 5f67  ,.    resource_g
+0002f880: 726f 7570 3a20 7479 7069 6e67 2e4f 7074  roup: typing.Opt
+0002f890: 696f 6e61 6c5b 6275 696c 7469 6e73 2e73  ional[builtins.s
+0002f8a0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+0002f8b0: 7265 7472 793a 2074 7970 696e 672e 4f70  retry: typing.Op
+0002f8c0: 7469 6f6e 616c 5b74 7970 696e 672e 556e  tional[typing.Un
+0002f8d0: 696f 6e5b 5265 7472 792c 2074 7970 696e  ion[Retry, typin
+0002f8e0: 672e 4469 6374 5b62 7569 6c74 696e 732e  g.Dict[builtins.
+0002f8f0: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
+0002f900: 5d5d 203d 204e 6f6e 652c 0a20 2020 2072  ]] = None,.    r
+0002f910: 756c 6573 3a20 7479 7069 6e67 2e4f 7074  ules: typing.Opt
+0002f920: 696f 6e61 6c5b 7479 7069 6e67 2e53 6571  ional[typing.Seq
+0002f930: 7565 6e63 655b 7479 7069 6e67 2e55 6e69  uence[typing.Uni
+0002f940: 6f6e 5b49 6e63 6c75 6465 5275 6c65 2c20  on[IncludeRule, 
+0002f950: 7479 7069 6e67 2e44 6963 745b 6275 696c  typing.Dict[buil
+0002f960: 7469 6e73 2e73 7472 2c20 7479 7069 6e67  tins.str, typing
+0002f970: 2e41 6e79 5d5d 5d5d 203d 204e 6f6e 652c  .Any]]]] = None,
+0002f980: 0a20 2020 2073 6372 6970 743a 2074 7970  .    script: typ
+0002f990: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0002f9a0: 696e 672e 5365 7175 656e 6365 5b62 7569  ing.Sequence[bui
+0002f9b0: 6c74 696e 732e 7374 725d 5d20 3d20 4e6f  ltins.str]] = No
+0002f9c0: 6e65 2c0a 2020 2020 7365 6372 6574 733a  ne,.    secrets:
+0002f9d0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0002f9e0: 5b74 7970 696e 672e 4d61 7070 696e 675b  [typing.Mapping[
+0002f9f0: 6275 696c 7469 6e73 2e73 7472 2c20 7479  builtins.str, ty
+0002fa00: 7069 6e67 2e4d 6170 7069 6e67 5b62 7569  ping.Mapping[bui
+0002fa10: 6c74 696e 732e 7374 722c 2074 7970 696e  ltins.str, typin
+0002fa20: 672e 556e 696f 6e5b 5365 6372 6574 2c20  g.Union[Secret, 
+0002fa30: 7479 7069 6e67 2e44 6963 745b 6275 696c  typing.Dict[buil
+0002fa40: 7469 6e73 2e73 7472 2c20 7479 7069 6e67  tins.str, typing
+0002fa50: 2e41 6e79 5d5d 5d5d 5d20 3d20 4e6f 6e65  .Any]]]]] = None
+0002fa60: 2c0a 2020 2020 7365 7276 6963 6573 3a20  ,.    services: 
+0002fa70: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0002fa80: 7479 7069 6e67 2e53 6571 7565 6e63 655b  typing.Sequence[
+0002fa90: 7479 7069 6e67 2e55 6e69 6f6e 5b53 6572  typing.Union[Ser
+0002faa0: 7669 6365 2c20 7479 7069 6e67 2e44 6963  vice, typing.Dic
+0002fab0: 745b 6275 696c 7469 6e73 2e73 7472 2c20  t[builtins.str, 
+0002fac0: 7479 7069 6e67 2e41 6e79 5d5d 5d5d 203d  typing.Any]]]] =
+0002fad0: 204e 6f6e 652c 0a20 2020 2073 7461 6765   None,.    stage
+0002fae0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+0002faf0: 6c5b 6275 696c 7469 6e73 2e73 7472 5d20  l[builtins.str] 
+0002fb00: 3d20 4e6f 6e65 2c0a 2020 2020 7374 6172  = None,.    star
+0002fb10: 745f 696e 3a20 7479 7069 6e67 2e4f 7074  t_in: typing.Opt
+0002fb20: 696f 6e61 6c5b 6275 696c 7469 6e73 2e73  ional[builtins.s
+0002fb30: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+0002fb40: 7461 6773 3a20 7479 7069 6e67 2e4f 7074  tags: typing.Opt
+0002fb50: 696f 6e61 6c5b 7479 7069 6e67 2e53 6571  ional[typing.Seq
+0002fb60: 7565 6e63 655b 6275 696c 7469 6e73 2e73  uence[builtins.s
+0002fb70: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
+0002fb80: 2074 696d 656f 7574 3a20 7479 7069 6e67   timeout: typing
+0002fb90: 2e4f 7074 696f 6e61 6c5b 6275 696c 7469  .Optional[builti
+0002fba0: 6e73 2e73 7472 5d20 3d20 4e6f 6e65 2c0a  ns.str] = None,.
+0002fbb0: 2020 2020 7472 6967 6765 723a 2074 7970      trigger: typ
+0002fbc0: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0002fbd0: 696e 672e 556e 696f 6e5b 6275 696c 7469  ing.Union[builti
+0002fbe0: 6e73 2e73 7472 2c20 7479 7069 6e67 2e55  ns.str, typing.U
+0002fbf0: 6e69 6f6e 5b54 7269 6767 6572 2c20 7479  nion[Trigger, ty
+0002fc00: 7069 6e67 2e44 6963 745b 6275 696c 7469  ping.Dict[builti
+0002fc10: 6e73 2e73 7472 2c20 7479 7069 6e67 2e41  ns.str, typing.A
+0002fc20: 6e79 5d5d 5d5d 203d 204e 6f6e 652c 0a20  ny]]]] = None,. 
+0002fc30: 2020 2076 6172 6961 626c 6573 3a20 7479     variables: ty
+0002fc40: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+0002fc50: 7069 6e67 2e4d 6170 7069 6e67 5b62 7569  ping.Mapping[bui
+0002fc60: 6c74 696e 732e 7374 722c 2062 7569 6c74  ltins.str, built
+0002fc70: 696e 732e 7374 725d 5d20 3d20 4e6f 6e65  ins.str]] = None
+0002fc80: 2c0a 2020 2020 7768 656e 3a20 7479 7069  ,.    when: typi
+0002fc90: 6e67 2e4f 7074 696f 6e61 6c5b 4a6f 6257  ng.Optional[JobW
+0002fca0: 6865 6e5d 203d 204e 6f6e 652c 0a29 202d  hen] = None,.) -
+0002fcb0: 3e20 4e6f 6e65 3a0a 2020 2020 2222 2254  > None:.    """T
+0002fcc0: 7970 6520 6368 6563 6b69 6e67 2073 7475  ype checking stu
+0002fcd0: 6273 2222 220a 2020 2020 7061 7373 0a0a  bs""".    pass..
+0002fce0: 6465 6620 5f74 7970 6563 6865 636b 696e  def _typecheckin
+0002fcf0: 6773 7475 625f 5f33 6235 3133 3565 3132  gstub__3b5135e12
+0002fd00: 3262 3066 6239 3063 3561 6535 6438 6336  2b0fb90c5ae5d8c6
+0002fd10: 3536 3236 3731 3563 3237 3962 6136 6338  5626715c279ba6c8
+0002fd20: 6262 3431 3033 6434 6264 3761 3132 3936  bb4103d4bd7a1296
+0002fd30: 3964 3166 3561 6428 0a20 2020 202a 2c0a  9d1f5ad(.    *,.
+0002fd40: 2020 2020 6e61 6d65 7370 6163 653a 2074      namespace: t
+0002fd50: 7970 696e 672e 4f70 7469 6f6e 616c 5b62  yping.Optional[b
+0002fd60: 7569 6c74 696e 732e 7374 725d 203d 204e  uiltins.str] = N
+0002fd70: 6f6e 652c 0a29 202d 3e20 4e6f 6e65 3a0a  one,.) -> None:.
+0002fd80: 2020 2020 2222 2254 7970 6520 6368 6563      """Type chec
+0002fd90: 6b69 6e67 2073 7475 6273 2222 220a 2020  king stubs""".  
+0002fda0: 2020 7061 7373 0a0a 6465 6620 5f74 7970    pass..def _typ
+0002fdb0: 6563 6865 636b 696e 6773 7475 625f 5f30  echeckingstub__0
+0002fdc0: 3033 3637 3765 3338 3734 6564 3236 3734  03677e3874ed2674
+0002fdd0: 3766 3034 3865 3862 3563 3038 6133 3262  7f048e8b5c08a32b
+0002fde0: 3837 6630 3232 3666 3335 3232 6331 3062  87f0226f3522c10b
+0002fdf0: 3038 3434 6164 6532 3532 3139 3636 6328  0844ade2521966c(
+0002fe00: 0a20 2020 202a 2c0a 2020 2020 6e61 6d65  .    *,.    name
+0002fe10: 3a20 6275 696c 7469 6e73 2e73 7472 2c0a  : builtins.str,.
+0002fe20: 2020 2020 7572 6c3a 2062 7569 6c74 696e      url: builtin
+0002fe30: 732e 7374 722c 0a20 2020 2066 696c 6570  s.str,.    filep
+0002fe40: 6174 683a 2074 7970 696e 672e 4f70 7469  ath: typing.Opti
+0002fe50: 6f6e 616c 5b62 7569 6c74 696e 732e 7374  onal[builtins.st
+0002fe60: 725d 203d 204e 6f6e 652c 0a20 2020 206c  r] = None,.    l
+0002fe70: 696e 6b5f 7479 7065 3a20 7479 7069 6e67  ink_type: typing
+0002fe80: 2e4f 7074 696f 6e61 6c5b 4c69 6e6b 5479  .Optional[LinkTy
+0002fe90: 7065 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e  pe] = None,.) ->
+0002fea0: 204e 6f6e 653a 0a20 2020 2022 2222 5479   None:.    """Ty
+0002feb0: 7065 2063 6865 636b 696e 6720 7374 7562  pe checking stub
+0002fec0: 7322 2222 0a20 2020 2070 6173 730a 0a64  s""".    pass..d
+0002fed0: 6566 205f 7479 7065 6368 6563 6b69 6e67  ef _typechecking
+0002fee0: 7374 7562 5f5f 6336 3261 3862 3564 3539  stub__c62a8b5d59
+0002fef0: 6465 3230 6430 3831 3161 3665 6232 6165  de20d0811a6eb2ae
+0002ff00: 3865 6635 6133 3830 3939 6432 6139 6461  8ef5a38099d2a9da
+0002ff10: 3065 6266 6439 6339 6365 3864 3134 3036  0ebfd9c9ce8d1406
+0002ff20: 6365 3466 3865 280a 2020 2020 2a2c 0a20  ce4f8e(.    *,. 
+0002ff30: 2020 206a 6f62 3a20 6275 696c 7469 6e73     job: builtins
+0002ff40: 2e73 7472 2c0a 2020 2020 6172 7469 6661  .str,.    artifa
+0002ff50: 6374 733a 2074 7970 696e 672e 4f70 7469  cts: typing.Opti
+0002ff60: 6f6e 616c 5b62 7569 6c74 696e 732e 626f  onal[builtins.bo
+0002ff70: 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ol] = None,.    
+0002ff80: 6f70 7469 6f6e 616c 3a20 7479 7069 6e67  optional: typing
+0002ff90: 2e4f 7074 696f 6e61 6c5b 6275 696c 7469  .Optional[builti
+0002ffa0: 6e73 2e62 6f6f 6c5d 203d 204e 6f6e 652c  ns.bool] = None,
+0002ffb0: 0a20 2020 2070 6970 656c 696e 653a 2074  .    pipeline: t
+0002ffc0: 7970 696e 672e 4f70 7469 6f6e 616c 5b62  yping.Optional[b
+0002ffd0: 7569 6c74 696e 732e 7374 725d 203d 204e  uiltins.str] = N
+0002ffe0: 6f6e 652c 0a20 2020 2070 726f 6a65 6374  one,.    project
+0002fff0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00030000: 6c5b 6275 696c 7469 6e73 2e73 7472 5d20  l[builtins.str] 
+00030010: 3d20 4e6f 6e65 2c0a 2020 2020 7265 663a  = None,.    ref:
+00030020: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00030030: 5b62 7569 6c74 696e 732e 7374 725d 203d  [builtins.str] =
+00030040: 204e 6f6e 652c 0a29 202d 3e20 4e6f 6e65   None,.) -> None
+00030050: 3a0a 2020 2020 2222 2254 7970 6520 6368  :.    """Type ch
+00030060: 6563 6b69 6e67 2073 7475 6273 2222 220a  ecking stubs""".
+00030070: 2020 2020 7061 7373 0a0a 6465 6620 5f74      pass..def _t
+00030080: 7970 6563 6865 636b 696e 6773 7475 625f  ypecheckingstub_
+00030090: 5f32 3364 3766 3164 3864 3234 3366 6237  _23d7f1d8d243fb7
+000300a0: 6532 3735 6130 6565 6261 3366 3134 3139  e275a0eeba3f1419
+000300b0: 3832 3262 6632 6332 3734 6534 3736 3431  822bf2c274e47641
+000300c0: 6535 3533 6135 3637 3563 3030 3261 3433  e553a5675c002a43
+000300d0: 3728 0a20 2020 2070 726f 6a65 6374 3a20  7(.    project: 
+000300e0: 5f50 726f 6a65 6374 5f35 3764 3839 3230  _Project_57d8920
+000300f0: 332c 0a20 2020 2070 6172 656e 743a 2047  3,.    parent: G
+00030100: 6974 6c61 6243 6f6e 6669 6775 7261 7469  itlabConfigurati
+00030110: 6f6e 2c0a 2020 2020 6e61 6d65 3a20 6275  on,.    name: bu
+00030120: 696c 7469 6e73 2e73 7472 2c0a 2020 2020  iltins.str,.    
+00030130: 2a2c 0a20 2020 2064 6566 6175 6c74 3a20  *,.    default: 
+00030140: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00030150: 7479 7069 6e67 2e55 6e69 6f6e 5b44 6566  typing.Union[Def
+00030160: 6175 6c74 2c20 7479 7069 6e67 2e44 6963  ault, typing.Dic
+00030170: 745b 6275 696c 7469 6e73 2e73 7472 2c20  t[builtins.str, 
+00030180: 7479 7069 6e67 2e41 6e79 5d5d 5d20 3d20  typing.Any]]] = 
+00030190: 4e6f 6e65 2c0a 2020 2020 6a6f 6273 3a20  None,.    jobs: 
+000301a0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+000301b0: 7479 7069 6e67 2e4d 6170 7069 6e67 5b62  typing.Mapping[b
+000301c0: 7569 6c74 696e 732e 7374 722c 2074 7970  uiltins.str, typ
+000301d0: 696e 672e 556e 696f 6e5b 4a6f 622c 2074  ing.Union[Job, t
+000301e0: 7970 696e 672e 4469 6374 5b62 7569 6c74  yping.Dict[built
+000301f0: 696e 732e 7374 722c 2074 7970 696e 672e  ins.str, typing.
+00030200: 416e 795d 5d5d 5d20 3d20 4e6f 6e65 2c0a  Any]]]] = None,.
+00030210: 2020 2020 7061 6765 733a 2074 7970 696e      pages: typin
+00030220: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00030230: 672e 556e 696f 6e5b 4a6f 622c 2074 7970  g.Union[Job, typ
+00030240: 696e 672e 4469 6374 5b62 7569 6c74 696e  ing.Dict[builtin
+00030250: 732e 7374 722c 2074 7970 696e 672e 416e  s.str, typing.An
+00030260: 795d 5d5d 203d 204e 6f6e 652c 0a20 2020  y]]] = None,.   
+00030270: 2073 7461 6765 733a 2074 7970 696e 672e   stages: typing.
+00030280: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+00030290: 5365 7175 656e 6365 5b62 7569 6c74 696e  Sequence[builtin
+000302a0: 732e 7374 725d 5d20 3d20 4e6f 6e65 2c0a  s.str]] = None,.
+000302b0: 2020 2020 7661 7269 6162 6c65 733a 2074      variables: t
+000302c0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+000302d0: 7970 696e 672e 4d61 7070 696e 675b 6275  yping.Mapping[bu
+000302e0: 696c 7469 6e73 2e73 7472 2c20 7479 7069  iltins.str, typi
+000302f0: 6e67 2e41 6e79 5d5d 203d 204e 6f6e 652c  ng.Any]] = None,
+00030300: 0a20 2020 2077 6f72 6b66 6c6f 773a 2074  .    workflow: t
+00030310: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00030320: 7970 696e 672e 556e 696f 6e5b 576f 726b  yping.Union[Work
+00030330: 666c 6f77 2c20 7479 7069 6e67 2e44 6963  flow, typing.Dic
+00030340: 745b 6275 696c 7469 6e73 2e73 7472 2c20  t[builtins.str, 
+00030350: 7479 7069 6e67 2e41 6e79 5d5d 5d20 3d20  typing.Any]]] = 
+00030360: 4e6f 6e65 2c0a 2920 2d3e 204e 6f6e 653a  None,.) -> None:
+00030370: 0a20 2020 2022 2222 5479 7065 2063 6865  .    """Type che
+00030380: 636b 696e 6720 7374 7562 7322 2222 0a20  cking stubs""". 
+00030390: 2020 2070 6173 730a 0a64 6566 205f 7479     pass..def _ty
+000303a0: 7065 6368 6563 6b69 6e67 7374 7562 5f5f  pecheckingstub__
+000303b0: 3237 3833 3761 6535 6339 6530 3538 6562  27837ae5c9e058eb
+000303c0: 3038 3036 6431 6162 6436 3535 3763 3366  0806d1abd6557c3f
+000303d0: 6133 3632 6532 6466 3539 6463 6162 3863  a362e2df59dcab8c
+000303e0: 6531 6462 3534 3136 6330 3035 3235 6531  e1db5416c00525e1
+000303f0: 280a 2020 2020 2a2c 0a20 2020 206d 6174  (.    *,.    mat
+00030400: 7269 783a 2074 7970 696e 672e 5365 7175  rix: typing.Sequ
+00030410: 656e 6365 5b74 7970 696e 672e 4d61 7070  ence[typing.Mapp
+00030420: 696e 675b 6275 696c 7469 6e73 2e73 7472  ing[builtins.str
+00030430: 2c20 7479 7069 6e67 2e53 6571 7565 6e63  , typing.Sequenc
+00030440: 655b 7479 7069 6e67 2e41 6e79 5d5d 5d2c  e[typing.Any]]],
+00030450: 0a29 202d 3e20 4e6f 6e65 3a0a 2020 2020  .) -> None:.    
+00030460: 2222 2254 7970 6520 6368 6563 6b69 6e67  """Type checking
+00030470: 2073 7475 6273 2222 220a 2020 2020 7061   stubs""".    pa
+00030480: 7373 0a0a 6465 6620 5f74 7970 6563 6865  ss..def _typeche
+00030490: 636b 696e 6773 7475 625f 5f63 3338 6537  ckingstub__c38e7
+000304a0: 3534 3563 6166 3231 3635 3064 3366 6438  545caf21650d3fd8
+000304b0: 6439 6338 3637 3266 3761 6334 3939 3738  d9c8672f7ac49978
+000304c0: 6531 3330 3330 3865 6666 3732 3164 3236  e130308eff721d26
+000304d0: 3266 3563 6138 3631 6439 3328 0a20 2020  2f5ca861d93(.   
+000304e0: 202a 2c0a 2020 2020 6465 7363 7269 7074   *,.    descript
+000304f0: 696f 6e3a 2062 7569 6c74 696e 732e 7374  ion: builtins.st
+00030500: 722c 0a20 2020 2074 6167 5f6e 616d 653a  r,.    tag_name:
+00030510: 2062 7569 6c74 696e 732e 7374 722c 0a20   builtins.str,. 
+00030520: 2020 2061 7373 6574 733a 2074 7970 696e     assets: typin
+00030530: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00030540: 672e 556e 696f 6e5b 4173 7365 7473 2c20  g.Union[Assets, 
+00030550: 7479 7069 6e67 2e44 6963 745b 6275 696c  typing.Dict[buil
+00030560: 7469 6e73 2e73 7472 2c20 7479 7069 6e67  tins.str, typing
+00030570: 2e41 6e79 5d5d 5d20 3d20 4e6f 6e65 2c0a  .Any]]] = None,.
+00030580: 2020 2020 6d69 6c65 7374 6f6e 6573 3a20      milestones: 
+00030590: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+000305a0: 7479 7069 6e67 2e53 6571 7565 6e63 655b  typing.Sequence[
+000305b0: 6275 696c 7469 6e73 2e73 7472 5d5d 203d  builtins.str]] =
+000305c0: 204e 6f6e 652c 0a20 2020 206e 616d 653a   None,.    name:
+000305d0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+000305e0: 5b62 7569 6c74 696e 732e 7374 725d 203d  [builtins.str] =
+000305f0: 204e 6f6e 652c 0a20 2020 2072 6566 3a20   None,.    ref: 
+00030600: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00030610: 6275 696c 7469 6e73 2e73 7472 5d20 3d20  builtins.str] = 
+00030620: 4e6f 6e65 2c0a 2020 2020 7265 6c65 6173  None,.    releas
+00030630: 6564 5f61 743a 2074 7970 696e 672e 4f70  ed_at: typing.Op
+00030640: 7469 6f6e 616c 5b62 7569 6c74 696e 732e  tional[builtins.
+00030650: 7374 725d 203d 204e 6f6e 652c 0a29 202d  str] = None,.) -
+00030660: 3e20 4e6f 6e65 3a0a 2020 2020 2222 2254  > None:.    """T
+00030670: 7970 6520 6368 6563 6b69 6e67 2073 7475  ype checking stu
+00030680: 6273 2222 220a 2020 2020 7061 7373 0a0a  bs""".    pass..
+00030690: 6465 6620 5f74 7970 6563 6865 636b 696e  def _typecheckin
+000306a0: 6773 7475 625f 5f32 6339 6634 3033 3063  gstub__2c9f4030c
+000306b0: 6436 6536 6439 6338 3938 3830 3830 6166  d6e6d9c8988080af
+000306c0: 6531 3233 3431 6436 3734 6136 6430 3735  e12341d674a6d075
+000306d0: 3164 6131 6337 3933 3764 6433 3930 3163  1da1c7937dd3901c
+000306e0: 3964 3630 3632 6328 0a20 2020 202a 2c0a  9d6062c(.    *,.
+000306f0: 2020 2020 636f 6265 7274 7572 613a 2074      cobertura: t
+00030700: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00030710: 7970 696e 672e 5365 7175 656e 6365 5b62  yping.Sequence[b
+00030720: 7569 6c74 696e 732e 7374 725d 5d20 3d20  uiltins.str]] = 
+00030730: 4e6f 6e65 2c0a 2020 2020 636f 6465 7175  None,.    codequ
+00030740: 616c 6974 793a 2074 7970 696e 672e 4f70  ality: typing.Op
+00030750: 7469 6f6e 616c 5b74 7970 696e 672e 5365  tional[typing.Se
+00030760: 7175 656e 6365 5b62 7569 6c74 696e 732e  quence[builtins.
+00030770: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+00030780: 2020 636f 6e74 6169 6e65 725f 7363 616e    container_scan
+00030790: 6e69 6e67 3a20 7479 7069 6e67 2e4f 7074  ning: typing.Opt
+000307a0: 696f 6e61 6c5b 7479 7069 6e67 2e53 6571  ional[typing.Seq
+000307b0: 7565 6e63 655b 6275 696c 7469 6e73 2e73  uence[builtins.s
+000307c0: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
+000307d0: 2063 6f76 6572 6167 655f 7265 706f 7274   coverage_report
+000307e0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+000307f0: 6c5b 7479 7069 6e67 2e55 6e69 6f6e 5b43  l[typing.Union[C
+00030800: 6f76 6572 6167 6552 6570 6f72 742c 2074  overageReport, t
+00030810: 7970 696e 672e 4469 6374 5b62 7569 6c74  yping.Dict[built
+00030820: 696e 732e 7374 722c 2074 7970 696e 672e  ins.str, typing.
+00030830: 416e 795d 5d5d 203d 204e 6f6e 652c 0a20  Any]]] = None,. 
+00030840: 2020 2064 6173 743a 2074 7970 696e 672e     dast: typing.
+00030850: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+00030860: 5365 7175 656e 6365 5b62 7569 6c74 696e  Sequence[builtin
+00030870: 732e 7374 725d 5d20 3d20 4e6f 6e65 2c0a  s.str]] = None,.
+00030880: 2020 2020 6465 7065 6e64 656e 6379 5f73      dependency_s
+00030890: 6361 6e6e 696e 673a 2074 7970 696e 672e  canning: typing.
+000308a0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+000308b0: 5365 7175 656e 6365 5b62 7569 6c74 696e  Sequence[builtin
+000308c0: 732e 7374 725d 5d20 3d20 4e6f 6e65 2c0a  s.str]] = None,.
+000308d0: 2020 2020 646f 7465 6e76 3a20 7479 7069      dotenv: typi
+000308e0: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
+000308f0: 6e67 2e53 6571 7565 6e63 655b 6275 696c  ng.Sequence[buil
+00030900: 7469 6e73 2e73 7472 5d5d 203d 204e 6f6e  tins.str]] = Non
+00030910: 652c 0a20 2020 206a 756e 6974 3a20 7479  e,.    junit: ty
+00030920: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+00030930: 7069 6e67 2e53 6571 7565 6e63 655b 6275  ping.Sequence[bu
+00030940: 696c 7469 6e73 2e73 7472 5d5d 203d 204e  iltins.str]] = N
+00030950: 6f6e 652c 0a20 2020 206c 6963 656e 7365  one,.    license
+00030960: 5f6d 616e 6167 656d 656e 743a 2074 7970  _management: typ
+00030970: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+00030980: 696e 672e 5365 7175 656e 6365 5b62 7569  ing.Sequence[bui
+00030990: 6c74 696e 732e 7374 725d 5d20 3d20 4e6f  ltins.str]] = No
+000309a0: 6e65 2c0a 2020 2020 6c69 6365 6e73 655f  ne,.    license_
+000309b0: 7363 616e 6e69 6e67 3a20 7479 7069 6e67  scanning: typing
+000309c0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+000309d0: 2e53 6571 7565 6e63 655b 6275 696c 7469  .Sequence[builti
+000309e0: 6e73 2e73 7472 5d5d 203d 204e 6f6e 652c  ns.str]] = None,
+000309f0: 0a20 2020 206c 7369 663a 2074 7970 696e  .    lsif: typin
+00030a00: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00030a10: 672e 5365 7175 656e 6365 5b62 7569 6c74  g.Sequence[built
+00030a20: 696e 732e 7374 725d 5d20 3d20 4e6f 6e65  ins.str]] = None
+00030a30: 2c0a 2020 2020 6d65 7472 6963 733a 2074  ,.    metrics: t
+00030a40: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00030a50: 7970 696e 672e 5365 7175 656e 6365 5b62  yping.Sequence[b
+00030a60: 7569 6c74 696e 732e 7374 725d 5d20 3d20  uiltins.str]] = 
+00030a70: 4e6f 6e65 2c0a 2020 2020 7065 7266 6f72  None,.    perfor
+00030a80: 6d61 6e63 653a 2074 7970 696e 672e 4f70  mance: typing.Op
+00030a90: 7469 6f6e 616c 5b74 7970 696e 672e 5365  tional[typing.Se
+00030aa0: 7175 656e 6365 5b62 7569 6c74 696e 732e  quence[builtins.
+00030ab0: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+00030ac0: 2020 7265 7175 6972 656d 656e 7473 3a20    requirements: 
+00030ad0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00030ae0: 7479 7069 6e67 2e53 6571 7565 6e63 655b  typing.Sequence[
+00030af0: 6275 696c 7469 6e73 2e73 7472 5d5d 203d  builtins.str]] =
+00030b00: 204e 6f6e 652c 0a20 2020 2073 6173 743a   None,.    sast:
+00030b10: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00030b20: 5b74 7970 696e 672e 5365 7175 656e 6365  [typing.Sequence
+00030b30: 5b62 7569 6c74 696e 732e 7374 725d 5d20  [builtins.str]] 
+00030b40: 3d20 4e6f 6e65 2c0a 2020 2020 7365 6372  = None,.    secr
+00030b50: 6574 5f64 6574 6563 7469 6f6e 3a20 7479  et_detection: ty
+00030b60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+00030b70: 7069 6e67 2e53 6571 7565 6e63 655b 6275  ping.Sequence[bu
+00030b80: 696c 7469 6e73 2e73 7472 5d5d 203d 204e  iltins.str]] = N
+00030b90: 6f6e 652c 0a20 2020 2074 6572 7261 666f  one,.    terrafo
+00030ba0: 726d 3a20 7479 7069 6e67 2e4f 7074 696f  rm: typing.Optio
+00030bb0: 6e61 6c5b 7479 7069 6e67 2e53 6571 7565  nal[typing.Seque
+00030bc0: 6e63 655b 6275 696c 7469 6e73 2e73 7472  nce[builtins.str
+00030bd0: 5d5d 203d 204e 6f6e 652c 0a29 202d 3e20  ]] = None,.) -> 
+00030be0: 4e6f 6e65 3a0a 2020 2020 2222 2254 7970  None:.    """Typ
+00030bf0: 6520 6368 6563 6b69 6e67 2073 7475 6273  e checking stubs
+00030c00: 2222 220a 2020 2020 7061 7373 0a0a 6465  """.    pass..de
+00030c10: 6620 5f74 7970 6563 6865 636b 696e 6773  f _typecheckings
+00030c20: 7475 625f 5f65 6362 6235 3763 3063 3931  tub__ecbb57c0c91
+00030c30: 3464 3366 6536 3161 6430 6663 3330 6336  4d3fe61ad0fc30c6
+00030c40: 3662 3166 6138 3932 3432 3235 3761 6532  6b1fa89242257ae2
+00030c50: 6537 6662 6433 3039 6535 3831 3932 3530  e7fbd309e5819250
+00030c60: 6163 3235 6528 0a20 2020 202a 2c0a 2020  ac25e(.    *,.  
+00030c70: 2020 6d61 783a 2074 7970 696e 672e 4f70    max: typing.Op
+00030c80: 7469 6f6e 616c 5b6a 7369 692e 4e75 6d62  tional[jsii.Numb
+00030c90: 6572 5d20 3d20 4e6f 6e65 2c0a 2020 2020  er] = None,.    
+00030ca0: 7768 656e 3a20 7479 7069 6e67 2e41 6e79  when: typing.Any
+00030cb0: 203d 204e 6f6e 652c 0a29 202d 3e20 4e6f   = None,.) -> No
+00030cc0: 6e65 3a0a 2020 2020 2222 2254 7970 6520  ne:.    """Type 
+00030cd0: 6368 6563 6b69 6e67 2073 7475 6273 2222  checking stubs""
+00030ce0: 220a 2020 2020 7061 7373 0a0a 6465 6620  ".    pass..def 
+00030cf0: 5f74 7970 6563 6865 636b 696e 6773 7475  _typecheckingstu
+00030d00: 625f 5f37 3839 6162 3837 6139 3337 6637  b__789ab87a937f7
+00030d10: 3532 3931 3233 6637 6466 6531 3566 3437  529123f7dfe15f47
+00030d20: 3331 6662 3262 6132 6364 3335 3239 3638  31fb2ba2cd352968
+00030d30: 3161 3163 3562 3763 3237 3636 6163 3531  1a1c5b7c2766ac51
+00030d40: 3865 6428 0a20 2020 202a 2c0a 2020 2020  8ed(.    *,.    
+00030d50: 7661 756c 743a 2074 7970 696e 672e 556e  vault: typing.Un
+00030d60: 696f 6e5b 5661 756c 7443 6f6e 6669 672c  ion[VaultConfig,
+00030d70: 2074 7970 696e 672e 4469 6374 5b62 7569   typing.Dict[bui
+00030d80: 6c74 696e 732e 7374 722c 2074 7970 696e  ltins.str, typin
+00030d90: 672e 416e 795d 5d2c 0a29 202d 3e20 4e6f  g.Any]],.) -> No
+00030da0: 6e65 3a0a 2020 2020 2222 2254 7970 6520  ne:.    """Type 
+00030db0: 6368 6563 6b69 6e67 2073 7475 6273 2222  checking stubs""
+00030dc0: 220a 2020 2020 7061 7373 0a0a 6465 6620  ".    pass..def 
+00030dd0: 5f74 7970 6563 6865 636b 696e 6773 7475  _typecheckingstu
+00030de0: 625f 5f31 6532 3039 3436 3861 3366 3961  b__1e209468a3f9a
+00030df0: 6162 3666 3035 3432 3631 3162 6335 6532  ab6f0542611bc5e2
+00030e00: 6237 3536 6261 6334 3234 3631 3431 3365  b756bac42461413e
+00030e10: 6165 6164 3137 3836 6131 6238 3365 6433  aead1786a1b83ed3
+00030e20: 6432 3728 0a20 2020 202a 2c0a 2020 2020  d27(.    *,.    
+00030e30: 6e61 6d65 3a20 6275 696c 7469 6e73 2e73  name: builtins.s
+00030e40: 7472 2c0a 2020 2020 616c 6961 733a 2074  tr,.    alias: t
+00030e50: 7970 696e 672e 4f70 7469 6f6e 616c 5b62  yping.Optional[b
+00030e60: 7569 6c74 696e 732e 7374 725d 203d 204e  uiltins.str] = N
+00030e70: 6f6e 652c 0a20 2020 2063 6f6d 6d61 6e64  one,.    command
+00030e80: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00030e90: 6c5b 7479 7069 6e67 2e53 6571 7565 6e63  l[typing.Sequenc
+00030ea0: 655b 6275 696c 7469 6e73 2e73 7472 5d5d  e[builtins.str]]
+00030eb0: 203d 204e 6f6e 652c 0a20 2020 2065 6e74   = None,.    ent
+00030ec0: 7279 706f 696e 743a 2074 7970 696e 672e  rypoint: typing.
+00030ed0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+00030ee0: 5365 7175 656e 6365 5b62 7569 6c74 696e  Sequence[builtin
+00030ef0: 732e 7374 725d 5d20 3d20 4e6f 6e65 2c0a  s.str]] = None,.
+00030f00: 2020 2020 7075 6c6c 5f70 6f6c 6963 793a      pull_policy:
+00030f10: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00030f20: 5b74 7970 696e 672e 5365 7175 656e 6365  [typing.Sequence
+00030f30: 5b50 756c 6c50 6f6c 6963 795d 5d20 3d20  [PullPolicy]] = 
+00030f40: 4e6f 6e65 2c0a 2020 2020 7661 7269 6162  None,.    variab
+00030f50: 6c65 733a 2074 7970 696e 672e 4f70 7469  les: typing.Opti
+00030f60: 6f6e 616c 5b74 7970 696e 672e 4d61 7070  onal[typing.Mapp
+00030f70: 696e 675b 6275 696c 7469 6e73 2e73 7472  ing[builtins.str
+00030f80: 2c20 6275 696c 7469 6e73 2e73 7472 5d5d  , builtins.str]]
+00030f90: 203d 204e 6f6e 652c 0a29 202d 3e20 4e6f   = None,.) -> No
+00030fa0: 6e65 3a0a 2020 2020 2222 2254 7970 6520  ne:.    """Type 
+00030fb0: 6368 6563 6b69 6e67 2073 7475 6273 2222  checking stubs""
+00030fc0: 220a 2020 2020 7061 7373 0a0a 6465 6620  ".    pass..def 
+00030fd0: 5f74 7970 6563 6865 636b 696e 6773 7475  _typecheckingstu
+00030fe0: 625f 5f37 3861 6563 3661 3663 3436 3233  b__78aec6a6c4623
+00030ff0: 3331 6366 6662 3864 3861 6635 3131 6137  31cffb8d8af511a7
+00031000: 6130 3465 6139 3661 3765 3236 3065 3033  a04ea96a7e260e03
+00031010: 6638 6438 3537 6261 3537 3130 3362 3663  f8d857ba57103b6c
+00031020: 3839 6628 0a20 2020 202a 2c0a 2020 2020  89f(.    *,.    
+00031030: 6272 616e 6368 3a20 7479 7069 6e67 2e4f  branch: typing.O
+00031040: 7074 696f 6e61 6c5b 6275 696c 7469 6e73  ptional[builtins
+00031050: 2e73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  .str] = None,.  
+00031060: 2020 696e 636c 7564 653a 2074 7970 696e    include: typin
+00031070: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00031080: 672e 5365 7175 656e 6365 5b74 7970 696e  g.Sequence[typin
+00031090: 672e 556e 696f 6e5b 5472 6967 6765 7249  g.Union[TriggerI
+000310a0: 6e63 6c75 6465 2c20 7479 7069 6e67 2e44  nclude, typing.D
+000310b0: 6963 745b 6275 696c 7469 6e73 2e73 7472  ict[builtins.str
+000310c0: 2c20 7479 7069 6e67 2e41 6e79 5d5d 5d5d  , typing.Any]]]]
+000310d0: 203d 204e 6f6e 652c 0a20 2020 2070 726f   = None,.    pro
+000310e0: 6a65 6374 3a20 7479 7069 6e67 2e4f 7074  ject: typing.Opt
+000310f0: 696f 6e61 6c5b 6275 696c 7469 6e73 2e73  ional[builtins.s
+00031100: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00031110: 7374 7261 7465 6779 3a20 7479 7069 6e67  strategy: typing
+00031120: 2e4f 7074 696f 6e61 6c5b 5374 7261 7465  .Optional[Strate
+00031130: 6779 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e  gy] = None,.) ->
+00031140: 204e 6f6e 653a 0a20 2020 2022 2222 5479   None:.    """Ty
+00031150: 7065 2063 6865 636b 696e 6720 7374 7562  pe checking stub
+00031160: 7322 2222 0a20 2020 2070 6173 730a 0a64  s""".    pass..d
+00031170: 6566 205f 7479 7065 6368 6563 6b69 6e67  ef _typechecking
+00031180: 7374 7562 5f5f 6263 6634 3965 3863 6362  stub__bcf49e8ccb
+00031190: 6533 3135 3463 3734 3266 3666 3130 6466  e3154c742f6f10df
+000311a0: 3630 6533 3932 3636 6662 3934 3831 6230  60e39266fb9481b0
+000311b0: 6332 3635 3832 3432 3635 3930 6266 3863  c26582426590bf8c
+000311c0: 6430 3365 3462 280a 2020 2020 2a2c 0a20  d03e4b(.    *,. 
+000311d0: 2020 2061 7274 6966 6163 743a 2074 7970     artifact: typ
+000311e0: 696e 672e 4f70 7469 6f6e 616c 5b62 7569  ing.Optional[bui
+000311f0: 6c74 696e 732e 7374 725d 203d 204e 6f6e  ltins.str] = Non
+00031200: 652c 0a20 2020 2066 696c 653a 2074 7970  e,.    file: typ
+00031210: 696e 672e 4f70 7469 6f6e 616c 5b62 7569  ing.Optional[bui
+00031220: 6c74 696e 732e 7374 725d 203d 204e 6f6e  ltins.str] = Non
+00031230: 652c 0a20 2020 206a 6f62 3a20 7479 7069  e,.    job: typi
+00031240: 6e67 2e4f 7074 696f 6e61 6c5b 6275 696c  ng.Optional[buil
+00031250: 7469 6e73 2e73 7472 5d20 3d20 4e6f 6e65  tins.str] = None
+00031260: 2c0a 2020 2020 6c6f 6361 6c3a 2074 7970  ,.    local: typ
+00031270: 696e 672e 4f70 7469 6f6e 616c 5b62 7569  ing.Optional[bui
+00031280: 6c74 696e 732e 7374 725d 203d 204e 6f6e  ltins.str] = Non
+00031290: 652c 0a20 2020 2070 726f 6a65 6374 3a20  e,.    project: 
+000312a0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+000312b0: 6275 696c 7469 6e73 2e73 7472 5d20 3d20  builtins.str] = 
+000312c0: 4e6f 6e65 2c0a 2020 2020 7265 663a 2074  None,.    ref: t
+000312d0: 7970 696e 672e 4f70 7469 6f6e 616c 5b62  yping.Optional[b
+000312e0: 7569 6c74 696e 732e 7374 725d 203d 204e  uiltins.str] = N
+000312f0: 6f6e 652c 0a20 2020 2074 656d 706c 6174  one,.    templat
+00031300: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
+00031310: 616c 5b62 7569 6c74 696e 732e 7374 725d  al[builtins.str]
+00031320: 203d 204e 6f6e 652c 0a29 202d 3e20 4e6f   = None,.) -> No
+00031330: 6e65 3a0a 2020 2020 2222 2254 7970 6520  ne:.    """Type 
+00031340: 6368 6563 6b69 6e67 2073 7475 6273 2222  checking stubs""
+00031350: 220a 2020 2020 7061 7373 0a0a 6465 6620  ".    pass..def 
+00031360: 5f74 7970 6563 6865 636b 696e 6773 7475  _typecheckingstu
+00031370: 625f 5f32 3730 6433 3434 3264 3263 3562  b__270d3442d2c5b
+00031380: 3966 3138 6534 3735 6261 3263 3934 3563  9f18e475ba2c945c
+00031390: 6135 3736 3565 6536 3165 6439 3463 3565  a5765ee61ed94c5e
+000313a0: 6132 3864 3433 3935 6239 6333 3935 3264  a28d4395b9c3952d
+000313b0: 6635 3828 0a20 2020 202a 2c0a 2020 2020  f58(.    *,.    
+000313c0: 6465 7363 7269 7074 696f 6e3a 2074 7970  description: typ
+000313d0: 696e 672e 4f70 7469 6f6e 616c 5b62 7569  ing.Optional[bui
+000313e0: 6c74 696e 732e 7374 725d 203d 204e 6f6e  ltins.str] = Non
+000313f0: 652c 0a20 2020 2076 616c 7565 3a20 7479  e,.    value: ty
+00031400: 7069 6e67 2e4f 7074 696f 6e61 6c5b 6275  ping.Optional[bu
+00031410: 696c 7469 6e73 2e73 7472 5d20 3d20 4e6f  iltins.str] = No
+00031420: 6e65 2c0a 2920 2d3e 204e 6f6e 653a 0a20  ne,.) -> None:. 
+00031430: 2020 2022 2222 5479 7065 2063 6865 636b     """Type check
+00031440: 696e 6720 7374 7562 7322 2222 0a20 2020  ing stubs""".   
+00031450: 2070 6173 730a 0a64 6566 205f 7479 7065   pass..def _type
+00031460: 6368 6563 6b69 6e67 7374 7562 5f5f 3862  checkingstub__8b
+00031470: 6638 6238 3839 3935 6537 6232 3336 6530  f8b88995e7b236e0
+00031480: 3534 3861 6664 3536 3030 3431 6663 3864  548afd560041fc8d
+00031490: 6536 3833 6337 3137 3038 3231 3863 6531  e683c71708218ce1
+000314a0: 6166 3238 3138 6566 6433 6232 3438 280a  af2818efd3b248(.
+000314b0: 2020 2020 2a2c 0a20 2020 2065 6e67 696e      *,.    engin
+000314c0: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
+000314d0: 456e 6769 6e65 2c20 7479 7069 6e67 2e44  Engine, typing.D
+000314e0: 6963 745b 6275 696c 7469 6e73 2e73 7472  ict[builtins.str
+000314f0: 2c20 7479 7069 6e67 2e41 6e79 5d5d 2c0a  , typing.Any]],.
+00031500: 2020 2020 6669 656c 643a 2062 7569 6c74      field: built
+00031510: 696e 732e 7374 722c 0a20 2020 2070 6174  ins.str,.    pat
+00031520: 683a 2062 7569 6c74 696e 732e 7374 722c  h: builtins.str,
+00031530: 0a29 202d 3e20 4e6f 6e65 3a0a 2020 2020  .) -> None:.    
+00031540: 2222 2254 7970 6520 6368 6563 6b69 6e67  """Type checking
+00031550: 2073 7475 6273 2222 220a 2020 2020 7061   stubs""".    pa
+00031560: 7373 0a0a 6465 6620 5f74 7970 6563 6865  ss..def _typeche
+00031570: 636b 696e 6773 7475 625f 5f65 3062 3735  ckingstub__e0b75
+00031580: 3034 3766 3662 6637 6562 3738 3862 3038  047f6bf7eb788b08
+00031590: 6663 3030 3761 3636 3537 3334 3830 6133  fc007a66573480a3
+000315a0: 3865 3931 3362 6465 3335 3161 6361 6163  8e913bde351acaac
+000315b0: 3035 3334 3764 3436 3762 3128 0a20 2020  05347d467b1(.   
+000315c0: 202a 2c0a 2020 2020 7275 6c65 733a 2074   *,.    rules: t
+000315d0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+000315e0: 7970 696e 672e 5365 7175 656e 6365 5b74  yping.Sequence[t
+000315f0: 7970 696e 672e 556e 696f 6e5b 576f 726b  yping.Union[Work
+00031600: 666c 6f77 5275 6c65 2c20 7479 7069 6e67  flowRule, typing
+00031610: 2e44 6963 745b 6275 696c 7469 6e73 2e73  .Dict[builtins.s
+00031620: 7472 2c20 7479 7069 6e67 2e41 6e79 5d5d  tr, typing.Any]]
+00031630: 5d5d 203d 204e 6f6e 652c 0a29 202d 3e20  ]] = None,.) -> 
+00031640: 4e6f 6e65 3a0a 2020 2020 2222 2254 7970  None:.    """Typ
+00031650: 6520 6368 6563 6b69 6e67 2073 7475 6273  e checking stubs
+00031660: 2222 220a 2020 2020 7061 7373 0a0a 6465  """.    pass..de
+00031670: 6620 5f74 7970 6563 6865 636b 696e 6773  f _typecheckings
+00031680: 7475 625f 5f30 3161 3263 6634 6332 6139  tub__01a2cf4c2a9
+00031690: 3832 6137 3439 6431 3235 3131 6439 6534  82a749d12511d9e4
+000316a0: 3334 3638 6633 6234 6139 6363 6131 3664  3468f3b4a9cca16d
+000316b0: 3663 3536 6439 6132 6366 6431 3135 3437  6c56d9a2cfd11547
+000316c0: 3230 6436 3328 0a20 2020 202a 2c0a 2020  20d63(.    *,.  
+000316d0: 2020 6368 616e 6765 733a 2074 7970 696e    changes: typin
+000316e0: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+000316f0: 672e 5365 7175 656e 6365 5b62 7569 6c74  g.Sequence[built
+00031700: 696e 732e 7374 725d 5d20 3d20 4e6f 6e65  ins.str]] = None
+00031710: 2c0a 2020 2020 6578 6973 7473 3a20 7479  ,.    exists: ty
+00031720: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+00031730: 7069 6e67 2e53 6571 7565 6e63 655b 6275  ping.Sequence[bu
+00031740: 696c 7469 6e73 2e73 7472 5d5d 203d 204e  iltins.str]] = N
+00031750: 6f6e 652c 0a20 2020 2069 665f 3a20 7479  one,.    if_: ty
+00031760: 7069 6e67 2e4f 7074 696f 6e61 6c5b 6275  ping.Optional[bu
+00031770: 696c 7469 6e73 2e73 7472 5d20 3d20 4e6f  iltins.str] = No
+00031780: 6e65 2c0a 2020 2020 7661 7269 6162 6c65  ne,.    variable
+00031790: 733a 2074 7970 696e 672e 4f70 7469 6f6e  s: typing.Option
+000317a0: 616c 5b74 7970 696e 672e 4d61 7070 696e  al[typing.Mappin
+000317b0: 675b 6275 696c 7469 6e73 2e73 7472 2c20  g[builtins.str, 
+000317c0: 7479 7069 6e67 2e55 6e69 6f6e 5b62 7569  typing.Union[bui
+000317d0: 6c74 696e 732e 7374 722c 206a 7369 692e  ltins.str, jsii.
+000317e0: 4e75 6d62 6572 5d5d 5d20 3d20 4e6f 6e65  Number]]] = None
+000317f0: 2c0a 2020 2020 7768 656e 3a20 7479 7069  ,.    when: typi
+00031800: 6e67 2e4f 7074 696f 6e61 6c5b 576f 726b  ng.Optional[Work
+00031810: 666c 6f77 5768 656e 5d20 3d20 4e6f 6e65  flowWhen] = None
+00031820: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
+00031830: 2022 2222 5479 7065 2063 6865 636b 696e   """Type checkin
+00031840: 6720 7374 7562 7322 2222 0a20 2020 2070  g stubs""".    p
+00031850: 6173 730a                                ass.
```

### Comparing `projen-0.81.9/src/projen/java/__init__.py` & `projen-0.82.0/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/javascript/__init__.py` & `projen-0.82.0/src/projen/javascript/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2188,15 +2188,15 @@
         :param bail: (experimental) By default, Jest runs all tests and produces all errors into the console upon completion. The bail config option can be used here to have Jest stop running tests after n failures. Setting bail to true is the same as setting bail to 1. Default: - 0
         :param cache_directory: (experimental) The directory where Jest should store its cached dependency information. Default: - "/tmp/"
         :param clear_mocks: (experimental) Automatically clear mock calls and instances before every test. Equivalent to calling jest.clearAllMocks() before each test. This does not remove any mock implementation that may have been provided Default: true
         :param collect_coverage: (experimental) Indicates whether the coverage information should be collected while executing the test. Because this retrofits all executed files with coverage collection statements, it may significantly slow down your tests Default: true
         :param collect_coverage_from: (experimental) An array of glob patterns indicating a set of files for which coverage information should be collected. Default: - undefined
         :param coverage_directory: (experimental) The directory where Jest should output its coverage files. Default: "coverage"
         :param coverage_path_ignore_patterns: (experimental) An array of regexp pattern strings that are matched against all file paths before executing the test. If the file path matches any of the patterns, coverage information will be skipped Default: "/node_modules/"
-        :param coverage_provider: (experimental) Indicates which provider should be used to instrument code for coverage. Allowed values are babel (default) or v8 Default: - "babel"
+        :param coverage_provider: (experimental) Indicates which provider should be used to instrument code for coverage. Allowed values are v8 (default) or babel Default: - "v8"
         :param coverage_reporters: (experimental) A list of reporter names that Jest uses when writing coverage reports. Any istanbul reporter can be used Default: - ["json", "lcov", "text", "clover", "cobertura"]
         :param coverage_threshold: (experimental) Specify the global coverage thresholds. This will be used to configure minimum threshold enforcement for coverage results. Thresholds can be specified as global, as a glob, and as a directory or file path. If thresholds aren't met, jest will fail. Default: - undefined
         :param dependency_extractor: (experimental) This option allows the use of a custom dependency extractor. It must be a node module that exports an object with an extract function Default: - undefined
         :param display_name: (experimental) Allows for a label to be printed alongside a test while it is running. Default: - undefined
         :param error_on_deprecated: (experimental) Make calling deprecated APIs throw helpful error messages. Useful for easing the upgrade process. Default: - false
         :param extra_globals: (experimental) Test files run inside a vm, which slows calls to global context properties (e.g. Math). With this option you can specify extra properties to be defined inside the vm for faster lookups. Default: - undefined
         :param force_coverage_match: (experimental) Test files are normally ignored from collecting code coverage. With this option, you can overwrite this behavior and include otherwise ignored files in code coverage. Default: - ['']
@@ -2572,17 +2572,17 @@
         result = self._values.get("coverage_path_ignore_patterns")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def coverage_provider(self) -> typing.Optional[builtins.str]:
         '''(experimental) Indicates which provider should be used to instrument code for coverage.
 
-        Allowed values are babel (default) or v8
+        Allowed values are v8 (default) or babel
 
-        :default: - "babel"
+        :default: - "v8"
 
         :stability: experimental
         '''
         result = self._values.get("coverage_provider")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
```

### Comparing `projen-0.81.9/src/projen/python/__init__.py` & `projen-0.82.0/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/release/__init__.py` & `projen-0.82.0/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/typescript/__init__.py` & `projen-0.82.0/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/vscode/__init__.py` & `projen-0.82.0/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen/web/__init__.py` & `projen-0.82.0/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.9/src/projen.egg-info/PKG-INFO` & `projen-0.82.0/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.81.9
+Version: 0.82.0
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.81.9/src/projen.egg-info/SOURCES.txt` & `projen-0.82.0/src/projen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.81.9.jsii.tgz
+src/projen/_jsii/projen@0.82.0.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

