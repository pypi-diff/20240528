# Comparing `tmp/airbyte_source_yahoo_finance_price-0.2.4.tar.gz` & `tmp/airbyte_source_yahoo_finance_price-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_yahoo_finance_price-0.2.4.tar", max compression
+gzip compressed data, was "airbyte_source_yahoo_finance_price-0.2.5.tar", max compression
```

## Comparing `airbyte_source_yahoo_finance_price-0.2.4.tar` & `airbyte_source_yahoo_finance_price-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4730 2024-04-20 23:28:42.000000 airbyte_source_yahoo_finance_price-0.2.4/README.md
--rw-r--r--   0        0        0      821 2024-04-21 00:10:15.542645 airbyte_source_yahoo_finance_price-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      146 2024-04-20 23:28:42.000000 airbyte_source_yahoo_finance_price-0.2.4/source_yahoo_finance_price/__init__.py
--rw-r--r--   0        0        0    15036 2024-04-20 23:28:42.000000 airbyte_source_yahoo_finance_price-0.2.4/source_yahoo_finance_price/manifest.yaml
--rw-r--r--   0        0        0      265 2024-04-20 23:28:42.000000 airbyte_source_yahoo_finance_price-0.2.4/source_yahoo_finance_price/run.py
--rw-r--r--   0        0        0      486 2024-04-20 23:28:42.000000 airbyte_source_yahoo_finance_price-0.2.4/source_yahoo_finance_price/source.py
--rw-r--r--   0        0        0     5473 1970-01-01 00:00:00.000000 airbyte_source_yahoo_finance_price-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     4740 2024-05-28 19:41:55.000000 airbyte_source_yahoo_finance_price-0.2.5/README.md
+-rw-r--r--   0        0        0      821 2024-05-28 19:58:50.738762 airbyte_source_yahoo_finance_price-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      146 2024-05-28 19:41:55.000000 airbyte_source_yahoo_finance_price-0.2.5/source_yahoo_finance_price/__init__.py
+-rw-r--r--   0        0        0    13824 2024-05-28 19:41:55.000000 airbyte_source_yahoo_finance_price-0.2.5/source_yahoo_finance_price/manifest.yaml
+-rw-r--r--   0        0        0      265 2024-05-28 19:41:55.000000 airbyte_source_yahoo_finance_price-0.2.5/source_yahoo_finance_price/run.py
+-rw-r--r--   0        0        0      486 2024-05-28 19:41:55.000000 airbyte_source_yahoo_finance_price-0.2.5/source_yahoo_finance_price/source.py
+-rw-r--r--   0        0        0     5483 1970-01-01 00:00:00.000000 airbyte_source_yahoo_finance_price-0.2.5/PKG-INFO
```

### Comparing `airbyte_source_yahoo_finance_price-0.2.4/README.md` & `airbyte_source_yahoo_finance_price-0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Yahoo-Finance-Price source connector
 
-
 This is the repository for the Yahoo-Finance-Price source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/yahoo-finance-price).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/yahoo-finance-price)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_yahoo_finance_price/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-yahoo-finance-price spec
 poetry run source-yahoo-finance-price check --config secrets/config.json
 poetry run source-yahoo-finance-price discover --config secrets/config.json
 poetry run source-yahoo-finance-price read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-yahoo-finance-price build
 ```
 
 An image will be available on your host with the tag `airbyte/source-yahoo-finance-price:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-yahoo-finance-price:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-yahoo-finance-price:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-yahoo-finance-price:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-yahoo-finance-price:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-yahoo-finance-price test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-yahoo-finance-price test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/yahoo-finance-price.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_yahoo_finance_price-0.2.4/pyproject.toml` & `airbyte_source_yahoo_finance_price-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.4"
+version = "0.2.5"
 name = "airbyte-source-yahoo-finance-price"
 description = "Source implementation for Yahoo Finance Price."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_yahoo_finance_price-0.2.4/source_yahoo_finance_price/manifest.yaml` & `airbyte_source_yahoo_finance_price-0.2.5/source_yahoo_finance_price/manifest.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,316 +1,77 @@
