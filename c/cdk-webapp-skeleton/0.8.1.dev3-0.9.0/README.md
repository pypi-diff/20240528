# Comparing `tmp/cdk_webapp_skeleton-0.8.1.dev3.tar.gz` & `tmp/cdk_webapp_skeleton-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_webapp_skeleton-0.8.1.dev3.tar", max compression
+gzip compressed data, was "cdk_webapp_skeleton-0.9.0.tar", max compression
```

## Comparing `cdk_webapp_skeleton-0.8.1.dev3.tar` & `cdk_webapp_skeleton-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       64 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/README.md
--rw-r--r--   0        0        0      463 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/__init__.py
--rw-r--r--   0        0        0     4144 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/auth_stack.py
--rw-r--r--   0        0        0     3070 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/branch_cicd_pipeline.py
--rw-r--r--   0        0        0     2996 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/branch_config.py
--rw-r--r--   0        0        0     4714 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/monitored_lambda_function.py
--rw-r--r--   0        0        0        0 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/py.typed
--rw-r--r--   0        0        0     4775 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/react_website.py
--rw-r--r--   0        0        0      447 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/test_utils.py
--rw-r--r--   0        0        0     5191 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/webapp_lambda.py
--rw-r--r--   0        0        0     1514 2024-05-28 04:03:28.536931 cdk_webapp_skeleton-0.8.1.dev3/pyproject.toml
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.8.1.dev3/PKG-INFO
+-rw-r--r--   0        0        0       64 2024-05-28 04:04:56.404765 cdk_webapp_skeleton-0.9.0/README.md
+-rw-r--r--   0        0        0      463 2024-05-28 04:04:56.404765 cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/__init__.py
+-rw-r--r--   0        0        0     4144 2024-05-28 04:04:56.404765 cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/auth_stack.py
+-rw-r--r--   0        0        0     3070 2024-05-28 04:04:56.404765 cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/branch_cicd_pipeline.py
+-rw-r--r--   0        0        0     2996 2024-05-28 04:04:56.404765 cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/branch_config.py
+-rw-r--r--   0        0        0     4714 2024-05-28 04:04:56.404765 cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/monitored_lambda_function.py
+-rw-r--r--   0        0        0        0 2024-05-28 04:04:56.404765 cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/py.typed
+-rw-r--r--   0        0        0     4775 2024-05-28 04:04:56.404765 cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/react_website.py
+-rw-r--r--   0        0        0      447 2024-05-28 04:04:56.404765 cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/test_utils.py
+-rw-r--r--   0        0        0     5191 2024-05-28 04:04:56.404765 cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/webapp_lambda.py
+-rw-r--r--   0        0        0     1509 2024-05-28 04:05:13.704729 cdk_webapp_skeleton-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.9.0/PKG-INFO
```

### Comparing `cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/auth_stack.py` & `cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/auth_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/branch_cicd_pipeline.py` & `cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/branch_cicd_pipeline.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/branch_config.py` & `cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/branch_config.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/monitored_lambda_function.py` & `cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/monitored_lambda_function.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/react_website.py` & `cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/react_website.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/webapp_lambda.py` & `cdk_webapp_skeleton-0.9.0/cdk_webapp_skeleton/webapp_lambda.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.8.1.dev3/pyproject.toml` & `cdk_webapp_skeleton-0.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdk-webapp-skeleton"
-version = "0.8.1.dev3"
+version = "0.9.0"
 description = ""
 authors = ["Ilya Nekhay <nekhayiv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cdk_webapp_skeleton"}]
 
 [tool.poetry.dependencies]
 python = " >=3.8.1,<4"
```

### Comparing `cdk_webapp_skeleton-0.8.1.dev3/PKG-INFO` & `cdk_webapp_skeleton-0.9.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-webapp-skeleton
-Version: 0.8.1.dev3
+Version: 0.9.0
 Summary: 
 Author: Ilya Nekhay
 Author-email: nekhayiv@gmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

