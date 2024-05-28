# Comparing `tmp/danila-lib-1.8.0.tar.gz` & `tmp/danila-lib-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.8.0.tar", last modified: Tue May 28 08:29:09 2024, max compression
+gzip compressed data, was "danila-lib-1.8.1.tar", last modified: Tue May 28 10:14:07 2024, max compression
```

## Comparing `danila-lib-1.8.0.tar` & `danila-lib-1.8.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 08:29:09.062759 danila-lib-1.8.0/
--rw-rw-rw-   0        0        0     9615 2024-05-28 08:29:09.061763 danila-lib-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 08:29:09.014973 danila-lib-1.8.0/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.0/danila/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.8.0/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.0/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.0/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.0/danila/danila_v3.py
--rw-rw-rw-   0        0        0    20948 2024-05-28 08:28:46.000000 danila-lib-1.8.0/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:29:09.046830 danila-lib-1.8.0/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-28 08:29:08.000000 danila-lib-1.8.0/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      940 2024-05-28 08:29:08.000000 danila-lib-1.8.0/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 08:29:08.000000 danila-lib-1.8.0/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-28 08:29:08.000000 danila-lib-1.8.0/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-28 08:29:08.000000 danila-lib-1.8.0/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 08:29:09.047826 danila-lib-1.8.0/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.0/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:29:09.054794 danila-lib-1.8.0/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.0/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.0/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.0/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.0/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.0/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.0/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6705 2024-05-28 08:02:16.000000 danila-lib-1.8.0/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      654 2024-05-22 10:13:34.000000 danila-lib-1.8.0/data/neuro/models.py
--rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.0/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4845 2024-05-28 08:02:16.000000 danila-lib-1.8.0/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:29:09.060767 danila-lib-1.8.0/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.0/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.0/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.0/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.0/data/result/Label_area.py
--rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.0/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.0/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.0/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.0/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.0/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.0/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.0/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-28 08:29:09.071718 danila-lib-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-28 08:28:46.000000 danila-lib-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:14:07.328394 danila-lib-1.8.1/
+-rw-rw-rw-   0        0        0     9615 2024-05-28 10:14:07.327399 danila-lib-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 10:14:07.268663 danila-lib-1.8.1/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.1/danila/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.8.1/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.1/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.1/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.1/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    24354 2024-05-28 10:13:47.000000 danila-lib-1.8.1/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:14:07.312466 danila-lib-1.8.1/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-28 10:14:07.000000 danila-lib-1.8.1/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2024-05-28 10:14:07.000000 danila-lib-1.8.1/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 10:14:07.000000 danila-lib-1.8.1/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-28 10:14:07.000000 danila-lib-1.8.1/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-28 10:14:07.000000 danila-lib-1.8.1/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 10:14:07.312466 danila-lib-1.8.1/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.1/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:14:07.319435 danila-lib-1.8.1/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.1/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.1/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.1/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.1/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.1/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.1/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6705 2024-05-28 08:02:16.000000 danila-lib-1.8.1/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      654 2024-05-22 10:13:34.000000 danila-lib-1.8.1/data/neuro/models.py
+-rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.1/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4845 2024-05-28 08:02:16.000000 danila-lib-1.8.1/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:14:07.326404 danila-lib-1.8.1/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.1/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.1/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.1/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.1/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.1/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.1/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.1/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.1/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.1/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.1/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.1/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-28 10:14:07.338350 danila-lib-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-28 10:13:47.000000 danila-lib-1.8.1/setup.py
```

### Comparing `danila-lib-1.8.0/PKG-INFO` & `danila-lib-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.8.0
+Version: 1.8.1
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.8.0/README.md` & `danila-lib-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/danila/danila.py` & `danila-lib-1.8.1/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/danila/danila_v1.py` & `danila-lib-1.8.1/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/danila/danila_v2.py` & `danila-lib-1.8.1/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/danila/danila_v3.py` & `danila-lib-1.8.1/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/danila/danila_v4.py` & `danila-lib-1.8.1/danila/danila_v4.py`

 * *Files 13% similar despite different names*

```diff
@@ -66,28 +66,50 @@
     def rama_classify(self, img, size = 256):
         """rama_classify(Img : openCv frame): String - returns class of rama using CNN network"""
         """rama_classify uses Rama_classify_class method - classify(Img)"""
         # img = cv2.imread(img_path)
         rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
         detail_prod = Text_cut_recognize_result(rama_prod_conf.rama_prod.name, rama_prod_conf.conf)
         detail = Text_recognize_result(detail_prod)
+        if (detail.detail.text == 'no_rama'):
+            sizes = [256,384,512,640]
+            flag = True
+            for s in sizes:
+                if flag:
+                    rama_prod_conf1 = self.rama_prod_classify_model.classify(img, s)
+                    detail_prod1 = Text_cut_recognize_result(rama_prod_conf1.rama_prod.name, rama_prod_conf1.conf)
+                    detail1 = Text_recognize_result(detail_prod1)
+                    if (detail1.detail.text != 'no_rama'):
+                        detail = detail1
+                        flag = False
         return detail
 
     # returns openCV frame with rama from openCV frame\
     def rama_detect(self, img, size = 256):
         """rama_detect(img : openCV img) -> openCV image with drawn rama rectangle"""
         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
         hash_str = hash_object.hexdigest()
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
         rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
         rama_prod = rama_prod_conf.rama_prod
         if rama_prod == Rama_Prod.no_rama:
-            os.remove(initial_image_path)
-            return img
+            sizes = [256, 384, 512, 640]
+            flag = True
+            for s in sizes:
+                if flag:
+                    rama_prod_conf1 = self.rama_prod_classify_model.classify(img, s)
+                    rama_prod1 = rama_prod_conf1.rama_prod
+                    if (rama_prod1 == Rama_Prod.no_rama):
+                        rama_prod_conf = rama_prod_conf1
+                        rama_prod = rama_prod_conf.rama_prod
+                        flag = False
+            if flag:
+                os.remove(initial_image_path)
+                return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
         else:
             rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
         new_img = img.copy()
         os.remove(initial_image_path)
@@ -104,16 +126,27 @@
         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
         hash_str = hash_object.hexdigest()
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
         rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
         rama_prod = rama_prod_conf.rama_prod
         if rama_prod == Rama_Prod.no_rama:
-            os.remove(initial_image_path)
-            return img
+            sizes = [256, 384, 512, 640]
+            flag = True
+            for s in sizes:
+                if flag:
+                    rama_prod_conf1 = self.rama_prod_classify_model.classify(img, s)
+                    rama_prod1 = rama_prod_conf1.rama_prod
+                    if (rama_prod1 == Rama_Prod.no_rama):
+                        rama_prod_conf = rama_prod_conf1
+                        rama_prod = rama_prod_conf.rama_prod
+                        flag = False
+            if flag:
+                os.remove(initial_image_path)
+                return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
         else:
             rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
         if rect is None:
             os.remove(initial_image_path)
@@ -128,16 +161,27 @@
         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
         hash_str = hash_object.hexdigest()
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
         rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
         rama_prod = rama_prod_conf.rama_prod
         if rama_prod == Rama_Prod.no_rama:
-            os.remove(initial_image_path)
-            return {'result': 'no_rama'}
+            sizes = [256, 384, 512, 640]
+            flag = True
+            for s in sizes:
+                if flag:
+                    rama_prod_conf1 = self.rama_prod_classify_model.classify(img, s)
+                    rama_prod1 = rama_prod_conf1.rama_prod
+                    if (rama_prod1 == Rama_Prod.no_rama):
+                        rama_prod_conf = rama_prod_conf1
+                        rama_prod = rama_prod_conf.rama_prod
+                        flag = False
+            if flag:
+                os.remove(initial_image_path)
+                return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
                 os.remove(initial_image_path)
                 return img
             img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
@@ -172,16 +216,27 @@
         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
         hash_str = hash_object.hexdigest()
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
         rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
         rama_prod = rama_prod_conf.rama_prod
         if rama_prod == Rama_Prod.no_rama:
-            os.remove(initial_image_path)
-            return img
+            sizes = [256, 384, 512, 640]
+            flag = True
+            for s in sizes:
+                if flag:
+                    rama_prod_conf1 = self.rama_prod_classify_model.classify(img, s)
+                    rama_prod1 = rama_prod_conf1.rama_prod
+                    if (rama_prod1 == Rama_Prod.no_rama):
+                        rama_prod_conf = rama_prod_conf1
+                        rama_prod = rama_prod_conf.rama_prod
+                        flag = False
+            if flag:
+                os.remove(initial_image_path)
+                return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
                 os.remove(initial_image_path)
                 return img
             img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
@@ -220,16 +275,31 @@
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
         rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
         rama_prod = rama_prod_conf.rama_prod
         detail_prod = Text_cut_recognize_result(rama_prod_conf.rama_prod.name, rama_prod_conf.conf)
         detail = Text_recognize_result(detail_prod)
         if rama_prod == Rama_Prod.no_rama:
-            os.remove(initial_image_path)
-            return detail
+            sizes = [256, 384, 512, 640]
+            flag = True
+            for s in sizes:
+                if flag:
+                    rama_prod_conf1 = self.rama_prod_classify_model.classify(img, s)
+                    rama_prod1 = rama_prod_conf1.rama_prod
+                    detail_prod1 = Text_cut_recognize_result(rama_prod_conf1.rama_prod.name, rama_prod_conf1.conf)
+                    detail1 = Text_recognize_result(detail_prod1)
+                    if (rama_prod1 == Rama_Prod.no_rama):
+                        rama_prod_conf = rama_prod_conf1
+                        rama_prod = rama_prod_conf.rama_prod
+                        detail = detail1
+                        detail_prod = detail_prod1
+                        flag = False
+            if flag:
+                os.remove(initial_image_path)
+                return img
         rect = Rect()
         detail.prod = Text_cut_recognize_result(rama_prod.name, rama_prod_conf.conf)
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
                 os.remove(initial_image_path)
                 return detail
```

### Comparing `danila-lib-1.8.0/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.8.1/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.8.0
+Version: 1.8.1
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.8.0/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.8.1/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/danila_lib.egg-info/requires.txt` & `danila-lib-1.8.1/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/neuro/Letters_recognize.py` & `danila-lib-1.8.1/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/neuro/Rama_classify_class.py` & `danila-lib-1.8.1/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/neuro/Rama_detect_class.py` & `danila-lib-1.8.1/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.8.1/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/neuro/Text_detect_class.py` & `danila-lib-1.8.1/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/neuro/letters_in_image.py` & `danila-lib-1.8.1/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/neuro/models.py` & `danila-lib-1.8.1/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/neuro/objs_in_image.py` & `danila-lib-1.8.1/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/neuro/text_recognize_yolo.py` & `danila-lib-1.8.1/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/result/Image_text_areas.py` & `danila-lib-1.8.1/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/result/Rect.py` & `danila-lib-1.8.1/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/result/Text_area.py` & `danila-lib-1.8.1/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/data/result/Yolo_label_rect.py` & `danila-lib-1.8.1/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.0/setup.py` & `danila-lib-1.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.8.0',
+  version='1.8.1',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

