# Comparing `tmp/py-seal-0.0.5.tar.gz` & `tmp/py-seal-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-seal-0.0.5.tar", last modified: Mon May 27 14:07:47 2024, max compression
+gzip compressed data, was "py-seal-0.0.6.tar", last modified: Tue May 28 09:38:30 2024, max compression
```

## Comparing `py-seal-0.0.5.tar` & `py-seal-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:07:47.398083 py-seal-0.0.5/
--rw-r--r--   0 yehao      (501) staff       (20)    35148 2024-05-27 11:31:04.000000 py-seal-0.0.5/LICENSE
--rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-27 14:07:47.397893 py-seal-0.0.5/PKG-INFO
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:07:47.391916 py-seal-0.0.5/py_seal.egg-info/
--rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-27 14:07:47.000000 py-seal-0.0.5/py_seal.egg-info/PKG-INFO
--rw-r--r--   0 yehao      (501) staff       (20)      705 2024-05-27 14:07:47.000000 py-seal-0.0.5/py_seal.egg-info/SOURCES.txt
--rw-r--r--   0 yehao      (501) staff       (20)        1 2024-05-27 14:07:47.000000 py-seal-0.0.5/py_seal.egg-info/dependency_links.txt
--rw-r--r--   0 yehao      (501) staff       (20)        5 2024-05-27 14:07:47.000000 py-seal-0.0.5/py_seal.egg-info/top_level.txt
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:07:47.392145 py-seal-0.0.5/seal/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:53:59.000000 py-seal-0.0.5/seal/__init__.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:07:47.392419 py-seal-0.0.5/seal/config/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:28.000000 py-seal-0.0.5/seal/config/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      309 2024-05-27 11:24:33.000000 py-seal-0.0.5/seal/config/config.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:07:47.393010 py-seal-0.0.5/seal/context/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:22.000000 py-seal-0.0.5/seal/context/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      626 2024-05-27 14:06:18.000000 py-seal-0.0.5/seal/context/context.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:07:47.393502 py-seal-0.0.5/seal/db/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:13.000000 py-seal-0.0.5/seal/db/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      122 2024-05-26 00:07:28.000000 py-seal-0.0.5/seal/db/connector.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:07:47.394637 py-seal-0.0.5/seal/db/mysql/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:13.000000 py-seal-0.0.5/seal/db/mysql/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)    10081 2024-05-27 14:06:34.000000 py-seal-0.0.5/seal/db/mysql/base_mapper.py
--rw-r--r--   0 yehao      (501) staff       (20)     6670 2024-05-27 14:06:49.000000 py-seal-0.0.5/seal/db/mysql/chained_query.py
--rw-r--r--   0 yehao      (501) staff       (20)      737 2024-05-27 14:06:58.000000 py-seal-0.0.5/seal/db/mysql/mysql_connector.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:07:47.395758 py-seal-0.0.5/seal/db/sqlite/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:13.000000 py-seal-0.0.5/seal/db/sqlite/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)     9496 2024-05-27 11:28:12.000000 py-seal-0.0.5/seal/db/sqlite/base_mapper.py
--rw-r--r--   0 yehao      (501) staff       (20)     6388 2024-05-27 11:28:12.000000 py-seal-0.0.5/seal/db/sqlite/chained_query.py
--rw-r--r--   0 yehao      (501) staff       (20)      285 2024-05-27 11:29:16.000000 py-seal-0.0.5/seal/db/sqlite/sqlite_connector.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:07:47.396522 py-seal-0.0.5/seal/model/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:05.000000 py-seal-0.0.5/seal/model/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      292 2024-05-25 14:35:24.000000 py-seal-0.0.5/seal/model/base_entity.py
--rw-r--r--   0 yehao      (501) staff       (20)      563 2024-04-03 02:38:36.000000 py-seal-0.0.5/seal/model/response.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:07:47.397038 py-seal-0.0.5/seal/router/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:10.000000 py-seal-0.0.5/seal/router/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)     2204 2024-05-27 14:07:17.000000 py-seal-0.0.5/seal/router/router.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:07:47.397346 py-seal-0.0.5/seal/wrapper/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:34.000000 py-seal-0.0.5/seal/wrapper/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)     1096 2024-05-26 00:54:07.000000 py-seal-0.0.5/seal/wrapper/decorator.py
--rw-r--r--   0 yehao      (501) staff       (20)       38 2024-05-27 14:07:47.398145 py-seal-0.0.5/setup.cfg
--rw-r--r--   0 yehao      (501) staff       (20)      314 2024-05-27 14:07:39.000000 py-seal-0.0.5/setup.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.314368 py-seal-0.0.6/
+-rw-r--r--   0 yehao      (501) staff       (20)    35148 2024-05-27 11:31:04.000000 py-seal-0.0.6/LICENSE
+-rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-28 09:38:30.314216 py-seal-0.0.6/PKG-INFO
+-rw-r--r--   0 yehao      (501) staff       (20)      772 2024-05-28 06:36:48.000000 py-seal-0.0.6/README.md
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.309059 py-seal-0.0.6/py_seal.egg-info/
+-rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-28 09:38:30.000000 py-seal-0.0.6/py_seal.egg-info/PKG-INFO
+-rw-r--r--   0 yehao      (501) staff       (20)      745 2024-05-28 09:38:30.000000 py-seal-0.0.6/py_seal.egg-info/SOURCES.txt
+-rw-r--r--   0 yehao      (501) staff       (20)        1 2024-05-28 09:38:30.000000 py-seal-0.0.6/py_seal.egg-info/dependency_links.txt
+-rw-r--r--   0 yehao      (501) staff       (20)        5 2024-05-28 09:38:30.000000 py-seal-0.0.6/py_seal.egg-info/top_level.txt
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.309207 py-seal-0.0.6/seal/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/__init__.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.309406 py-seal-0.0.6/seal/config/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/config/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      272 2024-05-28 09:21:01.000000 py-seal-0.0.6/seal/config/configuration.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.309762 py-seal-0.0.6/seal/context/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/context/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      626 2024-05-28 09:21:01.000000 py-seal-0.0.6/seal/context/context.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.310081 py-seal-0.0.6/seal/db/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/db/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      122 2024-05-26 00:07:28.000000 py-seal-0.0.6/seal/db/connector.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.311073 py-seal-0.0.6/seal/db/mysql/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/db/mysql/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)    10004 2024-05-28 08:22:36.000000 py-seal-0.0.6/seal/db/mysql/base_mapper.py
+-rw-r--r--   0 yehao      (501) staff       (20)     6593 2024-05-28 08:22:36.000000 py-seal-0.0.6/seal/db/mysql/chained_query.py
+-rw-r--r--   0 yehao      (501) staff       (20)      774 2024-05-28 09:21:01.000000 py-seal-0.0.6/seal/db/mysql/mysql_connector.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.311856 py-seal-0.0.6/seal/db/sqlite/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/db/sqlite/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)     9437 2024-05-28 08:28:54.000000 py-seal-0.0.6/seal/db/sqlite/base_mapper.py
+-rw-r--r--   0 yehao      (501) staff       (20)     6325 2024-05-28 08:29:03.000000 py-seal-0.0.6/seal/db/sqlite/chained_query.py
+-rw-r--r--   0 yehao      (501) staff       (20)      369 2024-05-28 09:21:01.000000 py-seal-0.0.6/seal/db/sqlite/sqlite_connector.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.312345 py-seal-0.0.6/seal/model/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/model/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      292 2024-05-25 14:35:24.000000 py-seal-0.0.6/seal/model/base_entity.py
+-rw-r--r--   0 yehao      (501) staff       (20)      563 2024-04-03 02:38:36.000000 py-seal-0.0.6/seal/model/response.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.312698 py-seal-0.0.6/seal/router/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/router/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)     2204 2024-05-27 14:07:17.000000 py-seal-0.0.6/seal/router/router.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.313975 py-seal-0.0.6/seal/wrapper/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/wrapper/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      735 2024-05-28 09:09:22.000000 py-seal-0.0.6/seal/wrapper/entity.py
+-rw-r--r--   0 yehao      (501) staff       (20)      767 2024-05-28 09:38:16.000000 py-seal-0.0.6/seal/wrapper/singleton.py
+-rw-r--r--   0 yehao      (501) staff       (20)       38 2024-05-28 09:38:30.314412 py-seal-0.0.6/setup.cfg
+-rw-r--r--   0 yehao      (501) staff       (20)      314 2024-05-28 08:34:13.000000 py-seal-0.0.6/setup.py
```

### Comparing `py-seal-0.0.5/LICENSE` & `py-seal-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.5/py_seal.egg-info/SOURCES.txt` & `py-seal-0.0.6/py_seal.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 LICENSE
+README.md
 setup.py
 py_seal.egg-info/PKG-INFO
 py_seal.egg-info/SOURCES.txt
 py_seal.egg-info/dependency_links.txt
 py_seal.egg-info/top_level.txt
 seal/__init__.py
 seal/config/__init__.py
