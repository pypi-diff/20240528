# Comparing `tmp/pthost-1.0.1.tar.gz` & `tmp/pthost-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pthost-1.0.1.tar", last modified: Thu May  9 21:15:18 2024, max compression
+gzip compressed data, was "pthost-1.0.2.tar", last modified: Tue May 28 10:22:53 2024, max compression
```

## Comparing `pthost-1.0.1.tar` & `pthost-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 21:15:18.161941 pthost-1.0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)    35823 2024-04-29 07:56:41.000000 pthost-1.0.1/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)       35 2024-04-29 07:56:41.000000 pthost-1.0.1/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     4835 2024-05-09 21:15:18.161941 pthost-1.0.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     4078 2024-04-30 09:47:21.000000 pthost-1.0.1/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 21:15:18.161941 pthost-1.0.1/pthost/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 07:56:41.000000 pthost-1.0.1/pthost/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-09 21:04:38.000000 pthost-1.0.1/pthost/_version.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 21:15:18.161941 pthost-1.0.1/pthost/modules/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 21:15:18.161941 pthost-1.0.1/pthost/modules/__pycache__/
--rw-r--r--   0 kali      (1000) kali      (1000)      778 2024-04-29 07:59:42.000000 pthost-1.0.1/pthost/modules/__pycache__/results.cpython-311.pyc
--rw-r--r--   0 kali      (1000) kali      (1000)    17424 2024-04-30 09:42:11.000000 pthost-1.0.1/pthost/modules/__pycache__/scanner.cpython-311.pyc
--rw-r--r--   0 kali      (1000) kali      (1000)    17449 2024-04-29 13:59:10.000000 pthost-1.0.1/pthost/modules/__pycache__/vuln_tester.cpython-311.pyc
--rw-r--r--   0 kali      (1000) kali      (1000)    12696 2024-04-30 09:42:10.000000 pthost-1.0.1/pthost/modules/scanner.py
--rw-r--r--   0 kali      (1000) kali      (1000)    10776 2024-05-09 21:13:40.000000 pthost-1.0.1/pthost/pthost.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 21:15:18.161941 pthost-1.0.1/pthost.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     4835 2024-05-09 21:15:18.000000 pthost-1.0.1/pthost.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      458 2024-05-09 21:15:18.000000 pthost-1.0.1/pthost.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 21:15:18.000000 pthost-1.0.1/pthost.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       46 2024-05-09 21:15:18.000000 pthost-1.0.1/pthost.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       28 2024-05-09 21:15:18.000000 pthost-1.0.1/pthost.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        7 2024-05-09 21:15:18.000000 pthost-1.0.1/pthost.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 21:15:18.161941 pthost-1.0.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1290 2024-05-09 21:04:09.000000 pthost-1.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:22:53.262071 pthost-1.0.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35823 2024-04-29 07:56:41.000000 pthost-1.0.2/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)       35 2024-04-29 07:56:41.000000 pthost-1.0.2/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     4171 2024-05-28 10:22:53.262071 pthost-1.0.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     3415 2024-05-28 10:21:28.000000 pthost-1.0.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:22:53.262071 pthost-1.0.2/pthost/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 07:56:41.000000 pthost-1.0.2/pthost/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-28 10:21:50.000000 pthost-1.0.2/pthost/_version.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:22:53.262071 pthost-1.0.2/pthost/modules/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:22:53.262071 pthost-1.0.2/pthost/modules/__pycache__/
+-rw-r--r--   0 kali      (1000) kali      (1000)      778 2024-04-29 07:59:42.000000 pthost-1.0.2/pthost/modules/__pycache__/results.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)    17424 2024-04-30 09:42:11.000000 pthost-1.0.2/pthost/modules/__pycache__/scanner.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)    17449 2024-04-29 13:59:10.000000 pthost-1.0.2/pthost/modules/__pycache__/vuln_tester.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)    12696 2024-04-30 09:42:10.000000 pthost-1.0.2/pthost/modules/scanner.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    10959 2024-05-28 10:16:14.000000 pthost-1.0.2/pthost/pthost.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:22:53.262071 pthost-1.0.2/pthost.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4171 2024-05-28 10:22:53.000000 pthost-1.0.2/pthost.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      458 2024-05-28 10:22:53.000000 pthost-1.0.2/pthost.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-28 10:22:53.000000 pthost-1.0.2/pthost.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       46 2024-05-28 10:22:53.000000 pthost-1.0.2/pthost.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       28 2024-05-28 10:22:53.000000 pthost-1.0.2/pthost.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        7 2024-05-28 10:22:53.000000 pthost-1.0.2/pthost.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-28 10:22:53.262071 pthost-1.0.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1277 2024-05-09 21:17:27.000000 pthost-1.0.2/setup.py
```

### Comparing `pthost-1.0.1/LICENSE` & `pthost-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pthost-1.0.1/PKG-INFO` & `pthost-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,34 @@
 Metadata-Version: 2.1
 Name: pthost
