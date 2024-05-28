# Comparing `tmp/pyobjc-framework-GameController-9.1b1.tar.gz` & `tmp/pyobjc-framework-GameController-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-GameController-9.1b1.tar", last modified: Sun Mar 26 11:25:09 2023, max compression
+gzip compressed data, was "pyobjc-framework-GameController-9.2.tar", last modified: Wed Jun  7 00:15:24 2023, max compression
```

## Comparing `pyobjc-framework-GameController-9.1b1.tar` & `pyobjc-framework-GameController-9.2.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:09.584087 pyobjc-framework-GameController-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:09.426041 pyobjc-framework-GameController-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:09.440205 pyobjc-framework-GameController-9.1b1/Lib/GameController/
--rw-r--r--   0 ronald     (501) staff       (20)      779 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.1b1/Lib/GameController/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    48306 2023-02-19 10:50:35.000000 pyobjc-framework-GameController-9.1b1/Lib/GameController/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:09.444201 pyobjc-framework-GameController-9.1b1/Lib/pyobjc_framework_GameController.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2143 2023-03-26 11:25:09.000000 pyobjc-framework-GameController-9.1b1/Lib/pyobjc_framework_GameController.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     2689 2023-03-26 11:25:09.000000 pyobjc-framework-GameController-9.1b1/Lib/pyobjc_framework_GameController.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:25:09.000000 pyobjc-framework-GameController-9.1b1/Lib/pyobjc_framework_GameController.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:14.000000 pyobjc-framework-GameController-9.1b1/Lib/pyobjc_framework_GameController.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:25:09.000000 pyobjc-framework-GameController-9.1b1/Lib/pyobjc_framework_GameController.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       15 2023-03-26 11:25:09.000000 pyobjc-framework-GameController-9.1b1/Lib/pyobjc_framework_GameController.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-GameController-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-GameController-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:09.447227 pyobjc-framework-GameController-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1105 2021-10-18 19:38:40.000000 pyobjc-framework-GameController-9.1b1/Modules/_GameController.m
--rw-r--r--   0 ronald     (501) staff       (20)     1860 2022-06-26 20:21:02.000000 pyobjc-framework-GameController-9.1b1/Modules/_GameController_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-GameController-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-GameController-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1932 2023-03-26 11:25:09.583725 pyobjc-framework-GameController-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:09.539025 pyobjc-framework-GameController-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      212 2022-04-11 08:03:15.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gamecontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      507 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gamepad.py
--rw-r--r--   0 ronald     (501) staff       (20)      254 2022-06-25 20:09:40.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcaxiselement.py
--rw-r--r--   0 ronald     (501) staff       (20)     1224 2022-06-25 20:14:58.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcaxisinput.py
--rw-r--r--   0 ronald     (501) staff       (20)      258 2022-06-25 20:14:28.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcbuttonelement.py
--rw-r--r--   0 ronald     (501) staff       (20)     2740 2022-10-18 09:53:23.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gccontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      576 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gccontrolleraxisinput.py
--rw-r--r--   0 ronald     (501) staff       (20)     1626 2021-07-30 09:00:38.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gccontrollerbuttoninput.py
--rw-r--r--   0 ronald     (501) staff       (20)      590 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gccontrollerdirectionpad.py
--rw-r--r--   0 ronald     (501) staff       (20)      927 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gccontrollerelement.py
--rw-r--r--   0 ronald     (501) staff       (20)     1736 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gccontrollertouchpad.py
--rw-r--r--   0 ronald     (501) staff       (20)      235 2022-06-25 20:07:03.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdevice.py
--rw-r--r--   0 ronald     (501) staff       (20)      526 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdevicebattery.py
--rw-r--r--   0 ronald     (501) staff       (20)      982 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdevicehaptics.py
--rw-r--r--   0 ronald     (501) staff       (20)     1223 2022-10-20 21:08:30.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdevicephysicalinput.py
--rw-r--r--   0 ronald     (501) staff       (20)      736 2022-06-25 09:12:32.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdevicephysicalinputstate.py
--rw-r--r--   0 ronald     (501) staff       (20)      634 2022-06-25 20:10:23.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdevicephysicalinputstatediff.py
--rw-r--r--   0 ronald     (501) staff       (20)      353 2021-04-09 10:15:21.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdirectionalgamepad.py
--rw-r--r--   0 ronald     (501) staff       (20)      270 2022-06-25 20:06:46.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdirectionpadelement.py
--rw-r--r--   0 ronald     (501) staff       (20)     2313 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdualsenseadaptivetrigger.py
--rw-r--r--   0 ronald     (501) staff       (20)      440 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gceventviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      560 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcextendedgamepad.py
--rw-r--r--   0 ronald     (501) staff       (20)     3873 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcextendedgamepadsnapshot.py
--rw-r--r--   0 ronald     (501) staff       (20)     1288 2022-01-02 11:04:26.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcgamepadsnapshot.py
--rw-r--r--   0 ronald     (501) staff       (20)     3290 2022-10-18 09:53:23.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcinputnames.py
--rw-r--r--   0 ronald     (501) staff       (20)      347 2021-07-30 09:00:38.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gckeyboard.py
--rw-r--r--   0 ronald     (501) staff       (20)      609 2021-07-30 09:00:38.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gckeyboardinput.py
--rw-r--r--   0 ronald     (501) staff       (20)     8841 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gckeycodes.py
--rw-r--r--   0 ronald     (501) staff       (20)     8705 2021-07-30 09:00:38.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gckeynames.py
--rw-r--r--   0 ronald     (501) staff       (20)     1242 2022-06-25 20:14:00.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gclinearinput.py
--rw-r--r--   0 ronald     (501) staff       (20)     1437 2021-08-14 10:34:11.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcmicrogamepad.py
--rw-r--r--   0 ronald     (501) staff       (20)     2538 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcmicrogamepadsnapshot.py
--rw-r--r--   0 ronald     (501) staff       (20)     1878 2022-01-02 11:04:26.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcmotion.py
--rw-r--r--   0 ronald     (501) staff       (20)      537 2021-07-30 09:00:38.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcmouse.py
--rw-r--r--   0 ronald     (501) staff       (20)      379 2021-07-30 09:00:38.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcmouseinput.py
--rw-r--r--   0 ronald     (501) staff       (20)      272 2022-06-25 20:13:56.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcphysicalinputelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      603 2022-06-26 20:22:18.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcphysicalinputprofile.py
--rw-r--r--   0 ronald     (501) staff       (20)     1063 2022-06-27 14:29:05.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcpressedstateinput.py
--rw-r--r--   0 ronald     (501) staff       (20)     1247 2022-06-23 11:03:28.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcproductcategories.py
--rw-r--r--   0 ronald     (501) staff       (20)      767 2022-06-27 13:50:04.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcracingwheel.py
--rw-r--r--   0 ronald     (501) staff       (20)     1176 2022-06-25 20:07:46.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcrelativeinput.py
--rw-r--r--   0 ronald     (501) staff       (20)      258 2022-06-25 20:12:40.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcswitchelement.py
--rw-r--r--   0 ronald     (501) staff       (20)     1890 2022-06-27 14:29:40.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcswitchpositioninput.py
--rw-r--r--   0 ronald     (501) staff       (20)      259 2022-06-23 11:03:28.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcsyntheticdevicekeys.py
--rw-r--r--   0 ronald     (501) staff       (20)     1178 2022-06-25 20:09:19.000000 pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gctouchedstateinput.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:09.541353 pyobjc-framework-GameController-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    21880 2022-10-20 21:08:30.000000 pyobjc-framework-GameController-9.1b1/metadata/GameController.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:15.000000 pyobjc-framework-GameController-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:09.581075 pyobjc-framework-GameController-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   112128 2022-01-02 11:04:26.000000 pyobjc-framework-GameController-9.1b1/metadata/raw/arm64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   114716 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   162154 2022-10-18 09:53:23.000000 pyobjc-framework-GameController-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   162154 2023-02-19 10:50:35.000000 pyobjc-framework-GameController-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    29763 2020-11-30 18:45:15.000000 pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    48349 2020-11-30 18:45:15.000000 pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   101354 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    25769 2020-11-30 18:45:15.000000 pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-10.9.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   112129 2022-01-02 11:04:26.000000 pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   114717 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   162155 2022-10-18 09:53:23.000000 pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   162155 2023-02-19 10:50:35.000000 pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-GameController-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:25:09.584192 pyobjc-framework-GameController-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1181 2023-03-25 14:20:31.000000 pyobjc-framework-GameController-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:24.050006 pyobjc-framework-GameController-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:23.954890 pyobjc-framework-GameController-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:23.960488 pyobjc-framework-GameController-9.2/Lib/GameController/
+-rw-r--r--   0 ronald     (501) staff       (20)      779 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.2/Lib/GameController/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    48370 2023-05-27 09:46:33.000000 pyobjc-framework-GameController-9.2/Lib/GameController/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:23.965540 pyobjc-framework-GameController-9.2/Lib/pyobjc_framework_GameController.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2141 2023-06-07 00:15:23.000000 pyobjc-framework-GameController-9.2/Lib/pyobjc_framework_GameController.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     2704 2023-06-07 00:15:23.000000 pyobjc-framework-GameController-9.2/Lib/pyobjc_framework_GameController.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:15:23.000000 pyobjc-framework-GameController-9.2/Lib/pyobjc_framework_GameController.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:14.000000 pyobjc-framework-GameController-9.2/Lib/pyobjc_framework_GameController.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:15:23.000000 pyobjc-framework-GameController-9.2/Lib/pyobjc_framework_GameController.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       15 2023-06-07 00:15:23.000000 pyobjc-framework-GameController-9.2/Lib/pyobjc_framework_GameController.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-GameController-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-GameController-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:23.968993 pyobjc-framework-GameController-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1105 2021-10-18 19:38:40.000000 pyobjc-framework-GameController-9.2/Modules/_GameController.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1860 2022-06-26 20:21:02.000000 pyobjc-framework-GameController-9.2/Modules/_GameController_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-GameController-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-GameController-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1930 2023-06-07 00:15:24.049613 pyobjc-framework-GameController-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:24.021863 pyobjc-framework-GameController-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-GameController-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      212 2022-04-11 08:03:15.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gamecontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      507 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gamepad.py
+-rw-r--r--   0 ronald     (501) staff       (20)      254 2022-06-25 20:09:40.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcaxiselement.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1224 2022-06-25 20:14:58.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcaxisinput.py
+-rw-r--r--   0 ronald     (501) staff       (20)      258 2022-06-25 20:14:28.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcbuttonelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2640 2023-05-04 11:00:07.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gccontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      576 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gccontrolleraxisinput.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1626 2021-07-30 09:00:38.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gccontrollerbuttoninput.py
+-rw-r--r--   0 ronald     (501) staff       (20)      590 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gccontrollerdirectionpad.py
+-rw-r--r--   0 ronald     (501) staff       (20)      927 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gccontrollerelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1736 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gccontrollertouchpad.py
+-rw-r--r--   0 ronald     (501) staff       (20)      235 2022-06-25 20:07:03.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)      526 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdevicebattery.py
+-rw-r--r--   0 ronald     (501) staff       (20)      982 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdevicehaptics.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1223 2022-10-20 21:08:30.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdevicephysicalinput.py
+-rw-r--r--   0 ronald     (501) staff       (20)      736 2022-06-25 09:12:32.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdevicephysicalinputstate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      634 2022-06-25 20:10:23.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdevicephysicalinputstatediff.py
+-rw-r--r--   0 ronald     (501) staff       (20)      353 2021-04-09 10:15:21.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdirectionalgamepad.py
+-rw-r--r--   0 ronald     (501) staff       (20)      270 2022-06-25 20:06:46.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdirectionpadelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2313 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdualsenseadaptivetrigger.py
+-rw-r--r--   0 ronald     (501) staff       (20)      440 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gceventviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      560 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcextendedgamepad.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3873 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcextendedgamepadsnapshot.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1288 2022-01-02 11:04:26.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcgamepadsnapshot.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3290 2022-10-18 09:53:23.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcinputnames.py
+-rw-r--r--   0 ronald     (501) staff       (20)      347 2021-07-30 09:00:38.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gckeyboard.py
+-rw-r--r--   0 ronald     (501) staff       (20)      609 2021-07-30 09:00:38.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gckeyboardinput.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8841 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gckeycodes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8705 2021-07-30 09:00:38.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gckeynames.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1242 2022-06-25 20:14:00.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gclinearinput.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1302 2023-05-04 11:00:07.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcmicrogamepad.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2490 2023-05-04 11:00:07.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcmicrogamepadsnapshot.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1878 2022-01-02 11:04:26.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcmotion.py
+-rw-r--r--   0 ronald     (501) staff       (20)      537 2021-07-30 09:00:38.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcmouse.py
+-rw-r--r--   0 ronald     (501) staff       (20)      379 2021-07-30 09:00:38.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcmouseinput.py
+-rw-r--r--   0 ronald     (501) staff       (20)      272 2022-06-25 20:13:56.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcphysicalinputelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      603 2022-06-26 20:22:18.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcphysicalinputprofile.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1063 2022-06-27 14:29:05.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcpressedstateinput.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1247 2022-06-23 11:03:28.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcproductcategories.py
+-rw-r--r--   0 ronald     (501) staff       (20)      767 2022-06-27 13:50:04.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcracingwheel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1176 2022-06-25 20:07:46.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcrelativeinput.py
+-rw-r--r--   0 ronald     (501) staff       (20)      258 2022-06-25 20:12:40.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcswitchelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1890 2022-06-27 14:29:40.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcswitchpositioninput.py
+-rw-r--r--   0 ronald     (501) staff       (20)      259 2022-06-23 11:03:28.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gcsyntheticdevicekeys.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1178 2022-06-25 20:09:19.000000 pyobjc-framework-GameController-9.2/PyObjCTest/test_gctouchedstateinput.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:24.024345 pyobjc-framework-GameController-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    21901 2023-05-27 09:46:33.000000 pyobjc-framework-GameController-9.2/metadata/GameController.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:15.000000 pyobjc-framework-GameController-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:24.048105 pyobjc-framework-GameController-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   112128 2022-01-02 11:04:26.000000 pyobjc-framework-GameController-9.2/metadata/raw/arm64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   114716 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   162154 2022-10-18 09:53:23.000000 pyobjc-framework-GameController-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   162154 2023-02-19 10:50:35.000000 pyobjc-framework-GameController-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    29763 2020-11-30 18:45:15.000000 pyobjc-framework-GameController-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    48349 2020-11-30 18:45:15.000000 pyobjc-framework-GameController-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   101354 2021-03-21 10:08:22.000000 pyobjc-framework-GameController-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    25769 2020-11-30 18:45:15.000000 pyobjc-framework-GameController-9.2/metadata/raw/x86_64-10.9.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   112129 2022-01-02 11:04:26.000000 pyobjc-framework-GameController-9.2/metadata/raw/x86_64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   114717 2022-02-24 08:47:16.000000 pyobjc-framework-GameController-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   162155 2022-10-18 09:53:23.000000 pyobjc-framework-GameController-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   162155 2023-02-19 10:50:35.000000 pyobjc-framework-GameController-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-GameController-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-GameController-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:15:24.050122 pyobjc-framework-GameController-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1252 2023-05-29 10:07:46.000000 pyobjc-framework-GameController-9.2/setup.py
```

### Comparing `pyobjc-framework-GameController-9.1b1/Lib/GameController/__init__.py` & `pyobjc-framework-GameController-9.2/Lib/GameController/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/Lib/GameController/_metadata.py` & `pyobjc-framework-GameController-9.2/Lib/GameController/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Feb 17 21:48:40 2023
+# Last update: Sat May 20 12:08:57 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -232,14 +232,16 @@
     "GCMicroGamepadSnapShotDataV100FromNSData": (
         b"Z^{_GCMicroGamepadSnapShotDataV100=SSffff}@",
         "",
         {"arguments": {0: {"type_modifier": "o"}}},
     ),
     "NSDataFromGCExtendedGamepadSnapShotDataV100": (
         b"@^{_GCExtendedGamepadSnapShotDataV100=SSffffffffffffff}",
+        "",
+        {"arguments": {0: {"type_modifier": "n"}}},
     ),
     "NSDataFromGCExtendedGamepadSnapshotData": (
         b"@^{_GCExtendedGamepadSnapshotData=SSffffffffffffffZZZ}",
         "",
         {"arguments": {0: {"type_modifier": "n"}}},
     ),
 }
