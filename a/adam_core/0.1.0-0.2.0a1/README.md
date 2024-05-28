# Comparing `tmp/adam_core-0.1.0.tar.gz` & `tmp/adam_core-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam_core-0.1.0.tar", last modified: Sun Jun 18 06:19:30 2023, max compression
+gzip compressed data, was "adam_core-0.2.0a1.tar", last modified: Tue May 28 18:15:50 2024, max compression
```

## Comparing `adam_core-0.1.0.tar` & `adam_core-0.2.0a1.tar`

### file list

```diff
@@ -1,86 +1,187 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.650369 adam_core-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-18 06:19:19.000000 adam_core-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-06-18 06:19:30.650369 adam_core-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-18 06:19:19.000000 adam_core-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.642369 adam_core-0.1.0/adam_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.646369 adam_core-0.1.0/adam_core/coordinates/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/cartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/cometary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/covariances.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/keplerian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/residuals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/spherical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.646369 adam_core-0.1.0/adam_core/coordinates/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/tests/test_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/tests/test_covariances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/tests/test_origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/tests/test_residuals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/tests/test_spherical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/tests/test_transforms_spherical.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/times.py
--rw-r--r--   0 runner    (1001) docker     (123)    46758 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/coordinates/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.646369 adam_core-0.1.0/adam_core/dynamics/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/dynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/dynamics/barker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/dynamics/kepler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.646369 adam_core-0.1.0/adam_core/dynamics/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/dynamics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/dynamics/tests/test_kepler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/dynamics/tests/test_tisserand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/dynamics/tisserand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.646369 adam_core-0.1.0/adam_core/orbits/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/orbits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/orbits/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/orbits/orbits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.646369 adam_core-0.1.0/adam_core/orbits/query/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/orbits/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/orbits/query/horizons.py
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/orbits/query/sbdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.646369 adam_core-0.1.0/adam_core/orbits/query/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/orbits/query/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/orbits/query/tests/test_sbdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.646369 adam_core-0.1.0/adam_core/orbits/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/orbits/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/orbits/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/orbits/tests/test_orbits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.646369 adam_core-0.1.0/adam_core/propagator/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/propagator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/propagator/propagator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/propagator/pyoorb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.646369 adam_core-0.1.0/adam_core/propagator/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/propagator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/propagator/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/propagator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.650369 adam_core-0.1.0/adam_core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.650369 adam_core-0.1.0/adam_core/utils/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/utils/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.650369 adam_core-0.1.0/adam_core/utils/helpers/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/utils/helpers/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17926 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/utils/helpers/data/sample_orbits.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/utils/helpers/orbits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.650369 adam_core-0.1.0/adam_core/utils/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/utils/helpers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/utils/helpers/tests/test_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/utils/mpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/utils/spice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.650369 adam_core-0.1.0/adam_core/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-06-18 06:19:19.000000 adam_core-0.1.0/adam_core/utils/tests/test_mpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:19:30.642369 adam_core-0.1.0/adam_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-06-18 06:19:30.000000 adam_core-0.1.0/adam_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-18 06:19:30.000000 adam_core-0.1.0/adam_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 06:19:30.000000 adam_core-0.1.0/adam_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-18 06:19:30.000000 adam_core-0.1.0/adam_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 06:19:30.000000 adam_core-0.1.0/adam_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-18 06:19:19.000000 adam_core-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-18 06:19:30.650369 adam_core-0.1.0/setup.cfg
+-rw-r--r--   0        0        0     2782 2024-05-28 17:05:15.871265 adam_core-0.2.0a1/LICENSE.md
+-rw-r--r--   0        0        0    12890 2024-05-28 17:06:44.754473 adam_core-0.2.0a1/README.md
+-rw-r--r--   0        0        0     2910 2024-05-28 18:15:50.395839 adam_core-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-05-28 17:06:44.754921 adam_core-0.2.0a1/src/adam_core/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-28 18:15:50.388175 adam_core-0.2.0a1/src/adam_core/_version.py
+-rw-r--r--   0        0        0     1377 2024-05-28 17:06:44.755022 adam_core-0.2.0a1/src/adam_core/constants.py
+-rw-r--r--   0        0        0      396 2024-05-28 17:06:44.755170 adam_core-0.2.0a1/src/adam_core/coordinates/__init__.py
+-rw-r--r--   0        0        0    10810 2024-05-28 17:06:44.755290 adam_core-0.2.0a1/src/adam_core/coordinates/cartesian.py
+-rw-r--r--   0        0        0    10202 2024-05-28 17:06:44.755414 adam_core-0.2.0a1/src/adam_core/coordinates/cometary.py
+-rw-r--r--   0        0        0     6505 2024-05-28 17:06:44.755532 adam_core-0.2.0a1/src/adam_core/coordinates/conversions.py
+-rw-r--r--   0        0        0    14285 2024-05-28 17:06:44.755677 adam_core-0.2.0a1/src/adam_core/coordinates/covariances.py
+-rw-r--r--   0        0        0     2634 2024-05-28 17:06:44.755755 adam_core-0.2.0a1/src/adam_core/coordinates/jacobian.py
+-rw-r--r--   0        0        0     9250 2024-05-28 17:06:44.755872 adam_core-0.2.0a1/src/adam_core/coordinates/keplerian.py
+-rw-r--r--   0        0        0     4194 2024-05-28 17:06:44.755988 adam_core-0.2.0a1/src/adam_core/coordinates/origin.py
+-rw-r--r--   0        0        0    16741 2024-05-28 17:06:44.756119 adam_core-0.2.0a1/src/adam_core/coordinates/residuals.py
+-rw-r--r--   0        0        0     7681 2024-05-28 17:06:44.756311 adam_core-0.2.0a1/src/adam_core/coordinates/spherical.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.756376 adam_core-0.2.0a1/src/adam_core/coordinates/tests/__init__.py
+-rw-r--r--   0        0        0     1211 2024-05-28 17:06:44.756514 adam_core-0.2.0a1/src/adam_core/coordinates/tests/conftest.py
+-rw-r--r--   0        0        0     2327 2024-05-28 17:06:44.756610 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     6568 2024-05-28 17:06:44.756722 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_cartesian.py
+-rw-r--r--   0        0        0     5367 2024-05-28 17:06:44.756850 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_cometary.py
+-rw-r--r--   0        0        0     6052 2024-05-28 17:06:44.757031 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_covariances.py
+-rw-r--r--   0        0        0     5444 2024-05-28 17:06:44.757227 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_keplerian.py
+-rw-r--r--   0        0        0     2948 2024-05-28 17:06:44.757314 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_origin.py
+-rw-r--r--   0        0        0    34081 2024-05-28 17:06:44.757510 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_residuals.py
+-rw-r--r--   0        0        0     1918 2024-05-28 17:06:44.757618 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_spherical.py
+-rw-r--r--   0        0        0     7646 2024-05-28 17:06:44.759302 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_cometary.py
+-rw-r--r--   0        0        0    10063 2024-05-28 17:06:44.759458 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_keplerian.py
+-rw-r--r--   0        0        0     4866 2024-05-28 17:06:44.759616 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_rotation.py
+-rw-r--r--   0        0        0     3243 2024-05-28 17:06:44.759769 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_spherical.py
+-rw-r--r--   0        0        0    11020 2024-05-28 17:06:44.759897 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_spice.py
+-rw-r--r--   0        0        0     8044 2024-05-28 17:06:44.760004 adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_translation.py
+-rw-r--r--   0        0        0    49595 2024-05-28 17:06:44.760222 adam_core-0.2.0a1/src/adam_core/coordinates/transform.py
+-rw-r--r--   0        0        0      691 2024-05-28 17:06:44.760362 adam_core-0.2.0a1/src/adam_core/coordinates/types.py
+-rw-r--r--   0        0        0     6647 2024-05-28 17:06:44.760507 adam_core-0.2.0a1/src/adam_core/coordinates/variants.py
+-rw-r--r--   0        0        0      110 2024-05-28 17:06:44.760609 adam_core-0.2.0a1/src/adam_core/dynamics/__init__.py
+-rw-r--r--   0        0        0   218508 2022-12-23 16:41:41.356795 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/aberrations.add_light_time-15.py310.1.nbc
+-rw-r--r--   0        0        0     1014 2022-12-23 16:41:41.347089 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/aberrations.add_light_time-15.py310.nbi
+-rw-r--r--   0        0        0   105441 2022-12-23 16:41:42.665228 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/aberrations.add_stellar_aberration-86.py310.1.nbc
+-rw-r--r--   0        0        0      983 2022-12-23 16:41:42.645978 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/aberrations.add_stellar_aberration-86.py310.nbi
+-rw-r--r--   0        0        0    76611 2022-12-23 16:41:30.071415 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/chi.calc_chi-13.py310.1.nbc
+-rw-r--r--   0        0        0      981 2022-12-23 16:41:30.059411 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/chi.calc_chi-13.py310.nbi
+-rw-r--r--   0        0        0    49303 2022-12-23 16:41:31.578450 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/lagrange.apply_lagrange_coefficients-92.py310.1.nbc
+-rw-r--r--   0        0        0     1008 2022-12-23 16:41:31.568284 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/lagrange.apply_lagrange_coefficients-92.py310.nbi
+-rw-r--r--   0        0        0    98285 2022-12-23 16:41:31.179470 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/lagrange.calc_lagrange_coefficients-14.py310.1.nbc
+-rw-r--r--   0        0        0     1034 2022-12-23 16:41:31.167530 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/lagrange.calc_lagrange_coefficients-14.py310.nbi
+-rw-r--r--   0        0        0    82910 2022-12-23 16:41:32.415608 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/state_transition._calc_M_matrix-15.py310.1.nbc
+-rw-r--r--   0        0        0     1022 2022-12-23 16:41:32.397995 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/state_transition._calc_M_matrix-15.py310.nbi
+-rw-r--r--   0        0        0   276594 2022-12-23 16:41:37.239361 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/state_transition.calc_state_transition_matrix-112.py310.1.nbc
+-rw-r--r--   0        0        0     1000 2022-12-23 16:41:37.220517 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/state_transition.calc_state_transition_matrix-112.py310.nbi
+-rw-r--r--   0        0        0    29452 2022-12-23 16:41:27.944024 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/stumpff.calc_stumpff-8.py310.1.nbc
+-rw-r--r--   0        0        0      962 2022-12-23 16:41:27.932619 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/stumpff.calc_stumpff-8.py310.nbi
+-rw-r--r--   0        0        0   156824 2022-12-23 16:41:38.691950 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/universal_propagate.propagate_universal-14.py310.1.nbc
+-rw-r--r--   0        0        0     1005 2022-12-23 16:41:38.679195 adam_core-0.2.0a1/src/adam_core/dynamics/__pycache__/universal_propagate.propagate_universal-14.py310.nbi
+-rw-r--r--   0        0        0     6601 2024-05-28 17:06:44.760697 adam_core-0.2.0a1/src/adam_core/dynamics/aberrations.py
+-rw-r--r--   0        0        0      780 2024-05-28 17:06:44.761711 adam_core-0.2.0a1/src/adam_core/dynamics/barker.py
+-rw-r--r--   0        0        0     3387 2024-05-28 17:06:44.761806 adam_core-0.2.0a1/src/adam_core/dynamics/chi.py
+-rw-r--r--   0        0        0    10553 2024-05-28 17:06:44.761912 adam_core-0.2.0a1/src/adam_core/dynamics/ephemeris.py
+-rw-r--r--   0        0        0     9796 2024-05-28 17:06:44.762068 adam_core-0.2.0a1/src/adam_core/dynamics/impacts.py
+-rw-r--r--   0        0        0     7728 2024-05-28 17:06:44.762231 adam_core-0.2.0a1/src/adam_core/dynamics/kepler.py
+-rw-r--r--   0        0        0     3747 2024-05-28 17:06:44.762306 adam_core-0.2.0a1/src/adam_core/dynamics/lagrange.py
+-rw-r--r--   0        0        0     5212 2024-05-28 17:06:44.762584 adam_core-0.2.0a1/src/adam_core/dynamics/moid.py
+-rw-r--r--   0        0        0     5614 2024-05-28 17:06:44.762865 adam_core-0.2.0a1/src/adam_core/dynamics/propagation.py
+-rw-r--r--   0        0        0     2250 2024-05-28 17:06:44.762960 adam_core-0.2.0a1/src/adam_core/dynamics/stumpff.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.763001 adam_core-0.2.0a1/src/adam_core/dynamics/tests/__init__.py
+-rw-r--r--   0        0        0     1115 2024-05-28 17:06:44.763131 adam_core-0.2.0a1/src/adam_core/dynamics/tests/conftest.py
+-rw-r--r--   0        0        0     5413 2024-05-28 17:06:44.763230 adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_ephemeris.py
+-rw-r--r--   0        0        0     7108 2024-05-28 17:06:44.763477 adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_impacts.py
+-rw-r--r--   0        0        0     8775 2024-05-28 17:06:44.763611 adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_kepler.py
+-rw-r--r--   0        0        0     5555 2024-05-28 17:06:44.763838 adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_moid.py
+-rw-r--r--   0        0        0    16189 2024-05-28 17:06:44.763985 adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_propagation.py
+-rw-r--r--   0        0        0     1311 2024-05-28 17:06:44.764071 adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_tisserand.py
+-rw-r--r--   0        0        0     1953 2024-05-28 17:06:44.764170 adam_core-0.2.0a1/src/adam_core/dynamics/tisserand.py
+-rw-r--r--   0        0        0      316 2024-05-28 17:06:44.764241 adam_core-0.2.0a1/src/adam_core/observations/__init__.py
+-rw-r--r--   0        0        0     2086 2024-05-28 17:06:44.764347 adam_core-0.2.0a1/src/adam_core/observations/associations.py
+-rw-r--r--   0        0        0     2616 2024-05-28 17:06:44.764474 adam_core-0.2.0a1/src/adam_core/observations/detections.py
+-rw-r--r--   0        0        0     2578 2024-05-28 17:06:44.764600 adam_core-0.2.0a1/src/adam_core/observations/exposures.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.764638 adam_core-0.2.0a1/src/adam_core/observations/tests/__init__.py
+-rw-r--r--   0        0        0     1582 2024-05-28 17:06:44.764744 adam_core-0.2.0a1/src/adam_core/observations/tests/test_associations.py
+-rw-r--r--   0        0        0     3349 2024-05-28 17:06:44.764818 adam_core-0.2.0a1/src/adam_core/observations/tests/test_detections.py
+-rw-r--r--   0        0        0     3623 2024-05-28 17:06:44.764947 adam_core-0.2.0a1/src/adam_core/observations/tests/test_exposures.py
+-rw-r--r--   0        0        0      139 2024-05-28 17:06:44.765039 adam_core-0.2.0a1/src/adam_core/observers/__init__.py
+-rw-r--r--   0        0        0     3703 2024-05-28 17:06:44.765147 adam_core-0.2.0a1/src/adam_core/observers/observers.py
+-rw-r--r--   0        0        0     6357 2024-05-28 17:06:44.765242 adam_core-0.2.0a1/src/adam_core/observers/state.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.765286 adam_core-0.2.0a1/src/adam_core/observers/tests/__init__.py
+-rw-r--r--   0        0        0     1339 2024-05-28 17:06:44.765452 adam_core-0.2.0a1/src/adam_core/observers/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     3141 2024-05-28 17:06:44.765577 adam_core-0.2.0a1/src/adam_core/observers/tests/test_state.py
+-rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.765793 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/000_ssb.parquet
+-rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.765999 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/000_sun.parquet
+-rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.766172 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/500_ssb.parquet
+-rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.766349 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/500_sun.parquet
+-rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.766573 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/F51_ssb.parquet
+-rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.766750 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/F51_sun.parquet
+-rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.766928 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/I41_ssb.parquet
+-rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.767125 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/I41_sun.parquet
+-rw-r--r--   0        0        0     1638 2024-05-28 17:06:44.767218 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/README.md
+-rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.767391 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/W84_ssb.parquet
+-rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.767550 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/W84_sun.parquet
+-rw-r--r--   0        0        0    26467 2024-05-28 17:06:44.767718 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/X05_ssb.parquet
+-rw-r--r--   0        0        0    26327 2024-05-28 17:06:44.767896 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/X05_sun.parquet
+-rw-r--r--   0        0        0     1475 2024-05-28 17:06:44.767981 adam_core-0.2.0a1/src/adam_core/observers/tests/testdata/get_states.py
+-rw-r--r--   0        0        0      266 2024-05-28 17:06:44.768062 adam_core-0.2.0a1/src/adam_core/orbit_determination/__init__.py
+-rw-r--r--   0        0        0     7438 2024-05-28 17:06:44.768223 adam_core-0.2.0a1/src/adam_core/orbit_determination/differential_correction.py
+-rw-r--r--   0        0        0     5219 2024-05-28 17:06:44.768382 adam_core-0.2.0a1/src/adam_core/orbit_determination/evaluate.py
+-rw-r--r--   0        0        0     1310 2024-05-28 17:06:44.768466 adam_core-0.2.0a1/src/adam_core/orbit_determination/fitted_orbits.py
+-rw-r--r--   0        0        0     2420 2024-05-28 17:06:44.768559 adam_core-0.2.0a1/src/adam_core/orbit_determination/outliers.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.768598 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/__init__.py
+-rw-r--r--   0        0        0      810 2024-05-28 17:06:44.768716 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/conftest.py
+-rw-r--r--   0        0        0     8261 2024-05-28 17:06:44.768898 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/data/pure_iod_orbit.parquet
+-rw-r--r--   0        0        0     3659 2024-05-28 17:06:44.769010 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/data/pure_iod_orbit_members.parquet
+-rw-r--r--   0        0        0    16284 2024-05-28 17:06:44.769171 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/data/pure_iod_orbit_observations.parquet
+-rw-r--r--   0        0        0      937 2024-05-28 17:06:44.769596 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/test_differential_correction.py
+-rw-r--r--   0        0        0     4281 2024-05-28 17:06:44.770015 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/test_evaluate.py
+-rw-r--r--   0        0        0     6049 2024-05-28 17:06:44.770121 adam_core-0.2.0a1/src/adam_core/orbit_determination/tests/test_outliers.py
+-rw-r--r--   0        0        0      275 2024-05-28 17:06:44.770264 adam_core-0.2.0a1/src/adam_core/orbits/__init__.py
+-rw-r--r--   0        0        0     2111 2024-05-28 17:06:44.770355 adam_core-0.2.0a1/src/adam_core/orbits/classification.py
+-rw-r--r--   0        0        0     4294 2024-05-28 17:06:44.770496 adam_core-0.2.0a1/src/adam_core/orbits/ephemeris.py
+-rw-r--r--   0        0        0     1381 2024-05-28 17:06:44.770648 adam_core-0.2.0a1/src/adam_core/orbits/orbits.py
+-rw-r--r--   0        0        0       87 2024-05-28 17:06:44.770738 adam_core-0.2.0a1/src/adam_core/orbits/query/__init__.py
+-rw-r--r--   0        0        0    11927 2024-05-28 17:06:44.770874 adam_core-0.2.0a1/src/adam_core/orbits/query/horizons.py
+-rw-r--r--   0        0        0     8414 2024-05-28 17:06:44.771011 adam_core-0.2.0a1/src/adam_core/orbits/query/sbdb.py
+-rw-r--r--   0        0        0     1726 2024-05-28 17:06:44.771084 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/__init__.py
+-rw-r--r--   0        0        0     3686 2024-05-28 17:06:44.771155 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/test_sbdb.py
+-rw-r--r--   0        0        0     2953 2024-05-28 17:06:44.771303 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/2001VB.json
+-rw-r--r--   0        0        0     5115 2024-05-28 17:06:44.771401 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/54509.json
+-rw-r--r--   0        0        0     3908 2024-05-28 17:06:44.771484 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/Ceres.json
+-rw-r--r--   0        0        0      442 2024-05-28 17:06:44.771558 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/README.md
+-rw-r--r--   0        0        0      114 2024-05-28 17:06:44.771632 adam_core-0.2.0a1/src/adam_core/orbits/query/tests/testdata/sbdb/missing.json
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.771667 adam_core-0.2.0a1/src/adam_core/orbits/tests/__init__.py
+-rw-r--r--   0        0        0      254 2024-05-28 17:06:44.771783 adam_core-0.2.0a1/src/adam_core/orbits/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     5773 2024-05-28 17:06:44.771901 adam_core-0.2.0a1/src/adam_core/orbits/tests/test_classification.py
+-rw-r--r--   0        0        0     3160 2024-05-28 17:06:44.771970 adam_core-0.2.0a1/src/adam_core/orbits/tests/test_ephemeris.py
+-rw-r--r--   0        0        0     1394 2024-05-28 17:06:44.772044 adam_core-0.2.0a1/src/adam_core/orbits/tests/test_orbits.py
+-rw-r--r--   0        0        0     1132 2024-05-28 17:06:44.772129 adam_core-0.2.0a1/src/adam_core/orbits/tests/test_variants.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.772238 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     2209 2024-05-28 17:06:44.772434 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/amo.csv
+-rw-r--r--   0        0        0     2222 2024-05-28 17:06:44.772547 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/apo.csv
+-rw-r--r--   0        0        0     2168 2024-05-28 17:06:44.772648 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/ast.csv
+-rw-r--r--   0        0        0     2195 2024-05-28 17:06:44.772906 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/ate.csv
+-rw-r--r--   0        0        0     2218 2024-05-28 17:06:44.773120 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/cen.csv
+-rw-r--r--   0        0        0      613 2024-05-28 17:06:44.773190 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/hya.csv
+-rw-r--r--   0        0        0     2178 2024-05-28 17:06:44.773377 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/ieo.csv
+-rw-r--r--   0        0        0     2243 2024-05-28 17:06:44.773469 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/imb.csv
+-rw-r--r--   0        0        0     2197 2024-05-28 17:06:44.773536 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/mba.csv
+-rw-r--r--   0        0        0     2219 2024-05-28 17:06:44.773696 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/mca.csv
+-rw-r--r--   0        0        0     2211 2024-05-28 17:06:44.773778 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/omb.csv
+-rw-r--r--   0        0        0     2226 2024-05-28 17:06:44.773869 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/tjn.csv
+-rw-r--r--   0        0        0     2161 2024-05-28 17:06:44.773946 adam_core-0.2.0a1/src/adam_core/orbits/tests/testdata/tno.csv
+-rw-r--r--   0        0        0    10048 2024-05-28 17:06:44.774074 adam_core-0.2.0a1/src/adam_core/orbits/variants.py
+-rw-r--r--   0        0        0      226 2024-05-28 17:06:44.774231 adam_core-0.2.0a1/src/adam_core/propagator/__init__.py
+-rw-r--r--   0        0        0    15904 2024-05-28 17:06:44.774376 adam_core-0.2.0a1/src/adam_core/propagator/propagator.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.774411 adam_core-0.2.0a1/src/adam_core/propagator/tests/__init__.py
+-rw-r--r--   0        0        0     3663 2024-05-28 17:06:44.774551 adam_core-0.2.0a1/src/adam_core/propagator/tests/test_propagator.py
+-rw-r--r--   0        0        0     1523 2024-05-28 17:06:44.774620 adam_core-0.2.0a1/src/adam_core/propagator/tests/test_utils.py
+-rw-r--r--   0        0        0     1899 2024-05-28 17:06:44.774927 adam_core-0.2.0a1/src/adam_core/propagator/utils.py
+-rw-r--r--   0        0        0     1556 2024-05-28 17:06:44.775025 adam_core-0.2.0a1/src/adam_core/ray_cluster.py
+-rw-r--r--   0        0        0      933 2024-05-28 17:06:44.775357 adam_core-0.2.0a1/src/adam_core/tests/test_imports.py
+-rw-r--r--   0        0        0     1276 2024-05-28 17:06:44.775455 adam_core-0.2.0a1/src/adam_core/tests/test_ray_cluster.py
+-rw-r--r--   0        0        0       60 2024-05-28 17:06:44.775645 adam_core-0.2.0a1/src/adam_core/time/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.775689 adam_core-0.2.0a1/src/adam_core/time/tests/__init__.py
+-rw-r--r--   0        0        0    21981 2024-05-28 17:06:44.775853 adam_core-0.2.0a1/src/adam_core/time/tests/test_time.py
+-rw-r--r--   0        0        0    19352 2024-05-28 17:06:44.776037 adam_core-0.2.0a1/src/adam_core/time/time.py
+-rw-r--r--   0        0        0      123 2024-05-28 17:06:44.776124 adam_core-0.2.0a1/src/adam_core/utils/__init__.py
+-rw-r--r--   0        0        0      212 2024-05-28 17:06:44.776209 adam_core-0.2.0a1/src/adam_core/utils/helpers/__init__.py
+-rw-r--r--   0        0        0     1245 2024-05-28 17:06:44.776453 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.776489 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/__init__.py
+-rw-r--r--   0        0        0    10395 2024-05-28 17:06:44.776652 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/elements_ssb_ec.csv
+-rw-r--r--   0        0        0    10398 2024-05-28 17:06:44.776772 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/elements_ssb_eq.csv
+-rw-r--r--   0        0        0    10402 2024-05-28 17:06:44.776892 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/elements_sun_ec.csv
+-rw-r--r--   0        0        0    10385 2024-05-28 17:06:44.776997 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/elements_sun_eq.csv
+-rw-r--r--   0        0        0  1797474 2024-05-28 17:06:44.780662 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/ephemeris.csv
+-rw-r--r--   0        0        0     6919 2024-05-28 17:06:44.780870 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/get_test_data.py
+-rw-r--r--   0        0        0      504 2024-05-28 17:06:44.780949 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/objects.csv
+-rw-r--r--   0        0        0    15438 2024-05-28 17:06:44.781091 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/orbits.parquet
+-rw-r--r--   0        0        0   156180 2024-05-28 17:06:44.781753 adam_core-0.2.0a1/src/adam_core/utils/helpers/data/propagated_orbits.parquet
+-rw-r--r--   0        0        0     5273 2024-05-28 17:06:44.781932 adam_core-0.2.0a1/src/adam_core/utils/helpers/observations.py
+-rw-r--r--   0        0        0     2836 2024-05-28 17:06:44.782022 adam_core-0.2.0a1/src/adam_core/utils/helpers/orbits.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.782055 adam_core-0.2.0a1/src/adam_core/utils/helpers/tests/__init__.py
+-rw-r--r--   0        0        0     2096 2024-05-28 17:06:44.782161 adam_core-0.2.0a1/src/adam_core/utils/helpers/tests/test_observations.py
+-rw-r--r--   0        0        0      698 2024-05-28 17:06:44.782222 adam_core-0.2.0a1/src/adam_core/utils/helpers/tests/test_orbits.py
+-rw-r--r--   0        0        0    13599 2024-05-28 17:06:44.782348 adam_core-0.2.0a1/src/adam_core/utils/mpc.py
+-rw-r--r--   0        0        0     5263 2024-05-28 17:06:44.782462 adam_core-0.2.0a1/src/adam_core/utils/spice.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:06:44.782504 adam_core-0.2.0a1/src/adam_core/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1455 2024-05-28 17:06:44.782631 adam_core-0.2.0a1/src/adam_core/utils/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     7211 2024-05-28 17:06:44.782845 adam_core-0.2.0a1/src/adam_core/utils/tests/test_mpc.py
+-rw-r--r--   0        0        0      550 2024-05-28 17:06:44.782919 adam_core-0.2.0a1/src/adam_core/utils/tests/test_spice.py
+-rw-r--r--   0        0        0    18170 1970-01-01 00:00:00.000000 adam_core-0.2.0a1/PKG-INFO
```

### Comparing `adam_core-0.1.0/LICENSE.md` & `adam_core-0.2.0a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `adam_core-0.1.0/adam_core/constants.py` & `adam_core-0.2.0a1/src/adam_core/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 
 __all__ = [
     "KM_P_AU",
     "S_P_DAY",
     "Constants",
-    "DE43X",
     "DE44X",
 ]
 
 # km in an au
 KM_P_AU = 149597870.700
 # seconds in a day
 S_P_DAY = 86400.0
@@ -31,30 +30,18 @@
         )
 
         # Transformation matrix from Ecliptic J2000 to Equatorial J2000
         self.TRANSFORM_EC2EQ = self.TRANSFORM_EQ2EC.T
         return
 
 
-DE43X_CONSTANTS = {
-    # Speed of Light : au / d (299792.458 km / s -- DE430/DE431)
-    "C": 299792.458 / KM_P_AU * S_P_DAY,
-    # Standard Gravitational Parameter -- Sun :  au**3 / d**2 (0.295912208285591100E-3 -- DE431/DE430)
-    "MU": 0.295912208285591100e-3,
-    # Earth Equatorial Radius: au (6378.1363 km -- DE431/DE430)
-    "R_Earth": 6378.1363 / KM_P_AU,
-    # Mean Obliquity at J2000: radians (84381.448 arcseconds -- DE431/DE430)
-    "Obliquity": 84381.448 * np.pi / (180.0 * 3600.0),
-}
-Constants = DE43X = _Constants(**DE43X_CONSTANTS)
-
 DE44X_CONSTANTS = {
     # Speed of Light : au / d (299792.458 km / s -- DE430/DE431)
     "C": 299792.458 / KM_P_AU * S_P_DAY,
     # Standard Gravitational Parameter -- Sun :  au**3 / d**2 (0.29591220828411956E-03 -- DE441/DE440)
     "MU": 0.29591220828411956e-03,
     # Earth Equatorial Radius: au (6378.1363 km -- DE431/DE430)
     "R_Earth": 6378.1363 / KM_P_AU,
     # Mean Obliquity at J2000: radians (84381.448 arcseconds -- DE431/DE430)
     "Obliquity": 84381.448 * np.pi / (180.0 * 3600.0),
 }
-DE44X = _Constants(**DE44X_CONSTANTS)
+DE44X = Constants = _Constants(**DE44X_CONSTANTS)
```

