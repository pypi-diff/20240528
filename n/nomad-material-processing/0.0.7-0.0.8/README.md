# Comparing `tmp/nomad-material-processing-0.0.7.tar.gz` & `tmp/nomad_material_processing-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomad-material-processing-0.0.7.tar", last modified: Tue Feb 20 10:19:53 2024, max compression
+gzip compressed data, was "nomad_material_processing-0.0.8.tar", last modified: Tue May 28 15:02:06 2024, max compression
```

## Comparing `nomad-material-processing-0.0.7.tar` & `nomad_material_processing-0.0.8.tar`

### file list

```diff
@@ -1,49 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:53.749907 nomad-material-processing-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:53.741907 nomad-material-processing-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:53.741907 nomad-material-processing-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:53.741907 nomad-material-processing-0.0.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-02-20 10:19:53.749907 nomad-material-processing-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/nomad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 10:19:53.749907 nomad-material-processing-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:53.741907 nomad-material-processing-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:53.745907 nomad-material-processing-0.0.7/src/nomad_material_processing/
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/src/nomad_material_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/src/nomad_material_processing/chemical_vapor_deposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/src/nomad_material_processing/combinatorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/src/nomad_material_processing/crystal_growth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/src/nomad_material_processing/epitaxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/src/nomad_material_processing/nomad_plugin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/src/nomad_material_processing/physical_vapor_deposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/src/nomad_material_processing/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/src/nomad_material_processing/vapor_deposition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:53.749907 nomad-material-processing-0.0.7/src/nomad_material_processing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-02-20 10:19:53.000000 nomad-material-processing-0.0.7/src/nomad_material_processing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-20 10:19:53.000000 nomad-material-processing-0.0.7/src/nomad_material_processing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 10:19:53.000000 nomad-material-processing-0.0.7/src/nomad_material_processing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-20 10:19:53.000000 nomad-material-processing-0.0.7/src/nomad_material_processing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-20 10:19:53.000000 nomad-material-processing-0.0.7/src/nomad_material_processing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:53.745907 nomad-material-processing-0.0.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:53.749907 nomad-material-processing-0.0.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_activity_step.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_crystal_growth.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_czochralski_process.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_epitaxy.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_metal_organic_vapor_phase_epitaxy.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_molecular_beam_epitaxy.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_physical_vapor_deposition.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_pulsed_laser_deposition.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_sample_deposition.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_sputter_deposition.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_substrate.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_thermal_evaporation.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_thin_film.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_thin_film_stack.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/data/test_vapor_phase_epitaxy.archive.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-20 10:19:44.000000 nomad-material-processing-0.0.7/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:02:05.994429 nomad_material_processing-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:02:05.986429 nomad_material_processing-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:02:05.986429 nomad_material_processing-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:02:05.986429 nomad_material_processing-0.0.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-05-28 15:02:05.994429 nomad_material_processing-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/nomad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:02:05.994429 nomad_material_processing-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:02:05.986429 nomad_material_processing-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:02:05.990429 nomad_material_processing-0.0.8/src/nomad_material_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/combinatorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/crystal_growth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/epitaxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/nomad_plugin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:02:05.990429 nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/
+-rw-r--r--   0 runner    (1001) docker     (127)    14976 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:02:05.990429 nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/cvd/
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/cvd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/cvd/nomad_plugin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/nomad_plugin.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:02:05.990429 nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/pvd/
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/pvd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/pvd/nomad_plugin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/pvd/pld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/pvd/sputtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/pvd/thermal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:02:05.994429 nomad_material_processing-0.0.8/src/nomad_material_processing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-05-28 15:02:05.000000 nomad_material_processing-0.0.8/src/nomad_material_processing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-28 15:02:05.000000 nomad_material_processing-0.0.8/src/nomad_material_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:02:05.000000 nomad_material_processing-0.0.8/src/nomad_material_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 15:02:05.000000 nomad_material_processing-0.0.8/src/nomad_material_processing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 15:02:05.000000 nomad_material_processing-0.0.8/src/nomad_material_processing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:02:05.990429 nomad_material_processing-0.0.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:02:05.994429 nomad_material_processing-0.0.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_activity_step.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_crystal_growth.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_czochralski_process.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_epitaxy.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_metal_organic_vapor_phase_epitaxy.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_molecular_beam_epitaxy.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_physical_vapor_deposition.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_pulsed_laser_deposition.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_sample_deposition.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_sputter_deposition.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_substrate.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_thermal_evaporation.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_thin_film.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_thin_film_stack.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/data/test_vapor_phase_epitaxy.archive.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-28 15:02:01.000000 nomad_material_processing-0.0.8/tests/test_schema.py
```

### Comparing `nomad-material-processing-0.0.7/.github/workflows/python-publish.yml` & `nomad_material_processing-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nomad-material-processing-0.0.7/.gitignore` & `nomad_material_processing-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nomad-material-processing-0.0.7/LICENSE` & `nomad_material_processing-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nomad-material-processing-0.0.7/PKG-INFO` & `nomad_material_processing-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomad-material-processing
-Version: 0.0.7
+Version: 0.0.8
 Summary: A plugin for NOMAD containing base sections for material processing.
 Author-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>, Andrea Albino <andrea.albino@physik.hu-berlin.de>, Sebastian Brückner <sebastian.brueckner@ikz-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `nomad-material-processing-0.0.7/README.md` & `nomad_material_processing-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nomad-material-processing-0.0.7/src/nomad_material_processing/__init__.py` & `nomad_material_processing-0.0.8/src/nomad_material_processing/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,83 +47,83 @@
     from nomad.datamodel.datamodel import (
         EntryArchive,
     )
     from structlog.stdlib import (
         BoundLogger,
     )
 
-m_package = Package(name="Material Processing")
+m_package = Package(name='Material Processing')
 
 
 class Geometry(ArchiveSection):
     """
     Geometrical shape attributes of a system.
     Sections derived from `Geometry` represent concrete geometrical shapes.
     """
 
     m_def = Section()
     volume = Quantity(
         type=float,
-        description="The measure of the amount of space occupied in 3D space.",
+        description='The measure of the amount of space occupied in 3D space.',
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.NumberEditQuantity,
         ),
-        unit="meter ** 3",
+        unit='meter ** 3',
     )
 
 
 class Parallelepiped(Geometry):
     """
     Six-faced polyhedron with each pair of opposite faces parallel and equal in size,
     characterized by rectangular sides and parallelogram faces.
     """
 
     m_def = Section()
     height = Quantity(
         type=float,
-        description="The z dimension of the parallelepiped.",
+        description='The z dimension of the parallelepiped.',
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.NumberEditQuantity,
-            defaultDisplayUnit="millimeter",
-            label="Height (z)",
+            defaultDisplayUnit='millimeter',
+            label='Height (z)',
         ),
-        unit="meter",
+        unit='meter',
     )
     width = Quantity(
         type=float,
-        description="The x dimension of the parallelepiped.",
+        description='The x dimension of the parallelepiped.',
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.NumberEditQuantity,
-            defaultDisplayUnit="millimeter",
-            label="Width (x)",
+            defaultDisplayUnit='millimeter',
+            label='Width (x)',
         ),
-        unit="meter",
+        unit='meter',
     )
     length = Quantity(
         type=float,
-        description="The y dimension of the parallelepiped.",
+        description='The y dimension of the parallelepiped.',
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.NumberEditQuantity,
-            defaultDisplayUnit="millimeter",
-            label="Length (y)",
+            defaultDisplayUnit='millimeter',
+            label='Length (y)',
         ),
-        unit="meter",
+        unit='meter',
     )
     surface_area = Quantity(
         type=float,
         description="""
         The product of length and width, representing the total exposed area of the
         primary surface.
         """,
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.NumberEditQuantity,
-            defaultDisplayUnit="millimeter ** 2",
-            label="Surface Area (x*y)",
+            defaultDisplayUnit='millimeter ** 2',
+            label='Surface Area (x*y)',
         ),
-        unit="meter ** 2",
+        unit='meter ** 2',
     )
 
 
 class Miscut(ArchiveSection):
     """
     The miscut in a crystalline substrate refers to
     the intentional deviation from a specific crystallographic orientation,
@@ -133,53 +133,53 @@
     angle = Quantity(
         type=float,
         description="""
         The angular displacement from the crystallographic orientation of the substrate.
         """,
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.NumberEditQuantity,
-            defaultDisplayUnit="deg",
-            label="Miscut Angle",
+            defaultDisplayUnit='deg',
+            label='Miscut Angle',
         ),
-        unit="deg",
+        unit='deg',
     )
     angle_deviation = Quantity(
         type=float,
-        description="The ± uncertainty in the angular displacement.",
+        description='The ± uncertainty in the angular displacement.',
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.NumberEditQuantity,
-            defaultDisplayUnit="deg",
-            label="± Miscut Angle Deviation",
+            defaultDisplayUnit='deg',
+            label='± Miscut Angle Deviation',
         ),
-        unit="deg",
+        unit='deg',
     )
     orientation = Quantity(
         type=str,
-        description="The direction of the miscut in Miller index, [hkl].",
+        description='The direction of the miscut in Miller index, [hkl].',
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.StringEditQuantity,
-            label="Miscut Orientation [hkl]",
+            label='Miscut Orientation [hkl]',
         ),
     )
 
 
 class Dopant(ElementalComposition):
     """
     A dopant element in a crystalline structure
     is a foreign atom intentionally introduced into the crystal lattice.
     """
 
     doping_level = Quantity(
         type=float,
-        description="The chemical doping level.",
+        description='The chemical doping level.',
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.NumberEditQuantity,
-            defaultDisplayUnit="1 / cm ** 3",
+            defaultDisplayUnit='1 / cm ** 3',
         ),
-        unit="1 / m ** 3",
+        unit='1 / m ** 3',
     )
 
 
 class CrystalProperties(ArchiveSection):
     """
     Characteristics arising from the ordered arrangement of atoms in a crystalline structure.
     These properties are defined by factors such as crystal symmetry, lattice parameters,
@@ -196,15 +196,15 @@
         type=str,
         description="""
         Alignment of crystal lattice with respect to a vector normal to the surface
         specified using Miller indices.
         """,
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.StringEditQuantity,
-            label="Substrate Orientation (hkl)",
+            label='Substrate Orientation (hkl)',
         ),
     )
     miscut = SubSection(
         section_def=Miscut,
         description="""
         Section describing any miscut of the substrate with respect to the substrate
         orientation.
@@ -217,51 +217,51 @@
     A thin free standing sheet of material. Not to be confused with the substrate role
     during a deposition, which can be a `Substrate` with `ThinFilm`(s) on it.
     """
 
     m_def = Section()
     supplier = Quantity(
         type=str,
-        description="The supplier of the current substrate specimen.",
+        description='The supplier of the current substrate specimen.',
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.StringEditQuantity,
-            label="Name of Supplier",
+            label='Name of Supplier',
         ),
     )
     supplier_id = Quantity(
         type=str,
-        description="An ID string that is unique from the supplier.",
+        description='An ID string that is unique from the supplier.',
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.StringEditQuantity,
-            label="Supplier ID",
+            label='Supplier ID',
         ),
     )
     lab_id = Quantity(
         type=str,
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.StringEditQuantity,
-            label="Substrate ID",
+            label='Substrate ID',
         ),
     )
 
 
 class CrystallineSubstrate(Substrate):
     """
     The substrate defined in this class is composed of periodic arrangement of atoms
     and shows typical features of a crystal structure.
     """
 
     m_def = Section()
     geometry = SubSection(
         section_def=Geometry,
-        description="Section containing the geometry of the substrate.",
+        description='Section containing the geometry of the substrate.',
     )
     crystal_properties = SubSection(
         section_def=SubstrateCrystalProperties,
-        description="Section containing the crystal properties of the substrate.",
+        description='Section containing the crystal properties of the substrate.',
     )
     dopants = SubSection(
         section_def=Dopant,
         repeats=True,
         description="""
         Repeating section containing information on any dopants in the substrate.
         """,
@@ -273,69 +273,69 @@
     A thin film of material which exists as part of a stack.
     """
 
     m_def = Section()
 
     geometry = SubSection(
         section_def=Geometry,
-        description="Section containing the geometry of the thin film.",
+        description='Section containing the geometry of the thin film.',
     )
 
 
 class ThinFilmReference(CompositeSystemReference):
     """
     Class autogenerated from yaml schema.
     """
 
     lab_id = Quantity(
         type=str,
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.StringEditQuantity,
-            label="Thin Film ID",
+            label='Thin Film ID',
         ),
     )
     reference = Quantity(
         type=ThinFilm,
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.ReferenceEditQuantity,
-            label="Thin Film",
+            label='Thin Film',
         ),
     )
 
 
 class SubstrateReference(CompositeSystemReference):
     """
     A section for describing a system component and its role in a composite system.
     """
 
     lab_id = Quantity(
         type=str,
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.StringEditQuantity,
-            label="Substrate ID",
+            label='Substrate ID',
         ),
     )
     reference = Quantity(
         type=Substrate,
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.ReferenceEditQuantity,
-            label="Substrate",
+            label='Substrate',
         ),
     )
 
 
 class ThinFilmStack(CompositeSystem):
     """
     A stack of `ThinFilm`(s). Typically deposited on a `Substrate`.
     """
 
     m_def = Section(
         a_eln=ELNAnnotation(
             hide=[
-                "components",
+                'components',
             ],
         ),
     )
     layers = SubSection(
         description="""
         An ordered list (starting at the substrate) of the thin films making up the
         thin film stacks.
@@ -347,27 +347,29 @@
         description="""
         The substrate which the thin film layers of the thin film stack are deposited
         on.
         """,
         section_def=SubstrateReference,
     )
 
-    def normalize(self, archive: "EntryArchive", logger: "BoundLogger") -> None:
+    def normalize(self, archive: 'EntryArchive', logger: 'BoundLogger') -> None:
         """
         The normalizer for the `ThinFilmStack` class.
 
         Args:
             archive (EntryArchive): The archive containing the section that is being
             normalized.
             logger (BoundLogger): A structlog logger.
         """
         self.components = []
         if self.layers:
             self.components = [
-                SystemComponent(system=layer.reference) for layer in self.layers if layer.reference
+                SystemComponent(system=layer.reference)
+                for layer in self.layers
+                if layer.reference
             ]
         if self.substrate.reference:
             self.components.append(SystemComponent(system=self.substrate.reference))
         super().normalize(archive, logger)
 
 
 class ThinFilmStackReference(CompositeSystemReference):
@@ -397,15 +399,15 @@
     new phase. [database_cross_reference: https://orcid.org/0000-0002-0640-0422]
 
     Synonyms:
      - deposition
     """
 
     m_def = Section(
-        links=["http://purl.obolibrary.org/obo/CHMO_0001310"],
+        links=['http://purl.obolibrary.org/obo/CHMO_0001310'],
     )
 
     def is_serial(self) -> bool:
         """
         Method for determining if the steps are serial. Can be overwritten by sub class.
         Default behavior is to return True if all steps start after the previous one.
 
@@ -414,24 +416,24 @@
         """
         start_times = []
         durations = []
         for step in self.steps:
             if step.start_time is None or step.duration is None:
                 return False
             start_times.append(step.start_time.timestamp())
-            durations.append(step.duration.to("s").magnitude)
+            durations.append(step.duration.to('s').magnitude)
         start_times = np.array(start_times)
         durations = np.array(durations)
         end_times = start_times + durations
         diffs = start_times[1:] - end_times[:-1]
         if np.any(diffs < 0):
             return False
         return True
 
-    def normalize(self, archive: "EntryArchive", logger: "BoundLogger") -> None:
+    def normalize(self, archive: 'EntryArchive', logger: 'BoundLogger') -> None:
         """
         The normalizer for the `SampleDeposition` class.
 
         Args:
             archive (EntryArchive): The archive containing the section that is being
             normalized.
             logger (BoundLogger): A structlog logger.
@@ -446,8 +448,73 @@
                 if previous is not None:
                     task.inputs.append(Link(name=previous.name, section=previous))
                 tasks.append(task)
                 previous = step
             archive.workflow2.tasks = tasks
 
 
+class TimeSeries(ArchiveSection):
+    """
+    A time series of data during a process step.
+    This is an abstract class and should not be used directly.
+    Instead, it should be derived and the the units of the `value` and `set_value` should
+    be specified.
+
+    For example, a derived class could be `Temperature` with `value` in Kelvin:
+    ```python
+    class Temperature(TimeSeries):
+        value = TimeSeries.value.m_copy()
+        value.unit = "kelvin"
+        set_value = TimeSeries.set_value.m_copy()
+        set_value.unit = "kelvin"
+        set_value.a_eln.defaultDisplayUnit = "celsius"
+    ```
+    """
+
+    m_def = Section(
+        a_plot=dict(
+            # x=['time', 'set_time'],
+            # y=['value', 'set_value'],
+            x='time',
+            y='value',
+        ),
+    )
+    set_value = Quantity(
+        type=float,
+        description='The set value(s) (i.e. the intended values) set.',
+        shape=['*'],
+        a_eln=ELNAnnotation(
+            component=ELNComponentEnum.NumberEditQuantity,
+            label='Set value',
+        ),
+    )
+    set_time = Quantity(
+        type=float,
+        unit='s',
+        description="""
+        The process time when each of the set values were set.
+        If this is empty and only one set value is present, it is assumed that the value
+        was set at the start of the process step.
+        If two set values are present, it is assumed that a linear ramp between the two
+        values was set.
+        """,
+        shape=['*'],
+        a_eln=ELNAnnotation(
+            component=ELNComponentEnum.NumberEditQuantity,
+            defaultDisplayUnit='s',
+            label='Set time',
+        ),
+    )
+    value = Quantity(
+        type=float,
+        description='The observed value as a function of time.',
+        shape=['*'],
+    )
+    time = Quantity(
+        type=float,
+        unit='s',
+        description='The process time when each of the values were recorded.',
+        shape=['*'],
+    )
+
+
 m_package.__init_metainfo__()
```

