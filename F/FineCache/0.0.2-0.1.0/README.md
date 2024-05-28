# Comparing `tmp/finecache-0.0.2.tar.gz` & `tmp/finecache-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finecache-0.0.2.tar", last modified: Tue Apr 30 15:49:13 2024, max compression
+gzip compressed data, was "finecache-0.1.0.tar", last modified: Tue May 28 11:57:19 2024, max compression
```

## Comparing `finecache-0.0.2.tar` & `finecache-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:49:13.090517 finecache-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:49:13.090517 finecache-0.0.2/FineCache/
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-30 15:49:09.000000 finecache-0.0.2/FineCache/CachedCall.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 15:49:09.000000 finecache-0.0.2/FineCache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-04-30 15:49:09.000000 finecache-0.0.2/FineCache/cachelib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:49:13.090517 finecache-0.0.2/FineCache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-30 15:49:13.000000 finecache-0.0.2/FineCache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-30 15:49:13.000000 finecache-0.0.2/FineCache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:49:13.000000 finecache-0.0.2/FineCache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 15:49:13.000000 finecache-0.0.2/FineCache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 15:49:09.000000 finecache-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-30 15:49:13.090517 finecache-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-30 15:49:09.000000 finecache-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:49:13.090517 finecache-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-30 15:49:09.000000 finecache-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:49:13.090517 finecache-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-30 15:49:09.000000 finecache-0.0.2/tests/test_cachelib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:57:19.381726 finecache-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:57:19.377726 finecache-0.1.0/FineCache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-28 11:57:10.000000 finecache-0.1.0/FineCache/CachedCall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-28 11:57:10.000000 finecache-0.1.0/FineCache/FineCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-28 11:57:10.000000 finecache-0.1.0/FineCache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-28 11:57:10.000000 finecache-0.1.0/FineCache/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:57:19.377726 finecache-0.1.0/FineCache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-28 11:57:19.000000 finecache-0.1.0/FineCache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 11:57:19.000000 finecache-0.1.0/FineCache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:57:19.000000 finecache-0.1.0/FineCache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 11:57:19.000000 finecache-0.1.0/FineCache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-28 11:57:10.000000 finecache-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-28 11:57:19.381726 finecache-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-28 11:57:10.000000 finecache-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:57:19.381726 finecache-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-28 11:57:10.000000 finecache-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:57:19.377726 finecache-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-28 11:57:10.000000 finecache-0.1.0/tests/test_cachelib.py
```

### Comparing `finecache-0.0.2/LICENSE` & `finecache-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finecache-0.0.2/setup.py` & `finecache-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="FineCache",
-  version="0.0.2",
+  version="0.1.0",
   author="Ciaran Chen",
   author_email="ciaranchen@qq.com",
-  description="A function cache for fine-tuning",
+  description="科研项目缓存中间结果和实验变动记录工具",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ciaranchen/FineCache",
   packages=setuptools.find_packages(),
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `finecache-0.0.2/tests/test_cachelib.py` & `finecache-0.1.0/tests/test_cachelib.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 import pickle
 import unittest
 from shutil import rmtree
 
-from FineCache import PickleCache, HistoryCache
+from FineCache import FineCache, IncrementDir
 
 
 def func(a1: int, a2: int, k1="v1", k2="v2"):
     """normal run function"""
     a3 = a1 + 1
     a4 = a2 + 2
     kr1, kr2 = k1[::-1], k2[::-1]
     # print(a1, a2, k1, k2)
     # print(a1, "+ 1 =", a1 + 1)
     return a3, a4, kr1, kr2
 
 
-class TestPickleCache(unittest.TestCase):
+class TestFineCache(unittest.TestCase):
     def setUp(self) -> None:
-        self.pc = PickleCache('.p_cache')
+        self.pc = FineCache('.p_cache')
 
     def tearDown(self):
         super().tearDown()
         # Clear folders...
         if os.path.exists('.p_cache'):
             rmtree('.p_cache')
 
@@ -46,15 +46,15 @@
         args = (3, lambda x: x + 2)
         kwargs = {'k1': 4, 'k2': lambda x: x + 3}
         _test_unpicklable(*args, **kwargs)
 
         wrapped = self.pc.cache()(_test_unpicklable)
         wrapped(*args, **kwargs)
 
-        filepaths = [file for file in os.listdir('.p_cache') if file.startswith(_test_unpicklable.__name__ + '@')]
+        filepaths = [file for file in os.listdir('.p_cache') if file.startswith(_test_unpicklable.__name__)]
         self.assertEqual(len(filepaths), 1)
         with open(os.path.join('.p_cache', filepaths[0]), 'rb') as fp:
             data = pickle.load(fp)
         self.assertEqual(data['func'], _test_unpicklable.__qualname__)
 
         self.assertEqual(len(data['args']), 2)
         self.assertEqual(data['args'][0], 3)
@@ -91,61 +91,41 @@
 
     def test_self_defined_hash(self):
         def test_func(a1, a2):
             return a1, a2
 
         wrapped = self.pc.cache(args_hash=[lambda a1: 'x', lambda a2: 'y'])(test_func)
         wrapped('a1', 'a2')
-        self.assertTrue(os.path.exists(os.path.join('.p_cache', "test_func@['x';'y']@.pk")))
+        self.assertTrue(os.path.exists(os.path.join('.p_cache', "test_func('x','y';).pk")))
 
 
 class TestHistoryCache(unittest.TestCase):
     def tearDown(self):
         super().tearDown()
         # Clear folders...
         if os.path.exists('.h_cache'):
             rmtree('.h_cache')
 
     def setUp(self) -> None:
-        self.hc = HistoryCache('.h_cache')
-
-        def _test_func_history(a1, a2):
-            """
-            test function version 1
-            :param a1:
-            :param a2:
-            :return:
-            """
-            return a1
-
-        self.wrapped1 = self.hc.cache()(_test_func_history)
-
-        def _test_func_history(a1, a2):
-            """
-            test function version 2
-            :param a1:
-            :param a2:
-            :return:
-            """
-            return a1 + 1
-
-        self.wrapped2 = self.hc.cache()(_test_func_history)
+        self.inc = IncrementDir('.h_cache', dir_prefix='test')
+        self.hc = FineCache('.h_cache', increment_dir=self.inc)
 
     def test_wrapped(self):
-        wrapped = self.hc.cache()(func)
+        wrapped = self.hc.record()(func)
         self.assertEqual(wrapped.__qualname__, func.__qualname__)
         self.assertEqual(wrapped.__doc__, func.__doc__)
 
-    def test_history_cache(self):
-        args = (1, 2)
-        self.assertEqual(self.wrapped1(*args) + 1, self.wrapped2(*args))
-
-        paths = [d for d in os.listdir('.h_cache') if d.startswith('_test_func_history@')]
-        self.assertEqual(len(paths), 1)
-
-    def test_unpicklable(self):
-        # TODO: finish it.
-        pass
+    def test_output_duplicate(self):
+        @self.hc.record()
+        def output():
+            print('123456789')
+
+        output()
+        _, latest_dir = self.inc.latest_number
+        filename = os.path.join('.h_cache', latest_dir, 'console.log')
+        with open(filename) as fp:
+            content = fp.read()
+        self.assertTrue('123456789' in content)
 
 
 if __name__ == '__main__':
     unittest.main()
```

