# Comparing `tmp/experiments_csv-0.5.3.tar.gz` & `tmp/experiments_csv-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiments_csv-0.5.3.tar", last modified: Sun Jul 23 14:15:28 2023, max compression
+gzip compressed data, was "experiments_csv-0.5.4.tar", last modified: Tue May 28 13:07:45 2024, max compression
```

## Comparing `experiments_csv-0.5.3.tar` & `experiments_csv-0.5.4.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 14:15:28.596269 experiments_csv-0.5.3/
-drwxrwxrwx   0        0        0        0 2023-07-23 14:15:28.586135 experiments_csv-0.5.3/.pytest_cache/
--rw-rw-rw-   0        0        0      310 2023-07-23 13:51:55.000000 experiments_csv-0.5.3/.pytest_cache/README.md
--rw-rw-rw-   0        0        0     1055 2022-05-24 07:51:17.000000 experiments_csv-0.5.3/LICENSE
--rw-rw-rw-   0        0        0      112 2022-05-24 07:51:17.000000 experiments_csv-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4189 2023-07-23 14:15:28.593263 experiments_csv-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     3566 2022-06-30 10:51:58.000000 experiments_csv-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 14:15:28.589256 experiments_csv-0.5.3/experiments_csv/
--rw-rw-rw-   0        0        0     8414 2022-07-04 14:17:36.000000 experiments_csv-0.5.3/experiments_csv/Experiment.py
--rw-rw-rw-   0        0        0        7 2023-07-23 14:13:09.000000 experiments_csv-0.5.3/experiments_csv/VERSION
--rw-rw-rw-   0        0        0      267 2022-07-05 07:42:29.000000 experiments_csv-0.5.3/experiments_csv/__init__.py
--rw-rw-rw-   0        0        0     1153 2022-05-24 07:51:17.000000 experiments_csv-0.5.3/experiments_csv/dict_product.py
--rw-rw-rw-   0        0        0     5398 2023-07-23 13:51:32.000000 experiments_csv-0.5.3/experiments_csv/dict_to_row.py
--rw-rw-rw-   0        0        0     8018 2023-07-23 14:12:53.000000 experiments_csv-0.5.3/experiments_csv/plot_results.py
-drwxrwxrwx   0        0        0        0 2023-07-23 14:15:28.593263 experiments_csv-0.5.3/experiments_csv.egg-info/
--rw-rw-rw-   0        0        0     4189 2023-07-23 14:15:28.000000 experiments_csv-0.5.3/experiments_csv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-07-23 14:15:28.000000 experiments_csv-0.5.3/experiments_csv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 14:15:28.000000 experiments_csv-0.5.3/experiments_csv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-23 14:15:28.000000 experiments_csv-0.5.3/experiments_csv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-23 14:15:28.000000 experiments_csv-0.5.3/experiments_csv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      302 2022-05-24 07:51:17.000000 experiments_csv-0.5.3/pyproject.toml
--rw-rw-rw-   0        0        0        8 2023-07-23 13:46:54.000000 experiments_csv-0.5.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 14:15:28.596269 experiments_csv-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1679 2022-07-12 07:42:16.000000 experiments_csv-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:07:45.211539 experiments_csv-0.5.4/
+-rw-rw-rw-   0        0        0     1055 2022-05-24 07:51:17.000000 experiments_csv-0.5.4/LICENSE
+-rw-rw-rw-   0        0        0      112 2022-05-24 07:51:17.000000 experiments_csv-0.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4274 2024-05-28 13:07:45.209538 experiments_csv-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3566 2022-06-30 10:51:58.000000 experiments_csv-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 13:07:45.163355 experiments_csv-0.5.4/experiments_csv/
+-rw-rw-rw-   0        0        0     8414 2022-07-04 14:17:36.000000 experiments_csv-0.5.4/experiments_csv/Experiment.py
+-rw-rw-rw-   0        0        0        7 2024-05-28 12:50:19.000000 experiments_csv-0.5.4/experiments_csv/VERSION
+-rw-rw-rw-   0        0        0      354 2024-05-28 12:52:00.000000 experiments_csv-0.5.4/experiments_csv/__init__.py
+-rw-rw-rw-   0        0        0     1153 2022-05-24 07:51:17.000000 experiments_csv-0.5.4/experiments_csv/dict_product.py
+-rw-rw-rw-   0        0        0     5398 2023-07-23 13:51:32.000000 experiments_csv-0.5.4/experiments_csv/dict_to_row.py
+-rw-rw-rw-   0        0        0     8018 2023-07-23 14:12:53.000000 experiments_csv-0.5.4/experiments_csv/plot_results.py
+drwxrwxrwx   0        0        0        0 2024-05-28 13:07:45.207532 experiments_csv-0.5.4/experiments_csv.egg-info/
+-rw-rw-rw-   0        0        0     4274 2024-05-28 13:07:45.000000 experiments_csv-0.5.4/experiments_csv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2024-05-28 13:07:45.000000 experiments_csv-0.5.4/experiments_csv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 13:07:45.000000 experiments_csv-0.5.4/experiments_csv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-28 13:07:45.000000 experiments_csv-0.5.4/experiments_csv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-28 13:07:45.000000 experiments_csv-0.5.4/experiments_csv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      302 2022-05-24 07:51:17.000000 experiments_csv-0.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0       15 2024-05-28 13:06:03.000000 experiments_csv-0.5.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 13:07:45.212207 experiments_csv-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1686 2024-05-28 13:06:12.000000 experiments_csv-0.5.4/setup.py
```

### Comparing `experiments_csv-0.5.3/LICENSE` & `experiments_csv-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `experiments_csv-0.5.3/PKG-INFO` & `experiments_csv-0.5.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: experiments_csv
-Version: 0.5.3
-Summary: Simple framework for running simulation experiments and recording them in a CSV file
-Home-page: https://github.com/erelsgl/experiments_csv
-Author: Erel Segal-Halevi
-Author-email: erelsgl@gmail.com
-License: MIT
-Project-URL: Bug Reports, https://github.com/erelsgl/experiments_csv/issues
-Project-URL: Source Code, https://github.com/erelsgl/experiments_csv
-Keywords: experiments
-Classifier: Development Status :: 2 - Pre-Alpha
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: plotting
-License-File: LICENSE
-
 # experiments_csv - experiment tracking via CSV files
 [![PyPI version](https://badge.fury.io/py/experiments_csv.svg)](https://badge.fury.io/py/experiments_csv)
 
 ## Motivation
 You run an experiments with various input parameters. You check various input combinations and run the experiment on each combination.
 
 Suddenly, during one of the runs, the program crashes. You have to restart the experiment for the current and future inputs, but you do not want to repeat it for all previous inputs.
@@ -106,8 +89,8 @@
 To plot the results, you can use the `plot_results` function, for example:
 
 ```
     from matplotlib import pyplot as plt
     experiments_csv.plot_results(plt, "results.csv", filter={"algorithm": "abc"}, xcolumn="size", ycolumn="runtime", zcolumn="bits")
 ```
 
-See the [demo programs](demo/) for usage examples.
+See the [demo programs](demo/) for usage examples.
```

