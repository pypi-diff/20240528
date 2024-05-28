# Comparing `tmp/alibabacloud_polardb20170801-5.1.1.tar.gz` & `tmp/alibabacloud_polardb20170801-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_polardb20170801-5.1.1.tar", last modified: Fri May 17 17:19:14 2024, max compression
+gzip compressed data, was "dist/alibabacloud_polardb20170801-5.1.2.tar", last modified: Tue May 28 17:12:58 2024, max compression
```

## Comparing `alibabacloud_polardb20170801-5.1.1.tar` & `alibabacloud_polardb20170801-5.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/
--rw-r--r--   0 root         (0) root         (0)     4060 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2442 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1111 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1196 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   858320 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801/client.py
--rw-r--r--   0 root         (0) root         (0)  1239934 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2442 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2644 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:12:58.000000 alibabacloud_polardb20170801-5.1.2/
+-rw-r--r--   0 root         (0) root         (0)     4464 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2442 2024-05-28 17:12:58.000000 alibabacloud_polardb20170801-5.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:12:58.000000 alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   858674 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801/client.py
+-rw-r--r--   0 root         (0) root         (0)  1242936 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:12:58.000000 alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2442 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-28 17:12:58.000000 alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-28 17:12:58.000000 alibabacloud_polardb20170801-5.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2644 2024-05-28 17:12:57.000000 alibabacloud_polardb20170801-5.1.2/setup.py
```

### Comparing `alibabacloud_polardb20170801-5.1.1/ChangeLog.md` & `alibabacloud_polardb20170801-5.1.2/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2024-05-17 Version: 5.1.1
+- Update API DescribeDBClusterServerlessConf: update response param.
+- Update API DescribeDBClusters: update response param.
+- Update API ModifyDBClusterServerlessConf: add param ServerlessRuleCpuEnlargeThreshold.
+- Update API ModifyDBClusterServerlessConf: add param ServerlessRuleCpuShrinkThreshold.
+- Update API ModifyDBClusterServerlessConf: add param ServerlessRuleMode.
+
+
 2024-04-24 Version: 5.1.0
 - Support API RestartDBLink.
 
 
 2024-04-18 Version: 5.0.8
 - Update API DescribeDBClusterAttribute: update response param.
 - Update API DescribeDBClusters: update response param.
```

### Comparing `alibabacloud_polardb20170801-5.1.1/LICENSE` & `alibabacloud_polardb20170801-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801-5.1.1/PKG-INFO` & `alibabacloud_polardb20170801-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_polardb20170801
-Version: 5.1.1
+Version: 5.1.2
 Summary: Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_polardb20170801-5.1.1/README-CN.md` & `alibabacloud_polardb20170801-5.1.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801-5.1.1/README.md` & `alibabacloud_polardb20170801-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801/client.py` & `alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -18560,14 +18560,16 @@
             query['PlannedStartTime'] = request.planned_start_time
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.target_dbrevision_version_code):
             query['TargetDBRevisionVersionCode'] = request.target_dbrevision_version_code
