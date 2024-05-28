# Comparing `tmp/felimination-0.2.2.tar.gz` & `tmp/felimination-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felimination-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "felimination-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `felimination-0.2.2.tar` & `felimination-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2167 2024-01-15 12:37:00.610675 felimination-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-01-15 12:37:00.610675 felimination-0.2.2/felimination/__init__.py
--rw-r--r--   0        0        0    27098 2024-01-15 12:37:00.610675 felimination-0.2.2/felimination/drift.py
--rw-r--r--   0        0        0     3863 2024-01-15 12:37:00.614675 felimination-0.2.2/felimination/importance.py
--rw-r--r--   0        0        0    32100 2024-01-15 12:37:00.614675 felimination-0.2.2/felimination/rfe.py
--rw-r--r--   0        0        0      249 2024-01-15 12:37:00.614675 felimination-0.2.2/felimination/utils/parallel.py
--rw-r--r--   0        0        0     1413 2024-01-15 12:37:00.614675 felimination-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 felimination-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2167 2024-05-28 09:29:44.409719 felimination-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 09:29:44.413719 felimination-0.2.3/felimination/__init__.py
+-rw-r--r--   0        0        0    27099 2024-05-28 09:29:44.413719 felimination-0.2.3/felimination/drift.py
+-rw-r--r--   0        0        0     3863 2024-05-28 09:29:44.413719 felimination-0.2.3/felimination/importance.py
+-rw-r--r--   0        0        0    32139 2024-05-28 09:29:44.413719 felimination-0.2.3/felimination/rfe.py
+-rw-r--r--   0        0        0      249 2024-05-28 09:29:44.413719 felimination-0.2.3/felimination/utils/parallel.py
+-rw-r--r--   0        0        0     1413 2024-05-28 09:29:44.413719 felimination-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 felimination-0.2.3/PKG-INFO
```

### Comparing `felimination-0.2.2/README.md` & `felimination-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `felimination-0.2.2/felimination/drift.py` & `felimination-0.2.3/felimination/drift.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 able anymore to distinguish between the two samples, or until a certain amount
 of features has been removed.
 
 This module contains the following classes:
 - `SampleSimilarityDriftRFE`: base class for drift-based sample similarity
     feature selection.
 """
+
 from collections import defaultdict
 from numbers import Integral
 
 import numpy as np
 from joblib import effective_n_jobs
 from sklearn.base import ClassifierMixin, clone
 from sklearn.metrics import check_scoring
```

### Comparing `felimination-0.2.2/felimination/importance.py` & `felimination-0.2.3/felimination/importance.py`

 * *Files identical despite different names*

### Comparing `felimination-0.2.2/felimination/rfe.py` & `felimination-0.2.3/felimination/rfe.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 This module contains the following classes:
 
 - `FeliminationRFECV`: base class for feature selection.
 - `PermutationImportanceRFECV`: recursive feature elimination with
     cross-validation based on permutation importance.
 """
+
 from collections import defaultdict
 from inspect import signature
 from numbers import Integral
 from operator import attrgetter
 
 import numpy as np
 import pandas as pd
@@ -63,16 +64,16 @@
         The features importances.
     """
 
     estimator = clone(estimator)
     X_train, y_train = _safe_split(estimator, X, y, train)
     X_test, y_test = _safe_split(estimator, X, y, test, train)
     estimator = estimator.fit(X_train, y_train)
-    train_score = _score(estimator, X_train, y_train, scorer)
-    test_score = _score(estimator, X_test, y_test, scorer)
+    train_score = _score(estimator, X_train, y_train, scorer, score_params=None)
+    test_score = _score(estimator, X_test, y_test, scorer, score_params=None)
     importances = _get_feature_importances(
         estimator, importance_getter, X=X_test, y=y_test
     )
     return train_score, test_score, importances
 
 
 def _get_feature_importances(
```

### Comparing `felimination-0.2.2/pyproject.toml` & `felimination-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "felimination"
 description = "This library contains some useful scikit-learn compatible classes for feature selection."
-version = "0.2.2"
+version = "0.2.3"
 keywords = ["feature selection", "scikit-learn", "machine learning"]
 authors = [
     { name = "Claudio Salvatore Arcidiacono", email = "author@email.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "scikit-learn>=1.0.1,<2.0.0",
+    "scikit-learn>=1.4.0,<2.0.0",
     "pandas>=1.1.1,<3.0.0",
     "seaborn>=0.11.1,<1.0.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
```

### Comparing `felimination-0.2.2/PKG-INFO` & `felimination-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: felimination
-Version: 0.2.2
+Version: 0.2.3
 Summary: This library contains some useful scikit-learn compatible classes for feature selection.
 Keywords: feature selection,scikit-learn,machine learning
 Author-email: Claudio Salvatore Arcidiacono <author@email.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Dist: scikit-learn>=1.0.1,<2.0.0
+Requires-Dist: scikit-learn>=1.4.0,<2.0.0
 Requires-Dist: pandas>=1.1.1,<3.0.0
 Requires-Dist: seaborn>=0.11.1,<1.0.0
 Requires-Dist: build ; extra == "build"
 Requires-Dist: twine ; extra == "build"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: flake8-pyproject ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
```

