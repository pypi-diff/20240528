# Comparing `tmp/innova-controls-2.2.1.tar.gz` & `tmp/innova_controls-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innova-controls-2.2.1.tar", last modified: Thu Feb 22 03:29:36 2024, max compression
+gzip compressed data, was "innova_controls-2.2.2.tar", last modified: Tue May 28 03:14:59 2024, max compression
```

## Comparing `innova-controls-2.2.1.tar` & `innova_controls-2.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 danielrivard  (1001) danielrivard  (1001)        0 2024-02-22 03:29:36.029972 innova-controls-2.2.1/
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)    11357 2024-02-22 03:11:30.000000 innova-controls-2.2.1/LICENSE
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     6751 2024-02-22 03:29:36.029972 innova-controls-2.2.1/PKG-INFO
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     5922 2024-02-22 03:11:30.000000 innova-controls-2.2.1/README.md
-drwxrwxr-x   0 danielrivard  (1001) danielrivard  (1001)        0 2024-02-22 03:29:36.029972 innova-controls-2.2.1/innova_controls/
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     5326 2024-02-22 03:11:30.000000 innova-controls-2.2.1/innova_controls/airleaf.py
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)      533 2024-02-22 03:11:30.000000 innova-controls-2.2.1/innova_controls/constants.py
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)      144 2024-02-22 03:11:30.000000 innova-controls-2.2.1/innova_controls/fan_speed.py
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     8357 2024-02-22 03:11:30.000000 innova-controls-2.2.1/innova_controls/innova.py
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     6263 2024-02-22 03:11:30.000000 innova-controls-2.2.1/innova_controls/innova_device.py
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)      777 2024-02-22 03:11:30.000000 innova-controls-2.2.1/innova_controls/innova_factory.py
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     1121 2024-02-22 03:11:30.000000 innova-controls-2.2.1/innova_controls/mode.py
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     2517 2024-02-22 03:11:30.000000 innova-controls-2.2.1/innova_controls/network_functions.py
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     4684 2024-02-22 03:11:30.000000 innova-controls-2.2.1/innova_controls/twopointzero.py
-drwxrwxr-x   0 danielrivard  (1001) danielrivard  (1001)        0 2024-02-22 03:29:36.029972 innova-controls-2.2.1/innova_controls.egg-info/
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     6751 2024-02-22 03:29:36.000000 innova-controls-2.2.1/innova_controls.egg-info/PKG-INFO
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)      501 2024-02-22 03:29:36.000000 innova-controls-2.2.1/innova_controls.egg-info/SOURCES.txt
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)        1 2024-02-22 03:29:36.000000 innova-controls-2.2.1/innova_controls.egg-info/dependency_links.txt
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)       36 2024-02-22 03:29:36.000000 innova-controls-2.2.1/innova_controls.egg-info/requires.txt
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)       16 2024-02-22 03:29:36.000000 innova-controls-2.2.1/innova_controls.egg-info/top_level.txt
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)       74 2024-02-22 03:29:36.029972 innova-controls-2.2.1/setup.cfg
--rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     1549 2024-02-22 03:14:34.000000 innova-controls-2.2.1/setup.py
+drwxrwxr-x   0 danielrivard  (1001) danielrivard  (1001)        0 2024-05-28 03:14:59.482854 innova_controls-2.2.2/
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)    11357 2024-02-22 03:11:30.000000 innova_controls-2.2.2/LICENSE
+-rw-r--r--   0 danielrivard  (1001) danielrivard  (1001)     6817 2024-05-28 03:14:59.482854 innova_controls-2.2.2/PKG-INFO
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     5922 2024-02-22 03:11:30.000000 innova_controls-2.2.2/README.md
+drwxrwxr-x   0 danielrivard  (1001) danielrivard  (1001)        0 2024-05-28 03:14:59.482854 innova_controls-2.2.2/innova_controls/
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     5259 2024-05-28 03:08:04.000000 innova_controls-2.2.2/innova_controls/airleaf.py
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)      533 2024-02-22 03:11:30.000000 innova_controls-2.2.2/innova_controls/constants.py
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)      105 2024-05-28 03:08:04.000000 innova_controls-2.2.2/innova_controls/fan_speed.py
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     8372 2024-05-28 03:08:04.000000 innova_controls-2.2.2/innova_controls/innova.py
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     6331 2024-05-28 03:08:04.000000 innova_controls-2.2.2/innova_controls/innova_device.py
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)      777 2024-02-22 03:11:30.000000 innova_controls-2.2.2/innova_controls/innova_factory.py
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     1121 2024-02-22 03:11:30.000000 innova_controls-2.2.2/innova_controls/mode.py
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     2517 2024-02-22 03:11:30.000000 innova_controls-2.2.2/innova_controls/network_functions.py
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     5173 2024-05-28 03:08:04.000000 innova_controls-2.2.2/innova_controls/twopointzero.py
+drwxrwxr-x   0 danielrivard  (1001) danielrivard  (1001)        0 2024-05-28 03:14:59.482854 innova_controls-2.2.2/innova_controls.egg-info/
+-rw-r--r--   0 danielrivard  (1001) danielrivard  (1001)     6817 2024-05-28 03:14:59.000000 innova_controls-2.2.2/innova_controls.egg-info/PKG-INFO
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)      501 2024-05-28 03:14:59.000000 innova_controls-2.2.2/innova_controls.egg-info/SOURCES.txt
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)        1 2024-05-28 03:14:59.000000 innova_controls-2.2.2/innova_controls.egg-info/dependency_links.txt
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)       36 2024-05-28 03:14:59.000000 innova_controls-2.2.2/innova_controls.egg-info/requires.txt
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)       16 2024-05-28 03:14:59.000000 innova_controls-2.2.2/innova_controls.egg-info/top_level.txt
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)       74 2024-05-28 03:14:59.482854 innova_controls-2.2.2/setup.cfg
+-rw-rw-r--   0 danielrivard  (1001) danielrivard  (1001)     1549 2024-05-28 03:08:04.000000 innova_controls-2.2.2/setup.py
```

### Comparing `innova-controls-2.2.1/LICENSE` & `innova_controls-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `innova-controls-2.2.1/PKG-INFO` & `innova_controls-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: innova-controls
-Version: 2.2.1
+Version: 2.2.2
 Summary: Innova Air Conditioner Control API
 Home-page: https://github.com/danielrivard/innova-controls
 Author: Daniel Rivard
 License: Apache
 Project-URL: Bug Reports, https://github.com/danielrivard/innova-controls/issues
 Project-URL: Source, https://github.com/danielrivard/innova-controls/
 Keywords: development,home automation,library,innova
@@ -14,14 +14,16 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp<4.0.0,>=3.0.0
+Requires-Dist: retry2>=0.9.5
 
 [![PyPI version](https://badge.fury.io/py/innova-controls.svg)](https://badge.fury.io/py/innova-controls)
 
 # Innova Control API
 
 Tested on a [Innova 2.0 unit](https://www.innovaenergie.com/en/products/air-conditioning-without-outdoor-unit/2.0-verticale/2.0/)
```

