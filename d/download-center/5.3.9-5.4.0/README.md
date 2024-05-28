# Comparing `tmp/download-center-5.3.9.tar.gz` & `tmp/download-center-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "download-center-5.3.9.tar", last modified: Tue May 28 03:54:23 2024, max compression
+gzip compressed data, was "dist\download-center-5.4.0.tar", last modified: Tue May 28 06:02:46 2024, max compression
```

## Comparing `download-center-5.3.9.tar` & `download-center-5.4.0.tar`

### file list

```diff
@@ -1,52 +1,48 @@
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.703291 download-center-5.3.9/
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1823 2024-05-28 03:54:23.703105 download-center-5.3.9/PKG-INFO
--rw-r--r--   0 berry-zhang   (501) staff       (20)      888 2024-05-28 03:53:33.000000 download-center-5.3.9/README.md
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.695105 download-center-5.3.9/download_center/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1347 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/config.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.695960 download-center-5.3.9/download_center/new_spider/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/__init__.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.696285 download-center-5.3.9/download_center/new_spider/downloader/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/downloader/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1347 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/downloader/config.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     9076 2024-05-28 03:53:36.000000 download-center-5.3.9/download_center/new_spider/downloader/html_local_downloader.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.697023 download-center-5.3.9/download_center/new_spider/spider/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/spider/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)    16614 2024-05-28 03:53:36.000000 download-center-5.3.9/download_center/new_spider/spider/basespider.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     4675 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/spider/spider.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.700951 download-center-5.3.9/download_center/new_spider/util/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)    71351 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/ua_mobile_list.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)    47414 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/ua_pc_list.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)      471 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/ua_spider_list.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)    37369 2024-05-16 09:59:13.000000 download-center-5.3.9/download_center/new_spider/util/util_baidu.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)    12709 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/util_baidu_relate.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      323 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/util_md5.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      540 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/util_ping.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      777 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/util_url.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      709 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/new_spider/util/util_useragent.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)       14 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/requirements.txt
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.702271 download-center-5.3.9/download_center/store/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     3147 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/baidu_cookies.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      770 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/config.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     9132 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/py_store_mysql_pool.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/store_cache.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     3285 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/store_es.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     4039 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/store_es_v2.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/store_file.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      739 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/store_mongo.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     2014 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/store/store_oss.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.702884 download-center-5.3.9/download_center/util/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/util/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     6124 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/util/py_util_basestore.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     2409 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/util/util_log.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     2480 2024-05-15 02:43:55.000000 download-center-5.3.9/download_center/util/util_log_v2.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-28 03:54:23.695838 download-center-5.3.9/download_center.egg-info/
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1823 2024-05-28 03:54:23.000000 download-center-5.3.9/download_center.egg-info/PKG-INFO
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1622 2024-05-28 03:54:23.000000 download-center-5.3.9/download_center.egg-info/SOURCES.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)        1 2024-05-28 03:54:23.000000 download-center-5.3.9/download_center.egg-info/dependency_links.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)      106 2024-05-28 03:54:23.000000 download-center-5.3.9/download_center.egg-info/requires.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)       16 2024-05-28 03:54:23.000000 download-center-5.3.9/download_center.egg-info/top_level.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)       38 2024-05-28 03:54:23.703377 download-center-5.3.9/setup.cfg
--rw-r--r--   0 berry-zhang   (501) staff       (20)     4025 2024-05-28 03:54:22.000000 download-center-5.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.295795 download-center-5.4.0/
+-rw-rw-rw-   0        0        0     1829 2024-05-28 06:02:46.294798 download-center-5.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2024-05-16 07:40:34.000000 download-center-5.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.249361 download-center-5.4.0/download_center/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/__init__.py
+-rw-rw-rw-   0        0        0     1399 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/config.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.268342 download-center-5.4.0/download_center/new_spider/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.270305 download-center-5.4.0/download_center/new_spider/downloader/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/downloader/__init__.py
+-rw-rw-rw-   0        0        0     1399 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/downloader/config.py
+-rw-rw-rw-   0        0        0     9318 2024-05-28 03:21:13.000000 download-center-5.4.0/download_center/new_spider/downloader/html_local_downloader.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.273297 download-center-5.4.0/download_center/new_spider/spider/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/spider/__init__.py
+-rw-rw-rw-   0        0        0    18441 2024-05-28 05:34:10.000000 download-center-5.4.0/download_center/new_spider/spider/basespider.py
+-rw-rw-rw-   0        0        0     4832 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/spider/spider.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.280278 download-center-5.4.0/download_center/new_spider/util/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/util/__init__.py
+-rw-rw-rw-   0        0        0    38181 2024-05-16 08:40:14.000000 download-center-5.4.0/download_center/new_spider/util/util_baidu.py
+-rw-rw-rw-   0        0        0    12892 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/util/util_baidu_relate.py
+-rw-rw-rw-   0        0        0      344 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/util/util_md5.py
+-rw-rw-rw-   0        0        0      558 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/util/util_ping.py
+-rw-rw-rw-   0        0        0      804 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/util/util_url.py
+-rw-rw-rw-   0        0        0      741 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/new_spider/util/util_useragent.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.289808 download-center-5.4.0/download_center/store/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/__init__.py
+-rw-rw-rw-   0        0        0     3254 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/baidu_cookies.py
+-rw-rw-rw-   0        0        0      802 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/config.py
+-rw-rw-rw-   0        0        0     9397 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/py_store_mysql_pool.py
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/store_cache.py
+-rw-rw-rw-   0        0        0     3398 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/store_es.py
+-rw-rw-rw-   0        0        0     4163 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/store_es_v2.py
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/store_file.py
+-rw-rw-rw-   0        0        0      764 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/store_mongo.py
+-rw-rw-rw-   0        0        0     2082 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/store/store_oss.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.293800 download-center-5.4.0/download_center/util/
+-rw-rw-rw-   0        0        0        0 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/util/__init__.py
+-rw-rw-rw-   0        0        0     6299 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/util/py_util_basestore.py
+-rw-rw-rw-   0        0        0     2490 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/util/util_log.py
+-rw-rw-rw-   0        0        0     2563 2024-05-16 07:40:34.000000 download-center-5.4.0/download_center/util/util_log_v2.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:02:46.266317 download-center-5.4.0/download_center.egg-info/
+-rw-rw-rw-   0        0        0     1829 2024-05-28 06:02:46.000000 download-center-5.4.0/download_center.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1440 2024-05-28 06:02:46.000000 download-center-5.4.0/download_center.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 06:02:46.000000 download-center-5.4.0/download_center.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2024-05-28 06:02:46.000000 download-center-5.4.0/download_center.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-28 06:02:46.000000 download-center-5.4.0/download_center.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 06:02:46.295795 download-center-5.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     4169 2024-05-28 05:46:24.000000 download-center-5.4.0/setup.py
```

### Comparing `download-center-5.3.9/download_center/config.py` & `download-center-5.4.0/download_center/config.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# -*- coding: utf8 -*-
-# from util.util_ping import Ping
-from platform import system as system_name  # Returns the system/OS name
-from os import system as system_call  # Execute a shell command
-
-
-def ping(ip):
-    try:
-        parameters = "-n 1" if system_name().lower() == "windows" else "-c 1"
-        return system_call("ping " + parameters + " " + ip + " > log.txt") == 0
-    except:
-        return False
-
-# request timeout
-REQUEST_TIMEOUT = 30
-
-IP_HOST = '182.254.155.218:9090'                   # 上線地址
-# 内网ip
-DOWNLOADER_CENTER_OUTER_IP = "182.254.155.218"
-DOWNLOADER_CENTER_INNER_IP = "172.17.0.13"
-PORT = '9090'
-
-# validate_accout
-VALIDATE_ACCOUNT_URL = "http://{}:9090/download/login"
-
-AGENCYIP_URL = "http://{}:9090/download/get_ip"
-
-ADD_BLACK_IP = "http://{}/download/addBlackIp"         # 添加黑名单
-
-# sendTask
-DOWNLOADER_SENDTASK = "http://{}/download/setTask"
-
-# getResult
-DOWNLOADER_GETRESULT = "http://{}/download/getResult"
-
-TASK_SCHEDULER_IP = "http://{}/adslGetIp"
-
-REQUEST_RETYR_SLEEP = 2     # 请求异常等待时间
-
-REQUEST_RETYR_MAX_SLEEP = 10    # 请求异常 超過幾次 等待时间
-
-
-DOWNLOADER_CENTER_IP = {
-    "inner": DOWNLOADER_CENTER_INNER_IP,
-    "outer": DOWNLOADER_CENTER_OUTER_IP
-}
-
-if ping(DOWNLOADER_CENTER_INNER_IP):
-    ENVIR = 'inner'
-else:
-    ENVIR = 'outer'
-
+# -*- coding: utf8 -*-
+# from util.util_ping import Ping
+from platform import system as system_name  # Returns the system/OS name
+from os import system as system_call  # Execute a shell command
+
+
+def ping(ip):
+    try:
+        parameters = "-n 1" if system_name().lower() == "windows" else "-c 1"
+        return system_call("ping " + parameters + " " + ip + " > log.txt") == 0
+    except:
+        return False
+
+# request timeout
+REQUEST_TIMEOUT = 30
+
+IP_HOST = '182.254.155.218:9090'                   # 上線地址
+# 内网ip
+DOWNLOADER_CENTER_OUTER_IP = "182.254.155.218"
+DOWNLOADER_CENTER_INNER_IP = "172.17.0.13"
+PORT = '9090'
+
+# validate_accout
+VALIDATE_ACCOUNT_URL = "http://{}:9090/download/login"
+
+AGENCYIP_URL = "http://{}:9090/download/get_ip"
+
+ADD_BLACK_IP = "http://{}/download/addBlackIp"         # 添加黑名单
+
+# sendTask
+DOWNLOADER_SENDTASK = "http://{}/download/setTask"
+
+# getResult
+DOWNLOADER_GETRESULT = "http://{}/download/getResult"
+
+TASK_SCHEDULER_IP = "http://{}/adslGetIp"
+
+REQUEST_RETYR_SLEEP = 2     # 请求异常等待时间
+
+REQUEST_RETYR_MAX_SLEEP = 10    # 请求异常 超過幾次 等待时间
+
+
+DOWNLOADER_CENTER_IP = {
+    "inner": DOWNLOADER_CENTER_INNER_IP,
+    "outer": DOWNLOADER_CENTER_OUTER_IP
+}
+
+if ping(DOWNLOADER_CENTER_INNER_IP):
+    ENVIR = 'inner'
+else:
+    ENVIR = 'outer'
+
 downloader_ip = None
```

### Comparing `download-center-5.3.9/download_center/new_spider/downloader/config.py` & `download-center-5.4.0/download_center/new_spider/downloader/config.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# -*- coding: utf8 -*-
-# from util.util_ping import Ping
-from platform import system as system_name  # Returns the system/OS name
-from os import system as system_call  # Execute a shell command
-
-
-def ping(ip):
-    try:
-        parameters = "-n 1" if system_name().lower() == "windows" else "-c 1"
-        return system_call("ping " + parameters + " " + ip + " > log.txt") == 0
-    except:
-        return False
-
-# request timeout
-REQUEST_TIMEOUT = 30
-
-IP_HOST = '182.254.155.218:9090'                   # 上線地址
-# 内网ip
-DOWNLOADER_CENTER_OUTER_IP = "182.254.155.218"
-DOWNLOADER_CENTER_INNER_IP = "172.17.0.13"
-PORT = '9090'
-
-# validate_accout
-VALIDATE_ACCOUNT_URL = "http://{}:9090/download/login"
-
-AGENCYIP_URL = "http://{}:9090/download/get_ip"
-
-ADD_BLACK_IP = "http://{}/download/addBlackIp"         # 添加黑名单
-
-# sendTask
-DOWNLOADER_SENDTASK = "http://{}/download/setTask"
-
-# getResult
-DOWNLOADER_GETRESULT = "http://{}/download/getResult"
-
-TASK_SCHEDULER_IP = "http://{}/adslGetIp"
-
-REQUEST_RETYR_SLEEP = 2     # 请求异常等待时间
-
-REQUEST_RETYR_MAX_SLEEP = 10    # 请求异常 超過幾次 等待时间
-
-
-DOWNLOADER_CENTER_IP = {
-    "inner": DOWNLOADER_CENTER_INNER_IP,
-    "outer": DOWNLOADER_CENTER_OUTER_IP
-}
-
-if ping(DOWNLOADER_CENTER_INNER_IP):
-    ENVIR = 'inner'
-else:
-    ENVIR = 'outer'
-
+# -*- coding: utf8 -*-
+# from util.util_ping import Ping
+from platform import system as system_name  # Returns the system/OS name
+from os import system as system_call  # Execute a shell command
+
+
+def ping(ip):
+    try:
+        parameters = "-n 1" if system_name().lower() == "windows" else "-c 1"
+        return system_call("ping " + parameters + " " + ip + " > log.txt") == 0
+    except:
+        return False
+
+# request timeout
+REQUEST_TIMEOUT = 30
+
+IP_HOST = '182.254.155.218:9090'                   # 上線地址
+# 内网ip
+DOWNLOADER_CENTER_OUTER_IP = "182.254.155.218"
+DOWNLOADER_CENTER_INNER_IP = "172.17.0.13"
+PORT = '9090'
+
+# validate_accout
+VALIDATE_ACCOUNT_URL = "http://{}:9090/download/login"
+
+AGENCYIP_URL = "http://{}:9090/download/get_ip"
+
+ADD_BLACK_IP = "http://{}/download/addBlackIp"         # 添加黑名单
+
+# sendTask
+DOWNLOADER_SENDTASK = "http://{}/download/setTask"
+
+# getResult
+DOWNLOADER_GETRESULT = "http://{}/download/getResult"
+
+TASK_SCHEDULER_IP = "http://{}/adslGetIp"
+
+REQUEST_RETYR_SLEEP = 2     # 请求异常等待时间
+
+REQUEST_RETYR_MAX_SLEEP = 10    # 请求异常 超過幾次 等待时间
+
+
+DOWNLOADER_CENTER_IP = {
+    "inner": DOWNLOADER_CENTER_INNER_IP,
+    "outer": DOWNLOADER_CENTER_OUTER_IP
+}
+
+if ping(DOWNLOADER_CENTER_INNER_IP):
+    ENVIR = 'inner'
+else:
+    ENVIR = 'outer'
+
 downloader_ip = None
