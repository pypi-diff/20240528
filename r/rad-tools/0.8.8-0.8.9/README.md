# Comparing `tmp/rad-tools-0.8.8.tar.gz` & `tmp/rad-tools-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.8.8.tar", last modified: Wed Sep 27 17:49:17 2023, max compression
+gzip compressed data, was "rad-tools-0.8.9.tar", last modified: Sat Sep 30 23:32:46 2023, max compression
```

## Comparing `rad-tools-0.8.8.tar` & `rad-tools-0.8.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-27 17:49:17.224257 rad-tools-0.8.8/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    35149 2023-09-20 00:56:50.000000 rad-tools-0.8.8/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2841 2023-09-27 17:49:17.223722 rad-tools-0.8.8/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2132 2023-09-26 09:00:20.000000 rad-tools-0.8.8/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-27 17:49:17.183420 rad-tools-0.8.8/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2841 2023-09-27 17:49:16.000000 rad-tools-0.8.8/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2104 2023-09-27 17:49:17.000000 rad-tools-0.8.8/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-09-27 17:49:16.000000 rad-tools-0.8.8/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-09-27 17:49:16.000000 rad-tools-0.8.8/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-09-27 17:49:16.000000 rad-tools-0.8.8/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-27 17:49:17.188726 rad-tools-0.8.8/radtools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1729 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1236 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/__main__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    35945 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/_license.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1032 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/_osfix.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      977 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/constants.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-27 17:49:17.195213 rad-tools-0.8.8/radtools/crystal/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1428 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    10727 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/atom.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-27 17:49:17.199089 rad-tools-0.8.8/radtools/crystal/bravais_lattice/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2412 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/bravais_lattice/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    14920 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/bravais_lattice/constructor.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4823 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/bravais_lattice/examples.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    20751 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/bravais_lattice/hs_points.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    20574 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/bravais_lattice/standardize.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     8854 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/bravais_lattice/variations.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5647 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/cell.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7098 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/constants.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    19795 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/crystal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    23815 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/identify.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    12416 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/kpoints.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    28091 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    37934 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/lattice_plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5396 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/crystal/properties.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-27 17:49:17.201375 rad-tools-0.8.8/radtools/decorate/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1002 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/decorate/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    15109 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/decorate/array.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2328 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/decorate/axes.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1408 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/decorate/colormap.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7313 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/decorate/stats.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-27 17:49:17.205039 rad-tools-0.8.8/radtools/dos/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1128 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/dos/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    31025 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/dos/dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     8815 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/dos/fatbands_plotting.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18768 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/dos/pdos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    11440 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/dos/pdos_plotting.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9250 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/dos/plotting.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2094 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/exceptions.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    11658 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/geometry.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-27 17:49:17.206991 rad-tools-0.8.8/radtools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1307 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    13889 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7495 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/io/tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9711 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/io/vampire.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     8655 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/io/vasp.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-27 17:49:17.210261 rad-tools-0.8.8/radtools/magnons/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1010 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/magnons/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4660 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/magnons/diagonalization.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    11533 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/magnons/dispersion.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3122 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/numerical.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-27 17:49:17.214237 rad-tools-0.8.8/radtools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2598 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7829 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/score/extract_tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5702 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/score/identify_wannier_centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9566 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/score/make_template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    13823 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/score/plot_dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    10765 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/score/plot_fatbands.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    16715 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/score/plot_tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18332 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/score/plot_tb2j_magnons.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-27 17:49:17.217583 rad-tools-0.8.8/radtools/spinham/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1129 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/spinham/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1734 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/spinham/constants.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    33551 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/spinham/hamiltonian.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    22263 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/spinham/parameter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2003 2023-09-27 17:49:11.000000 rad-tools-0.8.8/radtools/spinham/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-27 17:49:17.223143 rad-tools-0.8.8/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.8.8/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2951 2023-09-27 15:53:36.000000 rad-tools-0.8.8/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-08-24 10:46:21.000000 rad-tools-0.8.8/scripts/rad-extract-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-08-24 10:46:21.000000 rad-tools-0.8.8/scripts/rad-identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-08-24 10:46:21.000000 rad-tools-0.8.8/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-08-24 10:46:21.000000 rad-tools-0.8.8/scripts/rad-plot-dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-08-24 10:46:21.000000 rad-tools-0.8.8/scripts/rad-plot-fatbands.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      261 2023-08-24 10:46:21.000000 rad-tools-0.8.8/scripts/rad-plot-tb2j-magnons.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-08-24 10:46:21.000000 rad-tools-0.8.8/scripts/rad-plot-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-09-27 17:49:17.224430 rad-tools-0.8.8/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1497 2023-09-26 09:00:20.000000 rad-tools-0.8.8/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-30 23:32:46.322388 rad-tools-0.8.9/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    35149 2023-09-20 00:56:50.000000 rad-tools-0.8.9/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2961 2023-09-30 23:32:46.321334 rad-tools-0.8.9/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2252 2023-09-30 23:24:40.000000 rad-tools-0.8.9/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-30 23:32:46.277833 rad-tools-0.8.9/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2961 2023-09-30 23:32:46.000000 rad-tools-0.8.9/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2104 2023-09-30 23:32:46.000000 rad-tools-0.8.9/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-09-30 23:32:46.000000 rad-tools-0.8.9/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-09-30 23:32:46.000000 rad-tools-0.8.9/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-09-30 23:32:46.000000 rad-tools-0.8.9/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-30 23:32:46.281554 rad-tools-0.8.9/radtools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1724 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1235 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/__main__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    35945 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/_license.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1031 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/_osfix.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      976 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/constants.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-30 23:32:46.287652 rad-tools-0.8.9/radtools/crystal/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1427 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    10726 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/atom.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-30 23:32:46.292890 rad-tools-0.8.9/radtools/crystal/bravais_lattice/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2411 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/bravais_lattice/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    14919 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/bravais_lattice/constructor.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4822 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/bravais_lattice/examples.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    20750 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/bravais_lattice/hs_points.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    20573 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/bravais_lattice/standardize.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     8853 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/bravais_lattice/variations.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5646 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/cell.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7097 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/constants.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    19794 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/crystal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23814 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/identify.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    12415 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/kpoints.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    28090 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    37935 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/lattice_plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5395 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/crystal/properties.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-30 23:32:46.295940 rad-tools-0.8.9/radtools/decorate/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1001 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/decorate/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    15108 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/decorate/array.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2327 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/decorate/axes.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1407 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/decorate/colormap.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7312 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/decorate/stats.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-30 23:32:46.300265 rad-tools-0.8.9/radtools/dos/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1127 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/dos/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    31084 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/dos/dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     8814 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/dos/fatbands_plotting.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18767 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/dos/pdos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    11439 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/dos/pdos_plotting.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9249 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/dos/plotting.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2093 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/exceptions.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    11657 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/geometry.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-30 23:32:46.303061 rad-tools-0.8.9/radtools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1306 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    13889 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7494 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/io/tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9710 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/io/vampire.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     8656 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/io/vasp.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-30 23:32:46.304845 rad-tools-0.8.9/radtools/magnons/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1009 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/magnons/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4659 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/magnons/diagonalization.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    11532 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/magnons/dispersion.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3121 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/numerical.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-30 23:32:46.311714 rad-tools-0.8.9/radtools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2597 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7796 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/score/extract_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5700 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/score/identify_wannier_centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9565 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/score/make_template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    13821 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/score/plot_dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    10763 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/score/plot_fatbands.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    16714 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/score/plot_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    19385 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/score/plot_tb2j_magnons.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-30 23:32:46.314244 rad-tools-0.8.9/radtools/spinham/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1128 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/spinham/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1733 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/spinham/constants.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    33550 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/spinham/hamiltonian.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    22262 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/spinham/parameter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2002 2023-09-30 23:32:34.000000 rad-tools-0.8.9/radtools/spinham/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-09-30 23:32:46.320794 rad-tools-0.8.9/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.8.9/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2951 2023-09-27 15:53:36.000000 rad-tools-0.8.9/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-08-24 10:46:21.000000 rad-tools-0.8.9/scripts/rad-extract-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-08-24 10:46:21.000000 rad-tools-0.8.9/scripts/rad-identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-08-24 10:46:21.000000 rad-tools-0.8.9/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-08-24 10:46:21.000000 rad-tools-0.8.9/scripts/rad-plot-dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-08-24 10:46:21.000000 rad-tools-0.8.9/scripts/rad-plot-fatbands.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      261 2023-08-24 10:46:21.000000 rad-tools-0.8.9/scripts/rad-plot-tb2j-magnons.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-08-24 10:46:21.000000 rad-tools-0.8.9/scripts/rad-plot-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-09-30 23:32:46.322502 rad-tools-0.8.9/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1497 2023-09-26 09:00:20.000000 rad-tools-0.8.9/setup.py
```

### Comparing `rad-tools-0.8.8/LICENSE.txt` & `rad-tools-0.8.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.8.8/PKG-INFO` & `rad-tools-0.8.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.8.8
+Version: 0.8.9
 Summary: Spin Hamiltonians, magnons and condense matter post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
