# Comparing `tmp/airbyte_source_pinterest-1.3.3.tar.gz` & `tmp/airbyte_source_pinterest-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_pinterest-1.3.3.tar", max compression
+gzip compressed data, was "airbyte_source_pinterest-2.0.0.tar", max compression
```

## Comparing `airbyte_source_pinterest-1.3.3.tar` & `airbyte_source_pinterest-2.0.0.tar`

### file list

```diff
@@ -1,35 +1,16 @@
--rw-r--r--   0        0        0     4550 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/README.md
--rw-r--r--   0        0        0      805 2024-05-07 12:29:18.382990 airbyte_source_pinterest-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      130 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/__init__.py
--rw-r--r--   0        0        0      146 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/reports/__init__.py
--rw-r--r--   0        0        0      540 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/reports/errors.py
--rw-r--r--   0        0        0      787 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/reports/models.py
--rw-r--r--   0        0        0    12000 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/reports/reports.py
--rw-r--r--   0        0        0      239 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/run.py
--rw-r--r--   0        0        0    15617 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/ad_account_analytics.json
--rw-r--r--   0        0        0     1518 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/ad_accounts.json
--rw-r--r--   0        0        0    14207 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/ad_analytics.json
--rw-r--r--   0        0        0    14937 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/ad_group_analytics.json
--rw-r--r--   0        0        0     8456 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/ad_groups.json
--rw-r--r--   0        0        0     5928 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/ads.json
--rw-r--r--   0        0        0     3592 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/audiences.json
--rw-r--r--   0        0        0     3451 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/board_pins.json
--rw-r--r--   0        0        0     5644 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/board_section_pins.json
--rw-r--r--   0        0        0      332 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/board_sections.json
--rw-r--r--   0        0        0     2111 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/boards.json
--rw-r--r--   0        0        0    16631 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/campaign_analytics.json
--rw-r--r--   0        0        0    15018 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/campaign_analytics_report.json
--rw-r--r--   0        0        0     3547 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/campaigns.json
--rw-r--r--   0        0        0      876 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/catalogs.json
--rw-r--r--   0        0        0     2375 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/catalogs_feeds.json
--rw-r--r--   0        0        0     1300 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/catalogs_product_groups.json
--rw-r--r--   0        0        0     2727 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/conversion_tags.json
--rw-r--r--   0        0        0     1586 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/customer_lists.json
--rw-r--r--   0        0        0     1207 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/keywords.json
--rw-r--r--   0        0        0    15628 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/reports.json
--rw-r--r--   0        0        0     1957 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/schemas/user_account_analytics.json
--rw-r--r--   0        0        0     7829 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/source.py
--rw-r--r--   0        0        0    12837 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/spec.json
--rw-r--r--   0        0        0    17192 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/streams.py
--rw-r--r--   0        0        0     4214 2024-05-07 10:51:28.000000 airbyte_source_pinterest-1.3.3/source_pinterest/utils.py
--rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 airbyte_source_pinterest-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     4565 2024-05-28 11:19:34.796036 airbyte_source_pinterest-2.0.0/README.md
+-rw-r--r--   0        0        0      805 2024-05-28 11:23:36.583239 airbyte_source_pinterest-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/__init__.py
+-rw-r--r--   0        0        0     3206 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/components/auth.py
+-rw-r--r--   0        0        0   126647 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/manifest.yaml
+-rw-r--r--   0        0        0      146 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/reports/__init__.py
+-rw-r--r--   0        0        0      540 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/reports/errors.py
+-rw-r--r--   0        0        0      787 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/reports/models.py
+-rw-r--r--   0        0        0    12000 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/reports/reports.py
+-rw-r--r--   0        0        0      239 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/run.py
+-rw-r--r--   0        0        0    15018 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/schemas/campaign_analytics_report.json
+-rw-r--r--   0        0        0    15628 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/schemas/reports.json
+-rw-r--r--   0        0        0     5763 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/source.py
+-rw-r--r--   0        0        0     9638 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/streams.py
+-rw-r--r--   0        0        0     4214 2024-05-28 11:19:34.800036 airbyte_source_pinterest-2.0.0/source_pinterest/utils.py
+-rw-r--r--   0        0        0     5312 1970-01-01 00:00:00.000000 airbyte_source_pinterest-2.0.0/PKG-INFO
```

### Comparing `airbyte_source_pinterest-1.3.3/README.md` & `airbyte_source_pinterest-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Pinterest source connector
 
-
 This is the repository for the Pinterest source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pinterest).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pinterest)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pinterest/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-pinterest spec
 poetry run source-pinterest check --config secrets/config.json
 poetry run source-pinterest discover --config secrets/config.json
-poetry run source-pinterest read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-pinterest read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-pinterest build
 ```
 
 An image will be available on your host with the tag `airbyte/source-pinterest:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-pinterest:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pinterest:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pinterest:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pinterest:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-pinterest test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pinterest test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pinterest.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_pinterest-1.3.3/pyproject.toml` & `airbyte_source_pinterest-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.3.3"
