# Comparing `tmp/ptmultiviews-1.0.6.tar.gz` & `tmp/ptmultiviews-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptmultiviews-1.0.6.tar", last modified: Thu May  9 17:10:13 2024, max compression
+gzip compressed data, was "ptmultiviews-1.0.7.tar", last modified: Tue May 28 10:42:16 2024, max compression
```

## Comparing `ptmultiviews-1.0.6.tar` & `ptmultiviews-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:10:13.088027 ptmultiviews-1.0.6/
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2024-04-29 08:26:15.000000 ptmultiviews-1.0.6/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-09 17:10:13.088027 ptmultiviews-1.0.6/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     3596 2024-05-09 09:38:41.000000 ptmultiviews-1.0.6/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:10:13.088027 ptmultiviews-1.0.6/ptmultiviews/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:15.000000 ptmultiviews-1.0.6/ptmultiviews/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-09 17:08:39.000000 ptmultiviews-1.0.6/ptmultiviews/_version.py
--rw-r--r--   0 kali      (1000) kali      (1000)    16040 2024-05-09 17:07:56.000000 ptmultiviews-1.0.6/ptmultiviews/ptmultiviews.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:10:13.088027 ptmultiviews-1.0.6/ptmultiviews.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-09 17:10:13.000000 ptmultiviews-1.0.6/ptmultiviews.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      323 2024-05-09 17:10:13.000000 ptmultiviews-1.0.6/ptmultiviews.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 17:10:13.000000 ptmultiviews-1.0.6/ptmultiviews.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       64 2024-05-09 17:10:13.000000 ptmultiviews-1.0.6/ptmultiviews.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-09 17:10:13.000000 ptmultiviews-1.0.6/ptmultiviews.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2024-05-09 17:10:13.000000 ptmultiviews-1.0.6/ptmultiviews.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 17:10:13.088027 ptmultiviews-1.0.6/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1254 2024-05-09 10:21:25.000000 ptmultiviews-1.0.6/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:42:16.281930 ptmultiviews-1.0.7/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2024-04-29 08:26:15.000000 ptmultiviews-1.0.7/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-28 10:42:16.281930 ptmultiviews-1.0.7/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     3596 2024-05-09 09:38:41.000000 ptmultiviews-1.0.7/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:42:16.281930 ptmultiviews-1.0.7/ptmultiviews/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:15.000000 ptmultiviews-1.0.7/ptmultiviews/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-28 10:40:18.000000 ptmultiviews-1.0.7/ptmultiviews/_version.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    16274 2024-05-28 09:32:43.000000 ptmultiviews-1.0.7/ptmultiviews/ptmultiviews.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:42:16.281930 ptmultiviews-1.0.7/ptmultiviews.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-28 10:42:16.000000 ptmultiviews-1.0.7/ptmultiviews.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      323 2024-05-28 10:42:16.000000 ptmultiviews-1.0.7/ptmultiviews.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-28 10:42:16.000000 ptmultiviews-1.0.7/ptmultiviews.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       64 2024-05-28 10:42:16.000000 ptmultiviews-1.0.7/ptmultiviews.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-28 10:42:16.000000 ptmultiviews-1.0.7/ptmultiviews.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2024-05-28 10:42:16.000000 ptmultiviews-1.0.7/ptmultiviews.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-28 10:42:16.281930 ptmultiviews-1.0.7/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1254 2024-05-09 10:21:25.000000 ptmultiviews-1.0.7/setup.py
```

### Comparing `ptmultiviews-1.0.6/LICENSE` & `ptmultiviews-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ptmultiviews-1.0.6/PKG-INFO` & `ptmultiviews-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptmultiviews
-Version: 1.0.6
+Version: 1.0.7
 Summary: Apache Multiviews Detection & Enumeration Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptmultiviews
```

### Comparing `ptmultiviews-1.0.6/README.md` & `ptmultiviews-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ptmultiviews-1.0.6/ptmultiviews/ptmultiviews.py` & `ptmultiviews-1.0.7/ptmultiviews/ptmultiviews.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,17 +281,23 @@
     parser.add_argument("-wd", "--without-domain",       action="store_true")
     parser.add_argument("-wr", "--with-requested-url",   action="store_true")
     parser.add_argument("-r",  "--redirects",            action="store_true")
     parser.add_argument("-C",  "--cache",                action="store_true")
     parser.add_argument("-v",  "--version",              action="version", version=f"{SCRIPTNAME} {__version__}")
     parser.add_argument("-j",  "--json",                 action="store_true")
 
+    parser.add_argument("--socket-address",          type=str, default=None)
+    parser.add_argument("--socket-port",             type=str, default=None)
+    parser.add_argument("--process-ident",           type=str, default=None)
+
+
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
         ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
+
     args = parser.parse_args()
     ptprinthelper.print_banner(SCRIPTNAME, __version__, args.json)
     return args
 
 
 def main():
     global SCRIPTNAME
```

### Comparing `ptmultiviews-1.0.6/ptmultiviews.egg-info/PKG-INFO` & `ptmultiviews-1.0.7/ptmultiviews.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptmultiviews
-Version: 1.0.6
+Version: 1.0.7
 Summary: Apache Multiviews Detection & Enumeration Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptmultiviews
```

### Comparing `ptmultiviews-1.0.6/setup.py` & `ptmultiviews-1.0.7/setup.py`

 * *Files identical despite different names*

