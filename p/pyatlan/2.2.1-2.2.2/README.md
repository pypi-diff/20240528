# Comparing `tmp/pyatlan-2.2.1.tar.gz` & `tmp/pyatlan-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-2.2.1.tar", last modified: Tue May 21 13:09:02 2024, max compression
+gzip compressed data, was "pyatlan-2.2.2.tar", last modified: Tue May 28 11:27:28 2024, max compression
```

## Comparing `pyatlan-2.2.1.tar` & `pyatlan-2.2.2.tar`

### file list

```diff
@@ -1,503 +1,512 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.530149 pyatlan-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-21 13:08:58.000000 pyatlan-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 13:08:58.000000 pyatlan-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-21 13:08:58.000000 pyatlan-2.2.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-21 13:09:02.530149 pyatlan-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-21 13:08:58.000000 pyatlan-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.442149 pyatlan-2.2.1/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.446149 pyatlan-2.2.1/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/atlan_tag_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.450149 pyatlan-2.2.1/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    79101 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    59409 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/impersonate.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/search_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/typedef.py
--rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/client/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    33221 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.450149 pyatlan-2.2.1/pyatlan/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/events/atlan_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/events/atlan_lambda_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.450149 pyatlan-2.2.1/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32321 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/class_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/create_typedefs_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.450149 pyatlan-2.2.1/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/enums.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/globals.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/imports.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/init.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/macros.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/module.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/properties.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/referenceable_attributes.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/referenceable_methods.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/generator/templates/structs.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.458149 pyatlan-2.2.1/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/api_tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.506149 pyatlan-2.2.1/pyatlan/model/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    24476 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s.py
--rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    19153 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_p_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_p_i_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_p_i_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/a_w_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/airflow_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/airflow_task.py
--rw-r--r--   0 runner    (1001) docker     (127)   124326 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/atlas_glossary.py
--rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/atlas_glossary_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    21651 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/atlas_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/auth_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/azure_event_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/azure_event_hub_consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/azure_service_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/azure_service_bus_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/azure_service_bus_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/b_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/b_i_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/badge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/calculation_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite3_d_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognite_time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cognos_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    51792 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/column_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    25611 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cosmos_mongo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cosmos_mongo_d_b_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21623 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cosmos_mongo_d_b_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cube_dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cube_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/cube_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    18464 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_product.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_studio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13068 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/data_studio_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt.py
--rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_column_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_model_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    19524 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dbt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/domo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/domo_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/domo_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/domo_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/domo_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    29820 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    32513 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/dynamo_dbtable.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/event_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/g_c_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/g_c_s_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/g_c_s_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/google.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/insight.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/kafka_consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_look.py
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/looker_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/m_c_incident.py
--rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/m_c_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/materialised_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/matillion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/matillion_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/matillion_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/matillion_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/matillion_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/metabase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/metabase_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/metabase_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/metabase_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_dossier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_fact.py
--rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mode_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mode_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mode_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mode_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mode_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mongo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)    37085 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mongo_d_b_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/mongo_d_b_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/multi_dimensional_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/no_s_q_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/persona.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/power_b_i_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/preset_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11171 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/preset_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/preset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/preset_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/process.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/process_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik_space.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/qlik_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_analysis_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dashboard_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dataset_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/quick_sight_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/readme_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/redash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/redash_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/redash_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/redash_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/referenceable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/s3_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/s3_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/s_q_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/saa_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/salesforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/salesforce_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/salesforce_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/salesforce_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/salesforce_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/salesforce_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/schema_registry_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma_data_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma_data_element_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sigma_workbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sisense.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sisense_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sisense_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sisense_datamodel_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sisense_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/sisense_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/snowflake_dynamic_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/snowflake_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/snowflake_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/snowflake_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/soda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/soda_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/spark_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/stakeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/stakeholder_title.py
--rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/table_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau.py
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_calculated_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_datasource_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_workbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tableau_worksheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/tag_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_dashlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_liveboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_worksheet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/assets/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    77838 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.506149 pyatlan-2.2.1/pyatlan/model/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67647 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/fields/atlan_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/fluent_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/fluent_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/keycloak_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/lineage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.510149 pyatlan-2.2.1/pyatlan/model/packages/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.510149 pyatlan-2.2.1/pyatlan/model/packages/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/base/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/base/miner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/base/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/big_query_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/confluent_kafka_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/dbt_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/dynamo_d_b_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/glue_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/postgres_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/powerbi_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/s_q_l_server_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/sigma_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/snowflake_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/snowflake_miner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/sql_server_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/packages/tableau_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    66000 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/search_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    43068 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/model/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/multipart_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.510149 pyatlan-2.2.1/pyatlan/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/create_package_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.510149 pyatlan-2.2.1/pyatlan/pkg/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/templates/default_configmap.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/templates/default_template.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/templates/package_config.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33619 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/pkg/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 13:08:58.000000 pyatlan-2.2.1/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.530149 pyatlan-2.2.1/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-21 13:09:02.000000 pyatlan-2.2.1/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-05-21 13:09:02.000000 pyatlan-2.2.1/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:09:02.000000 pyatlan-2.2.1/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:09:02.000000 pyatlan-2.2.1/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-21 13:09:02.000000 pyatlan-2.2.1/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 13:09:02.000000 pyatlan-2.2.1/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-21 13:08:58.000000 pyatlan-2.2.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-21 13:08:58.000000 pyatlan-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:09:02.530149 pyatlan-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-21 13:08:58.000000 pyatlan-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.510149 pyatlan-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.518149 pyatlan-2.2.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/adls_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/airflow_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/api_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/atlan_tag_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    39630 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/custom_package_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/data_mesh_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/data_studio_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/gcs_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    31905 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26912 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/owner_propagator_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/persona_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/preset_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/purpose_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/requests_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_file_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_sql_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_sso_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_task_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/test_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/integration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.522149 pyatlan-2.2.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    26291 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.526149 pyatlan-2.2.1/tests/unit/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/a_d_l_s_account_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/a_d_l_s_container_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/a_d_l_s_object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/a_p_i_path_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/a_p_i_spec_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/airflow_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/airflow_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/badge_condition_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/badge_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/column_process_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/column_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/data_domain_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/data_product_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/data_studio_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/database_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.526149 pyatlan-2.2.1/tests/unit/model/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/fields/atlan_fields_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/gcs_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/gcs_object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/glossary_category_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/glossary_term_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/materialised_view_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/preset_chart_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/preset_dashboard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/preset_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/preset_workspace_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/process_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/readme_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/s3_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/s3object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/table_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/model/view_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:09:02.530149 pyatlan-2.2.1/tests/unit/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/pkg/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/pkg/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/pkg/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/pkg/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    53584 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/pkg/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_atlan_tag_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    69612 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_credential_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    18206 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_file_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (127)    36843 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)    33878 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21011 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_query_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_sso_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_task_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15955 2024-05-21 13:08:58.000000 pyatlan-2.2.1/tests/unit/test_workflow_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.238353 pyatlan-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-28 11:27:23.000000 pyatlan-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-28 11:27:23.000000 pyatlan-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 11:27:23.000000 pyatlan-2.2.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-28 11:27:28.238353 pyatlan-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-28 11:27:23.000000 pyatlan-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.150352 pyatlan-2.2.2/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.154352 pyatlan-2.2.2/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/cache/atlan_tag_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.158352 pyatlan-2.2.2/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79101 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59409 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/impersonate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/search_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23644 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/client/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33221 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.158352 pyatlan-2.2.2/pyatlan/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/events/atlan_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/events/atlan_lambda_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.158352 pyatlan-2.2.2/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32321 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/class_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/create_typedefs_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.162352 pyatlan-2.2.2/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/templates/enums.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/templates/globals.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/templates/imports.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/templates/init.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/templates/macros.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/templates/module.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/templates/properties.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/templates/referenceable_attributes.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/templates/referenceable_methods.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/generator/templates/structs.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.166352 pyatlan-2.2.2/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/api_tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.214352 pyatlan-2.2.2/pyatlan/model/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    24720 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/a_d_l_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/a_d_l_s_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/a_d_l_s_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19153 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/a_d_l_s_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/a_p_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/a_p_i_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/a_p_i_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/a_w_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/airflow_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/airflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124326 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/atlas_glossary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/atlas_glossary_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21651 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/atlas_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/auth_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/azure_event_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/azure_event_hub_consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/azure_service_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/azure_service_bus_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/azure_service_bus_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/b_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/b_i_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/calculation_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognite3_d_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognite_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognite_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognite_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognite_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognite_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognos_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognos_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognos_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognos_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognos_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognos_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognos_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cognos_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51792 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/column_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25611 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cosmos_mongo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cosmos_mongo_d_b_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21623 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cosmos_mongo_d_b_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cube_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cube_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/cube_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/data_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18464 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/data_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/data_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/data_studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13068 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/data_studio_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dbt_column_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dbt_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dbt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dbt_model_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19524 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dbt_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dbt_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dbt_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dbt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/domo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/domo_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/domo_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/domo_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/domo_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dynamo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29820 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dynamo_d_b_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32513 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/dynamo_dbtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/event_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/g_c_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/g_c_s_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/g_c_s_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/insight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/kafka_consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/looker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/looker_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/looker_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/looker_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/looker_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/looker_look.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/looker_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/looker_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/looker_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/looker_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/looker_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/m_c_incident.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/m_c_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/materialised_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/matillion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/matillion_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/matillion_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/matillion_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/matillion_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/metabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/metabase_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/metabase_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/metabase_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/micro_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_dossier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_fact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/mode_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/mode_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/mode_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/mode_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/mode_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/mongo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37085 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/mongo_d_b_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/mongo_d_b_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/multi_dimensional_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/no_s_q_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/persona.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/power_b_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/power_b_i_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/power_b_i_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/power_b_i_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/power_b_i_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/power_b_i_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/power_b_i_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/power_b_i_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/power_b_i_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/power_b_i_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/power_b_i_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/power_b_i_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/preset_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11171 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/preset_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/preset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/preset_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/process_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/qlik.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/qlik_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/qlik_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/qlik_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/qlik_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/qlik_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/qlik_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/quick_sight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/quick_sight_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/quick_sight_analysis_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/quick_sight_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/quick_sight_dashboard_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/quick_sight_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/quick_sight_dataset_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/quick_sight_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/readme_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/redash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/redash_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/redash_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/redash_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/referenceable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/s3_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/s3_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/s_q_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/saa_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/salesforce_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/salesforce_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/salesforce_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/salesforce_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/salesforce_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/schema_registry_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sigma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sigma_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sigma_data_element_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sigma_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sigma_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sigma_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sigma_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sisense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sisense_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sisense_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sisense_datamodel_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sisense_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/sisense_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/snowflake_dynamic_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/snowflake_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/snowflake_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/snowflake_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/soda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/soda_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/spark_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/stakeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/stakeholder_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/table_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tableau.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tableau_calculated_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tableau_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tableau_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tableau_datasource_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tableau_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tableau_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tableau_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tableau_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tableau_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tableau_worksheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/tag_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/thoughtspot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_dashlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_liveboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_worksheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/assets/workflow_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78564 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.214352 pyatlan-2.2.2/pyatlan/model/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67647 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/fields/atlan_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/fluent_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/fluent_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/keycloak_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/lineage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.218353 pyatlan-2.2.2/pyatlan/model/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.218353 pyatlan-2.2.2/pyatlan/model/packages/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/base/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/base/miner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/base/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/big_query_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/confluent_kafka_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/dbt_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/dynamo_d_b_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/glue_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/postgres_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/powerbi_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/s_q_l_server_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/sigma_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/snowflake_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/snowflake_miner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/sql_server_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/packages/tableau_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66333 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/search_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43068 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/model/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/multipart_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.218353 pyatlan-2.2.2/pyatlan/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/pkg/create_package_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/pkg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.218353 pyatlan-2.2.2/pyatlan/pkg/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/pkg/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/pkg/templates/default_configmap.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/pkg/templates/default_template.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/pkg/templates/package_config.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/pkg/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/pkg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33619 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/pkg/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 11:27:23.000000 pyatlan-2.2.2/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.238353 pyatlan-2.2.2/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-28 11:27:28.000000 pyatlan-2.2.2/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17350 2024-05-28 11:27:28.000000 pyatlan-2.2.2/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:27:28.000000 pyatlan-2.2.2/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:27:27.000000 pyatlan-2.2.2/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-28 11:27:28.000000 pyatlan-2.2.2/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 11:27:28.000000 pyatlan-2.2.2/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-28 11:27:23.000000 pyatlan-2.2.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-28 11:27:23.000000 pyatlan-2.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:27:28.238353 pyatlan-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-28 11:27:23.000000 pyatlan-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.218353 pyatlan-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.226353 pyatlan-2.2.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/adls_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/airflow_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/api_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/atlan_tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/azure_event_hub_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39630 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/custom_package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/data_mesh_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/data_studio_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/gcs_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31905 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/kafka_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26912 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/owner_propagator_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/persona_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/preset_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/purpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/requests_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30345 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/test_file_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/test_sql_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/test_sso_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/test_task_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/test_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/integration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.230352 pyatlan-2.2.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27534 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.234353 pyatlan-2.2.2/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/a_d_l_s_account_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/a_d_l_s_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/a_d_l_s_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/a_p_i_path_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/a_p_i_spec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/airflow_dag_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/airflow_task_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/azure_event_consumer_group_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/azure_event_hub_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/badge_condition_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/badge_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/column_process_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/column_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/data_domain_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/data_product_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/data_studio_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/database_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.234353 pyatlan-2.2.2/tests/unit/model/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/fields/atlan_fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/gcs_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/gcs_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/glossary_category_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/glossary_term_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/kafka_consumer_group_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/kafka_topic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/materialised_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/preset_chart_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/preset_dashboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/preset_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/preset_workspace_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/readme_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/s3_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/s3object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/model/view_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:28.238353 pyatlan-2.2.2/tests/unit/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/pkg/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/pkg/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/pkg/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/pkg/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53584 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/pkg/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_atlan_tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69612 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_credential_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18206 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_file_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36843 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33878 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21011 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_query_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_sso_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_task_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-05-28 11:27:23.000000 pyatlan-2.2.2/tests/unit/test_workflow_client.py
```

### Comparing `pyatlan-2.2.1/LICENSE` & `pyatlan-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/PKG-INFO` & `pyatlan-2.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 2.2.1
+Version: 2.2.2
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: requests>=2.24
-Requires-Dist: pydantic~=2.6.1
+Requires-Dist: pydantic<3.0.0,>=2.0.0
 Requires-Dist: jinja2==3.1.4
 Requires-Dist: networkx>=3.1
 Requires-Dist: tenacity==8.2.3
 
 <!-- SPDX-License-Identifier: CC-BY-4.0 -->
 <!-- Copyright 2022 Atlan Pte. Ltd. -->
