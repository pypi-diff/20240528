# Comparing `tmp/collabconnector-0.1.1716909176.tar.gz` & `tmp/collabconnector-0.1.1716921273.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collabconnector-0.1.1716909176.tar", last modified: Tue May 28 15:12:59 2024, max compression
+gzip compressed data, was "collabconnector-0.1.1716921273.tar", last modified: Tue May 28 18:34:40 2024, max compression
```

## Comparing `collabconnector-0.1.1716909176.tar` & `collabconnector-0.1.1716921273.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.915668 collabconnector-0.1.1716909176/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 collabconnector-0.1.1716909176/LICENSE
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-28 15:12:59.915525 collabconnector-0.1.1716909176/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 collabconnector-0.1.1716909176/README.md
--rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 collabconnector-0.1.1716909176/pyproject.toml
--rw-r--r--   0 jonsnipes   (501) staff       (20)      965 2024-05-28 15:12:59.916146 collabconnector-0.1.1716909176/setup.cfg
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.632749 collabconnector-0.1.1716909176/src/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.644799 collabconnector-0.1.1716909176/src/CollabConnector/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.648456 collabconnector-0.1.1716909176/src/CollabConnector/CER/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 collabconnector-0.1.1716909176/src/CollabConnector/CER/CER.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CER/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.650092 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.651838 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AST/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    10786 2023-08-29 12:33:53.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AST/AST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AST/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.657205 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   357792 2023-08-30 01:25:13.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/AXL.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2023-08-29 16:07:10.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.636482 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.664706 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.688134 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.708090 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.727660 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.752261 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.787767 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.797018 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/14.0/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.818418 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/7.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.825971 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.841037 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.857389 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.873566 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.883138 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/CDR/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20752 2023-08-03 20:55:28.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/CDR/CDR.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/CDR/CDROnDemand.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/CDR/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    13200 2023-08-30 01:25:13.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/CUCM.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.884763 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/DIME/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/DIME/DIME.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/DIME/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.886482 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Logs/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Logs/Logs.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Logs/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.888483 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Phone/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.890240 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Risport/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Risport/Risport.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Risport/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.892346 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Serviceability/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Serviceability/Serviceability.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Serviceability/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.894054 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/UDS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/UDS/UDS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/UDS/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCM/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.895737 collabconnector-0.1.1716909176/src/CollabConnector/CUCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    15091 2023-08-29 12:24:59.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCX/CUCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/CUCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.897324 collabconnector-0.1.1716909176/src/CollabConnector/Expressway/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 collabconnector-0.1.1716909176/src/CollabConnector/Expressway/Expressway.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 collabconnector-0.1.1716909176/src/CollabConnector/Expressway/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.898978 collabconnector-0.1.1716909176/src/CollabConnector/IOS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    22137 2023-08-15 19:43:30.000000 collabconnector-0.1.1716909176/src/CollabConnector/IOS/IOS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 collabconnector-0.1.1716909176/src/CollabConnector/IOS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.900506 collabconnector-0.1.1716909176/src/CollabConnector/PAWS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/PAWS/PAWS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/PAWS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.902045 collabconnector-0.1.1716909176/src/CollabConnector/UCCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 collabconnector-0.1.1716909176/src/CollabConnector/UCCX/UCCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/UCCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.903694 collabconnector-0.1.1716909176/src/CollabConnector/Webex/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.906954 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Connect/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5205 2023-09-29 22:42:01.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Connect/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2942 2023-09-29 22:55:16.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Connect/TXT.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1108 2024-05-09 12:42:58.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Connect/WhatsApp.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      224 2024-05-09 12:43:27.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Connect/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.908481 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Consent/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5425 2023-09-29 23:50:27.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Consent/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1011 2023-09-29 23:52:18.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Consent/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.909472 collabconnector-0.1.1716909176/src/CollabConnector/Webex/ContactCenter/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    16914 2024-05-28 15:12:38.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/ContactCenter/ContactCenter.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2024-05-22 19:21:49.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/ContactCenter/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.913129 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Engage/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8235 2023-11-02 16:46:15.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Engage/Chat.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5439 2023-09-29 14:23:57.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Engage/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1354 2023-09-29 14:23:57.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Engage/Team.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4817 2023-11-02 16:51:10.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Engage/User.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      338 2023-09-29 14:23:57.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Engage/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.914138 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3412 2024-03-08 12:53:56.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Phone/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    17743 2024-05-09 19:53:28.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/Webex.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2024-03-08 13:05:25.000000 collabconnector-0.1.1716909176/src/CollabConnector/Webex/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:05:58.000000 collabconnector-0.1.1716909176/src/CollabConnector/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 15:12:59.914990 collabconnector-0.1.1716909176/src/CollabConnector.egg-info/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-28 15:12:59.000000 collabconnector-0.1.1716909176/src/CollabConnector.egg-info/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4467 2024-05-28 15:12:59.000000 collabconnector-0.1.1716909176/src/CollabConnector.egg-info/SOURCES.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2024-05-28 15:12:59.000000 collabconnector-0.1.1716909176/src/CollabConnector.egg-info/dependency_links.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       77 2024-05-28 15:12:59.000000 collabconnector-0.1.1716909176/src/CollabConnector.egg-info/requires.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2024-05-28 15:12:59.000000 collabconnector-0.1.1716909176/src/CollabConnector.egg-info/top_level.txt
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:40.024148 collabconnector-0.1.1716921273/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 collabconnector-0.1.1716921273/LICENSE
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-28 18:34:40.023772 collabconnector-0.1.1716921273/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 collabconnector-0.1.1716921273/README.md
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 collabconnector-0.1.1716921273/pyproject.toml
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      965 2024-05-28 18:34:40.034507 collabconnector-0.1.1716921273/setup.cfg
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.262906 collabconnector-0.1.1716921273/src/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.314355 collabconnector-0.1.1716921273/src/CollabConnector/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.353066 collabconnector-0.1.1716921273/src/CollabConnector/CER/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 collabconnector-0.1.1716921273/src/CollabConnector/CER/CER.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CER/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.355251 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.360326 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AST/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    10786 2023-08-29 12:33:53.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AST/AST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AST/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.422960 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   357792 2023-08-30 01:25:13.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/AXL.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2023-08-29 16:07:10.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.280672 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.434686 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.505369 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.570711 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.632730 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.699213 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.747190 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.762067 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/14.0/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.789208 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/7.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.847094 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.869005 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.894745 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.918973 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.943124 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/CDR/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20752 2023-08-03 20:55:28.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/CDR/CDR.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/CDR/CDROnDemand.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/CDR/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    13200 2023-08-30 01:25:13.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/CUCM.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.945511 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/DIME/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/DIME/DIME.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/DIME/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.947437 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Logs/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Logs/Logs.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Logs/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.949769 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Phone/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.951372 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Risport/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Risport/Risport.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Risport/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.953096 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Serviceability/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Serviceability/Serviceability.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Serviceability/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.954689 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/UDS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/UDS/UDS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/UDS/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCM/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.958936 collabconnector-0.1.1716921273/src/CollabConnector/CUCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    15091 2023-08-29 12:24:59.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCX/CUCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/CUCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.960975 collabconnector-0.1.1716921273/src/CollabConnector/Expressway/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 collabconnector-0.1.1716921273/src/CollabConnector/Expressway/Expressway.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 collabconnector-0.1.1716921273/src/CollabConnector/Expressway/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.963099 collabconnector-0.1.1716921273/src/CollabConnector/IOS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    22137 2023-08-15 19:43:30.000000 collabconnector-0.1.1716921273/src/CollabConnector/IOS/IOS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 collabconnector-0.1.1716921273/src/CollabConnector/IOS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.964956 collabconnector-0.1.1716921273/src/CollabConnector/PAWS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/PAWS/PAWS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/PAWS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.966686 collabconnector-0.1.1716921273/src/CollabConnector/UCCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 collabconnector-0.1.1716921273/src/CollabConnector/UCCX/UCCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/UCCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.980607 collabconnector-0.1.1716921273/src/CollabConnector/Webex/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.985082 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Connect/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5205 2023-09-29 22:42:01.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Connect/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2942 2023-09-29 22:55:16.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Connect/TXT.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1108 2024-05-09 12:42:58.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Connect/WhatsApp.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      224 2024-05-09 12:43:27.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Connect/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:39.987320 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Consent/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5425 2023-09-29 23:50:27.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Consent/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1011 2023-09-29 23:52:18.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Consent/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:40.011374 collabconnector-0.1.1716921273/src/CollabConnector/Webex/ContactCenter/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    17583 2024-05-28 18:34:28.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/ContactCenter/ContactCenter.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2024-05-22 19:21:49.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/ContactCenter/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:40.017975 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Engage/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8235 2023-11-02 16:46:15.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Engage/Chat.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5439 2023-09-29 14:23:57.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Engage/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1354 2023-09-29 14:23:57.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Engage/Team.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4817 2023-11-02 16:51:10.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Engage/User.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      338 2023-09-29 14:23:57.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Engage/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:40.020221 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3412 2024-03-08 12:53:56.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Phone/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    17743 2024-05-09 19:53:28.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/Webex.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2024-03-08 13:05:25.000000 collabconnector-0.1.1716921273/src/CollabConnector/Webex/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:05:58.000000 collabconnector-0.1.1716921273/src/CollabConnector/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-28 18:34:40.022413 collabconnector-0.1.1716921273/src/CollabConnector.egg-info/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-28 18:34:39.000000 collabconnector-0.1.1716921273/src/CollabConnector.egg-info/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4467 2024-05-28 18:34:39.000000 collabconnector-0.1.1716921273/src/CollabConnector.egg-info/SOURCES.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2024-05-28 18:34:39.000000 collabconnector-0.1.1716921273/src/CollabConnector.egg-info/dependency_links.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       77 2024-05-28 18:34:39.000000 collabconnector-0.1.1716921273/src/CollabConnector.egg-info/requires.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2024-05-28 18:34:39.000000 collabconnector-0.1.1716921273/src/CollabConnector.egg-info/top_level.txt
```

### Comparing `collabconnector-0.1.1716909176/LICENSE` & `collabconnector-0.1.1716921273/LICENSE`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/PKG-INFO` & `collabconnector-0.1.1716921273/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1716909176
+Version: 0.1.1716921273
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `collabconnector-0.1.1716909176/README.md` & `collabconnector-0.1.1716921273/README.md`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/setup.cfg` & `collabconnector-0.1.1716921273/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CollabConnector
-version = 0.1.1716909176
+version = 0.1.1716921273
 author = Jon Snipes
 author_email = jsnipes@mycollablab.org
 description = An attempt at a simplified API collection for Cisco Collab products
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mycollablab/CollabConnector
 project_urls =
```

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CER/CER.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CER/CER.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AST/AST.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AST/AST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/AXL.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/AXL.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/CDR/CDR.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/CDR/CDR.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/CDR/CDROnDemand.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/CDR/CDROnDemand.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/CUCM.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/CUCM.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/DIME/DIME.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/DIME/DIME.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Logs/Logs.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Logs/Logs.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Phone/Phone.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Risport/Risport.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Risport/Risport.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/Serviceability/Serviceability.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/Serviceability/Serviceability.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCM/UDS/UDS.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCM/UDS/UDS.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/CUCX/CUCX.py` & `collabconnector-0.1.1716921273/src/CollabConnector/CUCX/CUCX.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Expressway/Expressway.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Expressway/Expressway.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/IOS/IOS.py` & `collabconnector-0.1.1716921273/src/CollabConnector/IOS/IOS.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/PAWS/PAWS.py` & `collabconnector-0.1.1716921273/src/CollabConnector/PAWS/PAWS.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/UCCX/UCCX.py` & `collabconnector-0.1.1716921273/src/CollabConnector/UCCX/UCCX.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Webex/Connect/REST.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Webex/Connect/REST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Webex/Connect/TXT.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Webex/Connect/TXT.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Webex/Connect/WhatsApp.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Webex/Connect/WhatsApp.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Webex/Consent/REST.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Webex/Consent/REST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Webex/Consent/__init__.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Webex/Consent/__init__.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Webex/ContactCenter/ContactCenter.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Webex/ContactCenter/ContactCenter.py`

 * *Files 6% similar despite different names*

```diff
@@ -214,26 +214,29 @@
                                                }
                                 return return_data
                             else:
                                 page += 1
                                 return_data['data'].extend( response_data['data'] if 'data' in response_data.keys() else response_data )
 
                 elif response.status_code >= 200 and response.status_code < 300:
