# Comparing `tmp/pyobjc-framework-Security-9.1b1.tar.gz` & `tmp/pyobjc-framework-Security-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Security-9.1b1.tar", last modified: Sun Mar 26 11:39:14 2023, max compression
+gzip compressed data, was "pyobjc-framework-Security-9.2.tar", last modified: Wed Jun  7 00:27:37 2023, max compression
```

## Comparing `pyobjc-framework-Security-9.1b1.tar` & `pyobjc-framework-Security-9.2.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:14.395987 pyobjc-framework-Security-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:14.144950 pyobjc-framework-Security-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:14.161092 pyobjc-framework-Security-9.1b1/Lib/Security/
--rw-r--r--   0 ronald     (501) staff       (20)      709 2020-11-30 18:45:15.000000 pyobjc-framework-Security-9.1b1/Lib/Security/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)   128269 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.1b1/Lib/Security/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:14.174476 pyobjc-framework-Security-9.1b1/Lib/pyobjc_framework_Security.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2094 2023-03-26 11:39:14.000000 pyobjc-framework-Security-9.1b1/Lib/pyobjc_framework_Security.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     3065 2023-03-26 11:39:14.000000 pyobjc-framework-Security-9.1b1/Lib/pyobjc_framework_Security.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:39:14.000000 pyobjc-framework-Security-9.1b1/Lib/pyobjc_framework_Security.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:34.000000 pyobjc-framework-Security-9.1b1/Lib/pyobjc_framework_Security.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:39:14.000000 pyobjc-framework-Security-9.1b1/Lib/pyobjc_framework_Security.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:39:14.000000 pyobjc-framework-Security-9.1b1/Lib/pyobjc_framework_Security.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Security-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Security-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:14.177512 pyobjc-framework-Security-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)    27838 2022-10-31 12:20:31.000000 pyobjc-framework-Security-9.1b1/Modules/_Security.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-Security-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1883 2023-03-26 11:39:14.395388 pyobjc-framework-Security-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:14.330023 pyobjc-framework-Security-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     5419 2022-02-24 08:47:17.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_authorization.py
--rw-r--r--   0 ronald     (501) staff       (20)     2563 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_authorizationdb.py
--rw-r--r--   0 ronald     (501) staff       (20)      740 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_authorizationtags.py
--rw-r--r--   0 ronald     (501) staff       (20)     1736 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_authsession.py
--rw-r--r--   0 ronald     (501) staff       (20)     5631 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_certextensions.py
--rw-r--r--   0 ronald     (501) staff       (20)    13224 2021-04-09 10:15:21.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_ciphersuite.py
--rw-r--r--   0 ronald     (501) staff       (20)     8080 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cmsdecoder.py
--rw-r--r--   0 ronald     (501) staff       (20)     9287 2023-03-03 17:21:59.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cmsencoder.py
--rw-r--r--   0 ronald     (501) staff       (20)     9375 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cscommon.py
--rw-r--r--   0 ronald     (501) staff       (20)      190 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmaci.py
--rw-r--r--   0 ronald     (501) staff       (20)    13715 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmapi.py
--rw-r--r--   0 ronald     (501) staff       (20)    31040 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmapple.py
--rw-r--r--   0 ronald     (501) staff       (20)      190 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmcli.py
--rw-r--r--   0 ronald     (501) staff       (20)      192 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmcspi.py
--rw-r--r--   0 ronald     (501) staff       (20)      190 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmdli.py
--rw-r--r--   0 ronald     (501) staff       (20)    38915 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmerr.py
--rw-r--r--   0 ronald     (501) staff       (20)     2387 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmkrapi.py
--rw-r--r--   0 ronald     (501) staff       (20)      192 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmkrspi.py
--rw-r--r--   0 ronald     (501) staff       (20)      743 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmspi.py
--rw-r--r--   0 ronald     (501) staff       (20)      190 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmtpi.py
--rw-r--r--   0 ronald     (501) staff       (20)    58895 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmtype.py
--rw-r--r--   0 ronald     (501) staff       (20)      621 2021-10-18 19:38:40.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_emmspi.h
--rw-r--r--   0 ronald     (501) staff       (20)      346 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_emmtype.py
--rw-r--r--   0 ronald     (501) staff       (20)      421 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_mds.py
--rw-r--r--   0 ronald     (501) staff       (20)     9878 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_mds_schema.py
--rw-r--r--   0 ronald     (501) staff       (20)     9558 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_oidsalg.py
--rw-r--r--   0 ronald     (501) staff       (20)    11655 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_oidsattr.py
--rw-r--r--   0 ronald     (501) staff       (20)    11221 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_oidscert.py
--rw-r--r--   0 ronald     (501) staff       (20)     4030 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_oidscrl.py
--rw-r--r--   0 ronald     (501) staff       (20)     5375 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secaccess.py
--rw-r--r--   0 ronald     (501) staff       (20)     1823 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secaccesscontrol.py
--rw-r--r--   0 ronald     (501) staff       (20)     3353 2023-03-03 17:21:59.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secacl.py
--rw-r--r--   0 ronald     (501) staff       (20)    32514 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secbase.py
--rw-r--r--   0 ronald     (501) staff       (20)    10813 2021-04-09 10:15:21.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_seccertificate.py
--rw-r--r--   0 ronald     (501) staff       (20)     9266 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_seccertificateoids.py
--rw-r--r--   0 ronald     (501) staff       (20)     8098 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_seccode.py
--rw-r--r--   0 ronald     (501) staff       (20)     2322 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_seccodehost.py
--rw-r--r--   0 ronald     (501) staff       (20)     6219 2021-08-04 10:00:48.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_seccustomtransform.py
--rw-r--r--   0 ronald     (501) staff       (20)      678 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secdecodetransform.py
--rw-r--r--   0 ronald     (501) staff       (20)     1588 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secdigesttransform.py
--rw-r--r--   0 ronald     (501) staff       (20)     1063 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secencodetransform.py
--rw-r--r--   0 ronald     (501) staff       (20)     2545 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secencrypttransform.py
--rw-r--r--   0 ronald     (501) staff       (20)     3655 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secidentity.py
--rw-r--r--   0 ronald     (501) staff       (20)      347 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secidentitysearch.py
--rw-r--r--   0 ronald     (501) staff       (20)     4970 2022-01-02 11:04:26.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secimporterexporter.py
--rw-r--r--   0 ronald     (501) staff       (20)    12604 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secitem.py
--rw-r--r--   0 ronald     (501) staff       (20)    21429 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_seckey.py
--rw-r--r--   0 ronald     (501) staff       (20)    20218 2022-01-02 11:04:26.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_seckeychain.py
--rw-r--r--   0 ronald     (501) staff       (20)     6292 2021-04-09 10:15:21.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_seckeychainitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      435 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_seckeychainsearch.py
--rw-r--r--   0 ronald     (501) staff       (20)     4904 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secpolicy.py
--rw-r--r--   0 ronald     (501) staff       (20)      411 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secpolicysearch.py
--rw-r--r--   0 ronald     (501) staff       (20)     3626 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secprotocolmetadata.py
--rw-r--r--   0 ronald     (501) staff       (20)      249 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secprotocolobject.py
--rw-r--r--   0 ronald     (501) staff       (20)     3293 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secprotocoloptions.py
--rw-r--r--   0 ronald     (501) staff       (20)     5114 2021-04-09 10:15:21.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secprotocoltypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      898 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secrandom.py
--rw-r--r--   0 ronald     (501) staff       (20)     2955 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secrequirement.py
--rw-r--r--   0 ronald     (501) staff       (20)      545 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secsharedcredential.py
--rw-r--r--   0 ronald     (501) staff       (20)     1376 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secsignverifytransform.py
--rw-r--r--   0 ronald     (501) staff       (20)     4027 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_secstaticcode.py
--rw-r--r--   0 ronald     (501) staff       (20)     2315 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_sectask.py
--rw-r--r--   0 ronald     (501) staff       (20)     5718 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_sectransform.py
--rw-r--r--   0 ronald     (501) staff       (20)      558 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_sectransformreadtransform.py
--rw-r--r--   0 ronald     (501) staff       (20)    10517 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_sectrust.py
--rw-r--r--   0 ronald     (501) staff       (20)     1612 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_sectrustedapplication.py
--rw-r--r--   0 ronald     (501) staff       (20)     5252 2021-04-09 10:15:21.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_sectrustsettings.py
--rw-r--r--   0 ronald     (501) staff       (20)     4626 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_securedownload.py
--rw-r--r--   0 ronald     (501) staff       (20)    27653 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_securetransport.py
--rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_security.py
--rw-r--r--   0 ronald     (501) staff       (20)     3790 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.1b1/PyObjCTest/test_x509defs.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:14.337387 pyobjc-framework-Security-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)   189360 2022-04-12 09:34:36.000000 pyobjc-framework-Security-9.1b1/metadata/Security.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1036 2021-08-04 10:01:02.000000 pyobjc-framework-Security-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:39:14.379887 pyobjc-framework-Security-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   184761 2021-08-04 10:01:04.000000 pyobjc-framework-Security-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   186270 2022-02-24 08:47:17.000000 pyobjc-framework-Security-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   192578 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   193048 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   184762 2021-08-04 10:01:04.000000 pyobjc-framework-Security-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   186271 2022-02-24 08:47:17.000000 pyobjc-framework-Security-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   192579 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   193049 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Security-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:39:14.396103 pyobjc-framework-Security-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      827 2023-03-25 14:20:32.000000 pyobjc-framework-Security-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:37.027731 pyobjc-framework-Security-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:36.884886 pyobjc-framework-Security-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:36.891880 pyobjc-framework-Security-9.2/Lib/Security/
+-rw-r--r--   0 ronald     (501) staff       (20)     1655 2023-05-04 11:00:07.000000 pyobjc-framework-Security-9.2/Lib/Security/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)   128108 2023-05-27 09:46:33.000000 pyobjc-framework-Security-9.2/Lib/Security/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:36.895775 pyobjc-framework-Security-9.2/Lib/pyobjc_framework_Security.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2092 2023-06-07 00:27:36.000000 pyobjc-framework-Security-9.2/Lib/pyobjc_framework_Security.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     3080 2023-06-07 00:27:36.000000 pyobjc-framework-Security-9.2/Lib/pyobjc_framework_Security.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:27:36.000000 pyobjc-framework-Security-9.2/Lib/pyobjc_framework_Security.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:50:34.000000 pyobjc-framework-Security-9.2/Lib/pyobjc_framework_Security.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:27:36.000000 pyobjc-framework-Security-9.2/Lib/pyobjc_framework_Security.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:27:36.000000 pyobjc-framework-Security-9.2/Lib/pyobjc_framework_Security.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Security-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-Security-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:36.898656 pyobjc-framework-Security-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)    27969 2023-04-03 12:55:10.000000 pyobjc-framework-Security-9.2/Modules/_Security.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-Security-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1881 2023-06-07 00:27:37.027323 pyobjc-framework-Security-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:36.985723 pyobjc-framework-Security-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-Security-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5419 2022-02-24 08:47:17.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_authorization.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2563 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_authorizationdb.py
+-rw-r--r--   0 ronald     (501) staff       (20)      740 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_authorizationtags.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1736 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_authsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5631 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_certextensions.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13224 2021-04-09 10:15:21.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_ciphersuite.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7969 2023-05-27 09:46:33.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cmsdecoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9287 2023-03-03 17:21:59.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cmsencoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9375 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cscommon.py
+-rw-r--r--   0 ronald     (501) staff       (20)      190 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cssmaci.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13715 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cssmapi.py
+-rw-r--r--   0 ronald     (501) staff       (20)    31040 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cssmapple.py
+-rw-r--r--   0 ronald     (501) staff       (20)      190 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cssmcli.py
+-rw-r--r--   0 ronald     (501) staff       (20)      192 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cssmcspi.py
+-rw-r--r--   0 ronald     (501) staff       (20)      190 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cssmdli.py
+-rw-r--r--   0 ronald     (501) staff       (20)    38915 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cssmerr.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2387 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cssmkrapi.py
+-rw-r--r--   0 ronald     (501) staff       (20)      192 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cssmkrspi.py
+-rw-r--r--   0 ronald     (501) staff       (20)      743 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cssmspi.py
+-rw-r--r--   0 ronald     (501) staff       (20)      190 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cssmtpi.py
+-rw-r--r--   0 ronald     (501) staff       (20)    58895 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_cssmtype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      621 2021-10-18 19:38:40.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_emmspi.h
+-rw-r--r--   0 ronald     (501) staff       (20)      346 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_emmtype.py
+-rw-r--r--   0 ronald     (501) staff       (20)      421 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_mds.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9878 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_mds_schema.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9558 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_oidsalg.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11655 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_oidsattr.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11221 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_oidscert.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4030 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_oidscrl.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5375 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secaccess.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1823 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secaccesscontrol.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3353 2023-03-03 17:21:59.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secacl.py
+-rw-r--r--   0 ronald     (501) staff       (20)    32514 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secbase.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10813 2021-04-09 10:15:21.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_seccertificate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9331 2023-05-04 11:00:07.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_seccertificateoids.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8186 2023-05-04 11:00:07.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_seccode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2322 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_seccodehost.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6219 2021-08-04 10:00:48.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_seccustomtransform.py
+-rw-r--r--   0 ronald     (501) staff       (20)      678 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secdecodetransform.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1588 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secdigesttransform.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1063 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secencodetransform.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2608 2023-05-04 11:00:07.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secencrypttransform.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3655 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secidentity.py
+-rw-r--r--   0 ronald     (501) staff       (20)      347 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secidentitysearch.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4970 2022-01-02 11:04:26.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secimporterexporter.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12604 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)    21429 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_seckey.py
+-rw-r--r--   0 ronald     (501) staff       (20)    20218 2022-01-02 11:04:26.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_seckeychain.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6292 2021-04-09 10:15:21.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_seckeychainitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      435 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_seckeychainsearch.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4904 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secpolicy.py
+-rw-r--r--   0 ronald     (501) staff       (20)      411 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secpolicysearch.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3626 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secprotocolmetadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      249 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secprotocolobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3293 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secprotocoloptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5114 2021-04-09 10:15:21.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secprotocoltypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      898 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secrandom.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2955 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secrequirement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      545 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secsharedcredential.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1376 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secsignverifytransform.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4027 2021-07-30 09:00:38.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_secstaticcode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2315 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_sectask.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5718 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_sectransform.py
+-rw-r--r--   0 ronald     (501) staff       (20)      558 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_sectransformreadtransform.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10517 2023-05-04 11:00:07.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_sectrust.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1612 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_sectrustedapplication.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5252 2021-04-09 10:15:21.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_sectrustsettings.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4626 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_securedownload.py
+-rw-r--r--   0 ronald     (501) staff       (20)    27653 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_securetransport.py
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_security.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3790 2021-03-21 10:08:23.000000 pyobjc-framework-Security-9.2/PyObjCTest/test_x509defs.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:37.004153 pyobjc-framework-Security-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)   189444 2023-05-27 09:46:33.000000 pyobjc-framework-Security-9.2/metadata/Security.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1036 2021-08-04 10:01:02.000000 pyobjc-framework-Security-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:27:37.025556 pyobjc-framework-Security-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   184761 2021-08-04 10:01:04.000000 pyobjc-framework-Security-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   186270 2022-02-24 08:47:17.000000 pyobjc-framework-Security-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   192578 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   193048 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   184762 2021-08-04 10:01:04.000000 pyobjc-framework-Security-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   186271 2022-02-24 08:47:17.000000 pyobjc-framework-Security-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   192579 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   193049 2023-02-19 10:50:35.000000 pyobjc-framework-Security-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Security-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Security-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:27:37.027841 pyobjc-framework-Security-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      909 2023-05-29 10:07:47.000000 pyobjc-framework-Security-9.2/setup.py
```

### Comparing `pyobjc-framework-Security-9.1b1/Lib/Security/_metadata.py` & `pyobjc-framework-Security-9.2/Lib/Security/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sat Feb 18 12:55:35 2023
+# Last update: Sat May 20 22:11:20 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -461,15 +461,14 @@
                     "null_accepted": True,
                     "already_cfretained": True,
                     "type_modifier": "o",
                 }
             }
         },
     ),
