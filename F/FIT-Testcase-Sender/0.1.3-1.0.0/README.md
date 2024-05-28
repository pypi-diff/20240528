# Comparing `tmp/FIT_Testcase_Sender-0.1.3.tar.gz` & `tmp/FIT_Testcase_Sender-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FIT_Testcase_Sender-0.1.3.tar", last modified: Mon May 27 04:31:03 2024, max compression
+gzip compressed data, was "FIT_Testcase_Sender-1.0.0.tar", last modified: Tue May 28 05:25:18 2024, max compression
```

## Comparing `FIT_Testcase_Sender-0.1.3.tar` & `FIT_Testcase_Sender-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 04:31:03.147892 FIT_Testcase_Sender-0.1.3/
-drwxrwxrwx   0        0        0        0 2024-05-27 04:31:03.145669 FIT_Testcase_Sender-0.1.3/FIT_Testcase_Sender.egg-info/
--rw-rw-rw-   0        0        0      718 2024-05-27 04:31:03.000000 FIT_Testcase_Sender-0.1.3/FIT_Testcase_Sender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-27 04:31:03.000000 FIT_Testcase_Sender-0.1.3/FIT_Testcase_Sender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 04:31:03.000000 FIT_Testcase_Sender-0.1.3/FIT_Testcase_Sender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-27 04:31:03.000000 FIT_Testcase_Sender-0.1.3/FIT_Testcase_Sender.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      718 2024-05-27 04:31:03.146671 FIT_Testcase_Sender-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      328 2024-05-27 04:15:15.000000 FIT_Testcase_Sender-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 04:31:03.144670 FIT_Testcase_Sender-0.1.3/fit_testcase_sender/
--rw-rw-rw-   0        0        0       21 2024-05-27 04:27:56.000000 FIT_Testcase_Sender-0.1.3/fit_testcase_sender/__init__.py
--rw-rw-rw-   0        0        0      721 2024-05-27 04:30:18.000000 FIT_Testcase_Sender-0.1.3/fit_testcase_sender/remote.py
--rw-rw-rw-   0        0        0       42 2024-05-27 04:31:03.147892 FIT_Testcase_Sender-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      582 2024-05-27 04:27:52.000000 FIT_Testcase_Sender-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:25:18.556511 FIT_Testcase_Sender-1.0.0/
+drwxrwxrwx   0        0        0        0 2024-05-28 05:25:18.554516 FIT_Testcase_Sender-1.0.0/FIT_Testcase_Sender.egg-info/
+-rw-rw-rw-   0        0        0      780 2024-05-28 05:25:18.000000 FIT_Testcase_Sender-1.0.0/FIT_Testcase_Sender.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-28 05:25:18.000000 FIT_Testcase_Sender-1.0.0/FIT_Testcase_Sender.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 05:25:18.000000 FIT_Testcase_Sender-1.0.0/FIT_Testcase_Sender.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-28 05:25:18.000000 FIT_Testcase_Sender-1.0.0/FIT_Testcase_Sender.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      780 2024-05-28 05:25:18.555512 FIT_Testcase_Sender-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2024-05-28 05:25:14.000000 FIT_Testcase_Sender-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 05:25:18.552512 FIT_Testcase_Sender-1.0.0/fit_testcase_sender/
+-rw-rw-rw-   0        0        0       21 2024-05-28 05:23:05.000000 FIT_Testcase_Sender-1.0.0/fit_testcase_sender/__init__.py
+-rw-rw-rw-   0        0        0      851 2024-05-28 05:23:13.000000 FIT_Testcase_Sender-1.0.0/fit_testcase_sender/remote.py
+-rw-rw-rw-   0        0        0       42 2024-05-28 05:25:18.556511 FIT_Testcase_Sender-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      582 2024-05-28 05:21:21.000000 FIT_Testcase_Sender-1.0.0/setup.py
```

### Comparing `FIT_Testcase_Sender-0.1.3/FIT_Testcase_Sender.egg-info/PKG-INFO` & `FIT_Testcase_Sender-1.0.0/FIT_Testcase_Sender.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: FIT_Testcase_Sender
-Version: 0.1.3
+Version: 1.0.0
 Summary: A utility for sending scenarios via TCP/IP and checking their completion
 Author: suresofttech
 Author-email: sdhan@suresofttch.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ## FIT REMOTE FUNCTION
 
 ### function name: remote
 
 - excute_testcase: Send a resquest message to the FIT tool with a list of scenario numbers for fault injection as arguments. 
+parameter: list
+return: dict
 
-- is_testcase_result: Takes the fault injection result as an argument and determines whether the fault injection was successfully completed.
-
+- is_testcase_complete: Takes the fault injection result as an argument and determines whether the fault injection was successfully completed.
+parameter: dict
+return: bool
```

### Comparing `FIT_Testcase_Sender-0.1.3/PKG-INFO` & `FIT_Testcase_Sender-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: FIT_Testcase_Sender
-Version: 0.1.3
+Version: 1.0.0
 Summary: A utility for sending scenarios via TCP/IP and checking their completion
 Author: suresofttech
 Author-email: sdhan@suresofttch.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ## FIT REMOTE FUNCTION
 
 ### function name: remote
 
 - excute_testcase: Send a resquest message to the FIT tool with a list of scenario numbers for fault injection as arguments. 
+parameter: list
+return: dict
 
-- is_testcase_result: Takes the fault injection result as an argument and determines whether the fault injection was successfully completed.
-
+- is_testcase_complete: Takes the fault injection result as an argument and determines whether the fault injection was successfully completed.
+parameter: dict
+return: bool
```

### Comparing `FIT_Testcase_Sender-0.1.3/fit_testcase_sender/remote.py` & `FIT_Testcase_Sender-1.0.0/fit_testcase_sender/remote.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import json
 
 class FIT_Remote:
     def __init__(self, ip_address: str, port: int) -> None:
         self.ip_address = ip_address
         self.port = port
     
+    # 시나리오 넘버를 리스트로 받아 TC 실행합니다.
     def excute_testcase(self, scenario_number: list) -> dict:
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
             scenario_number = {"ScenarioNo": scenario_number}
             sock.connect((self.ip_address, self.port))
             sock.sendall(json.dumps(scenario_number).encode('utf-8') + b'\n')
             return json.loads(sock.recv(1024).decode('utf-8'))       
     
+    # TC 실행 결과가 Complete 인지 확인합니다.
     def is_testcase_complete(self, scenario_response: dict) -> bool:
         return scenario_response['Result'] == 'Complete'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `FIT_Testcase_Sender-0.1.3/setup.py` & `FIT_Testcase_Sender-1.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FIT_Testcase_Sender',
-    version='0.1.3',
+    version='1.0.0',
     packages=find_packages(),
     description='A utility for sending scenarios via TCP/IP and checking their completion',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='suresofttech',
     author_email='sdhan@suresofttch.com',
     license='MIT',
```

