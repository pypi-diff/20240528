# Comparing `tmp/llama_index_llms_unionllm-0.1.1.tar.gz` & `tmp/llama_index_llms_unionllm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_unionllm-0.1.1.tar", last modified: Tue May 21 09:14:25 2024, max compression
+gzip compressed data, was "llama_index_llms_unionllm-0.1.2.tar", last modified: Tue May 28 10:19:50 2024, max compression
```

## Comparing `llama_index_llms_unionllm-0.1.1.tar` & `llama_index_llms_unionllm-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 09:14:25.633933 llama_index_llms_unionllm-0.1.1/
--rw-r--r--   0 everfly    (501) wheel        (0)      461 2024-05-21 09:14:25.633761 llama_index_llms_unionllm-0.1.1/PKG-INFO
--rw-r--r--   0 everfly    (501) wheel        (0)       40 2024-05-19 06:04:32.000000 llama_index_llms_unionllm-0.1.1/README.md
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 09:14:25.633560 llama_index_llms_unionllm-0.1.1/llama_index_llms_unionllm.egg-info/
--rw-r--r--   0 everfly    (501) wheel        (0)      461 2024-05-21 09:14:25.000000 llama_index_llms_unionllm-0.1.1/llama_index_llms_unionllm.egg-info/PKG-INFO
--rw-r--r--   0 everfly    (501) wheel        (0)      277 2024-05-21 09:14:25.000000 llama_index_llms_unionllm-0.1.1/llama_index_llms_unionllm.egg-info/SOURCES.txt
--rw-r--r--   0 everfly    (501) wheel        (0)        1 2024-05-21 09:14:25.000000 llama_index_llms_unionllm-0.1.1/llama_index_llms_unionllm.egg-info/dependency_links.txt
--rw-r--r--   0 everfly    (501) wheel        (0)       12 2024-05-21 09:14:25.000000 llama_index_llms_unionllm-0.1.1/llama_index_llms_unionllm.egg-info/requires.txt
--rw-r--r--   0 everfly    (501) wheel        (0)        1 2024-05-21 09:14:25.000000 llama_index_llms_unionllm-0.1.1/llama_index_llms_unionllm.egg-info/top_level.txt
--rw-r--r--   0 everfly    (501) wheel        (0)     1450 2024-05-19 06:08:28.000000 llama_index_llms_unionllm-0.1.1/pyproject.toml
--rw-r--r--   0 everfly    (501) wheel        (0)       38 2024-05-21 09:14:25.633966 llama_index_llms_unionllm-0.1.1/setup.cfg
--rw-r--r--   0 everfly    (501) wheel        (0)      643 2024-05-21 09:14:11.000000 llama_index_llms_unionllm-0.1.1/setup.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-28 10:19:50.353307 llama_index_llms_unionllm-0.1.2/
+-rw-r--r--   0 everfly    (501) wheel        (0)      461 2024-05-28 10:19:50.353137 llama_index_llms_unionllm-0.1.2/PKG-INFO
+-rw-r--r--   0 everfly    (501) wheel        (0)       40 2024-05-19 06:04:32.000000 llama_index_llms_unionllm-0.1.2/README.md
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-28 10:19:50.352935 llama_index_llms_unionllm-0.1.2/llama_index_llms_unionllm.egg-info/
+-rw-r--r--   0 everfly    (501) wheel        (0)      461 2024-05-28 10:19:50.000000 llama_index_llms_unionllm-0.1.2/llama_index_llms_unionllm.egg-info/PKG-INFO
+-rw-r--r--   0 everfly    (501) wheel        (0)      277 2024-05-28 10:19:50.000000 llama_index_llms_unionllm-0.1.2/llama_index_llms_unionllm.egg-info/SOURCES.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)        1 2024-05-28 10:19:50.000000 llama_index_llms_unionllm-0.1.2/llama_index_llms_unionllm.egg-info/dependency_links.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)       12 2024-05-28 10:19:50.000000 llama_index_llms_unionllm-0.1.2/llama_index_llms_unionllm.egg-info/requires.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)        1 2024-05-28 10:19:50.000000 llama_index_llms_unionllm-0.1.2/llama_index_llms_unionllm.egg-info/top_level.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)     1450 2024-05-28 10:19:44.000000 llama_index_llms_unionllm-0.1.2/pyproject.toml
+-rw-r--r--   0 everfly    (501) wheel        (0)       38 2024-05-28 10:19:50.353344 llama_index_llms_unionllm-0.1.2/setup.cfg
+-rw-r--r--   0 everfly    (501) wheel        (0)      643 2024-05-28 10:19:17.000000 llama_index_llms_unionllm-0.1.2/setup.py
```

### Comparing `llama_index_llms_unionllm-0.1.1/pyproject.toml` & `llama_index_llms_unionllm-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["everfly <tagriver@gmail.com>"]
 description = "llama-index llms unionllm integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-unionllm"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 unionllm = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_llms_unionllm-0.1.1/setup.py` & `llama_index_llms_unionllm-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='llama-index-llms-unionllm',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'llama-index',
         # 其他依赖项
     ],
     author='Your Name',
     author_email='your.email@example.com',
```

