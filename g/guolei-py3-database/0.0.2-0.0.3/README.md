# Comparing `tmp/guolei_py3_database-0.0.2.tar.gz` & `tmp/guolei_py3_database-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guolei_py3_database-0.0.2.tar", last modified: Tue May 28 01:13:11 2024, max compression
+gzip compressed data, was "guolei_py3_database-0.0.3.tar", last modified: Tue May 28 01:33:02 2024, max compression
```

## Comparing `guolei_py3_database-0.0.2.tar` & `guolei_py3_database-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 guolei     (501) staff       (20)        0 2024-05-28 01:13:11.000621 guolei_py3_database-0.0.2/
--rw-r--r--   0 guolei     (501) staff       (20)     1063 2024-05-27 02:50:52.000000 guolei_py3_database-0.0.2/LICENSE
--rw-r--r--   0 guolei     (501) staff       (20)     3897 2024-05-28 01:13:10.999797 guolei_py3_database-0.0.2/PKG-INFO
--rw-r--r--   0 guolei     (501) staff       (20)     3578 2024-05-27 08:44:18.000000 guolei_py3_database-0.0.2/README.md
-drwxr-xr-x   0 guolei     (501) staff       (20)        0 2024-05-28 01:13:10.998775 guolei_py3_database-0.0.2/guolei_py3_database/
--rw-r--r--   0 guolei     (501) staff       (20)     4629 2024-05-27 08:20:53.000000 guolei_py3_database-0.0.2/guolei_py3_database/__init__.py
--rw-r--r--   0 guolei     (501) staff       (20)     3664 2024-05-28 00:53:31.000000 guolei_py3_database-0.0.2/guolei_py3_database/pymysql.py
--rw-r--r--   0 guolei     (501) staff       (20)     3492 2024-05-28 00:57:56.000000 guolei_py3_database-0.0.2/guolei_py3_database/sqlite3.py
--rw-r--r--   0 guolei     (501) staff       (20)      889 2024-05-28 01:11:24.000000 guolei_py3_database-0.0.2/guolei_py3_database/strictredis.py
-drwxr-xr-x   0 guolei     (501) staff       (20)        0 2024-05-28 01:13:10.999638 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/
--rw-r--r--   0 guolei     (501) staff       (20)     3897 2024-05-28 01:13:10.000000 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/PKG-INFO
--rw-r--r--   0 guolei     (501) staff       (20)      411 2024-05-28 01:13:10.000000 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/SOURCES.txt
--rw-r--r--   0 guolei     (501) staff       (20)        1 2024-05-28 01:13:10.000000 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/dependency_links.txt
--rw-r--r--   0 guolei     (501) staff       (20)        1 2024-05-28 01:12:39.000000 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/not-zip-safe
--rw-r--r--   0 guolei     (501) staff       (20)       22 2024-05-28 01:13:10.000000 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/requires.txt
--rw-r--r--   0 guolei     (501) staff       (20)       20 2024-05-28 01:13:10.000000 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/top_level.txt
--rw-r--r--   0 guolei     (501) staff       (20)       38 2024-05-28 01:13:11.000688 guolei_py3_database-0.0.2/setup.cfg
--rw-r--r--   0 guolei     (501) staff       (20)      705 2024-05-28 01:12:59.000000 guolei_py3_database-0.0.2/setup.py
+drwxr-xr-x   0 guolei     (501) staff       (20)        0 2024-05-28 01:33:02.356191 guolei_py3_database-0.0.3/
+-rw-r--r--   0 guolei     (501) staff       (20)     1063 2024-05-27 02:50:52.000000 guolei_py3_database-0.0.3/LICENSE
+-rw-r--r--   0 guolei     (501) staff       (20)     2592 2024-05-28 01:33:02.355541 guolei_py3_database-0.0.3/PKG-INFO
+-rw-r--r--   0 guolei     (501) staff       (20)     2273 2024-05-28 01:31:36.000000 guolei_py3_database-0.0.3/README.md
+drwxr-xr-x   0 guolei     (501) staff       (20)        0 2024-05-28 01:33:02.354475 guolei_py3_database-0.0.3/guolei_py3_database/
+-rw-r--r--   0 guolei     (501) staff       (20)     4629 2024-05-27 08:20:53.000000 guolei_py3_database-0.0.3/guolei_py3_database/__init__.py
+-rw-r--r--   0 guolei     (501) staff       (20)     3664 2024-05-28 00:53:31.000000 guolei_py3_database-0.0.3/guolei_py3_database/pymysql.py
+-rw-r--r--   0 guolei     (501) staff       (20)     3492 2024-05-28 00:57:56.000000 guolei_py3_database-0.0.3/guolei_py3_database/sqlite3.py
+-rw-r--r--   0 guolei     (501) staff       (20)      889 2024-05-28 01:11:24.000000 guolei_py3_database-0.0.3/guolei_py3_database/strictredis.py
+drwxr-xr-x   0 guolei     (501) staff       (20)        0 2024-05-28 01:33:02.355374 guolei_py3_database-0.0.3/guolei_py3_database.egg-info/
+-rw-r--r--   0 guolei     (501) staff       (20)     2592 2024-05-28 01:33:02.000000 guolei_py3_database-0.0.3/guolei_py3_database.egg-info/PKG-INFO
+-rw-r--r--   0 guolei     (501) staff       (20)      411 2024-05-28 01:33:02.000000 guolei_py3_database-0.0.3/guolei_py3_database.egg-info/SOURCES.txt
+-rw-r--r--   0 guolei     (501) staff       (20)        1 2024-05-28 01:33:02.000000 guolei_py3_database-0.0.3/guolei_py3_database.egg-info/dependency_links.txt
+-rw-r--r--   0 guolei     (501) staff       (20)        1 2024-05-28 01:12:39.000000 guolei_py3_database-0.0.3/guolei_py3_database.egg-info/not-zip-safe
+-rw-r--r--   0 guolei     (501) staff       (20)       22 2024-05-28 01:33:02.000000 guolei_py3_database-0.0.3/guolei_py3_database.egg-info/requires.txt
+-rw-r--r--   0 guolei     (501) staff       (20)       20 2024-05-28 01:33:02.000000 guolei_py3_database-0.0.3/guolei_py3_database.egg-info/top_level.txt
+-rw-r--r--   0 guolei     (501) staff       (20)       38 2024-05-28 01:33:02.356242 guolei_py3_database-0.0.3/setup.cfg
+-rw-r--r--   0 guolei     (501) staff       (20)      705 2024-05-28 01:32:22.000000 guolei_py3_database-0.0.3/setup.py
```

### Comparing `guolei_py3_database-0.0.2/LICENSE` & `guolei_py3_database-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `guolei_py3_database-0.0.2/guolei_py3_database/__init__.py` & `guolei_py3_database-0.0.3/guolei_py3_database/__init__.py`

 * *Files identical despite different names*

### Comparing `guolei_py3_database-0.0.2/guolei_py3_database/pymysql.py` & `guolei_py3_database-0.0.3/guolei_py3_database/pymysql.py`

 * *Files identical despite different names*

### Comparing `guolei_py3_database-0.0.2/guolei_py3_database/sqlite3.py` & `guolei_py3_database-0.0.3/guolei_py3_database/sqlite3.py`

 * *Files identical despite different names*

### Comparing `guolei_py3_database-0.0.2/guolei_py3_database/strictredis.py` & `guolei_py3_database-0.0.3/guolei_py3_database/strictredis.py`

 * *Files identical despite different names*

### Comparing `guolei_py3_database-0.0.2/setup.py` & `guolei_py3_database-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(name="guolei_py3_database",
-      version="00.00.02",
+      version="00.00.03",
       description="a python3 database library by guolei",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/guolei19850528/guolei_py3_database",
       author="guolei",
       author_email="174000902@qq.com",
       license="MIT",
```