### Comparing `adam_core-0.1.0/adam_core/coordinates/cartesian.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/cartesian.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,201 +1,224 @@
+from __future__ import annotations
+
 import logging
-from typing import TYPE_CHECKING, Literal
 
 import numpy as np
-import pandas as pd
-from astropy import units as u
-from quivr import Float64Column, StringAttribute, Table
+import numpy.typing as npt
+import quivr as qv
 
+from ..time import Timestamp
+from . import cometary, keplerian, spherical
 from .covariances import CoordinateCovariances
-from .io import coords_from_dataframe, coords_to_dataframe
 from .origin import Origin
-from .times import Times
 
-if TYPE_CHECKING:
-    from .cometary import CometaryCoordinates
-    from .keplerian import KeplerianCoordinates
-    from .spherical import SphericalCoordinates
-
-__all__ = ["CartesianCoordinates", "CARTESIAN_COLS", "CARTESIAN_UNITS"]
-
-CARTESIAN_COLS = {}
-CARTESIAN_UNITS = {}
-for i in ["x", "y", "z"]:
-    CARTESIAN_COLS[i] = i
-    CARTESIAN_UNITS[i] = u.au
-for i in ["vx", "vy", "vz"]:
-    CARTESIAN_COLS[i] = i
-    CARTESIAN_UNITS[i] = u.au / u.d
+__all__ = ["CartesianCoordinates"]
 
 COVARIANCE_ROTATION_TOLERANCE = 1e-25
 logger = logging.getLogger(__name__)
 
 
-class CartesianCoordinates(Table):
+class CartesianCoordinates(qv.Table):
+    """Represents coordinates in Cartesian space."""
+
+    #: x coordinates in AU
+    x = qv.Float64Column(nullable=True)
+
+    #: y coordinates in AU
+    y = qv.Float64Column(nullable=True)
+
+    #: z coordinates in AU
+    z = qv.Float64Column(nullable=True)
+
+    #: x velocity in AU/day
+    vx = qv.Float64Column(nullable=True)
+
+    #: y velocity in AU/day
+    vy = qv.Float64Column(nullable=True)
+
+    #: z velocity in AU/day
+    vz = qv.Float64Column(nullable=True)
 
-    x = Float64Column(nullable=True)
-    y = Float64Column(nullable=True)
-    z = Float64Column(nullable=True)
-    vx = Float64Column(nullable=True)
-    vy = Float64Column(nullable=True)
-    vz = Float64Column(nullable=True)
-    times = Times.as_column(nullable=True)
-    covariances = CoordinateCovariances.as_column(nullable=True)
-    origin = Origin.as_column(nullable=False)
-    frame = StringAttribute()
+    #: The instant at which the coordinates are valid
+    time = Timestamp.as_column(nullable=True)
+
+    #: Covariance matrix for the x, y, z, vx, vy, and vz values
+    covariance = CoordinateCovariances.as_column(nullable=True)
+
+    #: Center of the coordinate system
+    origin = Origin.as_column()
+
+    #: Frame of the coordinate system - 'ecliptic' or 'equatorial' or 'unspecified'.
+    frame = qv.StringAttribute(default="unspecified")
 
     @property
-    def values(self) -> np.ndarray:
-        return np.array(self.table.select(["x", "y", "z", "vx", "vy", "vz"])).T
+    def values(self) -> npt.NDArray[np.float64]:
+        """The x, y, z, vx, vy, and vz columns all in one 6-N matrix
+        of numpy float64 values. Nulls are converted to NaNs.
+
+        """
+        return np.array(self.table.select(["x", "y", "z", "vx", "vy", "vz"]))
 
     @property
-    def r(self) -> np.ndarray:
+    def r(self) -> npt.NDArray[np.float64]:
         """
         Position vector.
         """
         return np.array(self.table.select(["x", "y", "z"]))
 
     @property
-    def r_mag(self) -> np.ndarray:
+    def r_mag(self) -> npt.NDArray[np.float64]:
         """
         Magnitude of the position vector.
         """
         return np.linalg.norm(self.r, axis=1)
 
     @property
-    def r_hat(self) -> np.ndarray:
+    def r_hat(self) -> npt.NDArray[np.float64]:
         """
         Unit vector in the direction of the position vector.
         """
         return self.r / self.r_mag[:, None]
 
     @property
-    def v(self) -> np.ndarray:
+    def v(self) -> npt.NDArray[np.float64]:
         """
         Velocity vector.
         """
         return np.array(self.table.select(["vx", "vy", "vz"]))
 
     @property
-    def v_mag(self) -> np.ndarray:
+    def v_mag(self) -> npt.NDArray[np.float64]:
         """
         Magnitude of the velocity vector.
         """
         return np.linalg.norm(self.v, axis=1)
 
     @property
-    def v_hat(self) -> np.ndarray:
+    def v_hat(self) -> npt.NDArray[np.float64]:
         """
         Unit vector in the direction of the velocity vector.
         """
         return self.v / self.v_mag[:, None]
 
     @property
-    def sigma_x(self) -> np.ndarray:
+    def sigma_x(self) -> npt.NDArray[np.float64]:
         """
         1-sigma uncertainty in the X-coordinate.
         """
-        return self.covariances.sigmas[:, 0]
+        return self.covariance.sigmas[:, 0]
 
     @property
-    def sigma_y(self) -> np.ndarray:
+    def sigma_y(self) -> npt.NDArray[np.float64]:
         """
         1-sigma uncertainty in the Y-coordinate.
         """
-        return self.covariances.sigmas[:, 1]
+        return self.covariance.sigmas[:, 1]
 
     @property
-    def sigma_z(self) -> np.ndarray:
+    def sigma_z(self) -> npt.NDArray[np.float64]:
         """
         1-sigma uncertainty in the Z-coordinate.
         """
-        return self.covariances.sigmas[:, 2]
+        return self.covariance.sigmas[:, 2]
 
     @property
-    def sigma_vx(self) -> np.ndarray:
+    def sigma_vx(self) -> npt.NDArray[np.float64]:
         """
         1-sigma uncertainty in the X-coordinate velocity.
         """
-        return self.covariances.sigmas[:, 3]
+        return self.covariance.sigmas[:, 3]
 
     @property
-    def sigma_vy(self) -> np.ndarray:
+    def sigma_vy(self) -> npt.NDArray[np.float64]:
         """
         1-sigma uncertainty in the Y-coordinate velocity.
         """
-        return self.covariances.sigmas[:, 4]
+        return self.covariance.sigmas[:, 4]
 
     @property
-    def sigma_vz(self) -> np.ndarray:
+    def sigma_vz(self) -> npt.NDArray[np.float64]:
         """
         1-sigma uncertainty in the Z-coordinate velocity.
         """
-        return self.covariances.sigmas[:, 5]
+        return self.covariance.sigmas[:, 5]
 
     @property
-    def sigma_r(self) -> np.ndarray:
+    def sigma_r(self) -> npt.NDArray[np.float64]:
         """
         1-sigma uncertainties in the position vector.
         """
-        return np.sqrt(self.covariances.sigmas[:, 0:3])
+        return self.covariance.sigmas[:, 0:3]
 
     @property
-    def sigma_r_mag(self) -> np.ndarray:
+    def sigma_r_mag(self) -> npt.NDArray[np.float64]:
         """
         1-sigma uncertainty in the position.
         """
-        return np.sqrt(np.sum(self.covariances.sigmas[:, 0:3] ** 2, axis=1))
+        return np.sqrt(np.sum(self.covariance.sigmas[:, 0:3] ** 2, axis=1))
 
     @property
-    def sigma_v(self) -> np.ndarray:
+    def sigma_v(self) -> npt.NDArray[np.float64]:
         """
         1-sigma uncertainties in the velocity vector.
         """
-        return np.sqrt(self.covariances.sigmas[:, 3:6])
+        return self.covariance.sigmas[:, 3:6]
 
     @property
-    def sigma_v_mag(self) -> np.ndarray:
+    def sigma_v_mag(self) -> npt.NDArray[np.float64]:
         """
         1-sigma uncertainty in the velocity vector.
         """
-        return np.sqrt(np.sum(self.covariances.sigmas[:, 3:6] ** 2, axis=1))
+        return np.sqrt(np.sum(self.covariance.sigmas[:, 3:6] ** 2, axis=1))
+
+    @property
+    def h(self) -> npt.NDArray[np.float64]:
+        """
+        Specific angular momentum vector.
+        """
+        return np.cross(self.r, self.v)
+
+    @property
+    def h_mag(self) -> npt.NDArray[np.float64]:
+        """
+        Magnitude of the specific angular momentum vector.
+        """
+        return np.linalg.norm(self.h, axis=1)
 
     def rotate(
-        self, rotation_matrix: np.ndarray, frame_out: str
-    ) -> "CartesianCoordinates":
+        self, rotation_matrix: npt.NDArray[np.float64], frame_out: str
+    ) -> CartesianCoordinates:
         """
         Rotate Cartesian coordinates and their covariances by the given rotation matrix.
 
         Covariance matrices are also rotated. Rotations will sometimes result
         in covariance matrix elements very near zero but not exactly zero. Any
         elements that are smaller than +-1e-25 are rounded down to 0.
 
         Parameters
         ----------
-        matrix : `~numpy.ndarray` (6, 6)
-            Rotation matrix.
-        frame_out : str
+        matrix:
+            6x6 rotation matrix.
+        frame_out: str
             Name of the frame to which coordinates are being rotated.
 
         Returns
         -------
-        CartesianCoordinates : `~adam_core.coordinates.cartesian.CartesianCoordinates`
             Rotated Cartesian coordinates and their covariances.
         """
         # Extract coordinate values into a masked array and mask NaNss
         masked_coords = np.ma.masked_array(self.values, fill_value=np.NaN)
         masked_coords.mask = np.isnan(masked_coords.data)
 
         # Rotate coordinates
         coords_rotated = np.ma.dot(masked_coords, rotation_matrix.T, strict=False)
 
         # Extract covariances
         masked_covariances = np.ma.masked_array(
-            self.covariances.to_matrix(), fill_value=0.0
+            self.covariance.to_matrix(), fill_value=0.0
         )
         masked_covariances.mask = np.isnan(masked_covariances.data)
 
         # Rotate covariances
         covariances_rotated = (
             rotation_matrix @ masked_covariances.filled() @ rotation_matrix.T
         )
@@ -222,36 +245,38 @@
         coords = self.from_kwargs(
             x=coords_rotated[:, 0],
             y=coords_rotated[:, 1],
             z=coords_rotated[:, 2],
             vx=coords_rotated[:, 3],
             vy=coords_rotated[:, 4],
             vz=coords_rotated[:, 5],
-            times=self.times,
-            covariances=CoordinateCovariances.from_matrix(covariances_rotated),
+            time=self.time,
+            covariance=CoordinateCovariances.from_matrix(covariances_rotated),
             origin=self.origin,
             frame=frame_out,
         )
         return coords
 
-    def translate(self, vector: np.ndarray, origin_out: str) -> "CartesianCoordinates":
+    def translate(
+        self, vector: npt.NDArray[np.float64], origin_out: str
+    ) -> CartesianCoordinates:
         """
         Translate Cartesian coordinates by the given vector.
 
         Parameters
         ----------
-        vector : `~numpy.ndarray` (6,) or (N, 6)
-            Translation vector. If a single vector is given, it is applied to all coordinates.
-            If an array of vectors is given, each vector is applied to the corresponding coordinate.
-        origin_out : str
+
+        vector:
+            6x1 or 6xN translation vector. If a 6x1 vector is given, it is applied to all coordinates.
+            If an 6xN array of vectors is given, each vector is applied to the corresponding coordinate.
+        origin_out:
             Name of the origin to which coordinates are being translated.
 
         Returns
         -------
-        CartesianCoordinates : `~adam_core.coordinates.cartesian.CartesianCoordinates`
             Translated Cartesian coordinates and their covariances.
         """
         N = len(self)
         if vector.shape == (6,):
             vector_ = vector.reshape(1, 6)
         elif vector.shape == (N, 6):
             vector_ = vector
@@ -268,93 +293,58 @@
         coords = self.from_kwargs(
             x=coords_translated[:, 0],
             y=coords_translated[:, 1],
             z=coords_translated[:, 2],
             vx=coords_translated[:, 3],
             vy=coords_translated[:, 4],
             vz=coords_translated[:, 5],
-            times=self.times,
-            covariances=self.covariances,
+            time=self.time,
+            covariance=self.covariance,
             origin=Origin.from_kwargs(code=[origin_out] * len(self)),
             frame=self.frame,
         )
         return coords
 
-    def to_cometary(self) -> "CometaryCoordinates":
-        from .cometary import CometaryCoordinates
-
-        return CometaryCoordinates.from_cartesian(self)
+    def to_cometary(self) -> cometary.CometaryCoordinates:
+        """
+        Converts the Cartesian coordinates to the cometary parameterization.
+        """
+        return cometary.CometaryCoordinates.from_cartesian(self)
 
     @classmethod
-    def from_cometary(cls, cometary: "CometaryCoordinates") -> "CartesianCoordinates":
+    def from_cometary(
+        cls, cometary: cometary.CometaryCoordinates
+    ) -> CartesianCoordinates:
+        """
+        Constructs CartesianCoordinates from the cometary parameterization.
+        """
         return cometary.to_cartesian()
 
-    def to_keplerian(self) -> "KeplerianCoordinates":
-        from .keplerian import KeplerianCoordinates
-
-        return KeplerianCoordinates.from_cartesian(self)
+    def to_keplerian(self) -> keplerian.KeplerianCoordinates:
+        """
+        Converts the Cartesian coordinates to the Keplerian parameterization.
+        """
+        return keplerian.KeplerianCoordinates.from_cartesian(self)
 
     @classmethod
     def from_keplerian(
-        cls, keplerian: "KeplerianCoordinates"
-    ) -> "CartesianCoordinates":
+        cls, keplerian: keplerian.KeplerianCoordinates
+    ) -> CartesianCoordinates:
+        """
+        Constructs CartesianCoordinates from the Keplerian parameterization.
+        """
         return keplerian.to_cartesian()
 
-    def to_spherical(self) -> "SphericalCoordinates":
-        from .spherical import SphericalCoordinates
-
-        return SphericalCoordinates.from_cartesian(self)
-
-    @classmethod
-    def from_spherical(
-        cls, spherical: "SphericalCoordinates"
-    ) -> "CartesianCoordinates":
-        return spherical.to_cartesian()
-
-    def to_dataframe(
-        self, sigmas: bool = False, covariances: bool = True
-    ) -> pd.DataFrame:
+    def to_spherical(self) -> spherical.SphericalCoordinates:
         """
-        Convert coordinates to a pandas DataFrame.
-
-        Parameters
-        ----------
-        sigmas : bool, optional
-            If True, include 1-sigma uncertainties in the DataFrame.
-        covariances : bool, optional
-            If True, include covariance matrices in the DataFrame. Covariance matrices
-            will be split into 21 columns, with the lower triangular elements stored.
-
-        Returns
-        -------
-        df : `~pandas.Dataframe`
-            DataFrame containing coordinates.
+        Converts the Cartesian coordinates to the spherical parameterization.
         """
