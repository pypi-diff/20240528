# Comparing `tmp/danila-lib-1.7.9.tar.gz` & `tmp/danila-lib-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.7.9.tar", last modified: Mon May 27 09:59:23 2024, max compression
+gzip compressed data, was "danila-lib-1.8.0.tar", last modified: Tue May 28 08:29:09 2024, max compression
```

## Comparing `danila-lib-1.7.9.tar` & `danila-lib-1.8.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 09:59:23.493369 danila-lib-1.7.9/
--rw-rw-rw-   0        0        0     9615 2024-05-27 09:59:23.492374 danila-lib-1.7.9/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.7.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 09:59:23.444588 danila-lib-1.7.9/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.7.9/danila/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.7.9/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.7.9/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.7.9/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.7.9/danila/danila_v3.py
--rw-rw-rw-   0        0        0    20456 2024-05-27 09:58:57.000000 danila-lib-1.7.9/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-05-27 09:59:23.465494 danila-lib-1.7.9/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-27 09:59:23.000000 danila-lib-1.7.9/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      940 2024-05-27 09:59:23.000000 danila-lib-1.7.9/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 09:59:23.000000 danila-lib-1.7.9/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-27 09:59:23.000000 danila-lib-1.7.9/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-27 09:59:23.000000 danila-lib-1.7.9/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-27 09:59:23.467486 danila-lib-1.7.9/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.7.9/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 09:59:23.479431 danila-lib-1.7.9/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.7.9/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.7.9/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.7.9/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     2982 2024-05-27 08:43:50.000000 danila-lib-1.7.9/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.7.9/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.9/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6607 2024-05-27 09:58:57.000000 danila-lib-1.7.9/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      654 2024-05-22 10:13:34.000000 danila-lib-1.7.9/data/neuro/models.py
--rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.7.9/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4843 2024-05-27 09:58:57.000000 danila-lib-1.7.9/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-27 09:59:23.491378 danila-lib-1.7.9/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.7.9/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.7.9/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.7.9/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.7.9/data/result/Label_area.py
--rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.7.9/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.7.9/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.7.9/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.7.9/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.9/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.7.9/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.7.9/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-27 09:59:23.495363 danila-lib-1.7.9/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-27 09:58:57.000000 danila-lib-1.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:29:09.062759 danila-lib-1.8.0/
+-rw-rw-rw-   0        0        0     9615 2024-05-28 08:29:09.061763 danila-lib-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 08:29:09.014973 danila-lib-1.8.0/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.0/danila/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.8.0/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.0/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.0/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.0/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    20948 2024-05-28 08:28:46.000000 danila-lib-1.8.0/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:29:09.046830 danila-lib-1.8.0/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-28 08:29:08.000000 danila-lib-1.8.0/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2024-05-28 08:29:08.000000 danila-lib-1.8.0/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 08:29:08.000000 danila-lib-1.8.0/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-28 08:29:08.000000 danila-lib-1.8.0/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-28 08:29:08.000000 danila-lib-1.8.0/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 08:29:09.047826 danila-lib-1.8.0/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.0/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:29:09.054794 danila-lib-1.8.0/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.0/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.0/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.0/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.0/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.0/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.0/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6705 2024-05-28 08:02:16.000000 danila-lib-1.8.0/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      654 2024-05-22 10:13:34.000000 danila-lib-1.8.0/data/neuro/models.py
+-rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.0/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4845 2024-05-28 08:02:16.000000 danila-lib-1.8.0/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:29:09.060767 danila-lib-1.8.0/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.0/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.0/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.0/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.0/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.0/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.0/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.0/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.0/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.0/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.0/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.0/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-28 08:29:09.071718 danila-lib-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-28 08:28:46.000000 danila-lib-1.8.0/setup.py
```

### Comparing `danila-lib-1.7.9/PKG-INFO` & `danila-lib-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.7.9
+Version: 1.8.0
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.7.9/README.md` & `danila-lib-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/danila/danila.py` & `danila-lib-1.8.0/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/danila/danila_v1.py` & `danila-lib-1.8.0/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/danila/danila_v2.py` & `danila-lib-1.8.0/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/danila/danila_v3.py` & `danila-lib-1.8.0/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/danila/danila_v4.py` & `danila-lib-1.8.0/danila/danila_v4.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,30 +32,37 @@
 
 class Danila_v4:
     """main class for user"""
     def __init__(self, yolov5_dir):
 
         yolo_path = yolov5_dir
         rama_prod_classify_model_path = RAMA_PROD_CLASSIFY_MODEL_ADDRESS
+        print('reading and loading - RAMA_PROD_CLASSIFY_MODEL')
         self.rama_prod_classify_model = Rama_prod_classify_class(rama_prod_classify_model_path, yolo_path)
         rama_no_spring_detect_model_path = RAMA_BEGICKAYA_DETECT_MODEL_ADDRESS
+        print('reading and loading - RAMA_BEGICKAYA_DETECT_MODEL')
         self.rama_no_spring_detect_model = Rama_detect_class(rama_no_spring_detect_model_path,
                                                              'rama_no_spring_detect', yolo_path)
         rama_spring_detect_model_path = RAMA_RUZHIMMASH_DETECT_MODEL_ADDRESS
+        print('reading and loading - RAMA_RUZHIMMASH_DETECT_MODEL')
         self.rama_spring_detect_model = Rama_detect_class(rama_spring_detect_model_path, 'rama_spring_detect',
                                                              yolo_path)
         rama_spring_ruzhimmash_text_detect_model_path = RAMA_RUZHIMMASH_TEXT_DETECT_MODEL_ADDRESS
