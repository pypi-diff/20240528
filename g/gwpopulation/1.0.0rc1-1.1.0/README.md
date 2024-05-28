# Comparing `tmp/gwpopulation-1.0.0rc1.tar.gz` & `tmp/gwpopulation-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwpopulation-1.0.0rc1.tar", last modified: Thu Feb  1 22:40:05 2024, max compression
+gzip compressed data, was "gwpopulation-1.1.0.tar", last modified: Tue May 28 19:03:09 2024, max compression
```

## Comparing `gwpopulation-1.0.0rc1.tar` & `gwpopulation-1.1.0.tar`

### file list

```diff
@@ -1,72 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.935865 gwpopulation-1.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.923865 gwpopulation-1.0.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.923865 gwpopulation-1.0.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-02-01 22:40:05.935865 gwpopulation-1.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.927865 gwpopulation-1.0.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/docs/Makefile.gh_pages
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/docs/Makefile.std
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.927865 gwpopulation-1.0.0rc1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.927865 gwpopulation-1.0.0rc1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)  5402044 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/examples/GWTC1.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.931865 gwpopulation-1.0.0rc1/gwpopulation/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-01 22:40:05.000000 gwpopulation-1.0.0rc1/gwpopulation/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.931865 gwpopulation-1.0.0rc1/gwpopulation/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/experimental/jax.py
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/experimental/numpyro.py
--rw-r--r--   0 runner    (1001) docker     (127)    15537 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/hyperpe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.931865 gwpopulation-1.0.0rc1/gwpopulation/models/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/models/interped.py
--rw-r--r--   0 runner    (1001) docker     (127)    30430 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/models/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/models/redshift.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/models/spin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/vt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.935865 gwpopulation-1.0.0rc1/gwpopulation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-02-01 22:40:05.000000 gwpopulation-1.0.0rc1/gwpopulation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-02-01 22:40:05.000000 gwpopulation-1.0.0rc1/gwpopulation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 22:40:05.000000 gwpopulation-1.0.0rc1/gwpopulation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-01 22:40:05.000000 gwpopulation-1.0.0rc1/gwpopulation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-01 22:40:05.000000 gwpopulation-1.0.0rc1/gwpopulation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/pages_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.931865 gwpopulation-1.0.0rc1/priors/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/priors/bbh_population.prior
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/priors/mass_rates.prior
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/priors/spin.prior
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/priors/spin_talbot_thrane.prior
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-01 22:40:05.935865 gwpopulation-1.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.935865 gwpopulation-1.0.0rc1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/example_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/likelihood_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12213 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/mass_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/redshift_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/spin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/test.prior
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/vt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:09.506631 gwpopulation-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:09.486631 gwpopulation-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:09.490631 gwpopulation-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-28 19:03:09.506631 gwpopulation-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:09.490631 gwpopulation-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:09.490631 gwpopulation-1.1.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:09.490631 gwpopulation-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)  8557137 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/examples/GWTC1.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:09.498631 gwpopulation-1.1.0/gwpopulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 19:03:09.000000 gwpopulation-1.1.0/gwpopulation/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:09.498631 gwpopulation-1.1.0/gwpopulation/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/experimental/cosmo_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/experimental/jax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/experimental/numpyro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15471 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/hyperpe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:09.502631 gwpopulation-1.1.0/gwpopulation/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/models/interped.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30798 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/models/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/models/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/models/spin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/gwpopulation/vt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:09.502631 gwpopulation-1.1.0/gwpopulation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-28 19:03:09.000000 gwpopulation-1.1.0/gwpopulation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-28 19:03:09.000000 gwpopulation-1.1.0/gwpopulation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:03:09.000000 gwpopulation-1.1.0/gwpopulation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-28 19:03:09.000000 gwpopulation-1.1.0/gwpopulation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-28 19:03:09.000000 gwpopulation-1.1.0/gwpopulation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 19:03:09.000000 gwpopulation-1.1.0/gwpopulation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/pages_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:09.502631 gwpopulation-1.1.0/priors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/priors/bbh_population.prior
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/priors/mass_rates.prior
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/priors/spin.prior
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/priors/spin_talbot_thrane.prior
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-28 19:03:09.506631 gwpopulation-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:03:09.502631 gwpopulation-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test/conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test/example_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test/interped_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test/likelihood_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test/mass_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test/redshift_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test/spin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test/test.prior
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test/vt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 19:03:06.000000 gwpopulation-1.1.0/test_requirements.txt
```

### Comparing `gwpopulation-1.0.0rc1/.codeclimate.yml` & `gwpopulation-1.1.0/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/.github/workflows/publish-to-pypi.yml` & `gwpopulation-1.1.0/.github/workflows/publish-to-pypi.yml`

 * *Files 7% similar despite different names*

```diff
@@ -10,17 +10,19 @@
   workflow_dispatch:
 
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI and TestPyPI
     runs-on: ubuntu-20.04
     steps:
-    - uses: actions/checkout@master
+    - uses: actions/checkout@v4
+      with:
+        fetch-depth: 0
     - name: Set up Python 3.10
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
     - name: Install pypa/build
       run: >-
         python -m pip install build --user
     - name: Build a binary wheel and a source tarball
       run: >-
