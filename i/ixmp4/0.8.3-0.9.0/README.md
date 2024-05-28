# Comparing `tmp/ixmp4-0.8.3.tar.gz` & `tmp/ixmp4-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixmp4-0.8.3.tar", max compression
+gzip compressed data, was "ixmp4-0.9.0.tar", max compression
```

## Comparing `ixmp4-0.8.3.tar` & `ixmp4-0.9.0.tar`

### file list

```diff
@@ -1,210 +1,210 @@
--rw-r--r--   0        0        0     1067 2024-04-19 07:27:24.598111 ixmp4-0.8.3/LICENSE
--rw-r--r--   0        0        0     3561 2024-04-19 07:27:24.598111 ixmp4-0.8.3/README.md
--rw-r--r--   0        0        0      800 2024-04-19 07:27:49.406341 ixmp4-0.8.3/ixmp4/__init__.py
--rw-r--r--   0        0        0       64 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/__main__.py
--rw-r--r--   0        0        0     2724 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/cli/__init__.py
--rw-r--r--   0        0        0     9357 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/cli/platforms.py
--rw-r--r--   0        0        0     1130 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/cli/server.py
--rw-r--r--   0        0        0      393 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/cli/utils.py
--rw-r--r--   0        0        0      243 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/conf/__init__.py
--rw-r--r--   0        0        0     4877 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/conf/auth.py
--rw-r--r--   0        0        0      255 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/conf/base.py
--rw-r--r--   0        0        0      827 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/conf/credentials.py
--rw-r--r--   0        0        0      404 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/conf/logging/debug.json
--rw-r--r--   0        0        0      402 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/conf/logging/development.json
--rw-r--r--   0        0        0      433 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/conf/logging/production.json
--rw-r--r--   0        0        0     1644 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/conf/logging/server.json
--rw-r--r--   0        0        0     6326 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/conf/manager.py
--rw-r--r--   0        0        0     5115 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/conf/settings.py
--rw-r--r--   0        0        0     1857 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/conf/toml.py
--rw-r--r--   0        0        0      468 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/conf/user.py
--rw-r--r--   0        0        0      432 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/__init__.py
--rw-r--r--   0        0        0      656 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/base.py
--rw-r--r--   0        0        0      525 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/decorators.py
--rw-r--r--   0        0        0     4419 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/exceptions.py
--rw-r--r--   0        0        0       64 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/iamc/__init__.py
--rw-r--r--   0        0        0     5596 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/iamc/data.py
--rw-r--r--   0        0        0     3658 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/iamc/variable.py
--rw-r--r--   0        0        0      381 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/meta.py
--rw-r--r--   0        0        0     3434 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/model.py
--rw-r--r--   0        0        0       35 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/optimization/__init__.py
--rw-r--r--   0        0        0      762 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/optimization/data.py
--rw-r--r--   0        0        0     3180 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/optimization/indexset.py
--rw-r--r--   0        0        0     4245 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/optimization/scalar.py
--rw-r--r--   0        0        0     3519 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/optimization/table.py
--rw-r--r--   0        0        0     2905 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/platform.py
--rw-r--r--   0        0        0     4565 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/region.py
--rw-r--r--   0        0        0     4566 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/run.py
--rw-r--r--   0        0        0     3568 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/scenario.py
--rw-r--r--   0        0        0     4245 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/unit.py
--rw-r--r--   0        0        0      708 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/core/utils.py
--rw-r--r--   0        0        0        0 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/data/__init__.py
--rw-r--r--   0        0        0     1041 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/data/abstract/__init__.py
--rw-r--r--   0        0        0     2022 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/data/abstract/base.py
--rw-r--r--   0        0        0     2849 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/data/abstract/docs.py
--rw-r--r--   0        0        0      308 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/data/abstract/iamc/__init__.py
--rw-r--r--   0        0        0     4620 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/data/abstract/iamc/datapoint.py
--rw-r--r--   0        0        0     1105 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/data/abstract/iamc/measurand.py
--rw-r--r--   0        0        0     4890 2024-04-19 07:27:24.602111 ixmp4-0.8.3/ixmp4/data/abstract/iamc/timeseries.py
--rw-r--r--   0        0        0     2659 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/abstract/iamc/variable.py
--rw-r--r--   0        0        0     5045 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/abstract/meta.py
--rw-r--r--   0        0        0     2704 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/abstract/model.py
--rw-r--r--   0        0        0      165 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/abstract/optimization/__init__.py
--rw-r--r--   0        0        0      798 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/abstract/optimization/column.py
--rw-r--r--   0        0        0     3833 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/abstract/optimization/indexset.py
--rw-r--r--   0        0        0     4709 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/abstract/optimization/scalar.py
--rw-r--r--   0        0        0     6019 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/abstract/optimization/table.py
--rw-r--r--   0        0        0     4104 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/abstract/region.py
--rw-r--r--   0        0        0     5775 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/abstract/run.py
--rw-r--r--   0        0        0     2693 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/abstract/scenario.py
--rw-r--r--   0        0        0     3692 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/abstract/unit.py
--rw-r--r--   0        0        0      750 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/__init__.py
--rw-r--r--   0        0        0    13984 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/base.py
--rw-r--r--   0        0        0     1160 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/docs.py
--rw-r--r--   0        0        0      255 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/iamc/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/iamc/datapoint.py
--rw-r--r--   0        0        0     1589 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/iamc/timeseries.py
--rw-r--r--   0        0        0     1483 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/iamc/variable.py
--rw-r--r--   0        0        0     1766 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/meta.py
--rw-r--r--   0        0        0     1417 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/model.py
--rw-r--r--   0        0        0      138 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/optimization/__init__.py
--rw-r--r--   0        0        0      474 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/optimization/column.py
--rw-r--r--   0        0        0     2086 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/optimization/indexset.py
--rw-r--r--   0        0        0     2282 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/optimization/scalar.py
--rw-r--r--   0        0        0     2376 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/optimization/table.py
--rw-r--r--   0        0        0     1675 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/region.py
--rw-r--r--   0        0        0     2214 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/run.py
--rw-r--r--   0        0        0     1470 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/scenario.py
--rw-r--r--   0        0        0     1593 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/api/unit.py
--rw-r--r--   0        0        0     3679 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/auth/context.py
--rw-r--r--   0        0        0     1465 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/auth/decorators.py
--rw-r--r--   0        0        0      141 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/backend/__init__.py
--rw-r--r--   0        0        0     6207 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/backend/api.py
--rw-r--r--   0        0        0     1234 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/backend/base.py
--rw-r--r--   0        0        0     4761 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/backend/db.py
--rw-r--r--   0        0        0      874 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/__init__.py
--rw-r--r--   0        0        0    15233 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/base.py
--rw-r--r--   0        0        0     3459 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/docs.py
--rw-r--r--   0        0        0      502 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/__init__.py
--rw-r--r--   0        0        0      528 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/meta.py
--rw-r--r--   0        0        0      391 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/model.py
--rw-r--r--   0        0        0      440 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/optimizationcolumn.py
--rw-r--r--   0        0        0      448 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/optimizationindexset.py
--rw-r--r--   0        0        0      581 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/optimizationscalar.py
--rw-r--r--   0        0        0      436 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/optimizationtable.py
--rw-r--r--   0        0        0      385 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/region.py
--rw-r--r--   0        0        0      776 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/run.py
--rw-r--r--   0        0        0      409 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/scenario.py
--rw-r--r--   0        0        0      419 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/timeseries.py
--rw-r--r--   0        0        0      470 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/unit.py
--rw-r--r--   0        0        0      490 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/filters/variable.py
--rw-r--r--   0        0        0      331 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/__init__.py
--rw-r--r--   0        0        0      302 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/base.py
--rw-r--r--   0        0        0      129 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/datapoint/__init__.py
--rw-r--r--   0        0        0     5896 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/datapoint/filter.py
--rw-r--r--   0        0        0     1356 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/datapoint/model.py
--rw-r--r--   0        0        0     7583 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/datapoint/repository.py
--rw-r--r--   0        0        0     2917 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/measurand.py
--rw-r--r--   0        0        0       75 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/timeseries/__init__.py
--rw-r--r--   0        0        0      401 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/timeseries/filter.py
--rw-r--r--   0        0        0     1160 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/timeseries/model.py
--rw-r--r--   0        0        0     4707 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/timeseries/repository.py
--rw-r--r--   0        0        0       86 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/variable/__init__.py
--rw-r--r--   0        0        0      235 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/variable/docs.py
--rw-r--r--   0        0        0      806 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/variable/filter.py
--rw-r--r--   0        0        0      584 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/variable/model.py
--rw-r--r--   0        0        0     1444 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/iamc/variable/repository.py
--rw-r--r--   0        0        0       79 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/meta/__init__.py
--rw-r--r--   0        0        0      570 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/meta/filter.py
--rw-r--r--   0        0        0     2246 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/meta/model.py
--rw-r--r--   0        0        0     7204 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/meta/repository.py
--rw-r--r--   0        0        0      118 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/model/__init__.py
--rw-r--r--   0        0        0      426 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/model/docs.py
--rw-r--r--   0        0        0     1780 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/model/filter.py
--rw-r--r--   0        0        0      517 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/model/model.py
--rw-r--r--   0        0        0     1371 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/model/repository.py
--rw-r--r--   0        0        0      183 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/optimization/__init__.py
--rw-r--r--   0        0        0      310 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/optimization/base.py
--rw-r--r--   0        0        0       67 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/optimization/column/__init__.py
--rw-r--r--   0        0        0      225 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/optimization/column/docs.py
--rw-r--r--   0        0        0      692 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/optimization/column/filter.py
--rw-r--r--   0        0        0     1170 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/optimization/column/model.py
--rw-r--r--   0        0        0     2440 2024-04-19 07:27:24.606111 ixmp4-0.8.3/ixmp4/data/db/optimization/column/repository.py
--rw-r--r--   0        0        0       71 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/indexset/__init__.py
--rw-r--r--   0        0        0      235 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/indexset/docs.py
--rw-r--r--   0        0        0      534 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/indexset/filter.py
--rw-r--r--   0        0        0     1278 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/indexset/model.py
--rw-r--r--   0        0        0     2348 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/indexset/repository.py
--rw-r--r--   0        0        0       67 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/scalar/__init__.py
--rw-r--r--   0        0        0      225 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/scalar/docs.py
--rw-r--r--   0        0        0      809 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/scalar/filter.py
--rw-r--r--   0        0        0     1084 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/scalar/model.py
--rw-r--r--   0        0        0     2552 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/scalar/repository.py
--rw-r--r--   0        0        0       65 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/table/__init__.py
--rw-r--r--   0        0        0      220 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/table/docs.py
--rw-r--r--   0        0        0      522 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/table/filter.py
--rw-r--r--   0        0        0     3554 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/table/model.py
--rw-r--r--   0        0        0     5079 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/optimization/table/repository.py
--rw-r--r--   0        0        0      121 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/region/__init__.py
--rw-r--r--   0        0        0      496 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/region/docs.py
--rw-r--r--   0        0        0     1547 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/region/filter.py
--rw-r--r--   0        0        0      611 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/region/model.py
--rw-r--r--   0        0        0     1569 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/region/repository.py
--rw-r--r--   0        0        0       61 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/run/__init__.py
--rw-r--r--   0        0        0     1254 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/run/filter.py
--rw-r--r--   0        0        0     1563 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/run/model.py
--rw-r--r--   0        0        0     5064 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/run/repository.py
--rw-r--r--   0        0        0      127 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/scenario/__init__.py
--rw-r--r--   0        0        0      222 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/scenario/docs.py
--rw-r--r--   0        0        0     1827 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/scenario/filter.py
--rw-r--r--   0        0        0      545 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/scenario/model.py
--rw-r--r--   0        0        0     1814 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/scenario/repository.py
--rw-r--r--   0        0        0     3331 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/timeseries.py
--rw-r--r--   0        0        0      126 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/unit/__init__.py
--rw-r--r--   0        0        0      495 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/unit/docs.py
--rw-r--r--   0        0        0     1714 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/unit/filter.py
--rw-r--r--   0        0        0      469 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/unit/model.py
--rw-r--r--   0        0        0     1725 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/unit/repository.py
--rw-r--r--   0        0        0      436 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/db/utils.py
--rw-r--r--   0        0        0     5531 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/generator.py
--rw-r--r--   0        0        0      292 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/data/types.py
--rw-r--r--   0        0        0     1585 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/db/__init__.py
--rw-r--r--   0        0        0     9465 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/db/filters.py
--rw-r--r--   0        0        0     2408 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/db/migrations/env.py
--rw-r--r--   0        0        0      509 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/db/migrations/script.py.mako
--rw-r--r--   0        0        0     5559 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/db/migrations/versions/081bbda6bb7b_create_optimization_table_table.py
--rw-r--r--   0        0        0     3778 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/db/migrations/versions/97ba231770e2_create_optimization_scalar_table.py
--rw-r--r--   0        0        0    19022 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/db/migrations/versions/c71efc396d2b_initial_migration.py
--rw-r--r--   0        0        0     5176 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/db/migrations/versions/da1fba23f206_create_optimization_indexset_table.py
--rw-r--r--   0        0        0     1478 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/db/utils/__init__.py
--rw-r--r--   0        0        0     1496 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/db/utils/alembic.py
--rw-r--r--   0        0        0     1052 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/db/utils/sqlite.py
--rw-r--r--   0        0        0        0 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/py.typed
--rw-r--r--   0        0        0      297 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/__init__.py
--rw-r--r--   0        0        0     2810 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/base.py
--rw-r--r--   0        0        0      192 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/decorators.py
--rw-r--r--   0        0        0     3606 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/deps.py
--rw-r--r--   0        0        0     6969 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/docs.py
--rw-r--r--   0        0        0       61 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/iamc/__init__.py
--rw-r--r--   0        0        0     2550 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/iamc/datapoint.py
--rw-r--r--   0        0        0      921 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/iamc/model.py
--rw-r--r--   0        0        0      930 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/iamc/region.py
--rw-r--r--   0        0        0      948 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/iamc/scenario.py
--rw-r--r--   0        0        0     1916 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/iamc/timeseries.py
--rw-r--r--   0        0        0      912 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/iamc/unit.py
--rw-r--r--   0        0        0     1263 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/iamc/variable.py
--rw-r--r--   0        0        0     1976 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/meta.py
--rw-r--r--   0        0        0      696 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/middleware.py
--rw-r--r--   0        0        0     1185 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/model.py
--rw-r--r--   0        0        0       38 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/optimization/__init__.py
--rw-r--r--   0        0        0     1832 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/optimization/indexset.py
--rw-r--r--   0        0        0     1946 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/optimization/scalar.py
--rw-r--r--   0        0        0     1928 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/optimization/table.py
--rw-r--r--   0        0        0     1372 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/region.py
--rw-r--r--   0        0        0     1621 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/run.py
--rw-r--r--   0        0        0     1227 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/scenario.py
--rw-r--r--   0        0        0     1304 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/rest/unit.py
--rw-r--r--   0        0        0      187 2024-04-19 07:27:24.610111 ixmp4-0.8.3/ixmp4/server/workers.py
--rw-r--r--   0        0        0     3046 2024-04-19 07:27:49.402341 ixmp4-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 ixmp4-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-28 11:26:38.445828 ixmp4-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3561 2024-05-28 11:26:38.445828 ixmp4-0.9.0/README.md
+-rw-r--r--   0        0        0      800 2024-05-28 11:26:54.965589 ixmp4-0.9.0/ixmp4/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/__main__.py
+-rw-r--r--   0        0        0     2724 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/cli/__init__.py
+-rw-r--r--   0        0        0     9357 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/cli/platforms.py
+-rw-r--r--   0        0        0     1317 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/cli/server.py
+-rw-r--r--   0        0        0      393 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/cli/utils.py
+-rw-r--r--   0        0        0      243 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/conf/__init__.py
+-rw-r--r--   0        0        0     4877 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/conf/auth.py
+-rw-r--r--   0        0        0      255 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/conf/base.py
+-rw-r--r--   0        0        0      827 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/conf/credentials.py
+-rw-r--r--   0        0        0      404 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/conf/logging/debug.json
+-rw-r--r--   0        0        0      402 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/conf/logging/development.json
+-rw-r--r--   0        0        0      433 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/conf/logging/production.json
+-rw-r--r--   0        0        0     1667 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/conf/logging/server.json
+-rw-r--r--   0        0        0     6326 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/conf/manager.py
+-rw-r--r--   0        0        0     4968 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/conf/settings.py
+-rw-r--r--   0        0        0     1857 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/conf/toml.py
+-rw-r--r--   0        0        0      468 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/conf/user.py
+-rw-r--r--   0        0        0      432 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/__init__.py
+-rw-r--r--   0        0        0      656 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/base.py
+-rw-r--r--   0        0        0      525 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/decorators.py
+-rw-r--r--   0        0        0     4419 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/exceptions.py
+-rw-r--r--   0        0        0       64 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/iamc/__init__.py
+-rw-r--r--   0        0        0     5152 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/iamc/data.py
+-rw-r--r--   0        0        0     3658 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/iamc/variable.py
+-rw-r--r--   0        0        0      381 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/meta.py
+-rw-r--r--   0        0        0     3434 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/model.py
+-rw-r--r--   0        0        0       35 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/optimization/__init__.py
+-rw-r--r--   0        0        0      762 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/optimization/data.py
+-rw-r--r--   0        0        0     3180 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/optimization/indexset.py
+-rw-r--r--   0        0        0     4287 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/optimization/scalar.py
+-rw-r--r--   0        0        0     3519 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/optimization/table.py
+-rw-r--r--   0        0        0     2905 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/platform.py
+-rw-r--r--   0        0        0     4565 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/region.py
+-rw-r--r--   0        0        0     4566 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/run.py
+-rw-r--r--   0        0        0     3568 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/scenario.py
+-rw-r--r--   0        0        0     4138 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/unit.py
+-rw-r--r--   0        0        0      708 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/core/utils.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/data/__init__.py
+-rw-r--r--   0        0        0     1041 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/data/abstract/__init__.py
+-rw-r--r--   0        0        0     2022 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/data/abstract/base.py
+-rw-r--r--   0        0        0     2849 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/data/abstract/docs.py
+-rw-r--r--   0        0        0      308 2024-05-28 11:26:38.449828 ixmp4-0.9.0/ixmp4/data/abstract/iamc/__init__.py
+-rw-r--r--   0        0        0     4620 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/iamc/datapoint.py
+-rw-r--r--   0        0        0     1105 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/iamc/measurand.py
+-rw-r--r--   0        0        0     4890 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/iamc/timeseries.py
+-rw-r--r--   0        0        0     2659 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/iamc/variable.py
+-rw-r--r--   0        0        0     5045 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/meta.py
+-rw-r--r--   0        0        0     2704 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/model.py
+-rw-r--r--   0        0        0      165 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/optimization/__init__.py
+-rw-r--r--   0        0        0      798 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/optimization/column.py
+-rw-r--r--   0        0        0     3833 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/optimization/indexset.py
+-rw-r--r--   0        0        0     4709 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/optimization/scalar.py
+-rw-r--r--   0        0        0     6019 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/optimization/table.py
+-rw-r--r--   0        0        0     4104 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/region.py
+-rw-r--r--   0        0        0     5775 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/run.py
+-rw-r--r--   0        0        0     2693 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/scenario.py
+-rw-r--r--   0        0        0     3692 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/abstract/unit.py
+-rw-r--r--   0        0        0      750 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/__init__.py
+-rw-r--r--   0        0        0    13509 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/base.py
+-rw-r--r--   0        0        0     1160 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/docs.py
+-rw-r--r--   0        0        0      255 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/iamc/__init__.py
+-rw-r--r--   0        0        0     1743 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/iamc/datapoint.py
+-rw-r--r--   0        0        0     1589 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/iamc/timeseries.py
+-rw-r--r--   0        0        0     1483 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/iamc/variable.py
+-rw-r--r--   0        0        0     1766 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/meta.py
+-rw-r--r--   0        0        0     1417 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/model.py
+-rw-r--r--   0        0        0      138 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/optimization/__init__.py
+-rw-r--r--   0        0        0      474 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/optimization/column.py
+-rw-r--r--   0        0        0     2086 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/optimization/indexset.py
+-rw-r--r--   0        0        0     2282 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/optimization/scalar.py
+-rw-r--r--   0        0        0     2376 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/optimization/table.py
+-rw-r--r--   0        0        0     1675 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/region.py
+-rw-r--r--   0        0        0     2214 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/run.py
+-rw-r--r--   0        0        0     1470 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/scenario.py
+-rw-r--r--   0        0        0     1593 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/api/unit.py
+-rw-r--r--   0        0        0     3679 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/auth/context.py
+-rw-r--r--   0        0        0     1465 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/auth/decorators.py
+-rw-r--r--   0        0        0      141 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/backend/__init__.py
+-rw-r--r--   0        0        0     6509 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/backend/api.py
+-rw-r--r--   0        0        0     1234 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/backend/base.py
+-rw-r--r--   0        0        0     4761 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/backend/db.py
+-rw-r--r--   0        0        0      874 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/__init__.py
+-rw-r--r--   0        0        0    15233 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/base.py
+-rw-r--r--   0        0        0     3459 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/docs.py
+-rw-r--r--   0        0        0      502 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/__init__.py
+-rw-r--r--   0        0        0      528 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/meta.py
+-rw-r--r--   0        0        0      391 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/model.py
+-rw-r--r--   0        0        0      440 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/optimizationcolumn.py
+-rw-r--r--   0        0        0      448 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/optimizationindexset.py
+-rw-r--r--   0        0        0      581 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/optimizationscalar.py
+-rw-r--r--   0        0        0      436 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/optimizationtable.py
+-rw-r--r--   0        0        0      385 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/region.py
+-rw-r--r--   0        0        0      776 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/run.py
+-rw-r--r--   0        0        0      409 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/scenario.py
+-rw-r--r--   0        0        0      419 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/timeseries.py
+-rw-r--r--   0        0        0      470 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/unit.py
+-rw-r--r--   0        0        0      490 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/filters/variable.py
+-rw-r--r--   0        0        0      331 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/__init__.py
+-rw-r--r--   0        0        0      302 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/base.py
+-rw-r--r--   0        0        0      129 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/datapoint/__init__.py
+-rw-r--r--   0        0        0     5896 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/datapoint/filter.py
+-rw-r--r--   0        0        0     1356 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/datapoint/model.py
+-rw-r--r--   0        0        0     7583 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/datapoint/repository.py
+-rw-r--r--   0        0        0     2917 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/measurand.py
+-rw-r--r--   0        0        0       75 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/timeseries/__init__.py
+-rw-r--r--   0        0        0      401 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/timeseries/filter.py
+-rw-r--r--   0        0        0     1160 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/timeseries/model.py
+-rw-r--r--   0        0        0     4707 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/timeseries/repository.py
+-rw-r--r--   0        0        0       86 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/variable/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/variable/docs.py
+-rw-r--r--   0        0        0      806 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/variable/filter.py
+-rw-r--r--   0        0        0      584 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/variable/model.py
+-rw-r--r--   0        0        0     1444 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/iamc/variable/repository.py
+-rw-r--r--   0        0        0       79 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/meta/__init__.py
+-rw-r--r--   0        0        0      570 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/meta/filter.py
+-rw-r--r--   0        0        0     2246 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/meta/model.py
+-rw-r--r--   0        0        0     7204 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/meta/repository.py
+-rw-r--r--   0        0        0      118 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/model/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/model/docs.py
+-rw-r--r--   0        0        0     1780 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/model/filter.py
+-rw-r--r--   0        0        0      517 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/model/model.py
+-rw-r--r--   0        0        0     1371 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/model/repository.py
+-rw-r--r--   0        0        0      183 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/optimization/__init__.py
+-rw-r--r--   0        0        0      310 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/optimization/base.py
+-rw-r--r--   0        0        0       67 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/optimization/column/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-28 11:26:38.453827 ixmp4-0.9.0/ixmp4/data/db/optimization/column/docs.py
+-rw-r--r--   0        0        0      692 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/column/filter.py
+-rw-r--r--   0        0        0     1170 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/column/model.py
+-rw-r--r--   0        0        0     2440 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/column/repository.py
+-rw-r--r--   0        0        0       71 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/indexset/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/indexset/docs.py
+-rw-r--r--   0        0        0      534 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/indexset/filter.py
+-rw-r--r--   0        0        0     1278 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/indexset/model.py
+-rw-r--r--   0        0        0     2348 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/indexset/repository.py
+-rw-r--r--   0        0        0       67 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/scalar/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/scalar/docs.py
+-rw-r--r--   0        0        0      809 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/scalar/filter.py
+-rw-r--r--   0        0        0     1084 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/scalar/model.py
+-rw-r--r--   0        0        0     2552 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/scalar/repository.py
+-rw-r--r--   0        0        0       65 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/table/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/table/docs.py
+-rw-r--r--   0        0        0      522 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/table/filter.py
+-rw-r--r--   0        0        0     3554 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/table/model.py
+-rw-r--r--   0        0        0     5079 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/optimization/table/repository.py
+-rw-r--r--   0        0        0      121 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/region/__init__.py
+-rw-r--r--   0        0        0      496 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/region/docs.py
+-rw-r--r--   0        0        0     1547 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/region/filter.py
+-rw-r--r--   0        0        0      611 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/region/model.py
+-rw-r--r--   0        0        0     1569 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/region/repository.py
+-rw-r--r--   0        0        0       61 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/run/__init__.py
+-rw-r--r--   0        0        0     1254 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/run/filter.py
+-rw-r--r--   0        0        0     1563 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/run/model.py
+-rw-r--r--   0        0        0     5064 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/run/repository.py
+-rw-r--r--   0        0        0      127 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/scenario/__init__.py
+-rw-r--r--   0        0        0      222 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/scenario/docs.py
+-rw-r--r--   0        0        0     1827 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/scenario/filter.py
+-rw-r--r--   0        0        0      545 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/scenario/model.py
+-rw-r--r--   0        0        0     1814 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/scenario/repository.py
+-rw-r--r--   0        0        0     3331 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/timeseries.py
+-rw-r--r--   0        0        0      126 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/unit/__init__.py
+-rw-r--r--   0        0        0      495 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/unit/docs.py
+-rw-r--r--   0        0        0     1714 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/unit/filter.py
+-rw-r--r--   0        0        0      469 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/unit/model.py
+-rw-r--r--   0        0        0     1725 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/unit/repository.py
+-rw-r--r--   0        0        0      436 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/db/utils.py
+-rw-r--r--   0        0        0     5531 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/generator.py
+-rw-r--r--   0        0        0      292 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/data/types.py
+-rw-r--r--   0        0        0     1585 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/db/__init__.py
+-rw-r--r--   0        0        0     9465 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/db/filters.py
+-rw-r--r--   0        0        0     2408 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/db/migrations/env.py
+-rw-r--r--   0        0        0      509 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/db/migrations/script.py.mako
+-rw-r--r--   0        0        0     5559 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/db/migrations/versions/081bbda6bb7b_create_optimization_table_table.py
+-rw-r--r--   0        0        0     3778 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/db/migrations/versions/97ba231770e2_create_optimization_scalar_table.py
+-rw-r--r--   0        0        0    19022 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/db/migrations/versions/c71efc396d2b_initial_migration.py
+-rw-r--r--   0        0        0     5176 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/db/migrations/versions/da1fba23f206_create_optimization_indexset_table.py
+-rw-r--r--   0        0        0     1478 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/db/utils/__init__.py
+-rw-r--r--   0        0        0     1496 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/db/utils/alembic.py
+-rw-r--r--   0        0        0     1052 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/db/utils/sqlite.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/py.typed
+-rw-r--r--   0        0        0      297 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/__init__.py
+-rw-r--r--   0        0        0     2810 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/__init__.py
+-rw-r--r--   0        0        0     1069 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/base.py
+-rw-r--r--   0        0        0      192 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/decorators.py
+-rw-r--r--   0        0        0     3606 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/deps.py
+-rw-r--r--   0        0        0     6969 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/docs.py
+-rw-r--r--   0        0        0       61 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/iamc/__init__.py
+-rw-r--r--   0        0        0     2550 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/iamc/datapoint.py
+-rw-r--r--   0        0        0      921 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/iamc/model.py
+-rw-r--r--   0        0        0      930 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/iamc/region.py
+-rw-r--r--   0        0        0      948 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/iamc/scenario.py
+-rw-r--r--   0        0        0     1916 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/iamc/timeseries.py
+-rw-r--r--   0        0        0      912 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/iamc/unit.py
+-rw-r--r--   0        0        0     1263 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/iamc/variable.py
+-rw-r--r--   0        0        0     1976 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/meta.py
+-rw-r--r--   0        0        0      696 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/middleware.py
+-rw-r--r--   0        0        0     1185 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/model.py
+-rw-r--r--   0        0        0       38 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/optimization/__init__.py
+-rw-r--r--   0        0        0     1832 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/optimization/indexset.py
+-rw-r--r--   0        0        0     1946 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/optimization/scalar.py
+-rw-r--r--   0        0        0     1928 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/optimization/table.py
+-rw-r--r--   0        0        0     1372 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/region.py
+-rw-r--r--   0        0        0     1621 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/run.py
+-rw-r--r--   0        0        0     1227 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/scenario.py
+-rw-r--r--   0        0        0     1304 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/rest/unit.py
+-rw-r--r--   0        0        0      187 2024-05-28 11:26:38.457827 ixmp4-0.9.0/ixmp4/server/workers.py
+-rw-r--r--   0        0        0     3024 2024-05-28 11:26:54.961589 ixmp4-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 ixmp4-0.9.0/PKG-INFO
```

### Comparing `ixmp4-0.8.3/LICENSE` & `ixmp4-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/README.md` & `ixmp4-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/__init__.py` & `ixmp4-0.9.0/ixmp4/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 from ixmp4.core import Table as Table
 from ixmp4.core.exceptions import InconsistentIamcType as InconsistentIamcType
 from ixmp4.core.exceptions import IxmpError as IxmpError
 from ixmp4.core.exceptions import NotFound as NotFound
 from ixmp4.core.exceptions import NotUnique as NotUnique
 from ixmp4.data.abstract import DataPoint as DataPoint
 
