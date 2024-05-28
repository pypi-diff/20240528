# Comparing `tmp/pyobjc-framework-GameKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-GameKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-GameKit-9.1b1.tar", last modified: Sun Mar 26 11:25:23 2023, max compression
+gzip compressed data, was "pyobjc-framework-GameKit-9.2.tar", last modified: Wed Jun  7 00:15:38 2023, max compression
```

## Comparing `pyobjc-framework-GameKit-9.1b1.tar` & `pyobjc-framework-GameKit-9.2.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:23.493766 pyobjc-framework-GameKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:23.359883 pyobjc-framework-GameKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:23.369577 pyobjc-framework-GameKit-9.1b1/Lib/GameKit/
--rw-r--r--   0 ronald     (501) staff       (20)      709 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.1b1/Lib/GameKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    89525 2023-03-24 18:54:07.000000 pyobjc-framework-GameKit-9.1b1/Lib/GameKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:23.375226 pyobjc-framework-GameKit-9.1b1/Lib/pyobjc_framework_GameKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2099 2023-03-26 11:25:23.000000 pyobjc-framework-GameKit-9.1b1/Lib/pyobjc_framework_GameKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     2254 2023-03-26 11:25:23.000000 pyobjc-framework-GameKit-9.1b1/Lib/pyobjc_framework_GameKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:25:23.000000 pyobjc-framework-GameKit-9.1b1/Lib/pyobjc_framework_GameKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:11.000000 pyobjc-framework-GameKit-9.1b1/Lib/pyobjc_framework_GameKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:25:23.000000 pyobjc-framework-GameKit-9.1b1/Lib/pyobjc_framework_GameKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        8 2023-03-26 11:25:23.000000 pyobjc-framework-GameKit-9.1b1/Lib/pyobjc_framework_GameKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-GameKit-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:23.378866 pyobjc-framework-GameKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      805 2021-10-18 19:38:40.000000 pyobjc-framework-GameKit-9.1b1/Modules/_GameKit.m
--rw-r--r--   0 ronald     (501) staff       (20)     1754 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.1b1/Modules/_GameKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-GameKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-GameKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1888 2023-03-26 11:25:23.491492 pyobjc-framework-GameKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:23.448529 pyobjc-framework-GameKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      419 2022-04-12 20:05:11.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gamekit.py
--rw-r--r--   0 ronald     (501) staff       (20)     1233 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkaccesspoint.py
--rw-r--r--   0 ronald     (501) staff       (20)     1173 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkachievement.py
--rw-r--r--   0 ronald     (501) staff       (20)      761 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkachievementdescription.py
--rw-r--r--   0 ronald     (501) staff       (20)      227 2022-06-25 20:06:52.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkachievementviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     2030 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkchallenge.py
--rw-r--r--   0 ronald     (501) staff       (20)      952 2022-06-25 20:18:03.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkchallengeeventhandler.py
--rw-r--r--   0 ronald     (501) staff       (20)      226 2022-06-25 20:15:19.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkchallengesviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      332 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkcloudplayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      212 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkdialogcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     2647 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      199 2022-06-25 20:12:43.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkeventlistener.py
--rw-r--r--   0 ronald     (501) staff       (20)      245 2022-06-25 20:18:01.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkfriendrequestcomposeviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      936 2022-06-25 20:11:34.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkgamecenterviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     2359 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkgamesession.py
--rw-r--r--   0 ronald     (501) staff       (20)     1542 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkgamesessionerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-25 20:17:42.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkgamesessioneventlistener.py
--rw-r--r--   0 ronald     (501) staff       (20)     2612 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkleaderboard.py
--rw-r--r--   0 ronald     (501) staff       (20)      930 2021-07-30 09:00:38.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkleaderboardset.py
--rw-r--r--   0 ronald     (501) staff       (20)      227 2022-06-25 20:07:50.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkleaderboardviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     4300 2022-06-25 09:13:17.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gklocalplayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2616 2022-06-25 09:13:00.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkmatch.py
--rw-r--r--   0 ronald     (501) staff       (20)     4703 2022-12-16 16:43:02.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkmatchmaker.py
--rw-r--r--   0 ronald     (501) staff       (20)     1438 2022-06-25 20:14:47.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkmatchmakerviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      511 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gknotificationhander.py
--rw-r--r--   0 ronald     (501) staff       (20)     1198 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkplayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1112 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkpublicconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)      509 2022-06-25 20:13:24.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkpublicprotocols.py
--rw-r--r--   0 ronald     (501) staff       (20)      832 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gksavedgame.py
--rw-r--r--   0 ronald     (501) staff       (20)      203 2022-06-25 20:06:54.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gksavedgamelistener.py
--rw-r--r--   0 ronald     (501) staff       (20)      546 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkscore.py
--rw-r--r--   0 ronald     (501) staff       (20)      792 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gksession.py
--rw-r--r--   0 ronald     (501) staff       (20)      278 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gksessionerror.py
--rw-r--r--   0 ronald     (501) staff       (20)     7002 2022-06-25 20:10:29.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkturnbasedmatch.py
--rw-r--r--   0 ronald     (501) staff       (20)      539 2022-06-25 20:15:39.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkturnbasedmatchmakerviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     1721 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkvoicechat.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:23.452713 pyobjc-framework-GameKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    35512 2021-08-01 07:34:44.000000 pyobjc-framework-GameKit-9.1b1/metadata/GameKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       30 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:25:23.489599 pyobjc-framework-GameKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   244751 2021-08-01 07:34:44.000000 pyobjc-framework-GameKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   245564 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   248389 2022-12-16 16:43:02.000000 pyobjc-framework-GameKit-9.1b1/metadata/raw/arm64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   248389 2023-03-24 18:54:07.000000 pyobjc-framework-GameKit-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   187824 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   191073 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   239953 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   244752 2021-08-01 07:34:44.000000 pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   245565 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   248390 2022-12-16 16:43:02.000000 pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   248390 2023-03-24 18:54:07.000000 pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-GameKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:25:23.493924 pyobjc-framework-GameKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1189 2023-03-25 14:20:31.000000 pyobjc-framework-GameKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:38.566268 pyobjc-framework-GameKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:38.441766 pyobjc-framework-GameKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:38.447610 pyobjc-framework-GameKit-9.2/Lib/GameKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      709 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.2/Lib/GameKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    89525 2023-03-24 18:54:07.000000 pyobjc-framework-GameKit-9.2/Lib/GameKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:38.451945 pyobjc-framework-GameKit-9.2/Lib/pyobjc_framework_GameKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2097 2023-06-07 00:15:38.000000 pyobjc-framework-GameKit-9.2/Lib/pyobjc_framework_GameKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     2269 2023-06-07 00:15:38.000000 pyobjc-framework-GameKit-9.2/Lib/pyobjc_framework_GameKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:15:38.000000 pyobjc-framework-GameKit-9.2/Lib/pyobjc_framework_GameKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:11.000000 pyobjc-framework-GameKit-9.2/Lib/pyobjc_framework_GameKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:15:38.000000 pyobjc-framework-GameKit-9.2/Lib/pyobjc_framework_GameKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        8 2023-06-07 00:15:38.000000 pyobjc-framework-GameKit-9.2/Lib/pyobjc_framework_GameKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-GameKit-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:38.455229 pyobjc-framework-GameKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      805 2021-10-18 19:38:40.000000 pyobjc-framework-GameKit-9.2/Modules/_GameKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1754 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.2/Modules/_GameKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-GameKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-GameKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1886 2023-06-07 00:15:38.564427 pyobjc-framework-GameKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:38.508628 pyobjc-framework-GameKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      419 2022-04-12 20:05:11.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gamekit.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1233 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkaccesspoint.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1173 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkachievement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      761 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkachievementdescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      227 2022-06-25 20:06:52.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkachievementviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2030 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkchallenge.py
+-rw-r--r--   0 ronald     (501) staff       (20)      952 2022-06-25 20:18:03.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkchallengeeventhandler.py
+-rw-r--r--   0 ronald     (501) staff       (20)      226 2022-06-25 20:15:19.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkchallengesviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      332 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkcloudplayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      212 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkdialogcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2647 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      199 2022-06-25 20:12:43.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkeventlistener.py
+-rw-r--r--   0 ronald     (501) staff       (20)      245 2022-06-25 20:18:01.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkfriendrequestcomposeviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      936 2022-06-25 20:11:34.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkgamecenterviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2359 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkgamesession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1542 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkgamesessionerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2022-06-25 20:17:42.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkgamesessioneventlistener.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2612 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkleaderboard.py
+-rw-r--r--   0 ronald     (501) staff       (20)      930 2021-07-30 09:00:38.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkleaderboardset.py
+-rw-r--r--   0 ronald     (501) staff       (20)      227 2022-06-25 20:07:50.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkleaderboardviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4300 2023-05-04 11:00:07.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gklocalplayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2616 2022-06-25 09:13:00.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkmatch.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4729 2023-05-04 11:00:07.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkmatchmaker.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1438 2022-06-25 20:14:47.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkmatchmakerviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      511 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gknotificationhander.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1198 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkplayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1112 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkpublicconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)      509 2022-06-25 20:13:24.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkpublicprotocols.py
+-rw-r--r--   0 ronald     (501) staff       (20)      832 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gksavedgame.py
+-rw-r--r--   0 ronald     (501) staff       (20)      203 2022-06-25 20:06:54.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gksavedgamelistener.py
+-rw-r--r--   0 ronald     (501) staff       (20)      546 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkscore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      792 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gksession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      278 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gksessionerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7002 2022-06-25 20:10:29.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkturnbasedmatch.py
+-rw-r--r--   0 ronald     (501) staff       (20)      539 2022-06-25 20:15:39.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkturnbasedmatchmakerviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1721 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkvoicechat.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:38.515797 pyobjc-framework-GameKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    35512 2021-08-01 07:34:44.000000 pyobjc-framework-GameKit-9.2/metadata/GameKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:38.552695 pyobjc-framework-GameKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   244751 2021-08-01 07:34:44.000000 pyobjc-framework-GameKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   245564 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   248389 2022-12-16 16:43:02.000000 pyobjc-framework-GameKit-9.2/metadata/raw/arm64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   248389 2023-03-24 18:54:07.000000 pyobjc-framework-GameKit-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   187824 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   191073 2020-11-30 18:45:15.000000 pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   239953 2021-03-21 10:08:22.000000 pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   244752 2021-08-01 07:34:44.000000 pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   245565 2022-02-24 08:47:16.000000 pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   248390 2022-12-16 16:43:02.000000 pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   248390 2023-03-24 18:54:07.000000 pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-GameKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-GameKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:15:38.566675 pyobjc-framework-GameKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1260 2023-05-29 10:07:46.000000 pyobjc-framework-GameKit-9.2/setup.py
```

### Comparing `pyobjc-framework-GameKit-9.1b1/Lib/GameKit/__init__.py` & `pyobjc-framework-GameKit-9.2/Lib/GameKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/Lib/GameKit/_metadata.py` & `pyobjc-framework-GameKit-9.2/Lib/GameKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/Lib/pyobjc_framework_GameKit.egg-info/PKG-INFO` & `pyobjc-framework-GameKit-9.2/Lib/pyobjc_framework_GameKit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-GameKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework GameKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,GameKit
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-GameKit-9.1b1/Lib/pyobjc_framework_GameKit.egg-info/SOURCES.txt` & `pyobjc-framework-GameKit-9.2/Lib/pyobjc_framework_GameKit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/GameKit/__init__.py
 Lib/GameKit/_metadata.py
 Lib/pyobjc_framework_GameKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_GameKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_GameKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_GameKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-GameKit-9.1b1/License.txt` & `pyobjc-framework-GameKit-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/Modules/_GameKit.m` & `pyobjc-framework-GameKit-9.2/Modules/_GameKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/Modules/_GameKit_protocols.m` & `pyobjc-framework-GameKit-9.2/Modules/_GameKit_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-GameKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-GameKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-GameKit-9.1b1/PKG-INFO` & `pyobjc-framework-GameKit-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-GameKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework GameKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,GameKit
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkaccesspoint.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkaccesspoint.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkachievement.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkachievement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkachievementdescription.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkachievementdescription.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkchallenge.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkchallenge.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkchallengeeventhandler.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkchallengeeventhandler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkerror.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkgamecenterviewcontroller.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkgamecenterviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkgamesession.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkgamesession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkgamesessionerror.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkgamesessionerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkleaderboard.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkleaderboard.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkleaderboardset.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkleaderboardset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gklocalplayer.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gklocalplayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             0,
             b"v@@@Q@",
         )
         self.assertArgIsBlock(
             GameKit.GKLocalPlayer.loadFriendPlayersWithCompletionHandler_, 0, b"v@@"
         )
 