-    "SecACLGetTypeID": (sel32or64(b"I", b"Q"),),
     "SecTrustSettingsSetTrustSettings": (b"i@I@",),
     "SecKeyCopyExternalRepresentation": (
         b"@@o^@",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "SecTransformCreateGroupTransform": (
@@ -495,19 +494,15 @@
                 }
             },
         },
     ),
     "SSLGetBufferedReadSize": (b"i@o^L",),
     "SecTrustSetVerifyDate": (b"i@@",),
     "sec_trust_copy_ref": (b"@@", "", {"retval": {"already_cfretained": True}}),
-    "SecKeychainItemCreateFromContent": (
-        b"iI^{SecKeychainAttributeList=I^{SecKeychainAttribute=II^v}}I^v^{__SecKeychain=}^{__SecAccess=}^^{__SecKeychainItem=}",
-        "",
-        {"retval": {"already_cfretained": True}},
-    ),
+    "SecACLGetTypeID": (sel32or64(b"I", b"Q"),),
     "SSLContextGetTypeID": (sel32or64(b"I", b"Q"),),
     "SessionCreate": (b"iII", "", {"retval": {"already_cfretained": True}}),
     "sec_identity_access_certificates": (
         b"B@@?",
         "",
         {
             "arguments": {
@@ -566,15 +561,14 @@
         {
             "arguments": {
                 1: {"already_cfretained": True},
                 2: {"already_cfretained": True},
             }
         },
     ),
-    "SecKeychainGetDLDBHandle": (b"i^{__SecKeychain=}^{cssm_dl_db_handle=qq}",),
     "SecCodeMapMemory": (b"i@I",),
     "CMSDecoderCopyContent": (
         b"i@o^@",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {1: {"already_cfretained": True}},
@@ -796,15 +790,15 @@
     ),
     "SecureDownloadCopyURLs": (
         b"i^{OpaqueSecureDownload=}o^@",
         "",
         {"arguments": {1: {"already_cfretained": True}}},
     ),
     "CMSEncoderAddRecipients": (b"i@@",),
-    "SecKeychainGetCSPHandle": (b"i^{__SecKeychain=}^q",),
+    "sec_protocol_options_set_tls_is_fallback_attempt": (b"vBB",),
     "SecTrustCopyPublicKey": (b"@@", "", {"retval": {"already_cfretained": True}}),
     "SecKeyCreateWithData": (b"@@@o^@", "", {"retval": {"already_cfretained": True}}),
     "sec_protocol_metadata_get_negotiated_tls_protocol_version": (b"S@",),
     "SecKeychainDelete": (b"i@",),
     "sec_identity_copy_certificates_ref": (
         b"@@",
         "",
@@ -964,17 +958,24 @@
         },
     ),
     "SecCertificateCopyData": (b"@@", "", {"retval": {"already_cfretained": True}}),
     "sec_protocol_options_set_tls_max_version": (b"v@i",),
     "SecKeyGenerateSymmetric": (b"@@o^@", "", {"retval": {"already_cfretained": True}}),
     "SecHostSetGuestStatus": (b"iII@I",),
     "CMSDecoderCopySignerStatus": (
-        b"i@L@Zo^Io^i^i",
+        b"i^{_CMSDecoder=}Q@Z^I^^{__SecTrust=}^i",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {
+                4: {"type_modifier": "o"},
+                5: {"type_modifier": "o"},
+                6: {"type_modifier": "o"},
+            },
+        },
     ),
     "SecTrustCopyCustomAnchorCertificates": (
         b"i@o^@",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {1: {"already_cfretained": True}},
@@ -1680,15 +1681,14 @@
         {
             "retval": {"already_cfretained": True},
             "arguments": {2: {"already_cfretained": True}},
         },
     ),
     "SecKeychainSetDomainSearchList": (b"ii@",),
     "sec_protocol_options_set_tls_diffie_hellman_parameters": (b"v@@",),
