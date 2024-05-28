# Comparing `tmp/pyobjc-framework-SceneKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-SceneKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SceneKit-9.1b1.tar", last modified: Sun Mar 26 11:37:35 2023, max compression
+gzip compressed data, was "pyobjc-framework-SceneKit-9.2.tar", last modified: Wed Jun  7 00:26:20 2023, max compression
```

## Comparing `pyobjc-framework-SceneKit-9.1b1.tar` & `pyobjc-framework-SceneKit-9.2.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:35.962367 pyobjc-framework-SceneKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:35.793347 pyobjc-framework-SceneKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:35.804756 pyobjc-framework-SceneKit-9.1b1/Lib/SceneKit/
--rw-r--r--   0 ronald     (501) staff       (20)     1251 2020-11-30 18:45:15.000000 pyobjc-framework-SceneKit-9.1b1/Lib/SceneKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    78936 2022-10-20 10:17:48.000000 pyobjc-framework-SceneKit-9.1b1/Lib/SceneKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:35.813119 pyobjc-framework-SceneKit-9.1b1/Lib/pyobjc_framework_SceneKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2128 2023-03-26 11:37:35.000000 pyobjc-framework-SceneKit-9.1b1/Lib/pyobjc_framework_SceneKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1689 2023-03-26 11:37:35.000000 pyobjc-framework-SceneKit-9.1b1/Lib/pyobjc_framework_SceneKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:37:35.000000 pyobjc-framework-SceneKit-9.1b1/Lib/pyobjc_framework_SceneKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:26.000000 pyobjc-framework-SceneKit-9.1b1/Lib/pyobjc_framework_SceneKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:37:35.000000 pyobjc-framework-SceneKit-9.1b1/Lib/pyobjc_framework_SceneKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:37:35.000000 pyobjc-framework-SceneKit-9.1b1/Lib/pyobjc_framework_SceneKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SceneKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SceneKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:35.834094 pyobjc-framework-SceneKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     3545 2022-10-21 10:40:04.000000 pyobjc-framework-SceneKit-9.1b1/Modules/_SceneKit.m
--rw-r--r--   0 ronald     (501) staff       (20)     2603 2021-03-21 10:08:23.000000 pyobjc-framework-SceneKit-9.1b1/Modules/_SceneKit_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)     1659 2020-11-30 18:45:15.000000 pyobjc-framework-SceneKit-9.1b1/Modules/_SceneKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-SceneKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-SceneKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1917 2023-03-26 11:37:35.961560 pyobjc-framework-SceneKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:35.932659 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scenekit.py
--rw-r--r--   0 ronald     (501) staff       (20)     5549 2022-10-21 10:39:54.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scenekittypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     1943 2022-06-25 09:24:45.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnaction.py
--rw-r--r--   0 ronald     (501) staff       (20)     3557 2022-06-25 09:24:38.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnanimation.py
--rw-r--r--   0 ronald     (501) staff       (20)      929 2021-03-21 10:08:23.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnaudiosource.py
--rw-r--r--   0 ronald     (501) staff       (20)     1737 2022-06-25 09:25:03.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnboundingvolume.py
--rw-r--r--   0 ronald     (501) staff       (20)     1546 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scncamera.py
--rw-r--r--   0 ronald     (501) staff       (20)     1302 2022-06-25 20:13:52.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scncameracontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     2998 2022-06-25 09:24:51.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnconstraint.py
--rw-r--r--   0 ronald     (501) staff       (20)     3323 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scngeometry.py
--rw-r--r--   0 ronald     (501) staff       (20)     1496 2022-10-18 09:53:23.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnhittest.py
--rw-r--r--   0 ronald     (501) staff       (20)      212 2021-03-21 10:08:23.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnjavascript.py
--rw-r--r--   0 ronald     (501) staff       (20)     4517 2022-10-18 09:53:23.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnlight.py
--rw-r--r--   0 ronald     (501) staff       (20)     2853 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnmaterial.py
--rw-r--r--   0 ronald     (501) staff       (20)      677 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnmaterialproperty.py
--rw-r--r--   0 ronald     (501) staff       (20)      584 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnmorpher.py
--rw-r--r--   0 ronald     (501) staff       (20)     7717 2022-10-20 21:08:30.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnnode.py
--rw-r--r--   0 ronald     (501) staff       (20)      675 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnparametricgeometry.py
--rw-r--r--   0 ronald     (501) staff       (20)     6554 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnparticlesystem.py
--rw-r--r--   0 ronald     (501) staff       (20)     1790 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnphysicsbody.py
--rw-r--r--   0 ronald     (501) staff       (20)     1257 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnphysicsfield.py
--rw-r--r--   0 ronald     (501) staff       (20)     1315 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnphysicsshape.py
--rw-r--r--   0 ronald     (501) staff       (20)     1512 2022-06-25 20:11:33.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnphysicsworld.py
--rw-r--r--   0 ronald     (501) staff       (20)      584 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnreferencenode.py
--rw-r--r--   0 ronald     (501) staff       (20)     2238 2022-06-25 20:13:34.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnscene.py
--rw-r--r--   0 ronald     (501) staff       (20)    10684 2022-06-25 09:24:54.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnscenerenderer.py
--rw-r--r--   0 ronald     (501) staff       (20)     5779 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnscenesource.py
--rw-r--r--   0 ronald     (501) staff       (20)     3999 2022-06-25 09:25:01.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnshadable.py
--rw-r--r--   0 ronald     (501) staff       (20)      489 2022-06-25 09:24:47.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scntechnique.py
--rw-r--r--   0 ronald     (501) staff       (20)      559 2021-03-21 10:08:23.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scntransaction.py
--rw-r--r--   0 ronald     (501) staff       (20)     3926 2022-06-25 09:24:56.000000 pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnview.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:35.935431 pyobjc-framework-SceneKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    46939 2022-10-20 21:08:30.000000 pyobjc-framework-SceneKit-9.1b1/metadata/SceneKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:15.000000 pyobjc-framework-SceneKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:37:35.945849 pyobjc-framework-SceneKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   584608 2022-10-18 09:53:23.000000 pyobjc-framework-SceneKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   584609 2022-10-18 09:53:23.000000 pyobjc-framework-SceneKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SceneKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:37:35.962482 pyobjc-framework-SceneKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1421 2023-03-25 14:20:32.000000 pyobjc-framework-SceneKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:20.807319 pyobjc-framework-SceneKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:20.752189 pyobjc-framework-SceneKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:20.757318 pyobjc-framework-SceneKit-9.2/Lib/SceneKit/
+-rw-r--r--   0 ronald     (501) staff       (20)     1251 2020-11-30 18:45:15.000000 pyobjc-framework-SceneKit-9.2/Lib/SceneKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    78936 2022-10-20 10:17:48.000000 pyobjc-framework-SceneKit-9.2/Lib/SceneKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:20.763338 pyobjc-framework-SceneKit-9.2/Lib/pyobjc_framework_SceneKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2126 2023-06-07 00:26:20.000000 pyobjc-framework-SceneKit-9.2/Lib/pyobjc_framework_SceneKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1704 2023-06-07 00:26:20.000000 pyobjc-framework-SceneKit-9.2/Lib/pyobjc_framework_SceneKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:26:20.000000 pyobjc-framework-SceneKit-9.2/Lib/pyobjc_framework_SceneKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:26.000000 pyobjc-framework-SceneKit-9.2/Lib/pyobjc_framework_SceneKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:26:20.000000 pyobjc-framework-SceneKit-9.2/Lib/pyobjc_framework_SceneKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:26:20.000000 pyobjc-framework-SceneKit-9.2/Lib/pyobjc_framework_SceneKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SceneKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SceneKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:20.767679 pyobjc-framework-SceneKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     3553 2023-05-04 11:00:07.000000 pyobjc-framework-SceneKit-9.2/Modules/_SceneKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2603 2021-03-21 10:08:23.000000 pyobjc-framework-SceneKit-9.2/Modules/_SceneKit_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1659 2020-11-30 18:45:15.000000 pyobjc-framework-SceneKit-9.2/Modules/_SceneKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-SceneKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-SceneKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1915 2023-06-07 00:26:20.806871 pyobjc-framework-SceneKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:20.799055 pyobjc-framework-SceneKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scenekit.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5528 2023-05-04 11:00:07.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scenekittypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1943 2022-06-25 09:24:45.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3557 2022-06-25 09:24:38.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnanimation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      929 2021-03-21 10:08:23.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnaudiosource.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1737 2022-06-25 09:25:03.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnboundingvolume.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1546 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scncamera.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1302 2022-06-25 20:13:52.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scncameracontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2998 2022-06-25 09:24:51.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnconstraint.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3323 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scngeometry.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1523 2023-05-04 11:00:07.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnhittest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      212 2021-03-21 10:08:23.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnjavascript.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4517 2022-10-18 09:53:23.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnlight.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2853 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnmaterial.py
+-rw-r--r--   0 ronald     (501) staff       (20)      677 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnmaterialproperty.py
+-rw-r--r--   0 ronald     (501) staff       (20)      584 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnmorpher.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7717 2022-10-20 21:08:30.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)      675 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnparametricgeometry.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6554 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnparticlesystem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1790 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnphysicsbody.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1257 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnphysicsfield.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1315 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnphysicsshape.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1512 2022-06-25 20:11:33.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnphysicsworld.py
+-rw-r--r--   0 ronald     (501) staff       (20)      584 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnreferencenode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2238 2022-06-25 20:13:34.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnscene.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10684 2022-06-25 09:24:54.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnscenerenderer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5779 2022-02-24 08:47:17.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnscenesource.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3999 2022-06-25 09:25:01.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnshadable.py
+-rw-r--r--   0 ronald     (501) staff       (20)      489 2022-06-25 09:24:47.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scntechnique.py
+-rw-r--r--   0 ronald     (501) staff       (20)      559 2021-03-21 10:08:23.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scntransaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3926 2022-06-25 09:24:56.000000 pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnview.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:20.800880 pyobjc-framework-SceneKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    46939 2022-10-20 21:08:30.000000 pyobjc-framework-SceneKit-9.2/metadata/SceneKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:15.000000 pyobjc-framework-SceneKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:26:20.804155 pyobjc-framework-SceneKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   584608 2022-10-18 09:53:23.000000 pyobjc-framework-SceneKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   584609 2022-10-18 09:53:23.000000 pyobjc-framework-SceneKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SceneKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-SceneKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:26:20.807419 pyobjc-framework-SceneKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1492 2023-05-29 10:07:47.000000 pyobjc-framework-SceneKit-9.2/setup.py
```

### Comparing `pyobjc-framework-SceneKit-9.1b1/Lib/SceneKit/__init__.py` & `pyobjc-framework-SceneKit-9.2/Lib/SceneKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/Lib/SceneKit/_metadata.py` & `pyobjc-framework-SceneKit-9.2/Lib/SceneKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/Lib/pyobjc_framework_SceneKit.egg-info/PKG-INFO` & `pyobjc-framework-SceneKit-9.2/Lib/pyobjc_framework_SceneKit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SceneKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SceneKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SceneKit
 Platform: MacOS X (>=10.7)
