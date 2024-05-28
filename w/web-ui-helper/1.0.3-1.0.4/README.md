# Comparing `tmp/web-ui-helper-1.0.3.tar.gz` & `tmp/web-ui-helper-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-1.0.3.tar", last modified: Tue May 28 13:56:55 2024, max compression
+gzip compressed data, was "web-ui-helper-1.0.4.tar", last modified: Tue May 28 14:49:13 2024, max compression
```

## Comparing `web-ui-helper-1.0.3.tar` & `web-ui-helper-1.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.224681 web-ui-helper-1.0.3/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      747 2024-05-28 13:56:55.222686 web-ui-helper-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-28 13:56:55.224681 web-ui-helper-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1325 2024-05-28 13:56:17.000000 web-ui-helper-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.037612 web-ui-helper-1.0.3/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.3/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.112545 web-ui-helper-1.0.3/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.3/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-05-25 01:33:22.000000 web-ui-helper-1.0.3/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0     1704 2024-05-24 09:36:39.000000 web-ui-helper-1.0.3/web_ui_helper/common/http_proxy.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.118530 web-ui-helper-1.0.3/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.3/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.138476 web-ui-helper-1.0.3/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.141467 web-ui-helper-1.0.3/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    39222 2024-05-28 13:53:35.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.144460 web-ui-helper-1.0.3/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.164406 web-ui-helper-1.0.3/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.195480 web-ui-helper-1.0.3/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.221689 web-ui-helper-1.0.3/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      747 2024-05-28 13:56:54.000000 web-ui-helper-1.0.3/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2024-05-28 13:56:54.000000 web-ui-helper-1.0.3/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 13:56:54.000000 web-ui-helper-1.0.3/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2024-05-28 13:56:54.000000 web-ui-helper-1.0.3/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-28 13:56:54.000000 web-ui-helper-1.0.3/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.992606 web-ui-helper-1.0.4/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      747 2024-05-28 14:49:13.990621 web-ui-helper-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 14:49:13.992606 web-ui-helper-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2024-05-28 14:49:06.000000 web-ui-helper-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.948724 web-ui-helper-1.0.4/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.4/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.969668 web-ui-helper-1.0.4/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.4/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-05-25 01:33:22.000000 web-ui-helper-1.0.4/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0     1704 2024-05-24 09:36:39.000000 web-ui-helper-1.0.4/web_ui_helper/common/http_proxy.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.973657 web-ui-helper-1.0.4/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.4/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.975651 web-ui-helper-1.0.4/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.977646 web-ui-helper-1.0.4/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    39558 2024-05-28 14:48:51.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.980641 web-ui-helper-1.0.4/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.983630 web-ui-helper-1.0.4/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.4/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.987619 web-ui-helper-1.0.4/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.4/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:49:13.989615 web-ui-helper-1.0.4/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      747 2024-05-28 14:49:13.000000 web-ui-helper-1.0.4/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2024-05-28 14:49:13.000000 web-ui-helper-1.0.4/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 14:49:13.000000 web-ui-helper-1.0.4/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2024-05-28 14:49:13.000000 web-ui-helper-1.0.4/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-28 14:49:13.000000 web-ui-helper-1.0.4/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-1.0.3/LICENSE` & `web-ui-helper-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/PKG-INFO` & `web-ui-helper-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-1.0.3/setup.py` & `web-ui-helper-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='1.0.3',
+    version='1.0.4',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
```

### Comparing `web-ui-helper-1.0.3/web_ui_helper/common/date_extend.py` & `web-ui-helper-1.0.4/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/web_ui_helper/common/dir.py` & `web-ui-helper-1.0.4/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/web_ui_helper/common/http_proxy.py` & `web-ui-helper-1.0.4/web_ui_helper/common/http_proxy.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/web_ui_helper/common/log.py` & `web-ui-helper-1.0.4/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/web_ui_helper/common/metaclass.py` & `web-ui-helper-1.0.4/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/web_ui_helper/common/platforms.py` & `web-ui-helper-1.0.4/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/web_ui_helper/common/webdriver.py` & `web-ui-helper-1.0.4/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-1.0.4/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-1.0.4/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-1.0.4/web_ui_helper/selenium/frame/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -756,57 +756,62 @@
     def exception_html_save_to_txt(self):
         su = get_current_datetime_int_str()
         file_name = os.path.join(self.browser_proxy.LOG_PATH, "exception_{}.html".format(su))
         with open(file_name, "w", encoding="utf-8") as file:
             file.write(self.get_page_source())
 
     def get_network_requests(self, target_urls: list) -> dict:
