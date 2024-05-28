# Comparing `tmp/aiodatabase-0.1.0.tar.gz` & `tmp/aiodatabase-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodatabase-0.1.0.tar", last modified: Tue May 28 08:37:27 2024, max compression
+gzip compressed data, was "aiodatabase-0.1.1.tar", last modified: Tue May 28 09:02:35 2024, max compression
```

## Comparing `aiodatabase-0.1.0.tar` & `aiodatabase-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 08:37:27.278862 aiodatabase-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-05-28 08:37:27.271326 aiodatabase-0.1.0/AioDatabase.egg-info/
--rw-rw-rw-   0        0        0      457 2024-05-28 08:37:27.000000 aiodatabase-0.1.0/AioDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2024-05-28 08:37:27.000000 aiodatabase-0.1.0/AioDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 08:37:27.000000 aiodatabase-0.1.0/AioDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-28 08:37:27.000000 aiodatabase-0.1.0/AioDatabase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-05-28 08:37:27.000000 aiodatabase-0.1.0/AioDatabase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-28 08:37:27.000000 aiodatabase-0.1.0/AioDatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      457 2024-05-28 08:37:27.276836 aiodatabase-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-28 08:37:27.278862 aiodatabase-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-05-28 08:32:01.000000 aiodatabase-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:37:27.270821 aiodatabase-0.1.0/src/
--rw-rw-rw-   0        0        0     4533 2024-05-28 08:20:52.000000 aiodatabase-0.1.0/src/AioDatabase.py
--rw-rw-rw-   0        0        0     1552 2024-05-28 08:18:41.000000 aiodatabase-0.1.0/src/DataConnector.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:37:27.271326 aiodatabase-0.1.0/src/Manager/
--rw-rw-rw-   0        0        0     2524 2024-05-28 07:15:04.000000 aiodatabase-0.1.0/src/Manager/ConfigManager.py
--rw-rw-rw-   0        0        0        0 2024-05-28 08:09:29.000000 aiodatabase-0.1.0/src/Manager/__init__.py
--rw-rw-rw-   0        0        0       35 2024-05-28 08:15:02.000000 aiodatabase-0.1.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:37:27.271326 aiodatabase-0.1.0/src/sqlite3/
--rw-rw-rw-   0        0        0     1164 2024-05-28 07:16:41.000000 aiodatabase-0.1.0/src/sqlite3/SqlLoader.py
--rw-rw-rw-   0        0        0        0 2024-05-28 08:09:45.000000 aiodatabase-0.1.0/src/sqlite3/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:02:35.268797 aiodatabase-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-28 09:02:35.264534 aiodatabase-0.1.1/AioDatabase.egg-info/
+-rw-rw-rw-   0        0        0      457 2024-05-28 09:02:35.000000 aiodatabase-0.1.1/AioDatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-05-28 09:02:35.000000 aiodatabase-0.1.1/AioDatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 09:02:35.000000 aiodatabase-0.1.1/AioDatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-28 09:02:35.000000 aiodatabase-0.1.1/AioDatabase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-05-28 09:02:35.000000 aiodatabase-0.1.1/AioDatabase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-28 09:02:35.000000 aiodatabase-0.1.1/AioDatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      457 2024-05-28 09:02:35.267651 aiodatabase-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-28 09:02:35.268797 aiodatabase-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      766 2024-05-28 09:01:44.000000 aiodatabase-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:02:35.264534 aiodatabase-0.1.1/src/
+-rw-rw-rw-   0        0        0     4533 2024-05-28 08:20:52.000000 aiodatabase-0.1.1/src/AioDatabase.py
+-rw-rw-rw-   0        0        0     1552 2024-05-28 08:18:41.000000 aiodatabase-0.1.1/src/DataConnector.py
+-rw-rw-rw-   0        0        0       35 2024-05-28 08:15:02.000000 aiodatabase-0.1.1/src/__init__.py
```

### Comparing `aiodatabase-0.1.0/setup.py` & `aiodatabase-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 setup(
     name="AioDatabase",
-    version="0.1.0",
-    packages=find_packages(include=["src", "src.*"]),
+    version="0.1.1",
+    packages=["src"],
     install_requires=["PyYAML", "aiomysql", "aiosqlite"],
     entry_points={
         "console_scripts": [
             "aiodatabase=src.AioDatabase:main",
         ],
     },
     package_data={
```

### Comparing `aiodatabase-0.1.0/src/AioDatabase.py` & `aiodatabase-0.1.1/src/AioDatabase.py`

 * *Files identical despite different names*

### Comparing `aiodatabase-0.1.0/src/DataConnector.py` & `aiodatabase-0.1.1/src/DataConnector.py`

 * *Files identical despite different names*