```

### Comparing `pyobjc-framework-GameController-9.1b1/Lib/pyobjc_framework_GameController.egg-info/PKG-INFO` & `pyobjc-framework-GameController-9.2/Lib/pyobjc_framework_GameController.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-GameController
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework GameController on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,GameController
 Platform: MacOS X
```

### Comparing `pyobjc-framework-GameController-9.1b1/Lib/pyobjc_framework_GameController.egg-info/SOURCES.txt` & `pyobjc-framework-GameController-9.2/Lib/pyobjc_framework_GameController.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/GameController/__init__.py
 Lib/GameController/_metadata.py
 Lib/pyobjc_framework_GameController.egg-info/PKG-INFO
 Lib/pyobjc_framework_GameController.egg-info/SOURCES.txt
 Lib/pyobjc_framework_GameController.egg-info/dependency_links.txt
 Lib/pyobjc_framework_GameController.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-GameController-9.1b1/License.txt` & `pyobjc-framework-GameController-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/Modules/_GameController.m` & `pyobjc-framework-GameController-9.2/Modules/_GameController.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/Modules/_GameController_protocols.m` & `pyobjc-framework-GameController-9.2/Modules/_GameController_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-GameController-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-GameController-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-GameController-9.1b1/PKG-INFO` & `pyobjc-framework-GameController-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-GameController
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework GameController on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,GameController
 Platform: MacOS X