### Comparing `innova-controls-2.2.1/README.md` & `innova_controls-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `innova-controls-2.2.1/innova_controls/airleaf.py` & `innova_controls-2.2.2/innova_controls/airleaf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from collections.abc import Iterable
 from enum import Enum
-from typing import List
 
 from innova_controls.constants import CMD_LOCK_OFF, CMD_LOCK_ON, CMD_SET_TEMP
 from innova_controls.fan_speed import FanSpeed
 from innova_controls.innova_device import InnovaDevice
 from innova_controls.mode import Mode
 from innova_controls.network_functions import NetWorkFunctions
 
@@ -81,20 +81,19 @@
             # so, let fan be labeled as AUTO in this case.
             if fn == self.Function.NIGHT:
                 fn = FanSpeed.AUTO
             return fn["fan"]
         return FanSpeed.AUTO
 
     @property
-    def supported_fan_speeds(self) -> List[FanSpeed]:
-        speeds: List[FanSpeed] = []
-        for function in self.Function:
-            if "fan" in function.value and function.value["fan"] is not None:
-                speeds.append(function.value["fan"])
-        return speeds
+    def supported_fan_speeds(self) -> Iterable[FanSpeed]:
+        return [
+            function.value['fan'] for function in self.Function
+            if function.value.get('fan') is not None
+        ]
 
     @property
     def rotation(self) -> bool:
         return False
 
     @property
     def night_mode(self) -> bool:
