# Comparing `tmp/bnb_futures_connector-4.0.1.tar.gz` & `tmp/bnb_futures_connector-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnb_futures_connector-4.0.1.tar", last modified: Mon May 27 02:57:49 2024, max compression
+gzip compressed data, was "bnb_futures_connector-4.1.0.tar", last modified: Tue May 28 06:48:30 2024, max compression
```

## Comparing `bnb_futures_connector-4.0.1.tar` & `bnb_futures_connector-4.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-27 02:57:49.010845 bnb_futures_connector-4.0.1/
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     1059 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/LICENSE.md
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)       31 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/MANIFEST.in
--rw-r--r--   0 hanhvn    (1000) hanhvn    (1000)     9163 2024-05-27 02:57:49.010845 bnb_futures_connector-4.0.1/PKG-INFO
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     8319 2024-05-27 02:53:57.000000 bnb_futures_connector-4.0.1/README.md
-drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-27 02:57:49.007845 bnb_futures_connector-4.0.1/binance/
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/__init__.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)       22 2024-05-27 02:55:10.000000 bnb_futures_connector-4.0.1/binance/__version__.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     6162 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/api.py
-drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-27 02:57:49.008844 bnb_futures_connector-4.0.1/binance/cm_futures/
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     3602 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/cm_futures/__init__.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)    28001 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/cm_futures/account.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     1321 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/cm_futures/data_stream.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)    20057 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/cm_futures/market.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)      477 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/cm_futures/portfolio_margin.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     1368 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/error.py
-drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-27 02:57:49.008844 bnb_futures_connector-4.0.1/binance/lib/
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/lib/__init__.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)      569 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/lib/authentication.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     2017 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/lib/utils.py
-drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-27 02:57:49.009845 bnb_futures_connector-4.0.1/binance/um_futures/
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     3972 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/um_futures/__init__.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)    31565 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/um_futures/account.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     1324 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/um_futures/data_stream.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)    18300 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/um_futures/market.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)      465 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/um_futures/portfolio_margin.py
-drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-27 02:57:49.009845 bnb_futures_connector-4.0.1/binance/websocket/
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/websocket/__init__.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     3383 2024-05-26 01:57:57.000000 bnb_futures_connector-4.0.1/binance/websocket/binance_socket_manager.py
-drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-27 02:57:49.009845 bnb_futures_connector-4.0.1/binance/websocket/cm_futures/
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/websocket/cm_futures/__init__.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)    11494 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/websocket/cm_futures/websocket_client.py
-drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-27 02:57:49.009845 bnb_futures_connector-4.0.1/binance/websocket/um_futures/
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/websocket/um_futures/__init__.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     9324 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/websocket/um_futures/websocket_client.py
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     3328 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/binance/websocket/websocket_client.py
-drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-27 02:57:49.010845 bnb_futures_connector-4.0.1/bnb_futures_connector.egg-info/
--rw-r--r--   0 hanhvn    (1000) hanhvn    (1000)     9163 2024-05-27 02:57:48.000000 bnb_futures_connector-4.0.1/bnb_futures_connector.egg-info/PKG-INFO
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     1067 2024-05-27 02:57:49.000000 bnb_futures_connector-4.0.1/bnb_futures_connector.egg-info/SOURCES.txt
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        1 2024-05-27 02:57:48.000000 bnb_futures_connector-4.0.1/bnb_futures_connector.egg-info/dependency_links.txt
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)       62 2024-05-27 02:57:48.000000 bnb_futures_connector-4.0.1/bnb_futures_connector.egg-info/requires.txt
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        8 2024-05-27 02:57:48.000000 bnb_futures_connector-4.0.1/bnb_futures_connector.egg-info/top_level.txt
-drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-27 02:57:49.010845 bnb_futures_connector-4.0.1/requirements/
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)       61 2024-05-26 01:52:17.000000 bnb_futures_connector-4.0.1/requirements/common.txt
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)      207 2024-05-27 02:57:49.011845 bnb_futures_connector-4.0.1/setup.cfg
--rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     1518 2024-05-27 02:46:44.000000 bnb_futures_connector-4.0.1/setup.py
+drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-28 06:48:30.829730 bnb_futures_connector-4.1.0/
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     1059 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/LICENSE.md
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)       31 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/MANIFEST.in
+-rw-r--r--   0 hanhvn    (1000) hanhvn    (1000)     9237 2024-05-28 06:48:30.829730 bnb_futures_connector-4.1.0/PKG-INFO
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     8393 2024-05-28 06:48:29.000000 bnb_futures_connector-4.1.0/README.md
+drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-28 06:48:30.825730 bnb_futures_connector-4.1.0/binance/
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/__init__.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)       22 2024-05-28 00:41:40.000000 bnb_futures_connector-4.1.0/binance/__version__.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     6162 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/api.py
+drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-28 06:48:30.825730 bnb_futures_connector-4.1.0/binance/cm_futures/
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     3602 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/cm_futures/__init__.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)    28001 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/cm_futures/account.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     1321 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/cm_futures/data_stream.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)    20057 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/cm_futures/market.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)      477 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/cm_futures/portfolio_margin.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     1368 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/error.py
+drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-28 06:48:30.826730 bnb_futures_connector-4.1.0/binance/lib/
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/lib/__init__.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)      569 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/lib/authentication.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     2017 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/lib/utils.py
+drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-28 06:48:30.827730 bnb_futures_connector-4.1.0/binance/um_futures/
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     3972 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/um_futures/__init__.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)    31565 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/um_futures/account.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     1324 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/um_futures/data_stream.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)    18300 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/um_futures/market.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)      465 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/um_futures/portfolio_margin.py
+drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-28 06:48:30.827730 bnb_futures_connector-4.1.0/binance/websocket/
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/websocket/__init__.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     3383 2024-05-26 01:57:57.000000 bnb_futures_connector-4.1.0/binance/websocket/binance_socket_manager.py
+drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-28 06:48:30.827730 bnb_futures_connector-4.1.0/binance/websocket/cm_futures/
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/websocket/cm_futures/__init__.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)    11494 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/websocket/cm_futures/websocket_client.py
+drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-28 06:48:30.828730 bnb_futures_connector-4.1.0/binance/websocket/um_futures/
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/websocket/um_futures/__init__.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     9911 2024-05-28 06:45:24.000000 bnb_futures_connector-4.1.0/binance/websocket/um_futures/websocket_client.py
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     3328 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/binance/websocket/websocket_client.py
+drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-28 06:48:30.829730 bnb_futures_connector-4.1.0/bnb_futures_connector.egg-info/
+-rw-r--r--   0 hanhvn    (1000) hanhvn    (1000)     9237 2024-05-28 06:48:30.000000 bnb_futures_connector-4.1.0/bnb_futures_connector.egg-info/PKG-INFO
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     1067 2024-05-28 06:48:30.000000 bnb_futures_connector-4.1.0/bnb_futures_connector.egg-info/SOURCES.txt
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        1 2024-05-28 06:48:30.000000 bnb_futures_connector-4.1.0/bnb_futures_connector.egg-info/dependency_links.txt
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)       62 2024-05-28 06:48:30.000000 bnb_futures_connector-4.1.0/bnb_futures_connector.egg-info/requires.txt
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)        8 2024-05-28 06:48:30.000000 bnb_futures_connector-4.1.0/bnb_futures_connector.egg-info/top_level.txt
+drwxrwxr-x   0 hanhvn    (1000) hanhvn    (1000)        0 2024-05-28 06:48:30.828730 bnb_futures_connector-4.1.0/requirements/
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)       61 2024-05-26 01:52:17.000000 bnb_futures_connector-4.1.0/requirements/common.txt
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)      207 2024-05-28 06:48:30.829730 bnb_futures_connector-4.1.0/setup.cfg
+-rw-rw-r--   0 hanhvn    (1000) hanhvn    (1000)     1518 2024-05-27 02:46:44.000000 bnb_futures_connector-4.1.0/setup.py
```

### Comparing `bnb_futures_connector-4.0.1/LICENSE.md` & `bnb_futures_connector-4.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/PKG-INFO` & `bnb_futures_connector-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnb-futures-connector
-Version: 4.0.1
+Version: 4.1.0
 Summary: This is a lightweight library that works as a connector to Binance Futures public API.
 Home-page: https://github.com/vonhathanh/binance-futures-connector-python
 License: MIT
 Keywords: Binance futures,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,21 @@
 - Response metadata can be displayed
 
 ## Installation
 
 ```bash
 pip install bnb-futures-connector
 ```
