# Comparing `tmp/google-shopping-merchant-conversions-0.1.0.tar.gz` & `tmp/google-shopping-merchant-conversions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-shopping-merchant-conversions-0.1.0.tar", last modified: Thu Apr 18 14:31:41 2024, max compression
+gzip compressed data, was "google-shopping-merchant-conversions-0.1.1.tar", last modified: Tue May 28 08:24:05 2024, max compression
```

## Comparing `google-shopping-merchant-conversions-0.1.0.tar` & `google-shopping-merchant-conversions-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.120770 google-shopping-merchant-conversions-0.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5230 2024-04-18 14:31:41.120770 google-shopping-merchant-conversions-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3818 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.108770 google-shopping-merchant-conversions-0.1.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.108770 google-shopping-merchant-conversions-0.1.0/google/shopping/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.112770 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions/
--rw-rw-r--   0 root         (0)     1003     1910 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       97 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.112770 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/
--rw-rw-r--   0 root         (0)     1003     1715 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     3262 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       97 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.112770 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.112770 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/
--rw-rw-r--   0 root         (0)     1003      809 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    39583 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    57015 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/client.py
--rw-rw-r--   0 root         (0)     1003     6313 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.116770 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/
--rw-rw-r--   0 root         (0)     1003     1561 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8925 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18847 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19186 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    39272 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.116770 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     1364 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16002 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/types/conversionsources.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.116770 google-shopping-merchant-conversions-0.1.0/google_shopping_merchant_conversions.egg-info/
--rw-r--r--   0 root         (0)     1003     5230 2024-04-18 14:31:41.000000 google-shopping-merchant-conversions-0.1.0/google_shopping_merchant_conversions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2060 2024-04-18 14:31:41.000000 google-shopping-merchant-conversions-0.1.0/google_shopping_merchant_conversions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-18 14:31:41.000000 google-shopping-merchant-conversions-0.1.0/google_shopping_merchant_conversions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-18 14:31:41.000000 google-shopping-merchant-conversions-0.1.0/google_shopping_merchant_conversions.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-04-18 14:31:41.000000 google-shopping-merchant-conversions-0.1.0/google_shopping_merchant_conversions.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-18 14:31:41.000000 google-shopping-merchant-conversions-0.1.0/google_shopping_merchant_conversions.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-04-18 14:31:41.120770 google-shopping-merchant-conversions-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3233 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.116770 google-shopping-merchant-conversions-0.1.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.116770 google-shopping-merchant-conversions-0.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.116770 google-shopping-merchant-conversions-0.1.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-18 14:31:41.120770 google-shopping-merchant-conversions-0.1.0/tests/unit/gapic/merchant_conversions_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/tests/unit/gapic/merchant_conversions_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   220867 2024-04-18 14:28:19.000000 google-shopping-merchant-conversions-0.1.0/tests/unit/gapic/merchant_conversions_v1beta/test_conversion_sources_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.947928 google-shopping-merchant-conversions-0.1.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5230 2024-05-28 08:24:05.947928 google-shopping-merchant-conversions-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3818 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.935926 google-shopping-merchant-conversions-0.1.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.935926 google-shopping-merchant-conversions-0.1.1/google/shopping/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.939926 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions/
+-rw-rw-r--   0 root         (0)     1003     1910 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       97 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.939926 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/
+-rw-rw-r--   0 root         (0)     1003     1715 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3262 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       97 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.943927 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.943927 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/
+-rw-rw-r--   0 root         (0)     1003      809 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41054 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    57278 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6313 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.943927 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1561 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8925 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19394 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21267 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    39272 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.943927 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     1364 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16012 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/types/conversionsources.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.947928 google-shopping-merchant-conversions-0.1.1/google_shopping_merchant_conversions.egg-info/
+-rw-r--r--   0 root         (0)     1003     5230 2024-05-28 08:24:05.000000 google-shopping-merchant-conversions-0.1.1/google_shopping_merchant_conversions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2060 2024-05-28 08:24:05.000000 google-shopping-merchant-conversions-0.1.1/google_shopping_merchant_conversions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-28 08:24:05.000000 google-shopping-merchant-conversions-0.1.1/google_shopping_merchant_conversions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-28 08:24:05.000000 google-shopping-merchant-conversions-0.1.1/google_shopping_merchant_conversions.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-05-28 08:24:05.000000 google-shopping-merchant-conversions-0.1.1/google_shopping_merchant_conversions.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-28 08:24:05.000000 google-shopping-merchant-conversions-0.1.1/google_shopping_merchant_conversions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-28 08:24:05.947928 google-shopping-merchant-conversions-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3233 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.947928 google-shopping-merchant-conversions-0.1.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.947928 google-shopping-merchant-conversions-0.1.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.947928 google-shopping-merchant-conversions-0.1.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:05.947928 google-shopping-merchant-conversions-0.1.1/tests/unit/gapic/merchant_conversions_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/tests/unit/gapic/merchant_conversions_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   249385 2024-05-28 08:20:21.000000 google-shopping-merchant-conversions-0.1.1/tests/unit/gapic/merchant_conversions_v1beta/test_conversion_sources_service.py
```

### Comparing `google-shopping-merchant-conversions-0.1.0/LICENSE` & `google-shopping-merchant-conversions-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/MANIFEST.in` & `google-shopping-merchant-conversions-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/PKG-INFO` & `google-shopping-merchant-conversions-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-merchant-conversions
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Shopping Merchant Conversions API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-conversions
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-merchant-conversions-0.1.0/README.rst` & `google-shopping-merchant-conversions-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions/__init__.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions/gapic_version.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/__init__.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/gapic_metadata.json` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/gapic_version.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/__init__.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/__init__.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/async_client.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
@@ -208,29 +209,37 @@
         type(ConversionSourcesServiceClient),
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, ConversionSourcesServiceTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[
+                str,
+                ConversionSourcesServiceTransport,
+                Callable[..., ConversionSourcesServiceTransport],
+            ]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the conversion sources service async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.ConversionSourcesServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,ConversionSourcesServiceTransport,Callable[..., ConversionSourcesServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the ConversionSourcesServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -346,39 +355,40 @@
                 Represents a conversion source owned
                 by a Merchant account. A merchant
                 account can have up to 200 conversion
                 sources.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, conversion_source])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = conversionsources.CreateConversionSourceRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, conversionsources.CreateConversionSourceRequest):
+            request = conversionsources.CreateConversionSourceRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if conversion_source is not None:
             request.conversion_source = conversion_source
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_conversion_source,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_conversion_source
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -471,39 +481,40 @@
                 Represents a conversion source owned
                 by a Merchant account. A merchant
                 account can have up to 200 conversion
                 sources.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([conversion_source, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = conversionsources.UpdateConversionSourceRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, conversionsources.UpdateConversionSourceRequest):
+            request = conversionsources.UpdateConversionSourceRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if conversion_source is not None:
             request.conversion_source = conversion_source
         if update_mask is not None:
             request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_conversion_source,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_conversion_source
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("conversion_source.name", request.conversion_source.name),)
             ),
@@ -578,37 +589,38 @@
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = conversionsources.DeleteConversionSourceRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, conversionsources.DeleteConversionSourceRequest):
+            request = conversionsources.DeleteConversionSourceRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_conversion_source,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_conversion_source
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -678,23 +690,24 @@
                 Represents a conversion source owned
                 by a Merchant account. A merchant
                 account can have up to 200 conversion
                 sources.
 
         """
         # Create or coerce a protobuf request object.
-        request = conversionsources.UndeleteConversionSourceRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, conversionsources.UndeleteConversionSourceRequest):
+            request = conversionsources.UndeleteConversionSourceRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.undelete_conversion_source,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.undelete_conversion_source
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -774,37 +787,38 @@
                 Represents a conversion source owned
                 by a Merchant account. A merchant
                 account can have up to 200 conversion
                 sources.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = conversionsources.GetConversionSourceRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, conversionsources.GetConversionSourceRequest):
+            request = conversionsources.GetConversionSourceRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_conversion_source,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_conversion_source
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -887,37 +901,38 @@
                 ListConversionSources method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = conversionsources.ListConversionSourcesRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, conversionsources.ListConversionSourcesRequest):
+            request = conversionsources.ListConversionSourcesRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_conversion_sources,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_conversion_sources
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
```

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/client.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
@@ -532,29 +533,37 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, ConversionSourcesServiceTransport]] = None,
+        transport: Optional[
+            Union[
+                str,
+                ConversionSourcesServiceTransport,
+                Callable[..., ConversionSourcesServiceTransport],
+            ]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the conversion sources service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ConversionSourcesServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,ConversionSourcesServiceTransport,Callable[..., ConversionSourcesServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the ConversionSourcesServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -657,16 +666,24 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[ConversionSourcesServiceTransport],
+                Callable[..., ConversionSourcesServiceTransport],
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., ConversionSourcesServiceTransport], transport)
+            )
+            # initialize with the provided callable or the passed in class
+            self._transport = transport_init(
                 credentials=credentials,
                 credentials_file=self._client_options.credentials_file,
                 host=self._api_endpoint,
                 scopes=self._client_options.scopes,
                 client_cert_source_for_mtls=self._client_cert_source,
                 quota_project_id=self._client_options.quota_project_id,
                 client_info=client_info,
@@ -750,27 +767,25 @@
                 Represents a conversion source owned
                 by a Merchant account. A merchant
                 account can have up to 200 conversion
                 sources.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, conversion_source])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a conversionsources.CreateConversionSourceRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, conversionsources.CreateConversionSourceRequest):
             request = conversionsources.CreateConversionSourceRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
             if conversion_source is not None:
