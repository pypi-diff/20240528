# Comparing `tmp/pyobjc-framework-CFNetwork-9.1b1.tar.gz` & `tmp/pyobjc-framework-CFNetwork-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CFNetwork-9.1b1.tar", last modified: Sun Mar 26 11:16:03 2023, max compression
+gzip compressed data, was "pyobjc-framework-CFNetwork-9.2.tar", last modified: Wed Jun  7 00:07:16 2023, max compression
```

## Comparing `pyobjc-framework-CFNetwork-9.1b1.tar` & `pyobjc-framework-CFNetwork-9.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:03.344031 pyobjc-framework-CFNetwork-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CFNetwork-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:03.241407 pyobjc-framework-CFNetwork-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:03.269297 pyobjc-framework-CFNetwork-9.1b1/Lib/CFNetwork/
--rw-r--r--   0 ronald     (501) staff       (20)     1281 2021-04-09 10:15:21.000000 pyobjc-framework-CFNetwork-9.1b1/Lib/CFNetwork/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    28084 2022-02-24 08:47:16.000000 pyobjc-framework-CFNetwork-9.1b1/Lib/CFNetwork/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:03.273914 pyobjc-framework-CFNetwork-9.1b1/Lib/pyobjc_framework_CFNetwork.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2387 2023-03-26 11:16:03.000000 pyobjc-framework-CFNetwork-9.1b1/Lib/pyobjc_framework_CFNetwork.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1181 2023-03-26 11:16:03.000000 pyobjc-framework-CFNetwork-9.1b1/Lib/pyobjc_framework_CFNetwork.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:16:03.000000 pyobjc-framework-CFNetwork-9.1b1/Lib/pyobjc_framework_CFNetwork.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:25.000000 pyobjc-framework-CFNetwork-9.1b1/Lib/pyobjc_framework_CFNetwork.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:16:03.000000 pyobjc-framework-CFNetwork-9.1b1/Lib/pyobjc_framework_CFNetwork.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:16:03.000000 pyobjc-framework-CFNetwork-9.1b1/Lib/pyobjc_framework_CFNetwork.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:03.276105 pyobjc-framework-CFNetwork-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     8304 2022-01-02 11:04:26.000000 pyobjc-framework-CFNetwork-9.1b1/Modules/_manual.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-CFNetwork-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CFNetwork-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2176 2023-03-26 11:16:03.343615 pyobjc-framework-CFNetwork-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:03.313659 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      155 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/proxy.pac
--rw-r--r--   0 ronald     (501) staff       (20)     3042 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfftpstream.py
--rw-r--r--   0 ronald     (501) staff       (20)     4127 2021-07-30 09:00:37.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfhost.py
--rw-r--r--   0 ronald     (501) staff       (20)     4954 2021-03-21 10:08:22.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfhttpauthentication.py
--rw-r--r--   0 ronald     (501) staff       (20)     5565 2021-07-30 09:00:37.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfhttpmessage.py
--rw-r--r--   0 ronald     (501) staff       (20)     2933 2021-03-21 10:08:22.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfhttpstream.py
--rw-r--r--   0 ronald     (501) staff       (20)     5765 2021-03-21 10:08:22.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfnetservices.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfnetwork.py
--rw-r--r--   0 ronald     (501) staff       (20)     1916 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfnetworkdiagnostics.py
--rw-r--r--   0 ronald     (501) staff       (20)     7335 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfnetworkerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)     7138 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfproxysupport.py
--rw-r--r--   0 ronald     (501) staff       (20)     8064 2021-04-09 10:15:21.000000 pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfsocketstream.py
--rw-r--r--   0 ronald     (501) staff       (20)      286 2021-10-18 19:38:40.000000 pyobjc-framework-CFNetwork-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:03.333875 pyobjc-framework-CFNetwork-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    16447 2021-03-21 10:08:22.000000 pyobjc-framework-CFNetwork-9.1b1/metadata/CFNetwork.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       78 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:03.342283 pyobjc-framework-CFNetwork-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    47858 2021-07-30 09:00:37.000000 pyobjc-framework-CFNetwork-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    48352 2022-02-24 08:47:16.000000 pyobjc-framework-CFNetwork-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    48972 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    47735 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    47797 2021-03-21 10:08:22.000000 pyobjc-framework-CFNetwork-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    47859 2021-07-30 09:00:37.000000 pyobjc-framework-CFNetwork-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    48353 2022-02-24 08:47:16.000000 pyobjc-framework-CFNetwork-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CFNetwork-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:16:03.344143 pyobjc-framework-CFNetwork-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1184 2023-03-25 14:20:30.000000 pyobjc-framework-CFNetwork-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:16.299584 pyobjc-framework-CFNetwork-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CFNetwork-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:16.245222 pyobjc-framework-CFNetwork-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:16.256519 pyobjc-framework-CFNetwork-9.2/Lib/CFNetwork/
+-rw-r--r--   0 ronald     (501) staff       (20)     1281 2021-04-09 10:15:21.000000 pyobjc-framework-CFNetwork-9.2/Lib/CFNetwork/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    27786 2023-05-27 09:46:33.000000 pyobjc-framework-CFNetwork-9.2/Lib/CFNetwork/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:16.260532 pyobjc-framework-CFNetwork-9.2/Lib/pyobjc_framework_CFNetwork.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2385 2023-06-07 00:07:16.000000 pyobjc-framework-CFNetwork-9.2/Lib/pyobjc_framework_CFNetwork.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1196 2023-06-07 00:07:16.000000 pyobjc-framework-CFNetwork-9.2/Lib/pyobjc_framework_CFNetwork.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:07:16.000000 pyobjc-framework-CFNetwork-9.2/Lib/pyobjc_framework_CFNetwork.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:25.000000 pyobjc-framework-CFNetwork-9.2/Lib/pyobjc_framework_CFNetwork.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:07:16.000000 pyobjc-framework-CFNetwork-9.2/Lib/pyobjc_framework_CFNetwork.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:07:16.000000 pyobjc-framework-CFNetwork-9.2/Lib/pyobjc_framework_CFNetwork.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:16.262948 pyobjc-framework-CFNetwork-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)    17233 2023-05-27 09:46:33.000000 pyobjc-framework-CFNetwork-9.2/Modules/_manual.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-CFNetwork-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CFNetwork-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2174 2023-06-07 00:07:16.299169 pyobjc-framework-CFNetwork-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:16.280307 pyobjc-framework-CFNetwork-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      155 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/proxy.pac
+-rw-r--r--   0 ronald     (501) staff       (20)     3042 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfftpstream.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4127 2021-07-30 09:00:37.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfhost.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4954 2021-03-21 10:08:22.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfhttpauthentication.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5565 2021-07-30 09:00:37.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfhttpmessage.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2933 2021-03-21 10:08:22.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfhttpstream.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5765 2021-03-21 10:08:22.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfnetservices.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfnetwork.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1916 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfnetworkdiagnostics.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7335 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfnetworkerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7138 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfproxysupport.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8064 2021-04-09 10:15:21.000000 pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfsocketstream.py
+-rw-r--r--   0 ronald     (501) staff       (20)      286 2021-10-18 19:38:40.000000 pyobjc-framework-CFNetwork-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:16.282960 pyobjc-framework-CFNetwork-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    16634 2023-05-27 09:46:33.000000 pyobjc-framework-CFNetwork-9.2/metadata/CFNetwork.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       78 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:16.297270 pyobjc-framework-CFNetwork-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    47858 2021-07-30 09:00:37.000000 pyobjc-framework-CFNetwork-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    48352 2022-02-24 08:47:16.000000 pyobjc-framework-CFNetwork-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    48972 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    47735 2020-11-30 18:45:14.000000 pyobjc-framework-CFNetwork-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    47797 2021-03-21 10:08:22.000000 pyobjc-framework-CFNetwork-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    47859 2021-07-30 09:00:37.000000 pyobjc-framework-CFNetwork-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    48353 2022-02-24 08:47:16.000000 pyobjc-framework-CFNetwork-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CFNetwork-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CFNetwork-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:07:16.299679 pyobjc-framework-CFNetwork-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1266 2023-05-29 10:07:45.000000 pyobjc-framework-CFNetwork-9.2/setup.py
```

### Comparing `pyobjc-framework-CFNetwork-9.1b1/LICENSE.txt` & `pyobjc-framework-CFNetwork-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/Lib/CFNetwork/__init__.py` & `pyobjc-framework-CFNetwork-9.2/Lib/CFNetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/Lib/CFNetwork/_metadata.py` & `pyobjc-framework-CFNetwork-9.2/Lib/CFNetwork/_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sun Feb 20 18:30:45 2022
+# Last update: Fri May 19 21:48:40 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -44,14 +44,15 @@
         "CFNetServiceRegisterFlags": NewType("CFNetServiceRegisterFlags", int),
         "CFNetDiagnosticStatusValues": NewType("CFNetDiagnosticStatusValues", int),
         "CFHostInfoType": NewType("CFHostInfoType", int),
         "CFNetworkErrors": NewType("CFNetworkErrors", int),
     }
 )
 misc.update({})
