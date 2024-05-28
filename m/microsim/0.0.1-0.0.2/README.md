# Comparing `tmp/microsim-0.0.1.tar.gz` & `tmp/microsim-0.0.2.tar.gz`

## Comparing `microsim-0.0.1.tar` & `microsim-0.0.2.tar`

### file list

```diff
@@ -1,72 +1,82 @@
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 microsim-0.0.1/.github_changelog_generator
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 microsim-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 microsim-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 microsim-0.0.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 microsim-0.0.1/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 microsim-0.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 microsim-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 microsim-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 microsim-0.0.1/docs/api.md
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 microsim-0.0.1/docs/concept.md
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 microsim-0.0.1/docs/index.md
--rw-r--r--   0        0        0    13446 2020-02-02 00:00:00.000000 microsim-0.0.1/docs/images/au02.png
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 microsim-0.0.1/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 microsim-0.0.1/examples/basic_confocal.py
--rw-r--r--   0        0        0   882468 2020-02-02 00:00:00.000000 microsim-0.0.1/examples/confocal.ipynb
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 microsim-0.0.1/examples/fftconv_bench.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 microsim-0.0.1/examples/illum_widget.py
--rw-r--r--   0        0        0   826527 2020-02-02 00:00:00.000000 microsim-0.0.1/examples/old_confocal.ipynb
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 microsim-0.0.1/examples/sim3d.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/__init__.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/_data_array.py
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/fpbase.py
--rw-r--r--   0        0        0    12010 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/psf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/py.typed
--rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/util.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/cosem/__init__.py
--rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/cosem/_cosem.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/cosem/_dataset.py
--rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/cosem/_xarray.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/cosem/download_cosem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/illum/__init__.py
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/illum/_sim.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/illum/_spinning_disc.py
--rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/samples/organelles.json
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/__init__.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/_base_model.py
--rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/_jax_bessel.py
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/backend.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/lens.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/settings.py
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/simulation.py
--rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/space.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/spectrum.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/detectors/__init__.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/detectors/_camera.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/detectors/_simulate.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/modality/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/modality/confocal.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/modality/widefield.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/optical_config/__init__.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/optical_config/config.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/optical_config/filter.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/sample/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/sample/fluorophore.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/sample/sample.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/sample/matslines/__init__.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/sample/matslines/_bresenham.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 microsim-0.0.1/src/microsim/schema/sample/matslines/_matslines.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 microsim-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0   147584 2020-02-02 00:00:00.000000 microsim-0.0.1/tests/illum_ref.npy
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 microsim-0.0.1/tests/test_bresenham.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 microsim-0.0.1/tests/test_cosem.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 microsim-0.0.1/tests/test_fpbase.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 microsim-0.0.1/tests/test_matslines.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 microsim-0.0.1/tests/test_schema.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 microsim-0.0.1/tests/test_sim_illum.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 microsim-0.0.1/tests/test_spinning_disc.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 microsim-0.0.1/.gitignore
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 microsim-0.0.1/LICENSE
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 microsim-0.0.1/README.md
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 microsim-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 microsim-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 microsim-0.0.2/.github_changelog_generator
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 microsim-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 microsim-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 microsim-0.0.2/x.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 microsim-0.0.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 microsim-0.0.2/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 microsim-0.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 microsim-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 microsim-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 microsim-0.0.2/docs/api.md
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 microsim-0.0.2/docs/concept.md
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 microsim-0.0.2/docs/index.md
+-rw-r--r--   0        0        0    13446 2020-02-02 00:00:00.000000 microsim-0.0.2/docs/images/au02.png
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 microsim-0.0.2/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 microsim-0.0.2/examples/basic_confocal.py
+-rw-r--r--   0        0        0   882468 2020-02-02 00:00:00.000000 microsim-0.0.2/examples/confocal.ipynb
+-rw-r--r--   0        0        0   404992 2020-02-02 00:00:00.000000 microsim-0.0.2/examples/direct_truth.ipynb
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 microsim-0.0.2/examples/emission_events.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 microsim-0.0.2/examples/fftconv_bench.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 microsim-0.0.2/examples/illum_widget.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 microsim-0.0.2/examples/sim3d.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/__init__.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/_data_array.py
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/_field_types.py
+-rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/fpbase.py
+-rw-r--r--   0        0        0    11985 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/psf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/py.typed
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/util.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/cosem/__init__.py
+-rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/cosem/_cosem.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/cosem/_dataset.py
+-rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/cosem/_xarray.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/cosem/download_cosem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/fft/__init__.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/fft/backends.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/fft/convolve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/illum/__init__.py
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/illum/_sim.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/illum/_spinning_disc.py
+-rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/samples/organelles.json
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/_base_model.py
+-rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/_jax_bessel.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/_validators.py
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/backend.py
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/lens.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/settings.py
+-rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/simulation.py
+-rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/space.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/spectrum.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/detectors/__init__.py
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/detectors/_camera.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/detectors/_simulate.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/modality/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/modality/confocal.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/modality/widefield.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/optical_config/__init__.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/optical_config/config.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/optical_config/filter.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/sample/__init__.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/sample/direct.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/sample/fluorophore.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/sample/sample.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/sample/matslines/__init__.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/sample/matslines/_bresenham.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 microsim-0.0.2/src/microsim/schema/sample/matslines/_matslines.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 microsim-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0   147584 2020-02-02 00:00:00.000000 microsim-0.0.2/tests/illum_ref.npy
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 microsim-0.0.2/tests/test_bresenham.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 microsim-0.0.2/tests/test_cosem.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 microsim-0.0.2/tests/test_examples.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 microsim-0.0.2/tests/test_fftconv.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 microsim-0.0.2/tests/test_fpbase.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 microsim-0.0.2/tests/test_matslines.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 microsim-0.0.2/tests/test_sim_illum.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 microsim-0.0.2/tests/test_simulation.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 microsim-0.0.2/tests/test_spinning_disc.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 microsim-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 microsim-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 microsim-0.0.2/README.md
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 microsim-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 microsim-0.0.2/PKG-INFO
```

