# Comparing `tmp/airbyte_source_gong-0.1.5.tar.gz` & `tmp/airbyte_source_gong-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_gong-0.1.5.tar", max compression
+gzip compressed data, was "airbyte_source_gong-0.1.6.tar", max compression
```

## Comparing `airbyte_source_gong-0.1.5.tar` & `airbyte_source_gong-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4460 2024-05-01 18:45:02.094853 airbyte_source_gong-0.1.5/README.md
--rw-r--r--   0        0        0      731 2024-05-01 18:48:11.099686 airbyte_source_gong-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      120 2024-05-01 18:45:02.094853 airbyte_source_gong-0.1.5/source_gong/__init__.py
--rw-r--r--   0        0        0    14860 2024-05-01 18:45:02.094853 airbyte_source_gong-0.1.5/source_gong/manifest.yaml
--rw-r--r--   0        0        0      224 2024-05-01 18:45:02.094853 airbyte_source_gong-0.1.5/source_gong/run.py
--rw-r--r--   0        0        0      473 2024-05-01 18:45:02.094853 airbyte_source_gong-0.1.5/source_gong/source.py
--rw-r--r--   0        0        0     1017 2024-05-01 18:45:02.094853 airbyte_source_gong-0.1.5/source_gong/spec.yaml
--rw-r--r--   0        0        0     5158 1970-01-01 00:00:00.000000 airbyte_source_gong-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4470 2024-05-28 19:40:53.000000 airbyte_source_gong-0.1.6/README.md
+-rw-r--r--   0        0        0      731 2024-05-28 19:57:38.638934 airbyte_source_gong-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-05-28 19:40:53.000000 airbyte_source_gong-0.1.6/source_gong/__init__.py
+-rw-r--r--   0        0        0    17001 2024-05-28 19:40:53.000000 airbyte_source_gong-0.1.6/source_gong/manifest.yaml
+-rw-r--r--   0        0        0      224 2024-05-28 19:40:53.000000 airbyte_source_gong-0.1.6/source_gong/run.py
+-rw-r--r--   0        0        0      473 2024-05-28 19:40:53.000000 airbyte_source_gong-0.1.6/source_gong/source.py
+-rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 airbyte_source_gong-0.1.6/PKG-INFO
```

### Comparing `airbyte_source_gong-0.1.5/README.md` & `airbyte_source_gong-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Gong source connector
 
-
 This is the repository for the Gong source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/gong).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/gong)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_gong/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-gong spec
 poetry run source-gong check --config secrets/config.json
 poetry run source-gong discover --config secrets/config.json
 poetry run source-gong read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-gong build
 ```
 
 An image will be available on your host with the tag `airbyte/source-gong:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-gong:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-gong:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-gong:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-gong:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-gong test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-gong test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/gong.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_gong-0.1.5/pyproject.toml` & `airbyte_source_gong-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.1.5"
+version = "0.1.6"
 name = "airbyte-source-gong"
 description = "Source implementation for Gong."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_gong-0.1.5/source_gong/manifest.yaml` & `airbyte_source_gong-0.1.6/source_gong/manifest.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,490 +1,597 @@
-version: "0.29.0"
+version: 0.79.1
+
+type: DeclarativeSource
+
+check:
+  type: CheckStream
+  stream_names:
+    - users
 
 definitions:
