# Comparing `tmp/easydrive-0.0.4.tar.gz` & `tmp/easydrive-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydrive-0.0.4.tar", last modified: Tue May 28 01:59:41 2024, max compression
+gzip compressed data, was "easydrive-0.0.5.tar", last modified: Tue May 28 03:53:00 2024, max compression
```

## Comparing `easydrive-0.0.4.tar` & `easydrive-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 01:59:41.766380 easydrive-0.0.4/
--rw-rw-rw-   0        0        0      516 2024-05-28 01:59:41.765374 easydrive-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-05-28 01:01:02.000000 easydrive-0.0.4/README.md
--rw-rw-rw-   0        0        0      462 2024-05-28 01:59:34.000000 easydrive-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 01:59:41.766380 easydrive-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 01:59:41.751276 easydrive-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 01:59:41.758846 easydrive-0.0.4/src/EasyDrive/
--rw-rw-rw-   0        0        0     9692 2024-05-28 01:58:37.000000 easydrive-0.0.4/src/EasyDrive/Drive.py
--rw-rw-rw-   0        0        0      246 2024-05-27 23:52:34.000000 easydrive-0.0.4/src/EasyDrive/Exceptions.py
--rw-rw-rw-   0        0        0    11349 2024-05-28 01:22:34.000000 easydrive-0.0.4/src/EasyDrive/FileSystemTypes.py
--rw-rw-rw-   0        0        0     1677 2024-05-26 02:34:40.000000 easydrive-0.0.4/src/EasyDrive/MIMETypes.py
--rw-rw-rw-   0        0        0       43 2024-05-28 01:58:48.000000 easydrive-0.0.4/src/EasyDrive/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:59:41.764368 easydrive-0.0.4/src/EasyDrive.egg-info/
--rw-rw-rw-   0        0        0      516 2024-05-28 01:59:41.000000 easydrive-0.0.4/src/EasyDrive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-28 01:59:41.000000 easydrive-0.0.4/src/EasyDrive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 01:59:41.000000 easydrive-0.0.4/src/EasyDrive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-28 01:59:41.000000 easydrive-0.0.4/src/EasyDrive.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 03:53:00.673270 easydrive-0.0.5/
+-rw-rw-rw-   0        0        0      516 2024-05-28 03:53:00.672269 easydrive-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-05-28 01:01:02.000000 easydrive-0.0.5/README.md
+-rw-rw-rw-   0        0        0      462 2024-05-28 03:52:48.000000 easydrive-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 03:53:00.673270 easydrive-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 03:53:00.656736 easydrive-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 03:53:00.665260 easydrive-0.0.5/src/EasyDrive/
+-rw-rw-rw-   0        0        0     9692 2024-05-28 03:02:54.000000 easydrive-0.0.5/src/EasyDrive/Drives.py
+-rw-rw-rw-   0        0        0      246 2024-05-27 23:52:34.000000 easydrive-0.0.5/src/EasyDrive/Exceptions.py
+-rw-rw-rw-   0        0        0    11349 2024-05-28 01:22:34.000000 easydrive-0.0.5/src/EasyDrive/FileSystemTypes.py
+-rw-rw-rw-   0        0        0     1677 2024-05-26 02:34:40.000000 easydrive-0.0.5/src/EasyDrive/MIMETypes.py
+-rw-rw-rw-   0        0        0       60 2024-05-28 03:51:41.000000 easydrive-0.0.5/src/EasyDrive/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:53:00.671764 easydrive-0.0.5/src/EasyDrive.egg-info/
+-rw-rw-rw-   0        0        0      516 2024-05-28 03:53:00.000000 easydrive-0.0.5/src/EasyDrive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-28 03:53:00.000000 easydrive-0.0.5/src/EasyDrive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 03:53:00.000000 easydrive-0.0.5/src/EasyDrive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 03:53:00.000000 easydrive-0.0.5/src/EasyDrive.egg-info/top_level.txt
```

### Comparing `easydrive-0.0.4/PKG-INFO` & `easydrive-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyDrive
-Version: 0.0.4
+Version: 0.0.5
 Summary: EasyGoogle Drive access
 Author-email: RanchMonster <ranchmonster06@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `easydrive-0.0.4/src/EasyDrive/Drive.py` & `easydrive-0.0.5/src/EasyDrive/Drives.py`

 * *Files identical despite different names*

### Comparing `easydrive-0.0.4/src/EasyDrive/FileSystemTypes.py` & `easydrive-0.0.5/src/EasyDrive/FileSystemTypes.py`

 * *Files identical despite different names*

### Comparing `easydrive-0.0.4/src/EasyDrive/MIMETypes.py` & `easydrive-0.0.5/src/EasyDrive/MIMETypes.py`

 * *Files identical despite different names*

### Comparing `easydrive-0.0.4/src/EasyDrive.egg-info/PKG-INFO` & `easydrive-0.0.5/src/EasyDrive.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyDrive
-Version: 0.0.4
+Version: 0.0.5
 Summary: EasyGoogle Drive access
 Author-email: RanchMonster <ranchmonster06@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

