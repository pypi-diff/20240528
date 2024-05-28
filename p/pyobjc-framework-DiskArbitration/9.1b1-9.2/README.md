# Comparing `tmp/pyobjc-framework-DiskArbitration-9.1b1.tar.gz` & `tmp/pyobjc-framework-DiskArbitration-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-DiskArbitration-9.1b1.tar", last modified: Sun Mar 26 11:23:32 2023, max compression
+gzip compressed data, was "pyobjc-framework-DiskArbitration-9.2.tar", last modified: Wed Jun  7 00:13:38 2023, max compression
```

## Comparing `pyobjc-framework-DiskArbitration-9.1b1.tar` & `pyobjc-framework-DiskArbitration-9.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:32.701352 pyobjc-framework-DiskArbitration-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:32.671384 pyobjc-framework-DiskArbitration-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:32.680619 pyobjc-framework-DiskArbitration-9.1b1/Lib/DiskArbitration/
--rw-r--r--   0 ronald     (501) staff       (20)      745 2020-11-30 18:45:14.000000 pyobjc-framework-DiskArbitration-9.1b1/Lib/DiskArbitration/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    12364 2022-02-24 08:47:16.000000 pyobjc-framework-DiskArbitration-9.1b1/Lib/DiskArbitration/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:32.684285 pyobjc-framework-DiskArbitration-9.1b1/Lib/pyobjc_framework_DiskArbitration.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2122 2023-03-26 11:23:32.000000 pyobjc-framework-DiskArbitration-9.1b1/Lib/pyobjc_framework_DiskArbitration.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      892 2023-03-26 11:23:32.000000 pyobjc-framework-DiskArbitration-9.1b1/Lib/pyobjc_framework_DiskArbitration.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:23:32.000000 pyobjc-framework-DiskArbitration-9.1b1/Lib/pyobjc_framework_DiskArbitration.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:02.000000 pyobjc-framework-DiskArbitration-9.1b1/Lib/pyobjc_framework_DiskArbitration.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:23:32.000000 pyobjc-framework-DiskArbitration-9.1b1/Lib/pyobjc_framework_DiskArbitration.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       16 2023-03-26 11:23:32.000000 pyobjc-framework-DiskArbitration-9.1b1/Lib/pyobjc_framework_DiskArbitration.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-DiskArbitration-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-DiskArbitration-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1911 2023-03-26 11:23:32.701027 pyobjc-framework-DiskArbitration-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:32.687799 pyobjc-framework-DiskArbitration-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       30 2020-11-30 18:45:14.000000 pyobjc-framework-DiskArbitration-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     4447 2021-03-21 10:08:22.000000 pyobjc-framework-DiskArbitration-9.1b1/PyObjCTest/test_dadisk.py
--rw-r--r--   0 ronald     (501) staff       (20)     1774 2023-03-03 17:21:59.000000 pyobjc-framework-DiskArbitration-9.1b1/PyObjCTest/test_dadissenter.py
--rw-r--r--   0 ronald     (501) staff       (20)     1648 2021-03-21 10:08:22.000000 pyobjc-framework-DiskArbitration-9.1b1/PyObjCTest/test_dasession.py
--rw-r--r--   0 ronald     (501) staff       (20)     5539 2022-04-11 08:03:15.000000 pyobjc-framework-DiskArbitration-9.1b1/PyObjCTest/test_diskarbitration.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:32.689424 pyobjc-framework-DiskArbitration-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    10253 2020-11-30 18:45:14.000000 pyobjc-framework-DiskArbitration-9.1b1/metadata/DiskArbitration.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:14.000000 pyobjc-framework-DiskArbitration-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:32.700083 pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    20632 2021-07-30 09:00:37.000000 pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    20651 2022-02-24 08:47:16.000000 pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    20633 2021-03-21 10:08:22.000000 pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21893 2021-03-21 10:08:22.000000 pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21919 2021-03-21 10:08:22.000000 pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    20633 2021-07-30 09:00:37.000000 pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    20652 2022-02-24 08:47:16.000000 pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-DiskArbitration-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:23:32.701449 pyobjc-framework-DiskArbitration-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      663 2023-03-25 14:20:31.000000 pyobjc-framework-DiskArbitration-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:38.653638 pyobjc-framework-DiskArbitration-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:38.614830 pyobjc-framework-DiskArbitration-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:38.619428 pyobjc-framework-DiskArbitration-9.2/Lib/DiskArbitration/
+-rw-r--r--   0 ronald     (501) staff       (20)      745 2020-11-30 18:45:14.000000 pyobjc-framework-DiskArbitration-9.2/Lib/DiskArbitration/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12380 2023-05-27 09:46:33.000000 pyobjc-framework-DiskArbitration-9.2/Lib/DiskArbitration/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:38.622941 pyobjc-framework-DiskArbitration-9.2/Lib/pyobjc_framework_DiskArbitration.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2120 2023-06-07 00:13:38.000000 pyobjc-framework-DiskArbitration-9.2/Lib/pyobjc_framework_DiskArbitration.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      907 2023-06-07 00:13:38.000000 pyobjc-framework-DiskArbitration-9.2/Lib/pyobjc_framework_DiskArbitration.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:13:38.000000 pyobjc-framework-DiskArbitration-9.2/Lib/pyobjc_framework_DiskArbitration.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:02.000000 pyobjc-framework-DiskArbitration-9.2/Lib/pyobjc_framework_DiskArbitration.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:13:38.000000 pyobjc-framework-DiskArbitration-9.2/Lib/pyobjc_framework_DiskArbitration.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       16 2023-06-07 00:13:38.000000 pyobjc-framework-DiskArbitration-9.2/Lib/pyobjc_framework_DiskArbitration.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-DiskArbitration-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-DiskArbitration-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1909 2023-06-07 00:13:38.653189 pyobjc-framework-DiskArbitration-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:38.631134 pyobjc-framework-DiskArbitration-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2020-11-30 18:45:14.000000 pyobjc-framework-DiskArbitration-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4447 2021-03-21 10:08:22.000000 pyobjc-framework-DiskArbitration-9.2/PyObjCTest/test_dadisk.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1774 2023-03-03 17:21:59.000000 pyobjc-framework-DiskArbitration-9.2/PyObjCTest/test_dadissenter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1648 2021-03-21 10:08:22.000000 pyobjc-framework-DiskArbitration-9.2/PyObjCTest/test_dasession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5539 2023-05-27 09:46:33.000000 pyobjc-framework-DiskArbitration-9.2/PyObjCTest/test_diskarbitration.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:38.633367 pyobjc-framework-DiskArbitration-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    10253 2023-05-27 09:46:33.000000 pyobjc-framework-DiskArbitration-9.2/metadata/DiskArbitration.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:14.000000 pyobjc-framework-DiskArbitration-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:38.651876 pyobjc-framework-DiskArbitration-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    20632 2021-07-30 09:00:37.000000 pyobjc-framework-DiskArbitration-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    20651 2022-02-24 08:47:16.000000 pyobjc-framework-DiskArbitration-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    20633 2021-03-21 10:08:22.000000 pyobjc-framework-DiskArbitration-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21893 2021-03-21 10:08:22.000000 pyobjc-framework-DiskArbitration-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21919 2021-03-21 10:08:22.000000 pyobjc-framework-DiskArbitration-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    20633 2021-07-30 09:00:37.000000 pyobjc-framework-DiskArbitration-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    20652 2022-02-24 08:47:16.000000 pyobjc-framework-DiskArbitration-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-DiskArbitration-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-DiskArbitration-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:13:38.653732 pyobjc-framework-DiskArbitration-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      744 2023-05-29 10:07:46.000000 pyobjc-framework-DiskArbitration-9.2/setup.py
```

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/Lib/DiskArbitration/__init__.py` & `pyobjc-framework-DiskArbitration-9.2/Lib/DiskArbitration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/Lib/DiskArbitration/_metadata.py` & `pyobjc-framework-DiskArbitration-9.2/Lib/DiskArbitration/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sun Feb 20 18:49:14 2022
+# Last update: Sat May 20 12:07:26 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -30,14 +30,15 @@
 
 
 misc = {}
 constants = """$kDADiskDescriptionBusNameKey$kDADiskDescriptionBusPathKey$kDADiskDescriptionDeviceGUIDKey$kDADiskDescriptionDeviceInternalKey$kDADiskDescriptionDeviceModelKey$kDADiskDescriptionDevicePathKey$kDADiskDescriptionDeviceProtocolKey$kDADiskDescriptionDeviceRevisionKey$kDADiskDescriptionDeviceTDMLockedKey$kDADiskDescriptionDeviceUnitKey$kDADiskDescriptionDeviceVendorKey$kDADiskDescriptionMatchMediaUnformatted@^{__CFDictionary=}$kDADiskDescriptionMatchMediaWhole@^{__CFDictionary=}$kDADiskDescriptionMatchVolumeMountable@^{__CFDictionary=}$kDADiskDescriptionMatchVolumeUnrecognized@^{__CFDictionary=}$kDADiskDescriptionMediaBSDMajorKey$kDADiskDescriptionMediaBSDMinorKey$kDADiskDescriptionMediaBSDNameKey$kDADiskDescriptionMediaBSDUnitKey$kDADiskDescriptionMediaBlockSizeKey$kDADiskDescriptionMediaContentKey$kDADiskDescriptionMediaEjectableKey$kDADiskDescriptionMediaEncryptedKey$kDADiskDescriptionMediaEncryptionDetailKey$kDADiskDescriptionMediaIconKey$kDADiskDescriptionMediaKindKey$kDADiskDescriptionMediaLeafKey$kDADiskDescriptionMediaNameKey$kDADiskDescriptionMediaPathKey$kDADiskDescriptionMediaRemovableKey$kDADiskDescriptionMediaSizeKey$kDADiskDescriptionMediaTypeKey$kDADiskDescriptionMediaUUIDKey$kDADiskDescriptionMediaWholeKey$kDADiskDescriptionMediaWritableKey$kDADiskDescriptionVolumeKindKey$kDADiskDescriptionVolumeMountableKey$kDADiskDescriptionVolumeNameKey$kDADiskDescriptionVolumeNetworkKey$kDADiskDescriptionVolumePathKey$kDADiskDescriptionVolumeTypeKey$kDADiskDescriptionVolumeUUIDKey$kDADiskDescriptionWatchVolumeName@^{__CFArray=}$kDADiskDescriptionWatchVolumePath@^{__CFArray=}$"""
 enums = """$err_local_diskarbitration@14286848$kDADiskClaimOptionDefault@0$kDADiskEjectOptionDefault@0$kDADiskMountOptionDefault@0$kDADiskMountOptionWhole@1$kDADiskOptionDefault@0$kDADiskOptionEjectUponLogout@1$kDADiskOptionMountAutomatic@16$kDADiskOptionMountAutomaticNoDefer@32$kDADiskOptionPrivate@256$kDADiskRenameOptionDefault@0$kDADiskUnmountOptionDefault@0$kDADiskUnmountOptionForce@524288$kDADiskUnmountOptionWhole@1$kDAReturnBadArgument@-119930877$kDAReturnBusy@-119930878$kDAReturnError@-119930879$kDAReturnExclusiveAccess@-119930876$kDAReturnNoResources@-119930875$kDAReturnNotFound@-119930874$kDAReturnNotMounted@-119930873$kDAReturnNotPermitted@-119930872$kDAReturnNotPrivileged@-119930871$kDAReturnNotReady@-119930870$kDAReturnNotWritable@-119930869$kDAReturnSuccess@0$kDAReturnUnsupported@-119930868$"""
 misc.update({})
 misc.update({})
+misc.update({})
 functions = {
     "DASessionGetTypeID": (b"Q",),
     "DADiskClaim": (
         b"v^{__DADisk=}I^?^v^?^v",
         "",
         {
             "arguments": {
@@ -179,15 +180,15 @@
                         "arguments": {
                             0: {"type": b"^{__DADisk=}"},
                             1: {"type": b"^{__DADissenter=}"},
                             2: {"type": b"^v"},
                         },
                     }
                 },
-                4: {"c_array_delimited_by_null": True, "type_modifier": "n"},
+                5: {"c_array_delimited_by_null": True, "type_modifier": "n"},
             }
         },
     ),
     "DAApprovalSessionScheduleWithRunLoop": (
         b"v^{__DASession=}^{__CFRunLoop=}^{__CFString=}",
     ),
     "DAApprovalSessionGetTypeID": (b"Q",),
```

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/Lib/pyobjc_framework_DiskArbitration.egg-info/PKG-INFO` & `pyobjc-framework-DiskArbitration-9.2/Lib/pyobjc_framework_DiskArbitration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-DiskArbitration
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework DiskArbitration on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,DiskArbitration
 Platform: MacOS X