-        # 获取所有性能日志
-        logs = self.browser.get_log('performance')
         network_requests = dict()
-        req_urls_local = deepcopy(target_urls)
-        rep_urls_local = deepcopy(target_urls)
-        for entry in logs:
-            log = json.loads(entry['message'])['message']
-            if rep_urls_local:
-                if log['method'] == 'Network.responseReceived':
-                    response = log['params']['response']
-                    url = response.get('url')
-                    if "?" in url:
-                        url = url.split("?")[0]
-                    if url in rep_urls_local:
-                        response_info = {
-                            'url': response['url'],
-                            'status': response['status'],
-                            'statusText': response['statusText'],
-                            'headers': response['headers'],
-                            'mimeType': response['mimeType']
-                        }
-                        info_local = network_requests.get("url") or dict()
-                        info_local["response_info"] = response_info
-                        network_requests[url] = info_local
-                        rep_urls_local.remove(url)
-            if req_urls_local:
-                if log['method'] == 'Network.requestWillBeSent':
-                    request = log['params']['request']
-                    url = request.get('url')
-                    if "?" in url:
-                        url = url.split("?")[0]
-                    if url in req_urls_local:
-                        request_info = {
-                            'url': request['url'],
-                            'status': request['status'],
-                            'statusText': request['statusText'],
-                            'headers': request['headers'],
-                            'mimeType': request['mimeType']
-                        }
-                        info_local = network_requests.get("url") or dict()
-                        info_local["request_info"] = request_info
-                        network_requests[url] = info_local
-                        req_urls_local.remove(url)
+        try:
+            # 获取所有性能日志
+            logs = self.browser.get_log('performance')
+            req_urls_local = deepcopy(target_urls)
+            rep_urls_local = deepcopy(target_urls)
+            for entry in logs:
+                log = json.loads(entry['message'])['message']
+                if rep_urls_local:
+                    if log['method'] == 'Network.responseReceived':
+                        response = log['params']['response']
+                        url = response.get('url')
+                        if "?" in url:
+                            url = url.split("?")[0]
+                        if url in rep_urls_local:
+                            response_info = {
+                                'url': response['url'],
+                                'status': response['status'],
+                                'statusText': response['statusText'],
+                                'headers': response['headers'],
+                                'mimeType': response['mimeType']
+                            }
+                            info_local = network_requests.get("url") or dict()
+                            info_local["response_info"] = response_info
+                            network_requests[url] = info_local
+                            rep_urls_local.remove(url)
+                if req_urls_local:
+                    if log['method'] == 'Network.requestWillBeSent':
+                        request = log['params']['request']
+                        url = request.get('url')
+                        if "?" in url:
+                            url = url.split("?")[0]
+                        if url in req_urls_local:
+                            request_info = {
+                                'url': request['url'],
+                                'status': request['status'],
+                                'statusText': request['statusText'],
+                                'headers': request['headers'],
+                                'mimeType': request['mimeType']
+                            }
+                            info_local = network_requests.get("url") or dict()
+                            info_local["request_info"] = request_info
+                            network_requests[url] = info_local
+                            req_urls_local.remove(url)
+        except Exception as e:
+            if "Stacktrace:" in str(e):
+                e = str(e).split("Stacktrace:")[0]
+            logger.error(e)
         return network_requests
 
 
 @element_find_exception
 def scroll_to_bottom(driver: webdriver) -> None:
     """模拟页面滚动到底部"""
     driver.execute_script("window.scrollTo(0, document.body.scrollHeight);")
```

### Comparing `web-ui-helper-1.0.3/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-1.0.4/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-1.0.4/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/web_ui_helper/terminal/device.py` & `web-ui-helper-1.0.4/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.3/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-1.0.4/web_ui_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-1.0.3/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-1.0.4/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

