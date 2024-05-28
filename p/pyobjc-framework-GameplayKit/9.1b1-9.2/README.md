# Comparing `tmp/pyobjc-framework-GameplayKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-GameplayKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-GameplayKit-9.1b1.tar", last modified: Sun Mar 26 11:25:44 2023, max compression
+gzip compressed data, was "pyobjc-framework-GameplayKit-9.2.tar", last modified: Wed Jun  7 00:16:00 2023, max compression
```

## Comparing `pyobjc-framework-GameplayKit-9.1b1.tar` & `pyobjc-framework-GameplayKit-9.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:44.465906 pyobjc-framework-GameplayKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:44.378077 pyobjc-framework-GameplayKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:44.383999 pyobjc-framework-GameplayKit-9.1b1/Lib/GameplayKit/
--rw-r--r--   0 ronald     (501) staff       (20)      777 2020-11-30 18:45:15.000000 pyobjc-framework-GameplayKit-9.1b1/Lib/GameplayKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    21289 2022-10-21 10:39:42.000000 pyobjc-framework-GameplayKit-9.1b1/Lib/GameplayKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:44.388201 pyobjc-framework-GameplayKit-9.1b1/Lib/pyobjc_framework_GameplayKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2116 2023-03-26 11:25:44.000000 pyobjc-framework-GameplayKit-9.1b1/Lib/pyobjc_framework_GameplayKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1458 2023-03-26 11:25:44.000000 pyobjc-framework-GameplayKit-9.1b1/Lib/pyobjc_framework_GameplayKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:25:44.000000 pyobjc-framework-GameplayKit-9.1b1/Lib/pyobjc_framework_GameplayKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:45.000000 pyobjc-framework-GameplayKit-9.1b1/Lib/pyobjc_framework_GameplayKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       83 2023-03-26 11:25:44.000000 pyobjc-framework-GameplayKit-9.1b1/Lib/pyobjc_framework_GameplayKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       12 2023-03-26 11:25:44.000000 pyobjc-framework-GameplayKit-9.1b1/Lib/pyobjc_framework_GameplayKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-GameplayKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-GameplayKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:44.390778 pyobjc-framework-GameplayKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      829 2021-10-18 19:38:40.000000 pyobjc-framework-GameplayKit-9.1b1/Modules/_GameplayKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      659 2020-11-30 18:45:15.000000 pyobjc-framework-GameplayKit-9.1b1/Modules/_GameplayKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-GameplayKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-GameplayKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1905 2023-03-26 11:25:44.465075 pyobjc-framework-GameplayKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:44.446647 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      206 2022-04-11 08:03:15.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gameplaykit.py
--rw-r--r--   0 ronald     (501) staff       (20)     1340 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkagent.py
--rw-r--r--   0 ronald     (501) staff       (20)      250 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkdecisiontree.py
--rw-r--r--   0 ronald     (501) staff       (20)     1468 2022-06-25 09:13:24.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkgamemodel.py
--rw-r--r--   0 ronald     (501) staff       (20)      240 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkgoal.py
--rw-r--r--   0 ronald     (501) staff       (20)      241 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkgraph.py
--rw-r--r--   0 ronald     (501) staff       (20)     1852 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkgraphnode.py
--rw-r--r--   0 ronald     (501) staff       (20)     1844 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkgridgraph.py
--rw-r--r--   0 ronald     (501) staff       (20)     2214 2022-10-18 09:53:23.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkmeshgraph.py
--rw-r--r--   0 ronald     (501) staff       (20)      750 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gknoise.py
--rw-r--r--   0 ronald     (501) staff       (20)     1711 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gknoisemap.py
--rw-r--r--   0 ronald     (501) staff       (20)      298 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gknoisesource.py
--rw-r--r--   0 ronald     (501) staff       (20)     1560 2022-10-18 09:53:23.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkobstacle.py
--rw-r--r--   0 ronald     (501) staff       (20)      248 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkobstaclegraph.py
--rw-r--r--   0 ronald     (501) staff       (20)     1171 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkoctree.py
--rw-r--r--   0 ronald     (501) staff       (20)     2891 2022-10-20 19:28:19.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkpath.py
--rw-r--r--   0 ronald     (501) staff       (20)      666 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkprimitives.py
--rw-r--r--   0 ronald     (501) staff       (20)     1345 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkquadtree.py
--rw-r--r--   0 ronald     (501) staff       (20)     1010 2022-06-25 09:13:26.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkrandomsource.py
--rw-r--r--   0 ronald     (501) staff       (20)     1633 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkrtree.py
--rw-r--r--   0 ronald     (501) staff       (20)      551 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkrulesystem.py
--rw-r--r--   0 ronald     (501) staff       (20)      195 2022-06-25 20:07:31.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkscene.py
--rw-r--r--   0 ronald     (501) staff       (20)      193 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkstate.py
--rw-r--r--   0 ronald     (501) staff       (20)      276 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkstatemachine.py
--rw-r--r--   0 ronald     (501) staff       (20)      194 2022-06-25 20:11:16.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkstrategist.py
--rw-r--r--   0 ronald     (501) staff       (20)      183 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkversion.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:44.449202 pyobjc-framework-GameplayKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2527 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.1b1/metadata/GameplayKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       38 2020-11-30 18:45:15.000000 pyobjc-framework-GameplayKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:44.462056 pyobjc-framework-GameplayKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   163015 2022-10-21 10:40:12.000000 pyobjc-framework-GameplayKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   163016 2022-10-21 10:40:12.000000 pyobjc-framework-GameplayKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-GameplayKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:25:44.466032 pyobjc-framework-GameplayKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1229 2023-03-25 14:20:31.000000 pyobjc-framework-GameplayKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:00.348791 pyobjc-framework-GameplayKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:00.306290 pyobjc-framework-GameplayKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:00.315431 pyobjc-framework-GameplayKit-9.2/Lib/GameplayKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      777 2020-11-30 18:45:15.000000 pyobjc-framework-GameplayKit-9.2/Lib/GameplayKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    21289 2022-10-21 10:39:42.000000 pyobjc-framework-GameplayKit-9.2/Lib/GameplayKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:00.320353 pyobjc-framework-GameplayKit-9.2/Lib/pyobjc_framework_GameplayKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2114 2023-06-07 00:16:00.000000 pyobjc-framework-GameplayKit-9.2/Lib/pyobjc_framework_GameplayKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1473 2023-06-07 00:16:00.000000 pyobjc-framework-GameplayKit-9.2/Lib/pyobjc_framework_GameplayKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:16:00.000000 pyobjc-framework-GameplayKit-9.2/Lib/pyobjc_framework_GameplayKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:45.000000 pyobjc-framework-GameplayKit-9.2/Lib/pyobjc_framework_GameplayKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       77 2023-06-07 00:16:00.000000 pyobjc-framework-GameplayKit-9.2/Lib/pyobjc_framework_GameplayKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       12 2023-06-07 00:16:00.000000 pyobjc-framework-GameplayKit-9.2/Lib/pyobjc_framework_GameplayKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-GameplayKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-GameplayKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:00.323715 pyobjc-framework-GameplayKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      829 2021-10-18 19:38:40.000000 pyobjc-framework-GameplayKit-9.2/Modules/_GameplayKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      699 2023-05-04 11:00:07.000000 pyobjc-framework-GameplayKit-9.2/Modules/_GameplayKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-GameplayKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-GameplayKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1903 2023-06-07 00:16:00.348379 pyobjc-framework-GameplayKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:00.339805 pyobjc-framework-GameplayKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      206 2022-04-11 08:03:15.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gameplaykit.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1381 2023-05-04 11:00:07.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkagent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      250 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkdecisiontree.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1468 2022-06-25 09:13:24.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkgamemodel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      240 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkgoal.py
+-rw-r--r--   0 ronald     (501) staff       (20)      241 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkgraph.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1927 2023-05-04 11:00:07.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkgraphnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1844 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkgridgraph.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2255 2023-05-04 11:00:07.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkmeshgraph.py
+-rw-r--r--   0 ronald     (501) staff       (20)      791 2023-05-04 11:00:07.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gknoise.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1752 2023-05-04 11:00:07.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gknoisemap.py
+-rw-r--r--   0 ronald     (501) staff       (20)      339 2023-05-04 11:00:07.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gknoisesource.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1634 2023-05-04 11:00:07.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkobstacle.py
+-rw-r--r--   0 ronald     (501) staff       (20)      248 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkobstaclegraph.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1212 2023-05-04 11:00:07.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkoctree.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2891 2022-10-20 19:28:19.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkpath.py
+-rw-r--r--   0 ronald     (501) staff       (20)      666 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkprimitives.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1386 2023-05-04 11:00:07.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkquadtree.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1010 2022-06-25 09:13:26.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkrandomsource.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1674 2023-05-04 11:00:07.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkrtree.py
+-rw-r--r--   0 ronald     (501) staff       (20)      551 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkrulesystem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      238 2023-05-04 11:00:07.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkscene.py
+-rw-r--r--   0 ronald     (501) staff       (20)      193 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkstate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      276 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkstatemachine.py
+-rw-r--r--   0 ronald     (501) staff       (20)      194 2022-06-25 20:11:16.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkstrategist.py
+-rw-r--r--   0 ronald     (501) staff       (20)      183 2021-03-21 10:08:22.000000 pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkversion.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:00.341177 pyobjc-framework-GameplayKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2527 2022-10-20 21:08:30.000000 pyobjc-framework-GameplayKit-9.2/metadata/GameplayKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2020-11-30 18:45:15.000000 pyobjc-framework-GameplayKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:00.346352 pyobjc-framework-GameplayKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   163015 2022-10-21 10:40:12.000000 pyobjc-framework-GameplayKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   163016 2022-10-21 10:40:12.000000 pyobjc-framework-GameplayKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-GameplayKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-GameplayKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:16:00.348900 pyobjc-framework-GameplayKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1300 2023-05-29 10:07:46.000000 pyobjc-framework-GameplayKit-9.2/setup.py
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/Lib/GameplayKit/__init__.py` & `pyobjc-framework-GameplayKit-9.2/Lib/GameplayKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/Lib/GameplayKit/_metadata.py` & `pyobjc-framework-GameplayKit-9.2/Lib/GameplayKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/Lib/pyobjc_framework_GameplayKit.egg-info/PKG-INFO` & `pyobjc-framework-GameplayKit-9.2/Lib/pyobjc_framework_GameplayKit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-GameplayKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework GameplayKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,GameplayKit
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/Lib/pyobjc_framework_GameplayKit.egg-info/SOURCES.txt` & `pyobjc-framework-GameplayKit-9.2/Lib/pyobjc_framework_GameplayKit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/GameplayKit/__init__.py
 Lib/GameplayKit/_metadata.py
 Lib/pyobjc_framework_GameplayKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_GameplayKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_GameplayKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_GameplayKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/License.txt` & `pyobjc-framework-GameplayKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/Modules/_GameplayKit.m` & `pyobjc-framework-GameplayKit-9.2/Modules/_GameplayKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-GameplayKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-GameplayKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PKG-INFO` & `pyobjc-framework-GameplayKit-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-GameplayKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework GameplayKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,GameplayKit
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkagent.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkagent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_os_level
 
 import GameplayKit
 
 from objc import simd
 
 
 class TestGKAgent(TestCase):
     def testProtocols(self):
         self.assertProtocolExists("GKAgentDelegate")
 
