# Comparing `tmp/zamba_torch-0.0.2.tar.gz` & `tmp/zamba_torch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zamba_torch-0.0.2.tar", max compression
+gzip compressed data, was "zamba_torch-0.0.3.tar", max compression
```

## Comparing `zamba_torch-0.0.2.tar` & `zamba_torch-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-05-28 14:10:54.098838 zamba_torch-0.0.2/LICENSE
--rw-r--r--   0        0        0       95 2024-05-28 15:16:00.309213 zamba_torch-0.0.2/README.md
--rw-r--r--   0        0        0     1335 2024-05-28 15:26:00.493375 zamba_torch-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       66 2024-05-28 15:17:06.467332 zamba_torch-0.0.2/zamba_torch/__init__.py
--rw-r--r--   0        0        0    11828 2024-05-28 15:25:36.582918 zamba_torch-0.0.2/zamba_torch/main.py
--rw-r--r--   0        0        0     2184 2024-05-28 15:15:42.024774 zamba_torch-0.0.2/zamba_torch/omni_proj.py
--rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 zamba_torch-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-28 14:10:54.098838 zamba_torch-0.0.3/LICENSE
+-rw-r--r--   0        0        0       95 2024-05-28 15:16:00.309213 zamba_torch-0.0.3/README.md
+-rw-r--r--   0        0        0     1335 2024-05-28 15:27:13.443849 zamba_torch-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       82 2024-05-28 15:26:59.745514 zamba_torch-0.0.3/zamba_torch/__init__.py
+-rw-r--r--   0        0        0    11828 2024-05-28 15:25:36.582918 zamba_torch-0.0.3/zamba_torch/main.py
+-rw-r--r--   0        0        0     2184 2024-05-28 15:15:42.024774 zamba_torch-0.0.3/zamba_torch/omni_proj.py
+-rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 zamba_torch-0.0.3/PKG-INFO
```

### Comparing `zamba_torch-0.0.2/LICENSE` & `zamba_torch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zamba_torch-0.0.2/pyproject.toml` & `zamba_torch-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "zamba-torch"
-version = "0.0.2"
+version = "0.0.3"
 description = "zamba - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/zamba"
 documentation = "https://github.com/kyegomez/zamba"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/zamba"
```

### Comparing `zamba_torch-0.0.2/zamba_torch/main.py` & `zamba_torch-0.0.3/zamba_torch/main.py`

 * *Files identical despite different names*

### Comparing `zamba_torch-0.0.2/zamba_torch/omni_proj.py` & `zamba_torch-0.0.3/zamba_torch/omni_proj.py`

 * *Files identical despite different names*

### Comparing `zamba_torch-0.0.2/PKG-INFO` & `zamba_torch-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zamba-torch
-Version: 0.0.2
+Version: 0.0.3
 Summary: zamba - Pytorch
 Home-page: https://github.com/kyegomez/zamba
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
```

