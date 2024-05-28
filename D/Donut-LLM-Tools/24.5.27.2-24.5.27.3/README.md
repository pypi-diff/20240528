# Comparing `tmp/donut_llm_tools-24.5.27.2.tar.gz` & `tmp/donut_llm_tools-24.5.27.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donut_llm_tools-24.5.27.2.tar", last modified: Mon May 27 14:09:53 2024, max compression
+gzip compressed data, was "donut_llm_tools-24.5.27.3.tar", last modified: Mon May 27 14:42:03 2024, max compression
```

## Comparing `donut_llm_tools-24.5.27.2.tar` & `donut_llm_tools-24.5.27.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 14:09:53.272962 donut_llm_tools-24.5.27.2/
--rw-rw-rw-   0        0        0     1092 2024-05-27 14:06:29.000000 donut_llm_tools-24.5.27.2/LICENSE
--rw-rw-rw-   0        0        0     3821 2024-05-27 14:09:53.271201 donut_llm_tools-24.5.27.2/PKG-INFO
--rw-rw-rw-   0        0        0     1980 2024-05-27 14:08:08.000000 donut_llm_tools-24.5.27.2/README
--rw-rw-rw-   0        0        0      795 2024-05-27 14:06:38.000000 donut_llm_tools-24.5.27.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 14:09:53.274890 donut_llm_tools-24.5.27.2/setup.cfg
--rw-rw-rw-   0        0        0      361 2024-05-27 13:48:31.000000 donut_llm_tools-24.5.27.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 14:09:53.217221 donut_llm_tools-24.5.27.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-27 14:09:53.269182 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/
--rw-rw-rw-   0        0        0     3821 2024-05-27 14:09:53.000000 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-05-27 14:09:53.000000 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 14:09:53.000000 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-27 14:09:53.000000 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2024-05-27 14:09:53.000000 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-27 14:09:53.000000 donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3868 2024-05-27 14:07:27.000000 donut_llm_tools-24.5.27.2/src/donutllmtools.py
+drwxrwxrwx   0        0        0        0 2024-05-27 14:42:03.191395 donut_llm_tools-24.5.27.3/
+-rw-rw-rw-   0        0        0     1088 2024-05-27 14:40:00.000000 donut_llm_tools-24.5.27.3/LICENSE
+-rw-rw-rw-   0        0        0     3771 2024-05-27 14:42:03.099757 donut_llm_tools-24.5.27.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1980 2024-05-27 14:39:47.000000 donut_llm_tools-24.5.27.3/README
+-rw-rw-rw-   0        0        0      700 2024-05-27 14:40:40.000000 donut_llm_tools-24.5.27.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 14:42:03.191395 donut_llm_tools-24.5.27.3/setup.cfg
+-rw-rw-rw-   0        0        0      361 2024-05-27 13:48:31.000000 donut_llm_tools-24.5.27.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 14:42:03.056142 donut_llm_tools-24.5.27.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-27 14:42:03.098666 donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/
+-rw-rw-rw-   0        0        0     3771 2024-05-27 14:42:02.000000 donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-27 14:42:03.000000 donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 14:42:02.000000 donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-27 14:42:02.000000 donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-27 14:42:02.000000 donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3868 2024-05-27 14:07:27.000000 donut_llm_tools-24.5.27.3/src/donutllmtools.py
```

### Comparing `donut_llm_tools-24.5.27.2/LICENSE` & `donut_llm_tools-24.5.27.3/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [2024] [Gautham Nair]
+Copyright (c) 2024 Gautham Nair
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `donut_llm_tools-24.5.27.2/PKG-INFO` & `donut_llm_tools-24.5.27.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: Donut-LLM-Tools
-Version: 24.5.27.2
+Version: 24.5.27.3
 Summary: Tools for Creating Datasets and Models locally
 Author-email: Gautham Nair <gautham.nair.2005@gmail.com>
 License: MIT License
         
-        Copyright (c) [2024] [Gautham Nair]
+        Copyright (c) 2024 Gautham Nair
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -21,28 +21,27 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/gauthamnair2005/donut-llm-tools
-Keywords: feed,reader,tutorial
+Keywords: AI,trainer,dataset
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: CreateLLM
 Requires-Dist: Wikipedia
 
 # Donut LLM Tools
 Donut LLM Tools is a suite of two programs that helps you create dataset from wikipedia data and your own LLM with the created or already existing dataset.
 
-*Latest Version 24.05.27 Update 2*
+*Latest Version 24.05.27 Update 3*
 
 ## How to install, import and use DonutLLM?
 ### Installation
 * Before installing Donut LLM Tools, make sure you have Python `3.9` or later till Python `3.11`. *Note : Python `3.12` is not supported by PyTorch, hence Donut LLM Tools will also have troubles running.* 
 * The dependencies for installing Donut LLM Tools are:
     1. CreateLLM (`pip install CreateLLM`)
     2. torch (Required by CreateLLM)
```

