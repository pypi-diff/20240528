# Comparing `tmp/rubin-scheduler-1.1.1.tar.gz` & `tmp/rubin_scheduler-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubin-scheduler-1.1.1.tar", last modified: Thu Feb 29 22:44:21 2024, max compression
+gzip compressed data, was "rubin_scheduler-1.2.0.tar", last modified: Tue May 28 01:51:06 2024, max compression
```

## Comparing `rubin-scheduler-1.1.1.tar` & `rubin_scheduler-1.2.0.tar`

### file list

```diff
@@ -1,213 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.060300 rubin-scheduler-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.024299 rubin-scheduler-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.028299 rubin-scheduler-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/.github/workflows/build_docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/.github/workflows/cache.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/.github/workflows/rebase_checker.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/.github/workflows/test_and_build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    42986 2024-02-29 22:44:21.060300 rubin-scheduler-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.028299 rubin-scheduler-1.1.1/ci/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/ci/Jenkinsfile_rubin_scheduler.conda
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.036300 rubin-scheduler-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/archive.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/data-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/data-download.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/documenteer.toml
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-api-basis-functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-api-detailers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-api-example-scheduler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-api-features.rst
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-api-model-observatory.rst
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-api-schedulers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-api-sim-runner.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-api-surveys.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-api-utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-arch.rst
--rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-output-schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs-running.rst
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/fbs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/site-models-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/site-models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/skybrightness-pre-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/skybrightness-pre.rst
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/user-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/utils-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.036300 rubin-scheduler-1.1.1/rubin_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.036300 rubin-scheduler-1.1.1/rubin_scheduler/data/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/data/data_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/data/rs_download_sky.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/data/scheduler_download_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.036300 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.040300 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/basis_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/basis_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75501 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/basis_functions/basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19304 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/basis_functions/feasibility_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/basis_functions/mask_basis_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14714 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/basis_functions/rolling_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.040300 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/detailers/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/detailers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/detailers/detailer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/detailers/dither_detailer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/detailers/short_survey.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/detailers/vary_exptime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.040300 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/example/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53704 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/example/example_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.040300 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/features/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24588 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/features/conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27182 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/features/features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.040300 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/model_observatory/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/model_observatory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/model_observatory/generate_almanac.py
--rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/model_observatory/generate_altitudes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/model_observatory/jerk.py
--rw-r--r--   0 runner    (1001) docker     (127)    26971 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/model_observatory/kinem_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    25672 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/model_observatory/model_observatory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.040300 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23593 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/schedulers/core_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/schedulers/filter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/sim_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.044300 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23496 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/base_survey.py
--rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/dd_surveys.py
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/ddf_presched.py
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/desc_ddf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/field_survey.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/generate_ddf_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/long_gap_survey.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/plan_night_survey.py
--rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/pointings_survey.py
--rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/scripted_surveys.py
--rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/surveys.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/too_surveys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.044300 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/comcam_tessellate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/dithering.py
--rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/footprints.py
--rw-r--r--   0 runner    (1001) docker     (127)    40765 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/sky_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/tsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    34257 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.044300 rubin-scheduler-1.1.1/rubin_scheduler/sim_archive/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/sim_archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20392 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/sim_archive/sim_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.048300 rubin-scheduler-1.1.1/rubin_scheduler/site_models/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/almanac.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/cloud_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/cloud_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/downtime_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/generate_planets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/generate_sun_moon_pos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/generate_sunsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/read_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/scheduled_downtime_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/seeing_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/seeing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/unscheduled_downtime_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/site_models/wind_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.048300 rubin-scheduler-1.1.1/rubin_scheduler/skybrightness_pre/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/skybrightness_pre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/skybrightness_pre/dark_sky.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.048300 rubin-scheduler-1.1.1/rubin_scheduler/skybrightness_pre/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/skybrightness_pre/data/generate_dark_sky.py
--rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/skybrightness_pre/sky_model_pre.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.052300 rubin-scheduler-1.1.1/rubin_scheduler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/approx_coord_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/bearing.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/binned_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/camera_footprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/code_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    15879 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/coordinate_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/ddf_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/file_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/get_package_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/healpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    42963 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/htm_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/m5_flat_sed.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/mjd_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/projections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/riseset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/sampling_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/season_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/site.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/sys_eng_vals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/tree_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/rubin_scheduler/utils/zernike_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-29 22:44:20.000000 rubin-scheduler-1.1.1/rubin_scheduler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.060300 rubin-scheduler-1.1.1/rubin_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42986 2024-02-29 22:44:20.000000 rubin-scheduler-1.1.1/rubin_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-02-29 22:44:21.000000 rubin-scheduler-1.1.1/rubin_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 22:44:20.000000 rubin-scheduler-1.1.1/rubin_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-29 22:44:20.000000 rubin-scheduler-1.1.1/rubin_scheduler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-29 22:44:20.000000 rubin-scheduler-1.1.1/rubin_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-29 22:44:20.000000 rubin-scheduler-1.1.1/rubin_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 22:44:21.060300 rubin-scheduler-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.028299 rubin-scheduler-1.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.052300 rubin-scheduler-1.1.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/data/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.056300 rubin-scheduler-1.1.1/tests/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)    13079 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/scheduler/test_baseline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/scheduler/test_basisfuncs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/scheduler/test_comcam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/scheduler/test_constant_weather.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/scheduler/test_coresched.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/scheduler/test_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/scheduler/test_modelobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/scheduler/test_scalarbf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/scheduler/test_skyarea.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/scheduler/test_surveys.py
--rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/scheduler/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.056300 rubin-scheduler-1.1.1/tests/sim_archive/
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/sim_archive/test_sim_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.056300 rubin-scheduler-1.1.1/tests/site_models/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/site_models/test_almanac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/site_models/test_clouddata.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/site_models/test_cloudmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/site_models/test_downtimemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/site_models/test_scheduleddowntimedata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/site_models/test_seeingdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/site_models/test_seeingmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/site_models/test_unscheduleddowntimedata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.056300 rubin-scheduler-1.1.1/tests/skybrightness_pre/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/skybrightness_pre/test_dark_sky.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/skybrightness_pre/test_skypre.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.060300 rubin-scheduler-1.1.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_approx.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_camerafootprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_codeutilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    36226 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_coordinatetransformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_filemaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_healutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_kdtree.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_m5flatsed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 22:44:21.060300 rubin-scheduler-1.1.1/tests/utils/test_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_modules/dummy_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_riseset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13755 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_site.py
--rw-r--r--   0 runner    (1001) docker     (127)    31447 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_trixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-02-29 22:44:12.000000 rubin-scheduler-1.1.1/tests/utils/test_zernikemodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.776593 rubin_scheduler-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.744593 rubin_scheduler-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.748592 rubin_scheduler-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/.github/workflows/build_docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/.github/workflows/cache.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/.github/workflows/rebase_checker.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/.github/workflows/test_and_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    42986 2024-05-28 01:51:06.776593 rubin_scheduler-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.748592 rubin_scheduler-1.2.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/ci/Jenkinsfile_rubin_scheduler.conda
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.752592 rubin_scheduler-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/archive.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/data-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/data-download.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/documenteer.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-api-basis-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-api-detailers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-api-example-scheduler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-api-features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-api-model-observatory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-api-schedulers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-api-sim-runner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-api-surveys.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-api-utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-arch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21594 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-output-schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs-running.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/fbs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/site-models-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/site-models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/skybrightness-pre-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/skybrightness-pre.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/user-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/utils-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.752592 rubin_scheduler-1.2.0/rubin_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.752592 rubin_scheduler-1.2.0/rubin_scheduler/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/data/data_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/data/rs_download_sky.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/data/scheduler_download_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.752592 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.756592 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/basis_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/basis_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81850 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/basis_functions/basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19785 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/basis_functions/feasibility_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17878 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/basis_functions/mask_basis_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16272 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/basis_functions/rolling_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.756592 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/detailers/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/detailers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14535 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/detailers/detailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/detailers/dither_detailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/detailers/short_survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/detailers/vary_exptime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.756592 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54055 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/example/example_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.756592 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/features/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25421 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/features/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36904 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/features/features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.756592 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/model_observatory/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/model_observatory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/model_observatory/generate_almanac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/model_observatory/generate_altitudes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/model_observatory/jerk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27149 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/model_observatory/kinem_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28422 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/model_observatory/model_observatory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.756592 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23907 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/schedulers/core_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/schedulers/filter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/sim_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.760593 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23402 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/base_survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/dd_surveys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21535 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/ddf_presched.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/desc_ddf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/field_survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/generate_ddf_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/long_gap_survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/plan_night_survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/pointings_survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14290 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/scripted_surveys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/too_surveys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.760593 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/comcam_tessellate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/dithering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18859 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/footprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41504 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/sky_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35301 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.760593 rubin_scheduler-1.2.0/rubin_scheduler/sim_archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/sim_archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/sim_archive/prenight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20341 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/sim_archive/sim_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.764593 rubin_scheduler-1.2.0/rubin_scheduler/site_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/almanac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/cloud_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/cloud_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/downtime_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/generate_planets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/generate_sun_moon_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/generate_sunsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/read_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/scheduled_downtime_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/seeing_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/seeing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/unscheduled_downtime_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/site_models/wind_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.764593 rubin_scheduler-1.2.0/rubin_scheduler/skybrightness_pre/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/skybrightness_pre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/skybrightness_pre/dark_sky.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.764593 rubin_scheduler-1.2.0/rubin_scheduler/skybrightness_pre/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/skybrightness_pre/data/generate_dark_sky.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/skybrightness_pre/sky_model_pre.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.768592 rubin_scheduler-1.2.0/rubin_scheduler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/approx_coord_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/bearing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/binned_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/camera_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/code_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/coordinate_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/ddf_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/file_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/get_package_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/healpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42308 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/htm_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/m5_flat_sed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/mjd_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/projections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/riseset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/rotskypos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/sampling_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/season_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/sys_eng_vals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/rubin_scheduler/utils/zernike_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 01:51:06.000000 rubin_scheduler-1.2.0/rubin_scheduler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.772592 rubin_scheduler-1.2.0/rubin_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42986 2024-05-28 01:51:06.000000 rubin_scheduler-1.2.0/rubin_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-28 01:51:06.000000 rubin_scheduler-1.2.0/rubin_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:51:06.000000 rubin_scheduler-1.2.0/rubin_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-28 01:51:06.000000 rubin_scheduler-1.2.0/rubin_scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-28 01:51:06.000000 rubin_scheduler-1.2.0/rubin_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-28 01:51:06.000000 rubin_scheduler-1.2.0/rubin_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:51:06.776593 rubin_scheduler-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.744593 rubin_scheduler-1.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.768592 rubin_scheduler-1.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/data/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.768592 rubin_scheduler-1.2.0/tests/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/scheduler/test_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/scheduler/test_basisfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/scheduler/test_comcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/scheduler/test_constant_weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/scheduler/test_coresched.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/scheduler/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/scheduler/test_modelobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/scheduler/test_scalarbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/scheduler/test_skyarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/scheduler/test_surveys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15093 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/scheduler/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.768592 rubin_scheduler-1.2.0/tests/sim_archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/sim_archive/test_prenight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/sim_archive/test_sim_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.772592 rubin_scheduler-1.2.0/tests/site_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/site_models/test_almanac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/site_models/test_clouddata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/site_models/test_cloudmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/site_models/test_downtimemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/site_models/test_scheduleddowntimedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/site_models/test_seeingdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/site_models/test_seeingmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/site_models/test_unscheduleddowntimedata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.772592 rubin_scheduler-1.2.0/tests/skybrightness_pre/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/skybrightness_pre/test_dark_sky.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/skybrightness_pre/test_skypre.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.772592 rubin_scheduler-1.2.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_approx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_camerafootprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_codeutilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36226 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_coordinatetransformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_filemaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_healutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_m5flatsed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:51:06.772592 rubin_scheduler-1.2.0/tests/utils/test_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_modules/dummy_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_riseset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_rotsky.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13755 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31447 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_trixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-28 01:51:01.000000 rubin_scheduler-1.2.0/tests/utils/test_zernikemodule.py
```

### Comparing `rubin-scheduler-1.1.1/.github/workflows/build_docs.yaml` & `rubin_scheduler-1.2.0/.github/workflows/build_docs.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 jobs:
   build_sphinx_docs:
     name: Build and upload documentation
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
-      - uses: conda-incubator/setup-miniconda@v2
+      - uses: conda-incubator/setup-miniconda@v3
         with:
           auto-update-conda: true
           python-version: ${{ matrix.python-version }}
           miniforge-variant: Mambaforge
           channels: conda-forge,defaults
           use-mamba: true
           channel-priority: strict
@@ -38,15 +38,15 @@
         run: |
           echo `pwd`
           ls ${{ github.workspace }}
           python -m pip install . --no-deps
 
       - name: Access rubin-sim-data cache
         id: cache-rs
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         env:
           cache-name: cached-rubin-sim-data
         with:
           path: ~/rubin_sim_data
           key: ${{ env.cache-name }}
           restore-keys: |
             ${{ env.cache-name }}
```

### Comparing `rubin-scheduler-1.1.1/.github/workflows/cache.yaml` & `rubin_scheduler-1.2.0/.github/workflows/cache.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 jobs:
   make-cache:
     runs-on: macos-latest
     steps:
       - uses: actions/checkout@v4
 
-      - uses: conda-incubator/setup-miniconda@v2
+      - uses: conda-incubator/setup-miniconda@v3
         with:
           auto-update-conda: true
           python-version: ${{ matrix.python-version }}
           miniforge-variant: Mambaforge
           channels: conda-forge,defaults
           use-mamba: true
           channel-priority: strict
@@ -34,15 +34,15 @@
         run: |
           echo `pwd`
           ls ${{ github.workspace }}
           python -m pip install .       
 
       - name: Access rubin-sim-data cache
         id: cache-rs
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         env:
           cache-name: cached-rubin-sim-data
         with:
           path: ~/rubin_sim_data
           key: ${{ env.cache-name }}
           restore-keys: |
             ${{ env.cache-name }}
```

### Comparing `rubin-scheduler-1.1.1/.github/workflows/test_and_build.yaml` & `rubin_scheduler-1.2.0/.github/workflows/test_and_build.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest", "macos-latest"]
         python-version: ["3.11"]
     steps:
       - uses: actions/checkout@v4
-      - uses: conda-incubator/setup-miniconda@v2
+      - uses: conda-incubator/setup-miniconda@v3
         with:
           auto-update-conda: true
           python-version: ${{ matrix.python-version }}
           miniforge-variant: Mambaforge
           channels: conda-forge,defaults
           use-mamba: true
           channel-priority: strict
@@ -46,15 +46,15 @@
         run: |
           echo `pwd`
           ls ${{ github.workspace }}
           python -m pip install -e . --no-deps
 
       - name: Access rubin-sim-data cache
         id: cache-rs
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         env:
           cache-name: cached-rubin-sim-data
         with:
           path: ~/rubin_sim_data
           key: ${{ env.cache-name }}
           restore-keys: |
             ${{ env.cache-name }}
```

### Comparing `rubin-scheduler-1.1.1/.gitignore` & `rubin_scheduler-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/LICENSE` & `rubin_scheduler-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/PKG-INFO` & `rubin_scheduler-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubin-scheduler
-Version: 1.1.1
+Version: 1.2.0
 Summary: Scheduling algorithms for Vera C. Rubin Observatory's Legacy Survey of Space and Time (LSST).
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `rubin-scheduler-1.1.1/README.md` & `rubin_scheduler-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/docs/Makefile` & `rubin_scheduler-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/docs/archive.rst` & `rubin_scheduler-1.2.0/docs/archive.rst`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/docs/data-download.rst` & `rubin_scheduler-1.2.0/docs/data-download.rst`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/docs/fbs-arch.rst` & `rubin_scheduler-1.2.0/docs/fbs-arch.rst`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/docs/fbs-output-schema.rst` & `rubin_scheduler-1.2.0/docs/fbs-output-schema.rst`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 +-----------------------+-------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | observationStartLST   | degrees           | the Local Sidereal Time at the start of the observation                                                                                                                                           |
 +-----------------------+-------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | observationStartMJD   | days              | Modified Julian Date at the start of the observation                                                                                                                                              |
 +-----------------------+-------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | paraAngle             | degrees           | Paralactic angle of the observation                                                                                                                                                               |
 +-----------------------+-------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
+| psudoParaAngle        | degrees           | Psudo-paralactic angle of the observation, see https://smtn-019.lsst.io/v/DM-44258/index.html                                                                                                                                                              |
++-----------------------+-------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | proposalId            | int               | deprecated                                                                                                                                                                                        |
 +-----------------------+-------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | rotSkyPos             | degrees           | The orientation of the sky in the focal plane measured as the angle between North on the sky and the "up" direction in the focal plane.                                                           |
 +-----------------------+-------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | rotTelPos             | degrees           | The physical angle of the rotator with respect to the mount. rotSkyPos = rotTelPos - ParallacticAngle                                                                                             |
 +-----------------------+-------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | seeingFwhm500         | arcseconds        | The full-width at half maximum of the PSF at 500 nm. (XXX-unsure if this is at zenith or at the pointing)                                                                                         |
```

### Comparing `rubin-scheduler-1.1.1/docs/fbs-running.rst` & `rubin_scheduler-1.2.0/docs/fbs-running.rst`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/docs/installation.rst` & `rubin_scheduler-1.2.0/docs/installation.rst`

 * *Files 10% similar despite different names*

```diff
@@ -31,36 +31,18 @@
 
 First, clone the `rubin_scheduler <https://github.com/lsst/rubin_scheduler>`_ repository:
 
 ::
 
  git clone git@github.com:lsst/rubin_scheduler.git
  cd rubin_scheduler
-
-
-Create a conda environment for it:
-
-::
-
  conda create --channel conda-forge --name rubin_scheduler --file requirements.txt python=3.11
-
-
-If you want to run tests, install the test requirements as well:
-
-::
-
  conda activate rubin_scheduler
- conda install -c conda-forge --file=test-requirements.txt
-
-
-Install the ``rubin_scheduler`` project into this environment (from the rubin_scheduler directory):
-
-::
-
- pip install -e .
+ conda install -c conda-forge --file=test-requirements.txt # Optional for running unit tests
+ pip install -e . --no-deps
 
 Please note that following installation,
 additional data must be downloaded to use the software,
 following the instructions at
 :ref:`Data Download<data-download>`.
```

### Comparing `rubin-scheduler-1.1.1/docs/introduction.rst` & `rubin_scheduler-1.2.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/docs/site-models.rst` & `rubin_scheduler-1.2.0/docs/site-models.rst`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/docs/skybrightness-pre.rst` & `rubin_scheduler-1.2.0/docs/skybrightness-pre.rst`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/pyproject.toml` & `rubin_scheduler-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,15 @@
   "documenteer[guide]",
 ]
 
 [project.scripts]
 scheduler_download_data = "rubin_scheduler.data.scheduler_download_data:scheduler_download_data"
 rs_download_sky = "rubin_scheduler.data.rs_download_sky:rs_download_sky"
 archive_sim = "rubin_scheduler.sim_archive:make_sim_archive_cli"
+prenight_sim = "rubin_scheduler.sim_archive:prenight_sim_cli"
 
 
 [tool.setuptools.dynamic]
 version = { attr = "setuptools_scm.get_version" }
 
 [tool.setuptools.packages.find]
 where = [ "" ]
@@ -120,12 +121,12 @@
 ]
 target-version = "py311"
 extend-select = [
     "RUF100", # Warn about unused noqa
 ]
 
 [tool.ruff.pycodestyle]
-max-doc-length = 110
+max-doc-length = 79
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/data/rs_download_sky.py` & `rubin_scheduler-1.2.0/rubin_scheduler/data/rs_download_sky.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/data/scheduler_download_data.py` & `rubin_scheduler-1.2.0/rubin_scheduler/data/scheduler_download_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,19 +108,21 @@
     """Download external data blobs
 
     Parameters
     ----------
     file_dict : `dict`
         A dict with keys of directory names and values of remote filenames.
     dirs : `list` [`str`]
-        List of directories to download. Default (None) assumes they are in file_dict
+        List of directories to download. Default (None) assumes they are
+        in file_dict
     versions : `bool`
         If True, print the versions currently on disk. Default False.
     update : `bool`
-        If True, update versions on disk to match expected 'current'. Default False.
+        If True, update versions on disk to match expected 'current'.
+        Default False.
     force : `bool`
         If True, replace versions on disk with new download. Default False.
     url_base : `str`
         The URL to use, default to DEFAULT_DATA_URL
     tdqm_disable : `bool`
         If True, disable the tdqm progress bar. Default False.
     """
@@ -158,17 +160,17 @@
             print(f"{','.join([k for k in mismatch_dict])} are not matching.")
             return 1
 
     version_file = os.path.join(data_dir, "versions.txt")
 
     # See if base URL is alive
     url_base = url_base
+    fail_message = f"Could not connect to {url_base}. Check site is up?"
     try:
         r = requests.get(url_base)
-        fail_message = f"Could not connect to {url_base} or {url_base}. Check sites are up?"
     except ConnectionError:
         print(fail_message)
         exit()
     if r.status_code != requests.codes.ok:
         print(fail_message)
         exit()
 
@@ -200,15 +202,15 @@
             print("Downloading file: %s" % url)
             # Stream and write in chunks (avoid large memory usage)
             r = requests.get(url, stream=True)
             file_size = int(r.headers.get("Content-Length", 0))
             if file_size < 245:
                 warnings.warn(f"{url} file size unexpectedly small.")
             # Download this size chunk at a time; reasonable guess
-            block_size = 512 * 512
+            block_size = 512 * 512 * 10
             progress_bar = tqdm(total=file_size, unit="iB", unit_scale=True, disable=tdqm_disable)
             print(f"Writing to {os.path.join(data_dir, filename)}")
             with open(os.path.join(data_dir, filename), "wb") as f:
                 for chunk in r.iter_content(chunk_size=block_size):
                     progress_bar.update(len(chunk))
                     f.write(chunk)
             progress_bar.close()
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/basis_functions/basis_functions.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/basis_functions/basis_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     "BaseBasisFunction",
     "HealpixLimitedBasisFunctionMixin",
     "ConstantBasisFunction",
     "SimpleArrayBasisFunction",
     "DelayStartBasisFunction",
     "TargetMapBasisFunction",
     "AvoidLongGapsBasisFunction",
-    "AvoidFastRevists",
+    "AvoidFastRevisits",
     "VisitRepeatBasisFunction",
     "M5DiffBasisFunction",
     "M5DiffAtHpixBasisFunction",
     "StrictFilterBasisFunction",
     "GoalStrictFilterBasisFunction",
     "FilterChangeBasisFunction",
     "SlewtimeBasisFunction",
@@ -48,40 +48,53 @@
 
 import healpy as hp
 import numpy as np
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 
 from rubin_scheduler.scheduler import features, utils
-from rubin_scheduler.scheduler.utils import IntRounded
+from rubin_scheduler.scheduler.utils import IntRounded, get_current_footprint
 from rubin_scheduler.skybrightness_pre import dark_m5
-from rubin_scheduler.utils import _hpid2_ra_dec
+from rubin_scheduler.utils import _hpid2_ra_dec, survey_start_mjd
+
+
+def send_unused_deprecation_warning(name):
+    message = (
+        f"The basis function {name} is not in use by the current "
+        "baseline scheduler and may be deprecated shortly. "
+        "Please contact the rubin_scheduler maintainers if "
+        "this is in use elsewhere."
+    )
+    warnings.warn(message, FutureWarning)
 
 
 class BaseBasisFunction:
-    """Class that takes features and computes a reward function when called."""
+    """Class that takes features and computes a reward function when
+    called."""
 
     def __init__(self, nside=None, filtername=None, **kwargs):
         # Set if basis function needs to be recalculated if there is a new
         # observation
         self.update_on_newobs = True
-        # Set if basis function needs to be recalculated if conditions change
+        # Set if basis function needs to be recalculated if conditions
+        # change
         self.update_on_mjd = True
         # Dict to hold all the features we want to track
         self.survey_features = {}
-        # Keep track of the last time the basis function was called. If mjd
-        # doesn't change, use cached value
+        # Keep track of the last time the basis function was called.
+        # If mjd doesn't change, use cached value
         self.mjd_last = None
         self.value = 0
-        # list the attributes to compare to check if basis functions are equal.
+        # list the attributes to compare to check if basis functions
+        # are equal.
         self.attrs_to_compare = []
         # Do we need to recalculate the basis function
         self.recalc = True
-        # Basis functions don't technically all need an nside, but so many do
-        #  might as well set it here
+        # Basis functions don't technically all need an nside, but so
+        # many do might as well set it here
         if nside is None:
             self.nside = utils.set_default_nside()
         else:
             self.nside = nside
 
         self.filtername = filtername
 
@@ -110,24 +123,25 @@
     def add_observation(self, observation, indx=None):
         """
         Parameters
         ----------
         observation : `np.array`
             An array with information about the input observation
         indx : `np.array`
-            The indices of the healpix map that the observation overlaps with
+            The indices of the healpix map that the observation overlaps
+            with
         """
         for feature in self.survey_features:
             self.survey_features[feature].add_observation(observation, indx=indx)
         if self.update_on_newobs:
             self.recalc = True
 
     def check_feasibility(self, conditions):
-        """If there is logic to decide if something is feasible (e.g., only if
-        moon is down), it can be calculated here.
+        """If there is logic to decide if something is feasible
+        (e.g., only if  moon is down), it can be calculated here.
 
         Helps prevent full __call__ from being called more than needed.
         """
         return True
 
     def _calc_value(self, conditions, **kwargs):
         self.value = 0
@@ -164,15 +178,16 @@
 
     def label(self):
         """Create a label for this basis function.
 
         Returns
         -------
         label : `str`
-            A string suitable for labeling the basis function in a plot or table.
+            A string suitable for labeling the basis function in a
+            plot or table.
         """
         label = self.__class__.__name__.replace("BasisFunction", "")
 
         if self.filtername is not None:
             label += f" {self.filtername}"
 
         label += f" @{id(self)}"
@@ -194,15 +209,16 @@
         ----------
         conditions : `rubin_scheduler.scheduler.features.Conditions`
             The conditions for which to test feasibility.
 
         Returns
         -------
         feasibility : `bool`
-            True if the current set of conditions is feasible, False otherwise.
+            True if the current set of conditions is feasible, False
+            otherwise.
         """
 
         if super().check_feasibility(conditions):
             if self.recalc or (self.update_on_mjd and conditions.mjd != self.mjd_last):
                 value = self._calc_value(conditions)
             else:
                 value = super().value
@@ -241,15 +257,21 @@
 
     def _calc_value(self, conditions, **kwargs):
         self.value = self.assigned_value
         return self.value
 
 
 class DelayStartBasisFunction(BaseBasisFunction):
-    """Force things to not run before a given night"""
+    """Force things to not run before a given night.
+
+    Parameters
+    ----------
+    nights_delay : `float`, optional
+        Return False until conditions.night >= nights_delay.
+    """
 
     def __init__(self, nights_delay=365.25 * 5):
         super().__init__()
         self.nights_delay = nights_delay
 
     def check_feasibility(self, conditions):
         result = True
@@ -290,16 +312,16 @@
         Should be a HEALpix map. Values of 0 or np.nan will be ignored.
     n_obs : `int` (3)
         The number of observations to demand
     season : `float` (300)
         The amount of time to allow pass before marking a region as "behind".
         Default 365.25 (days).
     season_start_hour : `float` (-2)
-        When to start the season relative to RA 180 degrees away from the sun
-        (hours)
+        When to start the season relative to RA 180 degrees away
+        from the sun (hours)
     season_end_hour : `float` (2)
         When to consider a season ending, the RA relative to the sun + 180
         degrees. (hours)
     night_max : float (365)
         Set value to zero after night_max is reached (days)
     """
 
@@ -353,83 +375,119 @@
         # mask off anything outside the footprint
         result[self.out_footprint] = 0
 
         return result
 
 
 class NGoodSeeingBasisFunction(BaseBasisFunction):
-    """Try to get N "good seeing" images each observing season
+    """Try to get N "good seeing" images each observing season.
 
     Parameters
     ----------
-    seeing_fwhm_max : `float` (0.8)
+    filtername : `str`
+        Bandpass in which to count images. Default r.
+    nside : `int`
+        The nside of the map for the basis function. Should match
+        survey and scheduler nside.
+        Default None uses `set_default_nside`.
+    seeing_fwhm_max : `float`
         Value to consider as "good" threshold (arcsec).
-    m5_penalty_max : `float` (0.5)
-        The maximum depth loss that is considered acceptable (magnitudes)
-    n_obs_desired : `int` (3)
+        Default of 0.8 arcseconds.
+    m5_penalty_max : `float`
+        The maximum depth loss that is considered acceptable (magnitudes),
+        compared to the dark-sky map in this filter.
+        Default 0.5 magnitudes.
+    n_obs_desired : `int`
         Number of good seeing observations to collect per season.
-    mjd_start : float (1)
-        The starting MJD.
-    footprint : `np.array` (None)
+        Default 3.
+    mjd_start : `float`
+        The starting MJD of the survey.
+        Default None uses `rubin_scheduler.utils.survey_start_mjd()`.
+    footprint : `np.array`, (N,)
         Only use area where footprint > 0. Should be a HEALpix map.
+        Default None calls `get_current_footprint()`.
     """
 
     def __init__(
         self,
         filtername="r",
         nside=None,
         seeing_fwhm_max=0.8,
         m5_penalty_max=0.5,
         n_obs_desired=3,
+        mjd_start=None,
         footprint=None,
-        mjd_start=1,
     ):
         super().__init__(nside=nside, filtername=filtername)
         self.seeing_fwhm_max = seeing_fwhm_max
         self.m5_penalty_max = m5_penalty_max
         self.n_obs_desired = n_obs_desired
-
+        if mjd_start is None:
+            mjd_start = survey_start_mjd()
+        self.mjd_start = mjd_start
         self.survey_features["N_good_seeing"] = features.NObservationsCurrentSeason(
-            filtername=filtername,
-            mjd_start=mjd_start,
-            seeing_fwhm_max=seeing_fwhm_max,
-            m5_penalty_max=m5_penalty_max,
-            nside=nside,
+            filtername=self.filtername,
+            mjd_start=self.mjd_start,
+            seeing_fwhm_max=self.seeing_fwhm_max,
+            m5_penalty_max=self.m5_penalty_max,
+            nside=self.nside,
         )
+        # Set footprint to current survey footprint class if undefined.
+        if footprint is None:
+            footprints, labels = get_current_footprint(self.nside)
+            footprint = footprints[self.filtername]
+        self.footprint = footprint
         self.result = np.zeros(hp.nside2npix(self.nside))
         self.dark_map = None
-        self.footprint = footprint
 
     def _calc_value(self, conditions, indx=None):
         if self.filtername is not None:
             if self.dark_map is None:
                 self.dark_map = dark_m5(
                     conditions.dec, self.filtername, conditions.site.latitude_rad, fiducial_FWHMEff=0.7
                 )
-        result = 0
-        # Need to update the feature to the current season
+        # Return the same kind of array (not float) regardless
+        # of result
+        result = self.result.copy()
+        # Update the feature to the current time.
         self.survey_features["N_good_seeing"].season_update(conditions=conditions)
 
         m5_penalty = self.dark_map - conditions.m5_depth[self.filtername]
         potential_pixels = np.where(
             (m5_penalty <= self.m5_penalty_max)
             & (conditions.fwhm_eff[self.filtername] <= self.seeing_fwhm_max)
             & (self.survey_features["N_good_seeing"].feature < self.n_obs_desired)
             & (self.footprint > 0)
         )[0]
 
-        if np.size(potential_pixels) > 0:
-            result = self.result.copy()
-            result[potential_pixels] = 1
+        result[potential_pixels] = 1
         return result
 
 
 class AvoidLongGapsBasisFunction(BaseBasisFunction):
     """Boost the reward on parts of the survey that haven't been
     observed for a while.
+
+    Parameters
+    ----------
+    filtername : `str`, optional
+        The filter to consider when tracking visits.
+    nside : `int`, optional
+        The nside to use for the basis function.
+        Default None uses `set_default_nside()`.
+    footprint : `np.ndarray`, (N,)
+        The footprint to consider when tracking visits.
+        Default None uses `get_current_footprint()`.
+    min_gap : `float`, optional
+        The minimum gap of time before boosting (in days).
+    max_gap : `float`, optional
+        The maximum gap of time before stopping boosting (in days).
+    ha_limit : `float, optional
+        Only boost visits at parts of the sky with HA < ha_limit
+        (in hours).
     """
 
     def __init__(
         self,
         filtername=None,
         nside=None,
         footprint=None,
@@ -437,19 +495,23 @@
         max_gap=40.0,
         ha_limit=3.5,
     ):
         super(AvoidLongGapsBasisFunction, self).__init__(nside=nside, filtername=filtername)
         self.min_gap = min_gap
         self.max_gap = max_gap
         self.filtername = filtername
+        if footprint is None:
+            footprints, labels = get_current_footprint(self.nside)
+            footprint = footprints[self.filtername]
         self.footprint = footprint
         self.ha_limit = 2.0 * np.pi * ha_limit / 24.0  # To radians
         self.survey_features = {}
-        self.survey_features["last_observed"] = features.Last_observed(nside=nside, filtername=filtername)
+        self.survey_features["last_observed"] = features.LastObserved(nside=nside, filtername=filtername)
         self.result = np.zeros(hp.nside2npix(self.nside))
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def _calc_value(self, conditions, indx=None):
         result = self.result.copy()
 
         gap = conditions.mjd - self.survey_features["last_observed"].feature
         in_range = np.where((gap > self.min_gap) & (gap < self.max_gap) & (self.footprint > 0))
         result[in_range] = 1
@@ -460,37 +522,41 @@
         ]
         result[out_ha] = 0
 
         return result
 
 
 class TargetMapBasisFunction(BaseBasisFunction):
-    """Basis function that tracks number of observations and tries to match a
-    specified spatial distribution
+    """Basis function that tracks number of observations and tries
+    to match a specified spatial distribution.
+
+    In general, this is deprecated in favor of
+    `FootprintBasisFunction`.
 
     Parameters
     ----------
     filtername: `str` ('r')
         The name of the filter for this target map.
     nside: `int` (default_nside)
         The healpix resolution.
     target_map : `np.array` (None)
-        A healpix map showing the ratio of observations desired for all points
-        on the sky
+        A healpix map showing the ratio of observations desired
+        for all points on the sky
     norm_factor : `float` (0.00010519)
         for converting target map to number of observations.
         Should be the area of the camera divided by the area of a healpixel
         divided by the sum of all your goal maps.
         Default value assumes LSST foV has 1.75 degree radius and the
         standard goal maps.
-        If using multiple filters, see rubin_scheduler.utils.calc_norm_factor
+        If using multiple filters, see
+        rubin_scheduler.utils.calc_norm_factor
         for a utility that computes norm_factor.
     out_of_bounds_val : `float` (-10.)
-        Reward value to give regions where there are no observations requested
-        (unitless).
+        Reward value to give regions where there are no
+        observations requested (unitless).
     """
 
     def __init__(
         self,
         filtername="r",
         nside=None,
         target_map=None,
@@ -507,33 +573,29 @@
 
         self.survey_features = {}
         # Map of the number of observations in filter
         self.survey_features["n_obs"] = features.NObservations(filtername=filtername, nside=self.nside)
         # Count of all the observations
         self.survey_features["n_obs_count_all"] = features.NObsCount(filtername=None)
         if target_map is None:
-            self.target_map = utils.generate_goal_map(filtername=filtername, nside=self.nside)
+            target_maps, labels = utils.get_current_footprint(self.nside)
+            self.target_map = target_maps[filtername]
         else:
             self.target_map = target_map
         self.out_of_bounds_area = np.where(self.target_map == 0)[0]
         self.out_of_bounds_val = out_of_bounds_val
         self.result = np.zeros(hp.nside2npix(self.nside), dtype=float)
         self.all_indx = np.arange(self.result.size)
+        # As of 4/2024,
+        # this is used in the ts_fbs_utils maintel "anytime" test survey.
+        # It is also used in unit tests.
+        # send_unused_deprecation_warning(self.__class__.__name__)
+        # In general, it is deprecated in favor of FootprintBasisFunction
 
     def _calc_value(self, conditions, indx=None):
-        """
-        Parameters
-        ----------
-        indx : `list` (None)
-            Index values to compute, if None, full map is computed
-
-        Returns
-        -------
-        Healpix reward map
-        """
         result = self.result.copy()
         if indx is None:
             indx = self.all_indx
 
         # Find out how many observations we want now at those points
         goal_n = self.target_map[indx] * self.survey_features["n_obs_count_all"].feature * self.norm_factor
 
@@ -551,62 +613,52 @@
     else:
         if az_rel_moon > np.pi:
             az_rel_moon = 2.0 * np.pi - az_rel_moon
     return az_rel_moon
 
 
 class NObsHighAmBasisFunction(BaseBasisFunction):
-    """Reward only reward/count observations at high airmass"""
+    """Reward only reward/count observations at high airmass."""
 
     def __init__(
         self,
         nside=None,
         filtername="r",
         footprint=None,
         n_obs=3,
         season=300.0,
         am_limits=[1.5, 2.2],
         out_of_bounds_val=np.nan,
     ):
         super(NObsHighAmBasisFunction, self).__init__(nside=nside, filtername=filtername)
+        if footprint is None:
+            footprints, labels = get_current_footprint(self.nside)
+            footprint = footprints[self.filtername]
         self.footprint = footprint
         self.out_footprint = np.where((footprint == 0) | np.isnan(footprint))
         self.am_limits = am_limits
         self.season = season
         self.survey_features["last_n_mjds"] = features.Last_n_obs_times(
             nside=nside, filtername=filtername, n_obs=n_obs
         )
 
         self.result = np.zeros(hp.nside2npix(self.nside), dtype=float) + out_of_bounds_val
         self.out_of_bounds_val = out_of_bounds_val
 
     def add_observation(self, observation, indx=None):
-        """
-        Parameters
-        ----------
-        observation : `np.array`
-            An array with information about the input observation
-        indx : `np.array`
-            The indices of the healpix map that the observation overlaps with
-        """
-
         # Only count the observations if they are at the airmass limits
         if (observation["airmass"] > np.min(self.am_limits)) & (
             observation["airmass"] < np.max(self.am_limits)
         ):
             for feature in self.survey_features:
                 self.survey_features[feature].add_observation(observation, indx=indx)
             if self.update_on_newobs:
                 self.recalc = True
 
     def check_feasibility(self, conditions):
-        """If there is logic to decide if something is feasible
-        (e.g., only if moon is down), it can be calculated here.
-        Helps prevent full __call__ from being called more than needed.
-        """
         result = True
         reward = self._calc_value(conditions)
         # If there are no non-NaN values, we're not feasible now
         if True not in np.isfinite(reward):
             result = False
 
         return result
@@ -650,30 +702,30 @@
 
 
 class CadenceInSeasonBasisFunction(BaseBasisFunction):
     """Drive observations at least every N days in a given area
 
     Parameters
     ----------
-    drive_map : np.array
+    drive_map : `np.ndarray`, (N,)
         A HEALpix map with values of 1 where the cadence should be driven.
     filtername : `str`
-        The filters that can count
-    season_span : `float` (2.5)
-        How long to consider a spot "in_season" (hours)
-    cadence : `float` (2.5)
-        How long to wait before activating the basis function (days)
+        The filters that can count.
+    season_span : `float`
+        How long to consider a spot "in_season" (hours).
+    cadence : `float`
+        How long to wait before activating the basis function (days).
     """
 
     def __init__(self, drive_map, filtername="griz", season_span=2.5, cadence=2.5, nside=None):
         super(CadenceInSeasonBasisFunction, self).__init__(nside=nside, filtername=filtername)
         self.drive_map = drive_map
         self.season_span = season_span / 12.0 * np.pi  # To radians
         self.cadence = cadence
-        self.survey_features["last_observed"] = features.Last_observed(nside=nside, filtername=filtername)
+        self.survey_features["last_observed"] = features.LastObserved(nside=nside, filtername=filtername)
         self.result = np.zeros(hp.nside2npix(self.nside), dtype=float)
 
     def _calc_value(self, conditions, indx=None):
         result = self.result.copy()
         ra_mid_season = (conditions.sunRA + np.pi) % (2.0 * np.pi)
 
         angle_to_mid_season = np.abs(conditions.ra - ra_mid_season)
@@ -689,96 +741,129 @@
         )
         result[active_pix] = 1.0
 
         return result
 
 
 class SeasonCoverageBasisFunction(BaseBasisFunction):
-    """Basis function to encourage N observations per observing season
+    """Basis function to encourage N observations per observing season.
 
     Parameters
     ----------
-    footprint : healpix map (None)
-        The footprint where one should demand coverage every season
-    n_per_season : `int` (3)
-        The number of observations to attempt to gather every season
-    offset : healpix map
-        The offset to apply when computing the current season over the sky.
-        rubin_scheduler.utils.create_season_offset is helpful for making this
-    season_frac_start : `float` (0.5)
-        Only start trying to gather observations after a season is fractionally this far over.
+    filtername : `str`, optional
+        Count observations in this filter. Default 'r'.
+    nside : `int`, optional
+        Nside for the healpix map to use for the feature.
+        This should match the nside of the survey and scheduler.
+    footprint : `np.array` (N,), optional
+        Healpix map of the footprint where one should demand coverage
+        every season. Default None will call `get_current_footprint()`.
+    n_per_season : `int`, optional
+        The number of observations to attempt to gather every season.
+        Default of 3 is suitable for first year template building.
+    mjd_start : `float`, optional
+        The mjd of the start of the survey (days).
+        Default None uses `rubin_scheduler.utils.survey_start_mjd()`.
+    season_frac_start : `float`
+        Only start trying to gather observations after a season
+        is fractionally this far along.
+        Seasons start when the apparent position of sun is at the RA of
+        the pixel (0) and finish when the sun returns again to this RA.
+        The default of 0.5 means that the basis function will not
+        start returning values until the RA reaches the peak of its season.
     """
 
     def __init__(
         self,
         filtername="r",
         nside=None,
         footprint=None,
         n_per_season=3,
-        offset=None,
+        mjd_start=None,
         season_frac_start=0.5,
     ):
-        super(SeasonCoverageBasisFunction, self).__init__(nside=nside, filtername=filtername)
+        super().__init__(nside=nside, filtername=filtername)
 
-        self.n_per_season = n_per_season
+        if footprint is None:
+            footprints, labels = get_current_footprint(self.nside)
+            footprint = footprints[self.filtername]
         self.footprint = footprint
+        # Calculate the RA values for each spot on the footprint
+        ra, dec = _hpid2_ra_dec(nside, np.arange(hp.nside2npix(nside)))
+        self.ra_deg = np.degrees(ra)
+
+        self.n_per_season = n_per_season
+        if mjd_start is None:
+            mjd_start = survey_start_mjd()
+        self.mjd_start = mjd_start
+        self.season_frac_start = season_frac_start
+        # Track how many observations have been taken at each RA/Dec
+        # in the current observing season (for that point on the sky).
         self.survey_features["n_obs_season"] = features.NObservationsCurrentSeason(
-            filtername=filtername, nside=nside, offset=offset
+            filtername=filtername, nside=nside, mjd_start=mjd_start
         )
         self.result = np.zeros(hp.nside2npix(self.nside), dtype=float)
-        self.season_frac_start = season_frac_start
-        self.offset = offset
 
     def _calc_value(self, conditions, indx=None):
         result = self.result.copy()
-        season = utils.season_calc(conditions.night, offset=self.offset, floor=False)
-        # Find the area that still needs observation
+
+        # Update the feature to the current time
+        self.survey_features["n_obs_season"].season_update(conditions)
         feature = self.survey_features["n_obs_season"].feature
+
+        # Get the season from the conditions object.
+        season = conditions.season
+
+        # Evaluate where there are not yet enough observations and also
+        # that season is far enough along to require more weight.
         not_enough = np.where(
             (self.footprint > 0)
             & (feature < self.n_per_season)
             & ((IntRounded(season - np.floor(season)) > IntRounded(self.season_frac_start)))
-            & (season >= 0)
         )
         result[not_enough] = 1
         return result
 
 
 class FootprintNvisBasisFunction(BaseBasisFunction):
     """Basis function to drive observations of a given footprint.
     Good to target of opportunity targets where one might want to observe
     a region 3 times.
 
     Parameters
     ----------
     footprint : `np.array`
-        A healpix array (1 for desired, 0 for not desired) of the target footprint.
+        A healpix array (1 for desired, 0 for not desired) of the
+        target footprint.
     nvis : `int` (1)
         The number of visits to try and gather
     """
 
     def __init__(
         self,
         filtername="r",
         nside=None,
         footprint=None,
         nvis=1,
         out_of_bounds_val=np.nan,
     ):
         super(FootprintNvisBasisFunction, self).__init__(nside=nside, filtername=filtername)
+        if footprint is None:
+            footprint = np.zeros(hp.nside2npix(self.nside))
         self.footprint = footprint
         self.nvis = nvis
 
         # Have a feature that tracks how many observations we have
         self.survey_features = {}
         # Map of the number of observations in filter
         self.survey_features["n_obs"] = features.n_observations(filtername=filtername, nside=self.nside)
         self.result = np.zeros(hp.nside2npix(nside))
         self.result.fill(out_of_bounds_val)
         self.out_of_bounds_val = out_of_bounds_val
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def _calc_value(self, conditions, indx=None):
         result = self.result.copy()
         diff = IntRounded(self.footprint * self.nvis - self.survey_features["n_obs"].feature)
 
         result[np.where(diff > IntRounded(0))] = 1
 
@@ -817,15 +902,15 @@
         d1 = IntRounded(conditions.mjd - self.survey_features["last_obs_f1"].feature)
         d2 = IntRounded(conditions.mjd - self.survey_features["last_obs_f2"].feature)
         good = np.where((d1 > self.gap_min) & (d1 < self.gap_max) & (d2 > self.gap_min) & (d2 < self.gap_max))
         result[good] = 1
         return result
 
 
-class AvoidFastRevists(BaseBasisFunction):
+class AvoidFastRevisits(BaseBasisFunction):
     """Marks targets as unseen if they are in a specified time window
     in order to avoid fast revisits.
 
     Parameters
     ----------
     filtername: `str` ('r')
         The name of the filter for this target map.
@@ -835,42 +920,50 @@
         The healpix resolution.
     penalty_val : `float` (np.nan)
         The reward value to use for regions to penalize.
         Will be masked if set to np.nan (default).
     """
 
     def __init__(self, filtername="r", nside=None, gap_min=25.0, penalty_val=np.nan):
-        super(AvoidFastRevists, self).__init__(nside=nside, filtername=filtername)
+        super().__init__(nside=nside, filtername=filtername)
 
         self.filtername = filtername
         self.penalty_val = penalty_val
 
         self.gap_min = IntRounded(gap_min / 60.0 / 24.0)
         self.nside = nside
 
         self.survey_features = dict()
-        self.survey_features["Last_observed"] = features.Last_observed(filtername=filtername, nside=nside)
+        self.survey_features["Last_observed"] = features.LastObserved(filtername=filtername, nside=nside)
 
     def _calc_value(self, conditions, indx=None):
         result = np.ones(hp.nside2npix(self.nside), dtype=float)
         if indx is None:
             indx = np.arange(result.size)
         diff = IntRounded(conditions.mjd - self.survey_features["Last_observed"].feature[indx])
         bad = np.where(diff < self.gap_min)[0]
         result[indx[bad]] = self.penalty_val
         return result
 
 
 class NearSunTwilightBasisFunction(BaseBasisFunction):
-    """Reward looking into the twilight for NEOs at high airmass
+    """Reward areas on the sky at high airmass, within 90 degrees azimuth
+    of the Sun, such as suitable for the near-sun twilight microsurvey for
+    near- or interior-to earth asteroids.
 
     Parameters
     ----------
-    max_airmass : `float` (2.5)
-        The maximum airmass to try and observe (unitless)
+    nside : `int`, optional
+        Nside for the basis function. If None, uses `set_default_nside()`.
+    max_airmass : `float`, oprionl
+        The maximum airmass to try and observe (unitless).
+    penalty : `float`, optional
+        The value to fill in non-rewarded parts of the sky.
+        Default np.nan, which serves to mask regions exceeding the airmass
+        limit and more than 90 degrees azimuth toward the sun.
     """
 
     def __init__(self, nside=None, max_airmass=2.5, penalty=np.nan):
         super(NearSunTwilightBasisFunction, self).__init__(nside=nside)
         self.max_airmass = IntRounded(max_airmass)
         self.result = np.empty(hp.nside2npix(self.nside))
         self.result.fill(penalty)
@@ -915,24 +1008,26 @@
         self.survey_features = {}
         # Track the number of pairs that have been taken in a night
         self.survey_features["Pair_in_night"] = features.PairInNight(
             filtername=filtername, gap_min=gap_min, gap_max=gap_max, nside=nside
         )
 
         # When was it last observed
-        # XXX--since this feature is also in Pair_in_night, I should just access that one!
+        # XXX--since this feature is also in Pair_in_night, I should just
+        # access that one!
         self.survey_features["Last_observed"] = features.LastObserved(filtername=filtername, nside=nside)
 
     def _calc_value(self, conditions, indx=None):
         result = np.zeros(hp.nside2npix(self.nside), dtype=float)
         if indx is None:
             indx = np.arange(result.size)
         diff = conditions.mjd - self.survey_features["Last_observed"].feature[indx]
         mask = np.isnan(diff)
-        # remove NaNs from diff, but save mask so we exclude those values later.
+        # remove NaNs from diff, but save mask so we exclude those values
+        # later.
         diff[mask] = 0.0
         ir_diff = IntRounded(diff)
         good = np.where(
             (ir_diff >= self.gap_min)
             & (ir_diff <= self.gap_max)
             & (self.survey_features["Pair_in_night"].feature[indx] < self.npairs)
             & (~mask)
@@ -944,31 +1039,39 @@
 class M5DiffBasisFunction(BaseBasisFunction):
     """Basis function based on the 5-sigma depth.
     Look up the best depth a healpixel achieves, and compute
     the limiting depth difference given current conditions
 
     Parameters
     ----------
-    fiducial_FWHMEff : `float`
-        The zenith seeing to assume for "good" conditions
+    filtername : `str`, optional
+        The filter to consider for visits.
+    fiducial_FWHMEff : `float`, optional
+        The zenith seeing to assume for "good" conditions.
+        While the dark sky depth map simply scales with this value,
+        picking a reasonable fiducial_FWHMEff is important because
+        this effects the overall value and scale of the reward
+        from the basis function.
+    nside : `int`, optional
+        The nside for the basis function.
+        Default None uses `set_default_nside()`.
     """
 
     def __init__(self, filtername="r", fiducial_FWHMEff=0.7, nside=None):
         super().__init__(nside=nside, filtername=filtername)
         # The dark sky surface brightness values
         self.dark_map = None
         self.fiducial_FWHMEff = fiducial_FWHMEff
         self.filtername = filtername
 
     def _calc_value(self, conditions, indx=None):
         if self.dark_map is None:
             self.dark_map = dark_m5(
                 conditions.dec, self.filtername, conditions.site.latitude_rad, self.fiducial_FWHMEff
             )
-
         # No way to get the sign on this right the first time.
         result = conditions.m5_depth[self.filtername] - self.dark_map
         return result
 
 
 class M5DiffAtHpixBasisFunction(HealpixLimitedBasisFunctionMixin, M5DiffBasisFunction):
     pass
@@ -1104,15 +1207,17 @@
         self.proportion = proportion
         self.aways_available = aways_available
 
         self.survey_features = {}
         self.survey_features["Last_observation"] = features.Last_observation()
         self.survey_features["Last_filter_change"] = features.LastFilterChange()
         self.survey_features["n_obs_all"] = features.NObsCount(filtername=None)
+        # Tag is not actually supported at observation level.
         self.survey_features["n_obs"] = features.NObsCount(filtername=filtername, tag=tag)
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def filter_change_bonus(self, time):
         lag_min = self.time_lag_min
         lag_max = self.time_lag_max
 
         a = 1.0 / (lag_max - lag_min)
         b = -a * lag_min
@@ -1135,37 +1240,39 @@
         elif IntRounded(time) >= IntRounded(lag_max):
             return 1.0 if IntRounded(time) < IntRounded(self.time_lag_boost) else self.boost_gain
 
         return bonus * need
 
     def check_feasibility(self, conditions):
         """
-        This method makes a pre-check of the feasibility of this basis function.
-        If a basis function returns False on the feasibility check,
-        it won't computed at all.
+        This method makes a pre-check of the feasibility of this
+        basis function. If a basis function returns False on the
+        feasibility check, it won't computed at all.
 
         Returns
         -------
         feasibility : `bool`
         """
 
         # Make a quick check about the feasibility of this basis function.
-        # If current filter is none, telescope is parked and we could, in principle, switch to any filter.
-        # If this basis function computes reward for the current filter, then it is also feasible.
-        # At last we check for an "aways_available" flag. Meaning, we force this basis function t
-        # o be aways be computed.
+        # If current filter is none, telescope is parked and we could,
+        # in principle, switch to any filter. If this basis function
+        # computes reward for the current filter, then it is also feasible.
+        # At last we check for an "aways_available" flag. Meaning, we
+        # force this basis function to be aways be computed.
         if (
             conditions.current_filter is None
             or conditions.current_filter == self.filtername
             or self.aways_available
         ):
             return True
 
         # If we arrive here,
-        # we make some extra checks to make sure this bf is feasible and should be computed.
+        # we make some extra checks to make sure this bf is
+        # feasible and should be computed.
 
         # Did the moon set or rise since last observation?
         moon_changed = conditions.moon_alt * self.survey_features["Last_observation"].feature["moonAlt"] < 0
 
         # Are we already in the filter (or at start of night)?
         not_in_filter = conditions.current_filter != self.filtername
 
@@ -1188,23 +1295,18 @@
             return True
         else:
             return False
 
     def _calc_value(self, conditions, **kwargs):
         if conditions.current_filter is None:
             return 0.0  # no bonus if no filter is mounted
-        # elif self.condition_features['Current_filter'].feature == self.filtername:
-        #     return 0.  # no bonus if on the filter already
 
         # Did the moon set or rise since last observation?
         moon_changed = conditions.moon_alt * self.survey_features["Last_observation"].feature["moonAlt"] < 0
 
-        # Are we already in the filter (or at start of night)?
-        # not_in_filter = (self.condition_features['Current_filter'].feature != self.filtername)
-
         # Has enough time past?
         lag = conditions.mjd - self.survey_features["Last_filter_change"].feature["mjd"]
         time_past = lag > self.time_lag_min
 
         # Did twilight start/end?
         twi_changed = (conditions.sun_alt - self.twi_change) * (
             self.survey_features["Last_observation"].feature["sun_alt"] - self.twi_change
@@ -1239,38 +1341,50 @@
 
 
 class SlewtimeBasisFunction(BaseBasisFunction):
     """Reward slews that take little time
 
     Parameters
     ----------
-    max_time : `float` (135)
+    max_time : `float`
          The estimated maximum slewtime (seconds).
-         Used to normalize so the basis function spans ~ -1-0 in reward units.
+         Used to normalize so the basis function spans ~ -1-0
+         in reward units. Default 135 seconds corresponds to just
+         slightly less than a filter change.
+    filtername : `str`, optional
+        The filter to check for pre-post slewtime estimates.
+        If a slew includes a filter change, other basis functions will
+        decide on the reward, so the result here can be 0.
+    nside : `int`, optional
+        Nside for the basis function.
+        Default None will use `set_default_nside()`.
     """
 
     def __init__(self, max_time=135.0, filtername="r", nside=None):
         super(SlewtimeBasisFunction, self).__init__(nside=nside, filtername=filtername)
 
         self.maxtime = max_time
         self.nside = nside
         self.filtername = filtername
 
     def add_observation(self, observation, indx=None):
-        # No tracking of observations in this basis function. Purely based on conditions.
+        # No tracking of observations in this basis function.
+        # Purely based on conditions.
         pass
 
     def _calc_value(self, conditions, indx=None):
-        # If we are in a different filter, the FilterChangeBasisFunction will take it
+        # If we are in a different filter, the
+        # FilterChangeBasisFunction will take it
         if conditions.current_filter != self.filtername:
             result = 0
         else:
             # Need to make sure smaller slewtime is larger reward.
             if np.size(conditions.slewtime) > 1:
-                # Slewtime map can contain nans and/or infs - mask these with nans
+                # Slewtime map can contain nans and/or
+                # infs - mask these with nans
                 result = np.where(
                     np.isfinite(conditions.slewtime),
                     -conditions.slewtime / self.maxtime,
                     np.nan,
                 )
             else:
                 result = -conditions.slewtime / self.maxtime
@@ -1288,17 +1402,19 @@
     def __init__(self, max_time=135.0, order=1.0, hard_max=None, filtername="r", nside=None):
         super(AggressiveSlewtimeBasisFunction, self).__init__(nside=nside, filtername=filtername)
 
         self.maxtime = max_time
         self.hard_max = hard_max
         self.order = order
         self.result = np.zeros(hp.nside2npix(nside), dtype=float)
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def _calc_value(self, conditions, indx=None):
-        # If we are in a different filter, the FilterChangeBasisFunction will take it
+        # If we are in a different filter, the
+        # FilterChangeBasisFunction will take it
         if conditions.current_filter != self.filtername:
             result = 0.0
         else:
             # Need to make sure smaller slewtime is larger reward.
             if np.size(self.condition_features["slewtime"].feature) > 1:
                 result = self.result.copy()
                 result.fill(np.nan)
@@ -1314,34 +1430,40 @@
                     result[hp_indx] = np.min(result[hp_indx])
             else:
                 result = (self.maxtime - conditions.slewtime) / self.maxtime
         return result
 
 
 class SkybrightnessLimitBasisFunction(BaseBasisFunction):
-    """Mask regions that are outside a sky brightness limit
-
-    XXX--TODO:  This should probably go to the mask basis functions.
+    """Mask regions that are outside a sky brightness limit.
 
     Parameters
     ----------
-    min : `float` (20.)
-         The minimum sky brightness (mags).
-    max : `float` (30.)
-         The maximum sky brightness (mags).
-
+    nside : `int`, optional
+        The nside for the basis function. Default None uses
+        `set_default_nside()`.
+    filtername : `str`, optional
+        The filter to consider for the skybrightness pre values.
+    sbmin : `float`, optional
+        The minimum (brightest) skybrightness to consider (mags).
+        Default of 20 will cut out some times of night or parts of the
+        sky.
+    sbmax : `float`, optional
+        The maximum (faintest) skybrightness to consider (mags).
+        Default of 30 will pass all skybrightness values.
     """
 
     def __init__(self, nside=None, filtername="r", sbmin=20.0, sbmax=30.0):
         super(SkybrightnessLimitBasisFunction, self).__init__(nside=nside, filtername=filtername)
 
         self.min = IntRounded(sbmin)
         self.max = IntRounded(sbmax)
         self.result = np.empty(hp.nside2npix(self.nside), dtype=float)
         self.result.fill(np.nan)
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def _calc_value(self, conditions, indx=None):
         result = self.result.copy()
 
         # Replace non-finite values so IntRounded works, then set
         # the result to nan.
         sky_brightness = conditions.skybrightness[self.filtername].copy()
@@ -1404,14 +1526,15 @@
         # Convert to half-width for convienence
         self.nside = nside
         self.active = False
         self.unwrap_direction = 0.0  # either -1., 0., 1.
         self.max_duration = max_duration / 60.0 / 24.0  # Convert to days
         self.activation_time = None
         self.result = np.zeros(hp.nside2npix(self.nside), dtype=float)
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def _calc_value(self, conditions, indx=None):
         result = self.result.copy()
 
         current_abs_rad = np.radians(conditions.az)
         unseen = np.where(np.bitwise_or(conditions.alt < self.min_alt, conditions.alt > self.max_alt))
         result[unseen] = np.nan
@@ -1461,15 +1584,16 @@
 
         # Compute wrap regions and fix distances
         mask_max = np.where(accum_abs_rad > max_abs_rad)
         distance_rad[mask_max] -= TWOPI
         mask_min = np.where(accum_abs_rad < min_abs_rad)
         distance_rad[mask_min] += TWOPI
 
-        # Step-2: Repeat but now with compute reward to unwrap using specified delta_unwrap
+        # Step-2: Repeat but now with compute reward to unwrap
+        # using specified delta_unwrap
         unwrap_current_abs_rad = current_abs_rad - (
             np.abs(self.delta_unwrap) if self.unwrap_direction > 0 else -np.abs(self.delta_unwrap)
         )
         unwrap_distance_rad = divmod(norm_az_rad - unwrap_current_abs_rad, TWOPI)[1]
         unwrap_get_shorter = np.where(unwrap_distance_rad > np.pi)
         unwrap_distance_rad[unwrap_get_shorter] -= TWOPI
         unwrap_distance_rad = np.abs(unwrap_distance_rad)
@@ -1517,15 +1641,15 @@
 
         self.supress_window = np.sort(supress_window)
         self.supress_val = supress_val
         self.enhance_window = np.sort(enhance_window)
         self.enhance_val = enhance_val
 
         self.survey_features = {}
-        self.survey_features["last_observed"] = features.Last_observed(filtername=filtername)
+        self.survey_features["last_observed"] = features.LastObserved(filtername=filtername)
 
         self.empty = np.zeros(hp.nside2npix(self.nside), dtype=float)
         # No map, try to drive the whole area
         if apply_area is None:
             self.apply_indx = np.arange(self.empty.size)
         else:
             self.apply_indx = np.where(apply_area != 0)[0]
@@ -1550,15 +1674,16 @@
                 (IntRounded(mjd_diff) > IntRounded(self.enhance_window[0]))
                 & (IntRounded(mjd_diff) < IntRounded(self.enhance_window[1]))
             )
             result[ind[to_enhance]] = self.enhance_val
         return result
 
 
-# https://docs.astropy.org/en/stable/_modules/astropy/modeling/functional_models.html#Trapezoid1D
+# https://docs.astropy.org/en/stable/_modules/astropy/modeling
+# functional_models.html#Trapezoid1D
 def trapezoid(x, amplitude, x_0, width, slope):
     """One dimensional Trapezoid model function"""
     # Compute the four points where the trapezoid changes slope
     # x1 <= x2 <= x3 <= x4
     x2 = x_0 - width / 2.0
     x3 = x_0 + width / 2.0
     x1 = x2 - amplitude / slope
@@ -1615,15 +1740,15 @@
         self.enhance_slope = enhance_slope
         self.enhance_peak = enhance_peak
         self.enhance_amp = enhance_amp
 
         self.season_limit = season_limit / 12 * np.pi  # To radians
 
         self.survey_features = {}
-        self.survey_features["last_observed"] = features.Last_observed(filtername=filtername)
+        self.survey_features["last_observed"] = features.LastObserved(filtername=filtername)
 
         self.empty = np.zeros(hp.nside2npix(self.nside), dtype=float)
         # No map, try to drive the whole area
         if apply_area is None:
             self.apply_indx = np.arange(self.empty.size)
         else:
             self.apply_indx = np.where(apply_area != 0)[0]
@@ -1637,15 +1762,15 @@
             self.enhance_peak,
             self.enhance_width,
             self.enhance_slope,
         )
 
         return result
 
-    def season_calc(self, conditions):
+    def season_len(self, conditions):
         ra_mid_season = (conditions.sunRA + np.pi) % (2.0 * np.pi)
         angle_to_mid_season = np.abs(conditions.ra - ra_mid_season)
         over = np.where(IntRounded(angle_to_mid_season) > IntRounded(np.pi))
         angle_to_mid_season[over] = 2.0 * np.pi - angle_to_mid_season[over]
 
         return angle_to_mid_season
 
@@ -1659,15 +1784,15 @@
         if np.size(ind) == 0:
             result = 0
         else:
             mjd_diff = conditions.mjd - self.survey_features["last_observed"].feature[ind]
             result[ind] += self.suppress_enhance(mjd_diff)
 
         if self.season_limit is not None:
-            radians_to_midseason = self.season_calc(conditions)
+            radians_to_midseason = self.season_len(conditions)
             outside_season = np.where(radians_to_midseason > self.season_limit)
             result[outside_season] = 0
 
         return result
 
 
 class AzimuthBasisFunction(BaseBasisFunction):
@@ -1686,16 +1811,16 @@
         az_dist[over] = 2.0 * np.pi - az_dist[over]
         # Normalize sp between 0 and 1
         result = az_dist / np.pi
         return result
 
 
 class AzModuloBasisFunction(BaseBasisFunction):
-    """Try to replicate the Rothchild et al cadence forcing by only observing
-    on limited az ranges per night.
+    """Try to replicate the Rothchild et al cadence forcing by
+    only observing on limited az ranges per night.
 
     Parameters
     ----------
     az_limits : `list` of `float` pairs (None)
         The azimuth limits (degrees) to use.
     """
 
@@ -1796,80 +1921,92 @@
     """Drive observations in good seeing conditions"""
 
     def __init__(
         self,
         nside=None,
         filtername="r",
         footprint=None,
-        fwh_meff_limit=0.8,
+        fwhm_eff_limit=0.8,
         mag_diff=0.75,
     ):
         super(GoodSeeingBasisFunction, self).__init__(nside=nside)
 
         self.filtername = filtername
-        self.fwh_meff_limit = IntRounded(fwh_meff_limit)
+        self.fwhm_eff_limit = IntRounded(fwhm_eff_limit)
         if footprint is None:
-            fp = utils.standard_goals(nside=nside)[filtername]
+            footprints, labels = get_current_footprint(nside=self.nside)
+            fp = footprints[self.filtername]
         else:
             fp = footprint
         self.out_of_bounds = np.where(fp == 0)[0]
         self.result = fp * 0
 
         self.mag_diff = IntRounded(mag_diff)
         self.survey_features = {}
-        self.survey_features["coadd_depth_all"] = features.Coadded_depth(filtername=filtername, nside=nside)
-        self.survey_features["coadd_depth_good"] = features.Coadded_depth(
-            filtername=filtername, nside=nside, fwh_meff_limit=fwh_meff_limit
+        self.survey_features["coadd_depth_all"] = features.CoaddedDepth(
+            filtername=self.filtername, nside=self.nside
+        )
+        self.survey_features["coadd_depth_good"] = features.CoaddedDepth(
+            filtername=self.filtername, nside=self.nside, fwhm_eff_limit=fwhm_eff_limit
         )
 
     def _calc_value(self, conditions, **kwargs):
         # Seeing is "bad"
-        if IntRounded(conditions.FWHMeff[self.filtername].min()) > self.fwh_meff_limit:
+        if IntRounded(conditions.FWHMeff[self.filtername].min()) > self.fwhm_eff_limit:
             return 0
         result = self.result.copy()
 
         diff = (
             self.survey_features["coadd_depth_all"].feature - self.survey_features["coadd_depth_good"].feature
         )
         # Where are there things we want to observe?
         good_pix = np.where(
             (IntRounded(diff) > self.mag_diff)
-            & (IntRounded(conditions.FWHMeff[self.filtername]) <= self.fwh_meff_limit)
+            & (IntRounded(conditions.FWHMeff[self.filtername]) <= self.fwhm_eff_limit)
         )
         # Hm, should this scale by the mag differences? Probably.
         result[good_pix] = diff[good_pix]
         result[self.out_of_bounds] = 0
 
         return result
 
 
 class TemplateGenerateBasisFunction(BaseBasisFunction):
     """Emphasize areas that have not been observed in a long time
 
     Parameters
     ----------
-    day_gap : `float`
-        How long to wait before boosting the reward (days)
-    footprint : `np.array`
+    nside : `int`, optional
+        The nside for the basis function and feature.
+        Default None uses `set_default_nside()`.
+    day_gap : `float`, optional
+        How long to wait before boosting the reward (days).
+        Default of 250 pushes visits into parts of the sky which missed
+        a significant chunk of a season.
+    filtername : `str`, optional
+        The filter to consider when tracking observations.
+    footprint : `np.array`, (N,)
         The indices of the healpixels to apply the boost to.
-        Uses the default footprint if None
+        Default None will call `get_current_footprint()`.
     """
 
     def __init__(self, nside=None, day_gap=250.0, filtername="r", footprint=None):
         super(TemplateGenerateBasisFunction, self).__init__(nside=nside)
         self.day_gap = day_gap
         self.filtername = filtername
         self.survey_features = {}
-        self.survey_features["Last_observed"] = features.Last_observed(filtername=filtername)
+        self.survey_features["Last_observed"] = features.LastObserved(filtername=filtername)
         self.result = np.zeros(hp.nside2npix(self.nside))
         if footprint is None:
-            fp = utils.standard_goals(nside=nside)[filtername]
+            footprints, labels = get_current_footprint(self.nside)
+            fp = footprints[self.filtername]
         else:
             fp = footprint
         self.out_of_bounds = np.where(fp == 0)
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def _calc_value(self, conditions, **kwargs):
         result = self.result.copy()
         overdue = np.where(
             (IntRounded(conditions.mjd - self.survey_features["Last_observed"].feature))
             > IntRounded(self.day_gap)
         )
@@ -1886,14 +2023,15 @@
         super(LimitRepeatBasisFunction, self).__init__(nside=nside)
         self.filtername = filtername
         self.n_limit = n_limit
         self.survey_features = {}
         self.survey_features["n_obs"] = features.NObsNight(nside=nside, filtername=filtername)
 
         self.result = np.zeros(hp.nside2npix(self.nside))
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def _calc_value(self, conditions, **kwargs):
         result = self.result.copy()
         good_pix = np.where(self.survey_features["n_obs"].feature >= self.n_limit)[0]
         result[good_pix] = 1
 
         return result
@@ -1908,14 +2046,15 @@
         self.n_obs_in_filt_needed = n_obs_in_filt_needed
         self.filtername = filtername
         self.survey_features = {}
         self.survey_features["n_obs_infilt"] = features.NObsNight(nside=nside, filtername=filtername)
         self.survey_features["n_obs_all"] = features.NObsNight(nside=nside, filtername="")
 
         self.result = np.zeros(hp.nside2npix(self.nside))
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def _calc_value(self, conditions, **kwargs):
         result = self.result.copy()
         good_pix = np.where(
             (self.survey_features["n_obs_infilt"].feature >= self.n_obs_in_filt_needed)
             & (self.survey_features["n_obs_all"].feature >= self.n_obs_needed)
         )[0]
@@ -1928,27 +2067,27 @@
     """Basis function to create a visit gap based on the survey note field.
 
     Parameters
     ----------
     note : str
         Value of the observation "note" field to be masked.
     filter_names : list [str], optional
-        List of filter names that will be considered when evaluating if the gap
-        has passed.
+        List of filter names that will be considered when evaluating
+        if the gap has passed.
     gap_min : float (optional)
         Time gap (default=25, in minutes).
     penalty_val : float or np.nan
         Value of the penalty to apply (default is np.nan).
 
     Notes
     -----
-    When a list of filters is provided, all filters must be observed before the
-    gap requirement will be activated, and once activated, only observations in
-    these filters will be evaluated in context of whether the last observation
-    was at least gap in the past.
+    When a list of filters is provided, all filters must be observed before
+    the gap requirement will be activated, and once activated, only
+    observations in these filters will be evaluated in context of whether
+    the last observation was at least gap in the past.
     """
 
     def __init__(self, note, filter_names=None, gap_min=25.0, penalty_val=np.nan):
         super().__init__()
         self.penalty_val = penalty_val
 
         self.gap = gap_min / 60.0 / 24.0
@@ -1974,20 +2113,23 @@
         return all(after_gap)
 
     def _calc_value(self, conditions, indx=None):
         return 1.0 if self.check_feasibility(conditions) else self.penalty_val
 
 
 class AvoidDirectWind(BaseBasisFunction):
-    """Basis function to avoid direct wind.
+    """Mask the sky where the wind pressure exceeds `wind_speed_maximum`.
 
     Parameters
     ----------
-    wind_speed_maximum : `float`
+    wind_speed_maximum : `float`, optional
         Wind speed to mark regions as unobservable (in m/s).
+    nside : `int`, optional
+        The nside for the basis function. Default None uses
+        `set_default_nside()`.
     """
 
     def __init__(self, wind_speed_maximum=20.0, nside=None):
         super().__init__(nside=nside)
 
         self.wind_speed_maximum = wind_speed_maximum
 
@@ -2025,19 +2167,19 @@
     Notes
     -----
     This basis function is designed to balance the reward of a group of
     surveys, such that the group get a reward boost based on the required
     collective number of observations.
 
     For example, if you have 3 surveys (e.g. SURVEY_A_REGION_1,
-    SURVEY_A_REGION_2, SURVEY_A_REGION_3), when one of them is observed once
-    (SURVEY_A_REGION_1) they all get a small reward boost proportional to the
-    collective number of observations (`nobs_reference`). Further observations
-    of SURVEY_A_REGION_1 would now cause the other surveys to gain a reward
-    boost in relative to it.
+    SURVEY_A_REGION_2, SURVEY_A_REGION_3), when one of them is observed
+    once (SURVEY_A_REGION_1) they all get a small reward boost proportional
+    to the collective number of observations (`nobs_reference`). Further
+    observations of SURVEY_A_REGION_1 would now cause the other surveys
+    to gain a reward boost in relative to it.
     """
 
     def __init__(self, nobs_reference, note_survey, note_interest, nside=None):
         super().__init__(nside=nside)
 
         self.nobs_reference = nobs_reference
 
@@ -2063,17 +2205,17 @@
     note_survey : `str`
         The value of the observation note, to take into account.
     nside : `int`, optional
         Healpix map resolution (ignored).
 
     Notes
     -----
-    This basis function is useful when a survey is composed of more than one
-    observation (e.g. in different filters) and one wants to make sure they are
-    all taken together.
+    This basis function is useful when a survey is composed of more than
+    one observation (e.g. in different filters) and one wants to make sure
+    they are all taken together.
     """
 
     def __init__(self, n_obs_survey, note_survey, nside=None):
         super().__init__(nside=nside)
 
         self.n_obs_survey = n_obs_survey
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/basis_functions/feasibility_funcs.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/basis_functions/feasibility_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,21 @@
 
 from rubin_scheduler.scheduler import features
 from rubin_scheduler.scheduler.basis_functions import BaseBasisFunction
 from rubin_scheduler.scheduler.utils import IntRounded
 
 
 class FilterLoadedBasisFunction(BaseBasisFunction):
-    """Check that the filter(s) needed are loaded
+    """Check that the filter(s) needed are loaded.
+
+    Are the filters in `filternames` loaded and available?
 
     Parameters
     ----------
-    filternames : str or list of str
+    filternames : `str` or `list` [ `str` ]
         The filternames that need to be mounted to execute.
     """
 
     def __init__(self, filternames="r"):
         super(FilterLoadedBasisFunction, self).__init__()
         if not isinstance(filternames, list):
             filternames = [filternames]
@@ -49,25 +51,37 @@
             result = filtername in conditions.mounted_filters
             if result is False:
                 return result
         return result
 
 
 class SunHighLimitBasisFunction(BaseBasisFunction):
-    """Only execute if the sun is high. Have a sum alt limit for sunset, and a time
-    until 12 degree twilight for sun rise.
+    """Only execute if the sun is higher than `sun_alt_limit`,
+    the current time is within `time_to_12deg` of -12 degree twilight,
+    and there is at least `time_remaining` time left before -12 degree
+    twilight.
+
+    Is the current time and sun altitude close to twilight, but not too close?
 
     Parameters
     ----------
     sun_alt_limit : `float`
-        The sun altitude limit (degrees). Sun must be higher than this at sunset to execute
+        The sun altitude limit (degrees). Sun must be higher than this
+        at sunset to execute
     time_to_12deg : `float`
-        How much time must be remaining before 12 degree twilight in the morning (minutes)
+        How much time must be remaining before 12 degree twilight in
+        the morning (minutes)
     time_remaining : `float`
-        Minimum about of time that must be available before trying to execute (minutes)
+        Minimum about of time that must be available before trying to
+        execute (minutes)
+
+    Notes
+    -----
+    This is primarily useful for surveys which must execute within close
+    limits of -12 degree twilight.
     """
 
     def __init__(self, sun_alt_limit=-14.8, time_to_12deg=21.0, time_remaining=15.0):
         super(SunHighLimitBasisFunction, self).__init__()
         if time_to_12deg < time_remaining:
             raise ValueError(
                 "time_to_12deg value of %f is less than time_remaining value of %f."
@@ -92,15 +106,15 @@
 
 
 class OnceInNightBasisFunction(BaseBasisFunction):
     """Stop observing if something has been executed already in the night
 
     Parameters
     ----------
-    notes : list of str
+    notes : `list` [ `str` ]
         A list of str to check if any observations with a matching note exist.
     """
 
     def __init__(self, notes=[]):
         super(OnceInNightBasisFunction, self).__init__()
         self.survey_features["note_in_night"] = features.NoteInNight(notes=notes)
 
@@ -237,16 +251,17 @@
     def check_feasibility(self, conditions):
         available_time = getattr(conditions, "sun_n" + self.alt_limit + "_rising") - conditions.mjd
         result = available_time > self.time_needed
         return result
 
 
 class TimeToScheduledBasisFunction(BaseBasisFunction):
-    """Make sure there is enough time before next scheduled observation. Useful
-    if you want to check before starting a long sequence of observations.
+    """Make sure there is enough time before next scheduled observation.
+    Useful if you want to check before starting a long sequence of
+    observations.
 
     Parameters
     ----------
     time_needed : float (30.)
         The time needed to run a survey (mintues).
     """
 
@@ -299,15 +314,16 @@
         result = True
         if conditions.mjd - self.survey_features["last_obs_self"].feature["mjd"] < self.days_delay:
             result = False
         return result
 
 
 class SoftDelayBasisFunction(BaseBasisFunction):
-    """Like Force_delay, but go ahead and let things catch up if they fall far behind.
+    """Like Force_delay, but go ahead and let things catch up if they fall
+    far behind.
 
     Parameters
     ----------
 
     """
 
     def __init__(self, fractions=[0.000, 0.009, 0.017], delays=[0.0, 0.5, 1.5], survey_name=None):
@@ -370,16 +386,16 @@
         if conditions.moon_alt > 0:
             result = False
         return result
 
 
 class FractionOfObsBasisFunction(BaseBasisFunction):
     """Limit the fraction of all observations that can be labled a certain
-    survey name. Useful for keeping DDFs from exceeding a given fraction of the
-    total survey.
+    survey name. Useful for keeping DDFs from exceeding a given fraction
+    of the total survey.
 
     Parameters
     ----------
     frac_total : float
         The fraction of total observations that can be of this survey
     survey_name : str
         The name of the survey
@@ -407,27 +423,30 @@
     """Look into the future to decide if it's a good time to observe or block.
 
     Parameters
     ----------
     frac_total : float
         The fraction of total observations that can be of this survey
     aggressive_fraction : float
-        If the fraction of observations drops below ths value, be more aggressive in scheduling.
-        e.g., do not wait for conditions to improve, execute as soon as possible.
+        If the fraction of observations drops below ths value, be more
+        aggressive in scheduling.  e.g., do not wait for conditions to
+        improve, execute as soon as possible.
     time_needed : float (30.)
-        Estimate of the amount of time needed to execute DDF sequence (minutes).
+        Estimate of the amount of time needed to execute DDF sequence
+        (minutes).
     RA : float (0.)
         The RA of the DDF
     ha_limits : list of lists (None)
         limits for what hour angles are acceptable (hours). e.g.,
         to give 4 hour window around HA=0, ha_limits=[[22,24], [0,2]]
     survey_name : str ('')
         The name of the survey
     time_jump : float (44.)
-        The amount of time to assume will jump ahead if another survey executes (minutes)
+        The amount of time to assume will jump ahead if another survey
+        executes (minutes)
     sun_alt_limit : float (-18.)
         The limit to assume twilight starts (degrees)
     """
 
     def __init__(
         self,
         frac_total,
@@ -461,29 +480,31 @@
         # If it's more that self.time_jump to hour angle zero
         # See if there will be enough time to twilight in the future
         if (IntRounded(target_ha) > IntRounded(12)) & (
             IntRounded(target_ha) < IntRounded(24.0 - self.time_jump)
         ):
             if IntRounded(available_time) > IntRounded(self.time_needed + self.time_jump):
                 result = False
-                # If we paused for better conditions, but the moon will rise, turn things back on.
+                # If we paused for better conditions, but the moon will
+                # rise, turn things back on.
                 if IntRounded(conditions.moon_alt) < IntRounded(0):
                     if IntRounded(conditions.moonrise) > IntRounded(conditions.mjd):
                         if IntRounded(conditions.moonrise - conditions.mjd) > IntRounded(self.time_jump):
                             result = True
         # If the moon is up and will set soon, pause
         if IntRounded(conditions.moon_alt) > IntRounded(0):
             time_after_moonset = (
                 getattr(conditions, "sun_" + self.sun_alt_limit + "_rising") - conditions.moonset
             )
             if IntRounded(conditions.moonset) > IntRounded(self.time_jump):
                 if IntRounded(time_after_moonset) > IntRounded(self.time_needed):
                     result = False
 
-        # If the survey has fallen far behind, be agressive and observe anytime it's up.
+        # If the survey has fallen far behind, be agressive and observe
+        # anytime it's up.
         if IntRounded(ratio) < IntRounded(self.aggressive_fraction):
             result = True
         return result
 
 
 class CloudedOutBasisFunction(BaseBasisFunction):
     def __init__(self, cloud_limit=0.7):
@@ -494,33 +515,36 @@
         result = True
         if conditions.bulk_cloud > self.cloud_limit:
             result = False
         return result
 
 
 class RisingMoreBasisFunction(BaseBasisFunction):
-    """Say a spot is not available if it will rise substatially before twilight.
+    """Say a spot is not available if it will rise substatially before
+    twilight.
 
     Parameters
     ----------
     RA : float
         The RA of the point in the sky (degrees)
     pad : float
-        When to start observations if there's plenty of time before twilight (minutes)
+        When to start observations if there's plenty of time before
+        twilight (minutes)
     """
 
     def __init__(self, RA, pad=30.0):
         super(RisingMoreBasisFunction, self).__init__()
         self.ra_hours = RA * 24 / 360.0
         self.pad = pad / 60.0  # To hours
 
     def check_feasibility(self, conditions):
         result = True
         hour_angle = conditions.lmst - self.ra_hours
-        # If it's rising, and twilight is well beyond when it crosses the meridian
+        # If it's rising, and twilight is well beyond when it crosses
+        # the meridian
         time_to_twi = (conditions.sun_n18_rising - conditions.mjd) * 24.0
         if (hour_angle < -self.pad) & (np.abs(hour_angle) < (time_to_twi - self.pad)):
             result = False
         return result
 
 
 class SunAltLimitBasisFunction(BaseBasisFunction):
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/basis_functions/mask_basis_funcs.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/basis_functions/mask_basis_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,16 @@
             good = np.where(conditions.HA > (self.ha_max / 12.0 * np.pi))[0]
             result[good] = np.nan
 
         return result
 
 
 class AreaCheckMaskBasisFunction(BaseBasisFunction):
-    """Take a list of other mask basis functions, and do an additional check for area available"""
+    """Take a list of other mask basis functions, and do an additional
+    check for area available"""
 
     def __init__(self, bf_list, nside=32, min_area=1000.0):
         super(AreaCheckMaskBasisFunction, self).__init__(nside=nside)
         self.bf_list = bf_list
         self.result = np.zeros(hp.nside2npix(self.nside), dtype=float)
         self.min_area = min_area
 
@@ -165,16 +166,17 @@
     """Mask the bright planets
 
     Parameters
     ----------
     mask_radius : float (3.5)
         The radius to mask around a planet (degrees).
     planets : list of str (None)
-        A list of planet names to mask. Defaults to ['venus', 'mars', 'jupiter']. Not including
-        Saturn because it moves really slow and has average apparent mag of ~0.4, so fainter than Vega.
+        A list of planet names to mask. Defaults to ['venus', 'mars',
+        'jupiter']. Not including Saturn because it moves really slow
+        and has average apparent mag of ~0.4, so fainter than Vega.
 
     """
 
     def __init__(self, mask_radius=3.5, planets=None, nside=None, scale=1e5):
         super(PlanetMaskBasisFunction, self).__init__(nside=nside)
         if planets is None:
             planets = ["venus", "mars", "jupiter"]
@@ -233,17 +235,17 @@
         # Mask everything to start
         result = np.zeros(hp.nside2npix(self.nside), dtype=float) + np.nan
 
         in_range_alt = np.zeros(hp.nside2npix(self.nside), dtype=int)
         in_range_az = np.zeros(hp.nside2npix(self.nside), dtype=int)
 
         # Compute the alt,az values in the future. Use the conditions object
-        # so the results are cached and can be used by other surveys is needed.
-        # Technically this could fail if the masked region is very narrow or shadow time
-        # is very large.
+        # so the results are cached and can be used by other surveys is
+        # needed. Technically this could fail if the masked region is
+        # very narrow or shadow time is very large.
         future_alt, future_az = conditions.future_alt_az(np.max(conditions.mjd + self.shadow_time))
 
         # apply limits from the conditions object
         for limits in conditions.tel_alt_limits:
             good = np.where(
                 (IntRounded(conditions.alt) >= IntRounded(np.min(limits)))
                 & (IntRounded(conditions.alt) <= IntRounded(np.max(limits)))
@@ -266,36 +268,39 @@
                 & (IntRounded(future_az) <= IntRounded(np.max(limits)))
             )[0]
             in_range_az[good] += 1
 
         passed_all = np.where((in_range_alt > 1) & (in_range_az > 1))[0]
         result[passed_all] = 0
 
-        # Apply additional alt constraint in case we want to be more conservative than the limit
+        # Apply additional alt constraint in case we want to be more
+        # conservative than the limit
         result[np.where(IntRounded(conditions.alt) < IntRounded(self.min_alt))] = np.nan
         result[np.where(IntRounded(conditions.alt) > IntRounded(self.max_alt))] = np.nan
 
         result[np.where(IntRounded(future_alt) < IntRounded(self.min_alt))] = np.nan
         result[np.where(IntRounded(future_alt) > IntRounded(self.max_alt))] = np.nan
 
         return result
 
 
 class ZenithShadowMaskBasisFunction(BaseBasisFunction):
-    """Mask the zenith, and things that will soon pass near zenith. Useful for making sure
-    observations will not be too close to zenith when they need to be observed again (e.g. for a pair).
+    """Mask the zenith, and things that will soon pass near zenith.
+    Useful for making sure observations will not be too close to zenith
+    when they need to be observed again (e.g. for a pair).
 
     Parameters
     ----------
     min_alt : float (20.)
         The minimum alititude to alow. Everything lower is masked. (degrees)
     max_alt : float (82.)
         The maximum altitude to alow. Everything higher is masked. (degrees)
     shadow_minutes : float (40.)
-        Mask anything that will pass through the max alt in the next shadow_minutes time. (minutes)
+        Mask anything that will pass through the max alt in the next
+        shadow_minutes time. (minutes)
     """
 
     def __init__(
         self,
         nside=None,
         min_alt=20.0,
         max_alt=82.0,
@@ -352,15 +357,16 @@
     """Avoid looking too close to the moon.
 
     Parameters
     ----------
     moon_distance: float (30.)
         Minimum allowed moon distance. (degrees)
 
-    XXX--TODO:  This could be a more complicated function of filter and moon phase.
+    XXX--TODO:  This could be a more complicated function of filter
+    and moon phase.
     """
 
     def __init__(self, nside=None, moon_distance=30.0):
         super(MoonAvoidanceBasisFunction, self).__init__(nside=nside)
         self.update_on_newobs = False
 
         self.moon_distance = IntRounded(np.radians(moon_distance))
@@ -383,17 +389,19 @@
     the same healpixels on a maximum cloud map.
 
     Parameters
     ----------
     nside: int (default_nside)
         The healpix resolution.
     max_cloud_map : numpy array (None)
-        A healpix map showing the maximum allowed cloud values for all points on the sky
+        A healpix map showing the maximum allowed cloud values for all
+        points on the sky
     out_of_bounds_val : float (10.)
-        Point value to give regions where there are no observations requested
+        Point value to give regions where there are no observations
+        requested
     """
 
     def __init__(self, nside=None, max_cloud_map=None, max_val=0.7, out_of_bounds_val=np.nan):
         super(BulkCloudBasisFunction, self).__init__(nside=nside)
         self.update_on_newobs = False
 
         if max_cloud_map is None:
@@ -408,16 +416,16 @@
         """
         Parameters
         ----------
         indx : list (None)
             Index values to compute, if None, full map is computed
         Returns
         -------
-        Healpix map where pixels with a cloud value greater than the max_cloud_map
-        value are marked as unseen.
+        Healpix map where pixels with a cloud value greater than the
+        max_cloud_map value are marked as unseen.
         """
 
         result = self.result.copy()
 
         clouded = np.where(self.max_cloud_map <= conditions.bulk_cloud)
         result[clouded] = self.out_of_bounds_val
 
@@ -430,17 +438,19 @@
     when the telemetry stream can include a full sky cloud map.
 
     Parameters
     ----------
     nside: int (default_nside)
         The healpix resolution.
     max_cloud_map : numpy array (None)
-        A healpix map showing the maximum allowed cloud values for all points on the sky
+        A healpix map showing the maximum allowed cloud values for all
+        points on the sky
     out_of_bounds_val : float (10.)
-        Point value to give regions where there are no observations requested
+        Point value to give regions where there are no observations
+        requested
     """
 
     def __init__(self, nside=None, max_cloud_map=None, max_val=0.7, out_of_bounds_val=np.nan):
         super(BulkCloudBasisFunction, self).__init__(nside=nside)
         self.update_on_newobs = False
 
         if max_cloud_map is None:
@@ -455,16 +465,16 @@
         """
         Parameters
         ----------
         indx : list (None)
             Index values to compute, if None, full map is computed
         Returns
         -------
-        Healpix map where pixels with a cloud value greater than the max_cloud_map
-        value are marked as unseen.
+        Healpix map where pixels with a cloud value greater than the
+        max_cloud_map value are marked as unseen.
         """
 
         result = self.result.copy()
 
         clouded = np.where(self.max_cloud_map <= conditions.bulk_cloud)
         result[clouded] = self.out_of_bounds_val
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/basis_functions/rolling_funcs.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/basis_functions/rolling_funcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,56 +7,80 @@
 import warnings
 
 import healpy as hp
 import numpy as np
 
 from rubin_scheduler.scheduler import features, utils
 from rubin_scheduler.scheduler.basis_functions import BaseBasisFunction
+from rubin_scheduler.scheduler.utils import ConstantFootprint
+
+
+def send_unused_deprecation_warning(name):
+    message = (
+        f"The basis function {name} is not in use by the current "
+        "baseline scheduler and may be deprecated shortly. "
+        "Please contact the rubin_scheduler maintainers if "
+        "this is in use elsewhere."
+    )
+    warnings.warn(message, FutureWarning)
 
 
 class FootprintBasisFunction(BaseBasisFunction):
     """Basis function that tries to maintain a uniformly covered footprint
 
     Parameters
     ----------
-    filtername : str ('r')
-        The filter for this footprint
-    footprint : rubin_scheduler.scheduler.utils.Footprint object
-        The desired footprint.
-    all_footprints_sum : float (None)
-        If using multiple filters, the sum of all the footprints. Needed to make sure basis functions are
-        normalized properly across all fitlers.
-    out_of_bounds_val : float (-10)
-        The value to set the basis function for regions that are not in the footprint (default -10, np.nan is
-        another good value to use)
+    filtername : `str`, optional
+        The filter for this footprint. Default r.
+    nside : `int`, optional
+        The nside for the basis function and features.
+        Default None uses `~utils.set_default_nside()`
+    footprint : `~rubin_scheduler.scheduler.utils.Footprint` object
+        The desired footprint. The default will set this to None,
+        but in general this is really not desirable.
+        In order to make default a kwarg, a current baseline footprint
+        is setup with a Constant footprint (not rolling, not even season
+        aware).
+    out_of_bounds_val : `float`, optional
+        The value to set the basis function for regions that are not in
+        the footprint. Default -10, np.nan is another good value to use.
 
     """
 
     def __init__(
         self,
         filtername="r",
         nside=None,
         footprint=None,
         out_of_bounds_val=-10.0,
-        window_size=6.0,
     ):
-        super(FootprintBasisFunction, self).__init__(nside=nside, filtername=filtername)
+        super().__init__(nside=nside, filtername=filtername)
+        if footprint is None:
+            # This is useful as a backup, but really footprint SHOULD
+            # be specified when basis function is set up.
+            # This just uses whole survey, but doesn't set up rolling.
+            warnings.warn("No Footprint set, using a constant default.")
+            target_maps, labels = utils.get_current_footprint(self.nside)
+            fp = ConstantFootprint(nside=self.nside)
+            for f in "ugrizy":
+                fp.set_footprint(f, target_maps[f])
         self.footprint = footprint
 
         self.survey_features = {}
         # All the observations in all filters
-        self.survey_features["N_obs_all"] = features.NObservations(nside=nside, filtername=None)
-        self.survey_features["N_obs"] = features.NObservations(nside=nside, filtername=filtername)
+        self.survey_features["N_obs_all"] = features.NObservations(nside=self.nside, filtername=None)
+        self.survey_features["N_obs"] = features.NObservations(nside=self.nside, filtername=filtername)
 
         # should probably actually loop over all the target maps?
         self.out_of_bounds_area = np.where(footprint.get_footprint(self.filtername) <= 0)[0]
         self.out_of_bounds_val = out_of_bounds_val
 
     def _calc_value(self, conditions, indx=None):
-        # Find out what the footprint object thinks we should have been observed
+        # Find out what the footprint object thinks we should have been
+        # observed
         desired_footprint_normed = self.footprint(conditions.mjd)[self.filtername]
 
         # Compute how many observations we should have on the sky
         desired = desired_footprint_normed * np.sum(self.survey_features["N_obs_all"].feature)
         result = desired - self.survey_features["N_obs"].feature
         result[self.out_of_bounds_area] = self.out_of_bounds_val
         return result
@@ -64,25 +88,27 @@
 
 class FootprintRollingBasisFunction(BaseBasisFunction):
     """Let's get the rolling really right.
 
     Parameters
     ----------
     footprints : list of np.array
-        List of HEALpix arrays. The footprints should all have matching sums and have the same nside.
+        List of HEALpix arrays. The footprints should all have matching
+        sums and have the same nside.
     all_footprints_sum : float
         The sum of footprints over all filters.
     all_rolling_sum : float
         The sum (over all filters) of the region of the maps that changs.
     season_modulo : int (2)
         The modulo to pass to utils.season_calc.
     season_length : float (365.25)
         How long a season should be (days).
     max_season : int (None)
-        If set, the season calc will return -1 for values greater than max_season
+        If set, the season calc will return -1 for values greater than
+        max_season
     day_offset : np.array (None)
         Offset to pass to utils.season_calc (days).
 
     """
 
     def __init__(
         self,
@@ -92,20 +118,20 @@
         all_footprints_sum=None,
         all_rolling_sum=None,
         out_of_bounds_val=-10,
         season_modulo=2,
         season_length=365.25,
         max_season=None,
         day_offset=None,
-        window_size=6.0,
     ):
         super(FootprintRollingBasisFunction, self).__init__(nside=nside, filtername=filtername)
 
-        # OK, going to find the parts of the map that are the same everywhere, and compute the
-        # basis function the same as usual for those.
+        # OK, going to find the parts of the map that are the same
+        # everywhere, and compute the basis function the same as usual
+        # for those.
         same_footprint = np.ones(footprints[0].size, dtype=bool)
         for footprint in footprints[0:-1]:
             same_footprint = same_footprint & (footprint == footprints[-1])
 
         sum_footprints = footprints[0] * 0
         for footprint in footprints:
             sum_footprints += footprint
@@ -153,24 +179,30 @@
             )
 
         # Now I need to track the observations taken in each season.
         self.out_of_bounds_area = np.where(footprint <= 0)[0]
         self.out_of_bounds_val = out_of_bounds_val
 
         self.result = np.zeros(hp.nside2npix(nside), dtype=float)
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def _calc_value(self, conditions, indx=None):
         result = self.result.copy()
 
         # Compute what season it is at each pixel
-        seasons = conditions.season(
-            modulo=self.season_modulo,
-            max_season=self.max_season,
-            season_length=self.season_length,
-        )
+        seasons = conditions.season.copy()
+        seasons = seasons * 365.25 / self.season_length
+        if self.max_season is not None:
+            over_indx = np.where(seasons >= self.max_season)
+        if self.season_modulo is not None:
+            neg = np.where(seasons < 0)
+            seasons = seasons % self.season_modulo
+            seasons[neg] = -1
+        if self.max_season is not None:
+            seasons[over_indx] = -1
 
         # Update the coverage of the sky so far
         # If RA to sun is zero, we are at phase np.pi/2.
         coverage_map_phase = (conditions.ra - conditions.sun_RA_start + np.pi / 2.0) % (2.0 * np.pi)
         zero = utils.step_line(0.0, 1.0, 365.25, phase=coverage_map_phase * 365.25 / 2 / np.pi)
         t_elapsed = conditions.mjd - conditions.mjd_start
         norm_coverage_raw = utils.step_line(
@@ -216,41 +248,46 @@
             )
 
         result[self.out_of_bounds_area] = self.out_of_bounds_val
         return result
 
 
 class TargetMapModuloBasisFunction(BaseBasisFunction):
-    """Basis function that tracks number of observations and tries to match a specified spatial distribution
-    can enter multiple maps that will be used at different times in the survey
+    """Basis function that tracks number of observations and tries to match
+    a specified spatial distribution can enter multiple maps that will be
+    used at different times in the survey
 
     Parameters
     ----------
     day_offset : np.array
-        Healpix map that has the offset to be applied to each pixel when computing what season it is on.
+        Healpix map that has the offset to be applied to each pixel when
+        computing what season it is on.
     filtername : (string 'r')
         The name of the filter for this target map.
     nside: int (default_nside)
         The healpix resolution.
     target_maps : list of numpy array (None)
-        healpix maps showing the ratio of observations desired for all points on the sky.
-        Last map will be used for season -1. Probably shouldn't support going to season
-        less than -1.
+        healpix maps showing the ratio of observations desired for all
+        points on the sky. Last map will be used for season -1. Probably
+        shouldn't support going to season less than -1.
     norm_factor : float (0.00010519)
-        for converting target map to number of observations. Should be the area of the camera
-        divided by the area of a healpixel divided by the sum of all your goal maps. Default
-        value assumes LSST foV has 1.75 degree radius and the standard goal maps. If using
-        mulitple filters, see rubin_scheduler.scheduler.utils.calc_norm_factor for a utility
-        that computes norm_factor.
+        for converting target map to number of observations. Should be the
+        area of the camera divided by the area of a healpixel divided by
+        the sum of all your goal maps. Default value assumes LSST foV has
+        1.75 degree radius and the standard goal maps. If using mulitple
+        filters, see rubin_scheduler.scheduler.utils.calc_norm_factor for
+        a utility that computes norm_factor.
     out_of_bounds_val : float (-10.)
-        Reward value to give regions where there are no observations requested (unitless).
+        Reward value to give regions where there are no observations
+        requested (unitless).
     season_modulo : int (2)
         The value to modulate the season by (years).
     max_season : int (None)
-        For seasons higher than this value (pre-modulo), the final target map is used.
+        For seasons higher than this value (pre-modulo), the final target
+        map is used.
 
     """
 
     def __init__(
         self,
         day_offset=None,
         filtername="r",
@@ -309,15 +346,16 @@
             season_modulo=season_modulo,
             offset=day_offset,
             nside=self.nside,
             max_season=max_season,
             season_length=season_length,
         )
         if target_maps is None:
-            self.target_maps = utils.generate_goal_map(filtername=filtername, nside=self.nside)
+            target_maps, labels = utils.get_current_footprint(nside)
+            self.target_map = target_maps[filtername]
         else:
             self.target_maps = target_maps
         # should probably actually loop over all the target maps?
         self.out_of_bounds_area = np.where(self.target_maps[0] == 0)[0]
         self.out_of_bounds_val = out_of_bounds_val
         self.result = np.zeros(hp.nside2npix(self.nside), dtype=float)
         self.all_indx = np.arange(self.result.size)
@@ -327,14 +365,15 @@
             self.day_offset = np.zeros(hp.nside2npix(self.nside), dtype=float)
         else:
             self.day_offset = day_offset
 
         self.season_modulo = season_modulo
         self.max_season = max_season
         self.season_length = season_length
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def _calc_value(self, conditions, indx=None):
         """
         Parameters
         ----------
         indx : list (None)
             Index values to compute, if None, full map is computed
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/detailers/detailer.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/detailers/detailer.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,60 +2,69 @@
     "BaseDetailer",
     "ZeroRotDetailer",
     "Comcam90rotDetailer",
     "Rottep2RotspDesiredDetailer",
     "CloseAltDetailer",
     "TakeAsPairsDetailer",
     "TwilightTripleDetailer",
-    "SpiderRotDetailer",
     "FlushForSchedDetailer",
     "FilterNexp",
     "FixedSkyAngleDetailer",
     "ParallacticRotationDetailer",
     "FlushByDetailer",
 )
 
 import copy
 
 import numpy as np
 
 from rubin_scheduler.scheduler.utils import IntRounded
-from rubin_scheduler.utils import _angular_separation, _approx_altaz2pa, _approx_ra_dec2_alt_az
+from rubin_scheduler.utils import (
+    _angular_separation,
+    _approx_altaz2pa,
+    _approx_ra_dec2_alt_az,
+    pseudo_parallactic_angle,
+    rotation_converter,
+)
 
 
 class BaseDetailer:
     """
-    A Detailer is an object that takes a list of proposed observations and adds "details" to them. The
-    primary purpose is that the Markov Decision Process does an excelent job selecting RA,Dec,filter
-    combinations, but we may want to add additional logic such as what to set the camera rotation angle
-    to, or what to use for an exposure time. We could also modify the order of the proposed observations.
-    For Deep Drilling Fields, a detailer could be useful for computing dither positions and modifying
-    the exact RA,Dec positions.
+    A Detailer is an object that takes a list of proposed observations and
+    adds "details" to them. The primary purpose is that the Markov Decision
+    Process does an excelent job selecting RA,Dec,filter combinations, but we
+    may want to add additional logic such as what to set the camera rotation
+    angle to, or what to use for an exposure time. We could also modify the
+    order of the proposed observations. For Deep Drilling Fields, a detailer
+    could be useful for computing dither positions and modifying the exact
+    RA,Dec positions.
     """
 
     def __init__(self, nside=32):
         """"""
         # Dict to hold all the features we want to track
         self.survey_features = {}
         self.nside = nside
 
     def add_observations_array(self, observations_array, observations_hpid):
-        """Like add_observation, but for loading a whole array of observations at a time"""
+        """Like add_observation, but for loading a whole array of
+        observations at a time"""
 
         for feature in self.survey_features:
             self.survey_features[feature].add_observations_array(observations_array, observations_hpid)
 
     def add_observation(self, observation, indx=None):
         """
         Parameters
         ----------
         observation : `np.array`
             An array with information about the input observation
         indx : `np.array`
-            The indices of the healpix map that the observation overlaps with
+            The indices of the healpix map that the observation overlaps
+            with
         """
         for feature in self.survey_features:
             self.survey_features[feature].add_observation(observation, indx=indx)
 
     def __call__(self, observation_list, conditions):
         """
         Parameters
@@ -69,15 +78,16 @@
         List of observations.
         """
 
         return observation_list
 
 
 class FlushByDetailer(BaseDetailer):
-    """Set the MJD an observation should be flushed from the scheduler queue if not yet completed.
+    """Set the MJD an observation should be flushed from the scheduler
+    queue if not yet completed.
 
     Parameters
     ----------
     flush_time : float
         The time to flush after the current MJD. Default 60 minutes
     """
 
@@ -91,28 +101,32 @@
             obs["flush_by_mjd"] = conditions.mjd + self.flush_time
         return observation_list
 
 
 class ParallacticRotationDetailer(BaseDetailer):
     """Set the rotator to near the parallactic angle"""
 
+    def __init__(self, telescope="rubin"):
+        self.rc = rotation_converter(telescope=telescope)
+        self.survey_features = {}
+
     def __call__(self, observation_list, conditions, limits=[-270, 270]):
         limits = np.radians(limits)
         for obs in observation_list:
             alt, az = _approx_ra_dec2_alt_az(
                 obs["RA"],
                 obs["dec"],
                 conditions.site.latitude_rad,
                 conditions.site.longitude_rad,
                 conditions.mjd,
             )
             obs_pa = _approx_altaz2pa(alt, az, conditions.site.latitude_rad)
             obs["rotSkyPos_desired"] = obs_pa
 
-            resulting_rot_tel_pos = obs["rotSkyPos_desired"] + obs_pa
+            resulting_rot_tel_pos = self.rc._rotskypos2rottelpos(obs["rotSkyPos_desired"], obs_pa)
 
             if resulting_rot_tel_pos > np.max(limits):
                 resulting_rot_tel_pos -= 2 * np.pi
             if resulting_rot_tel_pos < np.min(limits):
                 resulting_rot_tel_pos += 2 * np.pi
 
             # If those corrections still leave us bad, just pull it back 180.
@@ -126,98 +140,101 @@
 
         return observation_list
 
 
 class Rottep2RotspDesiredDetailer(BaseDetailer):
     """Convert all the rotTelPos values to rotSkyPos_desired"""
 
+    def __init__(self, telescope="rubin"):
+        self.rc = rotation_converter(telescope=telescope)
+        self.survey_features = {}
+
     def __call__(self, observation_list, conditions):
         obs_array = np.concatenate(observation_list)
 
         alt, az = _approx_ra_dec2_alt_az(
             obs_array["RA"],
             obs_array["dec"],
             conditions.site.latitude_rad,
             conditions.site.longitude_rad,
             conditions.mjd,
         )
         obs_pa = _approx_altaz2pa(alt, az, conditions.site.latitude_rad)
 
-        rot_sky_pos_desired = (obs_array["rotTelPos"] - obs_pa) % (2.0 * np.pi)
+        rot_sky_pos_desired = self.rc._rotskypos2rottelpos(obs_array["rotTelPos"], obs_pa)
 
         for obs, rotsp_d in zip(observation_list, rot_sky_pos_desired):
             obs["rotTelPos_backup"] = obs["rotTelPos"] + 0
             obs["rotTelPos"] = np.nan
             obs["rotSkyPos"] = np.nan
             obs["rotSkyPos_desired"] = rotsp_d
 
         return observation_list
 
 
 class ZeroRotDetailer(BaseDetailer):
     """
-    Detailer to set the camera rotation to be apporximately zero in rotTelPos.
-    Because it can never be written too many times:
-    rotSkyPos = rotTelPos - ParallacticAngle
-    But, wait, what? Is it really the other way?
+    Detailer to set the camera rotation to be apporximately zero in
+    rotTelPos.
+
+    Parameters
+    ----------
+    telescope : `str`
+        Which telescope convention to use for setting the conversion
+        between rotTelPos and rotSkyPos. Default "rubin".
     """
 
+    def __init__(self, telescope="rubin", nside=32):
+        self.rc = rotation_converter(telescope=telescope)
+        self.survey_features = {}
+
     def __call__(self, observation_list, conditions):
-        # XXX--should I convert the list into an array and get rid of this loop?
+        # XXX--should I convert the list into an array and get rid of this
+        # loop?
         for obs in observation_list:
-            alt, az = _approx_ra_dec2_alt_az(
+            obs_pa, alt, az = pseudo_parallactic_angle(
                 obs["RA"],
                 obs["dec"],
-                conditions.site.latitude_rad,
-                conditions.site.longitude_rad,
                 conditions.mjd,
+                np.degrees(conditions.site.longitude_rad),
+                np.degrees(conditions.site.latitude_rad),
             )
-            obs_pa = _approx_altaz2pa(alt, az, conditions.site.latitude_rad)
-            obs["rotSkyPos"] = obs_pa
 
-        return observation_list
-
-
-class SpiderRotDetailer(BaseDetailer):
-    """
-    Set the camera rotation to +/- 45 degrees so diffraction spikes align along chip rows
-    and columns
-    """
-
-    def __call__(self, observation_list, conditions):
-        indx = int(conditions.night % 2)
-        rot_tel_pos = np.radians([45.0, 315.0][indx])
-
-        for obs in observation_list:
-            obs["rotSkyPos"] = np.nan
-            obs["rot_tel_pos"] = rot_tel_pos
+            obs["rotSkyPos"] = self.rc.rottelpos2rotskypos(0.0, obs_pa)
 
         return observation_list
 
 
 class Comcam90rotDetailer(BaseDetailer):
     """
-    Detailer to set the camera rotation so rotSkyPos is 0, 90, 180, or 270 degrees. Whatever
-    is closest to rotTelPos of zero.
+    Detailer to set the camera rotation so rotSkyPos is 0, 90, 180, or
+    270 degrees. Whatever is closest to rotTelPos of zero.
     """
 
+    def __init__(self, telescope="rubin", nside=32):
+        self.rc = rotation_converter(telescope=telescope)
+        self.survey_features = {}
+
     def __call__(self, observation_list, conditions):
         favored_rot_sky_pos = np.radians([0.0, 90.0, 180.0, 270.0, 360.0]).reshape(5, 1)
         obs_array = np.concatenate(observation_list)
-        alt, az = _approx_ra_dec2_alt_az(
-            obs_array["RA"],
-            obs_array["dec"],
-            conditions.site.latitude_rad,
-            conditions.site.longitude_rad,
-            conditions.mjd,
+
+        parallactic_angle, alt, az = np.radians(
+            pseudo_parallactic_angle(
+                obs_array["RA"],
+                obs_array["dec"],
+                conditions.mjd,
+                np.degrees(conditions.site.longitude_rad),
+                np.degrees(conditions.site.latitude_rad),
+            )
         )
-        parallactic_angle = _approx_altaz2pa(alt, az, conditions.site.latitude_rad)
-        # If we set rotSkyPos to parallactic angle, rotTelPos will be zero. So, find the
-        # favored rotSkyPos that is closest to PA to keep rotTelPos as close as possible to zero.
-        ang_diff = np.abs(parallactic_angle - favored_rot_sky_pos)
+
+        # need to find the
+
+        ang_diff = np.abs(self.rc._rotskypos2rottelpos(favored_rot_sky_pos, parallactic_angle))
         min_indxs = np.argmin(ang_diff, axis=0)
         # can swap 360 and zero if needed?
         final_rot_sky_pos = favored_rot_sky_pos[min_indxs]
         # Set all the observations to the proper rotSkyPos
         for rsp, obs in zip(final_rot_sky_pos, observation_list):
             obs["rotSkyPos"] = rsp
 
@@ -243,15 +260,16 @@
             observation["rotSkyPos"] = self.sky_angle
 
         return observation_list
 
 
 class CloseAltDetailer(BaseDetailer):
     """
-    re-order a list of observations so that the closest in altitude to the current pointing is first.
+    re-order a list of observations so that the closest in altitude to
+    the current pointing is first.
 
     Parameters
     ----------
     alt_band : `float` (10)
         The altitude band to try and stay in (degrees)
     """
 
@@ -349,15 +367,16 @@
             result = paired + observation_list
         else:
             for obs in paired:
                 obs["note"] = obs["note"][0] + ", b"
             for obs in observation_list:
                 obs["note"] = obs["note"][0] + ", a"
             result = observation_list + paired
-        # XXX--maybe a temp debugging thing, label what part of sequence each observation is.
+        # XXX--maybe a temp debugging thing, label what part of sequence
+        # each observation is.
         for i, obs in enumerate(result):
             obs["survey_id"] = i
         return result
 
 
 class TwilightTripleDetailer(BaseDetailer):
     def __init__(self, slew_estimate=5.0, n_repeat=3, update_note=True):
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/detailers/dither_detailer.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/detailers/dither_detailer.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from rubin_scheduler.scheduler.utils import wrap_ra_dec
 from rubin_scheduler.utils import (
     _approx_altaz2pa,
     _approx_ra_dec2_alt_az,
     bearing,
     dest_latlon,
     gnomonic_project_tosky,
+    rotation_converter,
 )
 
 
 class DitherDetailer(BaseDetailer):
     """
-    make a uniform dither pattern. Offset by a maximum radius in a random direction.
-    Mostly intended for DDF pointings, the BaseMarkovDF_survey class includes dithering
-    for large areas.
+    make a uniform dither pattern. Offset by a maximum radius in a random
+    direction. Mostly intended for DDF pointings, the BaseMarkovDF_survey
+    class includes dithering for large areas.
 
     Parameters
     ----------
     max_dither : `float` (0.7)
         The maximum dither size to use (degrees).
     per_night : `bool` (True)
         If true, us the same dither offset for an entire night
@@ -49,15 +50,14 @@
                 self.current_night = night
                 self.offset = self.offsets[night, :]
                 angle = self.angles[night]
                 radius = self.radii[night]
                 self.offset = np.array([radius * np.cos(angle), radius * np.sin(angle)])
             offsets = np.tile(self.offset, (n_offsets, 1))
         else:
-            self.rng = np.random.default_rng()
             angle = self.rng.random(n_offsets) * 2 * np.pi
             radius = self.max_dither * np.sqrt(self.rng.random(n_offsets))
             offsets = np.array([radius * np.cos(angle), radius * np.sin(angle)]).T
 
         return offsets
 
     def __call__(self, observation_list, conditions):
@@ -206,29 +206,33 @@
     Parameters
     ----------
     max_rot : `float` (90.)
         The maximum amount to offset the camera (degrees)
     min_rot : `float` (90)
         The minimum to offset the camera (degrees)
     per_night : `bool` (True)
-        If True, only set a new offset per night. If False, randomly rotates every observation.
+        If True, only set a new offset per night. If False, randomly
+        rotates every observation.
+    telescope : `str`
+        Telescope name. Options of "rubin" or "auxtel". Default "rubin".
     """
 
-    def __init__(self, max_rot=90.0, min_rot=-90.0, per_night=True, seed=42, nnights=7305):
+    def __init__(self, max_rot=90.0, min_rot=-90.0, per_night=True, seed=42, nnights=7305, telescope="rubin"):
         self.survey_features = {}
 
         self.current_night = -1
         self.max_rot = np.radians(max_rot)
         self.min_rot = np.radians(min_rot)
         self.range = self.max_rot - self.min_rot
         self.per_night = per_night
         self.rng = np.random.default_rng(seed)
         self.offsets = self.rng.random(nnights)
 
         self.offset = None
+        self.rc = rotation_converter(telescope=telescope)
 
     def _generate_offsets(self, n_offsets, night):
         if self.per_night:
             if night != self.current_night:
                 self.current_night = night
                 self.offset = self.offsets[night] * self.range + self.min_rot
             offsets = np.ones(n_offsets) * self.offset
@@ -247,11 +251,11 @@
                 obs["RA"],
                 obs["dec"],
                 conditions.site.latitude_rad,
                 conditions.site.longitude_rad,
                 conditions.mjd,
             )
             obs_pa = _approx_altaz2pa(alt, az, conditions.site.latitude_rad)
-            obs["rotSkyPos"] = (offsets[i] - obs_pa) % (2.0 * np.pi)
+            obs["rotSkyPos"] = self.rc._rottelpos2rotskypos(offsets[i], obs_pa)
             obs["rotTelPos"] = offsets[i]
 
         return observation_list
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/detailers/short_survey.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/detailers/short_survey.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 import rubin_scheduler.scheduler.features as features
 from rubin_scheduler.scheduler.detailers import BaseDetailer
 from rubin_scheduler.scheduler.utils import HpInLsstFov
 from rubin_scheduler.utils import survey_start_mjd
 
 
 class ShortExptDetailer(BaseDetailer):
-    """Check if the area has been observed with a short exposure time this year.
-    If not, add some short exposures.
+    """Check if the area has been observed with a short exposure time
+    this year. If not, add some short exposures.
 
     Parameters
     ----------
     exp_time : `float` (1.)
         The short exposure time to use.
     nobs : `float` (2)
         The number of observations to try and take per year
     night_max : `float` (None)
-        Do not apply any changes to the observation list if the current night is greater than night_max.
+        Do not apply any changes to the observation list if the current
+        night is greater than night_max.
     n_repeat : `int` (1)
         How many short observations to do in a row.
     time_scale : `bool` (False)
         Should the short observations be scaled throughout the year (True),
         or taken as fast as possible (False).
 
     """
@@ -59,16 +60,17 @@
         self.survey_features["nobs"] = features.N_observations(
             filtername=filtername, nside=nside, survey_name=self.survey_name
         )
         # Need to be able to look up hpids for each observation
         self.obs2hpid = HpInLsstFov(nside=nside)
 
     def __call__(self, observation_list, conditions):
-        # XXX--this logic would probably make more sense as a feasability basis function.
-        # Might consider expanding the detailer base class to include basis functions.
+        # XXX--this logic would probably make more sense as a feasability
+        # basis function. Might consider expanding the detailer base class
+        # to include basis functions.
         if self.night_max is not None:
             if conditions.night > self.night_max:
                 return observation_list
 
         out_observations = []
         # Compute how many observations we should have taken by now
         if self.time_scale:
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/detailers/vary_exptime.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/detailers/vary_exptime.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,25 +51,27 @@
     for filtername in sky_mags:
         goal_m5[filtername] = m5_flat_sed(filtername, sky_mags[filtername], fiducial_seeing, exptime, airmass)
 
     return goal_m5
 
 
 class VaryExptDetailer(BaseDetailer):
-    """Vary the exposure time on observations to try and keep each observation at uniform depth.
+    """Vary the exposure time on observations to try and keep each
+    observation at uniform depth.
 
     Parameters
     ----------
     min_expt : `float` (20.)
         The minimum exposure time to use (seconds).
     max_expt : `float` (100.)
         The maximum exposure time to use
     target_m5 : `dict` (None)
-        Dictionary with keys of filternames as str and target 5-sigma depth values as floats.
-        If none, the target_m5s are set to a min_expt exposure at X=1.1 in dark time.
+        Dictionary with keys of filternames as str and target 5-sigma
+        depth values as floats. If none, the target_m5s are set to a
+        min_expt exposure at X=1.1 in dark time.
 
     """
 
     def __init__(self, nside=32, min_expt=20.0, max_expt=100.0, target_m5=None):
         """"""
         # Dict to hold all the features we want to track
         self.survey_features = {}
@@ -102,30 +104,32 @@
         """
         obs_array = np.concatenate(observation_list)
         hpids = ra_dec2_hpid(self.nside, obs_array["RA"], obs_array["dec"])
         new_expts = np.zeros(obs_array.size, dtype=float)
         for filtername in np.unique(obs_array["filter"]):
             in_filt = np.where(obs_array["filter"] == filtername)
             delta_m5 = self.target_m5[filtername] - conditions.M5Depth[filtername][hpids[in_filt]]
-            # We can get NaNs because dithering pushes the center of the pointing into masked regions.
+            # We can get NaNs because dithering pushes the center of the
+            # pointing into masked regions.
             nan_indices = np.argwhere(np.isnan(delta_m5)).ravel()
             for indx in nan_indices:
                 bad_hp = hpids[in_filt][indx]
-                # Note this might fail if we run at higher resolution, then we'd need to look farther for
-                # pixels to interpolate.
+                # Note this might fail if we run at higher resolution,
+                # then we'd need to look farther for pixels to interpolate.
                 near_pix = hp.get_all_neighbours(conditions.nside, bad_hp)
                 vals = conditions.M5Depth[filtername][near_pix]
                 if True in np.isfinite(vals):
                     estimate_m5 = np.mean(vals[np.isfinite(vals)])
                     delta_m5[indx] = self.target_m5[filtername] - estimate_m5
                 else:
                     raise ValueError("Failed to find a nearby unmasked sky value.")
 
             new_expts[in_filt] = conditions.exptime * 10 ** (delta_m5 / 1.25)
         new_expts = np.clip(new_expts, self.min_exp, self.max_exp)
-        # I'm not sure what level of precision we can expect, so let's just limit to seconds
+        # I'm not sure what level of precision we can expect, so let's
+        # just limit to seconds
         new_expts = np.round(new_expts)
 
         for i, observation in enumerate(observation_list):
             observation["exptime"] = new_expts[i]
 
         return observation_list
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/example/example_scheduler.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/example/example_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,16 @@
     season=300.0,
     season_start_hour=-4.0,
     season_end_hour=2.0,
     moon_distance=30.0,
     strict=True,
     wind_speed_maximum=20.0,
 ):
-    """Generate the standard basis functions that are shared by blob surveys
+    """Generate the standard basis functions that are shared by
+    blob surveys
 
     Parameters
     ----------
     nside : int (32)
         The HEALpix nside to use
     nexp : int (1)
         The number of exposures to use in a visit.
@@ -92,38 +93,46 @@
     filtername : list of str
         The filternames for the first set
     filtername2 : list of str
         The filter names for the second in the pair (None if unpaired)
     n_obs_template : dict (None)
         The number of observations to take every season in each filter
     season : float (300)
-        The length of season (i.e., how long before templates expire) (days)
+        The length of season (i.e., how long before templates expire)
+        (days)
     season_start_hour : float (-4.)
-        For weighting how strongly a template image needs to be observed (hours)
+        For weighting how strongly a template image needs to be
+        observed (hours)
     sesason_end_hour : float (2.)
-        For weighting how strongly a template image needs to be observed (hours)
+        For weighting how strongly a template image needs to be
+        observed (hours)
     moon_distance : float (30.)
         The mask radius to apply around the moon (degrees)
     m5_weight : float (3.)
         The weight for the 5-sigma depth difference basis function
     footprint_weight : float (0.3)
         The weight on the survey footprint basis function.
     slewtime_weight : float (3.)
         The weight on the slewtime basis function
     stayfilter_weight : float (3.)
-        The weight on basis function that tries to stay avoid filter changes.
+        The weight on basis function that tries to stay avoid filter
+        changes.
     template_weight : float (12.)
         The weight to place on getting image templates every season
     u_template_weight : float (24.)
-        The weight to place on getting image templates in u-band. Since there
-        are so few u-visits, it can be helpful to turn this up a little higher than
+        The weight to place on getting image templates in u-band. Since
+        there
+        are so few u-visits, it can be helpful to turn this up a little
+        higher than
         the standard template_weight kwarg.
     g_template_weight : float (24.)
-        The weight to place on getting image templates in g-band. Since there
-        are so few g-visits, it can be helpful to turn this up a little higher than
+        The weight to place on getting image templates in g-band. Since
+        there
+        are so few g-visits, it can be helpful to turn this up a little
+        higher than
         the standard template_weight kwarg.
 
     Returns
     -------
     basis_functions_weights : `list`
         list of tuple pairs (basis function, weight) that is
         (rubin_scheduler.scheduler.BasisFunction object, float)
@@ -310,23 +319,27 @@
     filter1s : list of str
         The filternames for the first set
     filter2s : list of str
         The filter names for the second in the pair (None if unpaired)
     pair_time : float (33)
         The ideal time between pairs (minutes)
     camera_rot_limits : list of float ([-80., 80.])
-        The limits to impose when rotationally dithering the camera (degrees).
+        The limits to impose when rotationally dithering the camera
+        (degrees).
     n_obs_template : dict (None)
-        The number of observations to take every season in each filter. If None, sets to 3 each.
+        The number of observations to take every season in each filter.
+        If None, sets to 3 each.
     season : float (300)
         The length of season (i.e., how long before templates expire) (days)
     season_start_hour : float (-4.)
-        For weighting how strongly a template image needs to be observed (hours)
+        For weighting how strongly a template image needs to be observed
+        (hours)
     sesason_end_hour : float (2.)
-        For weighting how strongly a template image needs to be observed (hours)
+        For weighting how strongly a template image needs to be observed
+        (hours)
     shadow_minutes : float (60.)
         Used to mask regions around zenith (minutes)
     max_alt : float (76.
         The maximium altitude to use when masking zenith (degrees)
     moon_distance : float (30.)
         The mask radius to apply around the moon (degrees)
     ignore_obs : str or list of str ('DD')
@@ -334,23 +347,27 @@
     m5_weight : float (3.)
         The weight for the 5-sigma depth difference basis function
     footprint_weight : float (0.3)
         The weight on the survey footprint basis function.
     slewtime_weight : float (3.)
         The weight on the slewtime basis function
     stayfilter_weight : float (3.)
-        The weight on basis function that tries to stay avoid filter changes.
+        The weight on basis function that tries to stay avoid filter
+        changes.
     template_weight : float (12.)
         The weight to place on getting image templates every season
     u_template_weight : float (24.)
-        The weight to place on getting image templates in u-band. Since there
-        are so few u-visits, it can be helpful to turn this up a little higher than
+        The weight to place on getting image templates in u-band. Since
+        there
+        are so few u-visits, it can be helpful to turn this up a little
+        higher than
         the standard template_weight kwarg.
     u_nexp1 : bool (True)
-        Add a detailer to make sure the number of expossures in a visit is always 1 for u observations.
+        Add a detailer to make sure the number of expossures in a visit
+        is always 1 for u observations.
     """
 
     BlobSurvey_params = {
         "slew_approx": 7.5,
         "filter_change_approx": 140.0,
         "read_approx": 2.0,
         "min_pair_time": 15.0,
@@ -518,31 +535,33 @@
     stayfilter_weight=100.0,
     repeat_weight=-1.0,
     footprints=None,
 ):
     """
     Make a quick set of greedy surveys
 
-    This is a convenience function to generate a list of survey objects that can be used with
+    This is a convenience function to generate a list of survey objects
+    that can be used with
     rubin_scheduler.scheduler.schedulers.Core_scheduler.
-    To ensure we are robust against changes in the sims_featureScheduler codebase, all kwargs are
-    explicitly set.
+    To ensure we are robust against changes in the sims_featureScheduler
+    codebase, all kwargs are explicitly set.
 
     Parameters
     ----------
     nside : int (32)
         The HEALpix nside to use
     nexp : int (1)
         The number of exposures to use in a visit.
     exptime : float (30.)
         The exposure time to use per visit (seconds)
     filters : list of str (['r', 'i', 'z', 'y'])
         Which filters to generate surveys for.
     camera_rot_limits : list of float ([-80., 80.])
-        The limits to impose when rotationally dithering the camera (degrees).
+        The limits to impose when rotationally dithering the camera
+        (degrees).
     shadow_minutes : float (60.)
         Used to mask regions around zenith (minutes)
     max_alt : float (76.
         The maximium altitude to use when masking zenith (degrees)
     moon_distance : float (30.)
         The mask radius to apply around the moon (degrees)
     ignore_obs : str or list of str ('DD')
@@ -550,18 +569,20 @@
     m5_weight : float (3.)
         The weight for the 5-sigma depth difference basis function
     footprint_weight : float (0.3)
         The weight on the survey footprint basis function.
     slewtime_weight : float (3.)
         The weight on the slewtime basis function
     stayfilter_weight : float (3.)
-        The weight on basis function that tries to stay avoid filter changes.
+        The weight on basis function that tries to stay avoid filter
+        changes.
     """
     # Define the extra parameters that are used in the greedy survey. I
-    # think these are fairly set, so no need to promote to utility func kwargs
+    # think these are fairly set, so no need to promote to utility func
+    # kwargs
     greed_survey_params = {
         "block_size": 1,
         "smoothing_kernel": None,
         "seed": 42,
         "camera": "LSST",
         "dither": True,
         "survey_name": "greedy",
@@ -672,23 +693,27 @@
     filter1s : list of str
         The filternames for the first set
     filter2s : list of str
         The filter names for the second in the pair (None if unpaired)
     pair_time : float (33)
         The ideal time between pairs (minutes)
     camera_rot_limits : list of float ([-80., 80.])
-        The limits to impose when rotationally dithering the camera (degrees).
+        The limits to impose when rotationally dithering the camera
+        (degrees).
     n_obs_template : Dict (None)
-        The number of observations to take every season in each filter. If None, sets to 3 each.
+        The number of observations to take every season in each filter.
+        If None, sets to 3 each.
     season : float (300)
         The length of season (i.e., how long before templates expire) (days)
     season_start_hour : float (-4.)
-        For weighting how strongly a template image needs to be observed (hours)
+        For weighting how strongly a template image needs to be observed
+        (hours)
     sesason_end_hour : float (2.)
-        For weighting how strongly a template image needs to be observed (hours)
+        For weighting how strongly a template image needs to be observed
+        (hours)
     shadow_minutes : float (60.)
         Used to mask regions around zenith (minutes)
     max_alt : float (76.
         The maximium altitude to use when masking zenith (degrees)
     moon_distance : float (30.)
         The mask radius to apply around the moon (degrees)
     ignore_obs : str or list of str ('DD')
@@ -696,25 +721,30 @@
     m5_weight : float (3.)
         The weight for the 5-sigma depth difference basis function
     footprint_weight : float (0.3)
         The weight on the survey footprint basis function.
     slewtime_weight : float (3.)
         The weight on the slewtime basis function
     stayfilter_weight : float (3.)
-        The weight on basis function that tries to stay avoid filter changes.
+        The weight on basis function that tries to stay avoid filter
+        changes.
     template_weight : float (12.)
         The weight to place on getting image templates every season
     u_template_weight : float (24.)
-        The weight to place on getting image templates in u-band. Since there
-        are so few u-visits, it can be helpful to turn this up a little higher than
+        The weight to place on getting image templates in u-band. Since
+        there
+        are so few u-visits, it can be helpful to turn this up a little
+        higher than
         the standard template_weight kwarg.
     u_nexp1 : bool (True)
-        Add a detailer to make sure the number of expossures in a visit is always 1 for u observations.
+        Add a detailer to make sure the number of expossures in a visit
+        is always 1 for u observations.
     scheduled_respect : float (45)
-        How much time to require there be before a pre-scheduled observation (minutes)
+        How much time to require there be before a pre-scheduled
+        observation (minutes)
     """
 
     BlobSurvey_params = {
         "slew_approx": 7.5,
         "filter_change_approx": 140.0,
         "read_approx": 2.0,
         "min_pair_time": 15.0,
@@ -910,23 +940,28 @@
     filter1s : list of str
         The filternames for the first set
     filter2s : list of str
         The filter names for the second in the pair (None if unpaired)
     pair_time : float (22)
         The ideal time between pairs (minutes)
     camera_rot_limits : list of float ([-80., 80.])
-        The limits to impose when rotationally dithering the camera (degrees).
+        The limits to impose when rotationally dithering the camera
+        (degrees).
     n_obs_template : dict (None)
-        The number of observations to take every season in each filter. If None, sets to 3 each.
+        The number of observations to take every season in each filter.
+        If None, sets to 3 each.
     season : float (300)
-        The length of season (i.e., how long before templates expire) (days)
+        The length of season (i.e., how long before templates expire)
+        (days)
     season_start_hour : float (-4.)
-        For weighting how strongly a template image needs to be observed (hours)
+        For weighting how strongly a template image needs to be observed
+        (hours)
     sesason_end_hour : float (2.)
-        For weighting how strongly a template image needs to be observed (hours)
+        For weighting how strongly a template image needs to be observed
+        (hours)
     shadow_minutes : float (60.)
         Used to mask regions around zenith (minutes)
     max_alt : float (76.
         The maximium altitude to use when masking zenith (degrees)
     moon_distance : float (30.)
         The mask radius to apply around the moon (degrees)
     ignore_obs : str or list of str ('DD')
@@ -938,16 +973,18 @@
     slewtime_weight : float (3.)
         The weight on the slewtime basis function
     stayfilter_weight : float (3.)
         The weight on basis function that tries to stay avoid filter changes.
     template_weight : float (12.)
         The weight to place on getting image templates every season
     u_template_weight : float (24.)
-        The weight to place on getting image templates in u-band. Since there
-        are so few u-visits, it can be helpful to turn this up a little higher than
+        The weight to place on getting image templates in u-band. Since
+        there
+        are so few u-visits, it can be helpful to turn this up a little
+        higher than
         the standard template_weight kwarg.
     """
 
     BlobSurvey_params = {
         "slew_approx": 7.5,
         "filter_change_approx": 140.0,
         "read_approx": 2.0,
@@ -1098,15 +1135,16 @@
     nside : int (32)
         The HEALpix nside to use
     dist_to_eclip : float (40)
         The distance to the ecliptic to constrain to (degrees).
     dec_max : float (30)
         The max declination to alow (degrees).
     mask : np.array (None)
-        Any additional mask to apply, should be a HEALpix mask with matching nside.
+        Any additional mask to apply, should be a HEALpix mask wit
+        matching nside.
     """
 
     ra, dec = _hpid2_ra_dec(nside, np.arange(hp.nside2npix(nside)))
     result = np.zeros(ra.size)
     coord = SkyCoord(ra=ra * u.rad, dec=dec * u.rad)
     eclip_lat = coord.barycentrictrueecliptic.lat.radian
     good = np.where((np.abs(eclip_lat) < np.radians(dist_to_eclip)) & (dec < np.radians(dec_max)))
@@ -1146,46 +1184,50 @@
     time_to_12deg=25.0,
 ):
     """Generate a survey for observing NEO objects in twilight
 
     Parameters
     ----------
     night_pattern : list of bool (None)
-        A list of bools that set when the survey will be active. e.g., [True, False]
+        A list of bools that set when the survey will be active. e.g.,
+        [True, False]
         for every-other night, [True, False, False] for every third night.
     nexp : int (1)
         Number of snaps in a visit
     exptime : float (15)
         Exposure time of visits
     ideal_pair_time : float (5)
         Ideal time between repeat visits (minutes).
     max_airmass : float (2)
         Maximum airmass to attempt (unitless).
     camera_rot_limits : list of float ([-80, 80])
         The camera rotation limits to use (degrees).
     time_needed : float (10)
-        How much time should be available (e.g., before twilight ends) (minutes).
+        How much time should be available (e.g., before twilight ends)
+        (minutes).
     footprint_mask : np.array (None)
         Mask to apply to the constructed ecliptic target mask (None).
     footprint_weight : float (0.1)
         Weight for footprint basis function
     slewtime_weight : float (3.)
         Weight for slewtime basis function
     stayfilter_weight : float (3.)
         Weight for staying in the same filter basis function
     area_required : float (None)
-        The area that needs to be available before the survey will return observations (sq degrees?)
+        The area that needs to be available before the survey will
+        return observations (sq degrees?)
     filters : str ('riz')
         The filters to use, default 'riz'
     n_repeat : int (4)
         The number of times a blob should be repeated, default 4.
     sun_alt_limit : float (-14.8)
         Do not start unless sun is higher than this limit (degrees)
     slew_estimate : float (4.5)
-        An estimate of how long it takes to slew between neighboring fields (seconds).
+        An estimate of how long it takes to slew between neighboring
+        fields (seconds).
     time_to_sunrise : float (25.)
         Do not execute if time to sunrise is greater than (minutes).
     """
     survey_name = "twilight_near_sun"
     footprint = ecliptic_target(nside=nside, mask=footprint_mask)
     constant_fp = ConstantFootprint(nside=nside)
     for filtername in filters:
@@ -1218,15 +1260,16 @@
             (
                 bf.SlewtimeBasisFunction(filtername=filtername, nside=nside),
                 slewtime_weight,
             )
         )
         bfs.append((bf.StrictFilterBasisFunction(filtername=filtername), stayfilter_weight))
         bfs.append((bf.FilterDistBasisFunction(filtername=filtername), filter_dist_weight))
-        # Need a toward the sun, reward high airmass, with an airmass cutoff basis function.
+        # Need a toward the sun, reward high airmass, with an
+        # airmass cutoff basis function.
         bfs.append((bf.NearSunTwilightBasisFunction(nside=nside, max_airmass=max_airmass), 0))
         bfs.append(
             (
                 bf.AltAzShadowMaskBasisFunction(nside=nside, shadow_minutes=shadow_minutes, max_alt=max_alt),
                 0,
             )
         )
@@ -1249,15 +1292,16 @@
             )
         )
 
         # unpack the basis functions and weights
         weights = [val[1] for val in bfs]
         basis_functions = [val[0] for val in bfs]
 
-        # Set huge ideal pair time and use the detailer to cut down the list of observations to fit twilight?
+        # Set huge ideal pair time and use the detailer to cut down
+        # the list of observations to fit twilight?
         surveys.append(
             BlobSurvey(
                 basis_functions,
                 weights,
                 filtername1=filtername,
                 filtername2=None,
                 ideal_pair_time=ideal_pair_time,
@@ -1350,15 +1394,16 @@
     neo_repeat = args.neo_repeat
     ddf_season_frac = args.ddf_season_frac
     neo_am = args.neo_am
     neo_elong_req = args.neo_elong_req
     neo_area_req = args.neo_area_req
     nside = args.nside
 
-    # Be sure to also update and regenerate DDF grid save file if changing mjd_start
+    # Be sure to also update and regenerate DDF grid save file if
+    # changing mjd_start
     mjd_start = 60796.0
     per_night = True  # Dither DDF per night
 
     camera_ddf_rot_limit = 75.0  # degrees
 
     fileroot, extra_info = set_run_info(dbroot=dbroot, file_end="v3.4_", out_dir=out_dir)
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/features/conditions.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/features/conditions.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,107 +4,120 @@
 import warnings
 from io import StringIO
 
 import healpy as hp
 import numpy as np
 import pandas as pd
 
-from rubin_scheduler.scheduler.utils import (
-    match_hp_resolution,
-    season_calc,
-    set_default_nside,
-    smallest_signed_angle,
-)
+from rubin_scheduler.scheduler.utils import match_hp_resolution, set_default_nside, smallest_signed_angle
 from rubin_scheduler.utils import (
     Site,
     _angular_separation,
     _approx_altaz2pa,
     _approx_ra_dec2_alt_az,
     _hpid2_ra_dec,
     calc_lmst,
+    calc_season,
     m5_flat_sed,
+    survey_start_mjd,
 )
 
 
 class Conditions:
-    """
-    Class to hold telemetry information
+    """Holds telemetry information, keeping calculated values in sync
+    for `self.mjd` (such as ra/dec mappings to alt/az).
 
-    If the incoming value is a healpix map, we use a setter to ensure the
-    resolution matches.
+    Incoming values have setters to keep values in sync. Healpix maps
+    are set to the expected (`self.nside`) resolution.
 
     Unless otherwise noted, all values are assumed to be valid at the time
-    given by self.mjd
+    given by `self.mjd`.
+
+    Parameters
+    ----------
+    nside : `int`, optional
+        The healpixel nside to set the resolution of attributes.
+        Default of None will use
+        `rubin_scheduler.scheduler.utils.set_default_nside`.
+    site : str ('LSST')
+        A site name used to create a sims.utils.Site object. For
+        looking up observatory parameters like latitude and longitude.
+    exptime : `float`, optional
+        The exposure time (seconds) to assume when computing the 5-sigma
+        limiting depth maps stored in Conditions. These maps are used
+        by basis functions, but are not used to calculate expected
+        observation m5 values (such as when exposure time varies).
+        Default 30 seconds.
+    mjd_start : `float`, optional
+        The starting MJD of the survey. Default uses
+        `rubin_scheduler.utils.survey_start_date()`.
+    season_map : `np.array`, (N,), optional
+        A HEALpix array that specifies the day offset when computing
+        the season for each HEALpix. Equivalent to season at mjd_start.
+    sun_ra_start : `float`, optional
+        The RA of the sun at the start of the survey (radians)
+    mjd : `float`, optional
+        The current MJD.
+        Default of None is fine on init - will be updated by telemetry
+        stream.
     """
 
     global_maps = set(["ra", "dec", "slewtime", "airmass", "zeros_map", "nan_map"])
     by_band_maps = set(["skybrightness", "fwhm_eff", "m5_depth"])
 
     def __init__(
         self,
         nside=None,
         site="LSST",
         exptime=30.0,
-        mjd_start=59853.5,
-        season_offset=None,
+        mjd_start=survey_start_mjd(),
+        season_map=None,
         sun_ra_start=None,
         mjd=None,
     ):
         """
-        Parameters
-        ----------
-        nside : int
-            The healpixel nside to set the resolution of attributes.
-        site : str ('LSST')
-            A site name used to create a sims.utils.Site object. For looking up
-            observatory paramteres like latitude and longitude.
-        expTime : float (30)
-            The exposure time to assume when computing the 5-sigma limiting depth
-        mjd_start : float (59853.5)
-            The starting MJD of the survey.
-        season_offset : np.array
-            A HEALpix array that specifies the day offset when computing the season for each HEALpix.
-        sun_ra_start : float (None)
-            The RA of the sun at the start of the survey (radians)
-        mjd : float
-            The current MJD.
-
         Attributes (Set on init)
         -----------
         nside : int
             Healpix resolution. All maps are set to this reslution.
         site : rubin_scheduler.Site object ('LSST')
-            Contains static site-specific data (lat, lon, altitude, etc). Defaults to 'LSST'.
+            Contains static site-specific data (lat, lon, altitude, etc).
+            Defaults to 'LSST'.
         ra : np.array
-            A healpix array with the RA of each healpixel center (radians). Automatically
-            generated.
+            A healpix array with the RA of each healpixel center (radians).
+            Automatically generated.
         dec : np.array
-            A healpix array with the Dec of each healpixel center (radians). Automatically generated.
+            A healpix array with the Dec of each healpixel center (radians).
+            Automatically generated.
 
         Attributes (to be set by user/telemetry stream/scheduler)
         -------------------------------------------
         mjd : float
             Modified Julian Date (days).
         bulk_cloud : float
-            The fraction of sky covered by clouds. (In the future might update to transparency map)
+            The fraction of sky covered by clouds. (In the future might
+            update to transparency map)
         cloud_map : np.array
             XXX--to be done. HEALpix array with cloudy pixels set to NaN.
         slewtime : np.array
             Healpix showing the slewtime to each healpixel center (seconds)
         current_filter : str
             The name of the current filter. (expect one of u, g, r, i, z, y).
         mounted_filters : list of str
-            The filters that are currently mounted and thu available (expect 5 of u, g, r, i, z, y)
+            The filters that are currently mounted and thu available
+            (expect 5 of u, g, r, i, z, y)
         night : int
             The current night number (days). Probably starts at 1.
         skybrightness : dict of np.array
-            Dictionary keyed by filtername. Values are healpix arrays with the sky brightness at each
+            Dictionary keyed by filtername. Values are healpix arrays with
+            the sky brightness at each
             healpix center (mag/acsec^2)
         fwhm_eff : dict of np.array
-            Dictionary keyed by filtername. Values are the effective seeing FWHM at each healpix
+            Dictionary keyed by filtername. Values are the effective seeing
+            FWHM at each healpix
             center (arcseconds)
         moon_alt : float
             The altitude of the Moon (radians)
         moon_az : float
             The Azimuth of the moon (radians)
         moon_ra : float
             RA of the moon (radians)
@@ -125,121 +138,157 @@
         tel_dec : float
             The current telescope Declination (radians).
         tel_alt : float
             The current telescope altitude (radians).
         tel_az : float
             The current telescope azimuth (radians).
         cumulative_azimuth_rad : float
-            The cummulative telescope azimuth (radians). For tracking cable wrap
+            The cummulative telescope azimuth (radians). For tracking
+            cable wrap
         cloud_map : np.array
-            A healpix map with the cloud coverage. XXX-expand, is this bool map? Transparency map?
+            A healpix map with the cloud coverage. XXX-expand,
+            is this bool map? Transparency map?
         airmass : np.array
             A healpix map with the airmass value of each healpixel. (unitless)
         wind_speed : float
             Wind speed (m/s).
         wind_direction : float
-            Direction from which the wind originates. A direction of 0.0 degrees
-            means the wind originates from the north and 90.0 degrees from the
-            east (radians).
+            Direction from which the wind originates. A direction of
+            0.0 degrees means the wind originates from the north and 90.0
+            degrees from the east (radians).
         sunset : float
-            The MJD of sunset that starts the current night. Note MJDs of sunset, moonset, twilight times, etc
-            are from interpolations. This means the sun may actually be slightly above/below the horizon
-            at the given sunset time.
+            The MJD of sunset that starts the current night. Note MJDs of
+            sunset, moonset, twilight times, etc are from interpolations.
+            This means the sun may actually be slightly above/below the
+            horizon at the given sunset time.
         sun_n12_setting : float
-            The MJD of when the sun is at -12 degees altitude and setting during the
-            current night. From interpolation.
+            The MJD of when the sun is at -12 degees altitude and
+            setting during the current night. From interpolation.
         sun_n18_setting : float
-            The MJD when the sun is at -18 degrees altitude and setting during the current night.
-            From interpolation.
+            The MJD when the sun is at -18 degrees altitude and setting
+            during the current night. From interpolation.
         sun_n18_rising : float
-            The MJD when the sun is at -18 degrees altitude and rising during the current night.
-            From interpolation.
+            The MJD when the sun is at -18 degrees altitude and rising
+            during the current night. From interpolation.
         sun_n12_rising : float
-            The MJD when the sun is at -12 degrees altitude and rising during the current night.
-            From interpolation.
+            The MJD when the sun is at -12 degrees altitude and rising
+            during the current night. From interpolation.
         sunrise : float
             The MJD of sunrise during the current night. From interpolation
         mjd_start : float
             The starting MJD of the survey.
         moonrise : float
             The MJD of moonrise during the current night. From interpolation.
         moonset : float
             The MJD of moonset during the current night. From interpolation.
-        targets_of_opportunity : list of rubin_scheduler.scheduler.targetoO object(s)
+        moon_phase_sunset : float
+            The phase of the moon (0-100 illuminater) at sunset.
+            Useful for setting which filters should be loaded.
+        targets_of_opportunity : list of rubin_scheduler.scheduler.targetoO
             targetoO objects.
         planet_positions : dict
-            Dictionary of planet name and coordinate e.g., 'venus_RA', 'mars_dec'
+            Dictionary of planet name and coordinate e.g., 'venus_RA',
+            'mars_dec'
         scheduled_observations : np.array
-            A list of MJD times when there are scheduled observations. Defaults to empty array.
+            A list of MJD times when there are scheduled observations.
+            Defaults to empty array.
         tel_az_limits : list of float pairs
-            A list of lists giving valid azimuth ranges. e.g., [0, 2*np.pi] would
-            mean all azimuth values are valid, while [[0, np.pi/2], [3*np.pi/2, 2*np.pi]]
-            would mean anywhere in the south is invalid.  Radians.
+            A list of lists giving valid azimuth ranges. e.g.,
+            [0, 2*np.pi] would mean all azimuth values are valid, while
+            [[0, np.pi/2], [3*np.pi/2, 2*np.pi]] would mean anywhere in
+            the south is invalid.  Radians.
         tel_alt_limits : list of float pairs
             A list of lists giving valid altitude ranges. Radians.
 
         Attributes (calculated on demand and cached)
         ------------------------------------------
         alt : np.array
-            Altitude of each healpixel (radians). Recaclulated if mjd is updated. Uses fast
-            approximate equation for converting RA,Dec to alt,az.
+            Altitude of each healpixel (radians). Recaclulated if mjd is
+            updated. Uses fast approximate equation for converting
+            RA,Dec to alt,az.
         az : np.array
-            Azimuth of each healpixel (radians). Recaclulated if mjd is updated. Uses fast
-            approximate equation for converting RA,Dec to alt,az.
+            Azimuth of each healpixel (radians). Recaclulated if mjd is
+            updated. Uses fast approximate equation for converting RA,Dec
+            to alt,az.
         pa : np.array
-            The parallactic angle of each healpixel (radians). Recaclulated if mjd is updated.
-            Based on the fast approximate alt,az values.
+            The parallactic angle of each healpixel (radians). Recaclulated
+            if mjd is updated. Based on the fast approximate alt,az values.
+        season : `np.array`, (N,)
+            The current season value (0-1) at each healpixel.
+            Recalculated if mjd is updated. Used by features that would
+            otherwise need to calculate `season`.
+            Uses `rubin_scheduler.utils.calc_season`.
         lmst : float
             The local mean sidearal time (hours). Updates is mjd is changed.
         m5_depth : dict of np.array
-            the 5-sigma limiting depth healpix maps, keyed by filtername (mags). Will be recalculated
-            if the skybrightness, seeing, or airmass are updated.
+            the 5-sigma limiting depth healpix maps, keyed by filtername
+            (mags). Will be recalculated if the skybrightness, seeing,
+            or airmass are updated.
         HA : np.array
-            Healpix map of the hour angle of each healpixel (radians). Runs from 0 to 2pi.
+            Healpix map of the hour angle of each healpixel (radians).
+            Runs from 0 to 2pi.
         az_to_sun : np.array
-            Healpix map of the azimuthal distance to the sun for each healpixel (radians)
+            Healpix map of the azimuthal distance to the sun for each
+            healpixel (radians)
         az_to_anitsun : np.array
-            Healpix map of the azimuthal distance to the anit-sun for each healpixel (radians)
+            Healpix map of the azimuthal distance to the anit-sun for each
+            healpixel (radians)
         solar_elongation : np.array
-            Healpix map of the solar elongation (angular distance to the sun) for each healpixel (radians)
+            Healpix map of the solar elongation (angular distance to the sun)
+            for each healpixel (radians)
 
         Attributes (set by the scheduler)
         -------------------------------
         queue : list of observation objects
-            The current queue of observations core_scheduler is waiting to execute.
+            The current queue of observations core_scheduler is waiting to
+            execute.
 
         """
         if nside is None:
             nside = set_default_nside()
         self.nside = nside
+
+        # The RA, Dec grid we are using
+        hpids = np.arange(hp.nside2npix(self.nside))
+        self.ra, self.dec = _hpid2_ra_dec(self.nside, hpids)
+
         self.site = Site(site)
         self.exptime = exptime
+
         self.mjd_start = mjd_start
-        hpids = np.arange(hp.nside2npix(nside))
-        self.season_offset = season_offset
+
+        # Keep these named in both ways, for backwards compatibility for now
+        if season_map is None:
+            season_map = calc_season(np.degrees(self.ra), [self.mjd_start], self.mjd_start).flatten()
+        # season_offset in units of days -useful for season_calc calculations
+        self.season_offset = season_map * 365.25
+        # Season_map is useful for utils.calc_season calculations
+        self.season_map = season_map
+
         self.sun_ra_start = sun_ra_start
+
         # Generate an empty map so we can copy when we need a new map
-        self.zeros_map = np.zeros(hp.nside2npix(nside), dtype=float)
-        self.nan_map = np.zeros(hp.nside2npix(nside), dtype=float)
+        self.zeros_map = np.zeros(hp.nside2npix(self.nside), dtype=float)
+        self.nan_map = np.zeros(hp.nside2npix(self.nside), dtype=float)
         self.nan_map.fill(np.nan)
-        # The RA, Dec grid we are using
-        self.ra, self.dec = _hpid2_ra_dec(nside, hpids)
 
+        # Set other attributes to Nones
         self._init_attributes()
         self.mjd = mjd
 
     def _init_attributes(self):
-        """Initialize all the attributes"""
+        """Initialize or clear all the attributes"""
 
         # Modified Julian Date (day)
         self._mjd = None
         # Altitude and azimuth. Dict with degrees and radians
         self._alt = None
         self._az = None
         self._pa = None
+
         # The cloud level. Fraction, but could upgrade to transparency map
         self.clouds = None
         self._slewtime = None
         self.current_filter = None
         self.mounted_filters = None
         self.night = None
         self._lmst = None
@@ -248,15 +297,15 @@
         self._fwhm_eff = {}
         self._m5_depth = None
         self._airmass = None
 
         self.wind_speed = None
         self.wind_direction = None
 
-        # Upcomming scheduled observations
+        # Upcoming scheduled observations
         self.scheduled_observations = np.array([], dtype=float)
 
         # Attribute to hold the current observing queue
         self.queue = None
 
         # Moon
         self.moon_alt = None
@@ -276,14 +325,15 @@
         self.sun_n12_setting = None
         self.sun_n18_setting = None
         self.sun_n18_rising = None
         self.sun_n12_rising = None
         self.sunrise = None
         self.moonrise = None
         self.moonset = None
+        self.moon_phase_sunset = None
 
         self.planet_positions = None
 
         # Current telescope pointing
         self.tel_ra = None
         self.tel_dec = None
         self.tel_alt = None
@@ -301,20 +351,19 @@
         # XXX--document
         self.bulk_cloud = None
 
         self.rot_tel_pos = None
 
         self.targets_of_opportunity = None
 
+        # self._season tracks the actual current
+        # observing season at each pixel
         self._season = None
-
-        self.season_modulo = None
-        self.season_max_season = None
-        self.season_length = 365.25
-        self.season_floor = True
+        # int_season = np.floor(season)
+        self._int_season = None
 
         # Potential attributes that get computed
         self._solar_elongation = None
         self._az_to_sun = None
         self._az_to_antisun = None
 
     @property
@@ -394,14 +443,30 @@
             self.ra,
             self.dec,
             self.site.latitude_rad,
             self.site.longitude_rad,
             self._mjd,
         )
 
+    @property
+    def season(self):
+        if self._season is None:
+            self.update_season()
+        return self._season
+
+    @property
+    def int_season(self):
+        if self._int_season is None:
+            self.update_season()
+        return self._int_season
+
+    def update_season(self):
+        self._season = self.season_map + (self.mjd - self.mjd_start) / 365.25
+        self._int_season = np.floor(self._season)
+
     @functools.lru_cache(maxsize=10)
     def future_alt_az(self, mjd):
         """Compute the altitude and azimuth for a future time.
 
         Returns
         -------
         altitude : `np.array`
@@ -493,42 +558,14 @@
 
     @property
     def az_to_antisun(self):
         if self._az_to_antisun is None:
             self.calc_az_to_antisun()
         return self._az_to_antisun
 
-    # XXX, there's probably an elegant decorator that could do this caching automatically
-    def season(self, modulo=None, max_season=None, season_length=365.25, floor=True):
-        if self.season_offset is not None:
-            kwargs_match = (
-                (modulo == self.season_modulo)
-                & (max_season == self.season_max_season)
-                & (season_length == self.season_length)
-                & (floor == self.season_floor)
-            )
-            if ~kwargs_match:
-                self.season_modulo = modulo
-                self.season_max_season = max_season
-                self.season_length = season_length
-                self.season_floor = floor
-            if (self._season is None) | (~kwargs_match):
-                self._season = season_calc(
-                    self.night,
-                    offset=self.season_offset,
-                    modulo=modulo,
-                    max_season=max_season,
-                    season_length=season_length,
-                    floor=floor,
-                )
-        else:
-            self._season = None
-
-        return self._season
-
     def __repr__(self):
         return f"<{self.__class__.__name__} mjd_start='{self.mjd_start}' at {hex(id(self))}>"
 
     def __str__(self):
         # If dependencies of to_markdown are not installed, fall back on repr
         try:
             pd.DataFrame().to_markdown()
@@ -566,18 +603,14 @@
             None if self.queue is None else len(self.queue),
             "  ",
             file=output,
         )
         print("moonPhase: ", self.moon_phase, "  ", file=output)
         print("bulk_cloud: ", self.bulk_cloud, "  ", file=output)
         print("targets_of_opportunity: ", self.targets_of_opportunity, "  ", file=output)
-        print("season_modulo: ", self.season_modulo, "  ", file=output)
-        print("season_max_season: ", self.season_max_season, "  ", file=output)
-        print("season_length: ", self.season_length, "  ", file=output)
-        print("season_floor: ", self.season_floor, "  ", file=output)
         print("cumulative_azimuth_rad: ", self.cumulative_azimuth_rad, "  ", file=output)
 
         positions = [
             {
                 "name": "sun",
                 "alt": self.sun_alt,
                 "az": self.sun_az,
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/features/features.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/features/features.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,117 +17,201 @@
     "NObservationsCurrentSeason",
     "LastNObsTimes",
     "SurveyInNight",
     "NoteInNight",
     "NoteLastObserved",
 )
 
+import warnings
+
 import healpy as hp
 import numpy as np
 from scipy.stats import binned_statistic
 
 from rubin_scheduler.scheduler import utils
 from rubin_scheduler.scheduler.utils import IntRounded
 from rubin_scheduler.skybrightness_pre import dark_sky
-from rubin_scheduler.utils import _hpid2_ra_dec, calc_season, m5_flat_sed, ra_dec2_hpid
+from rubin_scheduler.utils import _hpid2_ra_dec, calc_season, m5_flat_sed, survey_start_mjd
+
+
+def send_unused_deprecation_warning(name):
+    message = (
+        f"The feature {name} is not in use by the current "
+        "baseline scheduler and may be deprecated shortly. "
+        "Please contact the rubin_scheduler maintainers if "
+        "this is in use elsewhere."
+    )
+    warnings.warn(message, FutureWarning)
 
 
 class BaseFeature:
-    """
-    Base class for features.
+    """The base class for features.
+    This defines the standard API: a Feature should include
+    a `self.feature` attribute, which could be a float, bool,
+    or healpix size numpy array, or numpy masked array, and a
+    __call__ method which returns `self.feature`.
     """
 
     def __init__(self, **kwargs):
-        # self.feature should be a float, bool, or healpix size numpy array, or numpy masked array
+        # self.feature should be a float, bool, or healpix size numpy
+        # array, or numpy masked array
         self.feature = None
 
     def __call__(self):
         return self.feature
 
 
 class BaseSurveyFeature(BaseFeature):
-    """
-    Feature that tracks progreess of the survey.
-    Takes observations and updates self.feature
+    """Track information relevant to the progress of a survey, using
+    `self.feature` to hold this information.
+
+    Features can track a single piece of information, or keep a map across
+    the sky, or any other piece of information.
+
+    Information in `self.feature` is updated via `add_observation` or
+    `add_observation_array`.
     """
 
     def add_observations_array(self, observations_array, observations_hpid):
-        """ """
+        """Update self.feature based on information in `observations_array`
+        and `observations_hpid`.
+
+        This is a method to more rapidly restore the feature to its
+        expected state, by using an array of all previous observations
+        (`observations_array`) instead looping over the individual
+        observations, as in `self.add_observation`. The observations array
+        allows rapid calculation of acceptable observations, without
+        considering factors such as which healpix is relevant.
+
+        The `observations_hpid` is a reorganized version of the
+        `observations_array`, where the array representing each observation
+        is extended to include `hpid` and recorded multiple times (for each
+        healpixel). The `observations_hpid` allows rapid calculation of
+        feature values which depend on hpid.
+
+        Links between `observations_array` and `observations_hpid` can
+        be made using `ID`.
+        """
         print(self)
         raise NotImplementedError
 
     def add_observation(self, observation, indx=None, **kwargs):
-        """
+        """Update self.feature based on information in `observation`.
+        Observations should be ordered in monotonically increasing time.
+
         Parameters
         ----------
-        obsevation : dict-like
-            Object that contains the information about the observation
-            (ra, dec, filter, mjd, etc)
+        observation : `np.array`, (1,N)
+            Array of observation information, containing
+            `mjd` for the time. See
+            `rubin_scheduler.scheduler.utils.empty_observation`.
         indx : `list`-like of [`int`]
             The healpixel indices that the observation overlaps.
+            See `rubin_scheduler.utils.HpInLsstFov`.
         """
         raise NotImplementedError
 
 
 class SurveyInNight(BaseSurveyFeature):
-    """Keep track of how many times a survey has executed in a night."""
+    """Count appearances of `survey_str` within observation `note` in
+    the current night; `survey_str` must be contained in `note`.
+
+    Useful to keep track of how many times a survey has executed in a night.
+
+    Parameters
+    ----------
+    survey_str : `str`, optional
+        String to search for in observation `note`.
+        String does not have to match `note` exactly,
+        just be contained in `note`.
+        Default of "" means any observation will match.
+    """
 
     def __init__(self, survey_str=""):
         self.feature = 0
         self.survey_str = survey_str
-        self.night = -1
+        self.night = -100
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def add_observation(self, observation, indx=None):
         if observation["night"] != self.night:
             self.night = observation["night"]
             self.feature = 0
 
         if self.survey_str in observation["note"]:
             self.feature += 1
 
 
 class NoteInNight(BaseSurveyFeature):
-    """How many times a matching note has executed in the current night."""
+    """Count appearances of any of `notes` in observation `note` in the
+    current night; `note` must match one of `notes` exactly.
+
+    Useful for keeping track of how many times a survey or other subset
+    of visits has executed in a given night.
+
+    Parameters
+    ----------
+    notes : `list` [`str`], optional
+        List of strings to match against observation `note` values.
+        The `note` must match one of the items in notes exactly.
+        Default of None uses `[]` and will match any note.
+    """
 
-    def __init__(self, notes=[]):
+    def __init__(self, notes=None):
         self.feature = 0
+        if notes is None:
+            notes = []
         self.notes = notes
         self.current_night = -100
 
     def add_observations_array(self, observations_array, observations_hpid):
+        # Identify the most recent night.
         if self.current_night != observations_array["night"][-1]:
             self.current_night = observations_array["night"][-1].copy()
             self.feature = 0
+        # Identify observations within this night.
         indx = np.where(observations_array["night"] == observations_array["night"][-1])[0]
+        # Count observations that match notes.
         for ind in indx:
             if observations_array["note"][ind] in self.notes:
                 self.feature += 1
 
     def add_observation(self, observation, indx=None):
         if self.current_night != observation["night"]:
             self.current_night = observation["night"].copy()
             self.feature = 0
         if observation["note"] in self.notes:
             self.feature += 1
 
 
 class NObsCount(BaseSurveyFeature):
-    """Count the number of observations. Total number, not tracked over sky
+    """Count the number of observations.
+    Total number, not tracked over sky
 
     Parameters
     ----------
     filtername : `str` (None)
         The filter to count (if None, all filters counted)
+
     """
 
     def __init__(self, filtername=None, tag=None):
         self.feature = 0
         self.filtername = filtername
-        # XXX--is "tag" actually used anywhere? Maybe should remove that.
+        # 'tag' is used in GoalStrictFilterBasisFunction
         self.tag = tag
+        if self.tag is not None:
+            warnings.warn(
+                "Tag is not a supported element"
+                "of the `observation` and this aspect of "
+                "the feature will be "
+                "deprecated in 2 minor releases.",
+                DeprecationWarning,
+                stack_level=2,
+            )
 
     def add_observations_array(self, observations_array, observations_hpid):
         if self.filtername is None:
             self.feature += np.size(observations_array)
         else:
             in_filt = np.where(observations_array["filter"] == self.filtername)[0]
             self.feature += np.size(in_filt)
@@ -154,20 +238,26 @@
             (observation["filter"][0] in self.filtername)
             and (observation["tag"][0] in self.tag)
         ):
             self.feature += 1
 
 
 class NObsCountSeason(BaseSurveyFeature):
-    """Count the number of observations.
+    """Count the number of observations in a season.
 
     Parameters
     ----------
     filtername : `str` (None)
         The filter to count (if None, all filters counted)
+
+    Notes
+    -----
+    Uses `season_calc` to calculate season value.
+
+    Seems unused - added deprecation warning.
     """
 
     def __init__(
         self,
         season,
         nside=None,
         filtername=None,
@@ -184,14 +274,15 @@
         self.season_modulo = season_modulo
         if offset is None:
             self.offset = np.zeros(hp.nside2npix(nside), dtype=int)
         else:
             self.offset = offset
         self.max_season = max_season
         self.season_length = season_length
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def add_observation(self, observation, indx=None):
         season = utils.season_calc(
             observation["night"],
             modulo=self.season_modulo,
             offset=self.offset[indx],
             max_season=self.max_season,
@@ -211,28 +302,29 @@
             elif (self.filtername is None) and (self.tag is not None) and (observation["tag"][0] in self.tag):
                 # Track all observations on a specified tag
                 self.feature += 1
             elif (
                 (self.filtername is None)
                 and (self.tag is not None)
                 and
-                # Track all observations on a specified filter on a specified tag
+                # Track all observations on a specified filter on a
+                # specified tag
                 (observation["filter"][0] in self.filtername)
                 and (observation["tag"][0] in self.tag)
             ):
                 self.feature += 1
 
 
 class NObsSurvey(BaseSurveyFeature):
-    """Count the number of observations.
+    """Count the number of observations, whole sky (not per pixel).
 
     Parameters
     ----------
     note : `str` (None)
-        Only count observations that have str in their note field
+        Only count observations that contain str in their note field
     """
 
     def __init__(self, note=None):
         self.feature = 0
         self.note = note
 
     def add_observation(self, observation, indx=None):
@@ -241,24 +333,27 @@
             self.feature += 1
         else:
             if self.note in observation["note"]:
                 self.feature += 1
 
 
 class LastObservation(BaseSurveyFeature):
-    """Track the last observation. Useful if you want to see when the
+    """Track the last observation.
+    Useful if you want to see when the
     last time a survey took an observation.
 
     Parameters
     ----------
     survey_name : `str` (None)
         Only records if the survey name matches (or survey_name set to None)
     """
 
     def __init__(self, survey_name=None):
+        # Will this work for observations read from a database???
+        # "note" is definitely NOT guaranteed to match the survey_name.
         self.survey_name = survey_name
         # Start out with an empty observation
         self.feature = utils.empty_observation()
 
     def add_observations_array(self, observations_array, observations_hpid):
         if self.survey_name is not None:
             good = np.where(observations_array["note"] == self.survey_name)[0]
@@ -276,15 +371,16 @@
             self.feature = observation
 
 
 class LastsequenceObservation(BaseSurveyFeature):
     """When was the last observation"""
 
     def __init__(self, sequence_ids=""):
-        self.sequence_ids = sequence_ids  # The ids of all sequence observations...
+        self.sequence_ids = sequence_ids  # The ids of all sequence
+        # observations...
         # Start out with an empty observation
         self.feature = utils.empty_observation()
 
     def add_observation(self, observation, indx=None):
         if observation["survey_id"] in self.sequence_ids:
             self.feature = observation
 
@@ -339,21 +435,14 @@
         if np.size(data) > 0:
             result, _be, _bn = binned_statistic(
                 data["hpid"], np.ones(data.size), statistic=np.sum, bins=self.bins
             )
             self.feature += result
 
     def add_observation(self, observation, indx=None):
-        """
-        Parameters
-        ----------
-        indx : `list`-like of [`int`]
-            The indices of the healpixel map that have been observed by observation
-        """
-
         if self.filtername is None or observation["filter"][0] in self.filtername:
             if self.survey_name is None or observation["note"] in self.survey_name:
                 self.feature[indx] += 1
 
 
 class NObservationsSeason(BaseSurveyFeature):
     """
@@ -367,14 +456,18 @@
         String or list that has all the filters that can count.
     nside : `int` (32)
         The nside of the healpixel map to use
     offset : `int` (0)
         The offset to use when computing the season (days)
     modulo : `int` (None)
         How to mod the years when computing season
+
+    Notes
+    -----
+    Uses `season_calc` to calculate season value.
     """
 
     def __init__(
         self,
         season,
         filtername=None,
         nside=None,
@@ -386,28 +479,25 @@
         if offset is None:
             offset = np.zeros(hp.nside2npix(nside), dtype=int)
         if nside is None:
             nside = utils.set_default_nside()
 
         self.feature = np.zeros(hp.nside2npix(nside), dtype=float)
         self.filtername = filtername
+        ## How does this work if the default is 0 -- in add_observation
+        # an index is referenced for offset, so the default should fail
         self.offset = offset
         self.modulo = modulo
         self.season = season
         self.max_season = max_season
         self.season_length = season_length
+        send_unused_deprecation_warning(self.__class__.__name__)
 
     def add_observation(self, observation, indx=None):
-        """
-        Parameters
-        ----------
-        indx :`list`-like of [`int`]
-            The indices of the healpixel map that have been observed by observation
-        """
-
+        # How does this work if indx is None -- self.offset[indx] should fail
         observation_season = utils.season_calc(
             observation["night"],
             offset=self.offset[indx],
             modulo=self.modulo,
             max_season=self.max_season,
             season_length=self.season_length,
         )
@@ -455,131 +545,255 @@
     def add_observation(self, observation, indx=None):
         if self.filtername is None or observation["filter"][0] in self.filtername:
             self.feature[0:-1, indx] = self.feature[1:, indx]
             self.feature[-1, indx] = observation["mjd"]
 
 
 class NObservationsCurrentSeason(BaseSurveyFeature):
-    """Track how many observations have been taken in the current season
-    that meet criteria.
+    """Count the observations at each healpix, taken in the most
+    recent season, that meet filter, seeing and m5 criteria.
+
+    Useful for ensuring that "good quality" observations are acquired
+    in each season at each point in the survey footprint.
+
+    Parameters
+    ----------
+    filtername : `str`, optional
+        If None (default) count observations in any filter.
+        Otherwise, only count observations in the specified filter.
+    nside : `int`, optional
+        If None (default), use default nside for scheduler.
+        Otherwise, set nside for the map to nside.
+    seeing_fwhm_max : `float`, optional
+        If None (default), count observations up to any seeing value.
+        Otherwise, only count observations with better seeing (`FWHMeff`)
+        than `seeing_fwhm_max`. In arcseconds.
+    m5_penalty_max : `float`, optional
+        If None (default), count observations with any m5 value.
+        Otherwise, only count observations within this value of the
+        dark sky map at this pixel.
+        Only relevant if filtername is not None.
+    mjd_start : `float`, optional
+        If None, uses default survey_start_mjd for the start of the survey.
+        This defines the starting year for counting seasons, so should
+        be the start of the survey.
     """
 
     def __init__(
         self,
         filtername=None,
         nside=None,
         seeing_fwhm_max=None,
         m5_penalty_max=None,
-        mjd_start=1,
+        mjd_start=None,
     ):
-        self.filtername = filtername
         if nside is None:
-            self.nside = utils.set_default_nside()
-        else:
-            self.nside = nside
+            nside = utils.set_default_nside()
+        self.nside = nside
         self.seeing_fwhm_max = seeing_fwhm_max
+        self.filtername = filtername
         self.m5_penalty_max = m5_penalty_max
+        # If filtername not set, then we can't set m5_penalty_max.
+        if self.filtername is None and self.m5_penalty_max is not None:
+            warnings.warn("To use m5_penalty_max, filtername must be set. Disregarding m5_penalty_max.")
+            self.m5_penalty_max = None
 
-        self.feature = np.zeros(hp.nside2npix(nside), dtype=float)
+        # Get the dark sky map
         if self.filtername is not None:
             self.dark_map = dark_sky(nside)[filtername]
         self.ones = np.ones(hp.nside2npix(self.nside))
+
+        if mjd_start is None:
+            mjd_start = survey_start_mjd()
+        self.mjd_start = mjd_start
+
+        # Set up feature values - this includes the count in a given season
+        # Find the healpixels for each point on the sky
         self.ra, self.dec = _hpid2_ra_dec(nside, np.arange(hp.nside2npix(nside)))
-        self.season_map = calc_season(np.degrees(self.ra), mjd_start)
+        self.ra_deg = np.degrees(self.ra)
+
+        self.mjd = mjd_start
+        # Set up season_map. This should be the same as conditions.season_map
+        # but the important thing is that mjd_start matches.
+        self.season_map = calc_season(self.ra_deg, [self.mjd], self.mjd_start).flatten()
+        self.season = np.floor(self.season_map)
+
+        self.feature = np.zeros(hp.nside2npix(nside), dtype=float)
+        # Set bins for add_observations_array
         self.bins = np.arange(hp.nside2npix(nside) + 1) - 0.5
 
     def season_update(self, observation=None, conditions=None):
-        """clear the map anywhere the season has rolled over"""
+        """Update the season_map to the current time.
+
+        This assumes time increases monotonically in the conditions or
+        observations objects passed as arguments.
+        Using the 'mjd' from the conditions, where parts of the sky
+        have changed season (increasing in the `self.season_map` + 1)
+        the `self.feature` is cleared, in order to restart counting
+        observations in the new season.
+
+        Parameters
+        ----------
+        observation : `np.array`, (1,N)
+            Array of observation information, containing
+            `mjd` for the time. See
+            `rubin_scheduler.scheduler.utils.empty_observation`.
+        conditions : `rubin_scheduler.scheduler.Conditions`, optional
+            A conditions object, containing `mjd`.
+
+        Notes
+        -----
+        One of observations or conditions must be passed, but either
+        are options so this can be used with add_observation.
+        Most of the time, the updates will come from `conditions`.
+        """
+        mjd_now = None
+        mjd_from = None
         if observation is not None:
-            current_season = calc_season(np.degrees(self.ra), observation["mjd"])
+            mjd_now = observation["mjd"]
+            mjd_from = "observation"
+        # Prefer to use Conditions for the time.
         if conditions is not None:
-            current_season = calc_season(np.degrees(self.ra), conditions.mjd)
-
-        # If the season has changed anywhere, set that count to zero
-        new_season = np.where((self.season_map - current_season) != 0)
-        self.feature[new_season] = 0
-        self.season_map = current_season
+            mjd_now = conditions.mjd
+            mjd_from = "conditions"
+        if mjd_now is None:
+            warnings.warn(
+                "Expected either a conditions or observations object. Not updating season_map.",
+                UserWarning,
+            )
+            return
+        if isinstance(mjd_now, np.ndarray) or isinstance(mjd_now, list):
+            mjd_now = mjd_now[0]
+        # Check that time doesn't go backwards.
+        # But only bother to warn if it's coming from conditions.
+        # Observations may look like they go backwards.
+        if mjd_now < self.mjd:
+            if mjd_from == "conditions":
+                warnings.warn(
+                    f"Time must flow forwards to track the "
+                    f"feature in {self.__class__.__name__}."
+                    f"Not updating season_map.",
+                    UserWarning,
+                )
+            # But just return without update in either case.
+            return
+        # Calculate updated season values.
+        updated_season = np.floor(self.season_map + (mjd_now - self.mjd_start) / 365.25)
+        # Clear feature where season increased by 1 (note 'floor' above).
+        self.feature[np.where(updated_season > self.season)] = 0
+        # Update to new time and season.
+        self.mjd = mjd_now
+        self.season = updated_season
 
     def add_observations_array(self, observations_array, observations_hpid):
+        # Update self.season to the most recent observation time
         self.season_update(observation=observations_array[-1])
 
-        check1 = np.zeros(observations_array.size, dtype=bool)
-        if self.seeing_fwhm_max is not None:
-            check1[np.where(observations_array["FWHMeff"] <= self.seeing_fwhm_max)] = True
-        else:
-            check1[:] = True
-
-        check2 = np.zeros(observations_array.size, dtype=bool)
-        if self.m5_penalty_max is not None:
-            hpid = ra_dec2_hpid(self.nside, observations_array["RA"], observations_array["dec"])
-            penalty = self.dark_map[hpid] - observations_array["fivesigmadepth"]
-            check2[np.where(penalty <= self.m5_penalty_max)] = True
-        else:
-            check2[:] = True
+        # Start assuming 'check' is all True, for all observations.
+        check = np.ones(observations_array.size, dtype=bool)
 
-        if self.filtername is None:
-            check3 = np.zeros(observations_array.size, dtype=bool)
-            check3[np.where(observations_array["filter"] == self.filter)] = True
-        else:
-            check3 = np.ones(observations_array.size, dtype=bool)
+        # Rule out the observations with seeing fwhmeff > limit
+        if self.seeing_fwhm_max is not None:
+            check[np.where(observations_array["FWHMeff"] > self.seeing_fwhm_max)] = False
 
-        good_ids = observations_array[check1 & check2 % check3]["ID"]
+        # Rule out observations which are not in the desired filter
+        if self.filtername is not None:
+            check[np.where(observations_array["filter"] != self.filtername)] = False
 
-        indx = np.in1d(observations_hpid["ID"], observations_array["ID"][good_ids])
+        # Convert the "check" array on observations_array into a
+        # "check" array on the hpids so we can evaluate healpix-level items
+        check_hpid_indxs = np.in1d(observations_hpid["ID"], observations_array["ID"][check])
+        # Set up a new valid/not valid flag, now on observations_hpid
+        check_hp = np.zeros(len(observations_hpid), dtype=bool)
+        # Set all observations which passed simpler tests above to True
+        check_hp[check_hpid_indxs] = True
+
+        hpids = observations_hpid["hpid"]
+
+        # This could be done once per observation, but to make life
+        # easier for index matching, let's just calculate season
+        # based on the hpid array.
+        # We only want to count observations that would fall within the
+        # current season, so calculate the season for each obs.
+        seasons = np.floor(
+            calc_season(
+                np.degrees(observations_hpid["RA"]),
+                observations_hpid["mjd"],
+                self.mjd_start,
+                calc_diagonal=True,
+            )
+        )
+        season_change = self.season[hpids] - seasons
+        check_hp = np.where(season_change != 0, False, check_hp)
+        # And check for m5_penalty_map
+        if self.m5_penalty_max is not None:
+            penalty = self.dark_map[hpids] - observations_hpid["fivesigmadepth"]
+            check_hp = np.where(penalty > self.m5_penalty_max, False, check_hp)
 
+        # Bin up the observations per hpid and add them to the feature.
         result, _be, _bn = binned_statistic(
-            observations_hpid["hpid"][indx],
-            observations_hpid["hpid"][indx],
+            observations_hpid["hpid"][check_hp],
+            observations_hpid["hpid"][check_hp],
             bins=self.bins,
             statistic=np.size,
         )
+        # Add the resulting observations to feature.
         self.feature += result
 
-    def add_observation(self, observation, indx=None):
+    def add_observation(self, observation, indx):
+        # Update the season map to the current time.
         self.season_update(observation=observation)
+        # Check if *this* observation is in the current season
+        # (This means we could add observations from the past, but
+        # would count it against the current season).
+        season_obs = np.floor(self.season_map[indx] + (observation["mjd"] - self.mjd_start) / 365.25)
+        this_season_indx = np.array(indx)[np.where(season_obs == self.season[indx])]
 
+        # Check if seeing is good enough.
         if self.seeing_fwhm_max is not None:
-            check1 = observation["FWHMeff"] <= self.seeing_fwhm_max
+            check = observation["FWHMeff"] <= self.seeing_fwhm_max
         else:
-            check1 = True
+            check = True
 
-        if self.m5_penalty_max is not None:
-            hpid = ra_dec2_hpid(self.nside, observation["RA"], observation["dec"])
-            penalty = self.dark_map[hpid] - observation["fivesigmadepth"]
-            check2 = penalty <= self.m5_penalty_max
-        else:
-            check2 = True
+        # Check if observation is in the right filter
+        if self.filtername is not None and check:
+            if observation["filter"] != self.filtername:
+                check = False
+            else:
+                # Check if observation in correct filter and deep enough.
+                if self.m5_penalty_max is not None:
+                    penalty = self.dark_map[this_season_indx] - observation["fivesigmadepth"]
+                    this_season_indx = this_season_indx[np.where(penalty <= self.m5_penalty_max)]
 
-        if check1 & check2:
-            if self.filtername is None or observation["filter"][0] in self.filtername:
-                self.feature[indx] += 1
+        if check:
+            self.feature[this_season_indx] += 1
 
 
 class CoaddedDepth(BaseSurveyFeature):
     """Track the co-added depth that has been reached across the sky
 
     Parameters
     ----------
     fwh_meff_limit : `float` (100)
         The effective FWHM of the seeing (arcsecond).
-        Images will only be added to the coadded depth if the observation FWHM
-        is less than or equal to the limit.  Default 100.
+        Images will only be added to the coadded depth if the observation
+        FWHM is less than or equal to the limit.  Default 100.
     """
 
-    def __init__(self, filtername="r", nside=None, fwh_meff_limit=100.0):
+    def __init__(self, filtername="r", nside=None, fwhm_eff_limit=100.0):
         if nside is None:
             nside = utils.set_default_nside()
         self.filtername = filtername
-        self.fwh_meff_limit = IntRounded(fwh_meff_limit)
+        self.fwhm_eff_limit = IntRounded(fwhm_eff_limit)
         # Starting at limiting mag of zero should be fine.
         self.feature = np.zeros(hp.nside2npix(nside), dtype=float)
 
     def add_observation(self, observation, indx=None):
         if observation["filter"] == self.filtername:
-            if IntRounded(observation["FWHMeff"]) <= self.fwh_meff_limit:
+            if IntRounded(observation["FWHMeff"]) <= self.fwhm_eff_limit:
                 m5 = m5_flat_sed(
                     observation["filter"],
                     observation["skybrightness"],
                     observation["FWHMeff"],
                     observation["exptime"],
                     observation["airmass"],
                 )
@@ -693,25 +907,28 @@
         self.filtername = filtername
         self.feature = np.zeros(hp.nside2npix(nside), dtype=float)
         self.indx = np.arange(self.feature.size)
         self.last_observed = LastObserved(filtername=filtername)
         self.gap_min = IntRounded(gap_min / (24.0 * 60))  # Days
         self.gap_max = IntRounded(gap_max / (24.0 * 60))  # Days
         self.night = 0
-        # Need to keep a full record of times and healpixels observed in a night.
+        # Need to keep a full record of times and healpixels observed in
+        # a night.
         self.mjd_log = []
         self.hpid_log = []
 
     def add_observations_array(self, observations_array, observations_hpid):
-        # ok, let's just find the largest night and toss all those in one at a time
+        # ok, let's just find the largest night and toss all those in one
+        # at a time
         most_recent_night = np.where(observations_hpid["night"] == np.max(observations_hpid["night"]))[0]
         obs_hpid = observations_hpid[most_recent_night]
         uid = np.unique(obs_hpid["ID"])
         for ind_id in uid:
-            # maybe a faster searchsorted way to do this, but it'll work for now
+            # maybe a faster searchsorted way to do this, but it'll work
+            # for now
             good = np.where(obs_hpid["ID"] == ind_id)[0]
             self.add_observation(observations_hpid[good][0], observations_hpid[good]["hpid"])
 
     def add_observation(self, observation, indx=None):
         if self.filtername is None:
             infilt = True
         else:
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/model_observatory/generate_almanac.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/model_observatory/generate_almanac.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/model_observatory/generate_altitudes.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/model_observatory/generate_altitudes.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,16 @@
         The starting mjd
     duration : float (3653)
         How long to compute times for (days)
     rough_step : float (2.)
         Time step for computing first pass rough sunrise times (hours)
     """
 
-    # Let's find the nights first, find the times where the sun crosses the meridian.
+    # Let's find the nights first, find the times where the sun crosses
+    # the meridian.
     site = Site("LSST")
     location = EarthLocation(lat=site.latitude, lon=site.longitude, height=site.height)
     # go on 1/10th of a day steps
     t_step = rough_step / 24.0
     pad_around = 30.0 / 24.0
     t_sparse = Time(
         np.arange(mjd_start - pad_around, duration + mjd_start + pad_around + t_step, t_step),
@@ -199,16 +200,18 @@
     # I could do another seatchsorted pass here just
     # to be extra sure nothing changed.
 
     return alt_info_array, refined_mjds
 
 
 if __name__ == "__main__":
-    # Let's use astropy to pre-compute the sunrise/sunset/twilight/moonrise/moonset times we're interested in.
+    # Let's use astropy to pre-compute the
+    # sunrise/sunset/twilight/moonrise/moonset times we're interested in.
     mjd_start = 59853.5
     #
     rough_times, refined_mjds = generate_nights(
         mjd_start - 365.25 * 2 - 40.0, duration=365.25 * 24 + 80, rough_step=2
     )
-    # rough_times, refined_mjds = generate_nights(mjd_start, duration=50, rough_step=2)
+    # rough_times, refined_mjds = generate_nights(mjd_start, duration=50,
+    # rough_step=2)
     # Maybe just use pandas to dump it to a csv file?
     np.savez("night_info.npz", rough_times=rough_times, refined_mjds=refined_mjds)
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/model_observatory/jerk.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/model_observatory/jerk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 __all__ = ("jerk_time", "acc_time")
 
 import numpy as np
 
 
 def jerk_time(distance, v_max, acc_max, jerk_max):
-    """Calculate how long to move a distance given maximum jerk, acceleration, and velocity
+    """Calculate how long to move a distance given maximum jerk,
+    acceleration, and velocity
 
-    All parameters are assumed to be symetric (e.g, minimum jerk = -1*jerk_max)
+    All parameters are assumed to be symetric
+    (e.g, minimum jerk = -1*jerk_max)
 
-    modified from https://github.com/mdhom/py_constant_jerk/blob/main/constantJerk.py
+    modified from https://github.com/mdhom/py_constant_jerk/blob/main/
+    constantJerk.py
     see also:
-    https://www.researchgate.net/publication/289374755_THIRD_ORDER_POINT-TO-POINT_MOTION_-PROFILE
+    https://www.researchgate.net/publication/
+    289374755_THIRD_ORDER_POINT-TO-POINT_MOTION_-PROFILE
 
     Parameters
     ----------
     distance : `float`
-        The distance to travel. Could be units of length or angle as long as other
-        parameters match.
+        The distance to travel. Could be units of length or angle as long
+        as other parameters match.
     v_max : `float`
         The maximum velocity. Units of length or angle per unit of time
     acc_max : `float`
-        The maximum acceleration. Units of length or angle per unit of time squared.
+        The maximum acceleration. Units of length or angle per unit of
+        time squared.
     jerk_max : `float`
-        The maximum jerk. Units of length or angle per unit of time cubed. If
-        set to None, assumes jerk is infinite and defaults to use acc_time.
+        The maximum jerk. Units of length or angle per unit of time cubed.
+        If set to None, assumes jerk is infinite and defaults to use
+        acc_time.
     """
 
     # If distance is a scalar, convert to array.
     distance = np.atleast_1d(distance)
 
     # If there is no jerk, fall back on infinite jerk approximation
     if jerk_max is None:
@@ -59,26 +65,28 @@
             )
             result[indx] = tv + tj + ta
 
     return result
 
 
 def acc_time(distance, v_max, acc_max):
-    """Time to move given a maximum velocity and acceleration. Assumes infinite jerk.
-    Velocity and accelerations are assumed to be symetric (minimum acceleration = -1* acc_max)
+    """Time to move given a maximum velocity and acceleration. Assumes
+    infinite jerk. Velocity and accelerations are assumed to be
+    symetric (minimum acceleration = -1* acc_max)
 
     Parameters
     ----------
     distance : `float`
-        The distance to travel. Could be units of length or angle as long as other
-        parameters match.
+        The distance to travel. Could be units of length or angle as long
+        as other parameters match.
     v_max : `float`
         The maximum velocity. Units of length or angle per unit of time
     acc_max : `float`
-        The maximum acceleration. Units of length or angle per unit of time squared.
+        The maximum acceleration. Units of length or angle per unit of
+        time squared.
     """
 
     distance = np.atleast_1d(distance)
 
     dm = v_max**2 / acc_max
     slew_time = np.where(
         distance < dm,
@@ -87,15 +95,16 @@
     )
     return slew_time
 
 
 def _calculate_times(distance, v_max, acc_max, jerk_max, trajectory_instance_case=1):
     """Calculate travel time including jerk.
 
-    Modified from https://github.com/mdhom/py_constant_jerk/blob/main/constantJerk.py
+    Modified from https://github.com/mdhom/py_constant_jerk/blob/main/
+    #constantJerk.py
     """
     if trajectory_instance_case == 1 or trajectory_instance_case == 3:
         tj = np.sqrt(v_max / jerk_max)
         ta = tj
         tv = distance / v_max
         return tj, ta, tv
     elif trajectory_instance_case == 2 or trajectory_instance_case == 4:
@@ -122,40 +131,44 @@
     else:
         raise Exception("TrajectoryInstance must be between 1 and 6")
 
 
 def _get_trajectory_instance_case(distance, v_max, acc_max, jerk_max):
     """Determine which motion profile to use.
 
-    Modified from https://github.com/mdhom/py_constant_jerk/blob/main/constantJerk.py
+    Modified from https://github.com/mdhom/py_constant_jerk/blob/main/
+    constantJerk.py
     which was probably derived from:
-    https://www.researchgate.net/publication/289374755_THIRD_ORDER_POINT-TO-POINT_MOTION_-PROFILE
+    https://www.researchgate.net/publication/
+    289374755_THIRD_ORDER_POINT-TO-POINT_MOTION_-PROFILE
 
     Parameters
     ----------
     distance : `float`
-        The distance to travel. Could be units of length or angle as long as other
-        parameters match.
+        The distance to travel. Could be units of length or angle as long
+        as other parameters match.
     v_max : `float`
         The maximum velocity. Units of length or angle per unit of time.
     acc_max : `float`
-        The maximum acceleration. Units of length or angle per unit of time squared.
+        The maximum acceleration. Units of length or angle per unit of
+        time squared.
     jerk_max : `float`
         The maximum jerk. Units of length or angle per unit of time cubed.
 
     """
     # Case 1: a_max reached, v_max reached and constant for a time
     #          (s = 100,   j = 2000, a = 500,  vMax = 120)
     # Case 2: a_max not reached, v_max not reached
     #          (s = 15000, j = 2000, a = 5500, vMax = 20500)
     # Case 3: a_max not reached, v_max reached and constant for a time
     #          (s = 15000, j = 2000, a = 5500, vMax = 2500)
     # Case 4: a_max reached, v_max not reached
     #          (s = 57,    j = 2000, a = 500,  vMax = 120)
-    # Case 5: a_max reached and constant for a time, v_max reached and constant for a time
+    # Case 5: a_max reached and constant for a time, v_max reached and
+    # constant for a time
     #          (s = 15000, j = 2000, a = 500,  vMax = 2500)
     # Case 6: a_max reached and constant for a time, v_max not reached
     #          (s = 15000, j = 2000, a = 500,  vMax = 20500)
 
     result = np.array(distance * 0)
 
     v_a = acc_max * acc_max / jerk_max
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/model_observatory/kinem_model.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/model_observatory/kinem_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 import warnings
 
 import numpy as np
 
 from rubin_scheduler.scheduler.utils import smallest_signed_angle
-from rubin_scheduler.utils import Site, _approx_altaz2pa, _approx_ra_dec2_alt_az, approx_alt_az2_ra_dec
+from rubin_scheduler.utils import (
+    Site,
+    _approx_altaz2pa,
+    _approx_ra_dec2_alt_az,
+    approx_alt_az2_ra_dec,
+    rotation_converter,
+)
 
 from .jerk import jerk_time
 
 __all__ = ("KinemModel",)
 two_pi = 2.0 * np.pi
 
 
 class Radec2altazpa:
-    """Class to make it easy to swap in different alt/az conversion if wanted."""
+    """Class to make it easy to swap in different alt/az conversion if
+    wanted."""
 
     def __init__(self, location):
         self.location = location
 
     def __call__(self, ra, dec, mjd):
         alt, az, pa = _approx_ra_dec2_alt_az(
             ra, dec, self.location.lat_rad, self.location.lon_rad, mjd, return_pa=True
         )
         return alt, az, pa
 
 
-def _get_rot_sky_pos(pa_rad, rot_tel_rad):
-    """
-    Parameters
-    ----------
-    pa_rad : float or array
-        The parallactic angle
-    """
-    return (rot_tel_rad - pa_rad) % two_pi
-
-
-def _get_rot_tel_pos(pa_rad, rot_sky_rad):
-    """return between -pi and pi"""
-    result = (rot_sky_rad + pa_rad) % two_pi
-    result[np.where(result > np.pi)] -= two_pi
-    return result
-
-
 class KinemModel:
     """A Kinematic model of the telescope.
 
     Parameters
     ----------
     location : `astropy.coordinates.EarthLocation`
         The location of the telescope.
@@ -53,23 +43,27 @@
         The altitude the telescope gets parked at (degrees)
     park_az : `float` (0)
         The azimuth for telescope park position (degrees)
     start_filter : `str` ('r')
         The filter that gets loaded when the telescope is parked
     mjd0 : `float` (0)
         The MJD to assume we are starting from
+    telescope : `str'
+        The telescope name to use for sky rotation conversion. Default "rubin"
 
     Note
     ----
     Note there are additional parameters in the methods setup_camera,
     setup_dome, setup_telescope, and setup_optics.
     Just breaking it up a bit to make it more readable.
     """
 
-    def __init__(self, location=None, park_alt=86.5, park_az=0.0, start_filter="r", mjd0=0):
+    def __init__(
+        self, location=None, park_alt=86.5, park_az=0.0, start_filter="r", mjd0=0, telescope="rubin"
+    ):
         self.park_alt_rad = np.radians(park_alt)
         self.park_az_rad = np.radians(park_az)
         self.start_filter = start_filter
         self.current_filter = self.start_filter
         if location is None:
             self.location = Site("LSST")
             self.location.lat_rad = np.radians(self.location.latitude)
@@ -82,14 +76,17 @@
         self.setup_telescope()
         self.setup_optics()
 
         # Park the telescope
         self.park()
         self.last_mjd = mjd0
 
+        # Rotation conversion
+        self.rc = rotation_converter(telescope=telescope)
+
     def mount_filters(self, filter_list):
         """Change which filters are mounted
 
         Parameters
         ----------
         filter_list : `list` [`str`]
             List of the mounted filters.
@@ -111,32 +108,37 @@
     ):
         """
         Parameters
         ----------
         readtime : `float` (2)
             The readout time of the CCDs (seconds)
         shuttertime : `float` (1.)
-            The time it takes the shutter to go from closed to fully open (seconds)
+            The time it takes the shutter to go from closed to fully open
+            (seconds)
         filter_changetime : `float` (120)
             The time it takes to change filters (seconds)
         fov : `float` (3.5)
             The camera field of view (degrees)
         rotator_min : `float` (-90)
-            The minimum angle the camera rotator (rotTelPos) can move to (degrees)
+            The minimum angle the camera rotator (rotTelPos) can move to
+            (degrees)
         rotator_max : `float` (90)
-            The maximum angle the camera rotator (rotTelPos) can move to (degrees)
+            The maximum angle the camera rotator (rotTelPos) can move to
+            degrees)
         maxspeed : `float` (3.5)
             The maximum speed of the rotator (degrees/s)
         accel : `float` (1.0)
             The acceleration of the rotator (degrees/s^2)
         jerk : `float`
-            The jerk of the rotator (degrees/s^3). Default of None treats jerk as infinite
+            The jerk of the rotator (degrees/s^3). Default of None treats
+            jerk as infinite
         shutter_2motion_min_time : `float` (15.)
-            The time required for two shutter motions (seconds). If one takes
-            a 1-snap 10s exposure, there will be a 5s of overhead before the next exposure can start.
+            The time required for two shutter motions (seconds). If one
+            takes a 1-snap 10s exposure, there will be a 5s of overhead
+            before the next exposure can start.
         """
         self.readtime = readtime
         self.shuttertime = shuttertime
         self.filter_changetime = filter_changetime
         self.camera_fov = np.radians(fov)
 
         self.telrot_minpos_rad = np.radians(rotator_min)
@@ -263,26 +265,29 @@
             The delays for closed optics loops (seconds)
         cl_altlimit : list ([0.0, 9.0, 90.0])
             The altitude limits (degrees) for performing closed optice loops.
             Should be one element longer than cl_delay.
 
         Note
         ----
-        A given movement in altitude will cover X degrees; if X > cl_altlimit[i] there is
+        A given movement in altitude will cover X degrees;
+        if X > cl_altlimit[i] there is
         an additional delay of cl_delay[i]
         """
-        self.optics_ol_slope = ol_slope / np.radians(1.0)  # ah, 1./np.radians(1)=np.pi/180
+        # ah, 1./np.radians(1)=np.pi/180
+        self.optics_ol_slope = ol_slope / np.radians(1.0)
         self.optics_cl_delay = cl_delay
         self.optics_cl_altlimit = np.radians(cl_altlimit)
 
     def park(self):
         """Put the telescope in the park position."""
         # I'm going to ignore that the old model had the dome altitude at 90
         # and telescope altitude 86 for park.
-        # We should usually be dome az limited anyway, so this should be a negligible approximation.
+        # We should usually be dome az limited anyway, so this should be a
+        # negligible approximation.
         self.parked = True
 
         # We have no current position we are tracking
         self.current_ra_rad = None
         self.current_dec_rad = None
         self.current_rot_sky_pos_rad = None
         self.cumulative_azimuth_rad = 0
@@ -301,15 +306,15 @@
 
     def current_alt_az(self, mjd):
         """return the current alt az position that we have tracked to."""
         if self.parked:
             return self.last_alt_rad, self.last_az_rad, self.last_rot_tel_pos_rad
         else:
             alt_rad, az_rad, pa = self.radec2altaz(self.current_ra_rad, self.current_dec_rad, mjd)
-            rot_tel_pos = _get_rot_tel_pos(pa, self.last_rot_tel_pos_rad)
+            rot_tel_pos = self.rc._rotskypos2rottelpos(self.current_rot_sky_pos_rad, pa)
             return alt_rad, az_rad, rot_tel_pos
 
     def slew_times(
         self,
         ra_rad,
         dec_rad,
         mjd,
@@ -366,40 +371,41 @@
             The altitude(s) of the destination pointing(s) (radians).
             Will override ra_rad,dec_rad if provided.
         az_rad : `np.ndarray`
             The azimuth(s) of the destination pointing(s) (radians).
             Will override ra_rad,dec_rad if provided.
         lax_dome : `bool`, default True
             If True, allow the dome to creep, model a dome slit, and don't
-            require the dome to settle in azimuth. If False, adhere to the way
-            SOCS calculates slew times (as of June 21 2017) and do not allow
-            dome creep.
+            require the dome to settle in azimuth. If False, adhere to the
+            way SOCS calculates slew times (as of June 21 2017) and do not
+            allow dome creep.
         starting_alt_rad : `float` (None)
             The starting altitude for the slew (radians).
             If None, will use internally stored last pointing.
         starting_az_rad : `float` (None)
             The starting azimuth for the slew (radians).
             If None, will use internally stored last pointing.
         starting_rot_tel_pos_rad : `float` (None)
             The starting camera rotation for the slew (radians).
             If None, will use internally stored last pointing.
         update_tracking : `bool` (False)
-            If True, update the internal attributes to say we are tracking the
-            specified RA,Dec,RotSkyPos position.
+            If True, update the internal attributes to say we are tracking
+            the specified RA,Dec,RotSkyPos position.
 
         Returns
         -------
         slew_time : `np.ndarray`
             The number of seconds between the two specified exposures.
             Will be np.nan or np.inf if slew is not possible.
         """
         if filtername not in self.mounted_filters:
             return np.nan
 
-        # Don't trust folks to do pa calculation correctly, if both rotations set, rot_sky_pos wins
+        # Don't trust folks to do pa calculation correctly, if both
+        # rotations set, rot_sky_pos wins
         if (rot_tel_pos is not None) & (rot_sky_pos is not None):
             if np.isfinite(rot_tel_pos):
                 rot_sky_pos = None
             else:
                 rot_tel_pos = None
 
         # alt,az not provided, calculate from RA,Dec
@@ -422,73 +428,80 @@
                 )
 
         delta_alt = np.abs(alt_rad - starting_alt_rad)
         delta_az_short = smallest_signed_angle(starting_az_rad, az_rad)
         delta_az_long = delta_az_short - two_pi
         daslz = np.where(delta_az_short < 0)[0]
         delta_az_long[daslz] = two_pi + delta_az_short[daslz]
-        # So, for every position, we can get there by slewing long or short way
+        # So, for every position, we can get there by slewing long or
+        # short way
         cummulative_az_short = delta_az_short + self.cumulative_azimuth_rad
         oob = np.where(
             (cummulative_az_short < self.telaz_minpos_rad) | (cummulative_az_short > self.telaz_maxpos_rad)
         )[0]
         # Set out of bounds azimuths to infinite distance
         delta_az_short[oob] = np.inf
         cummulative_az_long = delta_az_long + self.cumulative_azimuth_rad
         oob = np.where(
             (cummulative_az_long < self.telaz_minpos_rad) | (cummulative_az_long > self.telaz_maxpos_rad)
         )[0]
         delta_az_long[oob] = np.inf
 
-        # Find minimum azimuth slew out of long/short direction (use absolute, because these can be negative)
-        # Note that with an impaired telescope with az range<180, infinite slewtimes can propagate
+        # Find minimum azimuth slew out of long/short direction (use
+        # absolute, because these can be negative)
+        # Note that with an impaired telescope with az range<180,
+        # infinite slewtimes can propagate
         delta_aztel = np.where(
             np.abs(delta_az_short) < np.abs(delta_az_long),
             delta_az_short,
             delta_az_long,
         )
 
-        # Calculate how long the telescope will take to slew to this position.
+        # Calculate how long the telescope will take to slew to this
+        # position.
         tel_alt_slew_time = jerk_time(
             delta_alt, self.telalt_maxspeed_rad, self.telalt_accel_rad, self.telalt_jerk_rad
         )
         tel_az_slew_time = jerk_time(
             np.abs(delta_aztel), self.telaz_maxspeed_rad, self.telaz_accel_rad, self.telaz_jerk_rad
         )
         tot_tel_time = np.maximum(tel_alt_slew_time, tel_az_slew_time)
 
         # Time for open loop optics correction
         ol_time = delta_alt / self.optics_ol_slope
         tot_tel_time += ol_time
         # Add time for telescope settle.
-        # note, this means we're going to have a settle time even for very small slews like dithering.
+        # note, this means we're going to have a settle time even for very
+        # small slews like dithering.
         settle_and_ol = np.where(tot_tel_time > 0)
         tot_tel_time[settle_and_ol] += np.maximum(0, self.mount_settletime - ol_time[settle_and_ol])
 
-        # And any leftover overhead sets a minimum on the total telescope time
+        # And any leftover overhead sets a minimum on the total telescope
+        # time
         tot_tel_time = np.maximum(self.overhead, tot_tel_time)
 
         # now compute dome slew time
-        # the dome can spin all the way around, so we will let it go the shortest angle,
-        # even if the telescope has to unwind
+        # the dome can spin all the way around, so we will let it go the
+        # shortest angle, even if the telescope has to unwind
         delta_az = np.abs(smallest_signed_angle(starting_az_rad, az_rad))
         if lax_dome:
             # model dome creep, dome slit, and no azimuth settle
             # if we can fit both exposures in the dome slit, do so
             same_dome = np.where(delta_alt**2 + delta_az**2 < self.camera_fov**2)
 
             # else, we take the minimum time from two options:
             # 1. assume we line up alt in the center of the dome slit so we
             #    minimize distance we have to travel in azimuth.
             # 2. line up az in the center of the slit
             # also assume:
             # * that we start out going maxspeed for both alt and az
             # * that we only just barely have to get the new field in the
             #   dome slit in one direction, but that we have to center the
-            #   field in the other (which depends which of the two options used)
+            #   field in the other (which depends which of the two options
+            #   used)
             # * that we don't have to slow down until after the shutter
             #   starts opening
             dom_delta_alt = delta_alt
             # on each side, we can start out with the dome shifted away from
             # the center of the field by an amount domSlitRadius - fovRadius
             dom_slit_diam = self.camera_fov / 2.0
             dom_delta_az = delta_az - 2 * (dom_slit_diam / 2 - self.camera_fov / 2)
@@ -502,16 +515,17 @@
             dom_az_slew_time = dom_delta_az / self.domaz_maxspeed_rad
             tot_dom_time2 = np.maximum(dom_alt_slew_time, dom_az_slew_time)
 
             tot_dom_time = np.minimum(tot_dom_time1, tot_dom_time2)
             tot_dom_time[same_dome] = 0
 
         else:
-            # the above models a dome slit and dome creep. However, it appears that
-            # SOCS requires the dome to slew exactly to each field and settle in az
+            # the above models a dome slit and dome creep. However, it
+            # appears that SOCS requires the dome to slew exactly to each
+            # field and settle in az
             dom_alt_slew_time = jerk_time(
                 delta_alt, self.domalt_maxspeed_rad, self.domalt_accel_rad, self.domalt_jerk_rad
             )
             dom_az_slew_time = jerk_time(
                 delta_az, self.domaz_maxspeed_rad, self.domaz_accel_rad, self.domaz_jerk_rad
             )
 
@@ -520,16 +534,16 @@
                 dom_az_slew_time > 0,
                 dom_az_slew_time + self.domaz_settletime,
                 dom_az_slew_time,
             )
             tot_dom_time = np.maximum(dom_alt_slew_time, dom_az_slew_time)
         # Find the max of the above for slew time.
         slew_time = np.maximum(tot_tel_time, tot_dom_time)
-        # include filter change time if necessary. Assume no filter change time
-        # needed if we are starting parked
+        # include filter change time if necessary. Assume no filter
+        # change time needed if we are starting parked
         if not self.parked:
             filter_change = np.where(filtername != self.current_filter)
             slew_time[filter_change] = np.maximum(slew_time[filter_change], self.filter_changetime)
         # Add closed loop optics correction
         # Find the limit where we must add the delay
         cl_limit = self.optics_cl_altlimit[1]
         cl_delay = self.optics_cl_delay[1]
@@ -540,40 +554,42 @@
         outside_limits = np.where((alt_rad > self.telalt_maxpos_rad) | (alt_rad < self.telalt_minpos_rad))[0]
         slew_time[outside_limits] = np.nan
 
         # If we want to include the camera rotation time
         if (rot_sky_pos is not None) | (rot_tel_pos is not None):
             if rot_tel_pos is None:
                 # This is now between -pi and pi
-                rot_tel_pos = _get_rot_tel_pos(pa, rot_sky_pos)
+                rot_tel_pos = self.rc._rotskypos2rottelpos(rot_sky_pos, pa)
             if rot_sky_pos is None:
-                rot_sky_pos = _get_rot_sky_pos(pa, rot_tel_pos)
+                rot_sky_pos = self.rc._rottelpos2rotskypos(rot_tel_pos, pa)
 
             # Is the new rot_tel_pos reachable? If not return NaN
             if (rot_tel_pos < self.telrot_minpos_rad) | (rot_tel_pos > self.telrot_maxpos_rad):
                 return np.nan
             # If there was no kwarg for starting rotator position
             if starting_rot_tel_pos_rad is None:
                 # If there is no current rot_sky_pos, we were parked
                 if self.current_rot_sky_pos_rad is None:
                     current_rot_tel_pos = self.last_rot_tel_pos_rad
                 else:
                     # We have been tracking, so rot_tel_pos needs to be updated
-                    current_rot_tel_pos = _get_rot_tel_pos(starting_pa, self.current_rot_sky_pos_rad)
+                    current_rot_tel_pos = self.rc._rotskypos2rottelpos(
+                        self.current_rot_sky_pos_rad, starting_pa
+                    )
             else:
                 # kwarg overrides if it was supplied
                 current_rot_tel_pos = starting_rot_tel_pos_rad
             delta_rotation = np.abs(smallest_signed_angle(current_rot_tel_pos, rot_tel_pos))
             rotator_time = jerk_time(
                 delta_rotation, self.telrot_maxspeed_rad, self.telrot_accel_rad, self.telrot_jerk_rad
             )
             slew_time = np.maximum(slew_time, rotator_time)
 
-        # Update the internal attributes to note that we are now pointing and tracking
-        # at the requested RA,Dec,rot_sky_pos
+        # Update the internal attributes to note that we are now pointing
+        # and tracking at the requested RA,Dec,rot_sky_pos
         if update_tracking:
             self.current_ra_rad = ra_rad
             self.current_dec_rad = dec_rad
             self.current_rot_sky_pos_rad = rot_sky_pos
             self.parked = False
             # Handy to keep as reference, but not used for any calculations
             self.last_rot_tel_pos_rad = rot_tel_pos
@@ -593,15 +609,16 @@
             observation["exptime"]
             + observation["nexp"] * self.shuttertime
             + max(observation["nexp"] - 1, 0) * self.readtime
         )
         return visit_time
 
     def shutter_stall(self, observation):
-        """Time we need to stall after shutter closes to let things cool down."""
+        """Time we need to stall after shutter closes to let things cool
+        down."""
         result = 0.0
         delta_t = observation["exptime"] / observation["nexp"]
         if delta_t < self.shutter_2motion_min_time:
             result = self.shutter_2motion_min_time - delta_t
         return result
 
     def observe(self, observation, mjd, rot_tel_pos=None, lax_dome=True):
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/model_observatory/model_observatory.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/model_observatory/model_observatory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,161 +1,215 @@
 __all__ = ("ModelObservatory",)
 
+import warnings
 
 import healpy as hp
 import numpy as np
 from astropy.coordinates import EarthLocation
 from astropy.time import Time
 
 import rubin_scheduler.skybrightness_pre as sb
 from rubin_scheduler.data import data_versions
 from rubin_scheduler.scheduler.features import Conditions
 from rubin_scheduler.scheduler.model_observatory import KinemModel
-from rubin_scheduler.scheduler.utils import create_season_offset, set_default_nside
+from rubin_scheduler.scheduler.utils import set_default_nside
 
 # For backwards compatibility
-from rubin_scheduler.site_models import Almanac, CloudData
-from rubin_scheduler.site_models import ConstantCloudData as NoClouds
-from rubin_scheduler.site_models import ConstantSeeingData as NominalSeeing
 from rubin_scheduler.site_models import (
+    Almanac,
+    CloudData,
+    ConstantCloudData,
+    ConstantSeeingData,
     ScheduledDowntimeData,
     SeeingData,
     SeeingModel,
     UnscheduledDowntimeData,
 )
 from rubin_scheduler.utils import (
     Site,
     _angular_separation,
     _approx_altaz2pa,
     _approx_ra_dec2_alt_az,
+    _hpid2_ra_dec,
     _ra_dec2_hpid,
     calc_lmst,
+    calc_season,
     m5_flat_sed,
+    rotation_converter,
     survey_start_mjd,
 )
 
 
 class ModelObservatory:
-    """A class to generate a realistic telemetry stream for the scheduler"""
+    """Generate a realistic telemetry stream for the scheduler in simulations,
+    including simulating the acquisition of observations.
+
+    Parameters
+    ----------
+    nside : `int`, optional
+        The healpix nside resolution.
+        Default None uses `set_default_nside()`.
+    mjd : `float`, optional
+        The MJD to start the model observatory for observations.
+        Used to set current conditions and load sky.
+        Default None uses mjd_start.
+    mjd_start : `float`, optional
+        The MJD of the start of the survey.
+        This must be set to start of whole survey, for tracking
+        purposes.  Default None uses `survey_start_mjd()`.
+    alt_min : `float`, optional
+        The minimum altitude to compute models at (degrees).
+    lax_dome : `bool`, optional
+        Passed to observatory model. If true, allows dome creep.
+    cloud_limit : `float`, optional.
+        The limit to stop taking observations if the cloud model returns
+        something equal or higher. Default of 0.3 is validated as a
+        "somewhat pessimistic" weather downtime choice.
+    sim_to_o : `sim_targetoO` object, optional
+        If one would like to inject simulated ToOs into the telemetry
+        stream. Default None adds no ToOs.
+    park_after : `float`, optional
+        Park the telescope after a gap longer than park_after (minutes).
+        Default 10 minutes is used to park the telescope during downtime.
+    init_load_length : `int`, optional
+        The length of pre-scheduled sky brightness values to load
+        initially (days). The default is 10 days; shorter values
+        can be used for quicker load times.
+    kinem_model : `~.scheduler.model_observatory.Kinem_model`, optional
+        An instantiated rubin_scheduler Kinem_model object.
+        Default of None uses a default Kinem_model.
+    seeing_db : `str`, optional
+        The filename of the seeing data database, if one would like
+        to use an alternate seeing database.
+        Default None uses the default seeing database.
+    seeing_data : `~.site_models.SeeingData`-like, optional
+        If one wants to replace the default seeing_data object.
+        Should be an object with a
+        __call__ method that takes MJD and returns zenith fwhm_500 in
+        arcsec. Set to "ideal" to have constant 0.7" seeing.
+    cloud_db : `str`, optional
+        The filename of the cloud data database.
+        Default of None uses the default database from rubin_sim_data.
+    cloud_offset_year : `int`, optional
+        The year offset to be passed to CloudData. Default 0.
+    cloud_data : `~.site_models.CloudData`-like, optional
+        If one wants to replace the default cloud data. Should be an
+        object with a __call__ method that takes MJD and returns
+        cloudy level. Set to "ideal" for  no clouds.
+    downtimes : `np.ndarray`, (N,3) or None, optional
+        If one wants to replace the default downtimes. Should be a
+        np.array with columns of "start" and "end" with MJD values
+        and should include both scheduled and unscheduled downtime.
+        Set to "ideal" for no downtime. Default of None will use
+        the downtime models from `~.site_models.ScheduledDowntime`
+        and `~.site_models.UnscheduledDowntime`.
+    no_sky : `bool`, optional
+        If True, then don't load any skybrightness files.
+        Handy if one wants a well filled out Conditions object,
+        but doesn't need the sky since that can be slower to load.
+        Default False.
+    wind_data : ~.site_models.WindData`-like, optional
+        If one wants to replace the default wind_data object. Should
+        be an object with a __call__ method that takes the time and
+        returns a tuple with the wind speed (m/s) and originating
+        direction (radians east of north).
+        Default of None uses an idealized WindData object with no wind.
+    starting_time_key : `str`, optional
+        What key in the almanac to use to determine the start of
+        observing on a night. Default "sun_n12_setting", e.g., sun
+        at -12 degrees and setting. Other options are
+        "sun_n18_setting" and "sunset".
+        If surveys are not configured to wait until the sun is lower
+        in the sky, observing will start as soon as the time passes
+        the time returned by this key, in each night.
+    ending_time_key : `str`, optional
+        What key in the almanac to use to signify it is time to skip
+        to the next night. Default "sun_n12_rising", e.g., sun at
+        -12 degrees and rising. Other options are "sun_n18_rising"
+        and "sunrise".
+    telescope : `str`
+        Telescope name for rotation computations. Default "rubin".
+    """
 
     def __init__(
         self,
         nside=None,
+        mjd=None,
         mjd_start=None,
         alt_min=5.0,
         lax_dome=True,
         cloud_limit=0.3,
         sim_to_o=None,
-        seeing_db=None,
         park_after=10.0,
         init_load_length=10,
         kinem_model=None,
+        seeing_db=None,
+        seeing_data=None,
         cloud_db=None,
         cloud_offset_year=0,
         cloud_data=None,
-        seeing_data=None,
         downtimes=None,
         no_sky=False,
         wind_data=None,
         starting_time_key="sun_n12_setting",
         ending_time_key="sun_n12_rising",
+        telescope="rubin",
     ):
-        """
-        Parameters
-        ----------
-        nside : int (None)
-            The healpix nside resolution
-        mjd_start : float (None)
-            The MJD to start the observatory up at. Uses util to lookup default if None.
-        alt_min : float (5.)
-            The minimum altitude to compute models at (degrees).
-        lax_dome : bool (True)
-            Passed to observatory model. If true, allows dome creep.
-        cloud_limit : float (0.3)
-            The limit to stop taking observations if the cloud model returns something equal or higher
-        sim_to_o : sim_targetoO object (None)
-            If one would like to inject simulated ToOs into the telemetry stream.
-        seeing_db : filename of the seeing data database (None)
-            If one would like to use an alternate seeing database
-        park_after : float (10)
-            Park the telescope after a gap longer than park_after (minutes)
-        init_load_length : int (10)
-            The length of pre-scheduled sky brighntess to load initially (days).
-        kinem_model : kinematic model object (None)
-            A instantiated rubin_scheduler.scheduler.model_observatory.Kinem_model object. If None, the
-            default is used
-        cloud_db : str (None)
-            The file to use for clouds. Default of None uses the database in rubin_sim_data.
-        cloud_offset_year : 0
-            The year offset to be passed to CloudData.
-        cloud_data : None
-            If one wants to replace the default cloud data. Should be an object with a
-            __call__ method that takes MJD and returns cloudy level. Set to "ideal" for
-            no clouds.
-        seeing_data : None
-            If one wants to replace the default seeing_data object. Should be an object with a
-            __call__ method that takes MJD and returns zenith fwhm_500 in arcsec. Set to
-            "ideal" to have constant 0.7" seeing.
-        downtimes : None
-            If one wants to replace the default downtimes. Should be a np.array with columns
-            of "start" and "end" with MJD values and should include both scheduled and unscheduled downtime.
-            Set to "ideal" for no downtime.
-        no_sky : bool
-            Don't bother loading sky files. Handy if one wants a well filled out Conditions object,
-            but doesn't need the sky since that can be slower to load. Default False.
-        wind_data : None
-            If one wants to replace the default wind_data object. Should be an
-            object with a __call__ method that takes the time and returns a
-            tuple with the wind speed (m/s) and originating direction (radians
-            east of north)
-        starting_time_key : str
-            What key in the almanac to use to determine the start of observing on a night.
-            Default "sun_n12_setting", e.g., sun at -12 degrees and setting. Other
-            options are "sun_n18_setting" and "sunset"
-        ending_time_key : str
-            What key in the almanac to use to signify it is time to skip to the next night.
-            Default "sun_n12_rising", e.g., sun at -12 degrees and rising. Other
-            options are "sun_n18_rising" and "sunrise"
-        """
-
         if nside is None:
             nside = set_default_nside()
         self.nside = nside
 
-        self.wind_data = wind_data
+        # Set the time now - mjd
+        # and the time of the survey start
+        if mjd_start is None:
+            mjd_start = survey_start_mjd()
+        self.mjd_start = mjd_start
+
+        if mjd is None:
+            mjd = mjd_start
+
+        self.filterlist = ["u", "g", "r", "i", "z", "y"]
 
         self.cloud_limit = cloud_limit
         self.no_sky = no_sky
-
         self.alt_min = np.radians(alt_min)
         self.lax_dome = lax_dome
-        self.mjd_start = survey_start_mjd() if mjd_start is None else mjd_start
         self.starting_time_key = starting_time_key
         self.ending_time_key = ending_time_key
 
         self.sim__to_o = sim_to_o
 
         self.park_after = park_after / 60.0 / 24.0  # To days
 
+        # Rotation converter
+        self.rc = rotation_converter(telescope=telescope)
+
         # Create an astropy location
         self.site = Site("LSST")
         self.location = EarthLocation(
             lat=self.site.latitude, lon=self.site.longitude, height=self.site.height
         )
 
-        # Load up all the models we need
+        # Set up the almanac - use mjd_start to keep "night" count the same.
+        self.almanac = Almanac(mjd_start=self.mjd_start)
 
+        # Load up all the models we need
+        # Use mjd_start to ensure models always initialize to the same
+        # starting point in time.
         mjd_start_time = Time(self.mjd_start, format="mjd")
-        # Downtime
+
+        # Set up the downtime
         if isinstance(downtimes, str):
             if downtimes == "ideal":
                 self.downtimes = np.array(
                     list(zip([], [])),
                     dtype=list(zip(["start", "end"], [float, float])),
                 )
+            else:
+                warnings.warn("Downtimes should be a string equal to " "'ideal', an array or None")
         elif downtimes is None:
             self.down_nights = []
             self.sched_downtime_data = ScheduledDowntimeData(mjd_start_time)
             self.unsched_downtime_data = UnscheduledDowntimeData(mjd_start_time)
 
             sched_downtimes = self.sched_downtime_data()
             unsched_downtimes = self.unsched_downtime_data()
@@ -174,78 +228,85 @@
                 dtype=list(zip(["start", "end"], [float, float])),
             )
             self.downtimes.sort(order="start")
 
             # Make sure there aren't any overlapping downtimes
             diff = self.downtimes["start"][1:] - self.downtimes["end"][0:-1]
             while np.min(diff) < 0:
-                # Should be able to do this wihtout a loop, but this works
+                # Should be able to do this without a loop, but this works
                 for i, dt in enumerate(self.downtimes[0:-1]):
                     if self.downtimes["start"][i + 1] < dt["end"]:
                         new_end = np.max([dt["end"], self.downtimes["end"][i + 1]])
                         self.downtimes[i]["end"] = new_end
                         self.downtimes[i + 1]["end"] = new_end
 
                 good = np.where(self.downtimes["end"] - np.roll(self.downtimes["end"], 1) != 0)
                 self.downtimes = self.downtimes[good]
                 diff = self.downtimes["start"][1:] - self.downtimes["end"][0:-1]
         else:
             self.downtimes = downtimes
 
+        # Set the wind data
+        self.wind_data = wind_data
+
+        # Set up the seeing data
         if seeing_data == "ideal":
-            self.seeing_data = NominalSeeing()
+            self.seeing_data = ConstantSeeingData()
         elif seeing_data is not None:
             self.seeing_data = seeing_data
         else:
             self.seeing_data = SeeingData(mjd_start_time, seeing_db=seeing_db)
         self.seeing_model = SeeingModel()
         self.seeing_indx_dict = {}
         for i, filtername in enumerate(self.seeing_model.filter_list):
             self.seeing_indx_dict[filtername] = i
 
+        self.seeing_fwhm_eff = {}
+        for key in self.filterlist:
+            self.seeing_fwhm_eff[key] = np.zeros(hp.nside2npix(self.nside), dtype=float)
+
+        # Set up the cloud data
         if cloud_data == "ideal":
-            self.cloud_data = NoClouds()
+            self.cloud_data = ConstantCloudData()
         elif cloud_data is not None:
             self.cloud_data = cloud_data
         else:
             self.cloud_data = CloudData(mjd_start_time, cloud_db=cloud_db, offset_year=cloud_offset_year)
 
+        # Set up the skybrightness
         if not self.no_sky:
             self.sky_model = sb.SkyModelPre(init_load_length=init_load_length)
         else:
             self.sky_model = None
 
+        # Set up the kinematic model
         if kinem_model is None:
             self.observatory = KinemModel(mjd0=self.mjd_start)
         else:
             self.observatory = kinem_model
 
-        self.filterlist = ["u", "g", "r", "i", "z", "y"]
-        self.seeing_fwhm_eff = {}
-        for key in self.filterlist:
-            self.seeing_fwhm_eff[key] = np.zeros(hp.nside2npix(self.nside), dtype=float)
-
-        self.almanac = Almanac(mjd_start=self.mjd_start)
-
         # Let's make sure we're at an openable MJD
         good_mjd = False
-        to_set_mjd = self.mjd_start
+        to_set_mjd = mjd
         while not good_mjd:
             good_mjd, to_set_mjd = self.check_mjd(to_set_mjd)
         self.mjd = to_set_mjd
 
-        sun_moon_info = self.almanac.get_sun_moon_positions(self.mjd)
-        season_offset = create_season_offset(self.nside, sun_moon_info["sun_RA"])
+        sun_moon_info = self.almanac.get_sun_moon_positions(mjd)
+        # Create the map of the season offsets - this map is constant
+        ra, dec = _hpid2_ra_dec(nside, np.arange(hp.nside2npix(self.nside)))
+        ra_deg = np.degrees(ra)
+        self.season_map = calc_season(ra_deg, [self.mjd_start], self.mjd_start).flatten()
         self.sun_ra_start = sun_moon_info["sun_RA"] + 0
-        self.season_offset = season_offset
         # Conditions object to update and return on request
+        # (at present, this is not updated -- recreated, below).
         self.conditions = Conditions(
             nside=self.nside,
             mjd_start=self.mjd_start,
-            season_offset=self.season_offset,
+            season_map=self.season_map,
             sun_ra_start=self.sun_ra_start,
         )
 
         self.obs_id_counter = 0
 
     def get_info(self):
         """
@@ -267,27 +328,28 @@
         Returns
         -------
         rubin_scheduler.scheduler.features.conditions object
         """
         self.conditions = Conditions(
             nside=self.nside,
             mjd_start=self.mjd_start,
-            season_offset=self.season_offset,
+            season_map=self.season_map,
             sun_ra_start=self.sun_ra_start,
             mjd=self.mjd,
         )
 
         self.conditions.night = int(self.night)
         # Current time as astropy time
         current_time = Time(self.mjd, format="mjd")
 
         # Clouds. XXX--just the raw value
         self.conditions.bulk_cloud = self.cloud_data(current_time)
 
-        # use conditions object itself to get aprox altitude of each healpx
+        # use conditions object itself to get aprox altitude of each
+        # healpx
         alts = self.conditions.alt
         azs = self.conditions.az
 
         good = np.where(alts > self.alt_min)
 
         # Compute the airmass at each heapix
         airmass = np.zeros(alts.size, dtype=float)
@@ -363,14 +425,16 @@
         self.conditions.sun_n12_setting = self.almanac.sunsets["sun_n12_setting"][self.almanac_indx]
         self.conditions.sun_n18_setting = self.almanac.sunsets["sun_n18_setting"][self.almanac_indx]
         self.conditions.sun_n18_rising = self.almanac.sunsets["sun_n18_rising"][self.almanac_indx]
         self.conditions.sun_n12_rising = self.almanac.sunsets["sun_n12_rising"][self.almanac_indx]
         self.conditions.sunrise = self.almanac.sunsets["sunrise"][self.almanac_indx]
         self.conditions.moonrise = self.almanac.sunsets["moonrise"][self.almanac_indx]
         self.conditions.moonset = self.almanac.sunsets["moonset"][self.almanac_indx]
+        sun_moon_info_start_of_night = self.almanac.get_sun_moon_positions(self.conditions.sunset)
+        self.conditions.moon_phase_sunset = sun_moon_info_start_of_night["moon_phase"]
 
         self.conditions.mjd_start = self.mjd_start
 
         # Telescope limits
         self.conditions.tel_az_limits = self.observatory.az_limits
         self.conditions.tel_alt_limits = self.observatory.alt_limits
 
@@ -488,29 +552,31 @@
         cloud_skip : float (20)
             How much time to skip ahead if it's cloudy (minutes)
 
         Returns
         -------
         mjd_ok : `bool`
         mdj : `float`
-            If True, the input mjd. If false, a good mjd to skip forward to.
+            If True, the input mjd. If false, a good mjd to skip
+            forward to.
         """
         passed = True
         new_mjd = mjd + 0
 
-        # Maybe set this to a while loop to make sure we don't land on another cloudy time?
+        # Maybe set this to a while loop to make sure we don't
+        # land on another cloudy time?
         # or just make this an entire recursive call?
         clouds = self.cloud_data(Time(mjd, format="mjd"))
 
         if clouds > self.cloud_limit:
             passed = False
             while clouds > self.cloud_limit:
                 new_mjd = new_mjd + cloud_skip / 60.0 / 24.0
                 clouds = self.cloud_data(Time(new_mjd, format="mjd"))
-        alm_indx = np.searchsorted(self.almanac.sunsets["sunset"], mjd, side="right") - 1
+        alm_indx = np.searchsorted(self.almanac.sunsets[self.starting_time_key], mjd, side="right") - 1
         # at the end of the night, advance to the next setting twilight
         if mjd > self.almanac.sunsets[self.ending_time_key][alm_indx]:
             passed = False
             new_mjd = self.almanac.sunsets[self.starting_time_key][alm_indx + 1]
         if mjd < self.almanac.sunsets[self.starting_time_key][alm_indx]:
             passed = False
             new_mjd = self.almanac.sunsets[self.starting_time_key][alm_indx + 1]
@@ -541,21 +607,22 @@
             self.site.latitude_rad,
             self.site.longitude_rad,
             self.mjd,
         )
 
         obs_pa = _approx_altaz2pa(alt, az, self.site.latitude_rad)
 
-        # If the observation has a rotTelPos set, use it to compute rotSkyPos
+        # If the observation has a rotTelPos set, use it to compute
+        # rotSkyPos
         if np.isfinite(observation["rotTelPos"]):
-            observation["rotSkyPos"] = (obs_pa + observation["rotTelPos"]) % (2 * np.pi)
+            observation["rotSkyPos"] = self.rc._rottelpos2rotskypos(observation["rotTelPos"], obs_pa)
             observation["rotTelPos"] = np.nan
         else:
             # Fall back to rotSkyPos_desired
-            possible_rot_tel_pos = (observation["rotSkyPos_desired"] + obs_pa) % (2.0 * np.pi)
+            possible_rot_tel_pos = self.rc._rotskypos2rottelpos(observation["rotSkyPos_desired"], obs_pa)
 
             if (possible_rot_tel_pos > rot_limit[0]) | (possible_rot_tel_pos < rot_limit[1]):
                 observation["rotSkyPos"] = observation["rotSkyPos_desired"]
                 observation["rotTelPos"] = np.nan
             else:
                 # Fall back to the backup rotation angle if needed.
                 observation["rotSkyPos"] = np.nan
@@ -565,41 +632,45 @@
 
     def observe(self, observation):
         """Try to make an observation
 
         Returns
         -------
         observation : observation object
-            None if there was no observation taken. Completed observation with meta data filled in.
+            None if there was no observation taken. Completed
+            observation with meta data filled in.
         new_night : bool
             Have we started a new night.
         """
 
         start_night = self.night.copy()
 
         if np.isnan(observation["rotSkyPos"]):
             observation = self._update_rot_sky_pos(observation)
 
-        # If there has been a long gap, assume telescope stopped tracking and parked
+        # If there has been a long gap, assume telescope stopped
+        # tracking and parked
         gap = self.mjd - self.observatory.last_mjd
         if gap > self.park_after:
             self.observatory.park()
 
         # Compute what alt,az we have tracked to (or are parked at)
         start_alt, start_az, start_rot_tel_pos = self.observatory.current_alt_az(self.mjd)
-        # Slew to new position and execute observation. Use the requested rotTelPos position,
-        # obsevation['rotSkyPos'] will be ignored.
+        # Slew to new position and execute observation. Use the
+        # requested rotTelPos position, obsevation['rotSkyPos'] will
+        # be ignored.
         slewtime, visittime = self.observatory.observe(
             observation,
             self.mjd,
             rot_tel_pos=observation["rotTelPos"],
             lax_dome=self.lax_dome,
         )
 
-        # inf slewtime means the observation failed (probably outside alt limits)
+        # inf slewtime means the observation failed (probably outside
+        # alt limits)
         if ~np.all(np.isfinite(slewtime)):
             return None, False
 
         observation_worked, new_mjd = self.check_mjd(self.mjd + (slewtime + visittime) / 24.0 / 3600.0)
 
         if observation_worked:
             observation["visittime"] = visittime
@@ -607,24 +678,32 @@
             observation["slewdist"] = _angular_separation(
                 start_az,
                 start_alt,
                 self.observatory.last_az_rad,
                 self.observatory.last_alt_rad,
             )
             self.mjd = self.mjd + slewtime / 24.0 / 3600.0
-            # Reach into the observatory model to pull out the relevant data it has calculated
-            # Note, this might be after the observation has been completed.
-            observation["alt"] = self.observatory.last_alt_rad
-            observation["az"] = self.observatory.last_az_rad
-            observation["pa"] = self.observatory.last_pa_rad
-            observation["rotTelPos"] = self.observatory.last_rot_tel_pos_rad
+            # Reach into the observatory model to pull out the
+            # relevant data it has calculated
+            # Not bothering to fetch alt,az,pa,rottelpos as those
+            # were computed before the slew was executed
+            # so will be off by seconds to minutes. And they
+            # shouldn't be needed by the scheduler.
+
             observation["rotSkyPos"] = self.observatory.current_rot_sky_pos_rad
             observation["cummTelAz"] = self.observatory.cumulative_azimuth_rad
 
-            # Metadata on observation is after slew and settle, so at start of exposure.
+            # But we do need the altitude to
+            # get the airmass and then 5-sigma depth
+            # this altitude should get clobbered later
+            # by sim_runner.
+            observation["alt"] = self.observatory.last_alt_rad
+
+            # Metadata on observation is after slew and settle,
+            # so at start of exposure.
             result = self.observation_add_data(observation)
             self.mjd = self.mjd + visittime / 24.0 / 3600.0
             new_night = False
         else:
             result = None
             self.observatory.park()
             # Skip to next legitimate mjd
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/schedulers/core_scheduler.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/schedulers/core_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,51 +8,56 @@
 
 import healpy as hp
 import numpy as np
 import pandas as pd
 from astropy.time import Time
 
 from rubin_scheduler.scheduler.utils import HpInComcamFov, HpInLsstFov, IntRounded, set_default_nside
-from rubin_scheduler.utils import _approx_altaz2pa, _approx_ra_dec2_alt_az, _hpid2_ra_dec
+from rubin_scheduler.utils import _approx_altaz2pa, _approx_ra_dec2_alt_az, _hpid2_ra_dec, rotation_converter
 
 
 class CoreScheduler:
-    """Core scheduler that takes requests observations, reports observatory
-    status and provides completed observations.
+    """Core scheduler that takes requests observations,
+    reports observatory status and provides completed observations.
 
     Parameters
     ----------
-    surveys : list (or list of lists) of rubin_scheduler.scheduler.survey objects
+    surveys : list (or list of lists) of rubin_scheduler.scheduler.survey
         A list of surveys to consider.
-        If multiple surveys return the same highest reward value, the survey
-        at the earliest position in the list will be selected.
-        Can also be a list of lists to make heirarchical priorities ('tiers').
+        If multiple surveys return the same highest reward value,
+        the survey at the earliest position in the list will be selected.
+        Can also be a list of lists to make heirarchical priorities
+        ('tiers').
     nside : `int`
         A HEALpix nside value.
     camera : `str`
         Which camera to use to compute the correspondence between
         visits and HEALpixels when recording observations.
         Can be 'LSST' or 'comcam'.
     rotator_limits : `list` [`float`, `float`]
         Limits for the camera rotator.
     log : `logging.Logger`
         If None, a new logger is created.
     keep_rewards : `bool`
         Flag whether to record the rewards and basis function values
         (this can be useful for schedview).
+    telescope : `str`
+        Which telescope model to use for rotTelPos/rotSkyPos conversions.
+        Default "rubin".
     """
 
     def __init__(
         self,
         surveys,
         nside=None,
         camera="LSST",
         rotator_limits=[85.0, 275.0],
         log=None,
         keep_rewards=False,
+        telescope="rubin",
     ):
         self.keep_rewards = keep_rewards
         # Use integer ns just to be sure there are no rounding issues.
         self.mjd_perf_counter_offset = np.int64(Time.now().mjd * 86400000000000) - time.perf_counter_ns()
 
         if nside is None:
             nside = set_default_nside()
@@ -81,14 +86,16 @@
         if camera == "LSST":
             self.pointing2hpindx = HpInLsstFov(nside=nside)
         elif camera == "comcam":
             self.pointing2hpindx = HpInComcamFov(nside=nside)
         else:
             raise ValueError("camera %s not implamented" % camera)
 
+        self.rc = rotation_converter(telescope=telescope)
+
         # keep track of how many observations get flushed from the queue
         self.flushed = 0
         self.rotator_limits = np.sort(np.radians(rotator_limits))
 
     def flush_queue(self):
         """Like it sounds, clear any currently queued desired observations."""
         self.queue = []
@@ -235,22 +242,24 @@
                     observation["RA"],
                     observation["dec"],
                     self.conditions.site.latitude_rad,
                     self.conditions.site.longitude_rad,
                     mjd,
                 )
                 obs_pa = _approx_altaz2pa(alt, az, self.conditions.site.latitude_rad)
-                rot_tel_pos_expected = (obs_pa - observation["rotSkyPos"]) % (2.0 * np.pi)
+                rot_tel_pos_expected = self.rc._rotskypos2rottelpos(observation["rotSkyPos"], obs_pa)
                 if np.isfinite(observation["rotSkyPos"]):
                     if (IntRounded(rot_tel_pos_expected) > IntRounded(self.rotator_limits[0])) & (
                         IntRounded(rot_tel_pos_expected) < IntRounded(self.rotator_limits[1])
                     ):
                         diff = np.abs(self.rotator_limits - rot_tel_pos_expected)
                         limit_indx = np.min(np.where(diff == np.min(diff))[0])
-                        observation["rotSkyPos"] = (obs_pa - self.rotator_limits[limit_indx]) % (2.0 * np.pi)
+                        observation["rotSkyPos"] = self.rc.rottelpos2rotskypos(
+                            self.rotator_limits[limit_indx], obs_pa
+                        )
             return observation
 
     def _fill_queue(self):
         """
         Compute reward function for each survey and fill the observing queue
         with the observations from the highest reward survey.
         """
@@ -420,16 +429,16 @@
         except TypeError:
             last_chosen = "None"
 
         misc = pd.Series(
             {
                 "camera": camera,
                 "nside": self.nside,
-                "rotator limits": self.rotator_limits,
-                "survey index": self.survey_index,
+                "rotator limits": list(self.rotator_limits),
+                "survey index": list(self.survey_index),
                 "Last chosen": last_chosen,
             }
         )
         misc.name = "value"
         print(misc.to_markdown(), file=output)
 
         print("", file=output)
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/schedulers/filter_scheduler.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/schedulers/filter_scheduler.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,38 +22,39 @@
 
 
 class SimpleFilterSched(FilterSwapScheduler):
     def __init__(self, illum_limit=10.0):
         self.illum_limit_ir = IntRounded(illum_limit)
 
     def __call__(self, conditions):
-        if IntRounded(conditions.moon_phase) > self.illum_limit_ir:
+        if IntRounded(conditions.moon_phase_sunset) > self.illum_limit_ir:
             result = ["g", "r", "i", "z", "y"]
         else:
             result = ["u", "g", "r", "i", "z"]
         return result
 
 
 class FilterSchedUzy(FilterSwapScheduler):
     """
-    remove u in bright time. Alternate between removing z and y in dark time.
+    remove u in bright time. Alternate between removing z and y in
+    dark time.
 
-    Note, this might not work properly if we need to restart a bunch. So a more robust
-    way of scheduling filter loading might be in order.
+    Note, this might not work properly if we need to restart a bunch.
+    So a more robust way of scheduling filter loading might be in order.
     """
 
     def __init__(self, illum_limit=10.0):
         self.illum_limit_ir = IntRounded(illum_limit)
         self.last_swap = 0
 
         self.bright_time = ["g", "r", "i", "z", "y"]
         self.dark_times = [["u", "g", "r", "i", "y"], ["u", "g", "r", "i", "z"]]
 
     def __call__(self, conditions):
-        if IntRounded(conditions.moon_phase) > self.illum_limit_ir:
+        if IntRounded(conditions.moon_phase_sunset) > self.illum_limit_ir:
             result = self.bright_time
         else:
             indx = self.last_swap % 2
             result = self.dark_times[indx]
             if result != conditions.mounted_filters:
                 self.last_swap += 1
         return result
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/sim_runner.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/sim_runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import warnings
 
 import numpy as np
 import pandas as pd
 
 from rubin_scheduler.scheduler.schedulers import SimpleFilterSched
 from rubin_scheduler.scheduler.utils import SchemaConverter, empty_observation, run_info_table
+from rubin_scheduler.utils import Site, _approx_altaz2pa, pseudo_parallactic_angle, rotation_converter
 
 
 def sim_runner(
     observatory,
     scheduler,
     filter_scheduler=None,
     mjd_start=None,
@@ -24,35 +25,47 @@
     step_none=15.0,
     verbose=True,
     extra_info=None,
     event_table=None,
     record_rewards=False,
     start_result_size=int(2e5),
     append_result_size=int(2.5e6),
+    anomalous_overhead_func=None,
+    telescope="rubin",
 ):
     """
     run a simulation
 
     Parameters
     ----------
     survey_length : float (3.)
         The length of the survey ot run (days)
     step_none : float (15)
-        The amount of time to advance if the scheduler fails to return a target (minutes).
+        The amount of time to advance if the scheduler fails to
+        return a target (minutes).
     extra_info : dict (None)
-        If present, dict gets added onto the information from the observatory model.
+        If present, dict gets added onto the information from the
+        observatory model.
     event_table : np.array (None)
         Any ToO events that were included in the simulation
     record_rewards : bool (False)
         Save computed rewards
     start_result_size : int
-        Size of observations array to pre-allocate at the start of the run. Default 2e5.
+        Size of observations array to pre-allocate at the start of
+        the run. Default 2e5.
     append_result_size : int
-        Size of observations array to append if start_result_size is too small.
-        Default 2.5e6.
+        Size of observations array to append if start_result_size is
+        too small. Default 2.5e6.
+    anomalous_overhead_func: `Callable` or None
+        A function or callable object that takes the visit time and slew time
+        (in seconds) as argument, and returns and additional offset (also
+        in seconds) to be applied as addinional overhead between exposures.
+        Defaults to None.
+    telescope : `str`
+        Name of telecope for camera rotation. Default "rubin".
     """
 
     if extra_info is None:
         extra_info = {}
 
     t0 = time.time()
 
@@ -77,14 +90,21 @@
 
     mjd_last_flush = -1
 
     last_obs_queue_fill_mjd_ns = None
     obs_rewards = {}
     reward_dfs = []
 
+    rc = rotation_converter(telescope=telescope)
+
+    # Make sure correct filters are mounted
+    conditions = observatory.return_conditions()
+    filters_needed = filter_scheduler(conditions)
+    observatory.observatory.mount_filters(filters_needed)
+
     counter = 0
     while mjd < end_mjd:
         if not scheduler._check_queue_mjd_only(observatory.mjd):
             scheduler.update_conditions(observatory.return_conditions())
         desired_obs = scheduler.request_observation(mjd=observatory.mjd)
         if record_rewards:
             if last_obs_queue_fill_mjd_ns != scheduler.queue_fill_mjd_ns:
@@ -95,27 +115,35 @@
             # No observation. Just step into the future and try again.
             warnings.warn("No observation. Step into the future and trying again.")
             observatory.mjd = observatory.mjd + step_none
             scheduler.update_conditions(observatory.return_conditions())
             nskip += 1
             continue
         completed_obs, new_night = observatory.observe(desired_obs)
+
         if completed_obs is not None:
+
+            if anomalous_overhead_func is not None:
+                observatory.mjd += (
+                    anomalous_overhead_func(completed_obs["visittime"], completed_obs["slewtime"]) / 86400
+                )
+
             scheduler.add_observation(completed_obs[0])
             observations[counter] = completed_obs[0]
             filter_scheduler.add_observation(completed_obs[0])
             counter += 1
             if counter == observations.size:
                 add_observations = empty_observation(n=append_result_size)
                 observations = np.concatenate([observations, add_observations])
 
             if record_rewards:
                 obs_rewards[completed_obs[0]["mjd"]] = last_obs_queue_fill_mjd_ns
         else:
-            # An observation failed to execute, usually it was outside the altitude limits.
+            # An observation failed to execute, usually it was outside
+            # the altitude limits.
             if observatory.mjd == mjd_last_flush:
                 raise RuntimeError("Scheduler has failed to provide a valid observation multiple times.")
             # if this is a first offence, might just be that targets set.
             # Flush queue and get some new targets.
             scheduler.flush_queue()
             mjd_last_flush = observatory.mjd + 0
         if new_night:
@@ -138,14 +166,36 @@
         # XXX--handy place to interupt and debug
         # if len(observations) > 25:
         #    import pdb ; pdb.set_trace()
 
     # trim off any observations that were pre-allocated but not used
     observations = observations[0:counter]
 
+    # Compute alt,az,pa, rottelpos for observations
+    # Only warn if it's a low-accuracy astropy conversion
+    lsst = Site("LSST")
+
+    # Using pseudo_parallactic_angle, see https://smtn-019.lsst.io/v/DM-44258/index.html
+    pa, alt, az = pseudo_parallactic_angle(
+        np.degrees(observations["RA"]),
+        np.degrees(observations["dec"]),
+        observations["mjd"],
+        lon=lsst.longitude,
+        lat=lsst.latitude,
+        height=lsst.height,
+    )
+    observations["alt"] = np.radians(alt)
+    observations["az"] = np.radians(az)
+    observations["psudo_pa"] = np.radians(pa)
+    observations["rotTelPos"] = rc._rotskypos2rottelpos(observations["rotSkyPos"], observations["psudo_pa"])
+
+    # Also include traditional parallactic angle
+    pa = _approx_altaz2pa(observations["alt"], observations["az"], lsst.latitude_rad)
+    observations["pa"] = pa
+
     runtime = time.time() - t0
     print("Skipped %i observations" % nskip)
     print("Flushed %i observations from queue for being stale" % scheduler.flushed)
     print("Completed %i observations" % len(observations))
     print("ran in %i min = %.1f hours" % (runtime / 60.0, runtime / 3600.0))
     if len(observations) > 0:
         if filename is not None:
@@ -167,15 +217,16 @@
             obs_rewards_series.name = "queue_fill_mjd_ns"
 
             if filename is not None:
                 with sqlite3.connect(filename) as con:
                     reward_df.to_sql("rewards", con)
                     obs_rewards_series.to_sql("obs_rewards", con)
     else:
-        # Make sure there is something to return if there are no observations
+        # Make sure there is something to return if there are no
+        # observations
         reward_df = None
         obs_rewards_series = None
 
     if record_rewards:
         result = observatory, scheduler, observations, reward_df, obs_rewards_series
     else:
         result = observatory, scheduler, observations
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/base_survey.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/base_survey.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,21 +26,23 @@
     Parameters
     ----------
     basis_functions : list
         List of basis_function objects
     extra_features : list XXX--should this be a dict for clarity?
         List of any additional features the survey may want to use
         e.g., for computing final dither positions.
-    extra_basis_functions : dict of rubin_scheduler.scheduler.basis_function objects
-        Extra basis function objects. Typically not psased in, but et in the __init__.
+    extra_basis_functions : dict of rubin_scheduler.scheduler.basis_function
+        Extra basis function objects. Typically not passed in, but et
+        in the __init__.
     ignore_obs : list of str (None)
-        If an incoming observation has this string in the note, ignore it. Handy if
-        one wants to ignore DD fields or observations requested by self. Take note,
-        if a survey is called 'mysurvey23', setting ignore_obs to 'mysurvey2' will
-        ignore it because 'mysurvey2' is a substring of 'mysurvey23'.
+        If an incoming observation has this string in the note, ignore it.
+        Handy if one wants to ignore DD fields or observations
+        requested by self. Take note, if a survey is called 'mysurvey23',
+        setting ignore_obs to 'mysurvey2' will ignore it because
+        'mysurvey2' is a substring of 'mysurvey23'.
     detailers : list of rubin_scheduler.scheduler.detailers objects
         The detailers to apply to the list of observations.
     scheduled_obs : np.array
         An array of MJD values for when observations should execute.
     """
 
     def __init__(
@@ -120,19 +122,20 @@
     def add_observations_array(self, observations_array_in, observations_hpid_in):
         """Add an array of observations rather than one at a time
 
         Parameters
         ----------
         observations_array_in : np.array
             An array of completed observations
-            (with columns like rubin_scheduler.scheduler.utils.empty_observation).
+            (with columns like
+            rubin_scheduler.scheduler.utils.empty_observation).
         observations_hpid_in : np.array
-            Same as observations_array_in, but larger and with an additional column
-            for HEALpix id. Each observation is listed mulitple times,
-            once for every HEALpix it overlaps.
+            Same as observations_array_in, but larger and with an
+            additional column for HEALpix id. Each observation is
+            listed mulitple times, once for every HEALpix it overlaps.
         """
 
         # Just to be sure things are sorted
         observations_array_in.sort(order="mjd")
         observations_hpid_in.sort(order="mjd")
 
         # Copy so we don't prune things for other survey objects
@@ -155,15 +158,16 @@
         for detailer in self.detailers:
             detailer.add_observations_array(observations_array, observations_hpid)
         self.reward_checked = False
 
     def add_observation(self, observation, **kwargs):
         # Check each posible ignore string
         checks = [io not in str(observation["note"]) for io in self.ignore_obs]
-        # ugh, I think here I have to assume observation is an array and not a dict.
+        # ugh, I think here I have to assume observation is an
+        # array and not a dict.
         if all(checks):
             for feature in self.extra_features:
                 self.extra_features[feature].add_observation(observation, **kwargs)
             for bf in self.extra_basis_functions:
                 self.extra_basis_functions[bf].add_observation(observation, **kwargs)
             for bf in self.basis_functions:
                 bf.add_observation(observation, **kwargs)
@@ -221,16 +225,18 @@
         observations = self.generate_observations_rough(conditions)
         if np.size(observations) > 0:
             for detailer in self.detailers:
                 observations = detailer(observations, conditions)
         return observations
 
     def viz_config(self):
-        # XXX--zomg, we should have a method that goes through all the objects and
-        # makes plots/prints info so there can be a little notebook showing the config!
+        # XXX--zomg, we should have a method that goes through all
+        # the objects and
+        # makes plots/prints info so there can be a little
+        # notebook showing the config!
         pass
 
     def __repr__(self):
         try:
             repr = f"<{self.__class__.__name__} survey_name='{self.survey_name}' at {hex(id(self))}>"
         except AttributeError:
             repr = f"<{self.__class__.__name__} at {hex(id(self))}>"
@@ -407,36 +413,40 @@
     xp = x
     yp = y * cos_t + z * sin_t
     zp = -y * sin_t + z * cos_t
     return xp, yp, zp
 
 
 class BaseMarkovSurvey(BaseSurvey):
-    """A Markov Decision Function survey object. Uses Basis functions to compute a
-    final reward function and decide what to observe based on the reward. Includes
-    methods for dithering and defaults to dithering nightly.
+    """A Markov Decision Function survey object. Uses Basis functions
+    to compute a final reward function and decide what to observe based
+    on the reward. Includes methods for dithering and defaults to
+    dithering nightly.
 
     Parameters
     ----------
-    basis_function : list of rubin_scheduler.schuler.basis_function objects
+    basis_function : list of rubin_scheduler.schuler.basis_function
 
     basis_weights : list of float
         Must be same length as basis_function
     seed : hashable
         Random number seed, used for randomly orienting sky tessellation.
     camera : str ('LSST')
         Should be 'LSST' or 'comcam'
     fields : np.array (None)
-        An array of field positions. Should be numpy array with columns of "RA" and
-        "dec" in radians. If none, site_models.read_fields or utils.comcam_tessellate is
-        used to read field positions.
+        An array of field positions. Should be numpy array with columns
+        of "RA" and "dec" in radians. If none,
+        site_models.read_fields or utils.comcam_tessellate is used to
+        read field positions.
     area_required : float (None)
-        The valid area that should be present in the reward function (square degrees).
+        The valid area that should be present in the reward
+        function (square degrees).
     npositions : int (7305)
-        The number of dither positions to pre-compute. Defaults to 7305 (so good for 20 years)
+        The number of dither positions to pre-compute. Defaults
+        to 7305 (so good for 20 years)
     """
 
     def __init__(
         self,
         basis_functions,
         basis_weights,
         extra_features=None,
@@ -496,16 +506,16 @@
 
         # Start tracking the night
         self.night = -1
 
         self.dither = dither
 
         # Generate and store rotation positions to use.
-        # This way, if different survey objects are seeded the same, they will
-        # use the same dither positions each night
+        # This way, if different survey objects are seeded the same,
+        # they will use the same dither positions each night
         rng = np.random.default_rng(seed)
         self.lon = rng.random(npositions) * np.pi * 2
         # Make sure latitude points spread correctly
         # http://mathworld.wolfram.com/SpherePointPicking.html
         self.lat = np.arccos(2.0 * rng.random(npositions) - 1.0)
         self.lon2 = rng.random(npositions) * np.pi * 2
 
@@ -522,16 +532,16 @@
             good_pix = np.where(np.isfinite(reward) == True)[0]
             area = hp.nside2pixarea(self.nside) * np.size(good_pix)
             if area < self.area_required:
                 return False
         return result
 
     def _hp2fieldsetup(self, ra, dec):
-        """Map each healpixel to nearest field. This will only work if healpix
-        resolution is higher than field resolution.
+        """Map each healpixel to nearest field. This will only work
+        if healpix resolution is higher than field resolution.
 
         Parameters
         ----------
         ra : `float`
             The RA of the possible pointings (radians)
         dec : `float`
             The decs of the possible pointings (radians)
@@ -549,21 +559,22 @@
             x, y, z = _xyz_from_ra_dec(hp_ra, hp_dec)
             dist, ind = tree.query(np.vstack([x, y, z]).T, k=1)
             self.hp2fields = ind
 
     def _spin_fields(self, conditions, lon=None, lat=None, lon2=None):
         """Spin the field tessellation to generate a random orientation
 
-        The default field tesselation is rotated randomly in longitude, and then the
-        pole is rotated to a random point on the sphere.
+        The default field tesselation is rotated randomly in longitude,
+        and then the pole is rotated to a random point on the sphere.
 
         Parameters
         ----------
         lon : float (None)
-            The amount to initially rotate in longitude (radians). Will use a random value
+            The amount to initially rotate in longitude (radians).
+            Will use a random value
             between 0 and 2 pi if None (default).
         lat : float (None)
             The amount to rotate in latitude (radians).
         lon2 : float (None)
             The amount to rotate the pole in longitude (radians).
         """
         if lon is None:
@@ -586,30 +597,29 @@
 
         # One more RA rotation
         ra = (ra + lon2) % (2.0 * np.pi)
 
         self.fields["RA"] = ra
         self.fields["dec"] = dec
         # Rebuild the kdtree with the new positions
-        # XXX-may be doing some ra,dec to conversions xyz more than needed.
+        # XXX-may be doing some ra,dec to conversions xyz more
+        # than needed.
         self._hp2fieldsetup(ra, dec)
 
     def smooth_reward(self):
         """If we want to smooth the reward function."""
         if hp.isnpixok(self.reward.size):
-            # Need to swap NaNs to hp.UNSEEN so smoothing doesn't spread mask
+            # Need to swap NaNs to hp.UNSEEN so smoothing doesn't
+            # spread mask
             reward_temp = copy(self.reward)
             mask = np.isnan(reward_temp)
             reward_temp[mask] = hp.UNSEEN
             self.reward_smooth = hp.sphtfunc.smoothing(reward_temp, fwhm=self.smoothing_kernel, verbose=False)
             self.reward_smooth[mask] = np.nan
             self.reward = self.reward_smooth
-            # good = ~np.isnan(self.reward_smooth)
-            # Round off to prevent strange behavior early on
-            # self.reward_smooth[good] = np.round(self.reward_smooth[good], decimals=4)
 
     def calc_reward_function(self, conditions):
         self.reward_checked = True
         if self._check_feasibility(conditions):
             self.reward = 0
             indx = np.arange(hp.nside2npix(self.nside))
             for bf, weight in zip(self.basis_functions, self.basis_weights):
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/dd_surveys.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/dd_surveys.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,32 +17,36 @@
 
 
 class DeepDrillingSurvey(BaseSurvey):
     """A survey class for running deep drilling fields.
 
     Parameters
     ----------
-    basis_functions : list of rubin_scheduler.scheduler.basis_function objects
+    basis_functions : list of rubin_scheduler.scheduler.basis_function
         These should be feasibility basis functions.
     RA : float
         The RA of the field (degrees)
     dec : float
         The dec of the field to observe (degrees)
     sequence : list of observation objects or str (rgizy)
-        The sequence of observations to take. Can be a string of list of obs objects.
+        The sequence of observations to take. Can be a string of
+        list of obs objects.
     nvis : list of ints
-        The number of visits in each filter. Should be same length as sequence.
+        The number of visits in each filter. Should be same length
+        as sequence.
     survey_name : str (DD)
         The name to give this survey so it can be tracked
     reward_value : float (101.)
         The reward value to report if it is able to start (unitless).
     readtime : float (2.)
-        Readout time for computing approximate time of observing the sequence. (seconds)
+        Readout time for computing approximate time of observing
+        the sequence. (seconds)
     flush_pad : float (30.)
-        How long to hold observations in the queue after they were expected to be completed (minutes).
+        How long to hold observations in the queue after they
+        were expected to be completed (minutes).
     """
 
     def __init__(
         self,
         basis_functions,
         RA,
         dec,
@@ -97,15 +101,16 @@
         # Let's just make this an array for ease of use
         self.observations = np.concatenate(self.observations)
         order = np.argsort(self.observations["filter"])
         self.observations = self.observations[order]
 
         n_filter_change = np.size(np.unique(self.observations["filter"]))
 
-        # Make an estimate of how long a seqeunce will take. Assumes no major rotational or spatial
+        # Make an estimate of how long a seqeunce will take.
+        # Assumes no major rotational or spatial
         # dithering slowing things down.
         self.approx_time = (
             np.sum(self.observations["exptime"] + readtime * self.observations["nexp"]) / 3600.0 / 24.0
             + filter_change_time * n_filter_change / 3600.0 / 24.0
         )  # to days
 
         if self.reward_value is None:
@@ -116,33 +121,37 @@
     def roi_hpid(self):
         hpid = ra_dec2_hpid(self.nside, np.degrees(self.ra), np.degrees(self.dec))
         return hpid
 
     def check_continue(self, observation, conditions):
         # feasibility basis functions?
         """
-        This method enables external calls to check if a given observations that belongs to this survey is
-        feasible or not. This is called once a sequence has started to make sure it can continue.
-
-        XXX--TODO:  Need to decide if we want to develope check_continue, or instead hold the
-        sequence in the survey, and be able to check it that way.
+        This method enables external calls to check if a given
+        observations that belongs to this survey is
+        feasible or not. This is called once a sequence has
+        started to make sure it can continue.
+
+        XXX--TODO:  Need to decide if we want to develope check_continue,
+        or instead hold the sequence in the survey, and be able to check
+        it that way.
         """
 
         result = True
 
         return result
 
     def calc_reward_function(self, conditions):
         result = -np.inf
         if self._check_feasibility(conditions):
             if self.reward_value is not None:
                 result = self.reward_value
             else:
-                # XXX This might backfire if we want to have DDFs with different fractions of the
-                # survey time. Then might need to define a goal fraction, and have the reward be the
+                # XXX This might backfire if we want to have DDFs with
+                # different fractions of the survey time. Then might need
+                # to define a goal fraction, and have the reward be the
                 # number of observations behind that target fraction.
                 result = self.extra_features["Ntot"].feature / (self.extra_features["N_survey"].feature + 1)
         return result
 
     def generate_observations_rough(self, conditions):
         result = []
         if self._check_feasibility(conditions):
@@ -155,15 +164,16 @@
             mask = np.isin(result["filter"], conditions.mounted_filters)
             result = result[mask]
             # Put current loaded filter first
             ind1 = np.where(result["filter"] == conditions.current_filter)[0]
             ind2 = np.where(result["filter"] != conditions.current_filter)[0]
             result = result[ind1.tolist() + (ind2.tolist())]
 
-            # convert to list of array. Arglebargle, don't understand why I need a reshape there
+            # convert to list of array. Arglebargle, don't understand
+            # why I need a reshape there
             final_result = [
                 row.reshape(
                     1,
                 )
                 for row in result
             ]
             result = final_result
@@ -376,15 +386,16 @@
     )
 
     # Euclid Fields
     # I can use the sequence kwarg to do two positions per sequence
     filters = "urgizy"
     nviss = nvis_master
     survey_name = "DD:EDFS"
-    # Note the sequences need to be in radians since they are using observation objects directly
+    # Note the sequences need to be in radians since they are using
+    # observation objects directly
     # Coords from jc.cuillandre@cea.fr Oct 15, 2020
     r_as = np.radians([locations["EDFS_a"][0], locations["EDFS_b"][0]])
     decs = np.radians([locations["EDFS_a"][1], locations["EDFS_b"][1]])
     suffixes = [", a", ", b"]
     sequence = []
 
     for filtername, nvis in zip(filters, nviss):
@@ -399,15 +410,16 @@
                 obs["RA"] = ra
                 obs["dec"] = dec
                 obs["nexp"] = nexp
                 obs["note"] = survey_name + suffix
                 sequence.append(obs)
 
     ha_limits = ([0.0, 1.5], [22.5, 24.0])
-    # And back to degrees for the basis function. Need to bump up the time needed since it's a double field.
+    # And back to degrees for the basis function. Need to bump up the
+    # time needed since it's a double field.
     bfs = dd_bfs(
         np.degrees(r_as[0]),
         np.degrees(decs[0]),
         survey_name,
         ha_limits,
         frac_total=frac_total,
         aggressive_frac=aggressive_frac,
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/ddf_presched.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/coordinate_transformations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,439 +1,585 @@
-__all__ = ("generate_ddf_scheduled_obs",)
+"""
+This file contains coordinate transformation methods that are
+very thin wrappers of palpy methods, or that have no
+dependence on palpy at all
+"""
+
+__all__ = (
+    "alt_az_pa_from_ra_dec",
+    "_alt_az_pa_from_ra_dec",
+    "spherical_from_cartesian",
+    "cartesian_from_spherical",
+    "xyz_from_ra_dec",
+    "_xyz_from_ra_dec",
+    "_ra_dec_from_xyz",
+    "ra_dec_from_xyz",
+    "xyz_angular_radius",
+    "_xyz_angular_radius",
+    "rotation_matrix_from_vectors",
+    "rot_about_z",
+    "rot_about_y",
+    "rot_about_x",
+    "calc_lmst",
+    "calc_lmst_astropy",
+    "angular_separation",
+    "_angular_separation",
+    "haversine",
+    "arcsec_from_radians",
+    "radians_from_arcsec",
+    "arcsec_from_degrees",
+    "degrees_from_arcsec",
+)
 
-import os
-import warnings
+import numbers
 
 import numpy as np
+from astropy import units as u
+from astropy.coordinates import AltAz, EarthLocation, SkyCoord
+from astropy.time import Time
+from astropy.utils.iers import conf
 
-from rubin_scheduler.data import get_data_dir
-from rubin_scheduler.scheduler.utils import scheduled_observation
-from rubin_scheduler.utils import calc_season, ddf_locations, survey_start_mjd
-
-
-def ddf_slopes(ddf_name, raw_obs, night_season):
-    """
-    Let's make custom slopes for each DDF
-
-    Parameters
-    ----------
-    ddf_name : str
-       The DDF name to use
-    raw_obs : np.array
-        An array with values of 1 or zero. One element per night, value of
-        1 indicates the night is during an active observing season.
-    night_season : np.array
-        An array of floats with the fractional season value
-        (e.g., 0.5 would be half way through the first season)
-    """
-
-    # OK, so 258 sequences is ~1% of the survey
-    # so a 25.8 sequences is a 0.1% season
-    # COSMOS is going to be 0.7% for 3 years, then 0.175 for the rest.
-
-    ss = 30  # standard season, was 45
-
-    if (ddf_name == "ELAISS1") | (ddf_name == "XMM_LSS") | (ddf_name == "ECDFS"):
-        # Dict with keys for each season and values of the number of sequences
-        # to attempt.
-        season_vals = {
-            0: 10,
-            1: ss,
-            2: ss,
-            3: ss,
-            4: ss,
-            5: ss,
-            6: ss,
-            7: ss,
-            8: ss,
-            9: ss,
-            10: 10,
-        }
-
-        round_season = np.floor(night_season)
-
-        cumulative_desired = np.zeros(raw_obs.size, dtype=float)
-        for season in np.unique(round_season):
-            in_season = np.where(round_season == season)
-            cumulative = np.cumsum(raw_obs[in_season])
-            if cumulative.max() > 0:
-                cumulative = cumulative / cumulative.max() * season_vals[season]
-                cumulative_desired[in_season] = cumulative + np.max(cumulative_desired)
-
-    if ddf_name == "EDFS_a":
-        season_vals = {
-            0: 10,
-            1: ss,
-            2: ss,
-            3: ss,
-            4: ss,
-            5: ss,
-            6: ss,
-            7: ss,
-            8: ss,
-            9: ss,
-            10: 10,
-        }
-
-        round_season = np.floor(night_season)
-
-        cumulative_desired = np.zeros(raw_obs.size, dtype=float)
-        for season in np.unique(round_season):
-            in_season = np.where(round_season == season)
-            cumulative = np.cumsum(raw_obs[in_season])
-            if cumulative.max() > 0:
-                cumulative = cumulative / cumulative.max() * season_vals[season]
-                cumulative_desired[in_season] = cumulative + np.max(cumulative_desired)
-
-    if ddf_name == "COSMOS":
-        # looks like COSMOS has no in-season time for 10 at the current start mjd.
-        season_vals = {
-            0: 10,
-            1: ss * 5,
-            2: ss * 5,
-            3: ss * 2,
-            4: ss,
-            5: ss,
-            6: ss,
-            7: ss,
-            8: ss,
-            9: ss,
-            10: 10,
-        }
-
-        round_season = np.floor(night_season)
-
-        cumulative_desired = np.zeros(raw_obs.size, dtype=float)
-        for season in np.unique(round_season):
-            in_season = np.where(round_season == season)[0]
-            cumulative = np.cumsum(raw_obs[in_season])
-            if cumulative.max() > 0:
-                cumulative = cumulative / cumulative.max() * season_vals[season]
-                cumulative_desired[in_season] = cumulative + np.max(cumulative_desired)
-
-    return cumulative_desired
-
-
-def match_cumulative(cumulative_desired, mask=None, no_duplicate=True):
-    """Generate a schedule that tries to match the desired cumulative distribution given a mask
-
-    Parameters
-    ----------
-    cumulative_desired : `np.array`, float
-        An array with the cumulative number of desired observations. Elements
-        are assumed to be evenly spaced.
-    mask : `np.array`, bool or int (None)
-        Set to zero for indices that cannot be scheduled
-    no_duplicate : `bool` (True)
-        If True, only 1 event can be scheduled per element
+from rubin_scheduler.utils.code_utilities import _validate_inputs
+
+
+def _wrap_hour_angle(ha_rad):
+    """wrap hour angle to go between -pi and pi"""
+
+    if np.size(ha_rad) == 1:
+        if ha_rad > np.pi:
+            ha_rad -= 2.0 * np.pi
+    else:
+        over = np.where(ha_rad > np.pi)[0]
+        ha_rad[over] -= 2.0 * np.pi
+
+    return ha_rad
+
+
+def alt_az_pa_from_ra_dec(ra, dec, mjd, site_longitude, site_latitude):
+    """ """
+
+    alt, az, pa = _alt_az_pa_from_ra_dec(
+        np.radians(ra), np.radians(dec), mjd, np.radians(site_longitude), np.radians(site_latitude)
+    )
+
+    return np.degrees(alt), np.degrees(az), np.degrees(pa)
+
+
+def _alt_az_pa_from_ra_dec(ra, dec, mjd, site_longitude, site_latitude):
+    """ """
+
+    observing_location = EarthLocation(
+        lat=site_latitude * u.rad, lon=site_longitude * u.rad, height=100 * u.m
+    )
+    observing_time = Time(mjd, format="mjd", location=observing_location)
+    aa = AltAz(location=observing_location, obstime=observing_time)
+    coord = SkyCoord(ra * u.rad, dec * u.rad)
+    altaz = coord.transform_to(aa)
+
+    lmst = observing_time.sidereal_time("mean")
+
+    hour_angle = _wrap_hour_angle(lmst.rad - ra)
+
+    # Position Angle Equation from:
+    # http://www.gb.nrao.edu/~rcreager/GBTMetrology/140ft/l0058/
+    # gbtmemo52/memo52.html
+    # or
+    # http://www.gb.nrao.edu/GBT/DA/gbtidl/release2pt9/contrib/
+    # contrib/parangle.pro
+    pa = np.arctan2(
+        np.sin(hour_angle),
+        (np.cos(dec) * np.tan(site_latitude) - np.sin(dec) * np.cos(hour_angle)),
+    )
+
+    return altaz.alt.rad, altaz.az.rad, pa
+
+
+def calc_lmst(mjd, longitude_rad):
+    """Calculate the LMST for a location
+    based on:  https://github.com/jhaupt/Sidereal-Time-Calculator/
+    blob/master/SiderealTimeCalculator.py
+    which uses:
+    http://aa.usno.navy.mil/faq/docs/JD_Formula.php
+    http://aa.usno.navy.mil/faq/docs/GAST.php and
+
+    Parameters
+    ----------
+    mjd : `float`
+        is the universal time (ut1) expressed as an MJD.
+        This can be a numpy array or a single value.
+    long_rad : `float`
+        is the longitude in radians (positive east of the prime meridian)
+        This can be numpy array or a single value.  If a numpy array,
+        should have the same length as mjd.  In that
+        case, each long_rad will be applied only to the corresponding mjd.
+
+    Returns
+    -------
+    lst : `float`
+        The local sidereal time in hours
+
+    """
+    gmst = 18.697374558 + 24.06570982441908 * (mjd - 51544.5)
+    gmst = gmst % 24  # to hours
+    longitude = np.degrees(longitude_rad) / 15.0  # Convert longi to hours
+    lst = gmst + longitude  # Fraction LST. If negative we want to add 24
+    if np.size(lst) == 1:
+        if lst < 0:
+            lst += 24
+    else:
+        lst[np.where(lst < 0)] += 24
+    return lst
+
+
+def calc_lmst_astropy(mjd, long_rad):
+    """
+    calculates local mean sidereal time
+
+    Parameters
+    ----------
+    mjd : `float`
+        is the universal time (ut1) expressed as an MJD.
+        This can be a numpy array or a single value.
+    long_rad : `float`
+        is the longitude in radians (positive east of the prime meridian)
+        This can be numpy array or a single value.  If a numpy array,
+        should have the same length as mjd.  In that
+        case, each long_rad will be applied only to the corresponding mjd.
+
+    Returns
+    -------
+    lmst : `float`
+        is the local mean sidereal time in hours
+    """
+    observing_location = EarthLocation(lat=0.0, lon=long_rad * u.rad, height=100 * u.m)
+    t = Time(mjd, format="mjd", location=observing_location)
+    # Ignore astropy if we wander too far into the future
+    with conf.set_temp("iers_degraded_accuracy", "warn"):
+        lmst = t.sidereal_time("mean").rad
+
+    # convert to hours
+    lmst = lmst * 12 / np.pi
+    return lmst
+
+
+def cartesian_from_spherical(longitude, latitude):
+    """
+    Transforms between spherical and Cartesian coordinates.
+
+    Parameters
+    ----------
+    longitude : `Unknown`
+        is a numpy array or a number in radians
+    latitude : `Unknown`
+        is a numpy array or number in radians
+    a : `Unknown`
+        numpy array of the (three-dimensional) cartesian
+        coordinates on a unit sphere.
+
+    if inputs are numpy arrays:
+    output[i][0] will be the x-coordinate of the ith point
+    output[i][1] will be the y-coordinate of the ith point
+    output[i][2] will be the z-coordinate of the ith point
+
+    All angles are in radians
+
+    Also, look at xyz_from_ra_dec().
+    """
+    return _xyz_from_ra_dec(longitude, latitude).transpose()
+
+
+def spherical_from_cartesian(xyz):
+    """
+    Transforms between Cartesian and spherical coordinates
+
+    Parameters
+    ----------
+    xyz : `Unknown`
+        is a numpy array of points in 3-D space.
+        Each row is a different point.
+    returns : `Unknown`
+        longitude and latitude
+
+    All angles are in radians
+
+    Also, look at ra_dec_from_xyz().
+    """
+    if not isinstance(xyz, np.ndarray):
+        raise RuntimeError("You need to pass a numpy array to spherical_from_cartesian")
+
+    if len(xyz.shape) > 1:
+        return _ra_dec_from_xyz(xyz[:, 0], xyz[:, 1], xyz[:, 2])
+    else:
+        return _ra_dec_from_xyz(xyz[0], xyz[1], xyz[2])
+
+
+def xyz_from_ra_dec(ra, dec):
+    """
+    Utility to convert RA,dec positions in x,y,z space.
+
+    Parameters
+    ----------
+    ra : float or array
+        RA in degrees
+    dec : float or array
+        Dec in degrees
+
+    Returns
+    -------
+    x,y,z : floats or arrays
+        The position of the given points on the unit sphere.
+    """
+    return _xyz_from_ra_dec(np.radians(ra), np.radians(dec))
+
+
+def _xyz_from_ra_dec(ra, dec):
+    """
+    Utility to convert RA,dec positions in x,y,z space.
+
+    Parameters
+    ----------
+    ra : float or array
+        RA in radians
+    dec : float or array
+        Dec in radians
+
+    Returns
+    -------
+    x,y,z : floats or arrays
+        The position of the given points on the unit sphere.
+    """
+    # It is ok to mix floats and numpy arrays.
+
+    cos_dec = np.cos(dec)
+    return np.array([np.cos(ra) * cos_dec, np.sin(ra) * cos_dec, np.sin(dec)])
+
+
+def _ra_dec_from_xyz(x, y, z):
+    """
+    Utility to convert x,y,z Cartesian coordinates to RA, dec
+    positions in space.
+
+    Parameters
+    ----------
+    x : float or array
+        The position on the x-axis of the given points on the unit sphere
+    y : float or array
+        The position on the y-axis of the given points on the unit sphere
+    z : float or array
+        The position on the z-axis of the given points on the unit sphere
+
+    Returns
+    -------
+    ra, dec : floats or arrays
+        Ra and dec coordinates in radians.
+    """
+    rad = np.sqrt(x**2 + y**2 + z**2)
+    ra = np.arctan2(y, x)
+    dec = np.arcsin(z / rad)
+
+    return ra, dec
+
+
+def ra_dec_from_xyz(x, y, z):
+    """
+    Utility to convert x,y,z Cartesian coordinates to RA, dec
+    positions in space.
+
+    Parameters
+    ----------
+    x : float or array
+        The position on the x-axis of the given points on the unit sphere
+    y : float or array
+        The position on the y-axis of the given points on the unit sphere
+    z : float or array
+        The position on the z-axis of the given points on the unit sphere
+
+    Returns
+    -------
+    ra, dec : floats or arrays
+        Ra and dec coordinates in degrees.
+    """
+
+    return np.degrees(_ra_dec_from_xyz(x, y, z))
+
+
+def xyz_angular_radius(radius=1.75):
+    """
+    Convert an angular radius into a physical radius for a kdtree search.
+
+    Parameters
+    ----------
+    radius : float
+        Radius in degrees.
 
     Returns
     -------
-    schedule : `np.array`
-        The resulting schedule, with values marking number of events in that cell.
+    radius : float
+    """
+    return _xyz_angular_radius(np.radians(radius))
+
+
+def _xyz_angular_radius(radius):
     """
+    Convert an angular radius into a physical radius for a kdtree search.
+
+    Parameters
+    ----------
+    radius : float
+        Radius in radians.
 
-    rounded_desired = np.round(cumulative_desired)
-    sched = cumulative_desired * 0
-    if mask is None:
-        mask = np.ones(sched.size)
-
-    valid = np.where(mask > 0)[0].tolist()
-    x = np.arange(sched.size)
-
-    drd = np.diff(rounded_desired)
-    step_points = np.where(drd > 0)[0] + 1
-
-    # would be nice to eliminate this loop, but it's not too bad.
-    # can't just use searchsorted on the whole array, because then there
-    # can be duplicate values, and array[[n,n]] = 1 means that extra match gets lost.
-    for indx in step_points:
-        left = np.searchsorted(x[valid], indx)
-        right = np.searchsorted(x[valid], indx, side="right")
-        d1 = indx - left
-        d2 = right - indx
-        if d1 < d2:
-            sched_at = left
-        else:
-            sched_at = right
-
-        # If we are off the end
-        if sched_at >= len(valid):
-            sched_at -= 1
-
-        sched[valid[sched_at]] += 1
-        if no_duplicate:
-            valid.pop(sched_at)
-
-    return sched
-
-
-def optimize_ddf_times(
-    ddf_name,
-    ddf_RA,
-    ddf_grid,
-    sun_limit=-18,
-    sequence_time=60.0,
-    airmass_limit=2.5,
-    sky_limit=None,
-    g_depth_limit=23.5,
-    season_unobs_frac=0.1,
-):
-    """
-
-    Parameters
-    ----------
-    ddf : `str`
-        The name of the DDF
-    ddf_grid : `np.array`
-        An array with info for the DDFs. Generated by the
-        rubin_scheduler.scheduler/surveys/generate_ddf_grid.py` script
-    season_unobs_frac : `float`
-        7.2 month observing season if season_unobs_frac = 0.2 (shaves 20% off
-        each end of the full year)
-    sequence_time : `float`
-        How long a sequence is expected to be (minutes). Used to make
-        sure things are not scheduled too close to twilight.
-    """
-    sun_limit = np.radians(sun_limit)
-    sequence_time = sequence_time / 60.0 / 24.0  # to days
-
-    # XXX-- double check that I got this right
-    ack = ddf_grid["sun_alt"][0:-1] * ddf_grid["sun_alt"][1:]
-    night = np.zeros(ddf_grid.size, dtype=int)
-    night[np.where((ddf_grid["sun_alt"][1:] >= 0) & (ack < 0))] += 1
-    night = np.cumsum(night)
-    ngrid = ddf_grid["mjd"].size
-
-    # set a sun, airmass, sky masks
-    sun_mask = np.ones(ngrid, dtype=int)
-    sun_mask[np.where(ddf_grid["sun_alt"] >= sun_limit)] = 0
-
-    # expand sun mask backwards by the sequence time.
-    n_back = np.ceil(sequence_time / (ddf_grid["mjd"][1] - ddf_grid["mjd"][0])).astype(int)
-    shadow_indx = np.where(sun_mask == 0)[0] - n_back
-    shadow_indx = shadow_indx[np.where(shadow_indx >= 0)]
-
-    sun_mask[shadow_indx] = 0
-
-    airmass_mask = np.ones(ngrid, dtype=int)
-    airmass_mask[np.where(ddf_grid["%s_airmass" % ddf_name] >= airmass_limit)] = 0
-
-    sky_mask = np.ones(ngrid, dtype=int)
-    if sky_limit is not None:
-        sky_mask[np.where(ddf_grid["%s_sky_g" % ddf_name] <= sky_limit)] = 0
-        sky_mask[np.where(np.isnan(ddf_grid["%s_sky_g" % ddf_name]) == True)] = 0
-
-    m5_mask = np.zeros(ngrid, dtype=bool)
-    m5_mask[np.isfinite(ddf_grid["%s_m5_g" % ddf_name])] = 1
-
-    if g_depth_limit is not None:
-        m5_mask[np.where(ddf_grid["%s_m5_g" % ddf_name] < g_depth_limit)] = 0
-
-    big_mask = sun_mask * airmass_mask * sky_mask * m5_mask
-
-    potential_nights = np.unique(night[np.where(big_mask > 0)])
-
-    # prevent a repeat sequence in a night
-    unights, indx = np.unique(night, return_index=True)
-    night_mjd = ddf_grid["mjd"][indx]
-    # The season of each night
-    night_season = calc_season(ddf_RA, night_mjd)
-
-    raw_obs = np.ones(unights.size)
-    # take out the ones that are out of season
-    season_mod = night_season % 1
-
-    out_season = np.where((season_mod < season_unobs_frac) | (season_mod > (1.0 - season_unobs_frac)))
-    raw_obs[out_season] = 0
-
-    cumulative_desired = ddf_slopes(ddf_name, raw_obs, night_season)
-
-    night_mask = unights * 0
-    night_mask[potential_nights] = 1
-
-    unight_sched = match_cumulative(cumulative_desired, mask=night_mask)
-    cumulative_sched = np.cumsum(unight_sched)
-
-    nights_to_use = unights[np.where(unight_sched == 1)]
-
-    # For each night, find the best time in the night.
-    # XXX--probably need to expand this part to resolve the times when multiple things get scheduled
-    mjds = []
-    for night_check in nights_to_use:
-        in_night = np.where((night == night_check) & (np.isfinite(ddf_grid["%s_m5_g" % ddf_name])))[0]
-        m5s = ddf_grid["%s_m5_g" % ddf_name][in_night]
-        # we could intorpolate this to get even better than 15 min resolution on when to observe
-        max_indx = np.where(m5s == m5s.max())[0].min()
-        mjds.append(ddf_grid["mjd"][in_night[max_indx]])
-
-    return mjds, night_mjd, cumulative_desired, cumulative_sched
-
-
-def generate_ddf_scheduled_obs(
-    data_file=None,
-    flush_length=2,
-    mjd_tol=15,
-    expt=30.0,
-    alt_min=25,
-    alt_max=85,
-    HA_min=21.0,
-    HA_max=3.0,
-    sun_alt_max=-18,
-    dist_tol=3.0,
-    season_unobs_frac=0.1,
-    nvis_master=[8, 10, 20, 20, 24, 18],
-    filters="ugrizy",
-    nsnaps=[1, 2, 2, 2, 2, 2],
-    mjd_start=None,
-    survey_length=10.0,
-    sequence_time=60.0,
-):
-    """
-
-    Parameters
-    ----------
-    data_file : `path` (None)
-        The data file to use for DDF airmass, m5, etc. Defaults to using whatever is in
-        rubin_sim_data/scheduler directory.
-    flush_length : `float` (2)
-        How long to keep a scheduled observation around before it is considered failed
-        and flushed (days).
-    mjd_tol : `float` (15)
-        How close an observation must be in time to be considered matching a scheduled
-        observation (minutes).
-    expt : `float` (30)
-        Total exposure time per visit (seconds).
-    alt_min/max : `float` (25, 85)
-        The minimum and maximum altitudes to permit observations to happen (degrees).
-    HA_min/max : `float` (21, 3)
-        The hour angle limits to permit observations to happen (hours).
-    dist_tol : `float` (3)
-        The distance tolerance for a visit to be considered matching a scheduled observation
-        (degrees).
-    season_unobs_frac : `float` (0.1)
-        What fraction of the season should the DDF be considered unobservable. Taken off both the
-        start and end of the year, so a season frac of 0.1 means 20% of the time the DDF is considered
-        unobservable, so it will be in-season for 9.6 months.
-    nvis_master : list of ints ([8, 10, 20, 20, 24, 18])
-        The number of visits to make per filter
-    filters : `str` (ugrizy)
-        The filter names.
-    nsnaps : `list of ints` ([1, 2, 2, 2, 2, 2])
-        The number of snaps to use per filter
-    mjd_start : `float`
-        Starting MJD of the survey. Default None, which calls rubin_sim.utils.survey_start_mjd
-    survey_length : `float`
-        Length of survey (years). Default 10.
-    """
-    if data_file is None:
-        data_file = os.path.join(get_data_dir(), "scheduler", "ddf_grid.npz")
-
-    if mjd_start is None:
-        mjd_start = survey_start_mjd()
-
-    flush_length = flush_length  # days
-    mjd_tol = mjd_tol / 60 / 24.0  # minutes to days
-    expt = expt
-    alt_min = np.radians(alt_min)
-    alt_max = np.radians(alt_max)
-    dist_tol = np.radians(dist_tol)
-    sun_alt_max = np.radians(sun_alt_max)
-
-    ddfs = ddf_locations()
-    ddf_data = np.load(data_file)
-    ddf_grid = ddf_data["ddf_grid"].copy()
-
-    mjd_max = mjd_start + survey_length * 365.25
-
-    # check if our pre-computed grid is over the time range we think we are scheduling for
-    if (ddf_grid["mjd"].min() > mjd_start) | (ddf_grid["mjd"].max() < mjd_max):
-        warnings.warn("Pre-computed DDF properties don't match requested survey times")
-
-    in_range = np.where((ddf_grid["mjd"] >= mjd_start) & (ddf_grid["mjd"] <= mjd_max))
-    ddf_grid = ddf_grid[in_range]
-
-    all_scheduled_obs = []
-    for ddf_name in ["ELAISS1", "XMM_LSS", "ECDFS", "COSMOS", "EDFS_a"]:
-        print("Optimizing %s" % ddf_name)
-
-        # 'ID', 'RA', 'dec', 'mjd', 'flush_by_mjd', 'exptime', 'filter', 'rotSkyPos', 'nexp',
-        #         'note'
-        # 'mjd_tol', 'dist_tol', 'alt_min', 'alt_max', 'HA_max', 'HA_min', 'observed'
-        mjds = optimize_ddf_times(
-            ddf_name,
-            ddfs[ddf_name][0],
-            ddf_grid,
-            season_unobs_frac=season_unobs_frac,
-            sequence_time=sequence_time,
-        )[0]
-        for mjd in mjds:
-            for filtername, nvis, nexp in zip(filters, nvis_master, nsnaps):
-                if "EDFS" in ddf_name:
-                    obs = scheduled_observation(n=int(nvis / 2))
-                    obs["RA"] = np.radians(ddfs[ddf_name][0])
-                    obs["dec"] = np.radians(ddfs[ddf_name][1])
-                    obs["mjd"] = mjd
-                    obs["flush_by_mjd"] = mjd + flush_length
-                    obs["exptime"] = expt
-                    obs["filter"] = filtername
-                    obs["nexp"] = nexp
-                    obs["note"] = "DD:%s" % ddf_name
-                    obs["target"] = ddf_name
-
-                    obs["mjd_tol"] = mjd_tol
-                    obs["dist_tol"] = dist_tol
-                    # Need to set something for HA limits
-                    obs["HA_min"] = HA_min
-                    obs["HA_max"] = HA_max
-                    obs["alt_min"] = alt_min
-                    obs["alt_max"] = alt_max
-                    obs["sun_alt_max"] = sun_alt_max
-                    all_scheduled_obs.append(obs)
-
-                    obs = scheduled_observation(n=int(nvis / 2))
-                    obs["RA"] = np.radians(ddfs[ddf_name.replace("_a", "_b")][0])
-                    obs["dec"] = np.radians(ddfs[ddf_name.replace("_a", "_b")][1])
-                    obs["mjd"] = mjd
-                    obs["flush_by_mjd"] = mjd + flush_length
-                    obs["exptime"] = expt
-                    obs["filter"] = filtername
-                    obs["nexp"] = nexp
-                    obs["note"] = "DD:%s" % ddf_name.replace("_a", "_b")
-                    obs["target"] = ddf_name.replace("_a", "_b")
-
-                    obs["mjd_tol"] = mjd_tol
-                    obs["dist_tol"] = dist_tol
-                    # Need to set something for HA limits
-                    obs["HA_min"] = HA_min
-                    obs["HA_max"] = HA_max
-                    obs["alt_min"] = alt_min
-                    obs["alt_max"] = alt_max
-                    obs["sun_alt_max"] = sun_alt_max
-                    all_scheduled_obs.append(obs)
-
-                else:
-                    obs = scheduled_observation(n=nvis)
-                    obs["RA"] = np.radians(ddfs[ddf_name][0])
-                    obs["dec"] = np.radians(ddfs[ddf_name][1])
-                    obs["mjd"] = mjd
-                    obs["flush_by_mjd"] = mjd + flush_length
-                    obs["exptime"] = expt
-                    obs["filter"] = filtername
-                    obs["nexp"] = nexp
-                    obs["note"] = "DD:%s" % ddf_name
-                    obs["target"] = ddf_name
-
-                    obs["mjd_tol"] = mjd_tol
-                    obs["dist_tol"] = dist_tol
-                    # Need to set something for HA limits
-                    obs["HA_min"] = HA_min
-                    obs["HA_max"] = HA_max
-                    obs["alt_min"] = alt_min
-                    obs["alt_max"] = alt_max
-                    obs["sun_alt_max"] = sun_alt_max
-                    all_scheduled_obs.append(obs)
-
-    result = np.concatenate(all_scheduled_obs)
-    # Put in the scripted ID so it's easier to track which ones fail.
-    result["scripted_id"] = np.arange(result.size)
+    Returns
+    -------
+    radius : float
+    """
+    x0, y0, z0 = (1, 0, 0)
+    x1, y1, z1 = _xyz_from_ra_dec(radius, 0)
+    result = np.sqrt((x1 - x0) ** 2 + (y1 - y0) ** 2 + (z1 - z0) ** 2)
     return result
+
+
+def z_rotation_matrix(theta):
+    cc = np.cos(theta)
+    ss = np.sin(theta)
+    return np.array([[cc, -ss, 0.0], [ss, cc, 0.0], [0.0, 0.0, 1.0]])
+
+
+def rot_about_z(vec, theta):
+    """
+    Rotate a Cartesian vector an angle theta about the z axis.
+    Theta is in radians.
+    Positive theta rotates +x towards +y.
+    """
+    return np.dot(z_rotation_matrix(theta), vec.transpose()).transpose()
+
+
+def y_rotation_matrix(theta):
+    cc = np.cos(theta)
+    ss = np.sin(theta)
+    return np.array([[cc, 0.0, ss], [0.0, 1.0, 0.0], [-ss, 0.0, cc]])
+
+
+def rot_about_y(vec, theta):
+    """
+    Rotate a Cartesian vector an angle theta about the y axis.
+    Theta is in radians.
+    Positive theta rotates +x towards -z.
+    """
+    return np.dot(y_rotation_matrix(theta), vec.transpose()).transpose()
+
+
+def x_rotation_matrix(theta):
+    cc = np.cos(theta)
+    ss = np.sin(theta)
+
+    return np.array([[1.0, 0.0, 0.0], [0.0, cc, -ss], [0.0, ss, cc]])
+
+
+def rot_about_x(vec, theta):
+    """
+    Rotate a Cartesian vector an angle theta about the x axis.
+    Theta is in radians.
+    Positive theta rotates +y towards +z.
+    """
+    return np.dot(x_rotation_matrix(theta), vec.transpose()).transpose()
+
+
+def rotation_matrix_from_vectors(v1, v2):
+    """
+    Given two vectors v1,v2 calculate the rotation matrix for v1->v2
+    using the axis-angle approach
+
+    Parameters
+    ----------
+    v1,v2 : `Unknown`
+        Cartesian unit vectors (in three dimensions).
+    rot : `Unknown`
+        is the rotation matrix that rotates from one to the other
+    """
+
+    if np.abs(np.sqrt(np.dot(v1, v1)) - 1.0) > 0.01:
+        raise RuntimeError("v1 in rotation_matrix_from_vectors is not a unit vector")
+
+    if np.abs(np.sqrt(np.dot(v2, v2)) - 1.0) > 0.01:
+        raise RuntimeError("v2 in rotation_matrix_from_vectors is not a unit vector")
+
+    # Calculate the axis of rotation by the cross product of v1 and v2
+    cross = np.cross(v1, v2)
+    cross = cross / np.sqrt(np.dot(cross, cross))
+
+    # calculate the angle of rotation via dot product
+    angle = np.arccos(np.dot(v1, v2))
+    sin_dot = np.sin(angle)
+    cos_dot = np.cos(angle)
+
+    # calculate the corresponding rotation matrix
+    # http://en.wikipedia.org/wiki/Rotation_matrix#
+    # Rotation_matrix_from_axis_and_angle
+    rot = [
+        [
+            cos_dot + cross[0] * cross[0] * (1 - cos_dot),
+            -cross[2] * sin_dot + (1 - cos_dot) * cross[0] * cross[1],
+            cross[1] * sin_dot + (1 - cos_dot) * cross[0] * cross[2],
+        ],
+        [
+            cross[2] * sin_dot + (1 - cos_dot) * cross[0] * cross[1],
+            cos_dot + (1 - cos_dot) * cross[1] * cross[1],
+            -cross[0] * sin_dot + (1 - cos_dot) * cross[1] * cross[2],
+        ],
+        [
+            -cross[1] * sin_dot + (1 - cos_dot) * cross[0] * cross[2],
+            cross[0] * sin_dot + (1 - cos_dot) * cross[1] * cross[2],
+            cos_dot + (1 - cos_dot) * (cross[2] * cross[2]),
+        ],
+    ]
+
+    return rot
+
+
+def _angular_separation(long1, lat1, long2, lat2):
+    """
+    Angular separation between two points in radians
+
+    Parameters
+    ----------
+    long1 is the first longitudinal coordinate in radians
+
+    lat1 is the first latitudinal coordinate in radians
+
+    long2 is the second longitudinal coordinate in radians
+
+    lat2 is the second latitudinal coordinate in radians
+
+    Returns
+    -------
+    The angular separation between the two points in radians
+
+    Calculated based on the haversine formula
+    From http://en.wikipedia.org/wiki/Haversine_formula
+    """
+    are_arrays_1 = _validate_inputs([long1, lat1], ["long1", "lat1"], "angular_separation")
+
+    are_arrays_2 = _validate_inputs([long2, lat2], ["long2", "lat2"], "angular_separation")
+
+    # The code below is necessary because the call to np.radians() in
+    # angular_separation() will automatically convert floats
+    # into length 1 numpy arrays, confusing validate_inputs()
+    if are_arrays_1 and len(long1) == 1:
+        are_arrays_1 = False
+        long1 = long1[0]
+        lat1 = lat1[0]
+
+    if are_arrays_2 and len(long2) == 1:
+        are_arrays_2 = False
+        long2 = long2[0]
+        lat2 = lat2[0]
+
+    if are_arrays_1 and are_arrays_2:
+        if len(long1) != len(long2):
+            raise RuntimeError(
+                "You need to pass arrays of the same length " "as arguments to angular_separation()"
+            )
+
+    t1 = np.sin(lat2 / 2.0 - lat1 / 2.0) ** 2
+    t2 = np.cos(lat1) * np.cos(lat2) * np.sin(long2 / 2.0 - long1 / 2.0) ** 2
+    _sum = t1 + t2
+
+    if isinstance(_sum, numbers.Number):
+        if _sum < 0.0:
+            _sum = 0.0
+    else:
+        _sum = np.where(_sum < 0.0, 0.0, _sum)
+
+    return 2.0 * np.arcsin(np.sqrt(_sum))
+
+
+def angular_separation(long1, lat1, long2, lat2):
+    """
+    Angular separation between two points in degrees
+
+    Parameters
+    ----------
+    long1 is the first longitudinal coordinate in degrees
+
+    lat1 is the first latitudinal coordinate in degrees
+
+    long2 is the second longitudinal coordinate in degrees
+
+    lat2 is the second latitudinal coordinate in degrees
+
+    Returns
+    -------
+    The angular separation between the two points in degrees
+    """
+    return np.degrees(
+        _angular_separation(np.radians(long1), np.radians(lat1), np.radians(long2), np.radians(lat2))
+    )
+
+
+def haversine(long1, lat1, long2, lat2):
+    """
+    DEPRECATED; use angular_separation() instead
+
+    Return the angular distance between two points in radians
+
+    Parameters
+    ----------
+    long1 : `Unknown`
+        is the longitude of point 1 in radians
+    lat1 : `Unknown`
+        is the latitude of point 1 in radians
+    long2 : `Unknown`
+        is the longitude of point 2 in radians
+    lat2 : `Unknown`
+        is the latitude of point 2 in radians
+    the : `Unknown`
+        angular separation between points 1 and 2 in radians
+    """
+    return _angular_separation(long1, lat1, long2, lat2)
+
+
+def arcsec_from_radians(value):
+    """
+    Convert an angle in radians to arcseconds
+
+    Note: if you input None, you will get None back
+    """
+    if value is None:
+        return None
+
+    return 3600.0 * np.degrees(value)
+
+
+def radians_from_arcsec(value):
+    """
+    Convert an angle in arcseconds to radians
+
+    Note: if you input None, you will get None back
+    """
+    if value is None:
+        return None
+
+    return np.radians(value / 3600.0)
+
+
+def arcsec_from_degrees(value):
+    """
+    Convert an angle in degrees to arcseconds
+
+    Note: if you input None, you will get None back
+    """
+    if value is None:
+        return None
+
+    return 3600.0 * value
+
+
+def degrees_from_arcsec(value):
+    """
+    Convert an angle in arcseconds to degrees
+
+    Note: if you input None, you will get None back
+    """
+    if value is None:
+        return None
+
+    return value / 3600.0
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/desc_ddf.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/desc_ddf.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,26 +63,30 @@
                 n_exp_in_seq = np.sum(list(sequence.values()))
                 time_needed = filter_change_time * len(sequence.keys())
                 time_needed += exptime * n_exp_in_seq
                 time_needed += readtime * n_exp_in_seq * nexp
                 self.approx_times.append(time_needed / 3600.0 / 24.0)
 
         # Track what we last tried to do
-        # XXX-this should probably go into self.extra_features or something for consistency.
+        # XXX-this should probably go into self.extra_features or
+        # something for consistency.
         self.sequence_index = 0
         self.last_night_observed = -100
 
     def check_continue(self, observation, conditions):
         # feasibility basis functions?
         """
-        This method enables external calls to check if a given observations that belongs to this survey is
-        feasible or not. This is called once a sequence has started to make sure it can continue.
+        This method enables external calls to check if a given
+        observations that belongs to this survey is
+        feasible or not. This is called once a sequence has started to
+        make sure it can continue.
 
-        XXX--TODO:  Need to decide if we want to develope check_continue, or instead hold the
-        sequence in the survey, and be able to check it that way.
+        XXX--TODO:  Need to decide if we want to develope check_continue
+         or instead hold the sequence in the survey, and be able to check
+         it that way.
         """
 
         result = True
         return result
 
     def _check_feasibility(self, conditions):
         """
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/field_survey.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/field_survey.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/generate_ddf_grid.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/generate_ddf_grid.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,40 +14,36 @@
 
 def generate_ddf_grid(
     verbose=True,
     mjd0=59560.2,
     delta_t=15.0,
     survey_length=40.0,
     sun_limit=-12,
-    nominal_seeing=0.7,
-    filtername="g",
     nominal_expt=30.0,
 ):
     """Pre-compute conditions for DDF locations over survey
 
     Parameters
     ----------
-    mjd0 : float
+    mjd0 : `float`
         The start MJD of the grid
-    delta_t : float
+    delta_t : `float`
         Spacing of time steps in minutes. Default 15
-    survey_length : float
+    survey_length : `float`
         Full span of DDF grid (years). Default 40.
-    sun_limit : float
-        Ignore times with sun above sun limit in degrees. Default -12.
-    nominal_seeling : float
-        Nominal seeing in arcseconds to assume for depth calculations. Default 0.7
-    filtername : str
-        The filter to use for the grid, default g
-    nominal_expt : float
-        Nominal exposure time in seconds to use for depth visits. Default 30
+    sun_limit : `float`
+        Ignore times with sun above sun limit in degrees.
+        Default -12.
+    nominal_expt : `float`
+        Nominal exposure time in seconds to use for depth visits.
+        Default 30
     """
 
     # Technically this script should be over in rubin_sim, but here to be more
-    # easily found. Burry import here so it's hopefully not a problem.
+    # easily found. Bury import here so it's hopefully not a problem.
     import rubin_sim.skybrightness as sb
     from astroplan import Observer
 
     dds = ddf_locations()
     delta_t = delta_t / 60.0 / 24.0  # to days
     survey_length = survey_length * 365.25
     sun_limit = np.radians(sun_limit)  # degrees
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/long_gap_survey.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/long_gap_survey.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,29 +14,34 @@
 
 
 class LongGapSurvey(BaseSurvey):
     """
     Parameters
     ----------
     blob_survey : rubin_scheduler.scheduler.surveys.BlobSurvey
-        A survey object that we will want to take repeat measurments of sometime later in the evening
+        A survey object that we will want to take repeat measurments of
+        sometime later in the evening
     scripted_survey : rubin_scheduler.scheduler.surveys.ScriptedSurvey
-        A scripted survey object that will have a queue updated with objects to observe later.
+        A scripted survey object that will have a queue updated with
+        objects to observe later.
     gap range : list of 2 floats
         The desired gap range (hours)
     long_name : str
-        The string to put in the observation 'note' for the scripted observations
+        The string to put in the observation 'note' for the scripted
+        observations
     scripted_tol : float
         The tolerance for when scripted observations can execute (hours)
     after_meridian : bool (False)
-        If True, force the scripted obsrevations to happen after they pass through the meridian.
-        This can help make sure we don't hit the zenith exclusion zone.
+        If True, force the scripted obsrevations to happen after they
+        pass through the meridian. This can help make sure we don't hit
+        the zenith exclusion zone.
     hour_step : float (0.5)
-        The amount of time to step scheduled observations forward if they could try to execute in the
-        zenith avoidance area (hours). Only used if `avoid_zenith` is True.
+        The amount of time to step scheduled observations forward if
+        they could try to execute in the zenith avoidance area (hours).
+        Only used if `avoid_zenith` is True.
     ha_min(_max) : float (0,24)
         Trying to set so they don't acctually get used.
 
     """
 
     def __init__(
         self,
@@ -90,19 +95,20 @@
 
     def _generate_survey_name(self):
         self.survey_name = (
             f"Long Gap ({self.blob_survey.survey_name} +" f" {self.scripted_survey.survey_name})"
         )
 
     def _schedule_obs(self, observations):
-        """Take incoming observations and decide if they should be added to the
-        scripted survey to try and be observered again later
+        """Take incoming observations and decide if they should be added
+        to the scripted survey to try and be observered again later
         """
 
-        # Only match if we have completed the second of a pair and are in most recent night.
+        # Only match if we have completed the second of a pair and are
+        # in most recent night.
         # ugh, stupid np.where doesn't support using scalars anymore
         if np.size(observations) == 1:
             if (observations["note"] == self.blob_survey.survey_note + ", b") & (
                 observations["night"] == np.max(observations["night"])
             ):
                 need_to_observe = np.array([0])
             else:
@@ -112,15 +118,16 @@
                 (observations["note"] == self.blob_survey.survey_note + ", b")
                 & (observations["night"] == np.max(observations["night"]))
             )[0]
 
         # Set to the proper gap
         self.gap = self.gaps[np.max(observations["night"])]
 
-        # If the incoming observation needs to have something scheduled later
+        # If the incoming observation needs to have something
+        # scheduled later
         if np.size(need_to_observe) > 0:
             sched_array = scheduled_observation(n=need_to_observe.size)
             for dt in np.intersect1d(observations.dtype.names, sched_array.dtype.names):
                 if np.size(observations) == 1:
                     sched_array[dt] = observations[dt]
                 else:
                     sched_array[dt] = observations[need_to_observe][dt]
@@ -144,15 +151,16 @@
                 earliest_mjd = sched_array["mjd"] - sched_array["mjd_tol"]
                 alts = []
                 mjds = np.arange(
                     np.min(earliest_mjd),
                     np.max(sched_array["mjd"]) + self.mjd_step,
                     self.mjd_step,
                 )
-                # Let's compute the alt of everything at earliest and scheduled
+                # Let's compute the alt of everything at earliest and
+                # scheduled
                 for mjd in mjds:
                     alt, az = _approx_ra_dec2_alt_az(
                         sched_array["RA"],
                         sched_array["dec"],
                         self.site.latitude_rad,
                         self.site.longitude_rad,
                         mjd,
@@ -166,28 +174,30 @@
                     earliest_mjd = sched_array["mjd"] - sched_array["mjd_tol"]
                     # Let's compute the alt of everything then
                     mjds = np.arange(
                         np.min(earliest_mjd),
                         np.max(sched_array["mjd"]) + self.mjd_step,
                         self.mjd_step,
                     )
-                    # Let's compute the alt of everything at earliest and scheduled
+                    # Let's compute the alt of everything at earliest
+                    # and scheduled
                     for mjd in mjds:
                         alt, az = _approx_ra_dec2_alt_az(
                             sched_array["RA"],
                             sched_array["dec"],
                             self.site.latitude_rad,
                             self.site.longitude_rad,
                             mjd,
                         )
                         alts.append(np.max(alt))
             # Make sure these have the note filled in
             sched_array["note"] = self.long_name
 
-            # See if we need to append things to the scripted survey object
+            # See if we need to append things to the scripted survey
+            # object
             if self.scripted_survey.obs_wanted is not None:
                 sched_array = np.concatenate([self.scripted_survey.obs_wanted, sched_array])
 
             self.scripted_survey.set_script(sched_array)
 
     def add_observations_array(self, observations_array_in, observations_hpid_in):
         self._schedule_obs(observations_array_in)
@@ -217,15 +227,16 @@
             # Clear out the scheduled observations
             self.scripted_survey.clear_script()
             self.night = copy(conditions.night)
             self.gap = self.gaps[conditions.night]
             time_remaining = conditions.sun_n18_rising - conditions.mjd
             if self.gap > time_remaining:
                 self.gap = time_remaining - self.block_length
-            # XXX-need to reach into the blob and set what the gap is I guess
+            # XXX-need to reach into the blob and set what the gap
+            # is I guess
 
         self.r1 = self.blob_survey.calc_reward_function(conditions)
         self.r2 = self.scripted_survey.calc_reward_function(conditions)
         self.reward_checked = True
         return np.nanmax([np.nanmax(self.r1), np.nanmax(self.r2)])
 
     def generate_observations_rough(self, conditions):
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/plan_night_survey.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/plan_night_survey.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,30 @@
 import rubin_scheduler.scheduler.basis_functions as bfs
 from rubin_scheduler.scheduler import features
 
 from .surveys import BlobSurvey
 
 
 class PlanAheadSurvey(BlobSurvey):
-    """Have a survey object that can plan ahead if it will want to observer a blob later in the night
+    """Have a survey object that can plan ahead if it will want to
+    observer a blob later in the night
 
     Parameters
     ----------
     delta_mjd_tol : float
-        The tolerance to alow on when to execute scheduled observations (days)
+        The tolerance to alow on when to execute scheduled observations
+        (days)
     minimum_sky_area : float
-        The minimum sky area to demand before making a scheduled observation (square degrees)
+        The minimum sky area to demand before making a scheduled
+        observation (square degrees)
     track_filters : str
         The filter name we want to prevent long gaps on
     in_season : float
-        The distance in RA from the meridian at midnight to consider (hours). This is the half-width
+        The distance in RA from the meridian at midnight to consider
+        (hours). This is the half-width
     cadence : float
         Ignore gaps below this length (days)
     """
 
     def __init__(
         self,
         basis_functions,
@@ -36,38 +40,31 @@
         minimum_sky_area=200.0,
         track_filters="g",
         in_season=2.5,
         cadence=9,
         **kwargs,
     ):
         super(PlanAheadSurvey, self).__init__(basis_functions, basis_weights, **kwargs)
-        # note that self.night is already being used for tracking tesselation.
-        # So here's an attribute for seeing if the night has changed for cadence tracking
+        # note that self.night is already being used for tracking
+        # tesselation. So here's an attribute for seeing if the night
+        # has changed for cadence tracking
         self.night_cad = -100
         self.scheduled_obs = None
         self.delta_mjd_tol = delta_mjd_tol
         self.minimum_sky_area = minimum_sky_area  # sq degrees
         self.extra_features = {}
         self.extra_features["last_observed"] = features.Last_observed(filtername=track_filters)
         self.extra_basis_functions = {}
         self.extra_basis_functions["moon_mask"] = bfs.Moon_avoidance_basis_function()
         self.track_filters = track_filters
         self.in_season = in_season / 12.0 * np.pi  # to radians
 
         self.pix_area = hp.nside2pixarea(self.nside, degrees=True)
         self.cadence = cadence
 
-    # def add_observation(self, observation, **kwargs):
-    #    # If a relevant observation got made, recompute when we actually want to observe in the night
-    #    if observation['filter'] in self.track_filters:
-    #        if self.scheduled_obs is not None:
-    #            # this will force a run of self.check_night on the next calc_reward_function
-    #            self.night = observation['night'] - 1
-    #    super(PlanAheadSurvey, self).add_observation(observation, **kwargs)
-
     def check_night(self, conditions):
         """"""
         delta_mjd = conditions.mjd - self.extra_features["last_observed"].feature
         moon_mask = self.extra_basis_functions["moon_mask"](conditions)
 
         pix_to_obs = np.where(
             (delta_mjd > self.cadence)
@@ -76,15 +73,16 @@
         )[0]
 
         area = np.size(pix_to_obs) * self.pix_area
 
         # If there are going to be some observations at a given time
         if area > self.minimum_sky_area:
             # Maybe just calculate the mean (with angles)
-            # Via https://en.wikipedia.org/wiki/Mean_of_circular_quantities
+            # Via https://en.wikipedia.org/wiki/
+            # Mean_of_circular_quantities
             mean_ra = np.arctan2(
                 np.mean(np.sin(conditions.ra[pix_to_obs])),
                 np.mean(np.cos(conditions.ra[pix_to_obs])),
             )
             if mean_ra < 0:
                 mean_ra += 2.0 * np.pi
 
@@ -106,24 +104,27 @@
         self.reward = -np.inf
         if self._check_feasibility(conditions):
             if self.night_cad != conditions.night:
                 self.check_night(conditions)
                 self.night_cad = copy(conditions.night)
 
             if self.scheduled_obs is not None:
-                # If there are scheduled observations, and we are in the correct time window
+                # If there are scheduled observations, and we are in
+                # the correct time window
                 delta_mjd = conditions.mjd - self.scheduled_obs
                 if (np.abs(delta_mjd) < self.delta_mjd_tol) & (self.scheduled_obs is not None):
-                    # So, we think there's a region that has had a long gap and can be observed
+                    # So, we think there's a region that has had a
+                    # long gap and can be observed
                     # call the standard reward function
                     self.reward = super(PlanAheadSurvey, self).calc_reward_function(conditions)
 
         return self.reward
 
     def generate_observations(self, conditions):
         observations = super(PlanAheadSurvey, self).generate_observations(conditions)
-        # We are providing observations, so clear the scheduled obs and reset the night so
-        # self.check_night will get called again in case there's another blob that should be done
-        # after this one completes
+        # We are providing observations, so clear the scheduled obs
+        # and reset the night so
+        # self.check_night will get called again in case there's
+        # another blob that should be done after this one completes
         self.scheduled_obs = None
         self.night_cad = conditions.night - 1
         return observations
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/pointings_survey.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/pointings_survey.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,41 +16,47 @@
     """Survey object for managing a set list of potential pointings
     without specified observing times. Does not follow the usual
     Survey class API by not using BasisFunction objects.
 
     Parameters
     ----------
     observations : `np.array`
-        An array of observations, from e.g. rubin_scheduler.scheduler.utils.empty_observation
+        An array of observations, from e.g.,
+        rubin_scheduler.scheduler.utils.empty_observation
         expect "RA", "dec", and "note" to be filled, other columns ignored.
     gap_min : `float`
-        The minimum gap to force between observations of the same spot (minutes)
+        The minimum gap to force between observations of the same
+        spot (minutes)
     alt_min : `float`
         Altitude limit of the telescope (degrees). Default 20.
     alt_max : `float`
         Altitude limit of the telescope (degrees). Default 85.
     ha_max, ha_min : `float` (4,-4)
-        hour angle limits (hours). Applied to all observations. Default 4,-4.
+        hour angle limits (hours). Applied to all observations.
+        Default 4,-4.
     weights : `dict`
         Dictionary with keys of method names and values of floats.
         Default of None uses {"visit_gap": 1.0, "balance_revisit": 1.0,
                               "m5diff": 1.0,
                               "wind_limit": 1.0, "slew_time": -1.0,
-                              "ha_limit": 0, "alt_limit": 0, "moon_limit": 0}
+                              "ha_limit": 0, "alt_limit": 0,
+                              "moon_limit": 0}
     wind_speed_maximum : `float`
-        The maximum wind (m/s), mask any targets that would take more wind than that.
-        Default 100 m/s.
+        The maximum wind (m/s), mask any targets that would take more
+        wind than that. Default 100 m/s.
     fiducial_FWHMEff : `float`
         A fiducial seeing value to use when computing dark sky depth.
         Default 0.7 arcsec.
     sun_alt_limit : `float`
-        Have survey as infeasible when sun altitude is above the limit. default -12 (degrees).
+        Have survey as infeasible when sun altitude is above the limit.
+        Default -12 (degrees).
     track_notes_ngoal : `dict`
-        If there are observations that should be tracked together (e.g., a sequence that
-        should be observed together). Dict with keys of str and values of int.
+        If there are observations that should be tracked together
+        (e.g., a sequence that should be observed together). Dict
+        with keys of str and values of int.
     """
 
     def __init__(
         self,
         observations,
         gap_min=25.0,
         moon_dist_limit=30.0,
@@ -140,15 +146,16 @@
 
         reward = self.calc_reward_function(conditions)
         if not np.isfinite(reward):
             result = False
         return result
 
     def calc_reward_function(self, conditions):
-        """Compute reward function using methods set by `weights` dict on init."""
+        """Compute reward function using methods set by `weights`
+        dict on init."""
         if self.last_computed_reward != conditions.mjd:
             self.alt, self.az = _approx_ra_dec2_alt_az(
                 self.observations["RA"],
                 self.observations["dec"],
                 conditions.site.latitude_rad,
                 conditions.site.longitude_rad,
                 conditions.mjd,
@@ -165,16 +172,17 @@
             for key in self.weights:
                 self.reward += self.weights[key] * getattr(self, key)(conditions)
 
             self.last_computed_reward = conditions.mjd
         return np.nanmax(self.reward)
 
     def generate_observations_rough(self, conditions):
-        """Calculate reward function and highest reward observation. This is usually
-        called by `generate_observations` which will take the result and then apply detailers to them.
+        """Calculate reward function and highest reward observation.
+        This is usually called by `generate_observations` which will
+        take the result and then apply detailers to them.
         """
         max_reward = self.calc_reward_function(conditions)
         # take the first one in the array if there's a tie
         # Could change logic to return multiple pointings
         winner = np.min(np.where(self.reward == max_reward)[0])
         return [self.observations[winner].copy().reshape(1)]
 
@@ -188,15 +196,16 @@
 
         # If we are tracking n observations of some type:
         for key in self.tracking_notes:
             if key in observation["note"]:
                 self.tracking_notes[key] += 1
 
     def add_observations_array(self, observations_array_in, observations_hpid_in):
-        """Like `add_observation`, but for a large array of completed observations."""
+        """Like `add_observation`, but for a large array of completed
+        observations."""
         for unote in np.unique(observations_array_in["note"]):
             matching = np.where(observations_array_in["note"] == unote)[0]
             indx = np.where(self.observations["note"] == unote)[0]
             self.n_obs[indx] += np.size(matching)
             self.last_observed[indx] = observations_array_in["mjd"][matching].max()
 
             for key in self.tracking_notes:
@@ -266,15 +275,16 @@
         result = hp.get_interp_val(
             conditions.slewtime,
             np.degrees(self.observations["RA"]),
             np.degrees(self.observations["dec"]),
             lonlat=True,
         )
 
-        # Could do a filter check here and add a penalty for changing filters
+        # Could do a filter check here and add a penalty for changing
+        # filters
 
         return result
 
     def sequence_boost(self, conditions):
         """Boost the reward if a sequence is incomplete."""
         result = self.zeros.copy()
         for key in self.sequence_mapping:
@@ -318,15 +328,16 @@
     def _reward_to_scalars(self, reward):
         scalar_reward = np.nanmax(reward)
         n_unmasked = np.sum(np.isfinite(reward))
 
         return scalar_reward, n_unmasked
 
     def make_reward_df(self, conditions, accum=True):
-        """Create a pandas.DataFrame describing the reward from the survey."""
+        """Create a pandas.DataFrame describing the reward from the
+        survey."""
 
         feasibility = []
         max_rewards = []
         n_possibles = []
         accum_rewards = []
         accum_areas = []
         bf_label = []
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/scripted_surveys.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/scripted_surveys.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,39 +3,42 @@
 import logging
 
 import healpy as hp
 import numpy as np
 
 from rubin_scheduler.scheduler.surveys import BaseSurvey
 from rubin_scheduler.scheduler.utils import empty_observation, set_default_nside
-from rubin_scheduler.utils import _approx_ra_dec2_alt_az
+from rubin_scheduler.utils import _angular_separation, _approx_ra_dec2_alt_az
 
 log = logging.getLogger(__name__)
 
 
 class ScriptedSurvey(BaseSurvey):
     """
     Take a set of scheduled observations and serve them up.
 
     Parameters
     ----------
-    basis_functions : list of rubin_scheduler.scheduler.BasisFunction objects
-        Basis functions to use. These are only used for masking regions of the sky and
-        computing survey feasibility. They do not contribute to the logic of how
-        observations are selected.
+    basis_functions : list of rubin_scheduler.scheduler.BasisFunction
+        Basis functions to use. These are only used for masking regions
+        of the sky and computing survey feasibility. They do not
+        contribute to the logic of how observations are selected.
     id_start : `int` (1)
-        The integer to start the "scripted id" field with. Bad things could happen
-        if you have multiple scripted survey objects with the same scripted IDs.
+        The integer to start the "scripted id" field with. Bad things
+        could happen if you have multiple scripted survey objects with
+        the same scripted IDs.
     return_n_limit : `int` (10)
-        The maximum number of observations to return. Set to high and your block
-        of scheduled observations can run into twilight time.
+        The maximum number of observations to return. Set to high and
+        your block of scheduled observations can run into twilight time.
     before_twi_check : `bool`
-        Check if the returned observations have enough time to complete before twilight starts. (default True)
+        Check if the returned observations have enough time to complete
+        before twilight starts. (default True)
     filter_change_time : `float`
-        The time needed to change filters. Default 120 seconds. Only used if before_twi_check is True.
+        The time needed to change filters. Default 120 seconds. Only
+        used if before_twi_check is True.
     """
 
     def __init__(
         self,
         basis_functions,
         basis_weights=None,
         reward=1e6,
@@ -95,15 +98,16 @@
             for bf in self.extra_basis_functions:
                 self.extra_basis_functions[bf].add_observations_array(observations_array, observations_hpid)
             for bf in self.basis_functions:
                 bf.add_observations_array(observations_array, observations_hpid)
             for detailer in self.detailers:
                 detailer.add_observations_array(observations_array, observations_hpid)
 
-            # If scripted_id, note, and filter match, then consider the observation completed.
+            # If scripted_id, note, and filter match, then consider
+            # the observation completed.
             completed = np.char.add(
                 observations_array["scripted_id"].astype(str),
                 observations_array["note"],
             )
             completed = np.char.add(completed, observations_array["filter"])
 
             wanted = np.char.add(self.obs_wanted["scripted_id"].astype(str), self.obs_wanted["note"])
@@ -137,15 +141,16 @@
                         & (self.obs_wanted["note"][indx] == observation["note"])
                         & (self.obs_wanted["filter"][indx] == observation["filter"])
                     ):
                         self.obs_wanted["observed"][indx] = True
                         self.scheduled_obs = self.obs_wanted["mjd"][~self.obs_wanted["observed"]]
 
     def calc_reward_function(self, conditions):
-        """If there is an observation ready to go, execute it, otherwise, -inf"""
+        """If there is an observation ready to go, execute it,
+        otherwise, -inf"""
         observation = self.generate_observations_rough(conditions)
         if (observation is None) | (np.size(observation) == 0):
             self.reward = -np.inf
         else:
             self.reward = self.reward_val
         return self.reward
 
@@ -165,36 +170,43 @@
             "flush_by_mjd",
             "scripted_id",
         ]:
             observation[key] = obs_row[key]
         return observation
 
     def _check_alts_ha(self, observation, conditions):
-        """Given scheduled observations, check which ones can be done in current conditions.
+        """Given scheduled observations, check which ones can be
+        done in current conditions.
 
         Parameters
         ----------
         observation : np.array
             An array of scheduled observations. Probably generated with
             rubin_scheduler.scheduler.utils.scheduled_observation
         """
+        # distance to the moon
+        d_to_moon = _angular_separation(
+            observation["RA"], observation["dec"], conditions.moon_ra, conditions.moon_dec
+        )
+
         # Just do a fast ra,dec to alt,az conversion.
         alt, az = _approx_ra_dec2_alt_az(
             observation["RA"],
             observation["dec"],
             conditions.site.latitude_rad,
             None,
             conditions.mjd,
             lmst=conditions.lmst,
         )
         HA = conditions.lmst - observation["RA"] * 12.0 / np.pi
         HA[np.where(HA > 24)] -= 24
         HA[np.where(HA < 0)] += 24
         in_range = np.where(
-            (alt < observation["alt_max"])
+            (d_to_moon > observation["moon_min_distance"])
+            & (alt < observation["alt_max"])
             & (alt > observation["alt_min"])
             & ((HA > observation["HA_max"]) | (HA < observation["HA_min"]))
             & (conditions.sun_alt < observation["sun_alt_max"])
         )[0]
 
         # Also check the alt,az limits given by the conditions object
         count = in_range * 0
@@ -213,15 +225,16 @@
 
         return in_range
 
     def _check_list(self, conditions):
         """Check to see if the current mjd is good"""
         observations = None
         if self.obs_wanted is not None:
-            # Scheduled observations that are in the right time window and have not been executed
+            # Scheduled observations that are in the right time
+            # window and have not been executed
             in_time_window = np.where(
                 (self.mjd_start < conditions.mjd)
                 & (self.obs_wanted["flush_by_mjd"] > conditions.mjd)
                 & (~self.obs_wanted["observed"])
             )[0]
 
             if np.size(in_time_window) > 0:
@@ -236,15 +249,16 @@
                 matches = []
 
             if np.size(matches) > 0:
                 # Do not return too many observations
                 if np.size(matches) > self.return_n_limit:
                     matches = matches[0 : self.return_n_limit]
                 observations = self.obs_wanted[matches]
-                # Need to check that none of these are masked by basis functions
+                # Need to check that none of these are masked by basis
+                # functions
                 reward = 0
                 for bf, weight in zip(self.basis_functions, self.basis_weights):
                     basis_value = bf(conditions)
                     reward += basis_value * weight
                 # If reward is an array, then it's a HEALpy map and we
                 # need to interpolate to the actual positions we want.
                 # now to interpolate to the reward positions
@@ -267,34 +281,37 @@
         self.scheduled_obs = None
 
     def set_script(self, obs_wanted):
         """
         Parameters
         ----------
         obs_wanted : np.array
-            The observations that should be executed. Needs to have columns with dtype names:
+            The observations that should be executed. Needs to have
+            columns with dtype names:
             Should be from lsst.sim.scheduler.utils.scheduled_observation
         mjds : np.array
-            The MJDs for the observaitons, should be same length as obs_list
+            The MJDs for the observaitons, should be same length as
+            obs_list
         mjd_tol : float (15.)
-            The tolerance to consider an observation as still good to observe (min)
+            The tolerance to consider an observation as still good to
+            observe (min)
         """
 
         self.obs_wanted = obs_wanted
 
         self.obs_wanted.sort(order=["mjd", "filter"])
         # Give each desired observation a unique "scripted ID". To be used for
         # matching and logging later.
         self.obs_wanted["scripted_id"] = np.arange(self.id_start, self.id_start + np.size(self.obs_wanted))
         # Update so if we set the script again the IDs will not be reused.
         self.id_start = np.max(self.obs_wanted["scripted_id"]) + 1
 
         self.mjd_start = self.obs_wanted["mjd"] - self.obs_wanted["mjd_tol"]
-        # Here is the atribute that core scheduler checks to broadcast scheduled observations
-        # in the conditions object.
+        # Here is the atribute that core scheduler checks to
+        # broadcast scheduled observations in the conditions object.
         self.scheduled_obs = self.obs_wanted["mjd"]
 
     def generate_observations_rough(self, conditions):
         # if we have already called for this mjd, no need to repeat.
         if self.last_mjd == conditions.mjd:
             return self.observations
 
@@ -302,15 +319,16 @@
         if observations is None:
             self.observations = []
             self.last_mjd = conditions.mjd
             return self.observations
 
         n_filter_changes = np.sum(observations[1:]["filter"] == observations[:-1]["filter"])
 
-        # If we want to ensure the observations can be completed before twilight starts
+        # If we want to ensure the observations can be completed
+        # before twilight starts
         if self.before_twi_check:
             # Note that if detailers are adding lots of exposures, this
             # calculation has the potential to not be right at all.
             # Also assumes slew time is negligable.
             exptime_needed = np.sum(observations["exptime"]) / 3600.0 / 24.0  # to days
             filter_change_needed = n_filter_changes * self.filter_change_time
             tot_time_needed = exptime_needed + filter_change_needed
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/surveys.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/surveys.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,48 +103,57 @@
     """Select observations in large, mostly contiguous, blobs.
 
     Parameters
     ----------
     filtername1 : `str`
         The filter to observe in.
     filtername2 : `str`
-        The filter to pair with the first observation. If set to None, no pair
-        will be observed.
+        The filter to pair with the first observation. If set to None,
+        no pair will be observed.
     slew_approx : `float`
-        The approximate slewtime between neerby fields (seconds). Used to calculate
-        how many observations can be taken in the desired time block.
+        The approximate slewtime between neerby fields (seconds). Used
+        to calculate how many observations can be taken in the
+        desired time block.
     nexp : `int`
         The number of exposures to take in a visit.
     exp_dict : `dict`
-        If set, should have keys of filtername and values of ints that are the nuber of exposures to take
-        per visit. For estimating block time, nexp is still used.
+        If set, should have keys of filtername and values of ints that
+        are the nuber of exposures to take per visit. For estimating
+        block time, nexp is still used.
     filter_change_approx : `float`
          The approximate time it takes to change filters (seconds).
     ideal_pair_time : `float`
-        The ideal time gap wanted between observations to the same pointing (minutes)
+        The ideal time gap wanted between observations to the same
+        pointing (minutes)
     min_pair_time : `float`
         The minimum acceptable pair time (minutes)
     flush_time : `float`
-        The time past the final expected exposure to flush the queue. Keeps observations
-        from lingering past when they should be executed. (minutes)
+        The time past the final expected exposure to flush the queue.
+        Keeps observations from lingering past when they should be
+        executed. (minutes)
     twilight_scale : `bool`
-        Scale the block size to fill up to twilight. Set to False if running in twilight
+        Scale the block size to fill up to twilight. Set to False if
+        running in twilight
     in_twilight : `bool`
         Scale the block size to stay within twilight time.
     check_scheduled : `bool`
-        Check if there are scheduled observations and scale blob size to match
+        Check if there are scheduled observations and scale blob size
+        to match
     min_area : `float`
-        If set, demand the reward function have an area of so many square degrees before executing
+        If set, demand the reward function have an area of so many
+        square degrees before executing
     grow_blob : `bool`
-        If True, try to grow the blob from the global maximum. Otherwise, just use a simple sort.
-        Simple sort will not constrain the blob to be contiguous.
+        If True, try to grow the blob from the global maximum. Otherwise,
+        just use a simple sort.  Simple sort will not constrain the
+        blob to be contiguous.
     max_radius_peak : `float`
-        The maximum radius to demand things be within the maximum of the reward function. (degrees)
-        Note that traveling salesman solver can have rare failures if this is set too large
-        (probably issue with projection effects or something).
+        The maximum radius to demand things be within the maximum of
+        the reward function. (degrees) Note that traveling salesman
+        solver can have rare failures if this is set too large (probably
+        issue with projection effects or something).
     """
 
     def __init__(
         self,
         basis_functions,
         basis_weights,
         filtername1="r",
@@ -208,18 +217,20 @@
         self.max_radius_peak = np.radians(max_radius_peak)
 
         if self.twilight_scale & self.in_twilight:
             warnings.warn("Both twilight_scale and in_twilight are set to True. That is probably wrong.")
 
         self.min_area = min_area
         self.check_scheduled = check_scheduled
-        # If we are taking pairs in same filter, no need to add filter change time.
+        # If we are taking pairs in same filter, no need to add filter
+        # change time.
         if filtername1 == filtername2:
             filter_change_approx = 0
-        # Compute the minimum time needed to observe a blob (or observe, then repeat.)
+        # Compute the minimum time needed to observe a blob (or observe,
+        # then repeat.)
         if filtername2 is not None:
             self.time_needed = (
                 (min_pair_time * 60.0 * 2.0 + exptime + read_approx + filter_change_approx) / 24.0 / 3600.0
             )  # Days
         else:
             self.time_needed = (min_pair_time * 60.0 + exptime + read_approx) / 24.0 / 3600.0  # Days
         self.filter_set = set(filtername1)
@@ -227,15 +238,15 @@
             self.filter2_set = self.filter_set
         else:
             self.filter2_set = set(filtername2)
 
         self.ra, self.dec = _hpid2_ra_dec(self.nside, self.hpids)
 
         self.survey_note = survey_note
-        self.counter = 1  # start at 1, because 0 is default in empty observation
+        self.counter = 1  # start at 1, because 0 is default in empty obs
         self.min_pair_time = min_pair_time
         self.ideal_pair_time = ideal_pair_time
 
         self.pixarea = hp.nside2pixarea(self.nside, degrees=True)
 
         # If we are only using one filter, this could be useful
         if (self.filtername2 is None) | (self.filtername1 == self.filtername2):
@@ -253,26 +264,31 @@
         Check if the survey is feasable in the current conditions.
         """
         for bf in self.basis_functions:
             result = bf.check_feasibility(conditions)
             if not result:
                 return result
 
-        # If we need to check that the reward function has enough area available
+        # If we need to check that the reward function has enough
+        # area available
         if self.min_area is not None:
             reward = 0
             for bf, weight in zip(self.basis_functions, self.basis_weights):
                 basis_value = bf(conditions)
                 reward += basis_value * weight
-            max_reward_indx = np.min(np.where(reward == np.nanmax(reward)))
-            distances = _angular_separation(
-                self.ra, self.dec, self.ra[max_reward_indx], self.dec[max_reward_indx]
-            )
-            valid_pix = np.where((np.isnan(reward) == False) & (distances < self.max_radius_peak))[0]
-            if np.size(valid_pix) * self.pixarea < self.min_area:
+            # Are there any valid reward pixels remaining
+            if np.sum(np.isfinite(reward)) > 0:
+                max_reward_indx = np.min(np.where(reward == np.nanmax(reward)))
+                distances = _angular_separation(
+                    self.ra, self.dec, self.ra[max_reward_indx], self.dec[max_reward_indx]
+                )
+                valid_pix = np.where((np.isnan(reward) == False) & (distances < self.max_radius_peak))[0]
+                if np.size(valid_pix) * self.pixarea < self.min_area:
+                    result = False
+            else:
                 result = False
         return result
 
     def _set_block_size(self, conditions):
         """
         Update the block size if it's getting near a break point.
         """
@@ -290,15 +306,16 @@
             if len(conditions.scheduled_observations) > 0:
                 available_time = np.min(conditions.scheduled_observations) - conditions.mjd
                 available_time *= 24.0 * 60.0  # to minutes
                 n_blocks = available_time / self.ideal_pair_time
                 if n_blocks < n_ideal_blocks:
                     n_ideal_blocks = n_blocks
 
-        # If we are trying to complete before twilight ends or the night ends
+        # If we are trying to complete before twilight ends or
+        # the night ends
         if self.in_twilight:
             at1 = conditions.sun_n12_rising - conditions.mjd
             at2 = conditions.sun_n18_setting - conditions.mjd
             times = np.array([at1, at2])
             times = times[np.where(times > 0)]
             available_time = np.min(times) if len(times) > 0 else 0.0
             available_time *= 24.0 * 60.0  # to minutes
@@ -311,17 +328,19 @@
                 np.floor(
                     self.ideal_pair_time
                     * 60.0
                     / (self.slew_approx + self.exptime + self.read_approx * (self.nexp - 1))
                 )
             )
         else:
-            # Now we can stretch or contract the block size to allocate the
+            # Now we can stretch or contract the block size to
+            # allocate the
             # remainder time until twilight starts
-            # We can take the remaining time and try to do 1,2, or 3 blocks.
+            # We can take the remaining time and try to do 1,2,
+            # or 3 blocks.
             possible_times = available_time / np.arange(1, 4)
             diff = np.abs(self.ideal_pair_time - possible_times)
             best_block_time = np.max(possible_times[np.where(diff == np.min(diff))])
             self.nvisit_block = int(
                 np.floor(
                     best_block_time
                     * 60.0
@@ -374,17 +393,19 @@
     def simple_order_sort(self):
         """Fall back if we can't link contiguous blobs in the reward map"""
 
         # Assuming reward has already been calcualted
 
         potential_hp = np.where(np.isfinite(self.reward))[0]
 
-        # Note, using nanmax, so masked pixels might be included in the pointing.
-        # I guess I should document that it's not "NaN pixels can't be observed", but
-        # "non-NaN pixles CAN be observed", which probably is not intuitive.
+        # Note, using nanmax, so masked pixels might be included in
+        # the pointing. I guess I should document that it's not
+        # "NaN pixels can't be observed", but
+        # "non-NaN pixles CAN be observed", which probably is
+        # not intuitive.
         ufields, reward_by_field = int_binned_stat(
             self.hp2fields[potential_hp], self.reward[potential_hp], statistic=np.nanmax
         )
         # chop off any nans
         not_nans = np.where(np.isfinite(reward_by_field))
         ufields = ufields[not_nans]
         reward_by_field = reward_by_field[not_nans]
@@ -430,29 +451,31 @@
         else:
             self.simple_order_sort()
 
         if len(self.best_fields) == 0:
             # everything was nans, or self.nvisit_block was zero
             return []
 
-        # Let's find the alt, az coords of the points (right now, hopefully doesn't change much in time block)
-        # Not sure why need to convert to alt,az before running TSP, but it
-        # does seem to be better.
+        # Let's find the alt, az coords of the points (right now,
+        # hopefully doesn't change much in time block)
+        # Not sure why need to convert to alt,az before running TSP,
+        # but it does seem to be better.
         pointing_alt, pointing_az = _approx_ra_dec2_alt_az(
             self.fields["RA"][self.best_fields],
             self.fields["dec"][self.best_fields],
             conditions.site.latitude_rad,
             conditions.site.longitude_rad,
             conditions.mjd,
             lmst=conditions.lmst,
         )
 
         better_order = order_observations(pointing_az, pointing_alt)
 
-        # XXX-TODO: Could try to roll better_order to start at the nearest/fastest slew from current position.
+        # XXX-TODO: Could try to roll better_order to start at
+        # the nearest/fastest slew from current position.
         observations = []
         counter2 = 0
         approx_end_time = np.size(better_order) * (
             self.slew_approx + self.exptime + self.read_approx * (self.nexp - 1)
         )
         flush_time = conditions.mjd + approx_end_time / 3600.0 / 24.0 + self.flush_time
         for i, indx in enumerate(better_order):
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/surveys/too_surveys.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/surveys/too_surveys.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 import numpy as np
 
 from rubin_scheduler.scheduler.surveys import BaseSurvey, BlobSurvey
 
 
 class TooMaster(BaseSurvey):
     """
-    A target of opportunity class. Every time a new ToO comes in, it will spawn a new sub-survey.
+    A target of opportunity class. Every time a new ToO comes in, it
+    will spawn a new sub-survey.
 
     Parameters
     ----------
-    example__to_o_survey : rubin_scheduler.scheduler.surveys.ToO_survey object
-        A survey object that will be coppied and have a new target map set
-        for each incoming ToO.
+    example__to_o_survey : rubin_scheduler.scheduler.surveys.ToO_survey
+        A survey object that will be coppied and have a new target
+        map set for each incoming ToO.
     """
 
     def __init__(self, example__to_o_survey):
         self.example__to_o_survey = example__to_o_survey
         self.surveys = []
         self.highest_reward = -np.inf
         self.scheduled_obs = None
@@ -75,18 +76,19 @@
     def generate_observations(self, conditions):
         if self.reward > -np.inf:
             result = self.surveys[self.highest_reward].generate_observations(conditions)
             return result
 
 
 class TooSurvey(BlobSurvey):
-    """Survey class to catch incoming target of opportunity anouncements and try to observe them.
+    """Survey class to catch incoming target of opportunity
+    anouncements and try to observe them.
 
-    The idea is that we can dynamically update the target footprint basis function,
-    and add new features as more ToOs come in.
+    The idea is that we can dynamically update the target
+    footprint basis function, and add new features as more ToOs come in.
 
     Parameters
     ----------
     too_id : int (None)
         A unique integer ID for the ToO getting observed
     """
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/comcam_tessellate.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/comcam_tessellate.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import numpy as np
 
 
 def comcam_tessellate(side_length=0.7, overlap=0.11):
     """Tesselate the sphere with a square footprint
 
-    XXX--TODO:  This really sucks at the poles, should add some different pole cap behavior.
+    XXX--TODO:  This really sucks at the poles, should add some
+    different pole cap behavior.
 
     Parameters
     ----------
     side_length : float (0.7)
         The length of a side of the square (degrees)
     overlap : float (0.11)
         How much overlap to have in pointings
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/dithering.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/dithering.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,20 +93,22 @@
     ra_p, dec_p = wrap_ra_dec(ra_p, dec_p)
 
     return ra_p, dec_p
 
 
 class Pointings2hp:
     """
-    Convert a list of telescope pointings and convert them to a pointing map
+    Convert a list of telescope pointings and convert them to a
+    pointing map
     """
 
     def __init__(self, nside, radius=1.75):
         """"""
-        # hmm, not sure what the leafsize should be? Kernel can crash if too low.
+        # hmm, not sure what the leafsize should be? Kernel can crash
+        # if too low.
         self.tree = hp_kd_tree(nside=nside, leafsize=300)
         self.nside = nside
         self.rad = _xyz_angular_radius(radius)
         self.bins = np.arange(hp.nside2npix(nside) + 1) - 0.5
 
     def __call__(self, ra, dec, stack=True):
         """
@@ -118,15 +120,16 @@
             RA in radians
         dec : array_like
             Dec in radians
 
         Returns
         -------
         result : healpy map
-            The number of times each healpxel is observed by the given pointings
+            The number of times each healpxel is observed by the
+            given pointings
         """
         xs, ys, zs = _xyz_from_ra_dec(ra, dec)
         coords = np.array((xs, ys, zs)).T
         indx = self.tree.query_ball_point(coords, self.rad)
         # Convert array of lists to single array
         if stack:
             indx = np.hstack(indx)
@@ -135,22 +138,24 @@
             result = indx
 
         return result
 
 
 class HpmapCross:
     """
-    Find the cross-correlation of a healpix map and a bunch of rotated pointings
+    Find the cross-correlation of a healpix map and a bunch of
+    rotated pointings
     """
 
     # XXX--just a very random radius search
     def __init__(self, nside=default_nside, radius=1.75, radius_search=1.75):
         """"""
         self.nside = nside
-        # XXX -- should I shrink the radius slightly to get rid of overlap? That would be clever!
+        # XXX -- should I shrink the radius slightly to get rid
+        # of overlap? That would be clever!
         self.p2hp_search = Pointings2hp(nside=nside, radius=radius_search)
         self.p2hp = Pointings2hp(nside=nside, radius=radius)
         # Load up a list of pointings, chop them down to a small block
         ra, dec = _read_fields()
         fields = np.empty(ra.size, dtype=list(zip(["RA", "dec"], [float, float])))
         fields["RA"] = ra
         fields["dec"] = dec
@@ -177,21 +182,22 @@
         x[0], ra_rot : float
             Amount to rotate the fields in RA (radians)
         x[1], dec_rot : float
             Amount to rotate the fields in Dec (radians)
         x[2], im_rot : float
             Initial rotation to apply to fields (radians)
         return_pointings_map : bool (False)
-            If set, return the overlapping fields and the resulting observing helpix map
+            If set, return the overlapping fields and the resulting
+            observing helpix map
 
         Returns
         -------
         cross_corr : float
-            If return_pointings_map is False, return the sum of the pointing map multipled
-            with the
+            If return_pointings_map is False, return the sum of the
+            pointing map multipled with the
         """
         # XXX-check the nside
 
         # Unpack the x variable
         ra_rot = x[0]
         dec_rot = x[1]
         im_rot = x[2]
@@ -235,15 +241,16 @@
         ra_delta = np.radians(ra_delta)
         dec_delta = np.radians(dec_delta)
         rot_delta = np.radians(rot_delta)
 
         # rots = np.arange(-np.pi/2., np.pi/2.+rot_delta, rot_delta)
         rots = [np.radians(0.0)]
         # Make sure the initial simplex is large enough
-        # XXX--might need to update scipy latest version to actually use this.
+        # XXX--might need to update scipy latest version to
+        # actually use this.
         deltas = np.array(
             [
                 [ra_delta, 0, 0],
                 [0, dec_delta, rot_delta],
                 [-ra_delta, 0, -rot_delta],
                 [ra_delta, -dec_delta, 2.0 * rot_delta],
             ]
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/footprints.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/footprints.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,16 +35,17 @@
     sun_ra_start=3.27717639,
     nslice=2,
     scale=0.8,
     nside=32,
     wfd_indx=None,
     order_roll=0,
     n_cycles=None,
-    n_constant_start=3,
+    n_constant_start=None,
     n_constant_end=6,
+    uniform=False,
 ):
     """
     Generate rolling footprints
 
     Parameters
     ----------
     fp_hp : dict-like
@@ -54,70 +55,109 @@
     sun_ra_start : `float`
         The RA of the sun at the start of the survey
     nslice : `int`
         How much to slice the sky up. Can be 2, 3, 4, or 6.
     scale : `float`
         The strength of the rolling, value of 1 is full power rolling.
         Zero is no rolling.
+    nside : `int`
+        HEALpix nisde to use to represent the footprints. Default is 32.
     wfd_indx : array of ints
         The indices of the HEALpix map that are to be included in the rolling.
     order_roll : `int`
         Change the order of when bands roll. Default 0.
     n_cycles : `int`
         Number of complete rolling cycles to attempt. If None, defaults to 3
         full cycles for nslice=2, 2 cycles for nslice=3 or 4, and 1 cycle for
         nslice=6.
     n_constant_start : `int`
-        The number of constant non-rolling seasons to start with.
-        Anything less than 3 results in rolling starting before the
-        entire sky has had a constant year.
+        The number of constant non-rolling seasons to start with. Anything
+        less than 2 will start rolling too early near Y1. If uniform rolling
+        is turned off, the lowest value should be 3. Defaults to None which
+        selects the correct lowest value based on the value of uniform.
     n_constant_end : `int`
         The number of constant seasons to end the survey with. Defaults to 6.
+    uniform : `bool`
+        If True, the rolling sequence is adjusted in half of the sky to
+        generate uniform surveys during years between rolling cycles. For
+        nslice=2 and three cycles, years 1, 4, 7, and 10 will be uniform.
+        For nslice=3 and two cycles, years 1, 5, 9, and 10 will be uniform.
+        Default is False.
 
     Returns
     -------
     Footprints object
     """
 
     nc_default = {2: 3, 3: 2, 4: 2, 6: 1}
     if n_cycles is None:
         n_cycles = nc_default[nslice]
 
+    if n_constant_start is None:
+        if uniform:
+            n_constant_start = 2
+        else:
+            n_constant_start = 3
+
     hp_footprints = fp_hp
 
     down = 1.0 - scale
     up = nslice - down * (nslice - 1)
 
     start = [1.0] * n_constant_start
     # After n_cycles, just go to no-rolling for 6 years.
     end = [1.0] * n_constant_end
 
     rolling = [up] + [down] * (nslice - 1)
-    rolling = rolling * n_cycles
-
     rolling = np.roll(rolling, order_roll).tolist()
 
-    all_slopes = [start + np.roll(rolling, i).tolist() + end for i in range(nslice)]
+    all_slopes = []
+    if uniform:
+        for i in range(nslice):
+            _roll = np.roll(rolling, i).tolist() + [1]
+            all_slopes.append(start + _roll * n_cycles + end)
+        for i in range(nslice):
+            _roll = np.roll(rolling, i).tolist() + [1]
+            _roll = [_roll[-1]] + _roll[1:-1] + [_roll[0]]
+            all_slopes.append(start + _roll * n_cycles + end)
+    else:
+        rolling = rolling * n_cycles
+        all_slopes = [start + np.roll(rolling, i).tolist() + end for i in range(nslice)]
 
     fp_non_wfd = Footprint(mjd_start, sun_ra_start=sun_ra_start, nside=nside)
     rolling_footprints = []
-    for i in range(nslice):
+    for i in range(len(all_slopes)):
         step_func = StepSlopes(rise=all_slopes[i])
         rolling_footprints.append(
             Footprint(mjd_start, sun_ra_start=sun_ra_start, step_func=step_func, nside=nside)
         )
 
     wfd = hp_footprints["r"] * 0
     if wfd_indx is None:
         wfd_indx = np.where(hp_footprints["r"] == 1)[0]
 
     wfd[wfd_indx] = 1
     non_wfd_indx = np.where(wfd == 0)[0]
 
-    split_wfd_indices = slice_quad_galactic_cut(hp_footprints, nslice=nslice, wfd_indx=wfd_indx)
+    if uniform:
+        split_wfd_indices = slice_quad_galactic_cut(
+            hp_footprints,
+            nslice=nslice,
+            wfd_indx=wfd_indx,
+            ra_range=(sun_ra_start + 1.5 * np.pi, sun_ra_start + np.pi / 2),
+        )
+
+        split_wfd_indices_delayed = slice_quad_galactic_cut(
+            hp_footprints,
+            nslice=nslice,
+            wfd_indx=wfd_indx,
+            ra_range=(sun_ra_start + np.pi / 2, sun_ra_start + 1.5 * np.pi),
+        )
+    else:
+        split_wfd_indices = slice_quad_galactic_cut(hp_footprints, nslice=nslice, wfd_indx=wfd_indx)
 
     for key in hp_footprints:
         temp = hp_footprints[key] + 0
         temp[wfd_indx] = 0
         fp_non_wfd.set_footprint(key, temp)
 
         for i in range(nslice):
@@ -129,14 +169,28 @@
             indx = split_wfd_indices[i]
             # invert the indices
             ze = temp * 0
             ze[indx] = 1
             temp = temp * ze
             rolling_footprints[i].set_footprint(key, temp)
 
+        if uniform:
+            for _i in range(nslice, nslice * 2):
+                # make a copy of the current filter
+                temp = hp_footprints[key] + 0
+                # Set the non-rolling area to zero
+                temp[non_wfd_indx] = 0
+
+                indx = split_wfd_indices_delayed[_i - nslice]
+                # invert the indices
+                ze = temp * 0
+                ze[indx] = 1
+                temp = temp * ze
+                rolling_footprints[_i].set_footprint(key, temp)
+
     result = Footprints([fp_non_wfd] + rolling_footprints)
     return result
 
 
 def slice_wfd_indx(target_map, nslice=2, wfd_indx=None):
     """
     simple map split
@@ -150,27 +204,39 @@
     split_wfd_indices = np.floor(np.max(wfd_accum) / nslice * (np.arange(nslice) + 1)).astype(int)
     split_wfd_indices = split_wfd_indices.tolist()
     split_wfd_indices = [0] + split_wfd_indices
 
     return split_wfd_indices
 
 
-def slice_quad_galactic_cut(target_map, nslice=2, wfd_indx=None):
+def _is_in_ra_range(ra, low, high):
+    _low = low % (2.0 * np.pi)
+    _high = high % (2.0 * np.pi)
+    if _low <= _high:
+        return (ra >= _low) & (ra <= _high)
+    else:
+        return (ra >= _low) | (ra <= _high)
+
+
+def slice_quad_galactic_cut(target_map, nslice=2, wfd_indx=None, ra_range=None):
     """
     Helper function for generating rolling footprints
 
     Parameters
     ----------
     target_map : dict of HEALpix maps
         The final desired footprint as HEALpix maps. Keys are filter names
     nslice : `int`
         The number of slices to make, can be 2 or 3.
     wfd_indx : array of ints
         The indices of target_map that should be used for rolling.
         If None, assumes the rolling area should be where target_map['r'] == 1.
+    ra_range : tuple of floats, optional
+        If not None, then the indices are restricted to the given RA range
+        in radians.
     """
 
     ra, dec = ra_dec_hp_map(nside=hp.npix2nside(target_map["r"].size))
 
     coord = SkyCoord(ra=ra * u.rad, dec=dec * u.rad)
     _, gal_lat = coord.galactic.l.deg, coord.galactic.b.deg
 
@@ -184,14 +250,19 @@
     for j in np.arange(nslice):
         indx_temp = []
         for i in np.arange(j + 1, nslice * 2 + 1, nslice):
             indx_temp += indx_north[splits_north[i - 1] : splits_north[i]].tolist()
             indx_temp += indx_south[splits_south[i - 1] : splits_south[i]].tolist()
         slice_indx.append(indx_temp)
 
+    if ra_range is not None:
+        ra_indx = np.where(_is_in_ra_range(ra, *ra_range))[0]
+        for j in range(nslice):
+            slice_indx[j] = np.intersect1d(ra_indx, slice_indx[j])
+
     return slice_indx
 
 
 def slice_wfd_area_quad(target_map, nslice=2, wfd_indx=None):
     """
     Divide a healpix map in an intelligent way
 
@@ -234,44 +305,27 @@
         self.t_start = t_start
 
     def __call__(self, mjd_in, phase):
         pass
 
 
 class StepLine(BasePixelEvolution):
-    """
-    Parameters
-    ----------
-    period : `float`
-        The period to use
-    rise : `float`
-        How much the curve should rise every period
-    """
 
     def __call__(self, mjd_in, phase):
         t = mjd_in + phase - self.t_start
         n_periods = np.floor(t / (self.period))
         result = n_periods * self.rise
         tphased = t % self.period
         step_area = np.where(tphased > self.period / 2.0)[0]
         result[step_area] += (tphased[step_area] - self.period / 2) * self.rise / (0.5 * self.period)
         result[np.where(t < 0)] = 0
         return result
 
 
 class StepSlopes(BasePixelEvolution):
-    """
-    Parameters
-    ----------
-    period : `float`
-        The period to use - typically should be a year.
-    rise : np.array-like
-        How much the curve should rise each period.
-    """
-
     def __call__(self, mjd_in, phase):
         steps = np.array(self.rise)
         t = mjd_in + phase - self.t_start
         season = np.floor(t / (self.period))
         season = season.astype(int)
         plateus = np.cumsum(steps) - steps[0]
         result = plateus[season]
@@ -298,30 +352,34 @@
     """
 
     def __init__(
         self,
         mjd_start,
         sun_ra_start=0,
         nside=32,
-        filters={"u": 0, "g": 1, "r": 2, "i": 3, "z": 4, "y": 5},
+        filters=None,
         period=365.25,
         step_func=None,
     ):
+        if filters is None:
+            filters = {"u": 0, "g": 1, "r": 2, "i": 3, "z": 4, "y": 5}
         self.period = period
         self.nside = nside
         if step_func is None:
             step_func = StepLine()
         self.step_func = step_func
         self.mjd_start = mjd_start
         self.sun_ra_start = sun_ra_start
         self.npix = hp.nside2npix(nside)
         self.filters = filters
         self.ra, self.dec = _hpid2_ra_dec(self.nside, np.arange(self.npix))
         # Set the phase of each healpixel.
         # If RA to sun is zero, we are at phase np.pi/2.
+        # This is similar to the season calculation, except
+        # that phase and season are offset by 90 degrees.
         self.phase = (-self.ra + self.sun_ra_start + np.pi / 2) % (2.0 * np.pi)
         self.phase = self.phase * (self.period / 2.0 / np.pi)
         # Empty footprints to start
         self.out_dtype = list(zip(filters, [float] * len(filters)))
         self.footprints = np.zeros((len(filters), self.npix), dtype=float)
         self.estimate = np.zeros((len(filters), self.npix), dtype=float)
         self.current_footprints = np.zeros((len(filters), self.npix), dtype=float)
@@ -383,22 +441,28 @@
             convert to the number of observations desired.
         """
         self._update_mjd(mjd, norm=norm)
         return self.arr2struc(self.current_footprints)
 
 
 class ConstantFootprint(Footprint):
-    def __init__(self, nside=32, filters={"u": 0, "g": 1, "r": 2, "i": 3, "z": 4, "y": 5}):
+    def __init__(self, nside=32, filters=None):
+        if filters is None:
+            filters = {"u": 0, "g": 1, "r": 2, "i": 3, "z": 4, "y": 5}
         self.nside = nside
         self.filters = filters
         self.npix = hp.nside2npix(nside)
         self.footprints = np.zeros((len(filters), self.npix), dtype=float)
         self.out_dtype = list(zip(filters, [float] * len(filters)))
         self.to_return = self.arr2struc(self.footprints)
 
+    def set_footprint(self, filtername, values):
+        self.footprints[self.filters[filtername], :] = values
+        self.to_return = self.arr2struc(self.footprints)
+
     def __call__(self, mjd, array=False):
         return self.to_return
 
 
 class Footprints(Footprint):
     """An object to combine multiple Footprint objects."""
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/sky_area.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/sky_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 __all__ = (
+    "get_current_footprint",
     "generate_all_sky",
     "filter_count_ratios",
     "SkyAreaGenerator",
     "SkyAreaGeneratorGalplane",
     "EuclidOverlapFootprint",
 )
 
@@ -20,14 +21,36 @@
 from rubin_scheduler import data as rs_data
 from rubin_scheduler.utils import Site, _angular_separation, angular_separation
 
 from .footprints import ra_dec_hp_map
 from .utils import IntRounded, set_default_nside
 
 
+def get_current_footprint(nside):
+    """Convenience method to return the current footprint.
+
+    This is primarily a way to help rubin-sim users keep up to date
+    on footprint changes (as we have been moving to new subclasses).
+
+    Parameters
+    ----------
+    nside : `int`
+        The nside for the footprint map.
+
+    Returns
+    -------
+    footprint_arrays, label_array : `np.array`, (N,), `np.array`, (N,)
+        HEALPix target survey maps for ugrizy,
+        and array of string labels for each healpix to indicate the "region".
+    """
+    sky = EuclidOverlapFootprint(nside=nside)
+    footprints, labels = sky.return_maps()
+    return footprints, labels
+
+
 def generate_all_sky(nside=None, elevation_limit=20, mask=hp.UNSEEN):
     """Set up a healpix map over the entire sky.
     Calculate RA & Dec, Galactic l & b, Ecliptic l & b, for all healpixels.
     Calculate max altitude, to define areas which LSST cannot reach.
 
     This is intended to be a useful tool to use to set up target maps,
     beyond the standard maps provided in the various SkyArea generator maps.
@@ -239,23 +262,25 @@
         self.low_dust = np.where((self.dustmap < dust_limit), 1, 0)
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=UserWarning)
             self.low_dust = hp.smoothing(self.low_dust, fwhm=np.radians(smoothing_beam))
         self.low_dust = np.where(self.low_dust > smoothing_cutoff, 1, 0)
 
     def read_dustmap(self, dustmap_file=None):
-        """Read the dustmap from rubin_scheduler, in the appropriate resolution."""
+        """Read the dustmap from rubin_scheduler, in the
+        appropriate resolution."""
         # Dustmap from rubin_sim_data
         if dustmap_file is None:
             datadir = rs_data.get_data_dir()
             if datadir is None:
                 raise Exception('Cannot find datadir, please set "RUBIN_SIM_DATA_DIR"')
             datadir = os.path.join(datadir, "scheduler", "dust_maps")
             filename = os.path.join(datadir, "dust_nside_%i.npz" % self.nside)
-        self.dustmap = np.load(filename)["ebvMap"]
+        with np.load(filename) as data:
+            self.dustmap = data["ebvMap"]
 
     def _set_circular_region(self, ra_center, dec_center, radius):
         """Define a circular region centered on ra_center, dec_center."""
         # find the healpixels that cover a circle of radius
         # "radius" around ra/dec center (deg).
         result = np.zeros(len(self.ra))
         distance = _angular_separation(
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/tsp.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/tsp.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 
 import numpy as np
 import scipy.spatial as spatial
 
 from .utils import IntRounded, gnomonic_project_toxy, mean_azimuth
 
 # Solve Traveling Salesperson using convex hulls.
-# re-write of https://github.com/jameskrysiak/ConvexSalesman/blob/master/convex_salesman.py
-# This like a good explination too https://www.youtube.com/watch?v=syRSy1MFuho
+# re-write of https://github.com/jameskrysiak/ConvexSalesman/
+# blob/master/convex_salesman.py
+# This like a good explination too
+# https://www.youtube.com/watch?v=syRSy1MFuho
 
 
-def order_observations(lon, lat, scale=1e6, optimize=False):
+def order_observations(lon, lat, optimize=False):
     """Use TSP solver to put observations in an order that minimizes
     angular distance traveled
 
     Parameters
     ----------
     lon : `float`
         A longitude-like (RA, azimuth) angle (radians).
@@ -37,24 +39,24 @@
     optimize : `bool`
         If the TSP should run extra optimization steps, default False
     """
 
     # Let's find a good spot to project the points to a plane
     mid_dec = (np.max(lat) - np.min(lat)) / 2.0 + np.min(lat)
     mid_ra = mean_azimuth(lon)
-    # Project the coordinates to a plane. Could consider scaling things to represent
-    # time between points rather than angular distance.
+    # Project the coordinates to a plane. Could consider scaling
+    # things to represent time between points rather than angular
+    # distance.
     pointing_x, pointing_y = gnomonic_project_toxy(lon, lat, mid_ra, mid_dec)
-    # Round off positions so that we ensure identical cross-platform performance
 
-    pointing_x = np.round(pointing_x * scale).astype(int)
-    pointing_y = np.round(pointing_y * scale).astype(int)
-    # Now I have a bunch of x,y pointings. Drop into TSP solver to get an effiencent route
+    # Now I have a bunch of x,y pointings. Drop into TSP solver
+    # to get an effiencent route
     towns = np.vstack((pointing_x, pointing_y)).T
-    # Leaving optimize=False for speed. The optimization step doesn't usually improve much.
+    # Leaving optimize=False for speed. The optimization step doesn't
+    # usually improve much.
     better_order = tsp_convex(towns, optimize=optimize)
     return better_order
 
 
 def generate_dist_matrix(towns):
     """Generate the matrix for the distance between town i and j
 
@@ -143,16 +145,16 @@
     collapsed_indices = deque(indices_lists[0])
     for ind_list in indices_lists[1:]:
         # insert each point indvidually
         for indx in ind_list:
             possible_results = []
             possible_lengths = []
             dindex = deque([indx])
-            # In theory, I think this could loop over fewer points. Only need to check
-            # points that can "see" the inner points?
+            # In theory, I think this could loop over fewer points.
+            # Only need to check points that can "see" the inner points?
             for i in range(len(collapsed_indices)):
                 collapsed_indices.rotate(1)
                 possible_results.append(collapsed_indices + dindex)
                 possible_lengths.append(route_length(possible_results[-1], dist_matrix))
             best = np.min(np.where(possible_lengths == np.nanmin(possible_lengths)))
             collapsed_indices = possible_results[best]
     return list(collapsed_indices)
@@ -182,15 +184,16 @@
     # The combinations of three places that we can split each route.
     combinations = list(itertools.combinations(range(len(route)), 3))
 
     min_route = route
     min_length = route_length(min_route, dist_matrix)
 
     for cuts in combinations:
-        # The three chunks that the route is broken into based on the cuts.
+        # The three chunks that the route is broken into based
+        # on the cuts.
         c1 = route[cuts[0] : cuts[1]]
         c2 = route[cuts[1] : cuts[2]]
         c3 = route[cuts[2] :] + route[: cuts[0]]
 
         # Reversed chunks 2 and 3.
         rc2 = c2[::-1]
         rc3 = c3[::-1]
@@ -244,15 +247,15 @@
 
     if optimize:
         distance = route_length(route, dist_matrix)
         iter_count = 0
         optimized = False
         while not optimized:
             new_route, new_distance = three_opt(route, dist_matrix)
-            if new_distance < distance:
+            if IntRounded(new_distance) < IntRounded(distance):
                 route = new_route
                 distance = new_distance
                 iter_count += 1
             else:
                 optimized = True
             if iter_count == niter:
                 return route
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/scheduler/utils/utils.py` & `rubin_scheduler-1.2.0/rubin_scheduler/scheduler/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 
 import rubin_scheduler.version as rsVersion
 from rubin_scheduler.utils import _build_tree, _hpid2_ra_dec, _xyz_from_ra_dec, xyz_angular_radius
 
 
 def smallest_signed_angle(a1, a2):
     """
-    via https://stackoverflow.com/questions/1878907/the-smallest-difference-between-2-angles
+    via https://stackoverflow.com/questions/1878907/
+    the-smallest-difference-between-2-angles
     """
     two_pi = 2.0 * np.pi
     x = a1 % two_pi
     y = a2 % two_pi
     a = (x - y) % two_pi
     b = (y - x) % two_pi
     result = b + 0
@@ -173,33 +174,37 @@
         set_default_nside.nside = nside
     if nside is not None:
         set_default_nside.nside = nside
     return set_default_nside.nside
 
 
 def restore_scheduler(observation_id, scheduler, observatory, in_obs, filter_sched=None, fast=True):
-    """Put the scheduler and observatory in the state they were in. Handy for checking reward fucnction
+    """Put the scheduler and observatory in the state they were in.
+    Handy for checking reward fucnction
 
     Parameters
     ----------
     observation_id : int
         The ID of the last observation that should be completed
     scheduler : rubin_scheduler.scheduler.scheduler object
         Scheduler object.
     observatory : rubin_scheduler.scheduler.observatory.Model_observatory
         The observaotry object
     in_obs : np.array or str
-        Array of observations (formated like rubin_scheduler.scheduler.empty_observation). If a string,
+        Array of observations (formated like
+        rubin_scheduler.scheduler.empty_observation). If a string,
         assumed to be a file and SchemaConverter is used to load it.
     filter_sched : rubin_scheduler.scheduler.scheduler object
-        The filter scheduler. Note that we don't look up the official end of the previous night,
-        so there is potential for the loaded filters to not match.
+        The filter scheduler. Note that we don't look up the official
+        end of the previous night, so there is potential for the
+        loaded filters to not match.
     fast : bool (True)
-        If True, loads observations and passes them as an array to the `add_observations_array`
-        method. If False, passes observations individually with `add_observation` method.
+        If True, loads observations and passes them as an array to
+        the `add_observations_array` method. If False,
+        passes observations individually with `add_observation` method.
     """
     if isinstance(in_obs, str):
         sc = SchemaConverter()
         # load up the observations
         observations = sc.opsim2obs(in_obs)
     else:
         observations = in_obs
@@ -219,15 +224,16 @@
 
     if filter_sched is not None:
         # We've assumed the filter scheduler doesn't have any filters
         # May need to call the add_observation method on it if that
         # changes.
 
         # Make sure we have mounted the right filters for the night
-        # XXX--note, this might not be exact, but should work most of the time.
+        # XXX--note, this might not be exact, but should work most
+        # of the time.
         mjd_start_night = np.min(observations["mjd"][np.where(observations["night"] == obs["night"])])
         observatory.mjd = mjd_start_night
         conditions = observatory.return_conditions()
         filters_needed = filter_sched(conditions)
     else:
         filters_needed = ["u", "g", "r", "i", "y"]
 
@@ -237,15 +243,16 @@
     observatory.observatory.parked = False
     observatory.observatory.current_ra_rad = obs["RA"]
     observatory.observatory.current_dec_rad = obs["dec"]
     observatory.observatory.current_rot_sky_pos_rad = obs["rotSkyPos"]
     observatory.observatory.cumulative_azimuth_rad = obs["cummTelAz"]
     observatory.observatory.current_filter = obs["filter"]
     observatory.observatory.mounted_filters = filters_needed
-    # Note that we haven't updated last_az_rad, etc, but those values should be ignored.
+    # Note that we haven't updated last_az_rad, etc, but those
+    # values should be ignored.
 
     return scheduler, observatory
 
 
 def int_binned_stat(ids, values, statistic=np.mean):
     """
     Like scipy.binned_statistic, but for unique int ids
@@ -264,35 +271,35 @@
     for le, ri in zip(left, right):
         stat_results.append(statistic(ordered_values[le:ri]))
 
     return uids, np.array(stat_results)
 
 
 def gnomonic_project_toxy(ra1, dec1, r_acen, deccen):
-    """Calculate x/y projection of ra1/dec1 in system with center at r_acen, deccen.
-    Input radians. Grabbed from sims_selfcal"""
+    """Calculate x/y projection of ra1/dec1 in system with center
+    at r_acen, deccen. Input radians. Grabbed from sims_selfcal"""
     # also used in Global Telescope Network website
     cosc = np.sin(deccen) * np.sin(dec1) + np.cos(deccen) * np.cos(dec1) * np.cos(ra1 - r_acen)
     x = np.cos(dec1) * np.sin(ra1 - r_acen) / cosc
     y = (np.cos(deccen) * np.sin(dec1) - np.sin(deccen) * np.cos(dec1) * np.cos(ra1 - r_acen)) / cosc
     return x, y
 
 
 def gnomonic_project_tosky(x, y, r_acen, deccen):
-    """Calculate RA/dec on sky of object with x/y and RA/Cen of field of view.
-    Returns Ra/dec in radians."""
+    """Calculate RA/dec on sky of object with x/y and RA/Cen of
+    field of view. Returns Ra/dec in radians."""
     denom = np.cos(deccen) - y * np.sin(deccen)
     RA = r_acen + np.arctan2(x, denom)
     dec = np.arctan2(np.sin(deccen) + y * np.cos(deccen), np.sqrt(x * x + denom * denom))
     return RA, dec
 
 
 def match_hp_resolution(in_map, nside_out, unseen2nan=True):
-    """Utility to convert healpix map resolution if needed and change hp.UNSEEN values to
-    np.nan.
+    """Utility to convert healpix map resolution if needed and
+    change hp.UNSEEN values to np.nan.
 
     Parameters
     ----------
     in_map : np.array
         A valie healpix map
     nside_out : int
         The desired resolution to convert in_map to
@@ -308,15 +315,16 @@
         out_map[np.where(out_map == hp.UNSEEN)] = np.nan
     return out_map
 
 
 def raster_sort(x0, order=["x", "y"], xbin=1.0):
     """XXXX--depriciated, use tsp instead.
 
-    Do a sort to scan a grid up and down. Simple starting guess to traveling salesman.
+    Do a sort to scan a grid up and down. Simple starting guess
+    to traveling salesman.
 
     Parameters
     ----------
     x0 : array
     order : list
         Keys for the order x0 should be sorted in.
     xbin : float (1.)
@@ -356,19 +364,21 @@
         return order1[index_sorted]
     else:
         return order1
 
 
 class SchemaConverter:
     """
-    Record how to convert an observation array to the standard opsim schema
+    Record how to convert an observation array to the standard
+    opsim schema
     """
 
     def __init__(self):
-        # Conversion dictionary, keys are opsim schema, values are observation dtype names
+        # Conversion dictionary, keys are opsim schema, values
+        # are observation dtype names
         self.convert_dict = {
             "observationId": "ID",
             "night": "night",
             "observationStartMJD": "mjd",
             "observationStartLST": "lmst",
             "numExposures": "nexp",
             "visitTime": "visittime",
@@ -386,14 +396,15 @@
             "seeingFwhm500": "FWHM_500",
             "seeingFwhmGeom": "FWHM_geometric",
             "seeingFwhmEff": "FWHMeff",
             "fiveSigmaDepth": "fivesigmadepth",
             "slewTime": "slewtime",
             "slewDistance": "slewdist",
             "paraAngle": "pa",
+            "psudoParaAngle": "psudo_pa",
             "rotTelPos": "rotTelPos",
             "rotTelPos_backup": "rotTelPos_backup",
             "rotSkyPos": "rotSkyPos",
             "rotSkyPos_desired": "rotSkyPos_desired",
             "moonRA": "moonRA",
             "moonDec": "moonDec",
             "moonAlt": "moonAlt",
@@ -402,24 +413,26 @@
             "moonPhase": "moonPhase",
             "sunAlt": "sunAlt",
             "sunAz": "sunAz",
             "solarElong": "solarElong",
             "note": "note",
             "target": "target",
         }
-        # Column(s) not bothering to remap:  'observationStartTime': None,
+        # Column(s) not bothering to remap:
+        # 'observationStartTime': None,
         self.inv_map = {v: k for k, v in self.convert_dict.items()}
         # angles to convert
         self.angles_rad2deg = [
             "fieldRA",
             "fieldDec",
             "altitude",
             "azimuth",
             "slewDistance",
             "paraAngle",
+            "psudoParaAngle",
             "rotTelPos",
             "rotSkyPos",
             "rotSkyPos_desired",
             "rotTelPos_backup",
             "moonRA",
             "moonDec",
             "moonAlt",
@@ -514,64 +527,73 @@
     n : `int`
         Size of array to return. Default 1.
 
     Returns
     -------
     empty_observation : `np.array`
 
-    The numpy fields have the following labels. These fields are required to be set to be a valid observation
-    the model observatory can execute.
+    The numpy fields have the following labels. These fields are
+    required to be set to be a valid observation the model observatory
+    can execute.
     RA : `float`
-       The Right Acension of the observation (center of the field) (Radians)
+       The Right Acension of the observation (center of the field)
+       (Radians)
     dec : `float`
        Declination of the observation (Radians)
     mjd : `float`
-       Modified Julian Date at the start of the observation (time shutter opens)
+       Modified Julian Date at the start of the observation
+       (time shutter opens)
     exptime : `float`
        Total exposure time of the visit (seconds)
     filter : `str`
         The filter used. Should be one of u, g, r, i, z, y.
     rotSkyPos : `float`
-        The rotation angle of the camera relative to the sky E of N (Radians).
-        Will be ignored if rotTelPos is finite.
+        The rotation angle of the camera relative to the sky E of N
+        (Radians). Will be ignored if rotTelPos is finite.
         If rotSkyPos is set to NaN, rotSkyPos_desired is used.
     rotTelPos : `float`
-        The rotation angle of the camera relative to the telescope (radians).
-        Set to np.nan to force rotSkyPos to be used.
+        The rotation angle of the camera relative to the telescope
+        (radians). Set to np.nan to force rotSkyPos to be used.
     rotSkyPos_desired : `float`
-        If both rotSkyPos and rotTelPos are None/NaN, then rotSkyPos_desired (radians) is used.
-        If rotSkyPos_desired results in a valid rotTelPos, rotSkyPos is set to rotSkyPos_desired.
-        If rotSkyPos and rotTelPos are both NaN, and rotSkyPos_desired results in an out of range value
-        for the camera rotator, then rotTelPos_backup is used.
+        If both rotSkyPos and rotTelPos are None/NaN, then
+        rotSkyPos_desired (radians) is used. If rotSkyPos_desired
+        results in a valid rotTelPos, rotSkyPos is set to
+        rotSkyPos_desired. If rotSkyPos and rotTelPos are both NaN,
+        and rotSkyPos_desired results in an out of range value for the
+        camera rotator, then rotTelPos_backup is used.
     rotTelPos_backup : `float`
-        Rotation angle of the camera relative to the telescope (radians). Only used as a last resort if
-        rotSkyPos and rotTelPos are set to NaN and rotSkyPos_desired results in an out of range rotator value.
+        Rotation angle of the camera relative to the telescope (radians).
+        Only used as a last resort if rotSkyPos and rotTelPos are set
+        to NaN and rotSkyPos_desired results in an out of range rotator
+        value.
     nexp : `int`
         Number of exposures in the visit.
     flush_by_mjd : `float`
         If we hit this MJD, we should flush the queue and refill it.
     note : `str` (optional)
-        Usually good to set the note field so one knows which survey object generated the observation.
+        Usually good to set the note field so one knows which survey
+        object generated the observation.
     target : `str` (optional)
         A note about what target is being observed.
 
     Notes
     -----
 
     On the camera rotator angle. Order of priority goes:
     rotTelPos > rotSkyPos > rotSkyPos_desired > rotTelPos_backup
     where if rotTelPos is NaN, it checks rotSkyPos. If rotSkyPos is set,
     but not at an accessible rotTelPos, the observation will fail.
     If rotSkyPos is NaN, then rotSkyPos_desired is used. If
-    rotSkyPos_desired is at an inaccessbile rotTelPos, the observation does
-    not fail, but falls back to the value in rotTelPos_backup.
+    rotSkyPos_desired is at an inaccessbile rotTelPos, the observation
+    does not fail, but falls back to the value in rotTelPos_backup.
 
     Lots of additional fields that get filled in by the model observatory
     when the observation is completed.
-    See documentation at: https://rubin-scheduler.lsst.io/output_schema.html
+    See documentation at:
+    https://rubin-scheduler.lsst.io/output_schema.html
 
     """
 
     names = [
         "ID",
         "RA",
         "dec",
@@ -591,14 +613,15 @@
         "slewtime",
         "visittime",
         "slewdist",
         "fivesigmadepth",
         "alt",
         "az",
         "pa",
+        "psudo_pa",
         "clouds",
         "moonAlt",
         "sunAlt",
         "note",
         "target",
         "field_id",
         "survey_id",
@@ -642,14 +665,15 @@
         float,
         float,
         float,
         float,
         float,
         float,
         float,
+        float,
         "U40",
         "U40",
         int,
         int,
         int,
         float,
         float,
@@ -679,34 +703,42 @@
 
 
     Note
     ----
     mjd_tol : `float`
         The tolerance on how early an observation can execute (days).
         Observation will be considered valid to attempt
-        when mjd-mjd_tol < current MJD < flush_by_mjd (and other conditions below pass)
+        when mjd-mjd_tol < current MJD < flush_by_mjd (and other
+        conditions below pass)
     dist_tol : `float`
-        The angular distance an observation can be away from the specified RA,Dec and
-        still count as completing the observation (radians).
+        The angular distance an observation can be away from the
+        specified RA,Dec and still count as completing the observation
+        (radians).
     alt_min : `float`
-        The minimum altitude to consider executing the observation (radians).
+        The minimum altitude to consider executing the observation
+        (radians).
     alt_max : `float`
         The maximuim altitude to try observing (radians).
     HA_max : `float`
-        Hour angle limit. Constraint is such that for hour angle running from 0 to 24 hours,
-        the target RA,Dec must be greather than HA_max and less than HA_min. Set HA_max to 0 for
-        no limit. (hours)
+        Hour angle limit. Constraint is such that for hour angle
+        running from 0 to 24 hours, the target RA,Dec must be greather
+        than HA_max and less than HA_min. Set HA_max to 0 for no
+        limit. (hours)
     HA_min : `float`
-        Hour angle limit. Constraint is such that for hour angle running from 0 to 24 hours,
-        the target RA,Dec must be greather than HA_max and less than HA_min. Set HA_min to 24 for
+        Hour angle limit. Constraint is such that for hour angle
+        running from 0 to 24 hours, the target RA,Dec must be greather
+        than HA_max and less than HA_min. Set HA_min to 24 for
         no limit. (hours)
-    sun_alt_max : float
+    sun_alt_max : `float`
         The sun must be below sun_alt_max to execute. (radians)
+    moon_min_distance : `float`
+        The minimum distance to demand the moon should be away (radians)
     observed : `bool`
-        If set to True, scheduler will probably consider this a completed observation an never attempt it.
+        If set to True, scheduler will probably consider this a
+        completed observation and never attempt it.
 
     """
 
     # Standard things from the usual observations
     names = [
         "ID",
         "RA",
@@ -743,18 +775,19 @@
         "mjd_tol",
         "dist_tol",
         "alt_min",
         "alt_max",
         "HA_max",
         "HA_min",
         "sun_alt_max",
+        "moon_min_distance",
         "observed",
         "scripted_id",
     ]
-    types += [float, float, float, float, float, float, float, bool, int]
+    types += [float, float, float, float, float, float, float, float, bool, int]
     result = np.zeros(n, dtype=list(zip(names, types)))
     return result
 
 
 def hp_kd_tree(nside=None, leafsize=100, scale=1e5):
     """
     Generate a KD-tree of healpixel locations
@@ -775,29 +808,50 @@
 
     hpid = np.arange(hp.nside2npix(nside))
     ra, dec = _hpid2_ra_dec(nside, hpid)
     return _build_tree(ra, dec, leafsize, scale=scale)
 
 
 class HpInLsstFov:
-    """
-    Return the healpixels within a pointing.
-    A very simple LSST camera model with no chip/raft gaps.
+    """Return the healpixels in an underlying healpix grid that
+    overlap an observation/pointing.
+
+    This uses a very simple circular LSST camera model with no chip/raft gaps.
+
+    Parameters
+    ----------
+    nside : `int`, optional
+        Nside to match for the healpix array.
+        Default None uses `set_default_nside`.
+    fov_radius : `float`, optional
+        Radius of the field of view in degrees. Default 1.75
+        covers the inscribed circle.
+    scale : `float`, optional
+        How many sig figs to round when considering matches to healpixels.
+        Useful for ensuring identical results cross-ploatform where
+        float precision can vary.
+
+
+    Examples
+    --------
+    Set up the class, then call to convert pointings to indices in the
+    healpix array. Note that RA and dec should be in RADIANS.
+
+    ```
+    >>> ra = np.radians(30)
+    >>> dec = np.radians(-20)
+    >>> pointing2indx = HpInLsstFov()
+    >>> indices = pointing2indx(ra, dec)
+    >>> indices
+    [8138, 8267]
+    ```
+
     """
 
     def __init__(self, nside=None, fov_radius=1.75, scale=1e5):
-        """
-        Parameters
-        ----------
-        fov_radius : float (1.75)
-            Radius of the filed of view in degrees
-        scale : float (1e5)
-            How many sig figs to round off to. Useful for ensuring identical results
-            cross-ploatform where float precision can vary.
-        """
         if nside is None:
             nside = set_default_nside()
 
         self.tree = hp_kd_tree(nside=nside, scale=scale)
         self.radius = np.round(xyz_angular_radius(fov_radius) * scale).astype(int)
         self.scale = scale
 
@@ -913,15 +967,16 @@
                     [x_rotated[0], y_rotated[0]],
                 ]
             ).astype(int)
         )
 
         ra_to_check, dec_to_check = _hpid2_ra_dec(self.nside, indices_to_check)
 
-        # Project the indices to check to the tangent plane, see if they fall inside the polygon
+        # Project the indices to check to the tangent plane, see
+        # if they fall inside the polygon
         x, y = gnomonic_project_toxy(ra_to_check, dec_to_check, ra, dec)
         x = (x * self.scale).astype(int)
         y = (y * self.scale).astype(int)
         for i, xcheck in enumerate(x):
             # I wonder if I can do this all at once rather than a loop?
             if bb_path.contains_point((x[i], y[i])):
                 indices.append(indices_to_check[i])
@@ -1001,22 +1056,23 @@
     Parameters
     ----------
     night : int or array
         The night we want to convert to a season
     offset : float or array (0)
         Offset to be applied to night (days)
     modulo : int (None)
-        If the season should be modulated (i.e., so we can get all even years)
-        (seasons, years w/default season_length)
+        If the season should be modulated (i.e., so we can get all
+        even years) (seasons, years w/default season_length)
     max_season : int (None)
         For any season above this value (before modulo), set to -1
     season_length : float (365.25)
         How long to consider one season (nights)
     floor : bool (True)
-        If true, take the floor of the season. Otherwise, returns season as a float
+        If true, take the floor of the season. Otherwise, returns
+        season as a float
     """
     if np.size(night) == 1:
         night = np.ravel(np.array([night]))
     result = night + offset
     result = result / season_length
     if floor:
         result = np.floor(result)
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/sim_archive/sim_archive.py` & `rubin_scheduler-1.2.0/rubin_scheduler/sim_archive/sim_archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import numpy as np
 import pandas as pd
 import yaml
 from astropy.time import Time
-from conda.cli.main_list import print_packages
-from conda.gateways.disk.test import is_conda_environment
 
 import rubin_scheduler
 from rubin_scheduler.scheduler import sim_runner
 from rubin_scheduler.scheduler.utils import SchemaConverter
 
 LOGGER = logging.getLogger(__name__)
 
@@ -66,26 +64,28 @@
     capture_env=True,
 ):
     """Create or fill a local simulation archive directory.
 
     Parameters
     ----------
     observations : `numpy.recarray`
-        The observations data, in the "obs" format as accepted and created by
-        `rubin_scheduler.scheduler.utils.SchemaConverter`.
+        The observations data, in the "obs" format as accepted and
+        created by `rubin_scheduler.scheduler.utils.SchemaConverter`.
     reward_df : `pandas.DataFrame`, optional
         The reward data, by default None.
     obs_rewards : `pandas.DataFrame`, optional
         The observation rewards data, by default None.
     in_files : `dict`, optional
-        Additional input files to be included in the archive, by default {}.
+        Additional input files to be included in the archive,
+        by default {}.
     sim_runner_kwargs : `dict`, optional
         Additional simulation runner keyword arguments, by default {}.
     tags : `list` [`str`], optional
-        A list of tags/keywords to be included in the metadata, by default [].
+        A list of tags/keywords to be included in the metadata, by
+        default [].
     label : `str`, optional
         A label to be included in the metadata, by default None.
     data_path : `str` or `pathlib.Path`, optional
         The path to the simulation archive directory, by default None.
     capture_env : `bool`
         Use the current environment as the sim environment.
         Defaults to True.
@@ -129,15 +129,16 @@
     if capture_env:
         # Save the conda environment
         conda_prefix = Path(sys.executable).parent.parent.as_posix()
         if have_conda and is_conda_environment(conda_prefix):
             conda_base_fname = "environment.txt"
             environment_fname = data_path.joinpath(conda_base_fname).as_posix()
 
-            # Python equivilent of conda list --export -p $conda_prefix > $environment_fname
+            # Python equivilent of
+            # conda list --export -p $conda_prefix > $environment_fname
             with open(environment_fname, "w") as environment_io:
                 with redirect_stdout(environment_io):
                     print_packages(conda_prefix, format="export")
 
             files["environment"] = {"name": conda_base_fname}
 
         # Save pypi packages
@@ -237,17 +238,19 @@
 
 def transfer_archive_dir(archive_dir, archive_base_uri="s3://rubin-scheduler-prenight/opsim/"):
     """Transfer the contents of an archive directory to an resource.
 
     Parameters:
     ----------
     archive_dir : `str`
-        The path to the archive directory containing the files to be transferred.
+        The path to the archive directory containing the files to be
+        transferred.
     archive_base_uri : `str`, optional
-        The base URI where the archive files will be transferred to. Default is "s3://rubin-scheduler-prenight/opsim/".
+        The base URI where the archive files will be transferred to.
+        Default is "s3://rubin-scheduler-prenight/opsim/".
 
     Returns:
     -------
     resource_rpath : `ResourcePath`
         The destination resource.
     """
 
@@ -490,15 +493,16 @@
         The scheduler to use.
     archive_uri : `str`, optional
         The root URI of the archive resource into which the results should
         be stored. Defaults to None.
     label : `str`, optional
         The label for the simulation in the archive. Defaults to None.
     tags : `list` of `str`, optional
-        The tags for the simulation in the archive. Defaults to an empty list.
+        The tags for the simulation in the archive. Defaults to an
+        empty list.
     script : `str`
         The filename of the script producing this simulation.
         Defaults to None.
     notebook : `str`, optional
         The filename of the notebook producing the simulation.
         Defaults to None.
 
@@ -525,18 +529,18 @@
     Additional parameters not described above will be passed into
     `sim_runner`.
 
     If the `archive_uri` parameter is not supplied, `sim_runner` is run
     directly, so that `drive_sim` can act as a drop-in replacement of
     `sim-runner`.
 
-    In a jupyter notebook, the notebook can be saved for the notebook paramater
-    using `%notebook $notebook_fname` (where `notebook_fname` is variable
-    holding the filename for the notebook) in the cell prior to calling
-    `drive_sim`.
+    In a jupyter notebook, the notebook can be saved for the notebook
+    paramater using `%notebook $notebook_fname` (where `notebook_fname`
+    is variable holding the filename for the notebook) in the cell prior
+    to calling `drive_sim`.
     """
     if "record_rewards" in kwargs:
         if kwargs["record_rewards"] and not scheduler.keep_rewards:
             raise ValueError("To keep rewards, scheduler.keep_rewards must be True")
     else:
         kwargs["record_rewards"] = scheduler.keep_rewards
 
@@ -544,16 +548,16 @@
     if script is not None:
         in_files["script"] = script
 
     if notebook is not None:
         in_files["notebook"] = notebook
 
     with TemporaryDirectory() as local_data_dir:
-        # We want to store the state of the scheduler at the start of the sim,
-        # so we need to save it now before we run the simulation.
+        # We want to store the state of the scheduler at the start of
+        # the sim, so we need to save it now before we run the simulation.
         scheduler_path = Path(local_data_dir).joinpath("scheduler.pickle.xz")
         with lzma.open(scheduler_path, "wb", format=lzma.FORMAT_XZ) as pio:
             pickle.dump(scheduler, pio)
             in_files["scheduler"] = scheduler_path.as_posix()
 
         sim_results = sim_runner(observatory, scheduler, **kwargs)
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/almanac.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/almanac.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import numpy as np
 from scipy.interpolate import interp1d
 
 from rubin_scheduler.data import get_data_dir
 
 
 class Almanac:
-    """Class to load and return pre-computed information about the LSST site."""
+    """Class to load and return pre-computed information about the
+    LSST site."""
 
     def __init__(self, mjd_start=None, kind="quadratic"):
         # Load up the sunrise/sunset times
         data_dir = os.path.join(get_data_dir(), "site_models")
 
         temp = np.load(os.path.join(data_dir, "sunsets.npz"))
         self.sunsets = temp["almanac"].copy()
@@ -87,16 +88,16 @@
 
         Parameters
         ----------
         mjd : `float`
             A UTC MJD that occurs during the desired night.
             Defaults to None.
         evening_date : `str` or `datetime.date`
-            The local date of the evening of the night whose index is desired,
-            in ISO8601 format (YYYY-MM-DD). Defaults to None.
+            The local date of the evening of the night whose index is
+            desired, in ISO8601 format (YYYY-MM-DD). Defaults to None.
         longitude : `float` or  `astropy.coordinates.angles.core.Angle`
             If a float, then the value is interpreted as being in radians.
             Defaults to None.
 
         Returns
         -------
         sunset_info : `numpy.void`
@@ -134,16 +135,16 @@
 
     def index_for_local_evening(self, evening_date, longitude):
         """The index of the night with sunset at a given local date.
 
         Parameters
         ----------
         evening_date : `str` or `datetime.date`
-            The local date of the evening of the night whose index is desired,
-            in ISO8601 format (YYYY-MM-DD).
+            The local date of the evening of the night whose index i
+            desired, in ISO8601 format (YYYY-MM-DD).
         longitude : `float` or  `astropy.coordinates.angles.core.Angle`
             If a float, then the value is interpreted as being in radians.
 
         Returns
         -------
         night_index : `int`
             The index of the requested night.
@@ -156,16 +157,17 @@
         if isinstance(evening_date, str):
             evening_date = datetime.date.fromisoformat(evening_date)
 
         evening_datetime = datetime.datetime(evening_date.year, evening_date.month, evening_date.day)
         evening_mjd = np.floor(evening_datetime.timestamp() / (24 * 60 * 60) + 40587)
 
         # Depending on the time of year, the UTC date rollover might not
-        # always be on the same side of local sunset. Shift by the longitude
-        # to make sure the rollover is always near midnight, far from sunset.
+        # always be on the same side of local sunset. Shift by the
+        # longitude to make sure the rollover is always near midnight,
+        # far from sunset.
         matching_nights = np.argwhere(
             np.floor(self.sunsets["sunset"] + longitude / (2 * np.pi)) == evening_mjd
         )
         if len(matching_nights) < 1:
             raise ValueError(f"Requested night {evening_date} outside of almanac date range")
 
         night_index = matching_nights.item()
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/cloud_data.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/cloud_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,59 +9,65 @@
 
 from rubin_scheduler.data import get_data_dir
 
 
 class CloudData:
     """Handle the cloud information.
 
-    This class deals with the cloud information that was previously produced for
-    OpSim version 3.
+    This class deals with the cloud information that was previously
+    produced for OpSim version 3.
 
     Parameters
     ----------
     start_time : astropy.time.Time
         The time of the start of the simulation.
-        The cloud database will be assumed to start on Jan 01 of the same year.
+        The cloud database will be assumed to start on Jan 01 of
+        the same year.
     cloud_db : str, optional
         The full path name for the cloud database. Default None,
-        which will use the database stored in the module (site_models/clouds_ctio_1975_2022.db).
+        which will use the database stored in the module
+        (site_models/clouds_ctio_1975_2022.db).
     offset_year : float, optional
         Offset into the cloud database by 'offset_year' years. Default 0.
     scale : float (1e6)
-        Enforce machine precision for cross-platform repeatability by scaling and rounding date values.
+        Enforce machine precision for cross-platform repeatability by
+        scaling and rounding date values.
     """
 
     def __init__(self, start_time, cloud_db=None, offset_year=0, scale=1e6):
         self.cloud_db = cloud_db
         if self.cloud_db is None:
             self.cloud_db = os.path.join(get_data_dir(), "site_models", "clouds_ctio_1975_2022.db")
 
-        # Cloud database starts in Jan 01 of the year of the start of the simulation.
+        # Cloud database starts in Jan 01 of the year of the
+        # start of the simulation.
         year_start = start_time.datetime.year + offset_year
         self.start_time = Time("%d-01-01" % year_start, format="isot", scale="tai")
 
         self.cloud_dates = None
         self.cloud_values = None
         self.scale = scale
         self.read_data()
 
     def __call__(self, time):
         """Get the cloud for the specified time.
 
         Parameters
         ----------
         time : astropy.time.Time
-            Time in the simulation for which to find the current cloud coverage.
-            The difference between this time and the start_time, plus the offset,
-            will be used to query the cloud database for the 'current' conditions.
+            Time in the simulation for which to find the current cloud
+            coverage. The difference between this time and the start_time,
+            plus the offset, will be used to query the cloud database
+            for the 'current' conditions.
 
         Returns
         -------
         float
-            The fraction of the sky that is cloudy (measured in steps of 8ths) closest to the specified time.
+            The fraction of the sky that is cloudy (measured in
+            steps of 8ths) closest to the specified time.
         """
         delta_time = (time - self.start_time).sec
         dbdate = delta_time % self.time_range + self.min_time
         if self.scale is not None:
             dbdate = np.round(dbdate * self.scale).astype(int)
         idx = np.searchsorted(self.cloud_dates, dbdate)
         # searchsorted ensures that left < date < right
@@ -80,37 +86,41 @@
             idx[to_sub] -= 1
 
         return self.cloud_values[idx]
 
     def read_data(self):
         """Read the cloud data from disk.
 
-        The default behavior is to use the module stored database. However, an
-        alternate database file can be provided. The alternate database file needs to have a
-        table called *Cloud* with the following columns:
+        The default behavior is to use the module stored database.
+        However, an alternate database file can be provided. The alternate
+        database file needs to have a table called *Cloud* with the
+        following columns:
 
         cloudId
             int : A unique index for each cloud entry.
         c_date
-            int : The time (units=seconds) since the start of the simulation for the cloud observation.
+            int : The time (units=seconds) since the start of the
+            simulation for the cloud observation.
         cloud
             float : The cloud coverage (in steps of 8ths) of the sky.
         """
         with sqlite3.connect(self.cloud_db) as conn:
             cur = conn.cursor()
             query = "select c_date, cloud from Cloud order by c_date;"
             cur.execute(query)
             results = np.array(cur.fetchall())
             self.cloud_dates = np.hsplit(results, 2)[0].flatten()
             self.cloud_values = np.hsplit(results, 2)[1].flatten()
             cur.close()
-        # Make sure seeing dates are ordered appropriately (monotonically increasing).
+        # Make sure seeing dates are ordered appropriately (monotonically
+        # increasing).
         ordidx = self.cloud_dates.argsort()
         self.cloud_dates = self.cloud_dates[ordidx]
-        # Record this information, in case the cloud database does not start at t=0.
+        # Record this information, in case the cloud database does not
+        # start at t=0.
         self.min_time = self.cloud_dates[0]
         self.max_time = self.cloud_dates[-1]
         self.time_range = self.max_time - self.min_time
         if self.scale is not None:
             self.cloud_dates = np.round(self.cloud_dates * self.scale).astype(int)
         self.cloud_values = self.cloud_values[ordidx]
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/cloud_model.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/cloud_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 import warnings
 
 import numpy as np
 
 
 class CloudModel:
     """LSST cloud calculations for cloud extinction.
-    Currently this actually only returns the cloud coverage of the sky, exactly as reported in the
-    cloud database (thus the sky coverage, in fractions of 8ths).
+    Currently this actually only returns the cloud coverage of the sky,
+    exactly as reported in the cloud database (thus the sky coverage,
+    in fractions of 8ths).
 
 
     Parameters
     ----------
     XXX--update docstring
 
     self.efd_requirements and self.map_requirements are also set.
     efd_requirements is a tuple: (list of str, float).
-    This corresponds to the data columns required from the EFD and the amount of time history required.
-    target_requirements is a list of str.
-    This corresponds to the data columns required in the target map dictionary passed when calculating the
-    processed telemetry values.
+    This corresponds to the data columns required from the EFD and
+    the amount of time history required. target_requirements is a
+    list of str. This corresponds to the data columns required in the
+    target map dictionary passed when calculating the processed
+    telemetry values.
     """
 
     def __init__(self, cloud_column="cloud", altitude_column="altitude", azimuth_column="azimuth"):
         self.altcol = altitude_column
         self.azcol = azimuth_column
         self.cloudcol = cloud_column
 
@@ -35,17 +37,18 @@
     def config_info(self):
         """"""
         warnings.warn("The config_info method is deprecated.")
 
     def __call__(self, cloud_value, altitude):
         """Calculate the sky coverage due to clouds.
 
-        This is where we'd plug in Peter's cloud transparency maps and predictions.
-        We could also try translating cloud transparency into a cloud extinction.
-        For now, we're simply returning the cloud coverage that we already got from the database,
+        This is where we'd plug in Peter's cloud transparency maps and
+        predictions. We could also try translating cloud transparency
+        into a cloud extinction. For now, we're simply returning the
+        cloud coverage that we already got from the database,
         but multiplied over the whole sky to provide a map.
 
         Parameters
         ----------
         cloud_value: float or efdData dict
             The value to give the clouds (XXX-units?).
         altitude:  float, np.array, or targetDict
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/downtime_model.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/downtime_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 class DowntimeModel:
     """Downtime estimates, both scheduled and unscheduled.
 
     Parameters
     ----------
     config: DowntimeModelConfig, optional
         A configuration class for the downtime model.
-        This can be None, in which case the default DowntimeModelConfig is used.
-        The user should set any non-default values for DowntimeModelConfig before
-        configuration of the actual DowntimeModel.
+        This can be None, in which case the default DowntimeModelConfig
+        is used. The user should set any non-default values for
+        DowntimeModelConfig before configuration of the actual
+        DowntimeModel.
 
     self.efd_requirements and self.target_requirements are also set.
     efd_requirements is a tuple: (list of str, float).
-    This corresponds to the data columns required from the EFD and the amount of time history required.
-    target_requirements is a list of str.
-    This corresponds to the data columns required in the target dictionary passed when calculating the
-    processed telemetry values.
+    This corresponds to the data columns required from the EFD and
+    the amount of time history required. target_requirements is a
+    list of str. This corresponds to the data columns required in the
+    target dictionary passed when calculating the processed telemetry
+    values.
     """
 
     def __init__(
         self,
         sched_down_col="scheduled_downtimes",
         unsched_down_col="unscheduled_downtimes",
         time_col="time",
@@ -44,24 +46,27 @@
         Parameters
         ----------
         efd_data: dict
             Dictionary of input telemetry, typically from the EFD.
             This must contain columns self.efd_requirements.
             (work in progress on handling time history).
         target_dict: dict
-            Dictionary of target values over which to calculate the processed telemetry.
-            (e.g. mapDict = {'ra': [], 'dec': [], 'altitude': [], 'azimuth': [], 'airmass': []})
-            Here we use 'time', an astropy.time.Time, as we just need to know the time.
+            Dictionary of target values over which to calculate the
+            processed telemetry. (e.g. mapDict = {'ra': [],
+            'dec': [], 'altitude': [], 'azimuth': [], 'airmass': []})
+            Here we use 'time', an astropy.time.Time, as we just need
+            to know the time.
 
         Returns
         -------
         dict of bool, astropy.time.Time, astropy.time.Time
             Status of telescope (True = Down, False = Up) at time,
-            time of expected end of downtime (~noon of the first available day),
-            time of next scheduled downtime (~noon of the first available day).
+            time of expected end of downtime (~noon of the first
+            available day), time of next scheduled downtime (~noon
+            of the first available day).
         """
         # Check for downtime in scheduled downtimes.
         time = target_dict[self.target_requirements]
         next_start = efd_data[self.sched_down]["start"].searchsorted(time, side="right")
         next_end = efd_data[self.sched_down]["end"].searchsorted(time, side="right")
         if next_start > next_end:
             # Currently in a scheduled downtime.
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/generate_planets.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/generate_planets.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/generate_sun_moon_pos.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/generate_sun_moon_pos.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 
     sun_moon_info["moon_alt"] = moon_aa.alt.rad
     sun_moon_info["moon_az"] = moon_aa.az.rad
 
     sun_moon_sep = _angular_separation(sun.ra.rad, sun.dec.rad, moon.ra.rad, moon.dec.rad)
     sun_moon_info["moon_phase"] = sun_moon_sep / np.pi * 100.0
 
-    # Let's cut down a bit, no need to save info when the sun is high in the sky
+    # Let's cut down a bit, no need to save info when the sun is
+    # high in the sky
     good_suns = np.where(sun_moon_info["sun_alt"] < np.radians(10.0))
     sun_moon_info = sun_moon_info[good_suns]
 
     np.savez("sun_moon.npz", sun_moon_info=sun_moon_info)
 
-    # Takes 6.25 mintues for 221,072.  In a sim, I need 5e6, so 141 min--over 2 hours.
+    # Takes 6.25 mintues for 221,072.  In a sim, I need 5e6, so
+    # 141 min--over 2 hours.
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/generate_sunsets.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/generate_sunsets.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/read_fields.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/read_fields.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/scheduled_downtime_data.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/scheduled_downtime_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,58 +8,64 @@
 
 from rubin_scheduler.data import get_data_dir
 
 
 class ScheduledDowntimeData:
     """Read the scheduled downtime data.
 
-    This class deals with the scheduled downtime information that was previously produced for
-    OpSim version 3.
+    This class deals with the scheduled downtime information that
+    was previously produced for OpSim version 3.
 
     Parameters
     ----------
     start_time : `astropy.time.Time`
         The time of the start of the simulation.
-        The cloud database will be assumed to start on Jan 01 of the same year.
+        The cloud database will be assumed to start on Jan 01 of the
+        same year.
     cloud_db : `str`, optional
         The full path name for the cloud database. Default None,
-        which will use the database stored in the module ($SIMS_CLOUDMODEL_DIR/data/cloud.db).
+        which will use the database stored in the module
+        ($SIMS_CLOUDMODEL_DIR/data/cloud.db).
     start_of_night_offset : `float`, optional
-        The fraction of a day to offset from MJD.0 to reach the defined start of a night ('noon' works).
-        Default 0.16 (UTC midnight in Chile) - 0.5 (minus half a day) = -0.34
+        The fraction of a day to offset from MJD.0 to reach the defined
+        start of a night ('noon' works). Default 0.16 (UTC midnight
+        in Chile) - 0.5 (minus half a day) = -0.34
     """
 
     def __init__(self, start_time, scheduled_downtime_db=None, start_of_night_offset=-0.34):
         self.scheduled_downtime_db = scheduled_downtime_db
         if self.scheduled_downtime_db is None:
             self.scheduled_downtime_db = os.path.join(get_data_dir(), "site_models", "scheduled_downtime.db")
 
-        # downtime database starts in Jan 01 of the year of the start of the simulation.
+        # downtime database starts in Jan 01 of the year of the
+        # start of the simulation.
         year_start = start_time.datetime.year
         self.night0 = Time("%d-01-01" % year_start, format="isot", scale="tai") + TimeDelta(
             start_of_night_offset, format="jd"
         )
 
-        # Scheduled downtime data is a np.ndarray of start / end / activity for each scheduled downtime.
+        # Scheduled downtime data is a np.ndarray of start / end /
+        # activity for each scheduled downtime.
         self.downtime = None
         self.read_data()
 
     def __call__(self):
         """Return the current (if any) and any future scheduled downtimes.
 
         Parameters
         ----------
         time : `astropy.time.Time`
             Time in the simulation for which to find the current downtime.
 
         Returns
         -------
         downtime : `np.ndarray`
-            The array of all unscheduled downtimes, with keys for 'start', 'end', 'activity',
-            corresponding to astropy.time.Time, astropy.time.Time, and str.
+            The array of all unscheduled downtimes, with keys for
+            'start', 'end', 'activity', corresponding to
+            astropy.time.Time, astropy.time.Time, and str.
         """
         return self.downtime
 
     def _downtime_status(self, time):
         """Look behind the scenes at the downtime status/next values"""
         next_start = self.downtime["start"].searchsorted(time, side="right")
         next_end = self.downtime["end"].searchsorted(time, side="right")
@@ -67,20 +73,22 @@
             current = self.downtime[next_end]
         else:
             current = None
         future = self.downtime[next_start:]
         return current, future
 
     def read_data(self):
-        """Read the scheduled downtime information from disk and translate to astropy.time.Times.
+        """Read the scheduled downtime information from disk and
+        translate to astropy.time.Times.
 
-        This function gets the appropriate database file and creates the set of
-        scheduled downtimes from it. The default behavior is to use the module stored
-        database. However, an alternate database file can be provided. The alternate
-        database file needs to have a table called *Downtime* with the following columns:
+        This function gets the appropriate database file and creates
+        the set of scheduled downtimes from it. The default behavior
+        is to use the module stored database. However, an alternate
+        database file can be provided. The alternate database file needs
+        to have a table called *Downtime* with the following columns:
 
         night : `int`
             The night (from start of simulation) the downtime occurs.
         duration : `int`
             The duration (units=days) of the downtime.
         activity : `str`
             A description of the activity involved.
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/seeing_data.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/seeing_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,57 +7,63 @@
 import numpy as np
 from astropy.time import Time
 
 from rubin_scheduler.data import get_data_dir
 
 
 class SeeingData:
-    """Read the seeing data from disk and return appropriate FWHM_500 value at a given time.
-    This is for use in simulations only. Otherwise data would come from the EFD.
+    """Read the seeing data from disk and return appropriate FWHM_500
+    value at a given time. This is for use in simulations only.
+    Otherwise data would come from the EFD.
 
     Parameters
     ----------
     start_time : astropy.time.Time
         The time of the start of the simulation.
-        The seeing database will be assumed to start on Jan 01 of the same year.
+        The seeing database will be assumed to start on Jan 01 of the
+        same year.
     seeing_db : str or None, optional
         The name of the seeing database.
-        If None (default), this will use the simsee_pachon_58777_13.db file in the 'data' directory
-        of this package.
+        If None (default), this will use the simsee_pachon_58777_13.db
+        file in the 'data' directory of this package.
         Other available seeing databases from sims_seeingModel include:
         seeing.db (the original, less-variable, 3 year seeing database)
-        simsee_pachon_58777_13.db (the current default, 10 year, seeing database)
-        simsee_pachon_58777_16.db (a similar, but slightly offset, 13 year seeing database)
-        For more info on simsee_pachon_58777_*, see https://github.com/lsst/sims_seeingModel/issues/2
+        simsee_pachon_58777_13.db (the current default, 10 year,
+        seeing database) simsee_pachon_58777_16.db (a similar, but
+        slightly offset, 13 year seeing database)
+        For more info on simsee_pachon_58777_*, see
+        https://github.com/lsst/sims_seeingModel/issues/2
     offset_year : float, optional
         Offset into the cloud database by 'offset_year' years. Default 0.
     """
 
     def __init__(self, start_time, seeing_db=None, offset_year=0):
         self.seeing_db = seeing_db
         if self.seeing_db is None:
             self.seeing_db = os.path.join(get_data_dir(), "site_models", "simsee_pachon_58777_13.db")
 
-        # Seeing database starts in Jan 01 of the year of the start of the simulation
+        # Seeing database starts in Jan 01 of the year of the start of
+        # the simulation
         year_start = start_time.datetime.year + offset_year
         self.start_time = Time("%d-01-01" % year_start, format="isot", scale="tai")
 
         self.seeing_dates = None
         self.seeing_values = None
         self.read_data()
 
     def __call__(self, time):
         """Get the FWHM_500 value for the specified time.
 
         Parameters
         ----------
         time : astropy.time.Time
-            Time in the simulation for which to find the 'current' zenith seeing values.
-            The difference between this time and the start_time, plus the offset,
-            will be used to query the seeing database.
+            Time in the simulation for which to find the 'current'
+            zenith seeing values. The difference between this time and
+            the start_time, plus the offset, will be used to query the
+            seeing database.
 
         Returns
         -------
         float
             The FWHM_500(") closest to the specified time.
         """
         delta_time = (time - self.start_time).sec
@@ -78,34 +84,38 @@
             to_sub = np.where(d1 < d2)
             idx[to_sub] -= 1
         return self.seeing_values[idx]
 
     def read_data(self):
         """Read the seeing information from disk.
 
-        The default behavior is to use the module stored database. However, an
-        alternate database file can be provided. The alternate database file needs to have a
-        table called *Seeing* with the following columns:
+        The default behavior is to use the module stored database.
+        However, an alternate database file can be provided. The
+        alternate database file needs to have a table called *Seeing*
+        with the following columns:
 
         seeingId
             int : A unique index for each seeing entry.
         s_date
-            int : The time (in seconds) from the start of the simulation, for the seeing observation.
+            int : The time (in seconds) from the start of the
+            simulation, for the seeing observation.
         seeing
-            float : The FWHM of the atmospheric PSF (in arcseconds) at zenith.
+            float : The FWHM of the atmospheric PSF (in arcseconds) at
+            zenith.
         """
         with sqlite3.connect(self.seeing_db) as conn:
             cur = conn.cursor()
             query = "select s_date, seeing from Seeing order by s_date;"
             cur.execute(query)
             results = np.array(cur.fetchall())
             self.seeing_dates = np.hsplit(results, 2)[0].flatten()
             self.seeing_values = np.hsplit(results, 2)[1].flatten()
             cur.close()
-        # Make sure seeing dates are ordered appropriately (monotonically increasing).
+        # Make sure seeing dates are ordered appropriately
+        # (monotonically increasing).
         ordidx = self.seeing_dates.argsort()
         self.seeing_dates = self.seeing_dates[ordidx]
         self.seeing_values = self.seeing_values[ordidx]
         self.min_time = self.seeing_dates[0]
         self.max_time = self.seeing_dates[-1]
         self.time_range = self.max_time - self.min_time
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/seeing_model.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/seeing_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,42 +6,46 @@
 
 from rubin_scheduler.utils import SysEngVals
 
 
 class SeeingModel:
     """LSST FWHM calculations for FWHM_effective and FWHM_geometric.
 
-    Calculations of the delivered values are based on equations in Document-20160
-    ("Atmospheric and Delivered Image Quality in OpSim" by Bo Xin, George Angeli, Zeljko Ivezic)
-    An example of the calculation of delivered image seeing from DIMM FWHM_500 is available in
-    https://smtn-002.lsst.io/#calculating-m5-values-in-the-lsst-operations-simulator
+    Calculations of the delivered values are based on equations in
+    Document-20160 ("Atmospheric and Delivered Image Quality in OpSim"
+    by Bo Xin, George Angeli, Zeljko Ivezic)
+    An example of the calculation of delivered image seeing from DIMM
+    FWHM_500 is available in
+    https://smtn-002.lsst.io/
+    #calculating-m5-values-in-the-lsst-operations-simulator
 
     Parameters
     ----------
     filter_list : `list` [`str`], opt
-        List of the filter bandpasses for which to calculate delivered FWHM_effective and FWHM_geometric
+        List of the filter bandpasses for which to calculate delivered
+        FWHM_effective and FWHM_geometric
         Default ['u', 'g', 'r', 'i', 'z', 'y']
     eff_wavelens : `list` [`float`] or None, opt
-        Effective wavelengths for those bandpasses, in nanometers. If None, loades from
-        rubin_scheduler.utils.SysEngVals
+        Effective wavelengths for those bandpasses, in nanometers.
+        If None, loades from rubin_scheduler.utils.SysEngVals
     telescope_seeing : `float`, opt
-        The contribution to the delivered FWHM from the telescope, in arcseconds.
-        Default 0.25"
+        The contribution to the delivered FWHM from the telescope,
+        in arcseconds. Default 0.25"
     optical_design_seeing : `float`, opt
-        The contribution to the seeing from the optical design, in arcseconds.
-        Default 0.08 arcseconds
+        The contribution to the seeing from the optical design, in
+        arcseconds. Default 0.08 arcseconds
     camera_seeing : `float`, opt
         The contribution to the seeing from the camera, in arcseconds.
         Default 0.30 arcseconds
     raw_seeing_wavelength : `float`, opt
-        The wavelength of the DIMM-delivered equivalent FWHM, in nanometers.
-        Default 500nm.
+        The wavelength of the DIMM-delivered equivalent FWHM, in
+        nanometers. Default 500nm.
     efd_seeing : `str`, opt
-        The name of the DIMM FWHM measurements in the efd / conditions object.
-        Default `FWHM_500`
+        The name of the DIMM FWHM measurements in the efd /
+        conditions object. Default `FWHM_500`
     """
 
     def __init__(
         self,
         filter_list=["u", "g", "r", "i", "z", "y"],
         eff_wavelens=None,
         telescope_seeing=0.25,
@@ -64,56 +68,63 @@
         self._set_fwhm_zenith_system()
 
     def configure(self):
         """Deprecated. Configure through the init method."""
         warnings.warn("the configure method is deprecated")
 
     def config_info(self):
-        """Deprecated. Report configuration parameters and version information."""
+        """Deprecated. Report configuration parameters and version
+        information."""
         warnings.warn("the config_info method is deprecated.")
 
     def _set_fwhm_zenith_system(self):
         """Calculate the system contribution to FWHM at zenith.
 
-        This is simply the individual telescope, optics, and camera contributions
-        combined in quadrature.
+        This is simply the individual telescope, optics, and camera
+        contributions combined in quadrature.
         """
         self.fwhm_system_zenith = np.sqrt(
             self.telescope_seeing**2 + self.optical_design_seeing**2 + self.camera_seeing**2
         )
 
     def __call__(self, fwhm_z, airmass):
-        """Calculate the seeing values FWHM_eff and FWHM_geom at the given airmasses,
-        for the specified effective wavelengths, given FWHM_zenith (typically FWHM_500).
-
-        FWHM_geom represents the geometric size of the PSF; FWHM_eff represents the FWHM of a
-        single gaussian which encloses the same number of pixels as N_eff (the number of pixels
-        enclosed in the actual PSF -- this is the value to use when calculating SNR).
+        """Calculate the seeing values FWHM_eff and FWHM_geom at the
+        given airmasses, for the specified effective wavelengths, given
+        FWHM_zenith (typically FWHM_500).
+
+        FWHM_geom represents the geometric size of the PSF; FWHM_eff
+        represents the FWHM of a single gaussian which encloses the
+        same number of pixels as N_eff (the number of pixels enclosed
+        in the actual PSF -- this is the value to use when calculating
+        SNR).
 
         FWHM_geom(") = 0.822 * FWHM_eff(") + 0.052"
 
-        The FWHM_eff includes a contribution from the system and from the atmosphere.
-        Both of these are expected to scale with airmass^0.6 and with (500(nm)/wavelength(nm))^0.3.
+        The FWHM_eff includes a contribution from the system and from
+        the atmosphere.  Both of these are expected to scale with
+        airmass^0.6 and with (500(nm)/wavelength(nm))^0.3.
         FWHM_eff = 1.16 * sqrt(FWHM_sys**2 + 1.04*FWHM_atm**2)
 
         Parameters
         ----------
         fwhm_z: `float`, or efdData `dict`
             FWHM at zenith (arcsec).
         airmass: `float`, `np.array`, or targetDict `dict`
             Airmass (unitless).
 
         Returns
         -------
         FWHMeff, FWHMGeom : `dict` of {`numpy.ndarray`, `numpy.ndarray`}
             FWHMeff, FWHMgeom: both are the same shape numpy.ndarray.
-            If airmass is a single value, FWHMeff & FWHMgeom are 1-d arrays,
-            with the same order as eff_wavelen (i.e. eff_wavelen[0] = u, then FWHMeff[0] = u).
-            If airmass is a numpy array, FWHMeff and FWHMgeom are 2-d arrays,
-            in the order of <filter><airmass> (i.e. eff_wavelen[0] = u, 1-d array over airmass range).
+            If airmass is a single value, FWHMeff & FWHMgeom are 1-d
+            arrays, with the same order as eff_wavelen (i.e.
+            eff_wavelen[0] = u, then FWHMeff[0] = u). If airmass is a
+            numpy array, FWHMeff and FWHMgeom are 2-d arrays, in the
+            order of <filter><airmass> (i.e. eff_wavelen[0] = u, 1-d
+            array over airmass range).
         """
         if isinstance(fwhm_z, dict):
             fwhm_z = fwhm_z[self.efd_seeing]
         if isinstance(airmass, dict):
             airmass = airmass["airmass"]
         airmass_correction = np.power(airmass, 0.6)
         wavelen_correction = np.power(self.raw_seeing_wavelength / self.eff_wavelens, 0.3)
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/unscheduled_downtime_data.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/unscheduled_downtime_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,24 @@
 class UnscheduledDowntimeData:
     """Handle (and create) the unscheduled downtime information.
 
     Parameters
     ----------
     start_time : `astropy.time.Time`
         The time of the start of the simulation.
-        The cloud database will be assumed to start on Jan 01 of the same year.
+        The cloud database will be assumed to start on Jan 01 of the
+        same year.
     seed : `int`, optional
-        The random seed for creating the random nights of unscheduled downtime. Default 1516231120.
+        The random seed for creating the random nights of unscheduled
+        downtime. Default 1516231120.
     start_of_night_offset : `float`, optional
-        The fraction of a day to offset from MJD.0 to reach the defined start of a night ('noon' works).
-        Default 0.16 (UTC midnight in Chile) - 0.5 (minus half a day) = -0.34
+        The fraction of a day to offset from MJD.0 to reach the
+        defined start of a night ('noon' works).
+        Default 0.16 (UTC midnight in Chile) - 0.5
+        (minus half a day) = -0.34
     survey_length : `int`, optional
         The number of nights in the total survey. Default 3650*2.
     """
 
     MINOR_EVENT = {"P": 0.0137, "length": 1, "level": "minor event"}
     INTERMEDIATE_EVENT = {"P": 0.00548, "length": 3, "level": "intermediate event"}
     MAJOR_EVENT = {"P": 0.00137, "length": 7, "level": "major event"}
@@ -38,31 +42,33 @@
         self.seed = seed
         self.survey_length = survey_length
         year_start = start_time.datetime.year
         self.night0 = Time("%d-01-01" % year_start, format="isot", scale="tai") + TimeDelta(
             start_of_night_offset, format="jd"
         )
 
-        # Scheduled downtime data is a np.ndarray of start / end / activity for each scheduled downtime.
+        # Scheduled downtime data is a np.ndarray of start
+        # / end / activity for each scheduled downtime.
         self.downtime = None
         self.make_data()
 
     def __call__(self):
         """Return the array of unscheduled downtimes.
 
         Parameters
         ----------
         time : `astropy.time.Time`
             Time in the simulation for which to find the current downtime.
 
         Returns
         -------
         downtime : `np.ndarray`
-            The array of all unscheduled downtimes, with keys for 'start', 'end', 'activity',
-            corresponding to `astropy.time.Time`, `astropy.time.Time`, and `str`.
+            The array of all unscheduled downtimes, with keys for
+            'start', 'end', 'activity',  corresponding to
+            `astropy.time.Time`, `astropy.time.Time`, and `str`.
         """
         return self.downtime
 
     def _downtime_status(self, time):
         """Look behind the scenes at the downtime status/next values"""
         next_start = self.downtime["start"].searchsorted(time, side="right")
         next_end = self.downtime["end"].searchsorted(time, side="right")
@@ -72,21 +78,24 @@
             current = None
         future = self.downtime[next_start:]
         return current, future
 
     def make_data(self):
         """Configure the set of unscheduled downtimes.
 
-        This function creates the unscheduled downtimes based on a set of probabilities
-        of the downtime type occurance.
+        This function creates the unscheduled downtimes based on a set
+        of probabilities of the downtime type occurance.
 
-        The random downtime is calculated using the following probabilities:
+        The random downtime is calculated using the following
+        probabilities:
 
-        minor event : remainder of night and next day = 5/365 days e.g. power supply failure
-        intermediate : 3 nights = 2/365 days e.g. repair filter mechanism, rotator, hexapod, or shutter
+        minor event : remainder of night and next day = 5/365 days
+        e.g. power supply failure
+        intermediate : 3 nights = 2/365 days e.g. repair filter
+        mechanism, rotator, hexapod, or shutter
         major event : 7 nights = 1/2*365 days
         catastrophic event : 14 nights = 1/3650 days e.g. replace a raft
         """
         random.seed(self.seed)
 
         starts = []
         ends = []
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/site_models/wind_data.py` & `rubin_scheduler-1.2.0/rubin_scheduler/site_models/wind_data.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/skybrightness_pre/dark_sky.py` & `rubin_scheduler-1.2.0/rubin_scheduler/skybrightness_pre/dark_sky.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/skybrightness_pre/data/generate_dark_sky.py` & `rubin_scheduler-1.2.0/rubin_scheduler/skybrightness_pre/data/generate_dark_sky.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 import h5py
 import numpy as np
 
 from rubin_scheduler.data import get_data_dir
 
 if __name__ == "__main__":
-    # Gererate an sky map for each filters that is an estimate of how faint that part of sky
-    # can get
+    # Gererate an sky map for each filters that is an estimate of
+    # how faint that part of sky can get
 
     data_dir = get_data_dir()
 
     sky_files = glob.glob(os.path.join(data_dir, "skybrightness_pre/*.h5"))
 
     maximum_maps = {}
     filternames = "ugrizy"
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/skybrightness_pre/sky_model_pre.py` & `rubin_scheduler-1.2.0/rubin_scheduler/skybrightness_pre/sky_model_pre.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 import warnings
 from pathlib import Path
 
 import h5py
 import healpy as hp
 import numpy as np
 import requests
+from astropy import units as u
+from astropy.coordinates import AltAz, EarthLocation, SkyCoord, get_sun
+from astropy.time import Time
 
 import rubin_scheduler.data.rs_download_sky
 from rubin_scheduler.data import get_data_dir
-from rubin_scheduler.utils import _angular_separation, _hpid2_ra_dec, survey_start_mjd
+from rubin_scheduler.utils import Site, _angular_separation, _hpid2_ra_dec, survey_start_mjd
 
 try:
     from lsst.resources import ResourcePath
 except ImportError:
     pass
 
 
@@ -29,16 +32,16 @@
     max_angle = 2.0 * np.pi
     da = (a1 - a0) % max_angle
     return 2.0 * da % max_angle - da
 
 
 def interp_angle(x_out, xp, anglep, degrees=False):
     """
-    Interpolate angle values (handle wrap around properly). Does nearest neighbor
-    interpolation if values out of range.
+    Interpolate angle values (handle wrap around properly).
+    Does nearest neighbor interpolation if values out of range.
 
     Parameters
     ----------
     x_out : `float` or array
         The points to interpolate to.
     xp : array
         Points to interpolate between (must be sorted)
@@ -69,44 +72,90 @@
         result = np.degrees(result)
     else:
         result = anglep[left] + short_angle_dist(anglep[left], anglep[right]) * wterm
         result = result % (2.0 * np.pi)
     return result
 
 
+def simple_daytime(sky_alt, sky_az, sun_alt, sun_az, filter_name="r", bright_val=2.0, sky_alt_min=20.0):
+    """A simple function to return a sky brightness map when the sun is up
+
+    Parameters
+    ----------
+    sky_alt : `float`
+        Altitude of poistion(s) on the sky. Degrees.
+    sky_az : `float`
+        Azimuth of poistion(s) on the sky. Degrees.
+    sun_alt : `float`
+        Altitude of the sun. Degrees.
+    sun_az : `float`
+        Azimuth of the sun. Degrees.
+    filter_name : `str`
+        Name of the filter, default "r". Currently unused, but
+        could be useful in the future if a more complicated function
+        gets subbed in.
+    bright_val : `float`
+        The value to plug into the sky. Default 2 mag/sq arcsec.
+    sky_alt_min : `float`
+        Set all sky below the alt limit to NaN. Default 20 degrees.
+    """
+
+    result = np.full_like(sky_alt, np.nan)
+    result[np.where(sky_alt > sky_alt_min)] = bright_val
+    return result
+
+
 class SkyModelPreBase(abc.ABC):
     """Load pre-computed sky brighntess maps for the LSST site
     and use them to interpolate to arbitrary dates.
 
     Parameters
     ----------
     data_path : `str`, opt
-        path to the numpy save files. Looks in standard SIMS_SKYBRIGHTNESS_DATA or RUBIN_SIM_DATA_DIR
-        if set to default (None).
+        path to the numpy save files. Looks in standard
+        SIMS_SKYBRIGHTNESS_DATA or RUBIN_SIM_DATA_DIR if set to
+        default (None).
     init_load_length : `int` (10)
-        The length of time (days) to load from disk initially. Set to something small for fast reads.
+        The length of time (days) to load from disk initially.
+        Set to something small for fast reads.
     load_length : `int` (365)
         The number of days to load after the initial load.
     mjd0 : `float` (None)
-        The starting MJD to load on initilization (days). Uses util to lookup default if None.
+        The starting MJD to load on initilization (days). Uses
+        util to lookup default if None.
+    location : `astropy.EarthLocation`
+        The location of the telescope. Default of None will load
+        Rubin position.
+    sun_alt_limit : `float`
+            The altitude limit to use a "bright" sky function. Default
+            of -8 degrees
     """
 
     def __init__(
         self,
         data_path=None,
         init_load_length=10,
         load_length=365,
         verbose=False,
         mjd0=None,
+        location=None,
+        sun_alt_limit=-8.0,
     ):
         self.info = None
         self.sb = None
         self.header = None
         self.filter_names = None
         self.verbose = verbose
+        self.sun_alt_limit = np.radians(sun_alt_limit)
+
+        if location is None:
+            site = Site("LSST")
+            self.location = EarthLocation(lat=site.latitude, lon=site.longitude, height=site.height)
+        else:
+            self.location = location
 
         # Look in default location for .npz files to load
         if data_path is not None:
             self.data_path = data_path
         elif "SIMS_SKYBRIGHTNESS_DATA" in os.environ:
             self.data_path = os.environ["SIMS_SKYBRIGHTNESS_DATA"]
         else:
@@ -135,46 +184,49 @@
             self.load_length = init_load_length
             self._load_data(mjd0)
         # swap back to the longer load length
         self.load_length = load_length
         self.nside = 32
         hpid = np.arange(hp.nside2npix(self.nside))
         self.ra, self.dec = _hpid2_ra_dec(self.nside, hpid)
+        self.skycoord = SkyCoord(ra=self.ra * u.rad, dec=self.dec * u.rad)
 
     def _load_data(self, mjd, filename=None, npyfile=None):
         """Load up the h5 file to interpolate things.
 
         Parameters
         ----------
         mjd : `float`
             The Modified Julian Date that we want to load
         filename : `str` (None)
-            The filename to restore. If None, it checks the filenames on disk to find one that
-            should have the requested MJD
+            The filename to restore. If None, it checks the filenames
+            on disk to find one that should have the requested MJD
         npyfile : `str` (None)
-            If sky brightness data not in npz file, checks the .npy file with same root name.
+            If sky brightness data not in npz file, checks the .npy
+            file with same root name.
         """
 
         if filename is None:
             # Figure out which file to load.
             file_indx = np.where((mjd >= self.mjd_left) & (mjd <= self.mjd_right))[0]
             if np.size(file_indx) == 0:
                 raise ValueError(
                     "MJD = %f is out of range for the files found (%f-%f)"
                     % (mjd, self.mjd_left.min(), self.mjd_right.max())
                 )
-            # Just take the later one, assuming we're probably simulating forward in time
+            # Just take the later one, assuming we're probably
+            # simulating forward in time
             file_indx = np.max(file_indx)
 
             filename = self.files[file_indx]
         else:
             self.loaded_range = None
 
-        # Use three separate try/excepet blocks so that if any of them throw
-        # exceptions, we still get the others.
+        # Use three separate try/excepet blocks so that if any of
+        # them throw exceptions, we still get the others.
         try:
             del self.sb
         except AttributeError:
             pass
 
         try:
             del self.filter_names
@@ -220,38 +272,39 @@
         """Return a full sky map or individual pixels for the input mjd.
 
         Parameters
         ----------
         mjd : `float`
             Modified Julian Date to interpolate to
         indx : `List` of `int` (None)
-            indices to interpolate the sky values at. Returns full sky if None. If the class was
-            instatiated with opsimFields, indx is the field ID, otherwise it is the healpix ID.
+            indices to interpolate the sky values at. Returns full sky
+            if None. If the class was instatiated with opsimFields,
+            indx is the field ID, otherwise it is the healpix ID.
         airmass_mask : `bool` (True)
             Set high (>2.5) airmass pixels to badval.
         planet_mask : `bool` (True)
             Set sky maps to badval near (2 degrees) bright planets.
         moon_mask : `bool` (True)
             Set sky maps near (10 degrees) the moon to badval.
         zenith_mask : `bool` (True)
             Set sky maps at high altitude (>86.5) to badval.
         badval : `float` (-1.6375e30)
             Mask value. Defaults to the healpy mask value.
         filters : `list`, opt
             List of strings for the filters that should be returned.
             Default returns ugrizy.
         extrapolate : `bool` (False)
-            In indx is set, extrapolate any masked pixels to be the same as the nearest non-masked
-            value from the full sky map.
+            In indx is set, extrapolate any masked pixels to be the
+            same as the nearest non-masked value from the full sky map.
 
         Returns
         -------
         sbs : `dict`
-            A dictionary with filter names as keys and np.arrays as values which
-            hold the sky brightness maps in mag/sq arcsec.
+            A dictionary with filter names as keys and np.arrays as
+            values which hold the sky brightness maps in mag/sq arcsec.
         """
         if mjd < self.loaded_range.min() or (mjd > self.loaded_range.max()):
             self._load_data(mjd)
 
         left = np.searchsorted(self.mjds, mjd) - 1
         right = left + 1
 
@@ -270,22 +323,44 @@
             left += 1
             baseline = 1.0
         else:
             baseline = self.mjds[right] - self.mjds[left]
 
         # Check if we are between sunrise/set
         if baseline > self.timestep_max + 1e-6:
-            warnings.warn("Requested MJD between sunrise and sunset, returning closest maps")
-            diff = np.abs(self.mjds[left.max() : right.max() + 1] - mjd)
-            closest_indx = np.array([left, right])[np.where(diff == np.min(diff))].min()
-            sbs = {}
-            for filter_name in filters:
-                sbs[filter_name] = self.sb[filter_name][closest_indx, indx]
-                sbs[filter_name][np.isinf(sbs[filter_name])] = badval
-                sbs[filter_name][np.where(sbs[filter_name] == hp.UNSEEN)] = badval
+
+            # Check if sun is really high:
+            obstime = Time(mjd, format="mjd")
+            sun = get_sun(obstime)
+            aa = AltAz(location=self.location, obstime=obstime)
+            sun_alt_az = sun.transform_to(aa)
+
+            if sun_alt_az.alt.rad > self.sun_alt_limit:
+                warnings.warn("Sun high, using bright sky approx")
+                hp_aa = self.skycoord.transform_to(aa)
+
+                sbs = {}
+                for filter_name in filters:
+                    sbs[filter_name] = simple_daytime(
+                        hp_aa.alt.deg,
+                        hp_aa.az.deg,
+                        sun_alt_az.alt.deg,
+                        sun_alt_az.az.deg,
+                        filter_name=filter_name,
+                    )
+
+            else:
+                warnings.warn("Requested MJD between sunrise and sunset, returning closest maps")
+                diff = np.abs(self.mjds[left.max() : right.max() + 1] - mjd)
+                closest_indx = np.array([left, right])[np.where(diff == np.min(diff))].min()
+                sbs = {}
+                for filter_name in filters:
+                    sbs[filter_name] = self.sb[filter_name][closest_indx, indx]
+                    sbs[filter_name][np.isinf(sbs[filter_name])] = badval
+                    sbs[filter_name][np.where(sbs[filter_name] == hp.UNSEEN)] = badval
         else:
             wterm = (mjd - self.mjds[left]) / baseline
             w1 = 1.0 - wterm
             w2 = wterm
             sbs = {}
             for filter_name in filters:
                 sbs[filter_name] = (
@@ -294,30 +369,32 @@
         # If requested a certain pixel(s), and want to extrapolate.
         if (not full_sky) & extrapolate:
             masked_pix = False
             for filter_name in filters:
                 if (badval in sbs[filter_name]) | (True in np.isnan(sbs[filter_name])):
                     masked_pix = True
             if masked_pix:
-                # We have pixels that are masked that we want reasonable values for
+                # We have pixels that are masked that we want
+                # reasonable values for
                 full_sky_sb = self.return_mags(
                     mjd,
                     filters=filters,
                 )
                 good = np.where((full_sky_sb[filters[0]] != badval) & ~np.isnan(full_sky_sb[filters[0]]))[0]
-                ra_full = self.ra[good]  # np.radians(self.header["ra"][good])
-                dec_full = self.dec[good]  # np.radians(self.header["dec"][good])
+                ra_full = self.ra[good]
+                dec_full = self.dec[good]
                 for filtername in filters:
                     full_sky_sb[filtername] = full_sky_sb[filtername][good]
                 # Going to assume the masked pixels are the same in all filters
                 masked_indx = np.where(
                     (sbs[filters[0]].ravel() == badval) | np.isnan(sbs[filters[0]].ravel())
                 )[0]
                 for i, mi in enumerate(masked_indx):
-                    # Note, this is going to be really slow for many pixels, should use a kdtree
+                    # Note, this is going to be really slow for many
+                    # pixels, should use a kdtree
                     dist = _angular_separation(
                         self.ra[indx[i]],
                         self.dec[indx[i]],
                         ra_full,
                         dec_full,
                     )
                     closest = np.where(dist == dist.min())[0]
@@ -371,17 +448,18 @@
 class SkyModelPreWithResources(SkyModelPreBase):
     def _init_files(self):
         data_resource = ResourcePath(self.data_path, forceDirectory=True)
 
         try:
             self.files = list(ResourcePath.findFileResources([data_resource], file_filter=r".*\.h5"))
         except NotImplementedError:
-            # lsst.requests does not implement walk for plain html, so do it manually here.
-            # Unlike the method above, however, this simple approach does not
-            # descend into subdirectories.
+            # lsst.requests does not implement walk for plain html,
+            # so do it manually here.
+            # Unlike the method above, however, this simple approach
+            # does not descend into subdirectories.
             self.files = []
             if urllib.parse.urlparse(data_resource.geturl()).scheme in ("http", "https"):
                 request_content = requests.get(data_resource.geturl()).text
                 html_parser = rubin_scheduler.data.rs_download_sky.MyHTMLParser()
                 html_parser.feed(request_content)
                 html_parser.close()
                 for file_name in html_parser.filenames:
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/__init__.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,13 +7,14 @@
 from .file_maps import *
 from .get_package_dir import *
 from .healpy_utils import *
 from .htm_module import *
 from .m5_flat_sed import *
 from .mjd_zero import *
 from .projections import *
+from .rotskypos import *
 from .sampling_functions import *
 from .season_utils import *
 from .site import *
 from .sys_eng_vals import *
 from .tree_utils import *
 from .zernike_module import *
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/approx_coord_transforms.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/approx_coord_transforms.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import numpy as np
 
 from .coordinate_transformations import calc_lmst
 
 
 def _approx_altaz2pa(alt_rad, az_rad, latitude_rad):
-    """A fast calculation of parallactic angle
+    """A fast calculation of parallactic angle.
 
     Parameters
     ----------
     alt_rad : `float`
         Altitude (radians)
     az_rad : `float`
         Azimuth (radians)
@@ -35,15 +35,15 @@
     pa = np.arctan2(y, x)
     # Make it run from 0-360 deg instead of of -180 to 180
     pa = pa % (2.0 * np.pi)
     return pa
 
 
 def approx_altaz2pa(alt_deg, az_deg, latitude_deg):
-    """A fast calculation of parallactic angle
+    """A fast calculation of parallactic angle.
 
     Parameters
     ----------
     alt_rad : `float`
         Altitude (degrees)
     az_rad : `float`
         Azimuth (degrees)
@@ -56,22 +56,24 @@
         Parallactic angle (degrees)
     """
     pa = _approx_altaz2pa(np.radians(alt_deg), np.radians(az_deg), np.radians(latitude_deg))
     return np.degrees(pa)
 
 
 def approx_alt_az2_ra_dec(alt, az, lat, lon, mjd, lmst=None):
-    """Convert alt, az to RA, Dec without taking into account aberration, precession, diffraction, etc.
+    """Convert alt, az to RA, Dec without taking into account aberration,
+    precession, diffraction, etc.
 
     Parameters
     ----------
     alt : numpy.array
         Altitude, same length as `ra` and `dec`. Degrees.
     az : numpy.array
-        Azimuth, same length as `ra` and `dec`. Must be same length as `alt`. Degrees.
+        Azimuth, same length as `ra` and `dec`. Must be same length
+        as `alt`. Degrees.
     lat : float
         Latitude of the observatory in degrees.
     lon : float
         Longitude of the observatory in degrees.
     mjd : float
         Modified Julian Date.
     lmst : float (None)
@@ -92,23 +94,24 @@
         mjd,
         lmst=lmst,
     )
     return np.degrees(ra), np.degrees(dec)
 
 
 def _approx_alt_az2_ra_dec(alt, az, lat, lon, mjd, lmst=None):
-    """
-    Convert alt, az to RA, Dec without taking into account aberration, precession, diffraction, etc.
+    """Convert alt, az to RA, Dec without taking into account aberration,
+    precession, diffraction, etc.
 
     Parameters
     ----------
     alt : numpy.array
         Altitude, same length as `ra` and `dec`. Radians.
     az : numpy.array
-        Azimuth, same length as `ra` and `dec`. Must be same length as `alt`. Radians.
+        Azimuth, same length as `ra` and `dec`. Must be same length
+        as `alt`. Radians.
     lat : float
         Latitude of the observatory in radians.
     lon : float
         Longitude of the observatory in radians.
     mjd : float
         Modified Julian Date.
     lmst : float (None)
@@ -136,19 +139,19 @@
     ra[raneg] = ra[raneg] + 2.0 * np.pi
     raover = np.where(ra > 2.0 * np.pi)
     ra[raover] -= 2.0 * np.pi
     return ra, dec
 
 
 def approx_ra_dec2_alt_az(ra, dec, lat, lon, mjd, lmst=None):
-    """
-    Convert Ra,Dec to Altitude and Azimuth.
+    """Convert Ra,Dec to Altitude and Azimuth.
 
-    Coordinate transformation is killing performance. Just use simple equations to speed it up
-    and ignore aberration, precession, nutation, nutrition, etc.
+    Coordinate transformation is killing performance. Just use
+    simple equations to speed it up and ignore aberration, precession,
+    nutation, nutrition, etc.
 
     Parameters
     ----------
     ra : array_like
         RA, in degrees.
     dec : array_like
         Dec, in degrees. Must be same length as `ra`.
@@ -176,19 +179,19 @@
         mjd,
         lmst=lmst,
     )
     return np.degrees(alt), np.degrees(az)
 
 
 def _approx_ra_dec2_alt_az(ra, dec, lat, lon, mjd, lmst=None, return_pa=False):
-    """
-    Convert Ra,Dec to Altitude and Azimuth.
+    """Convert Ra,Dec to Altitude and Azimuth.
 
-    Coordinate transformation is killing performance. Just use simple equations to speed it up
-    and ignore aberration, precession, nutation, nutrition, etc.
+    Coordinate transformation is killing performance. Just use
+    simple equations to speed it up and ignore aberration,
+    precession, nutation, nutrition, etc.
 
     Parameters
     ----------
     ra : array_like
         RA, in radians.
     dec : array_like
         Dec, in radians. Must be same length as `ra`.
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/bearing.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/bearing.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/binned_stats.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/binned_stats.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/camera_footprint.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/camera_footprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,20 @@
     """
     Identify point on the sky within an LSST camera footprint.
 
     Parameters
     ----------
     units : `str`, opt
         Units for the object RA/Dec and boresight RA/Dec/rotation values.
-        Default 'degrees'.  If not degrees, assumes incoming values are in radians.
+        Default 'degrees'.  If not degrees, assumes incoming values
+        are in radians.
     footprint_file : `str` or None, opt
         Location for the camera footprint map.
-        Default None loads the default map from $RUBIN_SIM_DATA_DIR/maf/fov_map.npz
+        Default None loads the default map from
+        $RUBIN_SIM_DATA_DIR/maf/fov_map.npz
 
     """
 
     def __init__(self, units="degrees", footprint_file=None):
         if footprint_file is None:
             footprint_file = os.path.join(get_data_dir(), "utils", "fov_map.npz")
         _temp = np.load(footprint_file)
@@ -43,15 +45,16 @@
         self.camera_fov = _temp["image"].copy()
         self.x_camera = np.radians(_temp["x"].copy())
         _temp.close()
         self.plate_scale = self.x_camera[1] - self.x_camera[0]
         self.indx_max = len(self.x_camera)
 
     def __call__(self, obj_ra, obj_dec, boresight_ra, boresight_dec, boresight_rot_sky_pos):
-        """Determine which observations are within the actual camera footprint for a series of observations.
+        """Determine which observations are within the actual camera
+        footprint for a series of observations.
 
         Parameters
         ----------
         obj_ra : `np.ndarray`
             RA values for the objects (in the field of view?)
         obj_dec : `np.ndarray`
             Dec values for the objects
@@ -61,29 +64,30 @@
             Dec value for the pointing
         boresight_rot_sky_pos : `float`
             RotSkyPos value for the pointing.
 
         Returns
         -------
         indices : `np.ndarray`
-            Returns the indexes of the numpy array of the object observations
-            which are inside the fov and land on a science chip.
-            Applying this to the input array (e.g. obj_ra[indices]) indicates the positions of
+            Returns the indexes of the numpy array of the object
+            observations which are inside the fov and land on a
+            science chip. Applying this to the input array
+            (e.g. obj_ra[indices]) indicates the positions of
             the objects which fell onto active silicon.
         """
         if self.units == "degrees":
             x_proj, y_proj = gnomonic_project_toxy(
                 np.radians(obj_ra),
                 np.radians(obj_dec),
                 np.radians(boresight_ra),
                 np.radians(boresight_dec),
             )
             # rotate them by rotskypos
-            # TODO: look up whether this is a positive or negative rotation
-            #  in the observatory documentation
+            # TODO: look up whether this is a positive or
+            # negative rotation in the observatory documentation
             x_proj, y_proj = rotate(x_proj, y_proj, np.radians(boresight_rot_sky_pos))
 
         else:
             x_proj, y_proj = gnomonic_project_toxy(obj_ra, obj_dec, boresight_ra, boresight_dec)
             x_proj, y_proj = rotate(x_proj, y_proj, boresight_rot_sky_pos)
 
         # look up which points are good
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/code_utilities.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/code_utilities.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/ddf_locations.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/ddf_locations.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/file_maps.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/file_maps.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/healpy_utils.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/healpy_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,29 +104,30 @@
         Healpixel IDs for the input positions.
     """
     return _ra_dec2_hpid(nside, np.radians(ra), np.radians(dec), **kwargs)
 
 
 def _healbin(ra, dec, values, nside=128, reduce_func=np.mean, dtype=float, fill_val=hp.UNSEEN):
     """
-    Take arrays of ra's, dec's, and value and bin into healpixels. Like numpy.hexbin but for
-    bins on a sphere.
+    Take arrays of ra's, dec's, and value and bin into healpixels.
+    Like numpy.hexbin but for bins on a sphere.
 
     Parameters
     ----------
     ra : np.array
         RA positions of the data points. Radians.
     dec : np.array
         Dec positions of the data points. Radians
     values : np.array
         The values at each ra,dec position.
     nside : int
         Healpixel nside resolution. Must be a value of 2^N.
     reduce_func : function (numpy.mean)
-        A function that will return a single value given a subset of `values`.
+        A function that will return a single value given a subset of
+        `values`.
     dtype : dtype ('float')
         Data type of the resulting mask
     fill_val : float (hp.UNSEEN)
         Value to fill in with healpixels that have no value.
         Default is the healpy mask value.
 
     Returns
@@ -143,41 +144,43 @@
     pixids = np.unique(hpids)
 
     left = np.searchsorted(hpids, pixids)
     right = np.searchsorted(hpids, pixids, side="right")
 
     map_vals = np.zeros(hp.nside2npix(nside), dtype=dtype) + fill_val
 
-    # Wow, I thought histogram would be faster than the loop, but this has been faster!
+    # Wow, I thought histogram would be faster than the loop, but
+    # this has been faster!
     for i, idx in enumerate(pixids):
         map_vals[idx] = reduce_func(values[left[i] : right[i]])
 
     # Change any NaNs to fill value
     map_vals[np.isnan(map_vals)] = fill_val
 
     return map_vals
 
 
 def healbin(ra, dec, values, nside=128, reduce_func=np.mean, dtype=float, fill_val=hp.UNSEEN):
     """
-    Take arrays of ra's, dec's, and value and bin into healpixels. Like numpy.hexbin but for
-    bins on a sphere.
+    Take arrays of ra's, dec's, and value and bin into healpixels.
+    Like numpy.hexbin but for bins on a sphere.
 
     Parameters
     ----------
     ra : np.array
         RA positions of the data points. Degrees.
     dec : np.array
         Dec positions of the data points. Degrees.
     values : np.array
         The values at each ra,dec position.
     nside : int
         Healpixel nside resolution. Must be a value of 2^N.
     reduce_func : function (numpy.mean)
-        A function that will return a single value given a subset of `values`.
+        A function that will return a single value given a subset
+        of `values`.
     dtype : dtype ('float')
         Data type of the resulting mask
     fill_val : float (hp.UNSEEN)
         Value to fill in with healpixels that have no value.
         Default is the healpy mask value.
 
     Returns
@@ -193,44 +196,50 @@
         reduce_func=reduce_func,
         dtype=dtype,
         fill_val=fill_val,
     )
 
 
 def moc2array(data, uniq, nside=128, reduce_func=np.sum, density=True, fill_val=0.0):
-    """Convert a Multi-Order Coverage Map to a single nside HEALPix array. Useful
-    for converting maps output by LIGO alerts. Expect that future versions of
-    healpy or astropy will be able to replace this functionality. Note that this is
-    a convienence function that will probably degrade portions of the MOC that are
-    sampled at high resolution.
+    """Convert a Multi-Order Coverage Map to a single nside HEALPix
+    array. Useful for converting maps output by LIGO alerts. Expect
+    that future versions of healpy or astropy will be able to replace
+    this functionality. Note that this is a convienence function that
+    will probably degrade portions of the MOC that are sampled at high
+    resolution.
 
-    Details of HEALPix Mulit-Order Coverage map: http://ivoa.net/documents/MOC/20190404/PR-MOC-1.1-20190404.pdf
+    Details of HEALPix Mulit-Order Coverage map:
+    http://ivoa.net/documents/MOC/20190404/PR-MOC-1.1-20190404.pdf
 
     Parameters
     ----------
     data : np.array
         Data values for the MOC map
     uniq : np.array
         The UNIQ values for the MOC map
     nside : int (128)
         The output map nside
     reduce_func : function (np.sum)
         The function to use to combine data into single healpixels.
     density : bool (True)
-        If True, multiplies data values by pixel area before applying reduce_func, and divides
-        the final array by the output pixel area. Should be True if working on a probability density MOC.
+        If True, multiplies data values by pixel area before applying
+        reduce_func, and divides the final array by the output pixel
+        area. Should be True if working on a probability density MOC.
     fill_val : float (0.)
-        Value to fill empty HEALPixels with. Good choices include 0 (default), hp.UNSEEN, and np.nan.
+        Value to fill empty HEALPixels with. Good choices include
+        0 (default), hp.UNSEEN, and np.nan.
 
     Returns
     -------
-    np.array : HEALpy array of nside. Units should be the same as the input map as processed by reduce_func.
+    np.array : HEALpy array of nside. Units should be the same as
+        the input map as processed by reduce_func.
     """
 
-    # NUNIQ packing, from page 12 of http://ivoa.net/documents/MOC/20190404/PR-MOC-1.1-20190404.pdf
+    # NUNIQ packing, from page 12 of
+    # http://ivoa.net/documents/MOC/20190404/PR-MOC-1.1-20190404.pdf
     orders = np.floor(np.log2(uniq / 4) / 2).astype(int)
     npixs = (uniq - 4 * 4**orders).astype(int)
 
     nsides = 2**orders
     names = ["ra", "dec", "area"]
     types = [float] * len(names)
     data_points = np.zeros(data.size, dtype=list(zip(names, types)))
@@ -292,16 +301,17 @@
     else:
         nside_match = False
 
     # If we already have neighbors chached, just use it
     if nside_match:
         neighbors = hp_grow_argsort.neighbors_cache
     else:
-        # Running a new nside, or for the first time, compute neighbors and set attributes
-        # Make a `bool` area to keep track of which pixels still need to be sorted
+        # Running a new nside, or for the first time, compute
+        # neighbors and set attributes Make a `bool` area to keep
+        # track of which pixels still need to be sorted
         neighbors = hp.get_all_neighbours(nside, pix_indx).T
         hp_grow_argsort.neighbors_cache = neighbors
         hp_grow_argsort.nside = nside
 
     valid_neighbors_mask = np.ones(neighbors.shape, dtype=bool)
 
     # Sometimes there can be no neighbors in some directions
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/htm_module.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/htm_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 This module implements utilities to convert between RA, Dec and indexes
-on the Hierarchical Triangular Mesh (HTM), a system of tiling the unit sphere
-with nested triangles.  The HTM is described in these references
+on the Hierarchical Triangular Mesh (HTM), a system of tiling the
+unit sphere with nested triangles.  The HTM is described in these
+references
 
 Kunszt P., Szalay A., Thakar A. (2006) in "Mining The Sky",
 Banday A, Zaroubi S, Bartelmann M. eds.
 ESO Astrophysics Symposia
-https://www.researchgate.net/publication/226072008_The_Hierarchical_Triangular_Mesh
+https://www.researchgate.net/publication/
+226072008_The_Hierarchical_Triangular_Mesh
 
 Szalay A. et al. (2007)
 "Indexing the Sphere with the Hierarchical Triangular Mesh"
 arXiv:cs/0701164
 """
 
 __all__ = (
@@ -34,18 +36,18 @@
 
 
 class Trixel:
     """
     A trixel is a single triangle in the Hierarchical Triangular Mesh (HTM)
     tiling scheme.  It is defined by its three corners on the unit sphere.
 
-    Instantiating this class directly is a bad idea. __init__() does nothing
-    to ensure that the parameters you give it are self-consistent.  Instead,
-    use the trixel_from_htmid() or get_all_trixels() methods in this module
-    to instantiate trixels.
+    Instantiating this class directly is a bad idea. __init__() does
+    nothing to ensure that the parameters you give it are
+    self-consistent.  Instead, use the trixel_from_htmid() or
+    get_all_trixels() methods in this module to instantiate trixels.
     """
 
     def __init__(self, present_htmid, present_corners):
         """
         Initialize the current Trixel
 
         Parameters
@@ -141,15 +143,16 @@
         is contained within this trixel; False if not.
 
         See equation 5 of
 
         Kunszt P., Szalay A., Thakar A. (2006) in "Mining The Sky",
         Banday A, Zaroubi S, Bartelmann M. eds.
         ESO Astrophysics Symposia
-        https://www.researchgate.net/publication/226072008_The_Hierarchical_Triangular_Mesh
+        https://www.researchgate.net/publication/
+        226072008_The_Hierarchical_Triangular_Mesh
         """
         if np.dot(self.cross01, pt) >= 0.0:
             if np.dot(self.cross12, pt) >= 0.0:
                 if np.dot(self.cross20, pt) >= 0.0:
                     return True
 
         return False
@@ -165,15 +168,16 @@
         within this trixel.
 
         See equation 5 of
 
         Kunszt P., Szalay A., Thakar A. (2006) in "Mining The Sky",
         Banday A, Zaroubi S, Bartelmann M. eds.
         ESO Astrophysics Symposia
-        https://www.researchgate.net/publication/226072008_The_Hierarchical_Triangular_Mesh
+        https://www.researchgate.net/publication/
+        226072008_The_Hierarchical_Triangular_Mesh
         """
         return (
             (np.dot(pts, self.cross01) >= 0.0)
             & (np.dot(pts, self.cross12) >= 0.0)
             & (np.dot(pts, self.cross20) >= 0.0)
         )
 
@@ -208,15 +212,16 @@
         """
         An array of vectors needed to define the child trixels
         of this trixel.  See equation (3) of
 
         Kunszt P., Szalay A., Thakar A. (2006) in "Mining The Sky",
         Banday A, Zaroubi S, Bartelmann M. eds.
         ESO Astrophysics Symposia
-        httpd://www.researchgate.net/publication/226072008_The_Hierarchical_Triangular_Mesh
+        httpd://www.researchgate.net/publication/
+        226072008_The_Hierarchical_Triangular_Mesh
         """
         if self._w_arr is None:
             self._create_w()
         return self._w_arr
 
     @property
     def t0(self):
@@ -292,15 +297,16 @@
         which child to return
 
         See Figure 1 of
 
         Kunszt P., Szalay A., Thakar A. (2006) in "Mining The Sky",
         Banday A, Zaroubi S, Bartelmann M. eds.
         ESO Astrophysics Symposia
-        https://www.researchgate.net/publication/226072008_The_Hierarchical_Triangular_Mesh
+        https://www.researchgate.net/publication/
+        226072008_The_Hierarchical_Triangular_Mesh
 
         for an explanation of which trixel corresponds to whic
         index.
         """
         if dex == 0:
             return self.t0
         elif dex == 1:
@@ -374,15 +380,16 @@
             the center of the bounding circle
 
             First element is the distance from the center of
             the unit sphere to the plane of the bounding circle
             (i.e. the dot product of the zeroth element with the
             most distant corner of the trixel).
 
-            Second element is the half angular extent of the bounding circle.
+            Second element is the half angular extent of the
+            bounding circle.
         """
         if self._bounding_circle is None:
             # find the unit vector pointing to the center of the trixel
             vb = np.cross(
                 (self._corners[1] - self._corners[0]),
                 (self._corners[2] - self._corners[1]),
             )
@@ -403,15 +410,16 @@
 # Below are defined the initial Trixels
 #
 # See equations (1) and (2) of
 #
 # Kunszt P., Szalay A., Thakar A. (2006) in "Mining The Sky",
 # Banday A, Zaroubi S, Bartelmann M. eds.
 # ESO Astrophysics Symposia
-# https://www.researchgate.net/publication/226072008_The_Hierarchical_Triangular_Mesh
+# https://www.researchgate.net/publication/
+# 226072008_The_Hierarchical_Triangular_Mesh
 
 _n0_trixel = Trixel(
     12,
     [np.array([1.0, 0.0, 0.0]), np.array([0.0, 0.0, 1.0]), np.array([0.0, -1.0, 0.0])],
 )
 
 _n1_trixel = Trixel(
@@ -642,16 +650,16 @@
 
     max_level is the level of the triangular mesh at which we want
     to find the htmid.  Higher levels correspond to finer meshes.
     A mesh with level == ell contains 8*4**(ell-1) trixels.
 
     Returns
     -------
-    The htmid at the desired level of the trixel containing the unit sphere
-    projection of the point in pt.
+    The htmid at the desired level of the trixel containing the unit
+    sphere projection of the point in pt.
     """
     children = parent.get_children()
     for child in children:
         if child.contains_pt(pt):
             if child.level == max_level:
                 return child.htmid
             else:
@@ -882,15 +890,16 @@
         regions on the unit sphere divided by the circle
         where the plane of the halfspace intersects the
         unit sphere.
         """
         self._v = vector / np.sqrt(np.power(vector, 2).sum())
         self._d = length
         if np.abs(self._d) < 1.0:
-            self._phi = np.arccos(self._d)  # half angular extent of the half space
+            self._phi = np.arccos(self._d)  # half angular
+            # extent of the half space
             if self._phi > np.pi:
                 raise RuntimeError("phi %e d %e" % (self._phi, self._d))
         else:
             if self._d < 0.0:
                 self._phi = np.pi
             else:
                 self._phi = 0.0
@@ -1090,15 +1099,16 @@
     def merge_trixel_bounds(bounds):
         """
         Take a list of trixel bounds as returned by HalfSpace.find_all_trixels
         and merge any tuples that should be merged
 
         Parameters
         ----------
-        bounds is a list of trixel bounds as returned by HalfSpace.find_all_trixels
+        bounds is a list of trixel bounds as returned by
+        HalfSpace.find_all_trixels
 
         Returns
         -------
         A new, equivalent list of trixel bounds
         """
         list_of_mins = np.array([r[0] for r in bounds])
         sorted_dex = np.argsort(list_of_mins)
@@ -1120,17 +1130,17 @@
         if len(current_list) > 0:
             final_output.append((min(current_list), max(current_list)))
         return final_output
 
     @staticmethod
     def join_trixel_bound_sets(b1, b2):
         """
-        Take two sets of trixel bounds as returned by HalfSpace.find_all_trixels
-        and return a set of trixel bounds that represents the intersection of
-        the original sets of bounds
+        Take two sets of trixel bounds as returned by
+        HalfSpace.find_all_trixels and return a set of trixel bounds
+        that represents the intersection of the original sets of bounds
         """
         b1_sorted = HalfSpace.merge_trixel_bounds(b1)
         b2_sorted = HalfSpace.merge_trixel_bounds(b2)
 
         # maximum/minimum trixel bounds outside of which trixel ranges
         # will be considered invalid
         global_t_min = max(b1_sorted[0][0], b2_sorted[0][0])
@@ -1235,33 +1245,20 @@
                 children = tt.get_children()
                 for child in children:
                     is_contained = self.contains_trixel(child)
                     if is_contained == "partial":
                         # need to investigate more fully
                         new_active_trixels.append(child)
                     elif is_contained == "full":
-                        # all of this trixels children, and their children are contained
+                        # all of this trixels children, and
+                        # their children are contained
                         min_htmid = child._htmid << 2 * (level - i_level)
                         max_htmid = min_htmid
                         max_htmid += max_d_htmid
                         output_prelim.append((min_htmid, max_htmid))
-
-                        ########################################
-                        # some assertions for debugging purposes
-                        # assert min_htmid<max_htmid
-                        # try:
-                        #     test_trix = trixel_from_htmid(min_htmid)
-                        #     assert self.contains_trixel(test_trix) != 'outside'
-                        #     test_trix = trixel_from_htmid(max_htmid)
-                        #     assert self.contains_trixel(test_trix) != 'outside'
-                        # except AssertionError:
-                        #     print('is_contained %s' % is_contained)
-                        #     print('level %d' % level_from_htmid(tt._htmid))
-                        #     raise
-
                 active_trixels = new_active_trixels
             if len(active_trixels) == 0:
                 break
 
         # final pass over the active_trixels to see which of their
         # children are inside this HalfSpace
         for trix in active_trixels:
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/m5_flat_sed.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/m5_flat_sed.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,44 +27,47 @@
     nexp : int
         Number of exposures
     airmass : float
         Airmass of the observation
     fwhm_eff : np.ndarray or pd.DataFrame
         FWHM (in arcseconds) per filter
     musky : np.ndarray or pd.DataFrame
-        Sky background (in magnitudes/sq arcsecond) per filter of the observation
+        Sky background (in magnitudes/sq arcsecond) per filter of
+        the observation
     dark_sky_mag : np.ndarray or pd.DataFrame
-        Dark Sky, zenith magnitude/sq arcsecond - to scale musky. per filter
+        Dark Sky, zenith magnitude/sq arcsecond - to scale musky.
+        per filter
     cm : np.ndarray or pd.DataFrame
         cm value for the throughputs per filter
     d_cm_infinity : np.ndarray or pd.DataFrame
         d_cm_infinity values for the throughputs, per filter
     k_atm : np.ndarray or pd.DataFrame
         Atmospheric extinction values, per filter
     tau_cloud : float, optional
         Extinction due to clouds
     base_exp_time : float, optional
-        The exposure time used to calculate cm / d_cm_infinity. Used to scale exp_time.
-        This is the individual exposure exposure time.
+        The exposure time used to calculate cm / d_cm_infinity.
+        Used to scale exp_time. This is the individual exposure exposure time.
 
     Returns
     -------
     np.ndarray or pd.DataFrame
         m5 values scaled for the visit conditions
 
-    Note: The columns required as input for m5_scale can be calculated using
-    the makeM5 function in lsst.syseng.throughputs.
+    Note: The columns required as input for m5_scale can be
+    calculated using the makeM5 function in lsst.syseng.throughputs.
     """
     # Calculate adjustment if readnoise is significant for exposure time
     # (see overview paper, equation 7)
     tscale = exp_time / base_exp_time * np.power(10.0, -0.4 * (musky - dark_sky_mag))
     d_cm = 0.0
     d_cm += d_cm_infinity
     d_cm -= 1.25 * np.log10(1 + (10 ** (0.8 * d_cm_infinity) - 1) / tscale)
-    # Calculate m5 for 1 exp - constants here come from definition of cm/d_cm_infinity
+    # Calculate m5 for 1 exp - constants here come from
+    # definition of cm/d_cm_infinity
     m5 = (
         cm
         + d_cm
         + 0.50 * (musky - 21.0)
         + 2.5 * np.log10(0.7 / fwhm_eff)
         + 1.25 * np.log10(exp_time / 30.0)
         - k_atm * (airmass - 1.0)
@@ -72,51 +75,60 @@
     )
     if nexp > 1:
         m5 = 1.25 * np.log10(nexp * 10 ** (0.8 * m5))
     return m5
 
 
 def m5_flat_sed(visit_filter, musky, fwhm_eff, exp_time, airmass, nexp=1, tau_cloud=0):
-    """Calculate the m5 value, using photometric scaling.  Note, does not include shape of the object SED.
+    """Calculate the m5 value, using photometric scaling.  Note,
+    does not include shape of the object SED.
 
     Parameters
     ----------
     visit_filter : str
          One of u,g,r,i,z,y
     musky : float
         Surface brightness of the sky in mag/sq arcsec
     fwhm_eff : float
         The seeing effective FWHM (arcsec)
     exp_time : float
         Exposure time for each exposure in the visit.
     airmass : float
         Airmass of the observation (unitless)
     nexp : int, optional
-        The number of exposures. Default 1.  (total on-sky time = exp_time * nexp)
+        The number of exposures. Default 1.  (total on-sky
+        time = exp_time * nexp)
     tau_cloud : float (0.)
-        Any extinction from clouds in magnitudes (positive values = more extinction)
+        Any extinction from clouds in magnitudes
+        (positive values = more extinction)
 
     Returns
     -------
     m5 : float
-        The five-sigma limiting depth of a point source observed in the given conditions.
+        The five-sigma limiting depth of a point source observed in
+        he given conditions.
     """
 
-    # Set up expected extinction (kAtm) and m5 normalization values (Cm) for each filter.
-    # The Cm values must be changed when telescope and site parameters are updated.
+    # Set up expected extinction (kAtm) and m5 normalization values
+    # (Cm) for each filter. The Cm values must be changed when
+    # telescope and site parameters are updated.
     #
-    # These values are calculated using $SYSENG_THROUGHPUTS/python/calcM5.py.
-    # This set of values are calculated using v1.2 of the SYSENG_THROUGHPUTS repo.
-    # The exposure time scaling depends on knowing the value of the exposure time used to calculate Cm/etc.
+    # These values are calculated using
+    # $SYSENG_THROUGHPUTS/python/calcM5.py.
+    # This set of values are calculated using v1.2 of the
+    # SYSENG_THROUGHPUTS repo. The exposure time scaling depends
+    # on knowing the value of the exposure time used to calculate Cm/etc.
 
     # Only define the dicts once on initial call
     if not hasattr(m5_flat_sed, "Cm"):
         # Using Cm / d_cm_infinity values calculated for a 1x30s visit.
-        # This results in an error of about 0.01 mag in u band for 2x15s visits (< in other bands)
-        # See https://github.com/lsst-pst/survey_strategy/blob/master/fbs_1.3/m5FlatSed%20update.ipynb
+        # This results in an error of about 0.01 mag in u band for
+        # 2x15s visits (< in other bands) See
+        # https://github.com/lsst-pst/survey_strategy/blob/master/
+        # fbs_1.3/m5FlatSed%20update.ipynb
         # for a more in-depth evaluation.
         sev = SysEngVals()
 
         m5_flat_sed.base_exp_time = sev.exptime
         m5_flat_sed.cm = sev.cm
         m5_flat_sed.d_cm_infinity = sev.d_cm_infinity
         m5_flat_sed.k_atm = sev.k_atm
@@ -125,15 +137,16 @@
     # (see overview paper, equation 7)
     tscale = (
         exp_time / m5_flat_sed.base_exp_time * np.power(10.0, -0.4 * (musky - m5_flat_sed.msky[visit_filter]))
     )
     d_cm = 0.0
     d_cm += m5_flat_sed.d_cm_infinity[visit_filter]
     d_cm -= 1.25 * np.log10(1 + (10 ** (0.8 * m5_flat_sed.d_cm_infinity[visit_filter]) - 1) / tscale)
-    # Calculate m5 for 1 exp - 30s and other constants here come from definition of Cm/d_cm_infinity
+    # Calculate m5 for 1 exp - 30s and other constants here come
+    # from definition of Cm/d_cm_infinity
     m5 = (
         m5_flat_sed.cm[visit_filter]
         + d_cm
         + 0.50 * (musky - 21.0)
         + 2.5 * np.log10(0.7 / fwhm_eff)
         + 1.25 * np.log10(exp_time / 30.0)
         - m5_flat_sed.k_atm[visit_filter] * (airmass - 1.0)
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/projections.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/projections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __all__ = ("gnomonic_project_toxy", "gnomonic_project_tosky")
 
 import numpy as np
 
 
 def gnomonic_project_toxy(ra1, dec1, r_acen, deccen):
-    """Calculate x/y projection of ra1/dec1 in system with center at r_acen, deccen.
+    """Calculate x/y projection of ra1/dec1 in system with center
+    at r_acen, deccen.
     Input radians. Grabbed from sims_selfcal"""
     # also used in Global Telescope Network website
     cosc = np.sin(deccen) * np.sin(dec1) + np.cos(deccen) * np.cos(dec1) * np.cos(ra1 - r_acen)
     x = np.cos(dec1) * np.sin(ra1 - r_acen) / cosc
     y = (np.cos(deccen) * np.sin(dec1) - np.sin(deccen) * np.cos(dec1) * np.cos(ra1 - r_acen)) / cosc
     return x, y
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/riseset.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/riseset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 """Second generation hourglass plotting classes.
 """
 
 __all__ = ("riseset_times",)
-# pylint: disable=too-many-arguments
-# pylint: disable=too-many-instance-attributes
 
-# imports
 import warnings
 
 import astropy.coordinates
 import astropy.time
 import numpy as np
 from astropy import units as u
 from astropy.utils import iers
 
-# constants
-
-# exception classes
-
-# interface functions
-
 
 def riseset_times(  # pylint: disable=too-many-locals
     night_mjds,
     which_direction="down",
     which_night="nearest",
     alt=-14.0,
     location=astropy.coordinates.EarthLocation.of_site("Cerro Pachon"),
@@ -68,15 +59,15 @@
             century = (mjd - 51544.5) / 36525
             gst = (
                 280.46061837
                 + 360.98564736629 * (mjd - 51544.5)
                 + 0.000387933 * century * century
                 - century * century * century / 38710000
             )
-            lst = ((gst + location.lon.deg) % 360) * u.deg  # pylint: disable=no-member
+            lst = ((gst + location.lon.deg) % 360) * u.deg
 
         return lst
 
     event_direction = 1 if which_direction == "down" else -1
 
     night_wraps = {"previous": 0.0, "nearest": 180.0, "next": 360.0}
     night_wrap = night_wraps[which_night]
@@ -107,15 +98,16 @@
         if finished:
             break
 
         current_sinalt = np.sin(current_alt.rad)
         target_sinalt = np.sin(np.radians(alt))
 
         ha = _compute_lst(times) - crds.ra  # pylint: disable=invalid-name
-        # Derivative of the standard formula for sin(alt) in terms of decl, latitude, and HA
+        # Derivative of the standard formula for sin(alt) in terms
+        # of decl, latitude, and HA
         dsinalt_dlst = (-1 * np.cos(crds.dec) * np.cos(location.lat) * np.sin(ha)).value
         dsinalt_dmjd = dsinalt_dlst * (2 * np.pi / 0.9972696)
         mjds = mjds - (current_sinalt - target_sinalt) / dsinalt_dmjd
 
     if np.max(np.abs(mjds - night_mjds)) > 1:
         warnings.warn("On some nights, found twilight more than a day away from the night mjd")
 
@@ -125,12 +117,7 @@
             try:
                 first_unfinished_mjd = night_mjds[unfinished][0]
             except IndexError:
                 first_unfinished_mjd = night_mjds[unfinished]
             warnings.warn(f"twilight_times did not converge, starting with {first_unfinished_mjd}")
 
     return mjds
-
-
-# classes
-
-# internal functions & classes
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/sampling_functions.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/sampling_functions.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/site.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,44 +9,46 @@
     """
     This is a struct containing the LSST site parameters as defined in
 
     https://docushare.lsstcorp.org/docushare/dsweb/ImageStoreViewer/LSE-30
 
     (accessed on 4 January 2016)
 
-    This class only exists for initializing Site with LSST parameter values.
+    This class only exists for initializing Site with LSST parametervalues.
     Users should not be accessing this class directly.
     """
 
     def __init__(self):
         self.longitude = -70.7494  # in degrees
         self.latitude = -30.2444  # in degrees
         self.height = 2650.0  # in meters
         self.temperature = 11.5  # in centigrade
         self.pressure = 750.0  # in millibars
         self.humidity = 0.4  # scale 0-1
         self.lapse_rate = 0.0065  # in Kelvin per meter
         # the lapse rate was not specified by LSE-30;
         # 0.0065 K/m appears to be the "standard" value
-        # see, for example http://mnras.oxfordjournals.org/content/365/4/1235.full
+        # see, for example
+        # http://mnras.oxfordjournals.org/content/365/4/1235.full
 
 
 class Site:
     """
     This class will store site information for use in Catalog objects.
 
-    Defaults values are LSST site values taken from the Observatory System Specification
-    document
+    Defaults values are LSST site values taken from the Observatory
+    System Specification document
     https://docushare.lsstcorp.org/docushare/dsweb/ImageStoreViewer/LSE-30
     on 4 January 2016
 
     Parameters
     ----------
     name : `str`, opt
-        The name of the observatory. Set to 'LSST' for other parameters to default to LSST values.
+        The name of the observatory. Set to 'LSST' for other parameters
+        to default to LSST values.
     longitude : `float`, opt
         Longitude of the site in degrees.
     latitude : `float`, opt
         Latitude of the site in degrees.
     height : `float`, opt
         Height of the site in meters.
     temperature : `float`, opt
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/sys_eng_vals.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/sys_eng_vals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# Values from systems engineering that may need to be updated when new filter curves come out
+# Values from systems engineering that may need to be updated when
+# new filter curves come out
 
 __all__ = ("SysEngVals",)
 
 
 class SysEngVals:
     """Object to store values calculated in sys-eng
 
-    generated from notebook in:  https://github.com/lsst-pst/syseng_throughputs/tree/master/notebooks
+    generated from notebook in:
+    https://github.com/lsst-pst/syseng_throughputs/tree/master/notebooks
     """
 
     def __init__(self):
         self.zp_t = {
             "u": 26.524237,
             "g": 28.508375,
             "r": 28.360838,
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/tree_utils.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/tree_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 """
-This file contains coordinate transformation methods and utilities for converting an ra,dec coordinate set to
-cartesian coordinates and to grid id using a spatial tree.
+This file contains coordinate transformation methods and utilities
+for converting an ra,dec coordinate set to cartesian coordinates and
+to grid id using a spatial tree.
 """
 
 __all__ = ("_build_tree",)
 
 import numpy as np
 from scipy.spatial import cKDTree as kdTree
 
 from rubin_scheduler.utils.coordinate_transformations import _xyz_from_ra_dec
 
 
 def _build_tree(ra, dec, leafsize=100, scale=None):
     """
-    Build KD tree on simDataRA/Dec and set radius (via set_rad) for matching.
+    Build KD tree on simDataRA/Dec and set radius (via set_rad) for
+    matching.
 
     Parameters
     ----------
     ra, dec : float (or arrays)
         RA and Dec values (in radians).
     leafsize : int (100)
         The number of Ra/Dec pointings in each leaf node.
     scale : float (None)
-        If set, the values are scaled up, rounded, and converted to integers. Useful for
-        forcing a set precision and preventing machine precision differences
+        If set, the values are scaled up, rounded, and converted to
+        integers. Useful for forcing a set precision and preventing
+        machine precision differences
     """
     if np.any(np.abs(ra) > np.pi * 2.0) or np.any(np.abs(dec) > np.pi * 2.0):
         raise ValueError("Expecting RA and Dec values to be in radians.")
     x, y, z = _xyz_from_ra_dec(ra, dec)
     if scale is not None:
         x = np.round(x * scale).astype(int)
         y = np.round(y * scale).astype(int)
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler/utils/zernike_module.py` & `rubin_scheduler-1.2.0/rubin_scheduler/utils/zernike_module.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler.egg-info/PKG-INFO` & `rubin_scheduler-1.2.0/rubin_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubin-scheduler
-Version: 1.1.1
+Version: 1.2.0
 Summary: Scheduling algorithms for Vera C. Rubin Observatory's Legacy Survey of Space and Time (LSST).
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `rubin-scheduler-1.1.1/rubin_scheduler.egg-info/SOURCES.txt` & `rubin_scheduler-1.2.0/rubin_scheduler.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 rubin_scheduler/scheduler/utils/comcam_tessellate.py
 rubin_scheduler/scheduler/utils/dithering.py
 rubin_scheduler/scheduler/utils/footprints.py
 rubin_scheduler/scheduler/utils/sky_area.py
 rubin_scheduler/scheduler/utils/tsp.py
 rubin_scheduler/scheduler/utils/utils.py
 rubin_scheduler/sim_archive/__init__.py
+rubin_scheduler/sim_archive/prenight.py
 rubin_scheduler/sim_archive/sim_archive.py
 rubin_scheduler/site_models/__init__.py
 rubin_scheduler/site_models/almanac.py
 rubin_scheduler/site_models/cloud_data.py
 rubin_scheduler/site_models/cloud_model.py
 rubin_scheduler/site_models/downtime_model.py
 rubin_scheduler/site_models/generate_planets.py
@@ -132,14 +133,15 @@
 rubin_scheduler/utils/get_package_dir.py
 rubin_scheduler/utils/healpy_utils.py
 rubin_scheduler/utils/htm_module.py
 rubin_scheduler/utils/m5_flat_sed.py
 rubin_scheduler/utils/mjd_zero.py
 rubin_scheduler/utils/projections.py
 rubin_scheduler/utils/riseset.py
+rubin_scheduler/utils/rotskypos.py
 rubin_scheduler/utils/sampling_functions.py
 rubin_scheduler/utils/season_utils.py
 rubin_scheduler/utils/site.py
 rubin_scheduler/utils/sys_eng_vals.py
 rubin_scheduler/utils/tree_utils.py
 rubin_scheduler/utils/zernike_module.py
 tests/data/test_data.py
@@ -150,14 +152,15 @@
 tests/scheduler/test_coresched.py
 tests/scheduler/test_features.py
 tests/scheduler/test_modelobs.py
 tests/scheduler/test_scalarbf.py
 tests/scheduler/test_skyarea.py
 tests/scheduler/test_surveys.py
 tests/scheduler/test_utils.py
+tests/sim_archive/test_prenight.py
 tests/sim_archive/test_sim_archive.py
 tests/site_models/test_almanac.py
 tests/site_models/test_clouddata.py
 tests/site_models/test_cloudmodel.py
 tests/site_models/test_downtimemodel.py
 tests/site_models/test_scheduleddowntimedata.py
 tests/site_models/test_seeingdata.py
@@ -171,11 +174,12 @@
 tests/utils/test_codeutilities.py
 tests/utils/test_coordinatetransformations.py
 tests/utils/test_filemaps.py
 tests/utils/test_healutils.py
 tests/utils/test_kdtree.py
 tests/utils/test_m5flatsed.py
 tests/utils/test_riseset.py
+tests/utils/test_rotsky.py
 tests/utils/test_site.py
 tests/utils/test_trixel.py
 tests/utils/test_zernikemodule.py
 tests/utils/test_modules/dummy_module.py
```

### Comparing `rubin-scheduler-1.1.1/tests/scheduler/test_baseline.py` & `rubin_scheduler-1.2.0/tests/scheduler/test_baseline.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,16 @@
         assert observations.size > 1000
         # Make sure nothing tried to look through the earth
         assert np.min(observations["alt"]) > 0
 
     @unittest.skipUnless(os.path.isfile(SAMPLE_BIG_DATA_FILE), "Test data not available.")
     def test_wind(self):
         """
-        Test that a wind mask prevent things from being executed in the wrong spot
+        Test that a wind mask prevent things from being executed in
+        the wrong spot
         """
         mjd_start = utils.survey_start_mjd()
         nside = 32
         survey_length = 4.0  # days
 
         surveys = []
         # Set up the DD
```

### Comparing `rubin-scheduler-1.1.1/tests/scheduler/test_basisfuncs.py` & `rubin_scheduler-1.2.0/tests/scheduler/test_basisfuncs.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/scheduler/test_comcam.py` & `rubin_scheduler-1.2.0/tests/scheduler/test_comcam.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/scheduler/test_constant_weather.py` & `rubin_scheduler-1.2.0/tests/scheduler/test_constant_weather.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/scheduler/test_coresched.py` & `rubin_scheduler-1.2.0/tests/scheduler/test_coresched.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/scheduler/test_modelobs.py` & `rubin_scheduler-1.2.0/tests/scheduler/test_modelobs.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/scheduler/test_scalarbf.py` & `rubin_scheduler-1.2.0/tests/scheduler/test_scalarbf.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/scheduler/test_skyarea.py` & `rubin_scheduler-1.2.0/tests/scheduler/test_skyarea.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/scheduler/test_surveys.py` & `rubin_scheduler-1.2.0/tests/scheduler/test_surveys.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/scheduler/test_utils.py` & `rubin_scheduler-1.2.0/tests/scheduler/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import os
 import unittest
 
+import healpy as hp
 import numpy as np
 
 from rubin_scheduler.data import get_data_dir
 from rubin_scheduler.scheduler import sim_runner
 from rubin_scheduler.scheduler.example import example_scheduler, run_sched
 from rubin_scheduler.scheduler.model_observatory import KinemModel, ModelObservatory
 from rubin_scheduler.scheduler.utils import (
     SchemaConverter,
     empty_observation,
+    make_rolling_footprints,
     restore_scheduler,
     run_info_table,
     season_calc,
 )
 from rubin_scheduler.utils import survey_start_mjd
 
 
@@ -38,17 +40,18 @@
     def test_example(self):
         """Test the example scheduler executes all the expected surveys"""
         mjd_start = survey_start_mjd()
         scheduler = example_scheduler(mjd_start=mjd_start)
         observatory, scheduler, observations = run_sched(scheduler, mjd_start=mjd_start, survey_length=7)
         u_notes = np.unique(observations["note"])
 
-        # Note that some of these may change and need to be updated if survey
-        # start date changes, e.g., different DDFs in season, or different lunar phase
-        # means different filters get picked for the blobs
+        # Note that some of these may change and need to be updated if
+        # survey start date changes, e.g., different DDFs in season,
+        # or different lunar phase means different filters get picked
+        # for the blobs
         notes_to_check = [
             "blob_long, gr, a",
             "blob_long, gr, b",
             "greedy",
             "long",
             "pair_15, iz, a",
             "pair_15, iz, b",
@@ -90,15 +93,16 @@
         )
 
     @unittest.skipUnless(
         os.path.isfile(os.path.join(get_data_dir(), "scheduler/dust_maps/dust_nside_32.npz")),
         "Test data not available.",
     )
     def test_altaz_limit(self):
-        """Test that setting some azimuth limits via the kinematic model works"""
+        """Test that setting some azimuth limits via the kinematic
+        model works"""
         mjd_start = survey_start_mjd()
         scheduler = example_scheduler(mjd_start=mjd_start)
         km = KinemModel(mjd0=mjd_start)
         km.setup_telescope(az_limits=[[0.0, 90.0], [270.0, 360.0]])
         mo = ModelObservatory(mjd_start=mjd_start, kinem_model=km)
 
         mo, scheduler, observations = sim_runner(
@@ -107,15 +111,16 @@
             survey_length=3.0,
             verbose=False,
             filename=None,
         )
 
         az = np.degrees(observations["az"])
         forbidden = np.where((az > 90) & (az < 270))[0]
-        # Let a few pairs try to complete since by default we don't use an agressive shadow_minutes
+        # Let a few pairs try to complete since by default we don't
+        # use an agressive shadow_minutes
         n_forbidden = np.size(
             [obs for obs in observations[forbidden]["note"] if (("pair_33" not in obs) | (", b" not in obs))]
         )
 
         assert n_forbidden == 0
 
         km = KinemModel(mjd0=mjd_start)
@@ -181,16 +186,16 @@
             new_sched,
             survey_length=20.0,
             verbose=False,
             filename=None,
             n_visit_limit=new_n_limit,
         )
 
-        # Check that observations taken after restart match those from before
-        # Jenkins can be bad at comparing things, so if it thinks
+        # Check that observations taken after restart match those from
+        # before Jenkins can be bad at comparing things, so if it thinks
         # they aren't the same, check column-by-column to double check
         if not np.all(new_obs == observations[break_indx:]):
             names = new_obs.dtype.names
             for name in names:
                 # If it's a string
                 if new_obs[name].dtype == "<U40":
                     assert np.all(new_obs[name] == observations[break_indx:][name])
@@ -214,17 +219,18 @@
             new_sched,
             survey_length=20.0,
             verbose=False,
             filename=None,
             n_visit_limit=new_n_limit,
         )
 
-        # Check that observations taken after restart match those from before
-        # Jenkins can be bad at comparing things, so if it thinks
-        # they aren't the same, check column-by-column to double check
+        # Check that observations taken after restart match those
+        # from before Jenkins can be bad at comparing things, so if
+        # it thinks they aren't the same, check column-by-column to
+        # double check
         if not np.all(new_obs_fast == observations[break_indx:]):
             names = new_obs_fast.dtype.names
             for name in names:
                 # If it's a string
                 if new_obs_fast[name].dtype == "<U40":
                     assert np.all(new_obs_fast[name] == observations[break_indx:][name])
                 # Otherwise should be number-like
@@ -293,10 +299,108 @@
             "site_models",
             "skybrightness_pre",
         ]
         have_keys = list(version_info["Parameter"])
         for k in need_keys:
             self.assertTrue(k in have_keys)
 
+    def test_make_rolling_footprints_uniform(self):
+        """Test that we can make a uniform folling footprint"""
+
+        # utility function to get sun ra at a given mjd
+        from astropy.coordinates import EarthLocation, get_sun
+        from astropy.time import Time
+
+        def _get_sun_ra_at_mjd(mjd):
+            t = Time(
+                mjd,
+                format="mjd",
+                location=EarthLocation.of_site("Cerro Pachon"),
+            )
+            return get_sun(t).ra.deg
+
+        nside = 32
+        scale = 0.9
+        order_roll = 1
+
+        # setup a simple test survey with dec < 20
+        _, dec = hp.pix2ang(nside, np.arange(hp.nside2npix(nside)), lonlat=True)
+        base_footprint = np.zeros(hp.nside2npix(nside), dtype=float)
+        wfd_indx = np.where(dec < 20)[0]
+        base_footprint[wfd_indx] = 1
+
+        # now test uniformity of uniform rolling and baseline at a range
+        # of survey start times
+        for mjd_offset in [0, 12, 60, 90, 180, 195, 240, 267, 270, 319]:
+            mjd_start = survey_start_mjd() + mjd_offset
+            sun_ra_start = _get_sun_ra_at_mjd(mjd_start)
+            fp_hp = {
+                "g": base_footprint.copy(),
+                "r": base_footprint.copy(),
+                "i": base_footprint.copy(),
+            }
+
+            for nslice in [2, 3]:
+                uniform_footprint = make_rolling_footprints(
+                    fp_hp=fp_hp,
+                    mjd_start=mjd_start,
+                    sun_ra_start=sun_ra_start,
+                    nslice=nslice,
+                    scale=scale,
+                    nside=nside,
+                    wfd_indx=wfd_indx,
+                    order_roll=order_roll,
+                    n_cycles=None,
+                    n_constant_start=None,
+                    n_constant_end=6,
+                    uniform=True,
+                )
+
+                footprint = make_rolling_footprints(
+                    fp_hp=fp_hp,
+                    mjd_start=mjd_start,
+                    sun_ra_start=sun_ra_start,
+                    nslice=nslice,
+                    scale=scale,
+                    nside=nside,
+                    wfd_indx=wfd_indx,
+                    order_roll=order_roll,
+                    n_cycles=None,
+                    n_constant_start=None,
+                    n_constant_end=6,
+                    uniform=False,
+                )
+
+                # make sure all of the bands are OK
+                for band in ["g", "r", "i"]:
+                    # look at each yearly release
+                    for i in range(1, 11):
+                        mjd = mjd_start + i * 365.25
+                        ud = uniform_footprint(mjd, norm=False)
+                        uniform_scat = np.std(ud[band][wfd_indx])
+
+                        # uniform rolling surveys have special times where the
+                        # scatter in the requested number of observations is 0
+                        if nslice == 2:
+                            if i in [1, 4, 7, 10]:
+                                self.assertTrue(np.allclose(uniform_scat, 0))
+                            else:
+                                self.assertTrue(uniform_scat != 0)
+                        elif nslice == 3:
+                            if i in [1, 5, 9, 10]:
+                                self.assertTrue(np.allclose(uniform_scat, 0))
+                            else:
+                                self.assertTrue(uniform_scat != 0)
+
+                        # non-uniform rolling surveys only have uniform
+                        # requests at Y1 and Y10
+                        d = footprint(mjd, norm=False)
+                        scat = np.std(d[band][wfd_indx])
+
+                        if i in [1, 10]:
+                            self.assertTrue(np.allclose(scat, 0))
+                        else:
+                            self.assertTrue(scat != 0)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `rubin-scheduler-1.1.1/tests/sim_archive/test_sim_archive.py` & `rubin_scheduler-1.2.0/tests/sim_archive/test_sim_archive.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/site_models/test_almanac.py` & `rubin_scheduler-1.2.0/tests/site_models/test_almanac.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/site_models/test_clouddata.py` & `rubin_scheduler-1.2.0/tests/site_models/test_clouddata.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/site_models/test_cloudmodel.py` & `rubin_scheduler-1.2.0/tests/site_models/test_cloudmodel.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/site_models/test_downtimemodel.py` & `rubin_scheduler-1.2.0/tests/site_models/test_downtimemodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,16 @@
         unsched = UnscheduledDowntimeData(t)
         unsched.make_data()
         efd_data = {"unscheduled_downtimes": unsched(), "scheduled_downtimes": sched()}
         # Set time to within first scheduled downtime.
         t_now = sched.downtime[0]["start"] + TimeDelta(0.5, format="jd")
         target_dict = {"time": t_now}
         dt_status = downtime_model(efd_data, target_dict)
-        # Expect return dict of : {'status': status, 'end': end_down, 'next': next_sched['start']}
+        # Expect return dict of : {'status': status, 'end': end_down,
+        # 'next': next_sched['start']}
         # Check keys
         for k in ("status", "end", "next"):
             self.assertTrue(k in dt_status)
         # downtime status is "True" if system is down.
         self.assertEqual(True, dt_status["status"])
         self.assertEqual(dt_status["end"], sched.downtime[0]["end"])
         self.assertEqual(dt_status["next"], sched.downtime[1]["start"])
```

### Comparing `rubin-scheduler-1.1.1/tests/site_models/test_scheduleddowntimedata.py` & `rubin_scheduler-1.2.0/tests/site_models/test_scheduleddowntimedata.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/site_models/test_seeingdata.py` & `rubin_scheduler-1.2.0/tests/site_models/test_seeingdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from astropy.time import Time, TimeDelta
 
 from rubin_scheduler.data import get_data_dir
 from rubin_scheduler.site_models import SeeingData
 
 # Unit test here uses oldest/original opsim seeing database, "Seeing.db".
-# Could be updated to use a new DB, but that would require changing some of these hard-coded numbers.
+# Could be updated to use a new DB, but that would require
+# changing some of these hard-coded numbers.
 
 
 class TestSeeingData(unittest.TestCase):
     def setUp(self):
         self.time = Time("2020-01-01", format="isot", scale="tai")
         self.seeing_db = os.path.join(get_data_dir(), "site_models", "seeing.db")
         print(self.seeing_db)
@@ -34,15 +35,16 @@
         dt = TimeDelta(63190400, format="sec")
         self.assertEqual(seeing_data(self.time + dt), 0.64860999584198)
         dt = TimeDelta(189424900, format="sec")
         self.assertEqual(seeing_data(self.time + dt), 0.699440002441406)
         # Test time selection from seeing data.
         dt = TimeDelta(800, format="sec")
         fwhm500 = seeing_data(self.time + dt)
-        # Hack seeing data to remove first date, thus db does not start at zero.
+        # Hack seeing data to remove first date, thus db does not start
+        # at zero.
         seeing_data.seeing_dates = seeing_data.seeing_dates[:-1]
         seeing_data.seeing_values = seeing_data.seeing_values[:-1]
         seeing_data.time_range = seeing_data.seeing_dates[-1] - seeing_data.seeing_dates[0]
         seeing_data.min_time = seeing_data.seeing_dates[0]
         self.assertEqual(fwhm500, seeing_data(self.time + dt))
 
     def test_using_different_start_month(self):
```

### Comparing `rubin-scheduler-1.1.1/tests/site_models/test_seeingmodel.py` & `rubin_scheduler-1.2.0/tests/site_models/test_seeingmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 class TestSeeingModel(unittest.TestCase):
     def test_fwhm_system_zenith(self):
         # Check calculation is being done as expected.
         seeing_model = SeeingModel()
         self.assertAlmostEqual(seeing_model.fwhm_system_zenith, 0.39862262855989494, places=7)
 
     def test_fwhm_geom_eff(self):
-        # Check that the translation between FWHM effective and geometric is done as expected.
-        # (note that fwhmEff_tofwhmGeom & fwhmGeom_to_fwhmEff are static methods)
-        # Document-20160 for reference.
+        # Check that the translation between FWHM effective and
+        # geometric is done as expected.
+        # (note that fwhmEff_tofwhmGeom & fwhmGeom_to_fwhmEff are
+        # static methods) Document-20160 for reference.
         fwhm_eff = 1.23
         fwhm_geom = 0.822 * fwhm_eff + 0.052
         self.assertEqual(fwhm_geom, SeeingModel.fwhm_eff_to_fwhm_geom(fwhm_eff))
         self.assertEqual(fwhm_eff, SeeingModel.fwhm_geom_to_fwhm_eff(fwhm_geom))
 
     def test_call(self):
         # Check the calculation from fwhm_500 to fwhm_eff/fwhm_geom.
@@ -30,15 +31,16 @@
         fwhm_500 = 1.0
         # Single airmass.
         airmass = 1.0
         seeing = seeing_model(fwhm_500, airmass)
         fwhm_eff = seeing["fwhmEff"]
         # Check shape of returned values.
         self.assertEqual(fwhm_eff.shape, (len(seeing_model.eff_wavelens),))
-        # Check actual value of seeing in @ wavelen[0] @ zenith after addition of system.
+        # Check actual value of seeing in @ wavelen[0] @ zenith
+        # after addition of system.
         fwhm_system = seeing_model.fwhm_system_zenith
         expected_fwhm_eff = 1.16 * np.sqrt(fwhm_system**2 + 1.04 * fwhm_500**2)
         self.assertAlmostEqual(fwhm_eff[0], expected_fwhm_eff, 15)
         # Check expected value if we remove the system component.
         seeing_model.fwhm_system_zenith = 0
         seeing = seeing_model(fwhm_500, airmass)
         expected_fwhm_eff = 1.16 * np.sqrt(1.04) * fwhm_500
```

### Comparing `rubin-scheduler-1.1.1/tests/site_models/test_unscheduleddowntimedata.py` & `rubin_scheduler-1.2.0/tests/site_models/test_unscheduleddowntimedata.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/skybrightness_pre/test_dark_sky.py` & `rubin_scheduler-1.2.0/tests/skybrightness_pre/test_dark_sky.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/skybrightness_pre/test_skypre.py` & `rubin_scheduler-1.2.0/tests/skybrightness_pre/test_skypre.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         if self.data_present:
             sms = [self.sm]
             mjds = []
             for mjd in sms[0].mjds[100:102]:
                 mjds.append(mjd)
                 mjds.append(mjd + 0.0002)
 
-            # Make sure there's an mjd that is between sunrise/set that gets tested
+            # Make sure there's an mjd that is between sunrise/set
+            # that gets tested
             diff = sms[0].mjds[1:] - sms[0].mjds[0:-1]
             between = np.where(diff >= timestep_max)[0][0]
             mjds.append(sms[0].mjds[between + 1] + timestep_max)
 
             indxes = [None, [100, 101]]
             filters = [["u", "g", "r", "i", "z", "y"], ["r"]]
 
@@ -56,14 +57,42 @@
                             # Check the magnitudes are correct
                             if indx is not None:
                                 self.assertEqual(
                                     np.size(mags[list(mags.keys())[0]]),
                                     np.size(indx),
                                 )
 
+    def test_bright_sky(self):
+        """Test that things behave if request a time with
+        a high sun altitude
+        """
+        # Find an MJD where the sun is high
+        diff = np.diff(self.sm.mjds)
+        mjd_indx = np.min(np.where(diff == diff.max())[0])
+        mjd = np.mean(self.sm.mjds[mjd_indx : mjd_indx + 2])
+
+        with self.assertWarns(Warning):
+            mags = self.sm.return_mags(mjd)
+            assert np.nanmin(mags["r"]) < 4.0
+
+        # Check that a little over raises the warning and returns
+        # closest map
+        mjd1 = self.sm.mjds[mjd_indx] - 0.001
+        mjd2 = self.sm.mjds[mjd_indx] + 0.001
+
+        # At a valid mjd
+        mags1 = self.sm.return_mags(mjd1)
+
+        # MJD slightly beyond where sky was calculated
+        with self.assertWarns(Warning):
+            mags2 = self.sm.return_mags(mjd2)
+
+        for key in mags1:
+            np.allclose(mags1[key], mags2[key])
+
     def test_various(self):
         """
         Test some various loading things
         """
         # check that the sims_data stuff loads
         sm = sbp.SkyModelPre(init_load_length=3)
         mjd = self.sm.mjds[10] + 0.1
```

### Comparing `rubin-scheduler-1.1.1/tests/utils/test_approx.py` & `rubin_scheduler-1.2.0/tests/utils/test_approx.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/utils/test_camerafootprint.py` & `rubin_scheduler-1.2.0/tests/utils/test_camerafootprint.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,13 +14,14 @@
         self.obs_rot_sky_pos = np.zeros(2)
 
     def test_camera(self):
         camera = LsstCameraFootprint(
             units="degrees",
         )
         idx_obs = camera(self.obj_ra, self.obj_dec, self.obs_ra, self.obs_dec, self.obs_rot_sky_pos)
-        # The first of these objects should be in the middle of the FOV, while the second is outside
+        # The first of these objects should be in the middle of
+        # the FOV, while the second is outside
         self.assertEqual(idx_obs, [0])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `rubin-scheduler-1.1.1/tests/utils/test_cleanup.py` & `rubin_scheduler-1.2.0/tests/utils/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/utils/test_codeutilities.py` & `rubin_scheduler-1.2.0/tests/utils/test_codeutilities.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/utils/test_coordinatetransformations.py` & `rubin_scheduler-1.2.0/tests/utils/test_coordinatetransformations.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/utils/test_filemaps.py` & `rubin_scheduler-1.2.0/tests/utils/test_filemaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from rubin_scheduler.utils import SpecMap, default_spec_map
 
 
 class SpecMapTest(unittest.TestCase):
     def verify_file(self, file_name, dir_name, test_spec_map=default_spec_map):
         """
-        Verify that test_spec_map[file_name] results in os.path.join(dir_name, file_name+'.gz')
+        Verify that test_spec_map[file_name] results in
+        os.path.join(dir_name, file_name+'.gz')
         """
         test_name = test_spec_map[file_name]
         control_name = os.path.join(dir_name, file_name + ".gz")
         msg = "%s should map to %s; it actually maps to %s" % (
             file_name,
             control_name,
             test_name,
```

### Comparing `rubin-scheduler-1.1.1/tests/utils/test_healutils.py` & `rubin_scheduler-1.2.0/tests/utils/test_healutils.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/utils/test_m5flatsed.py` & `rubin_scheduler-1.2.0/tests/utils/test_m5flatsed.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/utils/test_riseset.py` & `rubin_scheduler-1.2.0/tests/utils/test_riseset.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/utils/test_site.py` & `rubin_scheduler-1.2.0/tests/utils/test_site.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/utils/test_trixel.py` & `rubin_scheduler-1.2.0/tests/utils/test_trixel.py`

 * *Files identical despite different names*

### Comparing `rubin-scheduler-1.1.1/tests/utils/test_zernikemodule.py` & `rubin_scheduler-1.2.0/tests/utils/test_zernikemodule.py`

 * *Files identical despite different names*