```

### Comparing `pyatlan-2.2.1/README.md` & `pyatlan-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/cache/atlan_tag_cache.py` & `pyatlan-2.2.2/pyatlan/cache/atlan_tag_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-2.2.2/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/cache/enum_cache.py` & `pyatlan-2.2.2/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/cache/group_cache.py` & `pyatlan-2.2.2/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/cache/role_cache.py` & `pyatlan-2.2.2/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/cache/user_cache.py` & `pyatlan-2.2.2/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/admin.py` & `pyatlan-2.2.2/pyatlan/client/admin.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/asset.py` & `pyatlan-2.2.2/pyatlan/client/asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/atlan.py` & `pyatlan-2.2.2/pyatlan/client/atlan.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/audit.py` & `pyatlan-2.2.2/pyatlan/client/audit.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/common.py` & `pyatlan-2.2.2/pyatlan/client/common.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/constants.py` & `pyatlan-2.2.2/pyatlan/client/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -390,24 +390,49 @@
 LIMIT = "limit"
 OFFSET = "offset"
 
 INDEX_API = "search/indexsearch"
 INDEX_SEARCH = API(INDEX_API, HTTPMethod.POST, HTTPStatus.OK, endpoint=EndPoint.ATLAS)
 WORKFLOW_INDEX_API = "workflows/indexsearch"
 WORKFLOW_INDEX_RUN_API = "runs/indexsearch"
+SCHEDULE_QUERY_WORKFLOWS_SEARCH_API = "runs/cron/scheduleQueriesBetweenDuration"
+SCHEDULE_QUERY_WORKFLOWS_MISSED_API = "runs/cron/missedScheduleQueriesBetweenDuration"
+
+SCHEDULE_QUERY_WORKFLOWS_SEARCH = API(
+    SCHEDULE_QUERY_WORKFLOWS_SEARCH_API,
+    HTTPMethod.GET,
+    HTTPStatus.OK,
+    endpoint=EndPoint.HERACLES,
+)
+
+SCHEDULE_QUERY_WORKFLOWS_MISSED = API(
+    SCHEDULE_QUERY_WORKFLOWS_MISSED_API,
+    HTTPMethod.GET,
+    HTTPStatus.OK,
+    endpoint=EndPoint.HERACLES,
+)
+
 WORKFLOW_INDEX_SEARCH = API(
     WORKFLOW_INDEX_API, HTTPMethod.POST, HTTPStatus.OK, endpoint=EndPoint.HERACLES
 )
 WORKFLOW_INDEX_RUN_SEARCH = API(
     WORKFLOW_INDEX_RUN_API, HTTPMethod.POST, HTTPStatus.OK, endpoint=EndPoint.HERACLES
 )
+# triggers a workflow using the current user's credentials
 WORKFLOW_RERUN_API = "workflows/submit"
 WORKFLOW_RERUN = API(
     WORKFLOW_RERUN_API, HTTPMethod.POST, HTTPStatus.OK, endpoint=EndPoint.HERACLES
 )
+
+# triggers a workflow using the workflow owner's credentials
+WORKFLOW_OWNER_RERUN_API = "workflows/triggerAsOwner"
+WORKFLOW_OWNER_RERUN = API(
+    WORKFLOW_OWNER_RERUN_API, HTTPMethod.POST, HTTPStatus.OK, endpoint=EndPoint.HERACLES
+)
+
 WORKFLOW_RUN_API = "workflows?submit=true"
 WORKFLOW_RUN = API(
     WORKFLOW_RUN_API, HTTPMethod.POST, HTTPStatus.OK, endpoint=EndPoint.HERACLES
 )
 WORKFLOW_API = "workflows"
 WORKFLOW_UPDATE = API(
     WORKFLOW_API + "/{workflow_name}",
@@ -436,14 +461,22 @@
 )
 STOP_WORKFLOW_RUN = API(
     WORKFLOW_SCHEDULE_RUN + "/{workflow_run_id}/stop",
     HTTPMethod.POST,
     HTTPStatus.OK,
     endpoint=EndPoint.HERACLES,
 )
