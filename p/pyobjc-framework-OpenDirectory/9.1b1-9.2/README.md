# Comparing `tmp/pyobjc-framework-OpenDirectory-9.1b1.tar.gz` & `tmp/pyobjc-framework-OpenDirectory-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-OpenDirectory-9.1b1.tar", last modified: Sun Mar 26 11:32:59 2023, max compression
+gzip compressed data, was "pyobjc-framework-OpenDirectory-9.2.tar", last modified: Wed Jun  7 00:22:56 2023, max compression
```

## Comparing `pyobjc-framework-OpenDirectory-9.1b1.tar` & `pyobjc-framework-OpenDirectory-9.2.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:59.932726 pyobjc-framework-OpenDirectory-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-OpenDirectory-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:59.743784 pyobjc-framework-OpenDirectory-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:59.758333 pyobjc-framework-OpenDirectory-9.1b1/Lib/CFOpenDirectory/
--rw-r--r--   0 ronald     (501) staff       (20)      871 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.1b1/Lib/CFOpenDirectory/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    39058 2022-02-24 08:47:16.000000 pyobjc-framework-OpenDirectory-9.1b1/Lib/CFOpenDirectory/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:59.759900 pyobjc-framework-OpenDirectory-9.1b1/Lib/OpenDirectory/
--rw-r--r--   0 ronald     (501) staff       (20)      628 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.1b1/Lib/OpenDirectory/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    13082 2022-04-11 19:51:08.000000 pyobjc-framework-OpenDirectory-9.1b1/Lib/OpenDirectory/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:59.776064 pyobjc-framework-OpenDirectory-9.1b1/Lib/pyobjc_framework_OpenDirectory.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2203 2023-03-26 11:32:59.000000 pyobjc-framework-OpenDirectory-9.1b1/Lib/pyobjc_framework_OpenDirectory.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1766 2023-03-26 11:32:59.000000 pyobjc-framework-OpenDirectory-9.1b1/Lib/pyobjc_framework_OpenDirectory.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:32:59.000000 pyobjc-framework-OpenDirectory-9.1b1/Lib/pyobjc_framework_OpenDirectory.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:45.000000 pyobjc-framework-OpenDirectory-9.1b1/Lib/pyobjc_framework_OpenDirectory.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:32:59.000000 pyobjc-framework-OpenDirectory-9.1b1/Lib/pyobjc_framework_OpenDirectory.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       30 2023-03-26 11:32:59.000000 pyobjc-framework-OpenDirectory-9.1b1/Lib/pyobjc_framework_OpenDirectory.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1992 2023-03-26 11:32:59.931675 pyobjc-framework-OpenDirectory-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:59.801923 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)        0 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      203 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfodcontext.py
--rw-r--r--   0 ronald     (501) staff       (20)     4214 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfodnode.py
--rw-r--r--   0 ronald     (501) staff       (20)     1183 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfodquery.py
--rw-r--r--   0 ronald     (501) staff       (20)     5991 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfodrecord.py
--rw-r--r--   0 ronald     (501) staff       (20)      663 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfodsession.py
--rw-r--r--   0 ronald     (501) staff       (20)      524 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfopendirectory.py
--rw-r--r--   0 ronald     (501) staff       (20)    40742 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfopendirectoryconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)     2782 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_odconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)     4194 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_odnode.py
--rw-r--r--   0 ronald     (501) staff       (20)      782 2022-06-25 20:15:50.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_odquery.py
--rw-r--r--   0 ronald     (501) staff       (20)     7002 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_odrecord.py
--rw-r--r--   0 ronald     (501) staff       (20)     1805 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_odsession.py
--rw-r--r--   0 ronald     (501) staff       (20)      748 2022-06-25 20:09:04.000000 pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_opendirectory.py
--rw-r--r--   0 ronald     (501) staff       (20)      292 2021-10-18 19:38:40.000000 pyobjc-framework-OpenDirectory-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:59.818895 pyobjc-framework-OpenDirectory-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    15439 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/CFOpenDirectory.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    42983 2022-04-11 19:41:20.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/OpenDirectory.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      505 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:59.889554 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/
--rw-r--r--   0 ronald     (501) staff       (20)    60856 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60925 2022-02-24 08:47:16.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    59891 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60301 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60663 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    43785 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    45263 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    45522 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60857 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60926 2022-02-24 08:47:16.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-12.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:32:59.921073 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/
--rw-r--r--   0 ronald     (501) staff       (20)   131911 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   131980 2022-02-24 08:47:16.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   130033 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   130443 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   131718 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    65165 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    66783 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    67042 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   131912 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   131981 2022-02-24 08:47:16.000000 pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-OpenDirectory-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:32:59.932875 pyobjc-framework-OpenDirectory-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      736 2023-03-25 14:20:32.000000 pyobjc-framework-OpenDirectory-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:56.814823 pyobjc-framework-OpenDirectory-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-OpenDirectory-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:56.743753 pyobjc-framework-OpenDirectory-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:56.753148 pyobjc-framework-OpenDirectory-9.2/Lib/CFOpenDirectory/
+-rw-r--r--   0 ronald     (501) staff       (20)      871 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.2/Lib/CFOpenDirectory/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    39161 2023-05-27 09:46:33.000000 pyobjc-framework-OpenDirectory-9.2/Lib/CFOpenDirectory/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:56.755705 pyobjc-framework-OpenDirectory-9.2/Lib/OpenDirectory/
+-rw-r--r--   0 ronald     (501) staff       (20)      628 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.2/Lib/OpenDirectory/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13082 2022-04-11 19:51:08.000000 pyobjc-framework-OpenDirectory-9.2/Lib/OpenDirectory/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:56.760346 pyobjc-framework-OpenDirectory-9.2/Lib/pyobjc_framework_OpenDirectory.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2201 2023-06-07 00:22:56.000000 pyobjc-framework-OpenDirectory-9.2/Lib/pyobjc_framework_OpenDirectory.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1781 2023-06-07 00:22:56.000000 pyobjc-framework-OpenDirectory-9.2/Lib/pyobjc_framework_OpenDirectory.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:22:56.000000 pyobjc-framework-OpenDirectory-9.2/Lib/pyobjc_framework_OpenDirectory.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:45.000000 pyobjc-framework-OpenDirectory-9.2/Lib/pyobjc_framework_OpenDirectory.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:22:56.000000 pyobjc-framework-OpenDirectory-9.2/Lib/pyobjc_framework_OpenDirectory.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2023-06-07 00:22:56.000000 pyobjc-framework-OpenDirectory-9.2/Lib/pyobjc_framework_OpenDirectory.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1990 2023-06-07 00:22:56.814420 pyobjc-framework-OpenDirectory-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:56.773670 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)        0 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      203 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfodcontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4214 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfodnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1183 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfodquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5991 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfodrecord.py
+-rw-r--r--   0 ronald     (501) staff       (20)      663 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfodsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      524 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfopendirectory.py
+-rw-r--r--   0 ronald     (501) staff       (20)    40742 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfopendirectoryconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2782 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_odconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4194 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_odnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)      782 2022-06-25 20:15:50.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_odquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7002 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_odrecord.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1805 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_odsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      748 2022-06-25 20:09:04.000000 pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_opendirectory.py
+-rw-r--r--   0 ronald     (501) staff       (20)      292 2021-10-18 19:38:40.000000 pyobjc-framework-OpenDirectory-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:56.777469 pyobjc-framework-OpenDirectory-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    15495 2023-05-27 09:46:33.000000 pyobjc-framework-OpenDirectory-9.2/metadata/CFOpenDirectory.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    42961 2023-05-27 09:46:33.000000 pyobjc-framework-OpenDirectory-9.2/metadata/OpenDirectory.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      505 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:56.795626 pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/
+-rw-r--r--   0 ronald     (501) staff       (20)    60856 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60925 2022-02-24 08:47:16.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    59891 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60301 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60663 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    43785 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    45263 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    45522 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60857 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60926 2022-02-24 08:47:16.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-12.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:56.812305 pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/
+-rw-r--r--   0 ronald     (501) staff       (20)   131911 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   131980 2022-02-24 08:47:16.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   130033 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   130443 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   131718 2021-03-21 10:08:23.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    65165 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    66783 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    67042 2020-11-30 18:45:15.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   131912 2021-07-30 09:00:38.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   131981 2022-02-24 08:47:16.000000 pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-OpenDirectory-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-OpenDirectory-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:22:56.814927 pyobjc-framework-OpenDirectory-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      818 2023-05-29 10:07:46.000000 pyobjc-framework-OpenDirectory-9.2/setup.py
```

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/LICENSE.txt` & `pyobjc-framework-OpenDirectory-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/Lib/CFOpenDirectory/__init__.py` & `pyobjc-framework-OpenDirectory-9.2/Lib/CFOpenDirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/Lib/CFOpenDirectory/_metadata.py` & `pyobjc-framework-OpenDirectory-9.2/Lib/CFOpenDirectory/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sun Feb 20 19:13:32 2022
+# Last update: Sat May 20 22:17:41 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -30,14 +30,15 @@
 
 
 misc = {}
 constants = """$kODAttributeTypeAccessControlEntry$kODAttributeTypeAddressLine1$kODAttributeTypeAddressLine2$kODAttributeTypeAddressLine3$kODAttributeTypeAdminLimits$kODAttributeTypeAdvertisedServices$kODAttributeTypeAlias$kODAttributeTypeAllAttributes$kODAttributeTypeAllTypes$kODAttributeTypeAltSecurityIdentities$kODAttributeTypeAreaCode$kODAttributeTypeAttrListRefCount$kODAttributeTypeAttrListRefs$kODAttributeTypeAttrListValueRefCount$kODAttributeTypeAttrListValueRefs$kODAttributeTypeAuthCredential$kODAttributeTypeAuthMethod$kODAttributeTypeAuthenticationAuthority$kODAttributeTypeAuthenticationHint$kODAttributeTypeAuthorityRevocationList$kODAttributeTypeAutomaticSearchPath$kODAttributeTypeAutomountInformation$kODAttributeTypeBirthday$kODAttributeTypeBootParams$kODAttributeTypeBuildVersion$kODAttributeTypeBuilding$kODAttributeTypeCACertificate$kODAttributeTypeCapacity$kODAttributeTypeCertificateRevocationList$kODAttributeTypeCity$kODAttributeTypeComment$kODAttributeTypeCompany$kODAttributeTypeComputers$kODAttributeTypeConfigAvailable$kODAttributeTypeConfigFile$kODAttributeTypeContactGUID$kODAttributeTypeContactPerson$kODAttributeTypeCopyTimestamp$kODAttributeTypeCoreFWVersion$kODAttributeTypeCountry$kODAttributeTypeCreationTimestamp$kODAttributeTypeCrossCertificatePair$kODAttributeTypeCustomSearchPath$kODAttributeTypeDNSDomain$kODAttributeTypeDNSName$kODAttributeTypeDNSNameServer$kODAttributeTypeDataStamp$kODAttributeTypeDateRecordCreated$kODAttributeTypeDepartment$kODAttributeTypeDirRefCount$kODAttributeTypeDirRefs$kODAttributeTypeEMailAddress$kODAttributeTypeEMailContacts$kODAttributeTypeENetAddress$kODAttributeTypeExpire$kODAttributeTypeFWVersion$kODAttributeTypeFaxNumber$kODAttributeTypeFirstName$kODAttributeTypeFullName$kODAttributeTypeFunctionalState$kODAttributeTypeGUID$kODAttributeTypeGroup$kODAttributeTypeGroupMembers$kODAttributeTypeGroupMembership$kODAttributeTypeGroupServices$kODAttributeTypeHTML$kODAttributeTypeHardwareUUID$kODAttributeTypeHomeDirectory$kODAttributeTypeHomeDirectoryQuota$kODAttributeTypeHomeDirectorySoftQuota$kODAttributeTypeHomeLocOwner$kODAttributeTypeHomePhoneNumber$kODAttributeTypeIMHandle$kODAttributeTypeIPAddress$kODAttributeTypeIPAddressAndENetAddress$kODAttributeTypeIPv6Address$kODAttributeTypeInternetAlias$kODAttributeTypeJPEGPhoto$kODAttributeTypeJobTitle$kODAttributeTypeKDCAuthKey$kODAttributeTypeKDCConfigData$kODAttributeTypeKerberosRealm$kODAttributeTypeKerberosServices$kODAttributeTypeKeywords$kODAttributeTypeLDAPReadReplicas$kODAttributeTypeLDAPSearchBaseSuffix$kODAttributeTypeLDAPWriteReplicas$kODAttributeTypeLastName$kODAttributeTypeLocalOnlySearchPath$kODAttributeTypeLocaleRelay$kODAttributeTypeLocaleSubnets$kODAttributeTypeLocation$kODAttributeTypeMCXFlags$kODAttributeTypeMCXSettings$kODAttributeTypeMIME$kODAttributeTypeMailAttribute$kODAttributeTypeMapCoordinates$kODAttributeTypeMapGUID$kODAttributeTypeMapURI$kODAttributeTypeMetaAmbiguousName$kODAttributeTypeMetaAugmentedAttributes$kODAttributeTypeMetaAutomountMap$kODAttributeTypeMetaNodeLocation$kODAttributeTypeMetaRecordName$kODAttributeTypeMiddleName$kODAttributeTypeMobileNumber$kODAttributeTypeModificationTimestamp$kODAttributeTypeNFSHomeDirectory$kODAttributeTypeNTDomainComputerAccount$kODAttributeTypeNamePrefix$kODAttributeTypeNameSuffix$kODAttributeTypeNativeOnly$kODAttributeTypeNestedGroups$kODAttributeTypeNetGroupTriplet$kODAttributeTypeNetGroups$kODAttributeTypeNetworkInterfaces$kODAttributeTypeNetworkNumber$kODAttributeTypeNickName$kODAttributeTypeNodeOptions$kODAttributeTypeNodePath$kODAttributeTypeNodeRefCount$kODAttributeTypeNodeRefs$kODAttributeTypeNodeSASLRealm$kODAttributeTypeNote$kODAttributeTypeNumTableList$kODAttributeTypeOperatingSystem$kODAttributeTypeOperatingSystemVersion$kODAttributeTypeOrganizationInfo$kODAttributeTypeOrganizationName$kODAttributeTypeOriginalHomeDirectory$kODAttributeTypeOriginalNFSHomeDirectory$kODAttributeTypeOriginalNodeName$kODAttributeTypeOwner$kODAttributeTypeOwnerGUID$kODAttributeTypePGPPublicKey$kODAttributeTypePIDValue$kODAttributeTypePagerNumber$kODAttributeTypeParentLocales$kODAttributeTypePassword$kODAttributeTypePasswordPlus$kODAttributeTypePasswordPolicyOptions$kODAttributeTypePasswordServerList$kODAttributeTypePasswordServerLocation$kODAttributeTypePhoneContacts$kODAttributeTypePhoneNumber$kODAttributeTypePicture$kODAttributeTypePlugInInfo$kODAttributeTypePluginIndex$kODAttributeTypePort$kODAttributeTypePostalAddress$kODAttributeTypePostalAddressContacts$kODAttributeTypePostalCode$kODAttributeTypePresetUserIsAdmin$kODAttributeTypePrimaryComputerGUID$kODAttributeTypePrimaryComputerList$kODAttributeTypePrimaryGroupID$kODAttributeTypePrimaryLocale$kODAttributeTypePrimaryNTDomain$kODAttributeTypePrintServiceInfoText$kODAttributeTypePrintServiceInfoXML$kODAttributeTypePrintServiceUserData$kODAttributeTypePrinter1284DeviceID$kODAttributeTypePrinterLPRHost$kODAttributeTypePrinterLPRQueue$kODAttributeTypePrinterMakeAndModel$kODAttributeTypePrinterType$kODAttributeTypePrinterURI$kODAttributeTypePrinterXRISupported$kODAttributeTypeProcessName$kODAttributeTypeProfiles$kODAttributeTypeProfilesTimestamp$kODAttributeTypeProtocolNumber$kODAttributeTypeProtocols$kODAttributeTypePwdAgingPolicy$kODAttributeTypeRPCNumber$kODAttributeTypeReadOnlyNode$kODAttributeTypeRealUserID$kODAttributeTypeRecRefCount$kODAttributeTypeRecRefs$kODAttributeTypeRecordName$kODAttributeTypeRecordType$kODAttributeTypeRelationships$kODAttributeTypeRelativeDNPrefix$kODAttributeTypeResourceInfo$kODAttributeTypeResourceType$kODAttributeTypeSMBAcctFlags$kODAttributeTypeSMBGroupRID$kODAttributeTypeSMBHome$kODAttributeTypeSMBHomeDrive$kODAttributeTypeSMBKickoffTime$kODAttributeTypeSMBLogoffTime$kODAttributeTypeSMBLogonTime$kODAttributeTypeSMBPWDLastSet$kODAttributeTypeSMBPrimaryGroupSID$kODAttributeTypeSMBProfilePath$kODAttributeTypeSMBRID$kODAttributeTypeSMBSID$kODAttributeTypeSMBScriptPath$kODAttributeTypeSMBUserWorkstations$kODAttributeTypeSchema$kODAttributeTypeSearchPath$kODAttributeTypeSearchPolicy$kODAttributeTypeServiceType$kODAttributeTypeServicesLocator$kODAttributeTypeSetupAdvertising$kODAttributeTypeSetupAutoRegister$kODAttributeTypeSetupLocation$kODAttributeTypeSetupOccupation$kODAttributeTypeStandardOnly$kODAttributeTypeState$kODAttributeTypeStreet$kODAttributeTypeSubNodes$kODAttributeTypeTimePackage$kODAttributeTypeTimeToLive$kODAttributeTypeTotalRefCount$kODAttributeTypeTotalSize$kODAttributeTypeTrustInformation$kODAttributeTypeURL$kODAttributeTypeUniqueID$kODAttributeTypeUserCertificate$kODAttributeTypeUserPKCS12Data$kODAttributeTypeUserSMIMECertificate$kODAttributeTypeUserShell$kODAttributeTypeVFSDumpFreq$kODAttributeTypeVFSLinkDir$kODAttributeTypeVFSOpts$kODAttributeTypeVFSPassNo$kODAttributeTypeVFSType$kODAttributeTypeVersion$kODAttributeTypeWeblogURI$kODAttributeTypeXMLPlist$kODAuthenticationType2WayRandom$kODAuthenticationType2WayRandomChangePasswd$kODAuthenticationTypeAPOP$kODAuthenticationTypeCRAM_MD5$kODAuthenticationTypeChangePasswd$kODAuthenticationTypeClearText$kODAuthenticationTypeClearTextReadOnly$kODAuthenticationTypeCrypt$kODAuthenticationTypeDIGEST_MD5$kODAuthenticationTypeDeleteUser$kODAuthenticationTypeGetEffectivePolicy$kODAuthenticationTypeGetGlobalPolicy$kODAuthenticationTypeGetKerberosPrincipal$kODAuthenticationTypeGetPolicy$kODAuthenticationTypeGetUserData$kODAuthenticationTypeGetUserName$kODAuthenticationTypeKerberosTickets$kODAuthenticationTypeMPPEMasterKeys$kODAuthenticationTypeMPPEPrimaryKeys$kODAuthenticationTypeMSCHAP2$kODAuthenticationTypeNTLMv2$kODAuthenticationTypeNTLMv2WithSessionKey$kODAuthenticationTypeNewUser$kODAuthenticationTypeNewUserWithPolicy$kODAuthenticationTypeNodeNativeClearTextOK$kODAuthenticationTypeNodeNativeNoClearText$kODAuthenticationTypeReadSecureHash$kODAuthenticationTypeSMBNTv2UserSessionKey$kODAuthenticationTypeSMBWorkstationCredentialSessionKey$kODAuthenticationTypeSMB_LM_Key$kODAuthenticationTypeSMB_NT_Key$kODAuthenticationTypeSMB_NT_UserSessionKey$kODAuthenticationTypeSMB_NT_WithUserSessionKey$kODAuthenticationTypeSecureHash$kODAuthenticationTypeSetCertificateHashAsCurrent$kODAuthenticationTypeSetGlobalPolicy$kODAuthenticationTypeSetLMHash$kODAuthenticationTypeSetNTHash$kODAuthenticationTypeSetPassword$kODAuthenticationTypeSetPasswordAsCurrent$kODAuthenticationTypeSetPolicy$kODAuthenticationTypeSetPolicyAsCurrent$kODAuthenticationTypeSetUserData$kODAuthenticationTypeSetUserName$kODAuthenticationTypeSetWorkstationPassword$kODAuthenticationTypeWithAuthorizationRef$kODAuthenticationTypeWriteSecureHash$kODBackOffSeconds$kODErrorDomainFramework$kODModuleConfigOptionConnectionIdleDisconnect$kODModuleConfigOptionConnectionSetupTimeout$kODModuleConfigOptionManInTheMiddle$kODModuleConfigOptionPacketEncryption$kODModuleConfigOptionPacketSigning$kODModuleConfigOptionQueryTimeout$kODNodeOptionsQuerySkippedSubnode$kODPolicyAttributeCreationTime$kODPolicyAttributeCurrentDate$kODPolicyAttributeCurrentDayOfWeek$kODPolicyAttributeCurrentTime$kODPolicyAttributeCurrentTimeOfDay$kODPolicyAttributeDaysUntilExpiration$kODPolicyAttributeEnableAtTimeOfDay$kODPolicyAttributeEnableOnDate$kODPolicyAttributeEnableOnDayOfWeek$kODPolicyAttributeExpiresAtTimeOfDay$kODPolicyAttributeExpiresEveryNDays$kODPolicyAttributeExpiresOnDate$kODPolicyAttributeExpiresOnDayOfWeek$kODPolicyAttributeFailedAuthentications$kODPolicyAttributeLastAuthenticationTime$kODPolicyAttributeLastFailedAuthenticationTime$kODPolicyAttributeLastPasswordChangeTime$kODPolicyAttributeMaximumFailedAuthentications$kODPolicyAttributeNewPasswordRequiredTime$kODPolicyAttributePassword$kODPolicyAttributePasswordHashes$kODPolicyAttributePasswordHistory$kODPolicyAttributePasswordHistoryDepth$kODPolicyAttributeRecordName$kODPolicyAttributeRecordType$kODPolicyCategoryAuthentication$kODPolicyCategoryPasswordChange$kODPolicyCategoryPasswordContent$kODPolicyKeyContent$kODPolicyKeyContentDescription$kODPolicyKeyEvaluationDetails$kODPolicyKeyIdentifier$kODPolicyKeyParameters$kODPolicyKeyPolicySatisfied$kODPolicyTypeAccountExpiresOnDate$kODPolicyTypeAccountMaximumFailedLogins$kODPolicyTypeAccountMaximumMinutesOfNonUse$kODPolicyTypeAccountMaximumMinutesUntilDisabled$kODPolicyTypeAccountMinutesUntilFailedLoginReset$kODPolicyTypePasswordCannotBeAccountName$kODPolicyTypePasswordChangeRequired$kODPolicyTypePasswordHistory$kODPolicyTypePasswordMaximumAgeInMinutes$kODPolicyTypePasswordMaximumNumberOfCharacters$kODPolicyTypePasswordMinimumNumberOfCharacters$kODPolicyTypePasswordRequiresAlpha$kODPolicyTypePasswordRequiresMixedCase$kODPolicyTypePasswordRequiresNumeric$kODPolicyTypePasswordRequiresSymbol$kODPolicyTypePasswordSelfModification$kODRecordTypeAFPServer$kODRecordTypeAliases$kODRecordTypeAttributeTypes$kODRecordTypeAugments$kODRecordTypeAutoServerSetup$kODRecordTypeAutomount$kODRecordTypeAutomountMap$kODRecordTypeBootp$kODRecordTypeCertificateAuthorities$kODRecordTypeComputerGroups$kODRecordTypeComputerLists$kODRecordTypeComputers$kODRecordTypeConfiguration$kODRecordTypeEthernets$kODRecordTypeFTPServer$kODRecordTypeFileMakerServers$kODRecordTypeGroups$kODRecordTypeHostServices$kODRecordTypeHosts$kODRecordTypeLDAPServer$kODRecordTypeLocations$kODRecordTypeMounts$kODRecordTypeNFS$kODRecordTypeNetDomains$kODRecordTypeNetGroups$kODRecordTypeNetworks$kODRecordTypePeople$kODRecordTypePresetComputerGroups$kODRecordTypePresetComputerLists$kODRecordTypePresetComputers$kODRecordTypePresetGroups$kODRecordTypePresetUsers$kODRecordTypePrintService$kODRecordTypePrintServiceUser$kODRecordTypePrinters$kODRecordTypeProtocols$kODRecordTypeQTSServer$kODRecordTypeQueryInformation$kODRecordTypeRPC$kODRecordTypeRecordTypes$kODRecordTypeResources$kODRecordTypeSMBServer$kODRecordTypeServer$kODRecordTypeServices$kODRecordTypeSharePoints$kODRecordTypeUsers$kODRecordTypeWebServer$kODSessionDefault@^{__ODSession=}$kODSessionProxyAddress$kODSessionProxyPassword$kODSessionProxyPort$kODSessionProxyUsername$"""
 enums = """$kODErrorCredentialsAccountDisabled@5301$kODErrorCredentialsAccountExpired@5302$kODErrorCredentialsAccountInactive@5303$kODErrorCredentialsAccountLocked@5305$kODErrorCredentialsAccountNotFound@5300$kODErrorCredentialsAccountTemporarilyLocked@5304$kODErrorCredentialsContactMaster@5204$kODErrorCredentialsContactPrimary@5204$kODErrorCredentialsInvalid@5000$kODErrorCredentialsInvalidComputer@5501$kODErrorCredentialsInvalidLogonHours@5500$kODErrorCredentialsMethodNotSupported@5100$kODErrorCredentialsNotAuthorized@5101$kODErrorCredentialsOperationFailed@5103$kODErrorCredentialsParameterError@5102$kODErrorCredentialsPasswordChangeRequired@5401$kODErrorCredentialsPasswordChangeTooSoon@5407$kODErrorCredentialsPasswordExpired@5400$kODErrorCredentialsPasswordNeedsDigit@5406$kODErrorCredentialsPasswordNeedsLetter@5405$kODErrorCredentialsPasswordQualityFailed@5402$kODErrorCredentialsPasswordTooLong@5404$kODErrorCredentialsPasswordTooShort@5403$kODErrorCredentialsPasswordUnrecoverable@5408$kODErrorCredentialsServerCommunicationError@5205$kODErrorCredentialsServerError@5202$kODErrorCredentialsServerNotFound@5201$kODErrorCredentialsServerTimeout@5203$kODErrorCredentialsServerUnreachable@5200$kODErrorDaemonError@10002$kODErrorNodeConnectionFailed@2100$kODErrorNodeDisabled@2002$kODErrorNodeUnknownHost@2200$kODErrorNodeUnknownName@2000$kODErrorNodeUnknownType@2001$kODErrorPluginError@10001$kODErrorPluginOperationNotSupported@10000$kODErrorPluginOperationTimeout@10003$kODErrorPolicyOutOfRange@6001$kODErrorPolicyUnsupported@6000$kODErrorQueryInvalidMatchType@3100$kODErrorQuerySynchronize@3000$kODErrorQueryTimeout@3102$kODErrorQueryUnsupportedMatchType@3101$kODErrorRecordAlreadyExists@4102$kODErrorRecordAttributeNotFound@4201$kODErrorRecordAttributeUnknownType@4200$kODErrorRecordAttributeValueNotFound@4203$kODErrorRecordAttributeValueSchemaError@4202$kODErrorRecordInvalidType@4101$kODErrorRecordNoLongerExists@4104$kODErrorRecordParameterError@4100$kODErrorRecordPermissionError@4001$kODErrorRecordReadOnlyNode@4000$kODErrorRecordTypeDisabled@4103$kODErrorSessionDaemonNotRunning@1002$kODErrorSessionDaemonRefused@1003$kODErrorSessionLocalOnlyDaemonInUse@1000$kODErrorSessionNormalDaemonInUse@1001$kODErrorSessionProxyCommunicationError@1100$kODErrorSessionProxyIPUnreachable@1102$kODErrorSessionProxyUnknownHost@1103$kODErrorSessionProxyVersionMismatch@1101$kODErrorSuccess@0$kODExpirationTimeExpired@0$kODExpirationTimeNeverExpires@-1$kODMatchAny@1$kODMatchBeginsWith@8194$kODMatchContains@8196$kODMatchEndsWith@8195$kODMatchEqualTo@8193$kODMatchGreaterThan@8198$kODMatchInsensitiveBeginsWith@8450$kODMatchInsensitiveContains@8452$kODMatchInsensitiveEndsWith@8451$kODMatchInsensitiveEqualTo@8449$kODMatchLessThan@8199$kODNodeTypeAuthentication@8705$kODNodeTypeConfigure@8706$kODNodeTypeContacts@8708$kODNodeTypeLocalNodes@8704$kODNodeTypeNetwork@8709$"""
 misc.update({"ODFrameworkErrors": NewType("ODFrameworkErrors", int)})
 misc.update({})
+misc.update({})
 functions = {
     "ODNodeCopySubnodeNames": (
         b"^{__CFArray=}^{_ODNode=}^^{__CFError}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {
@@ -221,19 +222,21 @@
         },
     ),
     "ODNodeSetCredentialsExtended": (
         b"B^{_ODNode=}@@^{__CFArray=}^^{__CFArray}^^{_ODContext}^^{__CFError}",
         "",
         {
             "arguments": {
+                4: {"type_modifier": "o"},
+                5: {"type_modifier": "o"},
                 6: {
                     "already_cfretained": True,
                     "type_modifier": "o",
                     "null_accepted": True,
-                }
+                },
             }
         },
     ),
     "ODRecordPasswordChangeAllowed": (
         b"B^{__ODRecord=}^{__CFString=}^^{__CFError=}",
         "",
         {
```

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/Lib/OpenDirectory/__init__.py` & `pyobjc-framework-OpenDirectory-9.2/Lib/OpenDirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/Lib/OpenDirectory/_metadata.py` & `pyobjc-framework-OpenDirectory-9.2/Lib/OpenDirectory/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/Lib/pyobjc_framework_OpenDirectory.egg-info/PKG-INFO` & `pyobjc-framework-OpenDirectory-9.2/Lib/pyobjc_framework_OpenDirectory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-OpenDirectory
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework OpenDirectory on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,OpenDirectory,CFOpenDirectory
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/Lib/pyobjc_framework_OpenDirectory.egg-info/SOURCES.txt` & `pyobjc-framework-OpenDirectory-9.2/Lib/pyobjc_framework_OpenDirectory.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CFOpenDirectory/__init__.py
 Lib/CFOpenDirectory/_metadata.py
 Lib/OpenDirectory/__init__.py
 Lib/OpenDirectory/_metadata.py
 Lib/pyobjc_framework_OpenDirectory.egg-info/PKG-INFO
 Lib/pyobjc_framework_OpenDirectory.egg-info/SOURCES.txt
