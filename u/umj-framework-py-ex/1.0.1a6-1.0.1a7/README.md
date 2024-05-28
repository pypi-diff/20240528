# Comparing `tmp/umj-framework-py-ex-1.0.1a6.tar.gz` & `tmp/umj-framework-py-ex-1.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umj-framework-py-ex-1.0.1a6.tar", last modified: Tue May 28 07:56:00 2024, max compression
+gzip compressed data, was "umj-framework-py-ex-1.0.1a7.tar", last modified: Tue May 28 08:08:09 2024, max compression
```

## Comparing `umj-framework-py-ex-1.0.1a6.tar` & `umj-framework-py-ex-1.0.1a7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 07:56:00.474817 umj-framework-py-ex-1.0.1a6/
--rw-rw-rw-   0        0        0     1088 2024-05-23 14:31:37.000000 umj-framework-py-ex-1.0.1a6/LICENSE
--rw-rw-rw-   0        0        0     3206 2024-05-28 07:56:00.474817 umj-framework-py-ex-1.0.1a6/PKG-INFO
--rw-rw-rw-   0        0        0     2717 2024-05-25 10:17:35.000000 umj-framework-py-ex-1.0.1a6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-28 07:56:00.474817 umj-framework-py-ex-1.0.1a6/setup.cfg
--rw-rw-rw-   0        0        0      686 2024-05-28 07:55:54.000000 umj-framework-py-ex-1.0.1a6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:56:00.464818 umj-framework-py-ex-1.0.1a6/umj_framework_py_ex.egg-info/
--rw-rw-rw-   0        0        0     3206 2024-05-28 07:56:00.000000 umj-framework-py-ex-1.0.1a6/umj_framework_py_ex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-05-28 07:56:00.000000 umj-framework-py-ex-1.0.1a6/umj_framework_py_ex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 07:56:00.000000 umj-framework-py-ex-1.0.1a6/umj_framework_py_ex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-28 07:56:00.000000 umj-framework-py-ex-1.0.1a6/umj_framework_py_ex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 07:56:00.466818 umj-framework-py-ex-1.0.1a6/umj_framowrk/
--rw-rw-rw-   0        0        0      205 2024-05-28 07:49:29.000000 umj-framework-py-ex-1.0.1a6/umj_framowrk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:56:00.467818 umj-framework-py-ex-1.0.1a6/umj_framowrk/examples/
--rw-rw-rw-   0        0        0     4637 2024-05-28 07:16:19.000000 umj-framework-py-ex-1.0.1a6/umj_framowrk/examples/example_project.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:56:00.472818 umj-framework-py-ex-1.0.1a6/umj_framowrk/kernel/
--rw-rw-rw-   0        0        0    10322 2024-05-28 07:55:43.000000 umj-framework-py-ex-1.0.1a6/umj_framowrk/kernel/builder.py
--rw-rw-rw-   0        0        0      955 2024-05-28 03:50:53.000000 umj-framework-py-ex-1.0.1a6/umj_framowrk/kernel/common.py
--rw-rw-rw-   0        0        0     9015 2024-05-28 07:53:36.000000 umj-framework-py-ex-1.0.1a6/umj_framowrk/kernel/interpreter.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:08:09.654222 umj-framework-py-ex-1.0.1a7/
+-rw-rw-rw-   0        0        0     1088 2024-05-23 14:31:37.000000 umj-framework-py-ex-1.0.1a7/LICENSE
+-rw-rw-rw-   0        0        0     3206 2024-05-28 08:08:09.653226 umj-framework-py-ex-1.0.1a7/PKG-INFO
+-rw-rw-rw-   0        0        0     2717 2024-05-25 10:17:35.000000 umj-framework-py-ex-1.0.1a7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 08:08:09.654222 umj-framework-py-ex-1.0.1a7/setup.cfg
+-rw-rw-rw-   0        0        0      766 2024-05-28 08:08:05.000000 umj-framework-py-ex-1.0.1a7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:08:09.641219 umj-framework-py-ex-1.0.1a7/umj_framework_py_ex.egg-info/
+-rw-rw-rw-   0        0        0     3206 2024-05-28 08:08:09.000000 umj-framework-py-ex-1.0.1a7/umj_framework_py_ex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2024-05-28 08:08:09.000000 umj-framework-py-ex-1.0.1a7/umj_framework_py_ex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 08:08:09.000000 umj-framework-py-ex-1.0.1a7/umj_framework_py_ex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-28 08:08:09.000000 umj-framework-py-ex-1.0.1a7/umj_framework_py_ex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-28 08:08:09.000000 umj-framework-py-ex-1.0.1a7/umj_framework_py_ex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 08:08:09.643220 umj-framework-py-ex-1.0.1a7/umj_framowrk/
+-rw-rw-rw-   0        0        0      205 2024-05-28 07:49:29.000000 umj-framework-py-ex-1.0.1a7/umj_framowrk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:08:09.644220 umj-framework-py-ex-1.0.1a7/umj_framowrk/examples/
+-rw-rw-rw-   0        0        0     4637 2024-05-28 07:16:19.000000 umj-framework-py-ex-1.0.1a7/umj_framowrk/examples/example_project.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:08:09.649220 umj-framework-py-ex-1.0.1a7/umj_framowrk/kernel/
+-rw-rw-rw-   0        0        0    10322 2024-05-28 07:55:43.000000 umj-framework-py-ex-1.0.1a7/umj_framowrk/kernel/builder.py
+-rw-rw-rw-   0        0        0      955 2024-05-28 03:50:53.000000 umj-framework-py-ex-1.0.1a7/umj_framowrk/kernel/common.py
+-rw-rw-rw-   0        0        0     9015 2024-05-28 07:53:36.000000 umj-framework-py-ex-1.0.1a7/umj_framowrk/kernel/interpreter.py
```

### Comparing `umj-framework-py-ex-1.0.1a6/LICENSE` & `umj-framework-py-ex-1.0.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a6/PKG-INFO` & `umj-framework-py-ex-1.0.1a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umj-framework-py-ex
-Version: 1.0.1a6
+Version: 1.0.1a7
 Summary: A simple dinamic UI aiogram extension. Will be much more powered in future.
 Home-page: https://github.com/Waffe-Wafle/dynamic_py_loader
 Author: Waffe-Wafle
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `umj-framework-py-ex-1.0.1a6/README.md` & `umj-framework-py-ex-1.0.1a7/README.md`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a6/setup.py` & `umj-framework-py-ex-1.0.1a7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='umj-framework-py-ex',
-    version='1.0.1a6',
+    version='1.0.1a7',
     author='Waffe-Wafle',
     description='A simple dinamic UI aiogram extension. Will be much more powered in future.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/Waffe-Wafle/dynamic_py_loader',
     license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
