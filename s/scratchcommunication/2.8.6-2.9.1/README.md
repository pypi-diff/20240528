# Comparing `tmp/scratchcommunication-2.8.6.tar.gz` & `tmp/scratchcommunication-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.8.6.tar", last modified: Thu May 23 13:39:57 2024, max compression
+gzip compressed data, was "scratchcommunication-2.9.1.tar", last modified: Tue May 28 17:57:42 2024, max compression
```

## Comparing `scratchcommunication-2.8.6.tar` & `scratchcommunication-2.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:57.065498 scratchcommunication-2.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-23 13:39:57.065498 scratchcommunication-2.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:57.065498 scratchcommunication-2.8.6/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18236 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:57.065498 scratchcommunication-2.8.6/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:57.065498 scratchcommunication-2.8.6/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-23 13:39:57.000000 scratchcommunication-2.8.6/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-23 13:39:57.000000 scratchcommunication-2.8.6/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:39:57.000000 scratchcommunication-2.8.6/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 13:39:57.000000 scratchcommunication-2.8.6/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 13:39:57.000000 scratchcommunication-2.8.6/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:39:57.065498 scratchcommunication-2.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:57.065498 scratchcommunication-2.8.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-23 13:39:53.000000 scratchcommunication-2.8.6/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:57:42.767543 scratchcommunication-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-28 17:57:42.767543 scratchcommunication-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:57:42.763543 scratchcommunication-2.9.1/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18302 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:57:42.767543 scratchcommunication-2.9.1/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:57:42.767543 scratchcommunication-2.9.1/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-28 17:57:42.000000 scratchcommunication-2.9.1/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 17:57:42.000000 scratchcommunication-2.9.1/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:57:42.000000 scratchcommunication-2.9.1/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-28 17:57:42.000000 scratchcommunication-2.9.1/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 17:57:42.000000 scratchcommunication-2.9.1/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:57:42.767543 scratchcommunication-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:57:42.767543 scratchcommunication-2.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/tests/test1.py
```

### Comparing `scratchcommunication-2.8.6/LICENSE` & `scratchcommunication-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.6/PKG-INFO` & `scratchcommunication-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.8.6
+Version: 2.9.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.8.6/README.md` & `scratchcommunication-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.6/scratchcommunication/cloud.py` & `scratchcommunication-2.9.1/scratchcommunication/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal, Union, Any, Protocol
 from collections.abc import Callable
 from .exceptions import QuickAccessDisabledError, NotSupported, ErrorInEventHandler, StopException, EventExpiredError
 import scratchcommunication
+from func_timeout import StoppableThread
 import json, time, requests, warnings, traceback, secrets, sys
 from websocket import WebSocket
-from func_timeout import StoppableThread
 
 NoneType = type(None)
 CloudConnection = None
 
 class EventDispatcher(Protocol):
     def __call__(self, data : dict, **entries) -> None:
         pass
@@ -75,15 +75,15 @@
     reconnect : bool
     values : dict
     events : dict
     cloud_host : str
     accept_strs : bool
     wait_until : Union[float, int]
     receive_from_websocket : bool