-  selector:
-    extractor:
-      field_path: ["{{ parameters.name }}"]
-  requester:
-    url_base: "https://api.gong.io/v2/"
-    http_method: "GET"
+  streams:
+    users:
+      type: DeclarativeStream
+      name: users
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /users
+          http_method: GET
+          request_parameters:
+            fromDateTime: "{{ config['start_date'] }}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - users
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: cursor
+          page_size_option:
+            type: RequestOption
+            field_name: limit
+            inject_into: request_parameter
+          pagination_strategy:
+            type: CursorPagination
+            page_size: 100
+            cursor_value: "{{ response.records.cursor }}"
+            stop_condition: "{{ 'records' not in response }}"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/users"
+    calls:
+      type: DeclarativeStream
+      name: calls
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /calls
+          http_method: GET
+          request_parameters:
+            fromDateTime: "{{ config['start_date'] }}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - calls
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: cursor
+          pagination_strategy:
+            type: CursorPagination
+            cursor_value: "{{ response.records.cursor }}"
+            stop_condition: "{{ 'records' not in response }}"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/calls"
+    scorecards:
+      type: DeclarativeStream
+      name: scorecards
+      primary_key:
+        - scorecardId
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /settings/scorecards
+          http_method: GET
+          request_parameters:
+            fromDateTime: "{{ config['start_date'] }}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - scorecards
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: cursor
+          page_size_option:
+            type: RequestOption
+            field_name: limit
+            inject_into: request_parameter
+          pagination_strategy:
+            type: CursorPagination
+            page_size: 100
+            cursor_value: "{{ response.records.cursor }}"
+            stop_condition: "{{ 'records' not in response }}"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/scorecards"
+    answeredScorecards:
+      type: DeclarativeStream
+      name: answeredScorecards
+      primary_key:
+        - answeredScorecardId
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /stats/activity/scorecards
+          http_method: POST
+          request_parameters:
+            fromDateTime: "{{ config['start_date'] }}"
+          request_body_json:
+            filter: '{"callFromDate": "{{ config["start_date"] }}"}'
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - answeredScorecards
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: body_json
+            field_name: cursor
+          page_size_option:
+            type: RequestOption
+            field_name: limit
+            inject_into: body_json
+          pagination_strategy:
+            type: CursorPagination
+            page_size: 100
+            cursor_value: "{{ response.records.cursor }}"
+            stop_condition: "{{ 'records' not in response }}"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/answeredScorecards"
+  base_requester:
+    type: HttpRequester
+    url_base: https://api.gong.io/v2/
     authenticator:
       type: BasicHttpAuthenticator
       username: "{{ config['access_key'] }}"
       password: "{{ config['access_key_secret'] }}"
-    request_parameters:
-      fromDateTime: "{{ config['start_date'] }}"
-  retriever:
-    record_selector:
-      $ref: "#/definitions/selector"
-    paginator:
-      type: DefaultPaginator
-      pagination_strategy:
-        type: "CursorPagination"
-        cursor_value: "{{ response.records.cursor }}"
-        stop_condition: "{{ 'records' not in response }}"
-        page_size: 100
-      page_size_option:
-        field_name: "limit"
-        inject_into: "request_parameter"
-      page_token_option:
-        type: RequestOption
-        field_name: "cursor"
-        inject_into: "request_parameter"
-    requester:
-      $ref: "#/definitions/requester"
-
-  # base stream
-  base_stream:
-    retriever:
-      $ref: "#/definitions/retriever"
 
