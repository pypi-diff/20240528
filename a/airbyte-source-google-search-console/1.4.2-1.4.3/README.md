# Comparing `tmp/airbyte_source_google_search_console-1.4.2.tar.gz` & `tmp/airbyte_source_google_search_console-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_google_search_console-1.4.2.tar", max compression
+gzip compressed data, was "airbyte_source_google_search_console-1.4.3.tar", max compression
```

## Comparing `airbyte_source_google_search_console-1.4.2.tar` & `airbyte_source_google_search_console-1.4.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0     4771 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/README.md
--rw-r--r--   0        0        0      930 2024-05-07 12:21:58.536642 airbyte_source_google_search_console-1.4.2/pyproject.toml
--rwxr-xr-x   0        0        0     1191 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/__init__.py
--rw-r--r--   0        0        0     4134 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/config_migrations.py
--rw-r--r--   0        0        0     1097 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/exceptions.py
--rwxr-xr-x   0        0        0      462 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/run.py
--rw-r--r--   0        0        0     1729 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_all_fields.json
--rw-r--r--   0        0        0     1491 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_country.json
--rw-r--r--   0        0        0     1388 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_date.json
--rw-r--r--   0        0        0     1525 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_device.json
--rw-r--r--   0        0        0     1473 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_page.json
--rw-r--r--   0        0        0     1439 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_query.json
--rw-r--r--   0        0        0     1681 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_keyword_page_report.json
--rw-r--r--   0        0        0     1626 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_keyword_site_report_by_page.json
--rw-r--r--   0        0        0     1755 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_keyword_site_report_by_site.json
--rw-r--r--   0        0        0     1776 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_page_report.json
--rw-r--r--   0        0        0     1515 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_site_report_by_page.json
--rw-r--r--   0        0        0     1408 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_site_report_by_site.json
--rw-r--r--   0        0        0     1775 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/sitemaps.json
--rw-r--r--   0        0        0      383 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/sites.json
--rwxr-xr-x   0        0        0     1225 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/service_account_authenticator.py
--rwxr-xr-x   0        0        0    10013 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/source.py
--rwxr-xr-x   0        0        0     8470 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/spec.json
--rwxr-xr-x   0        0        0    18404 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/streams.py
--rw-r--r--   0        0        0     5609 1970-01-01 00:00:00.000000 airbyte_source_google_search_console-1.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     4781 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/README.md
+-rw-r--r--   0        0        0      930 2024-05-28 13:57:54.408971 airbyte_source_google_search_console-1.4.3/pyproject.toml
+-rwxr-xr-x   0        0        0     1191 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/__init__.py
+-rw-r--r--   0        0        0     4134 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/config_migrations.py
+-rw-r--r--   0        0        0     1097 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/exceptions.py
+-rwxr-xr-x   0        0        0      462 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/run.py
+-rw-r--r--   0        0        0     1729 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_all_fields.json
+-rw-r--r--   0        0        0     1491 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_by_country.json
+-rw-r--r--   0        0        0     1388 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_by_date.json
+-rw-r--r--   0        0        0     1525 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_by_device.json
+-rw-r--r--   0        0        0     1473 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_by_page.json
+-rw-r--r--   0        0        0     1439 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_by_query.json
+-rw-r--r--   0        0        0     1681 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_keyword_page_report.json
+-rw-r--r--   0        0        0     1626 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_keyword_site_report_by_page.json
+-rw-r--r--   0        0        0     1755 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_keyword_site_report_by_site.json
+-rw-r--r--   0        0        0     1776 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_page_report.json
+-rw-r--r--   0        0        0     1515 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_site_report_by_page.json
+-rw-r--r--   0        0        0     1408 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_site_report_by_site.json
+-rw-r--r--   0        0        0     1775 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/sitemaps.json
+-rw-r--r--   0        0        0      383 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/sites.json
+-rwxr-xr-x   0        0        0     1225 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/service_account_authenticator.py
+-rwxr-xr-x   0        0        0    10029 2024-05-28 13:53:06.115216 airbyte_source_google_search_console-1.4.3/source_google_search_console/source.py
+-rwxr-xr-x   0        0        0     8470 2024-05-28 13:53:06.119216 airbyte_source_google_search_console-1.4.3/source_google_search_console/spec.json
+-rwxr-xr-x   0        0        0    18331 2024-05-28 13:53:06.119216 airbyte_source_google_search_console-1.4.3/source_google_search_console/streams.py
+-rw-r--r--   0        0        0     5619 1970-01-01 00:00:00.000000 airbyte_source_google_search_console-1.4.3/PKG-INFO
```

### Comparing `airbyte_source_google_search_console-1.4.2/README.md` & `airbyte_source_google_search_console-1.4.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Google-Search-Console source connector
 
-
 This is the repository for the Google-Search-Console source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/google-search-console).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/google-search-console)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_google_search_console/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-google-search-console spec
 poetry run source-google-search-console check --config secrets/config.json
 poetry run source-google-search-console discover --config secrets/config.json
 poetry run source-google-search-console read --config secrets/config.json --catalog integration_tests/configured_catalog.json
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
 airbyte-ci connectors --name=source-google-search-console build
 ```
 
 An image will be available on your host with the tag `airbyte/source-google-search-console:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-google-search-console:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-google-search-console:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-google-search-console:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-google-search-console:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-google-search-console test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-google-search-console test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/google-search-console.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_google_search_console-1.4.2/pyproject.toml` & `airbyte_source_google_search_console-1.4.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.4.2"
