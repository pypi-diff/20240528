# Comparing `tmp/graphlit_client-1.0.20240519001.tar.gz` & `tmp/graphlit_client-1.0.20240528001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlit_client-1.0.20240519001.tar", last modified: Sun May 19 19:49:20 2024, max compression
+gzip compressed data, was "graphlit_client-1.0.20240528001.tar", last modified: Tue May 28 08:16:15 2024, max compression
```

## Comparing `graphlit_client-1.0.20240519001.tar` & `graphlit_client-1.0.20240528001.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:49:20.001531 graphlit_client-1.0.20240519001/
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-19 19:49:20.001531 graphlit_client-1.0.20240519001/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:49:19.977531 graphlit_client-1.0.20240519001/graphlit/
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1878 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit/graphlit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:49:20.001531 graphlit_client-1.0.20240519001/graphlit_api/
--rw-r--r--   0 vsts      (1001) docker     (127)    86074 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/add_contents_to_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/async_base_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/base_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/clear_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    99668 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/close_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      416 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      440 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/count_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8595 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/create_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      477 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_all_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)      506 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/delete_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/disable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/disable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/enable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/enable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17559 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/extract_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9942 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4286 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7098 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      387 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1164 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1119 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      763 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_share_point_consent_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5777 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8029 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/get_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      931 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/ingest_encoded_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      804 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/ingest_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)      790 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/ingest_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)    81097 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/input_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/is_content_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/is_feed_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/lookup_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1711 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/lookup_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    68926 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4043 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/prompt_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2390 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/prompt_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/publish_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/publish_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/publish_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10811 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12210 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_contents_facets.py
--rw-r--r--   0 vsts      (1001) docker     (127)      975 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_contents_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4895 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1004 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1576 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7902 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      553 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      834 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_microsoft_teams_channels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      782 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_microsoft_teams_teams.py
--rw-r--r--   0 vsts      (1001) docker     (127)      718 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_one_drive_folders.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1399 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1318 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1250 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      592 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      807 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_share_point_folders.py
--rw-r--r--   0 vsts      (1001) docker     (127)      961 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_share_point_libraries.py
--rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6292 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1645 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9007 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/query_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/remove_contents_from_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/suggest_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/summarize_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8595 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/graphlit_api/update_workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 19:49:20.001531 graphlit_client-1.0.20240519001/graphlit_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-19 19:49:19.000000 graphlit_client-1.0.20240519001/graphlit_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-05-19 19:49:19.000000 graphlit_client-1.0.20240519001/graphlit_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-19 19:49:19.000000 graphlit_client-1.0.20240519001/graphlit_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-05-19 19:49:19.000000 graphlit_client-1.0.20240519001/graphlit_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-19 19:49:19.000000 graphlit_client-1.0.20240519001/graphlit_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-19 19:49:20.001531 graphlit_client-1.0.20240519001/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-05-19 19:49:08.000000 graphlit_client-1.0.20240519001/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 08:16:15.953071 graphlit_client-1.0.20240528001/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-28 08:16:15.953071 graphlit_client-1.0.20240528001/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 08:16:15.925070 graphlit_client-1.0.20240528001/graphlit/
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1878 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit/graphlit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 08:16:15.953071 graphlit_client-1.0.20240528001/graphlit_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    86138 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/add_contents_to_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/async_base_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/base_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/clear_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    99668 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/close_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      416 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      440 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/count_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8575 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/create_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      477 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_all_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      506 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/delete_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/disable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/disable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/enable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/enable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17559 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/extract_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9942 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4286 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7098 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      387 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1164 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1119 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      763 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_share_point_consent_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5777 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8009 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/get_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      931 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/ingest_encoded_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      804 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/ingest_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      790 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/ingest_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    82206 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/input_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/is_content_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/is_feed_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/lookup_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1711 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/lookup_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    68926 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4043 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/prompt_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2390 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/prompt_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/publish_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/publish_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/publish_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10811 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12210 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_contents_facets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      975 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_contents_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4895 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1004 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1576 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7902 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      553 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      834 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_microsoft_teams_channels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      782 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_microsoft_teams_teams.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      718 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_one_drive_folders.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1399 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1318 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1250 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      592 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      807 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_share_point_folders.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      961 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_share_point_libraries.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6292 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1645 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8987 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/query_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/remove_contents_from_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/suggest_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/summarize_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8575 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/graphlit_api/update_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-28 08:16:15.953071 graphlit_client-1.0.20240528001/graphlit_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-28 08:16:15.000000 graphlit_client-1.0.20240528001/graphlit_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-05-28 08:16:15.000000 graphlit_client-1.0.20240528001/graphlit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-28 08:16:15.000000 graphlit_client-1.0.20240528001/graphlit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-05-28 08:16:15.000000 graphlit_client-1.0.20240528001/graphlit_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-28 08:16:15.000000 graphlit_client-1.0.20240528001/graphlit_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-28 08:16:15.953071 graphlit_client-1.0.20240528001/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-05-28 08:15:59.000000 graphlit_client-1.0.20240528001/setup.py
```

### Comparing `graphlit_client-1.0.20240519001/LICENSE` & `graphlit_client-1.0.20240528001/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/PKG-INFO` & `graphlit_client-1.0.20240528001/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240519001
+Version: 1.0.20240528001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240519001/README.md` & `graphlit_client-1.0.20240528001/README.md`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit/graphlit.py` & `graphlit_client-1.0.20240528001/graphlit/graphlit.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/__init__.py` & `graphlit_client-1.0.20240528001/graphlit_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,14 +498,15 @@
     CategoryUpdateInput,
     CohereModelPropertiesInput,
     CohereModelPropertiesUpdateInput,
     CollectionFilter,
     CollectionInput,
     CollectionUpdateInput,
     ContentCriteriaInput,
+    ContentCriteriaLevelInput,
     ContentFacetInput,
     ContentFilter,
     ContentFilterLevel,
     ContentGraphInput,
     ContentInput,
     ContentPublishingConnectorInput,
     ContentPublishingConnectorUpdateInput,
@@ -1321,14 +1322,15 @@
     "CohereModelPropertiesUpdateInput",
     "CohereModels",
     "CollectionFilter",
     "CollectionInput",
     "CollectionTypes",
     "CollectionUpdateInput",
     "ContentCriteriaInput",
+    "ContentCriteriaLevelInput",
     "ContentFacetInput",
     "ContentFacetTypes",
     "ContentFilter",
     "ContentFilterLevel",
     "ContentGraphInput",
     "ContentInput",
     "ContentPublishingConnectorInput",
```

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/add_contents_to_collections.py` & `graphlit_client-1.0.20240528001/graphlit_api/add_contents_to_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/async_base_client.py` & `graphlit_client-1.0.20240528001/graphlit_api/async_base_client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/base_model.py` & `graphlit_client-1.0.20240528001/graphlit_api/base_model.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/clear_conversation.py` & `graphlit_client-1.0.20240528001/graphlit_api/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/client.py` & `graphlit_client-1.0.20240528001/graphlit_api/client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/close_conversation.py` & `graphlit_client-1.0.20240528001/graphlit_api/close_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/create_collection.py` & `graphlit_client-1.0.20240528001/graphlit_api/create_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/create_conversation.py` & `graphlit_client-1.0.20240528001/graphlit_api/create_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/create_specification.py` & `graphlit_client-1.0.20240528001/graphlit_api/create_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/create_workflow.py` & `graphlit_client-1.0.20240528001/graphlit_api/create_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     if_: Optional["CreateWorkflowCreateWorkflowIngestionIf"] = Field(alias="if")
     collections: Optional[
         List[Optional["CreateWorkflowCreateWorkflowIngestionCollections"]]
     ]
 
 
 class CreateWorkflowCreateWorkflowIngestionIf(BaseModel):
