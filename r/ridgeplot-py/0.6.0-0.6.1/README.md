# Comparing `tmp/ridgeplot_py-0.6.0.tar.gz` & `tmp/ridgeplot_py-0.6.1.tar.gz`

## Comparing `ridgeplot_py-0.6.0.tar` & `ridgeplot_py-0.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    63867 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/Example.ipynb
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/mkdocs.yml
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/requirements-dev.lock
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/requirements.lock
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/docs/colors.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/docs/dotted_heatmap.md
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/docs/index.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/docs/ridge_plot.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/docs/stats.md
--rw-r--r--   0        0        0    21909 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/img/ridgeplot.png
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/src/ridgeplot/__init__.py
--rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/src/ridgeplot/colors.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/src/ridgeplot/dotted_heatmap.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/src/ridgeplot/ridge_plot.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/src/ridgeplot/stats.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/test/test_colors.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/test/test_dotted_heatmap.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/test/test_ridge_plot.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/test/test_stats.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/LICENSE
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/README.md
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    63867 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/Example.ipynb
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/mkdocs.yml
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/requirements-dev.lock
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/requirements.lock
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/docs/colors.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/docs/dotted_heatmap.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/docs/index.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/docs/ridge_plot.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/docs/stats.md
+-rw-r--r--   0        0        0    21909 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/img/ridgeplot.png
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/src/ridgeplot/__init__.py
+-rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/src/ridgeplot/colors.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/src/ridgeplot/dotted_heatmap.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/src/ridgeplot/ridge_plot.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/src/ridgeplot/stats.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/test/test_colors.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/test/test_dotted_heatmap.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/test/test_ridge_plot.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/test/test_stats.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/README.md
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 ridgeplot_py-0.6.1/PKG-INFO
```

### Comparing `ridgeplot_py-0.6.0/Example.ipynb` & `ridgeplot_py-0.6.1/Example.ipynb`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/requirements-dev.lock` & `ridgeplot_py-0.6.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/requirements.lock` & `ridgeplot_py-0.6.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/.github/workflows/ci.yaml` & `ridgeplot_py-0.6.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/docs/index.md` & `ridgeplot_py-0.6.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/img/ridgeplot.png` & `ridgeplot_py-0.6.1/img/ridgeplot.png`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/src/ridgeplot/colors.py` & `ridgeplot_py-0.6.1/src/ridgeplot/colors.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/src/ridgeplot/dotted_heatmap.py` & `ridgeplot_py-0.6.1/src/ridgeplot/dotted_heatmap.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/src/ridgeplot/ridge_plot.py` & `ridgeplot_py-0.6.1/src/ridgeplot/ridge_plot.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/src/ridgeplot/stats.py` & `ridgeplot_py-0.6.1/src/ridgeplot/stats.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/test/test_colors.py` & `ridgeplot_py-0.6.1/test/test_colors.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/test/test_ridge_plot.py` & `ridgeplot_py-0.6.1/test/test_ridge_plot.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/test/test_stats.py` & `ridgeplot_py-0.6.1/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/LICENSE` & `ridgeplot_py-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/README.md` & `ridgeplot_py-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.6.0/pyproject.toml` & `ridgeplot_py-0.6.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 
 [tool.hatch.version]
 source = "versioningit"
 
 [tool.versioningit]
 default-version = "0.0.0+unknown"
 
+[tool.versioningit.next-version]
+method = "smallest"
+
 [tool.versioningit.format]
 distance = "{next_version}"
 dirty = "{version}+dirty"
 distance-dirty = "{next_version}.dev{distance}+{vcs}{rev}.dirty"
 
 [tool.mypy]
 plugins = "numpy.typing.mypy_plugin"
```

### Comparing `ridgeplot_py-0.6.0/PKG-INFO` & `ridgeplot_py-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ridgeplot-py
-Version: 0.6.0
+Version: 0.6.1
 Summary: Plotting ridgeplots with matplotlib
 Author-email: Douglas Wu <wckdouglas@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: matplotlib>=3.8
 Requires-Dist: more-itertools>=8.9.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: ridgeplot-py Version: 0.6.0 Summary: Plotting
+Metadata-Version: 2.3 Name: ridgeplot-py Version: 0.6.1 Summary: Plotting
 ridgeplots with matplotlib Author-email: Douglas Wu
 gmail.com> License-Expression: MIT License-File: LICENSE Requires-Python: >=3.9
 Requires-Dist: matplotlib>=3.8 Requires-Dist: more-itertools>=8.9.0 Requires-
 Dist: numpy>=1.21.1 Requires-Dist: pandas>=2.2.2 Requires-Dist: scipy>=1.8.0
 Description-Content-Type: text/markdown # ridgeplot-py # [![CI](https://
 github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https:
 //github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov]
```

