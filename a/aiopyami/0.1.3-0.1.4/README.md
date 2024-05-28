# Comparing `tmp/aiopyami-0.1.3.tar.gz` & `tmp/aiopyami-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopyami-0.1.3.tar", last modified: Tue Sep 26 07:33:49 2023, max compression
+gzip compressed data, was "aiopyami-0.1.4.tar", last modified: Tue May 28 06:34:53 2024, max compression
```

## Comparing `aiopyami-0.1.3.tar` & `aiopyami-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 zahiriddinjamoliddinov   (501) staff       (20)        0 2023-09-26 07:33:49.885280 aiopyami-0.1.3/
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)     1066 2023-08-07 09:00:30.000000 aiopyami-0.1.3/LICENSE
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      722 2023-09-26 07:33:49.884949 aiopyami-0.1.3/PKG-INFO
-drwxr-xr-x   0 zahiriddinjamoliddinov   (501) staff       (20)        0 2023-09-26 07:33:49.883562 aiopyami-0.1.3/aiopyami/
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      122 2023-08-10 05:44:12.000000 aiopyami-0.1.3/aiopyami/__init__.py
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)     6496 2023-09-26 06:47:40.000000 aiopyami-0.1.3/aiopyami/ami.py
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)     5170 2023-09-26 06:49:49.000000 aiopyami-0.1.3/aiopyami/client.py
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)     3008 2023-08-10 10:40:14.000000 aiopyami-0.1.3/aiopyami/events.py
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      399 2023-08-10 05:44:12.000000 aiopyami-0.1.3/aiopyami/exceptions.py
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)     2141 2023-08-10 05:44:12.000000 aiopyami-0.1.3/aiopyami/formats.py
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      590 2023-08-10 05:44:12.000000 aiopyami-0.1.3/aiopyami/internal.py
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      371 2023-08-10 05:44:12.000000 aiopyami-0.1.3/aiopyami/utils.py
-drwxr-xr-x   0 zahiriddinjamoliddinov   (501) staff       (20)        0 2023-09-26 07:33:49.884295 aiopyami-0.1.3/aiopyami.egg-info/
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      722 2023-09-26 07:33:49.000000 aiopyami-0.1.3/aiopyami.egg-info/PKG-INFO
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      345 2023-09-26 07:33:49.000000 aiopyami-0.1.3/aiopyami.egg-info/SOURCES.txt
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)        1 2023-09-26 07:33:49.000000 aiopyami-0.1.3/aiopyami.egg-info/dependency_links.txt
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)        9 2023-09-26 07:33:49.000000 aiopyami-0.1.3/aiopyami.egg-info/top_level.txt
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)       38 2023-09-26 07:33:49.885343 aiopyami-0.1.3/setup.cfg
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      806 2023-09-26 07:33:45.000000 aiopyami-0.1.3/setup.py
-drwxr-xr-x   0 zahiriddinjamoliddinov   (501) staff       (20)        0 2023-09-26 07:33:49.884660 aiopyami-0.1.3/test/
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      491 2023-08-10 05:44:12.000000 aiopyami-0.1.3/test/test_actions.py
--rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)     2575 2023-08-10 05:44:12.000000 aiopyami-0.1.3/test/test_async_ami.py
+drwxr-xr-x   0 zahiriddinjamoliddinov   (501) staff       (20)        0 2024-05-28 06:34:53.928182 aiopyami-0.1.4/
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)     1066 2024-05-28 06:29:21.000000 aiopyami-0.1.4/LICENSE
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      722 2024-05-28 06:34:53.927812 aiopyami-0.1.4/PKG-INFO
+drwxr-xr-x   0 zahiriddinjamoliddinov   (501) staff       (20)        0 2024-05-28 06:34:53.925418 aiopyami-0.1.4/aiopyami/
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      122 2024-05-28 06:29:21.000000 aiopyami-0.1.4/aiopyami/__init__.py
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)     6684 2024-05-28 06:30:53.000000 aiopyami-0.1.4/aiopyami/ami.py
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)     5295 2024-05-28 06:31:28.000000 aiopyami-0.1.4/aiopyami/client.py
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)     3008 2024-05-28 06:29:21.000000 aiopyami-0.1.4/aiopyami/events.py
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      399 2024-05-28 06:29:21.000000 aiopyami-0.1.4/aiopyami/exceptions.py
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)     2141 2024-05-28 06:29:21.000000 aiopyami-0.1.4/aiopyami/formats.py
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      590 2024-05-28 06:29:21.000000 aiopyami-0.1.4/aiopyami/internal.py
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      371 2024-05-28 06:29:21.000000 aiopyami-0.1.4/aiopyami/utils.py
+drwxr-xr-x   0 zahiriddinjamoliddinov   (501) staff       (20)        0 2024-05-28 06:34:53.927383 aiopyami-0.1.4/aiopyami.egg-info/
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      722 2024-05-28 06:34:53.000000 aiopyami-0.1.4/aiopyami.egg-info/PKG-INFO
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      345 2024-05-28 06:34:53.000000 aiopyami-0.1.4/aiopyami.egg-info/SOURCES.txt
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)        1 2024-05-28 06:34:53.000000 aiopyami-0.1.4/aiopyami.egg-info/dependency_links.txt
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)        9 2024-05-28 06:34:53.000000 aiopyami-0.1.4/aiopyami.egg-info/top_level.txt
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)       38 2024-05-28 06:34:53.928249 aiopyami-0.1.4/setup.cfg
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      806 2024-05-28 06:32:04.000000 aiopyami-0.1.4/setup.py
+drwxr-xr-x   0 zahiriddinjamoliddinov   (501) staff       (20)        0 2024-05-28 06:34:53.927038 aiopyami-0.1.4/test/
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)      491 2024-05-28 06:29:21.000000 aiopyami-0.1.4/test/test_actions.py
+-rw-r--r--   0 zahiriddinjamoliddinov   (501) staff       (20)     2575 2024-05-28 06:29:21.000000 aiopyami-0.1.4/test/test_async_ami.py
```

### Comparing `aiopyami-0.1.3/LICENSE` & `aiopyami-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopyami-0.1.3/PKG-INFO` & `aiopyami-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopyami
-Version: 0.1.3
+Version: 0.1.4
 Summary: An asynchronous Asterisk AMI Client for Python
 Home-page: https://github.com/Zahgrom34/aiopyami
 Author: Zahcoder34
 Author-email: Zakhriw@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiopyami-0.1.3/aiopyami/ami.py` & `aiopyami-0.1.4/aiopyami/ami.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,20 @@
             event_data = AsteriskResponse.from_response(response)
             self._action_queue.remove(action_id)
             self.__client.queue.put_nowait(event_data)
 
             if not len(self._action_queue):
                 self._actions_queue_event.set()
     