-    types: Optional[List[Optional[ContentTypes]]]
-    file_types: Optional[List[Optional[FileTypes]]] = Field(alias="fileTypes")
+    types: Optional[List[ContentTypes]]
+    file_types: Optional[List[FileTypes]] = Field(alias="fileTypes")
 
 
 class CreateWorkflowCreateWorkflowIngestionCollections(BaseModel):
     id: str
 
 
 class CreateWorkflowCreateWorkflowPreparation(BaseModel):
```

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/delete_all_conversations.py` & `graphlit_client-1.0.20240528001/graphlit_api/delete_all_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/delete_all_organizations.py` & `graphlit_client-1.0.20240528001/graphlit_api/delete_all_organizations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/delete_all_specifications.py` & `graphlit_client-1.0.20240528001/graphlit_api/delete_all_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/enums.py` & `graphlit_client-1.0.20240528001/graphlit_api/enums.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/exceptions.py` & `graphlit_client-1.0.20240528001/graphlit_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/extract_contents.py` & `graphlit_client-1.0.20240528001/graphlit_api/extract_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_alert.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_alert.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_collection.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_content.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_conversation.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_event.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_event.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_feed.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_feed.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_organization.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_organization.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_person.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_person.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_place.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_place.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_product.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_product.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_project.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_project.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_software.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_software.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_specification.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/get_workflow.py` & `graphlit_client-1.0.20240528001/graphlit_api/get_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 
 class GetWorkflowWorkflowIngestion(BaseModel):
     if_: Optional["GetWorkflowWorkflowIngestionIf"] = Field(alias="if")
     collections: Optional[List[Optional["GetWorkflowWorkflowIngestionCollections"]]]
 
 
 class GetWorkflowWorkflowIngestionIf(BaseModel):
-    types: Optional[List[Optional[ContentTypes]]]
-    file_types: Optional[List[Optional[FileTypes]]] = Field(alias="fileTypes")
+    types: Optional[List[ContentTypes]]
+    file_types: Optional[List[FileTypes]] = Field(alias="fileTypes")
 
 
 class GetWorkflowWorkflowIngestionCollections(BaseModel):
     id: str
 
 
 class GetWorkflowWorkflowPreparation(BaseModel):
```

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/ingest_encoded_file.py` & `graphlit_client-1.0.20240528001/graphlit_api/ingest_encoded_file.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/ingest_text.py` & `graphlit_client-1.0.20240528001/graphlit_api/ingest_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/ingest_uri.py` & `graphlit_client-1.0.20240528001/graphlit_api/ingest_uri.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/input_types.py` & `graphlit_client-1.0.20240528001/graphlit_api/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,26 +142,26 @@
     types: Optional[List[ContentTypes]] = None
     file_types: Optional[List[FileTypes]] = Field(alias="fileTypes", default=None)
     uri: Optional[Any] = None
     location: Optional["PointFilter"] = None
     h_3: Optional["H3Filter"] = Field(alias="h3", default=None)
     boundaries: Optional[List[Optional[Any]]] = None
     contents: Optional[List["EntityReferenceFilter"]] = None
