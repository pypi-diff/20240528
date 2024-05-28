# Comparing `tmp/pyobjc-framework-Intents-9.1b1.tar.gz` & `tmp/pyobjc-framework-Intents-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Intents-9.1b1.tar", last modified: Sun Mar 26 11:27:28 2023, max compression
+gzip compressed data, was "pyobjc-framework-Intents-9.2.tar", last modified: Wed Jun  7 00:17:51 2023, max compression
```

## Comparing `pyobjc-framework-Intents-9.1b1.tar` & `pyobjc-framework-Intents-9.2.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:28.453407 pyobjc-framework-Intents-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:28.253244 pyobjc-framework-Intents-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:28.258202 pyobjc-framework-Intents-9.1b1/Lib/Intents/
--rw-r--r--   0 ronald     (501) staff       (20)      719 2020-11-30 18:45:15.000000 pyobjc-framework-Intents-9.1b1/Lib/Intents/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)   227479 2023-02-19 10:50:35.000000 pyobjc-framework-Intents-9.1b1/Lib/Intents/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:28.274402 pyobjc-framework-Intents-9.1b1/Lib/pyobjc_framework_Intents.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2100 2023-03-26 11:27:28.000000 pyobjc-framework-Intents-9.1b1/Lib/pyobjc_framework_Intents.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     2984 2023-03-26 11:27:28.000000 pyobjc-framework-Intents-9.1b1/Lib/pyobjc_framework_Intents.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:27:28.000000 pyobjc-framework-Intents-9.1b1/Lib/pyobjc_framework_Intents.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:21.000000 pyobjc-framework-Intents-9.1b1/Lib/pyobjc_framework_Intents.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:27:28.000000 pyobjc-framework-Intents-9.1b1/Lib/pyobjc_framework_Intents.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        8 2023-03-26 11:27:28.000000 pyobjc-framework-Intents-9.1b1/Lib/pyobjc_framework_Intents.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Intents-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Intents-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:28.277723 pyobjc-framework-Intents-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      806 2021-10-18 19:38:40.000000 pyobjc-framework-Intents-9.1b1/Modules/_Intents.m
--rw-r--r--   0 ronald     (501) staff       (20)     1162 2022-12-17 13:23:18.000000 pyobjc-framework-Intents-9.1b1/Modules/_Intents_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:33.000000 pyobjc-framework-Intents-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-02-19 12:24:44.000000 pyobjc-framework-Intents-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1889 2023-03-26 11:27:28.452121 pyobjc-framework-Intents-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:28.370378 pyobjc-framework-Intents-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      797 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inaddmediaintentresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)      703 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inanswercallintent.py
--rw-r--r--   0 ronald     (501) staff       (20)      817 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inanswercallintentresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)      296 2021-07-30 09:00:38.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inbooleanresolutionresult.py
--rw-r--r--   0 ronald     (501) staff       (20)      428 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_incallaudioroute.py
--rw-r--r--   0 ronald     (501) staff       (20)      445 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_incallcapability.py
--rw-r--r--   0 ronald     (501) staff       (20)      420 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_incallcapabilityoptions.py
--rw-r--r--   0 ronald     (501) staff       (20)     1621 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_incalldestinationtype.py
--rw-r--r--   0 ronald     (501) staff       (20)      264 2021-07-30 09:00:38.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_incallrecordresolutionresult.py
--rw-r--r--   0 ronald     (501) staff       (20)      935 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_incallrecordtype.py
--rw-r--r--   0 ronald     (501) staff       (20)      852 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_incallrecordtypeoptions.py
--rw-r--r--   0 ronald     (501) staff       (20)      455 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inconditionaloperator.py
--rw-r--r--   0 ronald     (501) staff       (20)      258 2022-01-02 11:04:26.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_infile.py
--rw-r--r--   0 ronald     (501) staff       (20)      819 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_infocusstatuscenter.py
--rw-r--r--   0 ronald     (501) staff       (20)      859 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_ingetreservationdetailsintentresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)      703 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inhangUpcallintent.py
--rw-r--r--   0 ronald     (501) staff       (20)      825 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inhangupcallintentresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)     2828 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inintenterrors.py
--rw-r--r--   0 ronald     (501) staff       (20)     1068 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inintentidentifiers.py
--rw-r--r--   0 ronald     (501) staff       (20)     1651 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_ininteraction.py
--rw-r--r--   0 ronald     (501) staff       (20)     1834 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inmessage.py
--rw-r--r--   0 ronald     (501) staff       (20)      643 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inmessageattributeoptions.py
--rw-r--r--   0 ronald     (501) staff       (20)      340 2021-07-30 09:00:38.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inobjectcollection.py
--rw-r--r--   0 ronald     (501) staff       (20)      451 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inoutgoingmessagetype.py
--rw-r--r--   0 ronald     (501) staff       (20)      237 2021-03-21 10:08:22.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inparameter.py
--rw-r--r--   0 ronald     (501) staff       (20)      709 2021-03-21 10:08:22.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inpaymentmethodtypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      599 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inperson.py
--rw-r--r--   0 ronald     (501) staff       (20)      354 2021-03-21 10:08:22.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inperson_siriadditions.py
--rw-r--r--   0 ronald     (501) staff       (20)      456 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inpersonhandle.py
--rw-r--r--   0 ronald     (501) staff       (20)     1025 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inpersonhandlelabel.py
--rw-r--r--   0 ronald     (501) staff       (20)     1261 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inpersonrelationship.py
--rw-r--r--   0 ronald     (501) staff       (20)      724 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inrecurrencefrequency.py
--rw-r--r--   0 ronald     (501) staff       (20)      368 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inreservationactiontype.py
--rw-r--r--   0 ronald     (501) staff       (20)      544 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inreservationstatus.py
--rw-r--r--   0 ronald     (501) staff       (20)     2351 2022-06-25 20:14:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insearchcallhistoryintent.py
--rw-r--r--   0 ronald     (501) staff       (20)     1062 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insearchcallhistoryintentresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)     3430 2022-06-25 20:06:29.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insearchformessagesintent.py
--rw-r--r--   0 ronald     (501) staff       (20)     1101 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insearchformessagesintentresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)     2753 2022-06-25 20:14:45.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insendmessageintent.py
--rw-r--r--   0 ronald     (501) staff       (20)      909 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insendmessageintentresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)      931 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insendmessagerecipientresolutionresult.py
--rw-r--r--   0 ronald     (501) staff       (20)      798 2022-06-25 20:16:06.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insharefocusstatusintent.py
--rw-r--r--   0 ronald     (501) staff       (20)      785 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insharefocusstatusintentresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)      230 2022-06-25 20:13:22.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inspeakable.py
--rw-r--r--   0 ronald     (501) staff       (20)     1362 2022-06-25 20:08:54.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_instartaudiocallintent.py
--rw-r--r--   0 ronald     (501) staff       (20)     1237 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_instartaudiocallintentresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)     1695 2022-06-25 20:16:53.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_instartcallintent.py
--rw-r--r--   0 ronald     (501) staff       (20)     1066 2022-06-25 20:11:43.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_instartvideocallintent.py
--rw-r--r--   0 ronald     (501) staff       (20)     1237 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_instartvideocallintentresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_intents.py
--rw-r--r--   0 ronald     (501) staff       (20)      366 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inticketedeventcategory.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:28.371939 pyobjc-framework-Intents-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    30300 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/metadata/Intents.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       30 2020-11-30 18:45:15.000000 pyobjc-framework-Intents-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:28.441283 pyobjc-framework-Intents-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   930893 2022-01-02 11:04:26.000000 pyobjc-framework-Intents-9.1b1/metadata/raw/arm64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   939566 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   961877 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.1b1/metadata/raw/arm64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   961882 2023-02-19 10:50:35.000000 pyobjc-framework-Intents-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   774867 2020-11-30 18:45:15.000000 pyobjc-framework-Intents-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   907461 2021-03-21 10:08:22.000000 pyobjc-framework-Intents-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   930917 2022-01-02 11:04:26.000000 pyobjc-framework-Intents-9.1b1/metadata/raw/x86_64-12.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   939590 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   961901 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.1b1/metadata/raw/x86_64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   961906 2023-02-19 10:50:35.000000 pyobjc-framework-Intents-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Intents-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:27:28.453581 pyobjc-framework-Intents-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1120 2023-03-25 14:20:31.000000 pyobjc-framework-Intents-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:51.918690 pyobjc-framework-Intents-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:51.742697 pyobjc-framework-Intents-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:51.757947 pyobjc-framework-Intents-9.2/Lib/Intents/
+-rw-r--r--   0 ronald     (501) staff       (20)      719 2020-11-30 18:45:15.000000 pyobjc-framework-Intents-9.2/Lib/Intents/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)   227479 2023-02-19 10:50:35.000000 pyobjc-framework-Intents-9.2/Lib/Intents/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:51.762991 pyobjc-framework-Intents-9.2/Lib/pyobjc_framework_Intents.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2098 2023-06-07 00:17:51.000000 pyobjc-framework-Intents-9.2/Lib/pyobjc_framework_Intents.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     2999 2023-06-07 00:17:51.000000 pyobjc-framework-Intents-9.2/Lib/pyobjc_framework_Intents.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:17:51.000000 pyobjc-framework-Intents-9.2/Lib/pyobjc_framework_Intents.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:21.000000 pyobjc-framework-Intents-9.2/Lib/pyobjc_framework_Intents.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:17:51.000000 pyobjc-framework-Intents-9.2/Lib/pyobjc_framework_Intents.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        8 2023-06-07 00:17:51.000000 pyobjc-framework-Intents-9.2/Lib/pyobjc_framework_Intents.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Intents-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Intents-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:51.766160 pyobjc-framework-Intents-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      806 2021-10-18 19:38:40.000000 pyobjc-framework-Intents-9.2/Modules/_Intents.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1162 2022-12-17 13:23:18.000000 pyobjc-framework-Intents-9.2/Modules/_Intents_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:33.000000 pyobjc-framework-Intents-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-05-29 07:18:42.000000 pyobjc-framework-Intents-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1887 2023-06-07 00:17:51.917806 pyobjc-framework-Intents-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:51.830337 pyobjc-framework-Intents-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-Intents-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      797 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inaddmediaintentresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)      703 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inanswercallintent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      817 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inanswercallintentresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)      296 2021-07-30 09:00:38.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inbooleanresolutionresult.py
+-rw-r--r--   0 ronald     (501) staff       (20)      428 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_incallaudioroute.py
+-rw-r--r--   0 ronald     (501) staff       (20)      445 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_incallcapability.py
+-rw-r--r--   0 ronald     (501) staff       (20)      420 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_incallcapabilityoptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1621 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_incalldestinationtype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      264 2021-07-30 09:00:38.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_incallrecordresolutionresult.py
+-rw-r--r--   0 ronald     (501) staff       (20)      935 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_incallrecordtype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      852 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_incallrecordtypeoptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)      455 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inconditionaloperator.py
+-rw-r--r--   0 ronald     (501) staff       (20)      258 2022-01-02 11:04:26.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_infile.py
+-rw-r--r--   0 ronald     (501) staff       (20)      819 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_infocusstatuscenter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      859 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_ingetreservationdetailsintentresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)      703 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inhangUpcallintent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      825 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inhangupcallintentresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2828 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inintenterrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1068 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inintentidentifiers.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1651 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_ininteraction.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1834 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inmessage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      643 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inmessageattributeoptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)      340 2021-07-30 09:00:38.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inobjectcollection.py
+-rw-r--r--   0 ronald     (501) staff       (20)      451 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inoutgoingmessagetype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      237 2021-03-21 10:08:22.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inparameter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      709 2021-03-21 10:08:22.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inpaymentmethodtypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      599 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inperson.py
+-rw-r--r--   0 ronald     (501) staff       (20)      354 2021-03-21 10:08:22.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inperson_siriadditions.py
+-rw-r--r--   0 ronald     (501) staff       (20)      456 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inpersonhandle.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1025 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inpersonhandlelabel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1261 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inpersonrelationship.py
+-rw-r--r--   0 ronald     (501) staff       (20)      724 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inrecurrencefrequency.py
+-rw-r--r--   0 ronald     (501) staff       (20)      368 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inreservationactiontype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      544 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inreservationstatus.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2351 2022-06-25 20:14:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_insearchcallhistoryintent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1062 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_insearchcallhistoryintentresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3430 2022-06-25 20:06:29.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_insearchformessagesintent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1101 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_insearchformessagesintentresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2753 2022-06-25 20:14:45.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_insendmessageintent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      909 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_insendmessageintentresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)      931 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_insendmessagerecipientresolutionresult.py
+-rw-r--r--   0 ronald     (501) staff       (20)      798 2022-06-25 20:16:06.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_insharefocusstatusintent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      785 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_insharefocusstatusintentresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)      230 2022-06-25 20:13:22.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inspeakable.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1362 2022-06-25 20:08:54.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_instartaudiocallintent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1237 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_instartaudiocallintentresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1695 2022-06-25 20:16:53.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_instartcallintent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1066 2022-06-25 20:11:43.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_instartvideocallintent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1237 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_instartvideocallintentresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)      198 2022-04-11 08:03:15.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_intents.py
+-rw-r--r--   0 ronald     (501) staff       (20)      366 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/PyObjCTest/test_inticketedeventcategory.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:51.831725 pyobjc-framework-Intents-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    30300 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/metadata/Intents.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       30 2020-11-30 18:45:15.000000 pyobjc-framework-Intents-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:51.890073 pyobjc-framework-Intents-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   930893 2022-01-02 11:04:26.000000 pyobjc-framework-Intents-9.2/metadata/raw/arm64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   939566 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   961877 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.2/metadata/raw/arm64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   961882 2023-02-19 10:50:35.000000 pyobjc-framework-Intents-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   774867 2020-11-30 18:45:15.000000 pyobjc-framework-Intents-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   907461 2021-03-21 10:08:22.000000 pyobjc-framework-Intents-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   930917 2022-01-02 11:04:26.000000 pyobjc-framework-Intents-9.2/metadata/raw/x86_64-12.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   939590 2022-02-24 08:47:16.000000 pyobjc-framework-Intents-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   961901 2022-12-16 16:43:02.000000 pyobjc-framework-Intents-9.2/metadata/raw/x86_64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   961906 2023-02-19 10:50:35.000000 pyobjc-framework-Intents-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Intents-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Intents-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:17:51.918801 pyobjc-framework-Intents-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1191 2023-05-29 10:07:46.000000 pyobjc-framework-Intents-9.2/setup.py
```

### Comparing `pyobjc-framework-Intents-9.1b1/Lib/Intents/__init__.py` & `pyobjc-framework-Intents-9.2/Lib/Intents/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/Lib/Intents/_metadata.py` & `pyobjc-framework-Intents-9.2/Lib/Intents/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/Lib/pyobjc_framework_Intents.egg-info/PKG-INFO` & `pyobjc-framework-Intents-9.2/Lib/pyobjc_framework_Intents.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Intents
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Intents on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Intents
 Platform: MacOS X (>=10.12)
