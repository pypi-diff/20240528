# Comparing `tmp/blue_media-0.0.2.tar.gz` & `tmp/blue_media-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue_media-0.0.2.tar", last modified: Wed Jan 10 10:11:20 2024, max compression
+gzip compressed data, was "blue_media-0.0.3.tar", last modified: Tue May 28 09:19:46 2024, max compression
```

## Comparing `blue_media-0.0.2.tar` & `blue_media-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-01-10 10:11:20.573724 blue_media-0.0.2/
--rw-r--r--   0 a08030320   (501) staff       (20)     1073 2024-01-09 12:07:09.000000 blue_media-0.0.2/LICENSE
--rw-r--r--   0 a08030320   (501) staff       (20)      982 2024-01-10 10:11:20.573393 blue_media-0.0.2/PKG-INFO
--rw-r--r--   0 a08030320   (501) staff       (20)      492 2024-01-09 12:31:06.000000 blue_media-0.0.2/README.md
-drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-01-10 10:11:20.572069 blue_media-0.0.2/blue_media/
--rw-r--r--   0 a08030320   (501) staff       (20)     3692 2024-01-10 10:10:40.000000 blue_media-0.0.2/blue_media/BlueClass.py
--rw-r--r--   0 a08030320   (501) staff       (20)        0 2024-01-09 10:03:21.000000 blue_media-0.0.2/blue_media/__init__.py
-drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-01-10 10:11:20.573096 blue_media-0.0.2/blue_media.egg-info/
--rw-r--r--   0 a08030320   (501) staff       (20)      982 2024-01-10 10:11:20.000000 blue_media-0.0.2/blue_media.egg-info/PKG-INFO
--rw-r--r--   0 a08030320   (501) staff       (20)      242 2024-01-10 10:11:20.000000 blue_media-0.0.2/blue_media.egg-info/SOURCES.txt
--rw-r--r--   0 a08030320   (501) staff       (20)        1 2024-01-10 10:11:20.000000 blue_media-0.0.2/blue_media.egg-info/dependency_links.txt
--rw-r--r--   0 a08030320   (501) staff       (20)       53 2024-01-10 10:11:20.000000 blue_media-0.0.2/blue_media.egg-info/requires.txt
--rw-r--r--   0 a08030320   (501) staff       (20)       11 2024-01-10 10:11:20.000000 blue_media-0.0.2/blue_media.egg-info/top_level.txt
--rw-r--r--   0 a08030320   (501) staff       (20)       38 2024-01-10 10:11:20.573783 blue_media-0.0.2/setup.cfg
--rw-r--r--   0 a08030320   (501) staff       (20)     1342 2024-01-10 10:10:40.000000 blue_media-0.0.2/setup.py
+drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-28 09:19:46.047110 blue_media-0.0.3/
+-rw-r--r--   0 a08030320   (501) staff       (20)     1073 2024-01-09 12:07:09.000000 blue_media-0.0.3/LICENSE
+-rw-r--r--   0 a08030320   (501) staff       (20)      982 2024-05-28 09:19:46.046853 blue_media-0.0.3/PKG-INFO
+-rw-r--r--   0 a08030320   (501) staff       (20)      492 2024-01-09 12:31:06.000000 blue_media-0.0.3/README.md
+drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-28 09:19:46.044698 blue_media-0.0.3/blue_media/
+-rw-r--r--   0 a08030320   (501) staff       (20)     3692 2024-01-10 10:10:40.000000 blue_media-0.0.3/blue_media/BlueClass.py
+-rw-r--r--   0 a08030320   (501) staff       (20)        0 2024-01-09 10:03:21.000000 blue_media-0.0.3/blue_media/__init__.py
+drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-28 09:19:46.046591 blue_media-0.0.3/blue_media.egg-info/
+-rw-r--r--   0 a08030320   (501) staff       (20)      982 2024-05-28 09:19:45.000000 blue_media-0.0.3/blue_media.egg-info/PKG-INFO
+-rw-r--r--   0 a08030320   (501) staff       (20)      242 2024-05-28 09:19:46.000000 blue_media-0.0.3/blue_media.egg-info/SOURCES.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)        1 2024-05-28 09:19:45.000000 blue_media-0.0.3/blue_media.egg-info/dependency_links.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)       53 2024-05-28 09:19:45.000000 blue_media-0.0.3/blue_media.egg-info/requires.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)       11 2024-05-28 09:19:45.000000 blue_media-0.0.3/blue_media.egg-info/top_level.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)       38 2024-05-28 09:19:46.047444 blue_media-0.0.3/setup.cfg
+-rw-r--r--   0 a08030320   (501) staff       (20)     1342 2024-05-28 09:15:48.000000 blue_media-0.0.3/setup.py
```

### Comparing `blue_media-0.0.2/LICENSE` & `blue_media-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blue_media-0.0.2/PKG-INFO` & `blue_media-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: blue_media
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper of the api logic used to interact with blue_media.
 Home-page: 
 Author: ranyu
 Author-email: wy176404@163.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp>=3.9.1
+Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: aiosignal>=1.3.1
 Requires-Dist: async-timeout>=4.0.3
 
 # What is it?
 
 > A wrapper of the api logic used to interact with blue_media.
```

### Comparing `blue_media-0.0.2/blue_media/BlueClass.py` & `blue_media-0.0.3/blue_media/BlueClass.py`

 * *Files identical despite different names*

### Comparing `blue_media-0.0.2/blue_media.egg-info/PKG-INFO` & `blue_media-0.0.3/blue_media.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: blue_media
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper of the api logic used to interact with blue_media.
 Home-page: 
 Author: ranyu
 Author-email: wy176404@163.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp>=3.9.1
+Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: aiosignal>=1.3.1
 Requires-Dist: async-timeout>=4.0.3
 
 # What is it?
 
 > A wrapper of the api logic used to interact with blue_media.
```

### Comparing `blue_media-0.0.2/setup.py` & `blue_media-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="blue_media",
-    version="0.0.2",
+    version="0.0.3",
     # 作者名
     author="ranyu",
     # 作者邮箱
     author_email="wy176404@163.com",
     # 包的简介描述
     description="A wrapper of the api logic used to interact with blue_media.",
     # 包的详细介绍(一般通过加载README.md)
@@ -27,12 +27,12 @@
         "Programming Language :: Python :: 3.6",
         # 根据MIT许可证开源
         "License :: OSI Approved :: MIT License",
         # 与操作系统无关
         "Operating System :: OS Independent",
     ],
     install_requires=[
-            'aiohttp>=3.9.1',
+            'aiohttp>=3.8.4',
             'aiosignal>=1.3.1',
             'async-timeout>=4.0.3',
         ]
 )
```