+    install_requires=[
+        'aiogram>=3.5',
+        'dill>=0.3.8'
+    ],
 )
```

### Comparing `umj-framework-py-ex-1.0.1a6/umj_framework_py_ex.egg-info/PKG-INFO` & `umj-framework-py-ex-1.0.1a7/umj_framework_py_ex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umj-framework-py-ex
-Version: 1.0.1a6
+Version: 1.0.1a7
 Summary: A simple dinamic UI aiogram extension. Will be much more powered in future.
 Home-page: https://github.com/Waffe-Wafle/dynamic_py_loader
 Author: Waffe-Wafle
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `umj-framework-py-ex-1.0.1a6/umj_framowrk/examples/example_project.py` & `umj-framework-py-ex-1.0.1a7/umj_framowrk/examples/example_project.py`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a6/umj_framowrk/kernel/builder.py` & `umj-framework-py-ex-1.0.1a7/umj_framowrk/kernel/builder.py`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a6/umj_framowrk/kernel/common.py` & `umj-framework-py-ex-1.0.1a7/umj_framowrk/kernel/common.py`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a6/umj_framowrk/kernel/interpreter.py` & `umj-framework-py-ex-1.0.1a7/umj_framowrk/kernel/interpreter.py`

 * *Files identical despite different names*

