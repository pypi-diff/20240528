# Comparing `tmp/pyobjc-framework-Vision-9.1b1.tar.gz` & `tmp/pyobjc-framework-Vision-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Vision-9.1b1.tar", last modified: Sun Mar 26 11:43:56 2023, max compression
+gzip compressed data, was "pyobjc-framework-Vision-9.2.tar", last modified: Wed Jun  7 00:31:44 2023, max compression
```

## Comparing `pyobjc-framework-Vision-9.1b1.tar` & `pyobjc-framework-Vision-9.2.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:56.929371 pyobjc-framework-Vision-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:56.797547 pyobjc-framework-Vision-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:56.802827 pyobjc-framework-Vision-9.1b1/Lib/Vision/
--rw-r--r--   0 ronald     (501) staff       (20)      753 2020-11-30 18:45:15.000000 pyobjc-framework-Vision-9.1b1/Lib/Vision/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    46356 2022-10-21 10:39:56.000000 pyobjc-framework-Vision-9.1b1/Lib/Vision/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:56.806626 pyobjc-framework-Vision-9.1b1/Lib/pyobjc_framework_Vision.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2096 2023-03-26 11:43:56.000000 pyobjc-framework-Vision-9.1b1/Lib/pyobjc_framework_Vision.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     2736 2023-03-26 11:43:56.000000 pyobjc-framework-Vision-9.1b1/Lib/pyobjc_framework_Vision.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:43:56.000000 pyobjc-framework-Vision-9.1b1/Lib/pyobjc_framework_Vision.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:59.000000 pyobjc-framework-Vision-9.1b1/Lib/pyobjc_framework_Vision.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)      111 2023-03-26 11:43:56.000000 pyobjc-framework-Vision-9.1b1/Lib/pyobjc_framework_Vision.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        7 2023-03-26 11:43:56.000000 pyobjc-framework-Vision-9.1b1/Lib/pyobjc_framework_Vision.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Vision-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Vision-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:56.830752 pyobjc-framework-Vision-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     5928 2022-10-18 09:53:23.000000 pyobjc-framework-Vision-9.1b1/Modules/_Vision.m
--rw-r--r--   0 ronald     (501) staff       (20)      454 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/Modules/_Vision_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-Vision-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-Vision-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1885 2023-03-26 11:43:56.929038 pyobjc-framework-Vision-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:56.888913 pyobjc-framework-Vision-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      367 2022-04-11 08:03:15.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vision.py
--rw-r--r--   0 ronald     (501) staff       (20)      575 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnclassifyimagerequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      574 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vncoremlrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      537 2022-06-23 11:03:28.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetectbarcodesrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      616 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetectcontoursrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      229 2021-07-30 16:20:55.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetectdocumentsegmentationrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      376 2022-10-18 09:53:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetectfacecapturequalityRequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      282 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetectfacelandmarks.py
--rw-r--r--   0 ronald     (501) staff       (20)      836 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetectfacelandmarksrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      367 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetectfacerectanglesrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      203 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetecthorizonrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     5968 2022-10-18 09:53:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetecthumanHandposerequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     5263 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetecthumanbodyposerequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      542 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetecthumanrectanglesrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      264 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetectpoint.py
--rw-r--r--   0 ronald     (501) staff       (20)      209 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetectrectanglesrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      521 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetecttextrectanglesrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      677 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetecttrajectoriesrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1412 2022-06-23 11:03:28.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      373 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnfacelandmarks.py
--rw-r--r--   0 ronald     (501) staff       (20)      264 2022-06-25 20:14:56.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnfaceobservationaccepting.py
--rw-r--r--   0 ronald     (501) staff       (20)      269 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vngenerateattentionbasedsaliencyimagerequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      227 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vngenerateimagefeatureprintrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      271 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vngenerateobjectnessbasedsaliencyimagerequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1081 2022-06-23 11:03:28.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vngenerateopticalflowrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1076 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vngeneratepersonsegmentationrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      569 2022-10-18 09:53:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vngeometry.py
--rw-r--r--   0 ronald     (501) staff       (20)     1762 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vngeometryutils.py
--rw-r--r--   0 ronald     (501) staff       (20)      307 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnimageregistrationrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1956 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnobservation.py
--rw-r--r--   0 ronald     (501) staff       (20)      953 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnrecognizeanimalsrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1539 2022-06-23 11:03:28.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnrecognizetextrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1384 2022-06-25 20:16:18.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     3879 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnrequesthandler.py
--rw-r--r--   0 ronald     (501) staff       (20)      525 2022-06-25 09:27:19.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnrequestrevisionproviding.py
--rw-r--r--   0 ronald     (501) staff       (20)      450 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnstatefulrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     3675 2021-07-30 16:26:37.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vntargetedimagerequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      676 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vntrackingrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      642 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vntrackobjectrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      569 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vntrackrectanglerequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     3558 2022-06-23 11:03:28.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vntypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     2442 2022-10-18 09:53:23.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnutils.py
--rw-r--r--   0 ronald     (501) staff       (20)     1344 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnvideoprocessor.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:56.907221 pyobjc-framework-Vision-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    24685 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.1b1/metadata/Vision.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:15.000000 pyobjc-framework-Vision-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:56.926970 pyobjc-framework-Vision-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   181466 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   179453 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   186476 2022-10-21 10:40:12.000000 pyobjc-framework-Vision-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    91375 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   165338 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   181467 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   179454 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   186477 2022-10-21 10:40:11.000000 pyobjc-framework-Vision-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Vision-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:43:56.929515 pyobjc-framework-Vision-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1228 2023-03-25 14:20:32.000000 pyobjc-framework-Vision-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:44.279033 pyobjc-framework-Vision-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:44.179658 pyobjc-framework-Vision-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:44.196883 pyobjc-framework-Vision-9.2/Lib/Vision/
+-rw-r--r--   0 ronald     (501) staff       (20)      753 2020-11-30 18:45:15.000000 pyobjc-framework-Vision-9.2/Lib/Vision/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    46356 2022-10-21 10:39:56.000000 pyobjc-framework-Vision-9.2/Lib/Vision/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:44.201630 pyobjc-framework-Vision-9.2/Lib/pyobjc_framework_Vision.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2094 2023-06-07 00:31:44.000000 pyobjc-framework-Vision-9.2/Lib/pyobjc_framework_Vision.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     2751 2023-06-07 00:31:44.000000 pyobjc-framework-Vision-9.2/Lib/pyobjc_framework_Vision.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:31:44.000000 pyobjc-framework-Vision-9.2/Lib/pyobjc_framework_Vision.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:59.000000 pyobjc-framework-Vision-9.2/Lib/pyobjc_framework_Vision.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)      103 2023-06-07 00:31:44.000000 pyobjc-framework-Vision-9.2/Lib/pyobjc_framework_Vision.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        7 2023-06-07 00:31:44.000000 pyobjc-framework-Vision-9.2/Lib/pyobjc_framework_Vision.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Vision-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Vision-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:44.205172 pyobjc-framework-Vision-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     5928 2022-10-18 09:53:23.000000 pyobjc-framework-Vision-9.2/Modules/_Vision.m
+-rw-r--r--   0 ronald     (501) staff       (20)      454 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/Modules/_Vision_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-Vision-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-Vision-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1883 2023-06-07 00:31:44.278639 pyobjc-framework-Vision-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:44.263308 pyobjc-framework-Vision-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-Vision-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      367 2022-04-11 08:03:15.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vision.py
+-rw-r--r--   0 ronald     (501) staff       (20)      575 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnclassifyimagerequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      574 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vncoremlrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      537 2022-06-23 11:03:28.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetectbarcodesrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      616 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetectcontoursrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      229 2021-07-30 16:20:55.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetectdocumentsegmentationrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      376 2022-10-18 09:53:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetectfacecapturequalityRequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      282 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetectfacelandmarks.py
+-rw-r--r--   0 ronald     (501) staff       (20)      836 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetectfacelandmarksrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      367 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetectfacerectanglesrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      203 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetecthorizonrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5968 2022-10-18 09:53:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetecthumanHandposerequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5263 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetecthumanbodyposerequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      542 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetecthumanrectanglesrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      264 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetectpoint.py
+-rw-r--r--   0 ronald     (501) staff       (20)      209 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetectrectanglesrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      521 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetecttextrectanglesrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      677 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetecttrajectoriesrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1412 2022-06-23 11:03:28.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      373 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnfacelandmarks.py
+-rw-r--r--   0 ronald     (501) staff       (20)      264 2022-06-25 20:14:56.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnfaceobservationaccepting.py
+-rw-r--r--   0 ronald     (501) staff       (20)      269 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vngenerateattentionbasedsaliencyimagerequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      227 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vngenerateimagefeatureprintrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      271 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vngenerateobjectnessbasedsaliencyimagerequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1081 2022-06-23 11:03:28.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vngenerateopticalflowrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1076 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vngeneratepersonsegmentationrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      569 2022-10-18 09:53:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vngeometry.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1762 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vngeometryutils.py
+-rw-r--r--   0 ronald     (501) staff       (20)      307 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnimageregistrationrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1956 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnobservation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      953 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnrecognizeanimalsrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1539 2022-06-23 11:03:28.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnrecognizetextrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1384 2022-06-25 20:16:18.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3879 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnrequesthandler.py
+-rw-r--r--   0 ronald     (501) staff       (20)      525 2022-06-25 09:27:19.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnrequestrevisionproviding.py
+-rw-r--r--   0 ronald     (501) staff       (20)      450 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnstatefulrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3675 2021-07-30 16:26:37.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vntargetedimagerequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      676 2022-02-24 08:47:17.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vntrackingrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      642 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vntrackobjectrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      569 2021-03-21 10:08:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vntrackrectanglerequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3558 2022-06-23 11:03:28.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vntypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2442 2022-10-18 09:53:23.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnutils.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1344 2021-07-30 09:00:38.000000 pyobjc-framework-Vision-9.2/PyObjCTest/test_vnvideoprocessor.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:44.264898 pyobjc-framework-Vision-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    24685 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.2/metadata/Vision.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:15.000000 pyobjc-framework-Vision-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:44.276530 pyobjc-framework-Vision-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   181466 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   179453 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   186476 2022-10-21 10:40:12.000000 pyobjc-framework-Vision-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    91375 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   165338 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   181467 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   179454 2022-10-20 21:08:30.000000 pyobjc-framework-Vision-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   186477 2022-10-21 10:40:11.000000 pyobjc-framework-Vision-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Vision-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Vision-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:31:44.279145 pyobjc-framework-Vision-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1299 2023-05-29 10:07:47.000000 pyobjc-framework-Vision-9.2/setup.py
```

### Comparing `pyobjc-framework-Vision-9.1b1/Lib/Vision/__init__.py` & `pyobjc-framework-Vision-9.2/Lib/Vision/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/Lib/Vision/_metadata.py` & `pyobjc-framework-Vision-9.2/Lib/Vision/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/Lib/pyobjc_framework_Vision.egg-info/PKG-INFO` & `pyobjc-framework-Vision-9.2/Lib/pyobjc_framework_Vision.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Vision
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Vision on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Vision
 Platform: MacOS X (>=10.13)
