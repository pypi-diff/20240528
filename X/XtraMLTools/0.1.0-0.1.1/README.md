# Comparing `tmp/XtraMLTools-0.1.0.tar.gz` & `tmp/XtraMLTools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XtraMLTools-0.1.0.tar", last modified: Mon May 27 18:06:23 2024, max compression
+gzip compressed data, was "XtraMLTools-0.1.1.tar", last modified: Mon May 27 22:50:31 2024, max compression
```

## Comparing `XtraMLTools-0.1.0.tar` & `XtraMLTools-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 18:06:23.345132 XtraMLTools-0.1.0/
--rw-rw-rw-   0        0        0     1094 2024-05-05 22:13:13.000000 XtraMLTools-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      157 2024-05-27 18:06:23.344118 XtraMLTools-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5657 2024-05-27 14:57:12.000000 XtraMLTools-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 18:06:23.328599 XtraMLTools-0.1.0/XtraMLTools/
--rw-rw-rw-   0        0        0    12530 2024-05-27 17:12:32.000000 XtraMLTools-0.1.0/XtraMLTools/Classification.py
--rw-rw-rw-   0        0        0    23883 2024-05-27 17:10:53.000000 XtraMLTools-0.1.0/XtraMLTools/Preprocessing.py
--rw-rw-rw-   0        0        0    73962 2024-05-27 15:57:13.000000 XtraMLTools-0.1.0/XtraMLTools/Regression.py
--rw-rw-rw-   0        0        0       92 2024-05-04 21:55:12.000000 XtraMLTools-0.1.0/XtraMLTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:06:23.338159 XtraMLTools-0.1.0/XtraMLTools.egg-info/
--rw-rw-rw-   0        0        0      157 2024-05-27 18:06:23.000000 XtraMLTools-0.1.0/XtraMLTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-05-27 18:06:23.000000 XtraMLTools-0.1.0/XtraMLTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 18:06:23.000000 XtraMLTools-0.1.0/XtraMLTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-27 18:06:23.000000 XtraMLTools-0.1.0/XtraMLTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 18:06:23.345132 XtraMLTools-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      376 2024-05-05 20:53:31.000000 XtraMLTools-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:06:23.341707 XtraMLTools-0.1.0/tests/
--rw-rw-rw-   0        0        0     2343 2024-05-27 17:13:03.000000 XtraMLTools-0.1.0/tests/test_Classification.py
--rw-rw-rw-   0        0        0     9861 2024-05-27 17:07:41.000000 XtraMLTools-0.1.0/tests/test_Preprocessing.py
--rw-rw-rw-   0        0        0     5096 2024-05-26 21:05:58.000000 XtraMLTools-0.1.0/tests/test_Regression.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:50:31.835243 XtraMLTools-0.1.1/
+-rw-rw-rw-   0        0        0     1094 2024-05-05 22:13:13.000000 XtraMLTools-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     6105 2024-05-27 22:50:31.833743 XtraMLTools-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5657 2024-05-27 14:57:12.000000 XtraMLTools-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 22:50:31.805118 XtraMLTools-0.1.1/XtraMLTools/
+-rw-rw-rw-   0        0        0    12530 2024-05-27 17:12:32.000000 XtraMLTools-0.1.1/XtraMLTools/Classification.py
+-rw-rw-rw-   0        0        0    23883 2024-05-27 17:10:53.000000 XtraMLTools-0.1.1/XtraMLTools/Preprocessing.py
+-rw-rw-rw-   0        0        0    73962 2024-05-27 15:57:13.000000 XtraMLTools-0.1.1/XtraMLTools/Regression.py
+-rw-rw-rw-   0        0        0       92 2024-05-04 21:55:12.000000 XtraMLTools-0.1.1/XtraMLTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:50:31.826852 XtraMLTools-0.1.1/XtraMLTools.egg-info/
+-rw-rw-rw-   0        0        0     6105 2024-05-27 22:50:31.000000 XtraMLTools-0.1.1/XtraMLTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-05-27 22:50:31.000000 XtraMLTools-0.1.1/XtraMLTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 22:50:31.000000 XtraMLTools-0.1.1/XtraMLTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-27 22:50:31.000000 XtraMLTools-0.1.1/XtraMLTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 22:50:31.000000 XtraMLTools-0.1.1/XtraMLTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 22:50:31.835243 XtraMLTools-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      749 2024-05-27 22:49:59.000000 XtraMLTools-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:50:31.832740 XtraMLTools-0.1.1/tests/
+-rw-rw-rw-   0        0        0     2343 2024-05-27 17:13:03.000000 XtraMLTools-0.1.1/tests/test_Classification.py
+-rw-rw-rw-   0        0        0     9861 2024-05-27 17:07:41.000000 XtraMLTools-0.1.1/tests/test_Preprocessing.py
+-rw-rw-rw-   0        0        0     5096 2024-05-26 21:05:58.000000 XtraMLTools-0.1.1/tests/test_Regression.py
```

### Comparing `XtraMLTools-0.1.0/LICENSE.txt` & `XtraMLTools-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `XtraMLTools-0.1.0/README.md` & `XtraMLTools-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `XtraMLTools-0.1.0/XtraMLTools/Classification.py` & `XtraMLTools-0.1.1/XtraMLTools/Classification.py`

 * *Files identical despite different names*

### Comparing `XtraMLTools-0.1.0/XtraMLTools/Preprocessing.py` & `XtraMLTools-0.1.1/XtraMLTools/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `XtraMLTools-0.1.0/XtraMLTools/Regression.py` & `XtraMLTools-0.1.1/XtraMLTools/Regression.py`

 * *Files identical despite different names*

### Comparing `XtraMLTools-0.1.0/tests/test_Classification.py` & `XtraMLTools-0.1.1/tests/test_Classification.py`

 * *Files identical despite different names*

### Comparing `XtraMLTools-0.1.0/tests/test_Preprocessing.py` & `XtraMLTools-0.1.1/tests/test_Preprocessing.py`

 * *Files identical despite different names*

### Comparing `XtraMLTools-0.1.0/tests/test_Regression.py` & `XtraMLTools-0.1.1/tests/test_Regression.py`

 * *Files identical despite different names*

