# Comparing `tmp/pyobjc-framework-VideoSubscriberAccount-9.1b1.tar.gz` & `tmp/pyobjc-framework-VideoSubscriberAccount-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-VideoSubscriberAccount-9.1b1.tar", last modified: Sun Mar 26 11:43:23 2023, max compression
+gzip compressed data, was "pyobjc-framework-VideoSubscriberAccount-9.2.tar", last modified: Wed Jun  7 00:31:09 2023, max compression
```

## Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1.tar` & `pyobjc-framework-VideoSubscriberAccount-9.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:23.571022 pyobjc-framework-VideoSubscriberAccount-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:23.523141 pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:23.534626 pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/VideoSubscriberAccount/
--rw-r--r--   0 ronald     (501) staff       (20)      809 2020-11-30 18:45:15.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/VideoSubscriberAccount/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     6069 2023-02-19 10:50:37.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/VideoSubscriberAccount/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:23.538957 pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2160 2023-03-26 11:43:23.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1087 2023-03-26 11:43:23.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:43:23.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:57.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:43:23.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       23 2023-03-26 11:43:23.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1949 2023-03-26 11:43:23.570542 pyobjc-framework-VideoSubscriberAccount-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:23.545658 pyobjc-framework-VideoSubscriberAccount-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      610 2022-10-18 09:53:23.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/PyObjCTest/test_VSSubscription.py
--rw-r--r--   0 ronald     (501) staff       (20)      228 2022-04-11 08:03:15.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/PyObjCTest/test_videosubscriberaccount.py
--rw-r--r--   0 ronald     (501) staff       (20)     1442 2022-02-24 08:47:17.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/PyObjCTest/test_videosubscriberaccounterrors.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:23.547104 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      275 2020-11-30 18:45:15.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/VideoSubscriberAccount.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      126 2022-06-15 11:57:00.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:23.568814 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    24686 2021-07-30 09:00:38.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    24857 2022-02-24 08:47:17.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36221 2022-10-18 09:53:23.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36418 2023-02-19 10:50:37.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21597 2020-11-30 18:45:15.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22191 2021-03-21 10:08:23.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    24687 2021-07-30 09:00:38.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    24858 2022-02-24 08:47:17.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36222 2022-10-18 09:53:23.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36419 2023-02-19 10:50:37.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:43:23.571132 pyobjc-framework-VideoSubscriberAccount-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      717 2023-03-25 14:20:32.000000 pyobjc-framework-VideoSubscriberAccount-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:09.122273 pyobjc-framework-VideoSubscriberAccount-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:09.092797 pyobjc-framework-VideoSubscriberAccount-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:09.097316 pyobjc-framework-VideoSubscriberAccount-9.2/Lib/VideoSubscriberAccount/
+-rw-r--r--   0 ronald     (501) staff       (20)      809 2020-11-30 18:45:15.000000 pyobjc-framework-VideoSubscriberAccount-9.2/Lib/VideoSubscriberAccount/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6069 2023-02-19 10:50:37.000000 pyobjc-framework-VideoSubscriberAccount-9.2/Lib/VideoSubscriberAccount/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:09.100364 pyobjc-framework-VideoSubscriberAccount-9.2/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2158 2023-06-07 00:31:09.000000 pyobjc-framework-VideoSubscriberAccount-9.2/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1102 2023-06-07 00:31:09.000000 pyobjc-framework-VideoSubscriberAccount-9.2/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:31:09.000000 pyobjc-framework-VideoSubscriberAccount-9.2/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:57.000000 pyobjc-framework-VideoSubscriberAccount-9.2/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:31:09.000000 pyobjc-framework-VideoSubscriberAccount-9.2/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       23 2023-06-07 00:31:09.000000 pyobjc-framework-VideoSubscriberAccount-9.2/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-VideoSubscriberAccount-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-VideoSubscriberAccount-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1947 2023-06-07 00:31:09.121861 pyobjc-framework-VideoSubscriberAccount-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:09.106185 pyobjc-framework-VideoSubscriberAccount-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-VideoSubscriberAccount-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      610 2022-10-18 09:53:23.000000 pyobjc-framework-VideoSubscriberAccount-9.2/PyObjCTest/test_VSSubscription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      228 2022-04-11 08:03:15.000000 pyobjc-framework-VideoSubscriberAccount-9.2/PyObjCTest/test_videosubscriberaccount.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1442 2022-02-24 08:47:17.000000 pyobjc-framework-VideoSubscriberAccount-9.2/PyObjCTest/test_videosubscriberaccounterrors.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:09.107656 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      275 2020-11-30 18:45:15.000000 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/VideoSubscriberAccount.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      126 2022-06-15 11:57:00.000000 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:09.120452 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    24686 2021-07-30 09:00:38.000000 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    24857 2022-02-24 08:47:17.000000 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36221 2022-10-18 09:53:23.000000 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36418 2023-02-19 10:50:37.000000 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21597 2020-11-30 18:45:15.000000 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22191 2021-03-21 10:08:23.000000 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    24687 2021-07-30 09:00:38.000000 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    24858 2022-02-24 08:47:17.000000 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36222 2022-10-18 09:53:23.000000 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36419 2023-02-19 10:50:37.000000 pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-VideoSubscriberAccount-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-VideoSubscriberAccount-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:31:09.122368 pyobjc-framework-VideoSubscriberAccount-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      799 2023-05-29 10:07:47.000000 pyobjc-framework-VideoSubscriberAccount-9.2/setup.py
```

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/VideoSubscriberAccount/__init__.py` & `pyobjc-framework-VideoSubscriberAccount-9.2/Lib/VideoSubscriberAccount/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/VideoSubscriberAccount/_metadata.py` & `pyobjc-framework-VideoSubscriberAccount-9.2/Lib/VideoSubscriberAccount/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/PKG-INFO` & `pyobjc-framework-VideoSubscriberAccount-9.2/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-VideoSubscriberAccount
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework VideoSubscriberAccount on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,VideoSubscriberAccount
 Platform: MacOS X (>=10.14)
```

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/SOURCES.txt` & `pyobjc-framework-VideoSubscriberAccount-9.2/Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/VideoSubscriberAccount/__init__.py
 Lib/VideoSubscriberAccount/_metadata.py
 Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/PKG-INFO
 Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/SOURCES.txt
 Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/dependency_links.txt
 Lib/pyobjc_framework_VideoSubscriberAccount.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/License.txt` & `pyobjc-framework-VideoSubscriberAccount-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/PKG-INFO` & `pyobjc-framework-VideoSubscriberAccount-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-VideoSubscriberAccount
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework VideoSubscriberAccount on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,VideoSubscriberAccount
 Platform: MacOS X (>=10.14)
```

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/PyObjCTest/test_VSSubscription.py` & `pyobjc-framework-VideoSubscriberAccount-9.2/PyObjCTest/test_VSSubscription.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/PyObjCTest/test_videosubscriberaccounterrors.py` & `pyobjc-framework-VideoSubscriberAccount-9.2/PyObjCTest/test_videosubscriberaccounterrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-VideoSubscriberAccount-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoSubscriberAccount-9.1b1/pyobjc_setup.py` & `pyobjc-framework-VideoSubscriberAccount-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