@@ -875,27 +890,25 @@
                 Represents a conversion source owned
                 by a Merchant account. A merchant
                 account can have up to 200 conversion
                 sources.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([conversion_source, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a conversionsources.UpdateConversionSourceRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, conversionsources.UpdateConversionSourceRequest):
             request = conversionsources.UpdateConversionSourceRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if conversion_source is not None:
                 request.conversion_source = conversion_source
             if update_mask is not None:
@@ -982,27 +995,25 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a conversionsources.DeleteConversionSourceRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, conversionsources.DeleteConversionSourceRequest):
             request = conversionsources.DeleteConversionSourceRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1082,18 +1093,16 @@
                 Represents a conversion source owned
                 by a Merchant account. A merchant
                 account can have up to 200 conversion
                 sources.
 
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a conversionsources.UndeleteConversionSourceRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, conversionsources.UndeleteConversionSourceRequest):
             request = conversionsources.UndeleteConversionSourceRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[
             self._transport.undelete_conversion_source
@@ -1181,27 +1190,25 @@
                 Represents a conversion source owned
                 by a Merchant account. A merchant
                 account can have up to 200 conversion
                 sources.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a conversionsources.GetConversionSourceRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, conversionsources.GetConversionSourceRequest):
             request = conversionsources.GetConversionSourceRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1294,27 +1301,25 @@
                 ListConversionSources method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a conversionsources.ListConversionSourcesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, conversionsources.ListConversionSourcesRequest):
             request = conversionsources.ListConversionSourcesRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
