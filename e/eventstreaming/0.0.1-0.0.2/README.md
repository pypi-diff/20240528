# Comparing `tmp/eventstreaming-0.0.1.tar.gz` & `tmp/eventstreaming-0.0.2.tar.gz`

## Comparing `eventstreaming-0.0.1.tar` & `eventstreaming-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/__init__.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/io_event.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/screen_recorder.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/websocket/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/websocket/index.html
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/websocket/index.js
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/websocket/io_event.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/websocket/screen_recorder.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/websocket/server.py
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/websocket/stream.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/websocket/video.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/websocket/web_server.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/src/eventstreaming/websocket/ws_server.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/tests/dino.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/tests/ffmpeg.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/tests/record.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/tests/screen.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/tests/test.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/tests/test_mss.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/tests/tk.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/tests/tkk.py
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/LICENSE
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/README.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 eventstreaming-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/__init__.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/io_event.py
+-rwxr-xr-x   0        0        0     3064 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/screen_recorder.py
+-rwxr-xr-x   0        0        0     2960 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/websocket/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/websocket/index.html
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/websocket/index.js
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/websocket/io_event.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/websocket/screen_recorder.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/websocket/server.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/websocket/stream.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/websocket/video.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/websocket/web_server.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/src/eventstreaming/websocket/ws_server.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/tests/dino.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/tests/ffmpeg.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/tests/record.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/tests/screen.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/tests/test.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/tests/test_mss.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/tests/tk.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/tests/tkk.py
+-rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/LICENSE
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/README.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 eventstreaming-0.0.2/PKG-INFO
```

### Comparing `eventstreaming-0.0.1/src/eventstreaming/io_event.py` & `eventstreaming-0.0.2/src/eventstreaming/io_event.py`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/src/eventstreaming/screen_recorder.py` & `eventstreaming-0.0.2/src/eventstreaming/screen_recorder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,81 @@
 import threading
 import time
+import sys
 import mss
-from PIL import Image
+from PIL import Image, ImageGrab
+import pyautogui
 from eventstreaming import stream
 
 start_time = 0
 screen_thread = None
 terminate = False
 
 def main(left=None, top=None, width=None, height=None, new_width=None, new_height=None, fullscreen=False):
-    with mss.mss() as sct:
-        monitors = sct.monitors
-        monitor = monitors[1]
+    if sys.platform == 'win32':
+        size = pyautogui.size()
 
         if fullscreen:
-            left = monitor['left']
-            top = monitor['top']
-            width = monitor['width']
-            height = monitor['height']
+            left = 0
+            top = 0
+            width = size.width
+            height = size.height
         if left is None:
-            left = monitor['left']
+            left = 0
         if top is None:
-            top = monitor['top']
+            top = 0
         if width is None:
-            width = monitor['width']
+            width = size.width
         if height is None:
-            height = monitor['height']
+            height = size.height
         if new_width is None:
             new_width = width
         if new_height is None:
             new_height = height
-
+        
         while not terminate:
-            screenshot = sct.grab({'left': left, 'top': top, 'width': width, 'height': height})
-            img = Image.frombytes('RGB', (screenshot.width, screenshot.height), screenshot.rgb)
+            img = ImageGrab.grab(bbox=(left, top, left + width, top + height))
             resized_img = img.resize((new_width, new_height), Image.Resampling.LANCZOS)
             timestamp = int((time.time() - start_time) * 1_000_000)
             stream.add_video_frame({
                 'image': resized_img,
                 'timestamp': timestamp
             })
+    else:
+        with mss.mss() as sct:
+            monitors = sct.monitors
+            monitor = monitors[1]
+
+            if fullscreen:
+                left = monitor['left']
+                top = monitor['top']
+                width = monitor['width']
+                height = monitor['height']
+            if left is None:
+                left = monitor['left']
+            if top is None:
+                top = monitor['top']
+            if width is None:
+                width = monitor['width']
+            if height is None:
+                height = monitor['height']
+            if new_width is None:
+                new_width = width
+            if new_height is None:
+                new_height = height
+
+            while not terminate:
+                screenshot = sct.grab({'left': left, 'top': top, 'width': width, 'height': height})
+                img = Image.frombytes('RGB', (screenshot.width, screenshot.height), screenshot.rgb)
+                resized_img = img.resize((new_width, new_height), Image.Resampling.LANCZOS)
+                timestamp = int((time.time() - start_time) * 1_000_000)
+                stream.add_video_frame({
+                    'image': resized_img,
+                    'timestamp': timestamp
+                })
 
 def start(left=None, top=None, width=None, height=None, new_width=None, new_height=None, fullscreen=False):
     global start_time, screen_thread, terminate
     start_time = time.time()
     terminate = False
     screen_thread = threading.Thread(target=main, args=(left, top, width, height, new_width, new_height, fullscreen), daemon=True)
     screen_thread.start()
```

