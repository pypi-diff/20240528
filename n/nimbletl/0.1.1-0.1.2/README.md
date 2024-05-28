# Comparing `tmp/nimbletl-0.1.1.tar.gz` & `tmp/nimbletl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimbletl-0.1.1.tar", last modified: Tue May 28 06:55:31 2024, max compression
+gzip compressed data, was "nimbletl-0.1.2.tar", last modified: Tue May 28 06:58:52 2024, max compression
```

## Comparing `nimbletl-0.1.1.tar` & `nimbletl-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 06:55:31.942705 nimbletl-0.1.1/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 06:55:31.942388 nimbletl-0.1.1/PKG-INFO
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      217 2024-05-28 06:32:53.000000 nimbletl-0.1.1/README.md
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 06:55:31.941986 nimbletl-0.1.1/nimbletl.egg-info/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 06:55:31.000000 nimbletl-0.1.1/nimbletl.egg-info/PKG-INFO
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      212 2024-05-28 06:55:31.000000 nimbletl-0.1.1/nimbletl.egg-info/SOURCES.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-28 06:55:31.000000 nimbletl-0.1.1/nimbletl.egg-info/dependency_links.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       58 2024-05-28 06:55:31.000000 nimbletl-0.1.1/nimbletl.egg-info/entry_points.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       57 2024-05-28 06:55:31.000000 nimbletl-0.1.1/nimbletl.egg-info/requires.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-28 06:55:31.000000 nimbletl-0.1.1/nimbletl.egg-info/top_level.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       38 2024-05-28 06:55:31.942794 nimbletl-0.1.1/setup.cfg
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      746 2024-05-28 06:55:27.000000 nimbletl-0.1.1/setup.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 06:58:52.167069 nimbletl-0.1.2/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 06:58:52.166767 nimbletl-0.1.2/PKG-INFO
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      217 2024-05-28 06:32:53.000000 nimbletl-0.1.2/README.md
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 06:58:52.166468 nimbletl-0.1.2/nimbletl.egg-info/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 06:58:52.000000 nimbletl-0.1.2/nimbletl.egg-info/PKG-INFO
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      212 2024-05-28 06:58:52.000000 nimbletl-0.1.2/nimbletl.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-28 06:58:52.000000 nimbletl-0.1.2/nimbletl.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       54 2024-05-28 06:58:52.000000 nimbletl-0.1.2/nimbletl.egg-info/entry_points.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       57 2024-05-28 06:58:52.000000 nimbletl-0.1.2/nimbletl.egg-info/requires.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-28 06:58:52.000000 nimbletl-0.1.2/nimbletl.egg-info/top_level.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       38 2024-05-28 06:58:52.167129 nimbletl-0.1.2/setup.cfg
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      742 2024-05-28 06:58:48.000000 nimbletl-0.1.2/setup.py
```

### Comparing `nimbletl-0.1.1/setup.py` & `nimbletl-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,20 @@
         lock_data = json.load(f)
     dependencies = lock_data['default']
     return [f"{pkg}{info.get('version', '')}" for pkg, info in dependencies.items()]
 
 
 setuptools.setup(
     name='nimbletl',
-    version='0.1.1',
+    version='0.1.2',
     packages=setuptools.find_packages(),
     install_requires=parse_pipfile_lock(),
     entry_points={
         'console_scripts': [
-            'nimbletl=src.log_driver.init.cli:main',
+            'nimbletl=log_driver.init.cli:main',
         ],
     },
     author="Ma Xiaoqiang",
     author_email="851788096@qq.com",
     description="Make your ETL easier and more nimble",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown'
```

