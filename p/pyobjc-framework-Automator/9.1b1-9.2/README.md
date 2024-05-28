# Comparing `tmp/pyobjc-framework-Automator-9.1b1.tar.gz` & `tmp/pyobjc-framework-Automator-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Automator-9.1b1.tar", last modified: Sun Mar 26 11:15:34 2023, max compression
+gzip compressed data, was "pyobjc-framework-Automator-9.2.tar", last modified: Wed Jun  7 00:06:54 2023, max compression
```

## Comparing `pyobjc-framework-Automator-9.1b1.tar` & `pyobjc-framework-Automator-9.2.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.680316 pyobjc-framework-Automator-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.465194 pyobjc-framework-Automator-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.525538 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/
--rw-r--r--   0 ronald     (501) staff       (20)     6815 2021-07-30 09:00:37.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/Controller.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.526118 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      178 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/English.lproj/InfoPlist.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.529695 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)   158300 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/English.lproj/MainMenu.nib/designable.nib
--rw-r--r--   0 ronald     (501) staff       (20)    27692 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     5300 2021-10-18 19:38:40.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/ReadMe.txt
--rw-r--r--   0 ronald     (501) staff       (20)       92 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      284 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      971 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.464578 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.463794 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Hello World.workflow/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.530481 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Hello World.workflow/Contents/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.531045 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Hello World.workflow/Contents/QuickLook/
--rw-r--r--   0 ronald     (501) staff       (20)    47276 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Hello World.workflow/Contents/QuickLook/Preview.pdf
--rwxr-xr-x   0 ronald     (501) staff       (20)     3716 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Hello World.workflow/Contents/document.wflow
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.464214 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Run Automator.workflow/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.531903 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Run Automator.workflow/Contents/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.532816 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Run Automator.workflow/Contents/QuickLook/
--rw-r--r--   0 ronald     (501) staff       (20)    31457 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Run Automator.workflow/Contents/QuickLook/Preview.pdf
--rwxr-xr-x   0 ronald     (501) staff       (20)     3680 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Run Automator.workflow/Contents/document.wflow
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.464874 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Small Step.workflow/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.539435 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Small Step.workflow/Contents/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.556626 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Small Step.workflow/Contents/QuickLook/
--rw-r--r--   0 ronald     (501) staff       (20)    42495 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Small Step.workflow/Contents/QuickLook/Preview.pdf
--rwxr-xr-x   0 ronald     (501) staff       (20)     7215 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Small Step.workflow/Contents/document.wflow
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.564401 pyobjc-framework-Automator-9.1b1/Examples/Get Buddy Info/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.565761 pyobjc-framework-Automator-9.1b1/Examples/Get Buddy Info/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)     1322 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/Get Buddy Info/English.lproj/InfoPlist.strings
--rw-r--r--   0 ronald     (501) staff       (20)     5193 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/Get Buddy Info/GetBuddyInfo.py
--rw-r--r--   0 ronald     (501) staff       (20)     2198 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/Get Buddy Info/Info.plist
--rw-r--r--   0 ronald     (501) staff       (20)     1323 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/Get Buddy Info/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       72 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Examples/Get Buddy Info/summary.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Automator-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.465759 pyobjc-framework-Automator-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.568325 pyobjc-framework-Automator-9.1b1/Lib/Automator/
--rw-r--r--   0 ronald     (501) staff       (20)      690 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/Lib/Automator/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     6372 2022-02-24 08:47:16.000000 pyobjc-framework-Automator-9.1b1/Lib/Automator/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.578886 pyobjc-framework-Automator-9.1b1/Lib/pyobjc_framework_Automator.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2358 2023-03-26 11:15:34.000000 pyobjc-framework-Automator-9.1b1/Lib/pyobjc_framework_Automator.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     2098 2023-03-26 11:15:34.000000 pyobjc-framework-Automator-9.1b1/Lib/pyobjc_framework_Automator.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:15:34.000000 pyobjc-framework-Automator-9.1b1/Lib/pyobjc_framework_Automator.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:23.000000 pyobjc-framework-Automator-9.1b1/Lib/pyobjc_framework_Automator.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:15:34.000000 pyobjc-framework-Automator-9.1b1/Lib/pyobjc_framework_Automator.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:15:34.000000 pyobjc-framework-Automator-9.1b1/Lib/pyobjc_framework_Automator.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     2147 2023-03-26 11:15:34.679984 pyobjc-framework-Automator-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.645611 pyobjc-framework-Automator-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1167 2022-02-24 08:47:16.000000 pyobjc-framework-Automator-9.1b1/PyObjCTest/test_amaction.py
--rw-r--r--   0 ronald     (501) staff       (20)      305 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/PyObjCTest/test_ambundleaction.py
--rw-r--r--   0 ronald     (501) staff       (20)      212 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/PyObjCTest/test_amshellscriptaction.py
--rw-r--r--   0 ronald     (501) staff       (20)      559 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/PyObjCTest/test_amworkflow.py
--rw-r--r--   0 ronald     (501) staff       (20)      530 2022-06-25 20:07:56.000000 pyobjc-framework-Automator-9.1b1/PyObjCTest/test_amworkflowcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      307 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/PyObjCTest/test_amworkflowview.py
--rw-r--r--   0 ronald     (501) staff       (20)      259 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/PyObjCTest/test_amworkspace.py
--rw-r--r--   0 ronald     (501) staff       (20)      842 2022-04-12 20:05:08.000000 pyobjc-framework-Automator-9.1b1/PyObjCTest/test_automator.py
--rw-r--r--   0 ronald     (501) staff       (20)     2879 2022-02-24 08:47:16.000000 pyobjc-framework-Automator-9.1b1/PyObjCTest/test_automatorerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)      286 2021-10-18 19:38:40.000000 pyobjc-framework-Automator-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.652840 pyobjc-framework-Automator-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     3883 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/metadata/Automator.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:15:34.678427 pyobjc-framework-Automator-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    36150 2021-07-30 09:00:37.000000 pyobjc-framework-Automator-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36254 2022-02-24 08:47:16.000000 pyobjc-framework-Automator-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31389 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    35772 2021-03-21 10:08:22.000000 pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    24376 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    26356 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    26444 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36151 2021-07-30 09:00:37.000000 pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    36255 2022-02-24 08:47:16.000000 pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Automator-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:15:34.680400 pyobjc-framework-Automator-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      872 2023-03-25 14:20:30.000000 pyobjc-framework-Automator-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.609272 pyobjc-framework-Automator-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.546088 pyobjc-framework-Automator-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.558181 pyobjc-framework-Automator-9.2/Examples/AutoSample/
+-rw-r--r--   0 ronald     (501) staff       (20)     6815 2021-07-30 09:00:37.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/Controller.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.558738 pyobjc-framework-Automator-9.2/Examples/AutoSample/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      178 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/English.lproj/InfoPlist.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.561262 pyobjc-framework-Automator-9.2/Examples/AutoSample/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)   158300 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/English.lproj/MainMenu.nib/designable.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    27692 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     5300 2021-10-18 19:38:40.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/ReadMe.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       92 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      284 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      971 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.545378 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.544404 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Hello World.workflow/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.562064 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Hello World.workflow/Contents/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.562602 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Hello World.workflow/Contents/QuickLook/
+-rw-r--r--   0 ronald     (501) staff       (20)    47276 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Hello World.workflow/Contents/QuickLook/Preview.pdf
+-rwxr-xr-x   0 ronald     (501) staff       (20)     3716 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Hello World.workflow/Contents/document.wflow
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.544954 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Run Automator.workflow/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.563405 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Run Automator.workflow/Contents/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.564223 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Run Automator.workflow/Contents/QuickLook/
+-rw-r--r--   0 ronald     (501) staff       (20)    31457 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Run Automator.workflow/Contents/QuickLook/Preview.pdf
+-rwxr-xr-x   0 ronald     (501) staff       (20)     3680 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Run Automator.workflow/Contents/document.wflow
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.545689 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Small Step.workflow/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.565366 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Small Step.workflow/Contents/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.566161 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Small Step.workflow/Contents/QuickLook/
+-rw-r--r--   0 ronald     (501) staff       (20)    42495 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Small Step.workflow/Contents/QuickLook/Preview.pdf
+-rwxr-xr-x   0 ronald     (501) staff       (20)     7215 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Small Step.workflow/Contents/document.wflow
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.569599 pyobjc-framework-Automator-9.2/Examples/Get Buddy Info/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.570259 pyobjc-framework-Automator-9.2/Examples/Get Buddy Info/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)     1322 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/Get Buddy Info/English.lproj/InfoPlist.strings
+-rw-r--r--   0 ronald     (501) staff       (20)     5193 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/Get Buddy Info/GetBuddyInfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2198 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/Get Buddy Info/Info.plist
+-rw-r--r--   0 ronald     (501) staff       (20)     1323 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/Get Buddy Info/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       72 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Examples/Get Buddy Info/summary.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Automator-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.546852 pyobjc-framework-Automator-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.571772 pyobjc-framework-Automator-9.2/Lib/Automator/
+-rw-r--r--   0 ronald     (501) staff       (20)      690 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/Lib/Automator/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6372 2022-02-24 08:47:16.000000 pyobjc-framework-Automator-9.2/Lib/Automator/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.576933 pyobjc-framework-Automator-9.2/Lib/pyobjc_framework_Automator.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2356 2023-06-07 00:06:54.000000 pyobjc-framework-Automator-9.2/Lib/pyobjc_framework_Automator.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     2113 2023-06-07 00:06:54.000000 pyobjc-framework-Automator-9.2/Lib/pyobjc_framework_Automator.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:06:54.000000 pyobjc-framework-Automator-9.2/Lib/pyobjc_framework_Automator.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:23.000000 pyobjc-framework-Automator-9.2/Lib/pyobjc_framework_Automator.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:06:54.000000 pyobjc-framework-Automator-9.2/Lib/pyobjc_framework_Automator.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:06:54.000000 pyobjc-framework-Automator-9.2/Lib/pyobjc_framework_Automator.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     2145 2023-06-07 00:06:54.608473 pyobjc-framework-Automator-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.585613 pyobjc-framework-Automator-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1167 2022-02-24 08:47:16.000000 pyobjc-framework-Automator-9.2/PyObjCTest/test_amaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)      305 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/PyObjCTest/test_ambundleaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)      212 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/PyObjCTest/test_amshellscriptaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)      559 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/PyObjCTest/test_amworkflow.py
+-rw-r--r--   0 ronald     (501) staff       (20)      530 2022-06-25 20:07:56.000000 pyobjc-framework-Automator-9.2/PyObjCTest/test_amworkflowcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      307 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/PyObjCTest/test_amworkflowview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      259 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/PyObjCTest/test_amworkspace.py
+-rw-r--r--   0 ronald     (501) staff       (20)      842 2022-04-12 20:05:08.000000 pyobjc-framework-Automator-9.2/PyObjCTest/test_automator.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2879 2022-02-24 08:47:16.000000 pyobjc-framework-Automator-9.2/PyObjCTest/test_automatorerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)      286 2021-10-18 19:38:40.000000 pyobjc-framework-Automator-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.587230 pyobjc-framework-Automator-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     3883 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/metadata/Automator.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:54.607591 pyobjc-framework-Automator-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    36150 2021-07-30 09:00:37.000000 pyobjc-framework-Automator-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36254 2022-02-24 08:47:16.000000 pyobjc-framework-Automator-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31389 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    35772 2021-03-21 10:08:22.000000 pyobjc-framework-Automator-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    24376 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    26356 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    26444 2020-11-30 18:45:14.000000 pyobjc-framework-Automator-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36151 2021-07-30 09:00:37.000000 pyobjc-framework-Automator-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    36255 2022-02-24 08:47:16.000000 pyobjc-framework-Automator-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Automator-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Automator-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:06:54.609410 pyobjc-framework-Automator-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      954 2023-05-29 10:07:45.000000 pyobjc-framework-Automator-9.2/setup.py
```

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/AutoSample/Controller.py` & `pyobjc-framework-Automator-9.2/Examples/AutoSample/Controller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/AutoSample/English.lproj/MainMenu.nib/designable.nib` & `pyobjc-framework-Automator-9.2/Examples/AutoSample/English.lproj/MainMenu.nib/designable.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/AutoSample/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Automator-9.2/Examples/AutoSample/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/AutoSample/ReadMe.txt` & `pyobjc-framework-Automator-9.2/Examples/AutoSample/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/AutoSample/summary.txt` & `pyobjc-framework-Automator-9.2/Examples/AutoSample/summary.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Hello World.workflow/Contents/QuickLook/Preview.pdf` & `pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Hello World.workflow/Contents/QuickLook/Preview.pdf`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Hello World.workflow/Contents/document.wflow` & `pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Hello World.workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Run Automator.workflow/Contents/QuickLook/Preview.pdf` & `pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Run Automator.workflow/Contents/QuickLook/Preview.pdf`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Run Automator.workflow/Contents/document.wflow` & `pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Run Automator.workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Small Step.workflow/Contents/QuickLook/Preview.pdf` & `pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Small Step.workflow/Contents/QuickLook/Preview.pdf`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/AutoSample/workflows/Small Step.workflow/Contents/document.wflow` & `pyobjc-framework-Automator-9.2/Examples/AutoSample/workflows/Small Step.workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/Get Buddy Info/English.lproj/InfoPlist.strings` & `pyobjc-framework-Automator-9.2/Examples/Get Buddy Info/English.lproj/InfoPlist.strings`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/Get Buddy Info/GetBuddyInfo.py` & `pyobjc-framework-Automator-9.2/Examples/Get Buddy Info/GetBuddyInfo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/Get Buddy Info/Info.plist` & `pyobjc-framework-Automator-9.2/Examples/Get Buddy Info/Info.plist`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Examples/Get Buddy Info/setup.py` & `pyobjc-framework-Automator-9.2/Examples/Get Buddy Info/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/LICENSE.txt` & `pyobjc-framework-Automator-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Lib/Automator/__init__.py` & `pyobjc-framework-Automator-9.2/Lib/Automator/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Lib/Automator/_metadata.py` & `pyobjc-framework-Automator-9.2/Lib/Automator/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/Lib/pyobjc_framework_Automator.egg-info/PKG-INFO` & `pyobjc-framework-Automator-9.2/Lib/pyobjc_framework_Automator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Automator
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Automator on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Automator
 Platform: MacOS X