### Comparing `microsim-0.0.1/.pre-commit-config.yaml` & `microsim-0.0.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -23,7 +23,8 @@
         files: "^src/microsim/schema/.*\\.py$"
         additional_dependencies:
           - numpy
           - pydantic
           - pydantic-settings
           - xarray
           - types-tqdm
+          - pint
```

### Comparing `microsim-0.0.1/mkdocs.yml` & `microsim-0.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/.github/workflows/ci.yml` & `microsim-0.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/.github/workflows/docs.yml` & `microsim-0.0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/docs/api.md` & `microsim-0.0.2/docs/api.md`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/docs/concept.md` & `microsim-0.0.2/docs/concept.md`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/docs/index.md` & `microsim-0.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/docs/images/au02.png` & `microsim-0.0.2/docs/images/au02.png`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/docs/stylesheets/extra.css` & `microsim-0.0.2/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/examples/confocal.ipynb` & `microsim-0.0.2/examples/confocal.ipynb`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/examples/fftconv_bench.py` & `microsim-0.0.2/examples/fftconv_bench.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # fftconvolve_benchmark.py
 
 import time
 
-import cupy
-import cupyx.scipy.signal as cuf
+try:
+    import cupy
+    import cupyx.scipy.signal as cuf
+except ImportError:
+    cupy = None
+
 import jax.numpy as jnp
 import jax.scipy.signal as jsig
 import numpy as np
 import torch
 import torchaudio.functional as taf
 from scipy.signal import fftconvolve
 
@@ -66,15 +70,16 @@
     # Benchmark PyTorch
     torch_signal = torch.asarray(np_signal)
     torch_kernel = torch.asarray(np_kernel)
     torch_time, mint = benchmark(torch_fftconvolve, torch_signal, torch_kernel)
     print(f"PyTorch FFT Convolve: {torch_time:.6f} seconds, {mint:.6f} seconds")
 
     # Benchmark CuPy
-    cupy_signal = cupy.asarray(np_signal)
-    cupy_kernel = cupy.asarray(np_kernel)
-    cupy_time, mint = benchmark(cupy_fftconvolve, cupy_signal, cupy_kernel)
-    print(f"CuPy FFT Convolve: {cupy_time:.6f} seconds, {mint:.6f} seconds")
+    if cupy is not None:
+        cupy_signal = cupy.asarray(np_signal)
+        cupy_kernel = cupy.asarray(np_kernel)
+        cupy_time, mint = benchmark(cupy_fftconvolve, cupy_signal, cupy_kernel)
+        print(f"CuPy FFT Convolve: {cupy_time:.6f} seconds, {mint:.6f} seconds")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `microsim-0.0.1/examples/illum_widget.py` & `microsim-0.0.2/examples/illum_widget.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/_data_array.py` & `microsim-0.0.2/src/microsim/_data_array.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/fpbase.py` & `microsim-0.0.2/src/microsim/fpbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import json
 from functools import cache
 from typing import Any, Literal
 from urllib.request import Request, urlopen
 
 from pydantic import BaseModel, Field, field_validator, model_validator
 
+from microsim._field_types import ExtCoeff, Nanometers, Nanoseconds
+
 __all__ = ["get_fluorophore", "get_microscope", "FPbaseFluorophore", "FPbaseMicroscope"]
 
-FPBASE_URL = "https://www.fpbase.org/graphql/"
+
+### Models ###
+
 SpectrumType = Literal[
     "A_2P", "BM", "BP", "BS", "BX", "EM", "EX", "LP", "PD", "QE", "AB"
 ]
 
-### Models ###
-
 
 class Spectrum(BaseModel):
     subtype: SpectrumType
     data: list[tuple[float, float]] = Field(..., repr=False)
 
 
 class SpectrumOwner(BaseModel):
     name: str
     spectrum: Spectrum
 
 
 class State(BaseModel):
     id: int
-    exMax: float
-    emMax: float
-    extCoeff: float
+    exMax: Nanometers
+    emMax: Nanometers
+    extCoeff: ExtCoeff
     qy: float
     spectra: list[Spectrum]
+    lifetime: Nanoseconds | None = None
 
     @property
     def excitation_spectrum(self) -> Spectrum | None:
         spect = next((s for s in self.spectra if s.subtype == "EX"), None)
         if not spect:
             spect = next((s for s in self.spectra if s.subtype == "AB"), None)
         return spect
@@ -110,15 +113,17 @@
     dye: FPbaseFluorophore
 
 
 class DyeResponse(BaseModel):
     data: DyePayload
 
 
-### Getter Functions ###
+### Graphql Queries ###
+
+FPBASE_URL = "https://www.fpbase.org/graphql/"
 
 
 @cache
 def get_microscope(id: str) -> FPbaseMicroscope:
     query = """
     {{
         microscope(id: "{id}") {{
@@ -214,14 +219,15 @@
             states {{
                 id
                 name
                 exMax
                 emMax
                 extCoeff
                 qy
+                lifetime
                 spectra {{ subtype data }}
             }}
             defaultState {{
                 id
             }}
         }}
     }}
```