-Version: 1.0.1
+Version: 1.0.2
 Summary: Default vhost tester
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/pthost
 Project-URL: tracker, https://github.com/penterep/pthost/issues
-Project-URL: changelog, https://github.com/penterep/pthost/CHANGELOG.md/blob/main/CHANGELOG.md
+Project-URL: changelog, https://github.com/penterep/pthost/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ptlibs<2,>=1.0.7
 Requires-Dist: tldextract
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# pthost
-Default vhost testing tool
-
-pthost is a script for testing the default vhost on a target server and checks for various vulnerabilities via the Host HTTP header. It includes options to test for:
-
-- default-vhost: Tests the default virtual host configuration.
-- open-redirect: Checks for vulnerabilities that allow open redirects.
-- crlf: Tests for CRLF injection.
-- host-injection: Looks for Host header injection issues.
-- redir-to-https: Tests redirection from HTTP to HTTPS.
-- seo-fragmentation: Evaluates SEO fragmentation vulnerabilities.
-- subdomain-reflection-www: Tests subdomain reflection including 'www'.
-- subdomain-reflection-no-www: Checks subdomain reflection excluding 'www'.
-
+## PTHOST - Default vhost testing tool
 
 ## Installation
 ```
 pip install pthost
 ```
 
 ## Adding to PATH
@@ -95,14 +82,15 @@
 ```
 
 ## Dependencies
 
 ```
 ptlibs
 validators
+tldextract
 ```
 
 
 ## License
 
 Copyright (c) 2024 Penterep Security s.r.o.
```

### Comparing `pthost-1.0.1/README.md` & `pthost-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# pthost
-Default vhost testing tool
-
-pthost is a script for testing the default vhost on a target server and checks for various vulnerabilities via the Host HTTP header. It includes options to test for:
-
-- default-vhost: Tests the default virtual host configuration.
-- open-redirect: Checks for vulnerabilities that allow open redirects.
-- crlf: Tests for CRLF injection.
-- host-injection: Looks for Host header injection issues.
-- redir-to-https: Tests redirection from HTTP to HTTPS.
-- seo-fragmentation: Evaluates SEO fragmentation vulnerabilities.
-- subdomain-reflection-www: Tests subdomain reflection including 'www'.
-- subdomain-reflection-no-www: Checks subdomain reflection excluding 'www'.
-
+## PTHOST - Default vhost testing tool
 
 ## Installation
 ```
 pip install pthost
 ```
 
 ## Adding to PATH
@@ -72,14 +59,15 @@
 ```
 
 ## Dependencies
 
 ```
 ptlibs
 validators
+tldextract
 ```
 
 
 ## License
 
 Copyright (c) 2024 Penterep Security s.r.o.
```

### Comparing `pthost-1.0.1/pthost/modules/__pycache__/results.cpython-311.pyc` & `pthost-1.0.2/pthost/modules/__pycache__/results.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pthost-1.0.1/pthost/modules/__pycache__/scanner.cpython-311.pyc` & `pthost-1.0.2/pthost/modules/__pycache__/scanner.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pthost-1.0.1/pthost/modules/__pycache__/vuln_tester.cpython-311.pyc` & `pthost-1.0.2/pthost/modules/__pycache__/vuln_tester.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pthost-1.0.1/pthost/modules/scanner.py` & `pthost-1.0.2/pthost/modules/scanner.py`

 * *Files identical despite different names*

### Comparing `pthost-1.0.1/pthost/pthost.py` & `pthost-1.0.2/pthost/pthost.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import tldextract
 import requests
 import validators
 
 from modules.scanner import VulnerabilityTester
 
 from _version import __version__
