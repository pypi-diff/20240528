# Comparing `tmp/scippneutron-24.3.0.tar.gz` & `tmp/scippneutron-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scippneutron-24.3.0.tar", last modified: Mon Mar 25 13:18:40 2024, max compression
+gzip compressed data, was "scippneutron-24.5.0.tar", last modified: Tue May 28 14:01:15 2024, max compression
```

## Comparing `scippneutron-24.3.0.tar` & `scippneutron-24.5.0.tar`

### file list

```diff
@@ -1,213 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.618994 scippneutron-24.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.586994 scippneutron-24.3.0/.buildconfig/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.buildconfig/ci-linux.yml
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.buildconfig/ci-macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.buildconfig/ci-windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.586994 scippneutron-24.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.586994 scippneutron-24.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.github/workflows/nightly_at_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.github/workflows/nightly_at_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.github/workflows/pr_and_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.github/workflows/python-version-ci
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.github/workflows/unpinned.yml
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-25 13:18:27.000000 scippneutron-24.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-03-25 13:18:27.000000 scippneutron-24.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-25 13:18:27.000000 scippneutron-24.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-25 13:18:27.000000 scippneutron-24.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-25 13:18:27.000000 scippneutron-24.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-25 13:18:40.618994 scippneutron-24.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-25 13:18:27.000000 scippneutron-24.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.590994 scippneutron-24.3.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:27.000000 scippneutron-24.3.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-25 13:18:27.000000 scippneutron-24.3.0/benchmarks/load_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-25 13:18:27.000000 scippneutron-24.3.0/benchmarks/transform_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.590994 scippneutron-24.3.0/conda/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-25 13:18:27.000000 scippneutron-24.3.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.590994 scippneutron-24.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.590994 scippneutron-24.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/_static/anaconda-icon.js
--rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    19453 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    19147 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    19908 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/_static/straight-beamline.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.594994 scippneutron-24.3.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/_templates/class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/_templates/doc_version.html
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/_templates/module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/_typehints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.594994 scippneutron-24.3.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/about/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/about/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.594994 scippneutron-24.3.0/docs/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/api-reference/chopper-cascade.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/api-reference/frame-unwrapping.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.594994 scippneutron-24.3.0/docs/api-reference/frameunwrapping/
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/api-reference/frameunwrapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/bibliography.bib
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.594994 scippneutron-24.3.0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/developer/coding-conventions.md
--rw-r--r--   0 runner    (1001) docker     (127)    16402 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/developer/data-stream.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.598994 scippneutron-24.3.0/docs/developer/data_stream/
--rw-r--r--   0 runner    (1001) docker     (127)    18688 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/developer/data_stream/data_stream_arch.svg
--rw-r--r--   0 runner    (1001) docker     (127)    19463 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/developer/data_stream/data_stream_arch_testing.svg
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/developer/data_stream/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/developer/dependency-management.md
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/developer/file-loading.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/developer/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/developer/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.598994 scippneutron-24.3.0/docs/environments/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/environments/scippneutron.yml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.598994 scippneutron-24.3.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    15970 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/tutorials/1_exploring-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/tutorials/2_working-with-masks.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    36016 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/tutorials/3_understanding-event-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/tutorials/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    16244 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/tutorials/powder-diffraction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/tutorials/strip-solutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.598994 scippneutron-24.3.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (127)    25991 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/user-guide/coordinate-transformations.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23083 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/user-guide/from-mantid-to-scipp.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/user-guide/groupby.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/user-guide/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/user-guide/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/user-guide/instrument-view.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/user-guide/make_PG3_4844_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-03-25 13:18:27.000000 scippneutron-24.3.0/docs/user-guide/recipes.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-03-25 13:18:27.000000 scippneutron-24.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.602994 scippneutron-24.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/basetest.in
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/basetest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/make_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/nightly.in
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/nightly.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-25 13:18:27.000000 scippneutron-24.3.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.602994 scippneutron-24.3.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    70398 2024-03-25 13:18:27.000000 scippneutron-24.3.0/resources/logo-2022.svg
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-25 13:18:40.622994 scippneutron-24.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.574994 scippneutron-24.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.602994 scippneutron-24.3.0/src/scippneutron/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.606994 scippneutron-24.3.0/src/scippneutron/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.606994 scippneutron-24.3.0/src/scippneutron/atoms/
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/atoms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/atoms/scattering_parameters.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/beamline_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.606994 scippneutron-24.3.0/src/scippneutron/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/conversion/beamline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.606994 scippneutron-24.3.0/src/scippneutron/conversion/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/conversion/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/conversion/graph/beamline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/conversion/graph/tof.py
--rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/conversion/tof.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.606994 scippneutron-24.3.0/src/scippneutron/core/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/core/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.606994 scippneutron-24.3.0/src/scippneutron/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.610994 scippneutron-24.3.0/src/scippneutron/data_streaming/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/data_streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/data_streaming/_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/data_streaming/_consumer_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    20070 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/data_streaming/_data_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/data_streaming/_data_consumption_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/data_streaming/_data_stream_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/data_streaming/_serialisation.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/data_streaming/_stop_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/data_streaming/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/data_streaming/data_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/instrument_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.610994 scippneutron-24.3.0/src/scippneutron/io/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19756 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/io/cif.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.610994 scippneutron-24.3.0/src/scippneutron/io/nexus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/io/nexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/io/nexus/_json_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/io/nexus/_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    16797 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/io/nexus/load_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/io/xye.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    59108 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/mantid.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.610994 scippneutron-24.3.0/src/scippneutron/tof/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/tof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17917 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/tof/chopper_cascade.py
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/tof/diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/tof/fakes.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-03-25 13:18:27.000000 scippneutron-24.3.0/src/scippneutron/tof/unwrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.618994 scippneutron-24.3.0/src/scippneutron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-25 13:18:40.000000 scippneutron-24.3.0/src/scippneutron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-03-25 13:18:40.000000 scippneutron-24.3.0/src/scippneutron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 13:18:40.000000 scippneutron-24.3.0/src/scippneutron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-25 13:18:40.000000 scippneutron-24.3.0/src/scippneutron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-25 13:18:40.000000 scippneutron-24.3.0/src/scippneutron.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.614994 scippneutron-24.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/HYS_mask.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.614994 scippneutron-24.3.0/tests/atoms/
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/atoms/test_atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/beamline_components_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.614994 scippneutron-24.3.0/tests/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/conversion/beamline_conversions_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.614994 scippneutron-24.3.0/tests/conversion/graph/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/conversion/graph/beamline_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/conversion/graph/tof_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21635 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/conversion/tof_conversions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24639 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/convert_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    44954 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/data_stream_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/instrument_view_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.614994 scippneutron-24.3.0/tests/io/
--rw-r--r--   0 runner    (1001) docker     (127)    20690 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/io/cif_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.618994 scippneutron-24.3.0/tests/io/json_nexus_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/io/json_nexus_examples/array_dataset.json
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/io/json_nexus_examples/dataset.json
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/io/json_nexus_examples/detector.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/io/json_nexus_examples/entry.json
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/io/json_nexus_examples/event_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    38541 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/io/json_nexus_examples/instrument.json
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/io/json_nexus_examples/log.json
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/io/load_nexus_json_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    74104 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/io/load_nexus_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    32537 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/io/nexus_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/io/xye_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.618994 scippneutron-24.3.0/tests/mantid_scipp_comparison/
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/mantid_scipp_comparison/beamline_calculations_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/mantid_scipp_comparison/histogram_events_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/mantid_scipp_comparison/neutron_convert_units_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    48662 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/mantid_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/package_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.618994 scippneutron-24.3.0/tests/tof/
--rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/tof/chopper_cascade_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/tof/fakes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/tof/to_time_of_flight_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tests/tof/unwrap_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:18:40.618994 scippneutron-24.3.0/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tools/make_tutorial_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-25 13:18:27.000000 scippneutron-24.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.080623 scippneutron-24.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.048622 scippneutron-24.5.0/.buildconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.buildconfig/ci-linux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.048622 scippneutron-24.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.048622 scippneutron-24.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.github/workflows/nightly_at_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.github/workflows/nightly_at_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.github/workflows/python-version-ci
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.github/workflows/unpinned.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-28 14:01:04.000000 scippneutron-24.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-28 14:01:04.000000 scippneutron-24.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-28 14:01:04.000000 scippneutron-24.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-28 14:01:04.000000 scippneutron-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 14:01:04.000000 scippneutron-24.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-28 14:01:15.080623 scippneutron-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-28 14:01:04.000000 scippneutron-24.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.048622 scippneutron-24.5.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:04.000000 scippneutron-24.5.0/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-28 14:01:04.000000 scippneutron-24.5.0/benchmarks/load_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-28 14:01:04.000000 scippneutron-24.5.0/benchmarks/transform_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.048622 scippneutron-24.5.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-28 14:01:04.000000 scippneutron-24.5.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.052622 scippneutron-24.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.052622 scippneutron-24.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/_static/anaconda-icon.js
+-rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    19453 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    19147 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    19908 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/_static/straight-beamline.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.052622 scippneutron-24.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/_templates/class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/_templates/module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.052622 scippneutron-24.5.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/about/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/about/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.052622 scippneutron-24.5.0/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/api-reference/chopper-cascade.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/api-reference/frame-unwrapping.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.052622 scippneutron-24.5.0/docs/api-reference/frameunwrapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/api-reference/frameunwrapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/bibliography.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.056622 scippneutron-24.5.0/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/developer/data-stream.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.056622 scippneutron-24.5.0/docs/developer/data_stream/
+-rw-r--r--   0 runner    (1001) docker     (127)    18688 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/developer/data_stream/data_stream_arch.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    19463 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/developer/data_stream/data_stream_arch_testing.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/developer/data_stream/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/developer/file-loading.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/developer/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.056622 scippneutron-24.5.0/docs/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/environments/scippneutron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.056622 scippneutron-24.5.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    15994 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/tutorials/1_exploring-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/tutorials/2_working-with-masks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    36016 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/tutorials/3_understanding-event-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/tutorials/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/tutorials/powder-diffraction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/tutorials/strip-solutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.060622 scippneutron-24.5.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)    25957 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/user-guide/coordinate-transformations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23036 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/user-guide/from-mantid-to-scipp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/user-guide/groupby.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/user-guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/user-guide/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/user-guide/instrument-view.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/user-guide/make_PG3_4844_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-28 14:01:04.000000 scippneutron-24.5.0/docs/user-guide/recipes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-28 14:01:04.000000 scippneutron-24.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.064622 scippneutron-24.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/basetest.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/basetest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/make_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/nightly.in
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/nightly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-28 14:01:04.000000 scippneutron-24.5.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.064622 scippneutron-24.5.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    70398 2024-05-28 14:01:04.000000 scippneutron-24.5.0/resources/logo-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:01:15.080623 scippneutron-24.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.040622 scippneutron-24.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.064622 scippneutron-24.5.0/src/scippneutron/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.064622 scippneutron-24.5.0/src/scippneutron/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.064622 scippneutron-24.5.0/src/scippneutron/atoms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/atoms/scattering_parameters.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/beamline_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.068622 scippneutron-24.5.0/src/scippneutron/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/conversion/beamline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.068622 scippneutron-24.5.0/src/scippneutron/conversion/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/conversion/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/conversion/graph/beamline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/conversion/graph/tof.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18632 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/conversion/tof.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.068622 scippneutron-24.5.0/src/scippneutron/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/core/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.068622 scippneutron-24.5.0/src/scippneutron/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.068622 scippneutron-24.5.0/src/scippneutron/data_streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/data_streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/data_streaming/_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/data_streaming/_consumer_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20130 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/data_streaming/_data_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/data_streaming/_data_consumption_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/data_streaming/_data_stream_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/data_streaming/_serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/data_streaming/_stop_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/data_streaming/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12676 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/data_streaming/data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/instrument_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.068622 scippneutron-24.5.0/src/scippneutron/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19636 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/io/cif.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.072622 scippneutron-24.5.0/src/scippneutron/io/nexus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/io/nexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/io/nexus/_json_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/io/nexus/_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16942 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/io/nexus/load_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/io/xye.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59044 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/mantid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.072622 scippneutron-24.5.0/src/scippneutron/peaks/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/peaks/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24133 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/peaks/_fit_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/peaks/_remove_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/peaks/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.072622 scippneutron-24.5.0/src/scippneutron/tof/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/tof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17891 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/tof/chopper_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/tof/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/tof/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21438 2024-05-28 14:01:04.000000 scippneutron-24.5.0/src/scippneutron/tof/unwrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.080623 scippneutron-24.5.0/src/scippneutron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-28 14:01:14.000000 scippneutron-24.5.0/src/scippneutron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-28 14:01:15.000000 scippneutron-24.5.0/src/scippneutron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:01:14.000000 scippneutron-24.5.0/src/scippneutron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 14:01:14.000000 scippneutron-24.5.0/src/scippneutron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 14:01:14.000000 scippneutron-24.5.0/src/scippneutron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.076622 scippneutron-24.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/HYS_mask.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.076622 scippneutron-24.5.0/tests/atoms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/atoms/test_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/beamline_components_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.076622 scippneutron-24.5.0/tests/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/conversion/beamline_conversions_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.076622 scippneutron-24.5.0/tests/conversion/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/conversion/graph/beamline_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/conversion/graph/tof_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21649 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/conversion/tof_conversions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24879 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/convert_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45171 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/data_stream_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/instrument_view_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.076622 scippneutron-24.5.0/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)    20771 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/io/cif_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.076622 scippneutron-24.5.0/tests/io/json_nexus_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/io/json_nexus_examples/array_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/io/json_nexus_examples/dataset.json
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/io/json_nexus_examples/detector.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/io/json_nexus_examples/entry.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/io/json_nexus_examples/event_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    38541 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/io/json_nexus_examples/instrument.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/io/json_nexus_examples/log.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/io/load_nexus_json_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74488 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/io/load_nexus_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32157 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/io/nexus_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/io/xye_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.080623 scippneutron-24.5.0/tests/mantid_scipp_comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/mantid_scipp_comparison/beamline_calculations_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/mantid_scipp_comparison/histogram_events_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/mantid_scipp_comparison/neutron_convert_units_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48409 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/mantid_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/package_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.080623 scippneutron-24.5.0/tests/peaks/
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/peaks/fit_peaks_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17580 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/peaks/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/peaks/remove_peaks_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.080623 scippneutron-24.5.0/tests/tof/
+-rw-r--r--   0 runner    (1001) docker     (127)    19616 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/tof/chopper_cascade_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/tof/fakes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/tof/to_time_of_flight_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tests/tof/unwrap_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:15.080623 scippneutron-24.5.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tools/make_tutorial_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-28 14:01:04.000000 scippneutron-24.5.0/tox.ini
```

### Comparing `scippneutron-24.3.0/.buildconfig/ci-linux.yml` & `scippneutron-24.5.0/.buildconfig/ci-linux.yml`

 * *Files 15% similar despite different names*

```diff
@@ -12,33 +12,33 @@
   - hypothesis==6.88.1
   - ipykernel==6.25.2
   - ipympl==0.9.3
   - ipywidgets==8.0.6
   - mantid==6.8.0
   - matplotlib==3.8.2
   - ninja==1.11.1
-  - plopp==24.01.1
+  - plopp==24.04.0
   - pooch==1.7.0
   - pytest==7.4.2
   - pytest-asyncio==0.21.1
   - python-confluent-kafka==2.1.1
   - python-graphviz==0.20.1
   - pythreejs==2.4.2
   - scipp==23.07.0
   - scippnexus==23.12.1
   - scipy==1.12.0
   - tox==4.11.3
 
   # docs
-  - myst-parser==2.0.0
+  - myst-parser==3.0.1
   - nbsphinx==0.9.3
-  - packaging==23.2
-  - pandoc==3.1.3
+  - packaging==24.0
+  - pandoc==3.1.13
   - pydata-sphinx-theme==0.15.2
-  - sphinx==7.2.6
-  - sphinx-autodoc-typehints==1.25.2
+  - sphinx==7.3.7
+  - sphinx-autodoc-typehints==2.1.0
   - sphinx-copybutton==0.5.2
   - sphinx-design==0.5.0
-  - sphinxcontrib-bibtex==2.6.1
+  - sphinxcontrib-bibtex==2.6.2
 
   # docs and tests
-  - sciline==24.01.1
+  - sciline==24.04.1
```

### Comparing `scippneutron-24.3.0/.github/dependabot.yml` & `scippneutron-24.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/.github/workflows/ci.yml` & `scippneutron-24.5.0/.github/workflows/ci.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: CI
 
 on:
   push:
     branches:
       - main
       - release
@@ -20,23 +17,24 @@
     steps:
       - uses: actions/checkout@v4
       - name: Get Python version for other CI jobs
         id: vars
         run: |
           echo "min_python=$(cat .github/workflows/python-version-ci)" >> $GITHUB_OUTPUT
           echo "min_tox_env=py$(cat .github/workflows/python-version-ci | sed 's/\.//g')" >> $GITHUB_OUTPUT
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version-file: '.github/workflows/python-version-ci'
-      - run: python -m pip install --upgrade pip
-      - run: python -m pip install -r requirements/ci.txt
-      - run: tox -e static
-      - uses: stefanzweifel/git-auto-commit-action@v5
+      - uses: pre-commit/action@v3.0.1
+        with:
+          extra_args: --all-files
+      - uses: pre-commit-ci/lite-action@v1.0.2
+        if: always()
         with:
-          commit_message: Apply automatic formatting
+          msg: Apply automatic formatting
 
   tests:
     name: Tests
     needs: formatting
     strategy:
       matrix:
         os: ['ubuntu-22.04']
@@ -45,14 +43,35 @@
             tox-env: '${{needs.formatting.outputs.min_tox_env}}'
     uses: ./.github/workflows/test.yml
     with:
       os-variant: ${{ matrix.os }}
       python-version: ${{ matrix.python.version }}
       tox-env: ${{ matrix.python.tox-env }}
 
+  mantid:
+    name: Mantid tests
+    needs: formatting
+    runs-on: 'ubuntu-22.04'
+    defaults:
+      run:
+        shell: bash -l {0}  # required for conda env
+    steps:
+      - uses: actions/checkout@v4
+      - name: Setup conda environment
+        uses: mamba-org/setup-micromamba@v1
+        with:
+          micromamba-version: 1.5.6-0
+          environment-file: .buildconfig/ci-linux.yml
+          cache-environment: true
+          create-args: >-
+            python=3.10
+            conda-build
+      - run: conda develop src
+      - run: python -m pytest tests/mantid_*
+
   docs:
-    needs: tests
+    needs: [tests, mantid]
     uses: ./.github/workflows/docs.yml
     with:
       publish: false
       linkcheck: ${{ contains(matrix.variant.os, 'ubuntu') && github.ref == 'refs/heads/main' }}
       branch: ${{ github.head_ref == '' && github.ref_name || github.head_ref }}
```

### Comparing `scippneutron-24.3.0/.github/workflows/docs.yml` & `scippneutron-24.5.0/.github/workflows/docs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: Docs
 
 on:
   workflow_dispatch:
     inputs:
       publish:
         default: false
@@ -46,17 +43,18 @@
     name: Build documentation
     runs-on: 'ubuntu-22.04'
     defaults:
       run:
         shell: bash -l {0}  # required for conda env
     steps:
       - run: sudo apt install --yes graphviz pandoc
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           ref: ${{ inputs.branch == '' && github.ref_name || inputs.branch }}
+          repository: ${{ github.event.pull_request.head.repo.full_name }}
           fetch-depth: 0  # history required so cmake can determine version
       - uses: mamba-org/setup-micromamba@v1
         if: ${{ inputs.version != '' }}
         with:
           environment-file: .buildconfig/ci-linux.yml
           cache-environment: true
           create-args: >-
@@ -66,26 +64,24 @@
         if: ${{ inputs.version == '' }}
         with:
           environment-file: .buildconfig/ci-linux.yml
           cache-environment: true
           create-args: >-
             python=3.10
             conda-build
-      - run: conda develop src
+      - run: pip install --no-build-isolation --no-deps -e .
         if: ${{ inputs.version == '' }}
-      - run: |
-          python -m sphinx -j2 -v -b html -d doctrees docs html
-          python -m sphinx -j2 -v -b doctest -d doctrees docs html
-          find html -type f -name "*.ipynb" -not -path "html/_sources/*" -delete
+      - run: python -m sphinx -W -v -b doctest -d doctrees docs html
+      - run: python -m sphinx -W -v -b html -d doctrees docs html
+      - run: find html -type f -name "*.ipynb" -not -path "html/_sources/*" -delete
       - run: tox -e linkcheck
         if: ${{ inputs.linkcheck }}
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: docs_html
           path: html/
-
-      - uses: JamesIves/github-pages-deploy-action@v4.4.3
+      - uses: JamesIves/github-pages-deploy-action@v4.6.1
         if: ${{ inputs.publish }}
         with:
           branch: gh-pages
           folder: html
           single-commit: true
```

### Comparing `scippneutron-24.3.0/.github/workflows/nightly_at_main.yml` & `scippneutron-24.5.0/.github/workflows/nightly_at_main.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: Nightly test at main branch
 
 on:
   workflow_dispatch:
   schedule:
     - cron: '30 1 * * 1-5'
```

### Comparing `scippneutron-24.3.0/.github/workflows/nightly_at_release.yml` & `scippneutron-24.5.0/.github/workflows/unpinned.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
-name: Nightly tests at latest release
+name: Unpinned tests at latest release
 
 on:
   workflow_dispatch:
   schedule:
-    - cron: '0 1 * * 1-5'
+    - cron: '0 2 * * 1'
 
 jobs:
   setup:
     name: Setup variables
     runs-on: 'ubuntu-22.04'
     outputs:
       min_python: ${{ steps.vars.outputs.min_python }}
@@ -30,14 +27,14 @@
     name: Tests
     needs: setup
     strategy:
       matrix:
         os: ['ubuntu-22.04']
         python:
           - version: '${{needs.setup.outputs.min_python}}'
-            tox-env: 'nightly'
+            tox-env: 'unpinned'
     uses: ./.github/workflows/test.yml
     with:
       os-variant: ${{ matrix.os }}
       python-version: ${{ matrix.python.version }}
       tox-env: ${{ matrix.python.tox-env }}
       checkout_ref: ${{ needs.setup.outputs.release_tag }}
```

### Comparing `scippneutron-24.3.0/.github/workflows/release.yml` & `scippneutron-24.5.0/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: Release
 
 on:
   release:
     types: [published]
   workflow_dispatch:
 
@@ -14,77 +11,77 @@
 
 jobs:
   build_conda:
     name: Conda build
     runs-on: 'ubuntu-22.04'
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: true
           fetch-depth: 0  # history required so setuptools_scm can determine version
 
       - uses: mamba-org/setup-micromamba@v1
         with:
           environment-name: build-env
           create-args: >-
             conda-build
             boa
       - run: conda mambabuild --channel conda-forge --channel scipp --channel ess-dmsc --no-anaconda-upload --override-channels --output-folder conda/package conda
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: conda-package-noarch
           path: conda/package/noarch/*.tar.bz2
 
   build_wheels:
     name: Wheels
     runs-on: 'ubuntu-22.04'
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0  # history required so setuptools_scm can determine version
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version-file: '.github/workflows/python-version-ci'
 
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/wheels.txt
 
       - name: Build wheels
         run: python -m build
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: dist
           path: dist
 
   upload_pypi:
     name: Deploy PyPI
     needs: [build_wheels, build_conda]
     runs-on: 'ubuntu-22.04'
     environment: release
     permissions:
       id-token: write
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
-      - uses: actions/download-artifact@v3
-      - uses: pypa/gh-action-pypi-publish@v1.8.10
+      - uses: actions/download-artifact@v4
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
 
   upload_conda:
     name: Deploy Conda
     needs: [build_wheels, build_conda]
     runs-on: 'ubuntu-22.04'
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
       - uses: mamba-org/setup-micromamba@v1
         with:
           environment-name: upload-env
           # frozen python due to breaking removal of 'imp' in 3.12
           create-args: >-
             anaconda-client
             python=3.11
@@ -101,15 +98,15 @@
   assets:
     name: Upload docs
     needs: docs
     runs-on: 'ubuntu-22.04'
     permissions:
       contents: write  # This is needed so that the action can upload the asset
     steps:
-    - uses: actions/download-artifact@v3
+    - uses: actions/download-artifact@v4
     - name: Zip documentation
       run: |
         mv docs_html documentation-${{ github.ref_name }}
         zip -r documentation-${{ github.ref_name }}.zip documentation-${{ github.ref_name }}
     - name: Upload release assets
       uses: svenstaro/upload-release-action@v2
       with:
```

### Comparing `scippneutron-24.3.0/.github/workflows/test.yml` & `scippneutron-24.5.0/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 name: Test
 
 on:
   workflow_dispatch:
     inputs:
       os-variant:
         default: 'ubuntu-22.04'
@@ -44,21 +41,21 @@
         type: string
 
 jobs:
   test:
     runs-on: ${{ inputs.os-variant }}
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           ref: ${{ inputs.checkout_ref }}
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ inputs.python-version }}
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r ${{ inputs.pip-recipe }}
       - run: tox -e ${{ inputs.tox-env }}
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         if: ${{ inputs.coverage-report }}
         with:
           name: CoverageReport
           path: coverage_html/
```

### Comparing `scippneutron-24.3.0/.github/workflows/unpinned.yml` & `scippneutron-24.5.0/.github/workflows/nightly_at_release.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
-name: Unpinned tests at latest release
+name: Nightly tests at latest release
 
 on:
   workflow_dispatch:
   schedule:
-    - cron: '0 2 * * 1'
+    - cron: '0 1 * * 1-5'
 
 jobs:
   setup:
     name: Setup variables
     runs-on: 'ubuntu-22.04'
     outputs:
       min_python: ${{ steps.vars.outputs.min_python }}
@@ -30,14 +27,14 @@
     name: Tests
     needs: setup
     strategy:
       matrix:
         os: ['ubuntu-22.04']
         python:
           - version: '${{needs.setup.outputs.min_python}}'
-            tox-env: 'unpinned'
+            tox-env: 'nightly'
     uses: ./.github/workflows/test.yml
     with:
       os-variant: ${{ matrix.os }}
       python-version: ${{ matrix.python.version }}
       tox-env: ${{ matrix.python.tox-env }}
       checkout_ref: ${{ needs.setup.outputs.release_tag }}
```

### Comparing `scippneutron-24.3.0/.pre-commit-config.yaml` & `scippneutron-24.5.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -9,42 +9,29 @@
       - id: check-toml
       - id: check-yaml
         exclude: conda/meta.yaml
       - id: detect-private-key
       - id: trailing-whitespace
         args: [ --markdown-linebreak-ext=md ]
         exclude: '\.svg'
-  - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        name: isort (python)
-  - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 23.11.0
-    hooks:
-      - id: black
   - repo: https://github.com/kynan/nbstripout
     rev: 0.6.0
     hooks:
       - id: nbstripout
         types: [ "jupyter" ]
         args: [ "--drop-empty-cells",
                 "--extra-keys 'metadata.language_info.version cell.metadata.jp-MarkdownHeadingCollapsed cell.metadata.pycharm'" ]
-  - repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
-    hooks:
-      - id: flake8
-        types: ["python"]
-        additional_dependencies: ["flake8-bugbear==23.9.16"]
-  - repo: https://github.com/pycqa/bandit
-    rev: 1.7.5
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.3
     hooks:
-      - id: bandit
-        additional_dependencies: ["bandit[toml]"]
-        args: ["-c", "pyproject.toml"]
+      - id: ruff
+        args: [ --fix ]
+        types_or: [ python, pyi, jupyter ]
+      - id: ruff-format
+        types_or: [ python, pyi ]
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
         additional_dependencies:
           - tomli
   - repo: https://github.com/pre-commit/pygrep-hooks
```

### Comparing `scippneutron-24.3.0/CODE_OF_CONDUCT.md` & `scippneutron-24.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/CONTRIBUTING.md` & `scippneutron-24.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/LICENSE` & `scippneutron-24.5.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
+Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `scippneutron-24.3.0/PKG-INFO` & `scippneutron-24.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: scippneutron
-Version: 24.3.0
+Version: 24.5.0
 Summary: Neutron scattering tools for Data Reduction
 Author: Scipp contributors
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
+        Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -38,30 +38,29 @@
 Project-URL: Source, https://github.com/scipp/scippneutron
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5py
 Requires-Dist: numpy>=1.20
 Requires-Dist: pooch
+Requires-Dist: plopp>=24.04.0
 Requires-Dist: scipp>=23.07.0
 Requires-Dist: scippnexus>=23.8.0
 Requires-Dist: scipy>=1.7.0
-Provides-Extra: interactive
-Requires-Dist: scipp[interactive]; extra == "interactive"
 Provides-Extra: all
 Requires-Dist: scipp[all]; extra == "all"
 
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 [![PyPI badge](http://img.shields.io/pypi/v/scippneutron.svg)](https://pypi.python.org/pypi/scippneutron)
 [![Anaconda-Server Badge](https://anaconda.org/scipp/scippneutron/badges/version.svg)](https://anaconda.org/scipp/scippneutron)
 [![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](LICENSE)
```

### Comparing `scippneutron-24.3.0/README.md` & `scippneutron-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/benchmarks/transform_coords.py` & `scippneutron-24.5.0/benchmarks/transform_coords.py`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/_static/anaconda-icon.js` & `scippneutron-24.5.0/docs/_static/anaconda-icon.js`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/_static/favicon.ico` & `scippneutron-24.5.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/_static/logo-dark.svg` & `scippneutron-24.5.0/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/_static/logo.svg` & `scippneutron-24.5.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/_static/straight-beamline.svg` & `scippneutron-24.5.0/docs/_static/straight-beamline.svg`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/_templates/class-template.rst` & `scippneutron-24.5.0/docs/_templates/class-template.rst`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/_templates/module-template.rst` & `scippneutron-24.5.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/about/index.md` & `scippneutron-24.5.0/docs/about/index.md`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/api-reference/chopper-cascade.ipynb` & `scippneutron-24.5.0/docs/api-reference/chopper-cascade.ipynb`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/api-reference/frame-unwrapping.ipynb` & `scippneutron-24.5.0/docs/api-reference/frame-unwrapping.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975942460317461%*

 * *Differences: {"'cells'": "{6: {'source': {delete: [0]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -95,15 +95,14 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b99c6293",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import scipp as sc\n",
                 "import sciline as sl\n",
                 "from scippneutron.tof import unwrap"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bdd00acc",
@@ -251,13 +250,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.12"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scippneutron-24.3.0/docs/api-reference/frameunwrapping/__init__.py` & `scippneutron-24.5.0/docs/api-reference/frameunwrapping/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     diagram.add_neutron(
         L=det1,
         time_offset=frame_offset,
         wavelength=20.0 * sc.units.angstrom,
         label=r'$T_0^{i+1}+\Delta t$',
     )
 
-    props = dict(arrowstyle='-|>')
+    props = {'arrowstyle': '-|>'}
     x0 = diagram.frame_length
     x1 = diagram.frame_length + frame_offset
     m = sc.Unit('m')
     ms = sc.Unit('ms')
     diagram.annotate(
         r'$T_0^i$', xy=(x0, 0 * m), xytext=(x0 - 20 * ms, 3 * m), arrowprops=props
     )
@@ -81,15 +81,15 @@
     diagram.add_sample(distance=20.0 * sc.Unit('m'))
     diagram.add_detector(distance=det1, name='detector1')
     diagram.add_detector(distance=det2, name='detector2')
     diagram.add_neutrons(
         Lmax=1.05 * det2, lambda_min=lambda_min, time_offset=frame_offset, stride=2
     )
 
-    props = dict(arrowstyle='-|>')
+    props = {'arrowstyle': '-|>'}
     x0 = 2 * diagram.frame_length
     x1 = 2 * diagram.frame_length + frame_offset
     m = sc.Unit('m')
     ms = sc.Unit('ms')
     diagram.annotate(
         r'$T_0^i$', xy=(x0, 0 * m), xytext=(x0 - 20 * ms, 3 * m), arrowprops=props
     )
```

### Comparing `scippneutron-24.3.0/docs/api-reference/index.md` & `scippneutron-24.5.0/docs/api-reference/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
    :template: module-template.rst
    :recursive:
 
    atoms
    conversion
    io
    logging
+   peaks
    tof
 ```
 
 ## Frame handling
 
 ```{toctree}
 ---
```

### Comparing `scippneutron-24.3.0/docs/bibliography.bib` & `scippneutron-24.5.0/docs/bibliography.bib`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/conf.py` & `scippneutron-24.5.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,53 @@
-# -*- coding: utf-8 -*-
-
 import doctest
 import os
 import sys
+from importlib.metadata import PackageNotFoundError
+from importlib.metadata import version as get_version
 
-import scippneutron
+from sphinx.util import logging
 
 sys.path.insert(0, os.path.abspath('.'))
 
-from _typehints import typehints_formatter_for  # noqa: E402
+logger = logging.getLogger(__name__)
 
 # General information about the project.
-project = u'ScippNeutron'
-copyright = u'2023 Scipp contributors'
-author = u'Scipp contributors'
+project = 'ScippNeutron'
+copyright = '2024 Scipp contributors'
+author = 'Scipp contributors'
 
 html_show_sourcelink = True
 
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.doctest',
     'sphinx.ext.githubpages',
     'sphinx.ext.intersphinx',
     'sphinx.ext.mathjax',
     'sphinx.ext.napoleon',
+    'sphinx.ext.viewcode',
     'sphinx_autodoc_typehints',
     'sphinx_copybutton',
     'sphinx_design',
     'sphinxcontrib.bibtex',
     'nbsphinx',
     'myst_parser',
 ]
 
+try:
+    import sciline.sphinxext.domain_types  # noqa: F401
+
+    extensions.append('sciline.sphinxext.domain_types')
+    # See https://github.com/tox-dev/sphinx-autodoc-typehints/issues/457
+    suppress_warnings = ["config.cache"]
+except ModuleNotFoundError:
+    pass
+
+
 myst_enable_extensions = [
     "amsmath",
     "colon_fence",
     "deflist",
     "dollarmath",
     "fieldlist",
     "html_admonition",
@@ -78,17 +89,29 @@
     # objects without namespace: scipp
     "DataArray": "~scipp.DataArray",
     "Dataset": "~scipp.Dataset",
     "Variable": "~scipp.Variable",
     # objects without namespace: numpy
     "ndarray": "~numpy.ndarray",
 }
+napoleon_custom_sections = ['Fit procedure', 'Model selection']
 typehints_defaults = 'comma'
 typehints_use_rtype = False
-typehints_formatter = typehints_formatter_for('scippneutron')
+
+
+sciline_domain_types_prefix = 'scippneutron'
+sciline_domain_types_aliases = {
+    'scipp._scipp.core.DataArray': 'scipp.DataArray',
+    'scipp._scipp.core.Dataset': 'scipp.Dataset',
+    'scipp._scipp.core.DType': 'scipp.DType',
+    'scipp._scipp.core.Unit': 'scipp.Unit',
+    'scipp._scipp.core.Variable': 'scipp.Variable',
+    'scipp.core.data_group.DataGroup': 'scipp.DataGroup',
+}
+
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
@@ -99,18 +122,23 @@
 master_doc = 'index'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 
-# The short X.Y version.
-version = scippneutron.__version__
-# The full version, including alpha/beta/rc tags.
-release = scippneutron.__version__
+try:
+    release = get_version("scippneutron")
+    version = ".".join(release.split('.')[:3])  # CalVer
+except PackageNotFoundError:
+    logger.info(
+        "Warning: determining version from package metadata failed, falling back to "
+        "a dummy version number."
+    )
+    release = version = "0.0.0-dev"
 
 warning_is_error = True
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
```

### Comparing `scippneutron-24.3.0/docs/developer/coding-conventions.md` & `scippneutron-24.5.0/docs/developer/coding-conventions.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Coding conventions
 
 ## Code formatting
 
-There are no explicit code formatting conventions since we use `black` to enforce a format.
+There are no explicit code formatting conventions since we use `ruff` to enforce a format.
 
 ## Docstring format
 
 We use the [NumPy docstring format](https://www.sphinx-doc.org/en/master/usage/extensions/example_numpy.html).
 We use `sphinx-autodocs-typehints` to automatically insert type hints into the docstrings.
 Our format thus deviates from the default NumPy example given by the link above.
 Docstrings should therefore be laid out as follows, including spacing and punctuation:
```

### Comparing `scippneutron-24.3.0/docs/developer/data-stream.rst` & `scippneutron-24.5.0/docs/developer/data-stream.rst`

 * *Files 0% similar despite different names*

```diff
@@ -176,17 +176,17 @@
     in the notebook.
 
 Unit Testing
 ------------
 
 For unit tests it would be convenient to use a fake consumer object in place of ``KafkaConsumer``
 instances. However, any input arguments or variables passed via the queue to the ``mp.Process``
-must be pickleable or ``mp.Queue``. This makes dependency injection difficult. To get around
+must be pickleable or ``mp.queues.Queue``. This makes dependency injection difficult. To get around
 this an enum can be passed via ``data_stream`` to the ``data_consumption_manager`` to tell it
-to create instances of ``FakeConsumer`` instead of ``KafkaConsumer``, additionally an ``mp.Queue``
+to create instances of ``FakeConsumer`` instead of ``KafkaConsumer``, additionally an ``mp.queues.Queue``
 can be provided and is passed to the ``FakeConsumer``. The ``FakeConsumer`` simply polls for messages
 on the queue instead of Kafka, thus allowing the test to provide the messages. There is no other
 configuration of ``FakeConsumer`` possible or necessary.
 
 .. image:: data_stream/data_stream_arch_testing.svg
    :width: 600
```

### Comparing `scippneutron-24.3.0/docs/developer/data_stream/data_stream_arch.svg` & `scippneutron-24.5.0/docs/developer/data_stream/data_stream_arch.svg`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/developer/data_stream/data_stream_arch_testing.svg` & `scippneutron-24.5.0/docs/developer/data_stream/data_stream_arch_testing.svg`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/developer/data_stream/docker-compose.yml` & `scippneutron-24.5.0/docs/developer/data_stream/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/developer/dependency-management.md` & `scippneutron-24.5.0/docs/developer/dependency-management.md`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/developer/file-loading.rst` & `scippneutron-24.5.0/docs/developer/file-loading.rst`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/developer/getting-started.md` & `scippneutron-24.5.0/docs/developer/getting-started.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ## Running tests
 
 `````{tab-set}
 ````{tab-item} tox
 Run the tests using
 
 ```sh
-tox -e py39
+tox -e py310
 ```
 
 (or just `tox` if you want to run all environments).
 
 ````
 ````{tab-item} Manually
 Run the tests using
```

### Comparing `scippneutron-24.3.0/docs/index.md` & `scippneutron-24.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/tutorials/1_exploring-data.ipynb` & `scippneutron-24.5.0/docs/tutorials/1_exploring-data.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997967479674796%*

 * *Differences: {"'cells'": '{22: {\'source\': {insert: [(1, "detector.coords[\'tof\'] += 2.3 * sc.Unit(\\n"), (2, '*

 * *            '"    \'us\'\\n"), (3, ")  # note how we forgot to fix the monitor\'s TOF\\n")], '*

 * *            'delete: [1]}}}'}*

```diff
@@ -307,15 +307,17 @@
                 "tags": [
                     "solution"
                 ]
             },
             "outputs": [],
             "source": [
                 "detector.coords['sample_position'] += sc.vector(value=[0.01, 0.01, 0.04], unit='m')\n",
-                "detector.coords['tof'] += 2.3 * sc.Unit('us')  # note how we forgot to fix the monitor's TOF\n",
+                "detector.coords['tof'] += 2.3 * sc.Unit(\n",
+                "    'us'\n",
+                ")  # note how we forgot to fix the monitor's TOF\n",
                 "detector"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": [
```

### Comparing `scippneutron-24.3.0/docs/tutorials/2_working-with-masks.ipynb` & `scippneutron-24.5.0/docs/tutorials/2_working-with-masks.ipynb`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/tutorials/3_understanding-event-data.ipynb` & `scippneutron-24.5.0/docs/tutorials/3_understanding-event-data.ipynb`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/tutorials/powder-diffraction.ipynb` & `scippneutron-24.5.0/docs/tutorials/powder-diffraction.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998931623931624%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(5, \'raw_vanadium = scn.load_with_mantid(\\n\'), (6, "    '*

 * *            'scn.data.get_path(\'PG3_4866_event.nxs\'), load_pulse_times=False\\n"), (7, \')\')], '*

 * *            'delete: [5]}}}'}*

```diff
@@ -39,15 +39,17 @@
             "outputs": [],
             "source": [
                 "raw_sample = scn.load_with_mantid(\n",
                 "    scn.data.get_path('PG3_4844_event.nxs'),\n",
                 "    load_pulse_times=False,\n",
                 "    mantid_args={'LoadMonitors': True},\n",
                 ")\n",
-                "raw_vanadium = scn.load_with_mantid(scn.data.get_path('PG3_4866_event.nxs'), load_pulse_times=False)"
+                "raw_vanadium = scn.load_with_mantid(\n",
+                "    scn.data.get_path('PG3_4866_event.nxs'), load_pulse_times=False\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The optional `mantid_args` dict is forwarded to the Mantid algorithm used for loading the files &ndash; in this case [LoadEventNexus](https://docs.mantidproject.org/nightly/algorithms/LoadEventNexus-v1.html) &ndash; and can be used to control, e.g., which part of a file to load.\n",
```

### Comparing `scippneutron-24.3.0/docs/tutorials/strip-solutions.py` & `scippneutron-24.5.0/docs/tutorials/strip-solutions.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,11 +20,11 @@
     help='Paths of notebooks to convert.',
 )
 parser.add_argument('--output-dir', dest='path', help='Output folder')
 
 args = parser.parse_args()
 
 for name in args.names:
-    print(f"Stripping solution cells from {name}")
+    print(f"Stripping solution cells from {name}")  # noqa: T201
     output = NotebookExporter(config=c).from_filename(name)
     with open(os.path.join(args.path, os.path.basename(name)), "w") as f:
         f.write(output[0])
```

### Comparing `scippneutron-24.3.0/docs/user-guide/coordinate-transformations.ipynb` & `scippneutron-24.5.0/docs/user-guide/coordinate-transformations.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997361111111112%*

 * *Differences: {"'cells'": "{33: {'source': {insert: [(2, 'da = scn.data.tutorial_dense_data()[\\n'), (3, "*

 * *            '"    \'detector\'\\n"), (4, \']  # Note that this is actually a SANS beamline, not an '*

 * *            "imaging beamline\\n')], delete: [4, 3, 2]}}, 41: {'source': {insert: [(2, '    return "*

 * *            "sc.sqrt(wavelength**2 - 2 * (lambda_K**2) * sc.log(sc.cos(0.5 * two_theta)))')], "*

 * *            'delete: [4, 3, 2]}}}'}*

```diff
@@ -490,17 +490,17 @@
             "execution_count": null,
             "id": "6a84eae2-b015-4d11-96a2-5846199b160e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import scippneutron as scn\n",
                 "\n",
-                "da = (\n",
-                "    scn.data.tutorial_dense_data()['detector']\n",
-                ")  # Note that this is actually a SANS beamline, not an imaging beamline\n",
+                "da = scn.data.tutorial_dense_data()[\n",
+                "    'detector'\n",
+                "]  # Note that this is actually a SANS beamline, not an imaging beamline\n",
                 "da_plane = da.transform_coords(\"wavelength\", graph=plane_graph)\n",
                 "da_plane"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "05781e6f-dad9-47d9-8ee4-92ceb1f1ca68",
@@ -593,17 +593,15 @@
             "execution_count": null,
             "id": "aed7624e-09fb-47ff-87ab-e3c7a3339bf5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def dspacing_perpendicular(wavelength, two_theta):\n",
                 "    lambda_K = sc.scalar(1.0, unit=\"angstrom\")\n",
-                "    return sc.sqrt(\n",
-                "        wavelength**2 - 2 * (lambda_K**2) * sc.log(sc.cos(0.5 * two_theta))\n",
-                "    )"
+                "    return sc.sqrt(wavelength**2 - 2 * (lambda_K**2) * sc.log(sc.cos(0.5 * two_theta)))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "573c7976-f205-4a15-b356-649701204364",
             "metadata": {},
             "source": [
```

### Comparing `scippneutron-24.3.0/docs/user-guide/from-mantid-to-scipp.ipynb` & `scippneutron-24.5.0/docs/user-guide/from-mantid-to-scipp.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975595238095238%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'import scippneutron as scn')], delete: [3, 2]}}, 41: "*

 * *            '{\'source\': ["sc.concat([a_scipp[\'data\'][\'spectrum\', 7], '*

 * *            'b_scipp[\'data\'][\'spectrum\', 7]], \'spectrum\')"]}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -78,16 +78,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import mantid.simpleapi as mantid\n",
                 "import scipp as sc\n",
-                "import scippneutron as scn\n",
-                "import numpy as np"
+                "import scippneutron as scn"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Test Data"
@@ -421,16 +420,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sc.concat([a_scipp['data']['spectrum', 7], b_scipp['data']['spectrum', 7]],\n",
-                "          'spectrum')"
+                "sc.concat([a_scipp['data']['spectrum', 7], b_scipp['data']['spectrum', 7]], 'spectrum')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### GroupWorkspaces"
@@ -955,13 +953,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.17"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `scippneutron-24.3.0/docs/user-guide/groupby.ipynb` & `scippneutron-24.5.0/docs/user-guide/groupby.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996753246753247%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(2, \'data = scn.load_with_mantid(\\n\'), (3, "    '*

 * *            'scn.data.get_path(\'PG3_4844_event.nxs\'), load_pulse_times=False\\n"), (4, '*

 * *            "')\\n')], delete: [2]}}}"}*

```diff
@@ -29,15 +29,17 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Load event data. Here, we use `get_path` to find a data file that comes bundled\n",
                 "# with scippneutron. Normally, we would simply pass a file path to `scn.load`.\n",
-                "data = scn.load_with_mantid(scn.data.get_path('PG3_4844_event.nxs'), load_pulse_times=False)\n",
+                "data = scn.load_with_mantid(\n",
+                "    scn.data.get_path('PG3_4844_event.nxs'), load_pulse_times=False\n",
+                ")\n",
                 "data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `scippneutron-24.3.0/docs/user-guide/installation.md` & `scippneutron-24.5.0/docs/user-guide/installation.md`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/user-guide/instrument-view.ipynb` & `scippneutron-24.5.0/docs/user-guide/instrument-view.ipynb`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/docs/user-guide/recipes.ipynb` & `scippneutron-24.5.0/docs/user-guide/recipes.ipynb`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/pyproject.toml` & `scippneutron-24.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -14,37 +14,37 @@
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Typing :: Typed",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 dynamic = ["version"]
 
 # IMPORTANT:
 # Run 'tox -e deps' after making changes here. This will update requirement files.
 # Make sure to list one dependency per line.
 dependencies = [
     "h5py",
     "numpy>=1.20",
     "pooch",
+    "plopp>=24.04.0",
     "scipp>=23.07.0",
     "scippnexus>=23.8.0",
     "scipy>=1.7.0",
 ]
 
 [project.optional-dependencies]
-interactive = ["scipp[interactive]"]
 all = ['scipp[all]']
 
 [project.urls]
 "Bug Tracker" = "https://github.com/scipp/scippneutron/issues"
 "Documentation" = "https://scipp.github.io/scippneutron"
 "Source" = "https://github.com/scipp/scippneutron"
 
@@ -85,34 +85,61 @@
   'ignore:Widget._active_widgets is deprecated:DeprecationWarning',
   'ignore:Widget._widget_types is deprecated:DeprecationWarning',
   'ignore:Widget.widget_types is deprecated:DeprecationWarning',
   'ignore:Widget.widgets is deprecated:DeprecationWarning',
   'ignore:`load_nexus` is deprecated:UserWarning',
 ]
 
-[tool.bandit]
-# Excluding tests because bandit doesn't like `assert`.
-exclude_dirs = ["docs/conf.py", "tests", "tools"]
-
 [tool.codespell]
 ignore-words-list = "elemt"
 skip = "./.git,./.tox,*/.virtual_documents,*/.ipynb_checkpoints,*.pdf,*.svg,*.csv"
 
