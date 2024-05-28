# Comparing `tmp/pyobjc-framework-CoreText-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreText-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreText-9.1b1.tar", last modified: Sun Mar 26 11:22:21 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreText-9.2.tar", last modified: Wed Jun  7 00:12:22 2023, max compression
```

## Comparing `pyobjc-framework-CoreText-9.1b1.tar` & `pyobjc-framework-CoreText-9.2.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:21.421022 pyobjc-framework-CoreText-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreText-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:21.328901 pyobjc-framework-CoreText-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:21.334501 pyobjc-framework-CoreText-9.1b1/Lib/CoreText/
--rw-r--r--   0 ronald     (501) staff       (20)      884 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.1b1/Lib/CoreText/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    78237 2023-03-04 10:55:09.000000 pyobjc-framework-CoreText-9.1b1/Lib/CoreText/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:21.338803 pyobjc-framework-CoreText-9.1b1/Lib/pyobjc_framework_CoreText.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2283 2023-03-26 11:22:21.000000 pyobjc-framework-CoreText-9.1b1/Lib/pyobjc_framework_CoreText.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1519 2023-03-26 11:22:21.000000 pyobjc-framework-CoreText-9.1b1/Lib/pyobjc_framework_CoreText.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:22:21.000000 pyobjc-framework-CoreText-9.1b1/Lib/pyobjc_framework_CoreText.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:09.000000 pyobjc-framework-CoreText-9.1b1/Lib/pyobjc_framework_CoreText.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:22:21.000000 pyobjc-framework-CoreText-9.1b1/Lib/pyobjc_framework_CoreText.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:22:21.000000 pyobjc-framework-CoreText-9.1b1/Lib/pyobjc_framework_CoreText.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:21.359379 pyobjc-framework-CoreText-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)    14503 2021-10-18 19:38:40.000000 pyobjc-framework-CoreText-9.1b1/Modules/_manual.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreText-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreText-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2072 2023-03-26 11:22:21.420481 pyobjc-framework-CoreText-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:21.379189 pyobjc-framework-CoreText-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1404 2022-04-11 08:03:15.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_coretext.py
--rw-r--r--   0 ronald     (501) staff       (20)    23710 2023-03-03 17:21:59.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctfont.py
--rw-r--r--   0 ronald     (501) staff       (20)     3056 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctfontcollection.py
--rw-r--r--   0 ronald     (501) staff       (20)     8962 2023-03-03 17:21:59.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctfontdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)     4182 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctfontmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     1638 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctfontmanagererrors.py
--rw-r--r--   0 ronald     (501) staff       (20)     5207 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctfonttraits.py
--rw-r--r--   0 ronald     (501) staff       (20)     3288 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctframe.py
--rw-r--r--   0 ronald     (501) staff       (20)     1736 2022-01-02 11:04:26.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctframesetter.py
--rw-r--r--   0 ronald     (501) staff       (20)     2931 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctglyphinfo.py
--rw-r--r--   0 ronald     (501) staff       (20)     4758 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctline.py
--rw-r--r--   0 ronald     (501) staff       (20)     8152 2022-01-02 11:04:26.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctparagraphstyle.py
--rw-r--r--   0 ronald     (501) staff       (20)     2382 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctrubyannotation.py
--rw-r--r--   0 ronald     (501) staff       (20)     4660 2021-07-31 13:52:16.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctrun.py
--rw-r--r--   0 ronald     (501) staff       (20)     1422 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctrundelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)     3181 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctstringattributes.py
--rw-r--r--   0 ronald     (501) staff       (20)     1021 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_cttexttab.py
--rw-r--r--   0 ronald     (501) staff       (20)     2081 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_cttypesetter.py
--rw-r--r--   0 ronald     (501) staff       (20)      285 2021-10-18 19:38:40.000000 pyobjc-framework-CoreText-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:21.385187 pyobjc-framework-CoreText-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    43227 2023-03-04 10:54:54.000000 pyobjc-framework-CoreText-9.1b1/metadata/CoreText.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      126 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:22:21.418086 pyobjc-framework-CoreText-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   138466 2021-07-30 09:00:37.000000 pyobjc-framework-CoreText-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   139831 2022-02-24 08:47:16.000000 pyobjc-framework-CoreText-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   150611 2022-10-18 09:53:23.000000 pyobjc-framework-CoreText-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   129432 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   137976 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   138514 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    56336 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    63052 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    67815 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   138467 2021-07-30 09:00:37.000000 pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   139832 2022-02-24 08:47:16.000000 pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   150612 2022-10-18 09:53:23.000000 pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreText-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:22:21.421144 pyobjc-framework-CoreText-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1075 2023-03-25 14:20:31.000000 pyobjc-framework-CoreText-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:22.700671 pyobjc-framework-CoreText-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreText-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:22.581448 pyobjc-framework-CoreText-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:22.617472 pyobjc-framework-CoreText-9.2/Lib/CoreText/
+-rw-r--r--   0 ronald     (501) staff       (20)      884 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.2/Lib/CoreText/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    78470 2023-05-27 09:46:33.000000 pyobjc-framework-CoreText-9.2/Lib/CoreText/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:22.621034 pyobjc-framework-CoreText-9.2/Lib/pyobjc_framework_CoreText.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2281 2023-06-07 00:12:22.000000 pyobjc-framework-CoreText-9.2/Lib/pyobjc_framework_CoreText.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1534 2023-06-07 00:12:22.000000 pyobjc-framework-CoreText-9.2/Lib/pyobjc_framework_CoreText.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:12:22.000000 pyobjc-framework-CoreText-9.2/Lib/pyobjc_framework_CoreText.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:09.000000 pyobjc-framework-CoreText-9.2/Lib/pyobjc_framework_CoreText.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:12:22.000000 pyobjc-framework-CoreText-9.2/Lib/pyobjc_framework_CoreText.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:12:22.000000 pyobjc-framework-CoreText-9.2/Lib/pyobjc_framework_CoreText.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:22.623025 pyobjc-framework-CoreText-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)    14503 2021-10-18 19:38:40.000000 pyobjc-framework-CoreText-9.2/Modules/_manual.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreText-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CoreText-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2070 2023-06-07 00:12:22.699588 pyobjc-framework-CoreText-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:22.664066 pyobjc-framework-CoreText-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1404 2022-04-11 08:03:15.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_coretext.py
+-rw-r--r--   0 ronald     (501) staff       (20)    23923 2023-05-27 09:46:33.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctfont.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3056 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctfontcollection.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8962 2023-03-03 17:21:59.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctfontdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4182 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctfontmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1638 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctfontmanagererrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5207 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctfonttraits.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3288 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctframe.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1736 2022-01-02 11:04:26.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctframesetter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2931 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctglyphinfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4758 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctline.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8152 2022-01-02 11:04:26.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctparagraphstyle.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2382 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctrubyannotation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4660 2021-07-31 13:52:16.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctrun.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1422 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctrundelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3181 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctstringattributes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1021 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_cttexttab.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2081 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/PyObjCTest/test_cttypesetter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      285 2021-10-18 19:38:40.000000 pyobjc-framework-CoreText-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:22.666032 pyobjc-framework-CoreText-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    38871 2023-05-27 09:46:33.000000 pyobjc-framework-CoreText-9.2/metadata/CoreText.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      126 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:12:22.692027 pyobjc-framework-CoreText-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   138466 2021-07-30 09:00:37.000000 pyobjc-framework-CoreText-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   139831 2022-02-24 08:47:16.000000 pyobjc-framework-CoreText-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   150611 2022-10-18 09:53:23.000000 pyobjc-framework-CoreText-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   129432 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   137976 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   138514 2021-03-21 10:08:22.000000 pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    56336 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    63052 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    67815 2020-11-30 18:45:14.000000 pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   138467 2021-07-30 09:00:37.000000 pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   139832 2022-02-24 08:47:16.000000 pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   150612 2022-10-18 09:53:23.000000 pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreText-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreText-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:12:22.700772 pyobjc-framework-CoreText-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1157 2023-05-29 10:07:46.000000 pyobjc-framework-CoreText-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreText-9.1b1/LICENSE.txt` & `pyobjc-framework-CoreText-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/Lib/CoreText/__init__.py` & `pyobjc-framework-CoreText-9.2/Lib/CoreText/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/Lib/CoreText/_metadata.py` & `pyobjc-framework-CoreText-9.2/Lib/CoreText/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Aug 12 16:58:36 2022
+# Last update: Sat May 20 10:15:41 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -239,15 +239,18 @@
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CTTypesetterSuggestClusterBreak": (b"q^{__CTTypesetter=}qd",),
     "CTFontCreateCopyWithFamily": (
         b"^{__CTFont=}^{__CTFont=}d^{CGAffineTransform=dddddd}^{__CFString=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {2: {"type_modifier": "n"}},
+        },
     ),
     "CTFontGetGlyphsForCharacters": (
         b"B^{__CTFont=}^T^Sq",
         "",
         {
             "arguments": {
                 1: {"c_array_length_in_arg": 3, "type_modifier": "n"},
@@ -575,15 +578,18 @@
         },
     ),
     "CTFontGetMatrix": (b"{CGAffineTransform=dddddd}^{__CTFont=}",),
     "CTFontGetSymbolicTraits": (b"I^{__CTFont=}",),
     "CTFontCreateCopyWithAttributes": (
         b"^{__CTFont=}^{__CTFont=}d^{CGAffineTransform=dddddd}^{__CTFontDescriptor=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {2: {"type_modifier": "n"}},
+        },
     ),
     "CTRubyAnnotationGetSizeFactor": (b"d^{__CTRubyAnnotation=}",),
     "CTFontCollectionCopyFontAttribute": (
         b"^{__CFArray=}^{__CTFontCollection=}^{__CFString=}I",
         "",
         {"retval": {"already_cfretained": True}},
     ),