-    feeds: Optional[List["EntityReferenceFilter"]] = None
-    workflows: Optional[List["EntityReferenceFilter"]] = None
-    collections: Optional[List["EntityReferenceFilter"]] = None
-    observations: Optional[List["ObservationReferenceFilter"]] = None
     original_date_range: Optional["DateRangeFilter"] = Field(
         alias="originalDateRange", default=None
     )
     formats: Optional[List[Optional[str]]] = None
     file_extensions: Optional[List[str]] = Field(alias="fileExtensions", default=None)
     file_size_range: Optional["Int64RangeFilter"] = Field(
         alias="fileSizeRange", default=None
     )
+    feeds: Optional[List["EntityReferenceFilter"]] = None
+    workflows: Optional[List["EntityReferenceFilter"]] = None
+    collections: Optional[List["EntityReferenceFilter"]] = None
+    observations: Optional[List["ObservationReferenceFilter"]] = None
     or_: Optional[List[Optional["ContentFilterLevel"]]] = Field(
         alias="or", default=None
     )
     and_: Optional[List[Optional["ContentFilterLevel"]]] = Field(
         alias="and", default=None
     )
 
@@ -1003,14 +1003,16 @@
     types: Optional[List[ContentTypes]] = None
     file_types: Optional[List[FileTypes]] = Field(alias="fileTypes", default=None)
     contents: Optional[List["EntityReferenceInput"]] = None
     feeds: Optional[List["EntityReferenceInput"]] = None
     workflows: Optional[List["EntityReferenceInput"]] = None
     collections: Optional[List["EntityReferenceInput"]] = None
     observations: Optional[List["ObservationCriteriaInput"]] = None
