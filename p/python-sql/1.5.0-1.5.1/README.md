# Comparing `tmp/python_sql-1.5.0.tar.gz` & `tmp/python_sql-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_sql-1.5.0.tar", last modified: Mon May 13 16:52:16 2024, max compression
+gzip compressed data, was "python_sql-1.5.1.tar", last modified: Tue May 28 16:00:47 2024, max compression
```

## Comparing `python_sql-1.5.0.tar` & `python_sql-1.5.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-13 16:52:16.977754 python_sql-1.5.0/
--rw-r--r--   0 ced       (1000) ced       (1000)       41 2020-02-29 23:00:32.000000 python_sql-1.5.0/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1360 2024-03-07 16:01:58.000000 python_sql-1.5.0/.gitlab-ci.yml
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2024-05-13 16:51:40.000000 python_sql-1.5.0/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       31 2021-12-18 00:47:59.000000 python_sql-1.5.0/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     3109 2024-05-13 16:51:04.000000 python_sql-1.5.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)     1576 2023-06-25 09:03:37.000000 python_sql-1.5.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)       55 2023-03-02 21:12:39.000000 python_sql-1.5.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     8514 2024-05-13 16:52:16.977754 python_sql-1.5.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     7265 2021-09-10 11:50:13.000000 python_sql-1.5.0/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-13 16:52:16.977754 python_sql-1.5.0/python_sql.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     8514 2024-05-13 16:52:16.000000 python_sql-1.5.0/python_sql.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      956 2024-05-13 16:52:16.000000 python_sql-1.5.0/python_sql.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-13 16:52:16.000000 python_sql-1.5.0/python_sql.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        4 2024-05-13 16:52:16.000000 python_sql-1.5.0/python_sql.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-13 16:52:16.977754 python_sql-1.5.0/setup.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1922 2023-10-07 13:08:26.000000 python_sql-1.5.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-13 16:52:16.974421 python_sql-1.5.0/sql/
--rw-r--r--   0 ced       (1000) ced       (1000)    59923 2024-05-13 16:50:38.000000 python_sql-1.5.0/sql/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5241 2022-01-29 01:09:33.000000 python_sql-1.5.0/sql/aggregate.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2541 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/conditionals.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12373 2024-05-06 07:52:59.000000 python_sql-1.5.0/sql/functions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10788 2024-03-07 16:01:58.000000 python_sql-1.5.0/sql/operators.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-13 16:52:16.977754 python_sql-1.5.0/sql/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      675 2022-04-27 16:41:54.000000 python_sql-1.5.0/sql/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2592 2022-01-28 11:56:33.000000 python_sql-1.5.0/sql/tests/test_aggregate.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_alias.py
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_as.py
--rw-r--r--   0 ced       (1000) ced       (1000)      653 2021-09-14 07:32:05.000000 python_sql-1.5.0/sql/tests/test_cast.py
--rw-r--r--   0 ced       (1000) ced       (1000)      842 2021-09-14 07:32:14.000000 python_sql-1.5.0/sql/tests/test_collate.py
--rw-r--r--   0 ced       (1000) ced       (1000)      866 2022-04-27 16:41:54.000000 python_sql-1.5.0/sql/tests/test_column.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2277 2023-12-10 22:48:45.000000 python_sql-1.5.0/sql/tests/test_combining_query.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2705 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_conditionals.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1591 2021-09-14 07:32:51.000000 python_sql-1.5.0/sql/tests/test_delete.py
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2021-09-14 07:33:00.000000 python_sql-1.5.0/sql/tests/test_for.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5377 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_functions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7378 2024-05-12 06:43:27.000000 python_sql-1.5.0/sql/tests/test_insert.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1891 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_join.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1046 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_lateral.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1010 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_literal.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4074 2024-05-12 06:35:08.000000 python_sql-1.5.0/sql/tests/test_merge.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15542 2024-03-07 16:01:58.000000 python_sql-1.5.0/sql/tests/test_operators.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1996 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_order.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19882 2024-03-07 16:01:58.000000 python_sql-1.5.0/sql/tests/test_select.py
--rw-r--r--   0 ced       (1000) ced       (1000)      758 2021-09-14 07:34:28.000000 python_sql-1.5.0/sql/tests/test_table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3490 2023-06-18 08:11:33.000000 python_sql-1.5.0/sql/tests/test_update.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1053 2021-09-14 07:34:49.000000 python_sql-1.5.0/sql/tests/test_values.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2383 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_window.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2256 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_with.py
--rw-r--r--   0 ced       (1000) ced       (1000)      583 2024-03-07 16:01:58.000000 python_sql-1.5.0/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-28 16:00:47.983760 python_sql-1.5.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)       41 2020-02-29 23:00:32.000000 python_sql-1.5.1/.flake8
+-rw-r--r--   0 ced       (1000) ced       (1000)     1360 2024-03-07 16:01:58.000000 python_sql-1.5.1/.gitlab-ci.yml
+-rw-r--r--   0 ced       (1000) ced       (1000)      969 2024-05-28 16:00:06.000000 python_sql-1.5.1/.hgtags
+-rw-r--r--   0 ced       (1000) ced       (1000)       31 2021-12-18 00:47:59.000000 python_sql-1.5.1/.isort.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     3224 2024-05-28 15:59:32.000000 python_sql-1.5.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)     1576 2023-06-25 09:03:37.000000 python_sql-1.5.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)       55 2023-03-02 21:12:39.000000 python_sql-1.5.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     8514 2024-05-28 16:00:47.983760 python_sql-1.5.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     7265 2021-09-10 11:50:13.000000 python_sql-1.5.1/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-28 16:00:47.983760 python_sql-1.5.1/python_sql.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8514 2024-05-28 16:00:47.000000 python_sql-1.5.1/python_sql.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      956 2024-05-28 16:00:47.000000 python_sql-1.5.1/python_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-28 16:00:47.000000 python_sql-1.5.1/python_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        4 2024-05-28 16:00:47.000000 python_sql-1.5.1/python_sql.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-28 16:00:47.983760 python_sql-1.5.1/setup.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1922 2023-10-07 13:08:26.000000 python_sql-1.5.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-28 16:00:47.983760 python_sql-1.5.1/sql/
+-rw-r--r--   0 ced       (1000) ced       (1000)    60610 2024-05-28 15:58:58.000000 python_sql-1.5.1/sql/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5241 2024-05-28 15:58:58.000000 python_sql-1.5.1/sql/aggregate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2541 2021-12-18 00:48:19.000000 python_sql-1.5.1/sql/conditionals.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12373 2024-05-28 15:58:58.000000 python_sql-1.5.1/sql/functions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10788 2024-05-28 15:58:58.000000 python_sql-1.5.1/sql/operators.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-28 16:00:47.983760 python_sql-1.5.1/sql/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      675 2022-04-27 16:41:54.000000 python_sql-1.5.1/sql/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2592 2022-01-28 11:56:33.000000 python_sql-1.5.1/sql/tests/test_aggregate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2021-12-18 00:48:19.000000 python_sql-1.5.1/sql/tests/test_alias.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2021-12-18 00:48:19.000000 python_sql-1.5.1/sql/tests/test_as.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      653 2021-09-14 07:32:05.000000 python_sql-1.5.1/sql/tests/test_cast.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      842 2021-09-14 07:32:14.000000 python_sql-1.5.1/sql/tests/test_collate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      866 2022-04-27 16:41:54.000000 python_sql-1.5.1/sql/tests/test_column.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2277 2023-12-10 22:48:45.000000 python_sql-1.5.1/sql/tests/test_combining_query.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2705 2021-12-18 00:48:19.000000 python_sql-1.5.1/sql/tests/test_conditionals.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1591 2021-09-14 07:32:51.000000 python_sql-1.5.1/sql/tests/test_delete.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2021-09-14 07:33:00.000000 python_sql-1.5.1/sql/tests/test_for.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5377 2021-12-18 00:48:19.000000 python_sql-1.5.1/sql/tests/test_functions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7378 2024-05-12 06:43:27.000000 python_sql-1.5.1/sql/tests/test_insert.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1891 2021-12-18 00:48:19.000000 python_sql-1.5.1/sql/tests/test_join.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1046 2021-12-18 00:48:19.000000 python_sql-1.5.1/sql/tests/test_lateral.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1010 2021-12-18 00:48:19.000000 python_sql-1.5.1/sql/tests/test_literal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4074 2024-05-12 06:35:08.000000 python_sql-1.5.1/sql/tests/test_merge.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15542 2024-03-07 16:01:58.000000 python_sql-1.5.1/sql/tests/test_operators.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1996 2021-12-18 00:48:19.000000 python_sql-1.5.1/sql/tests/test_order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19903 2024-05-27 16:10:47.000000 python_sql-1.5.1/sql/tests/test_select.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      758 2021-09-14 07:34:28.000000 python_sql-1.5.1/sql/tests/test_table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3490 2023-06-18 08:11:33.000000 python_sql-1.5.1/sql/tests/test_update.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1053 2021-09-14 07:34:49.000000 python_sql-1.5.1/sql/tests/test_values.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2392 2024-05-27 16:58:40.000000 python_sql-1.5.1/sql/tests/test_window.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2256 2021-12-18 00:48:19.000000 python_sql-1.5.1/sql/tests/test_with.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      583 2024-03-07 16:01:58.000000 python_sql-1.5.1/tox.ini
```

### Comparing `python_sql-1.5.0/.gitlab-ci.yml` & `python_sql-1.5.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/.hgtags` & `python_sql-1.5.1/.hgtags`

 * *Files 6% similar despite different names*

```diff
@@ -14,7 +14,8 @@
 1c38ffeacbb82a9ff6ae3568cdc017dbbeddff5d 1.2.2
 edc03ee84f0ac96d403d8f984d59fffa3274cd2f 1.3.0
 a317c40a4d60089ba9e465fbd64b78df24f9e890 1.4.0
 e71bbae3398cb6a0e72f97a0cada9fcdee2bddea 1.4.1
 fcb64787b51db2068061eb4aa13825abc1134916 1.4.2
 111e3e86865360f83a65c04fa48c55f3d2957ee3 1.4.3
 6f9066b83fe3a8c4699a8555ad1bc406f18974ff 1.5.0
