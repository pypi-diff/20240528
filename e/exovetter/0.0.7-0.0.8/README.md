# Comparing `tmp/exovetter-0.0.7.tar.gz` & `tmp/exovetter-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exovetter-0.0.7.tar", last modified: Mon May  6 22:56:01 2024, max compression
+gzip compressed data, was "exovetter-0.0.8.tar", last modified: Tue May 28 16:43:03 2024, max compression
```

## Comparing `exovetter-0.0.7.tar` & `exovetter-0.0.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.105566 exovetter-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 22:55:52.000000 exovetter-0.0.7/.bandit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.085566 exovetter-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.089566 exovetter-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-06 22:55:52.000000 exovetter-0.0.7/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-06 22:55:52.000000 exovetter-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-06 22:55:52.000000 exovetter-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-06 22:55:52.000000 exovetter-0.0.7/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 22:55:52.000000 exovetter-0.0.7/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-06 22:55:52.000000 exovetter-0.0.7/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 22:55:52.000000 exovetter-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-06 22:56:01.105566 exovetter-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-06 22:55:52.000000 exovetter-0.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.089566 exovetter-0.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/vetters.rst
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-06 22:55:52.000000 exovetter-0.0.7/docs/vetters_low_level.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.093566 exovetter-0.0.7/exovetter/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.097566 exovetter-0.0.7/exovetter/centroid/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/centroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/centroid/centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/centroid/covar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/centroid/disp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/centroid/fastpsffit.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/leo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/lightkurve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/lpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.097566 exovetter-0.0.7/exovetter/modshift/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/modshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/modshift/modshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/modshift/plotmodshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/odd_even.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/sweet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/tce.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/transit_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)    31097 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/trapezoid_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    24909 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-06 22:56:00.000000 exovetter-0.0.7/exovetter/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    37423 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/vetters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-06 22:55:52.000000 exovetter-0.0.7/exovetter/viz_transits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.105566 exovetter-0.0.7/exovetter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-06 22:56:01.000000 exovetter-0.0.7/exovetter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-06 22:56:01.000000 exovetter-0.0.7/exovetter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:56:01.000000 exovetter-0.0.7/exovetter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 22:56:01.000000 exovetter-0.0.7/exovetter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-06 22:56:01.000000 exovetter-0.0.7/exovetter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 22:56:01.000000 exovetter-0.0.7/exovetter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.097566 exovetter-0.0.7/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-06 22:55:52.000000 exovetter-0.0.7/licenses/DAVE_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-06 22:55:52.000000 exovetter-0.0.7/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-06 22:55:52.000000 exovetter-0.0.7/licenses/TEMPLATE_LICENCE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-06 22:55:52.000000 exovetter-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-06 22:55:52.000000 exovetter-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-06 22:56:01.105566 exovetter-0.0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1958 2024-05-06 22:55:52.000000 exovetter-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 22:56:01.105566 exovetter-0.0.7/tutorial_notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)  1714508 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/100100827.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   278575 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/Centroid.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   160061 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/LPP.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    70192 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/LeoTransitEvents.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   219164 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/OddEven.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   251796 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/SWEET.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/TCEs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   131489 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/TransitPhaseCoverage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   224308 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/VizTransits.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   241212 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/lightcurves.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   235866 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/modshift.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    86880 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/run_all.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   740160 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/wasp18b.fits
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-06 22:55:52.000000 exovetter-0.0.7/tutorial_notebooks/wasp18b_tce
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:43:03.599061 exovetter-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 16:42:51.000000 exovetter-0.0.8/.bandit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:43:03.579061 exovetter-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:43:03.583061 exovetter-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-28 16:42:51.000000 exovetter-0.0.8/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-28 16:42:51.000000 exovetter-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-28 16:42:51.000000 exovetter-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-28 16:42:51.000000 exovetter-0.0.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 16:42:51.000000 exovetter-0.0.8/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-28 16:42:51.000000 exovetter-0.0.8/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-28 16:42:51.000000 exovetter-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-28 16:43:03.599061 exovetter-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-28 16:42:51.000000 exovetter-0.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:43:03.583061 exovetter-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-28 16:42:51.000000 exovetter-0.0.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-05-28 16:42:51.000000 exovetter-0.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 16:42:51.000000 exovetter-0.0.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 16:42:51.000000 exovetter-0.0.8/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-28 16:42:51.000000 exovetter-0.0.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-28 16:42:51.000000 exovetter-0.0.8/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 16:42:51.000000 exovetter-0.0.8/docs/vetters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-28 16:42:51.000000 exovetter-0.0.8/docs/vetters_low_level.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:43:03.587061 exovetter-0.0.8/exovetter/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:43:03.587061 exovetter-0.0.8/exovetter/centroid/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/centroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/centroid/centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/centroid/covar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/centroid/disp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/centroid/fastpsffit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/leo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/lightkurve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/lpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:43:03.587061 exovetter-0.0.8/exovetter/modshift/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/modshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/modshift/modshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/modshift/plotmodshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/odd_even.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/sweet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/tce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/transit_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31097 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/trapezoid_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24909 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 16:43:03.000000 exovetter-0.0.8/exovetter/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37732 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/vetters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-28 16:42:51.000000 exovetter-0.0.8/exovetter/viz_transits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:43:03.595061 exovetter-0.0.8/exovetter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-28 16:43:03.000000 exovetter-0.0.8/exovetter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-28 16:43:03.000000 exovetter-0.0.8/exovetter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:43:03.000000 exovetter-0.0.8/exovetter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:43:03.000000 exovetter-0.0.8/exovetter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-28 16:43:03.000000 exovetter-0.0.8/exovetter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 16:43:03.000000 exovetter-0.0.8/exovetter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:43:03.587061 exovetter-0.0.8/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-28 16:42:51.000000 exovetter-0.0.8/licenses/DAVE_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 16:42:51.000000 exovetter-0.0.8/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-28 16:42:51.000000 exovetter-0.0.8/licenses/TEMPLATE_LICENCE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 16:42:51.000000 exovetter-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 16:42:51.000000 exovetter-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-28 16:43:03.599061 exovetter-0.0.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1958 2024-05-28 16:42:51.000000 exovetter-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:43:03.595061 exovetter-0.0.8/tutorial_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)  1714508 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/100100827.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   582653 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/Centroid.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   160061 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/LPP.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    70192 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/LeoTransitEvents.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   219164 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/OddEven.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   251796 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/SWEET.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/TCEs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   131489 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/TransitPhaseCoverage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   224308 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/VizTransits.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   241212 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/lightcurves.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   235866 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/modshift.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    86880 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/run_all.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   740160 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/wasp18b.fits
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 16:42:52.000000 exovetter-0.0.8/tutorial_notebooks/wasp18b_tce
```

### Comparing `exovetter-0.0.7/.github/workflows/ci_workflows.yml` & `exovetter-0.0.8/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/.github/workflows/publish.yml` & `exovetter-0.0.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/.gitignore` & `exovetter-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/.readthedocs.yml` & `exovetter-0.0.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/LICENSE.rst` & `exovetter-0.0.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/PKG-INFO` & `exovetter-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exovetter
-Version: 0.0.7
+Version: 0.0.8
 Summary: Exoplanet vetting package
 Home-page: https://github.com/spacetelescope/exovetter
 Author: Susan Mullally et al.
 Author-email: smullally@stsci.edu
 License: BSD 3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `exovetter-0.0.7/README.rst` & `exovetter-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/docs/Makefile` & `exovetter-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/docs/conf.py` & `exovetter-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/docs/install.rst` & `exovetter-0.0.8/docs/install.rst`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/docs/make.bat` & `exovetter-0.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/docs/vetters_low_level.rst` & `exovetter-0.0.8/docs/vetters_low_level.rst`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/centroid/centroid.py` & `exovetter-0.0.8/exovetter/centroid/centroid.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         time, 
         cube, 
         period_days, 
         epoch, 
         duration_days,
         remove_transits, 
         max_oot_shift_pix=1.5,
+        starloc_pix = None,
         plot=False
 ):
     """Compute difference image centroid shifts for every transit in a dataset.
 
     Given a data cube containing a time-series of images, and a transit
     defined by a period, epoch and duration, compute centroid shift
     between in- and out-of- transit images for each transit covered by
@@ -38,14 +39,17 @@
         (float) Orbital period of transit.
     epoch
         (float) Epoch of transit centre in the same time system as `time`.
     duration_days
         (float) Duration of transit. 
     remove_transits
         (list) List of 0 indexed transit integers to not calculate on.
+    starloc_pix
+        (2d array) catalog location of target star for plotting.
+        Default is None.
     max_oot_shift_pix
         (float) Passed to `fastpsffit.fastGaussianPrfFit()
 
     Returns
     ---------------
     A 2d numpy array. Each row represents a single transit event.
     The columns are