```

### Comparing `innova-controls-2.2.1/innova_controls/constants.py` & `innova_controls-2.2.2/innova_controls/constants.py`

 * *Files identical despite different names*

### Comparing `innova-controls-2.2.1/innova_controls/innova.py` & `innova_controls-2.2.2/innova_controls/innova.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import List
+from collections.abc import Iterable
 
 from aiohttp import ClientSession
 
 from innova_controls.constants import UNKNOWN_MODE
 from innova_controls.fan_speed import FanSpeed
 from innova_controls.innova_device import InnovaDevice
 from innova_controls.innova_factory import InnovaFactory
@@ -106,17 +106,17 @@
     @property
     def mode(self) -> Mode:
         if self._innova_device:
             return self._innova_device.mode
         return UNKNOWN_MODE
 
     @property
-    def supported_modes(self) -> List[Mode]:
+    def supported_modes(self) -> Iterable[Mode]:
         if self._innova_device:
-            return list(self._innova_device.Modes.get_supported_modes())
+            return self._innova_device.Modes.get_supported_modes()
         return []
 
     @property
     def rotation(self) -> bool:
         if self._innova_device:
             return self._innova_device.rotation
         return False
@@ -124,15 +124,15 @@
     @property
     def fan_speed(self) -> FanSpeed:
         if self._innova_device:
             return self._innova_device.fan_speed
         return 0
 
     @property
-    def supported_fan_speeds(self) -> List[FanSpeed]:
+    def supported_fan_speeds(self) -> Iterable[FanSpeed]:
         if self._innova_device:
             return self._innova_device.supported_fan_speeds
         return []
 
     @property
     def night_mode(self) -> bool:
         if self._innova_device:
```

### Comparing `innova-controls-2.2.1/innova_controls/innova_device.py` & `innova_controls-2.2.2/innova_controls/innova_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 import logging
 from abc import ABC, abstractmethod
-from typing import List
+from collections.abc import Iterable
 
-from innova_controls.constants import (
-    CMD_CALENDAR_OFF,
-    CMD_CALENDAR_ON,
-    CMD_POWER_OFF,
-    CMD_POWER_ON,
-    MAX_TEMP,
-    MIN_TEMP,
-    UNKNOWN_MODE,
-)
+from innova_controls.constants import (CMD_CALENDAR_OFF, CMD_CALENDAR_ON,
+                                       CMD_POWER_OFF, CMD_POWER_ON, MAX_TEMP,
+                                       MIN_TEMP, UNKNOWN_MODE)
 from innova_controls.fan_speed import FanSpeed
 from innova_controls.mode import Mode
 from innova_controls.network_functions import NetWorkFunctions
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class InnovaDevice(ABC):
     class Modes(ABC):
         codes: dict = None
 
         @classmethod
-        def get_supported_modes(cls) -> List[Mode]:
+        def get_supported_modes(cls) -> Iterable[Mode]:
             return cls.codes.values()
 
         @classmethod
         def get_mode(cls, code: int) -> Mode:
             if code in cls.codes:
                 return cls.codes[code]
             else:
@@ -71,15 +65,15 @@
     @property
     @abstractmethod
     def fan_speed(self) -> FanSpeed:
         pass
 
     @property
     @abstractmethod
-    def supported_fan_speeds(self) -> List[FanSpeed]:
+    def supported_fan_speeds(self) -> Iterable[FanSpeed]:
         pass
 
     @property
     @abstractmethod
     def rotation(self) -> bool:
         pass
```

### Comparing `innova-controls-2.2.1/innova_controls/innova_factory.py` & `innova_controls-2.2.2/innova_controls/innova_factory.py`

 * *Files identical despite different names*

### Comparing `innova-controls-2.2.1/innova_controls/mode.py` & `innova_controls-2.2.2/innova_controls/mode.py`

 * *Files identical despite different names*

### Comparing `innova-controls-2.2.1/innova_controls/network_functions.py` & `innova_controls-2.2.2/innova_controls/network_functions.py`

 * *Files identical despite different names*

### Comparing `innova-controls-2.2.1/innova_controls/twopointzero.py` & `innova_controls-2.2.2/innova_controls/twopointzero.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-from typing import List
+from collections.abc import Iterable
 