@@ -20,31 +20,34 @@
 *********
 RAD-TOOLS
 *********
 Spin Hamiltonians, magnons and condense matter post-processing.
 
 .. image:: https://badge.fury.io/py/rad-tools.svg
     :target: https://badge.fury.io/py/rad-tools
-    
+
 .. image:: https://readthedocs.org/projects/rad-tools/badge/?version=stable
     :target: https://rad-tools.org/en/stable/?badge=stable
     :alt: Documentation Status
-   
+
 .. image:: https://static.pepy.tech/personalized-badge/rad-tools?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads
  :target: https://pepy.tech/project/rad-tools
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
-   
+
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=505050
+    :target: https://pycqa.github.io/isort/
+
 .. image:: https://img.shields.io/github/license/adrybakov/rad-tools
    :alt: GitHub
 
-The package covers post-processing scenarios for the results of 
-`Quantum Espresso <https://www.quantum-espresso.org>`_, 
-`TB2J <https://tb2j.readthedocs.io/en/latest/>`_ 
+The package covers post-processing scenarios for the results of
+`Quantum Espresso <https://www.quantum-espresso.org>`_,
+`TB2J <https://tb2j.readthedocs.io/en/latest/>`_
 and `Wannier90 <http://www.wannier.org/>`_, as well as provides some custom scripts.
 
 It is expected to be used in two ways:
 
 * As Python library
 
 * Via scripts (i.e. usage from command line)
@@ -53,15 +56,15 @@
 `documentation. <https://rad-tools.org>`_
 
 Installation
 ============
 
 Requirement for RAD-tools installation are:
 
-* Python itself (>=3.8)
+* Python (>=3.8)
 * NumPy
 * SciPy
 * matplotlib
 * tqdm
 * termcolor
 
 RAD-tools can be installed with ``pip`` or from source.
@@ -92,15 +95,15 @@
 
 * To install RAD-tools, run (you may need to use ``pip3``):
 
 .. code-block:: console
 
    pip install rad-tools
 
