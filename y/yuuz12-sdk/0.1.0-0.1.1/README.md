# Comparing `tmp/yuuz12_sdk-0.1.0.tar.gz` & `tmp/yuuz12_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuuz12_sdk-0.1.0.tar", last modified: Tue May 28 13:04:48 2024, max compression
+gzip compressed data, was "yuuz12_sdk-0.1.1.tar", last modified: Tue May 28 13:32:52 2024, max compression
```

## Comparing `yuuz12_sdk-0.1.0.tar` & `yuuz12_sdk-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3018 2024-05-28 12:54:47.817399 yuuz12_sdk-0.1.0/README.md
--rw-r--r--   0        0        0      488 2024-05-28 13:04:48.799063 yuuz12_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       91 2024-05-28 12:47:52.090898 yuuz12_sdk-0.1.0/src/yuuz12_sdk/__init__.py
--rw-r--r--   0        0        0      223 2024-05-21 14:00:01.255203 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/__init__.py
--rw-r--r--   0        0        0     3124 2024-05-28 12:47:52.066469 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/_api.py
--rw-r--r--   0        0        0      302 2024-05-12 11:04:19.794367 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/baidu.py
--rw-r--r--   0        0        0      300 2024-05-10 04:49:42.229331 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/baidu.pyi
--rw-r--r--   0        0        0      275 2024-05-09 19:10:31.000000 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/bangumi.py
--rw-r--r--   0        0        0      287 2024-05-10 04:49:43.382950 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/bangumi.pyi
--rw-r--r--   0        0        0      263 2024-05-09 19:03:41.000000 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/cave.py
--rw-r--r--   0        0        0      889 2024-05-21 11:35:37.649122 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/cave.pyi
--rw-r--r--   0        0        0      237 2024-05-09 19:23:39.000000 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/email.py
--rw-r--r--   0        0        0      425 2024-05-10 07:03:45.835018 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/email.pyi
--rw-r--r--   0        0        0      456 2024-05-21 13:47:24.035280 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/invitation.py
--rw-r--r--   0        0        0      402 2024-05-10 07:11:34.636312 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/invitation.pyi
--rw-r--r--   0        0        0      820 2024-05-09 19:23:39.000000 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/minecraft.py
--rw-r--r--   0        0        0     1290 2024-05-10 08:23:01.614940 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/minecraft.pyi
--rw-r--r--   0        0        0      266 2024-05-09 19:16:12.000000 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/prize.py
--rw-r--r--   0        0        0      511 2024-05-10 04:49:54.033919 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/prize.pyi
--rw-r--r--   0        0        0      287 2024-05-09 19:06:37.000000 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/statistics.py
--rw-r--r--   0        0        0      311 2024-05-10 04:49:55.512140 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/statistics.pyi
--rw-r--r--   0        0        0      496 2024-05-09 18:22:36.000000 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/user.py
--rw-r--r--   0        0        0     3141 2024-05-21 11:34:20.747172 yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/user.pyi
--rw-r--r--   0        0        0     1369 2024-05-09 17:20:46.000000 yuuz12_sdk-0.1.0/src/yuuz12_sdk/exceptions.py
--rw-r--r--   0        0        0      213 2024-05-10 02:56:01.633792 yuuz12_sdk-0.1.0/src/yuuz12_sdk/log.py
--rw-r--r--   0        0        0       19 2024-05-09 19:56:14.000000 yuuz12_sdk-0.1.0/src/yuuz12_sdk/models/__init__.py
--rw-r--r--   0        0        0      604 2024-05-15 06:57:19.308450 yuuz12_sdk-0.1.0/src/yuuz12_sdk/models/user.py
--rw-r--r--   0        0        0        0 2024-05-28 12:45:40.681447 yuuz12_sdk-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 yuuz12_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3018 2024-05-28 13:27:39.736032 yuuz12_sdk-0.1.1/README.md
+-rw-r--r--   0        0        0      779 2024-05-28 13:32:52.410910 yuuz12_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-05-28 12:47:52.090898 yuuz12_sdk-0.1.1/src/yuuz12_sdk/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-21 14:00:01.255203 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/__init__.py
+-rw-r--r--   0        0        0     3124 2024-05-28 12:47:52.066469 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/_api.py
+-rw-r--r--   0        0        0      302 2024-05-12 11:04:19.794367 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/baidu.py
+-rw-r--r--   0        0        0      300 2024-05-10 04:49:42.229331 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/baidu.pyi
+-rw-r--r--   0        0        0      275 2024-05-09 19:10:31.000000 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/bangumi.py
+-rw-r--r--   0        0        0      287 2024-05-10 04:49:43.382950 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/bangumi.pyi
+-rw-r--r--   0        0        0      263 2024-05-09 19:03:41.000000 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/cave.py
+-rw-r--r--   0        0        0      889 2024-05-21 11:35:37.649122 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/cave.pyi
+-rw-r--r--   0        0        0      237 2024-05-09 19:23:39.000000 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/email.py
+-rw-r--r--   0        0        0      425 2024-05-10 07:03:45.835018 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/email.pyi
+-rw-r--r--   0        0        0      456 2024-05-21 13:47:24.035280 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/invitation.py
+-rw-r--r--   0        0        0      402 2024-05-10 07:11:34.636312 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/invitation.pyi
+-rw-r--r--   0        0        0      820 2024-05-09 19:23:39.000000 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/minecraft.py
+-rw-r--r--   0        0        0     1290 2024-05-10 08:23:01.614940 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/minecraft.pyi
+-rw-r--r--   0        0        0      266 2024-05-09 19:16:12.000000 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/prize.py
+-rw-r--r--   0        0        0      511 2024-05-10 04:49:54.033919 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/prize.pyi
+-rw-r--r--   0        0        0      287 2024-05-09 19:06:37.000000 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/statistics.py
+-rw-r--r--   0        0        0      311 2024-05-10 04:49:55.512140 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/statistics.pyi
+-rw-r--r--   0        0        0      496 2024-05-09 18:22:36.000000 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/user.py
+-rw-r--r--   0        0        0     3141 2024-05-21 11:34:20.747172 yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/user.pyi
+-rw-r--r--   0        0        0     1369 2024-05-09 17:20:46.000000 yuuz12_sdk-0.1.1/src/yuuz12_sdk/exceptions.py
+-rw-r--r--   0        0        0      213 2024-05-10 02:56:01.633792 yuuz12_sdk-0.1.1/src/yuuz12_sdk/log.py
+-rw-r--r--   0        0        0       19 2024-05-09 19:56:14.000000 yuuz12_sdk-0.1.1/src/yuuz12_sdk/models/__init__.py
+-rw-r--r--   0        0        0      604 2024-05-15 06:57:19.308450 yuuz12_sdk-0.1.1/src/yuuz12_sdk/models/user.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:45:40.681447 yuuz12_sdk-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 yuuz12_sdk-0.1.1/PKG-INFO
```

### Comparing `yuuz12_sdk-0.1.0/README.md` & `yuuz12_sdk-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 ```
 4. 使用示例:
 
 ```python
 """调用随机选择回声洞中回声信息"""
 import asyncio
 import httpx