### Comparing `eventstreaming-0.0.1/src/eventstreaming/stream.py` & `eventstreaming-0.0.2/src/eventstreaming/stream.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,18 +49,18 @@
     tmp_inputs = []
     state = 'start'
     while True:
         input = get_io_event()
         while input is None:
             time.sleep(0.001)
             input = get_io_event()
-        if state =='start' and input['event'] == 'p ctrl':
-            state = 'p ctrl'
+        if state =='start' and (input['event'] == 'p alt' or input['event'] == 'p alt_l'):
+            state = 'alt'
             tmp_inputs.append(input)
-        elif state =='p ctrl' and input['event'] == 'pr':
+        elif state =='alt' and input['event'] == 'pr':
             state = 'end'
             break
         else:
             if state != 'end' and len(tmp_inputs) > 0:
                 inputs.extend(tmp_inputs)
                 tmp_inputs = []
             state = 'start'
```

### Comparing `eventstreaming-0.0.1/src/eventstreaming/websocket/index.html` & `eventstreaming-0.0.2/src/eventstreaming/websocket/index.html`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/src/eventstreaming/websocket/index.js` & `eventstreaming-0.0.2/src/eventstreaming/websocket/index.js`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/src/eventstreaming/websocket/io_event.py` & `eventstreaming-0.0.2/src/eventstreaming/websocket/io_event.py`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/src/eventstreaming/websocket/screen_recorder.py` & `eventstreaming-0.0.2/src/eventstreaming/websocket/screen_recorder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import threading
 import time
 import websocket
 import av
+import sys
 import mss
+from PIL import ImageGrab
+import pyautogui
 import numpy as np
 import struct
 
 start_time = 0
 ws_thread = None
 screen_thread = None
 terminate = False
@@ -39,54 +42,93 @@
     is_keyframe = packet.is_keyframe
     data = bytes(packet)
     header = struct.pack('<BBBBQI', 0, 0, 0, is_keyframe, timestamp, len(data))
     if not terminate:
         ws.send(header + data, websocket.ABNF.OPCODE_BINARY)
 
 def main(left=None, top=None, width=None, height=None, new_width=None, new_height=None, fullscreen=False):
-    with mss.mss() as sct:
-        monitors = sct.monitors
-        monitor = monitors[1]
+    if sys.platform == 'win32':
+        size = pyautogui.size()
 
         if fullscreen:
-            left = monitor['left']
-            top = monitor['top']
-            width = monitor['width']
-            height = monitor['height']
+            left = 0
+            top = 0
+            width = size.width
+            height = size.height
         if left is None:
-            left = monitor['left']
+            left = 0
         if top is None:
-            top = monitor['top']
+            top = 0
         if width is None:
-            width = monitor['width']
+            width = size.width
         if height is None:
-            height = monitor['height']
+            height = size.height
         if new_width is None:
             new_width = width
         if new_height is None:
             new_height = height
 
         codec = av.codec.CodecContext.create('vp9', 'w')
         codec.width = new_width
         codec.height = new_height
         codec.pix_fmt = 'yuv420p'
         codec.bit_rate = 2_000_000
         codec.options = {'profile': '0'}
-
+        
         while not terminate:
-            screenshot = sct.grab({'left': left, 'top': top, 'width': width, 'height': height})
+            screenshot = ImageGrab.grab(bbox=(left, top, left + width, top + height))
             img = np.array(screenshot)
             frame = av.VideoFrame.from_ndarray(img, format='bgra')
             frame = frame.reformat(width=codec.width, height=codec.height, format='yuv420p')
             for packet in codec.encode(frame):
                 send_packet(packet)
             time.sleep(0.001)
-    
-    for packet in codec.encode():
-        send_packet(packet)
+        for packet in codec.encode():
+            send_packet(packet)
+    else:
+        with mss.mss() as sct:
+            monitors = sct.monitors
+            monitor = monitors[1]
+
+            if fullscreen:
+                left = monitor['left']
+                top = monitor['top']
+                width = monitor['width']
+                height = monitor['height']
+            if left is None:
+                left = monitor['left']
+            if top is None:
+                top = monitor['top']
+            if width is None:
+                width = monitor['width']
+            if height is None:
+                height = monitor['height']
+            if new_width is None:
+                new_width = width
+            if new_height is None:
+                new_height = height
+
+            codec = av.codec.CodecContext.create('vp9', 'w')
+            codec.width = new_width
+            codec.height = new_height
+            codec.pix_fmt = 'yuv420p'
+            codec.bit_rate = 2_000_000
+            codec.options = {'profile': '0'}
+
+            while not terminate:
+                screenshot = sct.grab({'left': left, 'top': top, 'width': width, 'height': height})
+                img = np.array(screenshot)
+                frame = av.VideoFrame.from_ndarray(img, format='bgra')
+                frame = frame.reformat(width=codec.width, height=codec.height, format='yuv420p')
+                for packet in codec.encode(frame):
+                    send_packet(packet)
+                time.sleep(0.001)
+        
+        for packet in codec.encode():
+            send_packet(packet)
 
 def start(left=None, top=None, width=None, height=None, new_width=None, new_height=None, fullscreen=False):
     global ws, start_time, ws_thread, screen_thread, terminate
     start_time = time.time()
     terminate = False
     ws_thread = threading.Thread(target=ws.run_forever, daemon=True)
     ws_thread.start()
```

