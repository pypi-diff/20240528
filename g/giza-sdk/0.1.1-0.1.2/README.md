# Comparing `tmp/giza_sdk-0.1.1.tar.gz` & `tmp/giza_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_sdk-0.1.1.tar", max compression
+gzip compressed data, was "giza_sdk-0.1.2.tar", max compression
```

## Comparing `giza_sdk-0.1.1.tar` & `giza_sdk-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1061 2024-05-23 09:42:13.144539 giza_sdk-0.1.1/LICENSE
--rw-r--r--   0        0        0     1154 2024-05-23 09:42:13.144539 giza_sdk-0.1.1/README.md
--rw-r--r--   0        0        0       21 2024-05-23 09:42:13.144539 giza_sdk-0.1.1/giza_sdk/__init__.py
--rw-r--r--   0        0        0      577 2024-05-23 09:42:13.144539 giza_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 giza_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-28 09:07:05.663366 giza_sdk-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1154 2024-05-28 09:07:05.663366 giza_sdk-0.1.2/README.md
+-rw-r--r--   0        0        0       21 2024-05-28 09:07:05.663366 giza_sdk-0.1.2/giza_sdk/__init__.py
+-rw-r--r--   0        0        0      577 2024-05-28 09:07:05.667366 giza_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 giza_sdk-0.1.2/PKG-INFO
```

### Comparing `giza_sdk-0.1.1/LICENSE` & `giza_sdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_sdk-0.1.1/README.md` & `giza_sdk-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `giza_sdk-0.1.1/pyproject.toml` & `giza_sdk-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "giza-sdk"
-version = "0.1.1"
+version = "0.1.2"
 description = "Metapackage for installing Giza packages"
 authors = ["Tu Nombre <tuemail@example.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gizatechxyz/giza-sdk"
 homepage = "https://github.com/gizatechxyz/giza-sdk"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 giza-cli = ">=0.17.0"
 giza-datasets = ">=0.3.0"
-giza-agents = ">=0.4.0"
+giza-agents = ">=0.4.2"
 giza-zkcook = "^0.2.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `giza_sdk-0.1.1/PKG-INFO` & `giza_sdk-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: giza-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Metapackage for installing Giza packages
 Home-page: https://github.com/gizatechxyz/giza-sdk
 License: MIT
 Author: Tu Nombre
 Author-email: tuemail@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: giza-agents (>=0.4.0)
+Requires-Dist: giza-agents (>=0.4.2)
 Requires-Dist: giza-cli (>=0.17.0)
 Requires-Dist: giza-datasets (>=0.3.0)
 Requires-Dist: giza-zkcook (>=0.2.1,<0.3.0)
 Project-URL: Repository, https://github.com/gizatechxyz/giza-sdk
 Description-Content-Type: text/markdown
 
 # giza-sdk
```

