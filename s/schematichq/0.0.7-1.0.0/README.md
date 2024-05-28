# Comparing `tmp/schematichq-0.0.7.tar.gz` & `tmp/schematichq-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schematichq-0.0.7.tar", max compression
+gzip compressed data, was "schematichq-1.0.0.tar", max compression
```

## Comparing `schematichq-0.0.7.tar` & `schematichq-1.0.0.tar`

### file list

```diff
@@ -1,302 +1,308 @@
--rw-r--r--   0        0        0     3922 2024-05-16 14:53:08.847939 schematichq-0.0.7/README.md
--rw-r--r--   0        0        0      597 2024-05-16 14:53:08.847939 schematichq-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    17054 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/__init__.py
--rw-r--r--   0        0        0     1259 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/__init__.py
--rw-r--r--   0        0        0    93187 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/client.py
--rw-r--r--   0        0        0     1909 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/__init__.py
--rw-r--r--   0        0        0     1325 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/count_api_keys_params.py
--rw-r--r--   0        0        0     1326 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/count_api_keys_response.py
--rw-r--r--   0        0        0     1356 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/count_api_requests_params.py
--rw-r--r--   0        0        0     1342 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/count_api_requests_response.py
--rw-r--r--   0        0        0     1318 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/create_api_key_response.py
--rw-r--r--   0        0        0      213 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/create_environment_request_body_environment_type.py
--rw-r--r--   0        0        0     1337 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/create_environment_response.py
--rw-r--r--   0        0        0     1285 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/delete_api_key_response.py
--rw-r--r--   0        0        0     1290 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/delete_environment_response.py
--rw-r--r--   0        0        0     1296 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/get_api_key_response.py
--rw-r--r--   0        0        0     1322 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/get_api_request_response.py
--rw-r--r--   0        0        0     1315 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/get_environment_response.py
--rw-r--r--   0        0        0     1324 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/list_api_keys_params.py
--rw-r--r--   0        0        0     1418 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/list_api_keys_response.py
--rw-r--r--   0        0        0     1355 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/list_api_requests_params.py
--rw-r--r--   0        0        0     1469 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/list_api_requests_response.py
--rw-r--r--   0        0        0     1299 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/update_api_key_response.py
--rw-r--r--   0        0        0      213 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/update_environment_request_body_environment_type.py
--rw-r--r--   0        0        0     1318 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/accounts/types/update_environment_response.py
--rw-r--r--   0        0        0     6614 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/base_client.py
--rw-r--r--   0        0        0      357 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/billing/__init__.py
--rw-r--r--   0        0        0    25969 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/billing/client.py
--rw-r--r--   0        0        0      479 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/billing/types/__init__.py
--rw-r--r--   0        0        0     1311 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/billing/types/list_products_params.py
--rw-r--r--   0        0        0     1445 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/billing/types/list_products_response.py
--rw-r--r--   0        0        0     1331 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/billing/types/upsert_billing_product_response.py
--rw-r--r--   0        0        0     1351 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/billing/types/upsert_billing_subscription_response.py
--rw-r--r--   0        0        0      241 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/client.py
--rw-r--r--   0        0        0     3327 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/__init__.py
--rw-r--r--   0        0        0   237379 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/client.py
--rw-r--r--   0        0        0     5169 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/__init__.py
--rw-r--r--   0        0        0     1413 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/count_companies_params.py
--rw-r--r--   0        0        0     1333 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/count_companies_response.py
--rw-r--r--   0        0        0     1368 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/count_entity_key_definitions_params.py
--rw-r--r--   0        0        0     1379 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/count_entity_key_definitions_response.py
--rw-r--r--   0        0        0     1412 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/count_entity_trait_definitions_params.py
--rw-r--r--   0        0        0     1387 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/count_entity_trait_definitions_response.py
--rw-r--r--   0        0        0     1391 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/count_users_params.py
--rw-r--r--   0        0        0     1317 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/count_users_response.py
--rw-r--r--   0        0        0     1321 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/create_company_response.py
--rw-r--r--   0        0        0      191 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/create_entity_trait_definition_request_body_entity_type.py
--rw-r--r--   0        0        0      235 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/create_entity_trait_definition_request_body_trait_type.py
--rw-r--r--   0        0        0     1309 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/create_user_response.py
--rw-r--r--   0        0        0     1308 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/delete_company_by_keys_response.py
--rw-r--r--   0        0        0     1296 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/delete_company_membership_response.py
--rw-r--r--   0        0        0     1286 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/delete_company_response.py
--rw-r--r--   0        0        0     1296 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/delete_user_by_keys_response.py
--rw-r--r--   0        0        0     1283 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/delete_user_response.py
--rw-r--r--   0        0        0     1283 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/get_active_company_subscription_params.py
--rw-r--r--   0        0        0     1526 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/get_active_company_subscription_response.py
--rw-r--r--   0        0        0     1318 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/get_company_response.py
--rw-r--r--   0        0        0     1357 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/get_entity_trait_definition_response.py
--rw-r--r--   0        0        0     1313 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/get_entity_trait_values_params.py
--rw-r--r--   0        0        0     1448 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/get_entity_trait_values_response.py
--rw-r--r--   0        0        0     1367 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/get_or_create_company_membership_response.py
--rw-r--r--   0        0        0     1365 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/get_or_create_entity_trait_definition_response.py
--rw-r--r--   0        0        0     1306 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/get_user_response.py
--rw-r--r--   0        0        0     1412 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/list_companies_params.py
--rw-r--r--   0        0        0     1446 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/list_companies_response.py
--rw-r--r--   0        0        0     1318 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/list_company_memberships_params.py
--rw-r--r--   0        0        0     1514 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/list_company_memberships_response.py
--rw-r--r--   0        0        0     1312 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/list_company_plans_params.py
--rw-r--r--   0        0        0     1453 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/list_company_plans_response.py
--rw-r--r--   0        0        0     1367 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/list_entity_key_definitions_params.py
--rw-r--r--   0        0        0     1511 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/list_entity_key_definitions_response.py
--rw-r--r--   0        0        0     1411 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/list_entity_trait_definitions_params.py
--rw-r--r--   0        0        0     1525 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/list_entity_trait_definitions_response.py
--rw-r--r--   0        0        0     1390 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/list_users_params.py
--rw-r--r--   0        0        0     1421 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/list_users_response.py
--rw-r--r--   0        0        0     1208 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/lookup_company_params.py
--rw-r--r--   0        0        0     1367 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/lookup_company_response.py
--rw-r--r--   0        0        0     1205 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/lookup_user_params.py
--rw-r--r--   0        0        0     1346 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/lookup_user_response.py
--rw-r--r--   0        0        0      235 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/update_entity_trait_definition_request_body_trait_type.py
--rw-r--r--   0        0        0     1360 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/update_entity_trait_definition_response.py
--rw-r--r--   0        0        0     1321 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/upsert_company_response.py
--rw-r--r--   0        0        0     1326 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/upsert_company_trait_response.py
--rw-r--r--   0        0        0     1309 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/upsert_user_response.py
--rw-r--r--   0        0        0     1314 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/companies/types/upsert_user_trait_response.py
--rw-r--r--   0        0        0      973 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/core/api_error.py
--rw-r--r--   0        0        0     1496 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/core/jsonable_encoder.py
--rw-r--r--   0        0        0      748 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/core/pydantic_utilities.py
--rw-r--r--   0        0        0     1215 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/core/query_encoder.py
--rw-r--r--   0        0        0      330 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/core/request_options.py
--rw-r--r--   0        0        0     2927 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/__init__.py
--rw-r--r--   0        0        0   153569 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/client.py
--rw-r--r--   0        0        0     4534 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/__init__.py
--rw-r--r--   0        0        0     1486 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/count_company_overrides_params.py
--rw-r--r--   0        0        0     1362 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/count_company_overrides_response.py
--rw-r--r--   0        0        0     1311 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/count_feature_companies_params.py
--rw-r--r--   0        0        0     1362 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/count_feature_companies_response.py
--rw-r--r--   0        0        0     1436 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/count_feature_usage_params.py
--rw-r--r--   0        0        0     1346 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/count_feature_usage_response.py
--rw-r--r--   0        0        0     1307 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/count_feature_users_params.py
--rw-r--r--   0        0        0     1346 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/count_feature_users_response.py
--rw-r--r--   0        0        0     1480 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/count_plan_entitlements_params.py
--rw-r--r--   0        0        0     1362 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/count_plan_entitlements_response.py
--rw-r--r--   0        0        0      222 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/create_company_override_request_body_metric_period.py
--rw-r--r--   0        0        0      215 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/create_company_override_request_body_value_type.py
--rw-r--r--   0        0        0     1335 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/create_company_override_response.py
--rw-r--r--   0        0        0      222 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/create_plan_entitlement_request_body_metric_period.py
--rw-r--r--   0        0        0      215 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/create_plan_entitlement_request_body_value_type.py
--rw-r--r--   0        0        0     1335 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/create_plan_entitlement_response.py
--rw-r--r--   0        0        0     1294 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/delete_company_override_response.py
--rw-r--r--   0        0        0     1294 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/delete_plan_entitlement_response.py
--rw-r--r--   0        0        0     1332 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/get_company_override_response.py
--rw-r--r--   0        0        0     1219 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/get_feature_usage_by_company_params.py
--rw-r--r--   0        0        0     1430 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/get_feature_usage_by_company_response.py
--rw-r--r--   0        0        0     1332 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/get_plan_entitlement_response.py
--rw-r--r--   0        0        0     1485 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/list_company_overrides_params.py
--rw-r--r--   0        0        0     1481 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/list_company_overrides_response.py
--rw-r--r--   0        0        0     1310 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/list_feature_companies_params.py
--rw-r--r--   0        0        0     1478 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/list_feature_companies_response.py
--rw-r--r--   0        0        0     1435 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/list_feature_usage_params.py
--rw-r--r--   0        0        0     1456 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/list_feature_usage_response.py
--rw-r--r--   0        0        0     1306 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/list_feature_users_params.py
--rw-r--r--   0        0        0     1475 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/list_feature_users_response.py
--rw-r--r--   0        0        0     1479 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/list_plan_entitlements_params.py
--rw-r--r--   0        0        0     1481 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/list_plan_entitlements_response.py
--rw-r--r--   0        0        0      222 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/update_company_override_request_body_metric_period.py
--rw-r--r--   0        0        0      215 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/update_company_override_request_body_value_type.py
--rw-r--r--   0        0        0     1335 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/update_company_override_response.py
--rw-r--r--   0        0        0      222 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/update_plan_entitlement_request_body_metric_period.py
--rw-r--r--   0        0        0      215 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/update_plan_entitlement_request_body_value_type.py
--rw-r--r--   0        0        0     1335 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/entitlements/types/update_plan_entitlement_response.py
--rw-r--r--   0        0        0      162 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/environment.py
--rw-r--r--   0        0        0      414 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/errors/__init__.py
--rw-r--r--   0        0        0      356 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/errors/bad_request_error.py
--rw-r--r--   0        0        0      355 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/errors/forbidden_error.py
--rw-r--r--   0        0        0      360 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/errors/internal_server_error.py
--rw-r--r--   0        0        0      354 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/errors/not_found_error.py
--rw-r--r--   0        0        0      358 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/errors/unauthorized_error.py
--rw-r--r--   0        0        0      681 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/__init__.py
--rw-r--r--   0        0        0    53522 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/client.py
--rw-r--r--   0        0        0      995 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/types/__init__.py
--rw-r--r--   0        0        0     1325 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/types/create_event_batch_response.py
--rw-r--r--   0        0        0     1304 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/types/create_event_response.py
--rw-r--r--   0        0        0     1310 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/types/get_event_response.py
--rw-r--r--   0        0        0     1324 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/types/get_event_summaries_params.py
--rw-r--r--   0        0        0     1460 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/types/get_event_summaries_response.py
--rw-r--r--   0        0        0     1329 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/types/get_event_summary_by_subtype_response.py
--rw-r--r--   0        0        0     1353 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/types/list_events_params.py
--rw-r--r--   0        0        0     1428 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/types/list_events_response.py
--rw-r--r--   0        0        0     1622 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/types/list_metric_counts_params.py
--rw-r--r--   0        0        0     1475 2024-05-16 14:53:08.851939 schematichq-0.0.7/src/schematic/events/types/list_metric_counts_response.py
--rw-r--r--   0        0        0     1931 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/__init__.py
--rw-r--r--   0        0        0   188965 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/client.py
--rw-r--r--   0        0        0     2970 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/__init__.py
--rw-r--r--   0        0        0     1305 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/check_flag_response.py
--rw-r--r--   0        0        0     1309 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/check_flags_response.py
--rw-r--r--   0        0        0     1292 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/count_audience_companies_response.py
--rw-r--r--   0        0        0     1288 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/count_audience_users_response.py
--rw-r--r--   0        0        0     1433 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/count_features_params.py
--rw-r--r--   0        0        0     1329 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/count_features_response.py
--rw-r--r--   0        0        0     1358 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/count_flag_checks_params.py
--rw-r--r--   0        0        0     1338 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/count_flag_checks_response.py
--rw-r--r--   0        0        0     1350 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/count_flags_params.py
--rw-r--r--   0        0        0     1317 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/count_flags_response.py
--rw-r--r--   0        0        0      188 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/create_feature_request_body_feature_type.py
--rw-r--r--   0        0        0     1321 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/create_feature_response.py
--rw-r--r--   0        0        0     1309 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/create_flag_response.py
--rw-r--r--   0        0        0     1286 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/delete_feature_response.py
--rw-r--r--   0        0        0     1283 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/delete_flag_response.py
--rw-r--r--   0        0        0     1318 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/get_feature_response.py
--rw-r--r--   0        0        0     1337 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/get_flag_check_response.py
--rw-r--r--   0        0        0     1306 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/get_flag_response.py
--rw-r--r--   0        0        0     1362 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/get_latest_flag_checks_params.py
--rw-r--r--   0        0        0     1470 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/get_latest_flag_checks_response.py
--rw-r--r--   0        0        0     1408 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/list_audience_companies_response.py
--rw-r--r--   0        0        0     1395 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/list_audience_users_response.py
--rw-r--r--   0        0        0     1432 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/list_features_params.py
--rw-r--r--   0        0        0     1442 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/list_features_response.py
--rw-r--r--   0        0        0     1357 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/list_flag_checks_params.py
--rw-r--r--   0        0        0     1468 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/list_flag_checks_response.py
--rw-r--r--   0        0        0     1349 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/list_flags_params.py
--rw-r--r--   0        0        0     1421 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/list_flags_response.py
--rw-r--r--   0        0        0      188 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/update_feature_request_body_feature_type.py
--rw-r--r--   0        0        0     1321 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/update_feature_response.py
--rw-r--r--   0        0        0     1309 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/update_flag_response.py
--rw-r--r--   0        0        0     1317 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/features/types/update_flag_rules_response.py
--rw-r--r--   0        0        0      797 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/__init__.py
--rw-r--r--   0        0        0    67207 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/client.py
--rw-r--r--   0        0        0     1179 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/__init__.py
--rw-r--r--   0        0        0     1407 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/count_plans_params.py
--rw-r--r--   0        0        0     1317 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/count_plans_response.py
--rw-r--r--   0        0        0      235 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/create_plan_request_body_plan_type.py
--rw-r--r--   0        0        0     1309 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/create_plan_response.py
--rw-r--r--   0        0        0     1287 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/delete_audience_response.py
--rw-r--r--   0        0        0     1283 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/delete_plan_response.py
--rw-r--r--   0        0        0     1335 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/get_audience_response.py
--rw-r--r--   0        0        0     1306 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/get_plan_response.py
--rw-r--r--   0        0        0     1406 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/list_plans_params.py
--rw-r--r--   0        0        0     1421 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/list_plans_response.py
--rw-r--r--   0        0        0     1338 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/update_audience_response.py
--rw-r--r--   0        0        0      235 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/update_plan_request_body_plan_type.py
--rw-r--r--   0        0        0     1309 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/plans/types/update_plan_response.py
--rw-r--r--   0        0        0        0 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/py.typed
--rw-r--r--   0        0        0     9060 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/__init__.py
--rw-r--r--   0        0        0     1165 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/api_error.py
--rw-r--r--   0        0        0     1426 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/api_key_create_response_data.py
--rw-r--r--   0        0        0     1719 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/api_key_request_list_response_data.py
--rw-r--r--   0        0        0     1886 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/api_key_request_response_data.py
--rw-r--r--   0        0        0     1404 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/api_key_response_data.py
--rw-r--r--   0        0        0     1690 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/audience_request_body.py
--rw-r--r--   0        0        0     1356 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/billing_product_response_data.py
--rw-r--r--   0        0        0     1352 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/billing_subscription_response_data.py
--rw-r--r--   0        0        0     1323 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/check_flag_output_with_flag_key.py
--rw-r--r--   0        0        0     1235 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/check_flag_request_body.py
--rw-r--r--   0        0        0     1347 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/check_flag_response_data.py
--rw-r--r--   0        0        0     1273 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/check_flags_response_data.py
--rw-r--r--   0        0        0     1826 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/company_detail_response_data.py
--rw-r--r--   0        0        0     1338 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/company_membership_detail_response_data.py
--rw-r--r--   0        0        0     1220 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/company_membership_response_data.py
--rw-r--r--   0        0        0     1914 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/company_override_response_data.py
--rw-r--r--   0        0        0     1238 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/company_plan_response_data.py
--rw-r--r--   0        0        0     1307 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/company_response_data.py
--rw-r--r--   0        0        0     1357 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/company_subscription_response_data.py
--rw-r--r--   0        0        0     1156 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/count_response.py
--rw-r--r--   0        0        0     1556 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_event_request_body.py
--rw-r--r--   0        0        0      176 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_event_request_body_event_type.py
--rw-r--r--   0        0        0     1242 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_flag_request_body.py
--rw-r--r--   0        0        0     1395 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_or_update_condition_group_request_body.py
--rw-r--r--   0        0        0     2694 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_or_update_condition_request_body.py
--rw-r--r--   0        0        0      242 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_or_update_condition_request_body_condition_type.py
--rw-r--r--   0        0        0      224 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_or_update_condition_request_body_metric_period.py
--rw-r--r--   0        0        0      210 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_or_update_condition_request_body_operator.py
--rw-r--r--   0        0        0     1286 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_or_update_flag_request_body.py
--rw-r--r--   0        0        0     1698 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_or_update_rule_request_body.py
--rw-r--r--   0        0        0      271 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_or_update_rule_request_body_rule_type.py
--rw-r--r--   0        0        0     1513 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_req_common.py
--rw-r--r--   0        0        0      199 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_req_common_metric_period.py
--rw-r--r--   0        0        0      192 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/create_req_common_value_type.py
--rw-r--r--   0        0        0     1223 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/delete_response.py
--rw-r--r--   0        0        0     1219 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/entity_key_definition_response_data.py
--rw-r--r--   0        0        0     1449 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/entity_key_detail_response_data.py
--rw-r--r--   0        0        0     1290 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/entity_key_response_data.py
--rw-r--r--   0        0        0     1282 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/entity_trait_definition_response_data.py
--rw-r--r--   0        0        0     1404 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/entity_trait_detail_response_data.py
--rw-r--r--   0        0        0     1239 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/entity_trait_response_data.py
--rw-r--r--   0        0        0     1140 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/entity_trait_value.py
--rw-r--r--   0        0        0     1365 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/environment_detail_response_data.py
--rw-r--r--   0        0        0     1217 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/environment_response_data.py
--rw-r--r--   0        0        0      237 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/event_body.py
--rw-r--r--   0        0        0     1809 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/event_body_identify.py
--rw-r--r--   0        0        0     1656 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/event_body_identify_company.py
--rw-r--r--   0        0        0     1693 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/event_body_track.py
--rw-r--r--   0        0        0     1954 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/event_detail_response_data.py
--rw-r--r--   0        0        0     1766 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/event_response_data.py
--rw-r--r--   0        0        0     1275 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/event_summary_response_data.py
--rw-r--r--   0        0        0     2133 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/feature_company_response_data.py
--rw-r--r--   0        0        0     2238 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/feature_company_user_response_data.py
--rw-r--r--   0        0        0     1851 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/feature_detail_response_data.py
--rw-r--r--   0        0        0     1368 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/feature_response_data.py
--rw-r--r--   0        0        0     1277 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/feature_usage_detail_response_data.py
--rw-r--r--   0        0        0     2000 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/feature_usage_response_data.py
--rw-r--r--   0        0        0     2163 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/flag_check_log_detail_response_data.py
--rw-r--r--   0        0        0     1617 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/flag_check_log_response_data.py
--rw-r--r--   0        0        0     1666 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/flag_detail_response_data.py
--rw-r--r--   0        0        0     1305 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/flag_response_data.py
--rw-r--r--   0        0        0     1140 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/keys_request_body.py
--rw-r--r--   0        0        0     1319 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/metric_counts_hourly_response_data.py
--rw-r--r--   0        0        0     1325 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/pagination_filter.py
--rw-r--r--   0        0        0     1705 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/plan_audience_detail_response_data.py
--rw-r--r--   0        0        0     1351 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/plan_audience_response_data.py
--rw-r--r--   0        0        0     1416 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/plan_detail_response_data.py
--rw-r--r--   0        0        0     1880 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/plan_entitlement_response_data.py
--rw-r--r--   0        0        0     1224 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/plan_response_data.py
--rw-r--r--   0        0        0     1168 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/preview_object.py
--rw-r--r--   0        0        0     1257 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/raw_event_batch_response_data.py
--rw-r--r--   0        0        0     1237 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/raw_event_response_data.py
--rw-r--r--   0        0        0     2101 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/rule_condition_detail_response_data.py
--rw-r--r--   0        0        0     1455 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/rule_condition_group_detail_response_data.py
--rw-r--r--   0        0        0     1307 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/rule_condition_group_response_data.py
--rw-r--r--   0        0        0     1145 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/rule_condition_resource_response_data.py
--rw-r--r--   0        0        0     1714 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/rule_condition_response_data.py
--rw-r--r--   0        0        0     1655 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/rule_detail_response_data.py
--rw-r--r--   0        0        0     1343 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/rule_response_data.py
--rw-r--r--   0        0        0     1479 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/rules_detail_response_data.py
--rw-r--r--   0        0        0     1493 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/update_req_common.py
--rw-r--r--   0        0        0      199 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/update_req_common_metric_period.py
--rw-r--r--   0        0        0      192 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/update_req_common_value_type.py
--rw-r--r--   0        0        0     1481 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/update_rule_request_body.py
--rw-r--r--   0        0        0     1473 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/upsert_company_request_body.py
--rw-r--r--   0        0        0     1846 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/upsert_trait_request_body.py
--rw-r--r--   0        0        0     1714 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/upsert_user_request_body.py
--rw-r--r--   0        0        0     1583 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/upsert_user_sub_request_body.py
--rw-r--r--   0        0        0     1844 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/user_detail_response_data.py
--rw-r--r--   0        0        0     1262 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/types/user_response_data.py
--rw-r--r--   0        0        0       79 2024-05-16 14:53:08.855939 schematichq-0.0.7/src/schematic/version.py
--rw-r--r--   0        0        0     4416 1970-01-01 00:00:00.000000 schematichq-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     8976 2024-05-28 14:09:36.098384 schematichq-1.0.0/README.md
+-rw-r--r--   0        0        0      597 2024-05-28 14:09:36.098384 schematichq-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    17174 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/__init__.py
+-rw-r--r--   0        0        0     1379 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/__init__.py
+-rw-r--r--   0        0        0   100506 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/client.py
+-rw-r--r--   0        0        0     2097 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/__init__.py
+-rw-r--r--   0        0        0     1325 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/count_api_keys_params.py
+-rw-r--r--   0        0        0     1326 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/count_api_keys_response.py
+-rw-r--r--   0        0        0     1356 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/count_api_requests_params.py
+-rw-r--r--   0        0        0     1342 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/count_api_requests_response.py
+-rw-r--r--   0        0        0     1318 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/create_api_key_response.py
+-rw-r--r--   0        0        0      213 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/create_environment_request_body_environment_type.py
+-rw-r--r--   0        0        0     1337 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/create_environment_response.py
+-rw-r--r--   0        0        0     1285 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/delete_api_key_response.py
+-rw-r--r--   0        0        0     1290 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/delete_environment_response.py
+-rw-r--r--   0        0        0     1296 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/get_api_key_response.py
+-rw-r--r--   0        0        0     1322 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/get_api_request_response.py
+-rw-r--r--   0        0        0     1315 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/get_environment_response.py
+-rw-r--r--   0        0        0     1324 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/list_api_keys_params.py
+-rw-r--r--   0        0        0     1418 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/list_api_keys_response.py
+-rw-r--r--   0        0        0     1355 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/list_api_requests_params.py
+-rw-r--r--   0        0        0     1469 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/list_api_requests_response.py
+-rw-r--r--   0        0        0     1277 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/list_environments_params.py
+-rw-r--r--   0        0        0     1451 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/list_environments_response.py
+-rw-r--r--   0        0        0     1299 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/update_api_key_response.py
+-rw-r--r--   0        0        0      213 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/update_environment_request_body_environment_type.py
+-rw-r--r--   0        0        0     1318 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/accounts/types/update_environment_response.py
+-rw-r--r--   0        0        0     6614 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/base_client.py
+-rw-r--r--   0        0        0      357 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/billing/__init__.py
+-rw-r--r--   0        0        0    25633 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/billing/client.py
+-rw-r--r--   0        0        0      479 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/billing/types/__init__.py
+-rw-r--r--   0        0        0     1311 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/billing/types/list_products_params.py
+-rw-r--r--   0        0        0     1445 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/billing/types/list_products_response.py
+-rw-r--r--   0        0        0     1331 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/billing/types/upsert_billing_product_response.py
+-rw-r--r--   0        0        0     1351 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/billing/types/upsert_billing_subscription_response.py
+-rw-r--r--   0        0        0     2997 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/cache.py
+-rw-r--r--   0        0        0     8915 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/client.py
+-rw-r--r--   0        0        0     3327 2024-05-28 14:09:36.098384 schematichq-1.0.0/src/schematic/companies/__init__.py
+-rw-r--r--   0        0        0   237379 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/client.py
+-rw-r--r--   0        0        0     5169 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/__init__.py
+-rw-r--r--   0        0        0     1413 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/count_companies_params.py
+-rw-r--r--   0        0        0     1333 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/count_companies_response.py
+-rw-r--r--   0        0        0     1368 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/count_entity_key_definitions_params.py
+-rw-r--r--   0        0        0     1379 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/count_entity_key_definitions_response.py
+-rw-r--r--   0        0        0     1412 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/count_entity_trait_definitions_params.py
+-rw-r--r--   0        0        0     1387 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/count_entity_trait_definitions_response.py
+-rw-r--r--   0        0        0     1391 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/count_users_params.py
+-rw-r--r--   0        0        0     1317 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/count_users_response.py
+-rw-r--r--   0        0        0     1321 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/create_company_response.py
+-rw-r--r--   0        0        0      191 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/create_entity_trait_definition_request_body_entity_type.py
+-rw-r--r--   0        0        0      235 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/create_entity_trait_definition_request_body_trait_type.py
+-rw-r--r--   0        0        0     1309 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/create_user_response.py
+-rw-r--r--   0        0        0     1308 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/delete_company_by_keys_response.py
+-rw-r--r--   0        0        0     1296 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/delete_company_membership_response.py
+-rw-r--r--   0        0        0     1286 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/delete_company_response.py
+-rw-r--r--   0        0        0     1296 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/delete_user_by_keys_response.py
+-rw-r--r--   0        0        0     1283 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/delete_user_response.py
+-rw-r--r--   0        0        0     1283 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/get_active_company_subscription_params.py
+-rw-r--r--   0        0        0     1526 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/get_active_company_subscription_response.py
+-rw-r--r--   0        0        0     1318 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/get_company_response.py
+-rw-r--r--   0        0        0     1357 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/get_entity_trait_definition_response.py
+-rw-r--r--   0        0        0     1313 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/get_entity_trait_values_params.py
+-rw-r--r--   0        0        0     1448 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/get_entity_trait_values_response.py
+-rw-r--r--   0        0        0     1367 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/get_or_create_company_membership_response.py
+-rw-r--r--   0        0        0     1365 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/get_or_create_entity_trait_definition_response.py
+-rw-r--r--   0        0        0     1306 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/get_user_response.py
+-rw-r--r--   0        0        0     1412 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/list_companies_params.py
+-rw-r--r--   0        0        0     1446 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/list_companies_response.py
+-rw-r--r--   0        0        0     1318 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/list_company_memberships_params.py
+-rw-r--r--   0        0        0     1514 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/list_company_memberships_response.py
+-rw-r--r--   0        0        0     1312 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/list_company_plans_params.py
+-rw-r--r--   0        0        0     1453 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/list_company_plans_response.py
+-rw-r--r--   0        0        0     1367 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/list_entity_key_definitions_params.py
+-rw-r--r--   0        0        0     1511 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/list_entity_key_definitions_response.py
+-rw-r--r--   0        0        0     1411 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/list_entity_trait_definitions_params.py
+-rw-r--r--   0        0        0     1525 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/list_entity_trait_definitions_response.py
+-rw-r--r--   0        0        0     1390 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/list_users_params.py
+-rw-r--r--   0        0        0     1421 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/list_users_response.py
+-rw-r--r--   0        0        0     1208 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/lookup_company_params.py
+-rw-r--r--   0        0        0     1367 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/lookup_company_response.py
+-rw-r--r--   0        0        0     1205 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/lookup_user_params.py
+-rw-r--r--   0        0        0     1346 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/lookup_user_response.py
+-rw-r--r--   0        0        0      235 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/update_entity_trait_definition_request_body_trait_type.py
+-rw-r--r--   0        0        0     1360 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/update_entity_trait_definition_response.py
+-rw-r--r--   0        0        0     1321 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/upsert_company_response.py
+-rw-r--r--   0        0        0     1326 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/upsert_company_trait_response.py
+-rw-r--r--   0        0        0     1309 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/upsert_user_response.py
+-rw-r--r--   0        0        0     1314 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/companies/types/upsert_user_trait_response.py
+-rw-r--r--   0        0        0      973 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/core/api_error.py
+-rw-r--r--   0        0        0     1496 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      748 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/core/pydantic_utilities.py
+-rw-r--r--   0        0        0     1215 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/core/query_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/core/request_options.py
+-rw-r--r--   0        0        0     2927 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/__init__.py
+-rw-r--r--   0        0        0   153569 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/client.py
+-rw-r--r--   0        0        0     4534 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/__init__.py
+-rw-r--r--   0        0        0     1486 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/count_company_overrides_params.py
+-rw-r--r--   0        0        0     1362 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/count_company_overrides_response.py
+-rw-r--r--   0        0        0     1311 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/count_feature_companies_params.py
+-rw-r--r--   0        0        0     1362 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/count_feature_companies_response.py
+-rw-r--r--   0        0        0     1436 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/count_feature_usage_params.py
+-rw-r--r--   0        0        0     1346 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/count_feature_usage_response.py
+-rw-r--r--   0        0        0     1307 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/count_feature_users_params.py
+-rw-r--r--   0        0        0     1346 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/count_feature_users_response.py
+-rw-r--r--   0        0        0     1480 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/count_plan_entitlements_params.py
+-rw-r--r--   0        0        0     1362 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/count_plan_entitlements_response.py
+-rw-r--r--   0        0        0      222 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/create_company_override_request_body_metric_period.py
+-rw-r--r--   0        0        0      215 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/create_company_override_request_body_value_type.py
+-rw-r--r--   0        0        0     1335 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/create_company_override_response.py
+-rw-r--r--   0        0        0      222 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/create_plan_entitlement_request_body_metric_period.py
+-rw-r--r--   0        0        0      215 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/create_plan_entitlement_request_body_value_type.py
+-rw-r--r--   0        0        0     1335 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/create_plan_entitlement_response.py
+-rw-r--r--   0        0        0     1294 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/delete_company_override_response.py
+-rw-r--r--   0        0        0     1294 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/delete_plan_entitlement_response.py
+-rw-r--r--   0        0        0     1332 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/get_company_override_response.py
+-rw-r--r--   0        0        0     1219 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/get_feature_usage_by_company_params.py
+-rw-r--r--   0        0        0     1430 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/get_feature_usage_by_company_response.py
+-rw-r--r--   0        0        0     1332 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/get_plan_entitlement_response.py
+-rw-r--r--   0        0        0     1485 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/list_company_overrides_params.py
+-rw-r--r--   0        0        0     1481 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/list_company_overrides_response.py
+-rw-r--r--   0        0        0     1310 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/list_feature_companies_params.py
+-rw-r--r--   0        0        0     1478 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/list_feature_companies_response.py
+-rw-r--r--   0        0        0     1435 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/list_feature_usage_params.py
+-rw-r--r--   0        0        0     1456 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/list_feature_usage_response.py
+-rw-r--r--   0        0        0     1306 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/list_feature_users_params.py
+-rw-r--r--   0        0        0     1475 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/list_feature_users_response.py
+-rw-r--r--   0        0        0     1479 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/list_plan_entitlements_params.py
+-rw-r--r--   0        0        0     1481 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/list_plan_entitlements_response.py
+-rw-r--r--   0        0        0      222 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/update_company_override_request_body_metric_period.py
+-rw-r--r--   0        0        0      215 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/update_company_override_request_body_value_type.py
+-rw-r--r--   0        0        0     1335 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/update_company_override_response.py
+-rw-r--r--   0        0        0      222 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/update_plan_entitlement_request_body_metric_period.py
+-rw-r--r--   0        0        0      215 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/update_plan_entitlement_request_body_value_type.py
+-rw-r--r--   0        0        0     1335 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/entitlements/types/update_plan_entitlement_response.py
+-rw-r--r--   0        0        0      162 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/environment.py
+-rw-r--r--   0        0        0      414 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/errors/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/errors/bad_request_error.py
+-rw-r--r--   0        0        0      355 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/errors/forbidden_error.py
+-rw-r--r--   0        0        0      360 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/errors/internal_server_error.py
+-rw-r--r--   0        0        0      354 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/errors/not_found_error.py
+-rw-r--r--   0        0        0      358 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/errors/unauthorized_error.py
+-rw-r--r--   0        0        0     4602 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/event_buffer.py
+-rw-r--r--   0        0        0      681 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/__init__.py
+-rw-r--r--   0        0        0    53522 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/client.py
+-rw-r--r--   0        0        0      995 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/types/__init__.py
+-rw-r--r--   0        0        0     1325 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/types/create_event_batch_response.py
+-rw-r--r--   0        0        0     1304 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/types/create_event_response.py
+-rw-r--r--   0        0        0     1310 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/types/get_event_response.py
+-rw-r--r--   0        0        0     1324 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/types/get_event_summaries_params.py
+-rw-r--r--   0        0        0     1460 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/types/get_event_summaries_response.py
+-rw-r--r--   0        0        0     1329 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/types/get_event_summary_by_subtype_response.py
+-rw-r--r--   0        0        0     1353 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/types/list_events_params.py
+-rw-r--r--   0        0        0     1428 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/types/list_events_response.py
+-rw-r--r--   0        0        0     1622 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/types/list_metric_counts_params.py
+-rw-r--r--   0        0        0     1475 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/events/types/list_metric_counts_response.py
+-rw-r--r--   0        0        0     1931 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/__init__.py
+-rw-r--r--   0        0        0   188965 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/client.py
+-rw-r--r--   0        0        0     2970 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/__init__.py
+-rw-r--r--   0        0        0     1305 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/check_flag_response.py
+-rw-r--r--   0        0        0     1309 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/check_flags_response.py
+-rw-r--r--   0        0        0     1292 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/count_audience_companies_response.py
+-rw-r--r--   0        0        0     1288 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/count_audience_users_response.py
+-rw-r--r--   0        0        0     1433 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/count_features_params.py
+-rw-r--r--   0        0        0     1329 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/count_features_response.py
+-rw-r--r--   0        0        0     1358 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/count_flag_checks_params.py
+-rw-r--r--   0        0        0     1338 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/count_flag_checks_response.py
+-rw-r--r--   0        0        0     1350 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/count_flags_params.py
+-rw-r--r--   0        0        0     1317 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/count_flags_response.py
+-rw-r--r--   0        0        0      188 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/create_feature_request_body_feature_type.py
+-rw-r--r--   0        0        0     1321 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/create_feature_response.py
+-rw-r--r--   0        0        0     1309 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/create_flag_response.py
+-rw-r--r--   0        0        0     1286 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/delete_feature_response.py
+-rw-r--r--   0        0        0     1283 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/delete_flag_response.py
+-rw-r--r--   0        0        0     1318 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/get_feature_response.py
+-rw-r--r--   0        0        0     1337 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/get_flag_check_response.py
+-rw-r--r--   0        0        0     1306 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/get_flag_response.py
+-rw-r--r--   0        0        0     1362 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/get_latest_flag_checks_params.py
+-rw-r--r--   0        0        0     1470 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/get_latest_flag_checks_response.py
+-rw-r--r--   0        0        0     1408 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/list_audience_companies_response.py
+-rw-r--r--   0        0        0     1395 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/list_audience_users_response.py
+-rw-r--r--   0        0        0     1432 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/list_features_params.py
+-rw-r--r--   0        0        0     1442 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/list_features_response.py
+-rw-r--r--   0        0        0     1357 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/list_flag_checks_params.py
+-rw-r--r--   0        0        0     1468 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/list_flag_checks_response.py
+-rw-r--r--   0        0        0     1349 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/list_flags_params.py
+-rw-r--r--   0        0        0     1421 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/list_flags_response.py
+-rw-r--r--   0        0        0      188 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/update_feature_request_body_feature_type.py
+-rw-r--r--   0        0        0     1321 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/update_feature_response.py
+-rw-r--r--   0        0        0     1309 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/update_flag_response.py
+-rw-r--r--   0        0        0     1317 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/features/types/update_flag_rules_response.py
+-rw-r--r--   0        0        0      505 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/http_client.py
+-rw-r--r--   0        0        0      592 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/logging.py
+-rw-r--r--   0        0        0      797 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/plans/__init__.py
+-rw-r--r--   0        0        0    67207 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/plans/client.py
+-rw-r--r--   0        0        0     1179 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/plans/types/__init__.py
+-rw-r--r--   0        0        0     1407 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/plans/types/count_plans_params.py
+-rw-r--r--   0        0        0     1317 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/plans/types/count_plans_response.py
+-rw-r--r--   0        0        0      235 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/plans/types/create_plan_request_body_plan_type.py
+-rw-r--r--   0        0        0     1309 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/plans/types/create_plan_response.py
+-rw-r--r--   0        0        0     1287 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/plans/types/delete_audience_response.py
+-rw-r--r--   0        0        0     1283 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/plans/types/delete_plan_response.py
+-rw-r--r--   0        0        0     1335 2024-05-28 14:09:36.102384 schematichq-1.0.0/src/schematic/plans/types/get_audience_response.py
+-rw-r--r--   0        0        0     1306 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/plans/types/get_plan_response.py
+-rw-r--r--   0        0        0     1406 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/plans/types/list_plans_params.py
+-rw-r--r--   0        0        0     1421 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/plans/types/list_plans_response.py
+-rw-r--r--   0        0        0     1338 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/plans/types/update_audience_response.py
+-rw-r--r--   0        0        0      235 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/plans/types/update_plan_request_body_plan_type.py
+-rw-r--r--   0        0        0     1309 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/plans/types/update_plan_response.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/py.typed
+-rw-r--r--   0        0        0     9060 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/__init__.py
+-rw-r--r--   0        0        0     1165 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/api_error.py
+-rw-r--r--   0        0        0     1426 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/api_key_create_response_data.py
+-rw-r--r--   0        0        0     1719 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/api_key_request_list_response_data.py
+-rw-r--r--   0        0        0     1886 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/api_key_request_response_data.py
+-rw-r--r--   0        0        0     1404 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/api_key_response_data.py
+-rw-r--r--   0        0        0     1690 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/audience_request_body.py
+-rw-r--r--   0        0        0     1374 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/billing_product_response_data.py
+-rw-r--r--   0        0        0     1324 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/billing_subscription_response_data.py
+-rw-r--r--   0        0        0     1323 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/check_flag_output_with_flag_key.py
+-rw-r--r--   0        0        0     1235 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/check_flag_request_body.py
+-rw-r--r--   0        0        0     1347 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/check_flag_response_data.py
+-rw-r--r--   0        0        0     1273 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/check_flags_response_data.py
+-rw-r--r--   0        0        0     1826 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/company_detail_response_data.py
+-rw-r--r--   0        0        0     1338 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/company_membership_detail_response_data.py
+-rw-r--r--   0        0        0     1220 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/company_membership_response_data.py
+-rw-r--r--   0        0        0     1914 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/company_override_response_data.py
+-rw-r--r--   0        0        0     1238 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/company_plan_response_data.py
+-rw-r--r--   0        0        0     1307 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/company_response_data.py
+-rw-r--r--   0        0        0     1375 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/company_subscription_response_data.py
+-rw-r--r--   0        0        0     1156 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/count_response.py
+-rw-r--r--   0        0        0     1556 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_event_request_body.py
+-rw-r--r--   0        0        0      176 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_event_request_body_event_type.py
+-rw-r--r--   0        0        0     1242 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_flag_request_body.py
+-rw-r--r--   0        0        0     1395 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_or_update_condition_group_request_body.py
+-rw-r--r--   0        0        0     2694 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_or_update_condition_request_body.py
+-rw-r--r--   0        0        0      242 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_or_update_condition_request_body_condition_type.py
+-rw-r--r--   0        0        0      224 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_or_update_condition_request_body_metric_period.py
+-rw-r--r--   0        0        0      210 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_or_update_condition_request_body_operator.py
+-rw-r--r--   0        0        0     1286 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_or_update_flag_request_body.py
+-rw-r--r--   0        0        0     1698 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_or_update_rule_request_body.py
+-rw-r--r--   0        0        0      271 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_or_update_rule_request_body_rule_type.py
+-rw-r--r--   0        0        0     1513 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_req_common.py
+-rw-r--r--   0        0        0      199 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_req_common_metric_period.py
+-rw-r--r--   0        0        0      192 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/create_req_common_value_type.py
+-rw-r--r--   0        0        0     1223 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/delete_response.py
+-rw-r--r--   0        0        0     1219 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/entity_key_definition_response_data.py
+-rw-r--r--   0        0        0     1449 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/entity_key_detail_response_data.py
+-rw-r--r--   0        0        0     1290 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/entity_key_response_data.py
+-rw-r--r--   0        0        0     1282 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/entity_trait_definition_response_data.py
+-rw-r--r--   0        0        0     1404 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/entity_trait_detail_response_data.py
+-rw-r--r--   0        0        0     1239 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/entity_trait_response_data.py
+-rw-r--r--   0        0        0     1140 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/entity_trait_value.py
+-rw-r--r--   0        0        0     1365 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/environment_detail_response_data.py
+-rw-r--r--   0        0        0     1217 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/environment_response_data.py
+-rw-r--r--   0        0        0      237 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/event_body.py
+-rw-r--r--   0        0        0     1809 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/event_body_identify.py
+-rw-r--r--   0        0        0     1656 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/event_body_identify_company.py
+-rw-r--r--   0        0        0     1693 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/event_body_track.py
+-rw-r--r--   0        0        0     1954 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/event_detail_response_data.py
+-rw-r--r--   0        0        0     1766 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/event_response_data.py
+-rw-r--r--   0        0        0     1275 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/event_summary_response_data.py
+-rw-r--r--   0        0        0     2133 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/feature_company_response_data.py
+-rw-r--r--   0        0        0     2238 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/feature_company_user_response_data.py
+-rw-r--r--   0        0        0     1851 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/feature_detail_response_data.py
+-rw-r--r--   0        0        0     1368 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/feature_response_data.py
+-rw-r--r--   0        0        0     1277 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/feature_usage_detail_response_data.py
+-rw-r--r--   0        0        0     2000 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/feature_usage_response_data.py
+-rw-r--r--   0        0        0     2163 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/flag_check_log_detail_response_data.py
+-rw-r--r--   0        0        0     1617 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/flag_check_log_response_data.py
+-rw-r--r--   0        0        0     1666 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/flag_detail_response_data.py
+-rw-r--r--   0        0        0     1305 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/flag_response_data.py
+-rw-r--r--   0        0        0     1140 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/keys_request_body.py
+-rw-r--r--   0        0        0     1319 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/metric_counts_hourly_response_data.py
+-rw-r--r--   0        0        0     1325 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/pagination_filter.py
+-rw-r--r--   0        0        0     1705 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/plan_audience_detail_response_data.py
+-rw-r--r--   0        0        0     1351 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/plan_audience_response_data.py
+-rw-r--r--   0        0        0     1416 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/plan_detail_response_data.py
+-rw-r--r--   0        0        0     1880 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/plan_entitlement_response_data.py
+-rw-r--r--   0        0        0     1224 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/plan_response_data.py
+-rw-r--r--   0        0        0     1168 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/preview_object.py
+-rw-r--r--   0        0        0     1257 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/raw_event_batch_response_data.py
+-rw-r--r--   0        0        0     1237 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/raw_event_response_data.py
+-rw-r--r--   0        0        0     2101 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/rule_condition_detail_response_data.py
+-rw-r--r--   0        0        0     1455 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/rule_condition_group_detail_response_data.py
+-rw-r--r--   0        0        0     1307 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/rule_condition_group_response_data.py
+-rw-r--r--   0        0        0     1145 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/rule_condition_resource_response_data.py
+-rw-r--r--   0        0        0     1714 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/rule_condition_response_data.py
+-rw-r--r--   0        0        0     1655 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/rule_detail_response_data.py
+-rw-r--r--   0        0        0     1343 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/rule_response_data.py
+-rw-r--r--   0        0        0     1479 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/rules_detail_response_data.py
+-rw-r--r--   0        0        0     1493 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/update_req_common.py
+-rw-r--r--   0        0        0      199 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/update_req_common_metric_period.py
+-rw-r--r--   0        0        0      192 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/update_req_common_value_type.py
+-rw-r--r--   0        0        0     1481 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/update_rule_request_body.py
+-rw-r--r--   0        0        0     1473 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/upsert_company_request_body.py
+-rw-r--r--   0        0        0     1846 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/upsert_trait_request_body.py
+-rw-r--r--   0        0        0     1714 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/upsert_user_request_body.py
+-rw-r--r--   0        0        0     1583 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/upsert_user_sub_request_body.py
+-rw-r--r--   0        0        0     1844 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/user_detail_response_data.py
+-rw-r--r--   0        0        0     1262 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/types/user_response_data.py
+-rw-r--r--   0        0        0       79 2024-05-28 14:09:36.106384 schematichq-1.0.0/src/schematic/version.py
+-rw-r--r--   0        0        0     9470 1970-01-01 00:00:00.000000 schematichq-1.0.0/PKG-INFO
```

### Comparing `schematichq-0.0.7/pyproject.toml` & `schematichq-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schematichq"
-version = "0.0.7"
+version = "1.0.0"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "schematic", from = "src"}
 ]