```

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/Lib/pyobjc_framework_DiskArbitration.egg-info/SOURCES.txt` & `pyobjc-framework-DiskArbitration-9.2/Lib/pyobjc_framework_DiskArbitration.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/DiskArbitration/__init__.py
 Lib/DiskArbitration/_metadata.py
 Lib/pyobjc_framework_DiskArbitration.egg-info/PKG-INFO
 Lib/pyobjc_framework_DiskArbitration.egg-info/SOURCES.txt
 Lib/pyobjc_framework_DiskArbitration.egg-info/dependency_links.txt
 Lib/pyobjc_framework_DiskArbitration.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/License.txt` & `pyobjc-framework-DiskArbitration-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/PKG-INFO` & `pyobjc-framework-DiskArbitration-9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-DiskArbitration
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework DiskArbitration on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,DiskArbitration
 Platform: MacOS X
```

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/PyObjCTest/test_dadisk.py` & `pyobjc-framework-DiskArbitration-9.2/PyObjCTest/test_dadisk.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/PyObjCTest/test_dadissenter.py` & `pyobjc-framework-DiskArbitration-9.2/PyObjCTest/test_dadissenter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/PyObjCTest/test_dasession.py` & `pyobjc-framework-DiskArbitration-9.2/PyObjCTest/test_dasession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/PyObjCTest/test_diskarbitration.py` & `pyobjc-framework-DiskArbitration-9.2/PyObjCTest/test_diskarbitration.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,16 @@
 
         self.assertArgIsFunction(
             DiskArbitration.DADiskMountWithArguments,
             3,
             b"v" + DADiskRef + DADissenterRef + b"^v",
             True,
         )