-                    return True
+                    if response.json():
+                        return response.json()
+                    else:
+                        return True
                 elif response.status_code == 429 or response.status_code == 429:  # handle throttling Wait and don't return to continue loop
                     print(f"{uri}{data} - API Request throttled: {response.headers['Retry-After']}", file=sys.stderr)
                     time.sleep(int(response.headers['Retry-After']) + 1)
 
                 elif response.status_code == 401:
                     raise Exception("Webex Admin token invalid.  Generate new token.")
 
                 else:
                     raise Exception(f"Error sending CC GET to Webex - {uri}{data} {response}{response.text}")
 
-    def delete(self, uri, debug: bool = False):
+    def delete(self, uri, debug: bool = False) -> dict:
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
 
         while True:  # loop for throttling
             try:
                 response = requests.delete(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}",
                                            headers=self.headers(),
@@ -246,19 +249,22 @@
                 if self.debug or debug:
                     print("DELETE", uri, response.status_code, response.headers)
                 if response.status_code == 429:  # handle throttling
                     time.sleep(int(response.headers['Retry-After']) + 1)
                 elif response.status_code == 200 and response.json():
                     return json.loads(response.text)
                 elif 200 < response.status_code < 300:
-                    return True
+                    if response.json():
+                        return response.json()
+                    else:
+                        return {"success": True}
                 else:
                     raise Exception(f"Error sending CC DELETE to Webex - {uri} {response}{response.text}")
 