```

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/pagers.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/__init__.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/base.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/grpc.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def __init__(
         self,
         *,
         host: str = "merchantapi.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[grpc.Channel] = None,
+        channel: Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -67,36 +67,39 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'merchantapi.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
-                which to make calls.
+                ignored if a ``channel`` instance is provided.
+            channel (Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -114,15 +117,15 @@
         self._stubs: Dict[str, Callable] = {}
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, grpc.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
 
         else:
@@ -155,15 +158,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
```

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/grpc_asyncio.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/grpc_asyncio.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
+from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, grpc_helpers_async
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.shopping.merchant_conversions_v1beta.types import conversionsources
@@ -62,15 +64,14 @@
             credentials (Optional[~.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify this application to the service. If
                 none are specified, the client will attempt to ascertain
                 the credentials from the environment.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             kwargs (Optional[dict]): Keyword arguments, which are passed to the
                 channel creation.
@@ -92,15 +93,15 @@
     def __init__(
         self,
         *,
         host: str = "merchantapi.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[aio.Channel] = None,
+        channel: Optional[Union[aio.Channel, Callable[..., aio.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -112,37 +113,40 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'merchantapi.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
-                which to make calls.
+            channel (Optional[Union[aio.Channel, Callable[..., aio.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -160,15 +164,15 @@
         self._stubs: Dict[str, Callable] = {}
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, aio.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
         else:
             if api_mtls_endpoint:
@@ -200,15 +204,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
@@ -411,12 +417,47 @@
             self._stubs["list_conversion_sources"] = self.grpc_channel.unary_unary(
                 "/google.shopping.merchant.conversions.v1beta.ConversionSourcesService/ListConversionSources",
                 request_serializer=conversionsources.ListConversionSourcesRequest.serialize,
                 response_deserializer=conversionsources.ListConversionSourcesResponse.deserialize,
             )
         return self._stubs["list_conversion_sources"]
 
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.create_conversion_source: gapic_v1.method_async.wrap_method(
+                self.create_conversion_source,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.update_conversion_source: gapic_v1.method_async.wrap_method(
+                self.update_conversion_source,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.delete_conversion_source: gapic_v1.method_async.wrap_method(
+                self.delete_conversion_source,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.undelete_conversion_source: gapic_v1.method_async.wrap_method(
+                self.undelete_conversion_source,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.get_conversion_source: gapic_v1.method_async.wrap_method(
+                self.get_conversion_source,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.list_conversion_sources: gapic_v1.method_async.wrap_method(
+                self.list_conversion_sources,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
 
 __all__ = ("ConversionSourcesServiceGrpcAsyncIOTransport",)
```

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/rest.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/services/conversion_sources_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/types/__init__.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/google/shopping/merchant_conversions_v1beta/types/conversionsources.py` & `google-shopping-merchant-conversions-0.1.1/google/shopping/merchant_conversions_v1beta/types/conversionsources.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,16 +274,17 @@
         proto.STRING,
         number=3,
     )
 
 
 class MerchantCenterDestination(proto.Message):
     r""" "Merchant Center Destination" sources can be used to send
-    conversion events from a website using a Google tag directly to
-    a Merchant Center account where the source is created.
+    conversion events from an online store using a Google tag
+    directly to a Merchant Center account where the source is
+    created.
 
     Attributes:
         destination (str):
             Output only. Merchant Center Destination ID.
         attribution_settings (google.shopping.merchant_conversions_v1beta.types.AttributionSettings):
             Required. Attribution settings being used for
             the Merchant Center Destination.
```

### Comparing `google-shopping-merchant-conversions-0.1.0/google_shopping_merchant_conversions.egg-info/PKG-INFO` & `google-shopping-merchant-conversions-0.1.1/google_shopping_merchant_conversions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-merchant-conversions
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Shopping Merchant Conversions API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-conversions
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-merchant-conversions-0.1.0/google_shopping_merchant_conversions.egg-info/SOURCES.txt` & `google-shopping-merchant-conversions-0.1.1/google_shopping_merchant_conversions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/setup.py` & `google-shopping-merchant-conversions-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/tests/__init__.py` & `google-shopping-merchant-conversions-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/tests/unit/__init__.py` & `google-shopping-merchant-conversions-0.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/tests/unit/gapic/__init__.py` & `google-shopping-merchant-conversions-0.1.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/tests/unit/gapic/merchant_conversions_v1beta/__init__.py` & `google-shopping-merchant-conversions-0.1.1/tests/unit/gapic/merchant_conversions_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-conversions-0.1.0/tests/unit/gapic/merchant_conversions_v1beta/test_conversion_sources_service.py` & `google-shopping-merchant-conversions-0.1.1/tests/unit/gapic/merchant_conversions_v1beta/test_conversion_sources_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -1246,14 +1246,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_conversion_source), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_conversion_source()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.CreateConversionSourceRequest()
 
 
 def test_create_conversion_source_non_empty_request_with_auto_populated_field():
@@ -1271,22 +1274,65 @@
         parent="parent_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_conversion_source), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_conversion_source(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.CreateConversionSourceRequest(
             parent="parent_value",
         )
 
 
+def test_create_conversion_source_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.create_conversion_source
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_conversion_source
+        ] = mock_rpc
+        request = {}
+        client.create_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_conversion_source_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ConversionSourcesServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1307,14 +1353,60 @@
         response = await client.create_conversion_source()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.CreateConversionSourceRequest()
 
 
 @pytest.mark.asyncio
+async def test_create_conversion_source_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.create_conversion_source
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.create_conversion_source
+        ] = mock_object
+
+        request = {}
+        await client.create_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.create_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_create_conversion_source_async(
     transport: str = "grpc_asyncio",
     request_type=conversionsources.CreateConversionSourceRequest,
 ):
     client = ConversionSourcesServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1591,14 +1683,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_conversion_source), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_conversion_source()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.UpdateConversionSourceRequest()
 
 
 def test_update_conversion_source_non_empty_request_with_auto_populated_field():
@@ -1614,20 +1709,63 @@
     # if they meet the requirements of AIP 4235.
     request = conversionsources.UpdateConversionSourceRequest()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_conversion_source), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_conversion_source(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.UpdateConversionSourceRequest()
 
 
+def test_update_conversion_source_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.update_conversion_source
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_conversion_source
+        ] = mock_rpc
+        request = {}
+        client.update_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_conversion_source_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ConversionSourcesServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1648,14 +1786,60 @@
         response = await client.update_conversion_source()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.UpdateConversionSourceRequest()
 
 
 @pytest.mark.asyncio
+async def test_update_conversion_source_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.update_conversion_source
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.update_conversion_source
+        ] = mock_object
+
+        request = {}
+        await client.update_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.update_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_update_conversion_source_async(
     transport: str = "grpc_asyncio",
     request_type=conversionsources.UpdateConversionSourceRequest,
 ):
     client = ConversionSourcesServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1925,14 +2109,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_conversion_source), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_conversion_source()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.DeleteConversionSourceRequest()
 
 
 def test_delete_conversion_source_non_empty_request_with_auto_populated_field():
@@ -1950,22 +2137,65 @@
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_conversion_source), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_conversion_source(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.DeleteConversionSourceRequest(
             name="name_value",
         )
 
 
+def test_delete_conversion_source_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.delete_conversion_source
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_conversion_source
+        ] = mock_rpc
+        request = {}
+        client.delete_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_conversion_source_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ConversionSourcesServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1980,14 +2210,60 @@
         response = await client.delete_conversion_source()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.DeleteConversionSourceRequest()
 
 
 @pytest.mark.asyncio
+async def test_delete_conversion_source_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.delete_conversion_source
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.delete_conversion_source
+        ] = mock_object
+
+        request = {}
+        await client.delete_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.delete_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_delete_conversion_source_async(
     transport: str = "grpc_asyncio",
     request_type=conversionsources.DeleteConversionSourceRequest,
 ):
     client = ConversionSourcesServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2217,14 +2493,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.undelete_conversion_source), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.undelete_conversion_source()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.UndeleteConversionSourceRequest()
 
 
 def test_undelete_conversion_source_non_empty_request_with_auto_populated_field():
@@ -2242,22 +2521,65 @@
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.undelete_conversion_source), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.undelete_conversion_source(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.UndeleteConversionSourceRequest(
             name="name_value",
         )
 
 
+def test_undelete_conversion_source_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.undelete_conversion_source
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.undelete_conversion_source
+        ] = mock_rpc
+        request = {}
+        client.undelete_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.undelete_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_undelete_conversion_source_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ConversionSourcesServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2278,14 +2600,60 @@
         response = await client.undelete_conversion_source()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.UndeleteConversionSourceRequest()
 
 
 @pytest.mark.asyncio
+async def test_undelete_conversion_source_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.undelete_conversion_source
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.undelete_conversion_source
+        ] = mock_object
+
+        request = {}
+        await client.undelete_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.undelete_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_undelete_conversion_source_async(
     transport: str = "grpc_asyncio",
     request_type=conversionsources.UndeleteConversionSourceRequest,
 ):
     client = ConversionSourcesServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2442,14 +2810,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_conversion_source), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_conversion_source()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.GetConversionSourceRequest()
 
 
 def test_get_conversion_source_non_empty_request_with_auto_populated_field():
@@ -2467,22 +2838,65 @@
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_conversion_source), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_conversion_source(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.GetConversionSourceRequest(
             name="name_value",
         )
 
 
+def test_get_conversion_source_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.get_conversion_source
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_conversion_source
+        ] = mock_rpc
+        request = {}
+        client.get_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_conversion_source_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ConversionSourcesServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2503,14 +2917,60 @@
         response = await client.get_conversion_source()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.GetConversionSourceRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_conversion_source_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_conversion_source
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_conversion_source
+        ] = mock_object
+
+        request = {}
+        await client.get_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_conversion_source_async(
     transport: str = "grpc_asyncio",
     request_type=conversionsources.GetConversionSourceRequest,
 ):
     client = ConversionSourcesServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2749,14 +3209,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_conversion_sources), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_conversion_sources()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.ListConversionSourcesRequest()
 
 
 def test_list_conversion_sources_non_empty_request_with_auto_populated_field():