+    @min_os_level("10.12")
     def testMethods(self):
         self.assertResultIsBOOL(GameplayKit.GKAgent3D.rightHanded)
         self.assertArgIsBOOL(GameplayKit.GKAgent3D.setRightHanded_, 0)
 
         self.assertResultHasType(
             GameplayKit.GKAgent3D.rotation, simd.matrix_float3x3.__typestr__
         )
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkgamemodel.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkgamemodel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkgraphnode.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkgraphnode.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_os_level
 
 import GameplayKit
 from objc import simd
 
 
 class TestGKGraphNode(TestCase):
     def testMethods(self):
@@ -23,32 +23,34 @@
             GameplayKit.GKGraphNode2D.nodeWithPoint_, 0, simd.vector_float2.__typestr__
         )
         self.assertArgHasType(
             GameplayKit.GKGraphNode2D.initWithPoint_, 0, simd.vector_float2.__typestr__
         )
 
         self.assertResultHasType(
-            GameplayKit.GKGraphNode3D.position, simd.vector_float3.__typestr__
-        )
-        self.assertArgHasType(
-            GameplayKit.GKGraphNode3D.setPosition_, 0, simd.vector_float3.__typestr__
-        )
-        self.assertArgHasType(
-            GameplayKit.GKGraphNode3D.nodeWithPoint_, 0, simd.vector_float3.__typestr__
-        )
-        self.assertArgHasType(
-            GameplayKit.GKGraphNode3D.initWithPoint_, 0, simd.vector_float3.__typestr__
-        )
-
-        self.assertResultHasType(
             GameplayKit.GKGridGraphNode.gridPosition, simd.vector_int2.__typestr__
         )
         self.assertArgHasType(
             GameplayKit.GKGridGraphNode.nodeWithGridPosition_,
             0,
             simd.vector_int2.__typestr__,
         )
         self.assertArgHasType(
             GameplayKit.GKGridGraphNode.initWithGridPosition_,
             0,
             simd.vector_int2.__typestr__,
         )