-    def post(self, uri, data, debug: bool = False):
+    def post(self, uri, data, debug: bool = False) -> dict:
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
 
         while True:  # loop for throttling
             try:
                 response = requests.post(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}",
                                          headers=self.headers(payload =True),
@@ -272,19 +278,22 @@
                 if self.debug or debug:
                     print("POST", uri, response.status_code, response.headers)
                 if response.status_code == 429:  # handle throttling
                     time.sleep(int(response.headers['Retry-After']) + 1)
                 elif response.status_code == 200 and response.json():
                     return json.loads(response.text)
                 elif 200 < response.status_code < 300:
-                    return True
+                    if response.json():
+                        return response.json()
+                    else:
+                        return {"success": True}
                 else:
                     raise Exception(f"Error sending POST to Webex - {uri} {response}{response.text}")
 
-    def put(self, uri, data, debug: bool = False):
+    def put(self, uri, data, debug: bool = False) -> dict:
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
 
         while True:  # loop for throttling
             try:
                 response = requests.put(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}",
                                         headers=self.headers(payload =True),
@@ -298,19 +307,22 @@
                 if self.debug or debug:
                     print("PUT", uri, response.status_code, response.headers)
                 if response.status_code == 429:  # handle throttling
                     time.sleep(int(response.headers['Retry-After']) + 1)
                 elif response.status_code == 200 and response.json():
                     return json.loads(response.text)
                 elif 200 < response.status_code < 300:
