# Comparing `tmp/umj-framework-py-ex-1.0.1a3.tar.gz` & `tmp/umj-framework-py-ex-1.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umj-framework-py-ex-1.0.1a3.tar", last modified: Tue May 28 07:44:59 2024, max compression
+gzip compressed data, was "umj-framework-py-ex-1.0.1a4.tar", last modified: Tue May 28 07:50:48 2024, max compression
```

## Comparing `umj-framework-py-ex-1.0.1a3.tar` & `umj-framework-py-ex-1.0.1a4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 07:44:59.986200 umj-framework-py-ex-1.0.1a3/
--rw-rw-rw-   0        0        0     1088 2024-05-23 14:31:37.000000 umj-framework-py-ex-1.0.1a3/LICENSE
--rw-rw-rw-   0        0        0     3206 2024-05-28 07:44:59.985197 umj-framework-py-ex-1.0.1a3/PKG-INFO
--rw-rw-rw-   0        0        0     2717 2024-05-25 10:17:35.000000 umj-framework-py-ex-1.0.1a3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-28 07:44:59.986200 umj-framework-py-ex-1.0.1a3/setup.cfg
--rw-rw-rw-   0        0        0      686 2024-05-28 07:36:21.000000 umj-framework-py-ex-1.0.1a3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:44:59.973201 umj-framework-py-ex-1.0.1a3/umj_framework_py_ex.egg-info/
--rw-rw-rw-   0        0        0     3206 2024-05-28 07:44:59.000000 umj-framework-py-ex-1.0.1a3/umj_framework_py_ex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-05-28 07:44:59.000000 umj-framework-py-ex-1.0.1a3/umj_framework_py_ex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 07:44:59.000000 umj-framework-py-ex-1.0.1a3/umj_framework_py_ex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-28 07:44:59.000000 umj-framework-py-ex-1.0.1a3/umj_framework_py_ex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 07:44:59.975202 umj-framework-py-ex-1.0.1a3/umj_framowrk/
--rw-rw-rw-   0        0        0      202 2024-05-28 07:17:55.000000 umj-framework-py-ex-1.0.1a3/umj_framowrk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:44:59.976197 umj-framework-py-ex-1.0.1a3/umj_framowrk/examples/
--rw-rw-rw-   0        0        0     4637 2024-05-28 07:16:19.000000 umj-framework-py-ex-1.0.1a3/umj_framowrk/examples/example_project.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:44:59.983197 umj-framework-py-ex-1.0.1a3/umj_framowrk/kernel/
--rw-rw-rw-   0        0        0    10327 2024-05-28 07:17:52.000000 umj-framework-py-ex-1.0.1a3/umj_framowrk/kernel/builder.py
--rw-rw-rw-   0        0        0      955 2024-05-28 03:50:53.000000 umj-framework-py-ex-1.0.1a3/umj_framowrk/kernel/common.py
--rw-rw-rw-   0        0        0     9000 2024-05-28 04:36:38.000000 umj-framework-py-ex-1.0.1a3/umj_framowrk/kernel/interpreter.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:50:48.755341 umj-framework-py-ex-1.0.1a4/
+-rw-rw-rw-   0        0        0     1088 2024-05-23 14:31:37.000000 umj-framework-py-ex-1.0.1a4/LICENSE
+-rw-rw-rw-   0        0        0     3206 2024-05-28 07:50:48.754341 umj-framework-py-ex-1.0.1a4/PKG-INFO
+-rw-rw-rw-   0        0        0     2717 2024-05-25 10:17:35.000000 umj-framework-py-ex-1.0.1a4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 07:50:48.755341 umj-framework-py-ex-1.0.1a4/setup.cfg
+-rw-rw-rw-   0        0        0      686 2024-05-28 07:50:43.000000 umj-framework-py-ex-1.0.1a4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:50:48.742340 umj-framework-py-ex-1.0.1a4/umj_framework_py_ex.egg-info/
+-rw-rw-rw-   0        0        0     3206 2024-05-28 07:50:48.000000 umj-framework-py-ex-1.0.1a4/umj_framework_py_ex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-05-28 07:50:48.000000 umj-framework-py-ex-1.0.1a4/umj_framework_py_ex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 07:50:48.000000 umj-framework-py-ex-1.0.1a4/umj_framework_py_ex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-28 07:50:48.000000 umj-framework-py-ex-1.0.1a4/umj_framework_py_ex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 07:50:48.744341 umj-framework-py-ex-1.0.1a4/umj_framowrk/
+-rw-rw-rw-   0        0        0      205 2024-05-28 07:49:29.000000 umj-framework-py-ex-1.0.1a4/umj_framowrk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:50:48.746343 umj-framework-py-ex-1.0.1a4/umj_framowrk/examples/
+-rw-rw-rw-   0        0        0     4637 2024-05-28 07:16:19.000000 umj-framework-py-ex-1.0.1a4/umj_framowrk/examples/example_project.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:50:48.752341 umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/
+-rw-rw-rw-   0        0        0    10327 2024-05-28 07:17:52.000000 umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/builder.py
+-rw-rw-rw-   0        0        0      955 2024-05-28 03:50:53.000000 umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/common.py
+-rw-rw-rw-   0        0        0     9000 2024-05-28 04:36:38.000000 umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/interpreter.py
```

### Comparing `umj-framework-py-ex-1.0.1a3/LICENSE` & `umj-framework-py-ex-1.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a3/PKG-INFO` & `umj-framework-py-ex-1.0.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umj-framework-py-ex
-Version: 1.0.1a3
+Version: 1.0.1a4
 Summary: A simple dinamic UI aiogram extension. Will be much more powered in future.
 Home-page: https://github.com/Waffe-Wafle/dynamic_py_loader
 Author: Waffe-Wafle
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `umj-framework-py-ex-1.0.1a3/README.md` & `umj-framework-py-ex-1.0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a3/setup.py` & `umj-framework-py-ex-1.0.1a4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='umj-framework-py-ex',
-    version='1.0.1a3',
+    version='1.0.1a4',
     author='Waffe-Wafle',
     description='A simple dinamic UI aiogram extension. Will be much more powered in future.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/Waffe-Wafle/dynamic_py_loader',
     license='MIT',
     classifiers=[
```

### Comparing `umj-framework-py-ex-1.0.1a3/umj_framework_py_ex.egg-info/PKG-INFO` & `umj-framework-py-ex-1.0.1a4/umj_framework_py_ex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umj-framework-py-ex
-Version: 1.0.1a3
+Version: 1.0.1a4
 Summary: A simple dinamic UI aiogram extension. Will be much more powered in future.
 Home-page: https://github.com/Waffe-Wafle/dynamic_py_loader
 Author: Waffe-Wafle
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `umj-framework-py-ex-1.0.1a3/umj_framowrk/examples/example_project.py` & `umj-framework-py-ex-1.0.1a4/umj_framowrk/examples/example_project.py`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a3/umj_framowrk/kernel/builder.py` & `umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/builder.py`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a3/umj_framowrk/kernel/common.py` & `umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/common.py`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a3/umj_framowrk/kernel/interpreter.py` & `umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/interpreter.py`

 * *Files identical despite different names*

