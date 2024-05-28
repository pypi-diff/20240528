# Comparing `tmp/pyobjc-framework-Contacts-9.1b1.tar.gz` & `tmp/pyobjc-framework-Contacts-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Contacts-9.1b1.tar", last modified: Sun Mar 26 11:18:41 2023, max compression
+gzip compressed data, was "pyobjc-framework-Contacts-9.2.tar", last modified: Wed Jun  7 00:09:06 2023, max compression
```

## Comparing `pyobjc-framework-Contacts-9.1b1.tar` & `pyobjc-framework-Contacts-9.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:41.318313 pyobjc-framework-Contacts-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:41.216619 pyobjc-framework-Contacts-9.1b1/Examples/
--rw-r--r--   0 ronald     (501) staff       (20)      741 2021-07-30 09:00:37.000000 pyobjc-framework-Contacts-9.1b1/Examples/print-contacts.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:41.209312 pyobjc-framework-Contacts-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:41.218225 pyobjc-framework-Contacts-9.1b1/Lib/Contacts/
--rw-r--r--   0 ronald     (501) staff       (20)      739 2020-11-30 18:45:14.000000 pyobjc-framework-Contacts-9.1b1/Lib/Contacts/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    20839 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.1b1/Lib/Contacts/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:41.242646 pyobjc-framework-Contacts-9.1b1/Lib/pyobjc_framework_Contacts.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2110 2023-03-26 11:18:41.000000 pyobjc-framework-Contacts-9.1b1/Lib/pyobjc_framework_Contacts.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1517 2023-03-26 11:18:41.000000 pyobjc-framework-Contacts-9.1b1/Lib/pyobjc_framework_Contacts.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:18:41.000000 pyobjc-framework-Contacts-9.1b1/Lib/pyobjc_framework_Contacts.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:36.000000 pyobjc-framework-Contacts-9.1b1/Lib/pyobjc_framework_Contacts.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:18:41.000000 pyobjc-framework-Contacts-9.1b1/Lib/pyobjc_framework_Contacts.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:18:41.000000 pyobjc-framework-Contacts-9.1b1/Lib/pyobjc_framework_Contacts.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Contacts-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-Contacts-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:41.256520 pyobjc-framework-Contacts-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      777 2021-10-18 19:38:40.000000 pyobjc-framework-Contacts-9.1b1/Modules/_Contacts.m
--rw-r--r--   0 ronald     (501) staff       (20)      406 2020-11-30 18:45:14.000000 pyobjc-framework-Contacts-9.1b1/Modules/_Contacts_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-Contacts-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-Contacts-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1899 2023-03-26 11:18:41.317509 pyobjc-framework-Contacts-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:41.283903 pyobjc-framework-Contacts-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      254 2022-06-25 20:14:22.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnchangehistoryevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      899 2022-06-25 20:09:23.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnchangehistoryfetchrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     3359 2022-06-25 20:12:02.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontact.py
--rw-r--r--   0 ronald     (501) staff       (20)      495 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontactfetchrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      789 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontactformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)    23894 2021-07-30 09:00:37.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontactrelation.py
--rw-r--r--   0 ronald     (501) staff       (20)     1951 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontactsstore.py
--rw-r--r--   0 ronald     (501) staff       (20)     1786 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontactstore.py
--rw-r--r--   0 ronald     (501) staff       (20)      410 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontactvcardserialization.py
--rw-r--r--   0 ronald     (501) staff       (20)      699 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontainer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2610 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      288 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cngroup.py
--rw-r--r--   0 ronald     (501) staff       (20)     1080 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cninstantmessageaddress.py
--rw-r--r--   0 ronald     (501) staff       (20)      665 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnlabeledvalue.py
--rw-r--r--   0 ronald     (501) staff       (20)      793 2021-07-30 09:00:37.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnphonenumber.py
--rw-r--r--   0 ronald     (501) staff       (20)      761 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnpostaladdress.py
--rw-r--r--   0 ronald     (501) staff       (20)      554 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnpostaladdressformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)      329 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnsaverequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1147 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnsocialprofile.py
--rw-r--r--   0 ronald     (501) staff       (20)      378 2022-04-11 08:03:15.000000 pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_contacts.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:41.285406 pyobjc-framework-Contacts-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    11798 2021-07-30 09:00:37.000000 pyobjc-framework-Contacts-9.1b1/metadata/Contacts.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:14.000000 pyobjc-framework-Contacts-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:18:41.315267 pyobjc-framework-Contacts-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   128744 2021-07-30 09:00:37.000000 pyobjc-framework-Contacts-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   129900 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   126098 2020-11-30 18:45:14.000000 pyobjc-framework-Contacts-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   127946 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   128745 2021-07-30 09:00:37.000000 pyobjc-framework-Contacts-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   129901 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Contacts-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:18:41.318451 pyobjc-framework-Contacts-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1135 2023-03-25 14:20:30.000000 pyobjc-framework-Contacts-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:06.970944 pyobjc-framework-Contacts-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:06.923457 pyobjc-framework-Contacts-9.2/Examples/
+-rw-r--r--   0 ronald     (501) staff       (20)      741 2021-07-30 09:00:37.000000 pyobjc-framework-Contacts-9.2/Examples/print-contacts.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:06.919447 pyobjc-framework-Contacts-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:06.925313 pyobjc-framework-Contacts-9.2/Lib/Contacts/
+-rw-r--r--   0 ronald     (501) staff       (20)      739 2020-11-30 18:45:14.000000 pyobjc-framework-Contacts-9.2/Lib/Contacts/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    20839 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.2/Lib/Contacts/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:06.930387 pyobjc-framework-Contacts-9.2/Lib/pyobjc_framework_Contacts.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2108 2023-06-07 00:09:06.000000 pyobjc-framework-Contacts-9.2/Lib/pyobjc_framework_Contacts.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1532 2023-06-07 00:09:06.000000 pyobjc-framework-Contacts-9.2/Lib/pyobjc_framework_Contacts.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:09:06.000000 pyobjc-framework-Contacts-9.2/Lib/pyobjc_framework_Contacts.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:36.000000 pyobjc-framework-Contacts-9.2/Lib/pyobjc_framework_Contacts.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:09:06.000000 pyobjc-framework-Contacts-9.2/Lib/pyobjc_framework_Contacts.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:09:06.000000 pyobjc-framework-Contacts-9.2/Lib/pyobjc_framework_Contacts.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Contacts-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-Contacts-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:06.933683 pyobjc-framework-Contacts-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      777 2021-10-18 19:38:40.000000 pyobjc-framework-Contacts-9.2/Modules/_Contacts.m
+-rw-r--r--   0 ronald     (501) staff       (20)      406 2020-11-30 18:45:14.000000 pyobjc-framework-Contacts-9.2/Modules/_Contacts_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-Contacts-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-Contacts-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1897 2023-06-07 00:09:06.970544 pyobjc-framework-Contacts-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:06.959575 pyobjc-framework-Contacts-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      254 2022-06-25 20:14:22.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnchangehistoryevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      899 2022-06-25 20:09:23.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnchangehistoryfetchrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3359 2022-06-25 20:12:02.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontact.py
+-rw-r--r--   0 ronald     (501) staff       (20)      495 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontactfetchrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      789 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontactformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)    23894 2021-07-30 09:00:37.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontactrelation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1951 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontactsstore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1786 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontactstore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      410 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontactvcardserialization.py
+-rw-r--r--   0 ronald     (501) staff       (20)      699 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontainer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2610 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      288 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cngroup.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1080 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cninstantmessageaddress.py
+-rw-r--r--   0 ronald     (501) staff       (20)      665 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnlabeledvalue.py
+-rw-r--r--   0 ronald     (501) staff       (20)      793 2021-07-30 09:00:37.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnphonenumber.py
+-rw-r--r--   0 ronald     (501) staff       (20)      827 2023-05-04 11:00:07.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnpostaladdress.py
+-rw-r--r--   0 ronald     (501) staff       (20)      554 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnpostaladdressformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      329 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnsaverequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1147 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnsocialprofile.py
+-rw-r--r--   0 ronald     (501) staff       (20)      378 2022-04-11 08:03:15.000000 pyobjc-framework-Contacts-9.2/PyObjCTest/test_contacts.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:06.961080 pyobjc-framework-Contacts-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    11798 2021-07-30 09:00:37.000000 pyobjc-framework-Contacts-9.2/metadata/Contacts.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:14.000000 pyobjc-framework-Contacts-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:09:06.969140 pyobjc-framework-Contacts-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   128744 2021-07-30 09:00:37.000000 pyobjc-framework-Contacts-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   129900 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   126098 2020-11-30 18:45:14.000000 pyobjc-framework-Contacts-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   127946 2021-03-21 10:08:22.000000 pyobjc-framework-Contacts-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   128745 2021-07-30 09:00:37.000000 pyobjc-framework-Contacts-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   129901 2022-02-24 08:47:16.000000 pyobjc-framework-Contacts-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Contacts-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Contacts-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:09:06.971074 pyobjc-framework-Contacts-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1206 2023-05-29 10:07:45.000000 pyobjc-framework-Contacts-9.2/setup.py
```

### Comparing `pyobjc-framework-Contacts-9.1b1/Examples/print-contacts.py` & `pyobjc-framework-Contacts-9.2/Examples/print-contacts.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/Lib/Contacts/__init__.py` & `pyobjc-framework-Contacts-9.2/Lib/Contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/Lib/Contacts/_metadata.py` & `pyobjc-framework-Contacts-9.2/Lib/Contacts/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/Lib/pyobjc_framework_Contacts.egg-info/PKG-INFO` & `pyobjc-framework-Contacts-9.2/Lib/pyobjc_framework_Contacts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Contacts
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Contacts on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Contacts
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-Contacts-9.1b1/Lib/pyobjc_framework_Contacts.egg-info/SOURCES.txt` & `pyobjc-framework-Contacts-9.2/Lib/pyobjc_framework_Contacts.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/print-contacts.py
 Lib/Contacts/__init__.py
 Lib/Contacts/_metadata.py
 Lib/pyobjc_framework_Contacts.egg-info/PKG-INFO
 Lib/pyobjc_framework_Contacts.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Contacts.egg-info/dependency_links.txt
