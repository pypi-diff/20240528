# Comparing `tmp/xspex-0.0.3.tar.gz` & `tmp/xspex-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspex-0.0.3.tar", last modified: Thu Apr 25 14:47:04 2024, max compression
+gzip compressed data, was "xspex-0.0.4.tar", last modified: Tue May 28 14:44:03 2024, max compression
```

## Comparing `xspex-0.0.3.tar` & `xspex-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.941582 xspex-0.0.3/
--rw-r--r--   0 xuewc      (501) staff       (20)    35122 2024-04-15 15:37:48.000000 xspex-0.0.3/LICENSE
--rw-r--r--   0 xuewc      (501) staff       (20)      224 2024-04-16 19:52:26.000000 xspex-0.0.3/MANIFEST.in
--rw-r--r--   0 xuewc      (501) staff       (20)     1560 2024-04-25 14:47:04.941247 xspex-0.0.3/PKG-INFO
--rw-r--r--   0 xuewc      (501) staff       (20)      887 2024-04-18 18:21:14.000000 xspex-0.0.3/README.md
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.935204 xspex-0.0.3/helpers/
--rw-r--r--   0 xuewc      (501) staff       (20)        0 2024-04-15 15:37:48.000000 xspex-0.0.3/helpers/__init__.py
--rw-r--r--   0 xuewc      (501) staff       (20)     2104 2024-04-15 15:37:48.000000 xspex-0.0.3/helpers/identify_xspec.py
--rw-r--r--   0 xuewc      (501) staff       (20)      310 2024-04-15 15:37:48.000000 xspex-0.0.3/helpers/report_xspec_version.cxx
--rw-r--r--   0 xuewc      (501) staff       (20)    14197 2024-04-15 15:37:48.000000 xspex-0.0.3/helpers/template.py
--rw-r--r--   0 xuewc      (501) staff       (20)      155 2024-04-15 15:37:48.000000 xspex-0.0.3/pyproject.toml
--rw-r--r--   0 xuewc      (501) staff       (20)      787 2024-04-25 14:47:04.942344 xspex-0.0.3/setup.cfg
--rw-r--r--   0 xuewc      (501) staff       (20)     3288 2024-04-25 14:45:58.000000 xspex-0.0.3/setup.py
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.935555 xspex-0.0.3/src/
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.936088 xspex-0.0.3/src/include/
--rw-r--r--   0 xuewc      (501) staff       (20)    27131 2024-04-23 20:12:30.000000 xspex-0.0.3/src/include/xspex.hpp
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.936621 xspex-0.0.3/src/xspex/
--rw-r--r--   0 xuewc      (501) staff       (20)   338104 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex/__init__.py
--rw-r--r--   0 xuewc      (501) staff       (20)    10035 2024-04-23 19:41:04.000000 xspex-0.0.3/src/xspex/primitive.py
--rw-r--r--   0 xuewc      (501) staff       (20)    94741 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.cpp
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.940551 xspex-0.0.3/src/xspex.egg-info/
--rw-r--r--   0 xuewc      (501) staff       (20)     1560 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.egg-info/PKG-INFO
--rw-r--r--   0 xuewc      (501) staff       (20)      523 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.egg-info/SOURCES.txt
--rw-r--r--   0 xuewc      (501) staff       (20)        1 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.egg-info/dependency_links.txt
--rw-r--r--   0 xuewc      (501) staff       (20)        1 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.egg-info/not-zip-safe
--rw-r--r--   0 xuewc      (501) staff       (20)        6 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.egg-info/requires.txt
--rw-r--r--   0 xuewc      (501) staff       (20)        6 2024-04-25 14:47:04.000000 xspex-0.0.3/src/xspex.egg-info/top_level.txt
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.939348 xspex-0.0.3/template/
--rw-r--r--   0 xuewc      (501) staff       (20)     4726 2024-04-17 10:50:41.000000 xspex-0.0.3/template/__init__.py
--rw-r--r--   0 xuewc      (501) staff       (20)     7005 2024-04-16 18:49:11.000000 xspex-0.0.3/template/xspex.cpp
-drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-04-25 14:47:04.940024 xspex-0.0.3/tests/
--rw-r--r--   0 xuewc      (501) staff       (20)     6286 2024-04-18 18:10:32.000000 xspex-0.0.3/tests/test_basic.py
--rw-r--r--   0 xuewc      (501) staff       (20)     7538 2024-04-25 14:41:30.000000 xspex-0.0.3/tests/test_primitive.py
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-05-28 14:44:03.764258 xspex-0.0.4/
+-rw-r--r--   0 xuewc      (501) staff       (20)    35122 2024-04-15 15:37:48.000000 xspex-0.0.4/LICENSE
+-rw-r--r--   0 xuewc      (501) staff       (20)      224 2024-04-16 19:52:26.000000 xspex-0.0.4/MANIFEST.in
+-rw-r--r--   0 xuewc      (501) staff       (20)     1872 2024-05-28 14:44:03.764159 xspex-0.0.4/PKG-INFO
+-rw-r--r--   0 xuewc      (501) staff       (20)     1142 2024-05-28 14:22:35.000000 xspex-0.0.4/README.md
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-05-28 14:44:03.760040 xspex-0.0.4/helpers/
+-rw-r--r--   0 xuewc      (501) staff       (20)        0 2024-04-15 15:37:48.000000 xspex-0.0.4/helpers/__init__.py
+-rw-r--r--   0 xuewc      (501) staff       (20)     2104 2024-04-15 15:37:48.000000 xspex-0.0.4/helpers/identify_xspec.py
+-rw-r--r--   0 xuewc      (501) staff       (20)      310 2024-04-15 15:37:48.000000 xspex-0.0.4/helpers/report_xspec_version.cxx
+-rw-r--r--   0 xuewc      (501) staff       (20)    14197 2024-04-15 15:37:48.000000 xspex-0.0.4/helpers/template.py
+-rw-r--r--   0 xuewc      (501) staff       (20)      155 2024-04-15 15:37:48.000000 xspex-0.0.4/pyproject.toml
+-rw-r--r--   0 xuewc      (501) staff       (20)      816 2024-05-28 14:44:03.764635 xspex-0.0.4/setup.cfg
+-rw-r--r--   0 xuewc      (501) staff       (20)     3288 2024-05-28 14:32:05.000000 xspex-0.0.4/setup.py
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-05-28 14:44:03.760524 xspex-0.0.4/src/
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-05-28 14:44:03.760808 xspex-0.0.4/src/include/
+-rw-r--r--   0 xuewc      (501) staff       (20)    27131 2024-04-25 14:58:39.000000 xspex-0.0.4/src/include/xspex.hpp
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-05-28 14:44:03.761343 xspex-0.0.4/src/xspex/
+-rw-r--r--   0 xuewc      (501) staff       (20)   338104 2024-05-28 14:44:03.000000 xspex-0.0.4/src/xspex/__init__.py
+-rw-r--r--   0 xuewc      (501) staff       (20)    10035 2024-04-25 14:58:39.000000 xspex-0.0.4/src/xspex/primitive.py
+-rw-r--r--   0 xuewc      (501) staff       (20)    94741 2024-05-28 14:44:03.000000 xspex-0.0.4/src/xspex.cpp
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-05-28 14:44:03.763851 xspex-0.0.4/src/xspex.egg-info/
+-rw-r--r--   0 xuewc      (501) staff       (20)     1872 2024-05-28 14:44:03.000000 xspex-0.0.4/src/xspex.egg-info/PKG-INFO
+-rw-r--r--   0 xuewc      (501) staff       (20)      523 2024-05-28 14:44:03.000000 xspex-0.0.4/src/xspex.egg-info/SOURCES.txt
+-rw-r--r--   0 xuewc      (501) staff       (20)        1 2024-05-28 14:44:03.000000 xspex-0.0.4/src/xspex.egg-info/dependency_links.txt
+-rw-r--r--   0 xuewc      (501) staff       (20)        1 2024-05-28 14:27:33.000000 xspex-0.0.4/src/xspex.egg-info/not-zip-safe
+-rw-r--r--   0 xuewc      (501) staff       (20)       33 2024-05-28 14:44:03.000000 xspex-0.0.4/src/xspex.egg-info/requires.txt
+-rw-r--r--   0 xuewc      (501) staff       (20)        6 2024-05-28 14:44:03.000000 xspex-0.0.4/src/xspex.egg-info/top_level.txt
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-05-28 14:44:03.763058 xspex-0.0.4/template/
+-rw-r--r--   0 xuewc      (501) staff       (20)     4726 2024-04-17 10:50:41.000000 xspex-0.0.4/template/__init__.py
+-rw-r--r--   0 xuewc      (501) staff       (20)     7005 2024-04-16 18:49:11.000000 xspex-0.0.4/template/xspex.cpp
+drwxr-xr-x   0 xuewc      (501) staff       (20)        0 2024-05-28 14:44:03.763575 xspex-0.0.4/tests/
+-rw-r--r--   0 xuewc      (501) staff       (20)     6286 2024-04-18 18:10:32.000000 xspex-0.0.4/tests/test_basic.py
+-rw-r--r--   0 xuewc      (501) staff       (20)     7538 2024-04-28 14:20:58.000000 xspex-0.0.4/tests/test_primitive.py
```

### Comparing `xspex-0.0.3/LICENSE` & `xspex-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xspex-0.0.3/PKG-INFO` & `xspex-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspex
-Version: 0.0.3
+Version: 0.0.4
 Summary: Access Xspec models and corresponding JAX/XLA ops.
 Home-page: https://github.com/wcxve/xspex
 Author: Wang-Chen Xue
 Author-email: wcxuemail@gmail.com
 License: GNU GPL v3
 Platform: Linux
 Platform: Mac OS X