```

### Comparing `pyobjc-framework-Automator-9.1b1/Lib/pyobjc_framework_Automator.egg-info/SOURCES.txt` & `pyobjc-framework-Automator-9.2/Lib/pyobjc_framework_Automator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/AutoSample/Controller.py
 Examples/AutoSample/ReadMe.txt
 Examples/AutoSample/main.py
 Examples/AutoSample/setup.py
 Examples/AutoSample/summary.txt
 Examples/AutoSample/English.lproj/InfoPlist.strings
```

### Comparing `pyobjc-framework-Automator-9.1b1/PKG-INFO` & `pyobjc-framework-Automator-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Automator
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Automator on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Automator
 Platform: MacOS X
```

### Comparing `pyobjc-framework-Automator-9.1b1/PyObjCTest/test_amaction.py` & `pyobjc-framework-Automator-9.2/PyObjCTest/test_amaction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/PyObjCTest/test_amworkflow.py` & `pyobjc-framework-Automator-9.2/PyObjCTest/test_amworkflow.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/PyObjCTest/test_amworkflowcontroller.py` & `pyobjc-framework-Automator-9.2/PyObjCTest/test_amworkflowcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/PyObjCTest/test_automator.py` & `pyobjc-framework-Automator-9.2/PyObjCTest/test_automator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/PyObjCTest/test_automatorerrors.py` & `pyobjc-framework-Automator-9.2/PyObjCTest/test_automatorerrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/metadata/Automator.fwinfo` & `pyobjc-framework-Automator-9.2/metadata/Automator.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-Automator-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Automator-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-Automator-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-Automator-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-Automator-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-Automator-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-Automator-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-Automator-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Automator-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Automator-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Automator-9.1b1/setup.py` & `pyobjc-framework-Automator-9.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,23 @@
 a bundle that, when loaded and run, performs a specific task.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
-from pyobjc_setup import setup
+import os
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-Automator",
     description="Wrappers for the framework Automator on macOS",
     packages=["Automator"],
     version=VERSION,
     install_requires=["pyobjc-core>=" + VERSION, "pyobjc-framework-Cocoa>=" + VERSION],
```

