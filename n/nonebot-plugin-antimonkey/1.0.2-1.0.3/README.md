# Comparing `tmp/nonebot_plugin_antimonkey-1.0.2.tar.gz` & `tmp/nonebot_plugin_antimonkey-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_antimonkey-1.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_antimonkey-1.0.3.tar", max compression
```

## Comparing `nonebot_plugin_antimonkey-1.0.2.tar` & `nonebot_plugin_antimonkey-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1086 2023-12-26 14:51:01.010053 nonebot_plugin_antimonkey-1.0.2/LICENSE
--rw-r--r--   0        0        0      471 2023-12-26 11:41:19.771085 nonebot_plugin_antimonkey-1.0.2/nonebot_plugin_antimonkey/__init__.py
--rw-r--r--   0        0        0      114 2023-12-26 09:19:29.657612 nonebot_plugin_antimonkey-1.0.2/nonebot_plugin_antimonkey/config.py
--rw-r--r--   0        0        0     2162 2023-12-26 18:07:44.611651 nonebot_plugin_antimonkey-1.0.2/nonebot_plugin_antimonkey/image_recognition.py
--rw-r--r--   0        0        0     1946 2023-12-27 17:24:36.597869 nonebot_plugin_antimonkey-1.0.2/nonebot_plugin_antimonkey/malou.py
--rw-r--r--   0        0        0    34885 2023-12-26 10:03:29.933870 nonebot_plugin_antimonkey-1.0.2/nonebot_plugin_antimonkey/monkey_test.jpg
--rw-r--r--   0        0        0      556 2023-12-27 17:39:03.480023 nonebot_plugin_antimonkey-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1922 2023-12-27 14:28:24.668661 nonebot_plugin_antimonkey-1.0.2/README.md
--rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 nonebot_plugin_antimonkey-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      471 2023-12-26 11:41:19.771085 nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/__init__.py
+-rw-r--r--   0        0        0      114 2023-12-26 09:19:29.657612 nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/config.py
+-rw-r--r--   0        0        0     2040 2024-05-15 09:35:45.433590 nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/image_recognition.py
+-rw-r--r--   0        0        0     1921 2024-05-28 07:53:44.039157 nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/malou.py
+-rw-r--r--   0        0        0    34885 2023-12-26 10:03:29.933870 nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/monkey_test.jpg
+-rw-r--r--   0        0        0      878 2024-05-28 08:15:44.937540 nonebot_plugin_antimonkey-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1939 2023-12-27 17:41:02.880702 nonebot_plugin_antimonkey-1.0.3/README.md
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 nonebot_plugin_antimonkey-1.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_antimonkey-1.0.2/nonebot_plugin_antimonkey/image_recognition.py` & `nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/image_recognition.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,20 +15,18 @@
     检查图像中是否有猴子。
     :param image: OpenCV图像数组。
     :return: 如果图像中有猴子，返回True；否则返回False。
     """
     # 调整图像大小为模型所需的尺寸
     image = cv2.resize(image, (224, 224))
 
-    # 将图像转换为数组并进行预处理
     image = img_to_array(image)
     image = np.expand_dims(image, axis=0)
     image = preprocess_input(image)
 
-    # 使用模型进行预测
     predictions = model.predict(image)
     results = imagenet_utils.decode_predictions(predictions)
 
     monkey_labels = {
         "guenon", "guenon monkey",
         "patas", "hussar monkey", "Erythrocebus patas",
         "baboon",
@@ -41,22 +39,21 @@
         "howler monkey", "howler",
         "titi", "titi monkey",
         "spider monkey", "Ateles geoffroyi",
         "squirrel monkey", "Saimiri sciureus"
     }
 
     for _, label, probability in results[0]:
-        if label in monkey_labels and probability > 0.1:  # 调整阈值
+        if label in monkey_labels and probability > 0.1:  # 阈值
             print(f"({probability:.2f})")
             return True
     print(f"({probability:.2f})")
     return False
 
 # if __name__ == "__main__":
-#     # 测试图像识别功能
 #     test_image_path = 'monkey_test.jpg'
 #
 #
 #     test_image = cv2.imread(test_image_path)
 #
 #
 #     if test_image is not None:
```

### Comparing `nonebot_plugin_antimonkey-1.0.2/nonebot_plugin_antimonkey/malou.py` & `nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/malou.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,28 @@
 
 
 # 只有当群聊消息中包含图像时才触发
 async def group_message_contains_image(event: MessageEvent) -> bool:
     return isinstance(event, GroupMessageEvent) and any(seg.type == 'image' for seg in event.message)
 
 
-# 应用规则
 revoke_plugin = on_message(rule=Rule(group_message_contains_image))
 
 
 @revoke_plugin.handle()
 async def handle_image_message(bot: Bot, event: GroupMessageEvent):
     group_id = event.group_id
-    member_info = await bot.get_group_member_info(group_id=group_id, user_id=event.self_id)  # 管理员检测，节省系统资源
+    member_info = await bot.get_group_member_info(group_id=group_id, user_id=event.self_id)  # 管理员检测
     if member_info['role'] != 'admin':
         return
 
     for seg in event.message:
         if seg.type == 'image':
             try:
                 image_url = seg.data['url']
                 image = await download_image(image_url)
                 if check_image(image):
-                    await bot.delete_msg(message_id=event.message_id)
+                    await bot.call_api('delete_msg', message_id=event.message_id)
                     await bot.send(event, "请不要发猴子图片")
                     logger.info(f"撤回了包含猴子的图片并发送警告：{image_url}")
             except Exception as e:
                 logger.error(f"处理图片时出错：{e}")
```

### Comparing `nonebot_plugin_antimonkey-1.0.2/nonebot_plugin_antimonkey/monkey_test.jpg` & `nonebot_plugin_antimonkey-1.0.3/nonebot_plugin_antimonkey/monkey_test.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_antimonkey-1.0.2/README.md` & `nonebot_plugin_antimonkey-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 ## 存在的问题
 
 不是百分百能识别准确！特别是抽象🐒图！
 
 偶尔会有cv2报错，可能存在于检测表情包这类较小的图片，调整尺寸时发生了错误从而无法读取图片
 
-与部分插件比如“今日运势”冲突，正在加紧修复
+~~与部分插件比如“今日运势”冲突，正在加紧修复~~ 已修复！
 
 管理员的🐒图撤不了
 
 群主的🐒图更撤不了
 
 ## 贡献
 欢迎提交Pull Request或报告Issues。
```

### Comparing `nonebot_plugin_antimonkey-1.0.2/PKG-INFO` & `nonebot_plugin_antimonkey-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-antimonkey
-Version: 1.0.2
+Version: 1.0.3
 Summary: 一个用于自动检测和撤回包含猴子图片的QQ机器人插件。
+Home-page: https://github.com/phquathi/nonebot_plugin_antimonkey
+Keywords: nonebot,plugin,antimonkey
 Author: phquathi
 Author-email: yangziqi233@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.0.0,<4.0.0)
+Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
+Requires-Dist: keras (>=2.4.3,<3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
-Requires-Dist: numpy (>=1.0.0,<2.0.0)
-Requires-Dist: opencv-python (>=4.0.0,<5.0.0)
-Requires-Dist: tensorflow (>=2.0.0,<3.0.0)
+Requires-Dist: numpy (>=1.19.5,<2.0.0)
+Requires-Dist: opencv-python (>=4.5.1.48,<5.0.0.0)
+Requires-Dist: tensorflow (>=2.4.1,<3.0.0)
+Project-URL: Repository, https://github.com/phquathi/nonebot_plugin_antimonkey
 Description-Content-Type: text/markdown
 
 # NoneBot-Plugin-AntiMonkey
 
 基于cv2和预训练的机器学习模型（TensorFlow）实现检测🐒猴子图并撤回的nonebot插件
 
 ## 声明
@@ -49,15 +54,15 @@
 
 ## 存在的问题
 
 不是百分百能识别准确！特别是抽象🐒图！
 
 偶尔会有cv2报错，可能存在于检测表情包这类较小的图片，调整尺寸时发生了错误从而无法读取图片
 
-与部分插件比如“今日运势”冲突，正在加紧修复
+~~与部分插件比如“今日运势”冲突，正在加紧修复~~ 已修复！
 
 管理员的🐒图撤不了
 
 群主的🐒图更撤不了
 
 ## 贡献
 欢迎提交Pull Request或报告Issues。
```