-version: 0.50.0
+version: 0.79.1
+
 type: DeclarativeSource
+
 check:
   type: CheckStream
   stream_names:
     - price
-streams:
-  - type: DeclarativeStream
-    name: price
-    primary_key: []
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
-        properties:
-          chart:
-            description: Contains the price data for the stock.
-            properties:
-              result:
-                description: Contains the information about the stock price.
-                items:
-                  properties:
-                    indicators:
-                      description: Contains technical indicators for the stock price.
-                      properties:
-                        quote:
-                          items:
-                            description: Contains the actual stock price data.
-                            properties:
-                              close:
-                                description: The closing price of the stock.
-                                items:
-                                  description:
-                                    Closing price of the stock for a specific
-                                    time period.
-                                  type:
-                                    - "null"
-                                    - number
-                                type: array
-                              high:
-                                description:
-                                  The highest price of the stock during the
-                                  trading period.
-                                items:
-                                  description:
-                                    Highest price the stock reached during
-                                    a specific time period.
-                                  type:
-                                    - "null"
-                                    - number
-                                type: array
-                              low:
-                                description:
-                                  The lowest price of the stock during the
-                                  trading period.
-                                items:
-                                  description:
-                                    Lowest price the stock reached during
-                                    a specific time period.
-                                  type:
-                                    - "null"
-                                    - number
-                                type: array
-                              open:
-                                description: The opening price of the stock.
-                                items:
-                                  description:
-                                    Opening price of the stock for a specific
-                                    time period.
-                                  type:
-                                    - "null"
-                                    - number
-                                type: array
-                              volume:
-                                description: The total volume of the stock traded.
-                                items:
-                                  description:
-                                    Total trading volume of the stock for
-                                    a specific time period.
-                                  type:
-                                    - "null"
-                                    - number
-                                type: array
-                            type: object
-                          type: array
-                      type: object
-                    meta:
-                      description: Contains metadata related to the stock price.
-                      properties:
-                        chartPreviousClose:
-                          description:
-                            Closing price of the stock from the previous
-                            trading day.
-                          type: number
-                        currency:
-                          description: Currency in which the prices are denoted.
-                          type:
-                            - "null"
-                            - string
-                        currentTradingPeriod:
-                          description:
-                            Contains information about different trading
-                            periods.
-                          properties:
-                            post:
-                              description: Information about post-trading period.
-                              properties:
-                                end:
-                                  description: End time of the post-market trading session.
-                                  type: number
-                                gmtoffset:
-                                  description: GMT offset for post-trading period.
-                                  type: number
-                                start:
-                                  description:
-                                    Start time of the post-market trading
-                                    session.
-                                  type: number
-                                timezone:
-                                  description:
-                                    Timezone in which the post-market trading
-                                    session occurs.
-                                  type: string
-                              type: object
-                            pre:
-                              description: Information about pre-trading period.
-                              properties:
-                                end:
-                                  description: End time of the pre-market trading session.
-                                  type: number
-                                gmtoffset:
-                                  description: GMT offset for pre-trading period.
-                                  type: number
-                                start:
-                                  description:
-                                    Start time of the pre-market trading
-                                    session.
-                                  type: number
-                                timezone:
-                                  description:
-                                    Timezone in which the pre-market trading
-                                    session occurs.
-                                  type: string
-                              type: object
-                            regular:
-                              description: Information about regular trading period.
-                              properties:
-                                end:
-                                  description: End time of the regular trading session.
-                                  type: number
-                                gmtoffset:
-                                  description: GMT offset for regular trading period.
-                                  type: number
-                                start:
-                                  description: Start time of the regular trading session.
-                                  type: number
-                                timezone:
-                                  description:
-                                    Timezone in which the regular trading
-                                    session occurs.
-                                  type: string
-                              type: object
-                          type: object
-                        dataGranularity:
-                          description:
-                            Granularity of the data intervals, like 1m, 1h,
-                            1d, etc.
-                          type: string
-                        exchangeName:
-                          description:
-                            Name of the stock exchange where the stock is
-                            traded.
-                          type: string
-                        exchangeTimezoneName:
-                          description: Timezone of the stock exchange.
-                          type: string
-                        firstTradeDate:
-                          description: Date of the stock's first trade on the exchange.
-                          type:
-                            - "null"
-                            - number
-                        gmtoffset:
-                          description: GMT Offset for the trading data.
-                          type: number
-                        instrumentType:
-                          description: Type of instrument, such as stock, ETF, etc.
-                          type: string
-                        previousClose:
-                          description:
-                            Closing price of the stock from the previous
-                            trading day.
-                          type: number
-                        priceHint:
-                          description: Decimal precision for the price data.
-                          type: number
-                        range:
-                          description:
-                            Price range for the stock during a specific time
-                            period.
-                          type: string
-                        regularMarketPrice:
-                          description: Price of the stock in the regular market session.
-                          type: number
-                        regularMarketTime:
-                          description:
-                            Time of the last price update in the regular
-                            market session.
-                          type: number
-                        scale:
-                          description: Numerical scale factor used to adjust prices.
-                          type: number
-                        symbol:
-                          description: Symbol or ticker of the stock.
-                          type: string
-                        timezone:
-                          description: Timezone where the trading data is provided.
-                          type: string
-                        tradingPeriods:
-                          description:
-                            Contains information about different trading
-                            periods.
-                          items:
-                            description: Contains individual trading periods.
-                            items:
-                              properties:
-                                end:
-                                  description: End time of a specific trading period.
-                                  type: number
-                                gmtoffset:
-                                  description: The GMT offset for the trading period.
-                                  type: number
-                                start:
-                                  description: Start time of a specific trading period.
-                                  type: number
-                                timezone:
-                                  description:
-                                    Timezone in which the trading period
-                                    occurs.
-                                  type: string
-                              type: object
-                            type: array
-                          type: array
-                        validRanges:
-                          description: Contains valid trading ranges for the stock.
-                          items:
-                            description: Ranges of valid trading data.
-                            type: string
-                          type: array
-                      type: object
-                    timestamp:
-                      description: The timestamp of the stock price data.
-                      items:
-                        description: Timestamp of the price data.
-                        type: number
-                      type: array
-                  type: object
-                type: array
-            type: object
-        required:
-          - chart
-        type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://query1.finance.yahoo.com
-        path: >-
-          {% if (next_page_token['next_page_token'] or 0) <
-          config['tickers'].split(',')|length %}/v8/finance/chart/{{
-          config['tickers'].split(',')[next_page_token['next_page_token'] or
-          0].strip() }}{% endif %}
-        http_method: GET
-        request_parameters:
-          range: "{{ config['range'] }}"
-          symbol: >-
+
+definitions:
+  streams:
+    price:
+      type: DeclarativeStream
+      name: price
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: >-
             {% if (next_page_token['next_page_token'] or 0) <
-            config['tickers'].split(',')|length %}{{
+            config['tickers'].split(',')|length %}/v8/finance/chart/{{
             config['tickers'].split(',')[next_page_token['next_page_token'] or
-            0].strip() }}{% else %} finish {% endif %}
-          interval: "{{ config['interval'] }}"
-        request_headers:
-          Accept: application/json
-          User-Agent: Mozilla/5.0 (X11; Linux x86_64)
-        authenticator:
-          type: NoAuth
-        error_handler:
-          type: CompositeErrorHandler
-          error_handlers:
-            - type: DefaultErrorHandler
-              response_filters:
-                - type: HttpResponseFilter
-                  action: SUCCESS
-                  http_codes:
-                    - 403
-        request_body_json: {}
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: DefaultPaginator
-        pagination_strategy:
-          type: PageIncrement
-          start_from_page: 0
+            0].strip() }}{% endif %}
+          http_method: GET
+          request_parameters:
+            range: "{{ config['range'] }}"
+            symbol: >-
+              {% if (next_page_token['next_page_token'] or 0) <
+              config['tickers'].split(',')|length %}{{
+              config['tickers'].split(',')[next_page_token['next_page_token'] or
+              0].strip() }}{% else %} finish {% endif %}
+            interval: "{{ config['interval'] }}"
+          request_headers:
+            Accept: application/json
+            User-Agent: Mozilla/5.0 (X11; Linux x86_64)
+          error_handler:
+            type: CompositeErrorHandler
+            error_handlers:
+              - type: DefaultErrorHandler
+                response_filters:
+                  - type: HttpResponseFilter
+                    action: SUCCESS
+                    http_codes:
+                      - 403
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+        paginator:
+          type: DefaultPaginator
+          pagination_strategy:
+            type: PageIncrement
+            start_from_page: 0
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/price"
+  base_requester:
+    type: HttpRequester
+    url_base: https://query1.finance.yahoo.com
+
+streams:
+  - $ref: "#/definitions/streams/price"
+
 spec:
+  type: Spec
   connection_specification:
-    $schema: http://json-schema.org/draft-07/schema#
     type: object
+    $schema: http://json-schema.org/draft-07/schema#
     required:
       - tickers
     properties:
       tickers:
         type: string
         order: 0
         title: Tickers
@@ -348,12 +109,247 @@
           - 6mo
           - 1y
           - 2y
           - 5y
           - ytd
           - max
     additionalProperties: true
-  documentation_url: https://example.org
-  type: Spec
+
 metadata:
   autoImportSchema:
     price: false
+
+schemas:
+  price:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      chart:
+        type: object
+        description: Contains the price data for the stock.
+        properties:
+          result:
+            type: array
+            description: Contains the information about the stock price.
+            items:
+              type: object
+              properties:
+                indicators:
+                  type: object
+                  description: Contains technical indicators for the stock price.
+                  properties:
+                    quote:
+                      type: array
+                      items:
+                        type: object
+                        description: Contains the actual stock price data.
+                        properties:
+                          close:
+                            type: array
+                            description: The closing price of the stock.
+                            items:
+                              type:
+                                - "null"
+                                - number
+                              description: >-
+                                Closing price of the stock for a specific time
+                                period.
+                          high:
+                            type: array
+                            description: >-
+                              The highest price of the stock during the trading
+                              period.
+                            items:
+                              type:
+                                - "null"
+                                - number
+                              description: >-
+                                Highest price the stock reached during a
+                                specific time period.
+                          low:
+                            type: array
+                            description: >-
+                              The lowest price of the stock during the trading
+                              period.
+                            items:
+                              type:
+                                - "null"
+                                - number
+                              description: >-
+                                Lowest price the stock reached during a specific
+                                time period.
+                          open:
+                            type: array
+                            description: The opening price of the stock.
+                            items:
+                              type:
+                                - "null"
+                                - number
+                              description: >-
+                                Opening price of the stock for a specific time
+                                period.
+                          volume:
+                            type: array
+                            description: The total volume of the stock traded.
+                            items:
+                              type:
+                                - "null"
+                                - number
+                              description: >-
+                                Total trading volume of the stock for a specific
+                                time period.
+                meta:
+                  type: object
+                  description: Contains metadata related to the stock price.
+                  properties:
+                    chartPreviousClose:
+                      type: number
+                      description: >-
+                        Closing price of the stock from the previous trading
+                        day.
+                    currency:
+                      type:
+                        - "null"
+                        - string
+                      description: Currency in which the prices are denoted.
+                    currentTradingPeriod:
+                      type: object
+                      description: Contains information about different trading periods.
+                      properties:
+                        post:
+                          type: object
+                          description: Information about post-trading period.
+                          properties:
+                            end:
+                              type: number
+                              description: End time of the post-market trading session.
+                            gmtoffset:
+                              type: number
+                              description: GMT offset for post-trading period.
+                            start:
+                              type: number
+                              description: Start time of the post-market trading session.
+                            timezone:
+                              type: string
+                              description: >-
+                                Timezone in which the post-market trading
+                                session occurs.
+                        pre:
+                          type: object
+                          description: Information about pre-trading period.
+                          properties:
+                            end:
+                              type: number
+                              description: End time of the pre-market trading session.
+                            gmtoffset:
+                              type: number
+                              description: GMT offset for pre-trading period.
+                            start:
+                              type: number
+                              description: Start time of the pre-market trading session.
+                            timezone:
+                              type: string
+                              description: >-
+                                Timezone in which the pre-market trading session
+                                occurs.
+                        regular:
+                          type: object
+                          description: Information about regular trading period.
+                          properties:
+                            end:
+                              type: number
+                              description: End time of the regular trading session.
+                            gmtoffset:
+                              type: number
+                              description: GMT offset for regular trading period.
+                            start:
+                              type: number
+                              description: Start time of the regular trading session.
+                            timezone:
+                              type: string
+                              description: >-
+                                Timezone in which the regular trading session
+                                occurs.
+                    dataGranularity:
+                      type: string
+                      description: Granularity of the data intervals, like 1m, 1h, 1d, etc.
+                    exchangeName:
+                      type: string
+                      description: Name of the stock exchange where the stock is traded.
+                    exchangeTimezoneName:
+                      type: string
+                      description: Timezone of the stock exchange.
+                    firstTradeDate:
+                      type:
+                        - "null"
+                        - number
+                      description: Date of the stock's first trade on the exchange.
+                    gmtoffset:
+                      type: number
+                      description: GMT Offset for the trading data.
+                    instrumentType:
+                      type: string
+                      description: Type of instrument, such as stock, ETF, etc.
+                    previousClose:
+                      type: number
+                      description: >-
+                        Closing price of the stock from the previous trading
+                        day.
+                    priceHint:
+                      type: number
+                      description: Decimal precision for the price data.
+                    range:
+                      type: string
+                      description: Price range for the stock during a specific time period.
+                    regularMarketPrice:
+                      type: number
+                      description: Price of the stock in the regular market session.
+                    regularMarketTime:
+                      type: number
+                      description: >-
+                        Time of the last price update in the regular market
+                        session.
+                    scale:
+                      type: number
+                      description: Numerical scale factor used to adjust prices.
+                    symbol:
+                      type: string
+                      description: Symbol or ticker of the stock.
+                    timezone:
+                      type: string
+                      description: Timezone where the trading data is provided.
+                    tradingPeriods:
+                      type: array
+                      description: Contains information about different trading periods.
+                      items:
+                        type: array
+                        description: Contains individual trading periods.
+                        items:
+                          type: object
+                          properties:
+                            end:
+                              type: number
+                              description: End time of a specific trading period.
+                            gmtoffset:
+                              type: number
+                              description: The GMT offset for the trading period.
+                            start:
+                              type: number
+                              description: Start time of a specific trading period.
+                            timezone:
+                              type: string
+                              description: Timezone in which the trading period occurs.
+                    validRanges:
+                      type: array
+                      description: Contains valid trading ranges for the stock.
+                      items:
+                        type: string
+                        description: Ranges of valid trading data.
+                timestamp:
+                  type: array
+                  description: The timestamp of the stock price data.
+                  items:
+                    type: number
+                    description: Timestamp of the price data.
+    required:
+      - chart
+    additionalProperties: true
```

### Comparing `airbyte_source_yahoo_finance_price-0.2.4/PKG-INFO` & `airbyte_source_yahoo_finance_price-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-yahoo-finance-price
-Version: 0.2.4
+Version: 0.2.5
 Summary: Source implementation for Yahoo Finance Price.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/yahoo-finance-price
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Yahoo-Finance-Price source connector
 
-
 This is the repository for the Yahoo-Finance-Price source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/yahoo-finance-price).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/yahoo-finance-price)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_yahoo_finance_price/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-yahoo-finance-price spec
 poetry run source-yahoo-finance-price check --config secrets/config.json
 poetry run source-yahoo-finance-price discover --config secrets/config.json
 poetry run source-yahoo-finance-price read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-yahoo-finance-price build
 ```
 
 An image will be available on your host with the tag `airbyte/source-yahoo-finance-price:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-yahoo-finance-price:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-yahoo-finance-price:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-yahoo-finance-price:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-yahoo-finance-price:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-yahoo-finance-price test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-yahoo-finance-price test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/yahoo-finance-price.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

