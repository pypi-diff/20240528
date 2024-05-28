# Comparing `tmp/web-ui-helper-1.0.2.tar.gz` & `tmp/web-ui-helper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-1.0.2.tar", last modified: Sat May 25 01:40:19 2024, max compression
+gzip compressed data, was "web-ui-helper-1.0.3.tar", last modified: Tue May 28 13:56:55 2024, max compression
```

## Comparing `web-ui-helper-1.0.2.tar` & `web-ui-helper-1.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.464902 web-ui-helper-1.0.2/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      747 2024-05-25 01:40:19.462907 web-ui-helper-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-25 01:40:19.464902 web-ui-helper-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1325 2024-05-25 01:32:05.000000 web-ui-helper-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.421019 web-ui-helper-1.0.2/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.2/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.441963 web-ui-helper-1.0.2/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.2/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-05-25 01:33:22.000000 web-ui-helper-1.0.2/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0     1704 2024-05-24 09:36:39.000000 web-ui-helper-1.0.2/web_ui_helper/common/http_proxy.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.446950 web-ui-helper-1.0.2/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.2/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.448944 web-ui-helper-1.0.2/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.451936 web-ui-helper-1.0.2/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    36302 2024-05-25 01:39:29.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.454929 web-ui-helper-1.0.2/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.457920 web-ui-helper-1.0.2/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.2/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.459915 web-ui-helper-1.0.2/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.2/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-25 01:40:19.461909 web-ui-helper-1.0.2/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      747 2024-05-25 01:40:19.000000 web-ui-helper-1.0.2/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2024-05-25 01:40:19.000000 web-ui-helper-1.0.2/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 01:40:19.000000 web-ui-helper-1.0.2/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2024-05-25 01:40:19.000000 web-ui-helper-1.0.2/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-25 01:40:19.000000 web-ui-helper-1.0.2/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.224681 web-ui-helper-1.0.3/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      747 2024-05-28 13:56:55.222686 web-ui-helper-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 13:56:55.224681 web-ui-helper-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2024-05-28 13:56:17.000000 web-ui-helper-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.037612 web-ui-helper-1.0.3/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.3/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.112545 web-ui-helper-1.0.3/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.3/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-05-25 01:33:22.000000 web-ui-helper-1.0.3/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0     1704 2024-05-24 09:36:39.000000 web-ui-helper-1.0.3/web_ui_helper/common/http_proxy.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.118530 web-ui-helper-1.0.3/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.3/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.138476 web-ui-helper-1.0.3/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.141467 web-ui-helper-1.0.3/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    39222 2024-05-28 13:53:35.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.144460 web-ui-helper-1.0.3/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.164406 web-ui-helper-1.0.3/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.3/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.195480 web-ui-helper-1.0.3/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.3/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:56:55.221689 web-ui-helper-1.0.3/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      747 2024-05-28 13:56:54.000000 web-ui-helper-1.0.3/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2024-05-28 13:56:54.000000 web-ui-helper-1.0.3/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 13:56:54.000000 web-ui-helper-1.0.3/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2024-05-28 13:56:54.000000 web-ui-helper-1.0.3/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-28 13:56:54.000000 web-ui-helper-1.0.3/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-1.0.2/LICENSE` & `web-ui-helper-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/PKG-INFO` & `web-ui-helper-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.2
+Version: 1.0.3
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 Requires-Dist: selenium>=4.20.0
 Requires-Dist: pandas>=2.2.2
-Requires-Dist: blinker>=1.7.0
+Requires-Dist: blinker==1.7.0
 Requires-Dist: airtest>=1.3.3
 Requires-Dist: pocoui>=1.0.94
 Requires-Dist: requests>=2.31.0
 Requires-Dist: selenium-wire>=5.1.0
 Requires-Dist: webdriver-manager>=4.0.1
 Requires-Dist: ddddocr>=1.4.11
 Requires-Dist: openpyxl>=3.1.2
```

### Comparing `web-ui-helper-1.0.2/setup.py` & `web-ui-helper-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='1.0.2',
+    version='1.0.3',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
         'selenium>=4.20.0',
         'pandas>=2.2.2',
