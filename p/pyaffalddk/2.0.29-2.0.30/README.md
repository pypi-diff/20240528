# Comparing `tmp/pyaffalddk-2.0.29.tar.gz` & `tmp/pyaffalddk-2.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaffalddk-2.0.29.tar", last modified: Sun May 12 15:51:29 2024, max compression
+gzip compressed data, was "pyaffalddk-2.0.30.tar", last modified: Tue May 28 09:41:24 2024, max compression
```

## Comparing `pyaffalddk-2.0.29.tar` & `pyaffalddk-2.0.30.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:51:29.710151 pyaffalddk-2.0.29/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-12 15:51:29.710151 pyaffalddk-2.0.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:51:29.710151 pyaffalddk-2.0.29/pyaffalddk/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/pyaffalddk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/pyaffalddk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/pyaffalddk/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/pyaffalddk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/pyaffalddk/images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:51:29.710151 pyaffalddk-2.0.29/pyaffalddk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-12 15:51:29.000000 pyaffalddk-2.0.29/pyaffalddk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-12 15:51:29.000000 pyaffalddk-2.0.29/pyaffalddk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 15:51:29.000000 pyaffalddk-2.0.29/pyaffalddk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-12 15:51:29.000000 pyaffalddk-2.0.29/pyaffalddk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 15:51:29.710151 pyaffalddk-2.0.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 15:51:26.000000 pyaffalddk-2.0.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:41:24.818634 pyaffalddk-2.0.30/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 09:41:20.000000 pyaffalddk-2.0.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-28 09:41:24.818634 pyaffalddk-2.0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-28 09:41:20.000000 pyaffalddk-2.0.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:41:24.818634 pyaffalddk-2.0.30/pyaffalddk/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-28 09:41:20.000000 pyaffalddk-2.0.30/pyaffalddk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-05-28 09:41:20.000000 pyaffalddk-2.0.30/pyaffalddk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-05-28 09:41:20.000000 pyaffalddk-2.0.30/pyaffalddk/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-28 09:41:20.000000 pyaffalddk-2.0.30/pyaffalddk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-28 09:41:20.000000 pyaffalddk-2.0.30/pyaffalddk/images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:41:24.818634 pyaffalddk-2.0.30/pyaffalddk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-28 09:41:24.000000 pyaffalddk-2.0.30/pyaffalddk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-28 09:41:24.000000 pyaffalddk-2.0.30/pyaffalddk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:41:24.000000 pyaffalddk-2.0.30/pyaffalddk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 09:41:24.000000 pyaffalddk-2.0.30/pyaffalddk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:41:24.818634 pyaffalddk-2.0.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-28 09:41:20.000000 pyaffalddk-2.0.30/setup.py
```

### Comparing `pyaffalddk-2.0.29/LICENSE` & `pyaffalddk-2.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.29/PKG-INFO` & `pyaffalddk-2.0.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.29
+Version: 2.0.30
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.29/pyaffalddk/__init__.py` & `pyaffalddk-2.0.30/pyaffalddk/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     AffaldDKNoConnection,
 )
 from pyaffalddk.data import PickupEvents, PickupType, AffaldDKAddressInfo
 
 from pyaffalddk.const import ICON_LIST, MUNICIPALITIES_ARRAY, NAME_ARRAY, NAME_LIST, WEEKDAYS, WEEKDAYS_SHORT
 
 __title__ = "pyaffalddk"
-__version__ = "2.0.29"
+__version__ = "2.0.30"
 __author__ = "briis"
 __license__ = "MIT"
```

### Comparing `pyaffalddk-2.0.29/pyaffalddk/api.py` & `pyaffalddk-2.0.30/pyaffalddk/api.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.29/pyaffalddk/const.py` & `pyaffalddk-2.0.30/pyaffalddk/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "pappi": [
         "Plast MDK og papir",
         "PAPPI",
         "Plast/MD-karton/PP",
         "Plast/Papir",
         "Papir/Plast og kartoner",
         "Plast og Mad- & drikkekartoner/Papir",
-        "Plast, Metal, MDK",
+        "Plast, Mad- og drikkekartoner, Småt Pap og Papir",
     ],
     "farligtaffald": [
         "Farligt affald",
         "Miljøkasser",
         "Farligt Affald, Rød boks",
         "Genbrugsbilen",
     ],
@@ -95,14 +95,15 @@
     "plastmetal": [
         "Plast & Metal",
         "Plast, metal & MDK 660L",
         "Plast/ Metal",
         "Plast/MDK/Metal",
         "Plast-metal",
         "Plast/Metal",
+        "Plast, Metal, MDK",
     ],
     "restaffald": ["",],
     "storskrald": [
         "Storskrald",
         "Stort elektronik",
         "Storskrald og genbrug",
         "Pap og Storskrald",
```

### Comparing `pyaffalddk-2.0.29/pyaffalddk/data.py` & `pyaffalddk-2.0.30/pyaffalddk/data.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.29/pyaffalddk/images.py` & `pyaffalddk-2.0.30/pyaffalddk/images.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.29/pyaffalddk.egg-info/PKG-INFO` & `pyaffalddk-2.0.30/pyaffalddk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.29
+Version: 2.0.30
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.29/setup.py` & `pyaffalddk-2.0.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyaffalddk",
-    version="2.0.29",
+    version="2.0.30",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets garbage collection data from danish Municipalities",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pyaffalddk",
```

