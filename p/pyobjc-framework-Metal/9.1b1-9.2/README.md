# Comparing `tmp/pyobjc-framework-Metal-9.1b1.tar.gz` & `tmp/pyobjc-framework-Metal-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Metal-9.1b1.tar", last modified: Sun Mar 26 11:29:16 2023, max compression
+gzip compressed data, was "pyobjc-framework-Metal-9.2.tar", last modified: Wed Jun  7 00:19:50 2023, max compression
```

## Comparing `pyobjc-framework-Metal-9.1b1.tar` & `pyobjc-framework-Metal-9.2.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:16.175565 pyobjc-framework-Metal-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:15.958697 pyobjc-framework-Metal-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:15.969757 pyobjc-framework-Metal-9.1b1/Lib/Metal/
--rw-r--r--   0 ronald     (501) staff       (20)      723 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.1b1/Lib/Metal/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)   186399 2023-03-25 15:03:24.000000 pyobjc-framework-Metal-9.1b1/Lib/Metal/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:15.978140 pyobjc-framework-Metal-9.1b1/Lib/pyobjc_framework_Metal.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2092 2023-03-26 11:29:15.000000 pyobjc-framework-Metal-9.1b1/Lib/pyobjc_framework_Metal.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     2840 2023-03-26 11:29:15.000000 pyobjc-framework-Metal-9.1b1/Lib/pyobjc_framework_Metal.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:29:15.000000 pyobjc-framework-Metal-9.1b1/Lib/pyobjc_framework_Metal.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:29.000000 pyobjc-framework-Metal-9.1b1/Lib/pyobjc_framework_Metal.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:29:15.000000 pyobjc-framework-Metal-9.1b1/Lib/pyobjc_framework_Metal.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        6 2023-03-26 11:29:15.000000 pyobjc-framework-Metal-9.1b1/Lib/pyobjc_framework_Metal.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Metal-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Metal-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:15.996237 pyobjc-framework-Metal-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      793 2021-10-18 19:38:40.000000 pyobjc-framework-Metal-9.1b1/Modules/_Metal.m
--rw-r--r--   0 ronald     (501) staff       (20)     2439 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.1b1/Modules/_Metal_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)     2880 2022-06-23 11:03:28.000000 pyobjc-framework-Metal-9.1b1/Modules/_Metal_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-Metal-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1881 2023-03-26 11:29:16.175114 pyobjc-framework-Metal-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:16.099550 pyobjc-framework-Metal-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      589 2020-11-30 18:45:15.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/redo.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1458 2022-10-18 09:53:24.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_MTLIOCommandQueue.py
--rw-r--r--   0 ronald     (501) staff       (20)      194 2022-04-11 08:03:15.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_metal.py
--rw-r--r--   0 ronald     (501) staff       (20)     3780 2023-03-25 13:59:58.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlaccelerationstructure.py
--rw-r--r--   0 ronald     (501) staff       (20)     4708 2022-06-25 09:16:56.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlaccelerationstructurecommandencoder.py
--rw-r--r--   0 ronald     (501) staff       (20)     1045 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlaccelerationstructuretypes.py
--rw-r--r--   0 ronald     (501) staff       (20)    10514 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlargument.py
--rw-r--r--   0 ronald     (501) staff       (20)     8043 2022-06-25 09:16:01.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlargumentencoder.py
--rw-r--r--   0 ronald     (501) staff       (20)     2469 2022-06-25 20:13:43.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlbinaryarchive.py
--rw-r--r--   0 ronald     (501) staff       (20)    22294 2022-06-25 09:17:01.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlblitcommandencoder.py
--rw-r--r--   0 ronald     (501) staff       (20)      259 2021-04-09 10:15:21.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlblitpass.py
--rw-r--r--   0 ronald     (501) staff       (20)     1419 2022-06-25 09:16:41.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlbuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1119 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcapturemanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      237 2022-06-25 20:12:36.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcapturescope.py
--rw-r--r--   0 ronald     (501) staff       (20)     5118 2022-06-25 09:16:38.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcommandbuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)      780 2022-06-25 20:14:15.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcommandencoder.py
--rw-r--r--   0 ronald     (501) staff       (20)    13812 2022-06-25 09:16:17.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcomputecommandencoder.py
--rw-r--r--   0 ronald     (501) staff       (20)     1877 2022-06-25 09:15:37.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcomputepipeline.py
--rw-r--r--   0 ronald     (501) staff       (20)     3908 2022-06-25 09:16:27.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcounters.py
--rw-r--r--   0 ronald     (501) staff       (20)     1729 2022-06-25 20:16:13.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtldepthstencil.py
--rw-r--r--   0 ronald     (501) staff       (20)    35289 2023-03-25 15:03:24.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtldevice.py
--rw-r--r--   0 ronald     (501) staff       (20)     1050 2022-06-25 09:16:54.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtldrawable.py
--rw-r--r--   0 ronald     (501) staff       (20)     1172 2022-06-25 20:07:42.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtldynamiclibrary.py
--rw-r--r--   0 ronald     (501) staff       (20)      865 2022-06-25 09:16:14.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      223 2022-06-25 20:13:29.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlfence.py
--rw-r--r--   0 ronald     (501) staff       (20)      351 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlfunctiondescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      486 2022-06-25 09:16:04.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlfunctionhandle.py
--rw-r--r--   0 ronald     (501) staff       (20)      990 2022-06-25 09:16:11.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlfunctionlog.py
--rw-r--r--   0 ronald     (501) staff       (20)      317 2022-06-25 20:14:43.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlfunctionstitching.py
--rw-r--r--   0 ronald     (501) staff       (20)     3931 2022-06-27 13:21:52.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlheap.py
--rw-r--r--   0 ronald     (501) staff       (20)     2869 2022-06-25 09:15:59.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlindirectcommandbuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)    12971 2022-06-25 09:16:21.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlindirectcommandencoder.py
--rw-r--r--   0 ronald     (501) staff       (20)     4182 2022-06-25 09:17:05.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlintersectionfunctiontable.py
--rw-r--r--   0 ronald     (501) staff       (20)     4813 2022-06-27 12:53:21.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtliocommandbuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)      833 2022-07-08 16:02:54.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtliocompressor.py
--rw-r--r--   0 ronald     (501) staff       (20)     6964 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtllibrary.py
--rw-r--r--   0 ronald     (501) staff       (20)     1931 2022-06-25 09:15:35.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlparallelrendercommandencoder.py
--rw-r--r--   0 ronald     (501) staff       (20)      376 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlpipeline.py
--rw-r--r--   0 ronald     (501) staff       (20)     8945 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlpixelformat.py
--rw-r--r--   0 ronald     (501) staff       (20)     4405 2022-06-25 09:15:30.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlrasterizationrate.py
--rw-r--r--   0 ronald     (501) staff       (20)    80414 2022-06-27 19:03:25.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlrendercommandencoder.py
--rw-r--r--   0 ronald     (501) staff       (20)     2719 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlrenderpass.py
--rw-r--r--   0 ronald     (501) staff       (20)     8322 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlrenderpipeline.py
--rw-r--r--   0 ronald     (501) staff       (20)     5300 2022-06-25 09:16:49.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlresource.py
--rw-r--r--   0 ronald     (501) staff       (20)     4735 2022-06-25 09:15:55.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlresourcestatecommandencoder.py
--rw-r--r--   0 ronald     (501) staff       (20)      277 2021-04-09 10:15:21.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlresourcestatepass.py
--rw-r--r--   0 ronald     (501) staff       (20)     2342 2022-06-25 20:09:47.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlsampler.py
--rw-r--r--   0 ronald     (501) staff       (20)     4390 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlstageinputoutputdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)    12546 2022-06-26 10:16:33.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtltexture.py
--rw-r--r--   0 ronald     (501) staff       (20)     2099 2022-06-23 11:03:28.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtltypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     3800 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlvertexdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)     1218 2022-06-25 09:16:52.000000 pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlvisiblefunctiontable.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:16.122644 pyobjc-framework-Metal-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    47113 2023-03-25 15:03:24.000000 pyobjc-framework-Metal-9.1b1/metadata/Metal.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       26 2020-11-30 18:45:15.000000 pyobjc-framework-Metal-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:29:16.172509 pyobjc-framework-Metal-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   554603 2021-08-01 09:17:31.000000 pyobjc-framework-Metal-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   558597 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   650634 2022-10-18 09:53:23.000000 pyobjc-framework-Metal-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   654176 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   366710 2021-06-05 10:25:38.000000 pyobjc-framework-Metal-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   501933 2021-03-21 10:08:23.000000 pyobjc-framework-Metal-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   554604 2021-08-01 09:17:32.000000 pyobjc-framework-Metal-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   558598 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   650635 2022-10-18 09:53:23.000000 pyobjc-framework-Metal-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   654177 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Metal-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:29:16.175674 pyobjc-framework-Metal-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1291 2023-03-25 14:20:31.000000 pyobjc-framework-Metal-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:50.908023 pyobjc-framework-Metal-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:50.709543 pyobjc-framework-Metal-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:50.715720 pyobjc-framework-Metal-9.2/Lib/Metal/
+-rw-r--r--   0 ronald     (501) staff       (20)      723 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.2/Lib/Metal/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)   186399 2023-03-25 15:03:24.000000 pyobjc-framework-Metal-9.2/Lib/Metal/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:50.720645 pyobjc-framework-Metal-9.2/Lib/pyobjc_framework_Metal.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2090 2023-06-07 00:19:50.000000 pyobjc-framework-Metal-9.2/Lib/pyobjc_framework_Metal.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     2855 2023-06-07 00:19:50.000000 pyobjc-framework-Metal-9.2/Lib/pyobjc_framework_Metal.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:19:50.000000 pyobjc-framework-Metal-9.2/Lib/pyobjc_framework_Metal.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:29.000000 pyobjc-framework-Metal-9.2/Lib/pyobjc_framework_Metal.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:19:50.000000 pyobjc-framework-Metal-9.2/Lib/pyobjc_framework_Metal.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        6 2023-06-07 00:19:50.000000 pyobjc-framework-Metal-9.2/Lib/pyobjc_framework_Metal.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Metal-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Metal-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:50.724242 pyobjc-framework-Metal-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      793 2021-10-18 19:38:40.000000 pyobjc-framework-Metal-9.2/Modules/_Metal.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2492 2023-05-04 11:00:07.000000 pyobjc-framework-Metal-9.2/Modules/_Metal_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2920 2023-05-04 11:00:07.000000 pyobjc-framework-Metal-9.2/Modules/_Metal_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-Metal-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1879 2023-06-07 00:19:50.907206 pyobjc-framework-Metal-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:50.845058 pyobjc-framework-Metal-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-Metal-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      589 2020-11-30 18:45:15.000000 pyobjc-framework-Metal-9.2/PyObjCTest/redo.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1458 2022-10-18 09:53:24.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_MTLIOCommandQueue.py
+-rw-r--r--   0 ronald     (501) staff       (20)      194 2022-04-11 08:03:15.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_metal.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3780 2023-03-25 13:59:58.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlaccelerationstructure.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4708 2022-06-25 09:16:56.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlaccelerationstructurecommandencoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1085 2023-05-04 11:00:07.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlaccelerationstructuretypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10514 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlargument.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8043 2022-06-25 09:16:01.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlargumentencoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2469 2022-06-25 20:13:43.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlbinaryarchive.py
+-rw-r--r--   0 ronald     (501) staff       (20)    22294 2022-06-25 09:17:01.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlblitcommandencoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      259 2021-04-09 10:15:21.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlblitpass.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1419 2022-06-25 09:16:41.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlbuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1119 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcapturemanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      237 2022-06-25 20:12:36.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcapturescope.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5118 2022-06-25 09:16:38.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcommandbuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      780 2022-06-25 20:14:15.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcommandencoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13812 2022-06-25 09:16:17.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcomputecommandencoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1935 2023-05-04 11:00:07.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcomputepipeline.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3908 2022-06-25 09:16:27.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcounters.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1729 2022-06-25 20:16:13.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtldepthstencil.py
+-rw-r--r--   0 ronald     (501) staff       (20)    35289 2023-03-25 15:03:24.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtldevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1050 2022-06-25 09:16:54.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtldrawable.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1172 2022-06-25 20:07:42.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtldynamiclibrary.py
+-rw-r--r--   0 ronald     (501) staff       (20)      865 2022-06-25 09:16:14.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      223 2022-06-25 20:13:29.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlfence.py
+-rw-r--r--   0 ronald     (501) staff       (20)      351 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlfunctiondescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      486 2022-06-25 09:16:04.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlfunctionhandle.py
+-rw-r--r--   0 ronald     (501) staff       (20)      990 2022-06-25 09:16:11.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlfunctionlog.py
+-rw-r--r--   0 ronald     (501) staff       (20)      317 2022-06-25 20:14:43.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlfunctionstitching.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3931 2022-06-27 13:21:52.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlheap.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2869 2022-06-25 09:15:59.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlindirectcommandbuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12971 2022-06-25 09:16:21.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlindirectcommandencoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4182 2022-06-25 09:17:05.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlintersectionfunctiontable.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4813 2022-06-27 12:53:21.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtliocommandbuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      833 2022-07-08 16:02:54.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtliocompressor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6964 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtllibrary.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1931 2022-06-25 09:15:35.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlparallelrendercommandencoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      376 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlpipeline.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8945 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlpixelformat.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4405 2022-06-25 09:15:30.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlrasterizationrate.py
+-rw-r--r--   0 ronald     (501) staff       (20)    80414 2022-06-27 19:03:25.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlrendercommandencoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2719 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlrenderpass.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8322 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlrenderpipeline.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5300 2022-06-25 09:16:49.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlresource.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4735 2022-06-25 09:15:55.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlresourcestatecommandencoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      277 2021-04-09 10:15:21.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlresourcestatepass.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2342 2022-06-25 20:09:47.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlsampler.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4390 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlstageinputoutputdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12546 2022-06-26 10:16:33.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtltexture.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2162 2023-05-04 11:00:07.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtltypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3800 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlvertexdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1218 2022-06-25 09:16:52.000000 pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlvisiblefunctiontable.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:50.848378 pyobjc-framework-Metal-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    47113 2023-03-25 15:03:24.000000 pyobjc-framework-Metal-9.2/metadata/Metal.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       26 2020-11-30 18:45:15.000000 pyobjc-framework-Metal-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:19:50.902245 pyobjc-framework-Metal-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   554603 2021-08-01 09:17:31.000000 pyobjc-framework-Metal-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   558597 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   650634 2022-10-18 09:53:23.000000 pyobjc-framework-Metal-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   654176 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   366710 2021-06-05 10:25:38.000000 pyobjc-framework-Metal-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   501933 2021-03-21 10:08:23.000000 pyobjc-framework-Metal-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   554604 2021-08-01 09:17:32.000000 pyobjc-framework-Metal-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   558598 2022-02-24 08:47:16.000000 pyobjc-framework-Metal-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   650635 2022-10-18 09:53:23.000000 pyobjc-framework-Metal-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   654177 2023-02-19 10:50:35.000000 pyobjc-framework-Metal-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Metal-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Metal-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:19:50.908132 pyobjc-framework-Metal-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1361 2023-05-29 10:07:46.000000 pyobjc-framework-Metal-9.2/setup.py
```

### Comparing `pyobjc-framework-Metal-9.1b1/Lib/Metal/__init__.py` & `pyobjc-framework-Metal-9.2/Lib/Metal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/Lib/Metal/_metadata.py` & `pyobjc-framework-Metal-9.2/Lib/Metal/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/Lib/pyobjc_framework_Metal.egg-info/PKG-INFO` & `pyobjc-framework-Metal-9.2/Lib/pyobjc_framework_Metal.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Metal
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Metal on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Metal
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-Metal-9.1b1/Lib/pyobjc_framework_Metal.egg-info/SOURCES.txt` & `pyobjc-framework-Metal-9.2/Lib/pyobjc_framework_Metal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/Metal/__init__.py
 Lib/Metal/_metadata.py
 Lib/pyobjc_framework_Metal.egg-info/PKG-INFO
 Lib/pyobjc_framework_Metal.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Metal.egg-info/dependency_links.txt
 Lib/pyobjc_framework_Metal.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-Metal-9.1b1/License.txt` & `pyobjc-framework-Metal-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/Modules/_Metal.m` & `pyobjc-framework-Metal-9.2/Modules/_Metal.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/Modules/_Metal_inlines.m` & `pyobjc-framework-Metal-9.2/Modules/_Metal_inlines.m`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 /*
  * The definitions below can cause warnings when using
  * -Wunguarded-availability, but those warnings are harmless
  * because the functions are inline functions and hence will
  * be available on all macOS versions once compiled.
  */
 #pragma clang diagnostic push
+#pragma clang diagnostic ignored "-Wunknown-pragmas"
 #pragma clang diagnostic ignored "-Wunguarded-availability"
 
 static PyObjC_function_map function_map[] = {
     {"MTLOriginMake", (PyObjC_Function_Pointer)&MTLOriginMake},
     {"MTLSizeMake", (PyObjC_Function_Pointer)&MTLSizeMake},
     {"MTLRegionMake1D", (PyObjC_Function_Pointer)&MTLRegionMake1D},
     {"MTLRegionMake2D", (PyObjC_Function_Pointer)&MTLRegionMake2D},
```

