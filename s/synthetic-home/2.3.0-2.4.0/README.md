# Comparing `tmp/synthetic_home-2.3.0.tar.gz` & `tmp/synthetic_home-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthetic_home-2.3.0.tar", last modified: Mon May 27 19:20:15 2024, max compression
+gzip compressed data, was "synthetic_home-2.4.0.tar", last modified: Mon May 27 21:53:15 2024, max compression
```

## Comparing `synthetic_home-2.3.0.tar` & `synthetic_home-2.4.0.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:15.047875 synthetic_home-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-27 19:20:15.047875 synthetic_home-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-27 19:20:15.047875 synthetic_home-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:15.039875 synthetic_home-2.3.0/synthetic_home/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:15.043875 synthetic_home-2.3.0/synthetic_home/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/door-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/fan-oscilating.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/garage-door.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/gate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/heat-pump.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/hvac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/light-dimmable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/light-rgbw.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/light.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/motion-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/smart-blinds.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/smart-lock.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/smart-plug.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/smart-speaker.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/switch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/temperature-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/todo-list.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/vacuum.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/water-valve.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/weather-service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/window-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/synthetic_home.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:15.047875 synthetic_home-2.3.0/synthetic_home.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-27 19:20:15.000000 synthetic_home-2.3.0/synthetic_home.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-27 19:20:15.000000 synthetic_home-2.3.0/synthetic_home.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:20:15.000000 synthetic_home-2.3.0/synthetic_home.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 19:20:15.000000 synthetic_home-2.3.0/synthetic_home.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 19:20:15.000000 synthetic_home-2.3.0/synthetic_home.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:15.047875 synthetic_home-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/tests/test_device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/tests/test_synthetic_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:53:15.241616 synthetic_home-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-27 21:53:15.241616 synthetic_home-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-27 21:53:15.241616 synthetic_home-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:53:15.233616 synthetic_home-2.4.0/synthetic_home/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:53:15.237616 synthetic_home-2.4.0/synthetic_home/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/door-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/exhaust-fan.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/fan-oscilating.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/garage-door.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/gate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/heat-pump.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/hvac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/light-dimmable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/light-rgbw.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/light.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/lock-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/motion-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/smart-blinds.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/smart-lock.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/smart-plug.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/smart-speaker.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/smart-sprinkler.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/smart-tv.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/switch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/temperature-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/todo-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/vacuum.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/water-valve.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/weather-service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/registry/window-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/synthetic_home/synthetic_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:53:15.241616 synthetic_home-2.4.0/synthetic_home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-27 21:53:15.000000 synthetic_home-2.4.0/synthetic_home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-27 21:53:15.000000 synthetic_home-2.4.0/synthetic_home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:53:15.000000 synthetic_home-2.4.0/synthetic_home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 21:53:15.000000 synthetic_home-2.4.0/synthetic_home.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 21:53:15.000000 synthetic_home-2.4.0/synthetic_home.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:53:15.241616 synthetic_home-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/tests/test_device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-27 21:53:11.000000 synthetic_home-2.4.0/tests/test_synthetic_home.py
```

### Comparing `synthetic_home-2.3.0/LICENSE` & `synthetic_home-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/PKG-INFO` & `synthetic_home-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetic_home
-Version: 2.3.0
+Version: 2.4.0
 Summary: Library for managing synthetic home device registry
 Home-page: https://github.com/allenporter/synthetic-home
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `synthetic_home-2.3.0/README.md` & `synthetic_home-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/pyproject.toml` & `synthetic_home-2.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/setup.cfg` & `synthetic_home-2.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = synthetic_home
-version = 2.3.0
+version = 2.4.0
 description = Library for managing synthetic home device registry
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/synthetic-home
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
```

