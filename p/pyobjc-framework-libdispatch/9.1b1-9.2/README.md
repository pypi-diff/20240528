# Comparing `tmp/pyobjc-framework-libdispatch-9.1b1.tar.gz` & `tmp/pyobjc-framework-libdispatch-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-libdispatch-9.1b1.tar", last modified: Sun Mar 26 11:44:37 2023, max compression
+gzip compressed data, was "pyobjc-framework-libdispatch-9.2.tar", last modified: Wed Jun  7 00:32:26 2023, max compression
```

## Comparing `pyobjc-framework-libdispatch-9.1b1.tar` & `pyobjc-framework-libdispatch-9.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:37.548641 pyobjc-framework-libdispatch-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:37.491296 pyobjc-framework-libdispatch-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:37.498523 pyobjc-framework-libdispatch-9.1b1/Lib/dispatch/
--rw-r--r--   0 ronald     (501) staff       (20)      795 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/Lib/dispatch/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    30312 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/Lib/dispatch/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:37.499719 pyobjc-framework-libdispatch-9.1b1/Lib/libdispatch/
--rw-r--r--   0 ronald     (501) staff       (20)      517 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/Lib/libdispatch/__init__.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:37.502493 pyobjc-framework-libdispatch-9.1b1/Lib/pyobjc_framework_libdispatch.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2105 2023-03-26 11:44:37.000000 pyobjc-framework-libdispatch-9.1b1/Lib/pyobjc_framework_libdispatch.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1395 2023-03-26 11:44:37.000000 pyobjc-framework-libdispatch-9.1b1/Lib/pyobjc_framework_libdispatch.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:44:37.000000 pyobjc-framework-libdispatch-9.1b1/Lib/pyobjc_framework_libdispatch.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:05.000000 pyobjc-framework-libdispatch-9.1b1/Lib/pyobjc_framework_libdispatch.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       19 2023-03-26 11:44:37.000000 pyobjc-framework-libdispatch-9.1b1/Lib/pyobjc_framework_libdispatch.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       21 2023-03-26 11:44:37.000000 pyobjc-framework-libdispatch-9.1b1/Lib/pyobjc_framework_libdispatch.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-libdispatch-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-libdispatch-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:37.504473 pyobjc-framework-libdispatch-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     6289 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/Modules/_libdispatch.m
--rw-r--r--   0 ronald     (501) staff       (20)     1245 2021-03-21 10:08:23.000000 pyobjc-framework-libdispatch-9.1b1/Modules/_libdispatch_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-libdispatch-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1894 2023-03-26 11:44:37.548219 pyobjc-framework-libdispatch-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:37.526059 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2021-08-07 09:55:59.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      190 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_base.py
--rw-r--r--   0 ronald     (501) staff       (20)     2470 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_block.py
--rw-r--r--   0 ronald     (501) staff       (20)     4380 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_data.py
--rw-r--r--   0 ronald     (501) staff       (20)      187 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_dispatch.py
--rw-r--r--   0 ronald     (501) staff       (20)     2715 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_group.py
--rw-r--r--   0 ronald     (501) staff       (20)      888 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_introspection.py
--rw-r--r--   0 ronald     (501) staff       (20)     5829 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_io.py
--rw-r--r--   0 ronald     (501) staff       (20)      200 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_libdispatch.py
--rw-r--r--   0 ronald     (501) staff       (20)     3378 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_object.py
--rw-r--r--   0 ronald     (501) staff       (20)     1275 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_once.py
--rw-r--r--   0 ronald     (501) staff       (20)    12731 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_queueu.py
--rw-r--r--   0 ronald     (501) staff       (20)      822 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_semaphore.py
--rw-r--r--   0 ronald     (501) staff       (20)     6950 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_source.py
--rw-r--r--   0 ronald     (501) staff       (20)     1549 2023-03-03 17:21:59.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_time.py
--rw-r--r--   0 ronald     (501) staff       (20)     1235 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_workgroup_interval.py
--rw-r--r--   0 ronald     (501) staff       (20)     3466 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_workgroup_object.py
--rw-r--r--   0 ronald     (501) staff       (20)      635 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_workgroup_parallel.py
--rw-r--r--   0 ronald     (501) staff       (20)     1701 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_workloop.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:37.528479 pyobjc-framework-libdispatch-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    37857 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/metadata/libdispatch.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       70 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:37.546613 pyobjc-framework-libdispatch-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)      631 2021-07-30 09:00:38.000000 pyobjc-framework-libdispatch-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      650 2022-02-24 08:47:17.000000 pyobjc-framework-libdispatch-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    38858 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/metadata/raw/arm64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      612 2020-11-30 18:45:15.000000 pyobjc-framework-libdispatch-9.1b1/metadata/raw/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      632 2021-03-21 10:08:23.000000 pyobjc-framework-libdispatch-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      632 2021-07-30 09:00:38.000000 pyobjc-framework-libdispatch-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      651 2022-02-24 08:47:17.000000 pyobjc-framework-libdispatch-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    38882 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.1b1/metadata/raw/x86_64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-libdispatch-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:44:37.548734 pyobjc-framework-libdispatch-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      945 2023-03-25 14:20:32.000000 pyobjc-framework-libdispatch-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:26.660136 pyobjc-framework-libdispatch-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:26.607312 pyobjc-framework-libdispatch-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:26.612344 pyobjc-framework-libdispatch-9.2/Lib/dispatch/
+-rw-r--r--   0 ronald     (501) staff       (20)      795 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/Lib/dispatch/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    30312 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/Lib/dispatch/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:26.613290 pyobjc-framework-libdispatch-9.2/Lib/libdispatch/
+-rw-r--r--   0 ronald     (501) staff       (20)      517 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/Lib/libdispatch/__init__.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:26.626857 pyobjc-framework-libdispatch-9.2/Lib/pyobjc_framework_libdispatch.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2103 2023-06-07 00:32:26.000000 pyobjc-framework-libdispatch-9.2/Lib/pyobjc_framework_libdispatch.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1410 2023-06-07 00:32:26.000000 pyobjc-framework-libdispatch-9.2/Lib/pyobjc_framework_libdispatch.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:32:26.000000 pyobjc-framework-libdispatch-9.2/Lib/pyobjc_framework_libdispatch.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:05.000000 pyobjc-framework-libdispatch-9.2/Lib/pyobjc_framework_libdispatch.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-06-07 00:32:26.000000 pyobjc-framework-libdispatch-9.2/Lib/pyobjc_framework_libdispatch.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       21 2023-06-07 00:32:26.000000 pyobjc-framework-libdispatch-9.2/Lib/pyobjc_framework_libdispatch.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-libdispatch-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-libdispatch-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:26.630226 pyobjc-framework-libdispatch-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     6289 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/Modules/_libdispatch.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1245 2021-03-21 10:08:23.000000 pyobjc-framework-libdispatch-9.2/Modules/_libdispatch_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-libdispatch-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1892 2023-06-07 00:32:26.659622 pyobjc-framework-libdispatch-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:26.651913 pyobjc-framework-libdispatch-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2021-08-07 09:55:59.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      190 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_base.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2470 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_block.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4380 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_data.py
+-rw-r--r--   0 ronald     (501) staff       (20)      187 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_dispatch.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2715 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_group.py
+-rw-r--r--   0 ronald     (501) staff       (20)      888 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_introspection.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5829 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_io.py
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_libdispatch.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3378 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_object.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1275 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_once.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12731 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_queueu.py
+-rw-r--r--   0 ronald     (501) staff       (20)      822 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_semaphore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6950 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_source.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1549 2023-03-03 17:21:59.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_time.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1235 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_workgroup_interval.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3466 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_workgroup_object.py
+-rw-r--r--   0 ronald     (501) staff       (20)      635 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_workgroup_parallel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1701 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/PyObjCTest/test_workloop.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:26.653424 pyobjc-framework-libdispatch-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    37857 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/metadata/libdispatch.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       70 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:26.658725 pyobjc-framework-libdispatch-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)      631 2021-07-30 09:00:38.000000 pyobjc-framework-libdispatch-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      650 2022-02-24 08:47:17.000000 pyobjc-framework-libdispatch-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    38858 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/metadata/raw/arm64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      612 2020-11-30 18:45:15.000000 pyobjc-framework-libdispatch-9.2/metadata/raw/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      632 2021-03-21 10:08:23.000000 pyobjc-framework-libdispatch-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      632 2021-07-30 09:00:38.000000 pyobjc-framework-libdispatch-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      651 2022-02-24 08:47:17.000000 pyobjc-framework-libdispatch-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    38882 2023-02-19 10:50:37.000000 pyobjc-framework-libdispatch-9.2/metadata/raw/x86_64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-libdispatch-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-libdispatch-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:32:26.660256 pyobjc-framework-libdispatch-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1027 2023-05-29 10:07:47.000000 pyobjc-framework-libdispatch-9.2/setup.py
```

### Comparing `pyobjc-framework-libdispatch-9.1b1/Lib/dispatch/__init__.py` & `pyobjc-framework-libdispatch-9.2/Lib/dispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/Lib/dispatch/_metadata.py` & `pyobjc-framework-libdispatch-9.2/Lib/dispatch/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/Lib/libdispatch/__init__.py` & `pyobjc-framework-libdispatch-9.2/Lib/libdispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/Lib/pyobjc_framework_libdispatch.egg-info/PKG-INFO` & `pyobjc-framework-libdispatch-9.2/Lib/pyobjc_framework_libdispatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-libdispatch
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for libdispatch on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,dispatch,libdispatch
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-libdispatch-9.1b1/Lib/pyobjc_framework_libdispatch.egg-info/SOURCES.txt` & `pyobjc-framework-libdispatch-9.2/Lib/pyobjc_framework_libdispatch.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/dispatch/__init__.py
 Lib/dispatch/_metadata.py
 Lib/libdispatch/__init__.py
 Lib/pyobjc_framework_libdispatch.egg-info/PKG-INFO
 Lib/pyobjc_framework_libdispatch.egg-info/SOURCES.txt
 Lib/pyobjc_framework_libdispatch.egg-info/dependency_links.txt