### Comparing `pyobjc-framework-Metal-9.1b1/Modules/_Metal_protocols.m` & `pyobjc-framework-Metal-9.2/Modules/_Metal_protocols.m`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 {
     PyObject* p __attribute__((__unused__));
 #if 0
     p = PyObjC_IdToPython(@protocol(MTKViewDelegate));
     Py_XDECREF(p);
 #endif
 
-#if PyObjC_BUILD_RELEASE >= 1013
-    p = PyObjC_IdToPython(@protocol(MTLArgumentEncoder));
-    Py_XDECREF(p);
+#if PyObjC_BUILD_RELEASE >= 1011
     p = PyObjC_IdToPython(@protocol(MTLRenderCommandEncoder));
     Py_XDECREF(p);
-    p = PyObjC_IdToPython(@protocol(MTLFence));
+    p = PyObjC_IdToPython(@protocol(MTLComputeCommandEncoder));
     Py_XDECREF(p);
     p = PyObjC_IdToPython(@protocol(MTLBlitCommandEncoder));
     Py_XDECREF(p);
-    p = PyObjC_IdToPython(@protocol(MTLCaptureScope));
+#endif
+#if PyObjC_BUILD_RELEASE >= 1013
+    p = PyObjC_IdToPython(@protocol(MTLArgumentEncoder));
     Py_XDECREF(p);
