# Comparing `tmp/metaflow-stubs-2.11.9.tar.gz` & `tmp/metaflow_stubs-2.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-stubs-2.11.9.tar", last modified: Fri Mar 29 22:28:02 2024, max compression
+gzip compressed data, was "metaflow_stubs-2.12.0.tar", last modified: Tue May 28 09:55:28 2024, max compression
```

## Comparing `metaflow-stubs-2.11.9.tar` & `metaflow_stubs-2.12.0.tar`

### file list

```diff
@@ -1,164 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.466081 metaflow-stubs-2.11.9/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-29 22:27:44.000000 metaflow-stubs-2.11.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-29 22:28:02.466081 metaflow-stubs-2.11.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-29 22:27:44.000000 metaflow-stubs-2.11.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.446081 metaflow-stubs-2.11.9/metaflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   107435 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/cli.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.446081 metaflow-stubs-2.11.9/metaflow-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/client/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/client/filecache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/clone_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/flowspec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/generated_for.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/includefile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.446081 metaflow-stubs-2.11.9/metaflow-stubs/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/metadata/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/metadata/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/metaflow_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/metaflow_current.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.446081 metaflow-stubs-2.11.9/metaflow-stubs/mflog/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/mflog/mflog.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/multicore_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/parameters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.450081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.450081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/exception.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.450081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.450081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14340 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_workflows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.454081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/aws_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/aws_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.454081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.454081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.454081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.454081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/azure_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/azure_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.458081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_creator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_datastore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.458081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/basic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/card.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.458081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/components.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/component_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/catch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.458081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/local.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.462081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/s3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/s3util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/debug_logger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/debug_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/environment_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/events_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.462081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/frameworks/pytorch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.462081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/gs_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.462081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/package_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/parallel_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/project_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.462081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/conda_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/conda_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/pypi_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/resources_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/retry_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.462081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/storage_executor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/tag_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/timeout_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/procpoll.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/pylint_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/tagging_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.466081 metaflow-stubs-2.11.9/metaflow_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-29 22:28:02.000000 metaflow-stubs-2.11.9/metaflow_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-03-29 22:28:02.000000 metaflow-stubs-2.11.9/metaflow_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 22:28:02.000000 metaflow-stubs-2.11.9/metaflow_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-29 22:28:02.000000 metaflow-stubs-2.11.9/metaflow_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-29 22:28:02.000000 metaflow-stubs-2.11.9/metaflow_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 22:28:02.466081 metaflow-stubs-2.11.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-29 22:27:44.000000 metaflow-stubs-2.11.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-29 22:28:02.000000 metaflow-stubs-2.11.9/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.796579 metaflow_stubs-2.12.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 09:55:03.000000 metaflow_stubs-2.12.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-28 09:55:28.796579 metaflow_stubs-2.12.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-28 09:55:03.000000 metaflow_stubs-2.12.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.776579 metaflow_stubs-2.12.0/metaflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   114255 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/cli.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.776579 metaflow_stubs-2.12.0/metaflow-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/client/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/client/filecache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/clone_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/flowspec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/generated_for.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/includefile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.776579 metaflow_stubs-2.12.0/metaflow-stubs/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/metadata/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/metadata/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/metaflow_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/metaflow_current.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.776579 metaflow_stubs-2.12.0/metaflow-stubs/mflog/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/mflog/mflog.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/multicore_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/parameters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.780579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.780579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/airflow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/airflow_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/airflow_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/exception.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.780579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.780579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/argo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/argo/argo_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/argo/argo_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/argo/argo_workflows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.780579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/aws_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/aws_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.784579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/batch/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/batch/batch_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.784579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.784579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.784579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/azure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/azure/azure_credential.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/azure/azure_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/azure/azure_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/azure/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.788579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_creator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_datastore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.788579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/basic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/card.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.788579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/components.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/component_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/catch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.788579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/local.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.788579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29098 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/s3/s3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/s3/s3util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/debug_logger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/debug_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/environment_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/events_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.792579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/frameworks/pytorch.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.792579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/gcp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/gcp/gs_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/gcp/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.792579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/kubernetes_jobsets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/logs_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/package_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/parallel_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/project_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.792579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/conda_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/conda_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/pypi_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/resources_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/retry_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.792579 metaflow_stubs-2.12.0/metaflow-stubs/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/secrets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/storage_executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/tag_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/plugins/timeout_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/procpoll.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/pylint_wrapper.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.796579 metaflow_stubs-2.12.0/metaflow-stubs/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/runner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23267 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/runner/metaflow_runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/runner/nbrun.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/runner/subprocess_manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/tagging_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/tuple_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-28 09:55:27.000000 metaflow_stubs-2.12.0/metaflow-stubs/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:28.796579 metaflow_stubs-2.12.0/metaflow_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-28 09:55:28.000000 metaflow_stubs-2.12.0/metaflow_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-28 09:55:28.000000 metaflow_stubs-2.12.0/metaflow_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:55:28.000000 metaflow_stubs-2.12.0/metaflow_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 09:55:28.000000 metaflow_stubs-2.12.0/metaflow_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 09:55:28.000000 metaflow_stubs-2.12.0/metaflow_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:55:28.796579 metaflow_stubs-2.12.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-28 09:55:03.000000 metaflow_stubs-2.12.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 09:55:28.000000 metaflow_stubs-2.12.0/version.py
```

### Comparing `metaflow-stubs-2.11.9/PKG-INFO` & `metaflow_stubs-2.12.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-stubs
-Version: 2.11.9
+Version: 2.12.0
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Requires-Dist: metaflow==2.11.9
+Requires-Dist: metaflow==2.12.0
 
 # Metaflow Stubs
 
 This package contains stub files for `metaflow` and thus offers type hints for various editors (such as `VSCode`) and language servers (such as `Pylance`).
 
 ## Installation
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/__init__.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.911417                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.155006                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.parameters
+    import metaflow._vendor.click.types
     import metaflow.datastore.inputs
+    import datetime
+    import metaflow.client.core
     import metaflow.plugins.datatools.s3.s3
-    import metaflow.metaflow_current
     import typing
+    import metaflow.metaflow_current
     import io
     import metaflow.events
-    import metaflow.parameters
-    import datetime
-    import metaflow.client.core
-    import metaflow._vendor.click.types
+    import metaflow.runner.metaflow_runner
 FlowSpecDerived = typing.TypeVar("FlowSpecDerived", bound="FlowSpec", contravariant=False, covariant=False)
 StepFlag = typing.NewType("StepFlag", bool)
 
 CURRENT_DIRECTORY: str
 
 INFO_FILE: str
 
@@ -722,129 +723,14 @@
     -------
     Union[Callable[[FlowSpecDerived, StepFlag], None], Callable[[FlowSpecDerived, Any, StepFlag], None]]
         Function that is a Metaflow Step
     """
     ...
 
 @typing.overload
-def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
-    
-    Note that you may add multiple `@card` decorators in a step with different parameters.
-    
-    Parameters
-    ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
-    
-    
-    """
-    ...
-
-@typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
-    """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
-    
-    Note that you may add multiple `@card` decorators in a step with different parameters.
-    
-    Parameters
-    ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
-    
-    
-    """
-    ...
-
-@typing.overload
-def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies environment variables to be set prior to the execution of a step.
-    
-    Parameters
-    ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
-    """
-    ...
-
-@typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
-    """
-    Specifies environment variables to be set prior to the execution of a step.
-    
-    Parameters
-    ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
-    """
-    ...
-
-@typing.overload
-def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
-    
-    Parameters
-    ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
-    """
-    ...
-
-@typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
-    """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
-    
-    Parameters
-    ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
-    """
-    ...
-
-@typing.overload
 def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the resources needed when executing this step.
     
     Use `@resources` to specify the resource requirements
     independently of the specific compute layer (`@batch`, `@kubernetes`).
     
