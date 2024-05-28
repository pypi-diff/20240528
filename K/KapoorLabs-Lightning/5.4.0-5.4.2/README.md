# Comparing `tmp/kapoorlabs_lightning-5.4.0.tar.gz` & `tmp/kapoorlabs_lightning-5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kapoorlabs_lightning-5.4.0.tar", last modified: Sun May 26 15:13:18 2024, max compression
+gzip compressed data, was "kapoorlabs_lightning-5.4.2.tar", last modified: Tue May 28 19:13:24 2024, max compression
```

## Comparing `kapoorlabs_lightning-5.4.0.tar` & `kapoorlabs_lightning-5.4.2.tar`

### file list

```diff
@@ -1,49 +1,45 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.369069 kapoorlabs_lightning-5.4.0/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.357069 kapoorlabs_lightning-5.4.0/.github/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.361069 kapoorlabs_lightning-5.4.0/.github/workflows/
--rw-r--r--   0 debian    (1000) debian    (1000)     1068 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/.github/workflows/deploy.yml
--rw-r--r--   0 debian    (1000) debian    (1000)     1963 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 debian    (1000) debian    (1000)      991 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/.gitignore
--rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/.pre-commit-config.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/LICENSE
--rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/MANIFEST.in
--rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-26 15:13:18.369069 kapoorlabs_lightning-5.4.0/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     2435 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/README.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.361069 kapoorlabs_lightning-5.4.0/licenses/
--rw-r--r--   0 debian    (1000) debian    (1000)    11358 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/licenses/Apache-2
--rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/licenses/BSD-3
--rw-r--r--   0 debian    (1000) debian    (1000)    35148 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/licenses/GPL-3
--rw-r--r--   0 debian    (1000) debian    (1000)     7653 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/licenses/LGPL-3
--rw-r--r--   0 debian    (1000) debian    (1000)     1080 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/licenses/MIT
--rw-r--r--   0 debian    (1000) debian    (1000)    16726 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/licenses/MPL-2
--rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/pyproject.toml
--rw-r--r--   0 debian    (1000) debian    (1000)     1766 2024-05-26 15:13:18.369069 kapoorlabs_lightning-5.4.0/setup.cfg
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.357069 kapoorlabs_lightning-5.4.0/src/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.365069 kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-26 15:13:18.000000 kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     1269 2024-05-26 15:13:18.000000 kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-05-26 15:13:18.000000 kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)      102 2024-05-26 15:13:18.000000 kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/requires.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       21 2024-05-26 15:13:18.000000 kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/top_level.txt
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.365069 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/
--rw-r--r--   0 debian    (1000) debian    (1000)     1603 2024-05-17 14:55:57.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.365069 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/_tests/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/_tests/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3106 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
--rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-05-25 17:21:15.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/_version.py
--rw-r--r--   0 debian    (1000) debian    (1000)       75 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/caped.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)     2065 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/graph_functions.py
--rw-r--r--   0 debian    (1000) debian    (1000)       68 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/kapoorlabs.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)    67911 2024-05-25 17:20:46.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/lightning_trainer.py
--rw-r--r--   0 debian    (1000) debian    (1000)    13532 2024-05-20 17:22:52.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/metrics.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4658 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/optimizers.py
--rw-r--r--   0 debian    (1000) debian    (1000)    10230 2024-05-13 17:03:42.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_callbacks.py
--rw-r--r--   0 debian    (1000) debian    (1000)    16120 2024-05-25 17:04:44.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_datasets.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2680 2024-02-23 15:21:15.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_loggers.py
--rw-r--r--   0 debian    (1000) debian    (1000)      762 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_losses.py
--rw-r--r--   0 debian    (1000) debian    (1000)    23059 2024-05-18 20:48:11.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_models.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1809 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_transforms.py
--rw-r--r--   0 debian    (1000) debian    (1000)     6283 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/schedulers.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2504 2024-05-17 21:13:17.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/utils.py
--rw-r--r--   0 debian    (1000) debian    (1000)      615 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/tox.ini
--rw-r--r--   0 debian    (1000) debian    (1000)      623 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/update_version.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-28 19:13:24.195317 kapoorlabs_lightning-5.4.2/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-28 19:13:24.183317 kapoorlabs_lightning-5.4.2/.github/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-28 19:13:24.187317 kapoorlabs_lightning-5.4.2/.github/workflows/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1068 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/.github/workflows/deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1963 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)      991 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/.gitignore
+-rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/LICENSE
+-rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/MANIFEST.in
+-rw-r--r--   0 debian    (1000) debian    (1000)     5043 2024-05-28 19:13:24.195317 kapoorlabs_lightning-5.4.2/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     3370 2024-05-27 13:23:19.000000 kapoorlabs_lightning-5.4.2/README.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-28 19:13:24.187317 kapoorlabs_lightning-5.4.2/images/
+-rw-r--r--   0 debian    (1000) debian    (1000)     6153 2024-05-27 13:04:25.000000 kapoorlabs_lightning-5.4.2/images/kapoorlablogo.png
+-rw-r--r--   0 debian    (1000) debian    (1000)   103449 2024-05-27 13:03:18.000000 kapoorlabs_lightning-5.4.2/images/mtrack.png
+-rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/pyproject.toml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1766 2024-05-28 19:13:24.195317 kapoorlabs_lightning-5.4.2/setup.cfg
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-28 19:13:24.187317 kapoorlabs_lightning-5.4.2/src/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-28 19:13:24.191317 kapoorlabs_lightning-5.4.2/src/KapoorLabs_Lightning.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     5043 2024-05-28 19:13:24.000000 kapoorlabs_lightning-5.4.2/src/KapoorLabs_Lightning.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     1220 2024-05-28 19:13:24.000000 kapoorlabs_lightning-5.4.2/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-05-28 19:13:24.000000 kapoorlabs_lightning-5.4.2/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)      102 2024-05-28 19:13:24.000000 kapoorlabs_lightning-5.4.2/src/KapoorLabs_Lightning.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       21 2024-05-28 19:13:24.000000 kapoorlabs_lightning-5.4.2/src/KapoorLabs_Lightning.egg-info/top_level.txt
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-28 19:13:24.191317 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1603 2024-05-17 14:55:57.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-28 19:13:24.191317 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/_tests/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/_tests/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3106 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-05-28 19:12:51.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/_version.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       75 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/caped.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     2065 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/graph_functions.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       68 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/kapoorlabs.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)    60859 2024-05-28 19:12:44.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/lightning_trainer.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    13532 2024-05-20 17:22:52.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/metrics.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4658 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/optimizers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    10230 2024-05-13 17:03:42.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/pytorch_callbacks.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    16120 2024-05-25 17:04:44.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/pytorch_datasets.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2680 2024-02-23 15:21:15.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/pytorch_loggers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      762 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/pytorch_losses.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    23059 2024-05-18 20:48:11.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/pytorch_models.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1809 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/pytorch_transforms.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     6283 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/schedulers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2504 2024-05-17 21:13:17.000000 kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/utils.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      615 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/tox.ini
+-rw-r--r--   0 debian    (1000) debian    (1000)      623 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.2/update_version.py
```

### Comparing `kapoorlabs_lightning-5.4.0/.github/workflows/deploy.yml` & `kapoorlabs_lightning-5.4.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/.github/workflows/test_and_deploy.yml` & `kapoorlabs_lightning-5.4.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/.gitignore` & `kapoorlabs_lightning-5.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/.pre-commit-config.yaml` & `kapoorlabs_lightning-5.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/LICENSE` & `kapoorlabs_lightning-5.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/PKG-INFO` & `kapoorlabs_lightning-5.4.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.4.0
+Version: 5.4.2
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
@@ -36,22 +36,37 @@
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 # KapoorLabs-Lightning
 