+        if not UtilClient.is_unset(request.target_proxy_revision_version_code):
+            query['TargetProxyRevisionVersionCode'] = request.target_proxy_revision_version_code
         if not UtilClient.is_unset(request.upgrade_label):
             query['UpgradeLabel'] = request.upgrade_label
         if not UtilClient.is_unset(request.upgrade_policy):
             query['UpgradePolicy'] = request.upgrade_policy
         if not UtilClient.is_unset(request.upgrade_type):
             query['UpgradeType'] = request.upgrade_type
         req = open_api_models.OpenApiRequest(
@@ -18620,14 +18622,16 @@
             query['PlannedStartTime'] = request.planned_start_time
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
             query['ResourceOwnerId'] = request.resource_owner_id
         if not UtilClient.is_unset(request.target_dbrevision_version_code):
             query['TargetDBRevisionVersionCode'] = request.target_dbrevision_version_code
+        if not UtilClient.is_unset(request.target_proxy_revision_version_code):
+            query['TargetProxyRevisionVersionCode'] = request.target_proxy_revision_version_code
         if not UtilClient.is_unset(request.upgrade_label):
             query['UpgradeLabel'] = request.upgrade_label
         if not UtilClient.is_unset(request.upgrade_policy):
             query['UpgradePolicy'] = request.upgrade_policy
         if not UtilClient.is_unset(request.upgrade_type):
             query['UpgradeType'] = request.upgrade_type
         req = open_api_models.OpenApiRequest(
```

### Comparing `alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801/models.py` & `alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12863,28 +12863,74 @@
         if m.get('RevisionVersionCode') is not None:
             self.revision_version_code = m.get('RevisionVersionCode')
         if m.get('RevisionVersionName') is not None:
             self.revision_version_name = m.get('RevisionVersionName')
         return self
 
 
+class DescribeDBClusterVersionResponseBodyProxyRevisionVersionList(TeaModel):
+    def __init__(
+        self,
+        release_note: str = None,
+        release_type: str = None,
+        revision_version_code: str = None,
+        revision_version_name: str = None,
+    ):
+        self.release_note = release_note
+        self.release_type = release_type
+        self.revision_version_code = revision_version_code
+        self.revision_version_name = revision_version_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.release_note is not None:
+            result['ReleaseNote'] = self.release_note
+        if self.release_type is not None:
+            result['ReleaseType'] = self.release_type
+        if self.revision_version_code is not None:
+            result['RevisionVersionCode'] = self.revision_version_code
+        if self.revision_version_name is not None:
+            result['RevisionVersionName'] = self.revision_version_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ReleaseNote') is not None:
+            self.release_note = m.get('ReleaseNote')
+        if m.get('ReleaseType') is not None:
+            self.release_type = m.get('ReleaseType')
+        if m.get('RevisionVersionCode') is not None:
+            self.revision_version_code = m.get('RevisionVersionCode')
+        if m.get('RevisionVersionName') is not None:
+            self.revision_version_name = m.get('RevisionVersionName')
+        return self
+
+
 class DescribeDBClusterVersionResponseBody(TeaModel):
     def __init__(
         self,
         dbcluster_id: str = None,
         dblatest_version: str = None,
         dbminor_version: str = None,
         dbrevision_version: str = None,
         dbrevision_version_list: List[DescribeDBClusterVersionResponseBodyDBRevisionVersionList] = None,
         dbversion: str = None,
         dbversion_status: str = None,
         is_latest_version: str = None,
         is_proxy_latest_version: str = None,
         proxy_latest_version: str = None,
         proxy_revision_version: str = None,
+        proxy_revision_version_list: List[DescribeDBClusterVersionResponseBodyProxyRevisionVersionList] = None,
         proxy_version_status: str = None,
         request_id: str = None,
     ):
         # The ID of cluster.
         self.dbcluster_id = dbcluster_id
         # The latest version of the database engine.
         self.dblatest_version = dblatest_version
@@ -12924,14 +12970,15 @@
         # - true
         # - false
         self.is_proxy_latest_version = is_proxy_latest_version
         # The latest version of PolarProxy.
         self.proxy_latest_version = proxy_latest_version
         # The revision version of the database engine.
         self.proxy_revision_version = proxy_revision_version
+        self.proxy_revision_version_list = proxy_revision_version_list
         # The status of PolarProxy. Valid values:
         # 
         # - Stable: The minor version is stable.
         # - Old: The minor version is outdated. We recommend that you upgrade the cluster to the latest version.
         # - HighRisk: The minor version has critical defects. We recommend that you immediately upgrade the cluster to the latest version.
         # - Beta: The minor version is a beta version.
         self.proxy_version_status = proxy_version_status
@@ -12939,14 +12986,18 @@
         self.request_id = request_id
 
     def validate(self):
         if self.dbrevision_version_list:
             for k in self.dbrevision_version_list:
                 if k:
                     k.validate()
+        if self.proxy_revision_version_list:
+            for k in self.proxy_revision_version_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -12970,14 +13021,18 @@
             result['IsLatestVersion'] = self.is_latest_version
         if self.is_proxy_latest_version is not None:
             result['IsProxyLatestVersion'] = self.is_proxy_latest_version
         if self.proxy_latest_version is not None:
             result['ProxyLatestVersion'] = self.proxy_latest_version
         if self.proxy_revision_version is not None:
             result['ProxyRevisionVersion'] = self.proxy_revision_version
+        result['ProxyRevisionVersionList'] = []
+        if self.proxy_revision_version_list is not None:
+            for k in self.proxy_revision_version_list:
+                result['ProxyRevisionVersionList'].append(k.to_map() if k else None)
         if self.proxy_version_status is not None:
             result['ProxyVersionStatus'] = self.proxy_version_status
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         return result
 
     def from_map(self, m: dict = None):
@@ -13003,14 +13058,19 @@
             self.is_latest_version = m.get('IsLatestVersion')
         if m.get('IsProxyLatestVersion') is not None:
             self.is_proxy_latest_version = m.get('IsProxyLatestVersion')
         if m.get('ProxyLatestVersion') is not None:
             self.proxy_latest_version = m.get('ProxyLatestVersion')
         if m.get('ProxyRevisionVersion') is not None:
             self.proxy_revision_version = m.get('ProxyRevisionVersion')
+        self.proxy_revision_version_list = []
+        if m.get('ProxyRevisionVersionList') is not None:
+            for k in m.get('ProxyRevisionVersionList'):
+                temp_model = DescribeDBClusterVersionResponseBodyProxyRevisionVersionList()
+                self.proxy_revision_version_list.append(temp_model.from_map(k))
         if m.get('ProxyVersionStatus') is not None:
             self.proxy_version_status = m.get('ProxyVersionStatus')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
@@ -32443,14 +32503,15 @@
         owner_account: str = None,
         owner_id: int = None,
         planned_end_time: str = None,
         planned_start_time: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         target_dbrevision_version_code: str = None,
+        target_proxy_revision_version_code: str = None,
         upgrade_label: str = None,
         upgrade_policy: str = None,
         upgrade_type: str = None,
     ):
         # The ID of cluster.
         # 
         # This parameter is required.
@@ -32474,14 +32535,15 @@
         # > *   The earliest start time of the task can be a point in time within the next 24 hours. For example, if the current time is `2021-01-14T09:00:00Z`, you can specify a point in time between `2021-01-14T09:00:00Z` and `2021-01-15T09:00:00Z`.
         # >*   If you do not specify this parameter, the kernel update task runs immediately after you submit the request.
         self.planned_start_time = planned_start_time
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The code of the version to which you want to upgrade the cluster. You can call the [DescribeDBClusterVersion](https://help.aliyun.com/document_detail/2319145.html) operation to query the version code.
         self.target_dbrevision_version_code = target_dbrevision_version_code
+        self.target_proxy_revision_version_code = target_proxy_revision_version_code
         # The upgrade tag. The value is fixed as **INNOVATE**.
         # 
         # > *   This parameter is applicable only when you upgrade PolarDB for MySQL 8.0.1 to PolarDB for MySQL 8.0.2.
         # >*   If you specify this parameter, you must set `UpgradePolicy` to **COLD**.
         self.upgrade_label = upgrade_label
         # The upgrade policy. Valid values:
         # 
@@ -32518,14 +32580,16 @@
             result['PlannedStartTime'] = self.planned_start_time
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
         if self.target_dbrevision_version_code is not None:
             result['TargetDBRevisionVersionCode'] = self.target_dbrevision_version_code
+        if self.target_proxy_revision_version_code is not None:
+            result['TargetProxyRevisionVersionCode'] = self.target_proxy_revision_version_code
         if self.upgrade_label is not None:
             result['UpgradeLabel'] = self.upgrade_label
         if self.upgrade_policy is not None:
             result['UpgradePolicy'] = self.upgrade_policy
         if self.upgrade_type is not None:
             result['UpgradeType'] = self.upgrade_type
         return result
@@ -32546,14 +32610,16 @@
             self.planned_start_time = m.get('PlannedStartTime')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
         if m.get('TargetDBRevisionVersionCode') is not None:
             self.target_dbrevision_version_code = m.get('TargetDBRevisionVersionCode')
+        if m.get('TargetProxyRevisionVersionCode') is not None:
+            self.target_proxy_revision_version_code = m.get('TargetProxyRevisionVersionCode')
         if m.get('UpgradeLabel') is not None:
             self.upgrade_label = m.get('UpgradeLabel')
         if m.get('UpgradePolicy') is not None:
             self.upgrade_policy = m.get('UpgradePolicy')
         if m.get('UpgradeType') is not None:
             self.upgrade_type = m.get('UpgradeType')
         return self
```

### Comparing `alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/PKG-INFO` & `alibabacloud_polardb20170801-5.1.2/alibabacloud_polardb20170801.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-polardb20170801
-Version: 5.1.1
+Version: 5.1.2
 Summary: Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_polardb20170801-5.1.1/setup.py` & `alibabacloud_polardb20170801-5.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_polardb20170801.
 
-Created on 17/05/2024
+Created on 28/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_polardb20170801"
 NAME = "alibabacloud_polardb20170801" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python"
```

