# Comparing `tmp/asyncflows-0.1.5.tar.gz` & `tmp/asyncflows-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncflows-0.1.5.tar", max compression
+gzip compressed data, was "asyncflows-0.1.6.tar", max compression
```

## Comparing `asyncflows-0.1.5.tar` & `asyncflows-0.1.6.tar`

### file list

```diff
@@ -1,99 +1,100 @@
--rw-r--r--   0        0        0     4019 2024-05-22 14:49:22.081858 asyncflows-0.1.5/LICENSE
--rw-r--r--   0        0        0    32806 2024-05-25 22:56:21.937598 asyncflows-0.1.5/README.md
--rw-r--r--   0        0        0      215 2024-05-22 14:47:42.260962 asyncflows-0.1.5/asyncflows/__init__.py
--rw-r--r--   0        0        0      721 2024-05-22 14:46:03.753765 asyncflows-0.1.5/asyncflows/actions/__init__.py
--rw-r--r--   0        0        0     6399 2024-05-22 14:47:42.261515 asyncflows-0.1.5/asyncflows/actions/base.py
--rw-r--r--   0        0        0     2143 2024-05-25 22:56:21.938190 asyncflows-0.1.5/asyncflows/actions/execute_db_statement.py
--rw-r--r--   0        0        0     1385 2024-05-22 14:49:22.057325 asyncflows-0.1.5/asyncflows/actions/extract_list.py
--rw-r--r--   0        0        0     1982 2024-05-22 18:55:04.922974 asyncflows-0.1.5/asyncflows/actions/extract_pdf_text.py
--rw-r--r--   0        0        0     1428 2024-05-22 14:47:42.368774 asyncflows-0.1.5/asyncflows/actions/extract_xml_tag.py
--rw-r--r--   0        0        0     1267 2024-05-25 22:56:21.943880 asyncflows-0.1.5/asyncflows/actions/get_db_schema.py
--rw-r--r--   0        0        0      582 2024-05-22 14:47:42.261922 asyncflows-0.1.5/asyncflows/actions/get_url.py
--rw-r--r--   0        0        0      860 2024-05-22 14:47:42.317491 asyncflows-0.1.5/asyncflows/actions/ocr.py
--rw-r--r--   0        0        0    16519 2024-05-25 22:46:36.212088 asyncflows-0.1.5/asyncflows/actions/prompt.py
--rw-r--r--   0        0        0     1297 2024-05-22 14:47:42.262400 asyncflows-0.1.5/asyncflows/actions/score.py
--rw-r--r--   0        0        0     4309 2024-05-22 18:55:04.923294 asyncflows-0.1.5/asyncflows/actions/transformer.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.755456 asyncflows-0.1.5/asyncflows/actions/utils/__init__.py
--rw-r--r--   0        0        0     5351 2024-05-22 21:28:30.270167 asyncflows-0.1.5/asyncflows/actions/utils/prompt_context.py
--rw-r--r--   0        0        0     4447 2024-05-25 20:36:32.571393 asyncflows-0.1.5/asyncflows/asyncflows.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.755962 asyncflows-0.1.5/asyncflows/examples/__init__.py
--rw-r--r--   0        0        0   287615 2024-05-22 18:55:04.925115 asyncflows-0.1.5/asyncflows/examples/books/Alice's Adventures in Wonderland, by Lewis Carroll.pdf
--rw-r--r--   0        0        0     1533 2024-05-22 18:55:04.925408 asyncflows-0.1.5/asyncflows/examples/chatbot.py
--rw-r--r--   0        0        0     3150 2024-05-25 22:40:56.343582 asyncflows-0.1.5/asyncflows/examples/chatbot.yaml
--rw-r--r--   0        0        0      716 2024-05-22 14:47:42.404980 asyncflows-0.1.5/asyncflows/examples/debono.py
--rw-r--r--   0        0        0     3415 2024-05-25 22:40:56.344104 asyncflows-0.1.5/asyncflows/examples/debono.yaml
--rw-r--r--   0        0        0      699 2024-05-22 14:47:42.405239 asyncflows-0.1.5/asyncflows/examples/get_page_title.py
--rw-r--r--   0        0        0      490 2024-05-25 22:40:56.344484 asyncflows-0.1.5/asyncflows/examples/get_page_title.yaml
--rw-r--r--   0        0        0   294692 2024-05-25 22:40:56.345676 asyncflows-0.1.5/asyncflows/examples/hello_world.ipynb
--rw-r--r--   0        0        0      651 2024-05-25 20:56:51.983126 asyncflows-0.1.5/asyncflows/examples/hello_world.py
--rw-r--r--   0        0        0      327 2024-05-25 22:40:56.346635 asyncflows-0.1.5/asyncflows/examples/hello_world.yaml
--rw-r--r--   0        0        0     1309 2024-05-25 22:40:56.347377 asyncflows-0.1.5/asyncflows/examples/rag.py
--rw-r--r--   0        0        0     1137 2024-05-25 22:40:56.347667 asyncflows-0.1.5/asyncflows/examples/rag.yaml
--rw-r--r--   0        0        0      280 2024-05-22 14:46:03.758066 asyncflows-0.1.5/asyncflows/examples/recipes/caprese.md
--rw-r--r--   0        0        0      380 2024-05-22 14:46:03.758468 asyncflows-0.1.5/asyncflows/examples/recipes/chana_masala.md
--rw-r--r--   0        0        0      329 2024-05-22 14:46:03.758593 asyncflows-0.1.5/asyncflows/examples/recipes/coconut_soup.md
--rw-r--r--   0        0        0      413 2024-05-22 14:46:03.758715 asyncflows-0.1.5/asyncflows/examples/recipes/gazpacho.md
--rw-r--r--   0        0        0      326 2024-05-22 14:46:03.758850 asyncflows-0.1.5/asyncflows/examples/recipes/guacamole.md
--rw-r--r--   0        0        0      375 2024-05-22 14:46:03.758989 asyncflows-0.1.5/asyncflows/examples/recipes/hummus.md
--rw-r--r--   0        0        0      326 2024-05-22 14:46:03.759115 asyncflows-0.1.5/asyncflows/examples/recipes/miso_soup.md
--rw-r--r--   0        0        0      331 2024-05-22 14:46:03.759255 asyncflows-0.1.5/asyncflows/examples/recipes/omelette.md
--rw-r--r--   0        0        0      327 2024-05-22 14:46:03.759525 asyncflows-0.1.5/asyncflows/examples/recipes/stir_fry.md
--rw-r--r--   0        0        0      321 2024-05-22 14:46:03.759651 asyncflows-0.1.5/asyncflows/examples/recipes/yogurt_parfait.md
--rw-r--r--   0        0        0     1105 2024-05-22 14:47:42.413403 asyncflows-0.1.5/asyncflows/examples/sql_rag.py
--rw-r--r--   0        0        0     1606 2024-05-25 22:56:21.938495 asyncflows-0.1.5/asyncflows/examples/sql_rag.yaml
--rw-r--r--   0        0        0     1198 2024-05-22 21:28:30.271238 asyncflows-0.1.5/asyncflows/examples/text_style_transfer.py
--rw-r--r--   0        0        0      575 2024-05-25 22:40:56.348440 asyncflows-0.1.5/asyncflows/examples/text_style_transfer.yaml
--rw-r--r--   0        0        0     1890 2024-05-22 14:46:03.761643 asyncflows-0.1.5/asyncflows/log_config.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.761683 asyncflows-0.1.5/asyncflows/models/__init__.py
--rw-r--r--   0        0        0      204 2024-05-22 14:46:03.761990 asyncflows-0.1.5/asyncflows/models/blob.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.762029 asyncflows-0.1.5/asyncflows/models/config/__init__.py
--rw-r--r--   0        0        0     3960 2024-05-25 20:36:32.571870 asyncflows-0.1.5/asyncflows/models/config/action.py
--rw-r--r--   0        0        0     2681 2024-05-22 14:46:03.762355 asyncflows-0.1.5/asyncflows/models/config/common.py
--rw-r--r--   0        0        0     2208 2024-05-25 20:36:32.572264 asyncflows-0.1.5/asyncflows/models/config/flow.py
--rw-r--r--   0        0        0     2491 2024-05-25 20:36:32.572548 asyncflows-0.1.5/asyncflows/models/config/model.py
--rw-r--r--   0        0        0     5075 2024-05-22 14:49:41.999198 asyncflows-0.1.5/asyncflows/models/config/transform.py
--rw-r--r--   0        0        0     5022 2024-05-22 14:49:22.058252 asyncflows-0.1.5/asyncflows/models/config/value_declarations.py
--rw-r--r--   0        0        0     3303 2024-05-22 14:49:22.058580 asyncflows-0.1.5/asyncflows/models/file.py
--rw-r--r--   0        0        0      700 2024-05-22 14:47:42.230677 asyncflows-0.1.5/asyncflows/models/primitives.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.763641 asyncflows-0.1.5/asyncflows/repos/__init__.py
--rw-r--r--   0        0        0    20233 2024-05-22 14:46:03.764021 asyncflows-0.1.5/asyncflows/repos/blob_repo.py
--rw-r--r--   0        0        0     4421 2024-05-22 14:46:03.764605 asyncflows-0.1.5/asyncflows/repos/cache_repo.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.764679 asyncflows-0.1.5/asyncflows/scripts/__init__.py
--rw-r--r--   0        0        0     4975 2024-05-23 10:43:58.865278 asyncflows-0.1.5/asyncflows/scripts/generate_config_schema.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.764985 asyncflows-0.1.5/asyncflows/services/__init__.py
--rw-r--r--   0        0        0    38941 2024-05-25 22:46:36.212742 asyncflows-0.1.5/asyncflows/services/action_service.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.765630 asyncflows-0.1.5/asyncflows/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.765743 asyncflows-0.1.5/asyncflows/tests/action_tests/__init__.py
--rw-r--r--   0        0        0      888 2024-05-25 22:56:21.938792 asyncflows-0.1.5/asyncflows/tests/action_tests/test_execute_db_statement.py
--rw-r--r--   0        0        0     1260 2024-05-22 14:47:42.369030 asyncflows-0.1.5/asyncflows/tests/action_tests/test_extract_xml_tag.py
--rw-r--r--   0        0        0      683 2024-05-22 14:48:15.166773 asyncflows-0.1.5/asyncflows/tests/action_tests/test_get_db_schema.py
--rw-r--r--   0        0        0     7985 2024-05-25 22:40:56.350212 asyncflows-0.1.5/asyncflows/tests/action_tests/test_prompt.py
--rw-r--r--   0        0        0     1902 2024-05-22 14:46:03.766510 asyncflows-0.1.5/asyncflows/tests/action_tests/test_transformers.py
--rw-r--r--   0        0        0    11472 2024-05-25 22:40:56.350881 asyncflows-0.1.5/asyncflows/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.766988 asyncflows-0.1.5/asyncflows/tests/repos/__init__.py
--rw-r--r--   0        0        0     8319 2024-05-22 14:46:03.767510 asyncflows-0.1.5/asyncflows/tests/repos/test_blob_repo.py
--rw-r--r--   0        0        0     6567 2024-05-22 14:46:03.767743 asyncflows-0.1.5/asyncflows/tests/repos/test_cache_repo.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.767812 asyncflows-0.1.5/asyncflows/tests/resources/__init__.py
--rw-r--r--   0        0        0     5737 2024-05-22 14:47:42.263059 asyncflows-0.1.5/asyncflows/tests/resources/actions.py
--rw-r--r--   0        0        0      263 2024-05-25 22:40:56.351632 asyncflows-0.1.5/asyncflows/tests/resources/default_model_var.yaml
--rw-r--r--   0        0        0     4079 2024-05-23 10:43:58.791187 asyncflows-0.1.5/asyncflows/tests/resources/testing_actions.yaml
--rw-r--r--   0        0        0    26138 2024-05-25 22:32:38.860953 asyncflows-0.1.5/asyncflows/tests/test_action_service.py
--rw-r--r--   0        0        0     6172 2024-05-25 22:40:56.352181 asyncflows-0.1.5/asyncflows/tests/test_async_utils.py
--rw-r--r--   0        0        0     1069 2024-05-25 22:40:56.352473 asyncflows-0.1.5/asyncflows/tests/test_asyncflows_interface.py
--rw-r--r--   0        0        0    11747 2024-05-22 18:55:04.928969 asyncflows-0.1.5/asyncflows/tests/test_config.py
--rw-r--r--   0        0        0     2053 2024-05-22 14:48:15.167483 asyncflows-0.1.5/asyncflows/tests/test_run_examples.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.769749 asyncflows-0.1.5/asyncflows/utils/__init__.py
--rw-r--r--   0        0        0     9877 2024-05-25 22:46:36.213306 asyncflows-0.1.5/asyncflows/utils/async_utils.py
--rw-r--r--   0        0        0      676 2024-05-22 14:46:03.770301 asyncflows-0.1.5/asyncflows/utils/cache_utils.py
--rw-r--r--   0        0        0     8602 2024-05-25 20:36:32.574834 asyncflows-0.1.5/asyncflows/utils/config_utils.py
--rw-r--r--   0        0        0      725 2024-05-22 14:47:42.393837 asyncflows-0.1.5/asyncflows/utils/db_utils.py
--rw-r--r--   0        0        0     1320 2024-05-22 14:46:03.771069 asyncflows-0.1.5/asyncflows/utils/jinja_utils.py
--rw-r--r--   0        0        0     1482 2024-05-22 14:46:03.771192 asyncflows-0.1.5/asyncflows/utils/redis_utils.py
--rw-r--r--   0        0        0     2686 2024-05-22 14:46:03.771325 asyncflows-0.1.5/asyncflows/utils/request_utils.py
--rw-r--r--   0        0        0      382 2024-05-22 14:46:03.771449 asyncflows-0.1.5/asyncflows/utils/secret_utils.py
--rw-r--r--   0        0        0      479 2024-05-22 14:46:03.771565 asyncflows-0.1.5/asyncflows/utils/sentinel_utils.py
--rw-r--r--   0        0        0      451 2024-05-22 14:46:03.771681 asyncflows-0.1.5/asyncflows/utils/singleton_utils.py
--rw-r--r--   0        0        0     3333 2024-05-22 14:47:42.303806 asyncflows-0.1.5/asyncflows/utils/transformers_utils.py
--rw-r--r--   0        0        0     2507 2024-05-22 14:46:03.772050 asyncflows-0.1.5/asyncflows/utils/type_utils.py
--rw-r--r--   0        0        0     2547 2024-05-25 22:56:21.947894 asyncflows-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    34917 1970-01-01 00:00:00.000000 asyncflows-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4019 2024-05-22 14:49:22.081858 asyncflows-0.1.6/LICENSE
+-rw-r--r--   0        0        0    34674 2024-05-28 14:05:37.409849 asyncflows-0.1.6/README.md
+-rw-r--r--   0        0        0      333 2024-05-28 11:42:33.951883 asyncflows-0.1.6/asyncflows/__init__.py
+-rw-r--r--   0        0        0     1538 2024-05-28 13:37:58.806851 asyncflows-0.1.6/asyncflows/actions/__init__.py
+-rw-r--r--   0        0        0     6399 2024-05-22 14:47:42.261515 asyncflows-0.1.6/asyncflows/actions/base.py
+-rw-r--r--   0        0        0     2143 2024-05-25 22:56:21.938190 asyncflows-0.1.6/asyncflows/actions/execute_db_statement.py
+-rw-r--r--   0        0        0     1385 2024-05-27 13:38:11.354900 asyncflows-0.1.6/asyncflows/actions/extract_list.py
+-rw-r--r--   0        0        0     1982 2024-05-22 18:55:04.922974 asyncflows-0.1.6/asyncflows/actions/extract_pdf_text.py
+-rw-r--r--   0        0        0     1428 2024-05-22 14:47:42.368774 asyncflows-0.1.6/asyncflows/actions/extract_xml_tag.py
+-rw-r--r--   0        0        0     1267 2024-05-25 22:56:21.943880 asyncflows-0.1.6/asyncflows/actions/get_db_schema.py
+-rw-r--r--   0        0        0      582 2024-05-22 14:47:42.261922 asyncflows-0.1.6/asyncflows/actions/get_url.py
+-rw-r--r--   0        0        0      860 2024-05-22 14:47:42.317491 asyncflows-0.1.6/asyncflows/actions/ocr.py
+-rw-r--r--   0        0        0    16519 2024-05-25 22:46:36.212088 asyncflows-0.1.6/asyncflows/actions/prompt.py
+-rw-r--r--   0        0        0     1297 2024-05-22 14:47:42.262400 asyncflows-0.1.6/asyncflows/actions/score.py
+-rw-r--r--   0        0        0     4454 2024-05-26 11:18:24.566364 asyncflows-0.1.6/asyncflows/actions/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.755456 asyncflows-0.1.6/asyncflows/actions/utils/__init__.py
+-rw-r--r--   0        0        0     5351 2024-05-22 21:28:30.270167 asyncflows-0.1.6/asyncflows/actions/utils/prompt_context.py
+-rw-r--r--   0        0        0     4819 2024-05-28 13:31:55.096094 asyncflows-0.1.6/asyncflows/asyncflows.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.755962 asyncflows-0.1.6/asyncflows/examples/__init__.py
+-rw-r--r--   0        0        0   287615 2024-05-22 18:55:04.925115 asyncflows-0.1.6/asyncflows/examples/books/Alice's Adventures in Wonderland, by Lewis Carroll.pdf
+-rw-r--r--   0        0        0     1533 2024-05-22 18:55:04.925408 asyncflows-0.1.6/asyncflows/examples/chatbot.py
+-rw-r--r--   0        0        0     3150 2024-05-25 22:40:56.343582 asyncflows-0.1.6/asyncflows/examples/chatbot.yaml
+-rw-r--r--   0        0        0      716 2024-05-22 14:47:42.404980 asyncflows-0.1.6/asyncflows/examples/debono.py
+-rw-r--r--   0        0        0     3415 2024-05-25 22:40:56.344104 asyncflows-0.1.6/asyncflows/examples/debono.yaml
+-rw-r--r--   0        0        0      699 2024-05-22 14:47:42.405239 asyncflows-0.1.6/asyncflows/examples/get_page_title.py
+-rw-r--r--   0        0        0      490 2024-05-25 22:40:56.344484 asyncflows-0.1.6/asyncflows/examples/get_page_title.yaml
+-rw-r--r--   0        0        0     4730 2024-05-28 13:36:36.226166 asyncflows-0.1.6/asyncflows/examples/hello_world.ipynb
+-rw-r--r--   0        0        0      651 2024-05-25 20:56:51.983126 asyncflows-0.1.6/asyncflows/examples/hello_world.py
+-rw-r--r--   0        0        0      327 2024-05-27 16:55:16.674972 asyncflows-0.1.6/asyncflows/examples/hello_world.yaml
+-rw-r--r--   0        0        0     1309 2024-05-25 22:40:56.347377 asyncflows-0.1.6/asyncflows/examples/rag.py
+-rw-r--r--   0        0        0     1137 2024-05-25 22:40:56.347667 asyncflows-0.1.6/asyncflows/examples/rag.yaml
+-rw-r--r--   0        0        0      280 2024-05-22 14:46:03.758066 asyncflows-0.1.6/asyncflows/examples/recipes/caprese.md
+-rw-r--r--   0        0        0      380 2024-05-22 14:46:03.758468 asyncflows-0.1.6/asyncflows/examples/recipes/chana_masala.md
+-rw-r--r--   0        0        0      329 2024-05-22 14:46:03.758593 asyncflows-0.1.6/asyncflows/examples/recipes/coconut_soup.md
+-rw-r--r--   0        0        0      413 2024-05-22 14:46:03.758715 asyncflows-0.1.6/asyncflows/examples/recipes/gazpacho.md
+-rw-r--r--   0        0        0      326 2024-05-22 14:46:03.758850 asyncflows-0.1.6/asyncflows/examples/recipes/guacamole.md
+-rw-r--r--   0        0        0      375 2024-05-22 14:46:03.758989 asyncflows-0.1.6/asyncflows/examples/recipes/hummus.md
+-rw-r--r--   0        0        0      326 2024-05-22 14:46:03.759115 asyncflows-0.1.6/asyncflows/examples/recipes/miso_soup.md
+-rw-r--r--   0        0        0      331 2024-05-22 14:46:03.759255 asyncflows-0.1.6/asyncflows/examples/recipes/omelette.md
+-rw-r--r--   0        0        0      327 2024-05-22 14:46:03.759525 asyncflows-0.1.6/asyncflows/examples/recipes/stir_fry.md
+-rw-r--r--   0        0        0      321 2024-05-22 14:46:03.759651 asyncflows-0.1.6/asyncflows/examples/recipes/yogurt_parfait.md
+-rw-r--r--   0        0        0     1105 2024-05-22 14:47:42.413403 asyncflows-0.1.6/asyncflows/examples/sql_rag.py
+-rw-r--r--   0        0        0     1606 2024-05-27 14:59:46.611396 asyncflows-0.1.6/asyncflows/examples/sql_rag.yaml
+-rw-r--r--   0        0        0     1198 2024-05-22 21:28:30.271238 asyncflows-0.1.6/asyncflows/examples/text_style_transfer.py
+-rw-r--r--   0        0        0      575 2024-05-27 13:40:49.695787 asyncflows-0.1.6/asyncflows/examples/text_style_transfer.yaml
+-rw-r--r--   0        0        0     1890 2024-05-22 14:46:03.761643 asyncflows-0.1.6/asyncflows/log_config.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.761683 asyncflows-0.1.6/asyncflows/models/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-22 14:46:03.761990 asyncflows-0.1.6/asyncflows/models/blob.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.762029 asyncflows-0.1.6/asyncflows/models/config/__init__.py
+-rw-r--r--   0        0        0     3694 2024-05-28 13:31:55.097088 asyncflows-0.1.6/asyncflows/models/config/action.py
+-rw-r--r--   0        0        0     2681 2024-05-22 14:46:03.762355 asyncflows-0.1.6/asyncflows/models/config/common.py
+-rw-r--r--   0        0        0     3085 2024-05-28 13:31:55.097760 asyncflows-0.1.6/asyncflows/models/config/flow.py
+-rw-r--r--   0        0        0     2491 2024-05-25 20:36:32.572548 asyncflows-0.1.6/asyncflows/models/config/model.py
+-rw-r--r--   0        0        0     5075 2024-05-22 14:49:41.999198 asyncflows-0.1.6/asyncflows/models/config/transform.py
+-rw-r--r--   0        0        0     5083 2024-05-26 12:24:53.735904 asyncflows-0.1.6/asyncflows/models/config/value_declarations.py
+-rw-r--r--   0        0        0     3303 2024-05-22 14:49:22.058580 asyncflows-0.1.6/asyncflows/models/file.py
+-rw-r--r--   0        0        0      700 2024-05-22 14:47:42.230677 asyncflows-0.1.6/asyncflows/models/primitives.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.763641 asyncflows-0.1.6/asyncflows/repos/__init__.py
+-rw-r--r--   0        0        0    20233 2024-05-22 14:46:03.764021 asyncflows-0.1.6/asyncflows/repos/blob_repo.py
+-rw-r--r--   0        0        0     4421 2024-05-22 14:46:03.764605 asyncflows-0.1.6/asyncflows/repos/cache_repo.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.764679 asyncflows-0.1.6/asyncflows/scripts/__init__.py
+-rw-r--r--   0        0        0     3372 2024-05-28 13:31:55.098021 asyncflows-0.1.6/asyncflows/scripts/generate_config_schema.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.764985 asyncflows-0.1.6/asyncflows/services/__init__.py
+-rw-r--r--   0        0        0    38678 2024-05-28 13:31:55.098627 asyncflows-0.1.6/asyncflows/services/action_service.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.765630 asyncflows-0.1.6/asyncflows/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.765743 asyncflows-0.1.6/asyncflows/tests/action_tests/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-25 22:56:21.938792 asyncflows-0.1.6/asyncflows/tests/action_tests/test_execute_db_statement.py
+-rw-r--r--   0        0        0     1260 2024-05-22 14:47:42.369030 asyncflows-0.1.6/asyncflows/tests/action_tests/test_extract_xml_tag.py
+-rw-r--r--   0        0        0      683 2024-05-22 14:48:15.166773 asyncflows-0.1.6/asyncflows/tests/action_tests/test_get_db_schema.py
+-rw-r--r--   0        0        0     7985 2024-05-25 22:40:56.350212 asyncflows-0.1.6/asyncflows/tests/action_tests/test_prompt.py
+-rw-r--r--   0        0        0     1902 2024-05-22 14:46:03.766510 asyncflows-0.1.6/asyncflows/tests/action_tests/test_transformers.py
+-rw-r--r--   0        0        0    11816 2024-05-28 13:31:55.099438 asyncflows-0.1.6/asyncflows/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.766988 asyncflows-0.1.6/asyncflows/tests/repos/__init__.py
+-rw-r--r--   0        0        0     8319 2024-05-22 14:46:03.767510 asyncflows-0.1.6/asyncflows/tests/repos/test_blob_repo.py
+-rw-r--r--   0        0        0     6567 2024-05-22 14:46:03.767743 asyncflows-0.1.6/asyncflows/tests/repos/test_cache_repo.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.767812 asyncflows-0.1.6/asyncflows/tests/resources/__init__.py
+-rw-r--r--   0        0        0     5737 2024-05-22 14:47:42.263059 asyncflows-0.1.6/asyncflows/tests/resources/actions.py
+-rw-r--r--   0        0        0      265 2024-05-28 13:31:55.099736 asyncflows-0.1.6/asyncflows/tests/resources/default_model_var.yaml
+-rw-r--r--   0        0        0     4079 2024-05-23 10:43:58.791187 asyncflows-0.1.6/asyncflows/tests/resources/testing_actions.yaml
+-rw-r--r--   0        0        0    26138 2024-05-25 22:32:38.860953 asyncflows-0.1.6/asyncflows/tests/test_action_service.py
+-rw-r--r--   0        0        0     6172 2024-05-25 22:40:56.352181 asyncflows-0.1.6/asyncflows/tests/test_async_utils.py
+-rw-r--r--   0        0        0      978 2024-05-28 13:31:55.100329 asyncflows-0.1.6/asyncflows/tests/test_asyncflows_interface.py
+-rw-r--r--   0        0        0    11747 2024-05-22 18:55:04.928969 asyncflows-0.1.6/asyncflows/tests/test_config.py
+-rw-r--r--   0        0        0     2053 2024-05-22 14:48:15.167483 asyncflows-0.1.6/asyncflows/tests/test_run_examples.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.769749 asyncflows-0.1.6/asyncflows/utils/__init__.py
+-rw-r--r--   0        0        0     9879 2024-05-28 13:38:40.873250 asyncflows-0.1.6/asyncflows/utils/async_utils.py
+-rw-r--r--   0        0        0      676 2024-05-22 14:46:03.770301 asyncflows-0.1.6/asyncflows/utils/cache_utils.py
+-rw-r--r--   0        0        0     8177 2024-05-28 13:31:55.100833 asyncflows-0.1.6/asyncflows/utils/config_utils.py
+-rw-r--r--   0        0        0      725 2024-05-22 14:47:42.393837 asyncflows-0.1.6/asyncflows/utils/db_utils.py
+-rw-r--r--   0        0        0     1320 2024-05-22 14:46:03.771069 asyncflows-0.1.6/asyncflows/utils/jinja_utils.py
+-rw-r--r--   0        0        0      725 2024-05-28 13:31:55.101217 asyncflows-0.1.6/asyncflows/utils/loader_utils.py
+-rw-r--r--   0        0        0     1482 2024-05-22 14:46:03.771192 asyncflows-0.1.6/asyncflows/utils/redis_utils.py
+-rw-r--r--   0        0        0     2686 2024-05-22 14:46:03.771325 asyncflows-0.1.6/asyncflows/utils/request_utils.py
+-rw-r--r--   0        0        0      382 2024-05-22 14:46:03.771449 asyncflows-0.1.6/asyncflows/utils/secret_utils.py
+-rw-r--r--   0        0        0      479 2024-05-22 14:46:03.771565 asyncflows-0.1.6/asyncflows/utils/sentinel_utils.py
+-rw-r--r--   0        0        0      451 2024-05-22 14:46:03.771681 asyncflows-0.1.6/asyncflows/utils/singleton_utils.py
+-rw-r--r--   0        0        0     3658 2024-05-26 11:25:18.264784 asyncflows-0.1.6/asyncflows/utils/transformers_utils.py
+-rw-r--r--   0        0        0     2507 2024-05-22 14:46:03.772050 asyncflows-0.1.6/asyncflows/utils/type_utils.py
+-rw-r--r--   0        0        0     2614 2024-05-28 14:14:46.690295 asyncflows-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    36785 1970-01-01 00:00:00.000000 asyncflows-0.1.6/PKG-INFO
```

### Comparing `asyncflows-0.1.5/LICENSE` & `asyncflows-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/README.md` & `asyncflows-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 2.2 [Local development](#local-development)  
 3. [Examples](#examples)  
 3.1 [Text Style Transfer](#text-style-transfer)  
 3.2 [De Bono's Six Thinking Hats](#de-bonos-six-thinking-hats)  
 3.3 [Retrieval Augmented Generation (RAG)](#retrieval-augmented-generation-rag)  
 3.4 [SQL Retrieval](#sql-retrieval)  
 3.5 [Chatbot](#chatbot)  
-3.6 [Writing your own actions](#writing-your-own-actions)  
 4. [Guides](#guides)  
-4.1 [Writing Flows with Autocomplete](#writing-flows-with-autocomplete)  
-4.2 [Setting up Ollama for Local Inference](#setting-up-ollama-for-local-inference)  
-4.3 [Using Any Language Model](#using-any-language-model)  
-4.4 [Prompting in-depth](#prompting-in-depth)  
+4.1 [Custom Actions](#custom-actions)  
+4.2 [Writing Flows with Autocomplete](#writing-flows-with-autocomplete)  
+4.3 [Caching with Redis](#caching-with-redis)  
+4.4 [Setting up Ollama for Local Inference](#setting-up-ollama-for-local-inference)  
+4.5 [Using Any Language Model](#using-any-language-model)  
+4.6 [Prompting in-depth](#prompting-in-depth)  
 5. [License](#license)
 
 
 # Introduction
 
 asyncflows is a framework for designing and running AI pipelines using simple YAML configuration.
 
@@ -208,15 +209,16 @@
 The examples default to Llama 3, and assume [Ollama](https://ollama.com/) is running locally.
 
 See [Setting up Ollama for Local Inference](#setting-up-ollama-for-local-inference) to setup Ollama.  
 See [Using Any Language Model](#using-any-language-model) to use a different model or provider.
 
 ## Text Style Transfer
 
-[![template](https://img.shields.io/badge/template-blue)](https://github.com/asynchronous-flows/text-style-transfer-example)
+[![template repo](https://img.shields.io/badge/template_repo-blue)](https://github.com/asynchronous-flows/text-style-transfer-example)
+[![Try in Colab](https://img.shields.io/badge/colab-red)](https://colab.research.google.com/github/asynchronous-flows/text-style-transfer-example/blob/main/text_style_transfer.ipynb)
 
 This example takes a writing sample, and writes about a topic in the style of the sample.
 
 <div align="center">
 <img width="706" alt="style transfer" src="https://github.com/asynchronous-flows/asyncflows/assets/24586651/f0e2a9ef-d714-48c4-9e03-96dfc5bde5f1">
 </div>
 
@@ -596,14 +598,16 @@
 
 ---
 
 </details>
 
 ## SQL Retrieval
 
+[![template repo](https://img.shields.io/badge/template_repo-blue)](https://github.com/asynchronous-flows/sql-rag-example)
+
 This flow facilitates asking questions over a SQL database.
 
 To use it with your database, install the corresponding [extra packages](#sql-databases) and set the `DATABASE_URL` environment variable.
 
 <div align="center">
 <img width="1368" alt="sql rag" src="https://github.com/asynchronous-flows/asyncflows/assets/24586651/96241659-d470-4dac-a459-b63222db4670">
 </div>
@@ -731,15 +735,15 @@
 
 ---
 
 </details>
 
 ## Chatbot
 
-[![template](https://img.shields.io/badge/template-blue)](https://github.com/asynchronous-flows/pdf-chatbot-example)
+[![template repo](https://img.shields.io/badge/template_repo-blue)](https://github.com/asynchronous-flows/pdf-chatbot-example)
 
 This flow facilitates a chatbot over a set of PDF documents.
 
 Given a list of filepaths, it extracts their text, uses retrieval augmented generation (RAG) to find the ones relevant to the question, and generates an answer.
 
 The form of RAG we're using is **retrieval** followed by **reranking**.
 Retrieval is great for searching through a large dataset, while reranking is slower but better at matching against the query.
@@ -913,19 +917,24 @@
 
 The Red Queen's perspective on punishment reveals a stark contrast between her cruel nature and the more benevolent attitudes of other characters, such as the King, who intervenes to save Alice from execution. The Queen's actions also create a sense of danger and chaos, making Wonderland an unpredictable and potentially deadly place for its inhabitants.
 
 ---
 
 </details>
 
-## Writing your own actions
+# Guides
+
+## Custom Actions
+
+[![template repo](https://img.shields.io/badge/template_repo-blue)](https://github.com/asynchronous-flows/api-call-example)
 
-You can create custom actions by subclassing `Action` and defining the input and output models using Pydantic.
+You can create custom actions by subclassing `Action`, and defining the input and output models using Pydantic.
+
+Here is an example action that visits a webpage and returns its text content:
 
-Python code for the custom action:
 ```python
 from asyncflows import Action, BaseModel, Field
 
 import aiohttp
 
 
 class Inputs(BaseModel):
@@ -945,15 +954,19 @@
 
     async def run(self, inputs: Inputs) -> Outputs:
         async with aiohttp.ClientSession() as session:
             async with session.get(inputs.url) as response:
                 return Outputs(result=await response.text())
 ```
 
-YAML file of an example flow using this action:
+<details>
+<summary>
+YAML file of an example flow using this action – click to expand
+</summary>
+
 ```yaml
 # get_page_title.yaml
 
 default_model:
   model: ollama/llama3
 flow:
   get_website:
@@ -966,24 +979,26 @@
       - heading: Website content
         link: get_website.result
       - text: |
           What is the title of the webpage?
 default_output: extract_title.result
 ```
 
+</details>
+
 <details>
 <summary>
 Running the flow (python and stdout)
 </summary>
 
 Python script that runs the flow:
 ```python
 from asyncflows import AsyncFlows
 
-flow = AsyncFlows.from_file("soup.yaml")
+flow = AsyncFlows.from_file("get_page_title.yaml")
 
 # Run the flow and return the default output (result of the extract_title action)
 result = await flow.set_vars(
     url="https://en.wikipedia.org/wiki/Python_(programming_language)",
 ).run()
 print(result)
 ```
@@ -991,29 +1006,69 @@
 Output of the python script:
 ```
 The title of the webpage is "Python (programming language) - Wikipedia".
 ```
 
 </details>
 
-# Guides
+As long as your custom actions are imported before instantiating the flow,
+they will be available for use.
+
+Alternatively, to ensure the action is always available, 
+and for it to show up when using the language server for YAML autocomplete,
+register an entrypoint for the module that contains your actions.  
+For example, using poetry, with your actions located in `my_package.actions`,
+include the following at the end of your `pyproject.toml`:
+
+```toml
+[tool.poetry.plugins."asyncflows"]
+actions = "my_package.actions"
+```
+
+See the [API Call Example](https://github.com/asynchronous-flows/api-call-example) for a custom actions template repository.
 
 ## Writing Flows with Autocomplete
 
 For an easier time writing flows, use YAML Language Server in your editor with our JsonSchema.
 
 Put the following at the top of your YAML flow config file:
 
 ```yaml
 # yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/asyncflows_schema.json
 ```
 
 The JsonSchema will only catch some errors, 
 stay tuned for a domain-specific language server that will provide more advanced features.
 
+## Caching with Redis
+
+By default, AsyncFlows caches action outputs with a shelve file in a temporary directory.
+
+To cache between runs, we support Redis as a backend:
+
+1. Run [Redis](https://redis.io/download) locally or use a cloud provider.
+
+2. Set the following environment variables:
+
+- `REDIS_HOST` (required)
+- `REDIS_PASSWORD` (required)
+- `REDIS_PORT` (optional, defaults to 6379)
+- `REDIS_USERNAME` (optional, defaults to empty string)
+
+3. Override the default cache with:
+
+```python
+from asyncflows import AsyncFlows, RedisCacheRepo
+
+flow = AsyncFlows.from_file(
+   "flow.yaml",
+   cache_repo=RedisCacheRepo,
+)
+```
+
 ## Setting up Ollama for Local Inference
 
 To run the examples, you need to have [Ollama](https://ollama.com/) running locally.
 
 1. [Download and Install Ollama](https://ollama.com/download) 
 2. On some platforms like macOS Ollama runs in the background automatically. 
    If not, start it with:
```

### Comparing `asyncflows-0.1.5/asyncflows/actions/base.py` & `asyncflows-0.1.6/asyncflows/actions/base.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/actions/execute_db_statement.py` & `asyncflows-0.1.6/asyncflows/actions/execute_db_statement.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/actions/extract_list.py` & `asyncflows-0.1.6/asyncflows/actions/extract_list.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/actions/extract_pdf_text.py` & `asyncflows-0.1.6/asyncflows/actions/extract_pdf_text.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/actions/extract_xml_tag.py` & `asyncflows-0.1.6/asyncflows/actions/extract_xml_tag.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/actions/get_db_schema.py` & `asyncflows-0.1.6/asyncflows/actions/get_db_schema.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/actions/get_url.py` & `asyncflows-0.1.6/asyncflows/actions/get_url.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/actions/ocr.py` & `asyncflows-0.1.6/asyncflows/actions/ocr.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/actions/prompt.py` & `asyncflows-0.1.6/asyncflows/actions/prompt.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/actions/score.py` & `asyncflows-0.1.6/asyncflows/actions/score.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/actions/transformer.py` & `asyncflows-0.1.6/asyncflows/actions/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import Any
+from typing import Any, Literal
 
 from asyncflows.actions.base import Action, BaseModel
 from asyncflows.models.config.model import BiEncoderModelType, CrossEncoderModelType
 
 # from asyncflows.scripts.run_transformers_service import DocumentQueryRequest
 from asyncflows.utils.transformers_utils import retrieve_indices, rerank_indices
 
 
 class BaseTransformerInputs(BaseModel):
     model: str
+    device: Literal["cpu", "cuda", "mps", "tensorrt"] | None = None
     # TODO use typevar
     documents: list[Any]
     texts: None | list[str] = None
     query: str
     # server_url: None | str
     k: int = 10
 
@@ -89,14 +90,15 @@
         #         url=url,
         #     )
         # else:
         # run the transformer in the same process
         indices = await retrieve_indices(
             log=self.log,
             model=inputs.model,
+            device=inputs.device,
             documents=texts,
             query=inputs.query,
             k=inputs.k,
         )
 
         result = [inputs.documents[i] for i in indices]
         return Outputs(result=result)
@@ -125,14 +127,15 @@
         #         url=url,
         #     )
         # else:
         # run the transformer in the same process
         indices = await rerank_indices(
             log=self.log,
             model=inputs.model,
+            device=inputs.device,
             documents=texts,
             query=inputs.query,
             k=inputs.k,
         )
 
         result = [inputs.documents[i] for i in indices]
         return Outputs(result=result)
```

### Comparing `asyncflows-0.1.5/asyncflows/actions/utils/prompt_context.py` & `asyncflows-0.1.6/asyncflows/actions/utils/prompt_context.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/asyncflows.py` & `asyncflows-0.1.6/asyncflows/asyncflows.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from asyncflows.models.config.flow import ActionConfig
 from asyncflows.services.action_service import ActionService
 
 from asyncflows.log_config import get_logger
 from asyncflows.models.config.value_declarations import VarDeclaration
 from asyncflows.repos.blob_repo import InMemoryBlobRepo, BlobRepo
 from asyncflows.repos.cache_repo import ShelveCacheRepo, CacheRepo
-from asyncflows.utils.config_utils import load_config_file, load_config_text
+from asyncflows.utils.loader_utils import load_config_file, load_config_text
 
 
 class AsyncFlows:
     def __init__(
         self,
         config: ActionConfig,
         cache_repo: CacheRepo | type[CacheRepo] = ShelveCacheRepo,
@@ -62,30 +62,38 @@
         if isinstance(self.temp_dir, TemporaryDirectory):
             self.temp_dir.cleanup()
 
     @classmethod
     def from_text(
         cls,
         text: str,
+        cache_repo: CacheRepo | type[CacheRepo] = ShelveCacheRepo,
+        blob_repo: BlobRepo | type[BlobRepo] = InMemoryBlobRepo,
     ):
-        config = load_config_text(ActionConfig, text)
+        config = load_config_text(text)
         return AsyncFlows(
             config=config,
+            cache_repo=cache_repo,
+            blob_repo=blob_repo,
         )
 
     @classmethod
     def from_file(
         cls,
         file: str | Path,
+        cache_repo: CacheRepo | type[CacheRepo] = ShelveCacheRepo,
+        blob_repo: BlobRepo | type[BlobRepo] = InMemoryBlobRepo,
     ) -> "AsyncFlows":
         if isinstance(file, Path):
             file = file.as_posix()
-        config = load_config_file(ActionConfig, file)
+        config = load_config_file(file)
         return AsyncFlows(
             config=config,
+            cache_repo=cache_repo,
+            blob_repo=blob_repo,
         )
 
     def set_vars(self, **kwargs) -> "AsyncFlows":
         variables = self.variables | kwargs
         return AsyncFlows(
             config=self.action_config,
             cache_repo=self.cache_repo,
```

### Comparing `asyncflows-0.1.5/asyncflows/examples/books/Alice's Adventures in Wonderland, by Lewis Carroll.pdf` & `asyncflows-0.1.6/asyncflows/examples/books/Alice's Adventures in Wonderland, by Lewis Carroll.pdf`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/examples/chatbot.py` & `asyncflows-0.1.6/asyncflows/examples/chatbot.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/examples/chatbot.yaml` & `asyncflows-0.1.6/asyncflows/examples/chatbot.yaml`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/examples/debono.py` & `asyncflows-0.1.6/asyncflows/examples/debono.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/examples/debono.yaml` & `asyncflows-0.1.6/asyncflows/examples/debono.yaml`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/examples/get_page_title.py` & `asyncflows-0.1.6/asyncflows/examples/get_page_title.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/examples/hello_world.py` & `asyncflows-0.1.6/asyncflows/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/examples/rag.py` & `asyncflows-0.1.6/asyncflows/examples/rag.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/examples/rag.yaml` & `asyncflows-0.1.6/asyncflows/examples/rag.yaml`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/examples/sql_rag.py` & `asyncflows-0.1.6/asyncflows/examples/sql_rag.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/examples/sql_rag.yaml` & `asyncflows-0.1.6/asyncflows/examples/sql_rag.yaml`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/examples/text_style_transfer.py` & `asyncflows-0.1.6/asyncflows/examples/text_style_transfer.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/examples/text_style_transfer.yaml` & `asyncflows-0.1.6/asyncflows/examples/text_style_transfer.yaml`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/log_config.py` & `asyncflows-0.1.6/asyncflows/log_config.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/models/config/action.py` & `asyncflows-0.1.6/asyncflows/models/config/action.py`

 * *Files 11% similar despite different names*

```diff
@@ -66,24 +66,27 @@
     ]
     union_elements.extend(other_elements)
 
     return Union[tuple(union_elements)]  # type: ignore
 
 
 def build_actions(
-    action_names: list[str],
+    action_names: list[str] | None = None,
     vars_: HintType | None = None,
     links: HintType | None = None,
     strict: bool = False,
 ):
     # Dynamically build action models from currently defined actions
     # for best typehints and autocompletion possible in the jsonschema
 
     HintedValueDeclaration = build_hinted_value_declaration(vars_, links, strict)
 
+    if action_names is None:
+        action_names = list(get_actions_dict().keys())
+
     actions_dict = get_actions_dict()
     action_models = []
     for action_name in action_names:
         action = actions_dict[action_name]
         # build base model field
         fields = {
             "action": (Literal[action.name], ...),  # type: ignore
@@ -104,24 +107,13 @@
         # build action invocation model
         action_basemodel = pydantic.create_model(
             action.name + "ActionInvocation",
             __base__=ActionInvocation,
             __module__=__name__,
             model_config=ConfigDict(
                 arbitrary_types_allowed=True,
+                extra="forbid",
             ),
             **fields,  # pyright: ignore[reportGeneralTypeIssues]
         )
         action_models.append(action_basemodel)
     return action_models
-
-
-_action_names = list(get_actions_dict().keys())
-ActionInvocationUnion = Union[tuple(build_actions(_action_names))]  # pyright: ignore
-
-
-# TODO assert tests not imported before this line
-import asyncflows.tests.resources.actions  # noqa
-
-
-_testing_action_names = list(get_actions_dict().keys())
-TestingActionInvocationUnion = Union[tuple(build_actions(_testing_action_names))]  # pyright: ignore
```

### Comparing `asyncflows-0.1.5/asyncflows/models/config/common.py` & `asyncflows-0.1.6/asyncflows/models/config/common.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/models/config/flow.py` & `asyncflows-0.1.6/asyncflows/models/config/flow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from typing import Union
 
 import pydantic
 from pydantic import Field
 
 from asyncflows.models.config.action import (
-    ActionInvocationUnion,
-    TestingActionInvocationUnion,
+    ActionInvocation,
+    build_actions,
 )
 from asyncflows.models.config.common import StrictModel
 from asyncflows.models.config.model import ModelConfig
 from asyncflows.models.config.value_declarations import ValueDeclaration
-from asyncflows.models.primitives import ContextVarName, ContextVarPath, ExecutableId
+from asyncflows.models.primitives import (
+    ContextVarName,
+    ContextVarPath,
+    ExecutableId,
+    HintType,
+)
 from asyncflows.models.config.action import build_hinted_value_declaration
 from asyncflows.models.config.value_declarations import (
     LinkDeclaration,
     LambdaDeclaration,
 )
 from asyncflows.utils.config_utils import templatify_model
 
@@ -27,18 +32,14 @@
     in_: ValueDeclaration = Field(
         ...,
         alias="in",
     )
     flow: "FlowConfig"
 
 
-class TestLoop(Loop):
-    flow: "TestFlowConfig"
-
-
 def build_model_config(
     strict: bool = False,
 ):
     # Dynamically build the model config like ActionModel, with the ValueDeclarations
 
     HintedValueDeclaration = build_hinted_value_declaration(
         strict=strict, excluded_declaration_types=[LinkDeclaration, LambdaDeclaration]
@@ -66,19 +67,53 @@
 ModelConfigDeclaration = build_model_config()
 
 
 class ActionConfig(StrictModel):
     default_model: ModelConfigDeclaration  # type: ignore
     action_timeout: float = 360
     flow: "FlowConfig"
-    default_output: ContextVarPath
+    default_output: ContextVarPath  # TODO `| ValueDeclaration`
 
 
-class TestActionConfig(ActionConfig):
-    flow: "TestFlowConfig"
+Executable = Union[ActionInvocation, Loop]
+FlowConfig = dict[ExecutableId, Executable]
 
 
-Executable = Union[ActionInvocationUnion, Loop]
-FlowConfig = dict[ExecutableId, Executable]
+def build_hinted_action_config(
+    action_names: list[str] | None = None,
+    vars_: HintType | None = None,
+    links: HintType | None = None,
+    strict: bool = False,
+):
+    HintedValueDeclaration = build_hinted_value_declaration(
+        # vars_=vars_,
+        links=links,
+        strict=strict,
+    )
+
+    ActionInvocationUnion = Union[
+        tuple(
+            build_actions(
+                action_names=action_names,
+                vars_=vars_,
+                links=links,
+                strict=strict,
+            )
+        )  # pyright: ignore
+    ]
+
+    class HintedLoop(Loop):
+        in_: HintedValueDeclaration = Field(  # type: ignore
+            ...,
+            alias="in",
+        )
+        flow: "HintedFlowConfig"  # type: ignore
+
+    class HintedActionConfig(ActionConfig):
+        flow: "HintedFlowConfig"  # type: ignore
+
+    HintedExecutable = Union[ActionInvocationUnion, HintedLoop]
+    HintedFlowConfig = dict[ExecutableId, HintedExecutable]
+
+    HintedActionConfig.model_rebuild()  # TODO is this necessary?
 
-TestExecutable = Union[TestingActionInvocationUnion, TestLoop]
-TestFlowConfig = dict[ExecutableId, TestExecutable]
+    return HintedActionConfig
```

### Comparing `asyncflows-0.1.5/asyncflows/models/config/model.py` & `asyncflows-0.1.6/asyncflows/models/config/model.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/models/config/transform.py` & `asyncflows-0.1.6/asyncflows/models/config/transform.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/models/config/value_declarations.py` & `asyncflows-0.1.6/asyncflows/models/config/value_declarations.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,16 @@
     def get_dependencies(self) -> set[ContextVarName]:
         parsed_code = ast.parse(self.lambda_, mode="eval")
         return get_names_from_ast(parsed_code)
 
     async def render(self, context: dict[str, Any]) -> Any:
         verify_ast(ast.parse(self.lambda_))
 
+        simpleeval.MAX_COMPREHENSION_LENGTH = 9999999999999
+
         evaluator = simpleeval.EvalWithCompoundTypes(
             names=context,
             functions={
                 "range": range,
             },
         )
         return evaluator.eval(self.lambda_)
```

### Comparing `asyncflows-0.1.5/asyncflows/models/file.py` & `asyncflows-0.1.6/asyncflows/models/file.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/models/primitives.py` & `asyncflows-0.1.6/asyncflows/models/primitives.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/repos/blob_repo.py` & `asyncflows-0.1.6/asyncflows/repos/blob_repo.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/repos/cache_repo.py` & `asyncflows-0.1.6/asyncflows/repos/cache_repo.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/services/action_service.py` & `asyncflows-0.1.6/asyncflows/services/action_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import traceback
 from collections import defaultdict
 from typing import Any, AsyncIterator, Iterable
+
 from typing_extensions import assert_never
 
 import sentry_sdk
 import structlog
 from pydantic import BaseModel, RootModel, ValidationError
 
 from asyncflows.actions import get_actions_dict
@@ -142,14 +143,15 @@
         )
         try:
             if isinstance(action, StreamingAction):
                 async for outputs in measure_async_iterator(
                     log,
                     action.run(inputs),
                     timer,
+                    timeout=self.config.action_timeout,
                 ):
                     # async for outputs in action.run(inputs):
                     log.debug(
                         "Yielding outputs",
                         partial=True,
                         # outputs=outputs,
                     )
@@ -339,21 +341,14 @@
 
         input_spec = {
             key: getattr(action_config, key)
             for key in action_config.model_fields
             if key not in ("id", "action") and getattr(action_config, key) is not None
         }
 
-        # FIXME remove this,
-        #  unnecessary since all strings are interpreted as templates in _dependency_ids_from_input_spec
-        # for key, value in input_spec.items():
-        #     if isinstance(value, str):
-        #         value = TemplateDeclaration(text=value)
-        #     input_spec[key] = value
-
         dependencies = self._get_dependency_ids_and_stream_flag_from_input_spec(
             input_spec
         )
         if not dependencies:
             rendered = await self._collect_inputs_from_context(
                 log,
                 input_spec=input_spec,
```

### Comparing `asyncflows-0.1.5/asyncflows/tests/action_tests/test_execute_db_statement.py` & `asyncflows-0.1.6/asyncflows/tests/action_tests/test_execute_db_statement.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/tests/action_tests/test_extract_xml_tag.py` & `asyncflows-0.1.6/asyncflows/tests/action_tests/test_extract_xml_tag.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/tests/action_tests/test_get_db_schema.py` & `asyncflows-0.1.6/asyncflows/tests/action_tests/test_get_db_schema.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/tests/action_tests/test_prompt.py` & `asyncflows-0.1.6/asyncflows/tests/action_tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/tests/action_tests/test_transformers.py` & `asyncflows-0.1.6/asyncflows/tests/action_tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/tests/conftest.py` & `asyncflows-0.1.6/asyncflows/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 import pytest
 import tenacity
 import yaml
 from sqlalchemy import Column, Integer, String, create_engine
 from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession
 from sqlalchemy.orm import declarative_base, sessionmaker
 
+from asyncflows.actions import get_actions_dict
 from asyncflows.actions.prompt import Outputs as PromptOutputs, Prompt
 from asyncflows.actions.transformer import (
     BaseTransformerInputs as TransformerInputs,
     Outputs as TransformerOutputs,
     Retrieve,
     Rerank,
 )
 from asyncflows.log_config import configure_logging, get_logger
 from asyncflows.models.blob import Blob
-from asyncflows.models.config.flow import TestActionConfig
+from asyncflows.models.config.flow import build_hinted_action_config
 from asyncflows.repos.blob_repo import (
     InMemoryBlobRepo,
     RedisBlobRepo,
     FilesystemBlobRepo,
     S3BlobRepo,
 )
 from asyncflows.repos.cache_repo import ShelveCacheRepo
@@ -253,16 +254,24 @@
     async def block(*args, **kwargs):
         await asyncio.sleep(1)
         return MagicMock()
 
     return block
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
 def testing_actions():
+    # TODO assert tests not imported before this line
+    import asyncflows.tests.resources.actions  # noqa
+
+    testing_action_names = list(get_actions_dict().keys())
+
+    TestActionConfig = build_hinted_action_config(
+        action_names=testing_action_names,
+    )
     with open("asyncflows/tests/resources/testing_actions.yaml") as f:
         return TestActionConfig.model_validate(yaml.safe_load(f))
 
 
 @pytest.fixture
 def simple_flow(testing_flows):
     return testing_flows.subflows["chat_and_react_flow"]
```

### Comparing `asyncflows-0.1.5/asyncflows/tests/repos/test_blob_repo.py` & `asyncflows-0.1.6/asyncflows/tests/repos/test_blob_repo.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/tests/repos/test_cache_repo.py` & `asyncflows-0.1.6/asyncflows/tests/repos/test_cache_repo.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/tests/resources/actions.py` & `asyncflows-0.1.6/asyncflows/tests/resources/actions.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/tests/resources/testing_actions.yaml` & `asyncflows-0.1.6/asyncflows/tests/resources/testing_actions.yaml`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/tests/test_action_service.py` & `asyncflows-0.1.6/asyncflows/tests/test_action_service.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/tests/test_async_utils.py` & `asyncflows-0.1.6/asyncflows/tests/test_async_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/tests/test_asyncflows_interface.py` & `asyncflows-0.1.6/asyncflows/tests/test_asyncflows_interface.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from unittest.mock import patch
 
 from asyncflows import AsyncFlows
-from asyncflows.models.config.flow import TestActionConfig
-from asyncflows.utils.config_utils import load_config_file
+from asyncflows.utils.loader_utils import load_config_file
 
 from asyncflows.actions.prompt import (
     Outputs as PromptOutputs,
     Prompt,
     Inputs as PromptInputs,
 )
 
 
 async def test_default_model_var(log_history):
-    config = load_config_file(
-        TestActionConfig, "asyncflows/tests/resources/default_model_var.yaml"
-    )
+    config = load_config_file("asyncflows/tests/resources/default_model_var.yaml")
     af = AsyncFlows(config=config).set_vars(
         some_model="hi",
     )
 
     outputs = PromptOutputs(
         result="3",
     )
```

### Comparing `asyncflows-0.1.5/asyncflows/tests/test_config.py` & `asyncflows-0.1.6/asyncflows/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/tests/test_run_examples.py` & `asyncflows-0.1.6/asyncflows/tests/test_run_examples.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/utils/async_utils.py` & `asyncflows-0.1.6/asyncflows/utils/async_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         return self.wall_end_time - self.wall_start_time
 
 
 async def measure_coro(
     log: structlog.stdlib.BoundLogger,
     f: Awaitable[T],
     timer: Timer,
-    timeout: int = 180,
+    timeout: float = 180,
 ) -> T:
     coro_wrapper = f.__await__()
     arg = None
     exc = None
     fut = None
     first_run = True
 
@@ -197,15 +197,15 @@
                     log.debug(
                         "Subcoroutine cancelled during wait",
                         arg=arg,
                         # exc_info=e,
                     )
                     # fut.set_exception(e)
                 except Exception as e:
-                    log.warning(
+                    log.debug(
                         "Subcoroutine raised exception",
                         arg=arg,
                         # exc_info=e,
                     )
                     exc = e
             timer.start()
             if exc is not None:
@@ -220,15 +220,15 @@
             arg = None
 
 
 async def measure_async_iterator(
     log: structlog.stdlib.BoundLogger,
     f: AsyncIterator[T],
     timer: Timer,
-    timeout: int = 180,
+    timeout: float = 180,
 ) -> AsyncIterator[T]:
     iter_wrapper = f.__aiter__()
     while True:
         try:
             yield await measure_coro(
                 log,
                 iter_wrapper.__anext__(),
```

### Comparing `asyncflows-0.1.5/asyncflows/utils/cache_utils.py` & `asyncflows-0.1.6/asyncflows/utils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/utils/config_utils.py` & `asyncflows-0.1.6/asyncflows/utils/config_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import ast
 import builtins
-import os
 import types
 import typing
 from typing import Optional, Any, Union
 
 import pydantic
-import yaml
 from pydantic import BaseModel, ConfigDict, Field
 
 from asyncflows.models.config.transform import resolve_transforms_from
 from asyncflows.models.primitives import HintType
 from asyncflows.utils.type_utils import filter_none_from_type
 
 
@@ -215,14 +213,15 @@
     ast.Name,
     ast.Attribute,
     ast.Load,
     ast.Store,
     ast.ListComp,
     ast.comprehension,
     ast.List,
+    ast.Dict,
     ast.Subscript,
     ast.Tuple,
     ast.BinOp,
     ast.Add,
     ast.Compare,
     ast.Eq,
     ast.NotEq,
@@ -240,22 +239,7 @@
 def collect_ast_types(node: ast.AST) -> set[type]:
     types = set()
     if isinstance(node, _allowed_ast_types):
         types.add(type(node))
         for child in ast.iter_child_nodes(node):
             types |= collect_ast_types(child)
     return types
-
-
-T = typing.TypeVar("T", bound=BaseModel)
-
-
-def load_config_text(model: type[T], config_text: str) -> T:
-    return model.model_validate(yaml.safe_load(config_text))
-
-
-def load_config_file(model: type[T], filename: str) -> T:
-    if not os.path.exists(filename):
-        raise FileNotFoundError(f"Could not find {filename}")
-
-    with open(filename, "r") as f:
-        return model.model_validate(yaml.safe_load(f))
```

### Comparing `asyncflows-0.1.5/asyncflows/utils/db_utils.py` & `asyncflows-0.1.6/asyncflows/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/utils/jinja_utils.py` & `asyncflows-0.1.6/asyncflows/utils/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/utils/redis_utils.py` & `asyncflows-0.1.6/asyncflows/utils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/utils/request_utils.py` & `asyncflows-0.1.6/asyncflows/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/asyncflows/utils/transformers_utils.py` & `asyncflows-0.1.6/asyncflows/utils/transformers_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import contextlib
 from collections import defaultdict
-from typing import AsyncIterator, Any
+from typing import AsyncIterator, Any, Literal
 
 import numpy as np
 # from infinity_emb import AsyncEmbeddingEngine, EngineArgs
 
 AsyncEmbeddingEngine = Any
 
 
@@ -25,28 +25,35 @@
             log.info("Shutting down engine", model=model)
             await engine.astop()
             log.info("Successfully shut down engine", model=model)
 
 
 @contextlib.asynccontextmanager
 async def get_engine(
-    log, model: str, keep_engine_alive_delay: float
+    log,
+    model: str,
+    device: Literal["cpu", "cuda", "mps", "tensorrt"] | None,
+    keep_engine_alive_delay: float,
 ) -> AsyncIterator[AsyncEmbeddingEngine]:
     from infinity_emb import AsyncEmbeddingEngine, EngineArgs
+    from infinity_emb.primitives import Device
 
     if model in active_engines:
         engine = active_engines[model]
         if not engine.running:
             # idk if this will ever trigger but here we are
             log.debug("Engine not running, waiting for it to start")
             await asyncio.sleep(0.1)
             if not engine.running:
                 raise ValueError("Engine not starting up, something is wrong")
     else:
-        args = EngineArgs(model_name_or_path=model)
+        args = EngineArgs(
+            model_name_or_path=model,
+            device=Device(device),
+        )
         engine = AsyncEmbeddingEngine.from_args(args)
         active_engines[model] = engine
         log.info("Starting engine", model=model)
         await engine.astart()
 
     _engine_usage_counts[model] += 1
     try:
@@ -57,22 +64,23 @@
             shutdown_engine(log, keep_engine_alive_delay, model, engine)
         )
 
 
 async def retrieve_indices(
     log,
     model: str,
+    device: Literal["cpu", "cuda", "mps", "tensorrt"] | None,
     documents: list[str],
     query: str,
     k: int,
     keep_engine_alive_delay: float = DEFAULT_KEEP_ENGINE_ALIVE_DELAY,
 ) -> list[int]:
     # embed query and documents
     documents.append(query)
-    async with get_engine(log, model, keep_engine_alive_delay) as engine:
+    async with get_engine(log, model, device, keep_engine_alive_delay) as engine:
         embeddings, usage = await engine.embed(sentences=documents)
     log.info("Embedded documents", usage=usage)
     query_embedding = embeddings.pop()
 
     # calculate cosine similarity between query and documents
     query_norm = np.linalg.norm(query_embedding)
     scores = [
@@ -84,19 +92,20 @@
     # return indices of most similar documents
     return sorted(range(len(scores)), key=lambda i: scores[i], reverse=True)[:k]
 
 
 async def rerank_indices(
     log,
     model: str,
+    device: Literal["cpu", "cuda", "mps", "tensorrt"] | None,
     documents: list[str],
     query: str,
     k: int,
     keep_engine_alive_delay: float = DEFAULT_KEEP_ENGINE_ALIVE_DELAY,
 ) -> list[int]:
     # rerank documents based on query
-    async with get_engine(log, model, keep_engine_alive_delay) as engine:
+    async with get_engine(log, model, device, keep_engine_alive_delay) as engine:
         scores, usage = await engine.rerank(query=query, docs=documents)
     log.info("Reranked documents", usage=usage)
 
     # return indices of most relevant documents
     return sorted(range(len(scores)), key=lambda i: scores[i], reverse=True)[:k]
```

### Comparing `asyncflows-0.1.5/asyncflows/utils/type_utils.py` & `asyncflows-0.1.6/asyncflows/utils/type_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.5/pyproject.toml` & `asyncflows-0.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncflows"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Rafael Irgolic <hello@irgolic.com>"]
 readme = "README.md"
 license = "BSL-1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
@@ -82,7 +82,10 @@
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     "allow_skip: marks tests that are allowed to be skipped",
 ]
 testpaths = [
     "asyncflows/tests",
 ]
+
+[tool.poetry.plugins."asyncflows"]
+actions = "asyncflows.actions"
```

### Comparing `asyncflows-0.1.5/PKG-INFO` & `asyncflows-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncflows
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: BSL-1.1
 Author: Rafael Irgolic
 Author-email: hello@irgolic.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -67,20 +67,21 @@
 2.2 [Local development](#local-development)  
 3. [Examples](#examples)  
 3.1 [Text Style Transfer](#text-style-transfer)  
 3.2 [De Bono's Six Thinking Hats](#de-bonos-six-thinking-hats)  
 3.3 [Retrieval Augmented Generation (RAG)](#retrieval-augmented-generation-rag)  
 3.4 [SQL Retrieval](#sql-retrieval)  
 3.5 [Chatbot](#chatbot)  
-3.6 [Writing your own actions](#writing-your-own-actions)  
 4. [Guides](#guides)  
-4.1 [Writing Flows with Autocomplete](#writing-flows-with-autocomplete)  
-4.2 [Setting up Ollama for Local Inference](#setting-up-ollama-for-local-inference)  
-4.3 [Using Any Language Model](#using-any-language-model)  
-4.4 [Prompting in-depth](#prompting-in-depth)  
+4.1 [Custom Actions](#custom-actions)  
+4.2 [Writing Flows with Autocomplete](#writing-flows-with-autocomplete)  
+4.3 [Caching with Redis](#caching-with-redis)  
+4.4 [Setting up Ollama for Local Inference](#setting-up-ollama-for-local-inference)  
+4.5 [Using Any Language Model](#using-any-language-model)  
+4.6 [Prompting in-depth](#prompting-in-depth)  
 5. [License](#license)
 
 
 # Introduction
 
 asyncflows is a framework for designing and running AI pipelines using simple YAML configuration.
 
@@ -258,15 +259,16 @@
 The examples default to Llama 3, and assume [Ollama](https://ollama.com/) is running locally.
 
 See [Setting up Ollama for Local Inference](#setting-up-ollama-for-local-inference) to setup Ollama.  
 See [Using Any Language Model](#using-any-language-model) to use a different model or provider.
 
 ## Text Style Transfer
 
-[![template](https://img.shields.io/badge/template-blue)](https://github.com/asynchronous-flows/text-style-transfer-example)
+[![template repo](https://img.shields.io/badge/template_repo-blue)](https://github.com/asynchronous-flows/text-style-transfer-example)
+[![Try in Colab](https://img.shields.io/badge/colab-red)](https://colab.research.google.com/github/asynchronous-flows/text-style-transfer-example/blob/main/text_style_transfer.ipynb)
 
 This example takes a writing sample, and writes about a topic in the style of the sample.
 
 <div align="center">
 <img width="706" alt="style transfer" src="https://github.com/asynchronous-flows/asyncflows/assets/24586651/f0e2a9ef-d714-48c4-9e03-96dfc5bde5f1">
 </div>
 
@@ -646,14 +648,16 @@
 
 ---
 
 </details>
 
 ## SQL Retrieval
 
+[![template repo](https://img.shields.io/badge/template_repo-blue)](https://github.com/asynchronous-flows/sql-rag-example)
+
 This flow facilitates asking questions over a SQL database.
 
 To use it with your database, install the corresponding [extra packages](#sql-databases) and set the `DATABASE_URL` environment variable.
 
 <div align="center">
 <img width="1368" alt="sql rag" src="https://github.com/asynchronous-flows/asyncflows/assets/24586651/96241659-d470-4dac-a459-b63222db4670">
 </div>
@@ -781,15 +785,15 @@
 
 ---
 
 </details>
 
 ## Chatbot
 
-[![template](https://img.shields.io/badge/template-blue)](https://github.com/asynchronous-flows/pdf-chatbot-example)
+[![template repo](https://img.shields.io/badge/template_repo-blue)](https://github.com/asynchronous-flows/pdf-chatbot-example)
 
 This flow facilitates a chatbot over a set of PDF documents.
 
 Given a list of filepaths, it extracts their text, uses retrieval augmented generation (RAG) to find the ones relevant to the question, and generates an answer.
 
 The form of RAG we're using is **retrieval** followed by **reranking**.
 Retrieval is great for searching through a large dataset, while reranking is slower but better at matching against the query.
@@ -963,19 +967,24 @@
 
 The Red Queen's perspective on punishment reveals a stark contrast between her cruel nature and the more benevolent attitudes of other characters, such as the King, who intervenes to save Alice from execution. The Queen's actions also create a sense of danger and chaos, making Wonderland an unpredictable and potentially deadly place for its inhabitants.
 
 ---
 
 </details>
 
-## Writing your own actions
+# Guides
+
+## Custom Actions
+
+[![template repo](https://img.shields.io/badge/template_repo-blue)](https://github.com/asynchronous-flows/api-call-example)
 
-You can create custom actions by subclassing `Action` and defining the input and output models using Pydantic.
+You can create custom actions by subclassing `Action`, and defining the input and output models using Pydantic.
+
+Here is an example action that visits a webpage and returns its text content:
 
-Python code for the custom action:
 ```python
 from asyncflows import Action, BaseModel, Field
 
 import aiohttp
 
 
 class Inputs(BaseModel):
@@ -995,15 +1004,19 @@
 
     async def run(self, inputs: Inputs) -> Outputs:
         async with aiohttp.ClientSession() as session:
             async with session.get(inputs.url) as response:
                 return Outputs(result=await response.text())
 ```
 
-YAML file of an example flow using this action:
+<details>
+<summary>
+YAML file of an example flow using this action – click to expand
+</summary>
+
 ```yaml
 # get_page_title.yaml
 
 default_model:
   model: ollama/llama3
 flow:
   get_website:
@@ -1016,24 +1029,26 @@
       - heading: Website content
         link: get_website.result
       - text: |
           What is the title of the webpage?
 default_output: extract_title.result
 ```
 
+</details>
+
 <details>
 <summary>
 Running the flow (python and stdout)
 </summary>
 
 Python script that runs the flow:
 ```python
 from asyncflows import AsyncFlows
 
-flow = AsyncFlows.from_file("soup.yaml")
+flow = AsyncFlows.from_file("get_page_title.yaml")
 
 # Run the flow and return the default output (result of the extract_title action)
 result = await flow.set_vars(
     url="https://en.wikipedia.org/wiki/Python_(programming_language)",
 ).run()
 print(result)
 ```
@@ -1041,29 +1056,69 @@
 Output of the python script:
 ```
 The title of the webpage is "Python (programming language) - Wikipedia".
 ```
 
 </details>
 
-# Guides
+As long as your custom actions are imported before instantiating the flow,
+they will be available for use.
+
+Alternatively, to ensure the action is always available, 
+and for it to show up when using the language server for YAML autocomplete,
+register an entrypoint for the module that contains your actions.  
+For example, using poetry, with your actions located in `my_package.actions`,
+include the following at the end of your `pyproject.toml`:
+
+```toml
+[tool.poetry.plugins."asyncflows"]
+actions = "my_package.actions"
+```
+
+See the [API Call Example](https://github.com/asynchronous-flows/api-call-example) for a custom actions template repository.
 
 ## Writing Flows with Autocomplete
 
 For an easier time writing flows, use YAML Language Server in your editor with our JsonSchema.
 
 Put the following at the top of your YAML flow config file:
 
 ```yaml
 # yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/asyncflows_schema.json
 ```
 
 The JsonSchema will only catch some errors, 
 stay tuned for a domain-specific language server that will provide more advanced features.
 
+## Caching with Redis
+
+By default, AsyncFlows caches action outputs with a shelve file in a temporary directory.
+
+To cache between runs, we support Redis as a backend:
+
+1. Run [Redis](https://redis.io/download) locally or use a cloud provider.
+
+2. Set the following environment variables:
+
+- `REDIS_HOST` (required)
+- `REDIS_PASSWORD` (required)
+- `REDIS_PORT` (optional, defaults to 6379)
+- `REDIS_USERNAME` (optional, defaults to empty string)
+
+3. Override the default cache with:
+
+```python
+from asyncflows import AsyncFlows, RedisCacheRepo
+
+flow = AsyncFlows.from_file(
+   "flow.yaml",
+   cache_repo=RedisCacheRepo,
+)
+```
+
 ## Setting up Ollama for Local Inference
 
 To run the examples, you need to have [Ollama](https://ollama.com/) running locally.
 
 1. [Download and Install Ollama](https://ollama.com/download) 
 2. On some platforms like macOS Ollama runs in the background automatically. 
    If not, start it with:
```