@@ -844,15 +850,15 @@
         b"d^{__CTLine=}q^d",
         "",
         {"arguments": {2: {"type_modifier": "o"}}},
     ),
     "CTFontManagerEnableFontDescriptors": (b"v^{__CFArray=}B",),
     "CTRubyAnnotationGetAlignment": (b"C^{__CTRubyAnnotation=}",),
     "CTFontCopyLocalizedName": (
-        b"^{__CFString=}^{__CTFont=}^{__CFString=}^^{__CFString}",
+        b"^{__CFString=}^{__CTFont=}^{__CFString=}^^{__CFString=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {2: {"type_modifier": "o"}},
         },
     ),
     "CTFontDescriptorCreateCopyWithFamily": (
@@ -981,15 +987,15 @@
     "CTFontDescriptorCreateCopyWithSymbolicTraits": (
         b"^{__CTFontDescriptor=}^{__CTFontDescriptor=}II",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CTLineGetBoundsWithOptions": (b"{CGRect={CGPoint=dd}{CGSize=dd}}^{__CTLine=}Q",),
     "CTFontCopyGraphicsFont": (
-        b"^{CGFont=}^{__CTFont=}^^{__CTFontDescriptor}",
+        b"^{CGFont=}^{__CTFont=}^^{__CTFontDescriptor=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {1: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
     "CTFontCollectionCreateMatchingFontDescriptorsForFamily": (
@@ -1024,15 +1030,18 @@
         b"B^{__CFArray=}I^^{__CFArray=}",
         "",
         {"arguments": {2: {"type_modifier": "o"}}},
     ),
     "CTFontCreateCopyWithSymbolicTraits": (
         b"^{__CTFont=}^{__CTFont=}d^{CGAffineTransform=dddddd}II",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {2: {"type_modifier": "n"}},
+        },
     ),
     "CTFontCopyTraits": (
         b"^{__CFDictionary=}^{__CTFont=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CTRunDraw": (b"v^{__CTRun=}^{CGContext=}{_CFRange=qq}",),
```

### Comparing `pyobjc-framework-CoreText-9.1b1/Lib/pyobjc_framework_CoreText.egg-info/PKG-INFO` & `pyobjc-framework-CoreText-9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreText
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreText on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreText
 Platform: MacOS X (>=10.5)
@@ -26,17 +26,14 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Objective C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
-Project-URL: Documentation, https://pyobjc.readthedocs.io/en/latest/
-Project-URL: Issue tracker, https://github.com/ronaldoussoren/pyobjc/issues
-Project-URL: Repository, https://github.com/ronaldoussoren/pyobjc
 
 
 Wrappers for the "CoreText" framework on macOS 10.5 or later. Core Text is an
 advanced, low-level technology for laying out text and handling fonts. It is
 designed for high performance and ease of use.
 
 These wrappers don't include documentation, please check Apple's documentation
```

### Comparing `pyobjc-framework-CoreText-9.1b1/Lib/pyobjc_framework_CoreText.egg-info/SOURCES.txt` & `pyobjc-framework-CoreText-9.2/Lib/pyobjc_framework_CoreText.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CoreText/__init__.py
 Lib/CoreText/_metadata.py
 Lib/pyobjc_framework_CoreText.egg-info/PKG-INFO
 Lib/pyobjc_framework_CoreText.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CoreText.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CoreText.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CoreText-9.1b1/Modules/_manual.m` & `pyobjc-framework-CoreText-9.2/Modules/_manual.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreText-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreText-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CoreText-9.1b1/PKG-INFO` & `pyobjc-framework-CoreText-9.2/Lib/pyobjc_framework_CoreText.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreText
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreText on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreText
 Platform: MacOS X (>=10.5)
@@ -26,14 +26,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Objective C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
+Project-URL: Documentation, https://pyobjc.readthedocs.io/en/latest/
+Project-URL: Issue tracker, https://github.com/ronaldoussoren/pyobjc/issues
+Project-URL: Repository, https://github.com/ronaldoussoren/pyobjc
 
 
 Wrappers for the "CoreText" framework on macOS 10.5 or later. Core Text is an
 advanced, low-level technology for laying out text and handling fonts. It is
 designed for high performance and ease of use.
 
 These wrappers don't include documentation, please check Apple's documentation
```

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_coretext.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_coretext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctfont.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctfont.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,24 +216,27 @@
         self.assertIsInstance(font, CoreText.CTFontRef)
         self.assertResultIsCFRetained(CoreText.CTFontCreateUIFontForLanguage)
 
         font2 = CoreText.CTFontCreateCopyWithAttributes(font, 9.0, None, None)
 
         self.assertIsInstance(font2, CoreText.CTFontRef)
         self.assertResultIsCFRetained(CoreText.CTFontCreateCopyWithAttributes)
+        self.assertArgIsIn(CoreText.CTFontCreateCopyWithAttributes, 2)
 
         font2 = CoreText.CTFontCreateCopyWithSymbolicTraits(
             font, 14.0, None, CoreText.kCTFontBoldTrait, CoreText.kCTFontBoldTrait
         )
         self.assertIsInstance(font2, CoreText.CTFontRef)
         self.assertResultIsCFRetained(CoreText.CTFontCreateCopyWithAttributes)
+        self.assertArgIsIn(CoreText.CTFontCreateCopyWithSymbolicTraits, 2)
 
         font2 = CoreText.CTFontCreateCopyWithFamily(font, 14.0, None, "Lucida Grande")
         self.assertIsInstance(font2, CoreText.CTFontRef)
         self.assertResultIsCFRetained(CoreText.CTFontCreateCopyWithFamily)
+        self.assertArgIsIn(CoreText.CTFontCreateCopyWithFamily, 2)
 
         font2 = CoreText.CTFontCreateForString(
             font, "hello world", CoreText.CFRange(1, 4)
         )
         self.assertIsInstance(font2, CoreText.CTFontRef)
         self.assertResultIsCFRetained(CoreText.CTFontCreateForString)
```

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctfontcollection.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctfontcollection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctfontdescriptor.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctfontdescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctfontmanager.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctfontmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctfontmanagererrors.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctfontmanagererrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctfonttraits.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctfonttraits.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctframe.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctframe.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctframesetter.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctframesetter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctglyphinfo.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctglyphinfo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctline.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctline.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctparagraphstyle.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctparagraphstyle.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctrubyannotation.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctrubyannotation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctrun.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctrun.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctrundelegate.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctrundelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_ctstringattributes.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_ctstringattributes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_cttexttab.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_cttexttab.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/PyObjCTest/test_cttypesetter.py` & `pyobjc-framework-CoreText-9.2/PyObjCTest/test_cttypesetter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/CoreText.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/CoreText.fwinfo`

 * *Files 12% similar despite different names*

```diff
@@ -302,67 +302,35 @@
      "0": {}
     },
     "retval": {
      "already_cfretained": true
     }
    },
    "CTFontCollectionCreateCopyWithFontDescriptors": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFontCollection=}"
