# Comparing `tmp/danila-lib-1.7.8.tar.gz` & `tmp/danila-lib-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.7.8.tar", last modified: Mon May 27 07:41:33 2024, max compression
+gzip compressed data, was "danila-lib-1.7.9.tar", last modified: Mon May 27 09:59:23 2024, max compression
```

## Comparing `danila-lib-1.7.8.tar` & `danila-lib-1.7.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 07:41:33.320762 danila-lib-1.7.8/
--rw-rw-rw-   0        0        0     9615 2024-05-27 07:41:33.320762 danila-lib-1.7.8/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.7.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 07:41:33.271979 danila-lib-1.7.8/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.7.8/danila/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.7.8/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.7.8/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.7.8/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.7.8/danila/danila_v3.py
--rw-rw-rw-   0        0        0    17970 2024-05-27 07:41:23.000000 danila-lib-1.7.8/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-05-27 07:41:33.304836 danila-lib-1.7.8/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-27 07:41:33.000000 danila-lib-1.7.8/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      940 2024-05-27 07:41:33.000000 danila-lib-1.7.8/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 07:41:33.000000 danila-lib-1.7.8/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-27 07:41:33.000000 danila-lib-1.7.8/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-27 07:41:33.000000 danila-lib-1.7.8/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-27 07:41:33.304836 danila-lib-1.7.8/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.7.8/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 07:41:33.312796 danila-lib-1.7.8/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.7.8/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.7.8/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.7.8/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     2818 2024-05-27 07:41:23.000000 danila-lib-1.7.8/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.7.8/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.8/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.7.8/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      654 2024-05-22 10:13:34.000000 danila-lib-1.7.8/data/neuro/models.py
--rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.7.8/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4619 2024-05-27 07:41:23.000000 danila-lib-1.7.8/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-27 07:41:33.319767 danila-lib-1.7.8/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.7.8/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.7.8/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.7.8/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.7.8/data/result/Label_area.py
--rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.7.8/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.7.8/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.7.8/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.7.8/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.8/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.7.8/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.7.8/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-27 07:41:33.323749 danila-lib-1.7.8/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-27 07:41:29.000000 danila-lib-1.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:59:23.493369 danila-lib-1.7.9/
+-rw-rw-rw-   0        0        0     9615 2024-05-27 09:59:23.492374 danila-lib-1.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.7.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 09:59:23.444588 danila-lib-1.7.9/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.7.9/danila/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.7.9/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.7.9/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.7.9/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.7.9/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    20456 2024-05-27 09:58:57.000000 danila-lib-1.7.9/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:59:23.465494 danila-lib-1.7.9/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-27 09:59:23.000000 danila-lib-1.7.9/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2024-05-27 09:59:23.000000 danila-lib-1.7.9/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 09:59:23.000000 danila-lib-1.7.9/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-27 09:59:23.000000 danila-lib-1.7.9/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 09:59:23.000000 danila-lib-1.7.9/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 09:59:23.467486 danila-lib-1.7.9/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.7.9/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:59:23.479431 danila-lib-1.7.9/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.7.9/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.7.9/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.7.9/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     2982 2024-05-27 08:43:50.000000 danila-lib-1.7.9/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.7.9/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.9/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6607 2024-05-27 09:58:57.000000 danila-lib-1.7.9/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      654 2024-05-22 10:13:34.000000 danila-lib-1.7.9/data/neuro/models.py
+-rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.7.9/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4843 2024-05-27 09:58:57.000000 danila-lib-1.7.9/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:59:23.491378 danila-lib-1.7.9/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.7.9/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.7.9/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.7.9/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.7.9/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.7.9/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.7.9/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.7.9/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.7.9/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.9/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.7.9/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.7.9/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 09:59:23.495363 danila-lib-1.7.9/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-27 09:58:57.000000 danila-lib-1.7.9/setup.py
```

### Comparing `danila-lib-1.7.8/PKG-INFO` & `danila-lib-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.7.8
+Version: 1.7.9
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.7.8/README.md` & `danila-lib-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/danila/danila.py` & `danila-lib-1.7.9/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/danila/danila_v1.py` & `danila-lib-1.7.9/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/danila/danila_v2.py` & `danila-lib-1.7.9/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/danila/danila_v3.py` & `danila-lib-1.7.9/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/danila/danila_v4.py` & `danila-lib-1.7.9/danila/danila_v4.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,26 @@
 from data.result.Rama_prod import Rama_Prod
 from data.result.Rect import Rect
 
 """main module for user"""
 from data.neuro.Rama_classify_class import Rama_classify_class
 from data.neuro.text_recognize_yolo import Text_Recognize_yolo
 