```

### Comparing `schematichq-0.0.7/src/schematic/__init__.py` & `schematichq-1.0.0/src/schematic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     GetApiKeyResponse,
     GetApiRequestResponse,
     GetEnvironmentResponse,
     ListApiKeysParams,
     ListApiKeysResponse,
     ListApiRequestsParams,
     ListApiRequestsResponse,
+    ListEnvironmentsParams,
+    ListEnvironmentsResponse,
     UpdateApiKeyResponse,
     UpdateEnvironmentRequestBodyEnvironmentType,
     UpdateEnvironmentResponse,
 )
 from .billing import (
     ListProductsParams,
     ListProductsResponse,
@@ -449,14 +451,16 @@
     "ListCompanyOverridesResponse",
     "ListCompanyPlansParams",
     "ListCompanyPlansResponse",
     "ListEntityKeyDefinitionsParams",
     "ListEntityKeyDefinitionsResponse",
     "ListEntityTraitDefinitionsParams",
     "ListEntityTraitDefinitionsResponse",
+    "ListEnvironmentsParams",
+    "ListEnvironmentsResponse",
     "ListEventsParams",
     "ListEventsResponse",
     "ListFeatureCompaniesParams",
     "ListFeatureCompaniesResponse",
     "ListFeatureUsageParams",
     "ListFeatureUsageResponse",
     "ListFeatureUsersParams",
```

### Comparing `schematichq-0.0.7/src/schematic/accounts/__init__.py` & `schematichq-1.0.0/src/schematic/accounts/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     GetApiKeyResponse,
     GetApiRequestResponse,
     GetEnvironmentResponse,
     ListApiKeysParams,
     ListApiKeysResponse,
     ListApiRequestsParams,
     ListApiRequestsResponse,
+    ListEnvironmentsParams,
+    ListEnvironmentsResponse,
     UpdateApiKeyResponse,
     UpdateEnvironmentRequestBodyEnvironmentType,
     UpdateEnvironmentResponse,
 )
 
 __all__ = [
     "CountApiKeysParams",
@@ -35,11 +37,13 @@
     "GetApiKeyResponse",
     "GetApiRequestResponse",
     "GetEnvironmentResponse",
     "ListApiKeysParams",
     "ListApiKeysResponse",
     "ListApiRequestsParams",
     "ListApiRequestsResponse",
+    "ListEnvironmentsParams",
+    "ListEnvironmentsResponse",
     "UpdateApiKeyResponse",
     "UpdateEnvironmentRequestBodyEnvironmentType",
     "UpdateEnvironmentResponse",
 ]