-[tool.black]
-skip-string-normalization = true
+[tool.ruff]
+line-length = 88
+extend-include = ["*.ipynb"]
+extend-exclude = [
+    ".*", "__pycache__", "build", "dist", "install",
+]
+
+[tool.ruff.lint]
+# See https://docs.astral.sh/ruff/rules/
+select = ["B", "C4", "DTZ", "E", "F", "G", "I", "PERF", "PGH", "PT", "PYI", "RUF", "S", "T20", "UP", "W"]
+ignore = [
+    # Conflict with ruff format, see
+    # https://docs.astral.sh/ruff/formatter/#conflicting-lint-rules
+    "COM812", "COM819", "D206", "D300", "E111", "E114", "E117", "ISC001", "ISC002", "Q000", "Q001", "Q002", "Q003", "W191",
+]
+fixable = ["I001", "B010"]
+isort.known-first-party = ["scippneutron"]
+pydocstyle.convention = "numpy"
+
+[tool.ruff.lint.per-file-ignores]
+# those files have an increased risk of relying on import order
+"__init__.py" = ["I"]
+"tests/*" = [
+    "S101",  # asserts are fine in tests
+    "B018",  # 'useless expressions' are ok because some tests just check for exceptions
+]
+"*.ipynb" = [
+    "E501",  # longer lines are sometimes more readable
+    "F403",  # *-imports used with domain types
+    "F405",  # linter may fail to find names because of *-imports
+    "I",  # we don't collect imports at the top
+    "S101",  # asserts are used for demonstration and are safe in notebooks
+    "T201",  # printing is ok for demonstration purposes
+]
+"docs/user-guide/recipes.ipynb" = [
+  "F821"  # this notebook is never executed and uses undefined names
+]
 
-[tool.isort]
-skip_gitignore = true
-profile = "black"
-known_first_party = ["scippneutron"]
-skip_glob = ["src/scippneutron/__init__.py"]
+[tool.ruff.format]
+quote-style = "preserve"
 
 [tool.mypy]
 strict = true
 ignore_missing_imports = true
 enable_error_code = [
     "ignore-without-code",
     "redundant-expr",
     "truthy-bool",
 ]
-show_error_codes = true
 warn_unreachable = true
```

### Comparing `scippneutron-24.3.0/requirements/base.txt` & `scippneutron-24.5.0/requirements/base.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,69 @@
-# SHA1:1f3acab129a5a13898348311ef3fb50f5354e09b
+# SHA1:ab44a7b6900bf9efbcb7e3b06a6cbdba11149163
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-asttokens==2.4.1
-    # via stack-data
-backcall==0.2.0
-    # via ipython
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
-decorator==5.1.1
-    # via ipython
-executing==2.0.1
-    # via stack-data
-fonttools==4.47.2
-    # via matplotlib
-graphviz==0.20.1
-    # via scipp
-h5py==3.10.0
+fonttools==4.52.1
+    # via matplotlib
+h5py==3.11.0
     # via
     #   -r base.in
-    #   scipp
     #   scippnexus
-idna==3.6
+idna==3.7
     # via requests
-ipython==8.9.0
-    # via -r base.in
-jedi==0.19.1
-    # via ipython
 kiwisolver==1.4.5
     # via matplotlib
-matplotlib==3.8.2
-    # via
-    #   plopp
-    #   scipp
-matplotlib-inline==0.1.6
-    # via ipython
-numpy==1.26.3
+matplotlib==3.9.0
+    # via plopp
+numpy==1.26.4
     # via
     #   -r base.in
     #   contourpy
     #   h5py
     #   matplotlib
     #   scipp
     #   scipy
-packaging==23.2
+packaging==24.0
     # via
     #   matplotlib
     #   pooch
-parso==0.8.3
-    # via jedi
-pexpect==4.9.0
-    # via ipython
-pickleshare==0.7.5
-    # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via matplotlib
-platformdirs==4.1.0
+platformdirs==4.2.2
     # via pooch
-plopp==24.1.1
-    # via scipp
-pooch==1.8.0
-    # via
-    #   -r base.in
-    #   scipp
-prompt-toolkit==3.0.36
-    # via
-    #   -r base.in
-    #   ipython
-ptyprocess==0.7.0
-    # via pexpect
-pure-eval==0.2.2
-    # via stack-data
-pygments==2.17.2
-    # via ipython
-pyparsing==3.1.1
+plopp==24.5.0
+    # via -r base.in
+pooch==1.8.1
+    # via -r base.in
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   matplotlib
     #   scippnexus
-requests==2.31.0
+requests==2.32.2
     # via pooch
-scipp[all]==24.2.0
+scipp==24.5.0
     # via
     #   -r base.in
     #   scippnexus
 scippnexus==24.3.1
     # via -r base.in
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   -r base.in
-    #   scipp
     #   scippnexus
 six==1.16.0
-    # via
-    #   asttokens
-    #   python-dateutil
-stack-data==0.6.3
-    # via ipython
-traitlets==5.14.1
-    # via
-    #   ipython
-    #   matplotlib-inline
-urllib3==2.1.0
+    # via python-dateutil
+urllib3==2.2.1
     # via requests
-wcwidth==0.2.13
-    # via prompt-toolkit
```

### Comparing `scippneutron-24.3.0/requirements/ci.txt` & `scippneutron-24.5.0/requirements/ci.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # SHA1:6344d52635ea11dca331a3bc6eb1833c4c64d585
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-cachetools==5.3.2
+cachetools==5.3.3
     # via tox
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 chardet==5.2.0
     # via tox
 charset-normalizer==3.3.2
     # via requests
 colorama==0.4.6
     # via tox
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   tox
     #   virtualenv
 gitdb==4.0.11
     # via gitpython
-gitpython==3.1.41
+gitpython==3.1.43
     # via -r ci.in
-idna==3.6
+idna==3.7
     # via requests
-packaging==23.2
+packaging==24.0
     # via
     #   -r ci.in
     #   pyproject-api
     #   tox
-platformdirs==4.1.0
+platformdirs==4.2.2
     # via
     #   tox
     #   virtualenv
-pluggy==1.3.0
+pluggy==1.5.0
     # via tox
 pyproject-api==1.6.1
     # via tox
-requests==2.31.0
+requests==2.32.2
     # via -r ci.in
 smmap==5.0.1
     # via gitdb
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.12.1
+tox==4.15.0
     # via -r ci.in
-urllib3==2.1.0
+urllib3==2.2.1
     # via requests
-virtualenv==20.25.0
+virtualenv==20.26.2
     # via tox
```

### Comparing `scippneutron-24.3.0/requirements/dev.txt` & `scippneutron-24.5.0/requirements/dev.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,124 +8,132 @@
 -r base.txt
 -r ci.txt
 -r docs.txt
 -r mypy.txt
 -r static.txt
 -r test.txt
 -r wheels.txt
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
-anyio==4.2.0
-    # via jupyter-server
+anyio==4.4.0
+    # via
+    #   httpx
+    #   jupyter-server
 argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.3.0
     # via isoduration
 async-lru==2.0.4
     # via jupyterlab
 cffi==1.16.0
     # via argon2-cffi-bindings
 click==8.1.7
     # via
     #   pip-compile-multi
     #   pip-tools
-copier==9.1.1
+copier==9.2.0
     # via -r dev.in
-dunamai==1.19.0
+dunamai==1.21.1
     # via copier
 fqdn==1.5.1
     # via jsonschema
 funcy==2.0
     # via copier
+h11==0.14.0
+    # via httpcore
+httpcore==1.0.5
+    # via httpx
+httpx==0.27.0
+    # via jupyterlab
 isoduration==20.11.0
     # via jsonschema
 jinja2-ansible-filters==1.3.2
     # via copier
-json5==0.9.14
+json5==0.9.25
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
-jsonschema[format-nongpl]==4.21.1
+jsonschema[format-nongpl]==4.22.0
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
-jupyter-events==0.9.0
+jupyter-events==0.10.0
     # via jupyter-server
-jupyter-lsp==2.2.2
+jupyter-lsp==2.2.5
     # via jupyterlab
-jupyter-server==2.12.5
+jupyter-server==2.14.0
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook-shim
-jupyter-server-terminals==0.5.2
+jupyter-server-terminals==0.5.3
     # via jupyter-server
-jupyterlab==4.0.11
+jupyterlab==4.2.1
     # via -r dev.in
-jupyterlab-server==2.25.2
+jupyterlab-server==2.27.2
     # via jupyterlab
-notebook-shim==0.2.3
+notebook-shim==0.2.4
     # via jupyterlab
-overrides==7.6.0
+overrides==7.7.0
     # via jupyter-server
 pathspec==0.12.1
     # via copier
 pip-compile-multi==2.6.3
     # via -r dev.in
-pip-tools==7.3.0
+pip-tools==7.4.1
     # via pip-compile-multi
-plumbum==1.8.2
+plumbum==1.8.3
     # via copier
-prometheus-client==0.19.0
+prometheus-client==0.20.0
     # via jupyter-server
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==2.5.3
+pydantic==2.7.1
     # via copier
-pydantic-core==2.14.6
+pydantic-core==2.18.2
     # via pydantic
 python-json-logger==2.0.7
     # via jupyter-events
-pyyaml-include==1.3.2
-    # via copier
-questionary==2.0.1
+questionary==1.10.0
     # via copier
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-send2trash==1.8.2
+send2trash==1.8.3
     # via jupyter-server
-sniffio==1.3.0
-    # via anyio
-terminado==0.18.0
+sniffio==1.3.1
+    # via
+    #   anyio
+    #   httpx
+terminado==0.18.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
 toposort==1.10
     # via pip-compile-multi
-types-docutils==0.20.0.20240106
+types-docutils==0.21.0.20240423
     # via -r dev.in
-types-python-dateutil==2.8.19.20240106
+types-python-dateutil==2.9.0.20240316
     # via arrow
-types-requests==2.31.0.20240106
+types-requests==2.32.0.20240523
     # via -r dev.in
 uri-template==1.3.0
     # via jsonschema
 webcolors==1.13
     # via jsonschema
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via jupyter-server
-wheel==0.42.0
+wheel==0.43.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `scippneutron-24.3.0/requirements/docs.txt` & `scippneutron-24.5.0/requirements/docs.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,159 +2,188 @@
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
 alabaster==0.7.16
     # via sphinx
+asttokens==2.4.1
+    # via stack-data
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   nbconvert
     #   pydata-sphinx-theme
 bleach==6.1.0
     # via nbconvert
-comm==0.2.1
+comm==0.2.2
     # via ipykernel
-debugpy==1.8.0
+debugpy==1.8.1
     # via ipykernel
+decorator==5.1.1
+    # via ipython
 defusedxml==0.7.1
     # via nbconvert
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   nbsphinx
     #   pybtex-docutils
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinxcontrib-bibtex
+exceptiongroup==1.2.1
+    # via ipython
+executing==2.0.1
+    # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==7.0.1
-    # via
-    #   jupyter-client
-    #   nbconvert
-    #   sphinx
-    #   sphinxcontrib-bibtex
-ipykernel==6.29.0
+ipykernel==6.29.4
     # via -r docs.in
-jinja2==3.1.3
+ipython==8.24.0
+    # via
+    #   -r docs.in
+    #   ipykernel
+jedi==0.19.1
+    # via ipython
+jinja2==3.1.4
     # via
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbconvert
     #   nbformat
 jupyterlab-pygments==0.3.0
     # via nbconvert
-latexcodec==2.0.1
+latexcodec==3.0.0
     # via pybtex
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.4
+markupsafe==2.1.5
     # via
     #   jinja2
     #   nbconvert
-mdit-py-plugins==0.4.0
+matplotlib-inline==0.1.7
+    # via
+    #   ipykernel
+    #   ipython
+mdit-py-plugins==0.4.1
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mistune==3.0.2
     # via nbconvert
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via -r docs.in
-nbclient==0.9.0
+nbclient==0.10.0
     # via nbconvert
-nbconvert==7.14.2
+nbconvert==7.16.4
     # via nbsphinx
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   nbclient
     #   nbconvert
     #   nbsphinx
-nbsphinx==0.9.3
+nbsphinx==0.9.4
     # via -r docs.in
 nest-asyncio==1.6.0
     # via ipykernel
 pandocfilters==1.5.1
     # via nbconvert
+parso==0.8.4
+    # via jedi
+pexpect==4.9.0
+    # via ipython
+prompt-toolkit==3.0.43
+    # via ipython
 psutil==5.9.8
     # via ipykernel
+ptyprocess==0.7.0
+    # via pexpect
+pure-eval==0.2.2
+    # via stack-data
 pybtex==0.24.0
     # via
     #   pybtex-docutils
     #   sphinxcontrib-bibtex
 pybtex-docutils==1.0.3
     # via sphinxcontrib-bibtex
 pydata-sphinx-theme==0.15.2
     # via -r docs.in
+pygments==2.18.0
+    # via
+    #   accessible-pygments
+    #   ipython
+    #   nbconvert
+    #   pydata-sphinx-theme
+    #   sphinx
 pyyaml==6.0.1
     # via
     #   myst-parser
     #   pybtex
-pyzmq==25.1.2
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
-referencing==0.32.1
+referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
-rpds-py==0.17.1
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   -r docs.in
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
     #   sphinx-copybutton
     #   sphinx-design
     #   sphinxcontrib-bibtex
-sphinx-autodoc-typehints==1.25.2
+sphinx-autodoc-typehints==2.1.0
     # via -r docs.in
 sphinx-copybutton==0.5.2
     # via -r docs.in
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via -r docs.in
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-bibtex==2.6.2
     # via -r docs.in
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
@@ -162,19 +191,39 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-tinycss2==1.2.1
+stack-data==0.6.3
+    # via ipython
+tinycss2==1.3.0
     # via nbconvert
+tomli==2.0.1
+    # via sphinx
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-typing-extensions==4.9.0
-    # via pydata-sphinx-theme
+traitlets==5.14.3
+    # via
+    #   comm
+    #   ipykernel
+    #   ipython
+    #   jupyter-client
+    #   jupyter-core
+    #   matplotlib-inline
+    #   nbclient
+    #   nbconvert
+    #   nbformat
+    #   nbsphinx
+typing-extensions==4.12.0
+    # via
+    #   ipython
+    #   pydata-sphinx-theme
+wcwidth==0.2.13
+    # via prompt-toolkit
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
```

### Comparing `scippneutron-24.3.0/requirements/make_base.py` & `scippneutron-24.5.0/requirements/make_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-# SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
-from typing import List
 
 import tomli
 
 parser = ArgumentParser()
 parser.add_argument(
     "--nightly",
     default="",
@@ -19,15 +15,15 @@
 
 CUSTOM_AUTO_SEPARATOR = """
 # --- END OF CUSTOM SECTION ---
 # The following was generated by 'tox -e deps', DO NOT EDIT MANUALLY!
 """
 
 
-def write_dependencies(dependency_name: str, dependencies: List[str]) -> None:
+def write_dependencies(dependency_name: str, dependencies: list[str]) -> None:
     path = Path(f"{dependency_name}.in")
     if path.exists():
         sections = path.read_text().split(CUSTOM_AUTO_SEPARATOR)
         if len(sections) > 1:
             custom = sections[0]
         else:
             custom = ""
@@ -39,15 +35,15 @@
         f.write("\n".join(dependencies))
         f.write("\n")
 
 
 with open("../pyproject.toml", "rb") as toml_file:
     pyproject = tomli.load(toml_file)
     dependencies = pyproject["project"].get("dependencies")
-    if not dependencies:
+    if dependencies is None:
         raise RuntimeError("No dependencies found in pyproject.toml")
     dependencies = [dep.strip().strip('"') for dep in dependencies]
 
 write_dependencies("base", dependencies)
 
 
 def as_nightly(repo: str) -> str:
```

### Comparing `scippneutron-24.3.0/resources/logo-2022.svg` & `scippneutron-24.5.0/resources/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/src/scippneutron/__init__.py` & `scippneutron-24.5.0/src/scippneutron/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
-# flake8: noqa
+# Copyright (c) 2024 Scipp contributors (https://github.com/scipp)
+# ruff: noqa: E402, F401
+
 """Neutron scattering toolkit built using scipp for Data Reduction.
 
 ScippNeutron is a generic (as in 'usable by different facilities')
 package for data processing in neutron scattering.
 It provides coordinate transformations, file I/O, and technique-specific tools.
 
 See the online documentation for user guides and the API reference:
```

### Comparing `scippneutron-24.3.0/src/scippneutron/_utils/__init__.py` & `scippneutron-24.5.0/src/scippneutron/_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
 """
 Internal utilities; do not use outside scippneutron!
 """
 
-from typing import MutableMapping
+from collections.abc import MutableMapping
 
 import scipp as sc
 from scipp.typing import VariableLike
 
 
 def elem_unit(var: VariableLike) -> sc.Unit:
     return var.bins.unit if var.bins is not None else var.unit
```

### Comparing `scippneutron-24.3.0/src/scippneutron/atoms/__init__.py` & `scippneutron-24.5.0/src/scippneutron/atoms/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """Parameters for neutron interactions with atoms."""
+
 from __future__ import annotations
 
 import dataclasses
 import importlib.resources
 from functools import lru_cache
-from typing import Optional, TextIO, Union
+from typing import TextIO
 
 import scipp as sc
 
 
 def reference_wavelength() -> sc.Variable:
     """Return the reference wavelength for absorption cross-sections.
 
@@ -36,43 +37,43 @@
     The absorption cross-section applies to neutrons with a wavelength
     of 1.7982 Å.
     See :func:`reference_wavelength`.
     """
 
     isotope: str
     """Element / isotope name."""
-    coherent_scattering_length_re: Optional[sc.Variable]
+    coherent_scattering_length_re: sc.Variable | None
     """Bound coherent scattering length (real part)."""
-    coherent_scattering_length_im: Optional[sc.Variable]
+    coherent_scattering_length_im: sc.Variable | None
     """Bound coherent scattering length (imaginary part)."""
-    incoherent_scattering_length_re: Optional[sc.Variable]
+    incoherent_scattering_length_re: sc.Variable | None
     """Bound incoherent scattering length (real part)."""
-    incoherent_scattering_length_im: Optional[sc.Variable]
+    incoherent_scattering_length_im: sc.Variable | None
     """Bound incoherent scattering length (imaginary part)."""
-    coherent_scattering_cross_section: Optional[sc.Variable]
+    coherent_scattering_cross_section: sc.Variable | None
     """Bound coherent scattering cross-section."""
-    incoherent_scattering_cross_section: Optional[sc.Variable]
+    incoherent_scattering_cross_section: sc.Variable | None
     """Bound incoherent scattering cross-section."""
-    total_scattering_cross_section: Optional[sc.Variable]
+    total_scattering_cross_section: sc.Variable | None
     """Total bound scattering cross-section."""
-    absorption_cross_section: Optional[sc.Variable]
+    absorption_cross_section: sc.Variable | None
     """Absorption cross-section for λ = 1.7982 Å neutrons."""
 
-    def __eq__(self, other: object) -> Union[bool, type(NotImplemented)]:
+    def __eq__(self, other: object) -> bool | type(NotImplemented):
         if not isinstance(other, ScatteringParams):
             return NotImplemented
         return all(
             self.isotope == other.isotope
             if field.name == 'isotope'
             else _eq_or_identical(getattr(self, field.name), getattr(other, field.name))
             for field in dataclasses.fields(self)
         )
 
     @staticmethod
-    @lru_cache()
+    @lru_cache
     def for_isotope(isotope: str) -> ScatteringParams:
         """Return the scattering parameters for the given element / isotope.
 
         Parameters
         ----------
         isotope:
             Name of the element or isotope.
@@ -112,19 +113,19 @@
             line[10], line[11], 'barn'
         ),
         total_scattering_cross_section=_assemble_scalar(line[12], line[13], 'barn'),
         absorption_cross_section=_assemble_scalar(line[14], line[15], 'barn'),
     )
 
 
-def _assemble_scalar(value: str, std: str, unit: str) -> Optional[sc.Variable]:
+def _assemble_scalar(value: str, std: str, unit: str) -> sc.Variable | None:
     if not value:
         return None
     value = float(value)
     variance = float(std) ** 2 if std else None
     return sc.scalar(value, variance=variance, unit=unit)
 
 
-def _eq_or_identical(a: Optional[sc.Variable], b: Optional[sc.Variable]) -> bool:
+def _eq_or_identical(a: sc.Variable | None, b: sc.Variable | None) -> bool:
     if a is None:
         return b is None
     return sc.identical(a, b)
```

### Comparing `scippneutron-24.3.0/src/scippneutron/atoms/scattering_parameters.csv` & `scippneutron-24.5.0/src/scippneutron/atoms/scattering_parameters.csv`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/src/scippneutron/beamline_components.py` & `scippneutron-24.5.0/src/scippneutron/beamline_components.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
-from typing import Union
 
 import scipp as sc
 
 from .conversion import graph
 
 
 def _derived_coord(
-    da: Union[sc.DataArray, sc.Dataset], name: str, scatter: bool = True
+    da: sc.DataArray | sc.Dataset, name: str, scatter: bool = True
 ) -> sc.Variable:
     tmp = da.transform_coords(
         name,
         graph=graph.beamline.beamline(scatter=scatter),
         rename_dims=False,
         keep_aliases=False,
         keep_inputs=False,
         keep_intermediate=False,
     )
     return tmp.coords[name]
 
 
-def position(da: Union[sc.DataArray, sc.Dataset]) -> sc.Variable:
+def position(da: sc.DataArray | sc.Dataset) -> sc.Variable:
     """Extract the detector pixel positions from a data array or dataset.
 
     Parameters
     ----------
     da:
         Get or compute the positions from coords and attrs of this.
 
@@ -34,15 +33,15 @@
     -------
     :
         The detector pixel positions.
     """
     return _derived_coord(da, 'position')
 
 
-def source_position(da: Union[sc.DataArray, sc.Dataset]) -> sc.Variable:
+def source_position(da: sc.DataArray | sc.Dataset) -> sc.Variable:
     """Extract the position of the neutron source from a data array or dataset.
 
     Parameters
     ----------
     da:
         Get or compute the source position from coords and attrs of this.
 
@@ -50,15 +49,15 @@
     -------
     :
         The source position.
     """
     return _derived_coord(da, 'source_position')
 
 
-def sample_position(da: Union[sc.DataArray, sc.Dataset]) -> sc.Variable:
+def sample_position(da: sc.DataArray | sc.Dataset) -> sc.Variable:
     """Extract the position of the sample from a data array or dataset.
 
     Parameters
     ----------
     da:
         Get or compute the sample position from coords and attrs of this.
 
@@ -66,15 +65,15 @@
     -------
     :
         The sample position.
     """
     return _derived_coord(da, 'sample_position')
 
 
-def incident_beam(da: Union[sc.DataArray, sc.Dataset]) -> sc.Variable:
+def incident_beam(da: sc.DataArray | sc.Dataset) -> sc.Variable:
     """Extract the incident beam vector from a data array or dataset.
 
     This is the direction and length of the primary flight path,
     i.e. from source to sample.
 
     Parameters
     ----------
@@ -85,15 +84,15 @@
     -------
     :
         The incident beam.
     """
     return _derived_coord(da, 'incident_beam')
 
 
-def scattered_beam(da: Union[sc.DataArray, sc.Dataset]) -> sc.Variable:
+def scattered_beam(da: sc.DataArray | sc.Dataset) -> sc.Variable:
     """Extract the scattered beam vector from a data array or dataset.
 
     This is the direction and length of the secondary flight path,
     i.e. from sample to detector.
 
     Parameters
     ----------
@@ -104,15 +103,15 @@
     -------
     :
         The scattered beam.
     """
     return _derived_coord(da, 'scattered_beam')
 
 
-def Ltotal(da: Union[sc.DataArray, sc.Dataset], scatter: bool) -> sc.Variable:
+def Ltotal(da: sc.DataArray | sc.Dataset, scatter: bool) -> sc.Variable:
     """Extract the length of the total flight path from a data array or dataset.
 
     Parameters
     ----------
     da:
         Get or compute the total flight path length from coords and attrs of this.
     scatter:
@@ -124,15 +123,15 @@
     -------
     :
         The length of the total flight path.
     """
     return _derived_coord(da, 'Ltotal', scatter=scatter)
 
 
-def L1(da: Union[sc.DataArray, sc.Dataset]) -> sc.Variable:
+def L1(da: sc.DataArray | sc.Dataset) -> sc.Variable:
     """Extract the length of the primary flight path from a data array or dataset.
 
     This is the distance between neutron source and sample.
 
     Parameters
     ----------
     da:
@@ -142,15 +141,15 @@
     -------
     :
         The length of the primary flight path.
     """
     return _derived_coord(da, 'L1')
 
 
-def L2(da: Union[sc.DataArray, sc.Dataset]) -> sc.Variable:
+def L2(da: sc.DataArray | sc.Dataset) -> sc.Variable:
     """Extract the length of the secondary flight path from a data array or dataset.
 
     This is the distance between sample and detector.
 
     Parameters
     ----------
     da:
@@ -160,15 +159,15 @@
     -------
     :
         The length of the secondary flight path.
     """
     return _derived_coord(da, 'L2')
 
 
-def two_theta(da: Union[sc.DataArray, sc.Dataset]) -> sc.Variable:
+def two_theta(da: sc.DataArray | sc.Dataset) -> sc.Variable:
     """Extract the scattering angle from a data array or dataset.
 
     The angle is defined as in Bragg's law.
     See the beamline `documentation <../modules/scippneutron.conversion.beamline.rst>`_
     for a full definition.
 
     Parameters
```

