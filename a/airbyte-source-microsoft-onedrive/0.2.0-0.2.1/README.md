# Comparing `tmp/airbyte_source_microsoft_onedrive-0.2.0.tar.gz` & `tmp/airbyte_source_microsoft_onedrive-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_microsoft_onedrive-0.2.0.tar", max compression
+gzip compressed data, was "airbyte_source_microsoft_onedrive-0.2.1.tar", max compression
```

## Comparing `airbyte_source_microsoft_onedrive-0.2.0.tar` & `airbyte_source_microsoft_onedrive-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4712 2024-03-25 16:49:07.320396 airbyte_source_microsoft_onedrive-0.2.0/README.md
--rw-r--r--   0        0        0      985 2024-03-25 16:52:38.878570 airbyte_source_microsoft_onedrive-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      146 2024-03-25 16:49:07.324396 airbyte_source_microsoft_onedrive-0.2.0/source_microsoft_onedrive/__init__.py
--rw-r--r--   0        0        0      747 2024-03-25 16:49:07.324396 airbyte_source_microsoft_onedrive-0.2.0/source_microsoft_onedrive/run.py
--rw-r--r--   0        0        0     3195 2024-03-25 16:49:07.324396 airbyte_source_microsoft_onedrive-0.2.0/source_microsoft_onedrive/source.py
--rw-r--r--   0        0        0     5295 2024-03-25 16:49:07.324396 airbyte_source_microsoft_onedrive-0.2.0/source_microsoft_onedrive/spec.py
--rw-r--r--   0        0        0    12100 2024-03-25 16:49:07.324396 airbyte_source_microsoft_onedrive-0.2.0/source_microsoft_onedrive/stream_reader.py
--rw-r--r--   0        0        0     5622 1970-01-01 00:00:00.000000 airbyte_source_microsoft_onedrive-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4722 2024-05-28 13:00:52.089541 airbyte_source_microsoft_onedrive-0.2.1/README.md
+-rw-r--r--   0        0        0      985 2024-05-28 13:05:41.003151 airbyte_source_microsoft_onedrive-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      146 2024-05-28 13:00:52.089541 airbyte_source_microsoft_onedrive-0.2.1/source_microsoft_onedrive/__init__.py
+-rw-r--r--   0        0        0      713 2024-05-28 13:00:52.089541 airbyte_source_microsoft_onedrive-0.2.1/source_microsoft_onedrive/run.py
+-rw-r--r--   0        0        0     3152 2024-05-28 13:00:52.089541 airbyte_source_microsoft_onedrive-0.2.1/source_microsoft_onedrive/source.py
+-rw-r--r--   0        0        0     5295 2024-05-28 13:00:52.089541 airbyte_source_microsoft_onedrive-0.2.1/source_microsoft_onedrive/spec.py
+-rw-r--r--   0        0        0    12078 2024-05-28 13:00:52.089541 airbyte_source_microsoft_onedrive-0.2.1/source_microsoft_onedrive/stream_reader.py
+-rw-r--r--   0        0        0     5632 1970-01-01 00:00:00.000000 airbyte_source_microsoft_onedrive-0.2.1/PKG-INFO
```

### Comparing `airbyte_source_microsoft_onedrive-0.2.0/README.md` & `airbyte_source_microsoft_onedrive-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Microsoft OneDrive source connector
 
-
 This is the repository for the Microsoft OneDrive source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/microsoft-onedrive).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/microsoft-onedrive)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_microsoft_onedrive/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-microsoft-onedrive spec
 poetry run source-microsoft-onedrive check --config secrets/config.json
 poetry run source-microsoft-onedrive discover --config secrets/config.json
 poetry run source-microsoft-onedrive read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-microsoft-onedrive build
 ```
 
 An image will be available on your host with the tag `airbyte/source-microsoft-onedrive:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-microsoft-onedrive:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-microsoft-onedrive:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-microsoft-onedrive:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-microsoft-onedrive:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-microsoft-onedrive test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-microsoft-onedrive test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/microsoft-onedrive.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_microsoft_onedrive-0.2.0/pyproject.toml` & `airbyte_source_microsoft_onedrive-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.0"
+version = "0.2.1"
 name = "airbyte-source-microsoft-onedrive"
 description = "Source implementation for Microsoft OneDrive."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -27,15 +27,15 @@
 msal = "==1.25.0"
 transformers = "4.38.2"
 
 [tool.poetry.dependencies.airbyte-cdk]
 extras = [
     "file-based",
 ]
-version = "^0"
+version = "^1"
 
 [tool.poetry.scripts]
 source-microsoft-onedrive = "source_microsoft_onedrive.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.11.0"
 pytest = "^6.1"
