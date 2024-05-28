# Comparing `tmp/py-progress-tracker-0.6.0.tar.gz` & `tmp/py_progress_tracker-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-progress-tracker-0.6.0.tar", max compression
+gzip compressed data, was "py_progress_tracker-0.7.0.tar", max compression
```

## Comparing `py-progress-tracker-0.6.0.tar` & `py_progress_tracker-0.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      146 2022-09-14 11:26:48.459413 py-progress-tracker-0.6.0/py_progress_tracker/__init__.py
--rw-r--r--   0        0        0     1519 2022-09-14 11:26:48.459413 py-progress-tracker-0.6.0/py_progress_tracker/measure.py
--rw-r--r--   0        0        0       43 2022-09-14 11:26:48.459413 py-progress-tracker-0.6.0/py_progress_tracker/state.py
--rw-r--r--   0        0        0     7604 2022-09-14 11:26:48.459413 py-progress-tracker-0.6.0/py_progress_tracker/track.py
--rw-r--r--   0        0        0      492 2022-09-14 12:13:28.112187 py-progress-tracker-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      734 2022-09-14 12:13:54.835864 py-progress-tracker-0.6.0/setup.py
--rw-r--r--   0        0        0      627 2022-09-14 12:13:54.836117 py-progress-tracker-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      146 2024-05-28 07:33:15.537488 py_progress_tracker-0.7.0/py_progress_tracker/__init__.py
+-rw-r--r--   0        0        0     1519 2024-05-28 07:33:15.537615 py_progress_tracker-0.7.0/py_progress_tracker/measure.py
+-rw-r--r--   0        0        0       43 2024-05-28 07:33:15.537772 py_progress_tracker-0.7.0/py_progress_tracker/state.py
+-rw-r--r--   0        0        0     7604 2024-05-28 07:33:15.537938 py_progress_tracker-0.7.0/py_progress_tracker/track.py
+-rw-r--r--   0        0        0      486 2024-05-28 07:33:15.538049 py_progress_tracker-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 py_progress_tracker-0.7.0/setup.py
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 py_progress_tracker-0.7.0/PKG-INFO
```

### Comparing `py-progress-tracker-0.6.0/py_progress_tracker/measure.py` & `py_progress_tracker-0.7.0/py_progress_tracker/measure.py`

 * *Files identical despite different names*

### Comparing `py-progress-tracker-0.6.0/py_progress_tracker/track.py` & `py_progress_tracker-0.7.0/py_progress_tracker/track.py`

 * *Files identical despite different names*

### Comparing `py-progress-tracker-0.6.0/setup.py` & `py_progress_tracker-0.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,23 @@
  'psutil>=5.8.0,<6.0.0',
  'py-cpuinfo>=8.0.0,<9.0.0',
  'tabulate>=0.8.9,<0.9.0',
  'termcolor>=1.1.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'py-progress-tracker',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'A simple benchmarking library',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Zama',
     'author_email': 'hello@zama.ai',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<3.11',
+    'python_requires': '>=3.7',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `py-progress-tracker-0.6.0/PKG-INFO` & `py_progress_tracker-0.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: py-progress-tracker
-Version: 0.6.0
+Version: 0.7.0
 Summary: A simple benchmarking library
 Author: Zama
 Author-email: hello@zama.ai
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.4,<0.5.0)
 Requires-Dist: psutil (>=5.8.0,<6.0.0)
 Requires-Dist: py-cpuinfo (>=8.0.0,<9.0.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
```