-  # streams
-  users_stream:
-    $ref: "#/definitions/base_stream"
-    $parameters:
-      name: "users"
-      primary_key: "id"
-      path: "/users"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        type: object
-        properties:
-          id:
-            description: Unique identifier for the user
-            type:
-              - "null"
-              - string
-          emailAddress:
-            description: The primary email address associated with the user
-            type:
-              - "null"
-              - string
-          trustedEmailAddress:
-            description: An email address that is considered trusted for the user
-            type:
-              - "null"
-              - string
-          created:
-            description: The timestamp denoting when the user account was created
-            type:
-              - "null"
-              - string
-            format: date-time
-          active:
-            description: Indicates if the user is currently active or not
-            type:
-              - "null"
-              - boolean
-          emailAliases:
-            description:
-              Additional email addresses that can be used to reach the
-              user
-            type:
-              - "null"
-              - array
-          firstName:
-            description: The first name of the user
-            type:
-              - "null"
-              - string
-          lastName:
-            description: The last name of the user
-            type:
-              - "null"
-              - string
-          title:
-            description: The job title or position of the user
-            type:
-              - "null"
-              - string
-          phoneNumber:
-            description: The phone number associated with the user
-            type:
-              - "null"
-              - string
-          extension:
-            description: The phone extension number for the user
-            type:
-              - "null"
-              - string
-          personalMeetingUrls:
-            description: URLs for personal meeting rooms assigned to the user
-            type:
-              - "null"
-              - array
-          settings:
-            description: User-specific settings and configurations
-            type:
-              - "null"
-              - object
-          managerId:
-            description: The ID of the user's manager
-            type:
-              - "null"
-              - string
-          meetingConsentPageUrl:
-            description: URL for the consent page related to meetings
-            type:
-              - "null"
-              - string
-          spokenLanguages:
-            description: Languages spoken by the user
-            type:
-              - "null"
-              - array
-  calls_stream:
-    $ref: "#/definitions/base_stream"
-    $parameters:
-      name: "calls"
-      primary_key: "id"
-      path: "/calls"
+streams:
+  - $ref: "#/definitions/streams/users"
+  - $ref: "#/definitions/streams/calls"
+  - $ref: "#/definitions/streams/scorecards"
+  - $ref: "#/definitions/streams/answeredScorecards"
 
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        type: object
-        properties:
-          id:
-            description: Unique identifier for the call.
-            type:
-              - "null"
-              - string
-          url:
-            description: URL associated with the call.
-            type:
-              - "null"
-              - string
-          title:
-            description: Title or headline of the call.
-            type:
-              - "null"
-              - string
-          scheduled:
-            description: Scheduled date and time of the call.
-            type:
-              - "null"
-              - string
-            format: date-time
-          started:
-            description: Start date and time of the call.
-            type:
-              - "null"
-              - string
-            format: date-time
-          duration:
-            description: Duration of the call in seconds.
-            type:
-              - "null"
-              - integer
-          primaryUserId:
-            description: Unique identifier for the primary user involved in the call.
-            type:
-              - "null"
-              - string
-          direction:
-            description: Direction of the call (inbound/outbound).
-            type:
-              - "null"
-              - string
-          system:
-            description: System information related to the call.
-            type:
-              - "null"
-              - string
-          scope:
-            description: Scope or extent of the call.
-            type:
-              - "null"
-              - string
-          media:
-            description: Media type used for communication (voice, video, etc.).
-            type:
-              - "null"
-              - string
-          language:
-            description: Language used in the call.
-            type:
-              - "null"
-              - string
-          workspaceId:
-            description: Identifier for the workspace to which the call belongs.
-            type:
-              - "null"
-              - string
-          sdrDisposition:
-            description: Disposition set by the sales development representative.
-            type:
-              - "null"
-              - string
-          clientUniqueId:
-            description: Unique identifier for the client related to the call.
-            type:
-              - "null"
-              - string
-          customData:
-            description: Custom data associated with the call.
-            type:
-              - "null"
-              - string
-          purpose:
-            description: Purpose or topic of the call.
-            type:
-              - "null"
-              - string
-          meetingUrl:
-            description: URL for accessing the meeting associated with the call.
-            type:
-              - "null"
-              - string
-          isPrivate:
-            description: Indicates if the call is private or not.
-            type:
-              - "null"
-              - boolean
-          calendarEventId:
-            description:
-              Unique identifier for the calendar event associated with
-              the call.
-            type:
-              - "null"
-              - string
-  scorecards_stream:
-    $ref: "#/definitions/base_stream"
-    $parameters:
-      name: "scorecards"
-      primary_key: "scorecardId"
-      path: "/settings/scorecards"
+spec:
+  type: Spec
+  connection_specification:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    required:
+      - access_key
+      - access_key_secret
+    properties:
+      access_key:
+        type: string
+        title: Gong Access Key
+        description: Gong Access Key
+        airbyte_secret: true
+        order: 0
+      access_key_secret:
+        type: string
+        title: Gong Access Key Secret
+        description: Gong Access Key Secret
+        airbyte_secret: true
+        order: 1
+      start_date:
+        type: string
+        title: Start date
+        pattern: ^[0-9]{4}-[0-9]{2}-[0-9]{2}T[0-9]{2}:[0-9]{2}:[0-9]{2}Z$
+        description: >-
+          The date from which to list calls, in the ISO-8601 format; if not
+          specified, the calls start with the earliest recorded call. For
+          web-conference calls recorded by Gong, the date denotes its scheduled
+          time, otherwise, it denotes its actual start time.
+        examples:
+          - "2018-02-18T08:00:00Z"
+        order: 2
+    additionalProperties: true
 
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        type: object
-        properties:
-          scorecardId:
-            description: The unique identifier of the scorecard
-            type:
-              - "null"
-              - string
-          scorecardName:
-            description: The name of the scorecard
-            type:
-              - "null"
-              - string
-          workspaceId:
-            description:
-              The unique identifier of the workspace associated with the
-              scorecard
-            type:
-              - "null"
-              - string
-          enabled:
-            description: Indicates if the scorecard is enabled or disabled
-            type:
-              - "null"
-              - boolean
-          updaterUserId:
-            description: The user ID of the person who last updated the scorecard
-            type:
-              - "null"
-              - string
-          created:
-            description: The timestamp when the scorecard was created
-            type:
-              - "null"
-              - string
-            format: date-time
-          updated:
-            description: The timestamp when the scorecard was last updated
-            type:
-              - "null"
-              - string
-            format: date-time
-          questions:
-            description: An array of questions related to the scorecard
-            type:
-              - "null"
-              - array
-            items:
-              type:
-                - "null"
-                - object
-              properties:
-                questionId:
-                  description: The unique identifier of the question
-                  type:
-                    - "null"
-                    - string
-                questionRevisionId:
-                  description: The revision identifier of the question
-                  type:
-                    - "null"
-                    - string
-                questionText:
-                  description: The text of the question
-                  type:
-                    - "null"
-                    - string
-                isOverall:
-                  description: Indicates if the question is an overall score or not
-                  type:
-                    - "null"
-                    - boolean
-                updaterUserId:
-                  description: The user ID of the person who last updated the question
-                  type:
-                    - "null"
-                    - string
-                created:
-                  description: The timestamp when the question was created
-                  type:
-                    - "null"
-                    - string
-                  format: date-time
-                updated:
-                  description: The timestamp when the question was last updated
-                  type:
-                    - "null"
-                    - string
-                  format: date-time
-  answered_scorecards_stream:
-    $ref: "#/definitions/base_stream"
-    $parameters:
-      name: "answeredScorecards"
-      primary_key: "answeredScorecardId"
-      path: "/stats/activity/scorecards"
-    retriever:
-      $ref: "#/definitions/base_stream/retriever"
-      paginator:
-        $ref: "#/definitions/retriever/paginator"
-        page_size_option:
-          field_name: "limit"
-          inject_into: "body_json"
-        page_token_option:
-          type: RequestOption
-          field_name: "cursor"
-          inject_into: "body_json"
-      requester:
-        $ref: "#/definitions/requester"
-        http_method: "POST"
-        request_body_json:
-          filter: '{"callFromDate": "{{ config["start_date"] }}"}'
+metadata:
+  autoImportSchema:
+    users: false
+    calls: false
+    scorecards: false
+    answeredScorecards: false
 
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        type: object
-        properties:
-          answeredScorecardId:
-            description: Unique identifier for the answered scorecard instance.
-            type:
-              - "null"
-              - string
-          scorecardId:
-            description: Unique identifier for the scorecard template used.
-            type:
-              - "null"
-              - string
-          scorecardName:
-            description: Name or title of the scorecard template used.
-            type:
-              - "null"
-              - string
-          callId:
-            description:
-              Unique identifier for the call associated with the answered
-              scorecard.
-            type:
-              - "null"
-              - string
-          callStartTime:
-            description: Timestamp indicating the start time of the call.
-            type:
-              - "null"
-              - string
-            format: date-time
-          reviewedUserId:
-            description: Unique identifier for the user whose performance was reviewed.
-            type:
-              - "null"
-              - string
-          reviewerUserId:
-            description: Unique identifier for the user who performed the review.
-            type:
-              - "null"
-              - string
-          reviewTime:
-            description:
-              Timestamp indicating when the review of the answered scorecard
-              was completed.
-            type:
-              - "null"
-              - string
-            format: date-time
-          visibilityType:
-            description:
-              Type indicating the visibility permissions for the answered
-              scorecard.
-            type:
-              - "null"
-              - string
-          answers:
-            description: Contains the answered questions in the scorecards
-            type:
-              - "null"
-              - array
-            items:
-              type:
-                - "null"
-                - object
-              properties:
-                questionId:
-                  description: Unique identifier for the question answered.
-                  type:
-                    - "null"
-                    - string
-                questionRevisionId:
-                  description:
-                    Unique identifier for the revision of the question
-                    answered.
-                  type:
-                    - "null"
-                    - string
-                isOverall:
-                  description:
-                    Boolean flag indicating if the answer is for an overall
-                    evaluation.
-                  type:
-                    - "null"
-                    - boolean
-                score:
-                  description: Numeric score assigned to the answer.
-                  type:
-                    - "null"
-                    - integer
-                answerText:
-                  description: Text containing the answer given.
-                  type:
-                    - "null"
-                    - string
-                notApplicable:
-                  description:
-                    Boolean flag indicating if the question is marked as
-                    not applicable.
-                  type:
-                    - "null"
-                    - boolean
-streams:
-  - "#/definitions/users_stream"
-  - "#/definitions/calls_stream"
-  - "#/definitions/scorecards_stream"
-  - "#/definitions/answered_scorecards_stream"
-
-check:
-  stream_names:
-    - "users"
+schemas:
+  users:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      active:
+        type:
+          - "null"
+          - boolean
+        description: Indicates if the user is currently active or not
+      created:
+        type:
+          - "null"
+          - string
+        description: The timestamp denoting when the user account was created
+        format: date-time
+      emailAddress:
+        type:
+          - "null"
+          - string
+        description: The primary email address associated with the user
+      emailAliases:
+        type:
+          - "null"
+          - array
+        description: Additional email addresses that can be used to reach the user
+      extension:
+        type:
+          - "null"
+          - string
+        description: The phone extension number for the user
+      firstName:
+        type:
+          - "null"
+          - string
+        description: The first name of the user
+      id:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the user
+      lastName:
+        type:
+          - "null"
+          - string
+        description: The last name of the user
+      managerId:
+        type:
+          - "null"
+          - string
+        description: The ID of the user's manager
+      meetingConsentPageUrl:
+        type:
+          - "null"
+          - string
+        description: URL for the consent page related to meetings
+      personalMeetingUrls:
+        type:
+          - "null"
+          - array
+        description: URLs for personal meeting rooms assigned to the user
+      phoneNumber:
+        type:
+          - "null"
+          - string
+        description: The phone number associated with the user
+      settings:
+        type:
+          - "null"
+          - object
+        description: User-specific settings and configurations
+      spokenLanguages:
+        type:
+          - "null"
+          - array
+        description: Languages spoken by the user
+      title:
+        type:
+          - "null"
+          - string
+        description: The job title or position of the user
+      trustedEmailAddress:
+        type:
+          - "null"
+          - string
+        description: An email address that is considered trusted for the user
+  calls:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      calendarEventId:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the calendar event associated with the call.
+      clientUniqueId:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the client related to the call.
+      customData:
+        type:
+          - "null"
+          - string
+        description: Custom data associated with the call.
+      direction:
+        type:
+          - "null"
+          - string
+        description: Direction of the call (inbound/outbound).
+      duration:
+        type:
+          - "null"
+          - integer
+        description: Duration of the call in seconds.
+      id:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the call.
+      isPrivate:
+        type:
+          - "null"
+          - boolean
+        description: Indicates if the call is private or not.
+      language:
+        type:
+          - "null"
+          - string
+        description: Language used in the call.
+      media:
+        type:
+          - "null"
+          - string
+        description: Media type used for communication (voice, video, etc.).
+      meetingUrl:
+        type:
+          - "null"
+          - string
+        description: URL for accessing the meeting associated with the call.
+      primaryUserId:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the primary user involved in the call.
+      purpose:
+        type:
+          - "null"
+          - string
+        description: Purpose or topic of the call.
+      scheduled:
+        type:
+          - "null"
+          - string
+        description: Scheduled date and time of the call.
+        format: date-time
+      scope:
+        type:
+          - "null"
+          - string
+        description: Scope or extent of the call.
+      sdrDisposition:
+        type:
+          - "null"
+          - string
+        description: Disposition set by the sales development representative.
+      started:
+        type:
+          - "null"
+          - string
+        description: Start date and time of the call.
+        format: date-time
+      system:
+        type:
+          - "null"
+          - string
+        description: System information related to the call.
+      title:
+        type:
+          - "null"
+          - string
+        description: Title or headline of the call.
+      url:
+        type:
+          - "null"
+          - string
+        description: URL associated with the call.
+      workspaceId:
+        type:
+          - "null"
+          - string
+        description: Identifier for the workspace to which the call belongs.
+  scorecards:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      created:
+        type:
+          - "null"
+          - string
+        description: The timestamp when the scorecard was created
+        format: date-time
+      enabled:
+        type:
+          - "null"
+          - boolean
+        description: Indicates if the scorecard is enabled or disabled
+      questions:
+        type:
+          - "null"
+          - array
+        description: An array of questions related to the scorecard
+        items:
+          type:
+            - "null"
+            - object
+          properties:
+            created:
+              type:
+                - "null"
+                - string
+              description: The timestamp when the question was created
+              format: date-time
+            isOverall:
+              type:
+                - "null"
+                - boolean
+              description: Indicates if the question is an overall score or not
+            questionId:
+              type:
+                - "null"
+                - string
+              description: The unique identifier of the question
+            questionRevisionId:
+              type:
+                - "null"
+                - string
+              description: The revision identifier of the question
+            questionText:
+              type:
+                - "null"
+                - string
+              description: The text of the question
+            updated:
+              type:
+                - "null"
+                - string
+              description: The timestamp when the question was last updated
+              format: date-time
+            updaterUserId:
+              type:
+                - "null"
+                - string
+              description: The user ID of the person who last updated the question
+      scorecardId:
+        type:
+          - "null"
+          - string
+        description: The unique identifier of the scorecard
+      scorecardName:
+        type:
+          - "null"
+          - string
+        description: The name of the scorecard
+      updated:
+        type:
+          - "null"
+          - string
+        description: The timestamp when the scorecard was last updated
+        format: date-time
+      updaterUserId:
+        type:
+          - "null"
+          - string
+        description: The user ID of the person who last updated the scorecard
+      workspaceId:
+        type:
+          - "null"
+          - string
+        description: The unique identifier of the workspace associated with the scorecard
+  answeredScorecards:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      answeredScorecardId:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the answered scorecard instance.
+      answers:
+        type:
+          - "null"
+          - array
+        description: Contains the answered questions in the scorecards
+        items:
+          type:
+            - "null"
+            - object
+          properties:
+            answerText:
+              type:
+                - "null"
+                - string
+              description: Text containing the answer given.
+            isOverall:
+              type:
+                - "null"
+                - boolean
+              description: >-
+                Boolean flag indicating if the answer is for an overall
+                evaluation.
+            notApplicable:
+              type:
+                - "null"
+                - boolean
+              description: >-
+                Boolean flag indicating if the question is marked as not
+                applicable.
+            questionId:
+              type:
+                - "null"
+                - string
+              description: Unique identifier for the question answered.
+            questionRevisionId:
+              type:
+                - "null"
+                - string
+              description: Unique identifier for the revision of the question answered.
+            score:
+              type:
+                - "null"
+                - integer
+              description: Numeric score assigned to the answer.
+      callId:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the call associated with the answered scorecard.
+      callStartTime:
+        type:
+          - "null"
+          - string
+        description: Timestamp indicating the start time of the call.
+        format: date-time
+      reviewTime:
+        type:
+          - "null"
+          - string
+        description: >-
+          Timestamp indicating when the review of the answered scorecard was
+          completed.
+        format: date-time
+      reviewedUserId:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the user whose performance was reviewed.
+      reviewerUserId:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the user who performed the review.
+      scorecardId:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the scorecard template used.
+      scorecardName:
+        type:
+          - "null"
+          - string
+        description: Name or title of the scorecard template used.
+      visibilityType:
+        type:
+          - "null"
+          - string
+        description: Type indicating the visibility permissions for the answered scorecard.
```

### Comparing `airbyte_source_gong-0.1.5/PKG-INFO` & `airbyte_source_gong-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-gong
-Version: 0.1.5
+Version: 0.1.6
 Summary: Source implementation for Gong.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/gong
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Gong source connector
 
-
 This is the repository for the Gong source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/gong).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/gong)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_gong/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-gong spec
 poetry run source-gong check --config secrets/config.json
 poetry run source-gong discover --config secrets/config.json
 poetry run source-gong read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-gong build
 ```
 
 An image will be available on your host with the tag `airbyte/source-gong:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-gong:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-gong:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-gong:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-gong:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-gong test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-gong test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/gong.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