### Comparing `scippneutron-24.3.0/src/scippneutron/conversion/__init__.py` & `scippneutron-24.5.0/src/scippneutron/conversion/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
 
-# flake8: noqa[F401]
 """Components for coordinate transformations.
 
 The submodules are mainly intended for constructing graphs for
 :func:`scipp.transform_coords` but can also be used independently.
 
 ``beamline`` and ``tof`` contain individual transformation kernels.
 ``graph`` contains concrete graphs that can be passed to ``transform_coords``.
 
 See also the user guide on
 `Coordinate Transformations <../../user-guide/coordinate-transformations.rst>`_.
 """
 
 from . import beamline, tof
+
+__all__ = ['beamline', 'tof']
```

### Comparing `scippneutron-24.3.0/src/scippneutron/conversion/beamline.py` & `scippneutron-24.5.0/src/scippneutron/conversion/beamline.py`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/src/scippneutron/conversion/graph/__init__.py` & `scippneutron-24.5.0/src/scippneutron/conversion/graph/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
 
-# flake8: noqa[F401]
 """Graphs for coordinate transformations.
 
 All graphs are defined in terms of the functions in the parent module
 :mod:`scippneutron.conversion`.
 See there for definitions of the individual conversions.
 
 Typically, multiple graphs need to be combined for a full transformation.
@@ -17,7 +16,9 @@
     ...                     **graph.tof.elastic_wavelength(start='tof')}
 
 The `user guide <../../user-guide/coordinate-transformations.rst>`_ gives
 more examples.
 """
 
 from . import beamline, tof
+
+__all__ = ['beamline', 'tof']
```

### Comparing `scippneutron-24.3.0/src/scippneutron/conversion/graph/beamline.py` & `scippneutron-24.5.0/src/scippneutron/conversion/graph/beamline.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # @author Jan-Lukas Wynen
 """Graphs for computing beamline parameters from positions.
 
 See :mod:`scippneutron.conversion.beamline` for definitions
 of the quantities used here.
 """
 
-from typing import Callable, Dict
+from collections.abc import Callable
 
 from .. import beamline as _kernels
 
-Graph = Dict[str, Callable]
+Graph = dict[str, Callable]
 
 
 def incident_beam() -> Graph:
     """Graph for computing 'incident_beam'.
 
     Returns
     -------
```

### Comparing `scippneutron-24.3.0/src/scippneutron/conversion/graph/tof.py` & `scippneutron-24.5.0/src/scippneutron/conversion/graph/tof.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 - can be used to compute a specific coordinate as identified by the function name
   (e.g. ``elastic_energy``) from a given coordinate as given by the ``start`` argument.
   These graphs may contain more than one node if necessary.
 - can be used to compute multiple coordinates, (``elastic`` and ``kinematic``).
   Their ``start`` argument works as in the other functions.
 """
 
-from typing import Callable, Dict
+from collections.abc import Callable
 
 from .. import tof as _kernels
 
-Graph = Dict[str, Callable]
+Graph = dict[str, Callable]
 
 _GRAPH_DYNAMICS_BY_ORIGIN = {
     'energy': {
         'dspacing': _kernels.dspacing_from_energy,
         'wavelength': _kernels.wavelength_from_energy,
     },
     'tof': {
```

### Comparing `scippneutron-24.3.0/src/scippneutron/conversion/tof.py` & `scippneutron-24.5.0/src/scippneutron/conversion/tof.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 """Functions for computing coordinates in time-of-flight neutron scattering.
 
 Some functions in this module use the neutron mass :math:`m_n`
 and Planck constant :math:`h`.
 Their values are taken from :mod:`scipp.constants`.
 """
 
-from typing import Tuple
-
 import numpy as np
 import scipp as sc
 import scipp.constants as const
 from scipp.typing import Variable, VariableLike
 
 from .._utils import as_float_type, elem_dtype, elem_unit
 
@@ -379,15 +377,15 @@
     return sc.to_unit(
         _wavelength_Q_conversions(Q, two_theta), unit='angstrom', copy=False
     )
 
 
 def Q_elements_from_wavelength(
     *, wavelength: Variable, incident_beam: Variable, scattered_beam: Variable
-) -> Tuple[Variable, Variable, Variable]:
+) -> tuple[Variable, Variable, Variable]:
     r"""Compute them momentum transfer vector from wavelength.
 
     Computes the three components of the Q-vector :math:`Q_x, Q_y, Q_z`
     separately using
 
     .. math::
 
@@ -636,15 +634,15 @@
     # This function uses implementation 3 as the performance gain
     # is expected to be significant over 1 and 2.
     return (sc.spatial.inv(sample_rotation * ub_matrix) * Q_vec) / (2 * np.pi)
 
 
 def hkl_elements_from_hkl_vec(
     *, hkl_vec: Variable
-) -> Tuple[Variable, Variable, Variable]:
+) -> tuple[Variable, Variable, Variable]:
     """Unpack vector of hkl indices into separate variables.
 
     Parameters
     ----------
     hkl_vec:
         Vector of hkl indices.
```

### Comparing `scippneutron-24.3.0/src/scippneutron/core/conversions.py` & `scippneutron-24.5.0/src/scippneutron/core/conversions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
 
-from typing import Callable, Dict, Tuple, Union
+from collections.abc import Callable
 
 import scipp as sc
 
 from ..conversion import graph as _graphs
 
 
 def _inelastic_scatter_graph(energy_mode):
@@ -41,15 +41,15 @@
         else _inelastic_scatter_graph(energy_mode)
     )
     return graph
 
 
 def conversion_graph(
     origin: str, target: str, scatter: bool, energy_mode: str
-) -> Dict[Union[str, Tuple[str]], Callable]:
+) -> dict[str | tuple[str], Callable]:
     """
     Get a conversion graph for given parameters.
 
     The graph can be used with `scipp.transform_coords`.
 
     :param origin: Name of the input coordinate.
     :param target: Name of the output coordinate.
@@ -101,16 +101,16 @@
                 f"({inelastic_inputs}) but conversion with elastic energy requested. "
                 f"This is not implemented."
             )
     return 'elastic'
 
 
 def deduce_conversion_graph(
-    data: Union[sc.DataArray, sc.Dataset], origin: str, target: str, scatter: bool
-) -> Dict[Union[str, Tuple[str]], Callable]:
+    data: sc.DataArray | sc.Dataset, origin: str, target: str, scatter: bool
+) -> dict[str | tuple[str], Callable]:
     """
     Get the conversion graph used by :py:func:`scippneutron.convert`
     when called with identical arguments.
 
     :param data: Input data.
     :param origin: Name of the input coordinate.
     :param target: Name of the output coordinate.
@@ -120,16 +120,16 @@
     """
     return conversion_graph(
         origin, target, scatter, _deduce_energy_mode(data, origin, target)
     )
 
 
 def convert(
-    data: Union[sc.DataArray, sc.Dataset], origin: str, target: str, scatter: bool
-) -> Union[sc.DataArray, sc.Dataset]:
+    data: sc.DataArray | sc.Dataset, origin: str, target: str, scatter: bool
+) -> sc.DataArray | sc.Dataset:
     """
     Perform a unit conversion from the given origin unit to target.
     See the documentation page on "Coordinate Transformations"
     (https://scipp.github.io/scippneutron/user-guide/coordinate-transformations.html)
     for more details.
 
     :param data: Input data.
@@ -147,14 +147,14 @@
     try:
         converted = data.transform_coords(target, graph=graph)
     except KeyError as err:
         if err.args[0] == target:
             raise RuntimeError(
                 f"No viable conversion from '{origin}' to '{target}' "
                 f"with scatter={scatter}."
-            )
+            ) from None
         raise RuntimeError(
             f"Missing coordinate '{err.args[0]}' for conversion "
             f"from '{origin}' to '{target}'"
         ) from None
 
     return converted
```

### Comparing `scippneutron-24.3.0/src/scippneutron/data/__init__.py` & `scippneutron-24.5.0/src/scippneutron/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/src/scippneutron/data_streaming/_consumer.py` & `scippneutron-24.5.0/src/scippneutron/data_streaming/_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,19 @@
   comprises one or more partitions.
 - The "offset" is the index of the message in a partition on the
   Kafka broker. Old messages are deleted from the partition, so the
   first available message may not be at offset 0.
 """
 
 import multiprocessing as mp
+import multiprocessing.queues
 import threading
+from collections.abc import Callable
 from queue import Empty as QueueEmpty
 from time import time_ns
-from typing import Callable, List, Optional, Tuple, Union
 from warnings import warn
 
 import numpy as np
 from confluent_kafka import Consumer, KafkaError, TopicPartition
 from streaming_data_types.exceptions import WrongSchemaException
 from streaming_data_types.run_start_pl72 import RunStartInfo, deserialise_pl72
 
@@ -39,26 +40,26 @@
 
 class FakeConsumer:
     """
     Use in place of confluent_kafka.Consumer
     to avoid network io in unit tests
     """
 
-    def __init__(self, input_queue: Optional[mp.Queue]):
+    def __init__(self, input_queue: mp.queues.Queue | None):
         if input_queue is None:
             raise RuntimeError(
                 "A multiprocessing queue for test messages "
                 "must be provided when using FakeConsumer"
             )
         # This queue is used to provide the consumer with
         # messages in unit tests, instead of it getting messages
         # from the Kafka broker
         self._input_queue = input_queue
 
-    def assign(self, topic_partitions: List[TopicPartition]):
+    def assign(self, topic_partitions: list[TopicPartition]):
         pass
 
     def poll(self, timeout: float):
         try:
             msg = self._input_queue.get(timeout=0.1)
             return msg
         except QueueEmpty:
@@ -68,32 +69,32 @@
         pass
 
 
 class KafkaConsumer:
     def __init__(
         self,
         topic_partition: TopicPartition,
-        consumer: Union[Consumer, FakeConsumer],
+        consumer: Consumer | FakeConsumer,
         callback: Callable,
-        stop_time_ms: Optional[int] = None,
+        stop_time_ms: int | None = None,
     ):
         self._consumer = consumer
         # To consume messages the consumer must "subscribe" to one
         # or more topics or "assign" specific topic partitions, the
         # latter allows us to start consuming at an offset specified
         # in the TopicPartition. Each KafkaConsumer consumes from only
         # a single partition, this simplifies the logic around run stop
         # behaviour.
         # Note that offsets are integer indices pointing to a position in the
         # topic partition, they are not a bytes offset.
         self._consumer.assign([topic_partition])
         self._callback = callback
         self._reached_eop = False
         self.cancelled = False
-        self._consume_data: Optional[threading.Thread] = None
+        self._consume_data: threading.Thread | None = None
         self.stopped = True
         self._stop_time_mutex = threading.Lock()
         # default stop time to distant future (run until manually stopped)
         self._stop_time = np.iinfo(np.int64).max
         if stop_time_ms is not None:
             self._stop_time = stop_time_ms
 
@@ -137,15 +138,15 @@
                     if reached_stop_time:
                         # Wall clock time is after run stop time and there
                         # are no more messages available on Kafka for us to
                         # consume, so cancel running the consumer.
                         self.cancelled = True
                         break
                     continue
-                warn(f"Message error in consumer: {msg.error()}")
+                warn(f"Message error in consumer: {msg.error()}", stacklevel=3)
                 self.cancelled = True
                 break
 
             at_end_of_partition = False
             with self._stop_time_mutex:
                 if msg.timestamp()[1] > self._stop_time:
                     reached_message_after_stop_time = True
@@ -212,37 +213,37 @@
 
     def poll(self, timeout=2.0):
         """
         Poll for a message from Kafka
         """
         return self._consumer.poll(timeout=timeout)
 
-    def get_watermark_offsets(self, partition: TopicPartition) -> Tuple[int, int]:
+    def get_watermark_offsets(self, partition: TopicPartition) -> tuple[int, int]:
         """
         Get the offset of the first and last available
         message in the given partition
         """
         return self._consumer.get_watermark_offsets(partition, cached=False)
 
-    def assign(self, partitions: List[TopicPartition]):
+    def assign(self, partitions: list[TopicPartition]):
         self._consumer.assign(partitions)
 
-    def offsets_for_times(self, partitions: List[TopicPartition]):
+    def offsets_for_times(self, partitions: list[TopicPartition]):
         return self._consumer.offsets_for_times(partitions)
 
 
 def create_consumers(
     start_time_ms: int,
-    stop_time_ms: Optional[int],
-    topics: List[str],
+    stop_time_ms: int | None,
+    topics: list[str],
     kafka_broker: str,
     consumer_type_enum: ConsumerType,  # so we can inject fake consumer
     callback: Callable,
-    test_message_queue: Optional[mp.Queue],
-) -> List[KafkaConsumer]:
+    test_message_queue: mp.queues.Queue | None,
+) -> list[KafkaConsumer]:
     """
     Creates one consumer per TopicPartition that start consuming
     at specified timestamp in the data stream
 
     Having each consumer only be responsible for one partition
     greatly simplifies the logic around stopping at the end of
     the stream (making use of "end of partition" event)
@@ -287,25 +288,25 @@
                 stop_time_ms,
             )
         ]
 
     return consumers
 
 
-def start_consumers(consumers: List[KafkaConsumer]):
+def start_consumers(consumers: list[KafkaConsumer]):
     for consumer in consumers:
         consumer.start()
 
 
-def stop_consumers(consumers: List[KafkaConsumer]):
+def stop_consumers(consumers: list[KafkaConsumer]):
     for consumer in consumers:
         consumer.stop()
 
 
-def all_consumers_stopped(consumers: List[KafkaConsumer]) -> bool:
+def all_consumers_stopped(consumers: list[KafkaConsumer]) -> bool:
     for consumer in consumers:
         if not consumer.stopped:
             # if the consumer is cancelled then cleanly stop it
             # (join the thread)
             if consumer.cancelled:
                 consumer.stop()
                 continue
```

### Comparing `scippneutron-24.3.0/src/scippneutron/data_streaming/_data_buffer.py` & `scippneutron-24.5.0/src/scippneutron/data_streaming/_data_buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 import multiprocessing as mp
+import multiprocessing.queues
 import threading
+from collections.abc import Callable
 from datetime import datetime
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any
 
 import numpy as np
 import scipp as sc
 from streaming_data_types.eventdata_ev42 import deserialise_ev42
 from streaming_data_types.exceptions import WrongSchemaException
 from streaming_data_types.logdata_f142 import LogDataInfo, deserialise_f142
 from streaming_data_types.run_stop_6s4t import deserialise_6s4t
@@ -81,15 +83,15 @@
         with self._buffer_mutex:
             self._data_array[self._name, self._buffer_filled_size] = log_event.value
             self._data_array.coords["time"][
                 self._name, self._buffer_filled_size
             ].value = np.datetime64(log_event.timestamp_unix_ns, 'ns')
             self._buffer_filled_size += 1
 
-    def get_metadata_array(self) -> Tuple[bool, sc.Variable]:
+    def get_metadata_array(self) -> tuple[bool, sc.Variable]:
         """
         Copy collected data from the buffer
         """
         with self._buffer_mutex:
             return_array = self._data_array[
                 self._name, : self._buffer_filled_size
             ].copy()
@@ -103,15 +105,17 @@
     Buffer for "fast" changing metadata from Kafka messages serialised
     according to the flatbuffer schema with id FAST_FB_ID.
     Typical data sources are sample environment apparatus with relatively
     rapidly values which, for efficiency, publish updates directly to Kafka
     rather than via EPICS and the Forwarder.
     """
 
-    def __init__(self, stream_info: StreamInfo, buffer_size: int, data_queue: mp.Queue):
+    def __init__(
+        self, stream_info: StreamInfo, buffer_size: int, data_queue: mp.queues.Queue
+    ):
         self._buffer_mutex = threading.Lock()
         self._buffer_size = buffer_size
         self._name = stream_info.source_name
         self._data_queue = data_queue
         self._buffer_filled_size = 0
         self._data_array = _create_metadata_buffer_array(
             self._name, stream_info.unit, stream_info.dtype, buffer_size
@@ -178,15 +182,15 @@
                     )
             self._data_array[
                 self._name,
                 self._buffer_filled_size : self._buffer_filled_size + message_size,
             ].coords["time"].values = timestamps
             self._buffer_filled_size += message_size
 
-    def get_metadata_array(self) -> Tuple[bool, sc.Variable]:
+    def get_metadata_array(self) -> tuple[bool, sc.Variable]:
         """
         Copy collected data from the buffer
         """
         with self._buffer_mutex:
             return_array = self._data_array[
                 self._name, : self._buffer_filled_size
             ].copy()
@@ -197,15 +201,17 @@
 
 class _ChopperMetadataBuffer:
     """
     Buffer for chopper top-dead-centre timestamps from Kafka messages
     serialised according to the flatbuffer schema with id CHOPPER_FB_ID.
     """
 
-    def __init__(self, stream_info: StreamInfo, buffer_size: int, data_queue: mp.Queue):
+    def __init__(
+        self, stream_info: StreamInfo, buffer_size: int, data_queue: mp.queues.Queue
+    ):
         self._buffer_mutex = threading.Lock()
         self._buffer_size = buffer_size
         self._name = stream_info.source_name
         self._data_queue = data_queue
         self._buffer_filled_size = 0
         self._data_array = sc.zeros(
             dims=[self._name],
@@ -235,31 +241,29 @@
         with self._buffer_mutex:
             self._data_array[
                 self._name,
                 self._buffer_filled_size : self._buffer_filled_size + message_size,
             ].values = chopper_timestamps.timestamps
             self._buffer_filled_size += message_size
 
-    def get_metadata_array(self) -> Tuple[bool, sc.Variable]:
+    def get_metadata_array(self) -> tuple[bool, sc.Variable]:
         """
         Copy collected data from the buffer
         """
         with self._buffer_mutex:
             return_array = self._data_array[
                 self._name, : self._buffer_filled_size
             ].copy()
             new_data_exists = self._buffer_filled_size != 0
             self._buffer_filled_size = 0
         return new_data_exists, sc.scalar(return_array)
 
 
 metadata_ids = (SLOW_FB_ID, FAST_FB_ID, CHOPPER_FB_ID)
-_MetadataBuffer = Union[
-    _FastMetadataBuffer, _SlowMetadataBuffer, _ChopperMetadataBuffer
-]
+_MetadataBuffer = _FastMetadataBuffer | _SlowMetadataBuffer | _ChopperMetadataBuffer
 
 
 class StreamedDataBuffer:
     """
     This owns the buffers for data consumed from Kafka.
     It periodically emits accumulated data to a queue
     and resets the buffer. If a buffer fills up within the emit time
@@ -267,15 +271,15 @@
 
     TODO: This also owns the metadata buffers. Maybe this should be moved to a
     separate place in the future?
     """
 
     def __init__(
         self,
-        queue: mp.Queue,
+        queue: mp.queues.Queue,
         event_buffer_size: int,
         slow_metadata_buffer_size: int,
         fast_metadata_buffer_size: int,
         chopper_buffer_size: int,
         interval_s: float,
         run_id: str,
     ):
@@ -315,46 +319,46 @@
                 'pulse_time': pulse_times,
             },
         )
         self._current_event = 0
         self._cancelled = False
         self._notify_cancelled = threading.Condition()
         self._unrecognised_fb_id_count = 0
-        self._periodic_emit: Optional[threading.Thread] = None
+        self._periodic_emit: threading.Thread | None = None
         self._emit_queue = queue
         # Access metadata buffer by
         # self._metadata_buffers[flatbuffer_id][source_name]
-        self._metadata_buffers: Dict[str, Dict[str, _MetadataBuffer]] = {
+        self._metadata_buffers: dict[str, dict[str, _MetadataBuffer]] = {
             flatbuffer_id: {} for flatbuffer_id in metadata_ids
         }
 
-    def init_metadata_buffers(self, stream_info: List[StreamInfo]):
+    def init_metadata_buffers(self, stream_info: list[StreamInfo]):
         """
         Create a buffer for each of the metadata sources.
         This is not in the constructor which allows the StreamedDataBuffer
         to be constructed before metadata sources are extracted from the
         run start message, this means the StreamedDataBuffer can be passed
         into data_stream to facilitate unit testing.
         """
         for stream in stream_info:
             if stream.flatbuffer_id == SLOW_FB_ID:
-                self._metadata_buffers[stream.flatbuffer_id][
-                    stream.source_name
-                ] = _SlowMetadataBuffer(stream, self._slow_metadata_buffer_size)
+                self._metadata_buffers[stream.flatbuffer_id][stream.source_name] = (
+                    _SlowMetadataBuffer(stream, self._slow_metadata_buffer_size)
+                )
             elif stream.flatbuffer_id == FAST_FB_ID:
-                self._metadata_buffers[stream.flatbuffer_id][
-                    stream.source_name
-                ] = _FastMetadataBuffer(
-                    stream, self._fast_metadata_buffer_size, self._emit_queue
+                self._metadata_buffers[stream.flatbuffer_id][stream.source_name] = (
+                    _FastMetadataBuffer(
+                        stream, self._fast_metadata_buffer_size, self._emit_queue
+                    )
                 )
             elif stream.flatbuffer_id == CHOPPER_FB_ID:
-                self._metadata_buffers[stream.flatbuffer_id][
-                    stream.source_name
-                ] = _ChopperMetadataBuffer(
-                    stream, self._chopper_buffer_size, self._emit_queue
+                self._metadata_buffers[stream.flatbuffer_id][stream.source_name] = (
+                    _ChopperMetadataBuffer(
+                        stream, self._chopper_buffer_size, self._emit_queue
+                    )
                 )
             elif stream.flatbuffer_id == EVENT_FB_ID:
                 pass  # detection events, not metadata
             else:
                 self._emit_queue.put(
                     UnknownFlatbufferIdWarning(
                         f"Stream in run start message specified flatbuffer id "
@@ -385,15 +389,15 @@
                         f"Received {self._unrecognised_fb_id_count}"
                         " messages with unrecognised FlatBuffer ids"
                     )
                 )
                 self._unrecognised_fb_id_count = 0
             new_data = self._events_buffer['event', : self._current_event].copy()
             new_data_exists = self._current_event != 0
-            for _, buffers in self._metadata_buffers.items():
+            for buffers in self._metadata_buffers.values():
                 for name, buffer in buffers.items():
                     (new_metadata_exists, metadata_array) = buffer.get_metadata_array()
                     new_data.attrs[name] = metadata_array
                     if new_metadata_exists:
                         new_data_exists = True
             self._current_event = 0
         if new_data_exists:
@@ -426,18 +430,17 @@
                 self._emit_data()
             with self._buffer_mutex:
                 frame = self._events_buffer[
                     'event', self._current_event : self._current_event + message_size
                 ]
                 frame.coords['detector_id'].values = deserialised_data.detector_id
                 frame.coords['tof'].values = deserialised_data.time_of_flight
-                frame.coords[
-                    'pulse_time'
-                ].values = deserialised_data.pulse_time * np.ones_like(
-                    deserialised_data.time_of_flight
+                frame.coords['pulse_time'].values = (
+                    deserialised_data.pulse_time
+                    * np.ones_like(deserialised_data.time_of_flight)
                 )
                 self._current_event += message_size
         except WrongSchemaException:
             return False
         return True
 
     def _handled_metadata(
```

### Comparing `scippneutron-24.3.0/src/scippneutron/data_streaming/_data_consumption_manager.py` & `scippneutron-24.5.0/src/scippneutron/data_streaming/_data_consumption_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 import multiprocessing as mp
+import multiprocessing.queues
 from dataclasses import dataclass
 from enum import Enum
 from queue import Empty as QueueEmpty
-from typing import List, Optional
 
 from ..io.nexus.load_nexus import StreamInfo
 from ._consumer import (
     all_consumers_stopped,
     create_consumers,
     start_consumers,
     stop_consumers,
@@ -21,39 +21,39 @@
     STOP_NOW = 1
     UPDATE_STOP_TIME = 2
 
 
 @dataclass(frozen=True)
 class ManagerInstruction:
     type: InstructionType
-    stop_time_ms: Optional[int] = None  # milliseconds from unix epoch
+    stop_time_ms: int | None = None  # milliseconds from unix epoch
 
 
 def data_consumption_manager(
     start_time_ms: int,
-    stop_time_ms: Optional[int],
+    stop_time_ms: int | None,
     run_id: str,
-    topics: List[str],
+    topics: list[str],
     kafka_broker: str,
     consumer_type: ConsumerType,
-    stream_info: Optional[List[StreamInfo]],
+    stream_info: list[StreamInfo] | None,
     interval_s: float,
     event_buffer_size: int,
     slow_metadata_buffer_size: int,
     fast_metadata_buffer_size: int,
     chopper_buffer_size: int,
-    worker_instruction_queue: mp.Queue,
-    data_queue: mp.Queue,
-    test_message_queue: Optional[mp.Queue],
+    worker_instruction_queue: mp.queues.Queue,
+    data_queue: mp.queues.Queue,
+    test_message_queue: mp.queues.Queue | None,
 ):
     """
     Starts and stops buffers and data consumers which collect data and
     send them back to the main process via a queue.
 
-    All input args must be mp.Queue or pickleable as this function is launched
+    All input args must be mp.queues.Queue or pickleable as this function is launched
     as a multiprocessing.Process.
     """
     buffer = StreamedDataBuffer(
         data_queue,
         event_buffer_size,
         slow_metadata_buffer_size,
         fast_metadata_buffer_size,
@@ -82,14 +82,14 @@
         try:
             instruction = worker_instruction_queue.get(timeout=0.5)
             if instruction.type == InstructionType.STOP_NOW:
                 stop_consumers(consumers)
             elif instruction.type == InstructionType.UPDATE_STOP_TIME:
                 for consumer in consumers:
                     consumer.update_stop_time(instruction.stop_time_ms)
-        except QueueEmpty:
+        except QueueEmpty:  # noqa: PERF203
             pass
         except (ValueError, OSError):
             # Queue has been closed, stop worker
             stop_consumers(consumers)
 
     buffer.stop()
```

### Comparing `scippneutron-24.3.0/src/scippneutron/data_streaming/_data_stream_widget.py` & `scippneutron-24.5.0/src/scippneutron/data_streaming/_data_stream_widget.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 from datetime import datetime
-from typing import Optional
 
 
 def _unix_ms_to_datetime(unix_ms: int) -> datetime:
-    return datetime.fromtimestamp(unix_ms / 1000.0)
+    return datetime.fromtimestamp(unix_ms / 1000.0, tz=None)  # noqa: DTZ006
 
 
 class DataStreamWidget:
     def __init__(
         self,
-        start_time_ms: Optional[int] = None,
-        stop_time_ms: Optional[int] = None,
-        run_title: Optional[str] = None,
+        start_time_ms: int | None = None,
+        stop_time_ms: int | None = None,
+        run_title: str | None = None,
     ):
         import ipywidgets as widgets
         from IPython.display import display
 
         self._stop_button = widgets.ToggleButton(description="Stop stream")
         self._stop_button.observe(self._on_button_clicked, "value")
         self._title = widgets.Label("-")
```

### Comparing `scippneutron-24.3.0/src/scippneutron/data_streaming/_serialisation.py` & `scippneutron-24.5.0/src/scippneutron/data_streaming/_serialisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """
 Convert a Scipp DataArray to a picklable dictionary and back.
 Can be used to move DataArrays between multiprocessing.Process.
 """
 
-from typing import Any, Dict
+from typing import Any
 
 import numpy as np
 import scipp as sc
 
 _scipp_containers = ("DataArray", "DataSet", "Variable")
 
 
-def convert_to_pickleable_dict(data: sc.DataArray) -> Dict:
+def convert_to_pickleable_dict(data: sc.DataArray) -> dict:
     data_dict = sc.to_dict(data)
 
     def _unit_and_dtype_to_str(d: Any):
         for k, v in d.items():
             if isinstance(v, dict):
                 _unit_and_dtype_to_str(v)
             elif k == "unit":
@@ -31,15 +31,15 @@
                     d["values"] = sc.to_dict(d["values"])
                     _unit_and_dtype_to_str(d["values"])
 
     _unit_and_dtype_to_str(data_dict)
     return data_dict
 
 
-def convert_from_pickleable_dict(data_dict: Dict) -> sc.DataArray:
+def convert_from_pickleable_dict(data_dict: dict) -> sc.DataArray:
     def convert_from_str_unit_and_dtype(d):
         delete_dtype = False
         for k, v in d.items():
             if isinstance(v, dict):
                 convert_from_str_unit_and_dtype(v)
                 if k not in ("attrs", "masks", "coords"):
                     if {"coords", "data"}.issubset(set(v.keys())):
```

### Comparing `scippneutron-24.3.0/src/scippneutron/data_streaming/data_stream.py` & `scippneutron-24.5.0/src/scippneutron/data_streaming/data_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+from __future__ import annotations
+
 import asyncio
 import multiprocessing as mp
+import multiprocessing.queues
 import time
+from collections.abc import Generator
 from enum import Enum
 from queue import Empty as QueueEmpty
-from typing import Generator, List, Optional
 from warnings import warn
 
 import numpy as np
 import scipp as sc
 
 from ..io.nexus.load_nexus import load_nexus_json_str
 from ._consumer_type import ConsumerType
@@ -35,21 +38,21 @@
     "installation instructions (https://scipp.github.io/"
     "scippneutron/getting-started/installation.html)"
 )
 
 
 async def data_stream(
     kafka_broker: str,
-    topics: Optional[List[str]] = None,
+    topics: list[str] | None = None,
     event_buffer_size: int = 1_048_576,
     slow_metadata_buffer_size: int = 1000,
     fast_metadata_buffer_size: int = 100_000,
     chopper_buffer_size: int = 10_000,
     interval: sc.Variable = 2.0 * sc.units.s,
-    run_info_topic: Optional[str] = None,
+    run_info_topic: str | None = None,
     start_time: StartTime = StartTime.NOW,
     stop_time: StopTime = StopTime.NEVER,
 ) -> Generator[sc.DataArray, None, None]:
     """
     Periodically yields accumulated data from stream.
     If the buffer fills up more frequently than the set interval
     then data is yielded more frequently.
@@ -110,15 +113,15 @@
         event_buffer_size,
         slow_metadata_buffer_size,
         fast_metadata_buffer_size,
         chopper_buffer_size,
         run_info_topic,
         start_time,
         stop_time,
-    ):  # noqa: E125
+    ):
         yield data_chunk
 
 
 def validate_buffer_size_args(
     chopper_buffer_size,
     event_buffer_size,
     fast_metadata_buffer_size,
@@ -130,40 +133,40 @@
         ("fast_metadata_buffer_size", fast_metadata_buffer_size),
         ("chopper_buffer_size", chopper_buffer_size),
     ):
         if buffer_size < 1:
             raise ValueError(f"{buffer_name} must be greater than zero")
 
 
-def _cleanup_queue(queue: Optional[mp.Queue]):
+def _cleanup_queue(queue: mp.queues.Queue | None):
     if queue is not None:
         queue.cancel_join_thread()
         queue.close()
         queue.join_thread()
 
 
 async def _data_stream(
-    data_queue: mp.Queue,
-    worker_instruction_queue: mp.Queue,
+    data_queue: mp.queues.Queue,
+    worker_instruction_queue: mp.queues.Queue,
     kafka_broker: str,
-    topics: Optional[List[str]],
+    topics: list[str] | None,
     interval: sc.Variable,
     event_buffer_size: int,
     slow_metadata_buffer_size: int,
     fast_metadata_buffer_size: int,
     chopper_buffer_size: int,
-    run_info_topic: Optional[str] = None,
+    run_info_topic: str | None = None,
     start_at: StartTime = StartTime.NOW,
     end_at: StopTime = StopTime.NEVER,
-    query_consumer: Optional["KafkaQueryConsumer"] = None,  # noqa: F821
+    query_consumer: KafkaQueryConsumer | None = None,  # noqa: F821
     consumer_type: ConsumerType = ConsumerType.REAL,
-    halt_after_n_data_chunks: int = np.iinfo(np.int32).max,  # noqa: B008
-    halt_after_n_warnings: int = np.iinfo(np.int32).max,  # noqa: B008
-    test_message_queue: Optional[mp.Queue] = None,  # for tests
-    timeout: Optional[sc.Variable] = None,  # for tests
+    halt_after_n_data_chunks: int = np.iinfo(np.int32).max,
+    halt_after_n_warnings: int = np.iinfo(np.int32).max,
+    test_message_queue: mp.queues.Queue | None = None,  # for tests
+    timeout: sc.Variable | None = None,  # for tests
 ) -> Generator[sc.DataArray, None, None]:
     """
     Main implementation of data stream is extracted to this function so that
     fake consumers can be injected for unit tests
     """
 
     # Search backwards to find the last run_start message
@@ -171,15 +174,15 @@
         from ._consumer import KafkaQueryConsumer, get_run_start_message
         from ._data_consumption_manager import (
             InstructionType,
             ManagerInstruction,
             data_consumption_manager,
         )
     except ImportError:
-        raise ImportError(_missing_dependency_message)
+        raise ImportError(_missing_dependency_message) from None
 
     if topics is None and run_info_topic is None:
         raise ValueError(
             "At least one of 'topics' and 'run_info_topic'" " must be specified"
         )
 
     # This is defaulted to None in the function signature
@@ -292,15 +295,15 @@
                 raise TimeoutError("data_stream timed out in test")
             try:
                 new_data = data_queue.get_nowait()
 
                 if isinstance(new_data, Warning):
                     # Raise warnings in this process so that they
                     # can be captured in tests
