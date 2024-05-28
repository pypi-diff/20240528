# Comparing `tmp/PlayDrissionPage-0.0.1.1.tar.gz` & `tmp/PlayDrissionPage-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlayDrissionPage-0.0.1.1.tar", last modified: Mon May 27 05:55:05 2024, max compression
+gzip compressed data, was "PlayDrissionPage-0.0.1.2.tar", last modified: Mon May 27 06:05:24 2024, max compression
```

## Comparing `PlayDrissionPage-0.0.1.1.tar` & `PlayDrissionPage-0.0.1.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 05:55:05.306650 PlayDrissionPage-0.0.1.1/
--rw-rw-rw-   0        0        0      629 2024-05-27 05:55:05.305652 PlayDrissionPage-0.0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 05:55:05.297175 PlayDrissionPage-0.0.1.1/PlayDrissionPage/
--rw-rw-rw-   0        0        0      129 2024-05-27 05:52:47.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 05:55:05.304135 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/
--rw-rw-rw-   0        0        0      629 2024-05-27 05:55:05.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-27 05:55:05.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 05:55:05.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-27 05:55:05.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-27 05:38:48.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2024-05-27 05:55:05.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-27 05:55:05.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 05:55:05.306650 PlayDrissionPage-0.0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1110 2024-05-27 05:55:03.000000 PlayDrissionPage-0.0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:05:24.498256 PlayDrissionPage-0.0.1.2/
+-rw-rw-rw-   0        0        0       17 2024-05-27 06:03:38.000000 PlayDrissionPage-0.0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      629 2024-05-27 06:05:24.497256 PlayDrissionPage-0.0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 06:05:24.490257 PlayDrissionPage-0.0.1.2/PlayDrissionPage/
+-rw-rw-rw-   0        0        0      129 2024-05-27 05:52:47.000000 PlayDrissionPage-0.0.1.2/PlayDrissionPage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:05:24.496255 PlayDrissionPage-0.0.1.2/PlayDrissionPage.egg-info/
+-rw-rw-rw-   0        0        0      629 2024-05-27 06:05:24.000000 PlayDrissionPage-0.0.1.2/PlayDrissionPage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2024-05-27 06:05:24.000000 PlayDrissionPage-0.0.1.2/PlayDrissionPage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 06:05:24.000000 PlayDrissionPage-0.0.1.2/PlayDrissionPage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-27 06:05:24.000000 PlayDrissionPage-0.0.1.2/PlayDrissionPage.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-27 05:38:48.000000 PlayDrissionPage-0.0.1.2/PlayDrissionPage.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2024-05-27 06:05:24.000000 PlayDrissionPage-0.0.1.2/PlayDrissionPage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 06:05:24.000000 PlayDrissionPage-0.0.1.2/PlayDrissionPage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       46 2024-05-15 03:34:19.000000 PlayDrissionPage-0.0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 06:05:24.498256 PlayDrissionPage-0.0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2024-05-27 06:05:05.000000 PlayDrissionPage-0.0.1.2/setup.py
```

### Comparing `PlayDrissionPage-0.0.1.1/PKG-INFO` & `PlayDrissionPage-0.0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlayDrissionPage
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Playwright and DrissionPage
 Home-page: https://gitee.com/xx299x/PlayDrissionPage
 Author: xx299x
 Author-email: xx299x@gmail.com
 License: BSD
 Keywords: Playwright,DrissionPage
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/PKG-INFO` & `PlayDrissionPage-0.0.1.2/PlayDrissionPage.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlayDrissionPage
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Playwright and DrissionPage
 Home-page: https://gitee.com/xx299x/PlayDrissionPage
 Author: xx299x
 Author-email: xx299x@gmail.com
 License: BSD
 Keywords: Playwright,DrissionPage
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `PlayDrissionPage-0.0.1.1/setup.py` & `PlayDrissionPage-0.0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding:utf-8 -*-
 from setuptools import setup, find_packages
-__version__ = '0.0.1.1'
+__version__ = '0.0.1.2'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="PlayDrissionPage",
     version=__version__,
```

