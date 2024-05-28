# Comparing `tmp/hypothesis_torch-0.7.1.tar.gz` & `tmp/hypothesis_torch-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis_torch-0.7.1.tar", last modified: Fri May 24 19:57:20 2024, max compression
+gzip compressed data, was "hypothesis_torch-0.7.2.tar", last modified: Tue May 28 17:17:33 2024, max compression
```

## Comparing `hypothesis_torch-0.7.1.tar` & `hypothesis_torch-0.7.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 19:57:20.511869 hypothesis_torch-0.7.1/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9338 2024-05-24 19:57:20.511869 hypothesis_torch-0.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5682 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 19:57:20.507869 hypothesis_torch-0.7.1/hypothesis_torch/
--rw-r--r--   0 root         (0) root         (0)     2168 2024-05-24 19:57:17.000000 hypothesis_torch-0.7.1/hypothesis_torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1340 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/hypothesis_torch/device.py
--rw-r--r--   0 root         (0) root         (0)     2727 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/hypothesis_torch/dtype.py
--rw-r--r--   0 root         (0) root         (0)    11710 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/hypothesis_torch/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     3036 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/hypothesis_torch/inspection_util.py
--rw-r--r--   0 root         (0) root         (0)      743 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/hypothesis_torch/layout.py
--rw-r--r--   0 root         (0) root         (0)      854 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/hypothesis_torch/memory_format.py
--rw-r--r--   0 root         (0) root         (0)    11193 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/hypothesis_torch/module.py
--rw-r--r--   0 root         (0) root         (0)     4914 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/hypothesis_torch/optim.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/hypothesis_torch/py.typed
--rw-r--r--   0 root         (0) root         (0)      995 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/hypothesis_torch/register_random_torch_state.py
--rw-r--r--   0 root         (0) root         (0)     9326 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/hypothesis_torch/tensor.py
--rw-r--r--   0 root         (0) root         (0)     1460 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/hypothesis_torch/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 19:57:20.507869 hypothesis_torch-0.7.1/hypothesis_torch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9338 2024-05-24 19:57:20.000000 hypothesis_torch-0.7.1/hypothesis_torch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      665 2024-05-24 19:57:20.000000 hypothesis_torch-0.7.1/hypothesis_torch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 19:57:20.000000 hypothesis_torch-0.7.1/hypothesis_torch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2024-05-24 19:57:20.000000 hypothesis_torch-0.7.1/hypothesis_torch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-24 19:57:20.000000 hypothesis_torch-0.7.1/hypothesis_torch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-24 19:57:20.000000 hypothesis_torch-0.7.1/hypothesis_torch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3149 2024-05-24 19:56:46.000000 hypothesis_torch-0.7.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 19:57:20.511869 hypothesis_torch-0.7.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:17:33.249532 hypothesis_torch-0.7.2/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9338 2024-05-28 17:17:33.249532 hypothesis_torch-0.7.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5682 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:17:33.245532 hypothesis_torch-0.7.2/hypothesis_torch/
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-05-28 17:17:29.000000 hypothesis_torch-0.7.2/hypothesis_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/hypothesis_torch/device.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/hypothesis_torch/dtype.py
+-rw-r--r--   0 root         (0) root         (0)    11710 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/hypothesis_torch/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/hypothesis_torch/inspection_util.py
+-rw-r--r--   0 root         (0) root         (0)      743 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/hypothesis_torch/layout.py
+-rw-r--r--   0 root         (0) root         (0)      854 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/hypothesis_torch/memory_format.py
+-rw-r--r--   0 root         (0) root         (0)    11193 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/hypothesis_torch/module.py
+-rw-r--r--   0 root         (0) root         (0)     4914 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/hypothesis_torch/optim.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/hypothesis_torch/py.typed
+-rw-r--r--   0 root         (0) root         (0)      995 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/hypothesis_torch/register_random_torch_state.py
+-rw-r--r--   0 root         (0) root         (0)     9326 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/hypothesis_torch/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/hypothesis_torch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 17:17:33.249532 hypothesis_torch-0.7.2/hypothesis_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9338 2024-05-28 17:17:33.000000 hypothesis_torch-0.7.2/hypothesis_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      665 2024-05-28 17:17:33.000000 hypothesis_torch-0.7.2/hypothesis_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 17:17:33.000000 hypothesis_torch-0.7.2/hypothesis_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2024-05-28 17:17:33.000000 hypothesis_torch-0.7.2/hypothesis_torch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-28 17:17:33.000000 hypothesis_torch-0.7.2/hypothesis_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-28 17:17:33.000000 hypothesis_torch-0.7.2/hypothesis_torch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3149 2024-05-28 17:16:57.000000 hypothesis_torch-0.7.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 17:17:33.249532 hypothesis_torch-0.7.2/setup.cfg
```

### Comparing `hypothesis_torch-0.7.1/LICENSE` & `hypothesis_torch-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/PKG-INFO` & `hypothesis_torch-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.7.1
+Version: 0.7.2
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,15 +60,15 @@
 Requires-Dist: pyright==1.1.364; extra == "dev"
 Requires-Dist: pytest==8.2.1; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.6.0; extra == "docs"
 Requires-Dist: mkdocstrings[python]==0.25.1; extra == "docs"
 Requires-Dist: mkdocs-autolinks-plugin==0.7.1; extra == "docs"
