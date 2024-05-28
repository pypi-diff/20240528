# Comparing `tmp/stac_asset-0.3.2.tar.gz` & `tmp/stac_asset-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_asset-0.3.2.tar", last modified: Mon May 20 12:30:56 2024, max compression
+gzip compressed data, was "stac_asset-0.3.3.tar", last modified: Tue May 28 15:22:39 2024, max compression
```

## Comparing `stac_asset-0.3.2.tar` & `stac_asset-0.3.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:30:56.833710 stac_asset-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 12:30:53.000000 stac_asset-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 12:30:53.000000 stac_asset-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-20 12:30:53.000000 stac_asset-0.3.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-20 12:30:56.833710 stac_asset-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-20 12:30:53.000000 stac_asset-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-20 12:30:53.000000 stac_asset-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:30:56.833710 stac_asset-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:30:56.825710 stac_asset-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:30:56.829710 stac_asset-0.3.2/src/stac_asset/
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    19461 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-20 12:30:53.000000 stac_asset-0.3.2/src/stac_asset/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:30:56.833710 stac_asset-0.3.2/src/stac_asset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-20 12:30:56.000000 stac_asset-0.3.2/src/stac_asset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-20 12:30:56.000000 stac_asset-0.3.2/src/stac_asset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:30:56.000000 stac_asset-0.3.2/src/stac_asset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 12:30:56.000000 stac_asset-0.3.2/src/stac_asset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-20 12:30:56.000000 stac_asset-0.3.2/src/stac_asset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 12:30:56.000000 stac_asset-0.3.2/src/stac_asset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:30:56.833710 stac_asset-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_earthdata_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_filesystem_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_planetary_computer_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-20 12:30:53.000000 stac_asset-0.3.2/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:22:39.273218 stac_asset-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 15:22:35.000000 stac_asset-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 15:22:35.000000 stac_asset-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-28 15:22:35.000000 stac_asset-0.3.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-28 15:22:39.273218 stac_asset-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-28 15:22:35.000000 stac_asset-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-28 15:22:35.000000 stac_asset-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:22:39.273218 stac_asset-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:22:39.265218 stac_asset-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:22:39.269218 stac_asset-0.3.3/src/stac_asset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20077 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-28 15:22:35.000000 stac_asset-0.3.3/src/stac_asset/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:22:39.269218 stac_asset-0.3.3/src/stac_asset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-28 15:22:39.000000 stac_asset-0.3.3/src/stac_asset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-28 15:22:39.000000 stac_asset-0.3.3/src/stac_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:22:39.000000 stac_asset-0.3.3/src/stac_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 15:22:39.000000 stac_asset-0.3.3/src/stac_asset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-28 15:22:39.000000 stac_asset-0.3.3/src/stac_asset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 15:22:39.000000 stac_asset-0.3.3/src/stac_asset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:22:39.269218 stac_asset-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-28 15:22:35.000000 stac_asset-0.3.3/tests/test_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-28 15:22:35.000000 stac_asset-0.3.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-28 15:22:35.000000 stac_asset-0.3.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-28 15:22:35.000000 stac_asset-0.3.3/tests/test_earthdata_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-28 15:22:35.000000 stac_asset-0.3.3/tests/test_filesystem_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-05-28 15:22:35.000000 stac_asset-0.3.3/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 15:22:35.000000 stac_asset-0.3.3/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-28 15:22:35.000000 stac_asset-0.3.3/tests/test_planetary_computer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-28 15:22:35.000000 stac_asset-0.3.3/tests/test_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-28 15:22:35.000000 stac_asset-0.3.3/tests/test_validate.py
```

### Comparing `stac_asset-0.3.2/LICENSE` & `stac_asset-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/NOTICE` & `stac_asset-0.3.3/NOTICE`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/PKG-INFO` & `stac_asset-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.3.2
+Version: 0.3.3
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Github, https://github.com/stac-utils/stac-asset
 Project-URL: CHANGELOG, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/stac-utils/stac-asset/issues
 Keywords: stac,async
@@ -34,15 +34,15 @@
 Requires-Dist: mypy~=1.3; extra == "dev"
 Requires-Dist: pre-commit~=3.3; extra == "dev"
 Requires-Dist: pystac[validation]>=1.8.4; extra == "dev"
 Requires-Dist: pytest~=8.2; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.21; extra == "dev"
 Requires-Dist: pytest-cov>=5.0; extra == "dev"
 Requires-Dist: pytest-recording~=0.13.1; extra == "dev"
-Requires-Dist: ruff==0.4.4; extra == "dev"
+Requires-Dist: ruff==0.4.5; extra == "dev"
 Requires-Dist: types-aiofiles~=23.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9; extra == "dev"
 Requires-Dist: types-tqdm~=4.66.0; extra == "dev"
 Requires-Dist: types-tabulate~=0.9.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
 Requires-Dist: sphinx~=7.3; extra == "docs"
```

