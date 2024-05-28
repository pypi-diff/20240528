# Comparing `tmp/pyobjc-framework-DiscRecording-9.1b1.tar.gz` & `tmp/pyobjc-framework-DiscRecording-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-DiscRecording-9.1b1.tar", last modified: Sun Mar 26 11:23:16 2023, max compression
+gzip compressed data, was "pyobjc-framework-DiscRecording-9.2.tar", last modified: Wed Jun  7 00:13:21 2023, max compression
```

## Comparing `pyobjc-framework-DiscRecording-9.1b1.tar` & `pyobjc-framework-DiscRecording-9.2.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:16.452494 pyobjc-framework-DiscRecording-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:16.365835 pyobjc-framework-DiscRecording-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:16.372099 pyobjc-framework-DiscRecording-9.1b1/Lib/DiscRecording/
--rw-r--r--   0 ronald     (501) staff       (20)     1379 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.1b1/Lib/DiscRecording/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    39292 2022-02-24 08:47:16.000000 pyobjc-framework-DiscRecording-9.1b1/Lib/DiscRecording/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:16.385986 pyobjc-framework-DiscRecording-9.1b1/Lib/pyobjc_framework_DiscRecording.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2114 2023-03-26 11:23:16.000000 pyobjc-framework-DiscRecording-9.1b1/Lib/pyobjc_framework_DiscRecording.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1635 2023-03-26 11:23:16.000000 pyobjc-framework-DiscRecording-9.1b1/Lib/pyobjc_framework_DiscRecording.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:23:16.000000 pyobjc-framework-DiscRecording-9.1b1/Lib/pyobjc_framework_DiscRecording.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:00.000000 pyobjc-framework-DiscRecording-9.1b1/Lib/pyobjc_framework_DiscRecording.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:23:16.000000 pyobjc-framework-DiscRecording-9.1b1/Lib/pyobjc_framework_DiscRecording.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       14 2023-03-26 11:23:16.000000 pyobjc-framework-DiscRecording-9.1b1/Lib/pyobjc_framework_DiscRecording.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-DiscRecording-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:16.395874 pyobjc-framework-DiscRecording-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1156 2021-10-18 19:38:40.000000 pyobjc-framework-DiscRecording-9.1b1/Modules/_DiscRecording.m
--rw-r--r--   0 ronald     (501) staff       (20)      266 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.1b1/Modules/_DiscRecording_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-DiscRecording-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-DiscRecording-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1903 2023-03-26 11:23:16.451985 pyobjc-framework-DiscRecording-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:16.426641 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      310 2022-04-11 08:03:15.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_discrecording.py
--rw-r--r--   0 ronald     (501) staff       (20)     2115 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drburn.py
--rw-r--r--   0 ronald     (501) staff       (20)     3978 2021-04-09 10:15:21.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcdtext.py
--rw-r--r--   0 ronald     (501) staff       (20)     2539 2022-01-02 11:04:26.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcontentfile.py
--rw-r--r--   0 ronald     (501) staff       (20)      870 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcontentfolder.py
--rw-r--r--   0 ronald     (501) staff       (20)     3471 2021-04-09 10:15:21.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcontentobject.py
--rw-r--r--   0 ronald     (501) staff       (20)     4626 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcontentproperties.py
--rw-r--r--   0 ronald     (501) staff       (20)      484 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcontenttrack.py
--rw-r--r--   0 ronald     (501) staff       (20)     2472 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcoreburn.py
--rw-r--r--   0 ronald     (501) staff       (20)     4757 2021-04-09 10:15:21.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcorecdtext.py
--rw-r--r--   0 ronald     (501) staff       (20)    11685 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcoredevice.py
--rw-r--r--   0 ronald     (501) staff       (20)      940 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcoreerase.py
--rw-r--r--   0 ronald     (501) staff       (20)     4202 2021-04-09 10:15:21.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcoreerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)      881 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcorenotifications.py
--rw-r--r--   0 ronald     (501) staff       (20)      428 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcoreobject.py
--rw-r--r--   0 ronald     (501) staff       (20)     1841 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcorestatus.py
--rw-r--r--   0 ronald     (501) staff       (20)     7250 2022-01-02 11:04:26.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcoretrack.py
--rw-r--r--   0 ronald     (501) staff       (20)    11185 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drdevice.py
--rw-r--r--   0 ronald     (501) staff       (20)      411 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drerase.py
--rw-r--r--   0 ronald     (501) staff       (20)     2586 2022-06-25 09:09:58.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drfile.py
--rw-r--r--   0 ronald     (501) staff       (20)     3960 2022-10-18 09:53:24.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drfsObject.py
--rw-r--r--   0 ronald     (501) staff       (20)      189 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drmsf.py
--rw-r--r--   0 ronald     (501) staff       (20)     2355 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drstatus.py
--rw-r--r--   0 ronald     (501) staff       (20)    10762 2022-06-25 09:10:01.000000 pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drtrack.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:16.429257 pyobjc-framework-DiscRecording-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    13202 2022-02-06 09:24:04.000000 pyobjc-framework-DiscRecording-9.1b1/metadata/DiscRecording.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       42 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:23:16.449586 pyobjc-framework-DiscRecording-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   117695 2021-07-30 09:00:37.000000 pyobjc-framework-DiscRecording-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   117714 2022-02-24 08:47:16.000000 pyobjc-framework-DiscRecording-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   117929 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.1b1/metadata/raw/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   117944 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.1b1/metadata/raw/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   117696 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   117696 2021-07-30 09:00:37.000000 pyobjc-framework-DiscRecording-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   117715 2022-02-24 08:47:16.000000 pyobjc-framework-DiscRecording-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-DiscRecording-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:23:16.452612 pyobjc-framework-DiscRecording-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1305 2023-03-25 14:20:31.000000 pyobjc-framework-DiscRecording-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:21.230445 pyobjc-framework-DiscRecording-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:21.166011 pyobjc-framework-DiscRecording-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:21.174091 pyobjc-framework-DiscRecording-9.2/Lib/DiscRecording/
+-rw-r--r--   0 ronald     (501) staff       (20)     1379 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.2/Lib/DiscRecording/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    39221 2023-05-27 09:46:33.000000 pyobjc-framework-DiscRecording-9.2/Lib/DiscRecording/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:21.178671 pyobjc-framework-DiscRecording-9.2/Lib/pyobjc_framework_DiscRecording.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2112 2023-06-07 00:13:21.000000 pyobjc-framework-DiscRecording-9.2/Lib/pyobjc_framework_DiscRecording.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1650 2023-06-07 00:13:21.000000 pyobjc-framework-DiscRecording-9.2/Lib/pyobjc_framework_DiscRecording.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:13:21.000000 pyobjc-framework-DiscRecording-9.2/Lib/pyobjc_framework_DiscRecording.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:00.000000 pyobjc-framework-DiscRecording-9.2/Lib/pyobjc_framework_DiscRecording.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:13:21.000000 pyobjc-framework-DiscRecording-9.2/Lib/pyobjc_framework_DiscRecording.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       14 2023-06-07 00:13:21.000000 pyobjc-framework-DiscRecording-9.2/Lib/pyobjc_framework_DiscRecording.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-DiscRecording-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:21.181939 pyobjc-framework-DiscRecording-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1156 2021-10-18 19:38:40.000000 pyobjc-framework-DiscRecording-9.2/Modules/_DiscRecording.m
+-rw-r--r--   0 ronald     (501) staff       (20)      266 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.2/Modules/_DiscRecording_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-DiscRecording-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-DiscRecording-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1901 2023-06-07 00:13:21.230049 pyobjc-framework-DiscRecording-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:21.213370 pyobjc-framework-DiscRecording-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      310 2022-04-11 08:03:15.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_discrecording.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2115 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drburn.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3978 2021-04-09 10:15:21.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcdtext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2539 2022-01-02 11:04:26.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcontentfile.py
+-rw-r--r--   0 ronald     (501) staff       (20)      870 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcontentfolder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3471 2021-04-09 10:15:21.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcontentobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4626 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcontentproperties.py
+-rw-r--r--   0 ronald     (501) staff       (20)      484 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcontenttrack.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2472 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcoreburn.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4757 2021-04-09 10:15:21.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcorecdtext.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11685 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcoredevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)      940 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcoreerase.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4202 2021-04-09 10:15:21.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcoreerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)      881 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcorenotifications.py
+-rw-r--r--   0 ronald     (501) staff       (20)      432 2023-05-27 09:46:33.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcoreobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1841 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcorestatus.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7250 2022-01-02 11:04:26.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcoretrack.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11185 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drdevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)      411 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drerase.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2586 2022-06-25 09:09:58.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drfile.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3960 2022-10-18 09:53:24.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drfsObject.py
+-rw-r--r--   0 ronald     (501) staff       (20)      189 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drmsf.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2355 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drstatus.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10762 2022-06-25 09:10:01.000000 pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drtrack.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:21.217994 pyobjc-framework-DiscRecording-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    13242 2023-05-27 09:46:33.000000 pyobjc-framework-DiscRecording-9.2/metadata/DiscRecording.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       42 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:13:21.228880 pyobjc-framework-DiscRecording-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   117695 2021-07-30 09:00:37.000000 pyobjc-framework-DiscRecording-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   117714 2022-02-24 08:47:16.000000 pyobjc-framework-DiscRecording-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   117929 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.2/metadata/raw/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   117944 2020-11-30 18:45:14.000000 pyobjc-framework-DiscRecording-9.2/metadata/raw/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   117696 2021-03-21 10:08:22.000000 pyobjc-framework-DiscRecording-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   117696 2021-07-30 09:00:37.000000 pyobjc-framework-DiscRecording-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   117715 2022-02-24 08:47:16.000000 pyobjc-framework-DiscRecording-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-DiscRecording-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-DiscRecording-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:13:21.230556 pyobjc-framework-DiscRecording-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1220 2023-05-29 10:07:46.000000 pyobjc-framework-DiscRecording-9.2/setup.py
```

### Comparing `pyobjc-framework-DiscRecording-9.1b1/Lib/DiscRecording/__init__.py` & `pyobjc-framework-DiscRecording-9.2/Lib/DiscRecording/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/Lib/DiscRecording/_metadata.py` & `pyobjc-framework-DiscRecording-9.2/Lib/DiscRecording/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sun Feb 20 18:48:57 2022
+# Last update: Sat May 20 12:05:06 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -56,14 +56,15 @@
         ),
     }
 )
 constants = """$DRAbstractFile$DRAccessDate$DRAllFilesystems$DRApplicationIdentifier$DRAttributeModificationDate$DRAudioFourChannelKey$DRAudioPreEmphasisKey$DRBackupDate$DRBibliographicFile$DRBlockSize$DRBlockSizeKey$DRBlockTypeKey$DRBurnAppendableKey$DRBurnCompletionActionEject$DRBurnCompletionActionKey$DRBurnCompletionActionMount$DRBurnDoubleLayerL0DataZoneBlocksKey$DRBurnFailureActionEject$DRBurnFailureActionKey$DRBurnFailureActionNone$DRBurnOverwriteDiscKey$DRBurnRequestedSpeedKey$DRBurnStatusChangedNotification$DRBurnStrategyBDDAO$DRBurnStrategyCDSAO$DRBurnStrategyCDTAO$DRBurnStrategyDVDDAO$DRBurnStrategyIsRequiredKey$DRBurnStrategyKey$DRBurnTestingKey$DRBurnUnderrunProtectionKey$DRBurnVerifyDiscKey$DRCDTextArrangerKey$DRCDTextCharacterCodeKey$DRCDTextClosedKey$DRCDTextComposerKey$DRCDTextCopyrightAssertedForNamesKey$DRCDTextCopyrightAssertedForSpecialMessagesKey$DRCDTextCopyrightAssertedForTitlesKey$DRCDTextDiscIdentKey$DRCDTextGenreCodeKey$DRCDTextGenreKey$DRCDTextKey$DRCDTextLanguageKey$DRCDTextMCNISRCKey$DRCDTextNSStringEncodingKey$DRCDTextPerformerKey$DRCDTextSizeKey$DRCDTextSongwriterKey$DRCDTextSpecialMessageKey$DRCDTextTOC2Key$DRCDTextTOCKey$DRCDTextTitleKey$DRContentModificationDate$DRCopyrightFile$DRCreationDate$DRDVDCopyrightInfoKey$DRDVDTimestampKey$DRDataFormKey$DRDataPreparer$DRDefaultDate$DRDeviceAppearedNotification$DRDeviceBurnSpeedBD1x@f$DRDeviceBurnSpeedCD1x@f$DRDeviceBurnSpeedDVD1x@f$DRDeviceBurnSpeedHDDVD1x@f$DRDeviceBurnSpeedMax@f$DRDeviceBurnSpeedsKey$DRDeviceCanTestWriteCDKey$DRDeviceCanTestWriteDVDKey$DRDeviceCanUnderrunProtectCDKey$DRDeviceCanUnderrunProtectDVDKey$DRDeviceCanWriteBDKey$DRDeviceCanWriteBDREKey$DRDeviceCanWriteBDRKey$DRDeviceCanWriteCDKey$DRDeviceCanWriteCDRKey$DRDeviceCanWriteCDRWKey$DRDeviceCanWriteCDRawKey$DRDeviceCanWriteCDSAOKey$DRDeviceCanWriteCDTAOKey$DRDeviceCanWriteCDTextKey$DRDeviceCanWriteDVDDAOKey$DRDeviceCanWriteDVDKey$DRDeviceCanWriteDVDPlusRDoubleLayerKey$DRDeviceCanWriteDVDPlusRKey$DRDeviceCanWriteDVDPlusRWDoubleLayerKey$DRDeviceCanWriteDVDPlusRWKey$DRDeviceCanWriteDVDRAMKey$DRDeviceCanWriteDVDRDualLayerKey$DRDeviceCanWriteDVDRKey$DRDeviceCanWriteDVDRWDualLayerKey$DRDeviceCanWriteDVDRWKey$DRDeviceCanWriteHDDVDKey$DRDeviceCanWriteHDDVDRAMKey$DRDeviceCanWriteHDDVDRDualLayerKey$DRDeviceCanWriteHDDVDRKey$DRDeviceCanWriteHDDVDRWDualLayerKey$DRDeviceCanWriteHDDVDRWKey$DRDeviceCanWriteISRCKey$DRDeviceCanWriteIndexPointsKey$DRDeviceCanWriteKey$DRDeviceCurrentWriteSpeedKey$DRDeviceDisappearedNotification$DRDeviceFirmwareRevisionKey$DRDeviceIORegistryEntryPathKey$DRDeviceIsBusyKey$DRDeviceIsTrayOpenKey$DRDeviceLoadingMechanismCanEjectKey$DRDeviceLoadingMechanismCanInjectKey$DRDeviceLoadingMechanismCanOpenKey$DRDeviceMaximumWriteSpeedKey$DRDeviceMediaBSDNameKey$DRDeviceMediaBlocksFreeKey$DRDeviceMediaBlocksOverwritableKey$DRDeviceMediaBlocksUsedKey$DRDeviceMediaClassBD$DRDeviceMediaClassCD$DRDeviceMediaClassDVD$DRDeviceMediaClassHDDVD$DRDeviceMediaClassKey$DRDeviceMediaClassUnknown$DRDeviceMediaDoubleLayerL0DataZoneBlocksKey$DRDeviceMediaFreeSpaceKey$DRDeviceMediaInfoKey$DRDeviceMediaIsAppendableKey$DRDeviceMediaIsBlankKey$DRDeviceMediaIsErasableKey$DRDeviceMediaIsOverwritableKey$DRDeviceMediaIsReservedKey$DRDeviceMediaOverwritableSpaceKey$DRDeviceMediaSessionCountKey$DRDeviceMediaStateInTransition$DRDeviceMediaStateKey$DRDeviceMediaStateMediaPresent$DRDeviceMediaStateNone$DRDeviceMediaTrackCountKey$DRDeviceMediaTypeBDR$DRDeviceMediaTypeBDRE$DRDeviceMediaTypeBDROM$DRDeviceMediaTypeCDR$DRDeviceMediaTypeCDROM$DRDeviceMediaTypeCDRW$DRDeviceMediaTypeDVDPlusR$DRDeviceMediaTypeDVDPlusRDoubleLayer$DRDeviceMediaTypeDVDPlusRW$DRDeviceMediaTypeDVDPlusRWDoubleLayer$DRDeviceMediaTypeDVDR$DRDeviceMediaTypeDVDRAM$DRDeviceMediaTypeDVDRDualLayer$DRDeviceMediaTypeDVDROM$DRDeviceMediaTypeDVDRW$DRDeviceMediaTypeDVDRWDualLayer$DRDeviceMediaTypeHDDVDR$DRDeviceMediaTypeHDDVDRAM$DRDeviceMediaTypeHDDVDRDualLayer$DRDeviceMediaTypeHDDVDROM$DRDeviceMediaTypeHDDVDRW$DRDeviceMediaTypeHDDVDRWDualLayer$DRDeviceMediaTypeKey$DRDeviceMediaTypeUnknown$DRDeviceMediaUsedSpaceKey$DRDevicePhysicalInterconnectATAPI$DRDevicePhysicalInterconnectFibreChannel$DRDevicePhysicalInterconnectFireWire$DRDevicePhysicalInterconnectKey$DRDevicePhysicalInterconnectLocationExternal$DRDevicePhysicalInterconnectLocationInternal$DRDevicePhysicalInterconnectLocationKey$DRDevicePhysicalInterconnectLocationUnknown$DRDevicePhysicalInterconnectSCSI$DRDevicePhysicalInterconnectUSB$DRDeviceProductNameKey$DRDeviceStatusChangedNotification$DRDeviceSupportLevelAppleShipping$DRDeviceSupportLevelAppleSupported$DRDeviceSupportLevelKey$DRDeviceSupportLevelNone$DRDeviceSupportLevelUnsupported$DRDeviceSupportLevelVendorSupported$DRDeviceTrackInfoKey$DRDeviceTrackRefsKey$DRDeviceVendorNameKey$DRDeviceWriteBufferSizeKey$DRDeviceWriteCapabilitiesKey$DREffectiveDate$DREraseStatusChangedNotification$DREraseTypeComplete$DREraseTypeKey$DREraseTypeQuick$DRErrorStatusAdditionalSenseStringKey$DRErrorStatusErrorInfoStringKey$DRErrorStatusErrorKey$DRErrorStatusErrorStringKey$DRErrorStatusKey$DRErrorStatusSenseCodeStringKey$DRErrorStatusSenseKey$DRExpirationDate$DRFreeBlocksKey$DRHFSPlus$DRHFSPlusCatalogNodeID$DRHFSPlusTextEncodingHint$DRISO9660$DRISO9660LevelOne$DRISO9660LevelTwo$DRISO9660VersionNumber$DRISOLevel$DRISOMacExtensions$DRISORockRidgeExtensions$DRIndexPointsKey$DRInvisible$DRJoliet$DRLinkTypeFinderAlias$DRLinkTypeHardLink$DRLinkTypeSymbolicLink$DRMacExtendedFinderFlags$DRMacFileCreator$DRMacFileType$DRMacFinderFlags$DRMacFinderHideExtension$DRMacIconLocation$DRMacScrollPosition$DRMacWindowBounds$DRMacWindowView$DRMaxBurnSpeedKey$DRMediaCatalogNumberKey$DRNextWritableAddressKey$DRPosixFileMode$DRPosixGID$DRPosixUID$DRPreGapIsRequiredKey$DRPreGapLengthKey$DRPublisher$DRRecordingDate$DRSCMSCopyrightFree$DRSCMSCopyrightProtectedCopy$DRSCMSCopyrightProtectedOriginal$DRSerialCopyManagementStateKey$DRSessionFormatKey$DRSessionNumberKey$DRStatusCurrentSessionKey$DRStatusCurrentSpeedKey$DRStatusCurrentTrackKey$DRStatusEraseTypeKey$DRStatusPercentCompleteKey$DRStatusProgressCurrentKPS$DRStatusProgressCurrentXFactor$DRStatusProgressInfoKey$DRStatusStateDone$DRStatusStateErasing$DRStatusStateFailed$DRStatusStateFinishing$DRStatusStateKey$DRStatusStateNone$DRStatusStatePreparing$DRStatusStateSessionClose$DRStatusStateSessionOpen$DRStatusStateTrackClose$DRStatusStateTrackOpen$DRStatusStateTrackWrite$DRStatusStateVerifying$DRStatusTotalSessionsKey$DRStatusTotalTracksKey$DRSubchannelDataFormKey$DRSubchannelDataFormNone$DRSubchannelDataFormPack$DRSubchannelDataFormRaw$DRSuppressMacSpecificFiles$DRSynchronousBehaviorKey$DRSystemIdentifier$DRTrackISRCKey$DRTrackIsEmptyKey$DRTrackLengthKey$DRTrackModeKey$DRTrackNumberKey$DRTrackPacketSizeKey$DRTrackPacketTypeFixed$DRTrackPacketTypeKey$DRTrackPacketTypeVariable$DRTrackStartAddressKey$DRTrackTypeClosed$DRTrackTypeIncomplete$DRTrackTypeInvisible$DRTrackTypeKey$DRTrackTypeReserved$DRUDF$DRUDFApplicationIdentifierSuffix$DRUDFExtendedFilePermissions$DRUDFInterchangeLevel$DRUDFMaxInterchangeLevel$DRUDFMaxVolumeSequenceNumber$DRUDFPrimaryVolumeDescriptorNumber$DRUDFRealTimeFile$DRUDFVersion102$DRUDFVersion150$DRUDFVolumeSequenceNumber$DRUDFVolumeSetIdentifier$DRUDFVolumeSetImplementationUse$DRUDFVolumeSetTimestamp$DRUDFWriteVersion$DRVerificationTypeChecksum$DRVerificationTypeKey$DRVerificationTypeNone$DRVerificationTypeProduceAgain$DRVerificationTypeReceiveData$DRVolumeCheckedDate$DRVolumeCreationDate$DRVolumeEffectiveDate$DRVolumeExpirationDate$DRVolumeModificationDate$DRVolumeSet$kDRAbstractFile$kDRAccessDate$kDRAllFilesystems$kDRApplicationIdentifier$kDRAttributeModificationDate$kDRAudioFourChannelKey$kDRAudioPreEmphasisKey$kDRBackupDate$kDRBibliographicFile$kDRBlockSize$kDRBlockSizeKey$kDRBlockTypeKey$kDRBufferZone1DataKey$kDRBurnAppendableKey$kDRBurnCompletionActionEject$kDRBurnCompletionActionKey$kDRBurnCompletionActionMount$kDRBurnDoubleLayerL0DataZoneBlocksKey$kDRBurnFailureActionEject$kDRBurnFailureActionKey$kDRBurnFailureActionNone$kDRBurnKey$kDRBurnOverwriteDiscKey$kDRBurnRequestedSpeedKey$kDRBurnStatusChangedNotification$kDRBurnStrategyBDDAO$kDRBurnStrategyCDSAO$kDRBurnStrategyCDTAO$kDRBurnStrategyDVDDAO$kDRBurnStrategyIsRequiredKey$kDRBurnStrategyKey$kDRBurnTestingKey$kDRBurnUnderrunProtectionKey$kDRBurnVerifyDiscKey$kDRCDTextArrangerKey$kDRCDTextCFStringEncodingKey$kDRCDTextCharacterCodeKey$kDRCDTextClosedKey$kDRCDTextComposerKey$kDRCDTextCopyrightAssertedForNamesKey$kDRCDTextCopyrightAssertedForSpecialMessagesKey$kDRCDTextCopyrightAssertedForTitlesKey$kDRCDTextDiscIdentKey$kDRCDTextGenreCodeKey$kDRCDTextGenreKey$kDRCDTextKey$kDRCDTextLanguageKey$kDRCDTextMCNISRCKey$kDRCDTextPerformerKey$kDRCDTextSizeKey$kDRCDTextSongwriterKey$kDRCDTextSpecialMessageKey$kDRCDTextTOC2Key$kDRCDTextTOCKey$kDRCDTextTitleKey$kDRContentModificationDate$kDRCopyrightFile$kDRCreationDate$kDRDVDCopyrightInfoKey$kDRDVDTimestampKey$kDRDataFormKey$kDRDataPreparer$kDRDefaultDate$kDRDeviceAppearedNotification$kDRDeviceBurnSpeedBD1x@f$kDRDeviceBurnSpeedCD1x@f$kDRDeviceBurnSpeedDVD1x@f$kDRDeviceBurnSpeedHDDVD1x@f$kDRDeviceBurnSpeedMax@f$kDRDeviceBurnSpeedsKey$kDRDeviceCanTestWriteCDKey$kDRDeviceCanTestWriteDVDKey$kDRDeviceCanUnderrunProtectCDKey$kDRDeviceCanUnderrunProtectDVDKey$kDRDeviceCanWriteBDKey$kDRDeviceCanWriteBDREKey$kDRDeviceCanWriteBDRKey$kDRDeviceCanWriteCDKey$kDRDeviceCanWriteCDRKey$kDRDeviceCanWriteCDRWKey$kDRDeviceCanWriteCDRawKey$kDRDeviceCanWriteCDSAOKey$kDRDeviceCanWriteCDTAOKey$kDRDeviceCanWriteCDTextKey$kDRDeviceCanWriteDVDDAOKey$kDRDeviceCanWriteDVDKey$kDRDeviceCanWriteDVDPlusRDoubleLayerKey$kDRDeviceCanWriteDVDPlusRKey$kDRDeviceCanWriteDVDPlusRWDoubleLayerKey$kDRDeviceCanWriteDVDPlusRWKey$kDRDeviceCanWriteDVDRAMKey$kDRDeviceCanWriteDVDRDualLayerKey$kDRDeviceCanWriteDVDRKey$kDRDeviceCanWriteDVDRWDualLayerKey$kDRDeviceCanWriteDVDRWKey$kDRDeviceCanWriteHDDVDKey$kDRDeviceCanWriteHDDVDRAMKey$kDRDeviceCanWriteHDDVDRDualLayerKey$kDRDeviceCanWriteHDDVDRKey$kDRDeviceCanWriteHDDVDRWDualLayerKey$kDRDeviceCanWriteHDDVDRWKey$kDRDeviceCanWriteISRCKey$kDRDeviceCanWriteIndexPointsKey$kDRDeviceCanWriteKey$kDRDeviceCurrentWriteSpeedKey$kDRDeviceDisappearedNotification$kDRDeviceFirmwareRevisionKey$kDRDeviceIORegistryEntryPathKey$kDRDeviceIsBusyKey$kDRDeviceIsTrayOpenKey$kDRDeviceLoadingMechanismCanEjectKey$kDRDeviceLoadingMechanismCanInjectKey$kDRDeviceLoadingMechanismCanOpenKey$kDRDeviceMaximumWriteSpeedKey$kDRDeviceMediaBSDNameKey$kDRDeviceMediaBlocksFreeKey$kDRDeviceMediaBlocksOverwritableKey$kDRDeviceMediaBlocksUsedKey$kDRDeviceMediaClassBD$kDRDeviceMediaClassCD$kDRDeviceMediaClassDVD$kDRDeviceMediaClassHDDVD$kDRDeviceMediaClassKey$kDRDeviceMediaClassUnknown$kDRDeviceMediaDoubleLayerL0DataZoneBlocksKey$kDRDeviceMediaInfoKey$kDRDeviceMediaIsAppendableKey$kDRDeviceMediaIsBlankKey$kDRDeviceMediaIsErasableKey$kDRDeviceMediaIsOverwritableKey$kDRDeviceMediaIsReservedKey$kDRDeviceMediaSessionCountKey$kDRDeviceMediaStateInTransition$kDRDeviceMediaStateKey$kDRDeviceMediaStateMediaPresent$kDRDeviceMediaStateNone$kDRDeviceMediaTrackCountKey$kDRDeviceMediaTypeBDR$kDRDeviceMediaTypeBDRE$kDRDeviceMediaTypeBDROM$kDRDeviceMediaTypeCDR$kDRDeviceMediaTypeCDROM$kDRDeviceMediaTypeCDRW$kDRDeviceMediaTypeDVDPlusR$kDRDeviceMediaTypeDVDPlusRDoubleLayer$kDRDeviceMediaTypeDVDPlusRW$kDRDeviceMediaTypeDVDPlusRWDoubleLayer$kDRDeviceMediaTypeDVDR$kDRDeviceMediaTypeDVDRAM$kDRDeviceMediaTypeDVDRDualLayer$kDRDeviceMediaTypeDVDROM$kDRDeviceMediaTypeDVDRW$kDRDeviceMediaTypeDVDRWDualLayer$kDRDeviceMediaTypeHDDVDR$kDRDeviceMediaTypeHDDVDRAM$kDRDeviceMediaTypeHDDVDRDualLayer$kDRDeviceMediaTypeHDDVDROM$kDRDeviceMediaTypeHDDVDRW$kDRDeviceMediaTypeHDDVDRWDualLayer$kDRDeviceMediaTypeKey$kDRDeviceMediaTypeUnknown$kDRDevicePhysicalInterconnectATAPI$kDRDevicePhysicalInterconnectFibreChannel$kDRDevicePhysicalInterconnectFireWire$kDRDevicePhysicalInterconnectKey$kDRDevicePhysicalInterconnectLocationExternal$kDRDevicePhysicalInterconnectLocationInternal$kDRDevicePhysicalInterconnectLocationKey$kDRDevicePhysicalInterconnectLocationUnknown$kDRDevicePhysicalInterconnectSCSI$kDRDevicePhysicalInterconnectUSB$kDRDeviceProductNameKey$kDRDeviceStatusChangedNotification$kDRDeviceSupportLevelAppleShipping$kDRDeviceSupportLevelAppleSupported$kDRDeviceSupportLevelKey$kDRDeviceSupportLevelNone$kDRDeviceSupportLevelUnsupported$kDRDeviceSupportLevelVendorSupported$kDRDeviceTrackInfoKey$kDRDeviceTrackRefsKey$kDRDeviceVendorNameKey$kDRDeviceWriteBufferSizeKey$kDRDeviceWriteCapabilitiesKey$kDREffectiveDate$kDREraseStatusChangedNotification$kDREraseTypeComplete$kDREraseTypeKey$kDREraseTypeQuick$kDRErrorStatusAdditionalSenseStringKey$kDRErrorStatusErrorInfoStringKey$kDRErrorStatusErrorKey$kDRErrorStatusErrorStringKey$kDRErrorStatusKey$kDRErrorStatusSenseCodeStringKey$kDRErrorStatusSenseKey$kDRExpirationDate$kDRFreeBlocksKey$kDRHFSPlus$kDRHFSPlusCatalogNodeID$kDRHFSPlusTextEncodingHint$kDRISO9660$kDRISO9660LevelOne$kDRISO9660LevelTwo$kDRISO9660VersionNumber$kDRISOLevel$kDRISOMacExtensions$kDRISORockRidgeExtensions$kDRIndexPointsKey$kDRInvisible$kDRJoliet$kDRMacExtendedFinderFlags$kDRMacFileCreator$kDRMacFileType$kDRMacFinderFlags$kDRMacFinderHideExtension$kDRMacIconLocation$kDRMacScrollPosition$kDRMacWindowBounds$kDRMacWindowView$kDRMaxBurnSpeedKey$kDRMediaCatalogNumberKey$kDRNextWritableAddressKey$kDRPosixFileMode$kDRPosixGID$kDRPosixUID$kDRPreGapIsRequiredKey$kDRPreGapLengthKey$kDRPublisher$kDRRecordingDate$kDRSCMSCopyrightFree$kDRSCMSCopyrightProtectedCopy$kDRSCMSCopyrightProtectedOriginal$kDRSerialCopyManagementStateKey$kDRSessionFormatKey$kDRSessionNumberKey$kDRStatusCurrentSessionKey$kDRStatusCurrentSpeedKey$kDRStatusCurrentTrackKey$kDRStatusEraseTypeKey$kDRStatusPercentCompleteKey$kDRStatusProgressCurrentKPS$kDRStatusProgressCurrentXFactor$kDRStatusProgressInfoKey$kDRStatusStateDone$kDRStatusStateErasing$kDRStatusStateFailed$kDRStatusStateFinishing$kDRStatusStateKey$kDRStatusStateNone$kDRStatusStatePreparing$kDRStatusStateSessionClose$kDRStatusStateSessionOpen$kDRStatusStateTrackClose$kDRStatusStateTrackOpen$kDRStatusStateTrackWrite$kDRStatusStateVerifying$kDRStatusTotalSessionsKey$kDRStatusTotalTracksKey$kDRSubchannelDataFormKey$kDRSubchannelDataFormNone$kDRSubchannelDataFormPack$kDRSubchannelDataFormRaw$kDRSuppressMacSpecificFiles$kDRSynchronousBehaviorKey$kDRSystemIdentifier$kDRTrackISRCKey$kDRTrackIsEmptyKey$kDRTrackLengthKey$kDRTrackModeKey$kDRTrackNumberKey$kDRTrackPacketSizeKey$kDRTrackPacketTypeFixed$kDRTrackPacketTypeKey$kDRTrackPacketTypeVariable$kDRTrackStartAddressKey$kDRTrackTypeClosed$kDRTrackTypeIncomplete$kDRTrackTypeInvisible$kDRTrackTypeKey$kDRTrackTypeReserved$kDRUDF$kDRUDFApplicationIdentifierSuffix$kDRUDFExtendedFilePermissions$kDRUDFInterchangeLevel$kDRUDFMaxInterchangeLevel$kDRUDFMaxVolumeSequenceNumber$kDRUDFPrimaryVolumeDescriptorNumber$kDRUDFRealTimeFile$kDRUDFVersion102$kDRUDFVersion150$kDRUDFVolumeSequenceNumber$kDRUDFVolumeSetIdentifier$kDRUDFVolumeSetImplementationUse$kDRUDFVolumeSetTimestamp$kDRUDFWriteVersion$kDRVerificationTypeChecksum$kDRVerificationTypeKey$kDRVerificationTypeNone$kDRVerificationTypeProduceAgain$kDRVerificationTypeReceiveData$kDRVolumeCheckedDate$kDRVolumeCreationDate$kDRVolumeEffectiveDate$kDRVolumeExpirationDate$kDRVolumeModificationDate$kDRVolumeSet$"""
 enums = """$DRCDTextEncodingASCII@1$DRCDTextEncodingISOLatin1Modified@5$DRCDTextGenreCodeAdultContemporary@2$DRCDTextGenreCodeAlternativeRock@3$DRCDTextGenreCodeChildrens@4$DRCDTextGenreCodeClassical@5$DRCDTextGenreCodeContemporaryChristian@6$DRCDTextGenreCodeCountry@7$DRCDTextGenreCodeDance@8$DRCDTextGenreCodeEasyListening@9$DRCDTextGenreCodeErotic@10$DRCDTextGenreCodeFolk@11$DRCDTextGenreCodeGospel@12$DRCDTextGenreCodeHipHop@13$DRCDTextGenreCodeJazz@14$DRCDTextGenreCodeLatin@15$DRCDTextGenreCodeMusical@16$DRCDTextGenreCodeNewAge@17$DRCDTextGenreCodeOpera@18$DRCDTextGenreCodeOperetta@19$DRCDTextGenreCodePop@20$DRCDTextGenreCodeRap@21$DRCDTextGenreCodeReggae@22$DRCDTextGenreCodeRhythmAndBlues@24$DRCDTextGenreCodeRock@23$DRCDTextGenreCodeSoundEffects@25$DRCDTextGenreCodeSoundtrack@26$DRCDTextGenreCodeSpokenWord@27$DRCDTextGenreCodeUnknown@1$DRCDTextGenreCodeWorldMusic@28$DRFileForkData@0$DRFileForkResource@1$DRFilesystemInclusionMaskHFSPlus@8$DRFilesystemInclusionMaskISO9660@1$DRFilesystemInclusionMaskJoliet@2$DRFilesystemInclusionMaskUDF@4$DRFlagSubchannelDataRequested@2$kDRAudioFileNotSupportedErr@2147614828$kDRBadLayoutErr@2147614821$kDRBlockSizeAudio@2352$kDRBlockSizeDVDData@2048$kDRBlockSizeMode1Data@2048$kDRBlockSizeMode2Data@2332$kDRBlockSizeMode2Form1Data@2048$kDRBlockSizeMode2Form2Data@2324$kDRBlockTypeAudio@0$kDRBlockTypeDVDData@8$kDRBlockTypeMode1Data@8$kDRBlockTypeMode2Data@13$kDRBlockTypeMode2Form1Data@10$kDRBlockTypeMode2Form2Data@12$kDRBurnMediaWriteFailureErr@2147614830$kDRBurnNotAllowedErr@2147614817$kDRBurnPowerCalibrationErr@2147614829$kDRBurnUnderrunErr@2147614816$kDRCDTextEncodingASCII@1536$kDRCDTextEncodingISOLatin1Modified@513$kDRCDTextGenreCodeAdultContemporary@2$kDRCDTextGenreCodeAlternativeRock@3$kDRCDTextGenreCodeChildrens@4$kDRCDTextGenreCodeClassical@5$kDRCDTextGenreCodeContemporaryChristian@6$kDRCDTextGenreCodeCountry@7$kDRCDTextGenreCodeDance@8$kDRCDTextGenreCodeEasyListening@9$kDRCDTextGenreCodeErotic@10$kDRCDTextGenreCodeFolk@11$kDRCDTextGenreCodeGospel@12$kDRCDTextGenreCodeHipHop@13$kDRCDTextGenreCodeJazz@14$kDRCDTextGenreCodeLatin@15$kDRCDTextGenreCodeMusical@16$kDRCDTextGenreCodeNewAge@17$kDRCDTextGenreCodeOpera@18$kDRCDTextGenreCodeOperetta@19$kDRCDTextGenreCodePop@20$kDRCDTextGenreCodeRap@21$kDRCDTextGenreCodeReggae@22$kDRCDTextGenreCodeRhythmAndBlues@24$kDRCDTextGenreCodeRock@23$kDRCDTextGenreCodeSoundEffects@25$kDRCDTextGenreCodeSoundtrack@26$kDRCDTextGenreCodeSpokenWord@27$kDRCDTextGenreCodeUnknown@1$kDRCDTextGenreCodeWorldMusic@28$kDRDataFormAudio@0$kDRDataFormDVDData@16$kDRDataFormMode1Data@16$kDRDataFormMode2Data@32$kDRDataFormMode2Form1Data@32$kDRDataFormMode2Form2Data@32$kDRDataProductionErr@2147614818$kDRDeviceAccessErr@2147614752$kDRDeviceBurnStrategyNotAvailableErr@2147615232$kDRDeviceBusyErr@2147614753$kDRDeviceCantWriteCDTextErr@2147615233$kDRDeviceCantWriteISRCErr@2147615235$kDRDeviceCantWriteIndexPointsErr@2147615234$kDRDeviceCantWriteSCMSErr@2147615236$kDRDeviceCommunicationErr@2147614754$kDRDeviceInvalidErr@2147614755$kDRDeviceNotReadyErr@2147614756$kDRDeviceNotSupportedErr@2147614757$kDRDevicePreGapLengthNotValidErr@2147615237$kDRDoubleLayerL0AlreadySpecifiedErr@2147614827$kDRDoubleLayerL0DataZoneBlocksParamErr@2147614826$kDRFileForkData@0$kDRFileForkResource@1$kDRFileForkSizeActual@0$kDRFileForkSizeEstimate@1$kDRFileLocationConflictErr@2147614977$kDRFileMessageForkSize@1718839674$kDRFileMessagePostBurn@1886352244$kDRFileMessagePreBurn@1886545184$kDRFileMessageProduceData@1886547812$kDRFileMessageRelease@1652122912$kDRFileMessageVerificationStarting@1987208825$kDRFileModifiedDuringBurnErr@2147614976$kDRFilesystemMaskDefault@4294967295$kDRFilesystemMaskHFSPlus@8$kDRFilesystemMaskISO9660@1$kDRFilesystemMaskJoliet@2$kDRFilesystemMaskUDF@4$kDRFilesystemsNotSupportedErr@2147614979$kDRFirstErr@2147614720$kDRFlagNoMoreData@1$kDRFlagSubchannelDataRequested@2$kDRFunctionNotSupportedErr@2147614823$kDRInternalErr@2147614720$kDRInvalidIndexPointsErr@2147614825$kDRLinkTypeFinderAlias@3$kDRLinkTypeHardLink@1$kDRLinkTypeSymbolicLink@2$kDRMediaBusyErr@2147614784$kDRMediaInvalidErr@2147614790$kDRMediaNotBlankErr@2147614788$kDRMediaNotErasableErr@2147614789$kDRMediaNotPresentErr@2147614785$kDRMediaNotSupportedErr@2147614787$kDRMediaNotWritableErr@2147614786$kDRSessionFormatAudio@0$kDRSessionFormatCDI@16$kDRSessionFormatCDXA@32$kDRSessionFormatDVDData@0$kDRSessionFormatMode1Data@0$kDRSpeedTestAlreadyRunningErr@2147614824$kDRTooManyNameConflictsErr@2147614978$kDRTooManyTracksForDVDErr@2147614820$kDRTrackMessageEstimateLength@1702065257$kDRTrackMessagePostBurn@1886352244$kDRTrackMessagePreBurn@1886545184$kDRTrackMessageProduceData@1886547812$kDRTrackMessageProducePreGap@1886548082$kDRTrackMessageVerificationDone@1986293614$kDRTrackMessageVerificationStarting@1987277938$kDRTrackMessageVerifyData@1987208825$kDRTrackMessageVerifyPreGap@1987211378$kDRTrackMode1Data@4$kDRTrackMode2Data@4$kDRTrackMode2Form1Data@4$kDRTrackMode2Form2Data@4$kDRTrackModeAudio@0$kDRTrackModeDVDData@5$kDRTrackReusedErr@2147614831$kDRUserCanceledErr@2147614822$kDRVerificationFailedErr@2147614819$"""
 misc.update({})
 misc.update({})
