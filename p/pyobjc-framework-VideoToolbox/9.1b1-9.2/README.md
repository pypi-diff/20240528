# Comparing `tmp/pyobjc-framework-VideoToolbox-9.1b1.tar.gz` & `tmp/pyobjc-framework-VideoToolbox-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-VideoToolbox-9.1b1.tar", last modified: Sun Mar 26 11:43:28 2023, max compression
+gzip compressed data, was "pyobjc-framework-VideoToolbox-9.2.tar", last modified: Wed Jun  7 00:31:14 2023, max compression
```

## Comparing `pyobjc-framework-VideoToolbox-9.1b1.tar` & `pyobjc-framework-VideoToolbox-9.2.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:28.158108 pyobjc-framework-VideoToolbox-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:28.051483 pyobjc-framework-VideoToolbox-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:28.078558 pyobjc-framework-VideoToolbox-9.1b1/Lib/VideoToolbox/
--rw-r--r--   0 ronald     (501) staff       (20)      827 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.1b1/Lib/VideoToolbox/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    22913 2022-07-08 16:02:54.000000 pyobjc-framework-VideoToolbox-9.1b1/Lib/VideoToolbox/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:28.086832 pyobjc-framework-VideoToolbox-9.1b1/Lib/pyobjc_framework_VideoToolbox.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2119 2023-03-26 11:43:28.000000 pyobjc-framework-VideoToolbox-9.1b1/Lib/pyobjc_framework_VideoToolbox.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1522 2023-03-26 11:43:28.000000 pyobjc-framework-VideoToolbox-9.1b1/Lib/pyobjc_framework_VideoToolbox.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:43:28.000000 pyobjc-framework-VideoToolbox-9.1b1/Lib/pyobjc_framework_VideoToolbox.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:57.000000 pyobjc-framework-VideoToolbox-9.1b1/Lib/pyobjc_framework_VideoToolbox.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)      114 2023-03-26 11:43:28.000000 pyobjc-framework-VideoToolbox-9.1b1/Lib/pyobjc_framework_VideoToolbox.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       13 2023-03-26 11:43:28.000000 pyobjc-framework-VideoToolbox-9.1b1/Lib/pyobjc_framework_VideoToolbox.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-VideoToolbox-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:28.088734 pyobjc-framework-VideoToolbox-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     6298 2021-10-18 19:38:40.000000 pyobjc-framework-VideoToolbox-9.1b1/Modules/_VideoToolbox.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-VideoToolbox-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-VideoToolbox-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1908 2023-03-26 11:43:28.157644 pyobjc-framework-VideoToolbox-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:28.127707 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_videotoolbox.py
--rw-r--r--   0 ronald     (501) staff       (20)      422 2022-01-02 11:04:26.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtbase.py
--rw-r--r--   0 ronald     (501) staff       (20)    13705 2022-07-08 16:02:54.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtcompressionproperties.py
--rw-r--r--   0 ronald     (501) staff       (20)     2156 2022-01-02 11:04:26.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtcompressionsession.py
--rw-r--r--   0 ronald     (501) staff       (20)     5886 2021-07-30 09:00:38.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtdecompressionproperties.py
--rw-r--r--   0 ronald     (501) staff       (20)     1848 2022-01-02 11:04:26.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtdecompressionsession.py
--rw-r--r--   0 ronald     (501) staff       (20)     3856 2022-06-15 11:57:00.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vterrors.py
--rw-r--r--   0 ronald     (501) staff       (20)     1153 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtframesilo.py
--rw-r--r--   0 ronald     (501) staff       (20)      752 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtmultipassstorage.py
--rw-r--r--   0 ronald     (501) staff       (20)      784 2022-06-15 11:57:00.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtpixelrotationproperties.py
--rw-r--r--   0 ronald     (501) staff       (20)      655 2022-06-24 08:03:30.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtpixelrotationsession.py
--rw-r--r--   0 ronald     (501) staff       (20)     1662 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtpixeltransferproperties.py
--rw-r--r--   0 ronald     (501) staff       (20)      635 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtpixeltransfersession.py
--rw-r--r--   0 ronald     (501) staff       (20)      327 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtprofessionalvideoworkflow.py
--rw-r--r--   0 ronald     (501) staff       (20)     1999 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtsession.py
--rw-r--r--   0 ronald     (501) staff       (20)      462 2021-07-30 09:00:38.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtutilities.py
--rw-r--r--   0 ronald     (501) staff       (20)     2216 2021-07-30 09:00:38.000000 pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtvideoencoderlist.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:28.130301 pyobjc-framework-VideoToolbox-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     8255 2022-06-24 08:05:11.000000 pyobjc-framework-VideoToolbox-9.1b1/metadata/VideoToolbox.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:28.154233 pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    37865 2021-08-04 10:01:04.000000 pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    38267 2022-02-24 08:47:17.000000 pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    41844 2022-07-08 16:02:54.000000 pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    34073 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    35526 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36461 2021-03-21 10:08:23.000000 pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    37866 2021-08-04 10:01:04.000000 pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    38268 2022-02-24 08:47:17.000000 pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    41845 2022-07-08 16:02:54.000000 pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-VideoToolbox-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:43:28.158217 pyobjc-framework-VideoToolbox-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1284 2023-03-25 14:20:32.000000 pyobjc-framework-VideoToolbox-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:14.190140 pyobjc-framework-VideoToolbox-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:14.138237 pyobjc-framework-VideoToolbox-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:14.145524 pyobjc-framework-VideoToolbox-9.2/Lib/VideoToolbox/
+-rw-r--r--   0 ronald     (501) staff       (20)      827 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.2/Lib/VideoToolbox/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    23018 2023-05-27 09:46:33.000000 pyobjc-framework-VideoToolbox-9.2/Lib/VideoToolbox/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:14.148829 pyobjc-framework-VideoToolbox-9.2/Lib/pyobjc_framework_VideoToolbox.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2117 2023-06-07 00:31:14.000000 pyobjc-framework-VideoToolbox-9.2/Lib/pyobjc_framework_VideoToolbox.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1537 2023-06-07 00:31:14.000000 pyobjc-framework-VideoToolbox-9.2/Lib/pyobjc_framework_VideoToolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:31:14.000000 pyobjc-framework-VideoToolbox-9.2/Lib/pyobjc_framework_VideoToolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:57.000000 pyobjc-framework-VideoToolbox-9.2/Lib/pyobjc_framework_VideoToolbox.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)      106 2023-06-07 00:31:14.000000 pyobjc-framework-VideoToolbox-9.2/Lib/pyobjc_framework_VideoToolbox.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2023-06-07 00:31:14.000000 pyobjc-framework-VideoToolbox-9.2/Lib/pyobjc_framework_VideoToolbox.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-VideoToolbox-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:14.152830 pyobjc-framework-VideoToolbox-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     6298 2021-10-18 19:38:40.000000 pyobjc-framework-VideoToolbox-9.2/Modules/_VideoToolbox.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-VideoToolbox-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-VideoToolbox-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1906 2023-06-07 00:31:14.189745 pyobjc-framework-VideoToolbox-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:14.169017 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      208 2022-04-11 08:03:15.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_videotoolbox.py
+-rw-r--r--   0 ronald     (501) staff       (20)      422 2022-01-02 11:04:26.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtbase.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13705 2022-07-08 16:02:54.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtcompressionproperties.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2156 2022-01-02 11:04:26.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtcompressionsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5886 2021-07-30 09:00:38.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtdecompressionproperties.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1848 2022-01-02 11:04:26.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtdecompressionsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3856 2022-06-15 11:57:00.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vterrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1153 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtframesilo.py
+-rw-r--r--   0 ronald     (501) staff       (20)      752 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtmultipassstorage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      784 2022-06-15 11:57:00.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtpixelrotationproperties.py
+-rw-r--r--   0 ronald     (501) staff       (20)      655 2022-06-24 08:03:30.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtpixelrotationsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1662 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtpixeltransferproperties.py
+-rw-r--r--   0 ronald     (501) staff       (20)      635 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtpixeltransfersession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      327 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtprofessionalvideoworkflow.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1999 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      462 2021-07-30 09:00:38.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtutilities.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2216 2021-07-30 09:00:38.000000 pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtvideoencoderlist.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:14.170978 pyobjc-framework-VideoToolbox-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     8299 2023-05-27 09:46:33.000000 pyobjc-framework-VideoToolbox-9.2/metadata/VideoToolbox.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:14.188832 pyobjc-framework-VideoToolbox-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    37865 2021-08-04 10:01:04.000000 pyobjc-framework-VideoToolbox-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    38267 2022-02-24 08:47:17.000000 pyobjc-framework-VideoToolbox-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    41844 2022-07-08 16:02:54.000000 pyobjc-framework-VideoToolbox-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    34073 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.2/metadata/raw/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    35526 2020-11-30 18:45:15.000000 pyobjc-framework-VideoToolbox-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36461 2021-03-21 10:08:23.000000 pyobjc-framework-VideoToolbox-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    37866 2021-08-04 10:01:04.000000 pyobjc-framework-VideoToolbox-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    38268 2022-02-24 08:47:17.000000 pyobjc-framework-VideoToolbox-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    41845 2022-07-08 16:02:54.000000 pyobjc-framework-VideoToolbox-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-VideoToolbox-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-VideoToolbox-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:31:14.190262 pyobjc-framework-VideoToolbox-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1355 2023-05-29 10:07:47.000000 pyobjc-framework-VideoToolbox-9.2/setup.py
```

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/Lib/VideoToolbox/__init__.py` & `pyobjc-framework-VideoToolbox-9.2/Lib/VideoToolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/Lib/VideoToolbox/_metadata.py` & `pyobjc-framework-VideoToolbox-9.2/Lib/VideoToolbox/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Thu Jul  7 21:46:36 2022
+# Last update: Sat May 20 22:04:00 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -212,15 +212,19 @@
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {4: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
     "VTDecompressionSessionGetTypeID": (b"Q",),
-    "VTCompressionSessionBeginPass": (b"i^{OpaqueVTCompressionSession=}I^I",),
+    "VTCompressionSessionBeginPass": (
+        b"i^{OpaqueVTCompressionSession=}I^I",
+        "",
+        {"arguments": {2: {"type_modifier": "o"}}},
+    ),
     "VTSessionSetProperties": (b"i@^{__CFDictionary=}",),
     "VTDecompressionSessionWaitForAsynchronousFrames": (
         b"i^{OpaqueVTDecompressionSession=}",
     ),
     "VTFrameSiloSetTimeRangesForNextPass": (
         b"i^{OpaqueVTFrameSilo=}q^{_CMTimeRange={_CMTime=qiIq}{_CMTime=qiIq}}",
         "",
@@ -252,15 +256,15 @@
                 },
             }
         },
     ),
     "VTCompressionSessionEndPass": (
         b"i^{OpaqueVTCompressionSession=}^Z^I",
         "",
-        {"arguments": {1: {"type_modifier": "o"}}},
+        {"arguments": {1: {"type_modifier": "o"}, 2: {"type_modifier": "o"}}},
     ),
     "VTCompressionSessionEncodeFrame": (
         b"i^{OpaqueVTCompressionSession=}^{__CVBuffer=}{_CMTime=qiIq}{_CMTime=qiIq}^{__CFDictionary=}^v^I",
         "",
         {"arguments": {6: {"type_modifier": "o"}}},
     ),
     "VTFrameSiloCreate": (
```

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/Lib/pyobjc_framework_VideoToolbox.egg-info/PKG-INFO` & `pyobjc-framework-VideoToolbox-9.2/Lib/pyobjc_framework_VideoToolbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-VideoToolbox
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework VideoToolbox on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,VideoToolbox
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/Lib/pyobjc_framework_VideoToolbox.egg-info/SOURCES.txt` & `pyobjc-framework-VideoToolbox-9.2/Lib/pyobjc_framework_VideoToolbox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/VideoToolbox/__init__.py
 Lib/VideoToolbox/_metadata.py
 Lib/pyobjc_framework_VideoToolbox.egg-info/PKG-INFO
 Lib/pyobjc_framework_VideoToolbox.egg-info/SOURCES.txt
 Lib/pyobjc_framework_VideoToolbox.egg-info/dependency_links.txt
 Lib/pyobjc_framework_VideoToolbox.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/License.txt` & `pyobjc-framework-VideoToolbox-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/Modules/_VideoToolbox.m` & `pyobjc-framework-VideoToolbox-9.2/Modules/_VideoToolbox.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-VideoToolbox-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-VideoToolbox-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PKG-INFO` & `pyobjc-framework-VideoToolbox-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-VideoToolbox
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework VideoToolbox on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,VideoToolbox
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtcompressionproperties.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtcompressionproperties.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtcompressionsession.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtcompressionsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtdecompressionproperties.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtdecompressionproperties.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtdecompressionsession.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtdecompressionsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vterrors.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vterrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtframesilo.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtframesilo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtmultipassstorage.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtmultipassstorage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtpixelrotationproperties.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtpixelrotationproperties.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtpixelrotationsession.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtpixelrotationsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtpixeltransferproperties.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtpixeltransferproperties.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtpixeltransfersession.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtpixeltransfersession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtsession.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/PyObjCTest/test_vtvideoencoderlist.py` & `pyobjc-framework-VideoToolbox-9.2/PyObjCTest/test_vtvideoencoderlist.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/metadata/VideoToolbox.fwinfo` & `pyobjc-framework-VideoToolbox-9.2/metadata/VideoToolbox.fwinfo`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     "args": {
      "1": { "type_modifier": "o", "already_cfretained": true }
     }
    },
    "VTCompressionSessionBeginPass": {
     "args": {
      "0": {},
-     "2": {}
+     "2": { "type_modifier": "o" }
     }
    },
    "VTCompressionSessionCompleteFrames": {
     "args": {
      "0": {}
     }
    },
@@ -130,15 +130,15 @@
      }
     }
    },
    "VTCompressionSessionEndPass": {
     "args": {
      "0": {},
      "1": { "type_modifier": "o" },
-     "2": {}
+     "2": { "type_modifier": "o" }
     }
    },
    "VTCompressionSessionGetPixelBufferPool": {
     "args": {
      "0": {}
     },
     "retval": {}
```

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-VideoToolbox-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-VideoToolbox-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-VideoToolbox-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/x86_64-10.14.fwinfo` & `pyobjc-framework-VideoToolbox-9.2/metadata/raw/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-VideoToolbox-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-VideoToolbox-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-VideoToolbox-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-VideoToolbox-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-VideoToolbox-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/pyobjc_setup.py` & `pyobjc-framework-VideoToolbox-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-VideoToolbox-9.1b1/setup.py` & `pyobjc-framework-VideoToolbox-9.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
 import os
+import sys
 
-from pyobjc_setup import Extension, setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-VideoToolbox",
     description="Wrappers for the framework VideoToolbox on macOS",
     min_os_level="10.8",
     packages=["VideoToolbox"],
     ext_modules=[
```