```

### Comparing `pyobjc-framework-Contacts-9.1b1/License.txt` & `pyobjc-framework-Contacts-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/Modules/_Contacts.m` & `pyobjc-framework-Contacts-9.2/Modules/_Contacts.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-Contacts-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-Contacts-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-Contacts-9.1b1/PKG-INFO` & `pyobjc-framework-Contacts-9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Contacts
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Contacts on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Contacts
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnchangehistoryfetchrequest.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnchangehistoryfetchrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontact.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontact.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontactformatter.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontactformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontactrelation.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontactrelation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontactsstore.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontactsstore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontactstore.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontactstore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cncontainer.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cncontainer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnerror.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cninstantmessageaddress.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cninstantmessageaddress.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnlabeledvalue.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnlabeledvalue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnphonenumber.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnphonenumber.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnpostaladdress.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnpostaladdress.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,9 +8,12 @@
         self.assertIsInstance(Contacts.CNPostalAddressStreetKey, str)
         self.assertIsInstance(Contacts.CNPostalAddressCityKey, str)
         self.assertIsInstance(Contacts.CNPostalAddressStateKey, str)
         self.assertIsInstance(Contacts.CNPostalAddressPostalCodeKey, str)
         self.assertIsInstance(Contacts.CNPostalAddressCountryKey, str)
         self.assertIsInstance(Contacts.CNPostalAddressISOCountryCodeKey, str)
 
-        self.assertIsInstance(Contacts.CNPostalAddressSubLocalityKey, str)
         self.assertIsInstance(Contacts.CNPostalAddressSubAdministrativeAreaKey, str)
+
+    @min_os_level("10.12.4")
+    def testConstants10_12_4(self):
+        self.assertIsInstance(Contacts.CNPostalAddressSubLocalityKey, str)
```

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnpostaladdressformatter.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnpostaladdressformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/PyObjCTest/test_cnsocialprofile.py` & `pyobjc-framework-Contacts-9.2/PyObjCTest/test_cnsocialprofile.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/metadata/Contacts.fwinfo` & `pyobjc-framework-Contacts-9.2/metadata/Contacts.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-Contacts-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Contacts-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-Contacts-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-Contacts-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-Contacts-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Contacts-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Contacts-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Contacts-9.1b1/setup.py` & `pyobjc-framework-Contacts-9.2/setup.py`

 * *Files 12% similar despite different names*

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
     name="pyobjc-framework-Contacts",
     description="Wrappers for the framework Contacts on macOS",
     min_os_level="10.11",
     packages=["Contacts"],
     ext_modules=[
```

