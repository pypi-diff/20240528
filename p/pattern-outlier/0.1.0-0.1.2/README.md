# Comparing `tmp/pattern_outlier-0.1.0.tar.gz` & `tmp/pattern_outlier-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pattern_outlier-0.1.0.tar", last modified: Sun May 26 23:01:04 2024, max compression
+gzip compressed data, was "pattern_outlier-0.1.2.tar", last modified: Tue May 28 21:53:18 2024, max compression
```

## Comparing `pattern_outlier-0.1.0.tar` & `pattern_outlier-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alexanderli   (501) staff       (20)        0 2024-05-26 23:01:04.896001 pattern_outlier-0.1.0/
--rw-r--r--   0 alexanderli   (501) staff       (20)    11324 2024-05-26 20:50:01.000000 pattern_outlier-0.1.0/LICENSE
--rw-r--r--   0 alexanderli   (501) staff       (20)      704 2024-05-26 23:01:04.895740 pattern_outlier-0.1.0/PKG-INFO
--rw-r--r--   0 alexanderli   (501) staff       (20)     3415 2024-05-26 21:25:55.000000 pattern_outlier-0.1.0/README.md
--rw-r--r--   0 alexanderli   (501) staff       (20)       38 2024-05-26 23:01:04.896052 pattern_outlier-0.1.0/setup.cfg
--rw-r--r--   0 alexanderli   (501) staff       (20)      909 2024-05-26 22:26:27.000000 pattern_outlier-0.1.0/setup.py
-drwxr-xr-x   0 alexanderli   (501) staff       (20)        0 2024-05-26 23:01:04.892177 pattern_outlier-0.1.0/src/
-drwxr-xr-x   0 alexanderli   (501) staff       (20)        0 2024-05-26 23:01:04.893727 pattern_outlier-0.1.0/src/pattern_outlier/
--rw-r--r--   0 alexanderli   (501) staff       (20)        0 2024-05-26 20:06:00.000000 pattern_outlier-0.1.0/src/pattern_outlier/__init__.py
--rw-r--r--   0 alexanderli   (501) staff       (20)      802 2024-05-26 20:07:31.000000 pattern_outlier-0.1.0/src/pattern_outlier/fpoff.py
--rw-r--r--   0 alexanderli   (501) staff       (20)      149 2024-05-26 20:07:52.000000 pattern_outlier-0.1.0/src/pattern_outlier/utils.py
-drwxr-xr-x   0 alexanderli   (501) staff       (20)        0 2024-05-26 23:01:04.895452 pattern_outlier-0.1.0/src/pattern_outlier.egg-info/
--rw-r--r--   0 alexanderli   (501) staff       (20)      704 2024-05-26 23:01:04.000000 pattern_outlier-0.1.0/src/pattern_outlier.egg-info/PKG-INFO
--rw-r--r--   0 alexanderli   (501) staff       (20)      350 2024-05-26 23:01:04.000000 pattern_outlier-0.1.0/src/pattern_outlier.egg-info/SOURCES.txt
--rw-r--r--   0 alexanderli   (501) staff       (20)        1 2024-05-26 23:01:04.000000 pattern_outlier-0.1.0/src/pattern_outlier.egg-info/dependency_links.txt
--rw-r--r--   0 alexanderli   (501) staff       (20)       15 2024-05-26 23:01:04.000000 pattern_outlier-0.1.0/src/pattern_outlier.egg-info/requires.txt
--rw-r--r--   0 alexanderli   (501) staff       (20)       16 2024-05-26 23:01:04.000000 pattern_outlier-0.1.0/src/pattern_outlier.egg-info/top_level.txt
-drwxr-xr-x   0 alexanderli   (501) staff       (20)        0 2024-05-26 23:01:04.895039 pattern_outlier-0.1.0/tests/
--rw-r--r--   0 alexanderli   (501) staff       (20)      962 2024-05-26 22:24:43.000000 pattern_outlier-0.1.0/tests/test_fpoff.py
+drwxr-xr-x   0 alexanderli   (501) staff       (20)        0 2024-05-28 21:53:18.855881 pattern_outlier-0.1.2/
+-rw-r--r--   0 alexanderli   (501) staff       (20)    11324 2024-05-26 20:50:01.000000 pattern_outlier-0.1.2/LICENSE
+-rw-r--r--   0 alexanderli   (501) staff       (20)      754 2024-05-28 21:53:18.855628 pattern_outlier-0.1.2/PKG-INFO
+-rw-r--r--   0 alexanderli   (501) staff       (20)     3726 2024-05-28 21:27:22.000000 pattern_outlier-0.1.2/README.md
+-rw-r--r--   0 alexanderli   (501) staff       (20)       38 2024-05-28 21:53:18.855936 pattern_outlier-0.1.2/setup.cfg
+-rw-r--r--   0 alexanderli   (501) staff       (20)      983 2024-05-28 21:53:11.000000 pattern_outlier-0.1.2/setup.py
+drwxr-xr-x   0 alexanderli   (501) staff       (20)        0 2024-05-28 21:53:18.852012 pattern_outlier-0.1.2/src/
+drwxr-xr-x   0 alexanderli   (501) staff       (20)        0 2024-05-28 21:53:18.853573 pattern_outlier-0.1.2/src/pattern_outlier/
+-rw-r--r--   0 alexanderli   (501) staff       (20)        0 2024-05-26 20:06:00.000000 pattern_outlier-0.1.2/src/pattern_outlier/__init__.py
+-rw-r--r--   0 alexanderli   (501) staff       (20)     2656 2024-05-28 21:09:56.000000 pattern_outlier-0.1.2/src/pattern_outlier/fpoff.py
+-rw-r--r--   0 alexanderli   (501) staff       (20)      149 2024-05-26 20:07:52.000000 pattern_outlier-0.1.2/src/pattern_outlier/utils.py
+drwxr-xr-x   0 alexanderli   (501) staff       (20)        0 2024-05-28 21:53:18.855323 pattern_outlier-0.1.2/src/pattern_outlier.egg-info/
+-rw-r--r--   0 alexanderli   (501) staff       (20)      754 2024-05-28 21:53:18.000000 pattern_outlier-0.1.2/src/pattern_outlier.egg-info/PKG-INFO
+-rw-r--r--   0 alexanderli   (501) staff       (20)      350 2024-05-28 21:53:18.000000 pattern_outlier-0.1.2/src/pattern_outlier.egg-info/SOURCES.txt
+-rw-r--r--   0 alexanderli   (501) staff       (20)        1 2024-05-28 21:53:18.000000 pattern_outlier-0.1.2/src/pattern_outlier.egg-info/dependency_links.txt
+-rw-r--r--   0 alexanderli   (501) staff       (20)       35 2024-05-28 21:53:18.000000 pattern_outlier-0.1.2/src/pattern_outlier.egg-info/requires.txt
+-rw-r--r--   0 alexanderli   (501) staff       (20)       16 2024-05-28 21:53:18.000000 pattern_outlier-0.1.2/src/pattern_outlier.egg-info/top_level.txt
+drwxr-xr-x   0 alexanderli   (501) staff       (20)        0 2024-05-28 21:53:18.854634 pattern_outlier-0.1.2/tests/
+-rw-r--r--   0 alexanderli   (501) staff       (20)     2176 2024-05-28 21:36:32.000000 pattern_outlier-0.1.2/tests/test_fpoff.py
```

### Comparing `pattern_outlier-0.1.0/LICENSE` & `pattern_outlier-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pattern_outlier-0.1.0/README.md` & `pattern_outlier-0.1.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,103 @@
 # Pattern-Outlier
 
