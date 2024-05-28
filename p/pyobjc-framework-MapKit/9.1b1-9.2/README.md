# Comparing `tmp/pyobjc-framework-MapKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-MapKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MapKit-9.1b1.tar", last modified: Sun Mar 26 11:28:31 2023, max compression
+gzip compressed data, was "pyobjc-framework-MapKit-9.2.tar", last modified: Wed Jun  7 00:19:03 2023, max compression
```

## Comparing `pyobjc-framework-MapKit-9.1b1.tar` & `pyobjc-framework-MapKit-9.2.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:31.834854 pyobjc-framework-MapKit-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MapKit-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:31.658146 pyobjc-framework-MapKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:31.667809 pyobjc-framework-MapKit-9.1b1/Lib/MapKit/
--rw-r--r--   0 ronald     (501) staff       (20)      822 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.1b1/Lib/MapKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    45010 2022-10-18 09:53:23.000000 pyobjc-framework-MapKit-9.1b1/Lib/MapKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:31.673225 pyobjc-framework-MapKit-9.1b1/Lib/pyobjc_framework_MapKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2121 2023-03-26 11:28:31.000000 pyobjc-framework-MapKit-9.1b1/Lib/pyobjc_framework_MapKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     2692 2023-03-26 11:28:31.000000 pyobjc-framework-MapKit-9.1b1/Lib/pyobjc_framework_MapKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:28:31.000000 pyobjc-framework-MapKit-9.1b1/Lib/pyobjc_framework_MapKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:15.000000 pyobjc-framework-MapKit-9.1b1/Lib/pyobjc_framework_MapKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)      117 2023-03-26 11:28:31.000000 pyobjc-framework-MapKit-9.1b1/Lib/pyobjc_framework_MapKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        7 2023-03-26 11:28:31.000000 pyobjc-framework-MapKit-9.1b1/Lib/pyobjc_framework_MapKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:31.677903 pyobjc-framework-MapKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1122 2021-10-18 19:38:40.000000 pyobjc-framework-MapKit-9.1b1/Modules/_MapKit.m
--rw-r--r--   0 ronald     (501) staff       (20)     3080 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/Modules/_MapKit_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)      873 2022-06-15 11:57:00.000000 pyobjc-framework-MapKit-9.1b1/Modules/_MapKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MapKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-MapKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1910 2023-03-26 11:28:31.834017 pyobjc-framework-MapKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:31.781248 pyobjc-framework-MapKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      196 2022-04-11 08:03:15.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mapkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      654 2022-06-25 20:16:45.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkannotation.py
--rw-r--r--   0 ronald     (501) staff       (20)     3860 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkannotationview.py
--rw-r--r--   0 ronald     (501) staff       (20)      235 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkcircle.py
--rw-r--r--   0 ronald     (501) staff       (20)      251 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkcirclerenderer.py
--rw-r--r--   0 ronald     (501) staff       (20)      653 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkdirections.py
--rw-r--r--   0 ronald     (501) staff       (20)      748 2022-06-15 11:57:00.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkdirectionsrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      633 2022-06-26 20:31:08.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkdirectionsresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)      627 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkdirectionstypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      834 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkdistanceformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)      659 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkgeodesicpolyline.py
--rw-r--r--   0 ronald     (501) staff       (20)      388 2022-06-25 20:13:07.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkgeojsonserialization.py
--rw-r--r--   0 ronald     (501) staff       (20)     6201 2022-01-02 11:04:26.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkgeometry.py
--rw-r--r--   0 ronald     (501) staff       (20)      340 2022-06-15 11:57:00.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkhybridmapconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      515 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mklocalsearch.py
--rw-r--r--   0 ronald     (501) staff       (20)     1001 2022-06-25 20:16:02.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mklocalsearchcompleter.py
--rw-r--r--   0 ronald     (501) staff       (20)      536 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mklocalsearchrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      261 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mklocalsearchresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)      459 2022-06-15 11:57:00.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mklookaroundscenerequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      383 2022-06-15 11:57:00.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mklookaroundsnapshotter.py
--rw-r--r--   0 ronald     (501) staff       (20)      995 2022-06-25 20:13:38.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mklookaroundviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      421 2022-06-15 11:57:00.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmapcamera.py
--rw-r--r--   0 ronald     (501) staff       (20)      243 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmapcamerazoomrange.py
--rw-r--r--   0 ronald     (501) staff       (20)      315 2022-06-25 20:19:21.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmapconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)     1793 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmapitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      245 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmapsnapshot.py
--rw-r--r--   0 ronald     (501) staff       (20)      500 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmapsnapshotoptions.py
--rw-r--r--   0 ronald     (501) staff       (20)      831 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmapsnapshotter.py
--rw-r--r--   0 ronald     (501) staff       (20)     4294 2022-06-26 21:30:10.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmapview.py
--rw-r--r--   0 ronald     (501) staff       (20)      525 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmultipoint.py
--rw-r--r--   0 ronald     (501) staff       (20)     1016 2022-06-25 20:13:48.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkoverlay.py
--rw-r--r--   0 ronald     (501) staff       (20)      477 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkoverlaypathrenderer.py
--rw-r--r--   0 ronald     (501) staff       (20)      432 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkoverlayrenderer.py
--rw-r--r--   0 ronald     (501) staff       (20)      740 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkpinannotationview.py
--rw-r--r--   0 ronald     (501) staff       (20)      241 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkplacemark.py
--rw-r--r--   0 ronald     (501) staff       (20)      253 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkpointannotation.py
--rw-r--r--   0 ronald     (501) staff       (20)     3355 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkpointofinterestcategory.py
--rw-r--r--   0 ronald     (501) staff       (20)      340 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkpointofinterestfilter.py
--rw-r--r--   0 ronald     (501) staff       (20)     1033 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkpolygon.py
--rw-r--r--   0 ronald     (501) staff       (20)      253 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkpolygonrenderer.py
--rw-r--r--   0 ronald     (501) staff       (20)      567 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkpolyline.py
--rw-r--r--   0 ronald     (501) staff       (20)      255 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkpolylinerenderer.py
--rw-r--r--   0 ronald     (501) staff       (20)      233 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkshape.py
--rw-r--r--   0 ronald     (501) staff       (20)      587 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mksnapshotoptions.py
--rw-r--r--   0 ronald     (501) staff       (20)      580 2022-06-25 20:19:21.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkstandardmapconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      945 2022-01-02 11:04:26.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mktileoverlay.py
--rw-r--r--   0 ronald     (501) staff       (20)      261 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mktileoverlayrenderer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1350 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mktypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      314 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkuserlocation.py
--rw-r--r--   0 ronald     (501) staff       (20)      312 2021-10-18 19:38:40.000000 pyobjc-framework-MapKit-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:31.782912 pyobjc-framework-MapKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     6774 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.1b1/metadata/MapKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:31.827152 pyobjc-framework-MapKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   210495 2021-07-30 09:00:38.000000 pyobjc-framework-MapKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   211255 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   242721 2022-10-18 09:53:23.000000 pyobjc-framework-MapKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   137583 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   186396 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   210496 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   136737 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-10.9.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   210496 2021-07-30 09:00:38.000000 pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   211256 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   242722 2022-10-18 09:53:23.000000 pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MapKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:28:31.834987 pyobjc-framework-MapKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1303 2023-03-25 14:20:31.000000 pyobjc-framework-MapKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:03.052708 pyobjc-framework-MapKit-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MapKit-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:02.929739 pyobjc-framework-MapKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:02.946482 pyobjc-framework-MapKit-9.2/Lib/MapKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      822 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.2/Lib/MapKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    45010 2022-10-18 09:53:23.000000 pyobjc-framework-MapKit-9.2/Lib/MapKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:02.950957 pyobjc-framework-MapKit-9.2/Lib/pyobjc_framework_MapKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2119 2023-06-07 00:19:02.000000 pyobjc-framework-MapKit-9.2/Lib/pyobjc_framework_MapKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     2707 2023-06-07 00:19:02.000000 pyobjc-framework-MapKit-9.2/Lib/pyobjc_framework_MapKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:19:02.000000 pyobjc-framework-MapKit-9.2/Lib/pyobjc_framework_MapKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:15.000000 pyobjc-framework-MapKit-9.2/Lib/pyobjc_framework_MapKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)      109 2023-06-07 00:19:02.000000 pyobjc-framework-MapKit-9.2/Lib/pyobjc_framework_MapKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        7 2023-06-07 00:19:02.000000 pyobjc-framework-MapKit-9.2/Lib/pyobjc_framework_MapKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:02.956452 pyobjc-framework-MapKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1122 2021-10-18 19:38:40.000000 pyobjc-framework-MapKit-9.2/Modules/_MapKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3080 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/Modules/_MapKit_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)      873 2022-06-15 11:57:00.000000 pyobjc-framework-MapKit-9.2/Modules/_MapKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MapKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-MapKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1908 2023-06-07 00:19:03.052294 pyobjc-framework-MapKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:03.016167 pyobjc-framework-MapKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      196 2022-04-11 08:03:15.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mapkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      654 2022-06-25 20:16:45.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkannotation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3860 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkannotationview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      235 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkcircle.py
+-rw-r--r--   0 ronald     (501) staff       (20)      251 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkcirclerenderer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      653 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkdirections.py
+-rw-r--r--   0 ronald     (501) staff       (20)      748 2022-06-15 11:57:00.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkdirectionsrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      633 2022-06-26 20:31:08.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkdirectionsresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)      627 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkdirectionstypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      834 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkdistanceformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      659 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkgeodesicpolyline.py
+-rw-r--r--   0 ronald     (501) staff       (20)      388 2022-06-25 20:13:07.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkgeojsonserialization.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6201 2022-01-02 11:04:26.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkgeometry.py
+-rw-r--r--   0 ronald     (501) staff       (20)      340 2022-06-15 11:57:00.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkhybridmapconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      515 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mklocalsearch.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1001 2022-06-25 20:16:02.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mklocalsearchcompleter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      536 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mklocalsearchrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      261 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mklocalsearchresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)      459 2022-06-15 11:57:00.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mklookaroundscenerequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      383 2022-06-15 11:57:00.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mklookaroundsnapshotter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      995 2022-06-25 20:13:38.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mklookaroundviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      421 2022-06-15 11:57:00.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmapcamera.py
+-rw-r--r--   0 ronald     (501) staff       (20)      243 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmapcamerazoomrange.py
+-rw-r--r--   0 ronald     (501) staff       (20)      315 2022-06-25 20:19:21.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmapconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1793 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmapitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      245 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmapsnapshot.py
+-rw-r--r--   0 ronald     (501) staff       (20)      500 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmapsnapshotoptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)      831 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmapsnapshotter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4294 2022-06-26 21:30:10.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmapview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      525 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmultipoint.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1016 2022-06-25 20:13:48.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkoverlay.py
+-rw-r--r--   0 ronald     (501) staff       (20)      477 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkoverlaypathrenderer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      432 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkoverlayrenderer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      740 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkpinannotationview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      241 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkplacemark.py
+-rw-r--r--   0 ronald     (501) staff       (20)      253 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkpointannotation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3355 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkpointofinterestcategory.py
+-rw-r--r--   0 ronald     (501) staff       (20)      340 2021-03-21 10:08:22.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkpointofinterestfilter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1033 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkpolygon.py
+-rw-r--r--   0 ronald     (501) staff       (20)      253 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkpolygonrenderer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      567 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkpolyline.py
+-rw-r--r--   0 ronald     (501) staff       (20)      255 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkpolylinerenderer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      233 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkshape.py
+-rw-r--r--   0 ronald     (501) staff       (20)      587 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mksnapshotoptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)      580 2022-06-25 20:19:21.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkstandardmapconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      945 2022-01-02 11:04:26.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mktileoverlay.py
+-rw-r--r--   0 ronald     (501) staff       (20)      261 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mktileoverlayrenderer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1350 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mktypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      314 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkuserlocation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      312 2021-10-18 19:38:40.000000 pyobjc-framework-MapKit-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:03.017919 pyobjc-framework-MapKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     6774 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.2/metadata/MapKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:03.049731 pyobjc-framework-MapKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   210495 2021-07-30 09:00:38.000000 pyobjc-framework-MapKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   211255 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   242721 2022-10-18 09:53:23.000000 pyobjc-framework-MapKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   137583 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   186396 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   210496 2021-03-21 10:08:23.000000 pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   136737 2020-11-30 18:45:15.000000 pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-10.9.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   210496 2021-07-30 09:00:38.000000 pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   211256 2022-02-24 08:47:16.000000 pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   242722 2022-10-18 09:53:23.000000 pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MapKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MapKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:19:03.052808 pyobjc-framework-MapKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1373 2023-05-29 10:07:46.000000 pyobjc-framework-MapKit-9.2/setup.py
```

### Comparing `pyobjc-framework-MapKit-9.1b1/LICENSE.txt` & `pyobjc-framework-MapKit-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/Lib/MapKit/__init__.py` & `pyobjc-framework-MapKit-9.2/Lib/MapKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/Lib/MapKit/_metadata.py` & `pyobjc-framework-MapKit-9.2/Lib/MapKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/Lib/pyobjc_framework_MapKit.egg-info/PKG-INFO` & `pyobjc-framework-MapKit-9.2/Lib/pyobjc_framework_MapKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MapKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MapKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MapKit
 Platform: MacOS X (>=10.9)