-        return coords_to_dataframe(
-            self,
-            ["x", "y", "z", "vx", "vy", "vz"],
-            sigmas=sigmas,
-            covariances=covariances,
-        )
+        return spherical.SphericalCoordinates.from_cartesian(self)
 
     @classmethod
-    def from_dataframe(
-        cls, df: pd.DataFrame, frame: Literal["ecliptic", "equatorial"]
-    ) -> "CartesianCoordinates":
+    def from_spherical(
+        cls, spherical: spherical.SphericalCoordinates
+    ) -> CartesianCoordinates:
         """
-        Create coordinates from a pandas DataFrame.
-
-        Parameters
-        ----------
-        df : `~pandas.Dataframe`
-            DataFrame containing coordinates.
-        frame : {"ecliptic", "equatorial"}
-            Frame in which coordinates are defined.
-
-        Returns
-        -------
-        coords : `~adam_core.coordinates.cartesian.CartesianCoordinates`
-            Cartesian coordinates.
+        Constructs CartesianCoordinates from the spherical parameterization.
         """
-        return coords_from_dataframe(
-            cls, df, coord_names=["x", "y", "z", "vx", "vy", "vz"], frame=frame
-        )
+        return spherical.to_cartesian()
```

### Comparing `adam_core-0.1.0/adam_core/coordinates/cometary.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/cometary.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,112 +1,93 @@
-from typing import TYPE_CHECKING, Literal
+from __future__ import annotations
 
 import numpy as np
-import pandas as pd
-from astropy import units as u
-from quivr import Float64Column, StringAttribute, Table
+import quivr as qv
 
-from .cartesian import CartesianCoordinates
+from ..time import Timestamp
+from . import cartesian, keplerian, spherical
 from .covariances import CoordinateCovariances, transform_covariances_jacobian
-from .io import coords_from_dataframe, coords_to_dataframe
 from .origin import Origin
-from .times import Times
-
-if TYPE_CHECKING:
-    from .keplerian import KeplerianCoordinates
-    from .spherical import SphericalCoordinates
-
 
 __all__ = [
     "CometaryCoordinates",
-    "COMETARY_COLS",
-    "COMETARY_UNITS",
 ]
 
-COMETARY_COLS = {}
-COMETARY_UNITS = {}
-for i in ["q", "e", "i", "raan", "ap", "tp"]:
-    COMETARY_COLS[i] = i
-COMETARY_UNITS["q"] = u.au
-COMETARY_UNITS["e"] = u.dimensionless_unscaled
-COMETARY_UNITS["i"] = u.deg
-COMETARY_UNITS["raan"] = u.deg
-COMETARY_UNITS["ap"] = u.deg
-COMETARY_UNITS["tp"] = u.d
 
-
-class CometaryCoordinates(Table):
+class CometaryCoordinates(qv.Table):
     # TODO: Time of periapse passage could perhaps be represented
     # as a Times object. We could then modify self.values to only
     # grab the MJD column. That said, we would want to force it
     # the time scale to be in TDB..
 
-    q = Float64Column(nullable=False)
-    e = Float64Column(nullable=False)
-    i = Float64Column(nullable=False)
-    raan = Float64Column(nullable=False)
-    ap = Float64Column(nullable=False)
-    tp = Float64Column(nullable=False)
-    times = Times.as_column(nullable=True)
-    covariances = CoordinateCovariances.as_column(nullable=True)
-    origin = Origin.as_column(nullable=False)
-    frame = StringAttribute()
+    q = qv.Float64Column()
+    e = qv.Float64Column()
+    i = qv.Float64Column()
+    raan = qv.Float64Column()
+    ap = qv.Float64Column()
+    tp = qv.Float64Column()
+    time = Timestamp.as_column(nullable=True)
+    covariance = CoordinateCovariances.as_column(nullable=True)
+    origin = Origin.as_column()
+    frame = qv.StringAttribute(default="unspecified")
 
     @property
     def values(self) -> np.ndarray:
-        return np.array(self.table.select(["q", "e", "i", "raan", "ap", "tp"])).T
+        return np.array(self.table.select(["q", "e", "i", "raan", "ap", "tp"]))
 
     @property
     def sigma_q(self) -> np.ndarray:
         """
         1-sigma uncertainty in periapsis distance.
         """
-        return self.covariances.sigmas[:, 0]
+        return self.covariance.sigmas[:, 0]
 
     @property
     def sigma_e(self) -> np.ndarray:
         """
         1-sigma uncertainty in eccentricity.
         """
-        return self.covariances.sigmas[:, 1]
+        return self.covariance.sigmas[:, 1]
 
     @property
     def sigma_i(self) -> np.ndarray:
         """
         1-sigma uncertainty in inclination.
         """
-        return self.covariances.sigmas[:, 2]
+        return self.covariance.sigmas[:, 2]
 
     @property
     def sigma_raan(self):
         """
         1-sigma uncertainty in right ascension of the ascending node.
         """
-        return self.covariances.sigmas[:, 3]
+        return self.covariance.sigmas[:, 3]
 
     @property
     def sigma_ap(self) -> np.ndarray:
         """
         1-sigma uncertainty in argument of periapsis.
         """
-        return self.covariances.sigmas[:, 4]
+        return self.covariance.sigmas[:, 4]
 
     @property
     def sigma_tp(self) -> np.ndarray:
         """
         1-sigma uncertainty in time of periapse passage.
         """
-        return self.covariances.sigmas[:, 5]
+        return self.covariance.sigmas[:, 5]
 
     @property
     def a(self) -> np.ndarray:
         """
         Semi-major axis.
         """
-        return self.q.to_numpy() / (1 - self.e.to_numpy())
+        from ..dynamics.kepler import calc_semi_major_axis
+
+        return np.array(calc_semi_major_axis(self.q.to_numpy(), self.e.to_numpy()))
 
     @a.setter
     def a(self, value):
         err = (
             "Cannot set semi-major axis (a) as it is"
             " derived from the periapsis distance (q) and eccentricity (e)."
         )
@@ -121,15 +102,17 @@
         raise ValueError(err)
 
     @property
     def Q(self) -> np.ndarray:
         """
         Apoapsis distance.
         """
-        return self.a.to_numpy() * (1 + self.e.to_numpy())
+        from ..dynamics.kepler import calc_apoapsis_distance
+
+        return np.array(calc_apoapsis_distance(self.a, self.e.to_numpy()))
 
     @Q.setter
     def Q(self, value):
         err = (
             "Cannot set apoapsis distance (Q) as it is"
             " derived from the semi-major axis (a) and eccentricity (e)."
         )
@@ -144,15 +127,17 @@
         raise ValueError(err)
 
     @property
     def p(self) -> np.ndarray:
         """
         Semi-latus rectum.
         """
-        return self.a.to_numpy() / (1 - self.e.to_numpy() ** 2)
+        from ..dynamics.kepler import calc_semi_latus_rectum
+
+        return np.array(calc_semi_latus_rectum(self.a, self.e.to_numpy()))
 
     @p.setter
     def p(self, value):
         err = (
             "Cannot set semi-latus rectum (p) as it is"
             " derived from the semi-major axis (a) and eccentricity (e)."
         )
@@ -167,121 +152,150 @@
         raise ValueError(err)
 
     @property
     def P(self) -> np.ndarray:
         """
         Period.
         """
-        return np.sqrt(4 * np.pi**2 * self.a.to_numpy() ** 3 / self.origin.mu)
+        from ..dynamics.kepler import calc_period
+
+        return np.array(calc_period(self.a, self.origin.mu()))
 
     @P.setter
     def P(self, value):
         err = (
             "Cannot set period (P) as it is"
             " derived from the semi-major axis (a) and gravitational parameter (mu)."
         )
         raise ValueError(err)
 
-    @p.deleter
+    @P.deleter
     def P(self):
         err = (
             "Cannot delete period (P) as it is"
             " derived from the semi-major axis (a) and gravitational parameter (mu)."
         )
         raise ValueError(err)
 
-    def to_cartesian(self) -> CartesianCoordinates:
+    @property
+    def n(self):
+        """
+        Mean motion in degrees.
+        """
+        from ..dynamics.kepler import calc_mean_motion
+
+        return np.degrees(np.array(calc_mean_motion(self.a, self.origin.mu())))
+
+    @n.setter
+    def n(self, value):
+        err = (
+            "Cannot set mean motion (n) as it is"
+            " derived from semi-major axis (a) and gravitational parameter (mu)."
+        )
+        raise ValueError(err)
+
+    @n.deleter
+    def n(self):
+        err = (
+            "Cannot delete mean motion (n) as it is"
+            " derived from semi-major axis (a) and gravitational parameter (mu)."
+        )
+        raise ValueError(err)
+
+    def to_cartesian(self) -> cartesian.CartesianCoordinates:
         from .transform import _cometary_to_cartesian, cometary_to_cartesian
 
-        if self.times is None:
+        if self.time is None:
             err = (
                 "To convert Cometary coordinates to Cartesian coordinates, the times\n"
                 "at which the Coordinates coordinates are defined is required to give\n"
                 "the time of periapsis passage context."
             )
             raise ValueError(err)
 
         # Extract gravitational parameter from origin
-        mu = self.origin.mu
+        mu = self.origin.mu()
 
         coords_cartesian = cometary_to_cartesian(
             self.values,
-            t0=self.times.to_astropy().tdb.mjd,
+            t0=self.time.to_numpy(),
             mu=mu,
             max_iter=100,
             tol=1e-15,
         )
         coords_cartesian = np.array(coords_cartesian)
 
-        cometary_covariances = self.covariances.to_matrix()
-        if not np.all(np.isnan(cometary_covariances)):
+        if not self.covariance.is_all_nan():
+            cometary_covariances = self.covariance.to_matrix()
             covariances_cartesian = transform_covariances_jacobian(
                 self.values,
                 cometary_covariances,
                 _cometary_to_cartesian,
-                in_axes=(0, 0, None, None, None),
+                in_axes=(0, 0, 0, None, None),
                 out_axes=0,
-                t0=self.times.to_astropy().tdb.mjd,
+                t0=self.time.to_numpy(),
                 mu=mu,
                 max_iter=100,
                 tol=1e-15,
             )
         else:
             covariances_cartesian = np.empty(
                 (len(coords_cartesian), 6, 6), dtype=np.float64
             )
             covariances_cartesian.fill(np.nan)
 
         covariances_cartesian = CoordinateCovariances.from_matrix(covariances_cartesian)
-        coords = CartesianCoordinates.from_kwargs(
+        coords = cartesian.CartesianCoordinates.from_kwargs(
             x=coords_cartesian[:, 0],
             y=coords_cartesian[:, 1],
             z=coords_cartesian[:, 2],
             vx=coords_cartesian[:, 3],
             vy=coords_cartesian[:, 4],
             vz=coords_cartesian[:, 5],
-            times=self.times,
-            covariances=covariances_cartesian,
+            time=self.time,
+            covariance=covariances_cartesian,
             origin=self.origin,
             frame=self.frame,
         )
 
         return coords
 
     @classmethod
-    def from_cartesian(cls, cartesian: CartesianCoordinates) -> "CometaryCoordinates":
+    def from_cartesian(
+        cls, cartesian: cartesian.CartesianCoordinates
+    ) -> CometaryCoordinates:
         from .transform import _cartesian_to_cometary, cartesian_to_cometary
 
-        if cartesian.times is None:
+        if cartesian.time is None:
             err = (
                 "To convert Cometary coordinates to Cartesian coordinates, the times\n"
                 "at which the Cartesian coordinates are defined is required to calculate\n"
                 "the time of periapsis passage."
             )
             raise ValueError(err)
 
         # Extract gravitational parameter from origin
-        mu = cartesian.origin.mu
+        mu = cartesian.origin.mu()
 
         coords_cometary = cartesian_to_cometary(
             cartesian.values,
-            cartesian.times.to_astropy().tdb.mjd,
+            cartesian.time.to_numpy(),
             mu=mu,
         )
         coords_cometary = np.array(coords_cometary)
 
-        cartesian_covariances = cartesian.covariances.to_matrix()
-        if not np.all(np.isnan(cartesian_covariances)):
+        if not cartesian.covariance.is_all_nan():
+            cartesian_covariances = cartesian.covariance.to_matrix()
             covariances_cometary = transform_covariances_jacobian(
                 cartesian.values,
                 cartesian_covariances,
                 _cartesian_to_cometary,
-                in_axes=(0, 0, None),
+                in_axes=(0, 0, 0),
                 out_axes=0,
-                t0=cartesian.times.to_astropy().tdb.mjd,
+                t0=cartesian.time.to_numpy(),
                 mu=mu,
             )
         else:
             covariances_cometary = np.empty(
                 (len(coords_cometary), 6, 6), dtype=np.float64
             )
             covariances_cometary.fill(np.nan)
@@ -290,85 +304,32 @@
         coords = cls.from_kwargs(
             q=coords_cometary[:, 0],
             e=coords_cometary[:, 1],
             i=coords_cometary[:, 2],
             raan=coords_cometary[:, 3],
             ap=coords_cometary[:, 4],
             tp=coords_cometary[:, 5],
-            times=cartesian.times,
-            covariances=covariances_cometary,
+            time=cartesian.time,
+            covariance=covariances_cometary,
             origin=cartesian.origin,
             frame=cartesian.frame,
         )
 
         return coords
 
-    def to_keplerian(self) -> "KeplerianCoordinates":
-        from .keplerian import KeplerianCoordinates
-
-        return KeplerianCoordinates.from_cartesian(self.to_cartesian())
+    def to_keplerian(self) -> keplerian.KeplerianCoordinates:
+        return keplerian.KeplerianCoordinates.from_cartesian(self.to_cartesian())
 
     @classmethod
     def from_keplerian(
-        cls, keplerian_coordinates: "KeplerianCoordinates"
-    ) -> "CometaryCoordinates":
+        cls, keplerian_coordinates: keplerian.KeplerianCoordinates
+    ) -> CometaryCoordinates:
         return cls.from_cartesian(keplerian_coordinates.to_cartesian())
 
-    def to_spherical(self) -> "SphericalCoordinates":
-        from .spherical import SphericalCoordinates
-
-        return SphericalCoordinates.from_cartesian(self.to_cartesian())
+    def to_spherical(self) -> spherical.SphericalCoordinates:
+        return spherical.SphericalCoordinates.from_cartesian(self.to_cartesian())
 
     @classmethod
     def from_spherical(
-        cls, spherical_coordinates: "SphericalCoordinates"
-    ) -> "CometaryCoordinates":
+        cls, spherical_coordinates: spherical.SphericalCoordinates
+    ) -> CometaryCoordinates:
         return cls.from_cartesian(spherical_coordinates.to_cartesian())
-
-    def to_dataframe(
-        self, sigmas: bool = False, covariances: bool = True
-    ) -> pd.DataFrame:
-        """
-        Convert coordinates to a pandas DataFrame.
-
-        Parameters
-        ----------
-        sigmas : bool, optional
-            If True, include 1-sigma uncertainties in the DataFrame.
-        covariances : bool, optional
-            If True, include covariance matrices in the DataFrame. Covariance matrices
-            will be split into 21 columns, with the lower triangular elements stored.
-
-        Returns
-        -------
-        df : `~pandas.Dataframe`
-            DataFrame containing coordinates.
-        """
-        return coords_to_dataframe(
-            self,
-            ["q", "e", "i", "raan", "ap", "tp"],
-            sigmas=sigmas,
-            covariances=covariances,
-        )
-
-    @classmethod
-    def from_dataframe(
-        cls, df: pd.DataFrame, frame: Literal["ecliptic", "equatorial"]
-    ) -> "CometaryCoordinates":
-        """
-        Create coordinates from a pandas DataFrame.
-
-        Parameters
-        ----------
-        df : `~pandas.Dataframe`
-            DataFrame containing coordinates.
-        frame : {"ecliptic", "equatorial"}
-            Frame in which coordinates are defined.
-
-        Returns
-        -------
-        coords : `~adam_core.coordinates.cometary.CometaryCoordinates`
-            Cometary coordinates.
-        """
-        return coords_from_dataframe(
-            cls, df, coord_names=["q", "e", "i", "raan", "ap", "tp"], frame=frame
-        )
```

### Comparing `adam_core-0.1.0/adam_core/coordinates/conversions.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/conversions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from copy import deepcopy
 from typing import List, Union
 
+import astropy.units
 import numpy as np
 
+from .types import Coordinates
+
+# This module is not maintained.
+__doctest_skip__ = ["*"]
+
 
 def _convert_coordinates_units(
     coords: Union[np.ndarray, np.ma.masked_array], units: List, desired_units: List
 ) -> Union[np.ndarray, np.ma.masked_array]:
     """
     Convert coordinate units to desired units.
 
@@ -88,44 +94,62 @@
 
     covariances_converted = conversion_matrix * covariances
 
     return covariances_converted
 
 
 def convert_coordinates(
-    coords,
-    desired_units: Union[List, dict],
+    coords: Coordinates,
+    desired_units: Union[List[astropy.units.Unit], dict[str, astropy.units.Unit]],
 ):
     """
-    Convert coordinates to desired units.
+    Convert the units in a Coordinates object to desired units.
 
     Parameters
     ----------
-    coords : `~thor.coordinates.Coordinates` (N, D)
+    coords :
         Coordinates that need to be converted.
     desired_units : list, `~numpy.ndarray`, dict
         Desired units for each coordinate dimension expressed as an array-like
         or a dictionary keyed on coordinate dimensions and with values that represent
         the desired units. If a dictionary is passed, then only the coordinate dimensions
         that need to be converted need to be defined.
 
-        desired_units = {
-            "x" : u.km
-        }
-        coordinates_converted = convert_coordinates(coords, desired_units)
-
     Returns
     -------
     coords_converted : `~thor.coordinates.Coordinates` (N, D)
         Coordinates converted to the desired coordinate units.
 
     Raises
     ------
     ValueError : If units or desired_units do not have length D.
     ValueError : If desired_units is not a list, `~numpy.ndarray`, dict
+
+    Examples
+    --------
+    >>> import astropy.units
+    >>> from adam_core.coordinates import CartesianCoordinates, convert_coordinates
+    >>> # By default, x, y, and z are in AU
+    >>> coords = CartesianCoordinates.from_kwargs(
+    ...    x=[1, 1, 1],
+    ...    y=[4, 5, 6],
+    ...    z=[7, 8, 9],
+    ...    vx=[10, 11, 12],
+    ...    vy=[13, 14, 15],
+    ...    vz=[16, 17, 18],
+    ... )
+    >>> desired_units = {
+    ...     "x" : astropy.units.km
+    ... }
+    >>> coordinates_converted = convert_coordinates(coords, desired_units)
+    >>> print(coordinates_converted.x.to_pylist())
+    [149597870.0, 149597870.0, 149597870.0]
+    >>> print(coordinates_converted.y.to_pylist())
+    [4.0, 5.0, 6.0]
+
     """
     N, D = coords.values.shape
 
     desired_units_ = {}
     if isinstance(desired_units, dict):
         for k, v in coords.units.items():
             if k not in desired_units:
```

### Comparing `adam_core-0.1.0/adam_core/coordinates/covariances.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/covariances.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,20 @@
 import logging
-from typing import Callable, List
+from typing import Callable, Optional, Tuple
 
 import numpy as np
-import pandas as pd
 import pyarrow as pa
-from astropy import units as u
-from astropy.table import Table as AstropyTable
-from quivr import ListColumn, Table
+import quivr as qv
+from scipy.linalg import sqrtm
 from scipy.stats import multivariate_normal
 
 from .jacobian import calc_jacobian
 
 logger = logging.getLogger(__name__)
 
-__all__ = [
-    "CoordinateCovariances",
-    "sigmas_to_covariances",
-    "sample_covariance",
-    "transform_covariances_sampling",
-    "transform_covariances_jacobian",
-    "sigmas_to_df",
-    "sigmas_from_df",
-    "covariances_to_df",
-    "covariances_from_df",
-    "covariances_to_table",
-]
-
 COVARIANCE_FILL_VALUE = np.NaN
 
 
 def sigmas_to_covariances(sigmas: np.ndarray) -> np.ndarray:
     """
     Convert an array of standard deviations to an array of covariance matrices.
     Non-diagonal elements are set to zero.
@@ -46,23 +31,21 @@
     """
     D = sigmas.shape[1]
     identity = np.identity(D, dtype=sigmas.dtype)
     covariances = np.einsum("kj,ji->kij", sigmas**2, identity, order="C")
     return covariances
 
 
-class CoordinateCovariances(Table):
+class CoordinateCovariances(qv.Table):
     # TODO: Would be interesting if the dimensionality can be generalized
     #      to D dimensions, so (N, D, D) instead of (N, 6, 6). We would be
     #      able to use this class for the covariance matrices of different
     #      measurments like projections (D = 4) and photometry (D = 1).
 
-    # This is temporary while we await the implementation of
-    # https://github.com/apache/arrow/issues/35599
-    values = ListColumn(pa.float64(), list_size=36)
+    values = qv.LargeListColumn(pa.float64(), nullable=True)
     # When fixed, we should revert to:
     # values = Column(pa.fixed_shape_tensor(pa.float64(), (6, 6)))
 
     @property
     def sigmas(self):
         cov_diag = np.diagonal(self.to_matrix(), axis1=1, axis2=2)
         sigmas = np.sqrt(cov_diag)
@@ -74,19 +57,50 @@
 
         Returns
         -------
         covariances : `numpy.ndarray` (N, 6, 6)
             Covariance matrices for N coordinates in 6 dimensions.
         """
         # return self.values.combine_chunks().to_numpy_ndarray()
-        cov = np.stack(self.values.to_numpy(zero_copy_only=False))
-        if np.all(cov == None):  # noqa: E711
-            return np.full((len(self), 6, 6), np.nan)
-        else:
-            cov = np.stack(cov).reshape(-1, 6, 6)
+        values = self.values.to_numpy(zero_copy_only=False)
+
+        # Try and see if all covariance matrices are None, if so return
+        # an array of NaNs.
+        try:
+            if np.all(values == None):  # noqa: E711
+                return np.full((len(self), 6, 6), np.nan)
+
+        except ValueError as e:
+            err_str = (
+                "The truth value of an array with more than one element is ambiguous."
+                " Use a.any() or a.all()"
+            )
+            if str(e) != err_str:
+                raise e
+
+        # Try to stack the values into a 3D array. If this works, then
+        # all covariance matrices are the same size and we can return
+        # the stacked matrices.
+        try:
+            cov = np.stack(values).reshape(-1, 6, 6)
+
+        # If not then some of the arrays might be None. Lets loop through
+        # the values and fill in the arrays that are missing (None) with NaNs.
+        except ValueError as e:
+            # If we don't get the error we expect, then raise it.
+            if str(e) != "all input arrays must have the same shape":
+                raise e
+            else:
+                for i in range(len(values)):
+                    if values[i] is None:
+                        values[i] = np.full(36, np.nan)
+
+            # Try stacking again
+            cov = np.stack(values).reshape(-1, 6, 6)
+
         return cov
 
     @classmethod
     def from_matrix(cls, covariances: np.ndarray) -> "CoordinateCovariances":
         """
         Create a Covariances object from a 3D array of covariance matrices.
 
@@ -95,18 +109,27 @@
         covariances : `numpy.ndarray` (N, 6, 6)
             Covariance matrices for N coordinates in 6 dimensions.
 
         Returns
         -------
         covariances : `Covariances`
             Covariance matrices for N coordinates in 6 dimensions.
+
+        Raises
+        ------
+        ValueError : If the covariance matrices are not (N, 6, 6)
         """
         # cov = pa.FixedShapeTensorArray.from_numpy_ndarray(covariances)