-Pattern-Outlier is a Python library for detecting outliers based on frequent pattern mining, inspired by the `fpmoutliers` R package.
+Pattern-Outlier is a Python library for detecting outliers based on frequent pattern mining, inspired by the `fpmoutliers` R package. The package supports multiple algorithms and allows users to dynamically calculate the most reasonable threshold and support parameters.
+
+
+
+## Features
+- **Support for Multiple Algorithms**: Choose from FPI, WFPI, FPOF, and FPCOF methods for outlier detection.
+- **Dynamic Parameter Calculation**: Automatically find the best support and threshold parameters.
+- **Model Persistence**: Save and load fitted models for reuse.
+- **Flexible Input Handling**: Accepts transaction data in list format.
+- **Easy to Use API**: Simple and intuitive interface for fitting models and predicting outliers.
+
 
 ## License
 
 This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.
 
-## Acknowledgments
 
-This project is based on the `fpmoutliers` R package by Jaroslav Kuchar and Vojtěch Svátek. Original R package can be found [here](https://github.com/jaroslav-kuchar/fpmoutliers).
+## Project on PyPI
+
+You can find this project on PyPI at the following link:
+[Pattern-Outlier on PyPI](https://pypi.org/project/pattern-outlier/)
+
 
 ## Installation
 
 ```bash
 pip install -r requirements.txt
 ```
 
-## Example Usage
-
-```python
-import pandas as pd
-from src.pattern_outlier.fpoff import FPOF
-
-# Create some dummy data
-data = {
-    'Bread': [1, 1, 0, 1, 0, 0, 1, 1, 0, 0],
-    'Milk': [1, 0, 1, 1, 1, 1, 1, 0, 1, 0],
-    'Diapers': [0, 1, 1, 1, 1, 0, 1, 1, 1, 1],
-    'Beer': [0, 1, 1, 1, 0, 1, 0, 1, 0, 1],
-    'Eggs': [1, 0, 0, 1, 0, 1, 0, 1, 0, 0]
-}
-
-df = pd.DataFrame(data)
-
-# Convert the data to boolean types as recommended
-df = df.astype(bool)
-
-# Initialize and fit the FPOF model
-fpof = FPOF(min_support=0.3)
-fpof.fit(df)
-
-# Score the data
-scores = fpof.score(df)
-df['outlier_score'] = scores
-
-# Predict outliers
-threshold = 2
-predictions = fpof.predict(df, threshold)
-df['outlier'] = predictions
-
-# Print the results
-print("DataFrame with Outlier Scores and Predictions:")
-print(df)
-
-```
 
 ## How to Contribute
 
 Contributions from the community are welcome! Here are some guidelines to help you get started:
 
+
 ### Reporting Bugs
 
 If you find a bug, please report it by opening an issue on the [GitHub repository](https://github.com/lihangalex/pattern-outlier/issues). Include as much detail as possible, such as steps to reproduce the bug, the expected behavior, and screenshots if applicable.
 
+
 ### Suggesting Features
 
 If you have an idea for a new feature, please open an issue on the [GitHub repository](https://github.com/lihangalex/pattern-outlier/issues) and describe your idea in detail. Explain why it would be useful and how it should work.
 
+
 ### Submitting Pull Requests
 
 If you'd like to contribute code, please follow these steps:
 
 1. **Fork the repository**: Click the "Fork" button at the top of the repository page on GitHub.
+
 2. **Clone your fork**: Clone your forked repository to your local machine.
    ```bash
    git clone https://github.com/lihangalex/pattern-outlier.git
    cd pattern-outlier
    ```
+
 3. **Create a branch**: Create a new branch for your work.
    ```bash
    git checkout -b feature-branch
    ```
+
+
 4. **Make your changes**: Make your changes to the codebase.
+
 5. **Commit your changes**: Commit your changes with a clear and concise commit message.
     ```bash
     git add .
     git commit -m "Add feature or fix bug"
     ```
+
 6. ***Push your changes***: Push your changes to your forked repository.
    ```bash
    git push origin feature-branch
    ```
+
 7. **Open a pull request**: Go to the original repository and open a pull request from your forked repository. Provide a clear description of your changes and any relevant information.
 
+
 ### Code Style and Guidelines
 
 - Follow the existing code style and conventions used in the project.
 - Write clear, concise, and descriptive commit messages.
 - Include comments and docstrings to explain your code where necessary.
 - Ensure your changes do not break existing tests and write new tests if applicable.
 
+
 ### Running Tests
 
 To run the tests locally, use the following command:
 
 ```bash
 pytest
-```
+```
+
+## References
+- He, Z., Xu, X., Huang, J. Z., Deng, S.: FP-Outlier: Frequent Pattern Based Outlier Detection. Computer Science and Information Systems, Vol. 2, No. 1, 103-118. (2005).
+
+- Tang, X., Li, G., Chen, G.: Fast Detecting Outliers over Online Data Streams. 2009 International Conference on Information Engineering and Computer Science, Wuhan, 2009, pp. 1-4.
+
+- Kuchar, J., Svatek, V.: Spotlighting Anomalies using Frequent Patterns. Proceedings of the KDD 2017 Workshop on Anomaly Detection in Finance, Halifax, Nova Scotia, Canada, PMLR, 2017.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pattern_outlier-0.1.0/setup.py` & `pattern_outlier-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pattern-outlier',
-    version='0.1.0',
+    version='0.1.2',  # Increment the version number
     description='A Python library for detecting outliers based on frequent pattern mining.',
     author='Alexander Li',
     author_email='lihangalex@pm.me',
     url='https://github.com/lihangalex/pattern-outlier',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'pandas',
         'mlxtend',
+        'scikit-learn',
+        'joblib',
     ],
     tests_require=[
         'pytest',
     ],
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

