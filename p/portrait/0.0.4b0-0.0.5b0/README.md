# Comparing `tmp/portrait-0.0.4b0.tar.gz` & `tmp/portrait-0.0.5b0.tar.gz`

## Comparing `portrait-0.0.4b0.tar` & `portrait-0.0.5b0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 portrait-0.0.4b0/.readthedocs.yaml
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 portrait-0.0.4b0/CITATION.cff
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 portrait-0.0.4b0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 portrait-0.0.4b0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 portrait-0.0.4b0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 portrait-0.0.4b0/.vscode/settings.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 portrait-0.0.4b0/docs/Makefile
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 portrait-0.0.4b0/docs/acknowledgement.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 portrait-0.0.4b0/docs/api.rst
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 portrait-0.0.4b0/docs/conf.py
--rw-r--r--   0        0        0    48344 2020-02-02 00:00:00.000000 portrait-0.0.4b0/docs/coverage.ipynb
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 portrait-0.0.4b0/docs/index.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 portrait-0.0.4b0/docs/installation.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 portrait-0.0.4b0/docs/make.bat
--rw-r--r--   0        0        0    23560 2020-02-02 00:00:00.000000 portrait-0.0.4b0/docs/periodmatch.ipynb
--rw-r--r--   0        0        0   124424 2020-02-02 00:00:00.000000 portrait-0.0.4b0/docs/tess.ipynb
--rw-r--r--   0        0        0    18599 2020-02-02 00:00:00.000000 portrait-0.0.4b0/docs/_static/portrait.png
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 portrait-0.0.4b0/portrait/__init__.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 portrait-0.0.4b0/portrait/core.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 portrait-0.0.4b0/tests/test_all.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 portrait-0.0.4b0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 portrait-0.0.4b0/LICENSE
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 portrait-0.0.4b0/README.md
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 portrait-0.0.4b0/pyproject.toml
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 portrait-0.0.4b0/PKG-INFO
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 portrait-0.0.5b0/.readthedocs.yaml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 portrait-0.0.5b0/CITATION.cff
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 portrait-0.0.5b0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 portrait-0.0.5b0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 portrait-0.0.5b0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 portrait-0.0.5b0/.vscode/settings.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 portrait-0.0.5b0/docs/Makefile
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 portrait-0.0.5b0/docs/acknowledgement.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 portrait-0.0.5b0/docs/api.rst
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 portrait-0.0.5b0/docs/conf.py
+-rw-r--r--   0        0        0    48344 2020-02-02 00:00:00.000000 portrait-0.0.5b0/docs/coverage.ipynb
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 portrait-0.0.5b0/docs/index.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 portrait-0.0.5b0/docs/installation.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 portrait-0.0.5b0/docs/make.bat
+-rw-r--r--   0        0        0    23560 2020-02-02 00:00:00.000000 portrait-0.0.5b0/docs/periodmatch.ipynb
+-rw-r--r--   0        0        0   124424 2020-02-02 00:00:00.000000 portrait-0.0.5b0/docs/tess.ipynb
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 portrait-0.0.5b0/docs/_static/icon.png
+-rw-r--r--   0        0        0    15029 2020-02-02 00:00:00.000000 portrait-0.0.5b0/docs/_static/portrait.png
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 portrait-0.0.5b0/portrait/__init__.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 portrait-0.0.5b0/portrait/core.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 portrait-0.0.5b0/tests/test_all.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 portrait-0.0.5b0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 portrait-0.0.5b0/LICENSE
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 portrait-0.0.5b0/README.md
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 portrait-0.0.5b0/pyproject.toml
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 portrait-0.0.5b0/PKG-INFO
```

### Comparing `portrait-0.0.4b0/CITATION.cff` & `portrait-0.0.5b0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/CODE_OF_CONDUCT.md` & `portrait-0.0.5b0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/CONTRIBUTING.md` & `portrait-0.0.5b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/.github/workflows/ci.yaml` & `portrait-0.0.5b0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/docs/Makefile` & `portrait-0.0.5b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/docs/conf.py` & `portrait-0.0.5b0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "portrait"
 copyright = "2023, Lionel Garcia"
 author = "Lionel Garcia"
 release = "0.0.1"
 html_logo = "_static/portrait.png"
