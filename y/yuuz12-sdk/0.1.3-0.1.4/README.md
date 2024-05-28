# Comparing `tmp/yuuz12_sdk-0.1.3.tar.gz` & `tmp/yuuz12_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuuz12_sdk-0.1.3.tar", last modified: Tue May 28 13:58:09 2024, max compression
+gzip compressed data, was "yuuz12_sdk-0.1.4.tar", last modified: Tue May 28 17:17:48 2024, max compression
```

## Comparing `yuuz12_sdk-0.1.3.tar` & `yuuz12_sdk-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3201 2024-05-28 13:51:30.959424 yuuz12_sdk-0.1.3/README.md
--rw-r--r--   0        0        0      738 2024-05-28 13:58:09.284691 yuuz12_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       91 2024-05-28 12:47:52.090898 yuuz12_sdk-0.1.3/src/yuuz12_sdk/__init__.py
--rw-r--r--   0        0        0      223 2024-05-21 14:00:01.255203 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/__init__.py
--rw-r--r--   0        0        0     3124 2024-05-28 12:47:52.066469 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/_api.py
--rw-r--r--   0        0        0      302 2024-05-12 11:04:19.794367 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/baidu.py
--rw-r--r--   0        0        0      300 2024-05-10 04:49:42.229331 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/baidu.pyi
--rw-r--r--   0        0        0      275 2024-05-09 19:10:31.000000 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/bangumi.py
--rw-r--r--   0        0        0      287 2024-05-10 04:49:43.382950 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/bangumi.pyi
--rw-r--r--   0        0        0      263 2024-05-09 19:03:41.000000 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/cave.py
--rw-r--r--   0        0        0      889 2024-05-21 11:35:37.649122 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/cave.pyi
--rw-r--r--   0        0        0      237 2024-05-09 19:23:39.000000 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/email.py
--rw-r--r--   0        0        0      425 2024-05-10 07:03:45.835018 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/email.pyi
--rw-r--r--   0        0        0      456 2024-05-21 13:47:24.035280 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/invitation.py
--rw-r--r--   0        0        0      402 2024-05-10 07:11:34.636312 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/invitation.pyi
--rw-r--r--   0        0        0      820 2024-05-09 19:23:39.000000 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/minecraft.py
--rw-r--r--   0        0        0     1290 2024-05-10 08:23:01.614940 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/minecraft.pyi
--rw-r--r--   0        0        0      266 2024-05-09 19:16:12.000000 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/prize.py
--rw-r--r--   0        0        0      511 2024-05-10 04:49:54.033919 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/prize.pyi
--rw-r--r--   0        0        0      287 2024-05-09 19:06:37.000000 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/statistics.py
--rw-r--r--   0        0        0      311 2024-05-10 04:49:55.512140 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/statistics.pyi
--rw-r--r--   0        0        0      496 2024-05-09 18:22:36.000000 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/user.py
--rw-r--r--   0        0        0     3141 2024-05-21 11:34:20.747172 yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/user.pyi
--rw-r--r--   0        0        0     1369 2024-05-09 17:20:46.000000 yuuz12_sdk-0.1.3/src/yuuz12_sdk/exceptions.py
--rw-r--r--   0        0        0      213 2024-05-10 02:56:01.633792 yuuz12_sdk-0.1.3/src/yuuz12_sdk/log.py
--rw-r--r--   0        0        0       19 2024-05-09 19:56:14.000000 yuuz12_sdk-0.1.3/src/yuuz12_sdk/models/__init__.py
--rw-r--r--   0        0        0      604 2024-05-15 06:57:19.308450 yuuz12_sdk-0.1.3/src/yuuz12_sdk/models/user.py
--rw-r--r--   0        0        0        0 2024-05-28 12:45:40.681447 yuuz12_sdk-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 yuuz12_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3198 2024-05-28 17:16:16.920272 yuuz12_sdk-0.1.4/README.md
+-rw-r--r--   0        0        0      738 2024-05-28 17:17:48.673454 yuuz12_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-05-28 12:47:52.090898 yuuz12_sdk-0.1.4/src/yuuz12_sdk/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-21 14:00:01.255203 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/__init__.py
+-rw-r--r--   0        0        0     3122 2024-05-28 17:16:16.897529 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/_api.py
+-rw-r--r--   0        0        0      302 2024-05-12 11:04:19.794367 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/baidu.py
+-rw-r--r--   0        0        0      300 2024-05-10 04:49:42.229331 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/baidu.pyi
+-rw-r--r--   0        0        0      275 2024-05-09 19:10:31.000000 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/bangumi.py
+-rw-r--r--   0        0        0      287 2024-05-10 04:49:43.382950 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/bangumi.pyi
+-rw-r--r--   0        0        0      263 2024-05-09 19:03:41.000000 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/cave.py
+-rw-r--r--   0        0        0      889 2024-05-21 11:35:37.649122 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/cave.pyi
+-rw-r--r--   0        0        0      237 2024-05-09 19:23:39.000000 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/email.py
+-rw-r--r--   0        0        0      425 2024-05-10 07:03:45.835018 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/email.pyi
+-rw-r--r--   0        0        0      456 2024-05-21 13:47:24.035280 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/invitation.py
+-rw-r--r--   0        0        0      402 2024-05-10 07:11:34.636312 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/invitation.pyi
+-rw-r--r--   0        0        0      820 2024-05-09 19:23:39.000000 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/minecraft.py
+-rw-r--r--   0        0        0     1290 2024-05-10 08:23:01.614940 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/minecraft.pyi
+-rw-r--r--   0        0        0      266 2024-05-09 19:16:12.000000 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/prize.py
+-rw-r--r--   0        0        0      511 2024-05-10 04:49:54.033919 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/prize.pyi
+-rw-r--r--   0        0        0      287 2024-05-09 19:06:37.000000 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/statistics.py
+-rw-r--r--   0        0        0      311 2024-05-10 04:49:55.512140 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/statistics.pyi
+-rw-r--r--   0        0        0      496 2024-05-09 18:22:36.000000 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/user.py
+-rw-r--r--   0        0        0     3141 2024-05-21 11:34:20.747172 yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/user.pyi
+-rw-r--r--   0        0        0     1369 2024-05-09 17:20:46.000000 yuuz12_sdk-0.1.4/src/yuuz12_sdk/exceptions.py
+-rw-r--r--   0        0        0      213 2024-05-10 02:56:01.633792 yuuz12_sdk-0.1.4/src/yuuz12_sdk/log.py
+-rw-r--r--   0        0        0       19 2024-05-09 19:56:14.000000 yuuz12_sdk-0.1.4/src/yuuz12_sdk/models/__init__.py
+-rw-r--r--   0        0        0      604 2024-05-15 06:57:19.308450 yuuz12_sdk-0.1.4/src/yuuz12_sdk/models/user.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:45:40.681447 yuuz12_sdk-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     3652 1970-01-01 00:00:00.000000 yuuz12_sdk-0.1.4/PKG-INFO
```

### Comparing `yuuz12_sdk-0.1.3/README.md` & `yuuz12_sdk-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Yuuz12-Api
-> 文档地址: https://doc.yuuz12.top/web/#/5/103
+> 文档地址: https://doc.yuuz12.top/web/#/5/
 > 
 > PYPI 地址: https://pypi.org/project/yuuz12-sdk
 > 
 > GitHub 仓库: https://github.com/NumberSir/yuuz12-sdk
 
 ## 简介
 全异步编写，可调用 Yuuz12-Api。需要 Python 3.11+