@@ -70,37 +74,38 @@
     isnan = np.isnan(time)
     time = time[~isnan]
     cube = cube[~isnan]
 
     transits = getIngressEgressCadences(
         time, period_days, epoch, duration_days)
 
-    figs = []
+    axs = []
     centroids = []
 
     for i in range(len(transits)):
         if i not in remove_transits:
             cin = transits[i]
-            cents, fig = measure_centroids(
+            cents, ax = measure_centroids(
                 cube, 
                 cin, 
                 max_oot_shift_pix=max_oot_shift_pix,
+                starloc_pix = starloc_pix,
                 plot=plot
             )
 
             if plot == True:
-                fig.suptitle('Transit '+str(i))
+                plt.gcf().suptitle('Transit '+str(i))
 
             centroids.append(cents)
-            figs.append(fig)
+            axs.append(ax)
             
     centroids = np.array(centroids)
     all_transits = list(np.arange(len(transits)))
     kept_transits = [x for x in all_transits if x not in remove_transits]
-    return centroids, figs, kept_transits
+    return centroids, axs, kept_transits
 
 
 def measure_centroid_shift(centroids, kept_transits, plot=False):
     """Measure the average offset of the DIC centroids from the OOT centroids.
 
     Inputs
     ----------
@@ -136,26 +141,71 @@
         dcol[~flags], drow[~flags])
 
     fig = None
     if plot:
         fig = covar.diagnostic_plot(dcol, drow, kept_transits, flags)
     return offset_pix, signif, fig
 
+def measure_centroid_shift_cat(centroids, kept_transits, starloc_pix, plot=False):
+    """Measure the average offset of the DIC centroids from the catalog position.
+
+    Inputs
+    ----------
+    centroids
+        (2d np array) Output of :func:`compute_diff_image_centroids`
+
+    kept_transits
+        (list) List of 0 indexed transit integers to calculate on.
+    
+    starloc_pix
+        (2d np array) col,row expected location of target star
+
+    Returns
+    -----------
+    offset
+        (float) Size of offset in pixels (or whatever unit `centroids`
+        is in)
+    signif
+        (float) The statistical significance of the transit. Values
+        close to 1 mean the transit is likely on the target star.
+        Values less than ~1e-3 suggest the target is not the
+        source of the transit.
+    fig
+        A figure handle. Is **None** if plot is **False**
+    """
+
+    # DIC - catalog
+    # dcol = centroids[:, 5] - centroids[:, 0]
+    # drow = centroids[:, 4] - centroids[:, 1]
+    dcol = centroids[:, 4] - starloc_pix[0]
+    drow = centroids[:, 5] - starloc_pix[1]
+
+    flags = centroids[:, -1].astype(bool)
+
+    offset_pix, signif = covar.compute_offset_and_signif(
+        dcol[~flags], drow[~flags])
+
+    fig = None
+    if plot:
+        fig = covar.diagnostic_plot(dcol, drow, kept_transits, flags)
+        
+    return offset_pix, signif, fig
+
 
 def getIngressEgressCadences(time, period_days, epoch_btjd, duration_days):
     assert np.all(np.isfinite(time))
 
     idx = utils.mark_transit_cadences(
         time, period_days, epoch_btjd, duration_days)
     transits = np.array(utils.plateau(idx, 0.5))
 
     return transits
 
 
-def measure_centroids(cube, cin, max_oot_shift_pix=0.5, plot=False):
+def measure_centroids(cube, cin, max_oot_shift_pix=0.5, starloc_pix = None, plot=False):
     """Private function of :func:`compute_diff_image_centroids`
 
     Computes OOT, ITR and diff images for a single transit event,
     and computes image centroid by fitting a Gaussian.
 
     Inputs
     ---------
@@ -205,25 +255,39 @@
         print("WARN: Not all fits converged for [%i, %i]" % (cin[0], cin[1]))
 
     if plot:
         clr = "orange"
         if diffSoln.success:
             clr = "green"
 
-        res = diffSoln.x
-        disp.plotCentroidLocation(res[0], res[1], marker="^", color=clr,
-                                  label="diff")
+        fig = plt.gcf()
+        axlist = fig.axes 
+        #assert len(axlist) == 3, axlist
 
-        res = ootSoln.x
-        disp.plotCentroidLocation(res[0], res[1], marker="o", color=clr,
-                                  label="OOT")
-
-        res = intransSoln.x
-        disp.plotCentroidLocation(res[0], res[1], marker="+", color=clr,
-                                  label="InT")
+        res = diffSoln.x
+        for ax in axlist:
+            if ax.get_label() == '<colorbar>':
+                continue
+
+            plt.sca(ax)
+            disp.plotCentroidLocation(res[0], res[1], marker="^", color=clr,
+                                    label="diff")
+
+            res1 = ootSoln.x
+            disp.plotCentroidLocation(res1[0], res1[1], marker="o", color=clr,
+                                    label="OOT")
+
+            res2 = intransSoln.x
+            disp.plotCentroidLocation(res2[0], res2[1], marker="+", color=clr,
+                                    label="InT")
+            
+            if starloc_pix is not None:
+                disp.plotCentroidLocation(starloc_pix[0], starloc_pix[1], marker="*",
+                                        color='red', label="Cat", ms=10)
+            
         plt.legend(fontsize=12, framealpha=0.7, facecolor='silver')
 
     out = []
     out.extend(ootSoln.x[:2])
     out.extend(intransSoln.x[:2])
     out.extend(diffSoln.x[:2])
     flag = 0
@@ -232,27 +296,29 @@
     if diffSoln.x[3] < 4 * np.median(diff):
         flag = 2
     out.append(flag)
 
     return out, ax
 
 
-def generateDiffImg(cube, transits, plot=False):
+def generateDiffImg(cube, transits, starloc_pix = None, plot=False):
     """Generate a difference image.
 
     Also generates an image for each the $n$ cadedences before
     and after the transit,
     where $n$ is the number of cadences of the transit itself
 
     Inputs
     ------------
     cube
         (np 3 array) Datacube of postage stamps
     transits
         (2-tuples) Indices of the first and last cadence
+    starloc_pix
+        (np 2 element array) col, row position of star
 
     Optional Inputs
     -----------------
     plot
         (Bool) If true, generate a diagnostic plot
 
 
@@ -282,14 +348,15 @@
     oot = 0.5 * (before + after)
     diff = oot - during
 
     if plot:
         fig = plt.figure()
         fig.set_size_inches(16, 4)
         disp.plotTransit(fig, oot, during, diff)
+
     else:
         fig = None
 
     return oot, during, diff, fig
 
 
 def pickInitialGuess(img):
```

### Comparing `exovetter-0.0.7/exovetter/centroid/covar.py` & `exovetter-0.0.8/exovetter/centroid/covar.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/centroid/disp.py` & `exovetter-0.0.8/exovetter/centroid/disp.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import matplotlib.colors as mcolor
 import matplotlib.pyplot as plt
 import numpy as np
 
 
 def plotTransit(fig, oot, during, diff, **kwargs):
 
-    fig.add_subplot(131)
+    ax1 = fig.add_subplot(131)
     plotImage(oot, **kwargs)
     plt.title("OOT")
 
-    fig.add_subplot(132)
+    ax2 = fig.add_subplot(132)
     plotImage(during, **kwargs)
     plt.title("In-transit")
 
-    fig.add_subplot(133)
+    ax3 = fig.add_subplot(133)
     plotDiffImage(diff, **kwargs)
     plt.title("Difference")
 
 
 def plotImage(img, **kwargs):
     """Plot an image in linear scale
```

### Comparing `exovetter-0.0.7/exovetter/centroid/fastpsffit.py` & `exovetter-0.0.8/exovetter/centroid/fastpsffit.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/const.py` & `exovetter-0.0.8/exovetter/const.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/leo.py` & `exovetter-0.0.8/exovetter/leo.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/lightkurve_utils.py` & `exovetter-0.0.8/exovetter/lightkurve_utils.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/lpp.py` & `exovetter-0.0.8/exovetter/lpp.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/model.py` & `exovetter-0.0.8/exovetter/model.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/modshift/modshift.py` & `exovetter-0.0.8/exovetter/modshift/modshift.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/modshift/plotmodshift.py` & `exovetter-0.0.8/exovetter/modshift/plotmodshift.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/odd_even.py` & `exovetter-0.0.8/exovetter/odd_even.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/sweet.py` & `exovetter-0.0.8/exovetter/sweet.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/tce.py` & `exovetter-0.0.8/exovetter/tce.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/transit_coverage.py` & `exovetter-0.0.8/exovetter/transit_coverage.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/trapezoid_fit.py` & `exovetter-0.0.8/exovetter/trapezoid_fit.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/utils.py` & `exovetter-0.0.8/exovetter/utils.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter/vetters.py` & `exovetter-0.0.8/exovetter/vetters.py`

 * *Files 1% similar despite different names*

```diff
@@ -581,15 +581,15 @@
     def plot(self):  # pragma: no cover
         self.run(self.tce, self.lc, plot=True)
 
 
 class Centroid(BaseVetter):
     """Class to handle centroid vetting"""
 
-    def __init__(self, lc_name="flux", diff_plots=False, centroid_plots=False):
+    def __init__(self, lc_name="flux", diff_plots=False, centroid_plots=False, starloc_pix=None):
         """
         Parameters
         ----------
         lc_name : str
             Name of the flux array in the ``lightkurve`` object.
 
         diff_plots : bool
@@ -612,14 +612,15 @@
 
         self.lc_name = lc_name
         self.tce = None
         self.tpf = None
         self.metrics = None
         self.diff_plots = diff_plots
         self.centroid_plots = centroid_plots
+        self.starloc_pix = starloc_pix
 
     def run(self, tce, lk_tpf, plot=False, remove_transits=None):
         """Runs cent.compute_diff_image_centroids and cent.measure_centroid_shift
         to populate the vetter object.
 
         Parameters
         ----------
@@ -661,20 +662,24 @@
         period_days = tce["period"].to_value(u.day)
         time_offset_q = getattr(exo_const, time_offset_str)
         epoch = tce.get_epoch(time_offset_q).to_value(u.day)
         duration_days = tce["duration"].to_value(u.day)
 
         if remove_transits is None: # reformat to be a blank list
             remove_transits = []
-        
+    
         centroids, figs, kept_transits = cent.compute_diff_image_centroids(
             time, cube, period_days, epoch, duration_days, 
-            remove_transits, plot=self.diff_plots)
+            remove_transits, starloc_pix=self.starloc_pix, plot=self.diff_plots)
         