-Additionally you may run the unit tests, 
+Additionally you may run the unit tests,
 which requires pytest (requires Python 3.7+) to be installed:
 
 .. code-block:: console
 
    make test
 
 To install pytest, run (you may need to use ``pip3``):
```

### Comparing `rad-tools-0.8.8/README.rst` & `rad-tools-0.8.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 *********
 RAD-TOOLS
 *********
 Spin Hamiltonians, magnons and condense matter post-processing.
 
 .. image:: https://badge.fury.io/py/rad-tools.svg
     :target: https://badge.fury.io/py/rad-tools
-    
+
 .. image:: https://readthedocs.org/projects/rad-tools/badge/?version=stable
     :target: https://rad-tools.org/en/stable/?badge=stable
     :alt: Documentation Status
-   
+
 .. image:: https://static.pepy.tech/personalized-badge/rad-tools?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads
  :target: https://pepy.tech/project/rad-tools
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
-   
+
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=505050
+    :target: https://pycqa.github.io/isort/
+
 .. image:: https://img.shields.io/github/license/adrybakov/rad-tools
    :alt: GitHub
 
-The package covers post-processing scenarios for the results of 
-`Quantum Espresso <https://www.quantum-espresso.org>`_, 
-`TB2J <https://tb2j.readthedocs.io/en/latest/>`_ 
+The package covers post-processing scenarios for the results of
+`Quantum Espresso <https://www.quantum-espresso.org>`_,
+`TB2J <https://tb2j.readthedocs.io/en/latest/>`_
 and `Wannier90 <http://www.wannier.org/>`_, as well as provides some custom scripts.
 
 It is expected to be used in two ways:
 
 * As Python library
 
 * Via scripts (i.e. usage from command line)
@@ -34,15 +37,15 @@
 `documentation. <https://rad-tools.org>`_
 
 Installation
 ============
 
 Requirement for RAD-tools installation are:
 
-* Python itself (>=3.8)
+* Python (>=3.8)
 * NumPy
 * SciPy
 * matplotlib
 * tqdm
 * termcolor
 
 RAD-tools can be installed with ``pip`` or from source.
@@ -73,15 +76,15 @@
 
 * To install RAD-tools, run (you may need to use ``pip3``):
 
 .. code-block:: console
 
    pip install rad-tools
 
-Additionally you may run the unit tests, 
+Additionally you may run the unit tests,
 which requires pytest (requires Python 3.7+) to be installed:
 
 .. code-block:: console
 
    make test
 
 To install pytest, run (you may need to use ``pip3``):
```

### Comparing `rad-tools-0.8.8/rad_tools.egg-info/PKG-INFO` & `rad-tools-0.8.9/rad_tools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.8.8
+Version: 0.8.9
 Summary: Spin Hamiltonians, magnons and condense matter post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
@@ -20,31 +20,34 @@
 *********
 RAD-TOOLS
 *********
 Spin Hamiltonians, magnons and condense matter post-processing.
 
 .. image:: https://badge.fury.io/py/rad-tools.svg
     :target: https://badge.fury.io/py/rad-tools
-    
+
 .. image:: https://readthedocs.org/projects/rad-tools/badge/?version=stable
     :target: https://rad-tools.org/en/stable/?badge=stable
     :alt: Documentation Status
-   
+
 .. image:: https://static.pepy.tech/personalized-badge/rad-tools?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads
  :target: https://pepy.tech/project/rad-tools
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
-   
+
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=505050
+    :target: https://pycqa.github.io/isort/
+
 .. image:: https://img.shields.io/github/license/adrybakov/rad-tools
    :alt: GitHub
 
-The package covers post-processing scenarios for the results of 
-`Quantum Espresso <https://www.quantum-espresso.org>`_, 
-`TB2J <https://tb2j.readthedocs.io/en/latest/>`_ 
+The package covers post-processing scenarios for the results of
+`Quantum Espresso <https://www.quantum-espresso.org>`_,
+`TB2J <https://tb2j.readthedocs.io/en/latest/>`_
 and `Wannier90 <http://www.wannier.org/>`_, as well as provides some custom scripts.
 
 It is expected to be used in two ways:
 
 * As Python library
 
 * Via scripts (i.e. usage from command line)
@@ -53,15 +56,15 @@
 `documentation. <https://rad-tools.org>`_
 
 Installation
 ============
 
 Requirement for RAD-tools installation are:
 
-* Python itself (>=3.8)
+* Python (>=3.8)
 * NumPy
 * SciPy
 * matplotlib
 * tqdm
 * termcolor
 
 RAD-tools can be installed with ``pip`` or from source.
@@ -92,15 +95,15 @@
 
 * To install RAD-tools, run (you may need to use ``pip3``):
 
 .. code-block:: console
 
    pip install rad-tools
 
-Additionally you may run the unit tests, 
+Additionally you may run the unit tests,
 which requires pytest (requires Python 3.7+) to be installed:
 
 .. code-block:: console
 
    make test
 
 To install pytest, run (you may need to use ``pip3``):