+
+# Developed by KapoorLabs
+
+
+<img src="images/mtrack.png" alt="Logo1" width="150"/>
+<img src="images/kapoorlablogo.png" alt="Logo2" width="150"/>
+
+This product is a testament to our expertise at KapoorLabs, where we specialize in creating cutting-edge solutions. We offer bespoke pipeline development services, transforming your developmental biology questions into publishable figures with our advanced computer vision and AI tools. Leverage our expertise and resources to achieve end-to-end solutions that make your research stand out.
+
+**Note:** The tools and pipelines showcased here represent only a fraction of what we can achieve. For tailored and comprehensive solutions beyond what was done in the referenced publication, engage with us directly. Our team is ready to provide the expertise and custom development you need to take your research to the next level. Visit us at [KapoorLabs](https://www.kapoorlabs.org/).
+
+
+
 [![License BSD-3](https://img.shields.io/pypi/l/KapoorLabs-Lightning.svg?color=green)](https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/KapoorLabs-Lightning.svg?color=green)](https://pypi.org/project/KapoorLabs-Lightning)
 [![Python Version](https://img.shields.io/pypi/pyversions/KapoorLabs-Lightning.svg?color=green)](https://python.org)
 [![tests](https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/workflows/tests/badge.svg)](https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/actions)
 [![codecov](https://codecov.io/gh/Kapoorlabs-CAPED/KapoorLabs-Lightning/branch/main/graph/badge.svg)](https://codecov.io/gh/Kapoorlabs-CAPED/KapoorLabs-Lightning)
 
 
-Lightning modules for KapoorLabs specific projects
+
+
+## Lightning modules for KapoorLabs specific projects
 
 ----------------------------------
 
 This [caped] package was generated with [Cookiecutter] using [@caped]'s [cookiecutter-template] template.
```

### Comparing `kapoorlabs_lightning-5.4.0/README.md` & `kapoorlabs_lightning-5.4.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 # KapoorLabs-Lightning
 
+
+# Developed by KapoorLabs
+
+
+<img src="images/mtrack.png" alt="Logo1" width="150"/>
+<img src="images/kapoorlablogo.png" alt="Logo2" width="150"/>
+
+This product is a testament to our expertise at KapoorLabs, where we specialize in creating cutting-edge solutions. We offer bespoke pipeline development services, transforming your developmental biology questions into publishable figures with our advanced computer vision and AI tools. Leverage our expertise and resources to achieve end-to-end solutions that make your research stand out.
+
+**Note:** The tools and pipelines showcased here represent only a fraction of what we can achieve. For tailored and comprehensive solutions beyond what was done in the referenced publication, engage with us directly. Our team is ready to provide the expertise and custom development you need to take your research to the next level. Visit us at [KapoorLabs](https://www.kapoorlabs.org/).
+
+
+
 [![License BSD-3](https://img.shields.io/pypi/l/KapoorLabs-Lightning.svg?color=green)](https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/KapoorLabs-Lightning.svg?color=green)](https://pypi.org/project/KapoorLabs-Lightning)
 [![Python Version](https://img.shields.io/pypi/pyversions/KapoorLabs-Lightning.svg?color=green)](https://python.org)
 [![tests](https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/workflows/tests/badge.svg)](https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/actions)
 [![codecov](https://codecov.io/gh/Kapoorlabs-CAPED/KapoorLabs-Lightning/branch/main/graph/badge.svg)](https://codecov.io/gh/Kapoorlabs-CAPED/KapoorLabs-Lightning)
 
 
-Lightning modules for KapoorLabs specific projects
+
+
+## Lightning modules for KapoorLabs specific projects
 
 ----------------------------------
 
 This [caped] package was generated with [Cookiecutter] using [@caped]'s [cookiecutter-template] template.
```

### Comparing `kapoorlabs_lightning-5.4.0/setup.cfg` & `kapoorlabs_lightning-5.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO` & `kapoorlabs_lightning-5.4.2/src/KapoorLabs_Lightning.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.4.0
+Version: 5.4.2
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
@@ -36,22 +36,37 @@
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 # KapoorLabs-Lightning
 
+
+# Developed by KapoorLabs
+
+
+<img src="images/mtrack.png" alt="Logo1" width="150"/>
+<img src="images/kapoorlablogo.png" alt="Logo2" width="150"/>
+
+This product is a testament to our expertise at KapoorLabs, where we specialize in creating cutting-edge solutions. We offer bespoke pipeline development services, transforming your developmental biology questions into publishable figures with our advanced computer vision and AI tools. Leverage our expertise and resources to achieve end-to-end solutions that make your research stand out.
+
+**Note:** The tools and pipelines showcased here represent only a fraction of what we can achieve. For tailored and comprehensive solutions beyond what was done in the referenced publication, engage with us directly. Our team is ready to provide the expertise and custom development you need to take your research to the next level. Visit us at [KapoorLabs](https://www.kapoorlabs.org/).
+
+
+
 [![License BSD-3](https://img.shields.io/pypi/l/KapoorLabs-Lightning.svg?color=green)](https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/KapoorLabs-Lightning.svg?color=green)](https://pypi.org/project/KapoorLabs-Lightning)
 [![Python Version](https://img.shields.io/pypi/pyversions/KapoorLabs-Lightning.svg?color=green)](https://python.org)
 [![tests](https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/workflows/tests/badge.svg)](https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/actions)
 [![codecov](https://codecov.io/gh/Kapoorlabs-CAPED/KapoorLabs-Lightning/branch/main/graph/badge.svg)](https://codecov.io/gh/Kapoorlabs-CAPED/KapoorLabs-Lightning)
 
 
-Lightning modules for KapoorLabs specific projects
+
+
+## Lightning modules for KapoorLabs specific projects
 
 ----------------------------------
 
 This [caped] package was generated with [Cookiecutter] using [@caped]'s [cookiecutter-template] template.
```

### Comparing `kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt` & `kapoorlabs_lightning-5.4.2/src/KapoorLabs_Lightning.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,16 @@
 README.md
 pyproject.toml
 setup.cfg
 tox.ini
 update_version.py
 .github/workflows/deploy.yml
 .github/workflows/test_and_deploy.yml
-licenses/Apache-2
-licenses/BSD-3
-licenses/GPL-3
-licenses/LGPL-3
-licenses/MIT
-licenses/MPL-2
+images/kapoorlablogo.png
+images/mtrack.png
 src/KapoorLabs_Lightning.egg-info/PKG-INFO
 src/KapoorLabs_Lightning.egg-info/SOURCES.txt
 src/KapoorLabs_Lightning.egg-info/dependency_links.txt
 src/KapoorLabs_Lightning.egg-info/requires.txt
 src/KapoorLabs_Lightning.egg-info/top_level.txt
 src/kapoorlabs_lightning/__init__.py
 src/kapoorlabs_lightning/_version.py
```

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/__init__.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/_tests/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/graph_functions.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/graph_functions.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/lightning_trainer.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/lightning_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,18 @@
 from pathlib import Path
 import numpy as np
 import torch
 import torch.nn.functional as F
 from lightning import Callback, LightningDataModule, LightningModule, Trainer
 from sklearn.cluster import KMeans
 from torch import optim
-import threading
 from datetime import timedelta
 import logging
-import fcntl
-import shutil
-from subprocess import call
 from types import FrameType
-from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Union
-from lightning.pytorch.utilities.rank_zero import rank_zero_info
-from lightning_utilities.core.rank_zero import rank_prefixed_message
+from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 from torch.nn import CosineSimilarity, BCEWithLogitsLoss, MSELoss
 from torch.nn.modules.loss import CrossEntropyLoss
 from torch.utils.data import DataLoader, Dataset
 from .utils import get_most_recent_file, load_checkpoint_model
 from . import optimizers, schedulers
 from .pytorch_models import (
     CloudAutoEncoder,
@@ -1689,19 +1683,14 @@
             num_sanity_val_steps=0,
             deterministic=self.deterministic,
             precision=self.precision,
             plugins=plugins,
             gradient_clip_val=self.gradient_clip_val,
             gradient_clip_algorithm=self.gradient_clip_algorithm,
         )
-        if self.slurm_auto_requeue:
-            self.trainer._signal_connector = _KlabSignalConnector(
-                self.trainer, self.model
-            )
-            self.trainer._signal_connector.register_signal_handlers()
 
         self.trainer.fit(
             self.model,
             train_dataloaders=self.train_dataloader,
             val_dataloaders=self.val_dataloader,
             ckpt_path=self.ckpt_path,
         )
@@ -1818,164 +1807,7 @@
 
     def __call__(self, signum: _SIGNUM, frame: FrameType) -> None:
         for signal_handler in self.signal_handlers:
             if isinstance(signal_handler, int):
                 signal_handler = signal.getsignal(signal_handler)
             if callable(signal_handler):
                 signal_handler(signum, frame)
-
-
-class _KlabSignalConnector:
-    def __init__(self, trainer: LightningTrainer, model: LightningModel) -> None:
-        self.received_sigterm = False
-        self.trainer = trainer
-        self.model = model
-        self._original_handlers: Dict[_SIGNUM, _HANDLER] = {}
-
-    def register_signal_handlers(self) -> None:
-        self.received_sigterm = False
-        self._original_handlers = self._get_current_signal_handlers()
-
-        sigusr_handlers: List[_HANDLER] = []
-        sigterm_handlers: List[_HANDLER] = [self._sigterm_notifier_fn]
-
-        environment = self.trainer._accelerator_connector.cluster_environment
-        if isinstance(environment, SLURMEnvironment) and environment.auto_requeue:
-            log.info("SLURM auto-requeueing enabled. Setting signal handlers for H100.")
-            sigusr_handlers.append(self._slurm_sigusr_handler_fn)
-            sigterm_handlers.append(self._sigterm_handler_fn)
-
-        sigusr = (
-            environment.requeue_signal
-            if isinstance(environment, SLURMEnvironment)
-            else signal.SIGUSR1
-        )
-        assert sigusr is not None
-        if sigusr_handlers and not self._has_already_handler(sigusr):
-            self._register_signal(sigusr, _HandlersCompose(sigusr_handlers))
-
-        # we have our own handler, but include existing ones too
-        if self._has_already_handler(signal.SIGTERM):
-            sigterm_handlers.append(signal.getsignal(signal.SIGTERM))
-        self._register_signal(signal.SIGTERM, _HandlersCompose(sigterm_handlers))
-
-    def _slurm_sigusr_handler_fn(self, signum: _SIGNUM, _: FrameType) -> None:
-        rank_zero_info(f"Handling auto-requeue signal on H100: {signum}")
-
-        log.info("recieved sigusr, Klabs custom pytorch lightning handler")
-
-        # save logger to make sure we get all the metrics
-        for logger in self.trainer.loggers:
-            logger.finalize("finished")
-        # Save the metrics
-        self._copy_files_on_sigterm()
-
-    def _copy_files_on_sigterm(self) -> None:
-        log.info("Copying files before handling SIGTERM.")
-        present_files = os.listdir(self.trainer.default_root_dir)
-
-        for file in present_files:
-            if file.endswith(".npz") or file.endswith(".json"):
-                backup_dir = os.path.join(self.trainer.default_root_dir, "backup")
-                Path(backup_dir).mkdir(parents=True, exist_ok=True)
-
-                # Lock the file before copying
-                with open(
-                    os.path.join(self.trainer.default_root_dir, file), "rb"
-                ) as src_file:
-                    with open(
-                        os.path.join(
-                            backup_dir,
-                            Path(file).stem
-                            + f"_epoch_{self.trainer.current_epoch}_step_{self.trainer.global_step}"
-                            + ".npz",
-                        ),
-                        "wb",
-                    ) as dst_file:
-                        fcntl.lockf(src_file.fileno(), fcntl.LOCK_SH)
-                        shutil.copyfileobj(src_file, dst_file)
-                        fcntl.lockf(src_file.fileno(), fcntl.LOCK_UN)
-
-        hpc_save_path = self.trainer._checkpoint_connector.hpc_save_path(
-            self.trainer.default_root_dir
-        )
-        self.trainer.save_checkpoint(hpc_save_path)
-
-        if self.trainer.is_global_zero:
-            # find job id
-            array_job_id = os.getenv("SLURM_ARRAY_JOB_ID")
-            if array_job_id is not None:
-                array_task_id = os.environ["SLURM_ARRAY_TASK_ID"]
-                job_id = f"{array_job_id}_{array_task_id}"
-            else:
-                job_id = os.environ["SLURM_JOB_ID"]
-
-            cmd = ["scontrol", "requeue", job_id]
-
-            # requeue job
-            log.info(f"requeing job {job_id}...")
-            try:
-                result = call(cmd)
-            except FileNotFoundError:
-                # This can occur if a subprocess call to `scontrol` is run outside a shell context
-                # Re-attempt call (now with shell context). If any error is raised, propagate to user.
-                # When running a shell command, it should be passed as a single string.
-                joint_cmd = [str(x) for x in cmd]
-                result = call(" ".join(joint_cmd), shell=True)
-
-            # print result text
-            if result == 0:
-                log.info(f"requeued exp {job_id}")
-            else:
-                log.warning("requeue failed...")
-
-        input()
-
-    def _sigterm_notifier_fn(self, signum: _SIGNUM, _: FrameType) -> None:
-        log.info(
-            rank_prefixed_message(
-                f"Received SIGTERM: {signum}", self.trainer.local_rank
-            )
-        )
-        # subprocesses killing the parent process is not supported, only the parent (rank 0) does it
-        if not self.received_sigterm:
-            # send the same signal to the subprocesses
-            launcher = self.trainer.strategy.launcher
-            if launcher is not None:
-                launcher.kill(signum)
-        self.received_sigterm = True
-
-    def _sigterm_handler_fn(self, signum: _SIGNUM, _: FrameType) -> None:
-        log.info(f"Bypassing SIGTERM on H100: {signum}")
-
-    def teardown(self) -> None:
-        """Restores the signals that were previously configured before :class:`_SignalConnector` replaced them."""
-        for signum, handler in self._original_handlers.items():
-            if handler is not None:
-                self._register_signal(signum, handler)
-        self._original_handlers = {}
-
-    @staticmethod
-    def _get_current_signal_handlers() -> Dict[_SIGNUM, _HANDLER]:
-        """Collects the currently assigned signal handlers."""
-        valid_signals = _KlabSignalConnector._valid_signals()
-        valid_signals -= {signal.SIGKILL, signal.SIGSTOP}
-        return {signum: signal.getsignal(signum) for signum in valid_signals}
-
-    @staticmethod
-    def _valid_signals() -> Set[signal.Signals]:
-        """Returns all valid signals supported on the current platform."""
-        return signal.valid_signals()
-
-    @staticmethod
-    def _has_already_handler(signum: _SIGNUM) -> bool:
-        return signal.getsignal(signum) not in (None, signal.SIG_DFL)
-
-    @staticmethod
-    def _register_signal(signum: _SIGNUM, handlers: _HANDLER) -> None:
-        if threading.current_thread() is threading.main_thread():
-            signal.signal(signum, handlers)  # type: ignore[arg-type]
-
-    def __getstate__(self) -> Dict:
-        state = self.__dict__.copy()
-        state["_original_handlers"] = {}
-        return state
```

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/metrics.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/metrics.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/optimizers.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/optimizers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_callbacks.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/pytorch_callbacks.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_datasets.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_loggers.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/pytorch_loggers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_losses.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/pytorch_losses.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_models.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/pytorch_models.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_transforms.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/pytorch_transforms.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/schedulers.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/schedulers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/utils.py` & `kapoorlabs_lightning-5.4.2/src/kapoorlabs_lightning/utils.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/tox.ini` & `kapoorlabs_lightning-5.4.2/tox.ini`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.4.0/update_version.py` & `kapoorlabs_lightning-5.4.2/update_version.py`

 * *Files identical despite different names*

