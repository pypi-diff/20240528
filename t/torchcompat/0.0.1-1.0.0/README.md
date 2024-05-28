# Comparing `tmp/torchcompat-0.0.1.tar.gz` & `tmp/torchcompat-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchcompat-0.0.1.tar", last modified: Tue May  7 15:00:15 2024, max compression
+gzip compressed data, was "torchcompat-1.0.0.tar", last modified: Tue May 28 12:54:37 2024, max compression
```

## Comparing `torchcompat-0.0.1.tar` & `torchcompat-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:15.178713 torchcompat-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-07 14:59:58.000000 torchcompat-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-07 14:59:58.000000 torchcompat-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-07 15:00:15.178713 torchcompat-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-07 14:59:58.000000 torchcompat-0.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 14:59:58.000000 torchcompat-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:00:15.178713 torchcompat-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-07 14:59:58.000000 torchcompat-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:15.178713 torchcompat-0.0.1/torchcompat/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 14:59:58.000000 torchcompat-0.0.1/torchcompat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:15.178713 torchcompat-0.0.1/torchcompat/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-07 14:59:58.000000 torchcompat-0.0.1/torchcompat/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 14:59:58.000000 torchcompat-0.0.1/torchcompat/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-07 14:59:58.000000 torchcompat-0.0.1/torchcompat/core/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:15.178713 torchcompat-0.0.1/torchcompat/data/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-07 14:59:58.000000 torchcompat-0.0.1/torchcompat/data/data.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:15.178713 torchcompat-0.0.1/torchcompat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-07 15:00:15.000000 torchcompat-0.0.1/torchcompat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-07 15:00:15.000000 torchcompat-0.0.1/torchcompat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:00:15.000000 torchcompat-0.0.1/torchcompat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 15:00:15.000000 torchcompat-0.0.1/torchcompat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 15:00:15.000000 torchcompat-0.0.1/torchcompat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:37.511315 torchcompat-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-28 12:53:05.000000 torchcompat-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 12:53:05.000000 torchcompat-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-28 12:54:37.511315 torchcompat-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-28 12:53:05.000000 torchcompat-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 12:53:05.000000 torchcompat-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:54:37.511315 torchcompat-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-28 12:53:05.000000 torchcompat-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:37.507315 torchcompat-1.0.0/torchcompat/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 12:53:05.000000 torchcompat-1.0.0/torchcompat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:37.511315 torchcompat-1.0.0/torchcompat/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-28 12:53:05.000000 torchcompat-1.0.0/torchcompat/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 12:53:05.000000 torchcompat-1.0.0/torchcompat/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-28 12:53:05.000000 torchcompat-1.0.0/torchcompat/core/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:37.511315 torchcompat-1.0.0/torchcompat/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-28 12:53:05.000000 torchcompat-1.0.0/torchcompat/data/data.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:37.511315 torchcompat-1.0.0/torchcompat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-28 12:54:37.000000 torchcompat-1.0.0/torchcompat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 12:54:37.000000 torchcompat-1.0.0/torchcompat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:54:37.000000 torchcompat-1.0.0/torchcompat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-28 12:54:37.000000 torchcompat-1.0.0/torchcompat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 12:54:37.000000 torchcompat-1.0.0/torchcompat.egg-info/top_level.txt
```

### Comparing `torchcompat-0.0.1/LICENSE` & `torchcompat-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchcompat-0.0.1/PKG-INFO` & `torchcompat-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: torchcompat
-Version: 0.0.1
+Version: 1.0.0
 Summary: torch compatibility layer
 Home-page: https://torchcompat.readthedocs.io
 Author: Anonymous
 Author-email: anony@mous.com
 License: BSD 3-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 Requires-Dist: importlib_resources
+Requires-Dist: torch
 Provides-Extra: plugins
 Requires-Dist: importlib_resources; extra == "plugins"
 Provides-Extra: all
 Requires-Dist: importlib_resources; extra == "all"
 
 torchcompat
 =============================
@@ -48,15 +49,15 @@
 
    pip install torchcompat
 
 
 Features
 --------
 
-* Provide a super set implementation of pytorch device interface 
+* Provide a super set implementation of pytorch device interface
   to enable code to run seamlessly between different accelerators.
 * Identify uniquely devices
 
 
 .. code-block:: python
 
    import torchcompat.core as accelerator
@@ -64,16 +65,16 @@
    # on  cuda accelerator == torch.cuda
    # on  rocm accelerator == torch.cuda
    # on   xpu accelerator == torch.xpu
    # on gaudi accelerator == ...
 
    assert accelerator.is_available() == true
    assert accelerator.device_name in ('xpu', 'cuda', "hpu")           # rocm is seen as cuda by pytorch
