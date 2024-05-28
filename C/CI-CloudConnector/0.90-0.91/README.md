# Comparing `tmp/ci_cloudconnector-0.90.tar.gz` & `tmp/ci_cloudconnector-0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-0.90.tar", last modified: Mon May 27 15:02:21 2024, max compression
+gzip compressed data, was "ci_cloudconnector-0.91.tar", last modified: Tue May 28 06:59:39 2024, max compression
```

## Comparing `ci_cloudconnector-0.90.tar` & `ci_cloudconnector-0.91.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 15:02:21.232042 ci_cloudconnector-0.90/
-drwxrwxrwx   0        0        0        0 2024-05-27 15:02:21.228096 ci_cloudconnector-0.90/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      358 2024-05-27 15:02:21.000000 ci_cloudconnector-0.90/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-05-27 15:02:21.000000 ci_cloudconnector-0.90/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 15:02:21.000000 ci_cloudconnector-0.90/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 15:02:21.000000 ci_cloudconnector-0.90/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      358 2024-05-27 15:02:21.229336 ci_cloudconnector-0.90/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.90/README.txt
--rw-rw-rw-   0        0        0    45614 2024-05-27 15:01:54.000000 ci_cloudconnector-0.90/logic.py
--rw-rw-rw-   0        0        0    12877 2024-05-27 14:59:45.000000 ci_cloudconnector-0.90/main.py
--rw-rw-rw-   0        0        0       42 2024-05-27 15:02:21.232539 ci_cloudconnector-0.90/setup.cfg
--rw-rw-rw-   0        0        0      769 2024-05-27 15:01:58.000000 ci_cloudconnector-0.90/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:59:39.860756 ci_cloudconnector-0.91/
+drwxrwxrwx   0        0        0        0 2024-05-28 06:59:39.855778 ci_cloudconnector-0.91/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      358 2024-05-28 06:59:39.000000 ci_cloudconnector-0.91/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-05-28 06:59:39.000000 ci_cloudconnector-0.91/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 06:59:39.000000 ci_cloudconnector-0.91/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-28 06:59:39.000000 ci_cloudconnector-0.91/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      358 2024-05-28 06:59:39.857766 ci_cloudconnector-0.91/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.91/README.txt
+-rw-rw-rw-   0        0        0    42313 2024-05-28 06:59:11.000000 ci_cloudconnector-0.91/logic.py
+-rw-rw-rw-   0        0        0     5949 2024-05-28 06:58:31.000000 ci_cloudconnector-0.91/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-28 06:59:39.860756 ci_cloudconnector-0.91/setup.cfg
+-rw-rw-rw-   0        0        0      769 2024-05-28 06:59:05.000000 ci_cloudconnector-0.91/setup.py
```

### Comparing `ci_cloudconnector-0.90/logic.py` & `ci_cloudconnector-0.91/logic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "0.90"
+VER = "0.91"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
@@ -157,40 +157,14 @@
         )
         # print(message, err_desc, exc_type, fname, exc_tb.tb_lineno)
         ci_print(srtMsg, "ERROR")
     except Exception as errIgnore:
         ci_print("Error in handleError " + str(errIgnore), "ERROR")
 
 
-
-# ============================
-def updateAliveFile(timeStamp=None, pid=None):
-
-    ret = False
-    try:
-        fileName = "/" + HomeDir + "/lc_pid.txt"
-        # write tags to file
-        data = {}
-        if pid == None:
-            pid = os.getpid()
-        if timeStamp == None:
-            timeStamp = str(datetime.now())
-
-        data["pid"] = pid
-        data["now"] = timeStamp
-        f = open(fileName, "w")
-        json.dump(data, f)
-        f.close()
-        ret = True
-    except Exception as inst:
-        handleError("Error in updateAliveFile !! ", inst)
-
-    return ret
-
-
 # ============================
 def getAliveFile():
 
     ret = None
     try:
         fileName = "/" + HomeDir + "/lc_pid.txt"
         # read alive file
@@ -199,46 +173,14 @@
         # print 'getAliveFile file=' + str(ret)
     except Exception as inst:
         handleError("Error in getAliveFile", inst)
     return ret
 
 
 # ============================
