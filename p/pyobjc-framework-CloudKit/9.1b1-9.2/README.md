# Comparing `tmp/pyobjc-framework-CloudKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-CloudKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CloudKit-9.1b1.tar", last modified: Sun Mar 26 11:16:50 2023, max compression
+gzip compressed data, was "pyobjc-framework-CloudKit-9.2.tar", last modified: Wed Jun  7 00:07:52 2023, max compression
```

## Comparing `pyobjc-framework-CloudKit-9.1b1.tar` & `pyobjc-framework-CloudKit-9.2.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:50.406914 pyobjc-framework-CloudKit-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CloudKit-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:50.182976 pyobjc-framework-CloudKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:50.199628 pyobjc-framework-CloudKit-9.1b1/Lib/CloudKit/
--rw-r--r--   0 ronald     (501) staff       (20)      773 2020-11-30 18:45:14.000000 pyobjc-framework-CloudKit-9.1b1/Lib/CloudKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    80942 2023-02-19 10:50:34.000000 pyobjc-framework-CloudKit-9.1b1/Lib/CloudKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:50.207502 pyobjc-framework-CloudKit-9.1b1/Lib/pyobjc_framework_CloudKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2130 2023-03-26 11:16:50.000000 pyobjc-framework-CloudKit-9.1b1/Lib/pyobjc_framework_CloudKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     2705 2023-03-26 11:16:50.000000 pyobjc-framework-CloudKit-9.1b1/Lib/pyobjc_framework_CloudKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:16:50.000000 pyobjc-framework-CloudKit-9.1b1/Lib/pyobjc_framework_CloudKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:47.000000 pyobjc-framework-CloudKit-9.1b1/Lib/pyobjc_framework_CloudKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)      152 2023-03-26 11:16:50.000000 pyobjc-framework-CloudKit-9.1b1/Lib/pyobjc_framework_CloudKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:16:50.000000 pyobjc-framework-CloudKit-9.1b1/Lib/pyobjc_framework_CloudKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CloudKit-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1919 2023-03-26 11:16:50.405064 pyobjc-framework-CloudKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:50.332219 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      682 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckacceptsharesoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)     1175 2022-06-15 11:57:00.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckallowedsharingoptions.py
--rw-r--r--   0 ronald     (501) staff       (20)      285 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckasset.py
--rw-r--r--   0 ronald     (501) staff       (20)     4651 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckcontainer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2137 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdatabase.py
--rw-r--r--   0 ronald     (501) staff       (20)      321 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdatabaseoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      734 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdiscoverallcontactsoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      881 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdiscoveralluseridentitiesoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      647 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdiscovereduserinfo.py
--rw-r--r--   0 ronald     (501) staff       (20)      858 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdiscoveruseridentitiesoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      722 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdiscoveruserinfosoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)     3120 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckerror.py
--rw-r--r--   0 ronald     (501) staff       (20)     2453 2021-07-30 09:00:37.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchdatabasechangesoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)     1239 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchnotificationchangesoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)     1484 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchrecordchangesoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)     1141 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchrecordsoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)     2365 2021-07-30 09:00:37.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchrecordzonechangesoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)     1049 2021-07-30 09:00:37.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchrecordzonesoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      995 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchsharemetadataoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      848 2021-08-04 10:00:17.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchshareparticipantsoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      655 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchsubscriptionsoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      563 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchwebauthtokenoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      336 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_cklocationsortdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      784 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckmarknotificationsreadoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      807 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckmodifybadgeoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)     2263 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckmodifyrecordsoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      722 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckmodifyrecordzonesoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      736 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckmodifysubscriptionoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)     1093 2021-07-30 09:00:37.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckmodifysubscriptionsoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)     1573 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_cknotification.py
--rw-r--r--   0 ronald     (501) staff       (20)     1521 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      869 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckoperationgroup.py
--rw-r--r--   0 ronald     (501) staff       (20)      285 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckquery.py
--rw-r--r--   0 ronald     (501) staff       (20)     1287 2021-07-30 09:00:37.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckqueryoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      734 2022-06-25 08:59:47.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckrecord.py
--rw-r--r--   0 ronald     (501) staff       (20)      294 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckrecordid.py
--rw-r--r--   0 ronald     (501) staff       (20)      827 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckrecordzone.py
--rw-r--r--   0 ronald     (501) staff       (20)      306 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckrecordzoneid.py
--rw-r--r--   0 ronald     (501) staff       (20)      570 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckreference.py
--rw-r--r--   0 ronald     (501) staff       (20)      556 2021-07-30 09:00:37.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckshare.py
--rw-r--r--   0 ronald     (501) staff       (20)     1652 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckshareparticipant.py
--rw-r--r--   0 ronald     (501) staff       (20)     2222 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_cksubscription.py
--rw-r--r--   0 ronald     (501) staff       (20)      788 2022-10-18 09:53:23.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_cksystemsharinguiobserver.py
--rw-r--r--   0 ronald     (501) staff       (20)      246 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckuseridentity.py
--rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_cloudkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      862 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_skfetchshareparticipantsoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      310 2021-10-18 19:38:40.000000 pyobjc-framework-CloudKit-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:50.343382 pyobjc-framework-CloudKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    68538 2022-06-27 11:20:33.000000 pyobjc-framework-CloudKit-9.1b1/metadata/CloudKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:14.000000 pyobjc-framework-CloudKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:50.399771 pyobjc-framework-CloudKit-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   224011 2021-07-31 11:33:37.000000 pyobjc-framework-CloudKit-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   220699 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   229862 2022-10-18 09:53:23.000000 pyobjc-framework-CloudKit-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   229730 2023-02-19 10:50:34.000000 pyobjc-framework-CloudKit-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   103817 2020-11-30 18:45:14.000000 pyobjc-framework-CloudKit-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   207379 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   224012 2021-07-31 11:33:37.000000 pyobjc-framework-CloudKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   220700 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   229863 2022-10-18 09:53:23.000000 pyobjc-framework-CloudKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   229731 2023-02-19 10:50:34.000000 pyobjc-framework-CloudKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CloudKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:16:50.407105 pyobjc-framework-CloudKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      835 2023-03-25 14:20:30.000000 pyobjc-framework-CloudKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:52.154918 pyobjc-framework-CloudKit-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CloudKit-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:52.062626 pyobjc-framework-CloudKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:52.070812 pyobjc-framework-CloudKit-9.2/Lib/CloudKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      773 2020-11-30 18:45:14.000000 pyobjc-framework-CloudKit-9.2/Lib/CloudKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    80942 2023-02-19 10:50:34.000000 pyobjc-framework-CloudKit-9.2/Lib/CloudKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:52.075034 pyobjc-framework-CloudKit-9.2/Lib/pyobjc_framework_CloudKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2128 2023-06-07 00:07:52.000000 pyobjc-framework-CloudKit-9.2/Lib/pyobjc_framework_CloudKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     2720 2023-06-07 00:07:52.000000 pyobjc-framework-CloudKit-9.2/Lib/pyobjc_framework_CloudKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:07:52.000000 pyobjc-framework-CloudKit-9.2/Lib/pyobjc_framework_CloudKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:47.000000 pyobjc-framework-CloudKit-9.2/Lib/pyobjc_framework_CloudKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)      142 2023-06-07 00:07:52.000000 pyobjc-framework-CloudKit-9.2/Lib/pyobjc_framework_CloudKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:07:52.000000 pyobjc-framework-CloudKit-9.2/Lib/pyobjc_framework_CloudKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CloudKit-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1917 2023-06-07 00:07:52.154529 pyobjc-framework-CloudKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:52.123620 pyobjc-framework-CloudKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      682 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckacceptsharesoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1175 2022-06-15 11:57:00.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckallowedsharingoptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)      285 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckasset.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4651 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckcontainer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2137 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdatabase.py
+-rw-r--r--   0 ronald     (501) staff       (20)      321 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdatabaseoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      734 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdiscoverallcontactsoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      881 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdiscoveralluseridentitiesoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      647 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdiscovereduserinfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)      858 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdiscoveruseridentitiesoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      722 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdiscoveruserinfosoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3120 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2453 2021-07-30 09:00:37.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchdatabasechangesoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1239 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchnotificationchangesoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1484 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchrecordchangesoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1141 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchrecordsoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2365 2021-07-30 09:00:37.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchrecordzonechangesoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1049 2021-07-30 09:00:37.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchrecordzonesoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      995 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchsharemetadataoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      848 2021-08-04 10:00:17.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchshareparticipantsoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      655 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchsubscriptionsoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      563 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchwebauthtokenoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      336 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_cklocationsortdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      784 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckmarknotificationsreadoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      807 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckmodifybadgeoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2263 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckmodifyrecordsoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      722 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckmodifyrecordzonesoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      736 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckmodifysubscriptionoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1093 2021-07-30 09:00:37.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckmodifysubscriptionsoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1573 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_cknotification.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1521 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      869 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckoperationgroup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      285 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1287 2021-07-30 09:00:37.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckqueryoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      861 2023-05-04 11:00:07.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckrecord.py
+-rw-r--r--   0 ronald     (501) staff       (20)      294 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckrecordid.py
+-rw-r--r--   0 ronald     (501) staff       (20)      827 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckrecordzone.py
+-rw-r--r--   0 ronald     (501) staff       (20)      306 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckrecordzoneid.py
+-rw-r--r--   0 ronald     (501) staff       (20)      570 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckreference.py
+-rw-r--r--   0 ronald     (501) staff       (20)      556 2021-07-30 09:00:37.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckshare.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1652 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckshareparticipant.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2222 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_cksubscription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      788 2022-10-18 09:53:23.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_cksystemsharinguiobserver.py
+-rw-r--r--   0 ronald     (501) staff       (20)      246 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckuseridentity.py
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_cloudkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      862 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/PyObjCTest/test_skfetchshareparticipantsoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      310 2021-10-18 19:38:40.000000 pyobjc-framework-CloudKit-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:52.127150 pyobjc-framework-CloudKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    68538 2022-06-27 11:20:33.000000 pyobjc-framework-CloudKit-9.2/metadata/CloudKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:14.000000 pyobjc-framework-CloudKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:52.151948 pyobjc-framework-CloudKit-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   224011 2021-07-31 11:33:37.000000 pyobjc-framework-CloudKit-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   220699 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   229862 2022-10-18 09:53:23.000000 pyobjc-framework-CloudKit-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   229730 2023-02-19 10:50:34.000000 pyobjc-framework-CloudKit-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   103817 2020-11-30 18:45:14.000000 pyobjc-framework-CloudKit-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   207379 2021-03-21 10:08:22.000000 pyobjc-framework-CloudKit-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   224012 2021-07-31 11:33:37.000000 pyobjc-framework-CloudKit-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   220700 2022-02-24 08:47:16.000000 pyobjc-framework-CloudKit-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   229863 2022-10-18 09:53:23.000000 pyobjc-framework-CloudKit-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   229731 2023-02-19 10:50:34.000000 pyobjc-framework-CloudKit-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CloudKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CloudKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:07:52.155034 pyobjc-framework-CloudKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      916 2023-05-29 10:07:45.000000 pyobjc-framework-CloudKit-9.2/setup.py
```

### Comparing `pyobjc-framework-CloudKit-9.1b1/LICENSE.txt` & `pyobjc-framework-CloudKit-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/Lib/CloudKit/__init__.py` & `pyobjc-framework-CloudKit-9.2/Lib/CloudKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/Lib/CloudKit/_metadata.py` & `pyobjc-framework-CloudKit-9.2/Lib/CloudKit/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/Lib/pyobjc_framework_CloudKit.egg-info/PKG-INFO` & `pyobjc-framework-CloudKit-9.2/Lib/pyobjc_framework_CloudKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CloudKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CloudKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CloudKit
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-CloudKit-9.1b1/Lib/pyobjc_framework_CloudKit.egg-info/SOURCES.txt` & `pyobjc-framework-CloudKit-9.2/Lib/pyobjc_framework_CloudKit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CloudKit/__init__.py
 Lib/CloudKit/_metadata.py
 Lib/pyobjc_framework_CloudKit.egg-info/PKG-INFO
 Lib/pyobjc_framework_CloudKit.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CloudKit.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CloudKit.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CloudKit-9.1b1/PKG-INFO` & `pyobjc-framework-CloudKit-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CloudKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CloudKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CloudKit
 Platform: MacOS X (>=10.10)