+version = "2.0.0"
 name = "airbyte-source-pinterest"
 description = "Source implementation for Pinterest."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -19,15 +19,15 @@
 packages = [
     { include = "source_pinterest" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 pendulum = "==2.1.2"
-airbyte-cdk = "0.80.0"
+airbyte-cdk = "0.86.3"
 
 [tool.poetry.scripts]
 source-pinterest = "source_pinterest.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.11.0"
 pytest-mock = "^3.6.1"
```

### Comparing `airbyte_source_pinterest-1.3.3/source_pinterest/reports/errors.py` & `airbyte_source_pinterest-2.0.0/source_pinterest/reports/errors.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.3/source_pinterest/reports/models.py` & `airbyte_source_pinterest-2.0.0/source_pinterest/reports/models.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.3/source_pinterest/reports/reports.py` & `airbyte_source_pinterest-2.0.0/source_pinterest/reports/reports.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.3/source_pinterest/schemas/ad_account_analytics.json` & `airbyte_source_pinterest-2.0.0/source_pinterest/schemas/reports.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9851892822025565%*

 * *Differences: {"'properties'": "{'DATE': {'description': 'Date of the data record'}, 'ADVERTISER_ID': {'type': "*

 * *                 "['null', 'number']}, 'CAMPAIGN_DAILY_SPEND_CAP': {'description': 'Daily spend "*

 * *                 "cap for the campaign'}, 'CAMPAIGN_ENTITY_STATUS': {'type': {insert: [(1, "*

 * *                 "'string')], delete: [1]}}, 'CAMPAIGN_LIFETIME_SPEND_CAP': {'description': "*

 * *                 "'Lifetime spend cap for the campaign'}, 'CLICKTHROUGH_1': {'description': "*

 * *                 "'Number of click […]*

```diff
@@ -1,14 +1,15 @@
 {
     "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
         "ADVERTISER_ID": {
             "description": "Unique identifier for the advertiser",
             "type": [
-                "string"
+                "null",
+                "number"
             ]
         },
         "AD_ACCOUNT_ID": {
             "description": "Unique identifier for the ad account",
             "type": [
                 "string"
             ]
@@ -31,36 +32,36 @@
             "description": "Unique identifier for the ad",
             "type": [
                 "null",
                 "string"
             ]
         },
         "CAMPAIGN_DAILY_SPEND_CAP": {
-            "description": "Daily spend cap set for the campaign",
+            "description": "Daily spend cap for the campaign",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CAMPAIGN_ENTITY_STATUS": {
             "description": "Status of the campaign entity",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "CAMPAIGN_ID": {
             "description": "Unique identifier for the campaign",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CAMPAIGN_LIFETIME_SPEND_CAP": {
-            "description": "Lifetime spend cap set for the campaign",
+            "description": "Lifetime spend cap for the campaign",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CAMPAIGN_NAME": {
             "description": "Name of the campaign",
@@ -73,43 +74,43 @@
             "description": "Return on ad spend for checkout actions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CLICKTHROUGH_1": {
-            "description": "Click-through rate related to specific actions",
+            "description": "Number of click-through events",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CLICKTHROUGH_1_GROSS": {
-            "description": "Gross click-through rate related to specific actions",
+            "description": "Gross number of click-through events",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CLICKTHROUGH_2": {
-            "description": "Secondary click-through rate related to specific actions",
+            "description": "Second type of click-through events",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CPC_IN_MICRO_DOLLAR": {
             "description": "Cost per click in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CPM_IN_DOLLAR": {
-            "description": "Cost per mille in dollars",
+            "description": "Cost per mille (cost per thousand impressions) in dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CPM_IN_MICRO_DOLLAR": {
             "description": "Cost per mille in micro dollars",
@@ -122,37 +123,37 @@
             "description": "Click-through rate",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CTR_2": {
-            "description": "Secondary click-through rate",
+            "description": "Second click-through rate",
             "type": [
                 "null",
                 "number"
             ]
         },
         "DATE": {
-            "description": "Date of the data entry",
+            "description": "Date of the data record",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
         "ECPCV_IN_DOLLAR": {
-            "description": "Effective cost per completed view in dollars",
+            "description": "Effective cost per conversion value in dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ECPCV_P95_IN_DOLLAR": {
-            "description": "95th percentile effective cost per completed view in dollars",
+            "description": "P95 percentile of effective cost per conversion value in dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ECPC_IN_DOLLAR": {
             "description": "Effective cost per click in dollars",
@@ -200,85 +201,85 @@
             "description": "Effective engagement rate",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ENGAGEMENT_1": {
-            "description": "Engagement rate related to specific actions",
+            "description": "Number of engagement events",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ENGAGEMENT_2": {
-            "description": "Secondary engagement rate related to specific actions",
+            "description": "Second type of engagement events",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ENGAGEMENT_RATE": {
-            "description": "Overall engagement rate",
+            "description": "Engagement rate",
             "type": [
                 "null",
                 "number"
             ]
         },
         "IDEA_PIN_PRODUCT_TAG_VISIT_1": {
-            "description": "Product tag visit rate related to specific actions",
+            "description": "Number of visits to pinned product tags",
             "type": [
                 "null",
                 "number"
             ]
         },
         "IDEA_PIN_PRODUCT_TAG_VISIT_2": {
-            "description": "Secondary product tag visit rate related to specific actions",
+            "description": "Second type of visits to pinned product tags",
             "type": [
                 "null",
                 "number"
             ]
         },
         "IMPRESSION_1": {
-            "description": "Impression rate related to specific actions",
+            "description": "Number of impressions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "IMPRESSION_1_GROSS": {
-            "description": "Gross impression rate related to specific actions",
+            "description": "Gross number of impressions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "IMPRESSION_2": {
-            "description": "Secondary impression rate related to specific actions",
+            "description": "Second type of impressions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "INAPP_CHECKOUT_COST_PER_ACTION": {
             "description": "Cost per in-app checkout action",
             "type": [
                 "null",
                 "number"
             ]
         },
         "OUTBOUND_CLICK_1": {
-            "description": "Outbound click rate related to specific actions",
+            "description": "Number of outbound clicks",
             "type": [
                 "null",
                 "number"
             ]
         },
         "OUTBOUND_CLICK_2": {
-            "description": "Secondary outbound click rate related to specific actions",
+            "description": "Second type of outbound clicks",
             "type": [
                 "null",
                 "number"
             ]
         },
         "PAGE_VISIT_COST_PER_ACTION": {
             "description": "Cost per page visit action",
@@ -298,43 +299,43 @@
             "description": "Number of paid impressions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "PIN_ID": {
-            "description": "Unique identifier for the pin",
+            "description": "Unique identifier for the pinned image",
             "type": [
                 "null",
                 "number"
             ]
         },
         "PIN_PROMOTION_ID": {
-            "description": "Unique identifier for the promoted pin",
+            "description": "Unique identifier for the pinned promotion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "REPIN_1": {
-            "description": "Repinned rate related to specific actions",
+            "description": "Number of repins",
             "type": [
                 "null",
                 "number"
             ]
         },
         "REPIN_2": {
-            "description": "Secondary repinned rate related to specific actions",
+            "description": "Second type of repins",
             "type": [
                 "null",
                 "number"
             ]
         },
         "REPIN_RATE": {
-            "description": "Overall repin rate",
+            "description": "Repins rate",
             "type": [
                 "null",
                 "number"
             ]
         },
         "SPEND_IN_DOLLAR": {
             "description": "Total spend in dollars",
@@ -361,71 +362,71 @@
             "description": "Total value of checkout actions in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICKTHROUGH": {
-            "description": "Total number of click-through actions",
+            "description": "Total number of click-through events",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICK_ADD_TO_CART": {
-            "description": "Total number of click actions leading to adding to cart",
+            "description": "Total number of click events leading to adding items to cart",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICK_CHECKOUT": {
-            "description": "Total number of click actions leading to checkout",
+            "description": "Total number of click events leading to checkout",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICK_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total value of click actions leading to checkout in micro dollars",
+            "description": "Total value of click events leading to checkout in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICK_LEAD": {
-            "description": "Total number of click actions leading to lead generation",
+            "description": "Total number of click events leading to generating leads",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICK_SIGNUP": {
-            "description": "Total number of click actions leading to signups",
+            "description": "Total number of click events leading to sign-ups",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICK_SIGNUP_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total value of click actions leading to signups in micro dollars",
+            "description": "Total value of click events leading to sign-ups in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CONVERSIONS": {
             "description": "Total number of conversions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CUSTOM": {
-            "description": "Total number of custom actions",
+            "description": "Total number of custom events",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_ENGAGEMENT": {
             "description": "Total number of engagement actions",
@@ -445,351 +446,351 @@
             "description": "Total value of engagement actions leading to checkout in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_ENGAGEMENT_LEAD": {
-            "description": "Total number of engagement actions leading to lead generation",
+            "description": "Total number of engagement actions leading to generating leads",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_ENGAGEMENT_SIGNUP": {
-            "description": "Total number of engagement actions leading to signups",
+            "description": "Total number of engagement actions leading to sign-ups",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_ENGAGEMENT_SIGNUP_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total value of engagement actions leading to signups in micro dollars",
+            "description": "Total value of engagement actions leading to sign-ups in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_IDEA_PIN_PRODUCT_TAG_VISIT": {
-            "description": "Total number of product tag visits",
+            "description": "Total number of visits to pinned product tags",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_IMPRESSION_FREQUENCY": {
             "description": "Total impression frequency",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_IMPRESSION_USER": {
-            "description": "Total number of users reached through impressions",
+            "description": "Total number of users reached by impressions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_LEAD": {
-            "description": "Total number of lead actions",
+            "description": "Total number of leads generated",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_OFFLINE_CHECKOUT": {
             "description": "Total number of offline checkout actions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_PAGE_VISIT": {
-            "description": "Total number of page visit actions",
+            "description": "Total number of page visits",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_REPIN_RATE": {
-            "description": "Overall repin rate",
+            "description": "Total repins rate",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_SIGNUP": {
-            "description": "Total number of signup actions",
+            "description": "Total number of sign-ups",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_SIGNUP_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total value of signup actions in micro dollars",
+            "description": "Total value of sign-ups in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_3SEC_VIEWS": {
-            "description": "Total number of 3-second video views",
+            "description": "Total number of views for 3 seconds or more on video ads",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_AVG_WATCHTIME_IN_SECOND": {
-            "description": "Average watch time for videos in seconds",
+            "description": "Total average watch time for video ads in seconds",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_MRC_VIEWS": {
-            "description": "Total number of MRC video views",
+            "description": "Total number of viewable impressions for video ads",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_P0_COMBINED": {
-            "description": "Total video play-through rate",
+            "description": "Total percentage of video ads viewed to the start",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_P100_COMPLETE": {
-            "description": "Total completion rate for videos",
+            "description": "Total percentage of video ads viewed to completion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_P25_COMBINED": {
-            "description": "Total 25% completion rate for videos",
+            "description": "Total percentage of video ads viewed to 25% completion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_P50_COMBINED": {
-            "description": "Total 50% completion rate for videos",
+            "description": "Total percentage of video ads viewed to 50% completion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_P75_COMBINED": {
-            "description": "Total 75% completion rate for videos",
+            "description": "Total percentage of video ads viewed to 75% completion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_P95_COMBINED": {
-            "description": "Total 95% completion rate for videos",
+            "description": "Total percentage of video ads viewed to 95% completion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIEW_ADD_TO_CART": {
-            "description": "Total view actions leading to adding to cart",
+            "description": "Total number of view events leading to adding items to cart",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIEW_CHECKOUT": {
-            "description": "Total view actions leading to checkout",
+            "description": "Total number of view events leading to checkout",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIEW_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total value of view actions leading to checkout in micro dollars",
+            "description": "Total value of view events leading to checkout in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIEW_LEAD": {
-            "description": "Total view actions leading to lead generation",
+            "description": "Total number of view events leading to generating leads",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIEW_SIGNUP": {
-            "description": "Total view actions leading to signups",
+            "description": "Total number of view events leading to sign-ups",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIEW_SIGNUP_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total value of view actions leading to signups in micro dollars",
+            "description": "Total value of view events leading to sign-ups in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_CHECKOUT": {
-            "description": "Total number of web checkout actions",
+            "description": "Total number of checkout actions on the web",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total value of web checkout actions in micro dollars",
+            "description": "Total value of checkout actions on the web in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_CLICK_CHECKOUT": {
-            "description": "Total number of web click actions leading to checkout",
+            "description": "Total number of click events leading to checkout on the web",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_CLICK_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total value of web click actions leading to checkout in micro dollars",
+            "description": "Total value of click events leading to checkout on the web in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_ENGAGEMENT_CHECKOUT": {
-            "description": "Total number of web engagement actions leading to checkout",
+            "description": "Total number of engagement actions leading to checkout on the web",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_ENGAGEMENT_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total value of web engagement actions leading to checkout in micro dollars",
+            "description": "Total value of engagement actions leading to checkout on the web in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_SESSIONS": {
-            "description": "Total number of web sessions",
+            "description": "Total number of sessions on the web",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_VIEW_CHECKOUT": {
-            "description": "Total number of web view actions leading to checkout",
+            "description": "Total number of view events leading to checkout on the web",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_VIEW_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total value of web view actions leading to checkout in micro dollars",
+            "description": "Total value of view events leading to checkout on the web in micro dollars",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_3SEC_VIEWS_2": {
-            "description": "Number of 3-second video views related to specific actions",
+            "description": "Number of 3-second views for a second type of video ad",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_LENGTH": {
-            "description": "Length of the video",
+            "description": "Length of the video ad",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_MRC_VIEWS_2": {
-            "description": "Number of MRC video views related to specific actions",
+            "description": "Number of viewable impressions for a second type of video ad",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_P0_COMBINED_2": {
-            "description": "Play-through rate of videos related to specific actions",
+            "description": "Percentage of the second type of video ads viewed to the start",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_P100_COMPLETE_2": {
-            "description": "Completion rate of videos related to specific actions",
+            "description": "Percentage of the second type of video ads viewed to completion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_P25_COMBINED_2": {
-            "description": "25% completion rate of videos related to specific actions",
+            "description": "Percentage of the second type of video ads viewed to 25% completion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_P50_COMBINED_2": {
-            "description": "50% completion rate of videos related to specific actions",
+            "description": "Percentage of the second type of video ads viewed to 50% completion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_P75_COMBINED_2": {
-            "description": "75% completion rate of videos related to specific actions",
+            "description": "Percentage of the second type of video ads viewed to 75% completion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_P95_COMBINED_2": {
-            "description": "95% completion rate of videos related to specific actions",
+            "description": "Percentage of the second type of video ads viewed to 95% completion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "WEB_CHECKOUT_COST_PER_ACTION": {
-            "description": "Cost per web checkout action",
+            "description": "Cost per checkout action on the web",
             "type": [
                 "null",
                 "number"
             ]
         },
         "WEB_CHECKOUT_ROAS": {
             "description": "Return on ad spend for web checkout actions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "WEB_SESSIONS_1": {
-            "description": "Number of web sessions related to specific actions",
+            "description": "Number of sessions on the web",
             "type": [
                 "null",
                 "number"
             ]
         },
         "WEB_SESSIONS_2": {
-            "description": "Secondary number of web sessions related to specific actions",
+            "description": "Second type of web sessions",
             "type": [
                 "null",
                 "number"
             ]
         }
     },
     "type": "object"
```

### Comparing `airbyte_source_pinterest-1.3.3/source_pinterest/schemas/ad_analytics.json` & `airbyte_source_pinterest-2.0.0/source_pinterest/schemas/campaign_analytics_report.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9854965585054081%*

 * *Differences: {"'properties'": "{'ADVERTISER_ID': {'type': ['null', 'number']}, 'AD_ACCOUNT_ID': {'description': "*

 * *                 "'The unique identifier of the advertising account.'}, "*

 * *                 "'CAMPAIGN_DAILY_SPEND_CAP': {'description': 'The daily spend cap set for the "*

 * *                 "campaign.'}, 'CAMPAIGN_ENTITY_STATUS': {'type': {insert: [(1, 'string')], "*

 * *                 "delete: [1]}}, 'CAMPAIGN_LIFETIME_SPEND_CAP': {'description': 'The lifetime "*

 * *                 "spend cap set for the campaign.' […]*

```diff
@@ -1,18 +1,19 @@
 {
     "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
         "ADVERTISER_ID": {
             "description": "The unique identifier of the advertiser.",
             "type": [
-                "string"
+                "null",
+                "number"
             ]
         },
         "AD_ACCOUNT_ID": {
-            "description": "The unique identifier of the ad account.",
+            "description": "The unique identifier of the advertising account.",
             "type": [
                 "string"
             ]
         },
         "AD_GROUP_ENTITY_STATUS": {
             "description": "The status of the ad group entity.",
             "type": [
@@ -31,71 +32,71 @@
             "description": "The unique identifier of the ad.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "CAMPAIGN_DAILY_SPEND_CAP": {
-            "description": "The daily spend limit set for the campaign.",
+            "description": "The daily spend cap set for the campaign.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CAMPAIGN_ENTITY_STATUS": {
             "description": "The status of the campaign entity.",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "CAMPAIGN_ID": {
             "description": "The unique identifier of the campaign.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CAMPAIGN_LIFETIME_SPEND_CAP": {
-            "description": "The total spend limit set for the campaign.",
+            "description": "The lifetime spend cap set for the campaign.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CAMPAIGN_NAME": {
             "description": "The name of the campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "CHECKOUT_ROAS": {
-            "description": "Return on ad spend for checkout conversions.",
+            "description": "Return on ad spend for checkout actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CLICKTHROUGH_1": {
-            "description": "Click-through conversions type 1.",
+            "description": "Click-throughs for a specific action 1.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CLICKTHROUGH_1_GROSS": {
-            "description": "Gross click-through conversions type 1.",
+            "description": "Gross click-throughs for a specific action 1.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CLICKTHROUGH_2": {
-            "description": "Click-through conversions type 2.",
+            "description": "Click-throughs for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CPC_IN_MICRO_DOLLAR": {
             "description": "Cost per click in micro dollars.",
@@ -122,37 +123,37 @@
             "description": "Click-through rate.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CTR_2": {
-            "description": "Click-through rate 2.",
+            "description": "Click-through rate for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "DATE": {
             "description": "The date for the data entry.",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
         "ECPCV_IN_DOLLAR": {
-            "description": "Effective cost per click view in dollars.",
+            "description": "Effective cost per click for view actions in dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ECPCV_P95_IN_DOLLAR": {
-            "description": "Effective cost per click view percentile 95 in dollars.",
+            "description": "Effective cost per click for view actions at the 95th percentile in dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ECPC_IN_DOLLAR": {
             "description": "Effective cost per click in dollars.",
@@ -179,120 +180,120 @@
             "description": "Effective cost per mille in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ECPV_IN_DOLLAR": {
-            "description": "Effective cost per view in dollar.",
+            "description": "Effective cost per view in dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ECTR": {
-            "description": "Effective click-through rate.",
+            "description": "Engagement click-through rate.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "EENGAGEMENT_RATE": {
             "description": "Effective engagement rate.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ENGAGEMENT_1": {
-            "description": "Engagement type 1.",
+            "description": "Engagements for a specific action 1.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ENGAGEMENT_2": {
-            "description": "Engagement type 2.",
+            "description": "Engagements for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ENGAGEMENT_RATE": {
             "description": "Engagement rate.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "IDEA_PIN_PRODUCT_TAG_VISIT_1": {
-            "description": "Idea pin product tag visit type 1.",
+            "description": "Product tag visits for a specific action 1.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "IDEA_PIN_PRODUCT_TAG_VISIT_2": {
-            "description": "Idea pin product tag visit type 2.",
+            "description": "Product tag visits for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "IMPRESSION_1": {
-            "description": "Impressions type 1.",
+            "description": "Impressions for a specific action 1.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "IMPRESSION_1_GROSS": {
-            "description": "Gross impressions type 1.",
+            "description": "Gross impressions for a specific action 1.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "IMPRESSION_2": {
-            "description": "Impressions type 2.",
+            "description": "Impressions for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "INAPP_CHECKOUT_COST_PER_ACTION": {
             "description": "In-app checkout cost per action.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "OUTBOUND_CLICK_1": {
-            "description": "Outbound clicks type 1.",
+            "description": "Outbound clicks for a specific action 1.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "OUTBOUND_CLICK_2": {
-            "description": "Outbound clicks type 2.",
+            "description": "Outbound clicks for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "PAGE_VISIT_COST_PER_ACTION": {
             "description": "Page visit cost per action.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "PAGE_VISIT_ROAS": {
-            "description": "Return on ad spend for page visits.",
+            "description": "Return on ad spend for page visit actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "PAID_IMPRESSION": {
             "description": "Paid impressions.",
@@ -305,29 +306,29 @@
             "description": "The unique identifier of the pin.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "PIN_PROMOTION_ID": {
-            "description": "The unique identifier of the pin promotion.",
+            "description": "The promotion ID of the pin.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "REPIN_1": {
-            "description": "Repins type 1.",
+            "description": "Repins for a specific action 1.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "REPIN_2": {
-            "description": "Repins type 2.",
+            "description": "Repins for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "REPIN_RATE": {
             "description": "Repins rate.",
@@ -347,162 +348,162 @@
             "description": "Total spend in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CHECKOUT": {
-            "description": "Total checkout conversions.",
+            "description": "Total checkout activities.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
             "description": "Total checkout value in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICKTHROUGH": {
-            "description": "Total click-through conversions.",
+            "description": "Total click-throughs.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICK_ADD_TO_CART": {
-            "description": "Total clicks add to cart.",
+            "description": "Total clicks to add to cart.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICK_CHECKOUT": {
-            "description": "Total clicks checkout.",
+            "description": "Total clicks to checkout.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICK_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total clicks checkout value in micro dollars.",
+            "description": "Total click checkout value in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICK_LEAD": {
-            "description": "Total clicks lead.",
+            "description": "Total clicks for generating leads.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICK_SIGNUP": {
-            "description": "Total clicks sign up.",
+            "description": "Total clicks for sign-ups.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CLICK_SIGNUP_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total clicks sign up value in micro dollars.",
+            "description": "Total click sign-up value in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CONVERSIONS": {
-            "description": "Total conversions.",
+            "description": "Total conversion actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_CUSTOM": {
             "description": "Total custom actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_ENGAGEMENT": {
-            "description": "Total engagements.",
+            "description": "Total engagement actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_ENGAGEMENT_CHECKOUT": {
-            "description": "Total engagements checkout.",
+            "description": "Total engagement actions leading to checkout.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_ENGAGEMENT_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total engagements checkout value in micro dollars.",
+            "description": "Total engagement checkout value in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_ENGAGEMENT_LEAD": {
-            "description": "Total engagements lead.",
+            "description": "Total engagement actions leading to a lead.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_ENGAGEMENT_SIGNUP": {
-            "description": "Total engagements sign up.",
+            "description": "Total engagement actions leading to sign-ups.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_ENGAGEMENT_SIGNUP_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total engagements sign up value in micro dollars.",
+            "description": "Total engagement sign-up value in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_IDEA_PIN_PRODUCT_TAG_VISIT": {
-            "description": "Total idea pin product tag visits.",
+            "description": "Total product tag visits.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_IMPRESSION_FREQUENCY": {
-            "description": "Total impressions frequency.",
+            "description": "Total impression frequency.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_IMPRESSION_USER": {
-            "description": "Total impressions per user.",
+            "description": "Total impression users.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_LEAD": {
-            "description": "Total leads.",
+            "description": "Total generated leads.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_OFFLINE_CHECKOUT": {
-            "description": "Total offline checkout conversions.",
+            "description": "Total offline checkout actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_PAGE_VISIT": {
             "description": "Total page visits.",
@@ -515,281 +516,281 @@
             "description": "Total repin rate.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_SIGNUP": {
-            "description": "Total signups.",
+            "description": "Total sign-ups.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_SIGNUP_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total sign up value in micro dollars.",
+            "description": "Total sign-up value in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_3SEC_VIEWS": {
-            "description": "Total video 3-second views.",
+            "description": "Total video views for at least 3 seconds.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_AVG_WATCHTIME_IN_SECOND": {
-            "description": "Total average watch time for videos in seconds.",
+            "description": "Average watch time for video in seconds.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_MRC_VIEWS": {
             "description": "Total video MRC views.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_P0_COMBINED": {
-            "description": "Total video P0 combined.",
+            "description": "Video views at point 0 combined.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_P100_COMPLETE": {
-            "description": "Total video P100 complete views.",
+            "description": "Video views at 100% completion.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_P25_COMBINED": {
-            "description": "Total video P25 combined.",
+            "description": "Video views at 25% completion combined.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_P50_COMBINED": {
-            "description": "Total video P50 combined.",
+            "description": "Video views at 50% completion combined.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_P75_COMBINED": {
-            "description": "Total video P75 combined.",
+            "description": "Video views at 75% completion combined.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIDEO_P95_COMBINED": {
-            "description": "Total video P95 combined.",
+            "description": "Video views at 95% completion combined.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIEW_ADD_TO_CART": {
-            "description": "Total view add to cart conversions.",
+            "description": "Total views leading to add to cart actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIEW_CHECKOUT": {
-            "description": "Total view checkouts.",
+            "description": "Total views leading to checkout actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIEW_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
             "description": "Total view checkout value in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIEW_LEAD": {
-            "description": "Total view leads.",
+            "description": "Total views leading to lead actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIEW_SIGNUP": {
-            "description": "Total view signups.",
+            "description": "Total views leading to sign-up actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_VIEW_SIGNUP_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total view signup value in micro dollars.",
+            "description": "Total view sign-up value in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_CHECKOUT": {
-            "description": "Total web checkouts.",
+            "description": "Total web checkout actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
             "description": "Total web checkout value in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_CLICK_CHECKOUT": {
-            "description": "Total web click checkouts.",
+            "description": "Total web click to checkout actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_CLICK_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
             "description": "Total web click checkout value in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_ENGAGEMENT_CHECKOUT": {
-            "description": "Total web engagements checkout.",
+            "description": "Total web engagement leading to checkout actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_ENGAGEMENT_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
-            "description": "Total web engagements checkout value in micro dollars.",
+            "description": "Total web engagement checkout value in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_SESSIONS": {
             "description": "Total web sessions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_VIEW_CHECKOUT": {
-            "description": "Total web view checkouts.",
+            "description": "Total web views leading to checkout actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TOTAL_WEB_VIEW_CHECKOUT_VALUE_IN_MICRO_DOLLAR": {
             "description": "Total web view checkout value in micro dollars.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_3SEC_VIEWS_2": {
-            "description": "Video 3-second views type 2.",
+            "description": "Video views for at least 3 seconds for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_LENGTH": {
-            "description": "Length of the video.",
+            "description": "The length of the video.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_MRC_VIEWS_2": {
-            "description": "Video MRC views type 2.",
+            "description": "Video MRC views for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_P0_COMBINED_2": {
-            "description": "Video P0 combined type 2.",
+            "description": "Video views at point 0 combined for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_P100_COMPLETE_2": {
-            "description": "Video P100 complete views type 2.",
+            "description": "Video views at 100% completion for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_P25_COMBINED_2": {
-            "description": "Video P25 combined type 2.",
+            "description": "Video views at 25% completion combined for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_P50_COMBINED_2": {
-            "description": "Video P50 combined type 2.",
+            "description": "Video views at 50% completion combined for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_P75_COMBINED_2": {
-            "description": "Video P75 combined type 2.",
+            "description": "Video views at 75% completion combined for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "VIDEO_P95_COMBINED_2": {
-            "description": "Video P95 combined type 2.",
+            "description": "Video views at 95% completion combined for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "WEB_CHECKOUT_COST_PER_ACTION": {
             "description": "Web checkout cost per action.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "WEB_CHECKOUT_ROAS": {
-            "description": "Return on ad spend for web checkouts.",
+            "description": "Return on ad spend for web checkout actions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "WEB_SESSIONS_1": {
-            "description": "Web sessions type 1.",
+            "description": "Web sessions for a specific action 1.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "WEB_SESSIONS_2": {
-            "description": "Web sessions type 2.",
+            "description": "Web sessions for a specific action 2.",
             "type": [
                 "null",
                 "number"
             ]
         }
     },
     "type": "object"
```

### Comparing `airbyte_source_pinterest-1.3.3/source_pinterest/source.py` & `airbyte_source_pinterest-2.0.0/source_pinterest/source.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import copy
 import logging
 from base64 import standard_b64encode
-from typing import Any, List, Mapping, Tuple, Type
+from typing import Any, List, Mapping
 
 import pendulum
-import requests
 from airbyte_cdk.models import FailureType
-from airbyte_cdk.sources import AbstractSource
+from airbyte_cdk.sources.declarative.yaml_declarative_source import YamlDeclarativeSource
 from airbyte_cdk.sources.streams import Stream
 from airbyte_cdk.sources.streams.http.auth import Oauth2Authenticator
 from airbyte_cdk.utils import AirbyteTracedException
 from source_pinterest.reports import CampaignAnalyticsReport
 
 from .reports.reports import (
     AdGroupReport,
@@ -26,43 +25,25 @@
     KeywordReport,
     PinPromotionReport,
     PinPromotionTargetingReport,
     ProductGroupReport,
     ProductGroupTargetingReport,
     ProductItemReport,
 )
-from .streams import (
-    AdAccountAnalytics,
-    AdAccounts,
-    AdAnalytics,
-    AdGroupAnalytics,
-    AdGroups,
-    Ads,
-    Audiences,
-    BoardPins,
-    Boards,
-    BoardSectionPins,
-    BoardSections,
-    CampaignAnalytics,
-    Campaigns,
-    Catalogs,
-    CatalogsFeeds,
-    CatalogsProductGroups,
-    ConversionTags,
-    CustomerLists,
-    Keywords,
-    PinterestStream,
-    UserAccountAnalytics,
-)
+from .streams import PinterestStream
 
 logger = logging.getLogger("airbyte")
 
 
-class SourcePinterest(AbstractSource):
-    def _validate_and_transform(self, config: Mapping[str, Any], amount_of_days_allowed_for_lookup: int = 89):
+class SourcePinterest(YamlDeclarativeSource):
+    def __init__(self) -> None:
+        super().__init__(**{"path_to_yaml": "manifest.yaml"})
+
+    @staticmethod
+    def _validate_and_transform(config: Mapping[str, Any], amount_of_days_allowed_for_lookup: int = 89) -> Mapping[str, Any]:
         config = copy.deepcopy(config)
         today = pendulum.today()
         latest_date_allowed_by_api = today.subtract(days=amount_of_days_allowed_for_lookup)
 
         start_date = config.get("start_date")
 
         # transform to datetime
@@ -75,101 +56,63 @@
                     message=message,
                     internal_message=message,
                     failure_type=FailureType.config_error,
                 )
 
         if not start_date or config["start_date"] < latest_date_allowed_by_api:
             logger.info(
-                f"Current start_date: {start_date} does not meet API report requirements. Resetting start_date to: {latest_date_allowed_by_api}"
+                f"Current start_date: {start_date} does not meet API report requirements. "
+                f"Resetting start_date to: {latest_date_allowed_by_api}"
             )
-            config["start_date"] = latest_date_allowed_by_api
+            config["start_date"] = latest_date_allowed_by_api.strftime("%Y-%m-%d")
 
         return config
 
     @staticmethod
-    def get_authenticator(config):
+    def get_authenticator(config) -> Oauth2Authenticator:
         config = config.get("credentials") or config
         credentials_base64_encoded = standard_b64encode(
             (config.get("client_id") + ":" + config.get("client_secret")).encode("ascii")
         ).decode("ascii")
         auth = f"Basic {credentials_base64_encoded}"
 
         return Oauth2Authenticator(
             token_refresh_endpoint=f"{PinterestStream.url_base}oauth/token",
             client_secret=config.get("client_secret"),
             client_id=config.get("client_id"),
             refresh_access_token_headers={"Authorization": auth},
             refresh_token=config.get("refresh_token"),
         )
 
-    def check_connection(self, logger, config) -> Tuple[bool, any]:
-        config = self._validate_and_transform(config)
-        authenticator = self.get_authenticator(config)
-        url = f"{PinterestStream.url_base}user_account"
-        try:
-            auth_headers = {"Accept": "application/json", **authenticator.get_auth_header()}
-            session = requests.get(url, headers=auth_headers)
-            session.raise_for_status()
-            return True, None
-        except requests.exceptions.HTTPError as e:
-            if "401 Client Error: Unauthorized for url" in str(e):
-                return False, f"Try to re-authenticate because current refresh token is not valid. {e}"
-            else:
-                return False, e
-        except requests.exceptions.RequestException as e:
-            return False, e
-
     def streams(self, config: Mapping[str, Any]) -> List[Stream]:
         config["authenticator"] = self.get_authenticator(config)
         report_config = self._validate_and_transform(config, amount_of_days_allowed_for_lookup=913)
-        config = self._validate_and_transform(config)
-        status = ",".join(config.get("status")) if config.get("status") else None
 
-        ad_accounts = AdAccounts(config)
-        ads = Ads(ad_accounts, config=config, status_filter=status)
-        ad_groups = AdGroups(ad_accounts, config=config, status_filter=status)
-        campaigns = Campaigns(ad_accounts, config=config, status_filter=status)
-        boards = Boards(config)
-        board_sections = BoardSections(boards, config=config)
-        return [
-            ad_accounts,
-            AdAccountAnalytics(ad_accounts, config=config),
-            ads,
-            AdAnalytics(ads, config=config),
-            ad_groups,
-            AdGroupAnalytics(ad_groups, config=config),
-            boards,
-            BoardPins(boards, config=config),
-            board_sections,
-            BoardSectionPins(board_sections, config=config),
-            campaigns,
-            CampaignAnalytics(campaigns, config=config),
+        declarative_streams = super().streams(config)
+        ad_accounts = [stream for stream in declarative_streams if stream.name == "ad_accounts"][0]
+
+        # Report streams involve async data fetch, which is currently not supported in low-code
+        report_streams = [
             CampaignAnalyticsReport(ad_accounts, config=report_config),
             CampaignTargetingReport(ad_accounts, config=report_config),
-            UserAccountAnalytics(None, config=config),
-            Keywords(ad_groups, config=config),
-            Audiences(ad_accounts, config=config),
-            ConversionTags(ad_accounts, config=config),
-            CustomerLists(ad_accounts, config=config),
-            Catalogs(config=config),
-            CatalogsFeeds(config=config),
-            CatalogsProductGroups(config=config),
             AdvertiserReport(ad_accounts, config=report_config),
             AdvertiserTargetingReport(ad_accounts, config=report_config),
             AdGroupReport(ad_accounts, config=report_config),
             AdGroupTargetingReport(ad_accounts, config=report_config),
             PinPromotionReport(ad_accounts, config=report_config),
             PinPromotionTargetingReport(ad_accounts, config=report_config),
             ProductGroupReport(ad_accounts, config=report_config),
             ProductGroupTargetingReport(ad_accounts, config=report_config),
             KeywordReport(ad_accounts, config=report_config),
             ProductItemReport(ad_accounts, config=report_config),
         ] + self.get_custom_report_streams(ad_accounts, config=report_config)
 
-    def get_custom_report_streams(self, parent, config: dict) -> List[Type[Stream]]:
+        return declarative_streams + report_streams
+
+    def get_custom_report_streams(self, parent, config: Mapping[str, Any]) -> List[Stream]:
         """return custom report streams"""
         custom_streams = []
         for report_config in config.get("custom_reports", []):
             report_config["authenticator"] = config["authenticator"]
 
             # https://developers.pinterest.com/docs/api/v5/#operation/analytics/get_report
             if report_config.get("granularity") == "HOUR":
@@ -182,13 +125,10 @@
 
             start_date = report_config.get("start_date")
             if not start_date:
                 report_config["start_date"] = config.get("start_date")
 
             report_config = self._validate_and_transform(report_config, amount_of_days_allowed_for_lookup)
 
-            stream = CustomReport(
-                parent=parent,
-                config=report_config,
-            )
+            stream = CustomReport(parent=parent, config=report_config)
             custom_streams.append(stream)
         return custom_streams
```

### Comparing `airbyte_source_pinterest-1.3.3/source_pinterest/utils.py` & `airbyte_source_pinterest-2.0.0/source_pinterest/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.3/PKG-INFO` & `airbyte_source_pinterest-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,111 +1,125 @@
 Metadata-Version: 2.1
 Name: airbyte-source-pinterest
-Version: 1.3.3
+Version: 2.0.0
 Summary: Source implementation for Pinterest.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.80.0)
+Requires-Dist: airbyte-cdk (==0.86.3)
 Requires-Dist: pendulum (==2.1.2)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/pinterest
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Pinterest source connector
 
-
 This is the repository for the Pinterest source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pinterest).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pinterest)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pinterest/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-pinterest spec
 poetry run source-pinterest check --config secrets/config.json
 poetry run source-pinterest discover --config secrets/config.json
-poetry run source-pinterest read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-pinterest read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-pinterest build
 ```
 
 An image will be available on your host with the tag `airbyte/source-pinterest:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-pinterest:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pinterest:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pinterest:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pinterest:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-pinterest test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pinterest test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pinterest.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