```

### Comparing `rad-tools-0.8.8/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.8.9/rad_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.8.8/radtools/__init__.py` & `rad-tools-0.8.9/radtools/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -12,22 +12,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-r""" 
+r"""
 RAD-tools
 """
 
-__version__ = "0.8.8"
+__version__ = "0.8.9"
 __doclink__ = "rad-tools.org"
-__git_hash__ = "9f889b599b9d334c4e4954631eb7dac28d6e13d4"
-__release_date__ = "27 September 2023"
+__git_hash__ = "cc3621d7b4bfcc1cb416f53106e24f21986dbfdb"
+__release_date__ = "1 October 2023"
 
 
 from . import (
     constants,
     crystal,
     decorate,
     dos,
```

### Comparing `rad-tools-0.8.8/radtools/__main__.py` & `rad-tools-0.8.9/radtools/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from argparse import ArgumentParser
 
-from radtools.decorate.stats import logo, license
+from radtools.decorate.stats import license, logo
 
 if __name__ == "__main__":
     parser = ArgumentParser(
         description="RAD-tools package",
     )
     parser.add_argument(
         "--license",
```

### Comparing `rad-tools-0.8.8/radtools/_license.py` & `rad-tools-0.8.9/radtools/_license.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -686,8 +686,8 @@
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
-"""
+"""
```

### Comparing `rad-tools-0.8.8/radtools/_osfix.py` & `rad-tools-0.8.9/radtools/_osfix.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/constants.py` & `rad-tools-0.8.9/radtools/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/__init__.py` & `rad-tools-0.8.9/radtools/crystal/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -25,16 +25,16 @@
 from .atom import Atom
 from .bravais_lattice import *
 from .constants import *
 from .crystal import Crystal
 from .identify import *
 from .kpoints import *
 from .lattice import *
-from .properties import *
 from .lattice_plotter import *
+from .properties import *
 
 __all__ = ["Atom", "Crystal", "Cell", "crystal_constants"]
 __all__.extend(bravais_lattice.__all__)
 __all__.extend(lattice.__all__)
 __all__.extend(kpoints.__all__)
 __all__.extend(identify.__all__)
 __all__.extend(properties.__all__)
```

### Comparing `rad-tools-0.8.8/radtools/crystal/atom.py` & `rad-tools-0.8.9/radtools/crystal/atom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/bravais_lattice/__init__.py` & `rad-tools-0.8.9/radtools/crystal/bravais_lattice/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/bravais_lattice/constructor.py` & `rad-tools-0.8.9/radtools/crystal/bravais_lattice/constructor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/bravais_lattice/examples.py` & `rad-tools-0.8.9/radtools/crystal/bravais_lattice/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/bravais_lattice/hs_points.py` & `rad-tools-0.8.9/radtools/crystal/bravais_lattice/hs_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/bravais_lattice/standardize.py` & `rad-tools-0.8.9/radtools/crystal/bravais_lattice/standardize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/bravais_lattice/variations.py` & `rad-tools-0.8.9/radtools/crystal/bravais_lattice/variations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/cell.py` & `rad-tools-0.8.9/radtools/crystal/cell.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/constants.py` & `rad-tools-0.8.9/radtools/crystal/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/crystal.py` & `rad-tools-0.8.9/radtools/crystal/crystal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/identify.py` & `rad-tools-0.8.9/radtools/crystal/identify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/kpoints.py` & `rad-tools-0.8.9/radtools/crystal/kpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/lattice.py` & `rad-tools-0.8.9/radtools/crystal/lattice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/crystal/lattice_plotter.py` & `rad-tools-0.8.9/radtools/crystal/lattice_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -12,24 +12,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+from random import choices
+from string import ascii_lowercase
+from typing import Iterable
+
 import matplotlib.pyplot as plt
+import numpy as np
+from matplotlib import rcParams
 from matplotlib.patches import FancyArrowPatch
 from mpl_toolkits.mplot3d import Axes3D, proj3d
-from matplotlib import rcParams
-import numpy as np
-from radtools.geometry import volume
+
 from radtools.crystal.constants import HS_PLOT_NAMES
-from typing import Iterable
-from random import choices
-from string import ascii_lowercase
+from radtools.geometry import volume
 
 try:
     import plotly.graph_objects as go
 
     PLOTLY_AVAILABLE = True
 except ImportError:
     PLOTLY_AVAILABLE = False
```

### Comparing `rad-tools-0.8.8/radtools/crystal/properties.py` & `rad-tools-0.8.9/radtools/crystal/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/decorate/__init__.py` & `rad-tools-0.8.9/radtools/decorate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/decorate/array.py` & `rad-tools-0.8.9/radtools/decorate/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/decorate/axes.py` & `rad-tools-0.8.9/radtools/decorate/axes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/decorate/colormap.py` & `rad-tools-0.8.9/radtools/decorate/colormap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/decorate/stats.py` & `rad-tools-0.8.9/radtools/decorate/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/dos/__init__.py` & `rad-tools-0.8.9/radtools/dos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/dos/dos.py` & `rad-tools-0.8.9/radtools/dos/dos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -133,15 +133,17 @@
         * Non-collinear, spin-orbit:
             E DOS(E) PDOS(E)
         """
 
         # Detect the case
         if self._case is None:
             # Read header
