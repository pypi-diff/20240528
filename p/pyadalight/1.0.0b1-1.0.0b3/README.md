# Comparing `tmp/pyadalight-1.0.0b1.tar.gz` & `tmp/pyadalight-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyadalight-1.0.0b1.tar", last modified: Mon Jun 26 14:01:52 2023, max compression
+gzip compressed data, was "pyadalight-1.0.0b3.tar", max compression
```

## Comparing `pyadalight-1.0.0b1.tar` & `pyadalight-1.0.0b3.tar`

### file list

```diff
@@ -1,20 +1,10 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 14:01:52.110104 pyadalight-1.0.0b1/
--rwxrwxrwx   0 root         (0) root         (0)     1072 2023-06-25 16:38:05.000000 pyadalight-1.0.0b1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1318 2023-06-26 14:01:52.089574 pyadalight-1.0.0b1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      616 2023-06-26 14:01:19.000000 pyadalight-1.0.0b1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 14:01:52.070184 pyadalight-1.0.0b1/pyadalight/
--rwxrwxrwx   0 root         (0) root         (0)       24 2023-06-25 16:39:28.000000 pyadalight-1.0.0b1/pyadalight/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       64 2023-06-26 09:29:43.000000 pyadalight-1.0.0b1/pyadalight/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     6233 2023-06-26 13:49:19.000000 pyadalight-1.0.0b1/pyadalight/adalight.py
--rwxrwxrwx   0 root         (0) root         (0)     3406 2023-06-26 13:53:44.000000 pyadalight-1.0.0b1/pyadalight/main.py
--rwxrwxrwx   0 root         (0) root         (0)      239 2023-06-25 14:37:51.000000 pyadalight-1.0.0b1/pyadalight/singleton.py
--rwxrwxrwx   0 root         (0) root         (0)     1456 2023-06-25 15:26:30.000000 pyadalight-1.0.0b1/pyadalight/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 14:01:52.088315 pyadalight-1.0.0b1/pyadalight.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1318 2023-06-26 14:01:51.000000 pyadalight-1.0.0b1/pyadalight.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      364 2023-06-26 14:01:51.000000 pyadalight-1.0.0b1/pyadalight.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-26 14:01:51.000000 pyadalight-1.0.0b1/pyadalight.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       81 2023-06-26 14:01:51.000000 pyadalight-1.0.0b1/pyadalight.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       76 2023-06-26 14:01:51.000000 pyadalight-1.0.0b1/pyadalight.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-06-26 14:01:51.000000 pyadalight-1.0.0b1/pyadalight.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-26 14:01:52.110762 pyadalight-1.0.0b1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1267 2023-06-26 09:36:23.000000 pyadalight-1.0.0b1/setup.py
+-rwxr-xr-x   0        0        0     1072 2023-06-25 16:38:05.814611 pyadalight-1.0.0b3/LICENSE
+-rwxr-xr-x   0        0        0      616 2023-06-26 14:01:19.125534 pyadalight-1.0.0b3/README.md
+-rwxr-xr-x   0        0        0       34 2024-02-16 12:57:32.500362 pyadalight-1.0.0b3/pyadalight/__init__.py
+-rwxr-xr-x   0        0        0       66 2024-02-16 12:58:14.584969 pyadalight-1.0.0b3/pyadalight/__main__.py
+-rwxr-xr-x   0        0        0     6193 2024-05-28 11:12:53.998926 pyadalight-1.0.0b3/pyadalight/adalight.py
+-rwxr-xr-x   0        0        0     3415 2024-05-28 11:13:14.349899 pyadalight-1.0.0b3/pyadalight/main.py
+-rwxr-xr-x   0        0        0      239 2023-06-25 14:37:51.976258 pyadalight-1.0.0b3/pyadalight/singleton.py
+-rwxr-xr-x   0        0        0     1456 2023-06-25 15:26:30.580510 pyadalight-1.0.0b3/pyadalight/utils.py
+-rwxr-xr-x   0        0        0     1037 2024-05-28 11:13:59.084514 pyadalight-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 pyadalight-1.0.0b3/PKG-INFO
```

### Comparing `pyadalight-1.0.0b1/LICENSE` & `pyadalight-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyadalight-1.0.0b1/PKG-INFO` & `pyadalight-1.0.0b3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 Metadata-Version: 2.1
 Name: pyadalight
-Version: 1.0.0b1
+Version: 1.0.0b3
 Summary: Simple adalight (ambient light) software written in python.
-Home-page: https://github.com/pyAdaLight/pyadalight
 Author: RuslanUC
