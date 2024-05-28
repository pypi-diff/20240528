# Comparing `tmp/pyobjc-framework-SpriteKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-SpriteKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-SpriteKit-9.1b1.tar", last modified: Sun Mar 26 11:41:36 2023, max compression
+gzip compressed data, was "pyobjc-framework-SpriteKit-9.2.tar", last modified: Wed Jun  7 00:29:28 2023, max compression
```

## Comparing `pyobjc-framework-SpriteKit-9.1b1.tar` & `pyobjc-framework-SpriteKit-9.2.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:36.367912 pyobjc-framework-SpriteKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:36.259924 pyobjc-framework-SpriteKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:36.265528 pyobjc-framework-SpriteKit-9.1b1/Lib/SpriteKit/
--rw-r--r--   0 ronald     (501) staff       (20)      761 2020-11-30 18:45:15.000000 pyobjc-framework-SpriteKit-9.1b1/Lib/SpriteKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    39426 2023-02-19 10:50:35.000000 pyobjc-framework-SpriteKit-9.1b1/Lib/SpriteKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:36.299071 pyobjc-framework-SpriteKit-9.1b1/Lib/pyobjc_framework_SpriteKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2132 2023-03-26 11:41:36.000000 pyobjc-framework-SpriteKit-9.1b1/Lib/pyobjc_framework_SpriteKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1726 2023-03-26 11:41:36.000000 pyobjc-framework-SpriteKit-9.1b1/Lib/pyobjc_framework_SpriteKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:41:36.000000 pyobjc-framework-SpriteKit-9.1b1/Lib/pyobjc_framework_SpriteKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:43.000000 pyobjc-framework-SpriteKit-9.1b1/Lib/pyobjc_framework_SpriteKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:41:36.000000 pyobjc-framework-SpriteKit-9.1b1/Lib/pyobjc_framework_SpriteKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       10 2023-03-26 11:41:36.000000 pyobjc-framework-SpriteKit-9.1b1/Lib/pyobjc_framework_SpriteKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SpriteKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SpriteKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:36.308464 pyobjc-framework-SpriteKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     7131 2022-10-21 10:41:40.000000 pyobjc-framework-SpriteKit-9.1b1/Modules/_SpriteKit.m
--rw-r--r--   0 ronald     (501) staff       (20)      517 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/Modules/_SpriteKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-SpriteKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-SpriteKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1921 2023-03-26 11:41:36.367185 pyobjc-framework-SpriteKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:36.349995 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1424 2022-10-18 09:53:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sk3dnode.py
--rw-r--r--   0 ronald     (501) staff       (20)     2417 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skaction.py
--rw-r--r--   0 ronald     (501) staff       (20)     3173 2022-10-21 10:41:40.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skattribute.py
--rw-r--r--   0 ronald     (501) staff       (20)      299 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skconstraint.py
--rw-r--r--   0 ronald     (501) staff       (20)      624 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skeffectnode.py
--rw-r--r--   0 ronald     (501) staff       (20)      437 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skemitternode.py
--rw-r--r--   0 ronald     (501) staff       (20)     1720 2022-10-18 09:53:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skfieldnode.py
--rw-r--r--   0 ronald     (501) staff       (20)      588 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skkeyframesequence.py
--rw-r--r--   0 ronald     (501) staff       (20)      869 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sklabelnode.py
--rw-r--r--   0 ronald     (501) staff       (20)      298 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sklightnode.py
--rw-r--r--   0 ronald     (501) staff       (20)      347 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skmutabletexture.py
--rw-r--r--   0 ronald     (501) staff       (20)     1879 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sknode.py
--rw-r--r--   0 ronald     (501) staff       (20)     1218 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skphysicsbody.py
--rw-r--r--   0 ronald     (501) staff       (20)      505 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skphysicsjoint.py
--rw-r--r--   0 ronald     (501) staff       (20)     1374 2022-10-29 09:17:58.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skphysicsworld.py
--rw-r--r--   0 ronald     (501) staff       (20)      230 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skregion.py
--rw-r--r--   0 ronald     (501) staff       (20)     1187 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skrenderer.py
--rw-r--r--   0 ronald     (501) staff       (20)      620 2022-06-25 20:13:36.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skscene.py
--rw-r--r--   0 ronald     (501) staff       (20)      761 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skshapenode.py
--rw-r--r--   0 ronald     (501) staff       (20)      284 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skspritenode.py
--rw-r--r--   0 ronald     (501) staff       (20)     1077 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sktexture.py
--rw-r--r--   0 ronald     (501) staff       (20)      446 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sktextureatlas.py
--rw-r--r--   0 ronald     (501) staff       (20)      904 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sktiledefinition.py
--rw-r--r--   0 ronald     (501) staff       (20)     7092 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sktileset.py
--rw-r--r--   0 ronald     (501) staff       (20)      985 2022-10-21 10:41:40.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sktransformnode.py
--rw-r--r--   0 ronald     (501) staff       (20)      888 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sktransition.py
--rw-r--r--   0 ronald     (501) staff       (20)     3632 2022-10-21 10:41:40.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skuniform.py
--rw-r--r--   0 ronald     (501) staff       (20)      184 2022-06-15 11:57:00.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skversion.py
--rw-r--r--   0 ronald     (501) staff       (20)     2246 2022-06-25 09:25:32.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skview.py
--rw-r--r--   0 ronald     (501) staff       (20)     2354 2022-10-29 12:02:25.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skwarpgeometry.py
--rw-r--r--   0 ronald     (501) staff       (20)      601 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_snode_nsaccessibility.py
--rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_spritekit.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:36.353921 pyobjc-framework-SpriteKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    16324 2022-10-29 09:25:17.000000 pyobjc-framework-SpriteKit-9.1b1/metadata/SpriteKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:15.000000 pyobjc-framework-SpriteKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:41:36.364385 pyobjc-framework-SpriteKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   384072 2022-10-18 09:53:23.000000 pyobjc-framework-SpriteKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   384072 2023-02-19 10:50:35.000000 pyobjc-framework-SpriteKit-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   384073 2022-10-18 09:53:23.000000 pyobjc-framework-SpriteKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   384073 2023-02-19 10:50:35.000000 pyobjc-framework-SpriteKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SpriteKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:41:36.368289 pyobjc-framework-SpriteKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1175 2023-03-25 14:20:32.000000 pyobjc-framework-SpriteKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:28.723320 pyobjc-framework-SpriteKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:28.633900 pyobjc-framework-SpriteKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:28.650400 pyobjc-framework-SpriteKit-9.2/Lib/SpriteKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      761 2020-11-30 18:45:15.000000 pyobjc-framework-SpriteKit-9.2/Lib/SpriteKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    39426 2023-02-19 10:50:35.000000 pyobjc-framework-SpriteKit-9.2/Lib/SpriteKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:28.654631 pyobjc-framework-SpriteKit-9.2/Lib/pyobjc_framework_SpriteKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2130 2023-06-07 00:29:28.000000 pyobjc-framework-SpriteKit-9.2/Lib/pyobjc_framework_SpriteKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1741 2023-06-07 00:29:28.000000 pyobjc-framework-SpriteKit-9.2/Lib/pyobjc_framework_SpriteKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:29:28.000000 pyobjc-framework-SpriteKit-9.2/Lib/pyobjc_framework_SpriteKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:43.000000 pyobjc-framework-SpriteKit-9.2/Lib/pyobjc_framework_SpriteKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:29:28.000000 pyobjc-framework-SpriteKit-9.2/Lib/pyobjc_framework_SpriteKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       10 2023-06-07 00:29:28.000000 pyobjc-framework-SpriteKit-9.2/Lib/pyobjc_framework_SpriteKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-SpriteKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-SpriteKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:28.658508 pyobjc-framework-SpriteKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     7131 2022-10-21 10:41:40.000000 pyobjc-framework-SpriteKit-9.2/Modules/_SpriteKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)      517 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/Modules/_SpriteKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-SpriteKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-SpriteKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1919 2023-06-07 00:29:28.722926 pyobjc-framework-SpriteKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:28.703283 pyobjc-framework-SpriteKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1424 2022-10-18 09:53:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sk3dnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2417 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3173 2022-10-21 10:41:40.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skattribute.py
+-rw-r--r--   0 ronald     (501) staff       (20)      299 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skconstraint.py
+-rw-r--r--   0 ronald     (501) staff       (20)      624 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skeffectnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)      437 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skemitternode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1720 2022-10-18 09:53:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skfieldnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)      588 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skkeyframesequence.py
+-rw-r--r--   0 ronald     (501) staff       (20)      869 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sklabelnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)      298 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sklightnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)      347 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skmutabletexture.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1879 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sknode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1218 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skphysicsbody.py
+-rw-r--r--   0 ronald     (501) staff       (20)      505 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skphysicsjoint.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1374 2022-10-29 09:17:58.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skphysicsworld.py
+-rw-r--r--   0 ronald     (501) staff       (20)      230 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skregion.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1187 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skrenderer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      620 2022-06-25 20:13:36.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skscene.py
+-rw-r--r--   0 ronald     (501) staff       (20)      761 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skshapenode.py
+-rw-r--r--   0 ronald     (501) staff       (20)      284 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skspritenode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1077 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sktexture.py
+-rw-r--r--   0 ronald     (501) staff       (20)      446 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sktextureatlas.py
+-rw-r--r--   0 ronald     (501) staff       (20)      904 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sktiledefinition.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7092 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sktileset.py
+-rw-r--r--   0 ronald     (501) staff       (20)      985 2022-10-21 10:41:40.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sktransformnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)      888 2022-02-24 08:47:17.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sktransition.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3632 2022-10-21 10:41:40.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skuniform.py
+-rw-r--r--   0 ronald     (501) staff       (20)      184 2022-06-15 11:57:00.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skversion.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2246 2022-06-25 09:25:32.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2354 2022-10-29 12:02:25.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skwarpgeometry.py
+-rw-r--r--   0 ronald     (501) staff       (20)      601 2021-03-21 10:08:23.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_snode_nsaccessibility.py
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2022-04-11 08:03:15.000000 pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_spritekit.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:28.710597 pyobjc-framework-SpriteKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    16324 2022-10-29 09:25:17.000000 pyobjc-framework-SpriteKit-9.2/metadata/SpriteKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       34 2020-11-30 18:45:15.000000 pyobjc-framework-SpriteKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:29:28.720436 pyobjc-framework-SpriteKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   384072 2022-10-18 09:53:23.000000 pyobjc-framework-SpriteKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   384072 2023-02-19 10:50:35.000000 pyobjc-framework-SpriteKit-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   384073 2022-10-18 09:53:23.000000 pyobjc-framework-SpriteKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   384073 2023-02-19 10:50:35.000000 pyobjc-framework-SpriteKit-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-SpriteKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-SpriteKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:29:28.723437 pyobjc-framework-SpriteKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1246 2023-05-29 10:07:47.000000 pyobjc-framework-SpriteKit-9.2/setup.py
```

### Comparing `pyobjc-framework-SpriteKit-9.1b1/Lib/SpriteKit/__init__.py` & `pyobjc-framework-SpriteKit-9.2/Lib/SpriteKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/Lib/SpriteKit/_metadata.py` & `pyobjc-framework-SpriteKit-9.2/Lib/SpriteKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/Lib/pyobjc_framework_SpriteKit.egg-info/PKG-INFO` & `pyobjc-framework-SpriteKit-9.2/Lib/pyobjc_framework_SpriteKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SpriteKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SpriteKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SpriteKit
 Platform: MacOS X (>=10.9)