-            with open(join(f"{self._input_folder}", f"{self.seedname}.pdos_tot")) as file:
+            with open(
+                join(f"{self._input_folder}", f"{self.seedname}.pdos_tot")
+            ) as file:
                 header = file.readline().lower().split()
 
             if "dos(e)" in header and "pdos(e)" in header:
                 self._case = 1
             if "dos(e)" in header and "pdosup(e)" in header and "pdosdw(e)" in header:
                 self._case = 3
             if (
@@ -196,15 +198,17 @@
     def k_resolved(self):
         r"""
         Whether DOS is k-resolved.
         """
 
         if self._k_resolved is None:
             # Check for k-resolved
-            with open(join(f"{self._input_folder}", f"{self.seedname}.pdos_tot")) as file:
+            with open(
+                join(f"{self._input_folder}", f"{self.seedname}.pdos_tot")
+            ) as file:
                 self._k_resolved = "ik" in file.readline().lower().split()
 
         return self._k_resolved
 
     def _extract_energy(self):
         # Load data
         dos = np.loadtxt(
```

### Comparing `rad-tools-0.8.8/radtools/dos/fatbands_plotting.py` & `rad-tools-0.8.9/radtools/dos/fatbands_plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/dos/pdos.py` & `rad-tools-0.8.9/radtools/dos/pdos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/dos/pdos_plotting.py` & `rad-tools-0.8.9/radtools/dos/pdos_plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/dos/plotting.py` & `rad-tools-0.8.9/radtools/dos/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/exceptions.py` & `rad-tools-0.8.9/radtools/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/geometry.py` & `rad-tools-0.8.9/radtools/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/io/__init__.py` & `rad-tools-0.8.9/radtools/io/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/io/internal.py` & `rad-tools-0.8.9/radtools/io/internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -25,19 +25,20 @@
     "read_template",
     "dump_spinham_txt",
     "dump_pickle",
     "load_pickle",
 ]
 
 import numpy as np
-from radtools.spinham.template import ExchangeTemplate
+
 from radtools.decorate.array import print_2d_array
 from radtools.decorate.stats import logo
 from radtools.spinham.constants import TXT_FLAGS
 from radtools.spinham.hamiltonian import SpinHamiltonian
+from radtools.spinham.template import ExchangeTemplate
 
 meV_TO_J = 1.602176634e-22
 
 
 def dump_pickle(object, filename):
     """
     Save any python Object in a binary format.
```

### Comparing `rad-tools-0.8.8/radtools/io/tb2j.py` & `rad-tools-0.8.9/radtools/io/tb2j.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/io/vampire.py` & `rad-tools-0.8.9/radtools/io/vampire.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -19,16 +19,16 @@
 r"""
 Input-output for |Vampire|_.
 """
 
 __all__ = ["dump_vampire", "dump_mat", "dump_ucf"]
 
 from radtools.decorate.array import print_2d_array
-from radtools.spinham.parameter import ExchangeParameter
 from radtools.decorate.stats import logo
+from radtools.spinham.parameter import ExchangeParameter
 
 meV_TO_J = 1.602176634e-22
 
 
 def dump_vampire(
     spinham,
     seedname="vampire",
```

### Comparing `rad-tools-0.8.8/radtools/io/vasp.py` & `rad-tools-0.8.9/radtools/io/vasp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -13,19 +13,21 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import os
+
 import numpy as np
-from radtools.decorate.array import print_2d_array
-from radtools.geometry import volume, absolute_to_relative
+
 from radtools.crystal.atom import Atom
 from radtools.crystal.crystal import Crystal
+from radtools.decorate.array import print_2d_array
+from radtools.geometry import absolute_to_relative, volume
 
 __all__ = ["load_poscar", "dump_poscar"]
 
 
 def load_poscar(file_object=None, return_crystal=True, return_comment=False):
     r"""
     Read the crystal structure from the |POSCAR|_ file.
@@ -232,15 +234,15 @@
             atom_coordinates, fmt=f".{decimals}f", print_result=False, borders=False
         )
         + "\n"
     )
 
 
 if __name__ == "__main__":
-    from radtools import Crystal, HEX
+    from radtools import HEX, Crystal
 
     c = Crystal(HEX(1, 2))
     c.add_atom("Cr2", position=[0.5, 0, 0])
     c.add_atom("C2", position=[0, 0, 0])
     c.add_atom("C1", position=[0, 0, 0.5])
     c.add_atom("C3", position=[0, 0.5, 0])
     c.add_atom("Cr1", position=[0, 0.5, 0.5])
```

### Comparing `rad-tools-0.8.8/radtools/magnons/__init__.py` & `rad-tools-0.8.9/radtools/magnons/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/magnons/diagonalization.py` & `rad-tools-0.8.9/radtools/magnons/diagonalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/magnons/dispersion.py` & `rad-tools-0.8.9/radtools/magnons/dispersion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/numerical.py` & `rad-tools-0.8.9/radtools/numerical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/score/__init__.py` & `rad-tools-0.8.9/radtools/score/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/score/extract_tb2j.py` & `rad-tools-0.8.9/radtools/score/extract_tb2j.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -12,22 +12,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from argparse import ArgumentParser
 import os
+from argparse import ArgumentParser
 
 from termcolor import cprint
 
-from radtools.io.internal import load_template
+from radtools.io.internal import dump_spinham_txt, load_template
 from radtools.io.tb2j import load_tb2j_model
