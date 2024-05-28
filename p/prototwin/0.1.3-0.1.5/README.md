# Comparing `tmp/prototwin-0.1.3.tar.gz` & `tmp/prototwin-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prototwin-0.1.3.tar", last modified: Fri May 24 02:41:17 2024, max compression
+gzip compressed data, was "prototwin-0.1.5.tar", last modified: Tue May 28 19:06:25 2024, max compression
```

## Comparing `prototwin-0.1.3.tar` & `prototwin-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:41:17.168783 prototwin-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-24 02:41:09.000000 prototwin-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-24 02:41:09.000000 prototwin-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-24 02:41:17.168783 prototwin-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-24 02:41:09.000000 prototwin-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:41:17.164783 prototwin-0.1.3/prototwin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-24 02:41:17.000000 prototwin-0.1.3/prototwin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-24 02:41:17.000000 prototwin-0.1.3/prototwin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:41:17.000000 prototwin-0.1.3/prototwin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-24 02:41:17.000000 prototwin-0.1.3/prototwin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:41:17.000000 prototwin-0.1.3/prototwin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-24 02:41:09.000000 prototwin-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-24 02:41:17.168783 prototwin-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-24 02:41:09.000000 prototwin-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:06:25.505689 prototwin-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-28 19:06:18.000000 prototwin-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 19:06:18.000000 prototwin-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-28 19:06:25.505689 prototwin-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-28 19:06:18.000000 prototwin-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:06:25.505689 prototwin-0.1.5/prototwin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-28 19:06:25.000000 prototwin-0.1.5/prototwin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-28 19:06:25.000000 prototwin-0.1.5/prototwin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:06:25.000000 prototwin-0.1.5/prototwin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 19:06:25.000000 prototwin-0.1.5/prototwin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:06:25.000000 prototwin-0.1.5/prototwin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-28 19:06:18.000000 prototwin-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 19:06:25.505689 prototwin-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-28 19:06:18.000000 prototwin-0.1.5/setup.py
```

### Comparing `prototwin-0.1.3/LICENSE.txt` & `prototwin-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prototwin-0.1.3/PKG-INFO` & `prototwin-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prototwin
-Version: 0.1.3
+Version: 0.1.5
 Summary: The official python client interface for ProtoTwin Connect.
 Home-page: https://prototwin.com
 Author: ProtoTwin
 License: MIT
 Keywords: Industrial Simulation,Physics,Machine Learning,Robotics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `prototwin-0.1.3/README.md` & `prototwin-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `prototwin-0.1.3/prototwin.egg-info/PKG-INFO` & `prototwin-0.1.5/prototwin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prototwin
-Version: 0.1.3
+Version: 0.1.5
 Summary: The official python client interface for ProtoTwin Connect.
 Home-page: https://prototwin.com
 Author: ProtoTwin
 License: MIT
 Keywords: Industrial Simulation,Physics,Machine Learning,Robotics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `prototwin-0.1.3/setup.py` & `prototwin-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name = "prototwin",
     packages = find_packages(include=["prototwin"]),
-    version = "0.1.3",
+    version = "0.1.5",
     license = "MIT",
     description = "The official python client interface for ProtoTwin Connect.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     author = "ProtoTwin",
     url = "https://prototwin.com",
     keywords = ["Industrial Simulation", "Physics", "Machine Learning", "Robotics"],
```