```

### Comparing `pyobjc-framework-SpriteKit-9.1b1/Lib/pyobjc_framework_SpriteKit.egg-info/SOURCES.txt` & `pyobjc-framework-SpriteKit-9.2/Lib/pyobjc_framework_SpriteKit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/SpriteKit/__init__.py
 Lib/SpriteKit/_metadata.py
 Lib/pyobjc_framework_SpriteKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_SpriteKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_SpriteKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_SpriteKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-SpriteKit-9.1b1/License.txt` & `pyobjc-framework-SpriteKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/Modules/_SpriteKit.m` & `pyobjc-framework-SpriteKit-9.2/Modules/_SpriteKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/Modules/_SpriteKit_protocols.m` & `pyobjc-framework-SpriteKit-9.2/Modules/_SpriteKit_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-SpriteKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-SpriteKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PKG-INFO` & `pyobjc-framework-SpriteKit-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-SpriteKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework SpriteKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,SpriteKit
 Platform: MacOS X (>=10.9)
```

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sk3dnode.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sk3dnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skaction.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skaction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skattribute.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skattribute.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skeffectnode.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skeffectnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skfieldnode.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skfieldnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skkeyframesequence.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skkeyframesequence.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sklabelnode.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sklabelnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sknode.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sknode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skphysicsbody.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skphysicsbody.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skphysicsworld.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skphysicsworld.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skrenderer.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skrenderer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skscene.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skscene.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skshapenode.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skshapenode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sktexture.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sktexture.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sktiledefinition.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sktiledefinition.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sktileset.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sktileset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sktransformnode.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sktransformnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_sktransition.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_sktransition.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skuniform.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skuniform.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skview.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_skwarpgeometry.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_skwarpgeometry.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/PyObjCTest/test_snode_nsaccessibility.py` & `pyobjc-framework-SpriteKit-9.2/PyObjCTest/test_snode_nsaccessibility.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/metadata/SpriteKit.fwinfo` & `pyobjc-framework-SpriteKit-9.2/metadata/SpriteKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-SpriteKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-SpriteKit-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-SpriteKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-SpriteKit-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-SpriteKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-SpriteKit-9.1b1/setup.py` & `pyobjc-framework-SpriteKit-9.2/setup.py`

 * *Files 5% similar despite different names*

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
     name="pyobjc-framework-SpriteKit",
     description="Wrappers for the framework SpriteKit on macOS",
     min_os_level="10.9",
     packages=["SpriteKit"],
     ext_modules=[
```