+
+WORKFLOW_CHANGE_OWNER = API(
+    WORKFLOW_API + "/{workflow_name}" + "/changeownership",
+    HTTPMethod.POST,
+    HTTPStatus.OK,
+    endpoint=EndPoint.HERACLES,
+)
+
 CREDENTIALS_API = "credentials"
 TEST_CREDENTIAL_API = CREDENTIALS_API + "/test"
 TEST_CREDENTIAL = API(
     TEST_CREDENTIAL_API,
     HTTPMethod.POST,
     HTTPStatus.OK,
     endpoint=EndPoint.HERACLES,
```

### Comparing `pyatlan-2.2.1/pyatlan/client/credential.py` & `pyatlan-2.2.2/pyatlan/client/credential.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/file.py` & `pyatlan-2.2.2/pyatlan/client/file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/group.py` & `pyatlan-2.2.2/pyatlan/client/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/impersonate.py` & `pyatlan-2.2.2/pyatlan/client/impersonate.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/query.py` & `pyatlan-2.2.2/pyatlan/client/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/role.py` & `pyatlan-2.2.2/pyatlan/client/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/search_log.py` & `pyatlan-2.2.2/pyatlan/client/search_log.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/sso.py` & `pyatlan-2.2.2/pyatlan/client/sso.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/task.py` & `pyatlan-2.2.2/pyatlan/client/task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/token.py` & `pyatlan-2.2.2/pyatlan/client/token.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/typedef.py` & `pyatlan-2.2.2/pyatlan/client/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/user.py` & `pyatlan-2.2.2/pyatlan/client/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/client/workflow.py` & `pyatlan-2.2.2/pyatlan/client/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,32 @@
 
 from pydantic.v1 import ValidationError, parse_obj_as, validate_arguments
 
 from pyatlan.client.common import ApiCaller
 from pyatlan.client.constants import (
     GET_ALL_SCHEDULE_RUNS,
     GET_SCHEDULE_RUN,
+    SCHEDULE_QUERY_WORKFLOWS_MISSED,
+    SCHEDULE_QUERY_WORKFLOWS_SEARCH,
     STOP_WORKFLOW_RUN,
     WORKFLOW_ARCHIVE,
+    WORKFLOW_CHANGE_OWNER,
     WORKFLOW_INDEX_RUN_SEARCH,
     WORKFLOW_INDEX_SEARCH,
+    WORKFLOW_OWNER_RERUN,
     WORKFLOW_RERUN,
     WORKFLOW_RUN,
     WORKFLOW_UPDATE,
 )
 from pyatlan.errors import ErrorCode
 from pyatlan.model.enums import AtlanWorkflowPhase, WorkflowPackage
 from pyatlan.model.search import Bool, NestedQuery, Prefix, Query, Term
 from pyatlan.model.workflow import (
     ReRunRequest,
+    ScheduleQueriesSearchRequest,
     Workflow,
     WorkflowResponse,
     WorkflowRunResponse,
     WorkflowSchedule,
     WorkflowScheduleResponse,
     WorkflowSearchRequest,
     WorkflowSearchResponse,
@@ -52,23 +57,54 @@
                 "client", "ApiCaller"
             )
         self._client = client
 
     @staticmethod
     def _parse_response(raw_json, response_type):
         try:
-            if isinstance(raw_json, List):
+            if not raw_json:
+                return
+            elif isinstance(raw_json, list):
                 return parse_obj_as(List[response_type], raw_json)
             return parse_obj_as(response_type, raw_json)
         except ValidationError as err:
             raise ErrorCode.JSON_ERROR.exception_with_parameters(
                 raw_json, 200, str(err)
             ) from err
 
     @validate_arguments
+    def find_by_type(
+        self, prefix: WorkflowPackage, max_results: int = 10
+    ) -> List[WorkflowSearchResult]:
+        """
+        Find workflows based on their type (prefix). Note: Only workflows that have been run will be found.
+
+        :param prefix: name of the specific workflow to find (for example CONNECTION_DELETE)
+        :param max_results: the maximum number of results to retrieve
+        :returns: the list of workflows of the provided type, with the most-recently created first
+        :raises ValidationError: If the provided prefix is invalid workflow package
+        :raises AtlanError: on any API communication issue
+        """
+        query = Bool(
+            filter=[
+                NestedQuery(
+                    query=Prefix(field="metadata.name.keyword", value=prefix.value),
+                    path="metadata",
+                )
+            ]
+        )
+        request = WorkflowSearchRequest(query=query, size=max_results)
+        raw_json = self._client._call_api(
+            WORKFLOW_INDEX_SEARCH,
+            request_obj=request,
+        )
+        response = WorkflowSearchResponse(**raw_json)
+        return response.hits.hits or []
+
+    @validate_arguments
     def _find_latest_run(self, workflow_name: str) -> Optional[WorkflowSearchResult]:
         """
         Find the latest run of a given workflow
         :param name: name of the workflow for which to find the current run
         :returns: the singular result giving the latest run of the workflow
         :raises AtlanError: on any API communication issue
         """
@@ -150,44 +186,14 @@
         workflow.metadata.annotations and workflow.metadata.annotations.update(
             {
                 self._WORKFLOW_RUN_SCHEDULE: workflow_schedule.cron_schedule,
                 self._WORKFLOW_RUN_TIMEZONE: workflow_schedule.timezone,
             }
         )
 
-    @validate_arguments
-    def find_by_type(
-        self, prefix: WorkflowPackage, max_results: int = 10
-    ) -> List[WorkflowSearchResult]:
-        """
-        Find workflows based on their type (prefix).
-        Note: Only workflows that have been run will be found.
-
-        :param prefix: name of the specific workflow to find (for example CONNECTION_DELETE)
-        :param max_results: the maximum number of results to retrieve
-        :returns: the list of workflows of the provided type, with the most-recently created first
-        :raises ValidationError: If the provided prefix is invalid workflow package
-        :raises AtlanError: on any API communication issue
-        """
-        query = Bool(
-            filter=[
-                NestedQuery(
-                    query=Prefix(field="metadata.name.keyword", value=prefix.value),
-                    path="metadata",
-                )
-            ]
-        )
-        request = WorkflowSearchRequest(query=query, size=max_results)
-        raw_json = self._client._call_api(
-            WORKFLOW_INDEX_SEARCH,
-            request_obj=request,
-        )
-        response = WorkflowSearchResponse(**raw_json)
-        return response.hits.hits or []
-
     def _handle_workflow_types(self, workflow):
         if isinstance(workflow, WorkflowPackage):
             if results := self.find_by_type(workflow):
                 detail = results[0].source
             else:
                 raise ErrorCode.NO_PRIOR_RUN_AVAILABLE.exception_with_parameters(
                     workflow
@@ -298,14 +304,30 @@
         """
         raw_json = self._client._call_api(
             WORKFLOW_UPDATE.format_path({"workflow_name": workflow.metadata.name}),
             request_obj=workflow,
         )
         return WorkflowResponse(**raw_json)
 
+    @validate_arguments
+    def update_owner(self, workflow_name: str, username: str) -> WorkflowResponse:
+        """
+        Update the owner of the specified workflow.
+
+        :param workflow_name: name of the workflow to update.
+        :param username: username of the new owner.
+        :raises AtlanError: on any API communication issue.
+        :returns: updated workflow.
+        """
+        raw_json = self._client._call_api(
+            WORKFLOW_CHANGE_OWNER.format_path({"workflow_name": workflow_name}),
+            query_params={"username": username},
+        )
+        return WorkflowResponse(**raw_json)
+
     @validate_arguments(config=dict(arbitrary_types_allowed=True))
     def monitor(
         self, workflow_response: WorkflowResponse, logger: Optional[Logger] = None
     ) -> Optional[AtlanWorkflowPhase]:
         """
         Monitor the status of the workflow's run.
 
@@ -335,15 +357,14 @@
         if logger:
             logger.info("Skipping workflow monitoring — nothing to monitor.")
         return None
 
     def _get_run_details(self, name: str) -> Optional[WorkflowSearchResult]:
         return self._find_latest_run(workflow_name=name)
 
-    @validate_arguments
     def get_runs(
         self,
         workflow_name: str,
         workflow_phase: AtlanWorkflowPhase,
         from_: int = 0,
         size: int = 100,
     ) -> Optional[List[WorkflowSearchResult]]:
@@ -524,7 +545,88 @@
         :returns: a list of scheduled workflow runs.
         :raises AtlanError: on any API communication issue.
         """
         raw_json = self._client._call_api(
             GET_SCHEDULE_RUN.format_path({"workflow_name": f"{workflow_name}-cron"}),
         )
         return self._parse_response(raw_json, WorkflowScheduleResponse)
+
+    @validate_arguments
+    def find_schedule_query(
+        self, saved_query_id: str, max_results: int = 10
+    ) -> List[WorkflowSearchResult]:
+        """
+        Find scheduled query workflows by their saved query identifier.
+
+        :param saved_query_id: identifier of the saved query.
+        :param max_results: maximum number of results to retrieve. Defaults to `10`.
+        :raises AtlanError: on any API communication issue.
+        :returns: a list of scheduled query workflows.
+        """
+        query = Bool(
+            filter=[
+                NestedQuery(
+                    path="metadata",
+                    query=Prefix(
+                        field="metadata.name.keyword", value=f"asq-{saved_query_id}"
+                    ),
+                ),
+                NestedQuery(
+                    path="metadata",
+                    query=Term(
+                        field="metadata.annotations.package.argoproj.io/name.keyword",
+                        value="@atlan/schedule-query",
+                    ),
+                ),
+            ]
+        )
+        request = WorkflowSearchRequest(query=query, size=max_results)
+        raw_json = self._client._call_api(
+            WORKFLOW_INDEX_SEARCH,
+            request_obj=request,
+        )
+        response = WorkflowSearchResponse(**raw_json)
+        return response.hits.hits or []
+
+    @validate_arguments
+    def re_run_schedule_query(self, schedule_query_id: str) -> WorkflowRunResponse:
+        """
+        Re-run the scheduled query workflow by its schedule query identifier.
+        NOTE: Scheduled query workflows are re-triggered using
+        or impersonating the workflow owner's credentials.
+
+        :param schedule_query_id: identifier of the schedule query.
+        :raises AtlanError: on any API communication issue.
+        :returns: details of the workflow run.
+        """
+        request = ReRunRequest(namespace="default", resource_name=schedule_query_id)
+        raw_json = self._client._call_api(
+            WORKFLOW_OWNER_RERUN,
+            request_obj=request,
+        )
+        return WorkflowRunResponse(**raw_json)
+
+    @validate_arguments
+    def find_schedule_query_between(
+        self, request: ScheduleQueriesSearchRequest, missed: bool = False
+    ) -> Optional[List[WorkflowRunResponse]]:
+        """
+        Find scheduled query workflows within the specified duration.
+
+        :param request: a `ScheduleQueriesSearchRequest` object containing
+        start and end dates in ISO 8601 format (e.g: `2024-03-25T16:30:00.000+05:30`).
+        :param missed: if `True`, perform a search for missed
+        scheduled query workflows. Defaults to `False`.
+        :raises AtlanError: on any API communication issue.
+        :returns: a list of scheduled query workflows found within the specified duration.
+        """
+        query_params = {
+            "startDate": request.start_date,
+            "endDate": request.end_date,
+        }
+        SEARCH_API = (
+            SCHEDULE_QUERY_WORKFLOWS_MISSED
+            if missed
+            else SCHEDULE_QUERY_WORKFLOWS_SEARCH
+        )
+        raw_json = self._client._call_api(SEARCH_API, query_params=query_params)
+        return self._parse_response(raw_json, WorkflowRunResponse)
```

### Comparing `pyatlan-2.2.1/pyatlan/errors.py` & `pyatlan-2.2.2/pyatlan/errors.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/events/atlan_event_handler.py` & `pyatlan-2.2.2/pyatlan/events/atlan_event_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/events/atlan_lambda_handler.py` & `pyatlan-2.2.2/pyatlan/events/atlan_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/generator/class_generator.py` & `pyatlan-2.2.2/pyatlan/generator/class_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/generator/create_typedefs_file.py` & `pyatlan-2.2.2/pyatlan/generator/create_typedefs_file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/generator/templates/globals.jinja2` & `pyatlan-2.2.2/pyatlan/generator/templates/globals.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/generator/templates/imports.jinja2` & `pyatlan-2.2.2/pyatlan/generator/templates/imports.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     NumericRankField,
     RelationField,
     TextField,
 )
 from pyatlan.model.internal import AtlasServer, Internal
 from pyatlan.model.search import IndexSearchRequest
 from pyatlan.model.structs import (
+    Action,
     AuthPolicyCondition,
     AuthPolicyValiditySchedule,
     AwsTag,
     AzureTag,
     BadgeCondition,
     ColumnValueFrequencyMap,
     DbtMetricFilter,
```

### Comparing `pyatlan-2.2.1/pyatlan/generator/templates/macros.jinja2` & `pyatlan-2.2.2/pyatlan/generator/templates/macros.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/generator/templates/module.jinja2` & `pyatlan-2.2.2/pyatlan/generator/templates/module.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/generator/templates/properties.jinja2` & `pyatlan-2.2.2/pyatlan/generator/templates/properties.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/generator/templates/referenceable_attributes.jinja2` & `pyatlan-2.2.2/pyatlan/generator/templates/referenceable_attributes.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/generator/templates/referenceable_methods.jinja2` & `pyatlan-2.2.2/pyatlan/generator/templates/referenceable_methods.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/generator/templates/structs.jinja2` & `pyatlan-2.2.2/pyatlan/generator/templates/structs.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/logging.conf` & `pyatlan-2.2.2/pyatlan/logging.conf`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/aggregation.py` & `pyatlan-2.2.2/pyatlan/model/aggregation.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/api_tokens.py` & `pyatlan-2.2.2/pyatlan/model/api_tokens.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/__init__.py` & `pyatlan-2.2.2/pyatlan/model/assets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # Copyright 2022 Atlan Pte. Ltd.
 # isort: skip_file
 from .referenceable import Referenceable
 from .asset import Asset
+from .task import Task
 from .data_set import DataSet
 from .tag_attachment import TagAttachment
 from .connection import Connection
+from .workflow import Workflow
 from .process import Process
 from .atlas_glossary_category import AtlasGlossaryCategory
 from .stakeholder_title import StakeholderTitle
 from .badge import Badge
 from .access_control import AccessControl
 from .namespace import Namespace
 from .catalog import Catalog
+from .workflow_run import WorkflowRun
 from .atlas_glossary import AtlasGlossary
 from .auth_policy import AuthPolicy
 from .process_execution import ProcessExecution
 from .atlas_glossary_term import AtlasGlossaryTerm
 from .auth_service import AuthService
 from .cloud import Cloud
 from .infrastructure import Infrastructure
@@ -256,24 +259,27 @@
 from .azure_event_hub_consumer_group import AzureEventHubConsumerGroup
 
 
 # Update asset forward references:
 localns = locals()
 Referenceable.Attributes.update_forward_refs(**localns)
 Asset.Attributes.update_forward_refs(**localns)
+Task.Attributes.update_forward_refs(**localns)
 DataSet.Attributes.update_forward_refs(**localns)
 TagAttachment.Attributes.update_forward_refs(**localns)
 Connection.Attributes.update_forward_refs(**localns)
+Workflow.Attributes.update_forward_refs(**localns)
 Process.Attributes.update_forward_refs(**localns)
 AtlasGlossaryCategory.Attributes.update_forward_refs(**localns)
 StakeholderTitle.Attributes.update_forward_refs(**localns)
 Badge.Attributes.update_forward_refs(**localns)
 AccessControl.Attributes.update_forward_refs(**localns)
 Namespace.Attributes.update_forward_refs(**localns)
 Catalog.Attributes.update_forward_refs(**localns)
+WorkflowRun.Attributes.update_forward_refs(**localns)
 AtlasGlossary.Attributes.update_forward_refs(**localns)
 AuthPolicy.Attributes.update_forward_refs(**localns)
 ProcessExecution.Attributes.update_forward_refs(**localns)
 AtlasGlossaryTerm.Attributes.update_forward_refs(**localns)
 AuthService.Attributes.update_forward_refs(**localns)
 Cloud.Attributes.update_forward_refs(**localns)
 Infrastructure.Attributes.update_forward_refs(**localns)
```

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s.py` & `pyatlan-2.2.2/pyatlan/model/assets/a_d_l_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s_account.py` & `pyatlan-2.2.2/pyatlan/model/assets/a_d_l_s_account.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s_container.py` & `pyatlan-2.2.2/pyatlan/model/assets/a_d_l_s_container.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/a_d_l_s_object.py` & `pyatlan-2.2.2/pyatlan/model/assets/a_d_l_s_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/a_p_i.py` & `pyatlan-2.2.2/pyatlan/model/assets/a_p_i.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/a_p_i_path.py` & `pyatlan-2.2.2/pyatlan/model/assets/a_p_i_path.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/a_p_i_spec.py` & `pyatlan-2.2.2/pyatlan/model/assets/a_p_i_spec.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/a_w_s.py` & `pyatlan-2.2.2/pyatlan/model/assets/a_w_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/access_control.py` & `pyatlan-2.2.2/pyatlan/model/assets/access_control.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/airflow.py` & `pyatlan-2.2.2/pyatlan/model/assets/airflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/airflow_dag.py` & `pyatlan-2.2.2/pyatlan/model/assets/airflow_dag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/airflow_task.py` & `pyatlan-2.2.2/pyatlan/model/assets/airflow_task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/asset.py` & `pyatlan-2.2.2/pyatlan/model/assets/asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/atlas_glossary.py` & `pyatlan-2.2.2/pyatlan/model/assets/atlas_glossary.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/atlas_glossary_category.py` & `pyatlan-2.2.2/pyatlan/model/assets/atlas_glossary_category.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,19 @@
             ),
             DeprecationWarning,
             stacklevel=2,
         )
         return cls.creator(name=name, anchor=anchor, parent_category=parent_category)
 
     def trim_to_required(self) -> AtlasGlossaryCategory:
+        # The backend raises an exception unless the `glossary_guid` is provided.
+        # Providing the `glossary_qualified_name` won't work
         if self.anchor is None or not self.anchor.guid:
             raise ValueError("anchor.guid must be available")
-        return self.create_for_modification(
+        return self.updater(
             qualified_name=self.qualified_name or "",
             name=self.name or "",
             glossary_guid=self.anchor.guid,
         )
 
     @classmethod
     def updater(
@@ -93,16 +95,15 @@
         name: str = "",
         glossary_guid: str = "",
     ) -> SelfAsset:
         validate_required_fields(
             ["name", "qualified_name", "glossary_guid"],
             [name, qualified_name, glossary_guid],
         )
-        glossary = AtlasGlossary()
-        glossary.guid = glossary_guid
+        glossary = AtlasGlossary.ref_by_guid(glossary_guid)
         return cls(
             attributes=cls.Attributes(
                 qualified_name=qualified_name, name=name, anchor=glossary
             )
         )
 
     @classmethod
```

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/atlas_glossary_term.py` & `pyatlan-2.2.2/pyatlan/model/assets/atlas_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/auth_policy.py` & `pyatlan-2.2.2/pyatlan/model/assets/auth_policy.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/auth_service.py` & `pyatlan-2.2.2/pyatlan/model/assets/auth_service.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/azure.py` & `pyatlan-2.2.2/pyatlan/model/assets/azure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/azure_event_hub.py` & `pyatlan-2.2.2/pyatlan/model/assets/azure_event_hub.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,35 @@
 
 from __future__ import annotations
 
 from typing import ClassVar, List, Optional
 
 from pydantic.v1 import Field, validator
 
+from pyatlan.model.enums import AtlanConnectorType
 from pyatlan.model.fields.atlan_fields import KeywordField
+from pyatlan.utils import init_guid, validate_required_fields
 
 from .kafka_topic import KafkaTopic
 
 
 class AzureEventHub(KafkaTopic):
     """Description"""
 
+    @classmethod
+    @init_guid
+    def creator(cls, *, name: str, connection_qualified_name: str) -> AzureEventHub:
+        validate_required_fields(
+            ["name", "connection_qualified_name"], [name, connection_qualified_name]
+        )
+        attributes = AzureEventHub.Attributes.creator(
+            name=name, connection_qualified_name=connection_qualified_name
+        )
+        return cls(attributes=attributes)
+
     type_name: str = Field(default="AzureEventHub", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "AzureEventHub":
             raise ValueError("must be AzureEventHub")
         return v
@@ -51,14 +64,31 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_event_hub_status = azure_event_hub_status
 
     class Attributes(KafkaTopic.Attributes):
         azure_event_hub_status: Optional[str] = Field(default=None, description="")
 
+        @classmethod
+        @init_guid
+        def creator(
+            cls, *, name: str, connection_qualified_name: str
+        ) -> AzureEventHub.Attributes:
+            validate_required_fields(
+                ["name", "connection_qualified_name"], [name, connection_qualified_name]
+            )
+            return AzureEventHub.Attributes(
+                name=name,
+                qualified_name=f"{connection_qualified_name}/topic/{name}",
+                connection_qualified_name=connection_qualified_name,
+                connector_name=AtlanConnectorType.get_connector_name(
+                    connection_qualified_name
+                ),
+            )
+
     attributes: AzureEventHub.Attributes = Field(
         default_factory=lambda: AzureEventHub.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
             "so are described in the sub-types of this schema."
         ),
```

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/azure_event_hub_consumer_group.py` & `pyatlan-2.2.2/pyatlan/model/assets/b_i.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 from __future__ import annotations
 
 from typing import ClassVar, List
 
 from pydantic.v1 import Field, validator
 
-from .kafka_consumer_group import KafkaConsumerGroup
+from .catalog import Catalog
 
 
-class AzureEventHubConsumerGroup(KafkaConsumerGroup):
+class BI(Catalog):
     """Description"""
 
-    type_name: str = Field(default="AzureEventHubConsumerGroup", allow_mutation=False)
+    type_name: str = Field(default="BI", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "AzureEventHubConsumerGroup":
-            raise ValueError("must be AzureEventHubConsumerGroup")
+        if v != "BI":
+            raise ValueError("must be BI")
         return v
 
     def __setattr__(self, name, value):
-        if name in AzureEventHubConsumerGroup._convenience_properties:
+        if name in BI._convenience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convenience_properties: ClassVar[List[str]] = []
```

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/azure_service_bus.py` & `pyatlan-2.2.2/pyatlan/model/assets/azure_service_bus.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/azure_service_bus_namespace.py` & `pyatlan-2.2.2/pyatlan/model/assets/azure_service_bus_namespace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/azure_service_bus_topic.py` & `pyatlan-2.2.2/pyatlan/model/assets/azure_service_bus_topic.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/b_i.py` & `pyatlan-2.2.2/pyatlan/model/assets/mongo_d_b.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 from __future__ import annotations
 
 from typing import ClassVar, List
 
 from pydantic.v1 import Field, validator
 
-from .catalog import Catalog
+from .no_s_q_l import NoSQL
 
 
-class BI(Catalog):
+class MongoDB(NoSQL):
     """Description"""
 
-    type_name: str = Field(default="BI", allow_mutation=False)
+    type_name: str = Field(default="MongoDB", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "BI":
-            raise ValueError("must be BI")
+        if v != "MongoDB":
+            raise ValueError("must be MongoDB")
         return v
 
     def __setattr__(self, name, value):
-        if name in BI._convenience_properties:
+        if name in MongoDB._convenience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convenience_properties: ClassVar[List[str]] = []
```

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/b_i_process.py` & `pyatlan-2.2.2/pyatlan/model/assets/b_i_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/badge.py` & `pyatlan-2.2.2/pyatlan/model/assets/badge.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/calculation_view.py` & `pyatlan-2.2.2/pyatlan/model/assets/calculation_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/catalog.py` & `pyatlan-2.2.2/pyatlan/model/assets/catalog.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cloud.py` & `pyatlan-2.2.2/pyatlan/model/assets/cloud.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognite.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognite.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognite3_d_model.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognite3_d_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognite_asset.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognite_asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognite_event.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognite_event.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognite_file.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognite_file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognite_sequence.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognite_sequence.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognite_time_series.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognite_time_series.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognos.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognos.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognos_dashboard.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognos_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognos_datasource.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognos_datasource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognos_exploration.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognos_exploration.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognos_file.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognos_file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognos_folder.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognos_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognos_module.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognos_module.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognos_package.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognos_package.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cognos_report.py` & `pyatlan-2.2.2/pyatlan/model/assets/cognos_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/collection.py` & `pyatlan-2.2.2/pyatlan/model/assets/collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/column.py` & `pyatlan-2.2.2/pyatlan/model/assets/column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/column_process.py` & `pyatlan-2.2.2/pyatlan/model/assets/column_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/connection.py` & `pyatlan-2.2.2/pyatlan/model/assets/connection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cosmos_mongo_d_b.py` & `pyatlan-2.2.2/pyatlan/model/assets/cosmos_mongo_d_b.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cosmos_mongo_d_b_collection.py` & `pyatlan-2.2.2/pyatlan/model/assets/cosmos_mongo_d_b_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cosmos_mongo_d_b_database.py` & `pyatlan-2.2.2/pyatlan/model/assets/cosmos_mongo_d_b_database.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cube.py` & `pyatlan-2.2.2/pyatlan/model/assets/cube.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cube_dimension.py` & `pyatlan-2.2.2/pyatlan/model/assets/cube_dimension.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cube_field.py` & `pyatlan-2.2.2/pyatlan/model/assets/cube_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/cube_hierarchy.py` & `pyatlan-2.2.2/pyatlan/model/assets/cube_hierarchy.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/data_contract.py` & `pyatlan-2.2.2/pyatlan/model/assets/data_contract.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/data_domain.py` & `pyatlan-2.2.2/pyatlan/model/assets/data_domain.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/data_mesh.py` & `pyatlan-2.2.2/pyatlan/model/assets/data_mesh.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/data_product.py` & `pyatlan-2.2.2/pyatlan/model/assets/data_product.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/data_quality.py` & `pyatlan-2.2.2/pyatlan/model/assets/data_quality.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/data_set.py` & `pyatlan-2.2.2/pyatlan/model/assets/data_set.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/data_studio.py` & `pyatlan-2.2.2/pyatlan/model/assets/data_studio.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/data_studio_asset.py` & `pyatlan-2.2.2/pyatlan/model/assets/data_studio_asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/database.py` & `pyatlan-2.2.2/pyatlan/model/assets/database.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dbt.py` & `pyatlan-2.2.2/pyatlan/model/assets/dbt.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dbt_column_process.py` & `pyatlan-2.2.2/pyatlan/model/assets/dbt_column_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dbt_metric.py` & `pyatlan-2.2.2/pyatlan/model/assets/dbt_metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dbt_model.py` & `pyatlan-2.2.2/pyatlan/model/assets/dbt_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dbt_model_column.py` & `pyatlan-2.2.2/pyatlan/model/assets/dbt_model_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dbt_process.py` & `pyatlan-2.2.2/pyatlan/model/assets/dbt_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dbt_source.py` & `pyatlan-2.2.2/pyatlan/model/assets/dbt_source.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dbt_tag.py` & `pyatlan-2.2.2/pyatlan/model/assets/dbt_tag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dbt_test.py` & `pyatlan-2.2.2/pyatlan/model/assets/dbt_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/domo.py` & `pyatlan-2.2.2/pyatlan/model/assets/domo.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/domo_card.py` & `pyatlan-2.2.2/pyatlan/model/assets/domo_card.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/domo_dashboard.py` & `pyatlan-2.2.2/pyatlan/model/assets/domo_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/domo_dataset.py` & `pyatlan-2.2.2/pyatlan/model/assets/domo_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/domo_dataset_column.py` & `pyatlan-2.2.2/pyatlan/model/assets/domo_dataset_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b.py` & `pyatlan-2.2.2/pyatlan/model/assets/dynamo_d_b.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py` & `pyatlan-2.2.2/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py` & `pyatlan-2.2.2/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dynamo_d_b_secondary_index.py` & `pyatlan-2.2.2/pyatlan/model/assets/dynamo_d_b_secondary_index.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/dynamo_dbtable.py` & `pyatlan-2.2.2/pyatlan/model/assets/dynamo_dbtable.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/event_store.py` & `pyatlan-2.2.2/pyatlan/model/assets/event_store.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/file.py` & `pyatlan-2.2.2/pyatlan/model/assets/file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/folder.py` & `pyatlan-2.2.2/pyatlan/model/assets/folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/function.py` & `pyatlan-2.2.2/pyatlan/model/assets/function.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/g_c_s.py` & `pyatlan-2.2.2/pyatlan/model/assets/g_c_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/g_c_s_bucket.py` & `pyatlan-2.2.2/pyatlan/model/assets/g_c_s_bucket.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/g_c_s_object.py` & `pyatlan-2.2.2/pyatlan/model/assets/g_c_s_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/google.py` & `pyatlan-2.2.2/pyatlan/model/assets/google.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/infrastructure.py` & `pyatlan-2.2.2/pyatlan/model/assets/infrastructure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/insight.py` & `pyatlan-2.2.2/pyatlan/model/assets/insight.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/kafka.py` & `pyatlan-2.2.2/pyatlan/model/assets/kafka.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/kafka_consumer_group.py` & `pyatlan-2.2.2/pyatlan/model/assets/kafka_consumer_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,23 +4,43 @@
 
 from __future__ import annotations
 
 from typing import ClassVar, List, Optional, Set
 
 from pydantic.v1 import Field, validator
 
+from pyatlan.model.enums import AtlanConnectorType
 from pyatlan.model.fields.atlan_fields import KeywordField, NumericField, RelationField
 from pyatlan.model.structs import KafkaTopicConsumption
+from pyatlan.utils import init_guid, validate_required_fields
 
 from .kafka import Kafka
 
 
 class KafkaConsumerGroup(Kafka):
     """Description"""
 
+    @classmethod
+    @init_guid
+    def creator(
+        cls,
+        *,
+        name: str,
+        kafka_topic_qualified_names: List[str],
+    ) -> KafkaConsumerGroup:
+        validate_required_fields(
+            ["name", "kafka_topic_qualified_names"],
+            [name, kafka_topic_qualified_names],
+        )
+        attributes = KafkaConsumerGroup.Attributes.creator(
+            name=name,
+            kafka_topic_qualified_names=kafka_topic_qualified_names,
+        )
+        return cls(attributes=attributes)
+
     type_name: str = Field(default="KafkaConsumerGroup", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "KafkaConsumerGroup":
             raise ValueError("must be KafkaConsumerGroup")
         return v
@@ -159,14 +179,42 @@
         kafka_topic_qualified_names: Optional[Set[str]] = Field(
             default=None, description=""
         )
         kafka_topics: Optional[List[KafkaTopic]] = Field(
             default=None, description=""
         )  # relationship
 
+        @classmethod
+        @init_guid
+        def creator(
+            cls,
+            *,
+            name: str,
+            kafka_topic_qualified_names: List[str],
+        ) -> KafkaConsumerGroup.Attributes:
+            validate_required_fields(
+                ["name", "kafka_topic_qualified_names"],
+                [name, kafka_topic_qualified_names],
+            )
+            kafka_topics = []
+            for kafka_topic_qn in kafka_topic_qualified_names:
+                connection_qn, connector_name = AtlanConnectorType.get_connector_name(
+                    kafka_topic_qn, "kafka_topic_qualified_names", 5
+                )
+                kafka_topics.append(KafkaTopic.ref_by_qualified_name(kafka_topic_qn))
+
+            return KafkaConsumerGroup.Attributes(
+                name=name,
+                connector_name=connector_name,
+                connection_qualified_name=connection_qn,
+                kafka_topics=kafka_topics,
+                kafka_topic_qualified_names=set(kafka_topic_qualified_names),
+                qualified_name=f"{connection_qn}/consumer-group/{name}",
+            )
+
     attributes: KafkaConsumerGroup.Attributes = Field(
         default_factory=lambda: KafkaConsumerGroup.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
             "so are described in the sub-types of this schema."
         ),
```

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/kafka_topic.py` & `pyatlan-2.2.2/pyatlan/model/assets/kafka_topic.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,44 @@
 
 from __future__ import annotations
 
 from typing import ClassVar, List, Optional
 
 from pydantic.v1 import Field, validator
 
-from pyatlan.model.enums import KafkaTopicCleanupPolicy, KafkaTopicCompressionType
+from pyatlan.model.enums import (
+    AtlanConnectorType,
+    KafkaTopicCleanupPolicy,
+    KafkaTopicCompressionType,
+)
 from pyatlan.model.fields.atlan_fields import (
     BooleanField,
     KeywordField,
     NumericField,
     RelationField,
 )
+from pyatlan.utils import init_guid, validate_required_fields
 
 from .kafka import Kafka
 
 
 class KafkaTopic(Kafka):
     """Description"""
 
+    @classmethod
+    @init_guid
+    def creator(cls, *, name: str, connection_qualified_name: str) -> KafkaTopic:
+        validate_required_fields(
+            ["name", "connection_qualified_name"], [name, connection_qualified_name]
+        )
+        attributes = KafkaTopic.Attributes.creator(
+            name=name, connection_qualified_name=connection_qualified_name
+        )
+        return cls(attributes=attributes)
+
     type_name: str = Field(default="KafkaTopic", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "KafkaTopic":
             raise ValueError("must be KafkaTopic")
         return v
@@ -278,14 +294,31 @@
         kafka_topic_cleanup_policy: Optional[KafkaTopicCleanupPolicy] = Field(
             default=None, description=""
         )
         kafka_consumer_groups: Optional[List[KafkaConsumerGroup]] = Field(
             default=None, description=""
         )  # relationship
 
+        @classmethod
+        @init_guid
+        def creator(
+            cls, *, name: str, connection_qualified_name: str
+        ) -> KafkaTopic.Attributes:
+            validate_required_fields(
+                ["name", "connection_qualified_name"], [name, connection_qualified_name]
+            )
+            return KafkaTopic.Attributes(
+                name=name,
+                qualified_name=f"{connection_qualified_name}/topic/{name}",
+                connection_qualified_name=connection_qualified_name,
+                connector_name=AtlanConnectorType.get_connector_name(
+                    connection_qualified_name
+                ),
+            )
+
     attributes: KafkaTopic.Attributes = Field(
         default_factory=lambda: KafkaTopic.Attributes(),
         description=(
             "Map of attributes in the instance and their values. "
             "The specific keys of this map will vary by type, "
             "so are described in the sub-types of this schema."
         ),
```

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/link.py` & `pyatlan-2.2.2/pyatlan/model/assets/link.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/looker.py` & `pyatlan-2.2.2/pyatlan/model/assets/looker.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/looker_dashboard.py` & `pyatlan-2.2.2/pyatlan/model/assets/looker_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/looker_explore.py` & `pyatlan-2.2.2/pyatlan/model/assets/looker_explore.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/looker_field.py` & `pyatlan-2.2.2/pyatlan/model/assets/looker_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/looker_folder.py` & `pyatlan-2.2.2/pyatlan/model/assets/looker_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/looker_look.py` & `pyatlan-2.2.2/pyatlan/model/assets/looker_look.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/looker_model.py` & `pyatlan-2.2.2/pyatlan/model/assets/looker_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/looker_project.py` & `pyatlan-2.2.2/pyatlan/model/assets/looker_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/looker_query.py` & `pyatlan-2.2.2/pyatlan/model/assets/looker_query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/looker_tile.py` & `pyatlan-2.2.2/pyatlan/model/assets/looker_tile.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/looker_view.py` & `pyatlan-2.2.2/pyatlan/model/assets/looker_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/m_c_incident.py` & `pyatlan-2.2.2/pyatlan/model/assets/m_c_incident.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/m_c_monitor.py` & `pyatlan-2.2.2/pyatlan/model/assets/m_c_monitor.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/materialised_view.py` & `pyatlan-2.2.2/pyatlan/model/assets/materialised_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/matillion.py` & `pyatlan-2.2.2/pyatlan/model/assets/matillion.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/matillion_component.py` & `pyatlan-2.2.2/pyatlan/model/assets/matillion_component.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/matillion_group.py` & `pyatlan-2.2.2/pyatlan/model/assets/matillion_group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/matillion_job.py` & `pyatlan-2.2.2/pyatlan/model/assets/matillion_job.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/matillion_project.py` & `pyatlan-2.2.2/pyatlan/model/assets/matillion_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/metabase.py` & `pyatlan-2.2.2/pyatlan/model/assets/metabase.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/metabase_collection.py` & `pyatlan-2.2.2/pyatlan/model/assets/metabase_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/metabase_dashboard.py` & `pyatlan-2.2.2/pyatlan/model/assets/metabase_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/metabase_question.py` & `pyatlan-2.2.2/pyatlan/model/assets/metabase_question.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/metric.py` & `pyatlan-2.2.2/pyatlan/model/assets/metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy.py` & `pyatlan-2.2.2/pyatlan/model/assets/micro_strategy.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_attribute.py` & `pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_attribute.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_cube.py` & `pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_cube.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_document.py` & `pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_document.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_dossier.py` & `pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_dossier.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_fact.py` & `pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_fact.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_metric.py` & `pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_project.py` & `pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_report.py` & `pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/micro_strategy_visualization.py` & `pyatlan-2.2.2/pyatlan/model/assets/micro_strategy_visualization.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/mode.py` & `pyatlan-2.2.2/pyatlan/model/assets/mode.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/mode_chart.py` & `pyatlan-2.2.2/pyatlan/model/assets/mode_chart.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/mode_collection.py` & `pyatlan-2.2.2/pyatlan/model/assets/mode_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/mode_query.py` & `pyatlan-2.2.2/pyatlan/model/assets/mode_query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/mode_report.py` & `pyatlan-2.2.2/pyatlan/model/assets/mode_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/mode_workspace.py` & `pyatlan-2.2.2/pyatlan/model/assets/mode_workspace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/mongo_d_b.py` & `pyatlan-2.2.2/pyatlan/model/assets/sisense.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 from __future__ import annotations
 
 from typing import ClassVar, List
 
 from pydantic.v1 import Field, validator
 
-from .no_s_q_l import NoSQL
+from .b_i import BI
 
 
-class MongoDB(NoSQL):
+class Sisense(BI):
     """Description"""
 
-    type_name: str = Field(default="MongoDB", allow_mutation=False)
+    type_name: str = Field(default="Sisense", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "MongoDB":
-            raise ValueError("must be MongoDB")
+        if v != "Sisense":
+            raise ValueError("must be Sisense")
         return v
 
     def __setattr__(self, name, value):
-        if name in MongoDB._convenience_properties:
+        if name in Sisense._convenience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convenience_properties: ClassVar[List[str]] = []
```

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/mongo_d_b_collection.py` & `pyatlan-2.2.2/pyatlan/model/assets/mongo_d_b_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/mongo_d_b_database.py` & `pyatlan-2.2.2/pyatlan/model/assets/mongo_d_b_database.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/monte_carlo.py` & `pyatlan-2.2.2/pyatlan/model/assets/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/multi_dimensional_dataset.py` & `pyatlan-2.2.2/pyatlan/model/assets/multi_dimensional_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/namespace.py` & `pyatlan-2.2.2/pyatlan/model/assets/namespace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/no_s_q_l.py` & `pyatlan-2.2.2/pyatlan/model/assets/no_s_q_l.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/object_store.py` & `pyatlan-2.2.2/pyatlan/model/assets/object_store.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/persona.py` & `pyatlan-2.2.2/pyatlan/model/assets/persona.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/power_b_i.py` & `pyatlan-2.2.2/pyatlan/model/assets/power_b_i.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_column.py` & `pyatlan-2.2.2/pyatlan/model/assets/power_b_i_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_dashboard.py` & `pyatlan-2.2.2/pyatlan/model/assets/power_b_i_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_dataflow.py` & `pyatlan-2.2.2/pyatlan/model/assets/power_b_i_dataflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_dataset.py` & `pyatlan-2.2.2/pyatlan/model/assets/power_b_i_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_datasource.py` & `pyatlan-2.2.2/pyatlan/model/assets/power_b_i_datasource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_measure.py` & `pyatlan-2.2.2/pyatlan/model/assets/power_b_i_measure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_page.py` & `pyatlan-2.2.2/pyatlan/model/assets/power_b_i_page.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_report.py` & `pyatlan-2.2.2/pyatlan/model/assets/power_b_i_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_table.py` & `pyatlan-2.2.2/pyatlan/model/assets/power_b_i_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_tile.py` & `pyatlan-2.2.2/pyatlan/model/assets/power_b_i_tile.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/power_b_i_workspace.py` & `pyatlan-2.2.2/pyatlan/model/assets/power_b_i_workspace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/preset.py` & `pyatlan-2.2.2/pyatlan/model/assets/preset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/preset_chart.py` & `pyatlan-2.2.2/pyatlan/model/assets/preset_chart.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/preset_dashboard.py` & `pyatlan-2.2.2/pyatlan/model/assets/preset_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/preset_dataset.py` & `pyatlan-2.2.2/pyatlan/model/assets/preset_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/preset_workspace.py` & `pyatlan-2.2.2/pyatlan/model/assets/preset_workspace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/procedure.py` & `pyatlan-2.2.2/pyatlan/model/assets/procedure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/process.py` & `pyatlan-2.2.2/pyatlan/model/assets/process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/process_execution.py` & `pyatlan-2.2.2/pyatlan/model/assets/process_execution.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/purpose.py` & `pyatlan-2.2.2/pyatlan/model/assets/purpose.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/qlik.py` & `pyatlan-2.2.2/pyatlan/model/assets/qlik.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/qlik_app.py` & `pyatlan-2.2.2/pyatlan/model/assets/qlik_app.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/qlik_chart.py` & `pyatlan-2.2.2/pyatlan/model/assets/qlik_chart.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/qlik_dataset.py` & `pyatlan-2.2.2/pyatlan/model/assets/qlik_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/qlik_sheet.py` & `pyatlan-2.2.2/pyatlan/model/assets/qlik_sheet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/qlik_space.py` & `pyatlan-2.2.2/pyatlan/model/assets/qlik_space.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/qlik_stream.py` & `pyatlan-2.2.2/pyatlan/model/assets/qlik_stream.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/query.py` & `pyatlan-2.2.2/pyatlan/model/assets/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/quick_sight.py` & `pyatlan-2.2.2/pyatlan/model/assets/quick_sight.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_analysis.py` & `pyatlan-2.2.2/pyatlan/model/assets/quick_sight_analysis.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_analysis_visual.py` & `pyatlan-2.2.2/pyatlan/model/assets/quick_sight_analysis_visual.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dashboard.py` & `pyatlan-2.2.2/pyatlan/model/assets/quick_sight_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dashboard_visual.py` & `pyatlan-2.2.2/pyatlan/model/assets/quick_sight_dashboard_visual.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dataset.py` & `pyatlan-2.2.2/pyatlan/model/assets/quick_sight_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_dataset_field.py` & `pyatlan-2.2.2/pyatlan/model/assets/quick_sight_dataset_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/quick_sight_folder.py` & `pyatlan-2.2.2/pyatlan/model/assets/quick_sight_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/readme.py` & `pyatlan-2.2.2/pyatlan/model/assets/readme.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/readme_template.py` & `pyatlan-2.2.2/pyatlan/model/assets/readme_template.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/redash.py` & `pyatlan-2.2.2/pyatlan/model/assets/redash.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/redash_dashboard.py` & `pyatlan-2.2.2/pyatlan/model/assets/redash_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/redash_query.py` & `pyatlan-2.2.2/pyatlan/model/assets/redash_query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/redash_visualization.py` & `pyatlan-2.2.2/pyatlan/model/assets/redash_visualization.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/referenceable.py` & `pyatlan-2.2.2/pyatlan/model/assets/referenceable.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/resource.py` & `pyatlan-2.2.2/pyatlan/model/assets/resource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/s3.py` & `pyatlan-2.2.2/pyatlan/model/assets/s3.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/s3_bucket.py` & `pyatlan-2.2.2/pyatlan/model/assets/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/s3_object.py` & `pyatlan-2.2.2/pyatlan/model/assets/s3_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/s_q_l.py` & `pyatlan-2.2.2/pyatlan/model/assets/s_q_l.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/saa_s.py` & `pyatlan-2.2.2/pyatlan/model/assets/saa_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/salesforce.py` & `pyatlan-2.2.2/pyatlan/model/assets/salesforce.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/salesforce_dashboard.py` & `pyatlan-2.2.2/pyatlan/model/assets/salesforce_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/salesforce_field.py` & `pyatlan-2.2.2/pyatlan/model/assets/salesforce_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/salesforce_object.py` & `pyatlan-2.2.2/pyatlan/model/assets/salesforce_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/salesforce_organization.py` & `pyatlan-2.2.2/pyatlan/model/assets/salesforce_organization.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/salesforce_report.py` & `pyatlan-2.2.2/pyatlan/model/assets/salesforce_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/schema.py` & `pyatlan-2.2.2/pyatlan/model/assets/schema.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/schema_registry.py` & `pyatlan-2.2.2/pyatlan/model/assets/schema_registry.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/schema_registry_subject.py` & `pyatlan-2.2.2/pyatlan/model/assets/schema_registry_subject.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sigma.py` & `pyatlan-2.2.2/pyatlan/model/assets/sigma.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sigma_data_element.py` & `pyatlan-2.2.2/pyatlan/model/assets/sigma_data_element.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sigma_data_element_field.py` & `pyatlan-2.2.2/pyatlan/model/assets/sigma_data_element_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sigma_dataset.py` & `pyatlan-2.2.2/pyatlan/model/assets/sigma_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sigma_dataset_column.py` & `pyatlan-2.2.2/pyatlan/model/assets/sigma_dataset_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sigma_page.py` & `pyatlan-2.2.2/pyatlan/model/assets/sigma_page.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sigma_workbook.py` & `pyatlan-2.2.2/pyatlan/model/assets/sigma_workbook.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sisense.py` & `pyatlan-2.2.2/pyatlan/model/assets/soda.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 from __future__ import annotations
 
 from typing import ClassVar, List
 
 from pydantic.v1 import Field, validator
 
-from .b_i import BI
+from .data_quality import DataQuality
 
 
-class Sisense(BI):
+class Soda(DataQuality):
     """Description"""
 
-    type_name: str = Field(default="Sisense", allow_mutation=False)
+    type_name: str = Field(default="Soda", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "Sisense":
-            raise ValueError("must be Sisense")
+        if v != "Soda":
+            raise ValueError("must be Soda")
         return v
 
     def __setattr__(self, name, value):
-        if name in Sisense._convenience_properties:
+        if name in Soda._convenience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convenience_properties: ClassVar[List[str]] = []
```

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sisense_dashboard.py` & `pyatlan-2.2.2/pyatlan/model/assets/sisense_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sisense_datamodel.py` & `pyatlan-2.2.2/pyatlan/model/assets/sisense_datamodel.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sisense_datamodel_table.py` & `pyatlan-2.2.2/pyatlan/model/assets/sisense_datamodel_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sisense_folder.py` & `pyatlan-2.2.2/pyatlan/model/assets/sisense_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/sisense_widget.py` & `pyatlan-2.2.2/pyatlan/model/assets/sisense_widget.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/snowflake_dynamic_table.py` & `pyatlan-2.2.2/pyatlan/model/assets/snowflake_dynamic_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/snowflake_pipe.py` & `pyatlan-2.2.2/pyatlan/model/assets/snowflake_pipe.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/snowflake_stream.py` & `pyatlan-2.2.2/pyatlan/model/assets/snowflake_stream.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/snowflake_tag.py` & `pyatlan-2.2.2/pyatlan/model/assets/snowflake_tag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/soda.py` & `pyatlan-2.2.2/pyatlan/model/assets/tableau.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 from __future__ import annotations
 
 from typing import ClassVar, List
 
 from pydantic.v1 import Field, validator
 
-from .data_quality import DataQuality
+from .b_i import BI
 
 
-class Soda(DataQuality):
+class Tableau(BI):
     """Description"""
 
-    type_name: str = Field(default="Soda", allow_mutation=False)
+    type_name: str = Field(default="Tableau", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "Soda":
-            raise ValueError("must be Soda")
+        if v != "Tableau":
+            raise ValueError("must be Tableau")
         return v
 
     def __setattr__(self, name, value):
-        if name in Soda._convenience_properties:
+        if name in Tableau._convenience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convenience_properties: ClassVar[List[str]] = []
```

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/soda_check.py` & `pyatlan-2.2.2/pyatlan/model/assets/soda_check.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/spark.py` & `pyatlan-2.2.2/pyatlan/model/assets/spark.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/spark_job.py` & `pyatlan-2.2.2/pyatlan/model/assets/spark_job.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/stakeholder.py` & `pyatlan-2.2.2/pyatlan/model/assets/stakeholder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/stakeholder_title.py` & `pyatlan-2.2.2/pyatlan/model/assets/stakeholder_title.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/table.py` & `pyatlan-2.2.2/pyatlan/model/assets/table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/table_partition.py` & `pyatlan-2.2.2/pyatlan/model/assets/table_partition.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/tableau_calculated_field.py` & `pyatlan-2.2.2/pyatlan/model/assets/tableau_calculated_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/tableau_dashboard.py` & `pyatlan-2.2.2/pyatlan/model/assets/tableau_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/tableau_datasource.py` & `pyatlan-2.2.2/pyatlan/model/assets/tableau_datasource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/tableau_datasource_field.py` & `pyatlan-2.2.2/pyatlan/model/assets/tableau_datasource_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/tableau_flow.py` & `pyatlan-2.2.2/pyatlan/model/assets/tableau_flow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/tableau_metric.py` & `pyatlan-2.2.2/pyatlan/model/assets/tableau_metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/tableau_project.py` & `pyatlan-2.2.2/pyatlan/model/assets/tableau_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/tableau_site.py` & `pyatlan-2.2.2/pyatlan/model/assets/tableau_site.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/tableau_workbook.py` & `pyatlan-2.2.2/pyatlan/model/assets/tableau_workbook.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/tableau_worksheet.py` & `pyatlan-2.2.2/pyatlan/model/assets/tableau_worksheet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/tag.py` & `pyatlan-2.2.2/pyatlan/model/assets/tag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/tag_attachment.py` & `pyatlan-2.2.2/pyatlan/model/assets/tag_attachment.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot.py` & `pyatlan-2.2.2/pyatlan/model/assets/thoughtspot.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_answer.py` & `pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_answer.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_column.py` & `pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_dashlet.py` & `pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_dashlet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_liveboard.py` & `pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_liveboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_table.py` & `pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_view.py` & `pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/thoughtspot_worksheet.py` & `pyatlan-2.2.2/pyatlan/model/assets/thoughtspot_worksheet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/assets/view.py` & `pyatlan-2.2.2/pyatlan/model/assets/view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/atlan_image.py` & `pyatlan-2.2.2/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/audit.py` & `pyatlan-2.2.2/pyatlan/model/audit.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/core.py` & `pyatlan-2.2.2/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/credential.py` & `pyatlan-2.2.2/pyatlan/model/credential.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/custom_metadata.py` & `pyatlan-2.2.2/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/data_mesh.py` & `pyatlan-2.2.2/pyatlan/model/data_mesh.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/enums.py` & `pyatlan-2.2.2/pyatlan/model/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -2338,7 +2338,38 @@
     PROTOBUF = "PROTOBUF"
 
 
 class SourceCostUnitType(str, Enum):
     CREDITS = "Credits"
     BYTES = "bytes"
     SLOT_MS = "slot-ms"
+
+
+class WorkflowRunStatus(str, Enum):
+    PENDING = "PENDING"
+    APPROVED = "APPROVED"
+    REJECTED = "REJECTED"
+    SUCCESS = "SUCCESS"
+    FAILURE = "FAILURE"
+    WITHDRAWN = "WITHDRAWN"
+    EXPIRED = "EXPIRED"
+    TERMINATED = "TERMINATED"
+
+
+class WorkflowRunType(str, Enum):
+    DATA_ACCESS = "DATA_ACCESS"
+    POLICY = "POLICY"
+    CHANGE_MANAGEMENT = "CHANGE_MANAGEMENT"
+    PUBLICATION_MANAGEMENT = "PUBLICATION_MANAGEMENT"
+
+
+class WorkflowStatus(str, Enum):
+    PUBLISHED = "PUBLISHED"
+    DRAFT = "DRAFT"
+    DISABLED = "DISABLED"
+
+
+class WorkflowType(str, Enum):
+    DATA_ACCESS = "DATA_ACCESS"
+    POLICY = "POLICY"
+    CHANGE_MANAGEMENT = "CHANGE_MANAGEMENT"
+    PUBLICATION_MANAGEMENT = "PUBLICATION_MANAGEMENT"
```

### Comparing `pyatlan-2.2.1/pyatlan/model/events.py` & `pyatlan-2.2.2/pyatlan/model/events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/fields/atlan_fields.py` & `pyatlan-2.2.2/pyatlan/model/fields/atlan_fields.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/fluent_search.py` & `pyatlan-2.2.2/pyatlan/model/fluent_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/fluent_tasks.py` & `pyatlan-2.2.2/pyatlan/model/fluent_tasks.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/group.py` & `pyatlan-2.2.2/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/keycloak_events.py` & `pyatlan-2.2.2/pyatlan/model/keycloak_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/lineage.py` & `pyatlan-2.2.2/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/__init__.py` & `pyatlan-2.2.2/pyatlan/model/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/base/crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/base/crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/base/miner.py` & `pyatlan-2.2.2/pyatlan/model/packages/base/miner.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/base/package.py` & `pyatlan-2.2.2/pyatlan/model/packages/base/package.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/big_query_crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/big_query_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/confluent_kafka_crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/confluent_kafka_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/dbt_crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/dbt_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/dynamo_d_b_crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/dynamo_d_b_crawler.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,15 +172,15 @@
                 "orchestration.atlan.com/icon": self._PACKAGE_ICON,
                 "orchestration.atlan.com/logo": self._PACKAGE_LOGO,
                 "orchestration.atlan.com/marketplaceLink": f"https://packages.atlan.com/-/web/detail/{self._PACKAGE_NAME}",  # noqa
                 "orchestration.atlan.com/name": "Amazon DynamoDB Assets",
                 "package.argoproj.io/author": "Atlan",
                 "package.argoproj.io/description": "Package to crawl Amazon DynamoDB assets and publish to Atlan for discovery",  # noqa
                 "package.argoproj.io/homepage": f"https://packages.atlan.com/-/web/detail/{self._PACKAGE_NAME}",
-                "package.argoproj.io/keywords": "[\"dynamodb\",\"nosql\",\"document-database\",\"connector\",\"crawler\"]",  # fmt: skip  # noqa
+                "package.argoproj.io/keywords": '["dynamodb","nosql","document-database","connector","crawler"]',  # fmt: skip  # noqa
                 "package.argoproj.io/name": self._PACKAGE_NAME,
                 "package.argoproj.io/registry": "https://packages.atlan.com",
                 "package.argoproj.io/repository": "https://github.com/atlanhq/marketplace-packages.git",
                 "package.argoproj.io/support": "support@atlan.com",
                 "orchestration.atlan.com/atlanName": f"{self._PACKAGE_PREFIX}-default-{self._NAME}-{self._epoch}",
             },
             name=f"{self._PACKAGE_PREFIX}-{self._epoch}",
```

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/glue_crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/postgres_crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/postgres_crawler.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
                 "orchestration.atlan.com/icon": self._PACKAGE_ICON,
                 "orchestration.atlan.com/logo": self._PACKAGE_LOGO,
                 "orchestration.atlan.com/marketplaceLink": f"https://packages.atlan.com/-/web/detail/{self._PACKAGE_NAME}",  # noqa
                 "orchestration.atlan.com/name": "Postgres Assets",
                 "package.argoproj.io/author": "Atlan",
                 "package.argoproj.io/description": "Package to crawl PostgreSQL assets and publish to Atlan for discovery",  # noqa
                 "package.argoproj.io/homepage": f"https://packages.atlan.com/-/web/detail/{self._PACKAGE_NAME}",
-                "package.argoproj.io/keywords": "[\"postgres\",\"database\",\"sql\",\"connector\",\"crawler\"]",  # fmt: skip  # noqa
+                "package.argoproj.io/keywords": '["postgres","database","sql","connector","crawler"]',  # fmt: skip  # noqa
                 "package.argoproj.io/name": self._PACKAGE_NAME,
                 "package.argoproj.io/registry": "https://packages.atlan.com",
                 "package.argoproj.io/repository": "https://github.com/atlanhq/marketplace-packages.git",
                 "package.argoproj.io/support": "support@atlan.com",
                 "orchestration.atlan.com/atlanName": f"{self._PACKAGE_PREFIX}-default-{self._NAME}-{self._epoch}",
             },
             name=f"{self._PACKAGE_PREFIX}-{self._epoch}",
```

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/powerbi_crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/powerbi_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/s_q_l_server_crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/s_q_l_server_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/sigma_crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/sigma_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/snowflake_crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/snowflake_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/snowflake_miner.py` & `pyatlan-2.2.2/pyatlan/model/packages/snowflake_miner.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/sql_server_crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/sql_server_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/packages/tableau_crawler.py` & `pyatlan-2.2.2/pyatlan/model/packages/tableau_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/query.py` & `pyatlan-2.2.2/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/response.py` & `pyatlan-2.2.2/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/role.py` & `pyatlan-2.2.2/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/search.py` & `pyatlan-2.2.2/pyatlan/model/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1879,14 +1879,22 @@
     )
     allow_deleted_relations: Optional[bool] = Field(
         default=None,
         description="Whether to include deleted relationships to this asset (true) or not (false). By default, "
         "this is false and therefore only active (not deleted) relationships will be included.",
         alias="allowDeletedRelations",
     )
+    include_atlan_tag_names: Optional[bool] = Field(
+        default=None,
+        description=(
+            "Whether to include Atlan tag names for this asset (`True`) or not (`False`) "
+            "Note: This will only work when `exclude_atlan_tags` is set to `True`."
+        ),
+        alias="includeClassificationNames",
+    )
 
     class Metadata(AtlanObject):
         save_search_log: bool = Field(
             default=True, description="Whether to log this search (True) or not (False)"
         )
         utm_tags: List[str] = Field(
             default_factory=list,
```

### Comparing `pyatlan-2.2.1/pyatlan/model/search_log.py` & `pyatlan-2.2.2/pyatlan/model/search_log.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/sso.py` & `pyatlan-2.2.2/pyatlan/model/sso.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/structs.py` & `pyatlan-2.2.2/pyatlan/model/structs.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,23 @@
 class Histogram(AtlanObject):
     """Description"""
 
     boundaries: Set[float] = Field(description="")
     frequencies: Set[float] = Field(description="")
 
 
+class Action(AtlanObject):
+    """Description"""
+
+    task_action_fulfillment_url: Optional[str] = Field(default=None, description="")
+    task_action_fulfillment_method: Optional[str] = Field(default=None, description="")
+    task_action_fulfillment_payload: Optional[str] = Field(default=None, description="")
+    task_action_display_text: Optional[str] = Field(default=None, description="")
+
+
 class ColumnValueFrequencyMap(AtlanObject):
     """Description"""
 
     column_value: Optional[str] = Field(default=None, description="")
     column_value_frequency: Optional[int] = Field(default=None, description="")
 
 
@@ -242,14 +251,16 @@
 
 AwsCloudWatchMetric.update_forward_refs()
 
 KafkaTopicConsumption.update_forward_refs()
 
 Histogram.update_forward_refs()
 
+Action.update_forward_refs()
+
 ColumnValueFrequencyMap.update_forward_refs()
 
 BadgeCondition.update_forward_refs()
 
 SourceTagAttachment.update_forward_refs()
 
 SourceTagAttachmentValue.update_forward_refs()
```

### Comparing `pyatlan-2.2.1/pyatlan/model/task.py` & `pyatlan-2.2.2/pyatlan/model/task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/typedef.py` & `pyatlan-2.2.2/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/user.py` & `pyatlan-2.2.2/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/utils.py` & `pyatlan-2.2.2/pyatlan/model/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/model/workflow.py` & `pyatlan-2.2.2/pyatlan/model/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,19 @@
     payload: Optional[List[Any]] = Field(default_factory=list)
 
 
 class WorkflowRunResponse(WorkflowResponse):
     status: WorkflowSearchResultStatus
 
 
+class ScheduleQueriesSearchRequest(AtlanObject):
+    start_date: str = Field(description="Start date in ISO 8601 format")
+    end_date: str = Field(description="End date in ISO 8601 format")
+
+
 class WorkflowSchedule(AtlanObject):
     timezone: str
     cron_schedule: str
 
 
 class WorkflowScheduleSpec(AtlanObject):
     schedule: Optional[str] = Field(default=None)
```

### Comparing `pyatlan-2.2.1/pyatlan/multipart_data_generator.py` & `pyatlan-2.2.2/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/pkg/create_package_files.py` & `pyatlan-2.2.2/pyatlan/pkg/create_package_files.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/pkg/models.py` & `pyatlan-2.2.2/pyatlan/pkg/models.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/pkg/templates/default_configmap.jinja2` & `pyatlan-2.2.2/pyatlan/pkg/templates/default_configmap.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/pkg/templates/default_template.jinja2` & `pyatlan-2.2.2/pyatlan/pkg/templates/default_template.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/pkg/templates/package_config.jinja2` & `pyatlan-2.2.2/pyatlan/pkg/templates/package_config.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/pkg/ui.py` & `pyatlan-2.2.2/pyatlan/pkg/ui.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/pkg/utils.py` & `pyatlan-2.2.2/pyatlan/pkg/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/pkg/widgets.py` & `pyatlan-2.2.2/pyatlan/pkg/widgets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan/utils.py` & `pyatlan-2.2.2/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/pyatlan.egg-info/PKG-INFO` & `pyatlan-2.2.2/pyatlan.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 2.2.1
+Version: 2.2.2
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: requests>=2.24
-Requires-Dist: pydantic~=2.6.1
+Requires-Dist: pydantic<3.0.0,>=2.0.0
 Requires-Dist: jinja2==3.1.4
 Requires-Dist: networkx>=3.1
 Requires-Dist: tenacity==8.2.3
 
 <!-- SPDX-License-Identifier: CC-BY-4.0 -->
 <!-- Copyright 2022 Atlan Pte. Ltd. -->
```

### Comparing `pyatlan-2.2.1/pyatlan.egg-info/SOURCES.txt` & `pyatlan-2.2.2/pyatlan.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -335,23 +335,26 @@
 pyatlan/model/assets/tableau_metric.py
 pyatlan/model/assets/tableau_project.py
 pyatlan/model/assets/tableau_site.py
 pyatlan/model/assets/tableau_workbook.py
 pyatlan/model/assets/tableau_worksheet.py
 pyatlan/model/assets/tag.py
 pyatlan/model/assets/tag_attachment.py
+pyatlan/model/assets/task.py
 pyatlan/model/assets/thoughtspot.py
 pyatlan/model/assets/thoughtspot_answer.py
 pyatlan/model/assets/thoughtspot_column.py
 pyatlan/model/assets/thoughtspot_dashlet.py
 pyatlan/model/assets/thoughtspot_liveboard.py
 pyatlan/model/assets/thoughtspot_table.py
 pyatlan/model/assets/thoughtspot_view.py
 pyatlan/model/assets/thoughtspot_worksheet.py
 pyatlan/model/assets/view.py
+pyatlan/model/assets/workflow.py
+pyatlan/model/assets/workflow_run.py
 pyatlan/model/fields/__init__.py
 pyatlan/model/fields/atlan_fields.py
 pyatlan/model/packages/__init__.py
 pyatlan/model/packages/big_query_crawler.py
 pyatlan/model/packages/confluent_kafka_crawler.py
 pyatlan/model/packages/dbt_crawler.py
 pyatlan/model/packages/dynamo_d_b_crawler.py
@@ -381,24 +384,26 @@
 tests/__init__.py
 tests/integration/__init__.py
 tests/integration/adls_asset_test.py
 tests/integration/admin_test.py
 tests/integration/airflow_asset_test.py
 tests/integration/api_asset_test.py
 tests/integration/atlan_tag_test.py
+tests/integration/azure_event_hub_asset_test.py
 tests/integration/client.py
 tests/integration/conftest.py
 tests/integration/connection_test.py
 tests/integration/custom_metadata_test.py
 tests/integration/custom_package_test.py
 tests/integration/data_mesh_test.py
 tests/integration/data_studio_asset_test.py
 tests/integration/file_test.py
 tests/integration/gcs_asset_test.py
 tests/integration/glossary_test.py
+tests/integration/kafka_asset_test.py
 tests/integration/lineage_test.py
 tests/integration/owner_propagator_cfg.py
 tests/integration/persona_test.py
 tests/integration/preset_asset_test.py
 tests/integration/purpose_test.py
 tests/integration/query_parser_test.py
 tests/integration/requests_test.py
@@ -436,16 +441,18 @@
 tests/unit/test_workflow_client.py
 tests/unit/model/__init__.py
 tests/unit/model/a_d_l_s_account_test.py
 tests/unit/model/a_d_l_s_container_test.py
 tests/unit/model/a_d_l_s_object_test.py
 tests/unit/model/a_p_i_path_test.py
 tests/unit/model/a_p_i_spec_test.py
-tests/unit/model/airflow_dag.py
-tests/unit/model/airflow_task.py
+tests/unit/model/airflow_dag_test.py
+tests/unit/model/airflow_task_test.py
+tests/unit/model/azure_event_consumer_group_test.py
+tests/unit/model/azure_event_hub_test.py
 tests/unit/model/badge_condition_test.py
 tests/unit/model/badge_test.py
 tests/unit/model/column_process_test.py
 tests/unit/model/column_test.py
 tests/unit/model/connection_test.py
 tests/unit/model/constants.py
 tests/unit/model/data_domain_test.py
@@ -454,14 +461,16 @@
 tests/unit/model/database_test.py
 tests/unit/model/file_test.py
 tests/unit/model/gcs_bucket_test.py
 tests/unit/model/gcs_object_test.py
 tests/unit/model/glossary_category_test.py
 tests/unit/model/glossary_term_test.py
 tests/unit/model/glossary_test.py
+tests/unit/model/kafka_consumer_group_test.py
+tests/unit/model/kafka_topic_test.py
 tests/unit/model/materialised_view_test.py
 tests/unit/model/preset_chart_test.py
 tests/unit/model/preset_dashboard_test.py
 tests/unit/model/preset_dataset_test.py
 tests/unit/model/preset_workspace_test.py
 tests/unit/model/process_test.py
 tests/unit/model/readme_test.py
```

### Comparing `pyatlan-2.2.1/setup.py` & `pyatlan-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/adls_asset_test.py` & `pyatlan-2.2.2/tests/integration/adls_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/admin_test.py` & `pyatlan-2.2.2/tests/integration/admin_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/airflow_asset_test.py` & `pyatlan-2.2.2/tests/integration/airflow_asset_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+# Copyright 2024 Atlan Pte. Ltd.
 from typing import Generator
 
 import pytest
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import AirflowDag, AirflowTask, Connection
 from pyatlan.model.core import Announcement
```

### Comparing `pyatlan-2.2.1/tests/integration/api_asset_test.py` & `pyatlan-2.2.2/tests/integration/api_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/atlan_tag_test.py` & `pyatlan-2.2.2/tests/integration/atlan_tag_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/client.py` & `pyatlan-2.2.2/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/connection_test.py` & `pyatlan-2.2.2/tests/integration/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/custom_metadata_test.py` & `pyatlan-2.2.2/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/custom_package_test.py` & `pyatlan-2.2.2/tests/integration/custom_package_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/data_mesh_test.py` & `pyatlan-2.2.2/tests/integration/data_mesh_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/data_studio_asset_test.py` & `pyatlan-2.2.2/tests/integration/data_studio_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/file_test.py` & `pyatlan-2.2.2/tests/integration/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/gcs_asset_test.py` & `pyatlan-2.2.2/tests/integration/gcs_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/glossary_test.py` & `pyatlan-2.2.2/tests/integration/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/lineage_test.py` & `pyatlan-2.2.2/tests/integration/lineage_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/owner_propagator_cfg.py` & `pyatlan-2.2.2/tests/integration/owner_propagator_cfg.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/persona_test.py` & `pyatlan-2.2.2/tests/integration/persona_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/preset_asset_test.py` & `pyatlan-2.2.2/tests/integration/preset_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/purpose_test.py` & `pyatlan-2.2.2/tests/integration/purpose_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/query_parser_test.py` & `pyatlan-2.2.2/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/requests_test.py` & `pyatlan-2.2.2/tests/integration/requests_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/s3_asset_test.py` & `pyatlan-2.2.2/tests/integration/s3_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/test_client.py` & `pyatlan-2.2.2/tests/integration/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,14 +431,42 @@
     assert glossary_term.atlan_tags
     assert len(glossary_term.atlan_tags) == 1
     classification = glossary_term.atlan_tags[0]
     assert str(classification.type_name) == CLASSIFICATION_NAME
 
 
 @pytest.mark.order(after="test_add_classification")
+def test_include_atlan_tag_names(client: AtlanClient, term1: AtlasGlossaryTerm):
+    assert term1 and term1.qualified_name
+    query = Term.with_type_name(term1.type_name) + Term.with_name(term1.name)
+    request = IndexSearchRequest(
+        dsl=DSL(query=query), exclude_atlan_tags=True, include_atlan_tag_names=False
+    )
+    response = client.asset.search(criteria=request)
+
+    # Ensure classification names are not present
+    assert response
+    assert response.current_page() and len(response.current_page()) == 1
+    assert response.current_page()[0].guid == term1.guid
+    assert response.current_page()[0].classification_names is None
+
+    request = IndexSearchRequest(
+        dsl=DSL(query=query), exclude_atlan_tags=True, include_atlan_tag_names=True
+    )
+    response = client.asset.search(criteria=request)
+
+    # Ensure classification names are present
+    assert response
+    assert response.current_page() and len(response.current_page()) == 1
+    assert response.current_page()[0].guid == term1.guid
+    classification_names = response.current_page()[0].classification_names
+    assert classification_names and len(classification_names) == 1
+
+
+@pytest.mark.order(after="test_add_classification")
 def test_remove_classification(client: AtlanClient, term1: AtlasGlossaryTerm):
     assert term1.qualified_name
     client.asset.remove_atlan_tag(
         AtlasGlossaryTerm, term1.qualified_name, CLASSIFICATION_NAME
     )
     glossary_term = client.asset.get_by_guid(term1.guid, asset_type=AtlasGlossaryTerm)
     assert not glossary_term.atlan_tags
```

### Comparing `pyatlan-2.2.1/tests/integration/test_file_client.py` & `pyatlan-2.2.2/tests/integration/test_file_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/test_index_search.py` & `pyatlan-2.2.2/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/test_sql_assets.py` & `pyatlan-2.2.2/tests/integration/test_sql_assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/test_sso_client.py` & `pyatlan-2.2.2/tests/integration/test_sso_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def delete_group(client: AtlanClient, guid: str) -> None:
     client.group.purge(guid)
 
 
 def delete_sso_mapping(client: AtlanClient, group_map_id: str) -> None:
     response = client.sso.delete_group_mapping(
-        sso_alias=AtlanSSO.AZURE_AD, group_map_id=group_map_id
+        sso_alias=AtlanSSO.JUMPCLOUD, group_map_id=group_map_id
     )
     assert response is None
 
 
 @pytest.fixture(scope="module")
 def group(client: AtlanClient) -> Generator[AtlanGroup, None, None]:
     to_create = AtlanGroup.create(GROUP_NAME)
@@ -49,20 +49,20 @@
 @pytest.fixture(scope="module")
 def sso_mapping(
     client: AtlanClient, group: AtlanGroup
 ) -> Generator[SSOMapper, None, None]:
     assert group
     assert group.id
     response = client.sso.create_group_mapping(
-        sso_alias=AtlanSSO.AZURE_AD, atlan_group=group, sso_group_name=SSO_GROUP_NAME
+        sso_alias=AtlanSSO.JUMPCLOUD, atlan_group=group, sso_group_name=SSO_GROUP_NAME
     )
     assert response
 
     azure_group_mapping = None
-    sso_mappings = client.sso.get_all_group_mappings(sso_alias=AtlanSSO.AZURE_AD)
+    sso_mappings = client.sso.get_all_group_mappings(sso_alias=AtlanSSO.JUMPCLOUD)
     for mapping in sso_mappings:
         if (
             group.id
             and group.id in str(mapping.name)
             and mapping.identity_provider_mapper == SSOClient.IDP_GROUP_MAPPER
         ):
             azure_group_mapping = mapping
@@ -73,15 +73,15 @@
 
 
 def _assert_sso_group_mapping(
     group: AtlanGroup, sso_mapping: SSOMapper, is_updated: bool = False
 ):
     assert sso_mapping
     assert sso_mapping.id
-    assert sso_mapping.identity_provider_alias == AtlanSSO.AZURE_AD
+    assert sso_mapping.identity_provider_alias == AtlanSSO.JUMPCLOUD
     assert sso_mapping.identity_provider_mapper == SSOClient.IDP_GROUP_MAPPER
     assert sso_mapping.config.attributes == "[]"
     assert sso_mapping.config.group_name == group.name
     assert sso_mapping.config.attribute_values_regex is None
     assert sso_mapping.config.attribute_friendly_name is None
 
     assert sso_mapping.config.sync_mode == SSOClient.GROUP_MAPPER_SYNC_MODE
@@ -111,15 +111,15 @@
     sso_mapping: SSOMapper,
 ):
     assert group
     assert sso_mapping
 
     with pytest.raises(InvalidRequestError) as err:
         client.sso.create_group_mapping(
-            sso_alias=AtlanSSO.AZURE_AD,
+            sso_alias=AtlanSSO.JUMPCLOUD,
             atlan_group=group,
             sso_group_name=SSO_GROUP_NAME,
         )
     assert (
         f"ATLAN-PYTHON-400-058 SSO group mapping already exists between "
         f"{group.alias} (Atlan group) <-> {SSO_GROUP_NAME} (SSO group)"
     ) in str(err.value)
@@ -135,15 +135,15 @@
 ):
     assert group
     assert sso_mapping
     assert sso_mapping.id
     time.sleep(5)
 
     retrieved_sso_mapping = client.sso.get_group_mapping(
-        sso_alias=AtlanSSO.AZURE_AD, group_map_id=sso_mapping.id
+        sso_alias=AtlanSSO.JUMPCLOUD, group_map_id=sso_mapping.id
     )
     _assert_sso_group_mapping(group, retrieved_sso_mapping)
 
 
 @pytest.mark.order(after="test_sso_retrieve_group_mapping")
 def test_sso_retrieve_all_group_mappings(
     client: AtlanClient,
@@ -151,42 +151,42 @@
     sso_mapping: SSOMapper,
 ):
     assert group
     assert group.id
     assert sso_mapping
     time.sleep(5)
 
-    retrieved_mappings = client.sso.get_all_group_mappings(sso_alias=AtlanSSO.AZURE_AD)
+    retrieved_mappings = client.sso.get_all_group_mappings(sso_alias=AtlanSSO.JUMPCLOUD)
     assert len(retrieved_mappings) >= 1
     mapping_found = False
     for mapping in retrieved_mappings:
         if (
             group.id in str(mapping.name)
             and mapping.identity_provider_mapper == SSOClient.IDP_GROUP_MAPPER
         ):
             mapping_found = True
             _assert_sso_group_mapping(group, mapping)
             break
     if not mapping_found:
         pytest.fail(
             f"{group.alias} (Atlan Group) <-> ({sso_mapping.config.attribute_value}) "
-            f"{AtlanSSO.AZURE_AD} SSO group mapping not found."
+            f"{AtlanSSO.JUMPCLOUD} SSO group mapping not found."
         )
 
 
 @pytest.mark.order(after="test_sso_retrieve_all_group_mappings")
 def test_update_group_mapping(
     client: AtlanClient,
     group: AtlanGroup,
     sso_mapping: SSOMapper,
 ):
     assert group
     assert sso_mapping
     assert sso_mapping.id
 
     updated_mapping = client.sso.update_group_mapping(
-        sso_alias=AtlanSSO.AZURE_AD,
+        sso_alias=AtlanSSO.JUMPCLOUD,
         atlan_group=group,
         group_map_id=sso_mapping.id,
         sso_group_name=SSO_GROUP_NAME_UPDATED,
     )
     _assert_sso_group_mapping(group, updated_mapping, True)
```

### Comparing `pyatlan-2.2.1/tests/integration/test_task_client.py` & `pyatlan-2.2.2/tests/integration/test_task_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/test_workflow_client.py` & `pyatlan-2.2.2/tests/integration/test_workflow_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/integration/utils.py` & `pyatlan-2.2.2/tests/integration/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/conftest.py` & `pyatlan-2.2.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/constants.py` & `pyatlan-2.2.2/tests/unit/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pyatlan.model.assets import AtlasGlossary
 from pyatlan.model.enums import AtlanWorkflowPhase
 from pyatlan.model.workflow import (
+    ScheduleQueriesSearchRequest,
     WorkflowMetadata,
     WorkflowResponse,
     WorkflowSchedule,
     WorkflowSpec,
 )
 
 TEST_ASSET_CLIENT_METHODS = {
@@ -497,14 +498,15 @@
         (
             ["test-url", None],
             "none is not an allowed value",
         ),
     ],
 }
 
+
 TEST_WORKFLOW_CLIENT_METHODS = {
     "run": [
         (["abc"], "value is not a valid dict"),
         ([None], "none is not an allowed value"),
     ],
     "rerun": [
         (["abc"], "value is not a valid enumeration member"),
@@ -560,14 +562,42 @@
         ([[123]], "value is not a valid enumeration member"),
         ([None], "none is not an allowed value"),
     ],
     "get_scheduled_run": [
         ([[123]], "str type expected"),
         ([None], "none is not an allowed value"),
     ],
+    "find_schedule_query": [
+        ([[123], 10], "saved_query_id\n  str type expected"),
+        ([None, 10], "none is not an allowed value"),
+        (["test-query-id", [123]], "max_results\n  value is not a valid integer"),
+        (["test-query-id", None], "none is not an allowed value"),
+    ],
+    "re_run_schedule_query": [
+        ([[123]], "schedule_query_id\n  str type expected"),
+        ([None], "none is not an allowed value"),
+    ],
+    "find_schedule_query_between": [
+        ([[123], True], "value is not a valid dict"),
+        ([None, True], "none is not an allowed value"),
+        (
+            [ScheduleQueriesSearchRequest(start_date="start", end_date="end"), [123]],
+            "missed\n  value could not be parsed to a boolean",
+        ),
+        (
+            [ScheduleQueriesSearchRequest(start_date="start", end_date="end"), None],
+            "none is not an allowed value",
+        ),
+    ],
+    "update_owner": [
+        ([[123], 10], "workflow_name\n  str type expected"),
+        ([None, 10], "none is not an allowed value"),
+        (["test-workflow", [123]], "username\n  str type expected"),
+        (["test-workflow", None], "none is not an allowed value"),
+    ],
 }
 
 APPLICABLE_GLOSSARIES = "applicable_glossaries"
 
 APPLICABLE_CONNECTIONS = "applicable_connections"
 
 APPLICABLE_ENTITY_TYPES = "applicable_entity_types"
```

### Comparing `pyatlan-2.2.1/tests/unit/model/a_d_l_s_account_test.py` & `pyatlan-2.2.2/tests/unit/model/a_d_l_s_account_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/a_d_l_s_container_test.py` & `pyatlan-2.2.2/tests/unit/model/a_d_l_s_container_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/a_d_l_s_object_test.py` & `pyatlan-2.2.2/tests/unit/model/a_d_l_s_object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/a_p_i_path_test.py` & `pyatlan-2.2.2/tests/unit/model/a_p_i_path_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/a_p_i_spec_test.py` & `pyatlan-2.2.2/tests/unit/model/a_p_i_spec_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/airflow_dag.py` & `pyatlan-2.2.2/tests/unit/model/airflow_dag_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/airflow_task.py` & `pyatlan-2.2.2/tests/unit/model/airflow_task_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/badge_condition_test.py` & `pyatlan-2.2.2/tests/unit/model/badge_condition_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/badge_test.py` & `pyatlan-2.2.2/tests/unit/model/badge_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/column_process_test.py` & `pyatlan-2.2.2/tests/unit/model/column_process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/column_test.py` & `pyatlan-2.2.2/tests/unit/model/column_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/connection_test.py` & `pyatlan-2.2.2/tests/unit/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/constants.py` & `pyatlan-2.2.2/tests/unit/model/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -102,7 +102,36 @@
 )
 CP_QUALIFIED_NAME = f"{CP_CONNECTION_QUALIFIED_NAME}/{CP_PROCESS_ID}"
 AIRFLOW_DAG_NAME = "test-airflow-dag"
 AIRFLOW_CONNECTION_QUALIFIED_NAME = "default/airflow/123456789"
 AIRFLOW_DAG_QUALIFIED_NAME = f"{AIRFLOW_CONNECTION_QUALIFIED_NAME}/{AIRFLOW_DAG_NAME}"
 AIRFLOW_TASK_NAME = "test-airflow-task"
 AIRFLOW_TASK_QUALIFIED_NAME = f"{AIRFLOW_DAG_QUALIFIED_NAME}/{AIRFLOW_TASK_NAME}"
+KAFKA_TOPIC_NAME = "test-kafka-topic"
+KAFKA_TOPIC_NAME_2 = f"{KAFKA_TOPIC_NAME}-2"
+KAFKA_CONNECTION_QUALIFIED_NAME = "default/kafka/123456789"
+KAFKA_TOPIC_QUALIFIED_NAME = (
+    f"{KAFKA_CONNECTION_QUALIFIED_NAME}/topic/{KAFKA_TOPIC_NAME}"
+)
+KAFKA_TOPIC_QUALIFIED_NAMES = [
+    KAFKA_TOPIC_QUALIFIED_NAME,
+    f"{KAFKA_CONNECTION_QUALIFIED_NAME}/topic/{KAFKA_TOPIC_NAME_2}",
+]
+KAFKA_CONSUMER_GROUP_NAME = "test-kafka-cg"
+KAFKA_CONSUMER_GROUP_QUALIFIED_NAME = (
+    f"{KAFKA_CONNECTION_QUALIFIED_NAME}/consumer-group/{KAFKA_CONSUMER_GROUP_NAME}"
+)
+EVENT_HUB_NAME = "test-event-hub"
+EVENT_HUB_NAME_2 = f"{EVENT_HUB_NAME}-2"
+EVENT_HUB_CONNECTION_QUALIFIED_NAME = "default/azure-event-hub/123456789"
+EVENT_HUB_QUALIFIED_NAME = (
+    f"{EVENT_HUB_CONNECTION_QUALIFIED_NAME}/topic/{EVENT_HUB_NAME}"
+)
+EVENT_HUB_QUALIFIED_NAMES = [
+    EVENT_HUB_QUALIFIED_NAME,
+    f"{EVENT_HUB_CONNECTION_QUALIFIED_NAME}/topic/{EVENT_HUB_NAME_2}",
+]
+EVENT_HUB_CONSUMER_GROUP_NAME = "test-event-cg"
+EVENT_HUB_CONSUMER_GROUP_QUALIFIED_NAME = (
+    f"{EVENT_HUB_CONNECTION_QUALIFIED_NAME}/consumer-group"
+    f"/{EVENT_HUB_NAME}/{EVENT_HUB_CONSUMER_GROUP_NAME}"
+)
```

### Comparing `pyatlan-2.2.1/tests/unit/model/data_domain_test.py` & `pyatlan-2.2.2/tests/unit/model/data_domain_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/data_product_test.py` & `pyatlan-2.2.2/tests/unit/model/data_product_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/data_studio_asset_test.py` & `pyatlan-2.2.2/tests/unit/model/data_studio_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/database_test.py` & `pyatlan-2.2.2/tests/unit/model/database_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/fields/atlan_fields_test.py` & `pyatlan-2.2.2/tests/unit/model/fields/atlan_fields_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/file_test.py` & `pyatlan-2.2.2/tests/unit/model/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/gcs_bucket_test.py` & `pyatlan-2.2.2/tests/unit/model/gcs_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/gcs_object_test.py` & `pyatlan-2.2.2/tests/unit/model/gcs_object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/glossary_category_test.py` & `pyatlan-2.2.2/tests/unit/model/glossary_category_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
     category.parent_category = None
     assert category.parent_category is None
     assert category.relationship_attributes == {"parentCategory": None}
 
 
 def test_trim_to_required():
-    sut = AtlasGlossaryCategory.create_for_modification(
+    sut = AtlasGlossaryCategory.updater(
         qualified_name=GLOSSARY_CATEGORY_QUALIFIED_NAME,
         name=GLOSSARY_CATEGORY_NAME,
         glossary_guid=GLOSSARY_GUID,
     ).trim_to_required()
 
     assert sut.name == GLOSSARY_CATEGORY_NAME
     assert sut.qualified_name == GLOSSARY_CATEGORY_QUALIFIED_NAME
@@ -129,15 +129,15 @@
 
 
 @pytest.mark.parametrize(
     "anchor",
     [(None), (AtlasGlossary())],
 )
 def test_trim_to_required_raises_value_error_when_anchor_is_none(anchor):
-    sut = AtlasGlossaryCategory.create_for_modification(
+    sut = AtlasGlossaryCategory.updater(
         qualified_name=GLOSSARY_CATEGORY_QUALIFIED_NAME,
         name=GLOSSARY_CATEGORY_NAME,
         glossary_guid=GLOSSARY_GUID,
     )
     sut.anchor = anchor
 
     with pytest.raises(ValueError, match="anchor.guid must be available"):
```

### Comparing `pyatlan-2.2.1/tests/unit/model/glossary_term_test.py` & `pyatlan-2.2.2/tests/unit/model/glossary_term_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         (ANCHOR, None, None, None),
         (None, GLOSSARY_QUALIFIED_NAME, None, None),
         (
             None,
             None,
             GLOSSARY_GUID,
             [
-                AtlasGlossaryCategory.create_for_modification(
+                AtlasGlossaryCategory.updater(
                     qualified_name="123", name="Category", glossary_guid=GLOSSARY_GUID
                 )
             ],
         ),
     ],
 )
 def test_create(
```

### Comparing `pyatlan-2.2.1/tests/unit/model/glossary_test.py` & `pyatlan-2.2.2/tests/unit/model/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/materialised_view_test.py` & `pyatlan-2.2.2/tests/unit/model/materialised_view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/preset_chart_test.py` & `pyatlan-2.2.2/tests/unit/model/preset_chart_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/preset_dashboard_test.py` & `pyatlan-2.2.2/tests/unit/model/preset_dashboard_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/preset_dataset_test.py` & `pyatlan-2.2.2/tests/unit/model/preset_dataset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/preset_workspace_test.py` & `pyatlan-2.2.2/tests/unit/model/preset_workspace_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/process_test.py` & `pyatlan-2.2.2/tests/unit/model/process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/readme_test.py` & `pyatlan-2.2.2/tests/unit/model/readme_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/s3_bucket_test.py` & `pyatlan-2.2.2/tests/unit/model/s3_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/s3object_test.py` & `pyatlan-2.2.2/tests/unit/model/s3object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/schema_test.py` & `pyatlan-2.2.2/tests/unit/model/schema_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/table_test.py` & `pyatlan-2.2.2/tests/unit/model/table_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/model/view_test.py` & `pyatlan-2.2.2/tests/unit/model/view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/pkg/conftest.py` & `pyatlan-2.2.2/tests/unit/pkg/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/pkg/test_models.py` & `pyatlan-2.2.2/tests/unit/pkg/test_models.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/pkg/test_ui.py` & `pyatlan-2.2.2/tests/unit/pkg/test_ui.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/pkg/test_utils.py` & `pyatlan-2.2.2/tests/unit/pkg/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/pkg/test_widgets.py` & `pyatlan-2.2.2/tests/unit/pkg/test_widgets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_atlan_tag_name.py` & `pyatlan-2.2.2/tests/unit/test_atlan_tag_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_client.py` & `pyatlan-2.2.2/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_core.py` & `pyatlan-2.2.2/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_credential_client.py` & `pyatlan-2.2.2/tests/unit/test_credential_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_custom_metadata.py` & `pyatlan-2.2.2/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_deprecated.py` & `pyatlan-2.2.2/tests/unit/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_events.py` & `pyatlan-2.2.2/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_file_client.py` & `pyatlan-2.2.2/tests/unit/test_file_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_glossary_term.py` & `pyatlan-2.2.2/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_lineage.py` & `pyatlan-2.2.2/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_model.py` & `pyatlan-2.2.2/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_packages.py` & `pyatlan-2.2.2/tests/unit/test_packages.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_query_client.py` & `pyatlan-2.2.2/tests/unit/test_query_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_search_model.py` & `pyatlan-2.2.2/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_sso_client.py` & `pyatlan-2.2.2/tests/unit/test_sso_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_structs.py` & `pyatlan-2.2.2/tests/unit/test_structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_task_client.py` & `pyatlan-2.2.2/tests/unit/test_task_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_typedef_model.py` & `pyatlan-2.2.2/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_utils.py` & `pyatlan-2.2.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.2.1/tests/unit/test_workflow_client.py` & `pyatlan-2.2.2/tests/unit/test_workflow_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,25 @@
 from unittest.mock import Mock, patch
 
 import pytest
 from pydantic.v1 import ValidationError
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.client.common import ApiCaller
-from pyatlan.client.constants import WORKFLOW_INDEX_SEARCH
+from pyatlan.client.constants import (
+    SCHEDULE_QUERY_WORKFLOWS_MISSED,
+    SCHEDULE_QUERY_WORKFLOWS_SEARCH,
+    WORKFLOW_INDEX_SEARCH,
+)
 from pyatlan.client.workflow import WorkflowClient
 from pyatlan.errors import InvalidRequestError
 from pyatlan.model.enums import AtlanWorkflowPhase, WorkflowPackage
 from pyatlan.model.workflow import (
     PackageParameter,
+    ScheduleQueriesSearchRequest,
     Workflow,
     WorkflowMetadata,
     WorkflowResponse,
     WorkflowRunResponse,
     WorkflowSchedule,
     WorkflowScheduleResponse,
     WorkflowScheduleSpec,
@@ -155,31 +160,31 @@
 def update_response() -> WorkflowResponse:
     return WorkflowResponse(
         metadata=WorkflowMetadata(name="name", namespace="namespace"),
         spec=WorkflowSpec(),
     )
 
 
+@pytest.mark.parametrize("method, params", TEST_WORKFLOW_CLIENT_METHODS.items())
+def test_workflow_client_methods_validation_error(method, params):
+    client_method = getattr(AtlanClient().workflow, method)
+    for param_values, error_msg in params:
+        with pytest.raises(ValidationError, match=error_msg):
+            client_method(*param_values)
+
+
 @pytest.mark.parametrize("api_caller", ["abc", None])
 def test_init_when_wrong_class_raises_exception(api_caller):
     with pytest.raises(
         InvalidRequestError,
         match="ATLAN-PYTHON-400-048 Invalid parameter type for client should be ApiCaller",
     ):
         WorkflowClient(api_caller)
 
 
-@pytest.mark.parametrize("method, params", TEST_WORKFLOW_CLIENT_METHODS.items())
-def test_workflow_client_methods_validation_error(method, params):
-    client_method = getattr(AtlanClient().workflow, method)
-    for param_values, error_msg in params:
-        with pytest.raises(ValidationError, match=error_msg):
-            client_method(*param_values)
-
-
 def test_find_by_type(client: WorkflowClient, mock_api_caller):
     raw_json = {"shards": {"dummy": None}, "hits": {"total": {"dummy": None}}}
     mock_api_caller._call_api.return_value = raw_json
 
     assert client.find_by_type(prefix=WorkflowPackage.FIVETRAN) == []
     mock_api_caller._call_api.called_once()
     assert mock_api_caller._call_api.call_args.args[0] == WORKFLOW_INDEX_SEARCH
@@ -350,14 +355,27 @@
     mock_api_caller._call_api.return_value = update_response.dict()
     response = client.update(workflow=search_result.to_workflow())
     assert response == update_response
     assert mock_api_caller._call_api.call_count == 1
     mock_api_caller.reset_mock()
 
 
+def test_workflow_update_owner(
+    client: WorkflowClient,
+    mock_api_caller,
+    workflow_response: WorkflowResponse,
+):
+    mock_api_caller._call_api.return_value = workflow_response.dict()
+    response = client.update_owner(workflow_name="test-workflow", username="test-owner")
+
+    assert mock_api_caller._call_api.call_count == 1
+    assert response == WorkflowResponse(**workflow_response.dict())
+    mock_api_caller.reset_mock()
+
+
 def test_workflow_get_runs(
     client: WorkflowClient,
     mock_api_caller,
     search_response: WorkflowSearchResponse,
 ):
     mock_api_caller._call_api.return_value = search_response.dict()
     response = client.get_runs(
@@ -426,14 +444,104 @@
     response = client.add_schedule(workflow=search_result, workflow_schedule=schedule)
 
     assert mock_api_caller._call_api.call_count == 1
     assert response == WorkflowResponse(**workflow_response.dict())
     mock_api_caller.reset_mock()
 
 
+def test_workflow_find_schedule_query_between(
+    client: WorkflowClient, mock_api_caller, workflow_run_response: WorkflowRunResponse
+):
+    mock_api_caller._call_api.return_value = [workflow_run_response]
+    response = client.find_schedule_query_between(
+        ScheduleQueriesSearchRequest(
+            start_date="2024-05-03T16:30:00.000+05:30",
+            end_date="2024-05-05T00:59:00.000+05:30",
+        )
+    )
+
+    assert mock_api_caller._call_api.call_count == 1
+    assert (
+        response
+        and len(response) == 1
+        and response[0] == WorkflowRunResponse(**workflow_run_response.dict())
+    )
+    # Ensure it is called by the correct API endpoint
+    assert (
+        mock_api_caller._call_api.call_args[0][0].path
+        == SCHEDULE_QUERY_WORKFLOWS_SEARCH.path
+    )
+    mock_api_caller.reset_mock()
+
+    # Missed schedule query workflows
+    mock_api_caller._call_api.return_value = [workflow_run_response]
+    response = client.find_schedule_query_between(
+        ScheduleQueriesSearchRequest(
+            start_date="2024-05-03T16:30:00.000+05:30",
+            end_date="2024-05-05T00:59:00.000+05:30",
+        ),
+        missed=True,
+    )
+
+    assert mock_api_caller._call_api.call_count == 1
+    # Ensure it is called by the correct API endpoint
+    assert (
+        mock_api_caller._call_api.call_args[0][0].path
+        == SCHEDULE_QUERY_WORKFLOWS_MISSED.path
+    )
+    assert (
+        response
+        and len(response) == 1
+        and response[0] == WorkflowRunResponse(**workflow_run_response.dict())
+    )
+    mock_api_caller.reset_mock()
+
+    # None response
+    mock_api_caller._call_api.return_value = None
+    response = client.find_schedule_query_between(
+        ScheduleQueriesSearchRequest(
+            start_date="2024-05-03T16:30:00.000+05:30",
+            end_date="2024-05-05T00:59:00.000+05:30",
+        )
+    )
+
+    assert mock_api_caller._call_api.call_count == 1
+    assert response is None
+    mock_api_caller.reset_mock()
+
+
+def test_workflow_find_schedule_query(
+    client: WorkflowClient,
+    mock_api_caller,
+    search_response: WorkflowSearchResponse,
+    search_result: WorkflowSearchResult,
+):
+    mock_api_caller._call_api.return_value = search_response.dict()
+    response = client.find_schedule_query(
+        saved_query_id="test-query-id", max_results=50
+    )
+
+    assert len(response) == 1
+    assert mock_api_caller._call_api.call_count == 1
+    assert response[0] == WorkflowSearchResult(**search_result.dict())
+    mock_api_caller.reset_mock()
+
+
+def test_workflow_rerun_schedule_query_workflow(
+    client,
+    mock_api_caller,
+    workflow_run_response: WorkflowRunResponse,
+):
+    mock_api_caller._call_api.return_value = workflow_run_response.dict()
+    response = client.re_run_schedule_query(schedule_query_id="test-query-id")
+
+    assert mock_api_caller._call_api.call_count == 1
+    assert response == WorkflowRunResponse(**workflow_run_response.dict())
+
+
 def test_workflow_remove_schedule(
     client: WorkflowClient,
     workflow_response: WorkflowResponse,
     search_response: WorkflowSearchResponse,
     search_result: WorkflowSearchResult,
     mock_api_caller,
 ):
```