### Comparing `nomad-material-processing-0.0.7/src/nomad_material_processing/combinatorial.py` & `nomad_material_processing-0.0.8/src/nomad_material_processing/combinatorial.py`

 * *Files identical despite different names*

### Comparing `nomad-material-processing-0.0.7/src/nomad_material_processing/crystal_growth.py` & `nomad_material_processing-0.0.8/src/nomad_material_processing/crystal_growth.py`

 * *Files identical despite different names*

### Comparing `nomad-material-processing-0.0.7/src/nomad_material_processing/epitaxy.py` & `nomad_material_processing-0.0.8/src/nomad_material_processing/epitaxy.py`

 * *Files identical despite different names*

### Comparing `nomad-material-processing-0.0.7/src/nomad_material_processing/physical_vapor_deposition.py` & `nomad_material_processing-0.0.8/src/nomad_material_processing/vapor_deposition/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,538 +29,516 @@
     ArchiveSection,
 )
 from nomad.datamodel.metainfo.annotations import (
     ELNAnnotation,
     ELNComponentEnum,
 )
 from nomad.datamodel.metainfo.basesections import (
-    CompositeSystem,
-    CompositeSystemReference,
-    ReadableIdentifiers,
+    ActivityStep,
+    PureSubstanceSection,
+    Component,
 )
