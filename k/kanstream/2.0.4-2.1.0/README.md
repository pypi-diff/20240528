# Comparing `tmp/kanstream-2.0.4.tar.gz` & `tmp/kanstream-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanstream-2.0.4.tar", last modified: Tue May 28 09:19:13 2024, max compression
+gzip compressed data, was "kanstream-2.1.0.tar", last modified: Tue May 28 09:19:58 2024, max compression
```

## Comparing `kanstream-2.0.4.tar` & `kanstream-2.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:19:13.610779 kanstream-2.0.4/
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-28 01:34:51.000000 kanstream-2.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2870 2024-05-28 09:19:13.610779 kanstream-2.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2653 2024-05-28 02:58:56.000000 kanstream-2.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:19:13.607779 kanstream-2.0.4/kanstream/
--rw-r--r--   0 root         (0) root         (0)     3521 2024-05-28 03:36:28.000000 kanstream-2.0.4/kanstream/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:19:13.609779 kanstream-2.0.4/kanstream/codec/
--rw-r--r--   0 root         (0) root         (0)       36 2024-05-27 07:56:18.000000 kanstream-2.0.4/kanstream/codec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      406 2024-05-27 07:22:05.000000 kanstream-2.0.4/kanstream/codec/abc.py
--rw-r--r--   0 root         (0) root         (0)     1289 2024-05-28 09:17:26.000000 kanstream-2.0.4/kanstream/codec/codec.py
--rw-r--r--   0 root         (0) root         (0)     3266 2024-05-28 09:13:52.000000 kanstream-2.0.4/kanstream/codec/h264.py
--rw-r--r--   0 root         (0) root         (0)     1209 2024-05-28 09:16:50.000000 kanstream-2.0.4/kanstream/codec/h265.py
--rw-r--r--   0 root         (0) root         (0)     1089 2024-05-28 09:08:35.000000 kanstream-2.0.4/kanstream/codec/vp9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:19:13.610779 kanstream-2.0.4/kanstream/stream/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:23:08.000000 kanstream-2.0.4/kanstream/stream/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1746 2024-05-28 03:32:03.000000 kanstream-2.0.4/kanstream/stream/base.py
--rw-r--r--   0 root         (0) root         (0)      972 2024-05-27 06:35:39.000000 kanstream-2.0.4/kanstream/stream/frame_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1402 2024-05-27 06:23:08.000000 kanstream-2.0.4/kanstream/stream/protobuf.py
--rw-r--r--   0 root         (0) root         (0)     2451 2024-05-28 03:32:49.000000 kanstream-2.0.4/kanstream/stream/receiver.py
--rw-r--r--   0 root         (0) root         (0)     2176 2024-05-27 10:08:54.000000 kanstream-2.0.4/kanstream/stream/sender.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:19:13.610779 kanstream-2.0.4/kanstream/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:23:08.000000 kanstream-2.0.4/kanstream/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1297 2024-05-27 06:23:08.000000 kanstream-2.0.4/kanstream/utils/calculate_bitrate.py
--rw-r--r--   0 root         (0) root         (0)      489 2024-05-28 01:46:00.000000 kanstream-2.0.4/kanstream/utils/frame_queue.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-28 09:14:31.000000 kanstream-2.0.4/kanstream/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:19:13.608779 kanstream-2.0.4/kanstream.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2870 2024-05-28 09:19:13.000000 kanstream-2.0.4/kanstream.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      666 2024-05-28 09:19:13.000000 kanstream-2.0.4/kanstream.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 09:19:13.000000 kanstream-2.0.4/kanstream.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 09:19:13.000000 kanstream-2.0.4/kanstream.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 09:19:13.000000 kanstream-2.0.4/kanstream.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 01:19:21.000000 kanstream-2.0.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 09:19:13.610779 kanstream-2.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1018 2024-05-28 03:01:29.000000 kanstream-2.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:19:58.240742 kanstream-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-28 01:34:51.000000 kanstream-2.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2870 2024-05-28 09:19:58.240742 kanstream-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2653 2024-05-28 02:58:56.000000 kanstream-2.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:19:58.237742 kanstream-2.1.0/kanstream/
+-rw-r--r--   0 root         (0) root         (0)     3521 2024-05-28 03:36:28.000000 kanstream-2.1.0/kanstream/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:19:58.239742 kanstream-2.1.0/kanstream/codec/
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-27 07:56:18.000000 kanstream-2.1.0/kanstream/codec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      406 2024-05-27 07:22:05.000000 kanstream-2.1.0/kanstream/codec/abc.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-05-28 09:17:26.000000 kanstream-2.1.0/kanstream/codec/codec.py
+-rw-r--r--   0 root         (0) root         (0)     3266 2024-05-28 09:13:52.000000 kanstream-2.1.0/kanstream/codec/h264.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-05-28 09:16:50.000000 kanstream-2.1.0/kanstream/codec/h265.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-05-28 09:08:35.000000 kanstream-2.1.0/kanstream/codec/vp9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:19:58.240742 kanstream-2.1.0/kanstream/stream/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:23:08.000000 kanstream-2.1.0/kanstream/stream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2024-05-28 03:32:03.000000 kanstream-2.1.0/kanstream/stream/base.py
+-rw-r--r--   0 root         (0) root         (0)      972 2024-05-27 06:35:39.000000 kanstream-2.1.0/kanstream/stream/frame_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2024-05-27 06:23:08.000000 kanstream-2.1.0/kanstream/stream/protobuf.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2024-05-28 03:32:49.000000 kanstream-2.1.0/kanstream/stream/receiver.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2024-05-27 10:08:54.000000 kanstream-2.1.0/kanstream/stream/sender.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:19:58.240742 kanstream-2.1.0/kanstream/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:23:08.000000 kanstream-2.1.0/kanstream/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2024-05-27 06:23:08.000000 kanstream-2.1.0/kanstream/utils/calculate_bitrate.py
+-rw-r--r--   0 root         (0) root         (0)      489 2024-05-28 01:46:00.000000 kanstream-2.1.0/kanstream/utils/frame_queue.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-28 09:19:36.000000 kanstream-2.1.0/kanstream/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:19:58.238742 kanstream-2.1.0/kanstream.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2870 2024-05-28 09:19:58.000000 kanstream-2.1.0/kanstream.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      666 2024-05-28 09:19:58.000000 kanstream-2.1.0/kanstream.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 09:19:58.000000 kanstream-2.1.0/kanstream.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 09:19:58.000000 kanstream-2.1.0/kanstream.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 09:19:58.000000 kanstream-2.1.0/kanstream.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 01:19:21.000000 kanstream-2.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 09:19:58.240742 kanstream-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-05-28 03:01:29.000000 kanstream-2.1.0/setup.py
```

### Comparing `kanstream-2.0.4/PKG-INFO` & `kanstream-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kanstream
-Version: 2.0.4
+Version: 2.1.0
 Summary: pull and push stream
 Home-page: UNKNOWN
 Author: flinzhao
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `kanstream-2.0.4/README.md` & `kanstream-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/kanstream/__init__.py` & `kanstream-2.1.0/kanstream/__init__.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/kanstream/codec/codec.py` & `kanstream-2.1.0/kanstream/codec/codec.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/kanstream/codec/h264.py` & `kanstream-2.1.0/kanstream/codec/h264.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/kanstream/codec/h265.py` & `kanstream-2.1.0/kanstream/codec/h265.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/kanstream/codec/vp9.py` & `kanstream-2.1.0/kanstream/codec/vp9.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/kanstream/stream/base.py` & `kanstream-2.1.0/kanstream/stream/base.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/kanstream/stream/frame_pb2.py` & `kanstream-2.1.0/kanstream/stream/frame_pb2.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/kanstream/stream/protobuf.py` & `kanstream-2.1.0/kanstream/stream/protobuf.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/kanstream/stream/receiver.py` & `kanstream-2.1.0/kanstream/stream/receiver.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/kanstream/stream/sender.py` & `kanstream-2.1.0/kanstream/stream/sender.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/kanstream/utils/calculate_bitrate.py` & `kanstream-2.1.0/kanstream/utils/calculate_bitrate.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/kanstream.egg-info/PKG-INFO` & `kanstream-2.1.0/kanstream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kanstream
-Version: 2.0.4
+Version: 2.1.0
 Summary: pull and push stream
 Home-page: UNKNOWN
 Author: flinzhao
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `kanstream-2.0.4/kanstream.egg-info/SOURCES.txt` & `kanstream-2.1.0/kanstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.4/setup.py` & `kanstream-2.1.0/setup.py`

 * *Files identical despite different names*

