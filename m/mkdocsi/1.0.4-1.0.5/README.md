# Comparing `tmp/mkdocsi-1.0.4.tar.gz` & `tmp/mkdocsi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.0.4.tar", last modified: Tue May 28 16:11:53 2024, max compression
+gzip compressed data, was "mkdocsi-1.0.5.tar", last modified: Tue May 28 16:13:50 2024, max compression
```

## Comparing `mkdocsi-1.0.4.tar` & `mkdocsi-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:11:53.277704 mkdocsi-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 16:11:53.277704 mkdocsi-1.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 16:11:44.000000 mkdocsi-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:11:53.275704 mkdocsi-1.0.4/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)      107 2024-05-28 16:11:44.000000 mkdocsi-1.0.4/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     5273 2024-05-28 16:11:44.000000 mkdocsi-1.0.4/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:11:53.276704 mkdocsi-1.0.4/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 16:11:53.000000 mkdocsi-1.0.4/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 16:11:53.000000 mkdocsi-1.0.4/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 16:11:53.000000 mkdocsi-1.0.4/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 16:11:53.000000 mkdocsi-1.0.4/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 16:11:53.000000 mkdocsi-1.0.4/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 16:11:53.000000 mkdocsi-1.0.4/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 16:11:53.277704 mkdocsi-1.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 16:11:44.000000 mkdocsi-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:13:50.273381 mkdocsi-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 16:13:50.273381 mkdocsi-1.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 16:13:40.000000 mkdocsi-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:13:50.271381 mkdocsi-1.0.5/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 16:13:40.000000 mkdocsi-1.0.5/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     5273 2024-05-28 16:13:40.000000 mkdocsi-1.0.5/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:13:50.273381 mkdocsi-1.0.5/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 16:13:50.000000 mkdocsi-1.0.5/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 16:13:50.000000 mkdocsi-1.0.5/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 16:13:50.000000 mkdocsi-1.0.5/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 16:13:50.000000 mkdocsi-1.0.5/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 16:13:50.000000 mkdocsi-1.0.5/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 16:13:50.000000 mkdocsi-1.0.5/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 16:13:50.273381 mkdocsi-1.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 16:13:40.000000 mkdocsi-1.0.5/setup.py
```

### Comparing `mkdocsi-1.0.4/PKG-INFO` & `mkdocsi-1.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.0.4
+Version: 1.0.5
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.0.4/mkdocsi/__init__.py` & `mkdocsi-1.0.5/mkdocsi/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocsi-1.0.4/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.0.5/mkdocsi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.0.4
+Version: 1.0.5
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.0.4/setup.py` & `mkdocsi-1.0.5/setup.py`

 * *Files identical despite different names*