-License: MIT
+Author-email: dev_ruslan_uc@protonmail.com
+Requires-Python: >=3.9,<4.0
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=3.9
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: mss (>=9.0.1,<10.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
+Requires-Dist: pyserial (>=3.5,<4.0)
+Project-URL: Homepage, https://github.com/pyAdaLight/pyadalight
+Project-URL: Repository, https://github.com/pyAdaLight/pyadalight
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # pyAdalight
 
 ### Installation
 ```shell
 $ pip install pyadalight
 ```
@@ -38,7 +44,8 @@
   --list-ports                Shows ports list and exits.
   --help                      Show this message and exit.
 
 ```
 
 ### License
 The source is released under MIT-License (see https://opensource.org/licenses/MIT).
+
```

### Comparing `pyadalight-1.0.0b1/README.md` & `pyadalight-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `pyadalight-1.0.0b1/pyadalight/adalight.py` & `pyadalight-1.0.0b3/pyadalight/adalight.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,69 +53,72 @@
             del self._threads[threadId]
 
     @property
     def monitors(self) -> list[dict]:
         return self._get().monitors
 
     def getImage(self, monitor: dict) -> np.array:
-        return np.array(self._get().grab(monitor))
+        return np.array(self._get().grab(monitor))[:, :, :3]
 
 
 class Adalight(metaclass=Singleton):
     def __init__(self, h_led_count: int=None, v_led_count: int=None, port: str=None, monitor: dict=None):
         self._h_led_count = h_led_count
         self._v_led_count = v_led_count
         self._port = port
         self._monitor = monitor
         self._ser = None
         self._brightness = 1
         self._running = False
         self._thread = None
 
+        self._zones = [None] * self.led_count
+
     @property
     def led_count(self) -> int:
         return self._h_led_count * 2 + self._v_led_count * 2
 
     def _adjustBrightness(self, img: np.array) -> np.array:
         return cv2.convertScaleAbs(img, beta=32*self._brightness)
 
     def getZonesColors(self, image: np.array) -> np.array:
-        image = self._adjustBrightness(image)
         assert self._h_led_count is not None, "Horizontal led count is not set!"
         assert self._v_led_count is not None, "Vertical led count is not set!"
         assert self._monitor is not None, "Monitor is not set!"
         hlc = self._h_led_count
         vlc = self._v_led_count
         mon = self._monitor
 
-        zones = [None] * self.led_count
+        img_w, img_h = image.shape[:2]
+
+        hw = (img_w - 100) // hlc
+        vh = (img_h - 50) // vlc
+        hh = img_w // 20
+        vw = img_h // 10
 
-        hw = (mon["width"] - 100) // hlc
-        hh = 100
-        vw = 100
-        vh = (mon["height"] - 50) // vlc
+        im: np.ndarray
         for i in range(self.led_count):  # Right to left direction
-            if i in range(hlc):
-                _i = i
-                im = image[mon["height"] - hh:mon["height"], mon["width"] - 50 - hw - hw * _i:mon["width"] - 50 - hw * _i]  # 50 is corner offset
-            elif i in range(hlc, hlc + vlc):
+            if i < hlc:
+                im = image[mon["height"] - hh:mon["height"], mon["width"] - 50 - hw - hw * i:mon["width"] - 50 - hw * i]  # 50 is corner offset
+            elif i < hlc + vlc:
                 _i = i - hlc
                 im = image[mon["height"] - 25 - vh - vh * _i:mon["height"] - 25 - vh * _i, 0:vw]  # 25 is corner offset
-            elif i in range(hlc + vlc, hlc * 2 + vlc):
+            elif i < hlc * 2 + vlc:
                 _i = i - hlc - vlc
                 im = image[0:hh, 50 + hw * _i:50 + hw + hw * _i]  # 50 is corner offset
-            elif i in range(hlc * 2 + vlc, hlc * 2 + vlc * 2):
+            elif i < hlc * 2 + vlc * 2:
                 _i = i - hlc * 2 - vlc
                 im = image[25 + vh * _i:25 + vh + vh * _i, mon["width"] - vw:mon["width"]]  # 25 is corner offset
             else:
-                assert False, "This error must never happen"
+                assert False, "Unreachable"
 
-            zones[i] = np.mean(im, axis=(0, 1)).astype(np.uint8)[:3][::-1]
+            w, h = im.shape[:2]
+            self._zones[i] = self._adjustBrightness(np.divide(np.sum(im, axis=(0, 1)), w*h))
 
-        return zones
+        return self._zones
 
     def connect(self) -> None:
         if isinstance(self._ser, Serial) and self._ser.is_open:
             self._ser.close()
 
         assert self._port is not None, "Port is not set!"
 
@@ -138,15 +141,15 @@
     def _run(self) -> None:
         self.connect()
         self._running = True
         while True:
             if not self._running: break
             img = Mss().getImage(self._monitor)
             self.writeImage(img)
-        self._running = False
+
         self.disconnect()
 
     def run(self) -> None:
         if self._thread is not None or self._running or (self._ser is not None and self._ser.is_open): return
         self._run()
 
     def stop(self) -> None:
```

### Comparing `pyadalight-1.0.0b1/pyadalight/main.py` & `pyadalight-1.0.0b3/pyadalight/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import serial.tools.list_ports
 
-from . import Mss, Adalight
+from pyadalight import Mss, Adalight
 from pathlib import Path
 from json import dump, load
 import click
 
 
 def load_config() -> dict:
     config_path = Path.home() / "pyadalight.json"
```

### Comparing `pyadalight-1.0.0b1/pyadalight/utils.py` & `pyadalight-1.0.0b3/pyadalight/utils.py`

 * *Files identical despite different names*

