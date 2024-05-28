# Comparing `tmp/generic_scpi_driver-1.5.2.tar.gz` & `tmp/generic_scpi_driver-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic_scpi_driver-1.5.2.tar", max compression
+gzip compressed data, was "generic_scpi_driver-1.5.3.tar", max compression
```

## Comparing `generic_scpi_driver-1.5.2.tar` & `generic_scpi_driver-1.5.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2023-12-12 15:30:40.509432 generic_scpi_driver-1.5.2/LICENSE
--rw-r--r--   0        0        0     8058 2023-12-12 15:30:40.509432 generic_scpi_driver-1.5.2/README.rst
--rw-r--r--   0        0        0      473 2023-12-12 15:30:40.510432 generic_scpi_driver-1.5.2/generic_scpi_driver/__init__.py
--rw-r--r--   0        0        0    12579 2023-12-12 15:30:40.510432 generic_scpi_driver-1.5.2/generic_scpi_driver/driver.py
--rw-r--r--   0        0        0     2944 2023-12-12 15:30:40.510432 generic_scpi_driver-1.5.2/generic_scpi_driver/generic_aqctl.py
--rw-r--r--   0        0        0     1260 2023-12-12 15:30:40.510432 generic_scpi_driver-1.5.2/generic_scpi_driver/session.py
--rw-r--r--   0        0        0     5590 2023-12-12 15:30:40.510432 generic_scpi_driver-1.5.2/generic_scpi_driver/visa_session.py
--rw-r--r--   0        0        0      790 2023-12-12 15:30:40.510432 generic_scpi_driver-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     8838 1970-01-01 00:00:00.000000 generic_scpi_driver-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-28 15:30:19.730173 generic_scpi_driver-1.5.3/LICENSE
+-rw-r--r--   0        0        0     8058 2024-05-28 15:30:19.730173 generic_scpi_driver-1.5.3/README.rst
+-rw-r--r--   0        0        0      473 2024-05-28 15:30:19.731173 generic_scpi_driver-1.5.3/generic_scpi_driver/__init__.py
+-rw-r--r--   0        0        0    12580 2024-05-28 15:30:19.731173 generic_scpi_driver-1.5.3/generic_scpi_driver/driver.py
+-rw-r--r--   0        0        0     2944 2024-05-28 15:30:19.731173 generic_scpi_driver-1.5.3/generic_scpi_driver/generic_aqctl.py
+-rw-r--r--   0        0        0     1260 2024-05-28 15:30:19.731173 generic_scpi_driver-1.5.3/generic_scpi_driver/session.py
+-rw-r--r--   0        0        0     5590 2024-05-28 15:30:19.731173 generic_scpi_driver-1.5.3/generic_scpi_driver/visa_session.py
+-rw-r--r--   0        0        0      790 2024-05-28 15:30:19.732173 generic_scpi_driver-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     8838 1970-01-01 00:00:00.000000 generic_scpi_driver-1.5.3/PKG-INFO
```

### Comparing `generic_scpi_driver-1.5.2/LICENSE` & `generic_scpi_driver-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `generic_scpi_driver-1.5.2/README.rst` & `generic_scpi_driver-1.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `generic_scpi_driver-1.5.2/generic_scpi_driver/driver.py` & `generic_scpi_driver-1.5.3/generic_scpi_driver/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
     def close(self):
         """
         Close the connection to this device.
 
         After this method is called, no other methods will work and this object should be discarded.
         """
-        logger.info("Closing connection to device %s", self.dev_id)
+        logger.debug("Closing connection to device %s", self.dev_id)
         self.instr.close()
         del _locks[self.dev_id]
         del _sessions[self.dev_id]
 
     @property
     def instr(self) -> Session:
         """
```

### Comparing `generic_scpi_driver-1.5.2/generic_scpi_driver/generic_aqctl.py` & `generic_scpi_driver-1.5.3/generic_scpi_driver/generic_aqctl.py`

 * *Files identical despite different names*

### Comparing `generic_scpi_driver-1.5.2/generic_scpi_driver/session.py` & `generic_scpi_driver-1.5.3/generic_scpi_driver/session.py`

 * *Files identical despite different names*

### Comparing `generic_scpi_driver-1.5.2/generic_scpi_driver/visa_session.py` & `generic_scpi_driver-1.5.3/generic_scpi_driver/visa_session.py`

 * *Files identical despite different names*

### Comparing `generic_scpi_driver-1.5.2/pyproject.toml` & `generic_scpi_driver-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "generic-scpi-driver"
-version = "1.5.2"
+version = "1.5.3"
 description = "A generic template for creating python object-based drivers for SCPI hardware devices which communicate via VISA. Compatible with ARTIQ  installed with [artiq] modifier"
 authors = ["Charles Baynham <charles.baynham@gmail.com>"]
 readme = "README.rst"
 packages = [{include = "generic_scpi_driver"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
```

### Comparing `generic_scpi_driver-1.5.2/PKG-INFO` & `generic_scpi_driver-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generic-scpi-driver
-Version: 1.5.2
+Version: 1.5.3
 Summary: A generic template for creating python object-based drivers for SCPI hardware devices which communicate via VISA. Compatible with ARTIQ  installed with [artiq] modifier
 Author: Charles Baynham
 Author-email: charles.baynham@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

