# Comparing `tmp/ptnmap-0.0.2.tar.gz` & `tmp/ptnmap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptnmap-0.0.2.tar", last modified: Thu May  9 17:55:44 2024, max compression
+gzip compressed data, was "ptnmap-0.0.3.tar", last modified: Tue May 28 10:47:30 2024, max compression
```

## Comparing `ptnmap-0.0.2.tar` & `ptnmap-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:55:44.215688 ptnmap-0.0.2/
--rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:27:08.000000 ptnmap-0.0.2/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3277 2024-05-09 17:55:44.215688 ptnmap-0.0.2/PKG-INFO
--rwxr-xr-x   0 kali      (1000) kali      (1000)     2448 2024-04-29 08:27:08.000000 ptnmap-0.0.2/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:55:44.205688 ptnmap-0.0.2/ptnmap/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:27:08.000000 ptnmap-0.0.2/ptnmap/__init__.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)       21 2024-05-09 17:54:45.000000 ptnmap-0.0.2/ptnmap/_version.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:55:44.205688 ptnmap-0.0.2/ptnmap/modules/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:27:08.000000 ptnmap-0.0.2/ptnmap/modules/__init__.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     4796 2024-05-09 17:45:44.000000 ptnmap-0.0.2/ptnmap/modules/xml_parser.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     5491 2024-05-09 17:50:40.000000 ptnmap-0.0.2/ptnmap/ptnmap.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:55:44.215688 ptnmap-0.0.2/ptnmap.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3277 2024-05-09 17:55:44.000000 ptnmap-0.0.2/ptnmap.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      319 2024-05-09 17:55:44.000000 ptnmap-0.0.2/ptnmap.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 17:55:44.000000 ptnmap-0.0.2/ptnmap.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       46 2024-05-09 17:55:44.000000 ptnmap-0.0.2/ptnmap.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       28 2024-05-09 17:55:44.000000 ptnmap-0.0.2/ptnmap.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        7 2024-05-09 17:55:44.000000 ptnmap-0.0.2/ptnmap.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 17:55:44.215688 ptnmap-0.0.2/setup.cfg
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1261 2024-05-06 19:27:52.000000 ptnmap-0.0.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:47:30.041895 ptnmap-0.0.3/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:27:08.000000 ptnmap-0.0.3/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3277 2024-05-28 10:47:30.041895 ptnmap-0.0.3/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2448 2024-04-29 08:27:08.000000 ptnmap-0.0.3/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:47:30.041895 ptnmap-0.0.3/ptnmap/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:27:08.000000 ptnmap-0.0.3/ptnmap/__init__.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)       21 2024-05-28 10:44:27.000000 ptnmap-0.0.3/ptnmap/_version.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:47:30.041895 ptnmap-0.0.3/ptnmap/modules/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:27:08.000000 ptnmap-0.0.3/ptnmap/modules/__init__.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     4803 2024-05-28 08:09:20.000000 ptnmap-0.0.3/ptnmap/modules/xml_parser.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     5725 2024-05-28 09:32:52.000000 ptnmap-0.0.3/ptnmap/ptnmap.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:47:30.041895 ptnmap-0.0.3/ptnmap.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3277 2024-05-28 10:47:30.000000 ptnmap-0.0.3/ptnmap.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      319 2024-05-28 10:47:30.000000 ptnmap-0.0.3/ptnmap.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-28 10:47:30.000000 ptnmap-0.0.3/ptnmap.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       46 2024-05-28 10:47:30.000000 ptnmap-0.0.3/ptnmap.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       28 2024-05-28 10:47:30.000000 ptnmap-0.0.3/ptnmap.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        7 2024-05-28 10:47:30.000000 ptnmap-0.0.3/ptnmap.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-28 10:47:30.041895 ptnmap-0.0.3/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1261 2024-05-06 19:27:52.000000 ptnmap-0.0.3/setup.py
```

### Comparing `ptnmap-0.0.2/LICENSE` & `ptnmap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ptnmap-0.0.2/PKG-INFO` & `ptnmap-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptnmap
-Version: 0.0.2
+Version: 0.0.3
 Summary: ptnmap
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptnmap
```

### Comparing `ptnmap-0.0.2/README.md` & `ptnmap-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ptnmap-0.0.2/ptnmap/modules/xml_parser.py` & `ptnmap-0.0.3/ptnmap/modules/xml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,19 @@
 
         for index, osmatch in enumerate(self.root.find("host").find("os").findall("osmatch")):
             osmatch_name = osmatch.get("name")
             osmatch_accuracy = osmatch.get("accuracy")
             result_string += f"{osmatch_name} ({osmatch_accuracy}%)"
 
             if int(osmatch_accuracy) > 90 and not self.ptjsonlib.json_object["results"]["properties"].get("vendor") and osmatch.find("osclass").get("vendor") is not None:
-                self.ptjsonlib.add_property("os", osmatch.find("osclass").get("vendor"))
+                self.ptjsonlib.add_properties({"os": osmatch.find("osclass").get("vendor")})
             if index+1 != len(self.root.find("host").find("os").findall("osmatch")):
                 result_string += ", "
 
-        self.ptjsonlib.add_property("description", "Nmap: "+ result_string)
-
+        self.ptjsonlib.add_properties({"description": "Nmap: " + result_string})
 
     def get_live_hosts(self):
         """Get result from live host scan"""
         for host in self.root.findall("host"):
             props = dict()
 
             for address in host.findall("address"):
```

### Comparing `ptnmap-0.0.2/ptnmap/ptnmap.py` & `ptnmap-0.0.3/ptnmap/ptnmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,14 +108,17 @@
     exclusive.add_argument("-sS", "--scan-port-syn",     action="store_true")
     exclusive.add_argument("-sT", "--scan-port-connect", action="store_true")
     parser.add_argument("-t",  "--target",       type=str)
     parser.add_argument("-p",  "--port",         type=str)
     parser.add_argument("-j",  "--json",         action="store_true", default=True)
     parser.add_argument("-v",  "--version",      action="version", version=f"{SCRIPTNAME} {__version__}")
 
+    parser.add_argument("--socket-address",          type=str, default=None)
+    parser.add_argument("--socket-port",             type=str, default=None)
+    parser.add_argument("--process-ident",           type=str, default=None)
 
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
         ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
     args = parser.parse_args()
     ptprinthelper.print_banner(SCRIPTNAME, __version__, args.json)
     return args
```

### Comparing `ptnmap-0.0.2/ptnmap.egg-info/PKG-INFO` & `ptnmap-0.0.3/ptnmap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptnmap
-Version: 0.0.2
+Version: 0.0.3
 Summary: ptnmap
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptnmap
```

### Comparing `ptnmap-0.0.2/setup.py` & `ptnmap-0.0.3/setup.py`

 * *Files identical despite different names*

