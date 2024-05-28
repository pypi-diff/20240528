# Comparing `tmp/silero-vad-0.0.4.tar.gz` & `tmp/silero-vad-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silero-vad-0.0.4.tar", last modified: Thu May 23 15:10:02 2024, max compression
+gzip compressed data, was "silero-vad-0.0.5.tar", last modified: Tue May 28 03:21:33 2024, max compression
```

## Comparing `silero-vad-0.0.4.tar` & `silero-vad-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:02.065923 silero-vad-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 15:10:01.000000 silero-vad-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 15:10:01.000000 silero-vad-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-23 15:10:02.065923 silero-vad-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-23 15:10:01.000000 silero-vad-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 15:10:01.000000 silero-vad-0.0.4/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 15:10:01.000000 silero-vad-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:10:02.065923 silero-vad-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-23 15:10:01.000000 silero-vad-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:02.065923 silero-vad-0.0.4/silero_vad/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/frame_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/inference_session.py
--rw-r--r--   0 runner    (1001) docker     (127)  1807522 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/silero_vad.onnx
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/silero_vad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-23 15:10:01.000000 silero-vad-0.0.4/silero_vad/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:10:02.065923 silero-vad-0.0.4/silero_vad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-23 15:10:02.000000 silero-vad-0.0.4/silero_vad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-23 15:10:02.000000 silero-vad-0.0.4/silero_vad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:10:02.000000 silero-vad-0.0.4/silero_vad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 15:10:02.000000 silero-vad-0.0.4/silero_vad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 15:10:02.000000 silero-vad-0.0.4/silero_vad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 15:10:02.000000 silero-vad-0.0.4/silero_vad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:21:33.566980 silero-vad-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 03:21:33.000000 silero-vad-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 03:21:33.000000 silero-vad-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-28 03:21:33.566980 silero-vad-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 03:21:33.000000 silero-vad-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 03:21:33.000000 silero-vad-0.0.5/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 03:21:33.000000 silero-vad-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 03:21:33.566980 silero-vad-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-28 03:21:33.000000 silero-vad-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:21:33.566980 silero-vad-0.0.5/silero_vad/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/frame_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/inference_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1807522 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/silero_vad.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/silero_vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:21:33.566980 silero-vad-0.0.5/silero_vad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 03:21:33.000000 silero-vad-0.0.5/silero_vad.egg-info/top_level.txt
```

### Comparing `silero-vad-0.0.4/LICENSE` & `silero-vad-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.4/PKG-INFO` & `silero-vad-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-vad
-Version: 0.0.4
+Version: 0.0.5
 Summary: Silero VAD
 Home-page: https://github.com/pengzhendong/silero-vad
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `silero-vad-0.0.4/setup.py` & `silero-vad-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.4/silero_vad/__init__.py` & `silero-vad-0.0.5/silero_vad/__init__.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.4/silero_vad/cli.py` & `silero-vad-0.0.5/silero_vad/cli.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.4/silero_vad/frame_queue.py` & `silero-vad-0.0.5/silero_vad/frame_queue.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.4/silero_vad/inference_session.py` & `silero-vad-0.0.5/silero_vad/inference_session.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.4/silero_vad/silero_vad.onnx` & `silero-vad-0.0.5/silero_vad/silero_vad.onnx`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.4/silero_vad/silero_vad.py` & `silero-vad-0.0.5/silero_vad/silero_vad.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,18 +245,20 @@
                     current_speech = {}
                     prev_end = 0
                     next_start = 0
                     temp_end = 0
                     triggered = False
 
         # deal with the last speech segment
-        if current_speech and len(wav) - current_speech["start"] > min_speech_samples:
-            current_speech["end"] = len(wav)
-            yield fn(idx, current_speech)
-            idx += 1
+        if current_speech:
+            end = len(wav) // queue.step
+            if end - current_speech["start"] > min_speech_samples:
+                current_speech["end"] = end
+                yield fn(idx, current_speech)
+                idx += 1
 
 
 class VADIterator:
     def __init__(
         self,
         threshold: float = 0.5,
         sampling_rate: int = 16000,
```

### Comparing `silero-vad-0.0.4/silero_vad/utils.py` & `silero-vad-0.0.5/silero_vad/utils.py`

 * *Files identical despite different names*

### Comparing `silero-vad-0.0.4/silero_vad.egg-info/PKG-INFO` & `silero-vad-0.0.5/silero_vad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-vad
-Version: 0.0.4
+Version: 0.0.5
 Summary: Silero VAD
 Home-page: https://github.com/pengzhendong/silero-vad
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