```

### Comparing `download-center-5.3.9/download_center/new_spider/spider/basespider.py` & `download-center-5.4.0/download_center/new_spider/spider/basespider.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,422 +1,447 @@
-# -*- coding: utf8 -*-
-import json
-
-import requests
-from download_center.new_spider.downloader.downloader import SpiderRequest
-from download_center.new_spider.downloader.html_local_downloader import HtmlLocalDownloader
-from download_center.new_spider.util.util_useragent import UtilUseragent
-from download_center.new_spider.downloader import config
-# from Queue import LifoQueue
-from queue import Queue
-from queue import Empty
-from threading import Thread
-import time
-import traceback
-import objgraph
-from datetime import datetime
-import uuid
-from prettytable import PrettyTable
-import sys
-
-
-class BaseSpider(object):
-    """
-    基本的爬虫类
-    该爬虫维护四个队列：待发送队列sending_queue、已发送队列sended_queue
-    取回结果队列response_queue、待存储队列store_queue
-    发送的对象统一封装成SpiderRequest对象
-    启动时，通过start_requests方法构造一批待发送的SpiderRequest对象送到待发送队列里面
-    发送线程send_requests依次从sending_queue队列取值并发送，获取的结果通过deal_request_results来处理
-    如果发送成功，将SpiderRequest对象送入已发送队列sended_queue，如果发送失败则重新回到待发送队列sending_queue
-    取结果线程get_response依次从sended_queue队列取值并发送，获取的结果放至取回结果队列response_queue，
-    deal_response_results从取回结果队列response_queue取出来处理，处理结束后可把结果放至待存储队列store_queue异步存储，也可在
-    deal_response_results直接调用stores的存储方法直接存储
-    如果抓取成功，将对应结果存入数据库，如果发送失败则重新回到已发送队列sended_queue
-    """
-
-    def __init__(self, remote=False):
-        self.remote = remote
-        self.pc_user_agents = UtilUseragent.get()
-        self.mb_user_agents = UtilUseragent.get(type='MOBILE')
-        self.sending_queue = Queue()
-        self.sended_queue = Queue()
-        self.response_queue = Queue()
-        self.store_queue = Queue()
-        self.user_id = 0
-        self.stores = self.get_stores()
-        self.downloader = self.get_downloader()
-        self.sended_queue_max = 5000    # sended_queue 最大值
-        self.response_queue_max = 1500  # response_queue 最大值
-        self.store_queue_max = 2000     # store_queue 最大值
-        self.url_repeat = True          # 默认重复的url重发 false 不重发
-        self.downloader_ip = None
-        self.thread_wait = 0            # 线程等待时间
-
-    def get_user_password(self):
-        """
-        设置用户名和密码，由子类实现。用于爬取前验证是否合法
-        """
-        raise NotImplementedError()
-
-    def validate_user(self):
-        """
-        验证用户
-        """
-        if self.remote:
-            user, password = self.get_user_password()
-            rdata = self.downloader.validate_accout(user=user, password=password)
-            if rdata:
-                self.user_id = rdata
-                print("user: {}; password: {} user validate success".format(user, password))
-            else:
-                raise RuntimeError('用户验证失败')
-                sys.exit()
-        else:
-            pass
-
-    def get_downloader(self):
-        """
-        # 设置下载器类型，默认为Downloader
-        由原默认为Downloader下载中心更改为proxy代理模式
-        Return:
-            SpiderDownloader
-        """
-        # if self.remote:
-        #     return Downloader()
-        print("local downloader")
-        return HtmlLocalDownloader()
-
-    def start_requests(self):
-        """
-        初始化待发送请求队列，由子类实现。拼装一串SpiderRequest对象并送到sending_queue队列中
-        """
-        raise NotImplementedError()
-
-    def is_finish(self):
-        """
-        根据相关队列是否全都为空来判断任务处理结束
-        """
-        return self.sending_queue.empty()and self.sended_queue.empty() \
-            and self.response_queue.empty() and self.store_queue.empty()
-
-    def send_requests(self, max_idle_time):
-        """
-        发送请求。将sending_queue队列中的SpiderRequest对象通过downloader发送到下载中心
-        """
-        start_time = time.time()
-        while True:
-            try:
-                if self.sended_queue.qsize() < self.sended_queue_max and self.response_queue.qsize() < self.response_queue_max:
-                    request = self.sending_queue.get(timeout=1)
-                    if request.user_id is None:
-                        request.user_id = self.user_id
-                    results = self.downloader.set(request)
-                    self.deal_request_results(request, results)
-                    start_time = time.time()
-                    self.send_wait()
-                else:
-                    time.sleep(10)
-            except Empty:
-                if max_idle_time == -1:
-                    pass
-                elif start_time + max_idle_time < time.time():
-                    if self.is_finish():
-                        break
-                time.sleep(10)
-            except Exception:
-                print(traceback.format_exc())
-
-    def send_wait(self):
-        """
-        发送等待, 控制发往下载中心的速率
-        """
-        if self.thread_wait != 0:
-            time.sleep(self.thread_wait)
-        else:
-            if self.sended_queue.qsize() > 8000:
-                time.sleep(10)
-            elif self.sending_queue.qsize() < 1000:
-                time.sleep(1)
-            else:
-                time.sleep(0.1)
-
-    def get_wait(self):
-        """
-        获取结果等待, 控制发往处理队列的速率
-        """
-        if self.thread_wait != 0:
-            time.sleep(self.thread_wait)
-        else:
-            if self.response_queue.qsize() > 4000:
-                time.sleep(10)
-            elif self.sended_queue.qsize() < 1000:
-                time.sleep(1)
-            else:
-                time.sleep(0.1)
-
-    def get_response(self, max_idle_time):
-        """
-        获取url爬取结果。将sended_queue队列中的SpiderRequest对象通过downloader到下载中心去获取抓取到的html
-        """
-        start_time = time.time()
-        while True:
-            try:
-                if self.response_queue.qsize() < self.response_queue_max:
-                    request = self.sended_queue.get(timeout=1)
-                    if self.remote:
-                        user, password = self.get_user_password()
-                        data = {"user": user, "password": password}
-                        # 获取代理 ip
-                        r = requests.post(config.AGENCYIP_URL.format(config.DOWNLOADER_CENTER_IP[config.ENVIR]),
-                                          data=data, timeout=config.REQUEST_TIMEOUT)
-                        request.config["proxies"] = json.loads(r.text)["proxy"]
-                    results = self.downloader.get(request)
-                    #status = results[request.urls[0]['unique_md5']]
-                    self.response_queue.put((request, results))
-                    start_time = time.time()
-                    self.get_wait()     # wait confirm
-                else:
-                    time.sleep(10)
-            except Empty:
-                if max_idle_time == -1:
-                    pass
-                elif start_time + max_idle_time < time.time():
-                    if self.is_finish():
-                        break
-                time.sleep(10)
-            except Exception:
-                print(traceback.format_exc())
-
-    def deal_response(self, max_idle_time):
-        """
-        从结果队列response_queue中取出结果进行处理
-        """
-        start_time = time.time()
-        while True:
-            try:
-                if self.store_queue.qsize() < self.store_queue_max:
-                    request, results = self.response_queue.get(timeout=1)
-                    try:
-                        self.deal_response_results(request, results, self.stores)
-                    except Exception:
-                        print(traceback.format_exc())
-                    start_time = time.time()
-                else:
-                    time.sleep(10)
-            except Empty:
-                if max_idle_time == -1:
-                    pass
-                elif start_time + max_idle_time < time.time():
-                    if self.is_finish():
-                        break
-                time.sleep(10)
-            except Exception:
-                print(traceback.format_exc())
-
-    def store_results(self, max_idle_time):
-        """
-        从store_queue里面取出待存储的数据进行存储
-        """
-        start_time = time.time()
-        while True:
-            try:
-                results = self.store_queue.get(timeout=1)
-                self.to_store_results(results, self.stores)
-                start_time = time.time()
-            except Empty:
-                if max_idle_time == -1:
-                    pass
-                elif start_time + max_idle_time < time.time():
-                    if self.is_finish():
-                        break
-                time.sleep(10)
-            except Exception:
-                print(traceback.format_exc())
-
-    def to_store_results(self, results, stores):
-        """
-        存储结果，由子类实现。
-        Args:
-            results:处理response后的结果
-            stores:list，可能会用到的存储器（SpiderStore）列表
-        """
-        pass
-
-    def get_stores(self):
-        """
-        设置存储器，供deal_response_results调用
-        Return:
-            list,成员为SpiderStore对象
-        """
-        stores = list()
-        return stores
-
-    def deal_request_results(self, request, results):
-        if results == 0:
-            print('params exception request failure urls: {}'.format(request.urls))
-        elif results == -2:
-            print('no district urls: {}'.format(request.urls))
-        elif results == -1:
-            print("set request failure  urls: {}".format(request.urls))
-            self.sended_queue.put(request)
-        else:
-            self.sended_queue.put(request)
-
-    def deal_response_results(self, request, results, stores):
-        if results == 0:
-            print("deal_response_results results = 0 ")
-            return False
-        else:
-            urls = list()       # 重新去获取的url
-            failed_urls = list()    # 失败重发的url
-            for u in request.urls:
-                url = u['unique_md5']
-                if url in results:
-                    result = results[url]
-                    task_status = str(result['status'])
-                    if task_status in ['2', '3']:
-                        ret_failed_urls = self.deal_response_results_status(task_status, u, result, request)
-                        if ret_failed_urls:
-                            failed_urls = failed_urls + ret_failed_urls
-                    else:
-                        urls.append(u)
-                else:
-                    print('url send failure unique_md5:{}; url have:{}'.format(url, u["url"]))
-                    if self.url_repeat:
-                        failed_urls.append(u)
-            if len(urls) > 0:
-                request.urls = urls
-                self.sended_queue.put(request)
-            if len(failed_urls) > 0:
-                new_request = SpiderRequest(headers=request.headers, config=request.config)
-                new_request.urls = failed_urls
-                self.sending_queue.put(new_request)
-                new_request = None
-
-    def deal_response_results_status(self, task_status, url, result, request):
-        """
-            处理 task_status 是2,3的任务  重试返回数组， 若重试需切换headers内容需自行定义
-        :param task_status:
-        :param url:
-        :param result:
-        :param request:
-        :return:
-        """
-        raise NotImplementedError()
-
-    def record_log(self):
-        """
-        记录抓取日志，用于调整各个线程参数设置
-        """
-        while True:
-            table = PrettyTable(["x", "y"])
-            table.add_row(["datetime", str(datetime.now())])
-            table.add_row(["sending_queue", self.sending_queue.qsize()])
-            table.add_row(["sended_queue", self.sended_queue.qsize()])
-            table.add_row(["response_queue", self.response_queue.qsize()])
-            table.add_row(["store_queue", self.store_queue.qsize()])
-            table.reversesort = True
-            print(table)
-            del table
-            # objgraph.show_most_common_types()
-            time.sleep(30)
-            if self.is_finish():
-                break
-
-    @staticmethod
-    def get_unique_key():
-        """
-        生成唯一标识
-        :return:
-        """
-        return str(uuid.uuid1())
-
-    def add_black_ip(self, ip, type, expire_time=6):
-        """
-        记录IP黑名单
-        使用黑名单功能需在发送请求时在config设置param参数中配置任务类型
-        config : {param: {'task_type': 1}}
-        Args:
-            ip: IP地址
-            type: 指定任务类型有效
-            expire_time: 超时时间(小时)
-        """
-        self.downloader.downloader_add_black_ip(ip, type, expire_time=expire_time)
-
-    def clear_task_pool(self):
-        """
-        清空当前用户已发往下载中心的任务
-        :return:
-        """
-        pass
-
-    def after_deal_response(self, request, results):
-        """
-        抓取结果的处理逻辑后的后续操作，按需使用，默认不作任何操作
-        :param request:
-        :param results:
-        :return:
-        """
-        pass
-
-    @staticmethod
-    def retry(u, count):
-        retry_urls = list()
-        if u.get("re_send", 0) < int(count):
-            u["re_send"] = u.get("re_send", 0) + 1
-            retry_urls.append(u)
-        else:
-            print("conf_search_count > {};url: {}".format(count, u["url"]))
-        return retry_urls
-
-    def run(self, send_num=0, get_num=0, deal_num=0, store_num=0,
-            send_idle_time=600, get_idle_time=600,
-            deal_idle_time=600, store_idle_time=600, record_log=False, spider_count=0):
-        """
-        爬虫启动入口
-        Args:
-            send_num:发送请求线程数，默认为0
-            get_num:获取结果线程数，默认为0
-            deal_num:处理结果线程数，默认为0
-            store_num:存储结果线程数，默认为0
-            send_idle_time:发送请求线程超过该时间没有要发送的请求就停止，-1永不停止
-            get_idle_time:获取结果线程超过该时间没有要获取的结果就停止，-1永不停止
-            deal_idle_time:处理结果线程超过该时间没有要处理的结果就停止，-1永不停止
-            store_idle_time:存储结果线程超过该时间没有要存储的结果就停止，-1永不停止
-            record_log:定时记录各个队列大小，便于分析抓取效率
-            spider_count: 设置每小时发送量
-        """
-        self.validate_user()
-        thread_start = Thread(target=self.start_requests)
-        thread_start.start()
-
-        if send_num == 0:        # 用户自行配置
-            if spider_count == 0:
-                print("not set send_num and spider_count")
-                sys.exit()
-            else:
-                send_num = 5
-                get_num = 7
-                if deal_num == 0:
-                    deal_num = 5
-                if store_num == 0:
-                    store_num = 5
-                self.thread_wait = round(3600/(float(spider_count)/send_num), 2)
-
-        print("send_num: {}; get_num: {}; deal_num: {}; store_num: {}; spider_count: {}".format(send_num, get_num, deal_num, store_num, spider_count))
-        threads = list()
-        for i in range(0, send_num):
-            threads.append(Thread(target=self.send_requests, args=(send_idle_time,)))
-        for i in range(0, get_num):
-            threads.append(Thread(target=self.get_response, args=(get_idle_time,)))
-        for i in range(0, deal_num):
-            threads.append(Thread(target=self.deal_response, args=(deal_idle_time,)))
-        for i in range(0, store_num):
-            threads.append(Thread(target=self.store_results, args=(store_idle_time,)))
-
-        if record_log:
-            thread = Thread(target=self.record_log)
-            thread.setDaemon(True)
-            threads.append(thread)
-        for thread in threads:
-            thread.start()
+# -*- coding: utf8 -*-
+import json
+
+import requests
+from download_center.new_spider.downloader.downloader import SpiderRequest
+from download_center.new_spider.downloader.html_local_downloader import HtmlLocalDownloader
+from download_center.new_spider.util.util_useragent import UtilUseragent
+from download_center.new_spider.downloader import config
+# from Queue import LifoQueue
+from queue import Queue
+from queue import Empty
+from threading import Thread
+import time
+import traceback
+import objgraph
+from datetime import datetime
+import uuid
+from prettytable import PrettyTable
+import sys
+
+
+class BaseSpider(object):
+    """
+    基本的爬虫类
+    该爬虫维护四个队列：待发送队列sending_queue、已发送队列sended_queue
+    取回结果队列response_queue、待存储队列store_queue
+    发送的对象统一封装成SpiderRequest对象
+    启动时，通过start_requests方法构造一批待发送的SpiderRequest对象送到待发送队列里面
+    发送线程send_requests依次从sending_queue队列取值并发送，获取的结果通过deal_request_results来处理
+    如果发送成功，将SpiderRequest对象送入已发送队列sended_queue，如果发送失败则重新回到待发送队列sending_queue
+    取结果线程get_response依次从sended_queue队列取值并发送，获取的结果放至取回结果队列response_queue，
+    deal_response_results从取回结果队列response_queue取出来处理，处理结束后可把结果放至待存储队列store_queue异步存储，也可在
+    deal_response_results直接调用stores的存储方法直接存储
+    如果抓取成功，将对应结果存入数据库，如果发送失败则重新回到已发送队列sended_queue
+    """
+
+    def __init__(self, remote=False):
+        self.remote = remote
+        self.pc_user_agents = UtilUseragent.get()
+        self.mb_user_agents = UtilUseragent.get(type='MOBILE')
+        self.sending_queue = Queue()
+        self.sended_queue = Queue()
+        self.response_queue = Queue()
+        self.store_queue = Queue()
+        self.user_id = 0
+        self.stores = self.get_stores()
+        self.downloader = self.get_downloader()
+        self.sended_queue_max = 5000    # sended_queue 最大值
+        self.response_queue_max = 1500  # response_queue 最大值
+        self.store_queue_max = 2000     # store_queue 最大值
+        self.url_repeat = True          # 默认重复的url重发 false 不重发
+        self.downloader_ip = None
+        self.thread_wait = 0            # 线程等待时间
+
+    def get_user_password(self):
+        """
+        设置用户名和密码，由子类实现。用于爬取前验证是否合法
+        """
+        raise NotImplementedError()
+    
+    def validate_accout(self, user="", password=""):
+        try:
+            ip_type = 1 if config.ENVIR == 'inner' else 2
+            data = {"user": user, "password": password, 'type': ip_type}
+            for i in range(2):
+                try:
+                    r = reqs.post(config.VALIDATE_ACCOUNT_URL.format(config.DOWNLOADER_CENTER_IP[config.ENVIR]), data=data, timeout=config.REQUEST_TIMEOUT)
+                    rdata = json.loads(r.text)
+                    break
+                except:
+                    time.sleep(config.REQUEST_RETYR_SLEEP)
+                    # print(traceback.format_exc())
+                    rdata = {'status': 0,'msg':'login failure'}
+
+            if rdata["status"] == 0:
+                print(rdata["msg"])
+                return False
+            else:
+                config.downloader_ip = rdata["ip"]
+                return rdata["user_id"]
+        except:
+            print("datetime: {}; error: {}".format(str(datetime.now()), str(traceback.format_exc())))
+            return False
+
+    def validate_user(self):
+        """
+        验证用户
+        """
+        if self.remote:
+            user, password = self.get_user_password()
+            try:
+                ip_type = 1 if config.ENVIR == 'inner' else 2
+                data = {"user": user, "password": password, 'type': ip_type}
+                try:
+                    r = requests.post(config.VALIDATE_ACCOUNT_URL.format(config.DOWNLOADER_CENTER_IP[config.ENVIR]),
+                                      data=data, timeout=config.REQUEST_TIMEOUT)
+                    rdata = json.loads(r.text)
+                except:
+                    time.sleep(config.REQUEST_RETYR_SLEEP)
+                    # print(traceback.format_exc())
+                    rdata = {'status': 0, 'msg': 'login failure'}
+                if rdata["status"] == 0:
+                    print(rdata["msg"])
+                    raise RuntimeError('用户验证失败')
+                    sys.exit()
+                else:
+                    config.downloader_ip = rdata["ip"]
+                    self.user_id = rdata
+                    print("user: {}; password: {} user validate success".format(user, password))
+            except:
+                print("datetime: {}; error: {}".format(str(datetime.now()), str(traceback.format_exc())))
+                return False
+
+    def get_downloader(self):
+        """
+        # 设置下载器类型，默认为Downloader
+        由原默认为Downloader下载中心更改为proxy代理模式
+        Return:
+            SpiderDownloader
+        """
+        # if self.remote:
+        #     return Downloader()
+        print("local downloader")
+        return HtmlLocalDownloader()
+
+    def start_requests(self):
+        """
+        初始化待发送请求队列，由子类实现。拼装一串SpiderRequest对象并送到sending_queue队列中
+        """
+        raise NotImplementedError()
+
+    def is_finish(self):
+        """
+        根据相关队列是否全都为空来判断任务处理结束
+        """
+        return self.sending_queue.empty()and self.sended_queue.empty() \
+            and self.response_queue.empty() and self.store_queue.empty()
+
+    def send_requests(self, max_idle_time):
+        """
+        发送请求。将sending_queue队列中的SpiderRequest对象通过downloader发送到下载中心
+        """
+        start_time = time.time()
+        while True:
+            try:
+                if self.sended_queue.qsize() < self.sended_queue_max and self.response_queue.qsize() < self.response_queue_max:
+                    request = self.sending_queue.get(timeout=1)
+                    if request.user_id is None:
+                        request.user_id = self.user_id
+                    results = self.downloader.set(request)
+                    self.deal_request_results(request, results)
+                    start_time = time.time()
+                    self.send_wait()
+                else:
+                    time.sleep(10)
+            except Empty:
+                if max_idle_time == -1:
+                    pass
+                elif start_time + max_idle_time < time.time():
+                    if self.is_finish():
+                        break
+                time.sleep(10)
+            except Exception:
+                print(traceback.format_exc())
+
+    def send_wait(self):
+        """
+        发送等待, 控制发往下载中心的速率
+        """
+        if self.thread_wait != 0:
+            time.sleep(self.thread_wait)
+        else:
+            if self.sended_queue.qsize() > 8000:
+                time.sleep(10)
+            elif self.sending_queue.qsize() < 1000:
+                time.sleep(1)
+            else:
+                time.sleep(0.1)
+
+    def get_wait(self):
+        """
+        获取结果等待, 控制发往处理队列的速率
+        """
+        if self.thread_wait != 0:
+            time.sleep(self.thread_wait)
+        else:
+            if self.response_queue.qsize() > 4000:
+                time.sleep(10)
+            elif self.sended_queue.qsize() < 1000:
+                time.sleep(1)
+            else:
+                time.sleep(0.1)
+
+    def get_response(self, max_idle_time):
+        """
+        获取url爬取结果。将sended_queue队列中的SpiderRequest对象通过downloader到下载中心去获取抓取到的html
+        """
+        start_time = time.time()
+        while True:
+            try:
+                if self.response_queue.qsize() < self.response_queue_max:
+                    request = self.sended_queue.get(timeout=1)
+                    if self.remote:
+                        user, password = self.get_user_password()
+                        data = {"user": user, "password": password}
+                        # 获取代理 ip
+                        r = requests.post(config.AGENCYIP_URL.format(config.DOWNLOADER_CENTER_IP[config.ENVIR]),
+                                          data=data, timeout=config.REQUEST_TIMEOUT)
+                        request.config["proxies"] = json.loads(r.text)["proxy"]
+                    results = self.downloader.get(request)
+                    #status = results[request.urls[0]['unique_md5']]
+                    self.response_queue.put((request, results))
+                    start_time = time.time()
+                    self.get_wait()     # wait confirm
+                else:
+                    time.sleep(10)
+            except Empty:
+                if max_idle_time == -1:
+                    pass
+                elif start_time + max_idle_time < time.time():
+                    if self.is_finish():
+                        break
+                time.sleep(10)
+            except Exception:
+                print(traceback.format_exc())
+
+    def deal_response(self, max_idle_time):
+        """
+        从结果队列response_queue中取出结果进行处理
+        """
+        start_time = time.time()
+        while True:
+            try:
+                if self.store_queue.qsize() < self.store_queue_max:
+                    request, results = self.response_queue.get(timeout=1)
+                    try:
+                        self.deal_response_results(request, results, self.stores)
+                    except Exception:
+                        print(traceback.format_exc())
+                    start_time = time.time()
+                else:
+                    time.sleep(10)
+            except Empty:
+                if max_idle_time == -1:
+                    pass
+                elif start_time + max_idle_time < time.time():
+                    if self.is_finish():
+                        break
+                time.sleep(10)
+            except Exception:
+                print(traceback.format_exc())
+
+    def store_results(self, max_idle_time):
+        """
+        从store_queue里面取出待存储的数据进行存储
+        """
+        start_time = time.time()
+        while True:
+            try:
+                results = self.store_queue.get(timeout=1)
+                self.to_store_results(results, self.stores)
+                start_time = time.time()
+            except Empty:
+                if max_idle_time == -1:
+                    pass
+                elif start_time + max_idle_time < time.time():
+                    if self.is_finish():
+                        break
+                time.sleep(10)
+            except Exception:
+                print(traceback.format_exc())
+
+    def to_store_results(self, results, stores):
+        """
+        存储结果，由子类实现。
+        Args:
+            results:处理response后的结果
+            stores:list，可能会用到的存储器（SpiderStore）列表
+        """
+        pass
+
+    def get_stores(self):
+        """
+        设置存储器，供deal_response_results调用
+        Return:
+            list,成员为SpiderStore对象
+        """
+        stores = list()
+        return stores
+
+    def deal_request_results(self, request, results):
+        if results == 0:
+            print('params exception request failure urls: {}'.format(request.urls))
+        elif results == -2:
+            print('no district urls: {}'.format(request.urls))
+        elif results == -1:
+            print("set request failure  urls: {}".format(request.urls))
+            self.sended_queue.put(request)
+        else:
+            self.sended_queue.put(request)
+
+    def deal_response_results(self, request, results, stores):
+        if results == 0:
+            print("deal_response_results results = 0 ")
+            return False
+        else:
+            urls = list()       # 重新去获取的url
+            failed_urls = list()    # 失败重发的url
+            for u in request.urls:
+                url = u['unique_md5']
+                if url in results:
+                    result = results[url]
+                    task_status = str(result['status'])
+                    if task_status in ['2', '3']:
+                        ret_failed_urls = self.deal_response_results_status(task_status, u, result, request)
+                        if ret_failed_urls:
+                            failed_urls = failed_urls + ret_failed_urls
+                    else:
+                        urls.append(u)
+                else:
+                    print('url send failure unique_md5:{}; url have:{}'.format(url, u["url"]))
+                    if self.url_repeat:
+                        failed_urls.append(u)
+            if len(urls) > 0:
+                request.urls = urls
+                self.sended_queue.put(request)
+            if len(failed_urls) > 0:
+                new_request = SpiderRequest(headers=request.headers, config=request.config)
+                new_request.urls = failed_urls
+                self.sending_queue.put(new_request)
+                new_request = None
+
+    def deal_response_results_status(self, task_status, url, result, request):
+        """
+            处理 task_status 是2,3的任务  重试返回数组， 若重试需切换headers内容需自行定义
+        :param task_status:
+        :param url:
+        :param result:
+        :param request:
+        :return:
+        """
+        raise NotImplementedError()
+
+    def record_log(self):
+        """
+        记录抓取日志，用于调整各个线程参数设置
+        """
+        while True:
+            table = PrettyTable(["x", "y"])
+            table.add_row(["datetime", str(datetime.now())])
+            table.add_row(["sending_queue", self.sending_queue.qsize()])
+            table.add_row(["sended_queue", self.sended_queue.qsize()])
+            table.add_row(["response_queue", self.response_queue.qsize()])
+            table.add_row(["store_queue", self.store_queue.qsize()])
+            table.reversesort = True
+            print(table)
+            del table
+            # objgraph.show_most_common_types()
+            time.sleep(30)
+            if self.is_finish():
+                break
+
+    @staticmethod
+    def get_unique_key():
+        """
+        生成唯一标识
+        :return:
+        """
+        return str(uuid.uuid1())
+
+    def clear_task_pool(self):
+        """
+        清空当前用户已发往下载中心的任务
+        :return:
+        """
+        pass
+
+    def after_deal_response(self, request, results):
+        """
+        抓取结果的处理逻辑后的后续操作，按需使用，默认不作任何操作
+        :param request:
+        :param results:
+        :return:
+        """
+        pass
+
+    @staticmethod
+    def retry(u, count):
+        retry_urls = list()
+        if u.get("re_send", 0) < int(count):
+            u["re_send"] = u.get("re_send", 0) + 1
+            retry_urls.append(u)
+        else:
+            print("conf_search_count > {};url: {}".format(count, u["url"]))
+        return retry_urls
+
+    def run(self, send_num=0, get_num=0, deal_num=0, store_num=0,
+            send_idle_time=600, get_idle_time=600,
+            deal_idle_time=600, store_idle_time=600, record_log=False, spider_count=0):
+        """
+        爬虫启动入口
+        Args:
+            send_num:发送请求线程数，默认为0
+            get_num:获取结果线程数，默认为0
+            deal_num:处理结果线程数，默认为0
+            store_num:存储结果线程数，默认为0
+            send_idle_time:发送请求线程超过该时间没有要发送的请求就停止，-1永不停止
+            get_idle_time:获取结果线程超过该时间没有要获取的结果就停止，-1永不停止
+            deal_idle_time:处理结果线程超过该时间没有要处理的结果就停止，-1永不停止
+            store_idle_time:存储结果线程超过该时间没有要存储的结果就停止，-1永不停止
+            record_log:定时记录各个队列大小，便于分析抓取效率
+            spider_count: 设置每小时发送量
+        """
+        self.validate_user()
+        thread_start = Thread(target=self.start_requests)
+        thread_start.start()
+
+        if send_num == 0:        # 用户自行配置
+            if spider_count == 0:
+                print("not set send_num and spider_count")
+                sys.exit()
+            else:
+                send_num = 5
+                get_num = 7
+                if deal_num == 0:
+                    deal_num = 5
+                if store_num == 0:
+                    store_num = 5
+                self.thread_wait = round(3600/(float(spider_count)/send_num), 2)
+
+        print("send_num: {}; get_num: {}; deal_num: {}; store_num: {}; spider_count: {}".format(send_num, get_num, deal_num, store_num, spider_count))
+        threads = list()
+        for i in range(0, send_num):
+            threads.append(Thread(target=self.send_requests, args=(send_idle_time,)))
+        for i in range(0, get_num):
+            threads.append(Thread(target=self.get_response, args=(get_idle_time,)))
+        for i in range(0, deal_num):
+            threads.append(Thread(target=self.deal_response, args=(deal_idle_time,)))
+        for i in range(0, store_num):
+            threads.append(Thread(target=self.store_results, args=(store_idle_time,)))
+
+        if record_log:
+            thread = Thread(target=self.record_log)
+            thread.setDaemon(True)
+            threads.append(thread)
+        for thread in threads:
+            thread.start()
```

### Comparing `download-center-5.3.9/download_center/new_spider/spider/spider.py` & `download-center-5.4.0/download_center/new_spider/spider/spider.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-# -*- coding: utf8 -*-
-import os
-import re
-import sys
-
-
-
-class SpiderDownloader(object):
-    """
-    下载器的抽象类
-    用于下载指定url的网页内容
-    下载器可能自身具备下载功能，也可能是作为与下载中心交互的接口
-    """
-
-    def __init__(self):
-        pass
-
-    def set(self, headers, config={}, urls=[]):
-        """
-        设置http头或者将相关配置发到下载中心
-        Args:
-            headers: 字典，http头信息，
-                举例，{'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; WOW64; rv:47.0) Gecko/20100101 Firefox/47.0'}
-            config: 字典，可为空，用于向下载中心发送下载类型、优先级、抓取频率等相关信息，
-                或者向下载函数设置超时等相关信息，
-                举例：{'type':0, 'priority':5, 'frequency':1} 或 {'timeout':10}
-            urls: 数组，不使用下载中心则为空，用于将待下载的url预先发到下载中心进行下载
-        Returns:
-            1: 正常, 0: 出错
-        """
-        return 0
-
-    def get(self, url):
-        """
-        下载特定url的页面或者向下载中心请求特定url的结果
-        Args:
-            url: 要获取结果的一个url
-        Returns :
-            None: 未取到结果，可能是下载中心还没有下载完成
-            文本: 下载结果
-        """
-        return None
-
-
-class SpiderExtractor(object):
-    """
-    解析器的抽象类
-    用于将特定网页解析成结构化信息
-    每个页面有一个独立的SpiderExtractor类
-    """
-
-    def __init__(self):
-        pass
-
-    def extractor(self, text):
-        """
-        将一个页面文本解析为结构化信息的字典
-        Args:
-            text: 需要解析的文本
-        Returns:
-            数组: 每条为一个完整记录，记录由字典格式保存
-        """
-        return []
-
-
-class SpiderStore(object):
-    """
-    存储器的抽象类
-    用于将结构化信息保存到指定存储媒介中
-    Attributes:
-        fields: 用于保持抽取器字典的key与数据库字段的对应关系，
-            如果结果字典的某个key不包含在fields中，则将直接使用key作为字段名
-    """
-
-    def __init__(self):
-        self.fields = {}
-        pass
-
-    def store(self, results, type=1, keys=[]):
-        """
-        将一个数组存储到指定的存储媒介中
-        Args:
-            reuslts: 数组，每条为一个完整记录，记录由字典格式保存
-            type: 1-只插入（出错则忽略），2-只更新（原记录不存在则忽略），3-插入更新（无记录则插入，有记录则更新）
-            keys: 只插入则为空，更新则存储关键字典，此字段将作为更新的where条件
-        Returns:
-            1: 正常, 0: 出错
-        """
-        pass
-
-
-class Spider(object):
-    """
-    爬虫的抽象类
-    Attributes:
-        headers: http头，同SpiderDownloader
-        config: 抓取配置，同SpiderDownloader
-        urls: 待抓取url，同SpiderDownloader
-        downloader: 下载器，通常一个Spider配一个下载器
-        extractor: 解析器，一个Spider可以配多个解析器
-        store: 存储器，通常一个Spider配一个存储器
-    """
-
-    def __init__(self):
-        self.headers = {}
-        self.config = {}
-        self.urls = []
-        self.downloader = SpiderDownloader()
-        self.extractor = SpiderExtractor()
-        self.store = SpiderStore()
-        pass
-
-    def get_seeds(self):
-        """
-        获取urls
-        """
-        f = open('seeds.txt')
-        for line in f:
-            self.urls.append(line[:-1])
-        f.close()
-
-    def prepare(self):
-        """
-        用于对接下载中心的异步抓取，作为独立操作运行，投递任务后即退出
-        """
-        self.get_seeds()
-        self.downloader.set(self.headers, self.config, self.urls)
-
-    def run(self):
-        """
-        运行主函数，可独立运行（独立下载器模式），也可放在prepare之后运行（下载中心模式）
-        """
-        self.get_seeds()
-        for url in self.urls:
-            content = self.downloader.get(url)
-            results = self.extractor.extractor(content)
-            if len(results) > 0:
-                self.store.store(results)
-
-    def test(self, url):
-        """
-        测试单体url的结果
-        """
-        content = self.downloader.get(url)
-        results = self.extractor.extractor(content)
-        print(results)
-
-
-"""
-def Main():
-    s = Spider()
-    #s.prepare
-    s.run()
-
-if __name__ == "__main__":
-    Main();
-"""
+# -*- coding: utf8 -*-
+import os
+import re
+import sys
+
+
+
+class SpiderDownloader(object):
+    """
+    下载器的抽象类
+    用于下载指定url的网页内容
+    下载器可能自身具备下载功能，也可能是作为与下载中心交互的接口
+    """
+
+    def __init__(self):
+        pass
+
+    def set(self, headers, config={}, urls=[]):
+        """
+        设置http头或者将相关配置发到下载中心
+        Args:
+            headers: 字典，http头信息，
+                举例，{'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; WOW64; rv:47.0) Gecko/20100101 Firefox/47.0'}
+            config: 字典，可为空，用于向下载中心发送下载类型、优先级、抓取频率等相关信息，
+                或者向下载函数设置超时等相关信息，
+                举例：{'type':0, 'priority':5, 'frequency':1} 或 {'timeout':10}
+            urls: 数组，不使用下载中心则为空，用于将待下载的url预先发到下载中心进行下载
+        Returns:
+            1: 正常, 0: 出错
+        """
+        return 0
+
+    def get(self, url):
+        """
+        下载特定url的页面或者向下载中心请求特定url的结果
+        Args:
+            url: 要获取结果的一个url
+        Returns :
+            None: 未取到结果，可能是下载中心还没有下载完成
+            文本: 下载结果
+        """
+        return None
+
+
+class SpiderExtractor(object):
+    """
+    解析器的抽象类
+    用于将特定网页解析成结构化信息
+    每个页面有一个独立的SpiderExtractor类
+    """
+
+    def __init__(self):
+        pass
+
+    def extractor(self, text):
+        """
+        将一个页面文本解析为结构化信息的字典
+        Args:
+            text: 需要解析的文本
+        Returns:
+            数组: 每条为一个完整记录，记录由字典格式保存
+        """
+        return []
+
+
+class SpiderStore(object):
+    """
+    存储器的抽象类
+    用于将结构化信息保存到指定存储媒介中
+    Attributes:
+        fields: 用于保持抽取器字典的key与数据库字段的对应关系，
+            如果结果字典的某个key不包含在fields中，则将直接使用key作为字段名
+    """
+
+    def __init__(self):
+        self.fields = {}
+        pass
+
+    def store(self, results, type=1, keys=[]):
+        """
+        将一个数组存储到指定的存储媒介中
+        Args:
+            reuslts: 数组，每条为一个完整记录，记录由字典格式保存
+            type: 1-只插入（出错则忽略），2-只更新（原记录不存在则忽略），3-插入更新（无记录则插入，有记录则更新）
+            keys: 只插入则为空，更新则存储关键字典，此字段将作为更新的where条件
+        Returns:
+            1: 正常, 0: 出错
+        """
+        pass
+
+
+class Spider(object):
+    """
+    爬虫的抽象类
+    Attributes:
+        headers: http头，同SpiderDownloader
+        config: 抓取配置，同SpiderDownloader
+        urls: 待抓取url，同SpiderDownloader
+        downloader: 下载器，通常一个Spider配一个下载器
+        extractor: 解析器，一个Spider可以配多个解析器
+        store: 存储器，通常一个Spider配一个存储器
+    """
+
+    def __init__(self):
+        self.headers = {}
+        self.config = {}
+        self.urls = []
+        self.downloader = SpiderDownloader()
+        self.extractor = SpiderExtractor()
+        self.store = SpiderStore()
+        pass
+
+    def get_seeds(self):
+        """
+        获取urls
+        """
+        f = open('seeds.txt')
+        for line in f:
+            self.urls.append(line[:-1])
+        f.close()
+
+    def prepare(self):
+        """
+        用于对接下载中心的异步抓取，作为独立操作运行，投递任务后即退出
+        """
+        self.get_seeds()
+        self.downloader.set(self.headers, self.config, self.urls)
+
+    def run(self):
+        """
+        运行主函数，可独立运行（独立下载器模式），也可放在prepare之后运行（下载中心模式）
+        """
+        self.get_seeds()
+        for url in self.urls:
+            content = self.downloader.get(url)
+            results = self.extractor.extractor(content)
+            if len(results) > 0:
+                self.store.store(results)
+
+    def test(self, url):
+        """
+        测试单体url的结果
+        """
+        content = self.downloader.get(url)
+        results = self.extractor.extractor(content)
+        print(results)
+
+
+"""
+def Main():
+    s = Spider()
+    #s.prepare
+    s.run()
+
+if __name__ == "__main__":
+    Main();
+"""
```

### Comparing `download-center-5.3.9/download_center/new_spider/util/util_baidu.py` & `download-center-5.4.0/download_center/new_spider/util/util_baidu.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,812 +1,812 @@
-# -*- coding: utf8 -*-
-"""
-duquan
-2019/12/19
-百度移动端解析工具
-"""
-import json
-import random
-import re
-import uuid
-
-import pymysql
-import requests
-from lxml import etree
-import redis
-import time
-
-from lxml.html import fromstring
-
-import download_center.config as pro_config
-from download_center.store import config
-from http import cookiejar
-from urllib.request import Request, HTTPCookieProcessor, build_opener
-
-from pymysql.converters import escape_string
-
-
-class UtilBaiduMb(object):
-    def __init__(self):
-        self.mobile_useragent_list = [
-            "Mozilla/5.0 (Linux; U; Android 5.0.2; zh-CN; Letv X501 Build/DBXCNOP5501304131S) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 UCBrowser/10.10.0.800 U3/0.8.0 Mobile Safari/534.30",
-            "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Mobile Safari/533.36",
-            "Mozilla/5.0 (Linux; U; Android 5.0.2; zh-cn; Letv X501 Build/DBXCNOP5501304131S) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/6.7 Mobile Safari/537.36",
-            "Mozilla/5.0 (Linux; U; Android 4.3; zh-cn; N5117 Build/JLS36C) AppleWebKit/534.24 (KHTML, like Gecko) Version/4.0 Mobile Safari/534.24 T5/2.0 baiduboxapp/7.0 (Baidu; P1 4.3)",
-            "Mozilla/5.0 (iPhone; CPU iPhone OS 9_2_1 like Mac OS X; zh-CN) AppleWebKit/537.51.1 (KHTML, like Gecko) Mobile/13D15 UCBrowser/10.9.15.793 Mobile",
-            "Mozilla/5.0 (iPhone 6p; CPU iPhone OS 9_2_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/6.0 MQQBrowser/6.7 Mobile/13D15 Safari/8536.25 MttCustomUA/2",
-            "Mozilla/5.0 (iPhone; CPU iPhone OS 9_2_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13D15 Safari/601.1",
-            "Mozilla/5.0 (Linux; U; Android 4.1.2; zh-cn; GT-S7572 Build/JZO54K) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/6.7 Mobile Safari/537.36",
-            "Mozilla/5.0 (Linux; U; Android 5.1.1; zh-cn; SM-J3109 Build/LMY47X) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/6.6 Mobile Safari/537.36",
-            "Mozilla/5.0 (Linux; U; Android 4.4.4; zh-cn; Coolpad 8297-T01 Build/KTU84P) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/6.6 Mobile Safari/537.36",
-            "Mozilla/5.0 (Linux; U; Android 5.1.1; zh-CN; MX4 Pro Build/LMY48W) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 UCBrowser/10.10.0.800 U3/0.8.0 Mobile Safari/534.30",
-            "Mozilla/5.0 (Linux; Android 5.1; m2 note Build/LMY47D) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/40.0.2214.114 Mobile Safari/537.36",
-            "Mozilla/5.0 (Linux; U; Android 5.1; zh-CN; m2 note Build/LMY47D) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 UCBrowser/10.9.10.788 U3/0.8.0 Mobile Safari/534.30",
-            "Mozilla/5.0 (Linux; U; Android 5.1; zh-cn; m2 note Build/LMY47D) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/6.6 Mobile Safari/537.36",
-            "Mozilla/5.0 (Linux; U; Android 4.4.4; zh-cn; CHM-CL00 Build/CHM-CL00) AppleWebKit/534.24 (KHTML, like Gecko) Version/4.0 Mobile Safari/534.24 T5/2.0 baiduboxapp/7.1 (Baidu; P1 4.4.4)",
-            "Mozilla/5.0 (Linux; Android 5.0.1; HUAWEI GRA-TL00 Build/HUAWEIGRA-TL00) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/37.0.0.0 Mobile Safari/537.36 MxBrowser/4.5.9.3000",
-            "Mozilla/5.0 (Linux; U; Android 4.4.2; zh-cn; HUAWEI P6-C00 Build/HuaweiP6-C00) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/6.7 Mobile Safari/537.36",
-            "Mozilla/5.0 (Linux; Android 5.1.1; KIW-CL00 Build/HONORKIW-CL00) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/35.0.1916.138 Mobile Safari/537.36 T7/7.1 baidubrowser/7.1.12.0 (Baidu; P1 5.1.1)",
-            "Mozilla/5.0(Linux;Android 5.1.1;OPPO A33 Build/LMY47V;wv) AppleWebKit/537.36(KHTML,link Gecko) Version/4.0 Chrome/43.0.2357.121 Mobile Safari/537.36 LieBaoFast/4.51.3",
-            "Mozilla/5.0(Linux;U;Android 5.1.1;zh-CN;OPPO A33 Build/LMY47V) AppleWebKit/537.36(KHTML,like Gecko) Version/4.0 Chrome/40.0.2214.89 UCBrowser/11.7.0.953 Mobile Safari/537.36",
-            "Mozilla/5.0 (Linux; Android 4.3; EVO Build/JSS15Q) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/34.0.1847.114 Mobile Safari/537.36",
-            "Mozilla/5.0(Linux;Android 5.1.1;OPPO A33 Build/LMY47V;wv) AppleWebKit/537.36(KHTML,link Gecko) Version/4.0 Chrome/53.0.2785.49 Mobile MQQBrowser/6.2 TBS/043508 Safari/537.36 MicroMessenger/6.5.13.1100 NetType/WIFI Language/zh_CN",
-            "Mozilla/5.0 (Linux; Android 7.0; FRD-AL00 Build/HUAWEIFRD-AL00; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/53.0.2785.49 Mobile MQQBrowser/6.2 TBS/043602 Safari/537.36 MicroMessenger/6.5.16.1120 NetType/WIFI Language/zh_CN",
-            "Mozilla/5.0 (Linux; U; Android 2.3.7; en-us; Nexus One Build/FRF91) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1",
-            "MQQBrowser/26 Mozilla/5.0 (Linux; U; Android 2.3.7; zh-cn; MB200 Build/GRJ22; CyanogenMod-7) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1",
-            "Opera/9.80 (Android 2.3.4; Linux; Opera Mobi/build-1107180945; U; en-GB) Presto/2.8.149 Version/11.10",
-            "Mozilla/5.0 (Linux; U; Android 3.0; en-us; Xoom Build/HRI39) AppleWebKit/534.13 (KHTML, like Gecko) Version/4.0 Safari/534.13",
-            "Mozilla/5.0 (BlackBerry; U; BlackBerry 9800; en) AppleWebKit/534.1+ (KHTML, like Gecko) Version/6.0.0.337 Mobile Safari/534.1+",
-            "Mozilla/5.0 (compatible; MSIE 9.0; Windows Phone OS 7.5; Trident/5.0; IEMobile/9.0; HTC; Titan)",
-            "Mozilla/5.0 (Linux; U; Android 2.2.1; zh-cn; HTC_Wildfire_A3333 Build/FRG83D) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1",
-            "MQQBrowser/26 Mozilla/5.0 (Linux; U; Android 2.3.7; zh-cn; MB200 Build/GRJ22; CyanogenMod-7) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1",
-            "Mozilla/5.0 (Androdi; Linux armv7l; rv:5.0) Gecko/ Firefox/5.0 fennec/5.0",
-            "Mozilla/4.0 (compatible; MSIE 6.0; ) Opera/UCWEB7.0.2.37/28/999",
-            "Mozilla/5.0 (iPad; CPU OS 9_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13B143 Safari/601.1",
-            "Mozilla/5.0 (iPhone; CPU iPhone OS 9_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13B143 Safari/601.1",
-            "Mozilla/5.0 (Windows Phone 10.0; Android 4.2.1; Microsoft; Lumia 950) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/46.0.2486.0 Mobile Safari/537.36 Edge/14.14263",
-            "Mozilla/5.0 (Linux; U; Android 4.4.4; zh-cn; HTC_D820u Build/KTU84P) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Mobile Safari/534.30",
-            "Mozilla/5.0 (iPhone 5SGLOBAL; CPU iPhone OS 8_0 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) Version/6.0 MQQBrowser/5.6 Mobile/12A365 Safari/8536.25",
-            "Mozilla/5.0 (iPhone; CPU iPhone OS 8_0 like Mac OS X) AppleWebKit/600.1.4.9 (KHTML, like Gecko) Version/6.0 Mobile/10A523 Safari/8536.25",
-            "Mozilla/5.0 (iPhone; CPU iPhone OS 8_0 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) Coast/4.01.88243 Mobile/12A365 Safari/7534.48.3",
-            "Mozilla/5.0 (Linux; U; Android 6.0.1; zh-cn; vivo Xplay6 Build/MXB48T) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/7.6 Mobile Safari/537.36",
-            "Mozilla/5.0 (Linux; U; Android 6.0.1; zh-CN; F5121 Build/34.0.A.1.247) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/40.0.2214.89 UCBrowser/11.5.1.944 Mobile Safari/537.36",
-            "Mozilla/5.0 (iPhone; CPU iPhone OS 10_2 like Mac OS X) AppleWebKit/602.3.12 (KHTML, like Gecko) Mobile/14C92 MicroMessenger/6.5.9 NetType/WIFI Language/zh_CN",
-            "Mozilla/5.0 (Linux; U; Android 5.1.1; zh-cn; YQ601 Build/LMY47V) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 UCBrowser/1.0.0.100 U3/0.8.0 Mobile Safari/534.30 AliApp(TB/6.4.3) WindVane/8.0.0 1080X1920 GCanvas/1.4.2.21",
-            "Mozilla/5.0 (Linux; U; Android 7.0; zh-cn; MI 5 Build/NRD90M) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/7.1 Mobile Safari/537.36"
-        ]
-
-    # -  资讯
-    def container_mb_zixun(self, container):
-        try:
-            item_list = list()
-            news_list = container.xpath('.//div[contains(@class,"c-gap-inner-top-middle tts-b-item")]')
-            for news in news_list:
-                try:
-                    title = news.xpath('string(.//h3/span)')
-                    show_url = news.xpath('string(.//div[contains(@data-module,"c-sr")])')
-                    baidu_url = news.xpath('./a/@href')[0]
-                    real_url = self.get_real_url_by_baidu_url(baidu_url)
-                    if real_url == '':
-                        real_url = baidu_url
-                    datas = {
-                        'title': title,
-                        'baidu_url': baidu_url,
-                        'show_url': show_url,
-                        'real_url': real_url,
-                    }
-                    item_list.append(datas)
-                except:
-                    pass
-        except:
-            return []
-        else:
-            return item_list
-
-    # -  两行图片
-    def container_mb_image(self, container):
-        try:
-            item_list = list()
-            news_list = container.xpath('.//div[contains(@class,"c-img image-img-item")]')
-            for image_list in news_list:
-                try:
-                    exposure = image_list.get("data-exposure", "")
-                    baidu_url = json.loads(str(exposure).replace("\'", "\""))['loc']
-                    title = ''
-                    show_url = ''
-                    real_url = baidu_url
-                    datas = {
-                        'title': title,
-                        'baidu_url': baidu_url,
-                        'show_url': show_url,
-                        'real_url': real_url,
-                    }
-                    item_list.append(datas)
-                except:
-                    pass
-        except:
-            return []
-        else:
-            return item_list
-
-    # -  视频
-    def container_mb_video(self, container):
-        try:
-            item_list = list()
-            news_list = container.xpath('.//div[contains(@class,"c-video-container")]/a')
-            for video_list in news_list:
-                title = video_list.xpath('string(.//div[contains(@class,"c-vid-title")])')
-                baidu_url = video_list.xpath('./@href')[0]
-                show_url = ""
-                datalog = video_list.get("data-log", "")
-                real_url = baidu_url
-                try:
-                    datalog = str(datalog).replace("\'", "\"")
-                    sx_data = json.loads(datalog)
-                    real_url = sx_data["mu"]
-                except:
-                    pass
-
-                datas = {
-                    'title': title,
-                    'baidu_url': baidu_url,
-                    'show_url': show_url,
-                    'real_url': real_url,
-                }
-                item_list.append(datas)
-        except:
-            return []
-        else:
-            return item_list
-
-    # 小视频
-    def container_mb_small_video(self, container):
-        try:
-            item_list = list()
-            # news_list = container.xpath('//div[@tpl="vid_pocket"]//div[@class="vid-scroll-content"]')
-            news_list = container.xpath('//div[@tpl="vid_pocket"]//div[@class="c-scroll-item"]')
-            for video_list in news_list:
-                try:
-                    see_more = video_list.xpath('.//div[@class="_v1-pF"]')
-                    if not see_more:
-                        title = ''.join(video_list.xpath('string(.//div[@class="vid-pocket-item"]/div[2]/div)'))
-                        baidu_url = ''
-                        show_url = ''.join(video_list.xpath('.//div[@class="vid-pocket-item"]/div[1]/div//span[contains(@class,"vid-info-author-name")]/text()')[0])
-                        real_url = ''.join(video_list.xpath('.//a[@class="c-blocka"]/@href'))
-                        datas = {
-                            'title': title,
-                            'baidu_url': baidu_url,
-                            'show_url': show_url,
-                            'real_url': real_url,
-                        }
-                        item_list.append(datas)
-                except:
-                    continue
-        except:
-            return []
-        else:
-            return item_list
-
-    def container_mb_notes(self, container):
-        try:
-            item_list = list()
-            news_list = container.xpath("//div[@class='text-list-inner']/div[contains(@data-module,'lgtlt')]")
-            for video_list in news_list:
-                title = video_list.xpath('./div/@titlehtml')
-                show_desc = video_list.xpath('./div/@deschtml')
-                baidu_url = video_list.xpath('./div/@rl-link-href')
-                real_url = video_list.xpath('./div/@rl-link-data-click')
-                show_url = ''
-                if real_url:
-                    data = json.loads(real_url[0])
-                    show_url = data.get('src', '')
-                datas = {
-                    'title': title,
-                    'show_desc': show_desc,
-                    'baidu_url': baidu_url,
-                    'show_url': show_url,
-                }
-                item_list.append(datas)
-        except:
-            return []
-        else:
-            return item_list
-
-    # 直播
-    def container_mb_zhibo(self, container):
-        try:
-            item_list = list()
-            news_list = container.xpath('//div[@tpl="live_converge"]//div[@class="c-scroll-item"]')
-            for video_list in news_list:
-                title = video_list.xpath('string(.//span[contains(@class,"c-abstract")])')
-                baidu_url = ''.join(video_list.xpath('.//a/@href'))
-                show_url = ''
-                datas = {
-                    'title': title,
-                    'baidu_url': baidu_url,
-                    'show_url': show_url,
-                }
-                item_list.append(datas)
-        except:
-            return []
-        else:
-            return item_list
-
-    def get_container_list(self, html):
-        """获取搜索结果列表元素"""
-        try:
-            html_element = fromstring(html.encode('utf-8', 'ignore').decode('utf-8', 'ignore'))
-            container_list = html_element.xpath('//div[@id="results"]/div[contains(@class,"c-result")]')
-        except:
-            return -1
-        else:
-            return container_list
-
-    # def get_container_list(self, html):
-    #     """获取搜索结果列表元素"""
-    #     try:
-    #         html_element = etree.HTML(html, etree.HTMLParser(encoding="utf-8"))
-    #         container_list = html_element.xpath('//div[contains(@class,"c-result")]')
-    #     except:
-    #         return -1
-    #     else:
-    #         return container_list
-
-    def get_rank(self, container):
-        """获取排名"""
-        try:
-            rank = int(container.xpath('./@order')[0])
-        except:
-            return 0
-        else:
-            return rank
-
-    def get_real_url_by_json(self, container):
-        """通过json，获取真实url"""
-        try:
-            real_url = ""
-            datalog = container.get("data-log", "")
-            if datalog:
-                try:
-                    datalog = str(datalog).replace("\'", "\"")
-                    sx_data = json.loads(datalog)
-                    real_url = sx_data["mu"]
-                except:
-                    pass
-            if real_url == "" or real_url == "notes.baidu.com":
-                try:
-                    article_list = container.xpath('.//article/@rl-link-href')
-                    if len(article_list) > 0:
-                        url = article_list[0]
-                        headers = {
-                            "User-Agent": "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1"
-                        }
-                        response = requests.get(url=url, headers=headers)
-                        if "window.location.replace" in response.text:
-                            url_list = re.findall(r'.*url=(.*?)".*', response.text)
-                            if len(url_list) > 0:
-                                url = url_list[0]
-                                real_url = url
-                except:
-                    pass
-        except Exception as e:
-            return -1
-        else:
-            return real_url
-
-    def get_real_url_by_baidu_url(self, baidu_url, try_count=1):
-        """通过百度url获取真实url"""
-        try:
-            if try_count > 3:
-                return ''
-            else:
-                headers = {
-                    'User-Agent': random.choice(self.mobile_useragent_list),
-                    "Cookie": self.get_cook()
-                }
-                response = requests.get(baidu_url, headers=headers, timeout=20)
-                if response.status_code > 400:
-                    print('获取real_url失败 - {}'.format(response.status_code))
-                    return self.get_real_url_by_baidu_url(baidu_url, try_count + 1)
-                return response.url
-        except Exception:
-            return self.get_real_url_by_baidu_url(baidu_url, try_count + 1)
-
-    # 判断是否需要获取真实url - （需要获取真实url情况：完全匹配， show_url不是url格式）
-    def check_get_real_url(self, container, real_url):
-        # 取页面上的真实url
-        datalog = container.get("data-log", "")
-        if datalog:
-            try:
-                datalog = str(datalog).replace("\'", "\"")
-                sx_data = json.loads(datalog)
-                real_url = sx_data["mu"]
-            except:
-                return -1
-        return real_url
-
-    def get_baidu_url(self, container):
-        """获取百度url"""
-        xpath_rules = ['.//header[@class="c-gap-bottom-small"]//a[1]/@href',
-                       './/div[@class="circle-sample"]//a[1]/@href',
-                       './/article/@rl-link-href']
-        return self.get_res_text(container, xpath_rules)
-
-    def get_show_url(self, container):
-        """获取显示url"""
-        xpath_rules = [
-            './/div[contains(@class,"android-text-top1")]//text()',
-            './/span[contains(@class,"android-text-top1")]//text()',
-            './/span[contains(@class,"c-showurl")]//text()',
-            './/div[contains(@class,"c-showurl")]//text()',
-            './/span[@class="c-color-gray"]//text()',
-            './/div[@class="c-line-clamp1"]//text()',
-        ]
-        return remove_special_characters(self.get_res_text(container, xpath_rules))
-
-    def get_show_title_mb(self, container):
-        """获取标题"""
-        xpath_rules = ['.//span[@class="c-line-clamp1"]//text()',
-                       './/header//span[@class="c-title-text"]//text()',
-                       './/span[@class="c-title-text"]//text()',
-                       './/h3[@class="c-title title-con"]//text()',
-                       './/span[@class="_1mmq3"]//text()',
-                       './/div[@class="c-line-clamp1"][1]//text()',
-                       './/div[@class="ugc-title__2ofi_"]//text()',
-                       './/div[contains(@class,"c-title")]//text()',
-                       '//div[@class="c-span7"]/div[contains(@class,"c-font-large")]/text()',
-                       'string(//div[contains(@class,"ugc-title")])',
-                       ".//div[@class='text-list-inner']/div[@class='text-item tts-b-item']"
-
-                       ]
-        return self.get_res_text_mb(container, xpath_rules)
-
-    def get_res_text_mb(self, container, xpath_rules):
-        """获取纯文本"""
-        text = ""
-        for rule in xpath_rules:
-            text_list = container.xpath(rule)
-            for i in text_list:
-                text += i.strip().strip('”').strip('“')
-            if text != "":
-                return escape_string(text)
-        return escape_string(text)
-
-    def get_show_desc(self, container):
-        """获取描述"""
-        xpath_rules = ['.//div[@class="c-line-clamp3"]//text()',
-
-                       './/span[@class="c-font-big wenda-abstract-quote"]/text()',
-                       './/div[@class="c-line-clamp2"]//text()',
-                       './/section//span//text()',
-                       './/div[@class="c-font-medium c-color c-gap-bottom-small wenda-abstract-text wenda-abstract-singo-line c-color-link"]//text()',
-                       './/div[@class="c-abstract c-gap-bottom wa-bk-polysemy-abstract c-line-clamp5"]//text()']
-        return self.get_res_text(container, xpath_rules)
-
-    def get_show_date(self, container):
-        """获取显示日期"""
-        xpath_rules = ['.//span[@class="c-gap-right-small"]//text()',
-                       './/span[@class="c-color-gray c-gap-left normal-footer-no-shrink"]//text()',
-                       './/span[@class="c-footer-showurl c-gap-left"]//text()',
-                       ]
-        res = self.get_res_text(container, xpath_rules)
-        if "回答时间：" in res:
-            return res.split("回答时间：")[-1]
-        elif "发贴时间" in res:
-            return res.split("发贴时间:")[-1]
-        else:
-            return res.replace('发布时间: ', '')
-
-    def get_res_text(self, container, xpath_rules):
-        """获取纯文本"""
-        text = ""
-        for rule in xpath_rules:
-            text_list = container.xpath(rule)
-            for i in text_list:
-                text += i.strip().strip('”').strip('“')
-            if text != "":
-                break
-        return escape_string(text)
-
-    def get_mb_cookie(self):
-        cookies = None
-        try:
-            cookie_jar = cookiejar.CookieJar()
-            request = Request('https://m.baidu.com/tc?tcreq4log=1', headers={})
-            handlers = [HTTPCookieProcessor(cookie_jar)]
-            opener = build_opener(*handlers)
-            opener.open(request, timeout=10)
-            for cookie in cookie_jar:
-                if cookie.name == 'BDORZ':
-                    cookies = 'BDORZ=' + cookie.value
-                    break
-        except Exception:
-            pass
-        return cookies
-
-    def get_cook(self):
-        """
-        获取有效的cookie
-        :return:
-        """
-        try:
-            key_name = 'mb'
-            for i in range(2):
-                if UtilBaiduCookie().totalCookies(key_name) > 0:
-                    cookie = str(UtilBaiduCookie().getLastCookies(key_name=key_name)[0], encoding="utf-8")
-                    return cookie
-                else:
-                    return self.get_mb_cookie()
-        except:
-            return self.get_mb_cookie()
-
-
-class UtilBaiduPc(object):
-    def get_container_list(self, html):
-        """获取搜索结果列表元素"""
-        try:
-            # html_element = etree.HTML(html, etree.HTMLParser(encoding="utf-8"))
-            # container_list = html_element.xpath('//div[@id="content_left"]/div')
-            # return container_list
-            html_element = fromstring(html)
-            container_list = html_element.xpath('//div[@id="content_left"]/div[contains(@class,"new-pmd")]')
-            return container_list
-        except:
-            return -1
-
-    def get_rank(self, container):
-        """获取排名"""
-        try:
-            rank = int(container.get('id', 0))
-            return rank
-        except:
-            return 0
-
-    # 最新相关信息
-    def container_pc_news(self, container):
-        try:
-            item_list = list()
-            news_list = container.xpath('//div[@tpl="news-realtime"]/div/div')
-            for i in news_list:
-                try:
-                    a_list = i.xpath('./a')
-                    if a_list:
-                        title = ''.join(a_list[0].xpath('string(.)'))
-                        baidu_url = a_list[0].xpath('./@href')[0]
-                        try:
-                            show_url = i.xpath('./span[@class="c-color-gray c-gap-left-small"]/text()')[0]
-                        except:
-                            show_url = i.xpath('./div/span[@class="c-color-gray"]/text()')[0]
-                        datas = {
-                            'title': title,
-                            'baidu_url': baidu_url,
-                            'show_url': show_url
-                        }
-                        item_list.append(datas)
-                except:
-                    continue
-        except:
-            return []
-        else:
-            return item_list
-
-    # 高清在线观看
-    def container_pc_video(self, html):
-        try:
-            item_list = list()
-            video_list = json.loads(re.findall('"videoList":(\[.*?\])', html)[0])
-
-            for i in video_list:
-                title = i.get('title', '')
-                baidu_url = i.get('jumpUrl', '')
-                show_url = i.get('source', '')
-                datas = {
-                    'title': title,
-                    'baidu_url': baidu_url,
-                    'show_url': show_url
-                }
-                item_list.append(datas)
-        except:
-            return []
-        else:
-            return item_list
-
-        # 最新相关信息
-
-    def container_pc_tieba(self, container):
-        try:
-            item_list = list()
-            tieba_list = container.xpath('//div[@tpl="tieba_general"]/div[@class="result c-container"]/div[contains(@class,"c-row")]')
-            for i in tieba_list:
-                a_list = i.xpath('./div[contains(@class,"c-span8")]')
-                if a_list:
-                    title = ''.join(a_list[0].xpath('string(./a)'))
-                    baidu_url = a_list[0].xpath('./a/@href')[0]
-                    datas = {
-                        'title': title,
-                        'baidu_url': baidu_url,
-                    }
-                    item_list.append(datas)
-        except:
-            return []
-        else:
-            return item_list
-
-    def get_show_url(self, container):
-        """获取显示url"""
-        xpath_rules = [
-            './/span[@class="nor-src-wrap"]//text()',
-            './/div[contains(@class,"se_st_footer")]/a[1]//text()',
-            './/div[@class="f13"]/a[1]/text()',
-            './/span[@class="c-showurl"]//text()',
-            './/a[@class="c-showurl"]/span//text()',
-            './/div[@class="f13"]/span//text()',
-            './/a[@class="c-showurl"]//text()',
-            './/a[@class="c-showurl "]//text()',
-            './/div[contains(@class,"c-showurl")]//text()',
-            './/section/a/div//text()',
-            'string(//div[@class="vmp-zxenterprise-new_qayMC"]/div/h3/a/@href)',
-            'string(//h3[@class="c-title"]/span)'
-        ]
-        return remove_special_characters(self.get_res_text(container, xpath_rules))
-
-    def get_show_title(self, container):
-        """获取标题"""
-        # xpath_rules = ['.//h3//text()', './/span[@class="c-title-text"]//text()',
-        #                './/div[@class="wenda-abstract-showurl-title c-line-clamp1"]//text()',
-        #                './/h3[@class="t c-gap-bottom-small"]//text()',
-        #                '//h3[@role="text"]/span[@class="c-title-text"]//text()']
-        xpath_rules = ['.//span[@class="c-title-text"]//text()', './/div[@class="c-line-clamp1"]//text()',
-                       './/div[@class="c-font-medium c-color-t"]//text()',
-                       './/div[@class="wenda-abstract-showurl-title c-line-clamp1"]//text()',
-                       './/h3[@class="t c-gap-bottom-small"]//text()', './/h3[contains(@class,"t")]//text()',
-                       'string(//span[@class="c-title-text"])', 'string(//div[@class="vmp-zxenterprise-new_qayMC"]/div/h3/a)',
-                       'string(//div[@tpl="wenda_abstract_pc"]//div[contains(@class,"wenda-abstract-wrap-new")]//a)', 'string(//span[@class="c-title-text"])',
-                       'string(//div[@tpl="vmp_zxenterprise_new"]//h3/a)']
-        return self.get_res_text(container, xpath_rules)
-
-    def get_show_desc(self, container):
-        """获取描述"""
-        try:
-            des_list = container.cssselect("div.c-abstract")
-            if len(des_list) > 0:
-                des = self.get_text(des_list[0])
-            else:
-                des_list = container.cssselect("div.c-span18c-span-last")
-                if len(des_list) > 0:
-                    des = self.get_text(des_list[0])
-                else:
-                    des_list = container.cssselect("div.c-gap-top-small")
-                    if des_list:
-                        des = self.get_text(des_list[0])
-                    else:
-                        des = ''
-        except:
-            return ''
-        else:
-            return des
-
-    def get_text(self, elem):
-        rc = []
-        for node in elem.itertext():
-            rc.append(node.strip())
-        return ''.join(rc)
-
-    def get_baidu_url(self, container):
-        """获取百度url"""
-        xpath_rules = [
-            './/h3[contains(@class,"t")]/a/@href',
-            './/a[@class="c-showurl"]/@href',
-            './/span[@class="c-showurl"]/text()',
-            './/h3[@class="t c-gap-bottom-small"]/a/@href',
-            './/section/a/@href',
-            '//div[@tpl="ads_b2c_universal_card"]//a[@data-module="c-t"]/@href',
-            '//*[@id="1"]/div/article/section/div/div[1]/a/@href',
-            '//header[@class="c-gap-bottom-small"]/div/a[@class="c-blocka"]/@href',
-            '//div[@tpl="wenda_abstract_pc"]//div[contains(@class,"wenda-abstract-wrap-new")]//a/@href',
-            '//div[@tpl="ads_b2c_universal_card"]//header[@class="c-gap-bottom-small"]//a/@href',
-            '//div[@tpl="vmp_zxenterprise_new"]//h3/a/@href'
-        ]
-        return self.get_res_text(container, xpath_rules)
-
-    def get_show_date(self, container):
-        """获取显示日期"""
-        try:
-            des_list = container.cssselect("div.c-abstract")
-            if len(des_list) > 0:
-                show_date_eles = des_list[0].xpath('descendant::span')
-                if show_date_eles:
-                    show_date = show_date_eles[0].text.strip()
-                    show_date = str(show_date).split("-")[0].strip().replace(" ", "")
-                else:
-                    show_date = ''
-            else:
-                des_list = container.cssselect("div.c-span18c-span-last")
-                if len(des_list) > 0:
-                    show_date_eles = des_list[0].xpath('descendant::span[@class="m"]')
-                    if show_date_eles:
-                        show_date = show_date_eles[0].text.strip()
-                        show_date = str(show_date).split("-")[0].strip().replace(" ", "")
-                    else:
-                        show_date = ''
-                else:
-                    des_list = container.cssselect("div.c-gap-top-small")
-                    if des_list:
-                        show_date_eles = des_list[0].xpath('descendant::span')
-                        if show_date_eles:
-                            show_date = show_date_eles[0].text.strip()
-                            show_date = str(show_date).split("-")[0].strip().replace(" ", "")
-                        else:
-                            show_date = ''
-                    else:
-                        show_date = ''
-        except AttributeError:
-            return ''
-        else:
-            return show_date.replace('最佳答案:', '')
-
-    def get_snapshoot_url(self, container):
-        try:
-            """获取快照url"""
-            xpath_rules = [
-                './/div[contains(@class,"se_st_footer")]/a[contains(@class,"m")]/@href',
-                './/div[@class="g"]/a[@class="m"]',
-                './/a[@class="m"]/@href'
-            ]
-            return self.get_res_text(container, xpath_rules)
-        except:
-            return ''
-
-    def get_res_text(self, container, xpath_rules):
-        text = ""
-        for rule in xpath_rules:
-            text_list = container.xpath(rule)
-            for i in text_list:
-                text += i.strip()
-            if text != "":
-                break
-        return escape_string(text)
-
-    def get_real_url(self, baidu_url, try_count=1, timeout=5):
-        max_retry_num = 3
-        if try_count > max_retry_num:
-            return ''
-
-        headers = {
-            "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.110 Safari/537.36"
-        }
-        try:
-            response = requests.get(baidu_url, headers=headers, timeout=timeout, allow_redirects=False)
-            if response.status_code == 302:
-                return response.headers['Location']
-            elif response.status_code == 200:
-                res = requests.get(baidu_url, headers=headers, timeout=timeout, allow_redirects=True)
-                return res.url
-            else:
-                return self.get_real_url(baidu_url, try_count + 1)
-                # return ''
-        except Exception as err:
-            return self.get_real_url(baidu_url, try_count + 1)
-            # return ''
-
-    def get_cook(self):
-        """
-        获取有效的cookie
-        :return:
-        """
-        try:
-            key_name = 'pc'
-            for i in range(2):
-                if UtilBaiduCookie().totalCookies(key_name) > 0:
-                    cookie = str(UtilBaiduCookie().getLastCookies(key_name=key_name)[0], encoding="utf-8")
-                    return cookie
-                else:
-                    print('pc no use cookie')
-                    return 'BAIDUID={}:FG=1; BIDUPSID={};'.format(uuid.uuid1(), uuid.uuid4())
-        except:
-            return 'BAIDUID={}:FG=1; BIDUPSID={};'.format(uuid.uuid1(), uuid.uuid4())
-
-
-class UtilBaiduCookie(object):
-    def __init__(self):
-        self.redisPool = redis.ConnectionPool(**(config.DOWNLOADER_CENTER_REDIS[pro_config.ENVIR]))
-        self.redisClient = redis.StrictRedis(connection_pool=self.redisPool)
-        self.pc_cookie_key = 'baidu:pc:cookies'
-        self.mb_cookie_key = 'baidu:mb:cookies'
-
-    def getCookies(self, num=0, key_name='pc'):
-        '''
-        [获取一个有效的cookie 正序]
-        :param num:
-        :param key_name:
-        :return:
-        '''
-        # noinspection PyBroadException
-        try:
-            if key_name == 'pc':
-                return self.redisClient.zrange(self.pc_cookie_key, 0, num)
-            elif key_name == 'mb':
-                return self.redisClient.zrange(self.mb_cookie_key, 0, num)
-            else:
-                return []
-        except Exception:
-            return []
-
-    def getLastCookies(self, num=0, key_name='pc'):
-        '''
-         [获取最新的cooie]
-        :param num:
-        :param key_name:
-        :return:
-        '''
-        # noinspection PyBroadException
-        try:
-            if key_name == 'pc':
-                return self.redisClient.zrevrange(self.pc_cookie_key, 0, num)
-            elif key_name == 'mb':
-                return self.redisClient.zrevrange(self.mb_cookie_key, 0, num)
-            else:
-                return []
-        except Exception:
-            return []
-
-    def addCookies(self, cookie, key_name='pc'):
-        '''
-        [添加一个值]
-        :param cookie:
-        :param key_name:
-        :return:
-        '''
-        # noinspection PyBroadException
-        try:
-            score = int(round(time.time() * 1000))
-            if key_name == 'pc':
-                return self.redisClient.zadd(self.pc_cookie_key, {cookie: score})
-            elif key_name == 'mb':
-                return self.redisClient.zadd(self.mb_cookie_key, {cookie: score})
-            else:
-                return 0
-        except Exception:
-            return 0
-
-    def delCookies(self, cookie, key_name='pc'):
-        '''
-        删除cookie
-        :param cookie:
-        :return:
-        '''
-        # noinspection PyBroadException
-        try:
-            if key_name == 'pc':
-                return self.redisClient.zrem(self.pc_cookie_key, cookie)
-            elif key_name == 'mb':
-                return self.redisClient.zrem(self.mb_cookie_key, cookie)
-            else:
-                return 0
-        except Exception:
-            return 0
-
-    def totalCookies(self, key_name='pc'):
-        '''
-        [统计个数]
-        :return:
-        '''
-        # noinspection PyBroadException
-        try:
-            if key_name == 'pc':
-                return self.redisClient.zcard(self.pc_cookie_key)
-            elif key_name == 'mb':
-                return self.redisClient.zcard(self.mb_cookie_key)
-            else:
-                return 0
-        except Exception:
-            return 0
-
-
-def remove_special_characters(text):
-    text = text.replace("<b>", "")
-    text = text.replace("</b>", "")
-    text = text.replace("&nbsp", "")
-    text = text.replace("›", "/")
-    text = text.replace("...", "")
-    text = text.replace(" ", "")
-    return text
+# -*- coding: utf8 -*-
+"""
+duquan
+2019/12/19
+百度移动端解析工具
+"""
+import json
+import random
+import re
+import uuid
+
+import pymysql
+import requests
+from lxml import etree
+import redis
+import time
+
+from lxml.html import fromstring
+
+import download_center.config as pro_config
+from download_center.store import config
+from http import cookiejar
+from urllib.request import Request, HTTPCookieProcessor, build_opener
+
+from pymysql.converters import escape_string
+
+
+class UtilBaiduMb(object):
+    def __init__(self):
+        self.mobile_useragent_list = [
+            "Mozilla/5.0 (Linux; U; Android 5.0.2; zh-CN; Letv X501 Build/DBXCNOP5501304131S) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 UCBrowser/10.10.0.800 U3/0.8.0 Mobile Safari/534.30",
+            "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Mobile Safari/533.36",
+            "Mozilla/5.0 (Linux; U; Android 5.0.2; zh-cn; Letv X501 Build/DBXCNOP5501304131S) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/6.7 Mobile Safari/537.36",
+            "Mozilla/5.0 (Linux; U; Android 4.3; zh-cn; N5117 Build/JLS36C) AppleWebKit/534.24 (KHTML, like Gecko) Version/4.0 Mobile Safari/534.24 T5/2.0 baiduboxapp/7.0 (Baidu; P1 4.3)",
+            "Mozilla/5.0 (iPhone; CPU iPhone OS 9_2_1 like Mac OS X; zh-CN) AppleWebKit/537.51.1 (KHTML, like Gecko) Mobile/13D15 UCBrowser/10.9.15.793 Mobile",
+            "Mozilla/5.0 (iPhone 6p; CPU iPhone OS 9_2_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/6.0 MQQBrowser/6.7 Mobile/13D15 Safari/8536.25 MttCustomUA/2",
+            "Mozilla/5.0 (iPhone; CPU iPhone OS 9_2_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13D15 Safari/601.1",
+            "Mozilla/5.0 (Linux; U; Android 4.1.2; zh-cn; GT-S7572 Build/JZO54K) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/6.7 Mobile Safari/537.36",
+            "Mozilla/5.0 (Linux; U; Android 5.1.1; zh-cn; SM-J3109 Build/LMY47X) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/6.6 Mobile Safari/537.36",
+            "Mozilla/5.0 (Linux; U; Android 4.4.4; zh-cn; Coolpad 8297-T01 Build/KTU84P) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/6.6 Mobile Safari/537.36",
+            "Mozilla/5.0 (Linux; U; Android 5.1.1; zh-CN; MX4 Pro Build/LMY48W) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 UCBrowser/10.10.0.800 U3/0.8.0 Mobile Safari/534.30",
+            "Mozilla/5.0 (Linux; Android 5.1; m2 note Build/LMY47D) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/40.0.2214.114 Mobile Safari/537.36",
+            "Mozilla/5.0 (Linux; U; Android 5.1; zh-CN; m2 note Build/LMY47D) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 UCBrowser/10.9.10.788 U3/0.8.0 Mobile Safari/534.30",
+            "Mozilla/5.0 (Linux; U; Android 5.1; zh-cn; m2 note Build/LMY47D) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/6.6 Mobile Safari/537.36",
+            "Mozilla/5.0 (Linux; U; Android 4.4.4; zh-cn; CHM-CL00 Build/CHM-CL00) AppleWebKit/534.24 (KHTML, like Gecko) Version/4.0 Mobile Safari/534.24 T5/2.0 baiduboxapp/7.1 (Baidu; P1 4.4.4)",
+            "Mozilla/5.0 (Linux; Android 5.0.1; HUAWEI GRA-TL00 Build/HUAWEIGRA-TL00) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/37.0.0.0 Mobile Safari/537.36 MxBrowser/4.5.9.3000",
+            "Mozilla/5.0 (Linux; U; Android 4.4.2; zh-cn; HUAWEI P6-C00 Build/HuaweiP6-C00) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/6.7 Mobile Safari/537.36",
+            "Mozilla/5.0 (Linux; Android 5.1.1; KIW-CL00 Build/HONORKIW-CL00) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/35.0.1916.138 Mobile Safari/537.36 T7/7.1 baidubrowser/7.1.12.0 (Baidu; P1 5.1.1)",
+            "Mozilla/5.0(Linux;Android 5.1.1;OPPO A33 Build/LMY47V;wv) AppleWebKit/537.36(KHTML,link Gecko) Version/4.0 Chrome/43.0.2357.121 Mobile Safari/537.36 LieBaoFast/4.51.3",
+            "Mozilla/5.0(Linux;U;Android 5.1.1;zh-CN;OPPO A33 Build/LMY47V) AppleWebKit/537.36(KHTML,like Gecko) Version/4.0 Chrome/40.0.2214.89 UCBrowser/11.7.0.953 Mobile Safari/537.36",
+            "Mozilla/5.0 (Linux; Android 4.3; EVO Build/JSS15Q) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/34.0.1847.114 Mobile Safari/537.36",
+            "Mozilla/5.0(Linux;Android 5.1.1;OPPO A33 Build/LMY47V;wv) AppleWebKit/537.36(KHTML,link Gecko) Version/4.0 Chrome/53.0.2785.49 Mobile MQQBrowser/6.2 TBS/043508 Safari/537.36 MicroMessenger/6.5.13.1100 NetType/WIFI Language/zh_CN",
+            "Mozilla/5.0 (Linux; Android 7.0; FRD-AL00 Build/HUAWEIFRD-AL00; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/53.0.2785.49 Mobile MQQBrowser/6.2 TBS/043602 Safari/537.36 MicroMessenger/6.5.16.1120 NetType/WIFI Language/zh_CN",
+            "Mozilla/5.0 (Linux; U; Android 2.3.7; en-us; Nexus One Build/FRF91) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1",
+            "MQQBrowser/26 Mozilla/5.0 (Linux; U; Android 2.3.7; zh-cn; MB200 Build/GRJ22; CyanogenMod-7) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1",
+            "Opera/9.80 (Android 2.3.4; Linux; Opera Mobi/build-1107180945; U; en-GB) Presto/2.8.149 Version/11.10",
+            "Mozilla/5.0 (Linux; U; Android 3.0; en-us; Xoom Build/HRI39) AppleWebKit/534.13 (KHTML, like Gecko) Version/4.0 Safari/534.13",
+            "Mozilla/5.0 (BlackBerry; U; BlackBerry 9800; en) AppleWebKit/534.1+ (KHTML, like Gecko) Version/6.0.0.337 Mobile Safari/534.1+",
+            "Mozilla/5.0 (compatible; MSIE 9.0; Windows Phone OS 7.5; Trident/5.0; IEMobile/9.0; HTC; Titan)",
+            "Mozilla/5.0 (Linux; U; Android 2.2.1; zh-cn; HTC_Wildfire_A3333 Build/FRG83D) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1",
+            "MQQBrowser/26 Mozilla/5.0 (Linux; U; Android 2.3.7; zh-cn; MB200 Build/GRJ22; CyanogenMod-7) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1",
+            "Mozilla/5.0 (Androdi; Linux armv7l; rv:5.0) Gecko/ Firefox/5.0 fennec/5.0",
+            "Mozilla/4.0 (compatible; MSIE 6.0; ) Opera/UCWEB7.0.2.37/28/999",
+            "Mozilla/5.0 (iPad; CPU OS 9_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13B143 Safari/601.1",
+            "Mozilla/5.0 (iPhone; CPU iPhone OS 9_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13B143 Safari/601.1",
+            "Mozilla/5.0 (Windows Phone 10.0; Android 4.2.1; Microsoft; Lumia 950) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/46.0.2486.0 Mobile Safari/537.36 Edge/14.14263",
+            "Mozilla/5.0 (Linux; U; Android 4.4.4; zh-cn; HTC_D820u Build/KTU84P) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 Mobile Safari/534.30",
+            "Mozilla/5.0 (iPhone 5SGLOBAL; CPU iPhone OS 8_0 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) Version/6.0 MQQBrowser/5.6 Mobile/12A365 Safari/8536.25",
+            "Mozilla/5.0 (iPhone; CPU iPhone OS 8_0 like Mac OS X) AppleWebKit/600.1.4.9 (KHTML, like Gecko) Version/6.0 Mobile/10A523 Safari/8536.25",
+            "Mozilla/5.0 (iPhone; CPU iPhone OS 8_0 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) Coast/4.01.88243 Mobile/12A365 Safari/7534.48.3",
+            "Mozilla/5.0 (Linux; U; Android 6.0.1; zh-cn; vivo Xplay6 Build/MXB48T) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/7.6 Mobile Safari/537.36",
+            "Mozilla/5.0 (Linux; U; Android 6.0.1; zh-CN; F5121 Build/34.0.A.1.247) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/40.0.2214.89 UCBrowser/11.5.1.944 Mobile Safari/537.36",
+            "Mozilla/5.0 (iPhone; CPU iPhone OS 10_2 like Mac OS X) AppleWebKit/602.3.12 (KHTML, like Gecko) Mobile/14C92 MicroMessenger/6.5.9 NetType/WIFI Language/zh_CN",
+            "Mozilla/5.0 (Linux; U; Android 5.1.1; zh-cn; YQ601 Build/LMY47V) AppleWebKit/534.30 (KHTML, like Gecko) Version/4.0 UCBrowser/1.0.0.100 U3/0.8.0 Mobile Safari/534.30 AliApp(TB/6.4.3) WindVane/8.0.0 1080X1920 GCanvas/1.4.2.21",
+            "Mozilla/5.0 (Linux; U; Android 7.0; zh-cn; MI 5 Build/NRD90M) AppleWebKit/537.36 (KHTML, like Gecko)Version/4.0 Chrome/37.0.0.0 MQQBrowser/7.1 Mobile Safari/537.36"
+        ]
+
+    # -  资讯
+    def container_mb_zixun(self, container):
+        try:
+            item_list = list()
+            news_list = container.xpath('.//div[contains(@class,"c-gap-inner-top-middle tts-b-item")]')
+            for news in news_list:
+                try:
+                    title = news.xpath('string(.//h3/span)')
+                    show_url = news.xpath('string(.//div[contains(@data-module,"c-sr")])')
+                    baidu_url = news.xpath('./a/@href')[0]
+                    real_url = self.get_real_url_by_baidu_url(baidu_url)
+                    if real_url == '':
+                        real_url = baidu_url
+                    datas = {
+                        'title': title,
+                        'baidu_url': baidu_url,
+                        'show_url': show_url,
+                        'real_url': real_url,
+                    }
+                    item_list.append(datas)
+                except:
+                    pass
+        except:
+            return []
+        else:
+            return item_list
+
+    # -  两行图片
+    def container_mb_image(self, container):
+        try:
+            item_list = list()
+            news_list = container.xpath('.//div[contains(@class,"c-img image-img-item")]')
+            for image_list in news_list:
+                try:
+                    exposure = image_list.get("data-exposure", "")
+                    baidu_url = json.loads(str(exposure).replace("\'", "\""))['loc']
+                    title = ''
+                    show_url = ''
+                    real_url = baidu_url
+                    datas = {
+                        'title': title,
+                        'baidu_url': baidu_url,
+                        'show_url': show_url,
+                        'real_url': real_url,
+                    }
+                    item_list.append(datas)
+                except:
+                    pass
+        except:
+            return []
+        else:
+            return item_list
+
+    # -  视频
+    def container_mb_video(self, container):
+        try:
+            item_list = list()
+            news_list = container.xpath('.//div[contains(@class,"c-video-container")]/a')
+            for video_list in news_list:
+                title = video_list.xpath('string(.//div[contains(@class,"c-vid-title")])')
+                baidu_url = video_list.xpath('./@href')[0]
+                show_url = ""
+                datalog = video_list.get("data-log", "")
+                real_url = baidu_url
+                try:
+                    datalog = str(datalog).replace("\'", "\"")
+                    sx_data = json.loads(datalog)
+                    real_url = sx_data["mu"]
+                except:
+                    pass
+
+                datas = {
+                    'title': title,
+                    'baidu_url': baidu_url,
+                    'show_url': show_url,
+                    'real_url': real_url,
+                }
+                item_list.append(datas)
+        except:
+            return []
+        else:
+            return item_list
+
+    # 小视频
+    def container_mb_small_video(self, container):
+        try:
+            item_list = list()
+            # news_list = container.xpath('//div[@tpl="vid_pocket"]//div[@class="vid-scroll-content"]')
+            news_list = container.xpath('//div[@tpl="vid_pocket"]//div[@class="c-scroll-item"]')
+            for video_list in news_list:
+                try:
+                    see_more = video_list.xpath('.//div[@class="_v1-pF"]')
+                    if not see_more:
+                        title = ''.join(video_list.xpath('string(.//div[@class="vid-pocket-item"]/div[2]/div)'))
+                        baidu_url = ''
+                        show_url = ''.join(video_list.xpath('.//div[@class="vid-pocket-item"]/div[1]/div//span[contains(@class,"vid-info-author-name")]/text()')[0])
+                        real_url = ''.join(video_list.xpath('.//a[@class="c-blocka"]/@href'))
+                        datas = {
+                            'title': title,
+                            'baidu_url': baidu_url,
+                            'show_url': show_url,
+                            'real_url': real_url,
+                        }
+                        item_list.append(datas)
+                except:
+                    continue
+        except:
+            return []
+        else:
+            return item_list
+
+    def container_mb_notes(self, container):
+        try:
+            item_list = list()
+            news_list = container.xpath("//div[@class='text-list-inner']/div[contains(@data-module,'lgtlt')]")
+            for video_list in news_list:
+                title = video_list.xpath('./div/@titlehtml')
+                show_desc = video_list.xpath('./div/@deschtml')
+                baidu_url = video_list.xpath('./div/@rl-link-href')
+                real_url = video_list.xpath('./div/@rl-link-data-click')
+                show_url = ''
+                if real_url:
+                    data = json.loads(real_url[0])
+                    show_url = data.get('src', '')
+                datas = {
+                    'title': title,
+                    'show_desc': show_desc,
+                    'baidu_url': baidu_url,
+                    'show_url': show_url,
+                }
+                item_list.append(datas)
+        except:
+            return []
+        else:
+            return item_list
+
+    # 直播
+    def container_mb_zhibo(self, container):
+        try:
+            item_list = list()
+            news_list = container.xpath('//div[@tpl="live_converge"]//div[@class="c-scroll-item"]')
+            for video_list in news_list:
+                title = video_list.xpath('string(.//span[contains(@class,"c-abstract")])')
+                baidu_url = ''.join(video_list.xpath('.//a/@href'))
+                show_url = ''
+                datas = {
+                    'title': title,
+                    'baidu_url': baidu_url,
+                    'show_url': show_url,
+                }
+                item_list.append(datas)
+        except:
+            return []
+        else:
+            return item_list
+
+    def get_container_list(self, html):
+        """获取搜索结果列表元素"""
+        try:
+            html_element = fromstring(html.encode('utf-8', 'ignore').decode('utf-8', 'ignore'))
+            container_list = html_element.xpath('//div[@id="results"]/div[contains(@class,"c-result")]')
+        except:
+            return -1
+        else:
+            return container_list
+
+    # def get_container_list(self, html):
+    #     """获取搜索结果列表元素"""
+    #     try:
+    #         html_element = etree.HTML(html, etree.HTMLParser(encoding="utf-8"))
+    #         container_list = html_element.xpath('//div[contains(@class,"c-result")]')
+    #     except:
+    #         return -1
+    #     else:
+    #         return container_list
+
+    def get_rank(self, container):
+        """获取排名"""
+        try:
+            rank = int(container.xpath('./@order')[0])
+        except:
+            return 0
+        else:
+            return rank
+
+    def get_real_url_by_json(self, container):
+        """通过json，获取真实url"""
+        try:
+            real_url = ""
+            datalog = container.get("data-log", "")
+            if datalog:
+                try:
+                    datalog = str(datalog).replace("\'", "\"")
+                    sx_data = json.loads(datalog)
+                    real_url = sx_data["mu"]
+                except:
+                    pass
+            if real_url == "" or real_url == "notes.baidu.com":
+                try:
+                    article_list = container.xpath('.//article/@rl-link-href')
+                    if len(article_list) > 0:
+                        url = article_list[0]
+                        headers = {
+                            "User-Agent": "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1"
+                        }
+                        response = requests.get(url=url, headers=headers)
+                        if "window.location.replace" in response.text:
+                            url_list = re.findall(r'.*url=(.*?)".*', response.text)
+                            if len(url_list) > 0:
+                                url = url_list[0]
+                                real_url = url
+                except:
+                    pass
+        except Exception as e:
+            return -1
+        else:
+            return real_url
+
+    def get_real_url_by_baidu_url(self, baidu_url, try_count=1):
+        """通过百度url获取真实url"""
+        try:
+            if try_count > 3:
+                return ''
+            else:
+                headers = {
+                    'User-Agent': random.choice(self.mobile_useragent_list),
+                    "Cookie": self.get_cook()
+                }
+                response = requests.get(baidu_url, headers=headers, timeout=20)
+                if response.status_code > 400:
+                    print('获取real_url失败 - {}'.format(response.status_code))
+                    return self.get_real_url_by_baidu_url(baidu_url, try_count + 1)
+                return response.url
+        except Exception:
+            return self.get_real_url_by_baidu_url(baidu_url, try_count + 1)
+
+    # 判断是否需要获取真实url - （需要获取真实url情况：完全匹配， show_url不是url格式）
+    def check_get_real_url(self, container, real_url):
+        # 取页面上的真实url
+        datalog = container.get("data-log", "")
+        if datalog:
+            try:
+                datalog = str(datalog).replace("\'", "\"")
+                sx_data = json.loads(datalog)
+                real_url = sx_data["mu"]
+            except:
+                return -1
+        return real_url
+
+    def get_baidu_url(self, container):
+        """获取百度url"""
+        xpath_rules = ['.//header[@class="c-gap-bottom-small"]//a[1]/@href',
+                       './/div[@class="circle-sample"]//a[1]/@href',
+                       './/article/@rl-link-href']
+        return self.get_res_text(container, xpath_rules)
+
+    def get_show_url(self, container):
+        """获取显示url"""
+        xpath_rules = [
+            './/div[contains(@class,"android-text-top1")]//text()',
+            './/span[contains(@class,"android-text-top1")]//text()',
+            './/span[contains(@class,"c-showurl")]//text()',
+            './/div[contains(@class,"c-showurl")]//text()',
+            './/span[@class="c-color-gray"]//text()',
+            './/div[@class="c-line-clamp1"]//text()',
+        ]
+        return remove_special_characters(self.get_res_text(container, xpath_rules))
+
+    def get_show_title_mb(self, container):
+        """获取标题"""
+        xpath_rules = ['.//span[@class="c-line-clamp1"]//text()',
+                       './/header//span[@class="c-title-text"]//text()',
+                       './/span[@class="c-title-text"]//text()',
+                       './/h3[@class="c-title title-con"]//text()',
+                       './/span[@class="_1mmq3"]//text()',
+                       './/div[@class="c-line-clamp1"][1]//text()',
+                       './/div[@class="ugc-title__2ofi_"]//text()',
+                       './/div[contains(@class,"c-title")]//text()',
+                       '//div[@class="c-span7"]/div[contains(@class,"c-font-large")]/text()',
+                       'string(//div[contains(@class,"ugc-title")])',
+                       ".//div[@class='text-list-inner']/div[@class='text-item tts-b-item']"
+
+                       ]
+        return self.get_res_text_mb(container, xpath_rules)
+
+    def get_res_text_mb(self, container, xpath_rules):
+        """获取纯文本"""
+        text = ""
+        for rule in xpath_rules:
+            text_list = container.xpath(rule)
+            for i in text_list:
+                text += i.strip().strip('”').strip('“')
+            if text != "":
+                return escape_string(text)
+        return escape_string(text)
+
+    def get_show_desc(self, container):
+        """获取描述"""
+        xpath_rules = ['.//div[@class="c-line-clamp3"]//text()',
+
+                       './/span[@class="c-font-big wenda-abstract-quote"]/text()',
+                       './/div[@class="c-line-clamp2"]//text()',
+                       './/section//span//text()',
+                       './/div[@class="c-font-medium c-color c-gap-bottom-small wenda-abstract-text wenda-abstract-singo-line c-color-link"]//text()',
+                       './/div[@class="c-abstract c-gap-bottom wa-bk-polysemy-abstract c-line-clamp5"]//text()']
+        return self.get_res_text(container, xpath_rules)
+
+    def get_show_date(self, container):
+        """获取显示日期"""
+        xpath_rules = ['.//span[@class="c-gap-right-small"]//text()',
+                       './/span[@class="c-color-gray c-gap-left normal-footer-no-shrink"]//text()',
+                       './/span[@class="c-footer-showurl c-gap-left"]//text()',
+                       ]
+        res = self.get_res_text(container, xpath_rules)
+        if "回答时间：" in res:
+            return res.split("回答时间：")[-1]
+        elif "发贴时间" in res:
+            return res.split("发贴时间:")[-1]
+        else:
+            return res.replace('发布时间: ', '')
+
+    def get_res_text(self, container, xpath_rules):
+        """获取纯文本"""
+        text = ""
+        for rule in xpath_rules:
+            text_list = container.xpath(rule)
+            for i in text_list:
+                text += i.strip().strip('”').strip('“')
+            if text != "":
+                break
+        return escape_string(text)
+
+    def get_mb_cookie(self):
+        cookies = None
+        try:
+            cookie_jar = cookiejar.CookieJar()
+            request = Request('https://m.baidu.com/tc?tcreq4log=1', headers={})
+            handlers = [HTTPCookieProcessor(cookie_jar)]
+            opener = build_opener(*handlers)
+            opener.open(request, timeout=10)
+            for cookie in cookie_jar:
+                if cookie.name == 'BDORZ':
+                    cookies = 'BDORZ=' + cookie.value
+                    break
+        except Exception:
+            pass
+        return cookies
+
+    def get_cook(self):
+        """
+        获取有效的cookie
+        :return:
+        """
+        try:
+            key_name = 'mb'
+            for i in range(2):
+                if UtilBaiduCookie().totalCookies(key_name) > 0:
+                    cookie = str(UtilBaiduCookie().getLastCookies(key_name=key_name)[0], encoding="utf-8")
+                    return cookie
+                else:
+                    return self.get_mb_cookie()
+        except:
+            return self.get_mb_cookie()
+
+
+class UtilBaiduPc(object):
+    def get_container_list(self, html):
+        """获取搜索结果列表元素"""
+        try:
+            # html_element = etree.HTML(html, etree.HTMLParser(encoding="utf-8"))
+            # container_list = html_element.xpath('//div[@id="content_left"]/div')
+            # return container_list
+            html_element = fromstring(html)
+            container_list = html_element.xpath('//div[@id="content_left"]/div[contains(@class,"new-pmd")]')
+            return container_list
+        except:
+            return -1
+
+    def get_rank(self, container):
+        """获取排名"""
+        try:
+            rank = int(container.get('id', 0))
+            return rank
+        except:
+            return 0
+
+    # 最新相关信息
+    def container_pc_news(self, container):
+        try:
+            item_list = list()
+            news_list = container.xpath('//div[@tpl="news-realtime"]/div/div')
+            for i in news_list:
+                try:
+                    a_list = i.xpath('./a')
+                    if a_list:
+                        title = ''.join(a_list[0].xpath('string(.)'))
+                        baidu_url = a_list[0].xpath('./@href')[0]
+                        try:
+                            show_url = i.xpath('./span[@class="c-color-gray c-gap-left-small"]/text()')[0]
+                        except:
+                            show_url = i.xpath('./div/span[@class="c-color-gray"]/text()')[0]
+                        datas = {
+                            'title': title,
+                            'baidu_url': baidu_url,
+                            'show_url': show_url
+                        }
+                        item_list.append(datas)
+                except:
+                    continue
+        except:
+            return []
+        else:
+            return item_list
+
+    # 高清在线观看
+    def container_pc_video(self, html):
+        try:
+            item_list = list()
+            video_list = json.loads(re.findall('"videoList":(\[.*?\])', html)[0])
+
+            for i in video_list:
+                title = i.get('title', '')
+                baidu_url = i.get('jumpUrl', '')
+                show_url = i.get('source', '')
+                datas = {
+                    'title': title,
+                    'baidu_url': baidu_url,
+                    'show_url': show_url
+                }
+                item_list.append(datas)
+        except:
+            return []
+        else:
+            return item_list
+
+        # 最新相关信息
+
+    def container_pc_tieba(self, container):
+        try:
+            item_list = list()
+            tieba_list = container.xpath('//div[@tpl="tieba_general"]/div[@class="result c-container"]/div[contains(@class,"c-row")]')
+            for i in tieba_list:
+                a_list = i.xpath('./div[contains(@class,"c-span8")]')
+                if a_list:
+                    title = ''.join(a_list[0].xpath('string(./a)'))
+                    baidu_url = a_list[0].xpath('./a/@href')[0]
+                    datas = {
+                        'title': title,
+                        'baidu_url': baidu_url,
+                    }
+                    item_list.append(datas)
+        except:
+            return []
+        else:
+            return item_list
+
+    def get_show_url(self, container):
+        """获取显示url"""
+        xpath_rules = [
+            './/span[@class="nor-src-wrap"]//text()',
+            './/div[contains(@class,"se_st_footer")]/a[1]//text()',
+            './/div[@class="f13"]/a[1]/text()',
+            './/span[@class="c-showurl"]//text()',
+            './/a[@class="c-showurl"]/span//text()',
+            './/div[@class="f13"]/span//text()',
+            './/a[@class="c-showurl"]//text()',
+            './/a[@class="c-showurl "]//text()',
+            './/div[contains(@class,"c-showurl")]//text()',
+            './/section/a/div//text()',
+            'string(//div[@class="vmp-zxenterprise-new_qayMC"]/div/h3/a/@href)',
+            'string(//h3[@class="c-title"]/span)'
+        ]
+        return remove_special_characters(self.get_res_text(container, xpath_rules))
+
+    def get_show_title(self, container):
+        """获取标题"""
+        # xpath_rules = ['.//h3//text()', './/span[@class="c-title-text"]//text()',
+        #                './/div[@class="wenda-abstract-showurl-title c-line-clamp1"]//text()',
+        #                './/h3[@class="t c-gap-bottom-small"]//text()',
+        #                '//h3[@role="text"]/span[@class="c-title-text"]//text()']
+        xpath_rules = ['.//span[@class="c-title-text"]//text()', './/div[@class="c-line-clamp1"]//text()',
+                       './/div[@class="c-font-medium c-color-t"]//text()',
+                       './/div[@class="wenda-abstract-showurl-title c-line-clamp1"]//text()',
+                       './/h3[@class="t c-gap-bottom-small"]//text()', './/h3[contains(@class,"t")]//text()',
+                       'string(//span[@class="c-title-text"])', 'string(//div[@class="vmp-zxenterprise-new_qayMC"]/div/h3/a)',
+                       'string(//div[@tpl="wenda_abstract_pc"]//div[contains(@class,"wenda-abstract-wrap-new")]//a)', 'string(//span[@class="c-title-text"])',
+                       'string(//div[@tpl="vmp_zxenterprise_new"]//h3/a)']
+        return self.get_res_text(container, xpath_rules)
+
+    def get_show_desc(self, container):
+        """获取描述"""
+        try:
+            des_list = container.cssselect("div.c-abstract")
+            if len(des_list) > 0:
+                des = self.get_text(des_list[0])
+            else:
+                des_list = container.cssselect("div.c-span18c-span-last")
+                if len(des_list) > 0:
+                    des = self.get_text(des_list[0])
+                else:
+                    des_list = container.cssselect("div.c-gap-top-small")
+                    if des_list:
+                        des = self.get_text(des_list[0])
+                    else:
+                        des = ''
+        except:
+            return ''
+        else:
+            return des
+
+    def get_text(self, elem):
+        rc = []
+        for node in elem.itertext():
+            rc.append(node.strip())
+        return ''.join(rc)
+
+    def get_baidu_url(self, container):
+        """获取百度url"""
+        xpath_rules = [
+            './/h3[contains(@class,"t")]/a/@href',
+            './/a[@class="c-showurl"]/@href',
+            './/span[@class="c-showurl"]/text()',
+            './/h3[@class="t c-gap-bottom-small"]/a/@href',
+            './/section/a/@href',
+            '//div[@tpl="ads_b2c_universal_card"]//a[@data-module="c-t"]/@href',
+            '//*[@id="1"]/div/article/section/div/div[1]/a/@href',
+            '//header[@class="c-gap-bottom-small"]/div/a[@class="c-blocka"]/@href',
+            '//div[@tpl="wenda_abstract_pc"]//div[contains(@class,"wenda-abstract-wrap-new")]//a/@href',
+            '//div[@tpl="ads_b2c_universal_card"]//header[@class="c-gap-bottom-small"]//a/@href',
+            '//div[@tpl="vmp_zxenterprise_new"]//h3/a/@href'
+        ]
+        return self.get_res_text(container, xpath_rules)
+
+    def get_show_date(self, container):
+        """获取显示日期"""
+        try:
+            des_list = container.cssselect("div.c-abstract")
+            if len(des_list) > 0:
+                show_date_eles = des_list[0].xpath('descendant::span')
+                if show_date_eles:
+                    show_date = show_date_eles[0].text.strip()
+                    show_date = str(show_date).split("-")[0].strip().replace(" ", "")
+                else:
+                    show_date = ''
+            else:
+                des_list = container.cssselect("div.c-span18c-span-last")
+                if len(des_list) > 0:
+                    show_date_eles = des_list[0].xpath('descendant::span[@class="m"]')
+                    if show_date_eles:
+                        show_date = show_date_eles[0].text.strip()
+                        show_date = str(show_date).split("-")[0].strip().replace(" ", "")
+                    else:
+                        show_date = ''
+                else:
+                    des_list = container.cssselect("div.c-gap-top-small")
+                    if des_list:
+                        show_date_eles = des_list[0].xpath('descendant::span')
+                        if show_date_eles:
+                            show_date = show_date_eles[0].text.strip()
+                            show_date = str(show_date).split("-")[0].strip().replace(" ", "")
+                        else:
+                            show_date = ''
+                    else:
+                        show_date = ''
+        except AttributeError:
+            return ''
+        else:
+            return show_date.replace('最佳答案:', '')
+
+    def get_snapshoot_url(self, container):
+        try:
+            """获取快照url"""
+            xpath_rules = [
+                './/div[contains(@class,"se_st_footer")]/a[contains(@class,"m")]/@href',
+                './/div[@class="g"]/a[@class="m"]',
+                './/a[@class="m"]/@href'
+            ]
+            return self.get_res_text(container, xpath_rules)
+        except:
+            return ''
+
+    def get_res_text(self, container, xpath_rules):
+        text = ""
+        for rule in xpath_rules:
+            text_list = container.xpath(rule)
+            for i in text_list:
+                text += i.strip()
+            if text != "":
+                break
+        return escape_string(text)
+
+    def get_real_url(self, baidu_url, try_count=1, timeout=5):
+        max_retry_num = 3
+        if try_count > max_retry_num:
+            return ''
+
+        headers = {
+            "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.110 Safari/537.36"
+        }
+        try:
+            response = requests.get(baidu_url, headers=headers, timeout=timeout, allow_redirects=False)
+            if response.status_code == 302:
+                return response.headers['Location']
+            elif response.status_code == 200:
+                res = requests.get(baidu_url, headers=headers, timeout=timeout, allow_redirects=True)
+                return res.url
+            else:
+                return self.get_real_url(baidu_url, try_count + 1)
+                # return ''
+        except Exception as err:
+            return self.get_real_url(baidu_url, try_count + 1)
+            # return ''
+
+    def get_cook(self):
+        """
+        获取有效的cookie
+        :return:
+        """
+        try:
+            key_name = 'pc'
+            for i in range(2):
+                if UtilBaiduCookie().totalCookies(key_name) > 0:
+                    cookie = str(UtilBaiduCookie().getLastCookies(key_name=key_name)[0], encoding="utf-8")
+                    return cookie
+                else:
+                    print('pc no use cookie')
+                    return 'BAIDUID={}:FG=1; BIDUPSID={};'.format(uuid.uuid1(), uuid.uuid4())
+        except:
+            return 'BAIDUID={}:FG=1; BIDUPSID={};'.format(uuid.uuid1(), uuid.uuid4())
+
+
+class UtilBaiduCookie(object):
+    def __init__(self):
+        self.redisPool = redis.ConnectionPool(**(config.DOWNLOADER_CENTER_REDIS[pro_config.ENVIR]))
+        self.redisClient = redis.StrictRedis(connection_pool=self.redisPool)
+        self.pc_cookie_key = 'baidu:pc:cookies'
+        self.mb_cookie_key = 'baidu:mb:cookies'
+
+    def getCookies(self, num=0, key_name='pc'):
+        '''
+        [获取一个有效的cookie 正序]
+        :param num:
+        :param key_name:
+        :return:
+        '''
+        # noinspection PyBroadException
+        try:
+            if key_name == 'pc':
+                return self.redisClient.zrange(self.pc_cookie_key, 0, num)
+            elif key_name == 'mb':
+                return self.redisClient.zrange(self.mb_cookie_key, 0, num)
+            else:
+                return []
+        except Exception:
+            return []
+
+    def getLastCookies(self, num=0, key_name='pc'):
+        '''
+         [获取最新的cooie]
+        :param num:
+        :param key_name:
+        :return:
+        '''
+        # noinspection PyBroadException
+        try:
+            if key_name == 'pc':
+                return self.redisClient.zrevrange(self.pc_cookie_key, 0, num)
+            elif key_name == 'mb':
+                return self.redisClient.zrevrange(self.mb_cookie_key, 0, num)
+            else:
+                return []
+        except Exception:
+            return []
+
+    def addCookies(self, cookie, key_name='pc'):
+        '''
+        [添加一个值]
+        :param cookie:
+        :param key_name:
+        :return:
+        '''
+        # noinspection PyBroadException
+        try:
+            score = int(round(time.time() * 1000))
+            if key_name == 'pc':
+                return self.redisClient.zadd(self.pc_cookie_key, {cookie: score})
+            elif key_name == 'mb':
+                return self.redisClient.zadd(self.mb_cookie_key, {cookie: score})
+            else:
+                return 0
+        except Exception:
+            return 0
+
+    def delCookies(self, cookie, key_name='pc'):
+        '''
+        删除cookie
+        :param cookie:
+        :return:
+        '''
+        # noinspection PyBroadException
+        try:
+            if key_name == 'pc':
+                return self.redisClient.zrem(self.pc_cookie_key, cookie)
+            elif key_name == 'mb':
+                return self.redisClient.zrem(self.mb_cookie_key, cookie)
+            else:
+                return 0
+        except Exception:
+            return 0
+
+    def totalCookies(self, key_name='pc'):
+        '''
+        [统计个数]
+        :return:
+        '''
+        # noinspection PyBroadException
+        try:
+            if key_name == 'pc':
+                return self.redisClient.zcard(self.pc_cookie_key)
+            elif key_name == 'mb':
+                return self.redisClient.zcard(self.mb_cookie_key)
+            else:
+                return 0
+        except Exception:
+            return 0
+
+
+def remove_special_characters(text):
+    text = text.replace("<b>", "")
+    text = text.replace("</b>", "")
+    text = text.replace("&nbsp", "")
+    text = text.replace("›", "/")
+    text = text.replace("...", "")
+    text = text.replace(" ", "")
+    return text
```

### Comparing `download-center-5.3.9/download_center/new_spider/util/util_ping.py` & `download-center-5.4.0/download_center/new_spider/util/util_ping.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-#!/usr/bin/python
-# -*- coding: utf8 -*-
-
-from platform import system as system_name  # Returns the system/OS name
-from os import system as system_call  # Execute a shell command
-import sys
-
-
-class Ping(object):
-
-    @staticmethod
-    def ping(ip):
-        try:
-            parameters = "-n 1" if system_name().lower() == "windows" else "-c 1"
-            # return system_call("ping " + parameters + " " + ip) == 0
-            return system_call("ping " + parameters + " " + ip + " > log.txt") == 0
-        except:
-            return False
+#!/usr/bin/python
+# -*- coding: utf8 -*-
+
+from platform import system as system_name  # Returns the system/OS name
+from os import system as system_call  # Execute a shell command
+import sys
+
+
+class Ping(object):
+
+    @staticmethod
+    def ping(ip):
+        try:
+            parameters = "-n 1" if system_name().lower() == "windows" else "-c 1"
+            # return system_call("ping " + parameters + " " + ip) == 0
+            return system_call("ping " + parameters + " " + ip + " > log.txt") == 0
+        except:
+            return False
```

### Comparing `download-center-5.3.9/download_center/new_spider/util/util_url.py` & `download-center-5.4.0/download_center/new_spider/util/util_url.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# -*- coding: utf8 -*-
-import sys
-
-
-class UtilUrl(object):
-    """
-    url处理工具类
-    """
-
-    @staticmethod
-    def get_url(from_url, cur_url):
-        """
-        拼接完整的url
-        Args:
-            from_url:源url
-            cur_url:要处理的url，可能是完整的url，也可能是以/、?等开始的不完整的url
-        """
-        if cur_url.startswith('http'):
-            return cur_url
-        elif cur_url.startswith('/'):
-            index = from_url.find('/', 8)
-            return from_url[0:index] + cur_url
-        elif cur_url.startswith('?'):
-            index = from_url.find('?')
-            return from_url[0:index] + cur_url
-        else:
-            index = from_url.rfind('/')
+# -*- coding: utf8 -*-
+import sys
+
+
+class UtilUrl(object):
+    """
+    url处理工具类
+    """
+
+    @staticmethod
+    def get_url(from_url, cur_url):
+        """
+        拼接完整的url
+        Args:
+            from_url:源url
+            cur_url:要处理的url，可能是完整的url，也可能是以/、?等开始的不完整的url
+        """
+        if cur_url.startswith('http'):
+            return cur_url
+        elif cur_url.startswith('/'):
+            index = from_url.find('/', 8)
+            return from_url[0:index] + cur_url
+        elif cur_url.startswith('?'):
+            index = from_url.find('?')
+            return from_url[0:index] + cur_url
+        else:
+            index = from_url.rfind('/')
             return from_url[0:index + 1] + cur_url
