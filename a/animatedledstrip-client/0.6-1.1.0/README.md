# Comparing `tmp/animatedledstrip-client-0.6.tar.gz` & `tmp/animatedledstrip_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/animatedledstrip-client-0.6.tar", last modified: Sat Jan 18 02:36:46 2020, max compression
+gzip compressed data, was "animatedledstrip_client-1.1.0.tar", last modified: Tue May 28 19:34:03 2024, max compression
```

## Comparing `animatedledstrip-client-0.6.tar` & `animatedledstrip_client-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,35 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 02:36:46.000000 animatedledstrip-client-0.6/
--rw-rw-r--   0 travis    (2000) travis    (2000)      347 2020-01-18 02:36:46.000000 animatedledstrip-client-0.6/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 02:36:46.000000 animatedledstrip-client-0.6/animatedledstrip_client.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      347 2020-01-18 02:36:46.000000 animatedledstrip-client-0.6/animatedledstrip_client.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      488 2020-01-18 02:36:46.000000 animatedledstrip-client-0.6/animatedledstrip_client.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-18 02:36:46.000000 animatedledstrip-client-0.6/animatedledstrip_client.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2020-01-18 02:36:46.000000 animatedledstrip-client-0.6/animatedledstrip_client.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 02:36:46.000000 animatedledstrip-client-0.6/client/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1794 2020-01-18 02:36:26.000000 animatedledstrip-client-0.6/client/Animation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4188 2020-01-18 02:36:26.000000 animatedledstrip-client-0.6/client/AnimationData.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1616 2020-01-18 02:36:26.000000 animatedledstrip-client-0.6/client/AnimationSender.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1456 2020-01-18 02:36:26.000000 animatedledstrip-client-0.6/client/ColorContainer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1229 2020-01-18 02:36:26.000000 animatedledstrip-client-0.6/client/Direction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-18 02:36:26.000000 animatedledstrip-client-0.6/client/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      200 2020-01-18 02:36:46.000000 animatedledstrip-client-0.6/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      417 2020-01-18 02:36:26.000000 animatedledstrip-client-0.6/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 02:36:46.000000 animatedledstrip-client-0.6/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-18 02:36:26.000000 animatedledstrip-client-0.6/test/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-18 02:36:46.000000 animatedledstrip-client-0.6/test/client/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-18 02:36:26.000000 animatedledstrip-client-0.6/test/client/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6161 2020-01-18 02:36:26.000000 animatedledstrip-client-0.6/test/client/test_animation_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1327 2020-01-18 02:36:26.000000 animatedledstrip-client-0.6/test/client/test_animation_sender.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2020-01-18 02:36:26.000000 animatedledstrip-client-0.6/test/client/test_colorcontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:34:03.856016 animatedledstrip_client-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-28 19:34:03.856016 animatedledstrip_client-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:34:03.856016 animatedledstrip_client-1.1.0/animatedledstrip/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/als_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/animation_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/animation_to_run_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/color_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/equation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/json_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/new_animation_group_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/running_animation_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/animatedledstrip/strip_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:34:03.856016 animatedledstrip_client-1.1.0/animatedledstrip_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-28 19:34:03.000000 animatedledstrip_client-1.1.0/animatedledstrip_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-28 19:34:03.000000 animatedledstrip_client-1.1.0/animatedledstrip_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:34:03.000000 animatedledstrip_client-1.1.0/animatedledstrip_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 19:34:03.000000 animatedledstrip_client-1.1.0/animatedledstrip_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-28 19:34:03.856016 animatedledstrip_client-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:34:03.856016 animatedledstrip_client-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:34:03.856016 animatedledstrip_client-1.1.0/test/animatedledstrip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/test/animatedledstrip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/test/animatedledstrip/test_animation_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/test/animatedledstrip/test_colorcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/test/animatedledstrip/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-28 19:34:00.000000 animatedledstrip_client-1.1.0/test/animatedledstrip/test_strip_info.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `animatedledstrip-client-0.6/client/AnimationSender.py` & `animatedledstrip_client-1.1.0/animatedledstrip/section.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-#   Copyright (c) 2019-2020 AnimatedLEDStrip
+#  Copyright (c) 2018-2021 AnimatedLEDStrip
 #
-#   Permission is hereby granted, free of charge, to any person obtaining a copy
-#   of this software and associated documentation files (the "Software"), to deal
-#   in the Software without restriction, including without limitation the rights
-#   to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-#   copies of the Software, and to permit persons to whom the Software is
-#   furnished to do so, subject to the following conditions:
+#  Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
 #
-#   The above copyright notice and this permission notice shall be included in
-#   all copies or substantial portions of the Software.
+#  The above copyright notice and this permission notice shall be included in
+#  all copies or substantial portions of the Software.
 #
-#   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-#   IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-#   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-#   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-#   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-#   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-#   THE SOFTWARE.
-
-import socket
-
-
-class AnimationSender(object):
-
-    def __init__(self, ip_address, port_num):
-        self.address = ip_address
-        self.port = port_num
-        self.connection = socket.socket()
-
-    def start(self):
-        self.connection = socket.create_connection((self.address, self.port))
-
-    def end(self):
-        self.connection.close()
-
-    def send_animation(self, animation_json):
-        json = bytearray(animation_json, "utf-8")
-        self.connection.send(json)
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+#  THE SOFTWARE.
+
+from typing import Dict, List, Optional
+
+
+class Section(object):
+    """Stores information about a section of the LED strip"""
+
+    def __init__(self,
+                 name: str = '',
+                 pixels: Optional[List[int]] = None,
+                 parent_section_name: str = ''):
+        self.name: str = name
+        self.parent_section_name: str = parent_section_name
+
+        if pixels is None:
+            self.pixels: List[int] = []
+        else:
+            self.pixels: List[int] = pixels
+
+    def json_dict(self) -> Dict:
+        return {
+            'name': self.name,
+            'pixels': self.pixels,
+            'parentSectionName': self.parent_section_name,
+        }
```

