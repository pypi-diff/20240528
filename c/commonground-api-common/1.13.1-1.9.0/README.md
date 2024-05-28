# Comparing `tmp/commonground_api_common-1.13.1.tar.gz` & `tmp/commonground-api-common-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonground_api_common-1.13.1.tar", last modified: Tue May 28 12:39:04 2024, max compression
+gzip compressed data, was "commonground-api-common-1.9.0.tar", last modified: Mon Dec 12 13:57:55 2022, max compression
```

## Comparing `commonground_api_common-1.13.1.tar` & `commonground-api-common-1.9.0.tar`

### file list

```diff
@@ -1,263 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.065290 commonground_api_common-1.13.1/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-05-28 12:39:04.065290 commonground_api_common-1.13.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.017290 commonground_api_common-1.13.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/bin/generate_schema
--rwxr-xr-x   0 runner    (1001) docker     (127)      319 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/bin/patch_content_types
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/bin/use_external_components
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.061290 commonground_api_common-1.13.1/commonground_api_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-05-28 12:39:03.000000 commonground_api_common-1.13.1/commonground_api_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-05-28 12:39:04.000000 commonground_api_common-1.13.1/commonground_api_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:39:03.000000 commonground_api_common-1.13.1/commonground_api_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:39:03.000000 commonground_api_common-1.13.1/commonground_api_common.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-28 12:39:03.000000 commonground_api_common-1.13.1/commonground_api_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 12:39:03.000000 commonground_api_common-1.13.1/commonground_api_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-28 12:39:04.065290 commonground_api_common-1.13.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.021290 commonground_api_common-1.13.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_autorisatie_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_cache_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_check_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_content_type_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_gegevensgroepen.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_get_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_jwt_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_jwtsecrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_nested_serializer_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_publish_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_schema_root_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_server_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/tests/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.029290 commonground_api_common-1.13.1/vng_api_common/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.029290 commonground_api_common-1.13.1/vng_api_common/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/api/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.029290 commonground_api_common-1.13.1/vng_api_common/audittrails/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.029290 commonground_api_common-1.13.1/vng_api_common/audittrails/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/api/scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/audits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.037290 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0002_auto_20190516_0830.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0003_auto_20190517_0844.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0004_auto_20190520_1238.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0005_auto_20190520_1450.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0006_audittrail_toelichting.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0007_auto_20190522_0916.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0008_audittrail_resource_weergave.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0009_auto_20190712_1643.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0010_audittrail_request_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0011_auto_20190918_1335.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0012_auto_20200619_0545.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0012_remove_audittrail_request_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0013_audittrail_logrecord_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0013_auto_20201207_0846.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0014_auto_20201221_0905.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0014_auto_20210323_1654.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0015_auto_20220318_1608.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0016_merge_20220607_0517.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0017_alter_audittrail_bron.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0018_auto_20221212_0745.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/audittrails/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.037290 commonground_api_common-1.13.1/vng_api_common/authorizations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.041290 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0002_authorizationsconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0003_auto_20190502_0409.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0004_auto_20190503_0941.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0005_auto_20190506_0842.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0006_auto_20190506_0901.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0007_auto_20190506_1212.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0008_auto_20190712_1541.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0009_update_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0010_auto_20190712_1643.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0011_auto_20191114_0728.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0012_auto_20200619_0545.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0013_auto_20201207_0846.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0014_auto_20201221_0905.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0015_auto_20220318_1608.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/authorizations/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.041290 commonground_api_common-1.13.1/vng_api_common/caching/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/caching/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/caching/etags.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/caching/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/caching/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/caching/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/caching/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.041290 commonground_api_common-1.13.1/vng_api_common/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/conf/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.041290 commonground_api_common-1.13.1/vng_api_common/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/db/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/geo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.041290 commonground_api_common-1.13.1/vng_api_common/inspectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/inspectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/inspectors/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/inspectors/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/inspectors/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    12575 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/inspectors/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/inspectors/polymorphic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/inspectors/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/inspectors/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/inspectors/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.013290 commonground_api_common-1.13.1/vng_api_common/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.013290 commonground_api_common-1.13.1/vng_api_common/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.045290 commonground_api_common-1.13.1/vng_api_common/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    19495 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.045290 commonground_api_common-1.13.1/vng_api_common/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.045290 commonground_api_common-1.13.1/vng_api_common/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/management/commands/generate_autorisaties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/management/commands/generate_notificaties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/management/commands/generate_swagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/management/commands/patch_error_contenttypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/management/commands/use_external_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.045290 commonground_api_common-1.13.1/vng_api_common/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/migrations/0002_apicredential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/migrations/0003_auto_20190417_1145.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/migrations/0004_auto_20190517_0903.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/migrations/0005_auto_20190614_1346.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.045290 commonground_api_common-1.13.1/vng_api_common/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.045290 commonground_api_common-1.13.1/vng_api_common/notifications/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.049290 commonground_api_common-1.13.1/vng_api_common/notifications/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0002_subscription__subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0003_auto_20190319_1048.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0004_auto_20190325_1313.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0005_fix_default_nrc.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0006_auto_20190417_1142.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0007_auto_20190429_1442.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0008_auto_20190502_0415.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0009_auto_20190729_0427.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0010_auto_20220704_1419.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/oas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/polymorphism.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/routers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.013290 commonground_api_common-1.13.1/vng_api_common/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.013290 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.049290 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/css/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.049290 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/css/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/css/admin/admin_overrides.css
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/css/screen.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.049290 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/ico/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/ico/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.049290 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/img/
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/img/vng.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.013290 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.057290 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.049290 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/css/
--rw-r--r--   0 runner    (1001) docker     (127)    69015 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.css
--rw-r--r--   0 runner    (1001) docker     (127)    55111 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.057290 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)   129916 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   694583 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)   129612 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    87688 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    74768 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    34388 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   144451 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34092 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16804 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   186728 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (127)   816926 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (127)   186444 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    96256 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (127)    74256 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.013290 commonground_api_common-1.13.1/vng_api_common/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.057290 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.061290 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/admin/base_site.html
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/autorisaties.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.061290 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/includes/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/includes/kanalen_card.html
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/master.html
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/notificaties.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.061290 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/ref/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/ref/error_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/ref/scopes.html
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/view_config.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.061290 commonground_api_common-1.13.1/vng_api_common/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/templatetags/vng_api_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:39:04.061290 commonground_api_common-1.13.1/vng_api_common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/tests/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/tests/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-28 12:38:59.000000 commonground_api_common-1.13.1/vng_api_common/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.644428 commonground-api-common-1.9.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      952 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/bin/generate_schema
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/bin/generate_schema.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)      319 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/bin/patch_content_types
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/bin/patch_content_types.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/bin/use_external_components
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/bin/use_external_components.cmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.644428 commonground-api-common-1.9.0/commonground_api_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2022-12-12 13:57:55.000000 commonground-api-common-1.9.0/commonground_api_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2022-12-12 13:57:55.000000 commonground-api-common-1.9.0/commonground_api_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 13:57:55.000000 commonground-api-common-1.9.0/commonground_api_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 13:57:55.000000 commonground-api-common-1.9.0/commonground_api_common.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2022-12-12 13:57:55.000000 commonground-api-common-1.9.0/commonground_api_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-12 13:57:55.000000 commonground-api-common-1.9.0/commonground_api_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.648428 commonground-api-common-1.9.0/vng_api_common/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.652428 commonground-api-common-1.9.0/vng_api_common/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.652428 commonground-api-common-1.9.0/vng_api_common/audittrails/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.652428 commonground-api-common-1.9.0/vng_api_common/audittrails/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/api/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/audits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.656429 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0002_auto_20190516_0830.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0003_auto_20190517_0844.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0004_auto_20190520_1238.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0005_auto_20190520_1450.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0006_audittrail_toelichting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0007_auto_20190522_0916.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0008_audittrail_resource_weergave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0009_auto_20190712_1643.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0010_audittrail_request_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0011_auto_20190918_1335.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0012_auto_20200619_0545.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0012_remove_audittrail_request_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0013_audittrail_logrecord_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0013_auto_20201207_0846.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0014_auto_20201221_0905.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0014_auto_20210323_1654.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0015_auto_20220318_1608.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0016_merge_20220607_0517.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0017_alter_audittrail_bron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0018_auto_20221212_0745.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/audittrails/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.656429 commonground-api-common-1.9.0/vng_api_common/authorizations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.656429 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0002_authorizationsconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0003_auto_20190502_0409.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0004_auto_20190503_0941.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0005_auto_20190506_0842.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0006_auto_20190506_0901.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0007_auto_20190506_1212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0008_auto_20190712_1541.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0009_update_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0010_auto_20190712_1643.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0011_auto_20191114_0728.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0012_auto_20200619_0545.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0013_auto_20201207_0846.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0014_auto_20201221_0905.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0015_auto_20220318_1608.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/authorizations/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/etags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/caching/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/conf/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/db/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/geo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/inspectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12575 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/polymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20425 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/inspectors/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.640428 commonground-api-common-1.9.0/vng_api_common/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.640428 commonground-api-common-1.9.0/vng_api_common/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19495 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/commands/generate_autorisaties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/commands/generate_notificaties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/commands/generate_swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/commands/patch_error_contenttypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/management/commands/use_external_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.660429 commonground-api-common-1.9.0/vng_api_common/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/migrations/0002_apicredential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/migrations/0003_auto_20190417_1145.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/migrations/0004_auto_20190517_0903.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/migrations/0005_auto_20190614_1346.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/notifications/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0002_subscription__subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0003_auto_20190319_1048.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0004_auto_20190325_1313.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0005_fix_default_nrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0006_auto_20190417_1142.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0007_auto_20190429_1442.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0008_auto_20190502_0415.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0009_auto_20190729_0427.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0010_auto_20220704_1419.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/oas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/polymorphism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.640428 commonground-api-common-1.9.0/vng_api_common/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.644428 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.640428 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/css/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/css/admin/admin_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/ico/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/ico/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/img/vng.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.644428 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.664429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.668429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    64548 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)   151749 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    48488 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   108539 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (123)    76483 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32461 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   192348 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   492048 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   155758 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   625953 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.672429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   222911 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   402249 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    78635 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   311949 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   131637 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)   250568 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    58072 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   190253 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.672429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.672429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    69015 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.css
+-rw-r--r--   0 runner    (1001) docker     (123)    55111 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.676429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   129916 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   694583 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   129612 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    87688 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    74768 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34388 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   144451 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   186728 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   816926 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   186444 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    96256 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    74256 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.676429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/jquery/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   218897 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69917 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.676429 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/popper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/popper/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    87203 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/popper/popper.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21004 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/popper/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.644428 commonground-api-common-1.9.0/vng_api_common/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/admin/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/autorisaties.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/includes/kanalen_card.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/master.html
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/notificaties.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/ref/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/ref/error_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/ref/scopes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/view_config.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/vng_api_common/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/templatetags/vng_api_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 13:57:55.680430 commonground-api-common-1.9.0/vng_api_common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/tests/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/tests/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2022-12-12 13:57:48.000000 commonground-api-common-1.9.0/vng_api_common/viewsets.py
```

### Comparing `commonground_api_common-1.13.1/README.rst` & `commonground-api-common-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/bin/generate_schema` & `commonground-api-common-1.9.0/bin/generate_schema`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/commonground_api_common.egg-info/SOURCES.txt` & `commonground-api-common-1.9.0/commonground_api_common.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,27 @@
-CHANGELOG.rst
 MANIFEST.in
 README.rst
-pyproject.toml
 setup.cfg
 setup.py
 bin/generate_schema
+bin/generate_schema.cmd
 bin/patch_content_types
+bin/patch_content_types.cmd
 bin/use_external_components
+bin/use_external_components.cmd
 commonground_api_common.egg-info/PKG-INFO
 commonground_api_common.egg-info/SOURCES.txt
 commonground_api_common.egg-info/dependency_links.txt
 commonground_api_common.egg-info/not-zip-safe
 commonground_api_common.egg-info/requires.txt
 commonground_api_common.egg-info/top_level.txt
-tests/test_autorisatie_validation.py
-tests/test_cache_headers.py
-tests/test_check_query_params.py
-tests/test_checks.py
-tests/test_choices.py
-tests/test_config.py
-tests/test_content_type_headers.py
-tests/test_filters.py
-tests/test_gegevensgroepen.py
-tests/test_get_resource.py
-tests/test_jwt_decoding.py
-tests/test_jwtsecrets.py
-tests/test_nested_serializer_validation.py
-tests/test_permissions.py
-tests/test_publish_validator.py
-tests/test_schema_root_tags.py
-tests/test_server_errors.py
-tests/test_utils.py
-tests/test_validators.py
-tests/test_views.py
 vng_api_common/__init__.py
 vng_api_common/admin.py
 vng_api_common/apps.py
 vng_api_common/checks.py
-vng_api_common/choices.py
 vng_api_common/client.py
 vng_api_common/compat.py
 vng_api_common/constants.py
 vng_api_common/decorators.py
 vng_api_common/descriptors.py
 vng_api_common/doc.py
 vng_api_common/exception_handling.py
@@ -176,18 +156,38 @@
 vng_api_common/notifications/migrations/0005_fix_default_nrc.py
 vng_api_common/notifications/migrations/0006_auto_20190417_1142.py
 vng_api_common/notifications/migrations/0007_auto_20190429_1442.py
 vng_api_common/notifications/migrations/0008_auto_20190502_0415.py
 vng_api_common/notifications/migrations/0009_auto_20190729_0427.py
 vng_api_common/notifications/migrations/0010_auto_20220704_1419.py
 vng_api_common/notifications/migrations/__init__.py
-vng_api_common/static/./vng_api_common/css/screen.css
 vng_api_common/static/./vng_api_common/css/admin/admin_overrides.css
 vng_api_common/static/./vng_api_common/ico/favicon.png
 vng_api_common/static/./vng_api_common/img/vng.svg
+vng_api_common/static/./vng_api_common/libs/bootstrap/LICENSE.txt
+vng_api_common/static/./vng_api_common/libs/bootstrap/css/bootstrap-grid.css
+vng_api_common/static/./vng_api_common/libs/bootstrap/css/bootstrap-grid.css.map
+vng_api_common/static/./vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css
+vng_api_common/static/./vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css.map
+vng_api_common/static/./vng_api_common/libs/bootstrap/css/bootstrap-reboot.css
+vng_api_common/static/./vng_api_common/libs/bootstrap/css/bootstrap-reboot.css.map
+vng_api_common/static/./vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css
+vng_api_common/static/./vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css.map
+vng_api_common/static/./vng_api_common/libs/bootstrap/css/bootstrap.css
+vng_api_common/static/./vng_api_common/libs/bootstrap/css/bootstrap.css.map
+vng_api_common/static/./vng_api_common/libs/bootstrap/css/bootstrap.min.css
+vng_api_common/static/./vng_api_common/libs/bootstrap/css/bootstrap.min.css.map
+vng_api_common/static/./vng_api_common/libs/bootstrap/js/bootstrap.bundle.js
+vng_api_common/static/./vng_api_common/libs/bootstrap/js/bootstrap.bundle.js.map
+vng_api_common/static/./vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js
+vng_api_common/static/./vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js.map
+vng_api_common/static/./vng_api_common/libs/bootstrap/js/bootstrap.js
+vng_api_common/static/./vng_api_common/libs/bootstrap/js/bootstrap.js.map
+vng_api_common/static/./vng_api_common/libs/bootstrap/js/bootstrap.min.js
+vng_api_common/static/./vng_api_common/libs/bootstrap/js/bootstrap.min.js.map
 vng_api_common/static/./vng_api_common/libs/fontawesome/LICENSE.txt
 vng_api_common/static/./vng_api_common/libs/fontawesome/css/all.css
 vng_api_common/static/./vng_api_common/libs/fontawesome/css/all.min.css
 vng_api_common/static/./vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot
 vng_api_common/static/./vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg
 vng_api_common/static/./vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf
 vng_api_common/static/./vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff
@@ -198,15 +198,24 @@
 vng_api_common/static/./vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff
 vng_api_common/static/./vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2
 vng_api_common/static/./vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot
 vng_api_common/static/./vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg
 vng_api_common/static/./vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf
 vng_api_common/static/./vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff
 vng_api_common/static/./vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2
+vng_api_common/static/./vng_api_common/libs/jquery/LICENSE.txt
+vng_api_common/static/./vng_api_common/libs/jquery/jquery-3.3.1.slim.js
+vng_api_common/static/./vng_api_common/libs/jquery/jquery-3.3.1.slim.min.js
+vng_api_common/static/./vng_api_common/libs/popper/LICENSE.md
+vng_api_common/static/./vng_api_common/libs/popper/popper.js
+vng_api_common/static/./vng_api_common/libs/popper/popper.min.js
+vng_api_common/static/vng_api_common/libs/bootstrap/LICENSE.txt
 vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt
+vng_api_common/static/vng_api_common/libs/jquery/LICENSE.txt
+vng_api_common/static/vng_api_common/libs/popper/LICENSE.md
 vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md
 vng_api_common/templates/vng_api_common/autorisaties.md
 vng_api_common/templates/vng_api_common/index.html
 vng_api_common/templates/vng_api_common/master.html
 vng_api_common/templates/vng_api_common/notificaties.md
 vng_api_common/templates/vng_api_common/view_config.html
 vng_api_common/templates/vng_api_common/admin/base_site.html
```