+79a69b0bbbd35a8d95e1b754ed3feb03df23fb70 1.5.1
```

### Comparing `python_sql-1.5.0/CHANGELOG` & `python_sql-1.5.1/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+Version 1.5.1 - 2024-05-28
+* Use parameter for start and end of WINDOW FRAME
+* Use parameter for limit and offset
+
 Version 1.5.0 - 2024-05-13
 * Skip alias on INSERT without ON CONFLICT or RETURNING
 * Add MERGE
 * Support UPSERT
 * Remove default escape char on LIKE and ILIKE
 * Add GROUPING SETS, CUBE, and ROLLUP
```

### Comparing `python_sql-1.5.0/COPYRIGHT` & `python_sql-1.5.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/PKG-INFO` & `python_sql-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sql
-Version: 1.5.0
+Version: 1.5.1
 Summary: Library to write SQL queries
 Home-page: https://pypi.org/project/python-sql/
 Download-URL: https://downloads.tryton.org/python-sql/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: BSD
 Project-URL: Bug Tracker, https://bugs.tryton.org/python-sql
```

### Comparing `python_sql-1.5.0/README.rst` & `python_sql-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/python_sql.egg-info/PKG-INFO` & `python_sql-1.5.1/python_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sql
-Version: 1.5.0
+Version: 1.5.1
 Summary: Library to write SQL queries
 Home-page: https://pypi.org/project/python-sql/
 Download-URL: https://downloads.tryton.org/python-sql/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: BSD
 Project-URL: Bug Tracker, https://bugs.tryton.org/python-sql