-        'blinker>=1.7.0',
+        'blinker==1.7.0',
         'airtest>=1.3.3',
         'pocoui>=1.0.94',
         'requests>=2.31.0',
         'selenium-wire>=5.1.0',
         'webdriver-manager>=4.0.1',
         'ddddocr>=1.4.11',
         'openpyxl>=3.1.2'
```

### Comparing `web-ui-helper-1.0.2/web_ui_helper/common/date_extend.py` & `web-ui-helper-1.0.3/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/web_ui_helper/common/dir.py` & `web-ui-helper-1.0.3/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/web_ui_helper/common/http_proxy.py` & `web-ui-helper-1.0.3/web_ui_helper/common/http_proxy.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/web_ui_helper/common/log.py` & `web-ui-helper-1.0.3/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/web_ui_helper/common/metaclass.py` & `web-ui-helper-1.0.3/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/web_ui_helper/common/platforms.py` & `web-ui-helper-1.0.3/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/web_ui_helper/common/webdriver.py` & `web-ui-helper-1.0.3/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-1.0.3/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-1.0.3/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-1.0.3/web_ui_helper/selenium/frame/browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 # Author:       mfkifhss2023
 # CreateDate:   2024/04/29
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 import os
 import time
+import json
 import string
 import base64
 import zipfile
 import ddddocr
 import requests
 import selenium
 from PIL import Image
 from io import BytesIO
+from copy import deepcopy
 from selenium import webdriver
 from abc import abstractmethod
 from selenium.webdriver import ActionChains
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.ui import Select
 from seleniumwire import webdriver as driver_wire
 from selenium.webdriver.chrome.options import Options
@@ -57,22 +59,24 @@
     BIN_PATH = os.path.join(get_project_path(), "bin")
     create_directory(BIN_PATH)
     USERDATA_PATH = None
     IMAGE_PATH = os.path.join(get_project_path(), "image")
     create_directory(IMAGE_PATH)
 
     def __init__(self, browser_path: str, is_headless: bool = True, proxy_address: str = '', proxy_username: str = '',
-                 proxy_password: str = '', proxy_scheme: str = "http", is_enable_proxy: bool = False) -> None:
+                 proxy_password: str = '', proxy_scheme: str = "http", is_enable_proxy: bool = False,
+                 enable_cdp: bool = False) -> None:
         self.browser_path = browser_path
         self.is_headless = is_headless
         self.proxy_address = proxy_address
         self.is_enable_proxy = is_enable_proxy
         self.proxy_scheme = proxy_scheme
         self.proxy_username = proxy_username
         self.proxy_password = proxy_password
+        self.enable_cdp = enable_cdp
 
     @abstractmethod
     def get_browser(self):
         pass
 
     @classmethod
     def get_options(cls):
@@ -87,17 +91,18 @@
         pass
 
 
 class ChromeBrowser(Browser):
     BROWSER_NAME = "Chrome"
 
     def __init__(self, browser_path: str, is_headless: bool = True, proxy_address: str = "", proxy_username: str = "",
-                 proxy_password: str = "", proxy_scheme: str = "http", is_enable_proxy: bool = False) -> None:
+                 proxy_password: str = "", proxy_scheme: str = "http", is_enable_proxy: bool = False,
+                 enable_cdp: bool = False) -> None:
         super().__init__(browser_path, is_headless, proxy_address, proxy_username, proxy_password, proxy_scheme,
-                         is_enable_proxy)
+                         is_enable_proxy, enable_cdp)
         self.driver_file = os.path.join(self.BIN_PATH, "chromedriver.exe")
         if is_file(self.driver_file) is False:
             logger.warning("开始下载与浏览器版本匹配的chromedriver.exe文件.")
             # 自动下载并安装适用于当前 Chrome 版本的 chromedriver
             driver_path = ChromeDriverManager().install()
             move_file(src_file=driver_path, dst_path=self.BIN_PATH)
             logger.warning("chromedriver.exe文件下载完成.")
