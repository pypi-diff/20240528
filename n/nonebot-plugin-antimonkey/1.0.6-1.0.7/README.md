# Comparing `tmp/nonebot_plugin_antimonkey-1.0.6.tar.gz` & `tmp/nonebot_plugin_antimonkey-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_antimonkey-1.0.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_antimonkey-1.0.7.tar", max compression
```

## Comparing `nonebot_plugin_antimonkey-1.0.6.tar` & `nonebot_plugin_antimonkey-1.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1086 2024-05-28 08:29:56.094426 nonebot_plugin_antimonkey-1.0.6/LICENSE
--rw-r--r--   0        0        0      471 2023-12-26 11:41:19.771085 nonebot_plugin_antimonkey-1.0.6/nonebot_plugin_antimonkey/__init__.py
--rw-r--r--   0        0        0      114 2023-12-26 09:19:29.657612 nonebot_plugin_antimonkey-1.0.6/nonebot_plugin_antimonkey/config.py
--rw-r--r--   0        0        0     4193 2024-05-28 09:59:00.753530 nonebot_plugin_antimonkey-1.0.6/nonebot_plugin_antimonkey/malou.py
--rw-r--r--   0        0        0    34885 2023-12-26 10:03:29.933870 nonebot_plugin_antimonkey-1.0.6/nonebot_plugin_antimonkey/monkey_test.jpg
--rw-r--r--   0        0        0      878 2024-05-28 10:01:29.172092 nonebot_plugin_antimonkey-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     2020 2024-05-28 08:43:07.239159 nonebot_plugin_antimonkey-1.0.6/README.md
--rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 nonebot_plugin_antimonkey-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-28 08:29:56.094426 nonebot_plugin_antimonkey-1.0.7/LICENSE
+-rw-r--r--   0        0        0      493 2024-05-28 10:17:49.209115 nonebot_plugin_antimonkey-1.0.7/nonebot_plugin_antimonkey/__init__.py
+-rw-r--r--   0        0        0      114 2023-12-26 09:19:29.657612 nonebot_plugin_antimonkey-1.0.7/nonebot_plugin_antimonkey/config.py
+-rw-r--r--   0        0        0     4171 2024-05-28 10:15:17.978973 nonebot_plugin_antimonkey-1.0.7/nonebot_plugin_antimonkey/malou.py
+-rw-r--r--   0        0        0    34885 2023-12-26 10:03:29.933870 nonebot_plugin_antimonkey-1.0.7/nonebot_plugin_antimonkey/monkey_test.jpg
+-rw-r--r--   0        0        0      878 2024-05-28 10:18:55.676547 nonebot_plugin_antimonkey-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2020 2024-05-28 08:43:07.239159 nonebot_plugin_antimonkey-1.0.7/README.md
+-rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 nonebot_plugin_antimonkey-1.0.7/PKG-INFO
```

### Comparing `nonebot_plugin_antimonkey-1.0.6/LICENSE` & `nonebot_plugin_antimonkey-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.6/nonebot_plugin_antimonkey/malou.py` & `nonebot_plugin_antimonkey-1.0.7/nonebot_plugin_antimonkey/malou.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import cv2
 from keras.src.applications import imagenet_utils
 from nonebot import on_message, require
 from nonebot.rule import Rule
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent
 import aiohttp
 
-# 配置日志记录
 logging.basicConfig(level=logging.DEBUG)
 logger = logging.getLogger(__name__)
 
 logger.info("Loading MobileNetV2 model...")
 # MobileNetV2模型
 model = MobileNetV2(weights="imagenet")
```

### Comparing `nonebot_plugin_antimonkey-1.0.6/nonebot_plugin_antimonkey/monkey_test.jpg` & `nonebot_plugin_antimonkey-1.0.7/nonebot_plugin_antimonkey/monkey_test.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.6/pyproject.toml` & `nonebot_plugin_antimonkey-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-antimonkey"
-version = "1.0.6"
+version = "1.0.7"
 description = "一个用于自动检测和撤回包含猴子图片的QQ机器人插件。"
 authors = ["phquathi <yangziqi233@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/phquathi/nonebot_plugin_antimonkey"
 repository = "https://github.com/phquathi/nonebot_plugin_antimonkey"
 keywords = ["nonebot", "plugin", "antimonkey"]
```

### Comparing `nonebot_plugin_antimonkey-1.0.6/README.md` & `nonebot_plugin_antimonkey-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.6/PKG-INFO` & `nonebot_plugin_antimonkey-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-antimonkey
-Version: 1.0.6
+Version: 1.0.7
 Summary: 一个用于自动检测和撤回包含猴子图片的QQ机器人插件。
 Home-page: https://github.com/phquathi/nonebot_plugin_antimonkey
 Keywords: nonebot,plugin,antimonkey
 Author: phquathi
 Author-email: yangziqi233@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
```