```

### Comparing `python_sql-1.5.0/python_sql.egg-info/SOURCES.txt` & `python_sql-1.5.1/python_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/setup.py` & `python_sql-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/__init__.py` & `python_sql-1.5.1/sql/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numbers
 import string
 import warnings
 from collections import defaultdict
 from itertools import chain
 from threading import current_thread, local
 
-__version__ = '1.5.0'
+__version__ = '1.5.1'
 __all__ = [
     'Flavor', 'Table', 'Values', 'Literal', 'Column', 'Grouping', 'Conflict',
     'Matched', 'MatchedUpdate', 'MatchedDelete',
     'NotMatched', 'NotMatchedInsert',
     'Rollup', 'Cube', 'Excluded', 'Join', 'Asc', 'Desc', 'NullsFirst',
     'NullsLast', 'format2numeric']
 
@@ -376,35 +376,51 @@
     def offset(self, value):
         if value is not None:
             assert isinstance(value, numbers.Integral)
         self._offset = value
 
     @property
     def _limit_offset_str(self):
+        param = Flavor.get().param
         if Flavor.get().limitstyle == 'limit':
             offset = ''
             if self.offset:
-                offset = ' OFFSET %s' % self.offset
+                offset = ' OFFSET %s' % param
             limit = ''
             if self.limit is not None:
-                limit = ' LIMIT %s' % self.limit
+                limit = ' LIMIT %s' % param
             elif self.offset:
                 max_limit = Flavor.get().max_limit
                 if max_limit:
                     limit = ' LIMIT %s' % max_limit
             return limit + offset
         else:
             offset = ''
             if self.offset:
-                offset = ' OFFSET (%s) ROWS' % self.offset
+                offset = ' OFFSET (%s) ROWS' % param
             fetch = ''
             if self.limit is not None:
-                fetch = ' FETCH FIRST (%s) ROWS ONLY' % self.limit
+                fetch = ' FETCH FIRST (%s) ROWS ONLY' % param
             return offset + fetch
 
+    @property
+    def _limit_offset_params(self):
+        p = []
+        if Flavor.get().limitstyle == 'limit':
+            if self.limit is not None:
+                p.append(self.limit)
+            if self.offset:
+                p.append(self.offset)
+        else:
+            if self.offset:
+                p.append(self.offset)
+            if self.limit is not None:
+                p.append(self.limit)
+        return tuple(p)
+
     def as_(self, output_name):
         return As(self, output_name)
 
 
 class Select(FromItem, SelectQuery):
     __slots__ = ('_columns', '_where', '_group_by', '_having', '_for_',
         'from_', '_distinct', '_distinct_on', '_windows')
@@ -659,14 +675,15 @@
             if self.order_by:
                 for expression in self.order_by:
                     p.extend(expression.params)
             if self.having:
                 p.extend(self.having.params)
             for window in self.windows:
                 p.extend(window.params)
