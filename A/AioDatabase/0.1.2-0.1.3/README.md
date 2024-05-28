# Comparing `tmp/aiodatabase-0.1.2.tar.gz` & `tmp/aiodatabase-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodatabase-0.1.2.tar", last modified: Tue May 28 09:07:31 2024, max compression
+gzip compressed data, was "aiodatabase-0.1.3.tar", last modified: Tue May 28 09:20:36 2024, max compression
```

## Comparing `aiodatabase-0.1.2.tar` & `aiodatabase-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 09:07:31.579048 aiodatabase-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-05-28 09:07:31.577983 aiodatabase-0.1.2/AioDatabase.egg-info/
--rw-rw-rw-   0        0        0      457 2024-05-28 09:07:31.000000 aiodatabase-0.1.2/AioDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-28 09:07:31.000000 aiodatabase-0.1.2/AioDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 09:07:31.000000 aiodatabase-0.1.2/AioDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-28 09:07:31.000000 aiodatabase-0.1.2/AioDatabase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-05-28 09:07:31.000000 aiodatabase-0.1.2/AioDatabase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-28 09:07:31.000000 aiodatabase-0.1.2/AioDatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      457 2024-05-28 09:07:31.579048 aiodatabase-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-28 09:07:31.579048 aiodatabase-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      766 2024-05-28 09:05:59.000000 aiodatabase-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:20:36.124669 aiodatabase-0.1.3/
+-rw-rw-rw-   0        0        0      457 2024-05-28 09:20:36.124669 aiodatabase-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-28 09:20:36.124669 aiodatabase-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      831 2024-05-28 09:20:11.000000 aiodatabase-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:20:36.100326 aiodatabase-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 09:20:36.116665 aiodatabase-0.1.3/src/AioDatabase.egg-info/
+-rw-rw-rw-   0        0        0      457 2024-05-28 09:20:36.000000 aiodatabase-0.1.3/src/AioDatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-05-28 09:20:36.000000 aiodatabase-0.1.3/src/AioDatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 09:20:36.000000 aiodatabase-0.1.3/src/AioDatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-28 09:20:36.000000 aiodatabase-0.1.3/src/AioDatabase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-05-28 09:20:36.000000 aiodatabase-0.1.3/src/AioDatabase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-28 09:20:36.000000 aiodatabase-0.1.3/src/AioDatabase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 09:20:36.116665 aiodatabase-0.1.3/src/Manager/
+-rw-rw-rw-   0        0        0     2524 2024-05-28 07:15:04.000000 aiodatabase-0.1.3/src/Manager/ConfigManager.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 08:09:29.000000 aiodatabase-0.1.3/src/Manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:20:36.116665 aiodatabase-0.1.3/src/sqlite3/
+-rw-rw-rw-   0        0        0     1164 2024-05-28 07:16:41.000000 aiodatabase-0.1.3/src/sqlite3/SqlLoader.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 08:09:45.000000 aiodatabase-0.1.3/src/sqlite3/__init__.py
```

### Comparing `aiodatabase-0.1.2/setup.py` & `aiodatabase-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name="AioDatabase",
-    version="0.1.2",
-    packages=["src"],
+    version="0.1.3",
     install_requires=["PyYAML", "aiomysql", "aiosqlite"],
     entry_points={
         "console_scripts": [
             "aiodatabase=src.AioDatabase:main",
         ],
-    },
+    }, 
+    package_dir={'': 'src'},
+    packages=find_packages(where='src'),
     package_data={
         "": ["queries.sql", "config.yml"],
     },
     include_package_data=True,
     description="AioDatabase is a simple database abstraction layer for SQLite and MySQL.",
     author="AmitxD",
     url="https://github.com/Amitminer/AioDatabase",
```

