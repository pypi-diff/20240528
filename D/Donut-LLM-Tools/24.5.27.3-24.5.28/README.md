# Comparing `tmp/donut_llm_tools-24.5.27.3.tar.gz` & `tmp/donut_llm_tools-24.5.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donut_llm_tools-24.5.27.3.tar", last modified: Mon May 27 14:42:03 2024, max compression
+gzip compressed data, was "donut_llm_tools-24.5.28.tar", last modified: Tue May 28 10:35:36 2024, max compression
```

## Comparing `donut_llm_tools-24.5.27.3.tar` & `donut_llm_tools-24.5.28.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 14:42:03.191395 donut_llm_tools-24.5.27.3/
--rw-rw-rw-   0        0        0     1088 2024-05-27 14:40:00.000000 donut_llm_tools-24.5.27.3/LICENSE
--rw-rw-rw-   0        0        0     3771 2024-05-27 14:42:03.099757 donut_llm_tools-24.5.27.3/PKG-INFO
--rw-rw-rw-   0        0        0     1980 2024-05-27 14:39:47.000000 donut_llm_tools-24.5.27.3/README
--rw-rw-rw-   0        0        0      700 2024-05-27 14:40:40.000000 donut_llm_tools-24.5.27.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 14:42:03.191395 donut_llm_tools-24.5.27.3/setup.cfg
--rw-rw-rw-   0        0        0      361 2024-05-27 13:48:31.000000 donut_llm_tools-24.5.27.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 14:42:03.056142 donut_llm_tools-24.5.27.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-27 14:42:03.098666 donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/
--rw-rw-rw-   0        0        0     3771 2024-05-27 14:42:02.000000 donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-27 14:42:03.000000 donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 14:42:02.000000 donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-27 14:42:02.000000 donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-27 14:42:02.000000 donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3868 2024-05-27 14:07:27.000000 donut_llm_tools-24.5.27.3/src/donutllmtools.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:35:36.637143 donut_llm_tools-24.5.28/
+-rw-rw-rw-   0        0        0     1088 2024-05-27 14:40:00.000000 donut_llm_tools-24.5.28/LICENSE
+-rw-rw-rw-   0        0        0     4036 2024-05-28 10:35:36.628861 donut_llm_tools-24.5.28/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2024-05-28 10:24:44.000000 donut_llm_tools-24.5.28/README.md
+-rw-rw-rw-   0        0        0     1327 2024-05-28 10:33:51.000000 donut_llm_tools-24.5.28/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 10:35:36.637143 donut_llm_tools-24.5.28/setup.cfg
+-rw-rw-rw-   0        0        0      491 2024-05-28 10:22:19.000000 donut_llm_tools-24.5.28/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:35:36.572667 donut_llm_tools-24.5.28/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 10:35:36.625849 donut_llm_tools-24.5.28/src/Donut_LLM_Tools.egg-info/
+-rw-rw-rw-   0        0        0     4036 2024-05-28 10:35:36.000000 donut_llm_tools-24.5.28/src/Donut_LLM_Tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-05-28 10:35:36.000000 donut_llm_tools-24.5.28/src/Donut_LLM_Tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 10:35:36.000000 donut_llm_tools-24.5.28/src/Donut_LLM_Tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-28 10:35:36.000000 donut_llm_tools-24.5.28/src/Donut_LLM_Tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-28 10:35:36.000000 donut_llm_tools-24.5.28/src/Donut_LLM_Tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3866 2024-05-28 10:27:03.000000 donut_llm_tools-24.5.28/src/donutllmtools.py
```

### Comparing `donut_llm_tools-24.5.27.3/LICENSE` & `donut_llm_tools-24.5.28/LICENSE`

 * *Files identical despite different names*

### Comparing `donut_llm_tools-24.5.27.3/PKG-INFO` & `donut_llm_tools-24.5.28/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: Donut-LLM-Tools
-Version: 24.5.27.3
-Summary: Tools for Creating Datasets and Models locally
-Author-email: Gautham Nair <gautham.nair.2005@gmail.com>
+Version: 24.5.28
+Summary: Tools for creating datasets, training and loading AI models
+Author: Gautham Nair
+Author-email: gautham.nair.2005@gmail.com
 License: MIT License
         
         Copyright (c) 2024 Gautham Nair
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -21,31 +22,38 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/gauthamnair2005/donut-llm-tools
-Keywords: AI,trainer,dataset
+Keywords: AI,ML,Train,Model,Dataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: GIUC
 Requires-Dist: CreateLLM
 Requires-Dist: Wikipedia
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpver; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # Donut LLM Tools
 Donut LLM Tools is a suite of two programs that helps you create dataset from wikipedia data and your own LLM with the created or already existing dataset.
 
