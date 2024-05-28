# Comparing `tmp/nimbus_splash-1.5.0.tar.gz` & `tmp/nimbus_splash-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimbus splash-1.5.0.tar", last modified: Mon Apr 22 16:32:08 2024, max compression
+gzip compressed data, was "nimbus splash-1.6.0.tar", last modified: Tue May 28 13:28:23 2024, max compression
```

## Comparing `nimbus_splash-1.5.0.tar` & `nimbus_splash-1.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:32:08.966194 nimbus splash-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 16:31:57.000000 nimbus splash-1.5.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:32:08.966194 nimbus splash-1.5.0/Nimbus_Splash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-22 16:32:08.000000 nimbus splash-1.5.0/Nimbus_Splash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-22 16:32:08.000000 nimbus splash-1.5.0/Nimbus_Splash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:32:08.000000 nimbus splash-1.5.0/Nimbus_Splash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 16:32:08.000000 nimbus splash-1.5.0/Nimbus_Splash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 16:32:08.000000 nimbus splash-1.5.0/Nimbus_Splash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 16:32:08.000000 nimbus splash-1.5.0/Nimbus_Splash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-22 16:32:08.966194 nimbus splash-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-22 16:31:57.000000 nimbus splash-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:32:08.966194 nimbus splash-1.5.0/nimbus_splash/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 16:31:57.000000 nimbus splash-1.5.0/nimbus_splash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 16:31:58.000000 nimbus splash-1.5.0/nimbus_splash/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9500 2024-04-22 16:31:57.000000 nimbus splash-1.5.0/nimbus_splash/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    14971 2024-04-22 16:31:57.000000 nimbus splash-1.5.0/nimbus_splash/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-22 16:31:57.000000 nimbus splash-1.5.0/nimbus_splash/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-22 16:31:57.000000 nimbus splash-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:32:08.966194 nimbus splash-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-22 16:31:58.000000 nimbus splash-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:28:23.837432 nimbus splash-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 13:28:11.000000 nimbus splash-1.6.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:28:23.837432 nimbus splash-1.6.0/Nimbus_Splash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-28 13:28:23.000000 nimbus splash-1.6.0/Nimbus_Splash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-28 13:28:23.000000 nimbus splash-1.6.0/Nimbus_Splash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:28:23.000000 nimbus splash-1.6.0/Nimbus_Splash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-28 13:28:23.000000 nimbus splash-1.6.0/Nimbus_Splash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 13:28:23.000000 nimbus splash-1.6.0/Nimbus_Splash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 13:28:23.000000 nimbus splash-1.6.0/Nimbus_Splash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-28 13:28:23.837432 nimbus splash-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-28 13:28:11.000000 nimbus splash-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:28:23.837432 nimbus splash-1.6.0/nimbus_splash/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-28 13:28:11.000000 nimbus splash-1.6.0/nimbus_splash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 13:28:12.000000 nimbus splash-1.6.0/nimbus_splash/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9500 2024-05-28 13:28:11.000000 nimbus splash-1.6.0/nimbus_splash/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14991 2024-05-28 13:28:11.000000 nimbus splash-1.6.0/nimbus_splash/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-28 13:28:11.000000 nimbus splash-1.6.0/nimbus_splash/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-28 13:28:11.000000 nimbus splash-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:28:23.837432 nimbus splash-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-28 13:28:12.000000 nimbus splash-1.6.0/setup.py
```

### Comparing `nimbus splash-1.5.0/LICENSE` & `nimbus splash-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nimbus splash-1.5.0/Nimbus_Splash.egg-info/PKG-INFO` & `nimbus splash-1.6.0/Nimbus_Splash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nimbus-Splash
-Version: 1.5.0
+Version: 1.6.0
 Summary: A package to make life easier when using the University of         Bath's cloud computing suite for Orca calculations.
 Home-page: https://github.com/jonkragskow/nimbus_splash
 Author: Jon Kragskow
 Author-email: jgck20@bath.ac.uk
 Project-URL: Bug Tracker, https://github.com/JonKragskow/nimbus_splash/issues
 Project-URL: Documentation, https://www.kragskow.dev/nimbus_splash/index.html
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nimbus splash-1.5.0/PKG-INFO` & `nimbus splash-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nimbus Splash
-Version: 1.5.0
+Version: 1.6.0
 Summary: A package to make life easier when using the University of         Bath's cloud computing suite for Orca calculations.
 Home-page: https://github.com/jonkragskow/nimbus_splash
 Author: Jon Kragskow
 Author-email: jgck20@bath.ac.uk
 Project-URL: Bug Tracker, https://github.com/JonKragskow/nimbus_splash/issues
 Project-URL: Documentation, https://www.kragskow.dev/nimbus_splash/index.html
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nimbus splash-1.5.0/README.md` & `nimbus splash-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nimbus splash-1.5.0/nimbus_splash/cli.py` & `nimbus splash-1.6.0/nimbus_splash/cli.py`

 * *Files identical despite different names*

### Comparing `nimbus splash-1.5.0/nimbus_splash/job.py` & `nimbus splash-1.6.0/nimbus_splash/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import subprocess
 
 from . import utils as ut
 
+ORCA_MODULE = 'ORCA/5.0.4'
+
 
 def write_file(input_file: str, node_type: str, time: str,
                dependency_paths: dict[str, str],
                verbose: bool = False,
                email: str = '') -> str:
     '''
     Writes slurm jobscript to file for ORCA calculation on nimbus
@@ -121,15 +123,15 @@
 
         j.write('# Module system setup\n')
         j.write('source /apps/build/easy_build/scripts/id_instance.sh\n')
         j.write('source /apps/build/easy_build/scripts/setup_modules.sh\n\n')
 
         j.write('# Load orca\n')
         j.write('module purge\n')
-        j.write('module load ORCA/5.0.1-gompi-2021a\n\n')
+        j.write(f'module load {ORCA_MODULE}\n\n')
 
         j.write('# UCX transport protocols for MPI\n')
         j.write('export UCX_TLS=self,tcp,sm\n\n')
 
         j.write('# If timeout, evicted, cancelled, then manually end orca\n')
 
         j.write("trap 'echo signal recieved in BATCH!; kill -15 ")
```

### Comparing `nimbus splash-1.5.0/nimbus_splash/utils.py` & `nimbus splash-1.6.0/nimbus_splash/utils.py`

 * *Files identical despite different names*

### Comparing `nimbus splash-1.5.0/pyproject.toml` & `nimbus splash-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nimbus splash-1.5.0/setup.py` & `nimbus splash-1.6.0/setup.py`

 * *Files identical despite different names*

```diff
@@ -8,15 +8,15 @@
 calculations.\n\n
 
 Please see the `nimbus_splash` documentation for more details.
 '''
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 
 setuptools.setup(
     name="Nimbus Splash",
     version=__version__,
     author="Jon Kragskow",
     author_email="jgck20@bath.ac.uk",
     description="A package to make life easier when using the University of \
```