+            p.extend(self._limit_offset_params)
         return tuple(p)
 
 
 class Insert(WithQuery):
     __slots__ = ('_table', '_columns', '_values', '_on_conflict', '_returning')
 
     def __init__(
@@ -1988,30 +2005,31 @@
         return AliasManager.get(self)
 
     @property
     def has_alias(self):
         return AliasManager.contains(self)
 
     def __str__(self):
+        param = Flavor.get().param
         partition = ''
         if self.partition:
             partition = 'PARTITION BY ' + ', '.join(map(str, self.partition))
         order_by = ''
         if self.order_by:
             order_by = ' ORDER BY ' + ', '.join(map(str, self.order_by))
 
         def format(frame, direction):
             if frame is None:
                 return 'UNBOUNDED %s' % direction
             elif not frame:
                 return 'CURRENT ROW'
             elif frame < 0:
-                return '%s PRECEDING' % -frame
+                return '%s PRECEDING' % param
             elif frame > 0:
-                return '%s FOLLOWING' % frame
+                return '%s FOLLOWING' % param
 
         frame = ''
         if self.frame:
             start = format(self.start, 'PRECEDING')
             end = format(self.end, 'FOLLOWING')
             frame = ' %s BETWEEN %s AND %s' % (self.frame, start, end)
         exclude = ''
@@ -2024,14 +2042,19 @@
         p = []
         if self.partition:
             for expression in self.partition:
                 p.extend(expression.params)
         if self.order_by:
             for expression in self.order_by:
                 p.extend(expression.params)
+        if self.frame:
+            if self.start:
+                p.append(abs(self.start))
+            if self.end:
+                p.append(abs(self.end))
         return tuple(p)
 
 
 class Order(Expression):
     __slots__ = ('_expression')
     _sql = ''
```

### Comparing `python_sql-1.5.0/sql/aggregate.py` & `python_sql-1.5.1/sql/aggregate.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/conditionals.py` & `python_sql-1.5.1/sql/conditionals.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/functions.py` & `python_sql-1.5.1/sql/functions.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/operators.py` & `python_sql-1.5.1/sql/operators.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/__init__.py` & `python_sql-1.5.1/sql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_aggregate.py` & `python_sql-1.5.1/sql/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_alias.py` & `python_sql-1.5.1/sql/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_as.py` & `python_sql-1.5.1/sql/tests/test_as.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_cast.py` & `python_sql-1.5.1/sql/tests/test_cast.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_collate.py` & `python_sql-1.5.1/sql/tests/test_collate.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_column.py` & `python_sql-1.5.1/sql/tests/test_column.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_combining_query.py` & `python_sql-1.5.1/sql/tests/test_combining_query.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_conditionals.py` & `python_sql-1.5.1/sql/tests/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_delete.py` & `python_sql-1.5.1/sql/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_for.py` & `python_sql-1.5.1/sql/tests/test_for.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_functions.py` & `python_sql-1.5.1/sql/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_insert.py` & `python_sql-1.5.1/sql/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_join.py` & `python_sql-1.5.1/sql/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_lateral.py` & `python_sql-1.5.1/sql/tests/test_lateral.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_literal.py` & `python_sql-1.5.1/sql/tests/test_literal.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_merge.py` & `python_sql-1.5.1/sql/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_operators.py` & `python_sql-1.5.1/sql/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_order.py` & `python_sql-1.5.1/sql/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_select.py` & `python_sql-1.5.1/sql/tests/test_select.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,21 +249,21 @@
         self.assertEqual(tuple(query.params), (1,))
 
     def test_select_limit_offset(self):
         try:
             Flavor.set(Flavor(limitstyle='limit'))
             query = self.table.select(limit=50, offset=10)
             self.assertEqual(str(query),
-                'SELECT * FROM "t" AS "a" LIMIT 50 OFFSET 10')
-            self.assertEqual(tuple(query.params), ())
+                'SELECT * FROM "t" AS "a" LIMIT %s OFFSET %s')
+            self.assertEqual(tuple(query.params), (50, 10))
 
             query.limit = None
             self.assertEqual(str(query),
-                'SELECT * FROM "t" AS "a" OFFSET 10')
-            self.assertEqual(tuple(query.params), ())
+                'SELECT * FROM "t" AS "a" OFFSET %s')
+            self.assertEqual(tuple(query.params), (10,))
 
             query.offset = 0
             self.assertEqual(str(query),
                 'SELECT * FROM "t" AS "a"')
             self.assertEqual(tuple(query.params), ())
 
             Flavor.set(Flavor(limitstyle='limit', max_limit=-1))