-    p = PyObjC_IdToPython(@protocol(MTLComputeCommandEncoder));
+    p = PyObjC_IdToPython(@protocol(MTLFence));
+    Py_XDECREF(p);
+    p = PyObjC_IdToPython(@protocol(MTLCaptureScope));
     Py_XDECREF(p);
 
 #endif
 
 #if PyObjC_BUILD_RELEASE >= 1015
     p = PyObjC_IdToPython(@protocol(MTLCounter));
     Py_XDECREF(p);
```

### Comparing `pyobjc-framework-Metal-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-Metal-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-Metal-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-Metal-9.1b1/PKG-INFO` & `pyobjc-framework-Metal-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Metal
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Metal on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Metal
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/redo.txt` & `pyobjc-framework-Metal-9.2/PyObjCTest/redo.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_MTLIOCommandQueue.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_MTLIOCommandQueue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlaccelerationstructure.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlaccelerationstructure.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlaccelerationstructurecommandencoder.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlaccelerationstructurecommandencoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlaccelerationstructuretypes.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlaccelerationstructuretypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import Metal
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_os_level
 
 
 class TestMTLAccelerationStructureTypes(TestCase):
     def test_structs(self):
         v = Metal.MTLPackedFloat3()
         self.assertEqual(v.elements, None)
 
@@ -19,11 +19,12 @@
         v = Metal.MTLAccelerationStructureInstanceDescriptor()
         self.assertIsInstance(v.transformationMatrix, Metal.MTLPackedFloat4x3)
         self.assertIsInstance(v.options, int)
         self.assertIsInstance(v.mask, int)
         self.assertIsInstance(v.intersectionFunctionTableOffset, int)
         self.assertIsInstance(v.accelerationStructureIndex, int)
 
