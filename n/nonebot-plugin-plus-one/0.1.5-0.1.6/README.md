# Comparing `tmp/nonebot_plugin_plus_one-0.1.5.tar.gz` & `tmp/nonebot_plugin_plus_one-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_plus_one-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_plus_one-0.1.6.tar", max compression
```

## Comparing `nonebot_plugin_plus_one-0.1.5.tar` & `nonebot_plugin_plus_one-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      629 2024-05-27 03:13:44.802874 nonebot_plugin_plus_one-0.1.5/nonebot_plugin_plus_one/__init__.py
--rw-r--r--   0        0        0      312 2024-05-24 03:08:41.722147 nonebot_plugin_plus_one-0.1.5/nonebot_plugin_plus_one/config.py
--rw-r--r--   0        0        0     1362 2024-05-27 03:25:12.294956 nonebot_plugin_plus_one-0.1.5/nonebot_plugin_plus_one/handler.py
--rw-r--r--   0        0        0      700 2024-05-27 03:26:16.876294 nonebot_plugin_plus_one-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1561 2024-05-27 03:24:57.326616 nonebot_plugin_plus_one-0.1.5/README.md
--rw-r--r--   0        0        0     2483 1970-01-01 00:00:00.000000 nonebot_plugin_plus_one-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      629 2024-05-27 03:13:44.802874 nonebot_plugin_plus_one-0.1.6/nonebot_plugin_plus_one/__init__.py
+-rw-r--r--   0        0        0      312 2024-05-24 03:08:41.722147 nonebot_plugin_plus_one-0.1.6/nonebot_plugin_plus_one/config.py
+-rw-r--r--   0        0        0     1362 2024-05-27 03:25:12.294956 nonebot_plugin_plus_one-0.1.6/nonebot_plugin_plus_one/handler.py
+-rw-r--r--   0        0        0      700 2024-05-28 02:42:33.137040 nonebot_plugin_plus_one-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1561 2024-05-27 03:24:57.326616 nonebot_plugin_plus_one-0.1.6/README.md
+-rw-r--r--   0        0        0     2483 1970-01-01 00:00:00.000000 nonebot_plugin_plus_one-0.1.6/PKG-INFO
```

### Comparing `nonebot_plugin_plus_one-0.1.5/nonebot_plugin_plus_one/__init__.py` & `nonebot_plugin_plus_one-0.1.6/nonebot_plugin_plus_one/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_plus_one-0.1.5/nonebot_plugin_plus_one/handler.py` & `nonebot_plugin_plus_one-0.1.6/nonebot_plugin_plus_one/handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_plus_one-0.1.5/pyproject.toml` & `nonebot_plugin_plus_one-0.1.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-plus-one"
-version = "0.1.5"
+version = "0.1.6"
 description = "全新复读姬，支持文本、图片、表情甚至是转发分享卡片复读，任意群聊触发 +1，姬就 +1。轻巧、专注，不使用任何数据库，不使用任何文件存储"
 authors = ["yejue <1145331931@qq.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nonebot_plugin_plus_one-0.1.5/README.md` & `nonebot_plugin_plus_one-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_plus_one-0.1.5/PKG-INFO` & `nonebot_plugin_plus_one-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-plus-one
-Version: 0.1.5
+Version: 0.1.6
 Summary: 全新复读姬，支持文本、图片、表情甚至是转发分享卡片复读，任意群聊触发 +1，姬就 +1。轻巧、专注，不使用任何数据库，不使用任何文件存储
 License: MIT
 Author: yejue
 Author-email: 1145331931@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-plus-one Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-plus-one Version: 0.1.6 Summary:
 å¨æ°å¤è¯»å§¬ï¼æ¯æææ¬ãå¾çãè¡¨æçè³æ¯è½¬ååäº«å¡çå¤è¯»ï¼ä»»æç¾¤èè§¦å
 +1ï¼å§¬å°±
 +1ãè½»å·§ãä¸æ³¨ï¼ä¸ä½¿ç¨ä»»ä½æ°æ®åºï¼ä¸ä½¿ç¨ä»»ä½æä»¶å­å¨
 License: MIT Author: yejue Author-email: 1145331931@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

