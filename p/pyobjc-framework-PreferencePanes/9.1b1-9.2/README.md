# Comparing `tmp/pyobjc-framework-PreferencePanes-9.1b1.tar.gz` & `tmp/pyobjc-framework-PreferencePanes-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-PreferencePanes-9.1b1.tar", last modified: Sun Mar 26 11:34:24 2023, max compression
+gzip compressed data, was "pyobjc-framework-PreferencePanes-9.2.tar", last modified: Wed Jun  7 00:24:01 2023, max compression
```

## Comparing `pyobjc-framework-PreferencePanes-9.1b1.tar` & `pyobjc-framework-PreferencePanes-9.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.954301 pyobjc-framework-PreferencePanes-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.897530 pyobjc-framework-PreferencePanes-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.908735 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/
--rw-r--r--   0 ronald     (501) staff       (20)     1056 2021-10-18 19:38:40.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/00ReadMe.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.910122 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/Dutch.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.912438 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/Dutch.lproj/EnvironmentPane.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      706 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/Dutch.lproj/EnvironmentPane.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      454 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/Dutch.lproj/EnvironmentPane.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     2635 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/Dutch.lproj/EnvironmentPane.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      244 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/Dutch.lproj/InfoPlist.strings
--rw-r--r--   0 ronald     (501) staff       (20)     2084 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/Dutch.lproj/Localizable.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.916230 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.920076 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/English.lproj/EnvironmentPane.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      706 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/English.lproj/EnvironmentPane.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      454 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/English.lproj/EnvironmentPane.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     2607 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/English.lproj/EnvironmentPane.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      248 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/English.lproj/InfoPlist.strings
--rw-r--r--   0 ronald     (501) staff       (20)     1998 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/English.lproj/Localizable.strings
--rw-r--r--   0 ronald     (501) staff       (20)    21894 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/ShellEnv.icns
--rw-r--r--   0 ronald     (501) staff       (20)     7796 2022-10-18 09:53:23.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/ShellEnv.py
--rw-r--r--   0 ronald     (501) staff       (20)     2196 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/ShellEnv.tiff
--rw-r--r--   0 ronald     (501) staff       (20)      795 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      148 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/summary.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-PreferencePanes-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.898402 pyobjc-framework-PreferencePanes-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.921094 pyobjc-framework-PreferencePanes-9.1b1/Lib/PreferencePanes/
--rw-r--r--   0 ronald     (501) staff       (20)      739 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/Lib/PreferencePanes/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1675 2022-02-24 08:47:16.000000 pyobjc-framework-PreferencePanes-9.1b1/Lib/PreferencePanes/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.924755 pyobjc-framework-PreferencePanes-9.1b1/Lib/pyobjc_framework_PreferencePanes.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2242 2023-03-26 11:34:24.000000 pyobjc-framework-PreferencePanes-9.1b1/Lib/pyobjc_framework_PreferencePanes.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1767 2023-03-26 11:34:24.000000 pyobjc-framework-PreferencePanes-9.1b1/Lib/pyobjc_framework_PreferencePanes.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:34:24.000000 pyobjc-framework-PreferencePanes-9.1b1/Lib/pyobjc_framework_PreferencePanes.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:51.000000 pyobjc-framework-PreferencePanes-9.1b1/Lib/pyobjc_framework_PreferencePanes.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:34:24.000000 pyobjc-framework-PreferencePanes-9.1b1/Lib/pyobjc_framework_PreferencePanes.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       16 2023-03-26 11:34:24.000000 pyobjc-framework-PreferencePanes-9.1b1/Lib/pyobjc_framework_PreferencePanes.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     2031 2023-03-26 11:34:24.953808 pyobjc-framework-PreferencePanes-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.928527 pyobjc-framework-PreferencePanes-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1998 2022-02-24 08:47:16.000000 pyobjc-framework-PreferencePanes-9.1b1/PyObjCTest/test_nspreferencepane.py
--rw-r--r--   0 ronald     (501) staff       (20)      448 2022-04-11 08:03:15.000000 pyobjc-framework-PreferencePanes-9.1b1/PyObjCTest/test_preferencepanes.py
--rw-r--r--   0 ronald     (501) staff       (20)      342 2021-10-18 19:38:40.000000 pyobjc-framework-PreferencePanes-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.935366 pyobjc-framework-PreferencePanes-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      925 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/metadata/PreferencePanes.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:34:24.952047 pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)     8447 2021-07-30 09:00:38.000000 pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8528 2022-02-24 08:47:16.000000 pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8448 2021-03-21 10:08:23.000000 pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6583 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6768 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     6869 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8448 2021-07-30 09:00:38.000000 pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8529 2022-02-24 08:47:16.000000 pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PreferencePanes-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:34:24.954408 pyobjc-framework-PreferencePanes-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      756 2023-03-25 14:20:32.000000 pyobjc-framework-PreferencePanes-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.207321 pyobjc-framework-PreferencePanes-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.140615 pyobjc-framework-PreferencePanes-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.151849 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/
+-rw-r--r--   0 ronald     (501) staff       (20)     1056 2021-10-18 19:38:40.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/00ReadMe.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.153259 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/Dutch.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.159982 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/Dutch.lproj/EnvironmentPane.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      706 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/Dutch.lproj/EnvironmentPane.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      454 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/Dutch.lproj/EnvironmentPane.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     2635 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/Dutch.lproj/EnvironmentPane.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      244 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/Dutch.lproj/InfoPlist.strings
+-rw-r--r--   0 ronald     (501) staff       (20)     2084 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/Dutch.lproj/Localizable.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.161370 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.163761 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/English.lproj/EnvironmentPane.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      706 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/English.lproj/EnvironmentPane.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      454 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/English.lproj/EnvironmentPane.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     2607 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/English.lproj/EnvironmentPane.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      248 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/English.lproj/InfoPlist.strings
+-rw-r--r--   0 ronald     (501) staff       (20)     1998 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/English.lproj/Localizable.strings
+-rw-r--r--   0 ronald     (501) staff       (20)    21894 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/ShellEnv.icns
+-rw-r--r--   0 ronald     (501) staff       (20)     7796 2022-10-18 09:53:23.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/ShellEnv.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2196 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/ShellEnv.tiff
+-rw-r--r--   0 ronald     (501) staff       (20)      795 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      148 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/summary.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-PreferencePanes-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.142143 pyobjc-framework-PreferencePanes-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.164925 pyobjc-framework-PreferencePanes-9.2/Lib/PreferencePanes/
+-rw-r--r--   0 ronald     (501) staff       (20)      739 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/Lib/PreferencePanes/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1675 2022-02-24 08:47:16.000000 pyobjc-framework-PreferencePanes-9.2/Lib/PreferencePanes/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.168045 pyobjc-framework-PreferencePanes-9.2/Lib/pyobjc_framework_PreferencePanes.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2240 2023-06-07 00:24:01.000000 pyobjc-framework-PreferencePanes-9.2/Lib/pyobjc_framework_PreferencePanes.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1782 2023-06-07 00:24:01.000000 pyobjc-framework-PreferencePanes-9.2/Lib/pyobjc_framework_PreferencePanes.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:24:01.000000 pyobjc-framework-PreferencePanes-9.2/Lib/pyobjc_framework_PreferencePanes.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:51.000000 pyobjc-framework-PreferencePanes-9.2/Lib/pyobjc_framework_PreferencePanes.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:24:01.000000 pyobjc-framework-PreferencePanes-9.2/Lib/pyobjc_framework_PreferencePanes.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       16 2023-06-07 00:24:01.000000 pyobjc-framework-PreferencePanes-9.2/Lib/pyobjc_framework_PreferencePanes.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     2029 2023-06-07 00:24:01.206935 pyobjc-framework-PreferencePanes-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.184030 pyobjc-framework-PreferencePanes-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1998 2022-02-24 08:47:16.000000 pyobjc-framework-PreferencePanes-9.2/PyObjCTest/test_nspreferencepane.py
+-rw-r--r--   0 ronald     (501) staff       (20)      448 2022-04-11 08:03:15.000000 pyobjc-framework-PreferencePanes-9.2/PyObjCTest/test_preferencepanes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      342 2021-10-18 19:38:40.000000 pyobjc-framework-PreferencePanes-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.191167 pyobjc-framework-PreferencePanes-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      925 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/metadata/PreferencePanes.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:24:01.206180 pyobjc-framework-PreferencePanes-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)     8447 2021-07-30 09:00:38.000000 pyobjc-framework-PreferencePanes-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8528 2022-02-24 08:47:16.000000 pyobjc-framework-PreferencePanes-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8448 2021-03-21 10:08:23.000000 pyobjc-framework-PreferencePanes-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6583 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6768 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     6869 2020-11-30 18:45:15.000000 pyobjc-framework-PreferencePanes-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8448 2021-07-30 09:00:38.000000 pyobjc-framework-PreferencePanes-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8529 2022-02-24 08:47:16.000000 pyobjc-framework-PreferencePanes-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-PreferencePanes-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-PreferencePanes-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:24:01.207521 pyobjc-framework-PreferencePanes-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      838 2023-05-29 10:07:47.000000 pyobjc-framework-PreferencePanes-9.2/setup.py
```

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/00ReadMe.txt` & `pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/00ReadMe.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/Dutch.lproj/EnvironmentPane.nib/classes.nib` & `pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/Dutch.lproj/EnvironmentPane.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/Dutch.lproj/EnvironmentPane.nib/objects.nib` & `pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/Dutch.lproj/EnvironmentPane.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/Dutch.lproj/Localizable.strings` & `pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/Dutch.lproj/Localizable.strings`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/English.lproj/EnvironmentPane.nib/classes.nib` & `pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/English.lproj/EnvironmentPane.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/English.lproj/EnvironmentPane.nib/objects.nib` & `pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/English.lproj/EnvironmentPane.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/English.lproj/Localizable.strings` & `pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/English.lproj/Localizable.strings`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/ShellEnv.icns` & `pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/ShellEnv.icns`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/ShellEnv.py` & `pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/ShellEnv.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/ShellEnv.tiff` & `pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/ShellEnv.tiff`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Examples/EnvironmentPrefs/setup.py` & `pyobjc-framework-PreferencePanes-9.2/Examples/EnvironmentPrefs/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/LICENSE.txt` & `pyobjc-framework-PreferencePanes-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Lib/PreferencePanes/__init__.py` & `pyobjc-framework-PreferencePanes-9.2/Lib/PreferencePanes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Lib/PreferencePanes/_metadata.py` & `pyobjc-framework-PreferencePanes-9.2/Lib/PreferencePanes/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Lib/pyobjc_framework_PreferencePanes.egg-info/PKG-INFO` & `pyobjc-framework-PreferencePanes-9.2/Lib/pyobjc_framework_PreferencePanes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PreferencePanes
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PreferencePanes on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PreferencePanes
 Platform: MacOS X
```

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/Lib/pyobjc_framework_PreferencePanes.egg-info/SOURCES.txt` & `pyobjc-framework-PreferencePanes-9.2/Lib/pyobjc_framework_PreferencePanes.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/EnvironmentPrefs/00ReadMe.txt
 Examples/EnvironmentPrefs/ShellEnv.icns
 Examples/EnvironmentPrefs/ShellEnv.py
 Examples/EnvironmentPrefs/ShellEnv.tiff
 Examples/EnvironmentPrefs/setup.py
 Examples/EnvironmentPrefs/summary.txt
```

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/PKG-INFO` & `pyobjc-framework-PreferencePanes-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-PreferencePanes
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework PreferencePanes on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,PreferencePanes
 Platform: MacOS X
```

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/PyObjCTest/test_nspreferencepane.py` & `pyobjc-framework-PreferencePanes-9.2/PyObjCTest/test_nspreferencepane.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/metadata/PreferencePanes.fwinfo` & `pyobjc-framework-PreferencePanes-9.2/metadata/PreferencePanes.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-PreferencePanes-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-PreferencePanes-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-PreferencePanes-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-PreferencePanes-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-PreferencePanes-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-PreferencePanes-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-PreferencePanes-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-PreferencePanes-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-PreferencePanes-9.1b1/pyobjc_setup.py` & `pyobjc-framework-PreferencePanes-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

