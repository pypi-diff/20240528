# Comparing `tmp/feishuconnector-0.1.6.tar.gz` & `tmp/feishuconnector-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/feishuconnector-0.1.6.tar", last modified: Fri May 17 00:11:40 2024, max compression
+gzip compressed data, was "dist/feishuconnector-0.1.7.tar", last modified: Tue May 28 05:57:56 2024, max compression
```

## Comparing `feishuconnector-0.1.6.tar` & `feishuconnector-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 00:11:40.915301 feishuconnector-0.1.6/
--rw-r--r--   0 root         (0) root         (0)      268 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1089 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1760 2024-05-17 00:11:40.915301 feishuconnector-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1119 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 00:11:40.914301 feishuconnector-0.1.6/feishuconnector/
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/feishuconnector/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-17 00:10:52.000000 feishuconnector-0.1.6/feishuconnector/_version.py
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/feishuconnector/encoder.py
--rw-r--r--   0 root         (0) root         (0)    16970 2024-05-17 00:10:00.000000 feishuconnector-0.1.6/feishuconnector/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 00:11:40.915301 feishuconnector-0.1.6/feishuconnector.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1760 2024-05-17 00:11:40.000000 feishuconnector-0.1.6/feishuconnector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-17 00:11:40.000000 feishuconnector-0.1.6/feishuconnector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 00:11:40.000000 feishuconnector-0.1.6/feishuconnector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-05-17 00:11:40.000000 feishuconnector-0.1.6/feishuconnector.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-17 00:11:40.000000 feishuconnector-0.1.6/feishuconnector.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      107 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 00:11:40.915301 feishuconnector-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1193 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 00:11:40.915301 feishuconnector-0.1.6/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/test/run.py
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/upload.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:57:56.761034 feishuconnector-0.1.7/
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-05-13 08:04:31.000000 feishuconnector-0.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1760 2024-05-28 05:57:56.761034 feishuconnector-0.1.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:57:56.760034 feishuconnector-0.1.7/feishuconnector/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-13 08:04:31.000000 feishuconnector-0.1.7/feishuconnector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-28 05:56:17.000000 feishuconnector-0.1.7/feishuconnector/_version.py
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-13 08:04:31.000000 feishuconnector-0.1.7/feishuconnector/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    16970 2024-05-17 00:10:00.000000 feishuconnector-0.1.7/feishuconnector/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:57:56.761034 feishuconnector-0.1.7/feishuconnector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1760 2024-05-28 05:57:56.000000 feishuconnector-0.1.7/feishuconnector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2024-05-28 05:57:56.000000 feishuconnector-0.1.7/feishuconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 05:57:56.000000 feishuconnector-0.1.7/feishuconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-28 05:57:56.000000 feishuconnector-0.1.7/feishuconnector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-28 05:57:56.000000 feishuconnector-0.1.7/feishuconnector.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 05:57:56.761034 feishuconnector-0.1.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:57:56.761034 feishuconnector-0.1.7/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 08:04:31.000000 feishuconnector-0.1.7/test/run.py
```

### Comparing `feishuconnector-0.1.6/LICENSE` & `feishuconnector-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `feishuconnector-0.1.6/PKG-INFO` & `feishuconnector-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feishuconnector
-Version: 0.1.6
+Version: 0.1.7
 Summary: connect feishu content franchise
 Home-page: http://www.puyuan.tech
 Author: Changhao Jiang
 Author-email: jch@puyuan.tech
 License: MIT License
 Platform: all
 Classifier: Development Status :: 4 - Beta
```

### Comparing `feishuconnector-0.1.6/feishuconnector/manager.py` & `feishuconnector-0.1.7/feishuconnector/manager.py`

 * *Files identical despite different names*

### Comparing `feishuconnector-0.1.6/feishuconnector.egg-info/PKG-INFO` & `feishuconnector-0.1.7/feishuconnector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feishuconnector
-Version: 0.1.6
+Version: 0.1.7
 Summary: connect feishu content franchise
 Home-page: http://www.puyuan.tech
 Author: Changhao Jiang
 Author-email: jch@puyuan.tech
 License: MIT License
 Platform: all
 Classifier: Development Status :: 4 - Beta
```