```

### Comparing `pyobjc-framework-SceneKit-9.1b1/Lib/pyobjc_framework_SceneKit.egg-info/SOURCES.txt` & `pyobjc-framework-SceneKit-9.2/Lib/pyobjc_framework_SceneKit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/SceneKit/__init__.py
 Lib/SceneKit/_metadata.py
 Lib/pyobjc_framework_SceneKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_SceneKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_SceneKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_SceneKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-SceneKit-9.1b1/License.txt` & `pyobjc-framework-SceneKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/Modules/_SceneKit.m` & `pyobjc-framework-SceneKit-9.2/Modules/_SceneKit.m`

 * *Files 2% similar despite different names*

```diff
@@ -69,31 +69,31 @@
 
     return PyObjC_ObjCToPython(@encode(SCNVector4), &result);
 }
 
 static PyObject*
 m_SCNMatrix4ToMat4(PyObject* module __attribute__((__unused__)), PyObject* vector)
 {
-    SCNMatrix4    arg;
-    simd_float4x4 result;
+    SCNMatrix4      arg;
+    matrix_float4x4 result;
 
     if (PyObjC_PythonToObjC(@encode(SCNMatrix4), vector, &arg) == -1) {
         return NULL;
     }
 
     result = SCNMatrix4ToMat4(arg);
 
     return PyObjC_ObjCToPython("{_simd_float4x4=[4<4f>]}", &result);
 }
 
 static PyObject*
 m_SCNMatrix4FromMat4(PyObject* module __attribute__((__unused__)), PyObject* vector)
 {
-    SCNMatrix4    result;
-    simd_float4x4 arg;
+    SCNMatrix4      result;
+    matrix_float4x4 arg;
 
     if (PyObjC_PythonToObjC("{_simd_float4x4=[4<4f>]}", vector, &arg) == -1) {
         return NULL;
     }
 
     result = SCNMatrix4FromMat4(arg);
```

### Comparing `pyobjc-framework-SceneKit-9.1b1/Modules/_SceneKit_inlines.m` & `pyobjc-framework-SceneKit-9.2/Modules/_SceneKit_inlines.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/Modules/_SceneKit_protocols.m` & `pyobjc-framework-SceneKit-9.2/Modules/_SceneKit_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-SceneKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-SceneKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-SceneKit-9.1b1/PKG-INFO` & `pyobjc-framework-SceneKit-9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SceneKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SceneKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SceneKit
 Platform: MacOS X (>=10.7)
```

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scenekittypes.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scenekittypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,14 @@
         self.assertEqual(v.m11, 1)
         self.assertEqual(v.m22, 2)
         self.assertEqual(v.m33, 3)
 
         w = SceneKit.SCNMatrix4Translate(v, 6, 7, 8)
         self.assertIsInstance(w, SceneKit.SCNMatrix4)
 
-    @expectedFailure
     def testFunctions_unsupported(self):
         # XXX
         SceneKit.SCNVector3FromGLKVector3
         SceneKit.SCNVector3ToGLKVector3
         SceneKit.SCNVector4FromGLKVector4
         SceneKit.SCNVector4ToGLKVector4
```

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnaction.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnaction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnanimation.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnanimation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnaudiosource.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnaudiosource.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnboundingvolume.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnboundingvolume.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scncamera.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scncamera.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scncameracontroller.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scncameracontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnconstraint.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnconstraint.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scngeometry.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scngeometry.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnhittest.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnhittest.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     def testConstants10_13(self):
         self.assertIsInstance(SceneKit.SCNHitTestOptionSearchMode, str)
 
     @min_os_level("10.15")
     def testConstants10_15(self):
         self.assertIsInstance(SceneKit.SCNHitTestOptionIgnoreLightArea, str)
 
+    @min_os_level("10.15")
     def test_methods(self):
         self.assertResultHasType(
             SceneKit.SCNHitTestResult.simdLocalCoordinates, simd.simd_float3.__typestr__
         )
         self.assertResultHasType(
             SceneKit.SCNHitTestResult.simdWorldCoordinates, simd.simd_float3.__typestr__
         )
```

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnlight.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnlight.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnmaterial.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnmaterial.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnmaterialproperty.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnmaterialproperty.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnmorpher.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnmorpher.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnnode.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnparametricgeometry.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnparametricgeometry.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnparticlesystem.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnparticlesystem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnphysicsbody.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnphysicsbody.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnphysicsfield.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnphysicsfield.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnphysicsshape.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnphysicsshape.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnphysicsworld.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnphysicsworld.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnreferencenode.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnreferencenode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnscene.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnscene.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnscenerenderer.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnscenerenderer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnscenesource.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnscenesource.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnshadable.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnshadable.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scntransaction.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scntransaction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/PyObjCTest/test_scnview.py` & `pyobjc-framework-SceneKit-9.2/PyObjCTest/test_scnview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/metadata/SceneKit.fwinfo` & `pyobjc-framework-SceneKit-9.2/metadata/SceneKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-SceneKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-SceneKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-SceneKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SceneKit-9.1b1/setup.py` & `pyobjc-framework-SceneKit-9.2/setup.py`

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
     name="pyobjc-framework-SceneKit",
     description="Wrappers for the framework SceneKit on macOS",
     min_os_level="10.7",
     packages=["SceneKit"],
     ext_modules=[
```

