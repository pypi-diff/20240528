# Comparing `tmp/eliasliu-0.1.62.tar.gz` & `tmp/eliasliu-0.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.62.tar", last modified: Tue May 28 14:04:18 2024, max compression
+gzip compressed data, was "eliasliu-0.1.63.tar", last modified: Tue May 28 14:28:19 2024, max compression
```

## Comparing `eliasliu-0.1.62.tar` & `eliasliu-0.1.63.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 14:04:18.962723 eliasliu-0.1.62/
--rw-rw-rw-   0        0        0     7058 2024-05-28 14:04:18.961722 eliasliu-0.1.62/PKG-INFO
--rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.62/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 14:04:18.941722 eliasliu-0.1.62/elias/
-drwxrwxrwx   0        0        0        0 2024-05-28 14:04:18.949721 eliasliu-0.1.62/elias/Scripts/
--rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/MysqlTool.py
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/__init__.py
--rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/douyin.py
--rw-rw-rw-   0        0        0     1394 2024-05-28 11:48:05.000000 eliasliu-0.1.62/elias/Scripts/image_check.py
--rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/jd.py
--rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/name_in_db.py
--rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/py_clickhouse.py
--rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/vm_clickhouse.py
--rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/youdao.py
--rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/__init__.py
--rw-rw-rw-   0        0        0     2278 2024-05-23 02:15:10.000000 eliasliu-0.1.62/elias/ai.py
--rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/check.py
--rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/config_env_variable.py
--rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datamove.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:04:18.956723 eliasliu-0.1.62/elias/datax/
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/__init__.py
--rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/auto_create_table.py
--rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/job.py
--rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/main.py
--rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/reader.py
--rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/run.py
--rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/writer.py
--rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/etl.py
--rw-rw-rw-   0        0        0    11389 2024-05-28 14:03:53.000000 eliasliu-0.1.62/elias/picture.py
--rw-rw-rw-   0        0        0     1902 2024-05-23 02:58:34.000000 eliasliu-0.1.62/elias/text_similarity.py
--rw-rw-rw-   0        0        0    81060 2024-05-24 08:57:38.000000 eliasliu-0.1.62/elias/usual.py
--rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/wechat.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:04:18.961722 eliasliu-0.1.62/eliasliu.egg-info/
--rw-rw-rw-   0        0        0     7058 2024-05-28 14:04:18.000000 eliasliu-0.1.62/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      754 2024-05-28 14:04:18.000000 eliasliu-0.1.62/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 14:04:18.000000 eliasliu-0.1.62/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2024-05-28 14:04:18.000000 eliasliu-0.1.62/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-28 14:04:18.000000 eliasliu-0.1.62/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 14:04:18.962723 eliasliu-0.1.62/setup.cfg
--rw-rw-rw-   0        0        0     1984 2024-05-28 14:04:01.000000 eliasliu-0.1.62/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:28:19.283278 eliasliu-0.1.63/
+-rw-rw-rw-   0        0        0     7058 2024-05-28 14:28:19.282278 eliasliu-0.1.63/PKG-INFO
+-rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.63/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 14:28:19.057777 eliasliu-0.1.63/elias/
+drwxrwxrwx   0        0        0        0 2024-05-28 14:28:19.180776 eliasliu-0.1.63/elias/Scripts/
+-rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/Scripts/MysqlTool.py
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/Scripts/__init__.py
+-rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/Scripts/douyin.py
+-rw-rw-rw-   0        0        0     1394 2024-05-28 11:48:05.000000 eliasliu-0.1.63/elias/Scripts/image_check.py
+-rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/Scripts/jd.py
+-rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/Scripts/name_in_db.py
+-rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/Scripts/py_clickhouse.py
+-rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/Scripts/vm_clickhouse.py
+-rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/Scripts/youdao.py
+-rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/__init__.py
+-rw-rw-rw-   0        0        0     2278 2024-05-23 02:15:10.000000 eliasliu-0.1.63/elias/ai.py
+-rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/check.py
+-rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/config_env_variable.py
+-rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/datamove.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:28:19.262357 eliasliu-0.1.63/elias/datax/
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/datax/__init__.py
+-rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/datax/auto_create_table.py
+-rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/datax/job.py
+-rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/datax/main.py
+-rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/datax/reader.py
+-rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/datax/run.py
+-rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/datax/writer.py
+-rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/etl.py
+-rw-rw-rw-   0        0        0    12061 2024-05-28 14:27:41.000000 eliasliu-0.1.63/elias/picture.py
+-rw-rw-rw-   0        0        0     1902 2024-05-23 02:58:34.000000 eliasliu-0.1.63/elias/text_similarity.py
+-rw-rw-rw-   0        0        0    81060 2024-05-24 08:57:38.000000 eliasliu-0.1.63/elias/usual.py
+-rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.63/elias/wechat.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:28:19.281279 eliasliu-0.1.63/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0     7058 2024-05-28 14:28:18.000000 eliasliu-0.1.63/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      754 2024-05-28 14:28:18.000000 eliasliu-0.1.63/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 14:28:18.000000 eliasliu-0.1.63/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2024-05-28 14:28:18.000000 eliasliu-0.1.63/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-28 14:28:18.000000 eliasliu-0.1.63/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 14:28:19.283278 eliasliu-0.1.63/setup.cfg
+-rw-rw-rw-   0        0        0     1984 2024-05-28 14:28:04.000000 eliasliu-0.1.63/setup.py
```

### Comparing `eliasliu-0.1.62/PKG-INFO` & `eliasliu-0.1.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.62
+Version: 0.1.63
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.62/README.md` & `eliasliu-0.1.63/README.md`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/Scripts/MysqlTool.py` & `eliasliu-0.1.63/elias/Scripts/MysqlTool.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/Scripts/douyin.py` & `eliasliu-0.1.63/elias/Scripts/douyin.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/Scripts/image_check.py` & `eliasliu-0.1.63/elias/Scripts/image_check.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/Scripts/jd.py` & `eliasliu-0.1.63/elias/Scripts/jd.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/Scripts/name_in_db.py` & `eliasliu-0.1.63/elias/Scripts/name_in_db.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/Scripts/py_clickhouse.py` & `eliasliu-0.1.63/elias/Scripts/py_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/Scripts/vm_clickhouse.py` & `eliasliu-0.1.63/elias/Scripts/vm_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/Scripts/youdao.py` & `eliasliu-0.1.63/elias/Scripts/youdao.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/ai.py` & `eliasliu-0.1.63/elias/ai.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/check.py` & `eliasliu-0.1.63/elias/check.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/config_env_variable.py` & `eliasliu-0.1.63/elias/config_env_variable.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/datamove.py` & `eliasliu-0.1.63/elias/datamove.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/datax/auto_create_table.py` & `eliasliu-0.1.63/elias/datax/auto_create_table.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/datax/job.py` & `eliasliu-0.1.63/elias/datax/job.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/datax/main.py` & `eliasliu-0.1.63/elias/datax/main.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/datax/reader.py` & `eliasliu-0.1.63/elias/datax/reader.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/datax/run.py` & `eliasliu-0.1.63/elias/datax/run.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/datax/writer.py` & `eliasliu-0.1.63/elias/datax/writer.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/etl.py` & `eliasliu-0.1.63/elias/etl.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/picture.py` & `eliasliu-0.1.63/elias/picture.py`

 * *Files 4% similar despite different names*