### Comparing `microsim-0.0.1/src/microsim/psf.py` & `microsim-0.0.2/src/microsim/psf.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,16 +153,17 @@
     off: Sequence[int] | None = None,
     xp: NumpyAPI | None = None,
 ) -> npt.NDArray:
     """Use interpolation to create a 3D XYZ PSF from a 2D ZR PSF."""
     xp = NumpyAPI.create(xp)
 
     # Create XY grid of radius values.
-    rmap = radius_map(xyshape, off) * sf
+    rmap = radius_map(xyshape, off, xp=xp) * sf
     nz = rz.shape[0]
+
     out = xp.asarray(
         [
             xp.map_coordinates(
                 rz, xp.asarray([xp.ones(rmap.size) * z, rmap.ravel()]), order=1
             ).reshape(xyshape)
             for z in range(nz)
         ]
@@ -197,15 +198,15 @@
     zv = tuple(np.asarray(zv) * 1e-6)  # convert to meters
     ny = ny or nx
     rz = vectorial_rz(
         zv, np.maximum(ny, nx), pos, dxy, wvl, objective=objective, sf=sf, xp=xp
     ).astype(xp.float_dtype)
 
     offsets = xp.asarray(pos[:2]) / (dxy * 1e-6)
-    _psf = rz_to_xyz(rz, (ny, nx), sf, off=offsets)  # type: ignore [arg-type]
+    _psf = rz_to_xyz(rz, (ny, nx), sf, off=offsets, xp=xp)  # type: ignore [arg-type]
     if normalize:
         _psf /= xp.max(_psf)
     return _psf
 
 
 def _centered_zv(nz: int, dz: float, pz: float = 0) -> tuple[float, ...]:
     lim = (nz - 1) * dz / 2
@@ -345,30 +346,27 @@
     space: SpaceProtocol,
     channel: OpticalConfig,
     objective: ObjectiveLens,
     pinhole_au: float | None = None,
     max_au_relative: float | None = None,
     xp: NumpyAPI | None = None,
 ) -> ArrayProtocol:
-    xp = NumpyAPI.create(xp)
     nz, _ny, nx = space.shape
     dz, _dy, dx = space.scale
