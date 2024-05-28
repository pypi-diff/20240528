# Comparing `tmp/nonebot_plugin_antimonkey-1.0.7.tar.gz` & `tmp/nonebot_plugin_antimonkey-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_antimonkey-1.0.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_antimonkey-1.0.8.tar", max compression
```

## Comparing `nonebot_plugin_antimonkey-1.0.7.tar` & `nonebot_plugin_antimonkey-1.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1086 2024-05-28 08:29:56.094426 nonebot_plugin_antimonkey-1.0.7/LICENSE
--rw-r--r--   0        0        0      493 2024-05-28 10:17:49.209115 nonebot_plugin_antimonkey-1.0.7/nonebot_plugin_antimonkey/__init__.py
--rw-r--r--   0        0        0      114 2023-12-26 09:19:29.657612 nonebot_plugin_antimonkey-1.0.7/nonebot_plugin_antimonkey/config.py
--rw-r--r--   0        0        0     4171 2024-05-28 10:15:17.978973 nonebot_plugin_antimonkey-1.0.7/nonebot_plugin_antimonkey/malou.py
--rw-r--r--   0        0        0    34885 2023-12-26 10:03:29.933870 nonebot_plugin_antimonkey-1.0.7/nonebot_plugin_antimonkey/monkey_test.jpg
--rw-r--r--   0        0        0      878 2024-05-28 10:18:55.676547 nonebot_plugin_antimonkey-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2020 2024-05-28 08:43:07.239159 nonebot_plugin_antimonkey-1.0.7/README.md
--rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 nonebot_plugin_antimonkey-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-28 08:29:56.094426 nonebot_plugin_antimonkey-1.0.8/LICENSE
+-rw-r--r--   0        0        0      493 2024-05-28 10:17:49.209115 nonebot_plugin_antimonkey-1.0.8/nonebot_plugin_antimonkey/__init__.py
+-rw-r--r--   0        0        0      114 2023-12-26 09:19:29.657612 nonebot_plugin_antimonkey-1.0.8/nonebot_plugin_antimonkey/config.py
+-rw-r--r--   0        0        0     3440 2024-05-28 10:25:15.232340 nonebot_plugin_antimonkey-1.0.8/nonebot_plugin_antimonkey/malou.py
+-rw-r--r--   0        0        0    34885 2023-12-26 10:03:29.933870 nonebot_plugin_antimonkey-1.0.8/nonebot_plugin_antimonkey/monkey_test.jpg
+-rw-r--r--   0        0        0      878 2024-05-28 10:25:32.752890 nonebot_plugin_antimonkey-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2020 2024-05-28 08:43:07.239159 nonebot_plugin_antimonkey-1.0.8/README.md
+-rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 nonebot_plugin_antimonkey-1.0.8/PKG-INFO
```

### Comparing `nonebot_plugin_antimonkey-1.0.7/LICENSE` & `nonebot_plugin_antimonkey-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.7/nonebot_plugin_antimonkey/malou.py` & `nonebot_plugin_antimonkey-1.0.8/nonebot_plugin_antimonkey/malou.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,34 +9,30 @@
 from nonebot.rule import Rule
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent
 import aiohttp
 
 logging.basicConfig(level=logging.DEBUG)
 logger = logging.getLogger(__name__)
 
-logger.info("Loading MobileNetV2 model...")
 # MobileNetV2模型
 model = MobileNetV2(weights="imagenet")
 
 
 def check_image(image: np.ndarray) -> bool:
     """
     检查图像中是否有猴子。
     :param image: OpenCV图像数组。
     :return: 如果图像中有猴子，返回True；否则返回False。
     """
-    logger.debug("Resizing image...")
     image = cv2.resize(image, (224, 224))
 
-    logger.debug("Converting image to array...")
     image = img_to_array(image)
     image = np.expand_dims(image, axis=0)
     image = preprocess_input(image)
 
-    logger.debug("Predicting image...")
     predictions = model.predict(image)
     results = imagenet_utils.decode_predictions(predictions)
 
     monkey_labels = {
         "guenon", "guenon monkey",
         "patas", "hussar monkey", "Erythrocebus patas",
         "baboon",
@@ -48,20 +44,17 @@
         "capuchin", "ringtail", "Cebus capucinus",
         "howler monkey", "howler",
         "titi", "titi monkey",
         "spider monkey", "Ateles geoffroyi",
         "squirrel monkey", "Saimiri sciureus"
     }
 
-    logger.debug("Checking predictions...")
     for _, label, probability in results[0]:
         if label in monkey_labels and probability > 0.1:  # 阈值
-            logger.info(f"Detected monkey with probability {probability:.2f}")
             return True
-    logger.info(f"No monkey detected, highest probability: {probability:.2f}")
     return False
 
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 
 async def download_image(url: str) -> np.ndarray:
@@ -72,38 +65,32 @@
                 image_array = np.asarray(bytearray(image_data), dtype="uint8")
                 image = cv2.imdecode(image_array, cv2.IMREAD_COLOR)
                 return image
 
 
 async def group_message_contains_image(event: MessageEvent) -> bool:
     if isinstance(event, GroupMessageEvent) and any(seg.type == 'image' for seg in event.message):
-        logger.debug("Message contains image.")
         return True
-    logger.debug("Message does not contain image.")
     return False
 
 
 revoke_plugin = on_message(rule=Rule(group_message_contains_image))
 
 
 @revoke_plugin.handle()
 async def handle_image_message(bot: Bot, event: GroupMessageEvent):
     group_id = event.group_id
-    logger.debug(f"Received image message in group {group_id}")
     member_info = await bot.get_group_member_info(group_id=group_id, user_id=event.self_id)  # 管理员检测
-    logger.debug(f"Bot role in group: {member_info['role']}")
     if member_info['role'] != 'admin':
-        logger.debug("Bot is not admin. Exiting.")
         return
 
     for seg in event.message:
         if seg.type == 'image':
             try:
                 image_url = seg.data['url']
-                logger.debug(f"Downloading image from {image_url}")
                 image = await download_image(image_url)
                 if check_image(image):
                     await bot.call_api('delete_msg', message_id=event.message_id)
                     await bot.send(event, "请不要发猴子图片")
                     logger.info(f"撤回了包含猴子的图片并发送警告：{image_url}")
                 else:
                     logger.debug("Image does not contain monkey.")
```

### Comparing `nonebot_plugin_antimonkey-1.0.7/nonebot_plugin_antimonkey/monkey_test.jpg` & `nonebot_plugin_antimonkey-1.0.8/nonebot_plugin_antimonkey/monkey_test.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.7/pyproject.toml` & `nonebot_plugin_antimonkey-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-antimonkey"
-version = "1.0.7"
+version = "1.0.8"
 description = "一个用于自动检测和撤回包含猴子图片的QQ机器人插件。"
 authors = ["phquathi <yangziqi233@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/phquathi/nonebot_plugin_antimonkey"
 repository = "https://github.com/phquathi/nonebot_plugin_antimonkey"
 keywords = ["nonebot", "plugin", "antimonkey"]
```

### Comparing `nonebot_plugin_antimonkey-1.0.7/README.md` & `nonebot_plugin_antimonkey-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.7/PKG-INFO` & `nonebot_plugin_antimonkey-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-antimonkey
-Version: 1.0.7
+Version: 1.0.8
 Summary: 一个用于自动检测和撤回包含猴子图片的QQ机器人插件。
 Home-page: https://github.com/phquathi/nonebot_plugin_antimonkey
 Keywords: nonebot,plugin,antimonkey
 Author: phquathi
 Author-email: yangziqi233@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
```