-    data_reception : Any
+    data_reception : Union[StoppableThread, None]
     event_order : dict[Union[float, int, bool], dict[Event, int]]
     processed_events : list[Event]
     keep_all_events : bool
     supports_cloud_logs : bool
     def __init__(
         self,
         *,
@@ -136,15 +136,16 @@
         self.stop_thread()
 
     def stop_thread(self):
         """
         Use for stopping the underlying thread.
         """
         self.thread_running = False
-        self.data_reception.stop(StopException)
+        self.data_reception.stop(StopException, 0.1)
+        self.data_reception.join()
 
     def enable_quickaccess(self):
         """
         Use for enabling the use of the object as a lookup table.
         """
         self.quickaccess = True
```

### Comparing `scratchcommunication-2.8.6/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.9.1/scratchcommunication/cloud_socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .cloud import CloudConnection
 from . import security as sec
-from threading import Lock
+from threading import Lock, Condition
 from typing import Union, Any, Self
 import random, time
 from itertools import islice
 from .exceptions import NotSupported
 
 alphabet = "abcdefghijklmnopqrstuvwxyz"
 special_characters = " .,-:;_'#!\"§$%&/()=?{[]}\\0123456789<>ß*"
@@ -78,14 +78,17 @@
     clients : dict
     new_clients : list
     connecting_clients : list
     key_parts : dict
     last_timestamp : float
     packet_size : int
     accepting : Lock
+    accepted : Condition
+    received_any : Condition
+    any_update : Condition
     def __init__(self, *, cloud : CloudConnection, packet_size : int = 220, security : Union[None, tuple] = None):
         raise NotImplementedError
 
     def __enter__(self) -> Self:
         raise NotImplementedError
     
     def __exit__(self, exc_type, exc_value, traceback):
@@ -120,14 +123,15 @@
     username : str
     security : str
     encrypter : sec.SymmetricEncryption
     secure : bool
     new_msgs : list
     current_msg : BaseCloudSocketMSG
     receiving : Lock
+    received : Condition
     sending : Lock
     def __init__(self, *, cloud_socket : BaseCloudSocket, client_id : str, username : str = None, security : str = None):
         raise NotImplementedError
     
     def __enter__(self) -> Self:
         raise NotImplementedError
     
@@ -156,14 +160,17 @@
         self.clients = {}
         self.new_clients = []
         self.connecting_clients = []
         self.key_parts = {}
         self.last_timestamp = time.time()
         self.packet_size = packet_size
         self.accepting = Lock()
+        self.accepted = Condition()
+        self.received_any = Condition()
+        self.any_update = Condition()
         
     def listen(self):
         """
         Start the cloud socket.
         """
         @self.cloud.on("set")
         def on_packet(event):
@@ -203,14 +210,15 @@
                     salt = int(msg_data[-15:]) / 100
                     assert salt > self.last_timestamp, "Invalid salt(too little)"
                     assert salt < time.time() + 30, "Invalid salt(too big)"
                     self.last_timestamp = salt
                     self.clients[client].current_msg.add(" "+self.clients[client].encrypter.decrypt(self._decode(msg_data[1:-15]), msg_data[-15:]))
                     assert not "-" in event.value
                     self.clients[client].current_msg.finalize(decode=False)
+                    self.clients[client]._new_msg()
                     self.clients[client].new_msgs.append(self.clients[client].current_msg)
                     self.clients[client].current_msg = CloudSocketMSG()
                     return
                 
                 # New secure user
                 
                 key = None
@@ -231,14 +239,16 @@
                 try:
                     client_username = event.user
                 except NotSupported:
                     client_username = None
                 client_obj = CloudSocketConnection(cloud_socket=self, client_id=client, username=client_username, security=key)
                 self.clients[client] = client_obj
                 self.new_clients.append((client_obj, client_username))
+                self.accepted.notify_all()
+                self.any_update.notify_all()
                 return
             except AssertionError:
                 pass
             
     def stop(self):
         self.cloud.stop_thread()
 
@@ -279,15 +289,15 @@
         """
         endtime = (time.time() + timeout) if timeout is not None else None
         result = self.accepting.acquire(timeout=timeout if timeout is not None else -1)
         if not result:
             raise TimeoutError("The timeout expired (consider setting timeout=None)")
         try:
             while (not self.new_clients) and (timeout is None or time.time() < endtime): 
-                pass
+                self.accepted.wait(timeout and endtime - time.time())
             try:
                 new_client = self.new_clients.pop(0)
                 return new_client
             except IndexError:
                 raise TimeoutError("The timeout expired (consider setting timeout=None)")
         finally:
             self.accepting.release()
@@ -303,14 +313,15 @@
         self.security = security
         self.encrypter = sec.SymmetricEncryption(self.security)
         self.secure = bool(self.security)
         self.new_msgs = []
         self.current_msg = CloudSocketMSG()
         self.receiving = Lock()
         self.sending = Lock()
+        self.received = Condition()
 
     def __enter__(self):
         return self
     
     def __exit__(self, exc_type, exc_value, traceback):
         pass
     
@@ -352,21 +363,29 @@
         """
         endtime = (time.time() + timeout) if timeout is not None else None
         result = self.receiving.acquire(timeout=timeout if timeout is not None else -1)
         if not result:
             raise TimeoutError("The timeout expired (consider setting timeout=None)")
         try:
             while (not self.new_msgs) and (timeout is None or time.time() < endtime):
-                pass
+                self.received.wait(timeout and endtime - time.time())
             try:
                 return self.new_msgs.pop(0).message
             except IndexError:
                 raise TimeoutError("The timeout expired (consider setting timeout=None)")
         finally:
             self.receiving.release()
+            
+    def _new_msg(self):
+        """
+        Don't use.
+        """
+        self.received.notify_all()
+        self.cloud_socket.received_any.notify_all()
+        self.cloud_socket.any_update.notify_all()
     
 class CloudSocketMSG(BaseCloudSocketMSG):
     """
     Class for cloud socket messages.
     """
     def __init__(self, message : str = "", complete : bool = False):
         self.message = message
```

### Comparing `scratchcommunication-2.8.6/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.9.1/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.6/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.9.1/scratchcommunication/cloudrequests/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             self.uses_thread = True
             self.thread = StoppableThread(target=lambda : self.start(thread=False), daemon=daemon_thread)
             self.thread.start()
             return
         clients : list[tuple[CloudSocketConnection, str]] = []
         end_time = duration and (time.time() + duration)
         while (not end_time) or time.time() < end_time:
-            time.sleep(0.05)
+            self.cloud_socket.any_update.wait(30)
             try:
                 try:
                     clients.append(self.cloud_socket.accept(timeout=0))
                 except TimeoutError:
                     pass
                 for client, username in clients:
                     try:
```

### Comparing `scratchcommunication-2.8.6/scratchcommunication/security.py` & `scratchcommunication-2.9.1/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.6/scratchcommunication/session.py` & `scratchcommunication-2.9.1/scratchcommunication/session.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.6/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.9.1/scratchcommunication.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.8.6
+Version: 2.9.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.8.6/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.9.1/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.8.6/setup.py` & `scratchcommunication-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '2.8.6'
+VERSION = '2.9.1'
 
 setup(
     name='scratchcommunication',
     version=VERSION,
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
```

### Comparing `scratchcommunication-2.8.6/tests/test1.py` & `scratchcommunication-2.9.1/tests/test1.py`

 * *Files identical despite different names*