-seal/config/config.py
+seal/config/configuration.py
 seal/context/__init__.py
 seal/context/context.py
 seal/db/__init__.py
 seal/db/connector.py
 seal/db/mysql/__init__.py
 seal/db/mysql/base_mapper.py
 seal/db/mysql/chained_query.py
@@ -21,8 +22,9 @@
 seal/db/sqlite/sqlite_connector.py
 seal/model/__init__.py
 seal/model/base_entity.py
 seal/model/response.py
 seal/router/__init__.py
 seal/router/router.py
 seal/wrapper/__init__.py
-seal/wrapper/decorator.py
+seal/wrapper/entity.py
+seal/wrapper/singleton.py
```

### Comparing `py-seal-0.0.5/seal/context/context.py` & `py-seal-0.0.6/seal/context/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from contextvars import ContextVar
 
-from seal.wrapper.decorator import singleton
+from seal.wrapper.singleton import singleton
 
 page_ctx = ContextVar('page')
 
 
 @singleton
 class PageContext:
```

### Comparing `py-seal-0.0.5/seal/db/mysql/base_mapper.py` & `py-seal-0.0.6/seal/db/mysql/base_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from datetime import datetime
 from seal.model.base_entity import BaseEntity
 from builtins import list as _list
 from seal.context.context import WebContext
