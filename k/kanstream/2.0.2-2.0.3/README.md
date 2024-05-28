# Comparing `tmp/kanstream-2.0.2.tar.gz` & `tmp/kanstream-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanstream-2.0.2.tar", last modified: Tue May 28 03:37:36 2024, max compression
+gzip compressed data, was "kanstream-2.0.3.tar", last modified: Tue May 28 07:53:59 2024, max compression
```

## Comparing `kanstream-2.0.2.tar` & `kanstream-2.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:37:36.917945 kanstream-2.0.2/
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-28 01:34:51.000000 kanstream-2.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2870 2024-05-28 03:37:36.917945 kanstream-2.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2653 2024-05-28 02:58:56.000000 kanstream-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:37:36.914945 kanstream-2.0.2/kanstream/
--rw-r--r--   0 root         (0) root         (0)     3521 2024-05-28 03:36:28.000000 kanstream-2.0.2/kanstream/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:37:36.915945 kanstream-2.0.2/kanstream/codec/
--rw-r--r--   0 root         (0) root         (0)       36 2024-05-27 07:56:18.000000 kanstream-2.0.2/kanstream/codec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      406 2024-05-27 07:22:05.000000 kanstream-2.0.2/kanstream/codec/abc.py
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-27 07:45:11.000000 kanstream-2.0.2/kanstream/codec/codec.py
--rw-r--r--   0 root         (0) root         (0)     3269 2024-05-27 09:02:44.000000 kanstream-2.0.2/kanstream/codec/h264.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-05-27 07:23:03.000000 kanstream-2.0.2/kanstream/codec/vp9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:37:36.916945 kanstream-2.0.2/kanstream/stream/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:23:08.000000 kanstream-2.0.2/kanstream/stream/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1746 2024-05-28 03:32:03.000000 kanstream-2.0.2/kanstream/stream/base.py
--rw-r--r--   0 root         (0) root         (0)      972 2024-05-27 06:35:39.000000 kanstream-2.0.2/kanstream/stream/frame_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1402 2024-05-27 06:23:08.000000 kanstream-2.0.2/kanstream/stream/protobuf.py
--rw-r--r--   0 root         (0) root         (0)     2451 2024-05-28 03:32:49.000000 kanstream-2.0.2/kanstream/stream/receiver.py
--rw-r--r--   0 root         (0) root         (0)     2176 2024-05-27 10:08:54.000000 kanstream-2.0.2/kanstream/stream/sender.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:37:36.917945 kanstream-2.0.2/kanstream/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:23:08.000000 kanstream-2.0.2/kanstream/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1297 2024-05-27 06:23:08.000000 kanstream-2.0.2/kanstream/utils/calculate_bitrate.py
--rw-r--r--   0 root         (0) root         (0)      489 2024-05-28 01:46:00.000000 kanstream-2.0.2/kanstream/utils/frame_queue.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-28 03:31:52.000000 kanstream-2.0.2/kanstream/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 03:37:36.914945 kanstream-2.0.2/kanstream.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2870 2024-05-28 03:37:36.000000 kanstream-2.0.2/kanstream.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      642 2024-05-28 03:37:36.000000 kanstream-2.0.2/kanstream.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 03:37:36.000000 kanstream-2.0.2/kanstream.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 03:37:36.000000 kanstream-2.0.2/kanstream.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 03:37:36.000000 kanstream-2.0.2/kanstream.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 01:19:21.000000 kanstream-2.0.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 03:37:36.917945 kanstream-2.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1018 2024-05-28 03:01:29.000000 kanstream-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 07:53:59.722056 kanstream-2.0.3/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-28 01:34:51.000000 kanstream-2.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2870 2024-05-28 07:53:59.722056 kanstream-2.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2653 2024-05-28 02:58:56.000000 kanstream-2.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 07:53:59.719057 kanstream-2.0.3/kanstream/
+-rw-r--r--   0 root         (0) root         (0)     3521 2024-05-28 03:36:28.000000 kanstream-2.0.3/kanstream/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 07:53:59.721057 kanstream-2.0.3/kanstream/codec/
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-27 07:56:18.000000 kanstream-2.0.3/kanstream/codec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      406 2024-05-27 07:22:05.000000 kanstream-2.0.3/kanstream/codec/abc.py
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-27 07:45:11.000000 kanstream-2.0.3/kanstream/codec/codec.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-05-28 07:53:19.000000 kanstream-2.0.3/kanstream/codec/h264.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-27 07:23:03.000000 kanstream-2.0.3/kanstream/codec/vp9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 07:53:59.721057 kanstream-2.0.3/kanstream/stream/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:23:08.000000 kanstream-2.0.3/kanstream/stream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2024-05-28 03:32:03.000000 kanstream-2.0.3/kanstream/stream/base.py
+-rw-r--r--   0 root         (0) root         (0)      972 2024-05-27 06:35:39.000000 kanstream-2.0.3/kanstream/stream/frame_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2024-05-27 06:23:08.000000 kanstream-2.0.3/kanstream/stream/protobuf.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2024-05-28 03:32:49.000000 kanstream-2.0.3/kanstream/stream/receiver.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2024-05-27 10:08:54.000000 kanstream-2.0.3/kanstream/stream/sender.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 07:53:59.721057 kanstream-2.0.3/kanstream/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 06:23:08.000000 kanstream-2.0.3/kanstream/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2024-05-27 06:23:08.000000 kanstream-2.0.3/kanstream/utils/calculate_bitrate.py
+-rw-r--r--   0 root         (0) root         (0)      489 2024-05-28 01:46:00.000000 kanstream-2.0.3/kanstream/utils/frame_queue.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-28 07:53:52.000000 kanstream-2.0.3/kanstream/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 07:53:59.719057 kanstream-2.0.3/kanstream.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2870 2024-05-28 07:53:59.000000 kanstream-2.0.3/kanstream.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      642 2024-05-28 07:53:59.000000 kanstream-2.0.3/kanstream.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 07:53:59.000000 kanstream-2.0.3/kanstream.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 07:53:59.000000 kanstream-2.0.3/kanstream.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 07:53:59.000000 kanstream-2.0.3/kanstream.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 01:19:21.000000 kanstream-2.0.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 07:53:59.722056 kanstream-2.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-05-28 03:01:29.000000 kanstream-2.0.3/setup.py
```

### Comparing `kanstream-2.0.2/PKG-INFO` & `kanstream-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kanstream
-Version: 2.0.2
+Version: 2.0.3
 Summary: pull and push stream
 Home-page: UNKNOWN
 Author: flinzhao
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `kanstream-2.0.2/README.md` & `kanstream-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.2/kanstream/__init__.py` & `kanstream-2.0.3/kanstream/__init__.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.2/kanstream/codec/codec.py` & `kanstream-2.0.3/kanstream/codec/codec.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.2/kanstream/codec/h264.py` & `kanstream-2.0.3/kanstream/codec/h264.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def __init__(self) -> None:
         super().__init__()
         self._save_video = None
         self._stream = None
         self._container = None
 
     def set_config(self, height: int, width: int, fps: int, gop_size=60, bit_rate=0):
-        container: av.OutputContainer = av.open('output.mp4', 'w')
+        container: av.OutputContainer = av.open('output.h264', 'w')
         stream: av.video.stream.VideoStream = container.add_stream('h264', rate=30)
 
         # 编码器相关配置
         bit_rate = bit_rate if bit_rate > 0 else calculate_bitrate(width, height, fps) * 2
         codec_context = stream.codec_context
         codec_context.bit_rate = bit_rate * 1000
         codec_context.bit_rate_tolerance = 200 * 1000
```

### Comparing `kanstream-2.0.2/kanstream/stream/base.py` & `kanstream-2.0.3/kanstream/stream/base.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.2/kanstream/stream/frame_pb2.py` & `kanstream-2.0.3/kanstream/stream/frame_pb2.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.2/kanstream/stream/protobuf.py` & `kanstream-2.0.3/kanstream/stream/protobuf.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.2/kanstream/stream/receiver.py` & `kanstream-2.0.3/kanstream/stream/receiver.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.2/kanstream/stream/sender.py` & `kanstream-2.0.3/kanstream/stream/sender.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.2/kanstream/utils/calculate_bitrate.py` & `kanstream-2.0.3/kanstream/utils/calculate_bitrate.py`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.2/kanstream.egg-info/PKG-INFO` & `kanstream-2.0.3/kanstream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kanstream
-Version: 2.0.2
+Version: 2.0.3
 Summary: pull and push stream
 Home-page: UNKNOWN
 Author: flinzhao
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `kanstream-2.0.2/kanstream.egg-info/SOURCES.txt` & `kanstream-2.0.3/kanstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kanstream-2.0.2/setup.py` & `kanstream-2.0.3/setup.py`

 * *Files identical despite different names*

