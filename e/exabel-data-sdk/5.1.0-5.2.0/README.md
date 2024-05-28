# Comparing `tmp/exabel-data-sdk-5.1.0.tar.gz` & `tmp/exabel_data_sdk-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exabel-data-sdk-5.1.0.tar", last modified: Tue Feb 27 12:00:24 2024, max compression
+gzip compressed data, was "exabel_data_sdk-5.2.0.tar", last modified: Tue May 28 12:55:19 2024, max compression
```

## Comparing `exabel-data-sdk-5.1.0.tar` & `exabel_data_sdk-5.2.0.tar`

### file list

```diff
@@ -1,365 +1,366 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.821076 exabel-data-sdk-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-02-27 12:00:24.821076 exabel-data-sdk-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.761076 exabel-data-sdk-5.1.0/exabel_data_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.761076 exabel-data-sdk-5.1.0/exabel_data_sdk/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.765076 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.769076 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/entity_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.769076 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/library_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/namespace_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/prediction_model_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/signal_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/tag_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/user_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/bulk_insert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.773076 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/derived_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/folder_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/paging_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/request_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_set_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/derived_signal_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/entity_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/export_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/library_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/namespace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/pageable_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/prediction_model_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16511 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/relationship_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/resource_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/search_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/signal_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29619 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/time_series_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/exabel_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13319 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/client/user_login.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.773076 exabel-data-sdk-5.1.0/exabel_data_sdk/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/examples/create_time_series_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/examples/get_company_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.777076 exabel-data-sdk-5.1.0/exabel_data_sdk/query/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/query/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/query/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/query/literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/query/predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/query/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/query/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/query/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.789076 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/base_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/command_line_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_derived_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_prediction_model_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/csv_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_time_series_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_time_series_points_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/export_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/export_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_entity_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_folder_accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_relationship_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/load_entities_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/load_relationships_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/load_time_series_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/load_time_series_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/load_time_series_metadata_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/move_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/search_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/share_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.789076 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/sql/read_athena.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/sql/read_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/sql/read_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/sql/sql_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/unshare_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/update_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/update_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/update_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/upsert_time_series_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.793076 exabel-data-sdk-5.1.0/exabel_data_sdk/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11610 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_loading_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_loading_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    23907 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_relationship_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/entity_mapping_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/feather_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/feather_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/file_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/file_loading_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/file_loading_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    39687 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/file_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    41749 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/file_time_series_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/file_writer_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.793076 exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/athena_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/snowflake_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/sql_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/sql_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/sqlalchemy_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.793076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.793076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.793076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.797076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.801076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.801076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.809076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    17980 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21976 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15088 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14364 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18059 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26840 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17111 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.809076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.813076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20539 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.813076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/math/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/math/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.813076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/time/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/time/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.813076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.817076 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    55413 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.817076 exabel-data-sdk-5.1.0/exabel_data_sdk/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/util/batcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/util/case_insensitive_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/util/deprecate_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/util/handle_missing_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/util/import_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/util/parse_property_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    17070 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/util/resource_name_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/util/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/exabel_data_sdk/util/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:00:24.817076 exabel-data-sdk-5.1.0/exabel_data_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-02-27 12:00:24.000000 exabel-data-sdk-5.1.0/exabel_data_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18076 2024-02-27 12:00:24.000000 exabel-data-sdk-5.1.0/exabel_data_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 12:00:24.000000 exabel-data-sdk-5.1.0/exabel_data_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-27 12:00:24.000000 exabel-data-sdk-5.1.0/exabel_data_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-27 12:00:24.000000 exabel-data-sdk-5.1.0/exabel_data_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 12:00:24.821076 exabel-data-sdk-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-02-27 11:59:09.000000 exabel-data-sdk-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.559394 exabel_data_sdk-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-28 12:55:19.559394 exabel_data_sdk-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.495395 exabel_data_sdk-5.2.0/exabel_data_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.495395 exabel_data_sdk-5.2.0/exabel_data_sdk/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.499395 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.503394 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/entity_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.503394 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/library_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/namespace_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/prediction_model_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/signal_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/tag_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/user_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/bulk_insert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.507395 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/derived_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/folder_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/paging_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_set_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/derived_signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/export_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/library_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/namespace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/pageable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/prediction_model_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16511 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/relationship_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/resource_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/search_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29619 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/time_series_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/exabel_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13319 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/client/user_login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.507395 exabel_data_sdk-5.2.0/exabel_data_sdk/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/examples/create_time_series_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/examples/get_company_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.511395 exabel_data_sdk-5.2.0/exabel_data_sdk/query/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/query/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/query/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/query/literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/query/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/query/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/query/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.519394 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/base_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/command_line_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_derived_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_prediction_model_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/csv_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_time_series_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_time_series_points_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/export_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_entity_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_folder_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_relationship_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/load_entities_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/load_relationships_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/load_time_series_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/load_time_series_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/load_time_series_metadata_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/move_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/search_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/share_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.523394 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/sql/read_athena.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/sql/read_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/sql/read_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/sql/sql_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/unshare_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/update_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/update_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/update_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/upsert_time_series_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.527395 exabel_data_sdk-5.2.0/exabel_data_sdk/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12213 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_loading_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_loading_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24602 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_relationship_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/entity_mapping_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/feather_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/feather_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/file_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/file_loading_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/file_loading_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41751 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/file_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44300 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/file_time_series_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/file_writer_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.527395 exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/athena_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/snowflake_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/sql_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/sql_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/sqlalchemy_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.527395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.527395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.527395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.531395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.535395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.535395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.547395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17980 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21976 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15088 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14364 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13807 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18059 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26840 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17111 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.547395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.551395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20539 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.551395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/math/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.551395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/time/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/time/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.551395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.555395 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55413 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.555395 exabel_data_sdk-5.2.0/exabel_data_sdk/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/util/batcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/util/case_insensitive_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/util/deprecate_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/util/handle_missing_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/util/import_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/util/logging_thread_pool_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/util/parse_property_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17070 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/util/resource_name_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/util/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/exabel_data_sdk/util/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:55:19.555395 exabel_data_sdk-5.2.0/exabel_data_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-28 12:55:19.000000 exabel_data_sdk-5.2.0/exabel_data_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18129 2024-05-28 12:55:19.000000 exabel_data_sdk-5.2.0/exabel_data_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:55:19.000000 exabel_data_sdk-5.2.0/exabel_data_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-28 12:55:19.000000 exabel_data_sdk-5.2.0/exabel_data_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 12:55:19.000000 exabel_data_sdk-5.2.0/exabel_data_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:55:19.559394 exabel_data_sdk-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-28 12:53:43.000000 exabel_data_sdk-5.2.0/setup.py
```

### Comparing `exabel-data-sdk-5.1.0/LICENSE` & `exabel_data_sdk-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/PKG-INFO` & `exabel_data_sdk-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exabel-data-sdk
-Version: 5.1.0
+Version: 5.2.0
 Summary: Python SDK for the Exabel Data API
 Home-page: https://github.com/Exabel/python-sdk
 Author: Exabel
 Author-email: support@exabel.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `exabel-data-sdk-5.1.0/README.md` & `exabel_data_sdk-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/entity_api_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/entity_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/library_api_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/library_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/signal_api_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/signal_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/tag_api_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/tag_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/api_client/user_api_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/api_client/user_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/bulk_import.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/bulk_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     DEFAULT_ABORT_THRESHOLD,
     DEFAULT_NUMBER_OF_RETRIES,
     DEFAULT_NUMBER_OF_THREADS_FOR_IMPORT,
     MAX_THREADS_FOR_IMPORT,
 )
 from exabel_data_sdk.util.deprecate_arguments import deprecate_arguments
 from exabel_data_sdk.util.import_ import get_batches_for_import
+from exabel_data_sdk.util.logging_thread_pool_executor import LoggingThreadPoolExecutor
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ResourceFailureHandler(Generic[ResourceT]):
     """Handles resource failures."""
@@ -43,23 +44,21 @@
                 violation.subject: violation for violation in precondition_failure.violations
             }
 
     @staticmethod
     @overload
     def get_time_series_result_from_violations(
         resource: TimeSeries, violations: Mapping[str, Violation]
-    ) -> ResourceCreationResult[TimeSeries]:
-        ...
+    ) -> ResourceCreationResult[TimeSeries]: ...
 
     @staticmethod
     @overload
     def get_time_series_result_from_violations(
         resource: pd.Series, violations: Mapping[str, Violation]
-    ) -> ResourceCreationResult[pd.Series]:
-        ...
+    ) -> ResourceCreationResult[pd.Series]: ...
 
     @staticmethod
     def get_time_series_result_from_violations(
         resource: Union[pd.Series, TimeSeries], violations: Mapping[str, Violation]
     ) -> Union[ResourceCreationResult[pd.Series], ResourceCreationResult[TimeSeries]]:
         """Get a time series creation result from precondition failure violations."""
         resource_name = TimeSeriesResourceName.from_string(resource.name)
@@ -258,25 +257,29 @@
                 results,
                 resource_batch,
                 import_func,
                 _raise_error,
             )
 
     else:
-        with ThreadPoolExecutor(max_workers=threads) as executor:
+        with (
+            LoggingThreadPoolExecutor(max_workers=threads)
+            if logger.getEffectiveLevel() == logging.DEBUG
+            else ThreadPoolExecutor(max_workers=threads)
+        ) as executor:
             for resource_batch in resource_batches:
                 if not results.abort:
                     # The generic type hints do not guarantee that TResource refers to the same
                     # class for each of the three parameters. This leads to mypy warnings for the
                     # following function call.
                     executor.submit(
                         _process,
-                        results,  # type: ignore[arg-type]
-                        resource_batch,  # type: ignore[arg-type]
-                        import_func,  # type: ignore[arg-type]
+                        results,
+                        resource_batch,
+                        import_func,
                         # Python 3.9 added support for the shutdown argument 'cancel_futures'.
                         # We should set this argument to True once we have moved to this python
                         # version.
                         lambda: executor.shutdown(wait=False),
                     )
         if results.abort:
             raise BulkInsertFailedError()
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/bulk_insert.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/bulk_insert.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,17 +89,17 @@
             for resource in resources:
                 if not results.abort:
                     # The generic type hints do not guarantee that TResource refers to the same
                     # class for each of the three parameters. This leads to mypy warnings for the
                     # following function call.
                     executor.submit(
                         _process,
-                        results,  # type: ignore[arg-type]
-                        resource,  # type: ignore[arg-type]
-                        insert_func,  # type: ignore[arg-type]
+                        results,
+                        resource,
+                        insert_func,
                         # Python 3.9 added support for the shutdown argument 'cancel_futures'.
                         # We should set this argument to True once we have moved to this python
                         # version.
                         lambda: executor.shutdown(wait=False),
                     )
         if results.abort:
             raise BulkInsertFailedError()
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/data_set.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/data_set.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/derived_signal.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/derived_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/entity.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/entity_type.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/folder.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/folder_item.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/folder_item.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/group.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/namespace.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/namespace.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/paging_result.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/paging_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,17 +78,19 @@
     @staticmethod
     def from_proto(model_run: ProtoPredictionModelRun) -> "PredictionModelRun":
         """Create a PredictionModelRun from the given protobuf PredictionModelRun."""
         return PredictionModelRun(
             name=model_run.name,
             description=model_run.description,
             configuration=ModelConfiguration(model_run.configuration),
-            configuration_source=model_run.configuration_source
-            if model_run.HasField("configuration_source")
-            else None,
+            configuration_source=(
+                model_run.configuration_source
+                if model_run.HasField("configuration_source")
+                else None
+            ),
             auto_activate=model_run.auto_activate,
         )
 
     def to_proto(self) -> ProtoPredictionModelRun:
         """Create a protobuf PredictionModelRun from this PredictionModelRun."""
         return ProtoPredictionModelRun(
             name=self.name,
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/relationship.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/relationship_type.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/request_error.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/request_error.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/signal.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/tag.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/tag.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/time_series.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/time_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,26 @@
     """Enum representing the dimension of a unit."""
 
     DIMENSION_UNKNOWN = ProtoUnit.Dimension.DIMENSION_UNKNOWN
     DIMENSION_CURRENCY = ProtoUnit.Dimension.DIMENSION_CURRENCY
     DIMENSION_MASS = ProtoUnit.Dimension.DIMENSION_MASS
     DIMENSION_LENGTH = ProtoUnit.Dimension.DIMENSION_LENGTH
     DIMENSION_TIME = ProtoUnit.Dimension.DIMENSION_TIME
+    DIMENSION_RATIO = ProtoUnit.Dimension.DIMENSION_RATIO
 
     @classmethod
     def from_string(cls, dimension: str) -> Dimension:
         """Get the Dimension enum from a string."""
         key = f"DIMENSION_{dimension.upper()}"
         try:
             return cls[key]
         except KeyError as e:
             raise ValueError(
                 f"Unknown dimension: {dimension}. "
-                + "Supported values are: unknown, currency, mass, length, time."
+                + "Supported values are: unknown, currency, mass, length, time, and ratio."
             ) from e
 
 
 DEFAULT_DIMENSION = Dimension.DIMENSION_UNKNOWN
 
 
 def _invalid_time_series_name(name: str) -> ValueError:
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_classes/user.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_classes/user.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/data_set_api.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/data_set_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/derived_signal_api.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/derived_signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/entity_api.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/entity_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/error_handler.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/error_handler.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/export_api.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/export_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/library_api.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/library_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/namespace_api.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/namespace_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/pageable_resource.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/pageable_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,13 +34,12 @@
         Return an iterator with all the resources returnable by function, paging through the
         results.
         """
         page_token: Optional[str] = None
         resource_count = 0
         while True:
             result = pageable_func(**kwargs, page_token=page_token)
-            for resource in result.results:
-                yield resource
+            yield from result.results
             page_token = result.next_page_token
             resource_count += len(result.results)
             if resource_count >= result.total_size:
                 break
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/prediction_model_api.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/prediction_model_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/proto_utils.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/proto_utils.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/relationship_api.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/relationship_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/resource_creation_result.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/resource_creation_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from exabel_data_sdk.client.api.data_classes.entity import Entity
 from exabel_data_sdk.client.api.data_classes.relationship import Relationship
 from exabel_data_sdk.client.api.data_classes.request_error import RequestError
 from exabel_data_sdk.client.api.data_classes.time_series import TimeSeries
 from exabel_data_sdk.services.csv_loading_constants import (
     DEFAULT_ABORT_THRESHOLD,
     DEFAULT_BULK_LOAD_CHECKPOINTS,
+    FAILURE_LOG_LIMIT,
 )
 
 logger = logging.getLogger(__name__)
 
 ResourceT = TypeVar("ResourceT", Entity, Relationship, pd.Series, TimeSeries)
 
 
@@ -86,15 +87,19 @@
         return str(self.resource)
 
     def get_printable_error(self) -> str:
         """
         Return a printable request error message if it is set, otherwise return the string
         representation of the error
         """
-        return self.error.message if self.error and self.error.message else str(self.error)
+        return (
+            f"{self.error.error_type.name}: {self.error.message}"
+            if self.error and self.error.message
+            else str(self.error)
+        )
 
 
 class ResourceCreationResults(Generic[ResourceT]):
     """
     Class for returning resource creation results.
     """
 
@@ -161,15 +166,17 @@
         """Whether this result contains failures."""
         return self.count(ResourceCreationStatus.FAILED) > 0
 
     def get_failures(self) -> Sequence[ResourceCreationResult[ResourceT]]:
         """Return all the failed results."""
         return list(filter(lambda r: r.status == ResourceCreationStatus.FAILED, self.results))
 
-    def extract_retryable_failures(self) -> Sequence[ResourceCreationResult[ResourceT]]:
+    def extract_retryable_failures(
+        self, log_summary: bool = True
+    ) -> Sequence[ResourceCreationResult[ResourceT]]:
         """
         Remove all retryable failures from this result set,
         and return them.
         """
         failed = []
         rest = []
         for result in self.results:
@@ -179,14 +186,22 @@
                 and result.error.error_type.retryable()
             ):
                 failed.append(result)
             else:
                 rest.append(result)
         self.counter.subtract([result.status for result in failed])
         self.results = rest
+
+        if log_summary and failed:
+            errors = [failure.error for failure in failed if failure.error]
+            error_types = Counter(error.error_type for error in errors)
+
+            logger.info("The following retryable failures were returned:")
+            for error_type, count in error_types.items():
+                logger.info("%d failures with error type: %s", count, error_type.name)
         return failed
 
     def check_failures(self) -> None:
         """
         Set the member field 'abort' to True if the fraction of errors exceeds the abort threshold.
         """
         fraction_error = self.count(ResourceCreationStatus.FAILED) / self.count()
@@ -194,31 +209,44 @@
             self.abort = True
             if self.do_print_status:
                 logger.error(
                     "Aborting - more than %.0f%% of the requests are failing.",
                     self.abort_threshold * 100,
                 )
 
-    def print_summary(self) -> None:
+    def print_summary(self, failure_log_limit: Optional[int] = FAILURE_LOG_LIMIT) -> None:
         """Prints a human legible summary of the resource creation results to screen."""
         if self.counter[ResourceCreationStatus.CREATED]:
             logger.info("%s new resources created", self.counter[ResourceCreationStatus.CREATED])
         if self.counter[ResourceCreationStatus.EXISTS]:
             logger.info("%s resources already existed", self.counter[ResourceCreationStatus.EXISTS])
         if self.counter[ResourceCreationStatus.UPSERTED]:
             logger.info("%s resources upserted", self.counter[ResourceCreationStatus.UPSERTED])
         if self.counter[ResourceCreationStatus.FAILED]:
             logger.warning("%s resources failed", self.counter[ResourceCreationStatus.FAILED])
-            for result in self.results:
-                if result.status == ResourceCreationStatus.FAILED:
+            failures = self.get_failures()
+            for i, failure in enumerate(failures):
+                if failure_log_limit and i > failure_log_limit:
                     logger.warning(
-                        "   %s\n      %s",
-                        result.get_printable_resource(),
-                        result.get_printable_error(),
+                        "%d resources failed. Only %d resources shown.",
+                        len(failures),
+                        failure_log_limit,
                     )
+                    break
+                logger.warning(
+                    "   %s\n      %s",
+                    failure.get_printable_resource(),
+                    failure.get_printable_error(),
+                )
+
+            errors = [failure.error for failure in failures if failure.error]
+            error_types = Counter(error.error_type for error in errors)
+            logger.warning("Summary of the errors for the failed resources:")
+            for error_type, count in error_types.items():
+                logger.warning("   %s: %d", error_type.name, count)
 
     def print_status(self) -> None:
         """
         Prints a status update on the progress of the data loading, showing the percentage complete
         and how many objects were created, already existed or failed.
         """
         message_parts = []
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/search_service.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/search_service.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/signal_api.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/tag_api.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/tag_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/time_series_api.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/time_series_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/api/user_api.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/client_config.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/client_config.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/exabel_client.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/exabel_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/client/user_login.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/client/user_login.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/examples/create_time_series_example.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/examples/create_time_series_example.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/examples/get_company_example.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/examples/get_company_example.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/query/column.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/query/column.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/query/dashboard.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/query/dashboard.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/query/literal.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/query/literal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/query/predicate.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/query/predicate.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/query/query.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/query/query.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/query/signals.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/query/signals.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/actions.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/actions.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/base_script.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/base_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,17 +68,17 @@
             for warning in entity_resource_names.warnings
         ]
         all_rows.extend(
             {identifier_type: identifier, "entity": entity, "warning": None}
             for identifier, entity in entity_resource_names.mapping.items()
         )
         df = pd.DataFrame(all_rows)
-        df.loc[
-            (df["entity"].duplicated(keep=False) & ~df["entity"].isna()), "warning"
-        ] = "Multiple identifiers mapping to the same company"
+        df.loc[(df["entity"].duplicated(keep=False) & ~df["entity"].isna()), "warning"] = (
+            "Multiple identifiers mapping to the same company"
+        )
         if not keep_all_identifiers:
             df = df[df["warning"].notnull()]
         df = df.fillna("").sort_values(["entity", identifier_type])
         return df
 
     def run_script(self, client: ExabelClient, args: argparse.Namespace) -> None:
         data_frame = self.read_csv(args, string_columns=[args.identifier_column])
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/command_line_script.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/command_line_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_derived_signal.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_derived_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_entity.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_entity_type.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_folder.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_prediction_model_run.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_prediction_model_run.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_relationship.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_relationship_type.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/create_signal.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/create_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/csv_script.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/csv_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_entities.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_entities.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_entity.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_entity_type.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_folder.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_relationship.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_relationship_type.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_signal.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_time_series.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_time_series_point.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_time_series_point.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/delete_time_series_points_from_file.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/delete_time_series_points_from_file.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/export_data.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/export_data.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/export_signals.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/export_signals.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/file_utils.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/file_utils.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_entity.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_entity_type.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_folder.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_relationship.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_relationship_type.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_signal.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/get_time_series.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/get_time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_entities.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_entities.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_entity_types.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_entity_types.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_folder_accessors.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_folder_accessors.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_folders.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_folders.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_items.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_items.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_relationship_types.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_relationship_types.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_relationships.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_relationships.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_signals.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_signals.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/list_time_series.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/list_time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/load_entities_from_csv.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/load_entities_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/load_relationships_from_csv.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/load_relationships_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/load_time_series_from_file.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/load_time_series_from_file.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/load_time_series_metadata_from_file.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/load_time_series_metadata_from_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,24 +87,14 @@
             action="store_true",
             default=False,
             help="If set, signal names are treated as case sensitive. Note that this will disable "
             "lowercasing of other column headers as well, as entities, 'date', and "
             "'known_time'. Take care to maintain correct casing in the file when using this "
             "option.",
         )
-        self.parser.add_argument(
-            "--unit-type",
-            required=False,
-            type=str,
-            default=None,
-            help=(
-                "The unit type of the time series. "
-                "One of 'currency', 'time', 'mass', 'length' or 'unknown'."
-            ),
-        )
 
     def run_script(self, client: ExabelClient, args: argparse.Namespace) -> None:
         try:
             FileTimeSeriesLoader(client).load_time_series_metadata(
                 filename=args.filename,
                 entity_mapping_filename=args.entity_mapping_filename,
                 separator=args.sep,
@@ -115,15 +105,14 @@
                 threads=args.threads,
                 dry_run=args.dry_run,
                 retries=args.retries,
                 abort_threshold=args.abort_threshold,
                 batch_size=args.batch_size,
                 skip_validation=args.skip_validation,
                 case_sensitive_signals=args.case_sensitive_signals,
-                unit_type=args.unit_type,
             )
 
         except FileLoadingException as e:
             print(e)
             sys.exit(1)
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/login.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/login.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/move_items.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/move_items.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/search_entities.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/search_entities.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/share_folder.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/share_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/sql/read_athena.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/sql/read_athena.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/sql/read_bigquery.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/sql/read_bigquery.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/sql/read_snowflake.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/sql/read_snowflake.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/sql/sql_script.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/sql/sql_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/unshare_folder.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/unshare_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/update_entity_type.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/update_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/update_folder.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/update_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/update_relationship_type.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/update_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/upsert_time_series_unit.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/upsert_time_series_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.parser.add_argument(
             "--unit-type",
             required=False,
             type=str,
             default=None,
             help=(
                 "The unit type of the time series. "
-                "One of 'unknown', 'currency', 'mass', 'length', 'time'."
+                "One of 'unknown', 'currency', 'mass', 'length', 'time', 'ratio'."
             ),
         )
         self.parser.add_argument(
             "--unit",
             required=False,
             type=str,
             default=None,
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/scripts/utils.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_entity_loader.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_entity_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         upsert: bool = False,
         dry_run: bool = False,
         error_on_any_failure: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = DEFAULT_ABORT_THRESHOLD,
         batch_size: Optional[int] = None,
         return_results: bool = True,
+        total_rows: Optional[int] = None,
         # Deprecated arguments
         name_column: Optional[str] = None,  # pylint: disable=unused-argument
         namespace: Optional[str] = None,  # pylint: disable=unused-argument
     ) -> FileLoadingResult:
         """
         Load a CSV file and upload the entities specified therein to the Exabel Data API.
 
@@ -78,14 +79,17 @@
             dry_run: if True, the file is processed, but no entities are actually uploaded
             error_on_any_failure: if True, an exception is raised if any entity failed to be created
             retries: the maximum number of retries to make for each failed request
             abort_threshold: the threshold for the proportion of failed requests that will cause the
                  upload to be aborted; if it is `None`, the upload is never aborted
             batch_size: the number of entities to upload in each batch; if not specified, the
                 entire file will be read into memory and uploaded in a single batch
+            return_results: if True, returns a FileLoadingResult with info, else returns an
+                empty FileLoadingResult
+            total_rows: the total number of rows to be processed
         """
         if dry_run:
             logger.info("Running dry-run...")
 
         logger.info("Loading entities from %s", filename)
         preview_df = CsvReader.read_file(
             filename, separator, string_columns=[], keep_default_na=False, nrows=0
@@ -151,14 +155,21 @@
                 dry_run=dry_run,
                 error_on_any_failure=error_on_any_failure,
                 retries=retries,
                 abort_threshold=abort_threshold,
             )
             if return_results:
                 combined_result.update(result)
+            if combined_result.processed_rows is not None and total_rows:
+                logger.info(
+                    "Rows processed: %d / %d. %.1f %%",
+                    combined_result.processed_rows,
+                    total_rows,
+                    100 * combined_result.processed_rows / total_rows,
+                )
 
         return combined_result
 
     def _load_entities(
         self,
         *,
         data_frame: DataFrame,
@@ -225,15 +236,15 @@
                 abort_threshold=abort_threshold,
             )
             if error_on_any_failure and result.has_failure():
                 raise FileLoadingException(
                     "An error occurred while uploading entities.",
                     failures=result.get_failures(),
                 )
-            return FileLoadingResult(result)
+            return FileLoadingResult(result, processed_rows=len(data_frame))
         except BulkInsertFailedError as e:
             # An error summary has already been printed.
             if error_on_any_failure:
                 raise FileLoadingException("An error occurred while uploading entities.") from e
             return FileLoadingResult(aborted=True)
 
     @staticmethod
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_reader.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_reader.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,51 +11,47 @@
     def read_file(
         filename: str,
         separator: Optional[str],
         string_columns: Iterable[Union[str, int]],
         *,
         keep_default_na: bool,
         nrows: Optional[int],
-    ) -> pd.DataFrame:
-        ...
+    ) -> pd.DataFrame: ...
 
     @overload
     @staticmethod
     def read_file(
         filename: str,
         separator: Optional[str],
         string_columns: Iterable[Union[str, int]],
         *,
         keep_default_na: bool,
-    ) -> pd.DataFrame:
-        ...
+    ) -> pd.DataFrame: ...
 
     @overload
     @staticmethod
     def read_file(
         filename: str,
         separator: Optional[str],
         string_columns: Iterable[Union[str, int]],
         *,
         keep_default_na: bool,
         chunksize: int,
-    ) -> Iterator[pd.DataFrame]:
-        ...
+    ) -> Iterator[pd.DataFrame]: ...
 
     @overload
     @staticmethod
     def read_file(
         filename: str,
         separator: Optional[str],
         string_columns: Iterable[Union[str, int]],
         *,
         keep_default_na: bool,
         chunksize: Optional[int],
-    ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-        ...
+    ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
 
     @staticmethod
     def read_file(
         filename: str,
         separator: Optional[str],
         string_columns: Iterable[Union[str, int]],
         *,
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_relationship_loader.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_relationship_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,15 @@
         upsert: bool = False,
         dry_run: bool = False,
         error_on_any_failure: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = DEFAULT_ABORT_THRESHOLD,
         batch_size: Optional[int] = None,
         return_results: bool = True,
+        total_rows: Optional[int] = None,
         # Deprecated arguments:
         entity_from_column: Optional[str] = None,  # pylint: disable=unused-argument
         entity_to_column: Optional[str] = None,  # pylint: disable=unused-argument
         namespace: Optional[str] = None,  # pylint: disable=unused-argument
     ) -> FileLoadingResult:
         """
         Load a CSV file and upload the relationships specified therein to the Exabel Data API.
@@ -341,14 +342,17 @@
             error_on_any_failure: if True, an exception is raised if any relationship failed to be
                 created
             retries: the maximum number of retries to make for each failed request
             abort_threshold: the threshold for the proportion of failed requests that will cause the
                  upload to be aborted; if it is `None`, the upload is never aborted
             batch_size: the number of relationships to upload in each batch; if not specified, the
                 relationship file will be read into memory and uploaded in a single batch
+            return_results: if True, returns a FileLoadingResult with info, else returns an
+                empty FileLoadingResult
+            total_rows: the total number of rows to be processed
         """
         if dry_run:
             logger.info("Running dry-run...")
         try:
             config = RelationshipLoaderColumnConfiguration.from_arguments(
                 from_entity_type=from_entity_type,
                 from_identifier_type=from_identifier_type,
@@ -410,14 +414,21 @@
                 dry_run=dry_run,
                 error_on_any_failure=error_on_any_failure,
                 retries=retries,
                 abort_threshold=abort_threshold,
             )
             if return_results:
                 combined_result.update(result)
+            if combined_result.processed_rows is not None and total_rows:
+                logger.info(
+                    "Rows processed: %d / %d. %.1f %%",
+                    combined_result.processed_rows,
+                    total_rows,
+                    100 * combined_result.processed_rows / total_rows,
+                )
         return combined_result
 
     def _load_relationships(
         self,
         data_frame: DataFrame,
         entity_mapping: Optional[Mapping[str, Mapping[str, str]]],
         relationship_type_name: str,
@@ -492,30 +503,34 @@
             ]
         except TypeConversionError as e:
             raise FileLoadingException("An error occurred while converting property types.") from e
 
         if dry_run:
             logger.info("Loading %d relationships", len(relationships))
             logger.info(relationships)
-            return FileLoadingResult(warnings=list(map(str, warnings)))
+            return FileLoadingResult(
+                warnings=list(map(str, warnings)), processed_rows=len(data_frame)
+            )
 
         try:
             result = self._client.relationship_api.bulk_create_relationships(
                 relationships,
                 threads=threads,
                 upsert=upsert,
                 retries=retries,
                 abort_threshold=abort_threshold,
             )
             if error_on_any_failure and result.has_failure():
                 raise FileLoadingException(
                     "An error occurred while uploading relationships.",
                     failures=result.get_failures(),
                 )
-            return FileLoadingResult(result, warnings=list(map(str, warnings)))
+            return FileLoadingResult(
+                result, warnings=list(map(str, warnings)), processed_rows=len(data_frame)
+            )
         except BulkInsertFailedError as e:
             # An error summary has already been printed.
             if error_on_any_failure:
                 raise FileLoadingException(
                     "An error occurred while uploading relationships."
                 ) from e
             return FileLoadingResult(warnings=list(map(str, warnings)), aborted=True)
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_time_series_loader.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_time_series_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/csv_writer.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/csv_writer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import logging
 import os
 from typing import Iterable, Union
 
 import pandas as pd
 
-from exabel_data_sdk.services.file_writer import FileWriter
+from exabel_data_sdk.services.file_writer import FileWriter, FileWritingResult
 
 logger = logging.getLogger(__name__)
 
 
 class CsvWriter(FileWriter):
     """Stores a DataFrame in a CSV file."""
 
     @staticmethod
-    def write_file(df: Union[pd.DataFrame, Iterable[pd.DataFrame]], filepath: str) -> None:
+    def write_file(
+        df: Union[pd.DataFrame, Iterable[pd.DataFrame]], filepath: str
+    ) -> FileWritingResult:
+        rows = 0
         if isinstance(df, pd.DataFrame):
             df.to_csv(filepath, index=False)
+            rows = len(df)
         else:
             mode = "w"
             for chunk in df:
                 header = mode == "w"
                 chunk.to_csv(filepath, header=header, index=False, mode=mode)
                 mode = "a"
+                rows += len(chunk)
 
         if os.path.isfile(filepath):
             logger.info("Wrote CSV file to: %s", filepath)
+
+        return FileWritingResult(rows)
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/entity_mapping_file_reader.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/entity_mapping_file_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/feather_reader.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/feather_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/feather_writer.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/feather_writer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import logging
 from pathlib import Path
 from typing import Iterable, Union
 
 import pandas as pd
 
-from exabel_data_sdk.services.file_writer import FileWriter
+from exabel_data_sdk.services.file_writer import FileWriter, FileWritingResult
 
 logger = logging.getLogger(__name__)
 
 
 class FeatherWriter(FileWriter):
     """Stores a DataFrame in a Feather file."""
 
     @staticmethod
-    def write_file(df: Union[pd.DataFrame, Iterable[pd.DataFrame]], filepath: str) -> None:
+    def write_file(
+        df: Union[pd.DataFrame, Iterable[pd.DataFrame]], filepath: str
+    ) -> FileWritingResult:
+        rows = 0
         if isinstance(df, pd.DataFrame):
             df.to_feather(filepath)
-            return
+            rows = len(df)
+        else:
+            filepath_stem = Path(filepath).stem
+            for batch_no, chunk in enumerate(df, 1):
+                feather_file = f"{filepath_stem}_{batch_no}.feather"
+                chunk.to_feather(feather_file)
+                rows += len(chunk)
 
-        filepath_stem = Path(filepath).stem
-        for batch_no, chunk in enumerate(df, 1):
-            feather_file = f"{filepath_stem}_{batch_no}.feather"
-            chunk.to_feather(feather_file)
+        return FileWritingResult(rows)
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/file_loading_exception.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/file_loading_exception.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/file_loading_result.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/file_loading_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,48 +34,54 @@
     Contains a summary of the results of uploading data from a data file.
 
     Attributes:
         results: the individual uploading results for all the resources; `None` if uploading was
             aborted or it was a dry run
         warnings: a list of warnings
         aborted: whether uploading was aborted
+        processed_rows: the number of rows processed
     """
 
     def __init__(
         self,
         results: Optional[ResourceCreationResults[ResourceT]] = None,
         *,
         warnings: Optional[Sequence[str]] = None,
         aborted: bool = False,
+        processed_rows: Optional[int] = None,
     ):
         self.results: Optional[ResourceCreationResults[ResourceT]] = results
         self.warnings = warnings or []
         self.aborted = aborted
+        self.processed_rows = processed_rows
 
     def update(self, other: FileLoadingResult[ResourceT]) -> None:
         """
         Update this result with the results from another result.
         """
         if self.results is None:
             self.results = other.results
         elif self.results is not None and other.results is not None:
             self.results.update(other.results)
         self.warnings = (*self.warnings, *other.warnings)
         self.aborted = self.aborted or other.aborted
+        if other.processed_rows is not None:
+            self.processed_rows = (self.processed_rows or 0) + other.processed_rows
 
 
 class TimeSeriesFileLoadingResult(FileLoadingResult[pd.Series]):
     """
     Contains a summary of the results of uploading data from a data file.
 
     Attributes:
         results:                the individual uploading results for all the resources; `None` if
                                 uploading was aborted or it was a dry run
         warnings:               a list of warnings
         aborted:                whether uploading was aborted
+        rows:                   the number of rows processed
         entity_mapping_result:  results of mapping entities in the input file
         created_data_signals:   resource names of data API signals which did not exist from before
         dry_run_results:        resource names of resources which would be created in case of a dry
                                 run
         sheet_name:             the name of the sheet, when applicable
         has_known_time:         whether the file contained a column specifying the known time
         replaced:               the names of time series requested to be replaced; `None` if
@@ -84,22 +90,23 @@
 
     def __init__(
         self,
         results: Optional[ResourceCreationResults[pd.Series]] = None,
         *,
         warnings: Optional[Sequence[str]] = None,
         aborted: bool = False,
+        processed_rows: Optional[int] = None,
         entity_mapping_result: Optional[EntityMappingResult] = None,
         created_data_signals: Optional[Sequence[str]] = None,
         dry_run_results: Optional[Sequence[str]] = None,
         sheet_name: Optional[str] = None,
         has_known_time: bool = False,
         replaced: Optional[Sequence[str]] = None,
     ):
-        super().__init__(results, warnings=warnings, aborted=aborted)
+        super().__init__(results, warnings=warnings, aborted=aborted, processed_rows=processed_rows)
         if entity_mapping_result is None:
             raise ValueError("Entity mapping result must be set.")
         self.entity_mapping_result = entity_mapping_result
         if created_data_signals is None:
             raise ValueError("List of created data API signals must be set.")
         self.created_data_signals = created_data_signals
         self.dry_run_results = dry_run_results
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/file_time_series_loader.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/file_time_series_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from typing import List, Mapping, MutableSequence, Optional, Sequence, Tuple, Type
 
 from google.protobuf.duration_pb2 import Duration
+from google.protobuf.field_mask_pb2 import FieldMask
 
 from exabel_data_sdk import ExabelClient
 from exabel_data_sdk.client.api.bulk_insert import BulkInsertFailedError
 from exabel_data_sdk.client.api.data_classes.signal import Signal
 from exabel_data_sdk.client.api.resource_creation_result import ResourceCreationResults
 from exabel_data_sdk.client.api.search_service import (
     COMPANY_SEARCH_TERM_FIELDS,
@@ -74,14 +75,16 @@
         abort_threshold: Optional[float] = DEFAULT_ABORT_THRESHOLD,
         batch_size: Optional[int] = None,
         skip_validation: bool = False,
         case_sensitive_signals: bool = False,
         replace_existing_time_series: bool = False,
         replace_existing_data_points: bool = False,
         return_results: bool = True,
+        processed_rows: int = 0,
+        total_rows: Optional[int] = None,
         # Deprecated arguments
         create_tag: Optional[bool] = None,  # pylint: disable=unused-argument
         namespace: Optional[str] = None,  # pylint: disable=unused-argument
     ) -> Sequence[TimeSeriesFileLoadingResult]:
         """
         Load a file and upload the time series to the Exabel Data API
 
@@ -117,14 +120,16 @@
                 entire file will be read into memory and uploaded in a single batch
             skip_validation: if True, the time series are not validated before uploading
             case_sensitive_signals: if True, signals are case sensitive
             replace_existing_time_series: if True, any existing time series are replaced
             replace_existing_data_points: if True, any existing time series data points are replaced
             return_results: if True, returns a list of TimeSeriesFileLoadingResults
                 or otherwise an empty list.
+            processed_rows: the number of rows already processed
+            total_rows: the total number of rows to be processed
         """
         if replace_existing_time_series and replace_existing_data_points:
             raise ValueError(
                 "Only one of replace_existing_time_series or replace_existing_data_points can be "
                 "true"
             )
         if batch_size is not None:
@@ -161,14 +166,22 @@
                 abort_threshold=abort_threshold,
                 skip_validation=skip_validation,
                 case_sensitive_signals=case_sensitive_signals,
                 replace_existing_time_series=replace_existing_time_series,
                 replace_existing_data_points=replace_existing_data_points,
                 replaced_time_series=replaced_time_series,
             )
+            if result.processed_rows is not None and total_rows:
+                processed_rows = processed_rows + result.processed_rows
+                logger.info(
+                    "Rows processed: %d / %d. %.1f %%",
+                    processed_rows,
+                    total_rows,
+                    100 * processed_rows / total_rows,
+                )
             if replace_existing_time_series and result.replaced:
                 replaced_time_series.extend(result.replaced)
             if return_results:
                 results.append(result)
         return results
 
     def _load_time_series(
@@ -294,15 +307,17 @@
         entity_mapping_result = EntityMappingResult(
             parsed_file.get_entity_lookup_result().mapping,
             parsed_file.get_entity_lookup_result().identifier_type,
             parsed_file.get_entity_names(),
             [w.query for w in parsed_file.get_entity_lookup_result().warnings],
         )
         series, invalid_series = parsed_file.get_series(
-            prefix=self._get_signal_prefix(), skip_validation=skip_validation
+            prefix=self._get_signal_prefix(),
+            skip_validation=skip_validation,
+            replace_existing_time_series=replace_existing_time_series,
         )
 
         if dry_run:
             logger.info("Running the script would create the following time series:")
             for ts in series:
                 logger.info("    %s", ts.name)
             if error_on_any_failure and invalid_series:
@@ -312,14 +327,15 @@
             return TimeSeriesFileLoadingResult(
                 warnings=file_warnings,
                 entity_mapping_result=entity_mapping_result,
                 created_data_signals=missing_signals,
                 dry_run_results=[str(ts.name) for ts in series],
                 sheet_name=parser.sheet_name(),
                 has_known_time=parsed_file.has_known_time(),
+                processed_rows=len(parsed_file.data),
             )
         try:
             replaced_in_this_batch = []
             if replace_existing_time_series:
                 if replaced_time_series is None:
                     replaced_time_series = []
                 series_to_replace = []
@@ -382,14 +398,15 @@
                 result,
                 warnings=file_warnings,
                 entity_mapping_result=entity_mapping_result,
                 created_data_signals=missing_signals,
                 sheet_name=parser.sheet_name(),
                 has_known_time=parsed_file.has_known_time(),
                 replaced=replaced_in_this_batch,
+                processed_rows=len(parsed_file.data),
             )
         except BulkInsertFailedError as e:
             # An error summary has already been printed.
             if error_on_any_failure:
                 raise FileLoadingException("An error occurred while uploading time series.") from e
             return TimeSeriesFileLoadingResult(
                 warnings=file_warnings,
@@ -413,14 +430,16 @@
         dry_run: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = DEFAULT_ABORT_THRESHOLD,
         batch_size: Optional[int] = None,
         skip_validation: bool = False,
         case_sensitive_signals: bool = False,
         return_results: bool = True,
+        processed_rows: int = 0,
+        total_rows: Optional[int] = None,
     ) -> Sequence[FileLoadingResult]:
         """
         Load a CSV file to delete the time series data points represented in it.
 
         Args:
             filename: the location of the CSV file
             entity_mapping_filename: the location of the entity mapping file to use; only *.json and
@@ -434,16 +453,18 @@
             dry_run: if True, the file is processed, but no time series data points are actually
                      deleted
             retries: the maximum number of retries to make for each failed request
             abort_threshold: the threshold for the proportion of failed requests that will cause the
                  process to be aborted; if it is `None`, the upload is never aborted
             skip_validation: if True, the time series are not validated before deletion
             case_sensitive_signals: if True, signals are case sensitive
-            return_results: if True, returns a list of TimeSeriesFileLoadingResults
+            return_results: if True, returns a list of FileLoadingResults
                 or otherwise an empty list.
+            processed_rows: the number of rows already processed
+            total_rows: the total number of rows to be processed
         """
         if dry_run:
             logger.info("Running dry-run...")
 
         logger.info("Deleting time series data points from %s", filename)
         entity_mapping = EntityMappingFileReader.read_entity_mapping_file(
             entity_mapping_filename, separator=separator
@@ -523,15 +544,29 @@
                     failures=[*invalid_series],
                 )
 
             result = self._client.time_series_api.batch_delete_time_series_points(
                 series, threads, retries, abort_threshold
             )
             if return_results:
-                results.append(FileLoadingResult(result, warnings=list(map(str, file_warnings))))
+                results.append(
+                    FileLoadingResult(
+                        result,
+                        warnings=list(map(str, file_warnings)),
+                        processed_rows=len(parsed_file.data),
+                    )
+                )
+            if len(parsed_file.data) is not None and total_rows:
+                processed_rows += len(parsed_file.data)
+                logger.info(
+                    "Rows processed: %d / %d. %.1f %%",
+                    processed_rows,
+                    total_rows,
+                    100 * processed_rows / total_rows,
+                )
         return results
 
     def load_time_series_metadata(
         self,
         *,
         filename: str,
         entity_mapping_filename: Optional[str] = None,
@@ -546,16 +581,17 @@
         error_on_any_failure: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = DEFAULT_ABORT_THRESHOLD,
         batch_size: Optional[int] = None,
         skip_validation: bool = False,
         case_sensitive_signals: bool = False,
         return_results: bool = True,
-        unit_type: Optional[str] = None,
-    ) -> Sequence[FileLoadingResult]:
+        processed_rows: int = 0,
+        total_rows: Optional[int] = None,
+    ) -> Sequence[TimeSeriesFileLoadingResult]:
         """
         Load a file and upload the time series metadata to the Exabel Data API
 
         If the file has multiple sheets, time series from all the sheets are loaded.
 
         Args:
             filename: the location of the file, either a CSV or Excel file
@@ -578,17 +614,18 @@
             retries: the maximum number of retries to make for each failed request
             abort_threshold: the threshold for the proportion of failed requests that will cause the
                  upload to be aborted; if it is `None`, the upload is never aborted
             batch_size: the number of rows to read and upload in each batch; if not specified, the
                 entire file will be read into memory and uploaded in a single batch
             skip_validation: if True, the time series are not validated before uploading
             case_sensitive_signals: if True, signals are case sensitive
-            return_results: if True, returns a list of TimeSeriesFileLoadingResults
+            return_results: if True, returns a list of FileLoadingResults
                 or otherwise an empty list.
-            unit_type: the unit type of the time series. E.g. "currency", "time", "mass", etc.
+            processed_rows: the number of rows already processed
+            total_rows: the total number of rows to be processed
         """
         if dry_run:
             logger.info("Running dry-run...")
 
         logger.info("Uploading time series metadata from %s", filename)
         if identifier_type and not entity_type:
             raise FileLoadingException(
@@ -639,18 +676,17 @@
             entity_mapping_result = EntityMappingResult(
                 parsed_file.get_entity_lookup_result().mapping,
                 parsed_file.get_entity_lookup_result().identifier_type,
                 parsed_file.get_entity_names(),
                 [w.query for w in parsed_file.get_entity_lookup_result().warnings],
             )
 
-            series, invalid_series = parsed_file.get_series(  # type: ignore[call-arg]
+            series, invalid_series = parsed_file.get_series(
                 prefix=self._get_signal_prefix(),
                 skip_validation=skip_validation,
-                unit_type=unit_type,
             )
             if dry_run:
                 logger.info("Running the script would upsert the following time series:")
                 for ts in series:
                     logger.info(ts.name)
                     logger.info(ts.units)
                 if error_on_any_failure and invalid_series:
@@ -684,14 +720,15 @@
                         results.append(
                             TimeSeriesFileLoadingResult(
                                 result,
                                 warnings=file_warnings,
                                 entity_mapping_result=entity_mapping_result,
                                 created_data_signals=missing_signals,
                                 sheet_name=parser.sheet_name(),
+                                processed_rows=len(parsed_file.data),
                             )
                         )
                 except BulkInsertFailedError as e:
                     # An error summary has already been printed.
                     if error_on_any_failure:
                         raise FileLoadingException(
                             "An error occurred while uploading time series."
@@ -702,14 +739,22 @@
                             aborted=True,
                             entity_mapping_result=entity_mapping_result,
                             created_data_signals=missing_signals,
                             sheet_name=parser.sheet_name(),
                             has_known_time=parsed_file.has_known_time(),
                         )
                     )
+            if len(parsed_file.data) is not None and total_rows:
+                processed_rows += len(parsed_file.data)
+                logger.info(
+                    "Rows processed: %d / %d. %.1f %%",
+                    processed_rows,
+                    total_rows,
+                    100 * processed_rows / total_rows,
+                )
 
         return results
 
     def _get_signal_prefix(self) -> str:
         """Get signal prefix."""
         if self._client.namespace:
             return SIGNAL_PREFIX + self._client.namespace + "."
@@ -772,16 +817,18 @@
 
         if missing_signals:
             logger.info("The following signals are missing:\n%s", missing_signals)
             if create_missing_signals:
                 logger.info("Creating the missing signals.")
                 if not dry_run:
                     for signal in missing_signals:
-                        self._client.signal_api.create_signal(
+                        self._client.signal_api.update_signal(
                             Signal(name=signal, display_name=signal),
+                            update_mask=FieldMask(paths=["name"]),
+                            allow_missing=True,
                             create_library_signal=create_library_signal,
                         )
             else:
                 raise FileLoadingException(
                     "Aborting script. Please create the missing signals, and try again."
                 )
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/file_time_series_parser.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/file_time_series_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 import collections
 import logging
 import re
-from collections import Counter, defaultdict
+from collections import defaultdict
 from dataclasses import dataclass
 from pathlib import Path
 from typing import (
     Any,
     Iterable,
     Iterator,
     Mapping,
@@ -108,15 +108,15 @@
                 )
 
             return iter([TimeSeriesFileParser(filename, None, None, None)])
         if batch_size is not None:
             logger.info("Reading input data in batches of %d rows. ", batch_size)
             return (
                 TimeSeriesFileParser(filename, separator, None, df)
-                for df in CsvReader.read_file(  # pylint: disable=not-an-iterable
+                for df in CsvReader.read_file(  # pylint: disable=all
                     filename,
                     separator,
                     (0,),
                     keep_default_na=True,
                     chunksize=batch_size,
                 )
             )
@@ -297,20 +297,30 @@
         """Get the signals."""
 
     @abc.abstractmethod
     def get_entity_names(self) -> Sequence[str]:
         """Get the entity resource names."""
 
     @abc.abstractmethod
-    def _get_series_with_potential_duplicate_data_points(self, prefix: str) -> Sequence[pd.Series]:
+    def _get_series_with_potential_duplicate_data_points(
+        self, prefix: str, replace_existing_time_series: bool
+    ) -> Sequence[pd.Series]:
         """Get the time series, with potential duplicate data points."""
 
-    def get_series(self, prefix: str, *, skip_validation: bool = False) -> ValidatedTimeSeries:
+    def get_series(
+        self,
+        prefix: str,
+        *,
+        replace_existing_time_series: bool = False,
+        skip_validation: bool = False,
+    ) -> ValidatedTimeSeries:
         """Get the time series."""
-        series = self._get_series_with_potential_duplicate_data_points(prefix)
+        series = self._get_series_with_potential_duplicate_data_points(
+            prefix, replace_existing_time_series
+        )
         failures = []
         if not skip_validation:
             series_without_duplicate_data_points = [
                 self._drop_duplicate_data_points(s) for s in series
             ]
             series_with_duplicate_indexes = list(
                 self._get_time_series_with_duplicates_in_index(series_without_duplicate_data_points)
@@ -528,22 +538,24 @@
         return list(set(self._data["entity"]))
 
     def validate_numeric(self) -> None:
         values = self._data["value"]
         if not is_numeric_dtype(values) and any(~values.apply(_is_float)):
             raise FileLoadingException("Found at least one non-numeric value in the value column.")
 
-    def _get_series_with_potential_duplicate_data_points(self, prefix: str) -> Sequence[pd.Series]:
+    def _get_series_with_potential_duplicate_data_points(
+        self, prefix: str, replace_existing_time_series: bool = False
+    ) -> Sequence[pd.Series]:
         series = []
 
         for (entity, signal), group in self._data.groupby(["entity", "signal"]):
             # Do not drop nan values, as this format is the only way to actually delete values
             # by explicitly importing empty values.
             ts = group["value"]
-            if ts.empty:
+            if ts.empty and not replace_existing_time_series:
                 continue
 
             ts.name = f"{entity}/{prefix}{signal}"
             series.append(ts)
         return series
 
     @classmethod
@@ -568,15 +580,16 @@
             entity_api,
             namespace,
             entity_mapping,
             preserve_namespace=entity_type is not None,
             entity_type=entity_type,
         )
         data[entity_column] = lookup_result.names
-        data.rename(columns={entity_column: "entity"}, inplace=True)
+        data = data.loc[~data[entity_column].isnull()]
+        data = data.rename(columns={entity_column: "entity"})
         return data, lookup_result
 
 
 class SignalNamesInColumns(DateParsingMixin, ParsedTimeSeriesFile):
     """
     Container for files which have one column for each signal.
 
@@ -630,22 +643,24 @@
             values = self._data[signal]
             if not is_numeric_dtype(values) and any(~values.apply(_is_float)):
                 non_numeric_signals[signal] = self._data.loc[~values.apply(_is_float)][
                     "entity"
                 ].values
         _check_non_numeric_error(non_numeric_signals)
 
-    def _get_series_with_potential_duplicate_data_points(self, prefix: str) -> Sequence[pd.Series]:
+    def _get_series_with_potential_duplicate_data_points(
+        self, prefix: str, replace_existing_time_series: bool = False
+    ) -> Sequence[pd.Series]:
         series = []
 
         for entity, entity_group in self._data.groupby("entity"):
             for signal in self.get_signals():
                 ts = entity_group[signal]
                 ts.dropna(inplace=True)
-                if ts.empty:
+                if ts.empty and not replace_existing_time_series:
                     continue
 
                 ts.name = f"{entity}/{prefix}{signal}"
                 series.append(ts)
         return series
 
     @classmethod
@@ -816,20 +831,24 @@
         for signal, entity in self._data.columns:
             values = self._data[(signal, entity)]
             if not is_numeric_dtype(values) and any(~values.apply(_is_float)):
                 non_numeric_signals[signal].append(entity)
 
         _check_non_numeric_error(non_numeric_signals)
 
-    def _get_series_with_potential_duplicate_data_points(self, prefix: str) -> Sequence[pd.Series]:
+    def _get_series_with_potential_duplicate_data_points(
+        self,
+        prefix: str,
+        replace_existing_time_series: bool = False,
+    ) -> Sequence[pd.Series]:
         series = []
 
         for signal, entity in self._data.columns:
             ts = self._data[(signal, entity)].dropna()
-            if ts.empty:
+            if ts.empty and not replace_existing_time_series:
                 continue
 
             ts.name = f"{entity}/{prefix}{signal}"
             series.append(ts)
         return series
 
     @classmethod
@@ -877,123 +896,171 @@
     Container for metadata files which have a row for each combination of signal and entity.
 
     +-----------------------+----------+-----------------+-------------+
     | entity / figi / etc   | signal   | unit / currency | description |
     +-----------------------+----------+-----------------+-------------+
     | AAPL US               | my_sig   | USD             | million     |
     | MSFT US               | my_sig   | EUR             |             |
+    | AAPL US               | my_sig2  | ratio           |             |
+    | MSFT US               | my_sig2  | percent         |             |
     +-----------------------+----------+-----------------+-------------+
 
-    The unit, dimension and description columns are optional.
+    At least one of the columns currency, unit, or description must be present.
+    Only one of currency and unit can be set.
     """
 
-    RESERVED_COLUMNS = {"signal", "unit", "dimension", "description"}
+    RESERVED_COLUMNS = {"signal", "unit", "description"}
     UNIT_TYPE_COLUMNS = {"currency"}
+    UNIT_COLUMNS = UNIT_TYPE_COLUMNS.union({"unit"})
+    METADATA_COLUMNS = UNIT_COLUMNS.union({"description"})
     VALID_COLUMNS = RESERVED_COLUMNS.union(UNIT_TYPE_COLUMNS)
 
+    # Units that will be mapped to unit type ratio
+    RATIO_UNITS = {"percent", "ratio", "%"}
+
     @classmethod
     def is_valid(cls, data: pd.DataFrame) -> bool:
         if "signal" not in data.columns:
             return False
         entity_column = None
+        has_metadata_column = False
         for column in data.columns:
+            if column in cls.METADATA_COLUMNS:
+                has_metadata_column = True
             if column in cls.VALID_COLUMNS:
                 continue
             if entity_column is None and _is_valid_entity_column(
                 column=column, invalid=cls.VALID_COLUMNS
             ):
                 entity_column = column
                 continue
             return False
         if _has_duplicate_columns(data.columns):
             return False
-        return True
+        return has_metadata_column
 
     def validate_numeric(self) -> None:
         return None
 
     def get_series(
-        self, prefix: str, *, skip_validation: bool = False, unit_type: Optional[str] = None
+        self,
+        prefix: str,
+        *,
+        replace_existing_time_series: bool = False,
+        skip_validation: bool = False,
     ) -> ParsedTimeSeriesFile.ValidatedTimeSeries:
-        series = self._get_series_with_potential_duplicates(prefix, unit_type)
+        series: Sequence[TimeSeries] = self._get_series_with_potential_duplicates(prefix)
         failures = []
         if not skip_validation:
-            series_names_counter = Counter([ts.name for ts in series])
-            series_with_duplicate_names = []
-            series_deduplicated = []
-            for ts in series:
-                if series_names_counter[ts.name] > 1:
-                    series_with_duplicate_names.append(ts)
-                else:
-                    series_deduplicated.append(ts)
-            duplicates = self._entity_lookup_result.get_duplicates()
+            series_deduplicated, series_with_duplicate_names = self._get_deduplicated_series(series)
+            duplicate_entities = self._entity_lookup_result.get_duplicates()
             failures.extend(
                 [
                     ResourceCreationResult(
                         ResourceCreationStatus.FAILED,
                         ts,
                         RequestError(
                             ErrorType.INVALID_ARGUMENT,
-                            message=self._format_duplicate_message(str(ts.name), duplicates),
+                            message=self._format_duplicate_message(
+                                str(ts.name), duplicate_entities
+                            ),
                         ),
                     )
                     for ts in series_with_duplicate_names
                 ]
             )
             return self.ValidatedTimeSeries(series_deduplicated, failures)
         return self.ValidatedTimeSeries(series, failures)
 
-    def _get_series_with_potential_duplicates(
-        self, prefix: str, unit_type: Optional[str] = None
-    ) -> Sequence[TimeSeries]:
+    def _get_series_with_potential_duplicates(self, prefix: str) -> Sequence[TimeSeries]:
         """
         Creates a list of time series, one for each combination of entity and signal.
         The name of the time series is constructed from the entity and signal columns.
         The units of the time series are constructed from the unit and dimension
         columns. If a column name matches one of the unit types, that unit type takes
         precedence over the unit type argument.
 
         The time series are empty, as this format does not contain any data points.
         """
         series = []
-        unit_column = "unit"
 
         for _, row in self._data.iterrows():
             entity, signal = row["entity"], row["signal"]
             row = row.dropna()
-            unit = []
+            unit_column = "unit"
+            unit_type = "unknown"
+            units = []
+            has_unit = False
 
             for col in row.index:
+                if col in self.UNIT_COLUMNS:
+                    if has_unit:
+                        raise FileLoadingException(
+                            f"More than one unit specified for {row['entity']}, {row['signal']}"
+                        )
+                    has_unit = True
                 if col in self.UNIT_TYPE_COLUMNS:
                     unit_column = unit_type = col
-                    break
 
             if row.get(unit_column):
-                unit.append(
+                unit = row.get(unit_column)
+                units.append(
                     Unit(
-                        dimension=Dimension.from_string(unit_type)
-                        if unit_type
-                        else Dimension.DIMENSION_UNKNOWN,
-                        unit=row.get(unit_column),
+                        dimension=(
+                            Dimension.DIMENSION_RATIO
+                            if unit in self.RATIO_UNITS
+                            else Dimension.from_string(unit_type)
+                        ),
+                        unit=unit,
                     )
                 )
 
             series.append(
                 TimeSeries(
                     series=pd.Series(data=[], name=f"{entity}/{prefix}{signal}", dtype=object),
-                    units=Units(
-                        units=unit,
-                        description=row.get("description"),
-                    )
-                    if (unit or row.get("description"))
-                    else None,
+                    units=(
+                        Units(
+                            units=units,
+                            description=row.get("description"),
+                        )
+                        if (units or row.get("description"))
+                        else None
+                    ),
                 )
             )
         return series
 
+    @staticmethod
+    def _get_deduplicated_series(
+        series: Sequence[TimeSeries],
+    ) -> Tuple[Sequence[TimeSeries], Sequence[TimeSeries]]:
+        """Get the deduplicated series and series with duplicate names"""
+        series_dict = defaultdict(list)
+        for ts in series:
+            series_dict[ts.name].append(ts)
+
+        series_with_duplicate_names = []
+        series_deduplicated = []
+        for ts_name, ts_list in series_dict.items():
+            if len(ts_list) > 1:
+                if any(ts != ts_list[0] for ts in ts_list):
+                    logger.error(
+                        "Time series %s detected with the following different metadata", ts_name
+                    )
+                    for ts in ts_list:
+                        logger.error(ts.units)
+                    logger.error("The time series metadata will not be uploaded.")
+                    series_with_duplicate_names.extend(ts_list)
+                else:
+                    series_deduplicated.append(ts_list[0])
+            else:
+                series_deduplicated.extend(ts_list)
+
+        return series_deduplicated, series_with_duplicate_names
+
     @classmethod
     def _set_index(cls, data: pd.DataFrame) -> pd.DataFrame:
         return data
 
     @staticmethod
     def _format_duplicate_message(name: str, duplicates: Mapping[str, Sequence[str]]) -> str:
         entity_name = "/".join(name.split("/")[0:4])
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/file_writer_provider.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/file_writer_provider.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/athena_reader_configuration.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/athena_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/snowflake_reader.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/snowflake_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/sql_reader.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/sql_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import abc
 import logging
 from typing import Iterable, Iterator, NewType, Optional, Union
 
 import pandas as pd
 
+from exabel_data_sdk.services.file_writer import FileWritingResult
 from exabel_data_sdk.services.file_writer_provider import FileWriterProvider
 
 logger = logging.getLogger(__name__)
 
 Query = NewType("Query", str)
 OutputFile = NewType("OutputFile", str)
 OutputFilePrefix = NewType("OutputFilePrefix", str)
 BatchSize = NewType("BatchSize", int)
+FileFormat = NewType("FileFormat", str)
 
 
 class SqlReader(abc.ABC):
     """
     Abstract class for readers of SQL queries.
     """
 
@@ -43,21 +45,21 @@
 
     def read_sql_query_and_write_result(
         self,
         query: Query,
         output_file: Optional[OutputFile] = None,
         *,
         batch_size: Optional[BatchSize] = None,
-    ) -> None:
+    ) -> Optional[FileWritingResult]:
         """
         Execute the given query and write the result to the given output file. If no output file is
         given, print a sample instead.
         """
         if batch_size is None:
             df = self.read_sql_query(query)
         else:
             df = self.read_sql_query_in_batches(query, batch_size)
         if not output_file:
             logger.info("No output file specified. Printing sample.")
             logger.info(self.get_data_frame(df))
-            return
-        FileWriterProvider.get_file_writer(output_file).write_file(df, output_file)
+            return None
+        return FileWriterProvider.get_file_writer(output_file).write_file(df, output_file)
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/sql_reader_configuration.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/sql_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/services/sql/sqlalchemy_reader.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/services/sql/sqlalchemy_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/__init__.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/__init__.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .....exabel.api.time import time_range_pb2 as exabel_dot_api_dot_time_dot_time__range__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.type import decimal_pb2 as google_dot_type_dot_decimal__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-exabel/api/data/v1/time_series_messages.proto\x12\x12exabel.api.data.v1\x1a exabel/api/time/time_range.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x19google/type/decimal.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x84\x02\n\nTimeSeries\x12x\n\x04name\x18\x01 \x01(\tBj\x92AbJL"entityTypes/store/entities/ns.apple_store_fifth_avenue/signals/ns.visitors"\xca>\x11\xfa\x02\x0etimeSeriesName\xe2A\x02\x05\x02\x123\n\x06points\x18\x02 \x03(\x0b2#.exabel.api.data.v1.TimeSeriesPoint\x12\x17\n\tread_only\x18\x03 \x01(\x08B\x04\xe2A\x01\x03\x12.\n\x05units\x18\x04 \x01(\x0b2\x19.exabel.api.data.v1.UnitsB\x04\xe2A\x01\x01"\x9e\x01\n\x0fTimeSeriesPoint\x12.\n\x04time\x18\x01 \x01(\x0b2\x1a.google.protobuf.TimestampB\x04\xe2A\x01\x02\x12+\n\x05value\x18\x02 \x01(\x0b2\x1c.google.protobuf.DoubleValue\x12.\n\nknown_time\x18\x03 \x01(\x0b2\x1a.google.protobuf.Timestamp"v\n\x0eTimeSeriesView\x12.\n\ntime_range\x18\x01 \x01(\x0b2\x1a.exabel.api.time.TimeRange\x124\n\nknown_time\x18\x02 \x01(\x0b2\x1a.google.protobuf.TimestampB\x04\xe2A\x01\x01"\x9f\x01\n\x10DefaultKnownTime\x12\x16\n\x0ccurrent_time\x18\x01 \x01(\x08H\x00\x120\n\nknown_time\x18\x02 \x01(\x0b2\x1a.google.protobuf.TimestampH\x00\x120\n\x0btime_offset\x18\x03 \x01(\x0b2\x19.google.protobuf.DurationH\x00B\x0f\n\rspecification"\x83\x01\n\x05Units\x12.\n\x05units\x18\x01 \x03(\x0b2\x18.exabel.api.data.v1.UnitB\x05\xe2A\x02\x01\x05\x12/\n\nmultiplier\x18\x02 \x01(\x0b2\x14.google.type.DecimalB\x05\xe2A\x02\x01\x05\x12\x19\n\x0bdescription\x18\x03 \x01(\tB\x04\xe2A\x01\x01"\xec\x01\n\x04Unit\x12<\n\tdimension\x18\x01 \x01(\x0e2".exabel.api.data.v1.Unit.DimensionB\x05\xe2A\x02\x01\x05\x12\x13\n\x04unit\x18\x02 \x01(\tB\x05\xe2A\x02\x02\x05\x12\x17\n\x08exponent\x18\x03 \x01(\x11B\x05\xe2A\x02\x01\x05"x\n\tDimension\x12\x15\n\x11DIMENSION_UNKNOWN\x10\x00\x12\x16\n\x12DIMENSION_CURRENCY\x10\x01\x12\x12\n\x0eDIMENSION_MASS\x10\x02\x12\x14\n\x10DIMENSION_LENGTH\x10\x03\x12\x12\n\x0eDIMENSION_TIME\x10\x04BK\n\x16com.exabel.api.data.v1B\x17TimeSeriesMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-exabel/api/data/v1/time_series_messages.proto\x12\x12exabel.api.data.v1\x1a exabel/api/time/time_range.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x19google/type/decimal.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\x84\x02\n\nTimeSeries\x12x\n\x04name\x18\x01 \x01(\tBj\x92AbJL"entityTypes/store/entities/ns.apple_store_fifth_avenue/signals/ns.visitors"\xca>\x11\xfa\x02\x0etimeSeriesName\xe2A\x02\x05\x02\x123\n\x06points\x18\x02 \x03(\x0b2#.exabel.api.data.v1.TimeSeriesPoint\x12\x17\n\tread_only\x18\x03 \x01(\x08B\x04\xe2A\x01\x03\x12.\n\x05units\x18\x04 \x01(\x0b2\x19.exabel.api.data.v1.UnitsB\x04\xe2A\x01\x01"\x9e\x01\n\x0fTimeSeriesPoint\x12.\n\x04time\x18\x01 \x01(\x0b2\x1a.google.protobuf.TimestampB\x04\xe2A\x01\x02\x12+\n\x05value\x18\x02 \x01(\x0b2\x1c.google.protobuf.DoubleValue\x12.\n\nknown_time\x18\x03 \x01(\x0b2\x1a.google.protobuf.Timestamp"v\n\x0eTimeSeriesView\x12.\n\ntime_range\x18\x01 \x01(\x0b2\x1a.exabel.api.time.TimeRange\x124\n\nknown_time\x18\x02 \x01(\x0b2\x1a.google.protobuf.TimestampB\x04\xe2A\x01\x01"\x9f\x01\n\x10DefaultKnownTime\x12\x16\n\x0ccurrent_time\x18\x01 \x01(\x08H\x00\x120\n\nknown_time\x18\x02 \x01(\x0b2\x1a.google.protobuf.TimestampH\x00\x120\n\x0btime_offset\x18\x03 \x01(\x0b2\x19.google.protobuf.DurationH\x00B\x0f\n\rspecification"\x93\x01\n\x05Units\x12.\n\x05units\x18\x01 \x03(\x0b2\x18.exabel.api.data.v1.UnitB\x05\xe2A\x02\x01\x05\x12/\n\nmultiplier\x18\x02 \x01(\x0b2\x14.google.type.DecimalB\x05\xe2A\x02\x01\x05\x12\x19\n\x0bdescription\x18\x03 \x01(\tB\x04\xe2A\x01\x01J\x04\x08\x04\x10\x05R\x08is_ratio"\x82\x02\n\x04Unit\x12<\n\tdimension\x18\x01 \x01(\x0e2".exabel.api.data.v1.Unit.DimensionB\x05\xe2A\x02\x01\x05\x12\x13\n\x04unit\x18\x02 \x01(\tB\x05\xe2A\x02\x01\x05\x12\x17\n\x08exponent\x18\x03 \x01(\x11B\x05\xe2A\x02\x01\x05"\x8d\x01\n\tDimension\x12\x15\n\x11DIMENSION_UNKNOWN\x10\x00\x12\x16\n\x12DIMENSION_CURRENCY\x10\x01\x12\x12\n\x0eDIMENSION_MASS\x10\x02\x12\x14\n\x10DIMENSION_LENGTH\x10\x03\x12\x12\n\x0eDIMENSION_TIME\x10\x04\x12\x13\n\x0fDIMENSION_RATIO\x10\x05BK\n\x16com.exabel.api.data.v1B\x17TimeSeriesMessagesProtoP\x01Z\x16exabel.com/api/data/v1b\x06proto3')
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.data.v1.time_series_messages_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     _globals['DESCRIPTOR']._options = None
     _globals['DESCRIPTOR']._serialized_options = b'\n\x16com.exabel.api.data.v1B\x17TimeSeriesMessagesProtoP\x01Z\x16exabel.com/api/data/v1'
     _globals['_TIMESERIES'].fields_by_name['name']._options = None
@@ -33,24 +33,24 @@
     _globals['_UNITS'].fields_by_name['multiplier']._options = None
     _globals['_UNITS'].fields_by_name['multiplier']._serialized_options = b'\xe2A\x02\x01\x05'
     _globals['_UNITS'].fields_by_name['description']._options = None
     _globals['_UNITS'].fields_by_name['description']._serialized_options = b'\xe2A\x01\x01'
     _globals['_UNIT'].fields_by_name['dimension']._options = None
     _globals['_UNIT'].fields_by_name['dimension']._serialized_options = b'\xe2A\x02\x01\x05'
     _globals['_UNIT'].fields_by_name['unit']._options = None
-    _globals['_UNIT'].fields_by_name['unit']._serialized_options = b'\xe2A\x02\x02\x05'
+    _globals['_UNIT'].fields_by_name['unit']._serialized_options = b'\xe2A\x02\x01\x05'
     _globals['_UNIT'].fields_by_name['exponent']._options = None
     _globals['_UNIT'].fields_by_name['exponent']._serialized_options = b'\xe2A\x02\x01\x05'
     _globals['_TIMESERIES']._serialized_start = 309
     _globals['_TIMESERIES']._serialized_end = 569
     _globals['_TIMESERIESPOINT']._serialized_start = 572
     _globals['_TIMESERIESPOINT']._serialized_end = 730
     _globals['_TIMESERIESVIEW']._serialized_start = 732
     _globals['_TIMESERIESVIEW']._serialized_end = 850
     _globals['_DEFAULTKNOWNTIME']._serialized_start = 853
     _globals['_DEFAULTKNOWNTIME']._serialized_end = 1012
     _globals['_UNITS']._serialized_start = 1015
-    _globals['_UNITS']._serialized_end = 1146
-    _globals['_UNIT']._serialized_start = 1149
-    _globals['_UNIT']._serialized_end = 1385
-    _globals['_UNIT_DIMENSION']._serialized_start = 1265
-    _globals['_UNIT_DIMENSION']._serialized_end = 1385
+    _globals['_UNITS']._serialized_end = 1162
+    _globals['_UNIT']._serialized_start = 1165
+    _globals['_UNIT']._serialized_end = 1423
+    _globals['_UNIT_DIMENSION']._serialized_start = 1282
+    _globals['_UNIT_DIMENSION']._serialized_end = 1423
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
 
     @property
     def units(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Unit]:
         """The product of all individual unit parts of this unit. For instance, if a time series measures
         speed and is given in meters per second, it would have one unit
         `{ dimension: DIMENSION_LENGTH, unit: 'm' }` and one unit
-        `{ dimension: DIMENSION_TIME, unit: 's', exponent: -1 }. And if a time series measures a
+        `{ dimension: DIMENSION_TIME, unit: 's', exponent: -1 }.` And if a time series measures a
         monetary amount and is specified in United States dollars, it would have the single unit
         `{ dimension: DIMENSION_CURRENCY, unit: 'USD' }`.
         """
 
     @property
     def multiplier(self) -> google.type.decimal_pb2.Decimal:
         """The multiplier of the time series, with default value "1". For instance, if the time series is