-__version__ = "0.8.3"
-__version_tuple__ = (0, 8, 3)
+__version__ = "0.9.0"
+__version_tuple__ = (0, 9, 0)
```

### Comparing `ixmp4-0.8.3/ixmp4/cli/__init__.py` & `ixmp4-0.9.0/ixmp4/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/cli/platforms.py` & `ixmp4-0.9.0/ixmp4/cli/platforms.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/cli/server.py` & `ixmp4-0.9.0/ixmp4/cli/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,23 +13,26 @@
 app = typer.Typer()
 
 
 @app.command()
 def start(
     host: str = typer.Option(default="127.0.0.1", help="The hostname to bind to."),
     port: int = typer.Option(default=9000, help="Requested server port."),
+    workers: int = typer.Option(default=1, help="How many worker threads to start."),
+    reload: bool = typer.Option(default=False, help="Wether to hot-reload."),
 ) -> None:
     """Starts the ixmp4 web api."""
-    reload = settings.mode != "production"
+    log_config = settings.get_server_logconf()
     uvicorn.run(
         "ixmp4.server:app",
         host=host,
         port=port,
         reload=reload,
-        log_config="ixmp4/conf/logging/server.conf",
+        workers=workers,
+        log_config=str(log_config.absolute()),
     )
 
 
 @app.command()
 def dump_schema(output_file: Optional[typer.FileTextWrite] = typer.Option(None, "-o")):
     schema = get_openapi(
         title=v1.title,
```

### Comparing `ixmp4-0.8.3/ixmp4/conf/auth.py` & `ixmp4-0.9.0/ixmp4/conf/auth.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/conf/credentials.py` & `ixmp4-0.9.0/ixmp4/conf/credentials.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/conf/logging/server.json` & `ixmp4-0.9.0/ixmp4/conf/logging/server.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333334%*

 * *Differences: {"'handlers'": "{'access': {'filename': 'ext://ixmp4.conf.settings.access_file'}, 'debug': "*

 * *               "{'filename': 'ext://ixmp4.conf.settings.debug_file'}, 'error': {'filename': "*

 * *               "'ext://ixmp4.conf.settings.error_file'}}"}*

```diff
@@ -5,36 +5,36 @@
             "datefmt": "%H:%M:%S",
             "format": "[%(levelname)s] %(asctime)s - %(name)s: %(message)s"
         }
     },
     "handlers": {
         "access": {
             "class": "logging.handlers.RotatingFileHandler",
-            "filename": "os.getenv('IXMP4_ACCESS_LOG')",
+            "filename": "ext://ixmp4.conf.settings.access_file",
             "formatter": "generic",
             "level": "INFO",
             "maxBytes": 250000,
             "mode": "a"
         },
         "console": {
             "class": "logging.StreamHandler",
             "formatter": "generic",
             "level": "INFO"
         },
         "debug": {
             "class": "logging.handlers.RotatingFileHandler",
-            "filename": "os.getenv('IXMP4_DEBUG_LOG')",
+            "filename": "ext://ixmp4.conf.settings.debug_file",
             "formatter": "generic",
             "level": "DEBUG",
             "maxBytes": 250000,
             "mode": "a"
         },
         "error": {
             "class": "logging.handlers.RotatingFileHandler",
-            "filename": "os.getenv('IXMP4_ERROR_LOG')",
+            "filename": "ext://ixmp4.conf.settings.error_file",
             "formatter": "generic",
             "level": "WARN",
             "maxBytes": 250000,
             "mode": "a"
         }
     },
     "loggers": {
```

### Comparing `ixmp4-0.8.3/ixmp4/conf/manager.py` & `ixmp4-0.9.0/ixmp4/conf/manager.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/conf/settings.py` & `ixmp4-0.9.0/ixmp4/conf/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import logging
 import logging.config
-import os
 from pathlib import Path
 from typing import Literal
 
 from httpx import ConnectError
 from pydantic import Field, HttpUrl, field_validator
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
@@ -22,25 +21,23 @@
 here = Path(__file__).parent
 
 
 class Settings(BaseSettings):
     mode: Literal["production"] | Literal["development"] | Literal["debug"] = (
         "production"
     )
-    storage_directory: Path = Field(
-        "~/.local/share/ixmp4/", json_schema_extra={"env": "ixmp4_dir"}
-    )
+    storage_directory: Path = Field("~/.local/share/ixmp4/")
     secret_hs256: str = "default_secret_hs256"
     migration_db_uri: str = "sqlite:///./run/db.sqlite"
     manager_url: HttpUrl = Field("https://api.manager.ece.iiasa.ac.at/v1")
     managed: bool = True
     max_page_size: int = 10_000
     default_page_size: int = 5_000
     client_default_upload_chunk_size: int = 10_000
-    client_max_concurrent_requests: int = Field(2, lt=4)
+    client_max_concurrent_requests: int = Field(2, le=4)
     client_max_request_retries: int = Field(3)
     client_backoff_factor: int = Field(5)
     client_timeout: int = Field(30)
     model_config = SettingsConfigDict(env_prefix="ixmp4_", extra="allow")
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
@@ -133,21 +130,21 @@
         self._toml = TomlConfig(toml_config, toml_user)
 
     @field_validator("storage_directory")
     def expand_user(cls, v):
         # translate ~/asdf into /home/user/asdf
         return Path.expanduser(v)
 
+    def get_server_logconf(self):
+        return here / "./logging/server.json"
+
     def configure_logging(self, config: str):
-        access_file = self.log_dir / "access.log"
-        debug_file = self.log_dir / "debug.log"
-        error_file = self.log_dir / "error.log"
-        os.environ.setdefault("IXMP4_ACCESS_LOG", str(access_file.absolute()))
-        os.environ.setdefault("IXMP4_DEBUG_LOG", str(debug_file.absolute()))
-        os.environ.setdefault("IXMP4_ERROR_LOG", str(error_file.absolute()))
+        self.access_file = str((self.log_dir / "access.log").absolute())
+        self.debug_file = str((self.log_dir / "debug.log").absolute())
+        self.error_file = str((self.log_dir / "error.log").absolute())
 
         logging_config = here / f"logging/{config}.json"
         with open(logging_config) as file:
             config_dict = json.load(file)
         logging.config.dictConfig(config_dict)
 
     def check_credentials(self):
```

### Comparing `ixmp4-0.8.3/ixmp4/conf/toml.py` & `ixmp4-0.9.0/ixmp4/conf/toml.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/base.py` & `ixmp4-0.9.0/ixmp4/core/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/decorators.py` & `ixmp4-0.9.0/ixmp4/core/decorators.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/exceptions.py` & `ixmp4-0.9.0/ixmp4/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/iamc/data.py` & `ixmp4-0.9.0/ixmp4/core/iamc/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,23 +9,14 @@
 from ixmp4.data.backend import Backend
 
 from ..base import BaseFacade
 from ..utils import substitute_type
 from .variable import VariableRepository
 
 
-def to_dimensionless(df: pd.DataFrame) -> pd.DataFrame:
-    if "dimensionless" in df.unit:
-        raise ValueError(
-            "Unit name 'dimensionless' is reserved, use an empty string '' instead."
-        )
-    df.replace(to_replace={"unit": ""}, value="dimensionless", inplace=True)
-    return df
-
-
 class RemoveDataPointFrameSchema(pa.DataFrameModel):
     type: Optional[Series[pa.String]] = pa.Field(isin=[t for t in DataPointModel.Type])
     step_year: Optional[Series[pa.Int]] = pa.Field(coerce=True, nullable=True)
     step_datetime: Optional[Series[pa.DateTime]] = pa.Field(coerce=True, nullable=True)
     step_category: Optional[Series[pa.String]] = pa.Field(nullable=True)
 
     region: Optional[Series[pa.String]] = pa.Field(coerce=True)
@@ -65,15 +56,14 @@
         columns += ["subannual"]
     return df[columns + ["value"]]
 
 
 def normalize_df(df: pd.DataFrame, raw: bool, join_runs: bool) -> pd.DataFrame:
     if not df.empty:
         df = df.drop(columns=["time_series__id"])
-        df.unit = df.unit.replace({"dimensionless": ""})
         if raw is False:
             return convert_to_std_format(df, join_runs)
     return df
 
 
 class RunIamcData(BaseFacade):
     """IAMC data.
@@ -116,27 +106,25 @@
 
     def add(
         self,
         df: pd.DataFrame,
         type: Optional[DataPointModel.Type] = None,
     ):
         df = AddDataPointFrameSchema.validate(df)  # type:ignore
-        df = to_dimensionless(df.copy())
         df["run__id"] = self.run.id
         df = self._get_or_create_ts(df)
         substitute_type(df, type)
         self.backend.iamc.datapoints.bulk_upsert(df)
 
     def remove(
         self,
         df: pd.DataFrame,
         type: Optional[DataPointModel.Type] = None,
     ):
         df = RemoveDataPointFrameSchema.validate(df)  # type:ignore
-        df = to_dimensionless(df.copy())
         df["run__id"] = self.run.id
         df = self._get_or_create_ts(df)
         substitute_type(df, type)
         df = df.drop(columns=["unit", "variable", "region"])
         self.backend.iamc.datapoints.bulk_delete(df)
 
     def tabulate(
```

### Comparing `ixmp4-0.8.3/ixmp4/core/iamc/variable.py` & `ixmp4-0.9.0/ixmp4/core/iamc/variable.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/model.py` & `ixmp4-0.9.0/ixmp4/core/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/optimization/data.py` & `ixmp4-0.9.0/ixmp4/core/optimization/data.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/optimization/indexset.py` & `ixmp4-0.9.0/ixmp4/core/optimization/indexset.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/optimization/scalar.py` & `ixmp4-0.9.0/ixmp4/core/optimization/scalar.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,16 +103,16 @@
     def create(self, name: str, value: float, unit: str | Unit | None = None) -> Scalar:
         if isinstance(unit, Unit):
             unit_name = unit.name
         elif isinstance(unit, str):
             unit_name = unit
         else:
             # TODO: provide logging information about None-units being converted
-            # to dimensionless
-            dimensionless_unit = self.backend.units.create(name="dimensionless")
+            # if unit is None, assume that this is a dimensionless scalar (unit = "")
+            dimensionless_unit = self.backend.units.create(name="")
             unit_name = dimensionless_unit.name
 
         try:
             model = self.backend.optimization.scalars.create(
                 name=name, value=value, unit_name=unit_name, run_id=self._run.id
             )
         except Scalar.NotUnique as e:
```

### Comparing `ixmp4-0.8.3/ixmp4/core/optimization/table.py` & `ixmp4-0.9.0/ixmp4/core/optimization/table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/platform.py` & `ixmp4-0.9.0/ixmp4/core/platform.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/region.py` & `ixmp4-0.9.0/ixmp4/core/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/run.py` & `ixmp4-0.9.0/ixmp4/core/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/scenario.py` & `ixmp4-0.9.0/ixmp4/core/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/core/unit.py` & `ixmp4-0.9.0/ixmp4/core/unit.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,14 @@
 import pandas as pd
 
 from ixmp4.core.base import BaseFacade, BaseModelFacade
 from ixmp4.data.abstract import Docs as DocsModel
 from ixmp4.data.abstract import Unit as UnitModel
 
 
-def to_dimensionless(name):
-    if name == "dimensionless":
-        raise ValueError(
-            "Unit name 'dimensionless' is reserved, use an empty string '' instead."
-        )
-    return "dimensionless" if name == "" else name
-
-
 class Unit(BaseModelFacade):
     _model: UnitModel
     NotUnique = UnitModel.NotUnique
     NotFound = UnitModel.NotFound
     DeletionPrevented = UnitModel.DeletionPrevented
 
     @property
@@ -67,18 +59,20 @@
 
 
 class UnitRepository(BaseFacade):
     def create(
         self,
         name: str,
     ) -> Unit:
-        name = to_dimensionless(name)
-        if name.strip() == "":
+        if name != "" and name.strip() == "":
             raise ValueError("Using a space-only unit name is not allowed.")
-
+        if name == "dimensionless":
+            raise ValueError(
+                "Unit name 'dimensionless' is reserved, use an empty string '' instead."
+            )
         model = self.backend.units.create(name)
         return Unit(_backend=self.backend, _model=model)
 
     def delete(self, x: Unit | int | str):
         if isinstance(x, Unit):
             id = x.id
         elif isinstance(x, int):
@@ -88,15 +82,15 @@
             id = model.id
         else:
             raise TypeError("Invalid argument: Must be `Unit`, `int` or `str`.")
 
         self.backend.units.delete(id)
 
     def get(self, name: str) -> Unit:
-        model = self.backend.units.get(to_dimensionless(name))
+        model = self.backend.units.get(name)
         return Unit(_backend=self.backend, _model=model)
 
     def list(self, name: str | None = None) -> list[Unit]:
         units = self.backend.units.list(name=name)
         return [Unit(_backend=self.backend, _model=u) for u in units]
 
     def tabulate(self, name: str | None = None) -> pd.DataFrame:
```

### Comparing `ixmp4-0.8.3/ixmp4/core/utils.py` & `ixmp4-0.9.0/ixmp4/core/utils.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/__init__.py` & `ixmp4-0.9.0/ixmp4/data/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/base.py` & `ixmp4-0.9.0/ixmp4/data/abstract/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/docs.py` & `ixmp4-0.9.0/ixmp4/data/abstract/docs.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/iamc/datapoint.py` & `ixmp4-0.9.0/ixmp4/data/abstract/iamc/datapoint.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/iamc/measurand.py` & `ixmp4-0.9.0/ixmp4/data/abstract/iamc/measurand.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/iamc/timeseries.py` & `ixmp4-0.9.0/ixmp4/data/abstract/iamc/timeseries.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/iamc/variable.py` & `ixmp4-0.9.0/ixmp4/data/abstract/iamc/variable.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/meta.py` & `ixmp4-0.9.0/ixmp4/data/abstract/meta.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/model.py` & `ixmp4-0.9.0/ixmp4/data/abstract/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/optimization/column.py` & `ixmp4-0.9.0/ixmp4/data/abstract/optimization/column.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/optimization/indexset.py` & `ixmp4-0.9.0/ixmp4/data/abstract/optimization/indexset.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/optimization/scalar.py` & `ixmp4-0.9.0/ixmp4/data/abstract/optimization/scalar.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/optimization/table.py` & `ixmp4-0.9.0/ixmp4/data/abstract/optimization/table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/region.py` & `ixmp4-0.9.0/ixmp4/data/abstract/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/run.py` & `ixmp4-0.9.0/ixmp4/data/abstract/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/scenario.py` & `ixmp4-0.9.0/ixmp4/data/abstract/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/abstract/unit.py` & `ixmp4-0.9.0/ixmp4/data/abstract/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/__init__.py` & `ixmp4-0.9.0/ixmp4/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/base.py` & `ixmp4-0.9.0/ixmp4/data/api/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import asyncio
 import logging
+import time
+from concurrent import futures
 from json.decoder import JSONDecodeError
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
-    Coroutine,
     Generic,
     Type,
     TypeVar,
 )
 
 import httpx
 import pandas as pd
@@ -122,89 +122,84 @@
         except KeyError:
             raise ImproperlyConfigured(
                 "Could not find remote exception in registry. "
                 "Are you sure client and server ixmp versions are compatible?"
             )
         return exc.from_dict(json)
 
-    def _request(self, *args, **kwargs) -> dict | list | None:
-        res = asyncio.run(self._async_request(*args, **kwargs))
-        return res
-
-    async def _async_request(
+    def _request(
         self,
         method: str,
         path: str,
         params: dict | None = None,
         json: dict | None = None,
         max_retries: int = settings.client_max_request_retries,
         **kwargs,
     ) -> dict | list | None:
-        """Sends an asyncronous request and handles potential error responses.
-        Uses the backend's semaphore to limit how many
-        requests are sent concurrently per backend.
+        """Sends a request and handles potential error responses.
         Re-raises a remote `IxmpError` if thrown and transferred from the backend.
-        Handles read timeouts and rate limiting responses
-        via retries with exponential backoffs.
+        Handles read timeouts and rate limiting responses via retries with backoffs.
         Returns `None` if the response body is empty
         but has a status code less than 300.
         """
 
-        async def retry(max_retries=max_retries) -> dict | list | None:
+        def retry(max_retries=max_retries) -> dict | list | None:
             if max_retries == 0:
-                self.backend.semaphore
                 logger.error(f"API Encumbered: '{self.backend.info.dsn}'")
                 raise ApiEncumbered(
                     f"The service connected to the backend '{self.backend.info.name}' "
                     "is currently overencumbered with requests. "
                     "Try again at a later time or re-configure your client "
                     "to behave more leniently."
                 )
             # increase backoff by `settings.client_backoff_factor`
             # for each retry
             backoff_s = settings.client_backoff_factor * (
                 settings.client_max_request_retries - max_retries
             )
             logger.debug(f"Retrying request in {backoff_s} seconds.")
-            await asyncio.sleep(backoff_s)
-            return await self._async_request(
+            time.sleep(backoff_s)
+            return self._request(
                 method,
                 path,
                 params=params,
                 json=json,
                 max_retries=max_retries - 1,
                 **kwargs,
             )
 
         if params is None:
             params = {}
         else:
             params = self.sanitize_params(params)
 
         try:
-            async with self.backend.semaphore:
-                res = await self.backend.async_client.request(
-                    method, path, params=params, json=json, **kwargs
-                )
+            res = self.backend.client.request(
+                method,
+                path,
+                params=params,
+                json=json,
+                **kwargs,
+            )
         except httpx.ReadTimeout:
             logger.warn("Read timeout, retrying request...")
-            return await retry()
+            return retry()
 
-        return await self._async_handle_response(res, retry)
+        return self._handle_response(res, retry)
 
-    async def _async_handle_response(
+    def _handle_response(
         self,
         res: httpx.Response,
-        retry: Callable[..., Coroutine[Any, Any, dict | list | None]],
+        retry: Callable[..., dict | list | None],
     ) -> dict | list | None:
         if res.status_code in [
             429,  # Too Many Requests
             420,  # Enhance Your Calm
         ]:
-            return await retry()
+            return retry()
         elif res.status_code >= 400:
             if res.status_code == 413:
                 raise ImproperlyConfigured(
                     "Received status code 413 (Payload Too Large). "
                     "Consider decreasing `IXMP4_CLIENT_DEFAULT_UPLOAD_CHUNK_SIZE` "
                     f"(current: {settings.client_default_upload_chunk_size})."
                 )
@@ -236,44 +231,41 @@
         return self._request(
             self.enumeration_method,
             self.prefix,
             params={**params, "table": table},
             json=json,
         )
 
-    def _build_pagination_requests(
+    def _dispatch_pagination_requests(
         self,
         total: int,
         start: int,
         limit: int,
         params: dict | None,
         json: dict | None,
-    ) -> list[Coroutine]:
-        requests: list[Coroutine] = []
+    ) -> list[list | dict]:
+        """Uses the backends executor to send many pagination requests concurrently."""
+        requests: list[futures.Future] = []
         for req_offset in range(start, total, limit):
             if params is not None:
                 req_params = params.copy()
             else:
                 req_params = {}
 
             req_params.update({"limit": limit, "offset": req_offset})
-            request = self._async_request(
+            futu = self.backend.executor.submit(
+                self._request,
                 self.enumeration_method,
                 self.prefix,
                 params=req_params,
                 json=json,
             )
-            requests.append(request)
-        return requests
-
-    def _collect_pagination_results(self, requests: list[Coroutine]) -> list:
-        async def gather():
-            return await asyncio.gather(*requests)
-
-        responses = asyncio.run(gather())
+            requests.append(futu)
+        results = futures.wait(requests)
+        responses = [f.result() for f in results.done]
         return [r.pop("results") for r in responses]
 
     def _handle_pagination(
         self,
         data: dict,
         table: bool = False,
         params: dict | None = None,
@@ -290,18 +282,17 @@
         total = data.pop("total")
         pagination = data.pop("pagination")
         offset = pagination.pop("offset")
         limit = pagination.pop("limit")
         if total <= offset + limit:
             return [data.pop("results")]
         else:
-            requests = self._build_pagination_requests(
+            results = self._dispatch_pagination_requests(
                 total, offset + limit, limit, params, json
             )
-            results = self._collect_pagination_results(requests)
             return [data.pop("results")] + results
 
     def _list(
         self, params: dict | None = None, json: dict | None = None, **kwargs
     ) -> list[ModelType]:
         data = self._request_enumeration(params=params, table=False, json=json)
         if isinstance(data, dict):
```

### Comparing `ixmp4-0.8.3/ixmp4/data/api/docs.py` & `ixmp4-0.9.0/ixmp4/data/api/docs.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/iamc/datapoint.py` & `ixmp4-0.9.0/ixmp4/data/api/iamc/datapoint.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/iamc/timeseries.py` & `ixmp4-0.9.0/ixmp4/data/api/iamc/timeseries.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/iamc/variable.py` & `ixmp4-0.9.0/ixmp4/data/api/iamc/variable.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/meta.py` & `ixmp4-0.9.0/ixmp4/data/api/meta.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/model.py` & `ixmp4-0.9.0/ixmp4/data/api/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/optimization/indexset.py` & `ixmp4-0.9.0/ixmp4/data/api/optimization/indexset.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/optimization/scalar.py` & `ixmp4-0.9.0/ixmp4/data/api/optimization/scalar.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/optimization/table.py` & `ixmp4-0.9.0/ixmp4/data/api/optimization/table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/region.py` & `ixmp4-0.9.0/ixmp4/data/api/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/run.py` & `ixmp4-0.9.0/ixmp4/data/api/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/scenario.py` & `ixmp4-0.9.0/ixmp4/data/api/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/api/unit.py` & `ixmp4-0.9.0/ixmp4/data/api/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/auth/context.py` & `ixmp4-0.9.0/ixmp4/data/auth/context.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/auth/decorators.py` & `ixmp4-0.9.0/ixmp4/data/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/backend/api.py` & `ixmp4-0.9.0/ixmp4/data/backend/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import asyncio
 import logging
+from concurrent.futures import ThreadPoolExecutor
 
 import httpx
 import pandas as pd
 from fastapi.testclient import TestClient
 
 from ixmp4.conf import settings
 from ixmp4.conf.auth import BaseAuth, SelfSignedAuth, User
@@ -30,31 +30,31 @@
 
 logger = logging.getLogger(__name__)
 
 
 class RestBackend(Backend):
     client: httpx.Client
     async_client: httpx.AsyncClient
-    semaphore: asyncio.Semaphore
+    executor: ThreadPoolExecutor
     timeout: httpx.Timeout
 
     def __init__(
         self,
         info: PlatformInfo,
         auth: BaseAuth | None = None,
         max_concurrent_requests: int = settings.client_max_concurrent_requests,
     ) -> None:
         super().__init__(info)
-        logger.info(f"Connecting to IXMP4 REST API at {info.dsn}.")
-        self.semaphore = asyncio.Semaphore(max_concurrent_requests)
+        logger.debug(f"Connecting to IXMP4 REST API at {info.dsn}.")
+        self.executor = ThreadPoolExecutor(max_workers=max_concurrent_requests)
         self.timeout = httpx.Timeout(settings.client_timeout, connect=60.0)
+        self.make_client(info.dsn, auth=auth)
         if isinstance(info, ManagerPlatformInfo):
             if info.notice is not None:
-                logger.info("Platform notice: " + info.notice)
-        self.make_client(info.dsn, auth=auth)
+                logger.info("Platform notice: >\n" + info.notice)
         self.create_repositories()
 
     def make_client(self, rest_url: str, auth: BaseAuth | None):
         auth = self.get_auth(rest_url, auth)
 
         self.client = httpx.Client(
             base_url=rest_url,
@@ -76,16 +76,23 @@
     def get_auth(self, rest_url: str, override_auth: BaseAuth | None) -> BaseAuth:
         root = httpx.get(rest_url, follow_redirects=True)
         if root.status_code != 200:
             logger.error("Root API response not OK: " + root.text)
             raise UnknownApiError(f"Server response not OK. ({root.status_code})")
 
         api_info = APIInfo(**root.json())
-        logger.info(f"Connected to Platform '{api_info.name}'")
-        logger.info("Server IXMP4 Version: " + api_info.version)
+        logger.info(f"Connected to IXMP4 Platform '{api_info.name}'")
+
+        import ixmp4
+
+        if ixmp4.__version__ != api_info.version:
+            logger.warning(
+                "IXMP4 Client and Server versions do not match. "
+                f"(Client: {ixmp4.__version__}, Server: {api_info.version})"
+            )
 
         logger.debug("Server UTC Time: " + api_info.utcnow.strftime("%c"))
         logger.debug("Server Is Managed: " + str(api_info.is_managed))
         if api_info.manager_url is not None:
             if (
                 api_info.manager_url.rstrip("/")
                 != str(settings.manager_url).rstrip("/")
@@ -170,7 +177,8 @@
         )
         v1.dependency_overrides[deps.get_backend] = deps.get_test_backend_dependency(
             self.db_backend, self.auth_params
         )
 
     def close(self):
         self.client.close()
+        self.executor.shutdown(cancel_futures=True)
```

### Comparing `ixmp4-0.8.3/ixmp4/data/backend/base.py` & `ixmp4-0.9.0/ixmp4/data/backend/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/backend/db.py` & `ixmp4-0.9.0/ixmp4/data/backend/db.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/__init__.py` & `ixmp4-0.9.0/ixmp4/data/db/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/base.py` & `ixmp4-0.9.0/ixmp4/data/db/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/docs.py` & `ixmp4-0.9.0/ixmp4/data/db/docs.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/filters/meta.py` & `ixmp4-0.9.0/ixmp4/data/db/filters/meta.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/filters/optimizationscalar.py` & `ixmp4-0.9.0/ixmp4/data/db/filters/optimizationscalar.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/filters/run.py` & `ixmp4-0.9.0/ixmp4/data/db/filters/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/iamc/datapoint/filter.py` & `ixmp4-0.9.0/ixmp4/data/db/iamc/datapoint/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/iamc/datapoint/model.py` & `ixmp4-0.9.0/ixmp4/data/db/iamc/datapoint/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/iamc/datapoint/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/iamc/datapoint/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/iamc/measurand.py` & `ixmp4-0.9.0/ixmp4/data/db/iamc/measurand.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/iamc/timeseries/model.py` & `ixmp4-0.9.0/ixmp4/data/db/iamc/timeseries/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/iamc/timeseries/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/iamc/timeseries/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/iamc/variable/filter.py` & `ixmp4-0.9.0/ixmp4/data/db/iamc/variable/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/iamc/variable/model.py` & `ixmp4-0.9.0/ixmp4/data/db/iamc/variable/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/iamc/variable/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/iamc/variable/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/meta/filter.py` & `ixmp4-0.9.0/ixmp4/data/db/meta/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/meta/model.py` & `ixmp4-0.9.0/ixmp4/data/db/meta/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/meta/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/meta/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/model/filter.py` & `ixmp4-0.9.0/ixmp4/data/db/model/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/model/model.py` & `ixmp4-0.9.0/ixmp4/data/db/model/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/model/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/model/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/optimization/column/filter.py` & `ixmp4-0.9.0/ixmp4/data/db/optimization/column/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/optimization/column/model.py` & `ixmp4-0.9.0/ixmp4/data/db/optimization/column/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/optimization/column/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/optimization/column/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/optimization/indexset/filter.py` & `ixmp4-0.9.0/ixmp4/data/db/optimization/indexset/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/optimization/indexset/model.py` & `ixmp4-0.9.0/ixmp4/data/db/optimization/indexset/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/optimization/indexset/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/optimization/indexset/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/optimization/scalar/filter.py` & `ixmp4-0.9.0/ixmp4/data/db/optimization/scalar/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/optimization/scalar/model.py` & `ixmp4-0.9.0/ixmp4/data/db/optimization/scalar/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/optimization/scalar/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/optimization/scalar/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/optimization/table/filter.py` & `ixmp4-0.9.0/ixmp4/data/db/optimization/table/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/optimization/table/model.py` & `ixmp4-0.9.0/ixmp4/data/db/optimization/table/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/optimization/table/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/optimization/table/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/region/filter.py` & `ixmp4-0.9.0/ixmp4/data/db/region/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/region/model.py` & `ixmp4-0.9.0/ixmp4/data/db/region/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/region/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/region/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/run/filter.py` & `ixmp4-0.9.0/ixmp4/data/db/run/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/run/model.py` & `ixmp4-0.9.0/ixmp4/data/db/run/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/run/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/run/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/scenario/filter.py` & `ixmp4-0.9.0/ixmp4/data/db/scenario/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/scenario/model.py` & `ixmp4-0.9.0/ixmp4/data/db/scenario/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/scenario/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/scenario/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/timeseries.py` & `ixmp4-0.9.0/ixmp4/data/db/timeseries.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/unit/filter.py` & `ixmp4-0.9.0/ixmp4/data/db/unit/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/db/unit/repository.py` & `ixmp4-0.9.0/ixmp4/data/db/unit/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/data/generator.py` & `ixmp4-0.9.0/ixmp4/data/generator.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/db/__init__.py` & `ixmp4-0.9.0/ixmp4/db/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/db/filters.py` & `ixmp4-0.9.0/ixmp4/db/filters.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/db/migrations/env.py` & `ixmp4-0.9.0/ixmp4/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/db/migrations/versions/081bbda6bb7b_create_optimization_table_table.py` & `ixmp4-0.9.0/ixmp4/db/migrations/versions/081bbda6bb7b_create_optimization_table_table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/db/migrations/versions/97ba231770e2_create_optimization_scalar_table.py` & `ixmp4-0.9.0/ixmp4/db/migrations/versions/97ba231770e2_create_optimization_scalar_table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/db/migrations/versions/c71efc396d2b_initial_migration.py` & `ixmp4-0.9.0/ixmp4/db/migrations/versions/c71efc396d2b_initial_migration.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/db/migrations/versions/da1fba23f206_create_optimization_indexset_table.py` & `ixmp4-0.9.0/ixmp4/db/migrations/versions/da1fba23f206_create_optimization_indexset_table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/db/utils/__init__.py` & `ixmp4-0.9.0/ixmp4/db/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/db/utils/alembic.py` & `ixmp4-0.9.0/ixmp4/db/utils/alembic.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/db/utils/sqlite.py` & `ixmp4-0.9.0/ixmp4/db/utils/sqlite.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/__init__.py` & `ixmp4-0.9.0/ixmp4/server/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/base.py` & `ixmp4-0.9.0/ixmp4/server/rest/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/deps.py` & `ixmp4-0.9.0/ixmp4/server/rest/deps.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/docs.py` & `ixmp4-0.9.0/ixmp4/server/rest/docs.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/iamc/datapoint.py` & `ixmp4-0.9.0/ixmp4/server/rest/iamc/datapoint.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/iamc/model.py` & `ixmp4-0.9.0/ixmp4/server/rest/iamc/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/iamc/region.py` & `ixmp4-0.9.0/ixmp4/server/rest/iamc/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/iamc/scenario.py` & `ixmp4-0.9.0/ixmp4/server/rest/iamc/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/iamc/timeseries.py` & `ixmp4-0.9.0/ixmp4/server/rest/iamc/timeseries.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/iamc/unit.py` & `ixmp4-0.9.0/ixmp4/server/rest/iamc/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/iamc/variable.py` & `ixmp4-0.9.0/ixmp4/server/rest/iamc/variable.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/meta.py` & `ixmp4-0.9.0/ixmp4/server/rest/meta.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/middleware.py` & `ixmp4-0.9.0/ixmp4/server/rest/middleware.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/model.py` & `ixmp4-0.9.0/ixmp4/server/rest/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/optimization/indexset.py` & `ixmp4-0.9.0/ixmp4/server/rest/optimization/indexset.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/optimization/scalar.py` & `ixmp4-0.9.0/ixmp4/server/rest/optimization/scalar.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/optimization/table.py` & `ixmp4-0.9.0/ixmp4/server/rest/optimization/table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/region.py` & `ixmp4-0.9.0/ixmp4/server/rest/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/run.py` & `ixmp4-0.9.0/ixmp4/server/rest/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/scenario.py` & `ixmp4-0.9.0/ixmp4/server/rest/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/ixmp4/server/rest/unit.py` & `ixmp4-0.9.0/ixmp4/server/rest/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.3/pyproject.toml` & `ixmp4-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors = [
     "Max Wolschlager <wolschlager@iiasa.ac.at>",
     "Fridolin Glatter <glatter@iiasa.ac.at>",
     "Daniel Huppmann <huppmann@iiasa.ac.at>",
     "Philip Hackstock <hackstock@iiasa.ac.at>",
 ]
 name = "ixmp4"
-version = "0.8.3"
+version = "0.9.0"
 description = "a data warehouse for scenario analysis"
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "ixmp4" }, { include = "ixmp4/py.typed" }]
 homepage = "https://software.ece.iiasa.ac.at"
 repository = "https://github.com/iiasa/ixmp4"
 documentation = "https://docs.ece.iiasa.ac.at/projects/ixmp4"
@@ -45,15 +45,14 @@
 sphinxcontrib-bibtex = ">=2.6.1"
 sphinxcontrib-openapi = ">=0.8.1"
 
 [tool.poetry.group.server]
 optional = true
 
 [tool.poetry.group.server.dependencies]
-gunicorn = ">=21.2.0"
 uvicorn = { extras = ["standard"], version = ">=0.24.0" }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 build = ">=1.0.3"
```

### Comparing `ixmp4-0.8.3/PKG-INFO` & `ixmp4-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixmp4
-Version: 0.8.3
+Version: 0.9.0
 Summary: a data warehouse for scenario analysis
 Home-page: https://software.ece.iiasa.ac.at
 License: MIT
 Author: Max Wolschlager
 Author-email: wolschlager@iiasa.ac.at
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