```

### Comparing `pyobjc-framework-Vision-9.1b1/Lib/pyobjc_framework_Vision.egg-info/SOURCES.txt` & `pyobjc-framework-Vision-9.2/Lib/pyobjc_framework_Vision.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/Vision/__init__.py
 Lib/Vision/_metadata.py
 Lib/pyobjc_framework_Vision.egg-info/PKG-INFO
 Lib/pyobjc_framework_Vision.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Vision.egg-info/dependency_links.txt
 Lib/pyobjc_framework_Vision.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-Vision-9.1b1/License.txt` & `pyobjc-framework-Vision-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/Modules/_Vision.m` & `pyobjc-framework-Vision-9.2/Modules/_Vision.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-Vision-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-Vision-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-Vision-9.1b1/PKG-INFO` & `pyobjc-framework-Vision-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Vision
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Vision on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Vision
 Platform: MacOS X (>=10.13)
```

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnclassifyimagerequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vnclassifyimagerequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vncoremlrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vncoremlrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetectbarcodesrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetectbarcodesrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetectcontoursrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetectcontoursrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetectfacelandmarksrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetectfacelandmarksrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetecthumanHandposerequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetecthumanHandposerequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetecthumanbodyposerequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetecthumanbodyposerequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetecthumanrectanglesrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetecthumanrectanglesrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetecttextrectanglesrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetecttextrectanglesrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vndetecttrajectoriesrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vndetecttrajectoriesrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnerror.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vnerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vngenerateopticalflowrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vngenerateopticalflowrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vngeneratepersonsegmentationrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vngeneratepersonsegmentationrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vngeometry.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vngeometry.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vngeometryutils.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vngeometryutils.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnobservation.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vnobservation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnrecognizeanimalsrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vnrecognizeanimalsrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnrecognizetextrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vnrecognizetextrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vnrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnrequesthandler.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vnrequesthandler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnrequestrevisionproviding.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vnrequestrevisionproviding.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vntargetedimagerequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vntargetedimagerequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vntrackingrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vntrackingrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vntrackobjectrequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vntrackobjectrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vntrackrectanglerequest.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vntrackrectanglerequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vntypes.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vntypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnutils.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vnutils.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/PyObjCTest/test_vnvideoprocessor.py` & `pyobjc-framework-Vision-9.2/PyObjCTest/test_vnvideoprocessor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/metadata/Vision.fwinfo` & `pyobjc-framework-Vision-9.2/metadata/Vision.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-Vision-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Vision-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-Vision-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-Vision-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-Vision-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-Vision-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Vision-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-Vision-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Vision-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Vision-9.1b1/setup.py` & `pyobjc-framework-Vision-9.2/setup.py`

 * *Files 10% similar despite different names*

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
     name="pyobjc-framework-Vision",
     description="Wrappers for the framework Vision on macOS",
     min_os_level="10.13",
     packages=["Vision"],
     ext_modules=[
```