-                    warn(new_data)
+                    warn(new_data, stacklevel=3)
                     n_warnings += 1
                     continue
                 elif isinstance(new_data, StopTimeUpdate):
                     data_stream_widget.set_stop_time(new_data.stop_time_ms)
                     if end_at == StopTime.END_OF_RUN:
                         worker_instruction_queue.put(
                             ManagerInstruction(
```

### Comparing `scippneutron-24.3.0/src/scippneutron/instrument_view.py` & `scippneutron-24.5.0/src/scippneutron/instrument_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,14 @@
     positions_var = get_meta(scipp_obj)[positions]
     if pixel_size is None:
         pos_array = positions_var.values
         if len(pos_array) > 1:
             pixel_size = np.linalg.norm(pos_array[1] - pos_array[0])
 
     fig = pp.scatter3d(scipp_obj, pos=positions, pixel_size=pixel_size, **kwargs)
-    scene = fig.children[0].canvas.scene
+    scene = fig.canvas.scene
 
     # Add additional components from the beamline
     if components:
         _plot_components(scipp_obj, components, positions_var, scene)
 
     return fig
```

### Comparing `scippneutron-24.3.0/src/scippneutron/io/cif.py` & `scippneutron-24.5.0/src/scippneutron/io/cif.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,44 +59,45 @@
   2.3 9.7 0.7071067811865476
 """
 
 from __future__ import annotations
 
 import io
 import warnings
+from collections.abc import Iterable, Mapping
 from contextlib import contextmanager
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Iterable, Mapping, Optional, Union
+from typing import Any
 
 import scipp as sc
 
 
 @dataclass(frozen=True)
 class CIFSchema:
     name: str
     version: str
     location: str
 
 
 CORE_SCHEMA = CIFSchema(
     name='coreCIF',
     version='3.3.0',
-    location='https://github.com/COMCIFS/cif_core/blob/fc3d75a298fd7c0c3cde43633f2a8616e826bfd5/cif_core.dic',  # noqa: E501
+    location='https://github.com/COMCIFS/cif_core/blob/fc3d75a298fd7c0c3cde43633f2a8616e826bfd5/cif_core.dic',
 )
 PD_SCHEMA = CIFSchema(
     name='pdCIF',
     version='2.5.0',
-    location='https://github.com/COMCIFS/Powder_Dictionary/blob/7608b92165f58f968f054344e67662e01d4b401a/cif_pow.dic',  # noqa: E501
+    location='https://github.com/COMCIFS/Powder_Dictionary/blob/7608b92165f58f968f054344e67662e01d4b401a/cif_pow.dic',
 )
 
 
 def save_cif(
-    fname: Union[str, Path, io.TextIOBase], blocks: Union[Block, Iterable[Block]]
+    fname: str | Path | io.TextIOBase, blocks: Block | Iterable[Block]
 ) -> None:
     """Save data blocks to a CIF file.
 
     To use, first create :class:`scippneutron.io.cif.Block` objects to collect and
     structure data for the file, then use this function to write the file.
 
     Parameters
@@ -123,19 +124,19 @@
 
     Note that CIF has no concept of chunks; they are only used for organizing
     data in ScippNeutron.
     """
 
     def __init__(
         self,
-        pairs: Union[Mapping[str, Any], Iterable[tuple[str, Any]], None],
+        pairs: Mapping[str, Any] | Iterable[tuple[str, Any]] | None,
         /,
         *,
         comment: str = '',
-        schema: Optional[Union[CIFSchema, Iterable[CIFSchema]]] = None,
+        schema: CIFSchema | Iterable[CIFSchema] | None = None,
     ) -> None:
         """Create a new CIF chunk.
 
         Parameters
         ----------
         pairs:
             Defines a mapping from keys (a.k.a. tags) to values.
@@ -191,20 +192,18 @@
     The strings are arbitrary and ``Loop`` can merge items from different categories
     into a single loop.
     All variables must have the same length.
     """
 
     def __init__(
         self,
-        columns: Union[
-            Mapping[str, sc.Variable], Iterable[tuple[str, sc.Variable]], None
-        ],
+        columns: Mapping[str, sc.Variable] | Iterable[tuple[str, sc.Variable]] | None,
         *,
         comment: str = '',
-        schema: Optional[Union[CIFSchema, Iterable[CIFSchema]]] = None,
+        schema: CIFSchema | Iterable[CIFSchema] | None = None,
     ) -> None:
         """Create a new CIF loop.
 
         Parameters
         ----------
         columns:
             Defines a mapping from column names (including their category)
@@ -263,15 +262,16 @@
             File handle.
         """
         _write_comment(f, self.comment)
         f.write('loop_\n')
         for key in self._columns:
             f.write(f'_{key}\n')
         formatted_values = [
-            tuple(map(_format_value, row)) for row in zip(*self._columns.values())
+            tuple(map(_format_value, row))
+            for row in zip(*self._columns.values(), strict=True)
         ]
         # If any value is a multi-line string, lay out elements as a flat vertical
         # list, otherwise use a 2d table.
         sep = (
             '\n'
             if any(';' in item for row in formatted_values for item in row)
             else ' '
@@ -288,18 +288,18 @@
     and chunks (groups of key-value-pairs).
     The contents are written to file in the order specified in the block.
     """
 
     def __init__(
         self,
         name: str,
-        content: Optional[Iterable[Union[Mapping[str, Any], Loop, Chunk]]] = None,
+        content: Iterable[Mapping[str, Any] | Loop | Chunk] | None = None,
         *,
         comment: str = '',
-        schema: Optional[Union[CIFSchema, Iterable[CIFSchema]]] = None,
+        schema: CIFSchema | Iterable[CIFSchema] | None = None,
     ) -> None:
         """Create a new CIF data block.
 
         Parameters
         ----------
         name:
             Name of the block.
@@ -358,29 +358,29 @@
         merged = set(self._schema)
         for item in self._content:
             merged.update(item.schema)
         return merged
 
     def add(
         self,
-        content: Union[Mapping[str, Any], Iterable[tuple[str, Any]], Chunk, Loop],
+        content: Mapping[str, Any] | Iterable[tuple[str, Any]] | Chunk | Loop,
         /,
         comment: str = '',
     ) -> None:
         """Add a chunk or loop to the end of the block.
 
         Parameters
         ----------
         content:
             A loop, chunk, or mapping to add.
             Mappings get converted to chunks.
         comment:
             Optional comment that can be written above the chunk or loop in the file.
         """
-        if not isinstance(content, (Chunk, Loop)):
+        if not isinstance(content, Chunk | Loop):
             content = Chunk(content, comment=comment)
         self._content.append(content)
 
     def add_reduced_powder_data(self, data: sc.DataArray, *, comment: str = '') -> None:
         """Add a loop with reduced powder data.
 
         The input must be 1-dimensional with a dimension name in
@@ -477,44 +477,42 @@
         if schema_loop is not None:
             schema_loop.write(f)
             f.write('\n')
         _write_multi(f, self._content)
 
 
 def _convert_input_content(
-    content: Iterable[Union[Mapping[str, Any], Loop, Chunk]]
-) -> list[Union[Loop, Chunk]]:
-    return [
-        item if isinstance(item, (Loop, Chunk)) else Chunk(item) for item in content
-    ]
+    content: Iterable[Mapping[str, Any] | Loop | Chunk],
+) -> list[Loop | Chunk]:
+    return [item if isinstance(item, Loop | Chunk) else Chunk(item) for item in content]
 
 
 @contextmanager
-def _open(fname: Union[str, Path, io.TextIOBase]):
+def _open(fname: str | Path | io.TextIOBase):
     if isinstance(fname, io.TextIOBase):
         yield fname
     else:
         with open(fname, 'w') as f:
             yield f
 
 
 def _preprocess_schema(
-    schema: Optional[Union[CIFSchema, Iterable[CIFSchema]]]
+    schema: CIFSchema | Iterable[CIFSchema] | None,
 ) -> set[CIFSchema]:
     if schema is None:
         return set()
     if isinstance(schema, CIFSchema):
         res = {schema}
     else:
         res = set(schema)
     res.add(CORE_SCHEMA)  # needed to encode schema itself
     return res
 
 
-def _make_schema_loop(schema: set[CIFSchema]) -> Optional[Loop]:
+def _make_schema_loop(schema: set[CIFSchema]) -> Loop | None:
     if not schema:
         return None
     columns = {
         'audit_conform.dict_name': [],
         'audit_conform.dict_version': [],
         'audit_conform.dict_location': [],
     }
@@ -523,15 +521,15 @@
         columns['audit_conform.dict_version'].append(s.version)
         columns['audit_conform.dict_location'].append(s.location)
     return Loop(
         {key: sc.array(dims=['schema'], values=val) for key, val in columns.items()}
     )
 
 
-def _quotes_for_string_value(value: str) -> Optional[str]:
+def _quotes_for_string_value(value: str) -> str | None:
     if '\n' in value:
         return ';'
     if "'" in value:
         if '"' in value:
             return ';'
         return '"'
     if '"' in value:
```

### Comparing `scippneutron-24.3.0/src/scippneutron/io/nexus/_json_nexus.py` & `scippneutron-24.5.0/src/scippneutron/io/nexus/_json_nexus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Matthew Jones
 from __future__ import annotations
 
 from collections.abc import Mapping
 from dataclasses import dataclass
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any
 
 import numpy as np
 
 _nexus_class = "NX_class"
 _nexus_units = "units"
 _nexus_name = "name"
 _nexus_path = "path"
@@ -54,15 +54,15 @@
 
 
 class MissingAttribute(Exception):
     pass
 
 
 def make_json_attr(name: str, value) -> dict:
-    if isinstance(value, (str, bytes)):
+    if isinstance(value, str | bytes):
         attr_info = {"string_size": len(value), "type": "string"}
     elif isinstance(value, float):
         attr_info = {"size": 1, "type": "float64"}
     elif isinstance(value, int):
         attr_info = {"size": 1, "type": "int64"}
     elif isinstance(value, list):
         attr_info = {"size": len(value), "type": "string"}
@@ -72,15 +72,15 @@
             "type": numpy_to_filewriter_type[value.dtype.type],
         }
     name_and_value = {"name": name, "values": value}
     return {**attr_info, **name_and_value}
 
 
 def make_json_dataset(name: str, data) -> dict:
-    if isinstance(data, (str, bytes)):
+    if isinstance(data, str | bytes):
         dataset_info = {"string_size": len(data), "type": "string"}
     elif isinstance(data, float):
         dataset_info = {"size": 1, "type": "float64"}
     elif isinstance(data, int):
         dataset_info = {"size": 1, "type": "int32"}
     else:
         dataset_info = {
@@ -95,16 +95,16 @@
             _nexus_values: data,
         },
         "attributes": [],
     }
 
 
 def _get_attribute_value(
-    element: Dict, attribute_name: str
-) -> Union[str, float, int, List]:
+    element: dict, attribute_name: str
+) -> str | float | int | list:
     """
     attributes can be a dictionary of key-value pairs, or an array
     of dictionaries with key, value, type, etc
     """
     try:
         attributes = element["attributes"]
         try:
@@ -114,41 +114,41 @@
                 if attribute[_nexus_name] == attribute_name:
                     return attribute[_nexus_values]
     except KeyError:
         pass
     raise MissingAttribute
 
 
-def _visitnodes(root: Dict):
+def _visitnodes(root: dict):
     for child in root.get(_nexus_children, ()):
         yield child
         yield from _visitnodes(child)
 
 
-def _name(node: Dict):
+def _name(node: dict):
     if _nexus_name in node:
         return node[_nexus_name]
     if _nexus_config in node:
         return node[_nexus_config][_nexus_name]
     return ''
 
 
-def _is_group(node: Dict):
+def _is_group(node: dict):
     return _nexus_children in node
 
 
-def _is_dataset(node: Dict):
+def _is_dataset(node: dict):
     return node.get('module') == _nexus_dataset
 
 
-def _is_link(node: Dict):
+def _is_link(node: dict):
     return node.get('module') == _nexus_link
 
 
-def _is_stream(node: Dict):
+def _is_stream(node: dict):
     return 'module' in node and not (_is_dataset(node) or _is_link(node))
 
 
 def contains_stream(group: JSONGroup) -> bool:
     """Return True if the group contains a stream object"""
     return (
         isinstance(group, JSONGroup)
@@ -279,29 +279,29 @@
     def __contains__(self, name: str) -> bool:
         try:
             self[name]
             return True
         except KeyError:
             return False
 
-    def keys(self) -> List[str]:
+    def keys(self) -> list[str]:
         if contains_stream(self):
             return []
         children = self._node[_nexus_children]
         return [_name(child) for child in children if not contains_stream(child)]
 
-    def items(self) -> List[Tuple[str, JSONNode]]:
+    def items(self) -> list[tuple[str, JSONNode]]:
         return [(key, self[key]) for key in self.keys()]
 
     def _as_group_or_dataset(self, item, parent):
         if _is_group(item):
             return JSONGroup(item, parent=parent)
         return JSONDataset(item, parent=parent)
 
-    def __getitem__(self, name: str) -> Union[JSONDataset, JSONGroup]:
+    def __getitem__(self, name: str) -> JSONDataset | JSONGroup:
         if name.startswith('/') and name.count('/') == 1:
             parent = self.file
         elif '/' in name:
             parent = self['/'.join(name.split('/')[:-1])]
         else:
             parent = self
 
@@ -351,15 +351,15 @@
     topic: str
     flatbuffer_id: str
     source_name: str
     dtype: Any
     unit: str
 
 
-def get_streams_info(root: Dict) -> List[StreamInfo]:
+def get_streams_info(root: dict) -> list[StreamInfo]:
     found_streams = [node for node in _visitnodes(root) if _is_stream(node)]
     streams = []
     for stream in found_streams:
         try:
             dtype = _filewriter_to_supported_numpy_dtype[stream[_nexus_config]["dtype"]]
         except KeyError:
             try:
```

### Comparing `scippneutron-24.3.0/src/scippneutron/io/nexus/load_nexus.py` & `scippneutron-24.5.0/src/scippneutron/io/nexus/load_nexus.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Matthew Jones
 import json
 from contextlib import contextmanager
 from pathlib import Path
 from timeit import default_timer as timer
-from typing import Any, Dict, Optional, Set, Tuple, Union
+from typing import Any
 from warnings import warn
 
 import h5py
 import numpy as np
 import scipp as sc
 import scippnexus as snx
 from scipp.binning import make_binned
@@ -38,15 +38,15 @@
     warn the user.
     """
 
     pass
 
 
 def add_position_and_transforms_to_data(
-    data: Union[sc.DataArray, sc.Dataset],
+    data: sc.DataArray | sc.Dataset,
     transform_name: str,
     position_name: str,
     base_position_name: str,
     transforms: sc.Variable,
     positions: sc.Variable,
 ):
     if isinstance(data, sc.DataArray):
@@ -66,55 +66,56 @@
         attrs[transform_name] = sc.scalar(value=transforms)
     else:
         coords[base_position_name] = positions
         coords[transform_name] = sc.scalar(value=transforms)
 
 
 @contextmanager
-def _open_if_path(file_in: Union[str, Path, h5py.File]):
+def _open_if_path(file_in: str | Path | h5py.File):
     """
     Open if file path is provided,
     otherwise yield the existing h5py.File object
     """
-    if isinstance(file_in, (str, Path)):
+    if isinstance(file_in, str | Path):
         with h5py.File(file_in, "r", libver='latest', swmr=True) as nexus_file:
             yield nexus_file
     else:
         yield file_in
 
 
-def _load_instrument_name(instruments: Dict[str, NXobject]) -> Dict:
+def _load_instrument_name(instruments: dict[str, NXobject]) -> dict:
     instrument = next(iter(instruments.values()))
     if len(instruments) > 1:
         warn(
             f"More than one NXinstrument found in file, "
-            f"loading name from {instrument.name} only"
+            f"loading name from {instrument.name} only",
+            stacklevel=4,
         )
     if (name := instrument.get("name")) is not None:
         return {"instrument_name": sc.scalar(name[()])}
     return {}
 
 
-def _load_title(entry: NXobject) -> Dict:
+def _load_title(entry: NXobject) -> dict:
     if (title := entry.get('title')) is not None:
         return {"experiment_title": sc.scalar(title[()])}
     return {}
 
 
-def _load_start_and_end_time(entry: NXobject) -> Dict:
+def _load_start_and_end_time(entry: NXobject) -> dict:
     times = {}
     for time in ["start_time", "end_time"]:
         if (dataset := entry.get(time)) is not None:
             times[time] = sc.scalar(dataset[()])
     return times
 
 
 def load_nexus(
-    data_file: Union[str, Path, h5py.File], root: str = "/", quiet=True
-) -> Optional[ScippData]:
+    data_file: str | Path | h5py.File, root: str = "/", quiet=True
+) -> ScippData | None:
     """
     Load a NeXus file and return required information.
 
     :param data_file: path of NeXus file containing data to load
     :param root: path of group in file, only load data from the subtree of
       this group
     :param quiet: if False prints some details of what is being loaded
@@ -122,33 +123,36 @@
     Usage example:
       data = sc.neutron.load_nexus('PG3_4844_event.nxs')
     """
     warn(
         "`load_nexus` is deprecated and will be removed in version 24.03, "
         "please switch to using ScippNexus.",
         VisibleDeprecationWarning,
+        stacklevel=2,
     )
     start_time = timer()
 
     with _open_if_path(data_file) as nexus_file:
         loaded_data = _load_data(nexus_file, root, quiet)
 
     if not quiet:
-        print("Total time:", timer() - start_time)
+        from ...logging import get_logger
+
+        get_logger().info("Total time: %s", timer() - start_time)
     return loaded_data
 
 
 def _origin(unit) -> sc.Variable:
     return sc.vector(value=[0, 0, 0], unit=unit)
 
 
-def _depends_on_to_position(obj) -> Union[None, sc.Variable]:
+def _depends_on_to_position(obj) -> None | sc.Variable:
     if (transform := obj.get('depends_on')) is not None:
         if (
-            isinstance(transform, (str, sc.DataArray))
+            isinstance(transform, str | sc.DataArray)
             or transform.dtype == sc.DType.DataArray
         ):
             return None  # cannot compute position if bad transform or time-dependent
         else:
             if transform.dtype == sc.DType.rotation3:
                 return transform * _origin('m')
             else:
@@ -184,19 +188,21 @@
     x = da.coords.pop('x_pixel_offset')
     offset = sc.zeros(dims=da.dims, shape=da.shape, unit=x.unit, dtype=sc.DType.vector3)
     offset.fields.x = x.to(dtype='float64', copy=False)
     if (y := da.coords.pop('y_pixel_offset', None)) is not None:
         offset.fields.y = y.to(dtype='float64', unit=x.unit, copy=False)
     if (z := da.coords.pop('z_pixel_offset', None)) is not None:
         offset.fields.z = z.to(dtype='float64', unit=x.unit, copy=False)
-    da.coords['pixel_offset'] = offset.rename_dims(dict(zip(offset.dims, da.dims)))
+    da.coords['pixel_offset'] = offset.rename_dims(
+        dict(zip(offset.dims, da.dims, strict=True))
+    )
     return da
 
 
-def _by_nx_class(group) -> Dict[str, Dict[str, 'NXobject']]:
+def _by_nx_class(group) -> dict[str, dict[str, 'NXobject']]:
     from scippnexus.v1.nxobject import _nx_class_registry
 
     classes = {name: [] for name in _nx_class_registry()}
 
     def _match_nx_class(_, node):
         if not hasattr(node, 'shape'):
             if (nx_class := node.attrs.get('NX_class')) is not None:
@@ -208,21 +214,21 @@
     group._group.visititems(_match_nx_class)
 
     out = {}
     for nx_class, groups in classes.items():
         names = [group.name.split('/')[-1] for group in groups]
         if len(names) != len(set(names)):  # fall back to full path if duplicate
             names = [group.name for group in groups]
-        out[nx_class] = {n: group._make(g) for n, g in zip(names, groups)}
+        out[nx_class] = {n: group._make(g) for n, g in zip(names, groups, strict=True)}
     return out
 
 
 def _load_data(
-    nexus_file: Union[h5py.File, Dict], root: Optional[str], quiet: bool
-) -> Optional[ScippData]:
+    nexus_file: h5py.File | dict, root: str | None, quiet: bool
+) -> ScippData | None:
     """
     Main implementation for loading data is extracted to this function so that
     in-memory data can be used for unit tests.
     """
     root = NXroot(nexus_file if root is None else nexus_file[root])
     classes = _by_nx_class(root)
 
@@ -267,25 +273,25 @@
                     transform_name="position_transformations",
                     position_name="position",
                     base_position_name="base_position",
                     positions=det.coords.pop('pixel_offset'),
                     transforms=det.coords.pop('depends_on', None),
                 )
             loaded_detectors.append(det)
-        except (
+        except (  # noqa: PERF203
             BadSource,
             SkipSource,
             NexusStructureError,
             KeyError,
             sc.DTypeError,
             ValueError,
             IndexError,
         ) as e:
             if not contains_stream(group._group):
-                warn(f"Skipped loading {group.name} due to:\n{e}")
+                warn(f"Skipped loading {group.name} due to:\n{e}", stacklevel=3)
 
     no_event_data = True
     loaded_data = {}
 
     # If no event data are found, make a Dataset and add the metadata as
     # Dataset entries. Otherwise, make a DataArray.
     if len(loaded_detectors):
@@ -307,17 +313,17 @@
                 if len(events.bins.constituents['data']) != 0:
                     # See scipp/scipp#2490
                     det_id = sc.arange('detector_id', det_min, det_max + 1, unit=None)
                     events = make_binned(
                         events, groups=[det_id], erase=['pulse', 'bank']
                     )
                 loaded_events.append(events)
-            except (BadSource, SkipSource, NexusStructureError, IndexError) as e:
+            except (BadSource, SkipSource, NexusStructureError, IndexError) as e:  # noqa:PERF203
                 if not contains_stream(group._group):
-                    warn(f"Skipped loading {group.name} due to:\n{e}")
+                    warn(f"Skipped loading {group.name} due to:\n{e}", stacklevel=3)
         if len(loaded_events):
             no_event_data = False
             loaded_data = sc.concat(loaded_events, 'detector_id')
 
     if not no_event_data:
         # Add single tof bin
         loaded_data = sc.DataArray(
@@ -328,15 +334,15 @@
             attrs=dict(get_attrs(loaded_data).items()),
         )
         tof_min = loaded_data.bins.coords['tof'].min().to(dtype='float64')
         tof_max = loaded_data.bins.coords['tof'].max().to(dtype='float64')
         tof_max.value = np.nextafter(tof_max.value, float("inf"))
         loaded_data.coords['tof'] = sc.concat([tof_min, tof_max], 'tof')
 
-    def add_metadata(metadata: Dict[str, sc.Variable]):
+    def add_metadata(metadata: dict[str, sc.Variable]):
         for key, value in metadata.items():
             if isinstance(loaded_data, sc.DataArray):
                 get_attrs(loaded_data)[key] = value
             else:
                 loaded_data[key] = value
 
     if entries := classes['NXentry']:
@@ -349,26 +355,26 @@
     def load_and_add_metadata(groups, process=lambda x: x):
         items = {}
         loaded_groups = []
         for name, group in groups.items():
             try:
                 items[name] = sc.scalar(process(group[()]))
                 loaded_groups.append(name)
-            except (
+            except (  # noqa: PERF203
                 BadSource,
                 SkipSource,
                 TransformationError,
                 sc.DimensionError,
                 sc.UnitError,
                 NexusStructureError,
                 KeyError,
                 ValueError,
             ) as e:
                 if not contains_stream(group._group):
-                    warn(f"Skipped loading {group.name} due to:\n{e}")
+                    warn(f"Skipped loading {group.name} due to:\n{e}", stacklevel=4)
         add_metadata(items)
         return loaded_groups
 
     load_and_add_metadata(classes.get('NXdisk_chopper', {}))
     load_and_add_metadata(classes.get('NXlog', {}))
     load_and_add_metadata(classes.get('NXmonitor', {}), _monitor_to_canonical)
     for name, tag in {'sample': 'NXsample', 'source': 'NXsource'}.items():
@@ -396,37 +402,37 @@
         return loaded_data
     return sc.Dataset(loaded_data)
 
 
 def load_nexus_json_str(
     json_template: str,
     get_start_info: bool = False,
-) -> Tuple[Optional[ScippData], Optional[sc.Variable], Optional[Set[StreamInfo]]]:
+) -> tuple[ScippData | None, sc.Variable | None, set[StreamInfo] | None]:
     """
     Use this function for testing so that file io is not required
     """
     # We do not use cls to convert value lists to sc.Variable at this
     # point because we do not know what dimension names to use here
     loaded_json = json.loads(json_template)
     streams = None
     if get_start_info:
         streams = get_streams_info(loaded_json)
     group = JSONGroup(loaded_json)
     return _load_data(group, None, True), streams
 
 
-def load_nexus_json(json_filename: str) -> Optional[ScippData]:
-    with open(json_filename, 'r') as json_file:
+def load_nexus_json(json_filename: str) -> ScippData | None:
+    with open(json_filename) as json_file:
         json_string = json_file.read()
     loaded_data, _ = load_nexus_json_str(json_string)
     return loaded_data
 
 
 def json_nexus_group(
-    json_dict: dict[str, Any], *, definitions: Optional[Dict[str, type]] = None
+    json_dict: dict[str, Any], *, definitions: dict[str, type] | None = None
 ) -> snx.Group:
     """Parse a JSON dictionary into a NeXus group.
 
     Parameters
     ----------
     json_dict:
         ``dict`` containing a NeXus structure as JSON.
```

### Comparing `scippneutron-24.3.0/src/scippneutron/io/xye.py` & `scippneutron-24.5.0/src/scippneutron/io/xye.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 """File writer and reader for XYE files."""
 
 import io
 from pathlib import Path
-from typing import Optional, Union
 
 import numpy as np
 import scipp as sc
 
 from ..logging import get_logger
 
 
@@ -17,19 +16,19 @@
         return 'GenerateHeader'
 
 
 GenerateHeader = GenerateHeaderType()
 
 
 def save_xye(
-    fname: Union[str, Path, io.TextIOBase],
+    fname: str | Path | io.TextIOBase,
     da: sc.DataArray,
     *,
-    coord: Optional[str] = None,
-    header: Union[str, GenerateHeaderType] = GenerateHeader,
+    coord: str | None = None,
+    header: str | GenerateHeaderType = GenerateHeader,
 ) -> None:
     """Write a data array to an XYE file.
 
     The input must be 1-dimensional, have variances, and at least one coordinate.
     It is possible to select which coordinate gets written with the ``coord`` argument.
 
     The data are written as an ASCII table with columns X, Y, E, where
@@ -99,20 +98,20 @@
         coord,
         fname,
     )
     np.savetxt(fname, to_save, delimiter=' ', header=header)
 
 
 def load_xye(
-    fname: Union[str, Path, io.TextIOBase],
+    fname: str | Path | io.TextIOBase,
     *,
     dim: str,
-    unit: Optional[Union[sc.Unit, str]],
-    coord_unit: Optional[Union[sc.Unit, str]],
-    coord: Optional[str] = None,
+    unit: sc.Unit | str | None,
+    coord_unit: sc.Unit | str | None,
+    coord: str | None = None,
 ) -> sc.DataArray:
     """Read a data array from an XYE file.
 
     See :func:`scippneutron.io.xye.save_xye` for a description of the file format.
 
     Since XYE files are lossy, some metadata must be provided manually when calling
     this function.
```

### Comparing `scippneutron-24.3.0/src/scippneutron/logging.py` & `scippneutron-24.5.0/src/scippneutron/logging.py`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/src/scippneutron/mantid.py` & `scippneutron-24.5.0/src/scippneutron/mantid.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import re
 import uuid
 import warnings
 from contextlib import contextmanager
 from copy import deepcopy
 from pathlib import Path
-from typing import Any, Dict, Union
+from typing import Any
 
 import numpy as np
 import scipp as sc
 from scipp.core.util import VisibleDeprecationWarning
 
 from ._utils import get_attrs
 
@@ -25,15 +25,15 @@
         from mantid.api import AnalysisDataService
     except ImportError:
         raise ImportError(
             "Mantid Python API was not found, please install Mantid framework "
             "as detailed in the installation instructions ("
             "https://scipp.github.io/scippneutron/getting-started/"
             "installation.html)"
-        )
+        ) from None
     # Deal with multiple calls to this function, which may have conflicting
     # names in the global AnalysisDataService by using uuid.
     ws_name = f'scipp.run_mantid_alg.{uuid.uuid4()}'
     # Deal with non-standard ways to define the prefix of output workspaces
     if alg == 'Fit':
         kwargs['Output'] = ws_name
     elif alg == 'LoadDiffCal':
@@ -179,42 +179,40 @@
     # but for now this is not necessary.
 
     return sc.Dataset(coords={'detector': detector, spectrum_dim: spectrum})
 
 
 def md_dimension(mantid_dim, index):
     # Look for q dimensions
-    patterns = ["^q.*{0}$".format(coord) for coord in ['x', 'y', 'z']]
+    patterns = [f"^q.*{coord}$" for coord in ['x', 'y', 'z']]
     q_dims = ['Q_x', 'Q_y', 'Q_z']
-    pattern_result = zip(patterns, q_dims)
+    pattern_result = zip(patterns, q_dims, strict=True)
     if mantid_dim.getMDFrame().isQ():
         for pattern, result in pattern_result:
             if re.search(pattern, mantid_dim.name, re.IGNORECASE):
                 return result
 
     # Look for common/known mantid dimensions
     patterns = ["DeltaE", "T"]
     dims = ['energy_transfer', 'temperature']
-    pattern_result = zip(patterns, dims)
+    pattern_result = zip(patterns, dims, strict=True)
     for pattern, result in pattern_result:
         if re.search(pattern, mantid_dim.name, re.IGNORECASE):
             return result
 
     # Look for common spatial dimensions
-    patterns = ["^{0}$".format(coord) for coord in ['x', 'y', 'z']]
+    patterns = [f"^{coord}$" for coord in ['x', 'y', 'z']]
     dims = ['x', 'y', 'z']
-    pattern_result = zip(patterns, dims)
+    pattern_result = zip(patterns, dims, strict=True)
     for pattern, result in pattern_result:
         if re.search(pattern, mantid_dim.name, re.IGNORECASE):
             return result
 
     raise ValueError(
-        "Cannot infer scipp dimension from input mantid dimension {}".format(
-            mantid_dim.name()
-        )
+        f"Cannot infer scipp dimension from input mantid dimension {mantid_dim.name()}"
     )
 
 
 def md_unit(frame):
     known_md_units = {
         "Angstrom^-1": sc.units.dimensionless / sc.units.angstrom,
         "r.l.u": sc.units.dimensionless,
@@ -269,15 +267,15 @@
 
 def _rot_from_vectors(vec1, vec2):
     a = sc.vector(value=vec1.value / np.linalg.norm(vec1.value))
     b = sc.vector(value=vec2.value / np.linalg.norm(vec2.value))
     c = sc.vector(value=np.cross(a.value, b.value))
     angle = sc.acos(sc.dot(a, b)).value
     return sc.spatial.rotation(
-        value=list(c.value * np.sin(angle / 2)) + [np.cos(angle / 2)]
+        value=[*(c.value * np.sin(angle / 2)), np.cos(angle / 2)]
     )
 
 
 def get_detector_pos(ws, spectrum_dim):
     nHist = ws.getNumberHistograms()
     pos = np.zeros([nHist, 3])
 
@@ -454,15 +452,15 @@
 
 
 def set_bin_masks(bin_masks, dim, index, masked_bins):
     for masked_bin in masked_bins:
         bin_masks['spectrum', index][dim, masked_bin].value = True
 
 
-def _as_dict_of_variables(d: Dict[str, Any]) -> Dict[str, sc.Variable]:
+def _as_dict_of_variables(d: dict[str, Any]) -> dict[str, sc.Variable]:
     return {
         key: val if isinstance(val, sc.Variable) else sc.scalar(val)
         for key, val in d.items()
     }
 
 
 def _convert_MatrixWorkspace_info(ws, advanced_geometry=False, load_run_logs=True):
@@ -892,15 +890,15 @@
             **coords_labs_data["attrs"],
         }
     )
 
 
 def convert_MDHistoWorkspace_to_data_group(md_histo, **ignored) -> sc.DataGroup:
     ndims = md_histo.getNumDims()
-    coords = dict()
+    coords = {}
     dims_used = []
     for i in range(ndims):
         dim = md_histo.getDimension(i)
         frame = dim.getMDFrame()
         sc_dim = md_dimension(dim, i)
         coords[sc_dim] = sc.array(
             dims=[sc_dim],
@@ -925,15 +923,15 @@
         'convert_MDHistoWorkspace_to_data_array is deprecated in favor of '
         'convert_MDHistoWorkspace_to_data_group.',
         VisibleDeprecationWarning,
         stacklevel=4,
     )
 
     ndims = md_histo.getNumDims()
-    coords = dict()
+    coords = {}
     dims_used = []
     for i in range(ndims):
         dim = md_histo.getDimension(i)
         frame = dim.getMDFrame()
         sc_dim = md_dimension(dim, i)
         coords[sc_dim] = sc.Variable(
             dims=[sc_dim],
@@ -1081,15 +1079,15 @@
     elif w_id == 'TableWorkspace':
         scipp_obj = convert_TableWorkspace_to_dataset(workspace, **kwargs)
     elif w_id == 'MDHistoWorkspace':
         scipp_obj = convert_MDHistoWorkspace_to_data_group(workspace, **kwargs)
     elif w_id == 'WorkspaceGroup':
         scipp_obj = convert_WorkspaceGroup_to_data_group(workspace, **kwargs)
     else:
-        raise RuntimeError('Unsupported workspace type {}'.format(w_id))
+        raise RuntimeError(f'Unsupported workspace type {w_id}')
 
     # TODO Is there ever a case where a Workspace2D has a separate monitor
     # workspace? This is not handled by ExtractMonitors above, I think.
     if monitor_ws is None:
         if hasattr(workspace, 'getMonitorWorkspace'):
             try:
                 monitor_ws = workspace.getMonitorWorkspace()
@@ -1107,15 +1105,15 @@
         )
     for ws in workspaces_to_delete:
         mantid.DeleteWorkspace(ws)
 
     return scipp_obj
 
 
-def array_from_mantid(workspace, **kwargs) -> Union[sc.DataArray, sc.Dataset]:
+def array_from_mantid(workspace, **kwargs) -> sc.DataArray | sc.Dataset:
     """Convert Mantid workspace to a scipp data array or dataset.
     :param workspace: Mantid workspace to convert.
 
     .. deprecated:: 23.07.0
        The old ``from_mantid`` was renamed to ``array_from_mantid`` and is deprecated
        in favor of the new ``from_mantid`` which return a data group.
     """
@@ -1151,15 +1149,15 @@
         scipp_obj = convert_TableWorkspace_to_dataset(workspace, **kwargs)
     elif w_id == 'MDHistoWorkspace':
         scipp_obj = convert_MDHistoWorkspace_to_data_array(workspace, **kwargs)
     elif w_id == 'WorkspaceGroup':
         scipp_obj = convert_WorkspaceGroup_to_dataarray_dict(workspace, **kwargs)
 
     if scipp_obj is None:
-        raise RuntimeError('Unsupported workspace type {}'.format(w_id))
+        raise RuntimeError(f'Unsupported workspace type {w_id}')
 
     # TODO Is there ever a case where a Workspace2D has a separate monitor
     # workspace? This is not handled by ExtractMonitors above, I think.
     if monitor_ws is None:
         if hasattr(workspace, 'getMonitorWorkspace'):
             try:
                 monitor_ws = workspace.getMonitorWorkspace()
@@ -1179,15 +1177,15 @@
     for ws in workspaces_to_delete:
         mantid.DeleteWorkspace(ws)
 
     return scipp_obj
 
 
 def load_with_mantid(
-    filename: Union[str, Path] = "",
+    filename: str | Path = "",
     load_pulse_times=True,
     instrument_filename=None,
     error_connection=None,
     mantid_alg='Load',
     mantid_args=None,
     advanced_geometry=False,
 ) -> sc.DataGroup:
@@ -1272,15 +1270,15 @@
             load_pulse_times=load_pulse_times,
             error_connection=error_connection,
             advanced_geometry=advanced_geometry,
         )
 
 
 def load(
-    filename: Union[str, Path] = "",
+    filename: str | Path = "",
     load_pulse_times=True,
     instrument_filename=None,
     error_connection=None,
     mantid_alg='Load',
     mantid_args=None,
     advanced_geometry=False,
 ) -> sc.Dataset:
@@ -1429,16 +1427,16 @@
 
     user_k = str(unit_dim).casefold()
     known_units = {k.casefold(): v for k, v in known_units.items()}
 
     if user_k not in known_units:
         raise RuntimeError(
             "Axis unit not currently supported."
-            "Possible values are: {}, "
-            "got '{}'. ".format([k for k in known_units.keys()], unit_dim)
+            f"Possible values are: {list(known_units.keys())}, "
+            f"got '{unit_dim}'. "
         )
     else:
         return known_units[user_k]
 
 
 def to_mantid(data, dim, instrument_file=None):
     """
@@ -1463,15 +1461,15 @@
     try:
         import mantid.simpleapi as mantid
     except ImportError:
         raise ImportError(
             "Mantid Python API was not found, please install Mantid framework "
             "as detailed in the installation instructions (https://scipp."
             "github.io/getting-started/installation.html)"
-        )
+        ) from None
     x = data.coords[dim].values
     y = data.values
     e = data.variances
 
     if len(y.shape) not in (1, 2):
         raise ValueError("Currently can only handle 2D data.")
```

### Comparing `scippneutron-24.3.0/src/scippneutron/tof/chopper_cascade.py` & `scippneutron-24.5.0/src/scippneutron/tof/chopper_cascade.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 # @author Simon Heybrock
 """
 Compute result of applying a chopper cascade to a neutron pulse at a time-of-flight
 neutron source.
 
 See :py:class:`FrameSequence` for the main entry point.
 """
+
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Any, List, Optional, Union
+from typing import Any
 
 import numpy as np
 import scipp as sc
 
 
 def wavelength_to_inverse_velocity(wavelength):
     h = sc.constants.h
@@ -56,15 +57,15 @@
         if time.sizes != wavelength.sizes:
             raise sc.DimensionError(
                 f'Inconsistent dims or shape: {time.sizes} vs {wavelength.sizes}'
             )
         self.time = time.to(unit='s', copy=False)
         self.wavelength = wavelength.to(unit='angstrom', copy=False)
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, Subframe):
             return NotImplemented
         return sc.identical(self.time, other.time) and sc.identical(
             self.wavelength, other.wavelength
         )
 
     def is_regular(self) -> bool:
@@ -126,15 +127,15 @@
 class Frame:
     """
     A frame of neutrons, created from a single neutron pulse, potentially chopped into
     subframes by choppers.
     """
 
     distance: sc.Variable
-    subframes: List[Subframe]
+    subframes: list[Subframe]
 
     def propagate_to(self, distance: sc.Variable) -> Frame:
         """
         Compute new frame by propagating to a distance.
 
         Parameters
         ----------
@@ -180,15 +181,15 @@
             )
         frame = self.propagate_to(chopper.distance)
 
         # A chopper can have multiple openings, call _chop for each of them. The result
         # is the union of the resulting subframes.
         chopped = Frame(distance=frame.distance, subframes=[])
         for subframe in frame.subframes:
-            for open, close in zip(chopper.time_open, chopper.time_close):
+            for open, close in zip(chopper.time_open, chopper.time_close, strict=True):
                 if (tmp := _chop(subframe, open, close_to_open=True)) is not None:
                     if (tmp := _chop(tmp, close, close_to_open=False)) is not None:
                         chopped.subframes.append(tmp)
         return chopped
 
     def bounds(self) -> sc.DataGroup:
         """The bounds of the frame, i.e., the global min and max time and wavelength."""
@@ -234,15 +235,15 @@
             end: sc.Variable
             wav_start: sc.Variable
             wav_end: sc.Variable
 
         bounds = [
             Bound(start, end, wav_start, wav_end)
             for start, end, wav_start, wav_end in zip(
-                starts, ends, wav_starts, wav_ends
+                starts, ends, wav_starts, wav_ends, strict=True
             )
         ]
         bounds = sorted(bounds, key=lambda x: x.start)
         current = bounds[0]
         merged_bounds = []
         for bound in bounds[1:]:
             # If start is before current end, merge
@@ -277,15 +278,15 @@
     subframes by choppers.
 
     It is recommended to use the :py:meth:`from_source_pulse` constructor to create a
     frame sequence from a source pulse. Then, a chopper cascade can be applied using
     :py:meth:`chop`.
     """
 
-    frames: List[Frame]
+    frames: list[Frame]
 
     @staticmethod
     def from_source_pulse(
         time_min: sc.Variable,
         time_max: sc.Variable,
         wavelength_min: sc.Variable,
         wavelength_max: sc.Variable,
@@ -310,15 +311,15 @@
         ]
         return FrameSequence(frames)
 
     def __len__(self) -> int:
         """Number of frames."""
         return len(self.frames)
 
-    def __getitem__(self, item: Union[int, sc.Variable]) -> Frame:
+    def __getitem__(self, item: int | sc.Variable) -> Frame:
         """Get a frame by index or distance."""
         if isinstance(item, int):
             return self.frames[item]
         distance = item.to(unit='m')
         frame_before_detector = None
         for frame in self:
             if frame.distance > distance:
@@ -339,17 +340,17 @@
             Distance to propagate.
 
         Returns
         -------
         :
             New frame sequence.
         """
-        return FrameSequence(self.frames + [self.frames[-1].propagate_to(distance)])
+        return FrameSequence([*self.frames, self.frames[-1].propagate_to(distance)])
 
-    def chop(self, choppers: List[Chopper]) -> FrameSequence:
+    def chop(self, choppers: list[Chopper]) -> FrameSequence:
         """
         Chop the frame sequence by a list of choppers.
 
         The choppers will be sorted by their distance, and applied in order.
 
         Parameters
         ----------
@@ -365,19 +366,19 @@
         frames = list(self.frames)
         for chopper in choppers:
             frames.append(frames[-1].chop(chopper))
         return FrameSequence(frames)
 
     def draw(
         self,
-        linewidth: Union[int, float] = 0,
+        linewidth: float = 0,
         fill: bool = True,
-        alpha: Optional[float] = None,
+        alpha: float | None = None,
         transpose: bool = False,
-        colors: Optional[List[str]] = None,
+        colors: list[str] | None = None,
         grid: bool = True,
         title: str = 'Frame propagation through chopper cascade',
         time_unit: str = 'ms',
         wavelength_unit: str = 'angstrom',
     ) -> Any:
         """
         Draw frames using matplotlib.
@@ -501,17 +502,15 @@
         return Chopper(
             distance=self.distance,
             time_open=self.time_open[key],
             time_close=self.time_close[key],
         )
 
 
-def _chop(
-    frame: Subframe, time: sc.Variable, close_to_open: bool
-) -> Optional[Subframe]:
+def _chop(frame: Subframe, time: sc.Variable, close_to_open: bool) -> Subframe | None:
     inside = frame.time >= time if close_to_open else frame.time <= time
     output = []
     for i in range(len(frame.time)):
         # Note how j wraps around to 0
         j = (i + 1) % len(frame.time)
         inside_i = inside[i]
         inside_j = inside[j]
```

### Comparing `scippneutron-24.3.0/src/scippneutron/tof/diagram.py` & `scippneutron-24.5.0/src/scippneutron/tof/diagram.py`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/src/scippneutron/tof/fakes.py` & `scippneutron-24.5.0/src/scippneutron/tof/fakes.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 
 This provides data in a structure as typically provided in a NeXus file, including:
 
 - Detector event data including event_time_offset and event_time_zero
 - Monitor event data including event_time_offset and event_time_zero
 - Chopper timestamps
 """
-from __future__ import annotations
 
-from typing import Optional
+from __future__ import annotations
 
 import scipp as sc
 from numpy import random
 
 from . import chopper_cascade
 
 
@@ -100,15 +99,15 @@
     def __init__(
         self,
         source: FakeSource,
         pulse: FakePulse,
         choppers: dict[str, chopper_cascade.Chopper],
         monitors: dict[str, sc.Variable],
         detectors: dict[str, sc.Variable],
-        time_of_flight_origin: Optional[str] = None,
+        time_of_flight_origin: str | None = None,
     ):
         """
         Return a fake beamline.
 
         Parameters
         ----------
         source:
@@ -160,27 +159,26 @@
                 0, self._source.events_per_pulse, size=self._source.number_of_pulses
             ),
             unit=None,
         )
         event_index = sc.cumsum(sizes, dim='pulse', mode='exclusive')
         size = sizes.sum().value
         subsizes = self._split_size(size, subframes)
-        subframe_times = []
-        for i in range(subframes):
-            subframe_times.append(
-                sc.array(
-                    dims=['event'],
-                    values=self._source.rng.uniform(
-                        subbounds['subframe', i][0].value,
-                        subbounds['subframe', i][-1].value,
-                        size=subsizes[i],
-                    ),
-                    unit=bounds.unit,
-                )
+        subframe_times = [
+            sc.array(
+                dims=['event'],
+                values=self._source.rng.uniform(
+                    subbounds['subframe', i][0].value,
+                    subbounds['subframe', i][-1].value,
+                    size=subsizes[i],
+                ),
+                unit=bounds.unit,
             )
+            for i in range(subframes)
+        ]
 
         # Offset from pulse that created the monitor event
         time_offset = sc.concat(subframe_times, 'event')
         # Ensure all pulses have events from all subframes
         self._source.rng.shuffle(time_offset.values)
         event_time_offset = time_offset % self._source.pulse_period
         time_zero_offset = time_offset - event_time_offset
```

### Comparing `scippneutron-24.3.0/src/scippneutron/tof/unwrap.py` & `scippneutron-24.5.0/src/scippneutron/tof/unwrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 data.
 
 The module handles standard unwrapping, unwrapping in pulse-skipping mode, and
 unwrapping for WFM instruments, as well as combinations of the latter two. The
 functions defined here are meant to be used as providers for a Sciline pipeline. See
 https://scipp.github.io/sciline/ on how to use Sciline.
 """
+
 import math
+from collections.abc import Callable, Mapping
 from dataclasses import dataclass
-from typing import Callable, Mapping, NewType, Optional, Tuple, Union
+from typing import NewType
 
 import scipp as sc
 
 from .._utils import elem_unit
 from . import chopper_cascade
 
 Choppers = NewType('Choppers', Mapping[str, chopper_cascade.Chopper])
@@ -109,21 +111,21 @@
 
 SampleDistance = NewType('SampleDistance', sc.Variable)
 """
 Location of the sample along the incident beam. Origin must be consistent with chopper
 distance origin.
 """
 