-        offset, signif, fig = cent.measure_centroid_shift(centroids, kept_transits, self.centroid_plots)
+        if (self.starloc_pix is not None) and (len(self.starloc_pix) == 2):
+            offset, signif, fig = cent.measure_centroid_shift_cat(centroids, kept_transits, self.starloc_pix, self.centroid_plots)
+        else:
+            offset, signif, fig = cent.measure_centroid_shift(centroids, kept_transits, self.centroid_plots)
+
         figs.append(fig)
 
         # TODO: If plot=True, figs is a list of figure handles.
         # Do I save those figures, put them in a single pdf,
         # close them all?
 
         self.metrics = dict(offset=offset, significance=signif)
```

### Comparing `exovetter-0.0.7/exovetter/viz_transits.py` & `exovetter-0.0.8/exovetter/viz_transits.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/exovetter.egg-info/PKG-INFO` & `exovetter-0.0.8/exovetter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exovetter
-Version: 0.0.7
+Version: 0.0.8
 Summary: Exoplanet vetting package
 Home-page: https://github.com/spacetelescope/exovetter
 Author: Susan Mullally et al.
 Author-email: smullally@stsci.edu
 License: BSD 3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `exovetter-0.0.7/exovetter.egg-info/SOURCES.txt` & `exovetter-0.0.8/exovetter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/licenses/DAVE_LICENSE` & `exovetter-0.0.8/licenses/DAVE_LICENSE`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/licenses/TEMPLATE_LICENCE.rst` & `exovetter-0.0.8/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/setup.cfg` & `exovetter-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/setup.py` & `exovetter-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/tutorial_notebooks/100100827.pdf` & `exovetter-0.0.8/tutorial_notebooks/100100827.pdf`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/tutorial_notebooks/LPP.ipynb` & `exovetter-0.0.8/tutorial_notebooks/LPP.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/tutorial_notebooks/LeoTransitEvents.ipynb` & `exovetter-0.0.8/tutorial_notebooks/LeoTransitEvents.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/tutorial_notebooks/OddEven.ipynb` & `exovetter-0.0.8/tutorial_notebooks/OddEven.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/tutorial_notebooks/SWEET.ipynb` & `exovetter-0.0.8/tutorial_notebooks/SWEET.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/tutorial_notebooks/TCEs.ipynb` & `exovetter-0.0.8/tutorial_notebooks/TCEs.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/tutorial_notebooks/TransitPhaseCoverage.ipynb` & `exovetter-0.0.8/tutorial_notebooks/TransitPhaseCoverage.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/tutorial_notebooks/VizTransits.ipynb` & `exovetter-0.0.8/tutorial_notebooks/VizTransits.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/tutorial_notebooks/lightcurves.ipynb` & `exovetter-0.0.8/tutorial_notebooks/lightcurves.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/tutorial_notebooks/modshift.ipynb` & `exovetter-0.0.8/tutorial_notebooks/modshift.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/tutorial_notebooks/run_all.ipynb` & `exovetter-0.0.8/tutorial_notebooks/run_all.ipynb`

 * *Files identical despite different names*

### Comparing `exovetter-0.0.7/tutorial_notebooks/wasp18b.fits` & `exovetter-0.0.8/tutorial_notebooks/wasp18b.fits`

 * *Files identical despite different names*