```

### Comparing `download-center-5.3.9/download_center/new_spider/util/util_useragent.py` & `download-center-5.4.0/download_center/new_spider/util/util_useragent.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# -*- coding: utf8 -*-
-import os
-import sys
-
-
-class UtilUseragent(object):
-    """
-    获取User-Agent
-    """
-    def __init__(self):
-        pass
-
-    @staticmethod
-    def get(type='PC'):
-        file_name = 'ua_pc_list.txt'
-        if type == 'MOBILE':
-            file_name = 'ua_mobile_list.txt'
-        elif type == 'SPIDER':
-            file_name = 'ua_spider_list.txt'
-        f = open(os.path.join(os.path.dirname(os.path.abspath(__file__)), file_name), 'r')
-        uas = [l.strip() for l in f.readlines()]
-        f.close()
-        return uas
-
-
-def test():
-    um = UtilUseragent()
-    ualist = um.get(type='MOBILE')
-    print(len(ualist))
-    print(ualist)
-
-if __name__ == "__main__":
+# -*- coding: utf8 -*-
+import os
+import sys
+
+
+class UtilUseragent(object):
+    """
+    获取User-Agent
+    """
+    def __init__(self):
+        pass
+
+    @staticmethod
+    def get(type='PC'):
+        file_name = 'ua_pc_list.txt'
+        if type == 'MOBILE':
+            file_name = 'ua_mobile_list.txt'
+        elif type == 'SPIDER':
+            file_name = 'ua_spider_list.txt'
+        f = open(os.path.join(os.path.dirname(os.path.abspath(__file__)), file_name), 'r')
+        uas = [l.strip() for l in f.readlines()]
+        f.close()
+        return uas
+
+
+def test():
+    um = UtilUseragent()
+    ualist = um.get(type='MOBILE')
+    print(len(ualist))
+    print(ualist)
+
+if __name__ == "__main__":
     test()
