# Comparing `tmp/ci_cloudconnector-0.91.tar.gz` & `tmp/ci_cloudconnector-0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-0.91.tar", last modified: Tue May 28 06:59:39 2024, max compression
+gzip compressed data, was "ci_cloudconnector-0.92.tar", last modified: Tue May 28 09:56:40 2024, max compression
```

## Comparing `ci_cloudconnector-0.91.tar` & `ci_cloudconnector-0.92.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 06:59:39.860756 ci_cloudconnector-0.91/
-drwxrwxrwx   0        0        0        0 2024-05-28 06:59:39.855778 ci_cloudconnector-0.91/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      358 2024-05-28 06:59:39.000000 ci_cloudconnector-0.91/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-05-28 06:59:39.000000 ci_cloudconnector-0.91/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 06:59:39.000000 ci_cloudconnector-0.91/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-28 06:59:39.000000 ci_cloudconnector-0.91/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      358 2024-05-28 06:59:39.857766 ci_cloudconnector-0.91/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.91/README.txt
--rw-rw-rw-   0        0        0    42313 2024-05-28 06:59:11.000000 ci_cloudconnector-0.91/logic.py
--rw-rw-rw-   0        0        0     5949 2024-05-28 06:58:31.000000 ci_cloudconnector-0.91/main.py
--rw-rw-rw-   0        0        0       42 2024-05-28 06:59:39.860756 ci_cloudconnector-0.91/setup.cfg
--rw-rw-rw-   0        0        0      769 2024-05-28 06:59:05.000000 ci_cloudconnector-0.91/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:56:40.454487 ci_cloudconnector-0.92/
+drwxrwxrwx   0        0        0        0 2024-05-28 09:56:40.450367 ci_cloudconnector-0.92/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      358 2024-05-28 09:56:40.000000 ci_cloudconnector-0.92/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-28 09:56:40.000000 ci_cloudconnector-0.92/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 09:56:40.000000 ci_cloudconnector-0.92/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-28 09:56:40.000000 ci_cloudconnector-0.92/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      358 2024-05-28 09:56:40.452080 ci_cloudconnector-0.92/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.92/README.txt
+-rw-rw-rw-   0        0        0    41538 2024-05-28 09:55:42.000000 ci_cloudconnector-0.92/logic.py
+-rw-rw-rw-   0        0        0     5949 2024-05-28 06:58:31.000000 ci_cloudconnector-0.92/main.py
+-rw-rw-rw-   0        0        0     1856 2024-05-28 09:52:46.000000 ci_cloudconnector-0.92/myservice.py
+-rw-rw-rw-   0        0        0       42 2024-05-28 09:56:40.454487 ci_cloudconnector-0.92/setup.cfg
+-rw-rw-rw-   0        0        0      791 2024-05-28 09:55:36.000000 ci_cloudconnector-0.92/setup.py
```

### Comparing `ci_cloudconnector-0.91/logic.py` & `ci_cloudconnector-0.92/logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "0.91"
+VER = "0.92"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
@@ -321,16 +321,15 @@
     return token
 
 
 # ============================
 # make http request to cloud if fails set currentToken='' so it will be initialized next time
 # ============================
 def ciRequest(url, data, postGet="get", method="", token=""):
-    print(f"{str(datetime.now())} start ciRequest {method}")
-    print(f'VERSION: {VER}')
+    print(f"{datetime.now()}, START CIRequest {method}, VERSION: {VER}")
 
     ans = {}
     ans["isOK"] = False
     global currentToken
     ansIsSucessful = False
     try:
         if token == "":
@@ -519,15 +518,15 @@
 
     except Exception as inst:
         handleError("Error in printTags", inst)
 
 
 # ============================
 def setCloudTags(tagValues, token=""):
-
+    print('setCloudTags')
     global TagStatus
     updatedSuccessfully = False
     try:
         # url = HTTP_PREFIX + '://'+cfg_server_address+'/api/CloudConnector/SetCounterHistory/'
         url = cfg_server_address + "/api/CloudConnector/SetCounterHistory/"
 
         payload = []
@@ -1198,48 +1197,26 @@
                                 values = readEtherNetIP_Tags(arranged_tags[connector_type])
                                 if values == []:
                                     time.sleep(1)
                                     ci_print("Ethernet Empty values ::2", "ERROR")
                                     values = readEtherNetIP_Tags(arranged_tags[connector_type])
 
                     if len(values) > 0:
-                        printVal = (
-                            " Val="
-                            + str(values[0]["value"])
-                            + " "
-                            + str(len(values))
-                            + " Tags"
-                        )
-                        ci_print(printVal, "INFO")
-                        print(
-                            str(datetime.now())
-                            + " Send Vals:"
-                            + str(scanRate)
-                            + " diff "
-                            + str(diff)
-                            + printVal
-                        )
+                        ci_print(f'VALUE: {values[0]["value"]}, TAGS: {len(values)}', 'INFO')
+                        print(f'SCANRATE: {scanRate}, DIFF: {diff}')
                     else:
-                        printVal = " No Values"
-                        ci_print(printVal, "ERROR")
-                        print(
-                            str(datetime.now())
-                            + " Send Vals:"
-                            + str(scanRate)
-                            + " diff "
-                            + str(diff)
-                            + printVal
-                        )
+                        ci_print(f'NO VALUES', 'ERROR')
+                        print(f'SCANRATE: {scanRate}, DIFF: {diff}')
 
                     if values:
                         saveValuesToFile(values, "")
                         removeOldestFile()
 
                         now = datetime.now()
-                        ci_print("scanRateStr time updated==>" + str(now), "INFO")
+                        ci_print("SCANRATE TIME UPDATED==>" + str(now), "INFO")
                         ScanRateLastRead[scanRateStr] = now
 
 
         if currentToken != "":
             handleAllValuesFiles(currentToken)
         else:
             ci_print("No Token, skipping upload step", "WARNING")
```

### Comparing `ci_cloudconnector-0.91/main.py` & `ci_cloudconnector-0.92/main.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-0.91/setup.py` & `ci_cloudconnector-0.92/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="0.91",
+    version="0.92",
     packages=find_packages(),
-    py_modules=["logic", "main"],
+    py_modules=["logic", "main", "setup", "myservice"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
     long_description=open("README.txt").read()  # Make sure you have README.txt in the same directory
 )
```

