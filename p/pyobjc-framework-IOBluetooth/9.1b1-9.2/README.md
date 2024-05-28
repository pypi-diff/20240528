# Comparing `tmp/pyobjc-framework-IOBluetooth-9.1b1.tar.gz` & `tmp/pyobjc-framework-IOBluetooth-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-IOBluetooth-9.1b1.tar", last modified: Sun Mar 26 11:26:27 2023, max compression
+gzip compressed data, was "pyobjc-framework-IOBluetooth-9.2.tar", last modified: Wed Jun  7 00:16:46 2023, max compression
```

## Comparing `pyobjc-framework-IOBluetooth-9.1b1.tar` & `pyobjc-framework-IOBluetooth-9.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:27.724157 pyobjc-framework-IOBluetooth-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:27.628794 pyobjc-framework-IOBluetooth-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:27.638643 pyobjc-framework-IOBluetooth-9.1b1/Lib/IOBluetooth/
--rw-r--r--   0 ronald     (501) staff       (20)      784 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/Lib/IOBluetooth/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3252 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/Lib/IOBluetooth/_funcmacros.py
--rw-r--r--   0 ronald     (501) staff       (20)   183595 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/Lib/IOBluetooth/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:27.648904 pyobjc-framework-IOBluetooth-9.1b1/Lib/pyobjc_framework_IOBluetooth.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2106 2023-03-26 11:26:27.000000 pyobjc-framework-IOBluetooth-9.1b1/Lib/pyobjc_framework_IOBluetooth.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1668 2023-03-26 11:26:27.000000 pyobjc-framework-IOBluetooth-9.1b1/Lib/pyobjc_framework_IOBluetooth.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:26:27.000000 pyobjc-framework-IOBluetooth-9.1b1/Lib/pyobjc_framework_IOBluetooth.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-02-19 13:45:26.000000 pyobjc-framework-IOBluetooth-9.1b1/Lib/pyobjc_framework_IOBluetooth.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:26:27.000000 pyobjc-framework-IOBluetooth-9.1b1/Lib/pyobjc_framework_IOBluetooth.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       12 2023-03-26 11:26:27.000000 pyobjc-framework-IOBluetooth-9.1b1/Lib/pyobjc_framework_IOBluetooth.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:27.653405 pyobjc-framework-IOBluetooth-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      829 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/Modules/_IOBluetooth.m
--rw-r--r--   0 ronald     (501) staff       (20)      836 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/Modules/_IOBluetooth_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-IOBluetooth-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1895 2023-03-26 11:26:27.723820 pyobjc-framework-IOBluetooth-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:27.687915 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)   144694 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_bluetooth.py
--rw-r--r--   0 ronald     (501) staff       (20)    62753 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_bluetoothassignednumbers.py
--rw-r--r--   0 ronald     (501) staff       (20)     1516 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobLuetoothdeviceinquiry.py
--rw-r--r--   0 ronald     (501) staff       (20)      739 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetooth.py
--rw-r--r--   0 ronald     (501) staff       (20)     2512 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothL2capchannel.py
--rw-r--r--   0 ronald     (501) staff       (20)     3430 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothdevice.py
--rw-r--r--   0 ronald     (501) staff       (20)     1522 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothdevicepair.py
--rw-r--r--   0 ronald     (501) staff       (20)     7484 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothhandsfree.py
--rw-r--r--   0 ronald     (501) staff       (20)      243 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothhandsfreeaudiogateway.py
--rw-r--r--   0 ronald     (501) staff       (20)      231 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothhandsfreedevice.py
--rw-r--r--   0 ronald     (501) staff       (20)      379 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothhostcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      475 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothobexsession.py
--rw-r--r--   0 ronald     (501) staff       (20)      315 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothobject.py
--rw-r--r--   0 ronald     (501) staff       (20)     3381 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothrfcommchannel.py
--rw-r--r--   0 ronald     (501) staff       (20)      228 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothsdpdataelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      576 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothsdpserviceRecord.py
--rw-r--r--   0 ronald     (501) staff       (20)      412 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothsdpuuid.py
--rw-r--r--   0 ronald     (501) staff       (20)     3300 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothuserlib.py
--rw-r--r--   0 ronald     (501) staff       (20)     1837 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothutilities.py
--rw-r--r--   0 ronald     (501) staff       (20)     3873 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_nsdictionaryobexextensions.py
--rw-r--r--   0 ronald     (501) staff       (20)    35285 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_obex.py
--rw-r--r--   0 ronald     (501) staff       (20)     1059 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_obexbluetooth.py
--rw-r--r--   0 ronald     (501) staff       (20)     1236 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_obexfiletransferservices.py
--rw-r--r--   0 ronald     (501) staff       (20)     5798 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_obexsession.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:27.689504 pyobjc-framework-IOBluetooth-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    31009 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/metadata/IOBluetooth.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:26:27.695057 pyobjc-framework-IOBluetooth-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   367168 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/metadata/raw/arm64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   367215 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.1b1/metadata/raw/x86_64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-IOBluetooth-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:26:27.724260 pyobjc-framework-IOBluetooth-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1153 2023-03-25 14:20:31.000000 pyobjc-framework-IOBluetooth-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:46.689503 pyobjc-framework-IOBluetooth-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:46.635989 pyobjc-framework-IOBluetooth-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:46.643969 pyobjc-framework-IOBluetooth-9.2/Lib/IOBluetooth/
+-rw-r--r--   0 ronald     (501) staff       (20)      784 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/Lib/IOBluetooth/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3252 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/Lib/IOBluetooth/_funcmacros.py
+-rw-r--r--   0 ronald     (501) staff       (20)   183595 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/Lib/IOBluetooth/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:46.648943 pyobjc-framework-IOBluetooth-9.2/Lib/pyobjc_framework_IOBluetooth.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2104 2023-06-07 00:16:46.000000 pyobjc-framework-IOBluetooth-9.2/Lib/pyobjc_framework_IOBluetooth.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1683 2023-06-07 00:16:46.000000 pyobjc-framework-IOBluetooth-9.2/Lib/pyobjc_framework_IOBluetooth.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:16:46.000000 pyobjc-framework-IOBluetooth-9.2/Lib/pyobjc_framework_IOBluetooth.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-02-19 13:45:26.000000 pyobjc-framework-IOBluetooth-9.2/Lib/pyobjc_framework_IOBluetooth.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:16:46.000000 pyobjc-framework-IOBluetooth-9.2/Lib/pyobjc_framework_IOBluetooth.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       12 2023-06-07 00:16:46.000000 pyobjc-framework-IOBluetooth-9.2/Lib/pyobjc_framework_IOBluetooth.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:46.651305 pyobjc-framework-IOBluetooth-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      829 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/Modules/_IOBluetooth.m
+-rw-r--r--   0 ronald     (501) staff       (20)      836 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/Modules/_IOBluetooth_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-IOBluetooth-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1893 2023-06-07 00:16:46.688799 pyobjc-framework-IOBluetooth-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:46.674966 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)   144694 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_bluetooth.py
+-rw-r--r--   0 ronald     (501) staff       (20)    62753 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_bluetoothassignednumbers.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1516 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobLuetoothdeviceinquiry.py
+-rw-r--r--   0 ronald     (501) staff       (20)      739 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetooth.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2586 2023-05-04 11:00:07.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothL2capchannel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3430 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothdevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1522 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothdevicepair.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7484 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothhandsfree.py
+-rw-r--r--   0 ronald     (501) staff       (20)      243 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothhandsfreeaudiogateway.py
+-rw-r--r--   0 ronald     (501) staff       (20)      231 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothhandsfreedevice.py
+-rw-r--r--   0 ronald     (501) staff       (20)      379 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothhostcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      475 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothobexsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      315 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3381 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothrfcommchannel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      228 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothsdpdataelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      576 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothsdpserviceRecord.py
+-rw-r--r--   0 ronald     (501) staff       (20)      412 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothsdpuuid.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3300 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothuserlib.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1837 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothutilities.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3873 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_nsdictionaryobexextensions.py
+-rw-r--r--   0 ronald     (501) staff       (20)    35285 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_obex.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1059 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_obexbluetooth.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1236 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_obexfiletransferservices.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5798 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_obexsession.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:46.682479 pyobjc-framework-IOBluetooth-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    31009 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/metadata/IOBluetooth.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:16:46.685796 pyobjc-framework-IOBluetooth-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   367168 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/metadata/raw/arm64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   367215 2023-02-19 10:50:35.000000 pyobjc-framework-IOBluetooth-9.2/metadata/raw/x86_64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-IOBluetooth-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-IOBluetooth-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:16:46.689645 pyobjc-framework-IOBluetooth-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1224 2023-05-29 10:07:46.000000 pyobjc-framework-IOBluetooth-9.2/setup.py
```

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/Lib/IOBluetooth/__init__.py` & `pyobjc-framework-IOBluetooth-9.2/Lib/IOBluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/Lib/IOBluetooth/_funcmacros.py` & `pyobjc-framework-IOBluetooth-9.2/Lib/IOBluetooth/_funcmacros.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/Lib/IOBluetooth/_metadata.py` & `pyobjc-framework-IOBluetooth-9.2/Lib/IOBluetooth/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/Lib/pyobjc_framework_IOBluetooth.egg-info/PKG-INFO` & `pyobjc-framework-IOBluetooth-9.2/Lib/pyobjc_framework_IOBluetooth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-IOBluetooth
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework IOBluetooth on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,IOBluetooth
 Platform: MacOS X
```

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/Lib/pyobjc_framework_IOBluetooth.egg-info/SOURCES.txt` & `pyobjc-framework-IOBluetooth-9.2/Lib/pyobjc_framework_IOBluetooth.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/IOBluetooth/__init__.py
 Lib/IOBluetooth/_funcmacros.py
 Lib/IOBluetooth/_metadata.py
 Lib/pyobjc_framework_IOBluetooth.egg-info/PKG-INFO
 Lib/pyobjc_framework_IOBluetooth.egg-info/SOURCES.txt
 Lib/pyobjc_framework_IOBluetooth.egg-info/dependency_links.txt
