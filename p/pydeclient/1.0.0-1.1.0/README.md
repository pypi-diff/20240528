# Comparing `tmp/pydeclient-1.0.0.tar.gz` & `tmp/pydeclient-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeclient-1.0.0.tar", last modified: Fri May 24 14:53:10 2024, max compression
+gzip compressed data, was "pydeclient-1.1.0.tar", last modified: Tue May 28 07:34:16 2024, max compression
```

## Comparing `pydeclient-1.0.0.tar` & `pydeclient-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vul337    (1001) vul337    (1001)        0 2024-05-24 14:53:10.985669 pydeclient-1.0.0/
--rw-rw-r--   0 vul337    (1001) vul337    (1001)     1063 2024-05-24 10:22:00.000000 pydeclient-1.0.0/LICENSE
--rw-r--r--   0 vul337    (1001) vul337    (1001)     1414 2024-05-24 14:53:10.985669 pydeclient-1.0.0/PKG-INFO
--rw-rw-r--   0 vul337    (1001) vul337    (1001)      974 2024-05-24 10:15:47.000000 pydeclient-1.0.0/README.md
-drwxrwxr-x   0 vul337    (1001) vul337    (1001)        0 2024-05-24 14:53:10.985669 pydeclient-1.0.0/declient/
--rw-rw-r--   0 vul337    (1001) vul337    (1001)      206 2024-05-24 08:56:07.000000 pydeclient-1.0.0/declient/__init__.py
--rw-rw-r--   0 vul337    (1001) vul337    (1001)     2311 2024-05-24 14:44:20.000000 pydeclient-1.0.0/declient/decompile.py
--rw-rw-r--   0 vul337    (1001) vul337    (1001)     2762 2024-05-24 10:51:40.000000 pydeclient-1.0.0/declient/decompile_async.py
-drwxrwxr-x   0 vul337    (1001) vul337    (1001)        0 2024-05-24 14:53:10.985669 pydeclient-1.0.0/pydeclient.egg-info/
--rw-r--r--   0 vul337    (1001) vul337    (1001)     1414 2024-05-24 14:53:10.000000 pydeclient-1.0.0/pydeclient.egg-info/PKG-INFO
--rw-rw-r--   0 vul337    (1001) vul337    (1001)      266 2024-05-24 14:53:10.000000 pydeclient-1.0.0/pydeclient.egg-info/SOURCES.txt
--rw-rw-r--   0 vul337    (1001) vul337    (1001)        1 2024-05-24 14:53:10.000000 pydeclient-1.0.0/pydeclient.egg-info/dependency_links.txt
--rw-rw-r--   0 vul337    (1001) vul337    (1001)       17 2024-05-24 14:53:10.000000 pydeclient-1.0.0/pydeclient.egg-info/requires.txt
--rw-rw-r--   0 vul337    (1001) vul337    (1001)        9 2024-05-24 14:53:10.000000 pydeclient-1.0.0/pydeclient.egg-info/top_level.txt
--rw-rw-r--   0 vul337    (1001) vul337    (1001)       38 2024-05-24 14:53:10.985669 pydeclient-1.0.0/setup.cfg
--rw-rw-r--   0 vul337    (1001) vul337    (1001)      652 2024-05-24 14:52:45.000000 pydeclient-1.0.0/setup.py
+drwxrwxr-x   0 vul337    (1001) vul337    (1001)        0 2024-05-28 07:34:16.327499 pydeclient-1.1.0/
+-rw-rw-r--   0 vul337    (1001) vul337    (1001)     1063 2024-05-24 10:22:00.000000 pydeclient-1.1.0/LICENSE
+-rw-r--r--   0 vul337    (1001) vul337    (1001)     2541 2024-05-28 07:34:16.327499 pydeclient-1.1.0/PKG-INFO
+-rw-rw-r--   0 vul337    (1001) vul337    (1001)     2077 2024-05-28 07:31:29.000000 pydeclient-1.1.0/README.md
+drwxrwxr-x   0 vul337    (1001) vul337    (1001)        0 2024-05-28 07:34:16.323499 pydeclient-1.1.0/declient/
+-rw-rw-r--   0 vul337    (1001) vul337    (1001)      160 2024-05-28 06:53:40.000000 pydeclient-1.1.0/declient/__init__.py
+-rw-rw-r--   0 vul337    (1001) vul337    (1001)     2311 2024-05-28 06:44:53.000000 pydeclient-1.1.0/declient/decompile.py
+-rw-rw-r--   0 vul337    (1001) vul337    (1001)     4661 2024-05-28 07:22:01.000000 pydeclient-1.1.0/declient/decompile_async.py
+drwxrwxr-x   0 vul337    (1001) vul337    (1001)        0 2024-05-28 07:34:16.327499 pydeclient-1.1.0/pydeclient.egg-info/
+-rw-r--r--   0 vul337    (1001) vul337    (1001)     2541 2024-05-28 07:34:16.000000 pydeclient-1.1.0/pydeclient.egg-info/PKG-INFO
+-rw-rw-r--   0 vul337    (1001) vul337    (1001)      266 2024-05-28 07:34:16.000000 pydeclient-1.1.0/pydeclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 vul337    (1001) vul337    (1001)        1 2024-05-28 07:34:16.000000 pydeclient-1.1.0/pydeclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 vul337    (1001) vul337    (1001)       22 2024-05-28 07:34:16.000000 pydeclient-1.1.0/pydeclient.egg-info/requires.txt
+-rw-rw-r--   0 vul337    (1001) vul337    (1001)        9 2024-05-28 07:34:16.000000 pydeclient-1.1.0/pydeclient.egg-info/top_level.txt
+-rw-rw-r--   0 vul337    (1001) vul337    (1001)       38 2024-05-28 07:34:16.327499 pydeclient-1.1.0/setup.cfg
+-rw-rw-r--   0 vul337    (1001) vul337    (1001)      671 2024-05-28 07:34:02.000000 pydeclient-1.1.0/setup.py
```

### Comparing `pydeclient-1.0.0/LICENSE` & `pydeclient-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeclient-1.0.0/declient/decompile.py` & `pydeclient-1.1.0/declient/decompile.py`

 * *Files identical despite different names*

### Comparing `pydeclient-1.0.0/setup.py` & `pydeclient-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pydeclient',
-    version='1.0.0',
+    version='1.1.0',
     packages=find_packages(),
     include_package_data=True,
-    description='A package for requesting decompiler service',
+    description='A package for requesting decompilebench service',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='hustcw',
     license='MIT',
     keywords='decompiler, binary, reverse engineering',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
         'aiohttp',
         'requests',
+        'tqdm'
     ]
 )
```

