# Comparing `tmp/bitopro-client-1.0.5.tar.gz` & `tmp/bitopro-client-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitopro-client-1.0.5.tar", last modified: Tue May 21 15:17:11 2024, max compression
+gzip compressed data, was "bitopro-client-1.0.6.tar", last modified: Tue May 28 13:20:08 2024, max compression
```

## Comparing `bitopro-client-1.0.5.tar` & `bitopro-client-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 15:17:11.437508 bitopro-client-1.0.5/
--rw-rw-rw-   0        0        0     1084 2023-12-17 12:09:19.000000 bitopro-client-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      454 2024-05-21 15:17:11.436512 bitopro-client-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    13274 2023-12-19 07:01:25.000000 bitopro-client-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 15:17:11.425715 bitopro-client-1.0.5/bitoproClient/
--rw-rw-rw-   0        0        0     2316 2023-12-18 13:54:10.000000 bitopro-client-1.0.5/bitoproClient/bitopro_indicator.py
--rw-rw-rw-   0        0        0    21319 2024-05-21 14:51:47.000000 bitopro-client-1.0.5/bitoproClient/bitopro_restful_client.py
--rw-rw-rw-   0        0        0      660 2023-12-17 12:10:21.000000 bitopro-client-1.0.5/bitoproClient/bitopro_util.py
--rw-rw-rw-   0        0        0     4575 2023-12-17 12:13:30.000000 bitopro-client-1.0.5/bitoproClient/bitopro_websocket_client.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:17:11.434561 bitopro-client-1.0.5/bitopro_client.egg-info/
--rw-rw-rw-   0        0        0      454 2024-05-21 15:17:11.000000 bitopro-client-1.0.5/bitopro_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-05-21 15:17:11.000000 bitopro-client-1.0.5/bitopro_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 15:17:11.000000 bitopro-client-1.0.5/bitopro_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-21 15:17:11.000000 bitopro-client-1.0.5/bitopro_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 15:17:11.437508 bitopro-client-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      548 2024-05-21 15:09:25.000000 bitopro-client-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:20:08.844211 bitopro-client-1.0.6/
+-rw-rw-rw-   0        0        0     1084 2023-12-17 12:09:19.000000 bitopro-client-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      454 2024-05-28 13:20:08.843234 bitopro-client-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    13274 2023-12-19 07:01:25.000000 bitopro-client-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 13:20:08.833241 bitopro-client-1.0.6/bitoproClient/
+-rw-rw-rw-   0        0        0     2316 2023-12-18 13:54:10.000000 bitopro-client-1.0.6/bitoproClient/bitopro_indicator.py
+-rw-rw-rw-   0        0        0    21319 2024-05-28 13:05:50.000000 bitopro-client-1.0.6/bitoproClient/bitopro_restful_client.py
+-rw-rw-rw-   0        0        0      660 2023-12-17 12:10:21.000000 bitopro-client-1.0.6/bitoproClient/bitopro_util.py
+-rw-rw-rw-   0        0        0     4596 2024-05-28 13:18:14.000000 bitopro-client-1.0.6/bitoproClient/bitopro_websocket_client.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:20:08.841252 bitopro-client-1.0.6/bitopro_client.egg-info/
+-rw-rw-rw-   0        0        0      454 2024-05-28 13:20:08.000000 bitopro-client-1.0.6/bitopro_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-05-28 13:20:08.000000 bitopro-client-1.0.6/bitopro_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 13:20:08.000000 bitopro-client-1.0.6/bitopro_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-28 13:20:08.000000 bitopro-client-1.0.6/bitopro_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 13:20:08.845211 bitopro-client-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      548 2024-05-28 13:16:21.000000 bitopro-client-1.0.6/setup.py
```

### Comparing `bitopro-client-1.0.5/LICENSE` & `bitopro-client-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bitopro-client-1.0.5/README.md` & `bitopro-client-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bitopro-client-1.0.5/bitoproClient/bitopro_indicator.py` & `bitopro-client-1.0.6/bitoproClient/bitopro_indicator.py`

 * *Files identical despite different names*

### Comparing `bitopro-client-1.0.5/bitoproClient/bitopro_restful_client.py` & `bitopro-client-1.0.6/bitoproClient/bitopro_restful_client.py`

 * *Files identical despite different names*

### Comparing `bitopro-client-1.0.5/bitoproClient/bitopro_util.py` & `bitopro-client-1.0.6/bitoproClient/bitopro_util.py`

 * *Files identical despite different names*

### Comparing `bitopro-client-1.0.5/bitoproClient/bitopro_websocket_client.py` & `bitopro-client-1.0.6/bitoproClient/bitopro_websocket_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.callback = callback 
 
         self._ws: websocket.WebSocketApp = None
         self.wst: threading.Thread = None
         
     def init_websocket(self):
         if self._account and self._api_key and self._api_secret:
-            params = {"identity": self._account, "nonce": ""}
+            params = {"identity": self._account, "nonce": get_current_timestamp()}
             ws_headers = build_headers(self._api_key, self._api_secret, params=params)
         else:
             ws_headers = None
 
         self._ws = websocket.WebSocketApp(
             self._connect_endpoint,
             on_message=lambda ws, msg:self._on_message(ws, msg),
```

### Comparing `bitopro-client-1.0.5/setup.py` & `bitopro-client-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import pathlib
 from setuptools import setup, find_packages
  
 HERE = pathlib.Path(__file__).parent.resolve()
 
 setup(name='bitopro-client',
-    version='1.0.5',
+    version='1.0.6',
     description='For BitoPro crypto currency exchange written in Python',
     url='https://github.com/bitoex/bitopro-api-python.git',
     author='Bitoex',
     author_email='support@bitopro.com',
     license='MIT',
     packages=['bitoproClient'],
     python_requires = ">=3.9",
```