```

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/License.txt` & `pyobjc-framework-IOBluetooth-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/Modules/_IOBluetooth.m` & `pyobjc-framework-IOBluetooth-9.2/Modules/_IOBluetooth.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/Modules/_IOBluetooth_protocols.m` & `pyobjc-framework-IOBluetooth-9.2/Modules/_IOBluetooth_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-IOBluetooth-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-IOBluetooth-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PKG-INFO` & `pyobjc-framework-IOBluetooth-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-IOBluetooth
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework IOBluetooth on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,IOBluetooth
 Platform: MacOS X
```

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_bluetooth.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_bluetooth.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_bluetoothassignednumbers.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_bluetoothassignednumbers.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobLuetoothdeviceinquiry.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobLuetoothdeviceinquiry.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetooth.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetooth.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothL2capchannel.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothL2capchannel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_os_level
 
 import IOBluetooth
 
 import objc
 
 
 class TestIOBluetoothL2CAPChannelHelper(IOBluetooth.NSObject):
@@ -56,26 +56,28 @@
             TestIOBluetoothL2CAPChannelHelper.l2capChannelWriteComplete_refcon_status_,
             2,
             objc._C_INT,
         )
 
     def test_methods(self):
         self.assertArgIsIn(
-            IOBluetooth.IOBluetoothL2CAPChannel.writeAsyncTrap_length_refcon_, 0
-        )
-        self.assertArgSizeInArg(
-            IOBluetooth.IOBluetoothL2CAPChannel.writeAsyncTrap_length_refcon_, 0, 1
-        )
-
-        self.assertArgIsIn(
             IOBluetooth.IOBluetoothL2CAPChannel.writeAsync_length_refcon_, 0
         )
         self.assertArgSizeInArg(
             IOBluetooth.IOBluetoothL2CAPChannel.writeAsync_length_refcon_, 0, 1
         )
 
         self.assertArgIsIn(IOBluetooth.IOBluetoothL2CAPChannel.writeSync_length_, 0)
         self.assertArgSizeInArg(
             IOBluetooth.IOBluetoothL2CAPChannel.writeSync_length_, 0, 1
         )
 
         self.assertResultIsBOOL(IOBluetooth.IOBluetoothL2CAPChannel.isIncoming)