```

### Comparing `yuuz12_sdk-0.1.3/pyproject.toml` & `yuuz12_sdk-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yuuz12-sdk"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python 3 SDK for Yuuz12-Api. Check https://doc.yuuz12.top/web/#/5/23 "
 authors = [
     { name = "Number_Sir", email = "number_sir@126.com" },
 ]
 maintainers = [
     { name = "Number_Sir", email = "number_sir@126.com" },
 ]
```

### Comparing `yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/_api.py` & `yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""https://doc.yuuz12.top/web/#/5/23"""
+"""https://doc.yuuz12.top/web/#/5/"""
 from json import JSONDecodeError
 
 import httpx
 import os
 from dotenv import load_dotenv
 
 from ..log import logger
```

### Comparing `yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/cave.pyi` & `yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/cave.pyi`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/minecraft.py` & `yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/minecraft.py`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/minecraft.pyi` & `yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/minecraft.pyi`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.3/src/yuuz12_sdk/apis/user.pyi` & `yuuz12_sdk-0.1.4/src/yuuz12_sdk/apis/user.pyi`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.3/src/yuuz12_sdk/exceptions.py` & `yuuz12_sdk-0.1.4/src/yuuz12_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.3/src/yuuz12_sdk/models/user.py` & `yuuz12_sdk-0.1.4/src/yuuz12_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `yuuz12_sdk-0.1.3/PKG-INFO` & `yuuz12_sdk-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: yuuz12-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python 3 SDK for Yuuz12-Api. Check https://doc.yuuz12.top/web/#/5/23 
 Keywords: yuuz12,shiruku
 Author-Email: Number_Sir <number_sir@126.com>
 Maintainer-Email: Number_Sir <number_sir@126.com>
 License: MIT
 Project-URL: Repository, https://github.com/NumberSir/yuuz12-sdk
 Project-URL: Issues, https://github.com/NumberSir/yuuz12-sdk/issues
 Requires-Python: >=3.11
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: python-dotenv>=1.0.1
 Requires-Dist: httpx>=0.27.0
 Description-Content-Type: text/markdown
 
 # Yuuz12-Api
-> 文档地址: https://doc.yuuz12.top/web/#/5/103
+> 文档地址: https://doc.yuuz12.top/web/#/5/
 > 
 > PYPI 地址: https://pypi.org/project/yuuz12-sdk
 > 
 > GitHub 仓库: https://github.com/NumberSir/yuuz12-sdk
 
 ## 简介
 全异步编写，可调用 Yuuz12-Api。需要 Python 3.11+
```

