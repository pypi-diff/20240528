# Comparing `tmp/pyobjc-framework-InstantMessage-9.1b1.tar.gz` & `tmp/pyobjc-framework-InstantMessage-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-InstantMessage-9.1b1.tar", last modified: Sun Mar 26 11:27:23 2023, max compression
+gzip compressed data, was "pyobjc-framework-InstantMessage-9.2.tar", last modified: Wed Jun  7 00:17:46 2023, max compression
```

## Comparing `pyobjc-framework-InstantMessage-9.1b1.tar` & `pyobjc-framework-InstantMessage-9.2.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:23.804386 pyobjc-framework-InstantMessage-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:23.766047 pyobjc-framework-InstantMessage-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:23.774516 pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/
--rw-r--r--   0 ronald     (501) staff       (20)     1436 2021-07-30 09:00:38.000000 pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/ABPersonDisplayNameAdditions.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:23.766333 pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:23.776651 pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      372 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      587 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    16560 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     6097 2021-10-18 19:38:40.000000 pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/PeopleDataSource.py
--rw-r--r--   0 ronald     (501) staff       (20)     2482 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/ServiceWatcher.py
--rw-r--r--   0 ronald     (501) staff       (20)      185 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      319 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      117 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/summary.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-InstantMessage-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:23.766750 pyobjc-framework-InstantMessage-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:23.787701 pyobjc-framework-InstantMessage-9.1b1/Lib/InstantMessage/
--rw-r--r--   0 ronald     (501) staff       (20)      747 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/Lib/InstantMessage/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     4311 2022-02-24 08:47:16.000000 pyobjc-framework-InstantMessage-9.1b1/Lib/InstantMessage/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:23.791174 pyobjc-framework-InstantMessage-9.1b1/Lib/pyobjc_framework_InstantMessage.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2408 2023-03-26 11:27:23.000000 pyobjc-framework-InstantMessage-9.1b1/Lib/pyobjc_framework_InstantMessage.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1328 2023-03-26 11:27:23.000000 pyobjc-framework-InstantMessage-9.1b1/Lib/pyobjc_framework_InstantMessage.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:27:23.000000 pyobjc-framework-InstantMessage-9.1b1/Lib/pyobjc_framework_InstantMessage.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:14.000000 pyobjc-framework-InstantMessage-9.1b1/Lib/pyobjc_framework_InstantMessage.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:27:23.000000 pyobjc-framework-InstantMessage-9.1b1/Lib/pyobjc_framework_InstantMessage.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       15 2023-03-26 11:27:23.000000 pyobjc-framework-InstantMessage-9.1b1/Lib/pyobjc_framework_InstantMessage.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     2197 2023-03-26 11:27:23.804054 pyobjc-framework-InstantMessage-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:23.794905 pyobjc-framework-InstantMessage-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      388 2021-03-21 10:08:22.000000 pyobjc-framework-InstantMessage-9.1b1/PyObjCTest/test_imavcontrol.py
--rw-r--r--   0 ronald     (501) staff       (20)     2024 2021-03-21 10:08:22.000000 pyobjc-framework-InstantMessage-9.1b1/PyObjCTest/test_imavmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     2823 2021-03-21 10:08:22.000000 pyobjc-framework-InstantMessage-9.1b1/PyObjCTest/test_imservice.py
--rw-r--r--   0 ronald     (501) staff       (20)      212 2022-04-11 08:03:15.000000 pyobjc-framework-InstantMessage-9.1b1/PyObjCTest/test_instantmessage.py
--rw-r--r--   0 ronald     (501) staff       (20)      291 2021-10-18 19:38:40.000000 pyobjc-framework-InstantMessage-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:23.796421 pyobjc-framework-InstantMessage-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2611 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/metadata/InstantMessage.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       88 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:23.803199 pyobjc-framework-InstantMessage-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    22012 2021-07-30 09:00:38.000000 pyobjc-framework-InstantMessage-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22031 2022-02-24 08:47:16.000000 pyobjc-framework-InstantMessage-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22013 2021-03-21 10:08:22.000000 pyobjc-framework-InstantMessage-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21943 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21943 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22011 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22013 2021-07-30 09:00:38.000000 pyobjc-framework-InstantMessage-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22032 2022-02-24 08:47:16.000000 pyobjc-framework-InstantMessage-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-InstantMessage-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:27:23.804645 pyobjc-framework-InstantMessage-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1008 2023-03-25 14:20:31.000000 pyobjc-framework-InstantMessage-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:46.636905 pyobjc-framework-InstantMessage-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:46.580292 pyobjc-framework-InstantMessage-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:46.594092 pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/
+-rw-r--r--   0 ronald     (501) staff       (20)     1436 2021-07-30 09:00:38.000000 pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/ABPersonDisplayNameAdditions.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:46.580657 pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:46.596577 pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      372 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      587 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    16560 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     6097 2021-10-18 19:38:40.000000 pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/PeopleDataSource.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2482 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/ServiceWatcher.py
+-rw-r--r--   0 ronald     (501) staff       (20)      185 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      319 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      117 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/summary.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-InstantMessage-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:46.581302 pyobjc-framework-InstantMessage-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:46.598086 pyobjc-framework-InstantMessage-9.2/Lib/InstantMessage/
+-rw-r--r--   0 ronald     (501) staff       (20)      747 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/Lib/InstantMessage/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4311 2022-02-24 08:47:16.000000 pyobjc-framework-InstantMessage-9.2/Lib/InstantMessage/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:46.601402 pyobjc-framework-InstantMessage-9.2/Lib/pyobjc_framework_InstantMessage.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2406 2023-06-07 00:17:46.000000 pyobjc-framework-InstantMessage-9.2/Lib/pyobjc_framework_InstantMessage.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1343 2023-06-07 00:17:46.000000 pyobjc-framework-InstantMessage-9.2/Lib/pyobjc_framework_InstantMessage.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:17:46.000000 pyobjc-framework-InstantMessage-9.2/Lib/pyobjc_framework_InstantMessage.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:14.000000 pyobjc-framework-InstantMessage-9.2/Lib/pyobjc_framework_InstantMessage.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:17:46.000000 pyobjc-framework-InstantMessage-9.2/Lib/pyobjc_framework_InstantMessage.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       15 2023-06-07 00:17:46.000000 pyobjc-framework-InstantMessage-9.2/Lib/pyobjc_framework_InstantMessage.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     2195 2023-06-07 00:17:46.635359 pyobjc-framework-InstantMessage-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:46.604770 pyobjc-framework-InstantMessage-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      388 2021-03-21 10:08:22.000000 pyobjc-framework-InstantMessage-9.2/PyObjCTest/test_imavcontrol.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2024 2021-03-21 10:08:22.000000 pyobjc-framework-InstantMessage-9.2/PyObjCTest/test_imavmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2823 2021-03-21 10:08:22.000000 pyobjc-framework-InstantMessage-9.2/PyObjCTest/test_imservice.py
+-rw-r--r--   0 ronald     (501) staff       (20)      212 2022-04-11 08:03:15.000000 pyobjc-framework-InstantMessage-9.2/PyObjCTest/test_instantmessage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      291 2021-10-18 19:38:40.000000 pyobjc-framework-InstantMessage-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:46.606464 pyobjc-framework-InstantMessage-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2611 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/metadata/InstantMessage.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       88 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:46.626831 pyobjc-framework-InstantMessage-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    22012 2021-07-30 09:00:38.000000 pyobjc-framework-InstantMessage-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22031 2022-02-24 08:47:16.000000 pyobjc-framework-InstantMessage-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22013 2021-03-21 10:08:22.000000 pyobjc-framework-InstantMessage-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21943 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21943 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22011 2020-11-30 18:45:15.000000 pyobjc-framework-InstantMessage-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22013 2021-07-30 09:00:38.000000 pyobjc-framework-InstantMessage-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22032 2022-02-24 08:47:16.000000 pyobjc-framework-InstantMessage-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-InstantMessage-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-InstantMessage-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:17:46.637011 pyobjc-framework-InstantMessage-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1090 2023-05-29 10:07:46.000000 pyobjc-framework-InstantMessage-9.2/setup.py
```

### Comparing `pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/ABPersonDisplayNameAdditions.py` & `pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/ABPersonDisplayNameAdditions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/PeopleDataSource.py` & `pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/PeopleDataSource.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/Examples/ABPresence/ServiceWatcher.py` & `pyobjc-framework-InstantMessage-9.2/Examples/ABPresence/ServiceWatcher.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/LICENSE.txt` & `pyobjc-framework-InstantMessage-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/Lib/InstantMessage/__init__.py` & `pyobjc-framework-InstantMessage-9.2/Lib/InstantMessage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/Lib/InstantMessage/_metadata.py` & `pyobjc-framework-InstantMessage-9.2/Lib/InstantMessage/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/Lib/pyobjc_framework_InstantMessage.egg-info/PKG-INFO` & `pyobjc-framework-InstantMessage-9.2/Lib/pyobjc_framework_InstantMessage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-InstantMessage
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework InstantMessage on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,InstantMessage
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-InstantMessage-9.1b1/Lib/pyobjc_framework_InstantMessage.egg-info/SOURCES.txt` & `pyobjc-framework-InstantMessage-9.2/Lib/pyobjc_framework_InstantMessage.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/ABPresence/ABPersonDisplayNameAdditions.py
 Examples/ABPresence/PeopleDataSource.py
 Examples/ABPresence/ServiceWatcher.py
 Examples/ABPresence/main.py
 Examples/ABPresence/setup.py
 Examples/ABPresence/summary.txt
```

### Comparing `pyobjc-framework-InstantMessage-9.1b1/PKG-INFO` & `pyobjc-framework-InstantMessage-9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-InstantMessage
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework InstantMessage on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,InstantMessage
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-InstantMessage-9.1b1/PyObjCTest/test_imavmanager.py` & `pyobjc-framework-InstantMessage-9.2/PyObjCTest/test_imavmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/PyObjCTest/test_imservice.py` & `pyobjc-framework-InstantMessage-9.2/PyObjCTest/test_imservice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/metadata/InstantMessage.fwinfo` & `pyobjc-framework-InstantMessage-9.2/metadata/InstantMessage.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-InstantMessage-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-InstantMessage-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-InstantMessage-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-InstantMessage-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-InstantMessage-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-InstantMessage-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-InstantMessage-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-InstantMessage-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstantMessage-9.1b1/pyobjc_setup.py` & `pyobjc-framework-InstantMessage-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

