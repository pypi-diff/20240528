# Comparing `tmp/pyobjc-framework-Photos-9.1b1.tar.gz` & `tmp/pyobjc-framework-Photos-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Photos-9.1b1.tar", last modified: Sun Mar 26 11:33:40 2023, max compression
+gzip compressed data, was "pyobjc-framework-Photos-9.2.tar", last modified: Wed Jun  7 00:23:28 2023, max compression
```

## Comparing `pyobjc-framework-Photos-9.1b1.tar` & `pyobjc-framework-Photos-9.2.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:40.855527 pyobjc-framework-Photos-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:40.649412 pyobjc-framework-Photos-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:40.700374 pyobjc-framework-Photos-9.1b1/Lib/Photos/
--rw-r--r--   0 ronald     (501) staff       (20)      709 2020-11-30 18:45:15.000000 pyobjc-framework-Photos-9.1b1/Lib/Photos/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    32140 2023-02-19 10:50:35.000000 pyobjc-framework-Photos-9.1b1/Lib/Photos/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:40.706029 pyobjc-framework-Photos-9.1b1/Lib/pyobjc_framework_Photos.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2096 2023-03-26 11:33:40.000000 pyobjc-framework-Photos-9.1b1/Lib/pyobjc_framework_Photos.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1662 2023-03-26 11:33:40.000000 pyobjc-framework-Photos-9.1b1/Lib/pyobjc_framework_Photos.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:33:40.000000 pyobjc-framework-Photos-9.1b1/Lib/pyobjc_framework_Photos.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:47.000000 pyobjc-framework-Photos-9.1b1/Lib/pyobjc_framework_Photos.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:33:40.000000 pyobjc-framework-Photos-9.1b1/Lib/pyobjc_framework_Photos.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        7 2023-03-26 11:33:40.000000 pyobjc-framework-Photos-9.1b1/Lib/pyobjc_framework_Photos.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Photos-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Photos-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:40.710415 pyobjc-framework-Photos-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      765 2021-10-18 19:38:40.000000 pyobjc-framework-Photos-9.1b1/Modules/_Photos.m
--rw-r--r--   0 ronald     (501) staff       (20)      581 2020-11-30 18:45:15.000000 pyobjc-framework-Photos-9.1b1/Modules/_Photos_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:33.000000 pyobjc-framework-Photos-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-02-19 12:24:44.000000 pyobjc-framework-Photos-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1885 2023-03-26 11:33:40.843895 pyobjc-framework-Photos-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:40.769082 pyobjc-framework-Photos-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      251 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phadjustmentdata.py
--rw-r--r--   0 ronald     (501) staff       (20)      778 2022-06-15 11:57:00.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phasset.py
--rw-r--r--   0 ronald     (501) staff       (20)     1414 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phassetchangerequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      493 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phassetresourcecreationoptions.py
--rw-r--r--   0 ronald     (501) staff       (20)     1024 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phassetresourcemanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      486 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phchange.py
--rw-r--r--   0 ronald     (501) staff       (20)      239 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phcloudidentifier.py
--rw-r--r--   0 ronald     (501) staff       (20)      391 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phcollection.py
--rw-r--r--   0 ronald     (501) staff       (20)      261 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phcontenteditinginput.py
--rw-r--r--   0 ronald     (501) staff       (20)      263 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phcontenteditingoutput.py
--rw-r--r--   0 ronald     (501) staff       (20)     1656 2022-06-15 11:57:00.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_pherror.py
--rw-r--r--   0 ronald     (501) staff       (20)      711 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phfetchoptions.py
--rw-r--r--   0 ronald     (501) staff       (20)      777 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phfetchresult.py
--rw-r--r--   0 ronald     (501) staff       (20)     5103 2022-02-24 08:47:16.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phimagemanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      736 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phlivephoto.py
--rw-r--r--   0 ronald     (501) staff       (20)     2361 2022-06-25 09:21:19.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phlivephotoeditingcontext.py
--rw-r--r--   0 ronald     (501) staff       (20)      196 2022-04-11 08:03:15.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_photos.py
--rw-r--r--   0 ronald     (501) staff       (20)     7746 2023-03-03 17:21:59.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_photostypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      287 2022-06-15 11:57:00.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phpersistentchange.py
--rw-r--r--   0 ronald     (501) staff       (20)      314 2022-06-15 11:57:00.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phpersistentchangefetchresult.py
--rw-r--r--   0 ronald     (501) staff       (20)     1849 2022-06-25 09:21:17.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phphotolibrary.py
--rw-r--r--   0 ronald     (501) staff       (20)      229 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phproject.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:40.772231 pyobjc-framework-Photos-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    21461 2022-02-24 08:47:16.000000 pyobjc-framework-Photos-9.1b1/metadata/Photos.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:15.000000 pyobjc-framework-Photos-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:33:40.812529 pyobjc-framework-Photos-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   133749 2021-07-30 09:00:38.000000 pyobjc-framework-Photos-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   135122 2022-02-24 08:47:16.000000 pyobjc-framework-Photos-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   145158 2022-06-15 11:57:00.000000 pyobjc-framework-Photos-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   145853 2023-02-19 10:50:35.000000 pyobjc-framework-Photos-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   120828 2020-11-30 18:45:15.000000 pyobjc-framework-Photos-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   129884 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   133750 2021-07-30 09:00:38.000000 pyobjc-framework-Photos-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   135123 2022-02-24 08:47:16.000000 pyobjc-framework-Photos-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   145159 2022-06-15 11:57:00.000000 pyobjc-framework-Photos-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   145854 2023-02-19 10:50:35.000000 pyobjc-framework-Photos-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Photos-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:33:40.855802 pyobjc-framework-Photos-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1110 2023-03-25 14:20:32.000000 pyobjc-framework-Photos-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:28.232330 pyobjc-framework-Photos-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:28.139862 pyobjc-framework-Photos-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:28.145330 pyobjc-framework-Photos-9.2/Lib/Photos/
+-rw-r--r--   0 ronald     (501) staff       (20)      709 2020-11-30 18:45:15.000000 pyobjc-framework-Photos-9.2/Lib/Photos/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    32140 2023-02-19 10:50:35.000000 pyobjc-framework-Photos-9.2/Lib/Photos/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:28.149356 pyobjc-framework-Photos-9.2/Lib/pyobjc_framework_Photos.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2094 2023-06-07 00:23:28.000000 pyobjc-framework-Photos-9.2/Lib/pyobjc_framework_Photos.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1677 2023-06-07 00:23:28.000000 pyobjc-framework-Photos-9.2/Lib/pyobjc_framework_Photos.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:23:28.000000 pyobjc-framework-Photos-9.2/Lib/pyobjc_framework_Photos.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:47.000000 pyobjc-framework-Photos-9.2/Lib/pyobjc_framework_Photos.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:23:28.000000 pyobjc-framework-Photos-9.2/Lib/pyobjc_framework_Photos.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        7 2023-06-07 00:23:28.000000 pyobjc-framework-Photos-9.2/Lib/pyobjc_framework_Photos.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Photos-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Photos-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:28.152022 pyobjc-framework-Photos-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      765 2021-10-18 19:38:40.000000 pyobjc-framework-Photos-9.2/Modules/_Photos.m
+-rw-r--r--   0 ronald     (501) staff       (20)      581 2020-11-30 18:45:15.000000 pyobjc-framework-Photos-9.2/Modules/_Photos_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:33.000000 pyobjc-framework-Photos-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-05-29 07:18:42.000000 pyobjc-framework-Photos-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1883 2023-06-07 00:23:28.230869 pyobjc-framework-Photos-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:28.189081 pyobjc-framework-Photos-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:15.000000 pyobjc-framework-Photos-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      251 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phadjustmentdata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      778 2022-06-15 11:57:00.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phasset.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1414 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phassetchangerequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      493 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phassetresourcecreationoptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1024 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phassetresourcemanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      486 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phchange.py
+-rw-r--r--   0 ronald     (501) staff       (20)      239 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phcloudidentifier.py
+-rw-r--r--   0 ronald     (501) staff       (20)      391 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phcollection.py
+-rw-r--r--   0 ronald     (501) staff       (20)      261 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phcontenteditinginput.py
+-rw-r--r--   0 ronald     (501) staff       (20)      263 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phcontenteditingoutput.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1656 2022-06-15 11:57:00.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_pherror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      711 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phfetchoptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)      777 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phfetchresult.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5103 2022-02-24 08:47:16.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phimagemanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      736 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phlivephoto.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2361 2022-06-25 09:21:19.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phlivephotoeditingcontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)      196 2022-04-11 08:03:15.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_photos.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7746 2023-03-03 17:21:59.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_photostypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      287 2022-06-15 11:57:00.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phpersistentchange.py
+-rw-r--r--   0 ronald     (501) staff       (20)      314 2022-06-15 11:57:00.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phpersistentchangefetchresult.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1849 2022-06-25 09:21:17.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phphotolibrary.py
+-rw-r--r--   0 ronald     (501) staff       (20)      229 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/PyObjCTest/test_phproject.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:28.191046 pyobjc-framework-Photos-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    21461 2022-02-24 08:47:16.000000 pyobjc-framework-Photos-9.2/metadata/Photos.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       28 2020-11-30 18:45:15.000000 pyobjc-framework-Photos-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:23:28.229272 pyobjc-framework-Photos-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   133749 2021-07-30 09:00:38.000000 pyobjc-framework-Photos-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   135122 2022-02-24 08:47:16.000000 pyobjc-framework-Photos-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   145158 2022-06-15 11:57:00.000000 pyobjc-framework-Photos-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   145853 2023-02-19 10:50:35.000000 pyobjc-framework-Photos-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   120828 2020-11-30 18:45:15.000000 pyobjc-framework-Photos-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   129884 2021-03-21 10:08:23.000000 pyobjc-framework-Photos-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   133750 2021-07-30 09:00:38.000000 pyobjc-framework-Photos-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   135123 2022-02-24 08:47:16.000000 pyobjc-framework-Photos-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   145159 2022-06-15 11:57:00.000000 pyobjc-framework-Photos-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   145854 2023-02-19 10:50:35.000000 pyobjc-framework-Photos-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Photos-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Photos-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:23:28.232446 pyobjc-framework-Photos-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1181 2023-05-29 10:07:47.000000 pyobjc-framework-Photos-9.2/setup.py
```

### Comparing `pyobjc-framework-Photos-9.1b1/Lib/Photos/__init__.py` & `pyobjc-framework-Photos-9.2/Lib/Photos/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/Lib/Photos/_metadata.py` & `pyobjc-framework-Photos-9.2/Lib/Photos/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/Lib/pyobjc_framework_Photos.egg-info/PKG-INFO` & `pyobjc-framework-Photos-9.2/Lib/pyobjc_framework_Photos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Photos
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Photos on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Photos
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-Photos-9.1b1/Lib/pyobjc_framework_Photos.egg-info/SOURCES.txt` & `pyobjc-framework-Photos-9.2/Lib/pyobjc_framework_Photos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/Photos/__init__.py
 Lib/Photos/_metadata.py
 Lib/pyobjc_framework_Photos.egg-info/PKG-INFO
 Lib/pyobjc_framework_Photos.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Photos.egg-info/dependency_links.txt
 Lib/pyobjc_framework_Photos.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-Photos-9.1b1/License.txt` & `pyobjc-framework-Photos-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/Modules/_Photos.m` & `pyobjc-framework-Photos-9.2/Modules/_Photos.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/Modules/_Photos_protocols.m` & `pyobjc-framework-Photos-9.2/Modules/_Photos_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-Photos-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-Photos-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-Photos-9.1b1/PKG-INFO` & `pyobjc-framework-Photos-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Photos
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Photos on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Photos
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phasset.py` & `pyobjc-framework-Photos-9.2/PyObjCTest/test_phasset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phassetchangerequest.py` & `pyobjc-framework-Photos-9.2/PyObjCTest/test_phassetchangerequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phassetresourcemanager.py` & `pyobjc-framework-Photos-9.2/PyObjCTest/test_phassetresourcemanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/PyObjCTest/test_pherror.py` & `pyobjc-framework-Photos-9.2/PyObjCTest/test_pherror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phfetchoptions.py` & `pyobjc-framework-Photos-9.2/PyObjCTest/test_phfetchoptions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phfetchresult.py` & `pyobjc-framework-Photos-9.2/PyObjCTest/test_phfetchresult.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phimagemanager.py` & `pyobjc-framework-Photos-9.2/PyObjCTest/test_phimagemanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phlivephoto.py` & `pyobjc-framework-Photos-9.2/PyObjCTest/test_phlivephoto.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phlivephotoeditingcontext.py` & `pyobjc-framework-Photos-9.2/PyObjCTest/test_phlivephotoeditingcontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/PyObjCTest/test_photostypes.py` & `pyobjc-framework-Photos-9.2/PyObjCTest/test_photostypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/PyObjCTest/test_phphotolibrary.py` & `pyobjc-framework-Photos-9.2/PyObjCTest/test_phphotolibrary.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/metadata/Photos.fwinfo` & `pyobjc-framework-Photos-9.2/metadata/Photos.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-Photos-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Photos-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-Photos-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-Photos-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-Photos-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-Photos-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-Photos-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Photos-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-Photos-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-Photos-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Photos-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Photos-9.1b1/setup.py` & `pyobjc-framework-Photos-9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 
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
     name="pyobjc-framework-Photos",
     description="Wrappers for the framework Photos on macOS",
     min_os_level="10.11",
     packages=["Photos"],
     ext_modules=[
```

