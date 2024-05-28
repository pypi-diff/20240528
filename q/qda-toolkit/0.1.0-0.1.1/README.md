# Comparing `tmp/qda_toolkit-0.1.0.tar.gz` & `tmp/qda_toolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qda_toolkit-0.1.0.tar", last modified: Tue May 28 15:46:24 2024, max compression
+gzip compressed data, was "qda_toolkit-0.1.1.tar", last modified: Tue May 28 16:12:26 2024, max compression
```

## Comparing `qda_toolkit-0.1.0.tar` & `qda_toolkit-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:46:24.172072 qda_toolkit-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    19089 2024-05-28 15:46:21.000000 qda_toolkit-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-28 15:46:24.172072 qda_toolkit-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-28 15:46:21.000000 qda_toolkit-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:46:24.168072 qda_toolkit-0.1.0/qda/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 15:46:21.000000 qda_toolkit-0.1.0/qda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42919 2024-05-28 15:46:21.000000 qda_toolkit-0.1.0/qda/controlcharts.py
--rw-r--r--   0 runner    (1001) docker     (127)    25382 2024-05-28 15:46:21.000000 qda_toolkit-0.1.0/qda/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:46:24.172072 qda_toolkit-0.1.0/qda_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-28 15:46:24.000000 qda_toolkit-0.1.0/qda_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-28 15:46:24.000000 qda_toolkit-0.1.0/qda_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:46:24.000000 qda_toolkit-0.1.0/qda_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-28 15:46:24.000000 qda_toolkit-0.1.0/qda_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 15:46:24.000000 qda_toolkit-0.1.0/qda_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 15:46:24.172072 qda_toolkit-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-28 15:46:21.000000 qda_toolkit-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:46:24.172072 qda_toolkit-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-28 15:46:21.000000 qda_toolkit-0.1.0/tests/test_CC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:12:26.565096 qda_toolkit-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    19089 2024-05-28 16:12:19.000000 qda_toolkit-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-28 16:12:26.565096 qda_toolkit-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-28 16:12:19.000000 qda_toolkit-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:12:26.565096 qda_toolkit-0.1.1/qda/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 16:12:19.000000 qda_toolkit-0.1.1/qda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42919 2024-05-28 16:12:19.000000 qda_toolkit-0.1.1/qda/controlcharts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25382 2024-05-28 16:12:19.000000 qda_toolkit-0.1.1/qda/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:12:26.565096 qda_toolkit-0.1.1/qda_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-28 16:12:26.000000 qda_toolkit-0.1.1/qda_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-28 16:12:26.000000 qda_toolkit-0.1.1/qda_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:12:26.000000 qda_toolkit-0.1.1/qda_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-28 16:12:26.000000 qda_toolkit-0.1.1/qda_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 16:12:26.000000 qda_toolkit-0.1.1/qda_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 16:12:26.565096 qda_toolkit-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-28 16:12:19.000000 qda_toolkit-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:12:26.565096 qda_toolkit-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-28 16:12:19.000000 qda_toolkit-0.1.1/tests/test_CC.py
```

### Comparing `qda_toolkit-0.1.0/LICENSE` & `qda_toolkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qda_toolkit-0.1.0/PKG-INFO` & `qda_toolkit-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qda-toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Quality data analysis toolkit
 Home-page: https://github.com/polimi-iclabs/qda
 Author: IC Labs (Matteo Bugatti)
 Author-email: <matteo.bugatti@polimi.it>
 License: CC BY-NC-SA 4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Requires-Dist: matplotlib==3.5.2
 Requires-Dist: numpy==1.21.5
 Requires-Dist: pandas==1.3.5
 Requires-Dist: scipy==1.7.3
 Requires-Dist: statsmodels==0.13.5
 
 <p align="center">
-  <img src="https://github.com/polimi-iclabs/qda/blob/main/docs/logo.svg" alt="Logo">
+  <img src="https://raw.githubusercontent.com/polimi-iclabs/qda-toolkit/main/docs/logo.svg" alt="Logo">
 </p>
 
 # qda-toolkit: a Python Package for Statistical Process Control and Quality Data Analysis
 
 This repository contains `qda-toolkit`, a Python package that provides functions for creating control charts and statistical models. The output is designed to be user-friendly and similar to the one provided by other popular commercial software for statistical process control and quality data modeling.
 
 ## Features
```

### Comparing `qda_toolkit-0.1.0/README.md` & `qda_toolkit-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img src="https://github.com/polimi-iclabs/qda/blob/main/docs/logo.svg" alt="Logo">
+  <img src="https://raw.githubusercontent.com/polimi-iclabs/qda-toolkit/main/docs/logo.svg" alt="Logo">
 </p>
 
 # qda-toolkit: a Python Package for Statistical Process Control and Quality Data Analysis
 
 This repository contains `qda-toolkit`, a Python package that provides functions for creating control charts and statistical models. The output is designed to be user-friendly and similar to the one provided by other popular commercial software for statistical process control and quality data modeling.
 
 ## Features
```

### Comparing `qda_toolkit-0.1.0/qda/controlcharts.py` & `qda_toolkit-0.1.1/qda/controlcharts.py`

 * *Files identical despite different names*

### Comparing `qda_toolkit-0.1.0/qda/models.py` & `qda_toolkit-0.1.1/qda/models.py`

 * *Files identical despite different names*

### Comparing `qda_toolkit-0.1.0/qda_toolkit.egg-info/PKG-INFO` & `qda_toolkit-0.1.1/qda_toolkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qda-toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Quality data analysis toolkit
 Home-page: https://github.com/polimi-iclabs/qda
 Author: IC Labs (Matteo Bugatti)
 Author-email: <matteo.bugatti@polimi.it>
 License: CC BY-NC-SA 4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Requires-Dist: matplotlib==3.5.2
 Requires-Dist: numpy==1.21.5
 Requires-Dist: pandas==1.3.5
 Requires-Dist: scipy==1.7.3
 Requires-Dist: statsmodels==0.13.5
 
 <p align="center">
-  <img src="https://github.com/polimi-iclabs/qda/blob/main/docs/logo.svg" alt="Logo">
+  <img src="https://raw.githubusercontent.com/polimi-iclabs/qda-toolkit/main/docs/logo.svg" alt="Logo">
 </p>
 
 # qda-toolkit: a Python Package for Statistical Process Control and Quality Data Analysis
 
 This repository contains `qda-toolkit`, a Python package that provides functions for creating control charts and statistical models. The output is designed to be user-friendly and similar to the one provided by other popular commercial software for statistical process control and quality data modeling.
 
 ## Features
```

### Comparing `qda_toolkit-0.1.0/setup.py` & `qda_toolkit-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Quality data analysis toolkit'
 LONG_DESCRIPTION = 'A package to create charts and models for statistical process control.'
 
 setup(
     name='qda-toolkit',
     version=VERSION,
     author="IC Labs (Matteo Bugatti)",
```

### Comparing `qda_toolkit-0.1.0/tests/test_CC.py` & `qda_toolkit-0.1.1/tests/test_CC.py`

 * *Files identical despite different names*