-from yuuz12_lib.apis import Cave
+from yuuz12_sdk.apis import Cave
 
 
 async def main():
     async with httpx.AsyncClient() as client:
         cave = Cave(client)
         await cave.get_cave()
         
@@ -80,16 +80,16 @@
     asyncio.run(main())
 ```
 
 ```python
 """获取签到图片"""
 import asyncio
 import httpx
-from yuuz12_lib.apis import UserCheck
-from yuuz12_lib.models import UserModel
+from yuuz12_sdk.apis import UserCheck
+from yuuz12_sdk.models import UserModel
 
 async def main():
     async with httpx.AsyncClient() as client:
         check = UserCheck(client)
         await check.get(qq=1234567, favorability=1, coin=5)
     
     image_binary: bytes = check.raw
```

### Comparing `yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/_api.py` & `yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/_api.py`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/cave.pyi` & `yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/cave.pyi`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/minecraft.py` & `yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/minecraft.py`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/minecraft.pyi` & `yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/minecraft.pyi`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.0/src/yuuz12_sdk/apis/user.pyi` & `yuuz12_sdk-0.1.1/src/yuuz12_sdk/apis/user.pyi`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.0/src/yuuz12_sdk/exceptions.py` & `yuuz12_sdk-0.1.1/src/yuuz12_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.0/src/yuuz12_sdk/models/user.py` & `yuuz12_sdk-0.1.1/src/yuuz12_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.0/PKG-INFO` & `yuuz12_sdk-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuuz12-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python 3 SDK for Yuuz12-Api. Check https://doc.yuuz12.top/web/#/5/23 
 Author-Email: Number_Sir <number_sir@126.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: python-dotenv>=1.0.1
 Requires-Dist: httpx>=0.27.0
@@ -71,15 +71,15 @@
 ```
 4. 使用示例:
 
 ```python
 """调用随机选择回声洞中回声信息"""
 import asyncio
 import httpx
-from yuuz12_lib.apis import Cave
+from yuuz12_sdk.apis import Cave
 
 
 async def main():
     async with httpx.AsyncClient() as client:
         cave = Cave(client)
         await cave.get_cave()
         
@@ -92,16 +92,16 @@
     asyncio.run(main())
 ```
 
 ```python
 """获取签到图片"""
 import asyncio
 import httpx
-from yuuz12_lib.apis import UserCheck
-from yuuz12_lib.models import UserModel
+from yuuz12_sdk.apis import UserCheck
+from yuuz12_sdk.models import UserModel
 
 async def main():
     async with httpx.AsyncClient() as client:
         check = UserCheck(client)
         await check.get(qq=1234567, favorability=1, coin=5)
     
     image_binary: bytes = check.raw
```