@@ -135,14 +140,16 @@
             chrome_options.add_argument('--headless')
             # 指定浏览器分辨率
             # chrome_options.add_argument('--window-size=1920,1080')
             chrome_options.add_argument('--window-size=2560,1440')
         else:
             # 浏览器最大化
             chrome_options.add_argument('--start-maximized')
+        if self.enable_cdp is True:
+            chrome_options.add_argument('--auto-open-devtools-for-tabs')
         chrome_options.add_argument('--disable-dev-shm-usage')
         # 或者使用下面的设置, 提升速度
         # chrome_options.add_argument('blink-settings=imagesEnabled=false')
         # 隐藏滚动条, 应对一些特殊页面
         # chrome_options.add_argument('--hide-scrollbars')
         # chrome_options.add_argument('--remote-debugging-port=9222')
         chrome_options.add_argument('--log-level=3')
@@ -199,14 +206,17 @@
         logger.warning("浏览器版本: {}".format(browser.capabilities['browserVersion']))
         # 设置隐式等待时间为3秒
         # browser.implicitly_wait(3)
         # 反屏蔽
         browser.execute_cdp_cmd('Page.addScriptToEvaluateOnNewDocument', {
             'source': 'Object.defineProperty(navigator, "webdriver", {get: () => undefined})',
         })
+        if self.enable_cdp is True:
+            # 启用 DevTools 并启用网络日志
+            browser.execute_cdp_cmd('Network.enable', {})
         wait = WebDriverWait(driver=browser, timeout=self.TIMEOUT)
         return browser, wait, self.BROWSER_NAME
 
     def is_running(self) -> bool:
         process_name = get_browser_process_name(self.BROWSER_NAME)
         return is_process_running(process_name=process_name)
 
@@ -286,17 +296,18 @@
         return plugin_path
 
 
 class FirefoxBrowser(Browser):
     BROWSER_NAME = "Firefox"
 
     def __init__(self, browser_path: str, is_headless: bool = True, proxy_address: str = "", proxy_username: str = "",
-                 proxy_password: str = "", proxy_scheme: str = "http", is_enable_proxy: bool = False) -> None:
+                 proxy_password: str = "", proxy_scheme: str = "http", is_enable_proxy: bool = False,
+                 enable_cdp: bool = False) -> None:
         super().__init__(browser_path, is_headless, proxy_address, proxy_username, proxy_password, proxy_scheme,
-                         is_enable_proxy)
+                         is_enable_proxy, enable_cdp)
 
     def get_options(self) -> FirefoxOptions:
         firefox_profile = FirefoxOptions()
         # 在无头模式下运行 Firefox
         firefox_profile.headless = self.is_headless
         # 设置代理
         # options.add_argument('--proxy-server=http://proxy.example.com:8080')
@@ -335,40 +346,42 @@
     def is_running(self) -> bool:
         process_name = get_browser_process_name(self.BROWSER_NAME)
         return is_process_running(process_name=process_name)
 
 
 class SeleniumProxy(object):
 
