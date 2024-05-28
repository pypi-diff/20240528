# Comparing `tmp/DXR_BJ-1.0.5.tar.gz` & `tmp/DXR_BJ-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR_BJ-1.0.5.tar", last modified: Tue Apr 23 09:10:52 2024, max compression
+gzip compressed data, was "DXR_BJ-1.0.6.tar", last modified: Tue May 28 06:39:15 2024, max compression
```

## Comparing `DXR_BJ-1.0.5.tar` & `DXR_BJ-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 09:10:52.728490 DXR_BJ-1.0.5/
-drwxrwxrwx   0        0        0        0 2024-04-23 09:10:52.670646 DXR_BJ-1.0.5/DXR_BJ/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:08:38.000000 DXR_BJ-1.0.5/DXR_BJ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:10:52.650696 DXR_BJ-1.0.5/DXR_BJ/common/
-drwxrwxrwx   0        0        0        0 2024-04-23 09:10:52.691590 DXR_BJ-1.0.5/DXR_BJ/common/dependency/
--rw-rw-rw-   0        0        0 10500792 2023-12-04 08:46:42.000000 DXR_BJ-1.0.5/DXR_BJ/common/dependency/simsun.ttc
--rw-rw-rw-   0        0        0    34404 2024-04-23 09:09:29.000000 DXR_BJ-1.0.5/DXR_BJ/drawer.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:10:52.690592 DXR_BJ-1.0.5/DXR_BJ.egg-info/
--rw-rw-rw-   0        0        0      183 2024-04-23 09:10:52.000000 DXR_BJ-1.0.5/DXR_BJ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-23 09:10:52.000000 DXR_BJ-1.0.5/DXR_BJ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 09:10:52.000000 DXR_BJ-1.0.5/DXR_BJ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-23 09:10:52.000000 DXR_BJ-1.0.5/DXR_BJ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 09:10:52.000000 DXR_BJ-1.0.5/DXR_BJ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       66 2024-04-16 01:18:00.000000 DXR_BJ-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      183 2024-04-23 09:10:52.726496 DXR_BJ-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-23 09:10:52.728490 DXR_BJ-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1766 2024-04-23 09:10:25.000000 DXR_BJ-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:10:52.725499 DXR_BJ-1.0.5/tests/
--rw-rw-rw-   0        0        0     1068 2024-04-22 02:24:43.000000 DXR_BJ-1.0.5/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:39:15.616474 DXR_BJ-1.0.6/
+drwxrwxrwx   0        0        0        0 2024-05-28 06:39:15.405214 DXR_BJ-1.0.6/DXR_BJ/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:08:38.000000 DXR_BJ-1.0.6/DXR_BJ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:39:15.374333 DXR_BJ-1.0.6/DXR_BJ/common/
+drwxrwxrwx   0        0        0        0 2024-05-28 06:39:15.580575 DXR_BJ-1.0.6/DXR_BJ/common/dependency/
+-rw-rw-rw-   0        0        0 10500792 2023-12-04 08:46:42.000000 DXR_BJ-1.0.6/DXR_BJ/common/dependency/simsun.ttc
+-rw-rw-rw-   0        0        0    35483 2024-05-28 06:33:15.000000 DXR_BJ-1.0.6/DXR_BJ/drawer.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:39:15.447262 DXR_BJ-1.0.6/DXR_BJ.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-05-28 06:39:14.000000 DXR_BJ-1.0.6/DXR_BJ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-05-28 06:39:14.000000 DXR_BJ-1.0.6/DXR_BJ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 06:39:14.000000 DXR_BJ-1.0.6/DXR_BJ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-28 06:39:14.000000 DXR_BJ-1.0.6/DXR_BJ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 06:39:14.000000 DXR_BJ-1.0.6/DXR_BJ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       66 2024-04-16 01:18:00.000000 DXR_BJ-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      193 2024-05-28 06:39:15.615477 DXR_BJ-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-28 06:39:15.617472 DXR_BJ-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1776 2024-05-28 06:36:14.000000 DXR_BJ-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 06:39:15.613482 DXR_BJ-1.0.6/tests/
+-rw-rw-rw-   0        0        0     1070 2024-04-29 07:36:16.000000 DXR_BJ-1.0.6/tests/test.py
```

### Comparing `DXR_BJ-1.0.5/DXR_BJ/common/dependency/simsun.ttc` & `DXR_BJ-1.0.6/DXR_BJ/common/dependency/simsun.ttc`

 * *Files identical despite different names*

### Comparing `DXR_BJ-1.0.5/DXR_BJ/drawer.py` & `DXR_BJ-1.0.6/DXR_BJ/drawer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# @Time    : 2024/04/23
+# @Time    : 2024/05/28
 # @Author  : zx
 # @File    : Drawer.py
-# @Version : 1.0.5
+# @Version : 1.0.6
 
 
 
 import copy
 import os
 import cv2
 import numpy as np
 import math
 import freetype   ## Freetypechinese
 import traceback  ## log
 
 
 ###全局变量