@@ -2775,23 +3238,66 @@
         page_token="page_token_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_conversion_sources), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_conversion_sources(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.ListConversionSourcesRequest(
             parent="parent_value",
             page_token="page_token_value",
         )
 
 
+def test_list_conversion_sources_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_conversion_sources
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_conversion_sources
+        ] = mock_rpc
+        request = {}
+        client.list_conversion_sources(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_conversion_sources(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_conversion_sources_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ConversionSourcesServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2810,14 +3316,60 @@
         response = await client.list_conversion_sources()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == conversionsources.ListConversionSourcesRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_conversion_sources_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_conversion_sources
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_conversion_sources
+        ] = mock_object
+
+        request = {}
+        await client.list_conversion_sources(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_conversion_sources(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_conversion_sources_async(
     transport: str = "grpc_asyncio",
     request_type=conversionsources.ListConversionSourcesRequest,
 ):
     client = ConversionSourcesServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -3334,14 +3886,55 @@
     # Establish that the response is the type that we expect.
     assert isinstance(response, conversionsources.ConversionSource)
     assert response.name == "name_value"
     assert response.state == conversionsources.ConversionSource.State.ACTIVE
     assert response.controller == conversionsources.ConversionSource.Controller.MERCHANT
 
 
+def test_create_conversion_source_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.create_conversion_source
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_conversion_source
+        ] = mock_rpc
+
+        request = {}
+        client.create_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_create_conversion_source_rest_required_fields(
     request_type=conversionsources.CreateConversionSourceRequest,
 ):
     transport_class = transports.ConversionSourcesServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -3719,14 +4312,55 @@
     # Establish that the response is the type that we expect.
     assert isinstance(response, conversionsources.ConversionSource)
     assert response.name == "name_value"
     assert response.state == conversionsources.ConversionSource.State.ACTIVE
     assert response.controller == conversionsources.ConversionSource.Controller.MERCHANT
 
 
+def test_update_conversion_source_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.update_conversion_source
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_conversion_source
+        ] = mock_rpc
+
+        request = {}
+        client.update_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_update_conversion_source_rest_required_fields(
     request_type=conversionsources.UpdateConversionSourceRequest,
 ):
     transport_class = transports.ConversionSourcesServiceRestTransport
 
     request_init = {}
     request = request_type(**request_init)
@@ -4004,14 +4638,55 @@
         req.return_value = response_value
         response = client.delete_conversion_source(request)
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
+def test_delete_conversion_source_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.delete_conversion_source
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_conversion_source
+        ] = mock_rpc
+
+        request = {}
+        client.delete_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_delete_conversion_source_rest_required_fields(
     request_type=conversionsources.DeleteConversionSourceRequest,
 ):
     transport_class = transports.ConversionSourcesServiceRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -4264,14 +4939,55 @@
     # Establish that the response is the type that we expect.
     assert isinstance(response, conversionsources.ConversionSource)
     assert response.name == "name_value"
     assert response.state == conversionsources.ConversionSource.State.ACTIVE
     assert response.controller == conversionsources.ConversionSource.Controller.MERCHANT
 
 