-    def __init__(self, browser_name: str, proxy_address: str = "", proxy_username: str = "",
+    def __init__(self, browser_name: str, proxy_address: str = "", proxy_username: str = "", enable_cdp: bool = False,
                  proxy_scheme: str = "http", proxy_password: str = "", is_enable_proxy: bool = False,
                  browser_path: str = None, is_headless: bool = True, is_single_instance: bool = True) -> None:
         if browser_path:
             if not is_file(browser_path):
                 raise ValueError("browser path is not exist")
         else:
             browser_path = get_var_path(var=browser_name)
             if not browser_path:
                 raise ValueError("system not installed {} browser.".format(browser_name))
         exe_name = get_browser_bin_exe(browser_name=browser_name)
         exe_file = os.path.join(browser_path, exe_name)
         if browser_name == "Chrome":
             self.browser_proxy = ChromeBrowser(
                 browser_path=exe_file, is_headless=is_headless, proxy_address=proxy_address, proxy_scheme=proxy_scheme,
-                is_enable_proxy=is_enable_proxy, proxy_username=proxy_username, proxy_password=proxy_password
+                is_enable_proxy=is_enable_proxy, proxy_username=proxy_username, proxy_password=proxy_password,
+                enable_cdp=enable_cdp
             )
             # 单实例模式下，系统只能有一个chrome浏览器进程在运行中
             if is_single_instance is True:
                 if self.browser_proxy.is_running() is True:
                     raise ValueError("Chrome browser is already running.")
             self.browser, self.wait, self.browser_name = self.browser_proxy.get_browser()
         elif browser_name == "Firefox":
             self.browser_proxy = FirefoxBrowser(
                 browser_path=exe_file, is_headless=is_headless, proxy_address=proxy_address, proxy_scheme=proxy_scheme,
                 proxy_password=proxy_password, is_enable_proxy=is_enable_proxy, proxy_username=proxy_username,
+                enable_cdp=enable_cdp
             )
             # 单实例模式下，系统只能有一个firefox浏览器进程在运行中
             if is_single_instance is True:
                 if self.browser_proxy.is_running() is True:
                     raise ValueError("Firefox browser is already running.")
             self.browser, self.wait, self.browser_name = self.browser_proxy.get_browser()
         else:
@@ -742,14 +755,60 @@
 
     def exception_html_save_to_txt(self):
         su = get_current_datetime_int_str()
         file_name = os.path.join(self.browser_proxy.LOG_PATH, "exception_{}.html".format(su))
         with open(file_name, "w", encoding="utf-8") as file:
             file.write(self.get_page_source())
 
+    def get_network_requests(self, target_urls: list) -> dict:
+        # 获取所有性能日志
+        logs = self.browser.get_log('performance')
+        network_requests = dict()
+        req_urls_local = deepcopy(target_urls)
+        rep_urls_local = deepcopy(target_urls)
+        for entry in logs:
+            log = json.loads(entry['message'])['message']
+            if rep_urls_local:
+                if log['method'] == 'Network.responseReceived':
+                    response = log['params']['response']
+                    url = response.get('url')
+                    if "?" in url:
+                        url = url.split("?")[0]
+                    if url in rep_urls_local:
+                        response_info = {
+                            'url': response['url'],
+                            'status': response['status'],
+                            'statusText': response['statusText'],
+                            'headers': response['headers'],
+                            'mimeType': response['mimeType']
+                        }
+                        info_local = network_requests.get("url") or dict()
+                        info_local["response_info"] = response_info
+                        network_requests[url] = info_local
+                        rep_urls_local.remove(url)
+            if req_urls_local:
+                if log['method'] == 'Network.requestWillBeSent':
+                    request = log['params']['request']
+                    url = request.get('url')
+                    if "?" in url:
+                        url = url.split("?")[0]
+                    if url in req_urls_local:
+                        request_info = {
+                            'url': request['url'],
+                            'status': request['status'],
+                            'statusText': request['statusText'],
+                            'headers': request['headers'],
+                            'mimeType': request['mimeType']
+                        }
+                        info_local = network_requests.get("url") or dict()
+                        info_local["request_info"] = request_info
+                        network_requests[url] = info_local
+                        req_urls_local.remove(url)
+        return network_requests
+
 
 @element_find_exception
 def scroll_to_bottom(driver: webdriver) -> None:
     """模拟页面滚动到底部"""
     driver.execute_script("window.scrollTo(0, document.body.scrollHeight);")
```

### Comparing `web-ui-helper-1.0.2/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-1.0.3/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-1.0.3/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/web_ui_helper/terminal/device.py` & `web-ui-helper-1.0.3/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.2/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-1.0.3/web_ui_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.2
+Version: 1.0.3
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 Requires-Dist: selenium>=4.20.0
 Requires-Dist: pandas>=2.2.2
-Requires-Dist: blinker>=1.7.0
+Requires-Dist: blinker==1.7.0
 Requires-Dist: airtest>=1.3.3
 Requires-Dist: pocoui>=1.0.94
 Requires-Dist: requests>=2.31.0
 Requires-Dist: selenium-wire>=5.1.0
 Requires-Dist: webdriver-manager>=4.0.1
 Requires-Dist: ddddocr>=1.4.11
 Requires-Dist: openpyxl>=3.1.2
```

### Comparing `web-ui-helper-1.0.2/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-1.0.3/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

