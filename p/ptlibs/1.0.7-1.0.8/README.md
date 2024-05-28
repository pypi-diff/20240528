# Comparing `tmp/ptlibs-1.0.7.tar.gz` & `tmp/ptlibs-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptlibs-1.0.7.tar", last modified: Thu May  9 13:54:34 2024, max compression
+gzip compressed data, was "ptlibs-1.0.8.tar", last modified: Tue May 28 09:40:41 2024, max compression
```

## Comparing `ptlibs-1.0.7.tar` & `ptlibs-1.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:54:34.055226 ptlibs-1.0.7/
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2024-04-27 19:41:20.000000 ptlibs-1.0.7/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     1565 2024-05-09 13:54:34.055226 ptlibs-1.0.7/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      849 2024-05-09 10:18:42.000000 ptlibs-1.0.7/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:54:34.055226 ptlibs-1.0.7/ptlibs/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-06 09:15:32.000000 ptlibs-1.0.7/ptlibs/_version.py
--rw-r--r--   0 kali      (1000) kali      (1000)      352 2024-05-09 10:18:42.000000 ptlibs-1.0.7/ptlibs/cli.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1115 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/ptcharsethelper.py
--rw-r--r--   0 kali      (1000) kali      (1000)      753 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/ptdefs.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6590 2024-05-09 10:18:42.000000 ptlibs-1.0.7/ptlibs/ptjsonlib.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7360 2024-05-09 10:18:42.000000 ptlibs-1.0.7/ptlibs/ptmisclib.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2096 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/ptnethelper.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7550 2024-05-09 10:18:37.000000 ptlibs-1.0.7/ptlibs/ptpathtypedetector.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5881 2024-05-06 15:00:46.000000 ptlibs-1.0.7/ptlibs/ptprinthelper.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:54:34.055226 ptlibs-1.0.7/ptlibs/threads/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/threads/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1040 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/threads/arraylock.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1316 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/threads/printlock.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2014 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/threads/ptthreads.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4092 2024-05-09 10:18:42.000000 ptlibs-1.0.7/ptlibs/tldparser.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:54:34.055226 ptlibs-1.0.7/ptlibs.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     1565 2024-05-09 13:54:34.000000 ptlibs-1.0.7/ptlibs.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      549 2024-05-09 13:54:34.000000 ptlibs-1.0.7/ptlibs.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 13:54:34.000000 ptlibs-1.0.7/ptlibs.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       43 2024-05-09 13:54:34.000000 ptlibs-1.0.7/ptlibs.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       27 2024-05-09 13:54:34.000000 ptlibs-1.0.7/ptlibs.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        7 2024-05-09 13:54:34.000000 ptlibs-1.0.7/ptlibs.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 13:54:34.055226 ptlibs-1.0.7/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1073 2024-05-09 13:54:08.000000 ptlibs-1.0.7/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 09:40:41.078046 ptlibs-1.0.8/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2024-04-27 19:41:20.000000 ptlibs-1.0.8/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     1565 2024-05-28 09:40:41.078046 ptlibs-1.0.8/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      849 2024-05-19 17:10:09.000000 ptlibs-1.0.8/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 09:40:41.068046 ptlibs-1.0.8/ptlibs/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-05-19 17:10:09.000000 ptlibs-1.0.8/ptlibs/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-19 17:11:49.000000 ptlibs-1.0.8/ptlibs/_version.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      352 2024-05-28 08:44:00.000000 ptlibs-1.0.8/ptlibs/cli.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1115 2024-04-27 19:41:20.000000 ptlibs-1.0.8/ptlibs/ptcharsethelper.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      753 2024-04-27 19:41:20.000000 ptlibs-1.0.8/ptlibs/ptdefs.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     9112 2024-05-19 19:34:59.000000 ptlibs-1.0.8/ptlibs/ptjsonlib.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7360 2024-05-28 09:39:32.000000 ptlibs-1.0.8/ptlibs/ptmisclib.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2135 2024-05-20 08:19:54.000000 ptlibs-1.0.8/ptlibs/ptnethelper.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7550 2024-05-19 17:10:09.000000 ptlibs-1.0.8/ptlibs/ptpathtypedetector.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5881 2024-05-19 17:10:09.000000 ptlibs-1.0.8/ptlibs/ptprinthelper.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 09:40:41.068046 ptlibs-1.0.8/ptlibs/threads/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-27 19:41:20.000000 ptlibs-1.0.8/ptlibs/threads/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1040 2024-04-27 19:41:20.000000 ptlibs-1.0.8/ptlibs/threads/arraylock.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1316 2024-04-27 19:41:20.000000 ptlibs-1.0.8/ptlibs/threads/printlock.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2014 2024-04-27 19:41:20.000000 ptlibs-1.0.8/ptlibs/threads/ptthreads.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4092 2024-05-19 17:10:09.000000 ptlibs-1.0.8/ptlibs/tldparser.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 09:40:41.078046 ptlibs-1.0.8/ptlibs.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1565 2024-05-28 09:40:41.000000 ptlibs-1.0.8/ptlibs.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      549 2024-05-28 09:40:41.000000 ptlibs-1.0.8/ptlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-28 09:40:41.000000 ptlibs-1.0.8/ptlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       43 2024-05-28 09:40:41.000000 ptlibs-1.0.8/ptlibs.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       27 2024-05-28 09:40:41.000000 ptlibs-1.0.8/ptlibs.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        7 2024-05-28 09:40:41.000000 ptlibs-1.0.8/ptlibs.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-28 09:40:41.078046 ptlibs-1.0.8/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1073 2024-05-19 17:10:09.000000 ptlibs-1.0.8/setup.py
```

### Comparing `ptlibs-1.0.7/LICENSE` & `ptlibs-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.7/PKG-INFO` & `ptlibs-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptlibs
-Version: 1.0.7
+Version: 1.0.8
 Summary: Support library for penterepTools
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptlibs
```

### Comparing `ptlibs-1.0.7/README.md` & `ptlibs-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.7/ptlibs/ptcharsethelper.py` & `ptlibs-1.0.8/ptlibs/ptcharsethelper.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.7/ptlibs/ptdefs.py` & `ptlibs-1.0.8/ptlibs/ptdefs.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.7/ptlibs/ptmisclib.py` & `ptlibs-1.0.8/ptlibs/ptmisclib.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.7/ptlibs/ptnethelper.py` & `ptlibs-1.0.8/ptlibs/ptnethelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,22 +46,22 @@
     except Exception as e:
         ptprint( out_if(f"{ptdefs.colors['ERROR']}URL is not available: {e}{ptdefs.colors['TEXT']}", "ERROR"))
         sys.exit(0)
 
 
 def get_request_headers(args) -> dict:
     request_headers = {}
