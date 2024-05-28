# Comparing `tmp/espresso_machine-0.0.200.tar.gz` & `tmp/espresso_machine-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espresso_machine-0.0.200.tar", last modified: Tue May 28 04:49:12 2024, max compression
+gzip compressed data, was "espresso_machine-0.0.25.tar", last modified: Tue May 28 04:46:04 2024, max compression
```

## Comparing `espresso_machine-0.0.200.tar` & `espresso_machine-0.0.25.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:49:12.563482 espresso_machine-0.0.200/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-28 04:49:12.563482 espresso_machine-0.0.200/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:49:12.555482 espresso_machine-0.0.200/espresso_machine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-28 04:49:12.000000 espresso_machine-0.0.200/espresso_machine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-28 04:49:12.000000 espresso_machine-0.0.200/espresso_machine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 04:49:12.000000 espresso_machine-0.0.200/espresso_machine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 04:49:12.000000 espresso_machine-0.0.200/espresso_machine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 04:49:12.000000 espresso_machine-0.0.200/espresso_machine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:49:12.563482 espresso_machine-0.0.200/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-28 04:49:10.000000 espresso_machine-0.0.200/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:49:12.555482 espresso_machine-0.0.200/src/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:49:12.559482 espresso_machine-0.0.200/src/espresso_machine/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/kpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/ph.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/ph_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/plot_band.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/plot_sigma_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/reads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:49:12.559482 espresso_machine-0.0.200/src/espresso_machine/seekpath/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/seekpath/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:49:12.559482 espresso_machine-0.0.200/src/espresso_machine/seekpath/brillouinzone/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/seekpath/brillouinzone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/seekpath/brillouinzone/brillouinzone.py
--rw-r--r--   0 runner    (1001) docker     (127)    26349 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/seekpath/getpaths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:49:12.559482 espresso_machine-0.0.200/src/espresso_machine/seekpath/hpkot/
--rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/seekpath/hpkot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/seekpath/hpkot/spg_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    11432 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/seekpath/hpkot/spg_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/seekpath/hpkot/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/seekpath/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-28 04:49:05.000000 espresso_machine-0.0.200/src/espresso_machine/writes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.697824 espresso_machine-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-28 04:46:04.697824 espresso_machine-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.693824 espresso_machine-0.0.25/espresso_machine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-28 04:46:04.000000 espresso_machine-0.0.25/espresso_machine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-28 04:46:04.000000 espresso_machine-0.0.25/espresso_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 04:46:04.000000 espresso_machine-0.0.25/espresso_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 04:46:04.000000 espresso_machine-0.0.25/espresso_machine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 04:46:04.000000 espresso_machine-0.0.25/espresso_machine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 04:46:04.697824 espresso_machine-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-28 04:46:02.000000 espresso_machine-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.693824 espresso_machine-0.0.25/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.693824 espresso_machine-0.0.25/src/espresso_machine/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/kpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/ph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/ph_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/plot_band.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/plot_sigma_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/reads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.693824 espresso_machine-0.0.25/src/espresso_machine/seekpath/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.697824 espresso_machine-0.0.25/src/espresso_machine/seekpath/brillouinzone/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/brillouinzone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/brillouinzone/brillouinzone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26349 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/getpaths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 04:46:04.697824 espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/
+-rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/spg_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11432 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/spg_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/seekpath/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-28 04:46:01.000000 espresso_machine-0.0.25/src/espresso_machine/writes.py
```

### Comparing `espresso_machine-0.0.200/LICENSE` & `espresso_machine-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/PKG-INFO` & `espresso_machine-0.0.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espresso_machine
-Version: 0.0.200
+Version: 0.0.25
 Summary: Quantum Espresso automation tool
 Home-page: https://github.com/susyexstsi/espresso-machine
 Author: Susy Exists
 Author-email: susy@selectron.me
 Keywords: pypi,cicd,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `espresso_machine-0.0.200/espresso_machine.egg-info/PKG-INFO` & `espresso_machine-0.0.25/espresso_machine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espresso-machine
-Version: 0.0.200
+Version: 0.0.25
 Summary: Quantum Espresso automation tool
 Home-page: https://github.com/susyexstsi/espresso-machine
 Author: Susy Exists
 Author-email: susy@selectron.me
 Keywords: pypi,cicd,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `espresso_machine-0.0.200/espresso_machine.egg-info/SOURCES.txt` & `espresso_machine-0.0.25/espresso_machine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/setup.py` & `espresso_machine-0.0.25/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="espresso_machine",
-    version='v0.0.200',
+    version='v0.0.25',
     author="Susy Exists",
     author_email="susy@selectron.me",
     description = "Quantum Espresso automation tool",
     url = "https://github.com/susyexstsi/espresso-machine",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

### Comparing `espresso_machine-0.0.200/src/espresso_machine/compute.py` & `espresso_machine-0.0.25/src/espresso_machine/compute.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/config.py` & `espresso_machine-0.0.25/src/espresso_machine/config.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/generate.py` & `espresso_machine-0.0.25/src/espresso_machine/generate.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/kpoints.py` & `espresso_machine-0.0.25/src/espresso_machine/kpoints.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/ph.py` & `espresso_machine-0.0.25/src/espresso_machine/ph.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/ph_plot.py` & `espresso_machine-0.0.25/src/espresso_machine/ph_plot.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/plot_band.py` & `espresso_machine-0.0.25/src/espresso_machine/plot_band.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/plot_sigma_energy.py` & `espresso_machine-0.0.25/src/espresso_machine/plot_sigma_energy.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/plots.py` & `espresso_machine-0.0.25/src/espresso_machine/plots.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/project.py` & `espresso_machine-0.0.25/src/espresso_machine/project.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/reads.py` & `espresso_machine-0.0.25/src/espresso_machine/reads.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/remote.py` & `espresso_machine-0.0.25/src/espresso_machine/remote.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/run.py` & `espresso_machine-0.0.25/src/espresso_machine/run.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/scaffold.py` & `espresso_machine-0.0.25/src/espresso_machine/scaffold.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/seekpath/__init__.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/__init__.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/seekpath/brillouinzone/brillouinzone.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/brillouinzone/brillouinzone.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/seekpath/getpaths.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/getpaths.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/seekpath/hpkot/__init__.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/__init__.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/seekpath/hpkot/spg_db.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/spg_db.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/seekpath/hpkot/spg_mapping.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/spg_mapping.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/seekpath/hpkot/tools.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/hpkot/tools.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/seekpath/util.py` & `espresso_machine-0.0.25/src/espresso_machine/seekpath/util.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/slurm.py` & `espresso_machine-0.0.25/src/espresso_machine/slurm.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/structure.py` & `espresso_machine-0.0.25/src/espresso_machine/structure.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/utils.py` & `espresso_machine-0.0.25/src/espresso_machine/utils.py`

 * *Files identical despite different names*

### Comparing `espresso_machine-0.0.200/src/espresso_machine/writes.py` & `espresso_machine-0.0.25/src/espresso_machine/writes.py`

 * *Files identical despite different names*

