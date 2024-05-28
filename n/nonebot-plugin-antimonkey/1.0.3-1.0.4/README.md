# Comparing `tmp/nonebot_plugin_antimonkey-1.0.3.tar.gz` & `tmp/nonebot_plugin_antimonkey-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_antimonkey-1.0.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_antimonkey-1.0.4.tar", max compression
```

## Comparing `nonebot_plugin_antimonkey-1.0.3.tar` & `nonebot_plugin_antimonkey-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      471 2023-12-26 11:41:19.771085 nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/__init__.py
--rw-r--r--   0        0        0      114 2023-12-26 09:19:29.657612 nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/config.py
--rw-r--r--   0        0        0     2040 2024-05-15 09:35:45.433590 nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/image_recognition.py
--rw-r--r--   0        0        0     1921 2024-05-28 07:53:44.039157 nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/malou.py
--rw-r--r--   0        0        0    34885 2023-12-26 10:03:29.933870 nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/monkey_test.jpg
--rw-r--r--   0        0        0      878 2024-05-28 08:15:44.937540 nonebot_plugin_antimonkey-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1939 2023-12-27 17:41:02.880702 nonebot_plugin_antimonkey-1.0.3/README.md
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 nonebot_plugin_antimonkey-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-28 08:29:56.094426 nonebot_plugin_antimonkey-1.0.4/LICENSE
+-rw-r--r--   0        0        0      471 2023-12-26 11:41:19.771085 nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/__init__.py
+-rw-r--r--   0        0        0      114 2023-12-26 09:19:29.657612 nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/config.py
+-rw-r--r--   0        0        0     2040 2024-05-15 09:35:45.433590 nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/image_recognition.py
+-rw-r--r--   0        0        0     1921 2024-05-28 07:53:44.039157 nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/malou.py
+-rw-r--r--   0        0        0    34885 2023-12-26 10:03:29.933870 nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/monkey_test.jpg
+-rw-r--r--   0        0        0      878 2024-05-28 09:16:35.221889 nonebot_plugin_antimonkey-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2020 2024-05-28 08:43:07.239159 nonebot_plugin_antimonkey-1.0.4/README.md
+-rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 nonebot_plugin_antimonkey-1.0.4/PKG-INFO
```

### Comparing `nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/image_recognition.py` & `nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/image_recognition.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/malou.py` & `nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/malou.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/monkey_test.jpg` & `nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/monkey_test.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.3/pyproject.toml` & `nonebot_plugin_antimonkey-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-antimonkey"
-version = "1.0.3"
+version = "1.0.4"
 description = "一个用于自动检测和撤回包含猴子图片的QQ机器人插件。"
 authors = ["phquathi <yangziqi233@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/phquathi/nonebot_plugin_antimonkey"
 repository = "https://github.com/phquathi/nonebot_plugin_antimonkey"
 keywords = ["nonebot", "plugin", "antimonkey"]
```

### Comparing `nonebot_plugin_antimonkey-1.0.3/README.md` & `nonebot_plugin_antimonkey-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 
 🐒🐒🐒
 
 本插件能在bot是管理员的群持续检测群聊人员所发图片，判断是否为🐒图并自动撤回，值得注意的是，**撤回功能并不受tx风控影响！**
 
 ## 安装
 
+使用nb-cli进行安装
+
+``nb plugin install nonebot-plugin-antimonkey``
+
+
 使用pip进行安装
 
 ``pip install nonebot-plugin-antimonkey``
 
 
 
 ## 使用
```

### Comparing `nonebot_plugin_antimonkey-1.0.3/PKG-INFO` & `nonebot_plugin_antimonkey-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-antimonkey
-Version: 1.0.3
+Version: 1.0.4
 Summary: 一个用于自动检测和撤回包含猴子图片的QQ机器人插件。
 Home-page: https://github.com/phquathi/nonebot_plugin_antimonkey
 Keywords: nonebot,plugin,antimonkey
 Author: phquathi
 Author-email: yangziqi233@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -38,14 +38,19 @@
 
 🐒🐒🐒
 
 本插件能在bot是管理员的群持续检测群聊人员所发图片，判断是否为🐒图并自动撤回，值得注意的是，**撤回功能并不受tx风控影响！**
 
 ## 安装
 
+使用nb-cli进行安装
+
+``nb plugin install nonebot-plugin-antimonkey``
+
+
 使用pip进行安装
 
 ``pip install nonebot-plugin-antimonkey``
 
 
 
 ## 使用
```