### Comparing `animatedledstrip-client-0.6/client/Direction.py` & `animatedledstrip_client-1.1.0/animatedledstrip/json_encoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,34 @@
-#   Copyright (c) 2019-2020 AnimatedLEDStrip
+#  Copyright (c) 2018-2021 AnimatedLEDStrip
 #
-#   Permission is hereby granted, free of charge, to any person obtaining a copy
-#   of this software and associated documentation files (the "Software"), to deal
-#   in the Software without restriction, including without limitation the rights
-#   to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-#   copies of the Software, and to permit persons to whom the Software is
-#   furnished to do so, subject to the following conditions:
+#  Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
 #
-#   The above copyright notice and this permission notice shall be included in
-#   all copies or substantial portions of the Software.
+#  The above copyright notice and this permission notice shall be included in
+#  all copies or substantial portions of the Software.
 #
-#   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-#   IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-#   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-#   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-#   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-#   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-#   THE SOFTWARE.
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+#  THE SOFTWARE.
 
-from enum import Enum, auto
+import json
+from json import JSONEncoder
+from typing import Any
 
 
-class Direction(Enum):
-    FORWARD = auto()
-    BACKWARD = auto()
+class ALSJsonEncoder(JSONEncoder):
+
+    def default(self, o: Any) -> Any:
+        # print(type(o))
+        if hasattr(o, 'json_dict'):
+            # noinspection PyCallingNonCallable
+            return o.json_dict()
+        else:
+            return json.JSONEncoder.default(self, o)
```

### Comparing `animatedledstrip-client-0.6/test/client/test_animation_sender.py` & `animatedledstrip_client-1.1.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,21 @@
-#   Copyright (c) 2019-2020 AnimatedLEDStrip
-#
-#   Permission is hereby granted, free of charge, to any person obtaining a copy
-#   of this software and associated documentation files (the "Software"), to deal
-#   in the Software without restriction, including without limitation the rights
-#   to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-#   copies of the Software, and to permit persons to whom the Software is
-#   furnished to do so, subject to the following conditions:
-#
-#   The above copyright notice and this permission notice shall be included in
-#   all copies or substantial portions of the Software.
-#
-#   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-#   IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-#   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-#   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-#   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-#   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-#   THE SOFTWARE.
+MIT License
 
-from client.AnimationSender import AnimationSender
+Copyright (c) 2018-2020 AnimatedLEDStrip
 
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-def test_constructor():
-    sender = AnimationSender("10.0.0.254", 5)
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
 
-    assert sender.address == "10.0.0.254"
-    assert sender.port == 5
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `animatedledstrip-client-0.6/test/client/test_colorcontainer.py` & `animatedledstrip_client-1.1.0/animatedledstrip/location.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,40 @@
-#   Copyright (c) 2019-2020 AnimatedLEDStrip
+#  Copyright (c) 2018-2021 AnimatedLEDStrip
 #
-#   Permission is hereby granted, free of charge, to any person obtaining a copy
-#   of this software and associated documentation files (the "Software"), to deal
-#   in the Software without restriction, including without limitation the rights
-#   to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-#   copies of the Software, and to permit persons to whom the Software is
-#   furnished to do so, subject to the following conditions:
+#  Permission is hereby granted, free of charge, to any person obtaining a copy
+#  of this software and associated documentation files (the "Software"), to deal
+#  in the Software without restriction, including without limitation the rights
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+#  copies of the Software, and to permit persons to whom the Software is
+#  furnished to do so, subject to the following conditions:
 #
-#   The above copyright notice and this permission notice shall be included in
-#   all copies or substantial portions of the Software.
+#  The above copyright notice and this permission notice shall be included in
+#  all copies or substantial portions of the Software.
 #
-#   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-#   IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-#   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-#   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-#   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-#   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-#   THE SOFTWARE.
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+#  THE SOFTWARE.
 
-from client.ColorContainer import ColorContainer
+from typing import Dict
 
 
-def test_colorcontainer():
-    color = ColorContainer()
+class Location(object):
+    """A location in 3D space"""
 
-    color.add_color(0xFF)
+    def __init__(self,
+                 x: float = 0.0,
+                 y: float = 0.0,
+                 z: float = 0.0):
+        self.x: float = x
+        self.y: float = y
+        self.z: float = z
 
-    try:
-        color.add_color(None)
-        raise AssertionError
-    except ValueError:
-        pass
+    def json_dict(self) -> Dict:
+        return {
+            'x': self.x,
+            'y': self.y,
+            'z': self.z,
+        }
```