-    ex_wvl_um = channel.excitation.bandcenter * 1e-3
-    em_wvl_um = channel.emission.bandcenter * 1e-3
     return cached_psf(
         nz=nz,
         nx=nx,
         dx=dx,
         dz=dz,
-        ex_wvl_um=ex_wvl_um,
-        em_wvl_um=em_wvl_um,
+        ex_wvl_um=channel.excitation.bandcenter.to("um").magnitude,
+        em_wvl_um=channel.emission.bandcenter.to("um").magnitude,
         objective=_cast_objective(objective),
         pinhole_au=pinhole_au,
         max_au_relative=max_au_relative,
-        xp=xp,
+        xp=NumpyAPI.create(xp),
     )
 
 
 # variant of make_psf that only accepts hashable arguments
 @cache
 def cached_psf(
     nz: int,
```

### Comparing `microsim-0.0.1/src/microsim/util.py` & `microsim-0.0.2/src/microsim/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -210,25 +210,29 @@
         return _centered(out, in1.shape)
     elif mode == "valid":
         return _centered(out, get_fftconvolve_shape(in1, in2, mode="valid"))
     return out
 
 
 # convenience function we'll use a couple times
-def ortho_plot(img: ArrayProtocol, gamma: float = 0.5, mip: bool = False) -> None:
+def ortho_plot(
+    img: ArrayProtocol, gamma: float = 0.5, mip: bool = False, cmap: str = "gray"
+) -> None:
     import matplotlib.pyplot as plt
     from matplotlib.colors import PowerNorm
 
+    if hasattr(img, "get"):
+        img = img.get()
     img = np.asarray(img)
     """Plot XY and XZ slices of a 3D array."""
     _, ax = plt.subplots(ncols=2, figsize=(10, 5))
     xy = img.max(axis=0) if mip else img[img.shape[0] // 2]
     xz = img.max(axis=1) if mip else img[:, img.shape[1] // 2]
-    ax[0].imshow(xy, norm=PowerNorm(gamma))
-    ax[1].imshow(xz, norm=PowerNorm(gamma))
+    ax[0].imshow(xy, norm=PowerNorm(gamma), cmap=cmap)
+    ax[1].imshow(xz, norm=PowerNorm(gamma), cmap=cmap)
     ax[0].set_title("XY slice")
     ax[1].set_title("XZ slice")
     plt.show()
 
 
 ArrayType = TypeVar("ArrayType", bound=ArrayProtocol)
```

### Comparing `microsim-0.0.1/src/microsim/cosem/_cosem.py` & `microsim-0.0.2/src/microsim/cosem/_cosem.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/cosem/_dataset.py` & `microsim-0.0.2/src/microsim/cosem/_dataset.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/cosem/_xarray.py` & `microsim-0.0.2/src/microsim/cosem/_xarray.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/cosem/download_cosem.py` & `microsim-0.0.2/src/microsim/cosem/download_cosem.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/illum/_sim.py` & `microsim-0.0.2/src/microsim/illum/_sim.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/illum/_spinning_disc.py` & `microsim-0.0.2/src/microsim/illum/_spinning_disc.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/samples/organelles.json` & `microsim-0.0.2/src/microsim/samples/organelles.json`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/schema/__init__.py` & `microsim-0.0.2/src/microsim/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/schema/_jax_bessel.py` & `microsim-0.0.2/src/microsim/schema/_jax_bessel.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/schema/backend.py` & `microsim-0.0.2/src/microsim/schema/backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 if TYPE_CHECKING:
     from collections.abc import Sequence
     from types import ModuleType
     from typing import SupportsIndex, TypeAlias
 
     import jax
 
+    from microsim._data_array import ArrayProtocol
+
     _Shape: TypeAlias = tuple[int, ...]
 
     # Anything that can be coerced to a shape tuple
     _ShapeLike: TypeAlias = SupportsIndex | Sequence[SupportsIndex]
 
 DeviceName = Literal["cpu", "gpu", "auto"]
 BackendName = Literal["numpy", "torch", "jax", "cupy", "auto"]
@@ -43,26 +45,27 @@
                 return JaxAPI()
         elif backend in ("torch", "auto"):
             with ctx:
                 return TorchAPI()
 
         return NumpyAPI()
 
+    _random_seed: int | None = None
+    _float_dtype: np.dtype | None = None
+
     def __init__(self) -> None:
         from scipy import signal, special, stats
         from scipy.ndimage import map_coordinates
 
-        self._random_seed: int | None = None
         self.xp = np
         self.signal = signal
         self.stats = stats
         self.j0 = special.j0
         self.j1 = special.j1
         self.map_coordinates = map_coordinates
-        self._float_dtype: np.dtype | None = None
 
     @property
     def float_dtype(self) -> np.dtype | None:
         return self._float_dtype
 
     @float_dtype.setter
     def float_dtype(self, dtype: npt.DTypeLike) -> None:
@@ -99,14 +102,19 @@
         return getattr(self.xp, name)
 
     def poisson_rvs(
         self, lam: npt.ArrayLike, shape: Sequence[int] | None = None
     ) -> npt.NDArray:
         return self.stats.poisson.rvs(lam, size=shape)  # type: ignore
 
+    def norm_rvs(
+        self, loc: ArrayProtocol, scale: npt.ArrayLike | None = None
+    ) -> ArrayProtocol:
+        return self.stats.norm.rvs(loc, scale)  # type: ignore
+
     def fftconvolve(
         self, a: ArrT, b: ArrT, mode: Literal["full", "valid", "same"] = "full"
     ) -> ArrT:
         return self.signal.fftconvolve(a, b, mode=mode)  # type: ignore
 
     def _simp_like(self, arr: npt.ArrayLike) -> npt.ArrayLike:
         simp = self.xp.empty_like(arr)
@@ -136,15 +144,14 @@
         import jax
         from jax.random import PRNGKey
         from jax.scipy import signal, stats
         from jax.scipy.ndimage import map_coordinates
 
         from ._jax_bessel import j0, j1
 
-        self._random_seed: int | None = None
         self.xp = jax.numpy
         self.signal = signal
         self.stats = stats
         self.map_coordinates = map_coordinates
         self.j0 = j0
         self.j1 = j1
         self._key = PRNGKey(0)
@@ -169,14 +176,23 @@
         lam: jax.Array | float,
         shape: Sequence[int] | None = None,
     ) -> jax.Array:
         from jax.random import poisson
 
         return poisson(self._key, lam, shape=shape)
 
+    def norm_rvs(
+        self, loc: ArrayProtocol, scale: npt.ArrayLike | None = None
+    ) -> ArrayProtocol:
+        from jax.random import normal
+
+        std_samples = normal(self._key, shape=loc.shape)
+        # scale and shift
+        return std_samples * scale + loc  # type: ignore
+
     def fftconvolve(
         self, a: ArrT, b: ArrT, mode: Literal["full", "valid", "same"] = "full"
     ) -> ArrT:
         return self.signal.fftconvolve(a, b, mode=mode)  # type: ignore[no-any-return]
 
     def _simp_like(self, arr: jax.Array) -> jax.Array:
         simp = self.xp.empty_like(arr)
@@ -207,14 +223,24 @@
         self.xp = cupy
         self.signal = signal
         self.stats = stats
         self.j0 = special.j0
         self.j1 = special.j1
         self.map_coordinates = map_coordinates
 
+    def poisson_rvs(
+        self, lam: npt.ArrayLike, shape: Sequence[int] | None = None
+    ) -> npt.NDArray:
+        return self.xp.random.poisson(lam, shape)  # type: ignore
+
+    def norm_rvs(
+        self, loc: ArrayProtocol, scale: npt.ArrayLike | None = None
+    ) -> ArrayProtocol:
+        return self.xp.random.normal(loc, scale)  # type: ignore
+
     def fftconvolve(
         self, a: ArrT, b: ArrT, mode: Literal["full", "valid", "same"] = "full"
     ) -> ArrT:
         return self.signal.fftconvolve(a, b, mode=mode)  # type: ignore
 
 
 class TorchAPI(NumpyAPI):
```

### Comparing `microsim-0.0.1/src/microsim/schema/lens.py` & `microsim-0.0.2/src/microsim/schema/lens.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Any, TypedDict
 
 import numpy as np
 from pydantic import Field, model_validator
 
+from microsim._field_types import Microns
+
 from ._base_model import SimBaseModel
 
 
 class ObjectiveKwargs(TypedDict, total=False):
     numerical_aperture: float
     coverslip_ri: float
     coverslip_ri_spec: float
@@ -22,17 +24,20 @@
 class ObjectiveLens(SimBaseModel):
     numerical_aperture: float = Field(1.4, alias="na")
     coverslip_ri: float = 1.515  # coverslip RI experimental value (ng)
     coverslip_ri_spec: float = 1.515  # coverslip RI design value (ng0)
     immersion_medium_ri: float = 1.515  # immersion medium RI experimental value (ni)
     immersion_medium_ri_spec: float = 1.515  # immersion medium RI design value (ni0)
     specimen_ri: float = 1.47  # specimen refractive index (ns)
-    working_distance: float = 150.0  # um, working distance, design value (ti0)
-    coverslip_thickness: float = 170.0  # um, coverslip thickness (tg)
-    coverslip_thickness_spec: float = 170.0  # um, coverslip thickness design (tg0)
+    # um, working distance, design value (ti0)
+    working_distance: Microns = 150.0  # type: ignore
+    # um, coverslip thickness (tg)
+    coverslip_thickness: Microns = 170.0  # type: ignore
+    # um, coverslip thickness design (tg0)
+    coverslip_thickness_spec: Microns = 170.0  # type: ignore
 
     magnification: float = Field(1, description="magnification of objective lens.")
 
     def __hash__(self) -> int:
         return hash(
             (
                 self.numerical_aperture,
@@ -74,23 +79,23 @@
 
     @property
     def ng(self) -> float:
         return self.coverslip_ri
 
     @property
     def tg(self) -> float:
-        return self.coverslip_thickness * 1e-6
+        return float(self.coverslip_thickness.to("meters").magnitude)
 
     @property
     def tg0(self) -> float:
-        return self.coverslip_thickness_spec * 1e-6
+        return float(self.coverslip_thickness_spec.to("meters").magnitude)
 
     @property
     def ti0(self) -> float:
-        return self.working_distance * 1e-6
+        return float(self.working_distance.to("meters").magnitude)
 
     @property
     def ng0(self) -> float:
         return self.coverslip_ri_spec
 
     @property
     def ni0(self) -> float:
```

### Comparing `microsim-0.0.1/src/microsim/schema/settings.py` & `microsim-0.0.2/src/microsim/schema/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,24 @@
 import random
-from typing import Annotated, Any, ClassVar
+from typing import ClassVar
 
-import numpy as np
 from pydantic import Field
-from pydantic.functional_serializers import PlainSerializer
-from pydantic.functional_validators import PlainValidator
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
+from microsim._field_types import FloatDtype
+
 from ._base_model import SimBaseModel
 from .backend import BackendName, DeviceName, NumpyAPI
 
 
-def _np_float_dtype(x: Any) -> np.dtype:
-    dt = np.dtype(x)
-    if not np.issubdtype(dt, np.floating):
-        raise ValueError(f"Expected a floating-point dtype, got {dt}")
-    return dt
-
-
-NpDtype = Annotated[
-    np.dtype,
-    PlainValidator(_np_float_dtype),
-    PlainSerializer(lambda x: str(x), return_type=str),
-]
-
-
 class Settings(SimBaseModel, BaseSettings):
-    model_config: ClassVar[SettingsConfigDict] = SettingsConfigDict(
-        validate_assignment=True
-    )
-
     np_backend: BackendName = "auto"
     device: DeviceName = "auto"
-    float_dtype: NpDtype = Field(
-        np.dtype("float32"),
+    float_dtype: FloatDtype = Field(  # type: ignore[assignment]
+        "float32",
         description="Floating-point precision to use for simulations.",
     )
     random_seed: int | None = Field(
         default_factory=lambda: random.randint(0, 2**32 - 1)
     )
     max_psf_radius_aus: float | None = Field(
         8,
@@ -45,13 +26,17 @@
             "When simulating, restrict generated lateral PSF size to no more than this "
             "many Airy units. Decreasing this can *dramatically* speed up simulations, "
             "but will decrease accuracy. If `None`, no restriction is applied, and the "
             "psf will be generated to the full extent of the simulated space."
         ),
     )
 
+    model_config: ClassVar[SettingsConfigDict] = SettingsConfigDict(
+        validate_assignment=True
+    )
+
     def backend_module(self) -> NumpyAPI:
         backend = NumpyAPI.create(self.np_backend)
         backend.float_dtype = self.float_dtype
         if self.random_seed is not None:
             backend.set_random_seed(self.random_seed)
         return backend
```

### Comparing `microsim-0.0.1/src/microsim/schema/simulation.py` & `microsim-0.0.2/src/microsim/schema/simulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Annotated
 
 if TYPE_CHECKING:
-    from typing import Self
+    from typing import Self, Unpack
 
     from .backend import NumpyAPI
 
 from pydantic import AfterValidator, Field, model_validator
 
-from microsim._data_array import DataArray
+from microsim._data_array import ArrayProtocol, DataArray
 
 from ._base_model import SimBaseModel
 from .detectors import Detector
 from .lens import ObjectiveLens
 from .modality import Modality, Widefield
 from .optical_config import FITC, OpticalConfig
-from .sample import Sample
+from .sample import FluorophoreDistribution, Sample
 from .settings import Settings
-from .space import Space, _RelativeSpace
+from .space import ShapeScaleSpace, Space, _RelativeSpace
+
+if TYPE_CHECKING:
+    from typing import TypedDict
+
+    class SimluationKwargs(TypedDict, total=False):
+        output_space: Space | dict | None
+        objective_lens: ObjectiveLens
+        channels: list[OpticalConfig]
+        detector: Detector | None
+        modality: Modality
+        settings: Settings
+        output_path: "OutPath" | None
 
 
 def _check_extensions(path: Path) -> Path:
     if path.suffix not in {".tif", ".tiff", ".zarr", ".nc"}:
         raise ValueError("Recognized extensions include: .tif, .tiff, .zarr")
     return path
 
@@ -38,14 +50,33 @@
     objective_lens: ObjectiveLens = Field(default_factory=ObjectiveLens)
     channels: list[OpticalConfig] = Field(default_factory=lambda: [FITC()])
     detector: Detector | None = None
     modality: Modality = Field(default_factory=Widefield)
     settings: Settings = Field(default_factory=Settings)
     output_path: OutPath | None = None
 
+    @classmethod
+    def from_ground_truth(
+        self,
+        ground_truth: ArrayProtocol,
+        scale: tuple[float, ...],
+        **kwargs: "Unpack[SimluationKwargs]",
+    ) -> "Self":
+        """Shortcut to create a simulation directly from a ground truth array.
+
+        In this case, we bypass derive the `truth_space` and `sample` objects directly
+        from a pre-calculated ground truth array.  `scale` must also be provided as a
+        tuple of floats, one for each dimension of the ground truth array.
+        """
+        return self(
+            truth_space=ShapeScaleSpace(shape=ground_truth.shape, scale=scale),
+            sample=Sample(labels=[FluorophoreDistribution.from_array(ground_truth)]),
+            **kwargs,
+        )
+
     @model_validator(mode="after")
     def _resolve_spaces(self) -> "Self":
         if isinstance(self.truth_space, _RelativeSpace):
             if self.output_space is not None:
                 if isinstance(self.output_space, _RelativeSpace):
                     raise ValueError("Cannot have two relative spaces.")
                 self.truth_space.reference = self.output_space
```

### Comparing `microsim-0.0.1/src/microsim/schema/space.py` & `microsim-0.0.2/src/microsim/schema/space.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/schema/detectors/_camera.py` & `microsim-0.0.2/src/microsim/schema/detectors/_camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,19 @@
         # assume ADC has been set such that voltage at FWC matches max bit depth
         return self.full_well / self.max_intensity
 
     @property
     def max_intensity(self) -> int:
         return int(2**self.bit_depth - 1)
 
-    def quantize_electrons(self, total_electrons: npt.NDArray) -> npt.NDArray:
-        voltage = stats.norm.rvs(total_electrons, self.read_noise) * self.gain
-        return np.round((voltage / self.adc_gain) + self.offset)  # type: ignore
+    def quantize_electrons(
+        self, total_electrons: npt.NDArray, xp: NumpyAPI
+    ) -> npt.NDArray:
+        voltage = xp.norm_rvs(total_electrons, self.read_noise) * self.gain
+        return xp.round((voltage / self.adc_gain) + self.offset)  # type: ignore
 
 
 class CameraCCD(Camera): ...
 
 
 class CameraEMCCD(Camera):
     em_full_well: int
```

### Comparing `microsim-0.0.1/src/microsim/schema/detectors/_simulate.py` & `microsim-0.0.2/src/microsim/schema/detectors/_simulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         total_electrons = bin(total_electrons, binning, "sum")
 
     # add em gain
     if isinstance(camera, CameraEMCCD):
         total_electrons = camera.apply_em_gain(total_electrons)
 
     # model read noise
-    gray_values = camera.quantize_electrons(total_electrons)
+    gray_values = camera.quantize_electrons(total_electrons, xp)
 
     # sCMOS binning
     if binning > 1 and isinstance(camera, CameraCMOS):
         gray_values = bin(gray_values, binning, "mean")
 
     # ADC saturation
     gray_values = xp.minimum(gray_values, camera.max_intensity)
```

### Comparing `microsim-0.0.1/src/microsim/schema/modality/confocal.py` & `microsim-0.0.2/src/microsim/schema/modality/confocal.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/schema/modality/widefield.py` & `microsim-0.0.2/src/microsim/schema/modality/widefield.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/schema/optical_config/config.py` & `microsim-0.0.2/src/microsim/schema/optical_config/config.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/schema/optical_config/filter.py` & `microsim-0.0.2/src/microsim/schema/optical_config/filter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,55 @@
-from typing import Literal
+from typing import Annotated, Literal
 
+from annotated_types import Interval
+
+from microsim._field_types import Nanometers
 from microsim.schema._base_model import SimBaseModel
 from microsim.schema.spectrum import Spectrum
 
+Transmission = Annotated[float, Interval(ge=0, le=1.0)]
+
 
 class _Filter(SimBaseModel):
     type: str
     name: str = ""
 
 
 class Bandpass(_Filter):
     type: Literal["bandpass"] = "bandpass"
-    bandcenter: float
-    bandwidth: float
-    transmission: float = 1.0
+    bandcenter: Nanometers
+    bandwidth: Nanometers
+    transmission: Transmission = 1.0
 
 
 class Shortpass(_Filter):
     type: Literal["shortpass"] = "shortpass"
-    cutoff: float
+    cutoff: Nanometers
     slope: float = 1.0
-    transmission: float = 1.0
+    transmission: Transmission = 1.0
 
     @property
-    def bandcenter(self) -> float:
+    def bandcenter(self) -> Nanometers:
         return self.cutoff
 
 
 class Longpass(_Filter):
     type: Literal["longpass"] = "longpass"
-    cutoff: float
+    cutoff: Nanometers
     slope: float = 1.0
-    transmission: float = 1.0
+    transmission: Transmission = 1.0
 
     @property
-    def bandcenter(self) -> float:
+    def bandcenter(self) -> Nanometers:
         return self.cutoff
 
 
 class FilterSpectrum(_Filter):
     type: Literal["spectrum"] = "spectrum"
     spectrum: Spectrum
 
     @property
-    def bandcenter(self) -> float:
+    def bandcenter(self) -> Nanometers:
         return self.spectrum.peak_wavelength
 
 
 Filter = Bandpass | Shortpass | Longpass | FilterSpectrum
```

### Comparing `microsim-0.0.1/src/microsim/schema/sample/sample.py` & `microsim-0.0.2/src/microsim/schema/sample/sample.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 from typing import Any
 
 from pydantic import Field, model_validator
 
-from microsim._data_array import DataArray
+from microsim._data_array import ArrayProtocol, DataArray
 from microsim.schema._base_model import SimBaseModel
 from microsim.schema.backend import NumpyAPI
 
+from .direct import FixedArrayTruth
 from .fluorophore import Fluorophore
 from .matslines import MatsLines
 
-Distribution = MatsLines
+Distribution = MatsLines | FixedArrayTruth
 
 
 class FluorophoreDistribution(SimBaseModel):
     distribution: Distribution = Field(..., discriminator="type")
     fluorophore: Fluorophore | None = None
 
     def render(self, space: DataArray, xp: NumpyAPI | None = None) -> DataArray:
         return self.distribution.render(space, xp)
 
     @model_validator(mode="before")
     def _vmodel(cls, value: Any) -> Any:
-        if isinstance(value, Distribution):
+        if isinstance(value, (MatsLines | FixedArrayTruth)):  # FIXME
             return {"distribution": value}
         if isinstance(value, dict):
             if "distribution" not in value and "type" in value:
                 return {"distribution": value}
         return value
 
+    @classmethod
+    def from_array(cls, array: ArrayProtocol) -> "FluorophoreDistribution":
+        return cls(distribution=FixedArrayTruth(array=array))
+
 
 class Sample(SimBaseModel):
     labels: list[FluorophoreDistribution]
```

### Comparing `microsim-0.0.1/src/microsim/schema/sample/matslines/_bresenham.py` & `microsim-0.0.2/src/microsim/schema/sample/matslines/_bresenham.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/src/microsim/schema/sample/matslines/_matslines.py` & `microsim-0.0.2/src/microsim/schema/sample/matslines/_matslines.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/tests/conftest.py` & `microsim-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/tests/illum_ref.npy` & `microsim-0.0.2/tests/illum_ref.npy`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/tests/test_bresenham.py` & `microsim-0.0.2/tests/test_bresenham.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/tests/test_fpbase.py` & `microsim-0.0.2/tests/test_fpbase.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/tests/test_sim_illum.py` & `microsim-0.0.2/tests/test_sim_illum.py`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/.gitignore` & `microsim-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/LICENSE` & `microsim-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/README.md` & `microsim-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `microsim-0.0.1/pyproject.toml` & `microsim-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,33 +26,36 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 dependencies = [
-    "pydantic>=2.4",
-    "numpy",
-    "annotated_types",
     'pydantic-settings',
+    "annotated_types",
+    "numpy",
+    "pint>=0.23",
+    "pydantic>=2.4",
     "scipy",
     "tqdm",
     "xarray",
 ]
 
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 cosem = ["xarray-datatree", "s3fs", "dask", "imageio", "supabase"]
 test = [
     "microsim[cosem]",
-    "pytest",
+    "jax[cpu]",
+    "matplotlib",
     "pytest-cov",
-    "zarr",
+    "pytest",
     "tifffile",
-    "jax[cpu]",
+    "torch",
+    "zarr",
 ]
 dev = [
     "microsim[test]",
     "ipython",
     "matplotlib",
     "mypy",
     "types-tqdm",
@@ -132,14 +135,15 @@
 # https://coverage.readthedocs.io/en/6.4/config.html
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
     "@overload",
     "except ImportError",
+    "raise ValueError",
     "\\.\\.\\.",
     "raise NotImplementedError()",
     "pass",
 ]
 
 [tool.coverage.run]
 source = ["microsim"]
```

### Comparing `microsim-0.0.1/PKG-INFO` & `microsim-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: microsim
-Version: 0.0.1
+Version: 0.0.2
 Summary: Light microscopy simulation in python
 Project-URL: homepage, https://github.com/tlambert03/microsim
 Project-URL: repository, https://github.com/tlambert03/microsim
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: annotated-types
 Requires-Dist: numpy
+Requires-Dist: pint>=0.23
 Requires-Dist: pydantic-settings
 Requires-Dist: pydantic>=2.4
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: xarray
 Provides-Extra: cosem
 Requires-Dist: dask; extra == 'cosem'
@@ -40,32 +41,35 @@
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: s3fs; extra == 'dev'
 Requires-Dist: supabase; extra == 'dev'
 Requires-Dist: tifffile; extra == 'dev'
+Requires-Dist: torch; extra == 'dev'
 Requires-Dist: types-tqdm; extra == 'dev'
 Requires-Dist: xarray-datatree; extra == 'dev'
 Requires-Dist: zarr; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: griffe-fieldz; extra == 'docs'
 Requires-Dist: mkdocs-material==9.5.17; extra == 'docs'
 Requires-Dist: mkdocs>=1.5.3; extra == 'docs'
 Requires-Dist: mkdocstrings-python==1.9.2; extra == 'docs'
 Requires-Dist: mkdocstrings==0.24.3; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: dask; extra == 'test'
 Requires-Dist: imageio; extra == 'test'
 Requires-Dist: jax[cpu]; extra == 'test'
+Requires-Dist: matplotlib; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: s3fs; extra == 'test'
 Requires-Dist: supabase; extra == 'test'
 Requires-Dist: tifffile; extra == 'test'
+Requires-Dist: torch; extra == 'test'
 Requires-Dist: xarray-datatree; extra == 'test'
 Requires-Dist: zarr; extra == 'test'
 Description-Content-Type: text/markdown
 
 # microsim
 
 [![License](https://img.shields.io/pypi/l/microsim.svg?color=green)](https://github.com/tlambert03/microsim/raw/main/LICENSE)
```