+misc.update({})
 functions = {
     "DREraseCreate": (
         b"^{__DRErase=}^{__DRDevice=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "DRDeviceCopyStatus": (
@@ -132,17 +133,14 @@
     ),
     "DRDeviceIsValid": (b"Z^{__DRDevice=}",),
     "DRCopyLocalizedStringForValue": (
         b"^{__CFString=}^{__CFString=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
-    "DRNotificationCenterRemoveObserver": (
-        b"v^{__DRNotificationCenter=}^v^{__CFString=}@",
-    ),
     "DRBurnSetProperties": (b"v^{__DRBurn=}^{__CFDictionary=}",),
     "DRBurnGetTypeID": (b"Q",),
     "DRFSObjectSetSpecificName": (b"v@^{__CFString=}^{__CFString=}",),
     "DRFolderCreateReal": (
         b"^{__DRFolder=}^{FSRef=[80C]}",
         "",
         {
@@ -232,15 +230,14 @@
     ),
     "DRCopyLocalizedStringForSenseCode": (
         b"^{__CFString=}C",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "DRCDTextBlockFlatten": (b"I^{__DRCDTextBlock=}",),
-    "DRSetRefCon": (b"v@^v^{DRRefConCallbacks=Q^?^?}",),
     "DRFSObjectCopyRealURL": (
         b"^{__CFURL=}@",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "DRFileCreateVirtualLink": (
         b"^{__DRFile=}@I^{__CFString=}",
@@ -294,15 +291,17 @@
     ),
     "DRBurnCreate": (
         b"^{__DRBurn=}^{__DRDevice=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "DRDeviceReleaseExclusiveAccess": (b"v^{__DRDevice=}",),
-    "DRGetRefCon": (b"^v@",),
+    "DRNotificationCenterRemoveObserver": (
+        b"v^{__DRNotificationCenter=}^v^{__CFString=}@",
+    ),
     "DRGetVersion": (b"{NumVersion=CCCC}",),
     "DRFSObjectSetSpecificNames": (b"v@^{__CFDictionary=}",),
     "DRDeviceAcquireMediaReservation": (b"v^{__DRDevice=}",),
     "DRTrackSetProperties": (b"v^{__DRTrack=}^{__CFDictionary=}",),
     "DRFSObjectCopySpecificName": (
         b"^{__CFString=}@^{__CFString=}",
         "",
```

### Comparing `pyobjc-framework-DiscRecording-9.1b1/Lib/pyobjc_framework_DiscRecording.egg-info/PKG-INFO` & `pyobjc-framework-DiscRecording-9.2/Lib/pyobjc_framework_DiscRecording.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-DiscRecording
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework DiscRecording on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,DiscRecording
 Platform: MacOS X
```

### Comparing `pyobjc-framework-DiscRecording-9.1b1/Lib/pyobjc_framework_DiscRecording.egg-info/SOURCES.txt` & `pyobjc-framework-DiscRecording-9.2/Lib/pyobjc_framework_DiscRecording.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/DiscRecording/__init__.py
 Lib/DiscRecording/_metadata.py
 Lib/pyobjc_framework_DiscRecording.egg-info/PKG-INFO
 Lib/pyobjc_framework_DiscRecording.egg-info/SOURCES.txt
 Lib/pyobjc_framework_DiscRecording.egg-info/dependency_links.txt
 Lib/pyobjc_framework_DiscRecording.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-DiscRecording-9.1b1/License.txt` & `pyobjc-framework-DiscRecording-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/Modules/_DiscRecording.m` & `pyobjc-framework-DiscRecording-9.2/Modules/_DiscRecording.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-DiscRecording-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-DiscRecording-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PKG-INFO` & `pyobjc-framework-DiscRecording-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-DiscRecording
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework DiscRecording on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,DiscRecording
 Platform: MacOS X
```

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drburn.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drburn.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcdtext.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcdtext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcontentfile.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcontentfile.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcontentfolder.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcontentfolder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcontentobject.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcontentobject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcontentproperties.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcontentproperties.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcoreburn.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcoreburn.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcorecdtext.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcorecdtext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcoredevice.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcoredevice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcoreerase.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcoreerase.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcoreerrors.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcoreerrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcorenotifications.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcorenotifications.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcorestatus.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcorestatus.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drcoretrack.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drcoretrack.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drdevice.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drdevice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drfile.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drfile.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drfsObject.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drfsObject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drstatus.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drstatus.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/PyObjCTest/test_drtrack.py` & `pyobjc-framework-DiscRecording-9.2/PyObjCTest/test_drtrack.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/metadata/DiscRecording.fwinfo` & `pyobjc-framework-DiscRecording-9.2/metadata/DiscRecording.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -600,14 +600,15 @@
    },
    "DRFolderRemoveChild": {
     "args": {
      "0": {}
     }
    },
    "DRGetRefCon": {
+    "ignore": true,
     "retval": {}
    },
    "DRNotificationCenterAddObserver": {
     "args": {
      "0": {},
      "1": {},
      "2": {
@@ -654,14 +655,15 @@
     "args": {
      "0": {},
      "1": {},
      "2": {}
     }
    },
    "DRSetRefCon": {
+    "ignore": true,
     "args": {
      "1": {},
      "2": {}
     }
    },
    "DRTrackCreate": {
     "args": {
```

### Comparing `pyobjc-framework-DiscRecording-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-DiscRecording-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-DiscRecording-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/metadata/raw/x86_64-10.13.fwinfo` & `pyobjc-framework-DiscRecording-9.2/metadata/raw/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/metadata/raw/x86_64-10.14.fwinfo` & `pyobjc-framework-DiscRecording-9.2/metadata/raw/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-DiscRecording-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-DiscRecording-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-DiscRecording-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/pyobjc_setup.py` & `pyobjc-framework-DiscRecording-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-DiscRecording-9.1b1/setup.py` & `pyobjc-framework-DiscRecording-9.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,26 +3,24 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
-#
-# Distutils doesn't understand '.mm' as an extension
-#
-import distutils.unixccompiler
 import os
+import sys
 
-from pyobjc_setup import Extension, setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
 
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
-distutils.unixccompiler.UnixCCompiler.src_extensions.append(".mm")
 
 setup(
     name="pyobjc-framework-DiscRecording",
     description="Wrappers for the framework DiscRecording on macOS",
     packages=["DiscRecording"],
     ext_modules=[
         Extension(
```

