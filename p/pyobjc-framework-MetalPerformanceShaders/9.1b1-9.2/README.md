# Comparing `tmp/pyobjc-framework-MetalPerformanceShaders-9.1b1.tar.gz` & `tmp/pyobjc-framework-MetalPerformanceShaders-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-MetalPerformanceShaders-9.1b1.tar", last modified: Sun Mar 26 11:30:01 2023, max compression
+gzip compressed data, was "pyobjc-framework-MetalPerformanceShaders-9.2.tar", last modified: Wed Jun  7 00:20:39 2023, max compression
```

## Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1.tar` & `pyobjc-framework-MetalPerformanceShaders-9.2.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:01.310377 pyobjc-framework-MetalPerformanceShaders-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:01.107348 pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:01.117609 pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/MetalPerformanceShaders/
--rw-r--r--   0 ronald     (501) staff       (20)      933 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/MetalPerformanceShaders/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    91277 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/MetalPerformanceShaders/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:01.123097 pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2164 2023-03-26 11:30:01.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     3433 2023-03-26 11:30:01.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:30:01.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:33.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:30:01.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       24 2023-03-26 11:30:01.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:01.130954 pyobjc-framework-MetalPerformanceShaders-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1159 2021-10-18 19:38:40.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Modules/_MetalPerformanceShaders.m
--rw-r--r--   0 ronald     (501) staff       (20)     1830 2022-10-18 09:53:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Modules/_MetalPerformanceShaders_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)      869 2022-03-05 09:55:08.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Modules/_MetalPerformanceShaders_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1953 2023-03-26 11:30:01.308969 pyobjc-framework-MetalPerformanceShaders-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:01.255689 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1117 2022-04-11 08:03:15.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_metalperformanceshaders.py
--rw-r--r--   0 ronald     (501) staff       (20)      553 2022-06-25 09:17:13.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpscommandbuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)     8122 2022-12-16 16:43:02.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpscoretypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     1890 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpsfunctionconstantindices.py
--rw-r--r--   0 ronald     (501) staff       (20)     3893 2022-06-25 09:17:11.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpsimage.py
--rw-r--r--   0 ronald     (501) staff       (20)     7694 2022-10-21 10:39:47.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpskerneltypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      659 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpskeyedunarchiver.py
--rw-r--r--   0 ronald     (501) staff       (20)     2610 2022-10-18 09:53:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpsndarray.py
--rw-r--r--   0 ronald     (501) staff       (20)     1517 2022-03-05 09:55:08.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpsstate.py
--rw-r--r--   0 ronald     (501) staff       (20)     1522 2021-07-30 09:00:38.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimageconvolution.py
--rw-r--r--   0 ronald     (501) staff       (20)     3819 2022-10-20 21:08:30.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimagehistogram.py
--rw-r--r--   0 ronald     (501) staff       (20)     1492 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimagekernel.py
--rw-r--r--   0 ronald     (501) staff       (20)      886 2022-10-21 10:40:54.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimagekeypoint.py
--rw-r--r--   0 ronald     (501) staff       (20)      513 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimagemorphology.py
--rw-r--r--   0 ronald     (501) staff       (20)     2122 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimagethreshold.py
--rw-r--r--   0 ronald     (501) staff       (20)      390 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimagetypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     1206 2022-01-02 11:04:26.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsmatrix_mpsmatrixcombination.py
--rw-r--r--   0 ronald     (501) staff       (20)      943 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsmatrix_mpsmatrixdecomposition.py
--rw-r--r--   0 ronald     (501) staff       (20)      835 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsmatrix_mpsmatrixmultiplication.py
--rw-r--r--   0 ronald     (501) staff       (20)      534 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsmatrix_mpsmatrixrandom.py
--rw-r--r--   0 ronald     (501) staff       (20)     1366 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsmatrix_mpsmatrixsolve.py
--rw-r--r--   0 ronald     (501) staff       (20)      810 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsmatrix_mpsndarraymultiarykernel.py
--rw-r--r--   0 ronald     (501) staff       (20)      460 2022-01-02 11:04:26.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsndarray_mpsndarraytypes.py
--rw-r--r--   0 ronald     (501) staff       (20)    11885 2022-10-20 21:08:30.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnnconvolution.py
--rw-r--r--   0 ronald     (501) staff       (20)     2226 2022-06-25 09:17:24.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnngroupnormalization.py
--rw-r--r--   0 ronald     (501) staff       (20)     2233 2022-06-25 09:17:34.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnninstancenormalization.py
--rw-r--r--   0 ronald     (501) staff       (20)     2905 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnnkernel.py
--rw-r--r--   0 ronald     (501) staff       (20)     1938 2021-07-30 09:00:38.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnnloss.py
--rw-r--r--   0 ronald     (501) staff       (20)     1579 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnnmath.py
--rw-r--r--   0 ronald     (501) staff       (20)     1573 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnnneuraltypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     1703 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnntypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      482 2022-03-05 09:55:08.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnnupsampling.py
--rw-r--r--   0 ronald     (501) staff       (20)      473 2022-03-05 09:55:08.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsmatrixbatchnormalization.py
--rw-r--r--   0 ronald     (501) staff       (20)      434 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsmatrixsum.py
--rw-r--r--   0 ronald     (501) staff       (20)     5638 2022-06-25 09:17:20.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsneuralnetworktypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     3251 2022-06-25 09:17:17.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsnnbatchnormalization.py
--rw-r--r--   0 ronald     (501) staff       (20)     1818 2022-03-05 09:55:08.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsnngraph.py
--rw-r--r--   0 ronald     (501) staff       (20)    13337 2022-06-25 10:46:59.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsnngraphnodes.py
--rw-r--r--   0 ronald     (501) staff       (20)      461 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsnngridsample.py
--rw-r--r--   0 ronald     (501) staff       (20)     1683 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsnnoptimzers.py
--rw-r--r--   0 ronald     (501) staff       (20)      714 2021-07-30 09:00:38.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsnnreshape.py
--rw-r--r--   0 ronald     (501) staff       (20)      483 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsnnresize.py
--rw-r--r--   0 ronald     (501) staff       (20)     8139 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsrnnlayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     4452 2022-10-20 21:08:30.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsrayintersector_mpsaccelerationstructure.py
--rw-r--r--   0 ronald     (501) staff       (20)      492 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsrayintersector_mpsinstanceaccelerationstructure.py
--rw-r--r--   0 ronald     (501) staff       (20)      490 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsrayintersector_mpspolygonaccelerationstructure.py
--rw-r--r--   0 ronald     (501) staff       (20)     4442 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsrayintersector_mpsrayintersector.py
--rw-r--r--   0 ronald     (501) staff       (20)     5113 2022-10-21 10:39:48.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsrayintersector_mpsrayintersectortypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      465 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsrayintersector_mpssvgf.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:01.258597 pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    32620 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/MetalPerformanceShaders.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       62 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:30:01.302361 pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)  1128066 2022-10-21 10:40:12.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1128190 2022-12-16 16:43:02.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/arm64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1128210 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1128067 2022-10-21 10:40:12.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1128191 2022-12-16 16:43:02.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/x86_64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1128211 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:30:01.310482 pyobjc-framework-MetalPerformanceShaders-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1507 2023-03-25 14:20:31.000000 pyobjc-framework-MetalPerformanceShaders-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:39.067608 pyobjc-framework-MetalPerformanceShaders-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:38.931034 pyobjc-framework-MetalPerformanceShaders-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:38.936478 pyobjc-framework-MetalPerformanceShaders-9.2/Lib/MetalPerformanceShaders/
+-rw-r--r--   0 ronald     (501) staff       (20)      933 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Lib/MetalPerformanceShaders/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    91277 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Lib/MetalPerformanceShaders/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:38.943298 pyobjc-framework-MetalPerformanceShaders-9.2/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2162 2023-06-07 00:20:38.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     3448 2023-06-07 00:20:38.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:20:38.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:33.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:20:38.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       24 2023-06-07 00:20:38.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-MetalPerformanceShaders-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:38.947460 pyobjc-framework-MetalPerformanceShaders-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1159 2021-10-18 19:38:40.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Modules/_MetalPerformanceShaders.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1830 2022-10-18 09:53:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Modules/_MetalPerformanceShaders_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)      869 2022-03-05 09:55:08.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Modules/_MetalPerformanceShaders_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-MetalPerformanceShaders-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1951 2023-06-07 00:20:39.067038 pyobjc-framework-MetalPerformanceShaders-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:39.014453 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1117 2022-04-11 08:03:15.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_metalperformanceshaders.py
+-rw-r--r--   0 ronald     (501) staff       (20)      553 2022-06-25 09:17:13.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpscommandbuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8122 2022-12-16 16:43:02.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpscoretypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1890 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpsfunctionconstantindices.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3893 2022-06-25 09:17:11.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpsimage.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7694 2022-10-21 10:39:47.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpskerneltypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      659 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpskeyedunarchiver.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2610 2022-10-18 09:53:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpsndarray.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1517 2022-03-05 09:55:08.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpsstate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1522 2021-07-30 09:00:38.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimageconvolution.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3819 2022-10-20 21:08:30.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimagehistogram.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1492 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimagekernel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      886 2022-10-21 10:40:54.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimagekeypoint.py
+-rw-r--r--   0 ronald     (501) staff       (20)      513 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimagemorphology.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2122 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimagethreshold.py
+-rw-r--r--   0 ronald     (501) staff       (20)      390 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimagetypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1206 2022-01-02 11:04:26.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsmatrix_mpsmatrixcombination.py
+-rw-r--r--   0 ronald     (501) staff       (20)      943 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsmatrix_mpsmatrixdecomposition.py
+-rw-r--r--   0 ronald     (501) staff       (20)      835 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsmatrix_mpsmatrixmultiplication.py
+-rw-r--r--   0 ronald     (501) staff       (20)      534 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsmatrix_mpsmatrixrandom.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1366 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsmatrix_mpsmatrixsolve.py
+-rw-r--r--   0 ronald     (501) staff       (20)      810 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsmatrix_mpsndarraymultiarykernel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      460 2022-01-02 11:04:26.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsndarray_mpsndarraytypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11885 2022-10-20 21:08:30.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnnconvolution.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2226 2022-06-25 09:17:24.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnngroupnormalization.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2233 2022-06-25 09:17:34.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnninstancenormalization.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2905 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnnkernel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1938 2021-07-30 09:00:38.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnnloss.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1579 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnnmath.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1573 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnnneuraltypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1703 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnntypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      482 2022-03-05 09:55:08.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnnupsampling.py
+-rw-r--r--   0 ronald     (501) staff       (20)      473 2022-03-05 09:55:08.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsmatrixbatchnormalization.py
+-rw-r--r--   0 ronald     (501) staff       (20)      434 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsmatrixsum.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5638 2022-06-25 09:17:20.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsneuralnetworktypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3251 2022-06-25 09:17:17.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsnnbatchnormalization.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1818 2022-03-05 09:55:08.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsnngraph.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13337 2022-06-25 10:46:59.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsnngraphnodes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      461 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsnngridsample.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1683 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsnnoptimzers.py
+-rw-r--r--   0 ronald     (501) staff       (20)      714 2021-07-30 09:00:38.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsnnreshape.py
+-rw-r--r--   0 ronald     (501) staff       (20)      483 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsnnresize.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8139 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsrnnlayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4452 2022-10-20 21:08:30.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsrayintersector_mpsaccelerationstructure.py
+-rw-r--r--   0 ronald     (501) staff       (20)      492 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsrayintersector_mpsinstanceaccelerationstructure.py
+-rw-r--r--   0 ronald     (501) staff       (20)      490 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsrayintersector_mpspolygonaccelerationstructure.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4442 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsrayintersector_mpsrayintersector.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5113 2022-10-21 10:39:48.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsrayintersector_mpsrayintersectortypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      465 2022-02-24 08:47:16.000000 pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsrayintersector_mpssvgf.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:39.016171 pyobjc-framework-MetalPerformanceShaders-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    32620 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShaders-9.2/metadata/MetalPerformanceShaders.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       62 2021-03-21 10:08:23.000000 pyobjc-framework-MetalPerformanceShaders-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:20:39.063141 pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)  1128066 2022-10-21 10:40:12.000000 pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1128190 2022-12-16 16:43:02.000000 pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/arm64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1128210 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1128067 2022-10-21 10:40:12.000000 pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1128191 2022-12-16 16:43:02.000000 pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/x86_64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1128211 2023-02-19 10:50:35.000000 pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-MetalPerformanceShaders-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-MetalPerformanceShaders-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:20:39.067732 pyobjc-framework-MetalPerformanceShaders-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1577 2023-05-29 10:07:46.000000 pyobjc-framework-MetalPerformanceShaders-9.2/setup.py
```

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/MetalPerformanceShaders/__init__.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/Lib/MetalPerformanceShaders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/MetalPerformanceShaders/_metadata.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/Lib/MetalPerformanceShaders/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/PKG-INFO` & `pyobjc-framework-MetalPerformanceShaders-9.2/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MetalPerformanceShaders
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MetalPerformanceShaders on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MetalPerformanceShaders
 Platform: MacOS X (>=10.13)
