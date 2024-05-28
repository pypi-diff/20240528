# Comparing `tmp/energyplus_python_apps-23.1b2.tar.gz` & `tmp/energyplus_python_apps-24.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_python_apps-23.1b2.tar", last modified: Fri Jun  2 22:12:23 2023, max compression
+gzip compressed data, was "energyplus_python_apps-24.1a1.tar", last modified: Tue May 28 16:03:04 2024, max compression
```

## Comparing `energyplus_python_apps-23.1b2.tar` & `energyplus_python_apps-24.1a1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:12:23.786191 energyplus_python_apps-23.1b2/
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-06-02 22:12:21.000000 energyplus_python_apps-23.1b2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-06-02 22:12:23.782191 energyplus_python_apps-23.1b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-06-02 22:12:21.000000 energyplus_python_apps-23.1b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:12:23.782191 energyplus_python_apps-23.1b2/energyplus_python_apps/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-02 22:12:21.000000 energyplus_python_apps-23.1b2/energyplus_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      763 2023-06-02 22:12:21.000000 energyplus_python_apps-23.1b2/energyplus_python_apps/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:12:23.782191 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-06-02 22:12:23.000000 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-02 22:12:23.000000 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 22:12:23.000000 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-02 22:12:23.000000 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-02 22:12:23.000000 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-02 22:12:23.000000 energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 22:12:23.786191 energyplus_python_apps-23.1b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1223 2023-06-02 22:12:21.000000 energyplus_python_apps-23.1b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:04.952142 energyplus_python_apps-24.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-28 16:03:02.000000 energyplus_python_apps-24.1a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-28 16:03:04.952142 energyplus_python_apps-24.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-28 16:03:02.000000 energyplus_python_apps-24.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:04.952142 energyplus_python_apps-24.1a1/energyplus_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 16:03:02.000000 energyplus_python_apps-24.1a1/energyplus_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-28 16:03:02.000000 energyplus_python_apps-24.1a1/energyplus_python_apps/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:03:04.952142 energyplus_python_apps-24.1a1/energyplus_python_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-28 16:03:04.000000 energyplus_python_apps-24.1a1/energyplus_python_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-28 16:03:04.000000 energyplus_python_apps-24.1a1/energyplus_python_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:03:04.000000 energyplus_python_apps-24.1a1/energyplus_python_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 16:03:04.000000 energyplus_python_apps-24.1a1/energyplus_python_apps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-28 16:03:04.000000 energyplus_python_apps-24.1a1/energyplus_python_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 16:03:04.000000 energyplus_python_apps-24.1a1/energyplus_python_apps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:03:04.952142 energyplus_python_apps-24.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-28 16:03:02.000000 energyplus_python_apps-24.1a1/setup.py
```

### Comparing `energyplus_python_apps-23.1b2/LICENSE.txt` & `energyplus_python_apps-24.1a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `energyplus_python_apps-23.1b2/PKG-INFO` & `energyplus_python_apps-24.1a1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_python_apps
-Version: 23.1b2
+Version: 24.1a1
 Summary: Meta-package collecting all official EnergyPlus Python utilities
 Home-page: https://github.com/Myoldmopar/EnergyPlusPythonApps
 Author: Edwin Lee, for NREL, for United States Department of Energy
 License: ModifiedBSD
 Description: # EnergyPlus Python Apps
         
         This is a meta-project which simply depends on all the EnergyPlus "Official" Python utilities.
@@ -29,14 +29,15 @@
         | energyplus-ruleset-model     | A utility for generating ruleset model reports from EnergyPlus inputs and outputs    | https://github.com/jasonglazer/createrulesetmodeldescription |
         | energyplus-transition-tools  | A lightweight interface for automatically transitioning EnergyPlus input files       | https://github.com/Myoldmopar/EnergyPlusTransitionTools      |
         | energyplus-pet               | A library and graphical tool for generating input coefficients for EnergyPlus models | https://github.com/Myoldmopar/energypluspet                  |
         | energyplus-idd-idf-utilities | A lightweight library for processing and querying idd and idf files                  | https://github.com/Myoldmopar/py-idd-idf                     |
         | energyplus-regressions       | A tool for comparing results from two EnergyPlus builds, for E+ developer usage      | https://github.com/NREL/EnergyPlusRegressionTool             |
         | energyplus-api-helpers       | A set of helper classes and demos for interacting with the EnergyPlus API            | https://github.com/Myoldmopar/EnergyPlusAPIHelper            |
         | energyplus-diff-analysis     | Tools for plotting and comparing csv data from two separate EnergyPlus runs          | https://github.com/mitchute/energyplus-diff-analysis         |
+        | energyplus-version           | Python-based version update classes and utilities                                    | https://github.com/mitchute/energyplus-version               |
         
         ## Usage
         
         Cover a few topics here:
          - Installation
          - Running the configuration script after install
          - Accessing all the tools, including the dev tools
```

