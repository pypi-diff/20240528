# Comparing `tmp/modelagnosticsafeaipackage-0.1.0.tar.gz` & `tmp/modelagnosticsafeaipackage-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelagnosticsafeaipackage-0.1.0.tar", last modified: Tue May 28 09:07:12 2024, max compression
+gzip compressed data, was "modelagnosticsafeaipackage-0.2.0.tar", last modified: Tue May 28 09:23:03 2024, max compression
```

## Comparing `modelagnosticsafeaipackage-0.1.0.tar` & `modelagnosticsafeaipackage-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 09:07:12.964346 modelagnosticsafeaipackage-0.1.0/
--rw-rw-rw-   0        0        0     1086 2024-05-26 18:09:20.000000 modelagnosticsafeaipackage-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4920 2024-05-28 09:07:12.963346 modelagnosticsafeaipackage-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4371 2024-05-26 14:20:44.000000 modelagnosticsafeaipackage-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 09:07:12.958856 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/
--rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/__init__.py
--rw-rw-rw-   0        0        0     3465 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/check_accuracy.py
--rw-rw-rw-   0        0        0     1336 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/check_explainability.py
--rw-rw-rw-   0        0        0     1296 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/check_fairness.py
--rw-rw-rw-   0        0        0     1291 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/check_privacy.py
--rw-rw-rw-   0        0        0     1458 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/check_robustness.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:07:12.963346 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/utils/
--rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/utils/__init__.py
--rw-rw-rw-   0        0        0     2646 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/utils/util.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:07:12.962342 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage.egg-info/
--rw-rw-rw-   0        0        0     4920 2024-05-28 09:07:12.000000 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2024-05-28 09:07:12.000000 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 09:07:12.000000 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-28 09:07:12.000000 modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 09:07:12.964346 modelagnosticsafeaipackage-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1064 2024-05-28 09:06:11.000000 modelagnosticsafeaipackage-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:23:03.952455 modelagnosticsafeaipackage-0.2.0/
+-rw-rw-rw-   0        0        0     1086 2024-05-26 18:09:20.000000 modelagnosticsafeaipackage-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4988 2024-05-28 09:23:03.951353 modelagnosticsafeaipackage-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4386 2024-05-28 09:08:56.000000 modelagnosticsafeaipackage-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 09:23:03.947494 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/
+-rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/__init__.py
+-rw-rw-rw-   0        0        0     3465 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_accuracy.py
+-rw-rw-rw-   0        0        0     1336 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_explainability.py
+-rw-rw-rw-   0        0        0     1296 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_fairness.py
+-rw-rw-rw-   0        0        0     1291 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_privacy.py
+-rw-rw-rw-   0        0        0     1424 2024-05-28 09:16:01.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_robustness.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:23:03.951353 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/utils/__init__.py
+-rw-rw-rw-   0        0        0     2646 2024-05-26 14:17:04.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/utils/util.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:23:03.949486 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/
+-rw-rw-rw-   0        0        0     4988 2024-05-28 09:23:03.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2024-05-28 09:23:03.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 09:23:03.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-28 09:23:03.000000 modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 09:23:03.952455 modelagnosticsafeaipackage-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2024-05-28 09:20:12.000000 modelagnosticsafeaipackage-0.2.0/setup.py
```

### Comparing `modelagnosticsafeaipackage-0.1.0/LICENSE` & `modelagnosticsafeaipackage-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.1.0/PKG-INFO` & `modelagnosticsafeaipackage-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: modelagnosticsafeaipackage
-Version: 0.1.0
-Summary: SAFE AI package to measure risks of AI models
+Version: 0.2.0
+Summary: MODEL AGNOSTIC SAFE AI package to measure risks of AI models WITHOUT CONSIDERING TYPE OF THE MODEL
 Author: Golnoosh Babaei
 Author-email: <golnoosh.babaei93@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SAFE AI
+# MODEL AGNOSTIC SAFE AI
 
 The increasing widespread of Artificial Intelligence (AI) applications implies the formalisa-
 tion of an AI risk management model which needs methodological guidelines for an effec-
 tive implementation. To fill the gap, [Giudici and Raffinetti (2023)](https://www.sciencedirect.com/science/article/pii/S1544612323004609) 
 introduced a S.A.F.E.
 risk management model which derives from the proposed international regulations four main
 compliance principles: Security, Accuracy, Fairness and Explainability, that can be measured
```

### Comparing `modelagnosticsafeaipackage-0.1.0/README.md` & `modelagnosticsafeaipackage-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SAFE AI
+# MODEL AGNOSTIC SAFE AI
 
 The increasing widespread of Artificial Intelligence (AI) applications implies the formalisa-
 tion of an AI risk management model which needs methodological guidelines for an effec-
 tive implementation. To fill the gap, [Giudici and Raffinetti (2023)](https://www.sciencedirect.com/science/article/pii/S1544612323004609) 
 introduced a S.A.F.E.
 risk management model which derives from the proposed international regulations four main
 compliance principles: Security, Accuracy, Fairness and Explainability, that can be measured
```

### Comparing `modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/check_accuracy.py` & `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_accuracy.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/check_explainability.py` & `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_explainability.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/check_fairness.py` & `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_fairness.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/check_privacy.py` & `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_privacy.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/check_robustness.py` & `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/check_robustness.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pandas as pd
 import numpy as np
 import scipy
-from utils.util import _den, _num
-from check_accuracy import rga
+from .check_accuracy import rga
 
 def rgr(yhat, yhat_pert):
     """
         ### RANK GRADUATION Robustness (RGR) MEASURE ###
         Function for the RGR measure computation regarding perturbation of a single variable
     """ 
     rgr = rga(yhat, yhat_pert)
```

### Comparing `modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage/utils/util.py` & `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage/utils/util.py`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage.egg-info/PKG-INFO` & `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: modelagnosticsafeaipackage
-Version: 0.1.0
-Summary: SAFE AI package to measure risks of AI models
+Version: 0.2.0
+Summary: MODEL AGNOSTIC SAFE AI package to measure risks of AI models WITHOUT CONSIDERING TYPE OF THE MODEL
 Author: Golnoosh Babaei
 Author-email: <golnoosh.babaei93@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SAFE AI
+# MODEL AGNOSTIC SAFE AI
 
 The increasing widespread of Artificial Intelligence (AI) applications implies the formalisa-
 tion of an AI risk management model which needs methodological guidelines for an effec-
 tive implementation. To fill the gap, [Giudici and Raffinetti (2023)](https://www.sciencedirect.com/science/article/pii/S1544612323004609) 
 introduced a S.A.F.E.
 risk management model which derives from the proposed international regulations four main
 compliance principles: Security, Accuracy, Fairness and Explainability, that can be measured
```

### Comparing `modelagnosticsafeaipackage-0.1.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt` & `modelagnosticsafeaipackage-0.2.0/modelagnosticsafeaipackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelagnosticsafeaipackage-0.1.0/setup.py` & `modelagnosticsafeaipackage-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 
 # Open README.md with UTF-8 encoding
 with open(this_directory / "README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '0.1.0'
-DESCRIPTION = 'SAFE AI package to measure risks of AI models'
+VERSION = '0.2.0'
+DESCRIPTION = 'MODEL AGNOSTIC SAFE AI package to measure risks of AI models WITHOUT CONSIDERING TYPE OF THE MODEL'
 
 # Setting up
 setup(
     name="modelagnosticsafeaipackage",
     version=VERSION,
     author="Golnoosh Babaei",
     author_email="<golnoosh.babaei93@gmail.com>",
```

