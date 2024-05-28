# Comparing `tmp/muffin_sentry-1.8.0.tar.gz` & `tmp/muffin_sentry-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_sentry-1.8.0.tar", max compression
+gzip compressed data, was "muffin_sentry-1.8.1.tar", max compression
```

## Comparing `muffin_sentry-1.8.0.tar` & `muffin_sentry-1.8.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3841 2023-10-11 09:12:07.326746 muffin_sentry-1.8.0/README.rst
--rw-r--r--   0        0        0       91 2023-10-11 09:12:07.326746 muffin_sentry-1.8.0/muffin_sentry/__init__.py
--rw-r--r--   0        0        0     4896 2023-10-11 09:12:07.326746 muffin_sentry-1.8.0/muffin_sentry/plugin.py
--rw-r--r--   0        0        0        0 2023-10-11 09:12:07.326746 muffin_sentry-1.8.0/muffin_sentry/py.typed
--rw-r--r--   0        0        0     1928 2023-10-11 09:12:07.326746 muffin_sentry-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     4853 1970-01-01 00:00:00.000000 muffin_sentry-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     3841 2023-10-11 14:17:13.976949 muffin_sentry-1.8.1/README.rst
+-rw-r--r--   0        0        0      111 2023-10-11 14:17:13.976949 muffin_sentry-1.8.1/muffin_sentry/__init__.py
+-rw-r--r--   0        0        0     4896 2023-10-11 14:17:13.976949 muffin_sentry-1.8.1/muffin_sentry/plugin.py
+-rw-r--r--   0        0        0        0 2023-10-11 14:17:13.976949 muffin_sentry-1.8.1/muffin_sentry/py.typed
+-rw-r--r--   0        0        0     1928 2023-10-11 14:17:13.980949 muffin_sentry-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4853 1970-01-01 00:00:00.000000 muffin_sentry-1.8.1/PKG-INFO
```

### Comparing `muffin_sentry-1.8.0/README.rst` & `muffin_sentry-1.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_sentry-1.8.0/muffin_sentry/plugin.py` & `muffin_sentry-1.8.1/muffin_sentry/plugin.py`

 * *Files identical despite different names*

### Comparing `muffin_sentry-1.8.0/pyproject.toml` & `muffin_sentry-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-sentry"
-version = "1.8.0"
+version = "1.8.1"
 description = "Sentry Integration for Muffin framework"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 homepage = "https://github.com/klen/muffin-sentry"
 repository = "https://github.com/klen/muffin-sentry"
 keywords = ["sentry", "asyncio", "trio", "asgi", "muffin"]
```

### Comparing `muffin_sentry-1.8.0/PKG-INFO` & `muffin_sentry-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-sentry
-Version: 1.8.0
+Version: 1.8.1
 Summary: Sentry Integration for Muffin framework
 Home-page: https://github.com/klen/muffin-sentry
 License: MIT
 Keywords: sentry,asyncio,trio,asgi,muffin
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