```diff
@@ -251,14 +251,17 @@
     else:
         avg_usetime = str(round((end-start)/new_pic_num, 2))+ ' seconds'
     logger.info(f"\n共计{folder_num}个文件夹，{pic_num}张图片\n\n新文件夹：{new_folder_num} ；老文件夹：{old_folder_num}\n新图片数：{new_pic_num} ；老图片数：{old_pic_num}\n\n总共用时：{usetime} ； 平均每图：{avg_usetime}")
 
 
 
 
+# A_path = 'E:\\头条发布\\logo.jpg'
+# B_path = 'E:\\头条发布\\待发头条\\【学者启智】“央视陈世美”水均益抛妻弃女？因娶小13岁美娇妻背负无数骂名\\origin\\9.jpg'
+# output_path = 'E:\\头条发布\\待发头条\\【学者启智】“央视陈世美”水均益抛妻弃女？因娶小13岁美娇妻背负无数骂名\\9.jpg'
 
 
 
 def merge_images(A_path, B_path, output_path, num_times=5):
     '''
     # # 示例用法
     # A_path = "A.png"  # 图片 A 的路径
@@ -294,14 +297,22 @@
     # 确保图片 A 的模式为 RGBA
     if A.mode != "RGBA":
         A = A.convert("RGBA")
 
     # 降低 A 图片的透明度到最低
     A = A.point(lambda p: p * 0.001)
 
+
+    # 获取 A 图片的宽度和高度
+    A_width, A_height = A.size
+
+    # 如果 B 图片的宽度或高度小于 A 图片，则将 B 图片等比例缩小一半，直到比 A 大为止
+    while B.width < A_width or B.height < A_height:
+        B = B.resize((B.width * 2, B.height * 2))
+
     # 获取 B 图片的宽度和高度
     B_width, B_height = B.size
 
     # 在 B 图片上随机添加 A 图片
     for _ in range(num_times):
         # 随机生成 A 图片的位置
         x_offset = random.randint(0, B_width - A.width)
```

### Comparing `eliasliu-0.1.62/elias/text_similarity.py` & `eliasliu-0.1.63/elias/text_similarity.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/usual.py` & `eliasliu-0.1.63/elias/usual.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/elias/wechat.py` & `eliasliu-0.1.63/elias/wechat.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.63/eliasliu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.62
+Version: 0.1.63
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.62/eliasliu.egg-info/SOURCES.txt` & `eliasliu-0.1.63/eliasliu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.62/setup.py` & `eliasliu-0.1.63/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.62',  # 版本号
+    version='0.1.63',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     long_description = long_description,
     # long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
     url='https://github.com/tenbj/elias',  # 项目的URL
```