-        self.assertArgIsIn(DiskArbitration.DADiskMountWithArguments, 4)
-        self.assertArgIsNullTerminated(DiskArbitration.DADiskMountWithArguments, 4)
+        self.assertArgIsIn(DiskArbitration.DADiskMountWithArguments, 5)
+        self.assertArgIsNullTerminated(DiskArbitration.DADiskMountWithArguments, 5)
 
         self.assertArgIsFunction(
             DiskArbitration.DARegisterDiskMountApprovalCallback,
             2,
             DADissenterRef + DADiskRef + b"^v",
             True,
         )
```

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/metadata/DiskArbitration.fwinfo` & `pyobjc-framework-DiskArbitration-9.2/metadata/DiskArbitration.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -281,16 +281,16 @@
         "typestr": [
          "v",
          false
         ]
        }
       }
      },
-     "4": { "type_modifier": "n", "c_array_delimited_by_null": true },
-     "5": {}
+     "4": {},
+     "5": { "type_modifier": "n", "c_array_delimited_by_null": true }
     }
    },
    "DADiskRename": {
     "args": {
      "0": {},
      "1": {},
      "3": {
```

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-DiskArbitration-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-DiskArbitration-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-DiskArbitration-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-DiskArbitration-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-DiskArbitration-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-DiskArbitration-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-DiskArbitration-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/pyobjc_setup.py` & `pyobjc-framework-DiskArbitration-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiskArbitration-9.1b1/setup.py` & `pyobjc-framework-DiskArbitration-9.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "DiskArbitration" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
+import os
+import sys
 
-from pyobjc_setup import setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-DiskArbitration",
     description="Wrappers for the framework DiskArbitration on macOS",
     packages=["DiskArbitration"],
     version=VERSION,
     install_requires=["pyobjc-core>=" + VERSION, "pyobjc-framework-Cocoa>=" + VERSION],
```