```

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PKG-INFO` & `pyobjc-framework-OpenDirectory-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-OpenDirectory
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework OpenDirectory on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,OpenDirectory,CFOpenDirectory
 Platform: MacOS X (>=10.6)
```

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfodnode.py` & `pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfodnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfodquery.py` & `pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfodquery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfodrecord.py` & `pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfodrecord.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfodsession.py` & `pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfodsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfopendirectory.py` & `pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfopendirectory.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_cfopendirectoryconstants.py` & `pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_cfopendirectoryconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_odconfiguration.py` & `pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_odconfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_odnode.py` & `pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_odnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_odquery.py` & `pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_odquery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_odrecord.py` & `pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_odrecord.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_odsession.py` & `pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_odsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/PyObjCTest/test_opendirectory.py` & `pyobjc-framework-OpenDirectory-9.2/PyObjCTest/test_opendirectory.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/CFOpenDirectory.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/CFOpenDirectory.fwinfo`

 * *Files 1% similar despite different names*

```diff
@@ -253,17 +253,19 @@
    },
    "ODNodeSetCredentialsExtended": {
     "args": {
      "0": {
       "type_override": "^{_ODNode=}"
      },
      "4": {
+      "type_modifier": "o",
       "type_override": "^^{__CFArray}"
      },
      "5": {
+      "type_modifier": "o",
       "type_override": "^^{_ODContext}"
      },
      "6": {
       "already_cfretained": true,
       "null_accepted": true,
       "type_modifier": "o",
       "type_override": "^^{__CFError}"
```

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/OpenDirectory.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/OpenDirectory.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -555,15 +555,15 @@
    "ODRecordPasswordChangeAllowed": { "ignore": true },
    "ODRecordRemoveAccountPolicy": { "ignore": true },
    "ODRecordRemovePolicy": { "ignore": true },
    "ODRecordSecondsUntilAuthenticationsExpire": { "ignore": true },
    "ODRecordSecondsUntilPasswordExpires": { "ignore": true },
    "ODRecordSetAccountPolicies": { "ignore": true },
    "ODRecordSetPolicies": { "ignore": true },
-   "ODRecordSetPolicy": { "ignore": true },": { "ignore": true },
+   "ODRecordSetPolicy": { "ignore": true },
    "ODRecordWillAuthenticationsExpire": { "ignore": true },
    "ODRecordWillPasswordExpire": { "ignore": true },
    "ODNodeSetPolicy": {"ignore": true },
    "ODNodeCopyDetails": { "ignore": true },
    "ODNodeCopyRecord": { "ignore": true },
    "ODNodeCopySubnodeNames": { "ignore": true },
    "ODNodeCopySupportedAttributes": { "ignore": true },
```

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/arm64-12.0.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/arm64-12.3.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-10.10.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-10.15.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-10.16.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-10.6.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-10.7.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-10.8.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-12.0.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.cfod/x86_64-12.3.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.cfod/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/arm64-12.0.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/arm64-12.3.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-10.10.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-10.15.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-10.16.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-10.6.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-10.7.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-10.8.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-12.0.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/metadata/raw.od/x86_64-12.3.fwinfo` & `pyobjc-framework-OpenDirectory-9.2/metadata/raw.od/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/pyobjc_setup.py` & `pyobjc-framework-OpenDirectory-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-OpenDirectory-9.1b1/setup.py` & `pyobjc-framework-OpenDirectory-9.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 macOS 10.6 and later.
 
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
     name="pyobjc-framework-OpenDirectory",
     description="Wrappers for the framework OpenDirectory on macOS",
     min_os_level="10.6",
     packages=["OpenDirectory", "CFOpenDirectory"],
     version=VERSION,
```

