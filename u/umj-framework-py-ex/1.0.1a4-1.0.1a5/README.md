# Comparing `tmp/umj-framework-py-ex-1.0.1a4.tar.gz` & `tmp/umj-framework-py-ex-1.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umj-framework-py-ex-1.0.1a4.tar", last modified: Tue May 28 07:50:48 2024, max compression
+gzip compressed data, was "umj-framework-py-ex-1.0.1a5.tar", last modified: Tue May 28 07:54:01 2024, max compression
```

## Comparing `umj-framework-py-ex-1.0.1a4.tar` & `umj-framework-py-ex-1.0.1a5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 07:50:48.755341 umj-framework-py-ex-1.0.1a4/
--rw-rw-rw-   0        0        0     1088 2024-05-23 14:31:37.000000 umj-framework-py-ex-1.0.1a4/LICENSE
--rw-rw-rw-   0        0        0     3206 2024-05-28 07:50:48.754341 umj-framework-py-ex-1.0.1a4/PKG-INFO
--rw-rw-rw-   0        0        0     2717 2024-05-25 10:17:35.000000 umj-framework-py-ex-1.0.1a4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-28 07:50:48.755341 umj-framework-py-ex-1.0.1a4/setup.cfg
--rw-rw-rw-   0        0        0      686 2024-05-28 07:50:43.000000 umj-framework-py-ex-1.0.1a4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:50:48.742340 umj-framework-py-ex-1.0.1a4/umj_framework_py_ex.egg-info/
--rw-rw-rw-   0        0        0     3206 2024-05-28 07:50:48.000000 umj-framework-py-ex-1.0.1a4/umj_framework_py_ex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-05-28 07:50:48.000000 umj-framework-py-ex-1.0.1a4/umj_framework_py_ex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 07:50:48.000000 umj-framework-py-ex-1.0.1a4/umj_framework_py_ex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-28 07:50:48.000000 umj-framework-py-ex-1.0.1a4/umj_framework_py_ex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 07:50:48.744341 umj-framework-py-ex-1.0.1a4/umj_framowrk/
--rw-rw-rw-   0        0        0      205 2024-05-28 07:49:29.000000 umj-framework-py-ex-1.0.1a4/umj_framowrk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:50:48.746343 umj-framework-py-ex-1.0.1a4/umj_framowrk/examples/
--rw-rw-rw-   0        0        0     4637 2024-05-28 07:16:19.000000 umj-framework-py-ex-1.0.1a4/umj_framowrk/examples/example_project.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:50:48.752341 umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/
--rw-rw-rw-   0        0        0    10327 2024-05-28 07:17:52.000000 umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/builder.py
--rw-rw-rw-   0        0        0      955 2024-05-28 03:50:53.000000 umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/common.py
--rw-rw-rw-   0        0        0     9000 2024-05-28 04:36:38.000000 umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/interpreter.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:54:01.536174 umj-framework-py-ex-1.0.1a5/
+-rw-rw-rw-   0        0        0     1088 2024-05-23 14:31:37.000000 umj-framework-py-ex-1.0.1a5/LICENSE
+-rw-rw-rw-   0        0        0     3206 2024-05-28 07:54:01.534173 umj-framework-py-ex-1.0.1a5/PKG-INFO
+-rw-rw-rw-   0        0        0     2717 2024-05-25 10:17:35.000000 umj-framework-py-ex-1.0.1a5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 07:54:01.536174 umj-framework-py-ex-1.0.1a5/setup.cfg
+-rw-rw-rw-   0        0        0      686 2024-05-28 07:53:48.000000 umj-framework-py-ex-1.0.1a5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:54:01.522172 umj-framework-py-ex-1.0.1a5/umj_framework_py_ex.egg-info/
+-rw-rw-rw-   0        0        0     3206 2024-05-28 07:54:01.000000 umj-framework-py-ex-1.0.1a5/umj_framework_py_ex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-05-28 07:54:01.000000 umj-framework-py-ex-1.0.1a5/umj_framework_py_ex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 07:54:01.000000 umj-framework-py-ex-1.0.1a5/umj_framework_py_ex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-28 07:54:01.000000 umj-framework-py-ex-1.0.1a5/umj_framework_py_ex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 07:54:01.524172 umj-framework-py-ex-1.0.1a5/umj_framowrk/
+-rw-rw-rw-   0        0        0      205 2024-05-28 07:49:29.000000 umj-framework-py-ex-1.0.1a5/umj_framowrk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:54:01.525172 umj-framework-py-ex-1.0.1a5/umj_framowrk/examples/
+-rw-rw-rw-   0        0        0     4637 2024-05-28 07:16:19.000000 umj-framework-py-ex-1.0.1a5/umj_framowrk/examples/example_project.py
+drwxrwxrwx   0        0        0        0 2024-05-28 07:54:01.532176 umj-framework-py-ex-1.0.1a5/umj_framowrk/kernel/
+-rw-rw-rw-   0        0        0    10327 2024-05-28 07:17:52.000000 umj-framework-py-ex-1.0.1a5/umj_framowrk/kernel/builder.py
+-rw-rw-rw-   0        0        0      955 2024-05-28 03:50:53.000000 umj-framework-py-ex-1.0.1a5/umj_framowrk/kernel/common.py
+-rw-rw-rw-   0        0        0     9015 2024-05-28 07:53:36.000000 umj-framework-py-ex-1.0.1a5/umj_framowrk/kernel/interpreter.py
```

### Comparing `umj-framework-py-ex-1.0.1a4/LICENSE` & `umj-framework-py-ex-1.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a4/PKG-INFO` & `umj-framework-py-ex-1.0.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umj-framework-py-ex
-Version: 1.0.1a4
+Version: 1.0.1a5
 Summary: A simple dinamic UI aiogram extension. Will be much more powered in future.
 Home-page: https://github.com/Waffe-Wafle/dynamic_py_loader
 Author: Waffe-Wafle
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `umj-framework-py-ex-1.0.1a4/README.md` & `umj-framework-py-ex-1.0.1a5/README.md`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a4/setup.py` & `umj-framework-py-ex-1.0.1a5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='umj-framework-py-ex',
-    version='1.0.1a4',
+    version='1.0.1a5',
     author='Waffe-Wafle',
     description='A simple dinamic UI aiogram extension. Will be much more powered in future.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/Waffe-Wafle/dynamic_py_loader',
     license='MIT',
     classifiers=[
```

### Comparing `umj-framework-py-ex-1.0.1a4/umj_framework_py_ex.egg-info/PKG-INFO` & `umj-framework-py-ex-1.0.1a5/umj_framework_py_ex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umj-framework-py-ex
-Version: 1.0.1a4
+Version: 1.0.1a5
 Summary: A simple dinamic UI aiogram extension. Will be much more powered in future.
 Home-page: https://github.com/Waffe-Wafle/dynamic_py_loader
 Author: Waffe-Wafle
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `umj-framework-py-ex-1.0.1a4/umj_framowrk/examples/example_project.py` & `umj-framework-py-ex-1.0.1a5/umj_framowrk/examples/example_project.py`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/builder.py` & `umj-framework-py-ex-1.0.1a5/umj_framowrk/kernel/builder.py`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/common.py` & `umj-framework-py-ex-1.0.1a5/umj_framowrk/kernel/common.py`

 * *Files identical despite different names*

### Comparing `umj-framework-py-ex-1.0.1a4/umj_framowrk/kernel/interpreter.py` & `umj-framework-py-ex-1.0.1a5/umj_framowrk/kernel/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from aiogram import Bot, Dispatcher
 from aiogram.fsm.storage.memory import MemoryStorage
 from aiogram.fsm.context import FSMContext
 from aiogram.types import (
     Message, CallbackQuery, InlineKeyboardMarkup, InlineKeyboardButton
 )
-from kernel.common import get_object_type
+
+from umj_framowrk.kernel.common import get_object_type
 from asyncio import run
 from dill import load
 from pathlib import Path
 import logging
 
 
 INTERPRETER_CON_KEY = 'intepr_data'
```

