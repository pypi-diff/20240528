# Comparing `tmp/grain_zip_deployer-2025.5.28.0.tar.gz` & `tmp/grain_zip_deployer-2025.5.28.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grain_zip_deployer-2025.5.28.0.tar", last modified: Tue May 28 13:49:30 2024, max compression
+gzip compressed data, was "grain_zip_deployer-2025.5.28.1.tar", last modified: Tue May 28 14:02:37 2024, max compression
```

## Comparing `grain_zip_deployer-2025.5.28.0.tar` & `grain_zip_deployer-2025.5.28.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 13:49:30.396088 grain_zip_deployer-2025.5.28.0/
--rw-rw-rw-   0        0        0      304 2024-05-28 13:49:30.395085 grain_zip_deployer-2025.5.28.0/PKG-INFO
--rw-rw-rw-   0        0        0     6419 2024-05-28 11:50:17.000000 grain_zip_deployer-2025.5.28.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 13:49:30.381800 grain_zip_deployer-2025.5.28.0/grain_zip_deployer/
--rw-rw-rw-   0        0        0        0 2024-05-28 13:17:17.000000 grain_zip_deployer-2025.5.28.0/grain_zip_deployer/__init__.py
--rw-rw-rw-   0        0        0     4825 2024-05-28 13:47:05.000000 grain_zip_deployer-2025.5.28.0/grain_zip_deployer/main.py
--rw-rw-rw-   0        0        0       44 2024-05-28 11:55:32.000000 grain_zip_deployer-2025.5.28.0/grain_zip_deployer/settings.py
--rw-rw-rw-   0        0        0       27 2024-05-28 13:13:37.000000 grain_zip_deployer-2025.5.28.0/grain_zip_deployer/version.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:49:30.395085 grain_zip_deployer-2025.5.28.0/grain_zip_deployer.egg-info/
--rw-rw-rw-   0        0        0      304 2024-05-28 13:49:30.000000 grain_zip_deployer-2025.5.28.0/grain_zip_deployer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-05-28 13:49:30.000000 grain_zip_deployer-2025.5.28.0/grain_zip_deployer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 13:49:30.000000 grain_zip_deployer-2025.5.28.0/grain_zip_deployer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-28 13:49:30.000000 grain_zip_deployer-2025.5.28.0/grain_zip_deployer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-05-28 13:49:30.000000 grain_zip_deployer-2025.5.28.0/grain_zip_deployer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-28 13:49:30.000000 grain_zip_deployer-2025.5.28.0/grain_zip_deployer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 13:49:30.397087 grain_zip_deployer-2025.5.28.0/setup.cfg
--rw-rw-rw-   0        0        0     1122 2024-05-28 13:42:36.000000 grain_zip_deployer-2025.5.28.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:02:37.122742 grain_zip_deployer-2025.5.28.1/
+-rw-rw-rw-   0        0        0      304 2024-05-28 14:02:37.122742 grain_zip_deployer-2025.5.28.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6419 2024-05-28 11:50:17.000000 grain_zip_deployer-2025.5.28.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 14:02:37.105455 grain_zip_deployer-2025.5.28.1/grain_zip_deployer/
+-rw-rw-rw-   0        0        0        0 2024-05-28 13:17:17.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer/__init__.py
+-rw-rw-rw-   0        0        0     4812 2024-05-28 14:01:48.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer/main.py
+-rw-rw-rw-   0        0        0       44 2024-05-28 11:55:32.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer/settings.py
+-rw-rw-rw-   0        0        0       27 2024-05-28 14:02:06.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer/version.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:02:37.122742 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-05-28 14:02:37.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-28 14:02:37.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 14:02:37.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-28 14:02:37.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-05-28 14:02:37.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-28 14:02:37.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 14:02:37.122742 grain_zip_deployer-2025.5.28.1/setup.cfg
+-rw-rw-rw-   0        0        0     1122 2024-05-28 13:42:36.000000 grain_zip_deployer-2025.5.28.1/setup.py
```

### Comparing `grain_zip_deployer-2025.5.28.0/README.md` & `grain_zip_deployer-2025.5.28.1/README.md`

 * *Files identical despite different names*

### Comparing `grain_zip_deployer-2025.5.28.0/grain_zip_deployer/main.py` & `grain_zip_deployer-2025.5.28.1/grain_zip_deployer/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import os
 from io import BytesIO
 import subprocess
 from grain_zip_deployer import settings
 import argparse
 import fnmatch
 
-from pathlib import PurePosixPath, Path, PurePath
+from pathlib import Path, PurePath
 
 # Determine the appropriate path class based on the operating system
 if os.name == 'nt':  # Windows
     from pathlib import WindowsPath as AppropriatePath
 else:  # Non-Windows (Linux, macOS, etc.)
     AppropriatePath = PurePath
 
 from google.cloud import storage
-from google.auth.credentials import Credentials
+from google.oauth2.credentials import Credentials
 
 
 __VERSION__ = 0.1
 
 def init_argparse():
 
     parser = argparse.ArgumentParser(
```

### Comparing `grain_zip_deployer-2025.5.28.0/setup.py` & `grain_zip_deployer-2025.5.28.1/setup.py`

 * *Files identical despite different names*