@@ -913,14 +799,73 @@
         Memory size (in MB) required for this step.
     shared_memory : int, optional, default None
         The value for the size (in MiB) of the /dev/shm volume for this step.
         This parameter maps to the `--shm-size` option in Docker.
     """
     ...
 
+def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, shared_memory: typing.Optional[int] = None, port: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies that this step should execute on Kubernetes.
+    
+    Parameters
+    ----------
+    cpu : int, default 1
+        Number of CPUs required for this step. If `@resources` is
+        also present, the maximum value from all decorators is used.
+    memory : int, default 4096
+        Memory size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    disk : int, default 10240
+        Disk size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    image : str, optional, default None
+        Docker image to use when launching on Kubernetes. If not specified, and
+        METAFLOW_KUBERNETES_CONTAINER_IMAGE is specified, that image is used. If
+        not, a default Docker image mapping to the current version of Python is used.
+    image_pull_policy: str, default KUBERNETES_IMAGE_PULL_POLICY
+        If given, the imagePullPolicy to be applied to the Docker image of the step.
+    service_account : str, default METAFLOW_KUBERNETES_SERVICE_ACCOUNT
+        Kubernetes service account to use when launching pod in Kubernetes.
+    secrets : List[str], optional, default None
+        Kubernetes secrets to use when launching pod in Kubernetes. These
+        secrets are in addition to the ones defined in `METAFLOW_KUBERNETES_SECRETS`
+        in Metaflow configuration.
+    namespace : str, default METAFLOW_KUBERNETES_NAMESPACE
+        Kubernetes namespace to use when launching pod in Kubernetes.
+    gpu : int, optional, default None
+        Number of GPUs required for this step. A value of zero implies that
+        the scheduled node should not have GPUs.
+    gpu_vendor : str, default KUBERNETES_GPU_VENDOR
+        The vendor of the GPUs to be used for this step.
+    tolerations : List[str], default []
+        The default is extracted from METAFLOW_KUBERNETES_TOLERATIONS.
+        Kubernetes tolerations to use when launching pod in Kubernetes.
+    use_tmpfs : bool, default False
+        This enables an explicit tmpfs mount for this step.
+    tmpfs_tempdir : bool, default True
+        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
+    tmpfs_size : int, optional, default: None
+        The value for the size (in MiB) of the tmpfs mount for this step.
+        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
+        memory allocated for this step.
+    tmpfs_path : str, optional, default /metaflow_temp
+        Path to tmpfs mount for this step.
+    persistent_volume_claims : Dict[str, str], optional, default None
+        A map (dictionary) of persistent volumes to be mounted to the pod for this step. The map is from persistent
+        volumes to the path to which the volume is to be mounted, e.g., `{'pvc-name': '/path/to/mount/on'}`.
+    shared_memory: int, optional
+        Shared memory size (in MiB) required for this step
+    port: int, optional
+        Port number to specify in the Kubernetes job object
+    """
+    ...
+
 @typing.overload
 def batch(*, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
     
     Parameters
     ----------
@@ -971,23 +916,23 @@
         Path to tmpfs mount for this step. Defaults to /metaflow_temp.
     inferentia : int, default 0
         Number of Inferentia chips required for this step.
     trainium : int, default None
         Alias for inferentia. Use only one of the two.
     efa : int, default 0
         Number of elastic fabric adapter network devices to attach to container
-    ephemeral_storage: int, default None
-        The total amount, in GiB, of ephemeral storage to set for the task (21-200)
+    ephemeral_storage : int, default None
+        The total amount, in GiB, of ephemeral storage to set for the task, 21-200GiB.
         This is only relevant for Fargate compute environments
     log_driver: str, optional, default None
         The log driver to use for the Amazon ECS container.
     log_options: List[str], optional, default None
         List of strings containing options for the chosen log driver. The configurable values
         depend on the `log driver` chosen. Validation of these options is not supported yet.
-        Example usage: ["awslogs-group:aws/batch/job"]
+        Example: [`awslogs-group:aws/batch/job`]
     """
     ...
 
 @typing.overload
 def batch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
@@ -1048,72 +993,144 @@
         Path to tmpfs mount for this step. Defaults to /metaflow_temp.
     inferentia : int, default 0
         Number of Inferentia chips required for this step.
     trainium : int, default None
         Alias for inferentia. Use only one of the two.
     efa : int, default 0
         Number of elastic fabric adapter network devices to attach to container
-    ephemeral_storage: int, default None
-        The total amount, in GiB, of ephemeral storage to set for the task (21-200)
+    ephemeral_storage : int, default None
+        The total amount, in GiB, of ephemeral storage to set for the task, 21-200GiB.
         This is only relevant for Fargate compute environments
     log_driver: str, optional, default None
         The log driver to use for the Amazon ECS container.
     log_options: List[str], optional, default None
         List of strings containing options for the chosen log driver. The configurable values
         depend on the `log driver` chosen. Validation of these options is not supported yet.
-        Example usage: ["awslogs-group:aws/batch/job"]
+        Example: [`awslogs-group:aws/batch/job`]
     """
     ...
 
 @typing.overload
-def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the PyPI packages for the step.
+    Specifies a timeout for your step.
     
-    Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
+    This decorator is useful if this step may hang indefinitely.
+    
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
     
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
     """
     ...
 
 @typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
+def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
     """
-    Specifies the PyPI packages for the step.
+    Specifies a timeout for your step.
     
-    Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
+    This decorator is useful if this step may hang indefinitely.
+    
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
     
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
+    """
+    ...
+
+@typing.overload
+def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies environment variables to be set prior to the execution of a step.
+    
+    Parameters
+    ----------
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
+    """
+    ...
+
+@typing.overload
+def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
+    """
+    Specifies environment variables to be set prior to the execution of a step.
+    
+    Parameters
+    ----------
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
+    """
+    ...
+
+@typing.overload
+def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
+    
+    Parameters
+    ----------
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
+    """
+    ...
+
+@typing.overload
+def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
+    """
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
+    
+    Parameters
+    ----------
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
     """
     ...
 
 @typing.overload
 def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the number of times the task corresponding
@@ -1163,14 +1180,65 @@
         Number of times to retry this task.
     minutes_between_retries : int, default 2
         Number of minutes between retries.
     """
     ...
 
 @typing.overload
+def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Creates a human-readable report, a Metaflow Card, after this step completes.
+    
+    Note that you may add multiple `@card` decorators in a step with different parameters.
+    
+    Parameters
+    ----------
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
+    """
+    ...
+
+@typing.overload
+def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
+    """
+    Creates a human-readable report, a Metaflow Card, after this step completes.
+    
+    Note that you may add multiple `@card` decorators in a step with different parameters.
+    
+    Parameters
+    ----------
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
+    """
+    ...
+
+@typing.overload
 def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that the step will success under all circumstances.
     
     The decorator will create an optional artifact, specified by `var`, which
     contains the exception raised. You can use it to detect the presence
     of errors, indicating that all happy-path artifacts produced by the step
@@ -1211,68 +1279,60 @@
         If not specified, the exception is not stored.
     print_exception : bool, default True
         Determines whether or not the exception is printed to
         stdout when caught.
     """
     ...
 
-def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+@typing.overload
+def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies that this step should execute on Kubernetes.
+    Specifies the PyPI packages for the step.
+    
+    Information in this decorator will augment any
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
     Parameters
     ----------
-    cpu : int, default 1
-        Number of CPUs required for this step. If `@resources` is
-        also present, the maximum value from all decorators is used.
-    memory : int, default 4096
-        Memory size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
-    disk : int, default 10240
-        Disk size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
-    image : str, optional, default None
-        Docker image to use when launching on Kubernetes. If not specified, and
-        METAFLOW_KUBERNETES_CONTAINER_IMAGE is specified, that image is used. If
-        not, a default Docker image mapping to the current version of Python is used.
-    image_pull_policy: str, default KUBERNETES_IMAGE_PULL_POLICY
-        If given, the imagePullPolicy to be applied to the Docker image of the step.
-    service_account : str, default METAFLOW_KUBERNETES_SERVICE_ACCOUNT
-        Kubernetes service account to use when launching pod in Kubernetes.
-    secrets : List[str], optional, default None
-        Kubernetes secrets to use when launching pod in Kubernetes. These
-        secrets are in addition to the ones defined in `METAFLOW_KUBERNETES_SECRETS`
-        in Metaflow configuration.
-    namespace : str, default METAFLOW_KUBERNETES_NAMESPACE
-        Kubernetes namespace to use when launching pod in Kubernetes.
-    gpu : int, optional, default None
-        Number of GPUs required for this step. A value of zero implies that
-        the scheduled node should not have GPUs.
-    gpu_vendor : str, default KUBERNETES_GPU_VENDOR
-        The vendor of the GPUs to be used for this step.
-    tolerations : List[str], default []
-        The default is extracted from METAFLOW_KUBERNETES_TOLERATIONS.
-        Kubernetes tolerations to use when launching pod in Kubernetes.
-    use_tmpfs : bool, default False
-        This enables an explicit tmpfs mount for this step.
-    tmpfs_tempdir : bool, default True
-        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
-    tmpfs_size : int, optional, default: None
-        The value for the size (in MiB) of the tmpfs mount for this step.
-        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
-        memory allocated for this step.
-    tmpfs_path : str, optional, default /metaflow_temp
-        Path to tmpfs mount for this step.
-    persistent_volume_claims : Dict[str, str], optional, default None
-        A map (dictionary) of persistent volumes to be mounted to the pod for this step. The map is from persistent
-        volumes to the path to which the volume is to be mounted, e.g., `{'pvc-name': '/path/to/mount/on'}`.
-    shared_memory: int, optional
-        Shared memory size (in MiB) required for this step
+    packages : Dict[str, str], default: {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    """
+    ...
+
+@typing.overload
+def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
+    """
+    Specifies the PyPI packages for the step.
+    
+    Information in this decorator will augment any
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
+    
+    Parameters
+    ----------
+    packages : Dict[str, str], default: {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
 def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the Conda environment for the step.
@@ -1326,89 +1386,14 @@
         that the version used will correspond to the version of the Python interpreter used to start the run.
     disabled : bool, default False
         If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
-    
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
-    
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
-    
-    Parameters
-    ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
-    """
-    ...
-
-@typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
-    """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
-    
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
-    
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
-    
-    Parameters
-    ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
-    """
-    ...
-
-def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies what flows belong to the same project.
-    
-    A project-specific namespace is created for all flows that
-    use the same `@project(name)`.
-    
-    Parameters
-    ----------
-    name : str
-        Project name. Make sure that the name is unique amongst all
-        projects that use the same production scheduler. The name may
-        contain only lowercase alphanumeric characters and underscores.
-    
-    
-    """
-    ...
-
-@typing.overload
 def trigger(*, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the event(s) that this flow depends on.
     
     ```
     @trigger(event='foo')
     ```
@@ -1495,14 +1480,32 @@
     options : Dict[str, Any], default {}
         Backend-specific configuration for tuning eventing behavior.
     
     
     """
     ...
 
+def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies what flows belong to the same project.
+    
+    A project-specific namespace is created for all flows that
+    use the same `@project(name)`.
+    
+    Parameters
+    ----------
+    name : str
+        Project name. Make sure that the name is unique amongst all
+        projects that use the same production scheduler. The name may
+        contain only lowercase alphanumeric characters and underscores.
+    
+    
+    """
+    ...
+
 @typing.overload
 def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the PyPI packages for all steps of the flow.
     
     Use `@pypi_base` to set common packages required by all
     steps and use `@pypi` to specify step-specific overrides.
@@ -1534,21 +1537,18 @@
         and the value is the version to use.
     python : str, optional, default: None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
-def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
-    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
-    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
-    added as a flow decorators. Adding more than one decorator will ensure that `start` step
-    starts only after all sensors finish.
+    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
+    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
     
     Parameters
     ----------
     timeout : int
         Time, in seconds before the task times out and fails. (Default: 3600)
     poke_interval : int
         Time in seconds that the job should wait in between each try. (Default: 60)
@@ -1561,75 +1561,29 @@
         slot pools are a way to limit concurrency for certain tasks. (Default:None)
     soft_fail : bool
         Set to true to mark the task as SKIPPED on failure. (Default: False)
     name : str
         Name of the sensor on Airflow
     description : str
         Description of sensor in the Airflow UI
-    bucket_key : Union[str, List[str]]
-        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
-        When it's specified as a full s3:// url, please leave `bucket_name` as None
-    bucket_name : str
-        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
-        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
-    wildcard_match : bool
-        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
-    aws_conn_id : str
-        a reference to the s3 connection on Airflow. (Default: None)
-    verify : bool
-        Whether or not to verify SSL certificates for S3 connection. (Default: None)
-    """
-    ...
-
-@typing.overload
-def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the Conda environment for all steps of the flow.
-    
-    Use `@conda_base` to set common libraries required by all
-    steps and use `@conda` to specify step-specific additions.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables Conda.
-    """
-    ...
-
-@typing.overload
-def conda_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def conda_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
-    """
-    Specifies the Conda environment for all steps of the flow.
-    
-    Use `@conda_base` to set common libraries required by all
-    steps and use `@conda` to specify step-specific additions.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables Conda.
+    external_dag_id : str
+        The dag_id that contains the task you want to wait for.
+    external_task_ids : List[str]
+        The list of task_ids that you want to wait for.
+        If None (default value) the sensor waits for the DAG. (Default: None)
+    allowed_states : List[str]
+        Iterable of allowed states, (Default: ['success'])
+    failed_states : List[str]
+        Iterable of failed or dis-allowed states. (Default: None)
+    execution_delta : datetime.timedelta
+        time difference with the previous execution to look at,
+        the default is the same logical date as the current task or DAG. (Default: None)
+    check_existence: bool
+        Set to True to check if the external task exists or check if
+        the DAG to wait for exists. (Default: True)
     """
     ...
 
 @typing.overload
 def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the flow(s) that this flow depends on.
@@ -1777,18 +1731,21 @@
         specified by this expression.
     timezone : str, optional, default None
         Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
         which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
     """
     ...
 
-def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
-    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
+    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
+    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
+    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
+    added as a flow decorators. Adding more than one decorator will ensure that `start` step
+    starts only after all sensors finish.
     
     Parameters
     ----------
     timeout : int
         Time, in seconds before the task times out and fails. (Default: 3600)
     poke_interval : int
         Time in seconds that the job should wait in between each try. (Default: 60)
@@ -1801,29 +1758,75 @@
         slot pools are a way to limit concurrency for certain tasks. (Default:None)
     soft_fail : bool
         Set to true to mark the task as SKIPPED on failure. (Default: False)
     name : str
         Name of the sensor on Airflow
     description : str
         Description of sensor in the Airflow UI
-    external_dag_id : str
-        The dag_id that contains the task you want to wait for.
-    external_task_ids : List[str]
-        The list of task_ids that you want to wait for.
-        If None (default value) the sensor waits for the DAG. (Default: None)
-    allowed_states : List[str]
-        Iterable of allowed states, (Default: ['success'])
-    failed_states : List[str]
-        Iterable of failed or dis-allowed states. (Default: None)
-    execution_delta : datetime.timedelta
-        time difference with the previous execution to look at,
-        the default is the same logical date as the current task or DAG. (Default: None)
-    check_existence: bool
-        Set to True to check if the external task exists or check if
-        the DAG to wait for exists. (Default: True)
+    bucket_key : Union[str, List[str]]
+        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
+        When it's specified as a full s3:// url, please leave `bucket_name` as None
+    bucket_name : str
+        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
+        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
+    wildcard_match : bool
+        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
+    aws_conn_id : str
+        a reference to the s3 connection on Airflow. (Default: None)
+    verify : bool
+        Whether or not to verify SSL certificates for S3 connection. (Default: None)
+    """
+    ...
+
+@typing.overload
+def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the Conda environment for all steps of the flow.
+    
+    Use `@conda_base` to set common libraries required by all
+    steps and use `@conda` to specify step-specific additions.
+    
+    Parameters
+    ----------
+    packages : Dict[str, str], default {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables Conda.
+    """
+    ...
+
+@typing.overload
+def conda_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def conda_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
+    """
+    Specifies the Conda environment for all steps of the flow.
+    
+    Use `@conda_base` to set common libraries required by all
+    steps and use `@conda` to specify step-specific additions.
+    
+    Parameters
+    ----------
+    packages : Dict[str, str], default {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables Conda.
     """
     ...
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
@@ -2769,7 +2772,205 @@
         ...
     def __getstate__(self):
         ...
     def __setstate__(self, state):
         ...
     ...
 
+class Runner(object, metaclass=type):
+    def __init__(self, flow_file: str, show_output: bool = True, profile: typing.Optional[str] = None, env: typing.Optional[typing.Dict] = None, cwd: typing.Optional[str] = None, **kwargs):
+        ...
+    def __enter__(self) -> metaflow.runner.metaflow_runner.Runner:
+        ...
+    def __aenter__(self) -> metaflow.runner.metaflow_runner.Runner:
+        ...
+    def _Runner__get_executing_run(self, tfp_runner_attribute, command_obj):
+        ...
+    def run(self, **kwargs) -> metaflow.runner.metaflow_runner.ExecutingRun:
+        """
+        Blocking execution of the run. This method will wait until
+        the run has completed execution.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `run` command, in particular, any parameters accepted by the flow.
+        
+        Returns
+        -------
+        ExecutingRun
+            ExecutingRun containing the results of the run.
+        """
+        ...
+    def resume(self, **kwargs):
+        """
+        Blocking resume execution of the run.
+        This method will wait until the resumed run has completed execution.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python ./myflow.py` after
+            the `resume` command.
+        
+        Returns
+        -------
+        ExecutingRun
+            ExecutingRun containing the results of the resumed run.
+        """
+        ...
+    def async_run(self, **kwargs) -> metaflow.runner.metaflow_runner.ExecutingRun:
+        """
+        Non-blocking execution of the run. This method will return as soon as the
+        run has launched.
+        
+        Note that this method is asynchronous and needs to be `await`ed.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `run` command, in particular, any parameters accepted by the flow.
+        
+        Returns
+        -------
+        ExecutingRun
+            ExecutingRun representing the run that was started.
+        """
+        ...
+    def async_resume(self, **kwargs):
+        """
+        Non-blocking resume execution of the run.
+        This method will return as soon as the resume has launched.
+        
+        Note that this method is asynchronous and needs to be `await`ed.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `resume` command.
+        
+        Returns
+        -------
+        ExecutingRun
+            ExecutingRun representing the resumed run that was started.
+        """
+        ...
+    def __exit__(self, exc_type, exc_value, traceback):
+        ...
+    def __aexit__(self, exc_type, exc_value, traceback):
+        ...
+    def cleanup(self):
+        """
+        Delete any temporary files created during execution.
+        """
+        ...
+    ...
+
+class NBRunner(object, metaclass=type):
+    def __init__(self, flow, show_output: bool = True, profile: typing.Optional[str] = None, env: typing.Optional[typing.Dict] = None, base_dir: str = "/tmp", **kwargs):
+        ...
+    def nbrun(self, **kwargs):
+        """
+        Blocking execution of the run. This method will wait until
+        the run has completed execution.
+        
+        Note that in contrast to `run`, this method returns a
+        `metaflow.Run` object directly and calls `cleanup()` internally
+        to support a common notebook pattern of executing a flow and
+        retrieving its results immediately.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `run` command, in particular, any parameters accepted by the flow.
+        
+        Returns
+        -------
+        Run
+            A `metaflow.Run` object representing the finished run.
+        """
+        ...
+    def nbresume(self, **kwargs):
+        """
+        Blocking resuming of a run. This method will wait until
+        the resumed run has completed execution.
+        
+        Note that in contrast to `resume`, this method returns a
+        `metaflow.Run` object directly and calls `cleanup()` internally
+        to support a common notebook pattern of executing a flow and
+        retrieving its results immediately.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `resume` command.
+        
+        Returns
+        -------
+        Run
+            A `metaflow.Run` object representing the resumed run.
+        """
+        ...
+    def run(self, **kwargs):
+        """
+        Runs the flow.
+        """
+        ...
+    def resume(self, **kwargs):
+        """
+        Resumes the flow.
+        """
+        ...
+    def async_run(self, **kwargs):
+        """
+        Non-blocking execution of the run. This method will return as soon as the
+        run has launched. This method is equivalent to `Runner.async_run`.
+        
+        Note that this method is asynchronous and needs to be `await`ed.
+        
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `run` command, in particular, any parameters accepted by the flow.
+        
+        Returns
+        -------
+        ExecutingRun
+            ExecutingRun representing the run that was started.
+        """
+        ...
+    def async_resume(self, **kwargs):
+        """
+        Non-blocking execution of the run. This method will return as soon as the
+        run has launched. This method is equivalent to `Runner.async_resume`.
+        
+        Note that this method is asynchronous and needs to be `await`ed.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `run` command, in particular, any parameters accepted by the flow.
+        
+        Returns
+        -------
+        ExecutingRun
+            ExecutingRun representing the run that was started.
+        """
+        ...
+    def cleanup(self):
+        """
+        Delete any temporary files created during execution.
+        
+        Call this method after using `async_run` or `async_resume`. You don't
+        have to call this after `nbrun` or `nbresume`.
+        """
+        ...
+    ...
+
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/cards.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/cards.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.937079                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.178939                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
-    import typing
-    import metaflow.plugins.cards.card_modules.basic
-    import metaflow.plugins.cards.card_modules.components
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.plugins.cards.card_modules.components
+    import typing
     import metaflow.plugins.cards.card_client
+    import metaflow.plugins.cards.card_modules.basic
 
 def get_cards(task: typing.Union[str, "metaflow.Task"], id: typing.Optional[str] = None, type: typing.Optional[str] = None, follow_resumed: bool = True) -> metaflow.plugins.cards.card_client.CardContainer:
     """
     Get cards related to a `Task`.
     
     Note that `get_cards` resolves the cards contained by the task, but it doesn't actually
     retrieve them from the datastore. Actual card contents are retrieved lazily either when
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/cli.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/cli.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.943055                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.188718                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
@@ -27,69 +27,89 @@
     Returns
     -------
     str, optional
         Namespace set (result of get_namespace()).
     """
     ...
 
-current: metaflow.metaflow_current.Current
-
-def validate_tags(tags, existing_tags = None):
+def get_metadata() -> str:
     """
-    Raises MetaflowTaggingError if invalid based on these rules:
+    Returns the current Metadata provider.
     
-    Tag set size is too large. But it's OK if tag set is not larger
-    than an existing tag set (if provided).
+    If this is not set explicitly using `metadata`, the default value is
+    determined through the Metaflow configuration. You can use this call to
+    check that your configuration is set up properly.
     
-    Then, we validate each tag.  See validate_tag()
+    If multiple configuration profiles are present, this call returns the one
+    selected through the `METAFLOW_PROFILE` environment variable.
+    
+    Returns
+    -------
+    str
+        Information about the Metadata provider currently selected. This information typically
+        returns provider specific information (like URL for remote providers or local paths for
+        local providers).
     """
     ...
 
 class CommandException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-DATASTORES: list
-
-ENVIRONMENTS: list
-
-LOGGING_SIDECARS: dict
-
-METADATA_PROVIDERS: list
-
-MONITOR_SIDECARS: dict
-
 DEFAULT_DATASTORE: str
 
 DEFAULT_ENVIRONMENT: str
 
 DEFAULT_EVENT_LOGGER: str
 
 DEFAULT_METADATA: str
 
 DEFAULT_MONITOR: str
 
 DEFAULT_PACKAGE_SUFFIXES: str
 
+current: metaflow.metaflow_current.Current
+
+LOG_SOURCES: list
+
+DATASTORES: list
+
+ENVIRONMENTS: list
+
+LOGGING_SIDECARS: dict
+
+METADATA_PROVIDERS: list
+
+MONITOR_SIDECARS: dict
+
 class PyLint(object, metaclass=type):
     def __init__(self, fname):
         ...
     def has_pylint(self):
         ...
     def run(self, logger = None, warnings = False, pylint_config = []):
         ...
     ...
 
-LOG_SOURCES: list
+def validate_tags(tags, existing_tags = None):
+    """
+    Raises MetaflowTaggingError if invalid based on these rules:
+    
+    Tag set size is too large. But it's OK if tag set is not larger
+    than an existing tag set (if provided).
+    
+    Then, we validate each tag.  See validate_tag()
+    """
+    ...
 
 UBF_CONTROL: str
 
 UBF_TASK: str
 
 ERASE_TO_EOL: str
 
@@ -111,15 +131,15 @@
 
 def logger(body = "", system_msg = False, head = "", bad = False, timestamp = True, nl = True):
     ...
 
 def common_run_options(func):
     ...
 
-def write_run_id(run_id_file, run_id):
+def write_file(file_path, content):
     ...
 
 def before_run(obj, tags, decospecs):
     ...
 
 def print_metaflow_exception(ex):
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/client/__init__.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/client/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.940233                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.181932                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.client.core
+    import metaflow.events
     import datetime
     import typing
-    import metaflow.events
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/client/core.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/client/core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.922677                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.165323                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
-    import metaflow.metaflow_current
+    import datetime
+    import metaflow.client.core
     import typing
-    import metaflow.exception
+    import metaflow.metaflow_current
     import metaflow.events
-    import metaflow.client.core
-    import datetime
     import tarfile
+    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/client/filecache.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/client/filecache.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.944136                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.189755                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.datastore.content_addressed_store
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/clone_util.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/clone_util.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.940759                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.187329                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaDatum(tuple, metaclass=type):
     @staticmethod
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/events.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/events.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.925117                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.167869                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow
     import metaflow.events
+    import metaflow
 
 TYPE_CHECKING: bool
 
 class MetaflowEvent(tuple, metaclass=type):
     @staticmethod
     def __new__(_cls, name, id, timestamp, type):
         """
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/exception.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/exception.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.912556                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.156081                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/flowspec.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/flowspec.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.924344                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.166982                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.unbounded_foreach
+    import metaflow.parameters
     import metaflow.datastore.inputs
+    import metaflow.unbounded_foreach
     import typing
     import metaflow.exception
-    import metaflow.parameters
 
 class DelayedEvaluationParameter(object, metaclass=type):
     def __init__(self, name, field, fun):
         ...
     def __call__(self, return_str = False):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/includefile.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/includefile.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.934714                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.176873                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.parameters
+    import metaflow._vendor.click.types
     import metaflow.plugins.datatools.s3.s3
     import typing
     import io
-    import metaflow.parameters
-    import metaflow._vendor.click.types
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/metadata/metadata.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/metadata/metadata.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.966396                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.211687                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metadata.metadata
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/metaflow_config.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/metaflow_config.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.913832                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.157447                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
@@ -24,14 +24,16 @@
 
 DEFAULT_MONITOR: str
 
 DEFAULT_PACKAGE_SUFFIXES: str
 
 DEFAULT_AWS_CLIENT_PROVIDER: str
 
+DEFAULT_GCP_CLIENT_PROVIDER: str
+
 DEFAULT_SECRETS_BACKEND_TYPE: None
 
 DEFAULT_SECRETS_ROLE: None
 
 USER: None
 
 DATASTORE_LOCAL_DIR: str
@@ -80,14 +82,18 @@
 
 DATATOOLS_GSROOT: None
 
 DATATOOLS_LOCALROOT: None
 
 AWS_SECRETS_MANAGER_DEFAULT_REGION: None
 
+GCP_SECRET_MANAGER_PREFIX: None
+
+AZURE_KEY_VAULT_PREFIX: None
+
 ARTIFACT_LOCALROOT: str
 
 CARD_SUFFIX: str
 
 CARD_LOCALROOT: None
 
 CARD_S3ROOT: None
@@ -122,14 +128,16 @@
 
 DEFAULT_CONTAINER_REGISTRY: None
 
 INCLUDE_FOREACH_STACK: bool
 
 MAXIMUM_FOREACH_VALUE_CHARS: int
 
+DEFAULT_RUNTIME_LIMIT: int
+
 UI_URL: None
 
 CONTACT_INFO: dict
 
 ECS_S3_ACCESS_IAM_ROLE: None
 
 ECS_FARGATE_EXECUTION_ROLE: None
@@ -178,18 +186,30 @@
 
 KUBERNETES_CONTAINER_REGISTRY: None
 
 KUBERNETES_FETCH_EC2_METADATA: bool
 
 KUBERNETES_SHARED_MEMORY: None
 
+KUBERNETES_PORT: None
+
+KUBERNETES_CPU: None
+
+KUBERNETES_MEMORY: None
+
+KUBERNETES_DISK: None
+
 ARGO_WORKFLOWS_KUBERNETES_SECRETS: str
 
 ARGO_WORKFLOWS_ENV_VARS_TO_SKIP: str
 
+KUBERNETES_JOBSET_GROUP: str
+
+KUBERNETES_JOBSET_VERSION: str
+
 ARGO_EVENTS_SERVICE_ACCOUNT: None
 
 ARGO_EVENTS_EVENT_BUS: str
 
 ARGO_EVENTS_EVENT_SOURCE: None
 
 ARGO_EVENTS_EVENT: None
@@ -214,14 +234,16 @@
 
 CONDA_PACKAGE_AZUREROOT: None
 
 CONDA_PACKAGE_GSROOT: None
 
 CONDA_DEPENDENCY_RESOLVER: str
 
+ESCAPE_HATCH_WARNING: bool
+
 DEBUG_OPTIONS: list
 
 DEBUG_SUBCOMMAND: bool
 
 DEBUG_SIDECAR: bool
 
 DEBUG_S3CLIENT: bool
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/metaflow_current.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/metaflow_current.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.023084                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.268101                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow
-    import metaflow.metaflow_current
     import metaflow.plugins.cards.component_serializer
+    import metaflow
     import typing
+    import metaflow.metaflow_current
     import metaflow.events
 
 TYPE_CHECKING: bool
 
 TEMPDIR: str
 
 class Parallel(tuple, metaclass=type):
@@ -238,14 +238,27 @@
         Returns
         -------
         CardComponentCollector
             The or one of the cards attached to this step.
         """
         ...
     @property
+    def trigger(self) -> "metaflow.events.Trigger":
+        """
+        (only in the presence of the @trigger, or @trigger_on_finish decorators)
+        
+        Returns `Trigger` if the current run is triggered by an event
+        
+        Returns
+        -------
+        Trigger
+            `Trigger` if triggered by an event
+        """
+        ...
+    @property
     def project_name(self) -> str:
         """
         (only in the presence of the @project decorator)
         
         The name of the project assigned to this flow, i.e. `X` in `@project(name=X)`.
         
         Returns
@@ -304,24 +317,11 @@
         
         Returns
         -------
         bool
             True if the flow is deployed with `--production`.
         """
         ...
-    @property
-    def trigger(self) -> "metaflow.events.Trigger":
-        """
-        (only in the presence of the @trigger, or @trigger_on_finish decorators)
-        
-        Returns `Trigger` if the current run is triggered by an event
-        
-        Returns
-        -------
-        Trigger
-            `Trigger` if triggered by an event
-        """
-        ...
     ...
 
 current: Current
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/mflog/mflog.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/mflog/mflog.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.966795                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.212074                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import datetime
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/multicore_utils.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/multicore_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.914344                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.157949                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/parameters.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/parameters.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.915738                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.159363                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.parameters
+    import typing
     import metaflow._vendor.click.types
     import metaflow.exception
-    import typing
 
 class ParameterFieldFailed(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, name, field):
         ...
     ...
 
 class ParameterFieldTypeMismatch(metaflow.exception.MetaflowException, metaclass=type):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/__init__.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.927203                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.169745                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.unbounded_foreach
@@ -48,14 +48,18 @@
 
 AWS_CLIENT_PROVIDERS_DESC: list
 
 SENSOR_FLOW_DECORATORS: list
 
 SECRETS_PROVIDERS_DESC: list
 
+GCP_CLIENT_PROVIDERS_DESC: list
+
+AZURE_CLIENT_PROVIDERS_DESC: list
+
 def get_plugin_cli():
     ...
 
 STEP_DECORATORS: list
 
 FLOW_DECORATORS: list
 
@@ -71,14 +75,18 @@
 
 MONITOR_SIDECARS: dict
 
 AWS_CLIENT_PROVIDERS: list
 
 SECRETS_PROVIDERS: list
 
+AZURE_CLIENT_PROVIDERS: list
+
+GCP_CLIENT_PROVIDERS: list
+
 MF_EXTERNAL_CARDS: list
 
 class BlankCard(metaflow.plugins.cards.card_modules.card.MetaflowCard, metaclass=type):
     def __init__(self, options = {"title": ""}, components = [], graph = None):
         ...
     def render(self, task, components = [], runtime = False):
         ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/airflow.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.980715                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.244542                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
-    import metaflow.metaflow_current
     import metaflow._vendor.click.types
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
@@ -38,14 +38,16 @@
 
 AIRFLOW_KUBERNETES_KUBECONFIG_FILE: None
 
 AIRFLOW_KUBERNETES_STARTUP_TIMEOUT_SECONDS: int
 
 AWS_SECRETS_MANAGER_DEFAULT_REGION: None
 
+GCP_SECRET_MANAGER_PREFIX: None
+
 AZURE_STORAGE_BLOB_SERVICE_ENDPOINT: None
 
 CARD_AZUREROOT: None
 
 CARD_GSROOT: None
 
 CARD_S3ROOT: None
@@ -66,14 +68,16 @@
 
 S3_ENDPOINT_URL: None
 
 SERVICE_HEADERS: dict
 
 SERVICE_INTERNAL_URL: None
 
+AZURE_KEY_VAULT_PREFIX: None
+
 class DelayedEvaluationParameter(object, metaclass=type):
     def __init__(self, name, field, fun):
         ...
     def __call__(self, return_str = False):
         ...
     ...
 
@@ -90,15 +94,19 @@
     ...
 
 class Kubernetes(object, metaclass=type):
     def __init__(self, datastore, metadata, environment):
         ...
     def launch_job(self, **kwargs):
         ...
-    def create_job(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, shared_memory = None):
+    def create_jobset(self, job_spec = None, run_id = None, step_name = None, task_id = None, namespace = None, env = None, num_parallel = None, port = None, annotations = None, labels = None):
+        ...
+    def create_job_object(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, shared_memory = None, port = None, name_pattern = None, num_parallel = None):
+        ...
+    def create_k8sjob(self, job):
         ...
     def wait(self, stdout_location, stderr_location, echo = None):
         ...
     ...
 
 def get_run_time_limit_for_task(step_decos):
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow_cli.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/airflow_cli.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.981934                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.245677                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
-    import metaflow.decorators
     import metaflow.exception
+    import metaflow.decorators
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/airflow_decorator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.978279                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.242239                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow_utils.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/airflow_utils.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.977803                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.241793                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 TASK_ID_XCOM_KEY: str
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/exception.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/exception.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.978549                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.242497                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/__init__.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/sensors/__init__.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.978822                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.242766                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.airflow.sensors.base_sensor
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.007423                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.264525                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.007905                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.265007                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.decorators
     import metaflow.plugins.airflow.sensors.base_sensor
     import metaflow.exception
-    import metaflow.decorators
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.008335                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.265418                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.decorators
     import metaflow.plugins.airflow.sensors.base_sensor
     import metaflow.exception
-    import metaflow.decorators
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_client.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/argo/argo_client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.995703                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.225381                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -18,14 +18,16 @@
     ...
 
 class KubernetesClient(object, metaclass=type):
     def __init__(self):
         ...
     def get(self):
         ...
+    def jobset(self, **kwargs):
+        ...
     def job(self, **kwargs):
         ...
     ...
 
 class ArgoClientException(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_events.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/argo/argo_events.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.993898                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.223794                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_workflows.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/argo/argo_workflows.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.001234                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.230567                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.parameters
     import metaflow.exception
-    import metaflow.metaflow_current
+    import metaflow.parameters
     import metaflow._vendor.click.types
+    import metaflow.metaflow_current
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
@@ -71,14 +71,18 @@
 
 DATATOOLS_S3ROOT: None
 
 DEFAULT_METADATA: str
 
 DEFAULT_SECRETS_BACKEND_TYPE: None
 
+GCP_SECRET_MANAGER_PREFIX: None
+
+AZURE_KEY_VAULT_PREFIX: None
+
 KUBERNETES_FETCH_EC2_METADATA: bool
 
 KUBERNETES_LABELS: str
 
 KUBERNETES_NAMESPACE: str
 
 KUBERNETES_NODE_SELECTOR: str
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.003195                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.232377                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.exception
     import metaflow.parameters
-    import metaflow.metaflow_current
     import metaflow.decorators
-    import metaflow.exception
+    import metaflow.metaflow_current
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.994990                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.224685                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.events
+    import metaflow.decorators
     import metaflow
     import metaflow.metaflow_current
-    import metaflow.decorators
-    import metaflow.events
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/aws_client.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/aws_client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.982847                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.213128                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 cached_aws_sandbox_creds: None
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/aws_utils.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/aws_utils.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.982460                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.212721                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/batch/batch.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.011553                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.260758                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch_cli.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/batch/batch_cli.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.013252                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.262341                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -18,14 +18,18 @@
 def sync_local_metadata_from_datastore(metadata_local_dir, task_ds):
     ...
 
 DATASTORE_LOCAL_DIR: str
 
 TASK_LOG_SOURCE: str
 
+UBF_CONTROL: str
+
+UBF_TASK: str
+
 class Batch(object, metaclass=type):
     def __init__(self, metadata, environment):
         ...
     def list_jobs(self, flow_name, run_id, user, echo):
         ...
     def kill_jobs(self, flow_name, run_id, user, echo):
         ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch_client.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/batch/batch_client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.010263                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.259572                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.012478                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.261657                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
-    import metaflow.metaflow_current
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
 
 def get_run_time_limit_for_task(step_decos):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.019609                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.262815                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.013514                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.252692                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 SFN_DYNAMO_DB_TABLE: None
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.014547                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.253964                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class EventBridgeClient(object, metaclass=type):
     def __init__(self, name):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/production_token.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/production_token.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.008766                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.253647                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def new_token(token_prefix, prev_token = None):
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/retry_decorator.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.014205                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.193939                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-class ScheduleDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
+        ...
+    ...
+
+MAX_ATTEMPTS: int
+
+class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+        ...
+    def step_task_retry_count(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.017517                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.256506                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.019097                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.258058                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.exception
     import metaflow.parameters
-    import metaflow.metaflow_current
     import metaflow.decorators
-    import metaflow.exception
+    import metaflow.metaflow_current
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.014929                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.254313                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 AWS_SANDBOX_ENABLED: bool
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.014009                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.253188                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/azure_exceptions.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/azure/azure_exceptions.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.004706                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.250214                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/azure_utils.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/azure/azure_utils.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.005224                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.250690                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -25,14 +25,17 @@
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
+def create_cacheable_azure_credential():
+    ...
+
 def check_azure_deps(func):
     """
     The decorated function checks Azure dependencies (as needed for Azure storage backend). This includes
     various Azure SDK packages, as well as a Python version of >3.6
     
     We also tune some warning and logging configurations to reduce excessive log lines from Azure SDK.
     """
@@ -64,13 +67,10 @@
 
 def handle_exceptions(func):
     """
     This is a decorator leveraging the logic from process_exception()
     """
     ...
 
-def create_cacheable_default_azure_credentials(*args, **kwargs):
-    ...
-
 def create_static_token_credential(*args, **kwargs):
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.005646                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.251187                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
 AZURE_STORAGE_BLOB_SERVICE_ENDPOINT: None
 
-def create_cacheable_default_azure_credentials(*args, **kwargs):
-    ...
-
 def check_azure_deps(func):
     """
     The decorated function checks Azure dependencies (as needed for Azure storage backend). This includes
     various Azure SDK packages, as well as a Python version of >3.6
     
     We also tune some warning and logging configurations to reduce excessive log lines from Azure SDK.
     """
     ...
 
+def create_cacheable_azure_credential():
+    ...
+
 AZURE_CLIENT_CONNECTION_DATA_BLOCK_SIZE: int
 
 AZURE_CLIENT_MAX_SINGLE_GET_SIZE_MB: int
 
 AZURE_CLIENT_MAX_SINGLE_PUT_SIZE_MB: int
 
 AZURE_CLIENT_MAX_CHUNK_GET_SIZE_MB: int
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/includefile_support.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/azure/includefile_support.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.959997                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.204657                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_cli.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.975418                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.240419                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.parameters
+    import datetime
+    import metaflow.client.core
     import typing
     import metaflow.exception
-    import metaflow.client.core
-    import datetime
-    import metaflow.parameters
 
 class Task(metaflow.client.core.MetaflowObject, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     @property
     def metadata(self) -> typing.List[metaflow.client.core.Metadata]:
         """
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_client.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.961948                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.206497                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow
     import metaflow.plugins.cards.card_client
+    import metaflow
     import metaflow.exception
 
 TYPE_CHECKING: bool
 
 CARD_SUFFIX: str
 
 def resolve_paths_from_task(flow_datastore, pathspec = None, type = None, hash = None, card_id = None):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_creator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_creator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.970143                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.235567                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_datastore.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_datastore.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.971977                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.237334                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.971043                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.236407                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class CardComponentCollector(object, metaclass=type):
     def __init__(self, logger = None, card_creator = None):
         ...
     @staticmethod
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/__init__.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.967391                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.232954                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/basic.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/basic.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.955015                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.199459                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.plugins.cards.card_modules.basic
     import metaflow
     import metaflow.plugins.cards.card_modules.card
-    import metaflow.plugins.cards.card_modules.basic
 
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
         Produce custom card contents in HTML.
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/card.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/card.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.962441                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.206968                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.006776                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.263918                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def main(template, data = None, **kwargs):
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.021710                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.266733                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def render(template = "", data = {}, partials_path = ".", partials_ext = "mustache", partials_dict = {}, padding = "", def_ldel = "{{", def_rdel = "}}", scopes = None, warn = False, keep = False):
     """
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.021255                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.266300                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 linesep: str
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.020783                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.265860                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class ChevronError(SyntaxError, metaclass=type):
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/components.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/components.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.964790                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.209125                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
     import metaflow.plugins.cards.card_modules.components
-    import metaflow.plugins.cards.card_modules.card
+    import typing
     import metaflow.plugins.cards.card_modules.basic
+    import metaflow.plugins.cards.card_modules.card
 
 class LogComponent(metaflow.plugins.cards.card_modules.basic.DefaultComponent, metaclass=type):
     def __init__(self, data = None):
         ...
     def render(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.006095                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.252137                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class TypeResolvedObject(tuple, metaclass=type):
     @staticmethod
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/gcp/gs_utils.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.006326                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.249237                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.basic
+    import metaflow.exception
 
-class SerializationErrorComponent(metaflow.plugins.cards.card_modules.basic.ErrorComponent, metaclass=type):
-    def __init__(self, component_name, error_message):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
         ...
+    def __str__(self):
+        ...
+    ...
+
+class MetaflowInternalError(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-def render_safely(func):
+def parse_gs_full_path(gs_uri):
+    ...
+
+def check_gs_deps(func):
     """
-    This is a decorator that can be added to any `MetaflowCardComponent.render`
-    The goal is to render subcomponents safely and ensure that they are JSON serializable.
+    The decorated function checks GS dependencies (as needed for Google Cloud storage backend). This includes
+    various GCP SDK packages, as well as a Python version of >=3.7
     """
     ...
 
+def process_gs_exception(*args, **kwargs):
+    ...
+
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.956478                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.200794                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_resolver.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/card_resolver.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.972610                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.237911                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class CardDatastore(object, metaclass=type):
     @classmethod
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/component_serializer.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/component_serializer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.969836                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.235275                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.components
+    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.card
     import metaflow.exception
-    import metaflow.plugins.cards.card_modules.basic
 
 class MetaflowCardComponent(object, metaclass=type):
     @property
     def component_id(self):
         ...
     @component_id.setter
     def component_id(self, value):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/exception.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/cards/exception.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.968100                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.233622                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/catch_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/catch_decorator.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.950078                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.194767                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
-    import metaflow.decorators
     import metaflow.exception
+    import metaflow.decorators
+    import metaflow.metaflow_current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/__init__.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.948860                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.192524                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.datatools.s3.s3
-    import metaflow.exception
     import io
+    import metaflow.exception
 
 def read_in_chunks(dst, src, src_sz, max_chunk_size):
     ...
 
 class MetaflowLocalNotFound(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/local.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/local.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.959424                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.204117                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/__init__.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/s3/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.985692                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.221883                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.datatools.s3.s3
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/s3.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/s3/s3.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.931185                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.173540                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.datastore.inputs
     import metaflow.plugins.datatools.s3.s3
-    import metaflow.metaflow_current
     import typing
-    import metaflow.exception
+    import metaflow.metaflow_current
     import io
+    import metaflow.exception
 
 TYPE_CHECKING: bool
 
 class FlowSpec(object, metaclass=type):
     def __init__(self, use_cli = True):
         """
         Construct a FlowSpec
@@ -246,14 +246,17 @@
 
 S3_TRANSIENT_RETRY_COUNT: int
 
 S3_SERVER_SIDE_ENCRYPTION: None
 
 TEMPDIR: str
 
+def namedtuple_with_defaults(typename, field_descr, defaults = ()):
+    ...
+
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/s3tail.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/s3/s3tail.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.020024                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.263500                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def aws_retry(f):
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/s3util.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/datatools/s3/s3util.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.958770                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.203387                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/debug_logger.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/debug_logger.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.952171                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.196845                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.event_logger
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/debug_monitor.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/debug_monitor.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.952458                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.197148                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.monitor
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/environment_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/environment_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.945820                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.193392                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/events_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/events_decorator.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.951252                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.195498                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/frameworks/pytorch.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/frameworks/pytorch.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.003673                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.222360                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.decorators
     import metaflow.plugins.parallel_decorator
     import metaflow.metaflow_current
-    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class ParallelDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
     def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/gs_exceptions.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/storage_executor.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.004068                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.196418                                        #
 ##################################################################################
 
 from __future__ import annotations
 
-import typing
-if typing.TYPE_CHECKING:
-    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
+class StorageExecutor(object, metaclass=type):
+    def __init__(self, use_processes = False):
+        ...
+    def warm_up(self):
+        ...
+    def submit(self, *args, **kwargs):
+        ...
+    ...
+
+def handle_executor_exceptions(func):
+    """
+    Decorator for handling errors that come from an Executor. This decorator should
+    only be used on functions where executor errors are possible. I.e. the function
+    uses StorageExecutor.
+    """
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/gs_utils.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/timeout_decorator.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:01.004422                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.191173                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.decorators
     import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class MetaflowInternalError(metaflow.exception.MetaflowException, metaclass=type):
-    ...
+UBF_CONTROL: str
 
-class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
-    ...
+DEFAULT_RUNTIME_LIMIT: int
 
-def parse_gs_full_path(gs_uri):
+class TimeoutException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-def check_gs_deps(func):
-    """
-    The decorated function checks GS dependencies (as needed for Google Cloud storage backend). This includes
-    various GCP SDK packages, as well as a Python version of >=3.7
-    """
+class TimeoutDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def __init__(self, *args, **kwargs):
+        ...
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+        ...
+    def task_pre_step(self, step_name, task_datastore, metadata, run_id, task_id, flow, graph, retry_count, max_user_code_retries, ubf_context, inputs):
+        ...
+    def task_post_step(self, step_name, flow, graph, retry_count, max_user_code_retries):
+        ...
     ...
 
-def process_gs_exception(*args, **kwargs):
+def get_run_time_limit_for_task(step_decos):
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/includefile_support.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/gcp/includefile_support.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.960608                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.205240                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/kubernetes.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.991316                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.217190                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
@@ -48,18 +48,24 @@
 
 DATASTORE_SYSROOT_S3: None
 
 DATATOOLS_S3ROOT: None
 
 DEFAULT_AWS_CLIENT_PROVIDER: str
 
+DEFAULT_GCP_CLIENT_PROVIDER: str
+
 DEFAULT_METADATA: str
 
 DEFAULT_SECRETS_BACKEND_TYPE: None
 
+GCP_SECRET_MANAGER_PREFIX: None
+
+AZURE_KEY_VAULT_PREFIX: None
+
 KUBERNETES_FETCH_EC2_METADATA: bool
 
 KUBERNETES_LABELS: str
 
 KUBERNETES_SANDBOX_INIT_SCRIPT: None
 
 S3_ENDPOINT_URL: None
@@ -75,14 +81,16 @@
 BASH_SAVE_LOGS: str
 
 class KubernetesClient(object, metaclass=type):
     def __init__(self):
         ...
     def get(self):
         ...
+    def jobset(self, **kwargs):
+        ...
     def job(self, **kwargs):
         ...
     ...
 
 LOGS_DIR: str
 
 STDOUT_FILE: str
@@ -100,15 +108,19 @@
     ...
 
 class Kubernetes(object, metaclass=type):
     def __init__(self, datastore, metadata, environment):
         ...
     def launch_job(self, **kwargs):
         ...
-    def create_job(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, shared_memory = None):
+    def create_jobset(self, job_spec = None, run_id = None, step_name = None, task_id = None, namespace = None, env = None, num_parallel = None, port = None, annotations = None, labels = None):
+        ...
+    def create_job_object(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, shared_memory = None, port = None, name_pattern = None, num_parallel = None):
+        ...
+    def create_k8sjob(self, job):
         ...
     def wait(self, stdout_location, stderr_location, echo = None):
         ...
     ...
 
 def validate_kube_labels(labels: typing.Optional[typing.Dict[str, typing.Optional[str]]]) -> bool:
     """
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.993416                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.219362                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.decorators
     import metaflow._vendor.click.types
+    import metaflow.exception
 
 class JSONTypeClass(metaflow._vendor.click.types.ParamType, metaclass=type):
     def convert(self, value, param, ctx):
         ...
     def __str__(self):
         ...
     def __repr__(self):
@@ -25,37 +25,48 @@
 
 class CommandException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 def sync_local_metadata_from_datastore(metadata_local_dir, task_ds):
     ...
 
+UBF_CONTROL: str
+
+UBF_TASK: str
+
 DATASTORE_LOCAL_DIR: str
 
 KUBERNETES_LABELS: str
 
 TASK_LOG_SOURCE: str
 
 class Kubernetes(object, metaclass=type):
     def __init__(self, datastore, metadata, environment):
         ...
     def launch_job(self, **kwargs):
         ...
-    def create_job(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, shared_memory = None):
+    def create_jobset(self, job_spec = None, run_id = None, step_name = None, task_id = None, namespace = None, env = None, num_parallel = None, port = None, annotations = None, labels = None):
+        ...
+    def create_job_object(self, flow_name, run_id, step_name, task_id, attempt, user, code_package_sha, code_package_url, code_package_ds, step_cli, docker_image, docker_image_pull_policy, service_account = None, secrets = None, node_selector = None, namespace = None, cpu = None, gpu = None, gpu_vendor = None, disk = None, memory = None, use_tmpfs = None, tmpfs_tempdir = None, tmpfs_size = None, tmpfs_path = None, run_time_limit = None, env = None, persistent_volume_claims = None, tolerations = None, labels = None, shared_memory = None, port = None, name_pattern = None, num_parallel = None):
+        ...
+    def create_k8sjob(self, job):
         ...
     def wait(self, stdout_location, stderr_location, echo = None):
         ...
     ...
 
 class KubernetesKilledException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 def parse_kube_keyvalue_list(items: typing.List[str], requires_both: bool = True):
     ...
 
+class KubernetesException(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
 class KubernetesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
     def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
         ...
     def package_init(self, flow, step_name, environment):
         ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.990192                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.215962                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -16,14 +16,16 @@
     def __str__(self):
         ...
     ...
 
 class KubernetesJob(object, metaclass=type):
     def __init__(self, client, **kwargs):
         ...
+    def create_job_spec(self):
+        ...
     def create(self):
         ...
     def execute(self):
         ...
     def step_name(self, step_name):
         ...
     def namespace(self, namespace):
@@ -42,21 +44,30 @@
         ...
     def label(self, name, value):
         ...
     def annotation(self, name, value):
         ...
     ...
 
+class KubernetesJobSet(object, metaclass=type):
+    def __init__(self, client, name = None, job_spec = None, namespace = None, num_parallel = None, annotations = None, labels = None, port = None, task_id = None, **kwargs):
+        ...
+    def execute(self):
+        ...
+    ...
+
 CLIENT_REFRESH_INTERVAL_SECONDS: int
 
 class KubernetesClientException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 class KubernetesClient(object, metaclass=type):
     def __init__(self):
         ...
     def get(self):
         ...
+    def jobset(self, **kwargs):
+        ...
     def job(self, **kwargs):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.992398                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.218344                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
-    import metaflow.metaflow_current
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
@@ -63,14 +63,22 @@
 
 KUBERNETES_TOLERATIONS: str
 
 KUBERNETES_SERVICE_ACCOUNT: None
 
 KUBERNETES_SHARED_MEMORY: None
 
+KUBERNETES_PORT: None
+
+KUBERNETES_CPU: None
+
+KUBERNETES_MEMORY: None
+
+KUBERNETES_DISK: None
+
 class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
 
 def get_run_time_limit_for_task(step_decos):
     ...
 
 def get_docker_registry(image_uri):
@@ -132,14 +140,33 @@
 
 class KubernetesException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 def parse_kube_keyvalue_list(items: typing.List[str], requires_both: bool = True):
     ...
 
+UBF_CONTROL: str
+
+class TaskIdConstructor(object, metaclass=type):
+    @classmethod
+    def jobset_worker_id(cls, control_task_id: str):
+        ...
+    @classmethod
+    def join_step_task_ids(cls, num_parallel):
+        """
+        Called within the step decorator to set the `flow._control_mapper_tasks`.
+        Setting these allows the flow to know which tasks are needed in the join step.
+        We set this in the `task_pre_step` method of the decorator.
+        """
+        ...
+    @classmethod
+    def argo(cls):
+        ...
+    ...
+
 class KubernetesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
     def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
         ...
     def package_init(self, flow, step_name, environment):
         ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.989578                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.215253                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -15,25 +15,38 @@
         ...
     def __str__(self):
         ...
     ...
 
 KUBERNETES_SECRETS: str
 
+UBF_CONTROL: str
+
+UBF_TASK: str
+
 CLIENT_REFRESH_INTERVAL_SECONDS: int
 
+class KubernetesJobSet(object, metaclass=type):
+    def __init__(self, client, name = None, job_spec = None, namespace = None, num_parallel = None, annotations = None, labels = None, port = None, task_id = None, **kwargs):
+        ...
+    def execute(self):
+        ...
+    ...
+
 class KubernetesJobException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 def k8s_retry(deadline_seconds = 60, max_backoff = 32):
     ...
 
 class KubernetesJob(object, metaclass=type):
     def __init__(self, client, **kwargs):
         ...
+    def create_job_spec(self):
+        ...
     def create(self):
         ...
     def execute(self):
         ...
     def step_name(self, step_name):
         ...
     def namespace(self, namespace):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/parallel_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/parallel_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.946493                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.193091                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/project_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/project_decorator.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.950856                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.195874                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/__init__.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.949148                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.195125                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/conda_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/conda_decorator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.986763                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.246614                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/conda_environment.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/conda_environment.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.988133                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.247898                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_environment
+    import io
     import abc
+    import metaflow.metaflow_environment
     import metaflow.exception
-    import io
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/pypi_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/pypi_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.986033                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.245964                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/pypi_environment.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/pypi_environment.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.988664                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.248354                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_environment
     import metaflow.plugins.pypi.conda_environment
+    import metaflow.metaflow_environment
 
 class CondaEnvironment(metaflow.metaflow_environment.MetaflowEnvironment, metaclass=type):
     def __init__(self, flow):
         ...
     def set_local_root(self, local_root):
         ...
     def decospecs(self):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/utils.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/pypi/utils.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.987137                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.246975                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/resources_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/resources_decorator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.946635                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.190614                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/__init__.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.946073                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.223346                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
+    import metaflow.plugins.secrets
 
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
         """
         ...
     ...
 
+class InlineSecretsProvider(metaflow.plugins.secrets.SecretsProvider, metaclass=abc.ABCMeta):
+    def get_secret_as_dict(self, secret_id, options = {}, role = None):
+        """
+        Intended to be used for testing purposes only.
+        """
+        ...
+    ...
+
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/secrets_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/secrets/secrets_decorator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.976213                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.223072                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/storage_executor.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/logs_cli.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.951779                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.201514                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
+if typing.TYPE_CHECKING:
+    import metaflow._vendor.click.core
+    import metaflow.plugins.logs_cli
+    import metaflow.exception
 
-class MetaflowException(Exception, metaclass=type):
-    def __init__(self, msg = "", lineno = None):
+LOGGER_TIMESTAMP: str
+
+class CommandException(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+LOG_SOURCES: list
+
+class CustomGroup(metaflow._vendor.click.core.Group, metaclass=type):
+    def __init__(self, name = None, commands = None, default_cmd = None, **attrs):
         ...
-    def __str__(self):
+    def get_command(self, ctx, cmd_name):
+        ...
+    def parse_args(self, ctx, args):
+        ...
+    def resolve_command(self, ctx, args):
+        ...
+    def format_commands(self, ctx, formatter):
         ...
     ...
 
-class StorageExecutor(object, metaclass=type):
-    def __init__(self, use_processes = False):
+class CustomFormatter(object, metaclass=type):
+    def __init__(self, default_cmd, original_formatter):
         ...
-    def warm_up(self):
+    def __getattr__(self, name):
         ...
-    def submit(self, *args, **kwargs):
+    def write_dl(self, rows):
         ...
     ...
 
-def handle_executor_exceptions(func):
-    """
-    Decorator for handling errors that come from an Executor. This decorator should
-    only be used on functions where executor errors are possible. I.e. the function
-    uses StorageExecutor.
-    """
-    ...
+logs: CustomGroup
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/tag_cli.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/tag_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.958278                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.202907                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import datetime
+    import metaflow.client.core
     import metaflow.metaflow_current
-    import metaflow.exception
     import metaflow.events
-    import metaflow.client.core
-    import datetime
+    import metaflow.exception
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.945489                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.190336                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.unbounded_foreach
     import metaflow.decorators
+    import metaflow.unbounded_foreach
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/procpoll.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/procpoll.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.941266                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.187038                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.procpoll
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/pylint_wrapper.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/pylint_wrapper.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.941612                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.186570                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow-stubs/tagging_util.pyi` & `metaflow_stubs-2.12.0/metaflow-stubs/tagging_util.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.9                                                             #
-# Generated on 2024-03-29T22:28:00.916120                                        #
+# MF version: 2.12.0                                                             #
+# Generated on 2024-05-28T09:55:27.159730                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.9/metaflow_stubs.egg-info/PKG-INFO` & `metaflow_stubs-2.12.0/metaflow_stubs.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-stubs
-Version: 2.11.9
+Version: 2.12.0
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Requires-Dist: metaflow==2.11.9
+Requires-Dist: metaflow==2.12.0
 
 # Metaflow Stubs
 
 This package contains stub files for `metaflow` and thus offers type hints for various editors (such as `VSCode`) and language servers (such as `Pylance`).
 
 ## Installation
```

### Comparing `metaflow-stubs-2.11.9/metaflow_stubs.egg-info/SOURCES.txt` & `metaflow_stubs-2.12.0/metaflow_stubs.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 metaflow-stubs/metaflow_current.pyi
 metaflow-stubs/multicore_utils.pyi
 metaflow-stubs/parameters.pyi
 metaflow-stubs/procpoll.pyi
 metaflow-stubs/py.typed
 metaflow-stubs/pylint_wrapper.pyi
 metaflow-stubs/tagging_util.pyi
+metaflow-stubs/tuple_util.pyi
 metaflow-stubs/version.pyi
 metaflow-stubs/client/__init__.pyi
 metaflow-stubs/client/core.pyi
 metaflow-stubs/client/filecache.pyi
 metaflow-stubs/metadata/metadata.pyi
 metaflow-stubs/metadata/util.pyi
 metaflow-stubs/mflog/mflog.pyi
 metaflow-stubs/plugins/__init__.pyi
 metaflow-stubs/plugins/catch_decorator.pyi
 metaflow-stubs/plugins/debug_logger.pyi
 metaflow-stubs/plugins/debug_monitor.pyi
 metaflow-stubs/plugins/environment_decorator.pyi
 metaflow-stubs/plugins/events_decorator.pyi
+metaflow-stubs/plugins/logs_cli.pyi
 metaflow-stubs/plugins/package_cli.pyi
 metaflow-stubs/plugins/parallel_decorator.pyi
 metaflow-stubs/plugins/project_decorator.pyi
 metaflow-stubs/plugins/resources_decorator.pyi
 metaflow-stubs/plugins/retry_decorator.pyi
 metaflow-stubs/plugins/storage_executor.pyi
 metaflow-stubs/plugins/tag_cli.pyi
@@ -73,15 +75,17 @@
 metaflow-stubs/plugins/aws/step_functions/production_token.pyi
 metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
 metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
 metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
 metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
 metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
 metaflow-stubs/plugins/azure/__init__.pyi
+metaflow-stubs/plugins/azure/azure_credential.pyi
 metaflow-stubs/plugins/azure/azure_exceptions.pyi
+metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi
 metaflow-stubs/plugins/azure/azure_utils.pyi
 metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
 metaflow-stubs/plugins/azure/includefile_support.pyi
 metaflow-stubs/plugins/cards/__init__.pyi
 metaflow-stubs/plugins/cards/card_cli.pyi
 metaflow-stubs/plugins/cards/card_client.pyi
 metaflow-stubs/plugins/cards/card_creator.pyi
@@ -107,31 +111,37 @@
 metaflow-stubs/plugins/datatools/s3/__init__.pyi
 metaflow-stubs/plugins/datatools/s3/s3.pyi
 metaflow-stubs/plugins/datatools/s3/s3tail.pyi
 metaflow-stubs/plugins/datatools/s3/s3util.pyi
 metaflow-stubs/plugins/frameworks/__init__.pyi
 metaflow-stubs/plugins/frameworks/pytorch.pyi
 metaflow-stubs/plugins/gcp/__init__.pyi
+metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
 metaflow-stubs/plugins/gcp/gs_exceptions.pyi
 metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
 metaflow-stubs/plugins/gcp/gs_utils.pyi
 metaflow-stubs/plugins/gcp/includefile_support.pyi
 metaflow-stubs/plugins/kubernetes/__init__.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
 metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi
+metaflow-stubs/plugins/kubernetes/kubernetes_jobsets.pyi
 metaflow-stubs/plugins/pypi/__init__.pyi
 metaflow-stubs/plugins/pypi/conda_decorator.pyi
 metaflow-stubs/plugins/pypi/conda_environment.pyi
 metaflow-stubs/plugins/pypi/pypi_decorator.pyi
 metaflow-stubs/plugins/pypi/pypi_environment.pyi
 metaflow-stubs/plugins/pypi/utils.pyi
 metaflow-stubs/plugins/secrets/__init__.pyi
 metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
 metaflow-stubs/plugins/secrets/secrets_decorator.pyi
+metaflow-stubs/runner/__init__.pyi
+metaflow-stubs/runner/metaflow_runner.pyi
+metaflow-stubs/runner/nbrun.pyi
+metaflow-stubs/runner/subprocess_manager.pyi
 metaflow_stubs.egg-info/PKG-INFO
 metaflow_stubs.egg-info/SOURCES.txt
 metaflow_stubs.egg-info/dependency_links.txt
 metaflow_stubs.egg-info/requires.txt
 metaflow_stubs.egg-info/top_level.txt
```

### Comparing `metaflow-stubs-2.11.9/setup.py` & `metaflow_stubs-2.12.0/setup.py`

 * *Files identical despite different names*

