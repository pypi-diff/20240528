# Comparing `tmp/phdi-1.2.9.tar.gz` & `tmp/phdi-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdi-1.2.9.tar", max compression
+gzip compressed data, was "phdi-1.4.0.tar", max compression
```

## Comparing `phdi-1.2.9.tar` & `phdi-1.4.0.tar`

### file list

```diff
@@ -1,72 +1,71 @@
--rw-r--r--   0        0        0     7048 2024-03-14 20:05:39.529269 phdi-1.2.9/LICENSE.md
--rw-r--r--   0        0        0    11872 2024-03-14 20:05:39.529269 phdi-1.2.9/README.md
--rw-r--r--   0        0        0       22 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/__init__.py
--rw-r--r--   0        0        0      223 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/cloud/README.md
--rw-r--r--   0        0        0        0 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/cloud/__init__.py
--rw-r--r--   0        0        0     9679 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/cloud/azure.py
--rw-r--r--   0        0        0     2549 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/cloud/core.py
--rw-r--r--   0        0        0     6073 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/cloud/gcp.py
--rw-r--r--   0        0        0      163 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/containers/README.md
--rw-r--r--   0        0        0        0 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/containers/__init__.py
--rw-r--r--   0        0        0     3686 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/containers/base_service.py
--rw-r--r--   0        0        0        0 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/__init__.py
--rw-r--r--   0        0        0      292 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/cloud/README.md
--rw-r--r--   0        0        0      119 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/cloud/__init__.py
--rw-r--r--   0        0        0     2147 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/cloud/azure.py
--rw-r--r--   0        0        0      311 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/conversion/README.md
--rw-r--r--   0        0        0      183 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/conversion/__init__.py
--rw-r--r--   0        0        0    12626 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/conversion/convert.py
--rw-r--r--   0        0        0      808 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/geospatial/README.md
--rw-r--r--   0        0        0      294 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/geospatial/__init__.py
--rw-r--r--   0        0        0     3494 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/geospatial/census.py
--rw-r--r--   0        0        0     4536 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/geospatial/core.py
--rw-r--r--   0        0        0     3710 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/geospatial/smarty.py
--rw-r--r--   0        0        0      890 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/harmonization/README.md
--rw-r--r--   0        0        0      514 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/harmonization/__init__.py
--rw-r--r--   0        0        0    11967 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/harmonization/standardization.py
--rw-r--r--   0        0        0      200 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/linkage/__init__.py
--rw-r--r--   0        0        0     3629 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/linkage/link.py
--rw-r--r--   0        0        0      412 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/tabulation/README.md
--rw-r--r--   0        0        0      498 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/tabulation/__init__.py
--rw-r--r--   0        0        0    27573 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/tabulation/tables.py
--rw-r--r--   0        0        0      397 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/transport/README.md
--rw-r--r--   0        0        0      381 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/transport/__init__.py
--rw-r--r--   0        0        0     7384 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/transport/export.py
--rw-r--r--   0        0        0     8853 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/transport/http.py
--rw-r--r--   0        0        0     7085 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/fhir/utils.py
--rw-r--r--   0        0        0      881 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/geospatial/README.md
--rw-r--r--   0        0        0      323 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/geospatial/__init__.py
--rw-r--r--   0        0        0     9345 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/geospatial/census.py
--rw-r--r--   0        0        0     2748 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/geospatial/core.py
--rw-r--r--   0        0        0     6061 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/geospatial/smarty.py
--rw-r--r--   0        0        0     1027 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/harmonization/README.md
--rw-r--r--   0        0        0     1138 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/harmonization/__init__.py
--rw-r--r--   0        0        0    28162 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/harmonization/double_metaphone.py
--rw-r--r--   0        0        0    10909 2024-03-14 20:05:40.113271 phdi-1.2.9/phdi/harmonization/hl7.py
--rw-r--r--   0        0        0    36359 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/harmonization/phdi_nicknames.csv
--rw-r--r--   0        0        0    12037 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/harmonization/standardization.py
--rw-r--r--   0        0        0     1953 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/harmonization/utils.py
--rw-r--r--   0        0        0      255 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/linkage/README.md
--rw-r--r--   0        0        0     2513 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/linkage/__init__.py
--rw-r--r--   0        0        0     2555 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/linkage/algorithms.py
--rw-r--r--   0        0        0      641 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/linkage/config.py
--rw-r--r--   0        0        0     1897 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/linkage/core.py
--rw-r--r--   0        0        0    17169 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/linkage/dal.py
--rw-r--r--   0        0        0    63295 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/linkage/link.py
--rw-r--r--   0        0        0    28096 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/linkage/mpi.py
--rw-r--r--   0        0        0     3092 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/linkage/new_tables.ddl
--rw-r--r--   0        0        0     3922 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/linkage/seed.py
--rw-r--r--   0        0        0      399 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/linkage/tables.ddl
--rw-r--r--   0        0        0     3421 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/linkage/utils.py
--rw-r--r--   0        0        0      225 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/tabulation/README.md
--rw-r--r--   0        0        0      202 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/tabulation/__init__.py
--rw-r--r--   0        0        0    11879 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/tabulation/tables.py
--rw-r--r--   0        0        0     2046 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/tabulation/validation_schema.json
--rw-r--r--   0        0        0      225 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/transport/README.md
--rw-r--r--   0        0        0       81 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/transport/__init__.py
--rw-r--r--   0        0        0     2352 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/transport/http.py
--rw-r--r--   0        0        0     1825 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/validation/__init__.py
--rw-r--r--   0        0        0     6342 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/validation/validation.py
--rw-r--r--   0        0        0    17871 2024-03-14 20:05:40.117271 phdi-1.2.9/phdi/validation/xml_utils.py
--rw-r--r--   0        0        0     1969 2024-03-14 20:05:40.121271 phdi-1.2.9/pyproject.toml
--rw-r--r--   0        0        0    13671 1970-01-01 00:00:00.000000 phdi-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0     7048 2024-05-28 21:15:25.375841 phdi-1.4.0/LICENSE.md
+-rw-r--r--   0        0        0    12239 2024-05-28 21:15:25.375841 phdi-1.4.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/cloud/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/cloud/__init__.py
+-rw-r--r--   0        0        0     9679 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/cloud/azure.py
+-rw-r--r--   0        0        0     2549 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/cloud/core.py
+-rw-r--r--   0        0        0     6073 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/cloud/gcp.py
+-rw-r--r--   0        0        0      163 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/containers/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/containers/__init__.py
+-rw-r--r--   0        0        0     3685 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/containers/base_service.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/fhir/__init__.py
+-rw-r--r--   0        0        0      292 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/fhir/cloud/README.md
+-rw-r--r--   0        0        0      119 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/fhir/cloud/__init__.py
+-rw-r--r--   0        0        0     2147 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/fhir/cloud/azure.py
+-rw-r--r--   0        0        0      311 2024-05-28 21:15:26.059850 phdi-1.4.0/phdi/fhir/conversion/README.md
+-rw-r--r--   0        0        0      183 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/conversion/__init__.py
+-rw-r--r--   0        0        0    12623 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/conversion/convert.py
+-rw-r--r--   0        0        0      808 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/geospatial/README.md
+-rw-r--r--   0        0        0      294 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/geospatial/__init__.py
+-rw-r--r--   0        0        0     3494 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/geospatial/census.py
+-rw-r--r--   0        0        0     4536 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/geospatial/core.py
+-rw-r--r--   0        0        0     3710 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/geospatial/smarty.py
+-rw-r--r--   0        0        0      890 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/harmonization/README.md
+-rw-r--r--   0        0        0      514 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/harmonization/__init__.py
+-rw-r--r--   0        0        0    11967 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/harmonization/standardization.py
+-rw-r--r--   0        0        0      200 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/linkage/__init__.py
+-rw-r--r--   0        0        0     3629 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/linkage/link.py
+-rw-r--r--   0        0        0      412 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/tabulation/README.md
+-rw-r--r--   0        0        0      498 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/tabulation/__init__.py
+-rw-r--r--   0        0        0    27573 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/tabulation/tables.py
+-rw-r--r--   0        0        0      397 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/transport/README.md
+-rw-r--r--   0        0        0      381 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/transport/__init__.py
+-rw-r--r--   0        0        0     7384 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/transport/export.py
+-rw-r--r--   0        0        0     8853 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/transport/http.py
+-rw-r--r--   0        0        0     7093 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/fhir/utils.py
+-rw-r--r--   0        0        0      881 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/geospatial/README.md
+-rw-r--r--   0        0        0      323 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/geospatial/__init__.py
+-rw-r--r--   0        0        0     9349 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/geospatial/census.py
+-rw-r--r--   0        0        0     2748 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/geospatial/core.py
+-rw-r--r--   0        0        0     6061 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/geospatial/smarty.py
+-rw-r--r--   0        0        0     1027 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/harmonization/README.md
+-rw-r--r--   0        0        0     1138 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/harmonization/__init__.py
+-rw-r--r--   0        0        0    28162 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/harmonization/double_metaphone.py
+-rw-r--r--   0        0        0    10909 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/harmonization/hl7.py
+-rw-r--r--   0        0        0    36359 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/harmonization/phdi_nicknames.csv
+-rw-r--r--   0        0        0    12036 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/harmonization/standardization.py
+-rw-r--r--   0        0        0     1953 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/harmonization/utils.py
+-rw-r--r--   0        0        0      255 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/linkage/README.md
+-rw-r--r--   0        0        0     2407 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/linkage/__init__.py
+-rw-r--r--   0        0        0     2555 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/linkage/algorithms.py
+-rw-r--r--   0        0        0      641 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/linkage/config.py
+-rw-r--r--   0        0        0     1935 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/linkage/core.py
+-rw-r--r--   0        0        0    17168 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/linkage/dal.py
+-rw-r--r--   0        0        0    63007 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/linkage/link.py
+-rw-r--r--   0        0        0    29430 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/linkage/mpi.py
+-rw-r--r--   0        0        0     3092 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/linkage/new_tables.ddl
+-rw-r--r--   0        0        0     3922 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/linkage/seed.py
+-rw-r--r--   0        0        0     3421 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/linkage/utils.py
+-rw-r--r--   0        0        0      225 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/tabulation/README.md
+-rw-r--r--   0        0        0      202 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/tabulation/__init__.py
+-rw-r--r--   0        0        0    11883 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/tabulation/tables.py
+-rw-r--r--   0        0        0     2046 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/tabulation/validation_schema.json
+-rw-r--r--   0        0        0      225 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/transport/README.md
+-rw-r--r--   0        0        0       81 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/transport/__init__.py
+-rw-r--r--   0        0        0     2352 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/transport/http.py
+-rw-r--r--   0        0        0     1825 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/validation/__init__.py
+-rw-r--r--   0        0        0     6341 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/validation/validation.py
+-rw-r--r--   0        0        0    17870 2024-05-28 21:15:26.063850 phdi-1.4.0/phdi/validation/xml_utils.py
+-rw-r--r--   0        0        0     2669 2024-05-28 21:15:26.071850 phdi-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    14079 1970-01-01 00:00:00.000000 phdi-1.4.0/PKG-INFO
```

### Comparing `phdi-1.2.9/LICENSE.md` & `phdi-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/README.md` & `phdi-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # PRIME Public Health Data Infrastructure (PHDI)
-[![Test github badge](https://github.com/CDCgov/phdi/actions/workflows/test.yaml/badge.svg)](https://github.com/CDCgov/phdi/actions/workflows/test.yaml)
 [![codecov](https://codecov.io/gh/CDCgov/phdi/branch/main/graph/badge.svg)](https://codecov.io/gh/CDCgov/phdi)
-- [PRIME Public Health Data Infrastructure](#prime-public-health-data-infrastructure)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Test github badge](https://github.com/CDCgov/phdi/actions/workflows/test.yaml/badge.svg)](https://github.com/CDCgov/phdi/actions/workflows/test.yaml)
+- [PRIME Public Health Data Infrastructure (PHDI)](#prime-public-health-data-infrastructure-phdi)
   - [Overview](#overview)
     - [Problem Scope](#problem-scope)
   - [Getting Started](#getting-started)
   - [Main Features](#main-features)
   - [Where to Get PHDI](#where-to-get-phdi)
   - [Documentation](#documentation)
+  - [Additional Acknowledgments](#additional-acknowledgments)
   - [Standard Notices](#standard-notices)
     - [Public Domain Standard Notice](#public-domain-standard-notice)
     - [License Standard Notice](#license-standard-notice)
     - [Privacy Standard Notice](#privacy-standard-notice)
     - [Contributing Standard Notice](#contributing-standard-notice)
     - [Records Management Standard Notice](#records-management-standard-notice)
     - [Related documents](#related-documents)
```

### Comparing `phdi-1.2.9/phdi/cloud/azure.py` & `phdi-1.4.0/phdi/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/cloud/core.py` & `phdi-1.4.0/phdi/cloud/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/cloud/gcp.py` & `phdi-1.4.0/phdi/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/containers/base_service.py` & `phdi-1.4.0/phdi/containers/base_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from importlib import metadata
 from pathlib import Path
 from typing import Literal
 
 from fastapi import FastAPI
 from pydantic import BaseModel
 
-
 # create a class with the DIBBs default Creative Commons Zero v1.0 and
 # MIT license to be used by the BaseService class
 LICENSES = {
     "CreativeCommonsZero": {
         "name": "Creative Commons Zero v1.0 Universal",
         "url": "https://creativecommons.org/publicdomain/zero/1.0/",
     },
```

### Comparing `phdi-1.2.9/phdi/fhir/cloud/azure.py` & `phdi-1.4.0/phdi/fhir/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/fhir/conversion/convert.py` & `phdi-1.4.0/phdi/fhir/conversion/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from lxml import etree
 
 from phdi.cloud.core import BaseCredentialManager
 from phdi.fhir.transport import http_request_with_reauth
 from phdi.harmonization import standardize_hl7_datetimes
 from phdi.transport.http import http_request_with_retry
 
-
 CCDA_CODES_TO_CONVERSION_RESOURCE = {
     "34133-9": "CCD",
     "11488-4": "ConsultationNote",
     "18842-5": "DischargeSummary",
     "34117-2": "HistoryandPhysical",
     "11504-8": "OperativeNote",
     "28570-0": "ProcedureNote",
@@ -319,15 +318,15 @@
 
         :param http_response: HTTP response returned by the converter service.
           Default: `None`
         :param message: Error message. Default: `None`
         """
         self.__http_response = http_response
 
-        if (message is None) and not (http_response is None):
+        if (message is None) and http_response is not None:
             message = (
                 "Conversion exception occurred with status code"
                 + f" {http_response.status_code} returned from the converter service."
             )
         self.message = message
 
         super().__init__(self.message)
```

### Comparing `phdi-1.2.9/phdi/fhir/geospatial/README.md` & `phdi-1.4.0/phdi/fhir/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/fhir/geospatial/census.py` & `phdi-1.4.0/phdi/fhir/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/fhir/geospatial/core.py` & `phdi-1.4.0/phdi/fhir/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/fhir/geospatial/smarty.py` & `phdi-1.4.0/phdi/fhir/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/fhir/harmonization/README.md` & `phdi-1.4.0/phdi/fhir/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/fhir/harmonization/__init__.py` & `phdi-1.4.0/phdi/fhir/harmonization/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/fhir/harmonization/standardization.py` & `phdi-1.4.0/phdi/fhir/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/fhir/linkage/link.py` & `phdi-1.4.0/phdi/fhir/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/fhir/tabulation/tables.py` & `phdi-1.4.0/phdi/fhir/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/fhir/transport/export.py` & `phdi-1.4.0/phdi/fhir/transport/export.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/fhir/transport/http.py` & `phdi-1.4.0/phdi/fhir/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/fhir/utils.py` & `phdi-1.4.0/phdi/fhir/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
         )
 
     # Temporary hack to ensure no structured data is written using pyarrow.
     # Currently Pyarrow does not support mixing non-structured and structured data.
     # https://github.com/awslabs/aws-data-wrangler/issues/463
     # Will need to consider other methods of writing to parquet if this is an essential
     # feature.
-    if type(value) is dict:  # pragma: no cover
+    if isinstance(value, dict):  # pragma: no cover
         value = json.dumps(value)
-    elif type(value) is list:
+    elif isinstance(value, list):
         value = ",".join(value)
     return value
 
 
 def extract_value_with_resource_path(
     resource: dict,
     path: str,
```

### Comparing `phdi-1.2.9/phdi/geospatial/README.md` & `phdi-1.4.0/phdi/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/geospatial/census.py` & `phdi-1.4.0/phdi/geospatial/census.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         :return: A properly formatted address for the Census API call, given as a
             string.
         """
         # Check that the address contains structure number and street name
         if searchtype == "onelineaddress":
             address = address.replace(" ", "+").replace(",", "%2C")
             return f"onelineaddress?address={address}"
-        elif searchtype == "address" and type(address) is dict:
+        elif searchtype == "address" and isinstance(address, dict):
             street = address.get("street", "").replace(" ", "+").replace(",", "%2C")
             city = address.get("city", "").replace(" ", "+").replace(",", "%2C")
             state = address.get("state", "").replace(" ", "+").replace(",", "%2C")
             zip = address.get("zip", "").replace(" ", "+").replace(",", "%2C")
 
             # If only "street" is present, format address with
             # searchtype = "onelineaddress"
```

### Comparing `phdi-1.2.9/phdi/geospatial/core.py` & `phdi-1.4.0/phdi/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/geospatial/smarty.py` & `phdi-1.4.0/phdi/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/harmonization/README.md` & `phdi-1.4.0/phdi/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/harmonization/__init__.py` & `phdi-1.4.0/phdi/harmonization/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/harmonization/double_metaphone.py` & `phdi-1.4.0/phdi/harmonization/double_metaphone.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/harmonization/hl7.py` & `phdi-1.4.0/phdi/harmonization/hl7.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/harmonization/phdi_nicknames.csv` & `phdi-1.4.0/phdi/harmonization/phdi_nicknames.csv`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/harmonization/standardization.py` & `phdi-1.4.0/phdi/harmonization/standardization.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import phonenumbers
 import pycountry
 from detect_delimiter import detect
 
 from phdi.harmonization.double_metaphone import DoubleMetaphone
 
-
 FHIR_DATE_FORMAT = "%Y-%m-%d"
 FHIR_DATE_DELIM = "-"
 
 
 def double_metaphone_string(string: str, dmeta=None) -> List[Union[str, None]]:
     """
     Performs the double metaphone phonetic encoding algorithm on the given
```

### Comparing `phdi-1.2.9/phdi/harmonization/utils.py` & `phdi-1.4.0/phdi/harmonization/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/linkage/__init__.py` & `phdi-1.4.0/phdi/linkage/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from phdi.linkage.algorithms import DIBBS_BASIC
 from phdi.linkage.algorithms import DIBBS_ENHANCED
 from phdi.linkage.core import BaseMPIConnectorClient
 from phdi.linkage.link import add_person_resource
-from phdi.linkage.link import aggregate_given_names_for_linkage
 from phdi.linkage.link import block_data
 from phdi.linkage.link import calculate_log_odds
 from phdi.linkage.link import calculate_m_probs
 from phdi.linkage.link import calculate_u_probs
 from phdi.linkage.link import compile_match_lists
 from phdi.linkage.link import eval_log_odds_cutoff
 from phdi.linkage.link import eval_perfect_match
@@ -25,15 +24,14 @@
 from phdi.linkage.link import read_linkage_config
 from phdi.linkage.link import score_linkage_vs_truth
 from phdi.linkage.link import write_linkage_config
 from phdi.linkage.mpi import DIBBsMPIConnectorClient
 from phdi.linkage.seed import convert_to_patient_fhir_resources
 from phdi.linkage.utils import datetime_to_str
 
-
 __all__ = [
     "DIBBS_BASIC",
     "DIBBS_ENHANCED",
     "generate_hash_str",
     "block_data",
     "match_within_block",
     "feature_match_exact",
@@ -58,9 +56,8 @@
     "link_record_against_mpi",
     "add_person_resource",
     "_compare_address_elements",
     "_compare_name_elements",
     "convert_to_patient_fhir_resources",
     "DIBBsMPIConnectorClient",
     "datetime_to_str",
-    "aggregate_given_names_for_linkage",
 ]
```

### Comparing `phdi-1.2.9/phdi/linkage/algorithms.py` & `phdi-1.4.0/phdi/linkage/algorithms.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/linkage/config.py` & `phdi-1.4.0/phdi/linkage/config.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/linkage/core.py` & `phdi-1.4.0/phdi/linkage/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,17 @@
         else inserts a new patient into the patient table, as well as all other
         subsequent MPI tables, and inserts a new person into the person table
         linking the new person to the new patient.
         """
         pass  # pragma: no cover
 
     @abstractmethod
-    def _generate_block_query(self, block_critieria: dict) -> Select:
+    def _generate_block_query(
+        self, organized_block_criteria: dict, query: Select
+    ) -> Select:
         """
          Generates a query for selecting a block of data from the MPI tables per the
         block field criteria.  The block field criteria should be a dictionary
         organized by MPI table name, with the ORM table object, and the blocking
         criteria.
         """
         pass  # pragma: no cover
```

### Comparing `phdi-1.2.9/phdi/linkage/dal.py` & `phdi-1.4.0/phdi/linkage/dal.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,15 +298,18 @@
                 session.execute(text(statements))
                 logging.info(
                     f"Done with INSERT statement execution at:{datetime.datetime.now().strftime('%m-%d-%yT%H:%M:%S.%f')}"  # noqa
                 )
         return return_results
 
     def select_results(
-        self, select_statement: select, include_col_header: bool = True
+        self,
+        select_statement: select,
+        include_col_header: bool = True,
+        query_params: dict = None,
     ) -> List[list]:
         """
         Perform a select query and add the results to a
         list of lists.  Then add the column header as the
         first row, in the list of lists if the
         'include_col_header' parameter is True.
 
@@ -320,15 +323,16 @@
         logging.info(
             f"In select_results, starting new session at {datetime.datetime.now().strftime('%m-%d-%yT%H:%M:%S.%f')}"  # noqa
         )
         with self.transaction() as session:
             logging.info(
                 f"Starting to execute statement to return results at: {datetime.datetime.now().strftime('%m-%d-%yT%H:%M:%S.%f')}"  # noqa
             )
-            results = session.execute(select_statement)
+            results = session.execute(select_statement, query_params)
+
             logging.info(
                 f"Done executing statement to return results at: {datetime.datetime.now().strftime('%m-%d-%yT%H:%M:%S.%f')}"  # noqa
             )
             list_results = [list(row) for row in results]
             if include_col_header:
                 list_results.insert(0, list(results.keys()))
         return list_results
@@ -352,16 +356,14 @@
         Get an SqlAlchemy ORM Table Object based upon the table
         name passed in.
 
         :param table_name: the name of the table you want to get.
         :return: SqlAlchemy ORM Table Object.
         """
 
-        self.initialize_schema()
-
         if table_name is not None and table_name != "":
             # TODO: I am sure there is an easier way to do this
             for table in self.TABLE_LIST:
                 if table.name == table_name:
                     return table
         return None
 
@@ -372,16 +374,14 @@
         in more than one table.
 
         :param column_name: the column name you want to find the
             table it belongs to.
         :return: SqlAlchemy ORM Table Object.
         """
 
-        self.initialize_schema()
-
         if column_name is not None and column_name != "":
             # TODO: I am sure there is an easier way to do this
             for table in self.TABLE_LIST:
                 if column_name in table.c:
                     return table
         return None
```

### Comparing `phdi-1.2.9/phdi/linkage/link.py` & `phdi-1.4.0/phdi/linkage/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -613,15 +613,15 @@
             f"Starting get_block_data at: {datetime.datetime.now().strftime('%m-%d-%yT%H:%M:%S.%f')}"  # noqa
         )
         raw_data_block = mpi_client.get_block_data(blocking_criteria)
         logging.info(
             f"Done with get_block_data at: {datetime.datetime.now().strftime('%m-%d-%yT%H:%M:%S.%f')}"  # noqa
         )
 
-        data_block = aggregate_given_names_for_linkage(raw_data_block)
+        data_block = _convert_given_name_to_first_name(raw_data_block)
 
         # First row of returned block is column headers
         # Map column name to idx, not including patient/person IDs
         col_to_idx = {v: k for k, v in enumerate(data_block[0][2:])}
         if len(data_block[1:]) > 0:  # Check if data_block is empty
             data_block = data_block[1:]
             logging.info(
@@ -1140,17 +1140,17 @@
     """
     Helper method that re-maps the string names of functions to their
     callable invocations as defined within the `link.py` module.
     """
     for lp in algo_config:
         feature_funcs = lp["funcs"]
         for func in feature_funcs:
-            if type(feature_funcs[func]) is str:
+            if isinstance(feature_funcs[func], str):
                 feature_funcs[func] = globals()[feature_funcs[func]]
-        if type(lp["matching_rule"]) is str:
+        if isinstance(lp["matching_rule"], str):
             lp["matching_rule"] = globals()[lp["matching_rule"]]
     return algo_config
 
 
 def _eval_record_in_cluster(
     block: List[List],
     i: int,
@@ -1281,42 +1281,51 @@
         feature_col,
         {feature_col: 0},
         **kwargs,
     )
     return feature_comp
 
 
-def _condense_extract_address_from_resource(resource: dict, field: str):
+def _condense_extract_address_from_resource(resource: dict, field: str) -> List[str]:
     """
     Formatting function to account for patient resources that have multiple
     associated addresses. Each address is a self-contained object, replete
     with its own `line` property that can hold a list of strings. This
     function condenses that `line` into a single concatenated string, for
     each address object, and returns the result in a properly formatted
     list.
+
+    :param resource: The patient resource to extract the address from.
+    :param field: The field to extract the address from.
+    :return: A list of strings, each string representing a single address.
     """
     expanded_address_fhirpath = LINKING_FIELDS_TO_FHIRPATHS[field]
     expanded_address_fhirpath = ".".join(expanded_address_fhirpath.split(".")[:-1])
-    list_of_address_objects = extract_value_with_resource_path(
-        resource, expanded_address_fhirpath, "all"
+    list_of_address_objects = (
+        extract_value_with_resource_path(resource, expanded_address_fhirpath, "all")
+        or []
     )
+    if not list_of_address_objects:
+        return None
+
     if field == "address":
         list_of_address_lists = [
             ao.get(LINKING_FIELDS_TO_FHIRPATHS[field].split(".")[-1], [])
             for ao in list_of_address_objects
         ]
         list_of_usable_address_elements = [
             " ".join(obj) for obj in list_of_address_lists
         ]
     else:
         list_of_usable_address_elements = []
         for address_object in list_of_address_objects:
             list_of_usable_address_elements.append(
                 address_object.get(LINKING_FIELDS_TO_FHIRPATHS[field].split(".")[-1])
             )
+
     return list_of_usable_address_elements
 
 
 def _find_strongest_link(linkage_scores: dict) -> str:
     """
     Helper method that determines the highest belongingness level that an
     incoming record achieved against a set of clusers based on existing
@@ -1539,53 +1548,28 @@
     }
 
     bundle.get("entry", []).append(person_resource)
 
     return bundle
 
 
-def aggregate_given_names_for_linkage(data: list[list]):
+def _convert_given_name_to_first_name(data: list[list]) -> list[list]:
     """
-    Aggregates the given names in the return block data into appropriate format for
-    record linkage, i.e., one row of data for each patient with all of the given names
-    in a space-delimited string, e.g., John Tiberius
+    In the list of query row results, convert the given_name column (which is a
+    list of given names) to a first_name column (which is a space-delimited string
+    of given names).
 
     :param data: List of lists block data.
-    :return: List of lists with aggregated given names.
+    :return: List of lists with first_name column.
     """
-    # Convert LoL to pandas dataframe
-    raw_data = pd.DataFrame(data[1:], columns=data[0])
-
-    # Aggregate given names
-    given_names = (
-        raw_data.sort_values(["name_id", "given_name_index"])
-        .groupby(["name_id"])["given_name"]
-        .apply(lambda x: " ".join(x))
-        .reset_index()
-    )
-    given_names.rename(columns={"given_name": "first_name"}, inplace=True)
-
-    # Merge aggregated given names into original data
-    df = raw_data.merge(given_names, on="name_id")
-
-    # Return only necessary columns
-    # TODO: remove hard coding of necessary columns
-    necessary_columns = [
-        "patient_id",
-        "person_id",
-        "birthdate",
-        "sex",
-        "mrn",
-        "last_name",
-        "first_name",
-        "address",
-        "zip",
-        "city",
-        "state",
-    ]
-    df = df[necessary_columns]
-    df = df.drop_duplicates()
-
-    # Convert dataframe to list of lists for record linkage
-    lol = df.values.tolist()
-    lol.insert(0, necessary_columns)
-    return lol
+    result = []
+    if not data:
+        return result  # empty list, should return an empty list
+
+    if "given_name" not in data[0]:
+        return data  # given_name not in data, should return the original
+
+    given_name_idx = data[0].index("given_name")
+    for idx, row in enumerate(data):
+        val = "first_name" if idx == 0 else " ".join(row[given_name_idx])
+        result.append(row[:given_name_idx] + [val] + row[given_name_idx + 1 :])
+    return result
```

### Comparing `phdi-1.2.9/phdi/linkage/mpi.py` & `phdi-1.4.0/phdi/linkage/mpi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import copy
 import datetime
 import logging
 import uuid
 from functools import cache
 from typing import Dict
 from typing import List
 from typing import Literal
 
 from sqlalchemy import and_
 from sqlalchemy import Select
 from sqlalchemy import select
 from sqlalchemy import text
+from sqlalchemy.dialects.postgresql import aggregate_order_by
+from sqlalchemy.dialects.postgresql import array_agg
 
 from phdi.fhir.utils import extract_value_with_resource_path
 from phdi.linkage.core import BaseMPIConnectorClient
 from phdi.linkage.dal import DataAccessLayer
 from phdi.linkage.utils import load_mpi_env_vars_os
 
 
@@ -157,25 +158,27 @@
         )
 
         # now tack on the where criteria using the block_vals
         # while ensuring they exist in the table structure ORM
         logging.info(
             f"Starting _generate_block_query at:{datetime.datetime.now().strftime('%m-%d-%yT%H:%M:%S.%f')}"  # noqa
         )
-        query_w_ctes = self._generate_block_query(
+        query_w_ctes, query_params = self._generate_block_query(
             organized_block_criteria=organized_block_vals, query=query
         )
         logging.info(
             f"Done with _generate_block_query at:{datetime.datetime.now().strftime('%m-%d-%yT%H:%M:%S.%f')}"  # noqa
         )
         logging.info(
             f"Starting dal.select_results at:{datetime.datetime.now().strftime('%m-%d-%yT%H:%M:%S.%f')}"  # noqa
         )
         blocked_data = self.dal.select_results(
-            select_statement=query_w_ctes, include_col_header=True
+            select_statement=query_w_ctes,
+            query_params=query_params,
+            include_col_header=True,
         )
         logging.info(
             f"Done with dal.select_results at:{datetime.datetime.now().strftime('%m-%d-%yT%H:%M:%S.%f')}"  # noqa
         )
 
         return blocked_data
 
@@ -241,102 +244,116 @@
                       done with _insert_external_person_id at:{datetime.datetime.now().strftime('%m-%d-%yT%H:%M:%S.%f')}"""  # noqa
                 )
         except Exception as error:  # pragma: no cover
             raise ValueError(f"{error}")
 
         return person_id
 
-    def _generate_where_criteria(self, block_criteria: dict, table_name: str) -> list:
+    def _generate_where_clause(
+        self, block_criteria: dict, table_name: str
+    ) -> tuple[str, list]:
         """
         Generates a list of where criteria leveraging the blocking criteria,
         including transformations such as 'first 4' or 'last 4'.  This
         function leverages the ORM to determine the table and columns.
 
         :param block_criteria: a dictionary that contains the blocking criteria.
-        :return: A list of where criteria used to append to the end of a query.
+        :return: A tuple containing the query's where clause as a string and a list of
+        the appropriate params to pass into the where clause.
 
         """
-        where_criteria = []
+        where_placeholders = []
+        where_params = {}
+
         for key, value in block_criteria.items():
+            placeholder = f"criterion_{table_name}_{key}"
             criteria_value = value["value"]
             criteria_transform = value.get("transformation", None)
 
             if criteria_transform is None:
-                where_criteria.append(f"{table_name}.{key} = '{criteria_value}'")
+                where_placeholders.append(f"{table_name}.{key} = :{placeholder}")
             else:
                 if criteria_transform == "first4":
-                    where_criteria.append(
-                        f"LEFT({table_name}.{key},4) = '{criteria_value}'"
+                    where_placeholders.append(
+                        f"LEFT({table_name}.{key},4) = :{placeholder}"
                     )
                 elif criteria_transform == "last4":
-                    where_criteria.append(
-                        f"RIGHT({table_name}.{key},4) = '{criteria_value}'"
+                    where_placeholders.append(
+                        f"RIGHT({table_name}.{key},4) = :{placeholder}"
                     )
-        return where_criteria
+            where_params[placeholder] = criteria_value
+
+        where_clause = " AND ".join(where_placeholders)
+
+        return where_clause, where_params
 
     def _generate_block_query(
         self, organized_block_criteria: dict, query: Select
-    ) -> Select:
+    ) -> tuple[Select, dict]:
         """
         Generates a query for selecting a block of data from the MPI tables per the
         block field criteria.  The block field criteria should be a dictionary
         organized by MPI table name, with the ORM table object, and the blocking
         criteria.
 
         :param organized_block_vals: a dictionary organized by MPI table name,
             with the ORM table object, and the blocking criteria.
-        :return: A 'Select' statement built by the sqlalchemy ORM utilizing
-            the blocking criteria.
+        :return: A tuple of a 'Select' statement built by the sqlalchemy ORM utilizing
+            the blocking criteria and a dictionary of the query parameters.
 
         """
         new_query = query
+        new_query_params = {}
 
         for table_key, table_info in organized_block_criteria.items():
-            query_criteria = None
+            where_params = None
             cte_query = None
             sub_query = None
 
             cte_query_table = table_info["table"]
-            query_criteria = self._generate_where_criteria(
+            where_clause, where_params = self._generate_where_clause(
                 table_info["criteria"], table_key
             )
+            new_query_params = {**new_query_params, **where_params}
 
-            if query_criteria is not None and len(query_criteria) > 0:
+            if where_clause != "" and len(where_params) > 0:
                 if self.dal.does_table_have_column(cte_query_table, "patient_id"):
                     cte_query = (
                         select(cte_query_table.c.patient_id.label("patient_id"))
-                        .where(text(" AND ".join(query_criteria)))
+                        .distinct()
+                        .where(text(where_clause))
                         .cte(f"{table_key}_cte")
                     )
                 else:
-                    fk_query_table = copy.deepcopy(cte_query_table)
-                    fk_info = fk_query_table.foreign_keys.pop()
+                    fk_info = next(iter(cte_query_table.foreign_keys))
                     fk_column = fk_info.column
                     fk_table = fk_info.column.table
                     sub_query = (
                         select(cte_query_table)
-                        .where(text(" AND ".join(query_criteria)))
+                        .where(text(where_clause))
                         .subquery(f"{cte_query_table.name}_cte_subq")
                     )
                     cte_query = (
-                        select(fk_table.c.patient_id).join(
+                        select(fk_table.c.patient_id)
+                        .distinct()
+                        .join(
                             sub_query,
                             text(
                                 f"{fk_table.name}.{fk_column.name} = "
                                 + f"{sub_query.name}.{fk_column.name}"
                             ),
                         )
                     ).cte(f"{table_key}_cte")
             if cte_query is not None:
                 new_query = new_query.join(
                     cte_query,
                     and_(cte_query.c.patient_id == self.dal.PATIENT_TABLE.c.patient_id),
                 )
 
-        return new_query
+        return new_query, new_query_params
 
     def _organize_block_criteria(self, block_fields: dict) -> dict:
         """
         Creates a dictionary with the MPI Table Names as keys
         that also stores the ORM Table Object, for each table,
         as well as the blocking criteria for each of the tables.
         The Table is discovered based upon the blocking columns.
@@ -428,17 +445,21 @@
             select(
                 self.dal.PATIENT_TABLE.c.patient_id,
                 self.dal.PATIENT_TABLE.c.person_id,
                 self.dal.PATIENT_TABLE.c.dob.label("birthdate"),
                 self.dal.PATIENT_TABLE.c.sex,
                 id_sub_query.c.mrn,
                 self.dal.NAME_TABLE.c.last_name,
-                self.dal.GIVEN_NAME_TABLE.c.given_name,
-                self.dal.GIVEN_NAME_TABLE.c.given_name_index,
-                self.dal.GIVEN_NAME_TABLE.c.name_id,
+                # Aggregate the given names into an array ordered by the name index
+                array_agg(
+                    aggregate_order_by(
+                        self.dal.GIVEN_NAME_TABLE.c.given_name,
+                        self.dal.GIVEN_NAME_TABLE.c.given_name_index.asc(),
+                    )
+                ).label("given_name"),
                 # TODO: keeping this here for the time
                 # when we decide to add phone numbers into
                 # the blocking data
                 #
                 # phone_sub_query.c.phone_number,
                 # phone_sub_query.c.phone_type,
                 self.dal.ADDRESS_TABLE.c.line_1.label("address"),
@@ -453,14 +474,27 @@
             .outerjoin(self.dal.GIVEN_NAME_TABLE)
             # TODO: keeping this here for the time
             # when we decide to add phone numbers into
             # the blocking data
             #
             # .outerjoin(phone_sub_query)
             .outerjoin(self.dal.ADDRESS_TABLE)
+            .group_by(
+                self.dal.PATIENT_TABLE.c.patient_id,
+                self.dal.PATIENT_TABLE.c.person_id,
+                "birthdate",
+                self.dal.PATIENT_TABLE.c.sex,
+                id_sub_query.c.mrn,
+                self.dal.NAME_TABLE.c.last_name,
+                self.dal.NAME_TABLE.c.name_id,
+                "address",
+                "zip",
+                self.dal.ADDRESS_TABLE.c.city,
+                self.dal.ADDRESS_TABLE.c.state,
+            )
         )
         return query
 
     def _get_mpi_records(self, patient_resource: dict) -> dict:
         """
         Generates a dictionary with the different MPI Table
         Name as keys along with the records for each of the
```

### Comparing `phdi-1.2.9/phdi/linkage/new_tables.ddl` & `phdi-1.4.0/phdi/linkage/new_tables.ddl`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/linkage/seed.py` & `phdi-1.4.0/phdi/linkage/seed.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/linkage/utils.py` & `phdi-1.4.0/phdi/linkage/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/tabulation/tables.py` & `phdi-1.4.0/phdi/tabulation/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     :return: A string representation of the list
     """
     for i, v in enumerate(val):
         if isinstance(v, list):
             val[i] = _convert_list_to_string(v)
         elif isinstance(v, dict):
             val[i] = str(v)
-        elif type(v) is not str:
+        elif not isinstance(v, str):
             val[i] = str(v)
     return (",").join(val)
 
 
 def _create_pa_schema_from_table_schema(
     schema: dict, col_names: List, table_name: str
 ) -> pa.Schema:
```

### Comparing `phdi-1.2.9/phdi/tabulation/validation_schema.json` & `phdi-1.4.0/phdi/tabulation/validation_schema.json`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/transport/http.py` & `phdi-1.4.0/phdi/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/validation/__init__.py` & `phdi-1.4.0/phdi/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.2.9/phdi/validation/validation.py` & `phdi-1.4.0/phdi/validation/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from .xml_utils import ECR_NAMESPACES
 from .xml_utils import get_ecr_message_ids
 from .xml_utils import get_xml_element_details
 from .xml_utils import validate_xml_attributes
 from .xml_utils import validate_xml_elements
 from .xml_utils import validate_xml_value
 
-
 ERROR_MESSAGES = {
     "fatal": [],
     "errors": [],
     "warnings": [],
     "information": [],
     "message_ids": {},
 }
```

### Comparing `phdi-1.2.9/phdi/validation/xml_utils.py` & `phdi-1.4.0/phdi/validation/xml_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 
 from lxml import etree
 
-
 EICR_MSG_ID_XPATH = "//hl7:ClinicalDocument/hl7:id"
 RR_MSG_ID_XPATH = "//hl7:ClinicalDocument/hl7:section/hl7:id"
 
 XML_PATH_DELIMITER = "/"
 
 ECR_NAMESPACES = {
     "hl7": "urn:hl7-org:v3",
```

### Comparing `phdi-1.2.9/PKG-INFO` & `phdi-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdi
-Version: 1.2.9
+Version: 1.4.0
 Summary: Public health data infrastructure Building Blocks is a library to help public health departments work with their data
 Home-page: https://github.com/CDCgov/phdi
 Author: Kenneth Chow
 Author-email: kenneth@skylight.digital
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -24,36 +24,40 @@
 Requires-Dist: hl7 (>=0.4.5,<0.5.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: jsonschema (==4.16.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: phonenumbers (>=8.12.48,<9.0.0)
+Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: polling (>=0.3.2,<0.4.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pyarrow (>=12,<15)
 Requires-Dist: pycountry (>=22.3.5,<23.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: rapidfuzz (>=2.13.6,<3.0.0)
 Requires-Dist: smartystreets-python-sdk (>=4.10.6,<5.0.0)
 Requires-Dist: sqlalchemy (>=2.0.0,<3.0.0)
 Project-URL: Documentation, https://cdcgov.github.io/phdi
 Project-URL: Repository, https://github.com/CDCgov/phdi
 Description-Content-Type: text/markdown
 
 # PRIME Public Health Data Infrastructure (PHDI)
-[![Test github badge](https://github.com/CDCgov/phdi/actions/workflows/test.yaml/badge.svg)](https://github.com/CDCgov/phdi/actions/workflows/test.yaml)
 [![codecov](https://codecov.io/gh/CDCgov/phdi/branch/main/graph/badge.svg)](https://codecov.io/gh/CDCgov/phdi)
-- [PRIME Public Health Data Infrastructure](#prime-public-health-data-infrastructure)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Test github badge](https://github.com/CDCgov/phdi/actions/workflows/test.yaml/badge.svg)](https://github.com/CDCgov/phdi/actions/workflows/test.yaml)
+- [PRIME Public Health Data Infrastructure (PHDI)](#prime-public-health-data-infrastructure-phdi)
   - [Overview](#overview)
     - [Problem Scope](#problem-scope)
   - [Getting Started](#getting-started)
   - [Main Features](#main-features)
   - [Where to Get PHDI](#where-to-get-phdi)
   - [Documentation](#documentation)
+  - [Additional Acknowledgments](#additional-acknowledgments)
   - [Standard Notices](#standard-notices)
     - [Public Domain Standard Notice](#public-domain-standard-notice)
     - [License Standard Notice](#license-standard-notice)
     - [Privacy Standard Notice](#privacy-standard-notice)
     - [Contributing Standard Notice](#contributing-standard-notice)
     - [Records Management Standard Notice](#records-management-standard-notice)
     - [Related documents](#related-documents)
```

