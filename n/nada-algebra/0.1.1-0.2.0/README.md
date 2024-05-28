# Comparing `tmp/nada_algebra-0.1.1.tar.gz` & `tmp/nada_algebra-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nada_algebra-0.1.1.tar", max compression
+gzip compressed data, was "nada_algebra-0.2.0.tar", max compression
```

## Comparing `nada_algebra-0.1.1.tar` & `nada_algebra-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11303 2024-05-17 14:32:21.033925 nada_algebra-0.1.1/LICENSE
--rw-r--r--   0        0        0     1348 2024-05-20 15:31:21.484494 nada_algebra-0.1.1/README.md
--rw-r--r--   0        0        0       71 2024-05-20 10:00:30.199434 nada_algebra-0.1.1/nada_algebra/__init__.py
--rw-r--r--   0        0        0    11730 2024-05-20 15:18:05.813514 nada_algebra-0.1.1/nada_algebra/array.py
--rw-r--r--   0        0        0     2197 2024-05-20 09:17:18.758994 nada_algebra-0.1.1/nada_algebra/client.py
--rw-r--r--   0        0        0     4402 2024-05-20 09:17:18.760024 nada_algebra-0.1.1/nada_algebra/funcs.py
--rw-r--r--   0        0        0      429 2024-05-20 15:38:35.642077 nada_algebra-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 nada_algebra-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11303 2024-05-28 13:17:34.553701 nada_algebra-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1348 2024-05-28 13:17:34.553701 nada_algebra-0.2.0/README.md
+-rw-r--r--   0        0        0      168 2024-05-28 13:17:34.557701 nada_algebra-0.2.0/nada_algebra/__init__.py
+-rw-r--r--   0        0        0    14172 2024-05-28 13:17:34.557701 nada_algebra-0.2.0/nada_algebra/array.py
+-rw-r--r--   0        0        0     2201 2024-05-28 13:17:34.557701 nada_algebra-0.2.0/nada_algebra/client.py
+-rw-r--r--   0        0        0     7267 2024-05-28 13:17:34.557701 nada_algebra-0.2.0/nada_algebra/funcs.py
+-rw-r--r--   0        0        0    15140 2024-05-28 13:17:34.557701 nada_algebra-0.2.0/nada_algebra/types.py
+-rw-r--r--   0        0        0      429 2024-05-28 13:17:34.557701 nada_algebra-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 nada_algebra-0.2.0/PKG-INFO
```

### Comparing `nada_algebra-0.1.1/LICENSE` & `nada_algebra-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nada_algebra-0.1.1/README.md` & `nada_algebra-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nada_algebra-0.1.1/nada_algebra/client.py` & `nada_algebra-0.2.0/nada_algebra/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module provides functions to work with the Python Nillion Client for handling
 secret and public variable integers and generating named party objects and input dictionaries.
 """
 
+from typing import Union
 from py_nillion_client import (
     SecretInteger,
     SecretUnsignedInteger,
     PublicVariableInteger,
     PublicVariableUnsignedInteger,
 )
 import numpy as np
@@ -25,20 +26,20 @@
     """
     return [f"{prefix}{i}" for i in range(num)]
 
 
 def array(
     arr: np.ndarray,
     prefix: str,
-    nada_type: (
-        type(SecretInteger)
-        | type(SecretUnsignedInteger)
-        | type(PublicVariableInteger)
-        | type(PublicVariableUnsignedInteger)
-    ) = SecretInteger,
+    nada_type: Union[
+        SecretInteger,
+        SecretUnsignedInteger,
+        PublicVariableInteger,
+        PublicVariableUnsignedInteger,
+    ] = SecretInteger,
 ) -> dict:
     """
     Recursively generates a dictionary of Nillion input objects for each element
     in the given array.
 
     Args:
         arr (np.ndarray): The input array.
```

### Comparing `nada_algebra-0.1.1/PKG-INFO` & `nada_algebra-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nada-algebra
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 Author: José Cabrero-Holgueras
 Author-email: jose.cabrero@nillion.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

