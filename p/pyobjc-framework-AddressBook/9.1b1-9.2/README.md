# Comparing `tmp/pyobjc-framework-AddressBook-9.1b1.tar.gz` & `tmp/pyobjc-framework-AddressBook-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-AddressBook-9.1b1.tar", last modified: Sun Mar 26 11:13:52 2023, max compression
+gzip compressed data, was "pyobjc-framework-AddressBook-9.2.tar", last modified: Wed Jun  7 00:05:39 2023, max compression
```

## Comparing `pyobjc-framework-AddressBook-9.1b1.tar` & `pyobjc-framework-AddressBook-9.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:52.237939 pyobjc-framework-AddressBook-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:52.097975 pyobjc-framework-AddressBook-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:52.096997 pyobjc-framework-AddressBook-9.1b1/Examples/Plugins/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:52.116167 pyobjc-framework-AddressBook-9.1b1/Examples/Plugins/Python Address Label/
--rw-r--r--   0 ronald     (501) staff       (20)     1431 2021-10-18 19:38:40.000000 pyobjc-framework-AddressBook-9.1b1/Examples/Plugins/Python Address Label/plugin.py
--rw-r--r--   0 ronald     (501) staff       (20)      270 2021-10-18 19:38:40.000000 pyobjc-framework-AddressBook-9.1b1/Examples/Plugins/Python Address Label/readme.txt
--rw-r--r--   0 ronald     (501) staff       (20)      743 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/Examples/Plugins/Python Address Label/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      106 2021-10-18 19:38:40.000000 pyobjc-framework-AddressBook-9.1b1/Examples/Plugins/Python Address Label/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:52.117907 pyobjc-framework-AddressBook-9.1b1/Examples/Scripts/
--rw-r--r--   0 ronald     (501) staff       (20)     2392 2022-01-02 11:20:34.000000 pyobjc-framework-AddressBook-9.1b1/Examples/Scripts/exportBook.py
--rw-r--r--   0 ronald     (501) staff       (20)      686 2021-10-18 19:38:40.000000 pyobjc-framework-AddressBook-9.1b1/Examples/Scripts/meInC.py
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AddressBook-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:52.098643 pyobjc-framework-AddressBook-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:52.127838 pyobjc-framework-AddressBook-9.1b1/Lib/AddressBook/
--rw-r--r--   0 ronald     (501) staff       (20)      769 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/Lib/AddressBook/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    24494 2022-02-24 08:47:16.000000 pyobjc-framework-AddressBook-9.1b1/Lib/AddressBook/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:52.137367 pyobjc-framework-AddressBook-9.1b1/Lib/pyobjc_framework_AddressBook.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2304 2023-03-26 11:13:52.000000 pyobjc-framework-AddressBook-9.1b1/Lib/pyobjc_framework_AddressBook.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1719 2023-03-26 11:13:52.000000 pyobjc-framework-AddressBook-9.1b1/Lib/pyobjc_framework_AddressBook.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:13:52.000000 pyobjc-framework-AddressBook-9.1b1/Lib/pyobjc_framework_AddressBook.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:16.000000 pyobjc-framework-AddressBook-9.1b1/Lib/pyobjc_framework_AddressBook.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:13:52.000000 pyobjc-framework-AddressBook-9.1b1/Lib/pyobjc_framework_AddressBook.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       12 2023-03-26 11:13:52.000000 pyobjc-framework-AddressBook-9.1b1/Lib/pyobjc_framework_AddressBook.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:52.149378 pyobjc-framework-AddressBook-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      829 2021-10-18 19:38:40.000000 pyobjc-framework-AddressBook-9.1b1/Modules/_AddressBook.m
--rw-r--r--   0 ronald     (501) staff       (20)      487 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/Modules/_AddressBook_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-AddressBook-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-AddressBook-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2093 2023-03-26 11:13:52.237406 pyobjc-framework-AddressBook-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:52.182778 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      383 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abactions.py
--rw-r--r--   0 ronald     (501) staff       (20)     1599 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abaddressbook.py
--rw-r--r--   0 ronald     (501) staff       (20)    17554 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abaddressbookc.py
--rw-r--r--   0 ronald     (501) staff       (20)     9544 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abglobals.py
--rw-r--r--   0 ronald     (501) staff       (20)      509 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abgroup.py
--rw-r--r--   0 ronald     (501) staff       (20)      529 2022-06-25 08:58:53.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abimageloading.py
--rw-r--r--   0 ronald     (501) staff       (20)      572 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abmultivalue.py
--rw-r--r--   0 ronald     (501) staff       (20)     5884 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abpeoplepickerc.py
--rw-r--r--   0 ronald     (501) staff       (20)     1834 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abpeoplepickerview.py
--rw-r--r--   0 ronald     (501) staff       (20)      256 2022-06-25 20:17:17.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abpersonpickerdelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      322 2021-03-21 10:08:22.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abpersonpickler.py
--rw-r--r--   0 ronald     (501) staff       (20)      580 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abpersonview.py
--rw-r--r--   0 ronald     (501) staff       (20)      577 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abrecord.py
--rw-r--r--   0 ronald     (501) staff       (20)      206 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_absearchelement.py
--rw-r--r--   0 ronald     (501) staff       (20)     3828 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abtypedefs.py
--rw-r--r--   0 ronald     (501) staff       (20)     3567 2023-03-04 17:22:26.000000 pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_addressbook.py
--rw-r--r--   0 ronald     (501) staff       (20)      330 2021-10-18 19:38:40.000000 pyobjc-framework-AddressBook-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:52.191216 pyobjc-framework-AddressBook-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    26447 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/metadata/AddressBook.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      202 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:13:52.229507 pyobjc-framework-AddressBook-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    76173 2021-07-30 09:00:37.000000 pyobjc-framework-AddressBook-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    76341 2022-02-24 08:47:16.000000 pyobjc-framework-AddressBook-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    75979 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    76174 2021-03-21 10:08:22.000000 pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    64577 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    68262 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    68866 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    77119 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-10.9.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    76174 2021-07-30 09:00:37.000000 pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    76342 2022-02-24 08:47:16.000000 pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AddressBook-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:13:52.238051 pyobjc-framework-AddressBook-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1302 2023-03-25 14:20:30.000000 pyobjc-framework-AddressBook-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:39.228567 pyobjc-framework-AddressBook-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:39.160824 pyobjc-framework-AddressBook-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:39.160616 pyobjc-framework-AddressBook-9.2/Examples/Plugins/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:39.169176 pyobjc-framework-AddressBook-9.2/Examples/Plugins/Python Address Label/
+-rw-r--r--   0 ronald     (501) staff       (20)     1431 2021-10-18 19:38:40.000000 pyobjc-framework-AddressBook-9.2/Examples/Plugins/Python Address Label/plugin.py
+-rw-r--r--   0 ronald     (501) staff       (20)      270 2021-10-18 19:38:40.000000 pyobjc-framework-AddressBook-9.2/Examples/Plugins/Python Address Label/readme.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      743 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/Examples/Plugins/Python Address Label/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      106 2021-10-18 19:38:40.000000 pyobjc-framework-AddressBook-9.2/Examples/Plugins/Python Address Label/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:39.170704 pyobjc-framework-AddressBook-9.2/Examples/Scripts/
+-rw-r--r--   0 ronald     (501) staff       (20)     2392 2022-01-02 11:20:34.000000 pyobjc-framework-AddressBook-9.2/Examples/Scripts/exportBook.py
+-rw-r--r--   0 ronald     (501) staff       (20)      686 2021-10-18 19:38:40.000000 pyobjc-framework-AddressBook-9.2/Examples/Scripts/meInC.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AddressBook-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:39.161371 pyobjc-framework-AddressBook-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:39.172113 pyobjc-framework-AddressBook-9.2/Lib/AddressBook/
+-rw-r--r--   0 ronald     (501) staff       (20)      769 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/Lib/AddressBook/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    24494 2022-02-24 08:47:16.000000 pyobjc-framework-AddressBook-9.2/Lib/AddressBook/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:39.175639 pyobjc-framework-AddressBook-9.2/Lib/pyobjc_framework_AddressBook.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2302 2023-06-07 00:05:39.000000 pyobjc-framework-AddressBook-9.2/Lib/pyobjc_framework_AddressBook.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1734 2023-06-07 00:05:39.000000 pyobjc-framework-AddressBook-9.2/Lib/pyobjc_framework_AddressBook.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:05:39.000000 pyobjc-framework-AddressBook-9.2/Lib/pyobjc_framework_AddressBook.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:16.000000 pyobjc-framework-AddressBook-9.2/Lib/pyobjc_framework_AddressBook.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:05:39.000000 pyobjc-framework-AddressBook-9.2/Lib/pyobjc_framework_AddressBook.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       12 2023-06-07 00:05:39.000000 pyobjc-framework-AddressBook-9.2/Lib/pyobjc_framework_AddressBook.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:39.180993 pyobjc-framework-AddressBook-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      829 2021-10-18 19:38:40.000000 pyobjc-framework-AddressBook-9.2/Modules/_AddressBook.m
+-rw-r--r--   0 ronald     (501) staff       (20)      487 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/Modules/_AddressBook_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-AddressBook-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:21.000000 pyobjc-framework-AddressBook-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2091 2023-06-07 00:05:39.228187 pyobjc-framework-AddressBook-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:39.206199 pyobjc-framework-AddressBook-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      383 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abactions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1599 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abaddressbook.py
+-rw-r--r--   0 ronald     (501) staff       (20)    17554 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abaddressbookc.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9544 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abglobals.py
+-rw-r--r--   0 ronald     (501) staff       (20)      509 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abgroup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      529 2022-06-25 08:58:53.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abimageloading.py
+-rw-r--r--   0 ronald     (501) staff       (20)      572 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abmultivalue.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5884 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abpeoplepickerc.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1834 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abpeoplepickerview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      256 2022-06-25 20:17:17.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abpersonpickerdelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      322 2021-03-21 10:08:22.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abpersonpickler.py
+-rw-r--r--   0 ronald     (501) staff       (20)      580 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abpersonview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      577 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abrecord.py
+-rw-r--r--   0 ronald     (501) staff       (20)      206 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_absearchelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3828 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abtypedefs.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3887 2023-05-04 11:00:07.000000 pyobjc-framework-AddressBook-9.2/PyObjCTest/test_addressbook.py
+-rw-r--r--   0 ronald     (501) staff       (20)      330 2021-10-18 19:38:40.000000 pyobjc-framework-AddressBook-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:39.208444 pyobjc-framework-AddressBook-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    26447 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/metadata/AddressBook.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:05:39.227024 pyobjc-framework-AddressBook-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    76173 2021-07-30 09:00:37.000000 pyobjc-framework-AddressBook-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    76341 2022-02-24 08:47:16.000000 pyobjc-framework-AddressBook-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    75979 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    76174 2021-03-21 10:08:22.000000 pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    64577 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    68262 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    68866 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    77119 2020-11-30 18:45:14.000000 pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-10.9.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    76174 2021-07-30 09:00:37.000000 pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    76342 2022-02-24 08:47:16.000000 pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AddressBook-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-AddressBook-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:05:39.228685 pyobjc-framework-AddressBook-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1373 2023-05-29 10:07:45.000000 pyobjc-framework-AddressBook-9.2/setup.py
```

### Comparing `pyobjc-framework-AddressBook-9.1b1/Examples/Plugins/Python Address Label/plugin.py` & `pyobjc-framework-AddressBook-9.2/Examples/Plugins/Python Address Label/plugin.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/Examples/Plugins/Python Address Label/setup.py` & `pyobjc-framework-AddressBook-9.2/Examples/Plugins/Python Address Label/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/Examples/Scripts/exportBook.py` & `pyobjc-framework-AddressBook-9.2/Examples/Scripts/exportBook.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/Examples/Scripts/meInC.py` & `pyobjc-framework-AddressBook-9.2/Examples/Scripts/meInC.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/LICENSE.txt` & `pyobjc-framework-AddressBook-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/Lib/AddressBook/__init__.py` & `pyobjc-framework-AddressBook-9.2/Lib/AddressBook/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/Lib/AddressBook/_metadata.py` & `pyobjc-framework-AddressBook-9.2/Lib/AddressBook/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/Lib/pyobjc_framework_AddressBook.egg-info/PKG-INFO` & `pyobjc-framework-AddressBook-9.2/Lib/pyobjc_framework_AddressBook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AddressBook
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AddressBook on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AddressBook
 Platform: MacOS X