-from innova_controls.constants import (
-    CMD_FAN_SPEED,
-    CMD_NIGHT_MODE,
-    CMD_ROTATION,
-    CMD_SET_TEMP,
-    NIGHT_MODE_OFF,
-    NIGHT_MODE_ON,
-    ROTATION_OFF,
-    ROTATION_ON,
-)
+from innova_controls.constants import (CMD_FAN_SPEED, CMD_NIGHT_MODE,
+                                       CMD_ROTATION, CMD_SET_TEMP,
+                                       NIGHT_MODE_OFF, NIGHT_MODE_ON,
+                                       ROTATION_OFF, ROTATION_ON)
 from innova_controls.fan_speed import FanSpeed
 from innova_controls.innova_device import InnovaDevice
 from innova_controls.mode import Mode
 from innova_controls.network_functions import NetWorkFunctions
 
 
 class TwoPointZero(InnovaDevice):
@@ -33,16 +27,22 @@
         }
 
     fan_speeds = {
         0: FanSpeed.AUTO,
         1: FanSpeed.LOW,
         2: FanSpeed.MEDIUM,
         3: FanSpeed.HIGH,
+        # Fan Speed 4 is a Boost mode, but it is not supported by the API.
+        # Only the remote and the LCD screen can set this speed.
+        # Therefore, I chose to default to report HIGH as the speed 
+        # since this value cannot be passed to set_fan_speed.
+        4: FanSpeed.HIGH,
     }
-    fan_speeds_reverse: dict = {v: k for k, v in fan_speeds.items()}
+    # Ignore speed 4 for reasons explained above
+    fan_speeds_reverse = {v: k for k, v in fan_speeds.items() if k != 4}
 
     def __init__(self, network_facade: NetWorkFunctions) -> None:
         super().__init__(network_facade)
 
     @property
     def model(self) -> str:
         return "TwoPointZero (2.0)"
@@ -72,16 +72,17 @@
     @property
     def fan_speed(self) -> FanSpeed:
         if "fs" in self._status:
             return self.fan_speeds[self._status["fs"]]
         return FanSpeed.AUTO
 
     @property
-    def supported_fan_speeds(self) -> List[FanSpeed]:
-        return list(self.fan_speeds.values())
+    def supported_fan_speeds(self) -> Iterable[FanSpeed]:
+        # Use a set to remove duplicates
+        return set(self.fan_speeds.values())
 
     @property
     def rotation(self) -> bool:
         if "fr" in self._status:
             if self._status["fr"] == ROTATION_ON:
                 return True
         return False
```

### Comparing `innova-controls-2.2.1/innova_controls.egg-info/PKG-INFO` & `innova_controls-2.2.2/innova_controls.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: innova-controls
-Version: 2.2.1
+Version: 2.2.2
 Summary: Innova Air Conditioner Control API
 Home-page: https://github.com/danielrivard/innova-controls
 Author: Daniel Rivard
 License: Apache
 Project-URL: Bug Reports, https://github.com/danielrivard/innova-controls/issues
 Project-URL: Source, https://github.com/danielrivard/innova-controls/
 Keywords: development,home automation,library,innova
@@ -14,14 +14,16 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp<4.0.0,>=3.0.0
+Requires-Dist: retry2>=0.9.5
 
 [![PyPI version](https://badge.fury.io/py/innova-controls.svg)](https://badge.fury.io/py/innova-controls)
 
 # Innova Control API
 
 Tested on a [Innova 2.0 unit](https://www.innovaenergie.com/en/products/air-conditioning-without-outdoor-unit/2.0-verticale/2.0/)
```

### Comparing `innova-controls-2.2.1/setup.py` & `innova_controls-2.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="innova-controls",
-    version="2.2.1",
+    version="2.2.2",
     description="Innova Air Conditioner Control API",
     license="Apache",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/danielrivard/innova-controls",
     author="Daniel Rivard",
     # author_email='author@example.com',
```