@@ -218,34 +218,38 @@
         'The dimension is a monetary currency. A unit of this dimension must be one of the ISO-4217\n        three letter currency codes.\n        '
         DIMENSION_MASS: Unit._Dimension.ValueType
         'The dimension is a mass. The SI unit of mass is "kg", but other units may also be used.'
         DIMENSION_LENGTH: Unit._Dimension.ValueType
         'The dimension is a one dimensional size. The SI unit of length is "m", but other units may\n        also be used.\n        '
         DIMENSION_TIME: Unit._Dimension.ValueType
         'The dimension is an amount of time. The SI unit of time is "s", but other units may also be\n        used.\n        '
+        DIMENSION_RATIO: Unit._Dimension.ValueType
+        'This unit is a ratio (strictly speaking without a dimension). Symbol is typically\n        empty or "%".\n        '
 
     class Dimension(_Dimension, metaclass=_DimensionEnumTypeWrapper):
         """The supported dimensions in the Exabel platform."""
     DIMENSION_UNKNOWN: Unit.Dimension.ValueType
     "The dimension of this unit is unknown, but may be inferred from the unit's symbol."
     DIMENSION_CURRENCY: Unit.Dimension.ValueType
     'The dimension is a monetary currency. A unit of this dimension must be one of the ISO-4217\n    three letter currency codes.\n    '
     DIMENSION_MASS: Unit.Dimension.ValueType
     'The dimension is a mass. The SI unit of mass is "kg", but other units may also be used.'
     DIMENSION_LENGTH: Unit.Dimension.ValueType
     'The dimension is a one dimensional size. The SI unit of length is "m", but other units may\n    also be used.\n    '
     DIMENSION_TIME: Unit.Dimension.ValueType
     'The dimension is an amount of time. The SI unit of time is "s", but other units may also be\n    used.\n    '
