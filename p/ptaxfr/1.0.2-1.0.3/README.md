# Comparing `tmp/ptaxfr-1.0.2.tar.gz` & `tmp/ptaxfr-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptaxfr-1.0.2.tar", last modified: Thu May  9 17:22:20 2024, max compression
+gzip compressed data, was "ptaxfr-1.0.3.tar", last modified: Tue May 28 09:58:32 2024, max compression
```

## Comparing `ptaxfr-1.0.2.tar` & `ptaxfr-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:22:20.746229 ptaxfr-1.0.2/
--rw-r--r--   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:26:26.000000 ptaxfr-1.0.2/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3539 2024-05-09 17:22:20.746229 ptaxfr-1.0.2/PKG-INFO
--rwxr-xr-x   0 kali      (1000) kali      (1000)     2766 2024-05-07 11:51:11.000000 ptaxfr-1.0.2/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:22:20.746229 ptaxfr-1.0.2/ptaxfr/
--rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:26.000000 ptaxfr-1.0.2/ptaxfr/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       23 2024-05-09 17:18:37.000000 ptaxfr-1.0.2/ptaxfr/_version.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    14421 2024-05-09 17:17:20.000000 ptaxfr-1.0.2/ptaxfr/ptaxfr.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:22:20.746229 ptaxfr-1.0.2/ptaxfr.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3539 2024-05-09 17:22:20.000000 ptaxfr-1.0.2/ptaxfr.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      263 2024-05-09 17:22:20.000000 ptaxfr-1.0.2/ptaxfr.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 17:22:20.000000 ptaxfr-1.0.2/ptaxfr.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       46 2024-05-09 17:22:20.000000 ptaxfr-1.0.2/ptaxfr.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       32 2024-05-09 17:22:20.000000 ptaxfr-1.0.2/ptaxfr.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        7 2024-05-09 17:22:20.000000 ptaxfr-1.0.2/ptaxfr.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 17:22:20.746229 ptaxfr-1.0.2/setup.cfg
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1289 2024-05-07 11:50:53.000000 ptaxfr-1.0.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 09:58:32.327918 ptaxfr-1.0.3/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:26:26.000000 ptaxfr-1.0.3/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3539 2024-05-28 09:58:32.327918 ptaxfr-1.0.3/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2766 2024-05-07 11:51:11.000000 ptaxfr-1.0.3/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 09:58:32.327918 ptaxfr-1.0.3/ptaxfr/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:26.000000 ptaxfr-1.0.3/ptaxfr/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       23 2024-05-28 09:52:12.000000 ptaxfr-1.0.3/ptaxfr/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    14661 2024-05-28 08:56:37.000000 ptaxfr-1.0.3/ptaxfr/ptaxfr.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 09:58:32.327918 ptaxfr-1.0.3/ptaxfr.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3539 2024-05-28 09:58:32.000000 ptaxfr-1.0.3/ptaxfr.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      263 2024-05-28 09:58:32.000000 ptaxfr-1.0.3/ptaxfr.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-28 09:58:32.000000 ptaxfr-1.0.3/ptaxfr.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       46 2024-05-28 09:58:32.000000 ptaxfr-1.0.3/ptaxfr.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       32 2024-05-28 09:58:32.000000 ptaxfr-1.0.3/ptaxfr.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        7 2024-05-28 09:58:32.000000 ptaxfr-1.0.3/ptaxfr.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-28 09:58:32.327918 ptaxfr-1.0.3/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1289 2024-05-07 11:50:53.000000 ptaxfr-1.0.3/setup.py
```

### Comparing `ptaxfr-1.0.2/LICENSE` & `ptaxfr-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ptaxfr-1.0.2/PKG-INFO` & `ptaxfr-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptaxfr
-Version: 1.0.2
+Version: 1.0.3
 Summary: DNS Zone Transfer Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptaxfr
```

### Comparing `ptaxfr-1.0.2/README.md` & `ptaxfr-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ptaxfr-1.0.2/ptaxfr/ptaxfr.py` & `ptaxfr-1.0.3/ptaxfr/ptaxfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,19 +219,25 @@
     parser.add_argument("-ps", "--print-subdomains", action="store_true")
     parser.add_argument("-u", "--unique",            action="store_true")
     parser.add_argument("-V", "--vulnerable-only",   action="store_true")
     parser.add_argument("-s", "--silent",            action="store_true")
     parser.add_argument("-j", "--json",              action="store_true")
     parser.add_argument("-v", "--version",           action="version", version=f"{SCRIPTNAME} {__version__}")
 
+    parser.add_argument("--socket-address",          type=str, default=None)
+    parser.add_argument("--socket-port",             type=str, default=None)
+    parser.add_argument("--process-ident",           type=str, default=None)
+
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
         ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
+
     args = parser.parse_args()
     ptprinthelper.print_banner(SCRIPTNAME, __version__, args.json or args.silent, space=0)
+
     return args
 
 
 def main():
     global SCRIPTNAME
     SCRIPTNAME = "ptaxfr"
     args = parse_args()
```

### Comparing `ptaxfr-1.0.2/ptaxfr.egg-info/PKG-INFO` & `ptaxfr-1.0.3/ptaxfr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptaxfr
-Version: 1.0.2
+Version: 1.0.3
 Summary: DNS Zone Transfer Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptaxfr
```

### Comparing `ptaxfr-1.0.2/setup.py` & `ptaxfr-1.0.3/setup.py`

 * *Files identical despite different names*

