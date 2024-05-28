# Comparing `tmp/pyobjc-framework-Virtualization-9.1b1.tar.gz` & `tmp/pyobjc-framework-Virtualization-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Virtualization-9.1b1.tar", last modified: Sun Mar 26 11:43:41 2023, max compression
+gzip compressed data, was "pyobjc-framework-Virtualization-9.2.tar", last modified: Wed Jun  7 00:31:28 2023, max compression
```

## Comparing `pyobjc-framework-Virtualization-9.1b1.tar` & `pyobjc-framework-Virtualization-9.2.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:41.296071 pyobjc-framework-Virtualization-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:41.228473 pyobjc-framework-Virtualization-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:41.234501 pyobjc-framework-Virtualization-9.1b1/Lib/Virtualization/
--rw-r--r--   0 ronald     (501) staff       (20)      790 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.1b1/Lib/Virtualization/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    12311 2022-07-08 16:02:54.000000 pyobjc-framework-Virtualization-9.1b1/Lib/Virtualization/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:41.237738 pyobjc-framework-Virtualization-9.1b1/Lib/pyobjc_framework_Virtualization.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2128 2023-03-26 11:43:41.000000 pyobjc-framework-Virtualization-9.1b1/Lib/pyobjc_framework_Virtualization.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1934 2023-03-26 11:43:41.000000 pyobjc-framework-Virtualization-9.1b1/Lib/pyobjc_framework_Virtualization.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:43:41.000000 pyobjc-framework-Virtualization-9.1b1/Lib/pyobjc_framework_Virtualization.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:52:21.000000 pyobjc-framework-Virtualization-9.1b1/Lib/pyobjc_framework_Virtualization.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:43:41.000000 pyobjc-framework-Virtualization-9.1b1/Lib/pyobjc_framework_Virtualization.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       15 2023-03-26 11:43:41.000000 pyobjc-framework-Virtualization-9.1b1/Lib/pyobjc_framework_Virtualization.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Virtualization-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:41.240820 pyobjc-framework-Virtualization-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1105 2021-10-18 19:38:40.000000 pyobjc-framework-Virtualization-9.1b1/Modules/_Virtualization.m
--rw-r--r--   0 ronald     (501) staff       (20)      547 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.1b1/Modules/_Virtualization_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-Virtualization-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-Virtualization-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1917 2023-03-26 11:43:41.295056 pyobjc-framework-Virtualization-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:41.262924 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      212 2022-04-11 08:03:15.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_virtualization.py
--rw-r--r--   0 ronald     (501) staff       (20)     1661 2022-02-24 08:47:17.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzdiskimagestoragedeviceattachment.py
--rw-r--r--   0 ronald     (501) staff       (20)      570 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzefivariablestore.py
--rw-r--r--   0 ronald     (501) staff       (20)     1418 2022-07-08 16:02:54.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      474 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzfileserialportattachment.py
--rw-r--r--   0 ronald     (501) staff       (20)      834 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzlinuxrosettadirectoryshare.py
--rw-r--r--   0 ronald     (501) staff       (20)      598 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzmacaddress.py
--rw-r--r--   0 ronald     (501) staff       (20)      669 2022-02-24 08:47:17.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzmacauxiliarystorage.py
--rw-r--r--   0 ronald     (501) staff       (20)      292 2021-07-30 17:45:16.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzmachardwaremodel.py
--rw-r--r--   0 ronald     (501) staff       (20)      336 2021-07-30 17:33:52.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzmacosinstaller.py
--rw-r--r--   0 ronald     (501) staff       (20)      700 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzmacosrestoreimage.py
--rw-r--r--   0 ronald     (501) staff       (20)      507 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzmacosvirtualmachinestartoptions.py
--rw-r--r--   0 ronald     (501) staff       (20)      413 2021-07-30 09:00:38.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzmultipledirectoryshare.py
--rw-r--r--   0 ronald     (501) staff       (20)      342 2021-07-30 09:00:38.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzshareddirectory.py
--rw-r--r--   0 ronald     (501) staff       (20)      455 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzspiceagentportattachment.py
--rw-r--r--   0 ronald     (501) staff       (20)      489 2022-02-24 08:47:17.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzvirtioblockdeviceconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      461 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzvirtioconsoleportconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      450 2021-07-30 09:00:38.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzvirtiofilesystemdeviceconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      542 2022-10-18 09:53:23.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzvirtiosocketListener.py
--rw-r--r--   0 ronald     (501) staff       (20)      298 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzvirtiosocketdevice.py
--rw-r--r--   0 ronald     (501) staff       (20)     2260 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzvirtualmachine.py
--rw-r--r--   0 ronald     (501) staff       (20)      386 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzvirtualmachineconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      221 2022-06-25 20:07:39.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzvirtualmachinedelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      418 2021-10-29 07:58:20.000000 pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzvirtualmachineview.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:41.273093 pyobjc-framework-Virtualization-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     1637 2021-08-15 08:47:00.000000 pyobjc-framework-Virtualization-9.1b1/metadata/Virtualization.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       44 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:43:41.292883 pyobjc-framework-Virtualization-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   101901 2021-08-04 10:01:04.000000 pyobjc-framework-Virtualization-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   105465 2022-02-24 08:47:17.000000 pyobjc-framework-Virtualization-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   136199 2022-07-08 16:02:54.000000 pyobjc-framework-Virtualization-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    52202 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.1b1/metadata/raw/x86_64-11.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    86513 2021-08-04 10:01:04.000000 pyobjc-framework-Virtualization-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    90004 2022-02-24 08:47:17.000000 pyobjc-framework-Virtualization-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   116834 2022-07-08 16:02:54.000000 pyobjc-framework-Virtualization-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Virtualization-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:43:41.296215 pyobjc-framework-Virtualization-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1182 2023-03-25 14:20:32.000000 pyobjc-framework-Virtualization-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:28.036163 pyobjc-framework-Virtualization-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:27.955709 pyobjc-framework-Virtualization-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:27.960975 pyobjc-framework-Virtualization-9.2/Lib/Virtualization/
+-rw-r--r--   0 ronald     (501) staff       (20)      790 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.2/Lib/Virtualization/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12311 2022-07-08 16:02:54.000000 pyobjc-framework-Virtualization-9.2/Lib/Virtualization/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:27.965136 pyobjc-framework-Virtualization-9.2/Lib/pyobjc_framework_Virtualization.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2126 2023-06-07 00:31:27.000000 pyobjc-framework-Virtualization-9.2/Lib/pyobjc_framework_Virtualization.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1949 2023-06-07 00:31:27.000000 pyobjc-framework-Virtualization-9.2/Lib/pyobjc_framework_Virtualization.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:31:27.000000 pyobjc-framework-Virtualization-9.2/Lib/pyobjc_framework_Virtualization.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:52:21.000000 pyobjc-framework-Virtualization-9.2/Lib/pyobjc_framework_Virtualization.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:31:27.000000 pyobjc-framework-Virtualization-9.2/Lib/pyobjc_framework_Virtualization.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       15 2023-06-07 00:31:27.000000 pyobjc-framework-Virtualization-9.2/Lib/pyobjc_framework_Virtualization.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Virtualization-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:27.978776 pyobjc-framework-Virtualization-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1105 2021-10-18 19:38:40.000000 pyobjc-framework-Virtualization-9.2/Modules/_Virtualization.m
+-rw-r--r--   0 ronald     (501) staff       (20)      547 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.2/Modules/_Virtualization_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-Virtualization-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-Virtualization-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1915 2023-06-07 00:31:28.035751 pyobjc-framework-Virtualization-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:28.006387 pyobjc-framework-Virtualization-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      212 2022-04-11 08:03:15.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_virtualization.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1661 2022-02-24 08:47:17.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzdiskimagestoragedeviceattachment.py
+-rw-r--r--   0 ronald     (501) staff       (20)      570 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzefivariablestore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1418 2022-07-08 16:02:54.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      474 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzfileserialportattachment.py
+-rw-r--r--   0 ronald     (501) staff       (20)      859 2023-05-27 09:46:33.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzlinuxrosettadirectoryshare.py
+-rw-r--r--   0 ronald     (501) staff       (20)      598 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzmacaddress.py
+-rw-r--r--   0 ronald     (501) staff       (20)      669 2022-02-24 08:47:17.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzmacauxiliarystorage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      292 2021-07-30 17:45:16.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzmachardwaremodel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      336 2021-07-30 17:33:52.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzmacosinstaller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      700 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzmacosrestoreimage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      507 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzmacosvirtualmachinestartoptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)      413 2021-07-30 09:00:38.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzmultipledirectoryshare.py
+-rw-r--r--   0 ronald     (501) staff       (20)      342 2021-07-30 09:00:38.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzshareddirectory.py
+-rw-r--r--   0 ronald     (501) staff       (20)      455 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzspiceagentportattachment.py
+-rw-r--r--   0 ronald     (501) staff       (20)      489 2022-02-24 08:47:17.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzvirtioblockdeviceconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      461 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzvirtioconsoleportconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      450 2021-07-30 09:00:38.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzvirtiofilesystemdeviceconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      542 2022-10-18 09:53:23.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzvirtiosocketListener.py
+-rw-r--r--   0 ronald     (501) staff       (20)      298 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzvirtiosocketdevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2260 2022-06-15 11:57:00.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzvirtualmachine.py
+-rw-r--r--   0 ronald     (501) staff       (20)      386 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzvirtualmachineconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      221 2022-06-25 20:07:39.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzvirtualmachinedelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      418 2021-10-29 07:58:20.000000 pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzvirtualmachineview.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:28.008255 pyobjc-framework-Virtualization-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     1637 2021-08-15 08:47:00.000000 pyobjc-framework-Virtualization-9.2/metadata/Virtualization.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       44 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:31:28.034215 pyobjc-framework-Virtualization-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   101901 2021-08-04 10:01:04.000000 pyobjc-framework-Virtualization-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   105465 2022-02-24 08:47:17.000000 pyobjc-framework-Virtualization-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   136199 2022-07-08 16:02:54.000000 pyobjc-framework-Virtualization-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    52202 2021-03-21 10:08:23.000000 pyobjc-framework-Virtualization-9.2/metadata/raw/x86_64-11.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    86513 2021-08-04 10:01:04.000000 pyobjc-framework-Virtualization-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    90004 2022-02-24 08:47:17.000000 pyobjc-framework-Virtualization-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   116834 2022-07-08 16:02:54.000000 pyobjc-framework-Virtualization-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Virtualization-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Virtualization-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:31:28.036256 pyobjc-framework-Virtualization-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1253 2023-05-29 10:07:47.000000 pyobjc-framework-Virtualization-9.2/setup.py
```

### Comparing `pyobjc-framework-Virtualization-9.1b1/Lib/Virtualization/__init__.py` & `pyobjc-framework-Virtualization-9.2/Lib/Virtualization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/Lib/Virtualization/_metadata.py` & `pyobjc-framework-Virtualization-9.2/Lib/Virtualization/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/Lib/pyobjc_framework_Virtualization.egg-info/PKG-INFO` & `pyobjc-framework-Virtualization-9.2/Lib/pyobjc_framework_Virtualization.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Virtualization
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Virtualization on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Virtualization
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-Virtualization-9.1b1/Lib/pyobjc_framework_Virtualization.egg-info/SOURCES.txt` & `pyobjc-framework-Virtualization-9.2/Lib/pyobjc_framework_Virtualization.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/Virtualization/__init__.py
 Lib/Virtualization/_metadata.py
 Lib/pyobjc_framework_Virtualization.egg-info/PKG-INFO
 Lib/pyobjc_framework_Virtualization.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Virtualization.egg-info/dependency_links.txt
 Lib/pyobjc_framework_Virtualization.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-Virtualization-9.1b1/License.txt` & `pyobjc-framework-Virtualization-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/Modules/_Virtualization.m` & `pyobjc-framework-Virtualization-9.2/Modules/_Virtualization.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/Modules/_Virtualization_protocols.m` & `pyobjc-framework-Virtualization-9.2/Modules/_Virtualization_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-Virtualization-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-Virtualization-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-Virtualization-9.1b1/PKG-INFO` & `pyobjc-framework-Virtualization-9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Virtualization
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Virtualization on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Virtualization
 Platform: MacOS X (>=10.16)