### Comparing `stac_asset-0.3.2/README.md` & `stac_asset-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/pyproject.toml` & `stac_asset-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stac-asset"
-version = "0.3.2"
+version = "0.3.3"
 description = "Read and download STAC assets across platforms and providers"
 authors = [{ name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }]
 readme = "README.md"
 keywords = ["stac", "async"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
@@ -36,15 +36,15 @@
     "mypy~=1.3",
     "pre-commit~=3.3",
     "pystac[validation]>=1.8.4",
     "pytest~=8.2",
     "pytest-asyncio~=0.21",
     "pytest-cov>=5.0",
     "pytest-recording~=0.13.1",
-    "ruff==0.4.4",
+    "ruff==0.4.5",
     "types-aiofiles~=23.1",
     "types-python-dateutil~=2.9",
     "types-tqdm~=4.66.0",
     "types-tabulate~=0.9.0",
 ]
 docs = ["pydata-sphinx-theme~=0.13", "sphinx~=7.3", "sphinx-click~=6.0"]
```

### Comparing `stac_asset-0.3.2/src/stac_asset/__init__.py` & `stac_asset-0.3.3/src/stac_asset/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """
 
 from ._functions import (
     assert_asset_exists,
     asset_exists,
     download_asset,
     download_collection,
+    download_file,
     download_item,
     download_item_collection,
     open_href,
     read_href,
 )
 from .client import Client
 from .config import Config
@@ -59,10 +60,11 @@
     "S3Client",
     "assert_asset_exists",
     "asset_exists",
     "download_asset",
     "download_collection",
     "download_item",
     "download_item_collection",
+    "download_file",
     "open_href",
     "read_href",
 ]
```

### Comparing `stac_asset-0.3.2/src/stac_asset/_cli.py` & `stac_asset-0.3.3/src/stac_asset/_cli.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/src/stac_asset/_functions.py` & `stac_asset-0.3.3/src/stac_asset/_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -580,7 +580,28 @@
                     )
                 except KeyError:
                     raise ValueError(
                         "invalid alternate asset definition (missing href): "
                         f"{alternate}"
                     )
     return asset.get_absolute_href()
+
+
+async def download_file(
+    href: str,
+    destination: PathLikeObject,
+    config: Optional[Config] = None,
+    clients: Optional[List[Client]] = None,
+) -> None:
+    """Downloads a file collection to the local filesystem.
+
+    Args:
+        href: The source href
+        destination: The destination file path
+        config: The download configuration
+        clients: Pre-configured clients to use for access
+    """
+    if config is None:
+        config = Config()
+    clients_ = Clients(config, clients=clients)
+    client = await clients_.get_client(href)
+    await client.download_href(href, destination)
```

### Comparing `stac_asset-0.3.2/src/stac_asset/blocking.py` & `stac_asset-0.3.3/src/stac_asset/blocking.py`

 * *Files 6% similar despite different names*

```diff
@@ -231,7 +231,24 @@
         config: The download configuration to use
         clients: Any pre-configured clients to use
 
     Returns:
         bytes: The bytes from the href
     """
     return asyncio.run(_functions.read_href(href, config, clients))