```

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcaxisinput.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcaxisinput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gccontroller.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gccontroller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-from PyObjCTools.TestSupport import (
-    TestCase,
-    min_os_level,
-    os_release,
-    expectedFailureIf,
-)
+from PyObjCTools.TestSupport import TestCase, min_os_level
 import objc
 import GameController
 
 
 class TestGCController(TestCase):
     def test_enum_types(self):
         self.assertIsEnumType(GameController.GCControllerPlayerIndex)
@@ -30,16 +25,15 @@
 
         self.assertArgIsBlock(
             GameController.GCController.startWirelessControllerDiscoveryWithCompletionHandler_,
             0,
             b"v",
         )
 
-    @expectedFailureIf(os_release() == "10.11")
-    @min_os_level("10.11")
+    @min_os_level("10.12")
     def testMethods10_11(self):
         self.assertResultIsBOOL(
             GameController.GCEventViewController.controllerUserInteractionEnabled
         )
         self.assertArgIsBOOL(
             GameController.GCEventViewController.setControllerUserInteractionEnabled_, 0
         )
```

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gccontrolleraxisinput.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gccontrolleraxisinput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gccontrollerbuttoninput.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gccontrollerbuttoninput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gccontrollerdirectionpad.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gccontrollerdirectionpad.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gccontrollerelement.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gccontrollerelement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gccontrollertouchpad.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gccontrollertouchpad.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdevicebattery.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdevicebattery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdevicehaptics.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdevicehaptics.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdevicephysicalinput.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdevicephysicalinput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdevicephysicalinputstate.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdevicephysicalinputstate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdevicephysicalinputstatediff.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdevicephysicalinputstatediff.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcdualsenseadaptivetrigger.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcdualsenseadaptivetrigger.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcextendedgamepad.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcextendedgamepad.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcextendedgamepadsnapshot.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcextendedgamepadsnapshot.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcgamepadsnapshot.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcgamepadsnapshot.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcinputnames.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcinputnames.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gckeyboardinput.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gckeyboardinput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gckeycodes.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gckeycodes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gckeynames.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gckeynames.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gclinearinput.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gclinearinput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcmicrogamepad.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcmicrogamepadsnapshot.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,37 +4,63 @@
     os_release,
     expectedFailureIf,
 )
 import objc
 import GameController
 
 
