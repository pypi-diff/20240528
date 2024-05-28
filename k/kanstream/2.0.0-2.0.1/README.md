# Comparing `tmp/kanstream-2.0.0.tar.gz` & `tmp/kanstream-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanstream-2.0.0.tar", last modified: Tue May 28 02:17:48 2024, max compression
+gzip compressed data, was "kanstream-2.0.1.tar", last modified: Tue May 28 03:09:01 2024, max compression
```

## Comparing `kanstream-2.0.0.tar` & `kanstream-2.0.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 02:17:48.108913 kanstream-2.0.0/
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-28 01:34:51.000000 kanstream-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      188 2024-05-28 02:17:48.108913 kanstream-2.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 02:17:48.107913 kanstream-2.0.0/kanstream/
--rw-r--r--   0 root         (0) root         (0)     3521 2024-05-27 10:07:32.000000 kanstream-2.0.0/kanstream/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 02:17:48.107913 kanstream-2.0.0/kanstream/codec/
--rw-r--r--   0 root         (0) root         (0)       36 2024-05-27 07:56:18.000000 kanstream-2.0.0/kanstream/codec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      406 2024-05-27 07:22:05.000000 kanstream-2.0.0/kanstream/codec/abc.py
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-27 07:45:11.000000 kanstream-2.0.0/kanstream/codec/codec.py
--rw-r--r--   0 root         (0) root         (0)     3269 2024-05-27 09:02:44.000000 kanstream-2.0.0/kanstream/codec/h264.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-05-27 07:23:03.000000 kanstream-2.0.0/kanstream/codec/vp9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 02:17:48.108913 kanstream-2.0.0/kanstream/stream/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:23:08.000000 kanstream-2.0.0/kanstream/stream/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1745 2024-05-27 09:06:17.000000 kanstream-2.0.0/kanstream/stream/base.py
--rw-r--r--   0 root         (0) root         (0)      972 2024-05-27 06:35:39.000000 kanstream-2.0.0/kanstream/stream/frame_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1402 2024-05-27 06:23:08.000000 kanstream-2.0.0/kanstream/stream/protobuf.py
--rw-r--r--   0 root         (0) root         (0)     2451 2024-05-27 10:09:11.000000 kanstream-2.0.0/kanstream/stream/receiver.py
--rw-r--r--   0 root         (0) root         (0)     2176 2024-05-27 10:08:54.000000 kanstream-2.0.0/kanstream/stream/sender.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 02:17:48.108913 kanstream-2.0.0/kanstream/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:23:08.000000 kanstream-2.0.0/kanstream/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1297 2024-05-27 06:23:08.000000 kanstream-2.0.0/kanstream/utils/calculate_bitrate.py
--rw-r--r--   0 root         (0) root         (0)      489 2024-05-28 01:46:00.000000 kanstream-2.0.0/kanstream/utils/frame_queue.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-27 08:52:31.000000 kanstream-2.0.0/kanstream/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 02:17:48.107913 kanstream-2.0.0/kanstream.egg-info/
--rw-r--r--   0 root         (0) root         (0)      188 2024-05-28 02:17:48.000000 kanstream-2.0.0/kanstream.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      632 2024-05-28 02:17:48.000000 kanstream-2.0.0/kanstream.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 02:17:48.000000 kanstream-2.0.0/kanstream.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 02:17:48.000000 kanstream-2.0.0/kanstream.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 02:17:48.000000 kanstream-2.0.0/kanstream.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 01:19:21.000000 kanstream-2.0.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 02:17:48.108913 kanstream-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      742 2024-05-28 02:06:02.000000 kanstream-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:09:01.015380 kanstream-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-28 01:34:51.000000 kanstream-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2870 2024-05-28 03:09:01.015380 kanstream-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2653 2024-05-28 02:58:56.000000 kanstream-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:09:01.013380 kanstream-2.0.1/kanstream/
+-rw-r--r--   0 root         (0) root         (0)     3521 2024-05-27 10:07:32.000000 kanstream-2.0.1/kanstream/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:09:01.014380 kanstream-2.0.1/kanstream/codec/
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-27 07:56:18.000000 kanstream-2.0.1/kanstream/codec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      406 2024-05-27 07:22:05.000000 kanstream-2.0.1/kanstream/codec/abc.py
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-27 07:45:11.000000 kanstream-2.0.1/kanstream/codec/codec.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2024-05-27 09:02:44.000000 kanstream-2.0.1/kanstream/codec/h264.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-27 07:23:03.000000 kanstream-2.0.1/kanstream/codec/vp9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:09:01.014380 kanstream-2.0.1/kanstream/stream/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:23:08.000000 kanstream-2.0.1/kanstream/stream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-05-27 09:06:17.000000 kanstream-2.0.1/kanstream/stream/base.py
+-rw-r--r--   0 root         (0) root         (0)      972 2024-05-27 06:35:39.000000 kanstream-2.0.1/kanstream/stream/frame_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2024-05-27 06:23:08.000000 kanstream-2.0.1/kanstream/stream/protobuf.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2024-05-27 10:09:11.000000 kanstream-2.0.1/kanstream/stream/receiver.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2024-05-27 10:08:54.000000 kanstream-2.0.1/kanstream/stream/sender.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:09:01.015380 kanstream-2.0.1/kanstream/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:23:08.000000 kanstream-2.0.1/kanstream/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2024-05-27 06:23:08.000000 kanstream-2.0.1/kanstream/utils/calculate_bitrate.py
+-rw-r--r--   0 root         (0) root         (0)      489 2024-05-28 01:46:00.000000 kanstream-2.0.1/kanstream/utils/frame_queue.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-28 03:02:59.000000 kanstream-2.0.1/kanstream/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:09:01.013380 kanstream-2.0.1/kanstream.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2870 2024-05-28 03:09:00.000000 kanstream-2.0.1/kanstream.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      642 2024-05-28 03:09:00.000000 kanstream-2.0.1/kanstream.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 03:09:00.000000 kanstream-2.0.1/kanstream.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 03:09:00.000000 kanstream-2.0.1/kanstream.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 03:09:00.000000 kanstream-2.0.1/kanstream.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 01:19:21.000000 kanstream-2.0.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 03:09:01.015380 kanstream-2.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-05-28 03:01:29.000000 kanstream-2.0.1/setup.py
```

### Comparing `kanstream-2.0.0/kanstream/__init__.py` & `kanstream-2.0.1/kanstream/__init__.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.0/kanstream/codec/codec.py` & `kanstream-2.0.1/kanstream/codec/codec.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.0/kanstream/codec/h264.py` & `kanstream-2.0.1/kanstream/codec/h264.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.0/kanstream/stream/base.py` & `kanstream-2.0.1/kanstream/stream/base.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.0/kanstream/stream/frame_pb2.py` & `kanstream-2.0.1/kanstream/stream/frame_pb2.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.0/kanstream/stream/protobuf.py` & `kanstream-2.0.1/kanstream/stream/protobuf.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.0/kanstream/stream/receiver.py` & `kanstream-2.0.1/kanstream/stream/receiver.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.0/kanstream/stream/sender.py` & `kanstream-2.0.1/kanstream/stream/sender.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.0/kanstream/utils/calculate_bitrate.py` & `kanstream-2.0.1/kanstream/utils/calculate_bitrate.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.0/kanstream.egg-info/SOURCES.txt` & `kanstream-2.0.1/kanstream.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 MANIFEST.in
+README.md
 requirements.txt
 setup.py
 kanstream/__init__.py
 kanstream/version.py
 kanstream.egg-info/PKG-INFO
 kanstream.egg-info/SOURCES.txt
 kanstream.egg-info/dependency_links.txt
```

### Comparing `kanstream-2.0.0/setup.py` & `kanstream-2.0.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,16 +18,26 @@
 def parse_requirements():
     with open(requirements_file, 'r') as f:
         requires = list(map(lambda x: x.strip(), f.readlines()))
 
     return requires
 
 
+def parse_long_description():
+    with open("README.md", "r", encoding='utf-8') as fh:
+        long_description = fh.read()
+    
+    return long_description
+
+
 setup(
     name='kanstream',
     description='pull and push stream',
     version=get_version(),
     author="flinzhao",
     packages=find_packages(),
+    long_description=parse_long_description(),
+    license='MIT',
+    long_description_content_type="text/markdown",
     install_requires=parse_requirements(),
     python_requires=">=3.10",
 )
```