-from seal.config import config
 import abc
 
 from seal.db.mysql.mysql_connector import MysqlConnector
 
 
 class BaseMapper(metaclass=abc.ABCMeta):
 
     def __init__(self, entity_clz):
         self.clz = entity_clz
-        self.placeholder = '?' if config['data_source'] == 'sqlite' else '%s'
+        self.placeholder = '%s'
 
     def all(self):
         """
         Get all entities
         :return: list of entities
         """
         conn = MysqlConnector().get_connection()
```

### Comparing `py-seal-0.0.5/seal/db/mysql/chained_query.py` & `py-seal-0.0.6/seal/db/mysql/chained_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from datetime import datetime
 from seal.context.context import PageContext, WebContext
-from seal.config import config
 from seal.db.mysql.mysql_connector import MysqlConnector
 
 
 class ChainedQuery:
     def __init__(self, entity_clz, logic_delete_col: str = None):
         self.clz = entity_clz
         self.__conditions = [(logic_delete_col if logic_delete_col is not None else 'deleted', 0, '=')]
         self.__select_cols = ()
         self.__sets = {}
         self.__page = ()
         self.__conn = MysqlConnector().get_connection()
         self.__raw = ""
-        self.placeholder = '?' if config['data_source'] == 'sqlite' else '%s'
+        self.placeholder = '%s'
 
     def __cols(self):
         if len(self.__select_cols) == 0:
             return ', '.join(self.clz.columns())
         return ', '.join(self.__select_cols)
 
     def __where(self):
