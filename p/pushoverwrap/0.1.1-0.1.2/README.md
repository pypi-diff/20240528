# Comparing `tmp/pushoverwrap-0.1.1.tar.gz` & `tmp/pushoverwrap-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushoverwrap-0.1.1.tar", last modified: Wed May 22 02:59:11 2024, max compression
+gzip compressed data, was "pushoverwrap-0.1.2.tar", last modified: Tue May 28 03:34:26 2024, max compression
```

## Comparing `pushoverwrap-0.1.1.tar` & `pushoverwrap-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:11.893493 pushoverwrap-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 02:59:02.000000 pushoverwrap-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-22 02:59:11.893493 pushoverwrap-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-22 02:59:02.000000 pushoverwrap-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:11.893493 pushoverwrap-0.1.1/pushoverwrap/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 02:59:02.000000 pushoverwrap-0.1.1/pushoverwrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-22 02:59:02.000000 pushoverwrap-0.1.1/pushoverwrap/pushover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:59:11.893493 pushoverwrap-0.1.1/pushoverwrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-22 02:59:11.000000 pushoverwrap-0.1.1/pushoverwrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-22 02:59:11.000000 pushoverwrap-0.1.1/pushoverwrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:59:11.000000 pushoverwrap-0.1.1/pushoverwrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 02:59:11.000000 pushoverwrap-0.1.1/pushoverwrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:59:11.893493 pushoverwrap-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-22 02:59:02.000000 pushoverwrap-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:34:26.702289 pushoverwrap-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-28 03:34:19.000000 pushoverwrap-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-28 03:34:26.702289 pushoverwrap-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-28 03:34:19.000000 pushoverwrap-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:34:26.702289 pushoverwrap-0.1.2/pushoverwrap/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 03:34:19.000000 pushoverwrap-0.1.2/pushoverwrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-28 03:34:19.000000 pushoverwrap-0.1.2/pushoverwrap/pushover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:34:26.702289 pushoverwrap-0.1.2/pushoverwrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-28 03:34:26.000000 pushoverwrap-0.1.2/pushoverwrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 03:34:26.000000 pushoverwrap-0.1.2/pushoverwrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 03:34:26.000000 pushoverwrap-0.1.2/pushoverwrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 03:34:26.000000 pushoverwrap-0.1.2/pushoverwrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 03:34:26.702289 pushoverwrap-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-28 03:34:19.000000 pushoverwrap-0.1.2/setup.py
```

### Comparing `pushoverwrap-0.1.1/LICENSE` & `pushoverwrap-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pushoverwrap-0.1.1/PKG-INFO` & `pushoverwrap-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pushoverwrap
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple Pushover API wrapper.
-Home-page: https://github.com/plutotree/pushovewrap
+Home-page: https://github.com/plutotree/pushoverwrap
 Author: plutotree
 Author-email: plutotreetree@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pushoverwrap-0.1.1/README.md` & `pushoverwrap-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pushoverwrap-0.1.1/pushoverwrap/pushover.py` & `pushoverwrap-0.1.2/pushoverwrap/pushover.py`

 * *Files identical despite different names*

### Comparing `pushoverwrap-0.1.1/pushoverwrap.egg-info/PKG-INFO` & `pushoverwrap-0.1.2/pushoverwrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pushoverwrap
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple Pushover API wrapper.
-Home-page: https://github.com/plutotree/pushovewrap
+Home-page: https://github.com/plutotree/pushoverwrap
 Author: plutotree
 Author-email: plutotreetree@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pushoverwrap-0.1.1/setup.py` & `pushoverwrap-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pushoverwrap',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[],
     python_requires='>=3.6',
     author='plutotree',
     author_email='plutotreetree@gmail.com',
     description='A simple Pushover API wrapper.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/plutotree/pushovewrap',
+    url='https://github.com/plutotree/pushoverwrap',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
     ],
 )
```