```

### Comparing `pyobjc-framework-MapKit-9.1b1/Lib/pyobjc_framework_MapKit.egg-info/SOURCES.txt` & `pyobjc-framework-MapKit-9.2/Lib/pyobjc_framework_MapKit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/MapKit/__init__.py
 Lib/MapKit/_metadata.py
 Lib/pyobjc_framework_MapKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_MapKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_MapKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_MapKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-MapKit-9.1b1/Modules/_MapKit.m` & `pyobjc-framework-MapKit-9.2/Modules/_MapKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/Modules/_MapKit_inlines.m` & `pyobjc-framework-MapKit-9.2/Modules/_MapKit_inlines.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/Modules/_MapKit_protocols.m` & `pyobjc-framework-MapKit-9.2/Modules/_MapKit_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-MapKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-MapKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-MapKit-9.1b1/PKG-INFO` & `pyobjc-framework-MapKit-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MapKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MapKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MapKit
 Platform: MacOS X (>=10.9)
```

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkannotation.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkannotation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkannotationview.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkannotationview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkdirections.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkdirections.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkdirectionsrequest.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkdirectionsrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkdirectionsresponse.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkdirectionsresponse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkdirectionstypes.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkdirectionstypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkdistanceformatter.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkdistanceformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkgeodesicpolyline.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkgeodesicpolyline.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkgeometry.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkgeometry.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mklocalsearch.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mklocalsearch.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mklocalsearchcompleter.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mklocalsearchcompleter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mklocalsearchrequest.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mklocalsearchrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mklookaroundviewcontroller.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mklookaroundviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmapitem.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmapitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmapsnapshotter.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmapsnapshotter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmapview.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmapview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkmultipoint.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkmultipoint.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkoverlay.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkoverlay.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkpinannotationview.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkpinannotationview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkpointofinterestcategory.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkpointofinterestcategory.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkpolygon.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkpolygon.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkpolyline.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkpolyline.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mksnapshotoptions.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mksnapshotoptions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mkstandardmapconfiguration.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mkstandardmapconfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mktileoverlay.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mktileoverlay.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/PyObjCTest/test_mktypes.py` & `pyobjc-framework-MapKit-9.2/PyObjCTest/test_mktypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/metadata/MapKit.fwinfo` & `pyobjc-framework-MapKit-9.2/metadata/MapKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-MapKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-MapKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-MapKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-10.9.fwinfo` & `pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-10.9.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-MapKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MapKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MapKit-9.1b1/setup.py` & `pyobjc-framework-MapKit-9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 Wrappers for the "MapKit" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
-
 import os
+import sys
+
+sys.path.insert(0, os.path.dirname(__file__))
+
 
-from pyobjc_setup import Extension, setup
+from pyobjc_setup import Extension, setup  # noqa: E402
 
-VERSION = "9.1b1"
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-MapKit",
     description="Wrappers for the framework MapKit on macOS",
     min_os_level="10.9",
     packages=["MapKit"],
     ext_modules=[
```