+    DIMENSION_RATIO: Unit.Dimension.ValueType
+    'This unit is a ratio (strictly speaking without a dimension). Symbol is typically\n    empty or "%".\n    '
     DIMENSION_FIELD_NUMBER: builtins.int
     UNIT_FIELD_NUMBER: builtins.int
     EXPONENT_FIELD_NUMBER: builtins.int
     dimension: global___Unit.Dimension.ValueType
     'The dimension of this unit.'
     unit: builtins.str
-    'The short hand symbol of a dimension of this unit, for instance "m" or "EUR".'
+    'The short hand symbol of a dimension of this unit, for instance "m" or "EUR".\n    Required, except for ratio units.\n    '
     exponent: builtins.int
     "The exponent (power) of this unit. It can be positive or negative, but if it is 0, the unit's\n    exponent defaults to the value 1.\n    "
 
     def __init__(self, *, dimension: global___Unit.Dimension.ValueType | None=..., unit: builtins.str | None=..., exponent: builtins.int | None=...) -> None:
         ...
 
     def ClearField(self, field_name: typing_extensions.Literal['dimension', b'dimension', 'exponent', b'exponent', 'unit', b'unit']) -> None:
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.pyi` & `exabel_data_sdk-5.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/util/case_insensitive_column.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/util/case_insensitive_column.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/util/deprecate_arguments.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/util/deprecate_arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,29 @@
 
 FunctionT = TypeVar("FunctionT", bound=Callable[..., Any])
 
 
 @overload
 def deprecate_arguments(
     **deprecation_replacements: Optional[str],
-) -> Callable[[FunctionT], FunctionT]:
-    ...
+) -> Callable[[FunctionT], FunctionT]: ...
 
 
 @overload
 def deprecate_arguments(
     __func: None,  # pylint: disable=invalid-name
     **deprecation_replacements: Optional[str],
-) -> Callable[[FunctionT], FunctionT]:
-    ...
+) -> Callable[[FunctionT], FunctionT]: ...
 
 
 @overload
 def deprecate_arguments(
     __func: FunctionT,  # pylint: disable=invalid-name
     **deprecation_replacements: Optional[str],
-) -> FunctionT:
-    ...
+) -> FunctionT: ...
 
 
 # Pylint flags '__func' as an invalid argument name, but we want the '__' prefix to make Mypy
 # interpret it as a positional-only argument. Therefore, we disable the check for this argument.
 def deprecate_arguments(
     __func: Optional[FunctionT] = None,  # pylint: disable=invalid-name
     **deprecation_replacements: Optional[str],
@@ -89,32 +86,29 @@
 
 
 # Pylint flags '__func' as an invalid argument name, but we want the '__' prefix to make Mypy
 # interpret it as a positional-only argument. Therefore, we disable the check for this argument.
 @overload
 def deprecate_argument_value(
     **deprecated_values: object,
-) -> Callable[[FunctionT], FunctionT]:
-    ...
+) -> Callable[[FunctionT], FunctionT]: ...
 
 
 @overload
 def deprecate_argument_value(
     __func: None,  # pylint: disable=invalid-name
     **deprecated_values: object,
-) -> Callable[[FunctionT], FunctionT]:
-    ...
+) -> Callable[[FunctionT], FunctionT]: ...
 
 
 @overload
 def deprecate_argument_value(
     __func: FunctionT,  # pylint: disable=invalid-name
     **deprecated_values: object,
-) -> FunctionT:
-    ...
+) -> FunctionT: ...
 
 
 def deprecate_argument_value(
     __func: Optional[FunctionT] = None,  # pylint: disable=invalid-name
     **deprecated_values: object,
 ) -> FunctionT:
     """
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/util/handle_missing_imports.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/util/handle_missing_imports.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/util/import_.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/util/import_.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/util/parse_property_columns.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/util/parse_property_columns.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/util/resource_name_normalization.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/util/resource_name_normalization.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk/util/type_converter.py` & `exabel_data_sdk-5.2.0/exabel_data_sdk/util/type_converter.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk.egg-info/PKG-INFO` & `exabel_data_sdk-5.2.0/exabel_data_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exabel-data-sdk
-Version: 5.1.0
+Version: 5.2.0
 Summary: Python SDK for the Exabel Data API
 Home-page: https://github.com/Exabel/python-sdk
 Author: Exabel
 Author-email: support@exabel.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `exabel-data-sdk-5.1.0/exabel_data_sdk.egg-info/SOURCES.txt` & `exabel_data_sdk-5.2.0/exabel_data_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -325,11 +325,12 @@
 exabel_data_sdk/util/__init__.py
 exabel_data_sdk/util/batcher.py
 exabel_data_sdk/util/case_insensitive_column.py
 exabel_data_sdk/util/deprecate_arguments.py
 exabel_data_sdk/util/exceptions.py
 exabel_data_sdk/util/handle_missing_imports.py
 exabel_data_sdk/util/import_.py
+exabel_data_sdk/util/logging_thread_pool_executor.py
 exabel_data_sdk/util/parse_property_columns.py
 exabel_data_sdk/util/resource_name_normalization.py
 exabel_data_sdk/util/type_converter.py
 exabel_data_sdk/util/warnings.py
```

### Comparing `exabel-data-sdk-5.1.0/pyproject.toml` & `exabel_data_sdk-5.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-5.1.0/setup.py` & `exabel_data_sdk-5.2.0/setup.py`

 * *Files identical despite different names*