### Comparing `commonground_api_common-1.13.1/setup.cfg` & `commonground-api-common-1.9.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,76 @@
 [metadata]
 name = commonground-api-common
-version = 1.13.1
+version = 1.9.0
 description = Commonground API tooling
 long_description = file: README.rst
 url = https://github.com/maykinmedia/commonground-api-common
 license = EUPL 1.2
 author = Maykin Media, VNG-Realisatie
 author_email = support@maykinmedia.nl
 keywords = openapi, swagger, django
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	Operating System :: Unix
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 scripts = 
 	bin/generate_schema
+	bin/generate_schema.cmd
 	bin/patch_content_types
+	bin/patch_content_types.cmd
 	bin/use_external_components
+	bin/use_external_components.cmd
 install_requires = 
 	django>=3.2.0
+	django-choices
 	django-filter>=2.0
 	django-solo
-	djangorestframework>=3.11.0
+	djangorestframework~=3.12.0
 	djangorestframework_camel_case>=1.2.0
 	django-rest-framework-condition
 	drf-yasg>=1.20.0
 	drf-nested-routers>=0.93.3
 	gemma-zds-client>=0.14.0
 	iso-639
 	isodate
-	notifications-api-common>=0.2.2
+	notifications-api-common
 	oyaml
 	PyJWT>=2.0.0
+	pyyaml
 	requests
-	coreapi
 tests_require = 
 	pytest
 	pytest-django
 	pytest-factoryboy
 	tox
 	isort
 	black
 	requests-mock
 	freezegun
 
 [options.packages.find]
 include = 
-	vng_api_common*
+	vng_api_common
+	vng_api_common.*
 
 [options.extras_require]
 markdown_docs = 
 	django-markup<=1.3
 	markdown
 tests = 
 	psycopg2
@@ -87,30 +91,32 @@
 release = 
 	bump2version
 
 [aliases]
 test = pytest
 
 [isort]
-profile = black
 combine_as_imports = true