-class TestGCMicroGamepad(TestCase):
-    @min_os_level("12.0")
-    def test_constants12_0(self):
-        self.assertIsInstance(GameController.GCInputMicroGamepadDpad, str)
-        self.assertIsInstance(GameController.GCInputMicroGamepadButtonA, str)
-        self.assertIsInstance(GameController.GCInputMicroGamepadButtonX, str)
-        self.assertIsInstance(GameController.GCInputMicroGamepadButtonMenu, str)
+class TestGCMicroGamepadSnapshot(TestCase):
+    def test_enum_types(self):
+        self.assertIsEnumType(GameController.GCMicroGamepadSnapshotDataVersion)
 
-    @expectedFailureIf(os_release() == "10.11")
-    @min_os_level("10.11")
+    @min_os_level("10.12")
     def testClasses(self):
-        self.assertIsInstance(GameController.GCMicroGamepad, objc.objc_class)
+        self.assertIsInstance(GameController.GCMicroGamepadSnapshot, objc.objc_class)
 
-    @expectedFailureIf(os_release() == "10.11")
     @min_os_level("10.11")
-    def testMethods(self):
-        self.assertResultIsBlock(
-            GameController.GCMicroGamepad.valueChangedHandler, b"v@@"
-        )
-        self.assertArgIsBlock(
-            GameController.GCMicroGamepad.setValueChangedHandler_, 0, b"v@@"
+    def testStructs(self):
+        self.assertEqual(
+            GameController.GCMicroGamepadSnapShotDataV100.__struct_pack__, 1
         )
 
-        self.assertResultIsBOOL(GameController.GCMicroGamepad.reportsAbsoluteDpadValues)
-        self.assertArgIsBOOL(
-            GameController.GCMicroGamepad.setReportsAbsoluteDpadValues_, 0
+        v = GameController.GCMicroGamepadSnapShotDataV100()
+        self.assertIsInstance(v.version, int)
+        self.assertIsInstance(v.size, int)
+        self.assertIsInstance(v.dpadX, float)
+        self.assertIsInstance(v.dpadY, float)
+        self.assertIsInstance(v.buttonA, float)
+        self.assertIsInstance(v.buttonX, float)
+        self.assertPickleRoundTrips(v)
+
+    @min_os_level("10.14")
+    def testStructs10_14_4(self):
+        self.assertEqual(GameController.GCMicroGamepadSnapshotData.__struct_pack__, 1)
+
+        v = GameController.GCMicroGamepadSnapshotData()
+        self.assertIsInstance(v.version, int)
+        self.assertIsInstance(v.size, int)
+        self.assertIsInstance(v.dpadX, float)
+        self.assertIsInstance(v.dpadY, float)
+        self.assertIsInstance(v.buttonA, float)
+        self.assertIsInstance(v.buttonX, float)
+
+    @expectedFailureIf(os_release().rsplit(".", 1)[0] in ("10.9", "10.10", "10.11"))
+    @min_os_level("10.9")
+    def testFunctions(self):
+        self.assertResultIsBOOL(GameController.GCMicroGamepadSnapShotDataV100FromNSData)
+        self.assertArgIsOut(GameController.GCMicroGamepadSnapShotDataV100FromNSData, 0)
+        self.assertArgIsIn(GameController.NSDataFromGCMicroGamepadSnapShotDataV100, 0)
+
+    @min_os_level("10.14.4")
+    def testFunctions10_14_4(self):
+        self.assertResultIsBOOL(GameController.GCMicroGamepadSnapshotDataFromNSData)
+        self.assertArgIsOut(GameController.GCMicroGamepadSnapshotDataFromNSData, 0)
+        self.assertArgIsIn(GameController.NSDataFromGCMicroGamepadSnapshotData, 0)
+
+    def test_constants(self):
+        self.assertEqual(GameController.GCMicroGamepadSnapshotDataVersion1, 0x0100)
+
+    @min_os_level("10.14.4")
+    def test_constants10_14_4(self):
+        self.assertIsInstance(
+            GameController.GCCurrentMicroGamepadSnapshotDataVersion, int
         )
-
-        self.assertResultIsBOOL(GameController.GCMicroGamepad.allowsRotation)
-        self.assertArgIsBOOL(GameController.GCMicroGamepad.setAllowsRotation_, 0)
```

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcmotion.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcmotion.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcmouse.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcmouse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcphysicalinputprofile.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcphysicalinputprofile.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcpressedstateinput.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcpressedstateinput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcproductcategories.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcproductcategories.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcracingwheel.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcracingwheel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcrelativeinput.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcrelativeinput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gcswitchpositioninput.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gcswitchpositioninput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/PyObjCTest/test_gctouchedstateinput.py` & `pyobjc-framework-GameController-9.2/PyObjCTest/test_gctouchedstateinput.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/GameController.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/GameController.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -1084,15 +1084,15 @@
    "GCMicroGamepadSnapshotDataFromNSData": {
     "args": {
      "0": { "type_modifier": "o" }
     }
    },
    "NSDataFromGCExtendedGamepadSnapShotDataV100": {
     "args": {
-     "0": {}
+     "0": { "type_modifier": "n"}
     }
    },
    "NSDataFromGCExtendedGamepadSnapshotData": {
     "args": {
      "0": { "type_modifier": "n" }
     }
    },
```

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/raw/arm64-12.1.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/raw/arm64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-10.9.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/raw/x86_64-10.9.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-12.1.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/raw/x86_64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-GameController-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/pyobjc_setup.py` & `pyobjc-framework-GameController-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameController-9.1b1/setup.py` & `pyobjc-framework-GameController-9.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 import os
+import sys
 
-from pyobjc_setup import setup, Extension
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import setup, Extension  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-GameController",
     description="Wrappers for the framework GameController on macOS",
     packages=["GameController"],
     ext_modules=[
         Extension(
```

