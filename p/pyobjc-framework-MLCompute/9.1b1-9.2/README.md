# Comparing `tmp/pyobjc-framework-MLCompute-9.1b1.tar.gz` & `tmp/pyobjc-framework-MLCompute-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MLCompute-9.1b1.tar", last modified: Sun Mar 26 11:28:22 2023, max compression
+gzip compressed data, was "pyobjc-framework-MLCompute-9.2.tar", last modified: Wed Jun  7 00:18:52 2023, max compression
```

## Comparing `pyobjc-framework-MLCompute-9.1b1.tar` & `pyobjc-framework-MLCompute-9.2.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:22.621477 pyobjc-framework-MLCompute-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:22.545652 pyobjc-framework-MLCompute-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:22.552584 pyobjc-framework-MLCompute-9.1b1/Lib/MLCompute/
--rw-r--r--   0 ronald     (501) staff       (20)      695 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/Lib/MLCompute/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    23852 2022-02-24 08:47:16.000000 pyobjc-framework-MLCompute-9.1b1/Lib/MLCompute/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:22.556127 pyobjc-framework-MLCompute-9.1b1/Lib/pyobjc_framework_MLCompute.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2108 2023-03-26 11:28:22.000000 pyobjc-framework-MLCompute-9.1b1/Lib/pyobjc_framework_MLCompute.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1555 2023-03-26 11:28:22.000000 pyobjc-framework-MLCompute-9.1b1/Lib/pyobjc_framework_MLCompute.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:28:22.000000 pyobjc-framework-MLCompute-9.1b1/Lib/pyobjc_framework_MLCompute.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:51.000000 pyobjc-framework-MLCompute-9.1b1/Lib/pyobjc_framework_MLCompute.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:28:22.000000 pyobjc-framework-MLCompute-9.1b1/Lib/pyobjc_framework_MLCompute.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:28:22.000000 pyobjc-framework-MLCompute-9.1b1/Lib/pyobjc_framework_MLCompute.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MLCompute-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1897 2023-03-26 11:28:22.621002 pyobjc-framework-MLCompute-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:22.600031 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      407 2021-08-01 07:47:38.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcadamoptimzer.py
--rw-r--r--   0 ronald     (501) staff       (20)      412 2021-07-30 09:00:38.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcadmwoptimzer.py
--rw-r--r--   0 ronald     (501) staff       (20)      367 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcconvolutiondescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      286 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcdevice.py
--rw-r--r--   0 ronald     (501) staff       (20)      473 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcembeddingdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      739 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcgraph.py
--rw-r--r--   0 ronald     (501) staff       (20)     2305 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcinferencegraph.py
--rw-r--r--   0 ronald     (501) staff       (20)      274 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlclayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2979 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlclstmdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      571 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcmatmuldescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)     1204 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcmultiheadattentiondescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcompute.py
--rw-r--r--   0 ronald     (501) staff       (20)      592 2021-08-01 07:45:23.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcoptimizer.py
--rw-r--r--   0 ronald     (501) staff       (20)      249 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcoptimizerdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      444 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcpoolingdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      371 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcrmspropoptimizer.py
--rw-r--r--   0 ronald     (501) staff       (20)      365 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcsgdoptimizer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1144 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlctensor.py
--rw-r--r--   0 ronald     (501) staff       (20)     1063 2021-04-07 11:13:21.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlctensordata.py
--rw-r--r--   0 ronald     (501) staff       (20)      213 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlctensordescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      285 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlctensorparameter.py
--rw-r--r--   0 ronald     (501) staff       (20)     3309 2021-04-07 11:16:05.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlctraininggraph.py
--rw-r--r--   0 ronald     (501) staff       (20)    11578 2022-02-24 08:47:16.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlctypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      329 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcupsamplelayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      298 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcyololossdescriptor.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:22.601828 pyobjc-framework-MLCompute-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     5828 2021-08-01 07:52:39.000000 pyobjc-framework-MLCompute-9.1b1/metadata/MLCompute.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       35 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:28:22.618477 pyobjc-framework-MLCompute-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   238038 2021-08-01 07:52:39.000000 pyobjc-framework-MLCompute-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   237404 2022-02-24 08:47:16.000000 pyobjc-framework-MLCompute-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   209266 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   238039 2021-08-01 07:52:39.000000 pyobjc-framework-MLCompute-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   237405 2022-02-24 08:47:16.000000 pyobjc-framework-MLCompute-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MLCompute-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:28:22.621585 pyobjc-framework-MLCompute-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      665 2023-03-25 14:20:31.000000 pyobjc-framework-MLCompute-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:52.554916 pyobjc-framework-MLCompute-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:52.480485 pyobjc-framework-MLCompute-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:52.489020 pyobjc-framework-MLCompute-9.2/Lib/MLCompute/
+-rw-r--r--   0 ronald     (501) staff       (20)      695 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/Lib/MLCompute/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    23852 2022-02-24 08:47:16.000000 pyobjc-framework-MLCompute-9.2/Lib/MLCompute/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:52.492543 pyobjc-framework-MLCompute-9.2/Lib/pyobjc_framework_MLCompute.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2106 2023-06-07 00:18:52.000000 pyobjc-framework-MLCompute-9.2/Lib/pyobjc_framework_MLCompute.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1570 2023-06-07 00:18:52.000000 pyobjc-framework-MLCompute-9.2/Lib/pyobjc_framework_MLCompute.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:18:52.000000 pyobjc-framework-MLCompute-9.2/Lib/pyobjc_framework_MLCompute.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:51.000000 pyobjc-framework-MLCompute-9.2/Lib/pyobjc_framework_MLCompute.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:18:52.000000 pyobjc-framework-MLCompute-9.2/Lib/pyobjc_framework_MLCompute.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:18:52.000000 pyobjc-framework-MLCompute-9.2/Lib/pyobjc_framework_MLCompute.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MLCompute-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1895 2023-06-07 00:18:52.554386 pyobjc-framework-MLCompute-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:52.532737 pyobjc-framework-MLCompute-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      407 2021-08-01 07:47:38.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcadamoptimzer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      412 2021-07-30 09:00:38.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcadmwoptimzer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      367 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcconvolutiondescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      286 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcdevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)      473 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcembeddingdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      739 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcgraph.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2305 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcinferencegraph.py
+-rw-r--r--   0 ronald     (501) staff       (20)      274 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlclayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2979 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlclstmdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      571 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcmatmuldescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1204 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcmultiheadattentiondescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcompute.py
+-rw-r--r--   0 ronald     (501) staff       (20)      592 2021-08-01 07:45:23.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcoptimizer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      249 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcoptimizerdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      444 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcpoolingdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      371 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcrmspropoptimizer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      365 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcsgdoptimizer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1144 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlctensor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1063 2021-04-07 11:13:21.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlctensordata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      213 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlctensordescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      285 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlctensorparameter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3309 2021-04-07 11:16:05.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlctraininggraph.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11578 2022-02-24 08:47:16.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlctypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      329 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcupsamplelayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      298 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcyololossdescriptor.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:52.534221 pyobjc-framework-MLCompute-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     5828 2021-08-01 07:52:39.000000 pyobjc-framework-MLCompute-9.2/metadata/MLCompute.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       35 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:18:52.542562 pyobjc-framework-MLCompute-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   238038 2021-08-01 07:52:39.000000 pyobjc-framework-MLCompute-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   237404 2022-02-24 08:47:16.000000 pyobjc-framework-MLCompute-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   209266 2021-03-21 10:08:22.000000 pyobjc-framework-MLCompute-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   238039 2021-08-01 07:52:39.000000 pyobjc-framework-MLCompute-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   237405 2022-02-24 08:47:16.000000 pyobjc-framework-MLCompute-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MLCompute-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MLCompute-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:18:52.555015 pyobjc-framework-MLCompute-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      746 2023-05-29 10:07:46.000000 pyobjc-framework-MLCompute-9.2/setup.py
```

### Comparing `pyobjc-framework-MLCompute-9.1b1/Lib/MLCompute/__init__.py` & `pyobjc-framework-MLCompute-9.2/Lib/MLCompute/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/Lib/MLCompute/_metadata.py` & `pyobjc-framework-MLCompute-9.2/Lib/MLCompute/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/Lib/pyobjc_framework_MLCompute.egg-info/PKG-INFO` & `pyobjc-framework-MLCompute-9.2/Lib/pyobjc_framework_MLCompute.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MLCompute
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MLCompute on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MLCompute
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-MLCompute-9.1b1/Lib/pyobjc_framework_MLCompute.egg-info/SOURCES.txt` & `pyobjc-framework-MLCompute-9.2/Lib/pyobjc_framework_MLCompute.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/MLCompute/__init__.py
 Lib/MLCompute/_metadata.py
 Lib/pyobjc_framework_MLCompute.egg-info/PKG-INFO
 Lib/pyobjc_framework_MLCompute.egg-info/SOURCES.txt
 Lib/pyobjc_framework_MLCompute.egg-info/dependency_links.txt
 Lib/pyobjc_framework_MLCompute.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-MLCompute-9.1b1/License.txt` & `pyobjc-framework-MLCompute-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/PKG-INFO` & `pyobjc-framework-MLCompute-9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MLCompute
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MLCompute on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MLCompute
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcgraph.py` & `pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcgraph.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcinferencegraph.py` & `pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcinferencegraph.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlclstmdescriptor.py` & `pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlclstmdescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcmatmuldescriptor.py` & `pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcmatmuldescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcmultiheadattentiondescriptor.py` & `pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcmultiheadattentiondescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlcoptimizer.py` & `pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlcoptimizer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlctensor.py` & `pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlctensor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlctensordata.py` & `pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlctensordata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlctraininggraph.py` & `pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlctraininggraph.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/PyObjCTest/test_mlctypes.py` & `pyobjc-framework-MLCompute-9.2/PyObjCTest/test_mlctypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/metadata/MLCompute.fwinfo` & `pyobjc-framework-MLCompute-9.2/metadata/MLCompute.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-MLCompute-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-MLCompute-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-MLCompute-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-MLCompute-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-MLCompute-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MLCompute-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MLCompute-9.1b1/setup.py` & `pyobjc-framework-MLCompute-9.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "MLCompute" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
+import os
+import sys
 
-from pyobjc_setup import setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-MLCompute",
     description="Wrappers for the framework MLCompute on macOS",
     min_os_level="10.16",
     packages=["MLCompute"],
     version=VERSION,
```