```

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/SOURCES.txt` & `pyobjc-framework-MetalPerformanceShaders-9.2/Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/MetalPerformanceShaders/__init__.py
 Lib/MetalPerformanceShaders/_metadata.py
 Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/PKG-INFO
 Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/SOURCES.txt
 Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/dependency_links.txt
 Lib/pyobjc_framework_MetalPerformanceShaders.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/License.txt` & `pyobjc-framework-MetalPerformanceShaders-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/Modules/_MetalPerformanceShaders.m` & `pyobjc-framework-MetalPerformanceShaders-9.2/Modules/_MetalPerformanceShaders.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/Modules/_MetalPerformanceShaders_inlines.m` & `pyobjc-framework-MetalPerformanceShaders-9.2/Modules/_MetalPerformanceShaders_inlines.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/Modules/_MetalPerformanceShaders_protocols.m` & `pyobjc-framework-MetalPerformanceShaders-9.2/Modules/_MetalPerformanceShaders_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-MetalPerformanceShaders-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-MetalPerformanceShaders-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PKG-INFO` & `pyobjc-framework-MetalPerformanceShaders-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-MetalPerformanceShaders
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework MetalPerformanceShaders on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,MetalPerformanceShaders
 Platform: MacOS X (>=10.13)
```

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_metalperformanceshaders.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_metalperformanceshaders.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpscommandbuffer.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpscommandbuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpscoretypes.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpscoretypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpsfunctionconstantindices.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpsfunctionconstantindices.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpsimage.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpsimage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpskerneltypes.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpskerneltypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpskeyedunarchiver.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpskeyedunarchiver.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpsndarray.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpsndarray.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpscore_mpsstate.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpscore_mpsstate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimageconvolution.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimageconvolution.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimagehistogram.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimagehistogram.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimagekernel.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimagekernel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimagekeypoint.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimagekeypoint.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimagemorphology.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimagemorphology.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsimage_mpsimagethreshold.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsimage_mpsimagethreshold.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsmatrix_mpsmatrixcombination.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsmatrix_mpsmatrixcombination.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsmatrix_mpsmatrixdecomposition.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsmatrix_mpsmatrixdecomposition.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsmatrix_mpsmatrixmultiplication.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsmatrix_mpsmatrixmultiplication.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsmatrix_mpsmatrixrandom.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsmatrix_mpsmatrixrandom.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsmatrix_mpsmatrixsolve.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsmatrix_mpsmatrixsolve.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsmatrix_mpsndarraymultiarykernel.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsmatrix_mpsndarraymultiarykernel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnnconvolution.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnnconvolution.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnngroupnormalization.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnngroupnormalization.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnninstancenormalization.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnninstancenormalization.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnnkernel.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnnkernel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnnloss.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnnloss.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnnmath.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnnmath.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnnneuraltypes.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnnneuraltypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpscnntypes.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpscnntypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsneuralnetworktypes.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsneuralnetworktypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsnnbatchnormalization.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsnnbatchnormalization.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsnngraph.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsnngraph.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsnngraphnodes.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsnngraphnodes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsnnoptimzers.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsnnoptimzers.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsnnreshape.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsnnreshape.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsneuralnetwork_mpsrnnlayer.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsneuralnetwork_mpsrnnlayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsrayintersector_mpsaccelerationstructure.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsrayintersector_mpsaccelerationstructure.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsrayintersector_mpsrayintersector.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsrayintersector_mpsrayintersector.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/PyObjCTest/test_mpsrayintersector_mpsrayintersectortypes.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/PyObjCTest/test_mpsrayintersector_mpsrayintersectortypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/MetalPerformanceShaders.fwinfo` & `pyobjc-framework-MetalPerformanceShaders-9.2/metadata/MetalPerformanceShaders.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/arm64-13.1.fwinfo` & `pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/arm64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/x86_64-13.1.fwinfo` & `pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/x86_64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-MetalPerformanceShaders-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/pyobjc_setup.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-MetalPerformanceShaders-9.1b1/setup.py` & `pyobjc-framework-MetalPerformanceShaders-9.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 Wrappers for the "MetalPerformanceShaders" framework on macOS.
 
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
     name="pyobjc-framework-MetalPerformanceShaders",
     description="Wrappers for the framework MetalPerformanceShaders on macOS",
     min_os_level="10.13",
     packages=["MetalPerformanceShaders"],
     ext_modules=[
```

