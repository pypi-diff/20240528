# Comparing `tmp/pyobjc-framework-MetalPerformanceShadersGraph-9.1b1.tar.gz` & `tmp/pyobjc-framework-MetalPerformanceShadersGraph-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MetalPerformanceShadersGraph-9.1b1.tar", last modified: Sun Mar 26 11:30:25 2023, max compression
+gzip compressed data, was "pyobjc-framework-MetalPerformanceShadersGraph-9.2.tar", last modified: Wed Jun  7 00:20:58 2023, max compression
```

## Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1.tar` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:25.514706 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:25.394612 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:25.406995 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/MetalPerformanceShadersGraph/
--rw-r--r--   0 ronald     (501) staff       (20)      868 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/MetalPerformanceShadersGraph/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    24704 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/MetalPerformanceShadersGraph/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:25.412517 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2184 2023-03-26 11:30:25.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1627 2023-03-26 11:30:25.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:30:25.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:57.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       67 2023-03-26 11:30:25.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       29 2023-03-26 11:30:25.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1973 2023-03-26 11:30:25.505605 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:25.453885 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1078 2022-10-18 09:53:24.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_MPSGraphExecutable.py
--rw-r--r--   0 ronald     (501) staff       (20)      240 2022-04-11 08:03:15.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_metalperformanceshadersgraph.py
--rw-r--r--   0 ronald     (501) staff       (20)     2537 2022-06-25 10:38:16.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraph.py
--rw-r--r--   0 ronald     (501) staff       (20)     1802 2021-07-30 09:00:38.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphcontrolflowops.py
--rw-r--r--   0 ronald     (501) staff       (20)     3616 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphcore.py
--rw-r--r--   0 ronald     (501) staff       (20)     2846 2022-07-30 15:06:02.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphcumulativeops.py
--rw-r--r--   0 ronald     (501) staff       (20)      341 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphdevice.py
--rw-r--r--   0 ronald     (501) staff       (20)      414 2021-07-30 09:00:38.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphlossops.py
--rw-r--r--   0 ronald     (501) staff       (20)     2577 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphpoolingops.py
--rw-r--r--   0 ronald     (501) staff       (20)      972 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphrandomops.py
--rw-r--r--   0 ronald     (501) staff       (20)     4088 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphresizeops.py
--rw-r--r--   0 ronald     (501) staff       (20)     4522 2022-06-25 10:30:51.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphrnnops.py
--rw-r--r--   0 ronald     (501) staff       (20)     1758 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphsamplegridops.py
--rw-r--r--   0 ronald     (501) staff       (20)      835 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphscatterndops.py
--rw-r--r--   0 ronald     (501) staff       (20)      784 2022-10-18 09:53:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphsortops.py
--rw-r--r--   0 ronald     (501) staff       (20)      520 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphsparseops.py
--rw-r--r--   0 ronald     (501) staff       (20)     2099 2022-10-18 09:53:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphtensorshapeops.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:25.457134 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     9333 2022-06-25 10:46:04.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/MetalPerformanceShadersGraph.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       72 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:25.495298 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   201173 2022-01-02 11:04:26.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/arm64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   225255 2022-02-24 08:48:43.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   300841 2022-10-18 09:53:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   326203 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   120656 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   201174 2022-01-02 11:04:26.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/x86_64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   225256 2022-02-24 08:48:43.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   300842 2022-10-18 09:53:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   326204 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:30:25.514855 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1402 2023-03-25 14:20:31.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:58.175482 pyobjc-framework-MetalPerformanceShadersGraph-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:58.111810 pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:58.117404 pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/MetalPerformanceShadersGraph/
+-rw-r--r--   0 ronald     (501) staff       (20)      868 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/MetalPerformanceShadersGraph/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    24704 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/MetalPerformanceShadersGraph/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:58.121131 pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2182 2023-06-07 00:20:58.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1642 2023-06-07 00:20:58.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:20:58.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:57.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       63 2023-06-07 00:20:58.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       29 2023-06-07 00:20:58.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1971 2023-06-07 00:20:58.174995 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:58.147270 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1078 2022-10-18 09:53:24.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_MPSGraphExecutable.py
+-rw-r--r--   0 ronald     (501) staff       (20)      240 2022-04-11 08:03:15.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_metalperformanceshadersgraph.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2537 2022-06-25 10:38:16.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraph.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1802 2021-07-30 09:00:38.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphcontrolflowops.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3616 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphcore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2846 2022-07-30 15:06:02.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphcumulativeops.py
+-rw-r--r--   0 ronald     (501) staff       (20)      341 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphdevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)      414 2021-07-30 09:00:38.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphlossops.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2577 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphpoolingops.py
+-rw-r--r--   0 ronald     (501) staff       (20)      972 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphrandomops.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4088 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphresizeops.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4522 2022-06-25 10:30:51.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphrnnops.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1758 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphsamplegridops.py
+-rw-r--r--   0 ronald     (501) staff       (20)      835 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphscatterndops.py
+-rw-r--r--   0 ronald     (501) staff       (20)      784 2022-10-18 09:53:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphsortops.py
+-rw-r--r--   0 ronald     (501) staff       (20)      520 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphsparseops.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2099 2022-10-18 09:53:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphtensorshapeops.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:58.155217 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     9333 2022-06-25 10:46:04.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/MetalPerformanceShadersGraph.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       72 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:58.173160 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   201173 2022-01-02 11:04:26.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/arm64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   225255 2022-02-24 08:48:43.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   300841 2022-10-18 09:53:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   326203 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   120656 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   201174 2022-01-02 11:04:26.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/x86_64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   225256 2022-02-24 08:48:43.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   300842 2022-10-18 09:53:23.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   326204 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:20:58.175598 pyobjc-framework-MetalPerformanceShadersGraph-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      863 2023-05-29 10:07:46.000000 pyobjc-framework-MetalPerformanceShadersGraph-9.2/setup.py
```

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/MetalPerformanceShadersGraph/__init__.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/MetalPerformanceShadersGraph/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/MetalPerformanceShadersGraph/_metadata.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/MetalPerformanceShadersGraph/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/PKG-INFO` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MetalPerformanceShadersGraph
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MetalPerformanceShadersGraph on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MetalPerformanceShadersGraph
 Platform: MacOS X (>=10.16)