### Comparing `energyplus_python_apps-23.1b2/README.md` & `energyplus_python_apps-24.1a1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 | energyplus-ruleset-model     | A utility for generating ruleset model reports from EnergyPlus inputs and outputs    | https://github.com/jasonglazer/createrulesetmodeldescription |
 | energyplus-transition-tools  | A lightweight interface for automatically transitioning EnergyPlus input files       | https://github.com/Myoldmopar/EnergyPlusTransitionTools      |
 | energyplus-pet               | A library and graphical tool for generating input coefficients for EnergyPlus models | https://github.com/Myoldmopar/energypluspet                  |
 | energyplus-idd-idf-utilities | A lightweight library for processing and querying idd and idf files                  | https://github.com/Myoldmopar/py-idd-idf                     |
 | energyplus-regressions       | A tool for comparing results from two EnergyPlus builds, for E+ developer usage      | https://github.com/NREL/EnergyPlusRegressionTool             |
 | energyplus-api-helpers       | A set of helper classes and demos for interacting with the EnergyPlus API            | https://github.com/Myoldmopar/EnergyPlusAPIHelper            |
 | energyplus-diff-analysis     | Tools for plotting and comparing csv data from two separate EnergyPlus runs          | https://github.com/mitchute/energyplus-diff-analysis         |
+| energyplus-version           | Python-based version update classes and utilities                                    | https://github.com/mitchute/energyplus-version               |
 
 ## Usage
 
 Cover a few topics here:
  - Installation
  - Running the configuration script after install
  - Accessing all the tools, including the dev tools
```

### Comparing `energyplus_python_apps-23.1b2/energyplus_python_apps/configure.py` & `energyplus_python_apps-24.1a1/energyplus_python_apps/configure.py`

 * *Files identical despite different names*

### Comparing `energyplus_python_apps-23.1b2/energyplus_python_apps.egg-info/PKG-INFO` & `energyplus_python_apps-24.1a1/energyplus_python_apps.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-python-apps
-Version: 23.1b2
+Version: 24.1a1
 Summary: Meta-package collecting all official EnergyPlus Python utilities
 Home-page: https://github.com/Myoldmopar/EnergyPlusPythonApps
 Author: Edwin Lee, for NREL, for United States Department of Energy
 License: ModifiedBSD
 Description: # EnergyPlus Python Apps
         
         This is a meta-project which simply depends on all the EnergyPlus "Official" Python utilities.
@@ -29,14 +29,15 @@
         | energyplus-ruleset-model     | A utility for generating ruleset model reports from EnergyPlus inputs and outputs    | https://github.com/jasonglazer/createrulesetmodeldescription |
         | energyplus-transition-tools  | A lightweight interface for automatically transitioning EnergyPlus input files       | https://github.com/Myoldmopar/EnergyPlusTransitionTools      |
         | energyplus-pet               | A library and graphical tool for generating input coefficients for EnergyPlus models | https://github.com/Myoldmopar/energypluspet                  |
         | energyplus-idd-idf-utilities | A lightweight library for processing and querying idd and idf files                  | https://github.com/Myoldmopar/py-idd-idf                     |
         | energyplus-regressions       | A tool for comparing results from two EnergyPlus builds, for E+ developer usage      | https://github.com/NREL/EnergyPlusRegressionTool             |
         | energyplus-api-helpers       | A set of helper classes and demos for interacting with the EnergyPlus API            | https://github.com/Myoldmopar/EnergyPlusAPIHelper            |
         | energyplus-diff-analysis     | Tools for plotting and comparing csv data from two separate EnergyPlus runs          | https://github.com/mitchute/energyplus-diff-analysis         |
+        | energyplus-version           | Python-based version update classes and utilities                                    | https://github.com/mitchute/energyplus-version               |
         
         ## Usage
         
         Cover a few topics here:
          - Installation
          - Running the configuration script after install
          - Accessing all the tools, including the dev tools
```

### Comparing `energyplus_python_apps-23.1b2/setup.py` & `energyplus_python_apps-24.1a1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         'energyplus-ruleset-model==0.5',
         'energyplus-transition-tools==2.0.8',
         'energyplus-pet==0.50',
         'energyplus-idd-idf-utilities==0.88',
         'energyplus-regressions==2.0.3',
         'energyplus-api-helpers==0.4',
         'energyplus-diff-analysis==0.2',
+        'energyplus-version==1.0.0'
         # 'energyplus-expand-objects==blah',
         # 'energyplus-epjson-editor==blah',
     ],
     entry_points={
         'console_scripts': [
             'energyplus_python_configure=energyplus_python_apps.configure:configure_cli',
         ]
```

