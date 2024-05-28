# Comparing `tmp/modelagnosticsafeaipackage-0.2.0.tar.gz` & `tmp/modelagnosticsafeaipackage-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelagnosticsafeaipackage-0.2.0.tar", last modified: Tue May 28 09:23:03 2024, max compression
+gzip compressed data, was "modelagnosticsafeaipackage-0.3.0.tar", last modified: Tue May 28 09:29:08 2024, max compression
```

## Comparing `modelagnosticsafeaipackage-0.2.0.tar` & `modelagnosticsafeaipackage-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 09:23:03.952455 modelagnosticsafeaipackage-0.2.0/
--rw-rw-rw-   0        0        0     1086 2024-05-26 18:09:20.000000 modelagnosticsafeaipackage-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4988 2024-05-28 09:23:03.951353 modelagnosticsafeaipackage-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4386 2024-05-28 09:08:56.000000 modelagnosticsafeaipackage-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 09:23:03.947494 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/
--rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/__init__.py
--rw-rw-rw-   0        0        0     3465 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_accuracy.py
--rw-rw-rw-   0        0        0     1336 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_explainability.py
--rw-rw-rw-   0        0        0     1296 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_fairness.py
--rw-rw-rw-   0        0        0     1291 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_privacy.py
--rw-rw-rw-   0        0        0     1424 2024-05-28 09:16:01.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_robustness.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:23:03.951353 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/utils/
--rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/utils/__init__.py
--rw-rw-rw-   0        0        0     2646 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/utils/util.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:23:03.949486 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/
--rw-rw-rw-   0        0        0     4988 2024-05-28 09:23:03.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2024-05-28 09:23:03.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 09:23:03.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-28 09:23:03.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 09:23:03.952455 modelagnosticsafeaipackage-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1117 2024-05-28 09:20:12.000000 modelagnosticsafeaipackage-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:29:08.498377 modelagnosticsafeaipackage-0.3.0/
+-rw-rw-rw-   0        0        0     1086 2024-05-26 18:09:20.000000 modelagnosticsafeaipackage-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4988 2024-05-28 09:29:08.497343 modelagnosticsafeaipackage-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4386 2024-05-28 09:08:56.000000 modelagnosticsafeaipackage-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 09:29:08.493585 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/
+-rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/__init__.py
+-rw-rw-rw-   0        0        0     3465 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/check_accuracy.py
+-rw-rw-rw-   0        0        0     1337 2024-05-28 09:27:36.000000 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/check_explainability.py
+-rw-rw-rw-   0        0        0     1297 2024-05-28 09:27:49.000000 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/check_fairness.py
+-rw-rw-rw-   0        0        0     1292 2024-05-28 09:27:56.000000 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/check_privacy.py
+-rw-rw-rw-   0        0        0     1424 2024-05-28 09:28:38.000000 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/check_robustness.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:29:08.497343 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/utils/__init__.py
+-rw-rw-rw-   0        0        0     2646 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/utils/util.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:29:08.495343 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage.egg-info/
+-rw-rw-rw-   0        0        0     4988 2024-05-28 09:29:08.000000 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2024-05-28 09:29:08.000000 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 09:29:08.000000 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-28 09:29:08.000000 modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 09:29:08.498377 modelagnosticsafeaipackage-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2024-05-28 09:28:54.000000 modelagnosticsafeaipackage-0.3.0/setup.py
```

### Comparing `modelagnosticsafeaipackage-0.2.0/LICENSE` & `modelagnosticsafeaipackage-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.2.0/PKG-INFO` & `modelagnosticsafeaipackage-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelagnosticsafeaipackage
-Version: 0.2.0
+Version: 0.3.0
 Summary: MODEL AGNOSTIC SAFE AI package to measure risks of AI models WITHOUT CONSIDERING TYPE OF THE MODEL
 Author: Golnoosh Babaei
 Author-email: <golnoosh.babaei93@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `modelagnosticsafeaipackage-0.2.0/README.md` & `modelagnosticsafeaipackage-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_accuracy.py` & `modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/check_accuracy.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_explainability.py` & `modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/check_explainability.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import numpy as np
 import scipy
 import matplotlib.pyplot as plt
-from utils.util import _num, _den, _test_delta_function
+from .utils.util import _num, _den, _test_delta_function
 from check_accuracy import rga
 
   
 def rge(yhat, yhat_rm):
     """
     ### RANK GRADUATION EXPLAINABILITY (RGE) MEASURE ###
     Function for the RGE measure computation
```

### Comparing `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_fairness.py` & `modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/check_fairness.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import numpy as np
 import scipy
-from utils.util import _num, _den, _test_delta_function
+from .utils.util import _num, _den, _test_delta_function
 from check_accuracy import rga
 
 def rgf(yhat, yhat_rm):
     """
     ### RANK GRADUATION FAIRNESS (RGF) MEASURE ###
     Function for the RGF measure computation
     """
```

### Comparing `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_privacy.py` & `modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/check_privacy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import numpy as np
 import scipy
-from utils.util import _num, _den, _test_delta_function
+from .utils.util import _num, _den, _test_delta_function
 from check_accuracy import rga
 
 def rgp(yhat, yhat_rm):
     """
     ### RANK GRADUATION PRIVACY (RGP) MEASURE ###
     Function for the RGP measure computation
     """
```

### Comparing `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_robustness.py` & `modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/check_robustness.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/utils/util.py` & `modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage/utils/util.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/PKG-INFO` & `modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelagnosticsafeaipackage
-Version: 0.2.0
+Version: 0.3.0
 Summary: MODEL AGNOSTIC SAFE AI package to measure risks of AI models WITHOUT CONSIDERING TYPE OF THE MODEL
 Author: Golnoosh Babaei
 Author-email: <golnoosh.babaei93@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt` & `modelagnosticsafeaipackage-0.3.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.2.0/setup.py` & `modelagnosticsafeaipackage-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 
 # Open README.md with UTF-8 encoding
 with open(this_directory / "README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '0.2.0'
+VERSION = '0.3.0'
 DESCRIPTION = 'MODEL AGNOSTIC SAFE AI package to measure risks of AI models WITHOUT CONSIDERING TYPE OF THE MODEL'
 
 # Setting up
 setup(
     name="modelagnosticsafeaipackage",
     version=VERSION,
     author="Golnoosh Babaei",
```