-
-from nomad_material_processing.vapor_deposition import (
-    EvaporationSource,
-    VaporDepositionSource,
-    SampleParameters,
-    VaporDepositionStep,
-    VaporDeposition,
+from nomad.datamodel.metainfo.plot import (
+    PlotSection,
+)
+from nomad.datamodel.metainfo.workflow import (
+    Link,
+    Task,
+)
+from nomad_material_processing import (
+    SampleDeposition,
+    ThinFilmStackReference,
+    ThinFilmReference,
+    TimeSeries,
 )
 
 if TYPE_CHECKING:
     from nomad.datamodel.datamodel import (
         EntryArchive,
     )
     from structlog.stdlib import (
         BoundLogger,
     )
 
-m_package = Package(name="Physical Vapor Deposition")
+m_package = Package(name='Vapor Deposition')
 
 
-class SourcePower(ArchiveSection):
-    m_def = Section(
-        a_plot=dict(
-            x="process_time",
-            y="power",
-        ),
-    )
-    power = Quantity(
-        type=float,
-        unit="watt",
-        shape=["*"],
-    )
-    process_time = Quantity(
-        type=float,
-        unit="second",
-        shape=["*"],
-    )
-
-
-class PVDEvaporationSource(EvaporationSource):
-    m_def = Section(
-        a_plot=dict(
-            x="power/process_time",
-            y="power/power",
-        ),
-    )
-    power = SubSection(
-        section_def=SourcePower,
-    )
-
+class MolarFlowRate(TimeSeries):
+    """
+    Molar flow rate is the amount of a substance which passes per unit of time.
+    """
 
-class ImpingingFlux(ArchiveSection):
     m_def = Section(
         a_plot=dict(
-            x="process_time",
-            y="rate",
+            # x=['time', 'set_time'],
+            # y=['value', 'set_value'],
+            x='time',
+            y='value',
         ),
     )
-    rate = Quantity(
-        type=float,
-        unit="mol/meter ** 2/second",
-        shape=["*"],
-    )
-    process_time = Quantity(
-        type=float,
-        unit="second",
-        shape=["*"],
-    )
     measurement_type = Quantity(
         type=MEnum(
-            "Assumed",
-            "Quartz Crystal Microbalance",
-        )
+            'Assumed',
+            'Mass Flow Controller',
+        ),
+        a_eln=ELNAnnotation(
+            component=ELNComponentEnum.EnumEditQuantity,
+        ),
     )
