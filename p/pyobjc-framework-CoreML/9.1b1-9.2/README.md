# Comparing `tmp/pyobjc-framework-CoreML-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreML-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreML-9.1b1.tar", last modified: Sun Mar 26 11:21:03 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreML-9.2.tar", last modified: Wed Jun  7 00:11:02 2023, max compression
```

## Comparing `pyobjc-framework-CoreML-9.1b1.tar` & `pyobjc-framework-CoreML-9.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:03.876483 pyobjc-framework-CoreML-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:03.749969 pyobjc-framework-CoreML-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:03.755252 pyobjc-framework-CoreML-9.1b1/Lib/CoreML/
--rw-r--r--   0 ronald     (501) staff       (20)      709 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.1b1/Lib/CoreML/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    18671 2023-02-19 10:50:35.000000 pyobjc-framework-CoreML-9.1b1/Lib/CoreML/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:03.778822 pyobjc-framework-CoreML-9.1b1/Lib/pyobjc_framework_CoreML.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2096 2023-03-26 11:21:03.000000 pyobjc-framework-CoreML-9.1b1/Lib/pyobjc_framework_CoreML.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1872 2023-03-26 11:21:03.000000 pyobjc-framework-CoreML-9.1b1/Lib/pyobjc_framework_CoreML.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:21:03.000000 pyobjc-framework-CoreML-9.1b1/Lib/pyobjc_framework_CoreML.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:49.000000 pyobjc-framework-CoreML-9.1b1/Lib/pyobjc_framework_CoreML.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:21:03.000000 pyobjc-framework-CoreML-9.1b1/Lib/pyobjc_framework_CoreML.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        7 2023-03-26 11:21:03.000000 pyobjc-framework-CoreML-9.1b1/Lib/pyobjc_framework_CoreML.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreML-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:03.785957 pyobjc-framework-CoreML-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      799 2021-10-18 19:38:40.000000 pyobjc-framework-CoreML-9.1b1/Modules/_CoreML.m
--rw-r--r--   0 ronald     (501) staff       (20)      659 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.1b1/Modules/_CoreML_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreML-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreML-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1885 2023-03-26 11:21:03.876160 pyobjc-framework-CoreML-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:03.836558 pyobjc-framework-CoreML-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      196 2022-04-11 08:03:15.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_coreml.py
--rw-r--r--   0 ronald     (501) staff       (20)      667 2022-06-25 09:09:12.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlbatchprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)     1608 2022-06-25 20:16:10.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlcustomlayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      963 2022-06-25 20:18:13.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlcustommodel.py
--rw-r--r--   0 ronald     (501) staff       (20)      298 2021-03-21 10:08:22.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mldictionaryfeatureprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      401 2021-03-21 10:08:22.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlfeaturedescription.py
--rw-r--r--   0 ronald     (501) staff       (20)      251 2022-06-25 20:10:17.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlfeatureprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      608 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlfeaturetype.py
--rw-r--r--   0 ronald     (501) staff       (20)      403 2021-03-21 10:08:22.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlfeaturevalue.py
--rw-r--r--   0 ronald     (501) staff       (20)     1779 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlfeaturevalue_mlimageconversion.py
--rw-r--r--   0 ronald     (501) staff       (20)      446 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlimagesizeconstrainttype.py
--rw-r--r--   0 ronald     (501) staff       (20)     1309 2022-06-23 11:03:28.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmodel.py
--rw-r--r--   0 ronald     (501) staff       (20)      428 2022-06-23 11:03:28.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmodel_mlmodelcompilation.py
--rw-r--r--   0 ronald     (501) staff       (20)      281 2022-06-23 11:03:28.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmodelasset.py
--rw-r--r--   0 ronald     (501) staff       (20)      668 2021-07-30 09:00:37.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmodelcollection.py
--rw-r--r--   0 ronald     (501) staff       (20)      887 2023-02-19 10:50:35.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmodelconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      955 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmodelerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      589 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmodelmetadatakeys.py
--rw-r--r--   0 ronald     (501) staff       (20)     1764 2022-06-26 20:17:38.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmultiarray.py
--rw-r--r--   0 ronald     (501) staff       (20)      476 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmultiarrayshapeconstrainttype.py
--rw-r--r--   0 ronald     (501) staff       (20)      323 2021-03-21 10:08:22.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlpredictionoptions.py
--rw-r--r--   0 ronald     (501) staff       (20)      482 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mltask.py
--rw-r--r--   0 ronald     (501) staff       (20)      448 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlupdateprogressevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      519 2021-03-21 10:08:22.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlupdateprogresshandlers.py
--rw-r--r--   0 ronald     (501) staff       (20)     1206 2021-07-30 09:00:37.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlupdatetask.py
--rw-r--r--   0 ronald     (501) staff       (20)      493 2022-06-25 20:08:48.000000 pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlwritable.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:03.838310 pyobjc-framework-CoreML-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    12976 2023-02-19 10:50:35.000000 pyobjc-framework-CoreML-9.1b1/metadata/CoreML.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:03.874854 pyobjc-framework-CoreML-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    84874 2022-01-02 11:04:26.000000 pyobjc-framework-CoreML-9.1b1/metadata/raw/arm64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    85290 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    90189 2022-06-23 11:03:28.000000 pyobjc-framework-CoreML-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    90083 2023-02-19 10:50:35.000000 pyobjc-framework-CoreML-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    41850 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    73239 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    83339 2021-03-21 10:08:22.000000 pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    84875 2022-01-02 11:04:26.000000 pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    85291 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    90190 2022-06-23 11:03:28.000000 pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    90084 2023-02-19 10:50:35.000000 pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreML-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:21:03.876584 pyobjc-framework-CoreML-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1111 2023-03-25 14:20:31.000000 pyobjc-framework-CoreML-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:02.084341 pyobjc-framework-CoreML-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:01.988968 pyobjc-framework-CoreML-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:01.995726 pyobjc-framework-CoreML-9.2/Lib/CoreML/
+-rw-r--r--   0 ronald     (501) staff       (20)      709 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.2/Lib/CoreML/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    18671 2023-02-19 10:50:35.000000 pyobjc-framework-CoreML-9.2/Lib/CoreML/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:02.006482 pyobjc-framework-CoreML-9.2/Lib/pyobjc_framework_CoreML.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2094 2023-06-07 00:11:01.000000 pyobjc-framework-CoreML-9.2/Lib/pyobjc_framework_CoreML.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1887 2023-06-07 00:11:01.000000 pyobjc-framework-CoreML-9.2/Lib/pyobjc_framework_CoreML.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:11:01.000000 pyobjc-framework-CoreML-9.2/Lib/pyobjc_framework_CoreML.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:49.000000 pyobjc-framework-CoreML-9.2/Lib/pyobjc_framework_CoreML.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:11:01.000000 pyobjc-framework-CoreML-9.2/Lib/pyobjc_framework_CoreML.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        7 2023-06-07 00:11:01.000000 pyobjc-framework-CoreML-9.2/Lib/pyobjc_framework_CoreML.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreML-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:02.009643 pyobjc-framework-CoreML-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      799 2021-10-18 19:38:40.000000 pyobjc-framework-CoreML-9.2/Modules/_CoreML.m
+-rw-r--r--   0 ronald     (501) staff       (20)      659 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.2/Modules/_CoreML_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreML-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CoreML-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1883 2023-06-07 00:11:02.083829 pyobjc-framework-CoreML-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:02.040505 pyobjc-framework-CoreML-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      196 2022-04-11 08:03:15.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_coreml.py
+-rw-r--r--   0 ronald     (501) staff       (20)      667 2022-06-25 09:09:12.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlbatchprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1608 2022-06-25 20:16:10.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlcustomlayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      963 2022-06-25 20:18:13.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlcustommodel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      298 2021-03-21 10:08:22.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mldictionaryfeatureprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      401 2021-03-21 10:08:22.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlfeaturedescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      251 2022-06-25 20:10:17.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlfeatureprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      608 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlfeaturetype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      403 2021-03-21 10:08:22.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlfeaturevalue.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1779 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlfeaturevalue_mlimageconversion.py
+-rw-r--r--   0 ronald     (501) staff       (20)      446 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlimagesizeconstrainttype.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1309 2022-06-23 11:03:28.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmodel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      428 2022-06-23 11:03:28.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmodel_mlmodelcompilation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      281 2022-06-23 11:03:28.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmodelasset.py
+-rw-r--r--   0 ronald     (501) staff       (20)      668 2021-07-30 09:00:37.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmodelcollection.py
+-rw-r--r--   0 ronald     (501) staff       (20)      887 2023-02-19 10:50:35.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmodelconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      955 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmodelerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      589 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmodelmetadatakeys.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1764 2022-06-26 20:17:38.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmultiarray.py
+-rw-r--r--   0 ronald     (501) staff       (20)      476 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmultiarrayshapeconstrainttype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      323 2021-03-21 10:08:22.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlpredictionoptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)      482 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mltask.py
+-rw-r--r--   0 ronald     (501) staff       (20)      448 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlupdateprogressevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      519 2021-03-21 10:08:22.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlupdateprogresshandlers.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1206 2021-07-30 09:00:37.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlupdatetask.py
+-rw-r--r--   0 ronald     (501) staff       (20)      493 2022-06-25 20:08:48.000000 pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlwritable.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:02.042014 pyobjc-framework-CoreML-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    12976 2023-02-19 10:50:35.000000 pyobjc-framework-CoreML-9.2/metadata/CoreML.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:02.082563 pyobjc-framework-CoreML-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    84874 2022-01-02 11:04:26.000000 pyobjc-framework-CoreML-9.2/metadata/raw/arm64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    85290 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    90189 2022-06-23 11:03:28.000000 pyobjc-framework-CoreML-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    90083 2023-02-19 10:50:35.000000 pyobjc-framework-CoreML-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    41850 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    73239 2020-11-30 18:45:14.000000 pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    83339 2021-03-21 10:08:22.000000 pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    84875 2022-01-02 11:04:26.000000 pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    85291 2022-02-24 08:47:16.000000 pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    90190 2022-06-23 11:03:28.000000 pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    90084 2023-02-19 10:50:35.000000 pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreML-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreML-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:11:02.084446 pyobjc-framework-CoreML-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1182 2023-05-29 10:07:45.000000 pyobjc-framework-CoreML-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreML-9.1b1/Lib/CoreML/__init__.py` & `pyobjc-framework-CoreML-9.2/Lib/CoreML/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/Lib/CoreML/_metadata.py` & `pyobjc-framework-CoreML-9.2/Lib/CoreML/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/Lib/pyobjc_framework_CoreML.egg-info/PKG-INFO` & `pyobjc-framework-CoreML-9.2/Lib/pyobjc_framework_CoreML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreML
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreML on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreML
 Platform: MacOS X (>=10.13)
