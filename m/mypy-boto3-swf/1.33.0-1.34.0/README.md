# Comparing `tmp/mypy-boto3-swf-1.33.0.tar.gz` & `tmp/mypy-boto3-swf-1.34.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-swf-1.33.0.tar", last modified: Tue Nov 28 18:30:38 2023, max compression
+gzip compressed data, was "mypy-boto3-swf-1.34.0.tar", last modified: Wed Dec 13 21:24:00 2023, max compression
```

## Comparing `mypy-boto3-swf-1.33.0.tar` & `mypy-boto3-swf-1.34.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:30:38.182581 mypy-boto3-swf-1.33.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-11-28 18:27:09.000000 mypy-boto3-swf-1.33.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13468 2023-11-28 18:30:38.182581 mypy-boto3-swf-1.33.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2023-11-28 18:27:09.000000 mypy-boto3-swf-1.33.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:30:38.178581 mypy-boto3-swf-1.33.0/mypy_boto3_swf/
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-11-28 18:27:09.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2023-11-28 18:27:09.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-11-28 18:27:09.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31240 2023-11-28 18:27:09.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    31236 2023-11-28 18:27:09.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16430 2023-11-28 18:27:10.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16428 2023-11-28 18:27:10.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2023-11-28 18:27:10.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2023-11-28 18:27:10.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 18:27:09.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    60541 2023-11-28 18:27:15.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    60540 2023-11-28 18:27:14.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-28 18:27:09.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:30:38.182581 mypy-boto3-swf-1.33.0/mypy_boto3_swf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13468 2023-11-28 18:30:38.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-11-28 18:30:38.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 18:30:38.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 18:30:38.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-28 18:30:38.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-28 18:30:38.000000 mypy-boto3-swf-1.33.0/mypy_boto3_swf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 18:30:38.182581 mypy-boto3-swf-1.33.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-11-28 18:27:09.000000 mypy-boto3-swf-1.33.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:00.395400 mypy-boto3-swf-1.34.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13468 2023-12-13 21:24:00.395400 mypy-boto3-swf-1.34.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:00.395400 mypy-boto3-swf-1.34.0/mypy_boto3_swf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31240 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31236 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16590 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9714 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    60541 2023-12-13 21:20:38.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60540 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:20:37.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:00.395400 mypy-boto3-swf-1.34.0/mypy_boto3_swf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13468 2023-12-13 21:24:00.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2023-12-13 21:24:00.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:24:00.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:24:00.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:24:00.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-13 21:24:00.000000 mypy-boto3-swf-1.34.0/mypy_boto3_swf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:24:00.395400 mypy-boto3-swf-1.34.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-12-13 21:20:36.000000 mypy-boto3-swf-1.34.0/setup.py
```

### Comparing `mypy-boto3-swf-1.33.0/LICENSE` & `mypy-boto3-swf-1.34.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.33.0/PKG-INFO` & `mypy-boto3-swf-1.34.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-swf
-Version: 1.33.0
-Summary: Type annotations for boto3.SWF 1.33.0 service generated with mypy-boto3-builder 7.20.3
+Version: 1.34.0
+Summary: Type annotations for boto3.SWF 1.34.0 service generated with mypy-boto3-builder 7.21.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-swf)](https://pepy.tech/project/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.33.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.20.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-swf-1.33.0/README.md` & `mypy-boto3-swf-1.34.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-swf)](https://pepy.tech/project/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.33.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.20.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf/__init__.py` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf/__init__.pyi` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf/__main__.py` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SWF 1.33.0\nVersion:         1.33.0\nBuilder version:"
-        " 7.20.3\nDocs:           "
+        "Type annotations for boto3.SWF 1.34.0\nVersion:         1.34.0\nBuilder version:"
+        " 7.21.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.33.0")
+    print("1.34.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf/client.py` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf/client.pyi` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf/literals.py` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,26 +256,29 @@
     "b2bi",
     "backup",
     "backup-gateway",
     "backupstorage",
     "batch",
     "bcm-data-exports",
     "bedrock",
+    "bedrock-agent",
+    "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
+    "cleanroomsml",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudfront-keyvaluestore",
     "cloudhsm",
@@ -435,15 +438,17 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
     "managedblockchain",
     "managedblockchain-query",
+    "marketplace-agreement",
     "marketplace-catalog",
+    "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
@@ -491,14 +496,16 @@
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
     "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
+    "qbusiness",
+    "qconnect",
     "qldb",
     "qldb-session",
     "quicksight",
     "ram",
     "rbin",
     "rds",
     "rds-data",
```

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf/literals.pyi` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -254,26 +254,29 @@
     "b2bi",
     "backup",
     "backup-gateway",
     "backupstorage",
     "batch",
     "bcm-data-exports",
     "bedrock",
+    "bedrock-agent",
+    "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
+    "cleanroomsml",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudfront-keyvaluestore",
     "cloudhsm",
@@ -433,15 +436,17 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
     "managedblockchain",
     "managedblockchain-query",
+    "marketplace-agreement",
     "marketplace-catalog",
+    "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
@@ -489,14 +494,16 @@
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
     "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
+    "qbusiness",
+    "qconnect",
     "qldb",
     "qldb-session",
     "quicksight",
     "ram",
     "rbin",
     "rds",
     "rds-data",
```

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf/paginator.py` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf/paginator.pyi` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf/type_defs.py` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf/type_defs.pyi` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf.egg-info/PKG-INFO` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-swf
-Version: 1.33.0
-Summary: Type annotations for boto3.SWF 1.33.0 service generated with mypy-boto3-builder 7.20.3
+Version: 1.34.0
+Summary: Type annotations for boto3.SWF 1.34.0 service generated with mypy-boto3-builder 7.21.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-swf)](https://pepy.tech/project/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.33.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.20.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-swf-1.33.0/mypy_boto3_swf.egg-info/SOURCES.txt` & `mypy-boto3-swf-1.34.0/mypy_boto3_swf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.33.0/setup.py` & `mypy-boto3-swf-1.34.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-swf",
-    version="1.33.0",
+    version="1.34.0",
     packages=["mypy_boto3_swf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SWF 1.33.0 service generated with mypy-boto3-builder 7.20.3"
+        "Type annotations for boto3.SWF 1.34.0 service generated with mypy-boto3-builder 7.21.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