+html_favicon = "_static/icon.png"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `portrait-0.0.4b0/docs/coverage.ipynb` & `portrait-0.0.5b0/docs/coverage.ipynb`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/docs/index.md` & `portrait-0.0.5b0/docs/index.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-# portrait
+# *portrait*
+
+Observation metrics for periodic events
+
+---
 
 A Python package to compute and visualize observation metrics for periodic events. In Astronomy, *portrait* is useful to answer the following questions:
 - How much of an orbit with period $P$ has been observed given certain observation times? ([tutorial](coverage))
 - What period $P$ matches with this list of events? ([tutorial](periodmatch))
 - How a certain target must be observed to cover all orbits with periods lower than $P$ days? 
 
 ## Table of content
```

### Comparing `portrait-0.0.4b0/docs/make.bat` & `portrait-0.0.5b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/docs/periodmatch.ipynb` & `portrait-0.0.5b0/docs/periodmatch.ipynb`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/docs/tess.ipynb` & `portrait-0.0.5b0/docs/tess.ipynb`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/portrait/__init__.py` & `portrait-0.0.5b0/portrait/__init__.py`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/portrait/core.py` & `portrait-0.0.5b0/portrait/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,25 +55,30 @@
 
         # segments_phases is unordered, some of them are
         # (0.6, 0.5) which corresponds to a segment that wraps around
         # the phase 1.0. We need to fix this and split it in (0.0, 0.5) and (0.6, 1.0)
         # we allocate segments_phases_2 for the extra split, as JAX requires fixed size arrays
         #
         # cases:
-        # - ||   0-----1 || -> |-----|
+        # - |   0-----1 |
         #
-        # - ||-----1  0--|| -> |-----|, |--|
+        # - |        0--+
+        #   +-----1     |
         #
-        # - ||--1
-        #    +-----------+
-        #           0----|| -> |--|, |-----------|, |----|
+        # - |--1
+        #    +----------+
+        #           0---|
         #
-        # - ||  0--------+
-        #    +-----------+
-        #    +-----1    || -> |--------|, |-----------|, |----|
+        # - |  0--------+
+        #   +-----------+
+        #   +------1    |
+        #
+        # | : bounds of full phase segment
+        # 0, 1 : start, end of the actual segment
+        # + : wrap around the phase 1.0
 
         n = raw_segments_phases.shape[0]
 
         full = jnp.floor((segments_times[:, 1] - segments_times[:, 0]) / period)
         is_positive = jnp.array(raw_segments_phases[:, 1] >= raw_segments_phases[:, 0])
         is_full = full > 0
```

### Comparing `portrait-0.0.4b0/tests/test_all.py` & `portrait-0.0.5b0/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/LICENSE` & `portrait-0.0.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/README.md` & `portrait-0.0.5b0/README.md`

 * *Files identical despite different names*

### Comparing `portrait-0.0.4b0/pyproject.toml` & `portrait-0.0.5b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "portrait"
-version = "0.0.4-beta"
+version = "0.0.5-beta"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "Lionel Garcia" }]
 description = "Compute and visualize observations phase coverage"
 readme = "README.md"
 keywords = ["jax", "astronomy", "image processing"]
 classifiers = [
```

### Comparing `portrait-0.0.4b0/PKG-INFO` & `portrait-0.0.5b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: portrait
-Version: 0.0.4b0
+Version: 0.0.5b0
 Summary: Compute and visualize observations phase coverage
 Author: Lionel Garcia
 License-Expression: MIT
 License-File: LICENSE
 Keywords: astronomy,image processing,jax
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: portrait Version: 0.0.4b0 Summary: Compute and
+Metadata-Version: 2.3 Name: portrait Version: 0.0.5b0 Summary: Compute and
 visualize observations phase coverage Author: Lionel Garcia License-Expression:
 MIT License-File: LICENSE Keywords: astronomy,image processing,jax Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
 Requires-Dist: jax>=0.2.25 Requires-Dist: jaxlib Requires-Dist: numpy>=1.23.5
 Provides-Extra: dev Requires-Dist: black; extra == 'dev' Requires-Dist: isort;
 extra == 'dev' Requires-Dist: pytest; extra == 'dev' Provides-Extra: docs
```