```

### Comparing `pyobjc-framework-libdispatch-9.1b1/License.txt` & `pyobjc-framework-libdispatch-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/Modules/_libdispatch.m` & `pyobjc-framework-libdispatch-9.2/Modules/_libdispatch.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/Modules/_libdispatch_inlines.m` & `pyobjc-framework-libdispatch-9.2/Modules/_libdispatch_inlines.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-libdispatch-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-libdispatch-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-libdispatch-9.1b1/PKG-INFO` & `pyobjc-framework-libdispatch-9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-libdispatch
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for libdispatch on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,dispatch,libdispatch
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_block.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_block.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_data.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_data.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_group.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_group.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_introspection.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_introspection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_io.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_io.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_object.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_object.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_once.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_once.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_queueu.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_queueu.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_semaphore.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_semaphore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_source.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_source.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_time.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_time.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_workgroup_interval.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_workgroup_interval.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_workgroup_object.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_workgroup_object.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_workgroup_parallel.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_workgroup_parallel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/PyObjCTest/test_workloop.py` & `pyobjc-framework-libdispatch-9.2/PyObjCTest/test_workloop.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/metadata/libdispatch.fwinfo` & `pyobjc-framework-libdispatch-9.2/metadata/libdispatch.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-libdispatch-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-libdispatch-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/metadata/raw/arm64-13.1.fwinfo` & `pyobjc-framework-libdispatch-9.2/metadata/raw/arm64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/metadata/raw/x86_64-10.13.fwinfo` & `pyobjc-framework-libdispatch-9.2/metadata/raw/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-libdispatch-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-libdispatch-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-libdispatch-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/metadata/raw/x86_64-13.1.fwinfo` & `pyobjc-framework-libdispatch-9.2/metadata/raw/x86_64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/pyobjc_setup.py` & `pyobjc-framework-libdispatch-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libdispatch-9.1b1/setup.py` & `pyobjc-framework-libdispatch-9.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 
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
     name="pyobjc-framework-libdispatch",
     description="Wrappers for libdispatch on macOS",
     min_os_level="10.8",
     packages=["dispatch", "libdispatch"],
     ext_modules=[
```

