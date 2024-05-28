# Comparing `tmp/ptsamesite-1.0.2.tar.gz` & `tmp/ptsamesite-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptsamesite-1.0.2.tar", last modified: Thu May  9 16:50:59 2024, max compression
+gzip compressed data, was "ptsamesite-1.0.3.tar", last modified: Tue May 28 10:51:47 2024, max compression
```

## Comparing `ptsamesite-1.0.2.tar` & `ptsamesite-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 16:50:59.458358 ptsamesite-1.0.2/
--rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:24:58.000000 ptsamesite-1.0.2/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3682 2024-05-09 16:50:59.458358 ptsamesite-1.0.2/PKG-INFO
--rwxr-xr-x   0 kali      (1000) kali      (1000)     2884 2024-05-07 11:36:10.000000 ptsamesite-1.0.2/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 16:50:59.458358 ptsamesite-1.0.2/ptsamesite/
--rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:24:58.000000 ptsamesite-1.0.2/ptsamesite/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-09 16:49:51.000000 ptsamesite-1.0.2/ptsamesite/_version.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     7305 2024-05-09 16:49:39.000000 ptsamesite-1.0.2/ptsamesite/ptsamesite.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 16:50:59.458358 ptsamesite-1.0.2/ptsamesite.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3682 2024-05-09 16:50:59.000000 ptsamesite-1.0.2/ptsamesite.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      303 2024-05-09 16:50:59.000000 ptsamesite-1.0.2/ptsamesite.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 16:50:59.000000 ptsamesite-1.0.2/ptsamesite.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       58 2024-05-09 16:50:59.000000 ptsamesite-1.0.2/ptsamesite.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       32 2024-05-09 16:50:59.000000 ptsamesite-1.0.2/ptsamesite.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       11 2024-05-09 16:50:59.000000 ptsamesite-1.0.2/ptsamesite.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 16:50:59.458358 ptsamesite-1.0.2/setup.cfg
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1309 2024-05-06 17:02:21.000000 ptsamesite-1.0.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:51:47.001868 ptsamesite-1.0.3/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:24:58.000000 ptsamesite-1.0.3/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3682 2024-05-28 10:51:47.001868 ptsamesite-1.0.3/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2884 2024-05-07 11:36:10.000000 ptsamesite-1.0.3/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:51:46.991868 ptsamesite-1.0.3/ptsamesite/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:24:58.000000 ptsamesite-1.0.3/ptsamesite/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-28 10:50:49.000000 ptsamesite-1.0.3/ptsamesite/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     7543 2024-05-28 09:33:07.000000 ptsamesite-1.0.3/ptsamesite/ptsamesite.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:51:47.001868 ptsamesite-1.0.3/ptsamesite.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3682 2024-05-28 10:51:46.000000 ptsamesite-1.0.3/ptsamesite.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      303 2024-05-28 10:51:46.000000 ptsamesite-1.0.3/ptsamesite.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-28 10:51:46.000000 ptsamesite-1.0.3/ptsamesite.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       58 2024-05-28 10:51:46.000000 ptsamesite-1.0.3/ptsamesite.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       32 2024-05-28 10:51:46.000000 ptsamesite-1.0.3/ptsamesite.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       11 2024-05-28 10:51:46.000000 ptsamesite-1.0.3/ptsamesite.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-28 10:51:47.001868 ptsamesite-1.0.3/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1309 2024-05-06 17:02:21.000000 ptsamesite-1.0.3/setup.py
```

### Comparing `ptsamesite-1.0.2/LICENSE` & `ptsamesite-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ptsamesite-1.0.2/PKG-INFO` & `ptsamesite-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptsamesite
-Version: 1.0.2
+Version: 1.0.3
 Summary: Same Site Scripting Detection Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptsamesite
```

### Comparing `ptsamesite-1.0.2/README.md` & `ptsamesite-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ptsamesite-1.0.2/ptsamesite/ptsamesite.py` & `ptsamesite-1.0.3/ptsamesite/ptsamesite.py`

 * *Files 8% similar despite different names*

```diff
@@ -125,14 +125,19 @@
     exclusive_group.add_argument("-f", "--file",   type=str)
     parser.add_argument("-t", "--threads",         type=int, default=20)
     parser.add_argument("-s", "--subdomains",      action="store_true")
     parser.add_argument("-V", "--vulnerable",      action="store_true")
     parser.add_argument("-j", "--json",            action="store_true")
     parser.add_argument("-v", "--version",         action="version", version=f"{SCRIPTNAME} {__version__}")
 
+    parser.add_argument("--socket-address",          type=str, default=None)
+    parser.add_argument("--socket-port",             type=str, default=None)
+    parser.add_argument("--process-ident",           type=str, default=None)
+
+
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
         ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
 
     args = parser.parse_args()
     ptprinthelper.print_banner(SCRIPTNAME, __version__, args.json, space=0)
     return args
```

### Comparing `ptsamesite-1.0.2/ptsamesite.egg-info/PKG-INFO` & `ptsamesite-1.0.3/ptsamesite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptsamesite
-Version: 1.0.2
+Version: 1.0.3
 Summary: Same Site Scripting Detection Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptsamesite
```

### Comparing `ptsamesite-1.0.2/setup.py` & `ptsamesite-1.0.3/setup.py`

 * *Files identical despite different names*