-    "sec_protocol_options_set_tls_is_fallback_attempt": (b"vBB",),
     "SecRequirementCopyString": (
         b"i@Io^@",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {2: {"already_cfretained": True}},
         },
```

### Comparing `pyobjc-framework-Security-9.1b1/Lib/pyobjc_framework_Security.egg-info/PKG-INFO` & `pyobjc-framework-Security-9.2/Lib/pyobjc_framework_Security.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Security
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Security on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Security
 Platform: MacOS X
```

### Comparing `pyobjc-framework-Security-9.1b1/Lib/pyobjc_framework_Security.egg-info/SOURCES.txt` & `pyobjc-framework-Security-9.2/Lib/pyobjc_framework_Security.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/Security/__init__.py
 Lib/Security/_metadata.py
 Lib/pyobjc_framework_Security.egg-info/PKG-INFO
 Lib/pyobjc_framework_Security.egg-info/SOURCES.txt
 Lib/pyobjc_framework_Security.egg-info/dependency_links.txt
 Lib/pyobjc_framework_Security.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-Security-9.1b1/License.txt` & `pyobjc-framework-Security-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/Modules/_Security.m` & `pyobjc-framework-Security-9.2/Modules/_Security.m`

 * *Files 1% similar despite different names*

```diff
@@ -69,29 +69,29 @@
     serverName_token =
         PyObjC_PythonToCArray(NO, NO, &string, py_serverName, (void**)&serverName,
                               &serverName_length, &serverName_buffer, &serverName_view);
     if (serverName_token == -1) {
         return NULL;
     }
 