-     },
-     "1": {
-      "type_override": "^{__CFArray=}"
-     },
-     "2": {
-      "type_override": "^{__CFDictionary=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CTFontCollection=}"
+     "already_cfretained": true
     }
    },
    "CTFontCollectionCreateFromAvailableFonts": {
-    "args": {
-     "0": {
-      "type_override": "^{__CFDictionary=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CTFontCollection=}"
+     "already_cfretained": true
     }
    },
    "CTFontCollectionCreateMatchingFontDescriptors": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFontCollection=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFArray=}"
+     "already_cfretained": true
     }
    },
    "CTFontCollectionCreateMatchingFontDescriptorsForFamily": {
-    "args": {
-     "0": {},
-     "1": {},
-     "2": {}
-    },
     "retval": {
      "already_cfretained": true
     }
    },
    "CTFontCollectionCreateMatchingFontDescriptorsSortedWithCallback": {
     "args": {
-     "0": {
-      "type_override": "^{__CTFontCollection=}"
-     },
      "1": {
       "function": {
        "args": {
         "0": {
          "typestr": "^{__CTFontDescriptor=}"
         },
         "1": {
@@ -379,360 +347,183 @@
       "callable_retained": false
      },
      "2": {
       "type_override": "@"
      }
     },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFArray=}"
+     "already_cfretained": true
     }
    },
    "CTFontCollectionCreateMatchingFontDescriptorsWithOptions": {
-    "args": {
-     "0": {},
-     "1": {}
-    },
     "retval": {
      "already_cfretained": true
     }
    },
    "CTFontCollectionCreateMutableCopy": {
-    "args": {
-     "0": {}
-    },
     "retval": {
      "already_cfretained": true
     }
    },
    "CTFontCollectionCreateWithFontDescriptors": {
-    "args": {
-     "0": {
-      "type_override": "^{__CFArray=}"
-     },
-     "1": {
-      "type_override": "^{__CFDictionary=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CTFontCollection=}"
+     "already_cfretained": true
     }
    },
    "CTFontCollectionSetExclusionDescriptors": {
     "args": {
      "0": {},
      "1": {}
     }
    },
    "CTFontCollectionSetQueryDescriptors": {
     "args": {
      "0": {},
      "1": {}
     }
    },
-   "CTFontCopyAttribute": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     },
-     "1": {
-      "type_override": "^{__CFString=}"
-     }
-    }
-   },
    "CTFontCopyAvailableTables": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFArray=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyCharacterSet": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFCharacterSet=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyDisplayName": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFString=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyFamilyName": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFString=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyFeatureSettings": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFArray=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyFeatures": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFArray=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyFontDescriptor": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CTFontDescriptor=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyFullName": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFString=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyGraphicsFont": {
     "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     },
      "1": {
       "already_cfretained": true,
-      "type_modifier": "o",
-      "type_override": "^^{__CTFontDescriptor}"
+      "type_modifier": "o"
      }
     },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{CGFont=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyLocalizedName": {
     "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     },
-     "1": {
-      "type_override": "^{__CFString=}"
-     },
      "2": {
-      "type_modifier": "o",
-      "type_override": "^^{__CFString}"
+      "type_modifier": "o"
      }
     },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFString=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyName": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     },
