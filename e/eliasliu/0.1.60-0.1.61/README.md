# Comparing `tmp/eliasliu-0.1.60.tar.gz` & `tmp/eliasliu-0.1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.60.tar", last modified: Fri May 24 09:12:32 2024, max compression
+gzip compressed data, was "eliasliu-0.1.61.tar", last modified: Tue May 28 11:48:59 2024, max compression
```

## Comparing `eliasliu-0.1.60.tar` & `eliasliu-0.1.61.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 09:12:32.101641 eliasliu-0.1.60/
--rw-rw-rw-   0        0        0     7058 2024-05-24 09:12:32.100642 eliasliu-0.1.60/PKG-INFO
--rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.60/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 09:12:31.827056 eliasliu-0.1.60/elias/
-drwxrwxrwx   0        0        0        0 2024-05-24 09:12:31.930886 eliasliu-0.1.60/elias/Scripts/
--rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/MysqlTool.py
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/__init__.py
--rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/douyin.py
--rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/jd.py
--rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/name_in_db.py
--rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/py_clickhouse.py
--rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/vm_clickhouse.py
--rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/Scripts/youdao.py
--rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/__init__.py
--rw-rw-rw-   0        0        0     2278 2024-05-23 02:15:10.000000 eliasliu-0.1.60/elias/ai.py
--rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/check.py
--rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/config_env_variable.py
--rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datamove.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:12:32.079650 eliasliu-0.1.60/elias/datax/
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/__init__.py
--rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/auto_create_table.py
--rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/job.py
--rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/main.py
--rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/reader.py
--rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/run.py
--rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/datax/writer.py
--rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/etl.py
--rw-rw-rw-   0        0        0     9840 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/picture.py
--rw-rw-rw-   0        0        0     1902 2024-05-23 02:58:34.000000 eliasliu-0.1.60/elias/text_similarity.py
--rw-rw-rw-   0        0        0    81060 2024-05-24 08:57:38.000000 eliasliu-0.1.60/elias/usual.py
--rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.60/elias/wechat.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:12:32.099642 eliasliu-0.1.60/eliasliu.egg-info/
--rw-rw-rw-   0        0        0     7058 2024-05-24 09:12:31.000000 eliasliu-0.1.60/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      725 2024-05-24 09:12:31.000000 eliasliu-0.1.60/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 09:12:31.000000 eliasliu-0.1.60/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2024-05-24 09:12:31.000000 eliasliu-0.1.60/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-24 09:12:31.000000 eliasliu-0.1.60/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 09:12:32.102643 eliasliu-0.1.60/setup.cfg
--rw-rw-rw-   0        0        0     1984 2024-05-24 08:58:12.000000 eliasliu-0.1.60/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:48:59.357648 eliasliu-0.1.61/
+-rw-rw-rw-   0        0        0     7058 2024-05-28 11:48:59.355649 eliasliu-0.1.61/PKG-INFO
+-rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.61/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 11:48:59.144612 eliasliu-0.1.61/elias/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:48:59.256590 eliasliu-0.1.61/elias/Scripts/
+-rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/MysqlTool.py
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/__init__.py
+-rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/douyin.py
+-rw-rw-rw-   0        0        0     1394 2024-05-28 11:48:05.000000 eliasliu-0.1.61/elias/Scripts/image_check.py
+-rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/jd.py
+-rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/name_in_db.py
+-rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/py_clickhouse.py
+-rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/vm_clickhouse.py
+-rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/youdao.py
+-rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/__init__.py
+-rw-rw-rw-   0        0        0     2278 2024-05-23 02:15:10.000000 eliasliu-0.1.61/elias/ai.py
+-rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/check.py
+-rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/config_env_variable.py
+-rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datamove.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:48:59.339265 eliasliu-0.1.61/elias/datax/
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/__init__.py
+-rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/auto_create_table.py
+-rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/job.py
+-rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/main.py
+-rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/reader.py
+-rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/run.py
+-rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/writer.py
+-rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/etl.py
+-rw-rw-rw-   0        0        0    11383 2024-05-28 11:48:20.000000 eliasliu-0.1.61/elias/picture.py
+-rw-rw-rw-   0        0        0     1902 2024-05-23 02:58:34.000000 eliasliu-0.1.61/elias/text_similarity.py
+-rw-rw-rw-   0        0        0    81060 2024-05-24 08:57:38.000000 eliasliu-0.1.61/elias/usual.py
+-rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/wechat.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:48:59.354649 eliasliu-0.1.61/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0     7058 2024-05-28 11:48:59.000000 eliasliu-0.1.61/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      754 2024-05-28 11:48:59.000000 eliasliu-0.1.61/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 11:48:59.000000 eliasliu-0.1.61/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2024-05-28 11:48:59.000000 eliasliu-0.1.61/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-28 11:48:59.000000 eliasliu-0.1.61/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 11:48:59.357648 eliasliu-0.1.61/setup.cfg
+-rw-rw-rw-   0        0        0     1984 2024-05-28 11:48:35.000000 eliasliu-0.1.61/setup.py
```

### Comparing `eliasliu-0.1.60/PKG-INFO` & `eliasliu-0.1.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.60
+Version: 0.1.61
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.60/README.md` & `eliasliu-0.1.61/README.md`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/Scripts/MysqlTool.py` & `eliasliu-0.1.61/elias/Scripts/MysqlTool.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/Scripts/douyin.py` & `eliasliu-0.1.61/elias/Scripts/douyin.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/Scripts/jd.py` & `eliasliu-0.1.61/elias/Scripts/jd.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/Scripts/name_in_db.py` & `eliasliu-0.1.61/elias/Scripts/name_in_db.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/Scripts/py_clickhouse.py` & `eliasliu-0.1.61/elias/Scripts/py_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/Scripts/vm_clickhouse.py` & `eliasliu-0.1.61/elias/Scripts/vm_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/Scripts/youdao.py` & `eliasliu-0.1.61/elias/Scripts/youdao.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/ai.py` & `eliasliu-0.1.61/elias/ai.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/check.py` & `eliasliu-0.1.61/elias/check.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/config_env_variable.py` & `eliasliu-0.1.61/elias/config_env_variable.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/datamove.py` & `eliasliu-0.1.61/elias/datamove.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/datax/auto_create_table.py` & `eliasliu-0.1.61/elias/datax/auto_create_table.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/datax/job.py` & `eliasliu-0.1.61/elias/datax/job.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/datax/main.py` & `eliasliu-0.1.61/elias/datax/main.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/datax/reader.py` & `eliasliu-0.1.61/elias/datax/reader.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/datax/run.py` & `eliasliu-0.1.61/elias/datax/run.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/datax/writer.py` & `eliasliu-0.1.61/elias/datax/writer.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/etl.py` & `eliasliu-0.1.61/elias/etl.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/picture.py` & `eliasliu-0.1.61/elias/picture.py`

 * *Files 17% similar despite different names*

