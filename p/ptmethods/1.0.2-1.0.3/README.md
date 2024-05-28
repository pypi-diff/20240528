# Comparing `tmp/ptmethods-1.0.2.tar.gz` & `tmp/ptmethods-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptmethods-1.0.2.tar", last modified: Tue May  7 11:43:25 2024, max compression
+gzip compressed data, was "ptmethods-1.0.3.tar", last modified: Tue May 28 10:37:49 2024, max compression
```

## Comparing `ptmethods-1.0.2.tar` & `ptmethods-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-07 11:43:25.390922 ptmethods-1.0.2/
--rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-05-06 14:28:31.000000 ptmethods-1.0.2/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     4285 2024-05-07 11:43:25.390922 ptmethods-1.0.2/PKG-INFO
--rwxr-xr-x   0 kali      (1000) kali      (1000)     3496 2024-05-07 11:39:41.000000 ptmethods-1.0.2/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-07 11:43:25.390922 ptmethods-1.0.2/ptmethods/
--rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 14:28:31.000000 ptmethods-1.0.2/ptmethods/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-07 11:34:00.000000 ptmethods-1.0.2/ptmethods/_version.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    15346 2024-05-07 11:42:23.000000 ptmethods-1.0.2/ptmethods/ptmethods.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-07 11:43:25.390922 ptmethods-1.0.2/ptmethods.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     4285 2024-05-07 11:43:25.000000 ptmethods-1.0.2/ptmethods.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      293 2024-05-07 11:43:25.000000 ptmethods-1.0.2/ptmethods.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-07 11:43:25.000000 ptmethods-1.0.2/ptmethods.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       55 2024-05-07 11:43:25.000000 ptmethods-1.0.2/ptmethods.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       26 2024-05-07 11:43:25.000000 ptmethods-1.0.2/ptmethods.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       10 2024-05-07 11:43:25.000000 ptmethods-1.0.2/ptmethods.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-07 11:43:25.390922 ptmethods-1.0.2/setup.cfg
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1264 2024-05-07 11:33:57.000000 ptmethods-1.0.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:37:49.921966 ptmethods-1.0.3/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-05-06 14:28:31.000000 ptmethods-1.0.3/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     4261 2024-05-28 10:37:49.921966 ptmethods-1.0.3/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     3496 2024-05-07 11:39:41.000000 ptmethods-1.0.3/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:37:49.921966 ptmethods-1.0.3/ptmethods/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 14:28:31.000000 ptmethods-1.0.3/ptmethods/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-28 10:35:48.000000 ptmethods-1.0.3/ptmethods/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    15586 2024-05-28 10:33:36.000000 ptmethods-1.0.3/ptmethods/ptmethods.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:37:49.921966 ptmethods-1.0.3/ptmethods.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4261 2024-05-28 10:37:49.000000 ptmethods-1.0.3/ptmethods.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      293 2024-05-28 10:37:49.000000 ptmethods-1.0.3/ptmethods.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-28 10:37:49.000000 ptmethods-1.0.3/ptmethods.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       55 2024-05-28 10:37:49.000000 ptmethods-1.0.3/ptmethods.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-28 10:37:49.000000 ptmethods-1.0.3/ptmethods.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       10 2024-05-28 10:37:49.000000 ptmethods-1.0.3/ptmethods.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-28 10:37:49.921966 ptmethods-1.0.3/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1252 2024-05-28 10:33:21.000000 ptmethods-1.0.3/setup.py
```

### Comparing `ptmethods-1.0.2/LICENSE` & `ptmethods-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ptmethods-1.0.2/PKG-INFO` & `ptmethods-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptmethods
-Version: 1.0.2
+Version: 1.0.3
 Summary: HTTP Methods Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptmethods
@@ -15,15 +15,14 @@
 Classifier: Environment :: Console
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ptlibs<2,>=1.0.7
-Requires-Dist: requests
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
 ## PTMETHODS - HTTP Methods Testing Tool
 
 - Script retrieves methods offered by server from OPTIONS request
```

### Comparing `ptmethods-1.0.2/README.md` & `ptmethods-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ptmethods-1.0.2/ptmethods/ptmethods.py` & `ptmethods-1.0.3/ptmethods/ptmethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         else:
             port = "443" if o.scheme == "https" else "80"
         return port, urllib.parse.urlunparse(o)
 
 
 def get_help():
     return [
-        {"description": ["HTTP methods testing tool"]},
+        {"description": ["HTTP Methods Testing Tool"]},
         {"usage": ["ptmethods <options>"]},
         {"Tip": ["Use this script against existing sources like homepages, images, or resources protected by HTTP authentication."]},
         {"usage_example": [
             "ptmethods -u https://www.example.com/image.png",
             "ptmethods -u https://www.example.com/index.php",
             "ptmethods -u https://www.example.com/index.php -c PHPSESSID=abcdef",
             "ptmethods -f urlList.txt",
@@ -260,17 +260,23 @@
     parser.add_argument("-r",  "--redirects",           action="store_true")
     parser.add_argument("-C",  "--cache",               action="store_true")
     parser.add_argument("-b",  "--check-basic-methods", action="store_true")
     parser.add_argument("-sr", "--show-response",       action="store_true")
     parser.add_argument("-sh", "--show-headers",        action="store_true")
     parser.add_argument("-v",  "--version",             action="version", version=f"{SCRIPTNAME} {__version__}")
 
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
     ptprinthelper.print_banner(SCRIPTNAME, __version__, args.json, space=0)
     return args
 
 
 def main():
     global SCRIPTNAME
```

### Comparing `ptmethods-1.0.2/ptmethods.egg-info/PKG-INFO` & `ptmethods-1.0.3/ptmethods.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptmethods
-Version: 1.0.2
+Version: 1.0.3
 Summary: HTTP Methods Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptmethods
@@ -15,15 +15,14 @@
 Classifier: Environment :: Console
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ptlibs<2,>=1.0.7
-Requires-Dist: requests
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
 ## PTMETHODS - HTTP Methods Testing Tool
 
 - Script retrieves methods offered by server from OPTIONS request
```

### Comparing `ptmethods-1.0.2/setup.py` & `ptmethods-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: Implementation :: CPython",
         "Environment :: Console",
         "Topic :: Security",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
     ],
     python_requires='>=3.9',
-    install_requires=["ptlibs>=1.0.7,<2", "requests"],
+    install_requires=["ptlibs>=1.0.7,<2"],
     entry_points = {'console_scripts': ['ptmethods = ptmethods.ptmethods:main']},
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls = {
     "homepage":   "https://www.penterep.com/",
     "repository": "https://github.com/penterep/ptmethods",
     "tracker":    "https://github.com/penterep/ptmethods/issues",
```