+
+
+def download_file(
+    href: str,
+    destination: PathLikeObject,
+    config: Optional[Config] = None,
+    clients: Optional[List[Client]] = None,
+) -> None:
+    """Downloads a file collection to the local filesystem.
+
+    Args:
+        href: The source href
+        destination: The destination file path
+        config: The download configuration
+        clients: Pre-configured clients to use for access
+    """
+    return asyncio.run(_functions.download_file(href, destination, config, clients))
```

### Comparing `stac_asset-0.3.2/src/stac_asset/client.py` & `stac_asset-0.3.3/src/stac_asset/client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/src/stac_asset/config.py` & `stac_asset-0.3.3/src/stac_asset/config.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/src/stac_asset/earthdata_client.py` & `stac_asset-0.3.3/src/stac_asset/earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/src/stac_asset/errors.py` & `stac_asset-0.3.3/src/stac_asset/errors.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/src/stac_asset/filesystem_client.py` & `stac_asset-0.3.3/src/stac_asset/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/src/stac_asset/http_client.py` & `stac_asset-0.3.3/src/stac_asset/http_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/src/stac_asset/messages.py` & `stac_asset-0.3.3/src/stac_asset/messages.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/src/stac_asset/planetary_computer_client.py` & `stac_asset-0.3.3/src/stac_asset/planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/src/stac_asset/s3_client.py` & `stac_asset-0.3.3/src/stac_asset/s3_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/src/stac_asset/strategy.py` & `stac_asset-0.3.3/src/stac_asset/strategy.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/src/stac_asset/types.py` & `stac_asset-0.3.3/src/stac_asset/types.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/src/stac_asset/validate.py` & `stac_asset-0.3.3/src/stac_asset/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .errors import ContentTypeError
 
 ALLOWABLE_PAIRS = [
-    ("image/tiff", "image/tiff; application=geotiff; profile=cloud-optimized")
+    ("image/tiff", "image/tiff; application=geotiff; profile=cloud-optimized"),
+    ("text/xml", "application/xml"),
 ]
 IGNORED_CONTENT_TYPES = ["binary/octet-stream", "application/octet-stream"]
 
 
 def content_type(actual: str, expected: str) -> None:
     """Validates that the actual content type matches the expected.
```

### Comparing `stac_asset-0.3.2/src/stac_asset.egg-info/PKG-INFO` & `stac_asset-0.3.3/src/stac_asset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-asset
-Version: 0.3.2
+Version: 0.3.3
 Summary: Read and download STAC assets across platforms and providers
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Github, https://github.com/stac-utils/stac-asset
 Project-URL: CHANGELOG, https://github.com/stac-utils/stac-asset/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/stac-utils/stac-asset/issues
 Keywords: stac,async
@@ -34,15 +34,15 @@
 Requires-Dist: mypy~=1.3; extra == "dev"
 Requires-Dist: pre-commit~=3.3; extra == "dev"
 Requires-Dist: pystac[validation]>=1.8.4; extra == "dev"
 Requires-Dist: pytest~=8.2; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.21; extra == "dev"
 Requires-Dist: pytest-cov>=5.0; extra == "dev"
 Requires-Dist: pytest-recording~=0.13.1; extra == "dev"
-Requires-Dist: ruff==0.4.4; extra == "dev"
+Requires-Dist: ruff==0.4.5; extra == "dev"
 Requires-Dist: types-aiofiles~=23.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9; extra == "dev"
 Requires-Dist: types-tqdm~=4.66.0; extra == "dev"
 Requires-Dist: types-tabulate~=0.9.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
 Requires-Dist: sphinx~=7.3; extra == "docs"
```

### Comparing `stac_asset-0.3.2/src/stac_asset.egg-info/SOURCES.txt` & `stac_asset-0.3.3/src/stac_asset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/tests/test_blocking.py` & `stac_asset-0.3.3/tests/test_blocking.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,7 +40,14 @@
 def test_asset_exists(item: Item) -> None:
     assert stac_asset.blocking.asset_exists(item.assets["data"])
 
 
 def test_read_href(data_path: Path) -> None:
     text = stac_asset.blocking.read_href(str(data_path / "item.json"))
     Item.from_dict(json.loads(text))
+
+
+def test_download_file(data_path: Path, tmp_path: Path) -> None:
+    stac_asset.blocking.download_file(
+        str(data_path / "item.json"), tmp_path / "item.json"
+    )
+    Item.from_file(tmp_path / "item.json")
```

### Comparing `stac_asset-0.3.2/tests/test_cli.py` & `stac_asset-0.3.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/tests/test_earthdata_client.py` & `stac_asset-0.3.3/tests/test_earthdata_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/tests/test_filesystem_client.py` & `stac_asset-0.3.3/tests/test_filesystem_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/tests/test_functions.py` & `stac_asset-0.3.3/tests/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,7 +237,12 @@
 
 async def test_keep_non_downloaded(item: Item, tmp_path: Path) -> None:
     item.assets["other-data"] = item.assets["data"].clone()
     item = await stac_asset.download_item(
         item, tmp_path, config=Config(include=["data"]), keep_non_downloaded=True
     )
     assert len(item.assets) == 2
+
+
+async def test_download_file(data_path: Path, tmp_path: Path) -> None:
+    await stac_asset.download_file(str(data_path / "item.json"), tmp_path / "item.json")
+    Item.from_file(tmp_path / "item.json")
```

### Comparing `stac_asset-0.3.2/tests/test_planetary_computer_client.py` & `stac_asset-0.3.3/tests/test_planetary_computer_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/tests/test_s3_client.py` & `stac_asset-0.3.3/tests/test_s3_client.py`

 * *Files identical despite different names*

### Comparing `stac_asset-0.3.2/tests/test_validate.py` & `stac_asset-0.3.3/tests/test_validate.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,9 +8,11 @@
         validate.content_type("foo", "bar")
     validate.content_type(
         "image/tiff", "image/tiff; application=geotiff; profile=cloud-optimized"
     )
     validate.content_type(
         "image/tiff; application=geotiff; profile=cloud-optimized", "image/tiff"
     )
+    validate.content_type("text/xml", "application/xml")
+    validate.content_type("application/xml", "text/xml")
     validate.content_type("binary/octet-stream", "doesn't matter")
     validate.content_type("application/octet-stream", "doesn't matter")
```