@@ -25,17 +25,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Objective C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
-Project-URL: Documentation, https://pyobjc.readthedocs.io/en/latest/
-Project-URL: Issue tracker, https://github.com/ronaldoussoren/pyobjc/issues
-Project-URL: Repository, https://github.com/ronaldoussoren/pyobjc
 
 
 Wrappers for the "MetalPerformanceShadersGraph" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
```

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/SOURCES.txt` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/MetalPerformanceShadersGraph/__init__.py
 Lib/MetalPerformanceShadersGraph/_metadata.py
 Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/PKG-INFO
 Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/SOURCES.txt
 Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/dependency_links.txt
 Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/License.txt` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PKG-INFO` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/Lib/pyobjc_framework_MetalPerformanceShadersGraph.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MetalPerformanceShadersGraph
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MetalPerformanceShadersGraph on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MetalPerformanceShadersGraph
 Platform: MacOS X (>=10.16)
@@ -25,14 +25,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Objective C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
+Project-URL: Documentation, https://pyobjc.readthedocs.io/en/latest/
+Project-URL: Issue tracker, https://github.com/ronaldoussoren/pyobjc/issues
+Project-URL: Repository, https://github.com/ronaldoussoren/pyobjc
 
 
 Wrappers for the "MetalPerformanceShadersGraph" framework on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
```

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_MPSGraphExecutable.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_MPSGraphExecutable.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraph.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraph.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphcontrolflowops.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphcontrolflowops.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphcore.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphcore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphcumulativeops.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphcumulativeops.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphpoolingops.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphpoolingops.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphrandomops.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphrandomops.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphresizeops.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphresizeops.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphrnnops.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphrnnops.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphsamplegridops.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphsamplegridops.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphscatterndops.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphscatterndops.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphsortops.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphsortops.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphsparseops.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphsparseops.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/PyObjCTest/test_mpsgraphtensorshapeops.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/PyObjCTest/test_mpsgraphtensorshapeops.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/MetalPerformanceShadersGraph.fwinfo` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/MetalPerformanceShadersGraph.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/arm64-12.1.fwinfo` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/arm64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/x86_64-12.1.fwinfo` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/x86_64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShadersGraph-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MetalPerformanceShadersGraph-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

