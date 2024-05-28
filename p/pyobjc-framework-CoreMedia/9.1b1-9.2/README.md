# Comparing `tmp/pyobjc-framework-CoreMedia-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreMedia-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreMedia-9.1b1.tar", last modified: Sun Mar 26 11:21:16 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreMedia-9.2.tar", last modified: Wed Jun  7 00:11:15 2023, max compression
```

## Comparing `pyobjc-framework-CoreMedia-9.1b1.tar` & `pyobjc-framework-CoreMedia-9.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:16.927929 pyobjc-framework-CoreMedia-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:16.819785 pyobjc-framework-CoreMedia-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:16.843891 pyobjc-framework-CoreMedia-9.1b1/Lib/CoreMedia/
--rw-r--r--   0 ronald     (501) staff       (20)      933 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.1b1/Lib/CoreMedia/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2144 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.1b1/Lib/CoreMedia/_macros.py
--rw-r--r--   0 ronald     (501) staff       (20)    89518 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMedia-9.1b1/Lib/CoreMedia/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:16.847563 pyobjc-framework-CoreMedia-9.1b1/Lib/pyobjc_framework_CoreMedia.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2107 2023-03-26 11:21:16.000000 pyobjc-framework-CoreMedia-9.1b1/Lib/pyobjc_framework_CoreMedia.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1402 2023-03-26 11:21:16.000000 pyobjc-framework-CoreMedia-9.1b1/Lib/pyobjc_framework_CoreMedia.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:21:16.000000 pyobjc-framework-CoreMedia-9.1b1/Lib/pyobjc_framework_CoreMedia.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:51.000000 pyobjc-framework-CoreMedia-9.1b1/Lib/pyobjc_framework_CoreMedia.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:21:16.000000 pyobjc-framework-CoreMedia-9.1b1/Lib/pyobjc_framework_CoreMedia.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:21:16.000000 pyobjc-framework-CoreMedia-9.1b1/Lib/pyobjc_framework_CoreMedia.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreMedia-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:16.849528 pyobjc-framework-CoreMedia-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)    11756 2022-10-18 09:53:23.000000 pyobjc-framework-CoreMedia-9.1b1/Modules/_CoreMedia.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreMedia-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreMedia-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1896 2023-03-26 11:21:16.927592 pyobjc-framework-CoreMedia-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:16.877104 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2190 2022-10-18 09:53:23.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmattachment.py
--rw-r--r--   0 ronald     (501) staff       (20)     1608 2022-10-18 09:53:23.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmaudiodeviceclock.py
--rw-r--r--   0 ronald     (501) staff       (20)      190 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmbase.py
--rw-r--r--   0 ronald     (501) staff       (20)     5571 2022-10-18 09:53:23.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmblockbuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)     5883 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmbufferqueue.py
--rw-r--r--   0 ronald     (501) staff       (20)    35530 2022-06-15 11:57:00.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmformatdescription.py
--rw-r--r--   0 ronald     (501) staff       (20)    11561 2022-06-15 11:57:00.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmformatdescriptionbridge.py
--rw-r--r--   0 ronald     (501) staff       (20)      642 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmmemorypool.py
--rw-r--r--   0 ronald     (501) staff       (20)     7033 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmmetadata.py
--rw-r--r--   0 ronald     (501) staff       (20)    18353 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmsamplebuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1061 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmsimplequeue.py
--rw-r--r--   0 ronald     (501) staff       (20)     5427 2021-07-30 09:00:37.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmsync.py
--rw-r--r--   0 ronald     (501) staff       (20)     4099 2022-06-15 11:57:00.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmtextmarkup.py
--rw-r--r--   0 ronald     (501) staff       (20)     3522 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmtime.py
--rw-r--r--   0 ronald     (501) staff       (20)     2655 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmtimerange.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_coremedia.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:16.879701 pyobjc-framework-CoreMedia-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    38597 2022-10-18 09:53:23.000000 pyobjc-framework-CoreMedia-9.1b1/metadata/CoreMedia.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:16.925673 pyobjc-framework-CoreMedia-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   152776 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMedia-9.1b1/metadata/raw/arm64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   152890 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMedia-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   157400 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMedia-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   147578 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.1b1/metadata/raw/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   149282 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   149776 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMedia-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   152778 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMedia-9.1b1/metadata/raw/x86_64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   152892 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMedia-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   157400 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMedia-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     2888 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMedia-9.1b1/patch.txt
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreMedia-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:21:16.928021 pyobjc-framework-CoreMedia-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      860 2023-03-25 14:20:31.000000 pyobjc-framework-CoreMedia-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:15.875074 pyobjc-framework-CoreMedia-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:15.800475 pyobjc-framework-CoreMedia-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:15.807053 pyobjc-framework-CoreMedia-9.2/Lib/CoreMedia/
+-rw-r--r--   0 ronald     (501) staff       (20)      933 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.2/Lib/CoreMedia/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2144 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.2/Lib/CoreMedia/_macros.py
+-rw-r--r--   0 ronald     (501) staff       (20)    89567 2023-05-27 09:46:33.000000 pyobjc-framework-CoreMedia-9.2/Lib/CoreMedia/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:15.810926 pyobjc-framework-CoreMedia-9.2/Lib/pyobjc_framework_CoreMedia.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2105 2023-06-07 00:11:15.000000 pyobjc-framework-CoreMedia-9.2/Lib/pyobjc_framework_CoreMedia.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1417 2023-06-07 00:11:15.000000 pyobjc-framework-CoreMedia-9.2/Lib/pyobjc_framework_CoreMedia.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:11:15.000000 pyobjc-framework-CoreMedia-9.2/Lib/pyobjc_framework_CoreMedia.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:51.000000 pyobjc-framework-CoreMedia-9.2/Lib/pyobjc_framework_CoreMedia.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:11:15.000000 pyobjc-framework-CoreMedia-9.2/Lib/pyobjc_framework_CoreMedia.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:11:15.000000 pyobjc-framework-CoreMedia-9.2/Lib/pyobjc_framework_CoreMedia.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreMedia-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:15.812863 pyobjc-framework-CoreMedia-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)    11756 2022-10-18 09:53:23.000000 pyobjc-framework-CoreMedia-9.2/Modules/_CoreMedia.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreMedia-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CoreMedia-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1894 2023-06-07 00:11:15.874640 pyobjc-framework-CoreMedia-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:15.845550 pyobjc-framework-CoreMedia-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2190 2022-10-18 09:53:23.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmattachment.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1608 2022-10-18 09:53:23.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmaudiodeviceclock.py
+-rw-r--r--   0 ronald     (501) staff       (20)      190 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmbase.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5571 2022-10-18 09:53:23.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmblockbuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5883 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmbufferqueue.py
+-rw-r--r--   0 ronald     (501) staff       (20)    37116 2023-05-27 09:46:33.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmformatdescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11561 2022-06-15 11:57:00.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmformatdescriptionbridge.py
+-rw-r--r--   0 ronald     (501) staff       (20)      642 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmmemorypool.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7033 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmmetadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)    18352 2023-05-27 09:46:33.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmsamplebuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1061 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmsimplequeue.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5427 2021-07-30 09:00:37.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmsync.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4099 2022-06-15 11:57:00.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmtextmarkup.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3522 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmtime.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2655 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmtimerange.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_coremedia.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:15.847918 pyobjc-framework-CoreMedia-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    39280 2023-05-27 09:46:33.000000 pyobjc-framework-CoreMedia-9.2/metadata/CoreMedia.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:15.862569 pyobjc-framework-CoreMedia-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   152776 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMedia-9.2/metadata/raw/arm64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   152890 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMedia-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   157400 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMedia-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   147578 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.2/metadata/raw/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   149282 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMedia-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   149776 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMedia-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   152778 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMedia-9.2/metadata/raw/x86_64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   152892 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMedia-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   157400 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMedia-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     2888 2022-10-19 09:49:10.000000 pyobjc-framework-CoreMedia-9.2/patch.txt
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreMedia-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreMedia-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:11:15.875175 pyobjc-framework-CoreMedia-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      941 2023-05-29 10:07:45.000000 pyobjc-framework-CoreMedia-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreMedia-9.1b1/Lib/CoreMedia/__init__.py` & `pyobjc-framework-CoreMedia-9.2/Lib/CoreMedia/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/Lib/CoreMedia/_macros.py` & `pyobjc-framework-CoreMedia-9.2/Lib/CoreMedia/_macros.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/Lib/CoreMedia/_metadata.py` & `pyobjc-framework-CoreMedia-9.2/Lib/CoreMedia/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Wed Oct 19 11:25:59 2022
+# Last update: Fri May 19 12:14:28 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -102,14 +102,16 @@
         {
             "retval": {"already_cfretained": True},
             "arguments": {3: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
     "CMAudioFormatDescriptionGetStreamBasicDescription": (
         b"^{AudioStreamBasicDescription=dIIIIIIII}^{opaqueCMFormatDescription=}",
+        "",
+        {"retval": {"deref_result_pointer": True}},
     ),
     "CMTimeMappingMakeFromDictionary": (
         b"{_CMTimeMapping={_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}{_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}}^{__CFDictionary=}",
     ),
     "CMBufferQueueEnqueue": (b"i^{opaqueCMBufferQueue=}@",),
     "CMBufferQueueInstallTrigger": (
         b"i^{opaqueCMBufferQueue=}^?^vi{_CMTime=qiIq}^^{opaqueCMBufferQueueTriggerToken=}",
@@ -154,15 +156,19 @@
     ),
     "CMTimebaseCopyMasterClock": (
         b"^{OpaqueCMClock=}^{OpaqueCMTimebase=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CMClockMightDrift": (b"Z^{OpaqueCMClock=}^{OpaqueCMClock=}",),
-    "CMTimebaseGetTimeAndRate": (b"i^{OpaqueCMTimebase=}^{_CMTime=qiIq}^d",),
+    "CMTimebaseGetTimeAndRate": (
+        b"i^{OpaqueCMTimebase=}^{_CMTime=qiIq}^d",
+        "",
+        {"arguments": {1: {"type_modifier": "o"}, 2: {"type_modifier": "o"}}},
+    ),
     "CMMetadataCreateIdentifierForKeyAndKeySpace": (
         b"i^{__CFAllocator=}@^{__CFString=}^^{__CFString=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {3: {"already_cfretained": True, "type_modifier": "o"}},
         },
@@ -328,15 +334,25 @@
     "CMMetadataFormatDescriptionGetKeyWithLocalID": (
         b"^{__CFDictionary=}^{opaqueCMFormatDescription=}I",
     ),
     "CMMetadataDataTypeRegistryRegisterDataType": (
         b"i^{__CFString=}^{__CFString=}^{__CFArray=}",
     ),
     "CMBufferQueueGetTypeID": (b"Q",),
-    "CMBlockBufferGetDataPointer": (b"i^{OpaqueCMBlockBuffer=}Q^Q^Q^^v",),
+    "CMBlockBufferGetDataPointer": (
+        b"i^{OpaqueCMBlockBuffer=}Q^Q^Q^^v",
+        "",
+        {
+            "arguments": {
+                2: {"type_modifier": "o"},
+                3: {"type_modifier": "o"},
+                4: {"c_array_length_in_arg": 2, "type_modifier": "o"},
+            }
+        },
+    ),
     "CMSampleBufferGetImageBuffer": (b"^{__CVBuffer=}^{opaqueCMSampleBuffer=}",),
     "CMBufferQueueCallForEachBuffer": (
         b"i^{opaqueCMBufferQueue=}^?^v",
         "",
         {
             "arguments": {
                 1: {
@@ -358,14 +374,15 @@
     ),
     "CMSampleBufferCreateForImageBufferWithMakeDataReadyHandler": (
         b"i^{__CFAllocator=}^{__CVBuffer=}Z^{opaqueCMFormatDescription=}^{_CMSampleTimingInfo={_CMTime=qiIq}{_CMTime=qiIq}{_CMTime=qiIq}}^^{opaqueCMSampleBuffer=}@?",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {
+                4: {"type_modifier": "n"},
                 5: {"already_cfretained": True, "type_modifier": "o"},
                 6: {
                     "callable": {
                         "retval": {"type": b"i"},
                         "arguments": {
                             0: {"type": "^v"},
                             1: {"type": "^{OpaqueCMSampleBuffer=}"},
@@ -575,14 +592,16 @@
         b"{_CMTime=qiIq}{_CMTime=qiIq}{_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}",
     ),
     "CMFormatDescriptionGetExtension": (
         b"@^{opaqueCMFormatDescription=}^{__CFString=}",
     ),
     "CMAudioFormatDescriptionGetRichestDecodableFormat": (
         b"^{AudioFormatListItem={AudioStreamBasicDescription=dIIIIIIII}I}^{opaqueCMFormatDescription=}",
+        "",
+        {"retval": {"deref_result_pointer": True}},
     ),
     "CMSyncGetRelativeRate": (b"d@@",),
     "CMMetadataCreateKeySpaceFromIdentifier": (
         b"i^{__CFAllocator=}^{__CFString=}^^{__CFString=}",
         "",
         {
             "retval": {"already_cfretained": True},
@@ -590,16 +609,16 @@
         },
     ),
     "CMTimebaseCopyUltimateMasterClock": (
         b"^{OpaqueCMClock=}^{OpaqueCMTimebase=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
-    "CMBufferQueueGetCallbacksForUnsortedSampleBuffers": (
-        b"^{_CMBufferCallbacks=I^v^?^?^?^?^?^{__CFString=}^?}",
+    "CMTimeRangeGetEnd": (
+        b"{_CMTime=qiIq}{_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}",
     ),
     "CMSampleBufferGetDataBuffer": (
         b"^{OpaqueCMBlockBuffer=}^{opaqueCMSampleBuffer=}",
     ),
     "CMSampleBufferInvalidate": (b"i^{opaqueCMSampleBuffer=}",),
     "CMBufferQueueGetDuration": (b"{_CMTime=qiIq}^{opaqueCMBufferQueue=}",),
     "CMMetadataFormatDescriptionCopyAsBigEndianMetadataDescriptionBlockBuffer": (
@@ -741,15 +760,18 @@
                 5: {"type_modifier": "o"},
             }
         },
     ),
     "CMAudioClockCreate": (
         b"i^{__CFAllocator=}^^{OpaqueCMClock=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {1: {"already_cfretained": True, "type_modifier": "o"}},
+        },
     ),
     "CMMetadataFormatDescriptionCreateWithMetadataFormatDescriptionAndMetadataSpecifications": (
         b"i^{__CFAllocator=}^{opaqueCMFormatDescription=}^{__CFArray=}^^{opaqueCMFormatDescription=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {3: {"already_cfretained": True, "type_modifier": "o"}},
@@ -1030,17 +1052,14 @@
         b"{_CMTime=qiIq}{_CMTime=qiIq}{_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}{_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}",
     ),
     "CMTextFormatDescriptionGetDefaultTextBox": (
         b"i^{opaqueCMFormatDescription=}Zd^{CGRect={CGPoint=dd}{CGSize=dd}}",
         "",
         {"arguments": {3: {"type_modifier": "o"}}},
     ),
-    "CMTimeRangeGetEnd": (
-        b"{_CMTime=qiIq}{_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}",
-    ),
     "CMBufferQueueSetValidationHandler": (
         b"i@@?",
         "",
         {
             "arguments": {
                 1: {
                     "callable": {
@@ -1059,14 +1078,16 @@
     "CMTimeRangeContainsTimeRange": (
         b"Z{_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}{_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}",
     ),
     "CMSampleBufferSetDataFailed": (b"i^{opaqueCMSampleBuffer=}i",),
     "CMTimebaseSetTimerDispatchSourceToFireImmediately": (b"i^{OpaqueCMTimebase=}@",),
     "CMAudioFormatDescriptionGetMostCompatibleFormat": (
         b"^{AudioFormatListItem={AudioStreamBasicDescription=dIIIIIIII}I}^{opaqueCMFormatDescription=}",
+        "",
+        {"retval": {"deref_result_pointer": True}},
     ),
     "CMTimeClampToRange": (
         b"{_CMTime=qiIq}{_CMTime=qiIq}{_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}",
     ),
     "CMFormatDescriptionEqualIgnoringExtensionKeys": (
         b"Z^{opaqueCMFormatDescription=}^{opaqueCMFormatDescription=}@@",
     ),
@@ -1137,29 +1158,18 @@
         {
             "arguments": {
                 2: {"c_array_length_in_arg": 1, "type_modifier": "o"},
                 3: {"type_modifier": "o"},
             }
         },
     ),
-    "CMVideoFormatDescriptionGetHEVCParameterSetAtIndex": (
-        b"i^{opaqueCMFormatDescription=}Q^^C^Q^Q^i",
-    ),
     "CMTimebaseSetTime": (b"i^{OpaqueCMTimebase=}{_CMTime=qiIq}",),
-    "CMVideoFormatDescriptionGetH264ParameterSetAtIndex": (
-        b"i^{opaqueCMFormatDescription=}Q^^C^Q^Q^i",
-    ),
     "CMMetadataDataTypeRegistryGetConformingDataTypes": (
         b"^{__CFArray=}^{__CFString=}",
     ),
-    "CMBufferQueueCreate": (
-        b"i^{__CFAllocator=}q^{_CMBufferCallbacks=I^v^?^?^?^?^?^{__CFString=}^?}^^{opaqueCMBufferQueue=}",
-        "",
-        {"retval": {"already_cfretained": True}},
-    ),
     "CMSyncGetTime": (b"{_CMTime=qiIq}@",),
     "CMAudioFormatDescriptionCreateFromBigEndianSoundDescriptionData": (
         b"i^{__CFAllocator=}^CQ^{__CFString=}^^{opaqueCMFormatDescription=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {
@@ -1247,15 +1257,18 @@
             "retval": {"already_cfretained": True},
             "arguments": {3: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
     "CMBlockBufferAccessDataBytes": (
         b"i^{OpaqueCMBlockBuffer=}QQ^v^^v",
         "",
-        {"suggestion": "Use CMBlockBufferCopyDataBytes"},
+        {
+            "arguments": {4: {"type_modifier": "o"}},
+            "suggestion": "Use CMBlockBufferCopyDataBytes",
+        },
     ),
     "CMTimeMappingCopyDescription": (
         b"^{__CFString=}^{__CFAllocator=}{_CMTimeMapping={_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}{_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CMAudioFormatDescriptionCreateSummary": (
@@ -1296,26 +1309,24 @@
     ),
     "CMAudioFormatDescriptionCreate": (
         b"i^{__CFAllocator=}^{AudioStreamBasicDescription=dIIIIIIII}Q^{AudioChannelLayout=III[1{AudioChannelDescription=II[3f]}]}Q^v^{__CFDictionary=}^^{opaqueCMFormatDescription=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {
+                1: {"type_modifier": "n"},
                 3: {"type_modifier": "n"},
                 5: {"c_array_length_in_arg": 4, "type_modifier": "n"},
                 7: {"already_cfretained": True, "type_modifier": "o"},
             },
         },
     ),
     "CMSampleBufferGetOutputPresentationTimeStamp": (
         b"{_CMTime=qiIq}^{opaqueCMSampleBuffer=}",
     ),
-    "CMBufferQueueGetCallbacksForSampleBuffersSortedByOutputPTS": (
-        b"^{_CMBufferCallbacks=I^v^?^?^?^?^?^{__CFString=}^?}",
-    ),
     "CMVideoFormatDescriptionCreate": (
         b"i^{__CFAllocator=}Iii^{__CFDictionary=}^^{opaqueCMFormatDescription=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {5: {"already_cfretained": True, "type_modifier": "o"}},
         },
@@ -1435,30 +1446,30 @@
         b"i^{opaqueCMFormatDescription=}^I",
         "",
         {"arguments": {1: {"type_modifier": "o"}}},
     ),
     "CMSimpleQueueGetTypeID": (b"Q",),
     "CMTimeMaximum": (b"{_CMTime=qiIq}{_CMTime=qiIq}{_CMTime=qiIq}",),
     "CMSampleBufferCreateWithMakeDataReadyHandler": (
-        b"i^{__CFAllocator=}^{OpaqueCMBlockBuffer=}Z^{OpaqueCMFormatDescription=}ll^{_CMSampleTimingInfo={_CMTime=qiIq}{_CMTime=qiIq}{_CMTime=qiIq}}^^{opaqueCMSampleBuffer=}@?^^{opaqueCMSampleBuffer=}@?",
+        b"i^{__CFAllocator=}^{OpaqueCMBlockBuffer=}Z^{OpaqueCMFormatDescription=}ll^{_CMSampleTimingInfo={_CMTime=qiIq}{_CMTime=qiIq}{_CMTime=qiIq}}l^Q@?@?",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {
-                8: {
+                8: {"c_array_length_in_arg": 7, "type_modifier": "n"},
+                9: {
                     "callable": {
                         "retval": {"type": b"i"},
                         "arguments": {
                             0: {"type": "^v"},
                             1: {"type": "^{OpaqueCMSampleBuffer=}"},
                         },
                     }
                 },
                 6: {"c_array_length_in_arg": 5, "type_modifier": "n"},
-                7: {"already_cfretained": True, "type_modifier": "o"},
             },
         },
     ),
     "CMTimeCodeFormatDescriptionCreate": (
         b"i^{__CFAllocator=}I{_CMTime=qiIq}II^{__CFDictionary=}^^{opaqueCMFormatDescription=}",
         "",
         {
```

### Comparing `pyobjc-framework-CoreMedia-9.1b1/Lib/pyobjc_framework_CoreMedia.egg-info/PKG-INFO` & `pyobjc-framework-CoreMedia-9.2/Lib/pyobjc_framework_CoreMedia.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreMedia
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreMedia on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreMedia
 Platform: MacOS X (>=10.7)
```

### Comparing `pyobjc-framework-CoreMedia-9.1b1/Lib/pyobjc_framework_CoreMedia.egg-info/SOURCES.txt` & `pyobjc-framework-CoreMedia-9.2/Lib/pyobjc_framework_CoreMedia.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 License.txt
 MANIFEST.in
 patch.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CoreMedia/__init__.py
 Lib/CoreMedia/_macros.py
 Lib/CoreMedia/_metadata.py
 Lib/pyobjc_framework_CoreMedia.egg-info/PKG-INFO
 Lib/pyobjc_framework_CoreMedia.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CoreMedia.egg-info/dependency_links.txt
```

### Comparing `pyobjc-framework-CoreMedia-9.1b1/License.txt` & `pyobjc-framework-CoreMedia-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/Modules/_CoreMedia.m` & `pyobjc-framework-CoreMedia-9.2/Modules/_CoreMedia.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreMedia-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreMedia-9.2/Modules/pyobjc-compat.h`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,22 @@
 #define MAC_OS_X_VERSION_13_2 130200
 #endif
 
 #ifndef MAC_OS_X_VERSION_13_3
 #define MAC_OS_X_VERSION_13_3 130300
 #endif
 
+#ifndef MAC_OS_X_VERSION_13_4
+#define MAC_OS_X_VERSION_13_4 130400
+#endif
+
+#ifndef MAC_OS_X_VERSION_13_5
+#define MAC_OS_X_VERSION_13_5 130500
+#endif
+
 /*
  *
  * End of Cocoa definitions
  *
  */
 
 /*
@@ -499,10 +507,12 @@
     }
 
 #define PyObjC_LEAVE_GIL                                                                 \
     do {                                                                                 \
         PyGILState_Release(_GILState);                                                   \
     } while (0)
 
+extern PyObject* _Nullable PyObjC_get_tp_dict(PyTypeObject* _Nonnull tp);
+
 NS_ASSUME_NONNULL_END
 
 #endif /* PyObjC_COMPAT_H */
```

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PKG-INFO` & `pyobjc-framework-CoreMedia-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreMedia
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreMedia on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreMedia
 Platform: MacOS X (>=10.7)
```

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmattachment.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmattachment.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmaudiodeviceclock.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmaudiodeviceclock.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmblockbuffer.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmblockbuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmbufferqueue.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmbufferqueue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmformatdescription.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmformatdescription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import CoreMedia
+import CoreAudio
 from PyObjCTools.TestSupport import TestCase, min_os_level, expectedFailure, fourcc
 import objc
 
 
 class TestCMFormatDescription(TestCase):
     def test_constants(self):
         self.assertEqual(CoreMedia.kCMFormatDescriptionError_InvalidParameter, -12710)
@@ -503,30 +504,32 @@
         )
         self.assertIsInstance(CoreMedia.kCMFormatDescriptionChromaLocation_Bottom, str)
         self.assertIsInstance(CoreMedia.kCMFormatDescriptionChromaLocation_DV420, str)
 
         self.assertIsInstance(
             CoreMedia.kCMMetadataFormatDescriptionKey_StructuralDependency, str
         )
-        self.assertIsInstance(CoreMedia.kCMMetadataFormatDescriptionKey_SetupData, str)
         self.assertIsInstance(
             CoreMedia.kCMMetadataFormatDescription_StructuralDependencyKey_DependencyIsInvalidFlag,
             str,
         )
         self.assertIsInstance(
             CoreMedia.kCMMetadataFormatDescriptionMetadataSpecificationKey_StructuralDependency,
             str,
         )
+
+    @min_os_level("10.12")
+    def test_constants10_12(self):
+        # The first two are documented as available on 10.11, but aren't
+        self.assertIsInstance(CoreMedia.kCMMetadataFormatDescriptionKey_SetupData, str)
         self.assertIsInstance(
             CoreMedia.kCMMetadataFormatDescriptionMetadataSpecificationKey_SetupData,
             str,
         )
 
-    @min_os_level("10.12")
-    def test_constants10_12(self):
         self.assertIsInstance(
             CoreMedia.kCMFormatDescriptionTransferFunction_SMPTE_ST_428_1, str
         )
 
     @min_os_level("10.13")
     def test_constants10_13(self):
         self.assertIsInstance(
@@ -760,7 +763,48 @@
         )
         self.assertArgIsCFRetained(
             CoreMedia.CMMetadataFormatDescriptionCreateByMergingMetadataFormatDescriptions,
             3,
         )
 
         CoreMedia.CMMetadataFormatDescriptionGetIdentifiers
+
+    def no_test_functions_usage(self):
+        # XXX: Test disabled due to periodic crashes in system libraries.
+        asbd = CoreAudio.AudioStreamBasicDescription(
+            mSampleRate=44000.0,
+            mFormatID=1819304813,
+            mFormatFlags=4,
+            mBytesPerPacket=4,
+            mFramesPerPacket=1,
+            mBytesPerFrame=0,
+            mChannelsPerFrame=2,
+            mBitsPerChannel=16,
+            mReserved=0,
+        )
+        ok, fmt = CoreMedia.CMAudioFormatDescriptionCreate(
+            None, asbd, 0, None, 0, None, None, None
+        )
+        self.assertEqual(ok, 0)
+
+        lst, cnt = CoreMedia.CMAudioFormatDescriptionGetFormatList(fmt, None)
+        self.assertEqual(len(lst), cnt)
+
+        result = CoreMedia.CMAudioFormatDescriptionGetMostCompatibleFormat(fmt)
+        self.assertIsInstance(result, CoreAudio.AudioFormatListItem)
+
+        for item in lst:
+            ok, fmt = CoreMedia.CMAudioFormatDescriptionCreate(
+                None, item.mASBD, 0, None, 0, None, None, None
+            )
+            if ok != 0:
+                continue
+
+            result = CoreMedia.CMAudioFormatDescriptionGetRichestDecodableFormat(fmt)
+            if result is None or result is objc.NULL:
+                continue
+            self.assertIsInstance(result, CoreAudio.AudioFormatListItem)
+            break
+        else:
+            # XXX: Seems to return NULL at all times...
+            pass
+            # self.fail("did not find richest format")
```

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmformatdescriptionbridge.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmformatdescriptionbridge.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmmemorypool.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmmemorypool.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmmetadata.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmmetadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmsamplebuffer.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmsamplebuffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,21 +380,21 @@
     @min_os_level("10.14.4")
     def test_functions_10_14_4(self):
         self.assertArgIsBOOL(CoreMedia.CMSampleBufferCreateWithMakeDataReadyHandler, 2)
         self.assertArgIsIn(CoreMedia.CMSampleBufferCreateWithMakeDataReadyHandler, 6)
         self.assertArgSizeInArg(
             CoreMedia.CMSampleBufferCreateWithMakeDataReadyHandler, 6, 5
         )
-        self.assertArgIsOut(CoreMedia.CMSampleBufferCreateWithMakeDataReadyHandler, 7)
-        self.assertArgIsCFRetained(
-            CoreMedia.CMSampleBufferCreateWithMakeDataReadyHandler, 7
+        self.assertArgIsIn(CoreMedia.CMSampleBufferCreateWithMakeDataReadyHandler, 8)
+        self.assertArgSizeInArg(
+            CoreMedia.CMSampleBufferCreateWithMakeDataReadyHandler, 8, 7
         )
         self.assertArgIsBlock(
             CoreMedia.CMSampleBufferCreateWithMakeDataReadyHandler,
-            8,
+            9,
             b"i^{OpaqueCMSampleBuffer=}",
         )
 
         self.assertArgIsBOOL(
             CoreMedia.CMAudioSampleBufferCreateWithPacketDescriptionsAndMakeDataReadyHandler,
             2,
         )
```

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmsimplequeue.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmsimplequeue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmsync.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmsync.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmtextmarkup.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmtextmarkup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmtime.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmtime.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/PyObjCTest/test_cmtimerange.py` & `pyobjc-framework-CoreMedia-9.2/PyObjCTest/test_cmtimerange.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/metadata/CoreMedia.fwinfo` & `pyobjc-framework-CoreMedia-9.2/metadata/CoreMedia.fwinfo`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,19 @@
   },
   "externs": {
    "kCMMetadataIdentifier_QuickTimeMetadataLivePhotoStillImageTransformReferenceDimensions": { "typestr": "@" },
    "kCMFormatDescriptionTransferFunction_Linear": { "typestr": "@" },
    "kCMFormatDescriptionExtension_AlternativeTransferCharacteristics": { "typestr": "@" }
   },
   "functions": {
+  "CMAudioClockCreate": {
+   "args": {
+    "1": { "type_modifier": "o", "already_cfretained": true }
+   }
+  },
   "CMTimebaseCreateWithSourceClock": {
    "args": {
     "2": { "type_modifier": "o", "already_cfretained": true }
    }
   },
   "CMTimebaseCreateWithSourceTimebase": {
    "args": {
@@ -89,14 +94,15 @@
       "retval": { "type": "i" }
      }
     }
    }
   },
   "CMSampleBufferCreateForImageBufferWithMakeDataReadyHandler": {
    "args": {
+    "4": { "type_modifier": "n" },
     "5": { "type_modifier": "o", "already_cfretained": true },
     "6": {
      "callable": {
       "arguments": {
        "0": { "type": "^v" },
        "1": { "type": "^{OpaqueCMSampleBuffer=}" }
       },
@@ -113,16 +119,17 @@
     "0": { "type_override": "^{__CFAllocator=}" },
     "1": { "type_override": "^{OpaqueCMBlockBuffer=}" },
     "2": { "type_override": "Z" },
     "3": { "type_override": "^{OpaqueCMFormatDescription=}" },
     "4": { "type_override": "l" },
     "5": { "type_override": "l" },
     "6": { "type_modifier": "n", "c_array_length_in_arg": 5, "type_override": "^{_CMSampleTimingInfo={_CMTime=qiIq}{_CMTime=qiIq}{_CMTime=qiIq}}" },
-    "7": { "type_modifier": "o", "type_override": "^^{opaqueCMSampleBuffer=}", "already_cfretained": true },
-    "8": {
+    "7": { "type_override": "l" },
+    "8": { "type_modifier": "n", "c_array_length_in_arg": 7 },
+    "9": {
      "type_override": "@?",
      "callable": {
       "arguments": {
        "0": { "type": "^v" },
        "1": { "type": "^{OpaqueCMSampleBuffer=}" }
       },
       "retval": { "type": "i" }
@@ -228,15 +235,15 @@
      "2": {},
      "3": { "type_modifier": "o", "already_cfretained": true }
     }
    },
    "CMAudioFormatDescriptionCreate": {
     "args": {
      "0": {},
-     "1": {},
+     "1": { "type_modifier": "n" },
      "3": { "type_modifier": "n" },
      "5": { "type_modifier": "n", "c_array_length_in_arg": 4 },
      "6": {},
      "7": { "type_modifier": "o", "already_cfretained": true }
     }
    },
    "CMAudioFormatDescriptionCreateFromBigEndianSoundDescriptionBlockBuffer": {
@@ -290,27 +297,27 @@
     },
     "retval": { "c_array_length_in_arg": 1 }
    },
    "CMAudioFormatDescriptionGetMostCompatibleFormat": {
     "args": {
      "0": {}
     },
-    "retval": {}
+    "retval": { "deref_result_pointer": true }
    },
    "CMAudioFormatDescriptionGetRichestDecodableFormat": {
     "args": {
      "0": {}
     },
-    "retval": {}
+    "retval": { "deref_result_pointer": true }
    },
    "CMAudioFormatDescriptionGetStreamBasicDescription": {
     "args": {
      "0": {}
     },
-    "retval": {}
+    "retval": { "deref_result_pointer": true }
    },
    "CMAudioSampleBufferCreateReadyWithPacketDescriptions": {
     "args": {
      "0": {},
      "1": {},
      "2": {},
      "5": { "type_modifier": "n", "c_array_length_in_arg": 3 },
@@ -343,15 +350,15 @@
     }
    },
    "CMBlockBufferAccessDataBytes": {
     "suggestion": "Use CMBlockBufferCopyDataBytes",
     "args": {
      "0": {},
      "3": {},
-     "4": { "type_override": "^^v" }
+     "4": { "type_override": "^^v", "type_modifier": "o" }
     }
    },
    "CMBlockBufferAppendBufferReference": {
     "args": {
      "0": {},
      "1": {}
     }
@@ -415,17 +422,17 @@
     "args": {
      "0": {}
     }
    },
    "CMBlockBufferGetDataPointer": {
     "args": {
      "0": {},
-     "2": {},
-     "3": {},
-     "4": { "type_override": "^^v" }
+     "2": { "type_modifier": "o" },
+     "3": { "type_modifier": "o" },
+     "4": { "type_override": "^^v", "type_modifier": "o", "c_array_length_in_arg": 2 }
     }
    },
    "CMBlockBufferIsEmpty": {
     "args": {
      "0": {}
     }
    },
@@ -463,14 +470,15 @@
    },
    "CMBufferQueueContainsEndOfData": {
     "args": {
      "0": {}
     }
    },
    "CMBufferQueueCreate": {
+    "ignore": true,
     "args": {
      "0": {},
      "2": {},
      "3": {}
     }
    },
    "CMBufferQueueDequeueAndRetain": {
@@ -496,17 +504,19 @@
    },
    "CMBufferQueueGetBufferCount": {
     "args": {
      "0": {}
     }
    },
    "CMBufferQueueGetCallbacksForSampleBuffersSortedByOutputPTS": {
+    "ignore": true,
     "retval": {}
    },
    "CMBufferQueueGetCallbacksForUnsortedSampleBuffers": {
+    "ignore": true,
     "retval": {}
    },
    "CMBufferQueueGetDuration": {
     "args": {
      "0": {}
     }
    },
@@ -1675,16 +1685,16 @@
     "args": {
      "0": {}
     }
    },
    "CMTimebaseGetTimeAndRate": {
     "args": {
      "0": {},
-     "1": {},
-     "2": {}
+     "1": { "type_modifier": "o" },
+     "2": { "type_modifier": "o" }
     }
    },
    "CMTimebaseGetTimeWithTimeScale": {
     "args": {
      "0": {}
     }
    },
@@ -1802,29 +1812,31 @@
      "0": {}
     }
    },
    "CMVideoFormatDescriptionGetExtensionKeysCommonWithImageBuffers": {
     "retval": {}
    },
    "CMVideoFormatDescriptionGetH264ParameterSetAtIndex": {
+    "ignore": true,
     "args": {
      "0": {},
-     "2": {},
-     "3": {},
-     "4": {},
-     "5": {}
+     "2": { "type_modifier": "o" },
+     "3": { "type_modifier": "o" },
+     "4": { "type_modifier": "o" },
+     "5": { "type_modifier": "o" }
     }
    },
    "CMVideoFormatDescriptionGetHEVCParameterSetAtIndex": {
+    "ignore": true,
     "args": {
      "0": {},
-     "2": {},
-     "3": {},
-     "4": {},
-     "5": {}
+     "2": { "type_modifier": "o" },
+     "3": { "type_modifier": "o" },
+     "4": { "type_modifier": "o" },
+     "5": { "type_modifier": "o" }
     }
    },
    "CMVideoFormatDescriptionGetPresentationDimensions": {
     "args": {
      "0": {}
     }
    },
```

### Comparing `pyobjc-framework-CoreMedia-9.1b1/metadata/raw/arm64-12.1.fwinfo` & `pyobjc-framework-CoreMedia-9.2/metadata/raw/arm64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreMedia-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-CoreMedia-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/metadata/raw/x86_64-10.14.fwinfo` & `pyobjc-framework-CoreMedia-9.2/metadata/raw/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreMedia-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreMedia-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/metadata/raw/x86_64-12.1.fwinfo` & `pyobjc-framework-CoreMedia-9.2/metadata/raw/x86_64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreMedia-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-CoreMedia-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/patch.txt` & `pyobjc-framework-CoreMedia-9.2/patch.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMedia-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreMedia-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