```

### Comparing `download-center-5.3.9/download_center/store/baidu_cookies.py` & `download-center-5.4.0/download_center/store/baidu_cookies.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-# -*- coding: utf8 -*-
-
-import redis
-import time
-from download_center.store import config
-
-
-class baiduCookie(object):
-    def __init__(self):
-        self.redisPool = redis.ConnectionPool(**(config.DOWNLOADER_CENTER_REDIS[config.ENVIR]))
-        self.redisClient = redis.StrictRedis(connection_pool=self.redisPool)
-        self.pc_cookie_key = 'baidu:pc:cookies'
-        self.mb_cookie_key = 'baidu:mb:cookies'
-
-    def getCookies(self, num=0, key_name='pc'):
-        '''
-        [获取一个有效的cookie 正序]
-        :param num:
-        :param key_name:
-        :return:
-        '''
-        # noinspection PyBroadException
-        try:
-            if key_name == 'pc':
-                return self.redisClient.zrange(self.pc_cookie_key, 0, num)
-            elif key_name == 'mb':
-                return self.redisClient.zrange(self.mb_cookie_key, 0, num)
-            else:
-                return []
-        except Exception:
-            return []
-
-    def getLastCookies(self, num=0, key_name='pc'):
-        '''
-         [获取最新的cooie]
-        :param num:
-        :param key_name:
-        :return:
-        '''
-        # noinspection PyBroadException
-        try:
-            if key_name == 'pc':
-                return self.redisClient.zrevrange(self.pc_cookie_key, 0, num)
-            elif key_name == 'mb':
-                return self.redisClient.zrevrange(self.mb_cookie_key, 0, num)
-            else:
-                return []
-        except Exception:
-            return []
-
-    def addCookies(self, cookie, key_name='pc'):
-        '''
-        [添加一个值]
-        :param cookie:
-        :param key_name:
-        :return:
-        '''
-        # noinspection PyBroadException
-        try:
-            score = int(round(time.time() * 1000))
-            if key_name == 'pc':
-                return self.redisClient.zadd(self.pc_cookie_key, {cookie: score})
-            elif key_name == 'mb':
-                return self.redisClient.zadd(self.mb_cookie_key, {cookie: score})
-            else:
-                return 0
-        except Exception:
-            return 0
-
-    def delCookies(self, cookie, key_name='pc'):
-        '''
-        删除cookie
-        :param cookie:
-        :return:
-        '''
-        # noinspection PyBroadException
-        try:
-            if key_name == 'pc':
-                return self.redisClient.zrem(self.pc_cookie_key, cookie)
-            elif key_name == 'mb':
-                return self.redisClient.zrem(self.mb_cookie_key, cookie)
-            else:
-                return 0
-        except Exception:
-            return 0
-
-    def totalCookies(self, key_name='pc'):
-        '''
-        [统计个数]
-        :return:
-        '''
-        # noinspection PyBroadException
-        try:
-            if key_name == 'pc':
-                return self.redisClient.zcard(self.pc_cookie_key)
-            elif key_name == 'mb':
-                return self.redisClient.zcard(self.mb_cookie_key)
-            else:
-                return 0
-        except Exception:
-            return 0
-
-
-if __name__ == '__main__':
-    bc = baiduCookie()
-    print(bc.getCookies(1, 'p'))
-    print(bc.totalCookies('mb'))
+# -*- coding: utf8 -*-
+
+import redis
+import time
+from download_center.store import config
+
+
+class baiduCookie(object):
+    def __init__(self):
+        self.redisPool = redis.ConnectionPool(**(config.DOWNLOADER_CENTER_REDIS[config.ENVIR]))
+        self.redisClient = redis.StrictRedis(connection_pool=self.redisPool)
+        self.pc_cookie_key = 'baidu:pc:cookies'
+        self.mb_cookie_key = 'baidu:mb:cookies'
+
+    def getCookies(self, num=0, key_name='pc'):
+        '''
+        [获取一个有效的cookie 正序]
+        :param num:
+        :param key_name:
+        :return:
+        '''
+        # noinspection PyBroadException
+        try:
+            if key_name == 'pc':
+                return self.redisClient.zrange(self.pc_cookie_key, 0, num)
+            elif key_name == 'mb':
+                return self.redisClient.zrange(self.mb_cookie_key, 0, num)
+            else:
+                return []
+        except Exception:
+            return []
+
+    def getLastCookies(self, num=0, key_name='pc'):
+        '''
+         [获取最新的cooie]
+        :param num:
+        :param key_name:
+        :return:
+        '''
+        # noinspection PyBroadException
+        try:
+            if key_name == 'pc':
+                return self.redisClient.zrevrange(self.pc_cookie_key, 0, num)
+            elif key_name == 'mb':
+                return self.redisClient.zrevrange(self.mb_cookie_key, 0, num)
+            else:
+                return []
+        except Exception:
+            return []
+
+    def addCookies(self, cookie, key_name='pc'):
+        '''
+        [添加一个值]
+        :param cookie:
+        :param key_name:
+        :return:
+        '''
+        # noinspection PyBroadException
+        try:
+            score = int(round(time.time() * 1000))
+            if key_name == 'pc':
+                return self.redisClient.zadd(self.pc_cookie_key, {cookie: score})
+            elif key_name == 'mb':
+                return self.redisClient.zadd(self.mb_cookie_key, {cookie: score})
+            else:
+                return 0
+        except Exception:
+            return 0
+
+    def delCookies(self, cookie, key_name='pc'):
+        '''
+        删除cookie
+        :param cookie:
+        :return:
+        '''
+        # noinspection PyBroadException
+        try:
+            if key_name == 'pc':
+                return self.redisClient.zrem(self.pc_cookie_key, cookie)
+            elif key_name == 'mb':
+                return self.redisClient.zrem(self.mb_cookie_key, cookie)
+            else:
+                return 0
+        except Exception:
+            return 0
+
+    def totalCookies(self, key_name='pc'):
+        '''
+        [统计个数]
+        :return:
+        '''
+        # noinspection PyBroadException
+        try:
+            if key_name == 'pc':
+                return self.redisClient.zcard(self.pc_cookie_key)
+            elif key_name == 'mb':
+                return self.redisClient.zcard(self.mb_cookie_key)
+            else:
+                return 0
+        except Exception:
+            return 0
+
+
+if __name__ == '__main__':
+    bc = baiduCookie()
+    print(bc.getCookies(1, 'p'))
+    print(bc.totalCookies('mb'))
```

### Comparing `download-center-5.3.9/download_center/store/py_store_mysql_pool.py` & `download-center-5.4.0/download_center/store/py_store_mysql_pool.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-# -*- coding: utf8 -*-
-import pymysql
-import time
-from DBUtils.PooledDB import PooledDB
-from DBUtils.PersistentDB import PersistentDB
-
-from pymysql.converters import escape_string
-
-import traceback
-from datetime import datetime
-
-
-class StoreMysqlPool(object):
-    """
-    mysql读写相关操作，pymysql，使用PooledDB连接池
-    Args:
-        host:数据库ip
-        user:数据库用户名
-        password:数据库用户密码
-        db:数据库名
-        port:数据库端口，默认3306
-        mincached:最少的空闲连接数， 默认为1
-        charset:数据库编码，默认utf8
-    """
-
-    def __init__(self, host="", user="", password="", db="", port=3306, mincached=1,
-                 pattern=1, charset="utf8"):
-        self.host = host
-
-        if pattern == 1:
-            self.pool = PooledDB(pymysql, mincached, host=host, user=user, passwd=password, db=db, port=port,
-                                 charset=charset)
-            self.close_able = True
-        elif pattern == 2:
-            self.pool = PersistentDB(pymysql, host=host, user=user, passwd=password, db=db, port=port,
-                                     charset=charset)
-
-            self.close_able = False
-        self._last_use_time = time.time()
-
-    def close(self, db):
-        if db is not None:
-            db.close()
-
-    def connect(self):
-        return self.pool.connection()
-
-    @staticmethod
-    def _cursor(db):
-        return db.cursor()
-
-    def query(self, sql):
-        """
-        根据sql查询
-        Returns：
-            数组的数组，外层数组元素为一行，内存数组元素为一行的一列
-        """
-        db = self.connect()
-        cur = self._cursor(db)
-        rows = []
-        try:
-            cur.execute(sql)
-            db.commit()
-            rows = cur.fetchall()
-        except pymysql.OperationalError:
-            print(traceback.format_exc())
-        except Exception:
-            print(traceback.format_exc())
-        finally:
-            cur.close()
-            self.close(db)
-        return rows
-
-    def count(self, tb):
-        """
-        返回某表的行数
-        Args:
-            tb:字符串，表名称
-        """
-        sql = 'select count(*) from %s' % tb
-        results = self.query(sql)
-        if len(results) == 1 and len(results[0]) == 1:
-            return int(results[0][0])
-
-    def do(self, sql, flag='lastrowid'):
-        """
-        执行sql，insert/delete/update操作
-        Args:
-            sql:要执行的sql
-            flag:返回值类型，flag=lastrowid返回lastrowid，flag=rowcount返回rowcount
-        """
-        db = self.connect()
-        cur = self._cursor(db)
-        r = None
-        try:
-            cur.execute(sql)
-            db.commit()
-            r = 1
-            if flag == 'lastrowid':
-                r = cur.lastrowid
-            elif flag == 'rowcount':
-                r = cur.rowcount
-        except pymysql.OperationalError:
-            print("time: %s; Error on %s: %s" % (str(datetime.now()), self.host, sql[0: 200]))
-            print(traceback.format_exc())
-            r = -1
-        except Exception:
-            print("time: %s; Error to MySQL on %s: %s" % (str(datetime.now()), self.host, sql[0: 200]))
-            print(traceback.format_exc())
-            r = -1
-        finally:
-            cur.close()
-            self.close(db)
-        return r
-
-    def save(self, table, data, mapping_fields=dict()):
-        """
-        将字典直接insert到数据库
-        Args:
-            table:字符串，插入目标表的名称
-            data:字典格式，key为字段名称，value为字段值，如{'id':'1','name':'temp'}
-            mapping_fields: 用于保持data字典的key与数据库字段的对应关系，
-                            如果结果字典的某个key不包含在mapping_fields中，则将直接使用key作为字段名
-        """
-
-        if len(data) <= 0:
-            return -1
-        try:
-            fields = ''
-            values = ''
-            for d in data:
-                if d in mapping_fields:
-                    fields += "`%s`," % (str(mapping_fields[d]))
-                else:
-                    fields += "`%s`," % (str(d))
-                values += "'%s'," % (escape_string(str(data[d])))
-            if len(fields) <= 0 or len(values) <= 0:
-                return -1
-            sql = "insert ignore into %s(%s) values(%s)" % (table, fields[:-1], values[:-1])
-            return self.do(sql)
-        except Exception:
-            print(traceback.format_exc())
-            return -1
-
-    def saveMany(self, sql, values, flag='lastrowid'):
-        """
-        执行sql，insert/delete/update操作
-        :param table: 'insert into table(id,name) values(%s,%s)'
-        :param names: 字符串
-        :param values:[{1,2},{1,2},...]  是一个列表，列表中的每一个元素必须是元组！！！
-        :param flag:
-        :return:
-        """
-        db = self.connect()
-        cur = self._cursor(db)
-        r = None
-        try:
-            cur.executemany(sql, values)
-            db.commit()
-            r = 1
-            if flag == 'lastrowid':
-                r = cur.lastrowid
-            elif flag == 'rowcount':
-                r = cur.rowcount
-
-        except pymysql.OperationalError:
-            print("Error connecting to MySQL on %s: %s" % (self.host, sql[0:255]))
-            print(traceback.format_exc())
-            r = -1
-        except Exception:
-            print("Error connecting to MySQL on %s: %s" % (self.host, sql[0:255]))
-            print(traceback.format_exc())
-            r = -1
-        finally:
-            cur.close()
-            self.close(db)
-        return r
-
-
-    def update(self, table, data, field, mapping_fields=dict()):
-        """
-        将字典直接update到数据库
-        Args:
-            table:字符串，更新目标表的名称
-            data:字典格式，key为字段名称，value为字段值，如{'id':'1','name':'temp'}
-            field:唯一索引字段，即根据该字段判断是否为同一条记录，作为where条件
-            mapping_fields: 用于保持data字典的key与数据库字段的对应关系，
-                            如果结果字典的某个key不包含在mapping_fields中，则将直接使用key作为字段名
-        """
-        if len(data) <= 0:
-            return -1
-        else:
-            try:
-                values = ''
-                field_value = None
-                for d in data:
-                    key = d
-                    if d in mapping_fields:
-                        key = mapping_fields[d]
-                    if key == field:
-                        field_value = data[d]
-                    values += "%s='%s'," % (str(key), escape_string(str(data[d])))
-                if len(values) <= 0 or field_value is None:
-                    return -1
-                sql = "update " + table + " set " + values[:-1] + " where " + field + "='" + escape_string(str(field_value)) + "'"
-                return self.do(sql, flag='rowcount')
-            except Exception:
-                print(traceback.format_exc())
-                return -1
-
-    def saveorupdate(self, table, data, field, mapping_fields=dict()):
-        """
-        将字典更新到数据库，如果已存在则update，不存在则insert
-        Args:
-            table:字符串，更新目标表的名称
-            data:字典格式，key为字段名称，value为字段值，如{'id':'1','name':'temp'}
-            field:唯一索引字段，即根据词字段判断是否为同一条记录，作为where条件
-            mapping_fields: 用于保持data字典的key与数据库字段的对应关系，
-                            如果结果字典的某个key不包含在mapping_fields中，则将直接使用key作为字段名
-        """
-        if len(data) <= 0:
-            return -1
-        try:
-            field_value = None
-            if field in data:
-                field_value = data[field]
-            else:
-                for key in mapping_fields:
-                    if mapping_fields[key] == field and key in data:
-                        field_value = data[key]
-            if field_value is None:
-                return -1
-            querysql = "select count(1) from " + table + " where " + field + "='" + escape_string(str(field_value)) + "'"
-            ed = self.query(querysql)
-            if ed and ed[0][0] > 0:
-                return self.update(table, data, field, mapping_fields)
-            else:
-                return self.save(table, data, mapping_fields)
-        except Exception:
-            print(traceback.format_exc())
-            return -1
-
-    def close_all(self):
-        """
-        关闭连接池全部连接
-        请在确保连接不再需要时确认
-        :return:
-        """
-        if self.close_able:
-            self.pool.close()
-
-
-def test():
-    db = {
-        'host': 'localhost',
-        'user': 'root',
-        'password': '',
-        'db': 'test'
-    }
-    mq = StoreMysqlPool(**db)
-    print(mq.count('urls'))
-
-
-if __name__ == "__main__":
-    test()
+# -*- coding: utf8 -*-
+import pymysql
+import time
+from DBUtils.PooledDB import PooledDB
+from DBUtils.PersistentDB import PersistentDB
+
+from pymysql.converters import escape_string
+
+import traceback
+from datetime import datetime
+
+
+class StoreMysqlPool(object):
+    """
+    mysql读写相关操作，pymysql，使用PooledDB连接池
+    Args:
+        host:数据库ip
+        user:数据库用户名
+        password:数据库用户密码
+        db:数据库名
+        port:数据库端口，默认3306
+        mincached:最少的空闲连接数， 默认为1
+        charset:数据库编码，默认utf8
+    """
+
+    def __init__(self, host="", user="", password="", db="", port=3306, mincached=1,
+                 pattern=1, charset="utf8"):
+        self.host = host
+
+        if pattern == 1:
+            self.pool = PooledDB(pymysql, mincached, host=host, user=user, passwd=password, db=db, port=port,
+                                 charset=charset)
+            self.close_able = True
+        elif pattern == 2:
+            self.pool = PersistentDB(pymysql, host=host, user=user, passwd=password, db=db, port=port,
+                                     charset=charset)
+
+            self.close_able = False
+        self._last_use_time = time.time()
+
+    def close(self, db):
+        if db is not None:
+            db.close()
+
+    def connect(self):
+        return self.pool.connection()
+
+    @staticmethod
+    def _cursor(db):
+        return db.cursor()
+
+    def query(self, sql):
+        """
+        根据sql查询
+        Returns：
+            数组的数组，外层数组元素为一行，内存数组元素为一行的一列
+        """
+        db = self.connect()
+        cur = self._cursor(db)
+        rows = []
+        try:
+            cur.execute(sql)
+            db.commit()
+            rows = cur.fetchall()
+        except pymysql.OperationalError:
+            print(traceback.format_exc())
+        except Exception:
+            print(traceback.format_exc())
+        finally:
+            cur.close()
+            self.close(db)
+        return rows
+
+    def count(self, tb):
+        """
+        返回某表的行数
+        Args:
+            tb:字符串，表名称
+        """
+        sql = 'select count(*) from %s' % tb
+        results = self.query(sql)
+        if len(results) == 1 and len(results[0]) == 1:
+            return int(results[0][0])
+
+    def do(self, sql, flag='lastrowid'):
+        """
+        执行sql，insert/delete/update操作
+        Args:
+            sql:要执行的sql
+            flag:返回值类型，flag=lastrowid返回lastrowid，flag=rowcount返回rowcount
+        """
+        db = self.connect()
+        cur = self._cursor(db)
+        r = None
+        try:
+            cur.execute(sql)
+            db.commit()
+            r = 1
+            if flag == 'lastrowid':
+                r = cur.lastrowid
+            elif flag == 'rowcount':
+                r = cur.rowcount
+        except pymysql.OperationalError:
+            print("time: %s; Error on %s: %s" % (str(datetime.now()), self.host, sql[0: 200]))
+            print(traceback.format_exc())
+            r = -1
+        except Exception:
+            print("time: %s; Error to MySQL on %s: %s" % (str(datetime.now()), self.host, sql[0: 200]))
+            print(traceback.format_exc())
+            r = -1
+        finally:
+            cur.close()
+            self.close(db)
+        return r
+
+    def save(self, table, data, mapping_fields=dict()):
+        """
+        将字典直接insert到数据库
+        Args:
+            table:字符串，插入目标表的名称
+            data:字典格式，key为字段名称，value为字段值，如{'id':'1','name':'temp'}
+            mapping_fields: 用于保持data字典的key与数据库字段的对应关系，
+                            如果结果字典的某个key不包含在mapping_fields中，则将直接使用key作为字段名
+        """
+
+        if len(data) <= 0:
+            return -1
+        try:
+            fields = ''
+            values = ''
+            for d in data:
+                if d in mapping_fields:
+                    fields += "`%s`," % (str(mapping_fields[d]))
+                else:
+                    fields += "`%s`," % (str(d))
+                values += "'%s'," % (escape_string(str(data[d])))
+            if len(fields) <= 0 or len(values) <= 0:
+                return -1
+            sql = "insert ignore into %s(%s) values(%s)" % (table, fields[:-1], values[:-1])
+            return self.do(sql)
+        except Exception:
+            print(traceback.format_exc())
+            return -1
+
+    def saveMany(self, sql, values, flag='lastrowid'):
+        """
+        执行sql，insert/delete/update操作
+        :param table: 'insert into table(id,name) values(%s,%s)'
+        :param names: 字符串
+        :param values:[{1,2},{1,2},...]  是一个列表，列表中的每一个元素必须是元组！！！
+        :param flag:
+        :return:
+        """
+        db = self.connect()
+        cur = self._cursor(db)
+        r = None
+        try:
+            cur.executemany(sql, values)
+            db.commit()
+            r = 1
+            if flag == 'lastrowid':
+                r = cur.lastrowid
+            elif flag == 'rowcount':
+                r = cur.rowcount
+
+        except pymysql.OperationalError:
+            print("Error connecting to MySQL on %s: %s" % (self.host, sql[0:255]))
+            print(traceback.format_exc())
+            r = -1
+        except Exception:
+            print("Error connecting to MySQL on %s: %s" % (self.host, sql[0:255]))
+            print(traceback.format_exc())
+            r = -1
+        finally:
+            cur.close()
+            self.close(db)
+        return r
+
+
+    def update(self, table, data, field, mapping_fields=dict()):
+        """
+        将字典直接update到数据库
+        Args:
+            table:字符串，更新目标表的名称
+            data:字典格式，key为字段名称，value为字段值，如{'id':'1','name':'temp'}
+            field:唯一索引字段，即根据该字段判断是否为同一条记录，作为where条件
+            mapping_fields: 用于保持data字典的key与数据库字段的对应关系，
+                            如果结果字典的某个key不包含在mapping_fields中，则将直接使用key作为字段名
+        """
+        if len(data) <= 0:
+            return -1
+        else:
+            try:
+                values = ''
+                field_value = None
+                for d in data:
+                    key = d
+                    if d in mapping_fields:
+                        key = mapping_fields[d]
+                    if key == field:
+                        field_value = data[d]
+                    values += "%s='%s'," % (str(key), escape_string(str(data[d])))
+                if len(values) <= 0 or field_value is None:
+                    return -1
+                sql = "update " + table + " set " + values[:-1] + " where " + field + "='" + escape_string(str(field_value)) + "'"
+                return self.do(sql, flag='rowcount')
+            except Exception:
+                print(traceback.format_exc())
+                return -1
+
+    def saveorupdate(self, table, data, field, mapping_fields=dict()):
+        """
+        将字典更新到数据库，如果已存在则update，不存在则insert
+        Args:
+            table:字符串，更新目标表的名称
+            data:字典格式，key为字段名称，value为字段值，如{'id':'1','name':'temp'}
+            field:唯一索引字段，即根据词字段判断是否为同一条记录，作为where条件
+            mapping_fields: 用于保持data字典的key与数据库字段的对应关系，
+                            如果结果字典的某个key不包含在mapping_fields中，则将直接使用key作为字段名
+        """
+        if len(data) <= 0:
+            return -1
+        try:
+            field_value = None
+            if field in data:
+                field_value = data[field]
+            else:
+                for key in mapping_fields:
+                    if mapping_fields[key] == field and key in data:
+                        field_value = data[key]
+            if field_value is None:
+                return -1
+            querysql = "select count(1) from " + table + " where " + field + "='" + escape_string(str(field_value)) + "'"
+            ed = self.query(querysql)
+            if ed and ed[0][0] > 0:
+                return self.update(table, data, field, mapping_fields)
+            else:
+                return self.save(table, data, mapping_fields)
+        except Exception:
+            print(traceback.format_exc())
+            return -1
+
+    def close_all(self):
+        """
+        关闭连接池全部连接
+        请在确保连接不再需要时确认
+        :return:
+        """
+        if self.close_able:
+            self.pool.close()
+
+
+def test():
+    db = {
+        'host': 'localhost',
+        'user': 'root',
+        'password': '',
+        'db': 'test'
+    }
+    mq = StoreMysqlPool(**db)
+    print(mq.count('urls'))
+
+
+if __name__ == "__main__":
+    test()
```

### Comparing `download-center-5.3.9/download_center/store/store_es_v2.py` & `download-center-5.4.0/download_center/store/store_es_v2.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-# -*- coding: utf8 -*-
-
-from elasticsearch import Elasticsearch
-import elasticsearch.helpers
-from datetime import time
-
-
-class StoreEs(object):
-    def __init__(self, host="localhost", port=9200, params=None, hosts=[]):
-        """
-        连接集群 或者单个节点
-        :param host:
-        :param port:
-        :param params:
-        :param hosts:
-        """
-        if hosts:
-            if params:
-                self.es = Elasticsearch(hosts, **params)
-            else:
-                self.es = Elasticsearch(hosts)
-        else:
-            if params:
-                self.es = Elasticsearch("{0}:{1}".format(host, port), **params)
-            else:
-                self.es = Elasticsearch("{0}:{1}".format(host, port))
-
-    def save(self, index, doc_type, body, id=None, params=None):
-        field = dict()
-        field['index'] = index
-        field['doc_type'] = doc_type
-        field['body'] = body
-        if id:
-            field['id'] = id
-        if params:
-            field['params'] = params
-        self.es.index(**field)
-
-    def batch_save(self, index, doc_type, body):
-        for i, val in enumerate(body):
-            while True:
-                try:
-                    self.save(index, doc_type, val)
-                    break
-                    pass
-                except:
-                    time.sleep(1)
-                    continue
-
-    def bulk_by_ids(self, index, doc_type, body, parallel=False):
-        """
-        批量操作指定id
-        :param index:
-        :param doc_type:
-        :param body:
-        :return:
-        """
-        actions = [
-            {
-                '_op_type': 'index',
-                '_index': index,
-                '_type': doc_type,
-                '_id': d.pop("id"),
-                '_source': d
-            }
-            for d in body
-            ]
-        if parallel:
-            for success, info in elasticsearch.helpers.parallel_bulk(client=self.es, actions=actions, thread_count=10,
-                                                                     chunk_size=1000):
-                if not success:
-                    print('Doc failed', info)
-        else:
-            elasticsearch.helpers.bulk(client=self.es, actions=actions,
-                                       stats_only=True)  # 如果为True，则仅报告成功/失败操作的数量，而不仅仅是成功的次数和错误响应列表
-
-    def bulk(self, index, doc_type, body):
-        actions = [
-            {
-                '_op_type': 'index',  # 该bulk()API接受index，create， delete，和update行动。使用该_op_type字段指定操作（_op_type默认为index）：
-                '_index': index,
-                '_type': doc_type,
-                '_source': d
-            }
-            for d in body
-            ]
-        elasticsearch.helpers.bulk(client=self.es, actions=actions)
-
-    def search(self, index, doc_type, body=None, params=None):
-        if params is None:
-            res = self.es.search(index=index, doc_type=doc_type, body=body)
-        else:
-            res = self.es.search(index=index, doc_type=doc_type, body=body, params=params)
-        return res
-
-    def get(self, index, doc_type, id):
-        return self.es.get(index=index, doc_type=doc_type, id=id)
-
-    def update_by_query(self, index, doc_type=None, body=None, params=None):
-        return self.es.update_by_query(index=index, doc_type=doc_type, body=body, params=params)
-
-    def delete(self, index, doc_type, id):
-        self.es.delete(index=index, doc_type=doc_type, id=id)
-
-
-if __name__ == '__main__':
-    # import uuid
-    # from Queue import Queue
-    # from threading import Thread
-    from download_center.store.store_es_v2 import StoreEs
-
-    config = {
-        'host': '115.159.158.157',
-        'port': 9200,
-        'params': {
-            'http_auth': ('admin', 'Iknowthat221@')
-        }
-    }
-    try:
-        es = StoreEs(**config)
-        result = es.get("content_center", "tiezi", "AWBaEjLkLUY1KU5jKSwu")
-        print("")
-    except:
-        pass
+# -*- coding: utf8 -*-
+
+from elasticsearch import Elasticsearch
+import elasticsearch.helpers
+from datetime import time
+
+
+class StoreEs(object):
+    def __init__(self, host="localhost", port=9200, params=None, hosts=[]):
+        """
+        连接集群 或者单个节点
+        :param host:
+        :param port:
+        :param params:
+        :param hosts:
+        """
+        if hosts:
+            if params:
+                self.es = Elasticsearch(hosts, **params)
+            else:
+                self.es = Elasticsearch(hosts)
+        else:
+            if params:
+                self.es = Elasticsearch("{0}:{1}".format(host, port), **params)
+            else:
+                self.es = Elasticsearch("{0}:{1}".format(host, port))
+
+    def save(self, index, doc_type, body, id=None, params=None):
+        field = dict()
+        field['index'] = index
+        field['doc_type'] = doc_type
+        field['body'] = body
+        if id:
+            field['id'] = id
+        if params:
+            field['params'] = params
+        self.es.index(**field)
+
+    def batch_save(self, index, doc_type, body):
+        for i, val in enumerate(body):
+            while True:
+                try:
+                    self.save(index, doc_type, val)
+                    break
+                    pass
+                except:
+                    time.sleep(1)
+                    continue
+
+    def bulk_by_ids(self, index, doc_type, body, parallel=False):
+        """
+        批量操作指定id
+        :param index:
+        :param doc_type:
+        :param body:
+        :return:
+        """
+        actions = [
+            {
+                '_op_type': 'index',
+                '_index': index,
+                '_type': doc_type,
+                '_id': d.pop("id"),
+                '_source': d
+            }
+            for d in body
+            ]
+        if parallel:
+            for success, info in elasticsearch.helpers.parallel_bulk(client=self.es, actions=actions, thread_count=10,
+                                                                     chunk_size=1000):
+                if not success:
+                    print('Doc failed', info)
+        else:
+            elasticsearch.helpers.bulk(client=self.es, actions=actions,
+                                       stats_only=True)  # 如果为True，则仅报告成功/失败操作的数量，而不仅仅是成功的次数和错误响应列表
+
+    def bulk(self, index, doc_type, body):
+        actions = [
+            {
+                '_op_type': 'index',  # 该bulk()API接受index，create， delete，和update行动。使用该_op_type字段指定操作（_op_type默认为index）：
+                '_index': index,
+                '_type': doc_type,
+                '_source': d
+            }
+            for d in body
+            ]
+        elasticsearch.helpers.bulk(client=self.es, actions=actions)
+
+    def search(self, index, doc_type, body=None, params=None):
+        if params is None:
+            res = self.es.search(index=index, doc_type=doc_type, body=body)
+        else:
+            res = self.es.search(index=index, doc_type=doc_type, body=body, params=params)
+        return res
+
+    def get(self, index, doc_type, id):
+        return self.es.get(index=index, doc_type=doc_type, id=id)
+
+    def update_by_query(self, index, doc_type=None, body=None, params=None):
+        return self.es.update_by_query(index=index, doc_type=doc_type, body=body, params=params)
+
+    def delete(self, index, doc_type, id):
+        self.es.delete(index=index, doc_type=doc_type, id=id)
+
+
+if __name__ == '__main__':
+    # import uuid
+    # from Queue import Queue
+    # from threading import Thread
+    from download_center.store.store_es_v2 import StoreEs
+
+    config = {
+        'host': '115.159.158.157',
+        'port': 9200,
+        'params': {
+            'http_auth': ('admin', 'Iknowthat221@')
+        }
+    }
+    try:
+        es = StoreEs(**config)
+        result = es.get("content_center", "tiezi", "AWBaEjLkLUY1KU5jKSwu")
+        print("")
+    except:
+        pass
```

### Comparing `download-center-5.3.9/download_center/store/store_mongo.py` & `download-center-5.4.0/download_center/store/store_mongo.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# -*- coding: utf8 -*-
-
-import time
-import sys
-
-
-from pymongo import *
-
-class StoreMongo(object):
-
-    """
-    mongoDB数据库链接
-    mongodb://{username}:{password}@{host}:{port}/{db_name}?authMechanism=MONGODB-CR
-    Args:
-        host:数据库ip
-        user:数据库用户名
-        password:数据库用户密码
-        db:数据库名
-        port:数据库端口，默认3306
-        authset:数据库认证模式，mongodb2.+默认为MONGODB-CR；3.0+默认为SCRAM-SHA-1
-    """
-    def __init__(self, host, port, user, password, db, authset='MONGODB-CR'):
-        uri = 'mongodb://%s:%s@%s:%d/%s?authMechanism=%s' % (user, password, host, port, db, authset)
-        client = MongoClient(uri)
-        self.db = client[db]
+# -*- coding: utf8 -*-
+
+import time
+import sys
+
+
+from pymongo import *
+
+class StoreMongo(object):
+
+    """
+    mongoDB数据库链接
+    mongodb://{username}:{password}@{host}:{port}/{db_name}?authMechanism=MONGODB-CR
+    Args:
+        host:数据库ip
+        user:数据库用户名
+        password:数据库用户密码
+        db:数据库名
+        port:数据库端口，默认3306
+        authset:数据库认证模式，mongodb2.+默认为MONGODB-CR；3.0+默认为SCRAM-SHA-1
+    """
+    def __init__(self, host, port, user, password, db, authset='MONGODB-CR'):
+        uri = 'mongodb://%s:%s@%s:%d/%s?authMechanism=%s' % (user, password, host, port, db, authset)
+        client = MongoClient(uri)
+        self.db = client[db]
```

### Comparing `download-center-5.3.9/download_center/store/store_oss.py` & `download-center-5.4.0/download_center/store/store_oss.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-# -*- coding: utf8 -*-
-import sys
-import oss2
-
-
-class StoreOSS(object):
-    """
-    阿里云OSS操作
-    Args:
-        key_id：用户访问密钥AccessKeyId，用于签名
-        key_secret：用户访问密钥AccessKeySecret，用于签名
-        endpoint：访问域名
-        bucket_name：存储空间（Bucket）名称
-        connect_timeout：连接超时时间
-    """
-    def __init__(self, key_id, key_secret, endpoint, bucket_name, connect_timeout=None):
-        self.bucket = oss2.Bucket(oss2.Auth(key_id, key_secret), endpoint, bucket_name, connect_timeout)
-
-    def put(self, key, data):
-        """
-        上传数据对象
-        Args:
-            key：上传到OSS的文件名
-            data：bytes，str或file-like object，待上传的内容
-        """
-        result = self.bucket.put_object(key, data)
-        return result
-
-    def get(self, key, filename=None):
-        """
-        下载数据对象
-        Args:
-            key：下载对象在OSS的文件名
-            filename：要保存的文件名，如果未传递则返回类文件对象
-        """
-        if filename is None:
-            return self.bucket.get_object(key)
-        else:
-            return self.bucket.get_object_to_file(key, filename)
-
-    def delete(self, key):
-        """
-        删除数据对象
-        Args:
-            key：对象在OSS的文件名
-        """
-        return self.bucket.delete_object(key)
-
-    def batch_delete(self, key_list):
-        """
-        批量删除数据对象
-        Args:
-            key_list：数据对象在OSS的文件名list
-        """
-        for i in range(0, len(key_list), 1000):
-            self.bucket.batch_delete_objects(key_list[i:i+1000])
-
-
-def test():
-    oss = StoreOSS("BWUNG5LjYOHpKyr1", "JWyFaaDz2ydzz1bvFRggIdjRknjXhx", 'http://oss-cn-shanghai.aliyuncs.com', "cluster2016")
-    oss.put('test.txt', 'just a test')
-    r = oss.get('test.txt')
-    print(r.read())
-    oss.delete('test.txt')
-
-
-if __name__ == "__main__":
-    test()
+# -*- coding: utf8 -*-
+import sys
+import oss2
+
+
+class StoreOSS(object):
+    """
+    阿里云OSS操作
+    Args:
+        key_id：用户访问密钥AccessKeyId，用于签名
+        key_secret：用户访问密钥AccessKeySecret，用于签名
+        endpoint：访问域名
+        bucket_name：存储空间（Bucket）名称
+        connect_timeout：连接超时时间
+    """
+    def __init__(self, key_id, key_secret, endpoint, bucket_name, connect_timeout=None):
+        self.bucket = oss2.Bucket(oss2.Auth(key_id, key_secret), endpoint, bucket_name, connect_timeout)
+
+    def put(self, key, data):
+        """
+        上传数据对象
+        Args:
+            key：上传到OSS的文件名
+            data：bytes，str或file-like object，待上传的内容
+        """
+        result = self.bucket.put_object(key, data)
+        return result
+
+    def get(self, key, filename=None):
+        """
+        下载数据对象
+        Args:
+            key：下载对象在OSS的文件名
+            filename：要保存的文件名，如果未传递则返回类文件对象
+        """
+        if filename is None:
+            return self.bucket.get_object(key)
+        else:
+            return self.bucket.get_object_to_file(key, filename)
+
+    def delete(self, key):
+        """
+        删除数据对象
+        Args:
+            key：对象在OSS的文件名
+        """
+        return self.bucket.delete_object(key)
+
+    def batch_delete(self, key_list):
+        """
+        批量删除数据对象
+        Args:
+            key_list：数据对象在OSS的文件名list
+        """
+        for i in range(0, len(key_list), 1000):
+            self.bucket.batch_delete_objects(key_list[i:i+1000])
+
+
+def test():
+    oss = StoreOSS("BWUNG5LjYOHpKyr1", "JWyFaaDz2ydzz1bvFRggIdjRknjXhx", 'http://oss-cn-shanghai.aliyuncs.com', "cluster2016")
+    oss.put('test.txt', 'just a test')
+    r = oss.get('test.txt')
+    print(r.read())
+    oss.delete('test.txt')
+
+
+if __name__ == "__main__":
+    test()
```

### Comparing `download-center-5.3.9/download_center.egg-info/SOURCES.txt` & `download-center-5.4.0/download_center.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 README.md
 setup.py
 download_center/__init__.py
 download_center/config.py