+    @min_os_level("12.0")
     def test_functions(self):
         v = Metal.MTLPackedFloat3Make(1, 2, 3)
         self.assertIsInstance(v, Metal.MTLPackedFloat3)
         self.assertEqual(v, [(1.0, 2.0, 3.0)])
```

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlargument.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlargument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlargumentencoder.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlargumentencoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlbinaryarchive.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlbinaryarchive.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlblitcommandencoder.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlblitcommandencoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlbuffer.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlbuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcapturemanager.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcapturemanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcommandbuffer.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcommandbuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcommandencoder.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcommandencoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcomputecommandencoder.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcomputecommandencoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcomputepipeline.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcomputepipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         self.assertArgIsBOOL(
             Metal.MTLComputePipelineDescriptor.alloc()
             .init()
             .setThreadGroupSizeIsMultipleOfThreadExecutionWidth_,
             0,
         )
 
+    @min_os_level("11.0")
+    def test_methods11_0(self):
         self.assertResultIsBOOL(
             Metal.MTLComputePipelineDescriptor.alloc()
             .init()
             .supportIndirectCommandBuffers
         )
 
     def test_methods(self):
```

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlcounters.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlcounters.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtldepthstencil.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtldepthstencil.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtldevice.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtldevice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtldrawable.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtldrawable.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtldynamiclibrary.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtldynamiclibrary.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlevent.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlfunctionlog.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlfunctionlog.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlheap.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlheap.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlindirectcommandbuffer.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlindirectcommandbuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlindirectcommandencoder.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlindirectcommandencoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlintersectionfunctiontable.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlintersectionfunctiontable.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtliocommandbuffer.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtliocommandbuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtliocompressor.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtliocompressor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtllibrary.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtllibrary.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlparallelrendercommandencoder.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlparallelrendercommandencoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlpixelformat.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlpixelformat.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlrasterizationrate.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlrasterizationrate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlrendercommandencoder.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlrendercommandencoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlrenderpass.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlrenderpass.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlrenderpipeline.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlrenderpipeline.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlresource.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlresource.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlresourcestatecommandencoder.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlresourcestatecommandencoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlsampler.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlsampler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlstageinputoutputdescriptor.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlstageinputoutputdescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtltexture.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtltexture.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtltypes.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtltypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 
         v = Metal.MTLRegionMake2D(1, 2, 3, 4)
         self.assertIsInstance(v, Metal.MTLRegion)
 
         v = Metal.MTLRegionMake3D(1, 2, 3, 4, 5, 6)
         self.assertIsInstance(v, Metal.MTLRegion)
 
+    @min_sdk_level("10.13")
+    def test_functions10_13(self):
         v = Metal.MTLSamplePositionMake(0.5, 1.5)
         self.assertIsInstance(v, Metal.MTLSamplePosition)
         self.assertEqual(v, (0.5, 1.5))
 
     @min_sdk_level("10.15")
     def test_functions10_15(self):
         if os_level_key(os_release()) < os_level_key("10.15"):
```

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlvertexdescriptor.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlvertexdescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/PyObjCTest/test_mtlvisiblefunctiontable.py` & `pyobjc-framework-Metal-9.2/PyObjCTest/test_mtlvisiblefunctiontable.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/metadata/Metal.fwinfo` & `pyobjc-framework-Metal-9.2/metadata/Metal.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-Metal-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Metal-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-Metal-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-Metal-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-Metal-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-Metal-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-Metal-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Metal-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-Metal-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-Metal-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Metal-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Metal-9.1b1/setup.py` & `pyobjc-framework-Metal-9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 Wrappers for the "Metal" framework on macOS.
 
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
     name="pyobjc-framework-Metal",
     description="Wrappers for the framework Metal on macOS",
     min_os_level="10.11",
     packages=["Metal"],
     ext_modules=[
```

