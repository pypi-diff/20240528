# Comparing `tmp/aiodatabase-0.1.6.tar.gz` & `tmp/aiodatabase-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodatabase-0.1.6.tar", last modified: Tue May 28 10:00:57 2024, max compression
+gzip compressed data, was "aiodatabase-0.1.7.tar", last modified: Tue May 28 11:13:27 2024, max compression
```

## Comparing `aiodatabase-0.1.6.tar` & `aiodatabase-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 10:00:57.117646 aiodatabase-0.1.6/
--rw-rw-rw-   0        0        0     1079 2024-05-28 09:46:29.000000 aiodatabase-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      480 2024-05-28 10:00:57.117646 aiodatabase-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      122 2024-05-28 10:00:57.119256 aiodatabase-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      730 2024-05-28 10:00:43.000000 aiodatabase-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 10:00:57.084914 aiodatabase-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 10:00:57.116649 aiodatabase-0.1.6/src/AioDatabase.egg-info/
--rw-rw-rw-   0        0        0      480 2024-05-28 10:00:57.000000 aiodatabase-0.1.6/src/AioDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2024-05-28 10:00:57.000000 aiodatabase-0.1.6/src/AioDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 10:00:57.000000 aiodatabase-0.1.6/src/AioDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-28 10:00:57.000000 aiodatabase-0.1.6/src/AioDatabase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-28 10:00:57.000000 aiodatabase-0.1.6/src/AioDatabase.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 10:00:57.113563 aiodatabase-0.1.6/src/Manager/
--rw-rw-rw-   0        0        0     2524 2024-05-28 07:15:04.000000 aiodatabase-0.1.6/src/Manager/ConfigManager.py
--rw-rw-rw-   0        0        0        0 2024-05-28 08:09:29.000000 aiodatabase-0.1.6/src/Manager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 10:00:57.114635 aiodatabase-0.1.6/src/sqlite3/
--rw-rw-rw-   0        0        0     1164 2024-05-28 07:16:41.000000 aiodatabase-0.1.6/src/sqlite3/SqlLoader.py
--rw-rw-rw-   0        0        0        0 2024-05-28 08:09:45.000000 aiodatabase-0.1.6/src/sqlite3/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:13:27.053551 aiodatabase-0.1.7/
+-rw-rw-rw-   0        0        0     1079 2024-05-28 09:46:29.000000 aiodatabase-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      480 2024-05-28 11:13:27.053551 aiodatabase-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-28 11:13:27.029029 aiodatabase-0.1.7/aiodatabase/
+-rw-rw-rw-   0        0        0       23 2024-05-28 11:10:53.000000 aiodatabase-0.1.7/aiodatabase/__init__.py
+-rw-rw-rw-   0        0        0     1552 2024-05-28 11:13:13.000000 aiodatabase-0.1.7/aiodatabase/dataConnector.py
+-rw-rw-rw-   0        0        0     4533 2024-05-28 11:06:40.000000 aiodatabase-0.1.7/aiodatabase/database.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:13:27.044738 aiodatabase-0.1.7/aiodatabase/manager/
+-rw-rw-rw-   0        0        0        0 2024-05-28 08:09:29.000000 aiodatabase-0.1.7/aiodatabase/manager/__init__.py
+-rw-rw-rw-   0        0        0     2524 2024-05-28 07:15:04.000000 aiodatabase-0.1.7/aiodatabase/manager/configManager.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:13:27.050262 aiodatabase-0.1.7/aiodatabase/sqlite3/
+-rw-rw-rw-   0        0        0        0 2024-05-28 08:09:45.000000 aiodatabase-0.1.7/aiodatabase/sqlite3/__init__.py
+-rw-rw-rw-   0        0        0     1164 2024-05-28 07:16:41.000000 aiodatabase-0.1.7/aiodatabase/sqlite3/sqlLoader.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:13:27.052551 aiodatabase-0.1.7/aiodatabase.egg-info/
+-rw-rw-rw-   0        0        0      480 2024-05-28 11:13:26.000000 aiodatabase-0.1.7/aiodatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-05-28 11:13:26.000000 aiodatabase-0.1.7/aiodatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 11:13:26.000000 aiodatabase-0.1.7/aiodatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-28 11:13:26.000000 aiodatabase-0.1.7/aiodatabase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-28 11:13:26.000000 aiodatabase-0.1.7/aiodatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 11:13:27.053551 aiodatabase-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      689 2024-05-28 10:31:56.000000 aiodatabase-0.1.7/setup.py
```

### Comparing `aiodatabase-0.1.6/LICENSE` & `aiodatabase-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodatabase-0.1.6/src/Manager/ConfigManager.py` & `aiodatabase-0.1.7/aiodatabase/manager/configManager.py`

 * *Files identical despite different names*

### Comparing `aiodatabase-0.1.6/src/sqlite3/SqlLoader.py` & `aiodatabase-0.1.7/aiodatabase/sqlite3/sqlLoader.py`

 * *Files identical despite different names*