+    def reset_events(self):
+        """
+        Resets the events to make them reusable.
+        """
+        self._actions_queue_event.clear()
+        self._action_callbacks_event.clear()
 
     async def wait_for_actions_complete(self) -> None:
         """
         Waits for all actions to be completed
         If  this function will be called inside coroutine, it will freeze that coroutine, until all actions won't be completed
         """
         await self._actions_queue_event.wait()
```

### Comparing `aiopyami-0.1.3/aiopyami/client.py` & `aiopyami-0.1.4/aiopyami/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,10 +148,13 @@
         if not self.queue.empty():
             # Wait for queue to be empty
             await self.queue.join()
         
         # Here we should add wait_for_actions_complete
         await self.__manager.wait_for_actions_complete()
 
+        # Here we should reset the actions events to wait for them in next connection
+        self.__manager.reset_events()
+
         logoff_cmd = Action("Logoff", {})
         await self.__manager.send_action(logoff_cmd)
         self.transport.close()
```

### Comparing `aiopyami-0.1.3/aiopyami/events.py` & `aiopyami-0.1.4/aiopyami/events.py`

 * *Files identical despite different names*

### Comparing `aiopyami-0.1.3/aiopyami/formats.py` & `aiopyami-0.1.4/aiopyami/formats.py`

 * *Files identical despite different names*

### Comparing `aiopyami-0.1.3/aiopyami/internal.py` & `aiopyami-0.1.4/aiopyami/internal.py`

 * *Files identical despite different names*

### Comparing `aiopyami-0.1.3/aiopyami.egg-info/PKG-INFO` & `aiopyami-0.1.4/aiopyami.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopyami
-Version: 0.1.3
+Version: 0.1.4
 Summary: An asynchronous Asterisk AMI Client for Python
 Home-page: https://github.com/Zahgrom34/aiopyami
 Author: Zahcoder34
 Author-email: Zakhriw@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiopyami-0.1.3/setup.py` & `aiopyami-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aiopyami",
-    version="0.1.3",
+    version="0.1.4",
     author="Zahcoder34",
     author_email="Zakhriw@gmail.com",
     description="An asynchronous Asterisk AMI Client for Python",
     url="https://github.com/Zahgrom34/aiopyami",
     packages=["aiopyami"],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `aiopyami-0.1.3/test/test_async_ami.py` & `aiopyami-0.1.4/test/test_async_ami.py`

 * *Files identical despite different names*

