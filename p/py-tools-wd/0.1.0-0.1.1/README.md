# Comparing `tmp/py-tools-wd-0.1.0.tar.gz` & `tmp/py-tools-wd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-tools-wd-0.1.0.tar", last modified: Mon May 27 14:57:38 2024, max compression
+gzip compressed data, was "py-tools-wd-0.1.1.tar", last modified: Tue May 28 06:52:45 2024, max compression
```

## Comparing `py-tools-wd-0.1.0.tar` & `py-tools-wd-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:57:38.526787 py-tools-wd-0.1.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-27 03:17:32.000000 py-tools-wd-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      880 2024-05-27 14:57:38.526787 py-tools-wd-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       27 2024-05-27 03:17:32.000000 py-tools-wd-0.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 14:57:38.526787 py-tools-wd-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3028 2024-05-27 07:00:35.000000 py-tools-wd-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:57:38.522786 py-tools-wd-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:57:38.526787 py-tools-wd-0.1.0/src/py_tools_wd/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:38:56.000000 py-tools-wd-0.1.0/src/py_tools_wd/__init__.py
--rw-r--r--   0 root         (0) root         (0)      333 2024-05-27 14:57:32.000000 py-tools-wd-0.1.0/src/py_tools_wd/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:57:38.526787 py-tools-wd-0.1.0/src/py_tools_wd/image/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:38:56.000000 py-tools-wd-0.1.0/src/py_tools_wd/image/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3864 2024-05-27 14:56:20.000000 py-tools-wd-0.1.0/src/py_tools_wd/image/coord.py
--rw-r--r--   0 root         (0) root         (0)     3627 2024-05-27 06:45:12.000000 py-tools-wd-0.1.0/src/py_tools_wd/image/image_converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:57:38.526787 py-tools-wd-0.1.0/src/py_tools_wd/mq/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:38:56.000000 py-tools-wd-0.1.0/src/py_tools_wd/mq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1191 2024-05-27 07:33:37.000000 py-tools-wd-0.1.0/src/py_tools_wd/mq/channel.py
--rw-r--r--   0 root         (0) root         (0)     3985 2024-05-27 07:46:10.000000 py-tools-wd-0.1.0/src/py_tools_wd/mq/kafka.py
--rw-r--r--   0 root         (0) root         (0)    11196 2024-05-27 07:58:15.000000 py-tools-wd-0.1.0/src/py_tools_wd/mq/rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:57:38.526787 py-tools-wd-0.1.0/src/py_tools_wd.egg-info/
--rw-r--r--   0 root         (0) root         (0)      880 2024-05-27 14:57:38.000000 py-tools-wd-0.1.0/src/py_tools_wd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      505 2024-05-27 14:57:38.000000 py-tools-wd-0.1.0/src/py_tools_wd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 14:57:38.000000 py-tools-wd-0.1.0/src/py_tools_wd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 05:54:38.000000 py-tools-wd-0.1.0/src/py_tools_wd.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-27 14:57:38.000000 py-tools-wd-0.1.0/src/py_tools_wd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:52:45.737579 py-tools-wd-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-27 03:17:32.000000 py-tools-wd-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      880 2024-05-28 06:52:45.737579 py-tools-wd-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       27 2024-05-27 03:17:32.000000 py-tools-wd-0.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 06:52:45.737579 py-tools-wd-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3028 2024-05-27 07:00:35.000000 py-tools-wd-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:52:45.733579 py-tools-wd-0.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:52:45.733579 py-tools-wd-0.1.1/src/py_tools_wd/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:38:56.000000 py-tools-wd-0.1.1/src/py_tools_wd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      333 2024-05-28 06:52:42.000000 py-tools-wd-0.1.1/src/py_tools_wd/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:52:45.733579 py-tools-wd-0.1.1/src/py_tools_wd/image/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:38:56.000000 py-tools-wd-0.1.1/src/py_tools_wd/image/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3864 2024-05-27 14:56:20.000000 py-tools-wd-0.1.1/src/py_tools_wd/image/coord.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2024-05-28 06:52:31.000000 py-tools-wd-0.1.1/src/py_tools_wd/image/image_converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:52:45.733579 py-tools-wd-0.1.1/src/py_tools_wd/mq/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:38:56.000000 py-tools-wd-0.1.1/src/py_tools_wd/mq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-05-27 07:33:37.000000 py-tools-wd-0.1.1/src/py_tools_wd/mq/channel.py
+-rw-r--r--   0 root         (0) root         (0)     3985 2024-05-27 07:46:10.000000 py-tools-wd-0.1.1/src/py_tools_wd/mq/kafka.py
+-rw-r--r--   0 root         (0) root         (0)    11196 2024-05-27 07:58:15.000000 py-tools-wd-0.1.1/src/py_tools_wd/mq/rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:52:45.733579 py-tools-wd-0.1.1/src/py_tools_wd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      880 2024-05-28 06:52:45.000000 py-tools-wd-0.1.1/src/py_tools_wd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      505 2024-05-28 06:52:45.000000 py-tools-wd-0.1.1/src/py_tools_wd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 06:52:45.000000 py-tools-wd-0.1.1/src/py_tools_wd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 05:54:38.000000 py-tools-wd-0.1.1/src/py_tools_wd.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-28 06:52:45.000000 py-tools-wd-0.1.1/src/py_tools_wd.egg-info/top_level.txt
```

### Comparing `py-tools-wd-0.1.0/LICENSE` & `py-tools-wd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-tools-wd-0.1.0/PKG-INFO` & `py-tools-wd-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tools-wd
-Version: 0.1.0
+Version: 0.1.1
 Summary: wd py tools
 Home-page: https://github.com/pgcomb/wd_tools_py
 Author: Wang Dongxu
 Author-email: wangdongxudyx@163.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `py-tools-wd-0.1.0/setup.py` & `py-tools-wd-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `py-tools-wd-0.1.0/src/py_tools_wd/image/coord.py` & `py-tools-wd-0.1.1/src/py_tools_wd/image/coord.py`

 * *Files identical despite different names*

### Comparing `py-tools-wd-0.1.0/src/py_tools_wd/image/image_converter.py` & `py-tools-wd-0.1.1/src/py_tools_wd/image/image_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,8 +124,9 @@
 def to_file(image, path: FilePath):
     if isinstance(image, str):
         base64_to_file(image, path)
     elif isinstance(image, PIL_Image):
         pil_to_file(image, path)
     elif isinstance(image, NPImage):
         np_to_file(image, path)
-    raise Exception('image type error')
+    else:
+        raise Exception('image type error')
```

### Comparing `py-tools-wd-0.1.0/src/py_tools_wd/mq/channel.py` & `py-tools-wd-0.1.1/src/py_tools_wd/mq/channel.py`

 * *Files identical despite different names*

### Comparing `py-tools-wd-0.1.0/src/py_tools_wd/mq/kafka.py` & `py-tools-wd-0.1.1/src/py_tools_wd/mq/kafka.py`

 * *Files identical despite different names*

### Comparing `py-tools-wd-0.1.0/src/py_tools_wd/mq/rabbitmq.py` & `py-tools-wd-0.1.1/src/py_tools_wd/mq/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `py-tools-wd-0.1.0/src/py_tools_wd.egg-info/PKG-INFO` & `py-tools-wd-0.1.1/src/py_tools_wd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tools-wd
-Version: 0.1.0
+Version: 0.1.1
 Summary: wd py tools
 Home-page: https://github.com/pgcomb/wd_tools_py
 Author: Wang Dongxu
 Author-email: wangdongxudyx@163.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

