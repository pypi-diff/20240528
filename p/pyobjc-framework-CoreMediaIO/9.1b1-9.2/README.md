# Comparing `tmp/pyobjc-framework-CoreMediaIO-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreMediaIO-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreMediaIO-9.1b1.tar", last modified: Sun Mar 26 11:21:30 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreMediaIO-9.2.tar", last modified: Wed Jun  7 00:11:30 2023, max compression
```

## Comparing `pyobjc-framework-CoreMediaIO-9.1b1.tar` & `pyobjc-framework-CoreMediaIO-9.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:30.747658 pyobjc-framework-CoreMediaIO-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:30.711340 pyobjc-framework-CoreMediaIO-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:30.716849 pyobjc-framework-CoreMediaIO-9.1b1/Lib/CoreMediaIO/
--rw-r--r--   0 ronald     (501) staff       (20)     1229 2021-04-09 10:15:21.000000 pyobjc-framework-CoreMediaIO-9.1b1/Lib/CoreMediaIO/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    33242 2022-02-24 21:31:40.000000 pyobjc-framework-CoreMediaIO-9.1b1/Lib/CoreMediaIO/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:30.726595 pyobjc-framework-CoreMediaIO-9.1b1/Lib/pyobjc_framework_CoreMediaIO.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2115 2023-03-26 11:21:30.000000 pyobjc-framework-CoreMediaIO-9.1b1/Lib/pyobjc_framework_CoreMediaIO.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1290 2023-03-26 11:21:30.000000 pyobjc-framework-CoreMediaIO-9.1b1/Lib/pyobjc_framework_CoreMediaIO.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:21:30.000000 pyobjc-framework-CoreMediaIO-9.1b1/Lib/pyobjc_framework_CoreMediaIO.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:52.000000 pyobjc-framework-CoreMediaIO-9.1b1/Lib/pyobjc_framework_CoreMediaIO.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:21:30.000000 pyobjc-framework-CoreMediaIO-9.1b1/Lib/pyobjc_framework_CoreMediaIO.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       12 2023-03-26 11:21:30.000000 pyobjc-framework-CoreMediaIO-9.1b1/Lib/pyobjc_framework_CoreMediaIO.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreMediaIO-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMediaIO-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:30.728430 pyobjc-framework-CoreMediaIO-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     3617 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.1b1/Modules/_CoreMediaIO.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreMediaIO-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreMediaIO-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1904 2023-03-26 11:21:30.747340 pyobjc-framework-CoreMediaIO-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:30.736704 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1269 2022-06-25 20:12:27.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmioextensiondevice.py
--rw-r--r--   0 ronald     (501) staff       (20)     2349 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmioextensionproperties.py
--rw-r--r--   0 ronald     (501) staff       (20)     1779 2022-06-25 20:10:20.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmioextensionprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)     3000 2022-06-25 20:10:02.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmioextensionstream.py
--rw-r--r--   0 ronald     (501) staff       (20)     1637 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiohardware.py
--rw-r--r--   0 ronald     (501) staff       (20)     6679 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiohardwarecontrol.py
--rw-r--r--   0 ronald     (501) staff       (20)    10069 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiohardwaredevice.py
--rw-r--r--   0 ronald     (501) staff       (20)     4285 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiohardwareobject.py
--rw-r--r--   0 ronald     (501) staff       (20)     7602 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiohardwarestream.py
--rw-r--r--   0 ronald     (501) staff       (20)     1915 2021-07-31 13:27:21.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiohardwaresystem.py
--rw-r--r--   0 ronald     (501) staff       (20)     9419 2021-04-09 10:15:21.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiosamplebuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)      206 2022-04-11 08:03:15.000000 pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_coremediaio.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:30.738335 pyobjc-framework-CoreMediaIO-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     7932 2022-02-24 21:31:25.000000 pyobjc-framework-CoreMediaIO-9.1b1/metadata/CoreMediaIO.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      572 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:30.746000 pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    35268 2021-07-30 09:00:37.000000 pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    94604 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    34323 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    34750 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    34861 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    34861 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    35269 2021-07-30 09:00:37.000000 pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    94605 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreMediaIO-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:21:30.747920 pyobjc-framework-CoreMediaIO-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      966 2023-03-25 14:20:31.000000 pyobjc-framework-CoreMediaIO-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:30.345457 pyobjc-framework-CoreMediaIO-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:30.292036 pyobjc-framework-CoreMediaIO-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:30.299387 pyobjc-framework-CoreMediaIO-9.2/Lib/CoreMediaIO/
+-rw-r--r--   0 ronald     (501) staff       (20)     1229 2021-04-09 10:15:21.000000 pyobjc-framework-CoreMediaIO-9.2/Lib/CoreMediaIO/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    33005 2023-05-13 09:51:01.000000 pyobjc-framework-CoreMediaIO-9.2/Lib/CoreMediaIO/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:30.303907 pyobjc-framework-CoreMediaIO-9.2/Lib/pyobjc_framework_CoreMediaIO.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2113 2023-06-07 00:11:30.000000 pyobjc-framework-CoreMediaIO-9.2/Lib/pyobjc_framework_CoreMediaIO.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1305 2023-06-07 00:11:30.000000 pyobjc-framework-CoreMediaIO-9.2/Lib/pyobjc_framework_CoreMediaIO.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:11:30.000000 pyobjc-framework-CoreMediaIO-9.2/Lib/pyobjc_framework_CoreMediaIO.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:52.000000 pyobjc-framework-CoreMediaIO-9.2/Lib/pyobjc_framework_CoreMediaIO.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:11:30.000000 pyobjc-framework-CoreMediaIO-9.2/Lib/pyobjc_framework_CoreMediaIO.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       12 2023-06-07 00:11:30.000000 pyobjc-framework-CoreMediaIO-9.2/Lib/pyobjc_framework_CoreMediaIO.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreMediaIO-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMediaIO-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:30.305536 pyobjc-framework-CoreMediaIO-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     3617 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.2/Modules/_CoreMediaIO.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreMediaIO-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CoreMediaIO-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1902 2023-06-07 00:11:30.345019 pyobjc-framework-CoreMediaIO-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:30.325670 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1269 2022-06-25 20:12:27.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmioextensiondevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2349 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmioextensionproperties.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1779 2022-06-25 20:10:20.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmioextensionprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3000 2022-06-25 20:10:02.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmioextensionstream.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1637 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiohardware.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6679 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiohardwarecontrol.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10069 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiohardwaredevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4647 2023-05-13 09:51:01.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiohardwareobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7602 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiohardwarestream.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1915 2021-07-31 13:27:21.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiohardwaresystem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9419 2021-04-09 10:15:21.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiosamplebuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      206 2022-04-11 08:03:15.000000 pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_coremediaio.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:30.327294 pyobjc-framework-CoreMediaIO-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     8170 2023-05-13 09:51:01.000000 pyobjc-framework-CoreMediaIO-9.2/metadata/CoreMediaIO.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      572 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:30.343535 pyobjc-framework-CoreMediaIO-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    35268 2021-07-30 09:00:37.000000 pyobjc-framework-CoreMediaIO-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    94604 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    34323 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMediaIO-9.2/metadata/raw/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    34750 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMediaIO-9.2/metadata/raw/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    34861 2020-11-30 18:45:14.000000 pyobjc-framework-CoreMediaIO-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    34861 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMediaIO-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    35269 2021-07-30 09:00:37.000000 pyobjc-framework-CoreMediaIO-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    94605 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMediaIO-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreMediaIO-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreMediaIO-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:11:30.345555 pyobjc-framework-CoreMediaIO-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1047 2023-05-29 10:07:46.000000 pyobjc-framework-CoreMediaIO-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/Lib/CoreMediaIO/__init__.py` & `pyobjc-framework-CoreMediaIO-9.2/Lib/CoreMediaIO/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/Lib/CoreMediaIO/_metadata.py` & `pyobjc-framework-CoreMediaIO-9.2/Lib/CoreMediaIO/_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Mon Feb 21 22:38:40 2022
+# Last update: Sat May 13 11:46:09 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -254,40 +254,39 @@
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {6: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
     "CMIOStreamClockInvalidate": (b"i@",),
-    "CMIOObjectsPublishedAndDied": (
-        b"i^^{CMIOHardwarePlugInInterface=^v^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?}II^II^I",
+    "CMIOObjectSetPropertyData": (
+        b"iI^{CMIOObjectPropertyAddress=III}I^vI^v",
+        "",
+        {
+            "arguments": {
+                1: {"type_modifier": "n"},
+                3: {"c_array_length_in_arg": 2, "type_modifier": "n"},
+                5: {"c_array_length_in_arg": 4, "type_modifier": "n"},
+            }
+        },
     ),
-    "CMIOObjectSetPropertyData": (b"iI^{CMIOObjectPropertyAddress=III}I^vI^v",),
     "CMIOSampleBufferGetDiscontinuityFlags": (b"I^{opaqueCMSampleBuffer=}",),
     "CMIOStreamDeckPlay": (b"iI",),
     "CMIOSampleBufferSetDiscontinuityFlags": (
         b"v^{__CFAllocator=}^{opaqueCMSampleBuffer=}I",
     ),
     "CMIOStreamDeckStop": (b"iI",),
-    "CMIOObjectPropertiesChanged": (
-        b"i^^{CMIOHardwarePlugInInterface=^v^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?}II^{CMIOObjectPropertyAddress=III}",
-    ),
     "CMIOSampleBufferSetSequenceNumber": (
         b"v^{__CFAllocator=}^{opaqueCMSampleBuffer=}Q",
     ),
     "CMIOSampleBufferCopySampleAttachments": (
         b"i^{opaqueCMSampleBuffer=}^{opaqueCMSampleBuffer=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
-    "CMIOObjectCreate": (
-        b"i^^{CMIOHardwarePlugInInterface=^v^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?^?}II^I",
-        "",
-        {"retval": {"already_cfretained": True}},
-    ),
     "CMIOStreamClockConvertHostTimeToDeviceTime": (b"{_CMTime=qiIq}Q@",),
     "CMIOObjectRemovePropertyListenerBlock": (
         b"iI^{CMIOObjectPropertyAddress=III}@@?",
         "",
         {
             "arguments": {
                 1: {"type_modifier": "n"},
```

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/Lib/pyobjc_framework_CoreMediaIO.egg-info/PKG-INFO` & `pyobjc-framework-CoreMediaIO-9.2/Lib/pyobjc_framework_CoreMediaIO.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreMediaIO
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreMediaIO on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreMediaIO
 Platform: MacOS X (>=10.7)
```

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/Lib/pyobjc_framework_CoreMediaIO.egg-info/SOURCES.txt` & `pyobjc-framework-CoreMediaIO-9.2/Lib/pyobjc_framework_CoreMediaIO.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CoreMediaIO/__init__.py
 Lib/CoreMediaIO/_metadata.py
 Lib/pyobjc_framework_CoreMediaIO.egg-info/PKG-INFO
 Lib/pyobjc_framework_CoreMediaIO.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CoreMediaIO.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CoreMediaIO.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/License.txt` & `pyobjc-framework-CoreMediaIO-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/Modules/_CoreMediaIO.m` & `pyobjc-framework-CoreMediaIO-9.2/Modules/_CoreMediaIO.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreMediaIO-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreMediaIO-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/PKG-INFO` & `pyobjc-framework-CoreMediaIO-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreMediaIO
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreMediaIO on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreMediaIO
 Platform: MacOS X (>=10.7)
```

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmioextensiondevice.py` & `pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmioextensiondevice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmioextensionproperties.py` & `pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmioextensionproperties.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmioextensionprovider.py` & `pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmioextensionprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmioextensionstream.py` & `pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmioextensionstream.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiohardware.py` & `pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiohardware.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiohardwarecontrol.py` & `pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiohardwarecontrol.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiohardwaredevice.py` & `pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiohardwaredevice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiohardwareobject.py` & `pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiohardwareobject.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,7 +89,13 @@
 
         self.assertArgIsIn(CoreMediaIO.CMIOObjectRemovePropertyListenerBlock, 1)
         self.assertArgIsBlock(
             CoreMediaIO.CMIOObjectRemovePropertyListenerBlock,
             3,
             CMIOObjectPropertyListenerBlock,
         )
+
+        self.assertArgIsIn(CoreMediaIO.CMIOObjectSetPropertyData, 1)
+        self.assertArgIsIn(CoreMediaIO.CMIOObjectSetPropertyData, 3)
+        self.assertArgSizeInArg(CoreMediaIO.CMIOObjectSetPropertyData, 3, 2)
+        self.assertArgIsIn(CoreMediaIO.CMIOObjectSetPropertyData, 5)
+        self.assertArgSizeInArg(CoreMediaIO.CMIOObjectSetPropertyData, 5, 4)
```

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiohardwarestream.py` & `pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiohardwarestream.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiohardwaresystem.py` & `pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiohardwaresystem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/PyObjCTest/test_cmiosamplebuffer.py` & `pyobjc-framework-CoreMediaIO-9.2/PyObjCTest/test_cmiosamplebuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/metadata/CoreMediaIO.fwinfo` & `pyobjc-framework-CoreMediaIO-9.2/metadata/CoreMediaIO.fwinfo`

 * *Files 2% similar despite different names*

```diff
@@ -8,44 +8,44 @@
   "classes": {
    "CMIOExtensionProvider": {
     "methods": [
      {
       "selector": "addDevice:error:",
       "class_method": false,
       "args": {
-       "0": { "type_modifier": "o" }
+       "1": { "type_modifier": "o" }
       }
      },
      {
       "selector": "removeDevice:error:",
       "class_method": false,
       "args": {
-       "0": { "type_modifier": "o" }
+       "1": { "type_modifier": "o" }
       }
      }
     ]
-   }
+   },
    "CMIOExtensionDevice": {
     "methods": [
      {
       "selector": "addStream:error:",
       "class_method": false,
       "args": {
-       "0": { "type_modifier": "o" }
+       "1": { "type_modifier": "o" }
       }
      },
      {
       "selector": "removeStream:error:",
       "class_method": false,
       "args": {
-       "0": { "type_modifier": "o" }
+       "1": { "type_modifier": "o" }
       }
      }
     ]
-   }
+   },
    "NSObject": {
     "methods": [
      {
       "selector": "startStreamAndReturnError:",
       "class_method": false,
       "args": {
        "0": { "type_modifier": "o" }
@@ -114,14 +114,15 @@
   "enum": {
    "kCMIOZoomRelativeControlClassID": { "value": 2054122866 },
    "kCMIOInvalidSequenceNumber": { "value": 18446744073709551615 },
    "kCMIOPanTiltRelativeControlClassID": { "value": 1886679660  },
    "kCMIOPanTiltAbsoluteControlClassID": { "value": 1886675298  }
   },
   "structs": {
+   "CMIOHardwarePlugInInterface": { "ignore": true },
    "CMIOStreamScheduledOutputNotificationProcAndRefCon": {
     "fieldnames": [
      "scheduledOutputNotificationProc",
      "scheduledOutputNotificationRefCon"
     ],
     "special": false,
     "typestr": "{CMIOStreamScheduledOutputNotificationProcAndRefCon=^?^?}"
@@ -185,14 +186,15 @@
        },
        "retval": { "type": "v" }
       }
      }
     }
    },
    "CMIOObjectCreate": {
+    "ignore": true,
     "args": {
      "0": {},
      "3": {}
     }
    },
    "CMIOObjectGetPropertyData": {
     "args": {
@@ -217,14 +219,15 @@
    "CMIOObjectIsPropertySettable": {
     "args": {
      "1": { "type_modifier": "n" },
      "2": { "type_modifier": "o" }
     }
    },
    "CMIOObjectPropertiesChanged": {
+    "ignore": true,
     "args": {
      "0": {},
      "3": {}
     }
    },
    "CMIOObjectRemovePropertyListener": {
     "args": {
@@ -266,20 +269,21 @@
        "retval": { "type": "v" }
       }
      }
     }
    },
    "CMIOObjectSetPropertyData": {
     "args": {
-     "1": {},
-     "3": {},
-     "5": {}
+     "1": { "type_modifier": "n" },
+     "3": { "type_modifier": "n", "c_array_length_in_arg": 2 },
+     "5": { "type_modifier": "n", "c_array_length_in_arg": 4 }
     }
    },
    "CMIOObjectsPublishedAndDied": {
+    "ignore": true,
     "args": {
      "0": {},
      "3": {},
      "5": {}
     }
    },
    "CMIOSampleBufferCopyNonRequiredAttachments": {
```

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/metadata/metadata.ini` & `pyobjc-framework-CoreMediaIO-9.2/metadata/metadata.ini`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CoreMediaIO-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreMediaIO-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/x86_64-10.13.fwinfo` & `pyobjc-framework-CoreMediaIO-9.2/metadata/raw/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/x86_64-10.14.fwinfo` & `pyobjc-framework-CoreMediaIO-9.2/metadata/raw/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreMediaIO-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreMediaIO-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreMediaIO-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreMediaIO-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMediaIO-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreMediaIO-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

