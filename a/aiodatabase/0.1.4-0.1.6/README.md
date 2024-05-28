# Comparing `tmp/aiodatabase-0.1.4.tar.gz` & `tmp/aiodatabase-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodatabase-0.1.4.tar", last modified: Tue May 28 09:26:45 2024, max compression
+gzip compressed data, was "aiodatabase-0.1.6.tar", last modified: Tue May 28 10:00:57 2024, max compression
```

## Comparing `aiodatabase-0.1.4.tar` & `aiodatabase-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 09:26:45.329886 aiodatabase-0.1.4/
--rw-rw-rw-   0        0        0      457 2024-05-28 09:26:45.328352 aiodatabase-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-28 09:26:45.329886 aiodatabase-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      851 2024-05-28 09:26:34.000000 aiodatabase-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:26:45.295365 aiodatabase-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 09:26:45.328352 aiodatabase-0.1.4/src/AioDatabase.egg-info/
--rw-rw-rw-   0        0        0      457 2024-05-28 09:26:45.000000 aiodatabase-0.1.4/src/AioDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-05-28 09:26:45.000000 aiodatabase-0.1.4/src/AioDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 09:26:45.000000 aiodatabase-0.1.4/src/AioDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-28 09:26:45.000000 aiodatabase-0.1.4/src/AioDatabase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-05-28 09:26:45.000000 aiodatabase-0.1.4/src/AioDatabase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-28 09:26:45.000000 aiodatabase-0.1.4/src/AioDatabase.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 09:26:45.321040 aiodatabase-0.1.4/src/Manager/
--rw-rw-rw-   0        0        0     2524 2024-05-28 07:15:04.000000 aiodatabase-0.1.4/src/Manager/ConfigManager.py
--rw-rw-rw-   0        0        0        0 2024-05-28 08:09:29.000000 aiodatabase-0.1.4/src/Manager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:26:45.324803 aiodatabase-0.1.4/src/sqlite3/
--rw-rw-rw-   0        0        0     1164 2024-05-28 07:16:41.000000 aiodatabase-0.1.4/src/sqlite3/SqlLoader.py
--rw-rw-rw-   0        0        0        0 2024-05-28 08:09:45.000000 aiodatabase-0.1.4/src/sqlite3/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:00:57.117646 aiodatabase-0.1.6/
+-rw-rw-rw-   0        0        0     1079 2024-05-28 09:46:29.000000 aiodatabase-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      480 2024-05-28 10:00:57.117646 aiodatabase-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2024-05-28 10:00:57.119256 aiodatabase-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      730 2024-05-28 10:00:43.000000 aiodatabase-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:00:57.084914 aiodatabase-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 10:00:57.116649 aiodatabase-0.1.6/src/AioDatabase.egg-info/
+-rw-rw-rw-   0        0        0      480 2024-05-28 10:00:57.000000 aiodatabase-0.1.6/src/AioDatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2024-05-28 10:00:57.000000 aiodatabase-0.1.6/src/AioDatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 10:00:57.000000 aiodatabase-0.1.6/src/AioDatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-28 10:00:57.000000 aiodatabase-0.1.6/src/AioDatabase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-28 10:00:57.000000 aiodatabase-0.1.6/src/AioDatabase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 10:00:57.113563 aiodatabase-0.1.6/src/Manager/
+-rw-rw-rw-   0        0        0     2524 2024-05-28 07:15:04.000000 aiodatabase-0.1.6/src/Manager/ConfigManager.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 08:09:29.000000 aiodatabase-0.1.6/src/Manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:00:57.114635 aiodatabase-0.1.6/src/sqlite3/
+-rw-rw-rw-   0        0        0     1164 2024-05-28 07:16:41.000000 aiodatabase-0.1.6/src/sqlite3/SqlLoader.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 08:09:45.000000 aiodatabase-0.1.6/src/sqlite3/__init__.py
```

### Comparing `aiodatabase-0.1.4/setup.py` & `aiodatabase-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AioDatabase",
-    version="0.1.4",
+    version="0.1.6",
     install_requires=["PyYAML", "aiomysql", "aiosqlite"],
-    entry_points={
-        "console_scripts": [
-            "aiodatabase=src.AioDatabase:main",
-        ],
-    }, 
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     package_data={
-        "": ["resources/queries.sql", "resources/config.yml"],
+        "": ["resources/sqlite.sql", "resources/config.yml"],
     },
     include_package_data=True,
     description="AioDatabase is a simple database abstraction layer for SQLite and MySQL.",
     author="AmitxD",
     url="https://github.com/Amitminer/AioDatabase",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `aiodatabase-0.1.4/src/Manager/ConfigManager.py` & `aiodatabase-0.1.6/src/Manager/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `aiodatabase-0.1.4/src/sqlite3/SqlLoader.py` & `aiodatabase-0.1.6/src/sqlite3/SqlLoader.py`

 * *Files identical despite different names*