+def test_undelete_conversion_source_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.undelete_conversion_source
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.undelete_conversion_source
+        ] = mock_rpc
+
+        request = {}
+        client.undelete_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.undelete_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_undelete_conversion_source_rest_required_fields(
     request_type=conversionsources.UndeleteConversionSourceRequest,
 ):
     transport_class = transports.ConversionSourcesServiceRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -4482,14 +5198,55 @@
     # Establish that the response is the type that we expect.
     assert isinstance(response, conversionsources.ConversionSource)
     assert response.name == "name_value"
     assert response.state == conversionsources.ConversionSource.State.ACTIVE
     assert response.controller == conversionsources.ConversionSource.Controller.MERCHANT
 
 
+def test_get_conversion_source_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.get_conversion_source
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_conversion_source
+        ] = mock_rpc
+
+        request = {}
+        client.get_conversion_source(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_conversion_source(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_conversion_source_rest_required_fields(
     request_type=conversionsources.GetConversionSourceRequest,
 ):
     transport_class = transports.ConversionSourcesServiceRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -4749,14 +5506,55 @@
         response = client.list_conversion_sources(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListConversionSourcesPager)
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_conversion_sources_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ConversionSourcesServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_conversion_sources
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_conversion_sources
+        ] = mock_rpc
+
+        request = {}
+        client.list_conversion_sources(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_conversion_sources(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_conversion_sources_rest_required_fields(
     request_type=conversionsources.ListConversionSourcesRequest,
 ):
     transport_class = transports.ConversionSourcesServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
```