-from radtools.io.internal import dump_spinham_txt
 
 
 def manager(
     input_filename,
     template_file=None,
     output_name=None,
     decimals=4,
```

### Comparing `rad-tools-0.8.8/radtools/score/identify_wannier_centres.py` & `rad-tools-0.8.9/radtools/score/identify_wannier_centres.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -12,16 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from argparse import ArgumentParser
 import os
+from argparse import ArgumentParser
 
 import numpy as np
 from termcolor import cprint
 
 
 def manager(input_filename, span=0.1, output_name=""):
     r"""
@@ -155,15 +155,15 @@
     parser = ArgumentParser()
     parser.add_argument(
         "-if",
         "--input-filename",
         required=True,
         metavar="filename",
         type=str,
-        help='Relative or absolute path to the "*_centres.xyz" file',
+        help='Relative or absolute path to the "_centres.xyz" file',
     )
     parser.add_argument(
         "-s",
         "--span",
         default=0.1,
         type=float,
         help="Distance tolerance between centre and atom. (in Angstroms)",
```

### Comparing `rad-tools-0.8.8/radtools/score/make_template.py` & `rad-tools-0.8.9/radtools/score/make_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -12,25 +12,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+import os
 from argparse import ArgumentParser
 from calendar import month_name
 from datetime import datetime
-import os
 
 import numpy as np
 from termcolor import cprint
 
 from radtools import __version__ as version
-from radtools.io.tb2j import load_tb2j_model
 from radtools.decorate.stats import logo
+from radtools.io.tb2j import load_tb2j_model
 
 
 def manager(
     output_name="template.txt",
     input_filename=None,
     R_vector=None,
     max_distance=None,
```

### Comparing `rad-tools-0.8.8/radtools/score/plot_dos.py` & `rad-tools-0.8.9/radtools/score/plot_dos.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -12,16 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from argparse import ArgumentParser
 import os
+from argparse import ArgumentParser
 
 from termcolor import cprint
 
 from radtools.dos.dos import DOSQE, detect_seednames
 from radtools.dos.pdos_plotting import (
     plot_atom_resolved,
     plot_atom_to_total,
@@ -312,165 +312,164 @@
             plot_atom_to_total(dos=dos, **pdos_parameters, separate=separate)
         # Plot custom plot
         else:
             plot_custom_pdos(dos=dos, custom=custom, **pdos_parameters, labels=labels)
 
 
 def create_parser():
-
     parser = ArgumentParser()
     parser.add_argument(
         "-if",
         "--input-folder",
         default=".",
         metavar="path",
         type=str,
-        help='Relative or absolute path to the folder with PDOS files.',
+        help="Relative or absolute path to the folder with PDOS files.",
     )
     parser.add_argument(
         "-s",
         "--seedname",
         default=None,
         metavar="name",
         type=str,
-        help='Prefix for input files with PDOS(E).',
+        help="Prefix for input files with PDOS(E).",
     )
     parser.add_argument(
         "-on",
         "--output-name",
         default="",
         metavar="path",
         type=str,
-        help='Relative or absolute path to the folder for saving outputs.',
+        help="Relative or absolute path to the folder for saving outputs.",
     )
     parser.add_argument(
         "-ew",
         "--energy-window",
         default=None,
         metavar=("min", "max"),
         type=float,
         nargs=2,
-        help='Energy window for the plots.',
+        help="Energy window for the plots.",
     )
     parser.add_argument(
         "-dw",
         "--dos-window",
         default=None,
         metavar=("min", "max"),
         type=float,
         nargs=2,
-        help='DOS window for the plots.',
+        help="DOS window for the plots.",
     )
     parser.add_argument(
         "-ef",
         "--efermi",
         default=0.0,
         metavar="energy",
         type=float,
-        help='Fermi energy.',
+        help="Fermi energy.",
     )
     parser.add_argument(
         "-sep",
         "--separate",
         default=False,
         action="store_true",
-        help='Whether to plot projected DOS for each atom of the same type separately.',
+        help="Whether to plot projected DOS for each atom of the same type separately.",
     )
     parser.add_argument(
         "-r",
         "--relative",
         default=False,
         action="store_true",
-        help='Whether to use relative style.',
+        help="Whether to use relative style.",
     )
     parser.add_argument(
         "-n",
         "--normalize",
         default=False,
         action="store_true",
-        help='Whether to normalized PDOS values to 1.',
+        help="Whether to normalized PDOS values to 1.",
     )
     parser.add_argument(
         "-v",
         "--verbose",
         default=False,
         action="store_true",
-        help='Verbose output, propagates to the called methods.',
+        help="Verbose output, propagates to the called methods.",
     )
     parser.add_argument(
         "-i",
         "--interactive",
         default=False,
         action="store_true",
-        help='Interactive plotting.',
+        help="Interactive plotting.",
     )
     parser.add_argument(
         "-sp",
         "--save-pickle",
         default=False,
         action="store_true",
-        help='Whether to save figures as .pickle files.',
+        help="Whether to save figures as .pickle files.",
     )
     parser.add_argument(
         "-st",
         "--save-txt",
         default=False,
         action="store_true",
-        help='Whether to save some data as txt files.',
+        help="Whether to save some data as txt files.",
     )
     parser.add_argument(
         "-bt",
         "--background-total",
         default=False,
         action="store_true",
-        help='Whether to use total PDOS as the background for all plots.',
+        help="Whether to use total PDOS as the background for all plots.",
     )
     parser.add_argument(
         "--custom",
         default=None,
         metavar="description",
         type=str,
         nargs="*",
-        help='Custom PDOS plot. See :ref:`rad-plot-dos_custom-plots` for info.',
+        help="Custom PDOS plot. See :ref:`rad-plot-dos_custom-plots` for info.",
     )
     parser.add_argument(
         "-cls",
         "--colours",
         default=None,
         type=str,
         nargs="*",
-        help='Colours for the relative and custom plots.',
+        help="Colours for the relative and custom plots.",
     )
     parser.add_argument(
         "-lbs",
         "--labels",
         default=None,
         type=str,
         nargs="*",
-        help='Labels for the custom plots.',
+        help="Labels for the custom plots.",
     )
     parser.add_argument(
         "-lfs",
         "--legend-fontsize",
         default=12,
         metavar="fontsize",
         type=int,
-        help='Fontsize of the legend.',
+        help="Fontsize of the legend.",
     )
     parser.add_argument(
         "-alfs",
         "--axes-labels-fontsize",
         default=14,
         metavar="fontsize",
         type=int,
-        help='Fontsize of the labes of the axes.',
+        help="Fontsize of the labes of the axes.",
     )
     parser.add_argument(
         "-tfs",
         "--title-fontsize",
         default=18,
         metavar="fontsize",
         type=int,
-        help='Fontsize of the title.',
+        help="Fontsize of the title.",
     )
 
     return parser
```

### Comparing `rad-tools-0.8.8/radtools/score/plot_fatbands.py` & `rad-tools-0.8.9/radtools/score/plot_fatbands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -12,16 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from argparse import ArgumentParser
 import os
+from argparse import ArgumentParser
 
 from termcolor import cprint
 
 from radtools.dos.dos import DOSQE, detect_seednames
 from radtools.dos.fatbands_plotting import plot_custom_fatbands
 from radtools.dos.plotting import COLOURS
 
@@ -226,153 +226,152 @@
             axes_labels_fontsize=axes_labels_fontsize,
             title_fontsize=title_fontsize,
             k_points=k_points,
         )
 
 
 def create_parser():
-
     parser = ArgumentParser()
     parser.add_argument(
         "-if",
         "--input-folder",
         default=".",
         metavar="path",
         type=str,
-        help='Relative or absolute path to the folder with PDOS files.',
+        help="Relative or absolute path to the folder with PDOS files.",
     )
     parser.add_argument(
         "-s",
         "--seedname",
         default=None,
         metavar="name",
         type=str,
-        help='Prefix for input files with PDOS(E).',
+        help="Prefix for input files with PDOS(E).",
     )
     parser.add_argument(
         "-on",
         "--output-name",
         default="",
         metavar="path",
         type=str,
-        help='Relative or absolute path to the folder for saving outputs.',
+        help="Relative or absolute path to the folder for saving outputs.",
     )
     parser.add_argument(
         "-ew",
         "--energy-window",
         default=None,
         metavar=("min", "max"),
         type=float,
         nargs=2,
-        help='Energy window for the plots.',
+        help="Energy window for the plots.",
     )
     parser.add_argument(
         "-kw",
         "--k-window",
         default=None,
         metavar=("min", "max"),
         type=float,
         nargs=2,
-        help='K-point window for the plots.',
+        help="K-point window for the plots.",
     )
     parser.add_argument(
         "-ef",
         "--efermi",
         default=0.0,
         metavar="energy",
         type=float,
-        help='Fermi energy.',
+        help="Fermi energy.",
     )
     parser.add_argument(
         "-v",
         "--verbose",
         default=False,
         action="store_true",
-        help='Verbose output, propagates to the called methods.',
+        help="Verbose output, propagates to the called methods.",
     )
     parser.add_argument(
         "-i",
         "--interactive",
         default=False,
         action="store_true",
-        help='Interactive plotting.',
+        help="Interactive plotting.",
     )
     parser.add_argument(
         "-sep",
         "--separate",
         default=False,
         action="store_true",
-        help='Whether to plot projected DOS for each atom of the same type separately.',
+        help="Whether to plot projected DOS for each atom of the same type separately.",
     )
     parser.add_argument(
         "-sp",
         "--save-pickle",
         default=False,
         action="store_true",
-        help='Whether to save figures as .pickle files.',
+        help="Whether to save figures as .pickle files.",
     )
     parser.add_argument(
         "-st",
         "--save-txt",
         default=False,
         action="store_true",
-        help='Whether to save some data as txt files.',
+        help="Whether to save some data as txt files.",
     )
     parser.add_argument(
         "--custom",
         default=None,
         metavar="description",
         type=str,
         nargs="*",
-        help='Custom PDOS plot.',
+        help="Custom PDOS plot.",
     )
     parser.add_argument(
         "-cls",
         "--colours",
         default=None,
         type=str,
         nargs="*",
-        help='Colours for the relative and custom plots.',
+        help="Colours for the relative and custom plots.",
     )
     parser.add_argument(
         "-lbs",
         "--labels",
         default=None,
         type=str,
         nargs="*",
-        help='Labels for the custom plots.',
+        help="Labels for the custom plots.",
     )
     parser.add_argument(
         "-lfs",
         "--legend-fontsize",
         default=12,
         metavar="fontsize",
         type=int,
-        help='Fontsize of the legend.',
+        help="Fontsize of the legend.",
     )
     parser.add_argument(
         "-alfs",
         "--axes-labels-fontsize",
         default=14,
         metavar="fontsize",
         type=int,
-        help='Fontsize of the labes of the axes.',
+        help="Fontsize of the labes of the axes.",
     )
     parser.add_argument(
         "-tfs",
         "--title-fontsize",
         default=18,
         metavar="fontsize",
         type=int,
-        help='Fontsize of the title.',
+        help="Fontsize of the title.",
     )
     parser.add_argument(
         "-kp",
         "--k-points",
         default=None,
         metavar="G 0.23 K 0.64 Y 1.2 ...",
         type=str,
         nargs="*",
-        help='Plot coordinates of high symmetry points.',
+        help="Plot coordinates of high symmetry points.",
     )
 
     return parser
```

### Comparing `rad-tools-0.8.8/radtools/score/plot_tb2j.py` & `rad-tools-0.8.9/radtools/score/plot_tb2j.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -12,17 +12,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+import os
 from argparse import ArgumentParser
 from math import asin, pi, sqrt
-import os
 
 import numpy as np
 from matplotlib import pyplot as plt
 from termcolor import cprint
 
 from radtools.constants import TODEGREES
 from radtools.io.internal import load_template
```

### Comparing `rad-tools-0.8.8/radtools/score/plot_tb2j_magnons.py` & `rad-tools-0.8.9/radtools/score/plot_tb2j_magnons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -12,37 +12,38 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from argparse import ArgumentParser
 import os
+from argparse import ArgumentParser
 
 import matplotlib.pyplot as plt
 import numpy as np
 from termcolor import cprint
 
+from radtools.decorate.array import print_2d_array
+from radtools.decorate.axes import plot_hlines
+from radtools.decorate.stats import logo
 from radtools.io.internal import load_template
 from radtools.io.tb2j import load_tb2j_model
 from radtools.magnons.dispersion import MagnonDispersion
-from radtools.decorate.stats import logo
 from radtools.spinham.constants import TXT_FLAGS
-from radtools.decorate.array import print_2d_array
-from radtools.decorate.axes import plot_hlines
 
 
 def manager(
     input_filename,
     spin,
     template_file=None,
     output_name="magnon_dispersion",
     spiral_vector=None,
     rotation_axis=None,
+    k_points=None,
     k_path=None,
     form_model=False,
     R_vector=None,
     max_distance=None,
     min_distance=None,
     save_txt=False,
     interactive=False,
@@ -68,15 +69,15 @@
         Console argument: ``-if`` / ``--input-filename``
 
         Metavar: "filename"
     spin : list of str, optional
         Spin of the atoms in the model.
 
         For each atom, which has at least one bond connected to it is necessary to specify
-        spin vector. The spin vector is specified in the form of atom`s name followed by
+        spin vector. The spin vector is specified in the form of atom's name followed by
         three numbers, separated by spaces.
         The numbers represent the x, y, and z components of the spin vector.
 
         Console argument: ``-s`` / ``--spin``
 
         Metavar: "Atom S_x S_y S_z"
     template_file : str, optional
@@ -99,14 +100,24 @@
         Metavar: ("Q_x", "Q_y", "Q_z")
     rotation_axis : list of 3 float, optional
         Direction of global rotation axis. In absolute coordinates in real space.
 
         Console argument: ``-ra`` / ``--rotation-axis``
 
         Metavar: ("n_x", "n_y", "n_z")
+    k_points : list of str, optional
+        Additional high-symmetry k-points.
+
+        Coordinates are relative to the reciprocal cell.
+
+        .. versionadded:: 0.8.9
+
+        Console argument: ``-kps`` / ``--k-points``
+
+        Metavar: "name label xrel yrel zrel ..."
     k_path : str, optional
         Path in reciprocal space for the magnon dispersion.
 
         Console argument: ``-kp`` / ``--k-path``
 
         Metavar: "G-X-M-G|G-Y"
     form_model : bool, default False
@@ -216,14 +227,25 @@
         input_filename, quiet=not verbose, bravais_type=bravais_type
     )
 
     cprint(f"{spinham.variation} crystal detected", "green")
 
     # Get k points of the spinham
     kp = spinham.kpoints
+
+    # Add additional points
+    if k_points is not None:
+        for i in range(len(k_points) // 5):
+            point_name = k_points[5 * i]
+            point_label = k_points[5 * i + 1]
+            point_coordinates = list(map(float, k_points[5 * i + 2 : 5 * i + 5]))
+            kp.add_hs_point(
+                name=point_name, coordinates=point_coordinates, label=point_label
+            )
+
     # Set custom k path
     if k_path is not None:
         kp.path = k_path
 
     if verbose:
         print("Predefined high symmetry k points:")
         for name in kp.hs_names:
@@ -275,16 +297,19 @@
         1,
         transform=ax.get_xaxis_transform(),
         colors="black",
         alpha=0.5,
         lw=1,
         ls="dashed",
     )
+    colors = ["#174FD5", "#F8AB00", "#0CE1A2", "#FF003C", "#46EC00", "#9823C9"]
+    i = 0
     for omega in omegas:
-        ax.plot(kp.flatten_points(), omega)
+        ax.plot(kp.flatten_points(), omega, color=colors[i % len(colors)])
+        i += 1
 
     ax.set_xlim(kp.flatten_points()[0], kp.flatten_points()[-1])
     plot_hlines(ax, [0])
 
     if save_txt:
         main_separator = "=" * 80 + "\n"
         info = [
@@ -490,14 +515,23 @@
         default=None,
         metavar=("n_x", "n_y", "n_z"),
         type=float,
         nargs=3,
         help="Direction of global rotation axis. In absolute coordinates in real space.",
     )
     parser.add_argument(
+        "-kps",
+        "--k-points",
+        default=None,
+        metavar="name label xrel yrel zrel ...",
+        type=str,
+        nargs="*",
+        help="Additional high-symmetry k-points.",
+    )
+    parser.add_argument(
         "-kp",
         "--k-path",
         default=None,
         metavar="G-X-M-G|G-Y",
         type=str,
         help="Path in reciprocal space for the magnon dispersion.",
     )
```

### Comparing `rad-tools-0.8.8/radtools/spinham/__init__.py` & `rad-tools-0.8.9/radtools/spinham/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/spinham/constants.py` & `rad-tools-0.8.9/radtools/spinham/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/spinham/hamiltonian.py` & `rad-tools-0.8.9/radtools/spinham/hamiltonian.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/spinham/parameter.py` & `rad-tools-0.8.9/radtools/spinham/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/radtools/spinham/template.py` & `rad-tools-0.8.9/radtools/spinham/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAD-tools - program for spin Hamiltonian and magnons.
 # Copyright (C) 2022-2023  Andrey Rybakov
-# 
+#
 # e-mail: anry@uv.es, web: adrybakov.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `rad-tools-0.8.8/scripts/compute-energies.py` & `rad-tools-0.8.9/scripts/compute-energies.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.8.8/scripts/phonopy-plotter.py` & `rad-tools-0.8.9/scripts/phonopy-plotter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.8.8/setup.py` & `rad-tools-0.8.9/setup.py`

 * *Files identical despite different names*