-     "1": {
-      "type_override": "^{__CFString=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFString=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyPostScriptName": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFString=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopySupportedLanguages": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFArray=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyTable": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFData=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyTraits": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFDictionary=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyVariation": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFDictionary=}"
+     "already_cfretained": true
     }
    },
    "CTFontCopyVariationAxes": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CFArray=}"
+     "already_cfretained": true
     }
    },
    "CTFontCreateCopyWithAttributes": {
     "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     },
      "2": {
-      "type_override": [
-       "^{CGAffineTransform=ffffff}",
-       "^{CGAffineTransform=dddddd}"
-      ]
-     },
-     "3": {
-      "type_override": "^{__CTFontDescriptor=}"
+      "type_modifier": "n"
      }
     },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CTFont=}"
+     "already_cfretained": true
     }
    },
    "CTFontCreateCopyWithFamily": {
     "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     },
      "2": {
-      "type_override": [
-       "^{CGAffineTransform=ffffff}",
-       "^{CGAffineTransform=dddddd}"
-      ]
-     },
-     "3": {
-      "type_override": "^{__CFString=}"
+      "type_modifier": "n"
      }
     },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CTFont=}"
+     "already_cfretained": true
     }
    },
    "CTFontCreateCopyWithSymbolicTraits": {
     "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     },
      "2": {
-      "type_override": [
-       "^{CGAffineTransform=ffffff}",
-       "^{CGAffineTransform=dddddd}"
-      ]
+      "type_modifier": "n"
      }
     },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CTFont=}"
+     "already_cfretained": true
     }
    },
    "CTFontCreateForString": {
-    "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     },
-     "1": {
-      "type_override": "^{__CFString=}"
-     }
-    },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{__CTFont=}"
+     "already_cfretained": true
     }
    },
    "CTFontCreatePathForGlyph": {
     "args": {
-     "0": {
-      "type_override": "^{__CTFont=}"
-     },
      "2": {
-      "type_modifier": "n",
-      "type_override": [
-       "^{CGAffineTransform=ffffff}",
-       "^{CGAffineTransform=dddddd}"
-      ]
+      "type_modifier": "n"
      }
     },
     "retval": {
-     "already_cfretained": true,
-     "type_override": "^{CGPath=}"
+     "already_cfretained": true
     }
    },
    "CTFontCreateUIFontForLanguage": {
     "args": {
      "2": {
       "type_override": "^{__CFString=}"
      }
```

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-CoreText-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreText-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreText-9.1b1/setup.py` & `pyobjc-framework-CoreText-9.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,23 @@
 designed for high performance and ease of use.
 
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
     name="pyobjc-framework-CoreText",
     description="Wrappers for the framework CoreText on macOS",
     min_os_level="10.5",
     packages=["CoreText"],
     ext_modules=[
```

