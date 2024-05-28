# Comparing `tmp/eliasliu-0.1.61.tar.gz` & `tmp/eliasliu-0.1.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.61.tar", last modified: Tue May 28 11:48:59 2024, max compression
+gzip compressed data, was "eliasliu-0.1.62.tar", last modified: Tue May 28 14:04:18 2024, max compression
```

## Comparing `eliasliu-0.1.61.tar` & `eliasliu-0.1.62.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 11:48:59.357648 eliasliu-0.1.61/
--rw-rw-rw-   0        0        0     7058 2024-05-28 11:48:59.355649 eliasliu-0.1.61/PKG-INFO
--rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.61/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 11:48:59.144612 eliasliu-0.1.61/elias/
-drwxrwxrwx   0        0        0        0 2024-05-28 11:48:59.256590 eliasliu-0.1.61/elias/Scripts/
--rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/MysqlTool.py
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/__init__.py
--rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/douyin.py
--rw-rw-rw-   0        0        0     1394 2024-05-28 11:48:05.000000 eliasliu-0.1.61/elias/Scripts/image_check.py
--rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/jd.py
--rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/name_in_db.py
--rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/py_clickhouse.py
--rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/vm_clickhouse.py
--rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/Scripts/youdao.py
--rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/__init__.py
--rw-rw-rw-   0        0        0     2278 2024-05-23 02:15:10.000000 eliasliu-0.1.61/elias/ai.py
--rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/check.py
--rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/config_env_variable.py
--rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datamove.py
-drwxrwxrwx   0        0        0        0 2024-05-28 11:48:59.339265 eliasliu-0.1.61/elias/datax/
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/__init__.py
--rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/auto_create_table.py
--rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/job.py
--rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/main.py
--rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/reader.py
--rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/run.py
--rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/datax/writer.py
--rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/etl.py
--rw-rw-rw-   0        0        0    11383 2024-05-28 11:48:20.000000 eliasliu-0.1.61/elias/picture.py
--rw-rw-rw-   0        0        0     1902 2024-05-23 02:58:34.000000 eliasliu-0.1.61/elias/text_similarity.py
--rw-rw-rw-   0        0        0    81060 2024-05-24 08:57:38.000000 eliasliu-0.1.61/elias/usual.py
--rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.61/elias/wechat.py
-drwxrwxrwx   0        0        0        0 2024-05-28 11:48:59.354649 eliasliu-0.1.61/eliasliu.egg-info/
--rw-rw-rw-   0        0        0     7058 2024-05-28 11:48:59.000000 eliasliu-0.1.61/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      754 2024-05-28 11:48:59.000000 eliasliu-0.1.61/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 11:48:59.000000 eliasliu-0.1.61/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2024-05-28 11:48:59.000000 eliasliu-0.1.61/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-28 11:48:59.000000 eliasliu-0.1.61/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 11:48:59.357648 eliasliu-0.1.61/setup.cfg
--rw-rw-rw-   0        0        0     1984 2024-05-28 11:48:35.000000 eliasliu-0.1.61/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:04:18.962723 eliasliu-0.1.62/
+-rw-rw-rw-   0        0        0     7058 2024-05-28 14:04:18.961722 eliasliu-0.1.62/PKG-INFO
+-rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.62/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 14:04:18.941722 eliasliu-0.1.62/elias/
+drwxrwxrwx   0        0        0        0 2024-05-28 14:04:18.949721 eliasliu-0.1.62/elias/Scripts/
+-rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/MysqlTool.py
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/__init__.py
+-rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/douyin.py
+-rw-rw-rw-   0        0        0     1394 2024-05-28 11:48:05.000000 eliasliu-0.1.62/elias/Scripts/image_check.py
+-rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/jd.py
+-rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/name_in_db.py
+-rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/py_clickhouse.py
+-rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/vm_clickhouse.py
+-rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/Scripts/youdao.py
+-rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/__init__.py
+-rw-rw-rw-   0        0        0     2278 2024-05-23 02:15:10.000000 eliasliu-0.1.62/elias/ai.py
+-rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/check.py
+-rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/config_env_variable.py
+-rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datamove.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:04:18.956723 eliasliu-0.1.62/elias/datax/
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/__init__.py
+-rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/auto_create_table.py
+-rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/job.py
+-rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/main.py
+-rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/reader.py
+-rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/run.py
+-rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/datax/writer.py
+-rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/etl.py
+-rw-rw-rw-   0        0        0    11389 2024-05-28 14:03:53.000000 eliasliu-0.1.62/elias/picture.py
+-rw-rw-rw-   0        0        0     1902 2024-05-23 02:58:34.000000 eliasliu-0.1.62/elias/text_similarity.py
+-rw-rw-rw-   0        0        0    81060 2024-05-24 08:57:38.000000 eliasliu-0.1.62/elias/usual.py
+-rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.62/elias/wechat.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:04:18.961722 eliasliu-0.1.62/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0     7058 2024-05-28 14:04:18.000000 eliasliu-0.1.62/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      754 2024-05-28 14:04:18.000000 eliasliu-0.1.62/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 14:04:18.000000 eliasliu-0.1.62/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2024-05-28 14:04:18.000000 eliasliu-0.1.62/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-28 14:04:18.000000 eliasliu-0.1.62/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 14:04:18.962723 eliasliu-0.1.62/setup.cfg
+-rw-rw-rw-   0        0        0     1984 2024-05-28 14:04:01.000000 eliasliu-0.1.62/setup.py
```

### Comparing `eliasliu-0.1.61/PKG-INFO` & `eliasliu-0.1.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.61
+Version: 0.1.62
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.61/README.md` & `eliasliu-0.1.62/README.md`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/Scripts/MysqlTool.py` & `eliasliu-0.1.62/elias/Scripts/MysqlTool.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/Scripts/douyin.py` & `eliasliu-0.1.62/elias/Scripts/douyin.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/Scripts/image_check.py` & `eliasliu-0.1.62/elias/Scripts/image_check.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/Scripts/jd.py` & `eliasliu-0.1.62/elias/Scripts/jd.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/Scripts/name_in_db.py` & `eliasliu-0.1.62/elias/Scripts/name_in_db.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/Scripts/py_clickhouse.py` & `eliasliu-0.1.62/elias/Scripts/py_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/Scripts/vm_clickhouse.py` & `eliasliu-0.1.62/elias/Scripts/vm_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/Scripts/youdao.py` & `eliasliu-0.1.62/elias/Scripts/youdao.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/ai.py` & `eliasliu-0.1.62/elias/ai.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/check.py` & `eliasliu-0.1.62/elias/check.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/config_env_variable.py` & `eliasliu-0.1.62/elias/config_env_variable.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/datamove.py` & `eliasliu-0.1.62/elias/datamove.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/datax/auto_create_table.py` & `eliasliu-0.1.62/elias/datax/auto_create_table.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/datax/job.py` & `eliasliu-0.1.62/elias/datax/job.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/datax/main.py` & `eliasliu-0.1.62/elias/datax/main.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/datax/reader.py` & `eliasliu-0.1.62/elias/datax/reader.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/datax/run.py` & `eliasliu-0.1.62/elias/datax/run.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/datax/writer.py` & `eliasliu-0.1.62/elias/datax/writer.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/etl.py` & `eliasliu-0.1.62/elias/etl.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/picture.py` & `eliasliu-0.1.62/elias/picture.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,12 +310,12 @@
         # 将 A 图片粘贴到 B 图片上
         B.paste(A, (x_offset, y_offset), A)
 
     # 保存合成后的图片
     B.save(output_path)
 
 def image_difference_check(image1, image2):
-    from Scripts import image_check as ic
+    from elias.Scripts import image_check as ic
     diff_count = ic.main(image1, image2)
     return diff_count
```

### Comparing `eliasliu-0.1.61/elias/text_similarity.py` & `eliasliu-0.1.62/elias/text_similarity.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/usual.py` & `eliasliu-0.1.62/elias/usual.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/elias/wechat.py` & `eliasliu-0.1.62/elias/wechat.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.62/eliasliu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.61
+Version: 0.1.62
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eliasliu-0.1.61/eliasliu.egg-info/SOURCES.txt` & `eliasliu-0.1.62/eliasliu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.61/setup.py` & `eliasliu-0.1.62/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.61',  # 版本号
+    version='0.1.62',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     long_description = long_description,
     # long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
     url='https://github.com/tenbj/elias',  # 项目的URL
```

