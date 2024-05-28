# Comparing `tmp/ptprssi-1.0.1.tar.gz` & `tmp/ptprssi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptprssi-1.0.1.tar", last modified: Mon May  6 18:52:55 2024, max compression
+gzip compressed data, was "ptprssi-1.0.2.tar", last modified: Tue May 28 10:49:29 2024, max compression
```

## Comparing `ptprssi-1.0.1.tar` & `ptprssi-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 18:52:55.976677 ptprssi-1.0.1/
--rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-28 10:49:37.000000 ptprssi-1.0.1/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3623 2024-05-06 18:52:55.976677 ptprssi-1.0.1/PKG-INFO
--rwxr-xr-x   0 kali      (1000) kali      (1000)     2817 2024-04-28 10:49:37.000000 ptprssi-1.0.1/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 18:52:55.966677 ptprssi-1.0.1/ptprssi/
--rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-28 10:49:37.000000 ptprssi-1.0.1/ptprssi/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-06 18:50:13.000000 ptprssi-1.0.1/ptprssi/_version.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    10572 2024-05-06 18:46:14.000000 ptprssi-1.0.1/ptprssi/ptprssi.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 18:52:55.976677 ptprssi-1.0.1/ptprssi.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3623 2024-05-06 18:52:55.000000 ptprssi-1.0.1/ptprssi.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      273 2024-05-06 18:52:55.000000 ptprssi-1.0.1/ptprssi.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-06 18:52:55.000000 ptprssi-1.0.1/ptprssi.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2024-05-06 18:52:55.000000 ptprssi-1.0.1/ptprssi.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       22 2024-05-06 18:52:55.000000 ptprssi-1.0.1/ptprssi.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        8 2024-05-06 18:52:55.000000 ptprssi-1.0.1/ptprssi.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-06 18:52:55.976677 ptprssi-1.0.1/setup.cfg
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1257 2024-05-06 18:46:42.000000 ptprssi-1.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:49:29.571885 ptprssi-1.0.2/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-28 10:49:37.000000 ptprssi-1.0.2/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3622 2024-05-28 10:49:29.571885 ptprssi-1.0.2/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2815 2024-05-06 18:54:31.000000 ptprssi-1.0.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:49:29.571885 ptprssi-1.0.2/ptprssi/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-28 10:49:37.000000 ptprssi-1.0.2/ptprssi/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-28 10:48:33.000000 ptprssi-1.0.2/ptprssi/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    10810 2024-05-28 09:32:58.000000 ptprssi-1.0.2/ptprssi/ptprssi.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:49:29.571885 ptprssi-1.0.2/ptprssi.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3622 2024-05-28 10:49:29.000000 ptprssi-1.0.2/ptprssi.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      273 2024-05-28 10:49:29.000000 ptprssi-1.0.2/ptprssi.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-28 10:49:29.000000 ptprssi-1.0.2/ptprssi.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2024-05-28 10:49:29.000000 ptprssi-1.0.2/ptprssi.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       22 2024-05-28 10:49:29.000000 ptprssi-1.0.2/ptprssi.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        8 2024-05-28 10:49:29.000000 ptprssi-1.0.2/ptprssi.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-28 10:49:29.571885 ptprssi-1.0.2/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1257 2024-05-06 18:46:42.000000 ptprssi-1.0.2/setup.py
```

### Comparing `ptprssi-1.0.1/LICENSE` & `ptprssi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptprssi-1.0.1/PKG-INFO` & `ptprssi-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptprssi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Path-Relative Style Sheet Import Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptprssi
@@ -67,15 +67,14 @@
 -c  --cookie      <cookie>        Set Cookie(s)
 -t  --threads     <threads>       Set threads count
 -r  --redirects                   Follow redirects (default False)
 -C  --cache                       Cache HTTP communication (load from tmp in future)
 -v  --version                     Show script version and exit
 -h  --help                        Show this help message and exit
 -j  --json                        Output in JSON format
-
 ```
 
 ## Dependencies
 ```
 ptlibs
 bs4
 lxml
```

### Comparing `ptprssi-1.0.1/README.md` & `ptprssi-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 -c  --cookie      <cookie>        Set Cookie(s)
 -t  --threads     <threads>       Set threads count
 -r  --redirects                   Follow redirects (default False)
 -C  --cache                       Cache HTTP communication (load from tmp in future)
 -v  --version                     Show script version and exit
 -h  --help                        Show this help message and exit
 -j  --json                        Output in JSON format
-
 ```
 
 ## Dependencies
 ```
 ptlibs
 bs4
 lxml
```

### Comparing `ptprssi-1.0.1/ptprssi/ptprssi.py` & `ptprssi-1.0.2/ptprssi/ptprssi.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,19 @@
     parser.add_argument("-t",  "--threads",       type=int, default=100)
     parser.add_argument("-H",  "--headers",       type=ptmisclib.pairs)
     parser.add_argument("-r",  "--redirects",     action="store_true")
     parser.add_argument("-C",  "--cache",         action="store_true")
     parser.add_argument("-j",  "--json",          action="store_true")
     parser.add_argument("-v",  "--version",       action="version", version=f"{SCRIPTNAME} {__version__}")
 
+    parser.add_argument("--socket-address",          type=str, default=None)
+    parser.add_argument("--socket-port",             type=str, default=None)
+    parser.add_argument("--process-ident",           type=str, default=None)
+
+
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
         ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
     args = parser.parse_args()
     ptprinthelper.print_banner(SCRIPTNAME, __version__, args.json)
     return args
```

### Comparing `ptprssi-1.0.1/ptprssi.egg-info/PKG-INFO` & `ptprssi-1.0.2/ptprssi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptprssi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Path-Relative Style Sheet Import Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptprssi
@@ -67,15 +67,14 @@
 -c  --cookie      <cookie>        Set Cookie(s)
 -t  --threads     <threads>       Set threads count
 -r  --redirects                   Follow redirects (default False)
 -C  --cache                       Cache HTTP communication (load from tmp in future)
 -v  --version                     Show script version and exit
 -h  --help                        Show this help message and exit
 -j  --json                        Output in JSON format
-
 ```
 
 ## Dependencies
 ```
 ptlibs
 bs4
 lxml
```

### Comparing `ptprssi-1.0.1/setup.py` & `ptprssi-1.0.2/setup.py`

 * *Files identical despite different names*