```

### Comparing `py-seal-0.0.5/seal/db/mysql/mysql_connector.py` & `py-seal-0.0.6/seal/db/mysql/mysql_connector.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pymysql
 import pymysql.cursors
-from seal.config import config
+from seal.config.configuration import Configuration
 from seal.db.connector import DBConnector
-from seal.wrapper.decorator import singleton
+from seal.wrapper.singleton import singleton
 
 
 @singleton
 class MysqlConnector(DBConnector):
     def __init__(self):
-        self.config = config['mysql']
+        self.config = Configuration().config['mysql']
         # self.pool = mysql.connector.pooling.MySQLConnectionPool(**self.config)
 
     def get_connection(self):
         # return self.pool.get_connection()
         return pymysql.connect(host=self.config['host'],
                                user=self.config['user'],
                                password=self.config['password'],
```

### Comparing `py-seal-0.0.5/seal/db/sqlite/base_mapper.py` & `py-seal-0.0.6/seal/db/sqlite/base_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from datetime import datetime
-from model.base_entity import BaseEntity
+from seal.model.base_entity import BaseEntity
 from builtins import list as _list
-from context.context import WebContext
-from config import config
+from seal.context.context import WebContext
+from seal.db.sqlite.sqlite_connector import SqliteConnector
 import abc
 
-from db.sqlite.sqlite_connector import SqliteConnector
-
 
 class BaseMapper(metaclass=abc.ABCMeta):
 
     def __init__(self, entity_clz):
         self.clz = entity_clz
-        self.placeholder = '?' if config['data_source'] == 'sqlite' else '%s'
+        self.placeholder = '?'
 
     def all(self):
         """
         Get all entities
         :return: list of entities
         """
         conn = SqliteConnector().get_connection()
```

### Comparing `py-seal-0.0.5/seal/db/sqlite/chained_query.py` & `py-seal-0.0.6/seal/db/sqlite/chained_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from datetime import datetime
-from context.context import PageContext, WebContext
-from config import config
-from db.sqlite.sqlite_connector import SqliteConnector
+from seal.context.context import PageContext, WebContext
+from seal.db.sqlite.sqlite_connector import SqliteConnector
 
 
 class ChainedQuery:
     def __init__(self, entity_clz, logic_delete_col: str = None):
         self.clz = entity_clz
         self.__conditions = [(logic_delete_col if logic_delete_col is not None else 'deleted', 0, '=')]
         self.__select_cols = ()
         self.__sets = {}
         self.__page = ()
         self.__conn = SqliteConnector().get_connection()
         self.__raw = ""
-        self.placeholder = '?' if config['data_source'] == 'sqlite' else '%s'
+        self.placeholder = '?'
 
     def __cols(self):
         if len(self.__select_cols) == 0:
             return ', '.join(self.clz.columns())
         return ', '.join(self.__select_cols)
 
     def __where(self):
```

### Comparing `py-seal-0.0.5/seal/model/response.py` & `py-seal-0.0.6/seal/model/response.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.5/seal/router/router.py` & `py-seal-0.0.6/seal/router/router.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.5/seal/wrapper/decorator.py` & `py-seal-0.0.6/seal/wrapper/entity.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from functools import wraps
 from boltons import strutils
 
 
 def parametrized(decorator):
     def layer(*args, **kwargs):
         def repl(cls):
             return decorator(cls, *args, **kwargs)
@@ -24,22 +23,7 @@
         if table is not None:
             return table
         return strutils.camel2under(cls.__name__)
 
     setattr(cls, 'columns', columns)
     setattr(cls, 'table_name', table_name)
     return cls
-
-
-def singleton(orig_cls):
-    orig_new = orig_cls.__new__
-    instance = None
-
-    @wraps(orig_cls.__new__)
-    def __new__(cls, *args, **kwargs):
-        nonlocal instance
-        if instance is None:
-            instance = orig_new(cls, *args, **kwargs)
-        return instance
-
-    orig_cls.__new__ = __new__
-    return orig_cls
```