-        cov = covariances.reshape(-1, 36)
-        return cls.from_kwargs(values=list(cov))
+        if covariances.shape[1:] != (6, 6):
+            raise ValueError(
+                f"Covariance matrices should have shape (N, 6, 6) but got {covariances.shape}"
+            )
+        cov = covariances.flatten()
+        offsets = np.arange(0, (len(covariances) + 1) * 36, 36, dtype=np.int64)
+        return cls.from_kwargs(values=pa.LargeListArray.from_arrays(offsets, cov))
 
     @classmethod
     def from_sigmas(cls, sigmas: np.ndarray) -> "CoordinateCovariances":
         """
         Create a Covariances object from a 2D array of sigmas.
 
         Parameters
@@ -119,93 +142,220 @@
         -------
         covariances : `Covariances`
             Covariance matrices with the diagonal elements set to the
             squares of the input sigmas.
         """
         return cls.from_matrix(sigmas_to_covariances(sigmas))
 
-    def to_dataframe(
-        self,
-        coord_names: List[str] = ["x", "y", "z", "vx", "vy", "vz"],
-        sigmas: bool = False,
-    ) -> pd.DataFrame:
+    @classmethod
+    def nulls(cls, length: int) -> "CoordinateCovariances":
         """
-        Return the covariance matrices represented as lower triangular columns in a pandas DataFrame.
-
+        Create a Covariances object with all covariance matrix elements set to NaN.
         Parameters
         ----------
-        coord_names : `list` of `str`, optional
-            Names of the coordinate axes. Default is ["x", "y", "z", "vx", "vy", "vz"].
-        sigmas : `bool`, optional
-            If True, the standard deviations are added as columns to the DataFrame. Default is False.
+        length : `int`
+            Number of coordinates.
 
         Returns
         -------
-        df : `pandas.DataFrame`
-            Covariance matrices (lower triangular) for N coordinates in 6 dimensions.
+        covariances : `CoordinateCovariances`
+            Covariance matrices for N coordinates in 6 dimensions.
         """
-        df = covariances_to_df(self.to_matrix(), coord_names=coord_names, kind="lower")
-        if sigmas:
-            df_sigmas = sigmas_to_df(self.sigmas, coord_names=coord_names)
-            df = df_sigmas.join(df)
-
-        return df
+        return cls.from_kwargs(
+            values=pa.ListArray.from_arrays(
+                pa.array(np.arange(0, 36 * (length + 1), 36)),
+                pa.nulls(36 * length, pa.float64()),
+            )
+        )
 
-    @classmethod
-    def from_dataframe(
-        cls, df, coord_names: List[str] = ["x", "y", "z", "vx", "vy", "vz"]
-    ) -> "CoordinateCovariances":
+    def is_all_nan(self) -> bool:
         """
-        Create a Covariances object from a pandas DataFrame.
-
-        Parameters
-        ----------
-        df : `pandas.DataFrame`
-            Covariance matrices (lower triangular) for N coordinates in 6 dimensions.
-        coord_names : `list` of `str`, optional
-            Names of the coordinate axes. Default is ["x", "y", "z", "vx", "vy", "vz"].
+        Check if all covariance matrix values are NaN.
 
         Returns
         -------
-        covariances : `CoordinateCovariances`
-            Covariance matrices for N coordinates in 6 dimensions.
+        is_all_nan : bool
+            True if all covariance matrix elements are NaN, False otherwise.
         """
-        try:
-            covariances = covariances_from_df(df, coord_names=coord_names, kind="lower")
-        except KeyError:
-            sigmas = sigmas_from_df(df, coord_names=coord_names)
-            covariances = sigmas_to_covariances(sigmas)
+        return np.all(np.isnan(self.to_matrix()))
 
-        return cls.from_matrix(covariances)
 