-    if args.user_agent:
+    if vars(args).get("user_agent"):
         request_headers.update({"User-Agent": args.user_agent})
-    if args.cookie:
+    if vars(args).get("cookie"):
         if isinstance(args.cookie, list):
             request_headers.update({"Cookie": '; '.join(args.cookie)})
         elif isinstance(args.cookie, str):
             request_headers.update({"Cookie": args.cookie})
-    if args.headers:
+    if vars(args).get("headers"):
         for header in args.headers:
             request_headers.update({header.split(":")[0]: header.split(":")[1]})
     return request_headers
 
 
 def add_slash_to_end_url(url: str) -> str:
     if url.find("*") == -1 and not url.endswith("/"):
```

### Comparing `ptlibs-1.0.7/ptlibs/ptpathtypedetector.py` & `ptlibs-1.0.8/ptlibs/ptpathtypedetector.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.7/ptlibs/ptprinthelper.py` & `ptlibs-1.0.8/ptlibs/ptprinthelper.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.7/ptlibs/threads/arraylock.py` & `ptlibs-1.0.8/ptlibs/threads/arraylock.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.7/ptlibs/threads/printlock.py` & `ptlibs-1.0.8/ptlibs/threads/printlock.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.7/ptlibs/threads/ptthreads.py` & `ptlibs-1.0.8/ptlibs/threads/ptthreads.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.7/ptlibs/tldparser.py` & `ptlibs-1.0.8/ptlibs/tldparser.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.7/ptlibs.egg-info/PKG-INFO` & `ptlibs-1.0.8/ptlibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptlibs
-Version: 1.0.7
+Version: 1.0.8
 Summary: Support library for penterepTools
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptlibs
```

### Comparing `ptlibs-1.0.7/ptlibs.egg-info/SOURCES.txt` & `ptlibs-1.0.8/ptlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.7/setup.py` & `ptlibs-1.0.8/setup.py`

 * *Files identical despite different names*