-    if (py_securityDomain == Py_None) {
+    if (py_securityDomain == Py_None || py_securityDomain == PyObjC_NULL) {
         securityDomain = NULL;
 
     } else {
         securityDomain_token = PyObjC_PythonToCArray(
             NO, NO, &string, py_securityDomain, (void**)&securityDomain,
             &securityDomain_length, &securityDomain_buffer, &securityDomain_view);
         if (securityDomain_token == -1) {
             PyObjC_FreeCArray(serverName_token, &serverName_view);
             Py_XDECREF(serverName_buffer);
             return NULL;
         }
     }
 
-    if (py_accountName == Py_None) {
+    if (py_accountName == Py_None || py_accountName == PyObjC_NULL) {
         accountName = NULL;
     } else {
         accountName_token = PyObjC_PythonToCArray(
             NO, NO, &string, py_accountName, (void**)&accountName, &accountName_length,
             &accountName_buffer, &accountName_view);
         if (accountName_token == -1) {
             PyObjC_FreeCArray(serverName_token, &serverName_view);
@@ -99,15 +99,15 @@
             if (py_securityDomain != NULL)
                 PyObjC_FreeCArray(securityDomain_token, &securityDomain_view);
             Py_XDECREF(securityDomain_buffer);
             return NULL;
         }
     }
 
-    if (py_path == NULL) {
+    if (py_path == Py_None || py_path == PyObjC_NULL) {
         path = NULL;
     } else {
         path_token = PyObjC_PythonToCArray(NO, NO, &string, py_path, (void**)&path,
                                            &path_length, &path_buffer, &path_view);
         if (path_token == -1) {
             PyObjC_FreeCArray(serverName_token, &serverName_view);
             Py_XDECREF(serverName_buffer);
@@ -256,15 +256,15 @@
     serviceName_token = PyObjC_PythonToCArray(NO, NO, &string, py_serviceName,
                                               (void**)&serviceName, &serviceName_length,
                                               &serviceName_buffer, &serviceName_view);
     if (serviceName_token == -1) {
         return NULL;
     }
 
-    if (py_accountName == Py_None) {
+    if (py_accountName == Py_None || py_accountName == PyObjC_NULL) {
         accountName = NULL;
     } else {
         accountName_token = PyObjC_PythonToCArray(
             NO, NO, &string, py_accountName, (void**)&accountName, &accountName_length,
             &accountName_buffer, &accountName_view);
         if (accountName_token == -1) {
             PyObjC_FreeCArray(serviceName_token, &serviceName_view);
```

### Comparing `pyobjc-framework-Security-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-Security-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-Security-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-Security-9.1b1/PKG-INFO` & `pyobjc-framework-Security-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Security
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework Security on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Security
 Platform: MacOS X
```

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_authorization.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_authorization.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_authorizationdb.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_authorizationdb.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_authorizationtags.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_authorizationtags.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_authsession.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_authsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_certextensions.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_certextensions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_ciphersuite.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_ciphersuite.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_cmsdecoder.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_cmsdecoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,28 +57,21 @@
         self.assertArgHasType(
             Security.CMSDecoderGetNumSigners,
             1,
             objc._C_OUT + objc._C_PTR + objc._C_ULNG,
         )
 
         self.assertResultHasType(Security.CMSDecoderCopySignerStatus, objc._C_INT)
-        self.assertArgHasType(Security.CMSDecoderCopySignerStatus, 0, objc._C_ID)
+        # self.assertArgHasType(Security.CMSDecoderCopySignerStatus, 0, objc._C_ID)
         self.assertArgHasType(Security.CMSDecoderCopySignerStatus, 1, objc._C_ULNG)
         self.assertArgHasType(Security.CMSDecoderCopySignerStatus, 2, objc._C_ID)
         self.assertArgHasType(Security.CMSDecoderCopySignerStatus, 3, objc._C_NSBOOL)
-        self.assertArgHasType(
-            Security.CMSDecoderCopySignerStatus,
-            4,
-            objc._C_OUT + objc._C_PTR + objc._C_UINT,
-        )
-        self.assertArgHasType(
-            Security.CMSDecoderCopySignerStatus,
-            5,
-            objc._C_OUT + objc._C_PTR + objc._C_INT,
-        )
+        self.assertArgIsOut(Security.CMSDecoderCopySignerStatus, 4)
+        self.assertArgIsOut(Security.CMSDecoderCopySignerStatus, 5)
+        self.assertArgIsOut(Security.CMSDecoderCopySignerStatus, 6)
 
         self.assertResultHasType(Security.CMSDecoderGetNumSigners, objc._C_INT)
         self.assertArgHasType(Security.CMSDecoderGetNumSigners, 0, objc._C_ID)
         self.assertArgHasType(
             Security.CMSDecoderGetNumSigners,
             1,
             objc._C_OUT + objc._C_PTR + objc._C_ULNG,
```

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_cmsencoder.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_cmsencoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_cscommon.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_cscommon.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmapi.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_cssmapi.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmapple.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_cssmapple.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmerr.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_cssmerr.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmkrapi.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_cssmkrapi.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmspi.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_cssmspi.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_cssmtype.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_cssmtype.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_emmspi.h` & `pyobjc-framework-Security-9.2/PyObjCTest/test_emmspi.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_mds_schema.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_mds_schema.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_oidsalg.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_oidsalg.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_oidsattr.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_oidsattr.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_oidscert.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_oidscert.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_oidscrl.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_oidscrl.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secaccess.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secaccess.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secaccesscontrol.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secaccesscontrol.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secacl.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secacl.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secbase.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secbase.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_seccertificate.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_seccertificate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_seccertificateoids.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_seccertificateoids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import Security
-from PyObjCTools.TestSupport import TestCase, min_os_level
+from PyObjCTools.TestSupport import TestCase, min_os_level, expectedFailure
 
 
 class TestSecCertificateOIDs(TestCase):
     def test_constants(self):
         self.assertIsInstance(Security.kSecOIDADC_CERT_POLICY, str)
         self.assertIsInstance(Security.kSecOIDAPPLE_CERT_POLICY, str)
         self.assertIsInstance(Security.kSecOIDAPPLE_EKU_CODE_SIGNING, str)
@@ -119,16 +119,18 @@
         self.assertIsInstance(Security.kSecOIDX509V3CertificateExtensionValue, str)
         self.assertIsInstance(Security.kSecOIDX509V3CertificateExtensionsCStruct, str)
         self.assertIsInstance(Security.kSecOIDX509V3CertificateExtensionsStruct, str)
         self.assertIsInstance(Security.kSecOIDX509V3CertificateNumberOfExtensions, str)
         self.assertIsInstance(Security.kSecOIDX509V3SignedCertificate, str)
         self.assertIsInstance(Security.kSecOIDX509V3SignedCertificateCStruct, str)
 
+    @expectedFailure
     @min_os_level("10.7")
     def test_constants_missing(self):
+        # Missing on 10.11
         self.assertIsInstance(Security.kSecOIDAPPLE_EXTENSION_INTERMEDIATE_MARKER, str)
         self.assertIsInstance(Security.kSecOIDAPPLE_EXTENSION_WWDR_INTERMEDIATE, str)
         self.assertIsInstance(Security.kSecOIDAPPLE_EXTENSION_ITMS_INTERMEDIATE, str)
         self.assertIsInstance(Security.kSecOIDAPPLE_EXTENSION_AAI_INTERMEDIATE, str)
         self.assertIsInstance(Security.kSecOIDAPPLE_EXTENSION_APPLEID_INTERMEDIATE, str)
 
     @min_os_level("10.8")
```

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_seccode.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_seccode.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,43 +32,47 @@
         self.assertIsInstance(Security.kSecCodeInfoEntitlements, str)
         self.assertIsInstance(Security.kSecCodeInfoEntitlementsDict, str)
         self.assertIsInstance(Security.kSecCodeInfoFlags, str)
         self.assertIsInstance(Security.kSecCodeInfoFormat, str)
         self.assertIsInstance(Security.kSecCodeInfoDigestAlgorithm, str)
         self.assertIsInstance(Security.kSecCodeInfoIdentifier, str)
         self.assertIsInstance(Security.kSecCodeInfoImplicitDesignatedRequirement, str)
-        self.assertIsInstance(
-            Security.kSecCodeInfoDefaultDesignatedLightweightCodeRequirement, str
-        )
         self.assertIsInstance(Security.kSecCodeInfoMainExecutable, str)
         self.assertIsInstance(Security.kSecCodeInfoPList, str)
         self.assertIsInstance(Security.kSecCodeInfoRequirements, str)
         self.assertIsInstance(Security.kSecCodeInfoRequirementData, str)
         self.assertIsInstance(Security.kSecCodeInfoSource, str)
         self.assertIsInstance(Security.kSecCodeInfoStatus, str)
         self.assertIsInstance(Security.kSecCodeInfoTeamIdentifier, str)
         self.assertIsInstance(Security.kSecCodeInfoTime, str)
         self.assertIsInstance(Security.kSecCodeInfoTimestamp, str)
         self.assertIsInstance(Security.kSecCodeInfoTrust, str)
         self.assertIsInstance(Security.kSecCodeInfoUnique, str)
 
+    @min_os_level("10.12")
     def test_constants_missing(self):
         self.assertIsInstance(Security.kSecGuestAttributeArchitecture, str)
         self.assertIsInstance(Security.kSecGuestAttributeSubarchitecture, str)
         self.assertIsInstance(Security.kSecCodeInfoPlatformIdentifier, str)
 
     @min_os_level("10.11.4")
     def test_constants_10_11_4(self):
         self.assertIsInstance(Security.kSecCodeInfoDigestAlgorithms, str)
         self.assertIsInstance(Security.kSecCodeInfoCdHashes, str)
 
     @min_os_level("10.12")
     def test_constants_10_12(self):
         self.assertIsInstance(Security.kSecGuestAttributeAudit, str)
 
+    @min_os_level("13.0")
+    def test_constants13_0(self):
+        self.assertIsInstance(
+            Security.kSecCodeInfoDefaultDesignatedLightweightCodeRequirement, str
+        )
+
     def test_functions(self):
         self.assertIsInstance(Security.SecCodeGetTypeID(), int)
 
         self.assertResultHasType(Security.SecCodeCopySelf, objc._C_INT)
         self.assertArgHasType(Security.SecCodeCopySelf, 0, objc._C_UINT)
         self.assertArgHasType(
             Security.SecCodeCopySelf, 1, objc._C_OUT + objc._C_PTR + objc._C_ID
```

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_seccodehost.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_seccodehost.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_seccustomtransform.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_seccustomtransform.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secdecodetransform.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secdecodetransform.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secdigesttransform.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secdigesttransform.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secencodetransform.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secencodetransform.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secencrypttransform.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secencrypttransform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import Security
-from PyObjCTools.TestSupport import TestCase, min_os_level
+from PyObjCTools.TestSupport import TestCase, min_os_level, expectedFailure
 import objc
 
 
 class TestSecEncryptTransform(TestCase):
     def test_constants(self):
         self.assertIsInstance(Security.kSecPaddingNoneKey, str)
         self.assertIsInstance(Security.kSecPaddingPKCS1Key, str)
@@ -20,16 +20,18 @@
         self.assertIsInstance(Security.kSecIVKey, str)
         self.assertIsInstance(Security.kSecEncryptionMode, str)
 
     @min_os_level("10.8")
     def test_constants10_8(self):
         self.assertIsInstance(Security.kSecOAEPEncodingParametersAttributeName, str)
 
+    @expectedFailure
     @min_os_level("10.8")
     def test_constants10_8_missing(self):
+        # Fails on 10.11
         self.assertIsInstance(Security.kSecOAEPMessageLengthAttributeName, str)
         self.assertIsInstance(Security.kSecOAEPMGF1DigestAlgorithmAttributeName, str)
 
     @min_os_level("10.7")
     def test_functions(self):
         self.assertResultHasType(Security.SecEncryptTransformCreate, objc._C_ID)
         self.assertResultIsCFRetained(Security.SecEncryptTransformCreate)
```

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secidentity.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secidentity.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secimporterexporter.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secimporterexporter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secitem.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_seckey.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_seckey.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_seckeychain.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_seckeychain.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_seckeychainitem.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_seckeychainitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secpolicy.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secpolicy.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secprotocolmetadata.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secprotocolmetadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secprotocoloptions.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secprotocoloptions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secprotocoltypes.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secprotocoltypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secrandom.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secrandom.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secrequirement.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secrequirement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secsharedcredential.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secsharedcredential.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secsignverifytransform.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secsignverifytransform.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_secstaticcode.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_secstaticcode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_sectask.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_sectask.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_sectransform.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_sectransform.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_sectransformreadtransform.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_sectransformreadtransform.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_sectrust.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_sectrust.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.assertIsInstance(Security.kSecTrustEvaluationDate, str)
         self.assertIsInstance(Security.kSecTrustExtendedValidation, str)
         self.assertIsInstance(Security.kSecTrustOrganizationName, str)
         self.assertIsInstance(Security.kSecTrustResultValue, str)
         self.assertIsInstance(Security.kSecTrustRevocationChecked, str)
         self.assertIsInstance(Security.kSecTrustRevocationValidUntilDate, str)
 
-    @min_os_level("10.11")
+    @min_os_level("10.12")
     def test_constants10_11(self):
         self.assertIsInstance(Security.kSecTrustCertificateTransparency, str)
 
     @min_os_level("10.12")
     def test_constants10_12(self):
         self.assertIsInstance(Security.kSecTrustCertificateTransparencyWhiteList, str)
```

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_sectrustedapplication.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_sectrustedapplication.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_sectrustsettings.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_sectrustsettings.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_securedownload.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_securedownload.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_securetransport.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_securetransport.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/PyObjCTest/test_x509defs.py` & `pyobjc-framework-Security-9.2/PyObjCTest/test_x509defs.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/metadata/Security.fwinfo` & `pyobjc-framework-Security-9.2/metadata/Security.fwinfo`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998040787852431%*

 * *Differences: {"'definitions'": "{'functions': {'CMSDecoderCopySignerStatus': {'args': {'4': {replace: "*

 * *                  "OrderedDict([('type_modifier', 'o')])}, '5': {replace: "*

 * *                  "OrderedDict([('type_modifier', 'o')])}, '6': OrderedDict([('type_modifier', "*

 * *                  "'o')]), delete: ['0', '1', '2']}}, 'SecKeychainItemCreateFromContent': "*

 * *                  "OrderedDict([('ignore', True)]), 'SecKeychainGetCSPHandle': "*

 * *                  "OrderedDict([('ignore', True)]), 'SecKeychainGetDLDBHand […]*

```diff
@@ -5689,31 +5689,25 @@
                 },
                 "retval": {
                     "type_override": "i"
                 }
             },
             "CMSDecoderCopySignerStatus": {
                 "args": {
-                    "0": {
-                        "type_override": "@"
-                    },
-                    "1": {
-                        "type_override": "L"
-                    },
-                    "2": {
-                        "type_override": "@"
-                    },
                     "3": {
                         "type_override": "Z"
                     },
                     "4": {
-                        "type_override": "o^I"
+                        "type_modifier": "o"
                     },
                     "5": {
-                        "type_override": "o^i"
+                        "type_modifier": "o"
+                    },
+                    "6": {
+                        "type_modifier": "o"
                     }
                 },
                 "retval": {
                     "type_override": "i"
                 }
             },
             "CMSDecoderCopySignerTimestamp": {
@@ -8759,14 +8753,20 @@
             },
             "SecKeychainFindInternetPassword": {
                 "ignore": true
             },
             "SecKeychainFreeAttributeInfo": {
                 "ignore": true
             },
+            "SecKeychainGetCSPHandle": {
+                "ignore": true
+            },
+            "SecKeychainGetDLDBHandle": {
+                "ignore": true
+            },
             "SecKeychainGetPath": {
                 "args": {
                     "0": {
                         "type_override": "@"
                     },
                     "1": {
                         "type_override": "N^I"
@@ -8896,14 +8896,17 @@
                         "type_override": "o^@"
                     }
                 },
                 "retval": {
                     "type_override": "i"
                 }
             },
+            "SecKeychainItemCreateFromContent": {
+                "ignore": true
+            },
             "SecKeychainItemCreatePersistentReference": {
                 "args": {
                     "0": {
                         "type_override": "@"
                     },
                     "1": {
                         "already_cfretained": true,
```

### Comparing `pyobjc-framework-Security-9.1b1/metadata/metadata.ini` & `pyobjc-framework-Security-9.2/metadata/metadata.ini`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-Security-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-Security-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-Security-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-Security-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-Security-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-Security-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-Security-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-Security-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Security-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Security-9.1b1/setup.py` & `pyobjc-framework-Security-9.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 
-from pyobjc_setup import Extension, setup
+import os
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-Security",
     description="Wrappers for the framework Security on macOS",
     packages=["Security"],
     ext_modules=[
         Extension(
```

