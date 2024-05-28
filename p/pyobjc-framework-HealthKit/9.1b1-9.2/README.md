# Comparing `tmp/pyobjc-framework-HealthKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-HealthKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-HealthKit-9.1b1.tar", last modified: Sun Mar 26 11:26:04 2023, max compression
+gzip compressed data, was "pyobjc-framework-HealthKit-9.2.tar", last modified: Wed Jun  7 00:16:21 2023, max compression
```

## Comparing `pyobjc-framework-HealthKit-9.1b1.tar` & `pyobjc-framework-HealthKit-9.2.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:04.285266 pyobjc-framework-HealthKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:04.154294 pyobjc-framework-HealthKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:04.159576 pyobjc-framework-HealthKit-9.1b1/Lib/HealthKit/
--rw-r--r--   0 ronald     (501) staff       (20)      757 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/Lib/HealthKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    76928 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.1b1/Lib/HealthKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:04.168803 pyobjc-framework-HealthKit-9.1b1/Lib/pyobjc_framework_HealthKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2107 2023-03-26 11:26:04.000000 pyobjc-framework-HealthKit-9.1b1/Lib/pyobjc_framework_HealthKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     2953 2023-03-26 11:26:04.000000 pyobjc-framework-HealthKit-9.1b1/Lib/pyobjc_framework_HealthKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:26:04.000000 pyobjc-framework-HealthKit-9.1b1/Lib/pyobjc_framework_HealthKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2022-06-23 11:14:43.000000 pyobjc-framework-HealthKit-9.1b1/Lib/pyobjc_framework_HealthKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:26:04.000000 pyobjc-framework-HealthKit-9.1b1/Lib/pyobjc_framework_HealthKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:26:04.000000 pyobjc-framework-HealthKit-9.1b1/Lib/pyobjc_framework_HealthKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-06-23 11:03:47.000000 pyobjc-framework-HealthKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-23 11:03:47.000000 pyobjc-framework-HealthKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:04.172734 pyobjc-framework-HealthKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      817 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/Modules/_HealthKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      452 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/Modules/_HealthKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-HealthKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1896 2023-03-26 11:26:04.284916 pyobjc-framework-HealthKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:04.261773 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      194 2022-06-27 18:36:42.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_healthkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      587 2022-10-18 09:53:24.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkHeartbeatseriesbuilder.py
--rw-r--r--   0 ronald     (501) staff       (20)      212 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkactivitysummary.py
--rw-r--r--   0 ronald     (501) staff       (20)      522 2022-06-27 07:36:11.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkactivitysummaryquery.py
--rw-r--r--   0 ronald     (501) staff       (20)      822 2022-06-27 07:40:02.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkanchoredobjectquery.py
--rw-r--r--   0 ronald     (501) staff       (20)      811 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkapplewalkingsteadinessclassification.py
--rw-r--r--   0 ronald     (501) staff       (20)      852 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkattachmentstore.py
--rw-r--r--   0 ronald     (501) staff       (20)      312 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkaudiogramsample.py
--rw-r--r--   0 ronald     (501) staff       (20)      210 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkcategorysample.py
--rw-r--r--   0 ronald     (501) staff       (20)      724 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkcdadocumentsample.py
--rw-r--r--   0 ronald     (501) staff       (20)      372 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkclinicalrecord.py
--rw-r--r--   0 ronald     (501) staff       (20)     1056 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkclinicaltype.py
--rw-r--r--   0 ronald     (501) staff       (20)      303 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkcorrelationquery.py
--rw-r--r--   0 ronald     (501) staff       (20)      210 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkcumulativequantitysample.py
--rw-r--r--   0 ronald     (501) staff       (20)    10017 2022-06-27 19:02:38.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkdefines.py
--rw-r--r--   0 ronald     (501) staff       (20)      752 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkdevice.py
--rw-r--r--   0 ronald     (501) staff       (20)      672 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkdiscretequantitysample.py
--rw-r--r--   0 ronald     (501) staff       (20)      597 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkdocumentquery.py
--rw-r--r--   0 ronald     (501) staff       (20)     1753 2022-10-18 09:53:24.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkeLectrocardiogram.py
--rw-r--r--   0 ronald     (501) staff       (20)      303 2022-06-27 07:33:59.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkelectrocardiogramquery.py
--rw-r--r--   0 ronald     (501) staff       (20)      384 2022-10-18 09:53:24.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkfhirRelease.py
--rw-r--r--   0 ronald     (501) staff       (20)     1220 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkfhirresource.py
--rw-r--r--   0 ronald     (501) staff       (20)      215 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkfhirversion.py
--rw-r--r--   0 ronald     (501) staff       (20)     3621 2022-06-26 21:48:13.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkhealthstore.py
--rw-r--r--   0 ronald     (501) staff       (20)      298 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkheartbeatseriesquery.py
--rw-r--r--   0 ronald     (501) staff       (20)      472 2022-06-25 20:13:31.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkliveworkoutbuilder.py
--rw-r--r--   0 ronald     (501) staff       (20)    11876 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkmetadata.py
--rw-r--r--   0 ronald     (501) staff       (20)      635 2022-10-18 09:53:24.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkoBject.py
--rw-r--r--   0 ronald     (501) staff       (20)      469 2022-06-27 07:05:27.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkobjecttype.py
--rw-r--r--   0 ronald     (501) staff       (20)      462 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkobserverquery.py
--rw-r--r--   0 ronald     (501) staff       (20)      200 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkquantity.py
--rw-r--r--   0 ronald     (501) staff       (20)      767 2022-06-27 19:02:38.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkquantityaggregationstyle.py
--rw-r--r--   0 ronald     (501) staff       (20)      275 2022-06-27 07:23:17.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkquantitysample.py
--rw-r--r--   0 ronald     (501) staff       (20)     1000 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkquantityseriessamplebuilder.py
--rw-r--r--   0 ronald     (501) staff       (20)      910 2022-06-27 07:33:25.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkquantityseriessamplequery.py
--rw-r--r--   0 ronald     (501) staff       (20)      380 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkquery.py
--rw-r--r--   0 ronald     (501) staff       (20)      530 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hksample.py
--rw-r--r--   0 ronald     (501) staff       (20)      737 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hksamplequery.py
--rw-r--r--   0 ronald     (501) staff       (20)      295 2022-06-27 07:37:27.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hksourcequery.py
--rw-r--r--   0 ronald     (501) staff       (20)      430 2022-06-27 07:18:05.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hksourcerevision.py
--rw-r--r--   0 ronald     (501) staff       (20)      924 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkstatistics.py
--rw-r--r--   0 ronald     (501) staff       (20)      851 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkstatisticscollectionquery.py
--rw-r--r--   0 ronald     (501) staff       (20)      321 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkstatisticsquery.py
--rw-r--r--   0 ronald     (501) staff       (20)    17553 2022-10-19 09:49:10.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hktypeidentifiers.py
--rw-r--r--   0 ronald     (501) staff       (20)     1085 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkunit.py
--rw-r--r--   0 ronald     (501) staff       (20)     1040 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkverifiableclinicalrecord.py
--rw-r--r--   0 ronald     (501) staff       (20)      513 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkverifiableclinicalrecordquery.py
--rw-r--r--   0 ronald     (501) staff       (20)      279 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkvisionprescription.py
--rw-r--r--   0 ronald     (501) staff       (20)      617 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkvisionprism.py
--rw-r--r--   0 ronald     (501) staff       (20)     8288 2022-06-26 21:43:53.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkworkout.py
--rw-r--r--   0 ronald     (501) staff       (20)      945 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkworkoutactivity.py
--rw-r--r--   0 ronald     (501) staff       (20)     1200 2022-06-27 06:27:47.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkworkoutbuilder.py
--rw-r--r--   0 ronald     (501) staff       (20)      432 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkworkoutconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      544 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkworkoutroutebuilder.py
--rw-r--r--   0 ronald     (501) staff       (20)      417 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkworkoutroutequery.py
--rw-r--r--   0 ronald     (501) staff       (20)      936 2022-06-25 20:14:39.000000 pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkworkoutsession.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:04.264666 pyobjc-framework-HealthKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     7009 2022-06-27 07:45:13.000000 pyobjc-framework-HealthKit-9.1b1/metadata/HealthKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:04.282886 pyobjc-framework-HealthKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   301906 2022-10-19 09:49:10.000000 pyobjc-framework-HealthKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   303650 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   301907 2022-10-19 09:49:10.000000 pyobjc-framework-HealthKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   303651 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-HealthKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:26:04.285369 pyobjc-framework-HealthKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1161 2023-03-25 14:20:31.000000 pyobjc-framework-HealthKit-9.1b1/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      465 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.1b1/t.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:21.217937 pyobjc-framework-HealthKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:21.090591 pyobjc-framework-HealthKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:21.098053 pyobjc-framework-HealthKit-9.2/Lib/HealthKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      757 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/Lib/HealthKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    76955 2023-05-27 09:46:33.000000 pyobjc-framework-HealthKit-9.2/Lib/HealthKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:21.102721 pyobjc-framework-HealthKit-9.2/Lib/pyobjc_framework_HealthKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2105 2023-06-07 00:16:21.000000 pyobjc-framework-HealthKit-9.2/Lib/pyobjc_framework_HealthKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     2968 2023-06-07 00:16:21.000000 pyobjc-framework-HealthKit-9.2/Lib/pyobjc_framework_HealthKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:16:21.000000 pyobjc-framework-HealthKit-9.2/Lib/pyobjc_framework_HealthKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2022-06-23 11:14:43.000000 pyobjc-framework-HealthKit-9.2/Lib/pyobjc_framework_HealthKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:16:21.000000 pyobjc-framework-HealthKit-9.2/Lib/pyobjc_framework_HealthKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:16:21.000000 pyobjc-framework-HealthKit-9.2/Lib/pyobjc_framework_HealthKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-06-23 11:03:47.000000 pyobjc-framework-HealthKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-23 11:03:47.000000 pyobjc-framework-HealthKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:21.105830 pyobjc-framework-HealthKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      817 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/Modules/_HealthKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      452 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/Modules/_HealthKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-HealthKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1894 2023-06-07 00:16:21.216874 pyobjc-framework-HealthKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:21.182370 pyobjc-framework-HealthKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      194 2022-06-27 18:36:42.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_healthkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      587 2022-10-18 09:53:24.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkHeartbeatseriesbuilder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      212 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkactivitysummary.py
+-rw-r--r--   0 ronald     (501) staff       (20)      522 2022-06-27 07:36:11.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkactivitysummaryquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      822 2022-06-27 07:40:02.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkanchoredobjectquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      811 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkapplewalkingsteadinessclassification.py
+-rw-r--r--   0 ronald     (501) staff       (20)      852 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkattachmentstore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      312 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkaudiogramsample.py
+-rw-r--r--   0 ronald     (501) staff       (20)      210 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkcategorysample.py
+-rw-r--r--   0 ronald     (501) staff       (20)      724 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkcdadocumentsample.py
+-rw-r--r--   0 ronald     (501) staff       (20)      372 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkclinicalrecord.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1056 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkclinicaltype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      303 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkcorrelationquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      210 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkcumulativequantitysample.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10017 2022-06-27 19:02:38.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkdefines.py
+-rw-r--r--   0 ronald     (501) staff       (20)      752 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkdevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)      672 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkdiscretequantitysample.py
+-rw-r--r--   0 ronald     (501) staff       (20)      597 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkdocumentquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1753 2022-10-18 09:53:24.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkeLectrocardiogram.py
+-rw-r--r--   0 ronald     (501) staff       (20)      303 2022-06-27 07:33:59.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkelectrocardiogramquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      384 2022-10-18 09:53:24.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkfhirRelease.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1220 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkfhirresource.py
+-rw-r--r--   0 ronald     (501) staff       (20)      215 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkfhirversion.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3621 2022-06-26 21:48:13.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkhealthstore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      298 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkheartbeatseriesquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      472 2022-06-25 20:13:31.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkliveworkoutbuilder.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11876 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkmetadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      635 2022-10-18 09:53:24.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkoBject.py
+-rw-r--r--   0 ronald     (501) staff       (20)      469 2022-06-27 07:05:27.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkobjecttype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      462 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkobserverquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkquantity.py
+-rw-r--r--   0 ronald     (501) staff       (20)      767 2022-06-27 19:02:38.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkquantityaggregationstyle.py
+-rw-r--r--   0 ronald     (501) staff       (20)      275 2022-06-27 07:23:17.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkquantitysample.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1000 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkquantityseriessamplebuilder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      910 2022-06-27 07:33:25.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkquantityseriessamplequery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      380 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      530 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hksample.py
+-rw-r--r--   0 ronald     (501) staff       (20)      737 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hksamplequery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      295 2022-06-27 07:37:27.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hksourcequery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      430 2022-06-27 07:18:05.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hksourcerevision.py
+-rw-r--r--   0 ronald     (501) staff       (20)      924 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkstatistics.py
+-rw-r--r--   0 ronald     (501) staff       (20)      851 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkstatisticscollectionquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      321 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkstatisticsquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)    17553 2022-10-19 09:49:10.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hktypeidentifiers.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1085 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkunit.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1040 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkverifiableclinicalrecord.py
+-rw-r--r--   0 ronald     (501) staff       (20)      513 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkverifiableclinicalrecordquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      279 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkvisionprescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      617 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkvisionprism.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8288 2022-06-26 21:43:53.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkworkout.py
+-rw-r--r--   0 ronald     (501) staff       (20)      945 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkworkoutactivity.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1200 2022-06-27 06:27:47.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkworkoutbuilder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      432 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkworkoutconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      544 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkworkoutroutebuilder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      417 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkworkoutroutequery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      936 2022-06-25 20:14:39.000000 pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkworkoutsession.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:21.183552 pyobjc-framework-HealthKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     7031 2023-05-27 09:46:33.000000 pyobjc-framework-HealthKit-9.2/metadata/HealthKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:21.210714 pyobjc-framework-HealthKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   301906 2022-10-19 09:49:10.000000 pyobjc-framework-HealthKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   303650 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   301907 2022-10-19 09:49:10.000000 pyobjc-framework-HealthKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   303651 2023-02-19 10:50:35.000000 pyobjc-framework-HealthKit-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-HealthKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-HealthKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:16:21.218040 pyobjc-framework-HealthKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-29 10:07:46.000000 pyobjc-framework-HealthKit-9.2/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      465 2022-06-23 11:03:28.000000 pyobjc-framework-HealthKit-9.2/t.py
```

### Comparing `pyobjc-framework-HealthKit-9.1b1/Lib/HealthKit/__init__.py` & `pyobjc-framework-HealthKit-9.2/Lib/HealthKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/Lib/HealthKit/_metadata.py` & `pyobjc-framework-HealthKit-9.2/Lib/HealthKit/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Feb 17 21:51:29 2023
+# Last update: Sat May 20 12:10:42 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -139,15 +139,15 @@
     }
 )
 misc.update({"HKUnitMolarMassBloodGlucose": 180.15588000005408})
 functions = {
     "HKAppleWalkingSteadinessClassificationForQuantity": (
         b"Z@^q^@",
         "",
-        {"arguments": {2: {"type_modifier": "o"}}},
+        {"arguments": {1: {"type_modifier": "o"}, 2: {"type_modifier": "o"}}},
     ),
     "HKAppleWalkingSteadinessMinimumQuantityForClassification": (b"@q",),
     "HKAppleWalkingSteadinessMaximumQuantityForClassification": (b"@q",),
     "HKCategoryValueSleepAnalysisAsleepValues": (b"@",),
 }
 aliases = {
     "HKCategoryValueSleepAnalysisAsleep": "HKCategoryValueSleepAnalysisAsleepUnspecified",
```

### Comparing `pyobjc-framework-HealthKit-9.1b1/Lib/pyobjc_framework_HealthKit.egg-info/PKG-INFO` & `pyobjc-framework-HealthKit-9.2/Lib/pyobjc_framework_HealthKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-HealthKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework HealthKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,HealthKit
 Platform: MacOS X (>=13.0)
```

### Comparing `pyobjc-framework-HealthKit-9.1b1/Lib/pyobjc_framework_HealthKit.egg-info/SOURCES.txt` & `pyobjc-framework-HealthKit-9.2/Lib/pyobjc_framework_HealthKit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 t.py
 Lib/HealthKit/__init__.py
 Lib/HealthKit/_metadata.py
 Lib/pyobjc_framework_HealthKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_HealthKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_HealthKit.egg-info/dependency_links.txt
```

### Comparing `pyobjc-framework-HealthKit-9.1b1/License.txt` & `pyobjc-framework-HealthKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/Modules/_HealthKit.m` & `pyobjc-framework-HealthKit-9.2/Modules/_HealthKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-HealthKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-HealthKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-HealthKit-9.1b1/PKG-INFO` & `pyobjc-framework-HealthKit-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-HealthKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework HealthKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,HealthKit
 Platform: MacOS X (>=13.0)
```

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkHeartbeatseriesbuilder.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkHeartbeatseriesbuilder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkactivitysummaryquery.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkactivitysummaryquery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkanchoredobjectquery.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkanchoredobjectquery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkapplewalkingsteadinessclassification.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkapplewalkingsteadinessclassification.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkattachmentstore.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkattachmentstore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkcdadocumentsample.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkcdadocumentsample.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkclinicaltype.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkclinicaltype.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkdefines.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkdefines.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkdevice.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkdevice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkdiscretequantitysample.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkdiscretequantitysample.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkdocumentquery.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkdocumentquery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkeLectrocardiogram.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkeLectrocardiogram.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkfhirresource.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkfhirresource.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkhealthstore.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkhealthstore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkmetadata.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkmetadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkoBject.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkoBject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkquantityaggregationstyle.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkquantityaggregationstyle.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkquantityseriessamplebuilder.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkquantityseriessamplebuilder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkquantityseriessamplequery.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkquantityseriessamplequery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hksample.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hksample.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hksamplequery.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hksamplequery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkstatistics.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkstatistics.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkstatisticscollectionquery.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkstatisticscollectionquery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hktypeidentifiers.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hktypeidentifiers.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkunit.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkunit.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkverifiableclinicalrecord.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkverifiableclinicalrecord.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkverifiableclinicalrecordquery.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkverifiableclinicalrecordquery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkvisionprism.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkvisionprism.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkworkout.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkworkout.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkworkoutactivity.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkworkoutactivity.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkworkoutbuilder.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkworkoutbuilder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkworkoutroutebuilder.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkworkoutroutebuilder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/PyObjCTest/test_hkworkoutsession.py` & `pyobjc-framework-HealthKit-9.2/PyObjCTest/test_hkworkoutsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/metadata/HealthKit.fwinfo` & `pyobjc-framework-HealthKit-9.2/metadata/HealthKit.fwinfo`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333333%*

 * *Differences: {"'definitions'": "{'functions': {'HKAppleWalkingSteadinessClassificationForQuantity': {'args': "*

 * *                  "{'1': {replace: OrderedDict([('type_modifier', 'o')])}}}}}"}*

```diff
@@ -395,15 +395,17 @@
                 "value": 0
             }
         },
         "formal_protocols": {},
         "functions": {
             "HKAppleWalkingSteadinessClassificationForQuantity": {
                 "args": {
-                    "1": {},
+                    "1": {
+                        "type_modifier": "o"
+                    },
                     "2": {
                         "type_modifier": "o"
                     }
                 }
             }
         },
         "informal_protocols": {},
```

### Comparing `pyobjc-framework-HealthKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-HealthKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-HealthKit-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-HealthKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-HealthKit-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-HealthKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-HealthKit-9.1b1/setup.py` & `pyobjc-framework-HealthKit-9.2/setup.py`

 * *Files 4% similar despite different names*

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
     name="pyobjc-framework-HealthKit",
     description="Wrappers for the framework HealthKit on macOS",
     min_os_level="13.0",
     packages=["HealthKit"],
     ext_modules=[
```