### Comparing `experiments_csv-0.5.3/README.md` & `experiments_csv-0.5.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: experiments_csv
+Version: 0.5.4
+Summary: Simple framework for running simulation experiments and recording them in a CSV file
+Home-page: https://github.com/erelsgl/experiments_csv
+Author: Erel Segal-Halevi
+Author-email: erelsgl@gmail.com
+License: MIT
+Project-URL: Bug Reports, https://github.com/erelsgl/experiments_csv/issues
+Project-URL: Source Code, https://github.com/erelsgl/experiments_csv
+Keywords: experiments
+Classifier: Development Status :: 2 - Pre-Alpha
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas>=2.2.2
+Provides-Extra: plotting
+Requires-Dist: matplotlib>=3.9.0; extra == "plotting"
+
 # experiments_csv - experiment tracking via CSV files
 [![PyPI version](https://badge.fury.io/py/experiments_csv.svg)](https://badge.fury.io/py/experiments_csv)
 
 ## Motivation
 You run an experiments with various input parameters. You check various input combinations and run the experiment on each combination.
 
 Suddenly, during one of the runs, the program crashes. You have to restart the experiment for the current and future inputs, but you do not want to repeat it for all previous inputs.
@@ -89,8 +108,8 @@
 To plot the results, you can use the `plot_results` function, for example:
 
 ```
     from matplotlib import pyplot as plt
     experiments_csv.plot_results(plt, "results.csv", filter={"algorithm": "abc"}, xcolumn="size", ycolumn="runtime", zcolumn="bits")
 ```
 
-See the [demo programs](demo/) for usage examples.
+See the [demo programs](demo/) for usage examples.
```

### Comparing `experiments_csv-0.5.3/experiments_csv/Experiment.py` & `experiments_csv-0.5.4/experiments_csv/Experiment.py`

 * *Files identical despite different names*

### Comparing `experiments_csv-0.5.3/experiments_csv/dict_product.py` & `experiments_csv-0.5.4/experiments_csv/dict_product.py`

 * *Files identical despite different names*

### Comparing `experiments_csv-0.5.3/experiments_csv/dict_to_row.py` & `experiments_csv-0.5.4/experiments_csv/dict_to_row.py`

 * *Files identical despite different names*

### Comparing `experiments_csv-0.5.3/experiments_csv/plot_results.py` & `experiments_csv-0.5.4/experiments_csv/plot_results.py`

 * *Files identical despite different names*

### Comparing `experiments_csv-0.5.3/experiments_csv.egg-info/PKG-INFO` & `experiments_csv-0.5.4/experiments_csv.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
-Name: experiments-csv
-Version: 0.5.3
+Name: experiments_csv
+Version: 0.5.4
 Summary: Simple framework for running simulation experiments and recording them in a CSV file
 Home-page: https://github.com/erelsgl/experiments_csv
 Author: Erel Segal-Halevi
 Author-email: erelsgl@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/erelsgl/experiments_csv/issues
 Project-URL: Source Code, https://github.com/erelsgl/experiments_csv
 Keywords: experiments
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: plotting
 License-File: LICENSE
+Requires-Dist: pandas>=2.2.2
+Provides-Extra: plotting
+Requires-Dist: matplotlib>=3.9.0; extra == "plotting"
 
 # experiments_csv - experiment tracking via CSV files
 [![PyPI version](https://badge.fury.io/py/experiments_csv.svg)](https://badge.fury.io/py/experiments_csv)
 
 ## Motivation
 You run an experiments with various input parameters. You check various input combinations and run the experiment on each combination.
```

### Comparing `experiments_csv-0.5.3/setup.py` & `experiments_csv-0.5.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 setuptools.setup(
     name=NAME,
     packages=setuptools.find_packages(),
     version=VERSION,
     install_requires=REQUIRES,
     extras_require = {
-        "plotting": ["matplotlib"]
+        "plotting": ["matplotlib>=3.9.0"]
     },
     author="Erel Segal-Halevi",
     author_email="erelsgl@gmail.com",
     description="Simple framework for running simulation experiments and recording them in a CSV file",
     keywords="experiments",
     license="MIT",
     license_files=("LICENSE",),
```