+version = "1.4.3"
 name = "airbyte-source-google-search-console"
 description = "Source implementation for Google Search Console."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "Elv2"
 readme = "README.md"
@@ -19,15 +19,15 @@
 packages = [
     { include = "source_google_search_console" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 google-api-python-client = "==2.105.0"
-airbyte-cdk = "0.80.0"
+airbyte-cdk = "0.90.0"
 google-auth = "==2.23.3"
 
 [tool.poetry.scripts]
 source-google-search-console = "source_google_search_console.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.11.0"
```

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/__init__.py` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/config_migrations.py` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/exceptions.py` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_all_fields.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_all_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_country.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_by_country.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_date.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_by_date.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_device.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_by_device.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_page.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_by_page.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_query.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_by_query.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_keyword_page_report.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_keyword_page_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_keyword_site_report_by_page.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_keyword_site_report_by_page.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_keyword_site_report_by_site.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_keyword_site_report_by_site.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_page_report.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_page_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_site_report_by_page.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_site_report_by_page.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_site_report_by_site.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/search_analytics_site_report_by_site.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/sitemaps.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/schemas/sitemaps.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/service_account_authenticator.py` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/service_account_authenticator.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/source.py` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import jsonschema
 import pendulum
 import requests
 from airbyte_cdk.logger import AirbyteLogger
 from airbyte_cdk.models import FailureType, SyncMode
 from airbyte_cdk.sources import AbstractSource
 from airbyte_cdk.sources.streams import Stream
-from airbyte_cdk.sources.streams.http.auth import Oauth2Authenticator
+from airbyte_cdk.sources.streams.http.requests_native_auth import Oauth2Authenticator
 from airbyte_cdk.utils import AirbyteTracedException
 from source_google_search_console.exceptions import (
     InvalidSiteURLValidationError,
     UnauthorizedOauthError,
     UnauthorizedServiceAccountError,
     UnidentifiedError,
 )
```

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/spec.json` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.2/source_google_search_console/streams.py` & `airbyte_source_google_search_console-1.4.3/source_google_search_console/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Dict, Iterable, List, Mapping, MutableMapping, Optional, Union
 from urllib.parse import quote_plus, unquote_plus
 
 import pendulum
 import requests
 from airbyte_cdk.models import SyncMode
 from airbyte_cdk.sources.streams.http import HttpStream
-from airbyte_cdk.sources.streams.http.auth import HttpAuthenticator
+from requests.auth import AuthBase
 
 BASE_URL = "https://www.googleapis.com/webmasters/v3/"
 ROW_LIMIT = 25000
 
 
 class QueryAggregationType(Enum):
     auto = "auto"
@@ -26,15 +26,15 @@
 class GoogleSearchConsole(HttpStream, ABC):
     url_base = BASE_URL
     data_field = ""
     raise_on_http_errors = True
 
     def __init__(
         self,
-        authenticator: Union[HttpAuthenticator, requests.auth.AuthBase],
+        authenticator: AuthBase,
         site_urls: list,
         start_date: str,
         end_date: str,
         data_state: str = "final",
     ):
         super().__init__(authenticator=authenticator)
         self._site_urls = self.sanitize_urls_list(site_urls)
@@ -362,15 +362,15 @@
         self,
         stream_state: Mapping[str, Any] = None,
         stream_slice: Mapping[str, Any] = None,
         next_page_token: Mapping[str, Any] = None,
     ) -> Optional[Union[Dict[str, Any], str]]:
         data = super().request_body_json(stream_state, stream_slice, next_page_token)
 
-        stream = SearchAppearance(self.authenticator, self._site_urls, self._start_date, self._end_date)
+        stream = SearchAppearance(self._session.auth, self._site_urls, self._start_date, self._end_date)
         keywords_records = stream.read_records(sync_mode=SyncMode.full_refresh, stream_state=stream_state, stream_slice=stream_slice)
         keywords = {record["searchAppearance"] for record in keywords_records}
         filters = []
         for keyword in keywords:
             filters.append({"dimension": "searchAppearance", "operator": "equals", "expression": keyword})
 
         data["dimensionFilterGroups"] = [{"filters": filters}]
```

### Comparing `airbyte_source_google_search_console-1.4.2/PKG-INFO` & `airbyte_source_google_search_console-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,112 +1,126 @@
 Metadata-Version: 2.1
 Name: airbyte-source-google-search-console
-Version: 1.4.2
+Version: 1.4.3
 Summary: Source implementation for Google Search Console.
 Home-page: https://airbyte.com
 License: Elv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.80.0)
+Requires-Dist: airbyte-cdk (==0.90.0)
 Requires-Dist: google-api-python-client (==2.105.0)
 Requires-Dist: google-auth (==2.23.3)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/google-search-console
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Google-Search-Console source connector
 
-
 This is the repository for the Google-Search-Console source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/google-search-console).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/google-search-console)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_google_search_console/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-google-search-console spec
 poetry run source-google-search-console check --config secrets/config.json
 poetry run source-google-search-console discover --config secrets/config.json
 poetry run source-google-search-console read --config secrets/config.json --catalog integration_tests/configured_catalog.json
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
 airbyte-ci connectors --name=source-google-search-console build
 ```
 
 An image will be available on your host with the tag `airbyte/source-google-search-console:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-google-search-console:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-google-search-console:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-google-search-console:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-google-search-console:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-google-search-console test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-google-search-console test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/google-search-console.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

