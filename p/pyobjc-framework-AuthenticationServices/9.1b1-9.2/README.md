# Comparing `tmp/pyobjc-framework-AuthenticationServices-9.1b1.tar.gz` & `tmp/pyobjc-framework-AuthenticationServices-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-AuthenticationServices-9.1b1.tar", last modified: Sun Mar 26 11:14:56 2023, max compression
+gzip compressed data, was "pyobjc-framework-AuthenticationServices-9.2.tar", last modified: Wed Jun  7 00:06:26 2023, max compression
```

## Comparing `pyobjc-framework-AuthenticationServices-9.1b1.tar` & `pyobjc-framework-AuthenticationServices-9.2.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:56.778887 pyobjc-framework-AuthenticationServices-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:56.587832 pyobjc-framework-AuthenticationServices-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:56.598884 pyobjc-framework-AuthenticationServices-9.1b1/Lib/AuthenticationServices/
--rw-r--r--   0 ronald     (501) staff       (20)      849 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.1b1/Lib/AuthenticationServices/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    27201 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.1b1/Lib/AuthenticationServices/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:56.620504 pyobjc-framework-AuthenticationServices-9.1b1/Lib/pyobjc_framework_AuthenticationServices.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2160 2023-03-26 11:14:56.000000 pyobjc-framework-AuthenticationServices-9.1b1/Lib/pyobjc_framework_AuthenticationServices.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     3122 2023-03-26 11:14:56.000000 pyobjc-framework-AuthenticationServices-9.1b1/Lib/pyobjc_framework_AuthenticationServices.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:14:56.000000 pyobjc-framework-AuthenticationServices-9.1b1/Lib/pyobjc_framework_AuthenticationServices.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:20.000000 pyobjc-framework-AuthenticationServices-9.1b1/Lib/pyobjc_framework_AuthenticationServices.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:14:56.000000 pyobjc-framework-AuthenticationServices-9.1b1/Lib/pyobjc_framework_AuthenticationServices.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       23 2023-03-26 11:14:56.000000 pyobjc-framework-AuthenticationServices-9.1b1/Lib/pyobjc_framework_AuthenticationServices.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AuthenticationServices-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:56.626287 pyobjc-framework-AuthenticationServices-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1210 2021-10-18 19:38:40.000000 pyobjc-framework-AuthenticationServices-9.1b1/Modules/_AuthenticationServices.m
--rw-r--r--   0 ronald     (501) staff       (20)      992 2022-06-15 11:57:00.000000 pyobjc-framework-AuthenticationServices-9.1b1/Modules/_AuthenticationServices_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-AuthenticationServices-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1949 2023-03-26 11:14:56.778048 pyobjc-framework-AuthenticationServices-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:56.709249 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      494 2022-10-18 09:53:23.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_ASAuthorizationSingleSignOnRequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1018 2022-10-18 09:53:23.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asAuthorizationproviderextensionauthorizationrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      363 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorization.py
--rw-r--r--   0 ronald     (501) staff       (20)     1239 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationappleidbutton.py
--rw-r--r--   0 ronald     (501) staff       (20)      519 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationappleidcredential.py
--rw-r--r--   0 ronald     (501) staff       (20)     1131 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationappleidprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      686 2022-06-25 20:17:55.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      274 2022-06-25 20:09:08.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationcredential.py
--rw-r--r--   0 ronald     (501) staff       (20)      704 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      777 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationopenidrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      560 2022-06-25 20:17:53.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)     2872 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationproviderextensionloginconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)     2105 2022-06-15 11:57:00.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationproviderextensionloginmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     3685 2022-06-25 08:59:25.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationproviderextensionregistrationhandler.py
--rw-r--r--   0 ronald     (501) staff       (20)      319 2022-10-18 09:53:23.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationpublicKeycredentialregistration.py
--rw-r--r--   0 ronald     (501) staff       (20)     1791 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationpublickeycredentialconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)      311 2022-06-25 20:10:40.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationpublickeycredentialdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      351 2022-06-25 20:11:14.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationpublickeycredentialregistrationrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      879 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationsecuritykeypublickeycredentialdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      346 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationsinglesignonprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)     1325 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationwebbrowserpublickeycredentialmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      589 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_ascoseconstants.py
--rw-r--r--   0 ronald     (501) staff       (20)     1600 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_ascredentialidentitystore.py
--rw-r--r--   0 ronald     (501) staff       (20)      456 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_ascredentialidentitystorestate.py
--rw-r--r--   0 ronald     (501) staff       (20)      653 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_ascredentialproviderextensioncontext.py
--rw-r--r--   0 ronald     (501) staff       (20)      481 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_ascredentialserviceidentifier.py
--rw-r--r--   0 ronald     (501) staff       (20)      833 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asextensionerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)      265 2022-06-25 20:12:08.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_aspublickeycredential.py
--rw-r--r--   0 ronald     (501) staff       (20)     1714 2022-06-25 20:10:42.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_aswebauthenticationsession.py
--rw-r--r--   0 ronald     (501) staff       (20)      306 2022-06-25 20:10:08.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_aswebauthenticationsessionrequestdelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      326 2022-10-18 09:53:23.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_aswebauthenticationsessionwebbrowsersessionHandling.py
--rw-r--r--   0 ronald     (501) staff       (20)      402 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_aswebauthenticationsessionwebbrowsersessionmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      228 2022-04-11 08:03:15.000000 pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_authenticationservices.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:56.714923 pyobjc-framework-AuthenticationServices-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2944 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.1b1/metadata/AuthenticationServices.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       60 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:14:56.775352 pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   112562 2021-08-04 10:01:04.000000 pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   113837 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   146588 2022-07-30 15:06:02.000000 pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   157709 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    55016 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    73304 2021-03-21 10:08:22.000000 pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   112563 2021-08-04 10:01:04.000000 pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   113838 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   146589 2022-07-30 15:06:02.000000 pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   157710 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AuthenticationServices-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:14:56.779039 pyobjc-framework-AuthenticationServices-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1255 2023-03-25 14:20:30.000000 pyobjc-framework-AuthenticationServices-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:26.647115 pyobjc-framework-AuthenticationServices-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:26.493378 pyobjc-framework-AuthenticationServices-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:26.499650 pyobjc-framework-AuthenticationServices-9.2/Lib/AuthenticationServices/
+-rw-r--r--   0 ronald     (501) staff       (20)      849 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.2/Lib/AuthenticationServices/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    27201 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.2/Lib/AuthenticationServices/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:26.504435 pyobjc-framework-AuthenticationServices-9.2/Lib/pyobjc_framework_AuthenticationServices.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2158 2023-06-07 00:06:26.000000 pyobjc-framework-AuthenticationServices-9.2/Lib/pyobjc_framework_AuthenticationServices.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     3137 2023-06-07 00:06:26.000000 pyobjc-framework-AuthenticationServices-9.2/Lib/pyobjc_framework_AuthenticationServices.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:06:26.000000 pyobjc-framework-AuthenticationServices-9.2/Lib/pyobjc_framework_AuthenticationServices.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:20.000000 pyobjc-framework-AuthenticationServices-9.2/Lib/pyobjc_framework_AuthenticationServices.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:06:26.000000 pyobjc-framework-AuthenticationServices-9.2/Lib/pyobjc_framework_AuthenticationServices.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       23 2023-06-07 00:06:26.000000 pyobjc-framework-AuthenticationServices-9.2/Lib/pyobjc_framework_AuthenticationServices.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-AuthenticationServices-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:26.533107 pyobjc-framework-AuthenticationServices-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1210 2021-10-18 19:38:40.000000 pyobjc-framework-AuthenticationServices-9.2/Modules/_AuthenticationServices.m
+-rw-r--r--   0 ronald     (501) staff       (20)      992 2022-06-15 11:57:00.000000 pyobjc-framework-AuthenticationServices-9.2/Modules/_AuthenticationServices_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:21.000000 pyobjc-framework-AuthenticationServices-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1947 2023-06-07 00:06:26.645434 pyobjc-framework-AuthenticationServices-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:26.600339 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      494 2022-10-18 09:53:23.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_ASAuthorizationSingleSignOnRequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1018 2022-10-18 09:53:23.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asAuthorizationproviderextensionauthorizationrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      363 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorization.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1239 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationappleidbutton.py
+-rw-r--r--   0 ronald     (501) staff       (20)      519 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationappleidcredential.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1131 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationappleidprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      686 2022-06-25 20:17:55.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      274 2022-06-25 20:09:08.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationcredential.py
+-rw-r--r--   0 ronald     (501) staff       (20)      704 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      777 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationopenidrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      560 2022-06-25 20:17:53.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2872 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationproviderextensionloginconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2105 2022-06-15 11:57:00.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationproviderextensionloginmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3685 2022-06-25 08:59:25.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationproviderextensionregistrationhandler.py
+-rw-r--r--   0 ronald     (501) staff       (20)      319 2022-10-18 09:53:23.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationpublicKeycredentialregistration.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1791 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationpublickeycredentialconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)      311 2022-06-25 20:10:40.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationpublickeycredentialdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      351 2022-06-25 20:11:14.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationpublickeycredentialregistrationrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      879 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationsecuritykeypublickeycredentialdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      346 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationsinglesignonprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1325 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationwebbrowserpublickeycredentialmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      589 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_ascoseconstants.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1600 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_ascredentialidentitystore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      456 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_ascredentialidentitystorestate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      653 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_ascredentialproviderextensioncontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)      481 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_ascredentialserviceidentifier.py
+-rw-r--r--   0 ronald     (501) staff       (20)      833 2021-07-30 09:00:37.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asextensionerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)      265 2022-06-25 20:12:08.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_aspublickeycredential.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1714 2022-06-25 20:10:42.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_aswebauthenticationsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)      306 2022-06-25 20:10:08.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_aswebauthenticationsessionrequestdelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      326 2022-10-18 09:53:23.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_aswebauthenticationsessionwebbrowsersessionHandling.py
+-rw-r--r--   0 ronald     (501) staff       (20)      402 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_aswebauthenticationsessionwebbrowsersessionmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      228 2022-04-11 08:03:15.000000 pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_authenticationservices.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:26.602593 pyobjc-framework-AuthenticationServices-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2944 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.2/metadata/AuthenticationServices.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       60 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:06:26.643483 pyobjc-framework-AuthenticationServices-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   112562 2021-08-04 10:01:04.000000 pyobjc-framework-AuthenticationServices-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   113837 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   146588 2022-07-30 15:06:02.000000 pyobjc-framework-AuthenticationServices-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   157709 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    55016 2020-11-30 18:45:14.000000 pyobjc-framework-AuthenticationServices-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    73304 2021-03-21 10:08:22.000000 pyobjc-framework-AuthenticationServices-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   112563 2021-08-04 10:01:04.000000 pyobjc-framework-AuthenticationServices-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   113838 2022-02-24 08:47:16.000000 pyobjc-framework-AuthenticationServices-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   146589 2022-07-30 15:06:02.000000 pyobjc-framework-AuthenticationServices-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   157710 2023-02-19 10:50:34.000000 pyobjc-framework-AuthenticationServices-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-AuthenticationServices-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-AuthenticationServices-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:06:26.647223 pyobjc-framework-AuthenticationServices-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1326 2023-05-29 10:07:45.000000 pyobjc-framework-AuthenticationServices-9.2/setup.py
```

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/Lib/AuthenticationServices/__init__.py` & `pyobjc-framework-AuthenticationServices-9.2/Lib/AuthenticationServices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/Lib/AuthenticationServices/_metadata.py` & `pyobjc-framework-AuthenticationServices-9.2/Lib/AuthenticationServices/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/Lib/pyobjc_framework_AuthenticationServices.egg-info/PKG-INFO` & `pyobjc-framework-AuthenticationServices-9.2/Lib/pyobjc_framework_AuthenticationServices.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AuthenticationServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AuthenticationServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AuthenticationServices
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/Lib/pyobjc_framework_AuthenticationServices.egg-info/SOURCES.txt` & `pyobjc-framework-AuthenticationServices-9.2/Lib/pyobjc_framework_AuthenticationServices.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/AuthenticationServices/__init__.py
 Lib/AuthenticationServices/_metadata.py
 Lib/pyobjc_framework_AuthenticationServices.egg-info/PKG-INFO
 Lib/pyobjc_framework_AuthenticationServices.egg-info/SOURCES.txt
 Lib/pyobjc_framework_AuthenticationServices.egg-info/dependency_links.txt
 Lib/pyobjc_framework_AuthenticationServices.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/License.txt` & `pyobjc-framework-AuthenticationServices-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/Modules/_AuthenticationServices.m` & `pyobjc-framework-AuthenticationServices-9.2/Modules/_AuthenticationServices.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/Modules/_AuthenticationServices_protocols.m` & `pyobjc-framework-AuthenticationServices-9.2/Modules/_AuthenticationServices_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-AuthenticationServices-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-AuthenticationServices-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PKG-INFO` & `pyobjc-framework-AuthenticationServices-9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-AuthenticationServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework AuthenticationServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,AuthenticationServices
 Platform: MacOS X (>=10.15)
```

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asAuthorizationproviderextensionauthorizationrequest.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asAuthorizationproviderextensionauthorizationrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationappleidbutton.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationappleidbutton.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationappleidcredential.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationappleidcredential.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationappleidprovider.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationappleidprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationcontroller.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationerror.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationopenidrequest.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationopenidrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationprovider.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationproviderextensionloginconfiguration.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationproviderextensionloginconfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationproviderextensionloginmanager.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationproviderextensionloginmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationproviderextensionregistrationhandler.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationproviderextensionregistrationhandler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationpublickeycredentialconstants.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationpublickeycredentialconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationsecuritykeypublickeycredentialdescriptor.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationsecuritykeypublickeycredentialdescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asauthorizationwebbrowserpublickeycredentialmanager.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asauthorizationwebbrowserpublickeycredentialmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_ascoseconstants.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_ascoseconstants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_ascredentialidentitystore.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_ascredentialidentitystore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_ascredentialproviderextensioncontext.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_ascredentialproviderextensioncontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_asextensionerrors.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_asextensionerrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/PyObjCTest/test_aswebauthenticationsession.py` & `pyobjc-framework-AuthenticationServices-9.2/PyObjCTest/test_aswebauthenticationsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/metadata/AuthenticationServices.fwinfo` & `pyobjc-framework-AuthenticationServices-9.2/metadata/AuthenticationServices.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-AuthenticationServices-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-AuthenticationServices-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-AuthenticationServices-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-AuthenticationServices-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-AuthenticationServices-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-AuthenticationServices-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-AuthenticationServices-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-AuthenticationServices-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-AuthenticationServices-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-AuthenticationServices-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/pyobjc_setup.py` & `pyobjc-framework-AuthenticationServices-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-AuthenticationServices-9.1b1/setup.py` & `pyobjc-framework-AuthenticationServices-9.2/setup.py`

 * *Files 16% similar despite different names*

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
     name="pyobjc-framework-AuthenticationServices",
     description="Wrappers for the framework AuthenticationServices on macOS",
     min_os_level="10.15",
     packages=["AuthenticationServices"],
     ext_modules=[
```

