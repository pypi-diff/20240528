# Comparing `tmp/aiodatabase-0.1.1.tar.gz` & `tmp/aiodatabase-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodatabase-0.1.1.tar", last modified: Tue May 28 09:02:35 2024, max compression
+gzip compressed data, was "aiodatabase-0.1.2.tar", last modified: Tue May 28 09:07:31 2024, max compression
```

## Comparing `aiodatabase-0.1.1.tar` & `aiodatabase-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 09:02:35.268797 aiodatabase-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-05-28 09:02:35.264534 aiodatabase-0.1.1/AioDatabase.egg-info/
--rw-rw-rw-   0        0        0      457 2024-05-28 09:02:35.000000 aiodatabase-0.1.1/AioDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-05-28 09:02:35.000000 aiodatabase-0.1.1/AioDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 09:02:35.000000 aiodatabase-0.1.1/AioDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-28 09:02:35.000000 aiodatabase-0.1.1/AioDatabase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-05-28 09:02:35.000000 aiodatabase-0.1.1/AioDatabase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-28 09:02:35.000000 aiodatabase-0.1.1/AioDatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      457 2024-05-28 09:02:35.267651 aiodatabase-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-28 09:02:35.268797 aiodatabase-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      766 2024-05-28 09:01:44.000000 aiodatabase-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:02:35.264534 aiodatabase-0.1.1/src/
--rw-rw-rw-   0        0        0     4533 2024-05-28 08:20:52.000000 aiodatabase-0.1.1/src/AioDatabase.py
--rw-rw-rw-   0        0        0     1552 2024-05-28 08:18:41.000000 aiodatabase-0.1.1/src/DataConnector.py
--rw-rw-rw-   0        0        0       35 2024-05-28 08:15:02.000000 aiodatabase-0.1.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:07:31.579048 aiodatabase-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-05-28 09:07:31.577983 aiodatabase-0.1.2/AioDatabase.egg-info/
+-rw-rw-rw-   0        0        0      457 2024-05-28 09:07:31.000000 aiodatabase-0.1.2/AioDatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-28 09:07:31.000000 aiodatabase-0.1.2/AioDatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 09:07:31.000000 aiodatabase-0.1.2/AioDatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-28 09:07:31.000000 aiodatabase-0.1.2/AioDatabase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-05-28 09:07:31.000000 aiodatabase-0.1.2/AioDatabase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-28 09:07:31.000000 aiodatabase-0.1.2/AioDatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      457 2024-05-28 09:07:31.579048 aiodatabase-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-28 09:07:31.579048 aiodatabase-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      766 2024-05-28 09:05:59.000000 aiodatabase-0.1.2/setup.py
```

### Comparing `aiodatabase-0.1.1/setup.py` & `aiodatabase-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="AioDatabase",
-    version="0.1.1",
+    version="0.1.2",
     packages=["src"],
     install_requires=["PyYAML", "aiomysql", "aiosqlite"],
     entry_points={
         "console_scripts": [
             "aiodatabase=src.AioDatabase:main",
         ],
     },
```

