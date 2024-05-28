# Comparing `tmp/pyobjc-framework-ApplicationServices-9.1b1.tar.gz` & `tmp/pyobjc-framework-ApplicationServices-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-ApplicationServices-9.1b1.tar", last modified: Sun Mar 26 11:14:28 2023, max compression
+gzip compressed data, was "pyobjc-framework-ApplicationServices-9.2.tar", last modified: Wed Jun  7 00:06:06 2023, max compression
```

## Comparing `pyobjc-framework-ApplicationServices-9.1b1.tar` & `pyobjc-framework-ApplicationServices-9.2.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:28.913324 pyobjc-framework-ApplicationServices-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:28.672882 pyobjc-framework-ApplicationServices-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:28.693660 pyobjc-framework-ApplicationServices-9.1b1/Lib/ApplicationServices/
--rw-r--r--   0 ronald     (501) staff       (20)      877 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/Lib/ApplicationServices/__init__.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:28.695317 pyobjc-framework-ApplicationServices-9.1b1/Lib/HIServices/
--rw-r--r--   0 ronald     (501) staff       (20)      757 2021-06-05 10:25:38.000000 pyobjc-framework-ApplicationServices-9.1b1/Lib/HIServices/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    47348 2022-04-11 08:03:15.000000 pyobjc-framework-ApplicationServices-9.1b1/Lib/HIServices/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:28.697575 pyobjc-framework-ApplicationServices-9.1b1/Lib/PrintCore/
--rw-r--r--   0 ronald     (501) staff       (20)     1256 2022-06-25 20:05:00.000000 pyobjc-framework-ApplicationServices-9.1b1/Lib/PrintCore/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    38273 2022-04-11 15:12:57.000000 pyobjc-framework-ApplicationServices-9.1b1/Lib/PrintCore/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:28.758459 pyobjc-framework-ApplicationServices-9.1b1/Lib/pyobjc_framework_ApplicationServices.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2313 2023-03-26 11:14:28.000000 pyobjc-framework-ApplicationServices-9.1b1/Lib/pyobjc_framework_ApplicationServices.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     2149 2023-03-26 11:14:28.000000 pyobjc-framework-ApplicationServices-9.1b1/Lib/pyobjc_framework_ApplicationServices.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:14:28.000000 pyobjc-framework-ApplicationServices-9.1b1/Lib/pyobjc_framework_ApplicationServices.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:08.000000 pyobjc-framework-ApplicationServices-9.1b1/Lib/pyobjc_framework_ApplicationServices.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       80 2023-03-26 11:14:28.000000 pyobjc-framework-ApplicationServices-9.1b1/Lib/pyobjc_framework_ApplicationServices.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       41 2023-03-26 11:14:28.000000 pyobjc-framework-ApplicationServices-9.1b1/Lib/pyobjc_framework_ApplicationServices.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ApplicationServices-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:28.763361 pyobjc-framework-ApplicationServices-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     5509 2021-10-28 09:35:32.000000 pyobjc-framework-ApplicationServices-9.1b1/Modules/_HIServices.m
--rw-r--r--   0 ronald     (501) staff       (20)      837 2022-06-24 14:42:41.000000 pyobjc-framework-ApplicationServices-9.1b1/Modules/_PrintCore.m
--rw-r--r--   0 ronald     (501) staff       (20)      398 2022-06-24 14:45:57.000000 pyobjc-framework-ApplicationServices-9.1b1/Modules/_PrintCore_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-ApplicationServices-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-ApplicationServices-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2102 2023-03-26 11:14:28.912902 pyobjc-framework-ApplicationServices-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:28.833390 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      757 2022-04-12 20:05:08.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_applicationservices.py
--rw-r--r--   0 ronald     (501) staff       (20)      825 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axactionconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)    13775 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axattributeconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)     1272 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axerror.py
--rw-r--r--   0 ronald     (501) staff       (20)     4268 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axnotificationconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)     7039 2021-10-26 11:32:35.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axroleconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)     2079 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axtextattributedstring.py
--rw-r--r--   0 ronald     (501) staff       (20)     5602 2021-10-25 15:33:38.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axuielement.py
--rw-r--r--   0 ronald     (501) staff       (20)     5138 2021-06-05 10:25:38.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axvalue.py
--rw-r--r--   0 ronald     (501) staff       (20)      801 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axvalueconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)     3065 2021-03-21 10:08:22.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_hishape.py
--rw-r--r--   0 ronald     (501) staff       (20)     1806 2022-06-25 20:10:11.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pdeplugininterface.py
--rw-r--r--   0 ronald     (501) staff       (20)     9816 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pmcore.py
--rw-r--r--   0 ronald     (501) staff       (20)     8442 2022-01-02 11:04:26.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pmdefinitions.py
--rw-r--r--   0 ronald     (501) staff       (20)     6078 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pmerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)     3517 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pmprintaetypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     4602 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pmprintingdialogextensions.py
--rw-r--r--   0 ronald     (501) staff       (20)    13667 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pmprintsettingskeys.py
--rw-r--r--   0 ronald     (501) staff       (20)      427 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_printcore.py
--rw-r--r--   0 ronald     (501) staff       (20)     1769 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_translationservicse.py
--rw-r--r--   0 ronald     (501) staff       (20)      473 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_universalaccess.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:28.842332 pyobjc-framework-ApplicationServices-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    23617 2022-04-11 08:03:15.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/HIServices.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22747 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/HIServices.fwinfo.sv
--rw-r--r--   0 ronald     (501) staff       (20)    26737 2022-06-15 11:57:00.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/PrintCore.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      300 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:28.903806 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/
--rw-r--r--   0 ronald     (501) staff       (20)   103372 2021-10-26 11:32:35.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   103897 2022-02-24 08:47:16.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    96594 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   100698 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   100690 2021-03-21 10:08:22.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   103373 2021-10-26 11:32:35.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   103898 2022-02-24 08:47:16.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/x86_64-12.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:28.911912 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/
--rw-r--r--   0 ronald     (501) staff       (20)    51933 2021-07-30 09:00:37.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    51997 2022-02-24 08:47:16.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    51307 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    51280 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    51934 2021-03-21 10:08:22.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    51934 2021-07-30 09:00:37.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    51998 2022-02-24 08:47:16.000000 pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ApplicationServices-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:14:28.913428 pyobjc-framework-ApplicationServices-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1740 2023-03-25 14:20:30.000000 pyobjc-framework-ApplicationServices-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:06.019544 pyobjc-framework-ApplicationServices-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:05.902809 pyobjc-framework-ApplicationServices-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:05.907656 pyobjc-framework-ApplicationServices-9.2/Lib/ApplicationServices/
+-rw-r--r--   0 ronald     (501) staff       (20)      877 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/Lib/ApplicationServices/__init__.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:05.913027 pyobjc-framework-ApplicationServices-9.2/Lib/HIServices/
+-rw-r--r--   0 ronald     (501) staff       (20)      757 2021-06-05 10:25:38.000000 pyobjc-framework-ApplicationServices-9.2/Lib/HIServices/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    49361 2023-05-27 09:46:33.000000 pyobjc-framework-ApplicationServices-9.2/Lib/HIServices/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:05.916170 pyobjc-framework-ApplicationServices-9.2/Lib/PrintCore/
+-rw-r--r--   0 ronald     (501) staff       (20)     1256 2022-06-25 20:05:00.000000 pyobjc-framework-ApplicationServices-9.2/Lib/PrintCore/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    38337 2023-05-27 09:46:33.000000 pyobjc-framework-ApplicationServices-9.2/Lib/PrintCore/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:05.920312 pyobjc-framework-ApplicationServices-9.2/Lib/pyobjc_framework_ApplicationServices.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2311 2023-06-07 00:06:05.000000 pyobjc-framework-ApplicationServices-9.2/Lib/pyobjc_framework_ApplicationServices.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     2164 2023-06-07 00:06:05.000000 pyobjc-framework-ApplicationServices-9.2/Lib/pyobjc_framework_ApplicationServices.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:06:05.000000 pyobjc-framework-ApplicationServices-9.2/Lib/pyobjc_framework_ApplicationServices.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:08.000000 pyobjc-framework-ApplicationServices-9.2/Lib/pyobjc_framework_ApplicationServices.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       74 2023-06-07 00:06:05.000000 pyobjc-framework-ApplicationServices-9.2/Lib/pyobjc_framework_ApplicationServices.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       41 2023-06-07 00:06:05.000000 pyobjc-framework-ApplicationServices-9.2/Lib/pyobjc_framework_ApplicationServices.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-ApplicationServices-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:05.935614 pyobjc-framework-ApplicationServices-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     5509 2021-10-28 09:35:32.000000 pyobjc-framework-ApplicationServices-9.2/Modules/_HIServices.m
+-rw-r--r--   0 ronald     (501) staff       (20)      837 2022-06-24 14:42:41.000000 pyobjc-framework-ApplicationServices-9.2/Modules/_PrintCore.m
+-rw-r--r--   0 ronald     (501) staff       (20)      398 2022-06-24 14:45:57.000000 pyobjc-framework-ApplicationServices-9.2/Modules/_PrintCore_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-ApplicationServices-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:21.000000 pyobjc-framework-ApplicationServices-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2100 2023-06-07 00:06:06.018765 pyobjc-framework-ApplicationServices-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:05.968400 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      757 2022-04-12 20:05:08.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_applicationservices.py
+-rw-r--r--   0 ronald     (501) staff       (20)      825 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axactionconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13775 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axattributeconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1272 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4268 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axnotificationconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7039 2021-10-26 11:32:35.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axroleconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2079 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axtextattributedstring.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5602 2021-10-25 15:33:38.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axuielement.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5138 2021-06-05 10:25:38.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axvalue.py
+-rw-r--r--   0 ronald     (501) staff       (20)      801 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axvalueconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3065 2021-03-21 10:08:22.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_hishape.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1728 2023-05-27 09:46:33.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pdeplugininterface.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9816 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pmcore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8442 2022-01-02 11:04:26.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pmdefinitions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6078 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pmerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3517 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pmprintaetypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4602 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pmprintingdialogextensions.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13667 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pmprintsettingskeys.py
+-rw-r--r--   0 ronald     (501) staff       (20)      427 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_printcore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1769 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_translationservicse.py
+-rw-r--r--   0 ronald     (501) staff       (20)      473 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_universalaccess.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:05.976597 pyobjc-framework-ApplicationServices-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    24951 2023-05-27 09:46:33.000000 pyobjc-framework-ApplicationServices-9.2/metadata/HIServices.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22747 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/metadata/HIServices.fwinfo.sv
+-rw-r--r--   0 ronald     (501) staff       (20)    26758 2023-05-27 09:46:33.000000 pyobjc-framework-ApplicationServices-9.2/metadata/PrintCore.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      300 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:06.000369 pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/
+-rw-r--r--   0 ronald     (501) staff       (20)   103372 2021-10-26 11:32:35.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   103897 2022-02-24 08:47:16.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    96594 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   100698 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   100690 2021-03-21 10:08:22.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   103373 2021-10-26 11:32:35.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   103898 2022-02-24 08:47:16.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/x86_64-12.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:06.017358 pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/
+-rw-r--r--   0 ronald     (501) staff       (20)    51933 2021-07-30 09:00:37.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    51997 2022-02-24 08:47:16.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    51307 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    51280 2020-11-30 18:45:14.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    51934 2021-03-21 10:08:22.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    51934 2021-07-30 09:00:37.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    51998 2022-02-24 08:47:16.000000 pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-ApplicationServices-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-ApplicationServices-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:06:06.019647 pyobjc-framework-ApplicationServices-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1811 2023-05-29 10:07:45.000000 pyobjc-framework-ApplicationServices-9.2/setup.py
```

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/Lib/ApplicationServices/__init__.py` & `pyobjc-framework-ApplicationServices-9.2/Lib/ApplicationServices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/Lib/HIServices/__init__.py` & `pyobjc-framework-ApplicationServices-9.2/Lib/HIServices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/Lib/HIServices/_metadata.py` & `pyobjc-framework-ApplicationServices-9.2/Lib/HIServices/_metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Mar 11 13:04:50 2022
+# Last update: Sat May 20 09:54:44 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -73,14 +73,19 @@
                 "processFreeMem",
                 "processLauncher",
                 "processLaunchDate",
                 "processActiveTime",
                 "processAppRef",
             ],
         ),
+        "ProcessSerialNumber": objc.createStructType(
+            "HIServices.ProcessSerialNumber",
+            b"{ProcessSerialNumber=II}",
+            ["highLongOfPSN", "lowLongOfPSN"],
+        ),
     }
 )
 constants = """$kAXAttachmentTextAttribute$kAXAutocorrectedTextAttribute$kAXBackgroundColorTextAttribute$kAXFontFamilyKey$kAXFontNameKey$kAXFontSizeKey$kAXFontTextAttribute$kAXForegoundColorTextAttribute$kAXForegroundColorTextAttribute$kAXLinkTextAttribute$kAXListItemIndexTextAttribute$kAXListItemLevelTextAttribute$kAXListItemPrefixTextAttribute$kAXMarkedMisspelledTextAttribute$kAXMisspelledTextAttribute$kAXNaturalLanguageTextAttribute$kAXReplacementStringTextAttribute$kAXShadowTextAttribute$kAXStrikethroughColorTextAttribute$kAXStrikethroughTextAttribute$kAXSuperscriptTextAttribute$kAXTrustedCheckOptionPrompt$kAXUnderlineColorTextAttribute$kAXUnderlineTextAttribute$kAXVisibleNameKey$"""
 enums = """$AX_ALLOW_OLD_SECURITY_METHOD@0$activDev@5$atAbsoluteCenter@5$atBottom@3$atBottomLeft@11$atBottomRight@15$atCenterBottom@7$atCenterLeft@9$atCenterRight@13$atCenterTop@6$atHorizontalCenter@4$atLeft@8$atNone@0$atRight@12$atTop@2$atTopLeft@10$atTopRight@14$atVerticalCenter@1$badPasteboardFlavorErr@-25133$badPasteboardIndexErr@-25131$badPasteboardItemErr@-25132$badPasteboardSyncErr@-25130$badTranslationRefErr@-3031$cdevGenErr@-1$cdevMemErr@0$cdevResErr@1$cdevUnset@3$clearDev@13$closeDev@2$copyDev@11$cursorDev@14$cutDev@10$deactivDev@6$duplicatePasteboardFlavorErr@-25134$extendedBlock@19523$extendedBlockLen@40$hitDev@1$initDev@0$kAXCopyMultipleAttributeOptionStopOnError@1$kAXErrorAPIDisabled@-25211$kAXErrorActionUnsupported@-25206$kAXErrorAttributeUnsupported@-25205$kAXErrorCannotComplete@-25204$kAXErrorFailure@-25200$kAXErrorIllegalArgument@-25201$kAXErrorInvalidUIElement@-25202$kAXErrorInvalidUIElementObserver@-25203$kAXErrorNoValue@-25212$kAXErrorNotEnoughPrecision@-25214$kAXErrorNotImplemented@-25208$kAXErrorNotificationAlreadyRegistered@-25209$kAXErrorNotificationNotRegistered@-25210$kAXErrorNotificationUnsupported@-25207$kAXErrorParameterizedAttributeUnsupported@-25213$kAXErrorSuccess@0$kAXMenuItemModifierControl@4$kAXMenuItemModifierNoCommand@8$kAXMenuItemModifierNone@0$kAXMenuItemModifierOption@2$kAXMenuItemModifierShift@1$kAXPriorityHigh@90$kAXPriorityLow@10$kAXPriorityMedium@50$kAXUnderlineStyleDouble@9$kAXUnderlineStyleNone@0$kAXUnderlineStyleSingle@1$kAXUnderlineStyleThick@2$kAXValueAXErrorType@5$kAXValueCFRangeType@4$kAXValueCGPointType@1$kAXValueCGRectType@3$kAXValueCGSizeType@2$kAXValueIllegalType@0$kAXValueTypeAXError@5$kAXValueTypeCFRange@4$kAXValueTypeCGPoint@1$kAXValueTypeCGRect@3$kAXValueTypeCGSize@2$kAXValueTypeIllegal@0$kAlignAbsoluteCenter@5$kAlignBottom@3$kAlignBottomLeft@11$kAlignBottomRight@15$kAlignCenterBottom@7$kAlignCenterLeft@9$kAlignCenterRight@13$kAlignCenterTop@6$kAlignHorizontalCenter@4$kAlignLeft@8$kAlignNone@0$kAlignRight@12$kAlignTop@2$kAlignTopLeft@10$kAlignTopRight@14$kAlignVerticalCenter@1$kCurrentProcess@2$kHIShapeEnumerateInit@1$kHIShapeEnumerateRect@2$kHIShapeEnumerateTerminate@3$kHIShapeParseFromBottom@1$kHIShapeParseFromBottomRight@3$kHIShapeParseFromLeft@0$kHIShapeParseFromRight@2$kHIShapeParseFromTop@0$kHIShapeParseFromTopLeft@0$kNoProcess@0$kPasteboardClientIsOwner@2$kPasteboardFlavorNoFlags@0$kPasteboardFlavorNotSaved@4$kPasteboardFlavorPromised@512$kPasteboardFlavorRequestOnly@8$kPasteboardFlavorSenderOnly@1$kPasteboardFlavorSenderTranslated@2$kPasteboardFlavorSystemTranslated@256$kPasteboardModified@1$kPasteboardStandardLocationTrash@1953657704$kPasteboardStandardLocationUnknown@1970170734$kPlotIconRefNoImage@2$kPlotIconRefNoMask@4$kPlotIconRefNormalFlags@0$kProcessDictionaryIncludeAllInformationMask@-1$kProcessTransformToBackgroundApplication@2$kProcessTransformToForegroundApplication@1$kProcessTransformToUIElementApplication@4$kQuitAtNormalTimeMask@2$kQuitBeforeFBAsQuitMask@4$kQuitBeforeNormalTimeMask@1$kQuitBeforeShellQuitsMask@8$kQuitBeforeTerminatorAppQuitsMask@16$kQuitNeverMask@32$kQuitNotQuitDuringInstallMask@256$kQuitNotQuitDuringLogoutMask@512$kQuitOptionsMask@127$kSelectorAll1BitData@16843009$kSelectorAll32BitData@134219784$kSelectorAll4BitData@33686018$kSelectorAll8BitData@67372036$kSelectorAllAvailableData@4294967295$kSelectorAllHugeData@4278190080$kSelectorAllLargeData@255$kSelectorAllMiniData@16711680$kSelectorAllSmallData@65280$kSelectorHuge1Bit@16777216$kSelectorHuge32Bit@134217728$kSelectorHuge4Bit@33554432$kSelectorHuge8Bit@67108864$kSelectorHuge8BitMask@268435456$kSelectorLarge1Bit@1$kSelectorLarge32Bit@8$kSelectorLarge4Bit@2$kSelectorLarge8Bit@4$kSelectorLarge8BitMask@16$kSelectorMini1Bit@65536$kSelectorMini4Bit@131072$kSelectorMini8Bit@262144$kSelectorSmall1Bit@256$kSelectorSmall32Bit@2048$kSelectorSmall4Bit@512$kSelectorSmall8Bit@1024$kSelectorSmall8BitMask@4096$kSetFrontProcessCausedByUser@2$kSetFrontProcessFrontWindowOnly@1$kSystemProcess@1$kTransformDisabled@1$kTransformLabel1@256$kTransformLabel2@512$kTransformLabel3@768$kTransformLabel4@1024$kTransformLabel5@1280$kTransformLabel6@1536$kTransformLabel7@1792$kTransformNone@0$kTransformOffline@2$kTransformOpen@3$kTransformSelected@16384$kTransformSelectedDisabled@16385$kTransformSelectedOffline@16386$kTransformSelectedOpen@16387$kTranslationDataTranslation@1$kTranslationFileTranslation@2$kUAZoomFocusTypeInsertionPoint@1$kUAZoomFocusTypeOther@0$keyEvtDev@7$launchAllow24Bit@256$launchContinue@16384$launchDontSwitch@512$launchInhibitDaemon@128$launchNoFileFlags@2048$launchUseMinimum@1024$macDev@8$mode32BitCompatible@128$modeCanBackground@4096$modeControlPanel@524288$modeDeskAccessory@131072$modeDisplayManagerAware@4$modeDoesActivateOnFGSwitch@2048$modeGetAppDiedMsg@256$modeGetFrontClicks@512$modeHighLevelEventAware@64$modeLaunchDontSwitch@262144$modeLocalAndRemoteHLEvents@32$modeMultiLaunch@65536$modeNeedSuspendResume@16384$modeOnlyBackground@1024$modeReserved@16777216$modeStationeryAware@16$modeUseTextEditServices@8$noPasteboardPromiseKeeperErr@-25136$notPasteboardOwnerErr@-25135$nulDev@3$pasteDev@12$svAll1BitData@16843009$svAll4BitData@33686018$svAll8BitData@67372036$svAllAvailableData@4294967295$svAllLargeData@255$svAllMiniData@16711680$svAllSmallData@65280$svLarge1Bit@1$svLarge4Bit@2$svLarge8Bit@4$svMini1Bit@65536$svMini4Bit@131072$svMini8Bit@262144$svSmall1Bit@256$svSmall4Bit@512$svSmall8Bit@1024$ttDisabled@1$ttLabel1@256$ttLabel2@512$ttLabel3@768$ttLabel4@1024$ttLabel5@1280$ttLabel6@1536$ttLabel7@1792$ttNone@0$ttOffline@2$ttOpen@3$ttSelected@16384$ttSelectedDisabled@16385$ttSelectedOffline@16386$ttSelectedOpen@16387$undoDev@9$updateDev@4$"""
 misc.update(
     {
         "AXError": NewType("AXError", int),
@@ -438,44 +443,44 @@
         b"i^{OpaqueTranslationRef=}^^{__CFString=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {1: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
-    "GetIconFamilyData": (
-        b"s^^{IconFamilyResource=Ii[1{IconFamilyElement=Ii[1C]}]}I^^c",
-    ),
-    "IconRefIntersectsCGRect": (
-        b"Z^{CGRect={CGPoint=dd}{CGSize=dd}}^{CGRect={CGPoint=dd}{CGSize=dd}}sI^{OpaqueIconRef=}",
-    ),
     "HIShapeCreateMutableWithRect": (
         b"^{__HIShape=}^{CGRect={CGPoint=dd}{CGSize=dd}}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {0: {"type_modifier": "n"}},
         },
     ),
     "PlotIconRefInContext": (
         b"i^{CGContext=}^{CGRect={CGPoint=dd}{CGSize=dd}}ss^{RGBColor=SSS}I^{OpaqueIconRef=}",
+        "",
+        {"arguments": {1: {"type_modifier": "n"}, 4: {"type_modifier": "n"}}},
     ),
     "AXUIElementPerformAction": (b"i^{__AXUIElement=}^{__CFString=}",),
     "AXUIElementPostKeyboardEvent": (b"i^{__AXUIElement=}SSZ",),
     "AXUIElementIsAttributeSettable": (
         b"i^{__AXUIElement=}^{__CFString=}^Z",
         "",
         {"arguments": {2: {"type_modifier": "o"}}},
     ),
     "AXTextMarkerRangeCreate": (
         b"^{__AXTextMarkerRange=}^{__CFAllocator=}^{__AXTextMarker=}^{__AXTextMarker=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
-    "GetCurrentProcess": (b"s^{ProcessSerialNumber=II}",),
+    "GetCurrentProcess": (
+        b"s^{ProcessSerialNumber=II}",
+        "",
+        {"arguments": {0: {"type_modifier": "o"}}},
+    ),
     "HIShapeCreateCopy": (
         b"^{__HIShape=}^{__HIShape=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "AXTextMarkerRangeCopyEndMarker": (
         b"^{__AXTextMarker=}^{__AXTextMarkerRange=}",
@@ -510,18 +515,21 @@
         },
     ),
     "AXUIElementCreateSystemWide": (
         b"^{__AXUIElement=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
-    "PasteboardCopyItemFlavors": (
-        b"i^{OpaquePasteboardRef=}^v^^{__CFArray=}",
+    "HIShapeIntersectsRect": (
+        b"Z^{__HIShape=}^{CGRect={CGPoint=dd}{CGSize=dd}}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"c_array_of_fixed_length": 1},
+            "arguments": {1: {"type_modifier": "n"}},
+        },
     ),
     "AXUIElementSetAttributeValue": (b"i^{__AXUIElement=}^{__CFString=}@",),
     "NewIconGetterUPP": (
         b"^?^?",
         "",
         {
             "arguments": {
@@ -532,20 +540,25 @@
                     }
                 }
             }
         },
     ),
     "GetProcessInformation": (
         b"s^{ProcessSerialNumber=II}^{ProcessInfoRec=I^C{ProcessSerialNumber=II}III^cII{ProcessSerialNumber=II}II^{FSRef=[80C]}}",
+        "",
+        {"arguments": {0: {"type_modifier": "n"}, 1: {"type_modifier": "o"}}},
     ),
     "AXMakeProcessTrusted": (b"i^{__CFString=}",),
     "ProcessInformationCopyDictionary": (
         b"^{__CFDictionary=}^{ProcessSerialNumber=II}I",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {0: {"type_modifier": "n"}},
+        },
     ),
     "AXTextMarkerCreate": (
         b"^{__AXTextMarker=}^{__CFAllocator=}^Cq",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {1: {"c_array_length_in_arg": 2, "type_modifier": "n"}},
@@ -556,20 +569,20 @@
         b"i^{__AXUIElement=}^^{__CFArray=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {1: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
-    "HIShapeIntersectsRect": (
-        b"Z^{__HIShape=}^{CGRect={CGPoint=dd}{CGSize=dd}}",
+    "PasteboardCopyItemFlavors": (
+        b"i^{OpaquePasteboardRef=}^v^^{__CFArray=}",
         "",
         {
-            "retval": {"c_array_of_fixed_length": 1},
-            "arguments": {1: {"type_modifier": "n"}},
+            "retval": {"already_cfretained": True},
+            "arguments": {2: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
     "HIShapeEnumerate": (
         b"i^{__HIShape=}I^?^v",
         "",
         {
             "arguments": {
@@ -590,55 +603,87 @@
                         },
                     },
                     "callable_retained": False,
                 }
             }
         },
     ),
-    "SameProcess": (b"s^{ProcessSerialNumber=II}^{ProcessSerialNumber=II}^Z",),
-    "WakeUpProcess": (b"s^{ProcessSerialNumber=II}",),
+    "SameProcess": (
+        b"s^{ProcessSerialNumber=II}^{ProcessSerialNumber=II}^Z",
+        "",
+        {
+            "arguments": {
+                0: {"type_modifier": "n"},
+                1: {"type_modifier": "n"},
+                2: {"type_modifier": "o"},
+            }
+        },
+    ),
+    "WakeUpProcess": (
+        b"s^{ProcessSerialNumber=II}",
+        "",
+        {"arguments": {0: {"type_modifier": "n"}}},
+    ),
     "PasteboardSynchronize": (b"I^{OpaquePasteboardRef=}",),
     "TranslationCopyDestinationType": (
         b"i^{OpaqueTranslationRef=}^^{__CFString=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {1: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
-    "IconRefContainsCGPoint": (
-        b"Z^{CGPoint=dd}^{CGRect={CGPoint=dd}{CGSize=dd}}sI^{OpaqueIconRef=}",
-    ),
     "AXUIElementCopyParameterizedAttributeNames": (
         b"i^{__AXUIElement=}^^{__CFArray=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {1: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
     "PasteboardCreate": (
         b"i^{__CFString=}^^{OpaquePasteboardRef=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {1: {"already_cfretained": True, "type_modifier": "o"}},
+        },
+    ),
+    "SetFrontProcessWithOptions": (
+        b"i^{ProcessSerialNumber=II}I",
+        "",
+        {"arguments": {0: {"type_modifier": "n"}}},
     ),
-    "SetFrontProcessWithOptions": (b"i^{ProcessSerialNumber=II}I",),
     "InvokeIconActionUPP": (b"sI^^^c^v^?",),
     "CopyProcessName": (
         b"i^{ProcessSerialNumber=II}^^{__CFString=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {
+                0: {"type_modifier": "n"},
+                1: {"already_cfretained": True, "type_modifier": "o"},
+            },
+        },
     ),
-    "PasteboardGetItemCount": (b"i^{OpaquePasteboardRef=}^Q",),
-    "PasteboardGetItemIdentifier": (b"i^{OpaquePasteboardRef=}q^^v",),
-    "IconRefToHIShape": (
-        b"^{__HIShape=}^{CGRect={CGPoint=dd}{CGSize=dd}}sI^{OpaqueIconRef=}",
+    "PasteboardGetItemCount": (
+        b"i^{OpaquePasteboardRef=}^Q",
+        "",
+        {"arguments": {1: {"type_modifier": "o"}}},
+    ),
+    "PasteboardGetItemIdentifier": (
+        b"i^{OpaquePasteboardRef=}q^^v",
+        "",
+        {"arguments": {2: {"type_modifier": "o"}}},
+    ),
+    "IsProcessVisible": (
+        b"Z^{ProcessSerialNumber=II}",
+        "",
+        {"arguments": {0: {"type_modifier": "n"}}},
     ),
-    "GetIconRefVariant": (b"^{OpaqueIconRef=}^{OpaqueIconRef=}I^s",),
-    "IsProcessVisible": (b"Z^{ProcessSerialNumber=II}",),
     "HIShapeIsRectangular": (b"Z^{__HIShape=}",),
     "AXTextMarkerGetBytePtr": (
         b"^C^{__AXTextMarker=}",
         "",
         {"retval": {"c_array_of_variable_length": True}},
     ),
     "HIShapeCreateWithRect": (
@@ -654,52 +699,71 @@
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {2: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
     "AXObserverGetRunLoopSource": (b"^{__CFRunLoopSource=}^{__AXObserver=}",),
-    "GetNextProcess": (b"s^{ProcessSerialNumber=II}",),
+    "GetNextProcess": (
+        b"s^{ProcessSerialNumber=II}",
+        "",
+        {"arguments": {0: {"type_modifier": "o"}}},
+    ),
     "AXUIElementGetAttributeValueCount": (
         b"i^{__AXUIElement=}^{__CFString=}^q",
         "",
         {"arguments": {2: {"type_modifier": "o"}}},
     ),
     "TranslationPerformForURL": (
         b"i^{OpaqueTranslationRef=}^{__CFURL=}^{__CFURL=}^^{__CFURL=}",
         "",
         {"arguments": {3: {"already_cfretained": True, "type_modifier": "o"}}},
     ),
     "AXValueGetType": (b"I^{__AXValue=}",),
     "UAZoomEnabled": (b"Z",),
-    "GetProcessPID": (b"i^{ProcessSerialNumber=II}^i",),
+    "GetProcessPID": (
+        b"i^{ProcessSerialNumber=II}^i",
+        "",
+        {"arguments": {0: {"type_modifier": "n"}, 1: {"type_modifier": "o"}}},
+    ),
     "AXUIElementGetPid": (
         b"i^{__AXUIElement=}^i",
         "",
         {"arguments": {1: {"type_modifier": "o"}}},
     ),
-    "GetProcessForPID": (b"ii^{ProcessSerialNumber=II}",),
+    "GetProcessForPID": (
+        b"ii^{ProcessSerialNumber=II}",
+        "",
+        {"arguments": {1: {"type_modifier": "o"}}},
+    ),
     "TranslationCreate": (
         b"i^{__CFString=}^{__CFString=}I^^{OpaqueTranslationRef=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {3: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
     "HIShapeUnionWithRect": (
         b"i^{__HIShape=}^{CGRect={CGPoint=dd}{CGSize=dd}}",
         "",
         {"arguments": {1: {"type_modifier": "n"}}},
     ),
-    "PasteboardGetItemFlavorFlags": (b"i^{OpaquePasteboardRef=}^v^{__CFString=}^I",),
+    "PasteboardGetItemFlavorFlags": (
+        b"i^{OpaquePasteboardRef=}^v^{__CFString=}^I",
+        "",
+        {"arguments": {3: {"type_modifier": "o"}}},
+    ),
     "PasteboardCopyPasteLocation": (
         b"i^{OpaquePasteboardRef=}^^{__CFURL=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {1: {"already_cfretained": True, "type_modifier": "o"}},
+        },
     ),
     "PasteboardSetPromiseKeeper": (
         b"i^{OpaquePasteboardRef=}^?^v",
         "",
         {
             "arguments": {
                 1: {
@@ -747,36 +811,43 @@
             "arguments": {4: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
     "SetIconFamilyData": (
         b"s^^{IconFamilyResource=Ii[1{IconFamilyElement=Ii[1C]}]}I^^c",
     ),
     "HIShapeIntersect": (b"i^{__HIShape=}^{__HIShape=}^{__HIShape=}",),
-    "IconRefToIconFamily": (
-        b"s^{OpaqueIconRef=}I^^^{IconFamilyResource=Ii[1{IconFamilyElement=Ii[1C]}]}",
-    ),
     "TranslationCreateWithSourceArray": (
         b"i^{__CFArray=}I^^{__CFArray=}^^{__CFDictionary=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {
                 2: {"already_cfretained": True, "type_modifier": "o"},
                 3: {"already_cfretained": True, "type_modifier": "o"},
             },
         },
     ),
-    "KillProcess": (b"s^{ProcessSerialNumber=II}",),
-    "SetFrontProcess": (b"s^{ProcessSerialNumber=II}",),
-    "DisposeIconActionUPP": (b"v^?",),
+    "KillProcess": (
+        b"s^{ProcessSerialNumber=II}",
+        "",
+        {"arguments": {0: {"type_modifier": "n"}}},
+    ),
+    "SetFrontProcess": (
+        b"s^{ProcessSerialNumber=II}",
+        "",
+        {"arguments": {0: {"type_modifier": "n"}}},
+    ),
     "InvokeIconGetterUPP": (b"^^cI^v^?",),
     "PasteboardCopyItemFlavorData": (
         b"i^{OpaquePasteboardRef=}^v^{__CFString=}^^{__CFData=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {3: {"already_cfretained": True, "type_modifier": "o"}},
+        },
     ),
     "AXUIElementCreateApplication": (
         b"^{__AXUIElement=}i",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "PasteboardGetTypeID": (b"Q",),
@@ -789,25 +860,35 @@
         },
     ),
     "HIShapeContainsPoint": (
         b"Z^{__HIShape=}^{CGPoint=dd}",
         "",
         {"arguments": {1: {"type_modifier": "n"}}},
     ),
-    "DisposeIconGetterUPP": (b"v^?",),
     "HIShapeGetBounds": (
         b"^{CGRect={CGPoint=dd}{CGSize=dd}}^{__HIShape=}^{CGRect={CGPoint=dd}{CGSize=dd}}",
         "",
-        {"arguments": {1: {"type_modifier": "o"}}},
+        {
+            "retval": {"deref_result_pointer": True},
+            "arguments": {1: {"type_modifier": "o"}},
+        },
     ),
     "AXObserverAddNotification": (
         b"i^{__AXObserver=}^{__AXUIElement=}^{__CFString=}^v",
     ),
-    "TransformProcessType": (b"i^{ProcessSerialNumber=II}I",),
-    "GetProcessBundleLocation": (b"i^{ProcessSerialNumber=II}^{FSRef=[80C]}",),
+    "TransformProcessType": (
+        b"i^{ProcessSerialNumber=II}I",
+        "",
+        {"arguments": {0: {"type_modifier": "n"}}},
+    ),
+    "GetProcessBundleLocation": (
+        b"i^{ProcessSerialNumber=II}^{FSRef=[80C]}",
+        "",
+        {"arguments": {0: {"type_modifier": "n"}, 1: {"type_modifier": "o"}}},
+    ),
     "HIShapeCreateIntersection": (
         b"^{__HIShape=}^{__HIShape=}^{__HIShape=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "HIShapeCreateMutableCopy": (
         b"^{__HIShape=}^{__HIShape=}",
@@ -818,15 +899,19 @@
         b"i^{__AXUIElement=}^{__CFString=}^@",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {2: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
-    "GetFrontProcess": (b"s^{ProcessSerialNumber=II}",),
+    "GetFrontProcess": (
+        b"s^{ProcessSerialNumber=II}",
+        "",
+        {"arguments": {0: {"type_modifier": "o"}}},
+    ),
     "HIShapeCreateEmpty": (
         b"^{__HIShape=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "AXObserverGetTypeID": (b"Q",),
     "AXTextMarkerRangeCopyStartMarker": (
@@ -894,24 +979,31 @@
     ),
     "HIShapeXor": (b"i^{__HIShape=}^{__HIShape=}^{__HIShape=}",),
     "HIShapeCreateMutable": (
         b"^{__HIShape=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
-    "ShowHideProcess": (b"s^{ProcessSerialNumber=II}Z",),
+    "ShowHideProcess": (
+        b"s^{ProcessSerialNumber=II}Z",
+        "",
+        {"arguments": {0: {"type_modifier": "n"}}},
+    ),
     "HIShapeIsEmpty": (b"Z^{__HIShape=}",),
     "AXUIElementSetMessagingTimeout": (b"i^{__AXUIElement=}f",),
     "ExitToShell": (b"v",),
     "AXIsProcessTrusted": (b"Z",),
     "AXUIElementGetTypeID": (b"Q",),
     "PasteboardCopyName": (
         b"i^{OpaquePasteboardRef=}^^{__CFString=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {1: {"already_cfretained": True, "type_modifier": "o"}},
+        },
     ),
     "HIShapeDifference": (b"i^{__HIShape=}^{__HIShape=}^{__HIShape=}",),
     "AXValueGetTypeID": (b"Q", "", {"variadic": False}),
     "AXUIElementCopyElementAtPosition": (
         b"i^{__AXUIElement=}ff^^{__AXUIElement=}",
         "",
         {
```

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/Lib/PrintCore/__init__.py` & `pyobjc-framework-ApplicationServices-9.2/Lib/PrintCore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/Lib/PrintCore/_metadata.py` & `pyobjc-framework-ApplicationServices-9.2/Lib/PrintCore/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Mar 11 13:04:50 2022
+# Last update: Sat May 20 09:54:44 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -537,14 +537,16 @@
         {
             "retval": {"already_cfretained": True},
             "arguments": {0: {"type_modifier": "o"}},
         },
     ),
     "PMSessionBeginPageNoDialog": (
         b"i^{OpaquePMPrintSession=}^{OpaquePMPageFormat=}^{PMRect=dddd}",
+        "",
+        {"arguments": {2: {"type_modifier": "n"}}},
     ),
     "PMPrinterGetLanguageInfo": (
         b"i^{OpaquePMPrinter=}^{PMLanguageInfo=[33C][33C][33C]}",
         "",
         {"arguments": {1: {"type_modifier": "o"}}},
     ),
     "PMSetLastPage": (b"i^{OpaquePMPrintSettings=}IZ",),
@@ -768,15 +770,15 @@
         "PMPrinter": objc.createOpaquePointerType("PMPrinter", b"^{OpaquePMPrinter}"),
         "PMServer": objc.createOpaquePointerType("PMServer", b"^{OpaquePMServer}"),
     }
 )
 r = objc.registerMetaDataForSelector
 objc._updatingMetadata(True)
 try:
-    r(b"NSObject", b"initWithBundle:", {"retval": {"type": "Z"}})
+    r(b"NSObject", b"initWithBundle:", {"retval": {"type": "@"}})
     r(b"NSObject", b"printWindowWillClose:", {"arguments": {2: {"type": "Z"}}})
     r(
         b"NSObject",
         b"restoreValuesAndReturnError:",
         {
             "retval": {"type": "Z"},
             "arguments": {2: {"type": "^@", "type_modifier": b"o"}},
```

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/Lib/pyobjc_framework_ApplicationServices.egg-info/PKG-INFO` & `pyobjc-framework-ApplicationServices-9.2/Lib/pyobjc_framework_ApplicationServices.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ApplicationServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ApplicationServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ApplicationServices,HIServices,PrintCore
 Platform: MacOS X
```

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/Lib/pyobjc_framework_ApplicationServices.egg-info/SOURCES.txt` & `pyobjc-framework-ApplicationServices-9.2/Lib/pyobjc_framework_ApplicationServices.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/ApplicationServices/__init__.py
 Lib/HIServices/__init__.py
 Lib/HIServices/_metadata.py
 Lib/PrintCore/__init__.py
 Lib/PrintCore/_metadata.py
 Lib/pyobjc_framework_ApplicationServices.egg-info/PKG-INFO
```

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/License.txt` & `pyobjc-framework-ApplicationServices-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/Modules/_HIServices.m` & `pyobjc-framework-ApplicationServices-9.2/Modules/_HIServices.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/Modules/_PrintCore.m` & `pyobjc-framework-ApplicationServices-9.2/Modules/_PrintCore.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-ApplicationServices-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-ApplicationServices-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PKG-INFO` & `pyobjc-framework-ApplicationServices-9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-ApplicationServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework ApplicationServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,ApplicationServices,HIServices,PrintCore
 Platform: MacOS X
```

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_applicationservices.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_applicationservices.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axactionconstants.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axactionconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axattributeconstants.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axattributeconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axerror.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axnotificationconstants.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axnotificationconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axroleconstants.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axroleconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axtextattributedstring.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axtextattributedstring.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axuielement.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axuielement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axvalue.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axvalue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_axvalueconstants.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_axvalueconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_hishape.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_hishape.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pdeplugininterface.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pdeplugininterface.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     @min_sdk_level("13.0")
     def test_protocols(self):
         self.assertProtocolExists("PDEPlugIn")
         self.assertProtocolExists("PDEPanel")
         self.assertProtocolExists("PDEPlugInCallbackProtocol")
 
     def testMethods(self):
-        self.assertResultIsBOOL(TestPDEPluginInterfaceHelper.initWithBundle_)
         self.assertResultIsBOOL(TestPDEPluginInterfaceHelper.shouldHide)
         self.assertResultIsBOOL(TestPDEPluginInterfaceHelper.saveValuesAndReturnError_)
         self.assertArgIsOut(TestPDEPluginInterfaceHelper.saveValuesAndReturnError_, 0)
         self.assertResultIsBOOL(
             TestPDEPluginInterfaceHelper.restoreValuesAndReturnError_
         )
         self.assertArgIsOut(
```

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pmcore.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pmcore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pmdefinitions.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pmdefinitions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pmerrors.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pmerrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pmprintaetypes.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pmprintaetypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pmprintingdialogextensions.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pmprintingdialogextensions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_pmprintsettingskeys.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_pmprintsettingskeys.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/PyObjCTest/test_translationservicse.py` & `pyobjc-framework-ApplicationServices-9.2/PyObjCTest/test_translationservicse.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/HIServices.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/HIServices.fwinfo`

 * *Files 2% similar despite different names*

```diff
@@ -1,1477 +1,1560 @@
-00000000: 2f2f 206f 626a 6563 7469 7665 2e6d 6574  // objective.met
-00000010: 6164 6174 6120 6578 6365 7074 696f 6e73  adata exceptions
-00000020: 2066 696c 652c 2073 6565 2069 7473 2064   file, see its d
-00000030: 6f63 756d 656e 740a 2f2f 2066 6f72 2069  ocument.// for i
-00000040: 6e66 6f72 6d61 7469 6f6e 206f 6e20 686f  nformation on ho
-00000050: 7720 746f 2075 7064 6174 6520 7468 6973  w to update this
-00000060: 2066 696c 652e 0a7b 0a20 2264 6566 696e   file..{. "defin
-00000070: 6974 696f 6e73 223a 207b 0a20 2022 636c  itions": {.  "cl
-00000080: 6173 7365 7322 3a20 7b7d 2c0a 2020 2266  asses": {},.  "f
-00000090: 6f72 6d61 6c5f 7072 6f74 6f63 6f6c 7322  ormal_protocols"
-000000a0: 3a20 7b7d 2c0a 2020 2266 756e 6374 696f  : {},.  "functio
-000000b0: 6e73 223a 207b 0a20 2020 2241 5854 6578  ns": {.   "AXTex
-000000c0: 744d 6172 6b65 7252 616e 6765 4372 6561  tMarkerRangeCrea
-000000d0: 7465 5769 7468 4279 7465 7322 3a20 7b0a  teWithBytes": {.
-000000e0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-000000f0: 2020 2022 3122 3a20 7b20 2274 7970 655f     "1": { "type_
-00000100: 6d6f 6469 6669 6572 223a 2022 6e22 2c20  modifier": "n", 
-00000110: 2263 5f61 7272 6179 5f6c 656e 6774 685f  "c_array_length_
-00000120: 696e 5f61 7267 223a 2032 207d 2c0a 2020  in_arg": 2 },.  
-00000130: 2020 2022 3322 3a20 7b20 2274 7970 655f     "3": { "type_
-00000140: 6d6f 6469 6669 6572 223a 2022 6e22 2c20  modifier": "n", 
-00000150: 2263 5f61 7272 6179 5f6c 656e 6774 685f  "c_array_length_
-00000160: 696e 5f61 7267 223a 2034 207d 0a20 2020  in_arg": 4 }.   
-00000170: 207d 2c0a 2020 2020 2272 6574 7661 6c22   },.    "retval"
-00000180: 3a20 7b20 2261 6c72 6561 6479 5f63 6672  : { "already_cfr
-00000190: 6574 6169 6e65 6422 3a20 7472 7565 207d  etained": true }
-000001a0: 0a20 2020 7d2c 0a20 2020 2241 5854 6578  .   },.   "AXTex
-000001b0: 744d 6172 6b65 7243 7265 6174 6522 3a20  tMarkerCreate": 
-000001c0: 7b0a 2020 2020 2261 7267 7322 3a7b 0a20  {.    "args":{. 
-000001d0: 2020 2020 2231 223a 207b 2022 7479 7065      "1": { "type
-000001e0: 5f6d 6f64 6966 6965 7222 3a20 226e 222c  _modifier": "n",
-000001f0: 2022 635f 6172 7261 795f 6c65 6e67 7468   "c_array_length
-00000200: 5f69 6e5f 6172 6722 3a20 3220 7d0a 2020  _in_arg": 2 }.  
-00000210: 2020 7d2c 0a20 2020 2022 7265 7476 616c    },.    "retval
-00000220: 223a 207b 2022 616c 7265 6164 795f 6366  ": { "already_cf
-00000230: 7265 7461 696e 6564 223a 2074 7275 6520  retained": true 
-00000240: 7d0a 2020 207d 2c0a 2020 2022 4158 5465  }.   },.   "AXTe
-00000250: 7874 4d61 726b 6572 4765 7442 7974 6550  xtMarkerGetByteP
-00000260: 7472 223a 207b 0a20 2020 2022 7265 7476  tr": {.    "retv
-00000270: 616c 223a 207b 2022 635f 6172 7261 795f  al": { "c_array_
-00000280: 6f66 5f76 6172 6961 626c 655f 6c65 6e67  of_variable_leng
-00000290: 7468 223a 2074 7275 6520 7d0a 2020 207d  th": true }.   }
-000002a0: 2c0a 2020 2022 4158 4973 5072 6f63 6573  ,.   "AXIsProces
-000002b0: 7354 7275 7374 6564 5769 7468 4f70 7469  sTrustedWithOpti
-000002c0: 6f6e 7322 3a20 7b0a 2020 2020 2261 7267  ons": {.    "arg
-000002d0: 7322 3a20 7b0a 2020 2020 2022 3022 3a20  s": {.     "0": 
-000002e0: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
-000002f0: 2020 2241 584d 616b 6550 726f 6365 7373    "AXMakeProcess
-00000300: 5472 7573 7465 6422 3a20 7b0a 2020 2020  Trusted": {.    
-00000310: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
-00000320: 3022 3a20 7b7d 0a20 2020 207d 0a20 2020  0": {}.    }.   
-00000330: 7d2c 0a20 2020 2241 584f 6273 6572 7665  },.   "AXObserve
-00000340: 7241 6464 4e6f 7469 6669 6361 7469 6f6e  rAddNotification
-00000350: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-00000360: 207b 0a20 2020 2020 2230 223a 207b 7d2c   {.     "0": {},
-00000370: 0a20 2020 2020 2231 223a 207b 7d2c 0a20  .     "1": {},. 
-00000380: 2020 2020 2232 223a 207b 7d2c 0a20 2020      "2": {},.   
-00000390: 2020 2233 223a 207b 7d0a 2020 2020 7d0a    "3": {}.    }.
-000003a0: 2020 207d 2c0a 2020 2022 4158 4f62 7365     },.   "AXObse
-000003b0: 7276 6572 4372 6561 7465 223a 207b 0a20  rverCreate": {. 
-000003c0: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
-000003d0: 2020 2231 223a 207b 0a20 2020 2020 2022    "1": {.      "
-000003e0: 6675 6e63 7469 6f6e 223a 207b 0a20 2020  function": {.   
-000003f0: 2020 2020 2261 7267 7322 3a20 5b0a 2020      "args": [.  
-00000400: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00000410: 2022 7479 7065 7374 7222 3a20 225e 7b5f   "typestr": "^{_
-00000420: 5f41 584f 6273 6572 7665 723d 7d22 0a20  _AXObserver=}". 
-00000430: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00000440: 2020 7b0a 2020 2020 2020 2020 2022 7479    {.         "ty
-00000450: 7065 7374 7222 3a20 225e 7b5f 5f41 5855  pestr": "^{__AXU
-00000460: 4945 6c65 6d65 6e74 3d7d 220a 2020 2020  IElement=}".    
-00000470: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
-00000480: 0a20 2020 2020 2020 2020 2274 7970 6573  .         "types
-00000490: 7472 223a 2022 5e7b 5f5f 4346 5374 7269  tr": "^{__CFStri
-000004a0: 6e67 3d7d 220a 2020 2020 2020 2020 7d2c  ng=}".        },
-000004b0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-000004c0: 2020 2020 2274 7970 6573 7472 223a 2022      "typestr": "
-000004d0: 5e76 220a 2020 2020 2020 2020 7d0a 2020  ^v".        }.  
-000004e0: 2020 2020 205d 2c0a 2020 2020 2020 2022       ],.       "
-000004f0: 7265 7476 616c 223a 207b 0a20 2020 2020  retval": {.     
-00000500: 2020 2022 7479 7065 7374 7222 3a20 2276     "typestr": "v
-00000510: 220a 2020 2020 2020 207d 0a20 2020 2020  ".       }.     
-00000520: 207d 0a20 2020 2020 7d2c 0a20 2020 2020   }.     },.     
-00000530: 2232 223a 207b 2022 7479 7065 5f6d 6f64  "2": { "type_mod
-00000540: 6966 6965 7222 3a20 226f 222c 2022 616c  ifier": "o", "al
-00000550: 7265 6164 795f 6366 7265 7461 696e 6564  ready_cfretained
-00000560: 223a 2074 7275 6520 7d0a 2020 2020 7d0a  ": true }.    }.
-00000570: 2020 207d 2c0a 2020 2022 4158 4f62 7365     },.   "AXObse
-00000580: 7276 6572 4372 6561 7465 5769 7468 496e  rverCreateWithIn
-00000590: 666f 4361 6c6c 6261 636b 223a 207b 0a20  foCallback": {. 
-000005a0: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
-000005b0: 2020 2231 223a 207b 0a20 2020 2020 2022    "1": {.      "
-000005c0: 6675 6e63 7469 6f6e 223a 207b 0a20 2020  function": {.   
-000005d0: 2020 2020 2261 7267 7322 3a20 5b0a 2020      "args": [.  
-000005e0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-000005f0: 2022 7479 7065 7374 7222 3a20 225e 7b5f   "typestr": "^{_
-00000600: 5f41 584f 6273 6572 7665 723d 7d22 0a20  _AXObserver=}". 
-00000610: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00000620: 2020 7b0a 2020 2020 2020 2020 2022 7479    {.         "ty
-00000630: 7065 7374 7222 3a20 225e 7b5f 5f41 5855  pestr": "^{__AXU
-00000640: 4945 6c65 6d65 6e74 3d7d 220a 2020 2020  IElement=}".    
-00000650: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
-00000660: 0a20 2020 2020 2020 2020 2274 7970 6573  .         "types
-00000670: 7472 223a 2022 5e7b 5f5f 4346 5374 7269  tr": "^{__CFStri
-00000680: 6e67 3d7d 220a 2020 2020 2020 2020 7d2c  ng=}".        },
-00000690: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-000006a0: 2020 2020 2274 7970 6573 7472 223a 2022      "typestr": "
-000006b0: 5e7b 5f5f 4346 4469 6374 696f 6e61 7279  ^{__CFDictionary
-000006c0: 3d7d 220a 2020 2020 2020 2020 7d2c 0a20  =}".        },. 
-000006d0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-000006e0: 2020 2274 7970 6573 7472 223a 2022 5e76    "typestr": "^v
-000006f0: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
-00000700: 2020 205d 2c0a 2020 2020 2020 2022 7265     ],.       "re
-00000710: 7476 616c 223a 207b 0a20 2020 2020 2020  tval": {.       
-00000720: 2022 7479 7065 7374 7222 3a20 2276 220a   "typestr": "v".
-00000730: 2020 2020 2020 207d 0a20 2020 2020 207d         }.      }
-00000740: 0a20 2020 2020 7d2c 0a20 2020 2020 2232  .     },.     "2
-00000750: 223a 207b 2022 7479 7065 5f6d 6f64 6966  ": { "type_modif
-00000760: 6965 7222 3a20 226f 222c 2022 616c 7265  ier": "o", "alre
-00000770: 6164 795f 6366 7265 7461 696e 6564 223a  ady_cfretained":
-00000780: 2074 7275 6520 7d0a 2020 2020 7d0a 2020   true }.    }.  
-00000790: 207d 2c0a 2020 2022 4158 4f62 7365 7276   },.   "AXObserv
-000007a0: 6572 4765 7452 756e 4c6f 6f70 536f 7572  erGetRunLoopSour
-000007b0: 6365 223a 207b 0a20 2020 2022 6172 6773  ce": {.    "args
-000007c0: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
-000007d0: 7d0a 2020 2020 7d2c 0a20 2020 2022 7265  }.    },.    "re
-000007e0: 7476 616c 223a 207b 7d0a 2020 207d 2c0a  tval": {}.   },.
-000007f0: 2020 2022 4158 4f62 7365 7276 6572 5265     "AXObserverRe
-00000800: 6d6f 7665 4e6f 7469 6669 6361 7469 6f6e  moveNotification
-00000810: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-00000820: 207b 0a20 2020 2020 2230 223a 207b 7d2c   {.     "0": {},
-00000830: 0a20 2020 2020 2231 223a 207b 7d2c 0a20  .     "1": {},. 
-00000840: 2020 2020 2232 223a 207b 7d0a 2020 2020      "2": {}.    
-00000850: 7d0a 2020 207d 2c0a 2020 2022 4158 5549  }.   },.   "AXUI
-00000860: 456c 656d 656e 7443 6f70 7941 6374 696f  ElementCopyActio
-00000870: 6e44 6573 6372 6970 7469 6f6e 223a 207b  nDescription": {
-00000880: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
-00000890: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
-000008a0: 2020 2231 223a 207b 7d2c 0a20 2020 2020    "1": {},.     
-000008b0: 2232 223a 207b 2022 7479 7065 5f6d 6f64  "2": { "type_mod
-000008c0: 6966 6965 7222 3a20 226f 222c 2022 616c  ifier": "o", "al
-000008d0: 7265 6164 795f 6366 7265 7461 696e 6564  ready_cfretained
-000008e0: 223a 2074 7275 6520 7d0a 2020 2020 7d0a  ": true }.    }.
-000008f0: 2020 207d 2c0a 2020 2022 4158 5549 456c     },.   "AXUIEl
-00000900: 656d 656e 7443 6f70 7941 6374 696f 6e4e  ementCopyActionN
-00000910: 616d 6573 223a 207b 0a20 2020 2022 6172  ames": {.    "ar
-00000920: 6773 223a 207b 0a20 2020 2020 2230 223a  gs": {.     "0":
-00000930: 207b 7d2c 0a20 2020 2020 2231 223a 207b   {},.     "1": {
-00000940: 2022 7479 7065 5f6d 6f64 6966 6965 7222   "type_modifier"
-00000950: 3a20 226f 222c 2022 616c 7265 6164 795f  : "o", "already_
-00000960: 6366 7265 7461 696e 6564 223a 2074 7275  cfretained": tru
-00000970: 6520 7d0a 2020 2020 7d0a 2020 207d 2c0a  e }.    }.   },.
-00000980: 2020 2022 4158 5549 456c 656d 656e 7443     "AXUIElementC
-00000990: 6f70 7941 7474 7269 6275 7465 4e61 6d65  opyAttributeName
-000009a0: 7322 3a20 7b0a 2020 2020 2261 7267 7322  s": {.    "args"
-000009b0: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
-000009c0: 2c0a 2020 2020 2022 3122 3a20 7b20 2274  ,.     "1": { "t
-000009d0: 7970 655f 6d6f 6469 6669 6572 223a 2022  ype_modifier": "
-000009e0: 6f22 2c20 2261 6c72 6561 6479 5f63 6672  o", "already_cfr
-000009f0: 6574 6169 6e65 6422 3a20 7472 7565 207d  etained": true }
-00000a00: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
-00000a10: 2241 5855 4945 6c65 6d65 6e74 436f 7079  "AXUIElementCopy
-00000a20: 4174 7472 6962 7574 6556 616c 7565 223a  AttributeValue":
-00000a30: 207b 0a20 2020 2022 6172 6773 223a 207b   {.    "args": {
-00000a40: 0a20 2020 2020 2230 223a 207b 7d2c 0a20  .     "0": {},. 
-00000a50: 2020 2020 2231 223a 207b 7d2c 0a20 2020      "1": {},.   
-00000a60: 2020 2232 223a 207b 2022 7479 7065 5f6d    "2": { "type_m
-00000a70: 6f64 6966 6965 7222 3a20 226f 222c 2022  odifier": "o", "
-00000a80: 616c 7265 6164 795f 6366 7265 7461 696e  already_cfretain
-00000a90: 6564 223a 2074 7275 6520 7d0a 2020 2020  ed": true }.    
-00000aa0: 7d0a 2020 207d 2c0a 2020 2022 4158 5549  }.   },.   "AXUI
-00000ab0: 456c 656d 656e 7443 6f70 7941 7474 7269  ElementCopyAttri
-00000ac0: 6275 7465 5661 6c75 6573 223a 207b 0a20  buteValues": {. 
-00000ad0: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
-00000ae0: 2020 2230 223a 207b 7d2c 0a20 2020 2020    "0": {},.     
-00000af0: 2231 223a 207b 7d2c 0a20 2020 2020 2234  "1": {},.     "4
-00000b00: 223a 207b 2022 7479 7065 5f6d 6f64 6966  ": { "type_modif
-00000b10: 6965 7222 3a20 226f 222c 2022 616c 7265  ier": "o", "alre
-00000b20: 6164 795f 6366 7265 7461 696e 6564 223a  ady_cfretained":
-00000b30: 2074 7275 6520 7d0a 2020 2020 7d0a 2020   true }.    }.  
-00000b40: 207d 2c0a 2020 2022 4158 5549 456c 656d   },.   "AXUIElem
-00000b50: 656e 7443 6f70 7945 6c65 6d65 6e74 4174  entCopyElementAt
-00000b60: 506f 7369 7469 6f6e 223a 207b 0a20 2020  Position": {.   
-00000b70: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
-00000b80: 2230 223a 207b 7d2c 0a20 2020 2020 2233  "0": {},.     "3
-00000b90: 223a 207b 2022 7479 7065 5f6d 6f64 6966  ": { "type_modif
-00000ba0: 6965 7222 3a20 226f 222c 2022 616c 7265  ier": "o", "alre
-00000bb0: 6164 795f 6366 7265 7461 696e 6564 223a  ady_cfretained":
-00000bc0: 2074 7275 6520 7d0a 2020 2020 7d0a 2020   true }.    }.  
-00000bd0: 207d 2c0a 2020 2022 4158 5549 456c 656d   },.   "AXUIElem
-00000be0: 656e 7443 6f70 794d 756c 7469 706c 6541  entCopyMultipleA
-00000bf0: 7474 7269 6275 7465 5661 6c75 6573 223a  ttributeValues":
-00000c00: 207b 0a20 2020 2022 6172 6773 223a 207b   {.    "args": {
-00000c10: 0a20 2020 2020 2230 223a 207b 7d2c 0a20  .     "0": {},. 
-00000c20: 2020 2020 2231 223a 207b 7d2c 0a20 2020      "1": {},.   
-00000c30: 2020 2233 223a 207b 2022 7479 7065 5f6d    "3": { "type_m
-00000c40: 6f64 6966 6965 7222 3a20 226f 222c 2022  odifier": "o", "
-00000c50: 616c 7265 6164 795f 6366 7265 7461 696e  already_cfretain
-00000c60: 6564 223a 2074 7275 6520 7d0a 2020 2020  ed": true }.    
-00000c70: 7d0a 2020 207d 2c0a 2020 2022 4158 5549  }.   },.   "AXUI
-00000c80: 456c 656d 656e 7443 6f70 7950 6172 616d  ElementCopyParam
-00000c90: 6574 6572 697a 6564 4174 7472 6962 7574  eterizedAttribut
-00000ca0: 654e 616d 6573 223a 207b 0a20 2020 2022  eNames": {.    "
-00000cb0: 6172 6773 223a 207b 0a20 2020 2020 2230  args": {.     "0
-00000cc0: 223a 207b 7d2c 0a20 2020 2020 2231 223a  ": {},.     "1":
-00000cd0: 207b 2022 7479 7065 5f6d 6f64 6966 6965   { "type_modifie
-00000ce0: 7222 3a20 226f 222c 2022 616c 7265 6164  r": "o", "alread
-00000cf0: 795f 6366 7265 7461 696e 6564 223a 2074  y_cfretained": t
-00000d00: 7275 6520 7d0a 2020 2020 7d0a 2020 207d  rue }.    }.   }
-00000d10: 2c0a 2020 2022 4158 5549 456c 656d 656e  ,.   "AXUIElemen
-00000d20: 7443 6f70 7950 6172 616d 6574 6572 697a  tCopyParameteriz
-00000d30: 6564 4174 7472 6962 7574 6556 616c 7565  edAttributeValue
-00000d40: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-00000d50: 207b 0a20 2020 2020 2230 223a 207b 7d2c   {.     "0": {},
-00000d60: 0a20 2020 2020 2231 223a 207b 7d2c 0a20  .     "1": {},. 
-00000d70: 2020 2020 2233 223a 207b 2022 7479 7065      "3": { "type
-00000d80: 5f6d 6f64 6966 6965 7222 3a20 226f 222c  _modifier": "o",
-00000d90: 2022 616c 7265 6164 795f 6366 7265 7461   "already_cfreta
-00000da0: 696e 6564 223a 2074 7275 6520 7d0a 2020  ined": true }.  
-00000db0: 2020 7d0a 2020 207d 2c0a 2020 2022 4158    }.   },.   "AX
-00000dc0: 5549 456c 656d 656e 7443 7265 6174 6541  UIElementCreateA
-00000dd0: 7070 6c69 6361 7469 6f6e 223a 207b 0a20  pplication": {. 
-00000de0: 2020 2022 7265 7476 616c 223a 207b 0a20     "retval": {. 
-00000df0: 2020 2020 2261 6c72 6561 6479 5f63 6672      "already_cfr
-00000e00: 6574 6169 6e65 6422 3a20 7472 7565 0a20  etained": true. 
-00000e10: 2020 207d 0a20 2020 7d2c 0a20 2020 2241     }.   },.   "A
-00000e20: 5855 4945 6c65 6d65 6e74 4372 6561 7465  XUIElementCreate
-00000e30: 5379 7374 656d 5769 6465 223a 207b 0a20  SystemWide": {. 
-00000e40: 2020 2022 7265 7476 616c 223a 207b 0a20     "retval": {. 
-00000e50: 2020 2020 2261 6c72 6561 6479 5f63 6672      "already_cfr
-00000e60: 6574 6169 6e65 6422 3a20 7472 7565 0a20  etained": true. 
-00000e70: 2020 207d 0a20 2020 7d2c 0a20 2020 2241     }.   },.   "A
-00000e80: 5855 4945 6c65 6d65 6e74 4765 7441 7474  XUIElementGetAtt
-00000e90: 7269 6275 7465 5661 6c75 6543 6f75 6e74  ributeValueCount
-00000ea0: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-00000eb0: 207b 0a20 2020 2020 2230 223a 207b 7d2c   {.     "0": {},
-00000ec0: 0a20 2020 2020 2231 223a 207b 7d2c 0a20  .     "1": {},. 
-00000ed0: 2020 2020 2232 223a 207b 2022 7479 7065      "2": { "type
-00000ee0: 5f6d 6f64 6966 6965 7222 3a20 226f 2220  _modifier": "o" 
-00000ef0: 7d0a 2020 2020 7d0a 2020 207d 2c0a 2020  }.    }.   },.  
-00000f00: 2022 4158 5549 456c 656d 656e 7447 6574   "AXUIElementGet
-00000f10: 5069 6422 3a20 7b0a 2020 2020 2261 7267  Pid": {.    "arg
-00000f20: 7322 3a20 7b0a 2020 2020 2022 3022 3a20  s": {.     "0": 
-00000f30: 7b7d 2c0a 2020 2020 2022 3122 3a20 7b20  {},.     "1": { 
-00000f40: 2274 7970 655f 6d6f 6469 6669 6572 223a  "type_modifier":
-00000f50: 2022 6f22 207d 0a20 2020 207d 0a20 2020   "o" }.    }.   
-00000f60: 7d2c 0a20 2020 2241 5855 4945 6c65 6d65  },.   "AXUIEleme
-00000f70: 6e74 4973 4174 7472 6962 7574 6553 6574  ntIsAttributeSet
-00000f80: 7461 626c 6522 3a20 7b0a 2020 2020 2261  table": {.    "a
-00000f90: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
-00000fa0: 3a20 7b7d 2c0a 2020 2020 2022 3122 3a20  : {},.     "1": 
-00000fb0: 7b7d 2c0a 2020 2020 2022 3222 3a20 7b20  {},.     "2": { 
-00000fc0: 2274 7970 655f 6d6f 6469 6669 6572 223a  "type_modifier":
-00000fd0: 2022 6f22 207d 0a20 2020 207d 0a20 2020   "o" }.    }.   
-00000fe0: 7d2c 0a20 2020 2241 5855 4945 6c65 6d65  },.   "AXUIEleme
-00000ff0: 6e74 5065 7266 6f72 6d41 6374 696f 6e22  ntPerformAction"
-00001000: 3a20 7b0a 2020 2020 2261 7267 7322 3a20  : {.    "args": 
-00001010: 7b0a 2020 2020 2022 3022 3a20 7b7d 2c0a  {.     "0": {},.
-00001020: 2020 2020 2022 3122 3a20 7b7d 0a20 2020       "1": {}.   
-00001030: 207d 0a20 2020 7d2c 0a20 2020 2241 5855   }.   },.   "AXU
-00001040: 4945 6c65 6d65 6e74 506f 7374 4b65 7962  IElementPostKeyb
-00001050: 6f61 7264 4576 656e 7422 3a20 7b0a 2020  oardEvent": {.  
-00001060: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
-00001070: 2022 3022 3a20 7b7d 0a20 2020 207d 0a20   "0": {}.    }. 
-00001080: 2020 7d2c 0a20 2020 2241 5855 4945 6c65    },.   "AXUIEle
-00001090: 6d65 6e74 5365 7441 7474 7269 6275 7465  mentSetAttribute
-000010a0: 5661 6c75 6522 3a20 7b0a 2020 2020 2261  Value": {.    "a
-000010b0: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
-000010c0: 3a20 7b7d 2c0a 2020 2020 2022 3122 3a20  : {},.     "1": 
-000010d0: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
-000010e0: 2020 2241 5855 4945 6c65 6d65 6e74 5365    "AXUIElementSe
-000010f0: 744d 6573 7361 6769 6e67 5469 6d65 6f75  tMessagingTimeou
-00001100: 7422 3a20 7b0a 2020 2020 2261 7267 7322  t": {.    "args"
-00001110: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
-00001120: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
-00001130: 2241 5856 616c 7565 4372 6561 7465 223a  "AXValueCreate":
-00001140: 207b 0a20 2020 2022 6967 6e6f 7265 223a   {.    "ignore":
-00001150: 2074 7275 652c 0a20 2020 2022 6172 6773   true,.    "args
-00001160: 223a 207b 0a20 2020 2020 2231 223a 207b  ": {.     "1": {
-00001170: 7d0a 2020 2020 7d2c 0a20 2020 2022 7265  }.    },.    "re
-00001180: 7476 616c 223a 207b 0a20 2020 2020 2261  tval": {.     "a
-00001190: 6c72 6561 6479 5f63 6672 6574 6169 6e65  lready_cfretaine
-000011a0: 6422 3a20 7472 7565 0a20 2020 207d 0a20  d": true.    }. 
-000011b0: 2020 7d2c 0a20 2020 2241 5856 616c 7565    },.   "AXValue
-000011c0: 4765 7454 7970 6522 3a20 7b0a 2020 2020  GetType": {.    
-000011d0: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
-000011e0: 3022 3a20 7b7d 0a20 2020 207d 0a20 2020  0": {}.    }.   
-000011f0: 7d2c 0a20 2020 2241 5856 616c 7565 4765  },.   "AXValueGe
-00001200: 7454 7970 6549 4422 3a20 7b0a 2020 2020  tTypeID": {.    
-00001210: 2276 6172 6961 6469 6322 3a20 6661 6c73  "variadic": fals
-00001220: 650a 2020 207d 2c0a 2020 2022 4158 5661  e.   },.   "AXVa
-00001230: 6c75 6547 6574 5661 6c75 6522 3a20 7b0a  lueGetValue": {.
-00001240: 2020 2020 2269 676e 6f72 6522 3a20 7472      "ignore": tr
-00001250: 7565 2c0a 2020 2020 2261 7267 7322 3a20  ue,.    "args": 
-00001260: 7b0a 2020 2020 2022 3022 3a20 7b7d 2c0a  {.     "0": {},.
-00001270: 2020 2020 2022 3222 3a20 7b7d 0a20 2020       "2": {}.   
-00001280: 207d 0a20 2020 7d2c 0a20 2020 2241 6464   }.   },.   "Add
-00001290: 4963 6f6e 546f 5375 6974 6522 3a20 7b0a  IconToSuite": {.
-000012a0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-000012b0: 2020 2022 3022 3a20 7b7d 2c0a 2020 2020     "0": {},.    
-000012c0: 2022 3122 3a20 7b7d 0a20 2020 207d 0a20   "1": {}.    }. 
-000012d0: 2020 7d2c 0a20 2020 2243 6f70 7950 726f    },.   "CopyPro
-000012e0: 6365 7373 4e61 6d65 223a 207b 0a20 2020  cessName": {.   
-000012f0: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
-00001300: 2230 223a 207b 7d2c 0a20 2020 2020 2231  "0": {},.     "1
-00001310: 223a 207b 7d0a 2020 2020 7d0a 2020 207d  ": {}.    }.   }
-00001320: 2c0a 2020 2022 4469 7370 6f73 6543 4963  ,.   "DisposeCIc
-00001330: 6f6e 223a 207b 0a20 2020 2022 6172 6773  on": {.    "args
-00001340: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
-00001350: 7d0a 2020 2020 7d0a 2020 207d 2c0a 2020  }.    }.   },.  
-00001360: 2022 4469 7370 6f73 6549 636f 6e41 6374   "DisposeIconAct
-00001370: 696f 6e55 5050 223a 207b 0a20 2020 2022  ionUPP": {.    "
-00001380: 6172 6773 223a 207b 0a20 2020 2020 2230  args": {.     "0
-00001390: 223a 207b 7d0a 2020 2020 7d0a 2020 207d  ": {}.    }.   }
-000013a0: 2c0a 2020 2022 4469 7370 6f73 6549 636f  ,.   "DisposeIco
-000013b0: 6e47 6574 7465 7255 5050 223a 207b 0a20  nGetterUPP": {. 
-000013c0: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
-000013d0: 2020 2230 223a 207b 7d0a 2020 2020 7d0a    "0": {}.    }.
-000013e0: 2020 207d 2c0a 2020 2022 4469 7370 6f73     },.   "Dispos
-000013f0: 6549 636f 6e53 7569 7465 223a 207b 0a20  eIconSuite": {. 
-00001400: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
-00001410: 2020 2230 223a 207b 7d0a 2020 2020 7d0a    "0": {}.    }.
-00001420: 2020 207d 2c0a 2020 2022 466f 7245 6163     },.   "ForEac
-00001430: 6849 636f 6e44 6f22 3a20 7b0a 2020 2020  hIconDo": {.    
-00001440: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
-00001450: 3022 3a20 7b7d 2c0a 2020 2020 2022 3222  0": {},.     "2"
-00001460: 3a20 7b7d 2c0a 2020 2020 2022 3322 3a20  : {},.     "3": 
-00001470: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
-00001480: 2020 2247 6574 4349 636f 6e22 3a20 7b0a    "GetCIcon": {.
-00001490: 2020 2020 2272 6574 7661 6c22 3a20 7b7d      "retval": {}
-000014a0: 0a20 2020 7d2c 0a20 2020 2247 6574 4375  .   },.   "GetCu
-000014b0: 7272 656e 7450 726f 6365 7373 223a 207b  rrentProcess": {
-000014c0: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
-000014d0: 2020 2020 2230 223a 207b 7d0a 2020 2020      "0": {}.    
-000014e0: 7d0a 2020 207d 2c0a 2020 2022 4765 7446  }.   },.   "GetF
-000014f0: 726f 6e74 5072 6f63 6573 7322 3a20 7b0a  rontProcess": {.
-00001500: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-00001510: 2020 2022 3022 3a20 7b7d 0a20 2020 207d     "0": {}.    }
-00001520: 0a20 2020 7d2c 0a20 2020 2247 6574 4963  .   },.   "GetIc
-00001530: 6f6e 223a 207b 0a20 2020 2022 7265 7476  on": {.    "retv
-00001540: 616c 223a 207b 7d0a 2020 207d 2c0a 2020  al": {}.   },.  
-00001550: 2022 4765 7449 636f 6e43 6163 6865 4461   "GetIconCacheDa
-00001560: 7461 223a 207b 0a20 2020 2022 6172 6773  ta": {.    "args
-00001570: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
-00001580: 7d2c 0a20 2020 2020 2231 223a 207b 7d0a  },.     "1": {}.
-00001590: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
-000015a0: 4765 7449 636f 6e43 6163 6865 5072 6f63  GetIconCacheProc
-000015b0: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-000015c0: 207b 0a20 2020 2020 2230 223a 207b 7d2c   {.     "0": {},
-000015d0: 0a20 2020 2020 2231 223a 207b 7d0a 2020  .     "1": {}.  
-000015e0: 2020 7d0a 2020 207d 2c0a 2020 2022 4765    }.   },.   "Ge
-000015f0: 7449 636f 6e46 616d 696c 7944 6174 6122  tIconFamilyData"
-00001600: 3a20 7b0a 2020 2020 2261 7267 7322 3a20  : {.    "args": 
-00001610: 7b0a 2020 2020 2022 3022 3a20 7b7d 2c0a  {.     "0": {},.
-00001620: 2020 2020 2022 3222 3a20 7b7d 0a20 2020       "2": {}.   
-00001630: 207d 0a20 2020 7d2c 0a20 2020 2247 6574   }.   },.   "Get
-00001640: 4963 6f6e 4672 6f6d 5375 6974 6522 3a20  IconFromSuite": 
-00001650: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
-00001660: 2020 2020 2022 3022 3a20 7b7d 2c0a 2020       "0": {},.  
-00001670: 2020 2022 3122 3a20 7b7d 0a20 2020 207d     "1": {}.    }
-00001680: 0a20 2020 7d2c 0a20 2020 2247 6574 4963  .   },.   "GetIc
-00001690: 6f6e 5265 6656 6172 6961 6e74 223a 207b  onRefVariant": {
-000016a0: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
-000016b0: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
-000016c0: 2020 2232 223a 207b 7d0a 2020 2020 7d2c    "2": {}.    },
-000016d0: 0a20 2020 2022 7265 7476 616c 223a 207b  .    "retval": {
-000016e0: 7d0a 2020 207d 2c0a 2020 2022 4765 7449  }.   },.   "GetI
-000016f0: 636f 6e53 697a 6573 4672 6f6d 4963 6f6e  conSizesFromIcon
-00001700: 5265 6622 3a20 7b0a 2020 2020 2261 7267  Ref": {.    "arg
-00001710: 7322 3a20 7b0a 2020 2020 2022 3122 3a20  s": {.     "1": 
-00001720: 7b7d 2c0a 2020 2020 2022 3322 3a20 7b7d  {},.     "3": {}
-00001730: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
-00001740: 2247 6574 4963 6f6e 5375 6974 6522 3a20  "GetIconSuite": 
-00001750: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
-00001760: 2020 2020 2022 3022 3a20 7b7d 0a20 2020       "0": {}.   
-00001770: 207d 0a20 2020 7d2c 0a20 2020 2247 6574   }.   },.   "Get
-00001780: 4c61 6265 6c22 3a20 7b0a 2020 2020 2261  Label": {.    "a
-00001790: 7267 7322 3a20 7b0a 2020 2020 2022 3122  rgs": {.     "1"
-000017a0: 3a20 7b7d 0a20 2020 207d 0a20 2020 7d2c  : {}.    }.   },
-000017b0: 0a20 2020 2247 6574 4e65 7874 5072 6f63  .   "GetNextProc
-000017c0: 6573 7322 3a20 7b0a 2020 2020 2261 7267  ess": {.    "arg
-000017d0: 7322 3a20 7b0a 2020 2020 2022 3022 3a20  s": {.     "0": 
-000017e0: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
-000017f0: 2020 2247 6574 5072 6f63 6573 7342 756e    "GetProcessBun
-00001800: 646c 654c 6f63 6174 696f 6e22 3a20 7b0a  dleLocation": {.
-00001810: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-00001820: 2020 2022 3022 3a20 7b7d 2c0a 2020 2020     "0": {},.    
-00001830: 2022 3122 3a20 7b7d 0a20 2020 207d 0a20   "1": {}.    }. 
-00001840: 2020 7d2c 0a20 2020 2247 6574 5072 6f63    },.   "GetProc
-00001850: 6573 7346 6f72 5049 4422 3a20 7b0a 2020  essForPID": {.  
-00001860: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
-00001870: 2022 3122 3a20 7b7d 0a20 2020 207d 0a20   "1": {}.    }. 
-00001880: 2020 7d2c 0a20 2020 2247 6574 5072 6f63    },.   "GetProc
-00001890: 6573 7349 6e66 6f72 6d61 7469 6f6e 223a  essInformation":
-000018a0: 207b 0a20 2020 2022 6172 6773 223a 207b   {.    "args": {
-000018b0: 0a20 2020 2020 2230 223a 207b 7d2c 0a20  .     "0": {},. 
-000018c0: 2020 2020 2231 223a 207b 7d0a 2020 2020      "1": {}.    
-000018d0: 7d0a 2020 207d 2c0a 2020 2022 4765 7450  }.   },.   "GetP
-000018e0: 726f 6365 7373 5049 4422 3a20 7b0a 2020  rocessPID": {.  
-000018f0: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
-00001900: 2022 3022 3a20 7b7d 2c0a 2020 2020 2022   "0": {},.     "
-00001910: 3122 3a20 7b7d 0a20 2020 207d 0a20 2020  1": {}.    }.   
-00001920: 7d2c 0a20 2020 2247 6574 5375 6974 654c  },.   "GetSuiteL
-00001930: 6162 656c 223a 207b 0a20 2020 2022 6172  abel": {.    "ar
-00001940: 6773 223a 207b 0a20 2020 2020 2230 223a  gs": {.     "0":
-00001950: 207b 7d0a 2020 2020 7d0a 2020 207d 2c0a   {}.    }.   },.
-00001960: 2020 2022 4849 5368 6170 6543 6f6e 7461     "HIShapeConta
-00001970: 696e 7350 6f69 6e74 223a 207b 0a20 2020  insPoint": {.   
-00001980: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
-00001990: 2231 223a 207b 2022 7479 7065 5f6d 6f64  "1": { "type_mod
-000019a0: 6966 6965 7222 3a20 226e 2220 7d0a 2020  ifier": "n" }.  
-000019b0: 2020 7d0a 2020 207d 2c0a 2020 2022 4849    }.   },.   "HI
-000019c0: 5368 6170 6543 7265 6174 654d 7574 6162  ShapeCreateMutab
-000019d0: 6c65 5769 7468 5265 6374 223a 207b 0a20  leWithRect": {. 
-000019e0: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
-000019f0: 2020 2230 223a 207b 2022 7479 7065 5f6d    "0": { "type_m
-00001a00: 6f64 6966 6965 7222 3a20 226e 2220 7d0a  odifier": "n" }.
-00001a10: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
-00001a20: 4849 5368 6170 6543 7265 6174 6557 6974  HIShapeCreateWit
-00001a30: 6851 4452 676e 223a 207b 2022 6967 6e6f  hQDRgn": { "igno
-00001a40: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
-00001a50: 2248 4953 6861 7065 4372 6561 7465 5769  "HIShapeCreateWi
-00001a60: 7468 5265 6374 223a 207b 0a20 2020 2022  thRect": {.    "
-00001a70: 6172 6773 223a 207b 0a20 2020 2020 2230  args": {.     "0
-00001a80: 223a 207b 2022 7479 7065 5f6d 6f64 6966  ": { "type_modif
-00001a90: 6965 7222 3a20 226e 2220 7d0a 2020 2020  ier": "n" }.    
-00001aa0: 7d0a 2020 207d 2c0a 2020 2022 4849 5368  }.   },.   "HISh
-00001ab0: 6170 6553 6574 5144 436c 6970 223a 207b  apeSetQDClip": {
-00001ac0: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
-00001ad0: 7d2c 0a20 2020 2248 4953 6861 7065 556e  },.   "HIShapeUn
-00001ae0: 696f 6e57 6974 6852 6563 7422 3a20 7b0a  ionWithRect": {.
-00001af0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-00001b00: 2020 2022 3122 3a20 7b20 2274 7970 655f     "1": { "type_
-00001b10: 6d6f 6469 6669 6572 223a 2022 6e22 7d0a  modifier": "n"}.
-00001b20: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
-00001b30: 4849 5368 6170 6545 6e75 6d65 7261 7465  HIShapeEnumerate
-00001b40: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-00001b50: 207b 0a20 2020 2020 2232 223a 207b 0a20   {.     "2": {. 
-00001b60: 2020 2020 2022 6361 6c6c 6162 6c65 5f72       "callable_r
-00001b70: 6574 6169 6e65 6422 3a20 6661 6c73 652c  etained": false,
-00001b80: 0a20 2020 2020 2022 6675 6e63 7469 6f6e  .      "function
-00001b90: 223a 207b 0a20 2020 2020 2020 2261 7267  ": {.       "arg
-00001ba0: 7322 3a20 5b0a 2020 2020 2020 2020 7b0a  s": [.        {.
-00001bb0: 2020 2020 2020 2020 2022 7479 7065 7374           "typest
-00001bc0: 7222 3a20 2269 220a 2020 2020 2020 2020  r": "i".        
-00001bd0: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
-00001be0: 2020 2020 2020 2274 7970 6573 7472 223a        "typestr":
-00001bf0: 2022 5e7b 5f5f 4849 5368 6170 653d 7d22   "^{__HIShape=}"
-00001c00: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-00001c10: 2020 2020 7b0a 2020 2020 2020 2020 2022      {.         "
-00001c20: 7479 7065 7374 7222 3a20 5b20 225e 7b43  typestr": [ "^{C
-00001c30: 4752 6563 743d 7b43 4750 6f69 6e74 3d66  GRect={CGPoint=f
-00001c40: 667d 7b43 4753 697a 653d 6666 7d7d 222c  f}{CGSize=ff}}",
-00001c50: 2022 5e7b 4347 5265 6374 3d7b 4347 506f   "^{CGRect={CGPo
-00001c60: 696e 743d 6464 7d7b 4347 5369 7a65 3d64  int=dd}{CGSize=d
-00001c70: 647d 7d22 2020 5d2c 0a09 2022 7479 7065  d}}"  ],.. "type
-00001c80: 5f6d 6f64 6966 6965 7222 3a20 226e 220a  _modifier": "n".
-00001c90: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00001ca0: 2020 207b 0a20 2020 2020 2020 2020 2274     {.         "t
-00001cb0: 7970 6573 7472 223a 2022 5e76 220a 2020  ypestr": "^v".  
-00001cc0: 2020 2020 2020 7d0a 2020 2020 2020 205d        }.       ]
-00001cd0: 2c0a 2020 2020 2020 2022 7265 7476 616c  ,.       "retval
-00001ce0: 223a 207b 0a20 2020 2020 2020 2022 7479  ": {.        "ty
-00001cf0: 7065 7374 7222 3a20 2269 220a 2020 2020  pestr": "i".    
-00001d00: 2020 207d 0a20 2020 2020 207d 0a20 2020     }.      }.   
-00001d10: 2020 7d0a 2020 2020 7d0a 2020 207d 2c0a    }.    }.   },.
-00001d20: 2020 2022 4849 5368 6170 6547 6574 426f     "HIShapeGetBo
-00001d30: 756e 6473 223a 207b 0a20 2020 2022 6172  unds": {.    "ar
-00001d40: 6773 223a 207b 0a20 2020 2020 2231 223a  gs": {.     "1":
-00001d50: 207b 2022 7479 7065 5f6d 6f64 6966 6965   { "type_modifie
-00001d60: 7222 3a20 226f 2220 7d0a 2020 2020 7d0a  r": "o" }.    }.
-00001d70: 2020 207d 2c0a 2020 2022 4849 5368 6170     },.   "HIShap
-00001d80: 6547 6574 4173 5144 5267 6e22 3a20 7b20  eGetAsQDRgn": { 
-00001d90: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
-00001da0: 2c0a 2020 2022 4849 5368 6170 6549 6e74  ,.   "HIShapeInt
-00001db0: 6572 7365 6374 7352 6563 7422 3a20 7b0a  ersectsRect": {.
-00001dc0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-00001dd0: 2020 2022 3122 3a20 7b20 2274 7970 655f     "1": { "type_
-00001de0: 6d6f 6469 6669 6572 223a 2022 6e22 207d  modifier": "n" }
-00001df0: 0a20 2020 207d 2c0a 2020 2020 2272 6574  .    },.    "ret
-00001e00: 7661 6c22 3a20 7b0a 2020 2020 2022 635f  val": {.     "c_
-00001e10: 6172 7261 795f 6f66 5f66 6978 6564 5f6c  array_of_fixed_l
-00001e20: 656e 6774 6822 3a20 310a 2020 2020 7d0a  ength": 1.    }.
-00001e30: 2020 207d 2c0a 2020 2022 4943 4164 644d     },.   "ICAddM
-00001e40: 6170 456e 7472 7922 3a20 7b20 2269 676e  apEntry": { "ign
-00001e50: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
-00001e60: 2022 4943 4164 6450 726f 6669 6c65 223a   "ICAddProfile":
-00001e70: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
-00001e80: 6520 7d2c 0a20 2020 2249 4342 6567 696e  e },.   "ICBegin
-00001e90: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00001ea0: 7275 6520 7d2c 0a20 2020 2249 4343 6f75  rue },.   "ICCou
-00001eb0: 6e74 4d61 7045 6e74 7269 6573 223a 207b  ntMapEntries": {
-00001ec0: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
-00001ed0: 7d2c 0a20 2020 2249 4343 6f75 6e74 5072  },.   "ICCountPr
-00001ee0: 6566 223a 207b 2022 6967 6e6f 7265 223a  ef": { "ignore":
-00001ef0: 2074 7275 6520 7d2c 0a20 2020 2249 4343   true },.   "ICC
-00001f00: 6f75 6e74 5072 6f66 696c 6573 223a 207b  ountProfiles": {
-00001f10: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
-00001f20: 7d2c 0a20 2020 2249 4343 7265 6174 6547  },.   "ICCreateG
-00001f30: 5552 4c45 7665 6e74 223a 207b 2022 6967  URLEvent": { "ig
-00001f40: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
-00001f50: 2020 2249 4344 656c 6574 654d 6170 456e    "ICDeleteMapEn
-00001f60: 7472 7922 3a20 7b20 2269 676e 6f72 6522  try": { "ignore"
-00001f70: 3a20 7472 7565 207d 2c0a 2020 2022 4943  : true },.   "IC
-00001f80: 4465 6c65 7465 5072 6566 223a 207b 2022  DeletePref": { "
-00001f90: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-00001fa0: 0a20 2020 2249 4344 656c 6574 6550 726f  .   "ICDeletePro
-00001fb0: 6669 6c65 223a 207b 2022 6967 6e6f 7265  file": { "ignore
-00001fc0: 223a 2074 7275 6520 7d2c 0a20 2020 2249  ": true },.   "I
-00001fd0: 4345 6469 7450 7265 6665 7265 6e63 6573  CEditPreferences
-00001fe0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00001ff0: 7275 6520 7d2c 0a20 2020 2249 4345 6e64  rue },.   "ICEnd
-00002000: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00002010: 7275 6520 7d2c 0a20 2020 2249 4346 696e  rue },.   "ICFin
-00002020: 6450 7265 6648 616e 646c 6522 3a20 7b20  dPrefHandle": { 
-00002030: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
-00002040: 2c0a 2020 2022 4943 4765 7443 6f6e 6669  ,.   "ICGetConfi
-00002050: 674e 616d 6522 3a20 7b20 2269 676e 6f72  gName": { "ignor
-00002060: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-00002070: 4943 4765 7443 7572 7265 6e74 5072 6f66  ICGetCurrentProf
-00002080: 696c 6522 3a20 7b20 2269 676e 6f72 6522  ile": { "ignore"
-00002090: 3a20 7472 7565 207d 2c0a 2020 2022 4943  : true },.   "IC
-000020a0: 4765 7444 6566 6175 6c74 5072 6566 223a  GetDefaultPref":
-000020b0: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
-000020c0: 6520 7d2c 0a20 2020 2249 4347 6574 496e  e },.   "ICGetIn
-000020d0: 644d 6170 456e 7472 7922 3a20 7b20 2269  dMapEntry": { "i
-000020e0: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
-000020f0: 2020 2022 4943 4765 7449 6e64 5072 6566     "ICGetIndPref
-00002100: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00002110: 7275 6520 7d2c 0a20 2020 2249 4347 6574  rue },.   "ICGet
-00002120: 496e 6450 726f 6669 6c65 223a 207b 2022  IndProfile": { "
-00002130: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-00002140: 0a20 2020 2249 4347 6574 4d61 7045 6e74  .   "ICGetMapEnt
-00002150: 7279 223a 207b 2022 6967 6e6f 7265 223a  ry": { "ignore":
-00002160: 2074 7275 6520 7d2c 0a20 2020 2249 4347   true },.   "ICG
-00002170: 6574 5065 726d 223a 207b 2022 6967 6e6f  etPerm": { "igno
-00002180: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
-00002190: 2249 4347 6574 5072 6566 223a 207b 2022  "ICGetPref": { "
-000021a0: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-000021b0: 0a20 2020 2249 4347 6574 5072 6566 4861  .   "ICGetPrefHa
-000021c0: 6e64 6c65 223a 207b 2022 6967 6e6f 7265  ndle": { "ignore
-000021d0: 223a 2074 7275 6520 7d2c 0a20 2020 2249  ": true },.   "I
-000021e0: 4347 6574 5072 6f66 696c 654e 616d 6522  CGetProfileName"
-000021f0: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-00002200: 7565 207d 2c0a 2020 2022 4943 4765 7453  ue },.   "ICGetS
-00002210: 6565 6422 3a20 7b20 2269 676e 6f72 6522  eed": { "ignore"
-00002220: 3a20 7472 7565 207d 2c0a 2020 2022 4943  : true },.   "IC
-00002230: 4765 7456 6572 7369 6f6e 223a 207b 2022  GetVersion": { "
-00002240: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-00002250: 0a20 2020 2249 434c 6175 6e63 6855 524c  .   "ICLaunchURL
-00002260: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00002270: 7275 6520 7d2c 0a20 2020 2249 434d 6170  rue },.   "ICMap
-00002280: 456e 7472 6965 7346 696c 656e 616d 6522  EntriesFilename"
-00002290: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-000022a0: 7565 207d 2c0a 2020 2022 4943 4d61 7045  ue },.   "ICMapE
-000022b0: 6e74 7269 6573 5479 7065 4372 6561 746f  ntriesTypeCreato
-000022c0: 7222 3a20 7b20 2269 676e 6f72 6522 3a20  r": { "ignore": 
-000022d0: 7472 7565 207d 2c0a 2020 2022 4943 4d61  true },.   "ICMa
-000022e0: 7046 696c 656e 616d 6522 3a20 7b20 2269  pFilename": { "i
-000022f0: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
-00002300: 2020 2022 4943 4d61 7054 7970 6543 7265     "ICMapTypeCre
-00002310: 6174 6f72 223a 207b 2022 6967 6e6f 7265  ator": { "ignore
-00002320: 223a 2074 7275 6520 7d2c 0a20 2020 2249  ": true },.   "I
-00002330: 4350 6172 7365 5552 4c22 3a20 7b20 2269  CParseURL": { "i
-00002340: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
-00002350: 2020 2022 4943 5365 6e64 4755 524c 4576     "ICSendGURLEv
-00002360: 656e 7422 3a20 7b20 2269 676e 6f72 6522  ent": { "ignore"
-00002370: 3a20 7472 7565 207d 2c0a 2020 2022 4943  : true },.   "IC
-00002380: 5365 7443 7572 7265 6e74 5072 6f66 696c  SetCurrentProfil
-00002390: 6522 3a20 7b20 2269 676e 6f72 6522 3a20  e": { "ignore": 
-000023a0: 7472 7565 207d 2c0a 2020 2022 4943 5365  true },.   "ICSe
-000023b0: 744d 6170 456e 7472 7922 3a20 7b20 2269  tMapEntry": { "i
-000023c0: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
-000023d0: 2020 2022 4943 5365 7450 7265 6622 3a20     "ICSetPref": 
-000023e0: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
-000023f0: 207d 2c0a 2020 2022 4943 5365 7450 7265   },.   "ICSetPre
-00002400: 6648 616e 646c 6522 3a20 7b20 2269 676e  fHandle": { "ign
-00002410: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
-00002420: 2022 4943 5365 7450 726f 6669 6c65 4e61   "ICSetProfileNa
-00002430: 6d65 223a 207b 2022 6967 6e6f 7265 223a  me": { "ignore":
-00002440: 2074 7275 6520 7d2c 0a20 2020 2249 4353   true },.   "ICS
-00002450: 7461 7274 223a 207b 2022 6967 6e6f 7265  tart": { "ignore
-00002460: 223a 2074 7275 6520 7d2c 0a20 2020 2249  ": true },.   "I
-00002470: 4353 746f 7022 3a20 7b20 2269 676e 6f72  CStop": { "ignor
-00002480: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-00002490: 4963 6f6e 4661 6d69 6c79 546f 4963 6f6e  IconFamilyToIcon
-000024a0: 5375 6974 6522 3a20 7b7d 2c0a 2020 2022  Suite": {},.   "
-000024b0: 4963 6f6e 4944 546f 5267 6e22 3a20 7b0a  IconIDToRgn": {.
-000024c0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-000024d0: 2020 2022 3022 3a20 7b7d 2c0a 2020 2020     "0": {},.    
-000024e0: 2022 3122 3a20 7b7d 0a20 2020 207d 0a20   "1": {}.    }. 
-000024f0: 2020 7d2c 0a20 2020 2249 636f 6e4d 6574    },.   "IconMet
-00002500: 686f 6454 6f52 676e 223a 207b 0a20 2020  hodToRgn": {.   
-00002510: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
-00002520: 2230 223a 207b 7d2c 0a20 2020 2020 2231  "0": {},.     "1
-00002530: 223a 207b 7d2c 0a20 2020 2020 2233 223a  ": {},.     "3":
-00002540: 207b 7d2c 0a20 2020 2020 2234 223a 207b   {},.     "4": {
-00002550: 7d0a 2020 2020 7d0a 2020 207d 2c0a 2020  }.    }.   },.  
-00002560: 2022 4963 6f6e 5265 6643 6f6e 7461 696e   "IconRefContain
-00002570: 7343 4750 6f69 6e74 223a 207b 0a20 2020  sCGPoint": {.   
-00002580: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
-00002590: 2230 223a 207b 7d2c 0a20 2020 2020 2231  "0": {},.     "1
-000025a0: 223a 207b 7d2c 0a20 2020 2020 2234 223a  ": {},.     "4":
-000025b0: 207b 7d0a 2020 2020 7d0a 2020 207d 2c0a   {}.    }.   },.
-000025c0: 2020 2022 4963 6f6e 5265 6649 6e74 6572     "IconRefInter
-000025d0: 7365 6374 7343 4752 6563 7422 3a20 7b0a  sectsCGRect": {.
-000025e0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-000025f0: 2020 2022 3022 3a20 7b7d 2c0a 2020 2020     "0": {},.    
-00002600: 2022 3122 3a20 7b7d 2c0a 2020 2020 2022   "1": {},.     "
-00002610: 3422 3a20 7b7d 0a20 2020 207d 0a20 2020  4": {}.    }.   
-00002620: 7d2c 0a20 2020 2249 636f 6e52 6566 546f  },.   "IconRefTo
-00002630: 4849 5368 6170 6522 3a20 7b0a 2020 2020  HIShape": {.    
-00002640: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
-00002650: 3022 3a20 7b7d 2c0a 2020 2020 2022 3322  0": {},.     "3"
-00002660: 3a20 7b7d 0a20 2020 207d 2c0a 2020 2020  : {}.    },.    
-00002670: 2272 6574 7661 6c22 3a20 7b7d 0a20 2020  "retval": {}.   
-00002680: 7d2c 0a20 2020 2249 636f 6e52 6566 546f  },.   "IconRefTo
-00002690: 4963 6f6e 4661 6d69 6c79 223a 207b 0a20  IconFamily": {. 
-000026a0: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
-000026b0: 2020 2230 223a 207b 7d2c 0a20 2020 2020    "0": {},.     
-000026c0: 2232 223a 207b 7d0a 2020 2020 7d0a 2020  "2": {}.    }.  
-000026d0: 207d 2c0a 2020 2022 4963 6f6e 5265 6654   },.   "IconRefT
-000026e0: 6f52 676e 223a 207b 0a20 2020 2022 6172  oRgn": {.    "ar
-000026f0: 6773 223a 207b 0a20 2020 2020 2230 223a  gs": {.     "0":
-00002700: 207b 7d2c 0a20 2020 2020 2231 223a 207b   {},.     "1": {
-00002710: 7d2c 0a20 2020 2020 2234 223a 207b 7d0a  },.     "4": {}.
-00002720: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
-00002730: 4963 6f6e 5375 6974 6554 6f49 636f 6e46  IconSuiteToIconF
-00002740: 616d 696c 7922 3a20 7b0a 2020 2020 2261  amily": {.    "a
-00002750: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
-00002760: 3a20 7b7d 2c0a 2020 2020 2022 3222 3a20  : {},.     "2": 
-00002770: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
-00002780: 2020 2249 636f 6e53 7569 7465 546f 5267    "IconSuiteToRg
-00002790: 6e22 3a20 7b0a 2020 2020 2261 7267 7322  n": {.    "args"
-000027a0: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
-000027b0: 2c0a 2020 2020 2022 3122 3a20 7b7d 2c0a  ,.     "1": {},.
-000027c0: 2020 2020 2022 3322 3a20 7b7d 0a20 2020       "3": {}.   
-000027d0: 207d 0a20 2020 7d2c 0a20 2020 2249 6e76   }.   },.   "Inv
-000027e0: 6f6b 6549 636f 6e41 6374 696f 6e55 5050  okeIconActionUPP
-000027f0: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-00002800: 207b 0a20 2020 2020 2231 223a 207b 7d2c   {.     "1": {},
-00002810: 0a20 2020 2020 2232 223a 207b 7d2c 0a20  .     "2": {},. 
-00002820: 2020 2020 2233 223a 207b 7d0a 2020 2020      "3": {}.    
-00002830: 7d0a 2020 207d 2c0a 2020 2022 496e 766f  }.   },.   "Invo
-00002840: 6b65 4963 6f6e 4765 7474 6572 5550 5022  keIconGetterUPP"
-00002850: 3a20 7b0a 2020 2020 2261 7267 7322 3a20  : {.    "args": 
-00002860: 7b0a 2020 2020 2022 3122 3a20 7b7d 2c0a  {.     "1": {},.
-00002870: 2020 2020 2022 3222 3a20 7b7d 0a20 2020       "2": {}.   
-00002880: 207d 2c0a 2020 2020 2272 6574 7661 6c22   },.    "retval"
-00002890: 3a20 7b7d 0a20 2020 7d2c 0a20 2020 2249  : {}.   },.   "I
-000028a0: 7349 636f 6e52 6566 4d61 736b 456d 7074  sIconRefMaskEmpt
-000028b0: 7922 3a20 7b0a 2020 2020 2261 7267 7322  y": {.    "args"
-000028c0: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
-000028d0: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
-000028e0: 2249 7350 726f 6365 7373 5669 7369 626c  "IsProcessVisibl
-000028f0: 6522 3a20 7b0a 2020 2020 2261 7267 7322  e": {.    "args"
-00002900: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
-00002910: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
-00002920: 224b 696c 6c50 726f 6365 7373 223a 207b  "KillProcess": {
-00002930: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
-00002940: 2020 2020 2230 223a 207b 7d0a 2020 2020      "0": {}.    
-00002950: 7d0a 2020 207d 2c0a 2020 2022 4c61 756e  }.   },.   "Laun
-00002960: 6368 4170 706c 6963 6174 696f 6e22 3a20  chApplication": 
-00002970: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
-00002980: 207d 2c0a 2020 2022 4c6f 6164 4963 6f6e   },.   "LoadIcon
-00002990: 4361 6368 6522 3a20 7b0a 2020 2020 2261  Cache": {.    "a
-000029a0: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
-000029b0: 3a20 7b7d 2c0a 2020 2020 2022 3322 3a20  : {},.     "3": 
-000029c0: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
-000029d0: 2020 224d 616b 6549 636f 6e43 6163 6865    "MakeIconCache
-000029e0: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-000029f0: 207b 0a20 2020 2020 2230 223a 207b 7d2c   {.     "0": {},
-00002a00: 0a20 2020 2020 2231 223a 207b 7d2c 0a20  .     "1": {},. 
-00002a10: 2020 2020 2232 223a 207b 7d0a 2020 2020      "2": {}.    
-00002a20: 7d0a 2020 207d 2c0a 2020 2022 4e65 7749  }.   },.   "NewI
-00002a30: 636f 6e41 6374 696f 6e55 5050 223a 207b  conActionUPP": {
-00002a40: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
-00002a50: 2020 2020 2230 223a 207b 0a20 2020 2020      "0": {.     
-00002a60: 2022 6675 6e63 7469 6f6e 223a 207b 0a20   "function": {. 
-00002a70: 2020 2020 2020 2261 7267 7322 3a20 5b0a        "args": [.
-00002a80: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00002a90: 2020 2022 7479 7065 7374 7222 3a20 2249     "typestr": "I
-00002aa0: 220a 2020 2020 2020 2020 7d2c 0a20 2020  ".        },.   
-00002ab0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00002ac0: 2274 7970 6573 7472 223a 2022 5e5e 5e63  "typestr": "^^^c
-00002ad0: 220a 2020 2020 2020 2020 7d2c 0a20 2020  ".        },.   
-00002ae0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00002af0: 2274 7970 6573 7472 223a 2022 5e76 220a  "typestr": "^v".
-00002b00: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00002b10: 205d 2c0a 2020 2020 2020 2022 7265 7476   ],.       "retv
-00002b20: 616c 223a 207b 0a20 2020 2020 2020 2022  al": {.        "
-00002b30: 7479 7065 7374 7222 3a20 2273 220a 2020  typestr": "s".  
-00002b40: 2020 2020 207d 0a20 2020 2020 207d 0a20       }.      }. 
-00002b50: 2020 2020 7d0a 2020 2020 7d2c 0a20 2020      }.    },.   
-00002b60: 2022 7265 7476 616c 223a 207b 7d0a 2020   "retval": {}.  
-00002b70: 207d 2c0a 2020 2022 4e65 7749 636f 6e47   },.   "NewIconG
-00002b80: 6574 7465 7255 5050 223a 207b 0a20 2020  etterUPP": {.   
-00002b90: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
-00002ba0: 2230 223a 207b 0a20 2020 2020 2022 6675  "0": {.      "fu
-00002bb0: 6e63 7469 6f6e 223a 207b 0a20 2020 2020  nction": {.     
-00002bc0: 2020 2261 7267 7322 3a20 5b0a 2020 2020    "args": [.    
-00002bd0: 2020 2020 7b0a 2020 2020 2020 2020 2022      {.         "
-00002be0: 7479 7065 7374 7222 3a20 2249 220a 2020  typestr": "I".  
-00002bf0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00002c00: 207b 0a20 2020 2020 2020 2020 2274 7970   {.         "typ
-00002c10: 6573 7472 223a 2022 5e76 220a 2020 2020  estr": "^v".    
-00002c20: 2020 2020 7d0a 2020 2020 2020 205d 2c0a      }.       ],.
-00002c30: 2020 2020 2020 2022 7265 7476 616c 223a         "retval":
-00002c40: 207b 0a20 2020 2020 2020 2022 7479 7065   {.        "type
-00002c50: 7374 7222 3a20 225e 5e63 220a 2020 2020  str": "^^c".    
-00002c60: 2020 207d 0a20 2020 2020 207d 0a20 2020     }.      }.   
-00002c70: 2020 7d0a 2020 2020 7d2c 0a20 2020 2022    }.    },.    "
-00002c80: 7265 7476 616c 223a 207b 7d0a 2020 207d  retval": {}.   }
-00002c90: 2c0a 2020 2022 4e65 7749 636f 6e53 7569  ,.   "NewIconSui
-00002ca0: 7465 223a 207b 0a20 2020 2022 6172 6773  te": {.    "args
-00002cb0: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
-00002cc0: 7d0a 2020 2020 7d0a 2020 207d 2c0a 2020  }.    }.   },.  
-00002cd0: 2022 5061 7374 6562 6f61 7264 436c 6561   "PasteboardClea
-00002ce0: 7222 3a20 7b0a 2020 2020 2261 7267 7322  r": {.    "args"
-00002cf0: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
-00002d00: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
-00002d10: 2250 6173 7465 626f 6172 6443 6f70 7949  "PasteboardCopyI
-00002d20: 7465 6d46 6c61 766f 7244 6174 6122 3a20  temFlavorData": 
-00002d30: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
-00002d40: 2020 2020 2022 3022 3a20 7b7d 2c0a 2020       "0": {},.  
-00002d50: 2020 2022 3122 3a20 7b7d 2c0a 2020 2020     "1": {},.    
-00002d60: 2022 3222 3a20 7b7d 2c0a 2020 2020 2022   "2": {},.     "
-00002d70: 3322 3a20 7b7d 0a20 2020 207d 0a20 2020  3": {}.    }.   
-00002d80: 7d2c 0a20 2020 2250 6173 7465 626f 6172  },.   "Pasteboar
-00002d90: 6443 6f70 7949 7465 6d46 6c61 766f 7273  dCopyItemFlavors
-00002da0: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-00002db0: 207b 0a20 2020 2020 2230 223a 207b 7d2c   {.     "0": {},
-00002dc0: 0a20 2020 2020 2231 223a 207b 7d2c 0a20  .     "1": {},. 
-00002dd0: 2020 2020 2232 223a 207b 7d0a 2020 2020      "2": {}.    
-00002de0: 7d0a 2020 207d 2c0a 2020 2022 5061 7374  }.   },.   "Past
-00002df0: 6562 6f61 7264 436f 7079 4e61 6d65 223a  eboardCopyName":
-00002e00: 207b 0a20 2020 2022 6172 6773 223a 207b   {.    "args": {
-00002e10: 0a20 2020 2020 2230 223a 207b 7d2c 0a20  .     "0": {},. 
-00002e20: 2020 2020 2231 223a 207b 7d0a 2020 2020      "1": {}.    
-00002e30: 7d0a 2020 207d 2c0a 2020 2022 5061 7374  }.   },.   "Past
-00002e40: 6562 6f61 7264 436f 7079 5061 7374 654c  eboardCopyPasteL
-00002e50: 6f63 6174 696f 6e22 3a20 7b0a 2020 2020  ocation": {.    
-00002e60: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
-00002e70: 3022 3a20 7b7d 2c0a 2020 2020 2022 3122  0": {},.     "1"
-00002e80: 3a20 7b7d 0a20 2020 207d 0a20 2020 7d2c  : {}.    }.   },
-00002e90: 0a20 2020 2250 6173 7465 626f 6172 6443  .   "PasteboardC
-00002ea0: 7265 6174 6522 3a20 7b0a 2020 2020 2261  reate": {.    "a
-00002eb0: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
-00002ec0: 3a20 7b7d 2c0a 2020 2020 2022 3122 3a20  : {},.     "1": 
-00002ed0: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
-00002ee0: 2020 2250 6173 7465 626f 6172 6447 6574    "PasteboardGet
-00002ef0: 4974 656d 436f 756e 7422 3a20 7b0a 2020  ItemCount": {.  
-00002f00: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
-00002f10: 2022 3022 3a20 7b7d 2c0a 2020 2020 2022   "0": {},.     "
-00002f20: 3122 3a20 7b7d 0a20 2020 207d 0a20 2020  1": {}.    }.   
-00002f30: 7d2c 0a20 2020 2250 6173 7465 626f 6172  },.   "Pasteboar
-00002f40: 6447 6574 4974 656d 466c 6176 6f72 466c  dGetItemFlavorFl
-00002f50: 6167 7322 3a20 7b0a 2020 2020 2261 7267  ags": {.    "arg
-00002f60: 7322 3a20 7b0a 2020 2020 2022 3022 3a20  s": {.     "0": 
-00002f70: 7b7d 2c0a 2020 2020 2022 3122 3a20 7b7d  {},.     "1": {}
-00002f80: 2c0a 2020 2020 2022 3222 3a20 7b7d 2c0a  ,.     "2": {},.
-00002f90: 2020 2020 2022 3322 3a20 7b7d 0a20 2020       "3": {}.   
-00002fa0: 207d 0a20 2020 7d2c 0a20 2020 2250 6173   }.   },.   "Pas
-00002fb0: 7465 626f 6172 6447 6574 4974 656d 4964  teboardGetItemId
-00002fc0: 656e 7469 6669 6572 223a 207b 0a20 2020  entifier": {.   
-00002fd0: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
-00002fe0: 2230 223a 207b 7d2c 0a20 2020 2020 2232  "0": {},.     "2
-00002ff0: 223a 207b 7d0a 2020 2020 7d0a 2020 207d  ": {}.    }.   }
-00003000: 2c0a 2020 2022 5061 7374 6562 6f61 7264  ,.   "Pasteboard
-00003010: 5075 7449 7465 6d46 6c61 766f 7222 3a20  PutItemFlavor": 
-00003020: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
-00003030: 2020 2020 2022 3022 3a20 7b7d 2c0a 2020       "0": {},.  
-00003040: 2020 2022 3122 3a20 7b7d 2c0a 2020 2020     "1": {},.    
-00003050: 2022 3222 3a20 7b7d 2c0a 2020 2020 2022   "2": {},.     "
-00003060: 3322 3a20 7b7d 0a20 2020 207d 0a20 2020  3": {}.    }.   
-00003070: 7d2c 0a20 2020 2250 6173 7465 626f 6172  },.   "Pasteboar
-00003080: 6452 6573 6f6c 7665 5072 6f6d 6973 6573  dResolvePromises
-00003090: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-000030a0: 207b 0a20 2020 2020 2230 223a 207b 7d0a   {.     "0": {}.
-000030b0: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
-000030c0: 5061 7374 6562 6f61 7264 5365 7450 6173  PasteboardSetPas
-000030d0: 7465 4c6f 6361 7469 6f6e 223a 207b 0a20  teLocation": {. 
-000030e0: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
-000030f0: 2020 2230 223a 207b 7d2c 0a20 2020 2020    "0": {},.     
-00003100: 2231 223a 207b 7d0a 2020 2020 7d0a 2020  "1": {}.    }.  
-00003110: 207d 2c0a 2020 2022 5061 7374 6562 6f61   },.   "Pasteboa
-00003120: 7264 5365 7450 726f 6d69 7365 4b65 6570  rdSetPromiseKeep
-00003130: 6572 223a 207b 0a20 2020 2022 6172 6773  er": {.    "args
-00003140: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
-00003150: 7d2c 0a20 2020 2020 2231 223a 207b 0a20  },.     "1": {. 
-00003160: 2020 2020 2022 6675 6e63 7469 6f6e 223a       "function":
-00003170: 207b 0a20 2020 2020 2020 2261 7267 7322   {.       "args"
-00003180: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
-00003190: 2020 2020 2020 2022 7479 7065 7374 7222         "typestr"
-000031a0: 3a20 225e 7b4f 7061 7175 6550 6173 7465  : "^{OpaquePaste
-000031b0: 626f 6172 6452 6566 3d7d 220a 2020 2020  boardRef=}".    
-000031c0: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
-000031d0: 0a20 2020 2020 2020 2020 2274 7970 6573  .         "types
-000031e0: 7472 223a 2022 5e76 220a 2020 2020 2020  tr": "^v".      
-000031f0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
-00003200: 2020 2020 2020 2020 2274 7970 6573 7472          "typestr
-00003210: 223a 2022 5e7b 5f5f 4346 5374 7269 6e67  ": "^{__CFString
-00003220: 3d7d 220a 2020 2020 2020 2020 7d2c 0a20  =}".        },. 
-00003230: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00003240: 2020 2274 7970 6573 7472 223a 2022 5e76    "typestr": "^v
-00003250: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
-00003260: 2020 205d 2c0a 2020 2020 2020 2022 7265     ],.       "re
-00003270: 7476 616c 223a 207b 0a20 2020 2020 2020  tval": {.       
-00003280: 2022 7479 7065 7374 7222 3a20 2269 220a   "typestr": "i".
-00003290: 2020 2020 2020 207d 0a20 2020 2020 207d         }.      }
-000032a0: 0a20 2020 2020 7d2c 0a20 2020 2020 2232  .     },.     "2
-000032b0: 223a 207b 7d0a 2020 2020 7d0a 2020 207d  ": {}.    }.   }
+00000000: 7b0a 2022 6465 6669 6e69 7469 6f6e 7322  {. "definitions"
+00000010: 3a20 7b0a 2020 2263 6c61 7373 6573 223a  : {.  "classes":
+00000020: 207b 7d2c 0a20 2022 666f 726d 616c 5f70   {},.  "formal_p
+00000030: 726f 746f 636f 6c73 223a 207b 7d2c 0a20  rotocols": {},. 
+00000040: 2022 6675 6e63 7469 6f6e 7322 3a20 7b0a   "functions": {.
+00000050: 2020 2022 4158 5465 7874 4d61 726b 6572     "AXTextMarker
+00000060: 5261 6e67 6543 7265 6174 6557 6974 6842  RangeCreateWithB
+00000070: 7974 6573 223a 207b 0a20 2020 2022 6172  ytes": {.    "ar
+00000080: 6773 223a 207b 0a20 2020 2020 2231 223a  gs": {.     "1":
+00000090: 207b 2022 7479 7065 5f6d 6f64 6966 6965   { "type_modifie
+000000a0: 7222 3a20 226e 222c 2022 635f 6172 7261  r": "n", "c_arra
+000000b0: 795f 6c65 6e67 7468 5f69 6e5f 6172 6722  y_length_in_arg"
+000000c0: 3a20 3220 7d2c 0a20 2020 2020 2233 223a  : 2 },.     "3":
+000000d0: 207b 2022 7479 7065 5f6d 6f64 6966 6965   { "type_modifie
+000000e0: 7222 3a20 226e 222c 2022 635f 6172 7261  r": "n", "c_arra
+000000f0: 795f 6c65 6e67 7468 5f69 6e5f 6172 6722  y_length_in_arg"
+00000100: 3a20 3420 7d0a 2020 2020 7d2c 0a20 2020  : 4 }.    },.   
+00000110: 2022 7265 7476 616c 223a 207b 2022 616c   "retval": { "al
+00000120: 7265 6164 795f 6366 7265 7461 696e 6564  ready_cfretained
+00000130: 223a 2074 7275 6520 7d0a 2020 207d 2c0a  ": true }.   },.
+00000140: 2020 2022 4158 5465 7874 4d61 726b 6572     "AXTextMarker
+00000150: 4372 6561 7465 223a 207b 0a20 2020 2022  Create": {.    "
+00000160: 6172 6773 223a 7b0a 2020 2020 2022 3122  args":{.     "1"
+00000170: 3a20 7b20 2274 7970 655f 6d6f 6469 6669  : { "type_modifi
+00000180: 6572 223a 2022 6e22 2c20 2263 5f61 7272  er": "n", "c_arr
+00000190: 6179 5f6c 656e 6774 685f 696e 5f61 7267  ay_length_in_arg
+000001a0: 223a 2032 207d 0a20 2020 207d 2c0a 2020  ": 2 }.    },.  
+000001b0: 2020 2272 6574 7661 6c22 3a20 7b20 2261    "retval": { "a
+000001c0: 6c72 6561 6479 5f63 6672 6574 6169 6e65  lready_cfretaine
+000001d0: 6422 3a20 7472 7565 207d 0a20 2020 7d2c  d": true }.   },
+000001e0: 0a20 2020 2241 5854 6578 744d 6172 6b65  .   "AXTextMarke
+000001f0: 7247 6574 4279 7465 5074 7222 3a20 7b0a  rGetBytePtr": {.
+00000200: 2020 2020 2272 6574 7661 6c22 3a20 7b20      "retval": { 
+00000210: 2263 5f61 7272 6179 5f6f 665f 7661 7269  "c_array_of_vari
+00000220: 6162 6c65 5f6c 656e 6774 6822 3a20 7472  able_length": tr
+00000230: 7565 207d 0a20 2020 7d2c 0a20 2020 2241  ue }.   },.   "A
+00000240: 5849 7350 726f 6365 7373 5472 7573 7465  XIsProcessTruste
+00000250: 6457 6974 684f 7074 696f 6e73 223a 207b  dWithOptions": {
+00000260: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
+00000270: 2020 2020 2230 223a 207b 7d0a 2020 2020      "0": {}.    
+00000280: 7d0a 2020 207d 2c0a 2020 2022 4158 4d61  }.   },.   "AXMa
+00000290: 6b65 5072 6f63 6573 7354 7275 7374 6564  keProcessTrusted
+000002a0: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
+000002b0: 207b 0a20 2020 2020 2230 223a 207b 7d0a   {.     "0": {}.
+000002c0: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
+000002d0: 4158 4f62 7365 7276 6572 4164 644e 6f74  AXObserverAddNot
+000002e0: 6966 6963 6174 696f 6e22 3a20 7b0a 2020  ification": {.  
+000002f0: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
+00000300: 2022 3022 3a20 7b7d 2c0a 2020 2020 2022   "0": {},.     "
+00000310: 3122 3a20 7b7d 2c0a 2020 2020 2022 3222  1": {},.     "2"
+00000320: 3a20 7b7d 2c0a 2020 2020 2022 3322 3a20  : {},.     "3": 
+00000330: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
+00000340: 2020 2241 584f 6273 6572 7665 7243 7265    "AXObserverCre
+00000350: 6174 6522 3a20 7b0a 2020 2020 2261 7267  ate": {.    "arg
+00000360: 7322 3a20 7b0a 2020 2020 2022 3122 3a20  s": {.     "1": 
+00000370: 7b0a 2020 2020 2020 2266 756e 6374 696f  {.      "functio
+00000380: 6e22 3a20 7b0a 2020 2020 2020 2022 6172  n": {.       "ar
+00000390: 6773 223a 205b 0a20 2020 2020 2020 207b  gs": [.        {
+000003a0: 0a20 2020 2020 2020 2020 2274 7970 6573  .         "types
+000003b0: 7472 223a 2022 5e7b 5f5f 4158 4f62 7365  tr": "^{__AXObse
+000003c0: 7276 6572 3d7d 220a 2020 2020 2020 2020  rver=}".        
+000003d0: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+000003e0: 2020 2020 2020 2274 7970 6573 7472 223a        "typestr":
+000003f0: 2022 5e7b 5f5f 4158 5549 456c 656d 656e   "^{__AXUIElemen
+00000400: 743d 7d22 0a20 2020 2020 2020 207d 2c0a  t=}".        },.
+00000410: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00000420: 2020 2022 7479 7065 7374 7222 3a20 225e     "typestr": "^
+00000430: 7b5f 5f43 4653 7472 696e 673d 7d22 0a20  {__CFString=}". 
+00000440: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00000450: 2020 7b0a 2020 2020 2020 2020 2022 7479    {.         "ty
+00000460: 7065 7374 7222 3a20 225e 7622 0a20 2020  pestr": "^v".   
+00000470: 2020 2020 207d 0a20 2020 2020 2020 5d2c       }.       ],
+00000480: 0a20 2020 2020 2020 2272 6574 7661 6c22  .       "retval"
+00000490: 3a20 7b0a 2020 2020 2020 2020 2274 7970  : {.        "typ
+000004a0: 6573 7472 223a 2022 7622 0a20 2020 2020  estr": "v".     
+000004b0: 2020 7d0a 2020 2020 2020 7d0a 2020 2020    }.      }.    
+000004c0: 207d 2c0a 2020 2020 2022 3222 3a20 7b20   },.     "2": { 
+000004d0: 2274 7970 655f 6d6f 6469 6669 6572 223a  "type_modifier":
+000004e0: 2022 6f22 2c20 2261 6c72 6561 6479 5f63   "o", "already_c
+000004f0: 6672 6574 6169 6e65 6422 3a20 7472 7565  fretained": true
+00000500: 207d 0a20 2020 207d 0a20 2020 7d2c 0a20   }.    }.   },. 
+00000510: 2020 2241 584f 6273 6572 7665 7243 7265    "AXObserverCre
+00000520: 6174 6557 6974 6849 6e66 6f43 616c 6c62  ateWithInfoCallb
+00000530: 6163 6b22 3a20 7b0a 2020 2020 2261 7267  ack": {.    "arg
+00000540: 7322 3a20 7b0a 2020 2020 2022 3122 3a20  s": {.     "1": 
+00000550: 7b0a 2020 2020 2020 2266 756e 6374 696f  {.      "functio
+00000560: 6e22 3a20 7b0a 2020 2020 2020 2022 6172  n": {.       "ar
+00000570: 6773 223a 205b 0a20 2020 2020 2020 207b  gs": [.        {
+00000580: 0a20 2020 2020 2020 2020 2274 7970 6573  .         "types
+00000590: 7472 223a 2022 5e7b 5f5f 4158 4f62 7365  tr": "^{__AXObse
+000005a0: 7276 6572 3d7d 220a 2020 2020 2020 2020  rver=}".        
+000005b0: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+000005c0: 2020 2020 2020 2274 7970 6573 7472 223a        "typestr":
+000005d0: 2022 5e7b 5f5f 4158 5549 456c 656d 656e   "^{__AXUIElemen
+000005e0: 743d 7d22 0a20 2020 2020 2020 207d 2c0a  t=}".        },.
+000005f0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00000600: 2020 2022 7479 7065 7374 7222 3a20 225e     "typestr": "^
+00000610: 7b5f 5f43 4653 7472 696e 673d 7d22 0a20  {__CFString=}". 
+00000620: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00000630: 2020 7b0a 2020 2020 2020 2020 2022 7479    {.         "ty
+00000640: 7065 7374 7222 3a20 225e 7b5f 5f43 4644  pestr": "^{__CFD
+00000650: 6963 7469 6f6e 6172 793d 7d22 0a20 2020  ictionary=}".   
+00000660: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000670: 7b0a 2020 2020 2020 2020 2022 7479 7065  {.         "type
+00000680: 7374 7222 3a20 225e 7622 0a20 2020 2020  str": "^v".     
+00000690: 2020 207d 0a20 2020 2020 2020 5d2c 0a20     }.       ],. 
+000006a0: 2020 2020 2020 2272 6574 7661 6c22 3a20        "retval": 
+000006b0: 7b0a 2020 2020 2020 2020 2274 7970 6573  {.        "types
+000006c0: 7472 223a 2022 7622 0a20 2020 2020 2020  tr": "v".       
+000006d0: 7d0a 2020 2020 2020 7d0a 2020 2020 207d  }.      }.     }
+000006e0: 2c0a 2020 2020 2022 3222 3a20 7b20 2274  ,.     "2": { "t
+000006f0: 7970 655f 6d6f 6469 6669 6572 223a 2022  ype_modifier": "
+00000700: 6f22 2c20 2261 6c72 6561 6479 5f63 6672  o", "already_cfr
+00000710: 6574 6169 6e65 6422 3a20 7472 7565 207d  etained": true }
+00000720: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
+00000730: 2241 584f 6273 6572 7665 7247 6574 5275  "AXObserverGetRu
+00000740: 6e4c 6f6f 7053 6f75 7263 6522 3a20 7b0a  nLoopSource": {.
+00000750: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+00000760: 2020 2022 3022 3a20 7b7d 0a20 2020 207d     "0": {}.    }
+00000770: 2c0a 2020 2020 2272 6574 7661 6c22 3a20  ,.    "retval": 
+00000780: 7b7d 0a20 2020 7d2c 0a20 2020 2241 584f  {}.   },.   "AXO
+00000790: 6273 6572 7665 7252 656d 6f76 654e 6f74  bserverRemoveNot
+000007a0: 6966 6963 6174 696f 6e22 3a20 7b0a 2020  ification": {.  
+000007b0: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
+000007c0: 2022 3022 3a20 7b7d 2c0a 2020 2020 2022   "0": {},.     "
+000007d0: 3122 3a20 7b7d 2c0a 2020 2020 2022 3222  1": {},.     "2"
+000007e0: 3a20 7b7d 0a20 2020 207d 0a20 2020 7d2c  : {}.    }.   },
+000007f0: 0a20 2020 2241 5855 4945 6c65 6d65 6e74  .   "AXUIElement
+00000800: 436f 7079 4163 7469 6f6e 4465 7363 7269  CopyActionDescri
+00000810: 7074 696f 6e22 3a20 7b0a 2020 2020 2261  ption": {.    "a
+00000820: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
+00000830: 3a20 7b7d 2c0a 2020 2020 2022 3122 3a20  : {},.     "1": 
+00000840: 7b7d 2c0a 2020 2020 2022 3222 3a20 7b20  {},.     "2": { 
+00000850: 2274 7970 655f 6d6f 6469 6669 6572 223a  "type_modifier":
+00000860: 2022 6f22 2c20 2261 6c72 6561 6479 5f63   "o", "already_c
+00000870: 6672 6574 6169 6e65 6422 3a20 7472 7565  fretained": true
+00000880: 207d 0a20 2020 207d 0a20 2020 7d2c 0a20   }.    }.   },. 
+00000890: 2020 2241 5855 4945 6c65 6d65 6e74 436f    "AXUIElementCo
+000008a0: 7079 4163 7469 6f6e 4e61 6d65 7322 3a20  pyActionNames": 
+000008b0: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
+000008c0: 2020 2020 2022 3022 3a20 7b7d 2c0a 2020       "0": {},.  
+000008d0: 2020 2022 3122 3a20 7b20 2274 7970 655f     "1": { "type_
+000008e0: 6d6f 6469 6669 6572 223a 2022 6f22 2c20  modifier": "o", 
+000008f0: 2261 6c72 6561 6479 5f63 6672 6574 6169  "already_cfretai
+00000900: 6e65 6422 3a20 7472 7565 207d 0a20 2020  ned": true }.   
+00000910: 207d 0a20 2020 7d2c 0a20 2020 2241 5855   }.   },.   "AXU
+00000920: 4945 6c65 6d65 6e74 436f 7079 4174 7472  IElementCopyAttr
+00000930: 6962 7574 654e 616d 6573 223a 207b 0a20  ibuteNames": {. 
+00000940: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
+00000950: 2020 2230 223a 207b 7d2c 0a20 2020 2020    "0": {},.     
+00000960: 2231 223a 207b 2022 7479 7065 5f6d 6f64  "1": { "type_mod
+00000970: 6966 6965 7222 3a20 226f 222c 2022 616c  ifier": "o", "al
+00000980: 7265 6164 795f 6366 7265 7461 696e 6564  ready_cfretained
+00000990: 223a 2074 7275 6520 7d0a 2020 2020 7d0a  ": true }.    }.
+000009a0: 2020 207d 2c0a 2020 2022 4158 5549 456c     },.   "AXUIEl
+000009b0: 656d 656e 7443 6f70 7941 7474 7269 6275  ementCopyAttribu
+000009c0: 7465 5661 6c75 6522 3a20 7b0a 2020 2020  teValue": {.    
+000009d0: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
+000009e0: 3022 3a20 7b7d 2c0a 2020 2020 2022 3122  0": {},.     "1"
+000009f0: 3a20 7b7d 2c0a 2020 2020 2022 3222 3a20  : {},.     "2": 
+00000a00: 7b20 2274 7970 655f 6d6f 6469 6669 6572  { "type_modifier
+00000a10: 223a 2022 6f22 2c20 2261 6c72 6561 6479  ": "o", "already
+00000a20: 5f63 6672 6574 6169 6e65 6422 3a20 7472  _cfretained": tr
+00000a30: 7565 207d 0a20 2020 207d 0a20 2020 7d2c  ue }.    }.   },
+00000a40: 0a20 2020 2241 5855 4945 6c65 6d65 6e74  .   "AXUIElement
+00000a50: 436f 7079 4174 7472 6962 7574 6556 616c  CopyAttributeVal
+00000a60: 7565 7322 3a20 7b0a 2020 2020 2261 7267  ues": {.    "arg
+00000a70: 7322 3a20 7b0a 2020 2020 2022 3022 3a20  s": {.     "0": 
+00000a80: 7b7d 2c0a 2020 2020 2022 3122 3a20 7b7d  {},.     "1": {}
+00000a90: 2c0a 2020 2020 2022 3422 3a20 7b20 2274  ,.     "4": { "t
+00000aa0: 7970 655f 6d6f 6469 6669 6572 223a 2022  ype_modifier": "
+00000ab0: 6f22 2c20 2261 6c72 6561 6479 5f63 6672  o", "already_cfr
+00000ac0: 6574 6169 6e65 6422 3a20 7472 7565 207d  etained": true }
+00000ad0: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
+00000ae0: 2241 5855 4945 6c65 6d65 6e74 436f 7079  "AXUIElementCopy
+00000af0: 456c 656d 656e 7441 7450 6f73 6974 696f  ElementAtPositio
+00000b00: 6e22 3a20 7b0a 2020 2020 2261 7267 7322  n": {.    "args"
+00000b10: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
+00000b20: 2c0a 2020 2020 2022 3322 3a20 7b20 2274  ,.     "3": { "t
+00000b30: 7970 655f 6d6f 6469 6669 6572 223a 2022  ype_modifier": "
+00000b40: 6f22 2c20 2261 6c72 6561 6479 5f63 6672  o", "already_cfr
+00000b50: 6574 6169 6e65 6422 3a20 7472 7565 207d  etained": true }
+00000b60: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
+00000b70: 2241 5855 4945 6c65 6d65 6e74 436f 7079  "AXUIElementCopy
+00000b80: 4d75 6c74 6970 6c65 4174 7472 6962 7574  MultipleAttribut
+00000b90: 6556 616c 7565 7322 3a20 7b0a 2020 2020  eValues": {.    
+00000ba0: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
+00000bb0: 3022 3a20 7b7d 2c0a 2020 2020 2022 3122  0": {},.     "1"
+00000bc0: 3a20 7b7d 2c0a 2020 2020 2022 3322 3a20  : {},.     "3": 
+00000bd0: 7b20 2274 7970 655f 6d6f 6469 6669 6572  { "type_modifier
+00000be0: 223a 2022 6f22 2c20 2261 6c72 6561 6479  ": "o", "already
+00000bf0: 5f63 6672 6574 6169 6e65 6422 3a20 7472  _cfretained": tr
+00000c00: 7565 207d 0a20 2020 207d 0a20 2020 7d2c  ue }.    }.   },
+00000c10: 0a20 2020 2241 5855 4945 6c65 6d65 6e74  .   "AXUIElement
+00000c20: 436f 7079 5061 7261 6d65 7465 7269 7a65  CopyParameterize
+00000c30: 6441 7474 7269 6275 7465 4e61 6d65 7322  dAttributeNames"
+00000c40: 3a20 7b0a 2020 2020 2261 7267 7322 3a20  : {.    "args": 
+00000c50: 7b0a 2020 2020 2022 3022 3a20 7b7d 2c0a  {.     "0": {},.
+00000c60: 2020 2020 2022 3122 3a20 7b20 2274 7970       "1": { "typ
+00000c70: 655f 6d6f 6469 6669 6572 223a 2022 6f22  e_modifier": "o"
+00000c80: 2c20 2261 6c72 6561 6479 5f63 6672 6574  , "already_cfret
+00000c90: 6169 6e65 6422 3a20 7472 7565 207d 0a20  ained": true }. 
+00000ca0: 2020 207d 0a20 2020 7d2c 0a20 2020 2241     }.   },.   "A
+00000cb0: 5855 4945 6c65 6d65 6e74 436f 7079 5061  XUIElementCopyPa
+00000cc0: 7261 6d65 7465 7269 7a65 6441 7474 7269  rameterizedAttri
+00000cd0: 6275 7465 5661 6c75 6522 3a20 7b0a 2020  buteValue": {.  
+00000ce0: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
+00000cf0: 2022 3022 3a20 7b7d 2c0a 2020 2020 2022   "0": {},.     "
+00000d00: 3122 3a20 7b7d 2c0a 2020 2020 2022 3322  1": {},.     "3"
+00000d10: 3a20 7b20 2274 7970 655f 6d6f 6469 6669  : { "type_modifi
+00000d20: 6572 223a 2022 6f22 2c20 2261 6c72 6561  er": "o", "alrea
+00000d30: 6479 5f63 6672 6574 6169 6e65 6422 3a20  dy_cfretained": 
+00000d40: 7472 7565 207d 0a20 2020 207d 0a20 2020  true }.    }.   
+00000d50: 7d2c 0a20 2020 2241 5855 4945 6c65 6d65  },.   "AXUIEleme
+00000d60: 6e74 4372 6561 7465 4170 706c 6963 6174  ntCreateApplicat
+00000d70: 696f 6e22 3a20 7b0a 2020 2020 2272 6574  ion": {.    "ret
+00000d80: 7661 6c22 3a20 7b0a 2020 2020 2022 616c  val": {.     "al
+00000d90: 7265 6164 795f 6366 7265 7461 696e 6564  ready_cfretained
+00000da0: 223a 2074 7275 650a 2020 2020 7d0a 2020  ": true.    }.  
+00000db0: 207d 2c0a 2020 2022 4158 5549 456c 656d   },.   "AXUIElem
+00000dc0: 656e 7443 7265 6174 6553 7973 7465 6d57  entCreateSystemW
+00000dd0: 6964 6522 3a20 7b0a 2020 2020 2272 6574  ide": {.    "ret
+00000de0: 7661 6c22 3a20 7b0a 2020 2020 2022 616c  val": {.     "al
+00000df0: 7265 6164 795f 6366 7265 7461 696e 6564  ready_cfretained
+00000e00: 223a 2074 7275 650a 2020 2020 7d0a 2020  ": true.    }.  
+00000e10: 207d 2c0a 2020 2022 4158 5549 456c 656d   },.   "AXUIElem
+00000e20: 656e 7447 6574 4174 7472 6962 7574 6556  entGetAttributeV
+00000e30: 616c 7565 436f 756e 7422 3a20 7b0a 2020  alueCount": {.  
+00000e40: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
+00000e50: 2022 3022 3a20 7b7d 2c0a 2020 2020 2022   "0": {},.     "
+00000e60: 3122 3a20 7b7d 2c0a 2020 2020 2022 3222  1": {},.     "2"
+00000e70: 3a20 7b20 2274 7970 655f 6d6f 6469 6669  : { "type_modifi
+00000e80: 6572 223a 2022 6f22 207d 0a20 2020 207d  er": "o" }.    }
+00000e90: 0a20 2020 7d2c 0a20 2020 2241 5855 4945  .   },.   "AXUIE
+00000ea0: 6c65 6d65 6e74 4765 7450 6964 223a 207b  lementGetPid": {
+00000eb0: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
+00000ec0: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
+00000ed0: 2020 2231 223a 207b 2022 7479 7065 5f6d    "1": { "type_m
+00000ee0: 6f64 6966 6965 7222 3a20 226f 2220 7d0a  odifier": "o" }.
+00000ef0: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
+00000f00: 4158 5549 456c 656d 656e 7449 7341 7474  AXUIElementIsAtt
+00000f10: 7269 6275 7465 5365 7474 6162 6c65 223a  ributeSettable":
+00000f20: 207b 0a20 2020 2022 6172 6773 223a 207b   {.    "args": {
+00000f30: 0a20 2020 2020 2230 223a 207b 7d2c 0a20  .     "0": {},. 
+00000f40: 2020 2020 2231 223a 207b 7d2c 0a20 2020      "1": {},.   
+00000f50: 2020 2232 223a 207b 2022 7479 7065 5f6d    "2": { "type_m
+00000f60: 6f64 6966 6965 7222 3a20 226f 2220 7d0a  odifier": "o" }.
+00000f70: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
+00000f80: 4158 5549 456c 656d 656e 7450 6572 666f  AXUIElementPerfo
+00000f90: 726d 4163 7469 6f6e 223a 207b 0a20 2020  rmAction": {.   
+00000fa0: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
+00000fb0: 2230 223a 207b 7d2c 0a20 2020 2020 2231  "0": {},.     "1
+00000fc0: 223a 207b 7d0a 2020 2020 7d0a 2020 207d  ": {}.    }.   }
+00000fd0: 2c0a 2020 2022 4158 5549 456c 656d 656e  ,.   "AXUIElemen
+00000fe0: 7450 6f73 744b 6579 626f 6172 6445 7665  tPostKeyboardEve
+00000ff0: 6e74 223a 207b 0a20 2020 2022 6172 6773  nt": {.    "args
+00001000: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
+00001010: 7d0a 2020 2020 7d0a 2020 207d 2c0a 2020  }.    }.   },.  
+00001020: 2022 4158 5549 456c 656d 656e 7453 6574   "AXUIElementSet
+00001030: 4174 7472 6962 7574 6556 616c 7565 223a  AttributeValue":
+00001040: 207b 0a20 2020 2022 6172 6773 223a 207b   {.    "args": {
+00001050: 0a20 2020 2020 2230 223a 207b 7d2c 0a20  .     "0": {},. 
+00001060: 2020 2020 2231 223a 207b 7d0a 2020 2020      "1": {}.    
+00001070: 7d0a 2020 207d 2c0a 2020 2022 4158 5549  }.   },.   "AXUI
+00001080: 456c 656d 656e 7453 6574 4d65 7373 6167  ElementSetMessag
+00001090: 696e 6754 696d 656f 7574 223a 207b 0a20  ingTimeout": {. 
+000010a0: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
+000010b0: 2020 2230 223a 207b 7d0a 2020 2020 7d0a    "0": {}.    }.
+000010c0: 2020 207d 2c0a 2020 2022 4158 5661 6c75     },.   "AXValu
+000010d0: 6543 7265 6174 6522 3a20 7b0a 2020 2020  eCreate": {.    
+000010e0: 2269 676e 6f72 6522 3a20 7472 7565 2c0a  "ignore": true,.
+000010f0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+00001100: 2020 2022 3122 3a20 7b7d 0a20 2020 207d     "1": {}.    }
+00001110: 2c0a 2020 2020 2272 6574 7661 6c22 3a20  ,.    "retval": 
+00001120: 7b0a 2020 2020 2022 616c 7265 6164 795f  {.     "already_
+00001130: 6366 7265 7461 696e 6564 223a 2074 7275  cfretained": tru
+00001140: 650a 2020 2020 7d0a 2020 207d 2c0a 2020  e.    }.   },.  
+00001150: 2022 4158 5661 6c75 6547 6574 5479 7065   "AXValueGetType
+00001160: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
+00001170: 207b 0a20 2020 2020 2230 223a 207b 7d0a   {.     "0": {}.
+00001180: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
+00001190: 4158 5661 6c75 6547 6574 5479 7065 4944  AXValueGetTypeID
+000011a0: 223a 207b 0a20 2020 2022 7661 7269 6164  ": {.    "variad
+000011b0: 6963 223a 2066 616c 7365 0a20 2020 7d2c  ic": false.   },
+000011c0: 0a20 2020 2241 5856 616c 7565 4765 7456  .   "AXValueGetV
+000011d0: 616c 7565 223a 207b 0a20 2020 2022 6967  alue": {.    "ig
+000011e0: 6e6f 7265 223a 2074 7275 652c 0a20 2020  nore": true,.   
+000011f0: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
+00001200: 2230 223a 207b 7d2c 0a20 2020 2020 2232  "0": {},.     "2
+00001210: 223a 207b 7d0a 2020 2020 7d0a 2020 207d  ": {}.    }.   }
+00001220: 2c0a 2020 2022 4164 6449 636f 6e54 6f53  ,.   "AddIconToS
+00001230: 7569 7465 223a 207b 0a20 2020 2022 6967  uite": {.    "ig
+00001240: 6e6f 7265 223a 2074 7275 652c 0a20 2020  nore": true,.   
+00001250: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
+00001260: 2230 223a 207b 7d2c 0a20 2020 2020 2231  "0": {},.     "1
+00001270: 223a 207b 7d0a 2020 2020 7d0a 2020 207d  ": {}.    }.   }
+00001280: 2c0a 2020 2022 436f 7079 5072 6f63 6573  ,.   "CopyProces
+00001290: 734e 616d 6522 3a20 7b0a 2020 2020 2261  sName": {.    "a
+000012a0: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
+000012b0: 3a20 7b20 2274 7970 655f 6d6f 6469 6669  : { "type_modifi
+000012c0: 6572 223a 2022 6e22 207d 2c0a 2020 2020  er": "n" },.    
+000012d0: 2022 3122 3a20 7b20 2274 7970 655f 6d6f   "1": { "type_mo
+000012e0: 6469 6669 6572 223a 2022 6f22 2c20 2261  difier": "o", "a
+000012f0: 6c72 6561 6479 5f63 6672 6574 6169 6e65  lready_cfretaine
+00001300: 6422 3a20 7472 7565 207d 0a20 2020 207d  d": true }.    }
+00001310: 0a20 2020 7d2c 0a20 2020 2244 6973 706f  .   },.   "Dispo
+00001320: 7365 4349 636f 6e22 3a20 7b0a 2020 2020  seCIcon": {.    
+00001330: 2269 676e 6f72 6522 3a20 7472 7565 2c0a  "ignore": true,.
+00001340: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+00001350: 2020 2022 3022 3a20 7b7d 0a20 2020 207d     "0": {}.    }
+00001360: 0a20 2020 7d2c 0a20 2020 2244 6973 706f  .   },.   "Dispo
+00001370: 7365 4963 6f6e 4163 7469 6f6e 5550 5022  seIconActionUPP"
+00001380: 3a20 7b0a 2020 2020 2269 676e 6f72 6522  : {.    "ignore"
+00001390: 3a20 7472 7565 2c0a 2020 2020 2261 7267  : true,.    "arg
+000013a0: 7322 3a20 7b0a 2020 2020 2022 3022 3a20  s": {.     "0": 
+000013b0: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
+000013c0: 2020 2244 6973 706f 7365 4963 6f6e 4765    "DisposeIconGe
+000013d0: 7474 6572 5550 5022 3a20 7b0a 2020 2020  tterUPP": {.    
+000013e0: 2269 676e 6f72 6522 3a20 7472 7565 2c0a  "ignore": true,.
+000013f0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+00001400: 2020 2022 3022 3a20 7b7d 0a20 2020 207d     "0": {}.    }
+00001410: 0a20 2020 7d2c 0a20 2020 2244 6973 706f  .   },.   "Dispo
+00001420: 7365 4963 6f6e 5375 6974 6522 3a20 7b0a  seIconSuite": {.
+00001430: 2020 2020 2269 676e 6f72 6522 3a20 7472      "ignore": tr
+00001440: 7565 2c0a 2020 2020 2261 7267 7322 3a20  ue,.    "args": 
+00001450: 7b0a 2020 2020 2022 3022 3a20 7b7d 0a20  {.     "0": {}. 
+00001460: 2020 207d 0a20 2020 7d2c 0a20 2020 2246     }.   },.   "F
+00001470: 6f72 4561 6368 4963 6f6e 446f 223a 207b  orEachIconDo": {
+00001480: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
+00001490: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
+000014a0: 2020 2232 223a 207b 7d2c 0a20 2020 2020    "2": {},.     
+000014b0: 2233 223a 207b 7d0a 2020 2020 7d0a 2020  "3": {}.    }.  
+000014c0: 207d 2c0a 2020 2022 4765 7443 4963 6f6e   },.   "GetCIcon
+000014d0: 223a 207b 0a20 2020 2022 7265 7476 616c  ": {.    "retval
+000014e0: 223a 207b 7d0a 2020 207d 2c0a 2020 2022  ": {}.   },.   "
+000014f0: 4765 7443 7572 7265 6e74 5072 6f63 6573  GetCurrentProces
+00001500: 7322 3a20 7b0a 2020 2020 2261 7267 7322  s": {.    "args"
+00001510: 3a20 7b0a 2020 2020 2022 3022 3a20 7b20  : {.     "0": { 
+00001520: 2274 7970 655f 6d6f 6469 6669 6572 223a  "type_modifier":
+00001530: 2022 6f22 207d 0a20 2020 207d 0a20 2020   "o" }.    }.   
+00001540: 7d2c 0a20 2020 2247 6574 4672 6f6e 7450  },.   "GetFrontP
+00001550: 726f 6365 7373 223a 207b 0a20 2020 2022  rocess": {.    "
+00001560: 6172 6773 223a 207b 0a20 2020 2020 2230  args": {.     "0
+00001570: 223a 207b 2022 7479 7065 5f6d 6f64 6966  ": { "type_modif
+00001580: 6965 7222 3a20 226f 2220 7d0a 2020 2020  ier": "o" }.    
+00001590: 7d0a 2020 207d 2c0a 2020 2022 4765 7449  }.   },.   "GetI
+000015a0: 636f 6e22 3a20 7b0a 2020 2020 2269 676e  con": {.    "ign
+000015b0: 6f72 6522 3a20 7472 7565 2c0a 2020 2020  ore": true,.    
+000015c0: 2272 6574 7661 6c22 3a20 7b7d 0a20 2020  "retval": {}.   
+000015d0: 7d2c 0a20 2020 2247 6574 4963 6f6e 4361  },.   "GetIconCa
+000015e0: 6368 6544 6174 6122 3a20 7b0a 2020 2020  cheData": {.    
+000015f0: 2269 676e 6f72 6522 3a20 7472 7565 2c0a  "ignore": true,.
+00001600: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+00001610: 2020 2022 3022 3a20 7b7d 2c0a 2020 2020     "0": {},.    
+00001620: 2022 3122 3a20 7b7d 0a20 2020 207d 0a20   "1": {}.    }. 
+00001630: 2020 7d2c 0a20 2020 2247 6574 4963 6f6e    },.   "GetIcon
+00001640: 4361 6368 6550 726f 6322 3a20 7b0a 2020  CacheProc": {.  
+00001650: 2020 2269 676e 6f72 6522 3a20 7472 7565    "ignore": true
+00001660: 2c0a 2020 2020 2261 7267 7322 3a20 7b0a  ,.    "args": {.
+00001670: 2020 2020 2022 3022 3a20 7b7d 2c0a 2020       "0": {},.  
+00001680: 2020 2022 3122 3a20 7b7d 0a20 2020 207d     "1": {}.    }
+00001690: 0a20 2020 7d2c 0a20 2020 2247 6574 4963  .   },.   "GetIc
+000016a0: 6f6e 4661 6d69 6c79 4461 7461 223a 207b  onFamilyData": {
+000016b0: 0a20 2020 2022 6967 6e6f 7265 223a 2074  .    "ignore": t
+000016c0: 7275 652c 0a20 2020 2022 6172 6773 223a  rue,.    "args":
+000016d0: 207b 0a20 2020 2020 2230 223a 207b 7d2c   {.     "0": {},
+000016e0: 0a20 2020 2020 2232 223a 207b 7d0a 2020  .     "2": {}.  
+000016f0: 2020 7d0a 2020 207d 2c0a 2020 2022 4765    }.   },.   "Ge
+00001700: 7449 636f 6e46 726f 6d53 7569 7465 223a  tIconFromSuite":
+00001710: 207b 0a20 2020 2022 6967 6e6f 7265 223a   {.    "ignore":
+00001720: 2074 7275 652c 0a20 2020 2022 6172 6773   true,.    "args
+00001730: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
+00001740: 7d2c 0a20 2020 2020 2231 223a 207b 7d0a  },.     "1": {}.
+00001750: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
+00001760: 4765 7449 636f 6e52 6566 5661 7269 616e  GetIconRefVarian
+00001770: 7422 3a20 7b0a 2020 2020 2269 676e 6f72  t": {.    "ignor
+00001780: 6522 3a20 7472 7565 2c0a 2020 2020 2261  e": true,.    "a
+00001790: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
+000017a0: 3a20 7b7d 2c0a 2020 2020 2022 3222 3a20  : {},.     "2": 
+000017b0: 7b7d 0a20 2020 207d 2c0a 2020 2020 2272  {}.    },.    "r
+000017c0: 6574 7661 6c22 3a20 7b7d 0a20 2020 7d2c  etval": {}.   },
+000017d0: 0a20 2020 2247 6574 4963 6f6e 5369 7a65  .   "GetIconSize
+000017e0: 7346 726f 6d49 636f 6e52 6566 223a 207b  sFromIconRef": {
+000017f0: 0a20 2020 2022 6967 6e6f 7265 223a 2074  .    "ignore": t
+00001800: 7275 652c 0a20 2020 2022 6172 6773 223a  rue,.    "args":
+00001810: 207b 0a20 2020 2020 2231 223a 207b 7d2c   {.     "1": {},
+00001820: 0a20 2020 2020 2233 223a 207b 7d0a 2020  .     "3": {}.  
+00001830: 2020 7d0a 2020 207d 2c0a 2020 2022 4765    }.   },.   "Ge
+00001840: 7449 636f 6e53 7569 7465 223a 207b 0a20  tIconSuite": {. 
+00001850: 2020 2022 6967 6e6f 7265 223a 2074 7275     "ignore": tru
+00001860: 652c 0a20 2020 2022 6172 6773 223a 207b  e,.    "args": {
+00001870: 0a20 2020 2020 2230 223a 207b 7d0a 2020  .     "0": {}.  
+00001880: 2020 7d0a 2020 207d 2c0a 2020 2022 4765    }.   },.   "Ge
+00001890: 744c 6162 656c 223a 207b 0a20 2020 2022  tLabel": {.    "
+000018a0: 6172 6773 223a 207b 0a20 2020 2020 2231  args": {.     "1
+000018b0: 223a 207b 7d0a 2020 2020 7d0a 2020 207d  ": {}.    }.   }
+000018c0: 2c0a 2020 2022 4765 744e 6578 7450 726f  ,.   "GetNextPro
+000018d0: 6365 7373 223a 207b 0a20 2020 2022 6172  cess": {.    "ar
+000018e0: 6773 223a 207b 0a20 2020 2020 2230 223a  gs": {.     "0":
+000018f0: 207b 2022 7479 7065 5f6d 6f64 6966 6965   { "type_modifie
+00001900: 7222 3a20 226f 2220 7d0a 2020 2020 7d0a  r": "o" }.    }.
+00001910: 2020 207d 2c0a 2020 2022 4765 7450 726f     },.   "GetPro
+00001920: 6365 7373 4275 6e64 6c65 4c6f 6361 7469  cessBundleLocati
+00001930: 6f6e 223a 207b 0a20 2020 2022 6172 6773  on": {.    "args
+00001940: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
+00001950: 2022 7479 7065 5f6d 6f64 6966 6965 7222   "type_modifier"
+00001960: 3a20 226e 2220 7d2c 0a20 2020 2020 2231  : "n" },.     "1
+00001970: 223a 207b 2022 7479 7065 5f6d 6f64 6966  ": { "type_modif
+00001980: 6965 7222 3a20 226f 2220 7d0a 2020 2020  ier": "o" }.    
+00001990: 7d0a 2020 207d 2c0a 2020 2022 4765 7450  }.   },.   "GetP
+000019a0: 726f 6365 7373 466f 7250 4944 223a 207b  rocessForPID": {
+000019b0: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
+000019c0: 2020 2020 2231 223a 207b 2022 7479 7065      "1": { "type
+000019d0: 5f6d 6f64 6966 6965 7222 3a20 226f 2220  _modifier": "o" 
+000019e0: 7d0a 2020 2020 7d0a 2020 207d 2c0a 2020  }.    }.   },.  
+000019f0: 2022 4765 7450 726f 6365 7373 496e 666f   "GetProcessInfo
+00001a00: 726d 6174 696f 6e22 3a20 7b0a 2020 2020  rmation": {.    
+00001a10: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
+00001a20: 3022 3a20 7b20 2274 7970 655f 6d6f 6469  0": { "type_modi
+00001a30: 6669 6572 223a 2022 6e22 207d 2c0a 2020  fier": "n" },.  
+00001a40: 2020 2022 3122 3a20 7b20 2274 7970 655f     "1": { "type_
+00001a50: 6d6f 6469 6669 6572 223a 2022 6f22 207d  modifier": "o" }
+00001a60: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
+00001a70: 2247 6574 5072 6f63 6573 7350 4944 223a  "GetProcessPID":
+00001a80: 207b 0a20 2020 2022 6172 6773 223a 207b   {.    "args": {
+00001a90: 0a20 2020 2020 2230 223a 207b 2022 7479  .     "0": { "ty
+00001aa0: 7065 5f6d 6f64 6966 6965 7222 3a20 226e  pe_modifier": "n
+00001ab0: 227d 2c0a 2020 2020 2022 3122 3a20 7b20  "},.     "1": { 
+00001ac0: 2274 7970 655f 6d6f 6469 6669 6572 223a  "type_modifier":
+00001ad0: 2022 6f22 207d 0a20 2020 207d 0a20 2020   "o" }.    }.   
+00001ae0: 7d2c 0a20 2020 2247 6574 5375 6974 654c  },.   "GetSuiteL
+00001af0: 6162 656c 223a 207b 0a20 2020 2022 6172  abel": {.    "ar
+00001b00: 6773 223a 207b 0a20 2020 2020 2230 223a  gs": {.     "0":
+00001b10: 207b 7d0a 2020 2020 7d0a 2020 207d 2c0a   {}.    }.   },.
+00001b20: 2020 2022 4849 5368 6170 6543 6f6e 7461     "HIShapeConta
+00001b30: 696e 7350 6f69 6e74 223a 207b 0a20 2020  insPoint": {.   
+00001b40: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
+00001b50: 2231 223a 207b 2022 7479 7065 5f6d 6f64  "1": { "type_mod
+00001b60: 6966 6965 7222 3a20 226e 2220 7d0a 2020  ifier": "n" }.  
+00001b70: 2020 7d0a 2020 207d 2c0a 2020 2022 4849    }.   },.   "HI
+00001b80: 5368 6170 6543 7265 6174 654d 7574 6162  ShapeCreateMutab
+00001b90: 6c65 5769 7468 5265 6374 223a 207b 0a20  leWithRect": {. 
+00001ba0: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
+00001bb0: 2020 2230 223a 207b 2022 7479 7065 5f6d    "0": { "type_m
+00001bc0: 6f64 6966 6965 7222 3a20 226e 2220 7d0a  odifier": "n" }.
+00001bd0: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
+00001be0: 4849 5368 6170 6543 7265 6174 6557 6974  HIShapeCreateWit
+00001bf0: 6851 4452 676e 223a 207b 2022 6967 6e6f  hQDRgn": { "igno
+00001c00: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
+00001c10: 2248 4953 6861 7065 4372 6561 7465 5769  "HIShapeCreateWi
+00001c20: 7468 5265 6374 223a 207b 0a20 2020 2022  thRect": {.    "
+00001c30: 6172 6773 223a 207b 0a20 2020 2020 2230  args": {.     "0
+00001c40: 223a 207b 2022 7479 7065 5f6d 6f64 6966  ": { "type_modif
+00001c50: 6965 7222 3a20 226e 2220 7d0a 2020 2020  ier": "n" }.    
+00001c60: 7d0a 2020 207d 2c0a 2020 2022 4849 5368  }.   },.   "HISh
+00001c70: 6170 6553 6574 5144 436c 6970 223a 207b  apeSetQDClip": {
+00001c80: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
+00001c90: 7d2c 0a20 2020 2248 4953 6861 7065 556e  },.   "HIShapeUn
+00001ca0: 696f 6e57 6974 6852 6563 7422 3a20 7b0a  ionWithRect": {.
+00001cb0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+00001cc0: 2020 2022 3122 3a20 7b20 2274 7970 655f     "1": { "type_
+00001cd0: 6d6f 6469 6669 6572 223a 2022 6e22 7d0a  modifier": "n"}.
+00001ce0: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
+00001cf0: 4849 5368 6170 6545 6e75 6d65 7261 7465  HIShapeEnumerate
+00001d00: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
+00001d10: 207b 0a20 2020 2020 2232 223a 207b 0a20   {.     "2": {. 
+00001d20: 2020 2020 2022 6361 6c6c 6162 6c65 5f72       "callable_r
+00001d30: 6574 6169 6e65 6422 3a20 6661 6c73 652c  etained": false,
+00001d40: 0a20 2020 2020 2022 6675 6e63 7469 6f6e  .      "function
+00001d50: 223a 207b 0a20 2020 2020 2020 2261 7267  ": {.       "arg
+00001d60: 7322 3a20 5b0a 2020 2020 2020 2020 7b0a  s": [.        {.
+00001d70: 2020 2020 2020 2020 2022 7479 7065 7374           "typest
+00001d80: 7222 3a20 2269 220a 2020 2020 2020 2020  r": "i".        
+00001d90: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+00001da0: 2020 2020 2020 2274 7970 6573 7472 223a        "typestr":
+00001db0: 2022 5e7b 5f5f 4849 5368 6170 653d 7d22   "^{__HIShape=}"
+00001dc0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00001dd0: 2020 2020 7b0a 2020 2020 2020 2020 2022      {.         "
+00001de0: 7479 7065 7374 7222 3a20 5b20 225e 7b43  typestr": [ "^{C
+00001df0: 4752 6563 743d 7b43 4750 6f69 6e74 3d66  GRect={CGPoint=f
+00001e00: 667d 7b43 4753 697a 653d 6666 7d7d 222c  f}{CGSize=ff}}",
+00001e10: 2022 5e7b 4347 5265 6374 3d7b 4347 506f   "^{CGRect={CGPo
+00001e20: 696e 743d 6464 7d7b 4347 5369 7a65 3d64  int=dd}{CGSize=d
+00001e30: 647d 7d22 2020 5d2c 0a09 2022 7479 7065  d}}"  ],.. "type
+00001e40: 5f6d 6f64 6966 6965 7222 3a20 226e 220a  _modifier": "n".
+00001e50: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001e60: 2020 207b 0a20 2020 2020 2020 2020 2274     {.         "t
+00001e70: 7970 6573 7472 223a 2022 5e76 220a 2020  ypestr": "^v".  
+00001e80: 2020 2020 2020 7d0a 2020 2020 2020 205d        }.       ]
+00001e90: 2c0a 2020 2020 2020 2022 7265 7476 616c  ,.       "retval
+00001ea0: 223a 207b 0a20 2020 2020 2020 2022 7479  ": {.        "ty
+00001eb0: 7065 7374 7222 3a20 2269 220a 2020 2020  pestr": "i".    
+00001ec0: 2020 207d 0a20 2020 2020 207d 0a20 2020     }.      }.   
+00001ed0: 2020 7d0a 2020 2020 7d0a 2020 207d 2c0a    }.    }.   },.
+00001ee0: 2020 2022 4849 5368 6170 6547 6574 426f     "HIShapeGetBo
+00001ef0: 756e 6473 223a 207b 0a20 2020 2022 6172  unds": {.    "ar
+00001f00: 6773 223a 207b 0a20 2020 2020 2231 223a  gs": {.     "1":
+00001f10: 207b 2022 7479 7065 5f6d 6f64 6966 6965   { "type_modifie
+00001f20: 7222 3a20 226f 2220 7d0a 2020 2020 7d2c  r": "o" }.    },
+00001f30: 0a20 2020 2022 7265 7476 616c 223a 207b  .    "retval": {
+00001f40: 2022 6465 7265 665f 7265 7375 6c74 5f70   "deref_result_p
+00001f50: 6f69 6e74 6572 223a 2074 7275 6520 7d0a  ointer": true }.
+00001f60: 2020 207d 2c0a 2020 2022 4849 5368 6170     },.   "HIShap
+00001f70: 6547 6574 4173 5144 5267 6e22 3a20 7b20  eGetAsQDRgn": { 
+00001f80: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+00001f90: 2c0a 2020 2022 4849 5368 6170 6549 6e74  ,.   "HIShapeInt
+00001fa0: 6572 7365 6374 7352 6563 7422 3a20 7b0a  ersectsRect": {.
+00001fb0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+00001fc0: 2020 2022 3122 3a20 7b20 2274 7970 655f     "1": { "type_
+00001fd0: 6d6f 6469 6669 6572 223a 2022 6e22 207d  modifier": "n" }
+00001fe0: 0a20 2020 207d 2c0a 2020 2020 2272 6574  .    },.    "ret
+00001ff0: 7661 6c22 3a20 7b0a 2020 2020 2022 635f  val": {.     "c_
+00002000: 6172 7261 795f 6f66 5f66 6978 6564 5f6c  array_of_fixed_l
+00002010: 656e 6774 6822 3a20 310a 2020 2020 7d0a  ength": 1.    }.
+00002020: 2020 207d 2c0a 2020 2022 4943 4164 644d     },.   "ICAddM
+00002030: 6170 456e 7472 7922 3a20 7b20 2269 676e  apEntry": { "ign
+00002040: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
+00002050: 2022 4943 4164 6450 726f 6669 6c65 223a   "ICAddProfile":
+00002060: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
+00002070: 6520 7d2c 0a20 2020 2249 4342 6567 696e  e },.   "ICBegin
+00002080: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00002090: 7275 6520 7d2c 0a20 2020 2249 4343 6f75  rue },.   "ICCou
+000020a0: 6e74 4d61 7045 6e74 7269 6573 223a 207b  ntMapEntries": {
+000020b0: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
+000020c0: 7d2c 0a20 2020 2249 4343 6f75 6e74 5072  },.   "ICCountPr
+000020d0: 6566 223a 207b 2022 6967 6e6f 7265 223a  ef": { "ignore":
+000020e0: 2074 7275 6520 7d2c 0a20 2020 2249 4343   true },.   "ICC
+000020f0: 6f75 6e74 5072 6f66 696c 6573 223a 207b  ountProfiles": {
+00002100: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
+00002110: 7d2c 0a20 2020 2249 4343 7265 6174 6547  },.   "ICCreateG
+00002120: 5552 4c45 7665 6e74 223a 207b 2022 6967  URLEvent": { "ig
+00002130: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
+00002140: 2020 2249 4344 656c 6574 654d 6170 456e    "ICDeleteMapEn
+00002150: 7472 7922 3a20 7b20 2269 676e 6f72 6522  try": { "ignore"
+00002160: 3a20 7472 7565 207d 2c0a 2020 2022 4943  : true },.   "IC
+00002170: 4465 6c65 7465 5072 6566 223a 207b 2022  DeletePref": { "
+00002180: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
+00002190: 0a20 2020 2249 4344 656c 6574 6550 726f  .   "ICDeletePro
+000021a0: 6669 6c65 223a 207b 2022 6967 6e6f 7265  file": { "ignore
+000021b0: 223a 2074 7275 6520 7d2c 0a20 2020 2249  ": true },.   "I
+000021c0: 4345 6469 7450 7265 6665 7265 6e63 6573  CEditPreferences
+000021d0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+000021e0: 7275 6520 7d2c 0a20 2020 2249 4345 6e64  rue },.   "ICEnd
+000021f0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00002200: 7275 6520 7d2c 0a20 2020 2249 4346 696e  rue },.   "ICFin
+00002210: 6450 7265 6648 616e 646c 6522 3a20 7b20  dPrefHandle": { 
+00002220: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+00002230: 2c0a 2020 2022 4943 4765 7443 6f6e 6669  ,.   "ICGetConfi
+00002240: 674e 616d 6522 3a20 7b20 2269 676e 6f72  gName": { "ignor
+00002250: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+00002260: 4943 4765 7443 7572 7265 6e74 5072 6f66  ICGetCurrentProf
+00002270: 696c 6522 3a20 7b20 2269 676e 6f72 6522  ile": { "ignore"
+00002280: 3a20 7472 7565 207d 2c0a 2020 2022 4943  : true },.   "IC
+00002290: 4765 7444 6566 6175 6c74 5072 6566 223a  GetDefaultPref":
+000022a0: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
+000022b0: 6520 7d2c 0a20 2020 2249 4347 6574 496e  e },.   "ICGetIn
+000022c0: 644d 6170 456e 7472 7922 3a20 7b20 2269  dMapEntry": { "i
+000022d0: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
+000022e0: 2020 2022 4943 4765 7449 6e64 5072 6566     "ICGetIndPref
+000022f0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00002300: 7275 6520 7d2c 0a20 2020 2249 4347 6574  rue },.   "ICGet
+00002310: 496e 6450 726f 6669 6c65 223a 207b 2022  IndProfile": { "
+00002320: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
+00002330: 0a20 2020 2249 4347 6574 4d61 7045 6e74  .   "ICGetMapEnt
+00002340: 7279 223a 207b 2022 6967 6e6f 7265 223a  ry": { "ignore":
+00002350: 2074 7275 6520 7d2c 0a20 2020 2249 4347   true },.   "ICG
+00002360: 6574 5065 726d 223a 207b 2022 6967 6e6f  etPerm": { "igno
+00002370: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
+00002380: 2249 4347 6574 5072 6566 223a 207b 2022  "ICGetPref": { "
+00002390: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
+000023a0: 0a20 2020 2249 4347 6574 5072 6566 4861  .   "ICGetPrefHa
+000023b0: 6e64 6c65 223a 207b 2022 6967 6e6f 7265  ndle": { "ignore
+000023c0: 223a 2074 7275 6520 7d2c 0a20 2020 2249  ": true },.   "I
+000023d0: 4347 6574 5072 6f66 696c 654e 616d 6522  CGetProfileName"
+000023e0: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
+000023f0: 7565 207d 2c0a 2020 2022 4943 4765 7453  ue },.   "ICGetS
+00002400: 6565 6422 3a20 7b20 2269 676e 6f72 6522  eed": { "ignore"
+00002410: 3a20 7472 7565 207d 2c0a 2020 2022 4943  : true },.   "IC
+00002420: 4765 7456 6572 7369 6f6e 223a 207b 2022  GetVersion": { "
+00002430: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
+00002440: 0a20 2020 2249 434c 6175 6e63 6855 524c  .   "ICLaunchURL
+00002450: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00002460: 7275 6520 7d2c 0a20 2020 2249 434d 6170  rue },.   "ICMap
+00002470: 456e 7472 6965 7346 696c 656e 616d 6522  EntriesFilename"
+00002480: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
+00002490: 7565 207d 2c0a 2020 2022 4943 4d61 7045  ue },.   "ICMapE
+000024a0: 6e74 7269 6573 5479 7065 4372 6561 746f  ntriesTypeCreato
+000024b0: 7222 3a20 7b20 2269 676e 6f72 6522 3a20  r": { "ignore": 
+000024c0: 7472 7565 207d 2c0a 2020 2022 4943 4d61  true },.   "ICMa
+000024d0: 7046 696c 656e 616d 6522 3a20 7b20 2269  pFilename": { "i
+000024e0: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
+000024f0: 2020 2022 4943 4d61 7054 7970 6543 7265     "ICMapTypeCre
+00002500: 6174 6f72 223a 207b 2022 6967 6e6f 7265  ator": { "ignore
+00002510: 223a 2074 7275 6520 7d2c 0a20 2020 2249  ": true },.   "I
+00002520: 4350 6172 7365 5552 4c22 3a20 7b20 2269  CParseURL": { "i
+00002530: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
+00002540: 2020 2022 4943 5365 6e64 4755 524c 4576     "ICSendGURLEv
+00002550: 656e 7422 3a20 7b20 2269 676e 6f72 6522  ent": { "ignore"
+00002560: 3a20 7472 7565 207d 2c0a 2020 2022 4943  : true },.   "IC
+00002570: 5365 7443 7572 7265 6e74 5072 6f66 696c  SetCurrentProfil
+00002580: 6522 3a20 7b20 2269 676e 6f72 6522 3a20  e": { "ignore": 
+00002590: 7472 7565 207d 2c0a 2020 2022 4943 5365  true },.   "ICSe
+000025a0: 744d 6170 456e 7472 7922 3a20 7b20 2269  tMapEntry": { "i
+000025b0: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
+000025c0: 2020 2022 4943 5365 7450 7265 6622 3a20     "ICSetPref": 
+000025d0: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
+000025e0: 207d 2c0a 2020 2022 4943 5365 7450 7265   },.   "ICSetPre
+000025f0: 6648 616e 646c 6522 3a20 7b20 2269 676e  fHandle": { "ign
+00002600: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
+00002610: 2022 4943 5365 7450 726f 6669 6c65 4e61   "ICSetProfileNa
+00002620: 6d65 223a 207b 2022 6967 6e6f 7265 223a  me": { "ignore":
+00002630: 2074 7275 6520 7d2c 0a20 2020 2249 4353   true },.   "ICS
+00002640: 7461 7274 223a 207b 2022 6967 6e6f 7265  tart": { "ignore
+00002650: 223a 2074 7275 6520 7d2c 0a20 2020 2249  ": true },.   "I
+00002660: 4353 746f 7022 3a20 7b20 2269 676e 6f72  CStop": { "ignor
+00002670: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+00002680: 4963 6f6e 4661 6d69 6c79 546f 4963 6f6e  IconFamilyToIcon
+00002690: 5375 6974 6522 3a20 7b7d 2c0a 2020 2022  Suite": {},.   "
+000026a0: 4963 6f6e 4944 546f 5267 6e22 3a20 7b0a  IconIDToRgn": {.
+000026b0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+000026c0: 2020 2022 3022 3a20 7b7d 2c0a 2020 2020     "0": {},.    
+000026d0: 2022 3122 3a20 7b7d 0a20 2020 207d 0a20   "1": {}.    }. 
+000026e0: 2020 7d2c 0a20 2020 2249 636f 6e4d 6574    },.   "IconMet
+000026f0: 686f 6454 6f52 676e 223a 207b 0a20 2020  hodToRgn": {.   
+00002700: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
+00002710: 2230 223a 207b 7d2c 0a20 2020 2020 2231  "0": {},.     "1
+00002720: 223a 207b 7d2c 0a20 2020 2020 2233 223a  ": {},.     "3":
+00002730: 207b 7d2c 0a20 2020 2020 2234 223a 207b   {},.     "4": {
+00002740: 7d0a 2020 2020 7d0a 2020 207d 2c0a 2020  }.    }.   },.  
+00002750: 2022 4963 6f6e 5265 6643 6f6e 7461 696e   "IconRefContain
+00002760: 7343 4750 6f69 6e74 223a 207b 0a20 2020  sCGPoint": {.   
+00002770: 2022 6967 6e6f 7265 223a 2074 7275 652c   "ignore": true,
+00002780: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
+00002790: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
+000027a0: 2020 2231 223a 207b 7d2c 0a20 2020 2020    "1": {},.     
+000027b0: 2234 223a 207b 7d0a 2020 2020 7d0a 2020  "4": {}.    }.  
+000027c0: 207d 2c0a 2020 2022 4963 6f6e 5265 6649   },.   "IconRefI
+000027d0: 6e74 6572 7365 6374 7343 4752 6563 7422  ntersectsCGRect"
+000027e0: 3a20 7b0a 2020 2020 2269 676e 6f72 6522  : {.    "ignore"
+000027f0: 3a20 7472 7565 2c0a 2020 2020 2261 7267  : true,.    "arg
+00002800: 7322 3a20 7b0a 2020 2020 2022 3022 3a20  s": {.     "0": 
+00002810: 7b7d 2c0a 2020 2020 2022 3122 3a20 7b7d  {},.     "1": {}
+00002820: 2c0a 2020 2020 2022 3422 3a20 7b7d 0a20  ,.     "4": {}. 
+00002830: 2020 207d 0a20 2020 7d2c 0a20 2020 2249     }.   },.   "I
+00002840: 636f 6e52 6566 546f 4849 5368 6170 6522  conRefToHIShape"
+00002850: 3a20 7b0a 2020 2020 2269 676e 6f72 6522  : {.    "ignore"
+00002860: 3a20 7472 7565 2c0a 2020 2020 2261 7267  : true,.    "arg
+00002870: 7322 3a20 7b0a 2020 2020 2022 3022 3a20  s": {.     "0": 
+00002880: 7b7d 2c0a 2020 2020 2022 3322 3a20 7b7d  {},.     "3": {}
+00002890: 0a20 2020 207d 2c0a 2020 2020 2272 6574  .    },.    "ret
+000028a0: 7661 6c22 3a20 7b7d 0a20 2020 7d2c 0a20  val": {}.   },. 
+000028b0: 2020 2249 636f 6e52 6566 546f 4963 6f6e    "IconRefToIcon
+000028c0: 4661 6d69 6c79 223a 207b 0a20 2020 2022  Family": {.    "
+000028d0: 6967 6e6f 7265 223a 2074 7275 652c 0a20  ignore": true,. 
+000028e0: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
+000028f0: 2020 2230 223a 207b 7d2c 0a20 2020 2020    "0": {},.     
+00002900: 2232 223a 207b 7d0a 2020 2020 7d0a 2020  "2": {}.    }.  
+00002910: 207d 2c0a 2020 2022 4963 6f6e 5265 6654   },.   "IconRefT
+00002920: 6f52 676e 223a 207b 0a20 2020 2022 6967  oRgn": {.    "ig
+00002930: 6e6f 7265 223a 2074 7275 652c 0a20 2020  nore": true,.   
+00002940: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
+00002950: 2230 223a 207b 7d2c 0a20 2020 2020 2231  "0": {},.     "1
+00002960: 223a 207b 7d2c 0a20 2020 2020 2234 223a  ": {},.     "4":
+00002970: 207b 7d0a 2020 2020 7d0a 2020 207d 2c0a   {}.    }.   },.
+00002980: 2020 2022 4963 6f6e 5375 6974 6554 6f49     "IconSuiteToI
+00002990: 636f 6e46 616d 696c 7922 3a20 7b0a 2020  conFamily": {.  
+000029a0: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
+000029b0: 2022 3022 3a20 7b7d 2c0a 2020 2020 2022   "0": {},.     "
+000029c0: 3222 3a20 7b7d 0a20 2020 207d 0a20 2020  2": {}.    }.   
+000029d0: 7d2c 0a20 2020 2249 636f 6e53 7569 7465  },.   "IconSuite
+000029e0: 546f 5267 6e22 3a20 7b0a 2020 2020 2261  ToRgn": {.    "a
+000029f0: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
+00002a00: 3a20 7b7d 2c0a 2020 2020 2022 3122 3a20  : {},.     "1": 
+00002a10: 7b7d 2c0a 2020 2020 2022 3322 3a20 7b7d  {},.     "3": {}
+00002a20: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
+00002a30: 2249 6e76 6f6b 6549 636f 6e41 6374 696f  "InvokeIconActio
+00002a40: 6e55 5050 223a 207b 0a20 2020 2022 6172  nUPP": {.    "ar
+00002a50: 6773 223a 207b 0a20 2020 2020 2231 223a  gs": {.     "1":
+00002a60: 207b 7d2c 0a20 2020 2020 2232 223a 207b   {},.     "2": {
+00002a70: 7d2c 0a20 2020 2020 2233 223a 207b 7d0a  },.     "3": {}.
+00002a80: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
+00002a90: 496e 766f 6b65 4963 6f6e 4765 7474 6572  InvokeIconGetter
+00002aa0: 5550 5022 3a20 7b0a 2020 2020 2261 7267  UPP": {.    "arg
+00002ab0: 7322 3a20 7b0a 2020 2020 2022 3122 3a20  s": {.     "1": 
+00002ac0: 7b7d 2c0a 2020 2020 2022 3222 3a20 7b7d  {},.     "2": {}
+00002ad0: 0a20 2020 207d 2c0a 2020 2020 2272 6574  .    },.    "ret
+00002ae0: 7661 6c22 3a20 7b7d 0a20 2020 7d2c 0a20  val": {}.   },. 
+00002af0: 2020 2249 7349 636f 6e52 6566 4d61 736b    "IsIconRefMask
+00002b00: 456d 7074 7922 3a20 7b0a 2020 2020 2261  Empty": {.    "a
+00002b10: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
+00002b20: 3a20 7b7d 0a20 2020 207d 0a20 2020 7d2c  : {}.    }.   },
+00002b30: 0a20 2020 2249 7350 726f 6365 7373 5669  .   "IsProcessVi
+00002b40: 7369 626c 6522 3a20 7b0a 2020 2020 2261  sible": {.    "a
+00002b50: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
+00002b60: 3a20 7b20 2274 7970 655f 6d6f 6469 6669  : { "type_modifi
+00002b70: 6572 223a 2022 6e22 207d 0a20 2020 207d  er": "n" }.    }
+00002b80: 0a20 2020 7d2c 0a20 2020 224b 696c 6c50  .   },.   "KillP
+00002b90: 726f 6365 7373 223a 207b 0a20 2020 2022  rocess": {.    "
+00002ba0: 6172 6773 223a 207b 0a20 2020 2020 2230  args": {.     "0
+00002bb0: 223a 207b 2022 7479 7065 5f6d 6f64 6966  ": { "type_modif
+00002bc0: 6965 7222 3a20 226e 2220 7d0a 2020 2020  ier": "n" }.    
+00002bd0: 7d0a 2020 207d 2c0a 2020 2022 4c61 756e  }.   },.   "Laun
+00002be0: 6368 4170 706c 6963 6174 696f 6e22 3a20  chApplication": 
+00002bf0: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
+00002c00: 207d 2c0a 2020 2022 4c6f 6164 4963 6f6e   },.   "LoadIcon
+00002c10: 4361 6368 6522 3a20 7b0a 2020 2020 2261  Cache": {.    "a
+00002c20: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
+00002c30: 3a20 7b7d 2c0a 2020 2020 2022 3322 3a20  : {},.     "3": 
+00002c40: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
+00002c50: 2020 224d 616b 6549 636f 6e43 6163 6865    "MakeIconCache
+00002c60: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
+00002c70: 207b 0a20 2020 2020 2230 223a 207b 7d2c   {.     "0": {},
+00002c80: 0a20 2020 2020 2231 223a 207b 7d2c 0a20  .     "1": {},. 
+00002c90: 2020 2020 2232 223a 207b 7d0a 2020 2020      "2": {}.    
+00002ca0: 7d0a 2020 207d 2c0a 2020 2022 4e65 7749  }.   },.   "NewI
+00002cb0: 636f 6e41 6374 696f 6e55 5050 223a 207b  conActionUPP": {
+00002cc0: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
+00002cd0: 2020 2020 2230 223a 207b 0a20 2020 2020      "0": {.     
+00002ce0: 2022 6675 6e63 7469 6f6e 223a 207b 0a20   "function": {. 
+00002cf0: 2020 2020 2020 2261 7267 7322 3a20 5b0a        "args": [.
+00002d00: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00002d10: 2020 2022 7479 7065 7374 7222 3a20 2249     "typestr": "I
+00002d20: 220a 2020 2020 2020 2020 7d2c 0a20 2020  ".        },.   
+00002d30: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00002d40: 2274 7970 6573 7472 223a 2022 5e5e 5e63  "typestr": "^^^c
+00002d50: 220a 2020 2020 2020 2020 7d2c 0a20 2020  ".        },.   
+00002d60: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00002d70: 2274 7970 6573 7472 223a 2022 5e76 220a  "typestr": "^v".
+00002d80: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00002d90: 205d 2c0a 2020 2020 2020 2022 7265 7476   ],.       "retv
+00002da0: 616c 223a 207b 0a20 2020 2020 2020 2022  al": {.        "
+00002db0: 7479 7065 7374 7222 3a20 2273 220a 2020  typestr": "s".  
+00002dc0: 2020 2020 207d 0a20 2020 2020 207d 0a20       }.      }. 
+00002dd0: 2020 2020 7d0a 2020 2020 7d2c 0a20 2020      }.    },.   
+00002de0: 2022 7265 7476 616c 223a 207b 7d0a 2020   "retval": {}.  
+00002df0: 207d 2c0a 2020 2022 4e65 7749 636f 6e47   },.   "NewIconG
+00002e00: 6574 7465 7255 5050 223a 207b 0a20 2020  etterUPP": {.   
+00002e10: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
+00002e20: 2230 223a 207b 0a20 2020 2020 2022 6675  "0": {.      "fu
+00002e30: 6e63 7469 6f6e 223a 207b 0a20 2020 2020  nction": {.     
+00002e40: 2020 2261 7267 7322 3a20 5b0a 2020 2020    "args": [.    
+00002e50: 2020 2020 7b0a 2020 2020 2020 2020 2022      {.         "
+00002e60: 7479 7065 7374 7222 3a20 2249 220a 2020  typestr": "I".  
+00002e70: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00002e80: 207b 0a20 2020 2020 2020 2020 2274 7970   {.         "typ
+00002e90: 6573 7472 223a 2022 5e76 220a 2020 2020  estr": "^v".    
+00002ea0: 2020 2020 7d0a 2020 2020 2020 205d 2c0a      }.       ],.
+00002eb0: 2020 2020 2020 2022 7265 7476 616c 223a         "retval":
+00002ec0: 207b 0a20 2020 2020 2020 2022 7479 7065   {.        "type
+00002ed0: 7374 7222 3a20 225e 5e63 220a 2020 2020  str": "^^c".    
+00002ee0: 2020 207d 0a20 2020 2020 207d 0a20 2020     }.      }.   
+00002ef0: 2020 7d0a 2020 2020 7d2c 0a20 2020 2022    }.    },.    "
+00002f00: 7265 7476 616c 223a 207b 7d0a 2020 207d  retval": {}.   }
+00002f10: 2c0a 2020 2022 4e65 7749 636f 6e53 7569  ,.   "NewIconSui
+00002f20: 7465 223a 207b 0a20 2020 2022 6172 6773  te": {.    "args
+00002f30: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
+00002f40: 7d0a 2020 2020 7d0a 2020 207d 2c0a 2020  }.    }.   },.  
+00002f50: 2022 5061 7374 6562 6f61 7264 436c 6561   "PasteboardClea
+00002f60: 7222 3a20 7b0a 2020 2020 2261 7267 7322  r": {.    "args"
+00002f70: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
+00002f80: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
+00002f90: 2250 6173 7465 626f 6172 6443 6f70 7949  "PasteboardCopyI
+00002fa0: 7465 6d46 6c61 766f 7244 6174 6122 3a20  temFlavorData": 
+00002fb0: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
+00002fc0: 2020 2020 2022 3022 3a20 7b7d 2c0a 2020       "0": {},.  
+00002fd0: 2020 2022 3122 3a20 7b7d 2c0a 2020 2020     "1": {},.    
+00002fe0: 2022 3222 3a20 7b7d 2c0a 2020 2020 2022   "2": {},.     "
+00002ff0: 3322 3a20 7b20 2274 7970 655f 6d6f 6469  3": { "type_modi
+00003000: 6669 6572 223a 2022 6f22 2c20 2261 6c72  fier": "o", "alr
+00003010: 6561 6479 5f63 6672 6574 6169 6e65 6422  eady_cfretained"
+00003020: 3a20 7472 7565 207d 0a20 2020 207d 0a20  : true }.    }. 
+00003030: 2020 7d2c 0a20 2020 2250 6173 7465 626f    },.   "Pastebo
+00003040: 6172 6443 6f70 7949 7465 6d46 6c61 766f  ardCopyItemFlavo
+00003050: 7273 223a 207b 0a20 2020 2022 6172 6773  rs": {.    "args
+00003060: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
+00003070: 7d2c 0a20 2020 2020 2231 223a 207b 7d2c  },.     "1": {},
+00003080: 0a20 2020 2020 2232 223a 207b 2022 7479  .     "2": { "ty
+00003090: 7065 5f6d 6f64 6966 6965 7222 3a20 226f  pe_modifier": "o
+000030a0: 222c 2022 616c 7265 6164 795f 6366 7265  ", "already_cfre
+000030b0: 7461 696e 6564 223a 2074 7275 657d 0a20  tained": true}. 
+000030c0: 2020 207d 0a20 2020 7d2c 0a20 2020 2250     }.   },.   "P
+000030d0: 6173 7465 626f 6172 6443 6f70 794e 616d  asteboardCopyNam
+000030e0: 6522 3a20 7b0a 2020 2020 2261 7267 7322  e": {.    "args"
+000030f0: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
+00003100: 2c0a 2020 2020 2022 3122 3a20 7b20 2274  ,.     "1": { "t
+00003110: 7970 655f 6d6f 6469 6669 6572 223a 2022  ype_modifier": "
+00003120: 6f22 2c20 2261 6c72 6561 6479 5f63 6672  o", "already_cfr
+00003130: 6574 6169 6e65 6422 3a20 7472 7565 207d  etained": true }
+00003140: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
+00003150: 2250 6173 7465 626f 6172 6443 6f70 7950  "PasteboardCopyP
+00003160: 6173 7465 4c6f 6361 7469 6f6e 223a 207b  asteLocation": {
+00003170: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
+00003180: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
+00003190: 2020 2231 223a 207b 2022 7479 7065 5f6d    "1": { "type_m
+000031a0: 6f64 6966 6965 7222 3a20 226f 222c 2022  odifier": "o", "
+000031b0: 616c 7265 6164 795f 6366 7265 7461 696e  already_cfretain
+000031c0: 6564 223a 2074 7275 6520 7d0a 2020 2020  ed": true }.    
+000031d0: 7d0a 2020 207d 2c0a 2020 2022 5061 7374  }.   },.   "Past
+000031e0: 6562 6f61 7264 4372 6561 7465 223a 207b  eboardCreate": {
+000031f0: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
+00003200: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
+00003210: 2020 2231 223a 207b 2022 7479 7065 5f6d    "1": { "type_m
+00003220: 6f64 6966 6965 7222 3a20 226f 222c 2022  odifier": "o", "
+00003230: 616c 7265 6164 795f 6366 7265 7461 696e  already_cfretain
+00003240: 6564 223a 2074 7275 6520 7d0a 2020 2020  ed": true }.    
+00003250: 7d0a 2020 207d 2c0a 2020 2022 5061 7374  }.   },.   "Past
+00003260: 6562 6f61 7264 4765 7449 7465 6d43 6f75  eboardGetItemCou
+00003270: 6e74 223a 207b 0a20 2020 2022 6172 6773  nt": {.    "args
+00003280: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
+00003290: 7d2c 0a20 2020 2020 2231 223a 207b 2022  },.     "1": { "
+000032a0: 7479 7065 5f6d 6f64 6966 6965 7222 3a20  type_modifier": 
+000032b0: 226f 2220 7d0a 2020 2020 7d0a 2020 207d  "o" }.    }.   }
 000032c0: 2c0a 2020 2022 5061 7374 6562 6f61 7264  ,.   "Pasteboard
-000032d0: 5379 6e63 6872 6f6e 697a 6522 3a20 7b0a  Synchronize": {.
-000032e0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-000032f0: 2020 2022 3022 3a20 7b7d 0a20 2020 207d     "0": {}.    }
-00003300: 0a20 2020 7d2c 0a20 2020 2250 6c6f 7443  .   },.   "PlotC
-00003310: 4963 6f6e 223a 207b 0a20 2020 2022 6172  Icon": {.    "ar
-00003320: 6773 223a 207b 0a20 2020 2020 2230 223a  gs": {.     "0":
-00003330: 207b 7d2c 0a20 2020 2020 2231 223a 207b   {},.     "1": {
+000032d0: 4765 7449 7465 6d46 6c61 766f 7246 6c61  GetItemFlavorFla
+000032e0: 6773 223a 207b 0a20 2020 2022 6172 6773  gs": {.    "args
+000032f0: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
+00003300: 7d2c 0a20 2020 2020 2231 223a 207b 7d2c  },.     "1": {},
+00003310: 0a20 2020 2020 2232 223a 207b 7d2c 0a20  .     "2": {},. 
+00003320: 2020 2020 2233 223a 207b 2022 7479 7065      "3": { "type
+00003330: 5f6d 6f64 6966 6965 7222 3a20 226f 2220  _modifier": "o" 
 00003340: 7d0a 2020 2020 7d0a 2020 207d 2c0a 2020  }.    }.   },.  
-00003350: 2022 506c 6f74 4349 636f 6e48 616e 646c   "PlotCIconHandl
-00003360: 6522 3a20 7b0a 2020 2020 2261 7267 7322  e": {.    "args"
-00003370: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
-00003380: 2c0a 2020 2020 2022 3322 3a20 7b7d 0a20  ,.     "3": {}. 
-00003390: 2020 207d 0a20 2020 7d2c 0a20 2020 2250     }.   },.   "P
-000033a0: 6c6f 7449 636f 6e22 3a20 7b0a 2020 2020  lotIcon": {.    
-000033b0: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
-000033c0: 3022 3a20 7b7d 2c0a 2020 2020 2022 3122  0": {},.     "1"
-000033d0: 3a20 7b7d 0a20 2020 207d 0a20 2020 7d2c  : {}.    }.   },
-000033e0: 0a20 2020 2250 6c6f 7449 636f 6e48 616e  .   "PlotIconHan
-000033f0: 646c 6522 3a20 7b0a 2020 2020 2261 7267  dle": {.    "arg
-00003400: 7322 3a20 7b0a 2020 2020 2022 3022 3a20  s": {.     "0": 
-00003410: 7b7d 2c0a 2020 2020 2022 3322 3a20 7b7d  {},.     "3": {}
-00003420: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
-00003430: 2250 6c6f 7449 636f 6e49 4422 3a20 7b0a  "PlotIconID": {.
-00003440: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-00003450: 2020 2022 3022 3a20 7b7d 0a20 2020 207d     "0": {}.    }
-00003460: 0a20 2020 7d2c 0a20 2020 2250 6c6f 7449  .   },.   "PlotI
-00003470: 636f 6e4d 6574 686f 6422 3a20 7b0a 2020  conMethod": {.  
-00003480: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
-00003490: 2022 3022 3a20 7b7d 2c0a 2020 2020 2022   "0": {},.     "
-000034a0: 3322 3a20 7b7d 2c0a 2020 2020 2022 3422  3": {},.     "4"
-000034b0: 3a20 7b7d 0a20 2020 207d 0a20 2020 7d2c  : {}.    }.   },
-000034c0: 0a20 2020 2250 6c6f 7449 636f 6e52 6566  .   "PlotIconRef
-000034d0: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-000034e0: 207b 0a20 2020 2020 2230 223a 207b 7d2c   {.     "0": {},
-000034f0: 0a20 2020 2020 2234 223a 207b 7d0a 2020  .     "4": {}.  
-00003500: 2020 7d0a 2020 207d 2c0a 2020 2022 506c    }.   },.   "Pl
-00003510: 6f74 4963 6f6e 5265 6649 6e43 6f6e 7465  otIconRefInConte
-00003520: 7874 223a 207b 0a20 2020 2022 6172 6773  xt": {.    "args
-00003530: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
-00003540: 7d2c 0a20 2020 2020 2231 223a 207b 7d2c  },.     "1": {},
-00003550: 0a20 2020 2020 2234 223a 207b 7d2c 0a20  .     "4": {},. 
-00003560: 2020 2020 2236 223a 207b 7d0a 2020 2020      "6": {}.    
-00003570: 7d0a 2020 207d 2c0a 2020 2022 506c 6f74  }.   },.   "Plot
-00003580: 4963 6f6e 5375 6974 6522 3a20 7b0a 2020  IconSuite": {.  
-00003590: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
-000035a0: 2022 3022 3a20 7b7d 2c0a 2020 2020 2022   "0": {},.     "
-000035b0: 3322 3a20 7b7d 0a20 2020 207d 0a20 2020  3": {}.    }.   
-000035c0: 7d2c 0a20 2020 2250 6c6f 7453 4943 4e48  },.   "PlotSICNH
-000035d0: 616e 646c 6522 3a20 7b0a 2020 2020 2261  andle": {.    "a
-000035e0: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
-000035f0: 3a20 7b7d 2c0a 2020 2020 2022 3322 3a20  : {},.     "3": 
-00003600: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
-00003610: 2020 2250 726f 6365 7373 496e 666f 726d    "ProcessInform
-00003620: 6174 696f 6e43 6f70 7944 6963 7469 6f6e  ationCopyDiction
-00003630: 6172 7922 3a20 7b0a 2020 2020 2261 7267  ary": {.    "arg
-00003640: 7322 3a20 7b0a 2020 2020 2022 3022 3a20  s": {.     "0": 
-00003650: 7b7d 0a20 2020 207d 2c0a 2020 2020 2272  {}.    },.    "r
-00003660: 6574 7661 6c22 3a20 7b0a 2020 2020 2022  etval": {.     "
-00003670: 616c 7265 6164 795f 6366 7265 7461 696e  already_cfretain
-00003680: 6564 223a 2074 7275 650a 2020 2020 7d0a  ed": true.    }.
-00003690: 2020 207d 2c0a 2020 2022 5074 496e 4963     },.   "PtInIc
-000036a0: 6f6e 4944 223a 207b 0a20 2020 2022 6172  onID": {.    "ar
-000036b0: 6773 223a 207b 0a20 2020 2020 2231 223a  gs": {.     "1":
-000036c0: 207b 7d0a 2020 2020 7d0a 2020 207d 2c0a   {}.    }.   },.
-000036d0: 2020 2022 5074 496e 4963 6f6e 4d65 7468     "PtInIconMeth
-000036e0: 6f64 223a 207b 0a20 2020 2022 6172 6773  od": {.    "args
-000036f0: 223a 207b 0a20 2020 2020 2231 223a 207b  ": {.     "1": {
-00003700: 7d2c 0a20 2020 2020 2233 223a 207b 7d2c  },.     "3": {},
-00003710: 0a20 2020 2020 2234 223a 207b 7d0a 2020  .     "4": {}.  
-00003720: 2020 7d0a 2020 207d 2c0a 2020 2022 5074    }.   },.   "Pt
-00003730: 496e 4963 6f6e 5265 6622 3a20 7b0a 2020  InIconRef": {.  
-00003740: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
-00003750: 2022 3022 3a20 7b7d 2c0a 2020 2020 2022   "0": {},.     "
-00003760: 3122 3a20 7b7d 2c0a 2020 2020 2022 3422  1": {},.     "4"
-00003770: 3a20 7b7d 0a20 2020 207d 0a20 2020 7d2c  : {}.    }.   },
-00003780: 0a20 2020 2250 7449 6e49 636f 6e53 7569  .   "PtInIconSui
-00003790: 7465 223a 207b 0a20 2020 2022 6172 6773  te": {.    "args
-000037a0: 223a 207b 0a20 2020 2020 2231 223a 207b  ": {.     "1": {
-000037b0: 7d2c 0a20 2020 2020 2233 223a 207b 7d0a  },.     "3": {}.
-000037c0: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
-000037d0: 5265 6374 496e 4963 6f6e 4944 223a 207b  RectInIconID": {
-000037e0: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
-000037f0: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
-00003800: 2020 2231 223a 207b 7d0a 2020 2020 7d0a    "1": {}.    }.
-00003810: 2020 207d 2c0a 2020 2022 5265 6374 496e     },.   "RectIn
-00003820: 4963 6f6e 4d65 7468 6f64 223a 207b 0a20  IconMethod": {. 
-00003830: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
-00003840: 2020 2230 223a 207b 7d2c 0a20 2020 2020    "0": {},.     
-00003850: 2231 223a 207b 7d2c 0a20 2020 2020 2233  "1": {},.     "3
-00003860: 223a 207b 7d2c 0a20 2020 2020 2234 223a  ": {},.     "4":
-00003870: 207b 7d0a 2020 2020 7d0a 2020 207d 2c0a   {}.    }.   },.
-00003880: 2020 2022 5265 6374 496e 4963 6f6e 5265     "RectInIconRe
-00003890: 6622 3a20 7b0a 2020 2020 2261 7267 7322  f": {.    "args"
-000038a0: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
-000038b0: 2c0a 2020 2020 2022 3122 3a20 7b7d 2c0a  ,.     "1": {},.
-000038c0: 2020 2020 2022 3422 3a20 7b7d 0a20 2020       "4": {}.   
-000038d0: 207d 0a20 2020 7d2c 0a20 2020 2252 6563   }.   },.   "Rec
-000038e0: 7449 6e49 636f 6e53 7569 7465 223a 207b  tInIconSuite": {
-000038f0: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
-00003900: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
-00003910: 2020 2231 223a 207b 7d2c 0a20 2020 2020    "1": {},.     
-00003920: 2233 223a 207b 7d0a 2020 2020 7d0a 2020  "3": {}.    }.  
-00003930: 207d 2c0a 2020 2022 5361 6d65 5072 6f63   },.   "SameProc
-00003940: 6573 7322 3a20 7b0a 2020 2020 2261 7267  ess": {.    "arg
-00003950: 7322 3a20 7b0a 2020 2020 2022 3022 3a20  s": {.     "0": 
-00003960: 7b7d 2c0a 2020 2020 2022 3122 3a20 7b7d  {},.     "1": {}
-00003970: 2c0a 2020 2020 2022 3222 3a20 7b7d 0a20  ,.     "2": {}. 
-00003980: 2020 207d 0a20 2020 7d2c 0a20 2020 2253     }.   },.   "S
-00003990: 6574 4672 6f6e 7450 726f 6365 7373 223a  etFrontProcess":
-000039a0: 207b 0a20 2020 2022 6172 6773 223a 207b   {.    "args": {
-000039b0: 0a20 2020 2020 2230 223a 207b 7d0a 2020  .     "0": {}.  
-000039c0: 2020 7d0a 2020 207d 2c0a 2020 2022 5365    }.   },.   "Se
-000039d0: 7446 726f 6e74 5072 6f63 6573 7357 6974  tFrontProcessWit
-000039e0: 684f 7074 696f 6e73 223a 207b 0a20 2020  hOptions": {.   
-000039f0: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
-00003a00: 2230 223a 207b 7d0a 2020 2020 7d0a 2020  "0": {}.    }.  
-00003a10: 207d 2c0a 2020 2022 5365 7449 636f 6e43   },.   "SetIconC
-00003a20: 6163 6865 4461 7461 223a 207b 0a20 2020  acheData": {.   
-00003a30: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
-00003a40: 2230 223a 207b 7d2c 0a20 2020 2020 2231  "0": {},.     "1
-00003a50: 223a 207b 7d0a 2020 2020 7d0a 2020 207d  ": {}.    }.   }
-00003a60: 2c0a 2020 2022 5365 7449 636f 6e43 6163  ,.   "SetIconCac
-00003a70: 6865 5072 6f63 223a 207b 0a20 2020 2022  heProc": {.    "
-00003a80: 6172 6773 223a 207b 0a20 2020 2020 2230  args": {.     "0
-00003a90: 223a 207b 7d2c 0a20 2020 2020 2231 223a  ": {},.     "1":
-00003aa0: 207b 7d0a 2020 2020 7d0a 2020 207d 2c0a   {}.    }.   },.
-00003ab0: 2020 2022 5365 7449 636f 6e46 616d 696c     "SetIconFamil
-00003ac0: 7944 6174 6122 3a20 7b0a 2020 2020 2261  yData": {.    "a
-00003ad0: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
-00003ae0: 3a20 7b7d 2c0a 2020 2020 2022 3222 3a20  : {},.     "2": 
-00003af0: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
-00003b00: 2020 2253 6574 5375 6974 654c 6162 656c    "SetSuiteLabel
-00003b10: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-00003b20: 207b 0a20 2020 2020 2230 223a 207b 7d0a   {.     "0": {}.
-00003b30: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
-00003b40: 5368 6f77 4869 6465 5072 6f63 6573 7322  ShowHideProcess"
-00003b50: 3a20 7b0a 2020 2020 2261 7267 7322 3a20  : {.    "args": 
-00003b60: 7b0a 2020 2020 2022 3022 3a20 7b7d 0a20  {.     "0": {}. 
-00003b70: 2020 207d 0a20 2020 7d2c 0a20 2020 2254     }.   },.   "T
-00003b80: 7261 6e73 666f 726d 5072 6f63 6573 7354  ransformProcessT
-00003b90: 7970 6522 3a20 7b0a 2020 2020 2261 7267  ype": {.    "arg
-00003ba0: 7322 3a20 7b0a 2020 2020 2022 3022 3a20  s": {.     "0": 
-00003bb0: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
-00003bc0: 2020 2254 7261 6e73 6c61 7469 6f6e 436f    "TranslationCo
-00003bd0: 7079 4465 7374 696e 6174 696f 6e54 7970  pyDestinationTyp
-00003be0: 6522 3a20 7b0a 2020 2020 2261 7267 7322  e": {.    "args"
-00003bf0: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
-00003c00: 2c0a 2020 2020 2022 3122 3a20 7b20 2274  ,.     "1": { "t
-00003c10: 7970 655f 6d6f 6469 6669 6572 223a 2022  ype_modifier": "
-00003c20: 6f22 2c20 2261 6c72 6561 6479 5f63 6672  o", "already_cfr
-00003c30: 6574 6169 6e65 6422 3a20 7472 7565 207d  etained": true }
-00003c40: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
-00003c50: 2254 7261 6e73 6c61 7469 6f6e 436f 7079  "TranslationCopy
-00003c60: 536f 7572 6365 5479 7065 223a 207b 0a20  SourceType": {. 
-00003c70: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
-00003c80: 2020 2230 223a 207b 7d2c 0a20 2020 2020    "0": {},.     
-00003c90: 2231 223a 207b 2022 7479 7065 5f6d 6f64  "1": { "type_mod
-00003ca0: 6966 6965 7222 3a20 226f 222c 2022 616c  ifier": "o", "al
-00003cb0: 7265 6164 795f 6366 7265 7461 696e 6564  ready_cfretained
-00003cc0: 223a 2074 7275 6520 7d0a 2020 2020 7d0a  ": true }.    }.
-00003cd0: 2020 207d 2c0a 2020 2022 5472 616e 736c     },.   "Transl
-00003ce0: 6174 696f 6e43 7265 6174 6522 3a20 7b0a  ationCreate": {.
-00003cf0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-00003d00: 2020 2022 3022 3a20 7b7d 2c0a 2020 2020     "0": {},.    
-00003d10: 2022 3122 3a20 7b7d 2c0a 2020 2020 2022   "1": {},.     "
-00003d20: 3322 3a20 7b20 2274 7970 655f 6d6f 6469  3": { "type_modi
-00003d30: 6669 6572 223a 2022 6f22 2c20 2261 6c72  fier": "o", "alr
-00003d40: 6561 6479 5f63 6672 6574 6169 6e65 6422  eady_cfretained"
-00003d50: 3a20 7472 7565 207d 0a20 2020 207d 0a20  : true }.    }. 
-00003d60: 2020 7d2c 0a20 2020 2254 7261 6e73 6c61    },.   "Transla
-00003d70: 7469 6f6e 4372 6561 7465 5769 7468 536f  tionCreateWithSo
-00003d80: 7572 6365 4172 7261 7922 3a20 7b0a 2020  urceArray": {.  
-00003d90: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
-00003da0: 2022 3022 3a20 7b7d 2c0a 2020 2020 2022   "0": {},.     "
-00003db0: 3222 3a20 7b20 2274 7970 655f 6d6f 6469  2": { "type_modi
-00003dc0: 6669 6572 223a 2022 6f22 2c20 2261 6c72  fier": "o", "alr
-00003dd0: 6561 6479 5f63 6672 6574 6169 6e65 6422  eady_cfretained"
-00003de0: 3a20 7472 7565 207d 2c0a 2020 2020 2022  : true },.     "
-00003df0: 3322 3a20 7b20 2274 7970 655f 6d6f 6469  3": { "type_modi
-00003e00: 6669 6572 223a 2022 6f22 2c20 2261 6c72  fier": "o", "alr
-00003e10: 6561 6479 5f63 6672 6574 6169 6e65 6422  eady_cfretained"
-00003e20: 3a20 7472 7565 207d 0a20 2020 207d 0a20  : true }.    }. 
-00003e30: 2020 7d2c 0a20 2020 2254 7261 6e73 6c61    },.   "Transla
-00003e40: 7469 6f6e 4765 7454 7261 6e73 6c61 7469  tionGetTranslati
-00003e50: 6f6e 466c 6167 7322 3a20 7b0a 2020 2020  onFlags": {.    
-00003e60: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
-00003e70: 3022 3a20 7b7d 2c0a 2020 2020 2022 3122  0": {},.     "1"
-00003e80: 3a20 7b20 2274 7970 655f 6d6f 6469 6669  : { "type_modifi
-00003e90: 6572 223a 2022 6f22 207d 0a20 2020 207d  er": "o" }.    }
-00003ea0: 0a20 2020 7d2c 0a20 2020 2254 7261 6e73  .   },.   "Trans
-00003eb0: 6c61 7469 6f6e 5065 7266 6f72 6d46 6f72  lationPerformFor
-00003ec0: 4461 7461 223a 207b 0a20 2020 2022 6172  Data": {.    "ar
-00003ed0: 6773 223a 207b 0a20 2020 2020 2230 223a  gs": {.     "0":
-00003ee0: 207b 7d2c 0a20 2020 2020 2231 223a 207b   {},.     "1": {
-00003ef0: 7d2c 0a20 2020 2020 2232 223a 207b 2022  },.     "2": { "
-00003f00: 7479 7065 5f6d 6f64 6966 6965 7222 3a20  type_modifier": 
-00003f10: 226f 222c 2022 616c 7265 6164 795f 6366  "o", "already_cf
-00003f20: 7265 7461 696e 6564 223a 2074 7275 6520  retained": true 
-00003f30: 7d0a 2020 2020 7d0a 2020 207d 2c0a 2020  }.    }.   },.  
-00003f40: 2022 5472 616e 736c 6174 696f 6e50 6572   "TranslationPer
-00003f50: 666f 726d 466f 7246 696c 6522 3a20 7b0a  formForFile": {.
-00003f60: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
-00003f70: 2020 2022 3022 3a20 7b7d 2c0a 2020 2020     "0": {},.    
-00003f80: 2022 3122 3a20 7b20 2274 7970 655f 6d6f   "1": { "type_mo
-00003f90: 6469 6669 6572 223a 2022 6e22 207d 2c0a  difier": "n" },.
-00003fa0: 2020 2020 2022 3222 3a20 7b20 2274 7970       "2": { "typ
-00003fb0: 655f 6d6f 6469 6669 6572 223a 2022 6e22  e_modifier": "n"
-00003fc0: 207d 2c0a 2020 2020 2022 3322 3a20 7b7d   },.     "3": {}
-00003fd0: 2c0a 2020 2020 2022 3422 3a20 7b20 2274  ,.     "4": { "t
-00003fe0: 7970 655f 6d6f 6469 6669 6572 223a 2022  ype_modifier": "
-00003ff0: 6f22 207d 0a20 2020 207d 0a20 2020 7d2c  o" }.    }.   },
-00004000: 0a20 2020 2254 7261 6e73 6c61 7469 6f6e  .   "Translation
-00004010: 5065 7266 6f72 6d46 6f72 5552 4c22 3a20  PerformForURL": 
-00004020: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
-00004030: 2020 2020 2022 3022 3a20 7b7d 2c0a 2020       "0": {},.  
-00004040: 2020 2022 3122 3a20 7b7d 2c0a 2020 2020     "1": {},.    
-00004050: 2022 3222 3a20 7b7d 2c0a 2020 2020 2022   "2": {},.     "
-00004060: 3322 3a20 7b20 2274 7970 655f 6d6f 6469  3": { "type_modi
-00004070: 6669 6572 223a 2022 6f22 2c20 2261 6c72  fier": "o", "alr
-00004080: 6561 6479 5f63 6672 6574 6169 6e65 6422  eady_cfretained"
-00004090: 3a20 7472 7565 7d0a 2020 2020 7d0a 2020  : true}.    }.  
-000040a0: 207d 2c0a 2020 2022 5541 5a6f 6f6d 4368   },.   "UAZoomCh
-000040b0: 616e 6765 466f 6375 7322 3a20 7b0a 2020  angeFocus": {.  
-000040c0: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
-000040d0: 2022 3022 3a20 7b20 2274 7970 655f 6d6f   "0": { "type_mo
-000040e0: 6469 6669 6572 223a 2022 6e22 207d 2c0a  difier": "n" },.
-000040f0: 2020 2020 2022 3122 3a20 7b20 2274 7970       "1": { "typ
-00004100: 655f 6d6f 6469 6669 6572 223a 2022 6e22  e_modifier": "n"
-00004110: 207d 0a20 2020 207d 0a20 2020 7d2c 0a20   }.    }.   },. 
-00004120: 2020 2257 616b 6555 7050 726f 6365 7373    "WakeUpProcess
-00004130: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
-00004140: 207b 0a20 2020 2020 2230 223a 207b 7d0a   {.     "0": {}.
-00004150: 2020 2020 7d0a 2020 207d 0a20 207d 2c0a      }.   }.  },.
-00004160: 2020 2269 6e66 6f72 6d61 6c5f 7072 6f74    "informal_prot
-00004170: 6f63 6f6c 7322 3a20 7b7d 2c0a 2020 2273  ocols": {},.  "s
-00004180: 7472 7563 7473 223a 207b 0a20 2020 224c  tructs": {.   "L
-00004190: 6175 6e63 6850 6172 616d 426c 6f63 6b52  aunchParamBlockR
-000041a0: 6563 223a 207b 2022 6967 6e6f 7265 223a  ec": { "ignore":
-000041b0: 2074 7275 6520 7d2c 0a20 2020 2241 7070   true },.   "App
-000041c0: 5061 7261 6d65 7465 7273 223a 207b 2022  Parameters": { "
-000041d0: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-000041e0: 0a20 2020 2249 4344 6972 5370 6563 223a  .   "ICDirSpec":
-000041f0: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
-00004200: 6520 7d2c 0a20 2020 2249 4346 6f6e 7452  e },.   "ICFontR
-00004210: 6563 6f72 6422 3a20 7b20 2269 676e 6f72  ecord": { "ignor
-00004220: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-00004230: 4943 4368 6172 5461 626c 6522 3a20 7b20  ICCharTable": { 
-00004240: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
-00004250: 2c0a 2020 2022 4943 4170 7053 7065 6322  ,.   "ICAppSpec"
-00004260: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-00004270: 7565 207d 2c0a 2020 2022 4943 4170 7053  ue },.   "ICAppS
-00004280: 7065 634c 6973 7422 3a20 7b20 2269 676e  pecList": { "ign
-00004290: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
-000042a0: 2022 4943 4669 6c65 5370 6563 223a 207b   "ICFileSpec": {
-000042b0: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
-000042c0: 7d2c 0a20 2020 2249 434d 6170 456e 7472  },.   "ICMapEntr
-000042d0: 7922 3a20 7b20 2269 676e 6f72 6522 3a20  y": { "ignore": 
-000042e0: 7472 7565 207d 2c0a 2020 2022 4943 5365  true },.   "ICSe
-000042f0: 7276 6963 6545 6e74 7279 223a 207b 2022  rviceEntry": { "
-00004300: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-00004310: 0a20 2020 2249 4353 6572 7669 6365 7322  .   "ICServices"
-00004320: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-00004330: 7565 207d 0a20 207d 2c0a 2020 2265 6e75  ue }.  },.  "enu
-00004340: 6d22 3a20 7b0a 2020 2022 6963 5072 6566  m": {.   "icPref
-00004350: 4e6f 7446 6f75 6e64 4572 7222 3a20 7b20  NotFoundErr": { 
-00004360: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
-00004370: 2c0a 2020 2022 6963 5065 726d 4572 7222  ,.   "icPermErr"
-00004380: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-00004390: 7565 207d 2c0a 2020 2022 6963 5072 6566  ue },.   "icPref
-000043a0: 4461 7461 4572 7222 3a20 7b20 2269 676e  DataErr": { "ign
-000043b0: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
-000043c0: 2022 6963 496e 7465 726e 616c 4572 7222   "icInternalErr"
-000043d0: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-000043e0: 7565 207d 2c0a 2020 2022 6963 5472 756e  ue },.   "icTrun
-000043f0: 6361 7465 6445 7272 223a 207b 2022 6967  catedErr": { "ig
-00004400: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
-00004410: 2020 2269 634e 6f4d 6f72 6557 7269 7465    "icNoMoreWrite
-00004420: 7273 4572 7222 3a20 7b20 2269 676e 6f72  rsErr": { "ignor
-00004430: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-00004440: 6963 4e6f 7468 696e 6754 6f4f 7665 7272  icNothingToOverr
-00004450: 6964 6545 7272 223a 207b 2022 6967 6e6f  ideErr": { "igno
-00004460: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
-00004470: 2269 634e 6f55 524c 4572 7222 3a20 7b20  "icNoURLErr": { 
-00004480: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
-00004490: 2c0a 2020 2022 6963 436f 6e66 6967 4e6f  ,.   "icConfigNo
-000044a0: 7446 6f75 6e64 4572 7222 3a20 7b20 2269  tFoundErr": { "i
-000044b0: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
-000044c0: 2020 2022 6963 436f 6e66 6967 496e 6170     "icConfigInap
-000044d0: 7072 6f70 7269 6174 6545 7272 223a 207b  propriateErr": {
-000044e0: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
-000044f0: 7d2c 0a20 2020 2269 6350 726f 6669 6c65  },.   "icProfile
-00004500: 4e6f 7446 6f75 6e64 4572 7222 3a20 7b20  NotFoundErr": { 
-00004510: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
-00004520: 2c0a 2020 2022 6963 546f 6f4d 616e 7950  ,.   "icTooManyP
-00004530: 726f 6669 6c65 7345 7272 223a 207b 2022  rofilesErr": { "
-00004540: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-00004550: 0a20 2020 226b 4943 436f 6d70 6f6e 656e  .   "kICComponen
-00004560: 7449 6e74 6572 6661 6365 5665 7273 696f  tInterfaceVersio
-00004570: 6e30 223a 207b 2022 6967 6e6f 7265 223a  n0": { "ignore":
-00004580: 2074 7275 6520 7d2c 0a20 2020 226b 4943   true },.   "kIC
-00004590: 436f 6d70 6f6e 656e 7449 6e74 6572 6661  ComponentInterfa
-000045a0: 6365 5665 7273 696f 6e31 223a 207b 2022  ceVersion1": { "
-000045b0: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-000045c0: 0a20 2020 226b 4943 436f 6d70 6f6e 656e  .   "kICComponen
-000045d0: 7449 6e74 6572 6661 6365 5665 7273 696f  tInterfaceVersio
-000045e0: 6e32 223a 207b 2022 6967 6e6f 7265 223a  n2": { "ignore":
-000045f0: 2074 7275 6520 7d2c 0a20 2020 226b 4943   true },.   "kIC
-00004600: 436f 6d70 6f6e 656e 7449 6e74 6572 6661  ComponentInterfa
-00004610: 6365 5665 7273 696f 6e33 223a 207b 2022  ceVersion3": { "
-00004620: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-00004630: 0a20 2020 226b 4943 436f 6d70 6f6e 656e  .   "kICComponen
-00004640: 7449 6e74 6572 6661 6365 5665 7273 696f  tInterfaceVersio
-00004650: 6e34 223a 207b 2022 6967 6e6f 7265 223a  n4": { "ignore":
-00004660: 2074 7275 6520 7d2c 0a20 2020 226b 4943   true },.   "kIC
-00004670: 436f 6d70 6f6e 656e 7449 6e74 6572 6661  ComponentInterfa
-00004680: 6365 5665 7273 696f 6e22 3a20 7b20 2269  ceVersion": { "i
-00004690: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
-000046a0: 2020 2022 6b49 4341 7474 724c 6f63 6b65     "kICAttrLocke
-000046b0: 6442 6974 223a 207b 2022 6967 6e6f 7265  dBit": { "ignore
-000046c0: 223a 2074 7275 6520 7d2c 0a20 2020 226b  ": true },.   "k
-000046d0: 4943 4174 7472 566f 6c61 7469 6c65 4269  ICAttrVolatileBi
-000046e0: 7422 3a20 7b20 2269 676e 6f72 6522 3a20  t": { "ignore": 
-000046f0: 7472 7565 207d 2c0a 2020 2022 6b49 4341  true },.   "kICA
-00004700: 7474 724e 6f43 6861 6e67 6522 3a20 7b20  ttrNoChange": { 
-00004710: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
-00004720: 2c0a 2020 2022 6b49 4341 7474 724c 6f63  ,.   "kICAttrLoc
-00004730: 6b65 644d 6173 6b22 3a20 7b20 2269 676e  kedMask": { "ign
-00004740: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
-00004750: 2022 6b49 4341 7474 7256 6f6c 6174 696c   "kICAttrVolatil
-00004760: 654d 6173 6b22 3a20 7b20 2269 676e 6f72  eMask": { "ignor
-00004770: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-00004780: 6963 4e6f 5065 726d 223a 207b 2022 6967  icNoPerm": { "ig
-00004790: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
-000047a0: 2020 2269 6352 6561 644f 6e6c 7950 6572    "icReadOnlyPer
-000047b0: 6d22 3a20 7b20 2269 676e 6f72 6522 3a20  m": { "ignore": 
-000047c0: 7472 7565 207d 2c0a 2020 2022 6963 5265  true },.   "icRe
-000047d0: 6164 5772 6974 6550 6572 6d22 3a20 7b20  adWritePerm": { 
-000047e0: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
-000047f0: 2c0a 2020 2022 6b49 434e 696c 5072 6f66  ,.   "kICNilProf
-00004800: 696c 6549 4422 3a20 7b20 2269 676e 6f72  ileID": { "ignor
-00004810: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-00004820: 6b49 434e 6f55 7365 7249 6e74 6572 6163  kICNoUserInterac
-00004830: 7469 6f6e 4269 7422 3a20 7b20 2269 676e  tionBit": { "ign
-00004840: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
-00004850: 2022 6b49 434e 6f55 7365 7249 6e74 6572   "kICNoUserInter
-00004860: 6163 7469 6f6e 4d61 736b 223a 207b 2022  actionMask": { "
-00004870: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-00004880: 0a20 2020 226b 4943 4669 6c65 5479 7065  .   "kICFileType
-00004890: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-000048a0: 7275 6520 7d2c 0a20 2020 226b 4943 4372  rue },.   "kICCr
-000048b0: 6561 746f 7222 3a20 7b20 2269 676e 6f72  eator": { "ignor
+00003350: 2022 5061 7374 6562 6f61 7264 4765 7449   "PasteboardGetI
+00003360: 7465 6d49 6465 6e74 6966 6965 7222 3a20  temIdentifier": 
+00003370: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
+00003380: 2020 2020 2022 3022 3a20 7b7d 2c0a 2020       "0": {},.  
+00003390: 2020 2022 3222 3a20 7b20 2274 7970 655f     "2": { "type_
+000033a0: 6d6f 6469 6669 6572 223a 2022 6f22 207d  modifier": "o" }
+000033b0: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
+000033c0: 2250 6173 7465 626f 6172 6450 7574 4974  "PasteboardPutIt
+000033d0: 656d 466c 6176 6f72 223a 207b 0a20 2020  emFlavor": {.   
+000033e0: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
+000033f0: 2230 223a 207b 7d2c 0a20 2020 2020 2231  "0": {},.     "1
+00003400: 223a 207b 7d2c 0a20 2020 2020 2232 223a  ": {},.     "2":
+00003410: 207b 7d2c 0a20 2020 2020 2233 223a 207b   {},.     "3": {
+00003420: 7d0a 2020 2020 7d0a 2020 207d 2c0a 2020  }.    }.   },.  
+00003430: 2022 5061 7374 6562 6f61 7264 5265 736f   "PasteboardReso
+00003440: 6c76 6550 726f 6d69 7365 7322 3a20 7b0a  lvePromises": {.
+00003450: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+00003460: 2020 2022 3022 3a20 7b7d 0a20 2020 207d     "0": {}.    }
+00003470: 0a20 2020 7d2c 0a20 2020 2250 6173 7465  .   },.   "Paste
+00003480: 626f 6172 6453 6574 5061 7374 654c 6f63  boardSetPasteLoc
+00003490: 6174 696f 6e22 3a20 7b0a 2020 2020 2261  ation": {.    "a
+000034a0: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
+000034b0: 3a20 7b7d 2c0a 2020 2020 2022 3122 3a20  : {},.     "1": 
+000034c0: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
+000034d0: 2020 2250 6173 7465 626f 6172 6453 6574    "PasteboardSet
+000034e0: 5072 6f6d 6973 654b 6565 7065 7222 3a20  PromiseKeeper": 
+000034f0: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
+00003500: 2020 2020 2022 3022 3a20 7b7d 2c0a 2020       "0": {},.  
+00003510: 2020 2022 3122 3a20 7b0a 2020 2020 2020     "1": {.      
+00003520: 2266 756e 6374 696f 6e22 3a20 7b0a 2020  "function": {.  
+00003530: 2020 2020 2022 6172 6773 223a 205b 0a20       "args": [. 
+00003540: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00003550: 2020 2274 7970 6573 7472 223a 2022 5e7b    "typestr": "^{
+00003560: 4f70 6171 7565 5061 7374 6562 6f61 7264  OpaquePasteboard
+00003570: 5265 663d 7d22 0a20 2020 2020 2020 207d  Ref=}".        }
+00003580: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+00003590: 2020 2020 2022 7479 7065 7374 7222 3a20       "typestr": 
+000035a0: 225e 7622 0a20 2020 2020 2020 207d 2c0a  "^v".        },.
+000035b0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000035c0: 2020 2022 7479 7065 7374 7222 3a20 225e     "typestr": "^
+000035d0: 7b5f 5f43 4653 7472 696e 673d 7d22 0a20  {__CFString=}". 
+000035e0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000035f0: 2020 7b0a 2020 2020 2020 2020 2022 7479    {.         "ty
+00003600: 7065 7374 7222 3a20 225e 7622 0a20 2020  pestr": "^v".   
+00003610: 2020 2020 207d 0a20 2020 2020 2020 5d2c       }.       ],
+00003620: 0a20 2020 2020 2020 2272 6574 7661 6c22  .       "retval"
+00003630: 3a20 7b0a 2020 2020 2020 2020 2274 7970  : {.        "typ
+00003640: 6573 7472 223a 2022 6922 0a20 2020 2020  estr": "i".     
+00003650: 2020 7d0a 2020 2020 2020 7d0a 2020 2020    }.      }.    
+00003660: 207d 2c0a 2020 2020 2022 3222 3a20 7b7d   },.     "2": {}
+00003670: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
+00003680: 2250 6173 7465 626f 6172 6453 796e 6368  "PasteboardSynch
+00003690: 726f 6e69 7a65 223a 207b 0a20 2020 2022  ronize": {.    "
+000036a0: 6172 6773 223a 207b 0a20 2020 2020 2230  args": {.     "0
+000036b0: 223a 207b 7d0a 2020 2020 7d0a 2020 207d  ": {}.    }.   }
+000036c0: 2c0a 2020 2022 506c 6f74 4349 636f 6e22  ,.   "PlotCIcon"
+000036d0: 3a20 7b0a 2020 2020 2261 7267 7322 3a20  : {.    "args": 
+000036e0: 7b0a 2020 2020 2022 3022 3a20 7b7d 2c0a  {.     "0": {},.
+000036f0: 2020 2020 2022 3122 3a20 7b7d 0a20 2020       "1": {}.   
+00003700: 207d 0a20 2020 7d2c 0a20 2020 2250 6c6f   }.   },.   "Plo
+00003710: 7443 4963 6f6e 4861 6e64 6c65 223a 207b  tCIconHandle": {
+00003720: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
+00003730: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
+00003740: 2020 2233 223a 207b 7d0a 2020 2020 7d0a    "3": {}.    }.
+00003750: 2020 207d 2c0a 2020 2022 506c 6f74 4963     },.   "PlotIc
+00003760: 6f6e 223a 207b 0a20 2020 2022 6172 6773  on": {.    "args
+00003770: 223a 207b 0a20 2020 2020 2230 223a 207b  ": {.     "0": {
+00003780: 7d2c 0a20 2020 2020 2231 223a 207b 7d0a  },.     "1": {}.
+00003790: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
+000037a0: 506c 6f74 4963 6f6e 4861 6e64 6c65 223a  PlotIconHandle":
+000037b0: 207b 0a20 2020 2022 6172 6773 223a 207b   {.    "args": {
+000037c0: 0a20 2020 2020 2230 223a 207b 7d2c 0a20  .     "0": {},. 
+000037d0: 2020 2020 2233 223a 207b 7d0a 2020 2020      "3": {}.    
+000037e0: 7d0a 2020 207d 2c0a 2020 2022 506c 6f74  }.   },.   "Plot
+000037f0: 4963 6f6e 4944 223a 207b 0a20 2020 2022  IconID": {.    "
+00003800: 6172 6773 223a 207b 0a20 2020 2020 2230  args": {.     "0
+00003810: 223a 207b 7d0a 2020 2020 7d0a 2020 207d  ": {}.    }.   }
+00003820: 2c0a 2020 2022 506c 6f74 4963 6f6e 4d65  ,.   "PlotIconMe
+00003830: 7468 6f64 223a 207b 0a20 2020 2022 6172  thod": {.    "ar
+00003840: 6773 223a 207b 0a20 2020 2020 2230 223a  gs": {.     "0":
+00003850: 207b 7d2c 0a20 2020 2020 2233 223a 207b   {},.     "3": {
+00003860: 7d2c 0a20 2020 2020 2234 223a 207b 7d0a  },.     "4": {}.
+00003870: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
+00003880: 506c 6f74 4963 6f6e 5265 6622 3a20 7b0a  PlotIconRef": {.
+00003890: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+000038a0: 2020 2022 3022 3a20 7b7d 2c0a 2020 2020     "0": {},.    
+000038b0: 2022 3422 3a20 7b7d 0a20 2020 207d 0a20   "4": {}.    }. 
+000038c0: 2020 7d2c 0a20 2020 2250 6c6f 7449 636f    },.   "PlotIco
+000038d0: 6e52 6566 496e 436f 6e74 6578 7422 3a20  nRefInContext": 
+000038e0: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
+000038f0: 2020 2020 2022 3022 3a20 7b7d 2c0a 2020       "0": {},.  
+00003900: 2020 2022 3122 3a20 7b20 2274 7970 655f     "1": { "type_
+00003910: 6d6f 6469 6669 6572 223a 2022 6e22 207d  modifier": "n" }
+00003920: 2c0a 2020 2020 2022 3422 3a20 7b20 2274  ,.     "4": { "t
+00003930: 7970 655f 6d6f 6469 6669 6572 223a 2022  ype_modifier": "
+00003940: 6e22 207d 2c0a 2020 2020 2022 3622 3a20  n" },.     "6": 
+00003950: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
+00003960: 2020 2250 6c6f 7449 636f 6e53 7569 7465    "PlotIconSuite
+00003970: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
+00003980: 207b 0a20 2020 2020 2230 223a 207b 7d2c   {.     "0": {},
+00003990: 0a20 2020 2020 2233 223a 207b 7d0a 2020  .     "3": {}.  
+000039a0: 2020 7d0a 2020 207d 2c0a 2020 2022 506c    }.   },.   "Pl
+000039b0: 6f74 5349 434e 4861 6e64 6c65 223a 207b  otSICNHandle": {
+000039c0: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
+000039d0: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
+000039e0: 2020 2233 223a 207b 7d0a 2020 2020 7d0a    "3": {}.    }.
+000039f0: 2020 207d 2c0a 2020 2022 5072 6f63 6573     },.   "Proces
+00003a00: 7349 6e66 6f72 6d61 7469 6f6e 436f 7079  sInformationCopy
+00003a10: 4469 6374 696f 6e61 7279 223a 207b 0a20  Dictionary": {. 
+00003a20: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
+00003a30: 2020 2230 223a 207b 2274 7970 655f 6d6f    "0": {"type_mo
+00003a40: 6469 6669 6572 223a 2022 6e22 7d0a 2020  difier": "n"}.  
+00003a50: 2020 7d2c 0a20 2020 2022 7265 7476 616c    },.    "retval
+00003a60: 223a 207b 0a20 2020 2020 2261 6c72 6561  ": {.     "alrea
+00003a70: 6479 5f63 6672 6574 6169 6e65 6422 3a20  dy_cfretained": 
+00003a80: 7472 7565 0a20 2020 207d 0a20 2020 7d2c  true.    }.   },
+00003a90: 0a20 2020 2250 7449 6e49 636f 6e49 4422  .   "PtInIconID"
+00003aa0: 3a20 7b0a 2020 2020 2261 7267 7322 3a20  : {.    "args": 
+00003ab0: 7b0a 2020 2020 2022 3122 3a20 7b7d 0a20  {.     "1": {}. 
+00003ac0: 2020 207d 0a20 2020 7d2c 0a20 2020 2250     }.   },.   "P
+00003ad0: 7449 6e49 636f 6e4d 6574 686f 6422 3a20  tInIconMethod": 
+00003ae0: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
+00003af0: 2020 2020 2022 3122 3a20 7b7d 2c0a 2020       "1": {},.  
+00003b00: 2020 2022 3322 3a20 7b7d 2c0a 2020 2020     "3": {},.    
+00003b10: 2022 3422 3a20 7b7d 0a20 2020 207d 0a20   "4": {}.    }. 
+00003b20: 2020 7d2c 0a20 2020 2250 7449 6e49 636f    },.   "PtInIco
+00003b30: 6e52 6566 223a 207b 0a20 2020 2022 6172  nRef": {.    "ar
+00003b40: 6773 223a 207b 0a20 2020 2020 2230 223a  gs": {.     "0":
+00003b50: 207b 7d2c 0a20 2020 2020 2231 223a 207b   {},.     "1": {
+00003b60: 7d2c 0a20 2020 2020 2234 223a 207b 7d0a  },.     "4": {}.
+00003b70: 2020 2020 7d0a 2020 207d 2c0a 2020 2022      }.   },.   "
+00003b80: 5074 496e 4963 6f6e 5375 6974 6522 3a20  PtInIconSuite": 
+00003b90: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
+00003ba0: 2020 2020 2022 3122 3a20 7b7d 2c0a 2020       "1": {},.  
+00003bb0: 2020 2022 3322 3a20 7b7d 0a20 2020 207d     "3": {}.    }
+00003bc0: 0a20 2020 7d2c 0a20 2020 2252 6563 7449  .   },.   "RectI
+00003bd0: 6e49 636f 6e49 4422 3a20 7b0a 2020 2020  nIconID": {.    
+00003be0: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
+00003bf0: 3022 3a20 7b7d 2c0a 2020 2020 2022 3122  0": {},.     "1"
+00003c00: 3a20 7b7d 0a20 2020 207d 0a20 2020 7d2c  : {}.    }.   },
+00003c10: 0a20 2020 2252 6563 7449 6e49 636f 6e4d  .   "RectInIconM
+00003c20: 6574 686f 6422 3a20 7b0a 2020 2020 2261  ethod": {.    "a
+00003c30: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
+00003c40: 3a20 7b7d 2c0a 2020 2020 2022 3122 3a20  : {},.     "1": 
+00003c50: 7b7d 2c0a 2020 2020 2022 3322 3a20 7b7d  {},.     "3": {}
+00003c60: 2c0a 2020 2020 2022 3422 3a20 7b7d 0a20  ,.     "4": {}. 
+00003c70: 2020 207d 0a20 2020 7d2c 0a20 2020 2252     }.   },.   "R
+00003c80: 6563 7449 6e49 636f 6e52 6566 223a 207b  ectInIconRef": {
+00003c90: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
+00003ca0: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
+00003cb0: 2020 2231 223a 207b 7d2c 0a20 2020 2020    "1": {},.     
+00003cc0: 2234 223a 207b 7d0a 2020 2020 7d0a 2020  "4": {}.    }.  
+00003cd0: 207d 2c0a 2020 2022 5265 6374 496e 4963   },.   "RectInIc
+00003ce0: 6f6e 5375 6974 6522 3a20 7b0a 2020 2020  onSuite": {.    
+00003cf0: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
+00003d00: 3022 3a20 7b7d 2c0a 2020 2020 2022 3122  0": {},.     "1"
+00003d10: 3a20 7b7d 2c0a 2020 2020 2022 3322 3a20  : {},.     "3": 
+00003d20: 7b7d 0a20 2020 207d 0a20 2020 7d2c 0a20  {}.    }.   },. 
+00003d30: 2020 2253 616d 6550 726f 6365 7373 223a    "SameProcess":
+00003d40: 207b 0a20 2020 2022 6172 6773 223a 207b   {.    "args": {
+00003d50: 0a20 2020 2020 2230 223a 207b 2274 7970  .     "0": {"typ
+00003d60: 655f 6d6f 6469 6669 6572 223a 2022 6e22  e_modifier": "n"
+00003d70: 207d 2c0a 2020 2020 2022 3122 3a20 7b22   },.     "1": {"
+00003d80: 7479 7065 5f6d 6f64 6966 6965 7222 3a20  type_modifier": 
+00003d90: 226e 2220 7d2c 0a20 2020 2020 2232 223a  "n" },.     "2":
+00003da0: 207b 2274 7970 655f 6d6f 6469 6669 6572   {"type_modifier
+00003db0: 223a 2022 6f22 207d 0a20 2020 207d 0a20  ": "o" }.    }. 
+00003dc0: 2020 7d2c 0a20 2020 2253 6574 4672 6f6e    },.   "SetFron
+00003dd0: 7450 726f 6365 7373 223a 207b 0a20 2020  tProcess": {.   
+00003de0: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
+00003df0: 2230 223a 207b 2022 7479 7065 5f6d 6f64  "0": { "type_mod
+00003e00: 6966 6965 7222 3a20 226e 2220 7d0a 2020  ifier": "n" }.  
+00003e10: 2020 7d0a 2020 207d 2c0a 2020 2022 5365    }.   },.   "Se
+00003e20: 7446 726f 6e74 5072 6f63 6573 7357 6974  tFrontProcessWit
+00003e30: 684f 7074 696f 6e73 223a 207b 0a20 2020  hOptions": {.   
+00003e40: 2022 6172 6773 223a 207b 0a20 2020 2020   "args": {.     
+00003e50: 2230 223a 207b 2022 7479 7065 5f6d 6f64  "0": { "type_mod
+00003e60: 6966 6965 7222 3a20 226e 2220 7d0a 2020  ifier": "n" }.  
+00003e70: 2020 7d0a 2020 207d 2c0a 2020 2022 5365    }.   },.   "Se
+00003e80: 7449 636f 6e43 6163 6865 4461 7461 223a  tIconCacheData":
+00003e90: 207b 0a20 2020 2022 6172 6773 223a 207b   {.    "args": {
+00003ea0: 0a20 2020 2020 2230 223a 207b 7d2c 0a20  .     "0": {},. 
+00003eb0: 2020 2020 2231 223a 207b 7d0a 2020 2020      "1": {}.    
+00003ec0: 7d0a 2020 207d 2c0a 2020 2022 5365 7449  }.   },.   "SetI
+00003ed0: 636f 6e43 6163 6865 5072 6f63 223a 207b  conCacheProc": {
+00003ee0: 0a20 2020 2022 6172 6773 223a 207b 0a20  .    "args": {. 
+00003ef0: 2020 2020 2230 223a 207b 7d2c 0a20 2020      "0": {},.   
+00003f00: 2020 2231 223a 207b 7d0a 2020 2020 7d0a    "1": {}.    }.
+00003f10: 2020 207d 2c0a 2020 2022 5365 7449 636f     },.   "SetIco
+00003f20: 6e46 616d 696c 7944 6174 6122 3a20 7b0a  nFamilyData": {.
+00003f30: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+00003f40: 2020 2022 3022 3a20 7b7d 2c0a 2020 2020     "0": {},.    
+00003f50: 2022 3222 3a20 7b7d 0a20 2020 207d 0a20   "2": {}.    }. 
+00003f60: 2020 7d2c 0a20 2020 2253 6574 5375 6974    },.   "SetSuit
+00003f70: 654c 6162 656c 223a 207b 0a20 2020 2022  eLabel": {.    "
+00003f80: 6172 6773 223a 207b 0a20 2020 2020 2230  args": {.     "0
+00003f90: 223a 207b 7d0a 2020 2020 7d0a 2020 207d  ": {}.    }.   }
+00003fa0: 2c0a 2020 2022 5368 6f77 4869 6465 5072  ,.   "ShowHidePr
+00003fb0: 6f63 6573 7322 3a20 7b0a 2020 2020 2261  ocess": {.    "a
+00003fc0: 7267 7322 3a20 7b0a 2020 2020 2022 3022  rgs": {.     "0"
+00003fd0: 3a20 7b20 2274 7970 655f 6d6f 6469 6669  : { "type_modifi
+00003fe0: 6572 223a 2022 6e22 7d0a 2020 2020 7d0a  er": "n"}.    }.
+00003ff0: 2020 207d 2c0a 2020 2022 5472 616e 7366     },.   "Transf
+00004000: 6f72 6d50 726f 6365 7373 5479 7065 223a  ormProcessType":
+00004010: 207b 0a20 2020 2022 6172 6773 223a 207b   {.    "args": {
+00004020: 0a20 2020 2020 2230 223a 207b 2022 7479  .     "0": { "ty
+00004030: 7065 5f6d 6f64 6966 6965 7222 3a20 226e  pe_modifier": "n
+00004040: 227d 0a20 2020 207d 0a20 2020 7d2c 0a20  "}.    }.   },. 
+00004050: 2020 2254 7261 6e73 6c61 7469 6f6e 436f    "TranslationCo
+00004060: 7079 4465 7374 696e 6174 696f 6e54 7970  pyDestinationTyp
+00004070: 6522 3a20 7b0a 2020 2020 2261 7267 7322  e": {.    "args"
+00004080: 3a20 7b0a 2020 2020 2022 3022 3a20 7b7d  : {.     "0": {}
+00004090: 2c0a 2020 2020 2022 3122 3a20 7b20 2274  ,.     "1": { "t
+000040a0: 7970 655f 6d6f 6469 6669 6572 223a 2022  ype_modifier": "
+000040b0: 6f22 2c20 2261 6c72 6561 6479 5f63 6672  o", "already_cfr
+000040c0: 6574 6169 6e65 6422 3a20 7472 7565 207d  etained": true }
+000040d0: 0a20 2020 207d 0a20 2020 7d2c 0a20 2020  .    }.   },.   
+000040e0: 2254 7261 6e73 6c61 7469 6f6e 436f 7079  "TranslationCopy
+000040f0: 536f 7572 6365 5479 7065 223a 207b 0a20  SourceType": {. 
+00004100: 2020 2022 6172 6773 223a 207b 0a20 2020     "args": {.   
+00004110: 2020 2230 223a 207b 7d2c 0a20 2020 2020    "0": {},.     
+00004120: 2231 223a 207b 2022 7479 7065 5f6d 6f64  "1": { "type_mod
+00004130: 6966 6965 7222 3a20 226f 222c 2022 616c  ifier": "o", "al
+00004140: 7265 6164 795f 6366 7265 7461 696e 6564  ready_cfretained
+00004150: 223a 2074 7275 6520 7d0a 2020 2020 7d0a  ": true }.    }.
+00004160: 2020 207d 2c0a 2020 2022 5472 616e 736c     },.   "Transl
+00004170: 6174 696f 6e43 7265 6174 6522 3a20 7b0a  ationCreate": {.
+00004180: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+00004190: 2020 2022 3022 3a20 7b7d 2c0a 2020 2020     "0": {},.    
+000041a0: 2022 3122 3a20 7b7d 2c0a 2020 2020 2022   "1": {},.     "
+000041b0: 3322 3a20 7b20 2274 7970 655f 6d6f 6469  3": { "type_modi
+000041c0: 6669 6572 223a 2022 6f22 2c20 2261 6c72  fier": "o", "alr
+000041d0: 6561 6479 5f63 6672 6574 6169 6e65 6422  eady_cfretained"
+000041e0: 3a20 7472 7565 207d 0a20 2020 207d 0a20  : true }.    }. 
+000041f0: 2020 7d2c 0a20 2020 2254 7261 6e73 6c61    },.   "Transla
+00004200: 7469 6f6e 4372 6561 7465 5769 7468 536f  tionCreateWithSo
+00004210: 7572 6365 4172 7261 7922 3a20 7b0a 2020  urceArray": {.  
+00004220: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
+00004230: 2022 3022 3a20 7b7d 2c0a 2020 2020 2022   "0": {},.     "
+00004240: 3222 3a20 7b20 2274 7970 655f 6d6f 6469  2": { "type_modi
+00004250: 6669 6572 223a 2022 6f22 2c20 2261 6c72  fier": "o", "alr
+00004260: 6561 6479 5f63 6672 6574 6169 6e65 6422  eady_cfretained"
+00004270: 3a20 7472 7565 207d 2c0a 2020 2020 2022  : true },.     "
+00004280: 3322 3a20 7b20 2274 7970 655f 6d6f 6469  3": { "type_modi
+00004290: 6669 6572 223a 2022 6f22 2c20 2261 6c72  fier": "o", "alr
+000042a0: 6561 6479 5f63 6672 6574 6169 6e65 6422  eady_cfretained"
+000042b0: 3a20 7472 7565 207d 0a20 2020 207d 0a20  : true }.    }. 
+000042c0: 2020 7d2c 0a20 2020 2254 7261 6e73 6c61    },.   "Transla
+000042d0: 7469 6f6e 4765 7454 7261 6e73 6c61 7469  tionGetTranslati
+000042e0: 6f6e 466c 6167 7322 3a20 7b0a 2020 2020  onFlags": {.    
+000042f0: 2261 7267 7322 3a20 7b0a 2020 2020 2022  "args": {.     "
+00004300: 3022 3a20 7b7d 2c0a 2020 2020 2022 3122  0": {},.     "1"
+00004310: 3a20 7b20 2274 7970 655f 6d6f 6469 6669  : { "type_modifi
+00004320: 6572 223a 2022 6f22 207d 0a20 2020 207d  er": "o" }.    }
+00004330: 0a20 2020 7d2c 0a20 2020 2254 7261 6e73  .   },.   "Trans
+00004340: 6c61 7469 6f6e 5065 7266 6f72 6d46 6f72  lationPerformFor
+00004350: 4461 7461 223a 207b 0a20 2020 2022 6172  Data": {.    "ar
+00004360: 6773 223a 207b 0a20 2020 2020 2230 223a  gs": {.     "0":
+00004370: 207b 7d2c 0a20 2020 2020 2231 223a 207b   {},.     "1": {
+00004380: 7d2c 0a20 2020 2020 2232 223a 207b 2022  },.     "2": { "
+00004390: 7479 7065 5f6d 6f64 6966 6965 7222 3a20  type_modifier": 
+000043a0: 226f 222c 2022 616c 7265 6164 795f 6366  "o", "already_cf
+000043b0: 7265 7461 696e 6564 223a 2074 7275 6520  retained": true 
+000043c0: 7d0a 2020 2020 7d0a 2020 207d 2c0a 2020  }.    }.   },.  
+000043d0: 2022 5472 616e 736c 6174 696f 6e50 6572   "TranslationPer
+000043e0: 666f 726d 466f 7246 696c 6522 3a20 7b0a  formForFile": {.
+000043f0: 2020 2020 2261 7267 7322 3a20 7b0a 2020      "args": {.  
+00004400: 2020 2022 3022 3a20 7b7d 2c0a 2020 2020     "0": {},.    
+00004410: 2022 3122 3a20 7b20 2274 7970 655f 6d6f   "1": { "type_mo
+00004420: 6469 6669 6572 223a 2022 6e22 207d 2c0a  difier": "n" },.
+00004430: 2020 2020 2022 3222 3a20 7b20 2274 7970       "2": { "typ
+00004440: 655f 6d6f 6469 6669 6572 223a 2022 6e22  e_modifier": "n"
+00004450: 207d 2c0a 2020 2020 2022 3322 3a20 7b7d   },.     "3": {}
+00004460: 2c0a 2020 2020 2022 3422 3a20 7b20 2274  ,.     "4": { "t
+00004470: 7970 655f 6d6f 6469 6669 6572 223a 2022  ype_modifier": "
+00004480: 6f22 207d 0a20 2020 207d 0a20 2020 7d2c  o" }.    }.   },
+00004490: 0a20 2020 2254 7261 6e73 6c61 7469 6f6e  .   "Translation
+000044a0: 5065 7266 6f72 6d46 6f72 5552 4c22 3a20  PerformForURL": 
+000044b0: 7b0a 2020 2020 2261 7267 7322 3a20 7b0a  {.    "args": {.
+000044c0: 2020 2020 2022 3022 3a20 7b7d 2c0a 2020       "0": {},.  
+000044d0: 2020 2022 3122 3a20 7b7d 2c0a 2020 2020     "1": {},.    
+000044e0: 2022 3222 3a20 7b7d 2c0a 2020 2020 2022   "2": {},.     "
+000044f0: 3322 3a20 7b20 2274 7970 655f 6d6f 6469  3": { "type_modi
+00004500: 6669 6572 223a 2022 6f22 2c20 2261 6c72  fier": "o", "alr
+00004510: 6561 6479 5f63 6672 6574 6169 6e65 6422  eady_cfretained"
+00004520: 3a20 7472 7565 7d0a 2020 2020 7d0a 2020  : true}.    }.  
+00004530: 207d 2c0a 2020 2022 5541 5a6f 6f6d 4368   },.   "UAZoomCh
+00004540: 616e 6765 466f 6375 7322 3a20 7b0a 2020  angeFocus": {.  
+00004550: 2020 2261 7267 7322 3a20 7b0a 2020 2020    "args": {.    
+00004560: 2022 3022 3a20 7b20 2274 7970 655f 6d6f   "0": { "type_mo
+00004570: 6469 6669 6572 223a 2022 6e22 207d 2c0a  difier": "n" },.
+00004580: 2020 2020 2022 3122 3a20 7b20 2274 7970       "1": { "typ
+00004590: 655f 6d6f 6469 6669 6572 223a 2022 6e22  e_modifier": "n"
+000045a0: 207d 0a20 2020 207d 0a20 2020 7d2c 0a20   }.    }.   },. 
+000045b0: 2020 2257 616b 6555 7050 726f 6365 7373    "WakeUpProcess
+000045c0: 223a 207b 0a20 2020 2022 6172 6773 223a  ": {.    "args":
+000045d0: 207b 0a20 2020 2020 2230 223a 207b 2022   {.     "0": { "
+000045e0: 7479 7065 5f6d 6f64 6966 6965 7222 3a20  type_modifier": 
+000045f0: 226e 227d 0a20 2020 207d 0a20 2020 7d0a  "n"}.    }.   }.
+00004600: 2020 7d2c 0a20 2022 696e 666f 726d 616c    },.  "informal
+00004610: 5f70 726f 746f 636f 6c73 223a 207b 7d2c  _protocols": {},
+00004620: 0a20 2022 7374 7275 6374 7322 3a20 7b0a  .  "structs": {.
+00004630: 2020 2022 5072 6f63 6573 7353 6572 6961     "ProcessSeria
+00004640: 6c4e 756d 6265 7222 3a20 7b0a 2020 2020  lNumber": {.    
+00004650: 2274 7970 6573 7472 223a 2022 7b50 726f  "typestr": "{Pro
+00004660: 6365 7373 5365 7269 616c 4e75 6d62 6572  cessSerialNumber
+00004670: 3d49 497d 222c 0a20 2020 2022 6669 656c  =II}",.    "fiel
+00004680: 646e 616d 6573 223a 205b 0a20 2020 2020  dnames": [.     
+00004690: 2268 6967 684c 6f6e 674f 6650 534e 222c  "highLongOfPSN",
+000046a0: 0a20 2020 2020 226c 6f77 4c6f 6e67 4f66  .     "lowLongOf
+000046b0: 5053 4e22 0a20 2020 205d 0a20 2020 7d2c  PSN".    ].   },
+000046c0: 0a20 2020 224c 6175 6e63 6850 6172 616d  .   "LaunchParam
+000046d0: 426c 6f63 6b52 6563 223a 207b 2022 6967  BlockRec": { "ig
+000046e0: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
+000046f0: 2020 2241 7070 5061 7261 6d65 7465 7273    "AppParameters
+00004700: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00004710: 7275 6520 7d2c 0a20 2020 2249 4344 6972  rue },.   "ICDir
+00004720: 5370 6563 223a 207b 2022 6967 6e6f 7265  Spec": { "ignore
+00004730: 223a 2074 7275 6520 7d2c 0a20 2020 2249  ": true },.   "I
+00004740: 4346 6f6e 7452 6563 6f72 6422 3a20 7b20  CFontRecord": { 
+00004750: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+00004760: 2c0a 2020 2022 4943 4368 6172 5461 626c  ,.   "ICCharTabl
+00004770: 6522 3a20 7b20 2269 676e 6f72 6522 3a20  e": { "ignore": 
+00004780: 7472 7565 207d 2c0a 2020 2022 4943 4170  true },.   "ICAp
+00004790: 7053 7065 6322 3a20 7b20 2269 676e 6f72  pSpec": { "ignor
+000047a0: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+000047b0: 4943 4170 7053 7065 634c 6973 7422 3a20  ICAppSpecList": 
+000047c0: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
+000047d0: 207d 2c0a 2020 2022 4943 4669 6c65 5370   },.   "ICFileSp
+000047e0: 6563 223a 207b 2022 6967 6e6f 7265 223a  ec": { "ignore":
+000047f0: 2074 7275 6520 7d2c 0a20 2020 2249 434d   true },.   "ICM
+00004800: 6170 456e 7472 7922 3a20 7b20 2269 676e  apEntry": { "ign
+00004810: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
+00004820: 2022 4943 5365 7276 6963 6545 6e74 7279   "ICServiceEntry
+00004830: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00004840: 7275 6520 7d2c 0a20 2020 2249 4353 6572  rue },.   "ICSer
+00004850: 7669 6365 7322 3a20 7b20 2269 676e 6f72  vices": { "ignor
+00004860: 6522 3a20 7472 7565 207d 0a20 207d 2c0a  e": true }.  },.
+00004870: 2020 2265 6e75 6d22 3a20 7b0a 2020 2022    "enum": {.   "
+00004880: 6963 5072 6566 4e6f 7446 6f75 6e64 4572  icPrefNotFoundEr
+00004890: 7222 3a20 7b20 2269 676e 6f72 6522 3a20  r": { "ignore": 
+000048a0: 7472 7565 207d 2c0a 2020 2022 6963 5065  true },.   "icPe
+000048b0: 726d 4572 7222 3a20 7b20 2269 676e 6f72  rmErr": { "ignor
 000048c0: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-000048d0: 6b49 4346 696c 6553 7065 6348 6561 6465  kICFileSpecHeade
-000048e0: 7253 697a 6522 3a20 7b20 2269 676e 6f72  rSize": { "ignor
-000048f0: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-00004900: 6b49 6e74 6572 6e65 7445 7665 6e74 436c  kInternetEventCl
-00004910: 6173 7322 3a20 7b20 2269 676e 6f72 6522  ass": { "ignore"
-00004920: 3a20 7472 7565 207d 2c0a 2020 2022 6b41  : true },.   "kA
-00004930: 4547 6574 5552 4c22 3a20 7b20 2269 676e  EGetURL": { "ign
-00004940: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
-00004950: 2022 6b41 4546 6574 6368 5552 4c22 3a20   "kAEFetchURL": 
-00004960: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
-00004970: 207d 2c0a 2020 2022 6b65 7941 4541 7474   },.   "keyAEAtt
-00004980: 6163 6869 6e67 223a 207b 2022 6967 6e6f  aching": { "igno
-00004990: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
-000049a0: 226b 4943 4564 6974 5072 6566 6572 656e  "kICEditPreferen
-000049b0: 6365 4576 656e 7443 6c61 7373 223a 207b  ceEventClass": {
-000049c0: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
-000049d0: 7d2c 0a20 2020 226b 4943 4564 6974 5072  },.   "kICEditPr
-000049e0: 6566 6572 656e 6365 4576 656e 7422 3a20  eferenceEvent": 
-000049f0: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
-00004a00: 207d 2c0a 2020 2022 6b65 7949 4345 6469   },.   "keyICEdi
-00004a10: 7450 7265 6665 7265 6e63 6544 6573 7469  tPreferenceDesti
-00004a20: 6e61 7469 6f6e 223a 207b 2022 6967 6e6f  nation": { "igno
-00004a30: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
-00004a40: 226b 4943 436f 6d70 6f6e 656e 7456 6572  "kICComponentVer
-00004a50: 7369 6f6e 223a 207b 2022 6967 6e6f 7265  sion": { "ignore
-00004a60: 223a 2074 7275 6520 7d2c 0a20 2020 226b  ": true },.   "k
-00004a70: 4943 4e75 6d56 6572 7369 6f6e 223a 207b  ICNumVersion": {
-00004a80: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
-00004a90: 7d2c 0a20 2020 226b 4943 4d61 7046 6978  },.   "kICMapFix
-00004aa0: 6564 4c65 6e67 7468 223a 207b 2022 6967  edLength": { "ig
+000048d0: 6963 5072 6566 4461 7461 4572 7222 3a20  icPrefDataErr": 
+000048e0: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
+000048f0: 207d 2c0a 2020 2022 6963 496e 7465 726e   },.   "icIntern
+00004900: 616c 4572 7222 3a20 7b20 2269 676e 6f72  alErr": { "ignor
+00004910: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+00004920: 6963 5472 756e 6361 7465 6445 7272 223a  icTruncatedErr":
+00004930: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
+00004940: 6520 7d2c 0a20 2020 2269 634e 6f4d 6f72  e },.   "icNoMor
+00004950: 6557 7269 7465 7273 4572 7222 3a20 7b20  eWritersErr": { 
+00004960: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+00004970: 2c0a 2020 2022 6963 4e6f 7468 696e 6754  ,.   "icNothingT
+00004980: 6f4f 7665 7272 6964 6545 7272 223a 207b  oOverrideErr": {
+00004990: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
+000049a0: 7d2c 0a20 2020 2269 634e 6f55 524c 4572  },.   "icNoURLEr
+000049b0: 7222 3a20 7b20 2269 676e 6f72 6522 3a20  r": { "ignore": 
+000049c0: 7472 7565 207d 2c0a 2020 2022 6963 436f  true },.   "icCo
+000049d0: 6e66 6967 4e6f 7446 6f75 6e64 4572 7222  nfigNotFoundErr"
+000049e0: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
+000049f0: 7565 207d 2c0a 2020 2022 6963 436f 6e66  ue },.   "icConf
+00004a00: 6967 496e 6170 7072 6f70 7269 6174 6545  igInappropriateE
+00004a10: 7272 223a 207b 2022 6967 6e6f 7265 223a  rr": { "ignore":
+00004a20: 2074 7275 6520 7d2c 0a20 2020 2269 6350   true },.   "icP
+00004a30: 726f 6669 6c65 4e6f 7446 6f75 6e64 4572  rofileNotFoundEr
+00004a40: 7222 3a20 7b20 2269 676e 6f72 6522 3a20  r": { "ignore": 
+00004a50: 7472 7565 207d 2c0a 2020 2022 6963 546f  true },.   "icTo
+00004a60: 6f4d 616e 7950 726f 6669 6c65 7345 7272  oManyProfilesErr
+00004a70: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00004a80: 7275 6520 7d2c 0a20 2020 226b 4943 436f  rue },.   "kICCo
+00004a90: 6d70 6f6e 656e 7449 6e74 6572 6661 6365  mponentInterface
+00004aa0: 5665 7273 696f 6e30 223a 207b 2022 6967  Version0": { "ig
 00004ab0: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
-00004ac0: 2020 226b 4943 5365 7276 6963 6573 5443    "kICServicesTC
-00004ad0: 5042 6974 223a 207b 2022 6967 6e6f 7265  PBit": { "ignore
-00004ae0: 223a 2074 7275 6520 7d2c 0a20 2020 226b  ": true },.   "k
-00004af0: 4943 5365 7276 6963 6573 5544 5042 6974  ICServicesUDPBit
-00004b00: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00004b10: 7275 6520 7d2c 0a20 2020 226b 4943 5365  rue },.   "kICSe
-00004b20: 7276 6963 6573 5443 504d 6173 6b22 3a20  rvicesTCPMask": 
-00004b30: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
-00004b40: 207d 2c0a 2020 2022 6b49 4353 6572 7669   },.   "kICServi
-00004b50: 6365 7355 4450 4d61 736b 223a 207b 2022  cesUDPMask": { "
-00004b60: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-00004b70: 0a20 2020 226b 4943 4d61 7042 696e 6172  .   "kICMapBinar
-00004b80: 7942 6974 223a 207b 2022 6967 6e6f 7265  yBit": { "ignore
-00004b90: 223a 2074 7275 6520 7d2c 0a20 2020 226b  ": true },.   "k
-00004ba0: 4943 4d61 7052 6573 6f75 7263 6546 6f72  ICMapResourceFor
-00004bb0: 6b42 6974 223a 207b 2022 6967 6e6f 7265  kBit": { "ignore
-00004bc0: 223a 2074 7275 6520 7d2c 0a20 2020 226b  ": true },.   "k
-00004bd0: 4943 4d61 7044 6174 6146 6f72 6b42 6974  ICMapDataForkBit
-00004be0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00004bf0: 7275 6520 7d2c 0a20 2020 226b 4943 4d61  rue },.   "kICMa
-00004c00: 7050 6f73 7442 6974 223a 207b 2022 6967  pPostBit": { "ig
-00004c10: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
-00004c20: 2020 226b 4943 4d61 704e 6f74 496e 636f    "kICMapNotInco
-00004c30: 6d69 6e67 4269 7422 3a20 7b20 2269 676e  mingBit": { "ign
-00004c40: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
-00004c50: 2022 6b49 434d 6170 4e6f 744f 7574 676f   "kICMapNotOutgo
-00004c60: 696e 6742 6974 223a 207b 2022 6967 6e6f  ingBit": { "igno
-00004c70: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
-00004c80: 226b 4943 4d61 7042 696e 6172 794d 6173  "kICMapBinaryMas
-00004c90: 6b22 3a20 7b20 2269 676e 6f72 6522 3a20  k": { "ignore": 
-00004ca0: 7472 7565 207d 2c0a 2020 2022 6b49 434d  true },.   "kICM
-00004cb0: 6170 5265 736f 7572 6365 466f 726b 4d61  apResourceForkMa
-00004cc0: 736b 223a 207b 2022 6967 6e6f 7265 223a  sk": { "ignore":
-00004cd0: 2074 7275 6520 7d2c 0a20 2020 226b 4943   true },.   "kIC
-00004ce0: 4d61 7044 6174 6146 6f72 6b4d 6173 6b22  MapDataForkMask"
-00004cf0: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-00004d00: 7565 207d 2c0a 2020 2022 6b49 434d 6170  ue },.   "kICMap
-00004d10: 506f 7374 4d61 736b 223a 207b 2022 6967  PostMask": { "ig
-00004d20: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
-00004d30: 2020 226b 4943 4d61 704e 6f74 496e 636f    "kICMapNotInco
-00004d40: 6d69 6e67 4d61 736b 223a 207b 2022 6967  mingMask": { "ig
-00004d50: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
-00004d60: 2020 226b 4943 4d61 704e 6f74 4f75 7467    "kICMapNotOutg
-00004d70: 6f69 6e67 4d61 736b 223a 207b 2022 6967  oingMask": { "ig
-00004d80: 6e6f 7265 223a 2074 7275 6520 7d0a 2020  nore": true }.  
-00004d90: 7d2c 0a20 2022 6c69 7465 7261 6c73 223a  },.  "literals":
-00004da0: 207b 0a20 2020 226b 4943 4172 6368 6965   {.   "kICArchie
-00004db0: 416c 6c22 3a20 7b20 2269 676e 6f72 6522  All": { "ignore"
-00004dc0: 3a20 7472 7565 207d 2c0a 2020 2022 6b49  : true },.   "kI
-00004dd0: 4341 7263 6869 6550 7265 6665 7272 6564  CArchiePreferred
-00004de0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00004df0: 7275 6520 7d2c 0a20 2020 226b 4943 4368  rue },.   "kICCh
-00004e00: 6172 6163 7465 7253 6574 223a 207b 2022  aracterSet": { "
-00004e10: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-00004e20: 0a20 2020 226b 4943 446f 6375 6d65 6e74  .   "kICDocument
-00004e30: 466f 6e74 223a 207b 2022 6967 6e6f 7265  Font": { "ignore
-00004e40: 223a 2074 7275 6520 7d2c 0a20 2020 226b  ": true },.   "k
-00004e50: 4943 446f 776e 6c6f 6164 466f 6c64 6572  ICDownloadFolder
-00004e60: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00004e70: 7275 6520 7d2c 0a20 2020 226b 4943 456d  rue },.   "kICEm
-00004e80: 6169 6c22 3a20 7b20 2269 676e 6f72 6522  ail": { "ignore"
-00004e90: 3a20 7472 7565 207d 2c0a 2020 2022 6b49  : true },.   "kI
-00004ea0: 4346 5450 486f 7374 223a 207b 2022 6967  CFTPHost": { "ig
-00004eb0: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
-00004ec0: 2020 226b 4943 4654 5050 726f 7879 4163    "kICFTPProxyAc
-00004ed0: 636f 756e 7422 3a20 7b20 2269 676e 6f72  count": { "ignor
-00004ee0: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-00004ef0: 6b49 4346 5450 5072 6f78 7948 6f73 7422  kICFTPProxyHost"
-00004f00: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-00004f10: 7565 207d 2c0a 2020 2022 6b49 4346 5450  ue },.   "kICFTP
-00004f20: 5072 6f78 7950 6173 7377 6f72 6422 3a20  ProxyPassword": 
-00004f30: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
-00004f40: 207d 2c0a 2020 2022 6b49 4346 5450 5072   },.   "kICFTPPr
-00004f50: 6f78 7955 7365 7222 3a20 7b20 2269 676e  oxyUser": { "ign
-00004f60: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
-00004f70: 2022 6b49 4346 696e 6765 7248 6f73 7422   "kICFingerHost"
-00004f80: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-00004f90: 7565 207d 2c0a 2020 2022 6b49 4347 6f70  ue },.   "kICGop
-00004fa0: 6865 7248 6f73 7422 3a20 7b20 2269 676e  herHost": { "ign
-00004fb0: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
-00004fc0: 2022 6b49 4347 6f70 6865 7250 726f 7879   "kICGopherProxy
-00004fd0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00004fe0: 7275 6520 7d2c 0a20 2020 226b 4943 4854  rue },.   "kICHT
-00004ff0: 5450 5072 6f78 7948 6f73 7422 3a20 7b20  TPProxyHost": { 
-00005000: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
-00005010: 2c0a 2020 2022 6b49 4348 656c 7065 7222  ,.   "kICHelper"
-00005020: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-00005030: 7565 207d 2c0a 2020 2022 6b49 4348 656c  ue },.   "kICHel
-00005040: 7065 7244 6573 6322 3a20 7b20 2269 676e  perDesc": { "ign
-00005050: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
-00005060: 2022 6b49 4348 656c 7065 724c 6973 7422   "kICHelperList"
-00005070: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-00005080: 7565 207d 2c0a 2020 2022 6b49 4349 5243  ue },.   "kICIRC
-00005090: 486f 7374 223a 207b 2022 6967 6e6f 7265  Host": { "ignore
-000050a0: 223a 2074 7275 6520 7d2c 0a20 2020 226b  ": true },.   "k
-000050b0: 4943 496e 666f 4d61 6341 6c6c 223a 207b  ICInfoMacAll": {
-000050c0: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
-000050d0: 7d2c 0a20 2020 226b 4943 496e 666f 4d61  },.   "kICInfoMa
-000050e0: 6350 7265 6665 7272 6564 223a 207b 2022  cPreferred": { "
+00004ac0: 2020 226b 4943 436f 6d70 6f6e 656e 7449    "kICComponentI
+00004ad0: 6e74 6572 6661 6365 5665 7273 696f 6e31  nterfaceVersion1
+00004ae0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00004af0: 7275 6520 7d2c 0a20 2020 226b 4943 436f  rue },.   "kICCo
+00004b00: 6d70 6f6e 656e 7449 6e74 6572 6661 6365  mponentInterface
+00004b10: 5665 7273 696f 6e32 223a 207b 2022 6967  Version2": { "ig
+00004b20: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
+00004b30: 2020 226b 4943 436f 6d70 6f6e 656e 7449    "kICComponentI
+00004b40: 6e74 6572 6661 6365 5665 7273 696f 6e33  nterfaceVersion3
+00004b50: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00004b60: 7275 6520 7d2c 0a20 2020 226b 4943 436f  rue },.   "kICCo
+00004b70: 6d70 6f6e 656e 7449 6e74 6572 6661 6365  mponentInterface
+00004b80: 5665 7273 696f 6e34 223a 207b 2022 6967  Version4": { "ig
+00004b90: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
+00004ba0: 2020 226b 4943 436f 6d70 6f6e 656e 7449    "kICComponentI
+00004bb0: 6e74 6572 6661 6365 5665 7273 696f 6e22  nterfaceVersion"
+00004bc0: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
+00004bd0: 7565 207d 2c0a 2020 2022 6b49 4341 7474  ue },.   "kICAtt
+00004be0: 724c 6f63 6b65 6442 6974 223a 207b 2022  rLockedBit": { "
+00004bf0: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
+00004c00: 0a20 2020 226b 4943 4174 7472 566f 6c61  .   "kICAttrVola
+00004c10: 7469 6c65 4269 7422 3a20 7b20 2269 676e  tileBit": { "ign
+00004c20: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
+00004c30: 2022 6b49 4341 7474 724e 6f43 6861 6e67   "kICAttrNoChang
+00004c40: 6522 3a20 7b20 2269 676e 6f72 6522 3a20  e": { "ignore": 
+00004c50: 7472 7565 207d 2c0a 2020 2022 6b49 4341  true },.   "kICA
+00004c60: 7474 724c 6f63 6b65 644d 6173 6b22 3a20  ttrLockedMask": 
+00004c70: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
+00004c80: 207d 2c0a 2020 2022 6b49 4341 7474 7256   },.   "kICAttrV
+00004c90: 6f6c 6174 696c 654d 6173 6b22 3a20 7b20  olatileMask": { 
+00004ca0: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+00004cb0: 2c0a 2020 2022 6963 4e6f 5065 726d 223a  ,.   "icNoPerm":
+00004cc0: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
+00004cd0: 6520 7d2c 0a20 2020 2269 6352 6561 644f  e },.   "icReadO
+00004ce0: 6e6c 7950 6572 6d22 3a20 7b20 2269 676e  nlyPerm": { "ign
+00004cf0: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
+00004d00: 2022 6963 5265 6164 5772 6974 6550 6572   "icReadWritePer
+00004d10: 6d22 3a20 7b20 2269 676e 6f72 6522 3a20  m": { "ignore": 
+00004d20: 7472 7565 207d 2c0a 2020 2022 6b49 434e  true },.   "kICN
+00004d30: 696c 5072 6f66 696c 6549 4422 3a20 7b20  ilProfileID": { 
+00004d40: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+00004d50: 2c0a 2020 2022 6b49 434e 6f55 7365 7249  ,.   "kICNoUserI
+00004d60: 6e74 6572 6163 7469 6f6e 4269 7422 3a20  nteractionBit": 
+00004d70: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
+00004d80: 207d 2c0a 2020 2022 6b49 434e 6f55 7365   },.   "kICNoUse
+00004d90: 7249 6e74 6572 6163 7469 6f6e 4d61 736b  rInteractionMask
+00004da0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00004db0: 7275 6520 7d2c 0a20 2020 226b 4943 4669  rue },.   "kICFi
+00004dc0: 6c65 5479 7065 223a 207b 2022 6967 6e6f  leType": { "igno
+00004dd0: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
+00004de0: 226b 4943 4372 6561 746f 7222 3a20 7b20  "kICCreator": { 
+00004df0: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+00004e00: 2c0a 2020 2022 6b49 4346 696c 6553 7065  ,.   "kICFileSpe
+00004e10: 6348 6561 6465 7253 697a 6522 3a20 7b20  cHeaderSize": { 
+00004e20: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+00004e30: 2c0a 2020 2022 6b49 6e74 6572 6e65 7445  ,.   "kInternetE
+00004e40: 7665 6e74 436c 6173 7322 3a20 7b20 2269  ventClass": { "i
+00004e50: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
+00004e60: 2020 2022 6b41 4547 6574 5552 4c22 3a20     "kAEGetURL": 
+00004e70: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
+00004e80: 207d 2c0a 2020 2022 6b41 4546 6574 6368   },.   "kAEFetch
+00004e90: 5552 4c22 3a20 7b20 2269 676e 6f72 6522  URL": { "ignore"
+00004ea0: 3a20 7472 7565 207d 2c0a 2020 2022 6b65  : true },.   "ke
+00004eb0: 7941 4541 7474 6163 6869 6e67 223a 207b  yAEAttaching": {
+00004ec0: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
+00004ed0: 7d2c 0a20 2020 226b 4943 4564 6974 5072  },.   "kICEditPr
+00004ee0: 6566 6572 656e 6365 4576 656e 7443 6c61  eferenceEventCla
+00004ef0: 7373 223a 207b 2022 6967 6e6f 7265 223a  ss": { "ignore":
+00004f00: 2074 7275 6520 7d2c 0a20 2020 226b 4943   true },.   "kIC
+00004f10: 4564 6974 5072 6566 6572 656e 6365 4576  EditPreferenceEv
+00004f20: 656e 7422 3a20 7b20 2269 676e 6f72 6522  ent": { "ignore"
+00004f30: 3a20 7472 7565 207d 2c0a 2020 2022 6b65  : true },.   "ke
+00004f40: 7949 4345 6469 7450 7265 6665 7265 6e63  yICEditPreferenc
+00004f50: 6544 6573 7469 6e61 7469 6f6e 223a 207b  eDestination": {
+00004f60: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
+00004f70: 7d2c 0a20 2020 226b 4943 436f 6d70 6f6e  },.   "kICCompon
+00004f80: 656e 7456 6572 7369 6f6e 223a 207b 2022  entVersion": { "
+00004f90: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
+00004fa0: 0a20 2020 226b 4943 4e75 6d56 6572 7369  .   "kICNumVersi
+00004fb0: 6f6e 223a 207b 2022 6967 6e6f 7265 223a  on": { "ignore":
+00004fc0: 2074 7275 6520 7d2c 0a20 2020 226b 4943   true },.   "kIC
+00004fd0: 4d61 7046 6978 6564 4c65 6e67 7468 223a  MapFixedLength":
+00004fe0: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
+00004ff0: 6520 7d2c 0a20 2020 226b 4943 5365 7276  e },.   "kICServ
+00005000: 6963 6573 5443 5042 6974 223a 207b 2022  icesTCPBit": { "
+00005010: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
+00005020: 0a20 2020 226b 4943 5365 7276 6963 6573  .   "kICServices
+00005030: 5544 5042 6974 223a 207b 2022 6967 6e6f  UDPBit": { "igno
+00005040: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
+00005050: 226b 4943 5365 7276 6963 6573 5443 504d  "kICServicesTCPM
+00005060: 6173 6b22 3a20 7b20 2269 676e 6f72 6522  ask": { "ignore"
+00005070: 3a20 7472 7565 207d 2c0a 2020 2022 6b49  : true },.   "kI
+00005080: 4353 6572 7669 6365 7355 4450 4d61 736b  CServicesUDPMask
+00005090: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+000050a0: 7275 6520 7d2c 0a20 2020 226b 4943 4d61  rue },.   "kICMa
+000050b0: 7042 696e 6172 7942 6974 223a 207b 2022  pBinaryBit": { "
+000050c0: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
+000050d0: 0a20 2020 226b 4943 4d61 7052 6573 6f75  .   "kICMapResou
+000050e0: 7263 6546 6f72 6b42 6974 223a 207b 2022  rceForkBit": { "
 000050f0: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-00005100: 0a20 2020 226b 4943 4c44 4150 5365 6172  .   "kICLDAPSear
-00005110: 6368 6261 7365 223a 207b 2022 6967 6e6f  chbase": { "igno
+00005100: 0a20 2020 226b 4943 4d61 7044 6174 6146  .   "kICMapDataF
+00005110: 6f72 6b42 6974 223a 207b 2022 6967 6e6f  orkBit": { "igno
 00005120: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
-00005130: 226b 4943 4c44 4150 5365 7276 6572 223a  "kICLDAPServer":
+00005130: 226b 4943 4d61 7050 6f73 7442 6974 223a  "kICMapPostBit":
 00005140: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
-00005150: 6520 7d2c 0a20 2020 226b 4943 4c69 7374  e },.   "kICList
-00005160: 466f 6e74 223a 207b 2022 6967 6e6f 7265  Font": { "ignore
-00005170: 223a 2074 7275 6520 7d2c 0a20 2020 226b  ": true },.   "k
-00005180: 4943 4d61 6353 6561 7263 6848 6f73 7422  ICMacSearchHost"
-00005190: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-000051a0: 7565 207d 2c0a 2020 2022 6b49 434d 6169  ue },.   "kICMai
-000051b0: 6c41 6363 6f75 6e74 223a 207b 2022 6967  lAccount": { "ig
-000051c0: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
-000051d0: 2020 226b 4943 4d61 696c 4865 6164 6572    "kICMailHeader
-000051e0: 7322 3a20 7b20 2269 676e 6f72 6522 3a20  s": { "ignore": 
-000051f0: 7472 7565 207d 2c0a 2020 2022 6b49 434d  true },.   "kICM
-00005200: 6169 6c50 6173 7377 6f72 6422 3a20 7b20  ailPassword": { 
-00005210: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
-00005220: 2c0a 2020 2022 6b49 434d 6170 7069 6e67  ,.   "kICMapping
-00005230: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00005240: 7275 6520 7d2c 0a20 2020 226b 4943 4e4e  rue },.   "kICNN
-00005250: 5450 486f 7374 223a 207b 2022 6967 6e6f  TPHost": { "igno
-00005260: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
-00005270: 226b 4943 4e54 5048 6f73 7422 3a20 7b20  "kICNTPHost": { 
-00005280: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
-00005290: 2c0a 2020 2022 6b49 434e 6577 4d61 696c  ,.   "kICNewMail
-000052a0: 4469 616c 6f67 223a 207b 2022 6967 6e6f  Dialog": { "igno
-000052b0: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
-000052c0: 226b 4943 4e65 774d 6169 6c46 6c61 7368  "kICNewMailFlash
-000052d0: 4963 6f6e 223a 207b 2022 6967 6e6f 7265  Icon": { "ignore
-000052e0: 223a 2074 7275 6520 7d2c 0a20 2020 226b  ": true },.   "k
-000052f0: 4943 4e65 774d 6169 6c50 6c61 7953 6f75  ICNewMailPlaySou
-00005300: 6e64 223a 207b 2022 6967 6e6f 7265 223a  nd": { "ignore":
-00005310: 2074 7275 6520 7d2c 0a20 2020 226b 4943   true },.   "kIC
-00005320: 4e65 774d 6169 6c53 6f75 6e64 4e61 6d65  NewMailSoundName
-00005330: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00005340: 7275 6520 7d2c 0a20 2020 226b 4943 4e65  rue },.   "kICNe
-00005350: 7773 4175 7468 5061 7373 776f 7264 223a  wsAuthPassword":
-00005360: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
-00005370: 6520 7d2c 0a20 2020 226b 4943 4e65 7773  e },.   "kICNews
-00005380: 4175 7468 5573 6572 6e61 6d65 223a 207b  AuthUsername": {
-00005390: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
-000053a0: 7d2c 0a20 2020 226b 4943 4e65 7773 4865  },.   "kICNewsHe
-000053b0: 6164 6572 7322 3a20 7b20 2269 676e 6f72  aders": { "ignor
-000053c0: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-000053d0: 6b49 434e 6f50 726f 7879 446f 6d61 696e  kICNoProxyDomain
-000053e0: 7322 3a20 7b20 2269 676e 6f72 6522 3a20  s": { "ignore": 
-000053f0: 7472 7565 207d 2c0a 2020 2022 6b49 434f  true },.   "kICO
-00005400: 7267 616e 697a 6174 696f 6e22 3a20 7b20  rganization": { 
+00005150: 6520 7d2c 0a20 2020 226b 4943 4d61 704e  e },.   "kICMapN
+00005160: 6f74 496e 636f 6d69 6e67 4269 7422 3a20  otIncomingBit": 
+00005170: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
+00005180: 207d 2c0a 2020 2022 6b49 434d 6170 4e6f   },.   "kICMapNo
+00005190: 744f 7574 676f 696e 6742 6974 223a 207b  tOutgoingBit": {
+000051a0: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
+000051b0: 7d2c 0a20 2020 226b 4943 4d61 7042 696e  },.   "kICMapBin
+000051c0: 6172 794d 6173 6b22 3a20 7b20 2269 676e  aryMask": { "ign
+000051d0: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
+000051e0: 2022 6b49 434d 6170 5265 736f 7572 6365   "kICMapResource
+000051f0: 466f 726b 4d61 736b 223a 207b 2022 6967  ForkMask": { "ig
+00005200: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
+00005210: 2020 226b 4943 4d61 7044 6174 6146 6f72    "kICMapDataFor
+00005220: 6b4d 6173 6b22 3a20 7b20 2269 676e 6f72  kMask": { "ignor
+00005230: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+00005240: 6b49 434d 6170 506f 7374 4d61 736b 223a  kICMapPostMask":
+00005250: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
+00005260: 6520 7d2c 0a20 2020 226b 4943 4d61 704e  e },.   "kICMapN
+00005270: 6f74 496e 636f 6d69 6e67 4d61 736b 223a  otIncomingMask":
+00005280: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
+00005290: 6520 7d2c 0a20 2020 226b 4943 4d61 704e  e },.   "kICMapN
+000052a0: 6f74 4f75 7467 6f69 6e67 4d61 736b 223a  otOutgoingMask":
+000052b0: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
+000052c0: 6520 7d0a 2020 7d2c 0a20 2022 6c69 7465  e }.  },.  "lite
+000052d0: 7261 6c73 223a 207b 0a20 2020 226b 4943  rals": {.   "kIC
+000052e0: 4172 6368 6965 416c 6c22 3a20 7b20 2269  ArchieAll": { "i
+000052f0: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
+00005300: 2020 2022 6b49 4341 7263 6869 6550 7265     "kICArchiePre
+00005310: 6665 7272 6564 223a 207b 2022 6967 6e6f  ferred": { "igno
+00005320: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
+00005330: 226b 4943 4368 6172 6163 7465 7253 6574  "kICCharacterSet
+00005340: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00005350: 7275 6520 7d2c 0a20 2020 226b 4943 446f  rue },.   "kICDo
+00005360: 6375 6d65 6e74 466f 6e74 223a 207b 2022  cumentFont": { "
+00005370: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
+00005380: 0a20 2020 226b 4943 446f 776e 6c6f 6164  .   "kICDownload
+00005390: 466f 6c64 6572 223a 207b 2022 6967 6e6f  Folder": { "igno
+000053a0: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
+000053b0: 226b 4943 456d 6169 6c22 3a20 7b20 2269  "kICEmail": { "i
+000053c0: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
+000053d0: 2020 2022 6b49 4346 5450 486f 7374 223a     "kICFTPHost":
+000053e0: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
+000053f0: 6520 7d2c 0a20 2020 226b 4943 4654 5050  e },.   "kICFTPP
+00005400: 726f 7879 4163 636f 756e 7422 3a20 7b20  roxyAccount": { 
 00005410: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
-00005420: 2c0a 2020 2022 6b49 4350 6848 6f73 7422  ,.   "kICPhHost"
-00005430: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-00005440: 7565 207d 2c0a 2020 2022 6b49 4350 6c61  ue },.   "kICPla
-00005450: 6e22 3a20 7b20 2269 676e 6f72 6522 3a20  n": { "ignore": 
-00005460: 7472 7565 207d 2c0a 2020 2022 6b49 4350  true },.   "kICP
-00005470: 7269 6e74 6572 466f 6e74 223a 207b 2022  rinterFont": { "
-00005480: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-00005490: 0a20 2020 226b 4943 5175 6f74 696e 6753  .   "kICQuotingS
-000054a0: 7472 696e 6722 3a20 7b20 2269 676e 6f72  tring": { "ignor
-000054b0: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-000054c0: 6b49 4352 5453 5050 726f 7879 486f 7374  kICRTSPProxyHost
-000054d0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-000054e0: 7275 6520 7d2c 0a20 2020 226b 4943 5265  rue },.   "kICRe
-000054f0: 616c 4e61 6d65 223a 207b 2022 6967 6e6f  alName": { "igno
-00005500: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
-00005510: 226b 4943 5265 7365 7276 6564 4b65 7922  "kICReservedKey"
-00005520: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-00005530: 7565 207d 2c0a 2020 2022 6b49 4353 4d54  ue },.   "kICSMT
-00005540: 5048 6f73 7422 3a20 7b20 2269 676e 6f72  PHost": { "ignor
-00005550: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-00005560: 6b49 4353 6372 6565 6e46 6f6e 7422 3a20  kICScreenFont": 
-00005570: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
-00005580: 207d 2c0a 2020 2022 6b49 4353 6572 7669   },.   "kICServi
-00005590: 6365 7322 3a20 7b20 2269 676e 6f72 6522  ces": { "ignore"
-000055a0: 3a20 7472 7565 207d 2c0a 2020 2022 6b49  : true },.   "kI
-000055b0: 4353 6967 6e61 7475 7265 223a 207b 2022  CSignature": { "
-000055c0: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-000055d0: 0a20 2020 226b 4943 536e 6169 6c4d 6169  .   "kICSnailMai
-000055e0: 6c41 6464 7265 7373 223a 207b 2022 6967  lAddress": { "ig
-000055f0: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
-00005600: 2020 226b 4943 536f 636b 7348 6f73 7422    "kICSocksHost"
-00005610: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
-00005620: 7565 207d 2c0a 2020 2022 6b49 4354 656c  ue },.   "kICTel
-00005630: 6e65 7448 6f73 7422 3a20 7b20 2269 676e  netHost": { "ign
-00005640: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
-00005650: 2022 6b49 4355 4d69 6368 416c 6c22 3a20   "kICUMichAll": 
-00005660: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
-00005670: 207d 2c0a 2020 2022 6b49 4355 4d69 6368   },.   "kICUMich
-00005680: 5072 6566 6572 7265 6422 3a20 7b20 2269  Preferred": { "i
-00005690: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
-000056a0: 2020 2022 6b49 4355 7365 4654 5050 726f     "kICUseFTPPro
-000056b0: 7879 223a 207b 2022 6967 6e6f 7265 223a  xy": { "ignore":
-000056c0: 2074 7275 6520 7d2c 0a20 2020 226b 4943   true },.   "kIC
-000056d0: 5573 6547 6f70 6865 7250 726f 7879 223a  UseGopherProxy":
-000056e0: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
-000056f0: 6520 7d2c 0a20 2020 226b 4943 5573 6548  e },.   "kICUseH
-00005700: 5454 5050 726f 7879 223a 207b 2022 6967  TTPProxy": { "ig
-00005710: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
-00005720: 2020 226b 4943 5573 6550 6173 7369 7665    "kICUsePassive
-00005730: 4654 5022 3a20 7b20 2269 676e 6f72 6522  FTP": { "ignore"
-00005740: 3a20 7472 7565 207d 2c0a 2020 2022 6b49  : true },.   "kI
-00005750: 4355 7365 5254 5350 5072 6f78 7922 3a20  CUseRTSPProxy": 
-00005760: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
-00005770: 207d 2c0a 2020 2022 6b49 4355 7365 536f   },.   "kICUseSo
-00005780: 636b 7322 3a20 7b20 2269 676e 6f72 6522  cks": { "ignore"
-00005790: 3a20 7472 7565 207d 2c0a 2020 2022 6b49  : true },.   "kI
-000057a0: 4357 4149 5347 6174 6577 6179 223a 207b  CWAISGateway": {
-000057b0: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
-000057c0: 7d2c 0a20 2020 226b 4943 5757 5748 6f6d  },.   "kICWWWHom
-000057d0: 6550 6167 6522 3a20 7b20 2269 676e 6f72  ePage": { "ignor
-000057e0: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-000057f0: 6b49 4357 6562 4261 636b 6772 6f75 6e64  kICWebBackground
-00005800: 436f 6c6f 7572 223a 207b 2022 6967 6e6f  Colour": { "igno
-00005810: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
-00005820: 226b 4943 5765 6252 6561 6443 6f6c 6f72  "kICWebReadColor
-00005830: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00005840: 7275 6520 7d2c 0a20 2020 226b 4943 5765  rue },.   "kICWe
-00005850: 6253 6561 7263 6850 6167 6550 7265 6673  bSearchPagePrefs
-00005860: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
-00005870: 7275 6520 7d2c 0a20 2020 226b 4943 5765  rue },.   "kICWe
-00005880: 6254 6578 7443 6f6c 6f72 223a 207b 2022  bTextColor": { "
-00005890: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
-000058a0: 0a20 2020 226b 4943 5765 6255 6e64 6572  .   "kICWebUnder
-000058b0: 6c69 6e65 4c69 6e6b 7322 3a20 7b20 2269  lineLinks": { "i
-000058c0: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
-000058d0: 2020 2022 6b49 4357 6562 556e 7265 6164     "kICWebUnread
-000058e0: 436f 6c6f 7222 3a20 7b20 2269 676e 6f72  Color": { "ignor
-000058f0: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
-00005900: 6b49 4357 686f 6973 486f 7374 223a 207b  kICWhoisHost": {
-00005910: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
-00005920: 7d0a 2020 7d2c 0a20 2022 6366 7479 7065  }.  },.  "cftype
-00005930: 7322 3a20 7b0a 2020 2022 4158 5465 7874  s": {.   "AXText
-00005940: 4d61 726b 6572 5261 6e67 6552 6566 223a  MarkerRangeRef":
-00005950: 207b 0a20 2020 2022 6765 7474 7970 6569   {.    "gettypei
-00005960: 645f 6675 6e63 223a 2022 4158 5465 7874  d_func": "AXText
-00005970: 4d61 726b 6572 5261 6e67 6547 6574 5479  MarkerRangeGetTy
-00005980: 7065 4944 222c 0a20 2020 2022 7479 7065  peID",.    "type
-00005990: 7374 7222 3a20 225e 7b5f 5f41 5854 6578  str": "^{__AXTex
-000059a0: 744d 6172 6b65 7252 616e 6765 3d7d 220a  tMarkerRange=}".
-000059b0: 2020 207d 2c0a 2020 2022 4158 5465 7874     },.   "AXText
-000059c0: 4d61 726b 6572 5265 6622 3a20 7b0a 2020  MarkerRef": {.  
-000059d0: 2020 2267 6574 7479 7065 6964 5f66 756e    "gettypeid_fun
-000059e0: 6322 3a20 2241 5854 6578 744d 6172 6b65  c": "AXTextMarke
-000059f0: 7247 6574 5479 7065 4944 222c 0a20 2020  rGetTypeID",.   
-00005a00: 2022 7479 7065 7374 7222 3a20 225e 7b5f   "typestr": "^{_
-00005a10: 5f41 5854 6578 744d 6172 6b65 723d 7d22  _AXTextMarker=}"
-00005a20: 0a20 2020 7d2c 0a20 2020 2241 584f 6273  .   },.   "AXObs
-00005a30: 6572 7665 7252 6566 223a 207b 0a20 2020  erverRef": {.   
-00005a40: 2022 6765 7474 7970 6569 645f 6675 6e63   "gettypeid_func
-00005a50: 223a 2022 4158 4f62 7365 7276 6572 4765  ": "AXObserverGe
-00005a60: 7454 7970 6549 4422 2c0a 2020 2020 2274  tTypeID",.    "t
-00005a70: 7970 6573 7472 223a 2022 5e7b 5f5f 4158  ypestr": "^{__AX
-00005a80: 4f62 7365 7276 6572 3d7d 220a 2020 207d  Observer=}".   }
-00005a90: 2c0a 2020 2022 4158 5549 456c 656d 656e  ,.   "AXUIElemen
-00005aa0: 7452 6566 223a 207b 0a20 2020 2022 6765  tRef": {.    "ge
-00005ab0: 7474 7970 6569 645f 6675 6e63 223a 2022  ttypeid_func": "
-00005ac0: 4158 5549 456c 656d 656e 7447 6574 5479  AXUIElementGetTy
-00005ad0: 7065 4944 222c 0a20 2020 2022 7479 7065  peID",.    "type
-00005ae0: 7374 7222 3a20 225e 7b5f 5f41 5855 4945  str": "^{__AXUIE
-00005af0: 6c65 6d65 6e74 3d7d 220a 2020 207d 2c0a  lement=}".   },.
-00005b00: 2020 2022 4158 5661 6c75 6552 6566 223a     "AXValueRef":
-00005b10: 207b 0a20 2020 2022 6765 7474 7970 6569   {.    "gettypei
-00005b20: 645f 6675 6e63 223a 2022 4158 5661 6c75  d_func": "AXValu
-00005b30: 6547 6574 5479 7065 4944 222c 0a20 2020  eGetTypeID",.   
-00005b40: 2022 7479 7065 7374 7222 3a20 225e 7b5f   "typestr": "^{_
-00005b50: 5f41 5856 616c 7565 3d7d 220a 2020 207d  _AXValue=}".   }
-00005b60: 2c0a 2020 2022 4849 5368 6170 6552 6566  ,.   "HIShapeRef
-00005b70: 223a 207b 0a20 2020 2022 6765 7474 7970  ": {.    "gettyp
-00005b80: 6569 645f 6675 6e63 223a 2022 4849 5368  eid_func": "HISh
-00005b90: 6170 6547 6574 5479 7065 4944 222c 0a20  apeGetTypeID",. 
-00005ba0: 2020 2022 7479 7065 7374 7222 3a20 225e     "typestr": "^
-00005bb0: 7b5f 5f48 4953 6861 7065 3d7d 220a 2020  {__HIShape=}".  
-00005bc0: 207d 2c0a 2020 2022 5472 616e 736c 6174   },.   "Translat
-00005bd0: 696f 6e52 6566 223a 207b 0a20 2020 2022  ionRef": {.    "
-00005be0: 6765 7474 7970 6569 645f 6675 6e63 223a  gettypeid_func":
-00005bf0: 2022 5472 616e 736c 6174 696f 6e47 6574   "TranslationGet
-00005c00: 5479 7065 4944 222c 0a20 2020 2022 7479  TypeID",.    "ty
-00005c10: 7065 7374 7222 3a20 225e 7b4f 7061 7175  pestr": "^{Opaqu
-00005c20: 6554 7261 6e73 6c61 7469 6f6e 5265 663d  eTranslationRef=
-00005c30: 7d22 0a20 2020 7d0a 2020 7d0a 207d 0a7d  }".   }.  }. }.}
-00005c40: 0a                                       .
+00005420: 2c0a 2020 2022 6b49 4346 5450 5072 6f78  ,.   "kICFTPProx
+00005430: 7948 6f73 7422 3a20 7b20 2269 676e 6f72  yHost": { "ignor
+00005440: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+00005450: 6b49 4346 5450 5072 6f78 7950 6173 7377  kICFTPProxyPassw
+00005460: 6f72 6422 3a20 7b20 2269 676e 6f72 6522  ord": { "ignore"
+00005470: 3a20 7472 7565 207d 2c0a 2020 2022 6b49  : true },.   "kI
+00005480: 4346 5450 5072 6f78 7955 7365 7222 3a20  CFTPProxyUser": 
+00005490: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
+000054a0: 207d 2c0a 2020 2022 6b49 4346 696e 6765   },.   "kICFinge
+000054b0: 7248 6f73 7422 3a20 7b20 2269 676e 6f72  rHost": { "ignor
+000054c0: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+000054d0: 6b49 4347 6f70 6865 7248 6f73 7422 3a20  kICGopherHost": 
+000054e0: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
+000054f0: 207d 2c0a 2020 2022 6b49 4347 6f70 6865   },.   "kICGophe
+00005500: 7250 726f 7879 223a 207b 2022 6967 6e6f  rProxy": { "igno
+00005510: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
+00005520: 226b 4943 4854 5450 5072 6f78 7948 6f73  "kICHTTPProxyHos
+00005530: 7422 3a20 7b20 2269 676e 6f72 6522 3a20  t": { "ignore": 
+00005540: 7472 7565 207d 2c0a 2020 2022 6b49 4348  true },.   "kICH
+00005550: 656c 7065 7222 3a20 7b20 2269 676e 6f72  elper": { "ignor
+00005560: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+00005570: 6b49 4348 656c 7065 7244 6573 6322 3a20  kICHelperDesc": 
+00005580: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
+00005590: 207d 2c0a 2020 2022 6b49 4348 656c 7065   },.   "kICHelpe
+000055a0: 724c 6973 7422 3a20 7b20 2269 676e 6f72  rList": { "ignor
+000055b0: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+000055c0: 6b49 4349 5243 486f 7374 223a 207b 2022  kICIRCHost": { "
+000055d0: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
+000055e0: 0a20 2020 226b 4943 496e 666f 4d61 6341  .   "kICInfoMacA
+000055f0: 6c6c 223a 207b 2022 6967 6e6f 7265 223a  ll": { "ignore":
+00005600: 2074 7275 6520 7d2c 0a20 2020 226b 4943   true },.   "kIC
+00005610: 496e 666f 4d61 6350 7265 6665 7272 6564  InfoMacPreferred
+00005620: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00005630: 7275 6520 7d2c 0a20 2020 226b 4943 4c44  rue },.   "kICLD
+00005640: 4150 5365 6172 6368 6261 7365 223a 207b  APSearchbase": {
+00005650: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
+00005660: 7d2c 0a20 2020 226b 4943 4c44 4150 5365  },.   "kICLDAPSe
+00005670: 7276 6572 223a 207b 2022 6967 6e6f 7265  rver": { "ignore
+00005680: 223a 2074 7275 6520 7d2c 0a20 2020 226b  ": true },.   "k
+00005690: 4943 4c69 7374 466f 6e74 223a 207b 2022  ICListFont": { "
+000056a0: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
+000056b0: 0a20 2020 226b 4943 4d61 6353 6561 7263  .   "kICMacSearc
+000056c0: 6848 6f73 7422 3a20 7b20 2269 676e 6f72  hHost": { "ignor
+000056d0: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+000056e0: 6b49 434d 6169 6c41 6363 6f75 6e74 223a  kICMailAccount":
+000056f0: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
+00005700: 6520 7d2c 0a20 2020 226b 4943 4d61 696c  e },.   "kICMail
+00005710: 4865 6164 6572 7322 3a20 7b20 2269 676e  Headers": { "ign
+00005720: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
+00005730: 2022 6b49 434d 6169 6c50 6173 7377 6f72   "kICMailPasswor
+00005740: 6422 3a20 7b20 2269 676e 6f72 6522 3a20  d": { "ignore": 
+00005750: 7472 7565 207d 2c0a 2020 2022 6b49 434d  true },.   "kICM
+00005760: 6170 7069 6e67 223a 207b 2022 6967 6e6f  apping": { "igno
+00005770: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
+00005780: 226b 4943 4e4e 5450 486f 7374 223a 207b  "kICNNTPHost": {
+00005790: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
+000057a0: 7d2c 0a20 2020 226b 4943 4e54 5048 6f73  },.   "kICNTPHos
+000057b0: 7422 3a20 7b20 2269 676e 6f72 6522 3a20  t": { "ignore": 
+000057c0: 7472 7565 207d 2c0a 2020 2022 6b49 434e  true },.   "kICN
+000057d0: 6577 4d61 696c 4469 616c 6f67 223a 207b  ewMailDialog": {
+000057e0: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
+000057f0: 7d2c 0a20 2020 226b 4943 4e65 774d 6169  },.   "kICNewMai
+00005800: 6c46 6c61 7368 4963 6f6e 223a 207b 2022  lFlashIcon": { "
+00005810: 6967 6e6f 7265 223a 2074 7275 6520 7d2c  ignore": true },
+00005820: 0a20 2020 226b 4943 4e65 774d 6169 6c50  .   "kICNewMailP
+00005830: 6c61 7953 6f75 6e64 223a 207b 2022 6967  laySound": { "ig
+00005840: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
+00005850: 2020 226b 4943 4e65 774d 6169 6c53 6f75    "kICNewMailSou
+00005860: 6e64 4e61 6d65 223a 207b 2022 6967 6e6f  ndName": { "igno
+00005870: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
+00005880: 226b 4943 4e65 7773 4175 7468 5061 7373  "kICNewsAuthPass
+00005890: 776f 7264 223a 207b 2022 6967 6e6f 7265  word": { "ignore
+000058a0: 223a 2074 7275 6520 7d2c 0a20 2020 226b  ": true },.   "k
+000058b0: 4943 4e65 7773 4175 7468 5573 6572 6e61  ICNewsAuthUserna
+000058c0: 6d65 223a 207b 2022 6967 6e6f 7265 223a  me": { "ignore":
+000058d0: 2074 7275 6520 7d2c 0a20 2020 226b 4943   true },.   "kIC
+000058e0: 4e65 7773 4865 6164 6572 7322 3a20 7b20  NewsHeaders": { 
+000058f0: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+00005900: 2c0a 2020 2022 6b49 434e 6f50 726f 7879  ,.   "kICNoProxy
+00005910: 446f 6d61 696e 7322 3a20 7b20 2269 676e  Domains": { "ign
+00005920: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
+00005930: 2022 6b49 434f 7267 616e 697a 6174 696f   "kICOrganizatio
+00005940: 6e22 3a20 7b20 2269 676e 6f72 6522 3a20  n": { "ignore": 
+00005950: 7472 7565 207d 2c0a 2020 2022 6b49 4350  true },.   "kICP
+00005960: 6848 6f73 7422 3a20 7b20 2269 676e 6f72  hHost": { "ignor
+00005970: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+00005980: 6b49 4350 6c61 6e22 3a20 7b20 2269 676e  kICPlan": { "ign
+00005990: 6f72 6522 3a20 7472 7565 207d 2c0a 2020  ore": true },.  
+000059a0: 2022 6b49 4350 7269 6e74 6572 466f 6e74   "kICPrinterFont
+000059b0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+000059c0: 7275 6520 7d2c 0a20 2020 226b 4943 5175  rue },.   "kICQu
+000059d0: 6f74 696e 6753 7472 696e 6722 3a20 7b20  otingString": { 
+000059e0: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+000059f0: 2c0a 2020 2022 6b49 4352 5453 5050 726f  ,.   "kICRTSPPro
+00005a00: 7879 486f 7374 223a 207b 2022 6967 6e6f  xyHost": { "igno
+00005a10: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
+00005a20: 226b 4943 5265 616c 4e61 6d65 223a 207b  "kICRealName": {
+00005a30: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
+00005a40: 7d2c 0a20 2020 226b 4943 5265 7365 7276  },.   "kICReserv
+00005a50: 6564 4b65 7922 3a20 7b20 2269 676e 6f72  edKey": { "ignor
+00005a60: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+00005a70: 6b49 4353 4d54 5048 6f73 7422 3a20 7b20  kICSMTPHost": { 
+00005a80: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+00005a90: 2c0a 2020 2022 6b49 4353 6372 6565 6e46  ,.   "kICScreenF
+00005aa0: 6f6e 7422 3a20 7b20 2269 676e 6f72 6522  ont": { "ignore"
+00005ab0: 3a20 7472 7565 207d 2c0a 2020 2022 6b49  : true },.   "kI
+00005ac0: 4353 6572 7669 6365 7322 3a20 7b20 2269  CServices": { "i
+00005ad0: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
+00005ae0: 2020 2022 6b49 4353 6967 6e61 7475 7265     "kICSignature
+00005af0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00005b00: 7275 6520 7d2c 0a20 2020 226b 4943 536e  rue },.   "kICSn
+00005b10: 6169 6c4d 6169 6c41 6464 7265 7373 223a  ailMailAddress":
+00005b20: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
+00005b30: 6520 7d2c 0a20 2020 226b 4943 536f 636b  e },.   "kICSock
+00005b40: 7348 6f73 7422 3a20 7b20 2269 676e 6f72  sHost": { "ignor
+00005b50: 6522 3a20 7472 7565 207d 2c0a 2020 2022  e": true },.   "
+00005b60: 6b49 4354 656c 6e65 7448 6f73 7422 3a20  kICTelnetHost": 
+00005b70: 7b20 2269 676e 6f72 6522 3a20 7472 7565  { "ignore": true
+00005b80: 207d 2c0a 2020 2022 6b49 4355 4d69 6368   },.   "kICUMich
+00005b90: 416c 6c22 3a20 7b20 2269 676e 6f72 6522  All": { "ignore"
+00005ba0: 3a20 7472 7565 207d 2c0a 2020 2022 6b49  : true },.   "kI
+00005bb0: 4355 4d69 6368 5072 6566 6572 7265 6422  CUMichPreferred"
+00005bc0: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
+00005bd0: 7565 207d 2c0a 2020 2022 6b49 4355 7365  ue },.   "kICUse
+00005be0: 4654 5050 726f 7879 223a 207b 2022 6967  FTPProxy": { "ig
+00005bf0: 6e6f 7265 223a 2074 7275 6520 7d2c 0a20  nore": true },. 
+00005c00: 2020 226b 4943 5573 6547 6f70 6865 7250    "kICUseGopherP
+00005c10: 726f 7879 223a 207b 2022 6967 6e6f 7265  roxy": { "ignore
+00005c20: 223a 2074 7275 6520 7d2c 0a20 2020 226b  ": true },.   "k
+00005c30: 4943 5573 6548 5454 5050 726f 7879 223a  ICUseHTTPProxy":
+00005c40: 207b 2022 6967 6e6f 7265 223a 2074 7275   { "ignore": tru
+00005c50: 6520 7d2c 0a20 2020 226b 4943 5573 6550  e },.   "kICUseP
+00005c60: 6173 7369 7665 4654 5022 3a20 7b20 2269  assiveFTP": { "i
+00005c70: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
+00005c80: 2020 2022 6b49 4355 7365 5254 5350 5072     "kICUseRTSPPr
+00005c90: 6f78 7922 3a20 7b20 2269 676e 6f72 6522  oxy": { "ignore"
+00005ca0: 3a20 7472 7565 207d 2c0a 2020 2022 6b49  : true },.   "kI
+00005cb0: 4355 7365 536f 636b 7322 3a20 7b20 2269  CUseSocks": { "i
+00005cc0: 676e 6f72 6522 3a20 7472 7565 207d 2c0a  gnore": true },.
+00005cd0: 2020 2022 6b49 4357 4149 5347 6174 6577     "kICWAISGatew
+00005ce0: 6179 223a 207b 2022 6967 6e6f 7265 223a  ay": { "ignore":
+00005cf0: 2074 7275 6520 7d2c 0a20 2020 226b 4943   true },.   "kIC
+00005d00: 5757 5748 6f6d 6550 6167 6522 3a20 7b20  WWWHomePage": { 
+00005d10: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+00005d20: 2c0a 2020 2022 6b49 4357 6562 4261 636b  ,.   "kICWebBack
+00005d30: 6772 6f75 6e64 436f 6c6f 7572 223a 207b  groundColour": {
+00005d40: 2022 6967 6e6f 7265 223a 2074 7275 6520   "ignore": true 
+00005d50: 7d2c 0a20 2020 226b 4943 5765 6252 6561  },.   "kICWebRea
+00005d60: 6443 6f6c 6f72 223a 207b 2022 6967 6e6f  dColor": { "igno
+00005d70: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
+00005d80: 226b 4943 5765 6253 6561 7263 6850 6167  "kICWebSearchPag
+00005d90: 6550 7265 6673 223a 207b 2022 6967 6e6f  ePrefs": { "igno
+00005da0: 7265 223a 2074 7275 6520 7d2c 0a20 2020  re": true },.   
+00005db0: 226b 4943 5765 6254 6578 7443 6f6c 6f72  "kICWebTextColor
+00005dc0: 223a 207b 2022 6967 6e6f 7265 223a 2074  ": { "ignore": t
+00005dd0: 7275 6520 7d2c 0a20 2020 226b 4943 5765  rue },.   "kICWe
+00005de0: 6255 6e64 6572 6c69 6e65 4c69 6e6b 7322  bUnderlineLinks"
+00005df0: 3a20 7b20 2269 676e 6f72 6522 3a20 7472  : { "ignore": tr
+00005e00: 7565 207d 2c0a 2020 2022 6b49 4357 6562  ue },.   "kICWeb
+00005e10: 556e 7265 6164 436f 6c6f 7222 3a20 7b20  UnreadColor": { 
+00005e20: 2269 676e 6f72 6522 3a20 7472 7565 207d  "ignore": true }
+00005e30: 2c0a 2020 2022 6b49 4357 686f 6973 486f  ,.   "kICWhoisHo
+00005e40: 7374 223a 207b 2022 6967 6e6f 7265 223a  st": { "ignore":
+00005e50: 2074 7275 6520 7d0a 2020 7d2c 0a20 2022   true }.  },.  "
+00005e60: 6366 7479 7065 7322 3a20 7b0a 2020 2022  cftypes": {.   "
+00005e70: 4158 5465 7874 4d61 726b 6572 5261 6e67  AXTextMarkerRang
+00005e80: 6552 6566 223a 207b 0a20 2020 2022 6765  eRef": {.    "ge
+00005e90: 7474 7970 6569 645f 6675 6e63 223a 2022  ttypeid_func": "
+00005ea0: 4158 5465 7874 4d61 726b 6572 5261 6e67  AXTextMarkerRang
+00005eb0: 6547 6574 5479 7065 4944 222c 0a20 2020  eGetTypeID",.   
+00005ec0: 2022 7479 7065 7374 7222 3a20 225e 7b5f   "typestr": "^{_
+00005ed0: 5f41 5854 6578 744d 6172 6b65 7252 616e  _AXTextMarkerRan
+00005ee0: 6765 3d7d 220a 2020 207d 2c0a 2020 2022  ge=}".   },.   "
+00005ef0: 4158 5465 7874 4d61 726b 6572 5265 6622  AXTextMarkerRef"
+00005f00: 3a20 7b0a 2020 2020 2267 6574 7479 7065  : {.    "gettype
+00005f10: 6964 5f66 756e 6322 3a20 2241 5854 6578  id_func": "AXTex
+00005f20: 744d 6172 6b65 7247 6574 5479 7065 4944  tMarkerGetTypeID
+00005f30: 222c 0a20 2020 2022 7479 7065 7374 7222  ",.    "typestr"
+00005f40: 3a20 225e 7b5f 5f41 5854 6578 744d 6172  : "^{__AXTextMar
+00005f50: 6b65 723d 7d22 0a20 2020 7d2c 0a20 2020  ker=}".   },.   
+00005f60: 2241 584f 6273 6572 7665 7252 6566 223a  "AXObserverRef":
+00005f70: 207b 0a20 2020 2022 6765 7474 7970 6569   {.    "gettypei
+00005f80: 645f 6675 6e63 223a 2022 4158 4f62 7365  d_func": "AXObse
+00005f90: 7276 6572 4765 7454 7970 6549 4422 2c0a  rverGetTypeID",.
+00005fa0: 2020 2020 2274 7970 6573 7472 223a 2022      "typestr": "
+00005fb0: 5e7b 5f5f 4158 4f62 7365 7276 6572 3d7d  ^{__AXObserver=}
+00005fc0: 220a 2020 207d 2c0a 2020 2022 4158 5549  ".   },.   "AXUI
+00005fd0: 456c 656d 656e 7452 6566 223a 207b 0a20  ElementRef": {. 
+00005fe0: 2020 2022 6765 7474 7970 6569 645f 6675     "gettypeid_fu
+00005ff0: 6e63 223a 2022 4158 5549 456c 656d 656e  nc": "AXUIElemen
+00006000: 7447 6574 5479 7065 4944 222c 0a20 2020  tGetTypeID",.   
+00006010: 2022 7479 7065 7374 7222 3a20 225e 7b5f   "typestr": "^{_
+00006020: 5f41 5855 4945 6c65 6d65 6e74 3d7d 220a  _AXUIElement=}".
+00006030: 2020 207d 2c0a 2020 2022 4158 5661 6c75     },.   "AXValu
+00006040: 6552 6566 223a 207b 0a20 2020 2022 6765  eRef": {.    "ge
+00006050: 7474 7970 6569 645f 6675 6e63 223a 2022  ttypeid_func": "
+00006060: 4158 5661 6c75 6547 6574 5479 7065 4944  AXValueGetTypeID
+00006070: 222c 0a20 2020 2022 7479 7065 7374 7222  ",.    "typestr"
+00006080: 3a20 225e 7b5f 5f41 5856 616c 7565 3d7d  : "^{__AXValue=}
+00006090: 220a 2020 207d 2c0a 2020 2022 4849 5368  ".   },.   "HISh
+000060a0: 6170 6552 6566 223a 207b 0a20 2020 2022  apeRef": {.    "
+000060b0: 6765 7474 7970 6569 645f 6675 6e63 223a  gettypeid_func":
+000060c0: 2022 4849 5368 6170 6547 6574 5479 7065   "HIShapeGetType
+000060d0: 4944 222c 0a20 2020 2022 7479 7065 7374  ID",.    "typest
+000060e0: 7222 3a20 225e 7b5f 5f48 4953 6861 7065  r": "^{__HIShape
+000060f0: 3d7d 220a 2020 207d 2c0a 2020 2022 5472  =}".   },.   "Tr
+00006100: 616e 736c 6174 696f 6e52 6566 223a 207b  anslationRef": {
+00006110: 0a20 2020 2022 6765 7474 7970 6569 645f  .    "gettypeid_
+00006120: 6675 6e63 223a 2022 5472 616e 736c 6174  func": "Translat
+00006130: 696f 6e47 6574 5479 7065 4944 222c 0a20  ionGetTypeID",. 
+00006140: 2020 2022 7479 7065 7374 7222 3a20 225e     "typestr": "^
+00006150: 7b4f 7061 7175 6554 7261 6e73 6c61 7469  {OpaqueTranslati
+00006160: 6f6e 5265 663d 7d22 0a20 2020 7d0a 2020  onRef=}".   }.  
+00006170: 7d0a 207d 0a7d 0a                        }. }.}.
```

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/HIServices.fwinfo.sv` & `pyobjc-framework-ApplicationServices-9.2/metadata/HIServices.fwinfo.sv`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/PrintCore.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/PrintCore.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -804,15 +804,15 @@
      "2": {}
     }
    },
    "PMSessionBeginPageNoDialog": {
     "args": {
      "0": {},
      "1": {},
-     "2": {}
+     "2": { "type_modifier": "n"}
     }
    },
    "PMSessionCopyDestinationFormat": {
     "args": {
      "0": {},
      "1": {},
      "2": { "type_modifier": "o", "already_cfretained": true }
```

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/arm64-12.0.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/arm64-12.3.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/x86_64-10.10.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/x86_64-10.15.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/x86_64-10.16.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/x86_64-12.0.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.HIServices/x86_64-12.3.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.HIServices/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/arm64-12.0.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/arm64-12.3.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/x86_64-10.14.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/x86_64-10.15.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/x86_64-10.16.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/x86_64-12.0.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/metadata/raw.PrintCore/x86_64-12.3.fwinfo` & `pyobjc-framework-ApplicationServices-9.2/metadata/raw.PrintCore/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/pyobjc_setup.py` & `pyobjc-framework-ApplicationServices-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-ApplicationServices-9.1b1/setup.py` & `pyobjc-framework-ApplicationServices-9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 
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
     name="pyobjc-framework-ApplicationServices",
     description="Wrappers for the framework ApplicationServices on macOS",
     packages=["ApplicationServices", "HIServices", "PrintCore"],
     ext_modules=[
         Extension(
```