-   assert accelerator.device_string(0) == "cuda:0" or "xpu:0" or "hpu:0" 
-   assert accelerator.fetch_device(0) == torch.device("cuda:0") 
+   assert accelerator.device_string(0) == "cuda:0" or "xpu:0" or "hpu:0"
+   assert accelerator.fetch_device(0) == torch.device("cuda:0")
 
 
    accelerator.set_enable_tf32(true) # toggle the right flags for each backend
 
 
 Example
 -------
```

### Comparing `torchcompat-0.0.1/README.rst` & `torchcompat-1.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
    pip install torchcompat
 
 
 Features
 --------
 
-* Provide a super set implementation of pytorch device interface 
+* Provide a super set implementation of pytorch device interface
   to enable code to run seamlessly between different accelerators.
 * Identify uniquely devices
 
 
 .. code-block:: python
 
    import torchcompat.core as accelerator
@@ -44,16 +44,16 @@
    # on  cuda accelerator == torch.cuda
    # on  rocm accelerator == torch.cuda
    # on   xpu accelerator == torch.xpu
    # on gaudi accelerator == ...
 
    assert accelerator.is_available() == true
    assert accelerator.device_name in ('xpu', 'cuda', "hpu")           # rocm is seen as cuda by pytorch
-   assert accelerator.device_string(0) == "cuda:0" or "xpu:0" or "hpu:0" 
-   assert accelerator.fetch_device(0) == torch.device("cuda:0") 
+   assert accelerator.device_string(0) == "cuda:0" or "xpu:0" or "hpu:0"
+   assert accelerator.fetch_device(0) == torch.device("cuda:0")
 
 
    accelerator.set_enable_tf32(true) # toggle the right flags for each backend
 
 
 Example
 -------
```

### Comparing `torchcompat-0.0.1/setup.py` & `torchcompat-1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,17 @@
         packages=[
             "torchcompat.core",
             "torchcompat.plugins.cuda",
             "torchcompat.plugins.rocm",
             "torchcompat.plugins.xpu",
         ],
         setup_requires=["setuptools"],
-        install_requires=["importlib_resources"],
+        install_requires=[
+            "importlib_resources",
+            "torch",
+        ],
         package_data={
             "torchcompat.data": [
                 "torchcompat/data",
             ],
         },
     )
```

### Comparing `torchcompat-0.0.1/torchcompat/core/__init__.py` & `torchcompat-1.0.0/torchcompat/core/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,92 @@
 """Top level module for torchcompat"""
 
-
 __descr__ = "torch compatibility layer"
-__version__ = "0.0.1"
+__version__ = "1.0.0"
 __license__ = "BSD 3-Clause License"
 __author__ = "Anonymous"
 __author_email__ = "anony@mous.com"
 __copyright__ = "2024 Anonymous"
 __url__ = "https://github.com/Delaunay/torchcompat"
 
 
 import sys
 
-from torchcompat.core.load import load_device
-
 import torch
 
+from torchcompat.core.load import load_device
+
 device_module = load_device()
 
 
 #
 # Helpers
 #
 def device_string(id: int):
-    return f"{device_module.device_name}:{id}"
+    return f"{device_module.device_type}:{id}"
+
+
+def mark_step():
+    pass
 
 
 def fetch_device(id: int):
     return torch.device(device_string(id))
 
 
 def init_process_group(*args, backend=None, rank=-1, world_size=-1, **kwargs):
     backend = backend or device_module.ccl
-    torch.distributed.init_process_group(*args, backend=backend, rank=rank, world_size=world_size, **kwargs)
+    torch.distributed.init_process_group(
+        *args, backend=backend, rank=rank, world_size=world_size, **kwargs
+    )
 
 
 def destroy_process_group():
     torch.distributed.destroy_process_group()
 
+
 #
-# Default noops that gets overriden if they exist
+# Default noops that gets overridden if they exist
 #
 
+
 # Not all device support tf32
 def set_enable_tf32(enable=True):
     pass
 
+
 #
 # XPU has a special optimizer
 #
-def optimizer(model, *args, optimizer=None, dtype=None, **kwargs):
+def optimize(model, *args, optimizer=None, dtype=None, **kwargs):
     if dtype is not None:
         # model.to(dtype=dtype) ?
         pass
 
     if optimizer is None:
         return model
     else:
         return model, optimizer
 
 
+def empty_cache():
+    pass
+
+
+def synchronize():
+    pass
+
+
 #
 # This actually cannot really trigger because  load_device would raise NoDeviceDetected
 # so this does not make it possible to fallback on CPU
 def is_available():
     return True
 