-
-def sample_covariance(
-    mean: np.ndarray, cov: np.ndarray, num_samples: int = 100000
-) -> np.ndarray:
+def sample_covariance_random(
+    mean: np.ndarray,
+    cov: np.ndarray,
+    num_samples: int = 10000,
+    seed: Optional[int] = None,
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
     Sample a multivariate Gaussian distribution with given
     mean and covariances.
 
+    The returned weights will be equal to 1 / num_samples so that
+    each sample is equally weighted. Weights are returned from this function
+    so its interface is identical to that of
+    `~adam_core.coordinates.covariances.sample_covariance_sigma_points`.
+
     Parameters
     ----------
     mean : `~numpy.ndarray` (D)
         Multivariate mean of the Gaussian distribution.
     cov : `~numpy.ndarray` (D, D)
         Multivariate variance-covariance matrix of the Gaussian distribution.
     num_samples : int, optional
         Number of samples to draw from the distribution.
 
     Returns
     -------
     samples : `~numpy.ndarray` (num_samples, D)
         The drawn samples row-by-row.
+    W: `~numpy.ndarray` (num_samples)
+        Weights of the samples.
+    W_cov: `~numpy.ndarray` (num_samples)
+        Weights of the samples to reconstruct covariance matrix.
     """
-    normal = multivariate_normal(mean=mean, cov=cov, allow_singular=True)
+    normal = multivariate_normal(mean=mean, cov=cov, allow_singular=True, seed=seed)
     samples = normal.rvs(num_samples)
-    return samples
+    W = np.full(num_samples, 1 / num_samples)
+    W_cov = np.full(num_samples, 1 / num_samples)
+    return samples, W, W_cov
+
+
+def sample_covariance_sigma_points(
+    mean: np.ndarray,
+    cov: np.ndarray,
+    alpha: float = 1,
+    beta: float = 0.0,
+    kappa: float = 0.0,
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+    """
+    Create sigma-point samples of a multivariate Gaussian distribution
+    with given mean and covariances.
+
+    Parameters
+    ----------
+    mean : `~numpy.ndarray` (D)
+        Multivariate mean of the Gaussian distribution.
+    cov : `~numpy.ndarray` (D, D)
+        Multivariate variance-covariance matrix of the Gaussian distribution.
+    alpha : float, optional
+        Spread of the sigma points between 1e^-2 and 1.
+    beta : float, optional
+        Prior knowledge of the distribution usually set to 2 for a Gaussian.
+    kappa : float, optional
+        Secondary scaling parameter usually set to 0.
+
+    Returns
+    -------
+    sigma_points : `~numpy.ndarray` (2 * D + 1, D)
+        Sigma points drawn from the distribution.
+    W: `~numpy.ndarray` (2 * D + 1)
+        Weights of the sigma points.
+    W_cov: `~numpy.ndarray` (2 * D + 1)
+        Weights of the sigma points to reconstruct covariance matrix.
+
+    References
+    ----------
+    [1] Wan, E. A; Van Der Merwe, R. (2000). The unscented Kalman filter for nonlinear estimation.
+        Proceedings of the IEEE 2000 Adaptive Systems for Signal Processing,
+        Communications, and Control Symposium, 153-158.
+        https://doi.org/10.1109/ASSPCC.2000.882463
+    """
+    # Calculate the dimensionality of the distribution
+    D = mean.shape[0]
+
+    # See equation 15 in Wan & Van Der Merwe (2000) [1]
+    N = 2 * D + 1
+    sigma_points = np.empty((N, D))
+    W = np.empty(N)
+    W_cov = np.empty(N)
+
+    # Calculate the scaling parameter lambda
+    lambd = alpha**2 * (D + kappa) - D
+
+    # First sigma point is the mean
+    sigma_points[0] = mean
+
+    # Beta is used to encode prior knowledge about the distribution.
+    # If the distribution is a well-constrained Gaussian, beta = 2 is optimal
+    # but lets set beta to 0 for now which has the effect of not weighting the mean state
+    # with 0 for the covariance matrix. This is generally better for more distributions.
+    # Calculate the weights for mean and the covariance matrix
+    # Weight are used to reconstruct the mean and covariance matrix from the sigma points
+    W[0] = lambd / (D + lambd)
+    W_cov[0] = W[0] + (1 - alpha**2 + beta)
+
+    # Take the matrix square root of the scaled covariance matrix.
+    # Sometimes you'll see this done with a Cholesky decomposition for speed
+    # but sqrtm is sufficiently optimized for this use case and typically provides
+    # better results
+    L = sqrtm((D + lambd) * cov)
+
+    # Calculate the remaining sigma points
+    for i in range(D):
+        offset = L[i]
+        sigma_points[i + 1] = mean + offset
+        sigma_points[i + 1 + D] = mean - offset
+
+    # The weights for the remaining sigma points are the same
+    # for the mean and the covariance matrix
+    W[1:] = 1 / (2 * (D + lambd))
+    W_cov[1:] = 1 / (2 * (D + lambd))
+
+    return sigma_points, W, W_cov
+
+
+def weighted_mean(samples: np.ndarray, W: np.ndarray) -> np.ndarray:
+    """
+    Calculate the weighted mean of a set of samples.
+
+    Parameters
+    ----------
+    samples : `~numpy.ndarray` (N, D)
+        Samples drawn from the distribution (these can be randomly drawn
+        or sigma points)
+    W: `~numpy.ndarray` (N)
+        Weights of the samples.
+
+    Returns
+    -------
+    mean : `~numpy.ndarray` (D)
+        Mean calculated from the samples and weights.
+    """
+    return np.dot(W, samples)
+
+
+def weighted_covariance(
+    mean: np.ndarray, samples: np.ndarray, W_cov: np.ndarray
+) -> np.ndarray:
+    """
+    Calculate a covariance matrix from samples and their corresponding weights.
+
+    Parameters
+    ----------
+    mean : `~numpy.ndarray` (D)
+        Mean calculated from the samples and weights.
+        See `~adam_core.coordinates.covariances.weighted_mean`.
+    samples : `~numpy.ndarray` (N, D)
+        Samples drawn from the distribution (these can be randomly drawn
+        or sigma points)
+    W_cov: `~numpy.ndarray` (N)
+        Weights of the samples to reconstruct covariance matrix.
+
+    Returns
+    -------
+    cov : `~numpy.ndarray` (D, D)
+        Covariance matrix calculated from the samples and weights.
+    """
+    # Calculate the covariance matrix from the sigma points and weights
+    # `~numpy.cov` does not support negative weights so we will calculate
+    # the covariance manually
+    # cov = np.cov(samples, aweights=W_cov, rowvar=False, bias=True)
+    residual = samples - mean
+    cov = (W_cov * residual.T) @ residual
+    return cov
 
 
 def transform_covariances_sampling(
     coords: np.ndarray,
     covariances: np.ndarray,
     func: Callable,
     num_samples: int = 100000,
@@ -229,15 +379,15 @@
     Returns
     -------
     covariances_out : `~numpy.ndarray` (N, D, D)
         Transformed covariance matrices.
     """
     covariances_out = []
     for coord, covariance in zip(coords, covariances):
-        samples = sample_covariance(coord, covariance, num_samples)
+        samples, W, W_cov = sample_covariance_random(coord, covariance, num_samples)
         samples_converted = func(samples)
         covariances_out.append(np.cov(samples_converted.T))
 
     covariances_out = np.stack(covariances_out)
     return covariances_out
 
 
@@ -266,283 +416,7 @@
     -------
     covariances_out : `~numpy.ndarray` (N, D, D)
         Transformed covariance matrices.
     """
     jacobian = calc_jacobian(coords, _func, **kwargs)
     covariances = jacobian @ covariances @ np.transpose(jacobian, axes=(0, 2, 1))
     return covariances
-
-
-def sigmas_to_df(
-    sigmas: np.ndarray,
-    coord_names: List[str] = ["x", "y", "z", "vx", "vy", "vz"],
-) -> pd.DataFrame:
-    """
-    Place sigmas into a `pandas.DataFrame`.
-
-    Parameters
-    ----------
-    sigmas : `~numpy.ndarray` (N, D)
-        1-sigma uncertainty values for each coordinate dimension D.
-    coord_names : List[str]
-        Names of the coordinate columns, will be used to determine column names for
-        each element in the triangular covariance matrix.
-
-    Returns
-    -------
-    df : `~pandas.DataFrame`
-        DataFrame containing covariances in either upper or lower triangular
-        form.
-    """
-    N, D = sigmas.shape
-
-    data = {}
-    for i in range(D):
-        data[f"sigma_{coord_names[i]}"] = sigmas[:, i]
-
-    return pd.DataFrame(data)
-
-
-def sigmas_from_df(
-    df: pd.DataFrame,
-    coord_names: List[str] = ["x", "y", "z", "vx", "vy", "vz"],
-) -> np.ndarray:
-    """
-    Read sigmas from a `~pandas.DataFrame`.
-
-    Parameters
-    ----------
-    df : `~pandas.DataFrame`
-        DataFrame containing covariances in either upper or lower triangular
-        form.
-    coord_names : List[str]
-        Names of the coordinate columns, will be used to determine column names for
-        each element in the triangular covariance matrix.
-
-    Returns
-    -------
-    sigmas : `~numpy.ndarray` (N, D)
-        1-sigma uncertainty values for each coordinate dimension D.
-    """
-    N = len(df)
-    D = len(coord_names)
-    sigmas = np.zeros((N, D), dtype=np.float64)
-    sigmas.fill(COVARIANCE_FILL_VALUE)
-
-    for i in range(D):
-        try:
-            sigmas[:, i] = df[f"sigma_{coord_names[i]}"].values
-
-        except KeyError:
-            logger.debug(f"No sigma column found for dimension {coord_names[i]}.")
-
-    return sigmas
-
-
-def covariances_to_df(
-    covariances: np.ndarray,
-    coord_names: List[str] = ["x", "y", "z", "vx", "vy", "vz"],
-    kind: str = "lower",
-) -> pd.DataFrame:
-    """
-    Place covariance matrices into a `pandas.DataFrame`. Splits the covariance matrices
-    into either upper or lower triangular form and then adds one column per dimension.
-
-    Parameters
-    ----------
-    covariances : `~numpy.ndarray` (N, D, D)
-        3D array of covariance matrices.
-    coord_names : List[str]
-        Names of the coordinate columns, will be used to determine column names for
-        each element in the triangular covariance matrix.
-    kind : {'upper', 'lower'}
-        The orientation of the triangular representation.
-
-    Returns
-    -------
-    df : `~pandas.DataFrame`
-        DataFrame containing covariances in either upper or lower triangular
-        form.
-
-    Raises
-    ------
-    ValueError : If kind is not one of {'upper', 'lower'}
-
-    """
-    N, D, D = covariances.shape
-
-    if kind == "upper":
-        ii, jj = np.triu_indices(D)
-    elif kind == "lower":
-        ii, jj = np.tril_indices(D)
-    else:
-        err = "kind should be one of {'upper', 'lower'}"
-        raise ValueError(err)
-
-    data = {}
-    for i, j in zip(ii, jj):
-        data[f"cov_{coord_names[i]}_{coord_names[j]}"] = covariances[:, i, j]
-
-    return pd.DataFrame(data)
-
-
-def covariances_from_df(
-    df: pd.DataFrame,
-    coord_names: List[str] = ["x", "y", "z", "vx", "vy", "vz"],
-    kind: str = "lower",
-) -> np.ndarray:
-    """
-    Read covariance matrices from a `~pandas.DataFrame`.
-
-    Parameters
-    ----------
-    df : `~pandas.DataFrame`
-        DataFrame containing covariances in either upper or lower triangular
-        form.
-    coord_names : List[str]
-        Names of the coordinate columns, will be used to determine column names for
-        each element in the triangular covariance matrix.
-    kind : {'upper', 'lower'}
-        The orientation of the triangular representation.
-
-    Returns
-    -------
-    covariances : `~numpy.ndarray` (N, D, D)
-        3D array of covariance matrices.
-
-    Raises
-    ------
-    ValueError : If kind is not one of {'upper', 'lower'}
-    """
-    N = len(df)
-    D = len(coord_names)
-    covariances = np.zeros((N, D, D), dtype=np.float64)
-    covariances.fill(COVARIANCE_FILL_VALUE)
-
-    if kind == "upper":
-        ii, jj = np.triu_indices(D)
-    elif kind == "lower":
-        ii, jj = np.tril_indices(D)
-    else:
-        err = "kind should be one of {'upper', 'lower'}"
-        raise ValueError(err)
-
-    for i, j in zip(ii, jj):
-        try:
-            covariances[:, i, j] = df[f"cov_{coord_names[i]}_{coord_names[j]}"].values
-            covariances[:, j, i] = covariances[:, i, j]
-        except KeyError:
-            logger.debug(
-                "No covariance column found for dimensions"
-                f" {coord_names[i]},{coord_names[j]}."
-            )
-
-    return covariances
-
-
-def covariances_to_table(
-    covariances: np.ma.masked_array,
-    coord_names: List[str] = ["x", "y", "z", "vx", "vy", "vz"],
-    coord_units=[u.au, u.au, u.au, u.au / u.d, u.au / u.d, u.au / u.d],
-    kind: str = "lower",
-) -> AstropyTable:
-    """
-    Place covariance matrices into a `astropy.table.table.Table`. Splits the covariance matrices
-    into either upper or lower triangular form and then adds one column per dimension.
-
-    Parameters
-    ----------
-    covariances : `~numpy.ma.masked_array` (N, D, D)
-        3D array of covariance matrices.
-    coord_names : List[str]
-        Names of the coordinate columns, will be used to determine column names for
-        each element in the triangular covariance matrix.
-    coord_units : List[]
-        The unit for each coordinate, will be used to determination the units for
-        element in the triangular covariance matrix.
-    kind : {'upper', 'lower'}
-        The orientation of the triangular representation.
-
-    Returns
-    -------
-    table : `~astropy.table.table.Table`
-        Table containing covariances in either upper or lower triangular
-        form.
-
-    Raises
-    ------
-    ValueError : If kind is not one of {'upper', 'lower'}
-    """
-    N, D, D = covariances.shape
-
-    if kind == "upper":
-        ii, jj = np.triu_indices(D)
-    elif kind == "lower":
-        ii, jj = np.tril_indices(D)
-    else:
-        err = "kind should be one of {'upper', 'lower'}"
-        raise ValueError(err)
-
-    data = {}
-    for i, j in zip(ii, jj):
-        data[f"cov_{coord_names[i]}_{coord_names[j]}"] = (
-            covariances[:, i, j] * coord_units[i] * coord_units[j]
-        )
-
-    return AstropyTable(data)
-
-
-def covariances_from_table(
-    table: AstropyTable,
-    coord_names: List[str] = ["x", "y", "z", "vx", "vy", "vz"],
-    kind: str = "lower",
-) -> np.ma.masked_array:
-    """
-    Read covariance matrices from a `~astropy.table.table.Table`.
-
-    Parameters
-    ----------
-    table : `~astropy.table.table.Table`
-        Table containing covariances in either upper or lower triangular
-        form.
-    coord_names : List[str]
-        Names of the coordinate columns, will be used to determine column names for
-        each element in the triangular covariance matrix.
-    kind : {'upper', 'lower'}
-        The orientation of the triangular representation.
-
-    Returns
-    -------
-    covariances : `~numpy.ma.masked_array` (N, D, D)
-        3D array of covariance matrices.
-
-    Raises
-    ------
-    ValueError : If kind is not one of {'upper', 'lower'}
-    """
-    N = len(table)
-    D = len(coord_names)
-    covariances = np.ma.zeros((N, D, D), dtype=np.float64)
-    covariances.fill_value = COVARIANCE_FILL_VALUE
-    covariances.mask = np.ones((N, D, D), dtype=bool)
-
-    if kind == "upper":
-        ii, jj = np.triu_indices(D)
-    elif kind == "lower":
-        ii, jj = np.tril_indices(D)
-    else:
-        err = "kind should be one of {'upper', 'lower'}"
-        raise ValueError(err)
-
-    for i, j in zip(ii, jj):
-        try:
-            covariances[:, i, j] = table[
-                f"cov_{coord_names[i]}_{coord_names[j]}"
-            ].values
-            covariances[:, j, i] = covariances[:, i, j]
-        except KeyError:
-            logger.debug(
-                "No covariance column found for dimensions"
-                f" {coord_names[i]},{coord_names[j]}."
-            )
-
-    return covariances
```

### Comparing `adam_core-0.1.0/adam_core/coordinates/jacobian.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/jacobian.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.1.0/adam_core/coordinates/keplerian.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/keplerian.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,89 @@
-from typing import TYPE_CHECKING, Literal
+from __future__ import annotations
 
 import numpy as np
-import pandas as pd
-from astropy import units as u
-from quivr import Float64Column, StringAttribute, Table
+import quivr as qv
 
-from .cartesian import CartesianCoordinates
+from ..time import Timestamp
+from . import cartesian, cometary, spherical
 from .covariances import CoordinateCovariances, transform_covariances_jacobian
-from .io import coords_from_dataframe, coords_to_dataframe
 from .origin import Origin
-from .times import Times
-
-if TYPE_CHECKING:
-    from .cometary import CometaryCoordinates
-    from .spherical import SphericalCoordinates
-
 
 __all__ = [
     "KeplerianCoordinates",
-    "KEPLERIAN_COLS",
-    "KEPLERIAN_UNITS",
 ]
 
-KEPLERIAN_COLS = {}
-KEPLERIAN_UNITS = {}
-for i in ["a", "e", "i", "raan", "ap", "M"]:
-    KEPLERIAN_COLS[i] = i
-KEPLERIAN_UNITS["a"] = u.au
-KEPLERIAN_UNITS["e"] = u.dimensionless_unscaled
-KEPLERIAN_UNITS["i"] = u.deg
-KEPLERIAN_UNITS["raan"] = u.deg
-KEPLERIAN_UNITS["ap"] = u.deg
-KEPLERIAN_UNITS["M"] = u.deg
-
-
-class KeplerianCoordinates(Table):
-
-    a = Float64Column(nullable=False)
-    e = Float64Column(nullable=False)
-    i = Float64Column(nullable=False)
-    raan = Float64Column(nullable=False)
-    ap = Float64Column(nullable=False)
-    M = Float64Column(nullable=False)
-    times = Times.as_column(nullable=True)
-    covariances = CoordinateCovariances.as_column(nullable=True)
-    origin = Origin.as_column(nullable=False)
-    frame = StringAttribute()
+
+class KeplerianCoordinates(qv.Table):
+
+    a = qv.Float64Column()
+    e = qv.Float64Column()
+    i = qv.Float64Column()
+    raan = qv.Float64Column()
+    ap = qv.Float64Column()
+    M = qv.Float64Column()
+    time = Timestamp.as_column(nullable=True)
+    covariance = CoordinateCovariances.as_column(nullable=True)
+    origin = Origin.as_column()
+    frame = qv.StringAttribute(default="unspecified")
 
     @property
     def values(self) -> np.ndarray:
-        return np.array(self.table.select(["a", "e", "i", "raan", "ap", "M"])).T
+        return np.array(self.table.select(["a", "e", "i", "raan", "ap", "M"]))
 
     @property
     def sigma_a(self) -> np.ndarray:
         """
         1-sigma uncertainty in semi-major axis.
         """
-        return self.covariances.sigmas[:, 0]
+        return self.covariance.sigmas[:, 0]
 
     @property
     def sigma_e(self) -> np.ndarray:
         """
         1-sigma uncertainty in eccentricity.
         """
-        return self.covariances.sigmas[:, 1]
+        return self.covariance.sigmas[:, 1]
 
     @property
     def sigma_i(self) -> np.ndarray:
         """
         1-sigma uncertainty in inclination.
         """
-        return self.covariances.sigmas[:, 2]
+        return self.covariance.sigmas[:, 2]
 
     @property
     def sigma_raan(self) -> np.ndarray:
         """
         1-sigma uncertainty in right ascension of the ascending node.
         """
-        return self.covariances.sigmas[:, 3]
+        return self.covariance.sigmas[:, 3]
 
     @property
     def sigma_ap(self) -> np.ndarray:
         """
         1-sigma uncertainty in argument of periapsis.
         """
-        return self.covariances.sigmas[:, 4]
+        return self.covariance.sigmas[:, 4]
 
     @property
     def sigma_M(self) -> np.ndarray:
         """
         1-sigma uncertainty in mean anomaly.
         """
-        return self.covariances.sigmas[:, 5]
+        return self.covariance.sigmas[:, 5]
 
     @property
     def q(self) -> np.ndarray:
         """
         Periapsis distance.
         """
-        return self.a.to_numpy() * (1 - self.e.to_numpy())
+        from ..dynamics.kepler import calc_periapsis_distance
+
+        return np.array(calc_periapsis_distance(self.a.to_numpy(), self.e.to_numpy()))
 
     @q.setter
     def q(self, value):
         err = (
             "Cannot set periapsis distance (q) as it is"
             " derived from semi-major axis (a) and eccentricity (e)."
         )
@@ -117,15 +98,17 @@
         raise ValueError(err)
 
     @property
     def Q(self) -> np.ndarray:
         """
         Apoapsis distance.
         """
-        return self.a.to_numpy() * (1 + self.e.to_numpy())
+        from ..dynamics.kepler import calc_apoapsis_distance
+
+        return np.array(calc_apoapsis_distance(self.a.to_numpy(), self.e.to_numpy()))
 
     @Q.setter
     def Q(self, value):
         err = (
             "Cannot set apoapsis distance (Q) as it is"
             " derived from semi-major axis (a) and eccentricity (e)."
         )
@@ -140,15 +123,17 @@
         raise ValueError(err)
 
     @property
     def p(self) -> np.ndarray:
         """
         Semi-latus rectum.
         """
-        return self.a.to_numpy() / (1 - self.e.to_numpy() ** 2)
+        from ..dynamics.kepler import calc_semi_latus_rectum
+
+        return np.array(calc_semi_latus_rectum(self.a.to_numpy(), self.e.to_numpy()))
 
     @p.setter
     def p(self, value):
         err = (
             "Cannot set semi-latus rectum (p) as it is"
             " derived from semi-major axis (a) and eccentricity (e)."
         )
@@ -163,103 +148,132 @@
         raise ValueError(err)
 
     @property
     def P(self) -> np.ndarray:
         """
         Period.
         """
-        return np.sqrt(4 * np.pi**2 * self.a.to_numpy() ** 3 / self.origin.mu)
+        from ..dynamics.kepler import calc_period
+
+        return np.array(calc_period(self.a.to_numpy(), self.origin.mu()))
 
     @P.setter
     def P(self, value):
         err = (
             "Cannot set period (P) as it is"
             " derived from semi-major axis (a) and gravitational parameter (mu)."
         )
         raise ValueError(err)
 
-    @p.deleter
+    @P.deleter
     def P(self):
         err = (
             "Cannot delete period (P) as it is"
             " derived from semi-major axis (a) and gravitational parameter (mu)."
         )
         raise ValueError(err)
 
-    def to_cartesian(self) -> CartesianCoordinates:
+    @property
+    def n(self):
+        """
+        Mean motion in degrees.
+        """
+        from ..dynamics.kepler import calc_mean_motion
+
+        return np.degrees(
+            np.array(calc_mean_motion(self.a.to_numpy(), self.origin.mu()))
+        )
+
+    @n.setter
+    def n(self, value):
+        err = (
+            "Cannot set mean motion (n) as it is"
+            " derived from semi-major axis (a) and gravitational parameter (mu)."
+        )
+        raise ValueError(err)
+
+    @n.deleter
+    def n(self):
+        err = (
+            "Cannot delete mean motion (n) as it is"
+            " derived from semi-major axis (a) and gravitational parameter (mu)."
+        )
+        raise ValueError(err)
+
+    def to_cartesian(self) -> cartesian.CartesianCoordinates:
         from .transform import _keplerian_to_cartesian_a, keplerian_to_cartesian
 
         # Extract gravitational parameter from origin
-        mu = self.origin.mu
+        mu = self.origin.mu()
 
         coords_cartesian = keplerian_to_cartesian(
             self.values,
             mu=mu,
             max_iter=1000,
             tol=1e-15,
         )
         coords_cartesian = np.array(coords_cartesian)
 
-        covariances_keplerian = self.covariances.to_matrix()
-        if not np.all(np.isnan(covariances_keplerian)):
+        if not self.covariance.is_all_nan():
+            covariances_keplerian = self.covariance.to_matrix()
             covariances_cartesian = transform_covariances_jacobian(
                 self.values,
                 covariances_keplerian,
                 _keplerian_to_cartesian_a,
-                in_axes=(0, None, None, None),
+                in_axes=(0, 0, None, None),
                 out_axes=0,
                 mu=mu,
                 max_iter=1000,
                 tol=1e-15,
             )
         else:
             covariances_cartesian = np.empty(
                 (len(coords_cartesian), 6, 6), dtype=np.float64
             )
             covariances_cartesian.fill(np.nan)
 
         covariances_cartesian = CoordinateCovariances.from_matrix(covariances_cartesian)
-        coords = CartesianCoordinates.from_kwargs(
+        coords = cartesian.CartesianCoordinates.from_kwargs(
             x=coords_cartesian[:, 0],
             y=coords_cartesian[:, 1],
             z=coords_cartesian[:, 2],
             vx=coords_cartesian[:, 3],
             vy=coords_cartesian[:, 4],
             vz=coords_cartesian[:, 5],
-            times=self.times,
-            covariances=covariances_cartesian,
+            time=self.time,
+            covariance=covariances_cartesian,
             origin=self.origin,
             frame=self.frame,
         )
 
         return coords
 
     @classmethod
-    def from_cartesian(cls, cartesian: CartesianCoordinates):
+    def from_cartesian(cls, cartesian: cartesian.CartesianCoordinates):
         from .transform import _cartesian_to_keplerian6, cartesian_to_keplerian
 
         # Extract gravitational parameter from origin
-        mu = cartesian.origin.mu
+        mu = cartesian.origin.mu()
 
         coords_keplerian = cartesian_to_keplerian(
             cartesian.values,
-            cartesian.times.to_astropy().tdb.mjd,
+            cartesian.time.to_numpy(),
             mu=mu,
         )
         coords_keplerian = np.array(coords_keplerian)
 
-        cartesian_covariances = cartesian.covariances.to_matrix()
-        if not np.all(np.isnan(cartesian_covariances)):
+        if not cartesian.covariance.is_all_nan():
+            cartesian_covariances = cartesian.covariance.to_matrix()
             covariances_keplerian = transform_covariances_jacobian(
                 cartesian.values,
                 cartesian_covariances,
                 _cartesian_to_keplerian6,
-                in_axes=(0, 0, None),
+                in_axes=(0, 0, 0),
                 out_axes=0,
-                t0=cartesian.times.to_astropy().tdb.mjd,
+                t0=cartesian.time.to_numpy(),
                 mu=mu,
             )
         else:
             covariances_keplerian = np.empty(
                 (len(coords_keplerian), 6, 6), dtype=np.float64
             )
             covariances_keplerian.fill(np.nan)
@@ -268,84 +282,31 @@
         coords = cls.from_kwargs(
             a=coords_keplerian[:, 0],
             e=coords_keplerian[:, 4],
             i=coords_keplerian[:, 5],
             raan=coords_keplerian[:, 6],
             ap=coords_keplerian[:, 7],
             M=coords_keplerian[:, 8],
-            times=cartesian.times,
-            covariances=covariances_keplerian,
+            time=cartesian.time,
+            covariance=covariances_keplerian,
             origin=cartesian.origin,
             frame=cartesian.frame,
         )
         return coords
 
-    def to_cometary(self) -> "CometaryCoordinates":
-        from .cometary import CometaryCoordinates
-
-        return CometaryCoordinates.from_cartesian(self.to_cartesian())
+    def to_cometary(self) -> cometary.CometaryCoordinates:
+        return cometary.CometaryCoordinates.from_cartesian(self.to_cartesian())
 
     @classmethod
     def from_cometary(
-        cls, cometary_coordinates: "CometaryCoordinates"
-    ) -> "KeplerianCoordinates":
+        cls, cometary_coordinates: cometary.CometaryCoordinates
+    ) -> KeplerianCoordinates:
         return cls.from_cartesian(cometary_coordinates.to_cartesian())
 
-    def to_spherical(self) -> "SphericalCoordinates":
-        from .spherical import SphericalCoordinates
-
-        return SphericalCoordinates.from_cartesian(self.to_cartesian())
+    def to_spherical(self) -> spherical.SphericalCoordinates:
+        return spherical.SphericalCoordinates.from_cartesian(self.to_cartesian())
 
     @classmethod
     def from_spherical(
-        cls, spherical_coordinates: "SphericalCoordinates"
-    ) -> "KeplerianCoordinates":
+        cls, spherical_coordinates: spherical.SphericalCoordinates
+    ) -> KeplerianCoordinates:
         return cls.from_cartesian(spherical_coordinates.to_cartesian())
-
-    def to_dataframe(
-        self, sigmas: bool = False, covariances: bool = True
-    ) -> pd.DataFrame:
-        """
-        Convert coordinates to a pandas DataFrame.
-
-        Parameters
-        ----------
-        sigmas : bool, optional
-            If True, include 1-sigma uncertainties in the DataFrame.
-        covariances : bool, optional
-            If True, include covariance matrices in the DataFrame. Covariance matrices
-            will be split into 21 columns, with the lower triangular elements stored.
-
-        Returns
-        -------
-        df : `~pandas.Dataframe`
-            DataFrame containing coordinates.
-        """
-        return coords_to_dataframe(
-            self,
-            ["a", "e", "i", "raan", "ap", "M"],
-            sigmas=sigmas,
-            covariances=covariances,
-        )
-
-    @classmethod
-    def from_dataframe(
-        cls, df: pd.DataFrame, frame: Literal["ecliptic", "equatorial"]
-    ) -> "KeplerianCoordinates":
-        """
-        Create coordinates from a pandas DataFrame.
-
-        Parameters
-        ----------
-        df : `~pandas.Dataframe`
-            DataFrame containing coordinates.
-        frame : {"ecliptic", "equatorial"}
-            Frame in which coordinates are defined.
-
-        Returns
-        -------
-        coords : `~adam_core.coordinates.keplerian.KeplerianCoordinates`
-            Keplerian coordinates.
-        """
-        return coords_from_dataframe(
-            cls, df, coord_names=["a", "e", "i", "raan", "ap", "M"], frame=frame
-        )
```

### Comparing `adam_core-0.1.0/adam_core/coordinates/origin.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/origin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from enum import Enum
-from typing import Optional
 
 import numpy as np
-import pyarrow as pa
-from quivr import StringColumn, Table
+import pyarrow.compute as pc
+import quivr as qv
 
 from ..constants import KM_P_AU, S_P_DAY
 
 logger = logging.getLogger(__name__)
 
 
 class OriginCodes(Enum):
@@ -45,67 +44,88 @@
     MERCURY_BARYCENTER = _convert_mu_units(22032.080486418)
     VENUS_BARYCENTER = _convert_mu_units(324858.592000)
     MARS_BARYCENTER = _convert_mu_units(42828.375816)
     JUPITER_BARYCENTER = _convert_mu_units(126712764.100000)
     SATURN_BARYCENTER = _convert_mu_units(37940584.841800)
     URANUS_BARYCENTER = _convert_mu_units(5794556.400000)
     NEPTUNE_BARYCENTER = _convert_mu_units(6836527.100580)
+    PLUTO_BARYCENTER = _convert_mu_units(975.500000)
     SUN = _convert_mu_units(132712440041.279419)
     MERCURY = _convert_mu_units(22031.868551)
     VENUS = _convert_mu_units(324858.592000)
     EARTH = _convert_mu_units(398600.435507)
     MOON = _convert_mu_units(4902.800118)
 
+    @classmethod
+    def SOLAR_SYSTEM_BARYCENTER(cls) -> float:
+        """
+        Return the gravitational parameter of the Solar System barycenter as approximated
+        by adding the gravitational parameters of the Sun, Mercury, Venus, Earth, Moon,
+        Mars, Jupiter, Uranus, and Neptune.
+
+        Returns
+        -------
+        mu : float
+            The gravitational parameter of the Solar System barycenter in au^3 / day^2.
+        """
+        return (
+            cls.SUN
+            + cls.MERCURY_BARYCENTER
+            + cls.VENUS_BARYCENTER
+            + cls.EARTH
+            + cls.MOON
+            + cls.MARS_BARYCENTER
+            + cls.JUPITER_BARYCENTER
+            + cls.URANUS_BARYCENTER
+            + cls.NEPTUNE_BARYCENTER
+            + cls.PLUTO_BARYCENTER
+        )
+
 
 # TODO: Replace with DictionaryColumn or similar
 #       Investigate whether this class is even necessary
-class Origin(Table):
-
-    code = StringColumn(nullable=False)
-
-    def __init__(self, table: pa.Table, mu: Optional[float] = None):
-        super().__init__(table)
-        self._mu = mu
-
-    def with_table(self, table: pa.Table) -> "Origin":
-        return super().with_table(table, mu=self.mu)
+class Origin(qv.Table):
+    code = qv.LargeStringColumn()
 
     def __eq__(self, other: object) -> np.ndarray:
         if isinstance(other, (str, np.ndarray)):
             codes = self.code.to_numpy(zero_copy_only=False)
             return codes == other
+        elif isinstance(other, OriginCodes):
+            codes = self.code.to_numpy(zero_copy_only=False)
+            return codes == other.name
         elif isinstance(other, Origin):
             codes = self.code.to_numpy(zero_copy_only=False)
             other_codes = other.code.to_numpy(zero_copy_only=False)
             return codes == other_codes
         else:
             raise TypeError(f"Cannot compare Origin to type: {type(other)}")
 
     def __ne__(self, other: object) -> np.ndarray:
         return ~self.__eq__(other)
 
-    @property
-    def mu(self):
-        if self._mu is None:
-            logger.debug(
-                "Origin.mu called without mu set. Finding mu in OriginGravitationalParameters."
-            )
-            codes = np.array(self.code)
-            if len(np.unique(codes)) > 1:
-                raise ValueError("Origin.mu called on table with multiple origins.")
-
-            try:
-                return OriginGravitationalParameters[codes[0]].value
-            except KeyError:
-                raise ValueError(
-                    "Origin.mu called on table with unrecognized origin code."
-                )
-        else:
-            return self._mu
+    def mu(self) -> np.ndarray:
+        """
+        Return the gravitational parameter of the origin.
+
+        Returns
+        -------
+        mu : `~numpy.ndarray` (N)
+            The gravitational parameter of the origin in au^3 / day^2.
+
+        Raises
+        ------
+        ValueError
+            If the origin code is not recognized.
+        """
+        mu = np.empty(len(self.code), dtype=np.float64)
+        for code in pc.unique(self.code):
+            code = code.as_py()
+            mask = pc.equal(self.code, code).to_numpy(zero_copy_only=False)
+            if code == "SOLAR_SYSTEM_BARYCENTER":
+                mu[mask] = OriginGravitationalParameters.SOLAR_SYSTEM_BARYCENTER()
+            elif code in OriginGravitationalParameters.__members__:
+                mu[mask] = OriginGravitationalParameters[code].value
+            else:
+                raise ValueError(f"Unknown origin code: {code}")
 
-    @mu.setter
-    def mu(self, mu: float):
-        self._mu = mu
-
-    @mu.deleter
-    def mu(self):
-        self._mu = None
+        return mu
```

### Comparing `adam_core-0.1.0/adam_core/coordinates/spherical.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/spherical.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,103 +1,82 @@
-from typing import TYPE_CHECKING, Literal
+from __future__ import annotations
 
 import numpy as np
-import pandas as pd
-from astropy import units as u
-from quivr import Float64Column, StringAttribute, Table
+import quivr as qv
 
-from .cartesian import CartesianCoordinates
+from ..time import Timestamp
+from . import cartesian, cometary, keplerian
 from .covariances import CoordinateCovariances, transform_covariances_jacobian
-from .io import coords_from_dataframe, coords_to_dataframe
 from .origin import Origin
-from .times import Times
-
-if TYPE_CHECKING:
-    from .cometary import CometaryCoordinates
-    from .keplerian import KeplerianCoordinates
-
 
 __all__ = [
     "SphericalCoordinates",
-    "SPHERICAL_COLS",
-    "SPHERICAL_UNITS",
 ]
 
-SPHERICAL_COLS = {}
-SPHERICAL_UNITS = {}
-for i in ["rho", "lon", "lat", "vrho", "vlon", "vlat"]:
-    SPHERICAL_COLS[i] = i
-SPHERICAL_UNITS["rho"] = u.au
-SPHERICAL_UNITS["lon"] = u.deg
-SPHERICAL_UNITS["lat"] = u.deg
-SPHERICAL_UNITS["vrho"] = u.au / u.d
-SPHERICAL_UNITS["vlon"] = u.deg / u.d
-SPHERICAL_UNITS["vlat"] = u.deg / u.d
-
-
-class SphericalCoordinates(Table):
-
-    rho = Float64Column(nullable=True)
-    lon = Float64Column(nullable=True)
-    lat = Float64Column(nullable=True)
-    vrho = Float64Column(nullable=True)
-    vlon = Float64Column(nullable=True)
-    vlat = Float64Column(nullable=True)
-    times = Times.as_column(nullable=True)
-    covariances = CoordinateCovariances.as_column(nullable=True)
-    origin = Origin.as_column(nullable=False)
-    frame = StringAttribute()
+
+class SphericalCoordinates(qv.Table):
+
+    rho = qv.Float64Column(nullable=True)
+    lon = qv.Float64Column(nullable=True)
+    lat = qv.Float64Column(nullable=True)
+    vrho = qv.Float64Column(nullable=True)
+    vlon = qv.Float64Column(nullable=True)
+    vlat = qv.Float64Column(nullable=True)
+    time = Timestamp.as_column(nullable=True)
+    covariance = CoordinateCovariances.as_column(nullable=True)
+    origin = Origin.as_column()
+    frame = qv.StringAttribute(default="unspecified")
 
     @property
     def values(self) -> np.ndarray:
         return np.array(
             self.table.select(["rho", "lon", "lat", "vrho", "vlon", "vlat"])
-        ).T
+        )
 
     @property
     def sigma_rho(self):
         """
         1-sigma uncertainty in radial distance.
         """
-        return self.covariances.sigmas[:, 0]
+        return self.covariance.sigmas[:, 0]
 
     @property
     def sigma_lon(self):
         """
         1-sigma uncertainty in longitude.
         """
-        return self.covariances.sigmas[:, 1]
+        return self.covariance.sigmas[:, 1]
 
     @property
     def sigma_lat(self):
         """
         1-sigma uncertainty in latitude.
         """
-        return self.covariances.sigmas[:, 2]
+        return self.covariance.sigmas[:, 2]
 
     @property
     def sigma_vrho(self):
         """
         1-sigma uncertainty in radial velocity.
         """
-        return self.covariances.sigmas[:, 3]
+        return self.covariance.sigmas[:, 3]
 
     @property
     def sigma_vlon(self):
         """
         1-sigma uncertainty in longitudinal velocity.
         """
-        return self.covariances.sigmas[:, 4]
+        return self.covariance.sigmas[:, 4]
 
     @property
     def sigma_vlat(self):
         """
         1-sigma uncertainty in latitudinal velocity.
         """
-        return self.covariances.sigmas[:, 5]
+        return self.covariance.sigmas[:, 5]
 
     def to_unit_sphere(self, only_missing: bool = False) -> "SphericalCoordinates":
         """
         Convert to unit sphere. By default, all coordinates will have their rho values
         set to 1.0 and their vrho values set to 0.0. If only_missing is True, then only
         coordinates that have NaN values for rho will be set to 1.0 and coordinates that
         have NaN values for vrho will be set to 0.0.
@@ -144,61 +123,63 @@
         return SphericalCoordinates.from_kwargs(
             rho=coords[:, 0],
             lon=coords[:, 1],
             lat=coords[:, 2],
             vrho=coords[:, 3],
             vlon=coords[:, 4],
             vlat=coords[:, 5],
-            times=self.times,
-            covariances=self.covariances,
+            time=self.time,
+            covariance=self.covariance,
             origin=self.origin,
             frame=self.frame,
         )
 
-    def to_cartesian(self) -> CartesianCoordinates:
+    def to_cartesian(self) -> cartesian.CartesianCoordinates:
         from .transform import _spherical_to_cartesian, spherical_to_cartesian
 
         coords_cartesian = spherical_to_cartesian(self.values)
         coords_cartesian = np.array(coords_cartesian)
 
-        covariances_spherical = self.covariances.to_matrix()
-        if not np.all(np.isnan(covariances_spherical)):
+        if not self.covariance.is_all_nan():
+            covariances_spherical = self.covariance.to_matrix()
             covariances_cartesian = transform_covariances_jacobian(
                 self.values, covariances_spherical, _spherical_to_cartesian
             )
         else:
             covariances_cartesian = np.empty(
                 (len(coords_cartesian), 6, 6), dtype=np.float64
             )
             covariances_cartesian.fill(np.nan)
 
         covariances_cartesian = CoordinateCovariances.from_matrix(covariances_cartesian)
-        coords = CartesianCoordinates.from_kwargs(
+        coords = cartesian.CartesianCoordinates.from_kwargs(
             x=coords_cartesian[:, 0],
             y=coords_cartesian[:, 1],
             z=coords_cartesian[:, 2],
             vx=coords_cartesian[:, 3],
             vy=coords_cartesian[:, 4],
             vz=coords_cartesian[:, 5],
-            times=self.times,
-            covariances=covariances_cartesian,
+            time=self.time,
+            covariance=covariances_cartesian,
             origin=self.origin,
             frame=self.frame,
         )
         return coords
 
     @classmethod
-    def from_cartesian(cls, cartesian: CartesianCoordinates) -> "SphericalCoordinates":
+    def from_cartesian(
+        cls, cartesian: cartesian.CartesianCoordinates
+    ) -> "SphericalCoordinates":
         from .transform import _cartesian_to_spherical, cartesian_to_spherical
 
         coords_spherical = cartesian_to_spherical(cartesian.values)
         coords_spherical = np.array(coords_spherical)
 
-        cartesian_covariances = cartesian.covariances.to_matrix()
-        if not np.all(np.isnan(cartesian_covariances)):
+        if not cartesian.covariance.is_all_nan():
+            cartesian_covariances = cartesian.covariance.to_matrix()
             covariances_spherical = transform_covariances_jacobian(
                 cartesian.values, cartesian_covariances, _cartesian_to_spherical
             )
         else:
             covariances_spherical = np.empty(
                 (len(coords_spherical), 6, 6), dtype=np.float64
             )
@@ -208,94 +189,38 @@
         coords = cls.from_kwargs(
             rho=coords_spherical[:, 0],
             lon=coords_spherical[:, 1],
             lat=coords_spherical[:, 2],
             vrho=coords_spherical[:, 3],
             vlon=coords_spherical[:, 4],
             vlat=coords_spherical[:, 5],
-            times=cartesian.times,
-            covariances=covariances_spherical,
+            time=cartesian.time,
+            covariance=covariances_spherical,
             origin=cartesian.origin,
             frame=cartesian.frame,
         )
 
         return coords
 
-    def to_cometary(self) -> "CometaryCoordinates":
-        from .cometary import CometaryCoordinates
-
-        return CometaryCoordinates.from_cartesian(self.to_cartesian())
+    def to_cometary(self) -> cometary.CometaryCoordinates:
+        return cometary.CometaryCoordinates.from_cartesian(self.to_cartesian())
 
     @classmethod
     def from_cometary(
-        cls, cometary_coordinates: "CometaryCoordinates"
-    ) -> "SphericalCoordinates":
+        cls, cometary_coordinates: cometary.CometaryCoordinates
+    ) -> SphericalCoordinates:
         return cls.from_cartesian(cometary_coordinates.to_cartesian())
 
-    def to_keplerian(self) -> "KeplerianCoordinates":
-        from .keplerian import KeplerianCoordinates
-
-        return KeplerianCoordinates.from_cartesian(self.to_cartesian())
+    def to_keplerian(self) -> keplerian.KeplerianCoordinates:
+        return keplerian.KeplerianCoordinates.from_cartesian(self.to_cartesian())
 
     @classmethod
     def from_keplerian(
-        cls, keplerian_coordinates: "KeplerianCoordinates"
-    ) -> "SphericalCoordinates":
+        cls, keplerian_coordinates: keplerian.KeplerianCoordinates
+    ) -> SphericalCoordinates:
         return cls.from_cartesian(keplerian_coordinates.to_cartesian())
 
     @classmethod
     def from_spherical(
-        cls, spherical_coordinates: "SphericalCoordinates"
-    ) -> "SphericalCoordinates":
+        cls, spherical_coordinates: SphericalCoordinates
+    ) -> SphericalCoordinates:
         return spherical_coordinates
