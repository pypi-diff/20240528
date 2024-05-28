# Comparing `tmp/alibabacloud_paiabtest20240119-1.0.0.tar.gz` & `tmp/alibabacloud_paiabtest20240119-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_paiabtest20240119-1.0.0.tar", last modified: Sat May 11 02:30:11 2024, max compression
+gzip compressed data, was "dist/alibabacloud_paiabtest20240119-1.0.1.tar", last modified: Tue May 28 06:32:50 2024, max compression
```

## Comparing `alibabacloud_paiabtest20240119-1.0.0.tar` & `alibabacloud_paiabtest20240119-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:11.000000 alibabacloud_paiabtest20240119-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-11 02:30:10.000000 alibabacloud_paiabtest20240119-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-11 02:30:10.000000 alibabacloud_paiabtest20240119-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2443 2024-05-11 02:30:11.000000 alibabacloud_paiabtest20240119-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1119 2024-05-11 02:30:10.000000 alibabacloud_paiabtest20240119-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1204 2024-05-11 02:30:10.000000 alibabacloud_paiabtest20240119-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:11.000000 alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-11 02:30:10.000000 alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   220447 2024-05-11 02:30:10.000000 alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119/client.py
--rw-r--r--   0 root         (0) root         (0)   254958 2024-05-11 02:30:10.000000 alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 02:30:11.000000 alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2443 2024-05-11 02:30:11.000000 alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 02:30:11.000000 alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 02:30:11.000000 alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-11 02:30:11.000000 alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-11 02:30:11.000000 alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-11 02:30:11.000000 alibabacloud_paiabtest20240119-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2641 2024-05-11 02:30:10.000000 alibabacloud_paiabtest20240119-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       72 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   220447 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119/client.py
+-rw-r--r--   0 root         (0) root         (0)   255412 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2641 2024-05-28 06:32:50.000000 alibabacloud_paiabtest20240119-1.0.1/setup.py
```

### Comparing `alibabacloud_paiabtest20240119-1.0.0/LICENSE` & `alibabacloud_paiabtest20240119-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_paiabtest20240119-1.0.0/PKG-INFO` & `alibabacloud_paiabtest20240119-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_paiabtest20240119
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud PAIABTest (20240119) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_paiabtest20240119-1.0.0/README-CN.md` & `alibabacloud_paiabtest20240119-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_paiabtest20240119-1.0.0/README.md` & `alibabacloud_paiabtest20240119-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119/client.py` & `alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119/models.py` & `alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2388,14 +2388,15 @@
         return self
 
 
 class GetDomainResponseBody(TeaModel):
     def __init__(
         self,
         bucket_type: str = None,
+        buckets: str = None,
         condition: str = None,
         crowd_ids: str = None,
         debug_users: str = None,
         description: str = None,
         domain_id: str = None,
         flow: int = None,
         gmt_create_time: str = None,
@@ -2406,14 +2407,15 @@
         name: str = None,
         project_id: str = None,
         project_name: str = None,
         request_id: str = None,
         workspace_id: str = None,
     ):
         self.bucket_type = bucket_type
+        self.buckets = buckets
         self.condition = condition
         self.crowd_ids = crowd_ids
         self.debug_users = debug_users
         self.description = description
         self.domain_id = domain_id
         self.flow = flow
         self.gmt_create_time = gmt_create_time
@@ -2434,14 +2436,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.bucket_type is not None:
             result['BucketType'] = self.bucket_type
+        if self.buckets is not None:
+            result['Buckets'] = self.buckets
         if self.condition is not None:
             result['Condition'] = self.condition
         if self.crowd_ids is not None:
             result['CrowdIds'] = self.crowd_ids
         if self.debug_users is not None:
             result['DebugUsers'] = self.debug_users
         if self.description is not None:
@@ -2472,14 +2476,16 @@
             result['WorkspaceId'] = self.workspace_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BucketType') is not None:
             self.bucket_type = m.get('BucketType')
+        if m.get('Buckets') is not None:
+            self.buckets = m.get('Buckets')
         if m.get('Condition') is not None:
             self.condition = m.get('Condition')
         if m.get('CrowdIds') is not None:
             self.crowd_ids = m.get('CrowdIds')
         if m.get('DebugUsers') is not None:
             self.debug_users = m.get('DebugUsers')
         if m.get('Description') is not None:
@@ -4133,14 +4139,15 @@
         return self
 
 
 class ListDomainsResponseBodyDomains(TeaModel):
     def __init__(
         self,
         bucket_type: str = None,
+        buckets: str = None,
         condition: str = None,
         crowd_ids: str = None,
         debug_users: str = None,
         description: str = None,
         domain_id: str = None,
         flow: int = None,
         gmt_create_time: str = None,
@@ -4150,14 +4157,15 @@
         layer_name: str = None,
         name: str = None,
         project_id: str = None,
         project_name: str = None,
         workspace_id: str = None,
     ):
         self.bucket_type = bucket_type
+        self.buckets = buckets
         self.condition = condition
         self.crowd_ids = crowd_ids
         self.debug_users = debug_users
         self.description = description
         self.domain_id = domain_id
         self.flow = flow
         self.gmt_create_time = gmt_create_time
@@ -4177,14 +4185,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.bucket_type is not None:
             result['BucketType'] = self.bucket_type
+        if self.buckets is not None:
+            result['Buckets'] = self.buckets
         if self.condition is not None:
             result['Condition'] = self.condition
         if self.crowd_ids is not None:
             result['CrowdIds'] = self.crowd_ids
         if self.debug_users is not None:
             result['DebugUsers'] = self.debug_users
         if self.description is not None:
@@ -4213,14 +4223,16 @@
             result['WorkspaceId'] = self.workspace_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BucketType') is not None:
             self.bucket_type = m.get('BucketType')
+        if m.get('Buckets') is not None:
+            self.buckets = m.get('Buckets')
         if m.get('Condition') is not None:
             self.condition = m.get('Condition')
         if m.get('CrowdIds') is not None:
             self.crowd_ids = m.get('CrowdIds')
         if m.get('DebugUsers') is not None:
             self.debug_users = m.get('DebugUsers')
         if m.get('Description') is not None:
```

### Comparing `alibabacloud_paiabtest20240119-1.0.0/alibabacloud_paiabtest20240119.egg-info/PKG-INFO` & `alibabacloud_paiabtest20240119-1.0.1/alibabacloud_paiabtest20240119.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-paiabtest20240119
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud PAIABTest (20240119) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_paiabtest20240119-1.0.0/setup.py` & `alibabacloud_paiabtest20240119-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_paiabtest20240119.
 
-Created on 11/05/2024
+Created on 28/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_paiabtest20240119"
 NAME = "alibabacloud_paiabtest20240119" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud PAIABTest (20240119) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