+    value = TimeSeries.value.m_copy()
+    value.unit = 'mol/second'
+    set_value = TimeSeries.set_value.m_copy()
+    set_value.unit = 'mol/second'
 
 
-class PVDSource(VaporDepositionSource):
-    m_def = Section(
-        a_plot=[
-            dict(
-                x=[
-                    "evaporation_source/power/process_time",
-                    "material_source/rate/process_time",
-                ],
-                y=[
-                    "evaporation_source/power/power",
-                    "material_source/rate/rate",
-                ],
-            ),
-        ],
-    )
-    vapor_source = SubSection(
-        section_def=PVDEvaporationSource,
+class EvaporationSource(ArchiveSection):
+    pass
+
+
+class VaporDepositionSource(ArchiveSection):
+    name = Quantity(
+        type=str,
         description="""
-        Example: A heater, a filament, a laser, etc.
+        A short and descriptive name for this source.
         """,
     )
-    impinging_flux = SubSection(
-        section_def=ImpingingFlux,
+    material = SubSection(
+        section_def=Component,
         description="""
-        The deposition rate of the material onto the substrate (mol/area/time).
+        The source of the material that is being evaporated.
+        Example: A sputtering target, a powder in a crucible, etc.
         """,
         repeats=True,
     )
-
-
-class PVDSampleParameters(SampleParameters):
-    heater = Quantity(
+    vapor_source = SubSection(
+        section_def=EvaporationSource,
         description="""
-        What is the substrate heated by.
+        Example: A heater, a filament, a laser, a bubbler, etc.
         """,
-        type=MEnum(
-            "No heating",
-            "Halogen lamp",
-            "Filament",
-            "Resistive element",
-            "CO2 laser",
-        ),
     )
-    distance_to_source = Quantity(
-        type=float,
-        unit="meter",
+    vapor_molar_flow_rate = SubSection(
+        section_def=MolarFlowRate,
         description="""
-        The distance between the substrate and all the sources.
-        In the case of multiple sources, the distances are listed in the same order as the
-        sources are listed in the parent `VaporDepositionStep` section.
+        The rate of the material being evaporated (mol/time).
         """,
-        shape=["*"],
-    )
-
-
-class PVDStep(VaporDepositionStep):
-    """
-    A step of any physical vapor deposition process.
-    """
-
-    sources = SubSection(
-        section_def=PVDSource,
-        repeats=True,
-    )
-    sample_parameters = SubSection(
-        section_def=PVDSampleParameters,
-        repeats=True,
     )
 
-    def normalize(self, archive: "EntryArchive", logger: "BoundLogger") -> None:
-        """
-        The normalizer for the `PVDStep` class.
-
-        Args:
-            archive (EntryArchive): The archive containing the section that is being
-            normalized.
-            logger (BoundLogger): A structlog logger.
-        """
-        super(PVDStep, self).normalize(archive, logger)
-
-
-class PhysicalVaporDeposition(VaporDeposition):
-    """
-    A synthesis technique where vaporized molecules or atoms condense on a surface,
-    forming a thin layer. The process is purely physical; no chemical reaction occurs
-    at the surface. [database_cross_reference: https://orcid.org/0000-0002-0640-0422]
-
-    Synonyms:
-     - PVD
-     - physical vapor deposition
-    """
 
+class GrowthRate(TimeSeries):
     m_def = Section(
-        links=["http://purl.obolibrary.org/obo/CHMO_0001356"],
-        a_plot=[
-            dict(
-                x="steps/:/environment/pressure/process_time",
-                y="steps/:/environment/pressure/pressure",
-            ),
-            dict(
-                x="steps/:/source/:/evaporation_source/power/process_time",
-                y="steps/:/source/:/evaporation_source/power/power",
-            ),
-        ],
-    )
-    steps = SubSection(
-        description="""
-        The steps of the deposition process.
-        """,
-        section_def=PVDStep,
-        repeats=True,
-    )
-
-    def normalize(self, archive: "EntryArchive", logger: "BoundLogger") -> None:
-        """
-        The normalizer for the `PhysicalVaporDeposition` class.
-
-        Args:
-            archive (EntryArchive): The archive containing the section that is being
-            normalized.
-            logger (BoundLogger): A structlog logger.
-        """
-        super(PhysicalVaporDeposition, self).normalize(archive, logger)
-
-
-class PLDTarget(CompositeSystem):
-    target_id = SubSection(
-        section_def=ReadableIdentifiers,
+        a_plot=dict(
+            # x=['time', 'set_time'],
+            # y=['value', 'set_value'],
+            x='time',
+            y='value',
+        ),
     )
-
-
-class PLDTargetReference(CompositeSystemReference):
-    lab_id = Quantity(
-        type=str,
+    measurement_type = Quantity(
+        type=MEnum(
+            'Assumed',
+            'RHEED',
+            'Reflectance',
+        ),
         a_eln=ELNAnnotation(
-            component=ELNComponentEnum.StringEditQuantity,
-            label="Target ID",
+            component=ELNComponentEnum.EnumEditQuantity,
         ),
     )
-    reference = Quantity(
-        type=PLDTarget,
+    # value = TimeSeries.value.m_copy()
+    # value.unit = 'meter/second'
+    # set_value = TimeSeries.set_value.m_copy()
+    # set_value.unit = 'meter/second'
+    # set_value.a_eln.defaultDisplayUnit = 'nm/second'
+    value = Quantity(
+        type=float,
+        unit='meter/second',
+        shape=['*'],
+    )
+    set_value = Quantity(
+        type=float,
+        description='The set value(s) (i.e. the intended values) set.',
+        shape=['*'],
+        unit='meter/second',
         a_eln=ELNAnnotation(
-            component=ELNComponentEnum.ReferenceEditQuantity,
+            component=ELNComponentEnum.NumberEditQuantity,
+            label='Set value',
         ),
     )
 
 
-class PLDLaser(PVDEvaporationSource):
-    wavelength = Quantity(
-        type=float,
-        unit="meter",
-        a_eln=ELNAnnotation(
-            component=ELNComponentEnum.NumberEditQuantity,
-            defaultDisplayUnit="nanometer",
+class Temperature(TimeSeries):
+    """
+    Generic Temperature monitoring
+    """
+
+    m_def = Section(
+        a_plot=dict(
+            # x=['time', 'set_time'],
+            # y=['value', 'set_value'],
+            x='time',
+            y='value',
         ),
     )
-    repetition_rate = Quantity(
-        type=float,
-        unit="hertz",
+    measurement_type = Quantity(
+        type=MEnum(
+            'Heater thermocouple',
+            'Thermocouple',
+            'Pyrometer',
+            'Assumed',
+        ),
         a_eln=ELNAnnotation(
-            component=ELNComponentEnum.NumberEditQuantity,
-            defaultDisplayUnit="hertz",
+            component=ELNComponentEnum.EnumEditQuantity,
         ),
     )
-    spot_size = Quantity(
+    # value = TimeSeries.value.m_copy()
+    # value.unit = 'kelvin'
+    # set_value = TimeSeries.set_value.m_copy()
+    # set_value.unit = 'kelvin'
+    # set_value.a_eln.defaultDisplayUnit = 'celsius'
+    value = Quantity(
         type=float,
-        unit="meter ** 2",
-        a_eln=ELNAnnotation(
-            component=ELNComponentEnum.NumberEditQuantity,
-            defaultDisplayUnit="millimeter ** 2",
-        ),
+        unit='kelvin',
+        shape=['*'],
     )
-    pulses = Quantity(
-        description="""
-        The total number of laser pulses during the deposition step.
-        """,
-        type=int,
+    set_value = Quantity(
+        type=float,
+        description='The set value(s) (i.e. the intended values) set.',
+        shape=['*'],
+        unit='kelvin',
         a_eln=ELNAnnotation(
             component=ELNComponentEnum.NumberEditQuantity,
+            label='Set value',
         ),
     )
 
 
-class PLDSource(PVDSource):
-    material = SubSection(
-        section_def=PLDTargetReference,
+class SampleParameters(PlotSection, ArchiveSection):
+    m_def = Section(
+        a_plotly_graph_object={
+            'label': 'Measured Temperatures',
+            'index': 1,
+            'dragmode': 'pan',
+            'data': {
+                'type': 'scattergl',
+                'line': {'width': 2},
+                'marker': {'size': 2},
+                'mode': 'lines+markers',
+                'name': 'Temperature',
+                'x': '#temperature/time',
+                'y': '#temperature/value',
+            },
+            'layout': {
+                'title': {'text': 'Measured Temperature'},
+                'xaxis': {
+                    'showticklabels': True,
+                    'fixedrange': True,
+                    'ticks': '',
+                    'title': {'text': 'Process time [s]'},
+                    'showline': True,
+                    'linewidth': 1,
+                    'linecolor': 'black',
+                    'mirror': True,
+                },
+                'yaxis': {
+                    'showticklabels': True,
+                    'fixedrange': True,
+                    'ticks': '',
+                    'title': {'text': 'Temperature [°C]'},
+                    'showline': True,
+                    'linewidth': 1,
+                    'linecolor': 'black',
+                    'mirror': True,
+                },
+                'showlegend': False,
+            },
+            'config': {
+                'displayModeBar': False,
+                'scrollZoom': False,
+                'responsive': False,
+                'displaylogo': False,
+                'dragmode': False,
+            },
+        },
+    )
+    growth_rate = SubSection(
+        section_def=GrowthRate,
         description="""
-        The source of the material that is being evaporated.
-        Example: A sputtering target, a powder in a crucible, etc.
+        The growth rate of the thin film (length/time).
+        Measured by in-situ RHEED or Reflection or assumed.
         """,
     )
-    vapor_source = SubSection(
-        section_def=PLDLaser,
+    substrate_temperature = SubSection(
+        section_def=Temperature,
+    )
+    layer = SubSection(
         description="""
-        Section containing the details of the laser source.
+        The thin film that is being created during this step.
         """,
+        section_def=ThinFilmReference,
     )
-
-
-class PLDStep(PVDStep):
-    sources = SubSection(
-        section_def=PLDSource,
-        repeats=True,
+    substrate = SubSection(
+        description="""
+        The thin film stack that is being evaporated on.
+        """,
+        section_def=ThinFilmStackReference,
     )
 
 
-class PulsedLaserDeposition(PhysicalVaporDeposition):
+class Pressure(TimeSeries):
     """
-    A synthesis technique where a high-power pulsed laser beam is focused (inside a
-    vacuum chamber) onto a target of the desired composition. Material is then
-    vaporized from the target ('ablation') and deposited as a thin film on a
-    substrate facing the target.
-    [database_cross_reference: https://orcid.org/0000-0002-0640-0422]
-
-    Synonyms:
-     - pulsed laser ablation deposition
-     - PLD
-     - pulsed-laser ablation deposition
-     - laser ablation growth
-     - PLA deposition
-     - pulsed-laser deposition
+    The pressure during the deposition process.
     """
 
     m_def = Section(
-        links=["http://purl.obolibrary.org/obo/CHMO_0001363"],
+        a_plot=dict(
+            # x=['time', 'set_time'],
+            # y=['value', 'set_value'],
+            x='time',
+            y='value',
+        ),
     )
-    method = Quantity(
-        type=str,
-        default="Pulsed Laser Deposition",
+    # value = TimeSeries.value.m_copy()
+    # value.unit = 'pascal'
+    # set_value = TimeSeries.set_value.m_copy()
+    # set_value.unit = 'pascal'
+    # set_value.a_eln.defaultDisplayUnit = 'mbar'
+    value = Quantity(
+        type=float,
+        unit='pascal',
+        shape=['*'],
     )
-    steps = SubSection(
-        description="""
-        The steps of the deposition process.
-        """,
-        section_def=PLDStep,
-        repeats=True,
+    time = Quantity(
+        type=float,
+        unit='second',
+        shape=['*'],
     )
-
-    def normalize(self, archive: "EntryArchive", logger: "BoundLogger") -> None:
-        """
-        The normalizer for the `PulsedLaserDeposition` class.
-
-        Args:
-            archive (EntryArchive): The archive containing the section that is being
-            normalized.
-            logger (BoundLogger): A structlog logger.
-        """
-        super(PulsedLaserDeposition, self).normalize(archive, logger)
-
-
-class SputterDeposition(PhysicalVaporDeposition):
-    """
-    A synthesis technique where a solid target is bombarded with electrons or
-    energetic ions (e.g. Ar+) causing atoms to be ejected ('sputtering'). The ejected
-    atoms then deposit, as a thin-film, on a substrate.
-    [database_cross_reference: https://orcid.org/0000-0002-0640-0422]
-
-    Synonyms:
-     - sputtering
-     - sputter coating
-    """
-
-    m_def = Section(
-        links=["http://purl.obolibrary.org/obo/CHMO_0001364"],
+    set_value = Quantity(
+        type=float,
+        unit='pascal',
+        shape=['*'],
     )
-    method = Quantity(
-        type=str,
-        default="Sputter Deposition",
+    set_time = Quantity(
+        type=float,
+        unit='second',
+        shape=['*'],
     )
 
-    def normalize(self, archive: "EntryArchive", logger: "BoundLogger") -> None:
-        """
-        The normalizer for the `SputterDeposition` class.
-
-        Args:
-            archive (EntryArchive): The archive containing the section that is being
-            normalized.
-            logger (BoundLogger): A structlog logger.
-        """
-        super(SputterDeposition, self).normalize(archive, logger)
 
+class VolumetricFlowRate(TimeSeries):
+    """
+    The volumetric flow rate of a gas at standard conditions, i.e. the equivalent rate
+    at a temperature of 0 °C (273.15 K) and a pressure of 1 atm (101325 Pa).
+    """
 
-class ThermalEvaporationHeaterTemperature(ArchiveSection):
     m_def = Section(
         a_plot=dict(
-            x="process_time",
-            y="temperature",
+            # x=['time', 'set_time'],
+            # y=['value', 'set_value'],
+            x='time',
+            y='value',
         ),
     )
-    temperature = Quantity(
+    measurement_type = Quantity(
+        type=MEnum(
+            'Mass Flow Controller',
+            'Flow Meter',
+            'Other',
+        ),
+    )
+    # value = TimeSeries.value.m_copy()
+    # value.unit = 'meter ** 3 / second'
+    # set_value = TimeSeries.set_value.m_copy()
+    # set_value.unit = 'meter ** 3 / second'
+    # set_value.a_eln.defaultDisplayUnit = 'centimeter ** 3 / minute'
+    value = Quantity(
         type=float,
-        unit="kelvin",
-        shape=["*"],
+        unit='meter ** 3 / second',
+        shape=['*'],
     )
-    process_time = Quantity(
+    set_value = Quantity(
         type=float,
-        unit="second",
-        shape=["*"],
+        description='The set value(s) (i.e. the intended values) set.',
+        shape=['*'],
+        unit='meter ** 3 / second',
+        a_eln=ELNAnnotation(
+            component=ELNComponentEnum.NumberEditQuantity,
+            label='Set value',
+            defaultDisplayUnit='centimeter ** 3 / minute',
+        ),
     )
 
 
-class ThermalEvaporationHeater(PVDEvaporationSource):
+class GasFlow(ArchiveSection):
+    """
+    Section describing the flow of a gas.
+    """
+
     m_def = Section(
         a_plot=dict(
-            x=[
-                "temperature/process_time",
-                "power/process_time",
-            ],
-            y=[
-                "temperature/temperature",
-                "power/power",
-            ],
-            lines=[
-                dict(
-                    mode="lines",
-                    line=dict(
-                        color="rgb(25, 46, 135)",
-                    ),
-                ),
-                dict(
-                    mode="lines",
-                    line=dict(
-                        color="rgb(0, 138, 104)",
-                    ),
-                ),
-            ],
+            # x=['flow_rate/time', 'flow_rate/set_time'],
+            # y=['flow_rate/value', 'flow_rate/set_value'],
+            x='flow_rate/time',
+            y='flow_rate/value',
         ),
     )
-    temperature = SubSection(
-        section_def=ThermalEvaporationHeaterTemperature,
+    gas = SubSection(
+        section_def=PureSubstanceSection,
     )
+    flow_rate = SubSection(
+        section_def=VolumetricFlowRate,
+    )
+
 
+class SubstrateHeater(ArchiveSection):
+    pass
 
-class ThermalEvaporationSource(PVDSource):
+
+class ChamberEnvironment(ArchiveSection):
     m_def = Section(
         a_plot=dict(
-            x=[
-                "deposition_rate/process_time",
-                "vapor_source/temperature/process_time",
-            ],
-            y=[
-                "deposition_rate/rate",
-                "vapor_source/temperature/temperature",
-            ],
-            lines=[
-                dict(
-                    mode="lines",
-                    line=dict(
-                        color="rgb(25, 46, 135)",
-                    ),
-                ),
-                dict(
-                    mode="lines",
-                    line=dict(
-                        color="rgb(0, 138, 104)",
-                    ),
-                ),
-            ],
+            x='pressure/time',
+            y='pressure/value',
         ),
     )
-    vapor_source = SubSection(
-        section_def=ThermalEvaporationHeater,
+    gas_flow = SubSection(
+        section_def=GasFlow,
+        repeats=True,
+    )
+    pressure = SubSection(
+        section_def=Pressure,
+    )
+    heater = SubSection(
+        section_def=SubstrateHeater,
     )
 
 
-class ThermalEvaporationStep(PVDStep):
-    m_def = Section(
-        a_plot=[
-            dict(
-                x="sources/:/deposition_rate/process_time",
-                y="sources/:/deposition_rate/rate",
-            ),
-            dict(
-                x="sources/:/vapor_source/temperature/process_time",
-                y="sources/:/vapor_source/temperature/temperature",
-            ),
-            dict(
-                x="sources/:/vapor_source/power/process_time",
-                y="sources/:/vapor_source/power/power",
-            ),
-        ],
+class VaporDepositionStep(ActivityStep):
+    """
+    A step of any vapor deposition process.
+    """
+
+    m_def = Section()
+    creates_new_thin_film = Quantity(
+        type=bool,
+        description="""
+        Whether or not this step creates a new thin film.
+        """,
+        default=False,
+        a_eln=ELNAnnotation(
+            component='BoolEditQuantity',
+        ),
+    )
+    duration = Quantity(
+        type=float,
+        unit='second',
     )
     sources = SubSection(
-        section_def=ThermalEvaporationSource,
+        section_def=VaporDepositionSource,
         repeats=True,
     )
+    sample_parameters = SubSection(
+        section_def=SampleParameters,
+        repeats=True,
+    )
+    environment = SubSection(
+        section_def=ChamberEnvironment,
+    )
+
+    def to_task(self) -> Task:
+        """
+        Returns the task description of this activity step.
 
+        Returns:
+            Task: The activity step as a workflow task.
+        """
+        inputs = []
+        for source in self.sources:
+            if source.material is not None and hasattr(source.material, 'system'):
+                inputs.append(
+                    Link(
+                        name=getattr(source.material, 'name', None),
+                        section=getattr(source.material, 'system', None),
+                    )
+                )
+            elif source.material is not None and hasattr(
+                source.material, 'pure_substance'
+            ):
+                inputs.append(
+                    Link(
+                        name=getattr(source.material, 'substance_name', None),
+                        section=getattr(source.material, 'pure_substance', None),
+                    )
+                )
+        outputs = [
+            Link(
+                name=parameters.layer.name,
+                section=parameters.layer.reference,
+            )
+            for parameters in self.sample_parameters
+            if parameters.layer is not None and parameters.layer.reference is not None
+        ]
+        return Task(name=self.name, inputs=inputs, outputs=outputs)
+
+    def normalize(self, archive: 'EntryArchive', logger: 'BoundLogger') -> None:
+        """
+        The normalizer for the `VaporDepositionStep` class.
 
-class ThermalEvaporation(PhysicalVaporDeposition):
+        Args:
+            archive (EntryArchive): The archive containing the section that is being
+            normalized.
+            logger (BoundLogger): A structlog logger.
+        """
+        super(VaporDepositionStep, self).normalize(archive, logger)
+
+
+class VaporDeposition(SampleDeposition):
     """
-    A synthesis technique where the material to be deposited is heated until
-    evaporation in a vacuum (<10^{-4} Pa) and eventually deposits as a thin film by
-    condensing on a (cold) substrate.
-    [database_cross_reference: https://orcid.org/0000-0002-0640-0422]
-
-    Synonyms:
-     - evaporative deposition)
-     - vacuum thermal evaporation
-     - TE
-     - thermal deposition
-     - filament evaporation
-     - vacuum condensation
+    VaporDeposition is a general class that encompasses both Physical Vapor Deposition
+    (PVD) and Chemical Vapor Deposition (CVD).
+    It involves the deposition of material from a vapor phase to a solid thin film or
+    coating onto a substrate.
+     - material sources:
+       Both PVD and CVD involve a source material that is transformed into a vapor phase.
+       In PVD, the source material is physically evaporated or sputtered from a solid
+       target.
+       In CVD, gaseous precursors undergo chemical reactions to produce a solid material
+       on the substrate.
+     - substrate:
+       The substrate is the material onto which the thin film is deposited.
+     - environment:
+       The process typically takes place in a controlled environment.
+       The deposition is usually affected by the pressure in the chamber.
+       For some processes additional background gasses are also added.
     """
 
     m_def = Section(
-        links=["http://purl.obolibrary.org/obo/CHMO_0001360"],
+        links=[
+            'http://purl.obolibrary.org/obo/CHMO_0001314',
+            'http://purl.obolibrary.org/obo/CHMO_0001356',
+        ],
         a_plot=[
             dict(
-                x="steps/:/sources/:/deposition_rate/process_time",
-                y="steps/:/sources/:/deposition_rate/rate",
-            ),
-            dict(
-                x="steps/:/sources/:/vapor_source/temperature/process_time",
-                y="steps/:/sources/:/vapor_source/temperature/temperature",
-            ),
-            dict(
-                x="steps/:/environment/pressure/process_time",
-                y="steps/:/environment/pressure/pressure",
-                layout=dict(
-                    yaxis=dict(
-                        type="log",
-                    ),
-                ),
+                x='steps/:/environment/pressure/time',
+                y='steps/:/environment/pressure/value',
             ),
         ],
     )
-    method = Quantity(
-        type=str,
-        default="Thermal Evaporation",
-    )
     steps = SubSection(
         description="""
         The steps of the deposition process.
         """,
-        section_def=ThermalEvaporationStep,
+        section_def=VaporDepositionStep,
         repeats=True,
     )
 
-    def normalize(self, archive: "EntryArchive", logger: "BoundLogger") -> None:
+    def normalize(self, archive: 'EntryArchive', logger: 'BoundLogger') -> None:
         """
-        The normalizer for the `ThermalEvaporation` class.
+        The normalizer for the `VaporDeposition` class.
 
         Args:
             archive (EntryArchive): The archive containing the section that is being
             normalized.
             logger (BoundLogger): A structlog logger.
         """
-        super(ThermalEvaporation, self).normalize(archive, logger)
+        super(VaporDeposition, self).normalize(archive, logger)
 
 
 m_package.__init_metainfo__()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nomad-material-processing-0.0.7/src/nomad_material_processing/utils.py` & `nomad_material_processing-0.0.8/src/nomad_material_processing/utils.py`

 * *Files identical despite different names*

### Comparing `nomad-material-processing-0.0.7/src/nomad_material_processing.egg-info/PKG-INFO` & `nomad_material_processing-0.0.8/src/nomad_material_processing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomad-material-processing
-Version: 0.0.7
+Version: 0.0.8
 Summary: A plugin for NOMAD containing base sections for material processing.
 Author-email: Hampus Näsström <hampus.naesstroem@physik.hu-berlin.de>, Andrea Albino <andrea.albino@physik.hu-berlin.de>, Sebastian Brückner <sebastian.brueckner@ikz-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `nomad-material-processing-0.0.7/src/nomad_material_processing.egg-info/SOURCES.txt` & `nomad_material_processing-0.0.8/src/nomad_material_processing.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,33 @@
 README.md
 nomad.yaml
 pyproject.toml
 setup.py
 .github/workflows/python-publish.yml
 .vscode/settings.json
 src/nomad_material_processing/__init__.py
-src/nomad_material_processing/chemical_vapor_deposition.py
 src/nomad_material_processing/combinatorial.py
 src/nomad_material_processing/crystal_growth.py
 src/nomad_material_processing/epitaxy.py
 src/nomad_material_processing/nomad_plugin.yaml
-src/nomad_material_processing/physical_vapor_deposition.py
 src/nomad_material_processing/utils.py
-src/nomad_material_processing/vapor_deposition.py
 src/nomad_material_processing.egg-info/PKG-INFO
 src/nomad_material_processing.egg-info/SOURCES.txt
 src/nomad_material_processing.egg-info/dependency_links.txt
 src/nomad_material_processing.egg-info/requires.txt
 src/nomad_material_processing.egg-info/top_level.txt
+src/nomad_material_processing/vapor_deposition/__init__.py
+src/nomad_material_processing/vapor_deposition/nomad_plugin.yaml
+src/nomad_material_processing/vapor_deposition/cvd/__init__.py
+src/nomad_material_processing/vapor_deposition/cvd/nomad_plugin.yaml
+src/nomad_material_processing/vapor_deposition/pvd/__init__.py
+src/nomad_material_processing/vapor_deposition/pvd/nomad_plugin.yaml
+src/nomad_material_processing/vapor_deposition/pvd/pld.py
+src/nomad_material_processing/vapor_deposition/pvd/sputtering.py
+src/nomad_material_processing/vapor_deposition/pvd/thermal.py
 tests/test_schema.py
 tests/data/test_activity_step.archive.yaml
 tests/data/test_crystal_growth.archive.yaml
 tests/data/test_czochralski_process.archive.yaml
 tests/data/test_epitaxy.archive.yaml
 tests/data/test_metal_organic_vapor_phase_epitaxy.archive.yaml
 tests/data/test_molecular_beam_epitaxy.archive.yaml
```

