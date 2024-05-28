# Comparing `tmp/jao-py-0.4.5.tar.gz` & `tmp/jao_py-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jao-py-0.4.5.tar", last modified: Fri Apr  5 07:33:17 2024, max compression
+gzip compressed data, was "jao_py-0.4.6.tar", last modified: Tue May 28 21:51:08 2024, max compression
```

## Comparing `jao-py-0.4.5.tar` & `jao_py-0.4.6.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:33:17.776136 jao-py-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 07:33:14.000000 jao-py-0.4.5/LICENSE.MD
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-05 07:33:17.776136 jao-py-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-05 07:33:14.000000 jao-py-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:33:17.772136 jao-py-0.4.5/jao/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:33:17.776136 jao-py-0.4.5/jao/CWE/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/CWE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/CWE/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/CWE/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14485 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/CWE/jao.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/CWE/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/jao.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/jao_par_run.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-05 07:33:14.000000 jao-py-0.4.5/jao/webservice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:33:17.776136 jao-py-0.4.5/jao_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-05 07:33:17.000000 jao-py-0.4.5/jao_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-05 07:33:17.000000 jao-py-0.4.5/jao_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:33:17.000000 jao-py-0.4.5/jao_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 07:33:17.000000 jao-py-0.4.5/jao_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 07:33:17.000000 jao-py-0.4.5/jao_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 07:33:17.776136 jao-py-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-05 07:33:14.000000 jao-py-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:51:08.217921 jao_py-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-28 21:51:04.000000 jao_py-0.4.6/LICENSE.MD
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-28 21:51:08.217921 jao_py-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-28 21:51:04.000000 jao_py-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:51:08.213921 jao_py-0.4.6/jao/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:51:08.217921 jao_py-0.4.6/jao/CWE/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-28 21:51:04.000000 jao_py-0.4.6/jao/CWE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-28 21:51:04.000000 jao_py-0.4.6/jao/CWE/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 21:51:04.000000 jao_py-0.4.6/jao/CWE/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14485 2024-05-28 21:51:04.000000 jao_py-0.4.6/jao/CWE/jao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-28 21:51:04.000000 jao_py-0.4.6/jao/CWE/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 21:51:04.000000 jao_py-0.4.6/jao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 21:51:04.000000 jao_py-0.4.6/jao/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-28 21:51:04.000000 jao_py-0.4.6/jao/jao.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-28 21:51:04.000000 jao_py-0.4.6/jao/jao_par_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-28 21:51:04.000000 jao_py-0.4.6/jao/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 21:51:04.000000 jao_py-0.4.6/jao/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-28 21:51:04.000000 jao_py-0.4.6/jao/webservice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:51:08.217921 jao_py-0.4.6/jao_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-28 21:51:08.000000 jao_py-0.4.6/jao_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-28 21:51:08.000000 jao_py-0.4.6/jao_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:51:08.000000 jao_py-0.4.6/jao_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 21:51:08.000000 jao_py-0.4.6/jao_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 21:51:08.000000 jao_py-0.4.6/jao_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 21:51:08.217921 jao_py-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-28 21:51:04.000000 jao_py-0.4.6/setup.py
```

### Comparing `jao-py-0.4.5/LICENSE.MD` & `jao_py-0.4.6/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `jao-py-0.4.5/PKG-INFO` & `jao_py-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jao-py
-Version: 0.4.5
+Version: 0.4.6
 Summary: A python API wrapper for JAO.eu
 Home-page: https://github.com/fboerman/jao-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: JAO data api energy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jao-py-0.4.5/README.md` & `jao_py-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `jao-py-0.4.5/jao/CWE/jao.py` & `jao_py-0.4.6/jao/CWE/jao.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.4.5/jao/CWE/parsers.py` & `jao_py-0.4.6/jao/CWE/parsers.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.4.5/jao/jao.py` & `jao_py-0.4.6/jao/jao.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import itertools
 from .exceptions import NoMatchingDataError
 from .parsers import parse_final_domain, parse_base_output
 from typing import List, Dict
 from .util import to_snake_case
 
 __title__ = "jao-py"
-__version__ = "0.4.5"
+__version__ = "0.4.6"
 __author__ = "Frank Boerman"
 __license__ = "MIT"
 
 
 class JaoPublicationToolClient:
     BASEURL = "https://publicationtool.jao.eu/core/api/data/"
 
@@ -222,7 +222,52 @@
         )
 
     def query_scheduled_exchange(self, d_from: pd.Timestamp, d_to: pd.Timestamp) -> (
             pd.DataFrame):
         return parse_base_output(
             super().query_scheduled_exchange(d_from=d_from, d_to=d_to)
         )
+
+
+class JaoPublicationToolPandasIntraDay(JaoPublicationToolPandasClient):
+    BASEURL = "https://publicationtool.jao.eu/coreID/api/data/ID2_"
+
+    def query_lta(self, d_from: pd.Timestamp, d_to: pd.Timestamp):
+        raise NotImplementedError
+
+    def query_status(self, d_from: pd.Timestamp, d_to: pd.Timestamp):
+        raise NotImplementedError
+
+    def query_active_constraints(self, day: pd.Timestamp):
+        raise NotImplementedError
+
+    def query_sidc_atc_raw(self, day: pd.Timestamp) -> List[Dict]:
+        return self._query_base_day(day, 'intradayAtc')
+
+    def query_sidc_ntc_raw(self, day: pd.Timestamp) -> List[Dict]:
+        return self._query_base_day(day, 'intradayNtc')
+
+    def query_sidc_atc(self, day: pd.Timestamp, from_zone: str = None, to_zone: str = None) -> pd.DataFrame:
+        df = parse_base_output(
+            self.query_sidc_atc_raw(day=day)
+        ).rename(columns=lambda x: x.lstrip('border_').replace('_', '>'))
+
+        if from_zone is not None:
+            df = df[[c for c in df.columns if c.split('>')[0] == from_zone]]
+
+        if to_zone is not None:
+            df = df[[c for c in df.columns if c.split('>')[1] == to_zone]]
+
+        return df
+
+    def query_sidc_ntc(self, day: pd.Timestamp, from_zone: str = None, to_zone: str = None) -> pd.DataFrame:
+        df = parse_base_output(
+            self.query_sidc_ntc_raw(day=day)
+        ).rename(columns=lambda x: x.lstrip('border_').replace('_', '>'))
+
+        if from_zone is not None:
+            df = df[[c for c in df.columns if c.split('>')[0] == from_zone]]
+
+        if to_zone is not None:
+            df = df[[c for c in df.columns if c.split('>')[1] == to_zone]]
+
+        return df
```

### Comparing `jao-py-0.4.5/jao/parsers.py` & `jao_py-0.4.6/jao/parsers.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.4.5/jao/webservice.py` & `jao_py-0.4.6/jao/webservice.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.4.5/jao_py.egg-info/PKG-INFO` & `jao_py-0.4.6/jao_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jao-py
-Version: 0.4.5
+Version: 0.4.6
 Summary: A python API wrapper for JAO.eu
 Home-page: https://github.com/fboerman/jao-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: JAO data api energy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jao-py-0.4.5/setup.py` & `jao_py-0.4.6/setup.py`

 * *Files identical despite different names*