-SourceTimeRange = NewType('SourceTimeRange', Tuple[sc.Variable, sc.Variable])
+SourceTimeRange = NewType('SourceTimeRange', tuple[sc.Variable, sc.Variable])
 """
 Time range of the source pulse, used for computing frame bounds.
 """
 
 SourceWavelengthRange = NewType(
-    'SourceWavelengthRange', Tuple[sc.Variable, sc.Variable]
+    'SourceWavelengthRange', tuple[sc.Variable, sc.Variable]
 )
 """
 Wavelength range of the source pulse, used for computing frame bounds.
 """
 
 SubframeBounds = NewType('SubframeBounds', sc.Variable)
 """
@@ -155,20 +157,20 @@
 
 @dataclass
 class TimeOfFlightOrigin:
     """
     The origin of the time-of-flight, time since pulse time and distance from source.
     """
 
-    time: Union[sc.Variable, sc.DataArray]
+    time: sc.Variable | sc.DataArray
     distance: sc.Variable
 
 
 def frame_period(
-    pulse_period: PulsePeriod, pulse_stride: Optional[PulseStride]
+    pulse_period: PulsePeriod, pulse_stride: PulseStride | None
 ) -> FramePeriod:
     if pulse_stride is None:
         return pulse_period
     return FramePeriod(pulse_period * pulse_stride)
 
 
 def frame_at_detector(
@@ -331,15 +333,15 @@
     )
     return DeltaFromWrapped(sc.lookup(offset, dim=dim)[wrapped_time_offset])
 
 
 def source_chopper(
     choppers: Choppers,
     source_time_range: SourceTimeRange,
-    source_chopper_name: Optional[SourceChopperName],
+    source_chopper_name: SourceChopperName | None,
 ) -> SourceChopper:
     """
     Return the chopper defining the source location and time-of-flight time origin.
 
     If there is no pulse-shaping chopper, then the source-pulse begin and end time
     are used to define a fake chopper.
     """
```

### Comparing `scippneutron-24.3.0/src/scippneutron.egg-info/PKG-INFO` & `scippneutron-24.5.0/src/scippneutron.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: scippneutron
-Version: 24.3.0
+Version: 24.5.0
 Summary: Neutron scattering tools for Data Reduction
 Author: Scipp contributors
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
+        Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -38,30 +38,29 @@
 Project-URL: Source, https://github.com/scipp/scippneutron
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5py
 Requires-Dist: numpy>=1.20
 Requires-Dist: pooch
+Requires-Dist: plopp>=24.04.0
 Requires-Dist: scipp>=23.07.0
 Requires-Dist: scippnexus>=23.8.0
 Requires-Dist: scipy>=1.7.0
-Provides-Extra: interactive
-Requires-Dist: scipp[interactive]; extra == "interactive"
 Provides-Extra: all
 Requires-Dist: scipp[all]; extra == "all"
 
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 [![PyPI badge](http://img.shields.io/pypi/v/scippneutron.svg)](https://pypi.python.org/pypi/scippneutron)
 [![Anaconda-Server Badge](https://anaconda.org/scipp/scippneutron/badges/version.svg)](https://anaconda.org/scipp/scippneutron)
 [![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](LICENSE)
```

### Comparing `scippneutron-24.3.0/src/scippneutron.egg-info/SOURCES.txt` & `scippneutron-24.5.0/src/scippneutron.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,34 +4,29 @@
 .pre-commit-config.yaml
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 tox.ini
 .buildconfig/ci-linux.yml
-.buildconfig/ci-macos.yml
-.buildconfig/ci-windows.yml
 .github/dependabot.yml
 .github/workflows/ci.yml
 .github/workflows/docs.yml
 .github/workflows/nightly_at_main.yml
 .github/workflows/nightly_at_release.yml
-.github/workflows/pr_and_main.yml
 .github/workflows/python-version-ci
 .github/workflows/release.yml
 .github/workflows/test.yml
 .github/workflows/unpinned.yml
 benchmarks/__init__.py
 benchmarks/load_nexus.py
 benchmarks/transform_coords.py
 conda/meta.yaml
-docs/_typehints.py
 docs/bibliography.bib
 docs/conf.py
 docs/index.md
 docs/_static/anaconda-icon.js
 docs/_static/favicon.ico
 docs/_static/logo-dark.svg
 docs/_static/logo.svg
@@ -127,14 +122,19 @@
 src/scippneutron/io/__init__.py
 src/scippneutron/io/cif.py
 src/scippneutron/io/xye.py
 src/scippneutron/io/nexus/__init__.py
 src/scippneutron/io/nexus/_json_nexus.py
 src/scippneutron/io/nexus/_nexus.py
 src/scippneutron/io/nexus/load_nexus.py
+src/scippneutron/peaks/__init__.py
+src/scippneutron/peaks/_common.py
+src/scippneutron/peaks/_fit_peaks.py
+src/scippneutron/peaks/_remove_peaks.py
+src/scippneutron/peaks/model.py
 src/scippneutron/tof/__init__.py
 src/scippneutron/tof/chopper_cascade.py
 src/scippneutron/tof/diagram.py
 src/scippneutron/tof/fakes.py
 src/scippneutron/tof/unwrap.py
 tests/HYS_mask.xml
 tests/beamline_components_test.py
@@ -160,12 +160,15 @@
 tests/io/json_nexus_examples/entry.json
 tests/io/json_nexus_examples/event_data.json
 tests/io/json_nexus_examples/instrument.json
 tests/io/json_nexus_examples/log.json
 tests/mantid_scipp_comparison/beamline_calculations_test.py
 tests/mantid_scipp_comparison/histogram_events_test.py
 tests/mantid_scipp_comparison/neutron_convert_units_test.py
+tests/peaks/fit_peaks_test.py
+tests/peaks/model_test.py
+tests/peaks/remove_peaks_test.py
 tests/tof/chopper_cascade_test.py
 tests/tof/fakes_test.py
 tests/tof/to_time_of_flight_test.py
 tests/tof/unwrap_test.py
 tools/make_tutorial_data.ipynb
```

### Comparing `scippneutron-24.3.0/tests/atoms/test_atoms.py` & `scippneutron-24.5.0/tests/atoms/test_atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,16 @@
         incoherent_scattering_length_im=sc.scalar(-55.8, unit='fm'),
         coherent_scattering_cross_section=sc.scalar(
             650.0, variance=4.0**2, unit='barn'
         ),
         incoherent_scattering_cross_section=sc.scalar(
             394.0, variance=7.0**2, unit='barn'
         ),
-        total_scattering_cross_section=sc.scalar(
-            1044.0, variance=8.0**2, unit='barn'
-        ),
+        total_scattering_cross_section=sc.scalar(1044.0, variance=8.0**2, unit='barn'),
         absorption_cross_section=sc.scalar(259000.0, variance=700.0**2, unit='barn'),
     )
     assert params == expected
 
 
 def test_scattering_params_unknown():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="No entry for element / isotope 'scippium'"):
         scn.atoms.ScatteringParams.for_isotope('scippium')
```

### Comparing `scippneutron-24.3.0/tests/beamline_components_test.py` & `scippneutron-24.5.0/tests/beamline_components_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import pytest
 import scipp as sc
 
 import scippneutron as scn
 
 
-@pytest.fixture
+@pytest.fixture()
 def data_array():
     positions = [[-1, 0, 0], [0, 1, 0], [0, 0, 1]]
     return sc.DataArray(
         sc.Variable(dims=['position', 'tof'], values=np.random.rand(3, 9)),
         coords={
             'position': sc.vectors(dims=['position'], values=positions, unit='m'),
             'source_position': sc.vector(value=np.array([0, 0, -10]), unit='m'),
```

### Comparing `scippneutron-24.3.0/tests/conftest.py` & `scippneutron-24.5.0/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
-from typing import Any, List
+from typing import Any
 
 import pytest
 import scipp as sc
 
 pytest.register_assert_rewrite('scipp.testing.assertions')
 
 
-def pytest_assertrepr_compare(op: str, left: Any, right: Any) -> List[str]:
+def pytest_assertrepr_compare(op: str, left: Any, right: Any) -> list[str]:
     if isinstance(left, sc.Unit) and isinstance(right, sc.Unit):
         return [f'Unit({left}) {op} Unit({right})']
     if isinstance(left, sc.DType) or isinstance(right, sc.DType):
         return [f'{left!r} {op} {right!r}']
```

### Comparing `scippneutron-24.3.0/tests/conversion/beamline_conversions_test.py` & `scippneutron-24.5.0/tests/conversion/beamline_conversions_test.py`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/tests/conversion/graph/beamline_graph_test.py` & `scippneutron-24.5.0/tests/conversion/graph/beamline_graph_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,27 +52,27 @@
         'Ltotal',
         'two_theta',
     }
 
 
 @pytest.mark.parametrize(
     'fn',
-    (
+    [
         beamline.incident_beam,
         beamline.scattered_beam,
         beamline.L1,
         beamline.L2,
         beamline.two_theta,
-    ),
+    ],
 )
 def test_beamline_returns_new_graph_without_scatter_arg(fn):
     g = fn()
     g['a_new_node'] = lambda position: 2 * position
     assert 'a_new_node' not in fn()
 
 
-@pytest.mark.parametrize('fn', (beamline.beamline, beamline.Ltotal))
-@pytest.mark.parametrize('scatter', (True, False))
+@pytest.mark.parametrize('fn', [beamline.beamline, beamline.Ltotal])
+@pytest.mark.parametrize('scatter', [True, False])
 def test_beamline_returns_new_graph_with_scatter_arg(fn, scatter):
     g = fn(scatter=scatter)
     g['a_new_node'] = lambda position: 2 * position
     assert 'a_new_node' not in fn(scatter=scatter)
```

### Comparing `scippneutron-24.3.0/tests/conversion/graph/tof_graph_test.py` & `scippneutron-24.5.0/tests/conversion/graph/tof_graph_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,110 +30,110 @@
         'Q_vec',
         'hkl_vec',
         ('h', 'k', 'l'),
         'ub_matrix',
     }
 
 
-@pytest.mark.parametrize('start', ('dspacing',))
+@pytest.mark.parametrize('start', ['dspacing'])
 def test_elastic_unsupported_starts(start):
     with pytest.raises(KeyError):
         tof.elastic(start)
 
 
 def test_kinematic():
     assert set(tof.kinematic('tof').keys()) == {'energy', 'wavelength'}
     assert set(tof.kinematic('wavelength').keys()) == {'energy'}
     assert set(tof.kinematic('energy').keys()) == {'wavelength'}
 
 
-@pytest.mark.parametrize('start', ('dspacing', 'Q'))
+@pytest.mark.parametrize('start', ['dspacing', 'Q'])
 def test_kinematic_unsupported_starts(start):
     with pytest.raises(KeyError):
         tof.kinematic(start)
 
 
 def test_elastic_dspacing():
     assert set(tof.elastic_dspacing('energy').keys()) == {'dspacing'}
     assert set(tof.elastic_dspacing('tof').keys()) == {'dspacing'}
     assert set(tof.elastic_dspacing('wavelength').keys()) == {'dspacing'}
 
 
-@pytest.mark.parametrize('start', ('Q',))
+@pytest.mark.parametrize('start', ['Q'])
 def test_elastic_dspacing_unsupported_starts(start):
     with pytest.raises(KeyError):
         tof.elastic_dspacing(start)
 
 
 def test_elastic_energy():
     assert set(tof.elastic_energy('tof').keys()) == {'energy'}
     assert set(tof.elastic_energy('wavelength').keys()) == {'energy'}
 
 
-@pytest.mark.parametrize('start', ('Q', 'dspacing'))
+@pytest.mark.parametrize('start', ['Q', 'dspacing'])
 def test_elastic_energy_unsupported_starts(start):
     with pytest.raises(KeyError):
         tof.elastic_energy(start)
 
 
 def test_elastic_Q():
     assert set(tof.elastic_Q('tof').keys()) == {'Q', 'wavelength'}
     assert set(tof.elastic_Q('wavelength').keys()) == {'Q'}
 
 
-@pytest.mark.parametrize('start', ('energy', 'dspacing'))
+@pytest.mark.parametrize('start', ['energy', 'dspacing'])
 def test_elastic_Q_unsupported_starts(start):
     with pytest.raises(KeyError):
         tof.elastic_Q(start)
 
 
 def test_elastic_wavelength():
     assert set(tof.elastic_wavelength('energy').keys()) == {'wavelength'}
     assert set(tof.elastic_wavelength('tof').keys()) == {'wavelength'}
     assert set(tof.elastic_wavelength('Q').keys()) == {'wavelength'}
 
 
-@pytest.mark.parametrize('start', ('dspacing',))
+@pytest.mark.parametrize('start', ['dspacing'])
 def test_elastic_wavelength_unsupported_starts(start):
     with pytest.raises(KeyError):
         tof.elastic_wavelength(start)
 
 
 def test_direct_inelastic():
     assert set(tof.direct_inelastic('tof').keys()) == {'energy_transfer'}
 
 
-@pytest.mark.parametrize('start', ('wavelength', 'Q', 'dspacing'))
+@pytest.mark.parametrize('start', ['wavelength', 'Q', 'dspacing'])
 def test_direct_inelastic_unsupported_starts(start):
     with pytest.raises(KeyError):
         tof.direct_inelastic(start)
 
 
 def test_indirect_inelastic():
     assert set(tof.indirect_inelastic('tof').keys()) == {'energy_transfer'}
 
 
-@pytest.mark.parametrize('start', ('wavelength', 'Q', 'dspacing'))
+@pytest.mark.parametrize('start', ['wavelength', 'Q', 'dspacing'])
 def test_indirect_inelastic_unsupported_starts(start):
     with pytest.raises(KeyError):
         tof.indirect_inelastic(start)
 
 
 @pytest.mark.parametrize(
     'arg',
-    (
+    [
         (tof.elastic, ('energy', 'tof', 'Q', 'wavelength')),
         (tof.kinematic, ('tof', 'wavelength', 'energy')),
         (tof.elastic_dspacing, ('tof', 'wavelength', 'energy')),
         (tof.elastic_energy, ('tof', 'wavelength')),
         (tof.elastic_Q, ('tof', 'wavelength')),
         (tof.elastic_wavelength, ('tof', 'energy', 'Q')),
         (tof.direct_inelastic, ('tof',)),
         (tof.indirect_inelastic, ('tof',)),
-    ),
+    ],
 )
 def test_returns_new_graph(arg):
     fn, starts = arg
     for start in starts:
         g = fn(start)
         g['a_new_node'] = lambda position: 2 * position
         assert 'a_new_node' not in fn(start)
```

### Comparing `scippneutron-24.3.0/tests/conversion/tof_conversions_test.py` & `scippneutron-24.5.0/tests/conversion/tof_conversions_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,23 +127,23 @@
 def test_wavelength_from_tof(tof, Ltotal):
     wavelength = tof_conv.wavelength_from_tof(tof=tof, Ltotal=Ltotal)
     assert sc.allclose(
         wavelength, sc.to_unit(const.h * tof / const.m_n / Ltotal, unit='angstrom')
     )
 
 
-@pytest.mark.parametrize('tof_dtype', ('float64', 'int64', 'int32'))
-@pytest.mark.parametrize('Ltotal_dtype', ('float64', 'float32', 'int64', 'int32'))
+@pytest.mark.parametrize('tof_dtype', ['float64', 'int64', 'int32'])
+@pytest.mark.parametrize('Ltotal_dtype', ['float64', 'float32', 'int64', 'int32'])
 def test_wavelength_from_tof_double_precision(tof_dtype, Ltotal_dtype):
     tof = sc.scalar(1.2, unit='s', dtype=tof_dtype)
     Ltotal = sc.scalar(10.1, unit='m', dtype=Ltotal_dtype)
     assert tof_conv.wavelength_from_tof(tof=tof, Ltotal=Ltotal).dtype == 'float64'
 
 
-@pytest.mark.parametrize('Ltotal_dtype', ('float64', 'float32', 'int64', 'int32'))
+@pytest.mark.parametrize('Ltotal_dtype', ['float64', 'float32', 'int64', 'int32'])
 def test_wavelength_from_tof_single_precision(Ltotal_dtype):
     tof = sc.scalar(1.2, unit='s', dtype='float32')
     Ltotal = sc.scalar(10.1, unit='m', dtype=Ltotal_dtype)
     assert tof_conv.wavelength_from_tof(tof=tof, Ltotal=Ltotal).dtype == 'float32'
 
 
 @given(
@@ -161,29 +161,29 @@
         sc.to_unit(
             const.h * tof / const.m_n / Ltotal / 2 / sc.sin(two_theta / 2),
             unit='angstrom',
         ),
     )
 
 
-@pytest.mark.parametrize('tof_dtype', ('float64', 'int64', 'int32'))
-@pytest.mark.parametrize('Ltotal_dtype', ('float64', 'float32', 'int64', 'int32'))
-@pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64', 'int32'))
+@pytest.mark.parametrize('tof_dtype', ['float64', 'int64', 'int32'])
+@pytest.mark.parametrize('Ltotal_dtype', ['float64', 'float32', 'int64', 'int32'])
+@pytest.mark.parametrize('two_theta_dtype', ['float64', 'float32', 'int64', 'int32'])
 def test_dspacing_from_tof_double_precision(tof_dtype, Ltotal_dtype, two_theta_dtype):
     tof = sc.scalar(52.0, unit='s', dtype=tof_dtype)
     Ltotal = sc.scalar(0.341, unit='m', dtype=Ltotal_dtype)
     two_theta = sc.scalar(1.68, unit='rad', dtype=two_theta_dtype)
     assert (
         tof_conv.dspacing_from_tof(tof=tof, Ltotal=Ltotal, two_theta=two_theta).dtype
         == 'float64'
     )
 
 
-@pytest.mark.parametrize('Ltotal_dtype', ('float64', 'float32', 'int64', 'int32'))
-@pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64', 'int32'))
+@pytest.mark.parametrize('Ltotal_dtype', ['float64', 'float32', 'int64', 'int32'])
+@pytest.mark.parametrize('two_theta_dtype', ['float64', 'float32', 'int64', 'int32'])
 def test_dspacing_from_tof_single_precision(Ltotal_dtype, two_theta_dtype):
     tof = sc.scalar(52.0, unit='s', dtype='float32')
     Ltotal = sc.scalar(0.341, unit='m', dtype=Ltotal_dtype)
     two_theta = sc.scalar(1.68, unit='rad', dtype=two_theta_dtype)
     assert (
         tof_conv.dspacing_from_tof(tof=tof, Ltotal=Ltotal, two_theta=two_theta).dtype
         == 'float32'
@@ -195,23 +195,23 @@
 def test_energy_from_tof(tof, Ltotal):
     energy = tof_conv.energy_from_tof(tof=tof, Ltotal=Ltotal)
     assert sc.allclose(
         energy, sc.to_unit(const.m_n * Ltotal**2 / 2 / tof**2, unit='meV')
     )
 
 
-@pytest.mark.parametrize('tof_dtype', ('float64', 'int64'))
-@pytest.mark.parametrize('Ltotal_dtype', ('float64', 'float32', 'int64'))
+@pytest.mark.parametrize('tof_dtype', ['float64', 'int64'])
+@pytest.mark.parametrize('Ltotal_dtype', ['float64', 'float32', 'int64'])
 def test_energy_from_tof_double_precision(tof_dtype, Ltotal_dtype):
     tof = sc.scalar(478.9, unit='s', dtype=tof_dtype)
     Ltotal = sc.scalar(1.256, unit='m', dtype=Ltotal_dtype)
     assert tof_conv.energy_from_tof(tof=tof, Ltotal=Ltotal).dtype == 'float64'
 
 
-@pytest.mark.parametrize('Ltotal_dtype', ('float64', 'float32', 'int64'))
+@pytest.mark.parametrize('Ltotal_dtype', ['float64', 'float32', 'int64'])
 def test_energy_from_tof_single_precision(Ltotal_dtype):
     tof = sc.scalar(478.9, unit='s', dtype='float32')
     Ltotal = sc.scalar(1.256, unit='m', dtype=Ltotal_dtype)
     assert tof_conv.energy_from_tof(tof=tof, Ltotal=Ltotal).dtype == 'float32'
 
 
 @given(
@@ -272,15 +272,15 @@
 def test_energy_from_wavelength(wavelength):
     energy = tof_conv.energy_from_wavelength(wavelength=wavelength)
     assert sc.allclose(
         energy, sc.to_unit(const.h**2 / 2 / const.m_n / wavelength**2, unit='meV')
     )
 
 
-@pytest.mark.parametrize('wavelength_dtype', ('float64', 'int64'))
+@pytest.mark.parametrize('wavelength_dtype', ['float64', 'int64'])
 def test_energy_from_wavelength_double_precision(wavelength_dtype):
     wavelength = sc.scalar(60.5, unit='m', dtype=wavelength_dtype)
     assert tof_conv.energy_from_wavelength(wavelength=wavelength).dtype == 'float64'
 
 
 def test_energy_from_wavelength_single_precision():
     wavelength = sc.scalar(60.5, unit='m', dtype='float32')
@@ -293,15 +293,15 @@
     wavelength = tof_conv.wavelength_from_energy(energy=energy)
     assert sc.allclose(
         wavelength,
         sc.to_unit(const.h / sc.sqrt(2 * const.m_n * energy), unit='angstrom'),
     )
 
 
-@pytest.mark.parametrize('energy_dtype', ('float64', 'int64'))
+@pytest.mark.parametrize('energy_dtype', ['float64', 'int64'])
 def test_wavelength_from_energy_double_precision(energy_dtype):
     energy = sc.scalar(61.0, unit='meV', dtype=energy_dtype)
     assert tof_conv.wavelength_from_energy(energy=energy).dtype == 'float64'
 
 
 def test_wavelength_from_energy_single_precision():
     energy = sc.scalar(61.0, unit='meV', dtype='float32')
@@ -311,26 +311,26 @@
 @given(wavelength=space_variables(), two_theta=angle_variables())
 @settings(**global_settings)
 def test_Q_from_wavelength(wavelength, two_theta):
     Q = tof_conv.Q_from_wavelength(wavelength=wavelength, two_theta=two_theta)
     assert sc.allclose(Q, 4 * np.pi * sc.sin(two_theta / 2) / wavelength)
 
 
-@pytest.mark.parametrize('wavelength_dtype', ('float64', 'int64'))
-@pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
+@pytest.mark.parametrize('wavelength_dtype', ['float64', 'int64'])
+@pytest.mark.parametrize('two_theta_dtype', ['float64', 'float32', 'int64'])
 def test_Q_from_wavelength_double_precision(wavelength_dtype, two_theta_dtype):
     wavelength = sc.scalar(3.51, unit='s', dtype=wavelength_dtype)
     two_theta = sc.scalar(0.041, unit='deg', dtype=two_theta_dtype)
     assert (
         tof_conv.Q_from_wavelength(wavelength=wavelength, two_theta=two_theta).dtype
         == 'float64'
     )
 
 
-@pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
+@pytest.mark.parametrize('two_theta_dtype', ['float64', 'float32', 'int64'])
 def test_Q_from_wavelength_single_precision(two_theta_dtype):
     wavelength = sc.scalar(3.51, unit='s', dtype='float32')
     two_theta = sc.scalar(0.041, unit='deg', dtype=two_theta_dtype)
     assert (
         tof_conv.Q_from_wavelength(wavelength=wavelength, two_theta=two_theta).dtype
         == 'float32'
     )
@@ -342,23 +342,23 @@
     Q.unit = f'1/{Q.unit}'
     wavelength = tof_conv.wavelength_from_Q(Q=Q, two_theta=two_theta)
     assert sc.allclose(
         wavelength, sc.to_unit(4 * np.pi * sc.sin(two_theta / 2) / Q, unit='angstrom')
     )
 
 
-@pytest.mark.parametrize('Q_dtype', ('float64', 'int64'))
-@pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
+@pytest.mark.parametrize('Q_dtype', ['float64', 'int64'])
+@pytest.mark.parametrize('two_theta_dtype', ['float64', 'float32', 'int64'])
 def test_wavelength_from_Q_double_precision(Q_dtype, two_theta_dtype):
     Q = sc.scalar(4.151, unit='1/nm', dtype=Q_dtype)
     two_theta = sc.scalar(5.71, unit='deg', dtype=two_theta_dtype)
     assert tof_conv.wavelength_from_Q(Q=Q, two_theta=two_theta).dtype == 'float64'
 
 
-@pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
+@pytest.mark.parametrize('two_theta_dtype', ['float64', 'float32', 'int64'])
 def test_wavelength_from_Q_single_precision(two_theta_dtype):
     Q = sc.scalar(4.151, unit='1/nm', dtype='float32')
     two_theta = sc.scalar(5.71, unit='deg', dtype=two_theta_dtype)
     assert tof_conv.wavelength_from_Q(Q=Q, two_theta=two_theta).dtype == 'float32'
 
 
 @given(incident_beam=vector_variables(), wavelength=space_variables())
@@ -436,28 +436,28 @@
         wavelength=wavelength, two_theta=two_theta
     )
     assert sc.allclose(
         dspacing, sc.to_unit(wavelength / 2 / sc.sin(two_theta / 2), unit='angstrom')
     )
 
 
-@pytest.mark.parametrize('wavelength_dtype', ('float64', 'int64'))
-@pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
+@pytest.mark.parametrize('wavelength_dtype', ['float64', 'int64'])
+@pytest.mark.parametrize('two_theta_dtype', ['float64', 'float32', 'int64'])
 def test_dspacing_from_wavelength_double_precision(wavelength_dtype, two_theta_dtype):
     wavelength = sc.scalar(41.4, unit='m', dtype=wavelength_dtype)
     two_theta = sc.scalar(8.4, unit='rad', dtype=two_theta_dtype)
     assert (
         tof_conv.dspacing_from_wavelength(
             wavelength=wavelength, two_theta=two_theta
         ).dtype
         == 'float64'
     )
 
 
-@pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
+@pytest.mark.parametrize('two_theta_dtype', ['float64', 'float32', 'int64'])
 def test_dspacing_from_wavelength_single_precision(two_theta_dtype):
     wavelength = sc.scalar(41.4, unit='m', dtype='float32')
     two_theta = sc.scalar(8.4, unit='rad', dtype=two_theta_dtype)
     assert (
         tof_conv.dspacing_from_wavelength(
             wavelength=wavelength, two_theta=two_theta
         ).dtype
@@ -474,26 +474,26 @@
         sc.to_unit(
             const.h / sc.sqrt(8 * const.m_n * energy) / sc.sin(two_theta / 2),
             unit='angstrom',
         ),
     )
 
 
-@pytest.mark.parametrize('energy_dtype', ('float64', 'int64'))
-@pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
+@pytest.mark.parametrize('energy_dtype', ['float64', 'int64'])
+@pytest.mark.parametrize('two_theta_dtype', ['float64', 'float32', 'int64'])
 def test_dspacing_from_energy_double_precision(energy_dtype, two_theta_dtype):
     energy = sc.scalar(26.90, unit='J', dtype=energy_dtype)
     two_theta = sc.scalar(1.985, unit='rad', dtype=two_theta_dtype)
     assert (
         tof_conv.dspacing_from_energy(energy=energy, two_theta=two_theta).dtype
         == 'float64'
     )
 
 
-@pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
+@pytest.mark.parametrize('two_theta_dtype', ['float64', 'float32', 'int64'])
 def test_dspacing_from_energy_single_precision(two_theta_dtype):
     energy = sc.scalar(26.90, unit='J', dtype='float32')
     two_theta = sc.scalar(1.985, unit='rad', dtype=two_theta_dtype)
     assert (
         tof_conv.dspacing_from_energy(energy=energy, two_theta=two_theta).dtype
         == 'float32'
     )
@@ -601,21 +601,21 @@
         2 * np.pi * (sample_rotation_matrix * u_matrix * b_matrix * hkl_vec)
     )
     assert sc.allclose(reconstructed_Q, Q_vec)
 
 
 def test_hkl_elements_from_hkl_vec():
     hkl_vec = sc.vector([3.1, 4.5, 6.9])
-    h, k, l = tof_conv.hkl_elements_from_hkl_vec(hkl_vec=hkl_vec)
+    h, k, l = tof_conv.hkl_elements_from_hkl_vec(hkl_vec=hkl_vec)  # noqa: E741
     sc.testing.assert_identical(h, hkl_vec.fields.x)
     sc.testing.assert_identical(k, hkl_vec.fields.y)
     sc.testing.assert_identical(l, hkl_vec.fields.z)
 
 
-@pytest.mark.parametrize('pulse_time', (0.0, 1.0))
+@pytest.mark.parametrize('pulse_time', [0.0, 1.0])
 def test_time_at_sample(pulse_time):
     ts = tof_conv.time_at_sample_from_tof(
         pulse_time=sc.scalar(pulse_time, unit='s'),
         tof=sc.scalar(3.0, unit='s'),
         L2=sc.scalar(2.0, unit='m'),
         wavelength=(sc.constants.h / sc.constants.m_n / sc.scalar(2.0, unit='m/s')).to(
             unit='Å'
```

### Comparing `scippneutron-24.3.0/tests/convert_test.py` & `scippneutron-24.5.0/tests/convert_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 def make_dataset_in(dim):
     tof_dset = make_test_data(coords=('tof', 'Ltotal', 'two_theta'), dataset=True)
     return scn.convert(tof_dset, origin='tof', target=dim, scatter=True)
 
 
 @pytest.mark.parametrize(
     ('origin', 'target'),
-    (('tof', 'dspacing'), ('tof', 'wavelength'), ('tof', 'energy')),
+    [('tof', 'dspacing'), ('tof', 'wavelength'), ('tof', 'energy')],
 )
 def test_convert_dataset_vs_dataarray(origin, target):
     inputs = make_dataset_in(origin)
     expected = scn.convert(inputs, origin=origin, target=target, scatter=True)
     result = sc.Dataset(
         data={
             name: scn.convert(data.copy(), origin=origin, target=target, scatter=True)
@@ -199,15 +199,15 @@
 
     wavelength = scn.convert(tof, origin='tof', target='wavelength', scatter=True)
     scn.convert(wavelength, origin='wavelength', target='Q', scatter=True)
     with pytest.raises(RuntimeError):
         scn.convert(wavelength, origin='wavelength', target='Q', scatter=False)
 
 
-@pytest.mark.parametrize('target', ('incident_beam', 'scattered_beam'))
+@pytest.mark.parametrize('target', ['incident_beam', 'scattered_beam'])
 def test_convert_beams(target):
     def check_positions(data):
         assert not data.coords['sample_position'].aligned
         assert data.coords['source_position'].aligned == (target == 'scattered_beam')
         assert data.coords['position'].aligned == (target == 'incident_beam')
 
     # A single sample position.
@@ -246,20 +246,20 @@
             ),
             rtol=1e-14 * sc.units.one,
         )
 
 
 @pytest.mark.parametrize(
     ('target', 'make_ref'),
-    (
+    [
         ('L1', make_L1),
         ('L2', make_L2),
         ('two_theta', make_two_theta),
         ('Ltotal', lambda: make_L1() + make_L2()),
-    ),
+    ],
 )
 def test_convert_beam_length_and_angle(target, make_ref):
     original = make_test_data(coords=('incident_beam', 'scattered_beam'))
     converted = scn.convert(original, origin='position', target=target, scatter=True)
     assert sc.allclose(converted.coords[target], make_ref(), rtol=sc.scalar(1e-12))
 
 
@@ -279,26 +279,30 @@
     # v [m/s] = 3956 / \lambda [ Angstrom ]
     tof_in_seconds = tof.coords['tof'] * 1e-6
 
     # Spectrum 0 is 11 m from source
     # 2d sin(theta) = n \lambda
     # theta = 45 deg => d = lambda / (2 * 1 / sqrt(2))
     for val, t in zip(
-        dspacing.coords['dspacing']['spectrum', 0].values, tof_in_seconds.values
+        dspacing.coords['dspacing']['spectrum', 0].values,
+        tof_in_seconds.values,
+        strict=True,
     ):
         np.testing.assert_almost_equal(
             val, 3956.0 / (11.0 / t) / math.sqrt(2.0), val * 1e-3
         )
 
     # Spectrum 1
     # sin(2 theta) = 0.1/(L-10)
     L = 10.0 + math.sqrt(1.0 * 1.0 + 0.1 * 0.1)
     lambda_to_d = 1.0 / (2.0 * math.sin(0.5 * math.asin(0.1 / (L - 10.0))))
     for val, t in zip(
-        dspacing.coords['dspacing']['spectrum', 1].values, tof_in_seconds.values
+        dspacing.coords['dspacing']['spectrum', 1].values,
+        tof_in_seconds.values,
+        strict=True,
     ):
         np.testing.assert_almost_equal(val, 3956.0 / (L / t) * lambda_to_d, val * 1e-3)
 
 
 def test_convert_tof_to_wavelength():
     tof = make_test_data(coords=('tof', 'Ltotal'), dataset=True)
     wavelength = scn.convert(tof, origin='tof', target='wavelength', scatter=True)
@@ -306,21 +310,25 @@
 
     # Rule of thumb (https://www.psi.ch/niag/neutron-physics):
     # v [m/s] = 3956 / \lambda [ Angstrom ]
     tof_in_seconds = tof.coords['tof'] * 1e-6
 
     # Spectrum 0 is 11 m from source
     for val, t in zip(
-        wavelength.coords['wavelength']['spectrum', 0].values, tof_in_seconds.values
+        wavelength.coords['wavelength']['spectrum', 0].values,
+        tof_in_seconds.values,
+        strict=True,
     ):
         np.testing.assert_almost_equal(val, 3956.0 / (11.0 / t), val * 1e-3)
     # Spectrum 1
     L = 10.0 + math.sqrt(1.0 * 1.0 + 0.1 * 0.1)
     for val, t in zip(
-        wavelength.coords['wavelength']['spectrum', 1].values, tof_in_seconds.values
+        wavelength.coords['wavelength']['spectrum', 1].values,
+        tof_in_seconds.values,
+        strict=True,
     ):
         np.testing.assert_almost_equal(val, 3956.0 / (L / t), val * 1e-3)
 
 
 def test_convert_tof_to_wavelength_no_scatter():
     # scatter=True and scatter=False only differ in how Ltotal is computed.
     tof = make_test_data(coords=('tof', 'Ltotal'), dataset=True)
@@ -347,26 +355,30 @@
     # v [m/s] = 3956 / \lambda [ Angstrom ]
     tof_in_seconds = tof.coords['tof'] * 1e-6
 
     # Spectrum 0 is 11 m from source
     # Q = 4pi sin(theta) / lambda
     # theta = 45 deg => Q = 2 sqrt(2) pi / lambda
     for val, t in zip(
-        Q_from_wavelength.coords['Q']['spectrum', 0].values, tof_in_seconds.values
+        Q_from_wavelength.coords['Q']['spectrum', 0].values,
+        tof_in_seconds.values,
+        strict=True,
     ):
         np.testing.assert_almost_equal(
             val, 2.0 * math.sqrt(2.0) * math.pi / (3956.0 / (11.0 / t)), val * 1e-3
         )
 
     # Spectrum 1
     # sin(2 theta) = 0.1/(L-10)
     L = 10.0 + math.sqrt(1.0 * 1.0 + 0.1 * 0.1)
     lambda_to_Q = 4.0 * math.pi * math.sin(math.asin(0.1 / (L - 10.0)) / 2.0)
     for val, t in zip(
-        Q_from_wavelength.coords['Q']['spectrum', 1].values, tof_in_seconds.values
+        Q_from_wavelength.coords['Q']['spectrum', 1].values,
+        tof_in_seconds.values,
+        strict=True,
     ):
         np.testing.assert_almost_equal(
             val, lambda_to_Q / (3956.0 / (L / t)), val * 1e-3
         )
 
 
 def test_convert_Q_to_wavelength():
@@ -392,23 +404,27 @@
     tof_in_seconds = sc.to_unit(tof.coords['tof'], 's')
     # e [J] = 1/2 m(n) [kg] (l [m] / tof [s])^2
     joule_to_mev = sc.to_unit(1.0 * sc.Unit('J'), sc.units.meV).value
     neutron_mass = sc.to_unit(m_n, sc.units.kg).value
 
     # Spectrum 0 is 11 m from source
     for val, t in zip(
-        energy.coords['energy']['spectrum', 0].values, tof_in_seconds.values
+        energy.coords['energy']['spectrum', 0].values,
+        tof_in_seconds.values,
+        strict=True,
     ):
         np.testing.assert_almost_equal(
             val, joule_to_mev * neutron_mass / 2 * (11 / t) ** 2, val * 1e-3
         )
     # Spectrum 1
     L = 10.0 + math.sqrt(1.0 * 1.0 + 0.1 * 0.1)
     for val, t in zip(
-        energy.coords['energy']['spectrum', 1].values, tof_in_seconds.values
+        energy.coords['energy']['spectrum', 1].values,
+        tof_in_seconds.values,
+        strict=True,
     ):
         np.testing.assert_almost_equal(
             val, joule_to_mev * 0.5 * neutron_mass * (L / t) ** 2, val * 1e-3
         )
 
 
 def test_convert_tof_to_energy_elastic_no_scatter():
@@ -535,24 +551,24 @@
         rtol=0.0 * sc.units.one,
         atol=1e-11 * sc.units.meV,
     )
 
 
 # Test conversions between quantities that are themselves
 # outputs of conversions from tof.
-@pytest.mark.parametrize('keep_tof', (False, True))
+@pytest.mark.parametrize('keep_tof', [False, True])
 @pytest.mark.parametrize(
     ('target', 'target_unit'),
-    (
+    [
         ('energy', sc.units.meV),
         ('wavelength', sc.units.angstrom),
         ('dspacing', sc.units.angstrom),
-    ),
+    ],
 )
-@pytest.mark.parametrize('origin', ('energy', 'wavelength'))
+@pytest.mark.parametrize('origin', ['energy', 'wavelength'])
 def test_convert_non_tof(origin, target, target_unit, keep_tof):
     tof = make_test_data(coords=('tof', 'Ltotal', 'two_theta'), dataset=True)
     original = scn.convert(tof, origin='tof', target=origin, scatter=True)
     if not keep_tof:
         del original.coords['tof']
     converted = scn.convert(original, origin=origin, target=target, scatter=True)
     check_tof_conversion_metadata(converted, target, target_unit)
@@ -592,17 +608,17 @@
     expected = scn.convert(da_float_coord, origin='tof', target=target, scatter=True)
     assert res.coords[target].dtype == sc.DType.float64
     assert sc.allclose(
         res.coords[target], expected.coords[target], rtol=1e-15 * sc.units.one
     )
 
 
-@pytest.mark.parametrize('input_energy', ('incident_energy', 'final_energy'))
+@pytest.mark.parametrize('input_energy', ['incident_energy', 'final_energy'])
 @pytest.mark.parametrize(
-    'input_dtypes', (('int64', 'float64'), ('float64', 'int64'), ('int64', 'int64'))
+    'input_dtypes', [('int64', 'float64'), ('float64', 'int64'), ('int64', 'int64')]
 )
 def test_convert_integer_input_inelastic(input_energy, input_dtypes):
     da_float_coord = make_test_data(coords=('tof', 'L1', 'L2', 'two_theta'))
     da_float_coord.coords[input_energy] = sc.scalar(
         35, dtype=sc.DType.float64, unit=sc.units.meV
     )
```

### Comparing `scippneutron-24.3.0/tests/data_stream_test.py` & `scippneutron-24.5.0/tests/data_stream_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,49 +3,50 @@
 import datetime
 import multiprocessing as mp
 import platform
 import sys
 import warnings
 from cmath import isclose
 from pathlib import Path
-from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import pytest
 import scipp as sc
 
 from scippneutron._utils import get_attrs
 from scippneutron.data_streaming._consumer_type import ConsumerType
 from scippneutron.data_streaming._warnings import (
     BufferSizeWarning,
     UnknownFlatbufferIdWarning,
 )
 
 sys.path.insert(0, str(Path(__file__).resolve().parent / 'io'))
-from nexus_helpers import EventData, Log, NexusBuilder, Stream  # noqa: E402
+from nexus_helpers import EventData, Log, NexusBuilder, Stream
 
 if platform.system() == "Darwin":
     pytest.skip(
         "Streaming tests disabled on MacOS because they tend to hang"
         " indefinitely for unknown reasons",
         allow_module_level=True,
     )
 
 try:
     import streaming_data_types  # noqa: F401
-    from confluent_kafka import KafkaError, TopicPartition  # noqa: F401
-    from streaming_data_types.eventdata_ev42 import serialise_ev42  # noqa: E402
+    from confluent_kafka import KafkaError, TopicPartition
+    from streaming_data_types.eventdata_ev42 import serialise_ev42
     from streaming_data_types.logdata_f142 import serialise_f142
     from streaming_data_types.run_start_pl72 import serialise_pl72
     from streaming_data_types.sample_environment_senv import Location, serialise_senv
     from streaming_data_types.timestamps_tdct import serialise_tdct
 
     from scippneutron.data_streaming._consumer import RunStartError
-    from scippneutron.data_streaming.data_stream import _data_stream  # noqa: E402
-    from scippneutron.data_streaming.data_stream import StopTime
+    from scippneutron.data_streaming.data_stream import (
+        StopTime,
+        _data_stream,
+    )
 except ImportError:
     pytest.skip("Kafka or Serialisation module is unavailable", allow_module_level=True)
 
 
 class FakeKafkaError:
     def __init__(self, kafka_error_code: int):
         self._error_code = kafka_error_code
@@ -55,71 +56,71 @@
 
     def __str__(self):
         return f"FakeKafkaError: code {self._error_code}"
 
 
 class FakeMessage:
     def __init__(
-        self, payload: bytes, error_code: Optional[int] = None, timestamp: int = 0
+        self, payload: bytes, error_code: int | None = None, timestamp: int = 0
     ):
         self._payload = payload
         self._error_code = error_code
         self._timestamp = timestamp
 
     def value(self):
         return self._payload
 
-    def error(self) -> Optional[KafkaError]:
+    def error(self) -> KafkaError | None:
         if self._error_code is not None:
             return FakeKafkaError(self._error_code)
         return None
 
-    def timestamp(self) -> Tuple[None, int]:
+    def timestamp(self) -> tuple[None, int]:
         return None, self._timestamp
 
 
 class FakeQueryConsumer:
     def __init__(
         self,
         instrument_name: str = "",
-        low_and_high_offset: Tuple[int, int] = (2, 10),
-        streams: List[Stream] = None,
-        start_time: Optional[Union[int, datetime.datetime]] = None,
-        stop_time: Optional[Union[int, datetime.datetime]] = None,
-        nexus_structure: Optional[str] = None,
+        low_and_high_offset: tuple[int, int] = (2, 10),
+        streams: list[Stream] | None = None,
+        start_time: int | datetime.datetime | None = None,
+        stop_time: int | datetime.datetime | None = None,
+        nexus_structure: str | None = None,
     ):
         self._instrument_name = instrument_name
         self._low_and_high_offset = low_and_high_offset
         self._streams = streams
         self.queried_topics = []
         self.queried_timestamp = None
         self._start_time = start_time
         self._stop_time = stop_time
         if self._start_time is None:
-            self._start_time = datetime.datetime.now()
+            self._start_time = datetime.datetime.now(tz=datetime.timezone.utc)
         if nexus_structure is None:
             builder = NexusBuilder()
             builder.add_instrument(self._instrument_name)
             if self._streams is not None:
                 for stream in self._streams:
                     builder.add_stream(stream)
             self._nexus_structure = builder.json_string
         else:
             self._nexus_structure = nexus_structure
 
     @staticmethod
-    def assign(partitions: List[TopicPartition]):
+    def assign(partitions: list[TopicPartition]):
         pass
 
-    def get_watermark_offsets(self, partition: TopicPartition) -> Tuple[int, int]:
+    def get_watermark_offsets(self, partition: TopicPartition) -> tuple[int, int]:
         return self._low_and_high_offset
 
     def get_topic_partitions(
         self, topic: str, offset: int = -1
-    ) -> List[TopicPartition]:
+    ) -> list[TopicPartition]:
         self.queried_topics.append(topic)
         return [TopicPartition(topic, partition=0, offset=offset)]
 
     def poll(self, timeout=2.0) -> FakeMessage:
         return FakeMessage(
             serialise_pl72(
                 "",
@@ -129,15 +130,15 @@
                 nexus_structure=self._nexus_structure,
             )
         )
 
     def seek(self, partition: TopicPartition):
         pass
 
-    def offsets_for_times(self, partitions: List[TopicPartition]):
+    def offsets_for_times(self, partitions: list[TopicPartition]):
         self.queried_timestamp = partitions[0].offset
         return partitions
 
 
 # Short time to use for buffer emit and data_stream interval in tests
 # pass or fail fast!
 SHORT_TEST_INTERVAL = 100.0 * sc.Unit('milliseconds')
@@ -156,27 +157,27 @@
     "timeout": 10.0 * sc.units.s,
 }
 # "timeout" arg: if something gets broken then this makes sure the
 # test will not get stuck in the _data_stream loop indefinitely.
 # A TimeoutError is raised by _data_stream if the timeout occurs.
 
 
-@pytest.fixture(scope="function")
+@pytest.fixture()
 def queues():
     # Specify to start the process using the "spawn" method, otherwise
     # on Linux the default is to fork the Python interpreter which
     # is "problematic" in a multithreaded process, in our case the use of
     # asyncio means the process is multithreaded.
     # See documentation:
     # https://docs.python.org/3/library/multiprocessing.html#contexts-and-start-methods
     ctx = mp.get_context("spawn")
     return ctx.Queue(), ctx.Queue(), ctx.Queue()
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_stream_returns_data_from_single_event_message(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     time_of_flight = np.array([1.0, 2.0, 3.0])
     detector_ids = np.array([4, 5, 6])
     test_message = FakeMessage(
         serialise_ev42("detector", 0, 0, time_of_flight, detector_ids)
     )
@@ -192,15 +193,15 @@
         **TEST_STREAM_ARGS,
     ):
         assert np.allclose(data.coords['tof'].values, time_of_flight)
         reached_assert = True
     assert reached_assert
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_stream_returns_data_from_multiple_event_messages(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     first_tof = np.array([1.0, 2.0, 3.0])
     first_detector_ids = np.array([4, 5, 6])
     first_test_message = serialise_ev42("detector", 0, 0, first_tof, first_detector_ids)
     second_tof = np.array([1.0, 2.0, 3.0])
     second_detector_ids = np.array([4, 5, 6])
@@ -223,15 +224,15 @@
         assert np.allclose(data.coords['tof'].values, expected_tofs)
         expected_ids = np.concatenate((first_detector_ids, second_detector_ids))
         assert np.array_equal(data.coords['detector_id'].values, expected_ids)
         reached_asserts = True
     assert reached_asserts
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_warn_if_unrecognised_message_was_encountered(queues):
     warnings.filterwarnings("error")
     data_queue, worker_instruction_queue, test_message_queue = queues
     # First 4 bytes of the message payload are the FlatBuffer schema identifier
     # "abcd" does not correspond to a FlatBuffer schema for data
     # that scipp is interested in
     test_message = b"abcd0000"
@@ -245,15 +246,15 @@
             test_message_queue=test_message_queue,
             query_consumer=FakeQueryConsumer(),
             **TEST_STREAM_ARGS,
         ):
             test_message_queue.put(FakeMessage(test_message))
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_warn_on_buffer_size_exceeded_by_single_message(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     buffer_size_2_events = 2
     time_of_flight = np.array([1.0, 2.0, 3.0])
     detector_ids = np.array([4, 5, 6])
     test_message = serialise_ev42("detector", 0, 0, time_of_flight, detector_ids)
 
@@ -269,15 +270,15 @@
             test_message_queue=test_message_queue,
             query_consumer=FakeQueryConsumer(),
             **test_steam_args,
         ):
             test_message_queue.put(FakeMessage(test_message))
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_returned_when_buffer_size_exceeded_by_event_messages(queues):
     # Messages cumulatively exceed the buffer size, data_stream
     # will return multiple chunks of data to clear the buffer
     # between messages.
     data_queue, worker_instruction_queue, test_message_queue = queues
     first_tof = np.array([1.0, 2.0, 3.0])
     first_detector_ids = np.array([4, 5, 6])
@@ -317,15 +318,15 @@
             assert np.allclose(data.coords['tof'].values, second_tof)
             reached_asserts = True
 
         n_chunks += 1
     assert reached_asserts
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_are_loaded_from_run_start_message(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     reached_assert = False
     test_instrument_name = "DATA_STREAM_TEST"
     async for data in _data_stream(
         data_queue,
@@ -337,57 +338,63 @@
         **TEST_STREAM_ARGS,
     ):
         assert data["instrument_name"].value == test_instrument_name
         reached_assert = True
     assert reached_assert
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_error_raised_if_no_run_start_message_available(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # Low and high offset are the same value, indicates there are
     # no messages available in the partition
     low_and_high_offset = (0, 0)
-    with pytest.raises(RunStartError):
-        async for _ in _data_stream(
+    stream = aiter(
+        _data_stream(
             data_queue,
             worker_instruction_queue,
             run_info_topic=run_info_topic,
             halt_after_n_data_chunks=0,
             test_message_queue=test_message_queue,
             query_consumer=FakeQueryConsumer(test_instrument_name, low_and_high_offset),
             **TEST_STREAM_ARGS,
-        ):
-            pass
+        )
+    )
+    with pytest.raises(RunStartError):
+        await anext(stream)
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_error_if_both_topics_and_run_start_topic_not_specified(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     # At least one of "topics" and "run_start_topic" must be specified
-    with pytest.raises(ValueError):
-        async for _ in _data_stream(
+    stream = aiter(
+        _data_stream(
             data_queue,
             worker_instruction_queue,
             run_info_topic=None,
             halt_after_n_data_chunks=0,
             **test_stream_args,
             query_consumer=FakeQueryConsumer(),
             test_message_queue=test_message_queue,
-        ):
-            pass
+        )
+    )
+    with pytest.raises(
+        ValueError, match="At least one of 'topics' and 'run_info_topic'"
+    ):
+        await anext(stream)
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_specified_topics_override_run_start_message_topics(queues):
     # If "topics" argument is specified then they should be used, even if
     # a run start topic is provided
     data_queue, worker_instruction_queue, test_message_queue = queues
     test_topics = ["whiting", "snail", "porpoise"]
     topic_in_run_start_message = "test_topic"
     test_streams = [Stream("/entry", topic_in_run_start_message)]
@@ -405,15 +412,15 @@
     ):
         pass
     assert not query_consumer.queried_topics, (
         "Expected specified topics" " to be used and none queried"
     )
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_stream_returns_metadata(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
     # the nexus_structure field of the run start message
@@ -515,15 +522,15 @@
     )
     assert np.array_equal(
         get_attrs(data_from_stream)[tdct_source_name].value.values,
         tdct_timestamps,
     )
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_stream_returns_data_from_multiple_slow_metadata_messages(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
     # the nexus_structure field of the run start message
@@ -582,15 +589,15 @@
         get_attrs(data_from_stream)[f142_source_name].value.coords['time'].values,
         np.array(
             [f142_timestamp_1, f142_timestamp_2], dtype=np.dtype('datetime64[ns]')
         ),
     )
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_stream_returns_data_from_multiple_fast_metadata_messages(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
     # the nexus_structure field of the run start message
@@ -682,15 +689,15 @@
     )
     assert np.array_equal(
         get_attrs(data_from_stream)[senv_source_name].value.coords['time'].values,
         np.concatenate((senv_expected_timestamps_1, senv_expected_timestamps_2)),
     )
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_stream_returns_data_from_multiple_chopper_messages(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
     # the nexus_structure field of the run start message
@@ -730,15 +737,15 @@
 
     assert np.array_equal(
         get_attrs(data_from_stream)[tdct_source_name].value.values,
         np.concatenate((tdct_timestamps_1, tdct_timestamps_2)),
     )
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_stream_warns_if_fast_metadata_message_exceeds_buffer(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     buffer_size = 2
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
@@ -790,15 +797,15 @@
                 senv_values,
                 Location.Start,
             )
 
             test_message_queue.put(FakeMessage(senv_test_message))
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_stream_warns_if_single_chopper_message_exceeds_buffer(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     buffer_size = 2
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
@@ -830,15 +837,15 @@
             # 3 values but buffer size is only 2!
             tdct_timestamps = np.array([1234, 2345, 3456])  # ns
             tdct_test_message = serialise_tdct(tdct_source_name, tdct_timestamps)
 
             test_message_queue.put(FakeMessage(tdct_test_message))
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_returned_if_multiple_slow_metadata_msgs_exceed_buffer(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
     # the nexus_structure field of the run start message
@@ -894,15 +901,15 @@
             )
             reached_asserts = True
         n_chunks += 1
 
     assert reached_asserts
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_returned_if_multiple_fast_metadata_msgs_exceed_buffer(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     buffer_size = 4
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
@@ -976,15 +983,15 @@
                 get_attrs(data)[senv_source_name].value.values, second_senv_values
             )
             reached_asserts = True
         n_chunks += 1
     assert reached_asserts
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_returned_if_multiple_chopper_msgs_exceed_buffer(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     buffer_size = 4
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
@@ -1031,15 +1038,15 @@
                 get_attrs(data)[tdct_source_name].value.values, tdct_timestamps_2
             )
             reached_asserts = True
         n_chunks += 1
     assert reached_asserts
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_passes_with_missing_datasets_if_group_contains_stream(queues):
     # Create NeXus description for run start message which contains
     # an NXlog which contains no datasets but does have a Stream
     # source for the data
     builder = NexusBuilder()
     test_instrument_name = "DATA_STREAM_TEST"
     builder.add_instrument(test_instrument_name)
@@ -1067,15 +1074,15 @@
             test_message_queue=test_message_queue,
         ):
             reached_assert = True
             break
         assert reached_assert
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_data_stream_times_out(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
@@ -1097,26 +1104,28 @@
             # Do nothing until it times out
             pass
     except TimeoutError:
         timed_out = True
     assert timed_out
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_stream_loop_exits_if_stop_time_and_end_of_partition_reached(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     # System time is already after this stop time so the stream will stop
     # as soon as it sees the end of partition or a message with a
     # timestamp after the stop time
-    stop_time_in_past = datetime.datetime(2017, 11, 28, 23, 55, 59, 342380)
+    stop_time_in_past = datetime.datetime(
+        2017, 11, 28, 23, 55, 59, 342380, tzinfo=datetime.timezone.utc
+    )
     n_chunks = 0
     async for _ in _data_stream(
         data_queue,
         worker_instruction_queue,
         run_info_topic=run_info_topic,
         query_consumer=FakeQueryConsumer(
             test_instrument_name, stop_time=stop_time_in_past
@@ -1131,15 +1140,15 @@
             # consumer has stopped and stop the buffer and the
             # _data_stream will exit.
             # A TimeoutError would occur if the functionality is broken.
             test_message_queue.put(FakeMessage(b"", KafkaError._PARTITION_EOF))
         n_chunks += 1
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_stream_loop_exits_if_stop_time_reached_and_later_message_seen(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
     # the nexus_structure field of the run start message
@@ -1157,15 +1166,17 @@
     ]
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     # System time is already after this stop time so the stream will stop
     # as soon as it sees the end of partition or a message with a
     # timestamp after the stop time
-    stop_time_in_past = datetime.datetime(2017, 11, 28, 23, 55, 59, 342380)
+    stop_time_in_past = datetime.datetime(
+        2017, 11, 28, 23, 55, 59, 342380, tzinfo=datetime.timezone.utc
+    )
     n_chunks = 0
     async for data in _data_stream(
         data_queue,
         worker_instruction_queue,
         run_info_topic=run_info_topic,
         query_consumer=FakeQueryConsumer(
             test_instrument_name, stop_time=stop_time_in_past, streams=streams
@@ -1173,15 +1184,17 @@
         **test_stream_args,
         test_message_queue=test_message_queue,
         end_at=StopTime.END_OF_RUN,
     ):
         if n_chunks == 0:
             # Publish a message with a timestamp before the stop time
             f142_value_1 = 26.1236
-            timestamp_before_stop_dt = datetime.datetime(2017, 11, 28, 23, 55, 50, 0)
+            timestamp_before_stop_dt = datetime.datetime(
+                2017, 11, 28, 23, 55, 50, 0, tzinfo=datetime.timezone.utc
+            )
             # Convert to integer nanoseconds
             # (for timestamp in message payload)
             timestamp_before_stop_ns = int(
                 timestamp_before_stop_dt.timestamp() * 1_000_000_000
             )
             # Convert to integer milliseconds
             # (for Kafka message header)
@@ -1203,15 +1216,17 @@
                 np.array([timestamp_before_stop_ns], dtype=np.dtype('datetime64[ns]')),
             )
 
             # Publish message with timestamp after stop time, this will trigger
             # the consumer to stop and data_stream to exit.
             # A TimeoutError would occur if the functionality is broken.
             f142_value_2 = 2.725
-            timestamp_after_stop_dt = datetime.datetime(2017, 11, 28, 23, 56, 50, 0)
+            timestamp_after_stop_dt = datetime.datetime(
+                2017, 11, 28, 23, 56, 50, 0, tzinfo=datetime.timezone.utc
+            )
             timestamp_after_stop_ns = int(
                 timestamp_after_stop_dt.timestamp() * 1_000_000_000
             )
             timestamp_after_stop_ms = int(timestamp_after_stop_dt.timestamp() * 1_000)
             f142_test_message = serialise_f142(
                 f142_value_2, f142_source_name, timestamp_after_stop_ns
             )
```

### Comparing `scippneutron-24.3.0/tests/instrument_view_test.py` & `scippneutron-24.5.0/tests/instrument_view_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,15 +120,17 @@
     d = make_dataset_with_beamline()
     # Check that all our valid shape types work
     for shape_type in ['box', 'cylinder', 'disk']:
         scn.instrument_view(
             d["a"],
             components={'sample': _make_component_settings(data=d, type=shape_type)},
         )
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError, match='Unknown shape: trefoil_knot requested for sample'
+    ):
         scn.instrument_view(
             d["a"],
             components={
                 'sample': _make_component_settings(data=d, type='trefoil_knot')
             },
         )
```

### Comparing `scippneutron-24.3.0/tests/io/cif_test.py` & `scippneutron-24.5.0/tests/io/cif_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 def test_write_block_empty():
     block = cif.Block('a-block-name')
     res = write_to_str(block)
     assert res == 'data_a-block-name\n\n'
 
 
 def test_write_block_name_with_space():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='Block name must not contain spaces'):
         cif.Block('a block-name with space')
 
 
 def test_write_block_comment():
     block = cif.Block('a-block-name', comment='some comment\n to describe the block')
     res = write_to_str(block)
     assert (
@@ -76,28 +76,28 @@
         == '''data_number
 
 _cell.angle_alpha 62
 '''
     )
 
 
-@pytest.mark.parametrize('unit', (None, 'deg'))
+@pytest.mark.parametrize('unit', [None, 'deg'])
 def test_write_block_single_pair_number_variable(unit):
     block = cif.Block('number', [{'cell.angle_alpha': sc.scalar(93, unit=unit)}])
     res = write_to_str(block)
     assert (
         res
         == '''data_number
 
 _cell.angle_alpha 93
 '''
     )
 
 
-@pytest.mark.parametrize('unit', (None, 'deg'))
+@pytest.mark.parametrize('unit', [None, 'deg'])
 def test_write_block_single_pair_number_error(unit):
     block = cif.Block(
         'number', [{'cell.angle_alpha': sc.scalar(93.2, variance=2.1**2, unit=unit)}]
     )
     res = write_to_str(block)
     assert (
         res
@@ -636,15 +636,15 @@
 loop_
 _audit_conform.dict_name
 _audit_conform.dict_version
 _audit_conform.dict_location
 coreCIF 3.3.0 https://github.com/COMCIFS/cif_core/blob/fc3d75a298fd7c0c3cde43633f2a8616e826bfd5/cif_core.dic
 
 _audit.creation_method 'written by scippneutron'
-'''  # noqa: E501
+'''
     )
 
 
 def test_write_block_core_schema_from_loop():
     author = sc.array(dims=['author'], values=['Ridcully, M.', 'Librarian'])
     email = sc.array(dims=['author'], values=['m.ridcully@uu.am', 'lib@uu.am'])
     loop = cif.Loop(
@@ -664,15 +664,15 @@
 coreCIF 3.3.0 https://github.com/COMCIFS/cif_core/blob/fc3d75a298fd7c0c3cde43633f2a8616e826bfd5/cif_core.dic
 
 loop_
 _audit_author.name
 _audit_author.email
 'Ridcully, M.' m.ridcully@uu.am
 Librarian lib@uu.am
-'''  # noqa: E501
+'''
     )
 
 
 def test_write_block_pd_schema_from_chunk():
     chunk = cif.Chunk(
         {'pd_meas.units_of_intensity': '1/(micro ampere)'}, schema=cif.PD_SCHEMA
     )
@@ -744,23 +744,23 @@
 _diffrn.ambient_environment
 water
 sulfur
 '''
     )
 
 
-@pytest.mark.parametrize('path_type', (str, Path))
+@pytest.mark.parametrize('path_type', [str, Path])
 def test_save_cif_one_block_file(tmpdir, path_type):
     path = path_type(Path(tmpdir) / "test_save_cif_one_block.cif")
     block1 = cif.Block(
         'block-1', [{'audit.creation_method': 'written by scippneutron'}]
     )
 
     cif.save_cif(path, block1)
-    with open(path, 'r') as f:
+    with open(path) as f:
         assert (
             f.read()
             == r'''#\#CIF_1.1
 data_block-1
 
 _audit.creation_method 'written by scippneutron'
 '''
@@ -858,15 +858,17 @@
             values=[13.6, 26.0, 9.7],
         ),
         coords={'tof': sc.array(dims=['tof'], values=[1.2, 1.4, 2.3], unit='us')},
         name='bad',
     )
 
     block = cif.Block('reduced', [])
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError, match='Unrecognized name for reduced powder data: bad'
+    ):
         block.add_reduced_powder_data(da)
 
 
 def test_block_with_reduced_powder_data_bad_coord_unit():
     da = sc.DataArray(
         sc.array(dims=['tof'], values=[13.6, 26.0, 9.7]),
         coords={'tof': sc.array(dims=['tof'], values=[1.2, 1.4, 2.3], unit='ns')},
```

### Comparing `scippneutron-24.3.0/tests/io/json_nexus_examples/event_data.json` & `scippneutron-24.5.0/tests/io/json_nexus_examples/event_data.json`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/tests/io/json_nexus_examples/instrument.json` & `scippneutron-24.5.0/tests/io/json_nexus_examples/instrument.json`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/tests/io/json_nexus_examples/log.json` & `scippneutron-24.5.0/tests/io/json_nexus_examples/log.json`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/tests/io/load_nexus_json_test.py` & `scippneutron-24.5.0/tests/io/load_nexus_json_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import scipp as sc
 import scipp.testing
 import scippnexus as snx
 
 from scippneutron.io.nexus.load_nexus import json_nexus_group, load_nexus_json_str
 
 sys.path.insert(0, str(Path(__file__).resolve().parent))
-from nexus_helpers import NexusBuilder, Source, Stream  # noqa: E402
+from nexus_helpers import NexusBuilder, Source, Stream
 
 
 class JsonNexusExampleLoader:
     BASE_PATH = Path(__file__).resolve().parent / "json_nexus_examples"
 
     @staticmethod
     @lru_cache
```

### Comparing `scippneutron-24.3.0/tests/io/load_nexus_test.py` & `scippneutron-24.5.0/tests/io/load_nexus_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 import pathlib
 import sys
 import warnings
+from collections.abc import Callable
 from pathlib import Path
-from typing import Callable, List, Type, Union
 
 import numpy as np
 import pytest
 import scipp as sc
 from dateutil.parser import parse as parse_date
 
 import scippneutron
 from scippneutron._utils import get_attrs, get_meta
 from scippneutron.io.nexus.load_nexus import load_nexus_json_str
 
 sys.path.insert(0, str(Path(__file__).resolve().parent))
-from nexus_helpers import (  # noqa: E402
+from nexus_helpers import (
     Chopper,
     Detector,
     EventData,
     Link,
     Log,
     Monitor,
     NexusBuilder,
@@ -30,15 +30,15 @@
     TransformationType,
     in_memory_hdf5_file_with_two_nxentry,
 )
 
 # representative sample of UTF-8 test strings from
 # https://www.w3.org/2001/06/utf-8-test/UTF-8-demo.html
 UTF8_TEST_STRINGS = (
-    "∮ E⋅da = Q,  n → ∞, ∑ f(i) = ∏ g(i), ∀x∈ℝ: ⌈x⌉ = −⌊−x⌋, α ∧ ¬β = ¬(¬α ∨ β)",
+    "∮ E⋅da = Q,  n → ∞, ∑ f(i) = ∏ g(i), ∀x∈ℝ: ⌈x⌉ = −⌊−x⌋, α ∧ ¬β = ¬(¬α ∨ β)",  # noqa: RUF001
     "2H₂ + O₂ ⇌ 2H₂O, R = 4.7 kΩ, ⌀ 200 mm",
     "Σὲ γνωρίζω ἀπὸ τὴν κόψη",
 )
 
 
 def _timestamp(date: str):
     return parse_date(date).timestamp()
@@ -55,22 +55,22 @@
         # There are 2 NXentry in the file, but root is used
         # to specify which to load data from
         assert scippneutron.load_nexus(nexus_file, root='/entry_1') is None
 
 
 def load_from_nexus(
     builder: NexusBuilder, *args, **kwargs
-) -> Union[sc.Dataset, sc.DataArray, None]:
+) -> sc.Dataset | sc.DataArray | None:
     with builder.file() as nexus_file:
         return scippneutron.load_nexus(nexus_file, *args, **kwargs)
 
 
 def load_from_json(
     builder: NexusBuilder, *args, **kwargs
-) -> Union[sc.Dataset, sc.DataArray, None]:
+) -> sc.Dataset | sc.DataArray | None:
     loaded_data, _ = load_nexus_json_str(builder.json_string, *args, **kwargs)
     return loaded_data
 
 
 @pytest.fixture(params=[load_from_nexus, load_from_json])
 def load_function(request) -> Callable:
     """