-                    return True
+                    if response.json():
+                        return response.json()
+                    else:
+                        return {"success": True}
                 else:
                     raise Exception(f"Error sending PUT to Webex - {uri} {response}{response.text}")
 
-    def patch(self, uri, data, debug: bool = False):
+    def patch(self, uri, data, debug: bool = False) -> dict:
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
 
         while True:  # loop for throttling
             try:
                 response = requests.patch(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}",
                                           headers=self.headers(payload =True),
@@ -324,15 +336,18 @@
                 if self.debug or debug:
                     print("PATCH", uri, response.status_code, response.headers)
                 if response.status_code == 429:  # handle throttling
                     time.sleep(int(response.headers['Retry-After']) + 1)
                 elif response.status_code == 200 and response.json():
                     return json.loads(response.text)
                 elif 200 < response.status_code < 300:
-                    return True
+                    if response.json():
+                        return response.json()
+                    else:
+                        return {"success": True}
                 else:
                     raise Exception(f"Error sending PATCH to Webex - {uri} {response}{response.text}")
 
     def search(self, graphql_query: str, debug: bool = False, ms_offset: int = 86400000) -> dict:
         #  if to/from is not defined in query, ie: samplerequests, yjrm replace with 1 day from now
         current_time = int(time.time() * 1000)
         graphql_query = graphql_query.replace("{from}", str(current_time - ms_offset)).replace("{to}", str(current_time))
```

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Webex/Engage/Chat.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Webex/Engage/Chat.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Webex/Engage/REST.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Webex/Engage/REST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Webex/Engage/Team.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Webex/Engage/Team.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Webex/Engage/User.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Webex/Engage/User.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Webex/Phone/Phone.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Webex/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector/Webex/Webex.py` & `collabconnector-0.1.1716921273/src/CollabConnector/Webex/Webex.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector.egg-info/PKG-INFO` & `collabconnector-0.1.1716921273/src/CollabConnector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1716909176
+Version: 0.1.1716921273
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `collabconnector-0.1.1716909176/src/CollabConnector.egg-info/SOURCES.txt` & `collabconnector-0.1.1716921273/src/CollabConnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

