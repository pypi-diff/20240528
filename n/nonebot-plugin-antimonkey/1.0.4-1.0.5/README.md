# Comparing `tmp/nonebot_plugin_antimonkey-1.0.4.tar.gz` & `tmp/nonebot_plugin_antimonkey-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_antimonkey-1.0.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_antimonkey-1.0.5.tar", max compression
```

## Comparing `nonebot_plugin_antimonkey-1.0.4.tar` & `nonebot_plugin_antimonkey-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1086 2024-05-28 08:29:56.094426 nonebot_plugin_antimonkey-1.0.4/LICENSE
--rw-r--r--   0        0        0      471 2023-12-26 11:41:19.771085 nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/__init__.py
--rw-r--r--   0        0        0      114 2023-12-26 09:19:29.657612 nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/config.py
--rw-r--r--   0        0        0     2040 2024-05-15 09:35:45.433590 nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/image_recognition.py
--rw-r--r--   0        0        0     1921 2024-05-28 07:53:44.039157 nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/malou.py
--rw-r--r--   0        0        0    34885 2023-12-26 10:03:29.933870 nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/monkey_test.jpg
--rw-r--r--   0        0        0      878 2024-05-28 09:16:35.221889 nonebot_plugin_antimonkey-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2020 2024-05-28 08:43:07.239159 nonebot_plugin_antimonkey-1.0.4/README.md
--rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 nonebot_plugin_antimonkey-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-28 08:29:56.094426 nonebot_plugin_antimonkey-1.0.5/LICENSE
+-rw-r--r--   0        0        0      471 2023-12-26 11:41:19.771085 nonebot_plugin_antimonkey-1.0.5/nonebot_plugin_antimonkey/__init__.py
+-rw-r--r--   0        0        0      114 2023-12-26 09:19:29.657612 nonebot_plugin_antimonkey-1.0.5/nonebot_plugin_antimonkey/config.py
+-rw-r--r--   0        0        0     1990 2024-05-28 09:25:35.659072 nonebot_plugin_antimonkey-1.0.5/nonebot_plugin_antimonkey/image_recognition.py
+-rw-r--r--   0        0        0     2347 2024-05-28 09:24:57.052023 nonebot_plugin_antimonkey-1.0.5/nonebot_plugin_antimonkey/malou.py
+-rw-r--r--   0        0        0    34885 2023-12-26 10:03:29.933870 nonebot_plugin_antimonkey-1.0.5/nonebot_plugin_antimonkey/monkey_test.jpg
+-rw-r--r--   0        0        0      878 2024-05-28 09:27:23.307682 nonebot_plugin_antimonkey-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2020 2024-05-28 08:43:07.239159 nonebot_plugin_antimonkey-1.0.5/README.md
+-rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 nonebot_plugin_antimonkey-1.0.5/PKG-INFO
```

### Comparing `nonebot_plugin_antimonkey-1.0.4/LICENSE` & `nonebot_plugin_antimonkey-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/image_recognition.py` & `nonebot_plugin_antimonkey-1.0.5/nonebot_plugin_antimonkey/image_recognition.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 def check_image(image: np.ndarray) -> bool:
     """
     检查图像中是否有猴子。
     :param image: OpenCV图像数组。
     :return: 如果图像中有猴子，返回True；否则返回False。
     """
-    # 调整图像大小为模型所需的尺寸
     image = cv2.resize(image, (224, 224))
 
     image = img_to_array(image)
     image = np.expand_dims(image, axis=0)
     image = preprocess_input(image)
 
     predictions = model.predict(image)
```

### Comparing `nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/malou.py` & `nonebot_plugin_antimonkey-1.0.5/nonebot_plugin_antimonkey/malou.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,33 +16,42 @@
             if resp.status == 200:
                 image_data = await resp.read()
                 image_array = np.asarray(bytearray(image_data), dtype="uint8")
                 image = cv2.imdecode(image_array, cv2.IMREAD_COLOR)
                 return image
 
 
-# 只有当群聊消息中包含图像时才触发
 async def group_message_contains_image(event: MessageEvent) -> bool:
-    return isinstance(event, GroupMessageEvent) and any(seg.type == 'image' for seg in event.message)
+    if isinstance(event, GroupMessageEvent) and any(seg.type == 'image' for seg in event.message):
+        logger.debug("Message contains image.")
+        return True
+    logger.debug("Message does not contain image.")
+    return False
 
 
 revoke_plugin = on_message(rule=Rule(group_message_contains_image))
 
 
 @revoke_plugin.handle()
 async def handle_image_message(bot: Bot, event: GroupMessageEvent):
     group_id = event.group_id
+    logger.debug(f"Received image message in group {group_id}")
     member_info = await bot.get_group_member_info(group_id=group_id, user_id=event.self_id)  # 管理员检测
+    logger.debug(f"Bot role in group: {member_info['role']}")
     if member_info['role'] != 'admin':
+        logger.debug("Bot is not admin. Exiting.")
         return
 
     for seg in event.message:
         if seg.type == 'image':
             try:
                 image_url = seg.data['url']
+                logger.debug(f"Downloading image from {image_url}")
                 image = await download_image(image_url)
                 if check_image(image):
                     await bot.call_api('delete_msg', message_id=event.message_id)
                     await bot.send(event, "请不要发猴子图片")
                     logger.info(f"撤回了包含猴子的图片并发送警告：{image_url}")
+                else:
+                    logger.debug("Image does not contain monkey.")
             except Exception as e:
                 logger.error(f"处理图片时出错：{e}")
```

### Comparing `nonebot_plugin_antimonkey-1.0.4/nonebot_plugin_antimonkey/monkey_test.jpg` & `nonebot_plugin_antimonkey-1.0.5/nonebot_plugin_antimonkey/monkey_test.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.4/pyproject.toml` & `nonebot_plugin_antimonkey-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-antimonkey"
-version = "1.0.4"
+version = "1.0.5"
 description = "一个用于自动检测和撤回包含猴子图片的QQ机器人插件。"
 authors = ["phquathi <yangziqi233@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/phquathi/nonebot_plugin_antimonkey"
 repository = "https://github.com/phquathi/nonebot_plugin_antimonkey"
 keywords = ["nonebot", "plugin", "antimonkey"]
```

### Comparing `nonebot_plugin_antimonkey-1.0.4/README.md` & `nonebot_plugin_antimonkey-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.4/PKG-INFO` & `nonebot_plugin_antimonkey-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-antimonkey
-Version: 1.0.4
+Version: 1.0.5
 Summary: 一个用于自动检测和撤回包含猴子图片的QQ机器人插件。
 Home-page: https://github.com/phquathi/nonebot_plugin_antimonkey
 Keywords: nonebot,plugin,antimonkey
 Author: phquathi
 Author-email: yangziqi233@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
```