@@ -81,15 +81,15 @@
     return request.param
 
 
 @pytest.mark.skip(
     reason="The 'bigfake' file is partially broken and contains "
     "HDF5 groups without NX_class attribute."
 )
-@pytest.mark.parametrize('path_type', (str, pathlib.Path))
+@pytest.mark.parametrize('path_type', [str, pathlib.Path])
 def test_loads_from_file(path_type):
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", message='Skipped load', category=UserWarning)
         da = scippneutron.load_nexus(path_type(scippneutron.data.bigfake()))
     assert da.sizes == {'detector_id': 90000, 'tof': 1}
     assert 'tof' in da.coords
     assert 'position' in da.coords
@@ -153,15 +153,15 @@
     expected_detector_ids = np.array([1, 2, 3])
     assert np.array_equal(
         loaded_data.coords['detector_id'].values, expected_detector_ids
     )
 
 
 @pytest.mark.parametrize(
-    "unit,multiplier", (("ns", 1), ("us", 10**3), ("ms", 10**6), ("s", 10**9))
+    ("unit", "multiplier"), [("ns", 1), ("us", 10**3), ("ms", 10**6), ("s", 10**9)]
 )
 def test_loads_pulse_times_from_single_event_with_different_units(
     load_function: Callable, unit: str, multiplier: float
 ):
     offsets = np.array([12, 34, 56, 78])
     zeros = np.array([12.0, 34.0, 56.0, 78.0], dtype="float64")
     event_data = EventData(
@@ -189,21 +189,21 @@
         assert all(
             np.abs(loaded_data.values[event].coords['pulse_time'].values - _time)
             <= np.array(1).astype("timedelta64[ns]")
         )
 
 
 @pytest.mark.parametrize(
-    "time_zero_offset,time_zero,time_zero_unit,expected_time",
-    (
+    ("time_zero_offset", "time_zero", "time_zero_unit", "expected_time"),
+    [
         ("1980-01-01T00:00:00.0", 30, "s", "1980-01-01T00:00:30.0"),
         ("1990-01-01T00:00:00.0", 5000, "ms", "1990-01-01T00:00:05.0"),
         ("2000-01-01T00:00:00.0", 3 * 10**6, "us", "2000-01-01T00:00:03.0"),
         ("2010-01-01T00:00:00.0", 12, "hour", "2010-01-01T12:00:00.0"),
-    ),
+    ],
 )
 def test_loads_pulse_times_with_combinations_of_offset_and_units(
     load_function: Callable,
     time_zero_offset: str,
     time_zero: float,
     time_zero_unit: str,
     expected_time: str,
@@ -243,16 +243,25 @@
     )
 
     builder = NexusBuilder()
     builder.add_detector(
         Detector(detector_numbers=np.array([0, 1]), event_data=event_data_1)
     )
 
-    with pytest.warns(UserWarning, match="Invalid index in NXevent_data at "):
+    # It seems that pytest changed the way multiple warnings are returned.
+    # We now record all warnings, and make sure there is at least one warning with
+    # the expected message
+    with pytest.warns(UserWarning) as record:
         load_function(builder)
+    msg = "Invalid index in NXevent_data at "
+    msg_found = False
+    for warn in record:
+        if msg in warn.message.args[0]:
+            msg_found = True
+    assert msg_found
 
 
 def test_loads_pulse_times_from_multiple_event_data_groups(load_function: Callable):
     offsets = np.array([0, 0, 0, 0])
 
     zeros_1 = np.array([12 * 10**9, 34 * 10**9, 56 * 10**9, 78 * 10**9])
     zeros_2 = np.array([87 * 10**9, 65 * 10**9, 43 * 10**9, 21 * 10**9])
@@ -890,47 +899,47 @@
     loaded_data = load_function(builder)
     assert 'source_1' in loaded_data
     assert 'source_2' in loaded_data
     assert 'source_position' not in loaded_data
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 def test_component_position_from_distance_dataset_missing_unit(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     load_function: Callable,
 ):
     builder = NexusBuilder()
     distance = 4.2
     builder.add_component(
         component_class(component_name, distance=distance, distance_units=None)
     )
     loaded_data = load_function(builder)
     assert loaded_data[f'{component_name}_position'].unit is None
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", [(Sample, "sample"), (Source, "source")]
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 @pytest.mark.parametrize(
-    "transform_type,value,value_units,expected_position",
-    (
+    ("transform_type", "value", "value_units", "expected_position"),
+    [
         (TransformationType.ROTATION, 0.27, "rad", [0, 0, 0]),
         (TransformationType.TRANSLATION, 230, "cm", [0, 0, 2.3]),
-    ),
+    ],
 )
 def test_loads_component_position_from_single_transformation(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     transform_type: TransformationType,
     value: float,
     value_units: str,
-    expected_position: List[float],
+    expected_position: list[float],
     load_function: Callable,
 ):
     builder = NexusBuilder()
     transformation = Transformation(
         transform_type,
         vector=np.array([0, 0, 1]),
         value=np.array(value),
@@ -943,30 +952,30 @@
     )
     # Resulting position will always be in metres, whatever units are
     # used in the NeXus file
     assert loaded_data[f"{component_name}_position"].unit == sc.Unit("m")
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", [(Sample, "sample"), (Source, "source")]
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 @pytest.mark.parametrize(
-    "transform_type,value,value_units,expected_position",
-    (
+    ("transform_type", "value", "value_units", "expected_position"),
+    [
         (TransformationType.ROTATION, 180, "deg", [-1, -2, 3]),
         (TransformationType.TRANSLATION, 230, "cm", [1, 2, 5.3]),
-    ),
+    ],
 )
 def test_loads_component_position_from_single_transformation_with_offset(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     transform_type: TransformationType,
     value: float,
     value_units: str,
-    expected_position: List[float],
+    expected_position: list[float],
     load_function: Callable,
 ):
     builder = NexusBuilder()
     transformation = Transformation(
         transform_type,
         vector=np.array([0, 0, 1]),
         value=np.array(value),
@@ -981,30 +990,30 @@
     )
     # Resulting position will always be in metres, whatever units are
     # used in the NeXus file
     assert loaded_data[f"{component_name}_position"].unit == sc.Unit("m")
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", [(Sample, "sample"), (Source, "source")]
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 @pytest.mark.parametrize(
-    "transform_type,value,value_units,expected_position",
-    (
+    ("transform_type", "value", "value_units", "expected_position"),
+    [
         (TransformationType.ROTATION, 180, "deg", [-1, -2, 3]),
         (TransformationType.TRANSLATION, 230, "cm", [1, 2, 5.3]),
-    ),
+    ],
 )
 def test_raises_if_offset_but_not_offset_units_found(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     transform_type: TransformationType,
     value: float,
     value_units: str,
-    expected_position: List[float],
+    expected_position: list[float],
     load_function: Callable,
 ):
     builder = NexusBuilder()
     transformation = Transformation(
         transform_type,
         vector=np.array([0, 0, 1]),
         value=np.array(value),
@@ -1018,30 +1027,30 @@
             "ignore", message='Failed to load', category=UserWarning
         )
         loaded_data = load_function(builder)
     assert isinstance(loaded_data[component_name].value['depends_on'], str)
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 @pytest.mark.parametrize(
-    "transform_type,value,value_units,expected_position",
-    (
+    ("transform_type", "value", "value_units", "expected_position"),
+    [
         (TransformationType.ROTATION, 0.27, "rad", [0, 0, 0]),
         (TransformationType.TRANSLATION, 230, "cm", [0, 0, 2.3]),
-    ),
+    ],
 )
 def test_loads_component_position_from_log_transformation(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     transform_type: TransformationType,
     value: float,
     value_units: str,
-    expected_position: List[float],
+    expected_position: list[float],
     load_function: Callable,
 ):
     builder = NexusBuilder()
     # Provide "time" data, the builder will write the transformation as
     # an NXlog
     transformation = Transformation(
         transform_type,
@@ -1057,28 +1066,28 @@
     assert np.allclose(
         loaded_data[f"{component_name}_position"].values, expected_position
     )
     assert loaded_data[f"{component_name}_position"].unit == sc.Unit("m")
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 @pytest.mark.parametrize(
-    "transform_type,value,value_units,expected_position",
-    (
+    ("transform_type", "value", "value_units", "expected_position"),
+    [
         (TransformationType.ROTATION, [0.27, 0.73], "rad", [0, 0, 0]),
         (TransformationType.TRANSLATION, [230, 310], "cm", [0, 0, 2.3]),
-    ),
+    ],
 )
 def test_loads_component_position_with_multi_value_log_transformation(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     transform_type: TransformationType,
-    value: List[float],
+    value: list[float],
     value_units: str,
     expected_position: float,
     load_function: Callable,
 ):
     builder = NexusBuilder()
     # Provide "time" data, the builder will write the transformation as
     # an NXlog. This would be encountered in a file from an experiment
@@ -1101,18 +1110,18 @@
             unit="ns",
             dtype=sc.DType.datetime64,
         ),
     )
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 def test_loads_component_position_with_multiple_multi_valued_log_transformations(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     load_function: Callable,
 ):
     builder = NexusBuilder()
     # Provide "time" data, the builder will write the transformation as
     # an NXlog. This would be encountered in a file from an experiment
     # involving a scan of a motion axis.
@@ -1141,18 +1150,18 @@
     assert sc.identical(
         comp['depends_on'].coords["time"],
         sc.Variable(dims=["time"], values=[0, 1], unit="s", dtype=sc.DType.datetime64),
     )
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 def test_multi_valued_log_transformations_time_axis_interpolated_and_trimmed(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     load_function: Callable,
 ):
     builder = NexusBuilder()
     t1 = Transformation(
         TransformationType.TRANSLATION,
         vector=np.array([0, 0, 1]),
@@ -1185,22 +1194,22 @@
             unit="ms",
             dtype=sc.DType.datetime64,
         ).to(unit="ns"),
     )
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 @pytest.mark.parametrize(
-    "transform_type,value_units",
-    ((TransformationType.ROTATION, "deg"), (TransformationType.TRANSLATION, "cm")),
+    ("transform_type", "value_units"),
+    [(TransformationType.ROTATION, "deg"), (TransformationType.TRANSLATION, "cm")],
 )
 def test_skips_component_position_with_empty_value_log_transformation(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     transform_type: TransformationType,
     value_units: str,
     load_function: Callable,
 ):
     builder = NexusBuilder()
     empty_value = np.array([])
@@ -1214,18 +1223,18 @@
     )
     builder.add_component(component_class(component_name, depends_on=transformation))
     with pytest.warns(UserWarning):
         load_function(builder)
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 def test_load_component_position_prefers_transform_over_distance(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     load_function: Callable,
 ):
     # The "distance" dataset gives the position along the z axis.
     # If there is a "depends_on" pointing to transformations then we
     # prefer to use that instead as it is likely to be more accurate; it
     # can define position and orientation in 3D.