+
 #
 # Add device interface to current module
 #   overriding the default implementation when available
 #
 self = current_module = sys.modules[__name__]
 for k, v in vars(device_module).items():
     setattr(self, k, v)
```

### Comparing `torchcompat-0.0.1/torchcompat/core/load.py` & `torchcompat-1.0.0/torchcompat/core/load.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """Top level module for torchcompat"""
 
 import importlib
 import pkgutil
-from functools import cache
+from functools import lru_cache
 
 from torchcompat.core.errors import NotAvailable
 
-
 missing_backend_reason = {}
 default_device = None
 
+
 class NoDeviceDetected(Exception):
     pass
 
 
 def explain_errors():
     global missing_backend_reason
 
     frags = []
     for k, v in missing_backend_reason.items():
         message = [str(v)]
         if v.__cause__:
-            message.append(f"because")
+            message.append("because")
             message.append(str(v.__cause__))
         error = " ".join(message)
 
         frags.append(f"{k}: {error}")
 
     sep = "\n    - "
     errors = sep.join(frags)
@@ -41,19 +41,19 @@
     path = module.__path__
     name = module.__name__
 
     plugins = {}
     errors = {}
 
     for _, name, _ in pkgutil.iter_modules(path, name + "."):
-        
+
         try:
             backend = importlib.import_module(name)
 
-            if 'cpu' in name:
+            if "cpu" in name:
                 default_device = backend
 
             plugins[name] = backend
         except NotAvailable as err:
             errors[name] = err
 
     missing_backend_reason = errors
@@ -65,47 +65,47 @@
     import torchcompat.plugins
 
     devices = discover_plugins(torchcompat.plugins)
 
     return devices
 
 
-@cache
+@lru_cache
 def load_device(ensure=None):
     """Load a compute device, CPU is not valid.
-    
+
     Arguments
     ---------
     ensure: optional, str
         name of the expected backend (xpu, cuda, hpu, rocm)
         if the backend do not match raise
-    
+
     """
     devices = load_plugins()
 
     if len(devices) == 0:
         explain_errors()
-        
+
     impl = devices.popitem()[1].impl
     if ensure is not None:
         assert impl.device_type == ensure
 
     return impl
 
 
-@cache
+@lru_cache
 def load_available(ensure=None):
     """Load the fastest available compute device, fallsback to CPU
-    
+
     Arguments
     ---------
     ensure: optional, str
         name of the expected backend (xpu, cuda, hpu, rocm)
         if the backend do not match raise
-    
+
     """
     devices = load_plugins()
     impl = default_device.impl
 
     if len(devices) > 0:
         impl = devices.popitem()[1].impl
```

### Comparing `torchcompat-0.0.1/torchcompat.egg-info/PKG-INFO` & `torchcompat-1.0.0/torchcompat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: torchcompat
-Version: 0.0.1
+Version: 1.0.0
 Summary: torch compatibility layer
 Home-page: https://torchcompat.readthedocs.io
 Author: Anonymous
 Author-email: anony@mous.com
 License: BSD 3-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 Requires-Dist: importlib_resources
+Requires-Dist: torch
 Provides-Extra: plugins
 Requires-Dist: importlib_resources; extra == "plugins"
 Provides-Extra: all
 Requires-Dist: importlib_resources; extra == "all"
 
 torchcompat
 =============================
@@ -48,15 +49,15 @@
 
    pip install torchcompat
 
 
 Features
 --------
 
-* Provide a super set implementation of pytorch device interface 
+* Provide a super set implementation of pytorch device interface
   to enable code to run seamlessly between different accelerators.
 * Identify uniquely devices
 
 
 .. code-block:: python
 
    import torchcompat.core as accelerator
@@ -64,16 +65,16 @@
    # on  cuda accelerator == torch.cuda
    # on  rocm accelerator == torch.cuda
    # on   xpu accelerator == torch.xpu
    # on gaudi accelerator == ...
 
    assert accelerator.is_available() == true
    assert accelerator.device_name in ('xpu', 'cuda', "hpu")           # rocm is seen as cuda by pytorch
-   assert accelerator.device_string(0) == "cuda:0" or "xpu:0" or "hpu:0" 
-   assert accelerator.fetch_device(0) == torch.device("cuda:0") 
+   assert accelerator.device_string(0) == "cuda:0" or "xpu:0" or "hpu:0"
+   assert accelerator.fetch_device(0) == torch.device("cuda:0")
 
 
    accelerator.set_enable_tf32(true) # toggle the right flags for each backend
 
 
 Example
 -------
```

