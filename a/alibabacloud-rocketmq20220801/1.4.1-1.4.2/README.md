# Comparing `tmp/alibabacloud_rocketmq20220801-1.4.1.tar.gz` & `tmp/alibabacloud_rocketmq20220801-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rocketmq20220801-1.4.1.tar", last modified: Fri Mar 29 17:19:12 2024, max compression
+gzip compressed data, was "dist/alibabacloud_rocketmq20220801-1.4.2.tar", last modified: Tue May 28 17:17:03 2024, max compression
```

## Comparing `alibabacloud_rocketmq20220801-1.4.1.tar` & `alibabacloud_rocketmq20220801-1.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/
--rw-r--r--   0 root         (0) root         (0)     1193 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92904 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801/client.py
--rw-r--r--   0 root         (0) root         (0)   217650 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-03-29 17:19:12.000000 alibabacloud_rocketmq20220801-1.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/
+-rw-r--r--   0 root         (0) root         (0)     1318 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   105632 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801/client.py
+-rw-r--r--   0 root         (0) root         (0)   223043 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-05-28 17:17:03.000000 alibabacloud_rocketmq20220801-1.4.2/setup.py
```

### Comparing `alibabacloud_rocketmq20220801-1.4.1/ChangeLog.md` & `alibabacloud_rocketmq20220801-1.4.2/ChangeLog.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-03-29 Version: 1.4.1
+- Update API GetInstance: update response param.
+- Update API UpdateInstance: update param body.
+
+
 2024-03-28 Version: 1.4.0
 - Support API ListAvailableZones.
 - Support API ListConsumerConnections.
 - Support API ListRegions.
 - Support API ListTopicSubscriptions.
 - Update API ListTopics: update param pageNumber.
 - Update API ListTopics: update param pageSize.