-Version_num='1.0.5'     ###版本号
+Version_num='1.0.6'     ###版本号
 py_path=os.path.dirname(os.path.abspath(__file__))   ##字体路径
                               
 alg_name = { 
     "smoke": "烟雾",
     "fire": "火焰",
     "person": "行人",
     "car": "车",
@@ -419,15 +419,15 @@
                     self.labelcolor = self.red
 
                 outimg = self.labelclass.DrawChinesename(outimg, name, position, self.rectcolor, self.labelcolor)
 
         ### 常规目标标记
         targettypes = ["SmogFire", "Person", "IRPerson", "Sand", "Door", 'FireHydrant', "EQ", 'PersonandFace', \
                        "Car", 'Doorwindow', 'MeterBox', 'ChemicalDrip', 'Hat', 'Pothole', 'SamllPersonCar', \
-                       'Facelocal', 'LPRlocal', 'SmokeFire']
+                       'Facelocal', 'LPRlocal', 'SmokeFire',"YoloWorld","WorldRanging","RetinaFace","arcface"]
         if message["sType"] in targettypes:
             warningstate = ['smoke', 'fire', 'person', 'open', 'car', 'no_hat', 'Pothole']
             for num, target_rect in enumerate(rects):
                 if message["sType"] == 'PersonandFace':  ##行人人脸会出现行人框和人脸框数目不一致现象，故单独处理成person
                     name = 'person'
                 else:
                     name = texts[num][0]
@@ -444,17 +444,26 @@
                 except Exception as e:
                     zh_name = name
                 iX = int(target_rect[0])
                 iY = int(target_rect[1])
                 iW = int(target_rect[2])
                 iH = int(target_rect[3])
                 position = (iX, iY, iX + iW, iY + iH)
-
+                if message["sType"]=="arcface":
+                    zh_name = name
                 outimg = self.labelclass.DrawChinesename(outimg, zh_name, position, self.rectcolor, self.labelcolor)
 
+
+        ##功能38单独处理
+        if message["sType"]=='workwear':
+            for bbox in rects:
+                #         print(bbox)
+                x, y, w, h, conf = bbox
+                outimg=cv2.rectangle(outimg, (int(x), int(y)), (int(x + w), int(y + h)), (128, 0, 128), 2)  ##紫色框标记工装
+
         return outimg
 
     def label_region_message(self, outimg, message):
 
         if message['sType'] == 'FireHydrant' or message['sType'] == 'ChemicalDrip' or message[
             'sType'] == 'IndoorFlooding':
             ## 循环region 进行标记
@@ -530,14 +539,28 @@
                 labelnum = int(track_rect[4])
 
                 position = (iX, iY, iX + iW, iY + iH)
                 outimg = self.labelclass.DrawChinesename(outimg, name, position, self.rectcolor, self.labelcolor)
                 cv2.putText(outimg, str(labelnum), (iX + iW - 50, iY), self.font, self.fontScale, self.red,
                             2 * self.thickness)
 
+        if message["sType"] == 'workwear':
+            for num, bbox in enumerate(tracks):
+                if texts[num] == 'warning':
+                    color = (0, 0, 255)
+                elif texts[num] == 'ok':
+                    color = (0, 255, 0)
+                else:
+                    color = (0, 255, 255)
+                x, y, w, h, label = bbox
+                cv2.rectangle(outimg, (int(x), int(y)), (int(x + w), int(y + h)), color, 2)
+                ##红色标记行人
+                cv2.putText(outimg, str(label), (int(x), int(y) - 5), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0, 0, 255), 3)
+
+
         return outimg
 
     def label_line_message(self, outimg, message):
         lines = list(message['lResults']["line"])
         sValues = list(message['lResults']["text"])
         if message["sType"] == 'Mesh':
             for num, target_line in enumerate(lines):
```

### Comparing `DXR_BJ-1.0.5/setup.py` & `DXR_BJ-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup,find_packages
 setup(
   name='DXR_BJ',      ##from 引入的名称
-  version='1.0.5',    ##发布的版本号
-  description='删除lResults中的sValue',
+  version='1.0.6',    ##发布的版本号
+  description='增加算法新人脸及工装标记',
   author='zx',
   author_email='450125770@qq.com',
   install_requires= ["freetype-py"], # 定义依赖哪些模块
   packages=find_packages(),  # 系统自动从当前目录开始找包
   include_package_data=True,
   # 如果有的文件不用打包，则只能指定需要打包的文件
   #packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
```

### Comparing `DXR_BJ-1.0.5/tests/test.py` & `DXR_BJ-1.0.6/tests/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 from DXR_BJ import drawer
 
 import cv2
 import time
-draw=drawer.Drawer()
+draw=drawer.Drawer('./')
 img=cv2.imread('1.jpg')
 res={'10': {'error': False, 'bFlag': True, 'bState': True, 'sType': 'IRPerson', 'cnType': '热成像行人检测', 'sValue': '1', 'lResults': {'rect': [[0.4, 0.001851851851851852, 0.515625, 0.9944444444444445, 0.557663]], 'track': [], 'region': [], 'line': [], 'point': [], 'text': [['person']], 'sValue': '1', 'res_key': 'rect'}}, '17': {'error': False, 'bFlag': True, 'bState': False, 'sType': 'HKIR', 'cnType': '温度监控', 'sValue': '0', 'lResults': {'rect': [], 'track': [], 'region': [], 'line': [], 'point': [], 'text': [], 'sValue': '', 'res_key': 'rect'}}}
 
 while True:
     num=0
     for key, value in res.items():
         outmessage=value
         t1=time.time()
         outframe,_= draw.draw_frame_box(img, outmessage)
         if num != 0:
             frame = outframe.copy()   ##多算法标记类兼容
-        print(f'标记时间:{1000*(time.time()-t1)}')
-        # cv2.imshow('1',outframe)
-        # cv2.waitKey(10) 
+        # print(f'标记时间:{1000*(time.time()-t1)}')
+        cv2.imshow('1',outframe)
+        cv2.waitKey(10) 
         num=num+1
```

