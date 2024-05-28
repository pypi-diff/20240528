# Comparing `tmp/unisim-0.0.2.tar.gz` & `tmp/unisim-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unisim-0.0.2.tar", last modified: Fri May 17 00:04:47 2024, max compression
+gzip compressed data, was "unisim-1.0.0.tar", last modified: Tue May 28 20:26:49 2024, max compression
```

## Comparing `unisim-0.0.2.tar` & `unisim-1.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:04:47.513437 unisim-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 00:03:39.000000 unisim-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 00:03:39.000000 unisim-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-05-17 00:04:47.513437 unisim-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-05-17 00:03:39.000000 unisim-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-17 00:03:39.000000 unisim-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 00:04:47.513437 unisim-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-17 00:03:39.000000 unisim-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:04:47.497437 unisim-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-17 00:03:39.000000 unisim-0.0.2/tests/test_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-17 00:03:39.000000 unisim-0.0.2/tests/test_textsim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:04:47.497437 unisim-0.0.2/unisim/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:04:47.501437 unisim-0.0.2/unisim/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/backend/load_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/backend/onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/backend/tf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:04:47.501437 unisim-0.0.2/unisim/embedder/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/embedder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/embedder/embedder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:04:47.489437 unisim-0.0.2/unisim/embedder/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:04:47.489437 unisim-0.0.2/unisim/embedder/models/text/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:04:47.501437 unisim-0.0.2/unisim/embedder/models/text/retsim/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:04:47.509437 unisim-0.0.2/unisim/embedder/models/text/retsim/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/embedder/models/text/retsim/v1/fingerprint.pb
--rw-r--r--   0 runner    (1001) docker     (127)    33457 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/embedder/models/text/retsim/v1/keras_metadata.pb
--rw-r--r--   0 runner    (1001) docker     (127)   418620 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/embedder/models/text/retsim/v1/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:04:47.513437 unisim-0.0.2/unisim/embedder/models/text/retsim/v1/variables/
--rw-r--r--   0 runner    (1001) docker     (127)  2160256 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/embedder/models/text/retsim/v1/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/embedder/models/text/retsim/v1/variables/variables.index
--rw-r--r--   0 runner    (1001) docker     (127)  6428768 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/embedder/models/text/retsim/v1.onnx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:04:47.513437 unisim-0.0.2/unisim/embedder/text/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/embedder/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/embedder/text/binarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/embedder/text/text_embedder.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/textsim.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-17 00:03:39.000000 unisim-0.0.2/unisim/unisim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:04:47.501437 unisim-0.0.2/unisim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-05-17 00:04:47.000000 unisim-0.0.2/unisim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-17 00:04:47.000000 unisim-0.0.2/unisim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 00:04:47.000000 unisim-0.0.2/unisim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-17 00:04:47.000000 unisim-0.0.2/unisim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 00:04:47.000000 unisim-0.0.2/unisim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:26:49.943418 unisim-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 20:26:02.000000 unisim-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 20:26:02.000000 unisim-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-28 20:26:49.943418 unisim-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8372 2024-05-28 20:26:02.000000 unisim-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 20:26:02.000000 unisim-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 20:26:49.943418 unisim-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-28 20:26:02.000000 unisim-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:26:49.923418 unisim-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-28 20:26:02.000000 unisim-1.0.0/tests/test_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-28 20:26:02.000000 unisim-1.0.0/tests/test_textsim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:26:49.927418 unisim-1.0.0/unisim/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:26:49.927418 unisim-1.0.0/unisim/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/backend/load_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/backend/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/backend/tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:26:49.927418 unisim-1.0.0/unisim/embedder/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/embedder/embedder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:26:49.923418 unisim-1.0.0/unisim/embedder/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:26:49.923418 unisim-1.0.0/unisim/embedder/models/text/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:26:49.927418 unisim-1.0.0/unisim/embedder/models/text/retsim/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:26:49.935418 unisim-1.0.0/unisim/embedder/models/text/retsim/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/embedder/models/text/retsim/v1/fingerprint.pb
+-rw-r--r--   0 runner    (1001) docker     (127)    33457 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/embedder/models/text/retsim/v1/keras_metadata.pb
+-rw-r--r--   0 runner    (1001) docker     (127)   418620 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/embedder/models/text/retsim/v1/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:26:49.939418 unisim-1.0.0/unisim/embedder/models/text/retsim/v1/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)  2160256 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/embedder/models/text/retsim/v1/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/embedder/models/text/retsim/v1/variables/variables.index
+-rw-r--r--   0 runner    (1001) docker     (127)  6428768 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/embedder/models/text/retsim/v1.onnx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:26:49.939418 unisim-1.0.0/unisim/embedder/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/embedder/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/embedder/text/binarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/embedder/text/text_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/textsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-28 20:26:02.000000 unisim-1.0.0/unisim/unisim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:26:49.927418 unisim-1.0.0/unisim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-28 20:26:49.000000 unisim-1.0.0/unisim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-28 20:26:49.000000 unisim-1.0.0/unisim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:26:49.000000 unisim-1.0.0/unisim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 20:26:49.000000 unisim-1.0.0/unisim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 20:26:49.000000 unisim-1.0.0/unisim.egg-info/top_level.txt
```

### Comparing `unisim-0.0.2/LICENSE` & `unisim-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/PKG-INFO` & `unisim-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: unisim
-Version: 0.0.2
+Version: 1.0.0
 Summary: UniSim: Universal Similarity
 Home-page: https://github.com/google/unisim
 Author: Google
 Author-email: unisim@google.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+Provides-Extra: tensorflow
 Provides-Extra: dev
 License-File: LICENSE
 
 # UniSim: Universal Similarity
 
 UniSim is a package for efficiently computing similarity, performing fuzzy matching, deduplicating datasets, and clustering data (text and images). The UniSim package is in beta and we may push breaking changes. The UniSim package currently supports text (e.g. for fuzzy string matching) and image support will be added soon.
 
 ## Installation
 You can use `pip` to install the latest version of UniSim:
 
 ```
 pip install unisim
 ```
 
