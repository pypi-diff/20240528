# Comparing `tmp/wcosmo-0.0.0.tar.gz` & `tmp/wcosmo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcosmo-0.0.0.tar", last modified: Tue May 28 18:31:55 2024, max compression
+gzip compressed data, was "wcosmo-0.1.1.tar", last modified: Tue May 28 19:03:35 2024, max compression
```

## Comparing `wcosmo-0.0.0.tar` & `wcosmo-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:31:55.963468 wcosmo-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:31:55.955469 wcosmo-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:31:55.959468 wcosmo-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-28 18:31:51.000000 wcosmo-0.0.0/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-28 18:31:51.000000 wcosmo-0.0.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 18:31:51.000000 wcosmo-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 18:31:51.000000 wcosmo-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-28 18:31:55.963468 wcosmo-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-28 18:31:51.000000 wcosmo-0.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:31:55.959468 wcosmo-0.0.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 18:31:51.000000 wcosmo-0.0.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 18:31:51.000000 wcosmo-0.0.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 18:31:51.000000 wcosmo-0.0.0/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 18:31:51.000000 wcosmo-0.0.0/doc/pages_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:31:55.959468 wcosmo-0.0.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:31:55.959468 wcosmo-0.0.0/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-28 18:31:51.000000 wcosmo-0.0.0/doc/source/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-28 18:31:51.000000 wcosmo-0.0.0/doc/source/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-28 18:31:51.000000 wcosmo-0.0.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-28 18:31:51.000000 wcosmo-0.0.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-28 18:31:51.000000 wcosmo-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:31:55.963468 wcosmo-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:31:51.000000 wcosmo-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:31:55.959468 wcosmo-0.0.0/wcosmo/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 18:31:51.000000 wcosmo-0.0.0/wcosmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-28 18:31:51.000000 wcosmo-0.0.0/wcosmo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-05-28 18:31:51.000000 wcosmo-0.0.0/wcosmo/wcosmo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:31:55.963468 wcosmo-0.0.0/wcosmo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-28 18:31:55.000000 wcosmo-0.0.0/wcosmo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-28 18:31:55.000000 wcosmo-0.0.0/wcosmo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:31:55.000000 wcosmo-0.0.0/wcosmo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-28 18:31:55.000000 wcosmo-0.0.0/wcosmo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 18:31:55.000000 wcosmo-0.0.0/wcosmo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 18:31:55.000000 wcosmo-0.0.0/wcosmo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:35.283499 wcosmo-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:35.279499 wcosmo-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:35.279499 wcosmo-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-28 19:03:31.000000 wcosmo-0.1.1/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-28 19:03:31.000000 wcosmo-0.1.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 19:03:31.000000 wcosmo-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 19:03:31.000000 wcosmo-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-28 19:03:35.283499 wcosmo-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-28 19:03:31.000000 wcosmo-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:35.283499 wcosmo-0.1.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 19:03:31.000000 wcosmo-0.1.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 19:03:31.000000 wcosmo-0.1.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 19:03:31.000000 wcosmo-0.1.1/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 19:03:31.000000 wcosmo-0.1.1/doc/pages_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:35.283499 wcosmo-0.1.1/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:35.283499 wcosmo-0.1.1/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-28 19:03:31.000000 wcosmo-0.1.1/doc/source/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-28 19:03:31.000000 wcosmo-0.1.1/doc/source/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-28 19:03:31.000000 wcosmo-0.1.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-28 19:03:31.000000 wcosmo-0.1.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-28 19:03:31.000000 wcosmo-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 19:03:35.283499 wcosmo-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 19:03:31.000000 wcosmo-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:35.283499 wcosmo-0.1.1/wcosmo/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 19:03:31.000000 wcosmo-0.1.1/wcosmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 19:03:35.000000 wcosmo-0.1.1/wcosmo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-28 19:03:31.000000 wcosmo-0.1.1/wcosmo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-05-28 19:03:31.000000 wcosmo-0.1.1/wcosmo/wcosmo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:35.283499 wcosmo-0.1.1/wcosmo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-28 19:03:35.000000 wcosmo-0.1.1/wcosmo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-28 19:03:35.000000 wcosmo-0.1.1/wcosmo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:03:35.000000 wcosmo-0.1.1/wcosmo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-28 19:03:35.000000 wcosmo-0.1.1/wcosmo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 19:03:35.000000 wcosmo-0.1.1/wcosmo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 19:03:35.000000 wcosmo-0.1.1/wcosmo.egg-info/top_level.txt
```

### Comparing `wcosmo-0.0.0/.github/workflows/pages.yml` & `wcosmo-0.1.1/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `wcosmo-0.0.0/.github/workflows/release.yaml` & `wcosmo-0.1.1/.github/workflows/release.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
       - name: build release distributions
         run: |
-          python -m pip install build
+          python -m pip install build setuptools_scm
           python -m build --sdist --wheel --outdir dist/ .
       - name: upload wheel and tarball
         uses: actions/upload-artifact@v4
         with:
           name: release-dists
           path: dist/
```