+        print('reading and loading - RAMA_RUZHIMMASH_TEXT_DETECT_MODEL')
         self.rama_spring_ruzhimmash_text_detect_model = Text_detect_class(rama_spring_ruzhimmash_text_detect_model_path,
                                                                           'rama_text_ruzhimmash_detect', yolo_path)
         rama_no_spring_bejickaya_text_detect_model_path = RAMA_BEJICKAYA_TEXT_DETECT_MODEL_ADDRESS
+        print('reading and loading - RAMA_BEJICKAYA_TEXT_DETECT_MODEL')
         self.rama_no_spring_bejickaya_text_detect_model = Text_detect_class(rama_no_spring_bejickaya_text_detect_model_path,
                                                                             'rama_text_begickaya_detect', yolo_path)
         text_recognize_yolo_ruzhimmash_model_path = TEXT_RECOGNIZE_RUZHIMMASH_MODEL_ADDRESS
+        print('reading and loading - TEXT_RECOGNIZE_RUZHIMMASH_MODEL')
         self.text_recognize_ruzhimmash_model = Text_Recognize_yolo(text_recognize_yolo_ruzhimmash_model_path, yolo_path)
         text_recognize_yolo_begickaya_model_path = TEXT_RECOGNIZE_BEGICKAYA_MODEL_ADDRESS
+        print('reading and loading - TEXT_RECOGNIZE_BEGICKAYA_MODEL')
         self.text_recognize_begickaya_model = Text_Recognize_yolo(text_recognize_yolo_begickaya_model_path, yolo_path)
 
     # returns Rama_Prod_Conf - class of rama and confidence using CNN network
     # img - openCV frame
     def rama_classify(self, img, size = 256):
         """rama_classify(Img : openCv frame): String - returns class of rama using CNN network"""
         """rama_classify uses Rama_classify_class method - classify(Img)"""
```

### Comparing `danila-lib-1.7.9/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.8.0/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.7.9
+Version: 1.8.0
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.7.9/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.8.0/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/danila_lib.egg-info/requires.txt` & `danila-lib-1.8.0/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/data/neuro/Letters_recognize.py` & `danila-lib-1.8.0/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/data/neuro/Rama_classify_class.py` & `danila-lib-1.8.0/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/data/neuro/Rama_detect_class.py` & `danila-lib-1.8.0/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.8.0/data/neuro/Rama_prod_classify_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,10 +61,10 @@
             return Rama_Prod_Conf(Rama_Prod(2), 0.0)
         else:
             if b_list_r and r_list_r:
                 return Rama_Prod_Conf(Rama_Prod(2), 0.0)
             else:
                 max_conf = image_objs.get_max_conf()
                 if b_list_r:
-                    return Rama_Prod_Conf(Rama_Prod(0), max_conf)
+                    return Rama_Prod_Conf(Rama_Prod(0), round(max_conf,2))
                 else:
-                    return Rama_Prod_Conf(Rama_Prod(1), max_conf)
+                    return Rama_Prod_Conf(Rama_Prod(1), round(max_conf,2))
```

### Comparing `danila-lib-1.7.9/data/neuro/Text_detect_class.py` & `danila-lib-1.8.0/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/data/neuro/letters_in_image.py` & `danila-lib-1.8.0/data/neuro/letters_in_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,19 @@
 
     def get_avg_conf(self):
         sum_conf = 0.0
         count_conf = 0
         for letter in self.letters:
             sum_conf = sum_conf + letter.confidence
             count_conf += 1
-        return sum_conf / count_conf
+        if count_conf==0:
+            res = 0.0
+        else:
+            res = sum_conf / count_conf
+        return round(res, 2)
 
     def __str__(self):
         res = ''
         for letter_in_image in self.letters:
             res = res + letter_in_image.__str__() + '\n'
         return res
```

### Comparing `danila-lib-1.7.9/data/neuro/models.py` & `danila-lib-1.8.0/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/data/neuro/objs_in_image.py` & `danila-lib-1.8.0/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/data/neuro/text_recognize_yolo.py` & `danila-lib-1.8.0/data/neuro/text_recognize_yolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         (str,conf) = ('', 0.0)
         for number_image_cut in number_image_cuts:
             # cv2.imwrite('data/neuro_classes/cut.jpg', number_image_cut)
             (cur_str, cur_conf) = self.work_img_word(number_image_cut, l, h, w)
             if len(cur_str) == l:
                 if cur_conf > conf:
                     (str, conf) = (cur_str, cur_conf)
-            if len(cur_str) > len(str):
+            elif len(cur_str) > len(str):
                 (str, conf) = (cur_str, cur_conf)
         return (str, conf)
 
         # main_method takes all image_text_areas from image_rama_cut and recognize text
 
     def work_image_cut(self, image_text_areas, image_rama_cut, number_l, number_h, number_w, prod_l, prod_h, prod_w, year_l, year_h, year_w):
         """main_method takes all image_text_areas from image_rama_cut and recognize text"""
```

### Comparing `danila-lib-1.7.9/data/result/Image_text_areas.py` & `danila-lib-1.8.0/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/data/result/Rect.py` & `danila-lib-1.8.0/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/data/result/Text_area.py` & `danila-lib-1.8.0/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/data/result/Yolo_label_rect.py` & `danila-lib-1.8.0/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.9/setup.py` & `danila-lib-1.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.7.9',
+  version='1.8.0',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