-By default, UniSim uses [Onnx](https://github.com/onnx/onnx) as the runtime. You can switch to using TensorFlow by setting the `BACKEND` environment variable (e.g. `os.environ["BACKEND"] = "tf"`).
+By default, UniSim uses [Onnx](https://github.com/onnx/onnx) when running on CPU, and [TensorFlow](https://www.tensorflow.org/) for GPU acceleration. You can switch backends by setting the `BACKEND` environment variable (e.g. `os.environ["BACKEND"] = "tf"` or `"onnx"`). If you have a GPU, you can additionally install TensorFlow using:
+2
+```
+pip install unisim[tensorflow]
+```
 
 ## Text UniSim (TextSim)
 
 The goal of TextSim is to provide an easy-to-use tool for efficient, accurate and multilingual fuzzy string matching, near-duplicate detection, and string similarity. Please see the tutorial [colab](notebooks/unisim_text_demo.ipynb) for an in-depth example on using TextSim for real-world use cases like fuzzy matching for addresses.
 
 TextSim is significantly faster than edit-distance algorithms such as Levenshtein Distance for fuzzy string matching and more accurate than ngram-based methods such as MinHash for near-duplicate text detection and clustering. TextSim accepts strings of arbitrary length and can scale to datasets with millions of examples.
```

### Comparing `unisim-0.0.2/README.md` & `unisim-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 ## Installation
 You can use `pip` to install the latest version of UniSim:
 
 ```
 pip install unisim
 ```
 
-By default, UniSim uses [Onnx](https://github.com/onnx/onnx) as the runtime. You can switch to using TensorFlow by setting the `BACKEND` environment variable (e.g. `os.environ["BACKEND"] = "tf"`).
+By default, UniSim uses [Onnx](https://github.com/onnx/onnx) when running on CPU, and [TensorFlow](https://www.tensorflow.org/) for GPU acceleration. You can switch backends by setting the `BACKEND` environment variable (e.g. `os.environ["BACKEND"] = "tf"` or `"onnx"`). If you have a GPU, you can additionally install TensorFlow using:
+2
+```
+pip install unisim[tensorflow]
+```
 
 ## Text UniSim (TextSim)
 
 The goal of TextSim is to provide an easy-to-use tool for efficient, accurate and multilingual fuzzy string matching, near-duplicate detection, and string similarity. Please see the tutorial [colab](notebooks/unisim_text_demo.ipynb) for an in-depth example on using TextSim for real-world use cases like fuzzy matching for addresses.
 
 TextSim is significantly faster than edit-distance algorithms such as Levenshtein Distance for fuzzy string matching and more accurate than ngram-based methods such as MinHash for near-duplicate text detection and clustering. TextSim accepts strings of arbitrary length and can scale to datasets with millions of examples.
```

### Comparing `unisim-0.0.2/setup.py` & `unisim-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,22 +37,22 @@
     author_email="unisim@google.com",
     url="https://github.com/google/unisim",
     license="MIT",
     install_requires=[
         "tabulate",
         "numpy",
         "tqdm",
-        "onnx",
         "jaxtyping",
-        "onnxruntime-gpu",
+        "onnx",
+        "onnxruntime",
         "pandas",
-        "tensorflow>=2.11,<2.16",
         "usearch>=2.6.0",
     ],
     extras_require={
+        "tensorflow": ["tensorflow>=2.11,<2.16"],
         "dev": [
             "datasets",
             "mypy",
             "pytest",
             "flake8",
             "pytest-cov",
             "twine",
```

### Comparing `unisim-0.0.2/tests/test_indexer.py` & `unisim-1.0.0/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/tests/test_textsim.py` & `unisim-1.0.0/tests/test_textsim.py`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/backend/__init__.py` & `unisim-1.0.0/unisim/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/backend/load_backend.py` & `unisim-1.0.0/unisim/backend/load_backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,43 +26,50 @@
     try:
         import tensorflow as tf  # noqa: F403, F401
 
         TF_AVAILABLE = True
     except ImportError:
         TF_AVAILABLE = False
 
+# detect accelerator
+if TF_AVAILABLE or get_backend() == BackendType.tf:
+    devices_types = [d.device_type for d in tf.config.list_physical_devices()]
+
+    if "GPU" in devices_types:
+        set_accelerator(AcceleratorType.gpu)
+    else:
+        set_accelerator(AcceleratorType.cpu)
+
+else:
+    set_accelerator(AcceleratorType.cpu)
+
 # choose backend if not set by user
 accel = get_accelerator()
 backend = get_backend()
 
 if "BACKEND" not in os.environ:
     if backend != BackendType.unknown:
         # backend forced by the user
         pass
     elif accel == AcceleratorType.cpu:
         # on CPU always onnx
         set_backend(BackendType.onnx)
-    elif TF_AVAILABLE:
+    elif TF_AVAILABLE and accel == AcceleratorType.gpu:
         # on GPU use TF by default
         set_backend(BackendType.tf)
     else:
         # if TensorFlow not available
         set_backend(BackendType.onnx)
 
 # post detection
 if get_backend() == BackendType.onnx:
-    import onnxruntime as rt
-
     from .onnx import *  # noqa: F403, F401
 
-    # FIXME onnx accelerator type support
-    if rt.get_device() == "GPU":
-        set_accelerator(AcceleratorType.gpu)
-    else:
-        set_accelerator(AcceleratorType.cpu)
+    # FIXME(marinazh): onnx accelerator type support
+    set_accelerator(AcceleratorType.cpu)
 
 elif get_backend() == BackendType.tf:
     from .tf import *  # type: ignore # noqa: F403, F401
 
     # ensure we are not running out of memory
     gpus = tf.config.list_physical_devices("GPU")
     if gpus:
```

### Comparing `unisim-0.0.2/unisim/backend/onnx.py` & `unisim-1.0.0/unisim/backend/onnx.py`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/backend/tf.py` & `unisim-1.0.0/unisim/backend/tf.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from typing import Any, Sequence, Union
 
 import numpy as np
 import tensorflow as tf
 from tensorflow import Tensor
 from tensorflow.keras import Model
 
-# typing
 from ..types import BatchEmbeddings
 
 
 def cosine_similarity(query_embeddings: BatchEmbeddings, index_embeddings: BatchEmbeddings) -> Tensor:
     """Compute cosine similarity between embeddings using TensorFlow.
 
     Args:
```

### Comparing `unisim-0.0.2/unisim/config.py` & `unisim-1.0.0/unisim/config.py`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/dataclass.py` & `unisim-1.0.0/unisim/dataclass.py`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/embedder/embedder.py` & `unisim-1.0.0/unisim/embedder/embedder.py`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/embedder/models/text/retsim/v1/keras_metadata.pb` & `unisim-1.0.0/unisim/embedder/models/text/retsim/v1/keras_metadata.pb`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/embedder/models/text/retsim/v1/saved_model.pb` & `unisim-1.0.0/unisim/embedder/models/text/retsim/v1/saved_model.pb`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/embedder/models/text/retsim/v1/variables/variables.data-00000-of-00001` & `unisim-1.0.0/unisim/embedder/models/text/retsim/v1/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/embedder/models/text/retsim/v1/variables/variables.index` & `unisim-1.0.0/unisim/embedder/models/text/retsim/v1/variables/variables.index`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/embedder/models/text/retsim/v1.onnx` & `unisim-1.0.0/unisim/embedder/models/text/retsim/v1.onnx`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/embedder/text/binarizer.py` & `unisim-1.0.0/unisim/embedder/text/binarizer.py`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/embedder/text/text_embedder.py` & `unisim-1.0.0/unisim/embedder/text/text_embedder.py`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/enums.py` & `unisim-1.0.0/unisim/enums.py`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/indexer.py` & `unisim-1.0.0/unisim/indexer.py`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim/textsim.py` & `unisim-1.0.0/unisim/textsim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright 2023 Google LLC
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
+from __future__ import annotations
+
 from typing import Any, Dict, List, Sequence
 
 from pandas import DataFrame
 from tabulate import tabulate
 
 from .dataclass import Result, ResultCollection
 from .embedder import TextEmbedder
```

### Comparing `unisim-0.0.2/unisim/unisim.py` & `unisim-1.0.0/unisim/unisim.py`

 * *Files identical despite different names*

### Comparing `unisim-0.0.2/unisim.egg-info/PKG-INFO` & `unisim-1.0.0/unisim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: unisim
-Version: 0.0.2
+Version: 1.0.0
 Summary: UniSim: Universal Similarity
 Home-page: https://github.com/google/unisim
 Author: Google
 Author-email: unisim@google.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+Provides-Extra: tensorflow
 Provides-Extra: dev
 License-File: LICENSE
 
 # UniSim: Universal Similarity
 
 UniSim is a package for efficiently computing similarity, performing fuzzy matching, deduplicating datasets, and clustering data (text and images). The UniSim package is in beta and we may push breaking changes. The UniSim package currently supports text (e.g. for fuzzy string matching) and image support will be added soon.
 
 ## Installation
 You can use `pip` to install the latest version of UniSim:
 
 ```
 pip install unisim
 ```
 
-By default, UniSim uses [Onnx](https://github.com/onnx/onnx) as the runtime. You can switch to using TensorFlow by setting the `BACKEND` environment variable (e.g. `os.environ["BACKEND"] = "tf"`).
+By default, UniSim uses [Onnx](https://github.com/onnx/onnx) when running on CPU, and [TensorFlow](https://www.tensorflow.org/) for GPU acceleration. You can switch backends by setting the `BACKEND` environment variable (e.g. `os.environ["BACKEND"] = "tf"` or `"onnx"`). If you have a GPU, you can additionally install TensorFlow using:
+2
+```
+pip install unisim[tensorflow]
+```
 
 ## Text UniSim (TextSim)
 
 The goal of TextSim is to provide an easy-to-use tool for efficient, accurate and multilingual fuzzy string matching, near-duplicate detection, and string similarity. Please see the tutorial [colab](notebooks/unisim_text_demo.ipynb) for an in-depth example on using TextSim for real-world use cases like fuzzy matching for addresses.
 
 TextSim is significantly faster than edit-distance algorithms such as Levenshtein Distance for fuzzy string matching and more accurate than ngram-based methods such as MinHash for near-duplicate text detection and clustering. TextSim accepts strings of arbitrary length and can scale to datasets with millions of examples.
```

### Comparing `unisim-0.0.2/unisim.egg-info/SOURCES.txt` & `unisim-1.0.0/unisim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