@@ -1247,39 +1256,39 @@
     assert np.allclose(
         loaded_data[f"{component_name}_position"].values, expected_position
     )
     assert loaded_data[f"{component_name}_position"].unit == sc.Unit("m")
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 @pytest.mark.parametrize(
-    "transform_type", (TransformationType.ROTATION, TransformationType.TRANSLATION)
+    "transform_type", [TransformationType.ROTATION, TransformationType.TRANSLATION]
 )
 def test_skips_component_position_from_transformation_missing_unit(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     transform_type: TransformationType,
     load_function: Callable,
 ):
     builder = NexusBuilder()
     transformation = Transformation(
         transform_type, np.array([0, 0, -1]), value=np.array(2.3)
     )
     builder.add_component(component_class(component_name, depends_on=transformation))
     with pytest.warns(UserWarning):
         load_function(builder)
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 def test_loads_component_position_from_multiple_transformations(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     load_function: Callable,
 ):
     builder = NexusBuilder()
     transformation_1 = Transformation(
         TransformationType.ROTATION,
         np.array([0, 1, 0]),
@@ -1307,18 +1316,18 @@
     builder = NexusBuilder()
     builder.add_source(Source("source"))
     loaded_data = load_function(builder)
     assert 'source_position' not in loaded_data
 
 
 @pytest.mark.parametrize(
-    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+    ("component_class", "component_name"), [(Sample, "sample"), (Source, "source")]
 )
 def test_loads_component_position_from_distance_dataset(
-    component_class: Union[Type[Source], Type[Sample]],
+    component_class: type[Source] | type[Sample],
     component_name: str,
     load_function: Callable,
 ):
     # If the NXsource or NXsample contains a "distance" dataset
     # this gives the position along the z axis. If there was a "depends_on"
     # pointing to transformations then we'd use that instead as it is
     # likely to be more accurate; it can define position and orientation in 3D.
@@ -1740,20 +1749,20 @@
     )
     assert sc.identical(
         loaded_data["end_time"], sc.DataArray(sc.scalar("2002-02-02T00:00:00"))
     )
 
 
 @pytest.mark.parametrize(
-    "log_start,scaling_factor",
-    (
+    ("log_start", "scaling_factor"),
+    [
         ("2000-01-01T01:00:00", 1000),
         ("2000-01-01T00:00:00", 0.001),
         ("2010-01-01T00:00:00", None),
-    ),
+    ],
 )
 def test_load_log_times(log_start: str, scaling_factor: float, load_function: Callable):
     times = np.array([0.0, 10.0, 20.0, 30.0, 40.0, 50.0], dtype="float64")
 
     builder = NexusBuilder()
     builder.add_log(
         Log(
@@ -1828,15 +1837,15 @@
 
     diffs = np.abs(actual.values - expected.values)
 
     # Allow 1ns difference for rounding errors between different routes
     assert all(diffs <= np.array(1).astype("timedelta64[ns]"))
 
 
-@pytest.mark.parametrize("units", ("ps", "ns", "us", "ms", "s", "minute", "hour"))
+@pytest.mark.parametrize("units", ["ps", "ns", "us", "ms", "s", "minute", "hour"])
 def test_adjust_log_times_with_different_time_units(units, load_function: Callable):
     times = [1, 2, 3]
 
     builder = NexusBuilder()
     builder.add_log(
         Log(
             name="test_log",
```

### Comparing `scippneutron-24.3.0/tests/io/nexus_helpers.py` & `scippneutron-24.5.0/tests/io/nexus_helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import json
+from collections.abc import Iterator
 from contextlib import contextmanager
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
+from typing import Any, Union
 
 import h5py
 import numpy as np
 import scipp as sc
 
 from scippneutron.io.nexus._json_nexus import (
     JSONGroup,
     _name,
     make_json_attr,
     make_json_dataset,
 )
 
-h5root = Union[h5py.File, h5py.Group]
+h5root = h5py.File | h5py.Group
 
 
 def _create_nx_class(group_name: str, nx_class_name: str, parent: h5root) -> h5py.Group:
     nx_class = parent.create_group(group_name)
     nx_class.attrs["NX_class"] = nx_class_name
     return nx_class
 
@@ -38,116 +39,116 @@
         yield nexus_file
     finally:
         nexus_file.close()
 
 
 @dataclass
 class EventData:
-    event_id: Optional[np.ndarray]
-    event_time_offset: Optional[np.ndarray]
-    event_time_zero: Optional[np.ndarray]
-    event_index: Optional[np.ndarray]
-    event_time_zero_unit: Optional[Union[str, bytes]] = "ns"
-    event_time_zero_offset: Optional[Union[str, bytes]] = "1970-01-01T00:00:00Z"
-    event_time_offset_unit: Optional[Union[str, bytes]] = "ns"
+    event_id: np.ndarray | None
+    event_time_offset: np.ndarray | None
+    event_time_zero: np.ndarray | None
+    event_index: np.ndarray | None
+    event_time_zero_unit: str | bytes | None = "ns"
+    event_time_zero_offset: str | bytes | None = "1970-01-01T00:00:00Z"
+    event_time_offset_unit: str | bytes | None = "ns"
 
 
 @dataclass
 class Log:
     name: str
-    value: Optional[np.ndarray]
-    time: Optional[np.ndarray] = None
-    value_units: Optional[Union[str, bytes]] = None
+    value: np.ndarray | None
+    time: np.ndarray | None = None
+    value_units: str | bytes | None = None
 
     # From
     # https://manual.nexusformat.org/classes/base_classes/NXlog.html?highlight=nxlog
     # time units are non-optional if time series data is present, and the unit
     # must be a unit of time (i.e. convertible to seconds).
-    time_units: Optional[Union[str, bytes]] = "s"
+    time_units: str | bytes | None = "s"
 
-    start_time: Optional[Union[str, bytes]] = "1970-01-01T00:00:00Z"
-    scaling_factor: Optional[float] = None
+    start_time: str | bytes | None = "1970-01-01T00:00:00Z"
+    scaling_factor: float | None = None
 
 
 class TransformationType(Enum):
     TRANSLATION = "translation"
     ROTATION = "rotation"
 
 
 @dataclass
 class Transformation:
     transform_type: TransformationType
     vector: np.ndarray
-    value: Optional[np.ndarray]
-    time: Optional[np.ndarray] = None
+    value: np.ndarray | None
+    time: np.ndarray | None = None
     depends_on: Union["Transformation", str, None] = None
-    offset: Optional[np.ndarray] = None
-    offset_unit: Optional[str] = None
-    value_units: Optional[Union[str, bytes]] = None
-    time_units: Optional[Union[str, bytes]] = None
+    offset: np.ndarray | None = None
+    offset_unit: str | None = None
+    value_units: str | bytes | None = None
+    time_units: str | bytes | None = None
 
 
 @dataclass
 class Detector:
-    detector_numbers: Optional[np.ndarray] = None
-    event_data: Optional[EventData] = None
-    log: Optional[Log] = None
-    x_offsets: Optional[np.ndarray] = None
-    y_offsets: Optional[np.ndarray] = None
-    z_offsets: Optional[np.ndarray] = None
-    offsets_unit: Optional[Union[str, bytes]] = None
-    depends_on: Optional[Transformation] = None
-    data: Optional[np.ndarray] = None
+    detector_numbers: np.ndarray | None = None
+    event_data: EventData | None = None
+    log: Log | None = None
+    x_offsets: np.ndarray | None = None
+    y_offsets: np.ndarray | None = None
+    z_offsets: np.ndarray | None = None
+    offsets_unit: str | bytes | None = None
+    depends_on: Transformation | None = None
+    data: np.ndarray | None = None
 
 
 @dataclass
 class Data:
     name: str
     data: sc.DataArray
     attrs: dict = None
 
 
 @dataclass
 class Sample:
     name: str
-    depends_on: Optional[Transformation] = None
-    distance: Optional[float] = None
-    distance_units: Optional[Union[str, bytes]] = None
-    ub_matrix: Optional[np.ndarray] = None
-    orientation_matrix: Optional[np.ndarray] = None
+    depends_on: Transformation | None = None
+    distance: float | None = None
+    distance_units: str | bytes | None = None
+    ub_matrix: np.ndarray | None = None
+    orientation_matrix: np.ndarray | None = None
 
 
 @dataclass
 class Source:
     name: str
-    depends_on: Union[Transformation, None, str] = None
-    distance: Optional[float] = None
-    distance_units: Optional[Union[str, bytes]] = None
+    depends_on: Transformation | None | str = None
+    distance: float | None = None
+    distance_units: str | bytes | None = None
 
 
 @dataclass
 class Chopper:
     name: str
     distance: float
     rotation_speed: float
-    distance_units: Optional[str] = None
-    rotation_units: Optional[str] = None
+    distance_units: str | None = None
+    rotation_units: str | None = None
 
 
 @dataclass
 class Link:
     new_path: str
     target_path: str
 
 
 @dataclass
 class DatasetAtPath:
     path: str
     data: np.ndarray
-    attributes: Dict[str, Any]
+    attributes: dict[str, Any]
 
 
 @dataclass
 class Stream:
     """
     Only present in the JSON NeXus file templates, not in HDF5 NeXus files.
     Records where to find data in Kafka that are streamed during an experiment.
@@ -180,41 +181,41 @@
     value_units: str = "m"
 
 
 @dataclass
 class Monitor:
     name: str
     data: np.ndarray
-    axes: List[Tuple[str, np.ndarray]]
-    events: Optional[EventData] = None
-    depends_on: Optional[Transformation] = None
+    axes: list[tuple[str, np.ndarray]]
+    events: EventData | None = None
+    depends_on: Transformation | None = None
 
 
 class InMemoryNeXusWriter:
     def add_dataset_at_path(
-        self, file_root: h5py.File, path: str, data: np.ndarray, attributes: Dict
+        self, file_root: h5py.File, path: str, data: np.ndarray, attributes: dict
     ):
         path_split = path.split("/")
         dataset_name = path_split[-1]
         parent_path = "/".join(path_split[:-1])
         dataset = self.add_dataset(file_root[parent_path], dataset_name, data)
         for name, value in attributes.items():
             self.add_attribute(dataset, name, value)
 
     @staticmethod
     def add_dataset(
-        parent: h5py.Group, name: str, data: Union[str, bytes, np.ndarray]
+        parent: h5py.Group, name: str, data: str | bytes | np.ndarray
     ) -> h5py.Dataset:
         return parent.create_dataset(name, data=data)
 
     @staticmethod
     def add_attribute(
-        parent: Union[h5py.Group, h5py.Dataset],
+        parent: h5py.Group | h5py.Dataset,
         name: str,
-        value: Union[str, bytes, np.ndarray],
+        value: str | bytes | np.ndarray,
     ):
         parent.attrs[name] = value
 
     @staticmethod
     def add_group(parent: h5py.Group, name: str) -> h5py.Group:
         return parent.create_group(name)
 
@@ -251,73 +252,69 @@
     path = path.split('/')[1:]  # Trim leading slash
     obj = file_root
     for name in path:
         obj = _get_child(obj, name)
     return obj
 
 
-def _add_link_to_json(file_root: Dict, new_path: str, target_path: str):
+def _add_link_to_json(file_root: dict, new_path: str, target_path: str):
     new_path_split = new_path.split("/")
     link_name = new_path_split[-1]
     parent_path = "/".join(new_path_split[:-1])
     parent_group = _get_object_by_path(file_root, parent_path)
     link = {"module": "link", "config": {"name": link_name, "target": target_path}}
     existing_object = _get_object_by_path(parent_group, link_name)
     if existing_object is not None:
         parent_group["children"].remove(existing_object)
     parent_group["children"].append(link)
 
 
-def _parent_and_name_from_path(file_root: Dict, path: str) -> Tuple[Dict, str]:
+def _parent_and_name_from_path(file_root: dict, path: str) -> tuple[dict, str]:
     path_split = path.split("/")
     name = path_split[-1]
     parent_path = '/'.join(path_split[:-1])
     parent_group = _get_object_by_path(file_root, parent_path)
     return parent_group, name
 
 
 class JsonWriter:
     def add_dataset_at_path(
-        self, file_root: Dict, path: str, data: np.ndarray, attributes: Dict
+        self, file_root: dict, path: str, data: np.ndarray, attributes: dict
     ):
         parent_group, dataset_name = _parent_and_name_from_path(file_root, path)
         dataset = self.add_dataset(parent_group, dataset_name, data)
         for name, value in attributes.items():
             self.add_attribute(dataset, name, value)
 
     @staticmethod
-    def add_dataset(
-        parent: Dict, name: str, data: Union[str, bytes, np.ndarray]
-    ) -> Dict:
+    def add_dataset(parent: dict, name: str, data: str | bytes | np.ndarray) -> dict:
         dataset = make_json_dataset(name, data)
         parent["children"].append(dataset)
         return dataset
 
     @staticmethod
-    def add_attribute(
-        parent: Dict, name: str, value: Union[str, bytes, list, np.ndarray]
-    ):
+    def add_attribute(parent: dict, name: str, value: str | bytes | list | np.ndarray):
         attr = make_json_attr(name, value)
         parent["attributes"].append(attr)
 
     @staticmethod
-    def add_group(parent: Dict, name: str) -> Dict:
+    def add_group(parent: dict, name: str) -> dict:
         new_group = {"type": "group", "name": name, "children": [], "attributes": []}
         parent["children"].append(new_group)
         return new_group
 
     @staticmethod
-    def add_hard_link(file_root: Dict, new_path: str, target_path: str):
+    def add_hard_link(file_root: dict, new_path: str, target_path: str):
         _add_link_to_json(file_root, new_path, target_path)
 
     @staticmethod
-    def add_soft_link(file_root: Dict, new_path: str, target_path: str):
+    def add_soft_link(file_root: dict, new_path: str, target_path: str):
         _add_link_to_json(file_root, new_path, target_path)
 
-    def add_stream(self, file_root: Dict, stream: Stream):
+    def add_stream(self, file_root: dict, stream: Stream):
         new_stream = {
             "module": stream.writer_module,
             "config": {
                 "topic": stream.topic,
                 "source": stream.source,
                 "type": stream.type,
                 "value_units": stream.value_units,
@@ -338,36 +335,36 @@
 
 class NexusBuilder:
     """
     Allows building an in-memory NeXus file for use in tests
     """
 
     def __init__(self):
-        self._event_data: List[EventData] = []
-        self._detectors: List[Detector] = []
-        self._logs: List[Log] = []
-        self._instrument_name: Optional[str] = None
-        self._choppers: List[Chopper] = []
-        self._title: Optional[str] = None
-        self._start_time: Optional[str] = None
-        self._end_time: Optional[str] = None
-        self._sample: List[Sample] = []
-        self._source: List[Source] = []
-        self._hard_links: List[Link] = []
-        self._soft_links: List[Link] = []
+        self._event_data: list[EventData] = []
+        self._detectors: list[Detector] = []
+        self._logs: list[Log] = []
+        self._instrument_name: str | None = None
+        self._choppers: list[Chopper] = []
+        self._title: str | None = None
+        self._start_time: str | None = None
+        self._end_time: str | None = None
+        self._sample: list[Sample] = []
+        self._source: list[Source] = []
+        self._hard_links: list[Link] = []
+        self._soft_links: list[Link] = []
         self._writer = None
-        self._datasets: List[DatasetAtPath] = []
+        self._datasets: list[DatasetAtPath] = []
         self._streams = []
         self._monitors = []
         self._datas = []
 
-    def add_dataset_at_path(self, path: str, data: np.ndarray, attributes: Dict):
+    def add_dataset_at_path(self, path: str, data: np.ndarray, attributes: dict):
         self._datasets.append(DatasetAtPath(path, data, attributes))
 
-    def _write_datasets(self, root: Union[Dict, h5py.File]):
+    def _write_datasets(self, root: dict | h5py.File):
         for dataset in self._datasets:
             self._writer.add_dataset_at_path(
                 root, dataset.path, dataset.data, dataset.attributes
             )
 
     def add_stream(self, stream: Stream):
         self._streams.append(stream)
@@ -415,15 +412,15 @@
     def add_soft_link(self, link: Link):
         """
         If there is a group or dataset at the link path it will
         be replaced by the link
         """
         self._soft_links.append(link)
 
-    def add_component(self, component: Union[Sample, Source]):
+    def add_component(self, component: Sample | Source):
         # This is a little ugly, but allows parametrisation
         # of tests which should work for sample and source
         if isinstance(component, Sample):
             self.add_sample(component)
         elif isinstance(component, Source):
             self.add_source(component)
 
@@ -466,15 +463,15 @@
         self._writer = InMemoryNeXusWriter()
         try:
             self._write_file(nexus_file)
             yield nexus_file
         finally:
             nexus_file.close()
 
-    def _write_file(self, nexus_file: Union[h5py.File, Dict]):
+    def _write_file(self, nexus_file: h5py.File | dict):
         entry_group = self._create_nx_class("entry", "NXentry", nexus_file)
         if self._title is not None:
             self._writer.add_dataset(entry_group, "title", data=self._title)
         if self._start_time is not None:
             self._writer.add_dataset(entry_group, "start_time", data=self._start_time)
         if self._end_time is not None:
             self._writer.add_dataset(entry_group, "end_time", data=self._end_time)
@@ -505,25 +502,25 @@
         nexus_file = h5py.File(filename, mode='w')
         self._writer = InMemoryNeXusWriter()
         try:
             self._write_file(nexus_file)
         finally:
             nexus_file.close()
 
-    def _write_links(self, file_root: Union[h5py.Group, Dict]):
+    def _write_links(self, file_root: h5py.Group | dict):
         for hard_link in self._hard_links:
             self._writer.add_hard_link(
                 file_root, hard_link.new_path, hard_link.target_path
             )
         for soft_link in self._soft_links:
             self._writer.add_soft_link(
                 file_root, soft_link.new_path, soft_link.target_path
             )
 
-    def _write_sample(self, parent_group: Union[h5py.Group, Dict]):
+    def _write_sample(self, parent_group: h5py.Group | dict):
         for sample in self._sample:
             sample_group = self._create_nx_class(sample.name, "NXsample", parent_group)
             if sample.depends_on is not None:
                 depends_on = self._add_transformations_to_file(
                     sample.depends_on, sample_group, f"/entry/{sample.name}"
                 )
                 self._writer.add_dataset(sample_group, "depends_on", data=depends_on)
@@ -542,15 +539,15 @@
                 )
 
             if sample.orientation_matrix is not None:
                 self._writer.add_dataset(
                     sample_group, "orientation_matrix", data=sample.orientation_matrix
                 )
 
-    def _write_source(self, parent_group: Union[h5py.Group, Dict]):
+    def _write_source(self, parent_group: h5py.Group | dict):
         for source in self._source:
             source_group = self._create_nx_class(source.name, "NXsource", parent_group)
             if source.depends_on is not None:
                 if isinstance(source.depends_on, str):
                     depends_on = source.depends_on
                 else:
                     depends_on = self._add_transformations_to_file(
@@ -562,24 +559,22 @@
                     source_group, "distance", data=source.distance
                 )
                 if source.distance_units is not None:
                     self._writer.add_attribute(
                         distance_ds, "units", source.distance_units
                     )
 
-    def _write_instrument(
-        self, parent_group: Union[h5py.Group, Dict]
-    ) -> Union[h5py.Group, Dict]:
+    def _write_instrument(self, parent_group: h5py.Group | dict) -> h5py.Group | dict:
         instrument_group = self._create_nx_class(
             "instrument", "NXinstrument", parent_group
         )
         self._writer.add_dataset(instrument_group, "name", self._instrument_name)
         return instrument_group
 
-    def _write_detectors(self, parent_group: Union[h5py.Group, Dict], parent_path: str):
+    def _write_detectors(self, parent_group: h5py.Group | dict, parent_path: str):
         for detector_index, detector in enumerate(self._detectors):
             detector_name = f"detector_{detector_index}"
             detector_group = self._add_detector_group_to_file(
                 detector, parent_group, detector_name
             )
             if detector.data is not None:
                 da = detector.data
@@ -603,15 +598,15 @@
                 depends_on = self._add_transformations_to_file(
                     detector.depends_on,
                     detector_group,
                     f"{parent_path}/{detector_name}",
                 )
                 self._writer.add_dataset(detector_group, "depends_on", data=depends_on)
 
-    def _write_choppers(self, parent_group: Union[h5py.Group, Dict]):
+    def _write_choppers(self, parent_group: h5py.Group | dict):
         for chopper in self._choppers:
             chopper_group = self._create_nx_class(
                 chopper.name, "NXdisk_chopper", parent_group
             )
             distance_ds = self._writer.add_dataset(
                 chopper_group, "distance", data=chopper.distance
             )
@@ -619,21 +614,21 @@
                 chopper_group, "rotation_speed", data=chopper.rotation_speed
             )
             if chopper.distance_units is not None:
                 self._writer.add_attribute(distance_ds, "units", chopper.distance_units)
             if chopper.rotation_units is not None:
                 self._writer.add_attribute(rotation_ds, "units", chopper.rotation_units)
 
-    def _write_event_data(self, parent_group: Union[h5py.Group, Dict]):
+    def _write_event_data(self, parent_group: h5py.Group | dict):
         for event_data_index, event_data in enumerate(self._event_data):
             self._add_event_data_group_to_file(
                 event_data, parent_group, f"events_{event_data_index}"
             )
 
-    def _write_monitors(self, parent_group: Union[h5py.Group, Dict]):
+    def _write_monitors(self, parent_group: h5py.Group | dict):
         for monitor in self._monitors:
             self._add_monitor_group_to_file(monitor, parent_group)
 
     def _add_monitor_group_to_file(self, monitor: Monitor, parent_group: h5py.Group):
         monitor_group = self._create_nx_class(monitor.name, "NXmonitor", parent_group)
         data_group = self._writer.add_dataset(monitor_group, "data", monitor.data)
         self._writer.add_attribute(data_group, "units", '')
@@ -656,15 +651,15 @@
                 depends_on = monitor.depends_on
             else:
                 depends_on = self._add_transformations_to_file(
                     monitor.depends_on, monitor_group, f"/{monitor.name}"
                 )
             self._writer.add_dataset(monitor_group, "depends_on", data=depends_on)
 
-    def _write_datas(self, parent_group: Union[h5py.Group, Dict]):
+    def _write_datas(self, parent_group: h5py.Group | dict):
         for data in self._datas:
             self._add_data_group_to_file(data, parent_group)
 
     def _add_data_group_to_file(self, data: Data, parent_group: h5py.Group):
         da = data.data
         group = self._create_nx_class(data.name, "NXdata", parent_group)
         self._writer.add_attribute(group, "axes", da.dims)
@@ -678,15 +673,15 @@
         for name, coord in da.coords.items():
             ds = self._writer.add_dataset(group, name, coord.values)
             self._writer.add_attribute(ds, "units", str(coord.unit))
         if data.attrs is not None:
             for k, v in data.attrs.items():
                 self._writer.add_attribute(group, k, v)
 
-    def _write_logs(self, parent_group: Union[h5py.Group, Dict]):
+    def _write_logs(self, parent_group: h5py.Group | dict):
         for log in self._logs:
             self._add_log_group_to_file(log, parent_group)
 
     def _add_event_data_group_to_file(
         self, data: EventData, parent_group: h5py.Group, group_name: str
     ):
         event_group = self._create_nx_class(group_name, "NXevent_data", parent_group)
@@ -755,15 +750,15 @@
 
     def _add_transformation_as_dataset(
         self,
         transform: Transformation,
         transform_number: int,
         transforms_group: h5py.Group,
         group_path: str,
-        depends_on: Optional[str],
+        depends_on: str | None,
     ) -> str:
         transform_name = f"transform_{transform_number}"
         added_transform = self._writer.add_dataset(
             transforms_group, f"transform_{transform_number}", data=transform.value
         )
         self._add_transform_attributes(added_transform, depends_on, transform)
         if transform.value_units is not None:
@@ -790,15 +785,15 @@
 
     def _add_transformation_as_log(
         self,
         transform: Transformation,
         transform_number: int,
         transforms_group: h5py.Group,
         group_path: str,
-        depends_on: Optional[str],
+        depends_on: str | None,
     ) -> str:
         transform_name = f"transform_{transform_number}"
         added_transform = self._add_log_group_to_file(
             Log(
                 transform_name,
                 transform.value,
                 transform.time,
@@ -831,16 +826,16 @@
                     self._writer.add_attribute(
                         offsets_ds, "units", detector.offsets_unit
                     )
         return detector_group
 
     def _add_transform_attributes(
         self,
-        added_transform: Union[h5py.Group, h5py.Dataset],
-        depends_on: Optional[str],
+        added_transform: h5py.Group | h5py.Dataset,
+        depends_on: str | None,
         transform: Transformation,
     ):
         self._writer.add_attribute(added_transform, "vector", transform.vector)
         self._writer.add_attribute(
             added_transform, "transformation_type", transform.transform_type.value
         )
         if transform.offset is not None:
@@ -859,11 +854,11 @@
     def _create_nx_class(
         self, group_name: str, nx_class_name: str, parent: h5root
     ) -> h5py.Group:
         nx_class = self._writer.add_group(parent, group_name)
         self._writer.add_attribute(nx_class, "NX_class", nx_class_name)
         return nx_class
 
-    def _write_streams(self, root: Union[h5py.File, Dict]):
+    def _write_streams(self, root: h5py.File | dict):
         if isinstance(self._writer, JsonWriter):
             for stream in self._streams:
                 self._writer.add_stream(root, stream)
```

### Comparing `scippneutron-24.3.0/tests/io/xye_test.py` & `scippneutron-24.5.0/tests/io/xye_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import string
 from io import StringIO
-from typing import Optional
 
 import numpy as np
 import pytest
 import scipp as sc
 from hypothesis import assume, given, settings
 from hypothesis import strategies as st
 from scipp.testing import strategies as scst
@@ -37,22 +36,22 @@
 
 def headers() -> st.SearchStrategy[str]:
     # Using only ASCII characters and excluding \r because Numpy and/or splitlines
     # do something funny with some other characters.
     return st.text(string.ascii_letters + string.digits + string.punctuation + ' \t\n')
 
 
-def save_to_buffer(da: sc.DataArray, coord: Optional[str] = None, **kwargs) -> StringIO:
+def save_to_buffer(da: sc.DataArray, coord: str | None = None, **kwargs) -> StringIO:
     buffer = StringIO()
     scn.io.save_xye(buffer, da, coord=coord, **kwargs)
     buffer.seek(0)
     return buffer
 
 
-def roundtrip(da: sc.DataArray, coord: Optional[str] = None, **kwargs) -> sc.DataArray:
+def roundtrip(da: sc.DataArray, coord: str | None = None, **kwargs) -> sc.DataArray:
     buffer = save_to_buffer(da, coord, **kwargs)
     return scn.io.xye.load_xye(
         buffer,
         dim=da.dim,
         coord=coord,
         unit=da.unit,
         coord_unit=da.coords[coord].unit if coord is not None else None,
@@ -73,15 +72,17 @@
 
 
 @given(da=one_dim_data_arrays(), data=st.data())
 def test_saved_file_contains_data_table(da, data):
     coord_name = data.draw(st.sampled_from(list(da.coords.keys())))
     file_contents = save_to_buffer(da, coord=coord_name).getvalue()
     for i, line in enumerate(
-        filter(lambda l: l and not l.startswith('#'), file_contents.split('\n'))
+        filter(
+            lambda line: line and not line.startswith('#'), file_contents.split('\n')
+        )
     ):
         x, y, e = map(float, line.split(' '))
         np.testing.assert_allclose(x, da.coords[coord_name][i].value)
         np.testing.assert_allclose(y, da[i].value)
         np.testing.assert_allclose(e, np.sqrt(da[i].variance))
 
 
@@ -115,24 +116,30 @@
 
 
 @given(da=one_dim_data_arrays(min_n_coords=2))
 @settings(max_examples=20)
 def test_save_cannot_deduce_coord_if_multiple_non_dim_coords(da):
     # It can deduce if there is a dim-coord, exclude that.
     assume(da.dim not in da.coords)
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError,
+        match='Cannot deduce which coordinate to save because the data '
+        'has more than one and no dimension-coordinate',
+    ):
         save_to_buffer(da)
 
 
 @given(da=one_dim_data_arrays(max_n_coords=1))
 @settings(max_examples=20)
 def test_input_must_have_at_least_one_coord(da):
     for c in list(da.coords.keys()):
         del da.coords[c]
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError, match='Cannot save data to XYE file because it has no coordinates'
+    ):
         save_to_buffer(da)
 
 
 @given(da=one_dim_data_arrays(), data=st.data())
 @settings(max_examples=20)
 def test_input_must_have_variances(da, data):
     da.variances = None
@@ -154,15 +161,17 @@
 
 
 @given(da=one_dim_data_arrays(), data=st.data())
 @settings(max_examples=20)
 def test_cannot_save_data_with_masks(da, data):
     mask = data.draw(scst.variables(sizes=da.sizes, dtype=bool))
     da.masks[data.draw(st.text())] = mask
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError, match='Cannot save data to XYE file because it has masks'
+    ):
         save_to_buffer(da, coord=next(iter(da.coords)))
 
 
 @pytest.mark.skipif(
     lambda: sc.__version__ >= (24, 1),
     reason='This use of the dataarrays strategy needs Scipp >= 24.*',
 )
```

### Comparing `scippneutron-24.3.0/tests/mantid_scipp_comparison/beamline_calculations_test.py` & `scippneutron-24.5.0/tests/mantid_scipp_comparison/beamline_calculations_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,28 +12,28 @@
     import mantid.simpleapi as sapi
 except ImportError:
     pytestmark = pytest.mark.skip('Mantid framework is unavailable')
     sapi = None
     kernel = None
 
 
-@pytest.fixture
+@pytest.fixture()
 def in_ws():
     ws = sapi.CreateSampleWorkspace(
         SourceDistanceFromSample=10.0,
         BankDistanceFromSample=1.1,
         BankPixelWidth=2,
         NumBanks=1,
         XMax=200,
         StoreInADS=False,
     )
     return ws
 
 
-@pytest.fixture
+@pytest.fixture()
 def in_da(in_ws):
     return scn.mantid.from_mantid(in_ws)
 
 
 def test_beamline_compute_l1(in_ws, in_da):
     out_mantid = in_ws.detectorInfo().l1() * sc.Unit('m')
     in_da = scn.mantid.from_mantid(in_ws)['data']
```

### Comparing `scippneutron-24.3.0/tests/mantid_scipp_comparison/histogram_events_test.py` & `scippneutron-24.5.0/tests/mantid_scipp_comparison/histogram_events_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,21 @@
     import mantid.simpleapi as sapi
 except ImportError:
     pytestmark = pytest.mark.skip('Mantid framework is unavailable')
     sapi = None
     kernel = None
 
 
-@pytest.fixture
+@pytest.fixture()
 def in_ws():
     ws = sapi.Load(Filename=scn.data.get_path("CNCS_51936_event.nxs"), StoreInADS=False)
     return ws
 
 
-@pytest.fixture
+@pytest.fixture()
 def in_da(in_ws):
     return scn.mantid.from_mantid(in_ws)['data'].astype('float64')
 
 
 def test_histogram_events(in_ws, in_da):
     from scipp.utils.comparison import isnear
```

### Comparing `scippneutron-24.3.0/tests/mantid_scipp_comparison/neutron_convert_units_test.py` & `scippneutron-24.5.0/tests/mantid_scipp_comparison/neutron_convert_units_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Jan-Lukas Wynen
 
-from typing import Optional
-
 import pytest
 import scipp as sc
 
 import scippneutron as scn
 
 try:
     import mantid.kernel as kernel
@@ -25,15 +23,15 @@
         'dspacing': 'dSpacing',
         'energy': 'Energy',
         'energy_transfer': 'DeltaE',
     }[scipp_coord]
 
 
 def make_workspace(
-    coord: str, emode: str = 'Elastic', efixed: Optional[sc.Variable] = None
+    coord: str, emode: str = 'Elastic', efixed: sc.Variable | None = None
 ) -> 'sapi.Workspace':
     ws = sapi.CreateSampleWorkspace(XMin=1000, NumBanks=1, StoreInADS=False)
     # Crop out spectra index 0 as has two_theta=0, gives inf d-spacing
     ws = sapi.CropWorkspace(ws, StartWorkspaceIndex=1, StoreInADS=False)
     ws = sapi.ConvertUnits(
         InputWorkspace=ws,
         Target=mantid_coord(coord),
@@ -54,15 +52,15 @@
     return ws
 
 
 def mantid_convert_units(
     ws: 'sapi.Workspace',
     target: str,
     emode: str = 'Elastic',
-    efixed: Optional[sc.Variable] = None,
+    efixed: sc.Variable | None = None,
 ) -> sc.DataArray:
     out_ws = sapi.ConvertUnits(
         InputWorkspace=ws,
         Target=mantid_coord(target),
         EMode=emode,
         EFixed=efixed.value if efixed is not None else None,
         StoreInADS=False,
```

### Comparing `scippneutron-24.3.0/tests/mantid_test.py` & `scippneutron-24.5.0/tests/mantid_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def setUpClass(cls):
         # This is from the Mantid system-test data
         filename = "CNCS_51936_event.nxs"
         # This needs OutputWorkspace specified, as it doesn't
         # pick up the name from the class variable name
         cls.base_event_ws = mantid.LoadEventNexus(
             scn.data.get_path(filename),
-            OutputWorkspace="test_ws{}".format(__file__),
+            OutputWorkspace=f"test_ws{__file__}",
             SpectrumMax=200,
             StoreInADS=False,
         )
 
     def test_Workspace2D_data_array(self):
         eventWS = self.base_event_ws
         ws = mantid.Rebin(eventWS, 10000, PreserveEvents=False)
@@ -81,15 +81,15 @@
         d = scn.mantid.convert_EventWorkspace_to_data_array(
             eventWS, load_pulse_times=False
         )
         histogrammed = d.hist(tof=target_tof)
 
         delta = sc.sum(binned_mantid - histogrammed, 'spectrum')
         delta = sc.sum(delta, 'tof')
-        self.assertLess(np.abs(delta.value), 1e-5)
+        assert np.abs(delta.value) < 1e-05
 
     def test_EventWorkspace(self):
         eventWS = self.base_event_ws
         ws = mantid.Rebin(eventWS, 10000)
 
         binned_mantid = scn.mantid.convert_Workspace2D_to_data_group(ws)["data"]
 
@@ -478,15 +478,15 @@
         from mantid.simpleapi import mtd
 
         mtd.clear()
         da = scn.load(
             scn.data.get_path("CNCS_51936_event.nxs"),
             mantid_args={"LoadMonitors": True, "SpectrumMax": 1},
         )
-        self.assertEqual(len(mtd), 0, mtd.getObjectNames())
+        assert len(mtd) == 0, mtd.getObjectNames()
         attrs = [str(key) for key in get_attrs(da).keys()]
         expected_monitor_attrs = {"monitor2", "monitor3"}
         assert expected_monitor_attrs.issubset(attrs)
         for monitor_name in expected_monitor_attrs:
             monitor = get_attrs(da)[monitor_name].value
             assert isinstance(monitor, sc.DataArray)
             assert monitor.shape == (200001,)
@@ -564,41 +564,41 @@
             AlignedDim1='Q_x,-10,10,4',
             AlignedDim2='Q_z,-10,10,5',
             StoreInADS=False,
         )
 
         histo_data_array = scn.mantid.convert_MDHistoWorkspace_to_data_array(md_histo)
 
-        self.assertEqual(histo_data_array.coords['Q_x'].shape, (4,))
-        self.assertEqual(histo_data_array.coords['Q_y'].shape, (3,))
-        self.assertEqual(histo_data_array.coords['Q_z'].shape, (5,))
-        self.assertEqual(
-            histo_data_array.coords['Q_x'].unit,
-            sc.units.dimensionless / sc.units.angstrom,
-        )
-        self.assertEqual(
-            histo_data_array.coords['Q_y'].unit,
-            sc.units.dimensionless / sc.units.angstrom,
-        )
-        self.assertEqual(
-            histo_data_array.coords['Q_z'].unit,
-            sc.units.dimensionless / sc.units.angstrom,
+        assert histo_data_array.coords['Q_x'].shape == (4,)
+        assert histo_data_array.coords['Q_y'].shape == (3,)
+        assert histo_data_array.coords['Q_z'].shape == (5,)
+        assert (
+            histo_data_array.coords['Q_x'].unit
+            == sc.units.dimensionless / sc.units.angstrom
+        )
+        assert (
+            histo_data_array.coords['Q_y'].unit
+            == sc.units.dimensionless / sc.units.angstrom
+        )
+        assert (
+            histo_data_array.coords['Q_z'].unit
+            == sc.units.dimensionless / sc.units.angstrom
         )
 
-        self.assertEqual(histo_data_array.shape, (3, 4, 5))
+        assert histo_data_array.shape == (3, 4, 5)
 
         # Sum over 2 dimensions to simplify finding max.
         max_1d = sc.sum(sc.sum(histo_data_array, dim='Q_y'), dim='Q_x').values
         max_index = np.argmax(max_1d)
         # Check position of max 'peak'
-        self.assertEqual(np.floor(len(max_1d) / 2), max_index)
+        assert np.floor(len(max_1d) / 2) == max_index
         # All events in central 'peak'
-        self.assertEqual(100000, max_1d[max_index])
+        assert 100000 == max_1d[max_index]
 
-        self.assertTrue('nevents' in get_attrs(histo_data_array))
+        assert 'nevents' in get_attrs(histo_data_array)
 
     def test_mdhisto_workspace_many_dims(self):
         from mantid.simpleapi import BinMD, CreateMDWorkspace, FakeMDEventData
 
         md_event = CreateMDWorkspace(
             Dimensions=4,
             Extents=[-10, 10, -10, 10, -10, 10, -10, 10],
@@ -644,15 +644,15 @@
             AlignedDim1='y,-10,10,4',
             AlignedDim2='z,-10,10,5',
             AlignedDim3='T,-10,10,7',
             StoreInADS=False,
         )
 
         histo_data_array = scn.mantid.convert_MDHistoWorkspace_to_data_array(md_histo)
-        self.assertEqual(4, len(histo_data_array.dims))
+        assert 4 == len(histo_data_array.dims)
 
     def test_to_workspace_2d_no_error(self):
         from mantid.simpleapi import mtd
 
         mtd.clear()
 
         # All Dims for which support is expected are
@@ -719,59 +719,52 @@
         assert 'cost_function' in params.coords
         assert 'chi^2/d.o.f.' in params.coords
 
     def test_convert_array_run_log_to_attrs(self):
         # Given a Mantid workspace with a run log
         target = mantid.CloneWorkspace(self.base_event_ws)
         log_name = "SampleTemp"
-        self.assertTrue(
-            target.run().hasProperty(log_name),
-            f"Expected input workspace to have a {log_name} run log",
-        )
+        assert target.run().hasProperty(
+            log_name
+        ), f'Expected input workspace to have a {log_name} run log'
 
         # When the workspace is converted to a scipp data array
         d = scn.mantid.convert_EventWorkspace_to_data_array(target, False)
 
         # Then the data array contains the run log as an unaligned coord
-        self.assertTrue(
-            np.allclose(
-                target.run()[log_name].value,
-                get_attrs(d)[log_name].values.data.values,
-            ),
-            "Expected values in the unaligned coord to match "
-            "the original run log from the Mantid workspace",
-        )
-        self.assertEqual(get_attrs(d)[log_name].values.unit, sc.units.K)
-        self.assertTrue(
-            np.array_equal(
-                target.run()[log_name].times.astype('datetime64[ns]'),
-                get_attrs(d)[log_name].values.coords["time"].values,
-            ),
-            "Expected times in the unaligned coord to match "
-            "the original run log from the Mantid workspace",
+        assert np.allclose(
+            target.run()[log_name].value, get_attrs(d)[log_name].values.data.values
+        ), (
+            'Expected values in the unaligned coord to match '
+            'the original run log from the Mantid workspace'
+        )
+        assert get_attrs(d)[log_name].values.unit == sc.units.K
+        assert np.array_equal(
+            target.run()[log_name].times.astype('datetime64[ns]'),
+            get_attrs(d)[log_name].values.coords['time'].values,
+        ), (
+            'Expected times in the unaligned coord to match '
+            'the original run log from the Mantid workspace'
         )
 
     def test_convert_scalar_run_log_to_attrs(self):
         # Given a Mantid workspace with a run log
         target = mantid.CloneWorkspace(self.base_event_ws)
         log_name = "start_time"
-        self.assertTrue(
-            target.run().hasProperty(log_name),
-            f"Expected input workspace to have a {log_name} run log",
-        )
+        assert target.run().hasProperty(
+            log_name
+        ), f'Expected input workspace to have a {log_name} run log'
 
         # When the workspace is converted to a scipp data array
         d = scn.mantid.convert_EventWorkspace_to_data_array(target, False)
 
         # Then the data array contains the run log as an unaligned coord
-        self.assertEqual(
-            target.run()[log_name].value,
-            get_attrs(d)[log_name].value,
-            "Expected value of the unaligned coord to match "
-            "the original run log from the Mantid workspace",
+        assert target.run()[log_name].value == get_attrs(d)[log_name].value, (
+            'Expected value of the unaligned coord to match '
+            'the original run log from the Mantid workspace'
         )
 
     def test_warning_raised_when_convert_run_log_with_unrecognised_units(self):
         target = mantid.CloneWorkspace(self.base_event_ws)
         target.getRun()['LambdaRequest'].units = 'abcde'
         with warnings.catch_warnings(record=True) as caught_warnings:
             warnings.simplefilter("always")
@@ -808,18 +801,18 @@
             )
 
     def test_set_sample(self):
         target = mantid.CloneWorkspace(self.base_event_ws)
         d = scn.mantid.convert_EventWorkspace_to_data_array(target, False)
         get_attrs(d)["sample"].value.setThickness(3)
         # before
-        self.assertNotEqual(3, target.sample().getThickness())
+        assert 3 != target.sample().getThickness()
         target.setSample(get_attrs(d)["sample"].value)
         # after
-        self.assertEqual(3, target.sample().getThickness())
+        assert 3 == target.sample().getThickness()
 
     def test_sample_ub(self):
         ws = mantid.CreateWorkspace(DataY=np.ones(1), DataX=np.arange(2))
         args = {'a': 1, 'b': 1, 'c': 1, 'alpha': 90, 'beta': 90, 'gamma': 90}
         mantid.SetUB(ws, **args)
         d = scn.mantid.from_mantid(ws)
         assert sc.identical(
@@ -886,28 +879,28 @@
         )
         moved = scn.mantid.convert_Workspace2D_to_data_array(eventWS)
         moved_det_position = moved.coords["position"]
         unmoved = scn.mantid.convert_Workspace2D_to_data_array(eventWS)
         unmoved_det_positions = unmoved.coords["position"]
         # Moving the sample accounted for in position calculations
         # but should not yield change to final detector positions
-        self.assertTrue(
-            np.all(np.isclose(moved_det_position.values, unmoved_det_positions.values))
+        assert np.all(
+            np.isclose(moved_det_position.values, unmoved_det_positions.values)
         )
 
     def test_validate_units(self):
         acceptable = ["wavelength", "Wavelength"]
         for i in acceptable:
             ret = scn.mantid.validate_dim_and_get_mantid_string(i)
-            self.assertEqual(ret, "Wavelength")
+            assert ret == 'Wavelength'
 
     def test_validate_units_throws(self):
         not_acceptable = [None, "None", "wavlength", 1, 1.0, ["wavelength"]]
         for i in not_acceptable:
-            with self.assertRaises(RuntimeError):
+            with pytest.raises(RuntimeError):
                 scn.mantid.validate_dim_and_get_mantid_string(i)
 
     def test_WorkspaceGroup_parsed_correctly(self):
         from mantid.simpleapi import CreateSampleWorkspace, GroupWorkspaces, mtd
 
         CreateSampleWorkspace(OutputWorkspace="ws1")
         CreateSampleWorkspace(OutputWorkspace="ws2")
@@ -955,15 +948,15 @@
     rot = scn.mantid._rot_from_vectors(b, a)
     assert np.allclose((rot * b).value, a.value)
 
 
 @pytest.mark.skipif(not memory_is_at_least_gb(8), reason='Insufficient virtual memory')
 @pytest.mark.parametrize(
     "param_dim",
-    ('tof', 'wavelength', 'energy', 'dspacing', 'Q', 'Q^2', 'energy_transfer'),
+    ['tof', 'wavelength', 'energy', 'dspacing', 'Q', 'Q^2', 'energy_transfer'],
 )
 def test_to_workspace_2d(param_dim):
     from mantid.simpleapi import mtd
 
     mtd.clear()
 
     data_len = 2
@@ -1038,15 +1031,15 @@
 
     ws = scn.to_mantid(data, "tof")
 
     assert ws.getNumberHistograms() == 2
     assert np.equal(ws.readX(0), expected_x).all()
     assert np.equal(ws.readX(1), expected_x).all()
 
-    for i, (y_vals, e_vals) in enumerate(zip(expected_y, expected_e)):
+    for i, (y_vals, e_vals) in enumerate(zip(expected_y, expected_e, strict=True)):
         assert np.equal(ws.readY(i), y_vals).all()
         assert np.equal(ws.readE(i), np.sqrt(e_vals)).all()
 
 
 def test_attrs_with_dims():
     import mantid.simpleapi as sapi
     from mantid.kernel import FloatArrayProperty
@@ -1233,15 +1226,15 @@
     monitors = scn.mantid.from_mantid(ws)["monitors"]
     assert monitors['monitor_1']['data'].coords['spectrum'].value == 1
     assert monitors['monitor_13']['data'].coords['spectrum'].value == 13
     assert monitors['monitor_14']['data'].coords['spectrum'].value == 14
 
 
 def test_load_error_when_file_not_found_via_fuzzy_match():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='fictional.nxs'):
         scn.load_with_mantid("fictional.nxs")
 
 
 def make_dynamic_algorithm_without_fileproperty(alg_name):
     from mantid.api import (
         AlgorithmFactory,
         PythonAlgorithm,
@@ -1269,22 +1262,22 @@
     Alg.__name__ = alg_name
     AlgorithmFactory.subscribe(Alg)
     importlib.reload(sys.modules["mantid.simpleapi"])
 
 
 def test_load_error_when_file_not_found_via_exact_match():
     make_dynamic_algorithm_without_fileproperty("DummyLoader")
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='fictional.nxs'):
         # DummyLoader has no FileProperty and forces
         # load to evaluate the path given as an absolute path
         scn.load_with_mantid("fictional.nxs", mantid_alg="DummyLoader")
 
 
 def test_load_via_exact_match():
     make_dynamic_algorithm_without_fileproperty("DummyLoader")
     # scn.load_with_mantid will need to check file exists
     # DummyLoader simply returns a TableWorkspace
     with tempfile.NamedTemporaryFile() as fp:
         scn.load_with_mantid(fp.name, mantid_alg="DummyLoader")
         # Sanity check corrupt full path will fail
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError, match='fictional_'):
             scn.load_with_mantid("fictional_" + fp.name, mantid_alg="DummyLoader")
```

### Comparing `scippneutron-24.3.0/tests/tof/chopper_cascade_test.py` & `scippneutron-24.5.0/tests/tof/chopper_cascade_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     subframe = chopper_cascade.Subframe(time=time, wavelength=wavelength)
     assert_identical(subframe.start_time, sc.scalar(0.0, unit='s'))
     assert_identical(subframe.end_time, sc.scalar(0.003, unit='s'))
     assert_identical(subframe.start_wavelength, sc.scalar(10.0, unit='angstrom'))
     assert_identical(subframe.end_wavelength, sc.scalar(21.0, unit='angstrom'))
 
 
-@pytest.fixture
+@pytest.fixture()
 def frame() -> chopper_cascade.Frame:
     time = sc.array(dims=['vertex'], values=[0.0, 1.0, 3.0, 2.0], unit='ms')
     wavelength = sc.array(dims=['vertex'], values=[1.0, 1.1, 2.1, 2.0], unit='nm')
     subframe1 = chopper_cascade.Subframe(time=time, wavelength=wavelength)
     subframe2 = chopper_cascade.Subframe(time=time * 2.0, wavelength=wavelength * 3.0)
     return chopper_cascade.Frame(
         distance=sc.scalar(1.0, unit='m'), subframes=[subframe1, subframe2]
@@ -189,15 +189,15 @@
     frame: chopper_cascade.Frame,
 ) -> None:
     chopper = chopper_cascade.Chopper(
         distance=sc.scalar(0.9, unit='m'),
         time_open=sc.array(dims=['slit'], values=[0.0], unit='s'),
         time_close=sc.array(dims=['slit'], values=[1.0], unit='s'),
     )
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match='smaller than frame distance'):
         frame.chop(chopper)
 
 
 def test_frame_chop_trims_subframes_using_chopper_open() -> None:
     time = sc.array(dims=['vertex'], values=[0.0, 2.0, 4.0, 2.0], unit='s')
     wavelength = sc.array(
         dims=['vertex'], values=[10.0, 10.0, 20.0, 20.0], unit='angstrom'
@@ -362,15 +362,15 @@
             )
         ],
     )
     assert len(frames) == 1
     assert frames[0] == expected
 
 
-@pytest.fixture
+@pytest.fixture()
 def source_frame_sequence() -> chopper_cascade.FrameSequence:
     return chopper_cascade.FrameSequence.from_source_pulse(
         time_min=sc.scalar(0.0, unit='ms'),
         time_max=sc.scalar(1.0, unit='ms'),
         wavelength_min=sc.scalar(1.0, unit='angstrom'),
         wavelength_max=sc.scalar(10.0, unit='angstrom'),
     )
```

### Comparing `scippneutron-24.3.0/tests/tof/fakes_test.py` & `scippneutron-24.5.0/tests/tof/fakes_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 import scipp as sc
 from scipp.testing import assert_identical
 
 from scippneutron.tof import fakes
 
 
-@pytest.fixture
+@pytest.fixture()
 def ess_10s_14Hz() -> fakes.FakeSource:
     return fakes.FakeSource(
         frequency=sc.scalar(14.0, unit='Hz'), run_length=sc.scalar(10.0, unit='s')
     )
 
 
 def test_fake_source(ess_10s_14Hz) -> None:
```

### Comparing `scippneutron-24.3.0/tests/tof/to_time_of_flight_test.py` & `scippneutron-24.5.0/tests/tof/to_time_of_flight_test.py`

 * *Files identical despite different names*

### Comparing `scippneutron-24.3.0/tests/tof/unwrap_test.py` & `scippneutron-24.5.0/tests/tof/unwrap_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from scipp.testing import assert_identical
 
 from scippneutron.tof import fakes, unwrap
 
 sl = pytest.importorskip('sciline')
 
 
-@pytest.fixture
+@pytest.fixture()
 def ess_10s_14Hz() -> fakes.FakeSource:
     return fakes.FakeSource(
         frequency=sc.scalar(14.0, unit='Hz'), run_length=sc.scalar(10.0, unit='s')
     )
 
 
-@pytest.fixture
+@pytest.fixture()
 def ess_10s_7Hz() -> fakes.FakeSource:
     return fakes.FakeSource(
         frequency=sc.scalar(7.0, unit='Hz'), run_length=sc.scalar(10.0, unit='s')
     )
 
 
-@pytest.fixture
+@pytest.fixture()
 def ess_pulse() -> fakes.FakePulse:
     return fakes.FakePulse(
         time_min=sc.scalar(0.0, unit='ms'),
         time_max=sc.scalar(3.0, unit='ms'),
         wavelength_min=sc.scalar(0.1, unit='angstrom'),
         wavelength_max=sc.scalar(10.0, unit='angstrom'),
     )
```

### Comparing `scippneutron-24.3.0/tools/make_tutorial_data.ipynb` & `scippneutron-24.5.0/tools/make_tutorial_data.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9934668485449736%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(6, 'filename, _ = urllib.request.urlretrieve(url)  # noqa: "*

 * *            'S310\\n\')], delete: [6]}}, 1: {\'source\': {insert: [(3, "filename, _ = '*

 * *            'urllib.request.urlretrieve(url, filename=\'PG3_4844_event.nxs\')  # noqa: S310")], '*

 * *            'delete: [3]}}, 2: {\'source\': {insert: [(3, "da = '*

 * *            'scn.load_with_mantid(filename=\'PG3_4844_event.nxs\', load_pulse_times=True)\\n")], '*

 * *            'delete: [3]}}}',*

 * * "'metadata'": "{'language_info […]*

```diff
@@ -9,15 +9,15 @@
             "source": [
                 "import numpy as np\n",
                 "import scipp as sc\n",
                 "import scippneutron as scn\n",
                 "import urllib.request\n",
                 "\n",
                 "url = 'https://github.com/ess-dmsc-dram/loki_tube_scripts/raw/master/test/test_data/LARMOR00049338.nxs'\n",
-                "filename, _ = urllib.request.urlretrieve(url)\n",
+                "filename, _ = urllib.request.urlretrieve(url)  # noqa: S310\n",
                 "data = scn.load_with_mantid(filename=filename)\n",
                 "edges = sc.array(dims=['tof'], unit='us', values=np.linspace(5.0, 100000.0, num=201))\n",
                 "data = sc.rebin(data, 'tof', edges)\n",
                 "for i in [1, 2, 3, 4, 5]:\n",
                 "    mon = data.attrs[f'monitor{i}']\n",
                 "    mon.value = sc.rebin(mon.value, 'tof', edges)\n",
                 "data.to_hdf5(filename='loki-at-larmor.hdf5')"
@@ -29,28 +29,28 @@
             "id": "5328874d-f101-43ea-82aa-41f97d360247",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import urllib\n",
                 "\n",
                 "url = 'http://198.74.56.37/ftp/external-data/MD5/d5ae38871d0a09a28ae01f85d969de1e'\n",
-                "filename, _ = urllib.request.urlretrieve(url, filename='PG3_4844_event.nxs')"
+                "filename, _ = urllib.request.urlretrieve(url, filename='PG3_4844_event.nxs')  # noqa: S310"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "71896365-76be-426d-986f-7aeffd8d3acb",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import scipp as sc\n",
                 "import scippneutron as scn\n",
                 "\n",
-                "da = scn.load_with_mantid(filename=f'PG3_4844_event.nxs', load_pulse_times=True)\n",
+                "da = scn.load_with_mantid(filename='PG3_4844_event.nxs', load_pulse_times=True)\n",
                 "\n",
                 "# Fake d-spacing shift\n",
                 "da = scn.convert(da, 'tof', 'dspacing', scatter=True)\n",
                 "proton_charge = da.attrs['proton_charge'].value\n",
                 "tmin = proton_charge.coords['time'].min()\n",
                 "tmax = proton_charge.coords['time'].max()\n",
                 "delta = sc.to_unit(tmax - tmin, 'us')\n",
@@ -88,13 +88,14 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3"
+            "pygments_lexer": "ipython3",
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `scippneutron-24.3.0/tox.ini` & `scippneutron-24.5.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tox]
-envlist = py39
+envlist = py310
 isolated_build = true
 
 [testenv]
 deps = -r requirements/test.txt
 setenv =
   JUPYTER_PLATFORM_DIRS = 1
 commands = pytest {posargs}
 
 [testenv:nightly]
 deps = -r requirements/nightly.txt
-commands = pytest
+commands = pytest {posargs}
 
 [testenv:unpinned]
 description = Test with unpinned dependencies, as a user would install now.
 deps =
   -r requirements/basetest.txt
   scippneutron[all]
-commands = pytest
+commands = pytest {posargs}
 
 [testenv:static]
 description = Code formatting and static analysis
 skip_install = true
 deps = -r requirements/static.txt
 allowlist_externals = sh
 # The first run of pre-commit may reformat files. If this happens, it returns 1 but this
```