@@ -13,41 +13,52 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: jax>=0.4.16
+Requires-Dist: jaxlib>=0.4.16
 
 # xspex
 
 Access Xspec models and corresponding JAX/XLA ops, based on [xspec_models_cxc](https://github.com/cxcsds/xspec-models-cxc/) and [extending-jax](https://github.com/dfm/extending-jax).
 
 ## Installation
 
-Note: `HEASoft` & `Xspec` are required to be installed on your system. You can download it from [here](https://heasarc.gsfc.nasa.gov/lheasoft/).
+Note: ``HEASoft`` & ``Xspec v12.12.1+`` are required to be installed on your system.
+You can download it from [here](https://heasarc.gsfc.nasa.gov/lheasoft/).
 
 ```bash
 pip install xspex
 ```
 
 ## Example
 
 ```python
 import jax
 import jax.numpy as jnp
+import numpy as np
 import xspex
 
 # For accuracy, it is recommended to enable double precision
 jax.config.update('jax_enable_x64', True)
 
 # Get APEC model primitive, whose JVP rule is defined by finite difference 
 apec, info = xspex.get_primitive('apec')
 
-# Evaluate the model
+# Evaluate the model via JAX primitive
 value = apec(
     params=jnp.array([1.0, 1.0, 0.0]),
     egrid=jnp.geomspace(0.1, 0.2, 6),
     spec_num=1,
 )
 print(value)  # [1.27358561 0.37946811 0.2477116  0.1071355  0.10049102]
+
+# Evaluate the model function
+value2 = xspex.apec(
+    pars=np.array([1.0, 1.0, 0.0]),
+    energies=np.geomspace(0.1, 0.2, 6),
+)
+print(value2)  # [1.27358561 0.37946811 0.2477116  0.1071355  0.10049102]
 ```
```

### Comparing `xspex-0.0.3/helpers/identify_xspec.py` & `xspex-0.0.4/helpers/identify_xspec.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.3/helpers/template.py` & `xspex-0.0.4/helpers/template.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.3/setup.cfg` & `xspex-0.0.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 zip_safe = False
 install_requires = 
 	numpy
+	jax>=0.4.16
+	jaxlib>=0.4.16
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
 
 [options.packages.find]
 where = src
```

### Comparing `xspex-0.0.3/setup.py` & `xspex-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 
 sys.path.append(os.path.dirname(__file__))
 from helpers import template
 from helpers.identify_xspec import get_xspec_macros
 
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 
 # Check HEASARC is set up. The following does not provide a useful
 # message from 'pip install' so how do we make it more meaningful?
 #
 HEADAS = os.getenv('HEADAS')
 if HEADAS is None:
     sys.stderr.write('ERROR: unable to find HEADAS environment variable.\n')
```

### Comparing `xspex-0.0.3/src/include/xspex.hpp` & `xspex-0.0.4/src/include/xspex.hpp`

 * *Files identical despite different names*

### Comparing `xspex-0.0.3/src/xspex/__init__.py` & `xspex-0.0.4/src/xspex/__init__.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.3/src/xspex/primitive.py` & `xspex-0.0.4/src/xspex/primitive.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.3/src/xspex.cpp` & `xspex-0.0.4/src/xspex.cpp`

 * *Files identical despite different names*

### Comparing `xspex-0.0.3/src/xspex.egg-info/PKG-INFO` & `xspex-0.0.4/src/xspex.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspex
-Version: 0.0.3
+Version: 0.0.4
 Summary: Access Xspec models and corresponding JAX/XLA ops.
 Home-page: https://github.com/wcxve/xspex
 Author: Wang-Chen Xue
 Author-email: wcxuemail@gmail.com
 License: GNU GPL v3
 Platform: Linux
 Platform: Mac OS X
@@ -13,41 +13,52 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: jax>=0.4.16
+Requires-Dist: jaxlib>=0.4.16
 
 # xspex
 
 Access Xspec models and corresponding JAX/XLA ops, based on [xspec_models_cxc](https://github.com/cxcsds/xspec-models-cxc/) and [extending-jax](https://github.com/dfm/extending-jax).
 
 ## Installation
 
-Note: `HEASoft` & `Xspec` are required to be installed on your system. You can download it from [here](https://heasarc.gsfc.nasa.gov/lheasoft/).
+Note: ``HEASoft`` & ``Xspec v12.12.1+`` are required to be installed on your system.
+You can download it from [here](https://heasarc.gsfc.nasa.gov/lheasoft/).
 
 ```bash
 pip install xspex
 ```
 
 ## Example
 
 ```python
 import jax
 import jax.numpy as jnp
+import numpy as np
 import xspex
 
 # For accuracy, it is recommended to enable double precision
 jax.config.update('jax_enable_x64', True)
 
 # Get APEC model primitive, whose JVP rule is defined by finite difference 
 apec, info = xspex.get_primitive('apec')
 
-# Evaluate the model
+# Evaluate the model via JAX primitive
 value = apec(
     params=jnp.array([1.0, 1.0, 0.0]),
     egrid=jnp.geomspace(0.1, 0.2, 6),
     spec_num=1,
 )
 print(value)  # [1.27358561 0.37946811 0.2477116  0.1071355  0.10049102]
+
+# Evaluate the model function
+value2 = xspex.apec(
+    pars=np.array([1.0, 1.0, 0.0]),
+    energies=np.geomspace(0.1, 0.2, 6),
+)
+print(value2)  # [1.27358561 0.37946811 0.2477116  0.1071355  0.10049102]
 ```
```

### Comparing `xspex-0.0.3/src/xspex.egg-info/SOURCES.txt` & `xspex-0.0.4/src/xspex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xspex-0.0.3/template/__init__.py` & `xspex-0.0.4/template/__init__.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.3/template/xspex.cpp` & `xspex-0.0.4/template/xspex.cpp`

 * *Files identical despite different names*

### Comparing `xspex-0.0.3/tests/test_basic.py` & `xspex-0.0.4/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `xspex-0.0.3/tests/test_primitive.py` & `xspex-0.0.4/tests/test_primitive.py`

 * *Files identical despite different names*

