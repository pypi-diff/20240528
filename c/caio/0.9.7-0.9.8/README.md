# Comparing `tmp/caio-0.9.7.tar.gz` & `tmp/caio-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caio-0.9.7.tar", last modified: Wed Aug 10 14:41:23 2022, max compression
+gzip compressed data, was "caio-0.9.8.tar", last modified: Sun Aug 14 06:53:14 2022, max compression
```

## Comparing `caio-0.9.7.tar` & `caio-0.9.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 14:41:23.981749 caio-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-10 14:41:17.000000 caio-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-08-10 14:41:17.000000 caio-0.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3215 2022-08-10 14:41:23.981749 caio-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-08-10 14:41:17.000000 caio-0.9.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 14:41:23.977749 caio-0.9.7/caio/
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-08-10 14:41:17.000000 caio-0.9.7/caio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-08-10 14:41:17.000000 caio-0.9.7/caio/abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-08-10 14:41:17.000000 caio-0.9.7/caio/asyncio_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    24526 2022-08-10 14:41:17.000000 caio-0.9.7/caio/linux_aio.c
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-08-10 14:41:17.000000 caio-0.9.7/caio/linux_aio.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-08-10 14:41:17.000000 caio-0.9.7/caio/linux_aio_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 14:41:17.000000 caio-0.9.7/caio/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     7162 2022-08-10 14:41:17.000000 caio-0.9.7/caio/python_aio.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-08-10 14:41:17.000000 caio-0.9.7/caio/python_aio_asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 14:41:23.977749 caio-0.9.7/caio/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 14:41:23.981749 caio-0.9.7/caio/src/threadpool/
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-08-10 14:41:17.000000 caio-0.9.7/caio/src/threadpool/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     8482 2022-08-10 14:41:17.000000 caio-0.9.7/caio/src/threadpool/threadpool.c
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-08-10 14:41:17.000000 caio-0.9.7/caio/src/threadpool/threadpool.h
--rw-r--r--   0 runner    (1001) docker     (121)    19008 2022-08-10 14:41:17.000000 caio-0.9.7/caio/thread_aio.c
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-08-10 14:41:17.000000 caio-0.9.7/caio/thread_aio.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-08-10 14:41:17.000000 caio-0.9.7/caio/thread_aio_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-08-10 14:41:17.000000 caio-0.9.7/caio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 14:41:23.977749 caio-0.9.7/caio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3215 2022-08-10 14:41:23.000000 caio-0.9.7/caio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-08-10 14:41:23.000000 caio-0.9.7/caio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 14:41:23.000000 caio-0.9.7/caio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-10 14:41:23.000000 caio-0.9.7/caio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-10 14:41:23.000000 caio-0.9.7/caio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-10 14:41:23.981749 caio-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-08-10 14:41:17.000000 caio-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:53:14.289030 caio-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-14 06:53:04.000000 caio-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-08-14 06:53:04.000000 caio-0.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3215 2022-08-14 06:53:14.289030 caio-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-08-14 06:53:04.000000 caio-0.9.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:53:14.289030 caio-0.9.8/caio/
+-rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-08-14 06:53:04.000000 caio-0.9.8/caio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-08-14 06:53:04.000000 caio-0.9.8/caio/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-08-14 06:53:04.000000 caio-0.9.8/caio/asyncio_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24526 2022-08-14 06:53:04.000000 caio-0.9.8/caio/linux_aio.c
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-08-14 06:53:04.000000 caio-0.9.8/caio/linux_aio.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2022-08-14 06:53:04.000000 caio-0.9.8/caio/linux_aio_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-14 06:53:04.000000 caio-0.9.8/caio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     7162 2022-08-14 06:53:04.000000 caio-0.9.8/caio/python_aio.py
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-08-14 06:53:04.000000 caio-0.9.8/caio/python_aio_asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:53:14.289030 caio-0.9.8/caio/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:53:14.289030 caio-0.9.8/caio/src/threadpool/
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-08-14 06:53:04.000000 caio-0.9.8/caio/src/threadpool/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     8482 2022-08-14 06:53:04.000000 caio-0.9.8/caio/src/threadpool/threadpool.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-08-14 06:53:04.000000 caio-0.9.8/caio/src/threadpool/threadpool.h
+-rw-r--r--   0 runner    (1001) docker     (121)    19008 2022-08-14 06:53:04.000000 caio-0.9.8/caio/thread_aio.c
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-08-14 06:53:04.000000 caio-0.9.8/caio/thread_aio.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-08-14 06:53:04.000000 caio-0.9.8/caio/thread_aio_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-08-14 06:53:04.000000 caio-0.9.8/caio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:53:14.289030 caio-0.9.8/caio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3215 2022-08-14 06:53:14.000000 caio-0.9.8/caio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-08-14 06:53:14.000000 caio-0.9.8/caio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-14 06:53:14.000000 caio-0.9.8/caio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-14 06:53:14.000000 caio-0.9.8/caio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-14 06:53:14.000000 caio-0.9.8/caio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-14 06:53:14.289030 caio-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-08-14 06:53:04.000000 caio-0.9.8/setup.py
```

### Comparing `caio-0.9.7/LICENSE` & `caio-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `caio-0.9.7/PKG-INFO` & `caio-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caio
-Version: 0.9.7
+Version: 0.9.8
 Summary: Asynchronous file IO for Linux MacOS or Windows.
 Home-page: UNKNOWN
 Author: Dmitry Orlov <me@mosquito.su>
 Author-email: me@mosquito.su
 License: Apache Software License
 Project-URL: Documentation, https://github.com/mosquito/caio/
 Project-URL: Source, https://github.com/mosquito/caio
```

