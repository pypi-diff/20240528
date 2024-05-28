# Comparing `tmp/pyobjc-framework-DVDPlayback-9.1b1.tar.gz` & `tmp/pyobjc-framework-DVDPlayback-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-DVDPlayback-9.1b1.tar", last modified: Sun Mar 26 11:22:58 2023, max compression
+gzip compressed data, was "pyobjc-framework-DVDPlayback-9.2.tar", last modified: Wed Jun  7 00:13:01 2023, max compression
```

## Comparing `pyobjc-framework-DVDPlayback-9.1b1.tar` & `pyobjc-framework-DVDPlayback-9.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:58.491384 pyobjc-framework-DVDPlayback-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:58.465011 pyobjc-framework-DVDPlayback-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:58.469471 pyobjc-framework-DVDPlayback-9.1b1/Lib/DVDPlayback/
--rw-r--r--   0 ronald     (501) staff       (20)      709 2020-11-30 18:45:14.000000 pyobjc-framework-DVDPlayback-9.1b1/Lib/DVDPlayback/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    22066 2022-04-12 19:30:26.000000 pyobjc-framework-DVDPlayback-9.1b1/Lib/DVDPlayback/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:58.473328 pyobjc-framework-DVDPlayback-9.1b1/Lib/pyobjc_framework_DVDPlayback.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2115 2023-03-26 11:22:58.000000 pyobjc-framework-DVDPlayback-9.1b1/Lib/pyobjc_framework_DVDPlayback.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      735 2023-03-26 11:22:58.000000 pyobjc-framework-DVDPlayback-9.1b1/Lib/pyobjc_framework_DVDPlayback.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:22:58.000000 pyobjc-framework-DVDPlayback-9.1b1/Lib/pyobjc_framework_DVDPlayback.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:58.000000 pyobjc-framework-DVDPlayback-9.1b1/Lib/pyobjc_framework_DVDPlayback.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:22:58.000000 pyobjc-framework-DVDPlayback-9.1b1/Lib/pyobjc_framework_DVDPlayback.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       12 2023-03-26 11:22:58.000000 pyobjc-framework-DVDPlayback-9.1b1/Lib/pyobjc_framework_DVDPlayback.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-DVDPlayback-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-DVDPlayback-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1904 2023-03-26 11:22:58.491035 pyobjc-framework-DVDPlayback-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:58.476424 pyobjc-framework-DVDPlayback-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-DVDPlayback-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    32373 2022-04-11 08:03:15.000000 pyobjc-framework-DVDPlayback-9.1b1/PyObjCTest/test_dvdplayback.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:58.478667 pyobjc-framework-DVDPlayback-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     8991 2022-04-12 19:30:13.000000 pyobjc-framework-DVDPlayback-9.1b1/metadata/DVDPlayback.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       38 2020-11-30 18:45:14.000000 pyobjc-framework-DVDPlayback-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:58.489675 pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    35299 2021-07-30 09:00:37.000000 pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    35751 2022-02-24 08:47:16.000000 pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    35285 2020-11-30 18:45:14.000000 pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    35300 2021-03-21 10:08:22.000000 pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    35300 2021-07-30 09:00:37.000000 pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    35752 2022-02-24 08:47:16.000000 pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-DVDPlayback-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:22:58.491647 pyobjc-framework-DVDPlayback-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      672 2023-03-25 14:20:31.000000 pyobjc-framework-DVDPlayback-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:01.702956 pyobjc-framework-DVDPlayback-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:01.677206 pyobjc-framework-DVDPlayback-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:01.682134 pyobjc-framework-DVDPlayback-9.2/Lib/DVDPlayback/
+-rw-r--r--   0 ronald     (501) staff       (20)      709 2020-11-30 18:45:14.000000 pyobjc-framework-DVDPlayback-9.2/Lib/DVDPlayback/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    22124 2023-05-27 09:46:33.000000 pyobjc-framework-DVDPlayback-9.2/Lib/DVDPlayback/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:01.686382 pyobjc-framework-DVDPlayback-9.2/Lib/pyobjc_framework_DVDPlayback.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2113 2023-06-07 00:13:01.000000 pyobjc-framework-DVDPlayback-9.2/Lib/pyobjc_framework_DVDPlayback.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      750 2023-06-07 00:13:01.000000 pyobjc-framework-DVDPlayback-9.2/Lib/pyobjc_framework_DVDPlayback.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:13:01.000000 pyobjc-framework-DVDPlayback-9.2/Lib/pyobjc_framework_DVDPlayback.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:58.000000 pyobjc-framework-DVDPlayback-9.2/Lib/pyobjc_framework_DVDPlayback.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:13:01.000000 pyobjc-framework-DVDPlayback-9.2/Lib/pyobjc_framework_DVDPlayback.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       12 2023-06-07 00:13:01.000000 pyobjc-framework-DVDPlayback-9.2/Lib/pyobjc_framework_DVDPlayback.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-DVDPlayback-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-DVDPlayback-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1902 2023-06-07 00:13:01.702529 pyobjc-framework-DVDPlayback-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:01.691125 pyobjc-framework-DVDPlayback-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-DVDPlayback-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    32373 2022-04-11 08:03:15.000000 pyobjc-framework-DVDPlayback-9.2/PyObjCTest/test_dvdplayback.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:01.692798 pyobjc-framework-DVDPlayback-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     9035 2023-05-27 09:46:33.000000 pyobjc-framework-DVDPlayback-9.2/metadata/DVDPlayback.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2020-11-30 18:45:14.000000 pyobjc-framework-DVDPlayback-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:01.699878 pyobjc-framework-DVDPlayback-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    35299 2021-07-30 09:00:37.000000 pyobjc-framework-DVDPlayback-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    35751 2022-02-24 08:47:16.000000 pyobjc-framework-DVDPlayback-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    35285 2020-11-30 18:45:14.000000 pyobjc-framework-DVDPlayback-9.2/metadata/raw/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    35300 2021-03-21 10:08:22.000000 pyobjc-framework-DVDPlayback-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    35300 2021-07-30 09:00:37.000000 pyobjc-framework-DVDPlayback-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    35752 2022-02-24 08:47:16.000000 pyobjc-framework-DVDPlayback-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-DVDPlayback-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-DVDPlayback-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:13:01.703056 pyobjc-framework-DVDPlayback-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      754 2023-05-29 10:07:46.000000 pyobjc-framework-DVDPlayback-9.2/setup.py
```

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/Lib/DVDPlayback/__init__.py` & `pyobjc-framework-DVDPlayback-9.2/Lib/DVDPlayback/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/Lib/DVDPlayback/_metadata.py` & `pyobjc-framework-DVDPlayback-9.2/Lib/DVDPlayback/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sun Feb 20 18:48:18 2022
+# Last update: Sat May 20 12:03:20 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -43,14 +43,15 @@
         "DVDAspectRatio": NewType("DVDAspectRatio", int),
         "DVDAudioFormat": NewType("DVDAudioFormat", int),
         "DVDState": NewType("DVDState", int),
         "DVDMenu": NewType("DVDMenu", int),
     }
 )
 misc.update({})
+misc.update({})
 functions = {
     "DVDIsDisplayingSubPicture": (
         b"i^Z",
         "",
         {"arguments": {0: {"type_modifier": "o"}}},
     ),
     "DVDGoToMenu": (b"iI",),
@@ -239,15 +240,15 @@
     "DVDDisplaySubPicture": (b"iZ",),
     "DVDGetScanRate": (
         b"i^s^z",
         "",
         {"arguments": {0: {"type_modifier": "o"}, 1: {"type_modifier": "o"}}},
     ),
     "DVDRegisterEventCallBack": (
-        b"i^?^II^v^^v",
+        b"i^?^II^v^I",
         "",
         {
             "arguments": {
                 0: {
                     "callable": {
                         "retval": {"type": b"v"},
                         "arguments": {
@@ -255,14 +256,15 @@
                             1: {"type": b"L"},
                             2: {"type": b"L"},
                             3: {"type": b"^v"},
                         },
                     }
                 },
                 1: {"type_modifier": "n"},
+                4: {"type_modifier": "o"},
             }
         },
     ),
     "DVDSetAudioOutputMode": (b"ii",),
     "DVDSetDriveRegionCode": (b"iI^{AuthorizationOpaqueRef=}",),
     "DVDIsValidMediaURL": (
         b"i^{__CFURL=}^Z",
```

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/Lib/pyobjc_framework_DVDPlayback.egg-info/PKG-INFO` & `pyobjc-framework-DVDPlayback-9.2/Lib/pyobjc_framework_DVDPlayback.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-DVDPlayback
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework DVDPlayback on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,DVDPlayback
 Platform: MacOS X (>=10.7)