```

### Comparing `pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzdiskimagestoragedeviceattachment.py` & `pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzdiskimagestoragedeviceattachment.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzefivariablestore.py` & `pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzefivariablestore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzerror.py` & `pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzlinuxrosettadirectoryshare.py` & `pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzlinuxrosettadirectoryshare.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,13 +9,15 @@
         self.assertEqual(Virtualization.VZLinuxRosettaAvailabilityNotSupported, 0)
         self.assertEqual(Virtualization.VZLinuxRosettaAvailabilityNotInstalled, 1)
         self.assertEqual(Virtualization.VZLinuxRosettaAvailabilityInstalled, 2)
 
     @min_os_level("13.0")
     @arch_only("arm64")
     def test_methods13_0(self):
-        self.assertArgIsOut(Virtualization.VZLinuxRosettaDirectoryShare.initWithError_)
+        self.assertArgIsOut(
+            Virtualization.VZLinuxRosettaDirectoryShare.initWithError_, 0
+        )
         self.assertArgIsBlock(
             Virtualization.VZLinuxRosettaDirectoryShare.installRosettaWithCompletionHandler_,
             0,
             b"v@",
         )
```

### Comparing `pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzmacaddress.py` & `pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzmacaddress.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzmacauxiliarystorage.py` & `pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzmacauxiliarystorage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzmacosrestoreimage.py` & `pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzmacosrestoreimage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzvirtiosocketListener.py` & `pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzvirtiosocketListener.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/PyObjCTest/test_vzvirtualmachine.py` & `pyobjc-framework-Virtualization-9.2/PyObjCTest/test_vzvirtualmachine.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/metadata/Virtualization.fwinfo` & `pyobjc-framework-Virtualization-9.2/metadata/Virtualization.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-Virtualization-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Virtualization-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-Virtualization-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/metadata/raw/x86_64-11.0.fwinfo` & `pyobjc-framework-Virtualization-9.2/metadata/raw/x86_64-11.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-Virtualization-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Virtualization-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-Virtualization-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Virtualization-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Virtualization-9.1b1/setup.py` & `pyobjc-framework-Virtualization-9.2/setup.py`

 * *Files 8% similar despite different names*

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
     name="pyobjc-framework-Virtualization",
     description="Wrappers for the framework Virtualization on macOS",
     min_os_level="10.16",
     packages=["Virtualization"],
     ext_modules=[
```

