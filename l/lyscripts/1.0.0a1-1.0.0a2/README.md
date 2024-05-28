# Comparing `tmp/lyscripts-1.0.0a1.tar.gz` & `tmp/lyscripts-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyscripts-1.0.0a1.tar", last modified: Wed Apr  3 13:01:05 2024, max compression
+gzip compressed data, was "lyscripts-1.0.0a2.tar", last modified: Tue May 28 12:57:29 2024, max compression
```

## Comparing `lyscripts-1.0.0a1.tar` & `lyscripts-1.0.0a2.tar`

### file list

```diff
@@ -1,134 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.329456 lyscripts-1.0.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.309456 lyscripts-1.0.0a1/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1044 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      815 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.305456 lyscripts-1.0.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.309456 lyscripts-1.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-03 13:01:05.329456 lyscripts-1.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.313456 lyscripts-1.0.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.313456 lyscripts-1.0.0a1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.313456 lyscripts-1.0.0a1/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.313456 lyscripts-1.0.0a1/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    18415 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)   105407 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/_static/github-social-card.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.313456 lyscripts-1.0.0a1/docs/source/app/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/app/init.rst
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/app/prevalence.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.313456 lyscripts-1.0.0a1/docs/source/compute/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/compute/init.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/compute/posteriors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/compute/prevalences.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/compute/priors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/compute/risks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/compute/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.317456 lyscripts-1.0.0a1/docs/source/data/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/enhance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/filter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/generate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/init.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/join.rst
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/lyproxify.rst
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/split.rst
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/data/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/decorators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/evaluate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/init.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.317456 lyscripts-1.0.0a1/docs/source/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/plot/corner.rst
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/plot/histograms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/plot/init.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/plot/thermo_int.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/plot/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/sample.rst
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/scenario.rst
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/temp_schedule.rst
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/docs/source/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18415 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)   105407 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/github-social-card.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.317456 lyscripts-1.0.0a1/lyscripts/
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.321456 lyscripts-1.0.0a1/lyscripts/app/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/app/prevalence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.321456 lyscripts-1.0.0a1/lyscripts/compute/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/posteriors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/prevalences.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/priors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/risks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/compute/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.321456 lyscripts-1.0.0a1/lyscripts/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10189 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/enhance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/join.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/lyproxify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/split.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.321456 lyscripts-1.0.0a1/lyscripts/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/plot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/plot/corner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/plot/histograms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/plot/thermo_int.py
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/temp_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    16344 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/lyscripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.329456 lyscripts-1.0.0a1/lyscripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 13:01:05.000000 lyscripts-1.0.0a1/lyscripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:01:05.329456 lyscripts-1.0.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.325456 lyscripts-1.0.0a1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.325456 lyscripts-1.0.0a1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/data/a.csv
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/data/b.csv
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/data/join_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.325456 lyscripts-1.0.0a1/tests/plot/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.325456 lyscripts-1.0.0a1/tests/plot/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/plot/baseline/sine.png
--rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/plot/baseline/sine.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/plot/baseline/sine_svg.png
--rw-r--r--   0 runner    (1001) docker     (127)    36976 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/plot/baseline/test_draw.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.325456 lyscripts-1.0.0a1/tests/plot/data/
--rw-r--r--   0 runner    (1001) docker     (127)    86144 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/plot/data/beta_samples.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/plot/plot_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:01:05.329456 lyscripts-1.0.0a1/tests/predict/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/predict/predict_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/predict/prevalences_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/run_doctests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   397288 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/test_backend.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/test_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/test_params_v0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/test_params_v1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/test_sample_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-03 13:00:53.000000 lyscripts-1.0.0a1/tests/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.596112 lyscripts-1.0.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.576112 lyscripts-1.0.0a2/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1044 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      815 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.572112 lyscripts-1.0.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.576112 lyscripts-1.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    17682 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-28 12:57:29.596112 lyscripts-1.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.576112 lyscripts-1.0.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.576112 lyscripts-1.0.0a2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.580112 lyscripts-1.0.0a2/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.580112 lyscripts-1.0.0a2/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18415 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   105407 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/_static/github-social-card.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.580112 lyscripts-1.0.0a2/docs/source/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/app/init.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/app/prevalence.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.580112 lyscripts-1.0.0a2/docs/source/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/compute/init.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/compute/posteriors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/compute/prevalences.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/compute/priors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/compute/risks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/compute/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.580112 lyscripts-1.0.0a2/docs/source/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/data/enhance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/data/filter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/data/generate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/data/init.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/data/join.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/data/lyproxify.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/data/split.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/data/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/evaluate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/init.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.580112 lyscripts-1.0.0a2/docs/source/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/plot/corner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/plot/histograms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/plot/init.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/plot/thermo_int.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/plot/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/sample.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/scenario.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/temp_schedule.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/docs/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18415 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   105407 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/github-social-card.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.584112 lyscripts-1.0.0a2/lyscripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-28 12:57:29.000000 lyscripts-1.0.0a2/lyscripts/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.584112 lyscripts-1.0.0a2/lyscripts/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/app/prevalence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.584112 lyscripts-1.0.0a2/lyscripts/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/compute/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/compute/posteriors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/compute/prevalences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/compute/priors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/compute/risks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/compute/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.588112 lyscripts-1.0.0a2/lyscripts/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/data/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10189 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/data/enhance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/data/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/data/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11224 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/data/lyproxify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/data/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.588112 lyscripts-1.0.0a2/lyscripts/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/plot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/plot/corner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/plot/histograms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/plot/thermo_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14290 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/temp_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16344 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/lyscripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.592112 lyscripts-1.0.0a2/lyscripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-28 12:57:29.000000 lyscripts-1.0.0a2/lyscripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-28 12:57:29.000000 lyscripts-1.0.0a2/lyscripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:57:29.000000 lyscripts-1.0.0a2/lyscripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 12:57:29.000000 lyscripts-1.0.0a2/lyscripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-28 12:57:29.000000 lyscripts-1.0.0a2/lyscripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 12:57:29.000000 lyscripts-1.0.0a2/lyscripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:57:29.596112 lyscripts-1.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.592112 lyscripts-1.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.592112 lyscripts-1.0.0a2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/data/a.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/data/b.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/data/join_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.592112 lyscripts-1.0.0a2/tests/plot/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.592112 lyscripts-1.0.0a2/tests/plot/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/plot/baseline/sine.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/plot/baseline/sine.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/plot/baseline/sine_svg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36976 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/plot/baseline/test_draw.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.592112 lyscripts-1.0.0a2/tests/plot/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    86144 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/plot/data/beta_samples.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/plot/plot_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:57:29.592112 lyscripts-1.0.0a2/tests/predict/
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/predict/predict_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/predict/prevalences_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/run_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   397288 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/test_backend.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/test_params_v0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/test_params_v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/test_sample_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-28 12:57:13.000000 lyscripts-1.0.0a2/tests/utils_test.py
```

### Comparing `lyscripts-1.0.0a1/.chglog/CHANGELOG.tpl.md` & `lyscripts-1.0.0a2/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/.chglog/config.yml` & `lyscripts-1.0.0a2/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/.github/workflows/build.yml` & `lyscripts-1.0.0a2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/.github/workflows/tests.yml` & `lyscripts-1.0.0a2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/.gitignore` & `lyscripts-1.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/.pre-commit-config.yaml` & `lyscripts-1.0.0a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/.readthedocs.yml` & `lyscripts-1.0.0a2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/CHANGELOG.md` & `lyscripts-1.0.0a2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,137 +1,151 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
-<a name="1.0.0.a1"></a>
-## [1.0.0.a1] - 2024-04-03
+<a name="1.0.0.a2"></a>
+## [1.0.0.a2] - 2024-04-28
 
