# Comparing `tmp/r2pipe-1.8.8.tar.gz` & `tmp/r2pipe-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2pipe-1.8.8.tar", last modified: Thu Jan 11 18:02:01 2024, max compression
+gzip compressed data, was "r2pipe-1.9.0.tar", last modified: Tue May 28 16:24:57 2024, max compression
```

## Comparing `r2pipe-1.8.8.tar` & `r2pipe-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-01-11 18:02:01.286342 r2pipe-1.8.8/
--rw-r--r--   0 pancake    (501) staff       (20)     1075 2022-06-03 11:32:45.000000 r2pipe-1.8.8/LICENSE
--rw-r--r--   0 pancake    (501) staff       (20)       97 2022-06-03 11:32:45.000000 r2pipe-1.8.8/MANIFEST.in
--rw-r--r--   0 pancake    (501) staff       (20)      727 2024-01-11 18:02:01.286259 r2pipe-1.8.8/PKG-INFO
--rw-r--r--   0 pancake    (501) staff       (20)      488 2022-06-03 11:32:45.000000 r2pipe-1.8.8/README.md
-drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-01-11 18:02:01.285225 r2pipe-1.8.8/r2pipe/
--rw-r--r--   0 pancake    (501) staff       (20)     4804 2024-01-11 18:01:50.000000 r2pipe-1.8.8/r2pipe/__init__.py
--rw-r--r--   0 pancake    (501) staff       (20)     3602 2024-01-11 18:01:50.000000 r2pipe-1.8.8/r2pipe/native.py
--rw-r--r--   0 pancake    (501) staff       (20)     6517 2022-06-03 11:32:45.000000 r2pipe-1.8.8/r2pipe/open_async.py
--rw-r--r--   0 pancake    (501) staff       (20)     9938 2023-12-12 11:21:34.000000 r2pipe-1.8.8/r2pipe/open_base.py
--rw-r--r--   0 pancake    (501) staff       (20)     5996 2024-01-11 17:48:36.000000 r2pipe-1.8.8/r2pipe/open_sync.py
-drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-01-11 18:02:01.285751 r2pipe-1.8.8/r2pipe.egg-info/
--rw-r--r--   0 pancake    (501) staff       (20)      727 2024-01-11 18:02:01.000000 r2pipe-1.8.8/r2pipe.egg-info/PKG-INFO
--rw-r--r--   0 pancake    (501) staff       (20)      308 2024-01-11 18:02:01.000000 r2pipe-1.8.8/r2pipe.egg-info/SOURCES.txt
--rw-r--r--   0 pancake    (501) staff       (20)        1 2024-01-11 18:02:01.000000 r2pipe-1.8.8/r2pipe.egg-info/dependency_links.txt
--rw-r--r--   0 pancake    (501) staff       (20)        7 2024-01-11 18:02:01.000000 r2pipe-1.8.8/r2pipe.egg-info/top_level.txt
--rw-r--r--   0 pancake    (501) staff       (20)      261 2024-01-11 18:02:01.286600 r2pipe-1.8.8/setup.cfg
--rw-r--r--   0 pancake    (501) staff       (20)      422 2022-06-03 11:32:45.000000 r2pipe-1.8.8/setup.py
-drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-01-11 18:02:01.285999 r2pipe-1.8.8/test/
--rw-r--r--   0 pancake    (501) staff       (20)     2922 2024-01-11 17:41:44.000000 r2pipe-1.8.8/test/test_integration.py
--rw-r--r--   0 pancake    (501) staff       (20)      811 2024-01-11 17:40:27.000000 r2pipe-1.8.8/test/test_unit.py
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-05-28 16:24:57.683171 r2pipe-1.9.0/
+-rw-r--r--   0 pancake    (501) staff       (20)     1075 2022-06-03 11:32:45.000000 r2pipe-1.9.0/LICENSE
+-rw-r--r--   0 pancake    (501) staff       (20)       97 2022-06-03 11:32:45.000000 r2pipe-1.9.0/MANIFEST.in
+-rw-r--r--   0 pancake    (501) staff       (20)      727 2024-05-28 16:24:57.683120 r2pipe-1.9.0/PKG-INFO
+-rw-r--r--   0 pancake    (501) staff       (20)      488 2022-06-03 11:32:45.000000 r2pipe-1.9.0/README.md
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-05-28 16:24:57.681993 r2pipe-1.9.0/r2pipe/
+-rw-r--r--   0 pancake    (501) staff       (20)     5147 2024-05-28 16:23:23.000000 r2pipe-1.9.0/r2pipe/__init__.py
+-rw-r--r--   0 pancake    (501) staff       (20)     3602 2024-01-11 18:01:50.000000 r2pipe-1.9.0/r2pipe/native.py
+-rw-r--r--   0 pancake    (501) staff       (20)     6517 2022-06-03 11:32:45.000000 r2pipe-1.9.0/r2pipe/open_async.py
+-rw-r--r--   0 pancake    (501) staff       (20)     9938 2023-12-12 11:21:34.000000 r2pipe-1.9.0/r2pipe/open_base.py
+-rw-r--r--   0 pancake    (501) staff       (20)     5996 2024-01-11 17:48:36.000000 r2pipe-1.9.0/r2pipe/open_sync.py
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-05-28 16:24:57.682940 r2pipe-1.9.0/r2pipe.egg-info/
+-rw-r--r--   0 pancake    (501) staff       (20)      727 2024-05-28 16:24:57.000000 r2pipe-1.9.0/r2pipe.egg-info/PKG-INFO
+-rw-r--r--   0 pancake    (501) staff       (20)      308 2024-05-28 16:24:57.000000 r2pipe-1.9.0/r2pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 pancake    (501) staff       (20)        1 2024-05-28 16:24:57.000000 r2pipe-1.9.0/r2pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 pancake    (501) staff       (20)        7 2024-05-28 16:24:57.000000 r2pipe-1.9.0/r2pipe.egg-info/top_level.txt
+-rw-r--r--   0 pancake    (501) staff       (20)      261 2024-05-28 16:24:57.683365 r2pipe-1.9.0/setup.cfg
+-rw-r--r--   0 pancake    (501) staff       (20)      422 2022-06-03 11:32:45.000000 r2pipe-1.9.0/setup.py
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-05-28 16:24:57.682684 r2pipe-1.9.0/test/
+-rw-r--r--   0 pancake    (501) staff       (20)     2922 2024-01-11 17:41:44.000000 r2pipe-1.9.0/test/test_integration.py
+-rw-r--r--   0 pancake    (501) staff       (20)      811 2024-01-11 17:40:27.000000 r2pipe-1.9.0/test/test_unit.py
```

### Comparing `r2pipe-1.8.8/LICENSE` & `r2pipe-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `r2pipe-1.8.8/PKG-INFO` & `r2pipe-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r2pipe
-Version: 1.8.8
+Version: 1.9.0
 Summary: Pipe interface for radare2
 Home-page: https://rada.re
 Author: pancake
 Author-email: pancake@nopcode.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `r2pipe-1.8.8/r2pipe/__init__.py` & `r2pipe-1.9.0/r2pipe/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,41 +20,52 @@
   > import r2pipe
   > r = r2pipe.open("/bin/ls")
   > print(r.cmd("pd 10"))
   > print(r.cmdj("aoj")[0]['size'])
   > r.quit()
 """
 
-import os
-import sys
-import time
-from r2pipe.open_sync import open as r2pipe_open
-
-open = r2pipe_open
+from r2pipe.open_sync import open
 
 try:
     import r2lang
 except ImportError:
     r2lang = None
 
-VERSION = "1.8.8"
+VERSION = "1.9.0"
+
+def in_r2():
+    """Return wheter r2pipe is called from radare2 environment or the system shell
+        """
+    try:
+      import os
+      a = int(os.environ["R2PIPE_IN"]),
+      b = int(os.environ["R2PIPE_OUT"]),
+      return a > 0 and b > 0
+    except:
+      return False
 
+from r2pipe.open_base import in_rlang
 
 def version():
     """Return string with the version of the r2pipe library
         """
     return VERSION
 
 
 # Open class is now in open_base.py
 if __name__ == "__main__":
+    import os
+    import sys
+    from r2pipe.open_sync import open as r2pipe_open
     print("[+] Spawning r2 tcp and http servers")
     os.system("pkill r2")
     os.system("radare2 -qc.:9080 /bin/ls &")
     os.system("radare2 -qc=h /bin/ls &")
+    import time
     time.sleep(1)
 
     if sys.version_info <= (3, 0):
         # Test r2pipe with local process
         print("[+] Testing python r2pipe local")
         rlocal = r2pipe_open("/bin/ls")
         print(rlocal.cmd("pi 5"))
```

### Comparing `r2pipe-1.8.8/r2pipe/native.py` & `r2pipe-1.9.0/r2pipe/native.py`

 * *Files identical despite different names*

### Comparing `r2pipe-1.8.8/r2pipe/open_async.py` & `r2pipe-1.9.0/r2pipe/open_async.py`

 * *Files identical despite different names*

### Comparing `r2pipe-1.8.8/r2pipe/open_base.py` & `r2pipe-1.9.0/r2pipe/open_base.py`

 * *Files identical despite different names*

### Comparing `r2pipe-1.8.8/r2pipe/open_sync.py` & `r2pipe-1.9.0/r2pipe/open_sync.py`

 * *Files identical despite different names*

### Comparing `r2pipe-1.8.8/r2pipe.egg-info/PKG-INFO` & `r2pipe-1.9.0/r2pipe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r2pipe
-Version: 1.8.8
+Version: 1.9.0
 Summary: Pipe interface for radare2
 Home-page: https://rada.re
 Author: pancake
 Author-email: pancake@nopcode.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `r2pipe-1.8.8/test/test_integration.py` & `r2pipe-1.9.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `r2pipe-1.8.8/test/test_unit.py` & `r2pipe-1.9.0/test/test_unit.py`

 * *Files identical despite different names*