### Comparing `eventstreaming-0.0.1/src/eventstreaming/websocket/stream.py` & `eventstreaming-0.0.2/src/eventstreaming/websocket/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,18 +77,18 @@
     tmp_inputs = []
     state = 'start'
     while True:
         input = get_io_event()
         while input is None:
             time.sleep(0.001)
             input = get_io_event()
-        if state =='start' and input['event'] == 'p ctrl':
-            state = 'p ctrl'
+        if state =='start' and (input['event'] == 'p alt' or input['event'] == 'p alt_l'):
+            state = 'alt'
             tmp_inputs.append(input)
-        elif state =='p ctrl' and input['event'] == 'pr':
+        elif state =='alt' and input['event'] == 'pr':
             state = 'end'
             break
         else:
             if state != 'end' and len(tmp_inputs) > 0:
                 inputs.extend(tmp_inputs)
                 tmp_inputs = []
             state = 'start'
```

### Comparing `eventstreaming-0.0.1/src/eventstreaming/websocket/video.py` & `eventstreaming-0.0.2/src/eventstreaming/websocket/video.py`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/src/eventstreaming/websocket/web_server.py` & `eventstreaming-0.0.2/src/eventstreaming/websocket/web_server.py`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/src/eventstreaming/websocket/ws_server.py` & `eventstreaming-0.0.2/src/eventstreaming/websocket/ws_server.py`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/tests/dino.py` & `eventstreaming-0.0.2/tests/dino.py`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/tests/ffmpeg.py` & `eventstreaming-0.0.2/tests/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/tests/screen.py` & `eventstreaming-0.0.2/tests/screen.py`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/tests/test.py` & `eventstreaming-0.0.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/tests/test_mss.py` & `eventstreaming-0.0.2/tests/test_mss.py`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/tests/tk.py` & `eventstreaming-0.0.2/tests/tk.py`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/tests/tkk.py` & `eventstreaming-0.0.2/tests/tkk.py`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/.gitignore` & `eventstreaming-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/LICENSE` & `eventstreaming-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eventstreaming-0.0.1/pyproject.toml` & `eventstreaming-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "eventstreaming"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="timcsy", email="timocsy@yahoo.com.tw" },
 ]
 description = "Event streaming library."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "pynput>=1.7",
+    "pyautogui",
+    "Pillow",
     "websockets>=10.1",
     "av>=9",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/timcsy/eventstreaming"
 "Bug Tracker" = "https://github.com/timcsy/eventstreaming/issues"
```

### Comparing `eventstreaming-0.0.1/PKG-INFO` & `eventstreaming-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.3
 Name: eventstreaming
-Version: 0.0.1
+Version: 0.0.2
 Summary: Event streaming library.
 Project-URL: Homepage, https://github.com/timcsy/eventstreaming
 Project-URL: Bug Tracker, https://github.com/timcsy/eventstreaming/issues
 Author-email: timcsy <timocsy@yahoo.com.tw>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: av>=9
+Requires-Dist: pillow
+Requires-Dist: pyautogui
 Requires-Dist: pynput>=1.7
 Requires-Dist: websockets>=10.1
 Description-Content-Type: text/markdown
 
 # EventStreaming
 
 Streaming the screen, keyboard and mouse evnts.
```