### Comparing `donut_llm_tools-24.5.27.2/README` & `donut_llm_tools-24.5.27.3/README`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Donut LLM Tools
 Donut LLM Tools is a suite of two programs that helps you create dataset from wikipedia data and your own LLM with the created or already existing dataset.
 
-*Latest Version 24.05.27 Update 2*
+*Latest Version 24.05.27 Update 3*
 
 ## How to install, import and use DonutLLM?
 ### Installation
 * Before installing Donut LLM Tools, make sure you have Python `3.9` or later till Python `3.11`. *Note : Python `3.12` is not supported by PyTorch, hence Donut LLM Tools will also have troubles running.* 
 * The dependencies for installing Donut LLM Tools are:
     1. CreateLLM (`pip install CreateLLM`)
     2. torch (Required by CreateLLM)
```

### Comparing `donut_llm_tools-24.5.27.2/pyproject.toml` & `donut_llm_tools-24.5.27.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -2,29 +2,25 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Donut-LLM-Tools"
-version = "24.05.27.2"
+version = "24.05.27.3"
 description = "Tools for Creating Datasets and Models locally"
 readme = "README"
 authors = [{ name = "Gautham Nair", email = "gautham.nair.2005@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-keywords = ["feed", "reader", "tutorial"]
+keywords = ["AI", "trainer", "dataset"]
 dependencies = [
     "CreateLLM",
     "Wikipedia",
 ]
 requires-python = ">=3.11"
 
 [project.urls]
-Homepage = "https://github.com/gauthamnair2005/donut-llm-tools"
-
-[project.scripts]
-donutllmtools = "donutllmtools"
+Homepage = "https://github.com/gauthamnair2005/donut-llm-tools"
```

### Comparing `donut_llm_tools-24.5.27.2/src/Donut_LLM_Tools.egg-info/PKG-INFO` & `donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: Donut-LLM-Tools
-Version: 24.5.27.2
+Version: 24.5.27.3
 Summary: Tools for Creating Datasets and Models locally
 Author-email: Gautham Nair <gautham.nair.2005@gmail.com>
 License: MIT License
         
-        Copyright (c) [2024] [Gautham Nair]
+        Copyright (c) 2024 Gautham Nair
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -21,28 +21,27 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/gauthamnair2005/donut-llm-tools
-Keywords: feed,reader,tutorial
+Keywords: AI,trainer,dataset
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: CreateLLM
 Requires-Dist: Wikipedia
 
 # Donut LLM Tools
 Donut LLM Tools is a suite of two programs that helps you create dataset from wikipedia data and your own LLM with the created or already existing dataset.
 
-*Latest Version 24.05.27 Update 2*
+*Latest Version 24.05.27 Update 3*
 
 ## How to install, import and use DonutLLM?
 ### Installation
 * Before installing Donut LLM Tools, make sure you have Python `3.9` or later till Python `3.11`. *Note : Python `3.12` is not supported by PyTorch, hence Donut LLM Tools will also have troubles running.* 
 * The dependencies for installing Donut LLM Tools are:
     1. CreateLLM (`pip install CreateLLM`)
     2. torch (Required by CreateLLM)
```

### Comparing `donut_llm_tools-24.5.27.2/src/donutllmtools.py` & `donut_llm_tools-24.5.27.3/src/donutllmtools.py`

 * *Files identical despite different names*