```

### Comparing `gwpopulation-1.0.0rc1/.github/workflows/python-package.yml` & `gwpopulation-1.1.0/.github/workflows/python-package.yml`

 * *Files 4% similar despite different names*

```diff
@@ -20,32 +20,34 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.10", "3.11"]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Setup conda
       uses: s-weigand/setup-conda@v1
       with:
         update-conda: true
         python-version: ${{ matrix.python-version }}
         conda-channels: anaconda, conda-forge
     - name: Install dependencies
       run: |
         conda install pip setuptools
-        conda install --file requirements.txt
+        # install via pip to install from source repo
+        pip install -r requirements.txt
+        # conda install --file requirements.txt
         conda install --file test_requirements.txt
         pre-commit install
     - name: Install gwpopulation
       run: |
         pip install .
     - name: List installed
       run: |
@@ -55,19 +57,20 @@
         pre-commit run --all-files --verbose --show-diff-on-failure
         jupyter nbconvert --clear-output --inplace examples/*.ipynb
         git reset --hard
     - name: Test with pytest
       run: |
         pytest --cov gwpopulation -ra --color yes --cov-report=xml --junitxml=pytest.xml
     - name: Publish coverage to Codecov
-      uses: codecov/codecov-action@v1.2.1
+      uses: codecov/codecov-action@v4
       with:
+        token: ${{ secrets.CODECOV_TOKEN }}
         files: coverage.xml
         flags: python${{ matrix.python-version }}
     - name: Coverage report
       run: python -m coverage report --show-missing
     - name: Upload test results
       if: always()
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v4
       with:
         name: pytest-${{ matrix.python-version }}
         path: pytest.xml
```

### Comparing `gwpopulation-1.0.0rc1/.pre-commit-config.yaml` & `gwpopulation-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/LICENSE.md` & `gwpopulation-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/PKG-INFO` & `gwpopulation-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwpopulation
-Version: 1.0.0rc1
+Version: 1.1.0
 Summary: Unified population inference
 Home-page: https://github.com/ColmTalbot/gwpopulation
 Author: Colm Talbot
 Author-email: talbotcolm@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,17 +12,17 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy>=1.16
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: tqdm
-Requires-Dist: astropy
 Requires-Dist: bilby>=2.2.0
 Requires-Dist: cached_interpolate
+Requires-Dist: wcosmo
 Provides-Extra: cupy
 Requires-Dist: cupy; extra == "cupy"
 Provides-Extra: jax
 Requires-Dist: jax; extra == "jax"
 Requires-Dist: jaxlib; extra == "jax"
 Provides-Extra: pages
 Requires-Dist: ipython_genutils; extra == "pages"
@@ -34,15 +34,17 @@
 Requires-Dist: sphinx; extra == "pages"
 Requires-Dist: sphinx_rtd_theme; extra == "pages"
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
 Requires-Dist: jupyter; extra == "test"
 Requires-Dist: nbconvert; extra == "test"
+Requires-Dist: astropy; extra == "test"
 Requires-Dist: jax; extra == "test"
+Requires-Dist: numpyro; extra == "test"
 
 [![Python package](https://github.com/ColmTalbot/gwpopulation/actions/workflows/python-package.yml/badge.svg)](https://github.com/ColmTalbot/gwpopulation/actions/workflows/python-package.yml)
 [![GitHub Pages](https://github.com/ColmTalbot/gwpopulation/actions/workflows/pages.yml/badge.svg)](https://github.com/ColmTalbot/gwpopulation/actions/workflows/pages.yml)
 [![codecov](https://codecov.io/gh/ColmTalbot/gwpopulation/branch/master/graph/badge.svg?token=4K4V0HRDMI)](https://codecov.io/gh/ColmTalbot/gwpopulation)
 [![Maintainability](https://api.codeclimate.com/v1/badges/579536603e8e06466e63/maintainability)](https://codeclimate.com/github/ColmTalbot/gwpopulation/maintainability)
 [![Versions](https://img.shields.io/pypi/pyversions/gwpopulation.svg)](https://pypi.org/project/gwpopulation/)
```

### Comparing `gwpopulation-1.0.0rc1/README.md` & `gwpopulation-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/docs/Makefile.gh_pages` & `gwpopulation-1.1.0/docs/Makefile`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 
 # You can set these variables from the command line.
 SPHINXOPTS    =
 SPHINXBUILD   = python -msphinx
 SPHINXPROJ    = population
 SOURCEDIR     = .
-BUILDDIR      = ../_gh-pages/latest
+BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 		@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
```

### Comparing `gwpopulation-1.0.0rc1/docs/_templates/custom-class-template.rst` & `gwpopulation-1.1.0/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/docs/_templates/custom-module-template.rst` & `gwpopulation-1.1.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/docs/conf.py` & `gwpopulation-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/gwpopulation/__init__.py` & `gwpopulation-1.1.0/gwpopulation/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/gwpopulation/backend.py` & `gwpopulation-1.1.0/gwpopulation/backend.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,47 +10,54 @@
 :code:`GWPopulation` provides a unified interface to a number of :code:`numpy/scipy` like APIs.
 
 The backend can be set using :code:`gwpopulation.set_backend(backend)`, where
 :code:`backend` is one of :code:`{', '.join(SUPPORTED_BACKENDS)}`.
 
 Downstream packages can automatically track the active backend using :code:`entry_points`.
 With this set up, packages can use :code:`xp` and :code:`scs` in specified modules.
+Additionally, users can provide a full arbitrary scipy object to be used if anything beyond
+:code:`scipy.special` is needed.
+An example of how to set :code:`numpy`, :code:`scipy.special`, and the :code:`toeplitz` function
+from :code:`scipy.linalg` via the :code:`setup.cfg` file is shown below.
+Specification using :code:`pyproject.toml` and :code:`setup.py` follows slightly
+different syntax documentation for which can be found online.
+
+.. code-block::
+
+    [options.entry_points]
+    gwpopulation.xp =
+        mypackage_foo = mypackage.foo
+    gwpopulation.scs =
+        mypackage_foo = mypackage.foo
+        mypackage_bar = mypackage.bar
+    gwpopulation.other =
+        mypackage_baz_toeplitz = mypackage.baz:scipy.linalg.toeplitz
 
-..note::
+.. note::
     Each module that wants to use the :code:`GWPopulation` backend must be specified independently
     for the automatic propagation to work.
 
 If there is a backend that you would like to use that is not currently supported, please open an issue.
 """
 
 
 def modules_to_update():
     import sys
 
     if sys.version_info < (3, 10):
         from importlib_metadata import entry_points
     else:
         from importlib.metadata import entry_points
-    all_with_xp = [
-        ".hyperpe",
-        ".models.interped",
-        ".models.mass",
-        ".models.redshift",
-        ".models.spin",
-        ".utils",
-        ".vt",
+    all_with_xp = [module.value for module in entry_points(group="gwpopulation.xp")]
+    all_with_scs = [module.value for module in entry_points(group="gwpopulation.scs")]
+    other_entries = [
+        module.value.split(":") for module in entry_points(group="gwpopulation.other")
     ]
-    all_with_xp.extend(
-        [module.value for module in entry_points(group="gwpopulation.xp")]
-    )
-    all_with_scs = [".models.mass", ".utils"]
-    all_with_scs.extend(
-        [module.value for module in entry_points(group="gwpopulation.scs")]
-    )
-    return all_with_xp, all_with_scs
+    others = {key: value for key, value in other_entries}
+    return all_with_xp, all_with_scs, others
 
 
 def disable_cupy():
     from warnings import warn
 
     warn(
         f"Function enable_cupy is deprecated, use set_backed('cupy') instead",
@@ -88,32 +95,39 @@
 
     if backend == "jax":
         _configure_jax(xp)
 
     return xp, scs
 
 
-def _set_in_module(module, name, value):
-    if module.startswith("."):
-        package = "gwpopulation"
-    else:
-        package = None
-    setattr(import_module(module, package=package), name, value)
+def _load_arbitrary(func, backend):
+    if func.startswith("scipy"):
+        func = func.replace("scipy", _scipy_module[backend])
+    elif func.startswith("numpy"):
+        func = func.replace("numpy", _np_module[backend])
+    module, func = func.rsplit(".", 1)
+    return getattr(import_module(module), func)
 
 
 def set_backend(backend="numpy"):
     global __backend__
     if backend not in SUPPORTED_BACKENDS:
         raise ValueError(
             f"Backend {backend} not supported, should be in {', '.join(SUPPORTED_BACKENDS)}"
         )
     elif backend == __backend__:
         return
 
     xp, scs = _load_numpy_and_scipy(backend)
 
     __backend__ = backend
-    all_with_xp, all_with_scs = modules_to_update()
+    all_with_xp, all_with_scs, others = modules_to_update()
     for module in all_with_xp:
-        _set_in_module(module, "xp", xp)
+        setattr(import_module(module), "xp", xp)
     for module in all_with_scs:
-        _set_in_module(module, "scs", scs)
+        setattr(import_module(module), "scs", scs)
+    for module, func in others.items():
+        setattr(
+            import_module(module),
+            func.split(".")[-1],
+            _load_arbitrary(func, backend),
+        )
```

### Comparing `gwpopulation-1.0.0rc1/gwpopulation/conversions.py` & `gwpopulation-1.1.0/gwpopulation/conversions.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/gwpopulation/experimental/jax.py` & `gwpopulation-1.1.0/gwpopulation/experimental/jax.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from functools import partial
 
 import numpy as np
 from bilby.core.likelihood import Likelihood
 from bilby.hyper.model import Model
-from jax import jit
 
 
 def generic_bilby_likelihood_function(likelihood, parameters, use_ratio=True):
     likelihood.parameters.update(parameters)
     if use_ratio:
         return likelihood.log_likelihood_ratio()
     else:
@@ -42,14 +41,16 @@
         return probability
 
 
 class JittedLikelihood(Likelihood):
     def __init__(
         self, likelihood, likelihood_func=generic_bilby_likelihood_function, kwargs=None
     ):
+        from jax import jit
+
         if kwargs is None:
             kwargs = dict()
         self.kwargs = kwargs
         self._likelihood = likelihood
         self.likelihood_func = jit(partial(likelihood_func, likelihood))
         super().__init__(dict())
```

### Comparing `gwpopulation-1.0.0rc1/gwpopulation/experimental/numpyro.py` & `gwpopulation-1.1.0/gwpopulation/experimental/numpyro.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/gwpopulation/hyperpe.py` & `gwpopulation-1.1.0/gwpopulation/hyperpe.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self,
         posteriors,
         hyper_prior,
         ln_evidences=None,
         max_samples=1e100,
         selection_function=lambda args: 1,
         conversion_function=lambda args: (args, None),
-        cupy=True,
+        cupy=False,
         maximum_uncertainty=xp.inf,
     ):
         """
         Parameters
         ----------
         posteriors: list
             An list of pandas data frames of samples sets of samples.
@@ -56,29 +56,26 @@
             Function which evaluates your population selection function.
         conversion_function: func
             Function which converts a dictionary of sampled parameter to a
             dictionary of parameters of the population model.
         max_samples: int, optional
             Maximum number of samples to use from each set.
         cupy: bool
-            If True and a compatible CUDA environment is available,
-            cupy will be used for performance.
-            Note: this requires setting up your hyper_prior properly.
+            DEPRECATED: if you want to use cupy, you should manually set the
+            backend using :code:`gwpopulation.set_backend`.
         maximum_uncertainty: float
             The maximum allowed uncertainty in the natural log likelihood.
             If the uncertainty is larger than this value a log likelihood of
             -inf will be returned. Default = inf
         """
         if cupy:
-            from .backend import set_backend
-
-            try:
-                set_backend("cupy")
-            except ImportError:
-                logger.warning(f"Cupy not available, using {xp.__name__}.")
+            logger.warning(
+                f"Setting the backend to cupy is no longer supported in the "
+                "likelihood. Use gwpopulation.set_backend instead."
+            )
 
         self.samples_per_posterior = max_samples
         self.data = self.resample_posteriors(posteriors, max_samples=max_samples)
 
         if isinstance(hyper_prior, types.FunctionType):
             hyper_prior = Model([hyper_prior])
         elif not (
```

### Comparing `gwpopulation-1.0.0rc1/gwpopulation/models/interped.py` & `gwpopulation-1.1.0/gwpopulation/models/interped.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 import numpy as np
 
 from ..utils import to_numpy
 
 xp = np
 
 
-def _setup_interpolant(nodes, values, kind="cubic", backend=xp):
+def _setup_interpolant(nodes, values, kind="cubic", backend=None):
     """
     Cache the information necessary for linear interpolation of the mass
     ratio normalisation
     """
     from cached_interpolate import RegularCachingInterpolant as CachingInterpolant
 
+    if backend is None:
+        backend = xp
+
     nodes = to_numpy(nodes)
     interpolant = CachingInterpolant(nodes, nodes, kind=kind, backend=backend)
-    interpolant.conversion = xp.asarray(interpolant.conversion)
-    interpolant = partial(interpolant, xp.asarray(values))
+    interpolant.conversion = backend.array(interpolant.conversion)
+    interpolant = partial(interpolant, backend.array(values))
     return interpolant
 
 
 class InterpolatedNoBaseModelIdentical:
     """
     Base class for the Interpolated classes with no base model
 
@@ -35,18 +38,28 @@
         Maximum value to normalize the spline over
     nodes: int
         Number of nodes to use in the spline, default=10
     kind: str
         The interpolation order of the spline, default="cubic"
     log_nodes: bool
         Whether to use log-spaced nodes, default=False
+    regularize: bool
+        Whether to regularize the spline node values to have root-mean-square value
+        :code:`rms{name}`, default=False
     """
 
     def __init__(
-        self, parameters, minimum, maximum, nodes=10, kind="cubic", log_nodes=False
+        self,
+        parameters,
+        minimum,
+        maximum,
+        nodes=10,
+        kind="cubic",
+        log_nodes=False,
+        regularize=False,
     ):
         """ """
         self.nodes = nodes
         self._norm_spline = None
         self._data_spline = dict()
         self.kind = kind
         self._xs = xp.linspace(minimum, maximum, 10 * self.nodes)
@@ -54,22 +67,25 @@
         self.min = minimum
         self.max = maximum
         self.log_nodes = log_nodes
 
         self.base = self.parameters[0].strip("_1")
         self.xkeys = [f"{self.base}{ii}" for ii in range(self.nodes)]
         self.fkeys = [f"f{self.base}{ii}" for ii in range(self.nodes)]
+        self.regularize = regularize
 
     def __call__(self, dataset, **kwargs):
         return self.p_x_identical(dataset, **kwargs)
 
     @property
     def variable_names(self):
 
         keys = self.xkeys + self.fkeys
+        if self.regularize:
+            keys += [f"rms{self.base}"]
         return keys
 
     def setup_interpolant(self, nodes, values):
         if self.log_nodes:
             func = xp.log
         else:
             func = xp.array
@@ -97,20 +113,42 @@
 
         perturbation = self._norm_spline(y=f_splines)
         p_x = xp.exp(perturbation)
         p_x *= (self._xs >= x_splines[0]) & (self._xs <= x_splines[-1])
         norm = xp.trapz(p_x, self._xs)
         return norm
 
+    def extract_spline_points(self, kwargs):
+        """
+        Extract the node positions and values from the dictionary of parameters
+
+        Parameters
+        ==========
+        kwargs: dict
+            Dictionary containing :code:`{self.base}_ii, f{self.base_ii}` and
+            optionally :code`rms{self.base}`
+
+        Returns
+        =======
+        f_splines: array-like
+            The values at the spline nodes
+        x_splines: array-like
+            The positions of the spline nodes
+        """
+        f_splines = xp.array([kwargs[key] for key in self.fkeys])
+        if self.regularize:
+            f_splines *= kwargs[f"rms{self.base}"] / xp.mean(f_splines**2) ** 0.5
+        x_splines = xp.array([kwargs[key] for key in self.xkeys])
+        return f_splines, x_splines
+
     def p_x_identical(self, dataset, **kwargs):
 
         self.infer_n_nodes(**kwargs)
 
-        f_splines = xp.array([kwargs[key] for key in self.fkeys])
-        x_splines = xp.array([kwargs[key] for key in self.xkeys])
+        f_splines, x_splines = self.extract_spline_points(kwargs)
 
         p_x = xp.ones(xp.shape(dataset[self.parameters[0]]))
 
         for param in self.parameters:
             p_x *= self.p_x_unnormed(
                 dataset, param, x_splines=x_splines, f_splines=f_splines, **kwargs
             )
```

### Comparing `gwpopulation-1.0.0rc1/gwpopulation/models/mass.py` & `gwpopulation-1.1.0/gwpopulation/models/mass.py`

 * *Files 2% similar despite different names*

```diff
@@ -530,22 +530,23 @@
         vars = set(vars).difference(self.kwargs.keys())
         return vars
 
     @property
     def kwargs(self):
         return dict()
 
-    def __init__(self, mmin=2, mmax=100, normalization_shape=(1000, 500)):
+    def __init__(self, mmin=2, mmax=100, normalization_shape=(1000, 500), cache=True):
         self.mmin = mmin
         self.mmax = mmax
         self.m1s = xp.linspace(mmin, mmax, normalization_shape[0])
         self.qs = xp.linspace(0.001, 1, normalization_shape[1])
         self.dm = self.m1s[1] - self.m1s[0]
         self.dq = self.qs[1] - self.qs[0]
         self.m1s_grid, self.qs_grid = xp.meshgrid(self.m1s, self.qs)
+        self.cache = cache
 
     def __call__(self, dataset, *args, **kwargs):
         beta = kwargs.pop("beta")
         mmin = kwargs.get("mmin", self.mmin)
         mmax = kwargs.get("mmax", self.mmax)
         if "jax" not in xp.__name__:
             if mmin < self.mmin:
@@ -576,43 +577,49 @@
         """Calculate the normalisation factor for the primary mass"""
         mmin = kwargs.get("mmin", self.mmin)
         if "jax" not in xp.__name__ and delta_m == 0:
             return 1
         p_m = self.__class__.primary_model(self.m1s, **kwargs)
         p_m *= self.smoothing(self.m1s, mmin=mmin, mmax=self.mmax, delta_m=delta_m)
 
-        norm = xp.where(xp.array(delta_m) > 0, xp.trapz(p_m, self.m1s), 1)
+        norm = xp.nan_to_num(xp.trapz(p_m, self.m1s)) * (delta_m != 0) + 1 * (
+            delta_m == 0
+        )
         return norm
 
     def p_q(self, dataset, beta, mmin, delta_m):
         p_q = powerlaw(dataset["mass_ratio"], beta, 1, mmin / dataset["mass_1"])
         p_q *= self.smoothing(
             dataset["mass_1"] * dataset["mass_ratio"],
             mmin=mmin,
             mmax=dataset["mass_1"],
             delta_m=delta_m,
         )
+
         try:
-            p_q /= self.norm_p_q(beta=beta, mmin=mmin, delta_m=delta_m)
+            if self.cache:
+                p_q /= self.norm_p_q(beta=beta, mmin=mmin, delta_m=delta_m)
+            else:
+                self._cache_q_norms(dataset["mass_1"])
+                p_q /= self.norm_p_q(beta=beta, mmin=mmin, delta_m=delta_m)
         except (AttributeError, TypeError, ValueError):
             self._cache_q_norms(dataset["mass_1"])
             p_q /= self.norm_p_q(beta=beta, mmin=mmin, delta_m=delta_m)
 
         return xp.nan_to_num(p_q)
 
     def norm_p_q(self, beta, mmin, delta_m):
         """Calculate the mass ratio normalisation by linear interpolation"""
         p_q = powerlaw(self.qs_grid, beta, 1, mmin / self.m1s_grid)
         p_q *= self.smoothing(
             self.m1s_grid * self.qs_grid, mmin=mmin, mmax=self.m1s_grid, delta_m=delta_m
         )
-        norms = xp.where(
-            xp.array(delta_m) > 0,
-            xp.nan_to_num(xp.trapz(p_q, self.qs, axis=0)),
-            xp.ones(self.m1s.shape),
+
+        norms = xp.nan_to_num(xp.trapz(p_q, self.qs, axis=0)) * (delta_m != 0) + 1 * (
+            delta_m == 0
         )
 
         return self._q_interpolant(norms)
 
     def _cache_q_norms(self, masses):
         """
         Cache the information necessary for linear interpolation of the mass
@@ -836,29 +843,38 @@
     fmass{ii}: float
         The values of the spline nodes for the primary mass distribution.
     """
 
     primary_model = power_law_mass
 
     def __init__(
-        self, nodes=10, kind="cubic", mmin=2, mmax=100, normalization_shape=(1000, 500)
+        self,
+        nodes=10,
+        kind="cubic",
+        mmin=2,
+        mmax=100,
+        normalization_shape=(1000, 500),
+        regularize=False,
     ):
         """
         Parameters
         ==========
         nodes: int
             Number of spline nodes to use for interpolation, default=10.
         kind: str
             Order of the spline to use for interpolation, default="cubic".
         mmin: float
             The minimum mass considered for numerical normalization, default=2.
         mmax: float
             The maximum mass considered for numerical normalization, default=100.
         normalization_shape: tuple
             Shape of the grid used for numerical normalization, default=(1000, 500).
+        regularize: bool
+            Whether to regularize the spline node values to have root-mean-square value
+            :code:`rms{name}`, default=False
         """
         BaseSmoothedMassDistribution.__init__(
             self,
             mmin=mmin,
             mmax=mmax,
             normalization_shape=normalization_shape,
         )
@@ -866,28 +882,28 @@
             self,
             minimum=mmin,
             maximum=mmax,
             parameters=["mass_1"],
             nodes=nodes,
             kind=kind,
             log_nodes=True,
+            regularize=regularize,
         )
         self._xs = self.m1s
 
     @property
     def variable_names(self):
         variable_names = super().variable_names.union(
             InterpolatedNoBaseModelIdentical.variable_names.fget(self)
         )
         return variable_names
 
     def p_m1(self, dataset, **kwargs):
 
-        f_splines = xp.array([kwargs[key] for key in self.fkeys])
-        m_splines = xp.array([kwargs[key] for key in self.xkeys])
+        f_splines, m_splines = self.extract_spline_points(kwargs)
 
         mmin = kwargs.get("mmin", self.mmin)
         delta_m = kwargs.pop("delta_m", 0)
         p_m = self.__class__.primary_model(
             dataset["mass_1"], **{key: kwargs[key] for key in ["alpha", "mmin", "mmax"]}
         )
         p_m *= self.smoothing(
@@ -899,15 +915,13 @@
         return p_m / norm
 
     def norm_p_m1(self, delta_m, f_splines=None, **kwargs):
         mmin = kwargs.get("mmin", self.mmin)
         p_m = self.__class__.primary_model(
             self.m1s, **{key: kwargs[key] for key in ["alpha", "mmin", "mmax"]}
         )
-        p_m = xp.where(
-            delta_m > 0,
-            p_m * self.smoothing(self.m1s, mmin=mmin, mmax=self.mmax, delta_m=delta_m),
-            p_m,
+        p_m *= self.smoothing(self.m1s, mmin=mmin, mmax=self.mmax, delta_m=delta_m) ** (
+            delta_m > 0
         )
         p_m *= xp.exp(self._norm_spline(y=f_splines))
         norm = xp.trapz(p_m, self.m1s)
         return norm
```

### Comparing `gwpopulation-1.0.0rc1/gwpopulation/models/spin.py` & `gwpopulation-1.1.0/gwpopulation/models/spin.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,28 +277,30 @@
         )
         return xp.trapz(
             y=xp.trapz(y=prob, axis=-1, x=self.chi_eff), axis=-1, x=self.chi_p
         )
 
 
 class SplineSpinMagnitudeIdentical(InterpolatedNoBaseModelIdentical):
-    def __init__(self, minimum=0, maximum=1, nodes=5, kind="cubic"):
+    def __init__(self, minimum=0, maximum=1, nodes=5, kind="cubic", regularize=False):
 
         super(SplineSpinMagnitudeIdentical, self).__init__(
             parameters=["a_1", "a_2"],
             minimum=minimum,
             maximum=maximum,
             nodes=nodes,
             kind=kind,
+            regularize=regularize,
         )
 
 
 class SplineSpinTiltIdentical(InterpolatedNoBaseModelIdentical):
-    def __init__(self, minimum=-1, maximum=1, nodes=5, kind="cubic"):
+    def __init__(self, minimum=-1, maximum=1, nodes=5, kind="cubic", regularize=False):
 
         super(SplineSpinTiltIdentical, self).__init__(
             parameters=["cos_tilt_1", "cos_tilt_2"],
             minimum=minimum,
             maximum=maximum,
             nodes=nodes,
             kind=kind,
+            regularize=regularize,
         )
```

### Comparing `gwpopulation-1.0.0rc1/gwpopulation/utils.py` & `gwpopulation-1.1.0/gwpopulation/utils.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/gwpopulation/vt.py` & `gwpopulation-1.1.0/gwpopulation/vt.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,11 +190,11 @@
         Returns
         -------
         float: The volume
 
         """
         if self.redshift_model is None:
             return self._surveyed_hypervolume
-        else:
+        elif isinstance(self.redshift_model, _Redshift):
             return (
                 self.redshift_model.normalisation(parameters) / 1e9 * self.analysis_time
             )
```

### Comparing `gwpopulation-1.0.0rc1/gwpopulation.egg-info/PKG-INFO` & `gwpopulation-1.1.0/gwpopulation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwpopulation
-Version: 1.0.0rc1
+Version: 1.1.0
 Summary: Unified population inference
 Home-page: https://github.com/ColmTalbot/gwpopulation
 Author: Colm Talbot
 Author-email: talbotcolm@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,17 +12,17 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy>=1.16
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: tqdm
-Requires-Dist: astropy
 Requires-Dist: bilby>=2.2.0
 Requires-Dist: cached_interpolate
+Requires-Dist: wcosmo
 Provides-Extra: cupy
 Requires-Dist: cupy; extra == "cupy"
 Provides-Extra: jax
 Requires-Dist: jax; extra == "jax"
 Requires-Dist: jaxlib; extra == "jax"
 Provides-Extra: pages
 Requires-Dist: ipython_genutils; extra == "pages"
@@ -34,15 +34,17 @@
 Requires-Dist: sphinx; extra == "pages"
 Requires-Dist: sphinx_rtd_theme; extra == "pages"
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
 Requires-Dist: jupyter; extra == "test"
 Requires-Dist: nbconvert; extra == "test"
+Requires-Dist: astropy; extra == "test"
 Requires-Dist: jax; extra == "test"
+Requires-Dist: numpyro; extra == "test"
 
 [![Python package](https://github.com/ColmTalbot/gwpopulation/actions/workflows/python-package.yml/badge.svg)](https://github.com/ColmTalbot/gwpopulation/actions/workflows/python-package.yml)
 [![GitHub Pages](https://github.com/ColmTalbot/gwpopulation/actions/workflows/pages.yml/badge.svg)](https://github.com/ColmTalbot/gwpopulation/actions/workflows/pages.yml)
 [![codecov](https://codecov.io/gh/ColmTalbot/gwpopulation/branch/master/graph/badge.svg?token=4K4V0HRDMI)](https://codecov.io/gh/ColmTalbot/gwpopulation)
 [![Maintainability](https://api.codeclimate.com/v1/badges/579536603e8e06466e63/maintainability)](https://codeclimate.com/github/ColmTalbot/gwpopulation/maintainability)
 [![Versions](https://img.shields.io/pypi/pyversions/gwpopulation.svg)](https://pypi.org/project/gwpopulation/)
```

### Comparing `gwpopulation-1.0.0rc1/gwpopulation.egg-info/SOURCES.txt` & `gwpopulation-1.1.0/gwpopulation.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 .codeclimate.yml
 .codecov.yml
 .gitignore
 .pre-commit-config.yaml
+CODE_OF_CONDUCT.md
 LICENSE.md
 MANIFEST.in
 README.md
 pages_requirements.txt
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 test_requirements.txt
 .github/workflows/pages.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/python-package.yml
-docs/Makefile.gh_pages
-docs/Makefile.std
+docs/.gitignore
+docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/_templates/custom-class-template.rst
 docs/_templates/custom-module-template.rst
 examples/GWTC1.ipynb
 gwpopulation/__init__.py
 gwpopulation/_version.py
@@ -27,17 +28,19 @@
 gwpopulation/conversions.py
 gwpopulation/hyperpe.py
 gwpopulation/utils.py
 gwpopulation/vt.py
 gwpopulation.egg-info/PKG-INFO
 gwpopulation.egg-info/SOURCES.txt
 gwpopulation.egg-info/dependency_links.txt
+gwpopulation.egg-info/entry_points.txt
 gwpopulation.egg-info/requires.txt
 gwpopulation.egg-info/top_level.txt
 gwpopulation/experimental/__init__.py
+gwpopulation/experimental/cosmo_models.py
 gwpopulation/experimental/jax.py
 gwpopulation/experimental/numpyro.py
 gwpopulation/models/__init__.py
 gwpopulation/models/interped.py
 gwpopulation/models/mass.py
 gwpopulation/models/redshift.py
 gwpopulation/models/spin.py
@@ -45,15 +48,15 @@
 priors/mass_rates.prior
 priors/spin.prior
 priors/spin_talbot_thrane.prior
 test/__init__.py
 test/backend_test.py
 test/conversion_test.py
 test/example_test.py
-test/jax_utils.py
+test/interped_test.py
 test/likelihood_test.py
 test/mass_test.py
 test/redshift_test.py
 test/spin_test.py
 test/test.prior
 test/utils_test.py
 test/vt_test.py
```

### Comparing `gwpopulation-1.0.0rc1/priors/bbh_population.prior` & `gwpopulation-1.1.0/priors/bbh_population.prior`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/priors/mass_rates.prior` & `gwpopulation-1.1.0/priors/mass_rates.prior`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/priors/spin.prior` & `gwpopulation-1.1.0/priors/spin.prior`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/test/backend_test.py` & `gwpopulation-1.1.0/test/backend_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import importlib
 
-import numpy
 import pytest
 
 import gwpopulation
 
 from . import TEST_BACKENDS
 
 
@@ -51,7 +50,22 @@
 
     gwpopulation.backend.import_module = _import
     with pytest.raises(ImportError):
         gwpopulation.set_backend("numpy")
         gwpopulation.set_backend("jax")
 
     gwpopulation.backend.import_module = importlib.import_module
+
+
+def test_loading_arbitrary():
+    """
+    Test loading arbitrary functions works as we don't have any native
+    entry points for them.
+    """
+    pytest.importorskip("jax")
+
+    from jax.scipy.linalg import toeplitz
+
+    func = gwpopulation.backend._load_arbitrary(
+        func="scipy.linalg.toeplitz", backend="jax"
+    )
+    assert func == toeplitz
```

### Comparing `gwpopulation-1.0.0rc1/test/conversion_test.py` & `gwpopulation-1.1.0/test/conversion_test.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/test/example_test.py` & `gwpopulation-1.1.0/test/example_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import glob
-from functools import partial
 
 import bilby
-import numpy as np
 import pandas as pd
 import pytest
-from bilby.core.likelihood import Likelihood
 from bilby.hyper.model import Model
-from jax import jit
 
 import gwpopulation
+from gwpopulation.experimental.jax import JittedLikelihood, NonCachingModel
 
 from . import TEST_BACKENDS
-from .jax_utils import JittedLikelihood, NonCachingModel
 
 
 def _template_likelihod_evaluation(backend, jit):
     gwpopulation.set_backend(backend)
     xp = gwpopulation.models.mass.xp
     bilby.core.utils.random.seed(10)
     rng = bilby.core.utils.random.rng
@@ -81,14 +77,16 @@
 
 @pytest.mark.parametrize("backend", TEST_BACKENDS)
 def test_likelihood_evaluation(backend):
     _template_likelihod_evaluation(backend, False)
 
 
 def test_jit_likelihood():
+    pytest.importorskip("jax")
+
     _template_likelihod_evaluation("jax", True)
 
 
 def test_prior_files_load():
     for fname in glob.glob("priors/*.prior"):
         print(fname)
         _ = bilby.core.prior.PriorDict(fname)
```

### Comparing `gwpopulation-1.0.0rc1/test/likelihood_test.py` & `gwpopulation-1.1.0/test/likelihood_test.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/test/mass_test.py` & `gwpopulation-1.1.0/test/mass_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     m1s, qs, dataset = get_primary_mass_ratio_data(xp)
     prior = double_power_prior()
     m1s = dataset["mass_1"]
     for ii in range(N_TEST):
         parameters = prior.sample()
         p_m = mass.double_power_law_primary_power_law_mass_ratio(dataset, **parameters)
         p_m = to_numpy(p_m)
-        assert np.max(p_m[m1s > parameters["mmax"]]) == 0.0
+        assert np.max(p_m[to_numpy(m1s) > parameters["mmax"]]) == 0.0
 
 
 def get_primary_mass_ratio_data(xp):
     m1s = xp.linspace(3, 100, 1000)
     qs = xp.linspace(0.01, 1, 500)
     m1s_grid, qs_grid = xp.meshgrid(m1s, qs)
     dataset = dict(mass_1=m1s_grid, mass_ratio=qs_grid)
```

### Comparing `gwpopulation-1.0.0rc1/test/redshift_test.py` & `gwpopulation-1.1.0/test/redshift_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,28 +42,29 @@
     priors["z_peak"] = Uniform(0, 5)
     _run_model_normalisation(model=model, priors=priors, xp=xp)
 
 
 @pytest.mark.parametrize("backend", TEST_BACKENDS)
 def test_powerlaw_volume(backend):
     """
-    Test that the total volume matches the expected value for a
+    Test that the total volume matches astropy for a
     trivial case
     """
     gwpopulation.set_backend(backend)
     xp = gwpopulation.utils.xp
     zs = xp.linspace(1e-3, 2.3, 1000)
     zs_numpy = gwpopulation.utils.to_numpy(zs)
     model = redshift.PowerLawRedshift()
     parameters = dict(lamb=1)
     total_volume = np.trapz(
         Planck15.differential_comoving_volume(zs_numpy).value * 4 * np.pi,
         zs_numpy,
     )
-    assert abs(total_volume - float(model.normalisation(parameters))) < 1e-3
+    approximation = float(model.normalisation(parameters))
+    assert abs(total_volume - approximation) / total_volume < 1e-2
 
 
 def test_zero_outside_domain():
     model = redshift.PowerLawRedshift(z_max=1)
     assert model(dict(redshift=5), lamb=1) == 0
```

### Comparing `gwpopulation-1.0.0rc1/test/spin_test.py` & `gwpopulation-1.1.0/test/spin_test.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/test/test.prior` & `gwpopulation-1.1.0/test/test.prior`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/test/utils_test.py` & `gwpopulation-1.1.0/test/utils_test.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc1/test/vt_test.py` & `gwpopulation-1.1.0/test/vt_test.py`

 * *Files identical despite different names*