+class Text_recognize_result:
+    def __init__(self, detail, number = None, prod = None, year = None):
+        self.detail = detail
+        self.number = number
+        self.prod = prod
+        self.year = year
+
+class Text_cut_recognize_result:
+    def __init__(self, text, conf):
+        self.text = text
+        self.conf = conf
+
 class Danila_v4:
     """main class for user"""
     def __init__(self, yolov5_dir):
 
         yolo_path = yolov5_dir
         rama_prod_classify_model_path = RAMA_PROD_CLASSIFY_MODEL_ADDRESS
         self.rama_prod_classify_model = Rama_prod_classify_class(rama_prod_classify_model_path, yolo_path)
@@ -37,32 +49,35 @@
         rama_no_spring_bejickaya_text_detect_model_path = RAMA_BEJICKAYA_TEXT_DETECT_MODEL_ADDRESS
         self.rama_no_spring_bejickaya_text_detect_model = Text_detect_class(rama_no_spring_bejickaya_text_detect_model_path,
                                                                             'rama_text_begickaya_detect', yolo_path)
         text_recognize_yolo_ruzhimmash_model_path = TEXT_RECOGNIZE_RUZHIMMASH_MODEL_ADDRESS
         self.text_recognize_ruzhimmash_model = Text_Recognize_yolo(text_recognize_yolo_ruzhimmash_model_path, yolo_path)
         text_recognize_yolo_begickaya_model_path = TEXT_RECOGNIZE_BEGICKAYA_MODEL_ADDRESS
         self.text_recognize_begickaya_model = Text_Recognize_yolo(text_recognize_yolo_begickaya_model_path, yolo_path)
-    # returns string - class of rama using CNN network
-    # img - openCV frame
 
+    # returns Rama_Prod_Conf - class of rama and confidence using CNN network
+    # img - openCV frame
     def rama_classify(self, img, size = 256):
         """rama_classify(Img : openCv frame): String - returns class of rama using CNN network"""
         """rama_classify uses Rama_classify_class method - classify(Img)"""
         # img = cv2.imread(img_path)
-        rama_prod = self.rama_prod_classify_model.classify(img, size)
-        return rama_prod.name
+        rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
+        detail_prod = Text_cut_recognize_result(rama_prod_conf.rama_prod.name, rama_prod_conf.conf)
+        detail = Text_recognize_result(detail_prod)
+        return detail
 
     # returns openCV frame with rama from openCV frame\
     def rama_detect(self, img, size = 256):
         """rama_detect(img : openCV img) -> openCV image with drawn rama rectangle"""
         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
         hash_str = hash_object.hexdigest()
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
-        rama_prod = self.rama_prod_classify_model.classify(img, size)
+        rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
+        rama_prod = rama_prod_conf.rama_prod
         if rama_prod == Rama_Prod.no_rama:
             os.remove(initial_image_path)
             return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
         else:
@@ -79,15 +94,16 @@
     # returns openCV image with cut_rama
     def rama_cut(self, img, size = 256):
         """rama_cut(img : openCV img) -> openCV image of rama rectangle"""
         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
         hash_str = hash_object.hexdigest()
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
-        rama_prod = self.rama_prod_classify_model.classify(img, size)
+        rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
+        rama_prod = rama_prod_conf.rama_prod
         if rama_prod == Rama_Prod.no_rama:
             os.remove(initial_image_path)
             return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
         else:
@@ -102,15 +118,16 @@
     # returns openCV cut rama with drawn text areas
     def text_detect_cut(self, img, size = 256):
         """returns openCV cut rama with drawn text areas"""
         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
         hash_str = hash_object.hexdigest()
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
-        rama_prod = self.rama_prod_classify_model.classify(img, size)
+        rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
+        rama_prod = rama_prod_conf.rama_prod
         if rama_prod == Rama_Prod.no_rama:
             os.remove(initial_image_path)
             return {'result': 'no_rama'}
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
@@ -145,15 +162,16 @@
     # returns openCV img with drawn text areas
     def text_detect(self, img, size = 256):
         """returns openCV img with drawn text areas"""
         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
         hash_str = hash_object.hexdigest()
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
-        rama_prod = self.rama_prod_classify_model.classify(img, size)
+        rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
+        rama_prod = rama_prod_conf.rama_prod
         if rama_prod == Rama_Prod.no_rama:
             os.remove(initial_image_path)
             return img
         rect = Rect()
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
@@ -190,88 +208,105 @@
     # returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'
     def text_recognize(self, img, size = 256):
         """returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'"""
         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
         hash_str = hash_object.hexdigest()
         initial_image_path = 'initial_image' + hash_str + '.jpg'
         cv2.imwrite(initial_image_path, img)
-        rama_prod = self.rama_prod_classify_model.classify(img, size)
+        rama_prod_conf = self.rama_prod_classify_model.classify(img, size)
+        rama_prod = rama_prod_conf.rama_prod
+        detail_prod = Text_cut_recognize_result(rama_prod_conf.rama_prod.name, rama_prod_conf.conf)
+        detail = Text_recognize_result(detail_prod)
         if rama_prod == Rama_Prod.no_rama:
             os.remove(initial_image_path)
-            return {'result': 'no_rama'}
+            return detail
         rect = Rect()
+        detail.prod = Text_cut_recognize_result(rama_prod.name, rama_prod_conf.conf)
         if (rama_prod == Rama_Prod.ruzhimmash):
             rect = self.rama_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
                 os.remove(initial_image_path)
-                return {'result': 'no_rama'}
+                return detail
             img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
             hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
             hash_str = hash_object.hexdigest()
             img_cut_path = 'cut_img' + hash_str + '.jpg'
             cv2.imwrite(img_cut_path, img_cut)
             image_text_areas = self.rama_spring_ruzhimmash_text_detect_model.text_detect(img_cut_path)
 
             label_area = self.text_recognize_ruzhimmash_model.work_image_cut(image_text_areas, img_cut, 5, 64,128,
                                                                   4, 64,128, 2, 64,64)
             res_labels = {}
-            if len(label_area.labels[Class_text.number]) == 5:
-                res_labels['number'] = label_area.labels[Class_text.number]
+            (number_text, number_conf) = label_area.labels[Class_text.number]
+            if len(number_text) == 5:
+                res_labels['number'] = (number_text, number_conf)
             else:
                 number_image_text_areas = image_text_areas.areas[Class_text.number]
                 image_text_areas_min = []
                 image_text_areas_max = []
                 for number_image_text_area in number_image_text_areas:
                     w = number_image_text_area.xmax - number_image_text_area.xmin