```

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/License.txt` & `pyobjc-framework-DVDPlayback-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/PKG-INFO` & `pyobjc-framework-DVDPlayback-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-DVDPlayback
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework DVDPlayback on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,DVDPlayback
 Platform: MacOS X (>=10.7)
```

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/PyObjCTest/test_dvdplayback.py` & `pyobjc-framework-DVDPlayback-9.2/PyObjCTest/test_dvdplayback.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/metadata/DVDPlayback.fwinfo` & `pyobjc-framework-DVDPlayback-9.2/metadata/DVDPlayback.fwinfo`

 * *Files 1% similar despite different names*

```diff
@@ -408,15 +408,15 @@
        "retval": {
         "typestr": "v"
        }
       }
      },
      "1": { "type_modifier": "n" },
      "3": {},
-     "4": {}
+     "4": { "type_modifier": "o", "type_override": "^I"}
     }
    },
    "DVDResume": {
     "variadic": false
    },
    "DVDReturnToTitle": {
     "variadic": false
```

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-DVDPlayback-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-DVDPlayback-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/x86_64-10.13.fwinfo` & `pyobjc-framework-DVDPlayback-9.2/metadata/raw/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-DVDPlayback-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-DVDPlayback-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-DVDPlayback-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DVDPlayback-9.1b1/pyobjc_setup.py` & `pyobjc-framework-DVDPlayback-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