```

### Comparing `alibabacloud_rocketmq20220801-1.4.1/LICENSE` & `alibabacloud_rocketmq20220801-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801-1.4.1/PKG-INFO` & `alibabacloud_rocketmq20220801-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rocketmq20220801
-Version: 1.4.1
+Version: 1.4.2
 Summary: Alibaba Cloud RocketMQ (20220801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rocketmq20220801-1.4.1/README-CN.md` & `alibabacloud_rocketmq20220801-1.4.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801-1.4.1/README.md` & `alibabacloud_rocketmq20220801-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801/client.py` & `alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,22 @@
 
     def change_resource_group_with_options(
         self,
         request: rocket_mq20220801_models.ChangeResourceGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ChangeResourceGroupResponse:
+        """
+        @summary Changes the resource group to which a ApsaraMQ for RocketMQ instance belongs.
+        
+        @param request: ChangeResourceGroupRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ChangeResourceGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['regionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['resourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.resource_id):
@@ -79,14 +87,22 @@
 
     async def change_resource_group_with_options_async(
         self,
         request: rocket_mq20220801_models.ChangeResourceGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ChangeResourceGroupResponse:
+        """
+        @summary Changes the resource group to which a ApsaraMQ for RocketMQ instance belongs.
+        
+        @param request: ChangeResourceGroupRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ChangeResourceGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['regionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['resourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.resource_id):
@@ -113,36 +129,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def change_resource_group(
         self,
         request: rocket_mq20220801_models.ChangeResourceGroupRequest,
     ) -> rocket_mq20220801_models.ChangeResourceGroupResponse:
+        """
+        @summary Changes the resource group to which a ApsaraMQ for RocketMQ instance belongs.
+        
+        @param request: ChangeResourceGroupRequest
+        @return: ChangeResourceGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.change_resource_group_with_options(request, headers, runtime)
 
     async def change_resource_group_async(
         self,
         request: rocket_mq20220801_models.ChangeResourceGroupRequest,
     ) -> rocket_mq20220801_models.ChangeResourceGroupResponse:
+        """
+        @summary Changes the resource group to which a ApsaraMQ for RocketMQ instance belongs.
+        
+        @param request: ChangeResourceGroupRequest
+        @return: ChangeResourceGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.change_resource_group_with_options_async(request, headers, runtime)
 
     def create_consumer_group_with_options(
         self,
         instance_id: str,
         consumer_group_id: str,
         request: rocket_mq20220801_models.CreateConsumerGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.CreateConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Creates a consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: CreateConsumerGroupRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateConsumerGroupResponse
         """
         UtilClient.validate_model(request)
@@ -178,15 +208,17 @@
         instance_id: str,
         consumer_group_id: str,
         request: rocket_mq20220801_models.CreateConsumerGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.CreateConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Creates a consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: CreateConsumerGroupRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateConsumerGroupResponse
         """
         UtilClient.validate_model(request)
@@ -220,15 +252,17 @@
     def create_consumer_group(
         self,
         instance_id: str,
         consumer_group_id: str,
         request: rocket_mq20220801_models.CreateConsumerGroupRequest,
     ) -> rocket_mq20220801_models.CreateConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Creates a consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: CreateConsumerGroupRequest
         @return: CreateConsumerGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_consumer_group_with_options(instance_id, consumer_group_id, request, headers, runtime)
@@ -236,15 +270,17 @@
     async def create_consumer_group_async(
         self,
         instance_id: str,
         consumer_group_id: str,
         request: rocket_mq20220801_models.CreateConsumerGroupRequest,
     ) -> rocket_mq20220801_models.CreateConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Creates a consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: CreateConsumerGroupRequest
         @return: CreateConsumerGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_consumer_group_with_options_async(instance_id, consumer_group_id, request, headers, runtime)
@@ -252,15 +288,17 @@
     def create_instance_with_options(
         self,
         request: rocket_mq20220801_models.CreateInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.CreateInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Creates an ApsaraMQ for RocketMQ 5.x instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: CreateInstanceRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateInstanceResponse
         """
         UtilClient.validate_model(request)
@@ -320,15 +358,17 @@
     async def create_instance_with_options_async(
         self,
         request: rocket_mq20220801_models.CreateInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.CreateInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Creates an ApsaraMQ for RocketMQ 5.x instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: CreateInstanceRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateInstanceResponse
         """
         UtilClient.validate_model(request)
@@ -386,29 +426,33 @@
         )
 
     def create_instance(
         self,
         request: rocket_mq20220801_models.CreateInstanceRequest,
     ) -> rocket_mq20220801_models.CreateInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Creates an ApsaraMQ for RocketMQ 5.x instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: CreateInstanceRequest
         @return: CreateInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_instance_with_options(request, headers, runtime)
 
     async def create_instance_async(
         self,
         request: rocket_mq20220801_models.CreateInstanceRequest,
     ) -> rocket_mq20220801_models.CreateInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Creates an ApsaraMQ for RocketMQ 5.x instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: CreateInstanceRequest
         @return: CreateInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_instance_with_options_async(request, headers, runtime)
@@ -417,14 +461,22 @@
         self,
         instance_id: str,
         topic_name: str,
         request: rocket_mq20220801_models.CreateTopicRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.CreateTopicResponse:
+        """
+        @summary Creates a topic.
+        
+        @param request: CreateTopicRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTopicResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.message_type):
             body['messageType'] = request.message_type
         if not UtilClient.is_unset(request.remark):
             body['remark'] = request.remark
         req = open_api_models.OpenApiRequest(
@@ -451,14 +503,22 @@
         self,
         instance_id: str,
         topic_name: str,
         request: rocket_mq20220801_models.CreateTopicRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.CreateTopicResponse:
+        """
+        @summary Creates a topic.
+        
+        @param request: CreateTopicRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTopicResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.message_type):
             body['messageType'] = request.message_type
         if not UtilClient.is_unset(request.remark):
             body['remark'] = request.remark
         req = open_api_models.OpenApiRequest(
@@ -483,37 +543,51 @@
 
     def create_topic(
         self,
         instance_id: str,
         topic_name: str,
         request: rocket_mq20220801_models.CreateTopicRequest,
     ) -> rocket_mq20220801_models.CreateTopicResponse:
+        """
+        @summary Creates a topic.
+        
+        @param request: CreateTopicRequest
+        @return: CreateTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_topic_with_options(instance_id, topic_name, request, headers, runtime)
 
     async def create_topic_async(
         self,
         instance_id: str,
         topic_name: str,
         request: rocket_mq20220801_models.CreateTopicRequest,
     ) -> rocket_mq20220801_models.CreateTopicResponse:
+        """
+        @summary Creates a topic.
+        
+        @param request: CreateTopicRequest
+        @return: CreateTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_topic_with_options_async(instance_id, topic_name, request, headers, runtime)
 
     def delete_consumer_group_with_options(
         self,
         instance_id: str,
         consumer_group_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.DeleteConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Deletes a specified consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         After you delete a consumer group, the consumer client associated with the consumer group cannot consume messages. Exercise caution when you call this operation.
         
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteConsumerGroupResponse
         """
         req = open_api_models.OpenApiRequest(
@@ -539,15 +613,17 @@
         self,
         instance_id: str,
         consumer_group_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.DeleteConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Deletes a specified consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         After you delete a consumer group, the consumer client associated with the consumer group cannot consume messages. Exercise caution when you call this operation.
         
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteConsumerGroupResponse
         """
         req = open_api_models.OpenApiRequest(
@@ -571,30 +647,34 @@
 
     def delete_consumer_group(
         self,
         instance_id: str,
         consumer_group_id: str,
     ) -> rocket_mq20220801_models.DeleteConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Deletes a specified consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         After you delete a consumer group, the consumer client associated with the consumer group cannot consume messages. Exercise caution when you call this operation.
         
         @return: DeleteConsumerGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.delete_consumer_group_with_options(instance_id, consumer_group_id, headers, runtime)
 
     async def delete_consumer_group_async(
         self,
         instance_id: str,
         consumer_group_id: str,
     ) -> rocket_mq20220801_models.DeleteConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Deletes a specified consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         After you delete a consumer group, the consumer client associated with the consumer group cannot consume messages. Exercise caution when you call this operation.
         
         @return: DeleteConsumerGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.delete_consumer_group_with_options_async(instance_id, consumer_group_id, headers, runtime)
@@ -602,17 +682,19 @@
     def delete_instance_with_options(
         self,
         instance_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.DeleteInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
-        *   After an instance is deleted, the instance cannot be restored. Exercise caution when you call this operation.
-        *   This operation is used to delete a pay-as-you-go instance. A subscription instance is automatically released after it expires. You do not need to manually delete a subscription instance.
+        @summary Deletes a ApsaraMQ for RocketMQ instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        After an instance is deleted, the instance cannot be restored. Exercise caution when you call this operation.
+        This operation is used to delete a pay-as-you-go instance. A subscription instance is automatically released after it expires. You do not need to manually delete a subscription instance.
         
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteInstanceResponse
         """
         req = open_api_models.OpenApiRequest(
             headers=headers
@@ -636,17 +718,19 @@
     async def delete_instance_with_options_async(
         self,
         instance_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.DeleteInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
-        *   After an instance is deleted, the instance cannot be restored. Exercise caution when you call this operation.
-        *   This operation is used to delete a pay-as-you-go instance. A subscription instance is automatically released after it expires. You do not need to manually delete a subscription instance.
+        @summary Deletes a ApsaraMQ for RocketMQ instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        After an instance is deleted, the instance cannot be restored. Exercise caution when you call this operation.
+        This operation is used to delete a pay-as-you-go instance. A subscription instance is automatically released after it expires. You do not need to manually delete a subscription instance.
         
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteInstanceResponse
         """
         req = open_api_models.OpenApiRequest(
             headers=headers
@@ -668,32 +752,36 @@
         )
 
     def delete_instance(
         self,
         instance_id: str,
     ) -> rocket_mq20220801_models.DeleteInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
-        *   After an instance is deleted, the instance cannot be restored. Exercise caution when you call this operation.
-        *   This operation is used to delete a pay-as-you-go instance. A subscription instance is automatically released after it expires. You do not need to manually delete a subscription instance.
+        @summary Deletes a ApsaraMQ for RocketMQ instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        After an instance is deleted, the instance cannot be restored. Exercise caution when you call this operation.
+        This operation is used to delete a pay-as-you-go instance. A subscription instance is automatically released after it expires. You do not need to manually delete a subscription instance.
         
         @return: DeleteInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.delete_instance_with_options(instance_id, headers, runtime)
 
     async def delete_instance_async(
         self,
         instance_id: str,
     ) -> rocket_mq20220801_models.DeleteInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
-        *   After an instance is deleted, the instance cannot be restored. Exercise caution when you call this operation.
-        *   This operation is used to delete a pay-as-you-go instance. A subscription instance is automatically released after it expires. You do not need to manually delete a subscription instance.
+        @summary Deletes a ApsaraMQ for RocketMQ instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        After an instance is deleted, the instance cannot be restored. Exercise caution when you call this operation.
+        This operation is used to delete a pay-as-you-go instance. A subscription instance is automatically released after it expires. You do not need to manually delete a subscription instance.
         
         @return: DeleteInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.delete_instance_with_options_async(instance_id, headers, runtime)
 
@@ -701,15 +789,17 @@
         self,
         instance_id: str,
         topic_name: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.DeleteTopicResponse:
         """
-        If you delete the topic, the publishing and subscription relationships that are established based on the topic are cleared. Exercise caution when you call this operation.
+        @summary Deletes a specified topic.
+        
+        @description If you delete the topic, the publishing and subscription relationships that are established based on the topic are cleared. Exercise caution when you call this operation.
         
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteTopicResponse
         """
         req = open_api_models.OpenApiRequest(
             headers=headers
@@ -734,15 +824,17 @@
         self,
         instance_id: str,
         topic_name: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.DeleteTopicResponse:
         """
-        If you delete the topic, the publishing and subscription relationships that are established based on the topic are cleared. Exercise caution when you call this operation.
+        @summary Deletes a specified topic.
+        
+        @description If you delete the topic, the publishing and subscription relationships that are established based on the topic are cleared. Exercise caution when you call this operation.
         
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteTopicResponse
         """
         req = open_api_models.OpenApiRequest(
             headers=headers
@@ -765,29 +857,33 @@
 
     def delete_topic(
         self,
         instance_id: str,
         topic_name: str,
     ) -> rocket_mq20220801_models.DeleteTopicResponse:
         """
-        If you delete the topic, the publishing and subscription relationships that are established based on the topic are cleared. Exercise caution when you call this operation.
+        @summary Deletes a specified topic.
+        
+        @description If you delete the topic, the publishing and subscription relationships that are established based on the topic are cleared. Exercise caution when you call this operation.
         
         @return: DeleteTopicResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.delete_topic_with_options(instance_id, topic_name, headers, runtime)
 
     async def delete_topic_async(
         self,
         instance_id: str,
         topic_name: str,
     ) -> rocket_mq20220801_models.DeleteTopicResponse:
         """
-        If you delete the topic, the publishing and subscription relationships that are established based on the topic are cleared. Exercise caution when you call this operation.
+        @summary Deletes a specified topic.
+        
+        @description If you delete the topic, the publishing and subscription relationships that are established based on the topic are cleared. Exercise caution when you call this operation.
         
         @return: DeleteTopicResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.delete_topic_with_options_async(instance_id, topic_name, headers, runtime)
 
@@ -795,15 +891,17 @@
         self,
         instance_id: str,
         consumer_group_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.GetConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries the details of a specified consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetConsumerGroupResponse
         """
         req = open_api_models.OpenApiRequest(
             headers=headers
@@ -828,15 +926,17 @@
         self,
         instance_id: str,
         consumer_group_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.GetConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries the details of a specified consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetConsumerGroupResponse
         """
         req = open_api_models.OpenApiRequest(
             headers=headers
@@ -859,44 +959,50 @@
 
     def get_consumer_group(
         self,
         instance_id: str,
         consumer_group_id: str,
     ) -> rocket_mq20220801_models.GetConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries the details of a specified consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @return: GetConsumerGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_consumer_group_with_options(instance_id, consumer_group_id, headers, runtime)
 
     async def get_consumer_group_async(
         self,
         instance_id: str,
         consumer_group_id: str,
     ) -> rocket_mq20220801_models.GetConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries the details of a specified consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @return: GetConsumerGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_consumer_group_with_options_async(instance_id, consumer_group_id, headers, runtime)
 
     def get_instance_with_options(
         self,
         instance_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.GetInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries the detailed information about an instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetInstanceResponse
         """
         req = open_api_models.OpenApiRequest(
             headers=headers
@@ -920,15 +1026,17 @@
     async def get_instance_with_options_async(
         self,
         instance_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.GetInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries the detailed information about an instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetInstanceResponse
         """
         req = open_api_models.OpenApiRequest(
             headers=headers
@@ -950,42 +1058,53 @@
         )
 
     def get_instance(
         self,
         instance_id: str,
     ) -> rocket_mq20220801_models.GetInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries the detailed information about an instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @return: GetInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_instance_with_options(instance_id, headers, runtime)
 
     async def get_instance_async(
         self,
         instance_id: str,
     ) -> rocket_mq20220801_models.GetInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries the detailed information about an instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @return: GetInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_instance_with_options_async(instance_id, headers, runtime)
 
     def get_topic_with_options(
         self,
         instance_id: str,
         topic_name: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.GetTopicResponse:
+        """
+        @summary Queries the details of a specified topic.
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTopicResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTopic',
             version='2022-08-01',
             protocol='HTTPS',
@@ -1004,14 +1123,21 @@
     async def get_topic_with_options_async(
         self,
         instance_id: str,
         topic_name: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.GetTopicResponse:
+        """
+        @summary Queries the details of a specified topic.
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTopicResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTopic',
             version='2022-08-01',
             protocol='HTTPS',
@@ -1028,32 +1154,49 @@
         )
 
     def get_topic(
         self,
         instance_id: str,
         topic_name: str,
     ) -> rocket_mq20220801_models.GetTopicResponse:
+        """
+        @summary Queries the details of a specified topic.
+        
+        @return: GetTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_topic_with_options(instance_id, topic_name, headers, runtime)
 
     async def get_topic_async(
         self,
         instance_id: str,
         topic_name: str,
     ) -> rocket_mq20220801_models.GetTopicResponse:
+        """
+        @summary Queries the details of a specified topic.
+        
+        @return: GetTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_topic_with_options_async(instance_id, topic_name, headers, runtime)
 
     def list_available_zones_with_options(
         self,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListAvailableZonesResponse:
+        """
+        @summary 查询支持的可用区
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAvailableZonesResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListAvailableZones',
             version='2022-08-01',
             protocol='HTTPS',
@@ -1070,14 +1213,21 @@
         )
 
     async def list_available_zones_with_options_async(
         self,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListAvailableZonesResponse:
+        """
+        @summary 查询支持的可用区
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAvailableZonesResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListAvailableZones',
             version='2022-08-01',
             protocol='HTTPS',
@@ -1090,30 +1240,47 @@
         )
         return TeaCore.from_map(
             rocket_mq20220801_models.ListAvailableZonesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def list_available_zones(self) -> rocket_mq20220801_models.ListAvailableZonesResponse:
+        """
+        @summary 查询支持的可用区
+        
+        @return: ListAvailableZonesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_available_zones_with_options(headers, runtime)
 
     async def list_available_zones_async(self) -> rocket_mq20220801_models.ListAvailableZonesResponse:
+        """
+        @summary 查询支持的可用区
+        
+        @return: ListAvailableZonesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_available_zones_with_options_async(headers, runtime)
 
     def list_consumer_connections_with_options(
         self,
         instance_id: str,
         consumer_group_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListConsumerConnectionsResponse:
+        """
+        @summary 查询消费者客户端连接信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListConsumerConnectionsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListConsumerConnections',
             version='2022-08-01',
             protocol='HTTPS',
@@ -1132,14 +1299,21 @@
     async def list_consumer_connections_with_options_async(
         self,
         instance_id: str,
         consumer_group_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListConsumerConnectionsResponse:
+        """
+        @summary 查询消费者客户端连接信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListConsumerConnectionsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListConsumerConnections',
             version='2022-08-01',
             protocol='HTTPS',
@@ -1156,34 +1330,51 @@
         )
 
     def list_consumer_connections(
         self,
         instance_id: str,
         consumer_group_id: str,
     ) -> rocket_mq20220801_models.ListConsumerConnectionsResponse:
+        """
+        @summary 查询消费者客户端连接信息
+        
+        @return: ListConsumerConnectionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_consumer_connections_with_options(instance_id, consumer_group_id, headers, runtime)
 
     async def list_consumer_connections_async(
         self,
         instance_id: str,
         consumer_group_id: str,
     ) -> rocket_mq20220801_models.ListConsumerConnectionsResponse:
+        """
+        @summary 查询消费者客户端连接信息
+        
+        @return: ListConsumerConnectionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_consumer_connections_with_options_async(instance_id, consumer_group_id, headers, runtime)
 
     def list_consumer_group_subscriptions_with_options(
         self,
         instance_id: str,
         consumer_group_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListConsumerGroupSubscriptionsResponse:
+        """
+        @summary Queries the subscriptions of a consumer group.
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListConsumerGroupSubscriptionsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListConsumerGroupSubscriptions',
             version='2022-08-01',
             protocol='HTTPS',
@@ -1202,14 +1393,21 @@
     async def list_consumer_group_subscriptions_with_options_async(
         self,
         instance_id: str,
         consumer_group_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListConsumerGroupSubscriptionsResponse:
+        """
+        @summary Queries the subscriptions of a consumer group.
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListConsumerGroupSubscriptionsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListConsumerGroupSubscriptions',
             version='2022-08-01',
             protocol='HTTPS',
@@ -1226,36 +1424,48 @@
         )
 
     def list_consumer_group_subscriptions(
         self,
         instance_id: str,
         consumer_group_id: str,
     ) -> rocket_mq20220801_models.ListConsumerGroupSubscriptionsResponse:
+        """
+        @summary Queries the subscriptions of a consumer group.
+        
+        @return: ListConsumerGroupSubscriptionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_consumer_group_subscriptions_with_options(instance_id, consumer_group_id, headers, runtime)
 
     async def list_consumer_group_subscriptions_async(
         self,
         instance_id: str,
         consumer_group_id: str,
     ) -> rocket_mq20220801_models.ListConsumerGroupSubscriptionsResponse:
+        """
+        @summary Queries the subscriptions of a consumer group.
+        
+        @return: ListConsumerGroupSubscriptionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_consumer_group_subscriptions_with_options_async(instance_id, consumer_group_id, headers, runtime)
 
     def list_consumer_groups_with_options(
         self,
         instance_id: str,
         request: rocket_mq20220801_models.ListConsumerGroupsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListConsumerGroupsResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries the consumer groups in a specified instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: ListConsumerGroupsRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListConsumerGroupsResponse
         """
         UtilClient.validate_model(request)
@@ -1290,15 +1500,17 @@
         self,
         instance_id: str,
         request: rocket_mq20220801_models.ListConsumerGroupsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListConsumerGroupsResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries the consumer groups in a specified instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: ListConsumerGroupsRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListConsumerGroupsResponse
         """
         UtilClient.validate_model(request)
@@ -1331,30 +1543,34 @@
 
     def list_consumer_groups(
         self,
         instance_id: str,
         request: rocket_mq20220801_models.ListConsumerGroupsRequest,
     ) -> rocket_mq20220801_models.ListConsumerGroupsResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries the consumer groups in a specified instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: ListConsumerGroupsRequest
         @return: ListConsumerGroupsResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_consumer_groups_with_options(instance_id, request, headers, runtime)
 
     async def list_consumer_groups_async(
         self,
         instance_id: str,
         request: rocket_mq20220801_models.ListConsumerGroupsRequest,
     ) -> rocket_mq20220801_models.ListConsumerGroupsResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries the consumer groups in a specified instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: ListConsumerGroupsRequest
         @return: ListConsumerGroupsResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_consumer_groups_with_options_async(instance_id, request, headers, runtime)
@@ -1362,15 +1578,17 @@
     def list_instances_with_options(
         self,
         request: rocket_mq20220801_models.ListInstancesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListInstancesResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries instances.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: ListInstancesRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListInstancesResponse
         """
         UtilClient.validate_model(request)
@@ -1408,15 +1626,17 @@
     async def list_instances_with_options_async(
         self,
         request: rocket_mq20220801_models.ListInstancesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListInstancesResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries instances.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: ListInstancesRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListInstancesResponse
         """
         UtilClient.validate_model(request)
@@ -1452,42 +1672,53 @@
         )
 
     def list_instances(
         self,
         request: rocket_mq20220801_models.ListInstancesRequest,
     ) -> rocket_mq20220801_models.ListInstancesResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries instances.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: ListInstancesRequest
         @return: ListInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_instances_with_options(request, headers, runtime)
 
     async def list_instances_async(
         self,
         request: rocket_mq20220801_models.ListInstancesRequest,
     ) -> rocket_mq20220801_models.ListInstancesResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Queries instances.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: ListInstancesRequest
         @return: ListInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_instances_with_options_async(request, headers, runtime)
 
     def list_regions_with_options(
         self,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListRegionsResponse:
+        """
+        @summary 查询region列表
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListRegionsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListRegions',
             version='2022-08-01',
             protocol='HTTPS',
@@ -1504,14 +1735,21 @@
         )
 
     async def list_regions_with_options_async(
         self,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListRegionsResponse:
+        """
+        @summary 查询region列表
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListRegionsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListRegions',
             version='2022-08-01',
             protocol='HTTPS',
@@ -1524,30 +1762,47 @@
         )
         return TeaCore.from_map(
             rocket_mq20220801_models.ListRegionsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def list_regions(self) -> rocket_mq20220801_models.ListRegionsResponse:
+        """
+        @summary 查询region列表
+        
+        @return: ListRegionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_regions_with_options(headers, runtime)
 
     async def list_regions_async(self) -> rocket_mq20220801_models.ListRegionsResponse:
+        """
+        @summary 查询region列表
+        
+        @return: ListRegionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_regions_with_options_async(headers, runtime)
 
     def list_topic_subscriptions_with_options(
         self,
         instance_id: str,
         topic_name: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListTopicSubscriptionsResponse:
+        """
+        @summary 查询主题订阅关系列表
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTopicSubscriptionsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListTopicSubscriptions',
             version='2022-08-01',
             protocol='HTTPS',
@@ -1566,14 +1821,21 @@
     async def list_topic_subscriptions_with_options_async(
         self,
         instance_id: str,
         topic_name: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListTopicSubscriptionsResponse:
+        """
+        @summary 查询主题订阅关系列表
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTopicSubscriptionsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListTopicSubscriptions',
             version='2022-08-01',
             protocol='HTTPS',
@@ -1590,34 +1852,52 @@
         )
 
     def list_topic_subscriptions(
         self,
         instance_id: str,
         topic_name: str,
     ) -> rocket_mq20220801_models.ListTopicSubscriptionsResponse:
+        """
+        @summary 查询主题订阅关系列表
+        
+        @return: ListTopicSubscriptionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_topic_subscriptions_with_options(instance_id, topic_name, headers, runtime)
 
     async def list_topic_subscriptions_async(
         self,
         instance_id: str,
         topic_name: str,
     ) -> rocket_mq20220801_models.ListTopicSubscriptionsResponse:
+        """
+        @summary 查询主题订阅关系列表
+        
+        @return: ListTopicSubscriptionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_topic_subscriptions_with_options_async(instance_id, topic_name, headers, runtime)
 
     def list_topics_with_options(
         self,
         instance_id: str,
         tmp_req: rocket_mq20220801_models.ListTopicsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListTopicsResponse:
+        """
+        @summary Queries the topics in a specified instance.
+        
+        @param tmp_req: ListTopicsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTopicsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = rocket_mq20220801_models.ListTopicsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.message_types):
             request.message_types_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.message_types, 'messageTypes', 'simple')
         query = {}
         if not UtilClient.is_unset(request.filter):
@@ -1651,14 +1931,22 @@
     async def list_topics_with_options_async(
         self,
         instance_id: str,
         tmp_req: rocket_mq20220801_models.ListTopicsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ListTopicsResponse:
+        """
+        @summary Queries the topics in a specified instance.
+        
+        @param tmp_req: ListTopicsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTopicsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = rocket_mq20220801_models.ListTopicsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.message_types):
             request.message_types_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.message_types, 'messageTypes', 'simple')
         query = {}
         if not UtilClient.is_unset(request.filter):
@@ -1690,36 +1978,56 @@
         )
 
     def list_topics(
         self,
         instance_id: str,
         request: rocket_mq20220801_models.ListTopicsRequest,
     ) -> rocket_mq20220801_models.ListTopicsResponse:
+        """
+        @summary Queries the topics in a specified instance.
+        
+        @param request: ListTopicsRequest
+        @return: ListTopicsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_topics_with_options(instance_id, request, headers, runtime)
 
     async def list_topics_async(
         self,
         instance_id: str,
         request: rocket_mq20220801_models.ListTopicsRequest,
     ) -> rocket_mq20220801_models.ListTopicsResponse:
+        """
+        @summary Queries the topics in a specified instance.
+        
+        @param request: ListTopicsRequest
+        @return: ListTopicsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_topics_with_options_async(instance_id, request, headers, runtime)
 
     def reset_consume_offset_with_options(
         self,
         instance_id: str,
         consumer_group_id: str,
         topic_name: str,
         request: rocket_mq20220801_models.ResetConsumeOffsetRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ResetConsumeOffsetResponse:
+        """
+        @summary Resets the consumer offset of a consumer group.
+        
+        @param request: ResetConsumeOffsetRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ResetConsumeOffsetResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.reset_time):
             body['resetTime'] = request.reset_time
         if not UtilClient.is_unset(request.reset_type):
             body['resetType'] = request.reset_type
         req = open_api_models.OpenApiRequest(
@@ -1747,14 +2055,22 @@
         instance_id: str,
         consumer_group_id: str,
         topic_name: str,
         request: rocket_mq20220801_models.ResetConsumeOffsetRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.ResetConsumeOffsetResponse:
+        """
+        @summary Resets the consumer offset of a consumer group.
+        
+        @param request: ResetConsumeOffsetRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ResetConsumeOffsetResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.reset_time):
             body['resetTime'] = request.reset_time
         if not UtilClient.is_unset(request.reset_type):
             body['resetType'] = request.reset_type
         req = open_api_models.OpenApiRequest(
@@ -1780,39 +2096,53 @@
     def reset_consume_offset(
         self,
         instance_id: str,
         consumer_group_id: str,
         topic_name: str,
         request: rocket_mq20220801_models.ResetConsumeOffsetRequest,
     ) -> rocket_mq20220801_models.ResetConsumeOffsetResponse:
+        """
+        @summary Resets the consumer offset of a consumer group.
+        
+        @param request: ResetConsumeOffsetRequest
+        @return: ResetConsumeOffsetResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.reset_consume_offset_with_options(instance_id, consumer_group_id, topic_name, request, headers, runtime)
 
     async def reset_consume_offset_async(
         self,
         instance_id: str,
         consumer_group_id: str,
         topic_name: str,
         request: rocket_mq20220801_models.ResetConsumeOffsetRequest,
     ) -> rocket_mq20220801_models.ResetConsumeOffsetResponse:
+        """
+        @summary Resets the consumer offset of a consumer group.
+        
+        @param request: ResetConsumeOffsetRequest
+        @return: ResetConsumeOffsetResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.reset_consume_offset_with_options_async(instance_id, consumer_group_id, topic_name, request, headers, runtime)
 
     def update_consumer_group_with_options(
         self,
         instance_id: str,
         consumer_group_id: str,
         request: rocket_mq20220801_models.UpdateConsumerGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.UpdateConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Updates the basic information about and the consumption retry policy of a consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: UpdateConsumerGroupRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateConsumerGroupResponse
         """
         UtilClient.validate_model(request)
@@ -1848,15 +2178,17 @@
         instance_id: str,
         consumer_group_id: str,
         request: rocket_mq20220801_models.UpdateConsumerGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.UpdateConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Updates the basic information about and the consumption retry policy of a consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: UpdateConsumerGroupRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateConsumerGroupResponse
         """
         UtilClient.validate_model(request)
@@ -1890,15 +2222,17 @@
     def update_consumer_group(
         self,
         instance_id: str,
         consumer_group_id: str,
         request: rocket_mq20220801_models.UpdateConsumerGroupRequest,
     ) -> rocket_mq20220801_models.UpdateConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Updates the basic information about and the consumption retry policy of a consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: UpdateConsumerGroupRequest
         @return: UpdateConsumerGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.update_consumer_group_with_options(instance_id, consumer_group_id, request, headers, runtime)
@@ -1906,15 +2240,17 @@
     async def update_consumer_group_async(
         self,
         instance_id: str,
         consumer_group_id: str,
         request: rocket_mq20220801_models.UpdateConsumerGroupRequest,
     ) -> rocket_mq20220801_models.UpdateConsumerGroupResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Updates the basic information about and the consumption retry policy of a consumer group.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: UpdateConsumerGroupRequest
         @return: UpdateConsumerGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.update_consumer_group_with_options_async(instance_id, consumer_group_id, request, headers, runtime)
@@ -1923,15 +2259,17 @@
         self,
         instance_id: str,
         request: rocket_mq20220801_models.UpdateInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.UpdateInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Updates the basic information and specifications of an ApsaraMQ for RocketMQ instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: UpdateInstanceRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateInstanceResponse
         """
         UtilClient.validate_model(request)
@@ -1970,15 +2308,17 @@
         self,
         instance_id: str,
         request: rocket_mq20220801_models.UpdateInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.UpdateInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Updates the basic information and specifications of an ApsaraMQ for RocketMQ instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: UpdateInstanceRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateInstanceResponse
         """
         UtilClient.validate_model(request)
@@ -2015,30 +2355,34 @@
 
     def update_instance(
         self,
         instance_id: str,
         request: rocket_mq20220801_models.UpdateInstanceRequest,
     ) -> rocket_mq20220801_models.UpdateInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Updates the basic information and specifications of an ApsaraMQ for RocketMQ instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: UpdateInstanceRequest
         @return: UpdateInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.update_instance_with_options(instance_id, request, headers, runtime)
 
     async def update_instance_async(
         self,
         instance_id: str,
         request: rocket_mq20220801_models.UpdateInstanceRequest,
     ) -> rocket_mq20220801_models.UpdateInstanceResponse:
         """
-        > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
+        @summary Updates the basic information and specifications of an ApsaraMQ for RocketMQ instance.
+        
+        @description > API operations provided by Alibaba Cloud are used to manage and query resources of Alibaba Cloud services. We recommend that you integrate these API operations only in management systems. Do not use these API operations in the core system of messaging services. Otherwise, system risks may occur.
         
         @param request: UpdateInstanceRequest
         @return: UpdateInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.update_instance_with_options_async(instance_id, request, headers, runtime)
@@ -2047,14 +2391,22 @@
         self,
         instance_id: str,
         topic_name: str,
         request: rocket_mq20220801_models.UpdateTopicRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.UpdateTopicResponse:
+        """
+        @summary Updates the basic information about a topic.
+        
+        @param request: UpdateTopicRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTopicResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.remark):
             body['remark'] = request.remark
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -2079,14 +2431,22 @@
         self,
         instance_id: str,
         topic_name: str,
         request: rocket_mq20220801_models.UpdateTopicRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> rocket_mq20220801_models.UpdateTopicResponse:
+        """
+        @summary Updates the basic information about a topic.
+        
+        @param request: UpdateTopicRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTopicResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.remark):
             body['remark'] = request.remark
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -2109,20 +2469,32 @@
 
     def update_topic(
         self,
         instance_id: str,
         topic_name: str,
         request: rocket_mq20220801_models.UpdateTopicRequest,
     ) -> rocket_mq20220801_models.UpdateTopicResponse:
+        """
+        @summary Updates the basic information about a topic.
+        
+        @param request: UpdateTopicRequest
+        @return: UpdateTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.update_topic_with_options(instance_id, topic_name, request, headers, runtime)
 
     async def update_topic_async(
         self,
         instance_id: str,
         topic_name: str,
         request: rocket_mq20220801_models.UpdateTopicRequest,
     ) -> rocket_mq20220801_models.UpdateTopicResponse:
+        """
+        @summary Updates the basic information about a topic.
+        
+        @param request: UpdateTopicRequest
+        @return: UpdateTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.update_topic_with_options_async(instance_id, topic_name, request, headers, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801/models.py` & `alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,32 @@
         self,
         region_id: str = None,
         resource_group_id: str = None,
         resource_id: str = None,
         resource_type: str = None,
     ):
         # The ID of the region in which the instance resides.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group to which the instance is changed.
         # 
         # You can call the [ListResourceGroups](https://www.alibabacloud.com/help/resource-management/latest/listresourcegroups) operation to query existing resource groups.
+        # 
+        # This parameter is required.
         self.resource_group_id = resource_group_id
         # The ID of the resource. Set this parameter to the ID of the ApsaraMQ for RocketMQ instance whose resource group you want to change.
+        # 
+        # This parameter is required.
         self.resource_id = resource_id
         # The type of resource.
         # 
         # Set this parameter to **instance**. The value of this parameter cannot be changed.
+        # 
+        # This parameter is required.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -180,24 +188,26 @@
         self,
         dead_letter_target_topic: str = None,
         max_retry_times: int = None,
         retry_policy: str = None,
     ):
         # The dead-letter topic.
         # 
-        # If a consumer still fails to consume a message after the message is retried for a specified number of times, the message is delivered to a dead-letter topic for subsequent business recovery or troubleshooting. For more information, see [Consumption retry and dead-letter messages](~~440356~~).
+        # If a consumer still fails to consume a message after the message is retried for a specified number of times, the message is delivered to a dead-letter topic for subsequent business recovery or troubleshooting. For more information, see [Consumption retry and dead-letter messages](https://help.aliyun.com/document_detail/440356.html).
         self.dead_letter_target_topic = dead_letter_target_topic
         # The maximum number of retries.
         self.max_retry_times = max_retry_times
-        # The retry policy. For more information, see [Message retry](~~440356~~).
+        # The retry policy. For more information, see [Message retry](https://help.aliyun.com/document_detail/440356.html).
         # 
         # Valid values:
         # 
         # *   FixedRetryPolicy: Failed messages are retried at a fixed interval.
         # *   DefaultRetryPolicy: Failed messages are retried at incremental intervals as the number of retries increases.
+        # 
+        # This parameter is required.
         self.retry_policy = retry_policy
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -227,22 +237,26 @@
 class CreateConsumerGroupRequest(TeaModel):
     def __init__(
         self,
         consume_retry_policy: CreateConsumerGroupRequestConsumeRetryPolicy = None,
         delivery_order_type: str = None,
         remark: str = None,
     ):
-        # The consumption retry policy that you want to configure for the consumer group. For more information, see [Consumption retry](~~440356~~).
+        # The consumption retry policy that you want to configure for the consumer group. For more information, see [Consumption retry](https://help.aliyun.com/document_detail/440356.html).
+        # 
+        # This parameter is required.
         self.consume_retry_policy = consume_retry_policy
         # The message delivery order of the consumer group.
         # 
         # Valid values:
         # 
         # *   Concurrently: concurrent delivery
         # *   Orderly: ordered delivery
+        # 
+        # This parameter is required.
         self.delivery_order_type = delivery_order_type
         # The remarks on the consumer group.
         self.remark = remark
 
     def validate(self):
         if self.consume_retry_policy:
             self.consume_retry_policy.validate()
@@ -406,24 +420,29 @@
         # Valid values: 1 to 1000.
         self.flow_out_bandwidth = flow_out_bandwidth
         # The billing method of Internet usage.
         # 
         # Valid values:
         # 
         # *   payByBandwidth: pay-by-bandwidth. If Internet access is enabled for an instance, specify this value for the parameter.
+        # *   payByTraffic: pay-by-traffic. If Internet access is enabled for an instance, specify this value for the parameter.
         # *   uninvolved: No billing method is involved. If Internet access is disabled for an instance, specify this value for the parameter.
+        # 
+        # This parameter is required.
         self.flow_out_type = flow_out_type
         # Specifies whether to enable the Internet access feature.
         # 
         # Valid values:
         # 
         # *   enable
         # *   disable
         # 
-        # By default, ApsaraMQ for RocketMQ allows you to access instances in VPCs. If you enable Internet access for an instance, you can access the instance over the Internet. After you enable this feature, you are charged for outbound Internet traffic. For more information, see [Internet access fee](~~427240~~).
+        # By default, ApsaraMQ for RocketMQ allows you to access instances in VPCs. If you enable Internet access for an instance, you can access the instance over the Internet. After you enable this feature, you are charged for outbound Internet traffic. For more information, see [Internet access fee](https://help.aliyun.com/document_detail/427240.html).
+        # 
+        # This parameter is required.
         self.internet_spec = internet_spec
         # The whitelist that includes the IP addresses that are allowed to access the ApsaraMQ for RocketMQ broker over the Internet. This parameter can be configured only if you use a public endpoint to access the instance.
         # 
         # *   If you do not configure an IP address whitelist, all CIDR blocks are allowed to access the ApsaraMQ for RocketMQ broker over the Internet.
         # *   If configure an IP address whitlist, only the IP addresses in the whitelist are allowed to access the ApsaraMQ for RocketMQ broker over the Internet.
         self.ip_whitelist = ip_whitelist
 
@@ -464,21 +483,25 @@
         self,
         security_group_ids: str = None,
         v_switch_id: str = None,
         vpc_id: str = None,
     ):
         # The ID of the security group to which the instance belongs.
         self.security_group_ids = security_group_ids
-        # The ID of the vSwitch with which you want to associate the instance.
+        # The ID of the vSwitch with which you want to associate the instance, If there are multiple vSwitchs, please concatenate them using the "|" character.
         # 
         # >  After an ApsaraMQ for RocketMQ instance is created, you cannot change the vSwitch with which the instance is associated. If you want to change the vSwitch with which the instance is associated, you must release the instance and purchase a new instance.
+        # 
+        # This parameter is required.
         self.v_switch_id = v_switch_id
         # The ID of the VPC in which you want to deploy the instance.
         # 
         # >  After an ApsaraMQ for RocketMQ instance is created, you cannot change the VPC in which the instance is deployed. If you want to change the VPC in which the instance is deployed, you must release the instance and create a new instance.
+        # 
+        # This parameter is required.
         self.vpc_id = vpc_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -508,16 +531,20 @@
 class CreateInstanceRequestNetworkInfo(TeaModel):
     def __init__(
         self,
         internet_info: CreateInstanceRequestNetworkInfoInternetInfo = None,
         vpc_info: CreateInstanceRequestNetworkInfoVpcInfo = None,
     ):
         # The Internet-related configurations.
+        # 
+        # This parameter is required.
         self.internet_info = internet_info
         # The virtual private cloud (VPC)-related configurations.
+        # 
+        # This parameter is required.
         self.vpc_info = vpc_info
 
     def validate(self):
         if self.internet_info:
             self.internet_info.validate()
         if self.vpc_info:
             self.vpc_info.validate()
@@ -558,34 +585,36 @@
         # Specifies whether to enable the elastic TPS feature for the instance.
         # 
         # Valid values:
         # 
         # *   true: enable
         # *   false: disable
         # 
-        # After you enable the elastic TPS feature for an ApsaraMQ for RocketMQ instance, you can use a specific number of TPS that exceeds the specification limit. You are charged for using the elastic TPS feature. For more information, see [Computing fees](~~427237~~).
+        # After you enable the elastic TPS feature for an ApsaraMQ for RocketMQ instance, you can use a specific number of TPS that exceeds the specification limit. You are charged for using the elastic TPS feature. For more information, see [Computing fees](https://help.aliyun.com/document_detail/427237.html).
         # 
-        # >  The elastic TPS feature is supported only by instances of specific editions. For more information, see [Instance editions](~~444715~~).
+        # >  The elastic TPS feature is supported only by instances of specific editions. For more information, see [Instance editions](https://help.aliyun.com/document_detail/444715.html).
         self.auto_scaling = auto_scaling
         # The billing method.
         # 
         # Valid values:
         # 
         # *   provisioned
         # *   ondemand
         self.charge_type = charge_type
         # This parameter is no longer used. You do not need to configure this parameter.
         self.intranet_spec = intranet_spec
         # The retention period of messages. Unit: hours.
         # 
-        # For information about the valid values of this parameter, see the "Limits on resource quotas" section of the [Limits](~~440347~~) topic.
+        # For information about the valid values of this parameter, see the "Limits on resource quotas" section of the [Limits](https://help.aliyun.com/document_detail/440347.html) topic.
         # 
-        # ApsaraMQ for RocketMQ supports serverless scaling of message storage. You are charged storage fees based on your actual storage usage. You can change the retention period of messages to manage storage capacity. For more information, see [Storage fees](~~427238~~).
+        # ApsaraMQ for RocketMQ supports serverless scaling of message storage. You are charged storage fees based on your actual storage usage. You can change the retention period of messages to manage storage capacity. For more information, see [Storage fees](https://help.aliyun.com/document_detail/427238.html).
         self.message_retention_time = message_retention_time
-        # The computing specification that specifies the messaging transactions per second (TPS) of the instance. For information about computing specification limits, see [Instance specifications](~~444715~~).
+        # The computing specification that specifies the messaging transactions per second (TPS) of the instance. For information about computing specification limits, see [Instance specifications](https://help.aliyun.com/document_detail/444715.html).
+        # 
+        # This parameter is required.
         self.msg_process_spec = msg_process_spec
         # The proportion of message sending TPS to the messaging TPS on the instance.
         # 
         # For example, you create an instance whose peak messaging TPS is specified as 1,000 and the proportion of message sending TPS is specified as 0.8. In this case, the peak message sending TPS is 800 and the peak message receiving TPS is 200 on the instance.
         # 
         # Valid values: 0 to 1. Default value: 0.5.
         self.send_receive_ratio = send_receive_ratio
@@ -666,23 +695,27 @@
         # *   ons_rmqsub_public_intl: subscription
         self.commodity_code = commodity_code
         # The name of the instance that you want to create.
         # 
         # If you do not configure this parameter, the instance ID is used as the instance name.
         self.instance_name = instance_name
         # The network configurations.
+        # 
+        # This parameter is required.
         self.network_info = network_info
         # The billing method of the instance. ApsaraMQ for RocketMQ supports the subscription and pay-as-you-go billing methods.
         # 
         # Valid values:
         # 
         # *   PayAsYouGo: This billing method allows you to use resources before you pay for the resources.
         # *   Subscription: This billing method allows you to use resources after you pay for the resources.
         # 
-        # For more information, see [Billing methods](~~427234~~).
+        # For more information, see [Billing methods](https://help.aliyun.com/document_detail/427234.html).
+        # 
+        # This parameter is required.
         self.payment_type = payment_type
         # The subscription duration of the instance. This parameter takes effect only if you set PaymentType to Subscription.
         # 
         # Valid values:
         # 
         # *   Monthly subscription: 1, 2, 3, 4, 5, and 6
         # *   Yearly subscription: 1, 2, and 3
@@ -696,36 +729,43 @@
         self.period_unit = period_unit
         # The information about the instance specifications.
         self.product_info = product_info
         # The instance description.
         self.remark = remark
         # The resource group ID.
         self.resource_group_id = resource_group_id
-        # The primary edition of the instance. For information about the differences between primary edition instances, see [Instance selection](~~444722~~).
+        # The primary edition of the instance. For information about the differences between primary edition instances, see [Instance selection](https://help.aliyun.com/document_detail/444722.html).
         # 
         # Valid values:
         # 
         # *   standard: Standard Edition
         # *   ultimate: Enterprise Platinum Edition
         # *   professional: Professional Edition
         # 
         # >  After an instance is created, you can only upgrade the primary edition of the instance. The following editions are sorted in ascending order: Standard Edition, Professional Edition, Enterprise Platinum Edition. For example, you can upgrade an instance of Standard Edition to Professional Edition, but cannot downgrade an instance of Professional Edition to Standard Edition.
+        # 
+        # This parameter is required.
         self.series_code = series_code
         # The code of the service to which the instance belongs. The service code of ApsaraMQ for RocketMQ is rmq.
+        # 
+        # This parameter is required.
         self.service_code = service_code
-        # The sub-category edition of the instance. For information about the differences between sub-category edition instances, see [Instance selection](~~444722~~).
+        # The sub-category edition of the instance. For information about the differences between sub-category edition instances, see [Instance selection](https://help.aliyun.com/document_detail/444722.html).
         # 
         # Valid values:
         # 
         # *   cluster_ha: High-availability Cluster Edition
         # *   single_node: Standalone Edition
+        # *   serverless: Serverless Edition
         # 
         # If you set seriesCode to ultimate, you can set this parameter to only cluster_ha.
         # 
         # >  After an instance is created, you cannot change the sub-category edition of the instance.
+        # 
+        # This parameter is required.
         self.sub_series_code = sub_series_code
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value of this parameter, but you must ensure that the value is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
 
     def validate(self):
         if self.network_info:
             self.network_info.validate()
@@ -1446,15 +1486,15 @@
         self,
         dead_letter_target_topic: str = None,
         max_retry_times: int = None,
         retry_policy: str = None,
     ):
         # The dead-letter topic.
         # 
-        # If a consumer still fails to consume a message after the message is retried for a specified number of times, the message is delivered to a dead-letter topic for subsequent business recovery or troubleshooting. For more information, see [Consumption retry and dead-letter messages](~~440356~~).
+        # If a consumer still fails to consume a message after the message is retried for a specified number of times, the message is delivered to a dead-letter topic for subsequent business recovery or troubleshooting. For more information, see [Consumption retry and dead-letter messages](https://help.aliyun.com/document_detail/440356.html).
         self.dead_letter_target_topic = dead_letter_target_topic
         # The maximum number of retries.
         self.max_retry_times = max_retry_times
         # The retry policy.
         # 
         # Valid values:
         # 
@@ -1524,15 +1564,15 @@
         delivery_order_type: str = None,
         instance_id: str = None,
         region_id: str = None,
         remark: str = None,
         status: str = None,
         update_time: str = None,
     ):
-        # The consumption retry policy that you want to configure for the consumer group. For more information, see [Consumption retry](~~440356~~).
+        # The consumption retry policy that you want to configure for the consumer group. For more information, see [Consumption retry](https://help.aliyun.com/document_detail/440356.html).
         self.consume_retry_policy = consume_retry_policy
         # The ID of the consumer group.
         self.consumer_group_id = consumer_group_id
         # The time when the consumer group was created.
         self.create_time = create_time
         # The message delivery order of the consumer group.
         # 
@@ -1808,31 +1848,43 @@
 class GetInstanceResponseBodyDataAclInfo(TeaModel):
     def __init__(
         self,
         acl_type: str = None,
         acl_types: List[str] = None,
         default_vpc_auth_free: bool = None,
     ):
-        # The authentication types of the instance. Deprecated, it is recommended to use the aclTypes field.
+        # The authentication type of the instance. This parameter is no longer in use. We recommend that you configure aclTypes.
         # 
         # Valid values:
         # 
-        # default: intelligent authentication
+        # - default: intelligent identity authentication
         # 
-        # apache_acl: apache acl authentication
+        # - apache_acl:access control list (ACL) identity authentication**\
         self.acl_type = acl_type
         # The authentication types of the instance.
+        self.acl_types = acl_types
+        # Indicates whether the authentication-free in VPCs feature is enabled.
         # 
         # Valid values:
         # 
-        # default: intelligent authentication
+        # *   true
         # 
-        # apache_acl: apache acl authentication
-        self.acl_types = acl_types
-        # No need for authentication in intranet.
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # *   false
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
         self.default_vpc_auth_free = default_vpc_auth_free
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1900,36 +1952,36 @@
         # Specifies whether to enable the Internet access feature.
         # 
         # Valid values:
         # 
         # *   enable
         # *   disable
         # 
-        # By default, ApsaraMQ for RocketMQ instances are accessed in virtual private clouds (VPCs). If you enable the Internet access feature, you are charged for Internet outbound bandwidth. For more information, see [Internet access fee](~~427240~~).
+        # By default, ApsaraMQ for RocketMQ instances are accessed in virtual private clouds (VPCs). If you enable the Internet access feature, you are charged for Internet outbound bandwidth. For more information, see [Internet access fee](https://help.aliyun.com/document_detail/427240.html).
         self.internet_spec = internet_spec
         # The retention period of messages. Unit: hours.
         # 
-        # For information about the valid values of this parameter, see the "Limits on resource quotas" section in [Usage limits](~~440347~~).
+        # For information about the valid values of this parameter, see the "Limits on resource quotas" section in [Usage limits](https://help.aliyun.com/document_detail/440347.html).
         # 
-        # The storage of messages in ApsaraMQ for RocketMQ is serverless and scalable. You are charged for message storage based on your actual usage. You can change the retention period of messages to adjust storage capacity. For more information, see [Storage fee](~~427238~~).
+        # The storage of messages in ApsaraMQ for RocketMQ is serverless and scalable. You are charged for message storage based on your actual usage. You can change the retention period of messages to adjust storage capacity. For more information, see [Storage fee](https://help.aliyun.com/document_detail/427238.html).
         self.message_retention_time = message_retention_time
-        # The computing specification that is used to send and receive messages. For information about the upper limit of TPS, see [Instance specifications](~~444715~~).
+        # The computing specification that is used to send and receive messages. For information about the upper limit of TPS, see [Instance specifications](https://help.aliyun.com/document_detail/444715.html).
         self.msg_process_spec = msg_process_spec
         # The ratio between sent messages and received messages in the instance.
         self.send_receive_ratio = send_receive_ratio
         # Specifies whether the elastic TPS feature is supported by the instance.
         # 
         # Valid values:
         # 
         # *   true: enable
         # *   false: disable
         # 
-        # After you enable the elastic TPS feature for a ApsaraMQ for RocketMQ instance, you can use a specific amount of TPS that exceeds the specification limit. You are charged for the elastic TPS feature. For more information, see [Computing fee](~~427237~~).
+        # After you enable the elastic TPS feature for a ApsaraMQ for RocketMQ instance, you can use a specific amount of TPS that exceeds the specification limit. You are charged for the elastic TPS feature. For more information, see [Computing fee](https://help.aliyun.com/document_detail/427237.html).
         # 
-        # > The elastic TPS feature is supported only by specific instance editions. For more information, see [Instance specifications](~~444715~~).
+        # > The elastic TPS feature is supported only by specific instance editions. For more information, see [Instance specifications](https://help.aliyun.com/document_detail/444715.html).
         self.support_auto_scaling = support_auto_scaling
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2040,44 +2092,23 @@
         endpoint_url: str = None,
         ip_whitelist: List[str] = None,
     ):
         # The type of the endpoint that is used to access the instance.
         # 
         # Valid values:
         # 
-        # *   TCP_VPC
-        # 
-        #     <!-- -->
-        # 
-        #     :
-        # 
-        #     <!-- -->
-        # 
-        #     VPC endpoint
-        # 
-        #     <!-- -->
-        # 
-        # *   TCP_INTERNET
-        # 
-        #     <!-- -->
-        # 
-        #     :
-        # 
-        #     <!-- -->
-        # 
-        #     public endpoint
-        # 
-        #     <!-- -->
+        # - TCP_VPC: VPC endpoint
+        # - TCP_INTERNET:public endpoint
         self.endpoint_type = endpoint_type
         # The endpoint that is used to access the instance.
         self.endpoint_url = endpoint_url
-        # The whitelist that includes the IP addresses that are allowed to access the ApsaraMQ for RocketMQ broker over the Internet. This parameter can be configured only if you use a public endpoint to access the ApsaraMQ for RocketMQ broker.
+        # The whitelist that includes the IP addresses that are allowed to access the ApsaraMQ for RocketMQ broker over the Internet. This parameter can be configured only if you use the public endpoint to access the instance.
         # 
-        # *   If this parameter is not configured, all IP addresses are allowed to access the ApsaraMQ for RocketMQ broker over the Internet.
-        # *   If this parameter is configured, only the IP addresses that are included in the whitelist can access the ApsaraMQ for RocketMQ broker over the Internet.
+        # *   If you do not configure an IP address whitelist, all CIDR blocks are allowed to access the ApsaraMQ for RocketMQ broker over the Internet.
+        # *   If you configure an IP address whitelist, only the IP addresses in the whitelist are allowed to access the ApsaraMQ for RocketMQ broker over the Internet.
         # 
         # We recommend that you configure internetInfo.ipWhitelist instead of this parameter.
         self.ip_whitelist = ip_whitelist
 
     def validate(self):
         pass
 
@@ -2126,15 +2157,15 @@
         # Specifies whether to enable the Internet access feature.
         # 
         # Valid values:
         # 
         # *   enable
         # *   disable
         # 
-        # By default, ApsaraMQ for RocketMQ instances are accessed in virtual private clouds (VPCs). If you enable the Internet access feature, you are charged for Internet outbound bandwidth. For more information, see [Internet access fee](~~427240~~).
+        # By default, ApsaraMQ for RocketMQ instances are accessed in virtual private clouds (VPCs). If you enable the Internet access feature, you are charged for Internet outbound bandwidth. For more information, see [Internet access fee](https://help.aliyun.com/document_detail/427240.html).
         self.internet_spec = internet_spec
         # The whitelist that includes the IP addresses that are allowed to access the ApsaraMQ for RocketMQ broker.
         # 
         # *   If this parameter is not configured, all IP addresses are allowed to access the ApsaraMQ for RocketMQ broker over the Internet.
         # *   If this parameter is configured, only the IP addresses that are included in the whitelist can access the ApsaraMQ for RocketMQ broker over the Internet.
         self.ip_whitelist = ip_whitelist
 
@@ -2166,51 +2197,98 @@
         if m.get('internetSpec') is not None:
             self.internet_spec = m.get('internetSpec')
         if m.get('ipWhitelist') is not None:
             self.ip_whitelist = m.get('ipWhitelist')
         return self
 
 
+class GetInstanceResponseBodyDataNetworkInfoVpcInfoVSwitches(TeaModel):
+    def __init__(
+        self,
+        v_switch_id: str = None,
+        zone_id: str = None,
+    ):
+        self.v_switch_id = v_switch_id
+        self.zone_id = zone_id
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
+        if self.v_switch_id is not None:
+            result['vSwitchId'] = self.v_switch_id
+        if self.zone_id is not None:
+            result['zoneId'] = self.zone_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('vSwitchId') is not None:
+            self.v_switch_id = m.get('vSwitchId')
+        if m.get('zoneId') is not None:
+            self.zone_id = m.get('zoneId')
+        return self
+
+
 class GetInstanceResponseBodyDataNetworkInfoVpcInfo(TeaModel):
     def __init__(
         self,
         security_group_ids: str = None,
         v_switch_id: str = None,
+        v_switches: List[GetInstanceResponseBodyDataNetworkInfoVpcInfoVSwitches] = None,
         vpc_id: str = None,
     ):
-        # The ID of the security group with which the instance is associated.
+        # The security group ID.
         self.security_group_ids = security_group_ids
         # The ID of the vSwitch with which the instance is associated.
         self.v_switch_id = v_switch_id
+        self.v_switches = v_switches
         # The ID of the VPC with which the instance is associated.
         self.vpc_id = vpc_id
 
     def validate(self):
-        pass
+        if self.v_switches:
+            for k in self.v_switches:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.security_group_ids is not None:
             result['securityGroupIds'] = self.security_group_ids
         if self.v_switch_id is not None:
             result['vSwitchId'] = self.v_switch_id
+        result['vSwitches'] = []
+        if self.v_switches is not None:
+            for k in self.v_switches:
+                result['vSwitches'].append(k.to_map() if k else None)
         if self.vpc_id is not None:
             result['vpcId'] = self.vpc_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('securityGroupIds') is not None:
             self.security_group_ids = m.get('securityGroupIds')
         if m.get('vSwitchId') is not None:
             self.v_switch_id = m.get('vSwitchId')
+        self.v_switches = []
+        if m.get('vSwitches') is not None:
+            for k in m.get('vSwitches'):
+                temp_model = GetInstanceResponseBodyDataNetworkInfoVpcInfoVSwitches()
+                self.v_switches.append(temp_model.from_map(k))
         if m.get('vpcId') is not None:
             self.vpc_id = m.get('vpcId')
         return self
 
 
 class GetInstanceResponseBodyDataNetworkInfo(TeaModel):
     def __init__(
@@ -2219,15 +2297,15 @@
         internet_info: GetInstanceResponseBodyDataNetworkInfoInternetInfo = None,
         vpc_info: GetInstanceResponseBodyDataNetworkInfoVpcInfo = None,
     ):
         # The information about endpoints.
         self.endpoints = endpoints
         # The information about the Internet.
         self.internet_info = internet_info
-        # The information about the VPC.
+        # The virtual private cloud (VPC) information.
         self.vpc_info = vpc_info
 
     def validate(self):
         if self.endpoints:
             for k in self.endpoints:
                 if k:
                     k.validate()
@@ -2285,34 +2363,39 @@
         # *   true: enable
         # *   false: disable
         # 
         # This parameter is valid only when the supportAutoScaling parameter is set to enable.
         self.auto_scaling = auto_scaling
         # The retention period of messages. Unit: hours.
         # 
-        # For information about the valid values of this parameter, see the "Limits on resource quotas" section in [Usage limits](~~440347~~).
+        # For information about the valid values of this parameter, see the "Limits on resource quotas" section in [Usage limits](https://help.aliyun.com/document_detail/440347.html).
         # 
-        # The storage of messages in ApsaraMQ for RocketMQ is serverless and scalable. You are charged for message storage based on your actual usage. You can change the retention period of messages to adjust storage capacity. For more information, see [Storage fee](~~427238~~).
+        # The storage of messages in ApsaraMQ for RocketMQ is serverless and scalable. You are charged for message storage based on your actual usage. You can change the retention period of messages to adjust storage capacity. For more information, see [Storage fee](https://help.aliyun.com/document_detail/427238.html).
         self.message_retention_time = message_retention_time
-        # The computing specification that is used to send and receive messages. For information about the upper limit of TPS, see [Instance specifications](~~444715~~).
+        # The computing specification that is used to send and receive messages. For information about the upper limit of TPS, see [Instance specifications](https://help.aliyun.com/document_detail/444715.html).
         self.msg_process_spec = msg_process_spec
         # The ratio between sent messages and received messages in the instance.
         self.send_receive_ratio = send_receive_ratio
         # Specifies whether to enable the elastic TPS feature for the instance.
         # 
         # Valid values:
         # 
         # *   true: enable
         # *   false: disable
         # 
-        # After you enable the elastic TPS feature for a ApsaraMQ for RocketMQ instance, you can use a specific amount of TPS that exceeds the specification limit. You are charged for the elastic TPS feature. For more information, see [Computing fee](~~427237~~).
+        # After you enable the elastic TPS feature for a ApsaraMQ for RocketMQ instance, you can use a specific amount of TPS that exceeds the specification limit. You are charged for the elastic TPS feature. For more information, see [Computing fee](https://help.aliyun.com/document_detail/427237.html).
         # 
-        # > The elastic TPS feature is supported by only specific instance editions. For more information, see [Instance specifications](~~444715~~).
+        # > The elastic TPS feature is supported by only specific instance editions. For more information, see [Instance specifications](https://help.aliyun.com/document_detail/444715.html).
         self.support_auto_scaling = support_auto_scaling
-        # Whether to enable tracking capability. Non-serverless instances are enabled by default, and serverless instances are optional for users.
+        # Indicates whether the message trace feature is enabled. Valid values:
+        # 
+        # *   true
+        # *   false
+        # 
+        # This parameter is not in use. By default, the message trace feature is enabled for ApsaraMQ for RocketMQ instances, regardless of whether this parameter is configured.
         self.trace_on = trace_on
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2474,23 +2557,23 @@
         self.bid = bid
         # The commodity code of the instance. The commodity code of a ApsaraMQ for RocketMQ 5.0 instance has a similar format as ons_rmqsub_public_cn.
         self.commodity_code = commodity_code
         # The time when the instance was created.
         self.create_time = create_time
         # The time when the instance expires.
         self.expire_time = expire_time
-        # The extended configurations. We recommend you configure the productInfo, internetInfo, or aclInfo parameter instead of this parameter.
+        # The extended configurations. We recommend you configure productInfo, internetInfo, or aclInfo instead of this parameter.
         self.ext_config = ext_config
         # The number of groups.
         self.group_count = group_count
         # The ID of the instance
         self.instance_id = instance_id
         # The name of the instance.
         self.instance_name = instance_name
-        # The quotas in the instance.
+        # The instance quotas.
         self.instance_quotas = instance_quotas
         # The network information.
         self.network_info = network_info
         # The billing method of the instance.
         # 
         # Valid values:
         # 
@@ -2503,15 +2586,15 @@
         self.region_id = region_id
         # The time when the instance was released.
         self.release_time = release_time
         # The description of the instance.
         self.remark = remark
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
-        # The primary edition of the instance. For information about the differences between primary edition instances, see [Instance selection](~~444722~~).
+        # The primary edition of the instance. For information about the differences between primary edition instances, see [Instance selection](https://help.aliyun.com/document_detail/444722.html).
         # 
         # Valid values:
         # 
         # *   standard: Standard Edition
         # *   ultimate: Enterprise Platinum Edition
         # *   professional: Professional Edition
         self.series_code = series_code
@@ -2527,15 +2610,15 @@
         # 
         # *   RELEASED
         # *   RUNNING
         # *   STOPPED
         # *   CHANGING
         # *   CREATING
         self.status = status
-        # The sub-category edition of the instance. For information about the differences between sub-category edition instances, see [Instance selection](~~444722~~).
+        # The sub-category edition of the instance. For information about the differences between sub-category edition instances, see [Instance selection](https://help.aliyun.com/document_detail/444722.html).
         # 
         # Valid values:
         # 
         # *   cluster_ha: Cluster High-availability Edition
         # *   single_node: Standalone Edition
         self.sub_series_code = sub_series_code
         # The resource tags.
@@ -3423,22 +3506,24 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListConsumerGroupSubscriptionsResponseBodyData(TeaModel):
     def __init__(
         self,
+        consistency: bool = None,
         consumer_group_id: str = None,
         filter_expression: str = None,
         filter_expression_type: str = None,
         message_model: str = None,
         subscription_status: str = None,
         topic_created: bool = None,
         topic_name: str = None,
     ):
+        self.consistency = consistency
         # The consumer group ID.
         self.consumer_group_id = consumer_group_id
         # The filter expression.
         self.filter_expression = filter_expression
         # The type of the filter expression. Valid values: SQL, TAG, and UNSPECIFIED.
         self.filter_expression_type = filter_expression_type
         # The consumption mode. Valid values: BROADCASTING and CLUSTERING.
@@ -3455,14 +3540,16 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.consistency is not None:
+            result['consistency'] = self.consistency
         if self.consumer_group_id is not None:
             result['consumerGroupId'] = self.consumer_group_id
         if self.filter_expression is not None:
             result['filterExpression'] = self.filter_expression
         if self.filter_expression_type is not None:
             result['filterExpressionType'] = self.filter_expression_type
         if self.message_model is not None:
@@ -3473,14 +3560,16 @@
             result['topicCreated'] = self.topic_created
         if self.topic_name is not None:
             result['topicName'] = self.topic_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('consistency') is not None:
+            self.consistency = m.get('consistency')
         if m.get('consumerGroupId') is not None:
             self.consumer_group_id = m.get('consumerGroupId')
         if m.get('filterExpression') is not None:
             self.filter_expression = m.get('filterExpression')
         if m.get('filterExpressionType') is not None:
             self.filter_expression_type = m.get('filterExpressionType')
         if m.get('messageModel') is not None:
@@ -3626,16 +3715,20 @@
         filter: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
         # The condition that you want to use to filter consumer groups in the instance. If you leave this parameter empty, all consumer groups in the instance are queried.
         self.filter = filter
         # The number of the page to return.
+        # 
+        # This parameter is required.
         self.page_number = page_number
         # The number of entries to return on each page.
+        # 
+        # This parameter is required.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3951,20 +4044,24 @@
         # The filter condition that is used to query instances. If you do not configure this parameter, all instances are queried.
         self.filter = filter
         # The number of the page to return.
         # 
         # Valid values: 1 to 100000000.
         # 
         # If the value that you specify for this parameter is less than 1, the system uses 1 as the value. If the value that you specify for this parameter is greater than 100000000, the system uses 100000000 as the value.
+        # 
+        # This parameter is required.
         self.page_number = page_number
         # The number of entries returned on each page.
         # 
         # Valid values: 10 to 200.
         # 
         # If the value that you specify for this parameter is less than 10, the system uses 10 as the value. If the value that you specify for this parameter is greater than 200, the system uses 200 as the value.
+        # 
+        # This parameter is required.
         self.page_size = page_size
         # The ID of the resource group to which the instance belongs.
         self.resource_group_id = resource_group_id
         # The tags that are used to filter instances.
         self.tags = tags
 
     def validate(self):
@@ -4667,21 +4764,23 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListTopicSubscriptionsResponseBodyData(TeaModel):
     def __init__(
         self,
+        consistency: str = None,
         consumer_group_id: str = None,
         filter_expression: str = None,
         filter_expression_type: str = None,
         message_model: str = None,
         subscription_status: str = None,
         topic_name: str = None,
     ):
+        self.consistency = consistency
         self.consumer_group_id = consumer_group_id
         self.filter_expression = filter_expression
         self.filter_expression_type = filter_expression_type
         self.message_model = message_model
         self.subscription_status = subscription_status
         self.topic_name = topic_name
 
@@ -4690,14 +4789,16 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.consistency is not None:
+            result['consistency'] = self.consistency
         if self.consumer_group_id is not None:
             result['consumerGroupId'] = self.consumer_group_id
         if self.filter_expression is not None:
             result['filterExpression'] = self.filter_expression
         if self.filter_expression_type is not None:
             result['filterExpressionType'] = self.filter_expression_type
         if self.message_model is not None:
@@ -4706,14 +4807,16 @@
             result['subscriptionStatus'] = self.subscription_status
         if self.topic_name is not None:
             result['topicName'] = self.topic_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('consistency') is not None:
+            self.consistency = m.get('consistency')
         if m.get('consumerGroupId') is not None:
             self.consumer_group_id = m.get('consumerGroupId')
         if m.get('filterExpression') is not None:
             self.filter_expression = m.get('filterExpression')
         if m.get('filterExpressionType') is not None:
             self.filter_expression_type = m.get('filterExpressionType')
         if m.get('messageModel') is not None:
@@ -5426,24 +5529,26 @@
         self,
         dead_letter_target_topic: str = None,
         max_retry_times: int = None,
         retry_policy: str = None,
     ):
         # The dead-letter topic.
         # 
-        # If a consumer still fails to consume a message after the message is retried for a specified number of times, the message is delivered to a dead-letter topic for subsequent business recovery or troubleshooting. For more information, see [Consumption retry and dead-letter messages](~~440356~~).
+        # If a consumer still fails to consume a message after the message is retried for a specified number of times, the message is delivered to a dead-letter topic for subsequent business recovery or troubleshooting. For more information, see [Consumption retry and dead-letter messages](https://help.aliyun.com/document_detail/440356.html).
         self.dead_letter_target_topic = dead_letter_target_topic
         # The maximum number of retries.
         self.max_retry_times = max_retry_times
-        # The retry policy. For more information, see [Message retry](~~440356~~).
+        # The retry policy. For more information, see [Message retry](https://help.aliyun.com/document_detail/440356.html).
         # 
         # Valid values:
         # 
         # *   FixedRetryPolicy: Failed messages are retried at a fixed interval.
         # *   DefaultRetryPolicy: Failed messages are retried at incremental intervals as the number of retries increases.
+        # 
+        # This parameter is required.
         self.retry_policy = retry_policy
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5473,22 +5578,26 @@
 class UpdateConsumerGroupRequest(TeaModel):
     def __init__(
         self,
         consume_retry_policy: UpdateConsumerGroupRequestConsumeRetryPolicy = None,
         delivery_order_type: str = None,
         remark: str = None,
     ):
-        # The new consumption retry policy that you want to configure for the consumer group. For more information, see [Consumption retry](~~440356~~).
+        # The new consumption retry policy that you want to configure for the consumer group. For more information, see [Consumption retry](https://help.aliyun.com/document_detail/440356.html).
+        # 
+        # This parameter is required.
         self.consume_retry_policy = consume_retry_policy
         # The new message delivery order of the consumer group.
         # 
         # Valid values:
         # 
         # *   Concurrently: concurrent delivery
         # *   Orderly: ordered delivery
+        # 
+        # This parameter is required.
         self.delivery_order_type = delivery_order_type
         # The new remarks on the consumer group.
         self.remark = remark
 
     def validate(self):
         if self.consume_retry_policy:
             self.consume_retry_policy.validate()
@@ -5639,15 +5748,21 @@
 
 class UpdateInstanceRequestAclInfo(TeaModel):
     def __init__(
         self,
         acl_types: List[str] = None,
         default_vpc_auth_free: bool = None,
     ):
+        # The authentication type of the instance.
         self.acl_types = acl_types
+        # Indicates whether the authentication-free in VPCs feature is enabled.
+        # Indicates whether the authentication-free in VPCs feature is enabled.
+        # Valid values:
+        # - true
+        # - false
         self.default_vpc_auth_free = default_vpc_auth_free
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5742,23 +5857,23 @@
         # Specifies whether to enable the elastic transactions per second (TPS) feature for the instance.
         # 
         # Valid values:
         # 
         # *   true
         # *   false
         # 
-        # After you enable the elastic TPS feature for an ApsaraMQ for RocketMQ instance, you can use a specific number of TPS that exceeds the specification limit. You are charged for using the elastic TPS feature. For more information, see [Computing fees](~~427237~~).
+        # After you enable the elastic TPS feature for an ApsaraMQ for RocketMQ instance, you can use a specific number of TPS that exceeds the specification limit. You are charged for using the elastic TPS feature. For more information, see [Computing fees](https://help.aliyun.com/document_detail/427237.html).
         # 
-        # >  The elastic TPS feature is supported only by specific instance editions. For more information, see [Instance editions](~~444715~~).
+        # >  The elastic TPS feature is supported only by specific instance editions. For more information, see [Instance editions](https://help.aliyun.com/document_detail/444715.html).
         self.auto_scaling = auto_scaling
         # The retention period of messages. Unit: hours.
         # 
-        # For information about the valid values of this parameter, see the "Limits on resource quotas" section of the [Limits](~~440347~~) topic.
+        # For information about the valid values of this parameter, see the "Limits on resource quotas" section of the [Limits](https://help.aliyun.com/document_detail/440347.html) topic.
         # 
-        # ApsaraMQ for RocketMQ supports serverless scaling of message storage. You are charged storage fees based on your actual storage usage. You can change the retention period of messages to manage storage capacity. For more information, see [Storage fees](~~427238~~).
+        # ApsaraMQ for RocketMQ supports serverless scaling of message storage. You are charged storage fees based on your actual storage usage. You can change the retention period of messages to manage storage capacity. For more information, see [Storage fees](https://help.aliyun.com/document_detail/427238.html).
         self.message_retention_time = message_retention_time
         # The ratio of the number of messages that you can send to the number of messages that you can receive on the instance.
         # 
         # Value values: 0.25 to 1.
         self.send_receive_ratio = send_receive_ratio
         # Specifies whether to enable the message trace feature.
         # 
@@ -5805,14 +5920,15 @@
         self,
         acl_info: UpdateInstanceRequestAclInfo = None,
         instance_name: str = None,
         network_info: UpdateInstanceRequestNetworkInfo = None,
         product_info: UpdateInstanceRequestProductInfo = None,
         remark: str = None,
     ):
+        # The access control list for the instance.
         self.acl_info = acl_info
         # The updated name of the instance.
         self.instance_name = instance_name
         # The updated network information about the instance.
         self.network_info = network_info
         # Additional configurations of the instance.
         self.product_info = product_info
```

### Comparing `alibabacloud_rocketmq20220801-1.4.1/alibabacloud_rocketmq20220801.egg-info/PKG-INFO` & `alibabacloud_rocketmq20220801-1.4.2/alibabacloud_rocketmq20220801.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rocketmq20220801
-Version: 1.4.1
+Version: 1.4.2
 Summary: Alibaba Cloud RocketMQ (20220801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rocketmq20220801-1.4.1/setup.py` & `alibabacloud_rocketmq20220801-1.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rocketmq20220801.
 
-Created on 29/03/2024
+Created on 28/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rocketmq20220801"
 NAME = "alibabacloud_rocketmq20220801" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud RocketMQ (20220801) SDK Library for Python"
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