+
+    @min_os_level("10.12")
+    def test_methods_10_12(self):
+        self.assertResultHasType(
+            GameplayKit.GKGraphNode3D.position, simd.vector_float3.__typestr__
+        )
+        self.assertArgHasType(
+            GameplayKit.GKGraphNode3D.setPosition_, 0, simd.vector_float3.__typestr__
+        )
+        self.assertArgHasType(
+            GameplayKit.GKGraphNode3D.nodeWithPoint_, 0, simd.vector_float3.__typestr__
+        )
+        self.assertArgHasType(
+            GameplayKit.GKGraphNode3D.initWithPoint_, 0, simd.vector_float3.__typestr__
+        )
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkgridgraph.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkgridgraph.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkmeshgraph.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkmeshgraph.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_os_level
 
 import GameplayKit
 from objc import simd
 
 
 class TestGKMeshGraph(TestCase):
     def test_enum_types(self):
         self.assertIsEnumType(GameplayKit.GKMeshGraphTriangulationMode)
 
     def testConstants(self):
         self.assertEqual(GameplayKit.GKMeshGraphTriangulationModeVertices, 1 << 0)
         self.assertEqual(GameplayKit.GKMeshGraphTriangulationModeCenters, 1 << 1)
         self.assertEqual(GameplayKit.GKMeshGraphTriangulationModeEdgeMidpoints, 1 << 2)
 