### Comparing `synthetic_home-2.3.0/synthetic_home/device_types.py` & `synthetic_home-2.4.0/synthetic_home/device_types.py`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/README.md` & `synthetic_home-2.4.0/synthetic_home/registry/README.md`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/camera.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/camera.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/door-sensor.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/door-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/heat-pump.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/heat-pump.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/hvac.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/hvac.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/motion-sensor.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/motion-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/smart-blinds.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/smart-blinds.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/smart-lock.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/lock-sensor.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ---
-device_type: smart-lock
-desc: A smart lock device that can be remotely monitored.
+device_type: lock-sensor
+desc: A smart lock device that can be remotely monitored only, but does not support remote control.
 device_states:
   locked:
     binary_sensor.lock: false
     sensor.battery: 90
   unlocked:
     binary_sensor.lock: true
     sensor.battery: 90
```

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/smart-speaker.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/smart-speaker.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/temperature-sensor.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/temperature-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/vacuum.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/vacuum.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/water-valve.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/water-valve.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/weather-service.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/weather-service.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/registry/window-sensor.yaml` & `synthetic_home-2.4.0/synthetic_home/registry/window-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home/synthetic_home.py` & `synthetic_home-2.4.0/synthetic_home/synthetic_home.py`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.3.0/synthetic_home.egg-info/PKG-INFO` & `synthetic_home-2.4.0/synthetic_home.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetic_home
-Version: 2.3.0
+Version: 2.4.0
 Summary: Library for managing synthetic home device registry
 Home-page: https://github.com/allenporter/synthetic-home
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `synthetic_home-2.3.0/synthetic_home.egg-info/SOURCES.txt` & `synthetic_home-2.4.0/synthetic_home.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,28 +8,32 @@
 ./synthetic_home/exceptions.py
 ./synthetic_home/py.typed
 ./synthetic_home/synthetic_home.py
 ./synthetic_home/registry/README.md
 ./synthetic_home/registry/__init__.py
 ./synthetic_home/registry/camera.yaml
 ./synthetic_home/registry/door-sensor.yaml
+./synthetic_home/registry/exhaust-fan.yaml
 ./synthetic_home/registry/fan-oscilating.yaml
 ./synthetic_home/registry/garage-door.yaml
 ./synthetic_home/registry/gate.yaml
 ./synthetic_home/registry/heat-pump.yaml
 ./synthetic_home/registry/hvac.yaml
 ./synthetic_home/registry/light-dimmable.yaml
 ./synthetic_home/registry/light-rgbw.yaml
 ./synthetic_home/registry/light.yaml
+./synthetic_home/registry/lock-sensor.yaml
 ./synthetic_home/registry/motion-sensor.yaml
 ./synthetic_home/registry/sensor.yaml
 ./synthetic_home/registry/smart-blinds.yaml
 ./synthetic_home/registry/smart-lock.yaml
 ./synthetic_home/registry/smart-plug.yaml
 ./synthetic_home/registry/smart-speaker.yaml
+./synthetic_home/registry/smart-sprinkler.yaml
+./synthetic_home/registry/smart-tv.yaml
 ./synthetic_home/registry/switch.yaml
 ./synthetic_home/registry/temperature-sensor.yaml
 ./synthetic_home/registry/todo-list.yaml
 ./synthetic_home/registry/vacuum.yaml
 ./synthetic_home/registry/water-valve.yaml
 ./synthetic_home/registry/weather-service.yaml
 ./synthetic_home/registry/window-sensor.yaml
```

### Comparing `synthetic_home-2.3.0/tests/test_device_types.py` & `synthetic_home-2.4.0/tests/test_device_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,17 @@
         assert isinstance(device_type.device_states_dict, dict)
         assert device_type.entities, "Device must have at least one entity"
         for domain, entity_entries in device_type.entities.items():
             assert domain
             assert entity_entries, "Domain must have at least one entity entry"
             for entry in entity_entries:
                 assert entry.key
-                assert entry.attributes, f"Entity for device {name} has no attributes"
+                assert (
+                    entry.attributes is not None
+                ), f"Entity for device {name} has no attributes"
 
 
 def test_camera_device() -> None:
     """Test the camera entry in the device registry."""
 
     reg = device_types.load_device_type_registry()
     assert reg.device_types
```

### Comparing `synthetic_home-2.3.0/tests/test_synthetic_home.py` & `synthetic_home-2.4.0/tests/test_synthetic_home.py`

 * *Files identical despite different names*

