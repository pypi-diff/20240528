# Comparing `tmp/pyobjc-framework-CalendarStore-9.1b1.tar.gz` & `tmp/pyobjc-framework-CalendarStore-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CalendarStore-9.1b1.tar", last modified: Sun Mar 26 11:16:20 2023, max compression
+gzip compressed data, was "pyobjc-framework-CalendarStore-9.2.tar", last modified: Wed Jun  7 00:07:29 2023, max compression
```

## Comparing `pyobjc-framework-CalendarStore-9.1b1.tar` & `pyobjc-framework-CalendarStore-9.2.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:20.523959 pyobjc-framework-CalendarStore-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:20.396763 pyobjc-framework-CalendarStore-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:20.414441 pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/
--rw-r--r--   0 ronald     (501) staff       (20)     5133 2023-03-03 17:21:59.000000 pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/AppController.py
--rw-r--r--   0 ronald     (501) staff       (20)     4722 2021-03-21 10:08:22.000000 pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/CalController.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:20.396507 pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:20.417668 pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)     1715 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      473 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    43347 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      166 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      321 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      222 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:20.426911 pyobjc-framework-CalendarStore-9.1b1/Examples/Scripts/
--rw-r--r--   0 ronald     (501) staff       (20)     1564 2021-07-30 09:00:37.000000 pyobjc-framework-CalendarStore-9.1b1/Examples/Scripts/add_wwdc_to_calendar.py
--rw-r--r--   0 ronald     (501) staff       (20)      298 2021-07-30 09:00:37.000000 pyobjc-framework-CalendarStore-9.1b1/Examples/Scripts/print_calendars.py
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CalendarStore-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:20.397283 pyobjc-framework-CalendarStore-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:20.429526 pyobjc-framework-CalendarStore-9.1b1/Lib/CalendarStore/
--rw-r--r--   0 ronald     (501) staff       (20)      717 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/Lib/CalendarStore/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3097 2022-02-24 08:47:16.000000 pyobjc-framework-CalendarStore-9.1b1/Lib/CalendarStore/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:20.434008 pyobjc-framework-CalendarStore-9.1b1/Lib/pyobjc_framework_CalendarStore.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2357 2023-03-26 11:16:20.000000 pyobjc-framework-CalendarStore-9.1b1/Lib/pyobjc_framework_CalendarStore.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1621 2023-03-26 11:16:20.000000 pyobjc-framework-CalendarStore-9.1b1/Lib/pyobjc_framework_CalendarStore.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:16:20.000000 pyobjc-framework-CalendarStore-9.1b1/Lib/pyobjc_framework_CalendarStore.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:27.000000 pyobjc-framework-CalendarStore-9.1b1/Lib/pyobjc_framework_CalendarStore.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:16:20.000000 pyobjc-framework-CalendarStore-9.1b1/Lib/pyobjc_framework_CalendarStore.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       14 2023-03-26 11:16:20.000000 pyobjc-framework-CalendarStore-9.1b1/Lib/pyobjc_framework_CalendarStore.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     2146 2023-03-26 11:16:20.523121 pyobjc-framework-CalendarStore-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:20.455995 pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      413 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calalarm.py
--rw-r--r--   0 ronald     (501) staff       (20)      438 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calattendee.py
--rw-r--r--   0 ronald     (501) staff       (20)      741 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calcalendar.py
--rw-r--r--   0 ronald     (501) staff       (20)      204 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calcalendaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)     2237 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calcalendarstore.py
--rw-r--r--   0 ronald     (501) staff       (20)      545 2022-04-11 08:03:15.000000 pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calendarstore.py
--rw-r--r--   0 ronald     (501) staff       (20)      428 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calendarstoreerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)      327 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      572 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calrecurrencerule.py
--rw-r--r--   0 ronald     (501) staff       (20)      529 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_caltask.py
--rw-r--r--   0 ronald     (501) staff       (20)      290 2021-10-18 19:38:40.000000 pyobjc-framework-CalendarStore-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:20.457260 pyobjc-framework-CalendarStore-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2897 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/metadata/CalendarStore.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       70 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:20.521675 pyobjc-framework-CalendarStore-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    43312 2021-07-30 09:00:37.000000 pyobjc-framework-CalendarStore-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43331 2022-02-24 08:47:16.000000 pyobjc-framework-CalendarStore-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    42977 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43313 2021-03-21 10:08:22.000000 pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    25567 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    25627 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    26710 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43313 2021-07-30 09:00:37.000000 pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43332 2022-02-24 08:47:16.000000 pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CalendarStore-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:16:20.524126 pyobjc-framework-CalendarStore-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      887 2023-03-25 14:20:30.000000 pyobjc-framework-CalendarStore-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:29.690828 pyobjc-framework-CalendarStore-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:29.631429 pyobjc-framework-CalendarStore-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:29.640097 pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/
+-rw-r--r--   0 ronald     (501) staff       (20)     5133 2023-03-03 17:21:59.000000 pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/AppController.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4722 2021-03-21 10:08:22.000000 pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/CalController.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:29.631222 pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:29.646356 pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)     1715 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      473 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    43347 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      166 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      321 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      222 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:29.647817 pyobjc-framework-CalendarStore-9.2/Examples/Scripts/
+-rw-r--r--   0 ronald     (501) staff       (20)     1564 2021-07-30 09:00:37.000000 pyobjc-framework-CalendarStore-9.2/Examples/Scripts/add_wwdc_to_calendar.py
+-rw-r--r--   0 ronald     (501) staff       (20)      298 2021-07-30 09:00:37.000000 pyobjc-framework-CalendarStore-9.2/Examples/Scripts/print_calendars.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CalendarStore-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:29.631964 pyobjc-framework-CalendarStore-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:29.649256 pyobjc-framework-CalendarStore-9.2/Lib/CalendarStore/
+-rw-r--r--   0 ronald     (501) staff       (20)      717 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/Lib/CalendarStore/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3097 2022-02-24 08:47:16.000000 pyobjc-framework-CalendarStore-9.2/Lib/CalendarStore/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:29.652433 pyobjc-framework-CalendarStore-9.2/Lib/pyobjc_framework_CalendarStore.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2355 2023-06-07 00:07:29.000000 pyobjc-framework-CalendarStore-9.2/Lib/pyobjc_framework_CalendarStore.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1636 2023-06-07 00:07:29.000000 pyobjc-framework-CalendarStore-9.2/Lib/pyobjc_framework_CalendarStore.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:07:29.000000 pyobjc-framework-CalendarStore-9.2/Lib/pyobjc_framework_CalendarStore.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:27.000000 pyobjc-framework-CalendarStore-9.2/Lib/pyobjc_framework_CalendarStore.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:07:29.000000 pyobjc-framework-CalendarStore-9.2/Lib/pyobjc_framework_CalendarStore.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2023-06-07 00:07:29.000000 pyobjc-framework-CalendarStore-9.2/Lib/pyobjc_framework_CalendarStore.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     2144 2023-06-07 00:07:29.690353 pyobjc-framework-CalendarStore-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:29.670206 pyobjc-framework-CalendarStore-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      413 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calalarm.py
+-rw-r--r--   0 ronald     (501) staff       (20)      438 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calattendee.py
+-rw-r--r--   0 ronald     (501) staff       (20)      741 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calcalendar.py
+-rw-r--r--   0 ronald     (501) staff       (20)      204 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calcalendaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2237 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calcalendarstore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      545 2022-04-11 08:03:15.000000 pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calendarstore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      428 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calendarstoreerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)      327 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      572 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calrecurrencerule.py
+-rw-r--r--   0 ronald     (501) staff       (20)      529 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_caltask.py
+-rw-r--r--   0 ronald     (501) staff       (20)      290 2021-10-18 19:38:40.000000 pyobjc-framework-CalendarStore-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:29.672160 pyobjc-framework-CalendarStore-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2897 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/metadata/CalendarStore.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       70 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:29.689191 pyobjc-framework-CalendarStore-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    43312 2021-07-30 09:00:37.000000 pyobjc-framework-CalendarStore-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43331 2022-02-24 08:47:16.000000 pyobjc-framework-CalendarStore-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    42977 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43313 2021-03-21 10:08:22.000000 pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    25567 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    25627 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    26710 2020-11-30 18:45:14.000000 pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43313 2021-07-30 09:00:37.000000 pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43332 2022-02-24 08:47:16.000000 pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CalendarStore-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CalendarStore-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:07:29.690935 pyobjc-framework-CalendarStore-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      969 2023-05-29 10:07:45.000000 pyobjc-framework-CalendarStore-9.2/setup.py
```

### Comparing `pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/AppController.py` & `pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/AppController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/CalController.py` & `pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/CalController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/Examples/Coding Headstart/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-CalendarStore-9.2/Examples/Coding Headstart/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/Examples/Scripts/add_wwdc_to_calendar.py` & `pyobjc-framework-CalendarStore-9.2/Examples/Scripts/add_wwdc_to_calendar.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/LICENSE.txt` & `pyobjc-framework-CalendarStore-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/Lib/CalendarStore/__init__.py` & `pyobjc-framework-CalendarStore-9.2/Lib/CalendarStore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/Lib/CalendarStore/_metadata.py` & `pyobjc-framework-CalendarStore-9.2/Lib/CalendarStore/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/Lib/pyobjc_framework_CalendarStore.egg-info/PKG-INFO` & `pyobjc-framework-CalendarStore-9.2/Lib/pyobjc_framework_CalendarStore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CalendarStore
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CalendarStore on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CalendarStore
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-CalendarStore-9.1b1/Lib/pyobjc_framework_CalendarStore.egg-info/SOURCES.txt` & `pyobjc-framework-CalendarStore-9.2/Lib/pyobjc_framework_CalendarStore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/Coding Headstart/AppController.py
 Examples/Coding Headstart/CalController.py
 Examples/Coding Headstart/main.py
 Examples/Coding Headstart/setup.py
 Examples/Coding Headstart/summary.txt
 Examples/Coding Headstart/English.lproj/MainMenu.nib/classes.nib
```

### Comparing `pyobjc-framework-CalendarStore-9.1b1/PKG-INFO` & `pyobjc-framework-CalendarStore-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CalendarStore
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CalendarStore on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CalendarStore
 Platform: MacOS X (>=10.5)
```

### Comparing `pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calcalendar.py` & `pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calcalendar.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calcalendarstore.py` & `pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calcalendarstore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calendarstore.py` & `pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calendarstore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_calrecurrencerule.py` & `pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_calrecurrencerule.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/PyObjCTest/test_caltask.py` & `pyobjc-framework-CalendarStore-9.2/PyObjCTest/test_caltask.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/metadata/CalendarStore.fwinfo` & `pyobjc-framework-CalendarStore-9.2/metadata/CalendarStore.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CalendarStore-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CalendarStore-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CalendarStore-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CalendarStore-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CalendarStore-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