```diff
@@ -248,7 +248,74 @@
     usetime = str(round(end-start, 2))+ ' seconds'
     if new_pic_num == 0:
         avg_usetime = '0.00 seconds'
     else:
         avg_usetime = str(round((end-start)/new_pic_num, 2))+ ' seconds'
     logger.info(f"\n共计{folder_num}个文件夹，{pic_num}张图片\n\n新文件夹：{new_folder_num} ；老文件夹：{old_folder_num}\n新图片数：{new_pic_num} ；老图片数：{old_pic_num}\n\n总共用时：{usetime} ； 平均每图：{avg_usetime}")
 
+
+
+
+
+
+
+def merge_images(A_path, B_path, output_path, num_times=5):
+    '''
+    # # 示例用法
+    # A_path = "A.png"  # 图片 A 的路径
+    # B_path = "B.png"  # 图片 B 的路径
+    # output_path = "output.png"  # 合成后的图片路径
+
+    # merge_images(A_path, B_path, output_path)
+
+    Parameters
+    ----------
+    A_path : TYPE
+        DESCRIPTION.
+    B_path : TYPE
+        DESCRIPTION.
+    output_path : TYPE
+        DESCRIPTION.
+    num_times : TYPE, optional
+        DESCRIPTION. The default is 5.
+
+    Returns
+    -------
+    None.
+
+    '''
+    
+    import random
+    from PIL import Image
+    
+    # 打开图片 A 和 B
+    A = Image.open(A_path)
+    B = Image.open(B_path)
+
+    # 确保图片 A 的模式为 RGBA
+    if A.mode != "RGBA":
+        A = A.convert("RGBA")
+
+    # 降低 A 图片的透明度到最低
+    A = A.point(lambda p: p * 0.001)
+
+    # 获取 B 图片的宽度和高度
+    B_width, B_height = B.size
+
+    # 在 B 图片上随机添加 A 图片
+    for _ in range(num_times):
+        # 随机生成 A 图片的位置
+        x_offset = random.randint(0, B_width - A.width)
+        y_offset = random.randint(0, B_height - A.height)
+
+        # 将 A 图片粘贴到 B 图片上
+        B.paste(A, (x_offset, y_offset), A)
+
+    # 保存合成后的图片
+    B.save(output_path)
+
+def image_difference_check(image1, image2):
+    from Scripts import image_check as ic
+    diff_count = ic.main(image1, image2)
+    return diff_count
+    
+
```

### Comparing `eliasliu-0.1.60/elias/text_similarity.py` & `eliasliu-0.1.61/elias/text_similarity.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/usual.py` & `eliasliu-0.1.61/elias/usual.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/elias/wechat.py` & `eliasliu-0.1.61/elias/wechat.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.60/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.61/eliasliu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.60
+Version: 0.1.61
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.60/eliasliu.egg-info/SOURCES.txt` & `eliasliu-0.1.61/eliasliu.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 elias/picture.py
 elias/text_similarity.py
 elias/usual.py
 elias/wechat.py
 elias/Scripts/MysqlTool.py
 elias/Scripts/__init__.py
 elias/Scripts/douyin.py
+elias/Scripts/image_check.py
 elias/Scripts/jd.py
 elias/Scripts/name_in_db.py
 elias/Scripts/py_clickhouse.py
 elias/Scripts/vm_clickhouse.py
 elias/Scripts/youdao.py
 elias/datax/__init__.py
 elias/datax/auto_create_table.py
```

### Comparing `eliasliu-0.1.60/setup.py` & `eliasliu-0.1.61/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.60',  # 版本号
+    version='0.1.61',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     long_description = long_description,
     # long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
     url='https://github.com/tenbj/elias',  # 项目的URL
```

