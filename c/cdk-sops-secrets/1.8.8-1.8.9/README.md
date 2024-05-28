# Comparing `tmp/cdk-sops-secrets-1.8.8.tar.gz` & `tmp/cdk-sops-secrets-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-sops-secrets-1.8.8.tar", last modified: Sat May 25 21:34:18 2024, max compression
+gzip compressed data, was "cdk-sops-secrets-1.8.9.tar", last modified: Tue May 28 11:32:30 2024, max compression
```

## Comparing `cdk-sops-secrets-1.8.8.tar` & `cdk-sops-secrets-1.8.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:34:18.701746 cdk-sops-secrets-1.8.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-25 21:34:08.000000 cdk-sops-secrets-1.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-25 21:34:08.000000 cdk-sops-secrets-1.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-25 21:34:18.701746 cdk-sops-secrets-1.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-05-25 21:34:08.000000 cdk-sops-secrets-1.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 21:34:08.000000 cdk-sops-secrets-1.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 21:34:18.701746 cdk-sops-secrets-1.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-25 21:34:08.000000 cdk-sops-secrets-1.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:34:18.685746 cdk-sops-secrets-1.8.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:34:18.689746 cdk-sops-secrets-1.8.8/src/cdk_sops_secrets/
--rw-r--r--   0 runner    (1001) docker     (127)    80660 2024-05-25 21:34:08.000000 cdk-sops-secrets-1.8.8/src/cdk_sops_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:34:18.689746 cdk-sops-secrets-1.8.8/src/cdk_sops_secrets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-25 21:34:08.000000 cdk-sops-secrets-1.8.8/src/cdk_sops_secrets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  8974134 2024-05-25 21:34:08.000000 cdk-sops-secrets-1.8.8/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.8.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 21:34:08.000000 cdk-sops-secrets-1.8.8/src/cdk_sops_secrets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:34:18.689746 cdk-sops-secrets-1.8.8/src/cdk_sops_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-25 21:34:18.000000 cdk-sops-secrets-1.8.8/src/cdk_sops_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-25 21:34:18.000000 cdk-sops-secrets-1.8.8/src/cdk_sops_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 21:34:18.000000 cdk-sops-secrets-1.8.8/src/cdk_sops_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-25 21:34:18.000000 cdk-sops-secrets-1.8.8/src/cdk_sops_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-25 21:34:18.000000 cdk-sops-secrets-1.8.8/src/cdk_sops_secrets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:32:30.199334 cdk-sops-secrets-1.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-28 11:32:18.000000 cdk-sops-secrets-1.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 11:32:18.000000 cdk-sops-secrets-1.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-28 11:32:30.199334 cdk-sops-secrets-1.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-05-28 11:32:18.000000 cdk-sops-secrets-1.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-28 11:32:18.000000 cdk-sops-secrets-1.8.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:32:30.199334 cdk-sops-secrets-1.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-28 11:32:18.000000 cdk-sops-secrets-1.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:32:30.183334 cdk-sops-secrets-1.8.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:32:30.187334 cdk-sops-secrets-1.8.9/src/cdk_sops_secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)    80660 2024-05-28 11:32:18.000000 cdk-sops-secrets-1.8.9/src/cdk_sops_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:32:30.187334 cdk-sops-secrets-1.8.9/src/cdk_sops_secrets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-28 11:32:18.000000 cdk-sops-secrets-1.8.9/src/cdk_sops_secrets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  8974067 2024-05-28 11:32:18.000000 cdk-sops-secrets-1.8.9/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.8.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:32:18.000000 cdk-sops-secrets-1.8.9/src/cdk_sops_secrets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:32:30.187334 cdk-sops-secrets-1.8.9/src/cdk_sops_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-28 11:32:30.000000 cdk-sops-secrets-1.8.9/src/cdk_sops_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-28 11:32:30.000000 cdk-sops-secrets-1.8.9/src/cdk_sops_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:32:30.000000 cdk-sops-secrets-1.8.9/src/cdk_sops_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 11:32:30.000000 cdk-sops-secrets-1.8.9/src/cdk_sops_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 11:32:30.000000 cdk-sops-secrets-1.8.9/src/cdk_sops_secrets.egg-info/top_level.txt
```

### Comparing `cdk-sops-secrets-1.8.8/LICENSE` & `cdk-sops-secrets-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.8.8/PKG-INFO` & `cdk-sops-secrets-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.8.8
+Version: 1.8.9
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<markus.siebert@deutschebahn.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dbsystel/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-sops-secrets-1.8.8/README.md` & `cdk-sops-secrets-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.8.8/setup.py` & `cdk-sops-secrets-1.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-sops-secrets",
-    "version": "1.8.8",
+    "version": "1.8.9",
     "description": "CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.",
     "license": "Apache-2.0",
     "url": "https://constructs.dev/packages/cdk-sops-secrets",
     "long_description_content_type": "text/markdown",
     "author": "Markus Siebert<markus.siebert@deutschebahn.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_sops_secrets",
         "cdk_sops_secrets._jsii"
     ],
     "package_data": {
         "cdk_sops_secrets._jsii": [
-            "cdk-sops-secrets@1.8.8.jsii.tgz"
+            "cdk-sops-secrets@1.8.9.jsii.tgz"
         ],
         "cdk_sops_secrets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-sops-secrets-1.8.8/src/cdk_sops_secrets/__init__.py` & `cdk-sops-secrets-1.8.9/src/cdk_sops_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.8.8/src/cdk_sops_secrets.egg-info/PKG-INFO` & `cdk-sops-secrets-1.8.9/src/cdk_sops_secrets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.8.8
+Version: 1.8.9
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<markus.siebert@deutschebahn.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dbsystel/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