+    @min_os_level("10.12")
     def test_methods(self):
         self.assertArgHasType(
             GameplayKit.GKMeshGraph.graphWithBufferRadius_minCoordinate_maxCoordinate_nodeClass_,
             1,
             simd.vector_float2.__typestr__,
         )
         self.assertArgHasType(
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gknoise.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gknoise.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_os_level
 
 import GameplayKit
 
 from objc import simd
 
 
 class TestGKNoise(TestCase):
+    @min_os_level("10.12")
     def testMethods(self):
         self.assertArgIsBOOL(
             GameplayKit.GKNoise.remapValuesToTerracesWithPeaks_terracesInverted_, 1
         )
 
         self.assertArgHasType(
             GameplayKit.GKNoise.valueAtPosition_, 0, simd.vector_float2.__typestr__
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gknoisemap.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gknoisemap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_os_level
 
 import GameplayKit
 from objc import simd
 
 
 class TestGKNoiseMap(TestCase):
+    @min_os_level("10.12")
     def testMethods(self):
         self.assertResultIsBOOL(GameplayKit.GKNoiseMap.isSeamless)
         # self.assertArgIsBOOL(GameplayKit.GKNoiseMap.setSeamless_, 0)
 
         self.assertResultHasType(
             GameplayKit.GKNoiseMap.size, simd.vector_double2.__typestr__
         )
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkobstacle.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkobstacle.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_os_level
 import GameplayKit  # noqa: F401
 from objc import simd
 
 
 class TestGKObstacle(TestCase):
     def testMethods(self):
         self.assertResultHasType(
@@ -32,13 +32,15 @@
             GameplayKit.GKPolygonObstacle.initWithPoints_count_, 0, 1
         )
 
         self.assertResultHasType(
             GameplayKit.GKPolygonObstacle.vertexAtIndex_, simd.vector_float2.__typestr__
         )
 
+    @min_os_level("10.12")
+    def test_methods10_12(self):
         self.assertResultHasType(
             GameplayKit.GKSphereObstacle.position, simd.vector_float3.__typestr__
         )
         self.assertArgHasType(
             GameplayKit.GKSphereObstacle.setPosition_, 0, simd.vector_float3.__typestr__
         )
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkoctree.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkoctree.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_os_level
 import GameplayKit
 
 from objc import simd
 
 
 class TestGKOctree(TestCase):
+    @min_os_level("10.12")
     def testMethods(self):
         self.assertArgHasType(
             GameplayKit.GKOctree.octreeWithBoundingBox_minimumCellSize_,
             0,
             GameplayKit.GKBox.__typestr__,
         )
         self.assertArgHasType(
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkpath.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkpath.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkprimitives.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkprimitives.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkquadtree.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkquadtree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_os_level
 
 import GameplayKit
 from objc import simd
 
 
 class TestGKQuadtree(TestCase):
+    @min_os_level("10.12")
     def testMethods(self):
         self.assertResultHasType(
             GameplayKit.GKQuadtreeNode.quad, GameplayKit.GKQuad.__typestr__
         )
 
         self.assertArgHasType(
             GameplayKit.GKQuadtree.quadtreeWithBoundingQuad_minimumCellSize_,
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkrandomsource.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkrandomsource.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkrtree.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkrtree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_os_level
 
 import GameplayKit
 from objc import simd
 
 
 class TestGKAgent(TestCase):
     def test_enum_types(self):
@@ -10,14 +10,15 @@
 
     def testConstants(self):
         self.assertEqual(GameplayKit.GKRTreeSplitStrategyHalve, 0)
         self.assertEqual(GameplayKit.GKRTreeSplitStrategyLinear, 1)
         self.assertEqual(GameplayKit.GKRTreeSplitStrategyQuadratic, 2)
         self.assertEqual(GameplayKit.GKRTreeSplitStrategyReduceOverlap, 3)
 
+    @min_os_level("10.12")
     def test_methods(self):
         self.assertArgHasType(
             GameplayKit.GKRTree.addElement_boundingRectMin_boundingRectMax_splitStrategy_,
             1,
             simd.vector_float2.__typestr__,
         )
         self.assertArgHasType(
```

### Comparing `pyobjc-framework-GameplayKit-9.1b1/PyObjCTest/test_gkrulesystem.py` & `pyobjc-framework-GameplayKit-9.2/PyObjCTest/test_gkrulesystem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/metadata/GameplayKit.fwinfo` & `pyobjc-framework-GameplayKit-9.2/metadata/GameplayKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-GameplayKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-GameplayKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-GameplayKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameplayKit-9.1b1/setup.py` & `pyobjc-framework-GameplayKit-9.2/setup.py`

 * *Files 7% similar despite different names*

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
     name="pyobjc-framework-GameplayKit",
     description="Wrappers for the framework GameplayKit on macOS",
     min_os_level="10.11",
     packages=["GameplayKit"],
     ext_modules=[
```

