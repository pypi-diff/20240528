# Comparing `tmp/pyobjc-framework-ScreenSaver-9.1b1.tar.gz` & `tmp/pyobjc-framework-ScreenSaver-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ScreenSaver-9.1b1.tar", last modified: Sun Mar 26 11:38:23 2023, max compression
+gzip compressed data, was "pyobjc-framework-ScreenSaver-9.2.tar", last modified: Wed Jun  7 00:26:58 2023, max compression
```

## Comparing `pyobjc-framework-ScreenSaver-9.1b1.tar` & `pyobjc-framework-ScreenSaver-9.2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:23.373451 pyobjc-framework-ScreenSaver-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:23.276343 pyobjc-framework-ScreenSaver-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:23.295281 pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:23.296018 pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      456 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/English.lproj/InfoPlist.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:23.300381 pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/English.lproj/SillyBalls.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      277 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/English.lproj/SillyBalls.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      383 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/English.lproj/SillyBalls.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)      882 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/English.lproj/SillyBalls.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      439 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/README.txt
--rw-r--r--   0 ronald     (501) staff       (20)      904 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/SillyBalls.py
--rw-r--r--   0 ronald     (501) staff       (20)      378 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/summary.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ScreenSaver-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:23.277265 pyobjc-framework-ScreenSaver-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:23.310584 pyobjc-framework-ScreenSaver-9.1b1/Lib/ScreenSaver/
--rw-r--r--   0 ronald     (501) staff       (20)      756 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/Lib/ScreenSaver/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1388 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenSaver-9.1b1/Lib/ScreenSaver/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:23.324694 pyobjc-framework-ScreenSaver-9.1b1/Lib/pyobjc_framework_ScreenSaver.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2196 2023-03-26 11:38:23.000000 pyobjc-framework-ScreenSaver-9.1b1/Lib/pyobjc_framework_ScreenSaver.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1351 2023-03-26 11:38:23.000000 pyobjc-framework-ScreenSaver-9.1b1/Lib/pyobjc_framework_ScreenSaver.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:38:23.000000 pyobjc-framework-ScreenSaver-9.1b1/Lib/pyobjc_framework_ScreenSaver.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:29.000000 pyobjc-framework-ScreenSaver-9.1b1/Lib/pyobjc_framework_ScreenSaver.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:38:23.000000 pyobjc-framework-ScreenSaver-9.1b1/Lib/pyobjc_framework_ScreenSaver.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       12 2023-03-26 11:38:23.000000 pyobjc-framework-ScreenSaver-9.1b1/Lib/pyobjc_framework_ScreenSaver.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:23.339013 pyobjc-framework-ScreenSaver-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1517 2021-10-18 19:38:40.000000 pyobjc-framework-ScreenSaver-9.1b1/Modules/_ScreenSaver_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenSaver-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-ScreenSaver-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1985 2023-03-26 11:38:23.373084 pyobjc-framework-ScreenSaver-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:23.341802 pyobjc-framework-ScreenSaver-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2234 2022-04-12 20:05:18.000000 pyobjc-framework-ScreenSaver-9.1b1/PyObjCTest/test_screensaver.py
--rw-r--r--   0 ronald     (501) staff       (20)      288 2021-10-18 19:38:40.000000 pyobjc-framework-ScreenSaver-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:23.344238 pyobjc-framework-ScreenSaver-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      965 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/metadata/ScreenSaver.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       38 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:38:23.371986 pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     6454 2021-07-30 09:00:38.000000 pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6473 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6491 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6455 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5758 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5758 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     5847 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6455 2021-07-30 09:00:38.000000 pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6474 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6492 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ScreenSaver-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:38:23.373539 pyobjc-framework-ScreenSaver-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1008 2023-03-25 14:20:32.000000 pyobjc-framework-ScreenSaver-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:58.283895 pyobjc-framework-ScreenSaver-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:58.238605 pyobjc-framework-ScreenSaver-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:58.248143 pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:58.248719 pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      456 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/English.lproj/InfoPlist.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:58.251031 pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/English.lproj/SillyBalls.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      277 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/English.lproj/SillyBalls.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      383 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/English.lproj/SillyBalls.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      882 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/English.lproj/SillyBalls.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      439 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/README.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      904 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/SillyBalls.py
+-rw-r--r--   0 ronald     (501) staff       (20)      378 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       40 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/summary.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ScreenSaver-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:58.239599 pyobjc-framework-ScreenSaver-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:58.255798 pyobjc-framework-ScreenSaver-9.2/Lib/ScreenSaver/
+-rw-r--r--   0 ronald     (501) staff       (20)      756 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/Lib/ScreenSaver/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1388 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenSaver-9.2/Lib/ScreenSaver/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:58.259971 pyobjc-framework-ScreenSaver-9.2/Lib/pyobjc_framework_ScreenSaver.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2194 2023-06-07 00:26:58.000000 pyobjc-framework-ScreenSaver-9.2/Lib/pyobjc_framework_ScreenSaver.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1366 2023-06-07 00:26:58.000000 pyobjc-framework-ScreenSaver-9.2/Lib/pyobjc_framework_ScreenSaver.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:26:58.000000 pyobjc-framework-ScreenSaver-9.2/Lib/pyobjc_framework_ScreenSaver.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:29.000000 pyobjc-framework-ScreenSaver-9.2/Lib/pyobjc_framework_ScreenSaver.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:26:58.000000 pyobjc-framework-ScreenSaver-9.2/Lib/pyobjc_framework_ScreenSaver.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       12 2023-06-07 00:26:58.000000 pyobjc-framework-ScreenSaver-9.2/Lib/pyobjc_framework_ScreenSaver.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:58.261932 pyobjc-framework-ScreenSaver-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1517 2021-10-18 19:38:40.000000 pyobjc-framework-ScreenSaver-9.2/Modules/_ScreenSaver_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenSaver-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-ScreenSaver-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1983 2023-06-07 00:26:58.283374 pyobjc-framework-ScreenSaver-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:58.263178 pyobjc-framework-ScreenSaver-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2234 2022-04-12 20:05:18.000000 pyobjc-framework-ScreenSaver-9.2/PyObjCTest/test_screensaver.py
+-rw-r--r--   0 ronald     (501) staff       (20)      288 2021-10-18 19:38:40.000000 pyobjc-framework-ScreenSaver-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:58.264797 pyobjc-framework-ScreenSaver-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      965 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/metadata/ScreenSaver.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:58.272356 pyobjc-framework-ScreenSaver-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     6454 2021-07-30 09:00:38.000000 pyobjc-framework-ScreenSaver-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6473 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenSaver-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6491 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenSaver-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6455 2021-03-21 10:08:23.000000 pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5758 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5758 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     5847 2020-11-30 18:45:15.000000 pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6455 2021-07-30 09:00:38.000000 pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6474 2022-02-24 08:47:17.000000 pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6492 2023-02-19 10:50:35.000000 pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ScreenSaver-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ScreenSaver-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:26:58.283996 pyobjc-framework-ScreenSaver-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1090 2023-05-29 10:07:47.000000 pyobjc-framework-ScreenSaver-9.2/setup.py
```

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/English.lproj/SillyBalls.nib/keyedobjects.nib` & `pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/English.lproj/SillyBalls.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/Examples/SillyBallsSaver/SillyBalls.py` & `pyobjc-framework-ScreenSaver-9.2/Examples/SillyBallsSaver/SillyBalls.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/LICENSE.txt` & `pyobjc-framework-ScreenSaver-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/Lib/ScreenSaver/__init__.py` & `pyobjc-framework-ScreenSaver-9.2/Lib/ScreenSaver/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/Lib/ScreenSaver/_metadata.py` & `pyobjc-framework-ScreenSaver-9.2/Lib/ScreenSaver/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/Lib/pyobjc_framework_ScreenSaver.egg-info/PKG-INFO` & `pyobjc-framework-ScreenSaver-9.2/Lib/pyobjc_framework_ScreenSaver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ScreenSaver
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ScreenSaver on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ScreenSaver
 Platform: MacOS X
```

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/Lib/pyobjc_framework_ScreenSaver.egg-info/SOURCES.txt` & `pyobjc-framework-ScreenSaver-9.2/Lib/pyobjc_framework_ScreenSaver.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/SillyBallsSaver/README.txt
 Examples/SillyBallsSaver/SillyBalls.py
 Examples/SillyBallsSaver/setup.py
 Examples/SillyBallsSaver/summary.txt
 Examples/SillyBallsSaver/English.lproj/InfoPlist.strings
 Examples/SillyBallsSaver/English.lproj/SillyBalls.nib/classes.nib
```

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/Modules/_ScreenSaver_inlines.m` & `pyobjc-framework-ScreenSaver-9.2/Modules/_ScreenSaver_inlines.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-ScreenSaver-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-ScreenSaver-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/PKG-INFO` & `pyobjc-framework-ScreenSaver-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ScreenSaver
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ScreenSaver on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ScreenSaver
 Platform: MacOS X
```

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/PyObjCTest/test_screensaver.py` & `pyobjc-framework-ScreenSaver-9.2/PyObjCTest/test_screensaver.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/metadata/ScreenSaver.fwinfo` & `pyobjc-framework-ScreenSaver-9.2/metadata/ScreenSaver.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-ScreenSaver-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-ScreenSaver-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-ScreenSaver-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-ScreenSaver-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ScreenSaver-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ScreenSaver-9.1b1/setup.py` & `pyobjc-framework-ScreenSaver-9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 you to write custom screensaver modules.
 
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
     name="pyobjc-framework-ScreenSaver",
     description="Wrappers for the framework ScreenSaver on macOS",
     packages=["ScreenSaver"],
     ext_modules=[
         Extension(
```