-skip = 
-	env
-	node_modules
-	.tox
-skip_glob = **/migrations/**
+default_section = THIRDPARTY
+include_trailing_comma = true
+line_length = 88
+multi_line_output = 3
+force_grid_wrap = 0
+use_parentheses = True
+ensure_newline_before_comments = True
+skip = env,.tox,.history,.eggs
 known_django = django
 known_first_party = vng_api_common
 sections = FUTURE,STDLIB,DJANGO,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
 
 [tool:pytest]
 testpaths = tests
 DJANGO_SETTINGS_MODULE = testapp.settings
 
-[pycodestyle]
+[pep8]
 max-line-length = 88
 exclude = env,.tox,doc
 
 [flake8]
 max-line-length = 88
 exclude = env,.tox,doc
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/admin.py` & `commonground-api-common-1.9.0/vng_api_common/admin.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/api/permissions.py` & `commonground-api-common-1.9.0/vng_api_common/api/permissions.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/apps.py` & `commonground-api-common-1.9.0/vng_api_common/apps.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     basic_type_info,
     model_field_to_basic_type,
     serializer_field_to_basic_type,
 )
 from rest_framework import serializers
 
 from . import fields
-from .choices import TextChoicesWithDescriptions, ensure_description_exists
 from .serializers import DurationField, LengthHyperlinkedRelatedField
 
 try:
     from relativedeltafield import RelativeDeltaField
 except ImportError:
     RelativeDeltaField = None
 
@@ -34,15 +33,14 @@
         from . import checks  # noqa
         from .caching import signals  # noqa
 
         patch_duration_type()
         register_serializer_field()
         set_custom_hyperlinkedmodelserializer_field()
         set_charfield_error_messages()
-        ensure_text_choice_descriptions(TextChoicesWithDescriptions)
 
 
 def patch_duration_type():
     def _patch(basic_types, _field_cls, format=None):
         for index, (field_cls, basic_type) in enumerate(basic_types):
             if field_cls is _field_cls:
                 basic_types[index] = (_field_cls, (openapi.TYPE_STRING, format))
@@ -86,14 +84,7 @@
     """
     CharField.default_error_messages.update(
         {
             "max_length": _("The value has too many characters"),
             "min_length": _("The value has too few characters"),
         }
     )
-
-
-def ensure_text_choice_descriptions(text_choice_class):
-    ensure_description_exists(text_choice_class)
-
-    for cls in text_choice_class.__subclasses__():
-        ensure_text_choice_descriptions(cls)
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/api/serializers.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/api/serializers.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0001_initial.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import django.contrib.postgres.fields.jsonb
 import django.core.serializers.json
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="AuditTrail",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0002_auto_20190516_0830.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0002_auto_20190516_0830.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-05-16 08:30
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0001_initial")]
 
     operations = [
         migrations.AddField(
             model_name="audittrail",
             name="applicatie_id",
             field=models.CharField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0003_auto_20190517_0844.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0003_auto_20190517_0844.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import django.contrib.postgres.fields.jsonb
 import django.core.serializers.json
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0002_auto_20190516_0830")]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
             name="aanmaakdatum",
             field=models.DateTimeField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0004_auto_20190520_1238.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0004_auto_20190520_1238.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-05-20 12:38
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0003_auto_20190517_0844")]
 
     operations = [
         migrations.AddField(
             model_name="audittrail",
             name="gebruikers_id",
             field=models.CharField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0005_auto_20190520_1450.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0005_auto_20190520_1450.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 2.0.13 on 2019-05-20 14:50
 
 import django.core.validators
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0004_auto_20190520_1238")]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
             name="bron",
             field=models.CharField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0006_audittrail_toelichting.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0006_audittrail_toelichting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-05-21 08:22
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0005_auto_20190520_1450")]
 
     operations = [
         migrations.AddField(
             model_name="audittrail",
             name="toelichting",
             field=models.CharField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0007_auto_20190522_0916.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0007_auto_20190522_0916.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-05-22 09:16
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0006_audittrail_toelichting")]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
             name="toelichting",
             field=models.TextField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0008_audittrail_resource_weergave.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0008_audittrail_resource_weergave.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.2 on 2019-06-06 12:04
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0007_auto_20190522_0916")]
 
     operations = [
         migrations.AddField(
             model_name="audittrail",
             name="resource_weergave",
             field=models.CharField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0009_auto_20190712_1643.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0009_auto_20190712_1643.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import django.contrib.postgres.fields.jsonb
 import django.core.serializers.json
 import django.core.validators
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0008_audittrail_resource_weergave")]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
             name="aanmaakdatum",
             field=models.DateTimeField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0010_audittrail_request_id.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0006_auto_20190417_1142.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-# Generated by Django 2.1.1 on 2019-08-19 12:01
+# Generated by Django 2.0.13 on 2019-04-17 11:42
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-    dependencies = [("audittrails", "0009_auto_20190712_1643")]
+
+    dependencies = [("notifications", "0005_fix_default_nrc")]
 
     operations = [
-        migrations.AddField(
-            model_name="audittrail",
-            name="request_id",
-            field=models.CharField(
-                blank=True,
-                help_text='Een globaal "request" ID om een verzoek door het netwerk heen te traceren.',
-                max_length=255,
+        migrations.RemoveField(model_name="notificationsconfig", name="client_id"),
+        migrations.RemoveField(model_name="notificationsconfig", name="secret"),
+        migrations.AlterField(
+            model_name="notificationsconfig",
+            name="api_root",
+            field=models.URLField(
+                default="https://ref.tst.vng.cloud/nrc/api/v1",
+                unique=True,
+                verbose_name="api root",
             ),
-        )
+        ),
     ]
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0011_auto_20190918_1335.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0011_auto_20190918_1335.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import django.contrib.postgres.indexes
 from django.contrib.postgres.operations import TrigramExtension
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("audittrails", "0010_audittrail_request_id")]
 
     operations = [
         TrigramExtension(),
         migrations.AddIndex(
             model_name="audittrail",
             index=django.contrib.postgres.indexes.GinIndex(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0012_auto_20200619_0545.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0012_auto_20200619_0545.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.6 on 2020-06-19 05:45
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0011_auto_20190918_1335"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0013_audittrail_logrecord_id.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0013_audittrail_logrecord_id.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.db import migrations, models
 
 from ._operations import AddField
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0012_remove_audittrail_request_id"),
     ]
 
     operations = [
         AddField(
             model_name="audittrail",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0013_auto_20201207_0846.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0013_auto_20201207_0846.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.8 on 2020-12-07 08:46
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0012_auto_20200619_0545"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0014_auto_20201221_0905.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0014_auto_20201221_0905.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.db import migrations, models
 
 from ._operations import AddField, RemoveField
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0013_auto_20201207_0846"),
     ]
 
     operations = [
         RemoveField(
             model_name="audittrail",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0014_auto_20210323_1654.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0014_auto_20210323_1654.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.17 on 2021-03-23 16:54
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0013_audittrail_logrecord_id"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0015_auto_20220318_1608.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0015_auto_20220318_1608.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.27 on 2022-03-18 16:08
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0014_auto_20201221_0905"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0017_alter_audittrail_bron.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0017_alter_audittrail_bron.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.14 on 2022-07-26 08:41
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0016_merge_20220607_0517"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/0018_auto_20221212_0745.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/0018_auto_20221212_0745.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.2.16 on 2022-12-12 07:45
 
 import django.core.serializers.json
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("audittrails", "0017_alter_audittrail_bron"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="audittrail",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/migrations/_operations.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/migrations/_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Custom operations to check the db state before applying the changes.
 
 This is needed because of the merge with stable/1.0.x and master where different
 migrations perform the same schema changes and are thus conflicting.
 """
-
 from django.core.exceptions import FieldDoesNotExist
 from django.db import migrations
 
 
 def check_field_exists(connection, model, field_name):
     try:
         field = model._meta.get_field(field_name)
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/models.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/models.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/audittrails/viewsets.py` & `commonground-api-common-1.9.0/vng_api_common/audittrails/viewsets.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
-from typing import Optional
 
 from django.db import transaction
 from django.http import Http404
 
-from rest_framework import serializers, viewsets
+from rest_framework import viewsets
 
 from ..compat import get_header
 from ..constants import CommonResourceAction
 from ..permissions import AuthScopesRequired
 from ..utils import get_uuid_from_path
 from ..viewsets import NestedViewSetMixin
 from .api.scopes import SCOPE_AUDITTRAILS_LEZEN
@@ -65,25 +64,22 @@
 
         user_id = jwt_auth.payload.get("user_id") or ""
         user_representation = jwt_auth.payload.get("user_representation") or ""
 
         toelichting = get_header(self.request, "X-Audit-Toelichting") or ""
 
         logrecord_id = get_header(self.request, "X-NLX-Logrecord-ID") or ""
-        action_labels = dict(
-            zip(CommonResourceAction.names, CommonResourceAction.labels)
-        )
 
         trail = AuditTrail(
             bron=self.audit.component_name,
             logrecord_id=logrecord_id,
             applicatie_id=app_id,
             applicatie_weergave=app_presentation,
             actie=action,
-            actie_weergave=action_labels.get(action, ""),
+            actie_weergave=CommonResourceAction.labels.get(action, ""),
             gebruikers_id=user_id,
             gebruikers_weergave=user_representation,
             resultaat=status_code,
             hoofd_object=main_object,
             resource=self.basename,
             resource_url=data["url"],
             toelichting=toelichting,
@@ -91,44 +87,33 @@
             oud=version_before_edit,
             nieuw=version_after_edit,
         )
         trail.save()
 
 
 class AuditTrailCreateMixin(AuditTrailMixin):
-    _audittrail_serializer: Optional[serializers.Serializer] = None
-
     def get_audittrail_instance(self, response):
-        if self._audittrail_serializer is not None:
-            return self._audittrail_serializer.instance
         zaak_uuid = get_uuid_from_path(response.data["url"])
         instance = self.get_queryset().get(uuid=zaak_uuid)
         return instance
 
-    def perform_create(self, serializer):
-        super().perform_create(serializer)
-        # cache for future re-use
-        self._audittrail_serializer = serializer
-
     def create(self, request, *args, **kwargs):
         response = super().create(request, *args, **kwargs)
         instance = self.get_audittrail_instance(response)
         self.create_audittrail(
             response.status_code,
             CommonResourceAction.create,
             version_before_edit=None,
             version_after_edit=response.data,
             unique_representation=instance.unique_representation(),
         )
         return response
 
 
 class AuditTrailUpdateMixin(AuditTrailMixin):
-    # TODO: cache serializer(s) via perform_update?
-
     def update(self, request, *args, **kwargs):
         # Retrieve the data stored in the object before updating
         instance = self.get_object()
         serializer = self.get_serializer(instance)
         version_before_edit = serializer.data
 
         action = (
@@ -145,16 +130,14 @@
             version_after_edit=response.data,
             unique_representation=instance.unique_representation(),
         )
         return response
 
 
 class AuditTrailDestroyMixin(AuditTrailMixin):
-    # TODO: cache serializer(s) via perform_update?
-
     def destroy(self, request, *args, **kwargs):
         # Retrieve the data stored in the object before updating
         instance = self.get_object()
         serializer = self.get_serializer(instance)
         version_before_edit = serializer.data
 
         # If the resource being deleted is the main resource, delete all the
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/admin.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/admin.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0001_initial.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from django.db import migrations, models
 
 import vng_api_common.fields
 import vng_api_common.models
 
 
 class Migration(migrations.Migration):
+
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="Applicatie",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0002_authorizationsconfig.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0002_authorizationsconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.8 on 2019-05-02 04:04
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0001_initial")]
 
     operations = [
         migrations.CreateModel(
             name="AuthorizationsConfig",
             fields=[
                 (
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0003_auto_20190502_0409.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0003_auto_20190502_0409.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.8 on 2019-05-02 04:09
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0002_authorizationsconfig")]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
             name="api_root",
             field=models.URLField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0004_auto_20190503_0941.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0004_auto_20190503_0941.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.db import migrations, models
 
 import vng_api_common.fields
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0003_auto_20190502_0409")]
 
     operations = [
         migrations.AlterField(
             model_name="autorisatie",
             name="max_vertrouwelijkheidaanduiding",
             field=vng_api_common.fields.VertrouwelijkheidsAanduidingField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0005_auto_20190506_0842.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0005_auto_20190506_0842.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.8 on 2019-05-06 08:42
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0004_auto_20190503_0941")]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
             name="component",
             field=models.CharField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0006_auto_20190506_0901.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0006_auto_20190506_0901.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import django.db.models.deletion
 from django.db import migrations, models
 
 import vng_api_common.fields
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0005_auto_20190506_0842")]
 
     operations = [
         migrations.AlterField(
             model_name="applicatie",
             name="client_ids",
             field=django.contrib.postgres.fields.ArrayField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0007_auto_20190506_1212.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0007_auto_20190506_1212.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.8 on 2019-05-06 12:12
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0006_auto_20190506_0901")]
 
     operations = [
         migrations.AddField(
             model_name="autorisatie",
             name="besluittype",
             field=models.URLField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0008_auto_20190712_1541.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0008_auto_20190712_1541.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.db import migrations, models
 
 import vng_api_common.fields
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0007_auto_20190506_1212")]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
             name="component",
             field=models.CharField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0009_update_enums.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0009_update_enums.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,10 +15,11 @@
         max_vertrouwelijkheidaanduiding=Lower(
             Replace(F("max_vertrouwelijkheidaanduiding"), Value(" "), Value("_"))
         ),
     )
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0008_auto_20190712_1541")]
 
     operations = [migrations.RunPython(forward, migrations.RunPython.noop)]
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0010_auto_20190712_1643.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0010_auto_20190712_1643.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.2 on 2019-07-12 14:43
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("authorizations", "0009_update_enums")]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
             name="api_root",
             field=models.URLField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0011_auto_20191114_0728.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0011_auto_20191114_0728.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     def patch_scope(self, scope: str) -> str:
         if not scope.startswith(f"{self.old}."):
             return scope
         return scope.replace(f"{self.old}.", f"{self.new}.", 1)
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("authorizations", "0010_auto_20190712_1643"),
     ]
 
     operations = [
         migrations.RunPython(
             Renamer("zaaktypes", "catalogi"),
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0012_auto_20200619_0545.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0012_auto_20200619_0545.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.6 on 2020-06-19 05:45
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("authorizations", "0011_auto_20191114_0728"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0013_auto_20201207_0846.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0013_auto_20201207_0846.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.8 on 2020-12-07 08:46
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("authorizations", "0012_auto_20200619_0545"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0014_auto_20201221_0905.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0014_auto_20201221_0905.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.14 on 2020-12-21 09:05
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("authorizations", "0013_auto_20201207_0846"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/migrations/0015_auto_20220318_1608.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/migrations/0015_auto_20220318_1608.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.2.27 on 2022-03-18 16:08
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("authorizations", "0014_auto_20201221_0905"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="authorizationsconfig",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/models.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,19 +19,14 @@
         default=ComponentTypes.zrc,
     )
 
     class Meta:
         verbose_name = _("Autorisatiecomponentconfiguratie")
 
 
-class ApplicatieManager(models.Manager):
-    def get_by_natural_key(self, uuid):
-        return self.get(uuid=uuid)
-
-
 class Applicatie(APIMixin, models.Model):
     """
     Client level of authorization
     """
 
     uuid = models.UUIDField(
         unique=True, default=uuid.uuid4, help_text="Unique resource identifier (UUID4)"
@@ -53,28 +48,18 @@
         help_text=_(
             "Indien alle autorisaties gegeven zijn, dan hoeven deze "
             "niet individueel opgegeven te worden. Gebruik dit alleen "
             "als je de consumer helemaal vertrouwt."
         ),
     )
 
-    objects = ApplicatieManager()
-
-    def natural_key(self):
-        return (str(self.uuid),)
-
     def __str__(self):
         return f"Applicatie ({self.label})"
 
 
-class AutorisatieManager(models.Manager):
-    def get_by_natural_key(self, applicatie, component, scopes):
-        return self.get(applicatie=applicatie, component=component, scopes=scopes)
-
-
 class Autorisatie(APIMixin, models.Model):
     applicatie = models.ForeignKey(
         "Applicatie",
         on_delete=models.CASCADE,
         related_name="autorisaties",
         verbose_name=_("applicatie"),
     )
@@ -120,23 +105,14 @@
 
     # ZRC & DRC exclusive
     max_vertrouwelijkheidaanduiding = VertrouwelijkheidsAanduidingField(
         help_text=_("Maximaal toegelaten vertrouwelijkheidaanduiding (inclusief)."),
         blank=True,
     )
 
-    objects = AutorisatieManager()
-
-    def natural_key(self):
-        return (
-            self.applicatie,
-            self.component,
-            self.scopes,
-        )
-
     def satisfy_vertrouwelijkheid(self, vertrouwelijkheidaanduiding: str) -> bool:
         max_confid_level = VertrouwelijkheidsAanduiding.get_choice(
             self.max_vertrouwelijkheidaanduiding
         ).order
         provided_confid_level = VertrouwelijkheidsAanduiding.get_choice(
             vertrouwelijkheidaanduiding
         ).order
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/serializers.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/serializers.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/authorizations/validators.py` & `commonground-api-common-1.9.0/vng_api_common/authorizations/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,28 @@
 
 
 class UniqueClientIDValidator:
     code = "clientId-exists"
     message = _(
         "The clientID(s) {client_id} are already used in application(s) {app_id}"
     )
-    requires_context = True
 
-    def __call__(self, value: List[str], serializer_field):
-        instance = getattr(serializer_field.parent, "instance", None)
+    def set_context(self, serializer_field):
+        """
+        This hook is called by the serializer instance,
+        prior to the validation call being made.
+        """
+        # Determine the existing instance, if this is an update operation.
+        self.instance = getattr(serializer_field.parent, "instance", None)
+
+    def __call__(self, value: List[str]):
         qs = Applicatie.objects.all()
 
-        if instance:
-            qs = qs.exclude(id=instance.id)
+        if self.instance:
+            qs = qs.exclude(id=self.instance.id)
 
         existing = qs.filter(client_ids__overlap=value).values_list(
             "uuid", "client_ids"
         )
         if existing:
             client_ids = set()
             for _existing in existing:
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/caching/__init__.py` & `commonground-api-common-1.9.0/vng_api_common/caching/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,13 @@
 an up to date version of the resource. It will reply with a HTTP 200 otherwise,
 including the ETag header.
 
 This package provides a model mixin to save the ETag header value to the db,
 and a decorator to enable conditional requests on viewsets. The rest are
 implementation details.
 """
-
 from .decorators import conditional_retrieve
 from .etags import calculate_etag
 from .models import ETagMixin
 
 # public API
 __all__ = ["ETagMixin", "calculate_etag", "conditional_retrieve"]
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/caching/decorators.py` & `commonground-api-common-1.9.0/vng_api_common/caching/decorators.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/caching/etags.py` & `commonground-api-common-1.9.0/vng_api_common/caching/etags.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,58 @@
 """
 Calculate ETag values for API resources.
 """
-
 import hashlib
 import logging
 from dataclasses import dataclass
 from typing import Optional
-from weakref import WeakKeyDictionary
 
 from django.conf import settings
+from django.contrib.sites.models import Site
 from django.core.exceptions import ObjectDoesNotExist
-from django.db import DatabaseError, models, transaction
+from django.db import models, transaction
 from django.http import Http404, HttpRequest
 
 from djangorestframework_camel_case.render import CamelCaseJSONRenderer
-from rest_framework import serializers
 from rest_framework.request import Request
 from rest_framework.settings import api_settings
 
-from ..utils import get_domain, get_resource_for_path
+from ..utils import get_resource_for_path
 from .registry import MODEL_SERIALIZERS
 
 logger = logging.getLogger(__name__)
 
-# entries are discarded when there are no hard references anymore to the model instance
-weak_object_serializers_dict = WeakKeyDictionary()
-
-
-def track_object_serializer(instance: models.Model, serializer: serializers.Serializer):
-    """
-    Track the serializer used for instance write.
-
-    This is a performance optimization trick - if we can extract the serializer instance
-    from the model instance used for the creation or update of the instance, we can
-    avoid multiple serializer rounds. Additionally, the serializer should already
-    contain context related to the request/domain.
-    """
-    existing = weak_object_serializers_dict.get(instance)
-    if existing and existing != serializer:
-        raise ValueError(
-            "The instance is already tracking a different serializer for "
-            "ETag calculation"
-        )
-    serializer_class = MODEL_SERIALIZERS[type(instance)]
-    if not isinstance(serializer, serializer_class):
-        raise TypeError(
-            "Cannot track serializer %r, expected a %r instance."
-            % (serializer, serializer_class)
-        )
-
-    weak_object_serializers_dict[instance] = serializer
-
 
 class StaticRequest(HttpRequest):
     def get_host(self) -> str:
-        return get_domain()
+        site = Site.objects.get_current()
+        return site.domain
 
     def _get_scheme(self) -> str:
         return "https" if settings.IS_HTTPS else "http"
 
 
-def get_etag_serializer(instance: models.Model) -> serializers.Serializer:
-    serializer = weak_object_serializers_dict.get(instance)
-    if serializer is not None:
-        return serializer
+def calculate_etag(instance: models.Model) -> str:
+    """
+    Calculate the MD5 hash of a resource representation in the API.
 
+    The serializer for the model class is retrieved, and then used to construct
+    the representation of the instance. Then, the representation is rendered
+    to camelCase JSON, after which the MD5 hash is calculated of this result.
+    """
     model_class = type(instance)
     serializer_class = MODEL_SERIALIZERS[model_class]
 
     # build a dummy request with the configured domain, since we're doing STRONG
     # comparison. Required as context for hyperlinked serializers
     request = Request(StaticRequest())
     request.version = api_settings.DEFAULT_VERSION
     request.versioning_scheme = api_settings.DEFAULT_VERSIONING_CLASS()
 
     serializer = serializer_class(instance=instance, context={"request": request})
-    return serializer
-
-
-def calculate_etag(instance: models.Model) -> str:
-    """
-    Calculate the MD5 hash of a resource representation in the API.
-
-    The serializer for the model class is retrieved, and then used to construct
-    the representation of the instance. Then, the representation is rendered
-    to camelCase JSON, after which the MD5 hash is calculated of this result.
-    """
-    serializer = get_etag_serializer(instance)
 
     # render the output to json, which is used as hash input
     renderer = CamelCaseJSONRenderer()
     rendered = renderer.render(serializer.data, "application/json")
 
     # calculate md5 hash
     return hashlib.md5(rendered).hexdigest()
@@ -153,42 +115,35 @@
         etag_update = cls(instance=obj, using=using)
 
         # we do not use the top-level transaction.commit, but need the underlying
         # connection object to ensure the update is only scheduled once.
         connection = transaction.get_connection(using)
 
         func = MethodCallback(etag_update.calculate_new_value)
-        for run_on_commit in connection.run_on_commit:
-            _func = run_on_commit[1]
+        for _, _func in connection.run_on_commit:
             if func == _func:
                 logger.debug(
                     "Update for model instance %r with pk %s was already scheduled",
                     type(obj),
                     obj.pk,
                 )
                 return
 
         logger.debug(
             "Scheduling model instance %r with pk %s for ETag update", type(obj), obj.pk
         )
-        # TODO: move this to celery to improve performance
         connection.on_commit(func)
 
     def calculate_new_value(self):
         with transaction.atomic(using=self.using):  # wrap in its own transaction
+            # check if the record still exists - it may have been deleted as part of a
+            # cascade delete, in which case we can't re-calculate and save anything.
+            try:
+                self.instance.refresh_from_db()
+            except self.instance.DoesNotExist:
+                return
+
             # track the actions _inside_ the on_commit handler, to prevent infinite
             # loops/stack overflows
-            try:
-                self.instance._updating_etag = True
-                self.instance.calculate_etag_value()
-            except DatabaseError as exc:
-                # the record may already have been deleted via a cascade delete. rather
-                # than always checking if the record still exists (which performs a query
-                # every time), we just try to update and see if it fails. The exception
-                # message is defined in django.db.models.base.Model._save_table
-                # TODO: see if we can tap into post_delete to remove the callback from
-                # the transaction.on_commit stack?
-                if exc.args[0] == "Save with update_fields did not affect any rows.":
-                    return
-                raise
-            finally:
-                del self.instance._updating_etag
+            self.instance._updating_etag = True
+            self.instance.calculate_etag_value()
+            del self.instance._updating_etag
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/caching/introspection.py` & `commonground-api-common-1.9.0/vng_api_common/caching/introspection.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/caching/models.py` & `commonground-api-common-1.9.0/vng_api_common/caching/models.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/caching/registry.py` & `commonground-api-common-1.9.0/vng_api_common/caching/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,41 +55,31 @@
     @property
     def affected_model(self) -> ModelBase:
         return self.field.model
 
     def __hash__(self):
         return hash(self.field)
 
-    def get_related_objects(
-        self,
-        instance: models.Model,
-        is_delete: bool = False,
-    ) -> Iterable[models.Model]:
+    def get_related_objects(self, instance: models.Model) -> Iterable[models.Model]:
         assert isinstance(
             instance, self.source_model
         ), "Instance is not of expected model class"
 
         reverse_relation_field = self.field.remote_field
 
         try:
             if isinstance(reverse_relation_field, ForeignObjectRel):
-                on_delete = self.field.remote_field.on_delete
                 query_like = getattr(
                     instance, reverse_relation_field.get_accessor_name()
                 )
             else:
-                on_delete = self.field.on_delete
                 query_like = getattr(instance, reverse_relation_field.name)
         except ObjectDoesNotExist:  # nullable OneToOneField, for example
             return []
 
-        if is_delete and on_delete is models.CASCADE:
-            # no point in trying to update records that will be cascade deleted
-            return []
-
         # reverse FK or m2m
         if isinstance(query_like, (models.Manager, models.QuerySet)):
             related_objects = query_like.all()
         # one-to-one field or FK
         else:
             related_objects = [query_like] if query_like is not None else []
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/caching/signals.py` & `commonground-api-common-1.9.0/vng_api_common/caching/signals.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,46 +2,43 @@
 Signals listen to changes in models using ETagMixin and models related to those.
 
 A changed m2m for example may affect the output of the ETag.
 
 The signal does nothing except clearing the calculated value, which will be
 re-calculated on the next fetch.
 """
-
 from typing import Optional, Set
 
 from django.core.exceptions import FieldDoesNotExist
 from django.db import models
 from django.db.models.base import ModelBase
 from django.db.models.signals import m2m_changed, post_delete, post_save
 from django.dispatch import receiver
 
 from .etags import EtagUpdate
 from .registry import DEPENDENCY_REGISTRY, Dependency
 
 
 def mark_affected_objects(
-    dependencies: Optional[Set[Dependency]],
-    instance: models.Model,
-    is_delete: bool = False,
+    dependencies: Optional[Set[Dependency]], instance: models.Model
 ):
     if dependencies is None:
         return
 
     for dependency in dependencies:
         if not is_etag_model(dependency.affected_model):
             continue
 
-        for obj in dependency.get_related_objects(instance, is_delete=is_delete):
+        for obj in dependency.get_related_objects(instance):
             EtagUpdate.mark_affected(obj)
 
 
 @receiver([post_save, post_delete])
 def mark_related_instances_for_etag_update(
-    sender: ModelBase, instance: models.Model, signal, **kwargs
+    sender: ModelBase, instance: models.Model, **kwargs
 ) -> None:
     """
     Determine which instances are affected by changes in ``instance``.
 
     The sender/instance may be a model supporting ETag-based caching, or may be related
     to such a model. We must determine which instances are affected and ensure that
     the ETag value is properly scheduled for re-computation based on the new data.
@@ -54,21 +51,20 @@
         return
 
     # prevent infinite recursion caused by the save of the new _etag value
     if kwargs.get("update_fields") == {"_etag"}:
         return
 
     # if the model is itself something that has an etag, mark it for update
-    is_delete = signal is post_delete
-    if is_etag_model(sender) and not is_delete:
+    if is_etag_model(sender) and not kwargs["signal"] is post_delete:
         EtagUpdate.mark_affected(instance)
 
     # otherwise, find out which relations are affected
     dependency_for = DEPENDENCY_REGISTRY.get(sender)
-    mark_affected_objects(dependency_for, instance, is_delete=is_delete)
+    mark_affected_objects(dependency_for, instance)
 
 
 @receiver(m2m_changed)
 def mark_m2m_related_instances_for_etag_update(
     sender: ModelBase,
     instance: models.Model,
     action: str,
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/checks.py` & `commonground-api-common-1.9.0/vng_api_common/checks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from typing import Any
 
 from django.core.checks import Warning, register
-from django.db.models import Choices
+
+from djchoices import DjangoChoices
 
 from .utils import get_subclasses
 
 ENUM_VALUE_PATTERN = re.compile(r"^[a-z_0-9]+$", re.ASCII)
 
 
 def enum_value_ok(value: Any) -> bool:
@@ -23,16 +24,16 @@
 @register()
 def check_lowercased_constants(app_configs, **kwargs):
     """
     Check that enum values have lowercased, underscore only values.
     """
     warnings = []
 
-    for klass in get_subclasses(Choices):
-        enum_values = klass.values
+    for klass in get_subclasses(DjangoChoices):
+        enum_values = klass.values.keys()
         if any((not enum_value_ok(value) for value in enum_values)):
             warnings.append(
                 Warning(
                     "Choices %s.%s has at least one value that is not lowercased/underscore ascii only"
                     % (klass.__module__, klass.__name__),
                     hint="Lower case the values and replace dashes/spaces with underscores",
                     obj=klass,
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/client.py` & `commonground-api-common-1.9.0/vng_api_common/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Interface to get a zds_client object for a given URL.
 """
-
 from typing import Optional
 
 from django.apps import apps
 from django.conf import settings
 from django.utils.module_loading import import_string
 
 from zds_client import Client
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/compat.py` & `commonground-api-common-1.9.0/vng_api_common/compat.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/conf/api.py` & `commonground-api-common-1.9.0/vng_api_common/conf/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     "GEMMA_URL_COMPONENTTYPE",
     "GEMMA_URL_INFORMATIEMODEL",
     "GEMMA_URL_INFORMATIEMODEL_VERSIE",
     "REDOC_SETTINGS",
     "NOTIFICATIONS_KANAAL",
     "NOTIFICATIONS_DISABLED",
     "JWT_LEEWAY",
-    "COMMONGROUND_API_COMMON_GET_DOMAIN",
 ]
 
 API_VERSION = "1.0.0-rc1"  # semantic version
 
 BASE_REST_FRAMEWORK = {
     "DEFAULT_RENDERER_CLASSES": (
         "djangorestframework_camel_case.render.CamelCaseJSONRenderer",
@@ -107,9 +106,7 @@
 NOTIFICATIONS_DISABLED = False
 
 vng_repo = "VNG-Realisatie/vng-api-common"
 vng_branch = "ref-responses"
 COMMON_SPEC = f"https://raw.githubusercontent.com/{vng_repo}/feature/{vng_branch}/vng_api_common/schemas/common.yaml"
 
 JWT_LEEWAY = 0  # default in PyJWT
-
-COMMONGROUND_API_COMMON_GET_DOMAIN = "vng_api_common.utils.get_site_domain"
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/db/operations.py` & `commonground-api-common-1.9.0/vng_api_common/db/operations.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/descriptors.py` & `commonground-api-common-1.9.0/vng_api_common/descriptors.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/doc.py` & `commonground-api-common-1.9.0/vng_api_common/doc.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/exception_handling.py` & `commonground-api-common-1.9.0/vng_api_common/exception_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 def get_validation_errors(validation_errors: dict):
     for field_name, error_list in validation_errors.items():
         # nested validation for fields where many=True
         if isinstance(error_list, list):
             for i, nested_error_dict in enumerate(error_list):
                 if isinstance(nested_error_dict, dict):
                     for err in get_validation_errors(nested_error_dict):
-                        err["name"] = (
-                            f"{underscore_to_camel(field_name)}.{i}.{err['name']}"
-                        )
+                        err[
+                            "name"
+                        ] = f"{underscore_to_camel(field_name)}.{i}.{err['name']}"
                         yield err
 
         # nested validation - recursively call the function
         if isinstance(error_list, dict):
             for err in get_validation_errors(error_list):
                 err["name"] = f"{underscore_to_camel(field_name)}.{err['name']}"
                 yield err
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/exceptions.py` & `commonground-api-common-1.9.0/vng_api_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/fields.py` & `commonground-api-common-1.9.0/vng_api_common/fields.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/filters.py` & `commonground-api-common-1.9.0/vng_api_common/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .utils import NotAViewSet, get_resource_for_path
 from .validators import validate_rsin
 
 logger = logging.getLogger(__name__)
 
 
 class Backend(DjangoFilterBackend):
+
     # Taken from drf_yasg.inspectors.field.CamelCaseJSONFilter
     def _is_camel_case(self, view):
         return any(
             issubclass(parser, CamelCaseJSONParser) for parser in view.parser_classes
         ) or any(
             issubclass(renderer, CamelCaseJSONRenderer)
             for renderer in view.renderer_classes
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/filtersets.py` & `commonground-api-common-1.9.0/vng_api_common/filtersets.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/generators.py` & `commonground-api-common-1.9.0/vng_api_common/generators.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/geo.py` & `commonground-api-common-1.9.0/vng_api_common/geo.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/inspectors/cache.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/cache.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/inspectors/fields.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/fields.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/inspectors/files.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/files.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/inspectors/geojson.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/geojson.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/inspectors/polymorphic.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/polymorphic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Introspect polymorphic resources
 
 Bulk of the code taken from https://github.com/axnsan12/drf-yasg/issues/100
 """
-
 from drf_yasg import openapi
 from drf_yasg.errors import SwaggerGenerationError
 from drf_yasg.inspectors.base import NotHandled
 from drf_yasg.inspectors.field import (
     CamelCaseJSONFilter,
     ReferencingSerializerInspector,
 )
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/inspectors/query.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.db import models
-from django.utils.encoding import force_str
+from django.utils.encoding import force_text
 from django.utils.translation import gettext as _
 
 from django_filters.filters import BaseCSVFilter, ChoiceFilter
 from drf_yasg import openapi
 from drf_yasg.inspectors.query import CoreAPICompatInspector
 from rest_framework.filters import OrderingFilter
 
@@ -21,15 +21,15 @@
     def get_filter_parameters(self, filter_backend):
         fields = super().get_filter_parameters(filter_backend)
         if isinstance(filter_backend, OrderingFilter):
             return fields
 
         if fields:
             queryset = self.view.get_queryset()
-            filter_class = filter_backend.get_filterset_class(self.view, queryset)
+            filter_class = filter_backend.get_filter_class(self.view, queryset)
 
             for parameter in fields:
                 filter_field = filter_class.base_filters[parameter.name]
                 model_field = get_target_field(queryset.model, parameter.name)
                 parameter._filter_field = filter_field
 
                 help_text = filter_field.extra.get(
@@ -68,15 +68,15 @@
                     parameter.enum = [
                         choice[0] for choice in filter_field.extra["choices"]
                     ]
                 elif model_field and isinstance(model_field, models.URLField):
                     parameter.format = openapi.FORMAT_URI
 
                 if not parameter.description and help_text:
-                    parameter.description = force_str(help_text)
+                    parameter.description = force_text(help_text)
 
                 if "max_length" in filter_field.extra:
                     parameter.max_length = filter_field.extra["max_length"]
                 if "min_length" in filter_field.extra:
                     parameter.min_length = filter_field.extra["min_length"]
 
         return fields
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/inspectors/utils.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/utils.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/inspectors/view.py` & `commonground-api-common-1.9.0/vng_api_common/inspectors/view.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/locale/nl/LC_MESSAGES/django.mo` & `commonground-api-common-1.9.0/vng_api_common/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/locale/nl/LC_MESSAGES/django.po` & `commonground-api-common-1.9.0/vng_api_common/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/management/commands/generate_autorisaties.py` & `commonground-api-common-1.9.0/vng_api_common/management/commands/generate_autorisaties.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/management/commands/generate_notificaties.py` & `commonground-api-common-1.9.0/vng_api_common/management/commands/generate_notificaties.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/management/commands/generate_swagger.py` & `commonground-api-common-1.9.0/vng_api_common/management/commands/generate_swagger.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/management/commands/patch_error_contenttypes.py` & `commonground-api-common-1.9.0/vng_api_common/management/commands/patch_error_contenttypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Patch the content-type of error responses.
 
 Due to the changes between Swagger 2.0 and OpenAPI 3.0, we cannot handle
 this at the Python level.
 """
-
 from django.core.management import BaseCommand
 
 import oyaml as yaml
 
 from ...views import ERROR_CONTENT_TYPE
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/management/commands/use_external_components.py` & `commonground-api-common-1.9.0/vng_api_common/management/commands/use_external_components.py`

 * *Files identical despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Replace internal references to external for reusable components
 
 Due to the limitations of drf_yasg we cannot handle this at the Python level
 """
-
 import os.path
 
 from django.conf import settings
 from django.core.management import BaseCommand
 
 import oyaml as yaml
 import requests
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/middleware.py` & `commonground-api-common-1.9.0/vng_api_common/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # https://pyjwt.readthedocs.io/en/latest/usage.html#reading-headers-without-validation
 # -> we can put the organization/service in the headers itself
 import logging
-from typing import Any, Dict, Iterable, List, Optional
+from typing import Any, Dict, List, Optional
 
 from django.conf import settings
 from django.db import models, transaction
 from django.db.models import QuerySet
 from django.utils.translation import gettext as _
 
 import jwt
@@ -24,15 +24,15 @@
 
 
 class JWTAuth:
     def __init__(self, encoded: str = None):
         self.encoded = encoded
 
     @property
-    def applicaties(self) -> Iterable[Applicatie]:
+    def applicaties(self) -> Optional[list]:
         if self.client_id is None:
             return []
 
         applicaties = self._get_auth()
 
         if not applicaties:
             auth_data = self._request_auth()
@@ -134,15 +134,15 @@
                 key = jwt_secret.secret
 
             # check signature of the token
             try:
                 payload = jwt.decode(
                     self.encoded,
                     key,
-                    algorithms=["HS256"],
+                    algorithms="HS256",
                     leeway=settings.JWT_LEEWAY,
                 )
             except jwt.InvalidSignatureError:
                 logger.exception("Invalid signature - possible payload tampering?")
                 raise PermissionDenied(
                     "Client credentials zijn niet geldig", code="invalid-jwt-signature"
                 )
@@ -157,15 +157,15 @@
             return None
         return self.payload["client_id"]
 
     def filter_vertrouwelijkheidaanduiding(self, base: QuerySet, value) -> QuerySet:
         if value is None:
             return base
 
-        order_provided = VertrouwelijkheidsAanduiding.get_choice_order(value)
+        order_provided = VertrouwelijkheidsAanduiding.get_choice(value).order
         order_case = VertrouwelijkheidsAanduiding.get_order_expression(
             "max_vertrouwelijkheidaanduiding"
         )
 
         # In this case we are filtering Autorisatie model to look for auth which meets our needs.
         # Therefore we're only considering authorizations here that have a max_vertrouwelijkheidaanduiding
         # bigger or equal than what we're checking for the object.
@@ -211,14 +211,15 @@
             for autorisatie in autorisaties:
                 scopes_provided.update(autorisatie.scopes)
 
         return scopes.is_contained_in(list(scopes_provided))
 
 
 class AuthMiddleware:
+
     header = "HTTP_AUTHORIZATION"
     auth_type = "Bearer"
 
     def __init__(self, get_response=None):
         self.get_response = get_response
 
     def __call__(self, request):
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/migrations/0001_initial.py` & `commonground-api-common-1.9.0/vng_api_common/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.6 on 2018-11-05 15:27
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="JWTSecret",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/migrations/0002_apicredential.py` & `commonground-api-common-1.9.0/vng_api_common/migrations/0002_apicredential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.6 on 2018-11-19 11:09
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("vng_api_common", "0001_initial")]
 
     operations = [
         migrations.CreateModel(
             name="APICredential",
             fields=[
                 (
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/migrations/0003_auto_20190417_1145.py` & `commonground-api-common-1.9.0/vng_api_common/migrations/0003_auto_20190417_1145.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-04-17 11:45
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("vng_api_common", "0002_apicredential")]
 
     operations = [
         migrations.AlterModelOptions(
             name="apicredential",
             options={
                 "verbose_name": "external API credential",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/migrations/0004_auto_20190517_0903.py` & `commonground-api-common-1.9.0/vng_api_common/migrations/0004_auto_20190517_0903.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-05-17 09:03
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("vng_api_common", "0003_auto_20190417_1145")]
 
     operations = [
         migrations.AddField(
             model_name="apicredential",
             name="user_id",
             field=models.CharField(default="", max_length=255, verbose_name="user id"),
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/migrations/0005_auto_20190614_1346.py` & `commonground-api-common-1.9.0/vng_api_common/migrations/0005_auto_20190614_1346.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.1 on 2019-06-14 13:46
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("vng_api_common", "0004_auto_20190517_0903")]
 
     operations = [
         migrations.AlterField(
             model_name="apicredential",
             name="api_root",
             field=models.URLField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/mocks.py` & `commonground-api-common-1.9.0/vng_api_common/mocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         return self.data.get(resource)[index]
 
     def create(self, resource: str, *args, **kwargs):
         return self.data.get(resource, {})
 
 
 class ZTCMockClient(MockClient):
+
     data = {
         "statustype": [
             {
                 "url": "https://ztc/api/v1/catalogussen/{catalogus_uuid}/zaaktypen/{zaaktype_uuid}/statustypen/{uuid}",
                 "volgnummer": 1,
                 "isEindstatus": False,
             },
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/models.py` & `commonground-api-common-1.9.0/vng_api_common/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,14 @@
         reverse_kwargs = {"uuid": self.uuid}
         reverse_kwargs.update(**kwargs)
 
         url = reverse(f"{resource_name}-detail", kwargs=reverse_kwargs, request=request)
         return url
 
 
-class JWTSecretManager(models.Manager):
-    def get_by_natural_key(self, identifier):
-        return self.get(identifier=identifier)
-
-
 class JWTSecret(models.Model):
     """
     Store credentials of clients that want to access our API.
 
     Only clients that are known can access the API (if so configured).
     """
 
@@ -54,19 +49,14 @@
             "Client ID to identify external API's and applications that access this API."
         ),
     )
     secret = models.CharField(
         _("secret"), max_length=255, help_text=_("Secret belonging to the client ID.")
     )
 
-    objects = JWTSecretManager()
-
-    def natural_key(self):
-        return (self.identifier,)
-
     class Meta:
         verbose_name = _("client credential")
         verbose_name_plural = _("client credentials")
 
     def __str__(self):
         return self.identifier
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/notifications/api/views.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/api/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     """
     Abstract view to receive webhooks
     """
 
     swagger_schema = None
 
     permission_classes = (AuthScopesRequired,)
-    required_scopes = Scope(SCOPE_NOTIFICATIES_PUBLICEREN_LABEL, private=True)
+    required_scopes = Scope(
+        SCOPE_NOTIFICATIES_PUBLICEREN_LABEL
+    )  # FIXME: this should be standalone!
 
     def get_serializer(self, *args, **kwargs):
         return NotificatieSerializer(*args, **kwargs)
 
     @swagger_auto_schema(
         responses={
             204: "",
@@ -49,17 +51,15 @@
     def handle_notification(self, message):
         raise NotImplementedError("You must implemented `handle_notification`")
 
 
 class NotificationView(NotificationBaseView):
     action = "create"
     permission_classes = (AuthScopesRequired,)
-    required_scopes = {
-        "create": Scope(SCOPE_NOTIFICATIES_PUBLICEREN_LABEL, private=True)
-    }
+    required_scopes = {"create": Scope(SCOPE_NOTIFICATIES_PUBLICEREN_LABEL)}
 
     def create(self, request, *args, **kwargs):
         return self.post(request, *args, **kwargs)
 
     def handle_notification(self, message: dict) -> None:
         _handler = getattr(
             settings,
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/notifications/handlers.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/handlers.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0001_initial.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import django.contrib.postgres.fields
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="NotificationsConfig",
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0002_subscription__subscription.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0002_subscription__subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-03-12 10:36
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("notifications", "0001_initial")]
 
     operations = [
         migrations.AddField(
             model_name="subscription",
             name="_subscription",
             field=models.URLField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0003_auto_20190319_1048.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0003_auto_20190319_1048.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.1 on 2019-03-19 09:48
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("notifications", "0002_subscription__subscription")]
 
     operations = [
         migrations.RenameField(
             model_name="notificationsconfig", old_name="location", new_name="api_root"
         ),
         migrations.AddField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0004_auto_20190325_1313.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0004_auto_20190325_1313.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.0.13 on 2019-03-25 13:13
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("notifications", "0003_auto_20190319_1048")]
 
     operations = [
         migrations.AlterField(
             model_name="notificationsconfig",
             name="api_root",
             field=models.URLField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0005_fix_default_nrc.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0005_fix_default_nrc.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 
     if config.api_root == "https://ref.tst.vng.cloud/nc/api/v1":
         config.api_root = "https://ref.tst.vng.cloud/nrc/api/v1"
         config.save()
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("notifications", "0004_auto_20190325_1313")]
 
     operations = [migrations.RunPython(fix_config, migrations.RunPython.noop)]
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0006_auto_20190417_1142.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0009_auto_20190729_0427.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Generated by Django 2.0.13 on 2019-04-17 11:42
+# Generated by Django 2.1.8 on 2019-07-29 04:27
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-    dependencies = [("notifications", "0005_fix_default_nrc")]
+
+    dependencies = [("notifications", "0008_auto_20190502_0415")]
 
     operations = [
-        migrations.RemoveField(model_name="notificationsconfig", name="client_id"),
-        migrations.RemoveField(model_name="notificationsconfig", name="secret"),
         migrations.AlterField(
             model_name="notificationsconfig",
             name="api_root",
             field=models.URLField(
-                default="https://ref.tst.vng.cloud/nrc/api/v1",
+                default="https://notificaties-api.vng.cloud/api/v1/",
                 unique=True,
                 verbose_name="api root",
             ),
-        ),
+        )
     ]
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0008_auto_20190502_0415.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0008_auto_20190502_0415.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 2.1.8 on 2019-05-02 04:15
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [("notifications", "0007_auto_20190429_1442")]
 
     operations = [
         migrations.AlterField(
             model_name="notificationsconfig",
             name="api_root",
             field=models.URLField(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/notifications/migrations/0010_auto_20220704_1419.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/migrations/0010_auto_20220704_1419.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
             )
         old_subscriptions.delete()
 
     return migrate_data
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("notifications", "0009_auto_20190729_0427"),
         ("notifications_api_common", "0001_initial"),
     ]
 
     operations = [
         migrations.RunPython(
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/notifications/models.py` & `commonground-api-common-1.9.0/vng_api_common/notifications/models.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/oas.py` & `commonground-api-common-1.9.0/vng_api_common/oas.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Utility module for Open API Specification 3.0.x.
 
 This should get merged into gemma-zds-client, but some heavy refactoring is
 needed for that.
 """
-
 from typing import Union
 
 import requests
 import yaml
 from drf_yasg import openapi
 
 TYPE_MAP = {
@@ -70,18 +69,14 @@
 
         value = obj[prop]
 
         # TODO Handling references not yet implemented
         if "$ref" in prop_schema:
             continue
 
-        # TODO Handling allOf and oneOf not yet implemented
-        if "allOf" in prop_schema or "oneOf" in prop_schema:
-            continue
-
         # Allow None if property is nullable
         if value is None:
             if prop_schema.get("nullable", False):
                 continue
             else:
                 return False
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/permissions.py` & `commonground-api-common-1.9.0/vng_api_common/permissions.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/polymorphism.py` & `commonground-api-common-1.9.0/vng_api_common/polymorphism.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 ...             'common_field',
 ...         )
 ...
 
 The serializer output will then either contain ``field_for_value2`` or
 ``field_for_value2``, depending on the value of the field ``type``.
 """
-
 import logging
 from collections import OrderedDict
 from typing import Any, Dict, Union
 
 from django.core.exceptions import FieldDoesNotExist
 
 from rest_framework import serializers
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/routers.py` & `commonground-api-common-1.9.0/vng_api_common/routers.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/schema.py` & `commonground-api-common-1.9.0/vng_api_common/schema.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/scopes.py` & `commonground-api-common-1.9.0/vng_api_common/scopes.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/search.py` & `commonground-api-common-1.9.0/vng_api_common/search.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/serializers.py` & `commonground-api-common-1.9.0/vng_api_common/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import datetime
 import inspect
 from collections import OrderedDict
-from typing import List, Optional, Tuple, Union
+from typing import Optional, Tuple, Union
 
-from django.db import models, transaction
+from django.db import transaction
 from django.utils.translation import gettext_lazy as _
 
 import isodate
+from djchoices import DjangoChoices
 from rest_framework import fields, serializers
 
-from .choices import TextChoicesWithDescriptions
 from .descriptors import GegevensGroepType
 
 try:
     # 1.1.x
     from relativedeltafield.utils import format_relativedelta, relativedelta
 except ImportError:
     try:
@@ -86,29 +86,31 @@
     )
 
 
 class ValidatieFoutSerializer(FoutSerializer):
     invalid_params = FieldValidationErrorSerializer(many=True)
 
 
-def add_choice_values_help_text(
-    choices: Union[models.Choices, List[Tuple[str, str]]]
-) -> str:
-    is_dj_choices = inspect.isclass(choices) and issubclass(choices, models.Choices)
-
-    if is_dj_choices:
-        _choices = choices.choices
-        if issubclass(choices, TextChoicesWithDescriptions):
-            descriptions = choices.descriptions()
-            _choices = [
-                (key, f"({value}) {descriptions[key]}") for key, value in _choices
-            ]
-    else:
-        _choices = choices
-    items = [f"* `{key}` - {value}" for key, value in _choices]
+def add_choice_values_help_text(choices: Union[DjangoChoices, Tuple[str, str]]) -> str:
+    items = []
+
+    is_dj_choices = inspect.isclass(choices) and issubclass(choices, DjangoChoices)
+    _choices = choices.choices if is_dj_choices else choices
+
+    for key, value in _choices:
+        description = (
+            getattr(choices.get_choice(key), "description", None)
+            if is_dj_choices
+            else None
+        )
+        if description:
+            item = f"* `{key}` - ({value}) {description}"
+        else:
+            item = f"* `{key}` - {value}"
+        items.append(item)
 
     return "Uitleg bij mogelijke waarden:\n\n" + "\n".join(items)
 
 
 class GegevensGroepSerializerMetaclass(serializers.SerializerMetaclass):
     def __new__(cls, name, bases, attrs):
         Meta = attrs.get("Meta")
@@ -236,35 +238,34 @@
     Usage: include the mixin on the ModelSerializer that has gegevensgroepen.
     """
 
     def _is_gegevensgroep(self, name: str):
         attr = getattr(self.Meta.model, name)
         return isinstance(attr, GegevensGroepType)
 
+    @transaction.atomic
     def create(self, validated_data):
         """
         Handle nested writes.
         """
         gegevensgroepen = {}
+
         for name in list(validated_data.keys()):
             if not self._is_gegevensgroep(name):
                 continue
 
             gegevensgroepen[name] = validated_data.pop(name)
 
-        # avoid a number of queries if there's no gegevensgroep actions to perform
-        if not gegevensgroepen:
-            return super().create(validated_data)
-
-        with transaction.atomic():
-            # perform the default create
-            obj = super().create(validated_data)
-            for name, gegevensgroepdata in gegevensgroepen.items():
-                setattr(obj, name, gegevensgroepdata)
-            obj.save()
+        # perform the default create
+        obj = super().create(validated_data)
+
+        for name, gegevensgroepdata in gegevensgroepen.items():
+            setattr(obj, name, gegevensgroepdata)
+
+        obj.save()
 
         return obj
 
     def update(self, instance, validated_data):
         """
         Handle nested writes.
         """
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/css/admin/admin_overrides.css` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/css/admin/admin_overrides.css`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/img/vng.svg` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/img/vng.svg`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.css` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.css`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.min.css` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff2` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.eot` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.svg` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.ttf` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2` & `commonground-api-common-1.9.0/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/admin/base_site.html` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/index.html` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/index.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,64 @@
 {% extends "vng_api_common/master.html" %}
 
 {% block content %}
 
-  <div class="header">
-    <h1 class="header__title">{{ settings.PROJECT_NAME }} startpunt</h1>
-    <p class="header__description">{{ settings.SITE_TITLE }}</p>
+  <div class="px-3 py-3 pt-md-5 pb-md-4 mx-auto text-center">
+    <h1 class="display-4">{{ settings.PROJECT_NAME }} startpunt</h1>
+    <p class="lead">{{ settings.SITE_TITLE }}</p>
   </div>
 
-  <div class="container container--center">
+  <div class="container text-center">
 
     {% block docs %}
 
       <h2>Documentatie</h2>
 
-      <div class="cardlist">
+      <div class="row justify-content-md-center">
 
         {% block docs_oas %}
-          <div class="cardlist__item">
+          <div class="col-sm-4">
+
             <div class="card">
-              <h5 class="card__title"><i class="fas fa-wifi"></i> API specificatie</h5>
-              <p>Technische API documentatie in de vorm van een Open API Specificatie (OAS).</p>
-              <a href="https://redocly.github.io/redoc/?url={{ settings.GITHUB_API_SPEC }}" class="button button--primary">API specificaties</a>
+              <div class="card-body">
+                <h5 class="card-title"><i class="fas fa-wifi"></i> API specificatie</h5>
+                <p class="card-text">Technische API documentatie in de vorm van een Open API Specificatie (OAS).</p>
+                <a href="https://redocly.github.io/redoc/?url={{ settings.GITHUB_API_SPEC }}" class="btn btn-primary">API specificaties</a>
+              </div>
             </div>
+
           </div>
         {% endblock %}
 
         {% block docs_scopes %}
-          <div class="cardlist__item">
+          <div class="col-sm-4">
+
             <div class="card">
-              <h5 class="card__title"><i class="fas fa-shield-alt"></i> API scopes</h5>
-              <p>Alle scopes binnen deze API voor gebruik in JWT's t.b.v. autorisaties.</p>
-              <a href="https://github.com/{{ settings.SELF_REPO }}/blob/{{ settings.SELF_BRANCH }}/src/autorisaties.md" class="button button--primary">API scopes</a>
+              <div class="card-body">
+                <h5 class="card-title"><i class="fas fa-shield-alt"></i> API scopes</h5>
+                <p class="card-text">Alle scopes binnen deze API voor gebruik in JWT's t.b.v. autorisaties.</p>
+                <a href="https://github.com/{{ settings.SELF_REPO }}/blob/{{ settings.SELF_BRANCH }}/src/autorisaties.md" class="btn btn-primary">API scopes</a>
+              </div>
             </div>
+
           </div>
        {% endblock %}
 
        {% block extra_docs %}{% endblock %}
 
      </div>
+     <p></p>
 
     {% endblock %}
 
     {% block extra_content %}{% endblock %}
 
     {% block admin_link %}
+      <p></p>
       <p>
-        <a href="{% url 'admin:index' %}" class="button button--alert"><i class="fas fa-lock"></i> Beheer</a>
+        <a href="{% url 'admin:index' %}" class="btn btn-sm btn-danger"><i class="fas fa-lock"></i> Beheer</a>
       </p>
     {% endblock %}
 
   </div>
 
 {% endblock %}
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/notificaties.md` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/notificaties.md`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/templates/vng_api_common/ref/error_detail.html` & `commonground-api-common-1.9.0/vng_api_common/templates/vng_api_common/ref/error_detail.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends "vng_api_common/master.html" %}
 {% load markup_tags %}
 
 {% block content %}
 
-  <div class="header">
-    <h1 class="header__title">{{ settings.PROJECT_NAME }} foutomschrijving</h1>
-    <p class="header__description">{{ settings.SITE_TITLE }}</p>
+  <div class="px-3 py-3 pt-md-5 pb-md-4 mx-auto text-center">
+    <h1 class="display-4">{{ settings.PROJECT_NAME }} foutomschrijving</h1>
+    <p class="lead">{{ settings.SITE_TITLE }}</p>
   </div>
 
   <div class="container">
 
     <h2><code>{{ type }}</code> fouttype</h2>
 
     <dl class="error-detail-properties">
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/templatetags/vng_api_common.py` & `commonground-api-common-1.9.0/vng_api_common/templatetags/vng_api_common.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/tests/auth.py` & `commonground-api-common-1.9.0/vng_api_common/tests/auth.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/tests/caching.py` & `commonground-api-common-1.9.0/vng_api_common/tests/caching.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/tests/schema.py` & `commonground-api-common-1.9.0/vng_api_common/tests/schema.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/tests/urls.py` & `commonground-api-common-1.9.0/vng_api_common/tests/urls.py`

 * *Files identical despite different names*

### Comparing `commonground_api_common-1.13.1/vng_api_common/utils.py` & `commonground-api-common-1.9.0/vng_api_common/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import logging
 import re
 import uuid
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from django.apps import apps
 from django.conf import settings
-from django.core.exceptions import ImproperlyConfigured
 from django.db import models
 from django.http import HttpRequest
 from django.urls import Resolver404, ResolverMatch, get_resolver, get_script_prefix
 from django.utils.encoding import smart_str
-from django.utils.module_loading import import_string
 
 from rest_framework.utils import formatting
 from zds_client.client import ClientError
 
 from .client import get_client
 
 try:
@@ -210,22 +208,23 @@
     model_name = getattr(model, "IDENTIFICATIE_PREFIX", model._meta.model_name.upper())
 
     year = getattr(instance, date_field_name).year
     prefix = f"{model_name}-{year}"
 
     pattern = prefix + r"-\d{10}"
 
-    # ⚡ start_with is added to use index in DB query
-    issued_ids_for_year = model._default_manager.filter(
-        identificatie__startswith=prefix, identificatie__regex=pattern
-    )
-    max_id = issued_ids_for_year.aggregate(models.Max("identificatie"))[
-        "identificatie__max"
-    ]
-    number = int(max_id.split("-")[-1]) + 1 if max_id is not None else 1
+    issued_ids_for_year = model._default_manager.filter(identificatie__regex=pattern)
+
+    if issued_ids_for_year.exists():
+        max_id = issued_ids_for_year.aggregate(models.Max("identificatie"))[
+            "identificatie__max"
+        ]
+        number = int(max_id.split("-")[-1]) + 1
+    else:
+        number = 1
 
     padded_number = str(number).zfill(10)
     return f"{prefix}-{padded_number}"
 
 
 def get_help_text(model_string: str, field_name: str) -> str:
     ModelClass = apps.get_model(model_string, require_ready=False)
@@ -266,34 +265,7 @@
 
 def get_field_attribute(
     model_string: str, field_name: str, attr_name: str
 ) -> Optional[str]:
     ModelClass = apps.get_model(model_string, require_ready=False)
     field = ModelClass._meta.get_field(field_name)
     return getattr(field, attr_name, None)
-
-
-def get_domain() -> str:
-    """
-    Derive the domain where the application is hosted.
-    """
-    getter = import_string(settings.COMMONGROUND_API_COMMON_GET_DOMAIN)
-    return getter()
-
-
-def get_site_domain() -> str:
-    """
-    Derive the domain where the application is hosted.
-
-    You can provide an alternative implementation via the
-    ``COMMONGROUND_API_COMMON_GET_DOMAIN`` setting, which takes a dotted path to a
-    callable taking no arguments.
-    """
-    if not apps.is_installed("django.contrib.sites"):
-        raise ImproperlyConfigured(
-            "'django.contrib.sites' is not installed in INSTALLED_APPS"
-        )
-
-    from django.contrib.sites.models import Site
-
-    site = Site.objects.get_current()
-    return site.domain
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/validators.py` & `commonground-api-common-1.9.0/vng_api_common/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,19 +39,17 @@
     def __call__(self, value):
         stripped_value = value[self.start :]
         match = WORD_REGEX.match(stripped_value)
         if not match:
             raise ValidationError(
                 'Waarde "{0}" mag geen diakrieten of non-ascii tekens bevatten{1}'.format(
                     value,
-                    (
-                        " na de eerste {0} karakters".format(self.start)
-                        if self.start
-                        else ""
-                    ),
+                    " na de eerste {0} karakters".format(self.start)
+                    if self.start
+                    else "",
                 )
             )
 
     def __eq__(self, other):
         return (
             isinstance(other, AlphanumericExcludingDiacritic)
             and self.start == other.start
@@ -202,44 +200,51 @@
                 self.__message.format(url=url, resource=self.resource), code=self.__code
             )
 
         return obj
 
 
 class InformatieObjectUniqueValidator(validators.UniqueTogetherValidator):
-    requires_context = True
-
     def __init__(self, parent_field, field: str):
         self.parent_field = parent_field
         self.field = field
         super().__init__(None, (parent_field, field))
 
-    def __call__(self, informatieobject: str, serializer):
-        attrs = {
-            self.parent_field: serializer.context["parent_object"],
-            self.field: informatieobject,
-        }
+    def set_context(self, serializer_field):
+        serializer = serializer_field.parent
+        super().set_context(serializer)
+
+        self.queryset = serializer.Meta.model._default_manager.all()
+        self.parent_object = serializer.context["parent_object"]
+
+    def __call__(self, informatieobject: str):
+        attrs = {self.parent_field: self.parent_object, self.field: informatieobject}
         super().__call__(attrs)
 
 
 class ObjectInformatieObjectValidator:
     """
     Validate that the INFORMATIEOBJECT is linked already in the DRC.
     """
 
     message = _(
         "Het informatieobject is in het DRC nog niet gerelateerd aan dit object."
     )
     code = "inconsistent-relation"
-    requires_context = True
 
-    def __call__(self, informatieobject: str, serializer):
-        object_url = serializer.context["parent_object"].get_absolute_api_url(
-            self.request
-        )
+    def set_context(self, serializer):
+        """
+        This hook is called by the serializer instance,
+        prior to the validation call being made.
+        """
+        self.parent_object = serializer.context["parent_object"]
+        self.request = serializer.context["request"]
+
+    def __call__(self, informatieobject: str):
+        object_url = self.parent_object.get_absolute_api_url(self.request)
 
         # dynamic so that it can be mocked in tests easily
         client = get_client(informatieobject)
 
         try:
             oios = client.list(
                 "objectinformatieobject",
@@ -300,41 +305,48 @@
 
     :param organisatie_field: naam van het veld dat de organisatie RSIN bevat
     :param identificatie_field: naam van het veld dat de identificatie bevat
     """
 
     message = _("Deze identificatie bestaat al binnen de organisatie")
     code = "identificatie-niet-uniek"
-    requires_context = True
 
     def __init__(self, organisatie_field: str, identificatie_field="identificatie"):
         self.organisatie_field = organisatie_field
         self.identificatie_field = identificatie_field
 
-    def __call__(self, attrs: dict, serializer):
-        instance = getattr(serializer, "instance", None)
+    def set_context(self, serializer):
+        """
+        This hook is called by the serializer instance,
+        prior to the validation call being made.
+        """
+        # Determine the existing instance, if this is an update operation.
+        self.instance = getattr(serializer, "instance", None)
+        self.model = serializer.Meta.model
+
+    def __call__(self, attrs: dict):
         identificatie = attrs.get(self.identificatie_field)
         if not identificatie:
-            if instance:
+            if self.instance:
                 # In case of a partial update
-                identificatie = instance.identificatie
+                identificatie = self.instance.identificatie
             else:
                 # identification is being generated, and the generation checks for
                 # uniqueness
                 return
 
         organisatie = attrs.get(self.organisatie_field)
-        pk = instance.pk if instance else None
+        pk = self.instance.pk if self.instance else None
 
         # if we're updating an instance, setting the current values will not
         # trigger an error because the instance-to-be-updated is excluded from
         # the queryset. If either bronorganisatie or identificatie changes,
         # and it already exists, it will raise a validation error
         combination_exists = (
-            serializer.Meta.model.objects
+            self.model.objects
             # in case of an update, exclude the current object. for a create, this
             # will be None
             .exclude(pk=pk)
             .filter(
                 **{
                     self.organisatie_field: organisatie,
                     self.identificatie_field: identificatie,
@@ -352,23 +364,30 @@
 class IsImmutableValidator:
     """
     Valideer dat de waarde van het veld niet wijzigt bij een update actie.
     """
 
     message = _("Dit veld mag niet gewijzigd worden.")
     code = "wijzigen-niet-toegelaten"
-    requires_context = True
 
-    def __call__(self, new_value, serializer_field):
-        instance = getattr(serializer_field.parent, "instance", None)
+    def set_context(self, serializer_field):
+        """
+        This hook is called by the serializer instance,
+        prior to the validation call being made.
+        """
+        # Determine the existing instance, if this is an update operation.
+        self.serializer_field = serializer_field
+        self.instance = getattr(serializer_field.parent, "instance", None)
+
+    def __call__(self, new_value):
         # no instance -> it's not an update
-        if not instance:
+        if not self.instance:
             return
 
-        current_value = getattr(instance, serializer_field.field_name)
+        current_value = getattr(self.instance, self.serializer_field.field_name)
 
         if new_value != current_value:
             raise serializers.ValidationError(self.message, code=self.code)
 
 
 class PublishValidator(ResourceValidator):
     """
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/views.py` & `commonground-api-common-1.9.0/vng_api_common/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import os
 from collections import OrderedDict
 
 from django.apps import apps
 from django.conf import settings
-from django.core.exceptions import ImproperlyConfigured
 from django.http import Http404, HttpRequest
 from django.utils.translation import gettext_lazy as _
 from django.views.generic import TemplateView
 
 import requests
 from rest_framework import exceptions as drf_exceptions, status
 from rest_framework.response import Response
@@ -16,15 +15,14 @@
 from zds_client import ClientError
 
 from . import exceptions
 from .compat import sentry_client
 from .constants import ComponentTypes
 from .exception_handling import HandledException
 from .scopes import SCOPE_REGISTRY
-from .utils import get_domain
 
 logger = logging.getLogger(__name__)
 
 ERROR_CONTENT_TYPE = "application/problem+json"
 
 
 def exception_handler(exc, context):
@@ -105,20 +103,23 @@
 
         context["config"] = config
 
         return context
 
 
 def _test_sites_config(request: HttpRequest) -> list:
-    try:
-        domain = get_domain()
-    except ImproperlyConfigured:
+    if not apps.is_installed("django.contrib.sites"):
         return []
+
+    from django.contrib.sites.models import Site
+
+    site = Site.objects.get_current()
+
     return [
-        (_("Site domain"), domain, request.get_host() == domain),
+        (_("Site domain"), site.domain, request.get_host() == site.domain),
         (_("HTTPS"), settings.IS_HTTPS, settings.IS_HTTPS == request.is_secure()),
     ]
 
 
 def _test_ac_config() -> list:
     if not apps.is_installed("vng_api_common.authorizations"):
         return []
```

### Comparing `commonground_api_common-1.13.1/vng_api_common/viewsets.py` & `commonground-api-common-1.9.0/vng_api_common/viewsets.py`

 * *Files identical despite different names*