```

### Comparing `pyobjc-framework-CoreML-9.1b1/Lib/pyobjc_framework_CoreML.egg-info/SOURCES.txt` & `pyobjc-framework-CoreML-9.2/Lib/pyobjc_framework_CoreML.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CoreML/__init__.py
 Lib/CoreML/_metadata.py
 Lib/pyobjc_framework_CoreML.egg-info/PKG-INFO
 Lib/pyobjc_framework_CoreML.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CoreML.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CoreML.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CoreML-9.1b1/License.txt` & `pyobjc-framework-CoreML-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/Modules/_CoreML.m` & `pyobjc-framework-CoreML-9.2/Modules/_CoreML.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/Modules/_CoreML_protocols.m` & `pyobjc-framework-CoreML-9.2/Modules/_CoreML_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreML-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreML-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CoreML-9.1b1/PKG-INFO` & `pyobjc-framework-CoreML-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreML
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreML on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreML
 Platform: MacOS X (>=10.13)
```

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlbatchprovider.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlbatchprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlcustomlayer.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlcustomlayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlcustommodel.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlcustommodel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlfeaturetype.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlfeaturetype.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlfeaturevalue_mlimageconversion.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlfeaturevalue_mlimageconversion.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmodel.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmodel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmodelcollection.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmodelcollection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmodelconfiguration.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmodelconfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmodelerror.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmodelerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmodelmetadatakeys.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmodelmetadatakeys.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlmultiarray.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlmultiarray.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlupdateprogresshandlers.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlupdateprogresshandlers.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/PyObjCTest/test_mlupdatetask.py` & `pyobjc-framework-CoreML-9.2/PyObjCTest/test_mlupdatetask.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/metadata/CoreML.fwinfo` & `pyobjc-framework-CoreML-9.2/metadata/CoreML.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/metadata/raw/arm64-12.1.fwinfo` & `pyobjc-framework-CoreML-9.2/metadata/raw/arm64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreML-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-CoreML-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-CoreML-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-10.14.fwinfo` & `pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-12.1.fwinfo` & `pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-CoreML-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreML-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreML-9.1b1/setup.py` & `pyobjc-framework-CoreML-9.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,22 @@
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
     name="pyobjc-framework-CoreML",
     description="Wrappers for the framework CoreML on macOS",
     min_os_level="10.13",
     packages=["CoreML"],
     ext_modules=[
```