-
-    def to_dataframe(
-        self, sigmas: bool = False, covariances: bool = True
-    ) -> pd.DataFrame:
-        """
-        Convert coordinates to a pandas DataFrame.
-
-        Parameters
-        ----------
-        sigmas : bool, optional
-            If True, include 1-sigma uncertainties in the DataFrame.
-        covariances : bool, optional
-            If True, include covariance matrices in the DataFrame. Covariance matrices
-            will be split into 21 columns, with the lower triangular elements stored.
-
-        Returns
-        -------
-        df : `~pandas.Dataframe`
-            DataFrame containing coordinates.
-        """
-        return coords_to_dataframe(
-            self,
-            ["rho", "lon", "lat", "vrho", "vlon", "vlat"],
-            sigmas=sigmas,
-            covariances=covariances,
-        )
-
-    @classmethod
-    def from_dataframe(
-        cls, df: pd.DataFrame, frame: Literal["ecliptic", "equatorial"]
-    ) -> "SphericalCoordinates":
-        """
-        Create coordinates from a pandas DataFrame.
-
-        Parameters
-        ----------
-        df : `~pandas.Dataframe`
-            DataFrame containing coordinates.
-        frame : {"ecliptic", "equatorial"}
-            Frame in which coordinates are defined.
-
-        Returns
-        -------
-        coords : `~adam_core.coordinates.spherical.SphericalCoordinates`
-            Spherical coordinates.
-        """
-        return coords_from_dataframe(
-            cls,
-            df,
-            coord_names=["rho", "lon", "lat", "vrho", "vlon", "vlat"],
-            frame=frame,
-        )
```

### Comparing `adam_core-0.1.0/adam_core/coordinates/tests/test_origin.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_origin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pytest
 
-from ..origin import Origin
+from ..origin import Origin, OriginCodes, OriginGravitationalParameters
 
 
 def test_origin_eq__():
     origin = Origin.from_kwargs(code=["SUN", "EARTH", "SUN"])
 
     # Test equality with string
     np.testing.assert_equal(origin == "SUN", np.array([True, False, True]))
@@ -42,13 +42,43 @@
         np.array([True, True, True]),
     )
     np.testing.assert_equal(
         origin != Origin.from_kwargs(code=["SUN", "EARTH", "SUN"]),
         np.array([False, False, False]),
     )
 
+    # Test equality with OriginCodes
+    np.testing.assert_equal(origin == OriginCodes.SUN, np.array([True, False, True]))
+    np.testing.assert_equal(origin != OriginCodes.SUN, np.array([False, True, False]))
+    np.testing.assert_equal(origin == OriginCodes.EARTH, np.array([False, True, False]))
+    np.testing.assert_equal(origin != OriginCodes.EARTH, np.array([True, False, True]))
 
-def test_origin_eq__raises():
+
+def test_origin__eq__raises():
     # Test that an error is raised when an unsupported type is passed
     origin = Origin.from_kwargs(code=["SUN", "EARTH", "MARS"])
     with pytest.raises(TypeError):
         origin == 1
+
+
+def test_origin_mu():
+    # Test that the mu function returns the correct values
+    origin = Origin.from_kwargs(
+        code=["SUN", "MARS_BARYCENTER", "JUPITER_BARYCENTER", "SUN"]
+    )
+
+    expected = np.array(
+        [
+            OriginGravitationalParameters.SUN,
+            OriginGravitationalParameters.MARS_BARYCENTER,
+            OriginGravitationalParameters.JUPITER_BARYCENTER,
+            OriginGravitationalParameters.SUN,
+        ]
+    )
+    np.testing.assert_equal(origin.mu(), expected)
+
+
+def test_origin_mu_raises():
+    # Test that the mu function raises a ValueError when an unsupported code is passed
+    origin = Origin.from_kwargs(code=["VESTA"])
+    with pytest.raises(ValueError):
+        origin.mu()
```

### Comparing `adam_core-0.1.0/adam_core/coordinates/tests/test_spherical.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_spherical.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.1.0/adam_core/coordinates/tests/test_transforms_spherical.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/tests/test_transforms_spherical.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.1.0/adam_core/coordinates/transform.py` & `adam_core-0.2.0a1/src/adam_core/coordinates/transform.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from __future__ import annotations
+
 import logging
 from typing import Literal, Optional, Union
 
 import jax.numpy as jnp
 import numpy as np
+import pyarrow.compute as pc
 from jax import config, jit, lax, vmap
 
 from ..constants import Constants as c
-from ..dynamics.barker import solve_barker
-from ..dynamics.kepler import calc_mean_anomaly, solve_kepler
+from . import types
 from .cartesian import CartesianCoordinates
 from .cometary import CometaryCoordinates
 from .keplerian import KeplerianCoordinates
 from .origin import OriginCodes
 from .spherical import SphericalCoordinates
 
 config.update("jax_enable_x64", True)
@@ -20,43 +22,23 @@
 TRANSFORM_EQ2EC = np.zeros((6, 6))
 TRANSFORM_EQ2EC[0:3, 0:3] = c.TRANSFORM_EQ2EC
 TRANSFORM_EQ2EC[3:6, 3:6] = c.TRANSFORM_EQ2EC
 TRANSFORM_EC2EQ = TRANSFORM_EQ2EC.T
 
 logger = logging.getLogger(__name__)
 
-__all__ = [
-    "transform_coordinates",
-    "_cartesian_to_keplerian",
-    "_cartesian_to_keplerian6",
-    "cartesian_to_keplerian",
-    "_keplerian_to_cartesian_a",
-    "_keplerian_to_cartesian_p",
-    "_keplerian_to_cartesian_q",
-    "_cartesian_to_cometary",
-    "cartesian_to_cometary",
-    "_cometary_to_cartesian",
-    "cometary_to_cartesian",
-]
 
-CoordinateType = Union[
-    CartesianCoordinates,
-    KeplerianCoordinates,
-    CometaryCoordinates,
-    SphericalCoordinates,
-]
 CoordinatesClasses = (
     CartesianCoordinates,
     KeplerianCoordinates,
     CometaryCoordinates,
     SphericalCoordinates,
 )
 
 
