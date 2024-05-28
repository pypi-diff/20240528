# Comparing `tmp/rm_tools-1.4.4.tar.gz` & `tmp/rm_tools-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rm_tools-1.4.4.tar", last modified: Wed May  8 07:56:54 2024, max compression
+gzip compressed data, was "rm_tools-1.4.6.tar", last modified: Tue May 28 08:02:49 2024, max compression
```

## Comparing `rm_tools-1.4.4.tar` & `rm_tools-1.4.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.629675 rm_tools-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-08 07:56:50.000000 rm_tools-1.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-08 07:56:50.000000 rm_tools-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-08 07:56:54.629675 rm_tools-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-08 07:56:50.000000 rm_tools-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.625675 rm_tools-1.4.4/RM_Tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-08 07:56:54.000000 rm_tools-1.4.4/RM_Tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-08 07:56:54.000000 rm_tools-1.4.4/RM_Tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:56:54.000000 rm_tools-1.4.4/RM_Tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 07:56:54.000000 rm_tools-1.4.4/RM_Tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-08 07:56:54.000000 rm_tools-1.4.4/RM_Tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 07:56:54.000000 rm_tools-1.4.4/RM_Tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.621675 rm_tools-1.4.4/RMtools_1D/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10722 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/calculate_RMSF.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.621675 rm_tools-1.4.4/RMtools_1D/cats/
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/cats/catComplex.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/cats/cat_simple_doQUfit.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/cats/catalogue.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/cats/catalogue1.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/cats/testCat.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)     5040 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/clean_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/do_QUfit_1D_mnest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21574 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/do_RMclean_1D.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29863 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/do_RMsynth_1D.py
--rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/do_RMsynth_1D_fromFITS.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15427 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/mk_test_ascii_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.621675 rm_tools-1.4.4/RMtools_1D/models_ns/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m11.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m111.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m6.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/models_ns/m7.py
--rw-r--r--   0 runner    (1001) docker     (127)    52381 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/rmtools_bwdepol.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_1D/rmtools_bwpredict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.625675 rm_tools-1.4.4/RMtools_3D/
--rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/RMpeakfit_3D.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/assemble_chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/create_chunks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21367 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/do_RMclean_3D.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    36920 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/do_RMsynth_3D.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21729 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/do_fitIcube.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/extract_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/make_freq_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/mk_test_cube_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMtools_3D/rescale_I_model_3D.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:56:54.625675 rm_tools-1.4.4/RMutils/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    95236 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/mpfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/util_FITS.py
--rw-r--r--   0 runner    (1001) docker     (127)    85719 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/util_RM.py
--rw-r--r--   0 runner    (1001) docker     (127)    47529 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/util_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/util_plotFITS.py
--rw-r--r--   0 runner    (1001) docker     (127)    75833 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/util_plotTk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-08 07:56:50.000000 rm_tools-1.4.4/RMutils/util_rec.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:56:54.629675 rm_tools-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-08 07:56:50.000000 rm_tools-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:02:49.724573 rm_tools-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-28 08:02:45.000000 rm_tools-1.4.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 08:02:45.000000 rm_tools-1.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-28 08:02:49.720573 rm_tools-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-28 08:02:45.000000 rm_tools-1.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:02:49.720573 rm_tools-1.4.6/RM_Tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-28 08:02:49.000000 rm_tools-1.4.6/RM_Tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-28 08:02:49.000000 rm_tools-1.4.6/RM_Tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:02:49.000000 rm_tools-1.4.6/RM_Tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-28 08:02:49.000000 rm_tools-1.4.6/RM_Tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-28 08:02:49.000000 rm_tools-1.4.6/RM_Tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 08:02:49.000000 rm_tools-1.4.6/RM_Tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:02:49.716573 rm_tools-1.4.6/RMtools_1D/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10722 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/calculate_RMSF.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:02:49.716573 rm_tools-1.4.6/RMtools_1D/cats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/cats/catComplex.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/cats/cat_simple_doQUfit.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/cats/catalogue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/cats/catalogue1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/cats/testCat.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5040 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/clean_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/do_QUfit_1D_mnest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21574 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/do_RMclean_1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29863 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/do_RMsynth_1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/do_RMsynth_1D_fromFITS.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15427 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/mk_test_ascii_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:02:49.716573 rm_tools-1.4.6/RMtools_1D/models_ns/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/models_ns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/models_ns/m1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/models_ns/m11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/models_ns/m111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/models_ns/m2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/models_ns/m3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/models_ns/m4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/models_ns/m5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/models_ns/m6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/models_ns/m7.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52381 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/rmtools_bwdepol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_1D/rmtools_bwpredict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:02:49.720573 rm_tools-1.4.6/RMtools_3D/
+-rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_3D/RMpeakfit_3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_3D/assemble_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_3D/create_chunks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21367 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_3D/do_RMclean_3D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    36920 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_3D/do_RMsynth_3D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21729 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_3D/do_fitIcube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_3D/extract_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_3D/make_freq_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_3D/mk_test_cube_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMtools_3D/rescale_I_model_3D.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:02:49.720573 rm_tools-1.4.6/RMutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95236 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMutils/mpfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMutils/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMutils/util_FITS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85714 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMutils/util_RM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47529 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMutils/util_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMutils/util_plotFITS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75833 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMutils/util_plotTk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-28 08:02:45.000000 rm_tools-1.4.6/RMutils/util_rec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:02:49.724573 rm_tools-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-28 08:02:45.000000 rm_tools-1.4.6/setup.py
```

### Comparing `rm_tools-1.4.4/LICENSE.txt` & `rm_tools-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/PKG-INFO` & `rm_tools-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: RM-Tools
-Version: 1.4.4
+Version: 1.4.6
 Summary: RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
 Home-page: https://github.com/CIRADA-Tools/RM-Tools
-Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.4.tar.gz
+Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.6.tar.gz
 Maintainer: Cameron Van Eck
 Maintainer-email: cameron.vaneck@anu.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rm_tools-1.4.4/README.md` & `rm_tools-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RM_Tools.egg-info/PKG-INFO` & `rm_tools-1.4.6/RM_Tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: RM-Tools
-Version: 1.4.4
+Version: 1.4.6
 Summary: RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
 Home-page: https://github.com/CIRADA-Tools/RM-Tools
-Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.4.tar.gz
+Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.6.tar.gz
 Maintainer: Cameron Van Eck
 Maintainer-email: cameron.vaneck@anu.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rm_tools-1.4.4/RM_Tools.egg-info/SOURCES.txt` & `rm_tools-1.4.6/RM_Tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RM_Tools.egg-info/entry_points.txt` & `rm_tools-1.4.6/RM_Tools.egg-info/entry_points.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [console_scripts]
 qufit = RMtools_1D.do_QUfit_1D_mnest:main
 rmclean1d = RMtools_1D.do_RMclean_1D:main
 rmclean3d = RMtools_3D.do_RMclean_3D:main
 rmsynth1d = RMtools_1D.do_RMsynth_1D:main
 rmsynth1dFITS = RMtools_1D.do_RMsynth_1D_fromFITS:main
 rmsynth3d = RMtools_3D.do_RMsynth_3D:main
-rmtools_3DIrescale = RMtools_3D.rescale_I_model_3D:main
+rmtools_3DIrescale = RMtools_3D.rescale_I_model_3D:command_line
 rmtools_assemblechunks = RMtools_3D.assemble_chunks:main
 rmtools_bwdepol = RMtools_1D.rmtools_bwdepol:main
 rmtools_bwpredict = RMtools_1D.rmtools_bwpredict:main
 rmtools_calcRMSF = RMtools_1D.calculate_RMSF:main
 rmtools_createchunks = RMtools_3D.create_chunks:main
 rmtools_extractregion = RMtools_3D.extract_region:main
 rmtools_fitIcube = RMtools_3D.do_fitIcube:main
