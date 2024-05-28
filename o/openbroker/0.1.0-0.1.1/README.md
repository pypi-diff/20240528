# Comparing `tmp/openbroker-0.1.0.tar.gz` & `tmp/openbroker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbroker-0.1.0.tar", max compression
+gzip compressed data, was "openbroker-0.1.1.tar", max compression
```

## Comparing `openbroker-0.1.0.tar` & `openbroker-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1081 2024-05-27 05:55:26.432212 openbroker-0.1.0/LICENSE
--rw-r--r--   0        0        0      881 2024-05-27 05:55:26.433031 openbroker-0.1.0/README.md
--rw-r--r--   0        0        0      142 2024-05-27 05:55:26.436556 openbroker-0.1.0/openbroker/__init__.py
--rw-r--r--   0        0        0      142 2024-05-27 05:55:26.437006 openbroker-0.1.0/openbroker/api/__init__.py
--rw-r--r--   0        0        0     1149 2024-05-27 05:55:26.437268 openbroker-0.1.0/openbroker/api/base.py
--rw-r--r--   0        0        0      352 2024-05-27 05:55:26.437563 openbroker-0.1.0/openbroker/api/instruments.py
--rw-r--r--   0        0        0     1541 2024-05-27 05:55:26.438039 openbroker-0.1.0/openbroker/api/orders.py
--rw-r--r--   0        0        0      444 2024-05-27 05:55:26.438269 openbroker-0.1.0/openbroker/api/user.py
--rw-r--r--   0        0        0     2487 2024-05-27 05:55:26.438535 openbroker-0.1.0/openbroker/api/ws.py
--rw-r--r--   0        0        0     4223 2024-05-27 05:55:26.438838 openbroker-0.1.0/openbroker/broker.py
--rw-r--r--   0        0        0     3152 2024-05-27 05:55:26.439041 openbroker-0.1.0/openbroker/broker_login.py
--rw-r--r--   0        0        0     3542 2024-05-27 05:55:26.439359 openbroker-0.1.0/openbroker/client.py
--rw-r--r--   0        0        0      524 2024-05-28 06:47:54.083425 openbroker-0.1.0/openbroker/config.py
--rw-r--r--   0        0        0      128 2024-05-27 05:55:26.439881 openbroker-0.1.0/openbroker/constant/__init__.py
--rw-r--r--   0        0        0      934 2024-05-27 05:55:26.440111 openbroker-0.1.0/openbroker/constant/broker.py
--rw-r--r--   0        0        0      330 2024-05-27 05:55:26.440327 openbroker-0.1.0/openbroker/constant/instrument.py
--rw-r--r--   0        0        0      921 2024-05-27 05:55:26.440557 openbroker-0.1.0/openbroker/constant/order.py
--rw-r--r--   0        0        0      244 2024-05-27 05:55:26.440782 openbroker-0.1.0/openbroker/datatype/__init__.py
--rw-r--r--   0        0        0     2552 2024-05-27 05:55:26.441007 openbroker-0.1.0/openbroker/datatype/instrument.py
--rw-r--r--   0        0        0     5426 2024-05-27 05:55:26.441302 openbroker-0.1.0/openbroker/datatype/order.py
--rw-r--r--   0        0        0       61 2024-05-27 05:55:26.441495 openbroker-0.1.0/openbroker/entity/__init__.py
--rw-r--r--   0        0        0     1548 2024-05-27 05:55:26.441692 openbroker-0.1.0/openbroker/entity/broker.py
--rw-r--r--   0        0        0     2724 2024-05-27 05:55:26.441891 openbroker-0.1.0/openbroker/entity/order.py
--rw-r--r--   0        0        0      101 2024-05-27 05:55:26.442058 openbroker-0.1.0/openbroker/exceptions.py
--rw-r--r--   0        0        0     7907 2024-05-27 05:55:26.442323 openbroker-0.1.0/openbroker/instrument.py
--rw-r--r--   0        0        0     7072 2024-05-27 05:55:26.442681 openbroker-0.1.0/openbroker/order.py
--rw-r--r--   0        0        0     1480 2024-05-27 05:55:26.442869 openbroker-0.1.0/openbroker/session.py
--rw-r--r--   0        0        0      222 2024-05-27 05:55:26.443102 openbroker-0.1.0/openbroker/utils.py
--rw-r--r--   0        0        0      528 2024-05-27 05:55:26.443783 openbroker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 openbroker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-05-27 05:55:26.432212 openbroker-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1023 2024-05-28 07:16:18.720351 openbroker-0.1.1/README.md
+-rw-r--r--   0        0        0      142 2024-05-27 05:55:26.436556 openbroker-0.1.1/openbroker/__init__.py
+-rw-r--r--   0        0        0      142 2024-05-27 05:55:26.437006 openbroker-0.1.1/openbroker/api/__init__.py
+-rw-r--r--   0        0        0     1149 2024-05-27 05:55:26.437268 openbroker-0.1.1/openbroker/api/base.py
+-rw-r--r--   0        0        0      352 2024-05-27 05:55:26.437563 openbroker-0.1.1/openbroker/api/instruments.py
+-rw-r--r--   0        0        0     1541 2024-05-27 05:55:26.438039 openbroker-0.1.1/openbroker/api/orders.py
+-rw-r--r--   0        0        0      444 2024-05-27 05:55:26.438269 openbroker-0.1.1/openbroker/api/user.py
+-rw-r--r--   0        0        0     2487 2024-05-27 05:55:26.438535 openbroker-0.1.1/openbroker/api/ws.py
+-rw-r--r--   0        0        0     4223 2024-05-27 05:55:26.438838 openbroker-0.1.1/openbroker/broker.py
+-rw-r--r--   0        0        0     3152 2024-05-27 05:55:26.439041 openbroker-0.1.1/openbroker/broker_login.py
+-rw-r--r--   0        0        0     3542 2024-05-27 05:55:26.439359 openbroker-0.1.1/openbroker/client.py
+-rw-r--r--   0        0        0      524 2024-05-28 06:47:54.083425 openbroker-0.1.1/openbroker/config.py
+-rw-r--r--   0        0        0      128 2024-05-27 05:55:26.439881 openbroker-0.1.1/openbroker/constant/__init__.py
+-rw-r--r--   0        0        0      934 2024-05-27 05:55:26.440111 openbroker-0.1.1/openbroker/constant/broker.py
+-rw-r--r--   0        0        0      330 2024-05-27 05:55:26.440327 openbroker-0.1.1/openbroker/constant/instrument.py
+-rw-r--r--   0        0        0      921 2024-05-27 05:55:26.440557 openbroker-0.1.1/openbroker/constant/order.py
+-rw-r--r--   0        0        0      244 2024-05-27 05:55:26.440782 openbroker-0.1.1/openbroker/datatype/__init__.py
+-rw-r--r--   0        0        0     2552 2024-05-27 05:55:26.441007 openbroker-0.1.1/openbroker/datatype/instrument.py
+-rw-r--r--   0        0        0     5426 2024-05-27 05:55:26.441302 openbroker-0.1.1/openbroker/datatype/order.py
+-rw-r--r--   0        0        0       61 2024-05-27 05:55:26.441495 openbroker-0.1.1/openbroker/entity/__init__.py
+-rw-r--r--   0        0        0     1548 2024-05-27 05:55:26.441692 openbroker-0.1.1/openbroker/entity/broker.py
+-rw-r--r--   0        0        0     2724 2024-05-27 05:55:26.441891 openbroker-0.1.1/openbroker/entity/order.py
+-rw-r--r--   0        0        0      101 2024-05-27 05:55:26.442058 openbroker-0.1.1/openbroker/exceptions.py
+-rw-r--r--   0        0        0     7907 2024-05-27 05:55:26.442323 openbroker-0.1.1/openbroker/instrument.py
+-rw-r--r--   0        0        0     7072 2024-05-27 05:55:26.442681 openbroker-0.1.1/openbroker/order.py
+-rw-r--r--   0        0        0     1480 2024-05-27 05:55:26.442869 openbroker-0.1.1/openbroker/session.py
+-rw-r--r--   0        0        0      222 2024-05-27 05:55:26.443102 openbroker-0.1.1/openbroker/utils.py
+-rw-r--r--   0        0        0      528 2024-05-28 07:20:14.995623 openbroker-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 openbroker-0.1.1/PKG-INFO
```

### Comparing `openbroker-0.1.0/LICENSE` & `openbroker-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/api/base.py` & `openbroker-0.1.1/openbroker/api/base.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/api/orders.py` & `openbroker-0.1.1/openbroker/api/orders.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/api/ws.py` & `openbroker-0.1.1/openbroker/api/ws.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/broker.py` & `openbroker-0.1.1/openbroker/broker.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/broker_login.py` & `openbroker-0.1.1/openbroker/broker_login.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/client.py` & `openbroker-0.1.1/openbroker/client.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/config.py` & `openbroker-0.1.1/openbroker/config.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/constant/broker.py` & `openbroker-0.1.1/openbroker/constant/broker.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/constant/order.py` & `openbroker-0.1.1/openbroker/constant/order.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/datatype/instrument.py` & `openbroker-0.1.1/openbroker/datatype/instrument.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/datatype/order.py` & `openbroker-0.1.1/openbroker/datatype/order.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/entity/broker.py` & `openbroker-0.1.1/openbroker/entity/broker.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/entity/order.py` & `openbroker-0.1.1/openbroker/entity/order.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/instrument.py` & `openbroker-0.1.1/openbroker/instrument.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/order.py` & `openbroker-0.1.1/openbroker/order.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/openbroker/session.py` & `openbroker-0.1.1/openbroker/session.py`

 * *Files identical despite different names*

### Comparing `openbroker-0.1.0/pyproject.toml` & `openbroker-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openbroker"
-version = "0.1.0"
+version = "0.1.1"
 description = "The first unified API for algo-trading on Indian markets - by AlgoTest"
 authors = ["rajat499", "BalzySte"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `openbroker-0.1.0/PKG-INFO` & `openbroker-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbroker
-Version: 0.1.0
+Version: 0.1.1
 Summary: The first unified API for algo-trading on Indian markets - by AlgoTest
 License: MIT
 Author: rajat499
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -28,25 +28,25 @@
 
 ```bash
 pip install openbroker
 ```
 
 ## Usage
 
-The library is designed to be as simple as possible to use. Take a look at the [examples](./examples/).
+The library is designed to be as simple as possible to use. Take a look at the [examples](https://github.com/Algo-Test/openbroker/tree/main/examples).
 
 ## Documentation
 
-The documentation for the library can be found [here](https://openbroker.readthedocs.io/en/latest/).
+The documentation for the library can be found [here](https://algo-test.github.io/openbroker/).
 
 ## Contributing
 
-Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for more information.
+Contributions are welcome! Please read [CONTRIBUTING.md](https://github.com/Algo-Test/openbroker/blob/main/CONTRIBUTING.md) for more information.
 
 ## License
 
-This project is licensed under the terms of the [MIT License](LICENSE).
+This project is licensed under the terms of the [MIT License](https://github.com/Algo-Test/openbroker/blob/main/LICENSE).
 
 ## Disclaimer
 
 This project is not affiliated with AlgoTest in any way.
```