-MU = c.MU
 Z_AXIS = jnp.array([0.0, 0.0, 1.0])
 FLOAT_TOLERANCE = 1e-15
 
 
 @jit
 def _cartesian_to_spherical(
     coords_cartesian: Union[np.ndarray, jnp.ndarray]
@@ -136,17 +118,19 @@
     coords_spherical = coords_spherical.at[4].set(jnp.degrees(vlon))
     coords_spherical = coords_spherical.at[5].set(jnp.degrees(vlat))
 
     return coords_spherical
 
 
 # Vectorization Map: _cartesian_to_spherical
-_cartesian_to_spherical_vmap = vmap(
-    _cartesian_to_spherical,
-    in_axes=(0,),
+_cartesian_to_spherical_vmap = jit(
+    vmap(
+        _cartesian_to_spherical,
+        in_axes=(0,),
+    )
 )
 
 
 def cartesian_to_spherical(
     coords_cartesian: Union[np.ndarray, jnp.ndarray]
 ) -> jnp.ndarray:
     """
@@ -249,17 +233,19 @@
     coords_cartesian = coords_cartesian.at[4].set(vy)
     coords_cartesian = coords_cartesian.at[5].set(vz)
 
     return coords_cartesian
 
 
 # Vectorization Map: _spherical_to_cartesian
-_spherical_to_cartesian_vmap = vmap(
-    _spherical_to_cartesian,
-    in_axes=(0,),
+_spherical_to_cartesian_vmap = jit(
+    vmap(
+        _spherical_to_cartesian,
+        in_axes=(0,),
+    )
 )
 
 
 def spherical_to_cartesian(
     coords_spherical: Union[np.ndarray, jnp.ndarray]
 ) -> jnp.ndarray:
     """
@@ -294,15 +280,15 @@
     return coords_cartesian
 
 
 @jit
 def _cartesian_to_keplerian(
     coords_cartesian: Union[np.ndarray, jnp.ndarray],
     t0: float,
-    mu: float = MU,
+    mu: float,
 ) -> jnp.ndarray:
     """
     Convert a single Cartesian coordinate to a Keplerian coordinate.
 
     If the orbit is found to be circular (e = 0 +- 1e-15) then
     the argument of periapsis is set to 0. The anomalies are then accordingly
     defined with this assumption.
@@ -319,15 +305,15 @@
         y : y-position in units of au.
         z : z-position in units of au.
         vx : x-velocity in units of au per day.
         vy : y-velocity in units of au per day.
         vz : z-velocity in units of au per day.
     t0 : float (1)
         Epoch at which cometary elements are defined in MJD TDB.
-    mu : float, optional
+    mu : float (1)
         Gravitational parameter (GM) of the attracting body in units of
         au**3 / d**2.
 
     Returns
     -------
     coords_keplerian : `~jax.numpy.ndarray` (13)
         13D Keplerian coordinate.
@@ -346,14 +332,20 @@
         tp : time of periapsis passage in days.
 
     References
     ----------
     [1] Bate, R. R; Mueller, D. D; White, J. E. (1971). Fundamentals of Astrodynamics. 1st ed.,
         Dover Publications, Inc. ISBN-13: 978-0486600611
     """
+    from ..dynamics.kepler import (
+        calc_mean_anomaly,
+        calc_mean_motion,
+        calc_periapsis_distance,
+    )
+
     coords_keplerian = jnp.zeros(13, dtype=jnp.float64)
     r = coords_cartesian[0:3]
     v = coords_cartesian[3:6]
 
     r_mag = jnp.linalg.norm(r)
     v_mag = jnp.linalg.norm(v)
 
@@ -418,29 +410,29 @@
         mu / (-2 * sme),
     )
 
     # Calculate the periapsis distance
     q = jnp.where(
         (e > (1.0 - FLOAT_TOLERANCE)) & (e < (1.0 + FLOAT_TOLERANCE)),
         p / 2,
-        a * (1 - e),
+        calc_periapsis_distance(a, e),
     )
 
     # Calculate the apoapsis distance (infinite for
     # parabolic and hyperbolic orbits)
     Q = jnp.where(e < 1.0, a * (1 + e), jnp.inf)
 
     # Calculate the mean anomaly
     M = calc_mean_anomaly(nu, e)
 
     # Calculate the mean motion
     n = lax.cond(
         (e > (1.0 - FLOAT_TOLERANCE)) & (e < (1.0 + FLOAT_TOLERANCE)),
         lambda a, q: jnp.sqrt(mu / (2 * q**3)),
-        lambda a, q: jnp.sqrt(mu / jnp.abs(a) ** 3),
+        lambda a, q: calc_mean_motion(a, mu),
         a,
         q,
     )
 
     # Calculate the orbital period which for parabolic and hyperbolic
     # orbits is infinite while for all closed orbits
     # is well defined.
@@ -473,25 +465,27 @@
     coords_keplerian = coords_keplerian.at[11].set(P)
     coords_keplerian = coords_keplerian.at[12].set(tp)
 
     return coords_keplerian
 
 
 # Vectorization Map: _cartesian_to_keplerian
-_cartesian_to_keplerian_vmap = vmap(
-    _cartesian_to_keplerian,
-    in_axes=(0, 0, None),
+_cartesian_to_keplerian_vmap = jit(
+    vmap(
+        _cartesian_to_keplerian,
+        in_axes=(0, 0, 0),
+    )
 )
 
 
 @jit
 def _cartesian_to_keplerian6(
     coords_cartesian: Union[np.ndarray, jnp.ndarray],
     t0: float,
-    mu: float = MU,
+    mu: float,
 ) -> jnp.ndarray:
     """
     Limit conversion of Cartesian coordinates to Keplerian 6 fundamental coordinates.
 
     Parameters
     ----------
     coords_cartesian : {`~numpy.ndarray`, `~jax.numpy.ndarray`} (6)
@@ -500,15 +494,15 @@
         y : y-position in units of au.
         z : z-position in units of au.
         vx : x-velocity in units of au per day.
         vy : y-velocity in units of au per day.
         vz : z-velocity in units of au per day.
     t0 : float (1)
         Epoch at which cometary elements are defined in MJD TDB.
-    mu : float, optional
+    mu : float (1)
         Gravitational parameter (GM) of the attracting body in units of
         au**3 / d**2.
 
     Returns
     -------
     coords_keplerian : `~jax.numpy.ndarray` (6)
         6D Keplerian coordinate.
@@ -522,15 +516,15 @@
     coords_keplerian = _cartesian_to_keplerian(coords_cartesian, t0, mu)
     return coords_keplerian[jnp.array([0, 4, 5, 6, 7, 8])]
 
 
 def cartesian_to_keplerian(
     coords_cartesian: Union[np.ndarray, jnp.ndarray],
     t0: Union[np.ndarray, jnp.ndarray],
-    mu: float = MU,
+    mu: Union[np.ndarray, jnp.ndarray],
 ) -> jnp.ndarray:
     """
     Convert Cartesian coordinates to Keplerian coordinates.
 
     Parameters
     ----------
     coords_cartesian : {`~numpy.ndarray`, `~jax.numpy.ndarray`} (N, 6)
@@ -539,15 +533,15 @@
         y : y-position in units of au.
         z : z-position in units of au.
         vx : x-velocity in units of au per day.
         vy : y-velocity in units of au per day.
         vz : z-velocity in units of au per day.
     t0 : {`~numpy.ndarray`, `~jax.numpy.ndarray`} (N)
         Epoch at which cometary elements are defined in MJD TDB.
-    mu : float, optional
+    mu : {`~numpy.ndarray`, `~jax.numpy.ndarray`} (N, 6)
         Gravitational parameter (GM) of the attracting body in units of
         au**3 / d**2.
 
     Returns
     -------
     coords_keplerian : `~jax.numpy.ndarray` (N, 13)
         13D Keplerian coordinates.
@@ -568,15 +562,15 @@
     coords_keplerian = _cartesian_to_keplerian_vmap(coords_cartesian, t0, mu)
     return coords_keplerian
 
 
 @jit
 def _keplerian_to_cartesian_p(
     coords_keplerian: Union[np.ndarray, jnp.ndarray],
-    mu: float = MU,
+    mu: float,
     max_iter: int = 1000,
     tol: float = 1e-15,
 ) -> jnp.ndarray:
     """
     Convert a single Keplerian coordinate to a Cartesian coordinate.
 
     Parabolic orbits (e = 1.0 +- 1e-15) with elements (a, e, i, raan, ap, M) cannot be converted
@@ -590,15 +584,15 @@
         6D Keplerian coordinate.
         p : semi-latus rectum in au.
         e : eccentricity.
         i : inclination in degrees.
         raan : Right ascension (longitude) of the ascending node in degrees.
         ap : argument of periapsis in degrees.
         M : mean anomaly in degrees.
-    mu : float, optional
+    mu : float
         Gravitational parameter (GM) of the attracting body in units of
         au**3 / d**2.
     max_iter : int, optional
         Maximum number of iterations over which to converge. If number of iterations is
         exceeded, will use the value of the relevant anomaly at the last iteration.
     tol : float, optional
         Numerical tolerance to which to compute anomalies using the Newtown-Raphson
@@ -611,14 +605,17 @@
         x : x-position in units of au.
         y : y-position in units of au.
         z : z-position in units of au.
         vx : x-velocity in units of au per day.
         vy : y-velocity in units of au per day.
         vz : z-velocity in units of au per day.
     """
+    from ..dynamics.barker import solve_barker
+    from ..dynamics.kepler import solve_kepler
+
     coords_cartesian = jnp.zeros(6, dtype=jnp.float64)
 
     p = coords_keplerian[0]
     e = coords_keplerian[1]
     i = jnp.radians(coords_keplerian[2])
     raan = jnp.radians(coords_keplerian[3])
     ap = jnp.radians(coords_keplerian[4])
@@ -690,24 +687,26 @@
     coords_cartesian = coords_cartesian.at[4].set(v[1])
     coords_cartesian = coords_cartesian.at[5].set(v[2])
 
     return coords_cartesian
 
 
 # Vectorization Map: _keplerian_to_cartesian_p
-_keplerian_to_cartesian_p_vmap = vmap(
-    _keplerian_to_cartesian_p,
-    in_axes=(0, None, None, None),
+_keplerian_to_cartesian_p_vmap = jit(
+    vmap(
+        _keplerian_to_cartesian_p,
+        in_axes=(0, 0, None, None),
+    )
 )
 
 
 @jit
 def _keplerian_to_cartesian_a(
     coords_keplerian: Union[np.ndarray, jnp.ndarray],
-    mu: float = MU,
+    mu: float,
     max_iter: int = 1000,
     tol: float = 1e-15,
 ) -> jnp.ndarray:
     """
     Convert a single Keplerian coordinate to a Cartesian coordinate.
 
     Parabolic orbits (e = 1.0 +- 1e-15) with elements (a, e, i, raan, ap, M) cannot be converted
@@ -721,15 +720,15 @@
         6D Keplerian coordinate.
         a : semi-major axis in au.
         e : eccentricity.
         i : inclination in degrees.
         raan : Right ascension (longitude) of the ascending node in degrees.
         ap : argument of periapsis in degrees.
         M : mean anomaly in degrees.
-    mu : float, optional
+    mu : float (1)
         Gravitational parameter (GM) of the attracting body in units of
         au**3 / d**2.
     max_iter : int, optional
         Maximum number of iterations over which to converge. If number of iterations is
         exceeded, will use the value of the relevant anomaly at the last iteration.
     tol : float, optional
         Numerical tolerance to which to compute anomalies using the Newtown-Raphson
@@ -771,24 +770,26 @@
         max_iter=max_iter,
         tol=tol,
     )
     return coords_cartesian
 
 
 # Vectorization Map: _keplerian_to_cartesian_a
-_keplerian_to_cartesian_a_vmap = vmap(
-    _keplerian_to_cartesian_a,
-    in_axes=(0, None, None, None),
+_keplerian_to_cartesian_a_vmap = jit(
+    vmap(
+        _keplerian_to_cartesian_a,
+        in_axes=(0, 0, None, None),
+    )
 )
 
 
 @jit
 def _keplerian_to_cartesian_q(
     coords_keplerian: Union[np.ndarray, jnp.ndarray],
-    mu: float = MU,
+    mu: float,
     max_iter: int = 1000,
     tol: float = 1e-15,
 ) -> jnp.ndarray:
     """
     Convert a single Keplerian coordinate to a Cartesian coordinate.
 
     Parabolic orbits (e = 1.0 +- 1e-15) with elements (a, e, i, raan, ap, M) cannot be converted
@@ -802,15 +803,15 @@
         6D Keplerian coordinate.
         q : periapsis distance in au.
         e : eccentricity.
         i : inclination in degrees.
         raan : Right ascension (longitude) of the ascending node in degrees.
         ap : argument of periapsis in degrees.
         M : mean anomaly in degrees.
-    mu : float, optional
+    mu : float (1)
         Gravitational parameter (GM) of the attracting body in units of
         au**3 / d**2.
     max_iter : int, optional
         Maximum number of iterations over which to converge. If number of iterations is
         exceeded, will use the value of the relevant anomaly at the last iteration.
     tol : float, optional
         Numerical tolerance to which to compute anomalies using the Newtown-Raphson
@@ -852,23 +853,25 @@
         max_iter=max_iter,
         tol=tol,
     )
     return coords_cartesian
 
 
 # Vectorization Map: _keplerian_to_cartesian_q
-_keplerian_to_cartesian_q_vmap = vmap(
-    _keplerian_to_cartesian_q,
-    in_axes=(0, None, None, None),
+_keplerian_to_cartesian_q_vmap = jit(
+    vmap(
+        _keplerian_to_cartesian_q,
+        in_axes=(0, 0, None, None),
+    )
 )
 
 
 def keplerian_to_cartesian(
     coords_keplerian: Union[np.ndarray, jnp.ndarray],
-    mu: float = MU,
+    mu: Union[np.ndarray, jnp.ndarray],
     max_iter: int = 100,
     tol: float = 1e-15,
 ) -> jnp.ndarray:
     """
     Convert Keplerian coordinates to Cartesian coordinates.
 
     Parabolic orbits (e = 1.0 +- 1e-15) with elements (a, e, i, raan, ap, M) cannot be converted
@@ -882,15 +885,15 @@
         6D Keplerian coordinate.
         a : semi-major axis in au.
         e : eccentricity.
         i : inclination in degrees.
         raan : Right ascension (longitude) of the ascending node in degrees.
         ap : argument of periapsis in degrees.
         M : mean anomaly in degrees.
-    mu : float, optional
+    mu : {`~numpy.ndarray`, `~jax.numpy.ndarray`} (N)
         Gravitational parameter (GM) of the attracting body in units of
         au**3 / d**2.
     max_iter : int, optional
         Maximum number of iterations over which to converge. If number of iterations is
         exceeded, will use the value of the relevant anomaly at the last iteration.
     tol : float, optional
         Numerical tolerance to which to compute anomalies using the Newtown-Raphson
@@ -948,15 +951,15 @@
     return coords_cartesian
 
 
 @jit
 def _cartesian_to_cometary(
     coords_cartesian: Union[np.ndarray, jnp.ndarray],
     t0: float,
-    mu: float = MU,
+    mu: float,
 ) -> jnp.ndarray:
     """
     Convert Cartesian coordinates to Cometary coordinates.
 
     Parameters
     ----------
     coords_cartesian : {`~numpy.ndarray`, `~jax.numpy.ndarray`} (6)
@@ -965,15 +968,15 @@
         y : y-position in units of au.
         z : z-position in units of au.
         vx : x-velocity in units of au per day.
         vy : y-velocity in units of au per day.
         vz : z-velocity in units of au per day.
     t0 : float (1)
         Epoch at which cometary elements are defined in MJD TDB.
-    mu : float, optional
+    mu : float (1)
         Gravitational parameter (GM) of the attracting body in units of
         au**3 / d**2.
 
     Returns
     -------
     coords_cometary : `~jax.numpy.ndarray` (6)
         6D Cometary coordinate.
@@ -985,24 +988,26 @@
         tp : time of periapse passage in days.
     """
     coords_cometary = _cartesian_to_keplerian(coords_cartesian, t0, mu=mu)
     return coords_cometary[jnp.array([2, 4, 5, 6, 7, 12])]
 
 
 # Vectorization Map: _cartesian_to_cometary
-_cartesian_to_cometary_vmap = vmap(
-    _cartesian_to_cometary,
-    in_axes=(0, 0, None),
+_cartesian_to_cometary_vmap = jit(
+    vmap(
+        _cartesian_to_cometary,
+        in_axes=(0, 0, 0),
+    )
 )
 
 
 def cartesian_to_cometary(
     coords_cartesian: Union[np.ndarray, jnp.ndarray],
     t0: Union[np.ndarray, jnp.ndarray],
-    mu: float = MU,
+    mu: Union[np.ndarray, jnp.ndarray],
 ) -> jnp.ndarray:
     """
     Convert Cartesian coordinates to Keplerian coordinates.
 
     Parameters
     ----------
     coords_cartesian : {`~numpy.ndarray`, `~jax.numpy.ndarray`} (N, 6)
@@ -1011,15 +1016,15 @@
         y : y-position in units of au.
         z : z-position in units of au.
         vx : x-velocity in units of au per day.
         vy : y-velocity in units of au per day.
         vz : z-velocity in units of au per day.
     t0 : {`~numpy.ndarray`, `~jax.numpy.ndarray`} (N)
         Epoch at which cometary elements are defined in MJD TDB.
-    mu : float, optional
+    mu : {`~numpy.ndarray`, `~jax.numpy.ndarray`} (N)
         Gravitational parameter (GM) of the attracting body in units of
         au**3 / d**2.
 
     Returns
     -------
     coords_cometary : `~jax.numpy.ndarray` (N, 6)
         6D Cometary coordinates.
@@ -1034,15 +1039,15 @@
     return coords_cometary
 
 
 @jit
 def _cometary_to_cartesian(
     coords_cometary: Union[np.ndarray, jnp.ndarray],
     t0: float,
-    mu: float = MU,
+    mu: float,
     max_iter: int = 100,
     tol: float = 1e-15,
 ) -> jnp.ndarray:
     """
     Convert a single Cometary coordinate to a Cartesian coordinate.
 
     Parameters
@@ -1053,15 +1058,15 @@
         e : eccentricity.
         i : inclination in degrees.
         raan : Right ascension (longitude) of the ascending node in degrees.
         ap : argument of periapsis in degrees.
         tp : time of periapse passage in days.
     t0 : float (1)
         Epoch at which cometary elements are defined in MJD TDB.
-    mu : float, optional
+    mu : float
         Gravitational parameter (GM) of the attracting body in units of
         au**3 / d**2.
     max_iter : int, optional
         Maximum number of iterations over which to converge. If number of iterations is
         exceeded, will use the value of the relevant anomaly at the last iteration.
     tol : float, optional
         Numerical tolerance to which to compute anomalies using the Newtown-Raphson
@@ -1128,24 +1133,26 @@
         coords_keplerian, mu=mu, max_iter=max_iter, tol=tol
     )
 
     return coords_cartesian
 
 
 # Vectorization Map: _cometary_to_cartesian
-_cometary_to_cartesian_vmap = vmap(
-    _cometary_to_cartesian,
-    in_axes=(0, 0, None, None, None),
+_cometary_to_cartesian_vmap = jit(
+    vmap(
+        _cometary_to_cartesian,
+        in_axes=(0, 0, 0, None, None),
+    )
 )
 
 
 def cometary_to_cartesian(
     coords_cometary: Union[np.ndarray, jnp.ndarray],
     t0: Union[np.ndarray, jnp.ndarray],
-    mu: float = MU,
+    mu: Union[np.ndarray, jnp.ndarray],
     max_iter: int = 100,
     tol: float = 1e-15,
 ) -> jnp.ndarray:
     """
     Convert Cometary coordinates to Cartesian coordinates.
 
     Parameters
@@ -1156,15 +1163,15 @@
         e : eccentricity.
         i : inclination in degrees.
         raan : Right ascension (longitude) of the ascending node in degrees.
         ap : argument of periapsis in degrees.
         tp : time of periapse passage in days.
     t0 : {`~numpy.ndarray`, `~jax.numpy.ndarray`} (N)
         Epoch at which cometary elements are defined in MJD TDB.
-    mu : float, optional
+    mu : {`~numpy.ndarray`, `~jax.numpy.ndarray`} (N)
         Gravitational parameter (GM) of the attracting body in units of
         au**3 / d**2.
     max_iter : int, optional
         Maximum number of iterations over which to converge. If number of iterations is
         exceeded, will use the value of the relevant anomaly at the last iteration.
     tol : float, optional
         Numerical tolerance to which to compute anomalies using the Newtown-Raphson
@@ -1193,31 +1200,64 @@
     """
     Translate coordinates to a different origin.
 
     Parameters
     ----------
     coords : `~adam_core.coordinates.cartesian.CartesianCoordinates`
         Cartesian coordinates and optionally their covariances.
-    origin : {'SUN', 'SOLAR_SYSTEM_BARYCENTER'}
-        Name of the desired origin.
+    origin : `~adam_core.coordinates.origin.OriginCodes`
+        Desired origin. Input origins may be either `~adam_core.coordinates.origin.OriginCodes`
+        or a str of an observatory code, but the output origin (this kwarg) should always be an
+        `~adam_core.coordinates.origin.OriginCodes`. If you are looking to generate ephemerides
+        for an observatory, please use a `~adam_core.propagator.propagator.Propagator` instead.
 
     Returns
     -------
     CartesianCoordinates : `~adam_core.coordinates.cartesian.CartesianCoordinates`
         Translated Cartesian coordinates and their covariances.
+
+    Raises
+    ------
+    ValueError
+        If origin is not a `~adam_core.coordinates.origin.OriginCodes` object or
+        a str of an observatory code.
     """
-    unique_origins = np.unique(coords.origin)
-    vectors = np.zeros(coords.values.shape, dtype=np.float64)
+    from ..observers.state import OBSERVATORY_CODES, get_observer_state
+    from ..utils.spice import get_perturber_state
+
+    unique_origins = coords.origin.code.unique()
+    vectors = np.empty(coords.values.shape, dtype=np.float64)
+    times = coords.time
 
     for origin_in in unique_origins:
-        raise NotImplementedError("get_perturber_state not implemented yet")
-        # mask = np.where(coords.origin == origin_in)[0]
-        # vectors[mask] = get_perturber_state(
-        #    origin_in, coords.times[mask], frame=coords.frame, origin=origin
-        # )
+
+        mask = pc.equal(coords.origin.code, origin_in).to_numpy(zero_copy_only=False)
+
+        origin_in_str = origin_in.as_py()
+        # Could use try / except block here but this is more explicit
+        if origin_in_str in OriginCodes.__members__:
+
+            vectors[mask] = get_perturber_state(
+                OriginCodes[origin_in_str],
+                times.apply_mask(mask),
+                frame=coords.frame,
+                origin=origin,
+            ).values
+
+        elif origin_in_str in OBSERVATORY_CODES:
+
+            vectors[mask] = get_observer_state(
+                origin_in_str,
+                times.apply_mask(mask),
+                frame=coords.frame,
+                origin=origin,
+            ).values
+
+        else:
+            raise ValueError("Unsupported origin: {}".format(origin_in_str))
 
     return coords.translate(vectors, origin.name)
 
 
 def cartesian_to_frame(
     coords: CartesianCoordinates, frame: Literal["ecliptic", "equatorial"]
 ) -> "CartesianCoordinates":
@@ -1233,44 +1273,52 @@
 
     Returns
     -------
     CartesianCoordinates : `~adam_core.coordinates.cartesian.CartesianCoordinates`
         Rotated Cartesian coordinates and their covariances.
     """
     if frame == "ecliptic" and coords.frame != "ecliptic":
-        return coords.rotate(TRANSFORM_EC2EQ, "ecliptic")
+        return coords.rotate(TRANSFORM_EQ2EC, "ecliptic")
     elif frame == "equatorial" and coords.frame != "equatorial":
-        return coords.rotate(TRANSFORM_EQ2EC, "equatorial")
+        return coords.rotate(TRANSFORM_EC2EQ, "equatorial")
     elif frame == coords.frame:
         return coords
     else:
         err = "frame should be one of {'ecliptic', 'equatorial'}"
         raise ValueError(err)
 
 
 def transform_coordinates(
-    coords: CoordinateType,
-    representation_out: CoordinateType,
+    coords: types.CoordinateType,
+    representation_out: Optional[type[types.CoordinateType]] = None,
     frame_out: Optional[Literal["ecliptic", "equatorial"]] = None,
     origin_out: Optional[OriginCodes] = None,
-) -> CoordinateType:
+) -> types.CoordinateType:
     """
     Transform coordinates between frames ('ecliptic', 'equatorial'), origins,
     and/or representations ('cartesian', 'spherical', 'keplerian', 'cometary').
 
+    Input coordinates may be defined from multiple origins but if origin_out is
+    specified, all coordinates will be transformed to that origin.
+
     Parameters
     ----------
-    coords : `~adam_core.coordinates.Coordinates`
+    coords:
         Coordinates to transform between representations and frames.
-    representation_out : `~adam_core.coordinates.Coordinates`
-        Desired coordinate type or representation of the output coordinates.
+    representation_out:
+        Desired coordinate type or representation of the output coordinates. If None,
+        the output coordinates will be the same type as the input coordinates.
     frame_out : {'ecliptic', 'equatorial'}
         Desired reference frame of the output coordinates.
-    origin_out : {'SUN', 'SOLAR_SYSTEM_BARYCENTER'}
-        Desired origin of the output coordinates.
+    origin_out : `~adam_core.coordinates.origin.OriginCodes`
+        Desired origin. Input origins may be either `~adam_core.coordinates.origin.OriginCodes`
+        or a str of an observatory code, but the output origin (this kwarg) should always be an
+        `~adam_core.coordinates.origin.OriginCodes`. If you are looking to generate ephemerides
+        for an observatory, please use a `~adam_core.propagator.propagator.Propagator` instead.
+
     Returns
     -------
     coords_out : `~adam_core.coordinates.Coordinates`
         Coordinates in desired output representation and frame.
 
     Raises
     ------
@@ -1288,37 +1336,58 @@
 
     if frame_out not in {None, "equatorial", "ecliptic"}:
         raise ValueError("Unsupported frame_out: {}".format(frame_out))
 
     if origin_out is not None and not isinstance(origin_out, OriginCodes):
         raise TypeError("Unsupported origin_out type: {}".format(type(origin_out)))
 
-    if representation_out not in CoordinatesClasses:
+    if representation_out is None:
+        representation_out_ = coords.__class__
+    else:
+        representation_out_ = representation_out
+
+    if representation_out_ not in CoordinatesClasses:
         raise ValueError(
-            "Unsupported representation_out: {}".format(representation_out)
+            "Unsupported representation_out: {}".format(representation_out_)
         )
 
     coord_frame = coords.frame
-    # Extract the origins from the input coordinates
+    # Extract the origins from the input coordinates. These typically correspond
+    # to the name of OriginCode enums but stored as an array of strings.
     coord_origin = coords.origin.code.to_numpy(zero_copy_only=False)
 
     if frame_out is None:
         frame_out = coord_frame
 
+    # If origin out is not None, then origin_out will be an OriginCode
+    # passed directly to this function. Otherwise, it will be an array of strings
+    # extracted from the input coordinates.
     if origin_out is None:
         origin_out = coord_origin
 
-    if type(coords) == representation_out:
+    # `~adam_core.coordinates.origin.Origin` support equality checks with
+    # `~adam_core.coordinates.origin.OriginCodes` so we can compare them directly.
+    # If its not an OriginCodes enum then origin_out will be an array of strings which
+    # also can be checked for equality.
+    if type(coords) == representation_out_:
         if coord_frame == frame_out and np.all(coord_origin == origin_out):
             return coords
 
-    cartesian = coords.to_cartesian()
+    if not isinstance(coords, CartesianCoordinates):
+        cartesian = coords.to_cartesian()
+    else:
+        cartesian = coords
 
-    # Translate coordinates to new origin (if different from current)
-    if np.all(cartesian.origin != origin_out):
+    # Translate coordinates to new origin (if any are different from current)
+    if np.any(cartesian.origin != origin_out):
         cartesian = cartesian_to_origin(cartesian, origin_out)
 
     # Rotate coordinates to new frame (if different from current)
     if cartesian.frame != frame_out:
         cartesian = cartesian_to_frame(cartesian, frame_out)
 
-    return representation_out.from_cartesian(cartesian)
+    # You might think this should be 'isinstance', but no! We're
+    # checking whether the input is a particular class variable, not
+    # an instance of a class.
+    if representation_out_ is CartesianCoordinates:
+        return cartesian
+    return representation_out_.from_cartesian(cartesian)
```

### Comparing `adam_core-0.1.0/adam_core/dynamics/barker.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/barker.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.1.0/adam_core/dynamics/tests/test_tisserand.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/tests/test_tisserand.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.1.0/adam_core/dynamics/tisserand.py` & `adam_core-0.2.0a1/src/adam_core/dynamics/tisserand.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 This code generates the dictionary of semi-major axes for the
 third body needed for the Tisserand parameter
 
-from astropy.time import Time
 from adam_core.orbits.query import _get_horizons_elements
 
 ids = ["199", "299", "399", "499", "599", "699", "799", "899"]
 elements = _get_horizons_elements(ids, times, id_type="majorbody")
 
 MAJOR_BODIES = {}
 for i, r in elements[["targetname", "a"]].iterrows():
    body_name = r["targetname"].split(" ")[0].lower()
    MAJOR_BODIES[body_name] = r["a"]
 
 """
+
 import numpy as np
 
 MAJOR_BODIES = {
     "mercury": 0.3870970330236769,
     "venus": 0.723341974974844,
     "earth": 0.9997889954736553,
     "mars": 1.523803685638066,
```

### Comparing `adam_core-0.1.0/adam_core/orbits/orbits.py` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/orbits.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,91 @@
-import logging
-from typing import Literal
+from importlib.resources import files
+from typing import Optional
 
-import pandas as pd
-from quivr import StringColumn, Table
+import numpy as np
 
-from ..coordinates.cartesian import CartesianCoordinates
-
-logger = logging.getLogger(__name__)
-
-
-class Orbits(Table):
-
-    orbit_ids = StringColumn(nullable=True)
-    object_ids = StringColumn(nullable=True)
-    coordinates = CartesianCoordinates.as_column(nullable=False)
-
-    def to_dataframe(self, sigmas: bool = False, covariances: bool = True):
-        """
-        Represent the orbits as a pandas DataFrame.
-
-        Parameters
-        ----------
-        sigmas : bool, optional
-            If True, include 1-sigma uncertainties in the DataFrame.
-        covariances : bool, optional
-            If True, include covariance matrices in the DataFrame. Covariance matrices
-            will be split into 21 columns, with the lower triangular elements stored.
-
-        Returns
-        -------
-        df : `~pandas.Dataframe`
-            DataFrame containing orbits and their Cartesian elements.
-        """
-        df = pd.DataFrame(
-            {
-                "orbit_ids": self.orbit_ids.to_pandas(),
-                "object_ids": self.object_ids.to_pandas(),
-            }
-        )
-        df = df.join(
-            self.coordinates.to_dataframe(sigmas=sigmas, covariances=covariances)
+from ...coordinates.covariances import CoordinateCovariances
+from ...coordinates.keplerian import KeplerianCoordinates
+from ...coordinates.origin import Origin
+from ...orbits.orbits import Orbits
+from ...time import Timestamp
+
+
+def make_real_orbits(num_orbits: Optional[int] = None) -> Orbits:
+    """
+    Returns an `~adam_core.orbits.orbits.Orbits` object with real orbits drawn
+    from our list of sample objects.
+
+    Parameters
+    ----------
+    num_orbits : optional, int
+        The number of orbits to return, which must be less than or equal to
+        the number of sample objects (27).
+
+    Returns
+    -------
+    orbits : `~adam_core.orbits.orbits.Orbits`
+        Orbits object containing the sample orbits.
+    """
+    orbits_file = files("adam_core.utils.helpers.data").joinpath("orbits.parquet")
+    orbits = Orbits.from_parquet(orbits_file)
+
+    if num_orbits is None:
+        return orbits
+
+    if num_orbits > len(orbits):
+        raise ValueError(
+            f"num_orbits must be less than or equal to the number of sample orbits ({len(orbits)})."
         )
-        return df
 
-    @classmethod
-    def from_dataframe(
-        cls, df: pd.DataFrame, frame: Literal["ecliptic", "equatorial"]
-    ) -> "Orbits":
-        """
-        Create an Orbits object from a pandas DataFrame.
-
-        Parameters
-        ----------
-        df : `~pandas.DataFrame`
-            DataFrame containing orbits and their Cartesian elements.
-        frame : {"ecliptic", "equatorial"}
-            Frame in which coordinates are defined.
-
-        Returns
-        -------
-        orbits : `~adam_core.orbits.orbits.Orbits`
-            Orbits.
-        """
-        orbit_ids = df["orbit_ids"].values
-        object_ids = df["object_ids"].values
-        coordinates = CartesianCoordinates.from_dataframe(df, frame=frame)
-        return cls.from_kwargs(
-            orbit_ids=orbit_ids, object_ids=object_ids, coordinates=coordinates
-        )
+    return orbits[:num_orbits]
+
+
+def make_simple_orbits(num_orbits: int = 10) -> Orbits:
+    """
+    Returns an `~adam_core.orbits.orbits.Orbits` object with simple orbits.
+
+    Parameters
+    ----------
+    num_orbits : int, optional
+        The number of orbits to return.
+        Default is 10.
+
+    Returns
+    -------
+    orbits : `~adam_core.orbits.orbits.Orbits`
+        Orbits object containing the sample orbits.
+    """
+
+    data = {
+        "a": np.linspace(1, 10, num_orbits),
+        "e": np.linspace(0, 2, num_orbits),
+        "i": np.linspace(0, 180, num_orbits),
+        "raan": np.linspace(0, 360, num_orbits),
+        "ap": np.linspace(0, 360, num_orbits),
+        "M": np.linspace(0, 360, num_orbits),
+    }
+    # Hyperbolic orbits have negative semi-major axes
+    data["a"] = np.where(data["e"] > 1.0, -data["a"], data["a"])
+
+    sigmas = np.zeros((num_orbits, 6))
+    for i, dim in enumerate(["a", "e", "i", "raan", "ap", "M"]):
+        sigmas[:, i] = np.round(0.01 * data[dim], 4)
+
+    data["covariance"] = CoordinateCovariances.from_sigmas(sigmas)
+    data["time"] = Timestamp.from_mjd(
+        np.round(np.linspace(59000.0, 59000.0 + num_orbits, num_orbits), 3),
+        scale="tdb",
+    )
+    data["origin"] = Origin.from_kwargs(code=["SUN" for i in range(num_orbits)])
+    data["frame"] = "ecliptic"
+
+    coords = KeplerianCoordinates.from_kwargs(**data)
+    object_ids = [f"Object {i:03d}" for i in range(num_orbits)]
+    orbit_ids = [f"Orbit {i:03d}" for i in range(num_orbits)]
+
+    orbits = Orbits.from_kwargs(
+        coordinates=coords.to_cartesian(),
+        orbit_id=orbit_ids,
+        object_id=object_ids,
+    )
+    return orbits
```

### Comparing `adam_core-0.1.0/adam_core/orbits/query/horizons.py` & `adam_core-0.2.0a1/src/adam_core/orbits/query/horizons.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,136 +1,250 @@
 from typing import List, Union
 
 import numpy.typing as npt
 import pandas as pd
-from astropy.time import Time
 from astroquery.jplhorizons import Horizons
 
 from ...coordinates.cartesian import CartesianCoordinates
 from ...coordinates.cometary import CometaryCoordinates
 from ...coordinates.keplerian import KeplerianCoordinates
 from ...coordinates.origin import Origin
-from ...coordinates.times import Times
+from ...observers import Observers
+from ...time import Timestamp
 from ..orbits import Orbits
 
 
 def _get_horizons_vectors(
     object_ids: Union[List, npt.ArrayLike],
-    times: Time,
+    times: Timestamp,
     location: str = "@sun",
     id_type: str = "smallbody",
     aberrations: str = "geometric",
+    refplane: str = "ecliptic",
 ) -> pd.DataFrame:
     """
     Query JPL Horizons (through astroquery) for an object's
     state vectors at the given times.
 
     Parameters
     ----------
-    object_ids : `~numpy.ndarray` (N)
+    object_ids : Union[List, `~numpy.ndarray`] (N)
         Object IDs / designations recognizable by HORIZONS.
-    times : `~astropy.core.time.Time` (M)
-        Astropy time object at which to gather state vectors.
+    times : Timestamp (M)
+        Time at which to gather state vectors.
     location : str, optional
         Location of the origin typically a NAIF code.
         ('0' or '@ssb' for solar system barycenter, '10' or '@sun' for heliocenter)
         [Default = '@sun']
     id_type : {'majorbody', 'smallbody', 'designation',
                'name', 'asteroid_name', 'comet_name', 'id'}
         ID type, Horizons will find closest match under any given type.
     aberrations : {'geometric', 'astrometric', 'apparent'}
         Adjust state for one of three different aberrations.
+    refplane : {'ecliptic', 'earth'}
+        Reference plane for state vectors.
 
     Returns
     -------
     vectors : `~pandas.DataFrame`
         Dataframe containing the full cartesian state, r, r_rate, delta, delta_rate and light time
         of the object at each time.
     """
     dfs = []
-    for obj_id in object_ids:
+    for i, obj_id in enumerate(object_ids):
         obj = Horizons(
             id=obj_id,
-            epochs=times.tdb.mjd,
+            epochs=times.rescale("tdb").mjd().to_numpy(zero_copy_only=False),
             location=location,
             id_type=id_type,
         )
         vectors = obj.vectors(
-            refplane="ecliptic", aberrations=aberrations, cache=False
+            refplane=refplane, aberrations=aberrations, cache=False
         ).to_pandas()
+        vectors.insert(0, "orbit_id", f"{i:05d}")
         dfs.append(vectors)
 
     vectors = pd.concat(dfs, ignore_index=True)
+    vectors.sort_values(
+        by=["orbit_id", "datetime_jd"],
+        inplace=True,
+        ignore_index=True,
+    )
     return vectors
 
 
 def _get_horizons_elements(
     object_ids: Union[List, npt.ArrayLike],
-    times: Time,
+    times: Timestamp,
     location: str = "@sun",
     id_type: str = "smallbody",
+    refplane: str = "ecliptic",
 ) -> pd.DataFrame:
     """
     Query JPL Horizons (through astroquery) for an object's
     elements at the given times.
 
     Parameters
     ----------
-    object_ids : `~numpy.ndarray` (N)
+    object_ids : Union[List, `~numpy.ndarray`] (N)
         Object IDs / designations recognizable by HORIZONS.
-    times : `~astropy.core.time.Time`
-        Astropy time object at which to gather state vectors.
+    times : Timestamp
+        Time at which to gather state vectors.
     location : str, optional
         Location of the origin typically a NAIF code.
         ('0' or '@ssb' for solar system barycenter, '10' or '@sun' for heliocenter)
         [Default = '@sun']
     id_type : {'majorbody', 'smallbody', 'designation',
                'name', 'asteroid_name', 'comet_name', 'id'}
         ID type, Horizons will find closest match under any given type.
+    refplane : {'ecliptic', 'earth'}
+        Reference plane for orbital elements.
 
     Returns
     -------
     elements : `~pandas.DataFrame`
         Dataframe containing the full cartesian state, r, r_rate, delta, delta_rate and light time
         of the object at each time.
     """
     dfs = []
-    for obj_id in object_ids:
+    for i, obj_id in enumerate(object_ids):
         obj = Horizons(
             id=obj_id,
-            epochs=times.tdb.mjd,
+            epochs=times.rescale("tdb").mjd().to_numpy(zero_copy_only=False),
             location=location,
             id_type=id_type,
         )
         elements = obj.elements(
-            refsystem="J2000", refplane="ecliptic", tp_type="absolute", cache=False
+            refsystem="J2000", refplane=refplane, tp_type="absolute", cache=False
         ).to_pandas()
+        elements.insert(0, "orbit_id", f"{i:05d}")
         dfs.append(elements)
 
     elements = pd.concat(dfs, ignore_index=True)
+    elements.sort_values(
+        by=["orbit_id", "datetime_jd"],
+        inplace=True,
+        ignore_index=True,
+    )
     return elements
 
 
+def _get_horizons_ephemeris(
+    object_ids: Union[List, npt.ArrayLike],
+    times: Timestamp,
+    location: str,
+    id_type: str = "smallbody",
+) -> pd.DataFrame:
+    """
+    Query JPL Horizons (through astroquery) for an object's
+    predicted ephemeris as seen from a given location at the given times.
+
+    Parameters
+    ----------
+    object_ids : Union[List, `~numpy.ndarray`] (N)
+        Object IDs / designations recognizable by HORIZONS.
+    times : Timestamp
+        Time at which to gather state vectors.
+    location : str, optional
+        Location of the origin typically a NAIF code or MPC observatory code
+    id_type : {'majorbody', 'smallbody', 'designation',
+               'name', 'asteroid_name', 'comet_name', 'id'}
+        ID type, Horizons will find closest match under any given type.
+
+    Returns
+    -------
+    ephemeris : `~pandas.DataFrame`
+        Dataframe containing the predicted ephemerides of the given objects
+        as seen from the observer location at the given times.
+    """
+    dfs = []
+    for i, obj_id in enumerate(object_ids):
+        obj = Horizons(
+            id=obj_id,
+            epochs=times.rescale("utc").mjd().to_numpy(zero_copy_only=False),
+            location=location,
+            id_type=id_type,
+        )
+        ephemeris = obj.ephemerides(
+            # RA, DEC, r, r_rate, delta, delta_rate, lighttime
+            # quantities="1, 2, 19, 20, 21",
+            extra_precision=True,
+            cache=False,
+        ).to_pandas()
+        ephemeris.insert(0, "orbit_id", f"{i:05d}")
+        ephemeris.insert(2, "mjd_utc", times.utc.mjd)
+        ephemeris.insert(3, "observatory_code", location)
+
+        dfs.append(ephemeris)
+
+    ephemeris = pd.concat(dfs)
+    ephemeris.sort_values(
+        by=["orbit_id", "datetime_jd", "observatory_code"],
+        inplace=True,
+        ignore_index=True,
+    )
+    return ephemeris
+
+
+def query_horizons_ephemeris(
+    object_ids: Union[List, npt.ArrayLike], observers: Observers
+) -> pd.DataFrame:
+    """
+    Query JPL Horizons (through astroquery) for an object's predicted ephemeris
+    as seen from a given location at the given times.
+
+    Parameters
+    ----------
+    object_ids : Union[List, `~numpy.ndarray`] (N)
+        Object IDs / designations recognizable by HORIZONS.
+    observers : `~adam_core.observers.observers.Observers`
+        Observers object containing the location and times
+        of the observers.
+
+    Returns
+    -------
+    ephemeris : `~pandas.DataFrame`
+        Dataframe containing the predicted ephemerides of the given objects
+        as seen from the observer location at the given times.
+    """
+    dfs = []
+    for observatory_code, observers_i in observers.iterate_codes():
+        ephemeris = _get_horizons_ephemeris(
+            object_ids,
+            observers_i.coordinates.time,
+            observatory_code,
+        )
+        dfs.append(ephemeris)
+
+    ephemeris = pd.concat(dfs, ignore_index=True)
+    ephemeris.sort_values(
+        by=["orbit_id", "datetime_jd", "observatory_code"],
+        inplace=True,
+        ignore_index=True,
+    )
+    return ephemeris
+
+
 def query_horizons(
     object_ids: Union[List, npt.ArrayLike],
-    times: Time,
+    times: Timestamp,
     coordinate_type: str = "cartesian",
     location: str = "@sun",
     id_type: str = "smallbody",
     aberrations: str = "geometric",
 ) -> Orbits:
     """
     Query JPL Horizons (through astroquery) for an object's state vectors or elements at the given times.
 
     Parameters
     ----------
     object_ids : npt.ArrayLike (N)
         Object IDs / designations recognizable by HORIZONS.
-    times : `~astropy.core.time.Time` (M)
-        Astropy time object at which to gather state vectors.
+    times : Timestamp (M)
+        Time at which to gather state vectors.
     coordinate_type : {'cartesian', 'keplerian', 'cometary'}
         Type of orbital elements to return.
     location : str, optional
         Location of the origin typically a NAIF code.
         ('0' or '@ssb' for solar system barycenter, '10' or '@sun' for heliocenter)
         [Default = '@sun']
     id_type : {'majorbody', 'smallbody', 'designation',
@@ -149,90 +263,97 @@
             object_ids,
             times,
             location=location,
             id_type=id_type,
             aberrations=aberrations,
         )
 
-        times = Times.from_astropy(
-            Time(vectors["datetime_jd"].values, scale="tdb", format="jd")
-        )
+        times = Timestamp.from_jd(vectors["datetime_jd"].values, scale="tdb")
         origin = Origin.from_kwargs(code=["SUN" for i in range(len(times))])
         frame = "ecliptic"
         coordinates = CartesianCoordinates.from_kwargs(
-            times=times,
+            time=times,
             x=vectors["x"].values,
             y=vectors["y"].values,
             z=vectors["z"].values,
             vx=vectors["vx"].values,
             vy=vectors["vy"].values,
             vz=vectors["vz"].values,
             origin=origin,
             frame=frame,
         )
-        object_ids = vectors["targetname"].values
+        orbit_id = vectors["orbit_id"].values
+        object_id = vectors["targetname"].values
 
-        return Orbits.from_kwargs(object_ids=object_ids, coordinates=coordinates)
+        return Orbits.from_kwargs(
+            orbit_id=orbit_id, object_id=object_id, coordinates=coordinates
+        )
 
     elif coordinate_type == "keplerian":
         elements = _get_horizons_elements(
             object_ids,
             times,
             location=location,
             id_type=id_type,
         )
 
-        times = Times.from_astropy(
-            Time(elements["datetime_jd"].values, scale="tdb", format="jd")
+        times = Timestamp.from_jd(
+            elements["datetime_jd"].values,
+            scale="tdb",
         )
         origin = Origin.from_kwargs(code=["SUN" for i in range(len(times))])
         frame = "ecliptic"
         coordinates = KeplerianCoordinates(
-            times=times,
+            time=times,
             a=elements["a"].values,
             e=elements["e"].values,
             i=elements["incl"].values,
             raan=elements["Omega"].values,
             ap=elements["w"].values,
             M=elements["M"].values,
             origin=origin,
             frame=frame,
         )
-        object_ids = elements["targetname"].values
+        orbit_id = elements["orbit_id"].values
+        object_id = elements["targetname"].values
 
         return Orbits.from_kwargs(
-            object_ids=object_ids, coordinates=coordinates.to_cartesian()
+            orbit_id=orbit_id,
+            object_id=object_id,
+            coordinates=coordinates.to_cartesian(),
         )
 
     elif coordinate_type == "cometary":
         elements = _get_horizons_elements(
             object_ids,
             times,
             location=location,
             id_type=id_type,
         )
 
-        tp = Time(elements["Tp_jd"].values, scale="tdb", format="jd")
-        times = Times.from_astropy(
-            Time(elements["datetime_jd"].values, scale="tdb", format="jd")
-        )
+        tp = Timestamp.from_jd(elements["Tp_jd"].values, scale="tdb")
+        times = Timestamp.from_jd(elements["datetime_jd"].values, scale="tdb")
         origin = Origin.from_kwargs(code=["SUN" for i in range(len(times))])
         frame = "ecliptic"
         coordinates = CometaryCoordinates.from_kwargs(
-            times=times,
+            time=times,
             q=elements["q"].values,
             e=elements["e"].values,
             i=elements["incl"].values,
             raan=elements["Omega"].values,
             ap=elements["w"].values,
-            tp=tp.tdb.mjd,
+            tp=tp.mjd(),
             origin=origin,
             frame=frame,
         )
-        object_ids = elements["targetname"].values
+        orbit_id = elements["orbit_id"].values
+        object_id = elements["targetname"].values
+
         return Orbits.from_kwargs(
-            object_ids=object_ids, coordinates=coordinates.to_cartesian()
+            orbit_id=orbit_id,
+            object_id=object_id,
+            coordinates=coordinates.to_cartesian(),
         )
 
     else:
         err = "coordinate_type should be one of {'cartesian', 'keplerian', 'cometary'}"
         raise ValueError(err)
```

### Comparing `adam_core-0.1.0/adam_core/orbits/query/sbdb.py` & `adam_core-0.2.0a1/src/adam_core/orbits/query/sbdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
 from typing import List, OrderedDict
 
 import numpy as np
 import numpy.typing as npt
-from astropy.time import Time
 from astroquery.jplsbdb import SBDB
 
 from ...coordinates.cometary import CometaryCoordinates
 from ...coordinates.covariances import CoordinateCovariances, sigmas_to_covariances
 from ...coordinates.origin import Origin
-from ...coordinates.times import Times
+from ...time import Timestamp
 from ..orbits import Orbits
 
 logger = logging.getLogger(__name__)
 
 
 def _convert_SBDB_covariances(
     sbdb_covariances: npt.ArrayLike,
@@ -131,24 +130,26 @@
 
     Raises
     ------
     NotFoundError: If any of the queries object IDs are not found.
     """
     results = _get_sbdb_elements(ids)
 
+    orbit_ids = []
     object_ids = []
     classes = []
     coords_cometary = np.zeros((len(results), 6), dtype=np.float64)
     covariances_sbdb = np.zeros((len(results), 6, 6), dtype=np.float64)
     times = np.zeros((len(results)), dtype=np.float64)
 
     for i, result in enumerate(results):
         if "object" not in result:
             raise NotFoundError("object {} was not found", ids[i])
 
+        orbit_ids.append(f"{i:05d}")
         object_ids.append(result["object"]["fullname"])
         classes.append(result["object"]["orbit_class"]["code"])
 
         orbit = result["orbit"]
         elements = orbit["elements"]
         epoch = orbit["epoch"]
         if "covariance" in orbit:
@@ -197,38 +198,41 @@
 
         times[i] = epoch.value
         coords_cometary[i, 0] = elements["q"].value
         coords_cometary[i, 1] = elements["e"]
         coords_cometary[i, 2] = elements["i"].value
         coords_cometary[i, 3] = elements["om"].value
         coords_cometary[i, 4] = elements["w"].value
-        coords_cometary[i, 5] = Time(elements["tp"].value, scale="tdb", format="jd").mjd
+        coords_cometary[i, 5] = (
+            Timestamp.from_jd([elements["tp"].value], scale="tdb").mjd()[0].as_py()
+        )
 
     covariances_cometary = _convert_SBDB_covariances(covariances_sbdb)
-    times = Times.from_astropy(Time(times, scale="tdb", format="jd"))
+    times = Timestamp.from_jd(times, scale="tdb")
     origin = Origin.from_kwargs(code=["SUN" for i in range(len(times))])
     frame = "ecliptic"
     coordinates = CometaryCoordinates.from_kwargs(
-        times=times,
+        time=times,
         q=coords_cometary[:, 0],
         e=coords_cometary[:, 1],
         i=coords_cometary[:, 2],
         raan=coords_cometary[:, 3],
         ap=coords_cometary[:, 4],
         tp=coords_cometary[:, 5],
-        covariances=CoordinateCovariances.from_matrix(covariances_cometary),
+        covariance=CoordinateCovariances.from_matrix(covariances_cometary),
         origin=origin,
         frame=frame,
     )
 
-    object_ids = np.array(object_ids)
+    orbit_ids = np.array(orbit_ids, dtype="object")
+    object_ids = np.array(object_ids, dtype="object")
     classes = np.array(classes)
 
     return Orbits.from_kwargs(
-        object_ids=object_ids, coordinates=coordinates.to_cartesian()
+        orbit_id=orbit_ids, object_id=object_ids, coordinates=coordinates.to_cartesian()
     )
 
 
 class NotFoundError(Exception):
     def __init__(self, message, object_id):
         self.message = message
         self.object_id = object_id
```

### Comparing `adam_core-0.1.0/adam_core/orbits/query/tests/__init__.py` & `adam_core-0.2.0a1/src/adam_core/orbits/query/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.1.0/adam_core/orbits/query/tests/test_sbdb.py` & `adam_core-0.2.0a1/src/adam_core/orbits/query/tests/test_sbdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,16 @@
             "i",
             "A2",
         ]
         result = query_sbdb(["54509"])
         mock.assert_called_once()
 
     assert len(result) == 1
-    assert result.coordinates.covariances.to_matrix().shape == (1, 6, 6)
-    assert not np.isnan(result.coordinates.covariances.to_matrix()).all()
+    assert result.coordinates.covariance.to_matrix().shape == (1, 6, 6)
+    assert not np.isnan(result.coordinates.covariance.to_matrix()).all()
 
 
 def test_query_sbdb_for_missing_value():
     with pytest.raises(NotFoundError):
         with mock_sbdb_query("missing.json"):
             query_sbdb(["missing"])
```

### Comparing `adam_core-0.1.0/adam_core/orbits/tests/test_orbits.py` & `adam_core-0.2.0a1/src/adam_core/orbits/tests/test_orbits.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-from astropy.time import Time
-
 from ...coordinates import CartesianCoordinates
 from ...coordinates.origin import Origin
-from ...coordinates.times import Times
+from ...time import Timestamp
 from ...utils.helpers import orbits as orbits_helpers
 from ..orbits import Orbits
 
 
 def test_orbits__init__():
     coordinates = CartesianCoordinates.from_kwargs(
         x=[0.5],
         y=[0.5],
         z=[0.004],
         vx=[0.005],
         vy=[-0.005],
         vz=[0.0002],
-        times=Times.from_astropy(Time([59000.0], scale="tdb", format="mjd")),
+        time=Timestamp.from_mjd([59000.0], scale="tdb"),
         origin=Origin.from_kwargs(code=["SUN"]),
         frame="ecliptic",
     )
 
     orbits = Orbits.from_kwargs(
-        coordinates=coordinates, orbit_ids=["1"], object_ids=["Test Orbit"]
+        coordinates=coordinates, orbit_id=["1"], object_id=["Test Orbit"]
     )
 
-    assert orbits.orbit_ids[0].as_py() == "1"
-    assert orbits.object_ids[0].as_py() == "Test Orbit"
-    assert orbits.coordinates.times.jd1.to_numpy()[0] == 2459000.0
-    assert orbits.coordinates.times.jd2.to_numpy()[0] == 0.5
-    assert orbits.coordinates.times.scale == "tdb"
+    assert orbits.orbit_id[0].as_py() == "1"
+    assert orbits.object_id[0].as_py() == "Test Orbit"
+    assert orbits.coordinates.time.days.to_numpy()[0] == 59000
+    assert orbits.coordinates.time.nanos.to_numpy()[0] == 0
+    assert orbits.coordinates.time.scale == "tdb"
     assert orbits.coordinates.x.to_numpy()[0] == 0.5
     assert orbits.coordinates.y.to_numpy()[0] == 0.5
     assert orbits.coordinates.z.to_numpy()[0] == 0.004
     assert orbits.coordinates.vx.to_numpy()[0] == 0.005
     assert orbits.coordinates.vy.to_numpy()[0] == -0.005
     assert orbits.coordinates.vz.to_numpy()[0] == 0.0002
```

### Comparing `adam_core-0.1.0/adam_core/utils/helpers/tests/test_orbits.py` & `adam_core-0.2.0a1/src/adam_core/utils/helpers/tests/test_orbits.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from ..orbits import make_real_orbits, make_simple_orbits
 
 
 def test_make_real_orbits():
     # Test that all sample orbits are read from the CSV file
     orbits = make_real_orbits()
-    assert len(orbits) == 27
+    assert len(orbits) == 28
 
     # Test that the number of orbits returned is correct
     orbits = make_real_orbits(num_orbits=10)
     assert len(orbits) == 10
 
 
 def test_make_simple_orbits_raises():
-    # Test that a ValueError is raised if num_orbits > 27
+    # Test that a ValueError is raised if num_orbits > 29
     with pytest.raises(ValueError):
-        make_real_orbits(num_orbits=28)
+        make_real_orbits(num_orbits=29)
 
 
 def test_make_simple_orbits():
     # Test that the number of orbits returned is correct
     orbits = make_simple_orbits(num_orbits=10)
     assert len(orbits) == 10
```

### Comparing `adam_core-0.1.0/adam_core/utils/mpc.py` & `adam_core-0.2.0a1/src/adam_core/utils/mpc.py`

 * *Files identical despite different names*

### Comparing `adam_core-0.1.0/adam_core/utils/tests/test_mpc.py` & `adam_core-0.2.0a1/src/adam_core/utils/tests/test_mpc.py`

 * *Files identical despite different names*