```

### Comparing `schematichq-0.0.7/src/schematic/accounts/client.py` & `schematichq-1.0.0/src/schematic/accounts/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from .types.delete_api_key_response import DeleteApiKeyResponse
 from .types.delete_environment_response import DeleteEnvironmentResponse
 from .types.get_api_key_response import GetApiKeyResponse
 from .types.get_api_request_response import GetApiRequestResponse
 from .types.get_environment_response import GetEnvironmentResponse
 from .types.list_api_keys_response import ListApiKeysResponse
 from .types.list_api_requests_response import ListApiRequestsResponse
+from .types.list_environments_response import ListEnvironmentsResponse
 from .types.update_api_key_response import UpdateApiKeyResponse
 from .types.update_environment_request_body_environment_type import UpdateEnvironmentRequestBodyEnvironmentType
 from .types.update_environment_response import UpdateEnvironmentResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
@@ -820,14 +821,103 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
         raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
 
+    def list_environments(
+        self,
+        *,
+        ids: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
+        limit: typing.Optional[int] = None,
+        offset: typing.Optional[int] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ListEnvironmentsResponse:
+        """
+        Parameters
+        ----------
+        ids : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+
+        limit : typing.Optional[int]
+            Page limit (default 100)
+
+        offset : typing.Optional[int]
+            Page offset (default 0)
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListEnvironmentsResponse
+            OK
+
+        Examples
+        --------
+        from schematic.client import Schematic
+
+        client = Schematic(
+            api_key="YOUR_API_KEY",
+        )
+        client.accounts.list_environments()
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "environments"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "ids": ids,
+                            "limit": limit,
+                            "offset": offset,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic_v1.parse_obj_as(ListEnvironmentsResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(
+                pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 403:
+            raise ForbiddenError(pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(
+                pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
     def create_environment(
         self,
         *,
         environment_type: CreateEnvironmentRequestBodyEnvironmentType,
         name: str,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> CreateEnvironmentResponse:
@@ -1917,14 +2007,103 @@
         if _response.status_code == 400:
             raise BadRequestError(pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
             )
         if _response.status_code == 403:
+            raise ForbiddenError(pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 500:
+            raise InternalServerError(
+                pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise core_api_error_ApiError(status_code=_response.status_code, body=_response.text)
+        raise core_api_error_ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def list_environments(
+        self,
+        *,
+        ids: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
+        limit: typing.Optional[int] = None,
+        offset: typing.Optional[int] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ListEnvironmentsResponse:
+        """
+        Parameters
+        ----------
+        ids : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+
+        limit : typing.Optional[int]
+            Page limit (default 100)
+
+        offset : typing.Optional[int]
+            Page offset (default 0)
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListEnvironmentsResponse
+            OK
+
+        Examples
+        --------
+        from schematic.client import AsyncSchematic
+
+        client = AsyncSchematic(
+            api_key="YOUR_API_KEY",
+        )
+        await client.accounts.list_environments()
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "environments"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "ids": ids,
+                            "limit": limit,
+                            "offset": offset,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic_v1.parse_obj_as(ListEnvironmentsResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(
+                pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
+            )
+        if _response.status_code == 403:
             raise ForbiddenError(pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
             )
         try:
             _response_json = _response.json()
```

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/__init__.py` & `schematichq-1.0.0/src/schematic/accounts/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from .get_api_key_response import GetApiKeyResponse
 from .get_api_request_response import GetApiRequestResponse
 from .get_environment_response import GetEnvironmentResponse
 from .list_api_keys_params import ListApiKeysParams
 from .list_api_keys_response import ListApiKeysResponse
 from .list_api_requests_params import ListApiRequestsParams
 from .list_api_requests_response import ListApiRequestsResponse
+from .list_environments_params import ListEnvironmentsParams
+from .list_environments_response import ListEnvironmentsResponse
 from .update_api_key_response import UpdateApiKeyResponse
 from .update_environment_request_body_environment_type import UpdateEnvironmentRequestBodyEnvironmentType
 from .update_environment_response import UpdateEnvironmentResponse
 
 __all__ = [
     "CountApiKeysParams",
     "CountApiKeysResponse",
@@ -33,11 +35,13 @@
     "GetApiKeyResponse",
     "GetApiRequestResponse",
     "GetEnvironmentResponse",
     "ListApiKeysParams",
     "ListApiKeysResponse",
     "ListApiRequestsParams",
     "ListApiRequestsResponse",
+    "ListEnvironmentsParams",
+    "ListEnvironmentsResponse",
     "UpdateApiKeyResponse",
     "UpdateEnvironmentRequestBodyEnvironmentType",
     "UpdateEnvironmentResponse",
 ]
```

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/count_api_keys_params.py` & `schematichq-1.0.0/src/schematic/accounts/types/count_api_keys_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/count_api_keys_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/count_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/count_api_requests_params.py` & `schematichq-1.0.0/src/schematic/accounts/types/count_api_requests_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/count_api_requests_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/count_api_requests_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/create_api_key_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/create_api_key_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/create_environment_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/create_environment_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/delete_api_key_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/delete_api_key_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/delete_environment_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/delete_environment_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/get_api_key_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/get_api_key_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/get_api_request_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/get_api_request_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/get_environment_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/get_environment_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/list_api_keys_params.py` & `schematichq-1.0.0/src/schematic/accounts/types/list_api_keys_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/list_api_keys_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/list_api_requests_params.py` & `schematichq-1.0.0/src/schematic/accounts/types/list_api_requests_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/list_api_requests_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/list_api_requests_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/update_api_key_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/update_api_key_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/accounts/types/update_environment_response.py` & `schematichq-1.0.0/src/schematic/accounts/types/update_environment_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/base_client.py` & `schematichq-1.0.0/src/schematic/base_client.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/billing/client.py` & `schematichq-1.0.0/src/schematic/billing/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,27 +229,30 @@
     def upsert_billing_subscription(
         self,
         *,
         customer_external_id: str,
         expired_at: dt.datetime,
         product_external_ids: typing.Sequence[str],
         subscription_external_id: str,
+        interval: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> UpsertBillingSubscriptionResponse:
         """
         Parameters
         ----------
         customer_external_id : str
 
         expired_at : dt.datetime
 
         product_external_ids : typing.Sequence[str]
 
         subscription_external_id : str
 
+        interval : typing.Optional[str]
+
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
         UpsertBillingSubscriptionResponse
             Created
@@ -268,40 +271,34 @@
             expired_at=datetime.datetime.fromisoformat(
                 "2024-01-15 09:30:00+00:00",
             ),
             product_external_ids=["product_external_ids"],
             subscription_external_id="subscription_external_id",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {
+            "customer_external_id": customer_external_id,
+            "expired_at": expired_at,
+            "product_external_ids": product_external_ids,
+            "subscription_external_id": subscription_external_id,
+        }
+        if interval is not OMIT:
+            _request["interval"] = interval
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "billing/subscription/upsert"),
             params=encode_query(
                 jsonable_encoder(
                     request_options.get("additional_query_parameters") if request_options is not None else None
                 )
             ),
-            json=jsonable_encoder(
-                {
-                    "customer_external_id": customer_external_id,
-                    "expired_at": expired_at,
-                    "product_external_ids": product_external_ids,
-                    "subscription_external_id": subscription_external_id,
-                }
-            )
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(
-                    {
-                        "customer_external_id": customer_external_id,
-                        "expired_at": expired_at,
-                        "product_external_ids": product_external_ids,
-                        "subscription_external_id": subscription_external_id,
-                    }
-                ),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -539,27 +536,30 @@
     async def upsert_billing_subscription(
         self,
         *,
         customer_external_id: str,
         expired_at: dt.datetime,
         product_external_ids: typing.Sequence[str],
         subscription_external_id: str,
+        interval: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> UpsertBillingSubscriptionResponse:
         """
         Parameters
         ----------
         customer_external_id : str
 
         expired_at : dt.datetime
 
         product_external_ids : typing.Sequence[str]
 
         subscription_external_id : str
 
+        interval : typing.Optional[str]
+
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
         UpsertBillingSubscriptionResponse
             Created
@@ -578,40 +578,34 @@
             expired_at=datetime.datetime.fromisoformat(
                 "2024-01-15 09:30:00+00:00",
             ),
             product_external_ids=["product_external_ids"],
             subscription_external_id="subscription_external_id",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {
+            "customer_external_id": customer_external_id,
+            "expired_at": expired_at,
+            "product_external_ids": product_external_ids,
+            "subscription_external_id": subscription_external_id,
+        }
+        if interval is not OMIT:
+            _request["interval"] = interval
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "billing/subscription/upsert"),
             params=encode_query(
                 jsonable_encoder(
                     request_options.get("additional_query_parameters") if request_options is not None else None
                 )
             ),
-            json=jsonable_encoder(
-                {
-                    "customer_external_id": customer_external_id,
-                    "expired_at": expired_at,
-                    "product_external_ids": product_external_ids,
-                    "subscription_external_id": subscription_external_id,
-                }
-            )
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(
-                    {
-                        "customer_external_id": customer_external_id,
-                        "expired_at": expired_at,
-                        "product_external_ids": product_external_ids,
-                        "subscription_external_id": subscription_external_id,
-                    }
-                ),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
```

### Comparing `schematichq-0.0.7/src/schematic/billing/types/list_products_params.py` & `schematichq-1.0.0/src/schematic/billing/types/list_products_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/billing/types/list_products_response.py` & `schematichq-1.0.0/src/schematic/billing/types/list_products_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/billing/types/upsert_billing_product_response.py` & `schematichq-1.0.0/src/schematic/billing/types/upsert_billing_product_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/billing/types/upsert_billing_subscription_response.py` & `schematichq-1.0.0/src/schematic/billing/types/upsert_billing_subscription_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/__init__.py` & `schematichq-1.0.0/src/schematic/companies/__init__.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/client.py` & `schematichq-1.0.0/src/schematic/companies/client.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/__init__.py` & `schematichq-1.0.0/src/schematic/companies/types/__init__.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/count_companies_params.py` & `schematichq-1.0.0/src/schematic/companies/types/count_companies_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/count_companies_response.py` & `schematichq-1.0.0/src/schematic/companies/types/count_companies_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/count_entity_key_definitions_params.py` & `schematichq-1.0.0/src/schematic/companies/types/count_entity_key_definitions_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/count_entity_key_definitions_response.py` & `schematichq-1.0.0/src/schematic/companies/types/count_entity_key_definitions_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/count_entity_trait_definitions_params.py` & `schematichq-1.0.0/src/schematic/companies/types/count_entity_trait_definitions_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/count_entity_trait_definitions_response.py` & `schematichq-1.0.0/src/schematic/companies/types/count_entity_trait_definitions_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/count_users_params.py` & `schematichq-1.0.0/src/schematic/companies/types/count_users_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/count_users_response.py` & `schematichq-1.0.0/src/schematic/companies/types/count_users_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/create_company_response.py` & `schematichq-1.0.0/src/schematic/companies/types/create_company_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/create_user_response.py` & `schematichq-1.0.0/src/schematic/companies/types/create_user_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/delete_company_by_keys_response.py` & `schematichq-1.0.0/src/schematic/companies/types/delete_company_by_keys_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/delete_company_membership_response.py` & `schematichq-1.0.0/src/schematic/companies/types/delete_company_membership_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/delete_company_response.py` & `schematichq-1.0.0/src/schematic/companies/types/delete_company_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/delete_user_by_keys_response.py` & `schematichq-1.0.0/src/schematic/companies/types/delete_user_by_keys_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/delete_user_response.py` & `schematichq-1.0.0/src/schematic/companies/types/delete_user_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/get_active_company_subscription_params.py` & `schematichq-1.0.0/src/schematic/companies/types/get_active_company_subscription_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/get_active_company_subscription_response.py` & `schematichq-1.0.0/src/schematic/companies/types/get_active_company_subscription_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/get_company_response.py` & `schematichq-1.0.0/src/schematic/companies/types/get_company_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/get_entity_trait_definition_response.py` & `schematichq-1.0.0/src/schematic/companies/types/get_entity_trait_definition_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/get_entity_trait_values_params.py` & `schematichq-1.0.0/src/schematic/companies/types/get_entity_trait_values_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/get_entity_trait_values_response.py` & `schematichq-1.0.0/src/schematic/companies/types/get_entity_trait_values_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/get_or_create_company_membership_response.py` & `schematichq-1.0.0/src/schematic/companies/types/get_or_create_company_membership_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/get_or_create_entity_trait_definition_response.py` & `schematichq-1.0.0/src/schematic/companies/types/get_or_create_entity_trait_definition_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/get_user_response.py` & `schematichq-1.0.0/src/schematic/companies/types/get_user_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/list_companies_params.py` & `schematichq-1.0.0/src/schematic/companies/types/list_companies_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/list_companies_response.py` & `schematichq-1.0.0/src/schematic/companies/types/list_companies_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/list_company_memberships_params.py` & `schematichq-1.0.0/src/schematic/companies/types/list_company_memberships_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/list_company_memberships_response.py` & `schematichq-1.0.0/src/schematic/companies/types/list_company_memberships_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/list_company_plans_params.py` & `schematichq-1.0.0/src/schematic/companies/types/list_company_plans_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/list_company_plans_response.py` & `schematichq-1.0.0/src/schematic/companies/types/list_company_plans_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/list_entity_key_definitions_params.py` & `schematichq-1.0.0/src/schematic/companies/types/list_entity_key_definitions_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/list_entity_key_definitions_response.py` & `schematichq-1.0.0/src/schematic/companies/types/list_entity_key_definitions_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/list_entity_trait_definitions_params.py` & `schematichq-1.0.0/src/schematic/companies/types/list_entity_trait_definitions_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/list_entity_trait_definitions_response.py` & `schematichq-1.0.0/src/schematic/companies/types/list_entity_trait_definitions_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/list_users_params.py` & `schematichq-1.0.0/src/schematic/companies/types/list_users_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/list_users_response.py` & `schematichq-1.0.0/src/schematic/companies/types/list_users_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/lookup_company_params.py` & `schematichq-1.0.0/src/schematic/companies/types/lookup_company_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/lookup_company_response.py` & `schematichq-1.0.0/src/schematic/companies/types/lookup_company_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/lookup_user_params.py` & `schematichq-1.0.0/src/schematic/companies/types/lookup_user_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/lookup_user_response.py` & `schematichq-1.0.0/src/schematic/companies/types/lookup_user_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/update_entity_trait_definition_response.py` & `schematichq-1.0.0/src/schematic/companies/types/update_entity_trait_definition_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/upsert_company_response.py` & `schematichq-1.0.0/src/schematic/companies/types/upsert_company_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/upsert_company_trait_response.py` & `schematichq-1.0.0/src/schematic/companies/types/upsert_company_trait_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/upsert_user_response.py` & `schematichq-1.0.0/src/schematic/companies/types/upsert_user_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/companies/types/upsert_user_trait_response.py` & `schematichq-1.0.0/src/schematic/companies/types/upsert_user_trait_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/core/__init__.py` & `schematichq-1.0.0/src/schematic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/core/client_wrapper.py` & `schematichq-1.0.0/src/schematic/core/client_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "schematichq",
-            "X-Fern-SDK-Version": "0.0.7",
+            "X-Fern-SDK-Version": "1.0.0",
         }
         headers["X-Schematic-Api-Key"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `schematichq-0.0.7/src/schematic/core/datetime_utils.py` & `schematichq-1.0.0/src/schematic/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/core/file.py` & `schematichq-1.0.0/src/schematic/core/file.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/core/http_client.py` & `schematichq-1.0.0/src/schematic/core/http_client.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/core/jsonable_encoder.py` & `schematichq-1.0.0/src/schematic/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/core/pydantic_utilities.py` & `schematichq-1.0.0/src/schematic/core/pydantic_utilities.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/core/query_encoder.py` & `schematichq-1.0.0/src/schematic/core/query_encoder.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/core/request_options.py` & `schematichq-1.0.0/src/schematic/core/request_options.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/__init__.py` & `schematichq-1.0.0/src/schematic/entitlements/__init__.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/client.py` & `schematichq-1.0.0/src/schematic/entitlements/client.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/__init__.py` & `schematichq-1.0.0/src/schematic/entitlements/types/__init__.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/count_company_overrides_params.py` & `schematichq-1.0.0/src/schematic/entitlements/types/count_company_overrides_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/count_company_overrides_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/count_company_overrides_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/count_feature_companies_params.py` & `schematichq-1.0.0/src/schematic/entitlements/types/count_feature_companies_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/count_feature_companies_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/count_feature_companies_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/count_feature_usage_params.py` & `schematichq-1.0.0/src/schematic/entitlements/types/count_feature_usage_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/count_feature_usage_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/count_feature_usage_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/count_feature_users_params.py` & `schematichq-1.0.0/src/schematic/entitlements/types/count_feature_users_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/count_feature_users_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/count_feature_users_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/count_plan_entitlements_params.py` & `schematichq-1.0.0/src/schematic/entitlements/types/count_plan_entitlements_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/count_plan_entitlements_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/count_plan_entitlements_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/create_company_override_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/create_company_override_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/create_plan_entitlement_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/create_plan_entitlement_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/delete_company_override_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/delete_company_override_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/delete_plan_entitlement_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/delete_plan_entitlement_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/get_company_override_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/get_company_override_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/get_feature_usage_by_company_params.py` & `schematichq-1.0.0/src/schematic/entitlements/types/get_feature_usage_by_company_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/get_feature_usage_by_company_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/get_feature_usage_by_company_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/get_plan_entitlement_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/get_plan_entitlement_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/list_company_overrides_params.py` & `schematichq-1.0.0/src/schematic/entitlements/types/list_company_overrides_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/list_company_overrides_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/list_company_overrides_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/list_feature_companies_params.py` & `schematichq-1.0.0/src/schematic/entitlements/types/list_feature_companies_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/list_feature_companies_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/list_feature_companies_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/list_feature_usage_params.py` & `schematichq-1.0.0/src/schematic/entitlements/types/list_feature_usage_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/list_feature_usage_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/list_feature_usage_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/list_feature_users_params.py` & `schematichq-1.0.0/src/schematic/entitlements/types/list_feature_users_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/list_feature_users_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/list_feature_users_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/list_plan_entitlements_params.py` & `schematichq-1.0.0/src/schematic/entitlements/types/list_plan_entitlements_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/list_plan_entitlements_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/list_plan_entitlements_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/update_company_override_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/update_company_override_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/entitlements/types/update_plan_entitlement_response.py` & `schematichq-1.0.0/src/schematic/entitlements/types/update_plan_entitlement_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/__init__.py` & `schematichq-1.0.0/src/schematic/events/__init__.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/client.py` & `schematichq-1.0.0/src/schematic/events/client.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/types/__init__.py` & `schematichq-1.0.0/src/schematic/events/types/__init__.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/types/create_event_batch_response.py` & `schematichq-1.0.0/src/schematic/events/types/create_event_batch_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/types/create_event_response.py` & `schematichq-1.0.0/src/schematic/events/types/create_event_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/types/get_event_response.py` & `schematichq-1.0.0/src/schematic/events/types/get_event_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/types/get_event_summaries_params.py` & `schematichq-1.0.0/src/schematic/events/types/get_event_summaries_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/types/get_event_summaries_response.py` & `schematichq-1.0.0/src/schematic/events/types/get_event_summaries_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/types/get_event_summary_by_subtype_response.py` & `schematichq-1.0.0/src/schematic/events/types/get_event_summary_by_subtype_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/types/list_events_params.py` & `schematichq-1.0.0/src/schematic/events/types/list_events_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/types/list_events_response.py` & `schematichq-1.0.0/src/schematic/events/types/list_events_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/types/list_metric_counts_params.py` & `schematichq-1.0.0/src/schematic/events/types/list_metric_counts_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/events/types/list_metric_counts_response.py` & `schematichq-1.0.0/src/schematic/events/types/list_metric_counts_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/__init__.py` & `schematichq-1.0.0/src/schematic/features/__init__.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/client.py` & `schematichq-1.0.0/src/schematic/features/client.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/__init__.py` & `schematichq-1.0.0/src/schematic/features/types/__init__.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/check_flag_response.py` & `schematichq-1.0.0/src/schematic/features/types/check_flag_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/check_flags_response.py` & `schematichq-1.0.0/src/schematic/features/types/check_flags_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/count_audience_companies_response.py` & `schematichq-1.0.0/src/schematic/features/types/count_audience_companies_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/count_audience_users_response.py` & `schematichq-1.0.0/src/schematic/features/types/count_audience_users_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/count_features_params.py` & `schematichq-1.0.0/src/schematic/features/types/count_features_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/count_features_response.py` & `schematichq-1.0.0/src/schematic/features/types/count_features_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/count_flag_checks_params.py` & `schematichq-1.0.0/src/schematic/features/types/count_flag_checks_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/count_flag_checks_response.py` & `schematichq-1.0.0/src/schematic/features/types/count_flag_checks_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/count_flags_params.py` & `schematichq-1.0.0/src/schematic/features/types/count_flags_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/count_flags_response.py` & `schematichq-1.0.0/src/schematic/features/types/count_flags_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/create_feature_response.py` & `schematichq-1.0.0/src/schematic/features/types/create_feature_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/create_flag_response.py` & `schematichq-1.0.0/src/schematic/features/types/create_flag_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/delete_feature_response.py` & `schematichq-1.0.0/src/schematic/features/types/delete_feature_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/delete_flag_response.py` & `schematichq-1.0.0/src/schematic/features/types/delete_flag_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/get_feature_response.py` & `schematichq-1.0.0/src/schematic/features/types/get_feature_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/get_flag_check_response.py` & `schematichq-1.0.0/src/schematic/features/types/get_flag_check_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/get_flag_response.py` & `schematichq-1.0.0/src/schematic/features/types/get_flag_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/get_latest_flag_checks_params.py` & `schematichq-1.0.0/src/schematic/features/types/get_latest_flag_checks_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/get_latest_flag_checks_response.py` & `schematichq-1.0.0/src/schematic/features/types/get_latest_flag_checks_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/list_audience_companies_response.py` & `schematichq-1.0.0/src/schematic/features/types/list_audience_companies_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/list_audience_users_response.py` & `schematichq-1.0.0/src/schematic/features/types/list_audience_users_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/list_features_params.py` & `schematichq-1.0.0/src/schematic/features/types/list_features_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/list_features_response.py` & `schematichq-1.0.0/src/schematic/features/types/list_features_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/list_flag_checks_params.py` & `schematichq-1.0.0/src/schematic/features/types/list_flag_checks_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/list_flag_checks_response.py` & `schematichq-1.0.0/src/schematic/features/types/list_flag_checks_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/list_flags_params.py` & `schematichq-1.0.0/src/schematic/features/types/list_flags_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/list_flags_response.py` & `schematichq-1.0.0/src/schematic/features/types/list_flags_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/update_feature_response.py` & `schematichq-1.0.0/src/schematic/features/types/update_feature_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/update_flag_response.py` & `schematichq-1.0.0/src/schematic/features/types/update_flag_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/features/types/update_flag_rules_response.py` & `schematichq-1.0.0/src/schematic/features/types/update_flag_rules_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/__init__.py` & `schematichq-1.0.0/src/schematic/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/client.py` & `schematichq-1.0.0/src/schematic/plans/client.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/types/__init__.py` & `schematichq-1.0.0/src/schematic/plans/types/__init__.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/types/count_plans_params.py` & `schematichq-1.0.0/src/schematic/plans/types/count_plans_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/types/count_plans_response.py` & `schematichq-1.0.0/src/schematic/plans/types/count_plans_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/types/create_plan_response.py` & `schematichq-1.0.0/src/schematic/plans/types/create_plan_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/types/delete_audience_response.py` & `schematichq-1.0.0/src/schematic/plans/types/delete_audience_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/types/delete_plan_response.py` & `schematichq-1.0.0/src/schematic/plans/types/delete_plan_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/types/get_audience_response.py` & `schematichq-1.0.0/src/schematic/plans/types/get_audience_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/types/get_plan_response.py` & `schematichq-1.0.0/src/schematic/plans/types/get_plan_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/types/list_plans_params.py` & `schematichq-1.0.0/src/schematic/plans/types/list_plans_params.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/types/list_plans_response.py` & `schematichq-1.0.0/src/schematic/plans/types/list_plans_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/types/update_audience_response.py` & `schematichq-1.0.0/src/schematic/plans/types/update_audience_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/plans/types/update_plan_response.py` & `schematichq-1.0.0/src/schematic/plans/types/update_plan_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/__init__.py` & `schematichq-1.0.0/src/schematic/types/__init__.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/api_error.py` & `schematichq-1.0.0/src/schematic/types/api_error.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/api_key_create_response_data.py` & `schematichq-1.0.0/src/schematic/types/api_key_create_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/api_key_request_list_response_data.py` & `schematichq-1.0.0/src/schematic/types/api_key_request_list_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/api_key_request_response_data.py` & `schematichq-1.0.0/src/schematic/types/api_key_request_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/api_key_response_data.py` & `schematichq-1.0.0/src/schematic/types/api_key_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/audience_request_body.py` & `schematichq-1.0.0/src/schematic/types/audience_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/billing_product_response_data.py` & `schematichq-1.0.0/src/schematic/types/billing_product_response_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
 
 class BillingProductResponseData(pydantic_v1.BaseModel):
     account_id: str
     created_at: dt.datetime
+    currency: str
     deleted_at: typing.Optional[dt.datetime] = None
     environment_id: str
     external_id: str
     name: str
     price: float
     product_id: str
     quantity: float
```

### Comparing `schematichq-0.0.7/src/schematic/types/billing_subscription_response_data.py` & `schematichq-1.0.0/src/schematic/types/billing_subscription_response_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 class BillingSubscriptionResponseData(pydantic_v1.BaseModel):
     """
     The created resource
     """
 
-    created_at: dt.datetime
     deleted_at: typing.Optional[dt.datetime] = None
     expired_at: typing.Optional[dt.datetime] = None
     external_id: str
     id: int
     updated_at: dt.datetime
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `schematichq-0.0.7/src/schematic/types/check_flag_output_with_flag_key.py` & `schematichq-1.0.0/src/schematic/types/check_flag_output_with_flag_key.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/check_flag_request_body.py` & `schematichq-1.0.0/src/schematic/types/check_flag_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/check_flag_response_data.py` & `schematichq-1.0.0/src/schematic/types/check_flag_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/check_flags_response_data.py` & `schematichq-1.0.0/src/schematic/types/check_flags_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/company_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/company_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/company_membership_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/company_membership_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/company_membership_response_data.py` & `schematichq-1.0.0/src/schematic/types/company_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/company_override_response_data.py` & `schematichq-1.0.0/src/schematic/types/company_override_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/company_plan_response_data.py` & `schematichq-1.0.0/src/schematic/types/company_plan_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/company_response_data.py` & `schematichq-1.0.0/src/schematic/types/company_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/company_subscription_response_data.py` & `schematichq-1.0.0/src/schematic/types/plan_detail_response_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
-from .billing_product_response_data import BillingProductResponseData
+from .feature_detail_response_data import FeatureDetailResponseData
 
 
-class CompanySubscriptionResponseData(pydantic_v1.BaseModel):
-    customer_external_id: str
-    expired_at: typing.Optional[dt.datetime] = None
-    products: typing.List[BillingProductResponseData]
-    subscription_external_id: str
+class PlanDetailResponseData(pydantic_v1.BaseModel):
+    """
+    The updated resource
+    """
+
+    company_count: int
+    created_at: dt.datetime
+    description: str
+    features: typing.List[FeatureDetailResponseData]
+    id: str
+    name: str
+    plan_type: str
+    updated_at: dt.datetime
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `schematichq-0.0.7/src/schematic/types/count_response.py` & `schematichq-1.0.0/src/schematic/types/count_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/create_event_request_body.py` & `schematichq-1.0.0/src/schematic/types/create_event_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/create_flag_request_body.py` & `schematichq-1.0.0/src/schematic/types/create_flag_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/create_or_update_condition_group_request_body.py` & `schematichq-1.0.0/src/schematic/types/create_or_update_condition_group_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/create_or_update_condition_request_body.py` & `schematichq-1.0.0/src/schematic/types/create_or_update_condition_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/create_or_update_flag_request_body.py` & `schematichq-1.0.0/src/schematic/types/create_or_update_flag_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/create_or_update_rule_request_body.py` & `schematichq-1.0.0/src/schematic/types/create_or_update_rule_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/create_req_common.py` & `schematichq-1.0.0/src/schematic/types/create_req_common.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/delete_response.py` & `schematichq-1.0.0/src/schematic/types/delete_response.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/entity_key_definition_response_data.py` & `schematichq-1.0.0/src/schematic/types/entity_key_definition_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/entity_key_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/entity_key_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/entity_key_response_data.py` & `schematichq-1.0.0/src/schematic/types/entity_key_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/entity_trait_definition_response_data.py` & `schematichq-1.0.0/src/schematic/types/entity_trait_definition_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/entity_trait_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/entity_trait_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/entity_trait_response_data.py` & `schematichq-1.0.0/src/schematic/types/entity_trait_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/entity_trait_value.py` & `schematichq-1.0.0/src/schematic/types/entity_trait_value.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/environment_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/environment_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/environment_response_data.py` & `schematichq-1.0.0/src/schematic/types/environment_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/event_body_identify.py` & `schematichq-1.0.0/src/schematic/types/event_body_identify.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/event_body_identify_company.py` & `schematichq-1.0.0/src/schematic/types/event_body_identify_company.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/event_body_track.py` & `schematichq-1.0.0/src/schematic/types/event_body_track.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/event_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/event_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/event_response_data.py` & `schematichq-1.0.0/src/schematic/types/event_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/event_summary_response_data.py` & `schematichq-1.0.0/src/schematic/types/event_summary_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/feature_company_response_data.py` & `schematichq-1.0.0/src/schematic/types/feature_company_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/feature_company_user_response_data.py` & `schematichq-1.0.0/src/schematic/types/feature_company_user_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/feature_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/feature_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/feature_response_data.py` & `schematichq-1.0.0/src/schematic/types/feature_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/feature_usage_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/feature_usage_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/feature_usage_response_data.py` & `schematichq-1.0.0/src/schematic/types/feature_usage_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/flag_check_log_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/flag_check_log_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/flag_check_log_response_data.py` & `schematichq-1.0.0/src/schematic/types/flag_check_log_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/flag_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/flag_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/flag_response_data.py` & `schematichq-1.0.0/src/schematic/types/flag_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/keys_request_body.py` & `schematichq-1.0.0/src/schematic/types/keys_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/metric_counts_hourly_response_data.py` & `schematichq-1.0.0/src/schematic/types/metric_counts_hourly_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/pagination_filter.py` & `schematichq-1.0.0/src/schematic/types/pagination_filter.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/plan_audience_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/plan_audience_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/plan_audience_response_data.py` & `schematichq-1.0.0/src/schematic/types/plan_audience_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/plan_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/raw_event_batch_response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
-from .feature_detail_response_data import FeatureDetailResponseData
+from .raw_event_response_data import RawEventResponseData
 
 
-class PlanDetailResponseData(pydantic_v1.BaseModel):
+class RawEventBatchResponseData(pydantic_v1.BaseModel):
     """
-    The updated resource
+    The created resource
     """
 
-    company_count: int
-    created_at: dt.datetime
-    description: str
-    features: typing.List[FeatureDetailResponseData]
-    id: str
-    name: str
-    plan_type: str
-    updated_at: dt.datetime
+    events: typing.List[RawEventResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `schematichq-0.0.7/src/schematic/types/plan_entitlement_response_data.py` & `schematichq-1.0.0/src/schematic/types/plan_entitlement_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/plan_response_data.py` & `schematichq-1.0.0/src/schematic/types/plan_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/preview_object.py` & `schematichq-1.0.0/src/schematic/types/preview_object.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/raw_event_batch_response_data.py` & `schematichq-1.0.0/src/schematic/accounts/types/list_environments_params.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
-from .raw_event_response_data import RawEventResponseData
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
 
-class RawEventBatchResponseData(pydantic_v1.BaseModel):
+class ListEnvironmentsParams(pydantic_v1.BaseModel):
     """
-    The created resource
+    Input parameters
     """
 
-    events: typing.List[RawEventResponseData]
+    ids: typing.Optional[typing.List[str]] = None
+    limit: typing.Optional[int] = None
+    offset: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `schematichq-0.0.7/src/schematic/types/raw_event_response_data.py` & `schematichq-1.0.0/src/schematic/types/raw_event_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/rule_condition_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/rule_condition_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/rule_condition_group_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/rule_condition_group_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/rule_condition_group_response_data.py` & `schematichq-1.0.0/src/schematic/types/rule_condition_group_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/rule_condition_resource_response_data.py` & `schematichq-1.0.0/src/schematic/types/rule_condition_resource_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/rule_condition_response_data.py` & `schematichq-1.0.0/src/schematic/types/rule_condition_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/rule_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/rule_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/rule_response_data.py` & `schematichq-1.0.0/src/schematic/types/rule_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/rules_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/rules_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/update_req_common.py` & `schematichq-1.0.0/src/schematic/types/update_req_common.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/update_rule_request_body.py` & `schematichq-1.0.0/src/schematic/types/update_rule_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/upsert_company_request_body.py` & `schematichq-1.0.0/src/schematic/types/upsert_company_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/upsert_trait_request_body.py` & `schematichq-1.0.0/src/schematic/types/upsert_trait_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/upsert_user_request_body.py` & `schematichq-1.0.0/src/schematic/types/upsert_user_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/upsert_user_sub_request_body.py` & `schematichq-1.0.0/src/schematic/types/upsert_user_sub_request_body.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/user_detail_response_data.py` & `schematichq-1.0.0/src/schematic/types/user_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `schematichq-0.0.7/src/schematic/types/user_response_data.py` & `schematichq-1.0.0/src/schematic/types/user_response_data.py`

 * *Files identical despite different names*