-download_center/requirements.txt
 download_center.egg-info/PKG-INFO
 download_center.egg-info/SOURCES.txt
 download_center.egg-info/dependency_links.txt
 download_center.egg-info/requires.txt
 download_center.egg-info/top_level.txt
 download_center/new_spider/__init__.py
 download_center/new_spider/downloader/__init__.py
 download_center/new_spider/downloader/config.py
 download_center/new_spider/downloader/html_local_downloader.py
 download_center/new_spider/spider/__init__.py
 download_center/new_spider/spider/basespider.py
 download_center/new_spider/spider/spider.py
 download_center/new_spider/util/__init__.py
-download_center/new_spider/util/ua_mobile_list.txt
-download_center/new_spider/util/ua_pc_list.txt
-download_center/new_spider/util/ua_spider_list.txt
 download_center/new_spider/util/util_baidu.py
 download_center/new_spider/util/util_baidu_relate.py
 download_center/new_spider/util/util_md5.py
 download_center/new_spider/util/util_ping.py
 download_center/new_spider/util/util_url.py
 download_center/new_spider/util/util_useragent.py
 download_center/store/__init__.py
```

### Comparing `download-center-5.3.9/setup.py` & `download-center-5.4.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Note: To use the 'upload' functionality of this file, you must:
-#   $ pipenv install twine --dev
-
-import io
-import os
-import sys
-from shutil import rmtree
-
-from setuptools import find_packages, setup, Command
-
-# Package meta-data.
-NAME = 'download-center'
-DESCRIPTION = 'spider framework for winndoo.'
-URL = 'http://git.winndoo.cn:82/python/download_center/downloader_client.git'
-EMAIL = 'baozhu.zhang@winndoo.com'
-AUTHOR = 'Welcome#1'
-REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '5.3.9'
-
-# What packages are required for this module to be executed?
-REQUIRED = [
-    'pymongo',
-    'oss2',
-    'redis',
-    'DBUtils',
-    'elasticsearch',
-    'flask',
-    'objgraph',
-    'lxml',
-    'cssselect',
-    'prettytable',
-    'pymysql',
-    'beautifulsoup4'
-]
-
-# What packages are optional?
-EXTRAS = {
-    # 'fancy feature': ['django'],
-}
-
-# The rest you shouldn't have to touch too much :)
-# ------------------------------------------------
-# Except, perhaps the License and Trove Classifiers!
-# If you do change the License, remember to change the Trove Classifier for that!
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# Load the package's __version__.py module as a dictionary.
-about = {}
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
-        exec(f.read(), about)
-else:
-    about['__version__'] = VERSION
-
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = 'Build and publish the package.'
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
-        except OSError:
-            pass
-
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
-
-        sys.exit()
-
-
-# Where the magic happens:
-setup(
-    name=NAME,
-    version=about['__version__'],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    # If your package is a single module, use this instead of 'packages':
-    # py_modules=['mypackage'],
-
-    # entry_points={
-    #     'console_scripts': ['mycli=mymodule:cli'],
-    # },
-    install_requires=REQUIRED,
-    extras_require=EXTRAS,
-    include_package_data=True,
-    package_data={
-        '': ['*.txt']
-      },
-    license='MIT',
-    classifiers=[
-        # Trove classifiers
-        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy'
-    ],
-    # $ setup.py publish support.
-    cmdclass={
-        'upload': UploadCommand,
-    },
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Note: To use the 'upload' functionality of this file, you must:
+#   $ pipenv install twine --dev
+
+import io
+import os
+import sys
+from shutil import rmtree
+
+from setuptools import find_packages, setup, Command
+
+# Package meta-data.
+NAME = 'download-center'
+DESCRIPTION = 'spider framework for winndoo.'
+URL = 'http://git.winndoo.cn:82/python/download_center/downloader_client.git'
+EMAIL = 'baozhu.zhang@winndoo.com'
+AUTHOR = 'Welcome#1'
+REQUIRES_PYTHON = '>=3.6.0'
+VERSION = '5.4.0'
+
+# What packages are required for this module to be executed?
+REQUIRED = [
+    'pymongo',
+    'oss2',
+    'redis',
+    'DBUtils',
+    'elasticsearch',
+    'flask',
+    'objgraph',
+    'lxml',
+    'cssselect',
+    'prettytable',
+    'pymysql',
+    'beautifulsoup4'
+]
+
+# What packages are optional?
+EXTRAS = {
+    # 'fancy feature': ['django'],
+}
+
+# The rest you shouldn't have to touch too much :)
+# ------------------------------------------------
+# Except, perhaps the License and Trove Classifiers!
+# If you do change the License, remember to change the Trove Classifier for that!
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
+try:
+    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+        long_description = '\n' + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+# Load the package's __version__.py module as a dictionary.
+about = {}
+if not VERSION:
+    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
+    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+        exec(f.read(), about)
+else:
+    about['__version__'] = VERSION
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = 'Build and publish the package.'
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print('\033[1m{0}\033[0m'.format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status('Removing previous builds…')
+            rmtree(os.path.join(here, 'dist'))
+        except OSError:
+            pass
+
+        self.status('Building Source and Wheel (universal) distribution…')
+        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+
+        self.status('Uploading the package to PyPI via Twine…')
+        os.system('twine upload dist/*')
+
+        self.status('Pushing git tags…')
+        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git push --tags')
+
+        sys.exit()
+
+
+# Where the magic happens:
+setup(
+    name=NAME,
+    version=about['__version__'],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    # If your package is a single module, use this instead of 'packages':
+    # py_modules=['mypackage'],
+
+    # entry_points={
+    #     'console_scripts': ['mycli=mymodule:cli'],
+    # },
+    install_requires=REQUIRED,
+    extras_require=EXTRAS,
+    include_package_data=True,
+    package_data={
+        '': ['*.txt']
+      },
+    license='MIT',
+    classifiers=[
+        # Trove classifiers
+        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy'
+    ],
+    # $ setup.py publish support.
+    cmdclass={
+        'upload': UploadCommand,
+    },
 )
```

