# Comparing `tmp/guolei_py3_database-0.0.1.tar.gz` & `tmp/guolei_py3_database-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guolei_py3_database-0.0.1.tar", last modified: Mon May 27 08:49:52 2024, max compression
+gzip compressed data, was "guolei_py3_database-0.0.2.tar", last modified: Tue May 28 01:13:11 2024, max compression
```

## Comparing `guolei_py3_database-0.0.1.tar` & `guolei_py3_database-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 guolei     (501) staff       (20)        0 2024-05-27 08:49:52.322664 guolei_py3_database-0.0.1/
--rw-r--r--   0 guolei     (501) staff       (20)     1063 2024-05-27 02:50:52.000000 guolei_py3_database-0.0.1/LICENSE
--rw-r--r--   0 guolei     (501) staff       (20)     3897 2024-05-27 08:49:52.321740 guolei_py3_database-0.0.1/PKG-INFO
--rw-r--r--   0 guolei     (501) staff       (20)     3578 2024-05-27 08:44:18.000000 guolei_py3_database-0.0.1/README.md
-drwxr-xr-x   0 guolei     (501) staff       (20)        0 2024-05-27 08:49:52.320525 guolei_py3_database-0.0.1/guolei_py3_database/
--rw-r--r--   0 guolei     (501) staff       (20)     4629 2024-05-27 08:20:53.000000 guolei_py3_database-0.0.1/guolei_py3_database/__init__.py
--rw-r--r--   0 guolei     (501) staff       (20)     8271 2024-05-27 05:31:55.000000 guolei_py3_database-0.0.1/guolei_py3_database/pymysql.py
--rw-r--r--   0 guolei     (501) staff       (20)     7906 2024-05-27 07:34:00.000000 guolei_py3_database-0.0.1/guolei_py3_database/sqlite3.py
--rw-r--r--   0 guolei     (501) staff       (20)     2126 2024-05-27 07:47:02.000000 guolei_py3_database-0.0.1/guolei_py3_database/strictredis.py
-drwxr-xr-x   0 guolei     (501) staff       (20)        0 2024-05-27 08:49:52.321529 guolei_py3_database-0.0.1/guolei_py3_database.egg-info/
--rw-r--r--   0 guolei     (501) staff       (20)     3897 2024-05-27 08:49:52.000000 guolei_py3_database-0.0.1/guolei_py3_database.egg-info/PKG-INFO
--rw-r--r--   0 guolei     (501) staff       (20)      411 2024-05-27 08:49:52.000000 guolei_py3_database-0.0.1/guolei_py3_database.egg-info/SOURCES.txt
--rw-r--r--   0 guolei     (501) staff       (20)        1 2024-05-27 08:49:52.000000 guolei_py3_database-0.0.1/guolei_py3_database.egg-info/dependency_links.txt
--rw-r--r--   0 guolei     (501) staff       (20)        1 2024-05-27 08:48:55.000000 guolei_py3_database-0.0.1/guolei_py3_database.egg-info/not-zip-safe
--rw-r--r--   0 guolei     (501) staff       (20)       22 2024-05-27 08:49:52.000000 guolei_py3_database-0.0.1/guolei_py3_database.egg-info/requires.txt
--rw-r--r--   0 guolei     (501) staff       (20)       20 2024-05-27 08:49:52.000000 guolei_py3_database-0.0.1/guolei_py3_database.egg-info/top_level.txt
--rw-r--r--   0 guolei     (501) staff       (20)       38 2024-05-27 08:49:52.322728 guolei_py3_database-0.0.1/setup.cfg
--rw-r--r--   0 guolei     (501) staff       (20)      705 2024-05-27 08:49:48.000000 guolei_py3_database-0.0.1/setup.py
+drwxr-xr-x   0 guolei     (501) staff       (20)        0 2024-05-28 01:13:11.000621 guolei_py3_database-0.0.2/
+-rw-r--r--   0 guolei     (501) staff       (20)     1063 2024-05-27 02:50:52.000000 guolei_py3_database-0.0.2/LICENSE
+-rw-r--r--   0 guolei     (501) staff       (20)     3897 2024-05-28 01:13:10.999797 guolei_py3_database-0.0.2/PKG-INFO
+-rw-r--r--   0 guolei     (501) staff       (20)     3578 2024-05-27 08:44:18.000000 guolei_py3_database-0.0.2/README.md
+drwxr-xr-x   0 guolei     (501) staff       (20)        0 2024-05-28 01:13:10.998775 guolei_py3_database-0.0.2/guolei_py3_database/
+-rw-r--r--   0 guolei     (501) staff       (20)     4629 2024-05-27 08:20:53.000000 guolei_py3_database-0.0.2/guolei_py3_database/__init__.py
+-rw-r--r--   0 guolei     (501) staff       (20)     3664 2024-05-28 00:53:31.000000 guolei_py3_database-0.0.2/guolei_py3_database/pymysql.py
+-rw-r--r--   0 guolei     (501) staff       (20)     3492 2024-05-28 00:57:56.000000 guolei_py3_database-0.0.2/guolei_py3_database/sqlite3.py
+-rw-r--r--   0 guolei     (501) staff       (20)      889 2024-05-28 01:11:24.000000 guolei_py3_database-0.0.2/guolei_py3_database/strictredis.py
+drwxr-xr-x   0 guolei     (501) staff       (20)        0 2024-05-28 01:13:10.999638 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/
+-rw-r--r--   0 guolei     (501) staff       (20)     3897 2024-05-28 01:13:10.000000 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/PKG-INFO
+-rw-r--r--   0 guolei     (501) staff       (20)      411 2024-05-28 01:13:10.000000 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/SOURCES.txt
+-rw-r--r--   0 guolei     (501) staff       (20)        1 2024-05-28 01:13:10.000000 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/dependency_links.txt
+-rw-r--r--   0 guolei     (501) staff       (20)        1 2024-05-28 01:12:39.000000 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/not-zip-safe
+-rw-r--r--   0 guolei     (501) staff       (20)       22 2024-05-28 01:13:10.000000 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/requires.txt
+-rw-r--r--   0 guolei     (501) staff       (20)       20 2024-05-28 01:13:10.000000 guolei_py3_database-0.0.2/guolei_py3_database.egg-info/top_level.txt
+-rw-r--r--   0 guolei     (501) staff       (20)       38 2024-05-28 01:13:11.000688 guolei_py3_database-0.0.2/setup.cfg
+-rw-r--r--   0 guolei     (501) staff       (20)      705 2024-05-28 01:12:59.000000 guolei_py3_database-0.0.2/setup.py
```

### Comparing `guolei_py3_database-0.0.1/LICENSE` & `guolei_py3_database-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `guolei_py3_database-0.0.1/PKG-INFO` & `guolei_py3_database-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guolei_py3_database
-Version: 0.0.1
+Version: 0.0.2
 Summary: a python3 database library by guolei
 Home-page: https://github.com/guolei19850528/guolei_py3_database
 Author: guolei
 Author-email: 174000902@qq.com
 License: MIT
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `guolei_py3_database-0.0.1/README.md` & `guolei_py3_database-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `guolei_py3_database-0.0.1/guolei_py3_database/__init__.py` & `guolei_py3_database-0.0.2/guolei_py3_database/__init__.py`

 * *Files identical despite different names*

### Comparing `guolei_py3_database-0.0.1/guolei_py3_database.egg-info/PKG-INFO` & `guolei_py3_database-0.0.2/guolei_py3_database.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guolei-py3-database
-Version: 0.0.1
+Version: 0.0.2
 Summary: a python3 database library by guolei
 Home-page: https://github.com/guolei19850528/guolei_py3_database
 Author: guolei
 Author-email: 174000902@qq.com
 License: MIT
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `guolei_py3_database-0.0.1/setup.py` & `guolei_py3_database-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(name="guolei_py3_database",
-      version="00.00.01",
+      version="00.00.02",
       description="a python3 database library by guolei",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/guolei19850528/guolei_py3_database",
       author="guolei",
       author_email="174000902@qq.com",
       license="MIT",
```