```

### Comparing `rm_tools-1.4.4/RMtools_1D/calculate_RMSF.py` & `rm_tools-1.4.6/RMtools_1D/calculate_RMSF.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/cats/catComplex.csv` & `rm_tools-1.4.6/RMtools_1D/cats/catComplex.csv`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/cats/cat_simple_doQUfit.bat` & `rm_tools-1.4.6/RMtools_1D/cats/cat_simple_doQUfit.bat`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/cats/catalogue.csv` & `rm_tools-1.4.6/RMtools_1D/cats/catalogue.csv`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/cats/catalogue1.csv` & `rm_tools-1.4.6/RMtools_1D/cats/catalogue1.csv`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/cats/testCat.dat` & `rm_tools-1.4.6/RMtools_1D/cats/testCat.dat`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/clean_model.py` & `rm_tools-1.4.6/RMtools_1D/clean_model.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/do_QUfit_1D_mnest.py` & `rm_tools-1.4.6/RMtools_1D/do_QUfit_1D_mnest.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/do_RMclean_1D.py` & `rm_tools-1.4.6/RMtools_1D/do_RMclean_1D.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/do_RMsynth_1D.py` & `rm_tools-1.4.6/RMtools_1D/do_RMsynth_1D.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/do_RMsynth_1D_fromFITS.py` & `rm_tools-1.4.6/RMtools_1D/do_RMsynth_1D_fromFITS.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/mk_test_ascii_data.py` & `rm_tools-1.4.6/RMtools_1D/mk_test_ascii_data.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/models_ns/m1.py` & `rm_tools-1.4.6/RMtools_1D/models_ns/m1.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/models_ns/m11.py` & `rm_tools-1.4.6/RMtools_1D/models_ns/m11.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/models_ns/m111.py` & `rm_tools-1.4.6/RMtools_1D/models_ns/m111.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/models_ns/m2.py` & `rm_tools-1.4.6/RMtools_1D/models_ns/m2.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/models_ns/m3.py` & `rm_tools-1.4.6/RMtools_1D/models_ns/m3.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/models_ns/m4.py` & `rm_tools-1.4.6/RMtools_1D/models_ns/m4.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/models_ns/m5.py` & `rm_tools-1.4.6/RMtools_1D/models_ns/m5.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/models_ns/m6.py` & `rm_tools-1.4.6/RMtools_1D/models_ns/m6.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/models_ns/m7.py` & `rm_tools-1.4.6/RMtools_1D/models_ns/m7.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/rmtools_bwdepol.py` & `rm_tools-1.4.6/RMtools_1D/rmtools_bwdepol.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_1D/rmtools_bwpredict.py` & `rm_tools-1.4.6/RMtools_1D/rmtools_bwpredict.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_3D/RMpeakfit_3D.py` & `rm_tools-1.4.6/RMtools_3D/RMpeakfit_3D.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_3D/assemble_chunks.py` & `rm_tools-1.4.6/RMtools_3D/assemble_chunks.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_3D/create_chunks.py` & `rm_tools-1.4.6/RMtools_3D/create_chunks.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_3D/do_RMclean_3D.py` & `rm_tools-1.4.6/RMtools_3D/do_RMclean_3D.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_3D/do_RMsynth_3D.py` & `rm_tools-1.4.6/RMtools_3D/do_RMsynth_3D.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_3D/do_fitIcube.py` & `rm_tools-1.4.6/RMtools_3D/do_fitIcube.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_3D/extract_region.py` & `rm_tools-1.4.6/RMtools_3D/extract_region.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_3D/make_freq_file.py` & `rm_tools-1.4.6/RMtools_3D/make_freq_file.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMtools_3D/mk_test_cube_data.py` & `rm_tools-1.4.6/RMtools_3D/mk_test_cube_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,15 +416,15 @@
         coordLst_deg.append([preLst[0], preLst[1]])
         [(x_pix, y_pix)] = wcs2D.wcs_world2pix([(preLst[0], preLst[1])], 0)
         coordLst_pix.append([x_pix, y_pix])
         successCount += 1
 
     # Loop through the frequency channels & insert the IQU planes
     for iChan, _ in enumerate(
-        tqdm(freqArr_Hz), desc=f"Looping through {nChans} frequency channels"
+        tqdm(freqArr_Hz, desc=f"Looping through {nChans} frequency channels")
     ):
         for iSrc, _ in enumerate(spectraILst):
             params = [
                 spectraILst[iSrc][iChan],  # amplitude
                 coordLst_pix[iSrc][0],  # X centre (pix)
                 coordLst_pix[iSrc][1],  # Y centre
                 beamMinSigma_pix,  # width (sigma)
```

### Comparing `rm_tools-1.4.4/RMtools_3D/rescale_I_model_3D.py` & `rm_tools-1.4.6/RMtools_3D/rescale_I_model_3D.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 import multiprocessing as mp
 import os
 from functools import partial
 
 import astropy.io.fits as pf
 import numpy as np
 
-from RMutils.util_misc import renormalize_StokesI_model
+from RMutils.util_misc import FitResult, renormalize_StokesI_model
 
 
 def command_line():
     """Handle invocation from the command line, parsing inputs and running
     everything."""
 
     # Help string to be shown using the -h option
