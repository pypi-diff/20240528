# Comparing `tmp/nonebot_plugin_plus_one-0.1.7.tar.gz` & `tmp/nonebot_plugin_plus_one-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_plus_one-0.1.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_plus_one-0.1.9.tar", max compression
```

## Comparing `nonebot_plugin_plus_one-0.1.7.tar` & `nonebot_plugin_plus_one-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      629 2024-05-27 03:13:44.802874 nonebot_plugin_plus_one-0.1.7/nonebot_plugin_plus_one/__init__.py
--rw-r--r--   0        0        0      312 2024-05-24 03:08:41.722147 nonebot_plugin_plus_one-0.1.7/nonebot_plugin_plus_one/config.py
--rw-r--r--   0        0        0     1362 2024-05-27 03:25:12.294956 nonebot_plugin_plus_one-0.1.7/nonebot_plugin_plus_one/handler.py
--rw-r--r--   0        0        0      700 2024-05-28 02:50:00.511551 nonebot_plugin_plus_one-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1561 2024-05-27 03:24:57.326616 nonebot_plugin_plus_one-0.1.7/README.md
--rw-r--r--   0        0        0     2483 1970-01-01 00:00:00.000000 nonebot_plugin_plus_one-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      814 2024-05-28 14:49:28.876266 nonebot_plugin_plus_one-0.1.9/nonebot_plugin_plus_one/__init__.py
+-rw-r--r--   0        0        0      312 2024-05-24 03:08:41.722147 nonebot_plugin_plus_one-0.1.9/nonebot_plugin_plus_one/config.py
+-rw-r--r--   0        0        0     1362 2024-05-27 03:25:12.294956 nonebot_plugin_plus_one-0.1.9/nonebot_plugin_plus_one/handler.py
+-rw-r--r--   0        0        0      700 2024-05-28 14:50:00.370709 nonebot_plugin_plus_one-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1561 2024-05-27 03:24:57.326616 nonebot_plugin_plus_one-0.1.9/README.md
+-rw-r--r--   0        0        0     2483 1970-01-01 00:00:00.000000 nonebot_plugin_plus_one-0.1.9/PKG-INFO
```

### Comparing `nonebot_plugin_plus_one-0.1.7/nonebot_plugin_plus_one/__init__.py` & `nonebot_plugin_plus_one-0.1.9/nonebot_plugin_plus_one/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-from nonebot.plugin import PluginMetadata
+from nonebot.plugin import PluginMetadata, inherit_supported_adapters
 from nonebot import require
 
 require("nonebot_plugin_session")
 
 from .config import Config
 from .handler import plus
 
+inherit_set = inherit_supported_adapters("nonebot_plugin_session")
+if not inherit_set:
+    inherit_set = set()
+
+
 __plugin_meta__ = PluginMetadata(
     name="复读姬+1 PlusOne",
     description="全新复读姬，支持文本、图片、表情甚至是转发分享卡片复读，任意群聊触发 +1，姬就 +1。\n"
                 "轻巧、专注，不使用任何数据库，不使用任何文件存储\n",
     usage="复读姬，任意群聊触发 +1，姬就 +1",
     config=Config,
     homepage="https://github.com/yejue/nonebot-plugin-plus-one",
-    type="application"
+    type="application",
+    supported_adapters=set() | inherit_set
 )
```

### Comparing `nonebot_plugin_plus_one-0.1.7/nonebot_plugin_plus_one/handler.py` & `nonebot_plugin_plus_one-0.1.9/nonebot_plugin_plus_one/handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_plus_one-0.1.7/pyproject.toml` & `nonebot_plugin_plus_one-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-plus-one"
-version = "0.1.7"
+version = "0.1.9"
 description = "全新复读姬，支持文本、图片、表情甚至是转发分享卡片复读，任意群聊触发 +1，姬就 +1。轻巧、专注，不使用任何数据库，不使用任何文件存储"
 authors = ["yejue <1145331931@qq.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nonebot_plugin_plus_one-0.1.7/README.md` & `nonebot_plugin_plus_one-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_plus_one-0.1.7/PKG-INFO` & `nonebot_plugin_plus_one-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-plus-one
-Version: 0.1.7
+Version: 0.1.9
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
-Metadata-Version: 2.1 Name: nonebot-plugin-plus-one Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-plus-one Version: 0.1.9 Summary:
 å¨æ°å¤è¯»å§¬ï¼æ¯æææ¬ãå¾çãè¡¨æçè³æ¯è½¬ååäº«å¡çå¤è¯»ï¼ä»»æç¾¤èè§¦å
 +1ï¼å§¬å°±
 +1ãè½»å·§ãä¸æ³¨ï¼ä¸ä½¿ç¨ä»»ä½æ°æ®åºï¼ä¸ä½¿ç¨ä»»ä½æä»¶å­å¨
 License: MIT Author: yejue Author-email: 1145331931@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