### Comparing `wcosmo-0.0.0/LICENSE` & `wcosmo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wcosmo-0.0.0/PKG-INFO` & `wcosmo-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcosmo
-Version: 0.0.0
+Version: 0.1.1
 Summary: A package for cosmology calculations with arbitrary numpy-like APIs
 Author: Amanda Farah
 Author-email: Colm Talbot <talbotcolm@gmail.com>
 License: MIT
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `wcosmo-0.0.0/README.rst` & `wcosmo-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `wcosmo-0.0.0/doc/Makefile` & `wcosmo-0.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `wcosmo-0.0.0/doc/make.bat` & `wcosmo-0.1.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `wcosmo-0.0.0/doc/source/_templates/custom-class-template.rst` & `wcosmo-0.1.1/doc/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `wcosmo-0.0.0/doc/source/_templates/custom-module-template.rst` & `wcosmo-0.1.1/doc/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `wcosmo-0.0.0/doc/source/conf.py` & `wcosmo-0.1.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `wcosmo-0.0.0/pyproject.toml` & `wcosmo-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,13 +21,16 @@
     "numpy"
 ]
 dynamic = ["version"]
 
 [tool.setuptools]
 packages = ["wcosmo"]
 
+[tool.setuptools_scm]
+write_to = "wcosmo/_version.py"
+
 [project.entry-points."gwpopulation.xp"]
 wcosmo = "wcosmo.wcosmo"
 wcosmo-utils = "wcosmo.utils"
 
 [project.entry-points."gwpopulation.other"]
 wcosmo-utils = "wcosmo.utils:scipy.linalg.toeplitz"
```

### Comparing `wcosmo-0.0.0/wcosmo/utils.py` & `wcosmo-0.1.1/wcosmo/utils.py`

 * *Files identical despite different names*

### Comparing `wcosmo-0.0.0/wcosmo/wcosmo.py` & `wcosmo-0.1.1/wcosmo/wcosmo.py`

 * *Files identical despite different names*

### Comparing `wcosmo-0.0.0/wcosmo.egg-info/PKG-INFO` & `wcosmo-0.1.1/wcosmo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcosmo
-Version: 0.0.0
+Version: 0.1.1
 Summary: A package for cosmology calculations with arbitrary numpy-like APIs
 Author: Amanda Farah
 Author-email: Colm Talbot <talbotcolm@gmail.com>
 License: MIT
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `wcosmo-0.0.0/wcosmo.egg-info/SOURCES.txt` & `wcosmo-0.1.1/wcosmo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 doc/make.bat
 doc/pages_requirements.txt
 doc/source/conf.py
 doc/source/index.rst
 doc/source/_templates/custom-class-template.rst
 doc/source/_templates/custom-module-template.rst
 wcosmo/__init__.py
+wcosmo/_version.py
 wcosmo/utils.py
 wcosmo/wcosmo.py
 wcosmo.egg-info/PKG-INFO
 wcosmo.egg-info/SOURCES.txt
 wcosmo.egg-info/dependency_links.txt
 wcosmo.egg-info/entry_points.txt
 wcosmo.egg-info/requires.txt
```

