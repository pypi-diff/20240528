# Comparing `tmp/lumicks.pylake-1.4.0.tar.gz` & `tmp/lumicks.pylake-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumicks.pylake-1.4.0.tar", last modified: Wed Feb 28 16:43:45 2024, max compression
+gzip compressed data, was "lumicks.pylake-1.5.0.tar", last modified: Tue May 28 17:50:23 2024, max compression
```

## Comparing `lumicks.pylake-1.4.0.tar` & `lumicks.pylake-1.5.0.tar`

### file list

```diff
@@ -1,322 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.783787 lumicks.pylake-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-02-28 16:43:45.783787 lumicks.pylake-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.735787 lumicks.pylake-1.4.0/lumicks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.743787 lumicks.pylake-1.4.0/lumicks/pylake/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/adjustments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.747787 lumicks.pylake-1.4.0/lumicks/pylake/detail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/bead_cropping.py
--rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/confocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/h5_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/imaging_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.747787 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.747787 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum0.npz
--rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum1.npz
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum2.npz
--rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum3.npz
--rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum4.npz
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum5.npz
--rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum6.npz
--rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum7.npz
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/test_bead_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/test_widefield.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/timeindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    25343 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/detail/widefield.py
--rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fdcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fdensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    15557 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/file_download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.747787 lumicks.pylake-1.4.0/lumicks/pylake/fitting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.751787 lumicks.pylake-1.4.0/lumicks/pylake/fitting/detail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/detail/derivative_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/detail/link_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    42415 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/detail/model_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/detail/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    29579 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/fitdata.py
--rw-r--r--   0 runner    (1001) docker     (127)    29383 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    35226 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/parameter_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    25485 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/profile_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.751787 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_condition_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_fd_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    26073 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_model_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_model_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_parameter_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_stderr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_stepping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.751787 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37305 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/calibration_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/convenience.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.755787 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/detail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/detail/drag_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/detail/driving_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/detail/hydrodynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/detail/power_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/detail/salty_water.py
--rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/power_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)    19165 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/power_spectrum_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.755787 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.755787 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    95740 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/data/reference_spectrum.npz
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_active_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_axial.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_camera_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_convenience.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_diode_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_driving_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    19096 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_hydro.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_power_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_power_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)    25654 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_simulations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_touchdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/touchdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    25972 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/image_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)    43587 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.759787 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.759787 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16087 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/denoising.py
--rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/gaussian_mle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/geometry_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/linalg_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/localization_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    44177 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/msd_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    21264 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/scoring_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/stitch.py
--rw-r--r--   0 runner    (1001) docker     (127)    19721 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/trace_line_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    81186 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/kymotrack.py
--rw-r--r--   0 runner    (1001) docker     (127)    27371 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/kymotracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/stitching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.763787 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.763787 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/csv_bad_format.csv
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/csv_unparseable.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/test_sequence.gb
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/test_sequence_corrupted.gb
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/tracks_v3.csv
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/tracks_v4.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.735787 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.763787 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_basic/
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_basic/output_image_1d.npz
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_basic/output_image_2d.npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.767787 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/1d_background.npz
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/1d_no_background.npz
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/2d_background.npz
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/2d_no_background.npz
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_denoise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.767787 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_geometry_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_image_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    61826 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_kymotrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_loc_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_stitching.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/marker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.767787 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/correlated_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.767787 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/detail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/detail/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/detail/undostack.py
--rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/image_editing.py
--rw-r--r--   0 runner    (1001) docker     (127)    38214 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/kymotracker_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/range_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.767787 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/test_fd_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/test_image_editing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/test_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/test_undostack.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/note.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.767787 lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/baseline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/piezo_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.767787 lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/tests/test_baseline.py
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/point_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.771787 lumicks.pylake-1.4.0/lumicks/pylake/population/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.771787 lumicks.pylake-1.4.0/lumicks/pylake/population/detail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/detail/fit_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/detail/hmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/detail/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/detail/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    55525 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/dwelltime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/hmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/mixture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.771787 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.771787 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    34952 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/data/exponential_data.npz
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/data/generate_exponential_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/data/generate_trace_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/data/trace_data.npz
--rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/test_dwelltimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/test_hmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/test_hmm_algos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/population/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/scalebar.py
--rw-r--r--   0 runner    (1001) docker     (127)    20041 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.771787 lumicks.pylake-1.4.0/lumicks/pylake/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/simulation/diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.771787 lumicks.pylake-1.4.0/lumicks/pylake/simulation/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/simulation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/simulation/tests/test_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.775787 lumicks.pylake-1.4.0/lumicks/pylake/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.775787 lumicks.pylake-1.4.0/lumicks/pylake/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/data/mock_confocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/data/mock_fdcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/data/mock_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/data/mock_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/data/mock_widefield.py
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/data/test_mock_confocal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.739787 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.779787 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/dict[1].npz
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/dict[2].npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/forced_filename_1.npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/forced_filename_2.npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/freezing[1].npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/freezing[2].npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/mytest[1].npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/mytest[2].npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/non_ndarray_matrix[1].npz
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/non_ndarray_matrix[2].npz
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/ragged[1].npz
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/ragged[2].npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.779787 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_channels/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_channels/test_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_fdcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_fdensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.779787 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_file/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_file/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_file/test_file_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_file_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.779787 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.779787 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/data/
--rw-r--r--   0 runner    (1001) docker     (127)    20460 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/data/tiff_from_scan_v1_3_1.tiff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.739787 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/reference_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.779787 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/reference_data/legacy_exposure_handling/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/reference_data/legacy_exposure_handling/dead_time[False].npz
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/reference_data/legacy_exposure_handling/dead_time[True].npz
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    50855 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.783787 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.783787 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/data/
--rw-r--r--   0 runner    (1001) docker     (127)   221862 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/data/bead_kymo.npz
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_downsampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_imagestack.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_slice_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_point_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)    15931 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_scan_slice_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_import_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_scalebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_timeindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/lumicks/pylake/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:43:45.739787 lumicks.pylake-1.4.0/lumicks.pylake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-02-28 16:43:45.000000 lumicks.pylake-1.4.0/lumicks.pylake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13415 2024-02-28 16:43:45.000000 lumicks.pylake-1.4.0/lumicks.pylake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 16:43:45.000000 lumicks.pylake-1.4.0/lumicks.pylake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 16:43:45.000000 lumicks.pylake-1.4.0/lumicks.pylake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-28 16:43:45.000000 lumicks.pylake-1.4.0/lumicks.pylake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-28 16:43:45.000000 lumicks.pylake-1.4.0/lumicks.pylake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-28 16:43:45.783787 lumicks.pylake-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/setup.manifest
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-28 16:43:25.000000 lumicks.pylake-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.363416 lumicks.pylake-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-28 17:50:23.363416 lumicks.pylake-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.311416 lumicks.pylake-1.5.0/lumicks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.319416 lumicks.pylake-1.5.0/lumicks/pylake/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/adjustments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.323416 lumicks.pylake-1.5.0/lumicks/pylake/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/bead_cropping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/confocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/h5_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11544 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/imaging_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.323416 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.323416 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum0.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum1.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum3.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum5.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum6.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum7.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/test_bead_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/test_widefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/timeindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27375 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/detail/widefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fdcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fdensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14770 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/file_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.327416 lumicks.pylake-1.5.0/lumicks/pylake/fitting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.327416 lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/derivative_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/link_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42415 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/model_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29579 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/fitdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29584 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35226 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/parameter_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25485 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/profile_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.327416 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_condition_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_fd_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26073 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_model_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_model_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_parameter_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_stderr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_stepping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.331416 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41587 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/calibration_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/convenience.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.331416 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/drag_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/driving_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/hydrodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/power_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/salty_water.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11214 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/power_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19623 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/power_spectrum_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.331416 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.335416 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95740 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/reference_spectrum.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.335416 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/1BGJQSPSHIFNM841G0X0WP2UL.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/3H9KBT8A28K43BCYEHIE0JD4L.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/5OF2DCE6DXL0LGPCPCPHOA3TH.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/7IJO3KH5G90URX2B9RYTYQKPG.json
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/999SUSJ01D14ZSRH7M58HWXHV.json
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/9M9JZPD6GZ6UA62TR9OG5MDUJ.json
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/ALYF6CK1Y54466J549VJ1BSJM.json
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/BCF825GIR11ZFL6ZQKN4D7K21.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/E45ZBFK5MYVRD1J9N8ITG6EQ4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/ref_data/E6JD3GX1S6X68LXWJED5VFZOJ.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_active_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_axial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_camera_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_diode_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_driving_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19093 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_hydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_power_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13499 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_power_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25575 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_touchdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/touchdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26193 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/image_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47726 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.335416 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.339416 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16087 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/denoising.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/gaussian_mle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/geometry_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/linalg_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/localization_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44177 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/msd_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21264 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/scoring_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/stitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19721 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/trace_line_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81248 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/kymotrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27371 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/kymotracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/stitching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.339416 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.343416 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/csv_bad_format.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/csv_unparseable.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/test_sequence.gb
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/test_sequence_corrupted.gb
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v4.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.343416 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/1d_background.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/1d_no_background.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/2d_background.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/2d_no_background.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/output_image_1d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/output_image_2d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_denoise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.343416 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_geometry_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_image_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61826 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_kymotrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_loc_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_stitching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/marker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.347416 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/correlated_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.347416 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/detail/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/detail/undostack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/image_editing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38089 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/kymotracker_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/range_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.347416 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_fd_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_image_editing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_undostack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/note.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.347416 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/piezo_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.347416 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/test_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/point_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.347416 lumicks.pylake-1.5.0/lumicks/pylake/population/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.351416 lumicks.pylake-1.5.0/lumicks/pylake/population/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/detail/fit_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/detail/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/detail/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/detail/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55527 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/dwelltime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/mixture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.351416 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.351416 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    34952 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/exponential_data.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/generate_exponential_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/generate_trace_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/trace_data.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_dwelltimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_hmm_algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/scalebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20262 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.351416 lumicks.pylake-1.5.0/lumicks/pylake/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/simulation/diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.351416 lumicks.pylake-1.5.0/lumicks/pylake/simulation/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/simulation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/simulation/tests/test_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.355416 lumicks.pylake-1.5.0/lumicks/pylake/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.355416 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_confocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_fdcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_widefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/data/test_mock_confocal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.359416 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/2MOF2FD1NDYBUVE5V2UV5OE5.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/49IRJMNKF3XEAQ6L2D38AFYC6.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/4RRE8ZG26TWBKKOUPK6CPFBIX.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/4TWTXTHAKH5N6BMWZI6KUMKK5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/5CBUUDH5DX4QNMKTT2J2B96GL.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/60TWXO09A93DLXSNN8B7QAIIT.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/60TWXO09A93DLXSNN8B7QAIIT.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/852E6XRLZFHJN2FQRJQPONQVA.json
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/9WDSTMR98ABMBPK6VPBYU3WFF.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/AELM9ISISBZJQ3AUKZIO6PZ7K.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/C1Z88G669DGF5HS3RX4OED5YL.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/C1Z88G669DGF5HS3RX4OED5YL.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/CMJN00XGRVG6SLMBMEJH8BKJK.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/EC0P3CT7JCJYDCD86TWKIQNGY.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/forced_filename_1.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/forced_filename_2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/ref_dict_freezing_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/ref_dict_freezing_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.359416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/test_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_fdcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_fdensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.359416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/test_file_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.359416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.359416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    20460 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/data/tiff_from_scan_v1_3_1.tiff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.359416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/ref_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/ref_data/21U0E1PWIF4T1V9BXHMY9P90F.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/ref_data/56OBGN66YAHPLZDQ8KXKGCI2P.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52907 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.363416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.363416 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   221862 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/data/bead_kymo.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_downsampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_imagestack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_slice_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_point_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15931 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_scan_slice_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_import_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_scalebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_timeindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/lumicks/pylake/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:50:23.319416 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-28 17:50:23.000000 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-05-28 17:50:23.000000 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:50:23.000000 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:50:23.000000 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 17:50:23.000000 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 17:50:23.000000 lumicks.pylake-1.5.0/lumicks.pylake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 17:50:23.363416 lumicks.pylake-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/setup.manifest
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-28 17:50:14.000000 lumicks.pylake-1.5.0/setup.py
```

### Comparing `lumicks.pylake-1.4.0/PKG-INFO` & `lumicks.pylake-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: lumicks.pylake
-Version: 1.4.0
+Version: 1.5.0
 Summary: Bluelake data analysis tools
 Home-page: https://github.com/lumicks/pylake
 Author: Lumicks B.V.
 Author-email: devteam@lumicks.com
 License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: notebook
 License-File: license.md
 
 <img src="https://media.githubusercontent.com/media/lumicks/pylake/main/docs/logo_light.png" alt="logo" width="489px"/>
 
 [![DOI](https://zenodo.org/badge/133832492.svg)](https://zenodo.org/badge/latestdoi/133832492)
@@ -44,9 +43,7 @@
 
 If you wish to publish results produced with this package, please mention the package name and cite the Zenodo DOI for this project:
 
 [![DOI](https://zenodo.org/badge/133832492.svg)](https://zenodo.org/badge/latestdoi/133832492)
 
 You'll find a *"Cite as"* section at the bottom right of the Zenodo page. You can select a citation
 style from the dropdown menu or export the data in BibTeX and similar formats.
-
-
```

### Comparing `lumicks.pylake-1.4.0/license.md` & `lumicks.pylake-1.5.0/license.md`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/__init__.py` & `lumicks.pylake-1.5.0/lumicks/pylake/__init__.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/adjustments.py` & `lumicks.pylake-1.5.0/lumicks/pylake/adjustments.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/benchmark.py` & `lumicks.pylake-1.5.0/lumicks/pylake/benchmark.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/calibration.py` & `lumicks.pylake-1.5.0/lumicks/pylake/calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/channel.py` & `lumicks.pylake-1.5.0/lumicks/pylake/channel.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/alignment.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/alignment.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/bead_cropping.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/bead_cropping.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/confocal.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/h5_helper.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/h5_helper.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/image.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/image.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/imaging_mixins.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/imaging_mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,38 +120,41 @@
         start_frame=None,
         stop_frame=None,
         fps=15,
         adjustment=no_adjustment,
         scale_bar=None,
         channel_slice=None,
         vertical=True,
+        downsample_to_frames=True,
         **kwargs,
     ):
         """Export a video
 
         Parameters
         ----------
         channel : str
             Color channel(s) to use "red", "green", "blue" or "rgb".
         file_name : str
             File name to export to.
         start_frame : int
-            First frame in exported video.
+            First frame in exported video (starts at zero).
         stop_frame : int
-            Last frame in exported video.
+            Stop frame in exported video. Note that this frame is no longer included.
         fps : int
             Frame rate.
         adjustment : lk.ColorAdjustment
             Color adjustments to apply to the output image.
         scale_bar : lk.ScaleBar
             Scale bar to add to the figure.
         channel_slice : lk.Slice, optional
             When specified, we export a video correlated to channel data
         vertical : bool, optional
             Render with the plots vertically aligned (default: True).
+        downsample_to_frames : bool, optional
+            Downsample the channel data over frame timestamp ranges (default: True).
         **kwargs
             Forwarded to :func:`matplotlib.pyplot.imshow`.
 
         Examples
         --------
         ::
 
@@ -202,31 +205,32 @@
         if "ffmpeg" in animation.writers:
             writer = animation.writers["ffmpeg"](fps=fps, metadata=metadata)
         elif "pillow" in animation.writers:
             writer = animation.writers["pillow"](fps=fps, metadata=metadata)
         else:
             raise RuntimeError("You need either ffmpeg or pillow installed to export videos.")
 
-        start_frame = start_frame if start_frame else 0
-        stop_frame = stop_frame if stop_frame else self.num_frames
+        start_frame = start_frame if start_frame is not None else 0
+        stop_frame = stop_frame if stop_frame is not None else self.num_frames
 
         shared_args = {"channel": channel, "adjustment": adjustment}
         if channel_slice:
             set_frame = self.plot_correlated(
                 **shared_args,
                 frame=start_frame,
                 channel_slice=channel_slice,
                 vertical=vertical,
                 return_frame_setter=True,
+                downsample_to_frames=downsample_to_frames,
             )
             fig = plt.gcf()  # plot_correlated makes its own plot
             fig.patch.set_alpha(1.0)  # Circumvents grainy rendering
 
             def plot(frame):
-                set_frame(frame)
+                set_frame(frame + start_frame)
                 artists = []
                 for ax in fig.get_children():
                     artists = ax.get_children()
                     if artists:
                         artists.extend(artists)
 
                 return artists
@@ -236,15 +240,15 @@
             fig.patch.set_alpha(1.0)  # Circumvents grainy rendering
             image_handle = None
 
             def plot(frame):
                 nonlocal image_handle
                 image_handle = self.plot(
                     **shared_args,
-                    frame=frame,
+                    frame=frame + start_frame,
                     image_handle=image_handle,
                     scale_bar=scale_bar,
                     **kwargs,
                 )
                 return plt.gca().get_children()
 
         # Don't store the FuncAnimation in a variable as this leads to mpl attempting to remove
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/mixin.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/mixin.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/plotting.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/plotting.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum0.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum0.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum1.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum1.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum2.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum2.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum3.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum3.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum4.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum4.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum5.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum5.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum6.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum6.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/data/kymo_sum7.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/data/kymo_sum7.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/test_bead_crop.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/test_bead_crop.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/test_plotting.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/tests/test_widefield.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/tests/test_widefield.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/timeindex.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/timeindex.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/utilities.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/detail/widefield.py` & `lumicks.pylake-1.5.0/lumicks/pylake/detail/widefield.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,34 +43,45 @@
         self._roi = roi
         self._tether = tether
 
     @property
     def _is_aligned(self):
         return self._description._alignment.is_aligned
 
+    def _normalize_array(self):
+        img = self._page.asarray()
+        if not self.is_rgb or img.shape[-1] == 3:
+            return img
+
+        # Handle two color images. We up-convert them to a 3-color image to be able to handle
+        # rgb-mappable images in a uniform manner.
+        three_colors = np.zeros((img.shape[0], img.shape[1], 3))
+        three_colors[:, :, self._description.channel_order] = img
+        return three_colors
+
     def _align_image(self):
         """reconstruct image using alignment matrices from Bluelake; return aligned image as a NumPy array"""
-        img = self._page.asarray()
+        img = self._normalize_array()
         for channel, mat in self._description._alignment_matrices.items():
             mat = self._tether.rot_matrix * mat
             img[:, :, channel] = mat.warp_image(img[:, :, channel])
         return img
 
     @property
     def data(self):
         data = (
             self._align_image()
             if self._description._alignment.do_alignment
-            else self._tether.rot_matrix.warp_image(self._page.asarray())
+            else self._tether.rot_matrix.warp_image(self._normalize_array())
         )
         return self._roi(data)
 
     @property
     def raw_data(self):
-        return self._roi(self._page.asarray())
+        return self._roi(self._normalize_array())
 
     @property
     def bit_depth(self):
         bit_depth = self._page.tags["BitsPerSample"].value
         if self.is_rgb:  # (int r, int g, int b)
             return bit_depth[0]
         else:  # int
@@ -307,14 +318,22 @@
         return np.sum(self._num_frames_per_tiff)
 
     def close(self):
         for file in self._tiff_files:
             file.close()
 
 
+def _parse_wavelength(wavelength_field):
+    """Parse excitation wavelength"""
+    try:
+        return float(wavelength_field.split("/")[0])  # Format is wavelength / width
+    except ValueError:
+        return
+
+
 class ImageDescription:
     """Wrapper around TIFF ImageDescription tag and other pylake specific metadata.
 
     Parameters
     ----------
     tiff_file : tifffile.TiffFile
         TIFF file recorded from a camera in Bluelake.
@@ -330,15 +349,15 @@
     json : dict
         dictionary of parsed json string held in frame ImageDescription tag.
     """
 
     def __init__(self, tiff_file, align_requested):
         first_page = tiff_file.pages[0]
         tags = first_page.tags
-        self.is_rgb = tags["SamplesPerPixel"].value == 3
+        self.is_rgb = tags["SamplesPerPixel"].value > 1
         self.width = tags["ImageWidth"].value
         self.height = tags["ImageLength"].value
         self.software = tags["Software"].value if "Software" in tags else ""
         self.pixelsize_um = None
         self._alignment_matrices = {}
 
         # parse json string stored in ImageDescription tag
@@ -360,21 +379,46 @@
 
         # update json fields if necessary
         if "Alignment red channel" in self.json:
             for j, color in enumerate(("red", "green", "blue")):
                 self.json[f"Channel {j} alignment"] = self.json.pop(f"Alignment {color} channel")
                 self.json[f"Channel {j} detection wavelength (nm)"] = "N/A"
 
-        if "Channel 0 alignment" in self.json:
-            self._alignment_matrices = {
-                channel: TransformMatrix.from_alignment(
-                    self._raw_alignment_matrix(channel), *self.offsets
-                ).invert()
-                for channel in range(3)
-            }
+        excitation_colors = [
+            key.split(" ")[0] for key in self.json.keys() if "Excitation Laser wavelength" in key
+        ]
+
+        self.channel_order = (0, 1, 2)
+        if len(excitation_colors) == 2:
+            self.channel_order = tuple(
+                ix
+                for ix, color in enumerate(("Red", "Green", "Blue"))
+                if color in excitation_colors
+            )
+
+        excitation_filter_wavelengths = [
+            _parse_wavelength(self.json[f"Channel {channel} detection wavelength (nm)"])
+            for channel in range(3)
+            if f"Channel {channel} detection wavelength (nm)" in self.json
+        ]
+
+        if excitation_filter_wavelengths and all(excitation_filter_wavelengths):
+            # Validate that the wavelengths are in ascending order
+            if not all(np.diff(excitation_filter_wavelengths) < 0):
+                raise RuntimeError(
+                    f"Wavelengths are not in descending order {excitation_filter_wavelengths}"
+                )
+
+        self._alignment_matrices = {
+            rgb_channel: TransformMatrix.from_alignment(
+                self._raw_alignment_matrix(channel), *self.offsets
+            ).invert()
+            for channel, rgb_channel in enumerate(self.channel_order)
+            if f"Channel {channel} alignment" in self.json
+        }
 
         # check alignment status
         if not self.is_rgb:
             self._alignment = Alignment(align_requested, AlignmentStatus.not_applicable, False)
         elif "Channel 0 alignment" in self.json.keys():
             self._alignment = Alignment(align_requested, AlignmentStatus.ready, align_requested)
         elif any([re.search(r"^Applied (.*)channel(.*)$", key) for key in self.json.keys()]):
@@ -448,15 +492,24 @@
         return np.array(self.json[f"Channel {index} alignment"]).reshape((2, 3))
 
     @property
     def for_export(self):
         out = copy(self.json)
         if self._alignment.do_alignment:
             for j in range(3):
-                out[f"Applied channel {j} alignment"] = out.pop(f"Channel {j} alignment")
+                if f"Channel {j} alignment" in out:
+                    out[f"Applied channel {j} alignment"] = out.pop(f"Channel {j} alignment")
+
+        # Add some Pylake specific metadata
+        out["Pylake"] = {
+            "Channel mapping": {
+                ("red", "green", "blue")[channel_idx]: idx
+                for idx, channel_idx in enumerate(self.channel_order)
+            }
+        }
         return out
 
 
 class AlignmentStatus(enum.Enum):
     empty = "File does not contain metadata. Only raw data is available"
     missing = "File does not contain alignment matrices. Only raw data is available"
     ready = "alignment is possible"
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fdcurve.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fdcurve.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fdensemble.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fdensemble.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/file.py` & `lumicks.pylake-1.5.0/lumicks/pylake/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -182,56 +182,35 @@
             )
 
         def print_force(field_name):
             field = getattr(self, field_name)
             calibration = "  .calibration\n" if field.calibration else ""
             return f".{field_name}\n{calibration}" if field else ""
 
+        rng = range(4)
+        axes = ("x", "y", "z")
+
         return (
             print_attributes(self.h5)
             + "\n"
             + print_group(self.h5)
             + "".join((print_dicts(field[0]) for field in self.redirect_list.values()))
             + "\n"
             + "".join(
                 (
                     print_force(field)
-                    for field in [
-                        "force1x",
-                        "force1y",
-                        "force1z",
-                        "force2x",
-                        "force2y",
-                        "force2z",
-                        "force3x",
-                        "force3y",
-                        "force3z",
-                        "force4x",
-                        "force4y",
-                        "force4z",
-                    ]
+                    for field in [f"force{channel + 1}{axis}" for channel in rng for axis in axes]
                 )
             )
             + "\n"
             + "".join(
                 (
                     print_force(field)
                     for field in [
-                        "downsampled_force1x",
-                        "downsampled_force1y",
-                        "downsampled_force1z",
-                        "downsampled_force2x",
-                        "downsampled_force2y",
-                        "downsampled_force2z",
-                        "downsampled_force3x",
-                        "downsampled_force3y",
-                        "downsampled_force3z",
-                        "downsampled_force4x",
-                        "downsampled_force4y",
-                        "downsampled_force4z",
+                        f"downsampled_force{channel + 1}{axis}" for channel in rng for axis in axes
                     ]
                 )
             )
         )
 
     def _get_force(self, n, xyz):
         """Return a Slice of force measurements, including calibration
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/file_download.py` & `lumicks.pylake-1.5.0/lumicks/pylake/file_download.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/datasets.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/datasets.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/detail/derivative_manipulation.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/derivative_manipulation.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/detail/link_functions.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/link_functions.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/detail/model_implementation.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/model_implementation.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/detail/utilities.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/detail/utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/fit.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/fit.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/fitdata.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/fitdata.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/model.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,17 @@
 
     def __call__(self, independent, params):
         """Evaluate the model for specific parameters
 
         Parameters
         ----------
         independent : array_like
-        params : lumicks.pylake.fitting.parameters.Params
+            Values for the independent parameter
+        params : Params | Dict[float | Parameter]
+            Model parameters
         """
         independent = np.asarray(independent, dtype=np.float64)
         missing_parameters = set(self.parameter_names) - set(params.keys())
         if missing_parameters:
             raise KeyError(
                 f"The following missing parameters must be specified to simulate the "
                 f"model: {missing_parameters}."
@@ -172,14 +174,17 @@
             independent,
             np.asarray([float(params[name]) for name in self.parameter_names], dtype=np.float64),
         )
 
     def _raw_call(self, independent, param_vector):
         return self.model_function(independent, *param_vector)
 
+    def __getitem__(self, item):
+        return self.defaults[item]
+
     def __add__(self, other):
         """
         Add two model outputs to form a new model.
 
         Parameters
         ----------
         other : pylake.fitting.Model
@@ -272,14 +277,15 @@
         param_name = (
             f"{self.name}/{self.independent}_offset" if self.independent else f"{self.name}/offset"
         )
         return SubtractIndependentOffset(self, self._independent_unit, param_name)
 
     @property
     def defaults(self):
+        """Default model parameters when added to an FdFit"""
         return self._params
 
     @property
     def parameter_names(self):
         return [x for x in self._params.keys()]
 
     def jacobian(self, independent, param_vector):
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/models.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/parameters.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,20 +86,22 @@
             return [self.value - dp, self.value + dp]
         else:
             raise RuntimeError("These parameters are not associated with a fitted model.")
 
 
 class Params:
     """
-    Model parameters. Internally stored as a list of Parameter.
+    Model parameters.
 
     Examples
     --------
     ::
-        fit = pylake.FdFit(pylake.ewlc_odijk_distance("my_model"))
+
+        import lumicks.pylake as lk
+        fit = lk.FdFit(lk.ewlc_odijk_distance("my_model"))
 
         print(fit.params)  # Prints the model parameters
         fit["test_parameter"].value = 5  # Set parameter test_parameter to 5
         fit["fix_me"].fixed = True  # Fix parameter fix_me (do not fit)
 
         # Copy parameters from another Parameters into this one.
         parameters.update_params(other_parameters)
@@ -206,17 +208,17 @@
 
         It mutates the parameter vector to contain the elements as specified in "parameters" with the defaults as
         specified in defaults. If the parameter already exists in the vector nothing happens to it. If it doesn't,
         it gets initialized to its default.
 
         Parameters
         ----------
-        params : list of str
+        params : List[str]
             parameter names
-        defaults : Parameter or None
+        defaults : List[Optional[Parameter]]
             default parameter objects
         """
         new_params = OrderedDict(
             zip(params, [x if isinstance(x, Parameter) else Parameter() for x in defaults])
         )
         for key, value in self._src.items():
             if key in new_params:
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/profile_likelihood.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/profile_likelihood.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_condition_handling.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_condition_handling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_fd_models.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_fd_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,7 +204,13 @@
 
     for param in ref_params.keys():
         np.testing.assert_allclose(params[param].value, ref_params[param])
 
     # The convenience part is in the parameters, with the old parameters they should produce the
     # exact same as what they are supposed to be based on
     np.testing.assert_allclose(model(x, params), ref_model("m")(x, params))
+
+
+def test_model_get_item():
+    m = ewlc_odijk_force("m")
+    m["m/Lc"].value = 3.1415
+    np.testing.assert_equal(float(m.defaults["m/Lc"]), 3.1415)
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_fit.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_model_composition.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_model_composition.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_model_sim.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_model_sim.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_parameters.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_pickling.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_profiles.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_stderr.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_stderr.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_stepping.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_stepping.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/fitting/tests/test_utilities.py` & `lumicks.pylake-1.5.0/lumicks/pylake/fitting/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/calibration_models.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/calibration_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     alias_spectrum,
     motion_blur_peak,
     motion_blur_spectrum,
     sphere_friction_coefficient,
     passive_power_spectrum_model,
     theoretical_driving_power_lorentzian,
 )
-from .detail.driving_input import driving_power_peak, estimate_driving_input_parameters
+from .detail.driving_input import DrivenPower, estimate_driving_input_parameters
 from .detail.hydrodynamics import (
+    calculate_complex_drag,
     passive_power_spectrum_model_hydro,
     theoretical_driving_power_hydrodynamics,
 )
 from .power_spectrum_calibration import CalibrationParameter
 
 
 def diode_params_from_voltage(
@@ -372,15 +373,15 @@
         force_slice = f.force1x
 
         # Decalibrate existing data
         volts = force_slice / force_slice.calibration[0]["Response (pN/V)"]
 
         power_spectrum = lk.calculate_power_spectrum(
             volts.data,
-            sample_rate=78125,
+            sample_rate=volts.sample_rate,
             excluded_ranges=[[4400, 4500]],  # Exclude a noise peak
             num_points_per_block=350,
         )
 
         model = lk.PassiveCalibrationModel(
             bead_diameter=4.89,
             temperature=25,
@@ -442,15 +443,16 @@
             if self.axial:
                 raise NotImplementedError(
                     "No hydrodynamically correct axial force model is currently available."
                 )
 
             # The hydrodynamically correct model already accounts for the effect of a nearby wall.
             # Here the drag coefficient in the model represents the bulk drag coefficient.
-            self._drag_correction_factor = 1
+            self._drag_correction_factor = 1.0
+
             # This model is only valid up to l/R < 1.5 [6] so throw in case that is violated.
             if (
                 distance_to_surface is not None
                 and distance_to_surface / (self.bead_diameter / 2) < 1.5
             ):
                 raise ValueError(
                     "The hydrodynamically correct model is only valid for distances to the surface "
@@ -460,32 +462,50 @@
 
             if rho_sample is not None and rho_sample < 100.0:
                 raise ValueError("Density of the sample cannot be below 100 kg/m^3")
 
             if rho_bead < 100.0:
                 raise ValueError("Density of the bead cannot be below 100 kg/m^3")
 
+            bead_radius_m = self.bead_diameter * 1e-6 / 2.0  # um diameter -> m radius
+            distance_to_surface_m = (
+                None if self.distance_to_surface is None else self.distance_to_surface * 1e-6
+            )  # um => m
+
+            # The hydrodynamic model is expressed as a function of drag in bulk. Therefore,
+            # to get the local drag, we have to forward-calculate it.
+            complex_drag = calculate_complex_drag(
+                f=0,
+                gamma0=1,
+                rho_sample=self.rho_sample,
+                bead_radius=bead_radius_m,
+                distance_to_surface=distance_to_surface_m,
+            )
+            self._to_local_drag_coefficient = complex_drag[0]
+
             self._passive_power_spectrum_model = partial(
                 passive_power_spectrum_model_hydro,
                 gamma0=self.drag_coeff,
-                bead_radius=self.bead_diameter * 1e-6 / 2.0,  # um diameter -> m radius
+                bead_radius=bead_radius_m,
                 rho_sample=self.rho_sample,
                 rho_bead=self.rho_bead,
-                distance_to_surface=None
-                if self.distance_to_surface is None
-                else self.distance_to_surface * 1e-6,  # um => m
+                distance_to_surface=distance_to_surface_m,
             )
         else:
+            # When performing active calibration with the simple models, the measured drag
+            # coefficient already corresponds to the value close to the surface.
+            self._to_local_drag_coefficient = 1.0
+
             if distance_to_surface:
                 args = (distance_to_surface * 1e-6, bead_diameter * 1e-6 / 2.0)
                 self._drag_correction_factor = (
                     brenner_axial(*args) if self.axial else faxen_factor(*args)
                 )
             else:
-                self._drag_correction_factor = 1
+                self._drag_correction_factor = 1.0
 
             self._passive_power_spectrum_model = passive_power_spectrum_model
 
     def _calculate_power_spectral_density(self, f, fc, diffusion_constant, *filter_params):
         physical_spectrum = self._passive_power_spectrum_model(f, fc, diffusion_constant)
         return physical_spectrum * self._filter(f, *filter_params)
 
@@ -625,24 +645,35 @@
         distance_response = (
             np.sqrt(scipy.constants.k * temperature_k / self._drag / diffusion_constant_volts) * 1e6
         )
 
         # Stiffness is output in pN/nm (N/m -> pN/nm or 1e12 / 1e9 = 1e3)
         kappa = 2 * np.pi * self._drag * fc * 1e3
 
+        # Determine errors by Gaussian Error Propagation (note that this neglects errors
+        # present in the drag due to imprecision in viscosity / temperature).
+        kappa_err = (kappa / fc) * fc_err
+        distance_response_err = (
+            distance_response / (2 * diffusion_constant_volts) * diffusion_constant_volts_err
+        )
+
         # Force response (Rf) is output in pN/V. Rd [um/V], stiffness [pN/nm]: um -> nm = 1e3
         force_response = distance_response * kappa * 1e3
 
         return {
             "Rd": CalibrationParameter("Distance response", distance_response, "um/V"),
             "kappa": CalibrationParameter("Trap stiffness", kappa, "pN/nm"),
             "Rf": CalibrationParameter("Force response", force_response, "pN/V"),
             self._drag_fieldname: CalibrationParameter(
                 self._drag_description, self.drag_coeff, "kg/s"
             ),
+            "err_kappa": CalibrationParameter("Stiffness Std Err", kappa_err, "pN/V"),
+            "err_Rd": CalibrationParameter(
+                "Distance response Std Err", distance_response_err, "um/V"
+            ),
             **self._format_passive_result(
                 fc,
                 diffusion_constant_volts,
                 filter_params,
                 fc_err,
                 diffusion_constant_volts_err,
                 filter_params_err,
@@ -677,17 +708,16 @@
     viscosity : float, optional
         Liquid viscosity [Pa*s].
         When omitted, the temperature will be used to look up the viscosity of water at that
         particular temperature.
     temperature : float, optional
         Liquid temperature [Celsius].
     num_windows : int, optional
-        Number of windows to average for the uncalibrated force. Using a larger number of
-        windows potentially increases spectral bleed from adjacent peaks, but may be useful when
-        the SNR is low.
+        Number of oscillations per window. Using a larger number of oscillations reduces the
+        spectral scalloping loss, but comes at the cost of SNR (due to less averaging taking place).
     hydrodynamically_correct : bool, optional
         Enable hydrodynamically correct model.
     distance_to_surface : float, optional
         Distance from bead center to the surface [um]
         When specifying `None`, the model will use an approximation which is only suitable for
         measurements performed deep in bulk.
     rho_sample : float, optional
@@ -750,24 +780,24 @@
         force_slice = f.force1x
 
         # Decalibrate existing data
         volts = force_slice / force_slice.calibration[0]["Response (pN/V)"]
 
         power_spectrum = lk.calculate_power_spectrum(
             volts.data,
-            sample_rate=78125,
+            sample_rate=volts.sample_rate,
             excluded_ranges=[[4400, 4500]],  # Exclude a noise peak
             num_points_per_block=350,
         )
 
         model = lk.ActiveCalibrationModel(
             f["Nanostage position"]["X"].data,  # Driving data
             volts.data,  # Position sensitive detector data
             temperature=25,
-            sample_rate=78125,
+            sample_rate=volts.sample_rate,
             bead_diameter=4.89,
             driving_frequency_guess=37,  # Have to provide a guess for the frequency
             hydrodynamically_correct=True,  # Big bead, so use hydrodynamic model
             distance_to_surface=10,  # Experiment performed 10 microns from surface
         )
 
         print(model.driving_frequency)  # Verify correct frequency determination
@@ -804,26 +834,27 @@
             rho_sample,
             rho_bead,
             fast_sensor,
             False,
         )
         self.driving_frequency_guess = driving_frequency_guess
         self.sample_rate = sample_rate
-        self.num_windows = num_windows
+        self.num_windows = num_windows  # TODO: misnamed parameter
         self._measured_drag_fieldname = "gamma_ex"
 
         # Estimate driving input and response
-        amplitude_um, self.driving_frequency = estimate_driving_input_parameters(
+        amplitude_um, self.driving_frequency, amplitude_um_std = estimate_driving_input_parameters(
             sample_rate, driving_data, driving_frequency_guess
         )
         self.driving_amplitude = amplitude_um * 1e-6
+        self._driving_amplitude_err = amplitude_um_std * 1e-6
 
         # The power density is the density (V^2/Hz) at the driving input. Multiplying this with
         # the frequency bin width gives the absolute power.
-        self._response_power_density, self._frequency_bin_width = driving_power_peak(
+        self.output_power = DrivenPower(
             force_voltage_data, sample_rate, self.driving_frequency, num_windows
         )
 
         if hydrodynamically_correct:
             self._theoretical_driving_power_model = partial(
                 theoretical_driving_power_hydrodynamics,
                 driving_frequency=self.driving_frequency,
@@ -845,15 +876,22 @@
 
     def calibration_parameters(self) -> dict:
         return {
             **super().calibration_parameters(),
             "Driving frequency (guess)": CalibrationParameter(
                 "Driving frequency (guess)", self.driving_frequency_guess, "Hz"
             ),
-            "num_windows": CalibrationParameter("Number of averaged windows", self.num_windows, ""),
+            "num_windows": CalibrationParameter(
+                "Number of oscillations per window", self.num_windows, ""
+            ),
+            "points_per_block_driving_power": CalibrationParameter(
+                "Points per block for driving power estimation",
+                self.output_power.ps.num_points_per_block,
+                "",
+            ),
         }
 
     def _theoretical_driving_power(self, f_corner):
         """Compute the power expected for a given driving input.
 
         When driving the stage or trap, we expect to see a delta spike in the power density
         spectrum. This function returns the expected power contribution of the bead motion to the
@@ -900,30 +938,64 @@
         diffusion_constant_volts_err : float
             Diffusion constant standard error, in Hz
         filter_params_err : list of float
             Standard errors for the filter model
         """
         import scipy.constants
 
-        reference_peak = self(self.driving_frequency, fc, diffusion_constant_volts, *filter_params)
+        thermal_noise = self(self.driving_frequency, fc, diffusion_constant_volts, *filter_params)
 
-        # Equation 14 from [6]
-        power_exp = (self._response_power_density - reference_peak) * self._frequency_bin_width
+        power_exp, power_exp_err = self.output_power.determine_power_output(thermal_noise)
+        power_theoretical = self._theoretical_driving_power(fc)
 
         # Equation 12 from [6]
-        distance_response = np.sqrt(self._theoretical_driving_power(fc) / power_exp)  # m/V
+        distance_response = np.sqrt(power_theoretical / power_exp)  # m/V
+
+        # dpower/dfc, dpower/dA in the limit driving_frequency->0 equates to
+        # -2/fc * power and 2/amplitude * power for both calibration models
+        dpower_fc = -(2 / fc) * power_theoretical
+        dpower_damp = (2 / self.driving_amplitude) * power_theoretical
+        power_theoretical_err = np.sqrt(
+            dpower_fc**2 * fc_err**2 + dpower_damp**2 * self._driving_amplitude_err**2
+        )
+
+        # Rd_err = sqrt((dRd/dPth)**2 * Pth_err**2 + (dRd/dPexp)**2+ Pexp_err**2)
+        dpower_dexp = -1 / (2 * power_exp)
+        dpower_dtheoretical = 1 / (2 * power_theoretical)
+        distance_response_err = (
+            np.sqrt(
+                dpower_dexp**2 * power_exp_err**2
+                + dpower_dtheoretical**2 * power_theoretical_err**2
+            )
+            * distance_response
+        )
 
         # Equation 16 from [6]
         temperature_kelvin = scipy.constants.convert_temperature(self.temperature, "C", "K")
         k_temperature = scipy.constants.k * temperature_kelvin
         measured_drag_coeff = k_temperature / (
             distance_response**2 * diffusion_constant_volts
         )  # kg/s
 
+        measured_drag_coeff_err = (
+            np.sqrt(
+                (-2 / distance_response) ** 2 * distance_response_err**2
+                + (-1 / diffusion_constant_volts) ** 2 * diffusion_constant_volts_err**2
+            )
+            * measured_drag_coeff
+        )
+
         kappa = 2.0 * np.pi * fc * measured_drag_coeff  # N/m
+        kappa_err = (
+            np.sqrt(
+                (1 / fc) ** 2 * fc_err**2
+                + (1 / measured_drag_coeff) ** 2 * measured_drag_coeff_err**2
+            )
+            * kappa
+        )
 
         force_response = distance_response * kappa  # N/V
 
         return {
             "Rd": CalibrationParameter("Distance response", distance_response * 1e6, "um/V"),
             "kappa": CalibrationParameter("Trap stiffness", kappa * 1e3, "pN/nm"),
             "Rf": CalibrationParameter("Force response", force_response * 1e12, "pN/V"),
@@ -931,14 +1003,19 @@
                 self._drag_description, self.drag_coeff, "kg/s"
             ),
             self._measured_drag_fieldname: CalibrationParameter(
                 "Measured bulk drag coefficient",
                 measured_drag_coeff / self._drag_correction_factor,
                 "kg/s",
             ),
+            "local_drag_coefficient": CalibrationParameter(
+                "Measured local drag coefficient",
+                measured_drag_coeff * self._to_local_drag_coefficient,
+                "kg/s",
+            ),
             "driving_amplitude": CalibrationParameter(
                 "Driving amplitude",
                 self.driving_amplitude * 1e6,
                 "um",
             ),
             "driving_frequency": CalibrationParameter(
                 "Driving frequency",
@@ -947,14 +1024,36 @@
             ),
             "driving_power": CalibrationParameter(
                 "Experimentally determined power in the spike observed on the positional power "
                 "spectrum",
                 power_exp,
                 "V^2",
             ),
+            "err_driving_power": CalibrationParameter(
+                "Experimentally determined power in the spike observed on the positional power "
+                "spectrum",
+                power_exp_err,
+                "V^2",
+            ),
+            "err_theoretical_power": CalibrationParameter(
+                "Experimentally determined power in the spike observed on the positional power "
+                "spectrum",
+                power_theoretical_err,
+                "V^2",
+            ),
+            "theoretical_power": CalibrationParameter(
+                "Theoretical determined power in the spike observed on the positional power "
+                "spectrum",
+                power_theoretical,
+                "V^2",
+            ),
+            "err_kappa": CalibrationParameter("Stiffness Std Err", kappa_err * 1e3, "pN/V"),
+            "err_Rd": CalibrationParameter(
+                "Distance response Std Err", distance_response_err * 1e6, "um/V"
+            ),
             **self._format_passive_result(
                 fc,
                 diffusion_constant_volts,
                 filter_params,
                 fc_err,
                 diffusion_constant_volts_err,
                 filter_params_err,
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/convenience.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/convenience.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,15 +92,18 @@
         fit. [Hz]
     num_points_per_block : int, optional
         The spectrum is first block averaged by this number of points per block.
         Default: 2000.
     excluded_ranges : list of tuple of float, optional
         List of ranges to exclude specified as a list of (frequency_min, frequency_max).
     drag : float, optional
-        Overrides the drag coefficient to this particular value.
+        Overrides the drag coefficient to this particular value. Note that you want to use the
+        bulk drag coefficient for this (obtained from the field `gamma_ex`). This can be used to
+        carry over an estimate of the drag coefficient obtained using an active calibration
+        procedure.
     fixed_diode : float, optional
         Fix diode frequency to a particular frequency.
     fixed_alpha : float, optional
         Fix diode relaxation factor to particular value.
 
     Raises
     ------
@@ -146,33 +149,35 @@
         f = lk.File("calibration_file.h5")
         force_slice = f.force1x
 
         # Decalibrate existing data
         volts = force_slice / force_slice.calibration[0]["Response (pN/V)"]
 
         # Determine calibration factors using the viscosity of water at T=25 C.
-        lk.calibrate_force(volts.data, bead_diameter=0.58, temperature=25, sample_rate=78125)
+        lk.calibrate_force(
+            volts.data, bead_diameter=0.58, temperature=25, sample_rate=volts.sample_rate
+        )
 
         # Determine calibration factors using the hydrodynamically correct model
         lk.calibrate_force(
             volts.data,
             bead_diameter=4.89,
             temperature=25,
-            sample_rate=78125,
+            sample_rate=volts.sample_rate,
             hydrodynamically_correct=True
         )
 
         # Determine calibration factors using the hydrodynamically correct model with active
         # calibration at a distance of 7 micron from the surface
         driving_data = f["Nanostage position"]["X"]
         lk.calibrate_force(
             volts.data,
             bead_diameter=4.89,
             temperature=25,
-            sample_rate=78125,
+            sample_rate=volts.sample_rate,
             hydrodynamically_correct=True,
             distance_to_surface=7,
             driving_data=driving_data.data,
             driving_frequency_guess=37,
             active_calibration=True
         )
     """
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/detail/drag_models.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/drag_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/detail/hydrodynamics.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/hydrodynamics.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         Frequency [Hz]
     gamma0 : float
         Drag coefficient [m Pa s]
     bead_radius : float
         Bead radius [m]
     rho_sample : float
         Sample mass density [kg/m^3]
-    distance_to_surface : float
+    distance_to_surface : float | None
         Distance from bead center to nearest surface [m]
     """
     # frequency_nu is the frequency at which the penetration depth in the liquid of the
     # bead’s linear harmonic motion equals the radius of the bead. It parametrizes the
     # flow pattern established around a sphere undergoing linear harmonic oscillations in
     # an incompressible fluid and it is unrelated to the mass of particle.
     #
@@ -135,15 +135,15 @@
         Drag coefficient, in m Pa s.
     bead_radius : float
         Bead radius, in m.
     rho_sample : float
         Sample mass density, in kg/m^3
     rho_bead : float
         Bead mass density, in kg/m^3
-    distance_to_surface : float
+    distance_to_surface : float | None
         Distance to nearest surface, in m
     """
     re_drag, im_drag = calculate_complex_drag(
         f, gamma0, rho_sample, bead_radius, distance_to_surface
     )
     frequency_m = calculate_dissipation_frequency(gamma0, bead_radius, rho_bead)
     denominator = (fc + f * (im_drag - f / frequency_m)) ** 2 + (f * re_drag) ** 2
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/detail/power_models.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/power_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/detail/salty_water.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/detail/salty_water.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/power_spectrum.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/power_spectrum.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,21 @@
         """
         if window_seconds is not None and window_seconds <= 0:
             raise ValueError("window_seconds must be positive")
 
         def squared_fft(d):
             return np.square(np.abs(np.fft.rfft(d)))
 
+        data = np.asarray(data)
+        if data.ndim != 1:
+            raise ValueError(
+                f"Only 1D arrays of data are supported. You provided a {data.ndim}D array of "
+                f"shape {data.shape}."
+            )
+
         self.unit = unit
         data = data - np.mean(data)
 
         # Calculate power spectrum for slices of data.
         num_points_per_window = (
             int(np.round(window_seconds * sample_rate)) if window_seconds else len(data)
         )
@@ -57,18 +64,27 @@
 
         squared_fft_chunks = [
             squared_fft(
                 data[chunk_idx * num_points_per_window : (chunk_idx + 1) * num_points_per_window]
             )
             for chunk_idx in np.arange(len(data) // num_points_per_window)
         ]
+
         squared_fft = np.mean(squared_fft_chunks, axis=0)
 
         self.frequency = np.fft.rfftfreq(num_points_per_window, 1.0 / sample_rate)
-        self.power = (2.0 / sample_rate) * squared_fft / num_points_per_window
+        scaling_factor = (2.0 / sample_rate) / num_points_per_window
+        self.power = scaling_factor * squared_fft
+
+        # Store a variance for temporally blocked power spectra
+        self._variance = (
+            scaling_factor**2 * np.var(squared_fft_chunks, axis=0)
+            if len(squared_fft_chunks) > 1
+            else None
+        )
 
         # Store metadata
         self.sample_rate = sample_rate
         self.total_duration = data.size / sample_rate
         self.num_points_per_block = len(squared_fft_chunks)
         self.total_sampled_used = num_points_per_window * self.num_points_per_block
 
@@ -79,14 +95,15 @@
 
     def downsampled_by(self, factor, reduce=np.mean) -> "PowerSpectrum":
         """Returns a spectrum downsampled by a given factor."""
         ba = copy(self)
         ba.frequency = downsample(self.frequency, factor, reduce)
         ba.power = downsample(self.power, factor, reduce)
         ba.num_points_per_block = self.num_points_per_block * factor
+        ba._variance = None  # Not supported
 
         return ba
 
     def _exclude_range(self, excluded_ranges) -> "PowerSpectrum":
         """Exclude given frequency ranges from the power spectrum.
 
         This function can be used to exclude noise peaks.
@@ -101,14 +118,18 @@
         ps = copy(self)
         indices = np.logical_and.reduce(
             [(ps.frequency < f_min) | (ps.frequency >= f_max) for f_min, f_max in excluded_ranges]
         )
 
         ps.frequency = ps.frequency[indices]
         ps.power = ps.power[indices]
+
+        if self._variance is not None:
+            ps._variance = ps._variance[indices]
+
         return ps
 
     def identify_peaks(
         self,
         model_fun: callable,
         *,
         peak_cutoff: float = 20.0,
@@ -119,19 +140,18 @@
         windowed. This is beta functionality. While usable, this has not yet been tested in a large
         number of different scenarios. The API can still be subject to change without any prior
         deprecation notice! If you use this functionality keep a close eye on the changelog for any
         changes that may affect your analysis.
 
         Parameters
         ----------
-        power_spectrum : PowerSpectrum
-            The power spectrum of the Brownian motion of the bead in a trap
         model_fun : callable
             A function of one argument, frequency, that gives the theoretical power spectrum. The
-            function is used to normalize the experimental power spectrum
+            function is used to normalize the experimental power spectrum. Note that you can
+            pass an instance of `CalibrationResults`.
         peak_cutoff: float
             Indicates what value of the normalized spectrum is deemed abnormally high. Default is
             20.0, which corresponds to a chance of about 2 in 1E9 that a peak of that magnitude
             occurs naturally in an exponential distribution with rate parameter = 1.0. The minimum
             is baseline (see below).
         baseline: float
             The baseline level a peak needs to drop down to. Lower means that exponentially more
@@ -184,15 +204,16 @@
         peak_ranges = grab_contiguous_ranges(peak_mask)
 
         if not peak_ranges.size:
             return []
 
         baseline_ranges = grab_contiguous_ranges(baseline_mask)
 
-        # Find start points of baseline sections (int because derivative can be negative, and bool doesn't allow that).
+        # Find start points of baseline sections (int because derivative can be negative, and bool
+        # doesn't allow that).
         start_points = np.diff(baseline_mask, prepend=0) > 0
 
         # This allows us to look up which baseline range to grab
         baseline_indices = np.cumsum(start_points) - 1
 
         # Any point inside the peak range will do to identify the baseline range
         exclusion_baseline_indices = [
@@ -208,28 +229,34 @@
 
     def in_range(self, frequency_min, frequency_max) -> "PowerSpectrum":
         """Returns part of the power spectrum within a given frequency range."""
         ir = copy(self)
         mask = (self.frequency > frequency_min) & (self.frequency <= frequency_max)
         ir.frequency = self.frequency[mask]
         ir.power = self.power[mask]
+
+        if self._variance is not None:
+            ir._variance = self._variance[mask]
+
         return ir
 
     def num_samples(self) -> int:
         return self.frequency.size
 
-    def with_spectrum(self, power, num_points_per_block=1) -> "PowerSpectrum":
+    def with_spectrum(self, power, num_points_per_block=1, variance=None) -> "PowerSpectrum":
         """Return a copy with a different spectrum
 
         Parameters
         ----------
         power : numpy.ndarray
             Vector of power spectral values
         num_points_per_block : int
             Number of points per block used to obtain power spectral values.
+        variance : numpy.ndarray, optional
+            Variance of the power spectrum.
 
         Returns
         -------
         power_spectrum : PowerSpectrum
             Power spectrum with new spectral density values.
 
         Raises
@@ -239,14 +266,15 @@
         """
         if len(power) != len(self.power):
             raise ValueError("New power spectral density vector has incorrect length")
 
         ps = copy(self)
         ps.power = power
         ps.num_points_per_block = num_points_per_block
+        ps._variance = variance
 
         return ps
 
     def plot(self, **kwargs):
         """Plot power spectrum
 
         Parameters
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/power_spectrum_calibration.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/power_spectrum_calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,29 +55,42 @@
         Power spectrum of the fitted model.
     ps_data : PowerSpectrum
         Power spectrum of the data that the model was fitted to.
     params : dict
         Dictionary of input parameters.
     results : dict
         Dictionary of calibration results.
+    fitted_params : np.ndarray
+        Fitted parameters.
     """
 
-    def __init__(self, model, ps_model, ps_data, params, results):
+    def __init__(self, model, ps_model, ps_data, params, results, fitted_params):
         self.model = model
         self.ps_model = ps_model
         self.ps_data = ps_data
         self.params = params
         self.results = results
+        self.fitted_params = fitted_params
 
         # A few parameters have to be present for this calibration to be used.
         mandatory_params = ["kappa", "Rf"]
         for key in mandatory_params:
             if key not in results:
                 raise RuntimeError(f"Calibration did not provide calibration parameter {key}")
 
+    def __call__(self, frequency):
+        """Evaluate the spectral model for one or more frequencies
+
+        Parameters
+        ----------
+        frequency : array_like
+            One or more frequencies at which to evaluate the spectral model.
+        """
+        return self.model(frequency, *self.fitted_params)
+
     def __contains__(self, key):
         return key in self.params or key in self.results
 
     def __getitem__(self, item):
         return self.params[item] if item in self.params else self.results[item]
 
     def plot(self):
@@ -399,15 +412,15 @@
         max_function_evals=max_function_evals,
         loss_function=loss_function,
     )
 
     # Calculate goodness-of-fit, in terms of the statistical backing (see ref. 1).
     n_degrees_of_freedom = power_spectrum.power.size - len(solution_params)
     chi_squared_per_deg = chi_squared / n_degrees_of_freedom
-    backing = (1 - scipy.special.gammainc(chi_squared / 2, n_degrees_of_freedom / 2)) * 100
+    backing = scipy.stats.chi2.sf(chi_squared, n_degrees_of_freedom) * 100
 
     # Fitted power spectrum values.
     ps_model = power_spectrum.with_spectrum(
         model(power_spectrum.frequency, *solution_params), power_spectrum.num_points_per_block
     )
 
     # When using theoretical weights for fitting, ref [5] mentions that the found value for D will
@@ -448,8 +461,9 @@
             "Bias correction": CalibrationParameter(
                 "Perform bias correction thermal fit", bias_correction, ""
             ),
             "Loss function": CalibrationParameter(
                 "Loss function used during minimization", loss_function, ""
             ),
         },
+        fitted_params=solution_params,
     )
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/conftest.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 import pytest
 
+from .data.simulate_calibration_data import generate_active_calibration_test_data
+
 
 class ReferenceModels:
     @staticmethod
     def lorentzian(f, fc, diffusion_constant):
         # Lorentzian in V^2/Hz
         return diffusion_constant / (np.pi**2) / (fc**2 + f**2)
 
@@ -63,7 +65,41 @@
             0.22333743993836863,
             -0.33331150250090585,
             0.1035148152731559,
         ],
         "focal_shift": 0.921283446497108,
         "nonlinear_shift": 0.0,
     }
+
+
+@pytest.fixture(scope="session")
+def active_calibration_surface_data():
+    shared_pars = {
+        "bead_diameter": 1.03,
+        "viscosity": 1.1e-3,
+        "temperature": 25,
+        "rho_sample": 997.0,
+        "rho_bead": 1040.0,
+        "distance_to_surface": 1.03 / 2 + 500e-3,
+    }
+
+    sim_pars = {
+        "sample_rate": 78125,
+        "stiffness": 0.1,
+        "pos_response_um_volt": 0.618,
+        "driving_sinusoid": (500, 31.95633),
+        "diode": (0.4, 15000),
+    }
+
+    np.random.seed(10071985)
+    volts, stage = generate_active_calibration_test_data(
+        10, hydrodynamically_correct=True, **sim_pars, **shared_pars
+    )
+
+    active_pars = {
+        "force_voltage_data": volts,
+        "driving_data": stage,
+        "sample_rate": 78125,
+        "driving_frequency_guess": 32,
+    }
+
+    return shared_pars, sim_pars, active_pars
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/data/reference_spectrum.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/reference_spectrum.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_active_calibration.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_active_calibration.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import numpy as np
 import scipy
 import pytest
 
 from lumicks.pylake.force_calibration.calibration_models import ActiveCalibrationModel
+from lumicks.pylake.force_calibration.detail.drag_models import faxen_factor
 from lumicks.pylake.force_calibration.detail.power_models import sphere_friction_coefficient
 from lumicks.pylake.force_calibration.power_spectrum_calibration import (
     fit_power_spectrum,
     calculate_power_spectrum,
 )
 
 from .data.simulate_calibration_data import generate_active_calibration_test_data
 
 
 @pytest.mark.parametrize(
     "stiffness, viscosity, temperature, pos_response_um_volt, driving_sinusoid, diode, driving_"
-    "frequency_guess, power_density, response_power",
+    "frequency_guess",
     [
-        [0.1, 1.002e-3, 20, 0.618, (500, 31.95633), (0.4, 15000), 32, 1.958068e-5, 0.000124879648],
-        [0.2, 1.012e-3, 20, 1.618, (500, 31.95633), (0.4, 14000), 32, 7.28664e-07, 4.64730000e-06],
-        [0.3, 1.002e-3, 50, 1.618, (300, 30.42633), (0.4, 16000), 29, 1.098337e-07, 6.63921666e-07],
+        [0.1, 1.002e-3, 20, 0.618, (500, 31.95633), (0.4, 15000), 32],
+        [0.2, 1.012e-3, 20, 1.618, (500, 31.95633), (0.4, 14000), 32],
+        [0.3, 1.002e-3, 50, 1.618, (300, 30.42633), (0.4, 16000), 29],
     ],
 )
 def test_integration_active_calibration(
+    compare_to_reference_dict,
     stiffness,
     viscosity,
     temperature,
     pos_response_um_volt,
     driving_sinusoid,
     diode,
     driving_frequency_guess,
-    power_density,
-    response_power,
 ):
     import scipy.constants
 
     """Functional end to end test for active calibration"""
     sample_rate, bead_diameter = 78125, 1.03
     np.random.seed(0)
     force_voltage_data, driving_data = generate_active_calibration_test_data(
@@ -59,19 +59,14 @@
         temperature,
     )
 
     # Validate estimation of the driving input
     np.testing.assert_allclose(model.driving_amplitude, driving_sinusoid[0] * 1e-9, rtol=1e-5)
     np.testing.assert_allclose(model.driving_frequency, driving_sinusoid[1], rtol=1e-5)
 
-    np.testing.assert_allclose(model._response_power_density, power_density, rtol=1e-5)
-    num_points_per_window = int(np.round(sample_rate * model.num_windows / model.driving_frequency))
-    freq_axis = np.fft.rfftfreq(num_points_per_window, 1.0 / sample_rate)
-    np.testing.assert_allclose(model._frequency_bin_width, freq_axis[1] - freq_axis[0])
-
     power_spectrum = calculate_power_spectrum(force_voltage_data, sample_rate)
     fit = fit_power_spectrum(power_spectrum, model)
 
     np.testing.assert_allclose(fit["kappa"].value, stiffness, rtol=5e-2)
     np.testing.assert_allclose(fit["alpha"].value, diode[0], rtol=5e-2)
     np.testing.assert_allclose(fit["f_diode"].value, diode[1], rtol=5e-2)
     np.testing.assert_allclose(fit["Rd"].value, pos_response_um_volt, rtol=5e-2)
@@ -83,26 +78,42 @@
     drag_coeff_calc = kt / (fit["D"].value * fit["Rd"].value ** 2)
     np.testing.assert_allclose(
         fit["gamma_0"].value,
         sphere_friction_coefficient(viscosity, bead_diameter * 1e-6),
         rtol=1e-9,
     )
     np.testing.assert_allclose(fit["gamma_ex"].value, drag_coeff_calc * 1e12, rtol=1e-9)
+    np.testing.assert_allclose(
+        fit["local_drag_coefficient"].value, drag_coeff_calc * 1e12, rtol=1e-9
+    )
 
     np.testing.assert_allclose(fit["Bead diameter"].value, bead_diameter)
     np.testing.assert_allclose(fit["Driving frequency (guess)"].value, driving_frequency_guess)
     np.testing.assert_allclose(fit["Sample rate"].value, sample_rate)
     np.testing.assert_allclose(fit["Viscosity"].value, viscosity)
     np.testing.assert_allclose(fit["num_windows"].value, 5)
 
     np.testing.assert_allclose(
         fit["driving_amplitude"].value, driving_sinusoid[0] * 1e-3, rtol=1e-5
     )
     np.testing.assert_allclose(fit["driving_frequency"].value, driving_sinusoid[1], rtol=1e-5)
-    np.testing.assert_allclose(fit["driving_power"].value, response_power, rtol=1e-6)
+
+    compare_to_reference_dict(
+        {
+            par: fit[par].value
+            for par in (
+                "driving_power",
+                "err_driving_power",
+                "err_theoretical_power",
+                "theoretical_power",
+                "err_kappa",
+                "err_Rd",
+            )
+        }
+    )
 
 
 def test_bias_correction():
     """Functional end to end test for active calibration"""
 
     np.random.seed(0)
     force_voltage_data, driving_data = generate_active_calibration_test_data(
@@ -146,67 +157,79 @@
         for fit, value in zip([fit_biased, fit_debiased], values):
             np.testing.assert_allclose(fit[key].value, value)
 
     assert fit_biased.params["Bias correction"].value is False
     assert fit_debiased.params["Bias correction"].value is True
 
 
-def test_faxen_correction_active():
+def test_faxen_correction_active(active_calibration_surface_data):
     """Active calibration should barely be affected by surface corrections for the drag coefficient.
     However, the interpretation of gamma_ex, which may be carried over to the other calibration
     *is* important, so this should be covered by a specific test."""
-    shared_pars = {
-        "bead_diameter": 1.03,
-        "viscosity": 1.1e-3,
-        "temperature": 25,
-        "rho_sample": 997.0,
-        "rho_bead": 1040.0,
-        "distance_to_surface": 1.03 / 2 + 500e-3,
-    }
-    sim_pars = {
-        "sample_rate": 78125,
-        "stiffness": 0.1,
-        "pos_response_um_volt": 0.618,
-        "driving_sinusoid": (500, 31.95633),
-        "diode": (0.4, 15000),
-    }
-
-    np.random.seed(10071985)
-    volts, stage = generate_active_calibration_test_data(
-        10, hydrodynamically_correct=True, **sim_pars, **shared_pars
-    )
-    power_spectrum = calculate_power_spectrum(volts, sim_pars["sample_rate"])
-
-    active_pars = {
-        "force_voltage_data": volts,
-        "driving_data": stage,
-        "sample_rate": 78125,
-        "driving_frequency_guess": 32,
-        "hydrodynamically_correct": False,
-    }
+    shared_pars, sim_pars, active_pars = active_calibration_surface_data
+    power_spectrum = calculate_power_spectrum(
+        active_pars["force_voltage_data"], sim_pars["sample_rate"]
+    )
 
-    model = ActiveCalibrationModel(**active_pars, **shared_pars)
+    model = ActiveCalibrationModel(**active_pars, **shared_pars, hydrodynamically_correct=False)
     fit = fit_power_spectrum(power_spectrum, model, bias_correction=False)
 
     # Fitting with *no* hydrodynamically correct model, but *with* Faxen's law
     np.testing.assert_allclose(fit.results["Rd"].value, 0.5979577465734786)
     np.testing.assert_allclose(fit.results["kappa"].value, 0.10852140970454485)
     np.testing.assert_allclose(fit.results["Rf"].value, 64.89121760190687)
     # gamma_0 and gamma_ex should be the same, since gamma_ex is corrected to be "in bulk".
     np.testing.assert_allclose(fit.results["gamma_0"].value, 1.0678273429551705e-08)
     np.testing.assert_allclose(fit.results["gamma_ex"].value, 1.1271667835127709e-08)
+    np.testing.assert_allclose(
+        fit.results["local_drag_coefficient"].value,
+        1.1271667835127709e-08
+        * faxen_factor(shared_pars["distance_to_surface"], shared_pars["bead_diameter"] / 2),
+    )
 
     # Disabling Faxen's correction on the drag makes the estimates *much* worse
-    shared_pars["distance_to_surface"] = None
-    model = ActiveCalibrationModel(**active_pars, **shared_pars)
+    model = ActiveCalibrationModel(
+        **active_pars, **dict(shared_pars, distance_to_surface=None), hydrodynamically_correct=False
+    )
     fit = fit_power_spectrum(power_spectrum, model, bias_correction=False)
 
     np.testing.assert_allclose(fit.results["Rd"].value, 0.5979577465734786)
     np.testing.assert_allclose(fit.results["kappa"].value, 0.10852140970454485)
     np.testing.assert_allclose(fit.results["Rf"].value, 64.89121760190687)
     # Not affected since this is gamma bulk
     np.testing.assert_allclose(fit.results["gamma_0"].value, 1.0678273429551705e-08)
     # The drag is now much different, since we're not using Faxen's law to back-correct the drag
     # to its actual bulk value.
     np.testing.assert_allclose(
         fit.results[model._measured_drag_fieldname].value, 1.571688034506783e-08
     )
+    # The local estimate is now the same.
+    np.testing.assert_allclose(fit.results["local_drag_coefficient"].value, 1.571688034506783e-08)
+
+
+def test_hydro_active(active_calibration_surface_data):
+    shared_pars, sim_pars, active_pars = active_calibration_surface_data
+    power_spectrum = calculate_power_spectrum(
+        active_pars["force_voltage_data"], sim_pars["sample_rate"]
+    )
+    model = ActiveCalibrationModel(**active_pars, **shared_pars, hydrodynamically_correct=True)
+    fit = fit_power_spectrum(power_spectrum, model, bias_correction=False)
+
+    np.testing.assert_allclose(fit.results["Rd"].value, 0.6093861540574103)
+    np.testing.assert_allclose(fit.results["gamma_0"].value, 1.0678273429551705e-08)
+    # Note proximity to gamma_0
+    gamma_ex = fit.results["gamma_ex"].value
+    np.testing.assert_allclose(gamma_ex, 1.0984573910537512e-08)
+    np.testing.assert_allclose(fit.results["local_drag_coefficient"].value, 1.537177770849885e-08)
+    np.testing.assert_allclose(
+        fit.results["local_drag_coefficient"].value,
+        gamma_ex
+        / (1 - (9 / 16) * 0.5 * shared_pars["bead_diameter"] / shared_pars["distance_to_surface"]),
+    )
+
+    model = ActiveCalibrationModel(
+        **active_pars, **dict(shared_pars, distance_to_surface=None), hydrodynamically_correct=True
+    )
+    fit = fit_power_spectrum(power_spectrum, model, bias_correction=False)
+    # No way to correct back to bulk without a height
+    np.testing.assert_allclose(fit.results["gamma_ex"].value, 1.6258510187033216e-08)
+    np.testing.assert_allclose(fit.results["local_drag_coefficient"].value, 1.6258510187033216e-08)
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_axial.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_axial.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_camera_calibration.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_camera_calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_convenience.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_convenience.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_diode_models.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_diode_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 )
 def test_fixed_f_diode(model_params, fixed_params, free_params, reference_models):
     """Test fixed diode model"""
     models, power_spectrum = model_and_data(reference_models, diode_alpha=0.4, fast_sensor=False)
     for model in models:
         model._filter = FixedDiodeModel(**model_params)
         fit = fit_power_spectrum(power_spectrum, model=model, bias_correction=False)
+        np.testing.assert_allclose(fit(fit.ps_model.frequency), fit.ps_model.power)
+        ref_params = [fit[p].value for p in ("fc", "D", "f_diode", "alpha") if p in fit.results]
+        np.testing.assert_allclose(fit.fitted_params, ref_params)
 
         # Test good fit
         np.testing.assert_allclose(fit.results["fc"].value, 4000, 1e-6)
         np.testing.assert_allclose(fit.results["D"].value, 1.14632, 1e-6)
         for key, value in free_params.items():
             np.testing.assert_allclose(fit.results[key].value, value, 1e-6)
 
@@ -80,14 +83,17 @@
 
         # Fix to the wrong value (this should mess up the fit)
         bad_params = deepcopy(model_params)
         for key in bad_params:
             bad_params[key] *= 1.1
         model._filter = FixedDiodeModel(**bad_params)
         fit = fit_power_spectrum(power_spectrum, model=model, bias_correction=False)
+        np.testing.assert_allclose(fit(fit.ps_model.frequency), fit.ps_model.power)
+        ref_params = [fit[p].value for p in ("fc", "D", "f_diode", "alpha") if p in fit.results]
+        np.testing.assert_allclose(fit.fitted_params, ref_params)
         assert abs(fit.results["fc"].value - 4000) > 1.0
         assert abs(fit.results["D"].value - 1.14632) > 1e-2
 
 
 def test_alpha_validity():
     # Alpha should be between 0 and 1
     for good_alpha in (0.0, 0.5, 1.0):
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_hydro.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_hydro.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,15 @@
         "err_fc": 13.075876724291339,
         "err_D": 0.0066021439072302835,
         "f_diode": 14675.638696737586,
         "alpha": 0.41651098052983593,
         "err_f_diode": 352.2917702189488,
         "err_alpha": 0.014231238753589254,
         "chi_squared_per_deg": 0.8659867914094764,
-        "backing": 14.340689726784328,
+        "backing": 84.05224555962526,
     }
 
     for key, value in expected_params.items():
         np.testing.assert_allclose(fit.params[key].value, value, err_msg=key)
 
     for key, value in expected_results.items():
         np.testing.assert_allclose(fit.results[key].value, value, err_msg=key)
@@ -344,15 +344,15 @@
         "err_fc": 13.075876724291339,
         "err_D": 0.0066021439072302835,
         "f_diode": 14675.638696737586,
         "alpha": 0.41651098052983593,
         "err_f_diode": 352.2917702189488,
         "err_alpha": 0.014231238753589254,
         "chi_squared_per_deg": 0.8659867914094764,
-        "backing": 14.340689726784328,
+        "backing": 84.05224555962526,
     }
 
     for key, value in expected_params.items():
         np.testing.assert_allclose(fit.params[key].value, value, err_msg=key)
 
     for key, value in expected_results.items():
         np.testing.assert_allclose(fit.results[key].value, value, err_msg=key)
@@ -398,15 +398,15 @@
         "f_diode": 14669.862556235465,
         "alpha": 0.41657472149713015,
         "err_fc": 11.599562805624199,
         "err_D": 0.007332334985757522,
         "err_f_diode": 376.8360414675165,
         "err_alpha": 0.014653541838852356,
         "chi_squared_per_deg": 0.8692145118092963,
-        "backing": 14.917612794899505,
+        "backing": 83.40493086075664,
     }
 
     assert fit.params["Distance to surface"].value is None
     for key, value in expected_params.items():
         np.testing.assert_allclose(fit.params[key].value, value, err_msg=key)
 
     for key, value in expected_results.items():
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_power_model.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_power_model.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_power_spectrum.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_power_spectrum.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,56 @@
 import numpy as np
 import pytest
 
 from lumicks.pylake.force_calibration.power_spectrum import PowerSpectrum
 
 
+def test_power_spectrum_bad_shape():
+    with pytest.raises(
+        ValueError,
+        match=r"Only 1D arrays of data are supported. You provided a 2D array of shape \(10, 2\)",
+    ):
+        _ = PowerSpectrum(np.ones((10, 2)), 1, window_seconds=1)
+
+
+def test_power_spectrum_variance():
+    """Testing the variance of Welch PSD estimates"""
+    sigma, sample_rate = 40, 100
+
+    np.random.seed(90083773)
+    ps = PowerSpectrum(sigma * np.random.normal(size=(1000000)), sample_rate, window_seconds=1)
+    avg_variance = np.mean(ps._variance[1:-1])  # First and last bin have twice the variance
+
+    # scaling_factor = (2.0 / sample_rate)
+    # average power is: sigma**2 * scaling_factor
+    # its variance is: (sigma**2 * scaling_factor)**2 (1024 here)
+    np.testing.assert_allclose(avg_variance, 1019.8465525703106)
+
+    mask = np.logical_and(ps.frequency > 10, ps.frequency <= 25)
+    np.testing.assert_equal(
+        ps.in_range(frequency_min=10.0, frequency_max=25.0)._variance, ps._variance[mask]
+    )
+
+    mask = np.logical_or(ps.frequency < 10, ps.frequency >= 25)
+    np.testing.assert_equal(ps._exclude_range([[10, 25]])._variance, ps._variance[mask])
+
+    # A single window won't give us a variance
+    ps = PowerSpectrum(
+        sigma * np.random.normal(size=(2 * sample_rate - 1)), sample_rate, window_seconds=1
+    )
+    assert ps._variance is None
+    assert ps.in_range(10, 15)._variance is None
+
+    # Two windows will (though it will likely not be a great estimate)
+    ps = PowerSpectrum(
+        sigma * np.random.normal(size=(2 * sample_rate)), sample_rate, window_seconds=1
+    )
+    assert np.all(ps._variance)
+
+
 @pytest.mark.parametrize(
     "frequency, num_data, sample_rate",
     [
         [200, 50, 2000],
         [400, 50, 2000],
         [400, 50, 4000],
         [400, 50, 4000],
@@ -212,14 +255,15 @@
         [[(3, 6), (9, 10)], [1, 7, 11], [10, 70, 110]],  # Disjoint range
     ],
 )
 def test_exclusions(exclusion_ranges, result_frequency, result_power):
     ps = PowerSpectrum([1], 78125, unit="V")
     ps.frequency = np.arange(1, 12, 2)
     ps.power = np.arange(10, 120, 20)
+    ps._variance = None
     excluded_range = ps._exclude_range(exclusion_ranges)
     np.testing.assert_allclose(excluded_range.frequency, result_frequency)
     np.testing.assert_allclose(excluded_range.power, result_power)
 
 
 def test_identify_peaks_args():
     power_spectrum = PowerSpectrum([1], 5)
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,52 +57,44 @@
 
 def test_calibration_result():
     with pytest.raises(TypeError):
         psc.CalibrationResults(invalid=5)
 
 
 @pytest.mark.parametrize(
-    "loss_function, corner_frequency,diffusion_constant,alpha,f_diode,num_samples,viscosity,bead_diameter,"
-    "temperature,err_fc,err_d,err_f_diode,err_alpha,",
-    # fmt: off
+    "loss_function, corner_frequency,diffusion_constant,alpha,f_diode,num_samples,viscosity,bead_diameter,temperature",
     [
-        ["gaussian", 1000, 1e-9, 0.5, 10000, 30000, 1.002e-3, 4.0, 20.0, 29.77266, 2.984664e-11, 1239.061833, 0.05615039],
-        ["gaussian", 1500, 1.2e-9, 0.5, 10000, 50000, 1.002e-3, 4.0, 20.0, 47.2181, 4.589085e-11, 1399.049903, 0.05856517],
-        ["gaussian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.002e-3, 4.0, 20.0, 70.59478, 8.226641e-11, 487.4102, 0.01342818],
-        ["gaussian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.2e-3, 4.0, 20.0, 70.59478, 8.226641e-11, 487.4102, 0.01342818],
-        ["gaussian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.002e-3, 8.0, 20.0, 70.59478, 8.226641e-11, 487.4102, 0.01342818],
-        ["gaussian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.002e-3, 4.0, 34.0, 70.59478, 8.226641e-11, 487.4102, 0.01342818],
-        ["gaussian", 1000, 1e-9, 0.5, 10000, 30000, 1.002e-3, 4.0, 20.0, 29.77266, 2.984664e-11, 1239.061833, 0.05615039],
-        ["gaussian", 1000, 1e-9, 0.5, 10000, 30000, 1, 4.0, 20.0, 29.77266, 2.984664e-11, 1239.061833, 0.05615039],
-        ["lorentzian", 1000, 1e-9, 0.5, 10000, 30000, 1.002e-3, 4.0, 20.0, np.nan, np.nan, np.nan, np.nan],
-        ["lorentzian", 1500, 1.2e-9, 0.5, 10000, 50000, 1.002e-3, 4.0, 20.0, np.nan, np.nan, np.nan, np.nan],
-        ["lorentzian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.002e-3, 4.0, 20.0, np.nan, np.nan, np.nan, np.nan],
-        ["lorentzian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.2e-3, 4.0, 20.0, np.nan, np.nan, np.nan, np.nan],
-        ["lorentzian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.002e-3, 8.0, 20.0, np.nan, np.nan, np.nan, np.nan],
-        ["lorentzian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.002e-3, 4.0, 34.0, np.nan, np.nan, np.nan, np.nan],
-        ["lorentzian", 1000, 1e-9, 0.5, 10000, 30000, 1.002e-3, 4.0, 20.0, np.nan, np.nan, np.nan, np.nan],
-        ["lorentzian", 1000, 1e-9, 0.5, 10000, 30000, 1, 4.0, 20.0, np.nan, np.nan, np.nan, np.nan],
+        ["gaussian", 1000, 1e-9, 0.5, 10000, 30000, 1.002e-3, 4.0, 20.0],
+        ["gaussian", 1500, 1.2e-9, 0.5, 10000, 50000, 1.002e-3, 4.0, 20.0],
+        ["gaussian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.002e-3, 4.0, 20.0],
+        ["gaussian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.2e-3, 4.0, 20.0],
+        ["gaussian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.002e-3, 8.0, 20.0],
+        ["gaussian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.002e-3, 4.0, 34.0],
+        ["gaussian", 1000, 1e-9, 0.5, 10000, 30000, 1, 4.0, 20.0],
+        ["lorentzian", 1000, 1e-9, 0.5, 10000, 30000, 1.002e-3, 4.0, 20.0],
+        ["lorentzian", 1500, 1.2e-9, 0.5, 10000, 50000, 1.002e-3, 4.0, 20.0],
+        ["lorentzian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.002e-3, 4.0, 20.0],
+        ["lorentzian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.2e-3, 4.0, 20.0],
+        ["lorentzian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.002e-3, 8.0, 20.0],
+        ["lorentzian", 1500, 1.2e-9, 0.5, 5000, 30000, 1.002e-3, 4.0, 34.0],
+        ["lorentzian", 1000, 1e-9, 0.5, 10000, 30000, 1, 4.0, 20.0],
     ],
-    # fmt: on
 )
-def test_good_fit_integration_test(
+def test_good_fit_integration(
+    compare_to_reference_dict,
     reference_models,
     loss_function,
     corner_frequency,
     diffusion_constant,
     alpha,
     f_diode,
     num_samples,
     viscosity,
     bead_diameter,
     temperature,
-    err_fc,
-    err_d,
-    err_f_diode,
-    err_alpha,
 ):
     data, f_sample = reference_models.lorentzian_td(
         corner_frequency, diffusion_constant, alpha, f_diode, num_samples
     )
     model = PassiveCalibrationModel(bead_diameter, temperature=temperature, viscosity=viscosity)
     power_spectrum = psc.calculate_power_spectrum(
         data, f_sample, fit_range=(0, 15000), num_points_per_block=20
@@ -126,18 +118,21 @@
     np.testing.assert_allclose(ps_calibration["kappa"].value, kappa_true, rtol=1e-4)
     np.testing.assert_allclose(ps_calibration["Rd"].value, rd_true, rtol=1e-4)
     np.testing.assert_allclose(ps_calibration["Rf"].value, rd_true * kappa_true * 1e3, rtol=1e-4)
     np.testing.assert_allclose(
         ps_calibration["chi_squared_per_deg"].value, 0, atol=1e-9
     )  # Noise free
 
-    np.testing.assert_allclose(ps_calibration["err_fc"].value, err_fc)
-    np.testing.assert_allclose(ps_calibration["err_D"].value, err_d, rtol=1e-4, atol=0)
-    np.testing.assert_allclose(ps_calibration["err_f_diode"].value, err_f_diode)
-    np.testing.assert_allclose(ps_calibration["err_alpha"].value, err_alpha, rtol=1e-6)
+    if loss_function == "gaussian":
+        compare_to_reference_dict(
+            {
+                par: ps_calibration[par].value
+                for par in ("err_fc", "err_D", "err_f_diode", "err_alpha", "err_kappa", "err_Rd")
+            }
+        )
 
 
 def test_fit_settings(reference_models):
     """This test tests whether the algorithm parameters ftol, max_function_evals and
     analytical_fit_range for lk.fit_power_spectrum() are applied as intended."""
     sample_rate = 78125
     corner_frequency, diffusion_volt = 4000, 1.14632
@@ -200,24 +195,38 @@
     ps_calibration = psc.fit_power_spectrum(
         power_spectrum=reference_spectrum, model=model, bias_correction=False
     )
 
     return ps_calibration, model, reference_spectrum
 
 
+def test_bad_fit(reference_calibration_result):
+    ps_calibration, model, reference_spectrum = reference_calibration_result
+    bad_spectrum = reference_spectrum.power.copy()
+    bad_spectrum[30:31] = reference_spectrum.power[10]  # Chop!
+    bad_spectrum = reference_spectrum.with_spectrum(
+        bad_spectrum, num_points_per_block=reference_spectrum.num_points_per_block
+    )
+    bad_calibration = psc.fit_power_spectrum(
+        power_spectrum=bad_spectrum, model=model, loss_function="gaussian"
+    )
+
+    assert ps_calibration["backing"].value > bad_calibration["backing"].value
+
+
 def test_actual_spectrum(reference_calibration_result):
     ps_calibration, model, reference_spectrum = reference_calibration_result
 
     results = {
         "D": {"desired": 0.0018512505734895896, "rtol": 1e-4, "atol": 0},
         "Rd": {"desired": 7.253677199344564, "rtol": 1e-4},
         "Rf": {"desired": 1243.966729922322, "rtol": 1e-4},
         "kappa": {"desired": 0.17149463585651784, "rtol": 1e-4},
         "alpha": {"desired": 0.5006070381347969, "rtol": 1e-4},
-        "backing": {"desired": 66.43310564863437, "rtol": 1e-4},
+        "backing": {"desired": 30.570451, "rtol": 1e-4},
         "chi_squared_per_deg": {"desired": 1.0637833024139873, "rtol": 1e-4},
         "err_fc": {"desired": 32.22822335114943, "rtol": 1e-4},
         "err_D": {"desired": 6.429704886151389e-05, "rtol": 1e-4, "atol": 0},
         "err_alpha": {"desired": 0.013140824804884007, "rtol": 1e-4},
         "err_f_diode": {"desired": 561.7212147994059, "rtol": 1e-4},
     }
 
@@ -256,28 +265,34 @@
 def test_attributes_ps_calibration(reference_calibration_result):
     ps_calibration, model, reference_spectrum = reference_calibration_result
     assert id(ps_calibration.model) == id(model)
     assert id(ps_calibration.ps_data) == id(reference_spectrum)
 
     with pytest.raises(RuntimeError):
         psc.CalibrationResults(
-            model=None, ps_model=None, ps_data=None, params={"test": 5}, results={"test2": 5}
+            model=None,
+            ps_model=None,
+            ps_data=None,
+            params={"test": 5},
+            results={"test2": 5},
+            fitted_params=[],
         )
 
 
 def test_calibration_results_params():
     result = psc.CalibrationResults(
         model=None,
         ps_model=None,
         ps_data=None,
         params={"test": psc.CalibrationParameter("par", "val", 5)},
         results={
             "Rf": psc.CalibrationParameter("Rf", "val", 5),
             "kappa": psc.CalibrationParameter("kappa", "val", 5),
         },
+        fitted_params=[],
     )
     assert "test" in result
     assert "Rf" in result
     assert "nope" not in result
 
 
 def test_repr(reference_calibration_result):
@@ -296,24 +311,26 @@
         Sample rate          Sample rate (Hz)                                          78125
         Bias correction      Perform bias correction thermal fit                       0
         Loss function        Loss function used during minimization                    gaussian
         Rd                   Distance response (um/V)                                  7.25366
         kappa                Trap stiffness (pN/nm)                                    0.171495
         Rf                   Force response (pN/V)                                     1243.97
         gamma_0              Theoretical bulk drag coefficient (kg/s)                  4.1552e-08
+        err_kappa            Stiffness Std Err (pN/V)                                  0.00841414
+        err_Rd               Distance response Std Err (um/V)                          0.125966
         fc                   Corner frequency (Hz)                                     656.872
         D                    Diffusion constant (V^2/s)                                0.00185126
         err_fc               Corner frequency Std Err (Hz)                             32.2284
         err_D                Diffusion constant Std Err (V^2/s)                        6.42974e-05
         f_diode              Diode low-pass filtering roll-off frequency (Hz)          7936.51
         alpha                Diode 'relaxation factor'                                 0.500609
         err_f_diode          Diode low-pass filtering roll-off frequency Std Err (Hz)  561.715
         err_alpha            Diode 'relaxation factor' Std Err                         0.0131406
         chi_squared_per_deg  Chi squared per degree of freedom                         1.06378
-        backing              Statistical backing (%)                                   66.4331"""
+        backing              Statistical backing (%)                                   30.5705"""
     )
 
 
 def test_invalid_bead_diameter():
     with pytest.raises(ValueError, match="Invalid bead diameter specified"):
         PassiveCalibrationModel(bead_diameter=0)
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_simulations.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_simulations.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/tests/test_touchdown.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/tests/test_touchdown.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/force_calibration/touchdown.py` & `lumicks.pylake-1.5.0/lumicks/pylake/force_calibration/touchdown.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/group.py` & `lumicks.pylake-1.5.0/lumicks/pylake/group.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/image_stack.py` & `lumicks.pylake-1.5.0/lumicks/pylake/image_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -482,14 +482,15 @@
         channel="rgb",
         figure_scale=0.75,
         adjustment=no_adjustment,
         *,
         vertical=False,
         include_dead_time=False,
         return_frame_setter=False,
+        downsample_to_frames=True,
     ):
         """Downsample channel on a frame by frame basis and plot the results. The downsampling
         function (e.g. `np.mean`) is evaluated for the time between a start and end time of a
         frame.
 
         Actions
         -------
@@ -516,14 +517,16 @@
             Color adjustments to apply to the output image.
         vertical : bool, optional
             Align plots vertically, default: False.
         include_dead_time : bool, optional
             Include dead time between frames, default: False.
         return_frame_setter : bool, optional
             Whether to return a handle that allows updating the plotted frame, default: False.
+        downsample_to_frames : bool, optional
+            Downsample the channel data over frame timestamp ranges (default: True).
 
         Note
         ----
         In environments which support interactive figures (e.g. `jupyter notebook` with
         `ipywidgets` or interactive python) this plot will be interactive.
 
         Examples
@@ -550,14 +553,15 @@
             get_plot_data=frame_grabber,
             title_factory=lambda frame: make_image_title(self, frame, show_name=False),
             frame=frame,
             reduce=reduce,
             figure_scale=figure_scale,
             post_update=post_update,
             vertical=vertical,
+            downsample_to_frames=downsample_to_frames,
         )
 
         if return_frame_setter:
             return frame_setter
 
     @property
     def size_um(self) -> Optional[list]:
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymo.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import warnings
 from copy import copy
 from dataclasses import dataclass
 
 import numpy as np
 
+from .channel import Slice
 from .adjustments import colormaps, no_adjustment
 from .detail.image import (
     InfowaveCode,
     round_down,
     histogram_rows,
     seek_timestamp_next_line,
     first_pixel_sample_indices,
@@ -409,62 +410,175 @@
         axes.set_xlabel("time (s)")
         axes.set_ylabel(f"position ({self._calibration.unit_label})")
         if show_title:
             axes.set_title(self.name)
 
         return image_handle
 
-    def plot_with_force(
+    def plot_with_channels(
         self,
-        force_channel,
-        color_channel,
+        channels,
+        color_channel="rgb",
+        *,
         aspect_ratio=0.25,
-        reduce=np.mean,
         kymo_args=None,
         adjustment=no_adjustment,
+        title_vertical=False,
+        labels=None,
+        colors=None,
+        scale_bar=None,
         **kwargs,
     ):
-        """Plot kymo with force channel downsampled over scan lines
-
-        Note that high frequency channel data must be available for this function to work.
+        """Plot kymo with channel data.
 
         Parameters
         ----------
-        force_channel: str
-            name of force channel to downsample and plot (e.g. '1x')
-        color_channel: str
+        channels : Slice | List[Slice]
+            data slice or list of slices
+        color_channel : str
             color channel of kymo to plot ('red', 'green', 'blue', 'rgb')
         aspect_ratio: float
             aspect ratio of the axes (i.e. ratio of y-unit to x-unit)
-        reduce : callable
-            The :mod:`numpy` function which is going to reduce multiple samples into one. Forwarded
-            to :meth:`Slice.downsampled_over() <lumicks.pylake.channel.Slice.downsampled_over()>`
         kymo_args : Optional[dict]
             Forwarded to :func:`matplotlib.pyplot.imshow()`
         adjustment : lk.ColorAdjustment
             Color adjustments to apply to the output image.
+        title_vertical : bool
+            Place channel title on vertical axis
+        labels : str | List[str]
+            Custom labels to plot with the channels
+        colors : List[matplotlib.color]
+            Forwarded to color argument of :func:`matplotlib.pyplot.plot()`.
+        scale_bar : lk.ScaleBar, optional
+            Scale bar to add to the kymograph.
         **kwargs
             Forwarded to :meth:`Slice.plot() <lumicks.pylake.channel.Slice.plot()>`.
+
+        Examples
+        --------
+        ::
+
+            import lumicks.pylake as lk
+            import matplotlib.pyplot as plt
+            import numpy as np
+
+            h5_file = lk.File("example.h5")
+            _, kymo = h5_file.kymos.popitem()
+
+            kymo.plot_with_channels(
+                [
+                    h5_file.force1x.downsampled_by(100),
+                    h5_file["Photon count"]["Green"].downsampled_over(kymo.line_timestamp_ranges(), reduce=np.sum),
+                ],
+                "rgb",
+                adjustment=lk.ColorAdjustment(5, 98, "percentile"),
+                aspect_ratio=0.2,
+                title_vertical=True,
+            )
         """
 
         def set_aspect_ratio(axis, ar):
             """This function forces a specific aspect ratio, can be useful when aligning figures"""
             axis.set_aspect(ar * np.abs(np.diff(axis.get_xlim())[0] / np.diff(axis.get_ylim()))[0])
 
+        def check_length(items, item_type):
+            if len(items) != len(channels):
+                raise ValueError(
+                    f"When a list of {item_type} is provided, it needs to have the same length as "
+                    f"the number of channels provided. Expected {len(channels)}, got: "
+                    f"{len(items)}."
+                )
+
         import matplotlib.pyplot as plt
+        from matplotlib.colors import is_color_like
+
+        channels = [channels] if isinstance(channels, Slice) else channels
+        for channel in channels:
+            if not isinstance(channel, Slice):
+                raise ValueError(
+                    "channel is not a Slice or list of Slice objects. "
+                    f"Got {type(channel).__name__} instead."
+                )
 
-        _, (ax1, ax2) = plt.subplots(2, 1, sharex="all")
+        if labels:
+            labels = [labels] if isinstance(labels, str) else labels
+            check_length(labels, "labels")
+
+        if colors:
+            colors = [colors] if is_color_like(colors) else colors
+            check_length(colors, "colors")
+
+        _, axes = plt.subplots(len(channels) + 1, 1, sharex="all")
 
         # plot kymo
-        self.plot(channel=color_channel, axes=ax1, adjustment=adjustment, **(kymo_args or {}))
-        ax1.set_xlabel(None)
-        xlim_kymo = ax1.get_xlim()  # Stored since plotting the force channel will change the limits
+        scale_bar = {"scale_bar": scale_bar} if scale_bar is not None else {}
+        kymo_args = ({} if kymo_args is None else kymo_args) | scale_bar
+        self.plot(channel=color_channel, axes=axes[0], adjustment=adjustment, **kymo_args)
+
+        # Storing these since plotting the data channels will change the limits
+        xlim_kymo = axes[0].get_xlim()
+
+        # plot data channels
+        for idx, (ax, channel) in enumerate(zip(axes[1:], channels)):
+            plt.sca(ax)
+            plot_args = kwargs if not colors else kwargs | {"color": colors[idx]}
+            # Cropping the channel to the kymograph time range leads to better axis limits
+            channel[self.start : self.stop + 1].plot(**plot_args)
+            ax.set_xlim(xlim_kymo)
+
+            if title_vertical:
+                ax.set_title(None)
+                y_label = channel.labels.get("y", "")
+
+                # Labelling with y is unnecessary.
+                y_label = f"\n{y_label}" if y_label != "y" else ""
+
+                ax.set_ylabel(f"{channel.labels.get('title', '').split('/')[-1]}{y_label}")
+
+            if labels:
+                ax.set_ylabel(labels[idx])
+
+        for ax in axes:
+            set_aspect_ratio(ax, aspect_ratio)
+
+        for ax in axes[:-1]:
+            ax.set_xlabel(None)
 
-        # plot force channel
-        plt.sca(ax2)
+    def plot_with_force(
+        self,
+        force_channel,
+        color_channel,
+        aspect_ratio=0.25,
+        reduce=np.mean,
+        kymo_args=None,
+        adjustment=no_adjustment,
+        **kwargs,
+    ):
+        """Plot kymo with force channel downsampled over scan lines
+
+        Note that high frequency channel data must be available for this function to work.
+
+        Parameters
+        ----------
+        force_channel : str
+            name of force channel to downsample and plot (e.g. '1x')
+        color_channel : str
+            color channel of kymo to plot ('red', 'green', 'blue', 'rgb')
+        aspect_ratio : float
+            aspect ratio of the axes (i.e. ratio of y-unit to x-unit)
+        reduce : callable
+            The :mod:`numpy` function which is going to reduce multiple samples into one. Forwarded
+            to :meth:`Slice.downsampled_over() <lumicks.pylake.channel.Slice.downsampled_over()>`
+        kymo_args : Optional[dict]
+            Forwarded to :func:`matplotlib.pyplot.imshow()`
+        adjustment : lk.ColorAdjustment
+            Color adjustments to apply to the output image.
+        **kwargs
+            Forwarded to :meth:`Slice.plot() <lumicks.pylake.channel.Slice.plot()>`.
+        """
         try:
             channel = getattr(self.file, f"force{force_channel}")
         except ValueError:
             raise ValueError(
                 f"There is no force data associated with this {self.__class__.__name__}"
             )
         if not channel:
@@ -474,22 +588,24 @@
                     f"Desired force channel {force_channel} not available in h5 file"
                 )
 
             warnings.warn(
                 RuntimeWarning("Using downsampled force since high frequency force is unavailable.")
             )
 
-        time_ranges = self.line_timestamp_ranges(include_dead_time=False)
-        force = channel.downsampled_over(time_ranges, reduce=reduce, where="center")
-
-        force.plot(**kwargs)
-        ax2.set_xlim(xlim_kymo)
-
-        set_aspect_ratio(ax1, aspect_ratio)
-        set_aspect_ratio(ax2, aspect_ratio)
+        self.plot_with_channels(
+            channel.downsampled_over(
+                self.line_timestamp_ranges(include_dead_time=False), reduce=reduce, where="center"
+            ),
+            color_channel,
+            aspect_ratio=aspect_ratio,
+            kymo_args=kymo_args,
+            adjustment=adjustment,
+            **kwargs,
+        )
 
     def plot_with_position_histogram(
         self,
         color_channel,
         pixels_per_bin=1,
         hist_ratio=0.25,
         adjustment=no_adjustment,
@@ -900,19 +1016,19 @@
         **kwargs
             Forwarded to :meth:`Kymo.plot()`.
 
         Examples
         --------
         ::
 
-            from lumicks import pylake
+            import lumicks.pylake as lk
             import matplotlib.pyplot as plt
 
             # Loading a kymograph.
-            h5_file = pylake.File("example.h5")
+            h5_file = lk.File("example.h5")
             _, kymo = h5_file.kymos.popitem()
             widget = kymo.crop_and_calibrate("green", 48.502)
             plt.show()
 
             # Select cropping ROI by left-click drag
 
             # Grab the updated image stack
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/denoising.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/denoising.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/gaussian_mle.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/gaussian_mle.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/geometry_2d.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/geometry_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/linalg_2d.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/linalg_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/localization_models.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/localization_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/msd_estimation.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/msd_estimation.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/peakfinding.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/peakfinding.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/scoring_functions.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/scoring_functions.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/sequence.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/sequence.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/stitch.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/stitch.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/detail/trace_line_2d.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/detail/trace_line_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/kymotrack.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/kymotrack.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,14 +413,15 @@
     def __getitem__(self, item):
         return np.squeeze(
             np.array(np.vstack((self.time_idx[item], self.coordinate_idx[item]))).transpose()
         )
 
     @property
     def time_idx(self):
+        """Return temporal coordinates in units of pixels."""
         return self._time_idx
 
     @property
     def coordinate_idx(self):
         """Return spatial coordinates in units of pixels.
 
         Coordinates are defined w.r.t. pixel centers (i.e. 0, 0 is the center of the first pixel).
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/kymotracker.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/kymotracker.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/stitching.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/stitching.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/conftest.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/test_sequence.gb` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/test_sequence.gb`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/tracks_v3.csv` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v3.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/tracks_v4.csv` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/tracks_v4.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_basic/output_image_1d.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/output_image_1d.npz`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 13712 bytes, number of entries: 1
-?rw-------  2.0 unx    13576 b- stor 80-Jan-01 00:00 arr_0.npy
+?rw-------  4.5 unx    13576 b- stor 80-Jan-01 00:00 arr_0.npy
 1 file, 13576 bytes uncompressed, 13576 bytes compressed:  0.0%
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v4.5 to extract, compression method=store
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_basic/output_image_2d.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/output_image_2d.npz`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 13712 bytes, number of entries: 1
-?rw-------  2.0 unx    13576 b- stor 80-Jan-01 00:00 arr_0.npy
+?rw-------  4.5 unx    13576 b- stor 80-Jan-01 00:00 arr_0.npy
 1 file, 13576 bytes uncompressed, 13576 bytes compressed:  0.0%
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v4.5 to extract, compression method=store
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/1d_background.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/1d_background.npz`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 13712 bytes, number of entries: 1
-?rw-------  2.0 unx    13576 b- stor 80-Jan-01 00:00 arr_0.npy
+?rw-------  4.5 unx    13576 b- stor 80-Jan-01 00:00 arr_0.npy
 1 file, 13576 bytes uncompressed, 13576 bytes compressed:  0.0%
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v4.5 to extract, compression method=store
```

#### arr_0.npy

```diff
@@ -12,19 +12,19 @@
 000000b0: 9b99 9919 8452 0040 0000 0000 80b1 0940  .....R.@.......@
 000000c0: 0000 0000 808a 0c40 0000 0000 8089 0840  .......@.......@
 000000d0: cdcc cc94 e3a6 0140 6666 5865 a12a 1440  .......@ffXe.*.@
 000000e0: 9999 99ed f21f 1040 0000 0000 8059 0a40  .......@.....Y.@
 000000f0: 0000 0000 005f 0440 0000 0000 0023 0640  ....._.@.....#.@
 00000100: cdcc cc44 5a71 0440 cdcc cc24 e0c4 0340  ...DZq.@...$...@
 00000110: 0000 0000 80b8 0840 0000 0000 0083 0740  .......@.......@
-00000120: 6666 66be 328d 1240 0200 2858 ab78 0040  fff.2..@..(X.x.@
+00000120: 6666 66be 328d 1240 0100 2858 ab78 0040  fff.2..@..(X.x.@
 00000130: cdcc cc64 bba4 0040 0000 0000 805c 0240  ...d...@.....\.@
 00000140: 9a99 9979 542c fe3f 0000 0000 00d2 0940  ...yT,.?.......@
 00000150: cdcc cc04 8ed5 0f40 9874 ee5e 590a 0840  .......@.t.^Y..@
-00000160: cd4c 0b05 c9f5 0e40 6462 1c61 6b88 1740  .L.....@db.ak..@
+00000160: cd4c 0b05 c9f5 0e40 6662 1c61 6b88 1740  .L.....@fb.ak..@
 00000170: 0000 0000 807b 0340 3333 3373 861f 0a40  .....{.@333s...@
 00000180: 0000 0000 80b6 0840 0000 0000 8010 0540  .......@.......@
 00000190: 0000 0000 0058 0940 0000 0000 001f 0840  .....X.@.......@
 000001a0: 0000 0000 40e2 1140 0000 0000 80bc 0e40  ....@..@.......@
 000001b0: 287d d07d abc3 1640 c8c4 a6d5 5f9d 1d40  (}.}...@...._..@
 000001c0: ea5a f119 f379 0740 0000 0000 0079 0740  .Z...y.@.....y.@
 000001d0: cc78 fbad 14c9 0840 3333 336b 7157 0d40  .x.....@333kqW.@
@@ -37,41 +37,41 @@
 00000240: 0000 0000 0018 0640 cdcc ccfc 5cb4 0440  .......@....\..@
 00000250: cdcc ccbc 19e7 0340 0000 0000 00d4 0840  .......@.......@
 00000260: 0000 0000 8086 0740 9999 9996 ff59 1240  .......@.....Y.@
 00000270: 9a99 5f26 c666 0840 cdcc cc1c 17db 0040  .._&.f.@.......@
 00000280: 0000 0000 0065 0240 9a99 9909 32e0 fe3f  .....e.@....2..?
 00000290: 0000 0000 00c5 0940 6766 66c6 c60b 1040  .......@gff....@
 000002a0: 76a1 d014 ae28 0840 0000 0000 00c1 0e40  v....(.@.......@
-000002b0: 9a91 3ff8 c7f6 1340 0000 0000 00af 0340  ..?....@.......@
+000002b0: 9891 3ff8 c7f6 1340 0000 0000 00af 0340  ..?....@.......@
 000002c0: 3333 334b f9c6 0940 0000 0000 00da 0840  333K...@.......@
 000002d0: 0000 0000 0012 0540 0000 0000 0049 0940  .......@.....I.@
 000002e0: 0000 0000 8005 0840 0000 0000 40e0 1140  .......@....@..@
 000002f0: 0000 0000 008d 0e40 b9e3 0932 9715 1240  .......@...2...@
-00000300: b45b 4829 cbdd 1a40 2c2f 2cee 3585 0740  .[H)...@,/,.5..@
+00000300: b45b 4829 cbdd 1a40 2d2f 2cee 3585 0740  .[H)...@-/,.5..@
 00000310: 0000 0000 00a8 0740 cdfc 6f39 f4cc 0940  .......@..o9...@
 00000320: 4d6f 522b 07d7 0c40 0000 0000 008d 0440  MoR+...@.......@
 00000330: 0000 0000 807c 0640 0000 0000 00f7 0740  .....|.@.......@
 00000340: 0100 0050 7210 0840 cbcc 4cce fb1c 0a40  ...Pr..@..L....@
 00000350: 0000 0000 80d9 0c40 0000 0000 808a 0840  .......@.......@
 00000360: cdcc cc64 4288 0240 9959 e699 c55f 1340  ...dB..@.Y..._.@
 00000370: 3333 33cb ffa3 0f40 0000 0000 805d 0a40  333....@.....].@
 00000380: 0000 0000 807c 0440 0000 0000 8010 0640  .....|.@.......@
 00000390: 0000 0000 8017 0540 cdcc cc24 9722 0440  .......@...$.".@
 000003a0: 0000 0000 000d 0940 0000 0000 0085 0740  .......@.......@
 000003b0: ffff ff2c 02f8 1140 cdcc 8d08 a447 0940  ...,...@.....G.@
 000003c0: 0000 0000 803c 0140 0000 0000 8078 0240  .....<.@.....x.@
 000003d0: cdcc cce4 4d18 0040 0000 0000 80ac 0940  ....M..@.......@
 000003e0: 0000 0000 c04b 1040 a219 9b12 4f64 0840  .....K.@....Od.@
-000003f0: 0000 0000 0070 0e40 68b8 fc3c 6d65 0e40  .....p.@h..<me.@
+000003f0: 0000 0000 0070 0e40 67b8 fc3c 6d65 0e40  .....p.@g..<me.@
 00000400: 0000 0000 0005 0440 0000 0000 8025 0940  .......@.....%.@
 00000410: 0000 0000 8018 0940 0000 0000 0013 0540  .......@.......@
 00000420: 0000 0000 802e 0940 0000 0000 80d2 0740  .......@.......@
 00000430: 0000 0000 40df 1140 0000 0000 8039 0e40  ....@..@.....9.@
-00000440: 08fa ba64 f060 1140 337b 7f27 0c17 1640  ...d.`.@3{.'...@
-00000450: fa28 8864 d7a2 0740 0000 0000 80e5 0740  .(.d...@.......@
+00000440: 08fa ba64 f060 1140 317b 7f27 0c17 1640  ...d.`.@1{.'...@
+00000450: fb28 8864 d7a2 0740 0000 0000 80e5 0740  .(.d...@.......@
 00000460: 0132 3b21 b351 0b40 e6d1 ba65 fb1a 0c40  .2;!.Q.@...e...@
 00000470: 0000 0000 805c 0440 0000 0000 80c4 0640  .....\.@.......@
 00000480: 0000 0000 8004 0840 0000 0000 80bf 0840  .......@.......@
 00000490: feff 93b9 5636 0e40 0000 0000 0017 0d40  ....V6.@.......@
 000004a0: 0000 0000 8082 0840 0000 0000 804c 0340  .......@.....L.@
 000004b0: 9999 952c 19ae 1240 0000 0000 802e 0f40  ...,...@.......@
 000004c0: 0000 0000 8053 0a40 0000 0000 009e 0440  .....S.@.......@
@@ -84,15 +84,15 @@
 00000530: b2a7 0ca6 83c3 0840 0000 0000 000c 0e40  .......@.......@
 00000540: 806a ad43 9573 0c40 0000 0000 006f 0440  .j.C.s.@.....o.@
 00000550: 0000 0000 0080 0840 0000 0000 8066 0940  .......@.....f.@
 00000560: 0000 0000 000c 0540 0000 0000 8004 0940  .......@.......@
 00000570: 0000 0000 0085 0740 0000 0000 00e2 1140  .......@.......@
 00000580: 0000 0000 00d5 0d40 0000 0000 402a 1040  .......@....@*.@
 00000590: 9dce 6810 83e0 1440 06c6 7001 95e0 0740  ..h....@..p....@
-000005a0: 0000 0000 002a 0840 98f9 d5c3 e93b 0c40  .....*.@.....;.@
+000005a0: 0000 0000 002a 0840 99f9 d5c3 e93b 0c40  .....*.@.....;.@
 000005b0: 8032 e3f8 7e28 0b40 0000 0000 002b 0440  .2..~(.@.....+.@
 000005c0: 0000 0000 8020 0740 0000 0000 000c 0840  ..... .@.......@
 000005d0: 0000 0000 0064 0940 5833 d3ec 1e58 d73f  .....d.@X3...X.?
 000005e0: 0000 0000 005b 0d40 0000 0000 0070 0840  .....[.@.....p.@
 000005f0: 0000 0000 000a 0440 cccc 67d7 14d5 1140  .......@..g....@
 00000600: 0000 0000 809a 0e40 0000 0000 0044 0a40  .......@.....D.@
 00000610: 0000 0000 80d9 0440 0000 0000 0028 0640  .......@.....(.@
@@ -103,56 +103,56 @@
 00000660: 0000 0000 00ea 0140 0000 0000 8079 0940  .......@.....y.@
 00000670: 0000 0000 c0df 1040 e1bb 32f8 a64e 0940  .......@..2..N.@
 00000680: 0000 0000 80b6 0d40 9bb1 5299 922a 0b40  .......@..R..*.@
 00000690: 0000 0000 00e0 0440 0000 0000 00ba 0740  .......@.......@
 000006a0: 0000 0000 80b1 0940 0000 0000 00f9 0440  .......@.......@
 000006b0: 0000 0000 00c7 0840 0000 0000 8024 0740  .......@.....$.@
 000006c0: 0000 0000 80ea 1140 0000 0000 0070 0d40  .......@.....p.@
-000006d0: 6294 7c1b 8e0e 0f40 f0a3 4ae9 f2bd 1340  b.|....@..J....@
-000006e0: cd21 5fd3 2650 0840 0000 0000 806a 0840  .!_.&P.@.....j.@
-000006f0: 9a99 72ff 1f30 0d40 0000 0000 003e 0a40  ..r..0.@.....>.@
+000006d0: 6294 7c1b 8e0e 0f40 f2a3 4ae9 f2bd 1340  b.|....@..J....@
+000006e0: ce21 5fd3 2650 0840 0000 0000 806a 0840  .!_.&P.@.....j.@
+000006f0: 9b99 72ff 1f30 0d40 0000 0000 003e 0a40  ..r..0.@.....>.@
 00000700: 0000 0000 0006 0440 0000 0000 008d 0740  .......@.......@
 00000710: 0000 0000 8010 0840 0000 0000 8004 0a40  .......@.......@
-00000720: cccc 9c63 8464 0e40 0000 0000 809b 0d40  ...c.d.@.......@
+00000720: cbcc 9c63 8464 0e40 0000 0000 809b 0d40  ...c.d.@.......@
 00000730: 0000 0000 0053 0840 0000 0000 00da 0440  .....S.@.......@
 00000740: 0000 0000 40f2 1040 0000 0000 00f5 0d40  ....@..@.......@
 00000750: 0000 0000 803c 0a40 0000 0000 0036 0540  .....<.@.....6.@
 00000760: cdcc cc2c 7066 0640 0000 0000 80d6 0640  ...,pf.@.......@
 00000770: cdcc cc5c d8da 0540 0000 0000 00f1 0940  ...\...@.......@
 00000780: 0000 0000 000f 0740 0000 0000 4043 1040  .......@....@C.@
 00000790: 9999 0628 13f5 0c40 0000 0000 80d3 0240  ...(...@.......@
 000007a0: 0000 0000 8017 0340 0000 0000 80d7 0240  .......@.......@
 000007b0: 0000 0000 0076 0940 0000 0000 c035 1140  .....v.@.....5.@
-000007c0: e0fe 1ac6 340f 0a40 65e6 d003 b4cb 0c40  ....4..@e......@
+000007c0: e0fe 1ac6 340f 0a40 66e6 d003 b4cb 0c40  ....4..@f......@
 000007d0: 9a59 5e5c b53d 0940 0000 0000 8057 0540  .Y^\.=.@.....W.@
 000007e0: 0000 0000 00ed 0640 0000 0000 80e5 0940  .......@.......@
 000007f0: 0000 0000 00db 0440 0000 0000 806b 0840  .......@.....k.@
 00000800: 0000 0000 00c5 0640 0000 0000 00f0 1140  .......@.......@
-00000810: 0000 0000 001a 0d40 0134 bd10 24bc 0c40  .......@.4..$..@
-00000820: 50ee be84 19f3 1140 562e 6276 f0ff 0840  P......@V.bv...@
+00000810: 0000 0000 001a 0d40 ff33 bd10 24bc 0c40  .......@.3..$..@
+00000820: 50ee be84 19f3 1140 572e 6276 f0ff 0840  P......@W.bv...@
 00000830: 0000 0000 00a3 0840 66fa aaf3 edca 0d40  .......@f......@
 00000840: 0000 0000 8045 0940 0000 0000 80f7 0340  .....E.@.......@
 00000850: 0000 0000 0002 0840 0000 0000 0013 0840  .......@.......@
 00000860: 0000 0000 0091 0a40 0000 40f3 11ad 0a40  .......@..@....@
 00000870: 0000 0000 80d8 0d40 0000 0000 002f 0840  .......@...../.@
 00000880: 0000 0000 80b1 0540 0000 0000 0025 1040  .......@.....%.@
 00000890: 0000 0000 8046 0d40 0000 0000 8044 0a40  .....F.@.....D.@
 000008a0: 0000 0000 00be 0540 0000 0000 80d5 0640  .......@.......@
 000008b0: 0000 0000 0075 0740 0000 0000 80d1 0640  .....u.@.......@
 000008c0: cd4c 3902 f81f 0a40 0000 0000 00bf 0640  .L9....@.......@
 000008d0: 0000 0000 0067 0f40 cdcc 44e8 b440 0e40  .....g.@..D..@.@
 000008e0: 0000 0000 006f 0340 0000 0000 8071 0340  .....o.@.....q.@
 000008f0: 0000 0000 80ce 0340 0000 0000 808c 0940  .......@.......@
 00000900: 0000 0000 008b 1140 0000 0000 00f7 0a40  .......@.......@
-00000910: 6966 6c17 af26 0d40 04e0 6012 3e69 fd3f  ifl..&.@..`.>i.?
+00000910: 6866 6c17 af26 0d40 04e0 6012 3e69 fd3f  hfl..&.@..`.>i.?
 00000920: 0000 0000 00cb 0540 0000 0000 0030 0640  .......@.....0.@
 00000930: 0000 0000 80f2 0940 0000 0000 00ac 0440  .......@.......@
 00000940: 0000 0000 80f3 0740 0000 0000 0074 0640  .......@.....t.@
 00000950: 0000 0000 00f2 1140 0000 0000 00dc 0c40  .......@.......@
-00000960: a35a 50c5 3fb3 0640 1124 e3d1 7ea4 0c40  .ZP.?..@.$..~..@
+00000960: a35a 50c5 3fb3 0640 1224 e3d1 7ea4 0c40  .ZP.?..@.$..~..@
 00000970: 3ab0 818a e6f8 0940 0000 0000 80cc 0840  :......@.......@
 00000980: 3263 5f51 d390 1540 0000 0000 0043 0840  2c_Q...@.....C.@
 00000990: 0000 0000 000c 0440 0000 0000 8070 0840  .......@.....p.@
 000009a0: 0000 0000 0008 0840 0000 0000 0005 0b40  .......@.......@
 000009b0: 3333 f343 17f5 0a40 0000 0000 8004 0e40  33.C...@.......@
 000009c0: 0000 0000 8004 0840 0000 0000 8080 0640  .......@.......@
 000009d0: 0000 0000 00a4 0e40 0000 0000 8097 0c40  .......@.......@
@@ -165,50 +165,50 @@
 00000a40: 0000 0000 80bf 0940 0000 0000 80dd 1140  .......@.......@
 00000a50: 0000 0000 00ef 0b40 9c99 59ec 229f 0340  .......@..Y."..@
 00000a60: 4d22 1150 e40e 0640 0000 0000 802c 0640  M".P...@.....,.@
 00000a70: cdcc cc54 fe86 0540 0000 0000 80d7 0940  ...T...@.......@
 00000a80: 0000 0000 0067 0440 0000 0000 8063 0740  .....g.@.....c.@
 00000a90: 0000 0000 8036 0640 0000 0000 00f0 1140  .....6.@.......@
 00000aa0: 0000 0000 00c2 0c40 9c9c a901 0103 0240  .......@.......@
-00000ab0: 62ea f8e1 8128 0740 34c4 7e27 8c78 0b40  b....(.@4.~'.x.@
-00000ac0: 0000 0000 80e5 0840 0020 b3af 0c8b 1740  .......@. .....@
+00000ab0: 61ea f8e1 8128 0740 36c4 7e27 8c78 0b40  a....(.@6.~'.x.@
+00000ac0: 0000 0000 80e5 0840 fe1f b3af 0c8b 1740  .......@.......@
 00000ad0: 0000 0000 003a 0740 0000 0000 0044 0440  .....:.@.....D.@
 00000ae0: 0000 0000 80d0 0840 0000 0000 00e9 0740  .......@.......@
 00000af0: 0000 0000 805c 0b40 0000 0000 00a0 0a40  .....\.@.......@
 00000b00: 0000 0000 8014 0e40 0000 0000 80cd 0740  .......@.......@
 00000b10: 0000 0000 803c 0740 0000 0000 800e 0d40  .....<.@.......@
 00000b20: 0000 0000 80ec 0b40 0000 0000 0071 0a40  .......@.....q.@
 00000b30: 0000 0000 0058 0740 0000 0000 8043 0840  .....X.@.....C.@
 00000b40: 0000 0000 8071 0840 0000 0000 00f6 0840  .....q.@.......@
 00000b50: 3333 53ed d9d5 0940 0000 0000 80d7 0540  33S....@.......@
 00000b60: 0000 0000 804b 0d40 33b3 93ef d567 0f40  .....K.@3....g.@
 00000b70: 0000 0000 00a5 0440 0000 0000 8042 0440  .......@.....B.@
 00000b80: 0000 0000 0095 0540 0000 0000 800c 0a40  .......@.......@
 00000b90: 0000 0000 c02a 1240 0000 0000 00ee 0c40  .....*.@.......@
-00000ba0: 3433 0be1 48b2 0340 4d09 26b6 e828 0540  43..H..@M.&..(.@
+00000ba0: 3433 0be1 48b2 0340 4e09 26b6 e828 0540  43..H..@N.&..(.@
 00000bb0: 0000 0000 0068 0640 cdcc cc84 d4f2 0440  .....h.@.......@
 00000bc0: 0000 0000 8095 0940 0000 0000 800f 0440  .......@.......@
 00000bd0: 0000 0000 80cb 0640 0000 0000 0012 0640  .......@.......@
 00000be0: 0000 0000 00eb 1140 0000 0000 80d4 0c40  .......@.......@
-00000bf0: 042a eb90 364a 0040 b9b7 29f8 bafc 0440  .*..6J.@..)....@
+00000bf0: 052a eb90 364a 0040 bab7 29f8 bafc 0440  .*..6J.@..)....@
 00000c00: 0abd 8757 f36f 0d40 0000 0000 00ed 0840  ...W.o.@.......@
 00000c10: 32f3 e0d2 a597 1440 0000 0000 8033 0640  2......@.....3.@
 00000c20: 0000 0000 009e 0440 3333 3363 6210 0940  .......@333cb..@
 00000c30: 0000 0000 00bd 0740 0000 0000 0097 0b40  .......@.......@
 00000c40: 0000 0000 80af 0a40 0000 0000 8001 0e40  .......@.......@
 00000c50: 0000 0000 808d 0740 0000 0000 80da 0740  .......@.......@
 00000c60: cd4c f27d f067 0b40 0000 0000 804b 0b40  .L.}.g.@.....K.@
 00000c70: 0000 0000 8083 0a40 0000 0000 8051 0840  .......@.....Q.@
 00000c80: 0000 0000 8038 0940 0000 0000 80b9 0840  .....8.@.......@
 00000c90: 0000 0000 0028 0a40 33b3 1068 2039 0940  .....(.@3..h 9.@
 00000ca0: 0000 0000 004d 0540 0000 0000 005d 0c40  .....M.@.....].@
 00000cb0: 3333 873c 1234 0f40 0000 0000 803e 0540  33.<.4.@.....>.@
 00000cc0: 0000 0000 80a4 0440 0000 0000 0050 0640  .......@.....P.@
 00000cd0: 0000 0000 8071 0a40 0000 0000 006c 1240  .....q.@.....l.@
-00000ce0: 0000 0000 80df 0d40 cf4c 430d 7366 0f40  .......@.LC.sf.@
+00000ce0: 0000 0000 80df 0d40 ce4c 430d 7366 0f40  .......@.LC.sf.@
 00000cf0: 6741 7224 68e1 0440 0000 0000 8081 0640  gAr$h..@.......@
 00000d00: cdcc ccb4 a5b7 0440 0000 0000 0037 0940  .......@.....7.@
 00000d10: 0000 0000 00ad 0340 0000 0000 003c 0640  .......@.....<.@
 00000d20: 0000 0000 8006 0640 0000 0000 80e0 1140  .......@.......@
 00000d30: 0000 0000 8014 0d40 b71e 44cd 43ed 0240  .......@..D.C..@
 00000d40: cfa1 c2d2 cda7 0840 2bc3 fe53 ae9f 0e40  .......@+..S...@
 00000d50: 0000 0000 00e5 0840 329b e343 7c33 0d40  .......@2..C|3.@
@@ -220,21 +220,21 @@
 00000db0: 0000 0000 80b8 0a40 0000 0000 0094 0a40  .......@.......@
 00000dc0: 0000 0000 805a 0940 0000 0000 003c 0a40  .....Z.@.....<.@
 00000dd0: 0000 0000 80d7 0840 0000 0000 806b 0b40  .......@.....k.@
 00000de0: 33b3 fa41 094c 0840 0000 0000 80c7 0440  3..A.L.@.......@
 00000df0: 0000 0000 8085 0b40 9999 6471 9c87 0e40  .......@..dq...@
 00000e00: 0000 0000 00db 0540 0000 0000 80ee 0440  .......@.......@
 00000e10: 0000 0000 00f0 0640 0000 0000 80e5 0a40  .......@.......@
-00000e20: 0000 0000 809b 1240 2d01 9856 3e0d 0f40  .......@-..V>..@
+00000e20: 0000 0000 809b 1240 2e01 9856 3e0d 0f40  .......@...V>..@
 00000e30: 0000 0000 801f 1040 9aa3 9162 9ed9 0440  .......@...b...@
 00000e40: 0000 0000 0083 0640 cdcc ccfc d7dc 0440  .......@.......@
 00000e50: 0000 0000 00d1 0840 0000 0000 8043 0340  .......@.....C.@
 00000e60: 0000 0000 80bc 0540 0000 0000 0019 0640  .......@.......@
 00000e70: 0000 0000 40cd 1140 0000 0000 0078 0d40  ....@..@.....x.@
-00000e80: b4d5 2dbf 9866 0a40 7a92 acc2 b5df 1140  ..-..f.@z......@
+00000e80: b6d5 2dbf 9866 0a40 7a92 acc2 b5df 1140  ..-..f.@z......@
 00000e90: b943 df1a 542b 0e40 0000 0000 80d4 0840  .C..T+.@.......@
 00000ea0: 0000 0000 802d 0d40 0000 0000 8060 0440  .....-.@.....`.@
 00000eb0: 0000 0000 809c 0540 3333 33cb a927 0940  .......@333..'.@
 00000ec0: 0000 0000 8077 0740 0000 0000 00d1 0b40  .....w.@.......@
 00000ed0: 6666 22fa f1be 0a40 3333 339b 7164 0d40  ff"....@333.qd.@
 00000ee0: 0000 0000 800a 0740 3333 334b 6fb0 0840  .......@333Ko..@
 00000ef0: 6766 8435 7bca 0840 0000 0000 0038 0a40  gf.5{..@.....8.@
@@ -246,16 +246,16 @@
 00000f50: 0000 0000 8014 0540 0000 0000 8073 0740  .......@.....s.@
 00000f60: 0000 0000 0059 0b40 4888 6c37 4acb 1240  .....Y.@H.l7J..@
 00000f70: 51bc e101 034e 1040 0000 0000 00a1 1040  Q....N.@.......@
 00000f80: 4def 4e18 e6e8 0440 0000 0000 0074 0640  M.N....@.....t.@
 00000f90: cdcc cc7c 6e66 0540 cdcc 88ed c176 0840  ...|nf.@.....v.@
 00000fa0: 0000 0000 80d9 0240 0000 0000 8058 0540  .......@.....X.@
 00000fb0: 0000 0000 804d 0640 0000 0000 40ab 1140  .....M.@....@..@
-00000fc0: 0000 0000 00ee 0d40 6fd7 d0e0 6579 0b40  .......@o...ey.@
-00000fd0: 2684 a729 6d4f 1240 e9f0 0efa 8413 1140  &..)mO.@.......@
+00000fc0: 0000 0000 00ee 0d40 6dd7 d0e0 6579 0b40  .......@m...ey.@
+00000fd0: 2684 a729 6d4f 1240 e8f0 0efa 8413 1140  &..)mO.@.......@
 00000fe0: 0000 0000 00c2 0840 6634 d6e1 89c1 0c40  .......@f4.....@
 00000ff0: 1a8f 8ef8 5997 0340 0000 0000 0033 0640  ....Y..@.....3.@
 00001000: 3333 3373 a9c9 0840 0000 0000 0069 0740  333s...@.....i.@
 00001010: 0000 0000 00ee 0b40 0000 0000 80ba 0a40  .......@.......@
 00001020: 0000 0000 80df 0c40 0000 0000 00de 0640  .......@.......@
 00001030: 3333 333b 6ed6 0840 cdcc 60ab 230b 0840  333;n..@..`.#..@
 00001040: 0000 0000 80ce 0940 0000 0000 00cb 0a40  .......@.......@
@@ -267,15 +267,15 @@
 000010a0: 0000 0000 80d7 0740 0000 0000 80c3 0b40  .......@.......@
 000010b0: eb70 8077 bceb 1240 eac0 42ac 2f05 1040  .p.w...@..B./..@
 000010c0: 0040 14fb 0d95 1040 1a85 19d1 c30a 0540  .@.....@.......@
 000010d0: 0000 0000 005d 0640 0000 0000 000a 0640  .....].@.......@
 000010e0: cdcc 6f83 1bfc 0740 0000 0000 0077 0240  ..o....@.....w.@
 000010f0: 0000 0000 8016 0540 0000 0000 80a4 0640  .......@.......@
 00001100: 0000 0000 4076 1140 0000 0000 8067 0e40  ....@v.@.....g.@
-00001110: 76d2 21cb 062a 0940 9c4b 1f7b 9230 0a40  v.!..*.@.K.{.0.@
+00001110: 7ad2 21cb 062a 0940 9e4b 1f7b 9230 0a40  z.!..*.@.K.{.0.@
 00001120: 9ef9 1bb0 b1c1 1440 0000 0000 00b2 0840  .......@.......@
 00001130: cf4c 0f38 7427 0140 3446 7057 abd4 0240  .L.8t'.@4FpW...@
 00001140: 0000 0000 80c8 0640 0000 0000 8045 0840  .......@.....E.@
 00001150: 0000 0000 0064 0740 0000 0000 8022 0c40  .....d.@.....".@
 00001160: 0000 0000 80ab 0a40 0000 0000 8041 0c40  .......@.....A.@
 00001170: 0000 0000 00be 0640 0000 0000 00da 0840  .......@.......@
 00001180: cd4c b9bc 09b1 0740 0000 0000 006f 0940  .L.....@.....o.@
@@ -308,132 +308,132 @@
 00001330: 0000 0000 804c 0840 0000 0000 807d 0c40  .....L.@.....}.@
 00001340: a87a 7679 f2e9 1240 2e6f 4fc9 9c3b 1640  .zvy...@.oO..;.@
 00001350: 3233 73bf ae91 1840 0000 0000 8031 0540  23s....@.....1.@
 00001360: 0000 0000 801d 0640 0000 0000 8098 0740  .......@.......@
 00001370: 6666 dafd 4007 0840 cdcc cc0c f8ee 0140  ff..@..@.......@
 00001380: 0000 0000 0007 0540 0000 0000 0084 0740  .......@.......@
 00001390: 0000 0000 c0dd 1040 0000 0000 0054 0f40  .......@.....T.@
-000013a0: 639c 076c e856 2540 8291 ff52 5a05 1f40  c..l.V%@...RZ..@
-000013b0: bea4 5274 c578 1540 0000 0000 00aa 0840  ..Rt.x.@.......@
+000013a0: 629c 076c e856 2540 8491 ff52 5a05 1f40  b..l.V%@...RZ..@
+000013b0: c0a4 5274 c578 1540 0000 0000 00aa 0840  ..Rt.x.@.......@
 000013c0: 675c 5fb4 2638 0a40 7fd6 83dd 91aa 0140  g\_.&8.@.......@
 000013d0: 0000 0000 00c3 0740 0000 0000 80e2 0640  .......@.......@
 000013e0: 0000 0000 0084 0740 0000 0000 00ed 0c40  .......@.......@
 000013f0: 0000 0000 0048 0a40 0000 0000 00a8 0a40  .....H.@.......@
 00001400: 0000 0000 808a 0640 0000 0000 8087 0840  .......@.......@
 00001410: cd4c 95ce 291a 0840 0000 0000 80ad 0840  .L..)..@.......@
 00001420: 0000 0000 002c 0b40 b7f6 0d5e a329 0d40  .....,.@...^.).@
 00001430: 0000 0000 8037 0e40 0000 0000 0099 0840  .....7.@.......@
 00001440: 9999 993d 1c5e 1040 cdcc 87f3 cbc6 0240  ...=.^.@.......@
 00001450: 0000 0000 001e 0440 cdcc ccbc d371 0840  .......@.....q.@
 00001460: 0000 0000 809c 0940 0000 0000 00d1 0940  .......@.......@
 00001470: 0000 0000 8003 0440 0000 0000 0072 0840  .......@.....r.@
 00001480: 0000 0000 00d2 0c40 24d7 c507 7eb6 1240  .......@$...~..@
-00001490: 4ca4 c5d8 4680 0e40 d28a d7f4 d2c8 1140  L...F..@.......@
+00001490: 4da4 c5d8 4680 0e40 d28a d7f4 d2c8 1140  M...F..@.......@
 000014a0: 0000 0000 005c 0540 0000 0000 8007 0640  .....\.@.......@
 000014b0: 0000 0000 8060 0840 6766 2e16 26ac 0840  .....`.@gf..&..@
 000014c0: cdcc cca4 12cf 0140 0000 0000 0039 0540  .......@.....9.@
 000014d0: 0000 0000 00f6 0740 0000 0000 807c 1040  .......@.....|.@
-000014e0: 0000 0000 00ca 0f40 048d 9c41 ae30 f53f  .......@...A.0.?
-000014f0: 622b c571 0828 1b40 baf7 7eba b416 1140  b+.q.(.@..~....@
+000014e0: 0000 0000 00ca 0f40 088d 9c41 ae30 f53f  .......@...A.0.?
+000014f0: 602b c571 0828 1b40 bbf7 7eba b416 1140  `+.q.(.@..~....@
 00001500: 0000 0000 80c0 0840 9a91 70d3 6275 0940  .......@..p.bu.@
 00001510: 191e b50f 8942 0140 0000 0000 801a 0840  .....B.@.......@
 00001520: 0000 0000 0016 0640 0000 0000 80be 0740  .......@.......@
 00001530: 0000 0000 0080 0d40 0000 0000 00f1 0940  .......@.......@
 00001540: 0000 0000 00c0 0940 0000 0000 0079 0640  .......@.....y.@
 00001550: 0000 0000 003d 0840 0000 0000 0091 0840  .....=.@.......@
 00001560: 0000 0000 0049 0840 0000 0000 005a 0b40  .....I.@.....Z.@
 00001570: 096f dd12 801a 0d40 0000 0000 8093 0e40  .o.....@.......@
 00001580: 0000 0000 00d7 0840 9999 9949 ef95 1040  .......@...I...@
-00001590: 9a99 cbcb 20fc 0140 0000 0000 8076 0440  .... ..@.....v.@
+00001590: 9b99 cbcb 20fc 0140 0000 0000 8076 0440  .... ..@.....v.@
 000015a0: cdcc cc7c cc15 0840 0000 0000 8004 0940  ...|...@.......@
 000015b0: 0000 0000 00dd 0a40 0000 0000 8076 0340  .......@.....v.@
-000015c0: 0000 0000 0093 0840 1747 4f15 f014 0d40  .......@.GO....@
+000015c0: 0000 0000 0093 0840 1647 4f15 f014 0d40  .......@.GO....@
 000015d0: cb70 b379 64ac 1240 6f88 1873 3f0b 0f40  .p.yd..@o..s?..@
 000015e0: 912c e9a0 7753 1240 0000 0000 0092 0540  .,..wS.@.......@
 000015f0: 0000 0000 800e 0640 3333 6662 6d40 0940  .......@33fbm@.@
 00001600: cdcc cd07 a4b9 0940 cdcc cc14 06e9 0140  .......@.......@
 00001610: 0000 0000 8086 0540 0000 0000 805a 0840  .......@.....Z.@
 00001620: 0000 0000 c00e 1040 0000 0000 0023 1040  .......@.....#.@
-00001630: a5a8 968d 3998 0a40 4ab9 1be3 be01 1540  ....9..@J......@
-00001640: 79a5 2f74 f349 1040 cdcc cc1c 23d9 0840  y./t.I.@....#..@
-00001650: 665e 6a15 3922 0a40 9288 f494 690d 0140  f^j.9".@....i..@
+00001630: a3a8 968d 3998 0a40 4ab9 1be3 be01 1540  ....9..@J......@
+00001640: 7aa5 2f74 f349 1040 cdcc cc1c 23d9 0840  z./t.I.@....#..@
+00001650: 675e 6a15 3922 0a40 9288 f494 690d 0140  g^j.9".@....i..@
 00001660: 0000 0000 005a 0840 0000 0000 8053 0540  .....Z.@.....S.@
 00001670: 0000 0000 0019 0840 0000 0000 002c 0e40  .......@.....,.@
 00001680: 0000 0000 807e 0940 0000 0000 80d4 0840  .....~.@.......@
 00001690: 0000 0000 806c 0640 0000 0000 00ec 0740  .....l.@.......@
 000016a0: 0000 0000 00f4 0840 0000 0000 80e4 0740  .......@.......@
 000016b0: 0000 0000 00a3 0b40 0000 0000 0000 0d40  .......@.......@
 000016c0: 0000 0000 80d7 0e40 0000 0000 0046 0940  .......@.....F.@
 000016d0: 9999 99cd a9a4 1040 0200 70d4 ca7e f73f  .......@..p..~.?
 000016e0: 0000 0000 80e7 0440 cdcc cc44 c6eb 0740  .......@...D...@
 000016f0: 0000 0000 00aa 0840 0000 0000 00f8 0b40  .......@.......@
 00001700: 0000 0000 80e4 0240 0000 0000 00b4 0840  .......@.......@
-00001710: 8a1f 80b7 c74c 0d40 6876 04a2 13c1 1240  .....L.@hv.....@
+00001710: 8a1f 80b7 c74c 0d40 6976 04a2 13c1 1240  .....L.@iv.....@
 00001720: 2ad6 6edc cc70 0e40 5efe 0307 0add 1140  *.n..p.@^......@
 00001730: 0000 0000 80d0 0540 0000 0000 0032 0640  .......@.....2.@
 00001740: 3333 7ddf d7f0 0940 cdcc 7ce2 d126 0b40  33}....@..|..&.@
 00001750: cdcc cc14 2d3e 0240 0000 0000 80e1 0540  ....->.@.......@
 00001760: 0000 0000 00ae 0840 0000 0000 802c 0f40  .......@.....,.@
-00001770: 0000 0000 c067 1040 d004 a664 c15f 0540  .....g.@...d._.@
+00001770: 0000 0000 c067 1040 d404 a664 c15f 0540  .....g.@...d._.@
 00001780: 70e6 c33e b5e6 1440 2d51 bcc0 aa9f 1040  p..>...@-Q.....@
 00001790: cdcc ccec d611 0940 0000 0000 0072 0a40  .......@.....r.@
-000017a0: 7bc7 ef29 b131 0140 0000 0000 808e 0840  {..).1.@.......@
+000017a0: 7ac7 ef29 b131 0140 0000 0000 808e 0840  z..).1.@.......@
 000017b0: 0000 0000 00a8 0440 0000 0000 8089 0840  .......@.......@
 000017c0: 0000 0000 80e9 0e40 0000 0000 00ed 0840  .......@.......@
 000017d0: 0000 0000 80f6 0740 0000 0000 8060 0640  .......@.....`.@
 000017e0: 0000 0000 0095 0740 0000 0000 805e 0940  .......@.....^.@
 000017f0: 0000 0000 007d 0740 0000 0000 000a 0c40  .....}.@.......@
 00001800: 0000 0000 00df 0c40 0000 0000 8014 0f40  .......@.......@
 00001810: 0000 0000 80e2 0940 9999 997d d687 1040  .......@...}...@
 00001820: 0400 109a d046 f63f 0000 0000 805f 0540  .....F.?....._.@
 00001830: cdcc ccdc 3103 0840 0000 0000 0082 0840  ....1..@.......@
 00001840: 0000 0000 0019 0d40 0000 0000 0061 0240  .......@.....a.@
 00001850: 0000 0000 80d4 0840 ddd8 a8d6 14bc 0d40  .......@.......@
-00001860: e79c efee 1f10 1240 762a f9de a8bb 0240  .......@v*.....@
+00001860: e89c efee 1f10 1240 772a f9de a8bb 0240  .......@w*.....@
 00001870: 0000 0000 c0ad 1140 0000 0000 0019 0640  .......@.......@
 00001880: 0000 0000 0070 0640 0080 5e39 bd39 0a40  .....p.@..^9.9.@
 00001890: 0000 0000 0088 0c40 0000 0000 00bd 0240  .......@.......@
 000018a0: 0000 0000 0048 0640 0000 0000 00e5 0840  .....H.@.......@
 000018b0: 0000 0000 802a 0e40 0000 0000 80b9 1040  .....*.@.......@
-000018c0: 33ac 2371 0198 0040 de1f 4fe0 61fa 1240  3.#q...@..O.a..@
+000018c0: 34ac 2371 0198 0040 de1f 4fe0 61fa 1240  4.#q...@..O.a..@
 000018d0: c7ea 696c cdec 0a40 cdcc cc6c 1b7f 0940  ..il...@...l...@
-000018e0: 0000 0000 00b2 0a40 6a36 c8a0 0cde fd3f  .......@j6.....?
+000018e0: 0000 0000 00b2 0a40 6836 c8a0 0cde fd3f  .......@h6.....?
 000018f0: 0000 0000 00c3 0840 cdcc cc9c 9602 0440  .......@.......@
 00001900: 0000 0000 0007 0940 0000 0000 80a7 0f40  .......@.......@
 00001910: 0000 0000 0038 0840 0000 0000 0027 0740  .....8.@.....'.@
 00001920: 0000 0000 8047 0640 0000 0000 0044 0740  .....G.@.....D.@
 00001930: 0000 0000 00c2 0940 0000 0000 000f 0740  .......@.......@
 00001940: 0000 0000 8083 0c40 0000 0000 00c3 0c40  .......@.......@
 00001950: 0000 0000 8055 0f40 0000 0000 80a3 0a40  .....U.@.......@
 00001960: 9999 99e1 c046 1040 9a99 4f30 268c 0240  .....F.@..O0&..@
 00001970: 0000 0000 00cf 0540 cdcc cc0c 3b60 0840  .......@....;`.@
 00001980: 0000 0000 0084 0840 0000 0000 0034 0e40  .......@.....4.@
 00001990: 0000 0000 00f9 0140 0000 0000 80f5 0840  .......@.......@
-000019a0: d716 0f2b 8a87 0e40 b81a 72ef cb0a 0f40  ...+...@..r....@
-000019b0: 6250 8fd4 2482 fc3f 0000 0000 0080 1140  bP..$..?.......@
+000019a0: d716 0f2b 8a87 0e40 b61a 72ef cb0a 0f40  ...+...@..r....@
+000019b0: 6450 8fd4 2482 fc3f 0000 0000 0080 1140  dP..$..?.......@
 000019c0: 0000 0000 0076 0640 0000 0000 80c9 0640  .....v.@.......@
 000019d0: 3333 2d06 bd0a 0a40 0000 0000 80db 0d40  33-....@.......@
 000019e0: 0000 0000 005f 0340 0000 0000 80b5 0640  ....._.@.......@
 000019f0: 0000 0000 00f8 0840 0000 0000 8022 0d40  .......@.....".@
-00001a00: 0000 0000 801e 1140 6cbb c8bd 19fe f83f  .......@l......?
-00001a10: 1903 90bc 0332 0d40 5259 cdf2 d986 0740  .....2.@RY.....@
+00001a00: 0000 0000 801e 1140 6abb c8bd 19fe f83f  .......@j......?
+00001a10: 1903 90bc 0332 0d40 5359 cdf2 d986 0740  .....2.@SY.....@
 00001a20: cdcc cc4c 2b2d 0a40 0000 0000 80fd 0a40  ...L+-.@.......@
 00001a30: 38c3 8566 a880 fc3f 0000 0000 8000 0940  8..f...?.......@
 00001a40: cdcc ccec e288 0340 0000 0000 8095 0940  .......@.......@
 00001a50: 66e6 332a 7d3f 1040 0000 0000 0065 0740  f.3*}?.@.....e.@
 00001a60: 0000 0000 0068 0640 0000 0000 8021 0640  .....h.@.....!.@
 00001a70: 0000 0000 80fb 0640 0000 0000 000c 0a40  .......@.......@
 00001a80: 0000 0000 8099 0640 0000 0000 8002 0d40  .......@.......@
 00001a90: 530e cf5d d497 0d40 0000 0000 009d 0f40  S..]...@.......@
 00001aa0: 0000 0000 0073 0b40 3333 335b 76d6 0f40  .....s.@333[v..@
 00001ab0: cdcc 319e de5a 0340 0000 0000 0025 0640  ..1..Z.@.....%.@
 00001ac0: 0000 0000 00d4 0840 0000 0000 80a4 0840  .......@.......@
 00001ad0: 3333 337b 8a48 0f40 0000 0000 80b6 0140  333{.H.@.......@
 00001ae0: 0000 0000 801c 0940 b754 768a fbb1 0f40  .......@.Tv....@
-00001af0: 5be7 b7ff 57ec 0d40 6157 ba79 f7cd 0040  [...W..@aW.y...@
+00001af0: 5be7 b7ff 57ec 0d40 6257 ba79 f7cd 0040  [...W..@bW.y...@
 00001b00: 0000 0000 c051 1140 0000 0000 00e3 0640  .....Q.@.......@
 00001b10: 0000 0000 803e 0740 6666 0c7c ae60 0940  .....>.@ff.|.`.@
 00001b20: 0000 0000 801f 0f40 0000 0000 8025 0440  .......@.....%.@
 00001b30: 0000 0000 8029 0740 0000 0000 00e1 0840  .....).@.......@
 00001b40: 0000 0000 0021 0c40 0000 0000 8098 1140  .....!.@.......@
 00001b50: 5601 745d 27dd fc3f 33d8 2fe4 8242 0840  V.t]'..?3./..B.@
 00001b60: a590 ecda 72d3 0540 cdcc cc7c a625 0b40  ....r..@...|.%.@
@@ -448,402 +448,402 @@
 00001bf0: 0000 0000 00fc 0e40 0000 0000 009e 0440  .......@.......@
 00001c00: 0000 0000 8053 0640 0000 0000 006e 0940  .....S.@.....n.@
 00001c10: 0000 0000 00cc 0840 9999 9961 9c32 1040  .......@...a.2.@
 00001c20: 0000 0000 0098 0140 0000 0000 0048 0940  .......@.....H.@
 00001c30: 672e 7f6f 0ca0 1040 f6ab 0b72 ec04 0c40  g..o...@...r...@
 00001c40: 095b fac0 55fa 0740 0000 0000 c022 1140  .[..U..@.....".@
 00001c50: 0000 0000 8058 0740 0000 0000 00cd 0740  .....X.@.......@
-00001c60: 3333 1f6f 0149 0840 cdcc faec 9f63 1040  33.o.I.@.....c.@
+00001c60: 3333 1f6f 0149 0840 cccc faec 9f63 1040  33.o.I.@.....c.@
 00001c70: 0000 0000 80ff 0440 0000 0000 00a9 0740  .......@.......@
 00001c80: 0000 0000 00a5 0840 0000 0000 0033 0b40  .......@.....3.@
 00001c90: 0000 0000 0022 1240 d80a 97f7 7ba1 0540  .....".@....{..@
-00001ca0: 8d07 51c5 4d49 0740 f90b effd 6a08 0740  ..Q.MI.@....j..@
+00001ca0: 8f07 51c5 4d49 0740 f60b effd 6a08 0740  ..Q.MI.@....j..@
 00001cb0: 0000 0000 804c 0c40 0000 0000 807e 0b40  .....L.@.....~.@
-00001cc0: d00e f3e3 1a79 0940 0000 0000 00d3 0940  .....y.@.......@
+00001cc0: d10e f3e3 1a79 0940 0000 0000 00d3 0940  .....y.@.......@
 00001cd0: cdcc cc74 1d86 0340 0000 0000 80e8 0a40  ...t...@.......@
 00001ce0: 99d9 0a04 42e4 1040 0000 0000 0089 0540  ....B..@.......@
 00001cf0: 0000 0000 0035 0540 0000 0000 00f1 0540  .....5.@.......@
 00001d00: 0000 0000 009d 0640 0000 0000 801f 0a40  .......@.......@
 00001d10: 0000 0000 80d1 0540 7d8b 806e 8d0f 0e40  .......@}..n...@
 00001d20: 2135 64c8 af78 0d40 0000 0000 001f 1040  !5d..x.@.......@
 00001d30: 3333 334b 810b 0d40 0000 0000 0039 0e40  333K...@.....9.@
 00001d40: 0000 0000 0091 0540 0000 0000 8054 0640  .......@.....T.@
 00001d50: 0000 0000 8025 0a40 0000 0000 80e8 0840  .....%.@.......@
 00001d60: 9999 991d dea8 1040 0000 0000 809b 0140  .......@.......@
 00001d70: 0000 0000 8072 0940 808c 2e66 e09d 1140  .....r.@...f...@
-00001d80: 6103 c0bb 7544 0b40 905a f629 a59a 1240  a...uD.@.Z.)...@
+00001d80: 6303 c0bb 7544 0b40 935a f629 a59a 1240  c...uD.@.Z.)...@
 00001d90: 0000 0000 80f5 1040 0000 0000 00c8 0740  .......@.......@
 00001da0: 0000 0000 0070 0840 0000 0000 80ef 0640  .....p.@.......@
 00001db0: 0000 0c91 9daf 1040 0000 0000 80d7 0540  .......@.......@
 00001dc0: 0000 0000 8035 0840 0000 0000 0048 0840  .....5.@.....H.@
 00001dd0: 0000 0000 005d 0a40 0000 0000 c0b0 1240  .....].@.......@
-00001de0: 329f 1e30 2de7 0e40 df7f c2c8 9dbe 0940  2..0-..@.......@
-00001df0: 25e7 1f38 b765 0c40 0000 0000 8084 0d40  %..8.e.@.......@
+00001de0: 349f 1e30 2de7 0e40 e07f c2c8 9dbe 0940  4..0-..@.......@
+00001df0: 21e7 1f38 b765 0c40 0000 0000 8084 0d40  !..8.e.@.......@
 00001e00: 0000 0000 00a3 0b40 9ad1 b84b 227d 0b40  .......@...K"}.@
 00001e10: 0000 0000 007b 0a40 cdcc ccac daed 0340  .....{.@.......@
 00001e20: 0000 0000 809d 0b40 cccc 66cf 52f3 1040  .......@..f.R..@
 00001e30: 0000 0000 009c 0440 0000 0000 80d8 0440  .......@.......@
 00001e40: ffff ffef 923c 0640 0000 0000 008f 0640  .....<.@.......@
 00001e50: 0000 0000 80e1 0940 0000 0000 808e 0540  .......@.......@
 00001e60: 6dfb 4f3c 2b9c 0e40 0000 0000 8003 0d40  m.O<+..@.......@
 00001e70: b133 b7dc 0745 1040 3333 336b 14b8 0d40  .3...E.@333k...@
 00001e80: 0000 0000 805d 0d40 0000 0000 8088 0640  .....].@.......@
 00001e90: 0000 0000 801f 0640 0000 0000 80e6 0a40  .......@.......@
 00001ea0: 0000 0000 80e2 0840 9999 9939 c701 1140  .......@...9...@
 00001eb0: 0000 0000 00bc 0140 0000 0000 8096 0940  .......@.......@
 00001ec0: 0000 0000 c094 1240 4e31 5bb7 78c0 f93f  .......@N1[.x..?
-00001ed0: fa0a c4af 4a84 1340 0000 0000 80c7 1040  ....J..@.......@
+00001ed0: fc0a c4af 4a84 1340 0000 0000 80c7 1040  ....J..@.......@
 00001ee0: 0000 0000 802c 0840 0000 0000 0019 0940  .....,.@.......@
 00001ef0: 0000 0000 00c0 0540 6666 26ed 0991 1740  .......@ff&....@
 00001f00: 0000 0000 8098 0640 0000 0000 00c8 0840  .......@.......@
 00001f10: 0000 0000 80d0 0740 0000 0000 00a4 0940  .......@.......@
-00001f20: 8d3d d45a 9636 1340 77df 2aef a37c 1440  .=.Z.6.@w.*..|.@
-00001f30: ab10 5074 1db9 0740 36df e80d 794a 1340  ..Pt...@6...yJ.@
+00001f20: 8d3d d45a 9636 1340 78df 2aef a37c 1440  .=.Z.6.@x.*..|.@
+00001f30: ae10 5074 1db9 0740 36df e80d 794a 1340  ..Pt...@6...yJ.@
 00001f40: 0000 0000 00da 0e40 0000 0000 00a9 0b40  .......@.......@
 00001f50: f80b d255 8425 0d40 0000 0000 004a 0b40  ...U.%.@.....J.@
 00001f60: 0000 0000 0086 0440 0000 0000 8042 0c40  .......@.....B.@
 00001f70: 9999 5819 38cc 1040 0000 0000 00bc 0340  ..X.8..@.......@
 00001f80: 0000 0000 00a1 0440 9e99 9959 9da2 fc3f  .......@...Y...?
 00001f90: 0000 0000 8095 0640 0000 0000 0078 0940  .......@.....x.@
 00001fa0: 0000 0000 805d 0540 ce1f 9af1 63e8 0e40  .....].@....c..@
 00001fb0: 861d d369 e850 0d40 31ca 9ba1 5a98 1040  ...i.P.@1...Z..@
 00001fc0: 3333 33a3 c8fc 0d40 0000 0000 0072 0c40  333....@.....r.@
 00001fd0: cdcc 0808 1779 0740 0000 0000 80bb 0540  .....y.@.......@
 00001fe0: 0000 0000 009a 0b40 0000 0000 80ac 0840  .......@.......@
 00001ff0: 9999 9911 3234 1140 0000 0000 00f3 0140  ....24.@.......@
 00002000: 0000 0000 00b6 0940 50e3 5b72 3238 1340  .......@P.[r28.@
-00002010: b3cd 7c69 c3de 1240 ed90 5ed5 ac51 1540  ..|i...@..^..Q.@
+00002010: b2cd 7c69 c3de 1240 ec90 5ed5 ac51 1540  ..|i...@..^..Q.@
 00002020: 0000 0000 c09b 1040 0000 0000 007f 0840  .......@.......@
 00002030: 0000 0000 80b6 0940 0000 0000 008c 0440  .......@.......@
 00002040: cc4c a279 f90f 1140 0000 0000 8038 0740  .L.y...@.....8.@
 00002050: 0000 0000 8064 0940 0000 0000 8048 0740  .....d.@.....H.@
 00002060: 0000 0000 0007 0940 9a4d 7cad 232d 1440  .......@.M|.#-.@
 00002070: 44a4 11b2 536d 1740 8eeb 2fd7 7cb6 1340  D...Sm.@../.|..@
-00002080: 0a91 a286 3adf 1340 0000 0000 c022 1040  ....:..@.....".@
+00002080: 0b91 a286 3adf 1340 0000 0000 c022 1040  ....:..@.....".@
 00002090: 0000 0000 0090 0b40 267e 6d76 93f0 1340  .......@&~mv...@
 000020a0: 0000 0000 003b 0c40 0000 0000 0020 0540  .....;.@..... .@
 000020b0: ffff b089 2ffb 0c40 6666 98a6 8b70 1040  ..../..@ff...p.@
 000020c0: cdcc cc8c 4df2 0240 0000 0000 808b 0440  ....M..@.......@
 000020d0: ffff ff0f fbbc 0640 0000 0000 80a6 0640  .......@.......@
 000020e0: 0000 0000 80e5 0840 0000 0000 803c 0540  .......@.....<.@
 000020f0: 320b cd78 a0d8 0e40 a091 fe57 57f7 0c40  2..x...@...WW..@
-00002100: 9acb 4e1c 1c53 1040 3333 33fb 8cd5 0d40  ..N..S.@333....@
+00002100: 99cb 4e1c 1c53 1040 3333 33fb 8cd5 0d40  ..N..S.@333....@
 00002110: 0000 0000 0089 0b40 33b3 b7a2 8770 0840  .......@3....p.@
 00002120: 0000 0000 0033 0540 3333 3363 6d46 0c40  .....3.@333cmF.@
 00002130: 0000 0000 0044 0840 9999 9971 443b 1140  .....D.@...qD;.@
 00002140: 0000 0000 803e 0240 0000 0000 00d4 0940  .....>.@.......@
 00002150: bd2f cde0 b0b2 1440 e8a5 7d94 6147 1640  ./.....@..}.aG.@
 00002160: 4168 b814 3996 1b40 0000 0000 006d 1040  Ah..9..@.....m.@
 00002170: 0000 0000 00bd 0840 0000 0000 0042 0a40  .......@.....B.@
 00002180: 3333 319f 4338 0340 0000 14c8 2a32 1140  331.C8.@....*2.@
 00002190: 3333 3363 75bd 0740 0000 0000 800f 0a40  333cu..@.......@
 000021a0: 0000 0000 00b4 0640 0000 0000 0089 0840  .......@.......@
-000021b0: 3369 1f27 2434 1440 e8d4 f6f6 252f 1f40  3i.'$4.@....%/.@
-000021c0: 404c 6620 411f 1740 0ba4 e0e8 7f14 1440  @Lf A..@.......@
+000021b0: 3369 1f27 2434 1440 ead4 f6f6 252f 1f40  3i.'$4.@....%/.@
+000021c0: 3e4c 6620 411f 1740 0ca4 e0e8 7f14 1440  >Lf A..@.......@
 000021d0: 0000 0000 40d7 1040 0000 0000 0055 0b40  ....@..@.....U.@
 000021e0: cc17 44e9 e68d 1840 0000 0000 8039 0d40  ..D....@.....9.@
 000021f0: 0000 0000 80d0 0540 3333 e474 238d 0d40  .......@33.t#..@
 00002200: 33b3 669c f4c5 0f40 cdcc cc54 0022 0240  3.f....@...T.".@
 00002210: 0000 0000 808f 0440 0000 0000 80dd 0640  .......@.......@
 00002220: 0000 0000 80ca 0640 0000 0000 8039 0840  .......@.....9.@
 00002230: 0000 0000 0030 0540 f2c9 2459 5f5b 0e40  .....0.@..$Y_[.@
-00002240: f02e 70b2 a329 1440 34bf 5e58 2497 1640  ..p..).@4.^X$..@
+00002240: f12e 70b2 a329 1440 34bf 5e58 2497 1640  ..p..).@4.^X$..@
 00002250: 3333 3313 7d45 0d40 0000 0000 80b2 0a40  333.}E.@.......@
 00002260: 33b3 7928 d922 0940 0000 0000 8095 0440  3.y(.".@.......@
 00002270: 3333 3323 41c1 0c40 0000 0000 80b1 0740  333#A..@.......@
 00002280: 9999 9969 9014 1140 0000 0000 8098 0240  ...i...@.......@
-00002290: 0000 0000 80f3 0940 ed0a 9636 00e8 1440  .......@...6...@
+00002290: 0000 0000 80f3 0940 ee0a 9636 00e8 1440  .......@...6...@
 000022a0: cbee e44b bff0 2c40 3be7 3c34 2070 2040  ...K..,@;.<4 p @
 000022b0: 0000 0000 803a 1040 0000 0000 00e6 0840  .....:.@.......@
 000022c0: 0000 0000 80b4 0a40 9919 3c7e 84e0 0140  .......@..<~...@
 000022d0: 0000 0000 c0d1 1040 3333 333b ab01 0840  .......@333;...@
 000022e0: 0000 0000 00c3 0a40 0000 0000 0020 0640  .......@..... .@
 000022f0: 0000 0000 002e 0840 0010 02ad f4d3 1a40  .......@.......@
-00002300: e712 523b b425 2440 e197 6f2b b327 3540  ..R;.%$@..o+.'5@
+00002300: e812 523b b425 2440 e197 6f2b b327 3540  ..R;.%$@..o+.'5@
 00002310: c831 28c8 04da 1e40 9999 9911 c987 1140  .1(....@.......@
 00002320: 0000 0000 00fa 0a40 b230 b1f3 befb 1840  .......@.0.....@
 00002330: 0000 0000 0031 0e40 0000 0000 008b 0640  .....1.@.......@
 00002340: 3333 0bb9 ebe4 0d40 3333 3dce 0053 0e40  33.....@33=..S.@
 00002350: cdcc ccb4 5e89 0140 0000 0000 00ac 0440  ....^..@.......@
 00002360: 0000 0000 8070 0740 0000 0000 80ff 0640  .....p.@.......@
 00002370: 0000 0000 0083 0740 0000 0000 803e 0540  .......@.....>.@
 00002380: b5f3 0864 af69 0d40 aa64 ddd5 1d78 1340  ...d.i.@.d...x.@
-00002390: 58a8 bd06 7520 1040 3333 33f3 cb58 0c40  X...u .@333..X.@
+00002390: 57a8 bd06 7520 1040 3333 33f3 cb58 0c40  W...u .@333..X.@
 000023a0: cd31 07bb 27e7 0940 3333 6b23 968f 0940  .1..'..@33k#...@
 000023b0: 0000 0000 00f0 0340 3333 333b d7d8 0c40  .......@333;...@
 000023c0: 0000 0000 80fa 0640 9999 9989 60c4 1040  .......@....`..@
 000023d0: 0000 0000 00fb 0240 3333 07d2 136f 0a40  .......@33...o.@
-000023e0: d8f6 0255 6d1f 1e40 3b97 e30d fbfa 2d40  ...Um..@;.....-@
-000023f0: 5795 2e6f bd43 2140 0000 0000 0008 1040  W..o.C!@.......@
+000023e0: daf6 0255 6d1f 1e40 3b97 e30d fbfa 2d40  ...Um..@;.....-@
+000023f0: 5695 2e6f bd43 2140 0000 0000 0008 1040  V..o.C!@.......@
 00002400: 0000 0000 00f2 0840 0000 0000 0008 0b40  .......@.......@
 00002410: 9e99 d930 7b7c f53f 0000 0000 80a3 1040  ...0{|.?.......@
 00002420: 0000 0000 00fa 0740 0000 0000 0077 0b40  .......@.....w.@
 00002430: 0000 0000 0096 0540 0000 0000 00f7 0740  .......@.......@
 00002440: cc28 3b6b f4c5 1b40 ad06 4114 31dc 3340  .(;k...@..A.1.3@
-00002450: ab35 a7d4 8b34 2840 c411 fac0 2df1 1f40  .5...4(@....-..@
+00002450: ab35 a7d4 8b34 2840 c611 fac0 2df1 1f40  .5...4(@....-..@
 00002460: 9999 9975 0932 1240 0000 0000 0084 0a40  ...u.2.@.......@
 00002470: a7f2 b03a 2e6d 1540 3333 33cb 0d32 0f40  ...:.m.@333..2.@
 00002480: 0000 0000 003e 0740 33b3 bb99 5bf4 0d40  .....>.@3...[..@
 00002490: 0000 0000 00fa 0c40 cdcc ccd4 0e32 0140  .......@.....2.@
 000024a0: 0000 0000 80d9 0440 0000 0000 0021 0840  .......@.....!.@
 000024b0: 0000 0000 8047 0740 0000 0000 00d8 0640  .....G.@.......@
 000024c0: 0000 0000 006d 0540 0000 0000 0005 0c40  .....m.@.......@
 000024d0: df02 0295 cbd1 0c40 0000 0000 c029 1040  .......@.....).@
 000024e0: 0000 0000 005d 0b40 4d97 6738 0705 0940  .....].@M.g8...@
 000024f0: 9999 e897 03af 0940 0000 0000 805a 0340  .......@.....Z.@
 00002500: 3333 33fb ef8c 0c40 0000 0000 8024 0640  333....@.....$.@
 00002510: 9999 992d e850 1040 0000 0000 8061 0340  ...-.P.@.....a.@
-00002520: ffbf 8e0f ea73 0a40 d28d 4078 c011 1f40  .....s.@..@x...@
+00002520: ffbf 8e0f ea73 0a40 d08d 4078 c011 1f40  .....s.@..@x...@
 00002530: 7cde 9771 5059 1940 f89e 02f4 5fc7 1e40  |..qPY.@...._..@
-00002540: ecd0 6d6c 7b9b 0f40 0000 0000 80e5 0840  ..ml{..@.......@
+00002540: eed0 6d6c 7b9b 0f40 0000 0000 80e5 0840  ..ml{..@.......@
 00002550: 3333 33fb 2935 0b40 0100 34cb 8250 0040  333.)5.@..4..P.@
 00002560: 0000 0000 4073 1040 0000 0000 00ca 0740  ....@s.@.......@
 00002570: 0000 0000 0022 0c40 0000 0000 801a 0540  .....".@.......@
-00002580: 0000 0000 00de 0740 67b3 eadb 9800 1440  .......@g......@
-00002590: 2a21 2812 b07c 1f40 eaae d8fe 133c 1540  *!(..|.@.....<.@
+00002580: 0000 0000 00de 0740 66b3 eadb 9800 1440  .......@f......@
+00002590: 2a21 2812 b07c 1f40 e9ae d8fe 133c 1540  *!(..|.@.....<.@
 000025a0: 205c a2d7 7fd0 1540 9999 9925 2cad 1240   \.....@...%,..@
-000025b0: 0000 0000 00fb 0940 4009 4075 8dc0 1040  .......@@.@u...@
+000025b0: 0000 0000 00fb 0940 4109 4075 8dc0 1040  .......@A.@u...@
 000025c0: 9999 9989 a00b 1040 0000 0000 80d7 0740  .......@.......@
 000025d0: 0180 f92b 48ae 0d40 0000 0000 80aa 0b40  ...+H..@.......@
 000025e0: cdcc ccec c420 0140 0000 0000 800f 0540  ..... .@.......@
 000025f0: 0000 0000 00d2 0840 0000 0000 809f 0740  .......@.......@
 00002600: 0000 0000 004e 0640 0000 0000 80b5 0540  .....N.@.......@
-00002610: 4fb7 8b22 6e38 0b40 0000 0000 80d7 0c40  O.."n8.@.......@
-00002620: b612 14cc 8d6b 0f40 0000 0000 0061 0a40  .....k.@.....a.@
+00002610: 50b7 8b22 6e38 0b40 0000 0000 80d7 0c40  P.."n8.@.......@
+00002620: b512 14cc 8d6b 0f40 0000 0000 0061 0a40  .....k.@.....a.@
 00002630: 4da0 aa18 284b 0840 cd4c 6472 e483 0940  M...(K.@.Ldr...@
 00002640: 0000 0000 80e4 0240 3333 3353 afe3 0b40  .......@333S...@
 00002650: 0000 0000 003e 0540 3333 3343 c07f 0f40  .....>.@333C...@
 00002660: 0000 0000 00cf 0340 febf f275 173f 0e40  .......@...u.?.@
-00002670: 915c a093 fbb7 1540 6c69 5122 94ee 1740  .\.....@liQ"...@
-00002680: 54bd 33a5 c72c 1540 b343 1b16 9fab 0e40  T.3..,.@.C.....@
+00002670: 905c a093 fbb7 1540 6c69 5122 94ee 1740  .\.....@liQ"...@
+00002680: 54bd 33a5 c72c 1540 b443 1b16 9fab 0e40  T.3..,.@.C.....@
 00002690: 0000 0000 80ce 0840 0000 0000 003b 0b40  .......@.....;.@
-000026a0: cecc 1452 b3a8 0040 0000 0000 804a 1040  ...R...@.....J.@
+000026a0: cdcc 1452 b3a8 0040 0000 0000 804a 1040  ...R...@.....J.@
 000026b0: 0000 0000 0076 0740 0000 0000 00b4 0c40  .....v.@.......@
 000026c0: 0000 0000 00ad 0440 0000 0000 00d1 0740  .......@.......@
-000026d0: e6f3 51b1 280c 1440 9eb6 40bf bbc1 1840  ..Q.(..@..@....@
-000026e0: fa67 dc92 56f9 1540 0000 0000 402e 1740  .g..V..@....@..@
+000026d0: e6f3 51b1 280c 1440 a0b6 40bf bbc1 1840  ..Q.(..@..@....@
+000026e0: f867 dc92 56f9 1540 0000 0000 402e 1740  .g..V..@....@..@
 000026f0: 9999 9969 2cf9 1240 0000 0000 8067 0940  ...i,..@.....g.@
 00002700: 0000 0000 c068 1140 9999 9945 4951 1040  .....h.@...EIQ.@
 00002710: 0000 0000 8051 0840 6566 c82c 9407 0d40  .....Q.@ef.,...@
 00002720: 0180 7e1b c069 0a40 cdcc cc54 4251 0140  ..~..i.@...TBQ.@
 00002730: 0000 0000 003b 0540 0000 0000 806c 0940  .....;.@.....l.@
 00002740: 0000 0000 8005 0840 cdcc ccec bfcf 0540  .......@.......@
-00002750: 0000 0000 8018 0640 2370 2c97 51ff 0940  .......@#p,.Q..@
-00002760: c68f 3fe1 ba3a 0c40 142e 510a 8a2e 0e40  ..?..:.@..Q....@
+00002750: 0000 0000 8018 0640 2470 2c97 51ff 0940  .......@$p,.Q..@
+00002760: c68f 3fe1 ba3a 0c40 182e 510a 8a2e 0e40  ..?..:.@..Q....@
 00002770: 0000 0000 005c 0940 cd0d 11f0 69d0 0740  .....\.@....i..@
 00002780: 33b3 507f 9910 0940 cdcc ccdc 9493 0240  3.P....@.......@
 00002790: 0000 0000 8024 0b40 0000 0000 8054 0440  .....$.@.....T.@
 000027a0: 0000 0000 0051 0e40 0000 0000 8041 0440  .....Q.@.....A.@
 000027b0: 5833 e3ca 1b43 da3f 0000 0000 c06c 1640  X3...C.?.....l.@
 000027c0: 2cad c923 e655 1640 e74a 5e78 969b 1540  ,..#.U.@.J^x...@
-000027d0: b6a1 1a94 4bd2 0d40 0000 0000 80bd 0840  ....K..@.......@
+000027d0: b7a1 1a94 4bd2 0d40 0000 0000 80bd 0840  ....K..@.......@
 000027e0: 0000 0000 8016 0b40 34b3 752d c040 0140  .......@4.u-.@.@
 000027f0: 0100 3a40 0e2d 1040 0000 0000 8013 0740  ..:@.-.@.......@
 00002800: 0000 0000 0028 0d40 0000 0000 004c 0440  .....(.@.....L.@
 00002810: 0000 0000 00ca 0740 34d3 109d fb1c 1340  .......@4......@
-00002820: 31f9 47b8 9bd2 1940 858a 0ae4 9c1c 1240  1.G....@.......@
-00002830: ff91 6801 31bc 1640 9999 9911 4419 1340  ..h.1..@....D..@
+00002820: 30f9 47b8 9bd2 1940 868a 0ae4 9c1c 1240  0.G....@.......@
+00002830: 0192 6801 31bc 1640 9999 9911 4419 1340  ..h.1..@....D..@
 00002840: 0000 0000 00d5 0840 f5b9 c7d4 b0c2 1140  .......@.......@
 00002850: 9999 99ad 2d62 1040 0000 0000 00ab 0840  ....-b.@.......@
 00002860: 3333 2c59 a901 0c40 cdcc c400 f4b4 0840  33,Y...@.......@
 00002870: cdcc cc1c e4bd 0140 0000 0000 004a 0540  .......@.....J.@
 00002880: 3333 33af edf0 0940 0000 0000 007e 0840  333....@.....~.@
 00002890: cdcc cc3c 7092 0540 0000 0000 8098 0640  ...<p..@.......@
-000028a0: b315 02e4 7d80 0840 f34a f1e5 bf58 0a40  ....}..@.J...X.@
+000028a0: b415 02e4 7d80 0840 f44a f1e5 bf58 0a40  ....}..@.J...X.@
 000028b0: d64f 123e 20c4 0740 0000 0000 8067 0840  .O.> ..@.....g.@
 000028c0: cda0 db52 8fa6 0740 3333 20b3 345f 0840  ...R...@33 .4_.@
 000028d0: cdcc cc7c bd69 0240 0000 0000 805c 0a40  ...|.i.@.....\.@
 000028e0: 0000 0000 8078 0340 0000 0000 0028 0d40  .....x.@.....(.@
-000028f0: 0000 0000 00b6 0440 ffbf 0a07 c10e 0f40  .......@.......@
-00002900: 38b2 0559 5ec8 1640 54da 5c8d 56c4 1240  8..Y^..@T.\.V..@
-00002910: aedc ad27 e179 1140 bf66 911f e7b6 0d40  ...'.y.@.f.....@
+000028f0: 0000 0000 00b6 0440 febf 0a07 c10e 0f40  .......@.......@
+00002900: 38b2 0559 5ec8 1640 55da 5c8d 56c4 1240  8..Y^..@U.\.V..@
+00002910: b0dc ad27 e179 1140 bf66 911f e7b6 0d40  ...'.y.@.f.....@
 00002920: 0000 0000 00bd 0840 0000 0000 00d1 0a40  .......@.......@
 00002930: cdcc 2465 372e 0240 9a99 5dab 8e2a 1040  ..$e7..@..]..*.@
 00002940: 0000 0000 80bc 0640 3333 33c3 5784 0d40  .......@333.W..@
 00002950: 0000 0000 80f7 0340 0000 0000 80c2 0740  .......@.......@
-00002960: 0000 0000 40a8 1240 1c07 dbc2 d91a 1240  ....@..@.......@
-00002970: 898b 2bfe 5133 0d40 3a44 9e74 2f7a 1340  ..+.Q3.@:D.t/z.@
+00002960: 0000 0000 40a8 1240 1e07 dbc2 d91a 1240  ....@..@.......@
+00002970: 8b8b 2bfe 5133 0d40 3a44 9e74 2f7a 1340  ..+.Q3.@:D.t/z.@
 00002980: 9999 99b9 3c13 1340 0000 0000 0053 0840  ....<..@.....S.@
-00002990: 3792 48a4 c8b4 0440 9999 9915 0f41 1040  7.H....@.....A.@
+00002990: 3592 48a4 c8b4 0440 9999 9915 0f41 1040  5.H....@.....A.@
 000029a0: 0000 0000 80d7 0840 33b3 8ee1 ecad 0a40  .......@3......@
 000029b0: 6766 122a ddd3 0740 0000 0000 8058 0240  gf.*...@.....X.@
 000029c0: 0000 0000 803a 0540 6666 6618 6345 0a40  .....:.@fff.cE.@
 000029d0: 0000 0000 800b 0940 cdcc cc84 b2a8 0540  .......@.......@
 000029e0: 0000 0000 803a 0740 329e 438f 3df0 ff3f  .....:.@2.C.=..?
-000029f0: cdcc cccc cc84 0540 7bb3 2f9c 5fca 0340  .......@{./._..@
+000029f0: cdcc cccc cc84 0540 7cb3 2f9c 5fca 0340  .......@|./._..@
 00002a00: 0000 0000 80a0 0740 4d1a 4b3d 14d9 0740  .......@M.K=...@
 00002a10: 0000 0000 80a2 0740 0000 0000 808a 0240  .......@.......@
 00002a20: 0000 0000 808f 0940 0000 0000 80b3 0240  .......@.......@
 00002a30: 0000 0000 00f2 0b40 0000 0000 802a 0540  .......@.....*.@
-00002a40: 0000 3cb3 ccd6 0b40 d90b b54c 1e7f 1140  ..<....@...L...@
-00002a50: f367 0644 e92f 0f40 a6ef 64e7 21ce 0840  .g.D./.@..d.!..@
-00002a60: 62bd 91fe a24e 0840 0000 0000 00d4 0840  b....N.@.......@
+00002a40: 0000 3cb3 ccd6 0b40 db0b b54c 1e7f 1140  ..<....@...L...@
+00002a50: f367 0644 e92f 0f40 a5ef 64e7 21ce 0840  .g.D./.@..d.!..@
+00002a60: 63bd 91fe a24e 0840 0000 0000 00d4 0840  c....N.@.......@
 00002a70: 0000 0000 8075 0a40 0000 0000 0029 0340  .....u.@.....).@
 00002a80: 9a19 73af 2850 1040 0000 0000 807b 0640  ..s.(P.@.....{.@
 00002a90: 3333 330b 84a6 0d40 0000 0000 00ab 0340  333....@.......@
 00002aa0: 0000 0000 00be 0740 9ad3 1b87 f819 1240  .......@.......@
-00002ab0: 61fa 3907 e6d1 0940 e08c 4ca9 a14c 0640  a.9....@..L..L.@
+00002ab0: 5bfa 3907 e6d1 0940 e08c 4ca9 a14c 0640  [.9....@..L..L.@
 00002ac0: e0e6 4cdd 3ee3 1040 9999 999d c0e8 1240  ..L.>..@.......@
 00002ad0: 0000 0000 80e9 0740 6a58 ebd7 b795 0640  .......@jX.....@
 00002ae0: 3333 332b ffe0 0f40 0000 0000 80dd 0840  333+...@.......@
 00002af0: 0000 0000 8036 0940 3633 b34c bdf7 ff3f  .....6.@63.L...?
 00002b00: 0000 0000 80f1 0240 0000 0000 8007 0540  .......@.......@
 00002b10: 0000 00e4 fd53 0a40 0000 0000 00b3 0940  .....S.@.......@
 00002b20: cdcc ccec 5218 0640 0000 0000 00fc 0740  ....R..@.......@
-00002b30: 6ee2 2c6b 195a f93f a2eb 2eb0 0c7b 0140  n.,k.Z.?.....{.@
+00002b30: 72e2 2c6b 195a f93f a0eb 2eb0 0c7b 0140  r.,k.Z.?.....{.@
 00002b40: 59ee 9a3e 982f 0440 cdcc cc54 6e0b 0740  Y..>./.@...Tn..@
 00002b50: 4d31 3e8d fd64 0840 0000 0000 80e9 0640  M1>..d.@.......@
 00002b60: 0000 0000 80d1 0240 0000 0000 00cf 0840  .......@.......@
 00002b70: 0000 0000 0008 0240 0000 0000 80bf 0a40  .......@.......@
 00002b80: 0000 0000 8095 0540 3333 876f 946a 0c40  .......@33.o.j.@
 00002b90: 837f 2e79 6e57 0a40 b156 a7db 3a27 0a40  ...ynW.@.V..:'.@
-00002ba0: a8ea 2501 c577 fe3f f195 0e82 5825 0740  ..%..w.?....X%.@
+00002ba0: a2ea 2501 c577 fe3f f095 0e82 5825 0740  ..%..w.?....X%.@
 00002bb0: 0000 0000 0006 0940 0000 0000 000a 0a40  .......@.......@
 00002bc0: 0000 0000 800c 0440 0000 0000 408b 1040  .......@....@..@
 00002bd0: 0000 0000 8055 0640 0000 0000 0097 0d40  .....U.@.......@
 00002be0: 0000 0000 0067 0340 0000 0000 00bd 0740  .....g.@.......@
 00002bf0: 34f8 6843 5a7a 1140 b48c 8d59 711f 0440  4.hCZz.@...Yq..@
-00002c00: ccef 3b9a c672 0240 2ba6 7eeb 581b 0f40  ..;..r.@+.~.X..@
+00002c00: d0ef 3b9a c672 0240 29a6 7eeb 581b 0f40  ..;..r.@).~.X..@
 00002c10: 0000 0000 00c2 1240 0000 0000 80a1 0740  .......@.......@
 00002c20: 3aad 3140 9e0d 1340 0000 0000 801d 0f40  :.1@...@.......@
 00002c30: 0000 0000 00c1 0840 0000 0000 80e1 0740  .......@.......@
 00002c40: cecc 14ca 0d84 0040 0000 0000 80a4 0340  .......@.......@
 00002c50: 0000 0000 00b0 0440 0000 0000 802f 0a40  .......@...../.@
 00002c60: 0000 0000 8069 0a40 0000 0000 0098 0640  .....i.@.......@
 00002c70: 0000 0000 00d6 0840 1ac7 cf7b 49bd fa3f  .......@...{I..?
-00002c80: c007 7ee6 d269 fa3f e6b8 10d5 aa44 0840  ..~..i.?.....D.@
+00002c80: c007 7ee6 d269 fa3f e4b8 10d5 aa44 0840  ..~..i.?.....D.@
 00002c90: cdcc cc54 01aa 0640 cd1c 6ea4 8148 0940  ...T...@..n..H.@
 00002ca0: 0000 0000 0021 0640 0000 0000 803e 0340  .....!.@.....>.@
 00002cb0: 0000 0000 802c 0840 0000 0000 0075 0140  .....,.@.....u.@
 00002cc0: 0000 0000 80a1 0940 0000 0000 00f0 0540  .......@.......@
-00002cd0: 0000 0000 0067 0c40 69f5 aa07 1b03 0a40  .....g.@i......@
-00002ce0: 515e 41f3 5b5e 0940 508c c897 37ad f73f  Q^A.[^.@P...7..?
-00002cf0: 0e6d 4690 3bbb 0940 0000 0000 0052 0940  .mF.;..@.....R.@
+00002cd0: 0000 0000 0067 0c40 67f5 aa07 1b03 0a40  .....g.@g......@
+00002ce0: 515e 41f3 5b5e 0940 548c c897 37ad f73f  Q^A.[^.@T...7..?
+00002cf0: 106d 4690 3bbb 0940 0000 0000 0052 0940  .mF.;..@.....R.@
 00002d00: 0000 0000 8096 0940 0000 0000 80fa 0440  .......@.......@
 00002d10: 0000 0000 c0d9 1040 0000 0000 0052 0640  .......@.....R.@
 00002d20: 0000 0000 805e 0d40 0000 0000 0025 0340  .....^.@.....%.@
 00002d30: 0000 0000 80b9 0740 9a4a 3c4a 860f 1140  .......@.J<J...@
-00002d40: ec1e 66df db3e 0240 f439 28b2 aab4 0940  ..f..>.@.9(....@
-00002d50: 8434 b036 471c 1140 0000 0000 409a 1240  .4.6G..@....@..@
+00002d40: e81e 66df db3e 0240 ec39 28b2 aab4 0940  ..f..>.@.9(....@
+00002d50: 8634 b036 471c 1140 0000 0000 409a 1240  .4.6G..@....@..@
 00002d60: 0000 0000 007b 0740 f227 c090 9d53 1340  .....{.@.'...S.@
 00002d70: 0000 0000 0061 0e40 0000 0000 008a 0840  .....a.@.......@
 00002d80: 0000 0000 0082 0640 9a19 3778 1e13 0840  .......@..7x...@
 00002d90: 0000 0000 8067 0440 0000 0000 0038 0440  .....g.@.....8.@
 00002da0: 0000 0000 00e5 0940 0000 0000 8027 0b40  .......@.....'.@
 00002db0: 0000 0000 8038 0740 0000 0000 80be 0940  .....8.@.......@
 00002dc0: 4330 094b c7cf 0240 0000 0000 0000 0000  C0.K...@........
-00002dd0: 1a4e 0b12 9cd0 1240 0000 0000 008b 0640  .N.....@.......@
+00002dd0: 1b4e 0b12 9cd0 1240 0000 0000 008b 0640  .N.....@.......@
 00002de0: cd93 6e88 b487 0a40 0000 0000 804d 0540  ..n....@.....M.@
 00002df0: 0000 0000 00c6 0340 0000 0000 80b3 0740  .......@.......@
 00002e00: 0000 0000 00fd 0040 0000 0000 009f 0840  .......@.......@
 00002e10: 0000 0000 003c 0640 0000 0000 00c4 0c40  .....<.@.......@
-00002e20: 5498 2bb8 423c 1240 20da 3468 1994 1040  T.+.B<.@ .4h...@
-00002e30: 9da4 aec9 3bab 0540 6971 90c1 c7ff 1240  ....;..@iq.....@
+00002e20: 5298 2bb8 423c 1240 20da 3468 1994 1040  R.+.B<.@ .4h...@
+00002e30: 9ba4 aec9 3bab 0540 6771 90c1 c7ff 1240  ....;..@gq.....@
 00002e40: 0000 0000 80b7 0940 0000 0000 801f 0940  .......@.......@
 00002e50: 0000 0000 00dd 0540 0000 0000 4036 1140  .......@....@6.@
 00002e60: 0000 0000 0079 0640 0000 0000 8004 0d40  .....y.@.......@
 00002e70: 0000 0000 00df 0240 0000 0000 00ac 0740  .......@.......@
-00002e80: f471 0882 7ed6 1040 18d2 9bf1 a2d8 fe3f  .q..~..@.......?
-00002e90: 022b 65dd 4d98 1640 5896 eca1 f1e2 1540  .+e.M..@X......@
+00002e80: f471 0882 7ed6 1040 20d2 9bf1 a2d8 fe3f  .q..~..@ ......?
+00002e90: 022b 65dd 4d98 1640 5696 eca1 f1e2 1540  .+e.M..@V......@
 00002ea0: 0000 0000 8075 1240 0000 0000 8072 0740  .....u.@.....r.@
 00002eb0: 5a67 7d55 8535 1440 0000 0000 8095 0d40  Zg}U.5.@.......@
 00002ec0: 0000 0000 0045 0840 0000 0000 0028 0540  .....E.@.....(.@
 00002ed0: 6766 c9c7 a7dc 0840 0000 0000 0027 0540  gf.....@.....'.@
 00002ee0: 0000 0000 80ac 0340 0000 0000 8073 0940  .......@.....s.@
 00002ef0: 0000 0000 80e2 0b40 0000 0000 00e7 0740  .......@.......@
-00002f00: 0000 0000 80a6 0a40 025b c514 186d 0c40  .......@.[...m.@
-00002f10: 60cf 5ab1 e65b 1740 0000 0000 c08d 1440  `.Z..[.@.......@
+00002f00: 0000 0000 80a6 0a40 035b c514 186d 0c40  .......@.[...m.@
+00002f10: 62cf 5ab1 e65b 1740 0000 0000 c08d 1440  b.Z..[.@.......@
 00002f20: 0000 0000 008f 0640 0000 0000 80be 0b40  .......@.......@
 00002f30: 0000 0000 007e 0440 0000 0000 0050 0440  .....~.@.....P.@
 00002f40: 0000 0000 805e 0740 0000 0000 00a4 0040  .....^.@.......@
 00002f50: cdcc ccec f596 0740 0000 0000 0078 0640  .......@.....x.@
-00002f60: 0080 0275 8219 0d40 d341 0207 c899 1b40  ...u...@.A.....@
+00002f60: 0080 0275 8219 0d40 d141 0207 c899 1b40  ...u...@.A.....@
 00002f70: 4739 ed74 c141 1c40 4448 cbed ac6e 1240  G9.t.A.@DH...n.@
 00002f80: 0000 0000 4054 1440 0000 0000 002f 0a40  ....@T.@...../.@
 00002f90: 0000 0000 80ac 0840 0000 0000 80a4 0640  .......@.......@
 00002fa0: 0000 0000 4094 1140 0000 0000 00c6 0640  ....@..@.......@
 00002fb0: 0000 0000 0098 0c40 0000 0000 8098 0240  .......@.......@
 00002fc0: 0000 0000 0093 0740 6795 967c 88c6 1040  .......@g..|...@
-00002fd0: 4e63 9fc5 aa1e 1340 48bc 3dd2 628e 2440  Nc.....@H.=.b.$@
+00002fd0: 4a63 9fc5 aa1e 1340 49bc 3dd2 628e 2440  Jc.....@I.=.b.$@
 00002fe0: 247a 303a f725 2140 0000 0000 4058 1240  $z0:.%!@....@X.@
 00002ff0: 0000 0000 8081 0740 4e40 ad21 1726 1540  .......@N@.!.&.@
 00003000: 0000 0000 00d3 0c40 0000 0000 0000 0840  .......@.......@
 00003010: 0080 1d01 4e82 0340 0000 0000 80d3 0940  ....N..@.......@
 00003020: 0000 0000 80d5 0540 0000 0000 801b 0340  .......@.......@
 00003030: 0000 0000 80f5 0840 0000 0000 0090 0c40  .......@.......@
 00003040: 0000 0000 008e 0840 3333 332b 0d83 0b40  .......@333+...@
 00003050: 0000 0000 006d 0d40 778e c7a5 2e97 1340  .....m.@w......@
-00003060: 8d04 aaf3 f567 1640 0000 0000 00b1 0640  .....g.@.......@
+00003060: 8c04 aaf3 f567 1640 0000 0000 00b1 0640  .....g.@.......@
 00003070: cd64 8924 f38a 0c40 0000 0000 00c1 0340  .d.$...@.......@
 00003080: 0000 0000 80cf 0440 0000 0000 002c 0740  .......@.....,.@
 00003090: 0000 0000 8065 0040 cdcc ccb4 34ba 0640  .....e.@....4..@
 000030a0: 0000 0000 80a1 0640 0000 0000 804f 0d40  .......@.....O.@
-000030b0: 3996 7322 ec03 1c40 7fdc 5364 bd58 1d40  9.s"...@..Sd.X.@
-000030c0: 0edd c76b b396 1a40 4764 beac 7d16 1640  ...k...@Gd..}..@
+000030b0: 3b96 7322 ec03 1c40 80dc 5364 bd58 1d40  ;.s"...@..Sd.X.@
+000030c0: 0fdd c76b b396 1a40 4764 beac 7d16 1640  ...k...@Gd..}..@
 000030d0: 0000 0000 00a7 0a40 0000 0000 0043 0840  .......@.....C.@
 000030e0: 0000 0cc3 9353 0740 0000 0000 c0ec 1140  .....S.@.......@
 000030f0: 0000 0000 8024 0740 0000 0000 802b 0c40  .....$.@.....+.@
 00003100: 0000 0000 8055 0240 0000 0000 807b 0740  .....U.@.....{.@
-00003110: 1a9c e07d 3dd3 1040 6e8c f650 8560 2340  ...}=..@n..P.`#@
-00003120: 7418 1178 6780 2640 4fd8 bca5 7409 2340  t..xg.&@O...t.#@
+00003110: 1a9c e07d 3dd3 1040 6c8c f650 8560 2340  ...}=..@l..P.`#@
+00003120: 7218 1178 6780 2640 4fd8 bca5 7409 2340  r..xg.&@O...t.#@
 00003130: 0000 0000 c040 1240 0000 0000 809d 0740  .....@.@.......@
-00003140: 2e17 05e7 ad3f 1640 0000 0000 002f 0c40  .....?.@...../.@
+00003140: 2d17 05e7 ad3f 1640 0000 0000 002f 0c40  -....?.@...../.@
 00003150: 0000 0000 00c1 0740 cdcc a0c7 d9da 0140  .......@.......@
 00003160: 33b3 8ce7 329b 0a40 3333 3383 3d72 0640  3...2..@333.=r.@
 00003170: 0000 0000 8099 0240 0000 0000 8083 0840  .......@.......@
 00003180: 3333 338b f137 0d40 0000 0000 8021 0940  333..7.@.....!.@
-00003190: 3333 333b 8678 0c40 0c4a 52e4 e48e 0f40  333;.x.@.JR....@
-000031a0: 3268 7dd9 c3e9 1540 8124 93f0 5e69 1840  2h}....@.$..^i.@
+00003190: 3333 333b 8678 0c40 0d4a 52e4 e48e 0f40  333;.x.@.JR....@
+000031a0: 2e68 7dd9 c3e9 1540 7f24 93f0 5e69 1840  .h}....@.$..^i.@
 000031b0: 0000 0000 00e2 0640 0043 d94c 742e 0e40  .......@.C.Lt..@
 000031c0: cdcc cc34 3003 0340 0000 0000 0041 0540  ...40..@.....A.@
 000031d0: 0000 0000 0014 0740 0000 0000 8039 0040  .......@.....9.@
 000031e0: cdcc cc8c 7913 0640 0000 0000 80bc 0640  ....y..@.......@
 000031f0: 0000 0000 007b 0d40 c610 d145 87fe 1d40  .....{.@...E...@
-00003200: bb12 97b6 41b7 1e40 ff12 7a8e f415 2140  ....A..@..z...!@
-00003210: e9b0 be4e 33d9 1740 0000 0000 8012 0b40  ...N3..@.......@
+00003200: bb12 97b6 41b7 1e40 0113 7a8e f415 2140  ....A..@..z...!@
+00003210: e7b0 be4e 33d9 1740 0000 0000 8012 0b40  ...N3..@.......@
 00003220: 0000 0000 80f2 0740 33b3 cbc6 9902 0840  .......@3......@
 00003230: 0000 0000 4038 1240 0000 0000 8080 0740  ....@8.@.......@
 00003240: 0000 0000 80c4 0b40 0000 0000 001f 0240  .......@.......@
 00003250: 0000 0000 0068 0740 0000 0000 40df 1040  .....h.@....@..@
 00003260: 335a 1643 ddcc 2a40 b9d9 9c15 7fbf 2d40  3Z.C..*@......-@
 00003270: 53c8 c939 6c6f 2640 0000 0000 802e 1240  S..9lo&@.......@
 00003280: 0000 0000 00bb 0740 f8bf 8d93 b418 1740  .......@.......@
 00003290: cdcc cc94 8f90 0b40 0000 0000 008f 0740  .......@.......@
-000032a0: 3433 521a b79c 0040 65e6 bcc1 c4f2 0a40  43R....@e......@
+000032a0: 3433 521a b79c 0040 66e6 bcc1 c4f2 0a40  43R....@f......@
 000032b0: 3333 3353 5608 0740 0000 0000 0039 0240  333SV..@.....9.@
 000032c0: 0000 0000 002f 0840 3333 335b 17c6 0d40  ...../.@333[...@
 000032d0: 3333 331b e89b 0940 3333 337b df29 0d40  333....@333{.).@
-000032e0: f8c6 7819 7e3c 1540 b80e ac01 e037 1f40  ..x.~<.@.....7.@
+000032e0: f6c6 7819 7e3c 1540 b80e ac01 e037 1f40  ..x.~<.@.....7.@
 000032f0: eebf a520 898c 1f40 0000 0000 8011 0740  ... ...@.......@
 00003300: 330d c3bf 67e3 0d40 cdcc ccc4 2c74 0240  3...g..@....,t.@
 00003310: 0000 0000 0099 0540 0000 0000 800d 0740  .......@.......@
 00003320: 0000 0000 801a 0040 cdcc cc94 88a1 0540  .......@.......@
 00003330: 0000 0000 80cb 0640 0000 0000 0096 0d40  .......@.......@
-00003340: 409c 2420 1872 2340 246e 20b2 4da6 2640  @.$ .r#@$n .M.&@
-00003350: 749f e12b ead6 2540 ca3e f6ee 93a4 1d40  t..+..%@.>.....@
+00003340: 409c 2420 1872 2340 216e 20b2 4da6 2640  @.$ .r#@!n .M.&@
+00003350: 759f e12b ead6 2540 ca3e f6ee 93a4 1d40  u..+..%@.>.....@
 00003360: 0000 0000 8061 0b40 0000 0000 00bd 0740  .....a.@.......@
 00003370: 0080 4b01 8d7d 0840 9999 9941 b282 1240  ..K..}.@...A...@
 00003380: 0000 0000 80c1 0740 0000 0000 8071 0b40  .......@.....q.@
 00003390: 0000 0000 00f8 0140 0000 0000 8060 0740  .......@.....`.@
-000033a0: 0000 0000 40eb 1040 688a 16fc 8c37 3140  ....@..@h....71@
-000033b0: cb13 e62e ac20 3340 e53a 07bb 4928 2c40  ..... 3@.:..I(,@
+000033a0: 0000 0000 40eb 1040 668a 16fc 8c37 3140  ....@..@f....71@
+000033b0: cd13 e62e ac20 3340 e53a 07bb 4928 2c40  ..... 3@.:..I(,@
 000033c0: 0000 0000 0022 1240 0000 0000 00cd 0740  .....".@.......@
-000033d0: aa4c 046a b591 1740 cdcc ccb4 5736 0b40  .L.j...@....W6.@
+000033d0: a94c 046a b591 1740 cdcc ccb4 5736 0b40  .L.j...@....W6.@
 000033e0: 0000 0000 0075 0740 3633 032d bf8b f53f  .....u.@63.-...?
 000033f0: cccc 0cee cf35 1240 3333 339b 5555 0740  .....5.@333.UU.@
 00003400: 0000 0000 0005 0240 0000 0000 8003 0840  .......@.......@
 00003410: 3333 3353 8f11 0e40 3333 33bb eef6 0940  333S...@333....@
-00003420: 3333 33b3 7185 0d40 e2c7 f8ea 095b 1840  333.q..@.....[.@
-00003430: cae0 a293 9c1f 2340 5e29 9b78 3b4b 2240  ......#@^).x;K"@
+00003420: 3333 33b3 7185 0d40 e4c7 f8ea 095b 1840  333.q..@.....[.@
+00003430: cbe0 a293 9c1f 2340 5e29 9b78 3b4b 2240  ......#@^).x;K"@
 00003440: 0000 0000 002c 0740 cce8 658e 56d0 1640  .....,.@..e.V..@
 00003450: cdcc cc4c f42d 0240 0000 0000 80c7 0540  ...L.-.@.......@
 00003460: 0000 0000 000a 0740 0000 0000 000a 0040  .......@.......@
 00003470: cdcc ccac be68 0540 0000 0000 00cf 0640  .....h.@.......@
-00003480: 0000 0000 00a3 0d40 b3bc 0abe e08b 2540  .......@......%@
-00003490: e556 07f7 b62c 2b40 e90d f608 6a87 2a40  .V...,+@....j.*@
+00003480: 0000 0000 00a3 0d40 b5bc 0abe e08b 2540  .......@......%@
+00003490: e656 07f7 b62c 2b40 e80d f608 6a87 2a40  .V...,+@....j.*@
 000034a0: 0205 eff7 6247 2040 0000 0000 808b 0b40  ....bG @.......@
 000034b0: 0000 0000 80a2 0740 6666 8bda f9bc 0840  .......@ff.....@
 000034c0: 9999 99d9 18ad 1240 0000 0000 00e1 0740  .......@.......@
 000034d0: 0000 0000 8042 0b40 0000 0000 00e6 0140  .....B.@.......@
 000034e0: 0000 0000 0060 0740 0000 0000 40f3 1040  .....`.@....@..@
-000034f0: bfa5 57aa 5237 3240 55ec fd1a 8a70 3540  ..W.R72@U....p5@
+000034f0: c0a5 57aa 5237 3240 54ec fd1a 8a70 3540  ..W.R72@T....p5@
 00003500: ac56 acdc b1cf 3040                      .V....0@
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/1d_no_background.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/1d_no_background.npz`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 13712 bytes, number of entries: 1
-?rw-------  2.0 unx    13576 b- stor 80-Jan-01 00:00 arr_0.npy
+?rw-------  4.5 unx    13576 b- stor 80-Jan-01 00:00 arr_0.npy
 1 file, 13576 bytes uncompressed, 13576 bytes compressed:  0.0%
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v4.5 to extract, compression method=store
```

#### arr_0.npy

```diff
@@ -16,15 +16,15 @@
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000120: 9c99 9999 af1c ba3f 0000 0000 0000 0000  .......?........
 00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 8033 332d 1424 633f 9289 7184 adea ff3f  .33-.$c?..q....?
+00000160: 8033 332d 1424 633f 9689 7184 adea ff3f  .33-.$c?..q....?
 00000170: 0000 0000 0000 0000 b8cc cccc 9ce1 a23f  ...............?
 00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 9ef4 41f7 ad5c f63f 1e13 9b56 7f25 fe3f  ..A..\.?...V.%.?
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 b8cc cccc 5abc ad3f  ............Z..?
@@ -37,15 +37,15 @@
 00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000260: 0000 0000 0000 0000 5c66 66a6 e5ff b63f  ........\ff....?
 00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002b0: 6646 fee0 1fa1 f23f 0000 0000 0000 0000  fF.....?........
+000002b0: 6246 fee0 1fa1 f23f 0000 0000 0000 0000  bF.....?........
 000002c0: 7099 9999 a53c 973f 0000 0000 0000 0000  p....<.?........
 000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000002f0: 0000 0000 0000 0000 973b 9e20 7399 d13f  .........;. s..?
 00000300: d26e 21a5 2c18 f43f 0000 0000 0000 0000  .n!.,..?........
 00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000320: 38d3 9bd4 ca41 a73f 0000 0000 0000 0000  8....A.?........
@@ -57,20 +57,20 @@
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: dcff ff3f 8b20 b13f 0000 0000 0000 0000  ...?. .?........
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003f0: 0000 0000 0000 0000 000d 979f a7bd b53f  ...............?
+000003f0: 0000 0000 0000 0000 e00c 979f a7bd b53f  ...............?
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000440: fe40 5f97 0cfe c73f 6066 efef 84e9 c53f  .@_....?`f.....?
+00000440: fe40 5f97 0cfe c73f 2066 efef 84e9 c53f  .@_....? f.....?
 00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000460: 0000 0000 0000 0000 f0f2 68dd b2bd 9b3f  ..........h....?
 00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000490: f8ff 4fe6 5af1 e03f 0000 0000 0000 0000  ..O.Z..?........
 000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004b0: 5c66 6625 4bf6 b73f 0000 0000 0000 0000  \ff%K..?........
@@ -108,15 +108,15 @@
 000006b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000720: 3033 738e 11ba e03f 0000 0000 0000 0000  03s....?........
+00000720: 2c33 738e 11ba e03f 0000 0000 0000 0000  ,3s....?........
 00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000790: 70cc 4c03 9409 913f 0000 0000 0000 0000  p.L....?........
@@ -166,15 +166,15 @@
 00000a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ac0: 0000 0000 0000 0000 ff3f 665f 9970 0040  .........?f_.p.@
+00000ac0: 0000 0000 0000 0000 fd3f 665f 9970 0040  .........?f_.p.@
 00000ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -200,15 +200,15 @@
 00000c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c90: 0000 0000 0000 0000 7099 5908 3450 973f  ........p.Y.4P.?
 00000ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000cb0: 5c66 e690 4772 b73f 0000 0000 0000 0000  \f..Gr.?........
 00000cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ce0: 0000 0000 0000 0000 20cf 4c43 0d73 8d3f  ........ .LC.s.?
+00000ce0: 0000 0000 0000 0000 20ce 4c43 0d73 8d3f  ........ .LC.s.?
 00000cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -220,15 +220,15 @@
 00000db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000de0: 80cb ccea 0725 643f 0000 0000 0000 0000  .....%d?........
 00000df0: 0000 0000 0000 0000 3866 2659 1cc7 af3f  ........8f&Y...?
 00000e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000e20: 0000 0000 0000 0000 384b 00a6 954f a73f  ........8K...O.?
+00000e20: 0000 0000 0000 0000 784b 00a6 954f a73f  ........xK...O.?
 00000e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -268,29 +268,29 @@
 000010b0: b875 38c0 3b3e a13f 3875 6021 d657 a63f  .u8.;>.?8u`!.W.?
 000010c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001120: eccc df80 8d9b e43f 0000 0000 0000 0000  .......?........
+00001120: f4cc df80 8d9b e43f 0000 0000 0000 0000  .......?........
 00001130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001190: 0000 0000 0000 0000 705f 5bf5 7b9d 903f  ........p_[.{..?
 000011a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011b0: b8cc cccc 94fe a03f 0000 0000 0000 0000  .......?........
 000011c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011f0: 0000 0000 0000 0000 38bf af5a 8a82 a63f  ........8..Z...?
-00001200: a204 7d54 4cb1 fc3f 3233 2305 87a1 fb3f  ..}TL..?23#....?
+00001200: 9e04 7d54 4cb1 fc3f 3233 2305 87a1 fb3f  ..}TL..?23#....?
 00001210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001250: 0000 0000 0000 0000 2e4c c625 350d 1a40  .........L.%5..@
 00001260: f423 951a e370 2640 493a 5d12 a9fa 2040  .#...p&@I:]... @
 00001270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -308,16 +308,16 @@
 00001330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001340: 3854 3dbb 3c99 a33f babc 3d25 738c f93f  8T=.<..?..=%s..?
 00001350: cacc ccfd ba39 fb3f 0000 0000 0000 0000  .....9.?........
 00001360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000013a0: c638 0fd8 1004 1b40 0323 ffa5 34f9 0140  .8.....@.#..4..@
-000013b0: f425 95a2 2b7e e83f 0000 0000 0000 0000  .%..+~.?........
+000013a0: c438 0fd8 1004 1b40 0723 ffa5 34f9 0140  .8.....@.#..4..@
+000013b0: fc25 95a2 2b7e e83f 0000 0000 0000 0000  .%..+~.?........
 000013c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001420: 0000 0000 0000 0000 705b fb06 afd1 9b3f  ........p[.....?
@@ -329,15 +329,15 @@
 00001480: 0000 0000 0000 0000 8023 b92e 3ef0 633f  .........#..>.c?
 00001490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000014a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000014b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000014c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000014d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000014e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000014f0: 86ad 14c7 216a f43f 0000 0000 0000 0000  ....!j.?........
+000014f0: 7ead 14c7 216a f43f 0000 0000 0000 0000  ~...!j.?........
 00001500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -363,15 +363,15 @@
 000016a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000016b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000016c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000016d0: 5c66 6666 73da b33f 0000 0000 0000 0000  \fffs..?........
 000016e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000016f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001710: 0000 0000 0000 0000 0068 7604 a293 903f  .........hv....?
+00001710: 0000 0000 0000 0000 0069 7604 a293 903f  .........iv....?
 00001720: 0000 0000 0000 0000 00bc fc07 0e14 843f  ...............?
 00001730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001740: 5c66 a6ef fbba b03f 0000 0000 0000 0000  \f.....?........
 00001750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -448,15 +448,15 @@
 00001bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c10: 0000 0000 0000 0000 b8cc cccc 302e a33f  ............0..?
 00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c60: b8cc ccc7 5b20 a33f 3c33 b33e fb67 b13f  ....[ .?<3.>.g.?
+00001c60: b8cc ccc7 5b20 a33f fc32 b33e fb67 b13f  ....[ .?.2.>.g.?
 00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -466,15 +466,15 @@
 00001d10: 0000 0000 0000 0000 70be 4540 b786 923f  ........p.E@...?
 00001d20: 20a4 860c f915 b43f 0000 0000 0000 0000   ......?........
 00001d30: 7099 9999 a500 973f 0000 0000 0000 0000  p......?........
 00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d60: 5c66 6666 8707 b03f 0000 0000 0000 0000  \fff...?........
 00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d80: 0000 0000 0000 0000 0048 2dfb 94d2 a93f  .........H-....?
+00001d80: 0000 0000 0000 0000 8049 2dfb 94d2 a93f  .........I-....?
 00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001db0: 3800 0086 c8ee a13f 0000 0000 0000 0000  8......?........
 00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -487,15 +487,15 @@
 00001e60: 38db fe13 cf8a a93f 0000 0000 0000 0000  8......?........
 00001e70: 0017 3b73 cb7d 5c3f b8cc cccc 1a85 a93f  ..;s.}\?.......?
 00001e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ea0: 0000 0000 0000 0000 5c66 6666 cee1 b43f  ........\fff...?
 00001eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ed0: 387d 05e2 57c5 a03f 0000 0000 0000 0000  8}..W..?........
+00001ed0: 387e 05e2 57c5 a03f 0000 0000 0000 0000  8~..W..?........
 00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ef0: 0000 0000 0000 0000 9699 99b4 27f5 fa3f  ............'..?
 00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f30: 0000 0000 0000 0000 009b 6ff4 86dc ae3f  ..........o....?
 00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -507,22 +507,22 @@
 00001fa0: 0000 0000 0000 0000 bcf9 4333 7e1c b33f  ..........C3~..?
 00001fb0: f0c2 8ee9 3474 903f b818 e5cd 508d ad3f  ....4t.?....P..?
 00001fc0: 5c66 6666 1449 b03f 0000 0000 0000 0000  \fff.I.?........
 00001fd0: c099 9911 102e 743f 0000 0000 0000 0000  ......t?........
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 5c66 6666 84bc b73f 0000 0000 0000 0000  \fff...?........
 00002000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002010: 0000 0000 0000 0000 d10e e955 cd3e d03f  ...........U.>.?
+00002010: 0000 0000 0000 0000 c10e e955 cd3e d03f  ...........U.>.?
 00002020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002040: 70cc 4ca2 79b9 9b3f 0000 0000 0000 0000  p.L.y..?........
 00002050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002060: 0000 0000 0000 0000 8066 135f ebf8 bd3f  .........f._...?
 00002070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002080: 700a 91a2 86fa 913f 0000 0000 0000 0000  p......?........
+00002080: 700b 91a2 86fa 913f 0000 0000 0000 0000  p......?........
 00002090: 0000 0000 0000 0000 98f8 b5d9 4d97 f13f  ............M..?
 000020a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020b0: 70ff 7fd8 c497 9a3f 9c99 19a6 e912 b43f  p......?.......?
 000020c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020d0: c0ff ffff c3fe a23f 0000 0000 0000 0000  .......?........
 000020e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020f0: 3c66 a119 0fd4 b63f 0000 0000 0000 0000  <f.....?........
@@ -533,85 +533,85 @@
 00002140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002150: 40ef 4b33 38dc bb3f 0000 0000 0000 0000  @.K38..?........
 00002160: 04a1 e152 e426 fa3f 0000 0000 0000 0000  ...R.&.?........
 00002170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002180: 0000 0000 0000 0000 1c00 0005 b26a b03f  .............j.?
 00002190: c065 6666 c6ea 7a3f 0000 0000 0000 0000  .eff..z?........
 000021a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021b0: b899 b48f 13f2 a13f 9e53 dbdb 977c f83f  .......?.S...|.?
+000021b0: b899 b48f 13f2 a13f a653 dbdb 977c f83f  .......?.S...|.?
 000021c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021e0: 972f 88d2 cdad 0040 0000 0000 0000 0000  ./.....@........
 000021f0: 0000 0000 0000 0000 b8cc 0c39 dde8 aa3f  ...........9...?
 00002200: b8cc ac19 27bd a93f 0000 0000 0000 0000  ....'..?........
 00002210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002230: 0000 0000 0000 0000 3c3e 9924 eb7b b63f  ........<>.$.{.?
-00002240: bebb c0c9 8eec f53f cefc 7a61 91db f83f  .......?..za...?
+00002240: c4bb c0c9 8eec f53f cefc 7a61 91db f83f  .......?..za...?
 00002250: b8cc cccc 44bf a63f 0000 0000 0000 0000  ....D..?........
 00002260: b8cc 6c1e 4ad6 aa3f 0000 0000 0000 0000  ..l.J..?........
 00002270: b8cc cccc 4810 a23f 0000 0000 0000 0000  ....H..?........
 00002280: 5c66 6666 1a84 b63f 0000 0000 0000 0000  \fff...?........
 00002290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000022a0: cbee e44b bfa2 2040 ed9c f3d0 80a6 0640  ...K.. @.......@
 000022b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000022c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000022d0: 0000 0000 0000 0000 c065 6666 7656 7c3f  .........effvV|?
 000022e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000022f0: 0000 0000 0000 0000 fe3f 08b4 d249 fa3f  .........?...I.?
-00002300: 9b4b 48ed 5098 0c40 c22f df56 46ad 2d40  .KH.P..@./.VF.-@
+00002300: 9f4b 48ed 5098 0c40 c22f df56 46ad 2d40  .KH.P..@./.VF.-@
 00002310: 8f63 5090 092e 0340 e032 3333 2392 823f  .cP....@.233#..?
 00002320: 0000 0000 0000 0000 6361 62e7 fd8d 0040  ........cab....@
 00002330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002340: 5c66 6621 779d b23f e032 333d ce80 813f  \ff!w..?.23=...?
 00002350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002380: 38ed 3c02 d98b af3f a892 7557 7763 f33f  8.<....?..uWwc.?
 00002390: 0000 0000 0000 0000 e032 3333 f3cb 8b3f  .........233...?
 000023a0: 0000 0000 0000 0000 b8cc ccda 88a5 af3f  ...............?
 000023b0: 0000 0000 0000 0000 b8cc cccc cef5 a43f  ...............?
 000023c0: 0000 0000 0000 0000 5c66 6666 2268 b23f  ........\fff"h.?
 000023d0: 0000 0000 0000 0000 b8cc cc81 f444 a53f  .............D.?
-000023e0: b1ed 05aa 5a43 0140 3b97 e30d fb82 2140  ....ZC.@;.....!@
-000023f0: 5b55 babc f57f 0940 0000 0000 0000 0000  [U.....@........
+000023e0: b3ed 05aa 5a43 0140 3b97 e30d fb82 2140  ....ZC.@;.....!@
+000023f0: 5755 babc f57f 0940 0000 0000 0000 0000  WU.....@........
 00002400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002440: 2ea3 ecac d117 fe3f 5a0d 8228 826e 2a40  .......?Z..(.n*@
-00002450: 566b 4ea9 d7d1 1640 8923 f481 5b0c 0440  VkN....@.#..[..@
+00002450: 566b 4ea9 d7d1 1640 8b23 f481 5b0c 0440  VkN....@.#..[..@
 00002460: b8cc cccc ba84 a33f 0000 0000 0000 0000  .......?........
 00002470: 9cca c3ea b891 f13f 7099 9999 e5c6 913f  .......?p......?
 00002480: 0000 0000 0000 0000 5c66 7637 739b b53f  ........\fv7s..?
 00002490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024f0: 3866 26fa e5a0 af3f 0000 0000 0000 0000  8f&....?........
 00002500: b8cc cccc fe3b a03f 0000 0000 0000 0000  .....;.?........
 00002510: b8cc cccc 1674 a83f 0000 0000 0000 0000  .....t.?........
-00002520: 80ff 5fc7 07f5 953f a31b 81f0 0065 0240  .._....?.....e.@
-00002530: 209f f765 1cc4 b43f ef3d 05e8 bf07 0240   ..e...?.=.....@
+00002520: 80ff 5fc7 07f5 953f a11b 81f0 0065 0240  .._....?.....e.@
+00002530: 209f f765 1cc4 b43f f13d 05e8 bf07 0240   ..e...?.=.....@
 00002540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002550: 0070 9999 99fd 143f 0000 0000 0000 0000  .p.....?........
 00002560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002590: aa84 a048 c09d f23f 0000 0000 0000 0000  ...H...?........
 000025a0: 0000 0000 0000 0000 b8cc cccc 1256 ac3f  .............V.?
 000025b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000025c0: b8cc cccc 44f0 a63f 0000 0000 0000 0000  ....D..?........
 000025d0: 1c00 307f 0509 b63f 0000 0000 0000 0000  ..0....?........
 000025e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000025f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002610: 70a7 db45 1137 933f 0000 0000 0000 0000  p..E.7.?........
+00002610: f0a7 db45 1137 933f 0000 0000 0000 0000  ...E.7.?........
 00002620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002630: 0000 0000 0000 0000 3833 1399 1cf9 aa3f  ........83.....?
 00002640: 0000 0000 0000 0000 e032 3333 532f 833f  .........233S/.?
 00002650: 0000 0000 0000 0000 7099 9999 2160 913f  ........p...!`.?
 00002660: 0000 0000 0000 0000 f1ff 95af bbe8 dd3f  ...............?
 00002670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -649,15 +649,15 @@
 00002880: c065 6666 5edb 793f 0000 0000 0000 0000  .eff^.y?........
 00002890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000028a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000028b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000028c0: 0000 0000 0000 0000 e032 3320 b334 873f  .........23 .4.?
 000028d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000028e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028f0: 0000 0000 0000 0000 f9ff 5538 0826 df3f  ..........U8.&.?
+000028f0: 0000 0000 0000 0000 f1ff 5538 0826 df3f  ..........U8.&.?
 00002900: 0070 640b b2bc 893f 0000 0000 0000 0000  .pd....?........
 00002910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002940: 0000 0000 0000 0000 c065 6666 86af 733f  .........eff..s?
 00002950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -746,104 +746,104 @@
 00002e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002eb0: 705a 677d 5585 9a3f 0000 0000 0000 0000  pZg}U..?........
 00002ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f00: 0000 0000 0000 0000 80c0 5631 05a6 a33f  ..........V1...?
-00002f10: 823d 6bc5 9a9e f33f 0000 0000 0000 0000  .=k....?........
+00002f00: 0000 0000 0000 0000 c0c0 5631 05a6 a33f  ..........V1...?
+00002f10: 8a3d 6bc5 9a9e f33f 0000 0000 0000 0000  .=k....?........
 00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f60: 80ff ff09 d409 6e3f 301d 2470 80d0 d03f  ......n?0.$p...?
+00002f60: 80ff ff09 d409 6e3f 101d 2470 80d0 d03f  ......n?..$p...?
 00002f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002fd0: 0000 0000 0000 0000 2424 de1e 69e1 b93f  ........$$..i..?
+00002fd0: 0000 0000 0000 0000 a424 de1e 69e1 b93f  .........$..i..?
 00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ff0: 0000 0000 0000 0000 9c13 506b c8b5 b33f  ..........Pk...?
 00003000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003040: 0000 0000 0000 0000 80cb cccc ac34 603f  .............4`?
 00003050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003060: 9291 4075 beb6 c53f 0000 0000 0000 0000  ..@u...?........
+00003060: 7291 4075 beb6 c53f 0000 0000 0000 0000  r.@u...?........
 00003070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000030a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000030b0: 408e e59c 086b b83f 0000 0000 0000 0000  @....k.?........
+000030b0: c08e e59c 086b b83f 0000 0000 0000 0000  .....k.?........
 000030c0: 0000 0000 0000 0000 e088 cc97 b587 c53f  ...............?
 000030d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000030e0: 80ff ff2f 0c4f 6c3f 0000 0000 0000 0000  .../.Ol?........
 000030f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003110: 0000 0000 0000 0000 6e1b a33d 5461 cc3f  ........n..=Ta.?
-00003120: 001d 4604 de99 cf3f ea09 9bb7 944e d63f  ..F....?.....N.?
+00003110: 0000 0000 0000 0000 ee1a a33d 5461 cc3f  ...........=Ta.?
+00003120: 801c 4604 de99 cf3f ea09 9bb7 944e d63f  ..F....?.....N.?
 00003130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003140: cee5 a2e0 bc55 c83f 0000 0000 0000 0000  .....U.?........
+00003140: aee5 a2e0 bc55 c83f 0000 0000 0000 0000  .....U.?........
 00003150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003160: 7099 59c6 7359 933f c065 6666 067b 743f  p.Y.sY.?.eff.{t?
 00003170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003180: e032 3333 8bf1 843f 0000 0000 0000 0000  .233...?........
-00003190: b8cc cccc 8ec1 a03f 8041 498a 9cac bd3f  .......?.AI....?
-000031a0: 2783 d697 3d50 d43f 1148 3209 ef95 da3f  '...=P.?.H2....?
+00003190: b8cc cccc 8ec1 a03f a041 498a 9cac bd3f  .......?.AI....?
+000031a0: e782 d697 3d50 d43f f147 3209 ef95 da3f  ....=P.?.G2....?
 000031b0: 0000 0000 0000 0000 0060 289b 89ae b03f  .........`(....?
 000031c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000031f0: 0000 0000 0000 0000 680c 115d 7470 d63f  ........h..]tp.?
-00003200: 0000 0000 0000 0000 f697 d073 a4b2 f83f  ...........s...?
-00003210: 910e ebeb 340b d83f 0000 0000 0000 0000  ....4..?........
+000031f0: 0000 0000 0000 0000 580c 115d 7470 d63f  ........X..]tp.?
+00003200: 0000 0000 0000 0000 0698 d073 a4b2 f83f  ...........s...?
+00003210: 710e ebeb 340b d83f 0000 0000 0000 0000  q...4..?........
 00003220: 0000 0000 0000 0000 7099 d965 e38c 983f  ........p..e...?
 00003230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003260: cd68 590c f516 0b40 e366 7356 7c3e 0940  .hY....@.fsV|>.@
 00003270: 9642 4ece 6111 f93f 0000 0000 0000 0000  .BN.a..?........
 00003280: 0000 0000 0000 0000 7eff db38 493f d23f  ........~..8I?.?
 00003290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000032a0: 0000 0000 0000 0000 0028 33e7 0d26 5e3f  .........(3..&^?
+000032a0: 0000 0000 0000 0000 0030 33e7 0d26 5e3f  .........03..&^?
 000032b0: 7099 9999 29ab 993f 0000 0000 0000 0000  p...)..?........
 000032c0: 0000 0000 0000 0000 7099 9999 ad4b 9c3f  ........p....K.?
 000032d0: c065 6666 36d0 743f b8cc cccc de57 ac3f  .eff6.t?.....W.?
-000032e0: de1b e365 f8e0 f53f 6f1d 5803 40a5 0340  ...e...?o.X.@..@
+000032e0: da1b e365 f8e0 f53f 711d 5803 40a5 0340  ...e...?q.X.@..@
 000032f0: dd7f 4b41 1215 0040 0000 0000 0000 0000  ..KA...@........
 00003300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003340: 0171 9280 602c 0340 91b8 81c8 3615 0b40  .q..`,.@....6..@
-00003350: d17d 86af a85d 0d40 2afb d8bb 4f93 fa3f  .}...].@*...O..?
+00003340: 0171 9280 602c 0340 85b8 81c8 3615 0b40  .q..`,.@....6..@
+00003350: d57d 86af a85d 0d40 2afb d8bb 4f93 fa3f  .}...].@*...O..?
 00003360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003370: f8ff df52 4043 a33f 7099 9999 4132 923f  ...R@C.?p...A2.?
 00003380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000033a0: 0000 0000 0000 0000 9e29 5af0 f334 1b40  .........)Z..4.@
-000033b0: 2c4f 98bb f08a 1b40 ca75 0e76 134d 1040  ,O.....@.u.v.M.@
+000033a0: 0000 0000 0000 0000 9a29 5af0 f334 1b40  .........)Z..4.@
+000033b0: 344f 98bb f08a 1b40 ca75 0e76 134d 1040  4O.....@.u.v.M.@
 000033c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000033d0: 9eca 44a0 56f7 d53f 0000 0000 0000 0000  ..D.V..?........
+000033d0: 8eca 44a0 56f7 d53f 0000 0000 0000 0000  ..D.V..?........
 000033e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000033f0: 2e33 33b8 3f7b f23f b8cc cccc 6635 a23f  .33.?{.?....f5.?
 00003400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003410: b8cc cccc d4e3 a23f 7099 9999 5df7 923f  .......?p...]..?
-00003420: 5c66 6666 363e b13f c58f f1d5 13b1 0040  \fff6>.?.......@
-00003430: 94c1 4527 b974 1040 79a5 6ce2 6d5e 0940  ..E'.t.@y.l.m^.@
+00003420: 5c66 6666 363e b13f c78f f1d5 13b1 0040  \fff6>.?.......@
+00003430: 96c1 4527 b974 1040 77a5 6ce2 6d5e 0940  ..E'.t.@w.l.m^.@
 00003440: 0000 0000 0000 0000 2ea3 9739 5ad9 fd3f  ...........9Z..?
 00003450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003480: 0000 0000 0000 0000 cdf2 2af8 02d9 0a40  ..........*....@
-00003490: caad 0eee ed21 1640 d21b ec11 1486 1740  .....!.@.......@
+00003480: 0000 0000 0000 0000 d5f2 2af8 02d9 0a40  ..........*....@
+00003490: ccad 0eee ed21 1640 d01b ec11 1486 1740  .....!.@.......@
 000034a0: 0914 bcdf 8b71 0240 0000 0000 0000 0000  .....q.@........
 000034b0: 0000 0000 0000 0000 7899 d9a2 76be a63f  ........x...v..?
 000034c0: 7099 9999 d9d8 9e3f 0000 0000 0000 0000  p......?........
 000034d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000034e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000034f0: fc96 5ea9 ca5d 1e40 aad8 fb35 34d9 2140  ..^..].@...54.!@
+000034f0: 0097 5ea9 ca5d 1e40 a8d8 fb35 34d9 2140  ..^..].@...54.!@
 00003500: b05a b172 077e 1a40                      .Z.r.~.@
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/2d_background.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/2d_background.npz`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 13712 bytes, number of entries: 1
-?rw-------  2.0 unx    13576 b- stor 80-Jan-01 00:00 arr_0.npy
+?rw-------  4.5 unx    13576 b- stor 80-Jan-01 00:00 arr_0.npy
 1 file, 13576 bytes uncompressed, 13576 bytes compressed:  0.0%
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v4.5 to extract, compression method=store
```

#### arr_0.npy

```diff
@@ -17,20 +17,20 @@
 00000100: 0000 00b0 1f82 0840 0000 00b0 884c 0840  .......@.....L.@
 00000110: 0000 0058 d920 0840 0000 0020 2402 0840  ...X. .@... $..@
 00000120: 0000 0090 a2f3 0740 0000 0050 6ef4 0740  .......@...Pn..@
 00000130: cdcc cccc c441 0640 cdcc cccc 6c22 0640  .....A.@....l".@
 00000140: 0000 00b8 5551 0840 0000 0038 b689 0840  ....UQ.@...8...@
 00000150: 0000 0048 7ac9 0840 1c00 c134 023d 0740  ...Hz..@...4.=.@
 00000160: 3759 1f49 1792 1740 4e02 f29b bd05 1440  7Y.I...@N......@
-00000170: 113d 9328 f8f1 0840 0000 0028 2c89 0a40  .=.(...@...(,..@
+00000170: 103d 9328 f8f1 0840 0000 0028 2c89 0a40  .=.(...@...(,..@
 00000180: f9e6 9686 e923 0b40 fca2 7983 095e f53f  .....#.@..y..^.?
 00000190: 5ec3 b8bb 7e29 0c40 0000 00b0 a6ca 0c40  ^...~).@.......@
 000001a0: 1c2c 6755 53b3 0f40 7aa6 254b 3b5a 1240  .,gUS..@z.%K;Z.@
 000001b0: 96a9 0b09 83c1 1d40 490e 07ec c7e4 1440  .......@I......@
-000001c0: b40b aeb0 de07 1440 0000 0060 cea4 0840  .......@...`...@
+000001c0: b30b aeb0 de07 1440 0000 0060 cea4 0840  .......@...`...@
 000001d0: 0000 0080 f0ad 0840 0000 0000 15be 0840  .......@.......@
 000001e0: 0000 0080 62d3 0840 0000 0090 7def 0840  ....b..@....}..@
 000001f0: 0000 0018 1d10 0940 0000 0000 cf32 0940  .......@.....2.@
 00000200: 0000 00f0 f952 0940 0000 0028 df6b 0940  .....R.@...(.k.@
 00000210: 0000 0080 f579 0940 0000 00d0 ff7b 0940  .....y.@.....{.@
 00000220: 0000 0000 7871 0940 0000 00e8 c556 0940  ....xq.@.....V.@
 00000230: 0000 0078 8f2e 0940 0000 0038 1bfc 0840  ...x...@...8...@
@@ -40,15 +40,15 @@
 00000270: 0000 00a0 b503 0840 cdcc cccc a477 0640  .......@.....w.@
 00000280: cdcc cccc 4c49 0640 0000 0088 5a5c 0840  ....LI.@....Z\.@
 00000290: 0000 0078 f291 0840 0000 00f8 76ce 0840  ...x...@....v..@
 000002a0: b1b7 5bb9 d47b 0840 2d45 8a48 8ea4 0740  ..[..{.@-E.H...@
 000002b0: 7fe6 ef58 1a2f 0840 7b07 aeb5 0db5 0940  ...X./.@{......@
 000002c0: 0000 0050 6a7b 0a40 9dfc d241 ca08 0b40  ...Pj{.@...A...@
 000002d0: 87aa f452 7db4 0b40 e461 e06b 8c0b 0c40  ...R}..@.a.k...@
-000002e0: 0000 0088 55af 0c40 fc1c 0138 6639 0d40  ....U..@...8f9.@
+000002e0: 0000 0088 55af 0c40 fd1c 0138 6639 0d40  ....U..@...8f9.@
 000002f0: 38e2 80cf 8e23 1140 7ef1 3ba8 f7a2 1240  8....#.@~.;....@
 00000300: bfe7 6ba7 3f13 1340 9e3b cc5e a3b0 1240  ..k.?..@.;.^...@
 00000310: 0000 0008 32c5 0840 0000 00a8 bfcd 0840  ....2..@.......@
 00000320: 0000 0008 bedc 0840 0000 0070 7ff0 0840  .......@...p...@
 00000330: 0000 0070 900a 0940 0000 0078 9d28 0940  ...p...@...x.(.@
 00000340: 0000 00a8 4648 0940 0000 00e0 3865 0940  ....FH.@....8e.@
 00000350: 0000 0090 fa7a 0940 0000 0028 4d86 0940  .....z.@...(M..@
@@ -82,25 +82,25 @@
 00000510: 0000 0098 4170 0840 0000 0010 8991 0840  ....Ap.@.......@
 00000520: 0000 0068 ceba 0840 0000 00a0 c0e8 0840  ...h...@.......@
 00000530: 0000 0068 491a 0940 0000 0000 f551 0940  ...hI..@.....Q.@
 00000540: 0000 0058 3c94 0940 0000 0018 16e3 0940  ...X<..@.......@
 00000550: 0000 0030 ef40 0a40 0000 0000 1fae 0a40  ...0.@.@.......@
 00000560: 0000 00b0 0b28 0b40 0000 00d0 c5ad 0b40  .....(.@.......@
 00000570: 0000 0088 803c 0c40 0000 0010 3bcb 0c40  .....<.@....;..@
-00000580: 0000 0078 324e 0d40 bbdf 65b0 a317 0e40  ...x2N.@..e....@
-00000590: 25e7 2ee7 8c92 0e40 4755 1e39 09d0 0e40  %......@GU.9...@
+00000580: 0000 0078 324e 0d40 bcdf 65b0 a317 0e40  ...x2N.@..e....@
+00000590: 26e7 2ee7 8c92 0e40 4755 1e39 09d0 0e40  &......@GU.9...@
 000005a0: 0000 0058 0e13 0940 0000 00a8 f619 0940  ...X...@.......@
 000005b0: 0000 00b8 c025 0940 0000 0070 4c35 0940  .....%.@...pL5.@
 000005c0: 0000 00a8 df49 0940 0000 0048 1061 0940  .....I.@...H.a.@
 000005d0: 0000 0068 be78 0940 0000 0048 728d 0940  ...h.x.@...Hr..@
 000005e0: 0000 00a8 879b 0940 0000 0080 90a0 0940  .......@.......@
 000005f0: 0000 0020 499c 0940 0000 0010 4e8e 0940  ... I..@....N..@
 00000600: 0000 0030 2874 0940 0000 00a0 cd50 0940  ...0(t.@.....P.@
-00000610: 7f8d 9e8e 19b1 0940 d017 be77 d7b2 f13f  .......@...w...?
-00000620: 9ef9 f3fc bf2f f33f d964 c57d a31e 0940  ...../.?.d.}...@
+00000610: 7f8d 9e8e 19b1 0940 d217 be77 d7b2 f13f  .......@...w...?
+00000620: 9cf9 f3fc bf2f f33f d964 c57d a31e 0940  ...../.?.d.}...@
 00000630: 0000 00c0 ba91 0840 0000 00f8 4880 0840  .......@....H..@
 00000640: 0000 00b0 d07a 0840 0000 0078 f57e 0840  .....z.@...x.~.@
 00000650: 0000 00d8 908b 0840 0000 00a8 e09f 0840  .......@.......@
 00000660: 0000 0098 16bb 0840 0000 00f0 22dc 0840  .......@...."..@
 00000670: 0000 00a8 2500 0940 0000 00a8 5f26 0940  ....%..@...._&.@
 00000680: 0000 0078 e451 0940 0000 0038 e287 0940  ...x.Q.@...8...@
 00000690: 0000 00a0 0fcb 0940 0000 0068 e91d 0a40  .......@...h...@
@@ -113,25 +113,25 @@
 00000700: 0000 00f0 6d53 0940 0000 00d8 9f65 0940  ....mS.@.....e.@
 00000710: 0000 0098 cb79 0940 0000 00a0 f48d 0940  .....y.@.......@
 00000720: 0000 00c0 209f 0940 0000 0080 1eaa 0940  .... ..@.......@
 00000730: 0000 0078 e7ac 0940 0000 0028 90a7 0940  ...x...@...(...@
 00000740: 0000 00b8 a899 0940 0000 0010 2f81 0940  .......@..../..@
 00000750: 0000 0048 2c61 0940 666f 3db9 6463 0940  ...H,a.@fo=.dc.@
 00000760: e16a cf24 a0c6 0640 07ba f73f cfc1 0640  .j.$...@...?...@
-00000770: 7f73 c43a f0f1 0840 0000 00b0 73c1 0840  .s.:...@....s..@
+00000770: 8073 c43a f0f1 0840 0000 00b0 73c1 0840  .s.:...@....s..@
 00000780: 0000 00a0 9cb5 0840 0000 0058 52b4 0840  .......@...XR..@
 00000790: 0000 00d0 abba 0840 0000 00e0 cbc6 0840  .......@.......@
 000007a0: 0000 0088 f6d7 0840 0000 0038 63ed 0840  .......@...8c..@
 000007b0: 90b5 258c 1506 0940 f229 72d5 6bbb 0840  ..%....@.)r.k..@
 000007c0: 90b5 159f e537 0940 0000 0070 f658 0940  .....7.@...p.X.@
 000007d0: 0000 00b8 d481 0940 0000 0018 acb8 0940  .......@.......@
-000007e0: 07fa 0a5b ace9 0940 c47d 33d4 4a35 0a40  ...[...@.}3.J5.@
-000007f0: e85e 761c bf9b 0a40 8c2b 2110 1918 0b40  .^v....@.+!....@
-00000800: ffca 3508 669e 0b40 b1a6 9132 1821 0c40  ..5.f..@...2.!.@
-00000810: 051b aae1 2392 0c40 b72a 6ca6 d4e9 0c40  ....#..@.*l....@
+000007e0: 07fa 0a5b ace9 0940 c37d 33d4 4a35 0a40  ...[...@.}3.J5.@
+000007f0: e75e 761c bf9b 0a40 8c2b 2110 1918 0b40  .^v....@.+!....@
+00000800: ffca 3508 669e 0b40 b2a6 9132 1821 0c40  ..5.f..@...2.!.@
+00000810: 041b aae1 2392 0c40 b92a 6ca6 d4e9 0c40  ....#..@.*l....@
 00000820: 4989 6de3 bd24 0d40 4936 7b9b 9340 0d40  I.m..$.@I6{..@.@
 00000830: 3333 3333 4331 0b40 0000 00d0 3753 0940  3333C1.@....7S.@
 00000840: 0000 0098 b45c 0940 0000 0008 7569 0940  .....\.@....ui.@
 00000850: 0000 0010 427a 0940 0000 00c8 8e8c 0940  ....Bz.@.......@
 00000860: 0000 0098 7a9e 0940 0000 0000 80ad 0940  ....z..@.......@
 00000870: 0000 00a0 d0b6 0940 0000 0038 b8b8 0940  .......@...8...@
 00000880: 0000 0090 90b3 0940 0000 00e8 c8a6 0940  .......@.......@
@@ -141,17 +141,17 @@
 000008c0: 0000 0048 1ff4 0840 0000 0018 f6ed 0840  ...H...@.......@
 000008d0: 0000 0018 36f1 0840 0000 0070 73fa 0840  ....6..@...ps..@
 000008e0: 0000 0008 1307 0940 0000 00d8 3f16 0940  .......@....?..@
 000008f0: 0000 0040 1227 0940 f229 e26a b6d6 0840  ...@.'.@.).j...@
 00000900: f4f2 9fd2 d169 1540 f229 b288 90f2 0840  .....i.@.).....@
 00000910: 0000 0018 4b6a 0940 0cf3 6cba 6079 0940  ....Kj.@..l.`y.@
 00000920: c301 ceb2 b674 0940 12f1 c4f9 0d90 0940  .....t.@.......@
-00000930: c8f9 47f1 17cd 0940 587a 6700 0d26 0a40  ..G....@Xzg..&.@
+00000930: c8f9 47f1 17cd 0940 597a 6700 0d26 0a40  ..G....@Yzg..&.@
 00000940: 986b 16b2 ee90 0a40 789a 2235 01fd 0a40  .k.....@x."5...@
-00000950: a4d8 eef5 f75c 0b40 ec81 f611 28a6 0b40  .....\.@....(..@
+00000950: a5d8 eef5 f75c 0b40 ec81 f611 28a6 0b40  .....\.@....(..@
 00000960: cdcc cccc ccd9 0a40 cdcc cccc dc92 0a40  .......@.......@
 00000970: cdcc cccc cc56 0a40 0000 5162 d415 0c40  .....V.@..Qb...@
 00000980: 3333 3333 e37e 0b40 0000 0058 8265 0940  3333.~.@...X.e.@
 00000990: 0000 00f8 3a72 0940 0000 00b0 d882 0940  ....:r.@.......@
 000009a0: 0000 0018 bf94 0940 0000 0060 22a6 0940  .......@...`"..@
 000009b0: 0000 0088 dfb4 0940 0000 0070 74be 0940  .......@...pt..@
 000009c0: 0000 0058 5ec1 0940 0000 0060 1cbe 0940  ...X^..@...`...@
@@ -162,18 +162,18 @@
 00000a10: 0000 0068 c825 0940 0000 0028 a72d 0940  ...h.%.@...(.-.@
 00000a20: 0000 0038 593a 0940 0000 0008 8c48 0940  ...8Y:.@.....H.@
 00000a30: 0000 0098 2f57 0940 0000 0008 1765 0940  ..../W.@.....e.@
 00000a40: 0000 0008 5871 0940 f229 a282 c219 0940  ....Xq.@.).....@
 00000a50: 0000 0008 537f 0940 0000 0028 1486 0940  ....S..@...(...@
 00000a60: a615 78cd 6459 0940 de00 4c0f 3734 0940  ..x.dY.@..L.74.@
 00000a70: 77e8 b27c 2133 0940 9160 3866 1a5c 0940  w..|!3.@.`8f.\.@
-00000a80: 1882 9ab1 dba9 0940 77a1 76e8 980f 0a40  .......@w.v....@
-00000a90: 5ab0 afde c777 0a40 ac94 faf1 f2d2 0a40  Z....w.@.......@
+00000a80: 1782 9ab1 dba9 0940 77a1 76e8 980f 0a40  .......@w.v....@
+00000a90: 59b0 afde c777 0a40 ac94 faf1 f2d2 0a40  Y....w.@.......@
 00000aa0: cdcc cccc 4c69 0a40 625f 0d7d 60bf 0940  ....Li.@b_.}`..@
-00000ab0: 8ea1 7fb7 5079 0940 cdcc cccc 4c97 0940  ....Py.@....L..@
+00000ab0: 8ca1 7fb7 5079 0940 cdcc cccc 4c97 0940  ....Py.@....L..@
 00000ac0: cccc 4cf8 33ed 0b40 3333 3333 c369 0b40  ..L.3..@3333.i.@
 00000ad0: 0000 00d0 e15b 0940 0000 0030 9269 0940  .....[.@...0.i.@
 00000ae0: 0000 0008 467b 0940 0000 00d0 548e 0940  ....F{.@....T..@
 00000af0: 0000 00b0 fda0 0940 0000 0078 69b1 0940  .......@...xi..@
 00000b00: 0000 0070 4bbd 0940 0000 0010 2ec3 0940  ...pK..@.......@
 00000b10: 0000 0010 91c3 0940 0000 00e8 50bd 0940  .......@....P..@
 00000b20: 0000 00c8 90af 0940 0000 0058 2e9d 0940  .......@...X...@
@@ -185,34 +185,34 @@
 00000b80: 0000 00f0 e0a2 0940 0000 0048 efab 0940  .......@...H...@
 00000b90: 0000 00b8 38af 0940 0000 0060 e0ac 0940  ....8..@...`...@
 00000ba0: 0000 00a0 75aa 0940 c355 6087 7c5c 0940  ....u..@.U`.|\.@
 00000bb0: cdcc cccc ecdf 0740 cdcc cccc a4ae 0740  .......@.......@
 00000bc0: cdcc cccc 44e9 0740 cdcc cccc 2c74 0840  ....D..@....,t.@
 00000bd0: cdcc cccc 9424 0940 cdcc cccc f4cc 0940  .....$.@.......@
 00000be0: cdcc cccc bc49 0a40 46b9 0a2b 9e50 0a40  .....I.@F..+.P.@
-00000bf0: 202c a62b 5cf8 fa3f 14d1 e13c e1e2 0840   ,.+\..?...<...@
+00000bf0: 1c2c a62b 5cf8 fa3f 14d1 e13c e1e2 0840  .,.+\..?...<...@
 00000c00: 2058 452a f8df 0840 0000 00e0 b42d 0940   XE*...@.....-.@
 00000c10: 0000 00e8 0734 0940 0000 00b8 f93e 0940  .....4.@.....>.@
 00000c20: 0000 0058 9b4e 0940 0000 0020 a462 0940  ...X.N.@... .b.@
 00000c30: 0000 0050 6478 0940 0000 0090 178e 0940  ...Pdx.@.......@
 00000c40: 0000 00d8 17a2 0940 0000 0040 36b2 0940  .......@...@6..@
 00000c50: 0000 00b0 e6bc 0940 0000 00f8 83c2 0940  .......@.......@
 00000c60: 0000 00a0 7ac1 0940 0000 00f0 22b9 0940  ....z..@...."..@
 00000c70: 0000 0038 25ac 0940 0000 0048 499d 0940  ...8%..@...HI..@
 00000c80: 0000 00e0 798e 0940 0000 0080 d981 0940  ....y..@.......@
 00000c90: 0000 0010 0a7a 0940 0000 00e8 0079 0940  .....z.@.....y.@
 00000ca0: 0000 00e8 2381 0940 0000 0038 d791 0940  ....#..@...8...@
 00000cb0: 0000 0068 c6a6 0940 0000 00d8 67bb 0940  ...h...@....g..@
 00000cc0: 0000 0030 dccd 0940 0000 0008 1bdc 0940  ...0...@.......@
-00000cd0: 5b02 18dc 65db 0940 239f 630e f9b5 0940  [...e..@#.c....@
+00000cd0: 5b02 18dc 65db 0940 229f 630e f9b5 0940  [...e..@".c....@
 00000ce0: 460a efb2 4bb5 0940 0000 0020 ebd4 0940  F...K..@... ...@
 00000cf0: 7157 7837 289f 0940 ccad ab81 30a1 0740  qWx7(..@....0..@
-00000d00: 1e9d b6f4 bcbd 0640 3d8a dca2 9f8c 0640  .......@=......@
+00000d00: 1f9d b6f4 bcbd 0640 3d8a dca2 9f8c 0640  .......@=......@
 00000d10: 5620 493b af2d 0740 cdcc cccc fc57 0840  V I;.-.@.....W.@
-00000d20: cdcc cccc a484 0940 1d0e 298d 2868 0b40  .......@..).(h.@
+00000d20: cdcc cccc a484 0940 1e0e 298d 2868 0b40  .......@..).(h.@
 00000d30: 271c d7d6 9fa2 0c40 547e 5730 70c3 fc3f  '......@T~W0p..?
 00000d40: 4761 904a 613c 0340 60d1 ee79 f7f1 0b40  Ga.Ja<.@`..y...@
 00000d50: 0000 0060 56ff 0840 0000 0020 6e06 0940  ...`V..@... n..@
 00000d60: 0000 0038 0613 0940 0000 0080 4825 0940  ...8...@....H%.@
 00000d70: 0000 00c0 893c 0940 0000 0010 1b56 0940  .....<.@.....V.@
 00000d80: 0000 0058 2770 0940 0000 00a8 2189 0940  ...X'p.@....!..@
 00000d90: 0000 0068 e59e 0940 0000 0028 b5af 0940  ...h...@...(...@
@@ -220,103 +220,103 @@
 00000db0: 0000 00c0 25be 0940 0000 0090 85b6 0940  ....%..@.......@
 00000dc0: 0000 0040 57ac 0940 0000 00c8 65a1 0940  ...@W..@....e..@
 00000dd0: 0000 0050 df97 0940 0000 0068 bf92 0940  ...P...@...h...@
 00000de0: 0000 00d0 4094 0940 0000 00c0 6d9f 0940  ....@..@....m..@
 00000df0: 0000 0048 b7b3 0940 0000 0070 c6cc 0940  ...H...@...p...@
 00000e00: 0000 0070 a4e5 0940 0000 0058 f3fb 0940  ...p...@...X...@
 00000e10: 4591 1770 6ddf 0940 2bf9 9f43 249c 0940  E..pm..@+..C$..@
-00000e20: 178f bfc8 23a9 0940 067b e85e 1f6a 0940  ....#..@.{.^.j.@
+00000e20: 178f bfc8 23a9 0940 057b e85e 1f6a 0940  ....#..@.{.^.j.@
 00000e30: d121 39e9 c85a 0940 b52f 2d5d 9784 0940  .!9..Z.@./-]...@
 00000e40: e857 27cb 975e 0740 b743 0ea6 16d9 0540  .W'..^.@.C.....@
 00000e50: f207 dce7 2530 0540 107a 1174 1ad0 0540  ....%0.@.z.t...@
-00000e60: 4181 c9be 3282 0740 cdcc cccc 54b5 0940  A...2..@....T..@
-00000e70: 132f e04e 0820 0c40 bfdd e08e 7161 0b40  ./.N. .@....qa.@
-00000e80: 1829 6b77 f047 0940 3013 aad6 1770 fa3f  .)kw.G.@0....p.?
-00000e90: de9b 4158 c4ef 0140 0000 00d0 30c8 0840  ..AX...@....0..@
+00000e60: 3f81 c9be 3282 0740 cdcc cccc 54b5 0940  ?...2..@....T..@
+00000e70: 142f e04e 0820 0c40 bfdd e08e 7161 0b40  ./.N. .@....qa.@
+00000e80: 1829 6b77 f047 0940 3613 aad6 1770 fa3f  .)kw.G.@6....p.?
+00000e90: dd9b 4158 c4ef 0140 0000 00d0 30c8 0840  ..AX...@....0..@
 00000ea0: 0000 0080 3cd0 0840 0000 0008 ddde 0840  ....<..@.......@
 00000eb0: 0000 0038 46f4 0840 0000 00b8 670f 0940  ...8F..@....g..@
 00000ec0: 0000 0008 962d 0940 0000 0050 d94c 0940  .....-.@...P.L.@
 00000ed0: 0000 0030 a36b 0940 0000 0008 c987 0940  ...0.k.@.......@
 00000ee0: 0000 00e0 489f 0940 0000 0098 dfb1 0940  ....H..@.......@
 00000ef0: 0000 0020 ebbc 0940 0000 0008 ebbf 0940  ... ...@.......@
 00000f00: 0000 0030 f0bc 0940 0000 0020 59b6 0940  ...0...@... Y..@
 00000f10: 0000 00b8 eaad 0940 0000 00f0 f3a5 0940  .......@.......@
 00000f20: 0000 0060 eca1 0940 0000 00b0 78a4 0940  ...`...@....x..@
 00000f30: 0000 0048 64b1 0940 0000 0050 4dc8 0940  ...Hd..@...PM..@
 00000f40: 0000 00e0 02e5 0940 0000 0028 4602 0a40  .......@...(F..@
 00000f50: 1586 2a96 7e01 0a40 30fc 4cb3 08e2 0940  ..*.~..@0.L....@
-00000f60: c644 b379 c39b 0b40 45b2 1c82 687b 0c40  .D.y...@E...h{.@
-00000f70: 1520 d761 6886 0b40 d44b caec dab2 0940  . .ah..@.K.....@
-00000f80: 9379 1f03 5c4b 0940 4154 7680 5866 0940  .y..\K.@ATv.Xf.@
+00000f60: c844 b379 c39b 0b40 45b2 1c82 687b 0c40  .D.y...@E...h{.@
+00000f70: 1420 d761 6886 0b40 d44b caec dab2 0940  . .ah..@.K.....@
+00000f80: 9379 1f03 5c4b 0940 4254 7680 5866 0940  .y..\K.@BTv.Xf.@
 00000f90: b0ee 1bad 4c3d 0540 2d3a 0035 f14c 0440  ....L=.@-:.5.L.@
-00000fa0: 3007 1bd6 7717 0540 8125 b22b eb32 0740  0...w..@.%.+.2.@
-00000fb0: 7956 b71b 5701 0a40 b97e afa5 b2fb 0b40  yV..W..@.~.....@
-00000fc0: 7a5e be4d f10c 0c40 3a3b 27ca c526 1040  z^.M...@:;'..&.@
-00000fd0: 210f f1da 020b 1240 58c5 2f5d b84e 1240  !......@X./].N.@
+00000fa0: 3007 1bd6 7717 0540 7f25 b22b eb32 0740  0...w..@.%.+.2.@
+00000fb0: 7856 b71b 5701 0a40 b87e afa5 b2fb 0b40  xV..W..@.~.....@
+00000fc0: 785e be4d f10c 0c40 3a3b 27ca c526 1040  x^.M...@:;'..&.@
+00000fd0: 1f0f f1da 020b 1240 58c5 2f5d b84e 1240  .......@X./].N.@
 00000fe0: 0000 0038 768f 0840 0000 00f8 7398 0840  ...8v..@....s..@
 00000ff0: 0000 0058 20a9 0840 0000 00b0 b1c1 0840  ...X ..@.......@
 00001000: 0000 0028 bde0 0840 0000 0058 a903 0940  ...(...@...X...@
 00001010: 0000 0088 5328 0940 0000 0018 184d 0940  ....S(.@.....M.@
 00001020: 0000 0068 c06f 0940 0000 0060 fc8d 0940  ...h.o.@...`...@
 00001030: 0000 0098 1ba7 0940 0000 0040 efb7 0940  .......@...@...@
 00001040: 0000 00a0 eebf 0940 0000 0028 cec0 0940  .......@...(...@
 00001050: 0000 0078 bdbc 0940 0000 00e0 90b5 0940  ...x...@.......@
 00001060: 0000 0030 bead 0940 0000 0078 4aa9 0940  ...0...@...xJ..@
 00001070: 0000 0080 60ab 0940 0000 00c0 9cb8 0940  ....`..@.......@
 00001080: 0000 00e8 e5d0 0940 0000 00b0 59f0 0940  .......@....Y..@
 00001090: 0000 0010 9c11 0a40 0dce 396d 61d2 0940  .......@..9ma..@
-000010a0: 513e 55d7 5741 0a40 48aa df5c d82d 0d40  Q>U.WA.@H..\.-.@
+000010a0: 523e 55d7 5741 0a40 47aa df5c d82d 0d40  R>U.WA.@G..\.-.@
 000010b0: 5671 e6af 93d6 0b40 2ab7 8bff 7343 1440  Vq.....@*...sC.@
-000010c0: 911f 2350 8ca1 0340 fabe 71cb 32b7 0840  ..#P...@..q.2..@
-000010d0: ff7b 3cf9 48ff 0840 9cf1 de4c 3d66 f73f  .{<.H..@...L=f.?
-000010e0: f534 5dda c87e 0440 9795 7e3c ca54 0540  .4]..~.@..~<.T.@
-000010f0: 5ab1 f0a5 d495 0740 bc71 39fd 4bb9 0b40  Z......@.q9.K..@
+000010c0: 901f 2350 8ca1 0340 f9be 71cb 32b7 0840  ..#P...@..q.2..@
+000010d0: fe7b 3cf9 48ff 0840 9cf1 de4c 3d66 f73f  .{<.H..@...L=f.?
+000010e0: f734 5dda c87e 0440 9695 7e3c ca54 0540  .4]..~.@..~<.T.@
+000010f0: 5ab1 f0a5 d495 0740 bd71 39fd 4bb9 0b40  Z......@.q9.K..@
 00001100: ce6e 4a20 6f16 0c40 85eb 07fa c923 1140  .nJ o..@.....#.@
-00001110: c85b f7d5 451e 0240 2493 7c6f e7a0 1a40  .[..E..@$.|o...@
+00001110: c65b f7d5 451e 0240 2293 7c6f e7a0 1a40  .[..E..@".|o...@
 00001120: 2cc5 b265 f91e 1b40 cdcc cccc 5c9f 0640  ,..e...@....\..@
 00001130: 0000 0078 4763 0840 0000 0088 af75 0840  ...xGc.@.....u.@
 00001140: 0000 00d0 f390 0840 0000 0050 62b3 0840  .......@...Pb..@
 00001150: 0000 00d0 84da 0840 0000 00b8 0e04 0940  .......@.......@
 00001160: 0000 0058 3e2e 0940 0000 00d0 da56 0940  ...X>..@.....V.@
 00001170: 0000 0038 4e7b 0940 0000 00e0 749a 0940  ...8N{.@....t..@
 00001180: 0000 00a0 9ab0 0940 0000 00a8 1ebd 0940  .......@.......@
 00001190: 047a 10e0 7655 0940 2eab 0de3 9e42 0940  .z..vU.@.....B.@
 000011a0: 9e5b aa1a 7745 0940 0000 0078 82b0 0940  .[..wE.@...x...@
 000011b0: 0000 0070 f2aa 0940 0000 00c0 cfab 0940  ...p...@.......@
 000011c0: 0000 00e0 80b8 0940 0000 0040 41d1 0940  .......@...@A..@
 000011d0: 0000 0028 98f2 0940 0000 0080 3017 0a40  ...(...@....0..@
-000011e0: 365f 692e 9ab7 0940 8c03 7f66 1e5a 0c40  6_i....@...f.Z.@
-000011f0: dcd4 003a dbfb 0c40 3a47 1a59 e860 1a40  ...:...@:G.Y.`.@
-00001200: 555b d277 2368 2140 e8a8 e131 23b4 2040  U[.w#h!@...1#. @
-00001210: 1bc6 4773 0b46 0540 dd51 57eb 732f 0940  ..Gs.F.@.QW.s/.@
-00001220: b0bf e0a7 ecf9 0640 9573 98f3 51ea 0540  .......@.s..Q..@
-00001230: 3a17 9a37 5779 0640 9c18 c406 ba8b 0840  :..7Wy.@.......@
-00001240: 3d15 fd6c 4eca 0b40 3994 68c6 1b88 0c40  =..lN..@9.h....@
-00001250: e194 e0eb 5054 0f40 1bcc ec29 d005 2340  ....PT.@...)..#@
+000011e0: 365f 692e 9ab7 0940 8d03 7f66 1e5a 0c40  6_i....@...f.Z.@
+000011f0: dbd4 003a dbfb 0c40 3c47 1a59 e860 1a40  ...:...@<G.Y.`.@
+00001200: 565b d277 2368 2140 e7a8 e131 23b4 2040  V[.w#h!@...1#. @
+00001210: 1ec6 4773 0b46 0540 dd51 57eb 732f 0940  ..Gs.F.@.QW.s/.@
+00001220: b0bf e0a7 ecf9 0640 9473 98f3 51ea 0540  .......@.s..Q..@
+00001230: 3817 9a37 5779 0640 9a18 c406 ba8b 0840  8..7Wy.@.......@
+00001240: 3d15 fd6c 4eca 0b40 3b94 68c6 1b88 0c40  =..lN..@;.h....@
+00001250: e194 e0eb 5054 0f40 1ccc ec29 d005 2340  ....PT.@...)..#@
 00001260: 7d87 7fef 4e00 2f40 593f 1639 f027 2540  }...N./@Y?.9.'%@
 00001270: cdcc cccc 2487 0640 0000 0048 3635 0840  ....$..@...H65.@
 00001280: 0000 00f0 9448 0840 0000 0078 7465 0840  .....H.@...xte.@
 00001290: 0000 0020 fe89 0840 0000 00d0 f6b3 0840  ... ...@.......@
 000012a0: 0000 00a0 f9e0 0840 0000 0078 2f0f 0940  .......@...x/..@
 000012b0: 0000 00d8 7a3c 0940 0000 0030 1966 0940  ....z<.@...0.f.@
 000012c0: 0000 0058 798a 0940 0000 00c8 6fa5 0940  ...Xy..@....o..@
 000012d0: 0000 0000 31b6 0940 9409 30b9 4842 0940  ....1..@..0.HB.@
 000012e0: 5300 ca40 ce26 1a40 9431 74a9 ef35 0940  S..@.&.@.1t..5.@
 000012f0: 0000 00c8 d0af 0940 0000 0048 55a9 0940  .......@...HU..@
 00001300: 0000 0050 fea8 0940 0000 0088 e1b4 0940  ...P...@.......@
 00001310: cdcc cccc ecd9 0740 0000 0098 0ff0 0940  .......@.......@
-00001320: 0000 00a8 2e17 0a40 b89d 94b9 4cb1 0940  .......@....L..@
-00001330: a909 93db 905a 0c40 2b17 b450 614a 0c40  .....Z.@+..PaJ.@
+00001320: 0000 00a8 2e17 0a40 b99d 94b9 4cb1 0940  .......@....L..@
+00001330: aa09 93db 905a 0c40 2c17 b450 614a 0c40  .....Z.@,..PaJ.@
 00001340: e2b8 54a4 98fa 1e40 0a58 6841 d148 2140  ..T....@.XhA.H!@
-00001350: ae29 a328 8d5c 1740 1f4f f374 2a3f 0740  .).(.\.@.O.t*?.@
-00001360: 10e7 3de5 54be 0940 7508 4418 addd 0940  ..=.T..@u.D....@
-00001370: c5d5 3afb dfc1 0740 8832 b553 140b 0840  ..:....@.2.S...@
-00001380: b572 bbf6 b6ce 0940 27cc 16d5 af1a 0c40  .r.....@'......@
-00001390: e9a6 1d94 83f3 0e40 fe6c a1ee b50f 1040  .......@.l.....@
-000013a0: dc5a b5fa f040 2040 0817 8bb1 0dd9 2340  .Z...@ @......#@
+00001350: ae29 a328 8d5c 1740 224f f374 2a3f 0740  .).(.\.@"O.t*?.@
+00001360: 11e7 3de5 54be 0940 7508 4418 addd 0940  ..=.T..@u.D....@
+00001370: c5d5 3afb dfc1 0740 8632 b553 140b 0840  ..:....@.2.S...@
+00001380: b572 bbf6 b6ce 0940 26cc 16d5 af1a 0c40  .r.....@&......@
+00001390: e9a6 1d94 83f3 0e40 fc6c a1ee b50f 1040  .......@.l.....@
+000013a0: dc5a b5fa f040 2040 0617 8bb1 0dd9 2340  .Z...@ @......#@
 000013b0: c60e e2c3 c47f 2140 0000 00a8 a30a 0840  ......!@.......@
 000013c0: 0000 00c8 8514 0840 0000 00d0 ba27 0840  .......@.....'.@
 000013d0: 0000 0010 a044 0840 0000 0040 6569 0840  .....D.@...@ei.@
 000013e0: 0000 0010 2594 0840 0000 0050 81c2 0840  ....%..@...P...@
 000013f0: 0000 0050 a7f2 0840 0000 0098 c022 0940  ...P...@.....".@
 00001400: 0000 0008 0450 0940 0000 0060 8278 0940  .....P.@...`.x.@
 00001410: 0000 0080 ac97 0940 0000 00f8 7cac 0940  .......@....|..@
@@ -324,526 +324,526 @@
 00001430: 9e13 9fd8 de3c 0940 0000 00e8 48af 0940  .....<.@....H..@
 00001440: 0000 00f8 dda8 0940 0000 0078 19a8 0940  .......@...x...@
 00001450: cdcc cccc 54e4 0740 cdcc cccc c49c 0740  ....T..@.......@
 00001460: cdcc cccc ccfa 0740 0000 00f0 5d18 0a40  .......@....]..@
 00001470: b27e ae8c 10d1 0940 cc92 10db 340b 0a40  .~.....@....4..@
 00001480: db2c c699 dbe5 0a40 5805 7f74 fb00 1740  .,.....@X..t...@
 00001490: 78b0 2656 75d0 1540 b993 e1d9 f359 0840  x.&Vu..@.....Y.@
-000014a0: 2cf4 80f2 f170 0940 9528 dd28 7411 0a40  ,....p.@.(.(t..@
+000014a0: 2af4 80f2 f170 0940 9428 dd28 7411 0a40  *....p.@.(.(t..@
 000014b0: 91e8 bcf3 7425 0a40 cdcc cccc 34e3 0840  ....t%.@....4..@
-000014c0: cdcc cccc 5c2e 0940 b4ab 084f f423 0b40  ....\..@...O.#.@
-000014d0: 675c c5a4 a19f 0c40 5ef0 2e51 74ac 0c40  g\.....@^..Qt..@
-000014e0: 71cf 6f67 7060 1140 9a6c 022e 2efa 1040  q.ogp`.@.l.....@
-000014f0: c818 9828 1f65 1140 16e7 737e cf16 1240  ...(.e.@..s~...@
+000014c0: cdcc cccc 5c2e 0940 b5ab 084f f423 0b40  ....\..@...O.#.@
+000014d0: 675c c5a4 a19f 0c40 5cf0 2e51 74ac 0c40  g\.....@\..Qt..@
+000014e0: 72cf 6f67 7060 1140 9a6c 022e 2efa 1040  r.ogp`.@.l.....@
+000014f0: ca18 9828 1f65 1140 16e7 737e cf16 1240  ...(.e.@..s~...@
 00001500: 0000 00b8 45fe 0740 0000 0008 3e07 0840  ....E..@....>..@
 00001510: 0000 0040 0119 0840 0000 00d8 1e34 0840  ...@...@.....4.@
 00001520: 0000 0050 fe56 0840 0000 0050 3380 0840  ...P.V.@...P3..@
 00001530: 0000 00a8 8ead 0840 0000 00f0 63dd 0840  .......@....c..@
 00001540: 0000 0060 520e 0940 0000 00f8 b13d 0940  ...`R..@.....=.@
 00001550: 0000 0018 4569 0940 0000 00b0 2d8c 0940  ....Ei.@....-..@
 00001560: 0000 0098 1ba5 0940 0000 0068 25b4 0940  .......@...h%..@
 00001570: 0000 0088 a3ba 0940 0000 0010 81ba 0940  .......@.......@
 00001580: 0000 0040 7db5 0940 0000 00f0 90b0 0940  ...@}..@.......@
 00001590: 0000 0078 9eb0 0940 cdcc cccc fcdf 0740  ...x...@.......@
 000015a0: cdcc cccc 9493 0740 cdcc cccc b4d9 0740  .......@.......@
 000015b0: 2bb2 3370 82f2 0940 e748 a8f5 ea23 0a40  +.3p...@.H...#.@
 000015c0: 2a60 29a7 a8f1 0940 f265 119c 7bf8 0940  *`)....@.e..{..@
-000015d0: 968c ba3c 632a 0a40 94a7 7335 5f2c 0a40  ...<c*.@..s5_,.@
-000015e0: 88a6 91d7 dbd7 0940 0e03 1471 27f3 0940  .......@...q'..@
-000015f0: 97f6 9863 b185 0a40 0ee4 e9cf 422f 0a40  ...c...@....B/.@
+000015d0: 978c ba3c 632a 0a40 94a7 7335 5f2c 0a40  ...<c*.@..s5_,.@
+000015e0: 87a6 91d7 dbd7 0940 0f03 1471 27f3 0940  .......@...q'..@
+000015f0: 97f6 9863 b185 0a40 0de4 e9cf 422f 0a40  ...c...@....B/.@
 00001600: cdcc cccc d429 0940 cdcc cccc bc8c 0940  .....).@.......@
 00001610: 96fc 8158 9af2 0a40 c6ce 2de1 8379 0c40  ...X...@..-..y.@
-00001620: 95cb 0901 524d 0d40 aea0 1d13 1f81 0f40  ....RM.@.......@
-00001630: 9ee8 1c59 69c2 1040 ed2b 9b68 ce71 1140  ...Yi..@.+.h.q.@
+00001620: 93cb 0901 524d 0d40 b0a0 1d13 1f81 0f40  ....RM.@.......@
+00001630: 9de8 1c59 69c2 1040 ed2b 9b68 ce71 1140  ...Yi..@.+.h.q.@
 00001640: 10a6 1c81 54ac 1140 0000 0098 1d0b 0840  ....T..@.......@
 00001650: 0000 0088 6f12 0840 0000 0080 5a21 0840  ....o..@....Z!.@
 00001660: 0000 0050 b838 0840 0000 0020 5e57 0840  ...P.8.@... ^W.@
 00001670: 0000 00b8 7d7c 0840 0000 00f8 49a6 0840  ....}|.@....I..@
 00001680: 0000 00e0 64d3 0840 0000 0018 1303 0940  ....d..@.......@
 00001690: 0000 0068 f232 0940 0000 00f0 8560 0940  ...h.2.@.....`.@
 000016a0: 0000 0090 b786 0940 0000 0008 dea3 0940  .......@.......@
 000016b0: 0000 0038 a3b7 0940 0000 0030 09c3 0940  ...8...@...0...@
 000016c0: 0000 0020 cac7 0940 0000 0060 ffc6 0940  ... ...@...`...@
 000016d0: 0000 0008 60c5 0940 0d29 3724 a8a7 0940  ....`..@.)7$...@
 000016e0: cdcc cccc 6ce4 0740 cdcc cccc 9c91 0740  ....l..@.......@
-000016f0: 37b7 12a9 e4b7 0740 cdcc cccc ac6b 0840  7......@.....k.@
-00001700: 5269 51a6 d13a 0a40 0965 1367 df6b 0a40  RiQ..:.@.e.g.k.@
+000016f0: 36b7 12a9 e4b7 0740 cdcc cccc ac6b 0840  6......@.....k.@
+00001700: 5169 51a6 d13a 0a40 0965 1367 df6b 0a40  QiQ..:.@.e.g.k.@
 00001710: de58 b180 0a50 0a40 6270 8857 7d4c 0a40  .X...P.@bp.W}L.@
 00001720: 39e1 1c72 b63c 0a40 31ec 728b 423f 0a40  9..r.<.@1.r.B?.@
 00001730: 2b29 a3a8 c992 0a40 23cf 46c8 ac80 0a40  +).....@#.F....@
 00001740: cdcc cccc 4453 0940 cdcc cccc f412 0940  ....DS.@.......@
 00001750: cdcc cccc 9476 0940 cdcc cccc c477 0a40  .....v.@.....w.@
 00001760: 75f0 fae5 80b2 0b40 762f 1849 4222 0d40  u......@v/.IB".@
-00001770: fed7 244f 0207 0e40 ee3f 7590 63e9 0d40  ..$O...@.?u.c..@
-00001780: 352e 05aa 8deb 0d40 83b8 b8c6 96e3 0d40  5......@.......@
+00001770: fed7 244f 0207 0e40 ec3f 7590 63e9 0d40  ..$O...@.?u.c..@
+00001780: 352e 05aa 8deb 0d40 81b8 b8c6 96e3 0d40  5......@.......@
 00001790: 0000 0020 6734 0840 0000 0048 3c39 0840  ... g4.@...H<9.@
 000017a0: 0000 0058 b543 0840 0000 00a0 0f55 0840  ...X.C.@.....U.@
 000017b0: 0000 0048 cb6c 0840 0000 0010 ea8a 0840  ...H.l.@.......@
 000017c0: 0000 0078 42ae 0840 0000 00e0 f3d5 0840  ...xB..@.......@
 000017d0: 0000 0090 1802 0940 0000 00e8 b330 0940  .......@.....0.@
 000017e0: 0000 0010 195f 0940 0000 0010 1488 0940  ....._.@.......@
 000017f0: 0000 0030 96a9 0940 0000 00d8 dac2 0940  ...0...@.......@
 00001800: 0000 0010 76d4 0940 0000 00b8 d8df 0940  ....v..@.......@
 00001810: 0000 00d0 54e5 0940 0000 0050 3de9 0940  ....T..@...P=..@
 00001820: 7b5b eb09 70bb 0940 cdcc cccc ccf3 0740  {[..p..@.......@
-00001830: f96c 41a4 878b 0740 6339 d0c5 cc82 0740  .lA....@c9.....@
+00001830: f76c 41a4 878b 0740 6239 d0c5 cc82 0740  .lA....@b9.....@
 00001840: cdcc cccc 6c17 0840 cdcc cccc 84b6 0840  ....l..@.......@
-00001850: 5892 8ff4 3065 0a40 04f9 4bed 79d5 0a40  X...0e.@..K.y..@
-00001860: 3961 1600 e6e7 0a40 6be1 cd11 cced 0a40  9a.....@k......@
+00001850: 5992 8ff4 3065 0a40 02f9 4bed 79d5 0a40  Y...0e.@..K.y..@
+00001860: 3961 1600 e6e7 0a40 6ae1 cd11 cced 0a40  9a.....@j......@
 00001870: 48a4 559f 19f4 0a40 b723 fcee b1ba 0a40  H.U....@.#.....@
 00001880: cdcc cccc 3c50 0940 cdcc cccc 1c00 0940  ....<P.@.......@
-00001890: 2c8d d354 e6d7 0840 53ff 4d05 9210 0940  ,..T...@S.M....@
-000018a0: 1e6b 3083 55c3 0940 cdcc cccc 0ca5 0a40  .k0.U..@.......@
+00001890: 2c8d d354 e6d7 0840 52ff 4d05 9210 0940  ,..T...@R.M....@
+000018a0: 1d6b 3083 55c3 0940 cdcc cccc 0ca5 0a40  .k0.U..@.......@
 000018b0: cdcc cccc dc9a 0b40 ce59 e235 5449 0c40  .......@.Y.5TI.@
-000018c0: 9933 3572 1974 0c40 3de5 3c2e 0478 0c40  .35r.t.@=.<..x.@
+000018c0: 9733 3572 1974 0c40 3de5 3c2e 0478 0c40  .35r.t.@=.<..x.@
 000018d0: 9862 5646 4856 0c40 cbcb c600 5768 0840  .bVFHV.@....Wh.@
 000018e0: b6d5 3249 7270 0840 0000 0000 0280 0840  ..2Irp.@.......@
 000018f0: 0000 0060 c088 0840 0000 0008 8196 0840  ...`...@.......@
 00001900: 0000 0010 55aa 0840 0000 0010 07c4 0840  ....U..@.......@
 00001910: 0000 0080 6fe3 0840 0000 0020 b009 0940  ....o..@... ...@
 00001920: 0000 0050 4e35 0940 0000 0008 7a63 0940  ...PN5.@....zc.@
 00001930: 0000 00d8 f48e 0940 0000 0028 3bb5 0940  .......@...(;..@
 00001940: 0000 00e8 12d5 0940 0000 0078 82ee 0940  .......@...x...@
 00001950: 0000 0040 9202 0a40 0000 00a0 b410 0a40  ...@...@.......@
 00001960: 0000 00d8 c01c 0a40 af15 6b7f 4ff4 0940  .......@..k.O..@
 00001970: cdcc cccc 9c30 0840 3f76 237e dcc4 0740  .....0.@?v#~...@
-00001980: 8ed6 7829 e194 0740 ac36 33ee a8f0 0740  ..x)...@.63....@
+00001980: 8dd6 7829 e194 0740 aa36 33ee a8f0 0740  ..x)...@.63....@
 00001990: cdcc cccc ac6e 0840 cdcc cccc c4ef 0840  .....n.@.......@
 000019a0: cdcc cccc 9464 0940 cdcc cccc f4ad 0940  .....d.@.......@
 000019b0: cdcc cccc 7cca 0940 cdcc cccc acc1 0940  ....|..@.......@
 000019c0: cdcc cccc ac97 0940 cdcc cccc 4c5e 0940  .......@....L^.@
-000019d0: cdcc cccc 7434 0940 9783 fd2f 8aec 0840  ....t4.@.../...@
-000019e0: 465d ccc0 1d80 0840 b7cd 968c 717c 0840  F].....@....q|.@
-000019f0: 89c6 b482 e024 0940 5544 bb67 8503 0a40  .....$.@UD.g...@
-00001a00: 28c2 d915 1e71 0a40 de6b ea76 fa67 0a40  (....q.@.k.v.g.@
-00001a10: 5fd6 f701 0f31 0a40 92bd ef7a 12e2 0940  _....1.@...z...@
+000019d0: cdcc cccc 7434 0940 9683 fd2f 8aec 0840  ....t4.@.../...@
+000019e0: 455d ccc0 1d80 0840 b8cd 968c 717c 0840  E].....@....q|.@
+000019f0: 88c6 b482 e024 0940 5444 bb67 8503 0a40  .....$.@TD.g...@
+00001a00: 26c2 d915 1e71 0a40 de6b ea76 fa67 0a40  &....q.@.k.v.g.@
+00001a10: 5ed6 f701 0f31 0a40 92bd ef7a 12e2 0940  ^....1.@...z...@
 00001a20: 1b4e 806b 5bac 0840 ffa2 eb57 6ab3 0840  .N.k[..@...Wj..@
 00001a30: 95e9 035a 96c0 0840 800b d0a2 f3d0 0840  ...Z...@.......@
 00001a40: 0000 0038 9dd3 0840 0000 0078 c8d9 0840  ...8...@...x...@
 00001a50: 0000 0000 7ce6 0840 03a8 15e0 f4f1 0840  ....|..@.......@
-00001a60: 0346 a73f 0501 0940 996f 8787 d323 0940  .F.?...@.o...#.@
+00001a60: 0446 a73f 0501 0940 996f 8787 d323 0940  .F.?...@.o...#.@
 00001a70: 0993 0f79 855f 0940 0000 00a8 b898 0940  ...y._.@.......@
 00001a80: 0000 0028 cac3 0940 0000 00e8 efea 0940  ...(...@.......@
 00001a90: 0000 0028 870d 0a40 0000 00e0 102c 0a40  ...(...@.....,.@
 00001aa0: 0000 0068 1245 0a40 0000 00f8 d75b 0a40  ...h.E.@.....[.@
-00001ab0: d738 e7fe 0752 0a40 cdcc cccc 14cd 0840  .8...R.@.......@
+00001ab0: d838 e7fe 0752 0a40 cdcc cccc 14cd 0840  .8...R.@.......@
 00001ac0: cdcc cccc 7c5c 0840 cdcc cccc 0c39 0840  ....|\.@.....9.@
 00001ad0: cdcc cccc 4c64 0840 cdcc cccc 0cb0 0840  ....Ld.@.......@
 00001ae0: cdcc cccc 0422 0940 cdcc cccc 0c98 0940  .....".@.......@
 00001af0: cdcc cccc 54f3 0940 cdcc cccc d42e 0a40  ....T..@.......@
 00001b00: cdcc cccc dc46 0a40 cdcc cccc ac3e 0a40  .....F.@.....>.@
 00001b10: cdcc cccc f41d 0a40 cdcc cccc 3cf7 0940  .......@....<..@
-00001b20: 27da 4a57 dabf 0940 4f31 2b1c 0ac2 0840  '.JW...@O1+....@
-00001b30: b6b1 f896 3928 f73f ac82 5fb6 c98b 0840  ....9(.?.._....@
-00001b40: c65a 7e62 a155 0940 9ed7 1262 d7b0 0940  .Z~b.U.@...b...@
+00001b20: 26da 4a57 dabf 0940 4d31 2b1c 0ac2 0840  &.JW...@M1+....@
+00001b30: b8b1 f896 3928 f73f ab82 5fb6 c98b 0840  ....9(.?.._....@
+00001b40: c55a 7e62 a155 0940 9ed7 1262 d7b0 0940  .Z~b.U.@...b...@
 00001b50: ff6e 2b59 b073 0940 f161 4f06 67b7 0840  .n+Y.s.@.aO.g..@
-00001b60: 1a9b fc6c a0dd 0740 9754 a8c7 2716 0940  ...l...@.T..'..@
+00001b60: 1b9b fc6c a0dd 0740 9754 a8c7 2716 0940  ...l...@.T..'..@
 00001b70: a6c1 ace7 de1b 0940 8474 f386 9924 0940  .......@.t...$.@
 00001b80: 1c26 41f6 b22a 0940 0000 00f8 9b23 0940  .&A..*.@.....#.@
 00001b90: 0000 00c8 0d19 0940 a7bd 8a19 7a02 0940  .......@....z..@
 00001ba0: b98b 0bcb 85ea 0840 abbf e4d1 bff2 0840  .......@.......@
 00001bb0: c5ec 1a0e a475 0940 d0d4 a874 bdb2 0940  .....u.@...t...@
 00001bc0: 7ed4 bc08 b7a1 0940 0000 0000 bcd3 0940  ~......@.......@
 00001bd0: 0000 0060 0b02 0a40 0000 0058 212e 0a40  ...`...@...X!..@
 00001be0: 0000 00b8 e257 0a40 0000 0088 ee7c 0a40  .....W.@.....|.@
 00001bf0: 0000 0010 0ca0 0a40 0000 0020 8dc6 0a40  .......@... ...@
 00001c00: bca1 e694 22ac 0a40 cdcc cccc 646b 0940  ...."..@....dk.@
 00001c10: cdcc cccc 1c3f 0940 cdcc cccc ec5b 0940  .....?.@.....[.@
 00001c20: cdcc cccc eca5 0940 8bdc b713 d616 0a40  .......@.......@
-00001c30: 4089 307a 62fc 0b40 5a80 0fb1 fb01 0c40  @.0zb..@Z......@
-00001c40: a4ae 12ac e818 0c40 17cf 0478 6408 0c40  .......@...xd..@
-00001c50: 14a9 fccc 44ca 0b40 7ff7 e488 f575 0b40  ....D..@.....u.@
+00001c30: 4089 307a 62fc 0b40 5980 0fb1 fb01 0c40  @.0zb..@Y......@
+00001c40: a4ae 12ac e818 0c40 16cf 0478 6408 0c40  .......@...xd..@
+00001c50: 14a9 fccc 44ca 0b40 7ef7 e488 f575 0b40  ....D..@~....u.@
 00001c60: 46c4 4ca8 3e2a 0b40 cdcc cccc 0cdc 0a40  F.L.>*.@.......@
-00001c70: 66c7 e90e e64b 0a40 e424 f4f6 9ea4 0940  f....K.@.$.....@
-00001c80: 6733 e845 31c9 0940 f986 ecb7 1650 0a40  g3.E1..@.....P.@
-00001c90: c7a3 896c 6b9b 0a40 dc92 e85c 9f24 0a40  ...lk..@...\.$.@
-00001ca0: 6100 9c1c 4b93 0840 943a d4f7 d4e1 0140  a...K..@.:.....@
-00001cb0: 1141 89f2 a9d1 0940 a9a2 2673 9ad0 0940  .A.....@..&s...@
+00001c70: 67c7 e90e e64b 0a40 e424 f4f6 9ea4 0940  g....K.@.$.....@
+00001c80: 6633 e845 31c9 0940 f886 ecb7 1650 0a40  f3.E1..@.....P.@
+00001c90: c5a3 896c 6b9b 0a40 dc92 e85c 9f24 0a40  ...lk..@...\.$.@
+00001ca0: 6100 9c1c 4b93 0840 953a d4f7 d4e1 0140  a...K..@.:.....@
+00001cb0: 1241 89f2 a9d1 0940 a9a2 2673 9ad0 0940  .A.....@..&s...@
 00001cc0: 0000 00f8 a1c3 0940 0000 0068 a4a4 0940  .......@...h...@
 00001cd0: 0000 0070 b083 0940 0000 00b0 3666 0940  ...p...@....6f.@
-00001ce0: 9170 e1be 6b30 0940 15bb ae80 e0fa 0840  .p..k0.@.......@
-00001cf0: 50a2 da36 104e 0940 d26c 2f8c 2473 f13f  P..6.N.@.l/.$s.?
+00001ce0: 9370 e1be 6b30 0940 15bb ae80 e0fa 0840  .p..k0.@.......@
+00001cf0: 50a2 da36 104e 0940 d46c 2f8c 2473 f13f  P..6.N.@.l/.$s.?
 00001d00: 9e07 f0e5 4728 f63f bc5a 933e 7cd9 0940  ....G(.?.Z.>|..@
 00001d10: 0000 0038 52e3 0940 0000 00b0 9e17 0a40  ...8R..@.......@
 00001d20: 0000 00e0 604c 0a40 0000 0010 de80 0a40  ....`L.@.......@
 00001d30: 0000 00d0 edb1 0a40 0000 0090 e9e1 0a40  .......@.......@
 00001d40: 0000 0030 2a16 0b40 86bc c66a bb45 0b40  ...0*..@...j.E.@
-00001d50: a0fc e3d4 323a 0b40 4770 103c 3f51 0b40  ....2:.@Gp.<?Q.@
+00001d50: a0fc e3d4 323a 0b40 4870 103c 3f51 0b40  ....2:.@Hp.<?Q.@
 00001d60: 4c55 a1b0 3095 0b40 43e7 2c84 164f 0c40  LU..0..@C.,..O.@
-00001d70: 9a85 42d4 8c06 0c40 c453 7d2f c576 0b40  ..B....@.S}/.v.@
-00001d80: 9c00 2be5 c6b4 0b40 2efe 7e4c cc9a 0c40  ..+....@..~L...@
-00001d90: 2aba 4b4b 7621 0d40 dfc2 34ca f108 0d40  *.KKv!.@..4....@
-00001da0: 0de0 9168 886d 0c40 ad48 1918 18f4 0b40  ...h.m.@.H.....@
-00001db0: 4b47 d6f2 77ba 0b40 cdcc cccc 54d4 0b40  KG..w..@....T..@
-00001dc0: cdcc cccc d4ea 0b40 34d5 c007 883b 0c40  .......@4....;.@
-00001dd0: 83e0 5f44 4eae 0c40 321b 1740 8420 0d40  .._DN..@2..@. .@
-00001de0: 8241 b8da 82ba 0c40 fef2 7bea 6570 0b40  .A.....@..{.ep.@
-00001df0: c76d e1be 524e 0340 d573 df6a 83c7 0940  .m..RN.@.s.j...@
+00001d70: 9b85 42d4 8c06 0c40 c453 7d2f c576 0b40  ..B....@.S}/.v.@
+00001d80: 9b00 2be5 c6b4 0b40 2ffe 7e4c cc9a 0c40  ..+....@/.~L...@
+00001d90: 2aba 4b4b 7621 0d40 e1c2 34ca f108 0d40  *.KKv!.@..4....@
+00001da0: 0de0 9168 886d 0c40 ae48 1918 18f4 0b40  ...h.m.@.H.....@
+00001db0: 4a47 d6f2 77ba 0b40 cdcc cccc 54d4 0b40  JG..w..@....T..@
+00001dc0: cdcc cccc d4ea 0b40 32d5 c007 883b 0c40  .......@2....;.@
+00001dd0: 81e0 5f44 4eae 0c40 321b 1740 8420 0d40  .._DN..@2..@. .@
+00001de0: 7f41 b8da 82ba 0c40 00f3 7bea 6570 0b40  .A.....@..{.ep.@
+00001df0: c76d e1be 524e 0340 d673 df6a 83c7 0940  .m..RN.@.s.j...@
 00001e00: b2b4 c4f8 12fa 0940 0000 0008 c250 0a40  .......@.....P.@
 00001e10: 0000 00d0 eb21 0a40 0000 0028 1bee 0940  .....!.@...(...@
 00001e20: 0000 0050 67bc 0940 0760 4e5c 1f7d 0940  ...Pg..@.`N\.}.@
-00001e30: 69a5 248a 9329 0940 f1b3 a0d9 18af 0740  i.$..).@.......@
+00001e30: 69a5 248a 9329 0940 f0b3 a0d9 18af 0740  i.$..).@.......@
 00001e40: 9034 458d 9c8d 0640 a319 7d0e c0e0 0640  .4E....@..}....@
 00001e50: be34 3c1a c085 0940 f770 8c61 a3de 0940  .4<....@.p.a...@
-00001e60: 5c43 9069 d507 0a40 6655 79fd 2e9a 0a40  \C.i...@fUy....@
-00001e70: 5654 5004 fdee 0a40 da19 20f3 ebf0 0a40  VTP....@.. ....@
+00001e60: 5d43 9069 d507 0a40 6555 79fd 2e9a 0a40  ]C.i...@eUy....@
+00001e70: 5654 5004 fdee 0a40 d919 20f3 ebf0 0a40  VTP....@.. ....@
 00001e80: 0000 00c0 ad17 0b40 0000 0000 c359 0b40  .......@.....Y.@
-00001e90: 0000 0048 69a6 0b40 5544 e38b eae1 0b40  ...Hi..@UD.....@
-00001ea0: 5d0f 7320 0629 0c40 0000 0058 f3b4 0c40  ].s .).@...X...@
+00001e90: 0000 0048 69a6 0b40 5444 e38b eae1 0b40  ...Hi..@TD.....@
+00001ea0: 5c0f 7320 0629 0c40 0000 0058 f3b4 0c40  \.s .).@...X...@
 00001eb0: 23e2 619e b9e9 0b40 2449 5a51 757d fe3f  #.a....@$IZQu}.?
-00001ec0: 78de c856 8d8d f33f a79a dd4a 0c05 0c40  x..V...?...J...@
-00001ed0: b0b9 9ff2 d519 0d40 7175 39dc 8a2a 0d40  .......@qu9..*.@
-00001ee0: 8e62 a565 8c29 0d40 da44 35d2 a17d 0d40  .b.e.).@.D5..}.@
-00001ef0: 0135 8dc3 24c7 0c40 48c8 c10d f76e 0c40  .5..$..@H....n.@
+00001ec0: 76de c856 8d8d f33f a79a dd4a 0c05 0c40  v..V...?...J...@
+00001ed0: b0b9 9ff2 d519 0d40 7075 39dc 8a2a 0d40  .......@pu9..*.@
+00001ee0: 8f62 a565 8c29 0d40 db44 35d2 a17d 0d40  .b.e.).@.D5..}.@
+00001ef0: 0135 8dc3 24c7 0c40 47c8 c10d f76e 0c40  .5..$..@G....n.@
 00001f00: cdcc cccc bcde 0c40 cdcc cccc dc6b 0d40  .......@.....k.@
-00001f10: 517e 92b5 9de4 0e40 721a 8c35 66ba 0f40  Q~.....@r..5f..@
-00001f20: d74d e319 3adf 0f40 07bb d277 c38e 0f40  .M..:..@...w...@
-00001f30: 9b07 38a9 8f58 0e40 102f d6ad 4a74 0040  ..8..X.@./..Jt.@
-00001f40: d6ee a9b8 bad2 f33f 38a2 e45b 6433 0940  .......?8..[d3.@
-00001f50: 0981 5878 6173 0a40 0000 0018 42a2 0a40  ..Xxas.@....B..@
+00001f10: 537e 92b5 9de4 0e40 721a 8c35 66ba 0f40  S~.....@r..5f..@
+00001f20: d74d e319 3adf 0f40 03bb d277 c38e 0f40  .M..:..@...w...@
+00001f30: 9907 38a9 8f58 0e40 0d2f d6ad 4a74 0040  ..8..X.@./..Jt.@
+00001f40: d8ee a9b8 bad2 f33f 38a2 e45b 6433 0940  .......?8..[d3.@
+00001f50: 0781 5878 6173 0a40 0000 0018 42a2 0a40  ..Xxas.@....B..@
 00001f60: 0000 00f0 135b 0a40 0000 00f0 6714 0a40  .....[.@....g..@
 00001f70: 0000 00d0 ccd5 0940 e403 2196 426c 0940  .......@..!.Bl.@
 00001f80: cdcc cccc b4d7 0740 cdcc cccc 8c9f 0740  .......@.......@
 00001f90: a655 47d3 6a98 0940 762b e7c6 d89a 0940  .UG.j..@v+.....@
-00001fa0: 7e27 224b d8e0 0940 dcc6 5680 eb50 0940  ~'"K...@..V..P.@
-00001fb0: 0565 5d23 003a 0c40 f0e5 db94 1650 0d40  .e]#.:.@.....P.@
+00001fa0: 7f27 224b d8e0 0940 dcc6 5680 eb50 0940  .'"K...@..V..P.@
+00001fb0: 0565 5d23 003a 0c40 eee5 db94 1650 0d40  .e]#.:.@.....P.@
 00001fc0: 3333 3333 5b90 0d40 3333 3333 fb0a 0d40  3333[..@3333...@
 00001fd0: 0000 00a0 b685 0b40 0000 0040 fae0 0b40  .......@...@...@
 00001fe0: 0000 0018 4847 0c40 0000 0050 6fb2 0c40  ....HG.@...Po..@
 00001ff0: d894 dac5 32e1 0c40 d58f 9c7b 700f 0c40  ....2..@...{p..@
-00002000: 65bf b221 3b46 0d40 2a3c 0444 101b 1040  e..!;F.@*<.D...@
+00002000: 67bf b221 3b46 0d40 2a3c 0444 101b 1040  g..!;F.@*<.D...@
 00002010: 4775 dfd2 748c 1140 4ccd c063 d979 1040  Gu..t..@L..c.y.@
-00002020: 314d de86 01e4 1040 8e94 c6e1 c0ee 0c40  1M.....@.......@
-00002030: 37ba 5a15 01d3 0c40 83ea d733 769b 0d40  7.Z....@...3v..@
-00002040: 8df3 f5bf 3af9 0c40 6033 1f40 6e4a 0d40  ....:..@`3.@nJ.@
+00002020: 304d de86 01e4 1040 8e94 c6e1 c0ee 0c40  0M.....@.......@
+00002030: 38ba 5a15 01d3 0c40 82ea d733 769b 0d40  8.Z....@...3v..@
+00002040: 8ef3 f5bf 3af9 0c40 6133 1f40 6e4a 0d40  ....:..@a3.@nJ.@
 00002050: 1d3c f0dd a68d 0e40 4991 3e69 22b7 0f40  .<.....@I.>i"..@
-00002060: c35d 58f2 e95d 0f40 5ff0 6c58 6141 1240  .]X..].@_.lXaA.@
-00002070: a243 4159 044d 1340 4243 21ca f48c 1540  .CAY.M.@BC!....@
+00002060: bf5d 58f2 e95d 0f40 5ef0 6c58 6141 1240  .]X..].@^.lXaA.@
+00002070: a343 4159 044d 1340 4343 21ca f48c 1540  .CAY.M.@CC!....@
 00002080: 7453 613f 77ae 1440 7122 e80b 1865 0b40  tSa?w..@q"...e.@
-00002090: 736e bf35 ac5c 0c40 b9ae f574 275d 0a40  sn.5.\.@...t'].@
-000020a0: de4f 2bf0 75aa 0a40 0000 00f0 51c3 0a40  .O+.u..@....Q..@
+00002090: 716e bf35 ac5c 0c40 b9ae f574 275d 0a40  qn.5.\.@...t'].@
+000020a0: df4f 2bf0 75aa 0a40 0000 00f0 51c3 0a40  .O+.u..@....Q..@
 000020b0: 0000 0018 7c67 0a40 0000 0030 7a13 0a40  ....|g.@...0z..@
 000020c0: d3e3 09bf 73b3 0940 9f1b 39da 2667 0940  ....s..@..9.&g.@
 000020d0: d2d1 f2bb 3677 0940 0000 0090 9096 0940  ....6w.@.......@
-000020e0: c63b 1692 7992 0940 6eea 649a d527 0940  .;..y..@n.d..'.@
-000020f0: 9f48 3d27 0f63 0b40 0034 fead b73c 1640  .H='.c.@.4...<.@
-00002100: 2227 a842 eca8 0f40 0351 1c98 3ad4 0e40  "'.B...@.Q..:..@
+000020e0: c63b 1692 7992 0940 6fea 649a d527 0940  .;..y..@o.d..'.@
+000020f0: 9e48 3d27 0f63 0b40 0234 fead b73c 1640  .H='.c.@.4...<.@
+00002100: 2327 a842 eca8 0f40 0351 1c98 3ad4 0e40  #'.B...@.Q..:..@
 00002110: 3333 3333 3bcf 0d40 0000 0018 a892 0b40  3333;..@.......@
 00002120: 0000 0078 a0fb 0b40 0000 0040 cd70 0c40  ...x...@...@.p.@
-00002130: 0000 0068 d8ea 0c40 ab1c dbb7 24df 0c40  ...h...@....$..@
-00002140: d671 b40a 357f 0f40 3146 f0a9 68f1 1140  .q..5..@1F..h..@
+00002130: 0000 0068 d8ea 0c40 a91c dbb7 24df 0c40  ...h...@....$..@
+00002140: d571 b40a 357f 0f40 3046 f0a9 68f1 1140  .q..5..@0F..h..@
 00002150: e0c0 1655 a2de 0140 9259 e6a0 255a 1b40  ...U...@.Y..%Z.@
-00002160: 72e4 9b3b 4bdf 1b40 ca57 b311 22ef 1040  r..;K..@.W.."..@
-00002170: 830d 973a 9666 0f40 7e80 424c e80a fb3f  ...:.f.@~.BL...?
+00002160: 70e4 9b3b 4bdf 1b40 ca57 b311 22ef 1040  p..;K..@.W.."..@
+00002170: 830d 973a 9666 0f40 7c80 424c e80a fb3f  ...:.f.@|.BL...?
 00002180: 59d5 83f9 b908 0e40 cdcc cccc 841f 0d40  Y......@.......@
 00002190: cdcc cccc 7472 0d40 93e0 07a0 bc3b 0f40  ....tr.@.....;.@
 000021a0: 5f7a 0d6e 90a3 0e40 43a7 88cb e1a7 1140  _z.n...@C......@
 000021b0: 2572 a435 61cd 0b40 3333 3333 33c7 1e40  %r.5a..@33333..@
 000021c0: 9a99 9999 9973 2040 a4d8 855a ebd6 1340  .....s @...Z...@
-000021d0: 3861 d00a 5a86 0e40 7e6c 91ca 67c3 0d40  8a..Z..@~l..g..@
-000021e0: 1449 4a0c 98bb 1840 7598 9236 59da 0c40  .IJ....@u..6Y..@
+000021d0: 3861 d00a 5a86 0e40 806c 91ca 67c3 0d40  8a..Z..@.l..g..@
+000021e0: 1249 4a0c 98bb 1840 7698 9236 59da 0c40  .IJ....@v..6Y..@
 000021f0: b85e f133 16f6 0a40 0000 0088 9aae 0a40  .^.3...@.......@
 00002200: 0000 00c8 5246 0a40 c0f3 7d26 18ee 0940  ....RF.@..}&...@
 00002210: 50d2 7a55 be8d 0940 0000 00e8 338e 0940  P.zU...@....3..@
 00002220: 0000 0070 8286 0940 528a dee8 ab68 0940  ...p...@R....h.@
-00002230: a44b 21d2 77fd 0a40 4ca0 791f c358 1440  .K!.w..@L.y..X.@
-00002240: ad84 3dc6 06ca 2140 ca44 3c39 6b54 1940  ..=...!@.D<9kT.@
-00002250: ddc2 9a05 3d41 0f40 3333 3333 23d0 0d40  ....=A.@3333#..@
+00002230: a44b 21d2 77fd 0a40 4aa0 791f c358 1440  .K!.w..@J.y..X.@
+00002240: ad84 3dc6 06ca 2140 c844 3c39 6b54 1940  ..=...!@.D<9kT.@
+00002250: dec2 9a05 3d41 0f40 3333 3333 23d0 0d40  ....=A.@3333#..@
 00002260: 0000 00e8 367e 0b40 0000 00d8 cff2 0b40  ....6~.@.......@
-00002270: 0000 00b8 1075 0c40 0580 ad88 6bf4 0c40  .....u.@....k..@
-00002280: 0a86 61fa e725 0d40 47c9 8892 b07a 1040  ..a..%.@G....z.@
-00002290: c89c 959b 6e28 0b40 ef28 39ca cc3b 2540  ....n(.@.(9..;%@
-000022a0: 9df4 07fb e3c3 2c40 ee1c 23ef ee83 2240  ......,@..#..."@
-000022b0: bec2 fa60 9608 1040 f40d 7ecd 9c69 1040  ...`...@..~..i.@
-000022c0: 8c0e f14a a19f 0c40 9950 b0e9 9833 0e40  ...J...@.P...3.@
+00002270: 0000 00b8 1075 0c40 0680 ad88 6bf4 0c40  .....u.@....k..@
+00002280: 0b86 61fa e725 0d40 48c9 8892 b07a 1040  ..a..%.@H....z.@
+00002290: ca9c 959b 6e28 0b40 ed28 39ca cc3b 2540  ....n(.@.(9..;%@
+000022a0: 9ff4 07fb e3c3 2c40 ef1c 23ef ee83 2240  ......,@..#..."@
+000022b0: bcc2 fa60 9608 1040 f30d 7ecd 9c69 1040  ...`...@..~..i.@
+000022c0: 8e0e f14a a19f 0c40 9b50 b0e9 9833 0e40  ...J...@.P...3.@
 000022d0: cdcc cccc bc87 0c40 1bea fd8c 2699 0c40  .......@....&..@
-000022e0: 1739 dc5b f3bf 0e40 1441 c002 14ee 0240  .9.[...@.A.....@
+000022e0: 1739 dc5b f3bf 0e40 1641 c002 14ee 0240  .9.[...@.A.....@
 000022f0: 1646 44d2 f3d2 1240 3333 3333 33f7 1c40  .FD....@33333..@
 00002300: 0fb8 9f3e 608a 2940 ee39 de9f ec96 3240  ...>`.)@.9....2@
-00002310: 511c d28f 8045 2440 34f7 d380 f21f 1b40  Q....E$@4......@
+00002310: 501c d28f 8045 2440 34f7 d380 f21f 1b40  P....E$@4......@
 00002320: 348a ef53 34a6 1c40 ee8a 4a50 c58d 1b40  4..S4..@..JP...@
-00002330: b1ea e70f bb31 0f40 3333 3333 137f 0d40  .....1.@3333...@
+00002330: b2ea e70f bb31 0f40 3333 3333 137f 0d40  .....1.@3333...@
 00002340: 0000 0038 6ae5 0a40 0000 0090 716b 0a40  ...8j..@....qk.@
 00002350: 0000 0000 c001 0a40 b164 e86b 6c94 0940  .......@.d.kl..@
 00002360: aae4 6c7e ab80 0940 0000 00d8 096c 0940  ..l~...@.....l.@
 00002370: 2ded e072 1b39 0940 74dc 9200 c1f4 0a40  -..r.9.@t......@
-00002380: 1804 c1bf a050 0b40 f4a7 540b dbde 1640  .....P.@..T....@
-00002390: 3036 b843 4715 1940 883f 5e4e c650 0d40  06.CG..@.?^N.P.@
+00002380: 1704 c1bf a050 0b40 f6a7 540b dbde 1640  .....P.@..T....@
+00002390: 3036 b843 4715 1940 873f 5e4e c650 0d40  06.CG..@.?^N.P.@
 000023a0: 3333 3333 7bd7 0c40 0000 0098 3f49 0b40  3333{..@....?I.@
 000023b0: 0000 0028 8bc6 0b40 0000 0010 2c53 0c40  ...(...@....,S.@
-000023c0: 0b72 7c93 f6d1 0c40 5699 6590 3df9 0c40  .r|....@V.e.=..@
-000023d0: ccd3 8ef5 575e 1040 0894 f3fa 3413 1040  ....W^.@....4..@
+000023c0: 0b72 7c93 f6d1 0c40 5399 6590 3df9 0c40  .r|....@S.e.=..@
+000023d0: ccd3 8ef5 575e 1040 0a94 f3fa 3413 1040  ....W^.@....4..@
 000023e0: 8596 250a 655e 2040 68a7 4d02 3312 2d40  ..%.e^ @h.M.3.-@
 000023f0: ba3e 45cd 9672 2140 e89b 2190 be80 1040  .>E..r!@..!....@
 00002400: 50e3 5f56 92a6 1040 d821 fbc9 f983 0d40  P._V...@.!.....@
-00002410: 98aa 259e f895 0c40 6fdc c425 dd9c 0b40  ..%....@o..%...@
-00002420: bee0 0460 fc02 0b40 a326 1236 462e 0b40  ...`...@.&.6F..@
-00002430: 3a6b 1ef8 4295 f73f e6d1 dbbf f67f 1040  :k..B..?.......@
+00002410: 97aa 259e f895 0c40 6edc c425 dd9c 0b40  ..%....@n..%...@
+00002420: bde0 0460 fc02 0b40 a526 1236 462e 0b40  ...`...@.&.6F..@
+00002430: 386b 1ef8 4295 f73f e8d1 dbbf f67f 1040  8k..B..?.......@
 00002440: 3333 3333 33c7 1d40 cd7f 710b 6589 3140  33333..@..q.e.1@
 00002450: 27f2 c16b 810b 2940 cdbd 4bc8 b7a4 2440  '..k..)@..K...$@
-00002460: f8ab dd25 df8c 1b40 5cc1 7a55 9704 1340  ...%...@\.zU...@
-00002470: e663 11da 2e7e 1140 4a9b dbd8 a20c 1040  .c...~.@J......@
+00002460: f6ab dd25 df8c 1b40 5cc1 7a55 9704 1340  ...%...@\.zU...@
+00002470: e663 11da 2e7e 1140 4b9b dbd8 a20c 1040  .c...~.@K......@
 00002480: 3333 3333 6bc6 0d40 0000 0020 b609 0b40  3333k..@... ...@
 00002490: 0000 0070 0f82 0a40 c003 ca84 c709 0a40  ...p...@.......@
 000024a0: 43b8 2c5f ec7a 0940 f00a 7341 b146 0940  C.,_.z.@..sA.F.@
-000024b0: 0000 0020 624c 0940 eb6b 685a 9020 0940  ... bL.@.khZ. .@
+000024b0: 0000 0020 624c 0940 e96b 685a 9020 0940  ... bL.@.khZ. .@
 000024c0: 9654 07e1 961e 0940 4369 3ac1 227f 0a40  .T.....@Ci:."..@
-000024d0: dd4a 3483 7176 0a40 87d3 79b5 14e5 0a40  .J4.qv.@..y....@
-000024e0: 6eae dd77 4827 0b40 0000 0030 9a8e 0a40  n..wH'.@...0...@
+000024d0: de4a 3483 7176 0a40 87d3 79b5 14e5 0a40  .J4.qv.@..y....@
+000024e0: 6dae dd77 4827 0b40 0000 0030 9a8e 0a40  m..wH'.@...0...@
 000024f0: 0000 0038 75fc 0a40 c484 dcaa 643b 0b40  ...8u..@....d;.@
-00002500: 407e 3af2 45ba 0b40 4b10 3a0e 3b9d 0c40  @~:.E..@K.:.;..@
-00002510: a80c 5de5 425b 0c40 10ec df28 d408 0f40  ..].B[.@...(...@
-00002520: 2252 3731 0d3b 1040 3333 3333 33ab 1940  "R71.;.@33333..@
-00002530: f75f 3232 78e4 2040 fa80 6c10 1db7 1b40  ._22x. @..l....@
-00002540: fbce 8acc b2ee 1040 24e1 7fdc ee03 1040  .......@$......@
+00002500: 3f7e 3af2 45ba 0b40 4a10 3a0e 3b9d 0c40  ?~:.E..@J.:.;..@
+00002510: a80c 5de5 425b 0c40 11ec df28 d408 0f40  ..].B[.@...(...@
+00002520: 2352 3731 0d3b 1040 3333 3333 33ab 1940  #R71.;.@33333..@
+00002530: f75f 3232 78e4 2040 fc80 6c10 1db7 1b40  ._22x. @..l....@
+00002540: fbce 8acc b2ee 1040 22e1 7fdc ee03 1040  .......@"......@
 00002550: 9d8c d6ad ccfc 0d40 a51b f633 2d99 0b40  .......@...3-..@
-00002560: 8992 f46f a955 0a40 82c0 bcbd 36d5 0940  ...o.U.@....6..@
-00002570: 6448 179b f3c1 0940 90be 1160 dca0 0340  dH.....@...`...@
-00002580: 7fac d70d 8896 0f40 b5dc 0a4e 5219 0540  .......@...NR..@
-00002590: 1038 8e45 3b03 2140 9a99 9999 9995 2040  .8.E;.!@...... @
+00002560: 8892 f46f a955 0a40 82c0 bcbd 36d5 0940  ...o.U.@....6..@
+00002570: 6448 179b f3c1 0940 91be 1160 dca0 0340  dH.....@...`...@
+00002580: 7fac d70d 8896 0f40 b3dc 0a4e 5219 0540  .......@...NR..@
+00002590: 0f38 8e45 3b03 2140 9a99 9999 9995 2040  .8.E;.!@...... @
 000025a0: a6e6 bcf9 5609 1740 325f e2c8 6571 1240  ....V..@2_..eq.@
 000025b0: dcf8 9e69 7bb3 1140 ebae 278e 6cba 1040  ...i{..@..'.l..@
 000025c0: 3333 3333 7b8f 0f40 1d45 3c75 25d2 0b40  3333{..@.E<u%..@
 000025d0: 0000 0028 f21a 0b40 0000 0098 818a 0a40  ...(...@.......@
-000025e0: 7787 5f02 59e9 0940 f90c 28b9 c246 0940  w._.Y..@..(..F.@
+000025e0: 7887 5f02 59e9 0940 f90c 28b9 c246 0940  x._.Y..@..(..F.@
 000025f0: 87aa 64bb 8eef 0840 f3b6 123a 58e3 0840  ..d....@...:X..@
 00002600: 0000 0018 4119 0940 6683 4ab4 c4f3 0840  ....A..@f.J....@
 00002610: 839b 9920 ed0d 0940 b5f2 2e43 e84d 0940  ... ...@...C.M.@
 00002620: c467 1552 a180 0940 0000 0068 09e0 0940  .g.R...@...h...@
 00002630: 0000 0038 8137 0a40 d109 c861 941f 0a40  ...8.7.@...a...@
 00002640: cdcc cccc 2448 0940 cdcc cccc 8c7f 0940  ....$H.@.......@
-00002650: 0151 09db 1d51 0a40 c2a0 e6ec 832f 0c40  .Q...Q.@...../.@
-00002660: a999 1b4e fea6 0c40 722e 5c40 8d57 1040  ...N...@r.\@.W.@
-00002670: 0816 9a19 3597 1040 82da 2a3f ee81 1040  ....5..@..*?...@
-00002680: 8886 f8f7 9cf1 1040 4c4a f695 5ce7 1040  .......@LJ..\..@
+00002650: 0151 09db 1d51 0a40 c0a0 e6ec 832f 0c40  .Q...Q.@...../.@
+00002660: a799 1b4e fea6 0c40 722e 5c40 8d57 1040  ...N...@r.\@.W.@
+00002670: 0616 9a19 3597 1040 80da 2a3f ee81 1040  ....5..@..*?...@
+00002680: 8886 f8f7 9cf1 1040 4b4a f695 5ce7 1040  .......@KJ..\..@
 00002690: dc87 d81f 91ab 0d40 5f62 7a53 37eb 0d40  .......@_bzS7..@
-000026a0: ee23 ed8d 6e4d 0a40 92d1 6091 1f35 0940  .#..nM.@..`..5.@
-000026b0: e06d f32f b42a 0940 5c4b 26a6 29fd 0940  .m./.*.@\K&.)..@
-000026c0: 1260 c594 a107 0c40 99c6 58a4 ca69 0f40  .`.....@..X..i.@
-000026d0: 25d0 ab09 d788 1140 8e52 04a5 ebb6 1240  %......@.R.....@
-000026e0: 4be9 ab91 3a19 1640 7ed7 38ff f833 1740  K...:..@~.8..3.@
+000026a0: ec23 ed8d 6e4d 0a40 92d1 6091 1f35 0940  .#..nM.@..`..5.@
+000026b0: df6d f32f b42a 0940 5d4b 26a6 29fd 0940  .m./.*.@]K&.)..@
+000026c0: 1460 c594 a107 0c40 97c6 58a4 ca69 0f40  .`.....@..X..i.@
+000026d0: 25d0 ab09 d788 1140 8c52 04a5 ebb6 1240  %......@.R.....@
+000026e0: 48e9 ab91 3a19 1640 7ed7 38ff f833 1740  H...:..@~.8..3.@
 000026f0: 9a99 9999 8dde 1040 9a99 9999 718f 1040  .......@....q..@
 00002700: 9999 9999 7104 1040 3333 3333 3b79 0e40  ....q..@3333;y.@
 00002710: 0000 0090 7db5 0b40 0000 0000 a91c 0b40  ....}..@.......@
 00002720: 0000 00b8 6288 0a40 0c9c 78a1 13b5 0940  ....b..@..x....@
 00002730: ace3 09c4 1105 0940 cdcc cccc dc6c 0740  .......@.....l.@
 00002740: cdcc cccc 9c38 0740 cdcc cccc e456 0740  .....8.@.....V.@
 00002750: fbae f286 c576 0840 d92f e0af c8a0 0840  .....v.@./.....@
-00002760: dcc1 38c2 50d0 0840 e5b3 c060 8d03 0940  ..8.P..@...`...@
-00002770: 6c57 3ea3 3d00 0940 3460 e9b0 5beb 0840  lW>.=..@4`..[..@
-00002780: cdcc cccc 04df 0740 9e33 a6a4 e083 0740  .......@.3.....@
-00002790: 1ab4 2e31 c595 0740 778d 2c2a f95e 0840  ...1...@w.,*.^.@
-000027a0: 84ee 45d2 60fb 0940 ed59 6205 ba5a 0c40  ..E.`..@.Yb..Z.@
+00002760: dbc1 38c2 50d0 0840 e5b3 c060 8d03 0940  ..8.P..@...`...@
+00002770: 6b57 3ea3 3d00 0940 3360 e9b0 5beb 0840  kW>.=..@3`..[..@
+00002780: cdcc cccc 04df 0740 9c33 a6a4 e083 0740  .......@.3.....@
+00002790: 1ab4 2e31 c595 0740 768d 2c2a f95e 0840  ...1...@v.,*.^.@
+000027a0: 85ee 45d2 60fb 0940 ec59 6205 ba5a 0c40  ..E.`..@.Yb..Z.@
 000027b0: 0289 c186 7ae6 0c40 5b61 fcc4 d863 0f40  ....z..@[a...c.@
 000027c0: e003 09ef b24e 1040 87ce f110 c3e7 0f40  .....N.@.......@
-000027d0: 96b9 38da b4b6 0d40 f9b8 0596 fbd3 0d40  ..8....@.......@
-000027e0: 776c 86d9 2ec5 0a40 2fec 6d7c ab1b 0940  wl.....@/.m|...@
-000027f0: a0f0 6130 9d7f 0840 3829 142b beeb 0840  ..a0...@8).+...@
-00002800: 136b 39cf 263e 0a40 9c09 5248 823c 0c40  .k9.&>.@..RH.<.@
-00002810: 7875 831f d2b1 0e40 dbf4 48a0 780e 1140  xu.....@..H.x..@
-00002820: 4dae b213 2568 1140 1bad 1ba2 bba7 1140  M...%h.@.......@
-00002830: 8233 3c27 2ee0 1140 3333 3333 a3b3 0f40  .3<'...@3333...@
+000027d0: 94b9 38da b4b6 0d40 f8b8 0596 fbd3 0d40  ..8....@.......@
+000027e0: 786c 86d9 2ec5 0a40 2fec 6d7c ab1b 0940  xl.....@/.m|...@
+000027f0: a2f0 6130 9d7f 0840 3729 142b beeb 0840  ..a0...@7).+...@
+00002800: 136b 39cf 263e 0a40 9b09 5248 823c 0c40  .k9.&>.@..RH.<.@
+00002810: 7875 831f d2b1 0e40 daf4 48a0 780e 1140  xu.....@..H.x..@
+00002820: 4dae b213 2568 1140 1cad 1ba2 bba7 1140  M...%h.@.......@
+00002830: 8433 3c27 2ee0 1140 3333 3333 a3b3 0f40  .3<'...@3333...@
 00002840: 3333 3333 133b 0f40 e1dd bfe0 5237 0d40  3333.;.@....R7.@
 00002850: 0000 0000 4d3d 0c40 0000 0028 0aad 0b40  ....M=.@...(...@
-00002860: 0000 00c0 0015 0b40 6735 dbd6 b65d 0a40  .......@g5...].@
+00002860: 0000 00c0 0015 0b40 6635 dbd6 b65d 0a40  .......@f5...].@
 00002870: 5c19 9b47 417d 0940 cdcc cccc 7cb8 0740  \..GA}.@....|..@
-00002880: cdcc cccc 7c19 0740 3e20 eb39 589f 0640  ....|..@> .9X..@
-00002890: 75eb ce3c 1241 0640 cef7 5e94 e51e 0640  u..<.A.@..^....@
+00002880: cdcc cccc 7c19 0740 3c20 eb39 589f 0640  ....|..@< .9X..@
+00002890: 74eb ce3c 1241 0640 cef7 5e94 e51e 0640  t..<.A.@..^....@
 000028a0: 3980 3cdd 6531 0640 6cd1 19a3 a579 0640  9.<.e1.@l....y.@
 000028b0: cdcc cccc eccf 0640 cdcc cccc dcda 0640  .......@.......@
 000028c0: cdcc cccc 3cc1 0640 35c5 5e68 dc60 0640  ....<..@5.^h.`.@
-000028d0: ad08 97cf a305 0640 31b8 3174 7a25 0640  .......@1.1tz%.@
-000028e0: ab26 8156 e9f1 0640 eb0e 2b34 068b 0840  .&.V...@..+4...@
-000028f0: 7521 2785 9b92 0a40 83ad ab87 393b 0d40  u!'....@....9;.@
-00002900: dea8 7e18 fea7 0d40 bb97 d7c1 3cef 0d40  ..~....@....<..@
-00002910: 39a6 4180 351f 0e40 15fb 77d2 6de3 0d40  9.A.5..@..w.m..@
-00002920: c414 3cd8 ede3 0a40 6713 5083 be44 0940  ..<....@g.P..D.@
-00002930: f2ee 2b5b d358 0840 768c 2b7d 4553 0840  ..+[.X.@v.+}ES.@
-00002940: 5f83 bf56 5005 0940 8204 f285 b849 0a40  _..VP..@.....I.@
-00002950: ff6d bd69 9ae3 0b40 9095 8f27 a4a5 0d40  .m.i...@...'...@
-00002960: 9658 775c 4a5b 0f40 7545 7cca 7d5f 1040  .Xw\J[.@uE|.}_.@
-00002970: 0f27 6e68 24e6 1040 a8b7 9d7b b534 1140  .'nh$..@...{.4.@
+000028d0: ad08 97cf a305 0640 2fb8 3174 7a25 0640  .......@/.1tz%.@
+000028e0: ac26 8156 e9f1 0640 ea0e 2b34 068b 0840  .&.V...@..+4...@
+000028f0: 7521 2785 9b92 0a40 81ad ab87 393b 0d40  u!'....@....9;.@
+00002900: e0a8 7e18 fea7 0d40 bb97 d7c1 3cef 0d40  ..~....@....<..@
+00002910: 38a6 4180 351f 0e40 17fb 77d2 6de3 0d40  8.A.5..@..w.m..@
+00002920: c214 3cd8 ede3 0a40 6713 5083 be44 0940  ..<....@g.P..D.@
+00002930: f2ee 2b5b d358 0840 758c 2b7d 4553 0840  ..+[.X.@u.+}ES.@
+00002940: 5e83 bf56 5005 0940 8204 f285 b849 0a40  ^..VP..@.....I.@
+00002950: fd6d bd69 9ae3 0b40 8d95 8f27 a4a5 0d40  .m.i...@...'...@
+00002960: 9858 775c 4a5b 0f40 7645 7cca 7d5f 1040  .Xw\J[.@vE|.}_.@
+00002970: 1027 6e68 24e6 1040 a9b7 9d7b b534 1140  .'nh$..@...{.4.@
 00002980: f15d 6f3e e475 0d40 423c c15e 6913 0d40  .]o>.u.@B<.^i..@
 00002990: 0000 00d8 0ea3 0c40 0000 0030 652b 0c40  .......@...0e+.@
 000029a0: 0000 00c8 d59e 0b40 0000 0030 a10b 0b40  .......@...0...@
-000029b0: fdc5 7b48 7a22 0a40 2c75 3dcf 5752 0940  ..{Hz".@,u=.WR.@
+000029b0: fec5 7b48 7a22 0a40 2c75 3dcf 5752 0940  ..{Hz".@,u=.WR.@
 000029c0: cdcc cccc 24a1 0740 cdcc cccc 2c14 0740  ....$..@....,..@
-000029d0: 381f 119e 8477 0640 d87e 71b3 4bc2 0540  8....w.@.~q.K..@
-000029e0: 08cd 93a5 152e 0540 dc42 cd47 9be4 0440  .......@.B.G...@
-000029f0: c0ec 272e 1502 0540 d8f6 4337 095e 0540  ..'....@..C7.^.@
-00002a00: 306f 5ffb 8ea6 0540 04f5 2c37 86b6 0540  0o_....@..,7...@
-00002a10: c786 dc98 de83 0540 4e6c 78a3 3152 0540  .......@Nlx.1R.@
-00002a20: e118 1d83 bd81 0540 3592 dd3e 364c 0640  .......@5..>6L.@
-00002a30: 94e4 8358 fed1 0740 50b6 1290 5cc2 0940  ...X...@P...\..@
-00002a40: 9738 c318 a5a3 0b40 7f64 bdec 9e6f 0d40  .8.....@.d...o.@
+000029d0: 371f 119e 8477 0640 d87e 71b3 4bc2 0540  7....w.@.~q.K..@
+000029e0: 08cd 93a5 152e 0540 db42 cd47 9be4 0440  .......@.B.G...@
+000029f0: bfec 272e 1502 0540 d7f6 4337 095e 0540  ..'....@..C7.^.@
+00002a00: 2f6f 5ffb 8ea6 0540 02f5 2c37 86b6 0540  /o_....@..,7...@
+00002a10: c686 dc98 de83 0540 4e6c 78a3 3152 0540  .......@Nlx.1R.@
+00002a20: e118 1d83 bd81 0540 3492 dd3e 364c 0640  .......@4..>6L.@
+00002a30: 93e4 8358 fed1 0740 4fb6 1290 5cc2 0940  ...X...@O...\..@
+00002a40: 9938 c318 a5a3 0b40 7f64 bdec 9e6f 0d40  .8.....@.d...o.@
 00002a50: 3ae3 8340 68c3 0d40 891e 9507 f356 0c40  :..@h..@.....V.@
-00002a60: 0988 f273 3efc 0a40 22cd fb88 db98 0940  ...s>..@"......@
-00002a70: 2738 1da5 6ca3 0840 5a04 f2c1 7c62 0840  '8..l..@Z...|b.@
-00002a80: aafc ea1b 94c1 0840 9953 5a12 757c 0940  .......@.SZ.u|.@
+00002a60: 0888 f273 3efc 0a40 20cd fb88 db98 0940  ...s>..@ ......@
+00002a70: 2638 1da5 6ca3 0840 5a04 f2c1 7c62 0840  &8..l..@Z...|b.@
+00002a80: a9fc ea1b 94c1 0840 9953 5a12 757c 0940  .......@.SZ.u|.@
 00002a90: 59aa da12 e774 0a40 7dba 276f 7f7d 0b40  Y....t.@}.'o.}.@
-00002aa0: 5c88 2b7a 3c8c 0c40 4e41 0449 5d97 0d40  \.+z<..@NA.I]..@
+00002aa0: 5e88 2b7a 3c8c 0c40 4e41 0449 5d97 0d40  ^.+z<..@NA.I]..@
 00002ab0: 5280 3baf 2fa2 0e40 c6eb 1428 57be 0f40  R.;./..@...(W..@
 00002ac0: 48ae b7fe 9f41 1040 0000 00f0 520a 0d40  H....A.@....R..@
 00002ad0: 0000 0068 58dc 0c40 0000 00a0 2c88 0c40  ...hX..@....,..@
 00002ae0: 0000 00a8 6415 0c40 0000 0070 8f8f 0b40  ....d..@...p...@
-00002af0: df7a 89a7 d7ce 0a40 af85 c36f a9f9 0940  .z.....@...o...@
+00002af0: de7a 89a7 d7ce 0a40 af85 c36f a9f9 0940  .z.....@...o...@
 00002b00: cdcc cccc b422 0840 cdcc cccc dcc0 0740  .....".@.......@
 00002b10: cdcc cccc 846d 0740 cdcc cccc fcf5 0640  .....m.@.......@
 00002b20: 0ef1 f3cf 3147 0640 d2f2 d272 be4f 0540  ....1G.@...r.O.@
-00002b30: d893 f321 1b8f 0440 93ff 66ef 7073 0440  ...!...@..f.ps.@
-00002b40: 63a3 b6fa cde2 0440 537a b45d 9852 0540  c......@Sz.].R.@
+00002b30: d893 f321 1b8f 0440 94ff 66ef 7073 0440  ...!...@..f.ps.@
+00002b40: 63a3 b6fa cde2 0440 547a b45d 9852 0540  c......@Tz.].R.@
 00002b50: 5e9c b6c1 147f 0540 8b97 a4e0 7365 0540  ^......@....se.@
-00002b60: c274 d99c e946 0540 723b 5db0 1686 0540  .t...F.@r;]....@
-00002b70: d9f6 42b1 fd62 0640 f35e a1a2 4af4 0740  ..B..b.@.^..J..@
+00002b60: c174 d99c e946 0540 723b 5db0 1686 0540  .t...F.@r;]....@
+00002b70: d9f6 42b1 fd62 0640 f25e a1a2 4af4 0740  ..B..b.@.^..J..@
 00002b80: 56f0 6c8d a9e6 0940 cdcc cccc 7c74 0b40  V.l....@....|t.@
 00002b90: cdcc cccc 7c54 0c40 cdcc cccc 4470 0c40  ....|T.@....Dp.@
-00002ba0: eeea b210 2561 0b40 4e77 b4ad 7034 0a40  ....%a.@Nw..p4.@
-00002bb0: ab0d 95bb 9272 0940 9d7e fb03 5f1a 0940  .....r.@.~.._..@
-00002bc0: 78d0 449a 0934 0940 4ce4 17e2 1ea4 0940  x.D..4.@L......@
-00002bd0: f017 e954 6436 0a40 cdcc cccc f4da 0a40  ...Td6.@.......@
-00002be0: f424 2208 6b72 0b40 eb0b d045 e7e7 0b40  .$".kr.@...E...@
-00002bf0: 2c3f a091 6f54 0c40 81ef a5ba 0753 0d40  ,?..oT.@.....S.@
-00002c00: 30c4 9201 a72f 0f40 9be5 9aaf 505c 1040  0..../.@....P\.@
+00002ba0: eeea b210 2561 0b40 4d77 b4ad 7034 0a40  ....%a.@Mw..p4.@
+00002bb0: ac0d 95bb 9272 0940 9c7e fb03 5f1a 0940  .....r.@.~.._..@
+00002bc0: 78d0 449a 0934 0940 4be4 17e2 1ea4 0940  x.D..4.@K......@
+00002bd0: ef17 e954 6436 0a40 cdcc cccc f4da 0a40  ...Td6.@.......@
+00002be0: f424 2208 6b72 0b40 ec0b d045 e7e7 0b40  .$".kr.@...E...@
+00002bf0: 2d3f a091 6f54 0c40 84ef a5ba 0753 0d40  -?..oT.@.....S.@
+00002c00: 30c4 9201 a72f 0f40 9ce5 9aaf 505c 1040  0..../.@....P\.@
 00002c10: 0000 00f0 96ec 0c40 0000 00a0 acc0 0c40  .......@.......@
 00002c20: 0000 0060 8870 0c40 0000 00d0 b903 0c40  ...`.p.@.......@
 00002c30: 8bba 2b9e 3180 0b40 cdcc cccc 0c3a 0940  ..+.1..@.....:.@
 00002c40: cdcc cccc fc68 0840 cdcc cccc 4c09 0840  .....h.@....L..@
 00002c50: cdcc cccc 14fe 0740 cdcc cccc 7cfe 0740  .......@....|..@
 00002c60: cdcc cccc 44cc 0740 cdcc cccc b45c 0740  ....D..@.....\.@
-00002c70: 3a02 2a31 8c3e 0640 1b2a edb7 eddc 0440  :.*1.>.@.*.....@
-00002c80: e17a f91e 118b 0440 ddce 5f94 b445 0540  .z.....@.._..E.@
-00002c90: 1f36 6990 a2ea 0540 9a77 c799 7001 0640  .6i....@.w..p..@
-00002ca0: 36da ee63 d4c2 0540 e56f 6058 bb95 0540  6..c...@.o`X...@
-00002cb0: 3fcd d600 a9e3 0540 eb47 fd64 08f1 0640  ?......@.G.d...@
-00002cc0: 6ea0 6b66 63c9 0840 cdcc cccc 6cea 0a40  n.kfc..@....l..@
+00002c70: 3a02 2a31 8c3e 0640 1d2a edb7 eddc 0440  :.*1.>.@.*.....@
+00002c80: e27a f91e 118b 0440 ddce 5f94 b445 0540  .z.....@.._..E.@
+00002c90: 1e36 6990 a2ea 0540 9977 c799 7001 0640  .6i....@.w..p..@
+00002ca0: 35da ee63 d4c2 0540 e56f 6058 bb95 0540  5..c...@.o`X...@
+00002cb0: 3ecd d600 a9e3 0540 eb47 fd64 08f1 0640  >......@.G.d...@
+00002cc0: 6ca0 6b66 63c9 0840 cdcc cccc 6cea 0a40  l.kfc..@....l..@
 00002cd0: cdcc cccc 8c96 0c40 2ca2 8ae3 b21a 0e40  .......@,......@
-00002ce0: 0de0 8d0a 7890 0e40 66f3 f1f6 b64b 0b40  ....x..@f....K.@
-00002cf0: ade7 1d5a 3134 0a40 b3e4 f2e4 8655 0a40  ...Z14.@.....U.@
-00002d00: 2351 b313 b483 0a40 71a4 05a1 4f92 0a40  #Q.....@q...O..@
+00002ce0: 0fe0 8d0a 7890 0e40 65f3 f1f6 b64b 0b40  ....x..@e....K.@
+00002cf0: abe7 1d5a 3134 0a40 b2e4 f2e4 8655 0a40  ...Z14.@.....U.@
+00002d00: 2151 b313 b483 0a40 71a4 05a1 4f92 0a40  !Q.....@q...O..@
 00002d10: cdcc cccc 4ca0 0a40 cdcc cccc 64b9 0a40  ....L..@....d..@
 00002d20: ae55 8916 9e11 0b40 0606 9c4e e431 0b40  .U.....@...N.1.@
-00002d30: d10e 94e2 9a59 0b40 d368 6f1e ecd6 0b40  .....Y.@.ho....@
-00002d40: bdfd 1a40 83f2 0240 0109 3a9f 4d78 1040  ...@...@..:.Mx.@
-00002d50: 4305 87db 61cb 1140 0000 0098 d0d8 0c40  C...a..@.......@
+00002d30: d00e 94e2 9a59 0b40 d268 6f1e ecd6 0b40  .....Y.@.ho....@
+00002d40: befd 1a40 83f2 0240 ff08 3a9f 4d78 1040  ...@...@..:.Mx.@
+00002d50: 4405 87db 61cb 1140 0000 0098 d0d8 0c40  D...a..@.......@
 00002d60: 0000 00f8 f4ae 0c40 0000 00f0 dd62 0c40  .......@.....b.@
 00002d70: 0000 0088 2cfc 0b40 cf9d 11fa ac78 0b40  ....,..@.....x.@
 00002d80: cdcc cccc 14f1 0840 cdcc cccc ac3f 0840  .......@.....?.@
 00002d90: cdcc cccc 8419 0840 cdcc cccc 245b 0840  .......@....$[.@
 00002da0: d161 86c3 aafe 0840 6c96 086f cf05 0940  .a.....@l..o...@
-00002db0: 701a 03ce f027 0940 2a90 0a17 ec55 0940  p....'.@*....U.@
-00002dc0: 6ac0 3092 41e0 fa3f e0c3 b902 b243 f73f  j.0.A..?.....C.?
-00002dd0: 403c 3c51 661a 0740 bc68 5422 c516 0740  @<<Qf..@.hT"...@
-00002de0: 2581 4aa2 6e92 0640 bfd4 e6a8 53f2 0540  %.J.n..@....S..@
-00002df0: 3551 cf8d 10cd 0540 ae2b 2462 d052 0640  5Q.....@.+$b.R.@
-00002e00: c484 f6c4 0db4 0740 8724 4d8d f604 0a40  .......@.$M....@
-00002e10: 6d85 e0c1 cafb 0c40 5214 6016 3ca3 0e40  m......@R.`.<..@
-00002e20: 9c21 ca8c e380 0e40 9415 5735 68f6 0c40  .!.....@..W5h..@
-00002e30: 38f3 4ae0 f671 fe3f 5509 4333 4c21 0540  8.J..q.?U.C3L!.@
-00002e40: b03b 4037 d6c3 0c40 40fc 8f02 cdc2 0c40  .;@7...@@......@
+00002db0: 6f1a 03ce f027 0940 2a90 0a17 ec55 0940  o....'.@*....U.@
+00002dc0: 68c0 3092 41e0 fa3f dec3 b902 b243 f73f  h.0.A..?.....C.?
+00002dd0: 413c 3c51 661a 0740 bb68 5422 c516 0740  A<<Qf..@.hT"...@
+00002de0: 2481 4aa2 6e92 0640 bed4 e6a8 53f2 0540  $.J.n..@....S..@
+00002df0: 3351 cf8d 10cd 0540 ae2b 2462 d052 0640  3Q.....@.+$b.R.@
+00002e00: c484 f6c4 0db4 0740 8524 4d8d f604 0a40  .......@.$M....@
+00002e10: 7185 e0c1 cafb 0c40 5114 6016 3ca3 0e40  q......@Q.`.<..@
+00002e20: 9b21 ca8c e380 0e40 9415 5735 68f6 0c40  .!.....@..W5h..@
+00002e30: 36f3 4ae0 f671 fe3f 5709 4333 4c21 0540  6.J..q.?W.C3L!.@
+00002e40: af3b 4037 d6c3 0c40 3efc 8f02 cdc2 0c40  .;@7...@>......@
 00002e50: cdcc cccc ac0e 0c40 cdcc cccc b476 0b40  .......@.....v.@
-00002e60: cdcc cccc 643e 0b40 4f87 2101 7dbb 0a40  ....d>.@O.!.}..@
-00002e70: 64dc ef74 7c5e 0a40 e10b 1512 1b2b 0b40  d..t|^.@.....+.@
-00002e80: 54df 81a9 3cb5 0640 b97a 75c5 ef3f 0b40  T...<..@.zu..?.@
+00002e60: cdcc cccc 643e 0b40 4e87 2101 7dbb 0a40  ....d>.@N.!.}..@
+00002e70: 67dc ef74 7c5e 0a40 e10b 1512 1b2b 0b40  g..t|^.@.....+.@
+00002e80: 54df 81a9 3cb5 0640 b77a 75c5 ef3f 0b40  T...<..@.zu..?.@
 00002e90: 509b c470 9131 1240 8efe 1da8 9e9e 1440  P..p.1.@.......@
 00002ea0: 0000 0078 6cd1 0c40 0000 0000 5ba9 0c40  ...xl..@....[..@
 00002eb0: 0000 00f8 d560 0c40 0000 0088 a8ff 0b40  .....`.@.......@
 00002ec0: 0000 0040 7993 0b40 cdcc cccc 6cf6 0840  ...@y..@....l..@
-00002ed0: b8ab 6da2 382e 0840 cf88 4f7b 1d2f 0840  ..m.8..@..O{./.@
+00002ed0: b8ab 6da2 382e 0840 cd88 4f7b 1d2f 0840  ..m.8..@..O{./.@
 00002ee0: cdcc cccc b4a8 0840 1f1b fdc0 efb4 0940  .......@.......@
 00002ef0: f80f c496 5921 0a40 6822 45ec 7b9a 0a40  ....Y!.@h"E.{..@
-00002f00: 39df bd42 2bcc 0940 e667 6f82 c003 0940  9..B+..@.go....@
-00002f10: a382 e86a b906 0940 b5a9 35fe 748a 0940  ...j...@..5.t..@
-00002f20: f1fd 4098 d3d0 0940 cfa9 523e 2d9c 0740  ..@....@..R>-..@
-00002f30: f1e8 52de cee3 0540 de99 534a 66d5 0540  ..R....@..SJf..@
-00002f40: da67 2855 e5c8 0640 5e0c 29dc a27b 0840  .g(U...@^.)..{.@
-00002f50: 207a 73a7 263a 0b40 3b72 12d0 0273 0e40   zs.&:.@;r...s.@
-00002f60: cf32 aa60 ac0e 0f40 57d7 01f5 bfea 1040  .2.`...@W......@
-00002f70: 303d 216b 8d89 1040 c58e ab47 b613 0f40  0=!k...@...G...@
-00002f80: ad80 9a3a c3f7 0d40 0819 0d75 4026 1040  ...:...@...u@&.@
-00002f90: ed3a 3469 7334 0f40 cdcc cccc bc94 0d40  .:4is4.@.......@
+00002f00: 3adf bd42 2bcc 0940 e367 6f82 c003 0940  :..B+..@.go....@
+00002f10: a482 e86a b906 0940 b4a9 35fe 748a 0940  ...j...@..5.t..@
+00002f20: effd 4098 d3d0 0940 cea9 523e 2d9c 0740  ..@....@..R>-..@
+00002f30: f1e8 52de cee3 0540 dd99 534a 66d5 0540  ..R....@..SJf..@
+00002f40: d967 2855 e5c8 0640 5d0c 29dc a27b 0840  .g(U...@].)..{.@
+00002f50: 1f7a 73a7 263a 0b40 3b72 12d0 0273 0e40  .zs.&:.@;r...s.@
+00002f60: d132 aa60 ac0e 0f40 57d7 01f5 bfea 1040  .2.`...@W......@
+00002f70: 303d 216b 8d89 1040 c28e ab47 b613 0f40  0=!k...@...G...@
+00002f80: af80 9a3a c3f7 0d40 0819 0d75 4026 1040  ...:...@...u@&.@
+00002f90: eb3a 3469 7334 0f40 cdcc cccc bc94 0d40  .:4is4.@.......@
 00002fa0: cdcc cccc f44d 0c40 98f4 4ee4 cdb3 0b40  .....M.@..N....@
-00002fb0: 830c 1d6a bb38 0a40 eab8 ca7d a85d 0140  ...j.8.@...}.].@
+00002fb0: 820c 1d6a bb38 0a40 ebb8 ca7d a85d 0140  ...j.8.@...}.].@
 00002fc0: 4d27 b243 39bf 0340 9a99 9999 9971 0f40  M'.C9..@.....q.@
 00002fd0: 7a38 3910 d0e8 1340 ae1c cb11 86a5 1740  z89....@.......@
-00002fe0: 67aa 0f6c 72ef 1940 a198 bd6c 6aef 0c40  g..lr..@...lj..@
+00002fe0: 68aa 0f6c 72ef 1940 a198 bd6c 6aef 0c40  h..lr..@...lj..@
 00002ff0: 0000 0080 eaae 0c40 0000 0098 3b69 0c40  .......@....;i.@
 00003000: 0000 00d0 8f0c 0c40 0000 0088 82a7 0b40  .......@.......@
 00003010: cdcc cccc 9c57 0940 29f4 8e14 bc78 0840  .....W.@)....x.@
 00003020: 4b51 1cb1 2051 0840 cdcc cccc d4e8 0840  KQ.. Q.@.......@
 00003030: 9d3d 97a1 db83 0a40 0000 00b8 1603 0b40  .=.....@.......@
-00003040: 277f 457e 3cb3 0a40 618c 62b7 7a05 0d40  '.E~<..@a.b.z..@
-00003050: 918c 0bf2 5cfc 0d40 d57d 8766 e3f0 0a40  ....\..@.}.f...@
-00003060: 4ed1 809b c9cc 0a40 2849 ad90 a100 0a40  N......@(I.....@
-00003070: c88b ce4b 5ece f43f 7411 922e 21c9 f43f  ...K^..?t...!..?
-00003080: 6d5d a309 396e 0640 c11f 821e 9457 0740  m]..9n.@.....W.@
-00003090: 2c72 2c52 02ee 0840 0dd8 42fb 6ec5 0b40  ,r,R...@..B.n..@
-000030a0: ddaa b400 04a1 0e40 ac3b 3bad 1015 1240  .......@.;;....@
-000030b0: 4487 cd32 dbb5 1140 6406 4b85 ba43 1240  D..2...@d.K..C.@
-000030c0: 50db 4a69 03a5 f63f ea57 c630 5ac9 1340  P.Ji...?.W.0Z..@
+00003040: 267f 457e 3cb3 0a40 618c 62b7 7a05 0d40  &.E~<..@a.b.z..@
+00003050: 918c 0bf2 5cfc 0d40 d67d 8766 e3f0 0a40  ....\..@.}.f...@
+00003060: 4fd1 809b c9cc 0a40 2649 ad90 a100 0a40  O......@&I.....@
+00003070: ca8b ce4b 5ece f43f 7411 922e 21c9 f43f  ...K^..?t...!..?
+00003080: 6c5d a309 396e 0640 bd1f 821e 9457 0740  l]..9n.@.....W.@
+00003090: 2c72 2c52 02ee 0840 0cd8 42fb 6ec5 0b40  ,r,R...@..B.n..@
+000030a0: deaa b400 04a1 0e40 ad3b 3bad 1015 1240  .......@.;;....@
+000030b0: 4287 cd32 dbb5 1140 6606 4b85 ba43 1240  B..2...@f.K..C.@
+000030c0: 48db 4a69 03a5 f63f ea57 c630 5ac9 1340  H.Ji...?.W.0Z..@
 000030d0: 7010 fe40 53e0 1040 9c96 dff5 7b15 1140  p..@S..@....{..@
 000030e0: 5dda abeb 2cf7 0e40 cdcc cccc 6427 0d40  ]...,..@....d'.@
-000030f0: d983 45be c72d 0c40 8dfc 5976 4b17 0a40  ..E..-.@..YvK..@
-00003100: 7a2c 3af8 fbcf 0040 bd81 7fbd 7b77 0340  z,:....@....{w.@
-00003110: 1a36 2e54 8478 1440 065b 5e49 83c2 1240  .6.T.x.@.[^I...@
-00003120: 1a93 7d2e 2bf5 1840 ee4c 9e57 0d9d 1f40  ..}.+..@.L.W...@
+000030f0: db83 45be c72d 0c40 8efc 5976 4b17 0a40  ..E..-.@..YvK..@
+00003100: 7b2c 3af8 fbcf 0040 bd81 7fbd 7b77 0340  {,:....@....{w.@
+00003110: 1836 2e54 8478 1440 055b 5e49 83c2 1240  .6.T.x.@.[^I...@
+00003120: 1a93 7d2e 2bf5 1840 f04c 9e57 0d9d 1f40  ..}.+..@.L.W...@
 00003130: e736 b2e0 9c14 1040 3333 3333 f353 0f40  .6.....@3333.S.@
 00003140: 1d6a 9636 6b72 0c40 0000 0098 3c1d 0c40  .j.6kr.@....<..@
-00003150: 0000 0060 febd 0b40 d48b 8021 6d33 0b40  ...`...@...!m3.@
+00003150: 0000 0060 febd 0b40 d38b 8021 6d33 0b40  ...`...@...!m3.@
 00003160: cdcc cccc 34d7 0840 b2bb f8d2 d38c 0840  ....4..@.......@
 00003170: cdcc cccc 2c28 0940 3a8f 7ba6 ac31 0b40  ....,(.@:.{..1.@
-00003180: 672f d5d8 5403 0b40 ca24 8276 ae60 0d40  g/..T..@.$.v.`.@
-00003190: c569 ebfb fa66 1040 1c26 c695 bc43 1040  .i...f.@.&...C.@
-000031a0: acaa c13e d4f7 1c40 42a0 ef60 3660 1640  ...>...@B..`6`.@
-000031b0: 1e15 41ba 0fc1 0940 928a 68c7 cbf2 0940  ..A....@..h....@
-000031c0: c7b0 3266 f98c 0b40 da8a 2a80 fe1e 0840  ..2f...@..*....@
-000031d0: 939d 5140 e5de 0740 1312 bb16 1d60 0840  ..Q@...@.....`.@
-000031e0: 3717 e5b8 7bf3 0b40 5744 7553 3e59 0d40  7...{..@WDuS>Y.@
-000031f0: 983e 0a7a c924 1240 004a 4b73 b98e 2040  .>.z.$.@.JKs.. @
-00003200: 82e6 0acc ad2a 2640 cf61 e235 6043 2940  .....*&@.a.5`C)@
-00003210: 1e32 65be 3c26 1d40 2904 5b5f 15bf 1340  .2e.<&.@).[_...@
-00003220: 3424 3255 b330 0140 5a8a 9d77 1849 1040  4$2U.0.@Z..w.I.@
-00003230: cdcc cccc 7cff 0d40 ec20 cce5 54e8 0c40  ....|..@. ..T..@
-00003240: 29ad 683c 16e7 0a40 0abd 26d2 6c79 0340  ).h<...@..&.ly.@
-00003250: b03a 84d2 f95d fa3f dcdb 3ae9 4cec 1340  .:...].?..:.L..@
-00003260: 4616 54c1 2791 3040 ef0a 19e6 23d0 3040  F.T.'.0@....#.0@
+00003180: 672f d5d8 5403 0b40 c924 8276 ae60 0d40  g/..T..@.$.v.`.@
+00003190: c569 ebfb fa66 1040 1e26 c695 bc43 1040  .i...f.@.&...C.@
+000031a0: aaaa c13e d4f7 1c40 42a0 ef60 3660 1640  ...>...@B..`6`.@
+000031b0: 1f15 41ba 0fc1 0940 908a 68c7 cbf2 0940  ..A....@..h....@
+000031c0: c8b0 3266 f98c 0b40 da8a 2a80 fe1e 0840  ..2f...@..*....@
+000031d0: 919d 5140 e5de 0740 1312 bb16 1d60 0840  ..Q@...@.....`.@
+000031e0: 3817 e5b8 7bf3 0b40 5744 7553 3e59 0d40  8...{..@WDuS>Y.@
+000031f0: 973e 0a7a c924 1240 004a 4b73 b98e 2040  .>.z.$.@.JKs.. @
+00003200: 80e6 0acc ad2a 2640 cf61 e235 6043 2940  .....*&@.a.5`C)@
+00003210: 1e32 65be 3c26 1d40 2a04 5b5f 15bf 1340  .2e.<&.@*.[_...@
+00003220: 3824 3255 b330 0140 5a8a 9d77 1849 1040  8$2U.0.@Z..w.I.@
+00003230: cdcc cccc 7cff 0d40 ed20 cce5 54e8 0c40  ....|..@. ..T..@
+00003240: 29ad 683c 16e7 0a40 0bbd 26d2 6c79 0340  ).h<...@..&.ly.@
+00003250: a83a 84d2 f95d fa3f dedb 3ae9 4cec 1340  .:...].?..:.L..@
+00003260: 4616 54c1 2791 3040 f00a 19e6 23d0 3040  F.T.'.0@....#.0@
 00003270: 6174 0040 4abf 2b40 087c 6041 4c84 1140  at.@J.+@.|`AL..@
-00003280: 2556 5cf9 13c7 1040 3333 3333 835b 0f40  %V\....@3333.[.@
+00003280: 2656 5cf9 13c7 1040 3333 3333 835b 0f40  &V\....@3333.[.@
 00003290: 0000 0090 d72b 0c40 0000 0098 cfd0 0b40  .....+.@.......@
 000032a0: 5627 3c6c a067 0b40 cdcc cccc fc2d 0940  V'<l.g.@.....-.@
 000032b0: febe e137 56be 0840 0a63 d4ad 1237 0940  ...7V..@.c...7.@
 000032c0: c5f0 6de4 8634 0b40 5f2b 040c 585a 0b40  ..m..4.@_+..XZ.@
-000032d0: e26b 8118 1311 0f40 9488 ff9b 4e73 1140  .k.....@....Ns.@
-000032e0: 8444 a0f6 90f3 1840 6388 0bdf 4cda 2140  .D.....@c...L.!@
-000032f0: 0f79 386e bc34 2340 bea7 a389 181b 0f40  .y8n.4#@.......@
-00003300: 3a0c 8963 2ee4 0f40 feab 1590 564c 0c40  :..c...@....VL.@
-00003310: e891 8b50 2fe5 0940 0c25 468a e6e7 0740  ...P/..@.%F....@
+000032d0: e46b 8118 1311 0f40 9488 ff9b 4e73 1140  .k.....@....Ns.@
+000032e0: 8444 a0f6 90f3 1840 6288 0bdf 4cda 2140  .D.....@b...L.!@
+000032f0: 0f79 386e bc34 2340 c4a7 a389 181b 0f40  .y8n.4#@.......@
+00003300: 3a0c 8963 2ee4 0f40 fcab 1590 564c 0c40  :..c...@....VL.@
+00003310: e791 8b50 2fe5 0940 0c25 468a e6e7 0740  ...P/..@.%F....@
 00003320: 4fd4 5c69 538d 0640 9a99 9999 99d9 0540  O.\iS..@.......@
-00003330: e9d3 977b fe28 0440 2c96 c61d c2d0 0f40  ...{.(.@,......@
-00003340: 85cd eea2 bb67 2540 9912 1e9c 7a6c 3240  .....g%@....zl2@
-00003350: c731 d2b3 c7ba 2940 de9c e9f3 6428 1f40  .1....)@....d(.@
-00003360: de03 09fa 01b7 1440 1489 727c 4853 fb3f  .......@..r|HS.?
-00003370: 26aa 2ab4 7cea 1040 cdcc cccc 7ca1 0e40  &.*.|..@....|..@
+00003330: e6d3 977b fe28 0440 3096 c61d c2d0 0f40  ...{.(.@0......@
+00003340: 84cd eea2 bb67 2540 9a12 1e9c 7a6c 3240  .....g%@....zl2@
+00003350: c631 d2b3 c7ba 2940 e09c e9f3 6428 1f40  .1....)@....d(.@
+00003360: df03 09fa 01b7 1440 1489 727c 4853 fb3f  .......@..r|HS.?
+00003370: 25aa 2ab4 7cea 1040 cdcc cccc 7ca1 0e40  %.*.|..@....|..@
 00003380: 8612 f85c 0993 0d40 7d64 9f35 f80d 0c40  ...\...@}d.5...@
-00003390: bf69 1d9f 12bc 0640 1191 4287 80cd 0040  .i.....@..B....@
-000033a0: 32a4 aa4e 6c46 1340 0c95 9158 eb7b 3340  2..NlF.@...X.{3@
+00003390: bf69 1d9f 12bc 0640 1391 4287 80cd 0040  .i.....@..B....@
+000033a0: 30a4 aa4e 6c46 1340 0c95 9158 eb7b 3340  0..NlF.@...X.{3@
 000033b0: 916e e1b0 4739 3940 cccc cccc ccd2 3040  .n..G99@......0@
-000033c0: 2a23 c807 c6a8 1240 08ec 60ef 4b92 1140  *#.....@..`.K..@
+000033c0: 2823 c807 c6a8 1240 08ec 60ef 4b92 1140  (#.....@..`.K..@
 000033d0: b3c3 e3ba 162d 1040 6766 ee1a a42a 0c40  .....-.@gf...*.@
 000033e0: 0000 0070 59da 0b40 0790 7bfa 5a85 0b40  ...pY..@..{.Z..@
 000033f0: cdcc cccc e46a 0940 bc15 f989 bce4 0840  .....j.@.......@
-00003400: 0df4 456b f443 0940 4dc1 cddf 1934 0b40  ..Ek.C.@M....4.@
-00003410: 5f42 4f40 b77f 0b40 c301 c86b b205 1040  _BO@...@...k...@
-00003420: 9699 422e 423f 1240 64ca 51d4 423d 1740  ..B.B?.@d.Q.B=.@
-00003430: 0f9d 966f 7cd8 2140 bd8b f622 d24d 2040  ...o|.!@...".M @
+00003400: 0df4 456b f443 0940 4ec1 cddf 1934 0b40  ..Ek.C.@N....4.@
+00003410: 5f42 4f40 b77f 0b40 c401 c86b b205 1040  _BO@...@...k...@
+00003420: 9699 422e 423f 1240 62ca 51d4 423d 1740  ..B.B?.@b.Q.B=.@
+00003430: 109d 966f 7cd8 2140 bd8b f622 d24d 2040  ...o|.!@...".M @
 00003440: d415 1dca 5ccc 1840 7f83 56ae 228a 0f40  ....\..@..V."..@
-00003450: e45a 3d9c 6430 0d40 698a 4e10 bda5 0a40  .Z=.d0.@i.N....@
+00003450: e35a 3d9c 6430 0d40 688a 4e10 bda5 0a40  .Z=.d0.@h.N....@
 00003460: 19d9 e803 ce8a 0740 ea52 32bc 4dd3 fd3f  .......@.R2.M..?
-00003470: a0b3 bfea 414b fc3f 70ec fa70 0d6c c63f  ....AK.?p..p.l.?
-00003480: 367d f901 4d92 1440 28ec 19ee 8411 1b40  6}..M..@(......@
+00003470: a0b3 bfea 414b fc3f b0ec fa70 0d6c c63f  ....AK.?...p.l.?
+00003480: 367d f901 4d92 1440 26ec 19ee 8411 1b40  6}..M..@&......@
 00003490: 260d 2896 0a70 2540 944e 8d32 81f1 2540  &.(..p%@.N.2..%@
 000034a0: 38d8 0436 6a38 1640 6e73 a1a8 25b7 1440  8..6j8.@ns..%..@
 000034b0: a98a 93ce 8465 0140 5801 c44d 025f 1140  .....e.@X..M._.@
-000034c0: b783 ac55 a8f8 0e40 ffa4 8c94 eddf 0d40  ...U...@.......@
+000034c0: b583 ac55 a8f8 0e40 00a5 8c94 eddf 0d40  ...U...@.......@
 000034d0: 6292 f959 00e6 0540 d2fb bcd5 d4b7 0a40  b..Y...@.......@
-000034e0: f88e 7bc3 8354 1240 d838 7cf8 9fff 1d40  ..{..T.@.8|....@
+000034e0: f88e 7bc3 8354 1240 da38 7cf8 9fff 1d40  ..{..T.@.8|....@
 000034f0: 9a99 9999 9981 2b40 cccc cccc cce3 3040  ......+@......0@
 00003500: 96be 9d65 8413 3140                      ...e..1@
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/2d_no_background.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/ref_data/2d_no_background.npz`

 * *Files 24% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 13712 bytes, number of entries: 1
-?rw-------  2.0 unx    13576 b- stor 80-Jan-01 00:00 arr_0.npy
+?rw-------  4.5 unx    13576 b- stor 80-Jan-01 00:00 arr_0.npy
 1 file, 13576 bytes uncompressed, 13576 bytes compressed:  0.0%
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v4.5 to extract, compression method=store
```

#### arr_0.npy

```diff
@@ -21,16 +21,16 @@
 00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000160: 6eb2 3e9a 5bc8 0540 3809 c82f daaf fc3f  n.>.[..@8../...?
 00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000180: 00f9 e696 ee2c 8a3f 0000 0000 0000 0000  .....,.?........
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: e060 39ab 565f d23f cc33 2d39 99f7 ea3f  .`9.V_.?.3-9...?
-000001b0: 2b53 176a cd14 0d40 2439 1ca0 980d f63f  +S.j...@$9.....?
-000001c0: d02e b8b2 3f45 f23f 0000 0000 0000 0000  ....?E.?........
+000001b0: 2d53 176a cd14 0d40 2439 1ca0 980d f63f  -S.j...@$9.....?
+000001c0: cc2e b8b2 3f45 f23f 0000 0000 0000 0000  ....?E.?........
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -41,15 +41,15 @@
 00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000002c0: 0000 0000 0000 0000 009d fcd2 a170 803f  .............p.?
 000002d0: 8043 557a cdc4 993f 0000 0000 0000 0000  .CUz...?........
 000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: c411 07fc 48c5 e13f f48b df21 4aea eb3f  ....H..?...!J..?
+000002f0: c411 07fc 48c5 e13f ec8b df21 4aea eb3f  ....H..?...!J..?
 00000300: f83d 5fdb 0920 ee3f f0dc 61d6 8264 ea3f  .=_.. .?..a..d.?
 00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -82,16 +82,16 @@
 00000510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000580: 0000 0000 0000 0000 b8ee 7719 22e7 a63f  ..........w."..?
-00000590: a0e4 dce5 7711 b13f e0a8 ca23 77da b33f  ....w..?...#w..?
+00000580: 0000 0000 0000 0000 f8ee 7719 22e7 a63f  ..........w."..?
+00000590: c0e4 dce5 7711 b13f e0a8 ca23 77da b33f  ....w..?...#w..?
 000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -113,15 +113,15 @@
 00000700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000750: 0000 0000 0000 0000 f0b2 b79e ec35 933f  .............5.?
 00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000770: e07e 73c4 3ade 8a3f 0000 0000 0000 0000  .~s.:..?........
+00000770: e07f 73c4 3ade 8a3f 0000 0000 0000 0000  ..s.:..?........
 00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -240,83 +240,83 @@
 00000ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f60: 604c 349b 21b8 c53f 2892 e5d0 fec3 d13f  `L4.!..?(......?
-00000f70: 5001 729d b0bf c43f 0000 0000 0000 0000  P.r....?........
+00000f60: 804c 349b 21b8 c53f 2892 e5d0 fec3 d13f  .L4.!..?(......?
+00000f70: 4001 729d b0bf c43f 0000 0000 0000 0000  @.r....?........
 00000f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 4267 e744 dec9 ce3f  ........Bg.D...?
-00000fd0: 0879 8837 69fd e43f c02a 7e89 4e24 e63f  .y.7i..?.*~.N$.?
+00000fd0: f878 8837 69fd e43f c02a 7e89 4e24 e63f  .x.7i..?.*~.N$.?
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000010a0: 0000 0000 0000 0000 4052 fd26 fd79 d63f  ........@R.&.y.?
+000010a0: 0000 0000 0000 0000 3852 fd26 fd79 d63f  ........8R.&.y.?
 000010b0: 5e15 67fe 1311 c73f a6dc 2ede 884d fc3f  ^.g....?.....M.?
 000010c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001100: 0000 0000 0000 0000 285c 3fd0 9bd2 e03f  ........(\?....?
-00001110: 0000 0000 0000 0000 4726 f906 390b 0640  ........G&..9..@
+00001110: 0000 0000 0000 0000 4526 f906 390b 0640  ........E&..9..@
 00001120: 598a 6593 4bc6 0640 0000 0000 0000 0000  Y.e.K..@........
 00001130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000011e0: 0000 0000 0000 0000 c038 f067 dde8 cf3f  .........8.g...?
-000011f0: e0a6 0610 e342 d43f 758e 34c2 0f42 0a40  .....B.?u.4..B.@
-00001200: aab6 a42b c990 1540 d051 c37f 712c 1440  ...+...@.Q..q,.@
+000011e0: 0000 0000 0000 0000 d038 f067 dde8 cf3f  .........8.g...?
+000011f0: d8a6 0610 e342 d43f 798e 34c2 0f42 0a40  .....B.?y.4..B.@
+00001200: acb6 a42b c990 1540 ce51 c37f 712c 1440  ...+...@.Q..q,.@
 00001210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001250: 104e 09be cc44 c03f 3698 d97b af8d 1640  .N...D.?6..{...@
+00001250: 104e 09be cc44 c03f 3898 d97b af8d 1640  .N...D.?8..{...@
 00001260: 7d87 7ff7 8f21 2740 b27e 2c06 fe70 1a40  }....!'@.~,..p.@
 00001270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000012a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000012b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000012c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000012d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000012e0: a600 9451 f28f 0a40 0000 0000 0000 0000  ...Q...@........
 000012f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001330: 909a 3039 fe67 cf3f ae72 410b 928d cc3f  ..09.g.?.rA....?
+00001330: a09a 3039 fe67 cf3f be72 410b 928d cc3f  ..09.g.?.rA....?
 00001340: e2b8 54f8 d6b0 1140 14b0 d00e 9345 1540  ..T....@.....E.@
-00001350: 5b53 4691 9223 0440 0000 0000 0000 0000  [SF..#.@........
+00001350: 5d53 4691 9223 0440 0000 0000 0000 0000  ]SF..#.@........
 00001360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001390: 906e da41 3e4d c43f d09f 2dd4 18c1 ca3f  .n.A>M.?..-....?
-000013a0: b8b5 6a41 86f2 1040 102e 161f 64e3 1740  ..jA...@....d..@
+00001390: 906e da41 3e4d c43f 909f 2dd4 18c1 ca3f  .n.A>M.?..-....?
+000013a0: b8b5 6a41 86f2 1040 0c2e 161f 64e3 1740  ..jA...@....d..@
 000013b0: 8c1d c40b 860f 1340 0000 0000 0000 0000  .......@........
 000013c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -328,16 +328,16 @@
 00001470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001480: b836 8b71 9cdb a53f b10a fe08 1f5c 0340  .6.q...?.....\.@
 00001490: ef60 4d7c 08f1 0040 0000 0000 0000 0000  .`M|...@........
 000014a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000014b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000014c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000014d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000014e0: 887b 7e1b 39fa e03f 98c9 26a0 e658 d63f  .{~.9..?..&..X.?
-000014f0: 888c 81c9 532d d93f b438 9ff3 0f21 e13f  ....S-.?.8...!.?
+000014e0: 907b 7e1b 39fa e03f a8c9 26a0 e658 d63f  .{~.9..?..&..X.?
+000014f0: 988c 81c9 532d d93f b438 9ff3 0f21 e13f  ....S-.?.8...!.?
 00001500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -348,16 +348,16 @@
 000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001620: 0000 0000 0000 0000 c015 b463 b0de be3f  ...........c...?
-00001630: e089 ce51 25d3 d23f d1be b249 b017 da3f  ...Q%..?...I...?
+00001620: 0000 0000 0000 0000 0016 b463 b0de be3f  ...........c...?
+00001630: d089 ce51 25d3 d23f d1be b249 b017 da3f  ...Q%..?...I...?
 00001640: 0161 ca51 03d0 db3f 0000 0000 0000 0000  .a.Q...?........
 00001650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000016a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -480,16 +480,16 @@
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e60: 0000 0000 0000 0000 00b3 aabc 3e22 9c3f  ............>".?
-00001e70: 8015 1514 91df a33f e0d9 1920 9387 853f  .......?... ...?
+00001e60: 0000 0000 0000 0000 80b2 aabc 3e22 9c3f  ............>".?
+00001e70: 8015 1514 91df a33f e0d8 1920 9387 853f  .......?... ...?
 00001e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -501,130 +501,130 @@
 00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fb0: 4e50 d6b5 593e cd3f 802f df66 9e2d d53f  NP..Y>.?./.f.-.?
+00001fb0: 4e50 d6b5 593e cd3f 702f df66 9e2d d53f  NP..Y>.?p/.f.-.?
 00001fc0: 9799 9959 5809 d53f 2e33 33b3 2848 cd3f  ...YX..?.33.(H.?
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 99c2 4300 4701 d13f  ..........C.G..?
-00002010: 38aa fbf6 a85c e33f c8d4 0c7c fa06 d53f  8....\.?...|...?
-00002020: 10d3 e42d a9ba db3f 0000 0000 0000 0000  ...-...?........
+00002010: 38aa fbf6 a85c e33f b8d4 0c7c fa06 d53f  8....\.?...|...?
+00002020: 00d3 e42d a9ba db3f 0000 0000 0000 0000  ...-...?........
 00002030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002060: 0000 0000 0000 0000 d20b 9e0d ae5f cd3f  ............._.?
-00002070: 213a 1454 07f3 d83f 0d1a 0a31 7a22 ec3f  !:.T...?...1z".?
+00002060: 0000 0000 0000 0000 b20b 9e0d ae5f cd3f  ............._.?
+00002070: 313a 1454 07f3 d83f 151a 0a31 7a22 ec3f  1:.T...?...1z".?
 00002080: a09b 0abb 10fa e33f 0000 0000 0000 0000  .......?........
-00002090: 64ce edb7 5c9d b63f 0000 0000 0000 0000  d...\..?........
+00002090: 24ce edb7 5c9d b63f 0000 0000 0000 0000  $...\..?........
 000020a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000020f0: ec89 d4f3 5807 c53f ff67 fc8b e525 0240  ....X..?.g...%.@
-00002100: 889c a0aa 7134 e43f 1788 e2c0 7068 df3f  ....q4.?....ph.?
+000020f0: dc89 d4f3 5807 c53f 0368 fc8b e525 0240  ....X..?.h...%.@
+00002100: 8c9c a0aa 7134 e43f 1788 e2c0 7068 df3f  ....q4.?....ph.?
 00002110: 9799 99d9 f4bc d43f 0000 0000 0000 0000  .......?........
 00002120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002140: 601d 47ab 42fc ca3f 8831 82ef ccd1 e63f  `.G.B..?.1.....?
+00002140: 501d 47ab 42fc ca3f 8031 82ef ccd1 e63f  P.G.B..?.1.....?
 00002150: 0000 0000 0000 0000 25b3 cc91 280c 0840  ........%...(..@
-00002160: e3c8 3787 6205 0940 a87c 355b 104c d93f  ..7.b..@.|5[.L.?
+00002160: dfc8 3787 6205 0940 a87c 355b 104c d93f  ..7.b..@.|5[.L.?
 00002170: 60b0 e152 9440 b73f 0000 0000 0000 0000  `..R.@.?........
 00002180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021a0: 0000 0000 0000 0000 a4d0 29e2 9535 be3f  ..........)..5.?
 000021b0: 0000 0000 0000 0000 6666 668e 354e 0940  ........fff.5N.@
-000021c0: 6666 66e6 21ec 0c40 488a 5de8 94bf d33f  fff.!..@H.]....?
-000021d0: bf09 83d6 4296 d13f dec7 16a9 095e c93f  ....B..?.....^.?
-000021e0: 2792 94a8 f98e 0540 4e87 29e9 3cfc c43f  '......@N.).<..?
+000021c0: 6666 66e6 21ec 0c40 388a 5de8 94bf d33f  fff.!..@8.]....?
+000021d0: bf09 83d6 4296 d13f fec7 16a9 095e c93f  ....B..?.....^.?
+000021e0: 2592 94a8 f98e 0540 5e87 29e9 3cfc c43f  %......@^.).<..?
 000021f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002230: 40ba 1422 304f c43f 2e81 e65d 508c fd3f  @.."0O.?...]P..?
-00002240: 5a09 7b50 c57e 1640 9589 78a2 1535 0840  Z.{P.~.@..x..5.@
-00002250: 740b 6bb6 eaf9 e13f 9799 99d9 4db3 d53f  t.k....?....M..?
+00002230: 40ba 1422 304f c43f 2681 e65d 508c fd3f  @.."0O.?&..]P..?
+00002240: 5a09 7b50 c57e 1640 9189 78a2 1535 0840  Z.{P.~.@..x..5.@
+00002250: 780b 6bb6 eaf9 e13f 9799 99d9 4db3 d53f  x.k....?....M..?
 00002260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002280: 0000 0000 0000 0000 7194 8c28 03d8 d73f  ........q..(...?
-00002290: 0000 0000 0000 0000 de51 72e8 1a1d 1b40  .........Qr....@
-000022a0: 9df4 07a5 f709 2540 dc39 4682 e18a 1540  ......%@.9F....@
-000022b0: b057 581f 88c6 c13f 80be c12f 507f ce3f  .WX....?.../P..?
+00002280: 0000 0000 0000 0000 8194 8c28 03d8 d73f  ...........(...?
+00002290: 0000 0000 0000 0000 da51 72e8 1a1d 1b40  .........Qr....@
+000022a0: 9ff4 07a5 f709 2540 de39 4682 e18a 1540  ......%@.9F....@
+000022b0: 9057 581f 88c6 c13f 60be c12f 507f ce3f  .WX....?`../P..?
 000022c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000022d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000022e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000022f0: 6161 44e4 cb77 d63f 6666 66e6 7b04 0640  aaD..w.?fff.{..@
 00002300: 0fb8 9f1c 3154 2040 dc73 bc55 6fcc 2b40  ....1T @.s.Uo.+@
-00002310: a238 a4db 7f9b 1540 69ee a711 147c 0940  .8.....@i....|.@
+00002310: a038 a4db 7f9b 1540 69ee a711 147c 0940  .8.....@i....|.@
 00002320: 6714 df17 38b3 0c40 dd15 9580 4fd0 0a40  g...8..@....O..@
-00002330: 8755 3fff d482 da3f 9799 9959 7bc9 d03f  .U?....?...Y{..?
+00002330: 8f55 3fff d482 da3f 9799 9959 7bc9 d03f  .U?....?...Y{..?
 00002340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002370: 0000 0000 0000 0000 40c7 2d89 20cb c63f  ........@.-. ..?
-00002380: 7c41 107c b8d0 c93f e94f a99e c0cf 0340  |A.|...?.O.....@
-00002390: 5f6c 70df cbf5 0740 3ffc f132 6665 d63f  _lp....@?..2fe.?
+00002380: 6c41 107c b8d0 c93f eb4f a99e c0cf 0340  lA.|...?.O.....@
+00002390: 616c 70df cbf5 0740 37fc f132 6665 d63f  alp....@7..2fe.?
 000023a0: 2e33 3333 4b91 cf3f 0000 0000 0000 0000  .333K..?........
 000023b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000023c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023d0: c13c ed18 9f15 d63f 1081 725e 59a7 cb3f  .<.....?..r^Y..?
+000023d0: c13c ed18 9f15 d63f 3081 725e 59a7 cb3f  .<.....?0.r^Y..?
 000023e0: 0a2d 4bac 585a 1140 68a7 4d64 2853 2540  .-K.XZ.@h.Md(S%@
 000023f0: 747d 8af2 aa5c 1340 107d 3304 af49 cf3f  t}...\.@.}3..I.?
 00002400: 0035 fea5 af49 d23f 0000 0000 0000 0000  .5...I.?........
 00002410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002440: 6666 66fe 854b 0740 9aff e2c6 75c3 2940  fff..K.@....u.)@
 00002450: 4ee4 83c3 981d 1f40 9a7b 976c 0821 1640  N......@.{.l.!.@
-00002460: ef57 bbdb ea06 0a40 6e05 eb45 a648 f23f  .W.....@n..E.H.?
-00002470: 2c1f 8b50 21af e93f a7b4 b90d 56dc df3f  ,..P!..?....V..?
+00002460: ed57 bbdb ea06 0a40 6e05 eb45 a648 f23f  .W.....@n..E.H.?
+00002470: 2c1f 8b50 21af e93f afb4 b90d 56dc df3f  ,..P!..?....V..?
 00002480: 9799 99d9 767b d13f 0000 0000 0000 0000  ....v{.?........
 00002490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000024c0: 0000 0000 0000 0000 3094 a613 13b9 c03f  ........0......?
-000024d0: 9c5b 8966 88fc b93f dc70 3aaf 19a5 bf3f  .[.f...?.p:....?
-000024e0: c0cd b5fb 0d5f be3f 0000 0000 0000 0000  ....._.?........
+000024d0: bc5b 8966 88fc b93f dc70 3aaf 19a5 bf3f  .[.f...?.p:....?
+000024e0: a0cd b5fb 0d5f be3f 0000 0000 0000 0000  ....._.?........
 000024f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002510: 0000 0000 0000 0000 00c1 fe8d 6530 c33f  ............e0.?
-00002520: 2722 75d3 262d d13f 6666 66ee e4a5 0440  '"u.&-.?fff....@
-00002530: eebf 6410 6152 1240 f501 d938 4c68 0840  ..d.aR.@...8Lh.@
-00002540: b7ef ac88 afc5 d63f 7224 fc8f bd9b c03f  .......?r$.....?
+00002510: 0000 0000 0000 0000 10c1 fe8d 6530 c33f  ............e0.?
+00002520: 3722 75d3 262d d13f 6666 66ee e4a5 0440  7"u.&-.?fff....@
+00002530: eebf 6410 6152 1240 f701 d938 4c68 0840  ..d.aR.@...8Lh.@
+00002540: b7ef ac88 afc5 d63f 3224 fc8f bd9b c03f  .......?2$.....?
 00002550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002590: 3fe0 38b6 5694 0e40 6666 660e 9621 0c40  ?.8.V..@fff..!.@
-000025a0: 3435 e70d ccf0 ed3f 8cf9 12c7 c391 ee3f  45.....?.......?
+00002590: 3be0 38b6 5694 0e40 6666 660e 9621 0c40  ;.8.V..@fff..!.@
+000025a0: 2c35 e70d ccf0 ed3f 8cf9 12c7 c391 ee3f  ,5.....?.......?
 000025b0: e4c6 f7ec 4e62 e93f 5877 3d71 1efa e23f  ....Nb.?Xw=q...?
 000025c0: 9799 99d9 f48b da3f 808e 229e 32f0 903f  .......?..".2..?
 000025d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000025e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000025f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002660: 0000 0000 0000 0000 19e7 c245 a170 d43f  ...........E.p.?
-00002670: 7860 a199 b12e d53f 18a8 ad72 88c3 d13f  x`.....?...r...?
-00002680: 8868 883f 03ce d73f b9a4 645f 5310 d73f  .h.?...?..d_S..?
+00002670: 6860 a199 b12e d53f 08a8 ad72 88c3 d13f  h`.....?...r...?
+00002680: 7868 883f 03ce d73f a9a4 645f 5310 d73f  xh.?...?..d_S..?
 00002690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000026a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000026b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000026c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000026d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026e0: 554a 5f4d 5a29 e73f f0bb c659 b96a ee3f  UJ_MZ).?...Y.j.?
+000026e0: 3d4a 5f4d 5a29 e73f f0bb c659 b96a ee3f  =J_MZ).?...Y.j.?
 000026f0: cccc ccac c9c6 e13f cccc cc2c 1f11 e03f  .......?...,...?
 00002700: 9799 9959 893f da3f 9799 99d9 d497 d13f  ...Y.?.?.......?
 00002710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -760,90 +760,90 @@
 00002f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002fe0: 70a6 fa00 90e7 d73f e0a0 98bd 54d4 893f  p......?....T..?
+00002fe0: 80a6 fa00 90e7 d73f e0a0 98bd 54d4 893f  .......?....T..?
 00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003040: 0000 0000 0000 0000 10c6 2876 09d3 ca3f  ..........(v...?
 00003050: 8864 5c90 ce01 d43f 0000 0000 0000 0000  .d\....?........
 00003060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000030a0: 0000 0000 0000 0000 c0ba b3d3 2a6c db3f  ............*l.?
-000030b0: 70e8 b059 e07d ce3f 4866 b0d4 6862 d33f  p..Y.}.?Hf..hb.?
+000030a0: 0000 0000 0000 0000 d0ba b3d3 2a6c db3f  ............*l.?
+000030b0: 50e8 b059 e07d ce3f 6866 b0d4 6862 d33f  P..Y.}.?hf..hb.?
 000030c0: 0000 0000 0000 0000 50bf 3206 b15d e33f  ........P.2..].?
 000030d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000030e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000030f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003120: 0000 0000 0000 0000 ba33 795e 5aaa f73f  .........3y^Z..?
+00003120: 0000 0000 0000 0000 c233 795e 5aaa f73f  .........3y^Z..?
 00003130: 6e6e 230b a44e da3f 9799 9919 2dd1 d43f  nn#..N.?....-..?
 00003140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003180: 0000 0000 0000 0000 a04c 22e8 8635 cb3f  .........L"..5.?
-00003190: 284e 5b5f 23a3 e33f e430 31ae b9d4 e13f  (N[_#..?.01....?
-000031a0: 5955 8315 36bf 0d40 8540 dfd1 f17d 0040  YU..6..@.@...}.@
+00003180: 0000 0000 0000 0000 904c 22e8 8635 cb3f  .........L"..5.?
+00003190: 284e 5b5f 23a3 e33f f430 31ae b9d4 e13f  (N[_#..?.01....?
+000031a0: 5555 8315 36bf 0d40 8340 dfd1 f17d 0040  UU..6..@.@...}.@
 000031b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000031e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000031f0: 81e9 a360 f1a9 d63f ff27 2d75 16f4 0f40  ...`...?.'-u...@
-00003200: 04cd 15c0 aee1 1a40 cf61 e2f3 1a6f 2040  .......@.a...o @
-00003210: 3d64 ca2c 3cba 0640 9142 b0b5 079b dd3f  =d.,<..@.B.....?
+000031f0: 71e9 a360 f1a9 d63f ff27 2d75 16f4 0f40  q..`...?.'-u...@
+00003200: 00cd 15c0 aee1 1a40 cf61 e2f3 1a6f 2040  .......@.a...o @
+00003210: 3b64 ca2c 3cba 0640 a142 b0b5 079b dd3f  ;d.,<..@.B.....?
 00003220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003260: 8c2c a8aa 015d 2440 de15 3270 8c71 2440  .,...]$@..2p.q$@
-00003270: c2e8 00b4 d7b2 1c40 44e0 03ab 297e e83f  .......@D...)~.?
-00003280: 28b1 e22a ae27 e33f 9799 9999 4bc9 d63f  (..*.'.?....K..?
+00003260: 8b2c a8aa 015d 2440 df15 3270 8c71 2440  .,...]$@..2p.q$@
+00003270: c2e8 00b4 d7b2 1c40 3ce0 03ab 297e e83f  .......@<...)~.?
+00003280: 30b1 e22a ae27 e33f 9799 9999 4bc9 d63f  0..*.'.?....K..?
 00003290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000032a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000032b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000032c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000032d0: 105f 0bc4 101d d83f a444 fc7f 965d ea3f  ._.....?.D...].?
-000032e0: 0989 4075 be63 0540 c610 1726 f161 1540  ..@u.c.@...&.a.@
-000032f0: 1ef2 70c4 710d 1840 f03d 1d8d 86ad d23f  ..p.q..@.=.....?
+000032d0: 205f 0bc4 101d d83f a444 fc7f 965d ea3f   _.....?.D...].?
+000032e0: 0789 4075 be63 0540 c410 1726 f161 1540  ..@u.c.@...&.a.@
+000032f0: 1ef2 70c4 710d 1840 203e 1d8d 86ad d23f  ..p.q..@ >.....?
 00003300: d061 481c 0918 d83f 0000 0000 0000 0000  .aH....?........
 00003310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003340: 0a9b dd9d 5b63 1940 3225 3c5a 28f9 2b40  ....[c.@2%<Z(.+@
-00003350: c731 d275 72bf 2040 bd39 d377 631f 0a40  .1.ur. @.9.wc..@
-00003360: f01e 48d0 a004 e43f 0000 0000 0000 0000  ..H....?........
+00003340: 089b dd9d 5b63 1940 3425 3c5a 28f9 2b40  ....[c.@4%<Z(.+@
+00003350: c631 d275 72bf 2040 bf39 d377 631f 0a40  .1.ur. @.9.wc..@
+00003360: f81e 48d0 a004 e43f 0000 0000 0000 0000  ..H....?........
 00003370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000033a0: 0000 0000 0000 0000 192a 23a3 cdd3 2940  .........*#...)@
 000033b0: 916e e107 a06f 3240 9999 9981 1bd8 2340  .n...o2@......#@
-000033c0: a68c 20ff 54c8 f03f 4060 073b 526e e93f  .. .T..?@`.;Rn.?
+000033c0: a28c 20ff 54c8 f03f 4060 073b 526e e93f  .. .T..?@`.;Rn.?
 000033d0: 2e3b 3cee 0e91 de3f 0000 0000 0000 0000  .;<....?........
 000033e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000033f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003410: 0000 0000 0000 0000 311c 80fc 2c56 de3f  ........1...,V.?
-00003420: accc 1472 4bdb ef3f c994 a350 e7ba 0140  ...rK..?...P...@
-00003430: 1e3a 2d0b 333f 1540 7a17 ede9 5220 1240  .:-.3?.@z...R .@
+00003410: 0000 0000 0000 0000 411c 80fc 2c56 de3f  ........A...,V.?
+00003420: accc 1472 4bdb ef3f c594 a350 e7ba 0140  ...rK..?...P...@
+00003430: 203a 2d0b 333f 1540 7a17 ede9 5220 1240   :-.3?.@z...R .@
 00003440: a92b 3a4c a595 0440 f81b b432 8566 d33f  .+:L...@...2.f.?
 00003450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003480: ace9 cb2f 8a7b eb3f 51d8 336c d6fe 0240  .../.{.?Q.3l...@
+00003480: b4e9 cb2f 8a7b eb3f 4dd8 336c d6fe 0240  .../.{.?M.3l...@
 00003490: 4c1a 5078 cff8 1840 289d 1a6d 83c3 1940  L.Px...@(..m...@
 000034a0: c4c1 26f0 dab0 ef3f 6c9b 0b45 97b2 e23f  ..&....?l..E...?
 000034b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000034c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000034d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000034e0: 0000 0000 0000 0000 5ee3 f021 1732 f23f  ........^..!.2.?
+000034e0: 0000 0000 0000 0000 66e3 f021 1732 f23f  ........f..!.2.?
 000034f0: 3333 33fb c857 1c40 9999 99db 8dff 2340  333..W.@......#@
 00003500: 2c7d 3ba3 3523 2440                      ,};.5#$@
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_denoise.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_denoise.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_geometry_2d.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_geometry_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_image_sampling.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_image_sampling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_io.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_kymotrack.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_kymotrack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_loc_models.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_loc_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_peakfinding.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_peakfinding.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_refinement.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_refinement.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_sequence.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_stitching.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_stitching.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/kymotracker/tests/test_tracing.py` & `lumicks.pylake-1.5.0/lumicks/pylake/kymotracker/tests/test_tracing.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/marker.py` & `lumicks.pylake-1.5.0/lumicks/pylake/marker.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/correlated_plot.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/correlated_plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     frame=0,
     reduce=np.mean,
     colormap="gray",
     figure_scale=0.75,
     post_update=None,
     *,
     vertical=False,
+    downsample_to_frames=True,
 ):
     """Downsample channel on a frame by frame basis and plot the results.
 
     Parameters
     ----------
     channel_slice : pylake.channel.Slice
         Data slice that we with to downsample.
@@ -42,20 +43,29 @@
     post_update : callable
         Function that will be called with the imshow handle and image data after the image data has
         been updated.
     vertical : bool
         Whether plots should be aligned vertically.
     return_handle : bool
         Whether to return a handle to the update function.
+    downsample_to_frames : bool
+        Downsample the channel data over frame timestamp ranges (default: True).
     """
     import matplotlib.pyplot as plt
 
-    downsampled = channel_slice.downsampled_over(frame_timestamps, where="left", reduce=reduce)
+    processed_channel = (
+        channel_slice.downsampled_over(frame_timestamps, where="left", reduce=reduce)
+        if downsample_to_frames
+        else channel_slice[frame_timestamps[0][0] : frame_timestamps[-1][-1]]
+    )
+
+    if len(processed_channel) < 2:
+        raise ValueError("Channel slice must contain at least two data points.")
 
-    if len(downsampled.timestamps) < len(frame_timestamps):
+    if len(processed_channel.timestamps) < len(frame_timestamps):
         warnings.warn("Only subset of time range available for selected channel")
 
     plot_data = get_plot_data(frame)
     aspect_ratio = plot_data.shape[0] / np.max([plot_data.shape])
 
     aspect_ratio = max(0.2, aspect_ratio)
     if vertical:
@@ -64,24 +74,28 @@
         fig, (ax_channel, ax_img) = plt.subplots(
             1,
             2,
             figsize=figure_scale * plt.figaspect(aspect_ratio / (aspect_ratio + 1)),
             gridspec_kw={"width_ratios": [1, 1 / aspect_ratio]},
         )
 
-    t0 = downsampled.timestamps[0]
-    t, y = downsampled.seconds, downsampled.data
+    t0 = processed_channel.timestamps[0]
+    t, y = processed_channel.seconds, processed_channel.data
 
     # We explicitly append the last frame time to make sure that it still shows up
-    last_dt = np.diff(
-        [
-            frame_range
-            for frame_range in frame_timestamps
-            if frame_range[0] >= channel_slice.start and frame_range[1] <= channel_slice.stop
-        ][-1]
+    last_dt = (
+        np.diff(
+            [
+                frame_range
+                for frame_range in frame_timestamps
+                if frame_range[0] >= channel_slice.start and frame_range[1] <= channel_slice.stop
+            ][-1]
+        )
+        if downsample_to_frames
+        else (processed_channel.timestamps[-1] - processed_channel.timestamps[-2])
     )
     t = np.hstack((t, t[-1] + last_dt * 1e-9))
     y = np.hstack((y, y[-1]))
 
     # We want a constant line from the start of the first frame, to the end. So we plot up to
     # the second point.
     ax_channel.step(t, y, where="post")
@@ -105,16 +119,16 @@
             alpha=0.7,
             color="r",
         )
 
     poly = update_position(*frame_timestamps[frame])
 
     ax_channel.set_xlabel("Time [s]")
-    ax_channel.set_ylabel(downsampled.labels["y"])
-    ax_channel.set_title(downsampled.labels["title"])
+    ax_channel.set_ylabel(processed_channel.labels["y"])
+    ax_channel.set_title(processed_channel.labels["title"])
     ax_channel.set_xlim([np.min(t), np.max(t)])
 
     if vertical:
         # Make sure we don't get a really elongated time plot
         x_lims, y_lims = ax_channel.get_xlim(), ax_channel.get_ylim()
         ax_channel.set_aspect(aspect_ratio * abs((x_lims[1] - x_lims[0]) / (y_lims[1] - y_lims[0])))
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/detail/mouse.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/detail/mouse.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/detail/undostack.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/detail/undostack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/image_editing.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/image_editing.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/kymotracker_widgets.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/kymotracker_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,19 +417,18 @@
         import ipywidgets
         import matplotlib.pyplot as plt
         from IPython.display import display
 
         if not max([backend in plt.get_backend() for backend in ("nbAgg", "ipympl")]):
             raise RuntimeError(
                 (
-                    "Please enable an interactive matplotlib backend for this widget to work. In jupyter "
-                    "notebook you can do this by invoking either %matplotlib notebook or %matplotlib "
-                    "widget (the latter requires ipympl to be installed). In Jupyter Lab only the latter "
-                    "works. Please note that you may have to restart the notebook kernel for this to "
-                    "work."
+                    "Please enable an interactive matplotlib backend for this plot to work. In "
+                    "jupyter notebook or lab you can do this by invoking either "
+                    "%matplotlib widget. Please note that you may have to restart the notebook "
+                    "kernel for this to work."
                 )
             )
 
         self._labels["status"] = ipywidgets.Label(value="")
         self._labels["warning"] = ipywidgets.HTML(value="")
 
         algorithm_sliders = self._create_algorithm_sliders()
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/range_selector.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/range_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,19 +269,18 @@
             raise ValueError(
                 "F,d selector widget cannot open without a non-empty dictionary containing F,d curves."
             )
 
         if not any(backend in plt.get_backend() for backend in ("nbAgg", "ipympl")):
             raise RuntimeError(
                 (
-                    "Please enable an interactive matplotlib backend for this plot to work. In jupyter"
-                    "notebook you can do this by invoking either %matplotlib notebook or %matplotlib "
-                    "widget (the latter requires ipympl to be installed). In Jupyter Lab only the latter "
-                    "works. Please note that you may have to restart the notebook kernel for this to "
-                    "work."
+                    "Please enable an interactive matplotlib backend for this plot to work. In "
+                    "jupyter notebook or lab you can do this by invoking either "
+                    "%matplotlib widget. Please note that you may have to restart the notebook "
+                    "kernel for this to work."
                 )
             )
 
         plt.figure()
         self.axes = plt.axes()
         self.active_plot = None
         self.selectors = {key: self._add_widget(curve) for key, curve in fd_curves.items()}
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/conftest.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/test_fd_selector.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_fd_selector.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/test_image_editing.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_image_editing.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/test_mouse.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_mouse.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/nb_widgets/tests/test_undostack.py` & `lumicks.pylake-1.5.0/lumicks/pylake/nb_widgets/tests/test_undostack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/note.py` & `lumicks.pylake-1.5.0/lumicks/pylake/note.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/baseline.py` & `lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/baseline.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/piezo_tracking.py` & `lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/piezo_tracking.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/tests/conftest.py` & `lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/tests/test_baseline.py` & `lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/test_baseline.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py` & `lumicks.pylake-1.5.0/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/point_scan.py` & `lumicks.pylake-1.5.0/lumicks/pylake/point_scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/detail/fit_info.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/detail/fit_info.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/detail/hmm.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/detail/hmm.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/detail/mixin.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/detail/mixin.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/dwelltime.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/dwelltime.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,15 +443,15 @@
             plt.axvspan(lower, upper, **span_kwargs)
             plt.axvline(mean, **line_kwargs)
             plt.xlabel(f"{key}" if key == "amplitude" else f"{key} (sec)")
             plt.ylabel("counts")
 
             label = "a" if key == "amplitude" else r"\tau"
             unit = "" if key == "amplitude" else "sec"
-            prefix = rf"${label}_{component+1}$" if use_index else rf"${label}$"
+            prefix = rf"${label}_{component + 1}$" if use_index else rf"${label}$"
             plt.title(f"{prefix} = {mean:0.2g} ({lower:0.2g}, {upper:0.2g}) {unit}")
 
         if self.n_components == 1:
             data = self.lifetime_distributions.squeeze()
             plot_axes(data, "lifetime", 0, False)
         else:
             for component in range(self.n_components):
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/hmm.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/hmm.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/mixture.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/mixture.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/tests/conftest.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/tests/data/exponential_data.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/exponential_data.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/tests/data/generate_exponential_data.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/generate_exponential_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/tests/data/generate_trace_data.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/generate_trace_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/tests/data/trace_data.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/data/trace_data.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/tests/test_dwelltimes.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_dwelltimes.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/tests/test_hmm.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_hmm.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/tests/test_hmm_algos.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_hmm_algos.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/population/tests/test_mixture.py` & `lumicks.pylake-1.5.0/lumicks/pylake/population/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/scalebar.py` & `lumicks.pylake-1.5.0/lumicks/pylake/scalebar.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/scan.py` & `lumicks.pylake-1.5.0/lumicks/pylake/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,14 +292,15 @@
         channel="rgb",
         figure_scale=0.75,
         adjustment=no_adjustment,
         *,
         vertical=False,
         include_dead_time=False,
         return_frame_setter=False,
+        downsample_to_frames=True,
     ):
         """Downsample channel on a frame by frame basis and plot the results. The downsampling
         function (e.g. np.mean) is evaluated for the time between a start and end time of a frame.
         Note: In environments which support interactive figures (e.g. jupyter notebook with
         ipywidgets or interactive python) this plot will be interactive.
 
         Actions
@@ -327,14 +328,16 @@
             Color adjustments to apply to the output image.
         vertical : bool, optional
             Align plots vertically.
         include_dead_time : bool, optional
             Include dead time between scan frames.
         return_frame_setter : bool, optional
             Whether to return a handle that allows updating the plotted frame.
+        downsample_to_frames : bool, optional
+            Downsample the channel data over frame timestamp ranges (default: True).
 
         Examples
         --------
         ::
 
             from lumicks import pylake
 
@@ -365,14 +368,15 @@
             title_factory,
             frame,
             reduce,
             colormap=colormaps._get_default_colormap(channel),
             figure_scale=figure_scale,
             post_update=post_update,
             vertical=vertical,
+            downsample_to_frames=downsample_to_frames,
         )
         if return_frame_setter:
             return frame_setter
 
     @property
     def lines_per_frame(self):
         """Number of scanned lines in each frame"""
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/simulation/diffusion.py` & `lumicks.pylake-1.5.0/lumicks/pylake/simulation/diffusion.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/simulation/tests/test_diffusion.py` & `lumicks.pylake-1.5.0/lumicks/pylake/simulation/tests/test_diffusion.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/conftest.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/data/mock_confocal.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/data/mock_fdcurve.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_fdcurve.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/data/mock_file.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_file.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/data/mock_json.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_json.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/data/mock_widefield.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/data/mock_widefield.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,26 +136,30 @@
     description["Camera"] = "IRM"
     return description
 
 
 def make_wt_description(version, bit_depth, m_red, m_blue, offsets):
     if version == 1:
         alignment_matrices = lambda color: f"Alignment {color} channel"
+        wavelength_fields = lambda color: f"Channel {color} detection wavelength (nm)"
         channel_choices = ("red", "green", "blue")
     else:
         alignment_matrices = lambda index: f"Channel {index} alignment"
+        wavelength_fields = lambda index: f"Channel {index} detection wavelength (nm)"
         channel_choices = range(3)
 
     offsets = [0, 0] if offsets is None else offsets
     matrices = (m_red, np.eye(3), m_blue)
+    wavelengths = ("680/42", "600/50", "525/40")
 
     description = _make_base_description(version, bit_depth)
     description["Camera"] = "WT"
-    for c, mat in zip(channel_choices, matrices):
+    for c, mat, wavelength in zip(channel_choices, matrices, wavelengths):
         description[alignment_matrices(c)] = mat[:2].ravel().tolist()
+        description[wavelength_fields(c)] = wavelength
     description["Alignment region of interest (x, y, width, height)"] = [*offsets, 200, 100]
     description["TIRF"] = None
     description["TIRF angle (device units)"] = None
     return description
 
 
 def make_alignment_image_data(
@@ -186,17 +190,16 @@
         warped_image = warped_image[:, :, 1]
     else:
         raise ValueError("camera argument must be 'wt' or 'irm'")
 
     return reference_image, warped_image, description, bit_depth
 
 
-def write_tiff_file(image, description, n_frames, filename):
+def write_tiff_file(image, description, n_frames, filename, **kwargs):
     # We use the dimension of image data to evaluate the number of color channels
-    channels = 1 if image.ndim == 2 else 3
     movie = np.stack([image for n in range(n_frames)], axis=0)
 
     # Orientation = ORIENTATION.TOPLEFT
     tag_orientation = (274, "H", 1, 1, False)
 
     with tifffile.TiffWriter(filename) as tif:
         for n, frame in enumerate(movie):
@@ -206,8 +209,9 @@
             tif.write(
                 frame,
                 description=json.dumps(description, indent=4),
                 software="Bluelake Unknown",
                 metadata=None,
                 contiguous=False,
                 extratags=(tag_orientation, tag_datetime),
+                **kwargs,
             )
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/data/test_mock_confocal.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/data/test_mock_confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/dict[1].npz` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/C1Z88G669DGF5HS3RX4OED5YL.npz`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 543 bytes, number of entries: 1
-?rw-------  2.0 unx      407 b- stor 80-Jan-01 00:00 arr_0.npy
+?rw-------  4.5 unx      407 b- stor 80-Jan-01 00:00 arr_0.npy
 1 file, 407 bytes uncompressed, 407 bytes compressed:  0.0%
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v4.5 to extract, compression method=store
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/reference_data/freezing/dict[2].npz` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/ref_data/60TWXO09A93DLXSNN8B7QAIIT.npz`

 * *Files 22% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 543 bytes, number of entries: 1
-?rw-------  2.0 unx      407 b- stor 80-Jan-01 00:00 arr_0.npy
+?rw-------  4.5 unx      407 b- stor 80-Jan-01 00:00 arr_0.npy
 1 file, 407 bytes uncompressed, 407 bytes compressed:  0.0%
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v4.5 to extract, compression method=store
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_channels/conftest.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_channels/test_arithmetic.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_channels/test_channels.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_channels/test_channels.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_fdcurve.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_fdcurve.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_fdensemble.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_fdensemble.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_file/conftest.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_file/test_file.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/test_file.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_file/test_file_items.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file/test_file_items.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_file_download.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_file_download.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_image.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/data/tiff_from_scan_v1_3_1.tiff` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/data/tiff_from_scan_v1_3_1.tiff`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/reference_data/legacy_exposure_handling/dead_time[False].npz` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/ref_data/21U0E1PWIF4T1V9BXHMY9P90F.npz`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 552 bytes, number of entries: 1
-?rw-------  2.0 unx      416 b- stor 80-Jan-01 00:00 arr_0.npy
+?rw-------  4.5 unx      416 b- stor 80-Jan-01 00:00 arr_0.npy
 1 file, 416 bytes uncompressed, 416 bytes compressed:  0.0%
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v4.5 to extract, compression method=store
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/reference_data/legacy_exposure_handling/dead_time[True].npz` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/ref_data/56OBGN66YAHPLZDQ8KXKGCI2P.npz`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 552 bytes, number of entries: 1
-?rw-------  2.0 unx      416 b- stor 80-Jan-01 00:00 arr_0.npy
+?rw-------  4.5 unx      416 b- stor 80-Jan-01 00:00 arr_0.npy
 1 file, 416 bytes uncompressed, 416 bytes compressed:  0.0%
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v4.5 to extract, compression method=store
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/test_export.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/test_export.py`

 * *Files 27% similar despite different names*

```diff
@@ -35,14 +35,16 @@
                 else:
                     assert "Applied channel 0 alignment" not in tif_out.pages[0].description
                     assert "Channel 0 alignment" in tif_out.pages[0].description
             # Check `_tiff_timestamp_ranges()`
             for page0, page in zip(tif_in.pages, tif_out.pages):
                 assert page0.tags["DateTime"].value == page.tags["DateTime"].value
 
+        stack.close()
+
 
 def test_export_roi(rgb_tiff_file, rgb_tiff_file_multi, gray_tiff_file, gray_tiff_file_multi):
     from os import stat
 
     for filename in (rgb_tiff_file, rgb_tiff_file_multi, gray_tiff_file, gray_tiff_file_multi):
         savename = str(filename.new(purebasename=f"roi_out_{filename.purebasename}"))
         stack = ImageStack(str(filename))[:, 20:80, 10:190]
@@ -50,14 +52,16 @@
         stack.export_tiff(savename)
         assert stat(savename).st_size > 0
 
         with tifffile.TiffFile(savename) as tif:
             assert tif.pages[0].tags["ImageWidth"].value == 180
             assert tif.pages[0].tags["ImageLength"].value == 60
 
+        stack.close()
+
 
 @pytest.mark.parametrize("vertical, correlated", [(False, False), (False, True), (True, True)])
 def test_stack_movie_export(
     tmpdir_factory,
     rgb_tiff_file,
     rgb_tiff_file_multi,
     gray_tiff_file,
@@ -92,7 +96,68 @@
             ValueError,
             match=(
                 "channel must be 'red', 'green', 'blue' or a combination of 'r', 'g', "
                 "and/or 'b', got 'gray'."
             ),
         ):
             stack.export_video("gray", "dummy.gif")  # Gray is not a color!
+
+        stack.close()
+
+
+@pytest.mark.parametrize(
+    "start, stop, ref, correlated",
+    [
+        (None, None, [0, 1], True),
+        (1, None, [1], True),
+        (0, None, [0, 1], True),
+        (0, 2, [0, 1], True),
+        (None, 1, [0], True),
+        (None, None, [0, 1], False),
+        (1, None, [1], False),
+        (0, None, [0, 1], False),
+        (0, 2, [0, 1], False),
+        (None, 1, [0], False),
+    ],
+)
+def test_movie_export_range(
+    monkeypatch, tmpdir_factory, rgb_tiff_file_multi, start, stop, ref, correlated
+):
+    tmpdir = tmpdir_factory.mktemp("pylake")
+    stack = ImageStack(str(rgb_tiff_file_multi))
+
+    dt_stack = stack.frame_timestamp_ranges()[1][0] - stack.frame_timestamp_ranges()[0][0]
+    corr_data = (
+        Slice(
+            Continuous(np.arange(100), stack.start, dt_stack // 2),
+            labels={"title": "title", "y": "y"},
+        )
+        if correlated
+        else None
+    )
+
+    fn = f"{tmpdir}/test.gif"
+
+    with monkeypatch.context() as m:
+        frames = []
+
+        if correlated:
+            # Plot correlated returns a frame setter that export uses to change the frame
+            def faux_set_frame(frame):
+                frames.append(frame)
+
+            def faux_plot_correlated(*_, **__):
+                return faux_set_frame
+
+            m.setattr("lumicks.pylake.image_stack.ImageStack.plot_correlated", faux_plot_correlated)
+        else:
+
+            def faux_plot(*_, frame, **__):
+                frames.append(frame)
+
+            m.setattr("lumicks.pylake.image_stack.ImageStack.plot", faux_plot)
+
+        stack.export_video("red", fn, start_frame=start, stop_frame=stop, channel_slice=corr_data)
+        stack.close()
+
+        # We take the unique frames, since plots are called a few times to "prepare" for rendering
+        np.testing.assert_equal(np.unique(frames), ref)
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         bit_depth=bit_depth,
     )
 
 
 def test_correlated_stack_deprecation(rgb_tiff_file):
     with pytest.warns(DeprecationWarning):
         cs = CorrelatedStack(str(rgb_tiff_file), align=True)
+        cs.close()
 
 
 @pytest.mark.parametrize("shape", [(3, 3), (5, 4, 3)])
 def test_image_stack(shape):
     fake_tiff = TiffStack(
         [MockTiffFile(data=[np.ones(shape)] * 6, times=make_frame_times(6))], align_requested=False
     )
@@ -147,14 +148,15 @@
     assert stack._stop_idx == 2
     assert stack._step == 3
 
 
 def test_stack_name_from_file(rgb_tiff_file):
     cs = ImageStack(str(rgb_tiff_file), align=True)
     assert cs.name == "rgb_single"
+    cs.close()
 
 
 @pytest.mark.parametrize("shape", [(3, 3), (5, 4, 3)])
 def test_slicing(shape):
     image = [np.random.poisson(10, size=shape) for _ in range(10)]
     start = _FIRST_TIMESTAMP + 100
     times = make_frame_times(10, step=int(0.8e9), start=start, frame_time=int(1e9))
@@ -515,14 +517,15 @@
                 err_msg=f"failed on {Path(filename).name}, align={align}, frame.data",
             )
             np.testing.assert_allclose(
                 cropped._get_frame(0).raw_data,
                 stack._get_frame(0).raw_data[25:50, 25:50],
                 err_msg=f"failed on {Path(filename).name}, align={align}, frame.raw_data",
             )
+            stack.close()
 
 
 def test_cropping_then_export(
     rgb_tiff_file, rgb_tiff_file_multi, gray_tiff_file, gray_tiff_file_multi
 ):
     from os import stat
 
@@ -534,14 +537,16 @@
         stack.export_tiff(savename)
         assert stat(savename).st_size > 0
 
         with tifffile.TiffFile(savename) as tif:
             assert tif.pages[0].tags["ImageWidth"].value == 180
             assert tif.pages[0].tags["ImageLength"].value == 60
 
+        stack.close()
+
 
 def test_get_image():
     # grayscale image - multiple frames
     data = [np.full((2, 2), j) for j in range(3)]
     times = make_frame_times(3)
 
     fake_tiff = TiffStack([MockTiffFile(data, times)], align_requested=False)
@@ -1222,22 +1227,24 @@
     ts_ranges = im.frame_timestamp_ranges(include_dead_time=include_dead_time)
     np.testing.assert_equal(ts_ranges, reference_data(ts_ranges, test_name="dead_time"))
 
     # Save it again
     tmpdir = tmpdir_factory.mktemp("legacy_exposures")
     tmp_file = tmpdir.join(f"include_dead_time={include_dead_time}.tiff")
     im.export_tiff(tmp_file)
+    im.close()
 
     # Test whether the round trip results in valid results
     im2 = ImageStack(tmp_file)
     ts_ranges2 = im2.frame_timestamp_ranges(include_dead_time=include_dead_time)
     np.testing.assert_equal(ts_ranges2, ts_ranges)
 
     # Verify that this migrated the file, and we are no longer using legacy reading for this
     assert im2._src._description._legacy_exposure is False
+    im2.close()
 
 
 def test_tiffstack_automatic_cleanup(gray_tiff_file_multi):
     im = TiffStack.from_file(gray_tiff_file_multi, False)
     weakref_file = weakref.ref(im._tiff_files[0])
     handle = im._tiff_files[0]._src.filehandle
     assert not handle.closed
@@ -1279,7 +1286,62 @@
 
     for current_stack in (im, derived_im):
         with pytest.raises(
             IOError,
             match=r"The file handle for this TiffStack \(gray_multi.tiff\) has already been closed.",
         ):
             current_stack.get_image("rgb")
+
+
+def test_two_color(gb_tiff_file_single, gb_tiff_file_multi, bg_tiff_file_single):
+    for filename, reference_image in (gb_tiff_file_single, gb_tiff_file_multi):
+        im = ImageStack(filename)
+
+        normalization = 1.0 / np.max(np.abs(reference_image))
+        np.testing.assert_allclose(
+            im.get_image() * normalization,
+            reference_image * normalization,
+            atol=0.05,
+        )
+        im.close()
+
+
+def test_invalid_order(bg_tiff_file_single):
+    with pytest.raises(
+        RuntimeError, match=re.escape("Wavelengths are not in descending order [525.0, 600.0]")
+    ):
+        ImageStack(bg_tiff_file_single[0])
+
+
+@pytest.mark.parametrize("align_export, align_load", [(False, False), (True, True), (False, True)])
+def test_two_color_write_again(
+    tmpdir_factory,
+    gb_tiff_file_single,
+    gb_tiff_file_multi,
+    bg_tiff_file_single,
+    align_export,
+    align_load,
+):
+    tmp_dir = tmpdir_factory.mktemp("two_color")
+    for filename, reference_image in (gb_tiff_file_single, gb_tiff_file_multi):
+        im = ImageStack(filename, align=align_export)
+        tmp_file = tmp_dir.join(f"export_{filename.basename}")
+        im.export_tiff(tmp_file)
+
+        # The tiff file we imported data was 2 channels.
+        assert im._src._tiff_files[0].pages[0].shape[-1] == 2
+        im.close()
+
+        # Reload source since we want to be able to test whether we can successfully align
+        im_read = ImageStack(tmp_file, align=align_load)
+        im = ImageStack(filename, align=align_load)
+        np.testing.assert_allclose(im_read.get_image(), im.get_image())
+
+        # Pylake always exports 3 channels, mapped to the correct RGB colors.
+        assert im_read._src._tiff_files[0].pages[0].shape[-1] == 3
+        assert im_read._src._description.json["Pylake"]["Channel mapping"] == {
+            "green": 0,
+            "blue": 1,
+        }
+
+        im.close()
+        im_read.close()
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/conftest.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/data/bead_kymo.npz` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/data/bead_kymo.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_export.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,13 +109,13 @@
     corr_data = Slice(
         Continuous(np.arange(1000), scan.start, int(1e9)), labels={"title": "title", "y": "y"}
     )
 
     scan.export_video(
         channel,
         f"{tmpdir}/{channel}_corr.gif",
-        start_frame=0,
-        stop_frame=0,
+        start_frame=None,
+        stop_frame=None,
         channel_slice=corr_data,
         vertical=vertical,
     )
     assert stat(f"{tmpdir}/{channel}_corr.gif").st_size > 0
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_downsampling.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_downsampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     np.testing.assert_allclose(kymo.start, ref.start)
     np.testing.assert_allclose(kymo.pixelsize_um, ref.metadata.pixelsize_um)
     np.testing.assert_allclose(kymo.line_time_seconds, ref.timestamps.line_time_seconds)
     np.testing.assert_equal(kymo.timestamps, ref.timestamps.data)
     assert kymo.contiguous
 
 
-def test_downsample_channel_downsampled_kymo(kymo_h5_file):
+def test_downsample_to_frames_downsampled_kymo(kymo_h5_file):
     f = lk.File.from_h5py(kymo_h5_file)
     kymo = f.kymos["tester"]
     kymo_ds = kymo.downsampled_by(position_factor=2)
 
     ds = f.force2x.downsampled_over(kymo_ds.line_timestamp_ranges(include_dead_time=False))
     np.testing.assert_allclose(ds.data[:2], 30)
     np.testing.assert_allclose(ds.data[2:], 10)
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_array.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_array.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_imagestack.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_imagestack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_slice_crop.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_slice_crop.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_transforms.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_kymo_transforms.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_plotting.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_plotting.py`

 * *Files 14% similar despite different names*

```diff
@@ -177,32 +177,58 @@
             image = plt.gca().get_images()[0]
             np.testing.assert_allclose(image.get_array(), ref_image)
             np.testing.assert_allclose(image.get_clim(), [lb_abs, ub_abs])
             plt.close(fig)
 
 
 @pytest.mark.parametrize(
-    "frame, vertical, channel",
+    "frame, vertical, channel, downsample",
     [
-        (0, False, "red"),
-        (0, False, "blue"),
-        (0, True, "red"),
-        (1, True, "red"),
+        (0, False, "red", True),
+        (0, False, "blue", True),
+        (0, True, "red", True),
+        (1, True, "red", True),
+        (0, False, "red", False),
     ],
 )
-def test_scan_plot_correlated(test_scans_multiframe, frame, vertical, channel):
+def test_scan_plot_correlated(test_scans_multiframe, frame, vertical, channel, downsample):
     import matplotlib as mpl
 
     scan, ref = test_scans_multiframe["fast Y slow X multiframe"]
     corr_data = Slice(
         Continuous(np.arange(1000), scan.start, int(1e9)), labels={"title": "title", "y": "y"}
     )
 
     image_axis = 0 if vertical else 1
-    scan.plot_correlated(channel=channel, channel_slice=corr_data, frame=frame, vertical=vertical)
+    scan.plot_correlated(
+        channel=channel,
+        channel_slice=corr_data,
+        frame=frame,
+        vertical=vertical,
+        downsample_to_frames=downsample,
+    )
     axes = plt.gcf().get_axes()
     imgs = [obj for obj in axes[image_axis].get_children() if isinstance(obj, mpl.image.AxesImage)]
 
     assert len(imgs) == 1
     np.testing.assert_allclose(imgs[0].get_array(), scan[frame].get_image(channel))
     assert axes[1 - image_axis].get_xlabel() == "Time [s]"
     assert axes[image_axis].get_title() == f"[frame {frame + 1} / 10]"
+
+    # Fetch raw data
+    lines = [o for o in axes[1 - image_axis].get_children() if isinstance(o, mpl.lines.Line2D)]
+    ref_time_vector, y = lines[0].get_data()
+
+    ts_ranges = scan.frame_timestamp_ranges()
+    if downsample:
+        ds = corr_data.downsampled_over(ts_ranges)
+        # Last sample is double because of step plot
+        np.testing.assert_allclose(np.hstack((ds.data, ds.data[-1])), y)
+        # Last frame does _not_ include dead time
+        seconds = (np.asarray(ts_ranges) - ts_ranges[0][0]) / 1e9
+        time_vector = np.hstack((seconds[:, 0], seconds[-1, 1]))
+        np.testing.assert_allclose(time_vector, ref_time_vector)
+    else:
+        slc = corr_data[ts_ranges[0][0] : ts_ranges[-1][-1]]
+        np.testing.assert_allclose(np.hstack((slc.data, slc.data[-1])), y)
+        time_vector = np.hstack((slc.seconds, slc.seconds[-1] + slc.seconds[-1] - slc.seconds[-2]))
+        np.testing.assert_allclose(time_vector, ref_time_vector)
```

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_point_scan.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_point_scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_scan.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_confocal/test_scan_slice_crop.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_confocal/test_scan_slice_crop.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_imaging_mixins.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_imaging_mixins.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_import_time.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_import_time.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_mixin.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_scalebar.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_scalebar.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_timeindex.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_timeindex.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/lumicks/pylake/tests/test_utilities.py` & `lumicks.pylake-1.5.0/lumicks/pylake/tests/test_utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 import numpy as np
 import pytest
 import matplotlib as mpl
 from numpy.testing import assert_array_equal
 
 from lumicks.pylake.detail.confocal import timestamp_mean
 from lumicks.pylake.detail.utilities import *
@@ -224,14 +226,58 @@
     for test, ref in zip(test_data, ref_data):
         np.testing.assert_allclose(test, ref)
 
     test_data = [[1, 2, 3], [1, 2, 3]]
     np.testing.assert_allclose(test_data, reference_data(test_data, test_name="non_ndarray_matrix"))
 
 
+@pytest.mark.parametrize("tst", [1, 2])
+def test_ref_dict_freezing(compare_to_reference_dict, reference_data, tst):
+    ref_dict = {"a": 5, "b": np.pi if tst == 1 else 1e-12}
+    test_dict = reference_data(ref_dict, test_name="dict", json=True)
+    np.testing.assert_allclose(list(test_dict.values()), list(ref_dict.values()))
+    compare_to_reference_dict(test_dict)
+
+
+def test_ref_dict_freezing_fail(request, compare_to_reference_dict):
+    if request.config.getoption("--update_reference_data"):
+        # Don't rewrite these as they intentionally fail
+        return
+
+    with pytest.raises(
+        RuntimeError,
+        match=re.escape(
+            "Differences with reference data detected.\n"
+            "a: 5 vs 5 (match)\n"
+            "b: 2 vs 3 (difference)"
+        ),
+    ):
+        compare_to_reference_dict({"a": 5, "b": 2})
+
+    with pytest.raises(
+        RuntimeError,
+        match=re.escape(
+            "Differences with reference data detected.\n"
+            "a: 5 vs 5 (match)\n"
+            "b: missing vs 3 (reference only)"
+        ),
+    ):
+        compare_to_reference_dict({"a": 5})
+
+    with pytest.raises(
+        RuntimeError,
+        match=re.escape(
+            "Differences with reference data detected.\n"
+            "a: 5 vs 5 (match)\n"
+            "b: 3 vs missing (test only)"
+        ),
+    ):
+        compare_to_reference_dict({"a": 5, "b": 3}, file_name="ref_dict_freezing_2")
+
+
 def test_cache_method():
     calls = 0
 
     def call():
         nonlocal calls
         calls += 1
```

### Comparing `lumicks.pylake-1.4.0/lumicks.pylake.egg-info/PKG-INFO` & `lumicks.pylake-1.5.0/lumicks.pylake.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: lumicks.pylake
-Version: 1.4.0
+Version: 1.5.0
 Summary: Bluelake data analysis tools
 Home-page: https://github.com/lumicks/pylake
 Author: Lumicks B.V.
 Author-email: devteam@lumicks.com
 License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: notebook
 License-File: license.md
 
 <img src="https://media.githubusercontent.com/media/lumicks/pylake/main/docs/logo_light.png" alt="logo" width="489px"/>
 
 [![DOI](https://zenodo.org/badge/133832492.svg)](https://zenodo.org/badge/latestdoi/133832492)
@@ -44,9 +43,7 @@
 
 If you wish to publish results produced with this package, please mention the package name and cite the Zenodo DOI for this project:
 
 [![DOI](https://zenodo.org/badge/133832492.svg)](https://zenodo.org/badge/latestdoi/133832492)
 
 You'll find a *"Cite as"* section at the bottom right of the Zenodo page. You can select a citation
 style from the dropdown menu or export the data in BibTeX and similar formats.
-
-
```

### Comparing `lumicks.pylake-1.4.0/lumicks.pylake.egg-info/SOURCES.txt` & `lumicks.pylake-1.5.0/lumicks.pylake.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,24 @@
 lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py
 lumicks/pylake/force_calibration/tests/test_simulations.py
 lumicks/pylake/force_calibration/tests/test_touchdown.py
 lumicks/pylake/force_calibration/tests/data/__init__.py
 lumicks/pylake/force_calibration/tests/data/reference_spectrum.npz
 lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py
 lumicks/pylake/force_calibration/tests/data/simulate_ideal.py
+lumicks/pylake/force_calibration/tests/ref_data/1BGJQSPSHIFNM841G0X0WP2UL.json
+lumicks/pylake/force_calibration/tests/ref_data/3H9KBT8A28K43BCYEHIE0JD4L.json
+lumicks/pylake/force_calibration/tests/ref_data/5OF2DCE6DXL0LGPCPCPHOA3TH.json
+lumicks/pylake/force_calibration/tests/ref_data/7IJO3KH5G90URX2B9RYTYQKPG.json
+lumicks/pylake/force_calibration/tests/ref_data/999SUSJ01D14ZSRH7M58HWXHV.json
+lumicks/pylake/force_calibration/tests/ref_data/9M9JZPD6GZ6UA62TR9OG5MDUJ.json
+lumicks/pylake/force_calibration/tests/ref_data/ALYF6CK1Y54466J549VJ1BSJM.json
+lumicks/pylake/force_calibration/tests/ref_data/BCF825GIR11ZFL6ZQKN4D7K21.json
+lumicks/pylake/force_calibration/tests/ref_data/E45ZBFK5MYVRD1J9N8ITG6EQ4.json
+lumicks/pylake/force_calibration/tests/ref_data/E6JD3GX1S6X68LXWJED5VFZOJ.json
 lumicks/pylake/kymotracker/__init__.py
 lumicks/pylake/kymotracker/kymotrack.py
 lumicks/pylake/kymotracker/kymotracker.py
 lumicks/pylake/kymotracker/stitching.py
 lumicks/pylake/kymotracker/detail/__init__.py
 lumicks/pylake/kymotracker/detail/denoising.py
 lumicks/pylake/kymotracker/detail/gaussian_mle.py
@@ -153,20 +163,20 @@
 lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb
 lumicks/pylake/kymotracker/tests/data/tracks_v0.csv
 lumicks/pylake/kymotracker/tests/data/tracks_v1.csv
 lumicks/pylake/kymotracker/tests/data/tracks_v2.csv
 lumicks/pylake/kymotracker/tests/data/tracks_v3.csv
 lumicks/pylake/kymotracker/tests/data/tracks_v4.csv
 lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz
-lumicks/pylake/kymotracker/tests/reference_data/denoising_basic/output_image_1d.npz
-lumicks/pylake/kymotracker/tests/reference_data/denoising_basic/output_image_2d.npz
-lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/1d_background.npz
-lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/1d_no_background.npz
-lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/2d_background.npz
-lumicks/pylake/kymotracker/tests/reference_data/denoising_regularized/2d_no_background.npz
+lumicks/pylake/kymotracker/tests/ref_data/1d_background.npz
+lumicks/pylake/kymotracker/tests/ref_data/1d_no_background.npz
+lumicks/pylake/kymotracker/tests/ref_data/2d_background.npz
+lumicks/pylake/kymotracker/tests/ref_data/2d_no_background.npz
+lumicks/pylake/kymotracker/tests/ref_data/output_image_1d.npz
+lumicks/pylake/kymotracker/tests/ref_data/output_image_2d.npz
 lumicks/pylake/kymotracker/tests/test_derived_quantities/__init__.py
 lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py
 lumicks/pylake/nb_widgets/__init__.py
 lumicks/pylake/nb_widgets/correlated_plot.py
 lumicks/pylake/nb_widgets/image_editing.py
 lumicks/pylake/nb_widgets/kymotracker_widgets.py
 lumicks/pylake/nb_widgets/range_selector.py
@@ -226,42 +236,48 @@
 lumicks/pylake/tests/data/__init__.py
 lumicks/pylake/tests/data/mock_confocal.py
 lumicks/pylake/tests/data/mock_fdcurve.py
 lumicks/pylake/tests/data/mock_file.py
 lumicks/pylake/tests/data/mock_json.py
 lumicks/pylake/tests/data/mock_widefield.py
 lumicks/pylake/tests/data/test_mock_confocal.py
-lumicks/pylake/tests/reference_data/freezing/dict[1].npz
-lumicks/pylake/tests/reference_data/freezing/dict[2].npz
-lumicks/pylake/tests/reference_data/freezing/forced_filename_1.npz
-lumicks/pylake/tests/reference_data/freezing/forced_filename_2.npz
-lumicks/pylake/tests/reference_data/freezing/freezing[1].npz
-lumicks/pylake/tests/reference_data/freezing/freezing[2].npz
-lumicks/pylake/tests/reference_data/freezing/mytest[1].npz
-lumicks/pylake/tests/reference_data/freezing/mytest[2].npz
-lumicks/pylake/tests/reference_data/freezing/non_ndarray_matrix[1].npz
-lumicks/pylake/tests/reference_data/freezing/non_ndarray_matrix[2].npz
-lumicks/pylake/tests/reference_data/freezing/ragged[1].npz
-lumicks/pylake/tests/reference_data/freezing/ragged[2].npz
+lumicks/pylake/tests/ref_data/2MOF2FD1NDYBUVE5V2UV5OE5.npz
+lumicks/pylake/tests/ref_data/49IRJMNKF3XEAQ6L2D38AFYC6.npz
+lumicks/pylake/tests/ref_data/4RRE8ZG26TWBKKOUPK6CPFBIX.npz
+lumicks/pylake/tests/ref_data/4TWTXTHAKH5N6BMWZI6KUMKK5.json
+lumicks/pylake/tests/ref_data/5CBUUDH5DX4QNMKTT2J2B96GL.npz
+lumicks/pylake/tests/ref_data/60TWXO09A93DLXSNN8B7QAIIT.json
+lumicks/pylake/tests/ref_data/60TWXO09A93DLXSNN8B7QAIIT.npz
+lumicks/pylake/tests/ref_data/852E6XRLZFHJN2FQRJQPONQVA.json
+lumicks/pylake/tests/ref_data/9WDSTMR98ABMBPK6VPBYU3WFF.npz
+lumicks/pylake/tests/ref_data/AELM9ISISBZJQ3AUKZIO6PZ7K.npz
+lumicks/pylake/tests/ref_data/C1Z88G669DGF5HS3RX4OED5YL.json
+lumicks/pylake/tests/ref_data/C1Z88G669DGF5HS3RX4OED5YL.npz
+lumicks/pylake/tests/ref_data/CMJN00XGRVG6SLMBMEJH8BKJK.npz
+lumicks/pylake/tests/ref_data/EC0P3CT7JCJYDCD86TWKIQNGY.npz
+lumicks/pylake/tests/ref_data/forced_filename_1.npz
+lumicks/pylake/tests/ref_data/forced_filename_2.npz
+lumicks/pylake/tests/ref_data/ref_dict_freezing_2.json
+lumicks/pylake/tests/ref_data/ref_dict_freezing_fail.json
 lumicks/pylake/tests/test_channels/__init__.py
 lumicks/pylake/tests/test_channels/conftest.py
 lumicks/pylake/tests/test_channels/test_arithmetic.py
 lumicks/pylake/tests/test_channels/test_channels.py
 lumicks/pylake/tests/test_file/__init__.py
 lumicks/pylake/tests/test_file/conftest.py
 lumicks/pylake/tests/test_file/test_file.py
 lumicks/pylake/tests/test_file/test_file_items.py
 lumicks/pylake/tests/test_imaging_camera/__init__.py
 lumicks/pylake/tests/test_imaging_camera/conftest.py
 lumicks/pylake/tests/test_imaging_camera/test_export.py
 lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py
 lumicks/pylake/tests/test_imaging_camera/test_image_stack.py
 lumicks/pylake/tests/test_imaging_camera/data/tiff_from_scan_v1_3_1.tiff
-lumicks/pylake/tests/test_imaging_camera/reference_data/legacy_exposure_handling/dead_time[False].npz
-lumicks/pylake/tests/test_imaging_camera/reference_data/legacy_exposure_handling/dead_time[True].npz
+lumicks/pylake/tests/test_imaging_camera/ref_data/21U0E1PWIF4T1V9BXHMY9P90F.npz
+lumicks/pylake/tests/test_imaging_camera/ref_data/56OBGN66YAHPLZDQ8KXKGCI2P.npz
 lumicks/pylake/tests/test_imaging_confocal/__init__.py
 lumicks/pylake/tests/test_imaging_confocal/conftest.py
 lumicks/pylake/tests/test_imaging_confocal/test_confocal.py
 lumicks/pylake/tests/test_imaging_confocal/test_export.py
 lumicks/pylake/tests/test_imaging_confocal/test_kymo.py
 lumicks/pylake/tests/test_imaging_confocal/test_kymo_downsampling.py
 lumicks/pylake/tests/test_imaging_confocal/test_kymo_from_array.py
```

### Comparing `lumicks.pylake-1.4.0/readme.md` & `lumicks.pylake-1.5.0/readme.md`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.4.0/setup.py` & `lumicks.pylake-1.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 
 from setuptools import PEP420PackageFinder, setup
 from setuptools.command.egg_info import manifest_maker
 
-if sys.version_info[:2] < (3, 9):
-    print("Python >= 3.9 is required.")
+if sys.version_info[:2] < (3, 10):
+    print("Python >= 3.10 is required.")
     sys.exit(-1)
 
 
 def about(package):
     ret = {}
     filename = os.path.join(os.path.dirname(__file__), package.replace(".", "/"), "__about__.py")
     with open(filename, "rb") as file:
@@ -35,43 +35,42 @@
     long_description_content_type="text/markdown",
     url=info["__url__"],
     license=info["__license__"],
     keywords="",
     author=info["__author__"],
     author_email=info["__email__"],
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Physics",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     packages=PEP420PackageFinder.find(include=["lumicks.*"]),
     include_package_data=True,
-    python_requires=">=3.9",
+    python_requires=">=3.10",
     install_requires=[
         "pytest>=3.5",
         "h5py>=3.4, <4",
         "numpy>=1.24, <2",  # 1.24 is needed for dtype in vstack/hstack (Dec 18th, 2022)
         "scipy>=1.9, <2",  # 1.9.0 needed for lazy imports (July 29th, 2022)
-        "matplotlib>=3.5",
+        "matplotlib>=3.8",
         "tifffile>=2022.7.28",
         "tabulate>=0.8.8, <0.9",
         "cachetools>=3.1",
         "deprecated>=1.2.8",
         "scikit-learn>=0.18.0",
         "scikit-image>=0.17.2",
         "tqdm>=4.27.0",  # 4.27.0 introduced tqdm.auto which auto-selects notebook or console
     ],
     extras_require={
         "notebook": [
-            # Notebook upper limit is a workaround for issues with IPython not being defined.
-            "notebook>=4.4.1,<7",
+            "notebook>=7",
             "ipywidgets>=7.0.0",
-            "jupyter_client<8",  # https://github.com/jupyter/notebook/issues/6748
-            "pyzmq<25",  # https://github.com/jupyter/notebook/issues/6748
+            "jupyter_client>=8",
+            "ipympl>=0.9.3",  # Needed for mpl compatibility (previous vers are only up to mpl 3.7)
         ],
     },
     zip_safe=False,
 )
```

