# Comparing `tmp/fastsupabased_acl-0.1.0.tar.gz` & `tmp/fastsupabased_acl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastsupabased_acl-0.1.0.tar", max compression
+gzip compressed data, was "fastsupabased_acl-0.1.1.tar", max compression
```

## Comparing `fastsupabased_acl-0.1.0.tar` & `fastsupabased_acl-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      783 2024-05-26 19:35:18.368939 fastsupabased_acl-0.1.0/README.md
--rw-r--r--   0        0        0       18 2024-05-26 19:35:18.368939 fastsupabased_acl-0.1.0/fastsupabased_acl/__init__.py
--rw-r--r--   0        0        0      904 2024-05-26 19:35:18.368939 fastsupabased_acl-0.1.0/fastsupabased_acl/main.py
--rw-r--r--   0        0        0      402 2024-05-26 19:35:18.368939 fastsupabased_acl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 fastsupabased_acl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      783 2024-05-28 13:02:19.851944 fastsupabased_acl-0.1.1/README.md
+-rw-r--r--   0        0        0      904 2024-05-28 13:02:19.851944 fastsupabased_acl-0.1.1/fastsupabased_acl/__init__.py
+-rw-r--r--   0        0        0      402 2024-05-28 13:02:19.851944 fastsupabased_acl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 fastsupabased_acl-0.1.1/PKG-INFO
```

### Comparing `fastsupabased_acl-0.1.0/README.md` & `fastsupabased_acl-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fastsupabased_acl-0.1.0/fastsupabased_acl/main.py` & `fastsupabased_acl-0.1.1/fastsupabased_acl/__init__.py`

 * *Files identical despite different names*

### Comparing `fastsupabased_acl-0.1.0/PKG-INFO` & `fastsupabased_acl-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsupabased-acl
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastAPI Dependency for Supabase-based ACL using Supabase Roles
 Author: Vinicius Mesel
 Author-email: 4984147+vmesel@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