-This prerelease finishes updating the code to the new [`lymph`] package API. It also features a rewrite of the commands to predict and compute e.g. risks and prevalences.
+### 🚀 Features
 
-[`lymph`]: https://lymph-model.readthedocs.io
+- *(sample)* Allow no multiprocessing (0 cores)
+- *(scenario)* Add `from_dict` classmethod
+- *(plot)* Add `offset` to hist and beta dist
 
+### 🐛 Bug Fixes
 
-### Bug Fixes
+- Use correct heaer rows, fixes [#57]
+- *(compute)* Observe bilateral prevalence
+- *(scenario)* Dataclass with prpoerty issue
+- Ensure sides in scenario diagnose/involvement
+- *(compute)* Correct obs and pred prevalences
 
-- ⚠ **BREAKING** Use modern lydata cols for t_stage matching.
-- Wrong lnls in predict prevalences.
-- ⚠ **BREAKING** Update prevalence prediction to new lymph API.
-- (**sample**) Match T-stage mapping with lymph API.\
-  The lymph model now accepts callables and dicts as T-stage mapping (but
-  not `None`). I can hence simply pass the dictionary from the config to
-  the loading function.
-- (**data**) Stop dtype change during `concat`.\
-  When a `DataFrame` with no `NaN`s was joined with one consisting _only_
-  of `NaN`s, then it forced some weird kind of dtype conversion onty the
-  respective column. Now, dtypes are converted _before_ the concatenation,
-  fixing that issue.
-- (**sample**) Skip 0 iter convergence check.
-- (**sample**) Missing import.
-- (**sample**) Only pass `side` to unilateral model.
-- (**sample**) Display converged message nicely.
-- (**utils**) Correct default args for `get_chain()`.
-- Wrong posterior shape.
-- (**predict**) Even out some bugs.
-- Don't pycln accessor import.
-- (**data**) Enhance failed due to copy on write.
+### 📚 Documentation
 
-### Documentation
+- *(data)* Refactor lyproxify docstrings
+- Update badge to link to RTD, fixes [#53]
 
-- Start with basic sphinx setup.
-- Start organizing top-level cmds with sphinx.
-- Include all modules in docs.
-- Update docstrings to reST format.
-- Add document files for precompute subcmd.
-- Allow links to lymph docs.
-- Fix `temp_schedule` docstring.
-- Shorten titles.
-- (**predict**) Update prevalence module docstring.
-- Refactor docs for new `compute` subcommand.
-- Fix typos and missing modules.
+### 🧪 Testing
 
-### Features
+- Fix testing setup & add new histogram test
 
-- (**data**) Add simple data filter command. Fixes [#51].
-- Customize log handler for better filename.
-- (**sample**) Allow custom T-stage mapping.
-- (**sample**) Allow to load `side` data.
-- (**utils**) Allow `Unilateral.binary` in params.
-- (**sample**) Display time elapsed during burnin.
-- (**predict**) Add cmd to precompute state dists.
-- (**precompute**) Add `priors` cmd. Related [#54].\
-  This allows precomputing the state distributions of all three
-  implemented lymph models.
-- (**utils**) Allow keywords in modalities def.\
-  One may now use a dict with keys `spec`, `sens`, and `kind` to define a
-  modality in the YAML params.
-- (**post**) Compute for multiple scenarios.\
-  One may now compute the posteriors for a list of defined scenarios.
-- Add class for storing scenarios.
-- (**precompute**) Priors from list of scenarios.
-- (**predict**) Finish prevalences cmd.
-- (**data**) Implement custom pandas accessor.
-- (**scenario**) Track laterality as well.
-- (**compute**) Risk works with lymph v1, too, now.
+### Change
 
-### Testing
+- *(data)* Make copy before edit in-place
+- *(scenario)* Make scenario dataclass
 
-- (**data**) Ensure new joining works correctly.
-- (**sample**) Check some sampling methods.
-- Fix typos in tests.
-- Update failing tests.
+### Merge
 
-### Build
+- Branch '57-lyproxify-loads-wrong-number-of-header-rows' into 'dev'
 
-- Bump lymph-model to v1.0.
-- Bump lymph version & add sphinx deps.
 
-### Change
+<a name="1.0.0.a1"></a>
+## [1.0.0.a1] - 2024-04-03
 
-- ⚠ **BREAKING** (**sample**) Reimplement sampling command.
-- (**precompute**) Use HDF5 cache. Fixes [#54].\
-  The `priors` and `posteriors` commands now use a simple `HDF5FileCache`
-  to avoid recomputing either of those quantities unnecessarily.
-- (**precompute**) Make recursive. Related [#54].\
-  The computation of priors and posteriors is now somewhat recursive. This
-  will allow us to just call one function and it will automatically
-  compute the priors, posteriors, and risks if necessary.
-- (**prevs**) Start on updated `prevalences` cmd.
-- Replace 'diagnose' & bump lymph to 1.2.0.
-- (**precompute**) Posteriors only from priors.\
-  Posteriors now require priors and cannot compute priors "along the way"
-  from given samples. This is to make it clear which is an input file and
-  which an output file. Otherwise, caching would have been even trickier.
-- (**scenario**) Shorten hash to 6 digits.
+### 🚀 Features
 
-### Ci
+- *(data)* Add simple data filter command, fixes [#51]
+- Customize log handler for better filename
+- *(sample)* Allow custom T-stage mapping
+- *(sample)* Allow to load `side` data
+- *(utils)* Allow `Unilateral.binary` in params
+- *(sample)* Display time elapsed during burnin
+- *(predict)* Add cmd to precompute state dists
+- *(post)* Start with posterior cmd (WIP)
+- *(precompute)* Add `priors` cmd, related to [#54]
+- *(precompute)* Work on posterior (WIP)
+- *(utils)* Allow keywords in modalities def
+- *(post)* Compute for multiple scenarios
+- *(predict)* Update prevalences cmd (WIP)
+- Add class for storing scenarios
+- *(precompute)* Priors from list of scenarios
+- *(predict)* Finish prevalences cmd
+- *(data)* Implement custom pandas accessor
+- *(scenario)* Track laterality as well
+- *(compute)* Risk works with lymph v1, too, now
+
+### 🐛 Bug Fixes
+
+- [**breaking**] Use modern lydata cols for t_stage matching
+- Wrong lnls in predict prevalences
+- [**breaking**] Update prev prediction to new lymph API
+- *(sample)* Match T-stage mapping with lymph API
+- *(data)* Stop dtype change during `concat`
+- *(sample)* Skip 0 iter convergence check
+- *(sample)* Missing import
+- *(sample)* Only pass `side` to unilateral model
+- *(sample)* Display converged message nicely
+- *(utils)* Correct default args for `get_chain()`
+- Wrong posterior shape
+- *(predict)* Even out some bugs
+- Don't pycln accessor import
+- *(data)* Enhance failed due to copy on write
+
+### 📚 Documentation
+
+- Start with basic sphinx setup
+- Start organizing top-level cmds with sphinx
+- Include all modules in docs
+- Update docstrings to reST format
+- Add document files for precompute subcmd
+- Allow links to lymph docs
+- Fix `temp_schedule` docstring
+- Shorten titles
+- *(predict)* Update prevalence module docstring
+- Refactor docs for new `compute` subcommand
+- Fix typos and missing modules
+
+### 🧪 Testing
+
+- *(data)* Ensure new joining works correctly
+- *(sample)* Check some sampling methods
+- Fix typos in tests
+- Update failing tests
+
+### ⚙️ Miscellaneous Tasks
+
+- Add readthedocs config file
+- Remove pdoc action
+- Update changelog
+
+### Build
 
-- Add readthedocs config file.
-- Remove pdoc action.
+- Bump lymph-model to v1.0
+- Bump lymph version & add sphinx deps
+
+### Change
+
+- *(sample)* [**breaking**] Start on new sample command (WIP)
+- *(sample)* [**breaking**] Reimplement sampling command
+- *(precompute)* Use HDF5 cache
+- *(precompute)* Make recursive. Related: [#54]
+- *(prevs)* Start on updated `prevalences` cmd
+- Replace 'diagnose' & bump lymph to 1.2.0
+- Simplify scenario handling (WIP)
+- *(precompute)* Posteriors only from priors
+- *(scenario)* Shorten hash to 6 digits
 
 ### Merge
 
-- Branch 'main' into 'dev'.
-- Branch '51-filter-command' into 'dev'.
-- Branch '53-use-sphinx-for-documentation' into 'dev'.
-- Branch '54-add-precompute-commands' into 'dev'.
+- Branch 'main' into 'dev'
+- Branch '51-filter-command' into 'dev'
+- Branch '53-use-sphinx-for-documentation' into 'dev'
+- Branch '54-add-precompute-commands' into 'dev'
 
 ### Refac
 
-- (**sample**) Better progress tracking.
-- (**precompute**) Comp state dist in own submod.
-- (**utils**) Move funcs out of `precompute`.
-- Bundle adding scneario args to parser.
-- (**compute**) Predict & precompute -> compute.\
-  The `predict` and `precompute` commands are now bundled under the
-  subcommand `compute`.
-
+- *(sample)* Better progress tracking
+- *(precompute)* Comp state dist in own submod
+- *(utils)* Move funcs out of `precompute`
+- Bundle adding scneario args to parser
+- *(compute)* Predict & precompute -> compute
 
 ### Remove
 
-- ⚠ **BREAKING** Midline_ext in create_patient_row for now.
+- [**breaking**] Midline_ext in create_patient_row for now
 
 
 <a name="1.0.0.a0"></a>
 ## [1.0.0.a0] - 2023-12-20
 
 ### Bug Fixes
 
@@ -473,15 +487,16 @@
 - set up git-chglog for creating changelogs
 - add pre-commit hook to check commit msg
 
 
 <a name="0.5.3"></a>
 ## [0.5.3] - 2022-08-22
 
-[Unreleased]: https://github.com/rmnldwg/lyscripts/compare/1.0.0.a1...HEAD
+[unreleased]: https://github.com/rmnldwg/lyscripts/compare/1.0.0.a2...HEAD
+[1.0.0.a2]: https://github.com/rmnldwg/lyscripts/compare/1.0.0.a1...1.0.0.a2
 [1.0.0.a1]: https://github.com/rmnldwg/lyscripts/compare/1.0.0.a0...1.0.0.a1
 [1.0.0.a0]: https://github.com/rmnldwg/lyscripts/compare/0.7.3...1.0.0.a0
 [0.7.3]: https://github.com/rmnldwg/lyscripts/compare/0.7.2...0.7.3
 [0.7.2]: https://github.com/rmnldwg/lyscripts/compare/0.7.1...0.7.2
 [0.7.1]: https://github.com/rmnldwg/lyscripts/compare/0.7.0...0.7.1
 [0.7.0]: https://github.com/rmnldwg/lyscripts/compare/0.6.9...0.7.0
 [0.6.9]: https://github.com/rmnldwg/lyscripts/compare/0.6.8...0.6.9
@@ -520,13 +535,15 @@
 [#31]: https://github.com/rmnldwg/lyscripts/issues/31
 [#33]: https://github.com/rmnldwg/lyscripts/issues/33
 [#40]: https://github.com/rmnldwg/lyscripts/issues/40
 [#41]: https://github.com/rmnldwg/lyscripts/issues/41
 [#44]: https://github.com/rmnldwg/lyscripts/issues/44
 [#45]: https://github.com/rmnldwg/lyscripts/issues/45
 [#51]: https://github.com/rmnldwg/lyscripts/issues/51
+[#53]: https://github.com/rmnldwg/lyscripts/issues/53
 [#54]: https://github.com/rmnldwg/lyscripts/issues/54
+[#57]: https://github.com/rmnldwg/lyscripts/issues/57
 
 [`emcee`]: https://emcee.readthedocs.io/en/stable/
 [`rich`]: https://rich.readthedocs.io/en/latest/
 [`rich_argparse`]: https://github.com/hamdanal/rich_argparse
 [LyProX]: https://lyprox.org
```

### Comparing `lyscripts-1.0.0a1/LICENSE` & `lyscripts-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/PKG-INFO` & `lyscripts-1.0.0a2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyscripts
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Package containing scripts used in lynference pipelines
 Author-email: Roman Ludwig <roman.ludwig@usz.ch>
 License: MIT
 Project-URL: source, https://github.com/rmnldwg/lyscripts
 Project-URL: documentation, https://rmnldwg.github.io/lyscripts
 Keywords: scripts,lymph,inference
 Classifier: Programming Language :: Python :: 3
@@ -43,15 +43,15 @@
 Requires-Dist: streamlit; extra == "apps"
 
 <img src="https://raw.githubusercontent.com/rmnldwg/lyscripts/main/github-social-card.png" alt="social card" style="width:830px;"/>
 
 [![MIT license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/rmnldwg/lyscripts/blob/main/LICENSE)
 [![GitHub repo](https://img.shields.io/badge/rmnldwg%2Flymph-grey.svg?style=flat&logo=github)](https://github.com/rmnldwg/lyscripts)
 [![build badge](https://github.com/rmnldwg/lyscripts/actions/workflows/build.yml/badge.svg?style=flat)](https://pypi.org/project/lyscripts/)
-[![docs badge](https://github.com/rmnldwg/lyscripts/actions/workflows/docs.yml/badge.svg?style=flat)](https://rmnldwg.github.io/lyscripts/)
+[![docs badge](https://readthedocs.org/projects/lyscripts/badge/?version=latest)](https://lyscripts.readthedocs.io/en/latest/?badge=latest)
 [![tests badge](https://github.com/rmnldwg/lyscripts/actions/workflows/tests.yml/badge.svg?style=flat)](https://rmnldwg.github.io/lyscripts/)
 
 
 ## What are these `lyscripts`?
 
 This package provides convenient scripts for performing inference and learning regarding the lymphatic spread of head & neck cancer. Essentially, it provides a *command line interface* (CLI) to the [lymph](https://github.com/rmnldwg/lymph) library.
```

### Comparing `lyscripts-1.0.0a1/README.md` & `lyscripts-1.0.0a2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <img src="https://raw.githubusercontent.com/rmnldwg/lyscripts/main/github-social-card.png" alt="social card" style="width:830px;"/>
 
 [![MIT license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/rmnldwg/lyscripts/blob/main/LICENSE)
 [![GitHub repo](https://img.shields.io/badge/rmnldwg%2Flymph-grey.svg?style=flat&logo=github)](https://github.com/rmnldwg/lyscripts)
 [![build badge](https://github.com/rmnldwg/lyscripts/actions/workflows/build.yml/badge.svg?style=flat)](https://pypi.org/project/lyscripts/)
-[![docs badge](https://github.com/rmnldwg/lyscripts/actions/workflows/docs.yml/badge.svg?style=flat)](https://rmnldwg.github.io/lyscripts/)
+[![docs badge](https://readthedocs.org/projects/lyscripts/badge/?version=latest)](https://lyscripts.readthedocs.io/en/latest/?badge=latest)
 [![tests badge](https://github.com/rmnldwg/lyscripts/actions/workflows/tests.yml/badge.svg?style=flat)](https://rmnldwg.github.io/lyscripts/)
 
 
 ## What are these `lyscripts`?
 
 This package provides convenient scripts for performing inference and learning regarding the lymphatic spread of head & neck cancer. Essentially, it provides a *command line interface* (CLI) to the [lymph](https://github.com/rmnldwg/lymph) library.
```

### Comparing `lyscripts-1.0.0a1/docs/Makefile` & `lyscripts-1.0.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/docs/make.bat` & `lyscripts-1.0.0a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/docs/source/_static/favicon.png` & `lyscripts-1.0.0a2/docs/source/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/docs/source/_static/github-social-card.png` & `lyscripts-1.0.0a2/docs/source/_static/github-social-card.png`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/docs/source/conf.py` & `lyscripts-1.0.0a2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/favicon.png` & `lyscripts-1.0.0a2/favicon.png`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/github-social-card.png` & `lyscripts-1.0.0a2/github-social-card.png`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/__init__.py` & `lyscripts-1.0.0a2/lyscripts/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/app/__init__.py` & `lyscripts-1.0.0a2/lyscripts/app/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/app/prevalence.py` & `lyscripts-1.0.0a2/lyscripts/app/prevalence.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/compute/__init__.py` & `lyscripts-1.0.0a2/lyscripts/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/compute/__main__.py` & `lyscripts-1.0.0a2/lyscripts/compute/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/compute/posteriors.py` & `lyscripts-1.0.0a2/lyscripts/compute/posteriors.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/compute/prevalences.py` & `lyscripts-1.0.0a2/lyscripts/compute/prevalences.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,28 +110,32 @@
     ``mapping`` defines how the T-stages in the data are supposed to be mapped to the
     T-stages defined in the ``scenario``.
 
     Warning:
         When computing prevalences for unilateral models, the contralateral diagnosis
         will still be considered for computing the prevalence in the *data*.
     """
+    # when looking at the data, we always consider both sides
+    is_uni = scenario.is_uni
+    scenario.is_uni = False
+
     modality = get_modality_subset(scenario.diagnosis).pop()
     diagnosis_pattern = scenario.get_pattern(get_from="diagnosis", modality=modality)
 
+    # reset `is_uni` to the original value. Otherwise hash computation will fail.
+    scenario.is_uni = is_uni
+
     data.ly.map_t_stage(mapping)
     has_t_stage = data.ly.t_stage.isin(scenario.t_stages)
-    eligible_data = data.loc[has_t_stage].reset_index()
-
-    # filter the data by the involvement, which includes the involvement pattern itself
-    # and the midline extension status
-    has_midext = eligible_data.ly.is_midext(scenario.midext)
+    has_midext = data.ly.is_midext(scenario.midext)
+    eligible_data = data.loc[has_t_stage & has_midext].reset_index()
     does_pattern_match = eligible_data.ly.match(diagnosis_pattern, modality)
 
     try:
-        matching_data = eligible_data.loc[does_pattern_match & has_midext]
+        matching_data = eligible_data.loc[does_pattern_match]
         len_matching_data = len(matching_data)
     except KeyError:
         # return X, X if no actual pattern was selected
         len_matching_data = len(eligible_data)
 
     return len_matching_data, len(eligible_data)
 
@@ -184,32 +188,43 @@
             cache_hit_msg="Loaded computed priors.",
         )
     except ValueError as val_err:
         msg = "No computed priors found for the given scenario."
         logger.error(msg)
         raise ValueError(msg) from val_err
 
-    kwargs = {"midext": scenario.midext} if isinstance(model, models.Midline) else {}
+    is_midline = isinstance(model, models.Midline)
+    kwargs = {"midext": scenario.midext} if is_midline else {}
     prevalences = []
 
     for prior in track(
         sequence=priors,
         description="[blue]INFO     [/blue]" + progress_desc,
         total=len(priors),
     ):
         obs_dist = model.obs_dist(given_state_dist=prior)
         # marginalizing the distribution over observational states is not quite the
         # intended use of the method. But as long as exactly one modality is set in
         # the model, this should work as expected, because then the observation matrix
         # is square and the `obs_dist` has the same shape as the `state_dist`.
-        prevalences.append(model.marginalize(
+        prev = model.marginalize(
             involvement=diagnosis_pattern,
             given_state_dist=obs_dist,
             **kwargs,
-        ))
+        )
+        if is_midline:
+            # divide by the marginal likelihood of the midline extension status. This
+            # is necessary because although we trat midline extension as a random
+            # variable, it *is* part of a scenario.
+            prev /= model.marginalize(
+                involvement=None,
+                given_state_dist=obs_dist,
+                **kwargs,
+            )
+        prevalences.append(prev)
 
     prevalences = np.stack(prevalences)
     prevalences_cache[prevalences_hash] = (prevalences, scenario.as_dict("prevalences"))
     return prevalences
 
 
 def main(args: argparse.Namespace):
```

### Comparing `lyscripts-1.0.0a1/lyscripts/compute/priors.py` & `lyscripts-1.0.0a2/lyscripts/compute/priors.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/compute/risks.py` & `lyscripts-1.0.0a2/lyscripts/compute/risks.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/compute/utils.py` & `lyscripts-1.0.0a2/lyscripts/compute/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/data/__init__.py` & `lyscripts-1.0.0a2/lyscripts/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/data/__main__.py` & `lyscripts-1.0.0a2/lyscripts/data/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/data/accessor.py` & `lyscripts-1.0.0a2/lyscripts/data/accessor.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/data/enhance.py` & `lyscripts-1.0.0a2/lyscripts/data/enhance.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/data/filter.py` & `lyscripts-1.0.0a2/lyscripts/data/filter.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/data/generate.py` & `lyscripts-1.0.0a2/lyscripts/data/generate.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/data/join.py` & `lyscripts-1.0.0a2/lyscripts/data/join.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/data/lyproxify.py` & `lyscripts-1.0.0a2/lyscripts/data/lyproxify.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,31 +87,30 @@
 
 def clean_header(
     table: pd.DataFrame,
     num_cols: int,
     num_header_rows: int,
 ) -> pd.DataFrame:
     """Rename the header cells in the ``table``."""
+    table = table.copy()
+
     for col in range(num_cols):
         for row in range(num_header_rows):
             table.rename(
                 columns={f"Unnamed: {col}_level_{row}": f"{col}_lvl_{row}"},
                 inplace=True,
             )
     return table
 
 
 def get_instruction_depth(nested_column_map: dict[tuple, dict[str, Any]]) -> int:
-    """
-    Get the depth at which the column mapping instructions are nested.
+    """Get the depth at which the column mapping instructions are nested.
 
     Instructions are a dictionary that contains either a 'func' or 'default' key.
 
-    Example:
-
     >>> nested_column_map = {"patient": {"age": {"func": int}}}
     >>> get_instruction_depth(nested_column_map)
     2
     >>> flat_column_map = flatten(nested_column_map, max_depth=2)
     >>> get_instruction_depth(flat_column_map)
     1
     >>> nested_column_map = {"patient": {"__doc__": "some patient info", "age": 61}}
@@ -133,21 +132,19 @@
 
 
 def generate_markdown_docs(
     nested_column_map: dict[tuple, dict[str, Any]],
     depth: int = 0,
     indent_len: int = 4,
 ) -> str:
-    """
-    Generate a markdown nested, ordered list as documentation for the column map.
+    """Generate a markdown nested, ordered list as documentation for the column map.
 
     A key in the doctionary is supposed to be documented, when its value is a dictionary
     containing a ``"__doc__"`` key.
 
-    Example:
     >>> nested_column_map = {
     ...     "patient": {
     ...         "__doc__": "some patient info",
     ...         "age": {
     ...             "__doc__": "age of the patient",
     ...             "func": int,
     ...             "columns": ["age"],
@@ -172,16 +169,15 @@
 
 
 @log_state()
 def transform_to_lyprox(
     raw: pd.DataFrame,
     column_map: dict[tuple, dict[str, Any]]
 ) -> pd.DataFrame:
-    """
-    Transform ``raw`` data frame into table that can be uploaded directly to `LyProX`_.
+    """Transform ``raw`` data frame into table that can be uploaded directly to `LyProX`_.
 
     To do so, it uses instructions in the `colum_map` dictionary, that needs to have
     a particular structure:
 
     For each column in the final 'lyproxified' `pd.DataFrame`, one entry must exist in
     the `column_map` dctionary. E.g., for the column corresponding to a patient's age,
     the dictionary should contain a key-value pair of this shape:
@@ -241,16 +237,15 @@
                     "describing how to fill this column."
                 )
     return processed
 
 
 @log_state()
 def leftright_to_ipsicontra(data: pd.DataFrame):
-    """
-    Change absolute side reporting to tumor-relative.
+    """Change absolute side reporting to tumor-relative.
 
     Transform reporting of LNL involvement by absolute side (right & left) to a
     reporting relative to the tumor (ipsi- & contralateral). The table ``data`` should
     already be in the format LyProX requires, except for the side-reporting of LNL
     involvement.
     """
     len_before = len(data)
@@ -271,20 +266,19 @@
             )
     assert len_before == len(data), "Number of patients changed"
     return data
 
 
 @log_state()
 def exclude_patients(raw: pd.DataFrame, exclude: list[tuple[str, Any]]):
-    """
-    Exclude patients in the ``raw`` data based on a list of what to ``exclude``. This
-    list contains tuples ``(column, check)``. The ``check`` function will then exclude
-    any patients from the cohort where ``check(raw[column])`` evaluates to ``True``.
+    """Exclude patients in the ``raw`` data based on a list of what to ``exclude``.
 
-    Example:
+    The ``exclude`` list contains tuples ``(column, check)``. The ``check`` function
+    will then exclude any patients from the cohort where ``check(raw[column])``
+    evaluates to ``True``.
 
     >>> exclude = [("age", lambda s: s > 50)]
     >>> table = pd.DataFrame({
     ...     "age":        [43, 82, 18, 67],
     ...     "T-category": [ 3,  4,  2,  1],
     ... })
     >>> exclude_patients(table, exclude)
@@ -296,15 +290,15 @@
         exclude = check(raw[column])
         raw = raw.loc[~exclude]
     return raw
 
 
 def main(args: argparse.Namespace):
     """Run the lyproxify main function."""
-    raw: pd.DataFrame = load_patient_data(args.input)
+    raw: pd.DataFrame = load_patient_data(args.input, header=args.header_rows)
     raw = clean_header(raw, num_cols=raw.shape[1], num_header_rows=len(args.header_rows))
 
     cols_to_drop = raw.columns[args.drop_cols]
     trimmed = raw.drop(cols_to_drop, axis="columns")
     trimmed = trimmed.drop(index=args.drop_rows)
     trimmed = trimmed.dropna(axis="index", how="all")
     logger.info(f"Dropped rows {args.drop_rows} and columns {cols_to_drop}.")
```

### Comparing `lyscripts-1.0.0a1/lyscripts/data/split.py` & `lyscripts-1.0.0a2/lyscripts/data/split.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/decorators.py` & `lyscripts-1.0.0a2/lyscripts/decorators.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/evaluate.py` & `lyscripts-1.0.0a2/lyscripts/evaluate.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/plot/__init__.py` & `lyscripts-1.0.0a2/lyscripts/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/plot/__main__.py` & `lyscripts-1.0.0a2/lyscripts/plot/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/plot/corner.py` & `lyscripts-1.0.0a2/lyscripts/plot/corner.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/plot/histograms.py` & `lyscripts-1.0.0a2/lyscripts/plot/histograms.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/plot/thermo_int.py` & `lyscripts-1.0.0a2/lyscripts/plot/thermo_int.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/plot/utils.py` & `lyscripts-1.0.0a2/lyscripts/plot/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Utility functions for the plotting commands.
 """
 from dataclasses import dataclass, field
 from itertools import cycle
 from pathlib import Path
-from typing import Any
+from typing import Any, TypeVar
 
 import h5py
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy as sp
 from matplotlib.axes._axes import Axes as MPLAxes
 from matplotlib.figure import Figure
@@ -68,78 +68,100 @@
     if not filepath.exists():
         raise FileNotFoundError(
             f"File with the name {filename} does not exist at {filepath.resolve()}"
         )
     return filepath
 
 
+HistogramT = TypeVar("HistogramT", bound="Histogram")
+
 @dataclass
 class Histogram:
     """Class containing data for plotting a histogram."""
     values: np.ndarray
-    scale: float = field(default=100.)
+    scale: float = 100.
+    offset: float = 0.
     kwargs: dict[str, Any] = field(default_factory=lambda: {})
 
     def __post_init__(self) -> None:
-        self.values = self.scale * self.values
+        self.values = self.scale * self.values + self.offset
 
     @classmethod
-    def from_hdf5(cls, filename, dataname, scale: float = 100., **kwargs):
+    def from_hdf5(
+        cls: type[HistogramT],
+        filename: str | Path,
+        dataname: str,
+        scale: float = 100.,
+        offset: float = 0.,
+        **kwargs,
+    ) -> HistogramT:
         """Create a histogram from an HDF5 file."""
         filename = clean_and_check(filename)
         with h5py.File(filename, mode="r") as h5file:
             dataset = h5file[dataname]
             if "label" not in kwargs:
                 kwargs["label"] = get_label(dataset.attrs)
-            return cls(values=dataset[:], scale=scale, kwargs=kwargs)
+            return cls(values=dataset[:], scale=scale, offset=offset, kwargs=kwargs)
 
     def left_percentile(self, percent: float) -> float:
         """Compute the point where `percent` of the values are to the left."""
         return np.percentile(self.values, percent)
 
     def right_percentile(self, percent: float) -> float:
         """Compute the point where `percent` of the values are to the right."""
         return np.percentile(self.values, 100. - percent)
 
 
+BetaPosteriorT = TypeVar("BetaPosteriorT", bound="BetaPosterior")
+
 @dataclass
 class BetaPosterior:
     """Class for storing plot configs for a Beta posterior."""
     num_success: int
     num_total: int
-    scale: float = field(default=100.)
+    scale: float = 100.
+    offset: float = 0.
     kwargs: dict[str, Any] = field(default_factory=lambda: {})
 
     @classmethod
-    def from_hdf5(cls, filename, dataname, scale: float = 100., **kwargs) -> None:
+    def from_hdf5(
+        cls: type[BetaPosteriorT],
+        filename: str | Path,
+        dataname: str,
+        scale: float = 100.,
+        offset: float = 0.,
+        **kwargs,
+    ) -> BetaPosteriorT:
         """Initialize data container for Beta posteriors from HDF5 file."""
         filename = clean_and_check(filename)
         with h5py.File(filename, mode="r") as h5file:
             dataset = h5file[dataname]
             try:
                 num_success = int(dataset.attrs["num_match"])
                 num_total = int(dataset.attrs["num_total"])
             except KeyError as key_err:
                 raise KeyError(
                     "Dataset does not contain observed prevalence data"
                 ) from key_err
 
-        return cls(num_success, num_total, scale=scale, kwargs=kwargs)
+        return cls(num_success, num_total, scale=scale, offset=offset, kwargs=kwargs)
 
     @property
     def num_fail(self):
+        """Return the number of failures, i.e. the totals minus the successes."""
         return self.num_total - self.num_success
 
     def pdf(self, x: np.ndarray) -> np.ndarray:
         """Compute the probability density function."""
         return sp.stats.beta.pdf(
             x,
             a=self.num_success+1,
             b=self.num_fail+1,
-            scale=self.scale
+            loc=self.offset,
+            scale=self.scale,
         )
 
     def left_percentile(self, percent: float) -> float:
         """Return the point where the CDF reaches ``percent``."""
         return sp.stats.beta.ppf(
             percent / 100.,
             a=self.num_success+1,
@@ -154,23 +176,20 @@
             a=self.num_success+1,
             b=self.num_fail+1,
             scale=self.scale,
         )
 
 
 def get_size(width="single", unit="cm", ratio="golden"):
-    """
-    Return a tuple of figure sizes in inches.
+    """Return a tuple of figure sizes in inches.
 
     This is provided as the ``matplotlib`` keyword argument ``figsize`` expects it.
     This figure size is computed from a ``width``, in the ``unit`` of centimeters by
     default, and a ``ratio`` which is set to the golden ratio by default.
 
-    Examples:
-
     >>> get_size(width="single", ratio="golden")
     (3.937007874015748, 2.4332557935820445)
     >>> get_size(width="full", ratio=2.)
     (6.299212598425196, 3.149606299212598)
     >>> get_size(width=10., ratio=1.)
     (3.937007874015748, 3.937007874015748)
     >>> get_size(width=5, unit="inches", ratio=2./3.)
@@ -220,21 +239,20 @@
     right_lim = np.max(right_percentiles)
     return left_lim, right_lim
 
 
 def draw(
     axes: MPLAxes,
     contents: list[Histogram | BetaPosterior],
-    percent_lims: tuple[float] = (10., 10.),
+    percent_lims: tuple[float, float] = (10., 10.),
     xlims: tuple[float] | None = None,
     hist_kwargs: dict[str, Any] | None = None,
     plot_kwargs: dict[str, Any] | None = None,
 ) -> MPLAxes:
-    """
-    Draw histograms and Beta posterior from ``contents`` into ``axes``.
+    """Draw histograms and Beta posterior from ``contents`` into ``axes``.
 
     The limits of the x-axis is computed to be the smallest and largest left and right
     percentile of all provided ``contents`` respectively via the ``percent_lims`` tuple.
 
     The ``hist_kwargs`` define general settings that will be applied to all histograms.
     One additional key ``'nbins'`` may be used to adjust only the numbers, not the
     spacing of the histogram bins.
```

### Comparing `lyscripts-1.0.0a1/lyscripts/sample.py` & `lyscripts-1.0.0a2/lyscripts/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,23 @@
         sequence=sampler.sample(state, iterations=nsteps * thin, thin=thin, store=True),
         description="[blue]INFO     [/blue]Sampling phase",
         total=nsteps * thin,
     ):
         continue
 
 
+class DummyPool:
+    """Dummy class to allow for no multiprocessing."""
+    def __enter__(self):
+        return None
+
+    def __exit__(self, *args):
+        pass
+
+
 def main(args: argparse.Namespace) -> None:
     """Main function to run the MCMC sampling."""
     # as recommended in https://emcee.readthedocs.io/en/stable/tutorials/parallel/#
     os.environ["OMP_NUM_THREADS"] = "1"
 
     params = load_yaml_params(args.params)
     inference_data = load_patient_data(args.input)
@@ -257,15 +266,20 @@
     nwalkers = ndim * args.walkers_per_dim
 
     # emcee does not support numpy's new random number generator yet.
     np.random.seed(args.seed)
     hdf5_backend = initialize_backend(args.output, nwalkers, ndim)
     moves_mix = [(emcee.moves.DEMove(), 0.8), (emcee.moves.DESnookerMove(), 0.2)]
 
-    with Pool(args.cores) as pool:
+    if args.cores == 0:
+        real_or_dummy_pool = DummyPool()
+    else:
+        real_or_dummy_pool = Pool(args.cores)
+
+    with real_or_dummy_pool as pool:
         sampler = emcee.EnsembleSampler(
             nwalkers, ndim, log_prob_fn,
             moves=moves_mix,
             backend=hdf5_backend,
             pool=pool,
         )
         burnin_history = run_burnin(
```

### Comparing `lyscripts-1.0.0a1/lyscripts/scenario.py` & `lyscripts-1.0.0a2/lyscripts/scenario.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,66 +9,105 @@
 model) are relevant. But e.g. posteriors and risks also require us to provide a
 diagnosis, given which to compute the quantities of interest.
 """
 import argparse
 import hashlib
 import inspect
 from collections.abc import Iterable
+from dataclasses import dataclass, field, fields
 from typing import Any, Literal, TypeVar
 
 import numpy as np
 from lymph import types
 
 from lyscripts.utils import optional_bool
 
-ScenarioT = TypeVar("ScenarioT", bound="Scenario")
 
+class UninitializedProperty(Exception):
+    """Raise when a uninitialized property of a dataclass is accessed.
+
+    If a field of a dataclass is also a property, then the dataclass will call the
+    property's setter during ``__init__`` with the ``proprety`` object as the value
+    (at least if nothing is provided to the constructor).
+
+    Thus, I will not allow setting a ``propoerty`` as the value and raise this exception
+    in the getter when no private attribute is found.
+    """
+
+ScenarioT = TypeVar("ScenarioT", bound="Scenario")
 
+@dataclass
 class Scenario:
-    """Class for storing configuration of a scenario.
+    """Dataclass for storing configuration of a scenario.
 
     This may be used by the :py:mod:`.compute` and :py:mod:`.predict` modules to
     compute priors, posteriors, prevalences, and risks.
     """
-    def __init__(
-        self,
-        t_stages: list[int | str] | None = None,
-        t_stages_dist: Iterable[float] | None = None,
-        mode: Literal["BN", "HMM"] = "HMM",
-        midext: bool | None = None,
-        diagnosis: dict[str, dict[str, types.PatternType]] | None = None,
-        involvement: dict[str, types.PatternType] | None = None,
-        is_uni: bool = False,
-        side: str = "ipsi",
-    ) -> None:
-        """Initialize a scenario.
+    t_stages: list[int | str] = field(default_factory=lambda: ["early"])
+    t_stages_dist: list[float] | np.ndarray
+    mode: Literal["BN", "HMM"] = "HMM"
+    midext: bool | None = None
+    diagnosis: dict[str, dict[str, types.PatternType]]
+    involvement: dict[str, types.PatternType]
+    is_uni: bool = False
+    side: str = "ipsi"
+
 
-        If ``t_stages`` is set to ``None``, the scenario will be initialized with the
-        default value ``["early"]``.
+    @staticmethod
+    def _defaults(property_name: str) -> Any:
+        """Return the default value for a property.
+
+        >>> scenario = Scenario()
+        >>> scenario.t_stages_dist
+        array([1.])
+        >>> scenario.diagnosis
+        {'ipsi': {}, 'contra': {}}
+        >>> scenario = Scenario(is_uni=True)
+        >>> scenario.involvement
+        {}
+        """
+        return {
+            "t_stages_dist": np.array([1.]),
+            "involvement": {"ipsi": {}, "contra": {}},
+            "diagnosis": {"ipsi": {}, "contra": {}},
+        }[property_name]
+
+
+    def __post_init__(self) -> None:
+        """Declate default value of properties.
+
+        >>> scenario = Scenario(t_stages=['a', 'b'], t_stages_dist=[0.1, 0.9])
+        >>> scenario.t_stages_dist
+        array([0.1, 0.9])
         """
-        self.t_stages = t_stages or ["early"]
-        self.t_stages_dist = t_stages_dist
-        self.mode = mode
-        self.midext = midext
-        self._diagnosis = diagnosis or {}
-        self._involvement = involvement or {}
-        self.is_uni = is_uni
-        self.side = side
+        for field in fields(self):
+            try:
+                _ = getattr(self, field.name)
+            except UninitializedProperty:
+                default = self._defaults(field.name)
+                setattr(self, field.name, default)
+
+        if not self.is_uni:
+            for side in ["ipsi", "contra"]:
+                if not side in self.diagnosis:
+                    self.diagnosis[side] = {}
+                if not side in self.involvement:
+                    self.involvement[side] = {}
 
 
     @classmethod
     def fields(cls) -> dict[str, Any]:
         """Return a list of fields that may make up a scenario."""
         params = inspect.signature(cls).parameters
         res = {}
-        for field, param in params.items():
+        for f, param in params.items():
             if param.default == inspect.Parameter.empty:
-                res[field] = None
+                res[f] = None
             else:
-                res[field] = param.default
+                res[f] = param.default
         return res
 
     @property
     def t_stages_dist(self) -> np.ndarray:
         """Distribution over T-stages. If not set, return uniform distribution.
 
         This will also interpolate the distribution if the number of T-stages has
@@ -81,28 +120,34 @@
         >>> scenario.t_stages_dist = [0.1, 0.2, 0.7]
         >>> scenario.t_stages_dist
         array([0.1, 0.2, 0.7])
         >>> scenario.t_stages = ["early", "late"]
         >>> scenario.t_stages_dist
         array([0.125, 0.875])
         """
+        if not hasattr(self, "_t_stages_dist"):
+            raise UninitializedProperty("t_stages_dist")
+
         if self._t_stages_dist is None:
-            return np.ones(len(self.t_stages)) / len(self.t_stages)
+            self._t_stages_dist = self._defaults("t_stages_dist")
 
         if len(self._t_stages_dist) != len(self.t_stages):
             new_x = np.linspace(0., 1., len(self.t_stages))
             old_x = np.linspace(0., 1., len(self._t_stages_dist))
             self._t_stages_dist = np.interp(new_x, old_x, self._t_stages_dist)
-            self._t_stages_dist /= self._t_stages_dist.sum()
+
+        if not np.isclose(np.sum(self._t_stages_dist), 1.):
+            self._t_stages_dist /= np.sum(self._t_stages_dist)
 
         return np.array(self._t_stages_dist)
 
     @t_stages_dist.setter
     def t_stages_dist(self, value: Iterable[float]) -> None:
-        self._t_stages_dist = value
+        if not isinstance(value, property):
+            self._t_stages_dist = value
 
 
     @classmethod
     def from_namespace(
         cls,
         namespace: argparse.Namespace,
         lnls: list[str] | None = None,
@@ -134,24 +179,49 @@
         kwargs["is_uni"] = is_uni
         kwargs["side"] = side
         scenario = cls(**kwargs)
 
         for side in ["ipsi", "contra"]:
             pattern = getattr(namespace, f"{side}_involvement", None) or [None] * len(lnls)
             tmp = {lnl: val for lnl, val in zip(lnls, pattern)}
-            getattr(scenario, "involvement")[side] = tmp
+            scenario._involvement[side] = tmp
 
             pattern = getattr(namespace, f"{side}_diagnosis", None) or [None] * len(lnls)
             tmp = {lnl: val for lnl, val in zip(lnls, pattern)}
             mod_name = getattr(namespace, "modality", "max_llh")
-            getattr(scenario, "diagnosis")[side] = {mod_name: tmp}
+            scenario._diagnosis[side] = {mod_name: tmp}
 
         return scenario
 
     @classmethod
+    def from_dict(
+        cls,
+        data: dict[str, Any],
+        **kwargs,
+    ) -> ScenarioT:
+        """Create a scenario from a dictionary.
+
+        >>> data = {
+        ...     "t_stages": ["early"],
+        ...     "mode": "BN",
+        ...     "diagnosis": {"ipsi": {"max_llh": {"II": True, "III": False}}},
+        ... }
+        >>> scenario = Scenario.from_dict(data)
+        >>> scenario.t_stages, scenario.mode
+        (['early'], 'BN')
+        >>> scenario.diagnosis
+        {'ipsi': {'max_llh': {'II': True, 'III': False}}, 'contra': {}}
+        """
+        init_kwargs = {
+            field: kwargs.get(field, data.get(field, value))
+            for field, value in cls.fields().items()
+        }
+        return cls(**init_kwargs)
+
+    @classmethod
     def list_from_params(
         cls,
         params: dict[str, Any],
         is_uni: bool = False,
         side: str = "ipsi",
     ) -> list[ScenarioT]:
         """Create scenarios from a dictionary of parameters.
@@ -167,40 +237,19 @@
         ['early'] BN
         ['late'] HMM
         """
         res = []
         uni_side_kwargs = {"is_uni": is_uni, "side": side}
         scenarios = params.get("scenarios", [])
         for scenario in scenarios:
-            kwargs = {
-                field: scenario.get(field, value)
-                for field, value in cls.fields().items()
-            }
-            kwargs.update(uni_side_kwargs)
-            res.append(cls(**kwargs))
+            res.append(cls.from_dict(scenario, **uni_side_kwargs))
 
         return res
 
 
-    def for_side(self, side: Literal["ipsi", "contra"]) -> ScenarioT:
-        """Return the side-specific part of the scenario.
-
-        >>> scenario = Scenario(involvement={"ipsi": {"II": True}})
-        >>> scenario.involvement
-        {'ipsi': {'II': True}}
-        >>> scenario.for_side("ipsi").involvement
-        {'II': True}
-        """
-        cls = type(self)
-        kwargs = {field: getattr(self, field) for field in cls.fields()}
-        kwargs["involvement"] = kwargs["involvement"].get(side, {})
-        kwargs["diagnosis"] = kwargs["diagnosis"].get(side, {})
-        return cls(**kwargs)
-
-
     def as_dict(
         self,
         for_comp: Literal["priors", "posteriors", "prevalences", "risks"],
     ) -> dict[str, Any]:
         """Return dict that may be used as keyword arguments for computing priors."""
         res = {
             "mode": self.mode,
@@ -208,59 +257,75 @@
             "t_stages_dist": self.t_stages_dist,
         }
         if for_comp == "priors":
             return res
 
         res.update({
             "midext": self.midext,
-            "diagnosis": self._diagnosis,
+            "diagnosis": self.diagnosis,
             "side": self.side,
             "is_uni": self.is_uni,
         })
 
         if for_comp == "risks":
-            res["involvement"] = self._involvement
+            res["involvement"] = self.involvement
 
         return res
 
 
     @property
     def diagnosis(self) -> dict[str, dict[str, types.PatternType]] | dict[str, types.PatternType]:
         """Get bi- or unilateral diagosis, depending on attrs ``side`` and ``is_uni``."""
+        if not hasattr(self, "_diagnosis"):
+            raise UninitializedProperty("diagnosis")
+
         if self.is_uni:
             return self._diagnosis[self.side]
 
         return self._diagnosis
 
+    @diagnosis.setter
+    def diagnosis(self, value: dict[str, dict[str, types.PatternType]]) -> None:
+        if not isinstance(value, property):
+            self._diagnosis = value
+
 
     @property
     def involvement(self) -> dict[str, types.PatternType] | types.PatternType:
         """Get bi- or unilateral involvement, depending on attrs ``side`` and ``is_uni``."""
+        if not hasattr(self, "_involvement"):
+            raise UninitializedProperty("involvement")
+
         if self.is_uni:
             return self._involvement[self.side]
 
         return self._involvement
 
+    @involvement.setter
+    def involvement(self, value: dict[str, types.PatternType]) -> None:
+        if not isinstance(value, property):
+            self._involvement = value
+
 
     def get_pattern(
         self,
         get_from: Literal["involvement", "diagnosis"],
         modality: str,
     ) -> dict[str, Any]:
         """Get an involvement pattern for the given ``modality``."""
         if get_from == "involvement":
             pattern = self._involvement
         else:
             pattern = {
-                side: self._diagnosis[side][modality]
+                side: self._diagnosis.get(side, {}).get(modality, {})
                 for side in ["ipsi", "contra"]
             }
 
         if self.is_uni:
-            return pattern[self.side]
+            return pattern.get(self.side, {})
 
         return pattern
 
 
     def md5_hash(
         self,
         for_comp: Literal["priors", "posteriors", "prevalences", "risks"],
@@ -270,15 +335,15 @@
 
         >>> scenario = Scenario(t_stages=["early"], mode="BN")
         >>> scenario.as_dict("priors")
         {'mode': 'BN', 't_stages': ['early'], 't_stages_dist': array([1.])}
         >>> scenario.md5_hash("priors")
         '49f9cb'
         >>> scenario.md5_hash("posteriors", length=12)
-        '2cd686a7fbad'
+        '1194fd880d47'
         """
         full_hash = hashlib.md5(str(self.as_dict(for_comp)).encode("utf-8")).hexdigest()
         return full_hash[:length]
 
 
 def add_scenario_arguments(
     parser: argparse.ArgumentParser,
@@ -353,9 +418,10 @@
     parser.add_argument(
         "--contra-diagnosis", nargs="+", type=optional_bool,
         help="Diagnosis of contralateral side.",
     )
 
 
 if __name__ == "__main__":
+    scenario = Scenario(t_stages=['a', 'b'], t_stages_dist=[0.2, 0.8])
     import doctest
     doctest.testmod()
```

### Comparing `lyscripts-1.0.0a1/lyscripts/temp_schedule.py` & `lyscripts-1.0.0a2/lyscripts/temp_schedule.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts/utils.py` & `lyscripts-1.0.0a2/lyscripts/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/lyscripts.egg-info/PKG-INFO` & `lyscripts-1.0.0a2/lyscripts.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyscripts
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Package containing scripts used in lynference pipelines
 Author-email: Roman Ludwig <roman.ludwig@usz.ch>
 License: MIT
 Project-URL: source, https://github.com/rmnldwg/lyscripts
 Project-URL: documentation, https://rmnldwg.github.io/lyscripts
 Keywords: scripts,lymph,inference
 Classifier: Programming Language :: Python :: 3
@@ -43,15 +43,15 @@
 Requires-Dist: streamlit; extra == "apps"
 
 <img src="https://raw.githubusercontent.com/rmnldwg/lyscripts/main/github-social-card.png" alt="social card" style="width:830px;"/>
 
 [![MIT license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/rmnldwg/lyscripts/blob/main/LICENSE)
 [![GitHub repo](https://img.shields.io/badge/rmnldwg%2Flymph-grey.svg?style=flat&logo=github)](https://github.com/rmnldwg/lyscripts)
 [![build badge](https://github.com/rmnldwg/lyscripts/actions/workflows/build.yml/badge.svg?style=flat)](https://pypi.org/project/lyscripts/)
-[![docs badge](https://github.com/rmnldwg/lyscripts/actions/workflows/docs.yml/badge.svg?style=flat)](https://rmnldwg.github.io/lyscripts/)
+[![docs badge](https://readthedocs.org/projects/lyscripts/badge/?version=latest)](https://lyscripts.readthedocs.io/en/latest/?badge=latest)
 [![tests badge](https://github.com/rmnldwg/lyscripts/actions/workflows/tests.yml/badge.svg?style=flat)](https://rmnldwg.github.io/lyscripts/)
 
 
 ## What are these `lyscripts`?
 
 This package provides convenient scripts for performing inference and learning regarding the lymphatic spread of head & neck cancer. Essentially, it provides a *command line interface* (CLI) to the [lymph](https://github.com/rmnldwg/lymph) library.
```

### Comparing `lyscripts-1.0.0a1/lyscripts.egg-info/SOURCES.txt` & `lyscripts-1.0.0a2/lyscripts.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 lyscripts/data/utils.py
 lyscripts/plot/__init__.py
 lyscripts/plot/__main__.py
 lyscripts/plot/corner.py
 lyscripts/plot/histograms.py
 lyscripts/plot/thermo_int.py
 lyscripts/plot/utils.py
+tests/__init__.py
 tests/run_doctests.py
 tests/sample_test.py
 tests/test.yaml
 tests/test_backend.hdf5
 tests/test_data.csv
 tests/test_params_v0.yaml
 tests/test_params_v1.yaml
```

### Comparing `lyscripts-1.0.0a1/pyproject.toml` & `lyscripts-1.0.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 [tool.setuptools_scm]
 write_to = "lyscripts/_version.py"
 local_scheme = "no-local-version"
 
 [tool.setuptools.dynamic]
 version = {attr = "lyscripts._version.version"}
 
+[tool.pytest.ini_options]
+testpaths = "."
+
 [tool.isort]
 line_length = 79
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
```

### Comparing `lyscripts-1.0.0a1/tests/data/join_test.py` & `lyscripts-1.0.0a2/tests/data/join_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/plot/baseline/sine.png` & `lyscripts-1.0.0a2/tests/plot/baseline/sine.png`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/plot/baseline/sine.svg` & `lyscripts-1.0.0a2/tests/plot/baseline/sine.svg`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/plot/baseline/sine_svg.png` & `lyscripts-1.0.0a2/tests/plot/baseline/sine_svg.png`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/plot/baseline/test_draw.png` & `lyscripts-1.0.0a2/tests/plot/baseline/test_draw.png`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/plot/data/beta_samples.hdf5` & `lyscripts-1.0.0a2/tests/plot/data/beta_samples.hdf5`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/plot/plot_utils_test.py` & `lyscripts-1.0.0a2/tests/plot/plot_utils_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -86,14 +86,48 @@
         "Label extraction did not work"
     )
     assert hist_from_path.kwargs["label"] == custom_label, (
         "Keyword override did not work"
     )
 
 
+def test_inverted_histogram_cls(beta_samples):
+    """Make sure the histogram data container works as intended."""
+    str_filename = beta_samples
+    path_filename = Path(str_filename)
+    custom_label = "Lorem ipsum"
+
+    hist_from_str = Histogram.from_hdf5(filename=str_filename, dataname="beta")
+    hist_from_path = Histogram.from_hdf5(
+        filename=path_filename,
+        dataname="beta",
+        scale=-100.,
+        offset=100.,
+        label=custom_label,
+    )
+
+    assert np.all(np.isclose(100. - hist_from_str.values, hist_from_path.values)), (
+        "Scaling and offsetting of data does not work correclty"
+    )
+    assert np.all(np.isclose(
+        hist_from_str.left_percentile(50.),
+        hist_from_str.right_percentile(50.),
+    )), "50% percentiles should be the same from the left and from the right."
+    assert np.all(np.isclose(
+        hist_from_path.left_percentile(10.),
+        hist_from_path.right_percentile(90.),
+    )), "10% from the left is not the same as 90% from the right"
+    assert hist_from_str.kwargs["label"] == "beta | mega scan | 100 | ext", (
+        "Label extraction did not work"
+    )
+    assert hist_from_path.kwargs["label"] == custom_label, (
+        "Keyword override did not work"
+    )
+
+
 def test_posterior_cls(beta_samples):
     """Test the container class for Beta posteriors."""
     str_filename = beta_samples
     path_filename = Path(str_filename)
     non_existent_filename = "non_existent.hdf5"
     custom_label = "Lorem ipsum"
     x_10 = np.linspace(0., 10., 100)
```

### Comparing `lyscripts-1.0.0a1/tests/predict/predict_utils_test.py` & `lyscripts-1.0.0a2/tests/predict/predict_utils_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/predict/prevalences_test.py` & `lyscripts-1.0.0a2/tests/predict/prevalences_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/sample_test.py` & `lyscripts-1.0.0a2/tests/sample_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/test_backend.hdf5` & `lyscripts-1.0.0a2/tests/test_backend.hdf5`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/test_params_v0.yaml` & `lyscripts-1.0.0a2/tests/test_params_v0.yaml`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/test_params_v1.yaml` & `lyscripts-1.0.0a2/tests/test_params_v1.yaml`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/test_sample_params.yaml` & `lyscripts-1.0.0a2/tests/test_sample_params.yaml`

 * *Files identical despite different names*

### Comparing `lyscripts-1.0.0a1/tests/utils_test.py` & `lyscripts-1.0.0a2/tests/utils_test.py`

 * *Files identical despite different names*

