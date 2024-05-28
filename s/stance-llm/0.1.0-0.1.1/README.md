# Comparing `tmp/stance_llm-0.1.0.tar.gz` & `tmp/stance_llm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stance_llm-0.1.0.tar", max compression
+gzip compressed data, was "stance_llm-0.1.1.tar", max compression
```

## Comparing `stance_llm-0.1.0.tar` & `stance_llm-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      798 2024-05-28 12:55:58.820897 stance_llm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      159 2024-05-21 10:15:09.089582 stance_llm-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-21 08:56:17.968717 stance_llm-0.1.0/stance_llm/__init__.py
--rw-r--r--   0        0        0    38960 2024-05-28 15:17:16.461482 stance_llm-0.1.0/stance_llm/base.py
--rw-r--r--   0        0        0    16415 2024-05-28 12:55:58.822898 stance_llm-0.1.0/stance_llm/process.py
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 stance_llm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1111 2024-05-21 09:34:20.112894 stance_llm-0.1.1/LICENSE
+-rw-r--r--   0        0        0      876 2024-05-28 15:40:16.627975 stance_llm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      159 2024-05-28 15:33:30.070907 stance_llm-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 08:56:17.968717 stance_llm-0.1.1/src/stance_llm/__init__.py
+-rw-r--r--   0        0        0    38960 2024-05-28 15:17:16.461482 stance_llm-0.1.1/src/stance_llm/base.py
+-rw-r--r--   0        0        0    16415 2024-05-28 12:55:58.822898 stance_llm-0.1.1/src/stance_llm/process.py
+-rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 stance_llm-0.1.1/PKG-INFO
```

### Comparing `stance_llm-0.1.0/pyproject.toml` & `stance_llm-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "stance-llm"
-version = "0.1.0"
+version = "0.1.1"
 description = "Classify stances of entities related to a statement in German text using large language models through guidance-llm"
 authors = ["Mario Angst <mario.angst@uzh.ch>", "Viviane Walker <viviane.walker@uzh.ch>"]
 readme = "README.md"
+repository = "https://github.com/urban-sustainability-lab-zurich/stance-llm"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 guidance = "^0.1.10"
 loguru = "^0.7.2"
 tdqm = "^0.0.1"
 polars = "^0.20.15"
```

### Comparing `stance_llm-0.1.0/stance_llm/base.py` & `stance_llm-0.1.1/src/stance_llm/base.py`

 * *Files identical despite different names*

### Comparing `stance_llm-0.1.0/stance_llm/process.py` & `stance_llm-0.1.1/src/stance_llm/process.py`

 * *Files identical despite different names*

### Comparing `stance_llm-0.1.0/PKG-INFO` & `stance_llm-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: stance-llm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Classify stances of entities related to a statement in German text using large language models through guidance-llm
+Home-page: https://github.com/urban-sustainability-lab-zurich/stance-llm
 Author: Mario Angst
 Author-email: mario.angst@uzh.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: guidance (>=0.1.10,<0.2.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: polars (>=0.20.15,<0.21.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Requires-Dist: tdqm (>=0.0.1,<0.0.2)
 Requires-Dist: wonderwords (>=2.2.0,<3.0.0)
+Project-URL: Repository, https://github.com/urban-sustainability-lab-zurich/stance-llm
 Description-Content-Type: text/markdown
 
 # stance_llm
 
 A python package to classify stances of entities related to a statement in German text using large language models built on top of guidance-llm
```