+    or_: Optional[List["ContentCriteriaLevelInput"]] = Field(alias="or", default=None)
+    and_: Optional[List["ContentCriteriaLevelInput"]] = Field(alias="and", default=None)
 
 
 class ContentPublishingConnectorInput(BaseModel):
     type: ContentPublishingServiceTypes
     format: ContentPublishingFormats
     eleven_labs: Optional["ElevenLabsPublishingPropertiesInput"] = Field(
         alias="elevenLabs", default=None
@@ -1100,14 +1102,16 @@
 class RSSFeedPropertiesInput(BaseModel):
     uri: Any
     read_limit: Optional[int] = Field(alias="readLimit", default=None)
 
 
 class WebFeedPropertiesInput(BaseModel):
     uri: Any
+    allowed_paths: Optional[List[str]] = Field(alias="allowedPaths", default=None)
+    excluded_paths: Optional[List[str]] = Field(alias="excludedPaths", default=None)
     include_files: Optional[bool] = Field(alias="includeFiles", default=None)
     read_limit: Optional[int] = Field(alias="readLimit", default=None)
 
 
 class RedditFeedPropertiesInput(BaseModel):
     subreddit_name: str = Field(alias="subredditName")
     read_limit: Optional[int] = Field(alias="readLimit", default=None)
@@ -1397,14 +1401,16 @@
 
 class RSSFeedPropertiesUpdateInput(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit", default=None)
 
 
 class WebFeedPropertiesUpdateInput(BaseModel):
     uri: Optional[Any] = None
+    allowed_paths: Optional[List[str]] = Field(alias="allowedPaths", default=None)
+    excluded_paths: Optional[List[str]] = Field(alias="excludedPaths", default=None)
     include_files: Optional[bool] = Field(alias="includeFiles", default=None)
     read_limit: Optional[int] = Field(alias="readLimit", default=None)
 
 
 class RedditFeedPropertiesUpdateInput(BaseModel):
     read_limit: Optional[int] = Field(alias="readLimit", default=None)
 
@@ -1596,14 +1602,21 @@
 
 class ObservationCriteriaInput(BaseModel):
     type: Optional[ObservableTypes] = None
     observable: Optional["EntityReferenceInput"] = None
     states: Optional[List[Optional[EntityState]]] = None
 
 
+class ContentCriteriaLevelInput(BaseModel):
+    feeds: Optional[List["EntityReferenceInput"]] = None
+    workflows: Optional[List["EntityReferenceInput"]] = None
+    collections: Optional[List["EntityReferenceInput"]] = None
+    observations: Optional[List["ObservationCriteriaInput"]] = None
+
+
 class ElevenLabsPublishingPropertiesInput(BaseModel):
     model: Optional[ElevenLabsModels] = None
     voice: Optional[str] = None
 
 
 class SlackIntegrationPropertiesInput(BaseModel):
     channel: str
@@ -1695,18 +1708,18 @@
     left: Optional[float] = None
     top: Optional[float] = None
     width: Optional[float] = None
     height: Optional[float] = None
 
 
 class IngestionContentFilterInput(BaseModel):
-    types: Optional[List[Optional[ContentTypes]]] = None
-    file_types: Optional[List[Optional[FileTypes]]] = Field(
-        alias="fileTypes", default=None
-    )
+    types: Optional[List[ContentTypes]] = None
+    file_types: Optional[List[FileTypes]] = Field(alias="fileTypes", default=None)
+    allowed_paths: Optional[List[str]] = Field(alias="allowedPaths", default=None)
+    excluded_paths: Optional[List[str]] = Field(alias="excludedPaths", default=None)
 
 
 class SummarizationStrategyInput(BaseModel):
     type: SummarizationTypes
     specification: Optional["EntityReferenceInput"] = None
     tokens: Optional[int] = None
     items: Optional[int] = None
@@ -1719,14 +1732,16 @@
 
 class ExtractionWorkflowJobInput(BaseModel):
     connector: Optional["EntityExtractionConnectorInput"] = None
 
 
 class LinkStrategyInput(BaseModel):
     enable_crawling: Optional[bool] = Field(alias="enableCrawling", default=None)
+    allowed_paths: Optional[List[str]] = Field(alias="allowedPaths", default=None)
+    excluded_paths: Optional[List[str]] = Field(alias="excludedPaths", default=None)
     allowed_domains: Optional[List[str]] = Field(alias="allowedDomains", default=None)
     excluded_domains: Optional[List[str]] = Field(alias="excludedDomains", default=None)
     allow_content_domain: Optional[bool] = Field(
         alias="allowContentDomain", default=None
     )
     allowed_links: Optional[List[LinkTypes]] = Field(alias="allowedLinks", default=None)
     excluded_links: Optional[List[LinkTypes]] = Field(
```

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/lookup_credits.py` & `graphlit_client-1.0.20240528001/graphlit_api/lookup_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/lookup_usage.py` & `graphlit_client-1.0.20240528001/graphlit_api/lookup_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/operations.py` & `graphlit_client-1.0.20240528001/graphlit_api/operations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/prompt_conversation.py` & `graphlit_client-1.0.20240528001/graphlit_api/prompt_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/prompt_specifications.py` & `graphlit_client-1.0.20240528001/graphlit_api/prompt_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/publish_contents.py` & `graphlit_client-1.0.20240528001/graphlit_api/publish_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/publish_conversation.py` & `graphlit_client-1.0.20240528001/graphlit_api/publish_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/publish_text.py` & `graphlit_client-1.0.20240528001/graphlit_api/publish_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_alerts.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_alerts.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_categories.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_categories.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_collections.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_contents.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_contents_facets.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_contents_facets.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_contents_graph.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_contents_graph.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_conversations.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_credits.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_events.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_events.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_feeds.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_feeds.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_labels.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_labels.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_microsoft_teams_channels.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_microsoft_teams_channels.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_microsoft_teams_teams.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_microsoft_teams_teams.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_one_drive_folders.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_one_drive_folders.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_organizations.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_organizations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_persons.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_persons.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_places.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_places.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_products.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_products.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_repos.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_repos.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_share_point_folders.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_share_point_folders.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_share_point_libraries.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_share_point_libraries.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_softwares.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_softwares.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_specifications.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_usage.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/query_workflows.py` & `graphlit_client-1.0.20240528001/graphlit_api/query_workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
     if_: Optional["QueryWorkflowsWorkflowsResultsIngestionIf"] = Field(alias="if")
     collections: Optional[
         List[Optional["QueryWorkflowsWorkflowsResultsIngestionCollections"]]
     ]
 
 
 class QueryWorkflowsWorkflowsResultsIngestionIf(BaseModel):
-    types: Optional[List[Optional[ContentTypes]]]
-    file_types: Optional[List[Optional[FileTypes]]] = Field(alias="fileTypes")
+    types: Optional[List[ContentTypes]]
+    file_types: Optional[List[FileTypes]] = Field(alias="fileTypes")
 
 
 class QueryWorkflowsWorkflowsResultsIngestionCollections(BaseModel):
     id: str
 
 
 class QueryWorkflowsWorkflowsResultsPreparation(BaseModel):
```

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/remove_contents_from_collection.py` & `graphlit_client-1.0.20240528001/graphlit_api/remove_contents_from_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/summarize_contents.py` & `graphlit_client-1.0.20240528001/graphlit_api/summarize_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/update_collection.py` & `graphlit_client-1.0.20240528001/graphlit_api/update_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/update_content.py` & `graphlit_client-1.0.20240528001/graphlit_api/update_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/update_conversation.py` & `graphlit_client-1.0.20240528001/graphlit_api/update_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/update_specification.py` & `graphlit_client-1.0.20240528001/graphlit_api/update_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/graphlit_api/update_workflow.py` & `graphlit_client-1.0.20240528001/graphlit_api/update_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     if_: Optional["UpdateWorkflowUpdateWorkflowIngestionIf"] = Field(alias="if")
     collections: Optional[
         List[Optional["UpdateWorkflowUpdateWorkflowIngestionCollections"]]
     ]
 
 
 class UpdateWorkflowUpdateWorkflowIngestionIf(BaseModel):
-    types: Optional[List[Optional[ContentTypes]]]
-    file_types: Optional[List[Optional[FileTypes]]] = Field(alias="fileTypes")
+    types: Optional[List[ContentTypes]]
+    file_types: Optional[List[FileTypes]] = Field(alias="fileTypes")
 
 
 class UpdateWorkflowUpdateWorkflowIngestionCollections(BaseModel):
     id: str
 
 
 class UpdateWorkflowUpdateWorkflowPreparation(BaseModel):
```

### Comparing `graphlit_client-1.0.20240519001/graphlit_client.egg-info/PKG-INFO` & `graphlit_client-1.0.20240528001/graphlit_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240519001
+Version: 1.0.20240528001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240519001/graphlit_client.egg-info/SOURCES.txt` & `graphlit_client-1.0.20240528001/graphlit_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240519001/setup.py` & `graphlit_client-1.0.20240528001/setup.py`

 * *Files identical despite different names*