-Requires-Dist: mkdocs-material==9.5.24; extra == "docs"
+Requires-Dist: mkdocs-material==9.5.25; extra == "docs"
 Requires-Dist: mkdocs-snippets==1.3.0; extra == "docs"
 Requires-Dist: mkdocs-exclude==1.0.2; extra == "docs"
 
 [![PyPI version](https://img.shields.io/pypi/v/hypothesis-torch.svg)](https://pypi.org/project/hypothesis-torch) ![PyPI - Downloads](https://img.shields.io/pypi/dm/hypothesis-torch)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
```

### Comparing `hypothesis_torch-0.7.1/README.md` & `hypothesis_torch-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch/__init__.py` & `hypothesis_torch-0.7.2/hypothesis_torch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
 """
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 import importlib.util
 
 from hypothesis_torch.device import (
     AVAILABLE_CPU_DEVICES,
     AVAILABLE_CUDA_DEVICES,
     AVAILABLE_META_DEVICES,
     AVAILABLE_MPS_DEVICES,
```

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch/device.py` & `hypothesis_torch-0.7.2/hypothesis_torch/device.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch/dtype.py` & `hypothesis_torch-0.7.2/hypothesis_torch/dtype.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch/huggingface.py` & `hypothesis_torch-0.7.2/hypothesis_torch/huggingface.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch/inspection_util.py` & `hypothesis_torch-0.7.2/hypothesis_torch/inspection_util.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch/layout.py` & `hypothesis_torch-0.7.2/hypothesis_torch/layout.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch/memory_format.py` & `hypothesis_torch-0.7.2/hypothesis_torch/memory_format.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch/module.py` & `hypothesis_torch-0.7.2/hypothesis_torch/module.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch/optim.py` & `hypothesis_torch-0.7.2/hypothesis_torch/optim.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch/register_random_torch_state.py` & `hypothesis_torch-0.7.2/hypothesis_torch/register_random_torch_state.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch/tensor.py` & `hypothesis_torch-0.7.2/hypothesis_torch/tensor.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch/utils.py` & `hypothesis_torch-0.7.2/hypothesis_torch/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch.egg-info/PKG-INFO` & `hypothesis_torch-0.7.2/hypothesis_torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.7.1
+Version: 0.7.2
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,15 +60,15 @@
 Requires-Dist: pyright==1.1.364; extra == "dev"
 Requires-Dist: pytest==8.2.1; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.6.0; extra == "docs"
 Requires-Dist: mkdocstrings[python]==0.25.1; extra == "docs"
 Requires-Dist: mkdocs-autolinks-plugin==0.7.1; extra == "docs"
-Requires-Dist: mkdocs-material==9.5.24; extra == "docs"
+Requires-Dist: mkdocs-material==9.5.25; extra == "docs"
 Requires-Dist: mkdocs-snippets==1.3.0; extra == "docs"
 Requires-Dist: mkdocs-exclude==1.0.2; extra == "docs"
 
 [![PyPI version](https://img.shields.io/pypi/v/hypothesis-torch.svg)](https://pypi.org/project/hypothesis-torch) ![PyPI - Downloads](https://img.shields.io/pypi/dm/hypothesis-torch)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
```

### Comparing `hypothesis_torch-0.7.1/hypothesis_torch.egg-info/SOURCES.txt` & `hypothesis_torch-0.7.2/hypothesis_torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.7.1/pyproject.toml` & `hypothesis_torch-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
   "pytest==8.2.1",
   "pytest-cov==5.0.0"
 ]
 docs = [
   "mkdocs==1.6.0",
   "mkdocstrings[python]==0.25.1",
   "mkdocs-autolinks-plugin==0.7.1",
-  "mkdocs-material==9.5.24",
+  "mkdocs-material==9.5.25",
   "mkdocs-snippets==1.3.0",
   "mkdocs-exclude==1.0.2",
 ]
 
 [project.urls]
 Homepage = "https://github.com/qthequartermasterman/hypothesis-torch"
 Documentation = "https://hypothesis-torch.readthedocs.io/en/stable/"
```