-    @min_os_level("10.11")
+    @min_os_level("10.12")
     def testMethods10_11(self):
         self.assertArgIsBlock(
             GameKit.GKLocalPlayer.loadRecentPlayersWithCompletionHandler_, 0, b"v@@"
         )
 
     @min_os_level("10.15")
     def testMethods10_15(self):
```

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkmatch.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkmatch.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkmatchmaker.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkmatchmaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 
     @min_os_level("10.15")
     @expectedFailure
     def testMethods10_15(self):
         self.assertResultIsBOOL(GameKit.GKMatchRequest.restrictToAutomatch)
         self.assertArgIsBOOL(GameKit.GKMatchRequest.setRestrictToAutomatch_, 0)
 
+    @min_os_level("13.1")
     def testMethods13_1(self):
         self.assertArgIsBlock(
             GameKit.GKMatchmaker.startGroupActivityWithPlayerHandler_, 0, b"v@"
         )
 
     def testProtocols(self):
         self.assertProtocolExists("GKInviteEventListener")
```

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkmatchmakerviewcontroller.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkmatchmakerviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkplayer.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkplayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkpublicconstants.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkpublicconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gksavedgame.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gksavedgame.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkscore.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkscore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gksession.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gksession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkturnbasedmatch.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkturnbasedmatch.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkturnbasedmatchmakerviewcontroller.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkturnbasedmatchmakerviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/PyObjCTest/test_gkvoicechat.py` & `pyobjc-framework-GameKit-9.2/PyObjCTest/test_gkvoicechat.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/metadata/GameKit.fwinfo` & `pyobjc-framework-GameKit-9.2/metadata/GameKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-GameKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-GameKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/metadata/raw/arm64-13.1.fwinfo` & `pyobjc-framework-GameKit-9.2/metadata/raw/arm64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-GameKit-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-10.13.fwinfo` & `pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-13.1.fwinfo` & `pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-GameKit-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-GameKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameKit-9.1b1/setup.py` & `pyobjc-framework-GameKit-9.2/setup.py`

 * *Files 8% similar despite different names*

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
     name="pyobjc-framework-GameKit",
     description="Wrappers for the framework GameKit on macOS",
     min_os_level="10.8",
     packages=["GameKit"],
     ext_modules=[
```