+
+    @min_os_level("10.14")
+    def test_methods10_14(self):
+        self.assertArgIsIn(
+            IOBluetooth.IOBluetoothL2CAPChannel.writeAsyncTrap_length_refcon_, 0
+        )
+        self.assertArgSizeInArg(
+            IOBluetooth.IOBluetoothL2CAPChannel.writeAsyncTrap_length_refcon_, 0, 1
+        )
```

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothdevice.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothdevice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothdevicepair.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothdevicepair.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothhandsfree.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothhandsfree.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothrfcommchannel.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothrfcommchannel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothsdpserviceRecord.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothsdpserviceRecord.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothuserlib.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothuserlib.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_iobluetoothutilities.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_iobluetoothutilities.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_nsdictionaryobexextensions.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_nsdictionaryobexextensions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_obex.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_obex.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_obexbluetooth.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_obexbluetooth.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_obexfiletransferservices.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_obexfiletransferservices.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/PyObjCTest/test_obexsession.py` & `pyobjc-framework-IOBluetooth-9.2/PyObjCTest/test_obexsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/metadata/IOBluetooth.fwinfo` & `pyobjc-framework-IOBluetooth-9.2/metadata/IOBluetooth.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/metadata/raw/arm64-13.1.fwinfo` & `pyobjc-framework-IOBluetooth-9.2/metadata/raw/arm64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/metadata/raw/x86_64-13.1.fwinfo` & `pyobjc-framework-IOBluetooth-9.2/metadata/raw/x86_64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/pyobjc_setup.py` & `pyobjc-framework-IOBluetooth-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-IOBluetooth-9.1b1/setup.py` & `pyobjc-framework-IOBluetooth-9.2/setup.py`

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
     name="pyobjc-framework-IOBluetooth",
     description="Wrappers for the framework IOBluetooth on macOS",
     packages=["IOBluetooth"],
     ext_modules=[
         Extension(
```

