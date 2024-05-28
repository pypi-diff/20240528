# Comparing `tmp/PID_Py-1.2.1.tar.gz` & `tmp/pid_py-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PID_Py-1.2.1.tar", last modified: Fri Aug  4 16:50:49 2023, max compression
+gzip compressed data, was "pid_py-1.2.2.tar", last modified: Mon May 27 23:49:50 2024, max compression
```

## Comparing `PID_Py-1.2.1.tar` & `pid_py-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:50:49.187931 PID_Py-1.2.1/
--rw-rw-rw-   0        0        0     1090 2023-08-04 16:45:54.000000 PID_Py-1.2.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-08-04 16:50:49.162435 PID_Py-1.2.1/PID_Py/
--rw-rw-rw-   0        0        0    31010 2023-08-04 16:46:50.000000 PID_Py-1.2.1/PID_Py/PID.py
--rw-rw-rw-   0        0        0    50006 2023-08-04 16:45:54.000000 PID_Py-1.2.1/PID_Py/SetupTool.py
--rw-rw-rw-   0        0        0      695 2023-08-04 16:45:54.000000 PID_Py-1.2.1/PID_Py/Simulation.py
--rw-rw-rw-   0        0        0      165 2023-08-04 16:45:54.000000 PID_Py-1.2.1/PID_Py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:50:49.177390 PID_Py-1.2.1/PID_Py.egg-info/
--rw-rw-rw-   0        0        0    19690 2023-08-04 16:50:49.000000 PID_Py-1.2.1/PID_Py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-08-04 16:50:49.000000 PID_Py-1.2.1/PID_Py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:50:49.000000 PID_Py-1.2.1/PID_Py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-04 16:50:49.000000 PID_Py-1.2.1/PID_Py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    19690 2023-08-04 16:50:49.178382 PID_Py-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    17446 2023-08-04 16:45:54.000000 PID_Py-1.2.1/README.md
--rw-rw-rw-   0        0        0     1154 2023-08-04 16:48:22.000000 PID_Py-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-04 16:50:49.187931 PID_Py-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 23:49:50.489221 pid_py-1.2.2/
+-rw-rw-rw-   0        0        0     1090 2023-08-04 16:45:54.000000 pid_py-1.2.2/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-27 23:49:50.445138 pid_py-1.2.2/PID_Py/
+-rw-rw-rw-   0        0        0    30962 2024-05-27 23:28:50.000000 pid_py-1.2.2/PID_Py/PID.py
+-rw-rw-rw-   0        0        0    50006 2023-08-04 16:45:54.000000 pid_py-1.2.2/PID_Py/SetupTool.py
+-rw-rw-rw-   0        0        0      695 2023-08-04 16:45:54.000000 pid_py-1.2.2/PID_Py/Simulation.py
+-rw-rw-rw-   0        0        0      165 2023-08-04 16:45:54.000000 pid_py-1.2.2/PID_Py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:49:50.484670 pid_py-1.2.2/PID_Py.egg-info/
+-rw-rw-rw-   0        0        0    19690 2024-05-27 23:49:50.000000 pid_py-1.2.2/PID_Py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-05-27 23:49:50.000000 pid_py-1.2.2/PID_Py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 23:49:50.000000 pid_py-1.2.2/PID_Py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-27 23:49:50.000000 pid_py-1.2.2/PID_Py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    19690 2024-05-27 23:49:50.486673 pid_py-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    17446 2023-08-04 16:45:54.000000 pid_py-1.2.2/README.md
+-rw-rw-rw-   0        0        0     1154 2024-05-27 23:47:30.000000 pid_py-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 23:49:50.489221 pid_py-1.2.2/setup.cfg
```

### Comparing `PID_Py-1.2.1/LICENSE` & `pid_py-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PID_Py-1.2.1/PID_Py/PID.py` & `pid_py-1.2.2/PID_Py/PID.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,57 +476,57 @@
 
             # ===== Historian =====
             if self.historian is not None:
                 if HistorianParams.P in self.historianParams:
                     self.historian["P"].append(self._p)
                     
                     if len(self.historian["P"]) > self.historianLenght:
-                        del self.historianLenght["P"][0]
+                        del self.historian["P"][0]
                 
                 if HistorianParams.I in self.historianParams:
                     self.historian["I"].append(self._i)
                     
                     if len(self.historian["I"]) > self.historianLenght:
-                        del self.historianLenght["I"][0]
+                        del self.historian["I"][0]
 
                 if HistorianParams.D in self.historianParams:
                     self.historian["D"].append(self._d)
                     
                     if len(self.historian["D"]) > self.historianLenght:
-                        del self.historianLenght["D"][0]
+                        del self.historian["D"][0]
                 
                 if HistorianParams.OUTPUT in self.historianParams:
                     self.historian["OUTPUT"].append(self.output)
                     
                     if len(self.historian["OUTPUT"]) > self.historianLenght:
-                        del self.historianLenght["OUTPUT"][0]
+                        del self.historian["OUTPUT"][0]
                 
                 if HistorianParams.SETPOINT in self.historianParams:
                     self.historian["SETPOINT"].append(self._setpoint)
                     
                     if len(self.historian["SETPOINT"]) > self.historianLenght:
-                        del self.historianLenght["SETPOINT"][0]
+                        del self.historian["SETPOINT"][0]
                 
                 if HistorianParams.PROCESS_VALUE in self.historianParams:
                     self.historian["PROCESS_VALUE"].append(processValue)
                     
                     if len(self.historian["PROCESS_VALUE"]) > self.historianLenght:
-                        del self.historianLenght["PROCESS_VALUE"][0]
+                        del self.historian["PROCESS_VALUE"][0]
 
                 if HistorianParams.ERROR in self.historianParams:
                     self.historian["ERROR"].append(error)
                     
                     if len(self.historian["ERROR"]) > self.historianLenght:
-                        del self.historianLenght["ERROR"][0]
+                        del self.historian["ERROR"][0]
 
                 if (HistorianParams.P in self.historianParams) or (HistorianParams.I in self.historianParams) or (HistorianParams.D in self.historianParams) or (HistorianParams.ERROR in self.historianParams) or (HistorianParams.OUTPUT in self.historianParams) or (HistorianParams.PROCESS_VALUE in self.historianParams) or (HistorianParams.SETPOINT in self.historianParams):
                     self.historian["TIME"].append(actualTime - self._startTime)
                     
                     if len(self.historian["TIME"]) > self.historianLenght:
-                        del self.historianLenght["TIME"][0]
+                        del self.historian["TIME"][0]
             
             # ===== Saving data for next execution =====
             self._lastError = error
             self._lastTime = actualTime
             self._lastProcessValue = processValue
 
             # ===== Simulation =====
```

### Comparing `PID_Py-1.2.1/PID_Py/SetupTool.py` & `pid_py-1.2.2/PID_Py/SetupTool.py`

 * *Files identical despite different names*

### Comparing `PID_Py-1.2.1/PID_Py/Simulation.py` & `pid_py-1.2.2/PID_Py/Simulation.py`

 * *Files identical despite different names*

### Comparing `PID_Py-1.2.1/PID_Py.egg-info/PKG-INFO` & `pid_py-1.2.2/PID_Py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: PID-Py
-Version: 1.2.1
+Name: PID_Py
+Version: 1.2.2
 Summary: Simple (but complete) PID controller in Python
 Author-email: ThunderTecke <thunder.tecke@gmail.com>
 Maintainer-email: ThunderTecke <thunder.tecke@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 ThunderTecke
```

### Comparing `PID_Py-1.2.1/PKG-INFO` & `pid_py-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PID_Py
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simple (but complete) PID controller in Python
 Author-email: ThunderTecke <thunder.tecke@gmail.com>
 Maintainer-email: ThunderTecke <thunder.tecke@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 ThunderTecke
```

### Comparing `PID_Py-1.2.1/README.md` & `pid_py-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `PID_Py-1.2.1/pyproject.toml` & `pid_py-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["PID_Py"]
 
 [project]
 name = "PID_Py"
-version = "1.2.1"
+version = "1.2.2"
 authors = [{name = "ThunderTecke", email = "thunder.tecke@gmail.com"}]
 maintainers = [{name = "ThunderTecke", email = "thunder.tecke@gmail.com"}]
 keywords = ["pid", "controller", "pid-controller", "control", "pid-control", "python", "raspberry", "raspberrypi", "raspberry-pi"]
 description = "Simple (but complete) PID controller in Python"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