### Comparing `caio-0.9.7/README.rst` & `caio-0.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `caio-0.9.7/caio/__init__.py` & `caio-0.9.8/caio/__init__.py`

 * *Files identical despite different names*

### Comparing `caio-0.9.7/caio/abstract.py` & `caio-0.9.8/caio/abstract.py`

 * *Files identical despite different names*

### Comparing `caio-0.9.7/caio/asyncio_base.py` & `caio-0.9.8/caio/asyncio_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         In general case impossible predict current thread and the thread
         of event loop. So have to use `call_soon_threadsave` the result setter.
         """
 
         if future.done():
             return
 
-        self.loop.call_soon_threadsafe(future.set_result, True)
+        self.loop.call_soon_threadsafe(
+            lambda: future.done() or future.set_result(True)
+        )
 
     def read(
         self, nbytes: int, fd: int,
         offset: int, priority: int = 0,
     ) -> typing.Awaitable[bytes]:
         return self.submit(
             self.OPERATION_CLASS.read(nbytes, fd, offset, priority),
```

### Comparing `caio-0.9.7/caio/linux_aio.c` & `caio-0.9.8/caio/linux_aio.c`

 * *Files identical despite different names*

### Comparing `caio-0.9.7/caio/linux_aio_asyncio.py` & `caio-0.9.8/caio/linux_aio_asyncio.py`

 * *Files identical despite different names*

### Comparing `caio-0.9.7/caio/python_aio.py` & `caio-0.9.8/caio/python_aio.py`

 * *Files identical despite different names*

### Comparing `caio-0.9.7/caio/src/threadpool/README.md` & `caio-0.9.8/caio/src/threadpool/README.md`

 * *Files identical despite different names*

### Comparing `caio-0.9.7/caio/src/threadpool/threadpool.c` & `caio-0.9.8/caio/src/threadpool/threadpool.c`

 * *Files identical despite different names*

### Comparing `caio-0.9.7/caio/src/threadpool/threadpool.h` & `caio-0.9.8/caio/src/threadpool/threadpool.h`

 * *Files identical despite different names*

### Comparing `caio-0.9.7/caio/thread_aio.c` & `caio-0.9.8/caio/thread_aio.c`

 * *Files identical despite different names*

### Comparing `caio-0.9.7/caio.egg-info/PKG-INFO` & `caio-0.9.8/caio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caio
-Version: 0.9.7
+Version: 0.9.8
 Summary: Asynchronous file IO for Linux MacOS or Windows.
 Home-page: UNKNOWN
 Author: Dmitry Orlov <me@mosquito.su>
 Author-email: me@mosquito.su
 License: Apache Software License
 Project-URL: Documentation, https://github.com/mosquito/caio/
 Project-URL: Source, https://github.com/mosquito/caio
```

### Comparing `caio-0.9.7/caio.egg-info/SOURCES.txt` & `caio-0.9.8/caio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caio-0.9.7/setup.py` & `caio-0.9.8/setup.py`

 * *Files identical despite different names*