@@ -225,16 +225,31 @@
     covar, coeff, old_freq, new_freq = data
     oldDict = {}  # Initialize a fitDict, which contains the relevant fit information
     oldDict["reference_frequency_Hz"] = old_freq
     oldDict["p"] = coeff
     oldDict["pcov"] = covar
     oldDict["fit_function"] = fit_function
 
-    newDict = renormalize_StokesI_model(oldDict, new_freq)
-    return newDict["p"], newDict["perror"]
+    old_result = FitResult(
+        params=coeff,
+        fitStatus=np.nan,  # Placeholder
+        chiSq=np.nan,  # Placeholder
+        chiSqRed=np.nan,  # Placeholder
+        AIC=np.nan,  # Placeholder
+        polyOrd=len(coeff) - 1,
+        nIter=0,  # Placeholder
+        reference_frequency_Hz=old_freq,
+        dof=np.nan,  # Placeholder
+        pcov=covar,
+        perror=np.zeros_like(coeff),  # Placeholder
+        fit_function=fit_function,
+    )
+
+    new_fit_result = renormalize_StokesI_model(old_result, new_freq)
+    return new_fit_result.params, new_fit_result.perror
 
 
 def rescale_I_model_3D(
     covar_map, old_reffreq_map, new_freq_map, coeffs, fit_function="log", num_cores=1
 ):
     """Rescale the Stokes I model parameters to a new reference frequency, for
     an entire image (i.e., 3D pipeline products).
```

### Comparing `rm_tools-1.4.4/RMutils/mpfit.py` & `rm_tools-1.4.6/RMutils/mpfit.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMutils/normalize.py` & `rm_tools-1.4.6/RMutils/normalize.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMutils/util_FITS.py` & `rm_tools-1.4.6/RMutils/util_FITS.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMutils/util_RM.py` & `rm_tools-1.4.6/RMutils/util_RM.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
 
         # Calculate the RMSF for each plane
         a = (lambdaSqArr_m2 - lam0Sq_m2).astype(dtFloat)
         RMSFcube = (
             finufft.nufft1d3(
                 x=a,
                 c=np.ascontiguousarray(weightCube.T),
-                s=(phiArr_radm2[::-1] * 2).astype(a.dtype),
+                s=(phi2Arr[::-1] * 2).astype(a.dtype),
                 eps=eps,
             )
             * KArr[..., None]
         ).T
 
         # Clean up one cube worth of memory
         del weightCube
```

### Comparing `rm_tools-1.4.4/RMutils/util_misc.py` & `rm_tools-1.4.6/RMutils/util_misc.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMutils/util_plotFITS.py` & `rm_tools-1.4.6/RMutils/util_plotFITS.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMutils/util_plotTk.py` & `rm_tools-1.4.6/RMutils/util_plotTk.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/RMutils/util_rec.py` & `rm_tools-1.4.6/RMutils/util_rec.py`

 * *Files identical despite different names*

### Comparing `rm_tools-1.4.4/setup.py` & `rm_tools-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from setuptools import setup
 
 NAME = "RM-Tools"
 DESCRIPTION = "RM-synthesis, RM-clean and QU-fitting on polarised radio spectra"
 URL = "https://github.com/CIRADA-Tools/RM-Tools"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.4.4"
+VERSION = "1.4.6"
 DOWNLOAD_URL = (
     "https://github.com/CIRADA-Tools/RM-Tools/archive/v" + VERSION + ".tar.gz"
 )
 
 REQUIRED = [
     "numpy<2",
     "numpy>1.22;python_version=='3.8'",
@@ -66,15 +66,15 @@
             "rmtools_assemblechunks=RMtools_3D.assemble_chunks:main",
             "rmtools_fitIcube=RMtools_3D.do_fitIcube:main",
             "rmtools_peakfitcube=RMtools_3D.RMpeakfit_3D:main",
             "rmtools_testdata3D=RMtools_3D.mk_test_cube_data:main",
             "rmtools_extractregion=RMtools_3D.extract_region:main",
             "rmtools_bwdepol=RMtools_1D.rmtools_bwdepol:main",
             "rmtools_bwpredict=RMtools_1D.rmtools_bwpredict:main",
-            "rmtools_3DIrescale=RMtools_3D.rescale_I_model_3D:main",
+            "rmtools_3DIrescale=RMtools_3D.rescale_I_model_3D:command_line",
         ],
     },
     install_requires=REQUIRED,
     extras_require=extras_require,
     include_package_data=True,
     license="MIT",
     classifiers=[
```

