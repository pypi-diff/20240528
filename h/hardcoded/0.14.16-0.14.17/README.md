# Comparing `tmp/hardcoded-0.14.16.tar.gz` & `tmp/hardcoded-0.14.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardcoded-0.14.16.tar", max compression
+gzip compressed data, was "hardcoded-0.14.17.tar", max compression
```

## Comparing `hardcoded-0.14.16.tar` & `hardcoded-0.14.17.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1871 2024-05-28 19:57:09.065958 hardcoded-0.14.16/README.md
--rw-r--r--   0        0        0     1177 2024-05-21 20:05:41.903335 hardcoded-0.14.16/hardcoded/__init__.py
--rw-r--r--   0        0        0     3394 2024-05-28 19:37:43.326688 hardcoded-0.14.16/hardcoded/cli.py
--rw-r--r--   0        0        0     1414 2024-05-21 19:41:50.996478 hardcoded-0.14.16/hardcoded/git.py
--rw-r--r--   0        0        0    25781 2024-05-22 08:24:07.526500 hardcoded-0.14.16/hardcoded/logic.py
--rw-r--r--   0        0        0      692 2024-05-28 20:01:23.865062 hardcoded-0.14.16/pyproject.toml
--rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 hardcoded-0.14.16/PKG-INFO
+-rw-r--r--   0        0        0     1871 2024-05-28 19:57:09.065958 hardcoded-0.14.17/README.md
+-rw-r--r--   0        0        0     1177 2024-05-21 20:05:41.903335 hardcoded-0.14.17/hardcoded/__init__.py
+-rw-r--r--   0        0        0     3394 2024-05-28 19:37:43.326688 hardcoded-0.14.17/hardcoded/cli.py
+-rw-r--r--   0        0        0     1414 2024-05-21 19:41:50.996478 hardcoded-0.14.17/hardcoded/git.py
+-rw-r--r--   0        0        0    25781 2024-05-22 08:24:07.526500 hardcoded-0.14.17/hardcoded/logic.py
+-rw-r--r--   0        0        0      692 2024-05-28 20:25:38.313375 hardcoded-0.14.17/pyproject.toml
+-rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 hardcoded-0.14.17/PKG-INFO
```

### Comparing `hardcoded-0.14.16/README.md` & `hardcoded-0.14.17/README.md`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.16/hardcoded/__init__.py` & `hardcoded-0.14.17/hardcoded/__init__.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.16/hardcoded/cli.py` & `hardcoded-0.14.17/hardcoded/cli.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.16/hardcoded/git.py` & `hardcoded-0.14.17/hardcoded/git.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.16/hardcoded/logic.py` & `hardcoded-0.14.17/hardcoded/logic.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.14.16/pyproject.toml` & `hardcoded-0.14.17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hardcoded"
-version = "0.14.16"
+version = "0.14.17"
 description = "For everything that you really should not be hardcoding."
 license = "LGPL-3.0-or-later"
 authors = ["moizuo <no_spam@example.com>"]
 readme = "README.md"
 homepage = "https://gitlab.com/zeroconfig/hardcoded"
 
 [tool.poetry.dependencies]
```

### Comparing `hardcoded-0.14.16/PKG-INFO` & `hardcoded-0.14.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardcoded
-Version: 0.14.16
+Version: 0.14.17
 Summary: For everything that you really should not be hardcoding.
 Home-page: https://gitlab.com/zeroconfig/hardcoded
 License: LGPL-3.0-or-later
 Author: moizuo
 Author-email: no_spam@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

