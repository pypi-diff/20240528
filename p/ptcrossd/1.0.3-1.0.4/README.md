# Comparing `tmp/ptcrossd-1.0.3.tar.gz` & `tmp/ptcrossd-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcrossd-1.0.3.tar", last modified: Thu May  9 10:57:07 2024, max compression
+gzip compressed data, was "ptcrossd-1.0.4.tar", last modified: Tue May 28 10:18:47 2024, max compression
```

## Comparing `ptcrossd-1.0.3.tar` & `ptcrossd-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 10:57:07.230878 ptcrossd-1.0.3/
--rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:26:45.000000 ptcrossd-1.0.3/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3532 2024-05-09 10:57:07.230878 ptcrossd-1.0.3/PKG-INFO
--rwxr-xr-x   0 kali      (1000) kali      (1000)     2684 2024-04-29 08:26:45.000000 ptcrossd-1.0.3/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 10:57:07.230878 ptcrossd-1.0.3/ptcrossd/
--rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:45.000000 ptcrossd-1.0.3/ptcrossd/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-04-29 08:26:45.000000 ptcrossd-1.0.3/ptcrossd/_version.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    13651 2024-05-09 09:06:31.000000 ptcrossd-1.0.3/ptcrossd/ptcrossd.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 10:57:07.230878 ptcrossd-1.0.3/ptcrossd.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3532 2024-05-09 10:57:07.000000 ptcrossd-1.0.3/ptcrossd.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      283 2024-05-09 10:57:07.000000 ptcrossd-1.0.3/ptcrossd.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 10:57:07.000000 ptcrossd-1.0.3/ptcrossd.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       52 2024-05-09 10:57:07.000000 ptcrossd-1.0.3/ptcrossd.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       28 2024-05-09 10:57:07.000000 ptcrossd-1.0.3/ptcrossd.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        9 2024-05-09 10:57:07.000000 ptcrossd-1.0.3/ptcrossd.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 10:57:07.230878 ptcrossd-1.0.3/setup.cfg
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1293 2024-04-29 08:26:45.000000 ptcrossd-1.0.3/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:18:47.942105 ptcrossd-1.0.4/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:26:45.000000 ptcrossd-1.0.4/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3542 2024-05-28 10:18:47.932105 ptcrossd-1.0.4/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2684 2024-04-29 08:26:45.000000 ptcrossd-1.0.4/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:18:47.932105 ptcrossd-1.0.4/ptcrossd/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:45.000000 ptcrossd-1.0.4/ptcrossd/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-28 10:12:48.000000 ptcrossd-1.0.4/ptcrossd/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    13891 2024-05-28 08:58:51.000000 ptcrossd-1.0.4/ptcrossd/ptcrossd.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:18:47.932105 ptcrossd-1.0.4/ptcrossd.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3542 2024-05-28 10:18:47.000000 ptcrossd-1.0.4/ptcrossd.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      283 2024-05-28 10:18:47.000000 ptcrossd-1.0.4/ptcrossd.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-28 10:18:47.000000 ptcrossd-1.0.4/ptcrossd.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       52 2024-05-28 10:18:47.000000 ptcrossd-1.0.4/ptcrossd.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       28 2024-05-28 10:18:47.000000 ptcrossd-1.0.4/ptcrossd.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        9 2024-05-28 10:18:47.000000 ptcrossd-1.0.4/ptcrossd.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-28 10:18:47.942105 ptcrossd-1.0.4/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1303 2024-05-28 10:13:26.000000 ptcrossd-1.0.4/setup.py
```

### Comparing `ptcrossd-1.0.3/LICENSE` & `ptcrossd-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcrossd-1.0.3/PKG-INFO` & `ptcrossd-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ptcrossd
-Version: 1.0.3
+Version: 1.0.4
 Summary: Crossdomain.xml Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptcrossd
 Project-URL: tracker, https://github.com/penterep/ptcrossd/issues
-Project-URL: changelog, https://github.com/penterep/ptcrossd/CHANGELOG.md
+Project-URL: changelog, https://github.com/penterep/ptcrossd/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ptcrossd-1.0.3/README.md` & `ptcrossd-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ptcrossd-1.0.3/ptcrossd/ptcrossd.py` & `ptcrossd-1.0.4/ptcrossd/ptcrossd.py`

 * *Files 4% similar despite different names*

```diff
@@ -234,14 +234,20 @@
     parser.add_argument("-H",   "--headers",             type=ptmisclib.pairs, nargs="+")
     parser.add_argument("-cf",  "--cross-domain-file",   action="store_true")
     parser.add_argument("-ch",  "--cross-origin-header", action="store_true")
     parser.add_argument("-j",   "--json",                action="store_true")
     parser.add_argument("-C",   "--cache",               action="store_true")
     parser.add_argument("-v",   "--version",             action="version", version=f"{SCRIPTNAME} {__version__}")
 
+    parser.add_argument("--socket-address",          type=str, default=None)
+    parser.add_argument("--socket-port",             type=str, default=None)
+    parser.add_argument("--process-ident",           type=str, default=None)
+
+
+
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
         ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
 
     args = parser.parse_args()
     ptprinthelper.print_banner(SCRIPTNAME, __version__, args.json)
     return args
```

### Comparing `ptcrossd-1.0.3/ptcrossd.egg-info/PKG-INFO` & `ptcrossd-1.0.4/ptcrossd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ptcrossd
-Version: 1.0.3
+Version: 1.0.4
 Summary: Crossdomain.xml Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptcrossd
 Project-URL: tracker, https://github.com/penterep/ptcrossd/issues
-Project-URL: changelog, https://github.com/penterep/ptcrossd/CHANGELOG.md
+Project-URL: changelog, https://github.com/penterep/ptcrossd/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ptcrossd-1.0.3/setup.py` & `ptcrossd-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     include_package_data= True,
     long_description=long_description,
     long_description_content_type="text/markdown",
         project_urls = {
         "homepage":   "https://www.penterep.com/",
         "repository": "https://github.com/penterep/ptcrossd",
         "tracker":    "https://github.com/penterep/ptcrossd/issues",
-        "changelog":  "https://github.com/penterep/ptcrossd/CHANGELOG.md",
+        "changelog":  "https://github.com/penterep/ptcrossd/blob/main/CHANGELOG.md",
     }
 )
```