-*Latest Version 24.05.27 Update 3*
+*Latest Version 24.05.28*
 
 ## How to install, import and use DonutLLM?
 ### Installation
-* Before installing Donut LLM Tools, make sure you have Python `3.9` or later till Python `3.11`. *Note : Python `3.12` is not supported by PyTorch, hence Donut LLM Tools will also have troubles running.* 
+* Before installing Donut LLM Tools, make sure you have Python `3.9` or later till Python `3.11`. *Note : Python `3.12` is not supported by PyTorch, hence Donut LLM Tools will also have trouble running in it.* 
 * The dependencies for installing Donut LLM Tools are:
     1. CreateLLM (`pip install CreateLLM`)
     2. torch (Required by CreateLLM)
     3. torchvision (Required by CreateLLM, PyTorch)
     4. torchaudio (Required by CreateLLM, PyTorch)
     5. Wikipedia
```

### Comparing `donut_llm_tools-24.5.27.3/README` & `donut_llm_tools-24.5.28/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Donut LLM Tools
 Donut LLM Tools is a suite of two programs that helps you create dataset from wikipedia data and your own LLM with the created or already existing dataset.
 
-*Latest Version 24.05.27 Update 3*
+*Latest Version 24.05.28*
 
 ## How to install, import and use DonutLLM?
 ### Installation
-* Before installing Donut LLM Tools, make sure you have Python `3.9` or later till Python `3.11`. *Note : Python `3.12` is not supported by PyTorch, hence Donut LLM Tools will also have troubles running.* 
+* Before installing Donut LLM Tools, make sure you have Python `3.9` or later till Python `3.11`. *Note : Python `3.12` is not supported by PyTorch, hence Donut LLM Tools will also have trouble running in it.* 
 * The dependencies for installing Donut LLM Tools are:
     1. CreateLLM (`pip install CreateLLM`)
     2. torch (Required by CreateLLM)
     3. torchvision (Required by CreateLLM, PyTorch)
     4. torchaudio (Required by CreateLLM, PyTorch)
     5. Wikipedia
```

### Comparing `donut_llm_tools-24.5.27.3/src/Donut_LLM_Tools.egg-info/PKG-INFO` & `donut_llm_tools-24.5.28/src/Donut_LLM_Tools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: Donut-LLM-Tools
-Version: 24.5.27.3
-Summary: Tools for Creating Datasets and Models locally
-Author-email: Gautham Nair <gautham.nair.2005@gmail.com>
+Version: 24.5.28
+Summary: Tools for creating datasets, training and loading AI models
+Author: Gautham Nair
+Author-email: gautham.nair.2005@gmail.com
 License: MIT License
         
         Copyright (c) 2024 Gautham Nair
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -21,31 +22,38 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/gauthamnair2005/donut-llm-tools
-Keywords: AI,trainer,dataset
+Keywords: AI,ML,Train,Model,Dataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: GIUC
 Requires-Dist: CreateLLM
 Requires-Dist: Wikipedia
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpver; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # Donut LLM Tools
 Donut LLM Tools is a suite of two programs that helps you create dataset from wikipedia data and your own LLM with the created or already existing dataset.
 
-*Latest Version 24.05.27 Update 3*
+*Latest Version 24.05.28*
 
 ## How to install, import and use DonutLLM?
 ### Installation
-* Before installing Donut LLM Tools, make sure you have Python `3.9` or later till Python `3.11`. *Note : Python `3.12` is not supported by PyTorch, hence Donut LLM Tools will also have troubles running.* 
+* Before installing Donut LLM Tools, make sure you have Python `3.9` or later till Python `3.11`. *Note : Python `3.12` is not supported by PyTorch, hence Donut LLM Tools will also have trouble running in it.* 
 * The dependencies for installing Donut LLM Tools are:
     1. CreateLLM (`pip install CreateLLM`)
     2. torch (Required by CreateLLM)
     3. torchvision (Required by CreateLLM, PyTorch)
     4. torchaudio (Required by CreateLLM, PyTorch)
     5. Wikipedia
```

### Comparing `donut_llm_tools-24.5.27.3/src/donutllmtools.py` & `donut_llm_tools-24.5.28/src/donutllmtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         print("2. Create Dataset")
         print("3. Exit")
         print("4. Help")
         print("5. About")
 
     def about():
         print("DonutLLM Studio | AI/ML Model Trainer/Loader")
-        print("Version 24.05.27.2")
+        print("Version 24.05.28")
         print("Developed by Gautham Nair")
 
     def exit():
         print("Exiting DonutLLM Studio")
         exit()
 
     def main():
```