```

### Comparing `airbyte_source_microsoft_onedrive-0.2.0/source_microsoft_onedrive/run.py` & `airbyte_source_microsoft_onedrive-0.2.1/source_microsoft_onedrive/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 import sys
 
-from airbyte_cdk import AirbyteEntrypoint
-from airbyte_cdk.entrypoint import launch
+from airbyte_cdk import AirbyteEntrypoint, launch
 from source_microsoft_onedrive import SourceMicrosoftOneDrive
 
 
 def run():
     args = sys.argv[1:]
     catalog_path = AirbyteEntrypoint.extract_catalog(args)
     config_path = AirbyteEntrypoint.extract_config(args)
```

### Comparing `airbyte_source_microsoft_onedrive-0.2.0/source_microsoft_onedrive/source.py` & `airbyte_source_microsoft_onedrive-0.2.1/source_microsoft_onedrive/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
+
+
 from typing import Any, Mapping, Optional
 
-from airbyte_cdk.models import AdvancedAuth, ConfiguredAirbyteCatalog, ConnectorSpecification, OAuthConfigSpecification
+from airbyte_cdk import AdvancedAuth, ConfiguredAirbyteCatalog, ConnectorSpecification, OAuthConfigSpecification, TState
 from airbyte_cdk.sources.file_based.file_based_source import FileBasedSource
 from airbyte_cdk.sources.file_based.stream.cursor.default_file_based_cursor import DefaultFileBasedCursor
-from airbyte_cdk.sources.source import TState
 from source_microsoft_onedrive.spec import SourceMicrosoftOneDriveSpec
 from source_microsoft_onedrive.stream_reader import SourceMicrosoftOneDriveStreamReader
 
 
 class SourceMicrosoftOneDrive(FileBasedSource):
     def __init__(self, catalog: Optional[ConfiguredAirbyteCatalog], config: Optional[Mapping[str, Any]], state: Optional[TState]):
         super().__init__(
```

### Comparing `airbyte_source_microsoft_onedrive-0.2.0/source_microsoft_onedrive/spec.py` & `airbyte_source_microsoft_onedrive-0.2.1/source_microsoft_onedrive/spec.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_microsoft_onedrive-0.2.0/source_microsoft_onedrive/stream_reader.py` & `airbyte_source_microsoft_onedrive-0.2.1/source_microsoft_onedrive/stream_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
+
 import logging
 from datetime import datetime
 from functools import lru_cache
 from io import IOBase
 from typing import Iterable, List, Optional, Tuple
 
 import requests
 import smart_open
+from airbyte_cdk import AirbyteTracedException, FailureType
 from airbyte_cdk.sources.file_based.file_based_stream_reader import AbstractFileBasedStreamReader, FileReadMode
 from airbyte_cdk.sources.file_based.remote_file import RemoteFile
-from airbyte_cdk.utils.traced_exception import AirbyteTracedException, FailureType
 from msal import ConfidentialClientApplication
 from msal.exceptions import MsalServiceError
 from office365.graph_client import GraphClient
 from source_microsoft_onedrive.spec import SourceMicrosoftOneDriveSpec
 
 
 class MicrosoftOneDriveRemoteFile(RemoteFile):
```

### Comparing `airbyte_source_microsoft_onedrive-0.2.0/PKG-INFO` & `airbyte_source_microsoft_onedrive-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,114 +1,128 @@
 Metadata-Version: 2.1
 Name: airbyte-source-microsoft-onedrive
-Version: 0.2.0
+Version: 0.2.1
 Summary: Source implementation for Microsoft OneDrive.
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
 Requires-Dist: Office365-REST-Python-Client (==2.5.5)
-Requires-Dist: airbyte-cdk[file-based] (>=0,<1)
+Requires-Dist: airbyte-cdk[file-based] (>=1,<2)
 Requires-Dist: msal (==1.25.0)
 Requires-Dist: smart-open (==6.4.0)
 Requires-Dist: transformers (==4.38.2)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/microsoft-onedrive
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Microsoft OneDrive source connector
 
-
 This is the repository for the Microsoft OneDrive source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/microsoft-onedrive).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/microsoft-onedrive)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_microsoft_onedrive/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-microsoft-onedrive spec
 poetry run source-microsoft-onedrive check --config secrets/config.json
 poetry run source-microsoft-onedrive discover --config secrets/config.json
 poetry run source-microsoft-onedrive read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-microsoft-onedrive build
 ```
 
 An image will be available on your host with the tag `airbyte/source-microsoft-onedrive:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-microsoft-onedrive:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-microsoft-onedrive:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-microsoft-onedrive:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-microsoft-onedrive:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-microsoft-onedrive test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-microsoft-onedrive test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/microsoft-onedrive.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

