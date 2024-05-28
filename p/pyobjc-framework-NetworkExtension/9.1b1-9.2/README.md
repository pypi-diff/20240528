# Comparing `tmp/pyobjc-framework-NetworkExtension-9.1b1.tar.gz` & `tmp/pyobjc-framework-NetworkExtension-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-NetworkExtension-9.1b1.tar", last modified: Sun Mar 26 11:31:58 2023, max compression
+gzip compressed data, was "pyobjc-framework-NetworkExtension-9.2.tar", last modified: Wed Jun  7 00:22:11 2023, max compression
```

## Comparing `pyobjc-framework-NetworkExtension-9.1b1.tar` & `pyobjc-framework-NetworkExtension-9.2.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:58.851087 pyobjc-framework-NetworkExtension-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:58.648418 pyobjc-framework-NetworkExtension-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:58.671766 pyobjc-framework-NetworkExtension-9.1b1/Lib/NetworkExtension/
--rw-r--r--   0 ronald     (501) staff       (20)      781 2020-11-30 18:45:15.000000 pyobjc-framework-NetworkExtension-9.1b1/Lib/NetworkExtension/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    49423 2023-02-19 10:50:35.000000 pyobjc-framework-NetworkExtension-9.1b1/Lib/NetworkExtension/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:58.691679 pyobjc-framework-NetworkExtension-9.1b1/Lib/pyobjc_framework_NetworkExtension.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2136 2023-03-26 11:31:58.000000 pyobjc-framework-NetworkExtension-9.1b1/Lib/pyobjc_framework_NetworkExtension.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     2352 2023-03-26 11:31:58.000000 pyobjc-framework-NetworkExtension-9.1b1/Lib/pyobjc_framework_NetworkExtension.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:31:58.000000 pyobjc-framework-NetworkExtension-9.1b1/Lib/pyobjc_framework_NetworkExtension.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:41.000000 pyobjc-framework-NetworkExtension-9.1b1/Lib/pyobjc_framework_NetworkExtension.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:31:58.000000 pyobjc-framework-NetworkExtension-9.1b1/Lib/pyobjc_framework_NetworkExtension.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       17 2023-03-26 11:31:58.000000 pyobjc-framework-NetworkExtension-9.1b1/Lib/pyobjc_framework_NetworkExtension.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-NetworkExtension-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-NetworkExtension-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:58.695426 pyobjc-framework-NetworkExtension-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1174 2021-10-18 19:38:40.000000 pyobjc-framework-NetworkExtension-9.1b1/Modules/_NetworkExtension.m
--rw-r--r--   0 ronald     (501) staff       (20)      430 2020-11-30 18:45:15.000000 pyobjc-framework-NetworkExtension-9.1b1/Modules/_NetworkExtension_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-NetworkExtension-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-NetworkExtension-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1925 2023-03-26 11:31:58.850749 pyobjc-framework-NetworkExtension-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:58.790161 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2287 2022-10-18 09:53:24.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_NEFilterProvider.py
--rw-r--r--   0 ronald     (501) staff       (20)     2499 2022-10-18 09:53:24.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_NWTCPConnection.py
--rw-r--r--   0 ronald     (501) staff       (20)     1476 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neappproxyflow.py
--rw-r--r--   0 ronald     (501) staff       (20)      781 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neappproxyprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      363 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neappproxyprovidermanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      464 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neappproxytcpflow.py
--rw-r--r--   0 ronald     (501) staff       (20)      512 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neappproxyudpflow.py
--rw-r--r--   0 ronald     (501) staff       (20)     1555 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nednsproxymanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      426 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nednssettings.py
--rw-r--r--   0 ronald     (501) staff       (20)     1633 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nednssettingsmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      741 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nefiltercontrolprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      566 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nefilterdataprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      256 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nefilterflow.py
--rw-r--r--   0 ronald     (501) staff       (20)     1999 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nefiltermanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     1061 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nefilterpacketprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      957 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nefilterproviderconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      732 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nenetworkrule.py
--rw-r--r--   0 ronald     (501) staff       (20)     1184 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neondemandrule.py
--rw-r--r--   0 ronald     (501) staff       (20)      771 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nepackettunnelflow.py
--rw-r--r--   0 ronald     (501) staff       (20)      720 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nepackettunnelprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)     2050 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)     1147 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neproxysettings.py
--rw-r--r--   0 ronald     (501) staff       (20)      369 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_netransparentproxymanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     1586 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_netunnelprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      359 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_netunnelprovidermanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      947 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_netunnelprovidersession.py
--rw-r--r--   0 ronald     (501) staff       (20)      216 2022-04-11 08:03:15.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_networkextension.py
--rw-r--r--   0 ronald     (501) staff       (20)     3819 2022-06-15 11:57:00.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nevpnconnection.py
--rw-r--r--   0 ronald     (501) staff       (20)     1767 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nevpnmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     1382 2023-02-19 10:50:35.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nevpnprotocol.py
--rw-r--r--   0 ronald     (501) staff       (20)     5088 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nevpnprotocolikev2.py
--rw-r--r--   0 ronald     (501) staff       (20)      835 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nevpnprotocolipsec.py
--rw-r--r--   0 ronald     (501) staff       (20)      404 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nsdnssettings.py
--rw-r--r--   0 ronald     (501) staff       (20)      732 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nwpath.py
--rw-r--r--   0 ronald     (501) staff       (20)     1318 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nwudpsession.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:58.795894 pyobjc-framework-NetworkExtension-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    30775 2021-04-06 19:20:58.000000 pyobjc-framework-NetworkExtension-9.1b1/metadata/NetworkExtension.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       48 2020-11-30 18:45:15.000000 pyobjc-framework-NetworkExtension-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:31:58.848551 pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   243133 2021-07-30 09:00:38.000000 pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   245325 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   253743 2022-06-15 11:57:00.000000 pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   255912 2023-02-19 10:50:35.000000 pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   206238 2020-11-30 18:45:15.000000 pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   239138 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   243134 2021-07-30 09:00:38.000000 pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   245326 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   253744 2022-06-15 11:57:00.000000 pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   255913 2023-02-19 10:50:35.000000 pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-NetworkExtension-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:31:58.851188 pyobjc-framework-NetworkExtension-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1201 2023-03-25 14:20:32.000000 pyobjc-framework-NetworkExtension-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:11.252676 pyobjc-framework-NetworkExtension-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:11.130352 pyobjc-framework-NetworkExtension-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:11.147438 pyobjc-framework-NetworkExtension-9.2/Lib/NetworkExtension/
+-rw-r--r--   0 ronald     (501) staff       (20)      781 2020-11-30 18:45:15.000000 pyobjc-framework-NetworkExtension-9.2/Lib/NetworkExtension/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    49423 2023-02-19 10:50:35.000000 pyobjc-framework-NetworkExtension-9.2/Lib/NetworkExtension/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:11.152460 pyobjc-framework-NetworkExtension-9.2/Lib/pyobjc_framework_NetworkExtension.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2134 2023-06-07 00:22:11.000000 pyobjc-framework-NetworkExtension-9.2/Lib/pyobjc_framework_NetworkExtension.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     2367 2023-06-07 00:22:11.000000 pyobjc-framework-NetworkExtension-9.2/Lib/pyobjc_framework_NetworkExtension.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:22:11.000000 pyobjc-framework-NetworkExtension-9.2/Lib/pyobjc_framework_NetworkExtension.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:41.000000 pyobjc-framework-NetworkExtension-9.2/Lib/pyobjc_framework_NetworkExtension.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:22:11.000000 pyobjc-framework-NetworkExtension-9.2/Lib/pyobjc_framework_NetworkExtension.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-06-07 00:22:11.000000 pyobjc-framework-NetworkExtension-9.2/Lib/pyobjc_framework_NetworkExtension.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-NetworkExtension-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-NetworkExtension-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:11.156014 pyobjc-framework-NetworkExtension-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1174 2021-10-18 19:38:40.000000 pyobjc-framework-NetworkExtension-9.2/Modules/_NetworkExtension.m
+-rw-r--r--   0 ronald     (501) staff       (20)      430 2020-11-30 18:45:15.000000 pyobjc-framework-NetworkExtension-9.2/Modules/_NetworkExtension_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-NetworkExtension-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-NetworkExtension-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1923 2023-06-07 00:22:11.252189 pyobjc-framework-NetworkExtension-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:11.209166 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2287 2022-10-18 09:53:24.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_NEFilterProvider.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2499 2022-10-18 09:53:24.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_NWTCPConnection.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1476 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neappproxyflow.py
+-rw-r--r--   0 ronald     (501) staff       (20)      781 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neappproxyprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      363 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neappproxyprovidermanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      464 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neappproxytcpflow.py
+-rw-r--r--   0 ronald     (501) staff       (20)      512 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neappproxyudpflow.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1555 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nednsproxymanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      426 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nednssettings.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1633 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nednssettingsmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      741 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nefiltercontrolprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      566 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nefilterdataprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      256 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nefilterflow.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1999 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nefiltermanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1061 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nefilterpacketprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      957 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nefilterproviderconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      732 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nenetworkrule.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1184 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neondemandrule.py
+-rw-r--r--   0 ronald     (501) staff       (20)      771 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nepackettunnelflow.py
+-rw-r--r--   0 ronald     (501) staff       (20)      720 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nepackettunnelprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2050 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1147 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neproxysettings.py
+-rw-r--r--   0 ronald     (501) staff       (20)      369 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_netransparentproxymanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1586 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_netunnelprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      359 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_netunnelprovidermanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      947 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_netunnelprovidersession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      216 2022-04-11 08:03:15.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_networkextension.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3819 2022-06-15 11:57:00.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nevpnconnection.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1767 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nevpnmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1382 2023-02-19 10:50:35.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nevpnprotocol.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5088 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nevpnprotocolikev2.py
+-rw-r--r--   0 ronald     (501) staff       (20)      835 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nevpnprotocolipsec.py
+-rw-r--r--   0 ronald     (501) staff       (20)      404 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nsdnssettings.py
+-rw-r--r--   0 ronald     (501) staff       (20)      732 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nwpath.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nwudpsession.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:11.212164 pyobjc-framework-NetworkExtension-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    30775 2021-04-06 19:20:58.000000 pyobjc-framework-NetworkExtension-9.2/metadata/NetworkExtension.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       48 2020-11-30 18:45:15.000000 pyobjc-framework-NetworkExtension-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:22:11.249936 pyobjc-framework-NetworkExtension-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   243133 2021-07-30 09:00:38.000000 pyobjc-framework-NetworkExtension-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   245325 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   253743 2022-06-15 11:57:00.000000 pyobjc-framework-NetworkExtension-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   255912 2023-02-19 10:50:35.000000 pyobjc-framework-NetworkExtension-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   206238 2020-11-30 18:45:15.000000 pyobjc-framework-NetworkExtension-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   239138 2021-03-21 10:08:23.000000 pyobjc-framework-NetworkExtension-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   243134 2021-07-30 09:00:38.000000 pyobjc-framework-NetworkExtension-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   245326 2022-02-24 08:47:16.000000 pyobjc-framework-NetworkExtension-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   253744 2022-06-15 11:57:00.000000 pyobjc-framework-NetworkExtension-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   255913 2023-02-19 10:50:35.000000 pyobjc-framework-NetworkExtension-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-NetworkExtension-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-NetworkExtension-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:22:11.252777 pyobjc-framework-NetworkExtension-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1271 2023-05-29 10:07:46.000000 pyobjc-framework-NetworkExtension-9.2/setup.py
```

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/Lib/NetworkExtension/__init__.py` & `pyobjc-framework-NetworkExtension-9.2/Lib/NetworkExtension/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/Lib/NetworkExtension/_metadata.py` & `pyobjc-framework-NetworkExtension-9.2/Lib/NetworkExtension/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/Lib/pyobjc_framework_NetworkExtension.egg-info/PKG-INFO` & `pyobjc-framework-NetworkExtension-9.2/Lib/pyobjc_framework_NetworkExtension.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-NetworkExtension
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework NetworkExtension on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,NetworkExtension
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/Lib/pyobjc_framework_NetworkExtension.egg-info/SOURCES.txt` & `pyobjc-framework-NetworkExtension-9.2/Lib/pyobjc_framework_NetworkExtension.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/NetworkExtension/__init__.py
 Lib/NetworkExtension/_metadata.py
 Lib/pyobjc_framework_NetworkExtension.egg-info/PKG-INFO
 Lib/pyobjc_framework_NetworkExtension.egg-info/SOURCES.txt
 Lib/pyobjc_framework_NetworkExtension.egg-info/dependency_links.txt
 Lib/pyobjc_framework_NetworkExtension.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/License.txt` & `pyobjc-framework-NetworkExtension-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/Modules/_NetworkExtension.m` & `pyobjc-framework-NetworkExtension-9.2/Modules/_NetworkExtension.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-NetworkExtension-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-NetworkExtension-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PKG-INFO` & `pyobjc-framework-NetworkExtension-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-NetworkExtension
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework NetworkExtension on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,NetworkExtension
 Platform: MacOS X (>=10.11)
```

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_NEFilterProvider.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_NEFilterProvider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_NWTCPConnection.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_NWTCPConnection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neappproxyflow.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neappproxyflow.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neappproxyprovider.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neappproxyprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neappproxyudpflow.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neappproxyudpflow.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nednsproxymanager.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nednsproxymanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nednssettingsmanager.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nednssettingsmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nefiltercontrolprovider.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nefiltercontrolprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nefilterdataprovider.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nefilterdataprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nefiltermanager.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nefiltermanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nefilterpacketprovider.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nefilterpacketprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nefilterproviderconfiguration.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nefilterproviderconfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nenetworkrule.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nenetworkrule.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neondemandrule.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neondemandrule.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nepackettunnelflow.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nepackettunnelflow.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nepackettunnelprovider.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nepackettunnelprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neprovider.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_neproxysettings.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_neproxysettings.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_netunnelprovider.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_netunnelprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_netunnelprovidersession.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_netunnelprovidersession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nevpnconnection.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nevpnconnection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nevpnmanager.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nevpnmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nevpnprotocol.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nevpnprotocol.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nevpnprotocolikev2.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nevpnprotocolikev2.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nevpnprotocolipsec.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nevpnprotocolipsec.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nwpath.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nwpath.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/PyObjCTest/test_nwudpsession.py` & `pyobjc-framework-NetworkExtension-9.2/PyObjCTest/test_nwudpsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/metadata/NetworkExtension.fwinfo` & `pyobjc-framework-NetworkExtension-9.2/metadata/NetworkExtension.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-NetworkExtension-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-NetworkExtension-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-NetworkExtension-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-NetworkExtension-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-NetworkExtension-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-NetworkExtension-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-NetworkExtension-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-NetworkExtension-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-NetworkExtension-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-NetworkExtension-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/pyobjc_setup.py` & `pyobjc-framework-NetworkExtension-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-NetworkExtension-9.1b1/setup.py` & `pyobjc-framework-NetworkExtension-9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,21 @@
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
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-NetworkExtension",
     description="Wrappers for the framework NetworkExtension on macOS",
     min_os_level="10.11",
     packages=["NetworkExtension"],
     ext_modules=[
```