-from ptlibs import ptjsonlib, ptmisclib, ptprinthelper, ptnethelper, tldparser
+from ptlibs import ptjsonlib, ptmisclib, ptprinthelper, ptnethelper
 
 
 class PtHost:
     def __init__(self, args):
         self.ptjsonlib      = ptjsonlib.PtJsonLib()
         self.test           = self._load_tests(args.test)
         self.scanner    = VulnerabilityTester(args, self.ptjsonlib, self.test)
@@ -107,15 +107,14 @@
                         incorporating the provided protocol.
 
         Example:
         - If `domain` is "example.com" and `protocol` is "https", this function
         might return ("93.184.216.34", "https://example.com", "https://www.example.com/").
         """
 
-        #extract = tldparser.parse(domain)
         extract = tldextract.extract(domain)
         if validators.ipv4(extract.domain): # if <extract.domain> is ipv4 address
             base_url   = f"{protocol}://{extract.domain}"
             full_url   = f"{protocol}://{extract.domain}"
             target_ip  = extract.domain
         else:
             base_url   = f"{protocol}://{'.'.join((extract.domain, extract.suffix))}"
@@ -187,17 +186,22 @@
     parser.add_argument("-a", "--user-agent",  type=str, default="Penterep Tools")
     parser.add_argument("-T",  "--timeout",    type=int, default=7)
     parser.add_argument("-H",  "--headers",    type=ptmisclib.pairs, nargs="+")
     parser.add_argument("-C",  "--cache",      action="store_true")
     parser.add_argument("-j",  "--json",       action="store_true")
     parser.add_argument("-v",  "--version",    action="version", version=f"%(prog)s {__version__}")
 
+    parser.add_argument("--socket-address",          type=str, default=None)
+    parser.add_argument("--socket-port",             type=str, default=None)
+    parser.add_argument("--process-ident",           type=str, default=None)
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

### Comparing `pthost-1.0.1/pthost.egg-info/PKG-INFO` & `pthost-1.0.2/pthost.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,34 @@
 Metadata-Version: 2.1
 Name: pthost
-Version: 1.0.1
+Version: 1.0.2
 Summary: Default vhost tester
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/pthost
 Project-URL: tracker, https://github.com/penterep/pthost/issues
-Project-URL: changelog, https://github.com/penterep/pthost/CHANGELOG.md/blob/main/CHANGELOG.md
+Project-URL: changelog, https://github.com/penterep/pthost/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ptlibs<2,>=1.0.7
 Requires-Dist: tldextract
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# pthost
-Default vhost testing tool
-
-pthost is a script for testing the default vhost on a target server and checks for various vulnerabilities via the Host HTTP header. It includes options to test for:
-
-- default-vhost: Tests the default virtual host configuration.
-- open-redirect: Checks for vulnerabilities that allow open redirects.
-- crlf: Tests for CRLF injection.
-- host-injection: Looks for Host header injection issues.
-- redir-to-https: Tests redirection from HTTP to HTTPS.
-- seo-fragmentation: Evaluates SEO fragmentation vulnerabilities.
-- subdomain-reflection-www: Tests subdomain reflection including 'www'.
-- subdomain-reflection-no-www: Checks subdomain reflection excluding 'www'.
-
+## PTHOST - Default vhost testing tool
 
 ## Installation
 ```
 pip install pthost
 ```
 
 ## Adding to PATH
@@ -95,14 +82,15 @@
 ```
 
 ## Dependencies
 
 ```
 ptlibs
 validators
+tldextract
 ```
 
 
 ## License
 
 Copyright (c) 2024 Penterep Security s.r.o.
```

### Comparing `pthost-1.0.1/setup.py` & `pthost-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     include_package_data= True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls = {
         "homepage":   "https://www.penterep.com/",
         "repository": "https://github.com/penterep/pthost",
         "tracker":    "https://github.com/penterep/pthost/issues",
-        "changelog":  "https://github.com/penterep/pthost/CHANGELOG.md/blob/main/CHANGELOG.md",
+        "changelog":  "https://github.com/penterep/pthost/blob/main/CHANGELOG.md",
     }
 )
```

