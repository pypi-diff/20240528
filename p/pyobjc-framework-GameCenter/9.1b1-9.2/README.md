# Comparing `tmp/pyobjc-framework-GameCenter-9.1b1.tar.gz` & `tmp/pyobjc-framework-GameCenter-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-GameCenter-9.1b1.tar", last modified: Sun Mar 26 11:24:48 2023, max compression
+gzip compressed data, was "pyobjc-framework-GameCenter-9.2.tar", last modified: Wed Jun  7 00:15:01 2023, max compression
```

## Comparing `pyobjc-framework-GameCenter-9.1b1.tar` & `pyobjc-framework-GameCenter-9.2.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:48.504012 pyobjc-framework-GameCenter-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:48.411550 pyobjc-framework-GameCenter-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:48.416886 pyobjc-framework-GameCenter-9.1b1/Lib/GameCenter/
--rw-r--r--   0 ronald     (501) staff       (20)      759 2020-11-30 18:45:15.000000 pyobjc-framework-GameCenter-9.1b1/Lib/GameCenter/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    53220 2022-02-24 08:47:16.000000 pyobjc-framework-GameCenter-9.1b1/Lib/GameCenter/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:48.420847 pyobjc-framework-GameCenter-9.1b1/Lib/pyobjc_framework_GameCenter.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2111 2023-03-26 11:24:48.000000 pyobjc-framework-GameCenter-9.1b1/Lib/pyobjc_framework_GameCenter.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1794 2023-03-26 11:24:48.000000 pyobjc-framework-GameCenter-9.1b1/Lib/pyobjc_framework_GameCenter.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:24:48.000000 pyobjc-framework-GameCenter-9.1b1/Lib/pyobjc_framework_GameCenter.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:12.000000 pyobjc-framework-GameCenter-9.1b1/Lib/pyobjc_framework_GameCenter.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:24:48.000000 pyobjc-framework-GameCenter-9.1b1/Lib/pyobjc_framework_GameCenter.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       11 2023-03-26 11:24:48.000000 pyobjc-framework-GameCenter-9.1b1/Lib/pyobjc_framework_GameCenter.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-GameCenter-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-GameCenter-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:48.423642 pyobjc-framework-GameCenter-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      854 2023-02-19 10:50:35.000000 pyobjc-framework-GameCenter-9.1b1/Modules/_GameCenter.m
--rw-r--r--   0 ronald     (501) staff       (20)     1754 2020-11-30 18:45:15.000000 pyobjc-framework-GameCenter-9.1b1/Modules/_GameCenter_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-GameCenter-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-GameCenter-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1900 2023-03-26 11:24:48.503458 pyobjc-framework-GameCenter-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:48.499585 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      425 2022-04-12 20:05:11.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gamecenter.py
--rw-r--r--   0 ronald     (501) staff       (20)     1277 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkachievement.py
--rw-r--r--   0 ronald     (501) staff       (20)      874 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkachievementdescription.py
--rw-r--r--   0 ronald     (501) staff       (20)      418 2022-06-25 09:11:02.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkachievementviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     1885 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkchallenge.py
--rw-r--r--   0 ronald     (501) staff       (20)     1174 2022-06-25 09:12:05.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkchallengeeventhandler.py
--rw-r--r--   0 ronald     (501) staff       (20)      453 2022-06-25 09:11:25.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkchallengesviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      468 2022-06-25 09:11:07.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkdialogcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     2037 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      244 2022-06-25 20:08:41.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkeventlistener.py
--rw-r--r--   0 ronald     (501) staff       (20)      289 2022-06-25 20:06:49.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkfriendrequestcomposeviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      645 2022-06-25 20:09:54.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkgamecenterviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     1531 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkleaderboard.py
--rw-r--r--   0 ronald     (501) staff       (20)      719 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkleaderboardset.py
--rw-r--r--   0 ronald     (501) staff       (20)      271 2022-06-25 20:15:23.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkleaderboardviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     2513 2022-06-25 09:12:11.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gklocalplayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2736 2022-06-25 09:11:13.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkmatch.py
--rw-r--r--   0 ronald     (501) staff       (20)     4441 2022-06-25 09:11:16.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkmatchmaker.py
--rw-r--r--   0 ronald     (501) staff       (20)      875 2022-06-25 09:10:58.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkmatchmakerviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      613 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gknotificationbanner.py
--rw-r--r--   0 ronald     (501) staff       (20)     1163 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkplayer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2430 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkpublicconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)      929 2022-06-25 09:11:41.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkpublicprotocols.py
--rw-r--r--   0 ronald     (501) staff       (20)      960 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gksavedgame.py
--rw-r--r--   0 ronald     (501) staff       (20)      248 2022-06-25 20:12:59.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gksavedgamelistener.py
--rw-r--r--   0 ronald     (501) staff       (20)      645 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkscore.py
--rw-r--r--   0 ronald     (501) staff       (20)     1011 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gksession.py
--rw-r--r--   0 ronald     (501) staff       (20)     1359 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gksessionerror.py
--rw-r--r--   0 ronald     (501) staff       (20)     6764 2022-06-25 20:18:14.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkturnbasedmatch.py
--rw-r--r--   0 ronald     (501) staff       (20)      713 2022-06-25 09:11:00.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkturnbasedmatchmakerviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     1594 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkvoicechat.py
--rw-r--r--   0 ronald     (501) staff       (20)      318 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkvoicechatservice.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:24:48.502547 pyobjc-framework-GameCenter-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    46728 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.1b1/metadata/GameCenter.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       36 2020-11-30 18:45:15.000000 pyobjc-framework-GameCenter-9.1b1/metadata/metadata.ini
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-GameCenter-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:24:48.504124 pyobjc-framework-GameCenter-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1143 2023-03-25 14:20:31.000000 pyobjc-framework-GameCenter-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:01.769539 pyobjc-framework-GameCenter-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:01.705521 pyobjc-framework-GameCenter-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:01.712496 pyobjc-framework-GameCenter-9.2/Lib/GameCenter/
+-rw-r--r--   0 ronald     (501) staff       (20)      759 2020-11-30 18:45:15.000000 pyobjc-framework-GameCenter-9.2/Lib/GameCenter/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    53220 2022-02-24 08:47:16.000000 pyobjc-framework-GameCenter-9.2/Lib/GameCenter/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:01.716550 pyobjc-framework-GameCenter-9.2/Lib/pyobjc_framework_GameCenter.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2109 2023-06-07 00:15:01.000000 pyobjc-framework-GameCenter-9.2/Lib/pyobjc_framework_GameCenter.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1809 2023-06-07 00:15:01.000000 pyobjc-framework-GameCenter-9.2/Lib/pyobjc_framework_GameCenter.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:15:01.000000 pyobjc-framework-GameCenter-9.2/Lib/pyobjc_framework_GameCenter.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:12.000000 pyobjc-framework-GameCenter-9.2/Lib/pyobjc_framework_GameCenter.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:15:01.000000 pyobjc-framework-GameCenter-9.2/Lib/pyobjc_framework_GameCenter.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       11 2023-06-07 00:15:01.000000 pyobjc-framework-GameCenter-9.2/Lib/pyobjc_framework_GameCenter.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-GameCenter-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-GameCenter-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:01.719146 pyobjc-framework-GameCenter-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      854 2023-02-19 10:50:35.000000 pyobjc-framework-GameCenter-9.2/Modules/_GameCenter.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1754 2020-11-30 18:45:15.000000 pyobjc-framework-GameCenter-9.2/Modules/_GameCenter_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-GameCenter-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-GameCenter-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1898 2023-06-07 00:15:01.768833 pyobjc-framework-GameCenter-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:01.766075 pyobjc-framework-GameCenter-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      425 2022-04-12 20:05:11.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gamecenter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1277 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkachievement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      874 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkachievementdescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      418 2022-06-25 09:11:02.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkachievementviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1885 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkchallenge.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1174 2022-06-25 09:12:05.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkchallengeeventhandler.py
+-rw-r--r--   0 ronald     (501) staff       (20)      453 2022-06-25 09:11:25.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkchallengesviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      468 2022-06-25 09:11:07.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkdialogcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2037 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      244 2022-06-25 20:08:41.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkeventlistener.py
+-rw-r--r--   0 ronald     (501) staff       (20)      289 2022-06-25 20:06:49.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkfriendrequestcomposeviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      645 2022-06-25 20:09:54.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkgamecenterviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1531 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkleaderboard.py
+-rw-r--r--   0 ronald     (501) staff       (20)      719 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkleaderboardset.py
+-rw-r--r--   0 ronald     (501) staff       (20)      271 2022-06-25 20:15:23.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkleaderboardviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2513 2022-06-25 09:12:11.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gklocalplayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2736 2022-06-25 09:11:13.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkmatch.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4441 2022-06-25 09:11:16.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkmatchmaker.py
+-rw-r--r--   0 ronald     (501) staff       (20)      875 2022-06-25 09:10:58.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkmatchmakerviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      613 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gknotificationbanner.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1163 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkplayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2430 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkpublicconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)      929 2022-06-25 09:11:41.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkpublicprotocols.py
+-rw-r--r--   0 ronald     (501) staff       (20)      960 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gksavedgame.py
+-rw-r--r--   0 ronald     (501) staff       (20)      248 2022-06-25 20:12:59.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gksavedgamelistener.py
+-rw-r--r--   0 ronald     (501) staff       (20)      645 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkscore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1011 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gksession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1359 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gksessionerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6764 2022-06-25 20:18:14.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkturnbasedmatch.py
+-rw-r--r--   0 ronald     (501) staff       (20)      713 2022-06-25 09:11:00.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkturnbasedmatchmakerviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1594 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkvoicechat.py
+-rw-r--r--   0 ronald     (501) staff       (20)      318 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkvoicechatservice.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:15:01.767987 pyobjc-framework-GameCenter-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    46728 2021-03-21 10:08:22.000000 pyobjc-framework-GameCenter-9.2/metadata/GameCenter.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       36 2020-11-30 18:45:15.000000 pyobjc-framework-GameCenter-9.2/metadata/metadata.ini
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-GameCenter-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-GameCenter-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:15:01.769649 pyobjc-framework-GameCenter-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1214 2023-05-29 10:07:46.000000 pyobjc-framework-GameCenter-9.2/setup.py
```

### Comparing `pyobjc-framework-GameCenter-9.1b1/Lib/GameCenter/__init__.py` & `pyobjc-framework-GameCenter-9.2/Lib/GameCenter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/Lib/GameCenter/_metadata.py` & `pyobjc-framework-GameCenter-9.2/Lib/GameCenter/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/Lib/pyobjc_framework_GameCenter.egg-info/PKG-INFO` & `pyobjc-framework-GameCenter-9.2/Lib/pyobjc_framework_GameCenter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-GameCenter
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework GameCenter on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,GameCenter
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-GameCenter-9.1b1/Lib/pyobjc_framework_GameCenter.egg-info/SOURCES.txt` & `pyobjc-framework-GameCenter-9.2/Lib/pyobjc_framework_GameCenter.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/GameCenter/__init__.py
 Lib/GameCenter/_metadata.py
 Lib/pyobjc_framework_GameCenter.egg-info/PKG-INFO
 Lib/pyobjc_framework_GameCenter.egg-info/SOURCES.txt
 Lib/pyobjc_framework_GameCenter.egg-info/dependency_links.txt
 Lib/pyobjc_framework_GameCenter.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-GameCenter-9.1b1/License.txt` & `pyobjc-framework-GameCenter-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/Modules/_GameCenter.m` & `pyobjc-framework-GameCenter-9.2/Modules/_GameCenter.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/Modules/_GameCenter_protocols.m` & `pyobjc-framework-GameCenter-9.2/Modules/_GameCenter_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-GameCenter-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-GameCenter-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-GameCenter-9.1b1/PKG-INFO` & `pyobjc-framework-GameCenter-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-GameCenter
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework GameCenter on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,GameCenter
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkachievement.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkachievement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkachievementdescription.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkachievementdescription.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkchallenge.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkchallenge.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkchallengeeventhandler.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkchallengeeventhandler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkerror.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkgamecenterviewcontroller.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkgamecenterviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkleaderboard.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkleaderboard.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkleaderboardset.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkleaderboardset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gklocalplayer.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gklocalplayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkmatch.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkmatch.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkmatchmaker.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkmatchmaker.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkmatchmakerviewcontroller.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkmatchmakerviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gknotificationbanner.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gknotificationbanner.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkplayer.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkplayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkpublicconstants.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkpublicconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkpublicprotocols.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkpublicprotocols.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gksavedgame.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gksavedgame.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkscore.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkscore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gksession.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gksession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gksessionerror.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gksessionerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkturnbasedmatch.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkturnbasedmatch.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkturnbasedmatchmakerviewcontroller.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkturnbasedmatchmakerviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/PyObjCTest/test_gkvoicechat.py` & `pyobjc-framework-GameCenter-9.2/PyObjCTest/test_gkvoicechat.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/metadata/GameCenter.fwinfo` & `pyobjc-framework-GameCenter-9.2/metadata/GameCenter.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-GameCenter-9.1b1/pyobjc_setup.py` & `pyobjc-framework-GameCenter-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

