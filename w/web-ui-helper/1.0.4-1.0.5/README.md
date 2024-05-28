# Comparing `tmp/web-ui-helper-1.0.4.tar.gz` & `tmp/web-ui-helper-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-1.0.4.tar", last modified: Tue May 28 14:49:13 2024, max compression
+gzip compressed data, was "web-ui-helper-1.0.5.tar", last modified: Tue May 28 16:01:12 2024, max compression
```

## Comparing `web-ui-helper-1.0.4.tar` & `web-ui-helper-1.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.992606 web-ui-helper-1.0.4/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      747 2024-05-28 14:49:13.990621 web-ui-helper-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-28 14:49:13.992606 web-ui-helper-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1325 2024-05-28 14:49:06.000000 web-ui-helper-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.948724 web-ui-helper-1.0.4/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.4/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.969668 web-ui-helper-1.0.4/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.4/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-05-25 01:33:22.000000 web-ui-helper-1.0.4/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0     1704 2024-05-24 09:36:39.000000 web-ui-helper-1.0.4/web_ui_helper/common/http_proxy.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.973657 web-ui-helper-1.0.4/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.4/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.975651 web-ui-helper-1.0.4/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.977646 web-ui-helper-1.0.4/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    39558 2024-05-28 14:48:51.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.980641 web-ui-helper-1.0.4/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.983630 web-ui-helper-1.0.4/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.987619 web-ui-helper-1.0.4/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.989615 web-ui-helper-1.0.4/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      747 2024-05-28 14:49:13.000000 web-ui-helper-1.0.4/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2024-05-28 14:49:13.000000 web-ui-helper-1.0.4/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 14:49:13.000000 web-ui-helper-1.0.4/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2024-05-28 14:49:13.000000 web-ui-helper-1.0.4/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-28 14:49:13.000000 web-ui-helper-1.0.4/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 16:01:12.742508 web-ui-helper-1.0.5/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      747 2024-05-28 16:01:12.740511 web-ui-helper-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 16:01:12.742508 web-ui-helper-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2024-05-28 16:00:51.000000 web-ui-helper-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:01:12.698626 web-ui-helper-1.0.5/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.5/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:01:12.718570 web-ui-helper-1.0.5/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.5/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.5/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-05-25 01:33:22.000000 web-ui-helper-1.0.5/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0     1704 2024-05-24 09:36:39.000000 web-ui-helper-1.0.5/web_ui_helper/common/http_proxy.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.5/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.5/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.5/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.5/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:01:12.723556 web-ui-helper-1.0.5/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.5/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.5/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.5/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:01:12.724554 web-ui-helper-1.0.5/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.5/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:01:12.727558 web-ui-helper-1.0.5/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.5/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    38442 2024-05-28 16:00:51.000000 web-ui-helper-1.0.5/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:01:12.731549 web-ui-helper-1.0.5/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.5/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.5/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:01:12.734528 web-ui-helper-1.0.5/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.5/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.5/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:01:12.738517 web-ui-helper-1.0.5/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.5/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.5/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:01:12.739515 web-ui-helper-1.0.5/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      747 2024-05-28 16:01:12.000000 web-ui-helper-1.0.5/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2024-05-28 16:01:12.000000 web-ui-helper-1.0.5/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 16:01:12.000000 web-ui-helper-1.0.5/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2024-05-28 16:01:12.000000 web-ui-helper-1.0.5/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-28 16:01:12.000000 web-ui-helper-1.0.5/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-1.0.4/LICENSE` & `web-ui-helper-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/PKG-INFO` & `web-ui-helper-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.4
+Version: 1.0.5
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-1.0.4/setup.py` & `web-ui-helper-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='1.0.4',
+    version='1.0.5',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
```

### Comparing `web-ui-helper-1.0.4/web_ui_helper/common/date_extend.py` & `web-ui-helper-1.0.5/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/web_ui_helper/common/dir.py` & `web-ui-helper-1.0.5/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/web_ui_helper/common/http_proxy.py` & `web-ui-helper-1.0.5/web_ui_helper/common/http_proxy.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/web_ui_helper/common/log.py` & `web-ui-helper-1.0.5/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/web_ui_helper/common/metaclass.py` & `web-ui-helper-1.0.5/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/web_ui_helper/common/platforms.py` & `web-ui-helper-1.0.5/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/web_ui_helper/common/webdriver.py` & `web-ui-helper-1.0.5/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-1.0.5/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-1.0.5/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-1.0.5/web_ui_helper/selenium/frame/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # Author:       mfkifhss2023
 # CreateDate:   2024/04/29
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 import os
 import time