-
+## Build
+```bash
+python setup.py sdist
+```
+```bash
+twine upload dist/*
+```
 
 ## RESTful APIs
 
 Usage examples:
 ```python
 
 from binance.cm_futures import CMFutures
```

### Comparing `bnb_futures_connector-4.0.1/README.md` & `bnb_futures_connector-4.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,21 @@
 - Response metadata can be displayed
 
 ## Installation
 
 ```bash
 pip install bnb-futures-connector
 ```
-
+## Build
+```bash
+python setup.py sdist
+```
+```bash
+twine upload dist/*
+```
 
 ## RESTful APIs
 
 Usage examples:
 ```python
 
 from binance.cm_futures import CMFutures
```

### Comparing `bnb_futures_connector-4.0.1/binance/api.py` & `bnb_futures_connector-4.1.0/binance/api.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/cm_futures/__init__.py` & `bnb_futures_connector-4.1.0/binance/cm_futures/__init__.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/cm_futures/account.py` & `bnb_futures_connector-4.1.0/binance/cm_futures/account.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/cm_futures/data_stream.py` & `bnb_futures_connector-4.1.0/binance/cm_futures/data_stream.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/cm_futures/market.py` & `bnb_futures_connector-4.1.0/binance/cm_futures/market.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/error.py` & `bnb_futures_connector-4.1.0/binance/error.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/lib/authentication.py` & `bnb_futures_connector-4.1.0/binance/lib/authentication.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/lib/utils.py` & `bnb_futures_connector-4.1.0/binance/lib/utils.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/um_futures/__init__.py` & `bnb_futures_connector-4.1.0/binance/um_futures/__init__.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/um_futures/account.py` & `bnb_futures_connector-4.1.0/binance/um_futures/account.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/um_futures/data_stream.py` & `bnb_futures_connector-4.1.0/binance/um_futures/data_stream.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/um_futures/market.py` & `bnb_futures_connector-4.1.0/binance/um_futures/market.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/websocket/binance_socket_manager.py` & `bnb_futures_connector-4.1.0/binance/websocket/binance_socket_manager.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/websocket/cm_futures/websocket_client.py` & `bnb_futures_connector-4.1.0/binance/websocket/cm_futures/websocket_client.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/binance/websocket/um_futures/websocket_client.py` & `bnb_futures_connector-4.1.0/binance/websocket/um_futures/websocket_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,31 @@
 
         Update Speed: 3000ms or 1000ms
         """
         stream_name = "{}@markPrice@{}s".format(symbol.lower(), speed)
 
         self.send_message_to_server(stream_name, action=action, id=id)
 
+    def agg_mark_price(self, speed: int = 0, id=None, action=None, **kwargs):
+        """Mark Price Streams
+
+        Mark price and funding rate for all symbols pushed every 3 seconds or every second.
+
+        Stream Name: !markPrice@arr or !markPrice@arr@1s
+
+        https://binance-docs.github.io/apidocs/futures/en/#mark-price-stream-for-all-market
+
+        Update Speed: 3000ms or 1000ms
+        """
+        stream_name = "!markPrice@arr"
+        if speed != 0:
+            stream_name += "@{}s".format(speed)
+
+        self.send_message_to_server(stream_name, action=action, id=id)
+
     def kline(self, symbol: str, interval: str, id=None, action=None, **kwargs):
         """Kline/Candlestick Streams
 
         The Kline/Candlestick Stream push updates to the current klines/candlestick every 250 milliseconds (if existing)
 
         Stream Name: <symbol>@kline_<interval>
```

### Comparing `bnb_futures_connector-4.0.1/binance/websocket/websocket_client.py` & `bnb_futures_connector-4.1.0/binance/websocket/websocket_client.py`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/bnb_futures_connector.egg-info/PKG-INFO` & `bnb_futures_connector-4.1.0/bnb_futures_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnb-futures-connector
-Version: 4.0.1
+Version: 4.1.0
 Summary: This is a lightweight library that works as a connector to Binance Futures public API.
 Home-page: https://github.com/vonhathanh/binance-futures-connector-python
 License: MIT
 Keywords: Binance futures,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,21 @@
 - Response metadata can be displayed
 
 ## Installation
 
 ```bash
 pip install bnb-futures-connector
 ```
-
+## Build
+```bash
+python setup.py sdist
+```
+```bash
+twine upload dist/*
+```
 
 ## RESTful APIs
 
 Usage examples:
 ```python
 
 from binance.cm_futures import CMFutures
```

### Comparing `bnb_futures_connector-4.0.1/bnb_futures_connector.egg-info/SOURCES.txt` & `bnb_futures_connector-4.1.0/bnb_futures_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnb_futures_connector-4.0.1/setup.py` & `bnb_futures_connector-4.1.0/setup.py`

 * *Files identical despite different names*