@@ -276,32 +276,32 @@
             query.offset = 0
             self.assertEqual(str(query),
                 'SELECT * FROM "t" AS "a"')
             self.assertEqual(tuple(query.params), ())
 
             query.offset = 10
             self.assertEqual(str(query),
-                'SELECT * FROM "t" AS "a" LIMIT -1 OFFSET 10')
-            self.assertEqual(tuple(query.params), ())
+                'SELECT * FROM "t" AS "a" LIMIT -1 OFFSET %s')
+            self.assertEqual(tuple(query.params), (10,))
         finally:
             Flavor.set(Flavor())
 
     def test_select_offset_fetch(self):
         try:
             Flavor.set(Flavor(limitstyle='fetch'))
             query = self.table.select(limit=50, offset=10)
             self.assertEqual(str(query),
                 'SELECT * FROM "t" AS "a" '
-                'OFFSET (10) ROWS FETCH FIRST (50) ROWS ONLY')
-            self.assertEqual(tuple(query.params), ())
+                'OFFSET (%s) ROWS FETCH FIRST (%s) ROWS ONLY')
+            self.assertEqual(tuple(query.params), (10, 50))
 
             query.limit = None
             self.assertEqual(str(query),
-                'SELECT * FROM "t" AS "a" OFFSET (10) ROWS')
-            self.assertEqual(tuple(query.params), ())
+                'SELECT * FROM "t" AS "a" OFFSET (%s) ROWS')
+            self.assertEqual(tuple(query.params), (10,))
 
             query.offset = 0
             self.assertEqual(str(query),
                 'SELECT * FROM "t" AS "a"')
             self.assertEqual(tuple(query.params), ())
         finally:
             Flavor.set(Flavor())
```

### Comparing `python_sql-1.5.0/sql/tests/test_table.py` & `python_sql-1.5.1/sql/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_update.py` & `python_sql-1.5.1/sql/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_values.py` & `python_sql-1.5.1/sql/tests/test_values.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/sql/tests/test_window.py` & `python_sql-1.5.1/sql/tests/test_window.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,30 +29,30 @@
             'PARTITION BY "c" RANGE '
             'BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW')
         self.assertEqual(window.params, ())
 
         window.start = -1
         self.assertEqual(str(window),
             'PARTITION BY "c" RANGE '
-            'BETWEEN 1 PRECEDING AND CURRENT ROW')
-        self.assertEqual(window.params, ())
+            'BETWEEN %s PRECEDING AND CURRENT ROW')
+        self.assertEqual(window.params, (1,))
 
         window.start = 0
         window.end = 1
         self.assertEqual(str(window),
             'PARTITION BY "c" RANGE '
-            'BETWEEN CURRENT ROW AND 1 FOLLOWING')
-        self.assertEqual(window.params, ())
+            'BETWEEN CURRENT ROW AND %s FOLLOWING')
+        self.assertEqual(window.params, (1,))
 
         window.start = 1
         window.end = None
         self.assertEqual(str(window),
             'PARTITION BY "c" RANGE '
-            'BETWEEN 1 FOLLOWING AND UNBOUNDED FOLLOWING')
-        self.assertEqual(window.params, ())
+            'BETWEEN %s FOLLOWING AND UNBOUNDED FOLLOWING')
+        self.assertEqual(window.params, (1,))
 
     def test_window_exclude(self):
         t = Table('t')
         window = Window([t.c], exclude='TIES')
 
         self.assertEqual(str(window),
             'PARTITION BY "c" EXCLUDE TIES')
```

### Comparing `python_sql-1.5.0/sql/tests/test_with.py` & `python_sql-1.5.1/sql/tests/test_with.py`

 * *Files identical despite different names*

### Comparing `python_sql-1.5.0/tox.ini` & `python_sql-1.5.1/tox.ini`

 * *Files identical despite different names*

