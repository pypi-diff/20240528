# Comparing `tmp/protai-0.7.0.tar.gz` & `tmp/protai-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protai-0.7.0.tar", last modified: Sun May 26 02:24:14 2024, max compression
+gzip compressed data, was "protai-0.7.1.tar", last modified: Tue May 28 14:27:04 2024, max compression
```

## Comparing `protai-0.7.0.tar` & `protai-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 02:24:14.044843 protai-0.7.0/
--rw-rw-rw-   0        0        0     1107 2024-05-23 18:18:24.000000 protai-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     4993 2024-05-26 02:24:14.043844 protai-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     4319 2024-05-26 01:15:37.000000 protai-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 02:24:14.030329 protai-0.7.0/protai/
--rw-rw-rw-   0        0        0        5 2024-05-26 01:52:02.000000 protai-0.7.0/protai/VERSION
--rw-rw-rw-   0        0        0       69 2024-05-23 18:18:24.000000 protai-0.7.0/protai/__init__.py
--rw-rw-rw-   0        0        0     4919 2024-05-25 22:43:02.000000 protai-0.7.0/protai/auth.py
--rw-rw-rw-   0        0        0     3388 2024-05-26 02:22:45.000000 protai-0.7.0/protai/protai.py
-drwxrwxrwx   0        0        0        0 2024-05-26 02:24:14.041843 protai-0.7.0/protai.egg-info/
--rw-rw-rw-   0        0        0     4993 2024-05-26 02:24:13.000000 protai-0.7.0/protai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-26 02:24:14.000000 protai-0.7.0/protai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 02:24:13.000000 protai-0.7.0/protai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-26 02:24:13.000000 protai-0.7.0/protai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2024-05-26 02:24:13.000000 protai-0.7.0/protai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 02:24:13.000000 protai-0.7.0/protai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 02:24:14.044843 protai-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     4178 2024-05-23 18:18:24.000000 protai-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:27:04.481591 protai-0.7.1/
+-rw-rw-rw-   0        0        0     1107 2024-05-23 18:18:24.000000 protai-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0     4993 2024-05-28 14:27:04.480591 protai-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4319 2024-05-26 01:15:37.000000 protai-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 14:27:04.471448 protai-0.7.1/protai/
+-rw-rw-rw-   0        0        0        5 2024-05-28 14:23:48.000000 protai-0.7.1/protai/VERSION
+-rw-rw-rw-   0        0        0      612 2024-05-28 14:21:45.000000 protai-0.7.1/protai/__init__.py
+-rw-rw-rw-   0        0        0     4919 2024-05-25 22:43:02.000000 protai-0.7.1/protai/auth.py
+-rw-rw-rw-   0        0        0     2971 2024-05-28 14:24:41.000000 protai-0.7.1/protai/protai.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:27:04.479591 protai-0.7.1/protai.egg-info/
+-rw-rw-rw-   0        0        0     4993 2024-05-28 14:27:04.000000 protai-0.7.1/protai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-28 14:27:04.000000 protai-0.7.1/protai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 14:27:04.000000 protai-0.7.1/protai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-28 14:27:04.000000 protai-0.7.1/protai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-05-28 14:27:04.000000 protai-0.7.1/protai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 14:27:04.000000 protai-0.7.1/protai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 14:27:04.481591 protai-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     4360 2024-05-28 14:23:28.000000 protai-0.7.1/setup.py
```

### Comparing `protai-0.7.0/LICENSE` & `protai-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `protai-0.7.0/PKG-INFO` & `protai-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protai
-Version: 0.7.0
+Version: 0.7.1
 Summary: A useful 0-Shot AI in the terminal
 Home-page: https://github.com/protik09/terminal-ai
 Author: Protik Banerji
 Author-email: protik09@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `protai-0.7.0/README.md` & `protai-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `protai-0.7.0/protai/auth.py` & `protai-0.7.1/protai/auth.py`

 * *Files identical despite different names*

### Comparing `protai-0.7.0/protai/protai.py` & `protai-0.7.1/protai/protai.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,33 +3,24 @@
 import os
 import argparse
 from rich import print
 from rich.markdown import Markdown
 from groq import Groq, GroqError
 from auth import authGroq, changeApiKey
 from yaspin import yaspin
+from protai import __version__  # Import the version
 
 
 # Set your GROQ API endpoint URL
 GROQ_API_URL = "https://api.groq.io/v1/query"
 
 
 def versionHandler() -> None:
     """Print the version number of ProtAI."""
-    # Get the absolute path of the current directory
-    current_directory = os.path.abspath(os.path.dirname(__file__))
-    # Construct the absolute path for the VERSION file
-    version_file_path = os.path.join(current_directory, "VERSION")
-    with open(version_file_path, "r") as f:
-        try:
-            ProtAI_VERSION = f.read().strip()
-            # print(ProtAI_VERSION)
-        except ValueError:
-            ProtAI_VERSION = "Invalid version number"
-    print(f"{ProtAI_VERSION}")
+    print(__version__)
     exitHandler(0)
 
 
 def exitHandler(exit_code: int) -> None:
     """TODO: Write more comprehensive exit handler when inspiration strikes."""
     sys.exit(exit_code)
```

### Comparing `protai-0.7.0/protai.egg-info/PKG-INFO` & `protai-0.7.1/protai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protai
-Version: 0.7.0
+Version: 0.7.1
 Summary: A useful 0-Shot AI in the terminal
 Home-page: https://github.com/protik09/terminal-ai
 Author: Protik Banerji
 Author-email: protik09@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `protai-0.7.0/setup.py` & `protai-0.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,21 +23,29 @@
 AUTHOR = "Protik Banerji"
 REQUIRES_PYTHON = ">=3.10.0"
 
 # Attempt to read the version from VERSION file
 version_file_path = os.path.join(
     os.path.abspath(os.path.dirname(__file__)), "protai", "VERSION"
 )
-try:
-    with open(version_file_path, "r") as version_file:
-        VERSION = version_file.read().strip()
-except FileNotFoundError:
-    VERSION = "0.0.0"  # Default version if VERSION file is not found
+default_version = "0.0.0"
 
 
+def read_version(version_file_path) -> str:
+    try:
+        with open(version_file_path, "r") as version_file:
+            return version_file.read().strip()
+    except FileNotFoundError:
+        return default_version  # Default version if not found
+    except Exception:
+        return default_version
+
+
+VERSION = read_version(version_file_path)
+
 # What packages are required for this module to be executed?
 REQUIRED = requirements
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

