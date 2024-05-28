# Comparing `tmp/package_tea_hanyan-1.0.3.tar.gz` & `tmp/package_tea_hanyan-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/package_tea_hanyan-1.0.3.tar", last modified: Mon Mar  4 01:59:21 2024, max compression
+gzip compressed data, was "dist/package_tea_hanyan-1.0.4.tar", last modified: Tue May 28 06:14:01 2024, max compression
```

## Comparing `package_tea_hanyan-1.0.3.tar` & `package_tea_hanyan-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 01:59:21.290620 package_tea_hanyan-1.0.3/
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1068 2024-03-04 01:59:21.290111 package_tea_hanyan-1.0.3/PKG-INFO
--rw-r--r--   0 xiaofeng   (502) staff       (20)      155 2024-03-01 02:52:44.000000 package_tea_hanyan-1.0.3/README.rst
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 01:59:21.287322 package_tea_hanyan-1.0.3/package_tea_hanyan/
--rw-r--r--   0 xiaofeng   (502) staff       (20)      127 2024-03-01 02:52:44.000000 package_tea_hanyan-1.0.3/package_tea_hanyan/__init__.py
--rw-r--r--   0 xiaofeng   (502) staff       (20)      505 2024-03-01 02:52:44.000000 package_tea_hanyan-1.0.3/package_tea_hanyan/main.py
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 01:59:21.289567 package_tea_hanyan-1.0.3/package_tea_hanyan.egg-info/
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1068 2024-03-04 01:59:21.000000 package_tea_hanyan-1.0.3/package_tea_hanyan.egg-info/PKG-INFO
--rw-r--r--   0 xiaofeng   (502) staff       (20)      245 2024-03-04 01:59:21.000000 package_tea_hanyan-1.0.3/package_tea_hanyan.egg-info/SOURCES.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)        1 2024-03-04 01:59:21.000000 package_tea_hanyan-1.0.3/package_tea_hanyan.egg-info/dependency_links.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       19 2024-03-04 01:59:21.000000 package_tea_hanyan-1.0.3/package_tea_hanyan.egg-info/top_level.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       38 2024-03-04 01:59:21.290705 package_tea_hanyan-1.0.3/setup.cfg
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1411 2024-03-04 01:58:01.000000 package_tea_hanyan-1.0.3/setup.py
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-28 06:14:01.000000 package_tea_hanyan-1.0.4/
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1169 2024-05-28 06:14:01.000000 package_tea_hanyan-1.0.4/PKG-INFO
+-rw-r--r--   0 xf.shen    (502) staff       (20)      148 2024-05-28 05:56:01.000000 package_tea_hanyan-1.0.4/README.rst
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-28 06:14:01.000000 package_tea_hanyan-1.0.4/package_tea_hanyan/
+-rw-r--r--   0 xf.shen    (502) staff       (20)      127 2024-05-28 05:22:13.000000 package_tea_hanyan-1.0.4/package_tea_hanyan/__init__.py
+-rw-r--r--   0 xf.shen    (502) staff       (20)      505 2024-05-28 05:22:13.000000 package_tea_hanyan-1.0.4/package_tea_hanyan/main.py
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-28 06:14:01.000000 package_tea_hanyan-1.0.4/package_tea_hanyan.egg-info/
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1169 2024-05-28 06:14:01.000000 package_tea_hanyan-1.0.4/package_tea_hanyan.egg-info/PKG-INFO
+-rw-r--r--   0 xf.shen    (502) staff       (20)      286 2024-05-28 06:14:01.000000 package_tea_hanyan-1.0.4/package_tea_hanyan.egg-info/SOURCES.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)        1 2024-05-28 06:14:01.000000 package_tea_hanyan-1.0.4/package_tea_hanyan.egg-info/dependency_links.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       51 2024-05-28 06:14:01.000000 package_tea_hanyan-1.0.4/package_tea_hanyan.egg-info/requires.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       19 2024-05-28 06:14:01.000000 package_tea_hanyan-1.0.4/package_tea_hanyan.egg-info/top_level.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       38 2024-05-28 06:14:01.000000 package_tea_hanyan-1.0.4/setup.cfg
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1457 2024-05-28 05:54:01.000000 package_tea_hanyan-1.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `package_tea_hanyan-1.0.3/PKG-INFO` & `package_tea_hanyan-1.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: package_tea_hanyan
-Version: 1.0.3
-Summary: small package just example
+Version: 1.0.4
+Summary: example for demo1
 Home-page: https://github.com/hanyan007/package_tea_hanyan.git
 Author: hanyan_news
 Author-email: hanyan0572@gmail.com
 License: BSD License
 Project-URL: Source, https://github.com/hanyan007/package_tea_hanyan.git
+Description: ========
+        发布示例
+        ========
+        - 主流的开源技术
+        - 自动化测试
+        - 性能测试
+        - 安全测试
+        - go开发实战
+        - CI/CD
+        - Docker
+        - DevOps
+        
+        
+        
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
-
-========
-发布示例
-========
-- test
-- 主流的开源技术
-- 自动化测试
-- 性能测试
-- 安全测试
-- go开发实战
-- CI/CD
-- Docker
-- DevOps
-
-
```

### Comparing `package_tea_hanyan-1.0.3/setup.py` & `package_tea_hanyan-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from setuptools import find_packages
 
 with open("README.rst", "r") as f:
   long_description = f.read()
 
 
 setup(name='package_tea_hanyan',  # 包名
-      version='1.0.3',  # 版本号
-      description='small package just example',
+      version='1.0.4',  # 版本号
+      description='example for demo1',
       long_description=long_description,
       author='hanyan_news',
       author_email='hanyan0572@gmail.com',
       url='https://github.com/hanyan007/package_tea_hanyan.git',
-      install_requires=[],
+      install_requires=["restful-dnspod-log==1.0.1", "dnspod-domain-log==1.0.4"],
       project_urls={  # Optional
         "Source": 'https://github.com/hanyan007/package_tea_hanyan.git',
       },
       license='BSD License',
       packages=find_packages(),
       platforms=["all"],
       classifiers=[
```

