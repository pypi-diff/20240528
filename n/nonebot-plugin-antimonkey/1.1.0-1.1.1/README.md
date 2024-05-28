# Comparing `tmp/nonebot_plugin_antimonkey-1.1.0.tar.gz` & `tmp/nonebot_plugin_antimonkey-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_antimonkey-1.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_antimonkey-1.1.1.tar", max compression
```

## Comparing `nonebot_plugin_antimonkey-1.1.0.tar` & `nonebot_plugin_antimonkey-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1086 2024-05-28 08:29:56.094426 nonebot_plugin_antimonkey-1.1.0/LICENSE
--rw-r--r--   0        0        0      357 2024-05-28 10:41:25.751059 nonebot_plugin_antimonkey-1.1.0/nonebot_plugin_antimonkey/__init__.py
--rw-r--r--   0        0        0      114 2023-12-26 09:19:29.657612 nonebot_plugin_antimonkey-1.1.0/nonebot_plugin_antimonkey/config.py
--rw-r--r--   0        0        0     3398 2024-05-28 10:32:53.131902 nonebot_plugin_antimonkey-1.1.0/nonebot_plugin_antimonkey/malou.py
--rw-r--r--   0        0        0    34885 2023-12-26 10:03:29.933870 nonebot_plugin_antimonkey-1.1.0/nonebot_plugin_antimonkey/monkey_test.jpg
--rw-r--r--   0        0        0      878 2024-05-28 10:41:25.755264 nonebot_plugin_antimonkey-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2020 2024-05-28 08:43:07.239159 nonebot_plugin_antimonkey-1.1.0/README.md
--rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 nonebot_plugin_antimonkey-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-28 08:29:56.094426 nonebot_plugin_antimonkey-1.1.1/LICENSE
+-rw-r--r--   0        0        0      357 2024-05-28 10:41:25.751059 nonebot_plugin_antimonkey-1.1.1/nonebot_plugin_antimonkey/__init__.py
+-rw-r--r--   0        0        0     3398 2024-05-28 10:32:53.131902 nonebot_plugin_antimonkey-1.1.1/nonebot_plugin_antimonkey/malou.py
+-rw-r--r--   0        0        0    34885 2023-12-26 10:03:29.933870 nonebot_plugin_antimonkey-1.1.1/nonebot_plugin_antimonkey/monkey_test.jpg
+-rw-r--r--   0        0        0      917 2024-05-28 13:23:45.556299 nonebot_plugin_antimonkey-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2020 2024-05-28 08:43:07.239159 nonebot_plugin_antimonkey-1.1.1/README.md
+-rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 nonebot_plugin_antimonkey-1.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_antimonkey-1.1.0/LICENSE` & `nonebot_plugin_antimonkey-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.1.0/nonebot_plugin_antimonkey/malou.py` & `nonebot_plugin_antimonkey-1.1.1/nonebot_plugin_antimonkey/malou.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.1.0/nonebot_plugin_antimonkey/monkey_test.jpg` & `nonebot_plugin_antimonkey-1.1.1/nonebot_plugin_antimonkey/monkey_test.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.1.0/pyproject.toml` & `nonebot_plugin_antimonkey-1.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-antimonkey"
-version = "1.1.0"
+version = "1.1.1"
 description = "一个用于自动检测和撤回包含猴子图片的QQ机器人插件。"
 authors = ["phquathi <yangziqi233@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/phquathi/nonebot_plugin_antimonkey"
 repository = "https://github.com/phquathi/nonebot_plugin_antimonkey"
 keywords = ["nonebot", "plugin", "antimonkey"]
 
@@ -13,14 +13,15 @@
 nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = "^2.0.0"
 opencv-python = "^4.5.1.48"
 aiohttp = "^3.7.4"
 numpy = "^1.19.5"
 tensorflow = "^2.4.1"
 keras = "^2.4.3"
+nonebot-plugin-apscheduler = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_antimonkey-1.1.0/README.md` & `nonebot_plugin_antimonkey-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.1.0/PKG-INFO` & `nonebot_plugin_antimonkey-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-antimonkey
-Version: 1.1.0
+Version: 1.1.1
 Summary: 一个用于自动检测和撤回包含猴子图片的QQ机器人插件。
 Home-page: https://github.com/phquathi/nonebot_plugin_antimonkey
 Keywords: nonebot,plugin,antimonkey
 Author: phquathi
 Author-email: yangziqi233@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
 Requires-Dist: keras (>=2.4.3,<3.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0,<3.0.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.4.0,<0.5.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: numpy (>=1.19.5,<2.0.0)
 Requires-Dist: opencv-python (>=4.5.1.48,<5.0.0.0)
 Requires-Dist: tensorflow (>=2.4.1,<3.0.0)
 Project-URL: Repository, https://github.com/phquathi/nonebot_plugin_antimonkey
 Description-Content-Type: text/markdown
```

