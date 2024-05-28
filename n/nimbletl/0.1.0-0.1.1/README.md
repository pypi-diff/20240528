# Comparing `tmp/nimbletl-0.1.0.tar.gz` & `tmp/nimbletl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimbletl-0.1.0.tar", last modified: Tue May 28 06:48:09 2024, max compression
+gzip compressed data, was "nimbletl-0.1.1.tar", last modified: Tue May 28 06:55:31 2024, max compression
```

## Comparing `nimbletl-0.1.0.tar` & `nimbletl-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 06:48:09.618955 nimbletl-0.1.0/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 06:48:09.618712 nimbletl-0.1.0/PKG-INFO
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      217 2024-05-28 06:32:53.000000 nimbletl-0.1.0/README.md
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 06:48:09.618456 nimbletl-0.1.0/nimbletl.egg-info/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 06:48:09.000000 nimbletl-0.1.0/nimbletl.egg-info/PKG-INFO
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      212 2024-05-28 06:48:09.000000 nimbletl-0.1.0/nimbletl.egg-info/SOURCES.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-28 06:48:09.000000 nimbletl-0.1.0/nimbletl.egg-info/dependency_links.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       58 2024-05-28 06:48:09.000000 nimbletl-0.1.0/nimbletl.egg-info/entry_points.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       57 2024-05-28 06:48:09.000000 nimbletl-0.1.0/nimbletl.egg-info/requires.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-28 06:48:09.000000 nimbletl-0.1.0/nimbletl.egg-info/top_level.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       38 2024-05-28 06:48:09.619014 nimbletl-0.1.0/setup.cfg
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      746 2024-05-28 06:40:04.000000 nimbletl-0.1.0/setup.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 06:55:31.942705 nimbletl-0.1.1/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 06:55:31.942388 nimbletl-0.1.1/PKG-INFO
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      217 2024-05-28 06:32:53.000000 nimbletl-0.1.1/README.md
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 06:55:31.941986 nimbletl-0.1.1/nimbletl.egg-info/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 06:55:31.000000 nimbletl-0.1.1/nimbletl.egg-info/PKG-INFO
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      212 2024-05-28 06:55:31.000000 nimbletl-0.1.1/nimbletl.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-28 06:55:31.000000 nimbletl-0.1.1/nimbletl.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       58 2024-05-28 06:55:31.000000 nimbletl-0.1.1/nimbletl.egg-info/entry_points.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       57 2024-05-28 06:55:31.000000 nimbletl-0.1.1/nimbletl.egg-info/requires.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-28 06:55:31.000000 nimbletl-0.1.1/nimbletl.egg-info/top_level.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       38 2024-05-28 06:55:31.942794 nimbletl-0.1.1/setup.cfg
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      746 2024-05-28 06:55:27.000000 nimbletl-0.1.1/setup.py
```

### Comparing `nimbletl-0.1.0/setup.py` & `nimbletl-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         lock_data = json.load(f)
     dependencies = lock_data['default']
     return [f"{pkg}{info.get('version', '')}" for pkg, info in dependencies.items()]
 
 
 setuptools.setup(
     name='nimbletl',
-    version='0.1.0',
+    version='0.1.1',
     packages=setuptools.find_packages(),
     install_requires=parse_pipfile_lock(),
     entry_points={
         'console_scripts': [
             'nimbletl=src.log_driver.init.cli:main',
         ],
     },
```