```

### Comparing `pyobjc-framework-Intents-9.1b1/Lib/pyobjc_framework_Intents.egg-info/SOURCES.txt` & `pyobjc-framework-Intents-9.2/Lib/pyobjc_framework_Intents.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/Intents/__init__.py
 Lib/Intents/_metadata.py
 Lib/pyobjc_framework_Intents.egg-info/PKG-INFO
 Lib/pyobjc_framework_Intents.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Intents.egg-info/dependency_links.txt
 Lib/pyobjc_framework_Intents.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-Intents-9.1b1/License.txt` & `pyobjc-framework-Intents-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/Modules/_Intents.m` & `pyobjc-framework-Intents-9.2/Modules/_Intents.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/Modules/_Intents_protocols.m` & `pyobjc-framework-Intents-9.2/Modules/_Intents_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-Intents-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-Intents-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-Intents-9.1b1/PKG-INFO` & `pyobjc-framework-Intents-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Intents
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Intents on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Intents
 Platform: MacOS X (>=10.12)
```

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inaddmediaintentresponse.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inaddmediaintentresponse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inanswercallintent.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inanswercallintent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inanswercallintentresponse.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inanswercallintentresponse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_incalldestinationtype.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_incalldestinationtype.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_incallrecordtype.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_incallrecordtype.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_incallrecordtypeoptions.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_incallrecordtypeoptions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_infocusstatuscenter.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_infocusstatuscenter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_ingetreservationdetailsintentresponse.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_ingetreservationdetailsintentresponse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inhangUpcallintent.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inhangUpcallintent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inhangupcallintentresponse.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inhangupcallintentresponse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inintenterrors.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inintenterrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inintentidentifiers.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inintentidentifiers.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_ininteraction.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_ininteraction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inmessage.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inmessage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inmessageattributeoptions.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inmessageattributeoptions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inpaymentmethodtypes.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inpaymentmethodtypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inperson.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inperson.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inpersonhandlelabel.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inpersonhandlelabel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inpersonrelationship.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inpersonrelationship.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inrecurrencefrequency.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inrecurrencefrequency.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_inreservationstatus.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_inreservationstatus.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insearchcallhistoryintent.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_insearchcallhistoryintent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insearchcallhistoryintentresponse.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_insearchcallhistoryintentresponse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insearchformessagesintent.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_insearchformessagesintent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insearchformessagesintentresponse.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_insearchformessagesintentresponse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insendmessageintent.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_insendmessageintent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insendmessageintentresponse.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_insendmessageintentresponse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insendmessagerecipientresolutionresult.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_insendmessagerecipientresolutionresult.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insharefocusstatusintent.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_insharefocusstatusintent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_insharefocusstatusintentresponse.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_insharefocusstatusintentresponse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_instartaudiocallintent.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_instartaudiocallintent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_instartaudiocallintentresponse.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_instartaudiocallintentresponse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_instartcallintent.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_instartcallintent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_instartvideocallintent.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_instartvideocallintent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/PyObjCTest/test_instartvideocallintentresponse.py` & `pyobjc-framework-Intents-9.2/PyObjCTest/test_instartvideocallintentresponse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/metadata/Intents.fwinfo` & `pyobjc-framework-Intents-9.2/metadata/Intents.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/metadata/raw/arm64-12.1.fwinfo` & `pyobjc-framework-Intents-9.2/metadata/raw/arm64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Intents-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/metadata/raw/arm64-13.1.fwinfo` & `pyobjc-framework-Intents-9.2/metadata/raw/arm64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-Intents-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-Intents-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-Intents-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/metadata/raw/x86_64-12.1.fwinfo` & `pyobjc-framework-Intents-9.2/metadata/raw/x86_64-12.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Intents-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/metadata/raw/x86_64-13.1.fwinfo` & `pyobjc-framework-Intents-9.2/metadata/raw/x86_64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-Intents-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Intents-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Intents-9.1b1/setup.py` & `pyobjc-framework-Intents-9.2/setup.py`

 * *Files 10% similar despite different names*

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
     name="pyobjc-framework-Intents",
     description="Wrappers for the framework Intents on macOS",
     min_os_level="10.12",
     packages=["Intents"],
     ext_modules=[
```