+misc.update({})
 functions = {
     "CFNetworkExecuteProxyAutoConfigurationURL": (
         b"^{__CFRunLoopSource=}^{__CFURL=}^{__CFURL=}^?^{_CFStreamClientContext=q^v^?^?^?}",
         "",
         {
             "arguments": {
                 2: {
@@ -95,19 +96,25 @@
     "CFHostCreateWithAddress": (
         b"^{__CFHost=}^{__CFAllocator=}^{__CFData=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CFNetServiceBrowserSearchForDomains": (
         b"Z^{__CFNetServiceBrowser=}Z^{_CFStreamError=qi}",
+        "",
+        {"arguments": {2: {"type_modifier": "o"}}},
     ),
     "CFNetServiceUnscheduleFromRunLoop": (
         b"v^{__CFNetService=}^{__CFRunLoop=}^{__CFString=}",
     ),
-    "CFNetServiceMonitorStop": (b"v^{__CFNetServiceMonitor=}^{_CFStreamError=qi}",),
+    "CFNetServiceMonitorStop": (
+        b"v^{__CFNetServiceMonitor=}^{_CFStreamError=qi}",
+        "",
+        {"arguments": {1: {"type_modifier": "o"}}},
+    ),
     "CFNetworkCopySystemProxySettings": (
         b"^{__CFDictionary=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CFHostGetReachability": (
         b"^{__CFData=}^{__CFHost=}^Z",
@@ -187,15 +194,19 @@
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CFNetServiceMonitorUnscheduleFromRunLoop": (
         b"v^{__CFNetServiceMonitor=}^{__CFRunLoop=}^{__CFString=}",
     ),
     "CFHostScheduleWithRunLoop": (b"v^{__CFHost=}^{__CFRunLoop=}^{__CFString=}",),
-    "CFNetServiceMonitorStart": (b"Z^{__CFNetServiceMonitor=}i^{_CFStreamError=qi}",),
+    "CFNetServiceMonitorStart": (
+        b"Z^{__CFNetServiceMonitor=}i^{_CFStreamError=qi}",
+        "",
+        {"arguments": {2: {"type_modifier": "o"}}},
+    ),
     "CFHostGetNames": (
         b"^{__CFArray=}^{__CFHost=}^Z",
         "",
         {"arguments": {1: {"type_modifier": "o"}}},
     ),
     "CFNetDiagnosticCopyNetworkStatusPassively": (
         b"q^{__CFNetDiagnostic=}^^{__CFString=}",
@@ -277,14 +288,16 @@
     "CFNetServiceBrowserInvalidate": (b"v^{__CFNetServiceBrowser=}",),
     "CFNetServiceGetAddressing": (b"^{__CFArray=}^{__CFNetService=}",),
     "CFHTTPMessageSetHeaderFieldValue": (
         b"v^{__CFHTTPMessage=}^{__CFString=}^{__CFString=}",
     ),
     "CFNetServiceBrowserStopSearch": (
         b"v^{__CFNetServiceBrowser=}^{_CFStreamError=qi}",
+        "",
+        {"arguments": {1: {"type_modifier": "o"}}},
     ),
     "CFHTTPMessageApplyCredentials": (
         b"Z^{__CFHTTPMessage=}^{_CFHTTPAuthentication=}^{__CFString=}^{__CFString=}^{_CFStreamError=qi}",
         "",
         {"arguments": {4: {"type_modifier": "o"}}},
     ),
     "CFHTTPReadStreamSetRedirectsAutomatically": (b"v^{__CFReadStream=}Z",),
@@ -294,35 +307,14 @@
         {"arguments": {2: {"type_modifier": "o"}}},
     ),
     "CFHTTPAuthenticationCopyMethod": (
         b"^{__CFString=}^{_CFHTTPAuthentication=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
-    "CFNetServiceBrowserCreate": (
-        b"^{__CFNetServiceBrowser=}^{__CFAllocator=}^?^{CFNetServiceClientContext=q^v^?^?^?}",
-        "",
-        {
-            "retval": {"already_cfretained": True},
-            "arguments": {
-                1: {
-                    "callable": {
-                        "retval": {"type": b"v"},
-                        "arguments": {
-                            0: {"type": b"^{__CFNetServiceBrowser=}"},
-                            1: {"type": b"Q"},
-                            2: {"type": b"@"},
-                            3: {"type": b"^{_CFStreamError=qi}"},
-                            4: {"type": b"^v"},
-                        },
-                    }
-                }
-            },
-        },
-    ),
     "CFNetServiceGetTargetHost": (b"^{__CFString=}^{__CFNetService=}",),
     "CFNetworkCopyProxiesForAutoConfigurationScript": (
         b"^{__CFArray=}^{__CFString=}^{__CFURL=}^^{__CFError=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {
@@ -335,15 +327,19 @@
         },
     ),
     "CFNetServiceCreateDictionaryWithTXTData": (
         b"^{__CFDictionary=}^{__CFAllocator=}^{__CFData=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
-    "CFNetServiceRegister": (b"Z^{__CFNetService=}^{_CFStreamError=qi}",),
+    "CFNetServiceRegister": (
+        b"Z^{__CFNetService=}^{_CFStreamError=qi}",
+        "",
+        {"arguments": {1: {"type_modifier": "o"}}},
+    ),
     "CFHTTPMessageCopySerializedMessage": (
         b"^{__CFData=}^{__CFHTTPMessage=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CFHostCreateCopy": (
         b"^{__CFHost=}^{__CFAllocator=}^{__CFHost=}",
@@ -423,15 +419,19 @@
     "CFHostUnscheduleFromRunLoop": (b"v^{__CFHost=}^{__CFRunLoop=}^{__CFString=}",),
     "CFHTTPMessageApplyCredentialDictionary": (
         b"Z^{__CFHTTPMessage=}^{_CFHTTPAuthentication=}^{__CFDictionary=}^{_CFStreamError=qi}",
         "",
         {"arguments": {3: {"type_modifier": "o"}}},
     ),
     "CFHTTPMessageIsRequest": (b"Z^{__CFHTTPMessage=}",),
-    "CFNetServiceResolve": (b"Z^{__CFNetService=}^{_CFStreamError=qi}",),
+    "CFNetServiceResolve": (
+        b"Z^{__CFNetService=}^{_CFStreamError=qi}",
+        "",
+        {"arguments": {1: {"type_modifier": "o"}}},
+    ),
     "CFHTTPMessageCopyBody": (
         b"^{__CFData=}^{__CFHTTPMessage=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CFNetServiceBrowserScheduleWithRunLoop": (
         b"v^{__CFNetServiceBrowser=}^{__CFRunLoop=}^{__CFString=}",
```

### Comparing `pyobjc-framework-CFNetwork-9.1b1/Lib/pyobjc_framework_CFNetwork.egg-info/PKG-INFO` & `pyobjc-framework-CFNetwork-9.2/Lib/pyobjc_framework_CFNetwork.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CFNetwork
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CFNetwork on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CFNetwork
 Platform: MacOS X
```

### Comparing `pyobjc-framework-CFNetwork-9.1b1/Lib/pyobjc_framework_CFNetwork.egg-info/SOURCES.txt` & `pyobjc-framework-CFNetwork-9.2/Lib/pyobjc_framework_CFNetwork.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CFNetwork/__init__.py
 Lib/CFNetwork/_metadata.py
 Lib/pyobjc_framework_CFNetwork.egg-info/PKG-INFO
 Lib/pyobjc_framework_CFNetwork.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CFNetwork.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CFNetwork.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CFNetwork-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CFNetwork-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CFNetwork-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CFNetwork-9.1b1/PKG-INFO` & `pyobjc-framework-CFNetwork-9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CFNetwork
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CFNetwork on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CFNetwork
 Platform: MacOS X
```

### Comparing `pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfftpstream.py` & `pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfftpstream.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfhost.py` & `pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfhost.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfhttpauthentication.py` & `pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfhttpauthentication.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfhttpmessage.py` & `pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfhttpmessage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfhttpstream.py` & `pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfhttpstream.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfnetservices.py` & `pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfnetservices.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfnetworkdiagnostics.py` & `pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfnetworkdiagnostics.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfnetworkerrors.py` & `pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfnetworkerrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfproxysupport.py` & `pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfproxysupport.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/PyObjCTest/test_cfsocketstream.py` & `pyobjc-framework-CFNetwork-9.2/PyObjCTest/test_cfsocketstream.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/metadata/CFNetwork.fwinfo` & `pyobjc-framework-CFNetwork-9.2/metadata/CFNetwork.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -462,14 +462,15 @@
    "CFNetDiagnosticSetName": {
     "args": {
      "0": {},
      "1": {}
     }
    },
    "CFNetServiceBrowserCreate": {
+    "ignore": true,
     "args": {
      "0": {},
      "1": {
       "function": {
        "args": [
         {
          "typestr": "^{__CFNetServiceBrowser=}"
@@ -509,29 +510,29 @@
      "1": {},
      "2": {}
     }
    },
    "CFNetServiceBrowserSearchForDomains": {
     "args": {
      "0": {},
-     "2": {}
+     "2": {"type_modifier": "o" }
     }
    },
    "CFNetServiceBrowserSearchForServices": {
     "args": {
      "0": {},
      "1": {},
      "2": {},
      "3": { "type_modifier": "o" }
     }
    },
    "CFNetServiceBrowserStopSearch": {
     "args": {
      "0": {},
-     "1": {}
+     "1": {"type_modifier": "o" }
     }
    },
    "CFNetServiceBrowserUnscheduleFromRunLoop": {
     "args": {
      "0": {},
      "1": {},
      "2": {}
@@ -628,14 +629,15 @@
    "CFNetServiceGetType": {
     "args": {
      "0": {}
     },
     "retval": {}
    },
    "CFNetServiceMonitorCreate": {
+    "ignore": true,
     "args": {
      "0": {},
      "1": {},
      "2": {
       "function": {
        "args": [
         {
@@ -679,46 +681,46 @@
      "1": {},
      "2": {}
     }
    },
    "CFNetServiceMonitorStart": {
     "args": {
      "0": {},
-     "2": {}
+     "2": { "type_modifier": "o"}
     }
    },
    "CFNetServiceMonitorStop": {
     "args": {
      "0": {},
-     "1": {}
+     "1": { "type_modifier": "o"}
     }
    },
    "CFNetServiceMonitorUnscheduleFromRunLoop": {
     "args": {
      "0": {},
      "1": {},
      "2": {}
     }
    },
    "CFNetServiceRegister": {
     "args": {
      "0": {},
-     "1": {}
+     "1": { "type_modifier": "o" }
     }
    },
    "CFNetServiceRegisterWithOptions": {
     "args": {
      "0": {},
      "2": { "type_modifier": "o" }
     }
    },
    "CFNetServiceResolve": {
     "args": {
      "0": {},
-     "1": {}
+     "1": { "type_modifier": "o"}
     }
    },
    "CFNetServiceResolveWithTimeout": {
     "args": {
      "0": {},
      "2": { "type_modifier": "o" }
     }
@@ -727,14 +729,15 @@
     "args": {
      "0": {},
      "1": {},
      "2": {}
     }
    },
    "CFNetServiceSetClient": {
+    "ignore": true,
     "args": {
      "0": {},
      "1": {
       "function": {
        "args": [
         {
          "typestr": "^{__CFNetService=}"
```

### Comparing `pyobjc-framework-CFNetwork-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CFNetwork-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CFNetwork-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-CFNetwork-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-CFNetwork-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CFNetwork-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CFNetwork-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CFNetwork-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CFNetwork-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CFNetwork-9.1b1/setup.py` & `pyobjc-framework-CFNetwork-9.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,23 @@
 diagnostics.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
-from pyobjc_setup import Extension, setup
+import os
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-CFNetwork",
     description="Wrappers for the framework CFNetwork on macOS",
     packages=["CFNetwork"],
     ext_modules=[
         Extension(
```