-def checkIsAlive():
-
-    ret = {}
-    ret["isAlive"] = False
-    isAliveTimeOutSeconds = 300
-    try:
-        ans = getAliveFile()
-        pid = ans["pid"]
-        lastTimeStampStr = ans["now"]
-
-        if lastTimeStampStr == "Started":
-            # in case the machine was restarted
-            ret["isAlive"] = False
-            return ret
-
-        # print 'lastTimeStampStr ' +lastTimeStampStr
-        lastTimeStamp = datetime.strptime(lastTimeStampStr, "%Y-%m-%d %H:%M:%S.%f")
-        now = datetime.now()
-        diff = (now - lastTimeStamp).total_seconds()
-        ret["diff"] = diff
-        # print 'Diff = ' + str(diff)
-        if diff <= isAliveTimeOutSeconds:
-            ret["isAlive"] = True
-
-    except Exception as inst:
-        # print 'error in checkIsAlive ' + str(inst)
-        handleError("Error in checkIsAlive", inst)
-    return ret
-
-
-
-# ============================
 
 import os
 import configparser
 
 def initialize_config(overwrite=False):
 
     global cfg_server_address
@@ -426,63 +368,14 @@
     ans["isOK"] = ansIsSucessful
     ans["response"] = response
     return ans
 
 
 
 # ============================
-def setClock(newUtcDate):
-
-    # strTime = '19/12/2016 13:53:55 +02:00'
-    # unixTime = '2006-08-07 12:34:56'
-    # newDate = unixTime
-    # newDate = strTime
-    try:
-        if newUtcDate == "":
-            return
-
-        serverUtcTime = datetime.strptime(newUtcDate, "%Y-%m-%d %H:%M:%S")
-        # print 'serverUtcTime=' + str(serverUtcTime)
-        utcNow = datetime.utcnow()
-        diff = (utcNow - serverUtcTime).total_seconds()
-        # print 'differencr from now=' + str(diff)
-        if abs(diff) > 3:
-            ci_print(
-                "setting new system time to "
-                + str(serverUtcTime)
-                + "(UTC) ,Currently: "
-                + str(utcNow)
-                + "(UTC)", "INFO"
-            )
-            set_system_time(newUtcDate)
-            now = datetime.now()
-            ci_print("New Local Time is " + str(now), "INFO")
-
-    except Exception as inst:
-        handleError("Error in setClock ", inst)
-
-
-def set_system_time(new_utc_date):
-    try:
-        if new_utc_date == '':
-            return
-
-        if platform.system() == "Windows":
-            print("set_system_time NO NEED FOR Windows", "INFO")
-            #command = f"powershell -Command \"Set-Date -Date '{new_utc_date}'\""
-            #subprocess.run(command, shell=True, check=True)
-        else:
-            # Command to set system time in Linux
-            os.system('sudo date --set="%s"' % new_utc_date + "+00:00")
-
-        ci_print(f"System time set to {new_utc_date}", "INFO")
-    except Exception as inst:
-        handleError("Error in set_system_time", inst)
-
-# ============================
 def get_cloud_version():
 
     global GetCloudVersionFromServerMinRateSeconds
     global g_lastGetCloudVersionFromServer
     global currentToken
     global VER
     global sugestedUpdateVersion
@@ -503,15 +396,14 @@
 
         ci_print(f"Last Get version from server was {getVersionTimePass} seconds ago, getVersionRate = {GetTagsFromServerMinRateSeconds}", "INFO")
 
         if getVersionTimePass == 0 or getVersionTimePass > GetCloudVersionFromServerMinRateSeconds:
 
             # print "update pid file for watchdog"
             # do after clock settings because some times the machine loads with old clock and trigger watchdog
-            updateAliveFile()
 
             # print "handleNewRequests"
             handleNewRequests()
 
             # print 'getting version from server'
 
             g_lastGetCloudVersionFromServer = datetime.now()
@@ -523,16 +415,14 @@
 
             if not ret["isOK"]:
                 return ""
 
             ci_print(f"gettags response = {response.text}", "INFO")
             ans = json.loads(response.text)
             update_to_version = ans[0]
-            server_time = ans[1]
-            setClock(server_time)
 
             sugestedUpdateVersion = update_to_version
 
             if bool(update_to_version) != "" and bool(update_to_version != VER):
                 ci_print(f"Local Version: {VER} but Server suggests Other Version: {update_to_version}", "INFO")
 
                 # printTags(tags)
```

### Comparing `ci_cloudconnector-0.90/setup.py` & `ci_cloudconnector-0.91/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="0.90",
+    version="0.91",
     packages=find_packages(),
     py_modules=["logic", "main"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