```

### Comparing `pyobjc-framework-AddressBook-9.1b1/Lib/pyobjc_framework_AddressBook.egg-info/SOURCES.txt` & `pyobjc-framework-AddressBook-9.2/Lib/pyobjc_framework_AddressBook.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/Plugins/Python Address Label/plugin.py
 Examples/Plugins/Python Address Label/readme.txt
 Examples/Plugins/Python Address Label/setup.py
 Examples/Plugins/Python Address Label/summary.txt
 Examples/Scripts/exportBook.py
 Examples/Scripts/meInC.py
```

### Comparing `pyobjc-framework-AddressBook-9.1b1/Modules/_AddressBook.m` & `pyobjc-framework-AddressBook-9.2/Modules/_AddressBook.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-AddressBook-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-AddressBook-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-AddressBook-9.1b1/PKG-INFO` & `pyobjc-framework-AddressBook-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AddressBook
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AddressBook on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AddressBook
 Platform: MacOS X
```

### Comparing `pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abaddressbook.py` & `pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abaddressbook.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abaddressbookc.py` & `pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abaddressbookc.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abglobals.py` & `pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abglobals.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abimageloading.py` & `pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abimageloading.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abmultivalue.py` & `pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abmultivalue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abpeoplepickerc.py` & `pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abpeoplepickerc.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abpeoplepickerview.py` & `pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abpeoplepickerview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abpersonview.py` & `pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abpersonview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abrecord.py` & `pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abrecord.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_abtypedefs.py` & `pyobjc-framework-AddressBook-9.2/PyObjCTest/test_abtypedefs.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/PyObjCTest/test_addressbook.py` & `pyobjc-framework-AddressBook-9.2/PyObjCTest/test_addressbook.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,9 +68,13 @@
                 ("ABPersonRef", "globalAPILockForAddressBook_inFile_line_"),
                 ("ABGroupRef", "abGlobalAPILockInFile_line_"),
                 ("ABGroupRef", "abGlobalAPILockInFile_line_togglingSuddenTermination_"),
                 ("ABGroupRef", "abGlobalAPITryLockInFile_line_"),
                 ("ABGroupRef", "globalAPIUnlockForAddressBook_inFile_line_"),
                 ("ABGroupRef", "abGlobalAPILockInFile_line_contextBlock_"),
                 ("ABGroupRef", "globalAPILockForAddressBook_inFile_line_"),
+                ("ABAddressBookRef", "abGlobalMailRecentAPILockInFile_line_"),
+                ("ABAddressBookRef", "abGlobalMailRecentAPIUnlockInFile_line_"),
+                ("ABAddressBookRef", "abGlobalMailRecentAPILockInFile_line_"),
+                ("ABAddressBookRef", "abGlobalMailRecentAPIUnlockInFile_line_"),
             },
         )
```

### Comparing `pyobjc-framework-AddressBook-9.1b1/metadata/AddressBook.fwinfo` & `pyobjc-framework-AddressBook-9.2/metadata/AddressBook.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-AddressBook-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-AddressBook-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-10.9.fwinfo` & `pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-10.9.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-AddressBook-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/pyobjc_setup.py` & `pyobjc-framework-AddressBook-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AddressBook-9.1b1/setup.py` & `pyobjc-framework-AddressBook-9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,22 @@
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
     name="pyobjc-framework-AddressBook",
     description="Wrappers for the framework AddressBook on macOS",
     packages=["AddressBook"],
     ext_modules=[
         Extension(
```