-                    if (number_image_text_area.xmin - (w//2)) < 0:
+                    if (number_image_text_area.xmin - (w // 2)) < 0:
                         new_xmin = 0
                     else:
-                        new_xmin = number_image_text_area.xmin - (w//2)
-                    rect_min = Rect(xmin=new_xmin, xmax=number_image_text_area.xmax, ymin=number_image_text_area.ymin, ymax=number_image_text_area.ymax)
+                        new_xmin = number_image_text_area.xmin - (w // 2)
+                    rect_min = Rect(xmin=new_xmin, xmax=number_image_text_area.xmax, ymin=number_image_text_area.ymin,
+                                    ymax=number_image_text_area.ymax)
                     image_text_areas_min.append(rect_min)
-                    new_xmax = number_image_text_area.xmax + w//2
-                    rect_max = Rect(xmin=number_image_text_area.xmin, xmax=new_xmax, ymin=number_image_text_area.ymin, ymax=number_image_text_area.ymax)
+                    new_xmax = number_image_text_area.xmax + w // 2
+                    rect_max = Rect(xmin=number_image_text_area.xmin, xmax=new_xmax, ymin=number_image_text_area.ymin,
+                                    ymax=number_image_text_area.ymax)
                     image_text_areas_max.append(rect_max)
                 image_text_areas.areas[Class_text.number] = image_text_areas_min
-                label_area_min = self.text_recognize_ruzhimmash_model.work_image_cut(image_text_areas, img_cut, 5, 64,128,
+                label_area_min = self.text_recognize_begickaya_model.work_image_cut(image_text_areas, img_cut, 5, 64,128,
                                                                   4, 64,128, 2, 64,64)
-                if len(label_area_min.labels[Class_text.number]) == 5:
-                    res_labels['number'] = label_area_min.labels[Class_text.number]
+                (number_text_min, number_conf_min) = label_area_min.labels[Class_text.number]
+                if len(number_text_min) == 5:
+                    res_labels['number'] = (number_text_min, number_conf_min)
                 else:
                     image_text_areas.areas[Class_text.number] = image_text_areas_max
-                    label_area_max = self.text_recognize_ruzhimmash_model.work_image_cut(image_text_areas, img_cut, 5, 64, 128,
-                                                                              4, 64, 128, 2, 64, 64)
-                    if len(label_area_max.labels[Class_text.number]) == 5:
-                        res_labels['number'] = label_area_max.labels[Class_text.number]
+                    label_area_max = self.text_recognize_begickaya_model.work_image_cut(image_text_areas, img_cut, 5, 64,128,
+                                                                  4, 64,128, 2, 64,64)
+                    (number_text_max, number_conf_max) = label_area_max.labels[Class_text.number]
+                    if len(number_text_max) == 5:
+                        res_labels['number'] = (number_text_max, number_conf_max)
                     else:
-                        res_labels['number'] = label_area.labels[Class_text.number]
-            res_labels['prod'] = '1275'
-            if (len(label_area.labels[Class_text.year]) == 2) and (int(label_area.labels[Class_text.year]) < 25):
-                res_labels['year'] = label_area.labels[Class_text.year]
+                        res_labels['number'] = (number_text, number_conf)
+            res_labels['prod'] = ('1275', detail.prod.conf)
+            (year_text, year_conf) = label_area.labels[Class_text.year]
+            if (len(year_text) == 2) and (int(year_text) < 25):
+                res_labels['year'] = (year_text, year_conf)
             else:
-                res_labels['year'] = '23'
+                res_labels['year'] = ('23', 0.25)
             os.remove(initial_image_path)
             os.remove(img_cut_path)
-            return res_labels
+            res_labels_number_text, res_labels_number_conf = res_labels['number']
+            detail.number = Text_cut_recognize_result(res_labels_number_text, res_labels_number_conf)
+            res_labels_year_text, res_labels_year_conf = res_labels['year']
+            detail.year = Text_cut_recognize_result(res_labels_year_text, res_labels_year_conf)
+            res_labels_prod_text, res_labels_prod_conf = res_labels['prod']
+            detail.prod = Text_cut_recognize_result(res_labels_prod_text, res_labels_prod_conf)
+            return detail
         else:
             rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
                 os.remove(initial_image_path)
-                return {"result" : "no_rama"}
+                return detail
             img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
             hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
             hash_str = hash_object.hexdigest()
             img_cut_path = 'cut_img' + hash_str + '.jpg'
             cv2.imwrite(img_cut_path, img_cut)
             image_text_areas = self.rama_no_spring_bejickaya_text_detect_model.text_detect(img_cut_path)
             label_area = self.text_recognize_begickaya_model.work_image_cut(image_text_areas, img_cut, 6, 64, 192,
                                                                   2, 64, 64, 2, 64,64)
             res_labels = {}
-            if len(label_area.labels[Class_text.number]) == 6:
-                res_labels['number'] = label_area.labels[Class_text.number]
+            (number_text, number_conf) = label_area.labels[Class_text.number]
+            if len(number_text) == 6:
+                res_labels['number'] = (number_text, number_conf)
             else:
                 number_image_text_areas = image_text_areas.areas[Class_text.number]
                 image_text_areas_min = []
                 image_text_areas_max = []
                 for number_image_text_area in number_image_text_areas:
                     w = number_image_text_area.xmax - number_image_text_area.xmin
                     if (number_image_text_area.xmin - (w//2)) < 0:
@@ -280,27 +315,36 @@
                         new_xmin = number_image_text_area.xmin - (w//2)
                     rect_min = Rect(xmin=new_xmin, xmax=number_image_text_area.xmax, ymin=number_image_text_area.ymin, ymax=number_image_text_area.ymax)
                     image_text_areas_min.append(rect_min)
                     new_xmax = number_image_text_area.xmax + w//2
                     rect_max = Rect(xmin=number_image_text_area.xmin, xmax=new_xmax, ymin=number_image_text_area.ymin, ymax=number_image_text_area.ymax)
                     image_text_areas_max.append(rect_max)
                 image_text_areas.areas[Class_text.number] = image_text_areas_min
-                label_area_min = self.text_recognize_begickaya_model.work_image_cut(image_text_areas, img_cut, 5, 64,128,
-                                                                  4, 64,128, 2, 64,64)
-                if len(label_area_min.labels[Class_text.number]) == 6:
-                    res_labels['number'] = label_area_min.labels[Class_text.number]
+                label_area_min = self.text_recognize_begickaya_model.work_image_cut(image_text_areas, img_cut, 6, 64, 192,
+                                                                  2, 64, 64, 2, 64,64)
+                (number_text_min, number_conf_min) = label_area_min.labels[Class_text.number]
+                if len(number_text_min) == 6:
+                    res_labels['number'] = (number_text_min, number_conf_min)
                 else:
                     image_text_areas.areas[Class_text.number] = image_text_areas_max
-                    label_area_max = self.text_recognize_begickaya_model.work_image_cut(image_text_areas, img_cut, 5, 64, 128,
-                                                                              4, 64, 128, 2, 64, 64)
-                    if len(label_area_max.labels[Class_text.number]) == 6:
-                        res_labels['number'] = label_area_max.labels[Class_text.number]
+                    label_area_max = self.text_recognize_begickaya_model.work_image_cut(image_text_areas, img_cut, 6, 64, 192,
+                                                                  2, 64, 64, 2, 64,64)
+                    (number_text_max, number_conf_max) = label_area_max.labels[Class_text.number]
+                    if len(number_text_max) == 6:
+                        res_labels['number'] = (number_text_max, number_conf_max)
                     else:
-                        res_labels['number'] = label_area.labels[Class_text.number]
-            res_labels['prod'] = '12'
-            if (len(label_area.labels[Class_text.year]) == 2) and (int(label_area.labels[Class_text.year]) < 25):
-                res_labels['year'] = label_area.labels[Class_text.year]
+                        res_labels['number'] = (number_text, number_conf)
+            res_labels['prod'] = ('12', detail.prod.conf)
+            (year_text, year_conf) = label_area.labels[Class_text.year]
+            if (len(year_text) == 2) and (int(year_text) < 25):
+                res_labels['year'] = (year_text, year_conf)
             else:
-                res_labels['year'] = '23'
+                res_labels['year'] = ('23', 0.25)
             os.remove(initial_image_path)
             os.remove(img_cut_path)
-            return res_labels
+            res_labels_number_text, res_labels_number_conf = res_labels['number']
+            detail.number = Text_cut_recognize_result(res_labels_number_text, res_labels_number_conf)
+            res_labels_year_text, res_labels_year_conf = res_labels['year']
+            detail.year = Text_cut_recognize_result(res_labels_year_text, res_labels_year_conf)
+            res_labels_prod_text, res_labels_prod_conf = res_labels['prod']
+            detail.prod = Text_cut_recognize_result(res_labels_prod_text, res_labels_prod_conf)
+            return detail
```

### Comparing `danila-lib-1.7.8/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.7.9/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.7.8
+Version: 1.7.9
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.7.8/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.7.9/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/danila_lib.egg-info/requires.txt` & `danila-lib-1.7.9/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/data/neuro/Letters_recognize.py` & `danila-lib-1.7.9/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/data/neuro/Rama_classify_class.py` & `danila-lib-1.7.9/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/data/neuro/Rama_detect_class.py` & `danila-lib-1.7.9/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.7.9/data/neuro/Rama_prod_classify_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torch
 import hashlib
 from datetime import datetime
 from data.neuro.letters_in_image import Letters_In_Image
 from data.neuro.objs_in_image import Objs_In_Image
 from data.result.Class_text import Class_text
 from data.result.Label_area import Label_area
-from data.result.Rama_prod import Rama_Prod
+from data.result.Rama_prod import Rama_Prod, Rama_Prod_Conf
 
 
 class Rama_prod_classify_class:
 
     def __init__(self, model_path, yolo_path):
         """reads yolov5 taught model from yandex-disk and includes it in class example"""
         base_url = 'https://cloud-api.yandex.net/v1/disk/public/resources/download?'
@@ -54,16 +54,17 @@
         return img_objs
 
     def classify(self, img, size):
         image_objs = self.work_image(img, size)
         b_list_r = any(obj.obj == 'bejickaya' for obj in image_objs.objs)
         r_list_r = any(obj.obj == 'ruzhimmash' for obj in image_objs.objs)
         if (b_list_r == False) and (r_list_r == False):
-            return Rama_Prod(2)
+            return Rama_Prod_Conf(Rama_Prod(2), 0.0)
         else:
             if b_list_r and r_list_r:
-                return Rama_Prod(2)
+                return Rama_Prod_Conf(Rama_Prod(2), 0.0)
             else:
+                max_conf = image_objs.get_max_conf()
                 if b_list_r:
-                    return Rama_Prod(0)
+                    return Rama_Prod_Conf(Rama_Prod(0), max_conf)
                 else:
-                    return Rama_Prod(1)
+                    return Rama_Prod_Conf(Rama_Prod(1), max_conf)
```

### Comparing `danila-lib-1.7.8/data/neuro/Text_detect_class.py` & `danila-lib-1.7.9/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/data/neuro/letters_in_image.py` & `danila-lib-1.7.9/data/neuro/letters_in_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,21 @@
             return '_'
         else:
             res = ''
             for letter in self.letters:
                 res += letter.letter
             return res
 
+    def get_avg_conf(self):
+        sum_conf = 0.0
+        count_conf = 0
+        for letter in self.letters:
+            sum_conf = sum_conf + letter.confidence
+            count_conf += 1
+        return sum_conf / count_conf
 
     def __str__(self):
         res = ''
         for letter_in_image in self.letters:
             res = res + letter_in_image.__str__() + '\n'
         return res
```

### Comparing `danila-lib-1.7.8/data/neuro/models.py` & `danila-lib-1.7.9/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/data/neuro/objs_in_image.py` & `danila-lib-1.7.9/data/neuro/objs_in_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,21 @@
         return str(res_dict)
 
 
 class Objs_In_Image:
     def __init__(self):
         self.objs = []
 
+    def get_max_conf(self):
+        max_conf = self.objs[0].confidence
+        for prod_in_image in self.objs:
+            if prod_in_image.confidence > max_conf:
+                max_conf = prod_in_image.confidence
+        return max_conf
+
     @staticmethod
     def get_objs_in_image_from_yolo_json(objs_json):
         objs_in_image = Objs_In_Image()
         for obj_json in objs_json:
             objs_in_image.objs.append(Prod_In_Image.get_obj_in_image_from_yolo_json(obj_json))
         return objs_in_image
```

### Comparing `danila-lib-1.7.8/data/neuro/text_recognize_yolo.py` & `danila-lib-1.7.9/data/neuro/text_recognize_yolo.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,41 +36,42 @@
         # weights_file_path = model_name + '_weights.pt'
         self.model = torch.hub.load(yolo_path, 'custom', 'text_recognize_yolo.pt', source='local')
 
         # for every text_class try to recognize text from all areas of text_class, length is depends on class and prod, returns string
 
     def work_image_cuts(self, number_image_cuts, l, h, w):
         """for every text_class try to recognize text from all areas of text_class, length is depends on class and prod, returns string """
-        str = ''
+        (str,conf) = ('', 0.0)
         for number_image_cut in number_image_cuts:
             # cv2.imwrite('data/neuro_classes/cut.jpg', number_image_cut)
-            cur_str = self.work_img_word(number_image_cut, l, h, w)
+            (cur_str, cur_conf) = self.work_img_word(number_image_cut, l, h, w)
             if len(cur_str) == l:
-                return cur_str
+                if cur_conf > conf:
+                    (str, conf) = (cur_str, cur_conf)
             if len(cur_str) > len(str):
-                str = cur_str
-        return str
+                (str, conf) = (cur_str, cur_conf)
+        return (str, conf)
 
         # main_method takes all image_text_areas from image_rama_cut and recognize text
 
     def work_image_cut(self, image_text_areas, image_rama_cut, number_l, number_h, number_w, prod_l, prod_h, prod_w, year_l, year_h, year_w):
         """main_method takes all image_text_areas from image_rama_cut and recognize text"""
         number_image_rects = image_text_areas.areas[Class_text.number]
         number_image_cuts = self.make_cuts(image_rama_cut, number_image_rects)
-        number = self.work_image_cuts(number_image_cuts, number_l, number_h, number_w)
+        (number, number_conf) = self.work_image_cuts(number_image_cuts, number_l, number_h, number_w)
         prod_image_rects = image_text_areas.areas[Class_text.prod]
         prod_image_cuts = self.make_cuts(image_rama_cut, prod_image_rects)
-        prod = self.work_image_cuts(prod_image_cuts, prod_l, prod_h, prod_w)
+        (prod, prod_conf) = self.work_image_cuts(prod_image_cuts, prod_l, prod_h, prod_w)
         year_image_rects = image_text_areas.areas[Class_text.year]
         year_image_cuts = self.make_cuts(image_rama_cut, year_image_rects)
-        year = self.work_image_cuts(year_image_cuts, year_l, year_h, year_w)
+        (year, year_conf) = self.work_image_cuts(year_image_cuts, year_l, year_h, year_w)
         label_area = Label_area()
-        label_area.labels[Class_text.number] = number
-        label_area.labels[Class_text.prod] = prod
-        label_area.labels[Class_text.year] = year
+        label_area.labels[Class_text.number] = (number, number_conf)
+        label_area.labels[Class_text.prod] = (prod, prod_conf)
+        label_area.labels[Class_text.year] = (year, year_conf)
         return label_area
 
     def work_img_word(self, number_image_cut, l, number_h, number_w):
         h, w = number_image_cut.shape[:2]
         hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
         hash_str = hash_object.hexdigest()
         img_cut_path = 'cut_text_img' + hash_str + '.jpg'
@@ -79,15 +80,15 @@
         results = self.model(img_cut_path, size=(number_h, number_w))
         json_res = results.pandas().xyxy[0].to_json(orient="records")
         res2 = json.loads(json_res)
         img_letters = Letters_In_Image.get_letters_in_image_from_yolo_json(res2)
         img_letters.sort_letters()
         img_letters.delete_intersections()
         os.remove(img_cut_path)
-        return img_letters.make_word()
+        return img_letters.make_word(), img_letters.get_avg_conf()
 
 
 
     # cut text_areas imgs for each Rect from rect_array returns openCv imgs list
     def make_cuts(self, img_rama_cut, rect_array):
         """cut text_areas imgs for each Rect from rect_array returns openCv imgs list"""
         number_image_cuts = []
```

### Comparing `danila-lib-1.7.8/data/result/Image_text_areas.py` & `danila-lib-1.7.9/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/data/result/Rect.py` & `danila-lib-1.7.9/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/data/result/Text_area.py` & `danila-lib-1.7.9/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/data/result/Yolo_label_rect.py` & `danila-lib-1.7.9/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.8/setup.py` & `danila-lib-1.7.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.7.8',
+  version='1.7.9',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