-import json
 import string
 import base64
 import zipfile
 import ddddocr
 import requests
 import selenium
 from PIL import Image
@@ -755,59 +754,45 @@
 
     def exception_html_save_to_txt(self):
         su = get_current_datetime_int_str()
         file_name = os.path.join(self.browser_proxy.LOG_PATH, "exception_{}.html".format(su))
         with open(file_name, "w", encoding="utf-8") as file:
             file.write(self.get_page_source())
 
+    def get_browser_logs(self) -> dict:
+        try:
+            # 获取所有性能日志
+            return self.browser.get_log('browser')
+        except Exception as e:
+            if "Stacktrace:" in str(e):
+                e = str(e).split("Stacktrace:")[0]
+            logger.error(e)
+        return dict()
+
     def get_network_requests(self, target_urls: list) -> dict:
         network_requests = dict()
         try:
-            # 获取所有性能日志
-            logs = self.browser.get_log('performance')
-            req_urls_local = deepcopy(target_urls)
             rep_urls_local = deepcopy(target_urls)
-            for entry in logs:
-                log = json.loads(entry['message'])['message']
-                if rep_urls_local:
-                    if log['method'] == 'Network.responseReceived':
-                        response = log['params']['response']
-                        url = response.get('url')
-                        if "?" in url:
-                            url = url.split("?")[0]
-                        if url in rep_urls_local:
-                            response_info = {
-                                'url': response['url'],
-                                'status': response['status'],
-                                'statusText': response['statusText'],
-                                'headers': response['headers'],
-                                'mimeType': response['mimeType']
-                            }
-                            info_local = network_requests.get("url") or dict()
-                            info_local["response_info"] = response_info
-                            network_requests[url] = info_local
-                            rep_urls_local.remove(url)
-                if req_urls_local:
-                    if log['method'] == 'Network.requestWillBeSent':
-                        request = log['params']['request']
-                        url = request.get('url')
-                        if "?" in url:
-                            url = url.split("?")[0]
-                        if url in req_urls_local:
-                            request_info = {
-                                'url': request['url'],
-                                'status': request['status'],
-                                'statusText': request['statusText'],
-                                'headers': request['headers'],
-                                'mimeType': request['mimeType']
-                            }
-                            info_local = network_requests.get("url") or dict()
-                            info_local["request_info"] = request_info
-                            network_requests[url] = info_local
-                            req_urls_local.remove(url)
+            # 遍历所有请求，找到与目标 URL 部分匹配的请求和响应信息
+            for request in self.browser.requests:
+                if not rep_urls_local:
+                    break
+                url = request.url
+                if "?" in url:
+                    url = url.split("?")[0]
+                if url in rep_urls_local:
+                    if request.response:
+                        response = request.response
+                        response_info = {
+                            'status_code': response.status_code,
+                            'headers': response.headers,
+                            'body': response.body.decode('utf-8', errors='replace')  # 解码响应体
+                        }
+                        network_requests[url] = response_info
+                        rep_urls_local.remove(url)
         except Exception as e:
             if "Stacktrace:" in str(e):
                 e = str(e).split("Stacktrace:")[0]
             logger.error(e)
         return network_requests
```

### Comparing `web-ui-helper-1.0.4/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-1.0.5/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-1.0.5/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/web_ui_helper/terminal/device.py` & `web-ui-helper-1.0.5/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.4/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-1.0.5/web_ui_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.4
+Version: 1.0.5
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-1.0.4/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-1.0.5/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