```

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckacceptsharesoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckacceptsharesoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckallowedsharingoptions.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckallowedsharingoptions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckcontainer.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckcontainer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdatabase.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdatabase.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdiscoverallcontactsoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdiscoverallcontactsoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdiscoveralluseridentitiesoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdiscoveralluseridentitiesoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdiscovereduserinfo.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdiscovereduserinfo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdiscoveruseridentitiesoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdiscoveruseridentitiesoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckdiscoveruserinfosoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckdiscoveruserinfosoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckerror.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchdatabasechangesoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchdatabasechangesoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchnotificationchangesoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchnotificationchangesoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchrecordchangesoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchrecordchangesoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchrecordsoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchrecordsoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchrecordzonechangesoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchrecordzonechangesoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchrecordzonesoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchrecordzonesoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchsharemetadataoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchsharemetadataoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchshareparticipantsoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchshareparticipantsoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchsubscriptionsoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchsubscriptionsoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckfetchwebauthtokenoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckfetchwebauthtokenoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckmarknotificationsreadoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckmarknotificationsreadoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckmodifybadgeoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckmodifybadgeoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckmodifyrecordsoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckmodifyrecordsoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckmodifyrecordzonesoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckmodifyrecordzonesoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckmodifysubscriptionoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckmodifysubscriptionoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckmodifysubscriptionsoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckmodifysubscriptionsoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_cknotification.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_cknotification.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckoperationgroup.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckoperationgroup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckqueryoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckqueryoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckrecord.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckrecord.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from PyObjCTools.TestSupport import TestCase, min_os_level, min_sdk_level
 import CloudKit
 import objc
 
 
 class TestCKRecord(TestCase):
-    @min_sdk_level("10.11")
+    @min_sdk_level("10.12")
     def testProtocols(self):
+        # Documentation claims this protocol is available on 10.11,
+        # but value isn't present in the latest 10.11 SDK.
         self.assertProtocolExists("CKRecordKeyValueSetting")
 
     @min_os_level("10.10")
     def testClasses(self):
         self.assertHasAttr(CloudKit, "CKRecord")
         self.assertIsInstance(CloudKit.CKRecord, objc.objc_class)
```

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckrecordzone.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckrecordzone.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckreference.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckreference.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckshare.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckshare.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_ckshareparticipant.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_ckshareparticipant.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_cksubscription.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_cksubscription.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_cksystemsharinguiobserver.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_cksystemsharinguiobserver.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/PyObjCTest/test_skfetchshareparticipantsoperation.py` & `pyobjc-framework-CloudKit-9.2/PyObjCTest/test_skfetchshareparticipantsoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/metadata/CloudKit.fwinfo` & `pyobjc-framework-CloudKit-9.2/metadata/CloudKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CloudKit-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CloudKit-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-CloudKit-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-CloudKit-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-CloudKit-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CloudKit-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CloudKit-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CloudKit-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-CloudKit-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-CloudKit-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CloudKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CloudKit-9.1b1/setup.py` & `pyobjc-framework-CloudKit-9.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "CloudKit" framework on macOS.
 
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
     name="pyobjc-framework-CloudKit",
     description="Wrappers for the framework CloudKit on macOS",
     min_os_level="10.10",
     packages=["CloudKit"],
     version=VERSION,
```

