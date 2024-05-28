# Comparing `tmp/google-shopping-merchant-reports-0.1.6.tar.gz` & `tmp/google-shopping-merchant-reports-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-shopping-merchant-reports-0.1.6.tar", last modified: Mon Apr 15 13:59:02 2024, max compression
+gzip compressed data, was "google-shopping-merchant-reports-0.1.7.tar", last modified: Tue May 28 08:24:19 2024, max compression
```

## Comparing `google-shopping-merchant-reports-0.1.6.tar` & `google-shopping-merchant-reports-0.1.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.436642 google-shopping-merchant-reports-0.1.6/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5310 2024-04-15 13:59:02.436642 google-shopping-merchant-reports-0.1.6/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3857 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.424641 google-shopping-merchant-reports-0.1.6/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.424641 google-shopping-merchant-reports-0.1.6/google/shopping/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.428641 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports/
--rw-rw-r--   0 root         (0)     1003     2062 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.428641 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/
--rw-rw-r--   0 root         (0)     1003     1878 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     1005 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.428641 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.428641 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/
--rw-rw-r--   0 root         (0)     1003      765 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    15830 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    31828 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/client.py
--rw-rw-r--   0 root         (0)     1003     5666 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6086 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11951 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12170 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12038 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     1600 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    84961 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/types/reports.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/
--rw-r--r--   0 root         (0)     1003     5310 2024-04-15 13:59:02.000000 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1822 2024-04-15 13:59:02.000000 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-15 13:59:02.000000 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-15 13:59:02.000000 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      343 2024-04-15 13:59:02.000000 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-15 13:59:02.000000 google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-04-15 13:59:02.436642 google-shopping-merchant-reports-0.1.6/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3265 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:59:02.432641 google-shopping-merchant-reports-0.1.6/tests/unit/gapic/merchant_reports_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/tests/unit/gapic/merchant_reports_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    96721 2024-04-15 13:54:45.000000 google-shopping-merchant-reports-0.1.6/tests/unit/gapic/merchant_reports_v1beta/test_report_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.290624 google-shopping-merchant-reports-0.1.7/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5310 2024-05-28 08:24:19.290624 google-shopping-merchant-reports-0.1.7/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3857 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.278621 google-shopping-merchant-reports-0.1.7/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.278621 google-shopping-merchant-reports-0.1.7/google/shopping/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.282622 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports/
+-rw-rw-r--   0 root         (0)     1003     2126 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.282622 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/
+-rw-rw-r--   0 root         (0)     1003     1942 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1005 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.282622 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.282622 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/
+-rw-rw-r--   0 root         (0)     1003      765 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16318 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    32463 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5666 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.286623 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6086 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12498 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13124 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12038 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.286623 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     1664 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    89017 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/types/reports.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.286623 google-shopping-merchant-reports-0.1.7/google_shopping_merchant_reports.egg-info/
+-rw-r--r--   0 root         (0)     1003     5310 2024-05-28 08:24:19.000000 google-shopping-merchant-reports-0.1.7/google_shopping_merchant_reports.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1822 2024-05-28 08:24:19.000000 google-shopping-merchant-reports-0.1.7/google_shopping_merchant_reports.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-28 08:24:19.000000 google-shopping-merchant-reports-0.1.7/google_shopping_merchant_reports.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-28 08:24:19.000000 google-shopping-merchant-reports-0.1.7/google_shopping_merchant_reports.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      343 2024-05-28 08:24:19.000000 google-shopping-merchant-reports-0.1.7/google_shopping_merchant_reports.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-28 08:24:19.000000 google-shopping-merchant-reports-0.1.7/google_shopping_merchant_reports.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-28 08:24:19.290624 google-shopping-merchant-reports-0.1.7/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3265 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.286623 google-shopping-merchant-reports-0.1.7/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.286623 google-shopping-merchant-reports-0.1.7/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.286623 google-shopping-merchant-reports-0.1.7/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:19.286623 google-shopping-merchant-reports-0.1.7/tests/unit/gapic/merchant_reports_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/tests/unit/gapic/merchant_reports_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   101053 2024-05-28 08:20:21.000000 google-shopping-merchant-reports-0.1.7/tests/unit/gapic/merchant_reports_v1beta/test_report_service.py
```

### Comparing `google-shopping-merchant-reports-0.1.6/LICENSE` & `google-shopping-merchant-reports-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/MANIFEST.in` & `google-shopping-merchant-reports-0.1.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/PKG-INFO` & `google-shopping-merchant-reports-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-merchant-reports
-Version: 0.1.6
+Version: 0.1.7
 Summary: Google Shopping Merchant Reports API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-reports
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-merchant-reports-0.1.6/README.rst` & `google-shopping-merchant-reports-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports/__init__.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from google.shopping.merchant_reports_v1beta.types.reports import (
     BestSellersBrandView,
     BestSellersProductClusterView,
     CompetitiveVisibilityBenchmarkView,
     CompetitiveVisibilityCompetitorView,
     CompetitiveVisibilityTopMerchantView,
     MarketingMethod,
+    NonProductPerformanceView,
     PriceCompetitivenessProductView,
     PriceInsightsProductView,
     ProductPerformanceView,
     ProductView,
     RelativeDemand,
     RelativeDemandChangeType,
     ReportGranularity,
@@ -49,14 +50,15 @@
     "ReportServiceAsyncClient",
     "BestSellersBrandView",
     "BestSellersProductClusterView",
     "CompetitiveVisibilityBenchmarkView",
     "CompetitiveVisibilityCompetitorView",
     "CompetitiveVisibilityTopMerchantView",
     "MarketingMethod",
+    "NonProductPerformanceView",
     "PriceCompetitivenessProductView",
     "PriceInsightsProductView",
     "ProductPerformanceView",
     "ProductView",
     "RelativeDemand",
     "RelativeDemandChangeType",
     "ReportGranularity",
```

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports/gapic_version.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.6"  # {x-release-please-version}
+__version__ = "0.1.7"  # {x-release-please-version}
```

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/__init__.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .types.reports import (
     BestSellersBrandView,
     BestSellersProductClusterView,
     CompetitiveVisibilityBenchmarkView,
     CompetitiveVisibilityCompetitorView,
     CompetitiveVisibilityTopMerchantView,
     MarketingMethod,
+    NonProductPerformanceView,
     PriceCompetitivenessProductView,
     PriceInsightsProductView,
     ProductPerformanceView,
     ProductView,
     RelativeDemand,
     RelativeDemandChangeType,
     ReportGranularity,
@@ -43,14 +44,15 @@
     "ReportServiceAsyncClient",
     "BestSellersBrandView",
     "BestSellersProductClusterView",
     "CompetitiveVisibilityBenchmarkView",
     "CompetitiveVisibilityCompetitorView",
     "CompetitiveVisibilityTopMerchantView",
     "MarketingMethod",
+    "NonProductPerformanceView",
     "PriceCompetitivenessProductView",
     "PriceInsightsProductView",
     "ProductPerformanceView",
     "ProductView",
     "RelativeDemand",
     "RelativeDemandChangeType",
     "ReportGranularity",
```

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/gapic_metadata.json` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/gapic_version.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.6"  # {x-release-please-version}
+__version__ = "0.1.7"  # {x-release-please-version}
```

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/__init__.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/__init__.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/async_client.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/async_client.py`

 * *Files 2% similar despite different names*

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
@@ -191,29 +192,33 @@
         type(ReportServiceClient).get_transport_class, type(ReportServiceClient)
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, ReportServiceTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[str, ReportServiceTransport, Callable[..., ReportServiceTransport]]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the report service async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.ReportServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,ReportServiceTransport,Callable[..., ReportServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the ReportServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -318,37 +323,36 @@
                 Response message for the ReportService.Search method.
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
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
 
-        request = reports.SearchRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, reports.SearchRequest):
+            request = reports.SearchRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.search,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[self._client._transport.search]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
```

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/client.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/client.py`

 * *Files 1% similar despite different names*

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
@@ -504,29 +505,33 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, ReportServiceTransport]] = None,
+        transport: Optional[
+            Union[str, ReportServiceTransport, Callable[..., ReportServiceTransport]]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the report service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ReportServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,ReportServiceTransport,Callable[..., ReportServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the ReportServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -627,16 +632,23 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[ReportServiceTransport], Callable[..., ReportServiceTransport]
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., ReportServiceTransport], transport)
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
@@ -709,27 +721,25 @@
                 Response message for the ReportService.Search method.
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
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
-        # in a reports.SearchRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, reports.SearchRequest):
             request = reports.SearchRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
```

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/pagers.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/__init__.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/base.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc.py`

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

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc_asyncio.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/transports/grpc_asyncio.py`

 * *Files 7% similar despite different names*

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
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.shopping.merchant_reports_v1beta.types import reports
 
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
@@ -258,12 +264,22 @@
             self._stubs["search"] = self.grpc_channel.unary_unary(
                 "/google.shopping.merchant.reports.v1beta.ReportService/Search",
                 request_serializer=reports.SearchRequest.serialize,
                 response_deserializer=reports.SearchResponse.deserialize,
             )
         return self._stubs["search"]
 
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.search: gapic_v1.method_async.wrap_method(
+                self.search,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
 
 __all__ = ("ReportServiceGrpcAsyncIOTransport",)
```

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/services/report_service/transports/rest.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/services/report_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/types/__init__.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/types/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .reports import (
     BestSellersBrandView,
     BestSellersProductClusterView,
     CompetitiveVisibilityBenchmarkView,
     CompetitiveVisibilityCompetitorView,
     CompetitiveVisibilityTopMerchantView,
     MarketingMethod,
+    NonProductPerformanceView,
     PriceCompetitivenessProductView,
     PriceInsightsProductView,
     ProductPerformanceView,
     ProductView,
     RelativeDemand,
     RelativeDemandChangeType,
     ReportGranularity,
@@ -36,14 +37,15 @@
 __all__ = (
     "BestSellersBrandView",
     "BestSellersProductClusterView",
     "CompetitiveVisibilityBenchmarkView",
     "CompetitiveVisibilityCompetitorView",
     "CompetitiveVisibilityTopMerchantView",
     "MarketingMethod",
+    "NonProductPerformanceView",
     "PriceCompetitivenessProductView",
     "PriceInsightsProductView",
     "ProductPerformanceView",
     "ProductView",
     "RelativeDemand",
     "RelativeDemandChangeType",
     "ReportGranularity",
```

### Comparing `google-shopping-merchant-reports-0.1.6/google/shopping/merchant_reports_v1beta/types/reports.py` & `google-shopping-merchant-reports-0.1.7/google/shopping/merchant_reports_v1beta/types/reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,5240 +72,5493 @@
 00000470: 6577 222c 0a20 2020 2020 2020 2022 5072  ew",.        "Pr
 00000480: 6963 6549 6e73 6967 6874 7350 726f 6475  iceInsightsProdu
 00000490: 6374 5669 6577 222c 0a20 2020 2020 2020  ctView",.       
 000004a0: 2022 4265 7374 5365 6c6c 6572 7350 726f   "BestSellersPro
 000004b0: 6475 6374 436c 7573 7465 7256 6965 7722  ductClusterView"
 000004c0: 2c0a 2020 2020 2020 2020 2242 6573 7453  ,.        "BestS
 000004d0: 656c 6c65 7273 4272 616e 6456 6965 7722  ellersBrandView"
-000004e0: 2c0a 2020 2020 2020 2020 2243 6f6d 7065  ,.        "Compe
-000004f0: 7469 7469 7665 5669 7369 6269 6c69 7479  titiveVisibility
-00000500: 436f 6d70 6574 6974 6f72 5669 6577 222c  CompetitorView",
-00000510: 0a20 2020 2020 2020 2022 436f 6d70 6574  .        "Compet
-00000520: 6974 6976 6556 6973 6962 696c 6974 7954  itiveVisibilityT
-00000530: 6f70 4d65 7263 6861 6e74 5669 6577 222c  opMerchantView",
-00000540: 0a20 2020 2020 2020 2022 436f 6d70 6574  .        "Compet
-00000550: 6974 6976 6556 6973 6962 696c 6974 7942  itiveVisibilityB
-00000560: 656e 6368 6d61 726b 5669 6577 222c 0a20  enchmarkView",. 
-00000570: 2020 2020 2020 2022 4d61 726b 6574 696e         "Marketin
-00000580: 674d 6574 686f 6422 2c0a 2020 2020 2020  gMethod",.      
-00000590: 2020 2252 6570 6f72 7447 7261 6e75 6c61    "ReportGranula
-000005a0: 7269 7479 222c 0a20 2020 2020 2020 2022  rity",.        "
-000005b0: 5265 6c61 7469 7665 4465 6d61 6e64 222c  RelativeDemand",
-000005c0: 0a20 2020 2020 2020 2022 5265 6c61 7469  .        "Relati
-000005d0: 7665 4465 6d61 6e64 4368 616e 6765 5479  veDemandChangeTy
-000005e0: 7065 222c 0a20 2020 2020 2020 2022 5472  pe",.        "Tr
-000005f0: 6166 6669 6353 6f75 7263 6522 2c0a 2020  afficSource",.  
-00000600: 2020 7d2c 0a29 0a0a 0a63 6c61 7373 2053    },.)...class S
-00000610: 6561 7263 6852 6571 7565 7374 2870 726f  earchRequest(pro
-00000620: 746f 2e4d 6573 7361 6765 293a 0a20 2020  to.Message):.   
-00000630: 2072 2222 2252 6571 7565 7374 206d 6573   r"""Request mes
-00000640: 7361 6765 2066 6f72 2074 6865 2060 6052  sage for the ``R
-00000650: 6570 6f72 7453 6572 7669 6365 2e53 6561  eportService.Sea
-00000660: 7263 6860 6020 6d65 7468 6f64 2e0a 0a20  rch`` method... 
-00000670: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
-00000680: 2020 2020 2020 2070 6172 656e 7420 2873         parent (s
-00000690: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-000006a0: 2052 6571 7569 7265 642e 2049 6420 6f66   Required. Id of
-000006b0: 2074 6865 2061 6363 6f75 6e74 206d 616b   the account mak
-000006c0: 696e 6720 7468 6520 6361 6c6c 2e0a 2020  ing the call..  
-000006d0: 2020 2020 2020 2020 2020 4d75 7374 2062            Must b
-000006e0: 6520 6120 7374 616e 6461 6c6f 6e65 2061  e a standalone a
-000006f0: 6363 6f75 6e74 206f 7220 616e 204d 4341  ccount or an MCA
-00000700: 0a20 2020 2020 2020 2020 2020 2073 7562  .            sub
-00000710: 6163 636f 756e 742e 2046 6f72 6d61 743a  account. Format:
-00000720: 2061 6363 6f75 6e74 732f 7b61 6363 6f75   accounts/{accou
-00000730: 6e74 7d0a 2020 2020 2020 2020 7175 6572  nt}.        quer
-00000740: 7920 2873 7472 293a 0a20 2020 2020 2020  y (str):.       
-00000750: 2020 2020 2052 6571 7569 7265 642e 2051       Required. Q
-00000760: 7565 7279 2074 6861 7420 6465 6669 6e65  uery that define
-00000770: 7320 6120 7265 706f 7274 2074 6f20 6265  s a report to be
-00000780: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00000790: 7269 6576 6564 2e0a 2020 2020 2020 2020  rieved..        
-000007a0: 2020 2020 466f 7220 6465 7461 696c 7320      For details 
-000007b0: 6f6e 2068 6f77 2074 6f20 636f 6e73 7472  on how to constr
-000007c0: 7563 7420 796f 7572 2071 7565 7279 2c20  uct your query, 
-000007d0: 7365 650a 2020 2020 2020 2020 2020 2020  see.            
-000007e0: 7468 6520 5175 6572 7920 4c61 6e67 7561  the Query Langua
-000007f0: 6765 2067 7569 6465 2e20 466f 7220 7468  ge guide. For th
-00000800: 6520 6675 6c6c 206c 6973 7420 6f66 0a20  e full list of. 
-00000810: 2020 2020 2020 2020 2020 2061 7661 696c             avail
-00000820: 6162 6c65 2074 6162 6c65 7320 616e 6420  able tables and 
-00000830: 6669 656c 6473 2c20 7365 6520 7468 6520  fields, see the 
-00000840: 4176 6169 6c61 626c 650a 2020 2020 2020  Available.      
-00000850: 2020 2020 2020 6669 656c 6473 2e0a 2020        fields..  
-00000860: 2020 2020 2020 7061 6765 5f73 697a 6520        page_size 
-00000870: 2869 6e74 293a 0a20 2020 2020 2020 2020  (int):.         
-00000880: 2020 204f 7074 696f 6e61 6c2e 204e 756d     Optional. Num
-00000890: 6265 7220 6f66 2060 6052 6570 6f72 7452  ber of ``ReportR
-000008a0: 6f77 7360 6020 746f 2072 6574 7269 6576  ows`` to retriev
-000008b0: 6520 696e 2061 2073 696e 676c 650a 2020  e in a single.  
-000008c0: 2020 2020 2020 2020 2020 7061 6765 2e20            page. 
-000008d0: 4465 6661 756c 7473 2074 6f20 3130 3030  Defaults to 1000
-000008e0: 2e20 5661 6c75 6573 2061 626f 7665 2035  . Values above 5
-000008f0: 3030 3020 6172 6520 636f 6572 6365 6420  000 are coerced 
-00000900: 746f 0a20 2020 2020 2020 2020 2020 2035  to.            5
-00000910: 3030 302e 0a20 2020 2020 2020 2070 6167  000..        pag
-00000920: 655f 746f 6b65 6e20 2873 7472 293a 0a20  e_token (str):. 
-00000930: 2020 2020 2020 2020 2020 204f 7074 696f             Optio
-00000940: 6e61 6c2e 2054 6f6b 656e 206f 6620 7468  nal. Token of th
-00000950: 6520 7061 6765 2074 6f20 7265 7472 6965  e page to retrie
-00000960: 7665 2e20 4966 206e 6f74 2073 7065 6369  ve. If not speci
-00000970: 6669 6564 2c0a 2020 2020 2020 2020 2020  fied,.          
-00000980: 2020 7468 6520 6669 7273 7420 7061 6765    the first page
-00000990: 206f 6620 7265 7375 6c74 7320 6973 2072   of results is r
-000009a0: 6574 7572 6e65 642e 2049 6e20 6f72 6465  eturned. In orde
-000009b0: 7220 746f 2072 6571 7565 7374 0a20 2020  r to request.   
-000009c0: 2020 2020 2020 2020 2074 6865 206e 6578           the nex
-000009d0: 7420 7061 6765 206f 6620 7265 7375 6c74  t page of result
-000009e0: 732c 2074 6865 2076 616c 7565 206f 6274  s, the value obt
-000009f0: 6169 6e65 6420 6672 6f6d 0a20 2020 2020  ained from.     
-00000a00: 2020 2020 2020 2060 606e 6578 745f 7061         ``next_pa
-00000a10: 6765 5f74 6f6b 656e 6060 2069 6e20 7468  ge_token`` in th
-00000a20: 6520 7072 6576 696f 7573 2072 6573 706f  e previous respo
-00000a30: 6e73 6520 7368 6f75 6c64 2062 6520 7573  nse should be us
-00000a40: 6564 2e0a 2020 2020 2222 220a 0a20 2020  ed..    """..   
-00000a50: 2070 6172 656e 743a 2073 7472 203d 2070   parent: str = p
-00000a60: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00000a70: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
-00000a80: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-00000a90: 3d31 2c0a 2020 2020 290a 2020 2020 7175  =1,.    ).    qu
-00000aa0: 6572 793a 2073 7472 203d 2070 726f 746f  ery: str = proto
-00000ab0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00000ac0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-00000ad0: 2020 2020 2020 6e75 6d62 6572 3d32 2c0a        number=2,.
-00000ae0: 2020 2020 290a 2020 2020 7061 6765 5f73      ).    page_s
-00000af0: 697a 653a 2069 6e74 203d 2070 726f 746f  ize: int = proto
-00000b00: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00000b10: 7072 6f74 6f2e 494e 5433 322c 0a20 2020  proto.INT32,.   
-00000b20: 2020 2020 206e 756d 6265 723d 332c 0a20       number=3,. 
-00000b30: 2020 2029 0a20 2020 2070 6167 655f 746f     ).    page_to
-00000b40: 6b65 6e3a 2073 7472 203d 2070 726f 746f  ken: str = proto
-00000b50: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00000b60: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-00000b70: 2020 2020 2020 6e75 6d62 6572 3d34 2c0a        number=4,.
-00000b80: 2020 2020 290a 0a0a 636c 6173 7320 5365      )...class Se
-00000b90: 6172 6368 5265 7370 6f6e 7365 2870 726f  archResponse(pro
-00000ba0: 746f 2e4d 6573 7361 6765 293a 0a20 2020  to.Message):.   
-00000bb0: 2072 2222 2252 6573 706f 6e73 6520 6d65   r"""Response me
-00000bc0: 7373 6167 6520 666f 7220 7468 6520 6060  ssage for the ``
-00000bd0: 5265 706f 7274 5365 7276 6963 652e 5365  ReportService.Se
-00000be0: 6172 6368 6060 206d 6574 686f 642e 0a0a  arch`` method...
-00000bf0: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
-00000c00: 2020 2020 2020 2020 7265 7375 6c74 7320          results 
-00000c10: 284d 7574 6162 6c65 5365 7175 656e 6365  (MutableSequence
-00000c20: 5b67 6f6f 676c 652e 7368 6f70 7069 6e67  [google.shopping
-00000c30: 2e6d 6572 6368 616e 745f 7265 706f 7274  .merchant_report
-00000c40: 735f 7631 6265 7461 2e74 7970 6573 2e52  s_v1beta.types.R
-00000c50: 6570 6f72 7452 6f77 5d29 3a0a 2020 2020  eportRow]):.    
-00000c60: 2020 2020 2020 2020 526f 7773 2074 6861          Rows tha
-00000c70: 7420 6d61 7463 6865 6420 7468 6520 7365  t matched the se
-00000c80: 6172 6368 2071 7565 7279 2e0a 2020 2020  arch query..    
-00000c90: 2020 2020 6e65 7874 5f70 6167 655f 746f      next_page_to
-00000ca0: 6b65 6e20 2873 7472 293a 0a20 2020 2020  ken (str):.     
-00000cb0: 2020 2020 2020 2054 6f6b 656e 2077 6869         Token whi
-00000cc0: 6368 2063 616e 2062 6520 7365 6e74 2061  ch can be sent a
-00000cd0: 7320 6060 7061 6765 5f74 6f6b 656e 6060  s ``page_token``
-00000ce0: 2074 6f20 7265 7472 6965 7665 2074 6865   to retrieve the
-00000cf0: 0a20 2020 2020 2020 2020 2020 206e 6578  .            nex
-00000d00: 7420 7061 6765 2e20 4966 206f 6d69 7474  t page. If omitt
-00000d10: 6564 2c20 7468 6572 6520 6172 6520 6e6f  ed, there are no
-00000d20: 2073 7562 7365 7175 656e 7420 7061 6765   subsequent page
-00000d30: 732e 0a20 2020 2022 2222 0a0a 2020 2020  s..    """..    
-00000d40: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00000d50: 6620 7261 775f 7061 6765 2873 656c 6629  f raw_page(self)
-00000d60: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00000d70: 2073 656c 660a 0a20 2020 2072 6573 756c   self..    resul
-00000d80: 7473 3a20 4d75 7461 626c 6553 6571 7565  ts: MutableSeque
-00000d90: 6e63 655b 2252 6570 6f72 7452 6f77 225d  nce["ReportRow"]
-00000da0: 203d 2070 726f 746f 2e52 6570 6561 7465   = proto.Repeate
-00000db0: 6446 6965 6c64 280a 2020 2020 2020 2020  dField(.        
-00000dc0: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
-00000dd0: 2020 2020 2020 206e 756d 6265 723d 312c         number=1,
-00000de0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-00000df0: 3d22 5265 706f 7274 526f 7722 2c0a 2020  ="ReportRow",.  
-00000e00: 2020 290a 2020 2020 6e65 7874 5f70 6167    ).    next_pag
-00000e10: 655f 746f 6b65 6e3a 2073 7472 203d 2070  e_token: str = p
-00000e20: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00000e30: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
-00000e40: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-00000e50: 3d32 2c0a 2020 2020 290a 0a0a 636c 6173  =2,.    )...clas
-00000e60: 7320 5265 706f 7274 526f 7728 7072 6f74  s ReportRow(prot
-00000e70: 6f2e 4d65 7373 6167 6529 3a0a 2020 2020  o.Message):.    
-00000e80: 7222 2222 5265 7375 6c74 2072 6f77 2072  r"""Result row r
-00000e90: 6574 7572 6e65 6420 6672 6f6d 2074 6865  eturned from the
-00000ea0: 2073 6561 7263 6820 7175 6572 792e 0a0a   search query...
-00000eb0: 2020 2020 4f6e 6c79 2074 6865 206d 6573      Only the mes
-00000ec0: 7361 6765 2063 6f72 7265 7370 6f6e 6469  sage correspondi
-00000ed0: 6e67 2074 6f20 7468 6520 7175 6572 6965  ng to the querie
-00000ee0: 6420 7461 626c 6520 6973 2070 6f70 756c  d table is popul
-00000ef0: 6174 6564 0a20 2020 2069 6e20 7468 6520  ated.    in the 
-00000f00: 7265 7370 6f6e 7365 2e20 5769 7468 696e  response. Within
-00000f10: 2074 6865 2070 6f70 756c 6174 6564 206d   the populated m
-00000f20: 6573 7361 6765 2c20 6f6e 6c79 2074 6865  essage, only the
-00000f30: 2066 6965 6c64 730a 2020 2020 7265 7175   fields.    requ
-00000f40: 6573 7465 6420 6578 706c 6963 6974 6c79  ested explicitly
-00000f50: 2069 6e20 7468 6520 7175 6572 7920 6172   in the query ar
-00000f60: 6520 706f 7075 6c61 7465 642e 0a0a 2020  e populated...  
-00000f70: 2020 4174 7472 6962 7574 6573 3a0a 2020    Attributes:.  
-00000f80: 2020 2020 2020 7072 6f64 7563 745f 7065        product_pe
-00000f90: 7266 6f72 6d61 6e63 655f 7669 6577 2028  rformance_view (
-00000fa0: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
-00000fb0: 6d65 7263 6861 6e74 5f72 6570 6f72 7473  merchant_reports
-00000fc0: 5f76 3162 6574 612e 7479 7065 732e 5072  _v1beta.types.Pr
-00000fd0: 6f64 7563 7450 6572 666f 726d 616e 6365  oductPerformance
-00000fe0: 5669 6577 293a 0a20 2020 2020 2020 2020  View):.         
-00000ff0: 2020 2046 6965 6c64 7320 6176 6169 6c61     Fields availa
-00001000: 626c 6520 666f 7220 7175 6572 7920 696e  ble for query in
-00001010: 2060 6070 726f 6475 6374 5f70 6572 666f   ``product_perfo
-00001020: 726d 616e 6365 5f76 6965 7760 600a 2020  rmance_view``.  
-00001030: 2020 2020 2020 2020 2020 7461 626c 652e            table.
-00001040: 0a20 2020 2020 2020 2070 726f 6475 6374  .        product
-00001050: 5f76 6965 7720 2867 6f6f 676c 652e 7368  _view (google.sh
-00001060: 6f70 7069 6e67 2e6d 6572 6368 616e 745f  opping.merchant_
-00001070: 7265 706f 7274 735f 7631 6265 7461 2e74  reports_v1beta.t
-00001080: 7970 6573 2e50 726f 6475 6374 5669 6577  ypes.ProductView
-00001090: 293a 0a20 2020 2020 2020 2020 2020 2046  ):.            F
-000010a0: 6965 6c64 7320 6176 6169 6c61 626c 6520  ields available 
-000010b0: 666f 7220 7175 6572 7920 696e 2060 6070  for query in ``p
-000010c0: 726f 6475 6374 5f76 6965 7760 6020 7461  roduct_view`` ta
-000010d0: 626c 652e 0a20 2020 2020 2020 2070 7269  ble..        pri
-000010e0: 6365 5f63 6f6d 7065 7469 7469 7665 6e65  ce_competitivene
-000010f0: 7373 5f70 726f 6475 6374 5f76 6965 7720  ss_product_view 
-00001100: 2867 6f6f 676c 652e 7368 6f70 7069 6e67  (google.shopping
-00001110: 2e6d 6572 6368 616e 745f 7265 706f 7274  .merchant_report
-00001120: 735f 7631 6265 7461 2e74 7970 6573 2e50  s_v1beta.types.P
-00001130: 7269 6365 436f 6d70 6574 6974 6976 656e  riceCompetitiven
-00001140: 6573 7350 726f 6475 6374 5669 6577 293a  essProductView):
-00001150: 0a20 2020 2020 2020 2020 2020 2046 6965  .            Fie
-00001160: 6c64 7320 6176 6169 6c61 626c 6520 666f  lds available fo
-00001170: 7220 7175 6572 7920 696e 0a20 2020 2020  r query in.     
-00001180: 2020 2020 2020 2060 6070 7269 6365 5f63         ``price_c
-00001190: 6f6d 7065 7469 7469 7665 6e65 7373 5f70  ompetitiveness_p
-000011a0: 726f 6475 6374 5f76 6965 7760 6020 7461  roduct_view`` ta
-000011b0: 626c 652e 0a20 2020 2020 2020 2070 7269  ble..        pri
-000011c0: 6365 5f69 6e73 6967 6874 735f 7072 6f64  ce_insights_prod
-000011d0: 7563 745f 7669 6577 2028 676f 6f67 6c65  uct_view (google
-000011e0: 2e73 686f 7070 696e 672e 6d65 7263 6861  .shopping.mercha
-000011f0: 6e74 5f72 6570 6f72 7473 5f76 3162 6574  nt_reports_v1bet
-00001200: 612e 7479 7065 732e 5072 6963 6549 6e73  a.types.PriceIns
-00001210: 6967 6874 7350 726f 6475 6374 5669 6577  ightsProductView
-00001220: 293a 0a20 2020 2020 2020 2020 2020 2046  ):.            F
-00001230: 6965 6c64 7320 6176 6169 6c61 626c 6520  ields available 
-00001240: 666f 7220 7175 6572 7920 696e 0a20 2020  for query in.   
-00001250: 2020 2020 2020 2020 2060 6070 7269 6365           ``price
-00001260: 5f69 6e73 6967 6874 735f 7072 6f64 7563  _insights_produc
-00001270: 745f 7669 6577 6060 2074 6162 6c65 2e0a  t_view`` table..
-00001280: 2020 2020 2020 2020 6265 7374 5f73 656c          best_sel
-00001290: 6c65 7273 5f70 726f 6475 6374 5f63 6c75  lers_product_clu
-000012a0: 7374 6572 5f76 6965 7720 2867 6f6f 676c  ster_view (googl
-000012b0: 652e 7368 6f70 7069 6e67 2e6d 6572 6368  e.shopping.merch
-000012c0: 616e 745f 7265 706f 7274 735f 7631 6265  ant_reports_v1be
-000012d0: 7461 2e74 7970 6573 2e42 6573 7453 656c  ta.types.BestSel
-000012e0: 6c65 7273 5072 6f64 7563 7443 6c75 7374  lersProductClust
-000012f0: 6572 5669 6577 293a 0a20 2020 2020 2020  erView):.       
-00001300: 2020 2020 2046 6965 6c64 7320 6176 6169       Fields avai
-00001310: 6c61 626c 6520 666f 7220 7175 6572 7920  lable for query 
-00001320: 696e 0a20 2020 2020 2020 2020 2020 2060  in.            `
-00001330: 6062 6573 745f 7365 6c6c 6572 735f 7072  `best_sellers_pr
-00001340: 6f64 7563 745f 636c 7573 7465 725f 7669  oduct_cluster_vi
-00001350: 6577 6060 2074 6162 6c65 2e0a 2020 2020  ew`` table..    
-00001360: 2020 2020 6265 7374 5f73 656c 6c65 7273      best_sellers
-00001370: 5f62 7261 6e64 5f76 6965 7720 2867 6f6f  _brand_view (goo
-00001380: 676c 652e 7368 6f70 7069 6e67 2e6d 6572  gle.shopping.mer
-00001390: 6368 616e 745f 7265 706f 7274 735f 7631  chant_reports_v1
-000013a0: 6265 7461 2e74 7970 6573 2e42 6573 7453  beta.types.BestS
-000013b0: 656c 6c65 7273 4272 616e 6456 6965 7729  ellersBrandView)
-000013c0: 3a0a 2020 2020 2020 2020 2020 2020 4669  :.            Fi
-000013d0: 656c 6473 2061 7661 696c 6162 6c65 2066  elds available f
-000013e0: 6f72 2071 7565 7279 2069 6e20 6060 6265  or query in ``be
-000013f0: 7374 5f73 656c 6c65 7273 5f62 7261 6e64  st_sellers_brand
-00001400: 5f76 6965 7760 600a 2020 2020 2020 2020  _view``.        
-00001410: 2020 2020 7461 626c 652e 0a20 2020 2020      table..     
-00001420: 2020 2063 6f6d 7065 7469 7469 7665 5f76     competitive_v
-00001430: 6973 6962 696c 6974 795f 636f 6d70 6574  isibility_compet
-00001440: 6974 6f72 5f76 6965 7720 2867 6f6f 676c  itor_view (googl
-00001450: 652e 7368 6f70 7069 6e67 2e6d 6572 6368  e.shopping.merch
-00001460: 616e 745f 7265 706f 7274 735f 7631 6265  ant_reports_v1be
-00001470: 7461 2e74 7970 6573 2e43 6f6d 7065 7469  ta.types.Competi
-00001480: 7469 7665 5669 7369 6269 6c69 7479 436f  tiveVisibilityCo
-00001490: 6d70 6574 6974 6f72 5669 6577 293a 0a20  mpetitorView):. 
-000014a0: 2020 2020 2020 2020 2020 2046 6965 6c64             Field
-000014b0: 7320 6176 6169 6c61 626c 6520 666f 7220  s available for 
-000014c0: 7175 6572 7920 696e 0a20 2020 2020 2020  query in.       
-000014d0: 2020 2020 2060 6063 6f6d 7065 7469 7469       ``competiti
-000014e0: 7665 5f76 6973 6962 696c 6974 795f 636f  ve_visibility_co
-000014f0: 6d70 6574 6974 6f72 5f76 6965 7760 6020  mpetitor_view`` 
-00001500: 7461 626c 652e 0a20 2020 2020 2020 2063  table..        c
-00001510: 6f6d 7065 7469 7469 7665 5f76 6973 6962  ompetitive_visib
-00001520: 696c 6974 795f 746f 705f 6d65 7263 6861  ility_top_mercha
-00001530: 6e74 5f76 6965 7720 2867 6f6f 676c 652e  nt_view (google.
-00001540: 7368 6f70 7069 6e67 2e6d 6572 6368 616e  shopping.merchan
-00001550: 745f 7265 706f 7274 735f 7631 6265 7461  t_reports_v1beta
-00001560: 2e74 7970 6573 2e43 6f6d 7065 7469 7469  .types.Competiti
-00001570: 7665 5669 7369 6269 6c69 7479 546f 704d  veVisibilityTopM
-00001580: 6572 6368 616e 7456 6965 7729 3a0a 2020  erchantView):.  
-00001590: 2020 2020 2020 2020 2020 4669 656c 6473            Fields
-000015a0: 2061 7661 696c 6162 6c65 2066 6f72 2071   available for q
-000015b0: 7565 7279 2069 6e0a 2020 2020 2020 2020  uery in.        
-000015c0: 2020 2020 6060 636f 6d70 6574 6974 6976      ``competitiv
-000015d0: 655f 7669 7369 6269 6c69 7479 5f74 6f70  e_visibility_top
-000015e0: 5f6d 6572 6368 616e 745f 7669 6577 6060  _merchant_view``
-000015f0: 2074 6162 6c65 2e0a 2020 2020 2020 2020   table..        
-00001600: 636f 6d70 6574 6974 6976 655f 7669 7369  competitive_visi
-00001610: 6269 6c69 7479 5f62 656e 6368 6d61 726b  bility_benchmark
-00001620: 5f76 6965 7720 2867 6f6f 676c 652e 7368  _view (google.sh
-00001630: 6f70 7069 6e67 2e6d 6572 6368 616e 745f  opping.merchant_
-00001640: 7265 706f 7274 735f 7631 6265 7461 2e74  reports_v1beta.t
-00001650: 7970 6573 2e43 6f6d 7065 7469 7469 7665  ypes.Competitive
-00001660: 5669 7369 6269 6c69 7479 4265 6e63 686d  VisibilityBenchm
-00001670: 6172 6b56 6965 7729 3a0a 2020 2020 2020  arkView):.      
-00001680: 2020 2020 2020 4669 656c 6473 2061 7661        Fields ava
-00001690: 696c 6162 6c65 2066 6f72 2071 7565 7279  ilable for query
-000016a0: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
-000016b0: 6060 636f 6d70 6574 6974 6976 655f 7669  ``competitive_vi
-000016c0: 7369 6269 6c69 7479 5f62 656e 6368 6d61  sibility_benchma
-000016d0: 726b 5f76 6965 7760 6020 7461 626c 652e  rk_view`` table.
-000016e0: 0a20 2020 2022 2222 0a0a 2020 2020 7072  .    """..    pr
-000016f0: 6f64 7563 745f 7065 7266 6f72 6d61 6e63  oduct_performanc
-00001700: 655f 7669 6577 3a20 2250 726f 6475 6374  e_view: "Product
-00001710: 5065 7266 6f72 6d61 6e63 6556 6965 7722  PerformanceView"
-00001720: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00001730: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
-00001740: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
-00001750: 756d 6265 723d 312c 0a20 2020 2020 2020  umber=1,.       
-00001760: 206d 6573 7361 6765 3d22 5072 6f64 7563   message="Produc
-00001770: 7450 6572 666f 726d 616e 6365 5669 6577  tPerformanceView
-00001780: 222c 0a20 2020 2029 0a20 2020 2070 726f  ",.    ).    pro
-00001790: 6475 6374 5f76 6965 773a 2022 5072 6f64  duct_view: "Prod
-000017a0: 7563 7456 6965 7722 203d 2070 726f 746f  uctView" = proto
-000017b0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-000017c0: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
-000017d0: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
-000017e0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-000017f0: 3d22 5072 6f64 7563 7456 6965 7722 2c0a  ="ProductView",.
-00001800: 2020 2020 290a 2020 2020 7072 6963 655f      ).    price_
-00001810: 636f 6d70 6574 6974 6976 656e 6573 735f  competitiveness_
-00001820: 7072 6f64 7563 745f 7669 6577 3a20 2250  product_view: "P
-00001830: 7269 6365 436f 6d70 6574 6974 6976 656e  riceCompetitiven
-00001840: 6573 7350 726f 6475 6374 5669 6577 2220  essProductView" 
-00001850: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00001860: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
-00001870: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
-00001880: 6d62 6572 3d33 2c0a 2020 2020 2020 2020  mber=3,.        
-00001890: 6d65 7373 6167 653d 2250 7269 6365 436f  message="PriceCo
-000018a0: 6d70 6574 6974 6976 656e 6573 7350 726f  mpetitivenessPro
-000018b0: 6475 6374 5669 6577 222c 0a20 2020 2029  ductView",.    )
-000018c0: 0a20 2020 2070 7269 6365 5f69 6e73 6967  .    price_insig
-000018d0: 6874 735f 7072 6f64 7563 745f 7669 6577  hts_product_view
-000018e0: 3a20 2250 7269 6365 496e 7369 6768 7473  : "PriceInsights
-000018f0: 5072 6f64 7563 7456 6965 7722 203d 2070  ProductView" = p
-00001900: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00001910: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
-00001920: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
-00001930: 723d 342c 0a20 2020 2020 2020 206d 6573  r=4,.        mes
-00001940: 7361 6765 3d22 5072 6963 6549 6e73 6967  sage="PriceInsig
-00001950: 6874 7350 726f 6475 6374 5669 6577 222c  htsProductView",
-00001960: 0a20 2020 2029 0a20 2020 2062 6573 745f  .    ).    best_
-00001970: 7365 6c6c 6572 735f 7072 6f64 7563 745f  sellers_product_
-00001980: 636c 7573 7465 725f 7669 6577 3a20 2242  cluster_view: "B
-00001990: 6573 7453 656c 6c65 7273 5072 6f64 7563  estSellersProduc
-000019a0: 7443 6c75 7374 6572 5669 6577 2220 3d20  tClusterView" = 
-000019b0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-000019c0: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
-000019d0: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
-000019e0: 6572 3d35 2c0a 2020 2020 2020 2020 6d65  er=5,.        me
-000019f0: 7373 6167 653d 2242 6573 7453 656c 6c65  ssage="BestSelle
-00001a00: 7273 5072 6f64 7563 7443 6c75 7374 6572  rsProductCluster
-00001a10: 5669 6577 222c 0a20 2020 2029 0a20 2020  View",.    ).   
-00001a20: 2062 6573 745f 7365 6c6c 6572 735f 6272   best_sellers_br
-00001a30: 616e 645f 7669 6577 3a20 2242 6573 7453  and_view: "BestS
-00001a40: 656c 6c65 7273 4272 616e 6456 6965 7722  ellersBrandView"
-00001a50: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00001a60: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
-00001a70: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
-00001a80: 756d 6265 723d 362c 0a20 2020 2020 2020  umber=6,.       
-00001a90: 206d 6573 7361 6765 3d22 4265 7374 5365   message="BestSe
-00001aa0: 6c6c 6572 7342 7261 6e64 5669 6577 222c  llersBrandView",
-00001ab0: 0a20 2020 2029 0a20 2020 2063 6f6d 7065  .    ).    compe
-00001ac0: 7469 7469 7665 5f76 6973 6962 696c 6974  titive_visibilit
-00001ad0: 795f 636f 6d70 6574 6974 6f72 5f76 6965  y_competitor_vie
-00001ae0: 773a 2022 436f 6d70 6574 6974 6976 6556  w: "CompetitiveV
-00001af0: 6973 6962 696c 6974 7943 6f6d 7065 7469  isibilityCompeti
-00001b00: 746f 7256 6965 7722 203d 2028 0a20 2020  torView" = (.   
-00001b10: 2020 2020 2070 726f 746f 2e46 6965 6c64       proto.Field
-00001b20: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
-00001b30: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
-00001b40: 2020 2020 2020 2020 206e 756d 6265 723d           number=
-00001b50: 382c 0a20 2020 2020 2020 2020 2020 206d  8,.            m
-00001b60: 6573 7361 6765 3d22 436f 6d70 6574 6974  essage="Competit
-00001b70: 6976 6556 6973 6962 696c 6974 7943 6f6d  iveVisibilityCom
-00001b80: 7065 7469 746f 7256 6965 7722 2c0a 2020  petitorView",.  
-00001b90: 2020 2020 2020 290a 2020 2020 290a 2020        ).    ).  
-00001ba0: 2020 636f 6d70 6574 6974 6976 655f 7669    competitive_vi
-00001bb0: 7369 6269 6c69 7479 5f74 6f70 5f6d 6572  sibility_top_mer
-00001bc0: 6368 616e 745f 7669 6577 3a20 2243 6f6d  chant_view: "Com
-00001bd0: 7065 7469 7469 7665 5669 7369 6269 6c69  petitiveVisibili
-00001be0: 7479 546f 704d 6572 6368 616e 7456 6965  tyTopMerchantVie
-00001bf0: 7722 203d 2028 0a20 2020 2020 2020 2070  w" = (.        p
-00001c00: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00001c10: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
-00001c20: 5353 4147 452c 0a20 2020 2020 2020 2020  SSAGE,.         
-00001c30: 2020 206e 756d 6265 723d 392c 0a20 2020     number=9,.   
-00001c40: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00001c50: 3d22 436f 6d70 6574 6974 6976 6556 6973  ="CompetitiveVis
-00001c60: 6962 696c 6974 7954 6f70 4d65 7263 6861  ibilityTopMercha
-00001c70: 6e74 5669 6577 222c 0a20 2020 2020 2020  ntView",.       
-00001c80: 2029 0a20 2020 2029 0a20 2020 2063 6f6d   ).    ).    com
-00001c90: 7065 7469 7469 7665 5f76 6973 6962 696c  petitive_visibil
-00001ca0: 6974 795f 6265 6e63 686d 6172 6b5f 7669  ity_benchmark_vi
-00001cb0: 6577 3a20 2243 6f6d 7065 7469 7469 7665  ew: "Competitive
-00001cc0: 5669 7369 6269 6c69 7479 4265 6e63 686d  VisibilityBenchm
-00001cd0: 6172 6b56 6965 7722 203d 2028 0a20 2020  arkView" = (.   
-00001ce0: 2020 2020 2070 726f 746f 2e46 6965 6c64       proto.Field
-00001cf0: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
-00001d00: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
-00001d10: 2020 2020 2020 2020 206e 756d 6265 723d           number=
-00001d20: 3130 2c0a 2020 2020 2020 2020 2020 2020  10,.            
-00001d30: 6d65 7373 6167 653d 2243 6f6d 7065 7469  message="Competi
-00001d40: 7469 7665 5669 7369 6269 6c69 7479 4265  tiveVisibilityBe
-00001d50: 6e63 686d 6172 6b56 6965 7722 2c0a 2020  nchmarkView",.  
-00001d60: 2020 2020 2020 290a 2020 2020 290a 0a0a        ).    )...
-00001d70: 636c 6173 7320 5072 6f64 7563 7450 6572  class ProductPer
-00001d80: 666f 726d 616e 6365 5669 6577 2870 726f  formanceView(pro
-00001d90: 746f 2e4d 6573 7361 6765 293a 0a20 2020  to.Message):.   
-00001da0: 2072 2222 2246 6965 6c64 7320 6176 6169   r"""Fields avai
-00001db0: 6c61 626c 6520 666f 7220 7175 6572 7920  lable for query 
-00001dc0: 696e 2060 6070 726f 6475 6374 5f70 6572  in ``product_per
-00001dd0: 666f 726d 616e 6365 5f76 6965 7760 6020  formance_view`` 
-00001de0: 7461 626c 652e 0a0a 2020 2020 5072 6f64  table...    Prod
-00001df0: 7563 7420 7065 7266 6f72 6d61 6e63 6520  uct performance 
-00001e00: 6461 7461 2066 6f72 2079 6f75 7220 6163  data for your ac
-00001e10: 636f 756e 742c 2069 6e63 6c75 6469 6e67  count, including
-00001e20: 2070 6572 666f 726d 616e 6365 0a20 2020   performance.   
-00001e30: 206d 6574 7269 6373 2028 666f 7220 6578   metrics (for ex
-00001e40: 616d 706c 652c 2060 6063 6c69 636b 7360  ample, ``clicks`
-00001e50: 6029 2061 6e64 2064 696d 656e 7369 6f6e  `) and dimension
-00001e60: 7320 6163 636f 7264 696e 6720 746f 2077  s according to w
-00001e70: 6869 6368 0a20 2020 2070 6572 666f 726d  hich.    perform
-00001e80: 616e 6365 206d 6574 7269 6373 2061 7265  ance metrics are
-00001e90: 2073 6567 6d65 6e74 6564 2028 666f 7220   segmented (for 
-00001ea0: 6578 616d 706c 652c 2060 606f 6666 6572  example, ``offer
-00001eb0: 5f69 6460 6029 2e0a 2020 2020 5661 6c75  _id``)..    Valu
-00001ec0: 6573 206f 6620 7072 6f64 7563 7420 6469  es of product di
-00001ed0: 6d65 6e73 696f 6e73 2c20 7375 6368 2061  mensions, such a
-00001ee0: 7320 6060 6f66 6665 725f 6964 6060 2c20  s ``offer_id``, 
-00001ef0: 7265 666c 6563 7420 7468 650a 2020 2020  reflect the.    
-00001f00: 7374 6174 6520 6f66 2061 2070 726f 6475  state of a produ
-00001f10: 6374 2061 7420 7468 6520 7469 6d65 206f  ct at the time o
-00001f20: 6620 7468 6520 696d 7072 6573 7369 6f6e  f the impression
-00001f30: 2e0a 0a20 2020 2053 6567 6d65 6e74 2066  ...    Segment f
-00001f40: 6965 6c64 7320 6361 6e6e 6f74 2062 6520  ields cannot be 
-00001f50: 7365 6c65 6374 6564 2069 6e20 7175 6572  selected in quer
-00001f60: 6965 7320 7769 7468 6f75 7420 616c 736f  ies without also
-00001f70: 2073 656c 6563 7469 6e67 0a20 2020 2061   selecting.    a
-00001f80: 7420 6c65 6173 7420 6f6e 6520 6d65 7472  t least one metr
-00001f90: 6963 2066 6965 6c64 2e0a 0a20 2020 2056  ic field...    V
-00001fa0: 616c 7565 7320 6172 6520 6f6e 6c79 2073  alues are only s
-00001fb0: 6574 2066 6f72 2066 6965 6c64 7320 7265  et for fields re
-00001fc0: 7175 6573 7465 6420 6578 706c 6963 6974  quested explicit
-00001fd0: 6c79 2069 6e20 7468 6520 7265 7175 6573  ly in the reques
-00001fe0: 7427 730a 2020 2020 7365 6172 6368 2071  t's.    search q
-00001ff0: 7565 7279 2e0a 0a0a 2020 2020 2e2e 205f  uery....    .. _
-00002000: 6f6e 656f 663a 2068 7474 7073 3a2f 2f70  oneof: https://p
-00002010: 726f 746f 2d70 6c75 732d 7079 7468 6f6e  roto-plus-python
-00002020: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00002030: 656e 2f73 7461 626c 652f 6669 656c 6473  en/stable/fields
-00002040: 2e68 746d 6c23 6f6e 656f 6673 2d6d 7574  .html#oneofs-mut
-00002050: 7561 6c6c 792d 6578 636c 7573 6976 652d  ually-exclusive-
-00002060: 6669 656c 6473 0a0a 2020 2020 4174 7472  fields..    Attr
-00002070: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
-00002080: 6d61 726b 6574 696e 675f 6d65 7468 6f64  marketing_method
-00002090: 2028 676f 6f67 6c65 2e73 686f 7070 696e   (google.shoppin
-000020a0: 672e 6d65 7263 6861 6e74 5f72 6570 6f72  g.merchant_repor
-000020b0: 7473 5f76 3162 6574 612e 7479 7065 732e  ts_v1beta.types.
-000020c0: 4d61 726b 6574 696e 674d 6574 686f 642e  MarketingMethod.
-000020d0: 4d61 726b 6574 696e 674d 6574 686f 6445  MarketingMethodE
-000020e0: 6e75 6d29 3a0a 2020 2020 2020 2020 2020  num):.          
-000020f0: 2020 4d61 726b 6574 696e 6720 6d65 7468    Marketing meth
-00002100: 6f64 2074 6f20 7768 6963 6820 6d65 7472  od to which metr
-00002110: 6963 7320 6170 706c 792e 0a20 2020 2020  ics apply..     
-00002120: 2020 2020 2020 2053 6567 6d65 6e74 2e0a         Segment..
-00002130: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-00002140: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-00002150: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-00002160: 6060 5f6d 6172 6b65 7469 6e67 5f6d 6574  ``_marketing_met
-00002170: 686f 6460 602e 0a20 2020 2020 2020 2064  hod``..        d
-00002180: 6174 6520 2867 6f6f 676c 652e 7479 7065  ate (google.type
-00002190: 2e64 6174 655f 7062 322e 4461 7465 293a  .date_pb2.Date):
-000021a0: 0a20 2020 2020 2020 2020 2020 2044 6174  .            Dat
-000021b0: 6520 696e 2074 6865 206d 6572 6368 616e  e in the merchan
-000021c0: 7420 7469 6d65 7a6f 6e65 2074 6f20 7768  t timezone to wh
-000021d0: 6963 6820 6d65 7472 6963 7320 6170 706c  ich metrics appl
-000021e0: 792e 0a20 2020 2020 2020 2020 2020 2053  y..            S
-000021f0: 6567 6d65 6e74 2e0a 0a20 2020 2020 2020  egment...       
-00002200: 2020 2020 2043 6f6e 6469 7469 6f6e 206f       Condition o
-00002210: 6e20 6060 6461 7465 6060 2069 7320 7265  n ``date`` is re
-00002220: 7175 6972 6564 2069 6e20 7468 6520 6060  quired in the ``
-00002230: 5748 4552 4560 6020 636c 6175 7365 2e0a  WHERE`` clause..
-00002240: 2020 2020 2020 2020 7765 656b 2028 676f          week (go
-00002250: 6f67 6c65 2e74 7970 652e 6461 7465 5f70  ogle.type.date_p
-00002260: 6232 2e44 6174 6529 3a0a 2020 2020 2020  b2.Date):.      
-00002270: 2020 2020 2020 4669 7273 7420 6461 7920        First day 
-00002280: 6f66 2074 6865 2077 6565 6b20 284d 6f6e  of the week (Mon
-00002290: 6461 7929 206f 6620 7468 6520 6d65 7472  day) of the metr
-000022a0: 6963 730a 2020 2020 2020 2020 2020 2020  ics.            
-000022b0: 6461 7465 2069 6e20 7468 6520 6d65 7263  date in the merc
-000022c0: 6861 6e74 2074 696d 657a 6f6e 652e 2053  hant timezone. S
-000022d0: 6567 6d65 6e74 2e0a 2020 2020 2020 2020  egment..        
-000022e0: 6375 7374 6f6d 6572 5f63 6f75 6e74 7279  customer_country
-000022f0: 5f63 6f64 6520 2873 7472 293a 0a20 2020  _code (str):.   
-00002300: 2020 2020 2020 2020 2043 6f64 6520 6f66           Code of
-00002310: 2074 6865 2063 6f75 6e74 7279 2077 6865   the country whe
-00002320: 7265 2074 6865 2063 7573 746f 6d65 7220  re the customer 
-00002330: 6973 0a20 2020 2020 2020 2020 2020 206c  is.            l
-00002340: 6f63 6174 6564 2061 7420 7468 6520 7469  ocated at the ti
-00002350: 6d65 206f 6620 7468 6520 6576 656e 742e  me of the event.
-00002360: 2052 6570 7265 7365 6e74 6564 2069 6e0a   Represented in.
-00002370: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00002380: 4953 4f20 3331 3636 2066 6f72 6d61 742e  ISO 3166 format.
-00002390: 2053 6567 6d65 6e74 2e0a 0a20 2020 2020   Segment...     
-000023a0: 2020 2020 2020 2049 6620 7468 6520 6375         If the cu
-000023b0: 7374 6f6d 6572 2063 6f75 6e74 7279 2063  stomer country c
-000023c0: 616e 6e6f 7420 6265 2064 6574 6572 6d69  annot be determi
-000023d0: 6e65 642c 2061 0a20 2020 2020 2020 2020  ned, a.         
-000023e0: 2020 2073 7065 6369 616c 2027 5a5a 2720     special 'ZZ' 
-000023f0: 636f 6465 2069 7320 7265 7475 726e 6564  code is returned
-00002400: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-00002410: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-00002420: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-00002430: 5f20 6060 5f63 7573 746f 6d65 725f 636f  _ ``_customer_co
-00002440: 756e 7472 795f 636f 6465 6060 2e0a 2020  untry_code``..  
-00002450: 2020 2020 2020 6f66 6665 725f 6964 2028        offer_id (
-00002460: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00002470: 2020 4d65 7263 6861 6e74 2d70 726f 7669    Merchant-provi
-00002480: 6465 6420 6964 206f 6620 7468 6520 7072  ded id of the pr
-00002490: 6f64 7563 742e 2053 6567 6d65 6e74 2e0a  oduct. Segment..
-000024a0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-000024b0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-000024c0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-000024d0: 6060 5f6f 6666 6572 5f69 6460 602e 0a20  ``_offer_id``.. 
-000024e0: 2020 2020 2020 2074 6974 6c65 2028 7374         title (st
-000024f0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00002500: 5469 746c 6520 6f66 2074 6865 2070 726f  Title of the pro
-00002510: 6475 6374 2e20 5365 676d 656e 742e 0a0a  duct. Segment...
-00002520: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00002530: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00002540: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00002550: 605f 7469 746c 6560 602e 0a20 2020 2020  `_title``..     
-00002560: 2020 2062 7261 6e64 2028 7374 7229 3a0a     brand (str):.
-00002570: 2020 2020 2020 2020 2020 2020 4272 616e              Bran
-00002580: 6420 6f66 2074 6865 2070 726f 6475 6374  d of the product
-00002590: 2e20 5365 676d 656e 742e 0a0a 2020 2020  . Segment...    
-000025a0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-000025b0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-000025c0: 6620 606f 6e65 6f66 605f 2060 605f 6272  f `oneof`_ ``_br
-000025d0: 616e 6460 602e 0a20 2020 2020 2020 2063  and``..        c
-000025e0: 6174 6567 6f72 795f 6c31 2028 7374 7229  ategory_l1 (str)
-000025f0: 3a0a 2020 2020 2020 2020 2020 2020 6050  :.            `P
-00002600: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
-00002610: 2831 7374 0a20 2020 2020 2020 2020 2020  (1st.           
-00002620: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
-00002630: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-00002640: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
-00002650: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
-00002660: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
-00002670: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
-00002680: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
-00002690: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
-000026a0: 2047 6f6f 676c 6527 7320 7072 6f64 7563   Google's produc
-000026b0: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
-000026c0: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
-000026d0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-000026e0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-000026f0: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
-00002700: 5f6c 3160 602e 0a20 2020 2020 2020 2063  _l1``..        c
-00002710: 6174 6567 6f72 795f 6c32 2028 7374 7229  ategory_l2 (str)
-00002720: 3a0a 2020 2020 2020 2020 2020 2020 6050  :.            `P
-00002730: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
-00002740: 2832 6e64 0a20 2020 2020 2020 2020 2020  (2nd.           
-00002750: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
-00002760: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-00002770: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
-00002780: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
-00002790: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
-000027a0: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
-000027b0: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
-000027c0: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
-000027d0: 2047 6f6f 676c 6527 7320 7072 6f64 7563   Google's produc
-000027e0: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
-000027f0: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
-00002800: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00002810: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00002820: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
-00002830: 5f6c 3260 602e 0a20 2020 2020 2020 2063  _l2``..        c
-00002840: 6174 6567 6f72 795f 6c33 2028 7374 7229  ategory_l3 (str)
-00002850: 3a0a 2020 2020 2020 2020 2020 2020 6050  :.            `P
-00002860: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
-00002870: 2833 7264 0a20 2020 2020 2020 2020 2020  (3rd.           
-00002880: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
-00002890: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-000028a0: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
-000028b0: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
-000028c0: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
-000028d0: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
-000028e0: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
-000028f0: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
-00002900: 2047 6f6f 676c 6527 7320 7072 6f64 7563   Google's produc
-00002910: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
-00002920: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
-00002930: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00002940: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00002950: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
-00002960: 5f6c 3360 602e 0a20 2020 2020 2020 2063  _l3``..        c
-00002970: 6174 6567 6f72 795f 6c34 2028 7374 7229  ategory_l4 (str)
-00002980: 3a0a 2020 2020 2020 2020 2020 2020 6050  :.            `P
-00002990: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
-000029a0: 2834 7468 0a20 2020 2020 2020 2020 2020  (4th.           
-000029b0: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
-000029c0: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-000029d0: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
-000029e0: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
-000029f0: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
-00002a00: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
-00002a10: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
-00002a20: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
-00002a30: 2047 6f6f 676c 6527 7320 7072 6f64 7563   Google's produc
-00002a40: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
-00002a50: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
-00002a60: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00002a70: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00002a80: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
-00002a90: 5f6c 3460 602e 0a20 2020 2020 2020 2063  _l4``..        c
-00002aa0: 6174 6567 6f72 795f 6c35 2028 7374 7229  ategory_l5 (str)
-00002ab0: 3a0a 2020 2020 2020 2020 2020 2020 6050  :.            `P
-00002ac0: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
-00002ad0: 2835 7468 0a20 2020 2020 2020 2020 2020  (5th.           
-00002ae0: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
-00002af0: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-00002b00: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
-00002b10: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
-00002b20: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
-00002b30: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
-00002b40: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
-00002b50: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
-00002b60: 2047 6f6f 676c 6527 7320 7072 6f64 7563   Google's produc
-00002b70: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
-00002b80: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
-00002b90: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00002ba0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00002bb0: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
-00002bc0: 5f6c 3560 602e 0a20 2020 2020 2020 2070  _l5``..        p
-00002bd0: 726f 6475 6374 5f74 7970 655f 6c31 2028  roduct_type_l1 (
-00002be0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00002bf0: 2020 6050 726f 6475 6374 2074 7970 6520    `Product type 
-00002c00: 2831 7374 0a20 2020 2020 2020 2020 2020  (1st.           
-00002c10: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
-00002c20: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
-00002c30: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
-00002c40: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
-00002c50: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
-00002c60: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
-00002c70: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
-00002c80: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
-00002c90: 206d 6572 6368 616e 7427 7320 6f77 6e20   merchant's own 
-00002ca0: 7072 6f64 7563 7420 7461 786f 6e6f 6d79  product taxonomy
-00002cb0: 2e20 5365 676d 656e 742e 0a0a 2020 2020  . Segment...    
-00002cc0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-00002cd0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-00002ce0: 6620 606f 6e65 6f66 605f 2060 605f 7072  f `oneof`_ ``_pr
-00002cf0: 6f64 7563 745f 7479 7065 5f6c 3160 602e  oduct_type_l1``.
-00002d00: 0a20 2020 2020 2020 2070 726f 6475 6374  .        product
-00002d10: 5f74 7970 655f 6c32 2028 7374 7229 3a0a  _type_l2 (str):.
-00002d20: 2020 2020 2020 2020 2020 2020 6050 726f              `Pro
-00002d30: 6475 6374 2074 7970 6520 2832 6e64 0a20  duct type (2nd. 
-00002d40: 2020 2020 2020 2020 2020 206c 6576 656c             level
-00002d50: 2920 3c68 7474 7073 3a2f 2f64 6576 656c  ) <https://devel
-00002d60: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
-00002d70: 2f73 686f 7070 696e 672d 636f 6e74 656e  /shopping-conten
-00002d80: 742f 6775 6964 6573 2f72 6570 6f72 7473  t/guides/reports
-00002d90: 2f73 6567 6d65 6e74 6174 696f 6e23 6361  /segmentation#ca
-00002da0: 7465 676f 7279 5f61 6e64 5f70 726f 6475  tegory_and_produ
-00002db0: 6374 5f74 7970 653e 605f 5f0a 2020 2020  ct_type>`__.    
-00002dc0: 2020 2020 2020 2020 696e 206d 6572 6368          in merch
-00002dd0: 616e 7427 7320 6f77 6e20 7072 6f64 7563  ant's own produc
-00002de0: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
-00002df0: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
-00002e00: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00002e10: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00002e20: 6f66 605f 2060 605f 7072 6f64 7563 745f  of`_ ``_product_
-00002e30: 7479 7065 5f6c 3260 602e 0a20 2020 2020  type_l2``..     
-00002e40: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
-00002e50: 6c33 2028 7374 7229 3a0a 2020 2020 2020  l3 (str):.      
-00002e60: 2020 2020 2020 6050 726f 6475 6374 2074        `Product t
-00002e70: 7970 6520 2833 7264 0a20 2020 2020 2020  ype (3rd.       
-00002e80: 2020 2020 206c 6576 656c 2920 3c68 7474       level) <htt
-00002e90: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
-00002ea0: 676f 6f67 6c65 2e63 6f6d 2f73 686f 7070  google.com/shopp
-00002eb0: 696e 672d 636f 6e74 656e 742f 6775 6964  ing-content/guid
-00002ec0: 6573 2f72 6570 6f72 7473 2f73 6567 6d65  es/reports/segme
-00002ed0: 6e74 6174 696f 6e23 6361 7465 676f 7279  ntation#category
-00002ee0: 5f61 6e64 5f70 726f 6475 6374 5f74 7970  _and_product_typ
-00002ef0: 653e 605f 5f0a 2020 2020 2020 2020 2020  e>`__.          
-00002f00: 2020 696e 206d 6572 6368 616e 7427 7320    in merchant's 
-00002f10: 6f77 6e20 7072 6f64 7563 7420 7461 786f  own product taxo
-00002f20: 6e6f 6d79 2e20 5365 676d 656e 742e 0a0a  nomy. Segment...
-00002f30: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00002f40: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00002f50: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00002f60: 605f 7072 6f64 7563 745f 7479 7065 5f6c  `_product_type_l
-00002f70: 3360 602e 0a20 2020 2020 2020 2070 726f  3``..        pro
-00002f80: 6475 6374 5f74 7970 655f 6c34 2028 7374  duct_type_l4 (st
-00002f90: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00002fa0: 6050 726f 6475 6374 2074 7970 6520 2834  `Product type (4
-00002fb0: 7468 0a20 2020 2020 2020 2020 2020 206c  th.            l
-00002fc0: 6576 656c 2920 3c68 7474 7073 3a2f 2f64  evel) <https://d
-00002fd0: 6576 656c 6f70 6572 732e 676f 6f67 6c65  evelopers.google
-00002fe0: 2e63 6f6d 2f73 686f 7070 696e 672d 636f  .com/shopping-co
-00002ff0: 6e74 656e 742f 6775 6964 6573 2f72 6570  ntent/guides/rep
-00003000: 6f72 7473 2f73 6567 6d65 6e74 6174 696f  orts/segmentatio
-00003010: 6e23 6361 7465 676f 7279 5f61 6e64 5f70  n#category_and_p
-00003020: 726f 6475 6374 5f74 7970 653e 605f 5f0a  roduct_type>`__.
-00003030: 2020 2020 2020 2020 2020 2020 696e 206d              in m
-00003040: 6572 6368 616e 7427 7320 6f77 6e20 7072  erchant's own pr
-00003050: 6f64 7563 7420 7461 786f 6e6f 6d79 2e20  oduct taxonomy. 
-00003060: 5365 676d 656e 742e 0a0a 2020 2020 2020  Segment...      
-00003070: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-00003080: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-00003090: 606f 6e65 6f66 605f 2060 605f 7072 6f64  `oneof`_ ``_prod
-000030a0: 7563 745f 7479 7065 5f6c 3460 602e 0a20  uct_type_l4``.. 
-000030b0: 2020 2020 2020 2070 726f 6475 6374 5f74         product_t
-000030c0: 7970 655f 6c35 2028 7374 7229 3a0a 2020  ype_l5 (str):.  
-000030d0: 2020 2020 2020 2020 2020 6050 726f 6475            `Produ
-000030e0: 6374 2074 7970 6520 2835 7468 0a20 2020  ct type (5th.   
-000030f0: 2020 2020 2020 2020 206c 6576 656c 2920           level) 
-00003100: 3c68 7474 7073 3a2f 2f64 6576 656c 6f70  <https://develop
-00003110: 6572 732e 676f 6f67 6c65 2e63 6f6d 2f73  ers.google.com/s
-00003120: 686f 7070 696e 672d 636f 6e74 656e 742f  hopping-content/
-00003130: 6775 6964 6573 2f72 6570 6f72 7473 2f73  guides/reports/s
-00003140: 6567 6d65 6e74 6174 696f 6e23 6361 7465  egmentation#cate
-00003150: 676f 7279 5f61 6e64 5f70 726f 6475 6374  gory_and_product
-00003160: 5f74 7970 653e 605f 5f0a 2020 2020 2020  _type>`__.      
-00003170: 2020 2020 2020 696e 206d 6572 6368 616e        in merchan
-00003180: 7427 7320 6f77 6e20 7072 6f64 7563 7420  t's own product 
-00003190: 7461 786f 6e6f 6d79 2e20 5365 676d 656e  taxonomy. Segmen
-000031a0: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
-000031b0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-000031c0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-000031d0: 605f 2060 605f 7072 6f64 7563 745f 7479  `_ ``_product_ty
-000031e0: 7065 5f6c 3560 602e 0a20 2020 2020 2020  pe_l5``..       
-000031f0: 2063 7573 746f 6d5f 6c61 6265 6c30 2028   custom_label0 (
-00003200: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00003210: 2020 4375 7374 6f6d 206c 6162 656c 2030    Custom label 0
-00003220: 2066 6f72 2063 7573 746f 6d20 6772 6f75   for custom grou
-00003230: 7069 6e67 206f 660a 2020 2020 2020 2020  ping of.        
-00003240: 2020 2020 7072 6f64 7563 7473 2e20 5365      products. Se
-00003250: 676d 656e 742e 0a0a 2020 2020 2020 2020  gment...        
-00003260: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-00003270: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-00003280: 6e65 6f66 605f 2060 605f 6375 7374 6f6d  neof`_ ``_custom
-00003290: 5f6c 6162 656c 3060 602e 0a20 2020 2020  _label0``..     
-000032a0: 2020 2063 7573 746f 6d5f 6c61 6265 6c31     custom_label1
-000032b0: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
-000032c0: 2020 2020 4375 7374 6f6d 206c 6162 656c      Custom label
-000032d0: 2031 2066 6f72 2063 7573 746f 6d20 6772   1 for custom gr
-000032e0: 6f75 7069 6e67 206f 660a 2020 2020 2020  ouping of.      
-000032f0: 2020 2020 2020 7072 6f64 7563 7473 2e20        products. 
-00003300: 5365 676d 656e 742e 0a0a 2020 2020 2020  Segment...      
-00003310: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-00003320: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-00003330: 606f 6e65 6f66 605f 2060 605f 6375 7374  `oneof`_ ``_cust
-00003340: 6f6d 5f6c 6162 656c 3160 602e 0a20 2020  om_label1``..   
-00003350: 2020 2020 2063 7573 746f 6d5f 6c61 6265       custom_labe
-00003360: 6c32 2028 7374 7229 3a0a 2020 2020 2020  l2 (str):.      
-00003370: 2020 2020 2020 4375 7374 6f6d 206c 6162        Custom lab
-00003380: 656c 2032 2066 6f72 2063 7573 746f 6d20  el 2 for custom 
-00003390: 6772 6f75 7069 6e67 206f 660a 2020 2020  grouping of.    
-000033a0: 2020 2020 2020 2020 7072 6f64 7563 7473          products
-000033b0: 2e20 5365 676d 656e 742e 0a0a 2020 2020  . Segment...    
-000033c0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-000033d0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-000033e0: 6620 606f 6e65 6f66 605f 2060 605f 6375  f `oneof`_ ``_cu
-000033f0: 7374 6f6d 5f6c 6162 656c 3260 602e 0a20  stom_label2``.. 
-00003400: 2020 2020 2020 2063 7573 746f 6d5f 6c61         custom_la
-00003410: 6265 6c33 2028 7374 7229 3a0a 2020 2020  bel3 (str):.    
-00003420: 2020 2020 2020 2020 4375 7374 6f6d 206c          Custom l
-00003430: 6162 656c 2033 2066 6f72 2063 7573 746f  abel 3 for custo
-00003440: 6d20 6772 6f75 7069 6e67 206f 660a 2020  m grouping of.  
-00003450: 2020 2020 2020 2020 2020 7072 6f64 7563            produc
-00003460: 7473 2e20 5365 676d 656e 742e 0a0a 2020  ts. Segment...  
-00003470: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00003480: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-00003490: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-000034a0: 6375 7374 6f6d 5f6c 6162 656c 3360 602e  custom_label3``.
-000034b0: 0a20 2020 2020 2020 2063 7573 746f 6d5f  .        custom_
-000034c0: 6c61 6265 6c34 2028 7374 7229 3a0a 2020  label4 (str):.  
-000034d0: 2020 2020 2020 2020 2020 4375 7374 6f6d            Custom
-000034e0: 206c 6162 656c 2034 2066 6f72 2063 7573   label 4 for cus
-000034f0: 746f 6d20 6772 6f75 7069 6e67 206f 660a  tom grouping of.
-00003500: 2020 2020 2020 2020 2020 2020 7072 6f64              prod
-00003510: 7563 7473 2e20 5365 676d 656e 742e 0a0a  ucts. Segment...
-00003520: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00003530: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00003540: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00003550: 605f 6375 7374 6f6d 5f6c 6162 656c 3460  `_custom_label4`
-00003560: 602e 0a20 2020 2020 2020 2063 6c69 636b  `..        click
-00003570: 7320 2869 6e74 293a 0a20 2020 2020 2020  s (int):.       
-00003580: 2020 2020 204e 756d 6265 7220 6f66 2063       Number of c
-00003590: 6c69 636b 732e 204d 6574 7269 632e 0a0a  licks. Metric...
-000035a0: 2020 2020 2020 2020 2020 2020 5468 6973              This
-000035b0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-000035c0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-000035d0: 605f 636c 6963 6b73 6060 2e0a 2020 2020  `_clicks``..    
-000035e0: 2020 2020 696d 7072 6573 7369 6f6e 7320      impressions 
-000035f0: 2869 6e74 293a 0a20 2020 2020 2020 2020  (int):.         
-00003600: 2020 204e 756d 6265 7220 6f66 2074 696d     Number of tim
-00003610: 6573 206d 6572 6368 616e 7427 7320 7072  es merchant's pr
-00003620: 6f64 7563 7473 2061 7265 0a20 2020 2020  oducts are.     
-00003630: 2020 2020 2020 2073 686f 776e 2e20 4d65         shown. Me
-00003640: 7472 6963 2e0a 0a20 2020 2020 2020 2020  tric...         
-00003650: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-00003660: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-00003670: 656f 6660 5f20 6060 5f69 6d70 7265 7373  eof`_ ``_impress
-00003680: 696f 6e73 6060 2e0a 2020 2020 2020 2020  ions``..        
-00003690: 636c 6963 6b5f 7468 726f 7567 685f 7261  click_through_ra
-000036a0: 7465 2028 666c 6f61 7429 3a0a 2020 2020  te (float):.    
-000036b0: 2020 2020 2020 2020 436c 6963 6b2d 7468          Click-th
-000036c0: 726f 7567 6820 7261 7465 202d 2074 6865  rough rate - the
-000036d0: 206e 756d 6265 7220 6f66 2063 6c69 636b   number of click
-000036e0: 730a 2020 2020 2020 2020 2020 2020 6d65  s.            me
-000036f0: 7263 6861 6e74 2773 2070 726f 6475 6374  rchant's product
-00003700: 7320 7265 6365 6976 6520 2863 6c69 636b  s receive (click
-00003710: 7329 2064 6976 6964 6564 2062 790a 2020  s) divided by.  
-00003720: 2020 2020 2020 2020 2020 7468 6520 6e75            the nu
-00003730: 6d62 6572 206f 6620 7469 6d65 7320 7468  mber of times th
-00003740: 6520 7072 6f64 7563 7473 2061 7265 2073  e products are s
-00003750: 686f 776e 0a20 2020 2020 2020 2020 2020  hown.           
-00003760: 2028 696d 7072 6573 7369 6f6e 7329 2e20   (impressions). 
-00003770: 4d65 7472 6963 2e0a 0a20 2020 2020 2020  Metric...       
-00003780: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-00003790: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-000037a0: 6f6e 656f 6660 5f20 6060 5f63 6c69 636b  oneof`_ ``_click
-000037b0: 5f74 6872 6f75 6768 5f72 6174 6560 602e  _through_rate``.
-000037c0: 0a20 2020 2020 2020 2063 6f6e 7665 7273  .        convers
-000037d0: 696f 6e73 2028 666c 6f61 7429 3a0a 2020  ions (float):.  
-000037e0: 2020 2020 2020 2020 2020 4e75 6d62 6572            Number
-000037f0: 206f 6620 636f 6e76 6572 7369 6f6e 7320   of conversions 
-00003800: 6174 7472 6962 7574 6564 2074 6f20 7468  attributed to th
-00003810: 6520 7072 6f64 7563 742c 2072 6570 6f72  e product, repor
-00003820: 7465 6420 6f6e 0a20 2020 2020 2020 2020  ted on.         
-00003830: 2020 2074 6865 2063 6f6e 7665 7273 696f     the conversio
-00003840: 6e20 6461 7465 2e20 4465 7065 6e64 696e  n date. Dependin
-00003850: 6720 6f6e 2074 6865 2061 7474 7269 6275  g on the attribu
-00003860: 7469 6f6e 206d 6f64 656c 2c20 610a 2020  tion model, a.  
-00003870: 2020 2020 2020 2020 2020 636f 6e76 6572            conver
-00003880: 7369 6f6e 206d 6967 6874 2062 6520 6469  sion might be di
-00003890: 7374 7269 6275 7465 6420 6163 726f 7373  stributed across
-000038a0: 206d 756c 7469 706c 6520 636c 6963 6b73   multiple clicks
-000038b0: 2c0a 2020 2020 2020 2020 2020 2020 7768  ,.            wh
-000038c0: 6572 6520 6561 6368 2063 6c69 636b 2067  ere each click g
-000038d0: 6574 7320 6974 7320 6f77 6e20 6372 6564  ets its own cred
-000038e0: 6974 2061 7373 6967 6e65 642e 2054 6869  it assigned. Thi
-000038f0: 7320 6d65 7472 6963 0a20 2020 2020 2020  s metric.       
-00003900: 2020 2020 2069 7320 6120 7375 6d20 6f66       is a sum of
-00003910: 2061 6c6c 2073 7563 6820 6372 6564 6974   all such credit
-00003920: 732e 204d 6574 7269 632e 0a0a 2020 2020  s. Metric...    
-00003930: 2020 2020 2020 2020 4176 6169 6c61 626c          Availabl
-00003940: 6520 6f6e 6c79 2066 6f72 2074 6865 2060  e only for the `
-00003950: 6046 5245 4560 6020 7472 6166 6669 6320  `FREE`` traffic 
-00003960: 736f 7572 6365 2e0a 0a20 2020 2020 2020  source...       
-00003970: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-00003980: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-00003990: 6f6e 656f 6660 5f20 6060 5f63 6f6e 7665  oneof`_ ``_conve
-000039a0: 7273 696f 6e73 6060 2e0a 2020 2020 2020  rsions``..      
-000039b0: 2020 636f 6e76 6572 7369 6f6e 5f76 616c    conversion_val
-000039c0: 7565 2028 676f 6f67 6c65 2e73 686f 7070  ue (google.shopp
-000039d0: 696e 672e 7479 7065 2e74 7970 6573 2e50  ing.type.types.P
-000039e0: 7269 6365 293a 0a20 2020 2020 2020 2020  rice):.         
-000039f0: 2020 2056 616c 7565 206f 6620 636f 6e76     Value of conv
-00003a00: 6572 7369 6f6e 7320 6174 7472 6962 7574  ersions attribut
-00003a10: 6564 2074 6f20 7468 6520 7072 6f64 7563  ed to the produc
-00003a20: 742c 2072 6570 6f72 7465 6420 6f6e 0a20  t, reported on. 
-00003a30: 2020 2020 2020 2020 2020 2074 6865 2063             the c
-00003a40: 6f6e 7665 7273 696f 6e20 6461 7465 2e20  onversion date. 
-00003a50: 4d65 7472 6963 2e0a 0a20 2020 2020 2020  Metric...       
-00003a60: 2020 2020 2041 7661 696c 6162 6c65 206f       Available o
-00003a70: 6e6c 7920 666f 7220 7468 6520 6060 4652  nly for the ``FR
-00003a80: 4545 6060 2074 7261 6666 6963 2073 6f75  EE`` traffic sou
-00003a90: 7263 652e 0a20 2020 2020 2020 2063 6f6e  rce..        con
-00003aa0: 7665 7273 696f 6e5f 7261 7465 2028 666c  version_rate (fl
-00003ab0: 6f61 7429 3a0a 2020 2020 2020 2020 2020  oat):.          
-00003ac0: 2020 4e75 6d62 6572 206f 6620 636f 6e76    Number of conv
-00003ad0: 6572 7369 6f6e 7320 6469 7669 6465 6420  ersions divided 
-00003ae0: 6279 2074 6865 206e 756d 6265 7220 6f66  by the number of
-00003af0: 2063 6c69 636b 732c 0a20 2020 2020 2020   clicks,.       
-00003b00: 2020 2020 2072 6570 6f72 7465 6420 6f6e       reported on
-00003b10: 2074 6865 2069 6d70 7265 7373 696f 6e20   the impression 
-00003b20: 6461 7465 2e20 4d65 7472 6963 2e0a 0a20  date. Metric... 
-00003b30: 2020 2020 2020 2020 2020 2041 7661 696c             Avail
-00003b40: 6162 6c65 206f 6e6c 7920 666f 7220 7468  able only for th
-00003b50: 6520 6060 4652 4545 6060 2074 7261 6666  e ``FREE`` traff
-00003b60: 6963 2073 6f75 7263 652e 0a0a 2020 2020  ic source...    
-00003b70: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-00003b80: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-00003b90: 6620 606f 6e65 6f66 605f 2060 605f 636f  f `oneof`_ ``_co
-00003ba0: 6e76 6572 7369 6f6e 5f72 6174 6560 602e  nversion_rate``.
-00003bb0: 0a20 2020 2022 2222 0a0a 2020 2020 6d61  .    """..    ma
-00003bc0: 726b 6574 696e 675f 6d65 7468 6f64 3a20  rketing_method: 
-00003bd0: 224d 6172 6b65 7469 6e67 4d65 7468 6f64  "MarketingMethod
-00003be0: 2e4d 6172 6b65 7469 6e67 4d65 7468 6f64  .MarketingMethod
-00003bf0: 456e 756d 2220 3d20 7072 6f74 6f2e 4669  Enum" = proto.Fi
-00003c00: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-00003c10: 746f 2e45 4e55 4d2c 0a20 2020 2020 2020  to.ENUM,.       
-00003c20: 206e 756d 6265 723d 312c 0a20 2020 2020   number=1,.     
-00003c30: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-00003c40: 2c0a 2020 2020 2020 2020 656e 756d 3d22  ,.        enum="
-00003c50: 4d61 726b 6574 696e 674d 6574 686f 642e  MarketingMethod.
-00003c60: 4d61 726b 6574 696e 674d 6574 686f 6445  MarketingMethodE
-00003c70: 6e75 6d22 2c0a 2020 2020 290a 2020 2020  num",.    ).    
-00003c80: 6461 7465 3a20 6461 7465 5f70 6232 2e44  date: date_pb2.D
-00003c90: 6174 6520 3d20 7072 6f74 6f2e 4669 656c  ate = proto.Fiel
-00003ca0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-00003cb0: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
-00003cc0: 2020 6e75 6d62 6572 3d32 2c0a 2020 2020    number=2,.    
-00003cd0: 2020 2020 6d65 7373 6167 653d 6461 7465      message=date
-00003ce0: 5f70 6232 2e44 6174 652c 0a20 2020 2029  _pb2.Date,.    )
-00003cf0: 0a20 2020 2077 6565 6b3a 2064 6174 655f  .    week: date_
-00003d00: 7062 322e 4461 7465 203d 2070 726f 746f  pb2.Date = proto
-00003d10: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00003d20: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
-00003d30: 2020 2020 2020 206e 756d 6265 723d 332c         number=3,
-00003d40: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-00003d50: 3d64 6174 655f 7062 322e 4461 7465 2c0a  =date_pb2.Date,.
-00003d60: 2020 2020 290a 2020 2020 6375 7374 6f6d      ).    custom
-00003d70: 6572 5f63 6f75 6e74 7279 5f63 6f64 653a  er_country_code:
-00003d80: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-00003d90: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00003da0: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-00003db0: 2020 6e75 6d62 6572 3d34 2c0a 2020 2020    number=4,.    
-00003dc0: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-00003dd0: 652c 0a20 2020 2029 0a20 2020 206f 6666  e,.    ).    off
-00003de0: 6572 5f69 643a 2073 7472 203d 2070 726f  er_id: str = pro
-00003df0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-00003e00: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
-00003e10: 2020 2020 2020 2020 6e75 6d62 6572 3d35          number=5
-00003e20: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-00003e30: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-00003e40: 2020 2074 6974 6c65 3a20 7374 7220 3d20     title: str = 
-00003e50: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00003e60: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-00003e70: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-00003e80: 723d 362c 0a20 2020 2020 2020 206f 7074  r=6,.        opt
-00003e90: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-00003ea0: 290a 2020 2020 6272 616e 643a 2073 7472  ).    brand: str
-00003eb0: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00003ec0: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
-00003ed0: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
-00003ee0: 6d62 6572 3d37 2c0a 2020 2020 2020 2020  mber=7,.        
-00003ef0: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
-00003f00: 2020 2029 0a20 2020 2063 6174 6567 6f72     ).    categor
-00003f10: 795f 6c31 3a20 7374 7220 3d20 7072 6f74  y_l1: str = prot
-00003f20: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00003f30: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-00003f40: 2020 2020 2020 206e 756d 6265 723d 382c         number=8,
-00003f50: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-00003f60: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-00003f70: 2020 6361 7465 676f 7279 5f6c 323a 2073    category_l2: s
-00003f80: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
-00003f90: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-00003fa0: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-00003fb0: 6e75 6d62 6572 3d39 2c0a 2020 2020 2020  number=9,.      
-00003fc0: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-00003fd0: 0a20 2020 2029 0a20 2020 2063 6174 6567  .    ).    categ
-00003fe0: 6f72 795f 6c33 3a20 7374 7220 3d20 7072  ory_l3: str = pr
-00003ff0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-00004000: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-00004010: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-00004020: 3130 2c0a 2020 2020 2020 2020 6f70 7469  10,.        opti
-00004030: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-00004040: 0a20 2020 2063 6174 6567 6f72 795f 6c34  .    category_l4
-00004050: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-00004060: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-00004070: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-00004080: 2020 206e 756d 6265 723d 3131 2c0a 2020     number=11,.  
-00004090: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-000040a0: 7275 652c 0a20 2020 2029 0a20 2020 2063  rue,.    ).    c
-000040b0: 6174 6567 6f72 795f 6c35 3a20 7374 7220  ategory_l5: str 
-000040c0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-000040d0: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-000040e0: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-000040f0: 6265 723d 3132 2c0a 2020 2020 2020 2020  ber=12,.        
-00004100: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
-00004110: 2020 2029 0a20 2020 2070 726f 6475 6374     ).    product
-00004120: 5f74 7970 655f 6c31 3a20 7374 7220 3d20  _type_l1: str = 
-00004130: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00004140: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-00004150: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-00004160: 723d 3133 2c0a 2020 2020 2020 2020 6f70  r=13,.        op
-00004170: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-00004180: 2029 0a20 2020 2070 726f 6475 6374 5f74   ).    product_t
-00004190: 7970 655f 6c32 3a20 7374 7220 3d20 7072  ype_l2: str = pr
-000041a0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-000041b0: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-000041c0: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-000041d0: 3134 2c0a 2020 2020 2020 2020 6f70 7469  14,.        opti
-000041e0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-000041f0: 0a20 2020 2070 726f 6475 6374 5f74 7970  .    product_typ
-00004200: 655f 6c33 3a20 7374 7220 3d20 7072 6f74  e_l3: str = prot
-00004210: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00004220: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-00004230: 2020 2020 2020 206e 756d 6265 723d 3135         number=15
-00004240: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-00004250: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-00004260: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
-00004270: 6c34 3a20 7374 7220 3d20 7072 6f74 6f2e  l4: str = proto.
-00004280: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00004290: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-000042a0: 2020 2020 206e 756d 6265 723d 3136 2c0a       number=16,.
-000042b0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-000042c0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-000042d0: 2070 726f 6475 6374 5f74 7970 655f 6c35   product_type_l5
-000042e0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-000042f0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-00004300: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-00004310: 2020 206e 756d 6265 723d 3137 2c0a 2020     number=17,.  
-00004320: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-00004330: 7275 652c 0a20 2020 2029 0a20 2020 2063  rue,.    ).    c
-00004340: 7573 746f 6d5f 6c61 6265 6c30 3a20 7374  ustom_label0: st
-00004350: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-00004360: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-00004370: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-00004380: 756d 6265 723d 3138 2c0a 2020 2020 2020  umber=18,.      
-00004390: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-000043a0: 0a20 2020 2029 0a20 2020 2063 7573 746f  .    ).    custo
-000043b0: 6d5f 6c61 6265 6c31 3a20 7374 7220 3d20  m_label1: str = 
-000043c0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-000043d0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-000043e0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-000043f0: 723d 3139 2c0a 2020 2020 2020 2020 6f70  r=19,.        op
-00004400: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-00004410: 2029 0a20 2020 2063 7573 746f 6d5f 6c61   ).    custom_la
-00004420: 6265 6c32 3a20 7374 7220 3d20 7072 6f74  bel2: str = prot
-00004430: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00004440: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-00004450: 2020 2020 2020 206e 756d 6265 723d 3230         number=20
-00004460: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-00004470: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-00004480: 2020 2063 7573 746f 6d5f 6c61 6265 6c33     custom_label3
-00004490: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-000044a0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-000044b0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-000044c0: 2020 206e 756d 6265 723d 3231 2c0a 2020     number=21,.  
-000044d0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-000044e0: 7275 652c 0a20 2020 2029 0a20 2020 2063  rue,.    ).    c
-000044f0: 7573 746f 6d5f 6c61 6265 6c34 3a20 7374  ustom_label4: st
-00004500: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-00004510: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-00004520: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-00004530: 756d 6265 723d 3232 2c0a 2020 2020 2020  umber=22,.      
-00004540: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-00004550: 0a20 2020 2029 0a20 2020 2063 6c69 636b  .    ).    click
-00004560: 733a 2069 6e74 203d 2070 726f 746f 2e46  s: int = proto.F
-00004570: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-00004580: 6f74 6f2e 494e 5436 342c 0a20 2020 2020  oto.INT64,.     
-00004590: 2020 206e 756d 6265 723d 3233 2c0a 2020     number=23,.  
-000045a0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-000045b0: 7275 652c 0a20 2020 2029 0a20 2020 2069  rue,.    ).    i
-000045c0: 6d70 7265 7373 696f 6e73 3a20 696e 7420  mpressions: int 
-000045d0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-000045e0: 2020 2020 2020 2070 726f 746f 2e49 4e54         proto.INT
-000045f0: 3634 2c0a 2020 2020 2020 2020 6e75 6d62  64,.        numb
-00004600: 6572 3d32 342c 0a20 2020 2020 2020 206f  er=24,.        o
-00004610: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-00004620: 2020 290a 2020 2020 636c 6963 6b5f 7468    ).    click_th
-00004630: 726f 7567 685f 7261 7465 3a20 666c 6f61  rough_rate: floa
-00004640: 7420 3d20 7072 6f74 6f2e 4669 656c 6428  t = proto.Field(
-00004650: 0a20 2020 2020 2020 2070 726f 746f 2e44  .        proto.D
-00004660: 4f55 424c 452c 0a20 2020 2020 2020 206e  OUBLE,.        n
-00004670: 756d 6265 723d 3235 2c0a 2020 2020 2020  umber=25,.      
-00004680: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-00004690: 0a20 2020 2029 0a20 2020 2063 6f6e 7665  .    ).    conve
-000046a0: 7273 696f 6e73 3a20 666c 6f61 7420 3d20  rsions: float = 
-000046b0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-000046c0: 2020 2020 2070 726f 746f 2e44 4f55 424c       proto.DOUBL
-000046d0: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
-000046e0: 723d 3236 2c0a 2020 2020 2020 2020 6f70  r=26,.        op
-000046f0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-00004700: 2029 0a20 2020 2063 6f6e 7665 7273 696f   ).    conversio
-00004710: 6e5f 7661 6c75 653a 2074 7970 6573 2e50  n_value: types.P
-00004720: 7269 6365 203d 2070 726f 746f 2e46 6965  rice = proto.Fie
-00004730: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00004740: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
-00004750: 2020 206e 756d 6265 723d 3237 2c0a 2020     number=27,.  
-00004760: 2020 2020 2020 6d65 7373 6167 653d 7479        message=ty
-00004770: 7065 732e 5072 6963 652c 0a20 2020 2029  pes.Price,.    )
-00004780: 0a20 2020 2063 6f6e 7665 7273 696f 6e5f  .    conversion_
-00004790: 7261 7465 3a20 666c 6f61 7420 3d20 7072  rate: float = pr
-000047a0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-000047b0: 2020 2070 726f 746f 2e44 4f55 424c 452c     proto.DOUBLE,
-000047c0: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-000047d0: 3238 2c0a 2020 2020 2020 2020 6f70 7469  28,.        opti
-000047e0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-000047f0: 0a0a 0a63 6c61 7373 2050 726f 6475 6374  ...class Product
-00004800: 5669 6577 2870 726f 746f 2e4d 6573 7361  View(proto.Messa
-00004810: 6765 293a 0a20 2020 2072 2222 2246 6965  ge):.    r"""Fie
-00004820: 6c64 7320 6176 6169 6c61 626c 6520 666f  lds available fo
-00004830: 7220 7175 6572 7920 696e 2060 6070 726f  r query in ``pro
-00004840: 6475 6374 5f76 6965 7760 6020 7461 626c  duct_view`` tabl
-00004850: 652e 0a0a 2020 2020 5072 6f64 7563 7473  e...    Products
-00004860: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
-00004870: 696e 7665 6e74 6f72 792e 2050 726f 6475  inventory. Produ
-00004880: 6374 7320 696e 2074 6869 7320 7461 626c  cts in this tabl
-00004890: 6520 6172 6520 7468 650a 2020 2020 7361  e are the.    sa
-000048a0: 6d65 2061 7320 696e 2050 726f 6475 6374  me as in Product
-000048b0: 7320 7375 622d 4150 4920 6275 7420 6e6f  s sub-API but no
-000048c0: 7420 616c 6c20 7072 6f64 7563 7420 6174  t all product at
-000048d0: 7472 6962 7574 6573 2066 726f 6d0a 2020  tributes from.  
-000048e0: 2020 5072 6f64 7563 7473 2073 7562 2d41    Products sub-A
-000048f0: 5049 2061 7265 2061 7661 696c 6162 6c65  PI are available
-00004900: 2066 6f72 2071 7565 7279 2069 6e20 7468   for query in th
-00004910: 6973 2074 6162 6c65 2e20 496e 2063 6f6e  is table. In con
-00004920: 7472 6173 740a 2020 2020 746f 2050 726f  trast.    to Pro
-00004930: 6475 6374 7320 7375 622d 4150 492c 2074  ducts sub-API, t
-00004940: 6869 7320 7461 626c 6520 616c 6c6f 7773  his table allows
-00004950: 2074 6f20 6669 6c74 6572 2074 6865 2072   to filter the r
-00004960: 6574 7572 6e65 6420 6c69 7374 0a20 2020  eturned list.   
-00004970: 206f 6620 7072 6f64 7563 7473 2062 7920   of products by 
-00004980: 7072 6f64 7563 7420 6174 7472 6962 7574  product attribut
-00004990: 6573 2e20 546f 2072 6574 7269 6576 6520  es. To retrieve 
-000049a0: 6120 7369 6e67 6c65 2070 726f 6475 6374  a single product
-000049b0: 2062 790a 2020 2020 6060 6964 6060 206f   by.    ``id`` o
-000049c0: 7220 6c69 7374 2061 6c6c 2070 726f 6475  r list all produ
-000049d0: 6374 732c 2050 726f 6475 6374 7320 7375  cts, Products su
-000049e0: 622d 4150 4920 7368 6f75 6c64 2062 6520  b-API should be 
-000049f0: 7573 6564 2e0a 0a20 2020 2056 616c 7565  used...    Value
-00004a00: 7320 6172 6520 6f6e 6c79 2073 6574 2066  s are only set f
-00004a10: 6f72 2066 6965 6c64 7320 7265 7175 6573  or fields reques
-00004a20: 7465 6420 6578 706c 6963 6974 6c79 2069  ted explicitly i
-00004a30: 6e20 7468 6520 7265 7175 6573 7427 730a  n the request's.
-00004a40: 2020 2020 7365 6172 6368 2071 7565 7279      search query
-00004a50: 2e0a 0a0a 2020 2020 2e2e 205f 6f6e 656f  ....    .. _oneo
-00004a60: 663a 2068 7474 7073 3a2f 2f70 726f 746f  f: https://proto
-00004a70: 2d70 6c75 732d 7079 7468 6f6e 2e72 6561  -plus-python.rea
-00004a80: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
-00004a90: 7461 626c 652f 6669 656c 6473 2e68 746d  table/fields.htm
-00004aa0: 6c23 6f6e 656f 6673 2d6d 7574 7561 6c6c  l#oneofs-mutuall
-00004ab0: 792d 6578 636c 7573 6976 652d 6669 656c  y-exclusive-fiel
-00004ac0: 6473 0a0a 2020 2020 4174 7472 6962 7574  ds..    Attribut
-00004ad0: 6573 3a0a 2020 2020 2020 2020 6964 2028  es:.        id (
-00004ae0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00004af0: 2020 5245 5354 2049 4420 6f66 2074 6865    REST ID of the
-00004b00: 2070 726f 6475 6374 2c20 696e 2074 6865   product, in the
-00004b10: 2066 6f72 6d20 6f66 0a20 2020 2020 2020   form of.       
-00004b20: 2020 2020 2060 6063 6861 6e6e 656c 7e6c       ``channel~l
-00004b30: 616e 6775 6167 6543 6f64 657e 6665 6564  anguageCode~feed
-00004b40: 4c61 6265 6c7e 6f66 6665 7249 6460 602e  Label~offerId``.
-00004b50: 204d 6572 6368 616e 7420 4150 490a 2020   Merchant API.  
-00004b60: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
-00004b70: 7320 7468 6174 206f 7065 7261 7465 206f  s that operate o
-00004b80: 6e20 7072 6f64 7563 7473 2074 616b 6520  n products take 
-00004b90: 7468 6973 2061 7320 7468 6569 7220 6060  this as their ``
-00004ba0: 6e61 6d65 6060 0a20 2020 2020 2020 2020  name``.         
-00004bb0: 2020 2070 6172 616d 6574 6572 2e0a 0a20     parameter... 
-00004bc0: 2020 2020 2020 2020 2020 2052 6571 7569             Requi
-00004bd0: 7265 6420 696e 2074 6865 2060 6053 454c  red in the ``SEL
-00004be0: 4543 5460 6020 636c 6175 7365 2e0a 0a20  ECT`` clause... 
-00004bf0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00004c00: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00004c10: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00004c20: 5f69 6460 602e 0a20 2020 2020 2020 2063  _id``..        c
-00004c30: 6861 6e6e 656c 2028 676f 6f67 6c65 2e73  hannel (google.s
-00004c40: 686f 7070 696e 672e 7479 7065 2e74 7970  hopping.type.typ
-00004c50: 6573 2e43 6861 6e6e 656c 2e43 6861 6e6e  es.Channel.Chann
-00004c60: 656c 456e 756d 293a 0a20 2020 2020 2020  elEnum):.       
-00004c70: 2020 2020 2043 6861 6e6e 656c 206f 6620       Channel of 
-00004c80: 7468 6520 7072 6f64 7563 742e 2043 616e  the product. Can
-00004c90: 2062 6520 6060 4f4e 4c49 4e45 6060 206f   be ``ONLINE`` o
-00004ca0: 7220 6060 4c4f 4341 4c60 602e 0a0a 2020  r ``LOCAL``...  
-00004cb0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00004cc0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-00004cd0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-00004ce0: 6368 616e 6e65 6c60 602e 0a20 2020 2020  channel``..     
-00004cf0: 2020 206c 616e 6775 6167 655f 636f 6465     language_code
-00004d00: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
-00004d10: 2020 2020 4c61 6e67 7561 6765 2063 6f64      Language cod
-00004d20: 6520 6f66 2074 6865 2070 726f 6475 6374  e of the product
-00004d30: 2069 6e20 4243 5020 3437 0a20 2020 2020   in BCP 47.     
-00004d40: 2020 2020 2020 2066 6f72 6d61 742e 0a0a         format...
-00004d50: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00004d60: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00004d70: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00004d80: 605f 6c61 6e67 7561 6765 5f63 6f64 6560  `_language_code`
-00004d90: 602e 0a20 2020 2020 2020 2066 6565 645f  `..        feed_
-00004da0: 6c61 6265 6c20 2873 7472 293a 0a20 2020  label (str):.   
-00004db0: 2020 2020 2020 2020 2046 6565 6420 6c61           Feed la
-00004dc0: 6265 6c20 6f66 2074 6865 2070 726f 6475  bel of the produ
-00004dd0: 6374 2e0a 0a20 2020 2020 2020 2020 2020  ct...           
-00004de0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-00004df0: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-00004e00: 6660 5f20 6060 5f66 6565 645f 6c61 6265  f`_ ``_feed_labe
-00004e10: 6c60 602e 0a20 2020 2020 2020 206f 6666  l``..        off
-00004e20: 6572 5f69 6420 2873 7472 293a 0a20 2020  er_id (str):.   
-00004e30: 2020 2020 2020 2020 204d 6572 6368 616e           Merchan
-00004e40: 742d 7072 6f76 6964 6564 2069 6420 6f66  t-provided id of
-00004e50: 2074 6865 2070 726f 6475 6374 2e0a 0a20   the product... 
-00004e60: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00004e70: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00004e80: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-00004e90: 5f6f 6666 6572 5f69 6460 602e 0a20 2020  _offer_id``..   
-00004ea0: 2020 2020 2074 6974 6c65 2028 7374 7229       title (str)
-00004eb0: 3a0a 2020 2020 2020 2020 2020 2020 5469  :.            Ti
-00004ec0: 746c 6520 6f66 2074 6865 2070 726f 6475  tle of the produ
-00004ed0: 6374 2e0a 0a20 2020 2020 2020 2020 2020  ct...           
-00004ee0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-00004ef0: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-00004f00: 6660 5f20 6060 5f74 6974 6c65 6060 2e0a  f`_ ``_title``..
-00004f10: 2020 2020 2020 2020 6272 616e 6420 2873          brand (s
-00004f20: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00004f30: 2042 7261 6e64 206f 6620 7468 6520 7072   Brand of the pr
-00004f40: 6f64 7563 742e 0a0a 2020 2020 2020 2020  oduct...        
-00004f50: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-00004f60: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-00004f70: 6e65 6f66 605f 2060 605f 6272 616e 6460  neof`_ ``_brand`
-00004f80: 602e 0a20 2020 2020 2020 2063 6174 6567  `..        categ
-00004f90: 6f72 795f 6c31 2028 7374 7229 3a0a 2020  ory_l1 (str):.  
-00004fa0: 2020 2020 2020 2020 2020 5072 6f64 7563            Produc
-00004fb0: 7420 6361 7465 676f 7279 2028 3173 7420  t category (1st 
-00004fc0: 6c65 7665 6c29 2069 6e20 6047 6f6f 676c  level) in `Googl
-00004fd0: 6527 7320 7072 6f64 7563 740a 2020 2020  e's product.    
-00004fe0: 2020 2020 2020 2020 7461 786f 6e6f 6d79          taxonomy
-00004ff0: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
-00005000: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
-00005010: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
-00005020: 3234 3433 363e 605f 5f2e 0a0a 2020 2020  24436>`__...    
-00005030: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-00005040: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-00005050: 6620 606f 6e65 6f66 605f 2060 605f 6361  f `oneof`_ ``_ca
-00005060: 7465 676f 7279 5f6c 3160 602e 0a20 2020  tegory_l1``..   
-00005070: 2020 2020 2063 6174 6567 6f72 795f 6c32       category_l2
-00005080: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
-00005090: 2020 2020 5072 6f64 7563 7420 6361 7465      Product cate
-000050a0: 676f 7279 2028 326e 6420 6c65 7665 6c29  gory (2nd level)
-000050b0: 2069 6e20 6047 6f6f 676c 6527 7320 7072   in `Google's pr
-000050c0: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
-000050d0: 2020 7461 786f 6e6f 6d79 203c 6874 7470    taxonomy <http
-000050e0: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
-000050f0: 6c65 2e63 6f6d 2f6d 6572 6368 616e 7473  le.com/merchants
-00005100: 2f61 6e73 7765 722f 3633 3234 3433 363e  /answer/6324436>
-00005110: 605f 5f2e 0a0a 2020 2020 2020 2020 2020  `__...          
-00005120: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00005130: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00005140: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
-00005150: 5f6c 3260 602e 0a20 2020 2020 2020 2063  _l2``..        c
-00005160: 6174 6567 6f72 795f 6c33 2028 7374 7229  ategory_l3 (str)
-00005170: 3a0a 2020 2020 2020 2020 2020 2020 5072  :.            Pr
-00005180: 6f64 7563 7420 6361 7465 676f 7279 2028  oduct category (
-00005190: 3372 6420 6c65 7665 6c29 2069 6e20 6047  3rd level) in `G
-000051a0: 6f6f 676c 6527 7320 7072 6f64 7563 740a  oogle's product.
-000051b0: 2020 2020 2020 2020 2020 2020 7461 786f              taxo
-000051c0: 6e6f 6d79 203c 6874 7470 733a 2f2f 7375  nomy <https://su
-000051d0: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
-000051e0: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
-000051f0: 722f 3633 3234 3433 363e 605f 5f2e 0a0a  r/6324436>`__...
-00005200: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00005210: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00005220: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00005230: 605f 6361 7465 676f 7279 5f6c 3360 602e  `_category_l3``.
-00005240: 0a20 2020 2020 2020 2063 6174 6567 6f72  .        categor
-00005250: 795f 6c34 2028 7374 7229 3a0a 2020 2020  y_l4 (str):.    
-00005260: 2020 2020 2020 2020 5072 6f64 7563 7420          Product 
-00005270: 6361 7465 676f 7279 2028 3474 6820 6c65  category (4th le
-00005280: 7665 6c29 2069 6e20 6047 6f6f 676c 6527  vel) in `Google'
-00005290: 7320 7072 6f64 7563 740a 2020 2020 2020  s product.      
-000052a0: 2020 2020 2020 7461 786f 6e6f 6d79 203c        taxonomy <
-000052b0: 6874 7470 733a 2f2f 7375 7070 6f72 742e  https://support.
-000052c0: 676f 6f67 6c65 2e63 6f6d 2f6d 6572 6368  google.com/merch
-000052d0: 616e 7473 2f61 6e73 7765 722f 3633 3234  ants/answer/6324
-000052e0: 3433 363e 605f 5f2e 0a0a 2020 2020 2020  436>`__...      
-000052f0: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-00005300: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-00005310: 606f 6e65 6f66 605f 2060 605f 6361 7465  `oneof`_ ``_cate
-00005320: 676f 7279 5f6c 3460 602e 0a20 2020 2020  gory_l4``..     
-00005330: 2020 2063 6174 6567 6f72 795f 6c35 2028     category_l5 (
-00005340: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00005350: 2020 5072 6f64 7563 7420 6361 7465 676f    Product catego
-00005360: 7279 2028 3574 6820 6c65 7665 6c29 2069  ry (5th level) i
-00005370: 6e20 6047 6f6f 676c 6527 7320 7072 6f64  n `Google's prod
-00005380: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
-00005390: 7461 786f 6e6f 6d79 203c 6874 7470 733a  taxonomy <https:
-000053a0: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
-000053b0: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
-000053c0: 6e73 7765 722f 3633 3234 3433 363e 605f  nswer/6324436>`_
-000053d0: 5f2e 0a0a 2020 2020 2020 2020 2020 2020  _...            
-000053e0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-000053f0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-00005400: 605f 2060 605f 6361 7465 676f 7279 5f6c  `_ ``_category_l
-00005410: 3560 602e 0a20 2020 2020 2020 2070 726f  5``..        pro
-00005420: 6475 6374 5f74 7970 655f 6c31 2028 7374  duct_type_l1 (st
-00005430: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00005440: 5072 6f64 7563 7420 7479 7065 2028 3173  Product type (1s
-00005450: 7420 6c65 7665 6c29 2069 6e20 6d65 7263  t level) in merc
-00005460: 6861 6e74 2773 206f 776e 2060 7072 6f64  hant's own `prod
-00005470: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
-00005480: 7461 786f 6e6f 6d79 203c 6874 7470 733a  taxonomy <https:
-00005490: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
-000054a0: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
-000054b0: 6e73 7765 722f 3633 3234 3430 363e 605f  nswer/6324406>`_
-000054c0: 5f2e 0a0a 2020 2020 2020 2020 2020 2020  _...            
-000054d0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-000054e0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-000054f0: 605f 2060 605f 7072 6f64 7563 745f 7479  `_ ``_product_ty
-00005500: 7065 5f6c 3160 602e 0a20 2020 2020 2020  pe_l1``..       
-00005510: 2070 726f 6475 6374 5f74 7970 655f 6c32   product_type_l2
-00005520: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
-00005530: 2020 2020 5072 6f64 7563 7420 7479 7065      Product type
-00005540: 2028 326e 6420 6c65 7665 6c29 2069 6e20   (2nd level) in 
-00005550: 6d65 7263 6861 6e74 2773 206f 776e 2060  merchant's own `
-00005560: 7072 6f64 7563 740a 2020 2020 2020 2020  product.        
-00005570: 2020 2020 7461 786f 6e6f 6d79 203c 6874      taxonomy <ht
-00005580: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
-00005590: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
-000055a0: 7473 2f61 6e73 7765 722f 3633 3234 3430  ts/answer/632440
-000055b0: 363e 605f 5f2e 0a0a 2020 2020 2020 2020  6>`__...        
-000055c0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-000055d0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-000055e0: 6e65 6f66 605f 2060 605f 7072 6f64 7563  neof`_ ``_produc
-000055f0: 745f 7479 7065 5f6c 3260 602e 0a20 2020  t_type_l2``..   
-00005600: 2020 2020 2070 726f 6475 6374 5f74 7970       product_typ
-00005610: 655f 6c33 2028 7374 7229 3a0a 2020 2020  e_l3 (str):.    
-00005620: 2020 2020 2020 2020 5072 6f64 7563 7420          Product 
-00005630: 7479 7065 2028 3372 6420 6c65 7665 6c29  type (3rd level)
-00005640: 2069 6e20 6d65 7263 6861 6e74 2773 206f   in merchant's o
-00005650: 776e 2060 7072 6f64 7563 740a 2020 2020  wn `product.    
-00005660: 2020 2020 2020 2020 7461 786f 6e6f 6d79          taxonomy
-00005670: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
-00005680: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
-00005690: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
-000056a0: 3234 3430 363e 605f 5f2e 0a0a 2020 2020  24406>`__...    
-000056b0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-000056c0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-000056d0: 6620 606f 6e65 6f66 605f 2060 605f 7072  f `oneof`_ ``_pr
-000056e0: 6f64 7563 745f 7479 7065 5f6c 3360 602e  oduct_type_l3``.
-000056f0: 0a20 2020 2020 2020 2070 726f 6475 6374  .        product
-00005700: 5f74 7970 655f 6c34 2028 7374 7229 3a0a  _type_l4 (str):.
-00005710: 2020 2020 2020 2020 2020 2020 5072 6f64              Prod
-00005720: 7563 7420 7479 7065 2028 3474 6820 6c65  uct type (4th le
-00005730: 7665 6c29 2069 6e20 6d65 7263 6861 6e74  vel) in merchant
-00005740: 2773 206f 776e 2060 7072 6f64 7563 740a  's own `product.
-00005750: 2020 2020 2020 2020 2020 2020 7461 786f              taxo
-00005760: 6e6f 6d79 203c 6874 7470 733a 2f2f 7375  nomy <https://su
-00005770: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
-00005780: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
-00005790: 722f 3633 3234 3430 363e 605f 5f2e 0a0a  r/6324406>`__...
-000057a0: 2020 2020 2020 2020 2020 2020 5468 6973              This
-000057b0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-000057c0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-000057d0: 605f 7072 6f64 7563 745f 7479 7065 5f6c  `_product_type_l
-000057e0: 3460 602e 0a20 2020 2020 2020 2070 726f  4``..        pro
-000057f0: 6475 6374 5f74 7970 655f 6c35 2028 7374  duct_type_l5 (st
-00005800: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00005810: 5072 6f64 7563 7420 7479 7065 2028 3574  Product type (5t
-00005820: 6820 6c65 7665 6c29 2069 6e20 6d65 7263  h level) in merc
-00005830: 6861 6e74 2773 206f 776e 2060 7072 6f64  hant's own `prod
-00005840: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
-00005850: 7461 786f 6e6f 6d79 203c 6874 7470 733a  taxonomy <https:
-00005860: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
-00005870: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
-00005880: 6e73 7765 722f 3633 3234 3430 363e 605f  nswer/6324406>`_
-00005890: 5f2e 0a0a 2020 2020 2020 2020 2020 2020  _...            
-000058a0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-000058b0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-000058c0: 605f 2060 605f 7072 6f64 7563 745f 7479  `_ ``_product_ty
-000058d0: 7065 5f6c 3560 602e 0a20 2020 2020 2020  pe_l5``..       
-000058e0: 2070 7269 6365 2028 676f 6f67 6c65 2e73   price (google.s
-000058f0: 686f 7070 696e 672e 7479 7065 2e74 7970  hopping.type.typ
-00005900: 6573 2e50 7269 6365 293a 0a20 2020 2020  es.Price):.     
-00005910: 2020 2020 2020 2050 726f 6475 6374 2070         Product p
-00005920: 7269 6365 2e20 4162 7365 6e74 2069 6620  rice. Absent if 
-00005930: 7468 6520 696e 666f 726d 6174 696f 6e0a  the information.
-00005940: 2020 2020 2020 2020 2020 2020 6162 6f75              abou
-00005950: 7420 7468 6520 7072 6963 6520 6f66 2074  t the price of t
-00005960: 6865 2070 726f 6475 6374 2069 7320 6e6f  he product is no
-00005970: 7420 6176 6169 6c61 626c 652e 0a20 2020  t available..   
-00005980: 2020 2020 2063 6f6e 6469 7469 6f6e 2028       condition (
-00005990: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-000059a0: 2020 6043 6f6e 6469 7469 6f6e 203c 6874    `Condition <ht
-000059b0: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
-000059c0: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
-000059d0: 7473 2f61 6e73 7765 722f 3633 3234 3436  ts/answer/632446
-000059e0: 393e 605f 5f0a 2020 2020 2020 2020 2020  9>`__.          
-000059f0: 2020 6f66 2074 6865 2070 726f 6475 6374    of the product
-00005a00: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-00005a10: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-00005a20: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-00005a30: 5f20 6060 5f63 6f6e 6469 7469 6f6e 6060  _ ``_condition``
-00005a40: 2e0a 2020 2020 2020 2020 6176 6169 6c61  ..        availa
-00005a50: 6269 6c69 7479 2028 7374 7229 3a0a 2020  bility (str):.  
-00005a60: 2020 2020 2020 2020 2020 6041 7661 696c            `Avail
-00005a70: 6162 696c 6974 7920 3c68 7474 7073 3a2f  ability <https:/
-00005a80: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
-00005a90: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
-00005aa0: 7377 6572 2f36 3332 3434 3438 3e60 5f5f  swer/6324448>`__
-00005ab0: 0a20 2020 2020 2020 2020 2020 206f 6620  .            of 
-00005ac0: 7468 6520 7072 6f64 7563 742e 0a0a 2020  the product...  
-00005ad0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00005ae0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-00005af0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-00005b00: 6176 6169 6c61 6269 6c69 7479 6060 2e0a  availability``..
-00005b10: 2020 2020 2020 2020 7368 6970 7069 6e67          shipping
-00005b20: 5f6c 6162 656c 2028 7374 7229 3a0a 2020  _label (str):.  
-00005b30: 2020 2020 2020 2020 2020 4e6f 726d 616c            Normal
-00005b40: 697a 6564 2060 7368 6970 7069 6e67 0a20  ized `shipping. 
-00005b50: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00005b60: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
-00005b70: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
-00005b80: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
-00005b90: 3234 3530 343e 605f 5f0a 2020 2020 2020  24504>`__.      
-00005ba0: 2020 2020 2020 7370 6563 6966 6965 6420        specified 
-00005bb0: 696e 2074 6865 2066 6565 642e 0a0a 2020  in the feed...  
-00005bc0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00005bd0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-00005be0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-00005bf0: 7368 6970 7069 6e67 5f6c 6162 656c 6060  shipping_label``
-00005c00: 2e0a 2020 2020 2020 2020 6774 696e 2028  ..        gtin (
-00005c10: 4d75 7461 626c 6553 6571 7565 6e63 655b  MutableSequence[
-00005c20: 7374 725d 293a 0a20 2020 2020 2020 2020  str]):.         
-00005c30: 2020 204c 6973 7420 6f66 2047 6c6f 6261     List of Globa
-00005c40: 6c20 5472 6164 6520 4974 656d 204e 756d  l Trade Item Num
-00005c50: 6265 7273 2028 4754 494e 7329 206f 660a  bers (GTINs) of.
-00005c60: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00005c70: 7072 6f64 7563 742e 0a20 2020 2020 2020  product..       
-00005c80: 2069 7465 6d5f 6772 6f75 705f 6964 2028   item_group_id (
-00005c90: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00005ca0: 2020 4974 656d 2067 726f 7570 2069 6420    Item group id 
-00005cb0: 7072 6f76 6964 6564 2062 7920 7468 6520  provided by the 
-00005cc0: 6d65 7263 6861 6e74 2066 6f72 0a20 2020  merchant for.   
-00005cd0: 2020 2020 2020 2020 2067 726f 7570 696e           groupin
-00005ce0: 6720 7661 7269 616e 7473 2074 6f67 6574  g variants toget
-00005cf0: 6865 722e 0a0a 2020 2020 2020 2020 2020  her...          
-00005d00: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00005d10: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00005d20: 6f66 605f 2060 605f 6974 656d 5f67 726f  of`_ ``_item_gro
-00005d30: 7570 5f69 6460 602e 0a20 2020 2020 2020  up_id``..       
-00005d40: 2074 6875 6d62 6e61 696c 5f6c 696e 6b20   thumbnail_link 
-00005d50: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-00005d60: 2020 204c 696e 6b20 746f 2074 6865 2070     Link to the p
-00005d70: 726f 6365 7373 6564 2069 6d61 6765 206f  rocessed image o
-00005d80: 6620 7468 6520 7072 6f64 7563 742c 0a20  f the product,. 
-00005d90: 2020 2020 2020 2020 2020 2068 6f73 7465             hoste
-00005da0: 6420 6f6e 2074 6865 2047 6f6f 676c 6520  d on the Google 
-00005db0: 696e 6672 6173 7472 7563 7475 7265 2e0a  infrastructure..
-00005dc0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-00005dd0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-00005de0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-00005df0: 6060 5f74 6875 6d62 6e61 696c 5f6c 696e  ``_thumbnail_lin
-00005e00: 6b60 602e 0a20 2020 2020 2020 2063 7265  k``..        cre
-00005e10: 6174 696f 6e5f 7469 6d65 2028 676f 6f67  ation_time (goog
-00005e20: 6c65 2e70 726f 746f 6275 662e 7469 6d65  le.protobuf.time
-00005e30: 7374 616d 705f 7062 322e 5469 6d65 7374  stamp_pb2.Timest
-00005e40: 616d 7029 3a0a 2020 2020 2020 2020 2020  amp):.          
-00005e50: 2020 5468 6520 7469 6d65 2074 6865 206d    The time the m
-00005e60: 6572 6368 616e 7420 6372 6561 7465 6420  erchant created 
-00005e70: 7468 6520 7072 6f64 7563 7420 696e 0a20  the product in. 
-00005e80: 2020 2020 2020 2020 2020 2074 696d 6573             times
-00005e90: 7461 6d70 2073 6563 6f6e 6473 2e0a 2020  tamp seconds..  
-00005ea0: 2020 2020 2020 6578 7069 7261 7469 6f6e        expiration
-00005eb0: 5f64 6174 6520 2867 6f6f 676c 652e 7479  _date (google.ty
-00005ec0: 7065 2e64 6174 655f 7062 322e 4461 7465  pe.date_pb2.Date
-00005ed0: 293a 0a20 2020 2020 2020 2020 2020 2045  ):.            E
-00005ee0: 7870 6972 6174 696f 6e20 6461 7465 2066  xpiration date f
-00005ef0: 6f72 2074 6865 2070 726f 6475 6374 2c20  or the product, 
-00005f00: 7370 6563 6966 6965 6420 6f6e 0a20 2020  specified on.   
-00005f10: 2020 2020 2020 2020 2069 6e73 6572 7469           inserti
-00005f20: 6f6e 2e0a 2020 2020 2020 2020 6167 6772  on..        aggr
-00005f30: 6567 6174 6564 5f72 6570 6f72 7469 6e67  egated_reporting
-00005f40: 5f63 6f6e 7465 7874 5f73 7461 7475 7320  _context_status 
-00005f50: 2867 6f6f 676c 652e 7368 6f70 7069 6e67  (google.shopping
-00005f60: 2e6d 6572 6368 616e 745f 7265 706f 7274  .merchant_report
-00005f70: 735f 7631 6265 7461 2e74 7970 6573 2e50  s_v1beta.types.P
-00005f80: 726f 6475 6374 5669 6577 2e41 6767 7265  roductView.Aggre
-00005f90: 6761 7465 6452 6570 6f72 7469 6e67 436f  gatedReportingCo
-00005fa0: 6e74 6578 7453 7461 7475 7329 3a0a 2020  ntextStatus):.  
-00005fb0: 2020 2020 2020 2020 2020 4167 6772 6567            Aggreg
-00005fc0: 6174 6564 2073 7461 7475 732e 0a0a 2020  ated status...  
-00005fd0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00005fe0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-00005ff0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-00006000: 6167 6772 6567 6174 6564 5f72 6570 6f72  aggregated_repor
-00006010: 7469 6e67 5f63 6f6e 7465 7874 5f73 7461  ting_context_sta
-00006020: 7475 7360 602e 0a20 2020 2020 2020 2069  tus``..        i
-00006030: 7465 6d5f 6973 7375 6573 2028 4d75 7461  tem_issues (Muta
-00006040: 626c 6553 6571 7565 6e63 655b 676f 6f67  bleSequence[goog
-00006050: 6c65 2e73 686f 7070 696e 672e 6d65 7263  le.shopping.merc
-00006060: 6861 6e74 5f72 6570 6f72 7473 5f76 3162  hant_reports_v1b
-00006070: 6574 612e 7479 7065 732e 5072 6f64 7563  eta.types.Produc
-00006080: 7456 6965 772e 4974 656d 4973 7375 655d  tView.ItemIssue]
-00006090: 293a 0a20 2020 2020 2020 2020 2020 204c  ):.            L
-000060a0: 6973 7420 6f66 2069 7465 6d20 6973 7375  ist of item issu
-000060b0: 6573 2066 6f72 2074 6865 2070 726f 6475  es for the produ
-000060c0: 6374 2e0a 0a20 2020 2020 2020 2020 2020  ct...           
-000060d0: 202a 2a54 6869 7320 6669 656c 6420 6361   **This field ca
-000060e0: 6e6e 6f74 2062 6520 7573 6564 2066 6f72  nnot be used for
-000060f0: 2073 6f72 7469 6e67 2074 6865 2072 6573   sorting the res
-00006100: 756c 7473 2e2a 2a0a 0a20 2020 2020 2020  ults.**..       
-00006110: 2020 2020 202a 2a4f 6e6c 7920 7365 6c65       **Only sele
-00006120: 6374 6564 2061 7474 7269 6275 7465 7320  cted attributes 
-00006130: 6f66 2074 6869 7320 6669 656c 6420 2866  of this field (f
-00006140: 6f72 2065 7861 6d70 6c65 2c0a 2020 2020  or example,.    
-00006150: 2020 2020 2020 2020 6060 6974 656d 5f69          ``item_i
-00006160: 7373 7565 732e 7365 7665 7269 7479 2e61  ssues.severity.a
-00006170: 6767 7265 6761 7465 645f 7365 7665 7269  ggregated_severi
-00006180: 7479 6060 2920 6361 6e20 6265 2075 7365  ty``) can be use
-00006190: 640a 2020 2020 2020 2020 2020 2020 666f  d.            fo
-000061a0: 7220 6669 6c74 6572 696e 6720 7468 6520  r filtering the 
-000061b0: 7265 7375 6c74 732e 2a2a 0a20 2020 2020  results.**.     
-000061c0: 2020 2063 6c69 636b 5f70 6f74 656e 7469     click_potenti
-000061d0: 616c 2028 676f 6f67 6c65 2e73 686f 7070  al (google.shopp
-000061e0: 696e 672e 6d65 7263 6861 6e74 5f72 6570  ing.merchant_rep
-000061f0: 6f72 7473 5f76 3162 6574 612e 7479 7065  orts_v1beta.type
-00006200: 732e 5072 6f64 7563 7456 6965 772e 436c  s.ProductView.Cl
-00006210: 6963 6b50 6f74 656e 7469 616c 293a 0a20  ickPotential):. 
-00006220: 2020 2020 2020 2020 2020 2045 7374 696d             Estim
-00006230: 6174 6564 2070 6572 666f 726d 616e 6365  ated performance
-00006240: 2070 6f74 656e 7469 616c 2063 6f6d 7061   potential compa
-00006250: 7265 6420 746f 0a20 2020 2020 2020 2020  red to.         
-00006260: 2020 2068 6967 6865 7374 2070 6572 666f     highest perfo
-00006270: 726d 696e 6720 7072 6f64 7563 7473 206f  rming products o
-00006280: 6620 7468 6520 6d65 7263 6861 6e74 2e0a  f the merchant..
-00006290: 2020 2020 2020 2020 636c 6963 6b5f 706f          click_po
-000062a0: 7465 6e74 6961 6c5f 7261 6e6b 2028 696e  tential_rank (in
-000062b0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-000062c0: 5261 6e6b 206f 6620 7468 6520 7072 6f64  Rank of the prod
-000062d0: 7563 7420 6261 7365 6420 6f6e 2069 7473  uct based on its
-000062e0: 2063 6c69 636b 2070 6f74 656e 7469 616c   click potential
-000062f0: 2e20 4120 7072 6f64 7563 740a 2020 2020  . A product.    
-00006300: 2020 2020 2020 2020 7769 7468 2060 6063          with ``c
-00006310: 6c69 636b 5f70 6f74 656e 7469 616c 5f72  lick_potential_r
-00006320: 616e 6b60 6020 3120 6861 7320 7468 6520  ank`` 1 has the 
-00006330: 6869 6768 6573 7420 636c 6963 6b0a 2020  highest click.  
-00006340: 2020 2020 2020 2020 2020 706f 7465 6e74            potent
-00006350: 6961 6c20 616d 6f6e 6720 7468 6520 6d65  ial among the me
-00006360: 7263 6861 6e74 2773 2070 726f 6475 6374  rchant's product
-00006370: 7320 7468 6174 2066 756c 6669 6c6c 2074  s that fulfill t
-00006380: 6865 0a20 2020 2020 2020 2020 2020 2073  he.            s
-00006390: 6561 7263 6820 7175 6572 7920 636f 6e64  earch query cond
-000063a0: 6974 696f 6e73 2e0a 0a20 2020 2020 2020  itions...       
-000063b0: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-000063c0: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-000063d0: 6f6e 656f 6660 5f20 6060 5f63 6c69 636b  oneof`_ ``_click
-000063e0: 5f70 6f74 656e 7469 616c 5f72 616e 6b60  _potential_rank`
-000063f0: 602e 0a20 2020 2022 2222 0a0a 2020 2020  `..    """..    
-00006400: 636c 6173 7320 4167 6772 6567 6174 6564  class Aggregated
-00006410: 5265 706f 7274 696e 6743 6f6e 7465 7874  ReportingContext
-00006420: 5374 6174 7573 2870 726f 746f 2e45 6e75  Status(proto.Enu
-00006430: 6d29 3a0a 2020 2020 2020 2020 7222 2222  m):.        r"""
-00006440: 5374 6174 7573 206f 6620 7468 6520 7072  Status of the pr
-00006450: 6f64 7563 7420 6167 6772 6567 6174 6564  oduct aggregated
-00006460: 2066 6f72 2061 6c6c 2072 6570 6f72 7469   for all reporti
-00006470: 6e67 2063 6f6e 7465 7874 732e 0a0a 2020  ng contexts...  
-00006480: 2020 2020 2020 4865 7265 2773 2061 6e20        Here's an 
-00006490: 6578 616d 706c 6520 6f66 2068 6f77 2074  example of how t
-000064a0: 6865 2061 6767 7265 6761 7465 6420 7374  he aggregated st
-000064b0: 6174 7573 2069 7320 636f 6d70 7574 6564  atus is computed
-000064c0: 3a0a 0a20 2020 2020 2020 2060 6060 0a20  :..        ```. 
-000064d0: 2020 2020 2020 2046 7265 6520 6c69 7374         Free list
-000064e0: 696e 6773 205c 7c20 5368 6f70 7069 6e67  ings \| Shopping
-000064f0: 2041 6473 205c 7c20 5374 6174 7573 0a20   Ads \| Status. 
-00006500: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00006510: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
-00006520: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
-00006530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006540: 2d2d 2d0a 2020 2020 2020 2020 4170 7072  ---.        Appr
-00006550: 6f76 6564 205c 7c20 4170 7072 6f76 6564  oved \| Approved
-00006560: 205c 7c20 454c 4947 4942 4c45 2041 7070   \| ELIGIBLE App
-00006570: 726f 7665 6420 5c7c 2050 656e 6469 6e67  roved \| Pending
-00006580: 205c 7c20 454c 4947 4942 4c45 0a20 2020   \| ELIGIBLE.   
-00006590: 2020 2020 2041 7070 726f 7665 6420 5c7c       Approved \|
-000065a0: 2044 6973 6170 7072 6f76 6564 205c 7c20   Disapproved \| 
-000065b0: 454c 4947 4942 4c45 5f4c 494d 4954 4544  ELIGIBLE_LIMITED
-000065c0: 2050 656e 6469 6e67 205c 7c20 5065 6e64   Pending \| Pend
-000065d0: 696e 6720 5c7c 0a20 2020 2020 2020 2050  ing \|.        P
-000065e0: 454e 4449 4e47 2044 6973 6170 7072 6f76  ENDING Disapprov
-000065f0: 6564 205c 7c20 4469 7361 7070 726f 7665  ed \| Disapprove
-00006600: 6420 5c7c 204e 4f54 5f45 4c49 4749 424c  d \| NOT_ELIGIBL
-00006610: 455f 4f52 5f44 4953 4150 5052 4f56 4544  E_OR_DISAPPROVED
-00006620: 0a20 2020 2020 2020 2060 6060 0a0a 2020  .        ```..  
-00006630: 2020 2020 2020 5661 6c75 6573 3a0a 2020        Values:.  
-00006640: 2020 2020 2020 2020 2020 4147 4752 4547            AGGREG
-00006650: 4154 4544 5f52 4550 4f52 5449 4e47 5f43  ATED_REPORTING_C
-00006660: 4f4e 5445 5854 5f53 5441 5455 535f 554e  ONTEXT_STATUS_UN
-00006670: 5350 4543 4946 4945 4420 2830 293a 0a20  SPECIFIED (0):. 
-00006680: 2020 2020 2020 2020 2020 2020 2020 204e                 N
-00006690: 6f74 2073 7065 6369 6669 6564 2e0a 2020  ot specified..  
-000066a0: 2020 2020 2020 2020 2020 4e4f 545f 454c            NOT_EL
-000066b0: 4947 4942 4c45 5f4f 525f 4449 5341 5050  IGIBLE_OR_DISAPP
-000066c0: 524f 5645 4420 2831 293a 0a20 2020 2020  ROVED (1):.     
-000066d0: 2020 2020 2020 2020 2020 2050 726f 6475             Produ
-000066e0: 6374 2069 7320 6e6f 7420 656c 6967 6962  ct is not eligib
-000066f0: 6c65 206f 7220 6973 2064 6973 6170 7072  le or is disappr
-00006700: 6f76 6564 2066 6f72 0a20 2020 2020 2020  oved for.       
-00006710: 2020 2020 2020 2020 2061 6c6c 2072 6570           all rep
-00006720: 6f72 7469 6e67 2063 6f6e 7465 7874 732e  orting contexts.
-00006730: 0a20 2020 2020 2020 2020 2020 2050 454e  .            PEN
-00006740: 4449 4e47 2028 3229 3a0a 2020 2020 2020  DING (2):.      
-00006750: 2020 2020 2020 2020 2020 5072 6f64 7563            Produc
-00006760: 7427 7320 7374 6174 7573 2069 7320 7065  t's status is pe
-00006770: 6e64 696e 6720 696e 2061 6c6c 2072 6570  nding in all rep
-00006780: 6f72 7469 6e67 0a20 2020 2020 2020 2020  orting.         
-00006790: 2020 2020 2020 2063 6f6e 7465 7874 732e         contexts.
-000067a0: 0a20 2020 2020 2020 2020 2020 2045 4c49  .            ELI
-000067b0: 4749 424c 455f 4c49 4d49 5445 4420 2833  GIBLE_LIMITED (3
-000067c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000067d0: 2020 2050 726f 6475 6374 2069 7320 656c     Product is el
-000067e0: 6967 6962 6c65 2066 6f72 2073 6f6d 6520  igible for some 
-000067f0: 2862 7574 206e 6f74 2061 6c6c 290a 2020  (but not all).  
-00006800: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00006810: 706f 7274 696e 6720 636f 6e74 6578 7473  porting contexts
-00006820: 2e0a 2020 2020 2020 2020 2020 2020 454c  ..            EL
-00006830: 4947 4942 4c45 2028 3429 3a0a 2020 2020  IGIBLE (4):.    
-00006840: 2020 2020 2020 2020 2020 2020 5072 6f64              Prod
-00006850: 7563 7420 6973 2065 6c69 6769 626c 6520  uct is eligible 
-00006860: 666f 7220 616c 6c20 7265 706f 7274 696e  for all reportin
-00006870: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-00006880: 2020 636f 6e74 6578 7473 2e0a 2020 2020    contexts..    
-00006890: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000068a0: 4147 4752 4547 4154 4544 5f52 4550 4f52  AGGREGATED_REPOR
-000068b0: 5449 4e47 5f43 4f4e 5445 5854 5f53 5441  TING_CONTEXT_STA
-000068c0: 5455 535f 554e 5350 4543 4946 4945 4420  TUS_UNSPECIFIED 
-000068d0: 3d20 300a 2020 2020 2020 2020 4e4f 545f  = 0.        NOT_
-000068e0: 454c 4947 4942 4c45 5f4f 525f 4449 5341  ELIGIBLE_OR_DISA
-000068f0: 5050 524f 5645 4420 3d20 310a 2020 2020  PPROVED = 1.    
-00006900: 2020 2020 5045 4e44 494e 4720 3d20 320a      PENDING = 2.
-00006910: 2020 2020 2020 2020 454c 4947 4942 4c45          ELIGIBLE
-00006920: 5f4c 494d 4954 4544 203d 2033 0a20 2020  _LIMITED = 3.   
-00006930: 2020 2020 2045 4c49 4749 424c 4520 3d20       ELIGIBLE = 
-00006940: 340a 0a20 2020 2063 6c61 7373 2043 6c69  4..    class Cli
-00006950: 636b 506f 7465 6e74 6961 6c28 7072 6f74  ckPotential(prot
-00006960: 6f2e 456e 756d 293a 0a20 2020 2020 2020  o.Enum):.       
-00006970: 2072 2222 2241 2070 726f 6475 6374 2773   r"""A product's
-00006980: 2060 636c 6963 6b0a 2020 2020 2020 2020   `click.        
-00006990: 706f 7465 6e74 6961 6c20 3c68 7474 7073  potential <https
-000069a0: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-000069b0: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-000069c0: 616e 7377 6572 2f31 3838 3438 383e 605f  answer/188488>`_
-000069d0: 5f0a 2020 2020 2020 2020 6573 7469 6d61  _.        estima
-000069e0: 7465 7320 6974 7320 7065 7266 6f72 6d61  tes its performa
-000069f0: 6e63 6520 706f 7465 6e74 6961 6c20 636f  nce potential co
-00006a00: 6d70 6172 6564 2074 6f20 6869 6768 6573  mpared to highes
-00006a10: 7420 7065 7266 6f72 6d69 6e67 0a20 2020  t performing.   
-00006a20: 2020 2020 2070 726f 6475 6374 7320 6f66       products of
-00006a30: 2074 6865 206d 6572 6368 616e 742e 2043   the merchant. C
-00006a40: 6c69 636b 2070 6f74 656e 7469 616c 206f  lick potential o
-00006a50: 6620 6120 7072 6f64 7563 7420 6865 6c70  f a product help
-00006a60: 730a 2020 2020 2020 2020 6d65 7263 6861  s.        mercha
-00006a70: 6e74 7320 746f 2070 7269 6f72 6974 697a  nts to prioritiz
-00006a80: 6520 7768 6963 6820 7072 6f64 7563 7473  e which products
-00006a90: 2074 6f20 6669 7820 616e 6420 6865 6c70   to fix and help
-00006aa0: 7320 7468 656d 0a20 2020 2020 2020 2075  s them.        u
-00006ab0: 6e64 6572 7374 616e 6420 686f 7720 7072  nderstand how pr
-00006ac0: 6f64 7563 7473 2061 7265 2070 6572 666f  oducts are perfo
-00006ad0: 726d 696e 6720 6167 6169 6e73 7420 7468  rming against th
-00006ae0: 6569 7220 706f 7465 6e74 6961 6c2e 0a0a  eir potential...
-00006af0: 2020 2020 2020 2020 5661 6c75 6573 3a0a          Values:.
-00006b00: 2020 2020 2020 2020 2020 2020 434c 4943              CLIC
-00006b10: 4b5f 504f 5445 4e54 4941 4c5f 554e 5350  K_POTENTIAL_UNSP
-00006b20: 4543 4946 4945 4420 2830 293a 0a20 2020  ECIFIED (0):.   
-00006b30: 2020 2020 2020 2020 2020 2020 2055 6e6b               Unk
-00006b40: 6e6f 776e 2070 7265 6469 6374 6564 2063  nown predicted c
-00006b50: 6c69 636b 7320 696d 7061 6374 2e0a 2020  licks impact..  
-00006b60: 2020 2020 2020 2020 2020 4c4f 5720 2831            LOW (1
-00006b70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00006b80: 2020 2050 6f74 656e 7469 616c 2074 6f20     Potential to 
-00006b90: 7265 6365 6976 6520 6120 6c6f 7720 6e75  receive a low nu
-00006ba0: 6d62 6572 206f 6620 636c 6963 6b73 0a20  mber of clicks. 
-00006bb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00006bc0: 6f6d 7061 7265 6420 746f 2074 6865 2068  ompared to the h
-00006bd0: 6967 6865 7374 2070 6572 666f 726d 696e  ighest performin
-00006be0: 6720 7072 6f64 7563 7473 206f 660a 2020  g products of.  
-00006bf0: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00006c00: 6520 6d65 7263 6861 6e74 2e0a 2020 2020  e merchant..    
-00006c10: 2020 2020 2020 2020 4d45 4449 554d 2028          MEDIUM (
-00006c20: 3229 3a0a 2020 2020 2020 2020 2020 2020  2):.            
-00006c30: 2020 2020 506f 7465 6e74 6961 6c20 746f      Potential to
-00006c40: 2072 6563 6569 7665 2061 206d 6f64 6572   receive a moder
-00006c50: 6174 6520 6e75 6d62 6572 206f 660a 2020  ate number of.  
-00006c60: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-00006c70: 6963 6b73 2063 6f6d 7061 7265 6420 746f  icks compared to
-00006c80: 2074 6865 2068 6967 6865 7374 2070 6572   the highest per
-00006c90: 666f 726d 696e 670a 2020 2020 2020 2020  forming.        
-00006ca0: 2020 2020 2020 2020 7072 6f64 7563 7473          products
-00006cb0: 206f 6620 7468 6520 6d65 7263 6861 6e74   of the merchant
-00006cc0: 2e0a 2020 2020 2020 2020 2020 2020 4849  ..            HI
-00006cd0: 4748 2028 3329 3a0a 2020 2020 2020 2020  GH (3):.        
-00006ce0: 2020 2020 2020 2020 506f 7465 6e74 6961          Potentia
-00006cf0: 6c20 746f 2072 6563 6569 7665 2061 2073  l to receive a s
-00006d00: 696d 696c 6172 206e 756d 6265 7220 6f66  imilar number of
-00006d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006d20: 2063 6c69 636b 7320 6173 2074 6865 2068   clicks as the h
-00006d30: 6967 6865 7374 2070 6572 666f 726d 696e  ighest performin
-00006d40: 6720 7072 6f64 7563 7473 206f 6620 7468  g products of th
-00006d50: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00006d60: 2020 6d65 7263 6861 6e74 2e0a 2020 2020    merchant..    
-00006d70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00006d80: 434c 4943 4b5f 504f 5445 4e54 4941 4c5f  CLICK_POTENTIAL_
-00006d90: 554e 5350 4543 4946 4945 4420 3d20 300a  UNSPECIFIED = 0.
-00006da0: 2020 2020 2020 2020 4c4f 5720 3d20 310a          LOW = 1.
-00006db0: 2020 2020 2020 2020 4d45 4449 554d 203d          MEDIUM =
-00006dc0: 2032 0a20 2020 2020 2020 2048 4947 4820   2.        HIGH 
-00006dd0: 3d20 330a 0a20 2020 2063 6c61 7373 2049  = 3..    class I
-00006de0: 7465 6d49 7373 7565 2870 726f 746f 2e4d  temIssue(proto.M
-00006df0: 6573 7361 6765 293a 0a20 2020 2020 2020  essage):.       
-00006e00: 2072 2222 2249 7465 6d20 6973 7375 6520   r"""Item issue 
-00006e10: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
-00006e20: 7468 6520 7072 6f64 7563 742e 0a0a 2020  the product...  
-00006e30: 2020 2020 2020 2e2e 205f 6f6e 656f 663a        .. _oneof:
-00006e40: 2068 7474 7073 3a2f 2f70 726f 746f 2d70   https://proto-p
-00006e50: 6c75 732d 7079 7468 6f6e 2e72 6561 6474  lus-python.readt
-00006e60: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-00006e70: 626c 652f 6669 656c 6473 2e68 746d 6c23  ble/fields.html#
-00006e80: 6f6e 656f 6673 2d6d 7574 7561 6c6c 792d  oneofs-mutually-
-00006e90: 6578 636c 7573 6976 652d 6669 656c 6473  exclusive-fields
-00006ea0: 0a0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
-00006eb0: 7574 6573 3a0a 2020 2020 2020 2020 2020  utes:.          
-00006ec0: 2020 7479 7065 5f20 2867 6f6f 676c 652e    type_ (google.
-00006ed0: 7368 6f70 7069 6e67 2e6d 6572 6368 616e  shopping.merchan
-00006ee0: 745f 7265 706f 7274 735f 7631 6265 7461  t_reports_v1beta
-00006ef0: 2e74 7970 6573 2e50 726f 6475 6374 5669  .types.ProductVi
-00006f00: 6577 2e49 7465 6d49 7373 7565 2e49 7465  ew.ItemIssue.Ite
-00006f10: 6d49 7373 7565 5479 7065 293a 0a20 2020  mIssueType):.   
-00006f20: 2020 2020 2020 2020 2020 2020 2049 7465               Ite
-00006f30: 6d20 6973 7375 6520 7479 7065 2e0a 2020  m issue type..  
-00006f40: 2020 2020 2020 2020 2020 7365 7665 7269            severi
-00006f50: 7479 2028 676f 6f67 6c65 2e73 686f 7070  ty (google.shopp
-00006f60: 696e 672e 6d65 7263 6861 6e74 5f72 6570  ing.merchant_rep
-00006f70: 6f72 7473 5f76 3162 6574 612e 7479 7065  orts_v1beta.type
-00006f80: 732e 5072 6f64 7563 7456 6965 772e 4974  s.ProductView.It
-00006f90: 656d 4973 7375 652e 4974 656d 4973 7375  emIssue.ItemIssu
-00006fa0: 6553 6576 6572 6974 7929 3a0a 2020 2020  eSeverity):.    
-00006fb0: 2020 2020 2020 2020 2020 2020 4974 656d              Item
-00006fc0: 2069 7373 7565 2073 6576 6572 6974 792e   issue severity.
-00006fd0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00006fe0: 6f6c 7574 696f 6e20 2867 6f6f 676c 652e  olution (google.
-00006ff0: 7368 6f70 7069 6e67 2e6d 6572 6368 616e  shopping.merchan
-00007000: 745f 7265 706f 7274 735f 7631 6265 7461  t_reports_v1beta
-00007010: 2e74 7970 6573 2e50 726f 6475 6374 5669  .types.ProductVi
-00007020: 6577 2e49 7465 6d49 7373 7565 2e49 7465  ew.ItemIssue.Ite
-00007030: 6d49 7373 7565 5265 736f 6c75 7469 6f6e  mIssueResolution
-00007040: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00007050: 2020 2049 7465 6d20 6973 7375 6520 7265     Item issue re
-00007060: 736f 6c75 7469 6f6e 2e0a 0a20 2020 2020  solution...     
-00007070: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00007080: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-00007090: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-000070a0: 5f72 6573 6f6c 7574 696f 6e60 602e 0a20  _resolution``.. 
-000070b0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-000070c0: 2020 2020 636c 6173 7320 4974 656d 4973      class ItemIs
-000070d0: 7375 6552 6573 6f6c 7574 696f 6e28 7072  sueResolution(pr
-000070e0: 6f74 6f2e 456e 756d 293a 0a20 2020 2020  oto.Enum):.     
-000070f0: 2020 2020 2020 2072 2222 2248 6f77 2074         r"""How t
-00007100: 6f20 7265 736f 6c76 6520 7468 6520 6973  o resolve the is
-00007110: 7375 652e 0a0a 2020 2020 2020 2020 2020  sue...          
-00007120: 2020 5661 6c75 6573 3a0a 2020 2020 2020    Values:.      
-00007130: 2020 2020 2020 2020 2020 4954 454d 5f49            ITEM_I
-00007140: 5353 5545 5f52 4553 4f4c 5554 494f 4e5f  SSUE_RESOLUTION_
-00007150: 554e 5350 4543 4946 4945 4420 2830 293a  UNSPECIFIED (0):
-00007160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007170: 2020 2020 204e 6f74 2073 7065 6369 6669       Not specifi
-00007180: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-00007190: 2020 2020 4d45 5243 4841 4e54 5f41 4354      MERCHANT_ACT
-000071a0: 494f 4e20 2831 293a 0a20 2020 2020 2020  ION (1):.       
-000071b0: 2020 2020 2020 2020 2020 2020 2054 6865               The
-000071c0: 206d 6572 6368 616e 7420 6861 7320 746f   merchant has to
-000071d0: 2066 6978 2074 6865 2069 7373 7565 2e0a   fix the issue..
-000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071f0: 5045 4e44 494e 475f 5052 4f43 4553 5349  PENDING_PROCESSI
-00007200: 4e47 2028 3229 3a0a 2020 2020 2020 2020  NG (2):.        
-00007210: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00007220: 6973 7375 6520 7769 6c6c 2062 6520 7265  issue will be re
-00007230: 736f 6c76 6564 2061 7574 6f6d 6174 6963  solved automatic
-00007240: 616c 6c79 2028 666f 720a 2020 2020 2020  ally (for.      
-00007250: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00007260: 616d 706c 652c 2069 6d61 6765 2063 7261  ample, image cra
-00007270: 776c 2920 6f72 2074 6872 6f75 6768 2061  wl) or through a
-00007280: 2047 6f6f 676c 650a 2020 2020 2020 2020   Google.        
-00007290: 2020 2020 2020 2020 2020 2020 7265 7669              revi
-000072a0: 6577 2e20 4e6f 206d 6572 6368 616e 7420  ew. No merchant 
-000072b0: 6163 7469 6f6e 2069 7320 7265 7175 6972  action is requir
-000072c0: 6564 206e 6f77 2e0a 2020 2020 2020 2020  ed now..        
-000072d0: 2020 2020 2020 2020 2020 2020 5265 736f              Reso
-000072e0: 6c75 7469 6f6e 206d 6967 6874 206c 6561  lution might lea
-000072f0: 6420 746f 2061 6e6f 7468 6572 2069 7373  d to another iss
-00007300: 7565 2028 666f 720a 2020 2020 2020 2020  ue (for.        
-00007310: 2020 2020 2020 2020 2020 2020 6578 616d              exam
-00007320: 706c 652c 2069 6620 6372 6177 6c20 6661  ple, if crawl fa
-00007330: 696c 7329 2e0a 2020 2020 2020 2020 2020  ils)..          
-00007340: 2020 2222 220a 2020 2020 2020 2020 2020    """.          
-00007350: 2020 4954 454d 5f49 5353 5545 5f52 4553    ITEM_ISSUE_RES
-00007360: 4f4c 5554 494f 4e5f 554e 5350 4543 4946  OLUTION_UNSPECIF
-00007370: 4945 4420 3d20 300a 2020 2020 2020 2020  IED = 0.        
-00007380: 2020 2020 4d45 5243 4841 4e54 5f41 4354      MERCHANT_ACT
-00007390: 494f 4e20 3d20 310a 2020 2020 2020 2020  ION = 1.        
-000073a0: 2020 2020 5045 4e44 494e 475f 5052 4f43      PENDING_PROC
-000073b0: 4553 5349 4e47 203d 2032 0a0a 2020 2020  ESSING = 2..    
-000073c0: 2020 2020 636c 6173 7320 4974 656d 4973      class ItemIs
-000073d0: 7375 6554 7970 6528 7072 6f74 6f2e 4d65  sueType(proto.Me
-000073e0: 7373 6167 6529 3a0a 2020 2020 2020 2020  ssage):.        
-000073f0: 2020 2020 7222 2222 4973 7375 6520 7479      r"""Issue ty
-00007400: 7065 2e0a 0a20 2020 2020 2020 2020 2020  pe...           
-00007410: 202e 2e20 5f6f 6e65 6f66 3a20 6874 7470   .. _oneof: http
-00007420: 733a 2f2f 7072 6f74 6f2d 706c 7573 2d70  s://proto-plus-p
-00007430: 7974 686f 6e2e 7265 6164 7468 6564 6f63  ython.readthedoc
-00007440: 732e 696f 2f65 6e2f 7374 6162 6c65 2f66  s.io/en/stable/f
-00007450: 6965 6c64 732e 6874 6d6c 236f 6e65 6f66  ields.html#oneof
-00007460: 732d 6d75 7475 616c 6c79 2d65 7863 6c75  s-mutually-exclu
-00007470: 7369 7665 2d66 6965 6c64 730a 0a20 2020  sive-fields..   
-00007480: 2020 2020 2020 2020 2041 7474 7269 6275           Attribu
-00007490: 7465 733a 0a20 2020 2020 2020 2020 2020  tes:.           
-000074a0: 2020 2020 2063 6f64 6520 2873 7472 293a       code (str):
-000074b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000074c0: 2020 2020 2045 7272 6f72 2063 6f64 6520       Error code 
-000074d0: 6f66 2074 6865 2069 7373 7565 2c20 6571  of the issue, eq
-000074e0: 7569 7661 6c65 6e74 2074 6f20 7468 6520  uivalent to the 
-000074f0: 6060 636f 6465 6060 206f 660a 2020 2020  ``code`` of.    
-00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007510: 6050 726f 6475 6374 0a20 2020 2020 2020  `Product.       
-00007520: 2020 2020 2020 2020 2020 2020 2069 7373               iss
-00007530: 7565 7320 3c68 7474 7073 3a2f 2f64 6576  ues <https://dev
-00007540: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
-00007550: 6f6d 2f73 686f 7070 696e 672d 636f 6e74  om/shopping-cont
-00007560: 656e 742f 6775 6964 6573 2f70 726f 6475  ent/guides/produ
-00007570: 6374 2d69 7373 7565 733e 605f 5f2e 0a0a  ct-issues>`__...
-00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007590: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-000075a0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-000075b0: 6e65 6f66 605f 2060 605f 636f 6465 6060  neof`_ ``_code``
-000075c0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000075d0: 2020 6361 6e6f 6e69 6361 6c5f 6174 7472    canonical_attr
-000075e0: 6962 7574 6520 2873 7472 293a 0a20 2020  ibute (str):.   
-000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007600: 2043 616e 6f6e 6963 616c 2061 7474 7269   Canonical attri
-00007610: 6275 7465 206e 616d 6520 666f 720a 2020  bute name for.  
-00007620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007630: 2020 6174 7472 6962 7574 652d 7370 6563    attribute-spec
-00007640: 6966 6963 2069 7373 7565 732e 0a0a 2020  ific issues...  
-00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007660: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00007670: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00007680: 6f66 605f 2060 605f 6361 6e6f 6e69 6361  of`_ ``_canonica
-00007690: 6c5f 6174 7472 6962 7574 6560 602e 0a20  l_attribute``.. 
-000076a0: 2020 2020 2020 2020 2020 2022 2222 0a0a             """..
-000076b0: 2020 2020 2020 2020 2020 2020 636f 6465              code
-000076c0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-000076d0: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
-000076e0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-000076f0: 472c 0a20 2020 2020 2020 2020 2020 2020  G,.             
-00007700: 2020 206e 756d 6265 723d 312c 0a20 2020     number=1,.   
-00007710: 2020 2020 2020 2020 2020 2020 206f 7074               opt
-00007720: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-00007730: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00007740: 2020 2020 2020 6361 6e6f 6e69 6361 6c5f        canonical_
-00007750: 6174 7472 6962 7574 653a 2073 7472 203d  attribute: str =
-00007760: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-00007770: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00007780: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
-00007790: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
-000077a0: 6572 3d32 2c0a 2020 2020 2020 2020 2020  er=2,.          
-000077b0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-000077c0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-000077d0: 2029 0a0a 2020 2020 2020 2020 636c 6173   )..        clas
-000077e0: 7320 4974 656d 4973 7375 6553 6576 6572  s ItemIssueSever
-000077f0: 6974 7928 7072 6f74 6f2e 4d65 7373 6167  ity(proto.Messag
-00007800: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00007810: 7222 2222 486f 7720 7468 6520 6973 7375  r"""How the issu
-00007820: 6520 6166 6665 6374 7320 7468 6520 7365  e affects the se
-00007830: 7276 696e 6720 6f66 2074 6865 2070 726f  rving of the pro
-00007840: 6475 6374 2e0a 0a20 2020 2020 2020 2020  duct...         
-00007850: 2020 202e 2e20 5f6f 6e65 6f66 3a20 6874     .. _oneof: ht
-00007860: 7470 733a 2f2f 7072 6f74 6f2d 706c 7573  tps://proto-plus
-00007870: 2d70 7974 686f 6e2e 7265 6164 7468 6564  -python.readthed
-00007880: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
-00007890: 2f66 6965 6c64 732e 6874 6d6c 236f 6e65  /fields.html#one
-000078a0: 6f66 732d 6d75 7475 616c 6c79 2d65 7863  ofs-mutually-exc
-000078b0: 6c75 7369 7665 2d66 6965 6c64 730a 0a20  lusive-fields.. 
-000078c0: 2020 2020 2020 2020 2020 2041 7474 7269             Attri
-000078d0: 6275 7465 733a 0a20 2020 2020 2020 2020  butes:.         
-000078e0: 2020 2020 2020 2073 6576 6572 6974 795f         severity_
-000078f0: 7065 725f 7265 706f 7274 696e 675f 636f  per_reporting_co
-00007900: 6e74 6578 7420 284d 7574 6162 6c65 5365  ntext (MutableSe
-00007910: 7175 656e 6365 5b67 6f6f 676c 652e 7368  quence[google.sh
-00007920: 6f70 7069 6e67 2e6d 6572 6368 616e 745f  opping.merchant_
-00007930: 7265 706f 7274 735f 7631 6265 7461 2e74  reports_v1beta.t
-00007940: 7970 6573 2e50 726f 6475 6374 5669 6577  ypes.ProductView
-00007950: 2e49 7465 6d49 7373 7565 2e49 7465 6d49  .ItemIssue.ItemI
-00007960: 7373 7565 5365 7665 7269 7479 2e49 7373  ssueSeverity.Iss
-00007970: 7565 5365 7665 7269 7479 5065 7252 6570  ueSeverityPerRep
-00007980: 6f72 7469 6e67 436f 6e74 6578 745d 293a  ortingContext]):
-00007990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000079a0: 2020 2020 2049 7373 7565 2073 6576 6572       Issue sever
-000079b0: 6974 7920 7065 7220 7265 706f 7274 696e  ity per reportin
-000079c0: 6720 636f 6e74 6578 742e 0a20 2020 2020  g context..     
-000079d0: 2020 2020 2020 2020 2020 2061 6767 7265             aggre
-000079e0: 6761 7465 645f 7365 7665 7269 7479 2028  gated_severity (
-000079f0: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
-00007a00: 6d65 7263 6861 6e74 5f72 6570 6f72 7473  merchant_reports
-00007a10: 5f76 3162 6574 612e 7479 7065 732e 5072  _v1beta.types.Pr
-00007a20: 6f64 7563 7456 6965 772e 4974 656d 4973  oductView.ItemIs
-00007a30: 7375 652e 4974 656d 4973 7375 6553 6576  sue.ItemIssueSev
-00007a40: 6572 6974 792e 4167 6772 6567 6174 6564  erity.Aggregated
-00007a50: 4973 7375 6553 6576 6572 6974 7929 3a0a  IssueSeverity):.
-00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a70: 2020 2020 4167 6772 6567 6174 6564 2073      Aggregated s
-00007a80: 6576 6572 6974 7920 6f66 2074 6865 2069  everity of the i
-00007a90: 7373 7565 2066 6f72 2061 6c6c 2072 6570  ssue for all rep
-00007aa0: 6f72 7469 6e67 2063 6f6e 7465 7874 730a  orting contexts.
-00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ac0: 2020 2020 6974 2061 6666 6563 7473 2e0a      it affects..
-00007ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007ae0: 2020 2020 202a 2a54 6869 7320 6669 656c       **This fiel
-00007af0: 6420 6361 6e20 6265 2075 7365 6420 666f  d can be used fo
-00007b00: 7220 6669 6c74 6572 696e 6720 7468 6520  r filtering the 
-00007b10: 7265 7375 6c74 732e 2a2a 0a0a 2020 2020  results.**..    
-00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b30: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-00007b40: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-00007b50: 605f 2060 605f 6167 6772 6567 6174 6564  `_ ``_aggregated
-00007b60: 5f73 6576 6572 6974 7960 602e 0a20 2020  _severity``..   
-00007b70: 2020 2020 2020 2020 2022 2222 0a0a 2020           """..  
-00007b80: 2020 2020 2020 2020 2020 636c 6173 7320            class 
-00007b90: 4167 6772 6567 6174 6564 4973 7375 6553  AggregatedIssueS
-00007ba0: 6576 6572 6974 7928 7072 6f74 6f2e 456e  everity(proto.En
-00007bb0: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
-00007bc0: 2020 2020 2072 2222 2249 7373 7565 2073       r"""Issue s
-00007bd0: 6576 6572 6974 7920 6167 6772 6567 6174  everity aggregat
-00007be0: 6564 2066 6f72 2061 6c6c 2072 6570 6f72  ed for all repor
-00007bf0: 7469 6e67 2063 6f6e 7465 7874 732e 0a0a  ting contexts...
-00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c10: 5661 6c75 6573 3a0a 2020 2020 2020 2020  Values:.        
-00007c20: 2020 2020 2020 2020 2020 2020 4147 4752              AGGR
-00007c30: 4547 4154 4544 5f49 5353 5545 5f53 4556  EGATED_ISSUE_SEV
-00007c40: 4552 4954 595f 554e 5350 4543 4946 4945  ERITY_UNSPECIFIE
-00007c50: 4420 2830 293a 0a20 2020 2020 2020 2020  D (0):.         
-00007c60: 2020 2020 2020 2020 2020 2020 2020 204e                 N
-00007c70: 6f74 2073 7065 6369 6669 6564 2e0a 2020  ot specified..  
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 4449 5341 5050 524f 5645 4420 2831    DISAPPROVED (1
-00007ca0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00007cb0: 2020 2020 2020 2020 2020 2049 7373 7565             Issue
-00007cc0: 2064 6973 6170 7072 6f76 6573 2074 6865   disapproves the
-00007cd0: 2070 726f 6475 6374 2069 6e20 6174 206c   product in at l
-00007ce0: 6561 7374 206f 6e65 0a20 2020 2020 2020  east one.       
-00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d00: 2072 6570 6f72 7469 6e67 2063 6f6e 7465   reporting conte
-00007d10: 7874 2e0a 2020 2020 2020 2020 2020 2020  xt..            
-00007d20: 2020 2020 2020 2020 4445 4d4f 5445 4420          DEMOTED 
-00007d30: 2832 293a 0a20 2020 2020 2020 2020 2020  (2):.           
-00007d40: 2020 2020 2020 2020 2020 2020 2049 7373               Iss
-00007d50: 7565 2064 656d 6f74 6573 2074 6865 2070  ue demotes the p
-00007d60: 726f 6475 6374 2069 6e20 616c 6c20 7265  roduct in all re
-00007d70: 706f 7274 696e 670a 2020 2020 2020 2020  porting.        
-00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d90: 636f 6e74 6578 7473 2069 7420 6166 6665  contexts it affe
-00007da0: 6374 732e 0a20 2020 2020 2020 2020 2020  cts..           
-00007db0: 2020 2020 2020 2020 2050 454e 4449 4e47           PENDING
-00007dc0: 2028 3329 3a0a 2020 2020 2020 2020 2020   (3):.          
-00007dd0: 2020 2020 2020 2020 2020 2020 2020 4973                Is
-00007de0: 7375 6520 7265 736f 6c75 7469 6f6e 2069  sue resolution i
-00007df0: 7320 6060 5045 4e44 494e 475f 5052 4f43  s ``PENDING_PROC
-00007e00: 4553 5349 4e47 6060 2e0a 2020 2020 2020  ESSING``..      
-00007e10: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
-00007e20: 2020 2020 2020 2020 2020 2020 2020 4147                AG
-00007e30: 4752 4547 4154 4544 5f49 5353 5545 5f53  GREGATED_ISSUE_S
-00007e40: 4556 4552 4954 595f 554e 5350 4543 4946  EVERITY_UNSPECIF
-00007e50: 4945 4420 3d20 300a 2020 2020 2020 2020  IED = 0.        
-00007e60: 2020 2020 2020 2020 4449 5341 5050 524f          DISAPPRO
-00007e70: 5645 4420 3d20 310a 2020 2020 2020 2020  VED = 1.        
-00007e80: 2020 2020 2020 2020 4445 4d4f 5445 4420          DEMOTED 
-00007e90: 3d20 320a 2020 2020 2020 2020 2020 2020  = 2.            
-00007ea0: 2020 2020 5045 4e44 494e 4720 3d20 330a      PENDING = 3.
-00007eb0: 0a20 2020 2020 2020 2020 2020 2063 6c61  .            cla
-00007ec0: 7373 2049 7373 7565 5365 7665 7269 7479  ss IssueSeverity
-00007ed0: 5065 7252 6570 6f72 7469 6e67 436f 6e74  PerReportingCont
-00007ee0: 6578 7428 7072 6f74 6f2e 4d65 7373 6167  ext(proto.Messag
-00007ef0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00007f00: 2020 2020 7222 2222 4973 7375 6520 7365      r"""Issue se
-00007f10: 7665 7269 7479 2070 6572 2072 6570 6f72  verity per repor
-00007f20: 7469 6e67 2063 6f6e 7465 7874 2e0a 0a20  ting context... 
-00007f30: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-00007f40: 2e20 5f6f 6e65 6f66 3a20 6874 7470 733a  . _oneof: https:
-00007f50: 2f2f 7072 6f74 6f2d 706c 7573 2d70 7974  //proto-plus-pyt
-00007f60: 686f 6e2e 7265 6164 7468 6564 6f63 732e  hon.readthedocs.
-00007f70: 696f 2f65 6e2f 7374 6162 6c65 2f66 6965  io/en/stable/fie
-00007f80: 6c64 732e 6874 6d6c 236f 6e65 6f66 732d  lds.html#oneofs-
-00007f90: 6d75 7475 616c 6c79 2d65 7863 6c75 7369  mutually-exclusi
-00007fa0: 7665 2d66 6965 6c64 730a 0a20 2020 2020  ve-fields..     
-00007fb0: 2020 2020 2020 2020 2020 2041 7474 7269             Attri
-00007fc0: 6275 7465 733a 0a20 2020 2020 2020 2020  butes:.         
-00007fd0: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
-00007fe0: 7469 6e67 5f63 6f6e 7465 7874 2028 676f  ting_context (go
-00007ff0: 6f67 6c65 2e73 686f 7070 696e 672e 7479  ogle.shopping.ty
-00008000: 7065 2e74 7970 6573 2e52 6570 6f72 7469  pe.types.Reporti
-00008010: 6e67 436f 6e74 6578 742e 5265 706f 7274  ngContext.Report
-00008020: 696e 6743 6f6e 7465 7874 456e 756d 293a  ingContextEnum):
-00008030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008040: 2020 2020 2020 2020 2052 6570 6f72 7469           Reporti
-00008050: 6e67 2063 6f6e 7465 7874 2074 6865 2069  ng context the i
-00008060: 7373 7565 2061 7070 6c69 6573 2074 6f2e  ssue applies to.
-00008070: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008080: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00008090: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-000080a0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-000080b0: 7265 706f 7274 696e 675f 636f 6e74 6578  reporting_contex
-000080c0: 7460 602e 0a20 2020 2020 2020 2020 2020  t``..           
-000080d0: 2020 2020 2020 2020 2064 6973 6170 7072           disappr
-000080e0: 6f76 6564 5f63 6f75 6e74 7269 6573 2028  oved_countries (
-000080f0: 4d75 7461 626c 6553 6571 7565 6e63 655b  MutableSequence[
-00008100: 7374 725d 293a 0a20 2020 2020 2020 2020  str]):.         
-00008110: 2020 2020 2020 2020 2020 2020 2020 204c                 L
-00008120: 6973 7420 6f66 2064 6973 6170 7072 6f76  ist of disapprov
-00008130: 6564 2063 6f75 6e74 7269 6573 2069 6e20  ed countries in 
-00008140: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-00008150: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-00008160: 7274 696e 6720 636f 6e74 6578 742c 2072  rting context, r
-00008170: 6570 7265 7365 6e74 6564 2069 6e20 4953  epresented in IS
-00008180: 4f20 3331 3636 0a20 2020 2020 2020 2020  O 3166.         
-00008190: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000081a0: 6f72 6d61 742e 0a20 2020 2020 2020 2020  ormat..         
-000081b0: 2020 2020 2020 2020 2020 2064 656d 6f74             demot
-000081c0: 6564 5f63 6f75 6e74 7269 6573 2028 4d75  ed_countries (Mu
-000081d0: 7461 626c 6553 6571 7565 6e63 655b 7374  tableSequence[st
-000081e0: 725d 293a 0a20 2020 2020 2020 2020 2020  r]):.           
-000081f0: 2020 2020 2020 2020 2020 2020 204c 6973               Lis
-00008200: 7420 6f66 2064 656d 6f74 6564 2063 6f75  t of demoted cou
-00008210: 6e74 7269 6573 2069 6e20 7468 6520 7265  ntries in the re
-00008220: 706f 7274 696e 670a 2020 2020 2020 2020  porting.        
-00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008240: 636f 6e74 6578 742c 2072 6570 7265 7365  context, represe
-00008250: 6e74 6564 2069 6e20 4953 4f20 3331 3636  nted in ISO 3166
-00008260: 2066 6f72 6d61 742e 0a20 2020 2020 2020   format..       
-00008270: 2020 2020 2020 2020 2022 2222 0a0a 2020           """..  
-00008280: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00008290: 706f 7274 696e 675f 636f 6e74 6578 743a  porting_context:
-000082a0: 2074 7970 6573 2e52 6570 6f72 7469 6e67   types.Reporting
-000082b0: 436f 6e74 6578 742e 5265 706f 7274 696e  Context.Reportin
-000082c0: 6743 6f6e 7465 7874 456e 756d 203d 2028  gContextEnum = (
-000082d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000082e0: 2020 2020 2070 726f 746f 2e46 6965 6c64       proto.Field
-000082f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00008300: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
-00008310: 454e 554d 2c0a 2020 2020 2020 2020 2020  ENUM,.          
-00008320: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00008330: 6d62 6572 3d31 2c0a 2020 2020 2020 2020  mber=1,.        
-00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008350: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
-00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008370: 2020 2020 2020 2065 6e75 6d3d 7479 7065         enum=type
-00008380: 732e 5265 706f 7274 696e 6743 6f6e 7465  s.ReportingConte
-00008390: 7874 2e52 6570 6f72 7469 6e67 436f 6e74  xt.ReportingCont
-000083a0: 6578 7445 6e75 6d2c 0a20 2020 2020 2020  extEnum,.       
-000083b0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-000083c0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000083d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000083e0: 2064 6973 6170 7072 6f76 6564 5f63 6f75   disapproved_cou
-000083f0: 6e74 7269 6573 3a20 4d75 7461 626c 6553  ntries: MutableS
-00008400: 6571 7565 6e63 655b 7374 725d 203d 2070  equence[str] = p
-00008410: 726f 746f 2e52 6570 6561 7465 6446 6965  roto.RepeatedFie
-00008420: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
-00008430: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
-00008440: 5249 4e47 2c0a 2020 2020 2020 2020 2020  RING,.          
-00008450: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-00008460: 3d32 2c0a 2020 2020 2020 2020 2020 2020  =2,.            
-00008470: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00008480: 2020 2020 2020 6465 6d6f 7465 645f 636f        demoted_co
-00008490: 756e 7472 6965 733a 204d 7574 6162 6c65  untries: Mutable
-000084a0: 5365 7175 656e 6365 5b73 7472 5d20 3d20  Sequence[str] = 
-000084b0: 7072 6f74 6f2e 5265 7065 6174 6564 4669  proto.RepeatedFi
-000084c0: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
-000084d0: 2020 2020 2020 2020 2070 726f 746f 2e53           proto.S
-000084e0: 5452 494e 472c 0a20 2020 2020 2020 2020  TRING,.         
-000084f0: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
-00008500: 723d 332c 0a20 2020 2020 2020 2020 2020  r=3,.           
-00008510: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00008520: 2020 2020 7365 7665 7269 7479 5f70 6572      severity_per
-00008530: 5f72 6570 6f72 7469 6e67 5f63 6f6e 7465  _reporting_conte
-00008540: 7874 3a20 4d75 7461 626c 6553 6571 7565  xt: MutableSeque
-00008550: 6e63 655b 0a20 2020 2020 2020 2020 2020  nce[.           
-00008560: 2020 2020 2022 5072 6f64 7563 7456 6965       "ProductVie
-00008570: 772e 4974 656d 4973 7375 652e 4974 656d  w.ItemIssue.Item
-00008580: 4973 7375 6553 6576 6572 6974 792e 4973  IssueSeverity.Is
-00008590: 7375 6553 6576 6572 6974 7950 6572 5265  sueSeverityPerRe
-000085a0: 706f 7274 696e 6743 6f6e 7465 7874 220a  portingContext".
-000085b0: 2020 2020 2020 2020 2020 2020 5d20 3d20              ] = 
-000085c0: 7072 6f74 6f2e 5265 7065 6174 6564 4669  proto.RepeatedFi
-000085d0: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
-000085e0: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
-000085f0: 4745 2c0a 2020 2020 2020 2020 2020 2020  GE,.            
-00008600: 2020 2020 6e75 6d62 6572 3d31 2c0a 2020      number=1,.  
-00008610: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00008620: 7373 6167 653d 2250 726f 6475 6374 5669  ssage="ProductVi
-00008630: 6577 2e49 7465 6d49 7373 7565 2e49 7465  ew.ItemIssue.Ite
-00008640: 6d49 7373 7565 5365 7665 7269 7479 2e49  mIssueSeverity.I
-00008650: 7373 7565 5365 7665 7269 7479 5065 7252  ssueSeverityPerR
-00008660: 6570 6f72 7469 6e67 436f 6e74 6578 7422  eportingContext"
-00008670: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00008680: 2020 2020 2020 2020 2020 2020 6167 6772              aggr
-00008690: 6567 6174 6564 5f73 6576 6572 6974 793a  egated_severity:
-000086a0: 2022 5072 6f64 7563 7456 6965 772e 4974   "ProductView.It
-000086b0: 656d 4973 7375 652e 4974 656d 4973 7375  emIssue.ItemIssu
-000086c0: 6553 6576 6572 6974 792e 4167 6772 6567  eSeverity.Aggreg
-000086d0: 6174 6564 4973 7375 6553 6576 6572 6974  atedIssueSeverit
-000086e0: 7922 203d 2070 726f 746f 2e46 6965 6c64  y" = proto.Field
-000086f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00008700: 2020 7072 6f74 6f2e 454e 554d 2c0a 2020    proto.ENUM,.  
-00008710: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00008720: 6d62 6572 3d32 2c0a 2020 2020 2020 2020  mber=2,.        
-00008730: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-00008740: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-00008750: 2020 2020 2020 2065 6e75 6d3d 2250 726f         enum="Pro
-00008760: 6475 6374 5669 6577 2e49 7465 6d49 7373  ductView.ItemIss
-00008770: 7565 2e49 7465 6d49 7373 7565 5365 7665  ue.ItemIssueSeve
-00008780: 7269 7479 2e41 6767 7265 6761 7465 6449  rity.AggregatedI
-00008790: 7373 7565 5365 7665 7269 7479 222c 0a20  ssueSeverity",. 
-000087a0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-000087b0: 2020 2020 2020 7479 7065 5f3a 2022 5072        type_: "Pr
-000087c0: 6f64 7563 7456 6965 772e 4974 656d 4973  oductView.ItemIs
-000087d0: 7375 652e 4974 656d 4973 7375 6554 7970  sue.ItemIssueTyp
-000087e0: 6522 203d 2070 726f 746f 2e46 6965 6c64  e" = proto.Field
-000087f0: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
-00008800: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
-00008810: 2020 2020 2020 2020 206e 756d 6265 723d           number=
-00008820: 312c 0a20 2020 2020 2020 2020 2020 206d  1,.            m
-00008830: 6573 7361 6765 3d22 5072 6f64 7563 7456  essage="ProductV
-00008840: 6965 772e 4974 656d 4973 7375 652e 4974  iew.ItemIssue.It
-00008850: 656d 4973 7375 6554 7970 6522 2c0a 2020  emIssueType",.  
-00008860: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00008870: 7365 7665 7269 7479 3a20 2250 726f 6475  severity: "Produ
-00008880: 6374 5669 6577 2e49 7465 6d49 7373 7565  ctView.ItemIssue
-00008890: 2e49 7465 6d49 7373 7565 5365 7665 7269  .ItemIssueSeveri
-000088a0: 7479 2220 3d20 7072 6f74 6f2e 4669 656c  ty" = proto.Fiel
-000088b0: 6428 0a20 2020 2020 2020 2020 2020 2070  d(.            p
-000088c0: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
-000088d0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-000088e0: 3d32 2c0a 2020 2020 2020 2020 2020 2020  =2,.            
-000088f0: 6d65 7373 6167 653d 2250 726f 6475 6374  message="Product
-00008900: 5669 6577 2e49 7465 6d49 7373 7565 2e49  View.ItemIssue.I
-00008910: 7465 6d49 7373 7565 5365 7665 7269 7479  temIssueSeverity
-00008920: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
-00008930: 2020 2020 2072 6573 6f6c 7574 696f 6e3a       resolution:
-00008940: 2022 5072 6f64 7563 7456 6965 772e 4974   "ProductView.It
-00008950: 656d 4973 7375 652e 4974 656d 4973 7375  emIssue.ItemIssu
-00008960: 6552 6573 6f6c 7574 696f 6e22 203d 2070  eResolution" = p
-00008970: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00008980: 2020 2020 2020 2020 7072 6f74 6f2e 454e          proto.EN
-00008990: 554d 2c0a 2020 2020 2020 2020 2020 2020  UM,.            
-000089a0: 6e75 6d62 6572 3d33 2c0a 2020 2020 2020  number=3,.      
-000089b0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-000089c0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-000089d0: 2065 6e75 6d3d 2250 726f 6475 6374 5669   enum="ProductVi
-000089e0: 6577 2e49 7465 6d49 7373 7565 2e49 7465  ew.ItemIssue.Ite
-000089f0: 6d49 7373 7565 5265 736f 6c75 7469 6f6e  mIssueResolution
-00008a00: 222c 0a20 2020 2020 2020 2029 0a0a 2020  ",.        )..  
-00008a10: 2020 6964 3a20 7374 7220 3d20 7072 6f74    id: str = prot
-00008a20: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00008a30: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-00008a40: 2020 2020 2020 206e 756d 6265 723d 312c         number=1,
-00008a50: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-00008a60: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-00008a70: 2020 6368 616e 6e65 6c3a 2074 7970 6573    channel: types
-00008a80: 2e43 6861 6e6e 656c 2e43 6861 6e6e 656c  .Channel.Channel
-00008a90: 456e 756d 203d 2070 726f 746f 2e46 6965  Enum = proto.Fie
-00008aa0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00008ab0: 6f2e 454e 554d 2c0a 2020 2020 2020 2020  o.ENUM,.        
-00008ac0: 6e75 6d62 6572 3d32 382c 0a20 2020 2020  number=28,.     
-00008ad0: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-00008ae0: 2c0a 2020 2020 2020 2020 656e 756d 3d74  ,.        enum=t
-00008af0: 7970 6573 2e43 6861 6e6e 656c 2e43 6861  ypes.Channel.Cha
-00008b00: 6e6e 656c 456e 756d 2c0a 2020 2020 290a  nnelEnum,.    ).
-00008b10: 2020 2020 6c61 6e67 7561 6765 5f63 6f64      language_cod
-00008b20: 653a 2073 7472 203d 2070 726f 746f 2e46  e: str = proto.F
-00008b30: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-00008b40: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
-00008b50: 2020 2020 6e75 6d62 6572 3d32 2c0a 2020      number=2,.  
-00008b60: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-00008b70: 7275 652c 0a20 2020 2029 0a20 2020 2066  rue,.    ).    f
-00008b80: 6565 645f 6c61 6265 6c3a 2073 7472 203d  eed_label: str =
-00008b90: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-00008ba0: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-00008bb0: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-00008bc0: 6572 3d33 2c0a 2020 2020 2020 2020 6f70  er=3,.        op
-00008bd0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-00008be0: 2029 0a20 2020 206f 6666 6572 5f69 643a   ).    offer_id:
-00008bf0: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-00008c00: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00008c10: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-00008c20: 2020 6e75 6d62 6572 3d34 2c0a 2020 2020    number=4,.    
-00008c30: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-00008c40: 652c 0a20 2020 2029 0a20 2020 2074 6974  e,.    ).    tit
-00008c50: 6c65 3a20 7374 7220 3d20 7072 6f74 6f2e  le: str = proto.
-00008c60: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00008c70: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-00008c80: 2020 2020 206e 756d 6265 723d 352c 0a20       number=5,. 
-00008c90: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-00008ca0: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
-00008cb0: 6272 616e 643a 2073 7472 203d 2070 726f  brand: str = pro
-00008cc0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-00008cd0: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
-00008ce0: 2020 2020 2020 2020 6e75 6d62 6572 3d36          number=6
-00008cf0: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-00008d00: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-00008d10: 2020 2063 6174 6567 6f72 795f 6c31 3a20     category_l1: 
-00008d20: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-00008d30: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-00008d40: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
-00008d50: 206e 756d 6265 723d 372c 0a20 2020 2020   number=7,.     
-00008d60: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-00008d70: 2c0a 2020 2020 290a 2020 2020 6361 7465  ,.    ).    cate
-00008d80: 676f 7279 5f6c 323a 2073 7472 203d 2070  gory_l2: str = p
-00008d90: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00008da0: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
-00008db0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-00008dc0: 3d38 2c0a 2020 2020 2020 2020 6f70 7469  =8,.        opti
-00008dd0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-00008de0: 0a20 2020 2063 6174 6567 6f72 795f 6c33  .    category_l3
-00008df0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-00008e00: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-00008e10: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-00008e20: 2020 206e 756d 6265 723d 392c 0a20 2020     number=9,.   
-00008e30: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-00008e40: 7565 2c0a 2020 2020 290a 2020 2020 6361  ue,.    ).    ca
-00008e50: 7465 676f 7279 5f6c 343a 2073 7472 203d  tegory_l4: str =
-00008e60: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-00008e70: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-00008e80: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-00008e90: 6572 3d31 302c 0a20 2020 2020 2020 206f  er=10,.        o
-00008ea0: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-00008eb0: 2020 290a 2020 2020 6361 7465 676f 7279    ).    category
-00008ec0: 5f6c 353a 2073 7472 203d 2070 726f 746f  _l5: str = proto
-00008ed0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00008ee0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-00008ef0: 2020 2020 2020 6e75 6d62 6572 3d31 312c        number=11,
-00008f00: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-00008f10: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-00008f20: 2020 7072 6f64 7563 745f 7479 7065 5f6c    product_type_l
-00008f30: 313a 2073 7472 203d 2070 726f 746f 2e46  1: str = proto.F
-00008f40: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-00008f50: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
-00008f60: 2020 2020 6e75 6d62 6572 3d31 322c 0a20      number=12,. 
-00008f70: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-00008f80: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
-00008f90: 7072 6f64 7563 745f 7479 7065 5f6c 323a  product_type_l2:
-00008fa0: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-00008fb0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00008fc0: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-00008fd0: 2020 6e75 6d62 6572 3d31 332c 0a20 2020    number=13,.   
-00008fe0: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-00008ff0: 7565 2c0a 2020 2020 290a 2020 2020 7072  ue,.    ).    pr
-00009000: 6f64 7563 745f 7479 7065 5f6c 333a 2073  oduct_type_l3: s
-00009010: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
-00009020: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-00009030: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-00009040: 6e75 6d62 6572 3d31 342c 0a20 2020 2020  number=14,.     
-00009050: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-00009060: 2c0a 2020 2020 290a 2020 2020 7072 6f64  ,.    ).    prod
-00009070: 7563 745f 7479 7065 5f6c 343a 2073 7472  uct_type_l4: str
-00009080: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00009090: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
-000090a0: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
-000090b0: 6d62 6572 3d31 352c 0a20 2020 2020 2020  mber=15,.       
-000090c0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-000090d0: 2020 2020 290a 2020 2020 7072 6f64 7563      ).    produc
-000090e0: 745f 7479 7065 5f6c 353a 2073 7472 203d  t_type_l5: str =
-000090f0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-00009100: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-00009110: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-00009120: 6572 3d31 362c 0a20 2020 2020 2020 206f  er=16,.        o
-00009130: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-00009140: 2020 290a 2020 2020 7072 6963 653a 2074    ).    price: t
-00009150: 7970 6573 2e50 7269 6365 203d 2070 726f  ypes.Price = pro
-00009160: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-00009170: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
-00009180: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-00009190: 3137 2c0a 2020 2020 2020 2020 6d65 7373  17,.        mess
-000091a0: 6167 653d 7479 7065 732e 5072 6963 652c  age=types.Price,
-000091b0: 0a20 2020 2029 0a20 2020 2063 6f6e 6469  .    ).    condi
-000091c0: 7469 6f6e 3a20 7374 7220 3d20 7072 6f74  tion: str = prot
-000091d0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-000091e0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-000091f0: 2020 2020 2020 206e 756d 6265 723d 3138         number=18
-00009200: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-00009210: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-00009220: 2020 2061 7661 696c 6162 696c 6974 793a     availability:
-00009230: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-00009240: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00009250: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-00009260: 2020 6e75 6d62 6572 3d31 392c 0a20 2020    number=19,.   
-00009270: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-00009280: 7565 2c0a 2020 2020 290a 2020 2020 7368  ue,.    ).    sh
-00009290: 6970 7069 6e67 5f6c 6162 656c 3a20 7374  ipping_label: st
-000092a0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-000092b0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-000092c0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-000092d0: 756d 6265 723d 3230 2c0a 2020 2020 2020  umber=20,.      
-000092e0: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-000092f0: 0a20 2020 2029 0a20 2020 2067 7469 6e3a  .    ).    gtin:
-00009300: 204d 7574 6162 6c65 5365 7175 656e 6365   MutableSequence
-00009310: 5b73 7472 5d20 3d20 7072 6f74 6f2e 5265  [str] = proto.Re
-00009320: 7065 6174 6564 4669 656c 6428 0a20 2020  peatedField(.   
-00009330: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-00009340: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-00009350: 723d 3231 2c0a 2020 2020 290a 2020 2020  r=21,.    ).    
-00009360: 6974 656d 5f67 726f 7570 5f69 643a 2073  item_group_id: s
-00009370: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
-00009380: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-00009390: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-000093a0: 6e75 6d62 6572 3d32 322c 0a20 2020 2020  number=22,.     
-000093b0: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-000093c0: 2c0a 2020 2020 290a 2020 2020 7468 756d  ,.    ).    thum
-000093d0: 626e 6169 6c5f 6c69 6e6b 3a20 7374 7220  bnail_link: str 
-000093e0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-000093f0: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-00009400: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-00009410: 6265 723d 3233 2c0a 2020 2020 2020 2020  ber=23,.        
-00009420: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
-00009430: 2020 2029 0a20 2020 2063 7265 6174 696f     ).    creatio
-00009440: 6e5f 7469 6d65 3a20 7469 6d65 7374 616d  n_time: timestam
-00009450: 705f 7062 322e 5469 6d65 7374 616d 7020  p_pb2.Timestamp 
-00009460: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00009470: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
-00009480: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
-00009490: 6d62 6572 3d32 342c 0a20 2020 2020 2020  mber=24,.       
-000094a0: 206d 6573 7361 6765 3d74 696d 6573 7461   message=timesta
-000094b0: 6d70 5f70 6232 2e54 696d 6573 7461 6d70  mp_pb2.Timestamp
-000094c0: 2c0a 2020 2020 290a 2020 2020 6578 7069  ,.    ).    expi
-000094d0: 7261 7469 6f6e 5f64 6174 653a 2064 6174  ration_date: dat
-000094e0: 655f 7062 322e 4461 7465 203d 2070 726f  e_pb2.Date = pro
-000094f0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-00009500: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
-00009510: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-00009520: 3235 2c0a 2020 2020 2020 2020 6d65 7373  25,.        mess
-00009530: 6167 653d 6461 7465 5f70 6232 2e44 6174  age=date_pb2.Dat
-00009540: 652c 0a20 2020 2029 0a20 2020 2061 6767  e,.    ).    agg
-00009550: 7265 6761 7465 645f 7265 706f 7274 696e  regated_reportin
-00009560: 675f 636f 6e74 6578 745f 7374 6174 7573  g_context_status
-00009570: 3a20 4167 6772 6567 6174 6564 5265 706f  : AggregatedRepo
-00009580: 7274 696e 6743 6f6e 7465 7874 5374 6174  rtingContextStat
-00009590: 7573 203d 2070 726f 746f 2e46 6965 6c64  us = proto.Field
-000095a0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-000095b0: 454e 554d 2c0a 2020 2020 2020 2020 6e75  ENUM,.        nu
-000095c0: 6d62 6572 3d32 362c 0a20 2020 2020 2020  mber=26,.       
-000095d0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-000095e0: 2020 2020 2020 2020 656e 756d 3d41 6767          enum=Agg
-000095f0: 7265 6761 7465 6452 6570 6f72 7469 6e67  regatedReporting
-00009600: 436f 6e74 6578 7453 7461 7475 732c 0a20  ContextStatus,. 
-00009610: 2020 2029 0a20 2020 2069 7465 6d5f 6973     ).    item_is
-00009620: 7375 6573 3a20 4d75 7461 626c 6553 6571  sues: MutableSeq
-00009630: 7565 6e63 655b 4974 656d 4973 7375 655d  uence[ItemIssue]
-00009640: 203d 2070 726f 746f 2e52 6570 6561 7465   = proto.Repeate
-00009650: 6446 6965 6c64 280a 2020 2020 2020 2020  dField(.        
-00009660: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
-00009670: 2020 2020 2020 206e 756d 6265 723d 3237         number=27
-00009680: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
-00009690: 653d 4974 656d 4973 7375 652c 0a20 2020  e=ItemIssue,.   
-000096a0: 2029 0a20 2020 2063 6c69 636b 5f70 6f74   ).    click_pot
-000096b0: 656e 7469 616c 3a20 436c 6963 6b50 6f74  ential: ClickPot
-000096c0: 656e 7469 616c 203d 2070 726f 746f 2e46  ential = proto.F
-000096d0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-000096e0: 6f74 6f2e 454e 554d 2c0a 2020 2020 2020  oto.ENUM,.      
-000096f0: 2020 6e75 6d62 6572 3d32 392c 0a20 2020    number=29,.   
-00009700: 2020 2020 2065 6e75 6d3d 436c 6963 6b50       enum=ClickP
-00009710: 6f74 656e 7469 616c 2c0a 2020 2020 290a  otential,.    ).
-00009720: 2020 2020 636c 6963 6b5f 706f 7465 6e74      click_potent
-00009730: 6961 6c5f 7261 6e6b 3a20 696e 7420 3d20  ial_rank: int = 
-00009740: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00009750: 2020 2020 2070 726f 746f 2e49 4e54 3634       proto.INT64
-00009760: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-00009770: 3d33 302c 0a20 2020 2020 2020 206f 7074  =30,.        opt
-00009780: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-00009790: 290a 0a0a 636c 6173 7320 5072 6963 6543  )...class PriceC
-000097a0: 6f6d 7065 7469 7469 7665 6e65 7373 5072  ompetitivenessPr
-000097b0: 6f64 7563 7456 6965 7728 7072 6f74 6f2e  oductView(proto.
-000097c0: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
-000097d0: 2222 4669 656c 6473 2061 7661 696c 6162  ""Fields availab
-000097e0: 6c65 2066 6f72 2071 7565 7279 2069 6e20  le for query in 
-000097f0: 6060 7072 6963 655f 636f 6d70 6574 6974  ``price_competit
-00009800: 6976 656e 6573 735f 7072 6f64 7563 745f  iveness_product_
-00009810: 7669 6577 6060 0a20 2020 2074 6162 6c65  view``.    table
-00009820: 2e0a 0a20 2020 2060 5072 6963 650a 2020  ...    `Price.  
-00009830: 2020 636f 6d70 6574 6974 6976 656e 6573    competitivenes
-00009840: 7320 3c68 7474 7073 3a2f 2f73 7570 706f  s <https://suppo
-00009850: 7274 2e67 6f6f 676c 652e 636f 6d2f 6d65  rt.google.com/me
-00009860: 7263 6861 6e74 732f 616e 7377 6572 2f39  rchants/answer/9
-00009870: 3632 3639 3033 3e60 5f5f 0a20 2020 2072  626903>`__.    r
-00009880: 6570 6f72 742e 0a0a 2020 2020 5661 6c75  eport...    Valu
-00009890: 6573 2061 7265 206f 6e6c 7920 7365 7420  es are only set 
-000098a0: 666f 7220 6669 656c 6473 2072 6571 7565  for fields reque
-000098b0: 7374 6564 2065 7870 6c69 6369 746c 7920  sted explicitly 
-000098c0: 696e 2074 6865 2072 6571 7565 7374 2773  in the request's
-000098d0: 0a20 2020 2073 6561 7263 6820 7175 6572  .    search quer
-000098e0: 792e 0a0a 0a20 2020 202e 2e20 5f6f 6e65  y....    .. _one
-000098f0: 6f66 3a20 6874 7470 733a 2f2f 7072 6f74  of: https://prot
-00009900: 6f2d 706c 7573 2d70 7974 686f 6e2e 7265  o-plus-python.re
-00009910: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00009920: 7374 6162 6c65 2f66 6965 6c64 732e 6874  stable/fields.ht
-00009930: 6d6c 236f 6e65 6f66 732d 6d75 7475 616c  ml#oneofs-mutual
-00009940: 6c79 2d65 7863 6c75 7369 7665 2d66 6965  ly-exclusive-fie
-00009950: 6c64 730a 0a20 2020 2041 7474 7269 6275  lds..    Attribu
-00009960: 7465 733a 0a20 2020 2020 2020 2072 6570  tes:.        rep
-00009970: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
-00009980: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
-00009990: 2020 2020 436f 756e 7472 7920 6f66 2074      Country of t
-000099a0: 6865 2070 7269 6365 2062 656e 6368 6d61  he price benchma
-000099b0: 726b 2e20 5265 7072 6573 656e 7465 6420  rk. Represented 
-000099c0: 696e 2074 6865 2049 534f 2033 3136 360a  in the ISO 3166.
-000099d0: 2020 2020 2020 2020 2020 2020 666f 726d              form
-000099e0: 6174 2e0a 0a20 2020 2020 2020 2020 2020  at...           
-000099f0: 2052 6571 7569 7265 6420 696e 2074 6865   Required in the
-00009a00: 2060 6053 454c 4543 5460 6020 636c 6175   ``SELECT`` clau
-00009a10: 7365 2e0a 0a20 2020 2020 2020 2020 2020  se...           
-00009a20: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-00009a30: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-00009a40: 6660 5f20 6060 5f72 6570 6f72 745f 636f  f`_ ``_report_co
-00009a50: 756e 7472 795f 636f 6465 6060 2e0a 2020  untry_code``..  
-00009a60: 2020 2020 2020 6964 2028 7374 7229 3a0a        id (str):.
-00009a70: 2020 2020 2020 2020 2020 2020 5245 5354              REST
-00009a80: 2049 4420 6f66 2074 6865 2070 726f 6475   ID of the produ
-00009a90: 6374 2c20 696e 2074 6865 2066 6f72 6d20  ct, in the form 
-00009aa0: 6f66 0a20 2020 2020 2020 2020 2020 2060  of.            `
-00009ab0: 6063 6861 6e6e 656c 7e6c 616e 6775 6167  `channel~languag
-00009ac0: 6543 6f64 657e 6665 6564 4c61 6265 6c7e  eCode~feedLabel~
-00009ad0: 6f66 6665 7249 6460 602e 2043 616e 2062  offerId``. Can b
-00009ae0: 6520 7573 6564 2074 6f0a 2020 2020 2020  e used to.      
-00009af0: 2020 2020 2020 6a6f 696e 2064 6174 6120        join data 
-00009b00: 7769 7468 2074 6865 2060 6070 726f 6475  with the ``produ
-00009b10: 6374 5f76 6965 7760 6020 7461 626c 652e  ct_view`` table.
-00009b20: 0a0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
-00009b30: 7175 6972 6564 2069 6e20 7468 6520 6060  quired in the ``
-00009b40: 5345 4c45 4354 6060 2063 6c61 7573 652e  SELECT`` clause.
-00009b50: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00009b60: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-00009b70: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-00009b80: 2060 605f 6964 6060 2e0a 2020 2020 2020   ``_id``..      
-00009b90: 2020 6f66 6665 725f 6964 2028 7374 7229    offer_id (str)
-00009ba0: 3a0a 2020 2020 2020 2020 2020 2020 4d65  :.            Me
-00009bb0: 7263 6861 6e74 2d70 726f 7669 6465 6420  rchant-provided 
-00009bc0: 6964 206f 6620 7468 6520 7072 6f64 7563  id of the produc
-00009bd0: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
-00009be0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-00009bf0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-00009c00: 605f 2060 605f 6f66 6665 725f 6964 6060  `_ ``_offer_id``
-00009c10: 2e0a 2020 2020 2020 2020 7469 746c 6520  ..        title 
-00009c20: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-00009c30: 2020 2054 6974 6c65 206f 6620 7468 6520     Title of the 
-00009c40: 7072 6f64 7563 742e 0a0a 2020 2020 2020  product...      
-00009c50: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-00009c60: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-00009c70: 606f 6e65 6f66 605f 2060 605f 7469 746c  `oneof`_ ``_titl
-00009c80: 6560 602e 0a20 2020 2020 2020 2062 7261  e``..        bra
-00009c90: 6e64 2028 7374 7229 3a0a 2020 2020 2020  nd (str):.      
-00009ca0: 2020 2020 2020 4272 616e 6420 6f66 2074        Brand of t
-00009cb0: 6865 2070 726f 6475 6374 2e0a 0a20 2020  he product...   
-00009cc0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-00009cd0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-00009ce0: 6f66 2060 6f6e 656f 6660 5f20 6060 5f62  of `oneof`_ ``_b
-00009cf0: 7261 6e64 6060 2e0a 2020 2020 2020 2020  rand``..        
-00009d00: 6361 7465 676f 7279 5f6c 3120 2873 7472  category_l1 (str
-00009d10: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
-00009d20: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
-00009d30: 2831 7374 206c 6576 656c 2920 696e 2060  (1st level) in `
-00009d40: 476f 6f67 6c65 2773 2070 726f 6475 6374  Google's product
-00009d50: 0a20 2020 2020 2020 2020 2020 2074 6178  .            tax
-00009d60: 6f6e 6f6d 7920 3c68 7474 7073 3a2f 2f73  onomy <https://s
-00009d70: 7570 706f 7274 2e67 6f6f 676c 652e 636f  upport.google.co
-00009d80: 6d2f 6d65 7263 6861 6e74 732f 616e 7377  m/merchants/answ
-00009d90: 6572 2f36 3332 3434 3336 3e60 5f5f 2e0a  er/6324436>`__..
-00009da0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-00009db0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-00009dc0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-00009dd0: 6060 5f63 6174 6567 6f72 795f 6c31 6060  ``_category_l1``
-00009de0: 2e0a 2020 2020 2020 2020 6361 7465 676f  ..        catego
-00009df0: 7279 5f6c 3220 2873 7472 293a 0a20 2020  ry_l2 (str):.   
-00009e00: 2020 2020 2020 2020 2050 726f 6475 6374           Product
-00009e10: 2063 6174 6567 6f72 7920 2832 6e64 206c   category (2nd l
-00009e20: 6576 656c 2920 696e 2060 476f 6f67 6c65  evel) in `Google
-00009e30: 2773 2070 726f 6475 6374 0a20 2020 2020  's product.     
-00009e40: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
-00009e50: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
-00009e60: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-00009e70: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
-00009e80: 3434 3336 3e60 5f5f 2e0a 0a20 2020 2020  4436>`__...     
-00009e90: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-00009ea0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-00009eb0: 2060 6f6e 656f 6660 5f20 6060 5f63 6174   `oneof`_ ``_cat
-00009ec0: 6567 6f72 795f 6c32 6060 2e0a 2020 2020  egory_l2``..    
-00009ed0: 2020 2020 6361 7465 676f 7279 5f6c 3320      category_l3 
-00009ee0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-00009ef0: 2020 2050 726f 6475 6374 2063 6174 6567     Product categ
-00009f00: 6f72 7920 2833 7264 206c 6576 656c 2920  ory (3rd level) 
-00009f10: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
-00009f20: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
-00009f30: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
-00009f40: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-00009f50: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-00009f60: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
-00009f70: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
-00009f80: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-00009f90: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-00009fa0: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
-00009fb0: 6c33 6060 2e0a 2020 2020 2020 2020 6361  l3``..        ca
-00009fc0: 7465 676f 7279 5f6c 3420 2873 7472 293a  tegory_l4 (str):
-00009fd0: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
-00009fe0: 6475 6374 2063 6174 6567 6f72 7920 2834  duct category (4
-00009ff0: 7468 206c 6576 656c 2920 696e 2060 476f  th level) in `Go
-0000a000: 6f67 6c65 2773 2070 726f 6475 6374 0a20  ogle's product. 
-0000a010: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
-0000a020: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
-0000a030: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-0000a040: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-0000a050: 2f36 3332 3434 3336 3e60 5f5f 2e0a 0a20  /6324436>`__... 
-0000a060: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-0000a070: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-0000a080: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-0000a090: 5f63 6174 6567 6f72 795f 6c34 6060 2e0a  _category_l4``..
-0000a0a0: 2020 2020 2020 2020 6361 7465 676f 7279          category
-0000a0b0: 5f6c 3520 2873 7472 293a 0a20 2020 2020  _l5 (str):.     
-0000a0c0: 2020 2020 2020 2050 726f 6475 6374 2063         Product c
-0000a0d0: 6174 6567 6f72 7920 2835 7468 206c 6576  ategory (5th lev
-0000a0e0: 656c 2920 696e 2060 476f 6f67 6c65 2773  el) in `Google's
-0000a0f0: 2070 726f 6475 6374 0a20 2020 2020 2020   product.       
-0000a100: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
-0000a110: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
-0000a120: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
-0000a130: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
-0000a140: 3336 3e60 5f5f 2e0a 0a20 2020 2020 2020  36>`__...       
-0000a150: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-0000a160: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-0000a170: 6f6e 656f 6660 5f20 6060 5f63 6174 6567  oneof`_ ``_categ
-0000a180: 6f72 795f 6c35 6060 2e0a 2020 2020 2020  ory_l5``..      
-0000a190: 2020 7072 6f64 7563 745f 7479 7065 5f6c    product_type_l
-0000a1a0: 3120 2873 7472 293a 0a20 2020 2020 2020  1 (str):.       
-0000a1b0: 2020 2020 2050 726f 6475 6374 2074 7970       Product typ
-0000a1c0: 6520 2831 7374 206c 6576 656c 2920 696e  e (1st level) in
-0000a1d0: 206d 6572 6368 616e 7427 7320 6f77 6e20   merchant's own 
-0000a1e0: 6070 726f 6475 6374 0a20 2020 2020 2020  `product.       
-0000a1f0: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
-0000a200: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
-0000a210: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
-0000a220: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
-0000a230: 3036 3e60 5f5f 2e0a 0a20 2020 2020 2020  06>`__...       
-0000a240: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-0000a250: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-0000a260: 6f6e 656f 6660 5f20 6060 5f70 726f 6475  oneof`_ ``_produ
-0000a270: 6374 5f74 7970 655f 6c31 6060 2e0a 2020  ct_type_l1``..  
-0000a280: 2020 2020 2020 7072 6f64 7563 745f 7479        product_ty
-0000a290: 7065 5f6c 3220 2873 7472 293a 0a20 2020  pe_l2 (str):.   
-0000a2a0: 2020 2020 2020 2020 2050 726f 6475 6374           Product
-0000a2b0: 2074 7970 6520 2832 6e64 206c 6576 656c   type (2nd level
-0000a2c0: 2920 696e 206d 6572 6368 616e 7427 7320  ) in merchant's 
-0000a2d0: 6f77 6e20 6070 726f 6475 6374 0a20 2020  own `product.   
-0000a2e0: 2020 2020 2020 2020 2074 6178 6f6e 6f6d           taxonom
-0000a2f0: 7920 3c68 7474 7073 3a2f 2f73 7570 706f  y <https://suppo
-0000a300: 7274 2e67 6f6f 676c 652e 636f 6d2f 6d65  rt.google.com/me
-0000a310: 7263 6861 6e74 732f 616e 7377 6572 2f36  rchants/answer/6
-0000a320: 3332 3434 3036 3e60 5f5f 2e0a 0a20 2020  324406>`__...   
-0000a330: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-0000a340: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-0000a350: 6f66 2060 6f6e 656f 6660 5f20 6060 5f70  of `oneof`_ ``_p
-0000a360: 726f 6475 6374 5f74 7970 655f 6c32 6060  roduct_type_l2``
-0000a370: 2e0a 2020 2020 2020 2020 7072 6f64 7563  ..        produc
-0000a380: 745f 7479 7065 5f6c 3320 2873 7472 293a  t_type_l3 (str):
-0000a390: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
-0000a3a0: 6475 6374 2074 7970 6520 2833 7264 206c  duct type (3rd l
-0000a3b0: 6576 656c 2920 696e 206d 6572 6368 616e  evel) in merchan
-0000a3c0: 7427 7320 6f77 6e20 6070 726f 6475 6374  t's own `product
-0000a3d0: 0a20 2020 2020 2020 2020 2020 2074 6178  .            tax
-0000a3e0: 6f6e 6f6d 7920 3c68 7474 7073 3a2f 2f73  onomy <https://s
-0000a3f0: 7570 706f 7274 2e67 6f6f 676c 652e 636f  upport.google.co
-0000a400: 6d2f 6d65 7263 6861 6e74 732f 616e 7377  m/merchants/answ
-0000a410: 6572 2f36 3332 3434 3036 3e60 5f5f 2e0a  er/6324406>`__..
-0000a420: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-0000a430: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-0000a440: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-0000a450: 6060 5f70 726f 6475 6374 5f74 7970 655f  ``_product_type_
-0000a460: 6c33 6060 2e0a 2020 2020 2020 2020 7072  l3``..        pr
-0000a470: 6f64 7563 745f 7479 7065 5f6c 3420 2873  oduct_type_l4 (s
-0000a480: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-0000a490: 2050 726f 6475 6374 2074 7970 6520 2834   Product type (4
-0000a4a0: 7468 206c 6576 656c 2920 696e 206d 6572  th level) in mer
-0000a4b0: 6368 616e 7427 7320 6f77 6e20 6070 726f  chant's own `pro
-0000a4c0: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
-0000a4d0: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
-0000a4e0: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-0000a4f0: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-0000a500: 616e 7377 6572 2f36 3332 3434 3036 3e60  answer/6324406>`
-0000a510: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
-0000a520: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-0000a530: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-0000a540: 6660 5f20 6060 5f70 726f 6475 6374 5f74  f`_ ``_product_t
-0000a550: 7970 655f 6c34 6060 2e0a 2020 2020 2020  ype_l4``..      
-0000a560: 2020 7072 6f64 7563 745f 7479 7065 5f6c    product_type_l
-0000a570: 3520 2873 7472 293a 0a20 2020 2020 2020  5 (str):.       
-0000a580: 2020 2020 2050 726f 6475 6374 2074 7970       Product typ
-0000a590: 6520 2835 7468 206c 6576 656c 2920 696e  e (5th level) in
-0000a5a0: 206d 6572 6368 616e 7427 7320 6f77 6e20   merchant's own 
-0000a5b0: 6070 726f 6475 6374 0a20 2020 2020 2020  `product.       
-0000a5c0: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
-0000a5d0: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
-0000a5e0: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
-0000a5f0: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
-0000a600: 3036 3e60 5f5f 2e0a 0a20 2020 2020 2020  06>`__...       
-0000a610: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-0000a620: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-0000a630: 6f6e 656f 6660 5f20 6060 5f70 726f 6475  oneof`_ ``_produ
-0000a640: 6374 5f74 7970 655f 6c35 6060 2e0a 2020  ct_type_l5``..  
-0000a650: 2020 2020 2020 7072 6963 6520 2867 6f6f        price (goo
-0000a660: 676c 652e 7368 6f70 7069 6e67 2e74 7970  gle.shopping.typ
-0000a670: 652e 7479 7065 732e 5072 6963 6529 3a0a  e.types.Price):.
-0000a680: 2020 2020 2020 2020 2020 2020 4375 7272              Curr
-0000a690: 656e 7420 7072 6963 6520 6f66 2074 6865  ent price of the
-0000a6a0: 2070 726f 6475 6374 2e0a 2020 2020 2020   product..      
-0000a6b0: 2020 6265 6e63 686d 6172 6b5f 7072 6963    benchmark_pric
-0000a6c0: 6520 2867 6f6f 676c 652e 7368 6f70 7069  e (google.shoppi
-0000a6d0: 6e67 2e74 7970 652e 7479 7065 732e 5072  ng.type.types.Pr
-0000a6e0: 6963 6529 3a0a 2020 2020 2020 2020 2020  ice):.          
-0000a6f0: 2020 4c61 7465 7374 2061 7661 696c 6162    Latest availab
-0000a700: 6c65 2070 7269 6365 2062 656e 6368 6d61  le price benchma
-0000a710: 726b 2066 6f72 2074 6865 0a20 2020 2020  rk for the.     
-0000a720: 2020 2020 2020 2070 726f 6475 6374 2773         product's
-0000a730: 2063 6174 616c 6f67 2069 6e20 7468 6520   catalog in the 
-0000a740: 6265 6e63 686d 6172 6b20 636f 756e 7472  benchmark countr
-0000a750: 792e 0a20 2020 2022 2222 0a0a 2020 2020  y..    """..    
-0000a760: 7265 706f 7274 5f63 6f75 6e74 7279 5f63  report_country_c
-0000a770: 6f64 653a 2073 7472 203d 2070 726f 746f  ode: str = proto
-0000a780: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000a790: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-0000a7a0: 2020 2020 2020 6e75 6d62 6572 3d31 2c0a        number=1,.
-0000a7b0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-0000a7c0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-0000a7d0: 2069 643a 2073 7472 203d 2070 726f 746f   id: str = proto
-0000a7e0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000a7f0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-0000a800: 2020 2020 2020 6e75 6d62 6572 3d32 2c0a        number=2,.
-0000a810: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-0000a820: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-0000a830: 206f 6666 6572 5f69 643a 2073 7472 203d   offer_id: str =
-0000a840: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-0000a850: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-0000a860: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-0000a870: 6572 3d33 2c0a 2020 2020 2020 2020 6f70  er=3,.        op
-0000a880: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-0000a890: 2029 0a20 2020 2074 6974 6c65 3a20 7374   ).    title: st
-0000a8a0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-0000a8b0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-0000a8c0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-0000a8d0: 756d 6265 723d 342c 0a20 2020 2020 2020  umber=4,.       
-0000a8e0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-0000a8f0: 2020 2020 290a 2020 2020 6272 616e 643a      ).    brand:
-0000a900: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
-0000a910: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-0000a920: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
-0000a930: 2020 6e75 6d62 6572 3d35 2c0a 2020 2020    number=5,.    
-0000a940: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-0000a950: 652c 0a20 2020 2029 0a20 2020 2063 6174  e,.    ).    cat
-0000a960: 6567 6f72 795f 6c31 3a20 7374 7220 3d20  egory_l1: str = 
-0000a970: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000a980: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-0000a990: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-0000a9a0: 723d 362c 0a20 2020 2020 2020 206f 7074  r=6,.        opt
-0000a9b0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-0000a9c0: 290a 2020 2020 6361 7465 676f 7279 5f6c  ).    category_l
-0000a9d0: 323a 2073 7472 203d 2070 726f 746f 2e46  2: str = proto.F
-0000a9e0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-0000a9f0: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
-0000aa00: 2020 2020 6e75 6d62 6572 3d37 2c0a 2020      number=7,.  
-0000aa10: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-0000aa20: 7275 652c 0a20 2020 2029 0a20 2020 2063  rue,.    ).    c
-0000aa30: 6174 6567 6f72 795f 6c33 3a20 7374 7220  ategory_l3: str 
-0000aa40: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-0000aa50: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-0000aa60: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-0000aa70: 6265 723d 382c 0a20 2020 2020 2020 206f  ber=8,.        o
-0000aa80: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-0000aa90: 2020 290a 2020 2020 6361 7465 676f 7279    ).    category
-0000aaa0: 5f6c 343a 2073 7472 203d 2070 726f 746f  _l4: str = proto
-0000aab0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000aac0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-0000aad0: 2020 2020 2020 6e75 6d62 6572 3d39 2c0a        number=9,.
-0000aae0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-0000aaf0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-0000ab00: 2063 6174 6567 6f72 795f 6c35 3a20 7374   category_l5: st
-0000ab10: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-0000ab20: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-0000ab30: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-0000ab40: 756d 6265 723d 3130 2c0a 2020 2020 2020  umber=10,.      
-0000ab50: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-0000ab60: 0a20 2020 2029 0a20 2020 2070 726f 6475  .    ).    produ
-0000ab70: 6374 5f74 7970 655f 6c31 3a20 7374 7220  ct_type_l1: str 
-0000ab80: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-0000ab90: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-0000aba0: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-0000abb0: 6265 723d 3131 2c0a 2020 2020 2020 2020  ber=11,.        
-0000abc0: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
-0000abd0: 2020 2029 0a20 2020 2070 726f 6475 6374     ).    product
-0000abe0: 5f74 7970 655f 6c32 3a20 7374 7220 3d20  _type_l2: str = 
-0000abf0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000ac00: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-0000ac10: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-0000ac20: 723d 3132 2c0a 2020 2020 2020 2020 6f70  r=12,.        op
-0000ac30: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-0000ac40: 2029 0a20 2020 2070 726f 6475 6374 5f74   ).    product_t
-0000ac50: 7970 655f 6c33 3a20 7374 7220 3d20 7072  ype_l3: str = pr
-0000ac60: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-0000ac70: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-0000ac80: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-0000ac90: 3133 2c0a 2020 2020 2020 2020 6f70 7469  13,.        opti
-0000aca0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-0000acb0: 0a20 2020 2070 726f 6475 6374 5f74 7970  .    product_typ
-0000acc0: 655f 6c34 3a20 7374 7220 3d20 7072 6f74  e_l4: str = prot
-0000acd0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-0000ace0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-0000acf0: 2020 2020 2020 206e 756d 6265 723d 3134         number=14
-0000ad00: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-0000ad10: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-0000ad20: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
-0000ad30: 6c35 3a20 7374 7220 3d20 7072 6f74 6f2e  l5: str = proto.
-0000ad40: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-0000ad50: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-0000ad60: 2020 2020 206e 756d 6265 723d 3135 2c0a       number=15,.
-0000ad70: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-0000ad80: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-0000ad90: 2070 7269 6365 3a20 7479 7065 732e 5072   price: types.Pr
-0000ada0: 6963 6520 3d20 7072 6f74 6f2e 4669 656c  ice = proto.Fiel
-0000adb0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-0000adc0: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
-0000add0: 2020 6e75 6d62 6572 3d31 362c 0a20 2020    number=16,.   
-0000ade0: 2020 2020 206d 6573 7361 6765 3d74 7970       message=typ
-0000adf0: 6573 2e50 7269 6365 2c0a 2020 2020 290a  es.Price,.    ).
-0000ae00: 2020 2020 6265 6e63 686d 6172 6b5f 7072      benchmark_pr
-0000ae10: 6963 653a 2074 7970 6573 2e50 7269 6365  ice: types.Price
-0000ae20: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-0000ae30: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
-0000ae40: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
-0000ae50: 756d 6265 723d 3137 2c0a 2020 2020 2020  umber=17,.      
-0000ae60: 2020 6d65 7373 6167 653d 7479 7065 732e    message=types.
-0000ae70: 5072 6963 652c 0a20 2020 2029 0a0a 0a63  Price,.    )...c
-0000ae80: 6c61 7373 2050 7269 6365 496e 7369 6768  lass PriceInsigh
-0000ae90: 7473 5072 6f64 7563 7456 6965 7728 7072  tsProductView(pr
-0000aea0: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
-0000aeb0: 2020 7222 2222 4669 656c 6473 2061 7661    r"""Fields ava
-0000aec0: 696c 6162 6c65 2066 6f72 2071 7565 7279  ilable for query
-0000aed0: 2069 6e20 6060 7072 6963 655f 696e 7369   in ``price_insi
-0000aee0: 6768 7473 5f70 726f 6475 6374 5f76 6965  ghts_product_vie
-0000aef0: 7760 6020 7461 626c 652e 0a0a 2020 2020  w`` table...    
-0000af00: 6050 7269 6365 0a20 2020 2069 6e73 6967  `Price.    insig
-0000af10: 6874 7320 3c68 7474 7073 3a2f 2f73 7570  hts <https://sup
-0000af20: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-0000af30: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-0000af40: 2f31 3139 3136 3932 363e 605f 5f0a 2020  /11916926>`__.  
-0000af50: 2020 7265 706f 7274 2e0a 0a20 2020 2056    report...    V
-0000af60: 616c 7565 7320 6172 6520 6f6e 6c79 2073  alues are only s
-0000af70: 6574 2066 6f72 2066 6965 6c64 7320 7265  et for fields re
-0000af80: 7175 6573 7465 6420 6578 706c 6963 6974  quested explicit
-0000af90: 6c79 2069 6e20 7468 6520 7265 7175 6573  ly in the reques
-0000afa0: 7427 730a 2020 2020 7365 6172 6368 2071  t's.    search q
-0000afb0: 7565 7279 2e0a 0a0a 2020 2020 2e2e 205f  uery....    .. _
-0000afc0: 6f6e 656f 663a 2068 7474 7073 3a2f 2f70  oneof: https://p
-0000afd0: 726f 746f 2d70 6c75 732d 7079 7468 6f6e  roto-plus-python
-0000afe0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-0000aff0: 656e 2f73 7461 626c 652f 6669 656c 6473  en/stable/fields
-0000b000: 2e68 746d 6c23 6f6e 656f 6673 2d6d 7574  .html#oneofs-mut
-0000b010: 7561 6c6c 792d 6578 636c 7573 6976 652d  ually-exclusive-
-0000b020: 6669 656c 6473 0a0a 2020 2020 4174 7472  fields..    Attr
-0000b030: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
-0000b040: 6964 2028 7374 7229 3a0a 2020 2020 2020  id (str):.      
-0000b050: 2020 2020 2020 5245 5354 2049 4420 6f66        REST ID of
-0000b060: 2074 6865 2070 726f 6475 6374 2c20 696e   the product, in
-0000b070: 2074 6865 2066 6f72 6d20 6f66 0a20 2020   the form of.   
-0000b080: 2020 2020 2020 2020 2060 6063 6861 6e6e           ``chann
-0000b090: 656c 7e6c 616e 6775 6167 6543 6f64 657e  el~languageCode~
-0000b0a0: 6665 6564 4c61 6265 6c7e 6f66 6665 7249  feedLabel~offerI
-0000b0b0: 6460 602e 2043 616e 2062 6520 7573 6564  d``. Can be used
-0000b0c0: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-0000b0d0: 6a6f 696e 2064 6174 6120 7769 7468 2074  join data with t
-0000b0e0: 6865 2060 6070 726f 6475 6374 5f76 6965  he ``product_vie
-0000b0f0: 7760 6020 7461 626c 652e 0a0a 2020 2020  w`` table...    
-0000b100: 2020 2020 2020 2020 5265 7175 6972 6564          Required
-0000b110: 2069 6e20 7468 6520 6060 5345 4c45 4354   in the ``SELECT
-0000b120: 6060 2063 6c61 7573 652e 0a0a 2020 2020  `` clause...    
-0000b130: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-0000b140: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-0000b150: 6620 606f 6e65 6f66 605f 2060 605f 6964  f `oneof`_ ``_id
-0000b160: 6060 2e0a 2020 2020 2020 2020 6f66 6665  ``..        offe
-0000b170: 725f 6964 2028 7374 7229 3a0a 2020 2020  r_id (str):.    
-0000b180: 2020 2020 2020 2020 4d65 7263 6861 6e74          Merchant
-0000b190: 2d70 726f 7669 6465 6420 6964 206f 6620  -provided id of 
-0000b1a0: 7468 6520 7072 6f64 7563 742e 0a0a 2020  the product...  
-0000b1b0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-0000b1c0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-0000b1d0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-0000b1e0: 6f66 6665 725f 6964 6060 2e0a 2020 2020  offer_id``..    
-0000b1f0: 2020 2020 7469 746c 6520 2873 7472 293a      title (str):
-0000b200: 0a20 2020 2020 2020 2020 2020 2054 6974  .            Tit
-0000b210: 6c65 206f 6620 7468 6520 7072 6f64 7563  le of the produc
-0000b220: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
-0000b230: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-0000b240: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-0000b250: 605f 2060 605f 7469 746c 6560 602e 0a20  `_ ``_title``.. 
-0000b260: 2020 2020 2020 2062 7261 6e64 2028 7374         brand (st
-0000b270: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0000b280: 4272 616e 6420 6f66 2074 6865 2070 726f  Brand of the pro
-0000b290: 6475 6374 2e0a 0a20 2020 2020 2020 2020  duct...         
-0000b2a0: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-0000b2b0: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-0000b2c0: 656f 6660 5f20 6060 5f62 7261 6e64 6060  eof`_ ``_brand``
-0000b2d0: 2e0a 2020 2020 2020 2020 6361 7465 676f  ..        catego
-0000b2e0: 7279 5f6c 3120 2873 7472 293a 0a20 2020  ry_l1 (str):.   
-0000b2f0: 2020 2020 2020 2020 2050 726f 6475 6374           Product
-0000b300: 2063 6174 6567 6f72 7920 2831 7374 206c   category (1st l
-0000b310: 6576 656c 2920 696e 2060 476f 6f67 6c65  evel) in `Google
-0000b320: 2773 2070 726f 6475 6374 0a20 2020 2020  's product.     
-0000b330: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
-0000b340: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
-0000b350: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-0000b360: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
-0000b370: 3434 3336 3e60 5f5f 2e0a 0a20 2020 2020  4436>`__...     
-0000b380: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-0000b390: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-0000b3a0: 2060 6f6e 656f 6660 5f20 6060 5f63 6174   `oneof`_ ``_cat
-0000b3b0: 6567 6f72 795f 6c31 6060 2e0a 2020 2020  egory_l1``..    
-0000b3c0: 2020 2020 6361 7465 676f 7279 5f6c 3220      category_l2 
-0000b3d0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-0000b3e0: 2020 2050 726f 6475 6374 2063 6174 6567     Product categ
-0000b3f0: 6f72 7920 2832 6e64 206c 6576 656c 2920  ory (2nd level) 
-0000b400: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
-0000b410: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
-0000b420: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
-0000b430: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-0000b440: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-0000b450: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
-0000b460: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
-0000b470: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-0000b480: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-0000b490: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
-0000b4a0: 6c32 6060 2e0a 2020 2020 2020 2020 6361  l2``..        ca
-0000b4b0: 7465 676f 7279 5f6c 3320 2873 7472 293a  tegory_l3 (str):
-0000b4c0: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
-0000b4d0: 6475 6374 2063 6174 6567 6f72 7920 2833  duct category (3
-0000b4e0: 7264 206c 6576 656c 2920 696e 2060 476f  rd level) in `Go
-0000b4f0: 6f67 6c65 2773 2070 726f 6475 6374 0a20  ogle's product. 
-0000b500: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
-0000b510: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
-0000b520: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-0000b530: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-0000b540: 2f36 3332 3434 3336 3e60 5f5f 2e0a 0a20  /6324436>`__... 
-0000b550: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-0000b560: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-0000b570: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-0000b580: 5f63 6174 6567 6f72 795f 6c33 6060 2e0a  _category_l3``..
-0000b590: 2020 2020 2020 2020 6361 7465 676f 7279          category
-0000b5a0: 5f6c 3420 2873 7472 293a 0a20 2020 2020  _l4 (str):.     
-0000b5b0: 2020 2020 2020 2050 726f 6475 6374 2063         Product c
-0000b5c0: 6174 6567 6f72 7920 2834 7468 206c 6576  ategory (4th lev
-0000b5d0: 656c 2920 696e 2060 476f 6f67 6c65 2773  el) in `Google's
-0000b5e0: 2070 726f 6475 6374 0a20 2020 2020 2020   product.       
-0000b5f0: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
-0000b600: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
-0000b610: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
-0000b620: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
-0000b630: 3336 3e60 5f5f 2e0a 0a20 2020 2020 2020  36>`__...       
-0000b640: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-0000b650: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-0000b660: 6f6e 656f 6660 5f20 6060 5f63 6174 6567  oneof`_ ``_categ
-0000b670: 6f72 795f 6c34 6060 2e0a 2020 2020 2020  ory_l4``..      
-0000b680: 2020 6361 7465 676f 7279 5f6c 3520 2873    category_l5 (s
-0000b690: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-0000b6a0: 2050 726f 6475 6374 2063 6174 6567 6f72   Product categor
-0000b6b0: 7920 2835 7468 206c 6576 656c 2920 696e  y (5th level) in
-0000b6c0: 2060 476f 6f67 6c65 2773 2070 726f 6475   `Google's produ
-0000b6d0: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
-0000b6e0: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
-0000b6f0: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
-0000b700: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
-0000b710: 7377 6572 2f36 3332 3434 3336 3e60 5f5f  swer/6324436>`__
-0000b720: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-0000b730: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-0000b740: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-0000b750: 5f20 6060 5f63 6174 6567 6f72 795f 6c35  _ ``_category_l5
-0000b760: 6060 2e0a 2020 2020 2020 2020 7072 6f64  ``..        prod
-0000b770: 7563 745f 7479 7065 5f6c 3120 2873 7472  uct_type_l1 (str
-0000b780: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
-0000b790: 726f 6475 6374 2074 7970 6520 2831 7374  roduct type (1st
-0000b7a0: 206c 6576 656c 2920 696e 206d 6572 6368   level) in merch
-0000b7b0: 616e 7427 7320 6f77 6e20 6070 726f 6475  ant's own `produ
-0000b7c0: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
-0000b7d0: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
-0000b7e0: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
-0000b7f0: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
-0000b800: 7377 6572 2f36 3332 3434 3036 3e60 5f5f  swer/6324406>`__
-0000b810: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-0000b820: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-0000b830: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-0000b840: 5f20 6060 5f70 726f 6475 6374 5f74 7970  _ ``_product_typ
-0000b850: 655f 6c31 6060 2e0a 2020 2020 2020 2020  e_l1``..        
-0000b860: 7072 6f64 7563 745f 7479 7065 5f6c 3220  product_type_l2 
-0000b870: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-0000b880: 2020 2050 726f 6475 6374 2074 7970 6520     Product type 
-0000b890: 2832 6e64 206c 6576 656c 2920 696e 206d  (2nd level) in m
-0000b8a0: 6572 6368 616e 7427 7320 6f77 6e20 6070  erchant's own `p
-0000b8b0: 726f 6475 6374 0a20 2020 2020 2020 2020  roduct.         
-0000b8c0: 2020 2074 6178 6f6e 6f6d 7920 3c68 7474     taxonomy <htt
-0000b8d0: 7073 3a2f 2f73 7570 706f 7274 2e67 6f6f  ps://support.goo
-0000b8e0: 676c 652e 636f 6d2f 6d65 7263 6861 6e74  gle.com/merchant
-0000b8f0: 732f 616e 7377 6572 2f36 3332 3434 3036  s/answer/6324406
-0000b900: 3e60 5f5f 2e0a 0a20 2020 2020 2020 2020  >`__...         
-0000b910: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-0000b920: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-0000b930: 656f 6660 5f20 6060 5f70 726f 6475 6374  eof`_ ``_product
-0000b940: 5f74 7970 655f 6c32 6060 2e0a 2020 2020  _type_l2``..    
-0000b950: 2020 2020 7072 6f64 7563 745f 7479 7065      product_type
-0000b960: 5f6c 3320 2873 7472 293a 0a20 2020 2020  _l3 (str):.     
-0000b970: 2020 2020 2020 2050 726f 6475 6374 2074         Product t
-0000b980: 7970 6520 2833 7264 206c 6576 656c 2920  ype (3rd level) 
-0000b990: 696e 206d 6572 6368 616e 7427 7320 6f77  in merchant's ow
-0000b9a0: 6e20 6070 726f 6475 6374 0a20 2020 2020  n `product.     
-0000b9b0: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
-0000b9c0: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
-0000b9d0: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-0000b9e0: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
-0000b9f0: 3434 3036 3e60 5f5f 2e0a 0a20 2020 2020  4406>`__...     
-0000ba00: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
-0000ba10: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
-0000ba20: 2060 6f6e 656f 6660 5f20 6060 5f70 726f   `oneof`_ ``_pro
-0000ba30: 6475 6374 5f74 7970 655f 6c33 6060 2e0a  duct_type_l3``..
-0000ba40: 2020 2020 2020 2020 7072 6f64 7563 745f          product_
-0000ba50: 7479 7065 5f6c 3420 2873 7472 293a 0a20  type_l4 (str):. 
-0000ba60: 2020 2020 2020 2020 2020 2050 726f 6475             Produ
-0000ba70: 6374 2074 7970 6520 2834 7468 206c 6576  ct type (4th lev
-0000ba80: 656c 2920 696e 206d 6572 6368 616e 7427  el) in merchant'
-0000ba90: 7320 6f77 6e20 6070 726f 6475 6374 0a20  s own `product. 
-0000baa0: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
-0000bab0: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
-0000bac0: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-0000bad0: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-0000bae0: 2f36 3332 3434 3036 3e60 5f5f 2e0a 0a20  /6324406>`__... 
-0000baf0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-0000bb00: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-0000bb10: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-0000bb20: 5f70 726f 6475 6374 5f74 7970 655f 6c34  _product_type_l4
-0000bb30: 6060 2e0a 2020 2020 2020 2020 7072 6f64  ``..        prod
-0000bb40: 7563 745f 7479 7065 5f6c 3520 2873 7472  uct_type_l5 (str
-0000bb50: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
-0000bb60: 726f 6475 6374 2074 7970 6520 2835 7468  roduct type (5th
-0000bb70: 206c 6576 656c 2920 696e 206d 6572 6368   level) in merch
-0000bb80: 616e 7427 7320 6f77 6e20 6070 726f 6475  ant's own `produ
-0000bb90: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
-0000bba0: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
-0000bbb0: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
-0000bbc0: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
-0000bbd0: 7377 6572 2f36 3332 3434 3036 3e60 5f5f  swer/6324406>`__
-0000bbe0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-0000bbf0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-0000bc00: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-0000bc10: 5f20 6060 5f70 726f 6475 6374 5f74 7970  _ ``_product_typ
-0000bc20: 655f 6c35 6060 2e0a 2020 2020 2020 2020  e_l5``..        
-0000bc30: 7072 6963 6520 2867 6f6f 676c 652e 7368  price (google.sh
-0000bc40: 6f70 7069 6e67 2e74 7970 652e 7479 7065  opping.type.type
-0000bc50: 732e 5072 6963 6529 3a0a 2020 2020 2020  s.Price):.      
-0000bc60: 2020 2020 2020 4375 7272 656e 7420 7072        Current pr
-0000bc70: 6963 6520 6f66 2074 6865 2070 726f 6475  ice of the produ
-0000bc80: 6374 2e0a 2020 2020 2020 2020 7375 6767  ct..        sugg
-0000bc90: 6573 7465 645f 7072 6963 6520 2867 6f6f  ested_price (goo
-0000bca0: 676c 652e 7368 6f70 7069 6e67 2e74 7970  gle.shopping.typ
-0000bcb0: 652e 7479 7065 732e 5072 6963 6529 3a0a  e.types.Price):.
-0000bcc0: 2020 2020 2020 2020 2020 2020 4c61 7465              Late
-0000bcd0: 7374 2073 7567 6765 7374 6564 2070 7269  st suggested pri
-0000bce0: 6365 2066 6f72 2074 6865 2070 726f 6475  ce for the produ
-0000bcf0: 6374 2e0a 2020 2020 2020 2020 7072 6564  ct..        pred
-0000bd00: 6963 7465 645f 696d 7072 6573 7369 6f6e  icted_impression
-0000bd10: 735f 6368 616e 6765 5f66 7261 6374 696f  s_change_fractio
-0000bd20: 6e20 2866 6c6f 6174 293a 0a20 2020 2020  n (float):.     
-0000bd30: 2020 2020 2020 2050 7265 6469 6374 6564         Predicted
-0000bd40: 2063 6861 6e67 6520 696e 2069 6d70 7265   change in impre
-0000bd50: 7373 696f 6e73 2061 7320 6120 6672 6163  ssions as a frac
-0000bd60: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-0000bd70: 2061 6674 6572 2069 6e74 726f 6475 6369   after introduci
-0000bd80: 6e67 2074 6865 2073 7567 6765 7374 6564  ng the suggested
-0000bd90: 2070 7269 6365 2063 6f6d 7061 7265 640a   price compared.
-0000bda0: 2020 2020 2020 2020 2020 2020 746f 2063              to c
-0000bdb0: 7572 7265 6e74 2061 6374 6976 6520 7072  urrent active pr
-0000bdc0: 6963 652e 2046 6f72 2065 7861 6d70 6c65  ice. For example
-0000bdd0: 2c20 302e 3035 2069 7320 610a 2020 2020  , 0.05 is a.    
-0000bde0: 2020 2020 2020 2020 3525 2070 7265 6469          5% predi
-0000bdf0: 6374 6564 2069 6e63 7265 6173 6520 696e  cted increase in
-0000be00: 2069 6d70 7265 7373 696f 6e73 2e0a 0a20   impressions... 
-0000be10: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-0000be20: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-0000be30: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-0000be40: 5f70 7265 6469 6374 6564 5f69 6d70 7265  _predicted_impre
-0000be50: 7373 696f 6e73 5f63 6861 6e67 655f 6672  ssions_change_fr
-0000be60: 6163 7469 6f6e 6060 2e0a 2020 2020 2020  action``..      
-0000be70: 2020 7072 6564 6963 7465 645f 636c 6963    predicted_clic
-0000be80: 6b73 5f63 6861 6e67 655f 6672 6163 7469  ks_change_fracti
-0000be90: 6f6e 2028 666c 6f61 7429 3a0a 2020 2020  on (float):.    
-0000bea0: 2020 2020 2020 2020 5072 6564 6963 7465          Predicte
-0000beb0: 6420 6368 616e 6765 2069 6e20 636c 6963  d change in clic
-0000bec0: 6b73 2061 7320 6120 6672 6163 7469 6f6e  ks as a fraction
-0000bed0: 0a20 2020 2020 2020 2020 2020 2061 6674  .            aft
-0000bee0: 6572 2069 6e74 726f 6475 6369 6e67 2074  er introducing t
-0000bef0: 6865 2073 7567 6765 7374 6564 2070 7269  he suggested pri
-0000bf00: 6365 2063 6f6d 7061 7265 640a 2020 2020  ce compared.    
-0000bf10: 2020 2020 2020 2020 746f 2063 7572 7265          to curre
-0000bf20: 6e74 2061 6374 6976 6520 7072 6963 652e  nt active price.
-0000bf30: 2046 6f72 2065 7861 6d70 6c65 2c20 302e   For example, 0.
-0000bf40: 3035 2069 7320 610a 2020 2020 2020 2020  05 is a.        
-0000bf50: 2020 2020 3525 2070 7265 6469 6374 6564      5% predicted
-0000bf60: 2069 6e63 7265 6173 6520 696e 2063 6c69   increase in cli
-0000bf70: 636b 732e 0a0a 2020 2020 2020 2020 2020  cks...          
-0000bf80: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-0000bf90: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-0000bfa0: 6f66 605f 2060 605f 7072 6564 6963 7465  of`_ ``_predicte
-0000bfb0: 645f 636c 6963 6b73 5f63 6861 6e67 655f  d_clicks_change_
-0000bfc0: 6672 6163 7469 6f6e 6060 2e0a 2020 2020  fraction``..    
-0000bfd0: 2020 2020 7072 6564 6963 7465 645f 636f      predicted_co
-0000bfe0: 6e76 6572 7369 6f6e 735f 6368 616e 6765  nversions_change
-0000bff0: 5f66 7261 6374 696f 6e20 2866 6c6f 6174  _fraction (float
-0000c000: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
-0000c010: 7265 6469 6374 6564 2063 6861 6e67 6520  redicted change 
-0000c020: 696e 2063 6f6e 7665 7273 696f 6e73 2061  in conversions a
-0000c030: 7320 6120 6672 6163 7469 6f6e 0a20 2020  s a fraction.   
-0000c040: 2020 2020 2020 2020 2061 6674 6572 2069           after i
-0000c050: 6e74 726f 6475 6369 6e67 2074 6865 2073  ntroducing the s
-0000c060: 7567 6765 7374 6564 2070 7269 6365 2063  uggested price c
-0000c070: 6f6d 7061 7265 640a 2020 2020 2020 2020  ompared.        
-0000c080: 2020 2020 746f 2063 7572 7265 6e74 2061      to current a
-0000c090: 6374 6976 6520 7072 6963 652e 2046 6f72  ctive price. For
-0000c0a0: 2065 7861 6d70 6c65 2c20 302e 3035 2069   example, 0.05 i
-0000c0b0: 7320 610a 2020 2020 2020 2020 2020 2020  s a.            
-0000c0c0: 3525 2070 7265 6469 6374 6564 2069 6e63  5% predicted inc
-0000c0d0: 7265 6173 6520 696e 2063 6f6e 7665 7273  rease in convers
-0000c0e0: 696f 6e73 292e 0a0a 2020 2020 2020 2020  ions)...        
-0000c0f0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-0000c100: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-0000c110: 6e65 6f66 605f 2060 605f 7072 6564 6963  neof`_ ``_predic
-0000c120: 7465 645f 636f 6e76 6572 7369 6f6e 735f  ted_conversions_
-0000c130: 6368 616e 6765 5f66 7261 6374 696f 6e60  change_fraction`
-0000c140: 602e 0a20 2020 2022 2222 0a0a 2020 2020  `..    """..    
-0000c150: 6964 3a20 7374 7220 3d20 7072 6f74 6f2e  id: str = proto.
-0000c160: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-0000c170: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-0000c180: 2020 2020 206e 756d 6265 723d 312c 0a20       number=1,. 
-0000c190: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-0000c1a0: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
-0000c1b0: 6f66 6665 725f 6964 3a20 7374 7220 3d20  offer_id: str = 
-0000c1c0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000c1d0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-0000c1e0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-0000c1f0: 723d 322c 0a20 2020 2020 2020 206f 7074  r=2,.        opt
-0000c200: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-0000c210: 290a 2020 2020 7469 746c 653a 2073 7472  ).    title: str
-0000c220: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-0000c230: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
-0000c240: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
-0000c250: 6d62 6572 3d33 2c0a 2020 2020 2020 2020  mber=3,.        
-0000c260: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
-0000c270: 2020 2029 0a20 2020 2062 7261 6e64 3a20     ).    brand: 
-0000c280: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
-0000c290: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-0000c2a0: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
-0000c2b0: 206e 756d 6265 723d 342c 0a20 2020 2020   number=4,.     
-0000c2c0: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-0000c2d0: 2c0a 2020 2020 290a 2020 2020 6361 7465  ,.    ).    cate
-0000c2e0: 676f 7279 5f6c 313a 2073 7472 203d 2070  gory_l1: str = p
-0000c2f0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-0000c300: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
-0000c310: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-0000c320: 3d35 2c0a 2020 2020 2020 2020 6f70 7469  =5,.        opti
-0000c330: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-0000c340: 0a20 2020 2063 6174 6567 6f72 795f 6c32  .    category_l2
-0000c350: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-0000c360: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-0000c370: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-0000c380: 2020 206e 756d 6265 723d 362c 0a20 2020     number=6,.   
-0000c390: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-0000c3a0: 7565 2c0a 2020 2020 290a 2020 2020 6361  ue,.    ).    ca
-0000c3b0: 7465 676f 7279 5f6c 333a 2073 7472 203d  tegory_l3: str =
-0000c3c0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-0000c3d0: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
-0000c3e0: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
-0000c3f0: 6572 3d37 2c0a 2020 2020 2020 2020 6f70  er=7,.        op
-0000c400: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-0000c410: 2029 0a20 2020 2063 6174 6567 6f72 795f   ).    category_
-0000c420: 6c34 3a20 7374 7220 3d20 7072 6f74 6f2e  l4: str = proto.
-0000c430: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-0000c440: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-0000c450: 2020 2020 206e 756d 6265 723d 382c 0a20       number=8,. 
-0000c460: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-0000c470: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
-0000c480: 6361 7465 676f 7279 5f6c 353a 2073 7472  category_l5: str
-0000c490: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-0000c4a0: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
-0000c4b0: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
-0000c4c0: 6d62 6572 3d39 2c0a 2020 2020 2020 2020  mber=9,.        
-0000c4d0: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
-0000c4e0: 2020 2029 0a20 2020 2070 726f 6475 6374     ).    product
-0000c4f0: 5f74 7970 655f 6c31 3a20 7374 7220 3d20  _type_l1: str = 
-0000c500: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000c510: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-0000c520: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-0000c530: 723d 3130 2c0a 2020 2020 2020 2020 6f70  r=10,.        op
-0000c540: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-0000c550: 2029 0a20 2020 2070 726f 6475 6374 5f74   ).    product_t
-0000c560: 7970 655f 6c32 3a20 7374 7220 3d20 7072  ype_l2: str = pr
-0000c570: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-0000c580: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
-0000c590: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-0000c5a0: 3131 2c0a 2020 2020 2020 2020 6f70 7469  11,.        opti
-0000c5b0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-0000c5c0: 0a20 2020 2070 726f 6475 6374 5f74 7970  .    product_typ
-0000c5d0: 655f 6c33 3a20 7374 7220 3d20 7072 6f74  e_l3: str = prot
-0000c5e0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-0000c5f0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-0000c600: 2020 2020 2020 206e 756d 6265 723d 3132         number=12
-0000c610: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-0000c620: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-0000c630: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
-0000c640: 6c34 3a20 7374 7220 3d20 7072 6f74 6f2e  l4: str = proto.
-0000c650: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-0000c660: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
-0000c670: 2020 2020 206e 756d 6265 723d 3133 2c0a       number=13,.
-0000c680: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-0000c690: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-0000c6a0: 2070 726f 6475 6374 5f74 7970 655f 6c35   product_type_l5
-0000c6b0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-0000c6c0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-0000c6d0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-0000c6e0: 2020 206e 756d 6265 723d 3134 2c0a 2020     number=14,.  
-0000c6f0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-0000c700: 7275 652c 0a20 2020 2029 0a20 2020 2070  rue,.    ).    p
-0000c710: 7269 6365 3a20 7479 7065 732e 5072 6963  rice: types.Pric
-0000c720: 6520 3d20 7072 6f74 6f2e 4669 656c 6428  e = proto.Field(
-0000c730: 0a20 2020 2020 2020 2070 726f 746f 2e4d  .        proto.M
-0000c740: 4553 5341 4745 2c0a 2020 2020 2020 2020  ESSAGE,.        
-0000c750: 6e75 6d62 6572 3d31 352c 0a20 2020 2020  number=15,.     
-0000c760: 2020 206d 6573 7361 6765 3d74 7970 6573     message=types
-0000c770: 2e50 7269 6365 2c0a 2020 2020 290a 2020  .Price,.    ).  
-0000c780: 2020 7375 6767 6573 7465 645f 7072 6963    suggested_pric
-0000c790: 653a 2074 7970 6573 2e50 7269 6365 203d  e: types.Price =
-0000c7a0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-0000c7b0: 2020 2020 2020 7072 6f74 6f2e 4d45 5353        proto.MESS
-0000c7c0: 4147 452c 0a20 2020 2020 2020 206e 756d  AGE,.        num
-0000c7d0: 6265 723d 3136 2c0a 2020 2020 2020 2020  ber=16,.        
-0000c7e0: 6d65 7373 6167 653d 7479 7065 732e 5072  message=types.Pr
-0000c7f0: 6963 652c 0a20 2020 2029 0a20 2020 2070  ice,.    ).    p
-0000c800: 7265 6469 6374 6564 5f69 6d70 7265 7373  redicted_impress
-0000c810: 696f 6e73 5f63 6861 6e67 655f 6672 6163  ions_change_frac
-0000c820: 7469 6f6e 3a20 666c 6f61 7420 3d20 7072  tion: float = pr
-0000c830: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
-0000c840: 2020 2070 726f 746f 2e44 4f55 424c 452c     proto.DOUBLE,
-0000c850: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-0000c860: 3137 2c0a 2020 2020 2020 2020 6f70 7469  17,.        opti
-0000c870: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-0000c880: 0a20 2020 2070 7265 6469 6374 6564 5f63  .    predicted_c
-0000c890: 6c69 636b 735f 6368 616e 6765 5f66 7261  licks_change_fra
-0000c8a0: 6374 696f 6e3a 2066 6c6f 6174 203d 2070  ction: float = p
-0000c8b0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-0000c8c0: 2020 2020 7072 6f74 6f2e 444f 5542 4c45      proto.DOUBLE
-0000c8d0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-0000c8e0: 3d31 382c 0a20 2020 2020 2020 206f 7074  =18,.        opt
-0000c8f0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-0000c900: 290a 2020 2020 7072 6564 6963 7465 645f  ).    predicted_
-0000c910: 636f 6e76 6572 7369 6f6e 735f 6368 616e  conversions_chan
-0000c920: 6765 5f66 7261 6374 696f 6e3a 2066 6c6f  ge_fraction: flo
-0000c930: 6174 203d 2070 726f 746f 2e46 6965 6c64  at = proto.Field
-0000c940: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-0000c950: 444f 5542 4c45 2c0a 2020 2020 2020 2020  DOUBLE,.        
-0000c960: 6e75 6d62 6572 3d31 392c 0a20 2020 2020  number=19,.     
-0000c970: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-0000c980: 2c0a 2020 2020 290a 0a0a 636c 6173 7320  ,.    )...class 
-0000c990: 4265 7374 5365 6c6c 6572 7350 726f 6475  BestSellersProdu
-0000c9a0: 6374 436c 7573 7465 7256 6965 7728 7072  ctClusterView(pr
-0000c9b0: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
-0000c9c0: 2020 7222 2222 4669 656c 6473 2061 7661    r"""Fields ava
-0000c9d0: 696c 6162 6c65 2066 6f72 2071 7565 7279  ilable for query
-0000c9e0: 2069 6e20 6060 6265 7374 5f73 656c 6c65   in ``best_selle
-0000c9f0: 7273 5f70 726f 6475 6374 5f63 6c75 7374  rs_product_clust
-0000ca00: 6572 5f76 6965 7760 600a 2020 2020 7461  er_view``.    ta
-0000ca10: 626c 652e 0a0a 2020 2020 6042 6573 740a  ble...    `Best.
-0000ca20: 2020 2020 7365 6c6c 6572 7320 3c68 7474      sellers <htt
-0000ca30: 7073 3a2f 2f73 7570 706f 7274 2e67 6f6f  ps://support.goo
-0000ca40: 676c 652e 636f 6d2f 6d65 7263 6861 6e74  gle.com/merchant
-0000ca50: 732f 616e 7377 6572 2f39 3438 3836 3739  s/answer/9488679
-0000ca60: 3e60 5f5f 0a20 2020 2072 6570 6f72 7420  >`__.    report 
-0000ca70: 7769 7468 2074 6f70 2070 726f 6475 6374  with top product
-0000ca80: 2063 6c75 7374 6572 732e 2041 2070 726f   clusters. A pro
-0000ca90: 6475 6374 2063 6c75 7374 6572 2069 7320  duct cluster is 
-0000caa0: 6120 6772 6f75 7069 6e67 0a20 2020 2066  a grouping.    f
-0000cab0: 6f72 2064 6966 6665 7265 6e74 206f 6666  or different off
-0000cac0: 6572 7320 616e 6420 7661 7269 616e 7473  ers and variants
-0000cad0: 2074 6861 7420 7265 7072 6573 656e 7420   that represent 
-0000cae0: 7468 6520 7361 6d65 2070 726f 6475 6374  the same product
-0000caf0: 2c0a 2020 2020 666f 7220 6578 616d 706c  ,.    for exampl
-0000cb00: 652c 2047 6f6f 676c 6520 5069 7865 6c20  e, Google Pixel 
-0000cb10: 372e 0a0a 2020 2020 5661 6c75 6573 2061  7...    Values a
-0000cb20: 7265 206f 6e6c 7920 7365 7420 666f 7220  re only set for 
-0000cb30: 6669 656c 6473 2072 6571 7565 7374 6564  fields requested
-0000cb40: 2065 7870 6c69 6369 746c 7920 696e 2074   explicitly in t
-0000cb50: 6865 2072 6571 7565 7374 2773 0a20 2020  he request's.   
-0000cb60: 2073 6561 7263 6820 7175 6572 792e 0a0a   search query...
-0000cb70: 0a20 2020 202e 2e20 5f6f 6e65 6f66 3a20  .    .. _oneof: 
-0000cb80: 6874 7470 733a 2f2f 7072 6f74 6f2d 706c  https://proto-pl
-0000cb90: 7573 2d70 7974 686f 6e2e 7265 6164 7468  us-python.readth
-0000cba0: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
-0000cbb0: 6c65 2f66 6965 6c64 732e 6874 6d6c 236f  le/fields.html#o
-0000cbc0: 6e65 6f66 732d 6d75 7475 616c 6c79 2d65  neofs-mutually-e
-0000cbd0: 7863 6c75 7369 7665 2d66 6965 6c64 730a  xclusive-fields.
-0000cbe0: 0a20 2020 2041 7474 7269 6275 7465 733a  .    Attributes:
-0000cbf0: 0a20 2020 2020 2020 2072 6570 6f72 745f  .        report_
-0000cc00: 6461 7465 2028 676f 6f67 6c65 2e74 7970  date (google.typ
-0000cc10: 652e 6461 7465 5f70 6232 2e44 6174 6529  e.date_pb2.Date)
-0000cc20: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
-0000cc30: 706f 7274 2064 6174 652e 2054 6865 2076  port date. The v
-0000cc40: 616c 7565 206f 6620 7468 6973 2066 6965  alue of this fie
-0000cc50: 6c64 2063 616e 206f 6e6c 7920 6265 206f  ld can only be o
-0000cc60: 6e65 206f 6620 7468 650a 2020 2020 2020  ne of the.      
-0000cc70: 2020 2020 2020 666f 6c6c 6f77 696e 673a        following:
-0000cc80: 0a0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
-0000cc90: 2054 6865 2066 6972 7374 2064 6179 206f   The first day o
-0000cca0: 6620 7468 6520 7765 656b 2028 4d6f 6e64  f the week (Mond
-0000ccb0: 6179 2920 666f 7220 7765 656b 6c79 2072  ay) for weekly r
-0000ccc0: 6570 6f72 7473 2c0a 2020 2020 2020 2020  eports,.        
-0000ccd0: 2020 2020 2d20 2054 6865 2066 6972 7374      -  The first
-0000cce0: 2064 6179 206f 6620 7468 6520 6d6f 6e74   day of the mont
-0000ccf0: 6820 666f 7220 6d6f 6e74 686c 7920 7265  h for monthly re
-0000cd00: 706f 7274 732e 0a0a 2020 2020 2020 2020  ports...        
-0000cd10: 2020 2020 5265 7175 6972 6564 2069 6e20      Required in 
-0000cd20: 7468 6520 6060 5345 4c45 4354 6060 2063  the ``SELECT`` c
-0000cd30: 6c61 7573 652e 2049 6620 6120 6060 5748  lause. If a ``WH
-0000cd40: 4552 4560 6020 636f 6e64 6974 696f 6e0a  ERE`` condition.
-0000cd50: 2020 2020 2020 2020 2020 2020 6f6e 2060              on `
-0000cd60: 6072 6570 6f72 745f 6461 7465 6060 2069  `report_date`` i
-0000cd70: 7320 6e6f 7420 7370 6563 6966 6965 6420  s not specified 
-0000cd80: 696e 2074 6865 2071 7565 7279 2c20 7468  in the query, th
-0000cd90: 6520 6c61 7465 7374 0a20 2020 2020 2020  e latest.       
-0000cda0: 2020 2020 2061 7661 696c 6162 6c65 2077       available w
-0000cdb0: 6565 6b6c 7920 6f72 206d 6f6e 7468 6c79  eekly or monthly
-0000cdc0: 2072 6570 6f72 7420 6973 2072 6574 7572   report is retur
-0000cdd0: 6e65 642e 0a20 2020 2020 2020 2072 6570  ned..        rep
-0000cde0: 6f72 745f 6772 616e 756c 6172 6974 7920  ort_granularity 
-0000cdf0: 2867 6f6f 676c 652e 7368 6f70 7069 6e67  (google.shopping
-0000ce00: 2e6d 6572 6368 616e 745f 7265 706f 7274  .merchant_report
-0000ce10: 735f 7631 6265 7461 2e74 7970 6573 2e52  s_v1beta.types.R
-0000ce20: 6570 6f72 7447 7261 6e75 6c61 7269 7479  eportGranularity
-0000ce30: 2e52 6570 6f72 7447 7261 6e75 6c61 7269  .ReportGranulari
-0000ce40: 7479 456e 756d 293a 0a20 2020 2020 2020  tyEnum):.       
-0000ce50: 2020 2020 2047 7261 6e75 6c61 7269 7479       Granularity
-0000ce60: 206f 6620 7468 6520 7265 706f 7274 2e20   of the report. 
-0000ce70: 5468 6520 7261 6e6b 696e 6720 6361 6e20  The ranking can 
-0000ce80: 6265 2064 6f6e 6520 6f76 6572 2061 0a20  be done over a. 
-0000ce90: 2020 2020 2020 2020 2020 2077 6565 6b20             week 
-0000cea0: 6f72 2061 206d 6f6e 7468 2074 696d 6566  or a month timef
-0000ceb0: 7261 6d65 2e0a 0a20 2020 2020 2020 2020  rame...         
-0000cec0: 2020 2052 6571 7569 7265 6420 696e 2074     Required in t
-0000ced0: 6865 2060 6053 454c 4543 5460 6020 636c  he ``SELECT`` cl
-0000cee0: 6175 7365 2e20 436f 6e64 6974 696f 6e20  ause. Condition 
-0000cef0: 6f6e 0a20 2020 2020 2020 2020 2020 2060  on.            `
-0000cf00: 6072 6570 6f72 745f 6772 616e 756c 6172  `report_granular
-0000cf10: 6974 7960 6020 6973 2072 6571 7569 7265  ity`` is require
-0000cf20: 6420 696e 2074 6865 2060 6057 4845 5245  d in the ``WHERE
-0000cf30: 6060 2063 6c61 7573 652e 0a0a 2020 2020  `` clause...    
-0000cf40: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-0000cf50: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-0000cf60: 6620 606f 6e65 6f66 605f 2060 605f 7265  f `oneof`_ ``_re
-0000cf70: 706f 7274 5f67 7261 6e75 6c61 7269 7479  port_granularity
-0000cf80: 6060 2e0a 2020 2020 2020 2020 7265 706f  ``..        repo
-0000cf90: 7274 5f63 6f75 6e74 7279 5f63 6f64 6520  rt_country_code 
-0000cfa0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-0000cfb0: 2020 2043 6f75 6e74 7279 2077 6865 7265     Country where
-0000cfc0: 2074 6865 2072 616e 6b69 6e67 2069 7320   the ranking is 
-0000cfd0: 6361 6c63 756c 6174 6564 2e20 5265 7072  calculated. Repr
-0000cfe0: 6573 656e 7465 6420 696e 2074 6865 0a20  esented in the. 
-0000cff0: 2020 2020 2020 2020 2020 2049 534f 2033             ISO 3
-0000d000: 3136 3620 666f 726d 6174 2e0a 0a20 2020  166 format...   
-0000d010: 2020 2020 2020 2020 2052 6571 7569 7265           Require
-0000d020: 6420 696e 2074 6865 2060 6053 454c 4543  d in the ``SELEC
-0000d030: 5460 6020 636c 6175 7365 2e20 436f 6e64  T`` clause. Cond
-0000d040: 6974 696f 6e20 6f6e 0a20 2020 2020 2020  ition on.       
-0000d050: 2020 2020 2060 6072 6570 6f72 745f 636f       ``report_co
-0000d060: 756e 7472 795f 636f 6465 6060 2069 7320  untry_code`` is 
-0000d070: 7265 7175 6972 6564 2069 6e20 7468 6520  required in the 
-0000d080: 6060 5748 4552 4560 6020 636c 6175 7365  ``WHERE`` clause
-0000d090: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-0000d0a0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-0000d0b0: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-0000d0c0: 5f20 6060 5f72 6570 6f72 745f 636f 756e  _ ``_report_coun
-0000d0d0: 7472 795f 636f 6465 6060 2e0a 2020 2020  try_code``..    
-0000d0e0: 2020 2020 7265 706f 7274 5f63 6174 6567      report_categ
-0000d0f0: 6f72 795f 6964 2028 696e 7429 3a0a 2020  ory_id (int):.  
-0000d100: 2020 2020 2020 2020 2020 476f 6f67 6c65            Google
-0000d110: 2070 726f 6475 6374 2063 6174 6567 6f72   product categor
-0000d120: 7920 4944 2074 6f20 6361 6c63 756c 6174  y ID to calculat
-0000d130: 6520 7468 6520 7261 6e6b 696e 6720 666f  e the ranking fo
-0000d140: 722c 0a20 2020 2020 2020 2020 2020 2072  r,.            r
-0000d150: 6570 7265 7365 6e74 6564 2069 6e20 6047  epresented in `G
-0000d160: 6f6f 676c 6527 7320 7072 6f64 7563 740a  oogle's product.
-0000d170: 2020 2020 2020 2020 2020 2020 7461 786f              taxo
-0000d180: 6e6f 6d79 203c 6874 7470 733a 2f2f 7375  nomy <https://su
-0000d190: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
-0000d1a0: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
-0000d1b0: 722f 3633 3234 3433 363e 605f 5f2e 0a0a  r/6324436>`__...
-0000d1c0: 2020 2020 2020 2020 2020 2020 5265 7175              Requ
-0000d1d0: 6972 6564 2069 6e20 7468 6520 6060 5345  ired in the ``SE
-0000d1e0: 4c45 4354 6060 2063 6c61 7573 652e 2049  LECT`` clause. I
-0000d1f0: 6620 6120 6060 5748 4552 4560 6020 636f  f a ``WHERE`` co
-0000d200: 6e64 6974 696f 6e0a 2020 2020 2020 2020  ndition.        
-0000d210: 2020 2020 6f6e 2060 6072 6570 6f72 745f      on ``report_
-0000d220: 6361 7465 676f 7279 5f69 6460 6020 6973  category_id`` is
-0000d230: 206e 6f74 2073 7065 6369 6669 6564 2069   not specified i
-0000d240: 6e20 7468 6520 7175 6572 792c 0a20 2020  n the query,.   
-0000d250: 2020 2020 2020 2020 2072 616e 6b69 6e67           ranking
-0000d260: 7320 666f 7220 616c 6c20 746f 702d 6c65  s for all top-le
-0000d270: 7665 6c20 6361 7465 676f 7269 6573 2061  vel categories a
-0000d280: 7265 2072 6574 7572 6e65 642e 0a0a 2020  re returned...  
-0000d290: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-0000d2a0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-0000d2b0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-0000d2c0: 7265 706f 7274 5f63 6174 6567 6f72 795f  report_category_
-0000d2d0: 6964 6060 2e0a 2020 2020 2020 2020 7469  id``..        ti
-0000d2e0: 746c 6520 2873 7472 293a 0a20 2020 2020  tle (str):.     
-0000d2f0: 2020 2020 2020 2054 6974 6c65 206f 6620         Title of 
-0000d300: 7468 6520 7072 6f64 7563 7420 636c 7573  the product clus
-0000d310: 7465 722e 0a0a 2020 2020 2020 2020 2020  ter...          
-0000d320: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-0000d330: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-0000d340: 6f66 605f 2060 605f 7469 746c 6560 602e  of`_ ``_title``.
-0000d350: 0a20 2020 2020 2020 2062 7261 6e64 2028  .        brand (
-0000d360: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-0000d370: 2020 4272 616e 6420 6f66 2074 6865 2070    Brand of the p
-0000d380: 726f 6475 6374 2063 6c75 7374 6572 2e0a  roduct cluster..
-0000d390: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-0000d3a0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-0000d3b0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-0000d3c0: 6060 5f62 7261 6e64 6060 2e0a 2020 2020  ``_brand``..    
-0000d3d0: 2020 2020 6361 7465 676f 7279 5f6c 3120      category_l1 
-0000d3e0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
-0000d3f0: 2020 2050 726f 6475 6374 2063 6174 6567     Product categ
-0000d400: 6f72 7920 2831 7374 206c 6576 656c 2920  ory (1st level) 
-0000d410: 6f66 2074 6865 2070 726f 6475 6374 2063  of the product c
-0000d420: 6c75 7374 6572 2c0a 2020 2020 2020 2020  luster,.        
-0000d430: 2020 2020 7265 7072 6573 656e 7465 6420      represented 
-0000d440: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
-0000d450: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
-0000d460: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
-0000d470: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-0000d480: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-0000d490: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
-0000d4a0: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
-0000d4b0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
-0000d4c0: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
-0000d4d0: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
-0000d4e0: 6c31 6060 2e0a 2020 2020 2020 2020 6361  l1``..        ca
-0000d4f0: 7465 676f 7279 5f6c 3220 2873 7472 293a  tegory_l2 (str):
-0000d500: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
-0000d510: 6475 6374 2063 6174 6567 6f72 7920 2832  duct category (2
-0000d520: 6e64 206c 6576 656c 2920 6f66 2074 6865  nd level) of the
-0000d530: 2070 726f 6475 6374 2063 6c75 7374 6572   product cluster
-0000d540: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
-0000d550: 7072 6573 656e 7465 6420 696e 2060 476f  presented in `Go
-0000d560: 6f67 6c65 2773 2070 726f 6475 6374 0a20  ogle's product. 
-0000d570: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
-0000d580: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
-0000d590: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-0000d5a0: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-0000d5b0: 2f36 3332 3434 3336 3e60 5f5f 2e0a 0a20  /6324436>`__... 
-0000d5c0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-0000d5d0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-0000d5e0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-0000d5f0: 5f63 6174 6567 6f72 795f 6c32 6060 2e0a  _category_l2``..
-0000d600: 2020 2020 2020 2020 6361 7465 676f 7279          category
-0000d610: 5f6c 3320 2873 7472 293a 0a20 2020 2020  _l3 (str):.     
-0000d620: 2020 2020 2020 2050 726f 6475 6374 2063         Product c
-0000d630: 6174 6567 6f72 7920 2833 7264 206c 6576  ategory (3rd lev
-0000d640: 656c 2920 6f66 2074 6865 2070 726f 6475  el) of the produ
-0000d650: 6374 2063 6c75 7374 6572 2c0a 2020 2020  ct cluster,.    
-0000d660: 2020 2020 2020 2020 7265 7072 6573 656e          represen
-0000d670: 7465 6420 696e 2060 476f 6f67 6c65 2773  ted in `Google's
-0000d680: 2070 726f 6475 6374 0a20 2020 2020 2020   product.       
-0000d690: 2020 2020 2074 6178 6f6e 6f6d 7920 3c68       taxonomy <h
-0000d6a0: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
-0000d6b0: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
-0000d6c0: 6e74 732f 616e 7377 6572 2f36 3332 3434  nts/answer/63244
-0000d6d0: 3336 3e60 5f5f 2e0a 0a20 2020 2020 2020  36>`__...       
-0000d6e0: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-0000d6f0: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-0000d700: 6f6e 656f 6660 5f20 6060 5f63 6174 6567  oneof`_ ``_categ
-0000d710: 6f72 795f 6c33 6060 2e0a 2020 2020 2020  ory_l3``..      
-0000d720: 2020 6361 7465 676f 7279 5f6c 3420 2873    category_l4 (s
-0000d730: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-0000d740: 2050 726f 6475 6374 2063 6174 6567 6f72   Product categor
-0000d750: 7920 2834 7468 206c 6576 656c 2920 6f66  y (4th level) of
-0000d760: 2074 6865 2070 726f 6475 6374 2063 6c75   the product clu
-0000d770: 7374 6572 2c0a 2020 2020 2020 2020 2020  ster,.          
-0000d780: 2020 7265 7072 6573 656e 7465 6420 696e    represented in
-0000d790: 2060 476f 6f67 6c65 2773 2070 726f 6475   `Google's produ
-0000d7a0: 6374 0a20 2020 2020 2020 2020 2020 2074  ct.            t
-0000d7b0: 6178 6f6e 6f6d 7920 3c68 7474 7073 3a2f  axonomy <https:/
-0000d7c0: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
-0000d7d0: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
-0000d7e0: 7377 6572 2f36 3332 3434 3336 3e60 5f5f  swer/6324436>`__
-0000d7f0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-0000d800: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-0000d810: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-0000d820: 5f20 6060 5f63 6174 6567 6f72 795f 6c34  _ ``_category_l4
-0000d830: 6060 2e0a 2020 2020 2020 2020 6361 7465  ``..        cate
-0000d840: 676f 7279 5f6c 3520 2873 7472 293a 0a20  gory_l5 (str):. 
-0000d850: 2020 2020 2020 2020 2020 2050 726f 6475             Produ
-0000d860: 6374 2063 6174 6567 6f72 7920 2835 7468  ct category (5th
-0000d870: 206c 6576 656c 2920 6f66 2074 6865 2070   level) of the p
-0000d880: 726f 6475 6374 2063 6c75 7374 6572 2c0a  roduct cluster,.
-0000d890: 2020 2020 2020 2020 2020 2020 7265 7072              repr
-0000d8a0: 6573 656e 7465 6420 696e 2060 476f 6f67  esented in `Goog
-0000d8b0: 6c65 2773 2070 726f 6475 6374 0a20 2020  le's product.   
-0000d8c0: 2020 2020 2020 2020 2074 6178 6f6e 6f6d           taxonom
-0000d8d0: 7920 3c68 7474 7073 3a2f 2f73 7570 706f  y <https://suppo
-0000d8e0: 7274 2e67 6f6f 676c 652e 636f 6d2f 6d65  rt.google.com/me
-0000d8f0: 7263 6861 6e74 732f 616e 7377 6572 2f36  rchants/answer/6
-0000d900: 3332 3434 3336 3e60 5f5f 2e0a 0a20 2020  324436>`__...   
-0000d910: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-0000d920: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-0000d930: 6f66 2060 6f6e 656f 6660 5f20 6060 5f63  of `oneof`_ ``_c
-0000d940: 6174 6567 6f72 795f 6c35 6060 2e0a 2020  ategory_l5``..  
-0000d950: 2020 2020 2020 7661 7269 616e 745f 6774        variant_gt
-0000d960: 696e 7320 284d 7574 6162 6c65 5365 7175  ins (MutableSequ
-0000d970: 656e 6365 5b73 7472 5d29 3a0a 2020 2020  ence[str]):.    
-0000d980: 2020 2020 2020 2020 4754 494e 7320 6f66          GTINs of
-0000d990: 2065 7861 6d70 6c65 2076 6172 6961 6e74   example variant
-0000d9a0: 7320 6f66 2074 6865 2070 726f 6475 6374  s of the product
-0000d9b0: 0a20 2020 2020 2020 2020 2020 2063 6c75  .            clu
-0000d9c0: 7374 6572 2e0a 2020 2020 2020 2020 696e  ster..        in
-0000d9d0: 7665 6e74 6f72 795f 7374 6174 7573 2028  ventory_status (
-0000d9e0: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
-0000d9f0: 6d65 7263 6861 6e74 5f72 6570 6f72 7473  merchant_reports
-0000da00: 5f76 3162 6574 612e 7479 7065 732e 4265  _v1beta.types.Be
-0000da10: 7374 5365 6c6c 6572 7350 726f 6475 6374  stSellersProduct
-0000da20: 436c 7573 7465 7256 6965 772e 496e 7665  ClusterView.Inve
-0000da30: 6e74 6f72 7953 7461 7475 7329 3a0a 2020  ntoryStatus):.  
-0000da40: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
-0000da50: 7220 7468 6520 7072 6f64 7563 7420 636c  r the product cl
-0000da60: 7573 7465 7220 6973 2060 6049 4e5f 5354  uster is ``IN_ST
-0000da70: 4f43 4b60 6020 696e 2079 6f75 7220 7072  OCK`` in your pr
-0000da80: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
-0000da90: 2020 6665 6564 2069 6e20 6174 206c 6561    feed in at lea
-0000daa0: 7374 206f 6e65 206f 6620 7468 6520 636f  st one of the co
-0000dab0: 756e 7472 6965 732c 2060 604f 5554 5f4f  untries, ``OUT_O
-0000dac0: 465f 5354 4f43 4b60 6020 696e 0a20 2020  F_STOCK`` in.   
-0000dad0: 2020 2020 2020 2020 2079 6f75 7220 7072           your pr
-0000dae0: 6f64 7563 7420 6665 6564 2069 6e20 616c  oduct feed in al
-0000daf0: 6c20 636f 756e 7472 6965 732c 206f 7220  l countries, or 
-0000db00: 6060 4e4f 545f 494e 5f49 4e56 454e 544f  ``NOT_IN_INVENTO
-0000db10: 5259 6060 0a20 2020 2020 2020 2020 2020  RY``.           
-0000db20: 2061 7420 616c 6c2e 0a0a 2020 2020 2020   at all...      
-0000db30: 2020 2020 2020 5468 6520 6669 656c 6420        The field 
-0000db40: 646f 6573 6e27 7420 7461 6b65 2074 6865  doesn't take the
-0000db50: 2042 6573 7420 7365 6c6c 6572 7320 7265   Best sellers re
-0000db60: 706f 7274 2063 6f75 6e74 7279 0a20 2020  port country.   
-0000db70: 2020 2020 2020 2020 2066 696c 7465 7220           filter 
-0000db80: 696e 746f 2061 6363 6f75 6e74 2e0a 0a20  into account... 
-0000db90: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-0000dba0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-0000dbb0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-0000dbc0: 5f69 6e76 656e 746f 7279 5f73 7461 7475  _inventory_statu
-0000dbd0: 7360 602e 0a20 2020 2020 2020 2062 7261  s``..        bra
-0000dbe0: 6e64 5f69 6e76 656e 746f 7279 5f73 7461  nd_inventory_sta
-0000dbf0: 7475 7320 2867 6f6f 676c 652e 7368 6f70  tus (google.shop
-0000dc00: 7069 6e67 2e6d 6572 6368 616e 745f 7265  ping.merchant_re
-0000dc10: 706f 7274 735f 7631 6265 7461 2e74 7970  ports_v1beta.typ
-0000dc20: 6573 2e42 6573 7453 656c 6c65 7273 5072  es.BestSellersPr
-0000dc30: 6f64 7563 7443 6c75 7374 6572 5669 6577  oductClusterView
-0000dc40: 2e49 6e76 656e 746f 7279 5374 6174 7573  .InventoryStatus
-0000dc50: 293a 0a20 2020 2020 2020 2020 2020 2057  ):.            W
-0000dc60: 6865 7468 6572 2074 6865 7265 2069 7320  hether there is 
-0000dc70: 6174 206c 6561 7374 206f 6e65 2070 726f  at least one pro
-0000dc80: 6475 6374 206f 6620 7468 6520 6272 616e  duct of the bran
-0000dc90: 6420 6375 7272 656e 746c 790a 2020 2020  d currently.    
-0000dca0: 2020 2020 2020 2020 6060 494e 5f53 544f          ``IN_STO
-0000dcb0: 434b 6060 2069 6e20 796f 7572 2070 726f  CK`` in your pro
-0000dcc0: 6475 6374 2066 6565 6420 696e 2061 7420  duct feed in at 
-0000dcd0: 6c65 6173 7420 6f6e 6520 6f66 2074 6865  least one of the
-0000dce0: 0a20 2020 2020 2020 2020 2020 2063 6f75  .            cou
-0000dcf0: 6e74 7269 6573 2c20 616c 6c20 7072 6f64  ntries, all prod
-0000dd00: 7563 7473 2061 7265 2060 604f 5554 5f4f  ucts are ``OUT_O
-0000dd10: 465f 5354 4f43 4b60 6020 696e 2079 6f75  F_STOCK`` in you
-0000dd20: 7220 7072 6f64 7563 740a 2020 2020 2020  r product.      
-0000dd30: 2020 2020 2020 6665 6564 2069 6e20 616c        feed in al
-0000dd40: 6c20 636f 756e 7472 6965 732c 206f 7220  l countries, or 
-0000dd50: 6060 4e4f 545f 494e 5f49 4e56 454e 544f  ``NOT_IN_INVENTO
-0000dd60: 5259 6060 2e0a 0a20 2020 2020 2020 2020  RY``...         
-0000dd70: 2020 2054 6865 2066 6965 6c64 2064 6f65     The field doe
-0000dd80: 736e 2774 2074 616b 6520 7468 6520 4265  sn't take the Be
-0000dd90: 7374 2073 656c 6c65 7273 2072 6570 6f72  st sellers repor
-0000dda0: 7420 636f 756e 7472 790a 2020 2020 2020  t country.      
-0000ddb0: 2020 2020 2020 6669 6c74 6572 2069 6e74        filter int
-0000ddc0: 6f20 6163 636f 756e 742e 0a0a 2020 2020  o account...    
-0000ddd0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-0000dde0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-0000ddf0: 6620 606f 6e65 6f66 605f 2060 605f 6272  f `oneof`_ ``_br
-0000de00: 616e 645f 696e 7665 6e74 6f72 795f 7374  and_inventory_st
-0000de10: 6174 7573 6060 2e0a 2020 2020 2020 2020  atus``..        
-0000de20: 7261 6e6b 2028 696e 7429 3a0a 2020 2020  rank (int):.    
-0000de30: 2020 2020 2020 2020 506f 7075 6c61 7269          Populari
-0000de40: 7479 206f 6620 7468 6520 7072 6f64 7563  ty of the produc
-0000de50: 7420 636c 7573 7465 7220 6f6e 2041 6473  t cluster on Ads
-0000de60: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-0000de70: 206f 7267 616e 6963 2073 7572 6661 6365   organic surface
-0000de80: 732c 2069 6e20 7468 6520 7365 6c65 6374  s, in the select
-0000de90: 6564 2063 6174 6567 6f72 7920 616e 640a  ed category and.
-0000dea0: 2020 2020 2020 2020 2020 2020 636f 756e              coun
-0000deb0: 7472 792c 2062 6173 6564 206f 6e20 7468  try, based on th
-0000dec0: 6520 6573 7469 6d61 7465 6420 6e75 6d62  e estimated numb
-0000ded0: 6572 206f 6620 756e 6974 730a 2020 2020  er of units.    
-0000dee0: 2020 2020 2020 2020 736f 6c64 2e0a 0a20          sold... 
-0000def0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-0000df00: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
-0000df10: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
-0000df20: 5f72 616e 6b60 602e 0a20 2020 2020 2020  _rank``..       
-0000df30: 2070 7265 7669 6f75 735f 7261 6e6b 2028   previous_rank (
-0000df40: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-0000df50: 2020 506f 7075 6c61 7269 7479 2072 616e    Popularity ran
-0000df60: 6b20 696e 2074 6865 2070 7265 7669 6f75  k in the previou
-0000df70: 7320 7765 656b 206f 720a 2020 2020 2020  s week or.      
-0000df80: 2020 2020 2020 6d6f 6e74 682e 0a0a 2020        month...  
-0000df90: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-0000dfa0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-0000dfb0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-0000dfc0: 7072 6576 696f 7573 5f72 616e 6b60 602e  previous_rank``.
-0000dfd0: 0a20 2020 2020 2020 2072 656c 6174 6976  .        relativ
-0000dfe0: 655f 6465 6d61 6e64 2028 676f 6f67 6c65  e_demand (google
-0000dff0: 2e73 686f 7070 696e 672e 6d65 7263 6861  .shopping.mercha
-0000e000: 6e74 5f72 6570 6f72 7473 5f76 3162 6574  nt_reports_v1bet
-0000e010: 612e 7479 7065 732e 5265 6c61 7469 7665  a.types.Relative
-0000e020: 4465 6d61 6e64 2e52 656c 6174 6976 6544  Demand.RelativeD
-0000e030: 656d 616e 6445 6e75 6d29 3a0a 2020 2020  emandEnum):.    
-0000e040: 2020 2020 2020 2020 4573 7469 6d61 7465          Estimate
-0000e050: 6420 6465 6d61 6e64 2069 6e20 7265 6c61  d demand in rela
-0000e060: 7469 6f6e 2074 6f20 7468 6520 7072 6f64  tion to the prod
-0000e070: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
-0000e080: 636c 7573 7465 7220 7769 7468 2074 6865  cluster with the
-0000e090: 2068 6967 6865 7374 2070 6f70 756c 6172   highest popular
-0000e0a0: 6974 7920 7261 6e6b 2069 6e20 7468 650a  ity rank in the.
-0000e0b0: 2020 2020 2020 2020 2020 2020 7361 6d65              same
-0000e0c0: 2063 6174 6567 6f72 7920 616e 6420 636f   category and co
-0000e0d0: 756e 7472 792e 0a0a 2020 2020 2020 2020  untry...        
-0000e0e0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-0000e0f0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-0000e100: 6e65 6f66 605f 2060 605f 7265 6c61 7469  neof`_ ``_relati
-0000e110: 7665 5f64 656d 616e 6460 602e 0a20 2020  ve_demand``..   
-0000e120: 2020 2020 2070 7265 7669 6f75 735f 7265       previous_re
-0000e130: 6c61 7469 7665 5f64 656d 616e 6420 2867  lative_demand (g
-0000e140: 6f6f 676c 652e 7368 6f70 7069 6e67 2e6d  oogle.shopping.m
-0000e150: 6572 6368 616e 745f 7265 706f 7274 735f  erchant_reports_
-0000e160: 7631 6265 7461 2e74 7970 6573 2e52 656c  v1beta.types.Rel
-0000e170: 6174 6976 6544 656d 616e 642e 5265 6c61  ativeDemand.Rela
-0000e180: 7469 7665 4465 6d61 6e64 456e 756d 293a  tiveDemandEnum):
-0000e190: 0a20 2020 2020 2020 2020 2020 2045 7374  .            Est
-0000e1a0: 696d 6174 6564 2064 656d 616e 6420 696e  imated demand in
-0000e1b0: 2072 656c 6174 696f 6e20 746f 2074 6865   relation to the
-0000e1c0: 2070 726f 6475 6374 0a20 2020 2020 2020   product.       
-0000e1d0: 2020 2020 2063 6c75 7374 6572 2077 6974       cluster wit
-0000e1e0: 6820 7468 6520 6869 6768 6573 7420 706f  h the highest po
-0000e1f0: 7075 6c61 7269 7479 2072 616e 6b20 696e  pularity rank in
-0000e200: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-0000e210: 2073 616d 6520 6361 7465 676f 7279 2061   same category a
-0000e220: 6e64 2063 6f75 6e74 7279 2069 6e20 7468  nd country in th
-0000e230: 6520 7072 6576 696f 7573 2077 6565 6b0a  e previous week.
-0000e240: 2020 2020 2020 2020 2020 2020 6f72 206d              or m
-0000e250: 6f6e 7468 2e0a 0a20 2020 2020 2020 2020  onth...         
-0000e260: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
-0000e270: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
-0000e280: 656f 6660 5f20 6060 5f70 7265 7669 6f75  eof`_ ``_previou
-0000e290: 735f 7265 6c61 7469 7665 5f64 656d 616e  s_relative_deman
-0000e2a0: 6460 602e 0a20 2020 2020 2020 2072 656c  d``..        rel
-0000e2b0: 6174 6976 655f 6465 6d61 6e64 5f63 6861  ative_demand_cha
-0000e2c0: 6e67 6520 2867 6f6f 676c 652e 7368 6f70  nge (google.shop
-0000e2d0: 7069 6e67 2e6d 6572 6368 616e 745f 7265  ping.merchant_re
-0000e2e0: 706f 7274 735f 7631 6265 7461 2e74 7970  ports_v1beta.typ
-0000e2f0: 6573 2e52 656c 6174 6976 6544 656d 616e  es.RelativeDeman
-0000e300: 6443 6861 6e67 6554 7970 652e 5265 6c61  dChangeType.Rela
-0000e310: 7469 7665 4465 6d61 6e64 4368 616e 6765  tiveDemandChange
-0000e320: 5479 7065 456e 756d 293a 0a20 2020 2020  TypeEnum):.     
-0000e330: 2020 2020 2020 2043 6861 6e67 6520 696e         Change in
-0000e340: 2074 6865 2065 7374 696d 6174 6564 2064   the estimated d
-0000e350: 656d 616e 642e 2057 6865 7468 6572 2069  emand. Whether i
-0000e360: 740a 2020 2020 2020 2020 2020 2020 726f  t.            ro
-0000e370: 7365 2c20 7361 6e6b 206f 7220 7265 6d61  se, sank or rema
-0000e380: 696e 6564 2066 6c61 742e 0a0a 2020 2020  ined flat...    
-0000e390: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-0000e3a0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-0000e3b0: 6620 606f 6e65 6f66 605f 2060 605f 7265  f `oneof`_ ``_re
-0000e3c0: 6c61 7469 7665 5f64 656d 616e 645f 6368  lative_demand_ch
-0000e3d0: 616e 6765 6060 2e0a 2020 2020 2222 220a  ange``..    """.
-0000e3e0: 0a20 2020 2063 6c61 7373 2049 6e76 656e  .    class Inven
-0000e3f0: 746f 7279 5374 6174 7573 2870 726f 746f  toryStatus(proto
-0000e400: 2e45 6e75 6d29 3a0a 2020 2020 2020 2020  .Enum):.        
-0000e410: 7222 2222 5374 6174 7573 206f 6620 7468  r"""Status of th
-0000e420: 6520 7072 6f64 7563 7420 636c 7573 7465  e product cluste
-0000e430: 7220 6f72 2062 7261 6e64 2069 6e20 796f  r or brand in yo
-0000e440: 7572 2069 6e76 656e 746f 7279 2e0a 0a20  ur inventory... 
-0000e450: 2020 2020 2020 2056 616c 7565 733a 0a20         Values:. 
-0000e460: 2020 2020 2020 2020 2020 2049 4e56 454e             INVEN
-0000e470: 544f 5259 5f53 5441 5455 535f 554e 5350  TORY_STATUS_UNSP
-0000e480: 4543 4946 4945 4420 2830 293a 0a20 2020  ECIFIED (0):.   
-0000e490: 2020 2020 2020 2020 2020 2020 204e 6f74               Not
-0000e4a0: 2073 7065 6369 6669 6564 2e0a 2020 2020   specified..    
-0000e4b0: 2020 2020 2020 2020 494e 5f53 544f 434b          IN_STOCK
-0000e4c0: 2028 3129 3a0a 2020 2020 2020 2020 2020   (1):.          
-0000e4d0: 2020 2020 2020 596f 7520 6861 7665 2061        You have a
-0000e4e0: 2070 726f 6475 6374 2066 6f72 2074 6869   product for thi
-0000e4f0: 7320 7072 6f64 7563 7420 636c 7573 7465  s product cluste
-0000e500: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-0000e510: 2020 6f72 2062 7261 6e64 2069 6e20 7374    or brand in st
-0000e520: 6f63 6b2e 0a20 2020 2020 2020 2020 2020  ock..           
-0000e530: 204f 5554 5f4f 465f 5354 4f43 4b20 2832   OUT_OF_STOCK (2
-0000e540: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000e550: 2020 2059 6f75 2068 6176 6520 6120 7072     You have a pr
-0000e560: 6f64 7563 7420 666f 7220 7468 6973 2070  oduct for this p
-0000e570: 726f 6475 6374 2063 6c75 7374 6572 0a20  roduct cluster. 
-0000e580: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000e590: 7220 6272 616e 6420 696e 2069 6e76 656e  r brand in inven
-0000e5a0: 746f 7279 2062 7574 2069 7420 6973 2063  tory but it is c
-0000e5b0: 7572 7265 6e74 6c79 206f 7574 206f 660a  urrently out of.
-0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5d0: 7374 6f63 6b2e 0a20 2020 2020 2020 2020  stock..         
-0000e5e0: 2020 204e 4f54 5f49 4e5f 494e 5645 4e54     NOT_IN_INVENT
-0000e5f0: 4f52 5920 2833 293a 0a20 2020 2020 2020  ORY (3):.       
-0000e600: 2020 2020 2020 2020 2059 6f75 2064 6f20           You do 
-0000e610: 6e6f 7420 6861 7665 2061 2070 726f 6475  not have a produ
-0000e620: 6374 2066 6f72 2074 6869 7320 7072 6f64  ct for this prod
-0000e630: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
-0000e640: 2020 2020 636c 7573 7465 7220 6f72 2062      cluster or b
-0000e650: 7261 6e64 2069 6e20 696e 7665 6e74 6f72  rand in inventor
-0000e660: 792e 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
-0000e670: 2020 2020 2020 2049 4e56 454e 544f 5259         INVENTORY
-0000e680: 5f53 5441 5455 535f 554e 5350 4543 4946  _STATUS_UNSPECIF
-0000e690: 4945 4420 3d20 300a 2020 2020 2020 2020  IED = 0.        
-0000e6a0: 494e 5f53 544f 434b 203d 2031 0a20 2020  IN_STOCK = 1.   
-0000e6b0: 2020 2020 204f 5554 5f4f 465f 5354 4f43       OUT_OF_STOC
-0000e6c0: 4b20 3d20 320a 2020 2020 2020 2020 4e4f  K = 2.        NO
-0000e6d0: 545f 494e 5f49 4e56 454e 544f 5259 203d  T_IN_INVENTORY =
-0000e6e0: 2033 0a0a 2020 2020 7265 706f 7274 5f64   3..    report_d
-0000e6f0: 6174 653a 2064 6174 655f 7062 322e 4461  ate: date_pb2.Da
-0000e700: 7465 203d 2070 726f 746f 2e46 6965 6c64  te = proto.Field
-0000e710: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-0000e720: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
-0000e730: 206e 756d 6265 723d 312c 0a20 2020 2020   number=1,.     
-0000e740: 2020 206d 6573 7361 6765 3d64 6174 655f     message=date_
-0000e750: 7062 322e 4461 7465 2c0a 2020 2020 290a  pb2.Date,.    ).
-0000e760: 2020 2020 7265 706f 7274 5f67 7261 6e75      report_granu
-0000e770: 6c61 7269 7479 3a20 2252 6570 6f72 7447  larity: "ReportG
-0000e780: 7261 6e75 6c61 7269 7479 2e52 6570 6f72  ranularity.Repor
-0000e790: 7447 7261 6e75 6c61 7269 7479 456e 756d  tGranularityEnum
-0000e7a0: 2220 3d20 7072 6f74 6f2e 4669 656c 6428  " = proto.Field(
-0000e7b0: 0a20 2020 2020 2020 2070 726f 746f 2e45  .        proto.E
-0000e7c0: 4e55 4d2c 0a20 2020 2020 2020 206e 756d  NUM,.        num
-0000e7d0: 6265 723d 322c 0a20 2020 2020 2020 206f  ber=2,.        o
-0000e7e0: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-0000e7f0: 2020 2020 2020 656e 756d 3d22 5265 706f        enum="Repo
-0000e800: 7274 4772 616e 756c 6172 6974 792e 5265  rtGranularity.Re
-0000e810: 706f 7274 4772 616e 756c 6172 6974 7945  portGranularityE
-0000e820: 6e75 6d22 2c0a 2020 2020 290a 2020 2020  num",.    ).    
-0000e830: 7265 706f 7274 5f63 6f75 6e74 7279 5f63  report_country_c
-0000e840: 6f64 653a 2073 7472 203d 2070 726f 746f  ode: str = proto
-0000e850: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000e860: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-0000e870: 2020 2020 2020 6e75 6d62 6572 3d33 2c0a        number=3,.
-0000e880: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-0000e890: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-0000e8a0: 2072 6570 6f72 745f 6361 7465 676f 7279   report_category
-0000e8b0: 5f69 643a 2069 6e74 203d 2070 726f 746f  _id: int = proto
-0000e8c0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000e8d0: 7072 6f74 6f2e 494e 5436 342c 0a20 2020  proto.INT64,.   
-0000e8e0: 2020 2020 206e 756d 6265 723d 342c 0a20       number=4,. 
-0000e8f0: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-0000e900: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
-0000e910: 7469 746c 653a 2073 7472 203d 2070 726f  title: str = pro
-0000e920: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-0000e930: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
-0000e940: 2020 2020 2020 2020 6e75 6d62 6572 3d36          number=6
-0000e950: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
-0000e960: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
-0000e970: 2020 2062 7261 6e64 3a20 7374 7220 3d20     brand: str = 
-0000e980: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-0000e990: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-0000e9a0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-0000e9b0: 723d 372c 0a20 2020 2020 2020 206f 7074  r=7,.        opt
-0000e9c0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-0000e9d0: 290a 2020 2020 6361 7465 676f 7279 5f6c  ).    category_l
-0000e9e0: 313a 2073 7472 203d 2070 726f 746f 2e46  1: str = proto.F
-0000e9f0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-0000ea00: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
-0000ea10: 2020 2020 6e75 6d62 6572 3d38 2c0a 2020      number=8,.  
-0000ea20: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-0000ea30: 7275 652c 0a20 2020 2029 0a20 2020 2063  rue,.    ).    c
-0000ea40: 6174 6567 6f72 795f 6c32 3a20 7374 7220  ategory_l2: str 
-0000ea50: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-0000ea60: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-0000ea70: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-0000ea80: 6265 723d 392c 0a20 2020 2020 2020 206f  ber=9,.        o
-0000ea90: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-0000eaa0: 2020 290a 2020 2020 6361 7465 676f 7279    ).    category
-0000eab0: 5f6c 333a 2073 7472 203d 2070 726f 746f  _l3: str = proto
-0000eac0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-0000ead0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
-0000eae0: 2020 2020 2020 6e75 6d62 6572 3d31 302c        number=10,
-0000eaf0: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-0000eb00: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-0000eb10: 2020 6361 7465 676f 7279 5f6c 343a 2073    category_l4: s
-0000eb20: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
-0000eb30: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-0000eb40: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
-0000eb50: 6e75 6d62 6572 3d31 312c 0a20 2020 2020  number=11,.     
-0000eb60: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-0000eb70: 2c0a 2020 2020 290a 2020 2020 6361 7465  ,.    ).    cate
-0000eb80: 676f 7279 5f6c 353a 2073 7472 203d 2070  gory_l5: str = p
-0000eb90: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-0000eba0: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
-0000ebb0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-0000ebc0: 3d31 322c 0a20 2020 2020 2020 206f 7074  =12,.        opt
-0000ebd0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-0000ebe0: 290a 2020 2020 7661 7269 616e 745f 6774  ).    variant_gt
-0000ebf0: 696e 733a 204d 7574 6162 6c65 5365 7175  ins: MutableSequ
-0000ec00: 656e 6365 5b73 7472 5d20 3d20 7072 6f74  ence[str] = prot
-0000ec10: 6f2e 5265 7065 6174 6564 4669 656c 6428  o.RepeatedField(
-0000ec20: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-0000ec30: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-0000ec40: 756d 6265 723d 3133 2c0a 2020 2020 290a  umber=13,.    ).
-0000ec50: 2020 2020 696e 7665 6e74 6f72 795f 7374      inventory_st
-0000ec60: 6174 7573 3a20 496e 7665 6e74 6f72 7953  atus: InventoryS
-0000ec70: 7461 7475 7320 3d20 7072 6f74 6f2e 4669  tatus = proto.Fi
-0000ec80: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-0000ec90: 746f 2e45 4e55 4d2c 0a20 2020 2020 2020  to.ENUM,.       
-0000eca0: 206e 756d 6265 723d 3134 2c0a 2020 2020   number=14,.    
-0000ecb0: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-0000ecc0: 652c 0a20 2020 2020 2020 2065 6e75 6d3d  e,.        enum=
-0000ecd0: 496e 7665 6e74 6f72 7953 7461 7475 732c  InventoryStatus,
-0000ece0: 0a20 2020 2029 0a20 2020 2062 7261 6e64  .    ).    brand
-0000ecf0: 5f69 6e76 656e 746f 7279 5f73 7461 7475  _inventory_statu
-0000ed00: 733a 2049 6e76 656e 746f 7279 5374 6174  s: InventoryStat
-0000ed10: 7573 203d 2070 726f 746f 2e46 6965 6c64  us = proto.Field
-0000ed20: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-0000ed30: 454e 554d 2c0a 2020 2020 2020 2020 6e75  ENUM,.        nu
-0000ed40: 6d62 6572 3d31 352c 0a20 2020 2020 2020  mber=15,.       
-0000ed50: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-0000ed60: 2020 2020 2020 2020 656e 756d 3d49 6e76          enum=Inv
-0000ed70: 656e 746f 7279 5374 6174 7573 2c0a 2020  entoryStatus,.  
-0000ed80: 2020 290a 2020 2020 7261 6e6b 3a20 696e    ).    rank: in
-0000ed90: 7420 3d20 7072 6f74 6f2e 4669 656c 6428  t = proto.Field(
-0000eda0: 0a20 2020 2020 2020 2070 726f 746f 2e49  .        proto.I
-0000edb0: 4e54 3634 2c0a 2020 2020 2020 2020 6e75  NT64,.        nu
-0000edc0: 6d62 6572 3d31 362c 0a20 2020 2020 2020  mber=16,.       
-0000edd0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-0000ede0: 2020 2020 290a 2020 2020 7072 6576 696f      ).    previo
-0000edf0: 7573 5f72 616e 6b3a 2069 6e74 203d 2070  us_rank: int = p
-0000ee00: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-0000ee10: 2020 2020 7072 6f74 6f2e 494e 5436 342c      proto.INT64,
-0000ee20: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
-0000ee30: 3137 2c0a 2020 2020 2020 2020 6f70 7469  17,.        opti
-0000ee40: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-0000ee50: 0a20 2020 2072 656c 6174 6976 655f 6465  .    relative_de
-0000ee60: 6d61 6e64 3a20 2252 656c 6174 6976 6544  mand: "RelativeD
-0000ee70: 656d 616e 642e 5265 6c61 7469 7665 4465  emand.RelativeDe
-0000ee80: 6d61 6e64 456e 756d 2220 3d20 7072 6f74  mandEnum" = prot
-0000ee90: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-0000eea0: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
-0000eeb0: 2020 2020 206e 756d 6265 723d 3138 2c0a       number=18,.
-0000eec0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-0000eed0: 3d54 7275 652c 0a20 2020 2020 2020 2065  =True,.        e
-0000eee0: 6e75 6d3d 2252 656c 6174 6976 6544 656d  num="RelativeDem
-0000eef0: 616e 642e 5265 6c61 7469 7665 4465 6d61  and.RelativeDema
-0000ef00: 6e64 456e 756d 222c 0a20 2020 2029 0a20  ndEnum",.    ). 
-0000ef10: 2020 2070 7265 7669 6f75 735f 7265 6c61     previous_rela
-0000ef20: 7469 7665 5f64 656d 616e 643a 2022 5265  tive_demand: "Re
-0000ef30: 6c61 7469 7665 4465 6d61 6e64 2e52 656c  lativeDemand.Rel
-0000ef40: 6174 6976 6544 656d 616e 6445 6e75 6d22  ativeDemandEnum"
-0000ef50: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-0000ef60: 2020 2020 2020 2020 7072 6f74 6f2e 454e          proto.EN
-0000ef70: 554d 2c0a 2020 2020 2020 2020 6e75 6d62  UM,.        numb
-0000ef80: 6572 3d31 392c 0a20 2020 2020 2020 206f  er=19,.        o
-0000ef90: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-0000efa0: 2020 2020 2020 656e 756d 3d22 5265 6c61        enum="Rela
-0000efb0: 7469 7665 4465 6d61 6e64 2e52 656c 6174  tiveDemand.Relat
-0000efc0: 6976 6544 656d 616e 6445 6e75 6d22 2c0a  iveDemandEnum",.
-0000efd0: 2020 2020 290a 2020 2020 7265 6c61 7469      ).    relati
-0000efe0: 7665 5f64 656d 616e 645f 6368 616e 6765  ve_demand_change
-0000eff0: 3a20 2252 656c 6174 6976 6544 656d 616e  : "RelativeDeman
-0000f000: 6443 6861 6e67 6554 7970 652e 5265 6c61  dChangeType.Rela
-0000f010: 7469 7665 4465 6d61 6e64 4368 616e 6765  tiveDemandChange
-0000f020: 5479 7065 456e 756d 2220 3d20 280a 2020  TypeEnum" = (.  
-0000f030: 2020 2020 2020 7072 6f74 6f2e 4669 656c        proto.Fiel
-0000f040: 6428 0a20 2020 2020 2020 2020 2020 2070  d(.            p
-0000f050: 726f 746f 2e45 4e55 4d2c 0a20 2020 2020  roto.ENUM,.     
-0000f060: 2020 2020 2020 206e 756d 6265 723d 3230         number=20
-0000f070: 2c0a 2020 2020 2020 2020 2020 2020 6f70  ,.            op
-0000f080: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-0000f090: 2020 2020 2020 2020 2065 6e75 6d3d 2252           enum="R
-0000f0a0: 656c 6174 6976 6544 656d 616e 6443 6861  elativeDemandCha
-0000f0b0: 6e67 6554 7970 652e 5265 6c61 7469 7665  ngeType.Relative
-0000f0c0: 4465 6d61 6e64 4368 616e 6765 5479 7065  DemandChangeType
-0000f0d0: 456e 756d 222c 0a20 2020 2020 2020 2029  Enum",.        )
-0000f0e0: 0a20 2020 2029 0a0a 0a63 6c61 7373 2042  .    )...class B
-0000f0f0: 6573 7453 656c 6c65 7273 4272 616e 6456  estSellersBrandV
-0000f100: 6965 7728 7072 6f74 6f2e 4d65 7373 6167  iew(proto.Messag
-0000f110: 6529 3a0a 2020 2020 7222 2222 4669 656c  e):.    r"""Fiel
-0000f120: 6473 2061 7661 696c 6162 6c65 2066 6f72  ds available for
-0000f130: 2071 7565 7279 2069 6e20 6060 6265 7374   query in ``best
-0000f140: 5f73 656c 6c65 7273 5f62 7261 6e64 5f76  _sellers_brand_v
-0000f150: 6965 7760 6020 7461 626c 652e 0a0a 2020  iew`` table...  
-0000f160: 2020 6042 6573 740a 2020 2020 7365 6c6c    `Best.    sell
-0000f170: 6572 7320 3c68 7474 7073 3a2f 2f73 7570  ers <https://sup
-0000f180: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-0000f190: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-0000f1a0: 2f39 3438 3836 3739 3e60 5f5f 0a20 2020  /9488679>`__.   
-0000f1b0: 2072 6570 6f72 7420 7769 7468 2074 6f70   report with top
-0000f1c0: 2062 7261 6e64 732e 0a0a 2020 2020 5661   brands...    Va
-0000f1d0: 6c75 6573 2061 7265 206f 6e6c 7920 7365  lues are only se
-0000f1e0: 7420 666f 7220 6669 656c 6473 2072 6571  t for fields req
-0000f1f0: 7565 7374 6564 2065 7870 6c69 6369 746c  uested explicitl
-0000f200: 7920 696e 2074 6865 2072 6571 7565 7374  y in the request
-0000f210: 2773 0a20 2020 2073 6561 7263 6820 7175  's.    search qu
-0000f220: 6572 792e 0a0a 0a20 2020 202e 2e20 5f6f  ery....    .. _o
-0000f230: 6e65 6f66 3a20 6874 7470 733a 2f2f 7072  neof: https://pr
-0000f240: 6f74 6f2d 706c 7573 2d70 7974 686f 6e2e  oto-plus-python.
-0000f250: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-0000f260: 6e2f 7374 6162 6c65 2f66 6965 6c64 732e  n/stable/fields.
-0000f270: 6874 6d6c 236f 6e65 6f66 732d 6d75 7475  html#oneofs-mutu
-0000f280: 616c 6c79 2d65 7863 6c75 7369 7665 2d66  ally-exclusive-f
-0000f290: 6965 6c64 730a 0a20 2020 2041 7474 7269  ields..    Attri
-0000f2a0: 6275 7465 733a 0a20 2020 2020 2020 2072  butes:.        r
-0000f2b0: 6570 6f72 745f 6461 7465 2028 676f 6f67  eport_date (goog
-0000f2c0: 6c65 2e74 7970 652e 6461 7465 5f70 6232  le.type.date_pb2
-0000f2d0: 2e44 6174 6529 3a0a 2020 2020 2020 2020  .Date):.        
-0000f2e0: 2020 2020 5265 706f 7274 2064 6174 652e      Report date.
-0000f2f0: 2054 6865 2076 616c 7565 206f 6620 7468   The value of th
-0000f300: 6973 2066 6965 6c64 2063 616e 206f 6e6c  is field can onl
-0000f310: 7920 6265 206f 6e65 206f 6620 7468 650a  y be one of the.
-0000f320: 2020 2020 2020 2020 2020 2020 666f 6c6c              foll
-0000f330: 6f77 696e 673a 0a0a 2020 2020 2020 2020  owing:..        
-0000f340: 2020 2020 2d20 2054 6865 2066 6972 7374      -  The first
-0000f350: 2064 6179 206f 6620 7468 6520 7765 656b   day of the week
-0000f360: 2028 4d6f 6e64 6179 2920 666f 7220 7765   (Monday) for we
-0000f370: 656b 6c79 2072 6570 6f72 7473 2c0a 2020  ekly reports,.  
-0000f380: 2020 2020 2020 2020 2020 2d20 2054 6865            -  The
-0000f390: 2066 6972 7374 2064 6179 206f 6620 7468   first day of th
-0000f3a0: 6520 6d6f 6e74 6820 666f 7220 6d6f 6e74  e month for mont
-0000f3b0: 686c 7920 7265 706f 7274 732e 0a0a 2020  hly reports...  
-0000f3c0: 2020 2020 2020 2020 2020 5265 7175 6972            Requir
-0000f3d0: 6564 2069 6e20 7468 6520 6060 5345 4c45  ed in the ``SELE
-0000f3e0: 4354 6060 2063 6c61 7573 652e 2049 6620  CT`` clause. If 
-0000f3f0: 6120 6060 5748 4552 4560 6020 636f 6e64  a ``WHERE`` cond
-0000f400: 6974 696f 6e0a 2020 2020 2020 2020 2020  ition.          
-0000f410: 2020 6f6e 2060 6072 6570 6f72 745f 6461    on ``report_da
-0000f420: 7465 6060 2069 7320 6e6f 7420 7370 6563  te`` is not spec
-0000f430: 6966 6965 6420 696e 2074 6865 2071 7565  ified in the que
-0000f440: 7279 2c20 7468 6520 6c61 7465 7374 0a20  ry, the latest. 
-0000f450: 2020 2020 2020 2020 2020 2061 7661 696c             avail
-0000f460: 6162 6c65 2077 6565 6b6c 7920 6f72 206d  able weekly or m
-0000f470: 6f6e 7468 6c79 2072 6570 6f72 7420 6973  onthly report is
-0000f480: 2072 6574 7572 6e65 642e 0a20 2020 2020   returned..     
-0000f490: 2020 2072 6570 6f72 745f 6772 616e 756c     report_granul
-0000f4a0: 6172 6974 7920 2867 6f6f 676c 652e 7368  arity (google.sh
-0000f4b0: 6f70 7069 6e67 2e6d 6572 6368 616e 745f  opping.merchant_
-0000f4c0: 7265 706f 7274 735f 7631 6265 7461 2e74  reports_v1beta.t
-0000f4d0: 7970 6573 2e52 6570 6f72 7447 7261 6e75  ypes.ReportGranu
-0000f4e0: 6c61 7269 7479 2e52 6570 6f72 7447 7261  larity.ReportGra
-0000f4f0: 6e75 6c61 7269 7479 456e 756d 293a 0a20  nularityEnum):. 
-0000f500: 2020 2020 2020 2020 2020 2047 7261 6e75             Granu
-0000f510: 6c61 7269 7479 206f 6620 7468 6520 7265  larity of the re
-0000f520: 706f 7274 2e20 5468 6520 7261 6e6b 696e  port. The rankin
-0000f530: 6720 6361 6e20 6265 2064 6f6e 6520 6f76  g can be done ov
-0000f540: 6572 2061 0a20 2020 2020 2020 2020 2020  er a.           
-0000f550: 2077 6565 6b20 6f72 2061 206d 6f6e 7468   week or a month
-0000f560: 2074 696d 6566 7261 6d65 2e0a 0a20 2020   timeframe...   
-0000f570: 2020 2020 2020 2020 2052 6571 7569 7265           Require
-0000f580: 6420 696e 2074 6865 2060 6053 454c 4543  d in the ``SELEC
-0000f590: 5460 6020 636c 6175 7365 2e20 436f 6e64  T`` clause. Cond
-0000f5a0: 6974 696f 6e20 6f6e 0a20 2020 2020 2020  ition on.       
-0000f5b0: 2020 2020 2060 6072 6570 6f72 745f 6772       ``report_gr
-0000f5c0: 616e 756c 6172 6974 7960 6020 6973 2072  anularity`` is r
-0000f5d0: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
-0000f5e0: 6057 4845 5245 6060 2063 6c61 7573 652e  `WHERE`` clause.
-0000f5f0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-0000f600: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-0000f610: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-0000f620: 2060 605f 7265 706f 7274 5f67 7261 6e75   ``_report_granu
-0000f630: 6c61 7269 7479 6060 2e0a 2020 2020 2020  larity``..      
-0000f640: 2020 7265 706f 7274 5f63 6f75 6e74 7279    report_country
-0000f650: 5f63 6f64 6520 2873 7472 293a 0a20 2020  _code (str):.   
-0000f660: 2020 2020 2020 2020 2043 6f75 6e74 7279           Country
-0000f670: 2077 6865 7265 2074 6865 2072 616e 6b69   where the ranki
-0000f680: 6e67 2069 7320 6361 6c63 756c 6174 6564  ng is calculated
-0000f690: 2e20 5265 7072 6573 656e 7465 6420 696e  . Represented in
-0000f6a0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-0000f6b0: 2049 534f 2033 3136 3620 666f 726d 6174   ISO 3166 format
-0000f6c0: 2e0a 0a20 2020 2020 2020 2020 2020 2052  ...            R
-0000f6d0: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
-0000f6e0: 6053 454c 4543 5460 6020 636c 6175 7365  `SELECT`` clause
-0000f6f0: 2e20 436f 6e64 6974 696f 6e20 6f6e 0a20  . Condition on. 
-0000f700: 2020 2020 2020 2020 2020 2060 6072 6570             ``rep
-0000f710: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
-0000f720: 6060 2069 7320 7265 7175 6972 6564 2069  `` is required i
-0000f730: 6e20 7468 6520 6060 5748 4552 4560 6020  n the ``WHERE`` 
-0000f740: 636c 6175 7365 2e0a 0a20 2020 2020 2020  clause...       
-0000f750: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-0000f760: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-0000f770: 6f6e 656f 6660 5f20 6060 5f72 6570 6f72  oneof`_ ``_repor
-0000f780: 745f 636f 756e 7472 795f 636f 6465 6060  t_country_code``
-0000f790: 2e0a 2020 2020 2020 2020 7265 706f 7274  ..        report
-0000f7a0: 5f63 6174 6567 6f72 795f 6964 2028 696e  _category_id (in
-0000f7b0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0000f7c0: 476f 6f67 6c65 2070 726f 6475 6374 2063  Google product c
-0000f7d0: 6174 6567 6f72 7920 4944 2074 6f20 6361  ategory ID to ca
-0000f7e0: 6c63 756c 6174 6520 7468 6520 7261 6e6b  lculate the rank
-0000f7f0: 696e 6720 666f 722c 0a20 2020 2020 2020  ing for,.       
-0000f800: 2020 2020 2072 6570 7265 7365 6e74 6564       represented
-0000f810: 2069 6e20 6047 6f6f 676c 6527 7320 7072   in `Google's pr
-0000f820: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
-0000f830: 2020 7461 786f 6e6f 6d79 203c 6874 7470    taxonomy <http
-0000f840: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
-0000f850: 6c65 2e63 6f6d 2f6d 6572 6368 616e 7473  le.com/merchants
-0000f860: 2f61 6e73 7765 722f 3633 3234 3433 363e  /answer/6324436>
-0000f870: 605f 5f2e 0a0a 2020 2020 2020 2020 2020  `__...          
-0000f880: 2020 5265 7175 6972 6564 2069 6e20 7468    Required in th
-0000f890: 6520 6060 5345 4c45 4354 6060 2063 6c61  e ``SELECT`` cla
-0000f8a0: 7573 652e 2049 6620 6120 6060 5748 4552  use. If a ``WHER
-0000f8b0: 4560 6020 636f 6e64 6974 696f 6e0a 2020  E`` condition.  
-0000f8c0: 2020 2020 2020 2020 2020 6f6e 2060 6072            on ``r
-0000f8d0: 6570 6f72 745f 6361 7465 676f 7279 5f69  eport_category_i
-0000f8e0: 6460 6020 6973 206e 6f74 2073 7065 6369  d`` is not speci
-0000f8f0: 6669 6564 2069 6e20 7468 6520 7175 6572  fied in the quer
-0000f900: 792c 0a20 2020 2020 2020 2020 2020 2072  y,.            r
-0000f910: 616e 6b69 6e67 7320 666f 7220 616c 6c20  ankings for all 
-0000f920: 746f 702d 6c65 7665 6c20 6361 7465 676f  top-level catego
-0000f930: 7269 6573 2061 7265 2072 6574 7572 6e65  ries are returne
-0000f940: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-0000f950: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-0000f960: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-0000f970: 605f 2060 605f 7265 706f 7274 5f63 6174  `_ ``_report_cat
-0000f980: 6567 6f72 795f 6964 6060 2e0a 2020 2020  egory_id``..    
-0000f990: 2020 2020 6272 616e 6420 2873 7472 293a      brand (str):
-0000f9a0: 0a20 2020 2020 2020 2020 2020 204e 616d  .            Nam
-0000f9b0: 6520 6f66 2074 6865 2062 7261 6e64 2e0a  e of the brand..
-0000f9c0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-0000f9d0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-0000f9e0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-0000f9f0: 6060 5f62 7261 6e64 6060 2e0a 2020 2020  ``_brand``..    
-0000fa00: 2020 2020 7261 6e6b 2028 696e 7429 3a0a      rank (int):.
-0000fa10: 2020 2020 2020 2020 2020 2020 506f 7075              Popu
-0000fa20: 6c61 7269 7479 206f 6620 7468 6520 6272  larity of the br
-0000fa30: 616e 6420 6f6e 2041 6473 2061 6e64 206f  and on Ads and o
-0000fa40: 7267 616e 6963 0a20 2020 2020 2020 2020  rganic.         
-0000fa50: 2020 2073 7572 6661 6365 732c 2069 6e20     surfaces, in 
-0000fa60: 7468 6520 7365 6c65 6374 6564 2063 6174  the selected cat
-0000fa70: 6567 6f72 7920 616e 6420 636f 756e 7472  egory and countr
-0000fa80: 792c 0a20 2020 2020 2020 2020 2020 2062  y,.            b
-0000fa90: 6173 6564 206f 6e20 7468 6520 6573 7469  ased on the esti
-0000faa0: 6d61 7465 6420 6e75 6d62 6572 206f 6620  mated number of 
-0000fab0: 756e 6974 7320 736f 6c64 2e0a 0a20 2020  units sold...   
-0000fac0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-0000fad0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-0000fae0: 6f66 2060 6f6e 656f 6660 5f20 6060 5f72  of `oneof`_ ``_r
-0000faf0: 616e 6b60 602e 0a20 2020 2020 2020 2070  ank``..        p
-0000fb00: 7265 7669 6f75 735f 7261 6e6b 2028 696e  revious_rank (in
-0000fb10: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0000fb20: 506f 7075 6c61 7269 7479 2072 616e 6b20  Popularity rank 
-0000fb30: 696e 2074 6865 2070 7265 7669 6f75 7320  in the previous 
-0000fb40: 7765 656b 206f 720a 2020 2020 2020 2020  week or.        
-0000fb50: 2020 2020 6d6f 6e74 682e 0a0a 2020 2020      month...    
-0000fb60: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-0000fb70: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-0000fb80: 6620 606f 6e65 6f66 605f 2060 605f 7072  f `oneof`_ ``_pr
-0000fb90: 6576 696f 7573 5f72 616e 6b60 602e 0a20  evious_rank``.. 
-0000fba0: 2020 2020 2020 2072 656c 6174 6976 655f         relative_
-0000fbb0: 6465 6d61 6e64 2028 676f 6f67 6c65 2e73  demand (google.s
-0000fbc0: 686f 7070 696e 672e 6d65 7263 6861 6e74  hopping.merchant
-0000fbd0: 5f72 6570 6f72 7473 5f76 3162 6574 612e  _reports_v1beta.
-0000fbe0: 7479 7065 732e 5265 6c61 7469 7665 4465  types.RelativeDe
-0000fbf0: 6d61 6e64 2e52 656c 6174 6976 6544 656d  mand.RelativeDem
-0000fc00: 616e 6445 6e75 6d29 3a0a 2020 2020 2020  andEnum):.      
-0000fc10: 2020 2020 2020 4573 7469 6d61 7465 6420        Estimated 
-0000fc20: 6465 6d61 6e64 2069 6e20 7265 6c61 7469  demand in relati
-0000fc30: 6f6e 2074 6f20 7468 6520 6272 616e 640a  on to the brand.
-0000fc40: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000fc50: 2074 6865 2068 6967 6865 7374 2070 6f70   the highest pop
-0000fc60: 756c 6172 6974 7920 7261 6e6b 2069 6e20  ularity rank in 
-0000fc70: 7468 6520 7361 6d65 0a20 2020 2020 2020  the same.       
-0000fc80: 2020 2020 2063 6174 6567 6f72 7920 616e       category an
-0000fc90: 6420 636f 756e 7472 792e 0a0a 2020 2020  d country...    
-0000fca0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-0000fcb0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-0000fcc0: 6620 606f 6e65 6f66 605f 2060 605f 7265  f `oneof`_ ``_re
-0000fcd0: 6c61 7469 7665 5f64 656d 616e 6460 602e  lative_demand``.
-0000fce0: 0a20 2020 2020 2020 2070 7265 7669 6f75  .        previou
-0000fcf0: 735f 7265 6c61 7469 7665 5f64 656d 616e  s_relative_deman
-0000fd00: 6420 2867 6f6f 676c 652e 7368 6f70 7069  d (google.shoppi
-0000fd10: 6e67 2e6d 6572 6368 616e 745f 7265 706f  ng.merchant_repo
-0000fd20: 7274 735f 7631 6265 7461 2e74 7970 6573  rts_v1beta.types
-0000fd30: 2e52 656c 6174 6976 6544 656d 616e 642e  .RelativeDemand.
-0000fd40: 5265 6c61 7469 7665 4465 6d61 6e64 456e  RelativeDemandEn
-0000fd50: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
-0000fd60: 2045 7374 696d 6174 6564 2064 656d 616e   Estimated deman
-0000fd70: 6420 696e 2072 656c 6174 696f 6e20 746f  d in relation to
-0000fd80: 2074 6865 2062 7261 6e64 0a20 2020 2020   the brand.     
-0000fd90: 2020 2020 2020 2077 6974 6820 7468 6520         with the 
-0000fda0: 6869 6768 6573 7420 706f 7075 6c61 7269  highest populari
-0000fdb0: 7479 2072 616e 6b20 696e 2074 6865 2073  ty rank in the s
-0000fdc0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-0000fdd0: 6361 7465 676f 7279 2061 6e64 2063 6f75  category and cou
-0000fde0: 6e74 7279 2069 6e20 7468 6520 7072 6576  ntry in the prev
-0000fdf0: 696f 7573 2077 6565 6b20 6f72 0a20 2020  ious week or.   
-0000fe00: 2020 2020 2020 2020 206d 6f6e 7468 2e0a           month..
-0000fe10: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-0000fe20: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-0000fe30: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-0000fe40: 6060 5f70 7265 7669 6f75 735f 7265 6c61  ``_previous_rela
-0000fe50: 7469 7665 5f64 656d 616e 6460 602e 0a20  tive_demand``.. 
-0000fe60: 2020 2020 2020 2072 656c 6174 6976 655f         relative_
-0000fe70: 6465 6d61 6e64 5f63 6861 6e67 6520 2867  demand_change (g
-0000fe80: 6f6f 676c 652e 7368 6f70 7069 6e67 2e6d  oogle.shopping.m
-0000fe90: 6572 6368 616e 745f 7265 706f 7274 735f  erchant_reports_
-0000fea0: 7631 6265 7461 2e74 7970 6573 2e52 656c  v1beta.types.Rel
-0000feb0: 6174 6976 6544 656d 616e 6443 6861 6e67  ativeDemandChang
-0000fec0: 6554 7970 652e 5265 6c61 7469 7665 4465  eType.RelativeDe
-0000fed0: 6d61 6e64 4368 616e 6765 5479 7065 456e  mandChangeTypeEn
-0000fee0: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
-0000fef0: 2043 6861 6e67 6520 696e 2074 6865 2065   Change in the e
-0000ff00: 7374 696d 6174 6564 2064 656d 616e 642e  stimated demand.
-0000ff10: 2057 6865 7468 6572 2069 740a 2020 2020   Whether it.    
-0000ff20: 2020 2020 2020 2020 726f 7365 2c20 7361          rose, sa
-0000ff30: 6e6b 206f 7220 7265 6d61 696e 6564 2066  nk or remained f
-0000ff40: 6c61 742e 0a0a 2020 2020 2020 2020 2020  lat...          
-0000ff50: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-0000ff60: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-0000ff70: 6f66 605f 2060 605f 7265 6c61 7469 7665  of`_ ``_relative
-0000ff80: 5f64 656d 616e 645f 6368 616e 6765 6060  _demand_change``
-0000ff90: 2e0a 2020 2020 2222 220a 0a20 2020 2072  ..    """..    r
-0000ffa0: 6570 6f72 745f 6461 7465 3a20 6461 7465  eport_date: date
-0000ffb0: 5f70 6232 2e44 6174 6520 3d20 7072 6f74  _pb2.Date = prot
-0000ffc0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-0000ffd0: 2070 726f 746f 2e4d 4553 5341 4745 2c0a   proto.MESSAGE,.
-0000ffe0: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
-0000fff0: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
-00010000: 653d 6461 7465 5f70 6232 2e44 6174 652c  e=date_pb2.Date,
-00010010: 0a20 2020 2029 0a20 2020 2072 6570 6f72  .    ).    repor
-00010020: 745f 6772 616e 756c 6172 6974 793a 2022  t_granularity: "
-00010030: 5265 706f 7274 4772 616e 756c 6172 6974  ReportGranularit
-00010040: 792e 5265 706f 7274 4772 616e 756c 6172  y.ReportGranular
-00010050: 6974 7945 6e75 6d22 203d 2070 726f 746f  ityEnum" = proto
-00010060: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
-00010070: 7072 6f74 6f2e 454e 554d 2c0a 2020 2020  proto.ENUM,.    
-00010080: 2020 2020 6e75 6d62 6572 3d32 2c0a 2020      number=2,.  
-00010090: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
-000100a0: 7275 652c 0a20 2020 2020 2020 2065 6e75  rue,.        enu
-000100b0: 6d3d 2252 6570 6f72 7447 7261 6e75 6c61  m="ReportGranula
-000100c0: 7269 7479 2e52 6570 6f72 7447 7261 6e75  rity.ReportGranu
-000100d0: 6c61 7269 7479 456e 756d 222c 0a20 2020  larityEnum",.   
-000100e0: 2029 0a20 2020 2072 6570 6f72 745f 636f   ).    report_co
-000100f0: 756e 7472 795f 636f 6465 3a20 7374 7220  untry_code: str 
-00010100: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00010110: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
-00010120: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
-00010130: 6265 723d 332c 0a20 2020 2020 2020 206f  ber=3,.        o
-00010140: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-00010150: 2020 290a 2020 2020 7265 706f 7274 5f63    ).    report_c
-00010160: 6174 6567 6f72 795f 6964 3a20 696e 7420  ategory_id: int 
-00010170: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00010180: 2020 2020 2020 2070 726f 746f 2e49 4e54         proto.INT
-00010190: 3634 2c0a 2020 2020 2020 2020 6e75 6d62  64,.        numb
-000101a0: 6572 3d34 2c0a 2020 2020 2020 2020 6f70  er=4,.        op
-000101b0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-000101c0: 2029 0a20 2020 2062 7261 6e64 3a20 7374   ).    brand: st
-000101d0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-000101e0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-000101f0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-00010200: 756d 6265 723d 362c 0a20 2020 2020 2020  umber=6,.       
-00010210: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-00010220: 2020 2020 290a 2020 2020 7261 6e6b 3a20      ).    rank: 
-00010230: 696e 7420 3d20 7072 6f74 6f2e 4669 656c  int = proto.Fiel
-00010240: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-00010250: 2e49 4e54 3634 2c0a 2020 2020 2020 2020  .INT64,.        
-00010260: 6e75 6d62 6572 3d37 2c0a 2020 2020 2020  number=7,.      
-00010270: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-00010280: 0a20 2020 2029 0a20 2020 2070 7265 7669  .    ).    previ
-00010290: 6f75 735f 7261 6e6b 3a20 696e 7420 3d20  ous_rank: int = 
-000102a0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-000102b0: 2020 2020 2070 726f 746f 2e49 4e54 3634       proto.INT64
-000102c0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-000102d0: 3d38 2c0a 2020 2020 2020 2020 6f70 7469  =8,.        opti
-000102e0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
-000102f0: 0a20 2020 2072 656c 6174 6976 655f 6465  .    relative_de
-00010300: 6d61 6e64 3a20 2252 656c 6174 6976 6544  mand: "RelativeD
-00010310: 656d 616e 642e 5265 6c61 7469 7665 4465  emand.RelativeDe
-00010320: 6d61 6e64 456e 756d 2220 3d20 7072 6f74  mandEnum" = prot
-00010330: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00010340: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
-00010350: 2020 2020 206e 756d 6265 723d 392c 0a20       number=9,. 
-00010360: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-00010370: 5472 7565 2c0a 2020 2020 2020 2020 656e  True,.        en
-00010380: 756d 3d22 5265 6c61 7469 7665 4465 6d61  um="RelativeDema
-00010390: 6e64 2e52 656c 6174 6976 6544 656d 616e  nd.RelativeDeman
-000103a0: 6445 6e75 6d22 2c0a 2020 2020 290a 2020  dEnum",.    ).  
-000103b0: 2020 7072 6576 696f 7573 5f72 656c 6174    previous_relat
-000103c0: 6976 655f 6465 6d61 6e64 3a20 2252 656c  ive_demand: "Rel
-000103d0: 6174 6976 6544 656d 616e 642e 5265 6c61  ativeDemand.Rela
-000103e0: 7469 7665 4465 6d61 6e64 456e 756d 2220  tiveDemandEnum" 
-000103f0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00010400: 2020 2020 2020 2070 726f 746f 2e45 4e55         proto.ENU
-00010410: 4d2c 0a20 2020 2020 2020 206e 756d 6265  M,.        numbe
-00010420: 723d 3130 2c0a 2020 2020 2020 2020 6f70  r=10,.        op
-00010430: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-00010440: 2020 2020 2065 6e75 6d3d 2252 656c 6174       enum="Relat
-00010450: 6976 6544 656d 616e 642e 5265 6c61 7469  iveDemand.Relati
-00010460: 7665 4465 6d61 6e64 456e 756d 222c 0a20  veDemandEnum",. 
-00010470: 2020 2029 0a20 2020 2072 656c 6174 6976     ).    relativ
-00010480: 655f 6465 6d61 6e64 5f63 6861 6e67 653a  e_demand_change:
-00010490: 2022 5265 6c61 7469 7665 4465 6d61 6e64   "RelativeDemand
-000104a0: 4368 616e 6765 5479 7065 2e52 656c 6174  ChangeType.Relat
-000104b0: 6976 6544 656d 616e 6443 6861 6e67 6554  iveDemandChangeT
-000104c0: 7970 6545 6e75 6d22 203d 2028 0a20 2020  ypeEnum" = (.   
-000104d0: 2020 2020 2070 726f 746f 2e46 6965 6c64       proto.Field
-000104e0: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
-000104f0: 6f74 6f2e 454e 554d 2c0a 2020 2020 2020  oto.ENUM,.      
-00010500: 2020 2020 2020 6e75 6d62 6572 3d31 312c        number=11,
-00010510: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
-00010520: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-00010530: 2020 2020 2020 2020 656e 756d 3d22 5265          enum="Re
-00010540: 6c61 7469 7665 4465 6d61 6e64 4368 616e  lativeDemandChan
-00010550: 6765 5479 7065 2e52 656c 6174 6976 6544  geType.RelativeD
-00010560: 656d 616e 6443 6861 6e67 6554 7970 6545  emandChangeTypeE
-00010570: 6e75 6d22 2c0a 2020 2020 2020 2020 290a  num",.        ).
-00010580: 2020 2020 290a 0a0a 636c 6173 7320 436f      )...class Co
-00010590: 6d70 6574 6974 6976 6556 6973 6962 696c  mpetitiveVisibil
-000105a0: 6974 7943 6f6d 7065 7469 746f 7256 6965  ityCompetitorVie
-000105b0: 7728 7072 6f74 6f2e 4d65 7373 6167 6529  w(proto.Message)
-000105c0: 3a0a 2020 2020 7222 2222 4669 656c 6473  :.    r"""Fields
-000105d0: 2061 7661 696c 6162 6c65 2066 6f72 2071   available for q
-000105e0: 7565 7279 2069 6e0a 2020 2020 6060 636f  uery in.    ``co
-000105f0: 6d70 6574 6974 6976 655f 7669 7369 6269  mpetitive_visibi
-00010600: 6c69 7479 5f63 6f6d 7065 7469 746f 725f  lity_competitor_
-00010610: 7669 6577 6060 2074 6162 6c65 2e0a 0a20  view`` table... 
-00010620: 2020 2060 436f 6d70 6574 6974 6976 650a     `Competitive.
-00010630: 2020 2020 7669 7369 6269 6c69 7479 203c      visibility <
-00010640: 6874 7470 733a 2f2f 7375 7070 6f72 742e  https://support.
-00010650: 676f 6f67 6c65 2e63 6f6d 2f6d 6572 6368  google.com/merch
-00010660: 616e 7473 2f61 6e73 7765 722f 3131 3336  ants/answer/1136
-00010670: 3634 3432 3e60 5f5f 0a20 2020 2072 6570  6442>`__.    rep
-00010680: 6f72 7420 7769 7468 2062 7573 696e 6573  ort with busines
-00010690: 7365 7320 7769 7468 2073 696d 696c 6172  ses with similar
-000106a0: 2076 6973 6962 696c 6974 792e 0a0a 2020   visibility...  
-000106b0: 2020 5661 6c75 6573 2061 7265 206f 6e6c    Values are onl
-000106c0: 7920 7365 7420 666f 7220 6669 656c 6473  y set for fields
-000106d0: 2072 6571 7565 7374 6564 2065 7870 6c69   requested expli
-000106e0: 6369 746c 7920 696e 2074 6865 2072 6571  citly in the req
-000106f0: 7565 7374 2773 0a20 2020 2073 6561 7263  uest's.    searc
-00010700: 6820 7175 6572 792e 0a0a 0a20 2020 202e  h query....    .
-00010710: 2e20 5f6f 6e65 6f66 3a20 6874 7470 733a  . _oneof: https:
-00010720: 2f2f 7072 6f74 6f2d 706c 7573 2d70 7974  //proto-plus-pyt
-00010730: 686f 6e2e 7265 6164 7468 6564 6f63 732e  hon.readthedocs.
-00010740: 696f 2f65 6e2f 7374 6162 6c65 2f66 6965  io/en/stable/fie
-00010750: 6c64 732e 6874 6d6c 236f 6e65 6f66 732d  lds.html#oneofs-
-00010760: 6d75 7475 616c 6c79 2d65 7863 6c75 7369  mutually-exclusi
-00010770: 7665 2d66 6965 6c64 730a 0a20 2020 2041  ve-fields..    A
-00010780: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
-00010790: 2020 2064 6174 6520 2867 6f6f 676c 652e     date (google.
-000107a0: 7479 7065 2e64 6174 655f 7062 322e 4461  type.date_pb2.Da
-000107b0: 7465 293a 0a20 2020 2020 2020 2020 2020  te):.           
-000107c0: 2044 6174 6520 6f66 2074 6869 7320 726f   Date of this ro
-000107d0: 772e 0a0a 2020 2020 2020 2020 2020 2020  w...            
-000107e0: 4120 636f 6e64 6974 696f 6e20 6f6e 2060  A condition on `
-000107f0: 6064 6174 6560 6020 6973 2072 6571 7569  `date`` is requi
-00010800: 7265 6420 696e 2074 6865 2060 6057 4845  red in the ``WHE
-00010810: 5245 6060 2063 6c61 7573 652e 0a20 2020  RE`` clause..   
-00010820: 2020 2020 2064 6f6d 6169 6e20 2873 7472       domain (str
-00010830: 293a 0a20 2020 2020 2020 2020 2020 2044  ):.            D
-00010840: 6f6d 6169 6e20 6f66 2079 6f75 7220 636f  omain of your co
-00010850: 6d70 6574 6974 6f72 206f 7220 796f 7572  mpetitor or your
-00010860: 2064 6f6d 6169 6e2c 2069 660a 2020 2020   domain, if.    
-00010870: 2020 2020 2020 2020 2769 735f 796f 7572          'is_your
-00010880: 5f64 6f6d 6169 6e27 2069 7320 7472 7565  _domain' is true
-00010890: 2e0a 0a20 2020 2020 2020 2020 2020 2052  ...            R
-000108a0: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
-000108b0: 6053 454c 4543 5460 6020 636c 6175 7365  `SELECT`` clause
-000108c0: 2e20 4361 6e6e 6f74 2062 6520 6669 6c74  . Cannot be filt
-000108d0: 6572 6564 206f 6e20 696e 0a20 2020 2020  ered on in.     
-000108e0: 2020 2020 2020 2074 6865 2027 5748 4552         the 'WHER
-000108f0: 4527 2063 6c61 7573 652e 0a0a 2020 2020  E' clause...    
-00010900: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-00010910: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-00010920: 6620 606f 6e65 6f66 605f 2060 605f 646f  f `oneof`_ ``_do
-00010930: 6d61 696e 6060 2e0a 2020 2020 2020 2020  main``..        
-00010940: 6973 5f79 6f75 725f 646f 6d61 696e 2028  is_your_domain (
-00010950: 626f 6f6c 293a 0a20 2020 2020 2020 2020  bool):.         
-00010960: 2020 2054 7275 6520 6966 2074 6869 7320     True if this 
-00010970: 726f 7720 636f 6e74 6169 6e73 2064 6174  row contains dat
-00010980: 6120 666f 7220 796f 7572 0a20 2020 2020  a for your.     
-00010990: 2020 2020 2020 2064 6f6d 6169 6e2e 0a20         domain.. 
-000109a0: 2020 2020 2020 2020 2020 2043 616e 6e6f             Canno
-000109b0: 7420 6265 2066 696c 7465 7265 6420 6f6e  t be filtered on
-000109c0: 2069 6e20 7468 6520 2757 4845 5245 2720   in the 'WHERE' 
-000109d0: 636c 6175 7365 2e0a 0a20 2020 2020 2020  clause...       
-000109e0: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-000109f0: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-00010a00: 6f6e 656f 6660 5f20 6060 5f69 735f 796f  oneof`_ ``_is_yo
-00010a10: 7572 5f64 6f6d 6169 6e60 602e 0a20 2020  ur_domain``..   
-00010a20: 2020 2020 2072 6570 6f72 745f 636f 756e       report_coun
-00010a30: 7472 795f 636f 6465 2028 7374 7229 3a0a  try_code (str):.
-00010a40: 2020 2020 2020 2020 2020 2020 436f 756e              Coun
-00010a50: 7472 7920 7768 6572 6520 696d 7072 6573  try where impres
-00010a60: 7369 6f6e 7320 6170 7065 6172 6564 2e0a  sions appeared..
-00010a70: 0a20 2020 2020 2020 2020 2020 2052 6571  .            Req
-00010a80: 7569 7265 6420 696e 2074 6865 2060 6053  uired in the ``S
-00010a90: 454c 4543 5460 6020 636c 6175 7365 2e20  ELECT`` clause. 
-00010aa0: 4120 636f 6e64 6974 696f 6e20 6f6e 0a20  A condition on. 
-00010ab0: 2020 2020 2020 2020 2020 2060 6072 6570             ``rep
-00010ac0: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
-00010ad0: 6060 2069 7320 7265 7175 6972 6564 2069  `` is required i
-00010ae0: 6e20 7468 6520 6060 5748 4552 4560 6020  n the ``WHERE`` 
-00010af0: 636c 6175 7365 2e0a 0a20 2020 2020 2020  clause...       
-00010b00: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-00010b10: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-00010b20: 6f6e 656f 6660 5f20 6060 5f72 6570 6f72  oneof`_ ``_repor
-00010b30: 745f 636f 756e 7472 795f 636f 6465 6060  t_country_code``
-00010b40: 2e0a 2020 2020 2020 2020 7265 706f 7274  ..        report
-00010b50: 5f63 6174 6567 6f72 795f 6964 2028 696e  _category_id (in
-00010b60: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00010b70: 476f 6f67 6c65 2070 726f 6475 6374 2063  Google product c
-00010b80: 6174 6567 6f72 7920 4944 2074 6f20 6361  ategory ID to ca
-00010b90: 6c63 756c 6174 6520 7468 6520 7265 706f  lculate the repo
-00010ba0: 7274 2066 6f72 2c0a 2020 2020 2020 2020  rt for,.        
-00010bb0: 2020 2020 7265 7072 6573 656e 7465 6420      represented 
-00010bc0: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
-00010bd0: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
-00010be0: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
-00010bf0: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-00010c00: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-00010c10: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
-00010c20: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
-00010c30: 2052 6571 7569 7265 6420 696e 2074 6865   Required in the
-00010c40: 2060 6053 454c 4543 5460 6020 636c 6175   ``SELECT`` clau
-00010c50: 7365 2e20 4120 636f 6e64 6974 696f 6e20  se. A condition 
-00010c60: 6f6e 0a20 2020 2020 2020 2020 2020 2060  on.            `
-00010c70: 6072 6570 6f72 745f 6361 7465 676f 7279  `report_category
-00010c80: 5f69 6460 6020 6973 2072 6571 7569 7265  _id`` is require
-00010c90: 6420 696e 2074 6865 2060 6057 4845 5245  d in the ``WHERE
-00010ca0: 6060 2063 6c61 7573 652e 0a0a 2020 2020  `` clause...    
-00010cb0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
-00010cc0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
-00010cd0: 6620 606f 6e65 6f66 605f 2060 605f 7265  f `oneof`_ ``_re
-00010ce0: 706f 7274 5f63 6174 6567 6f72 795f 6964  port_category_id
-00010cf0: 6060 2e0a 2020 2020 2020 2020 7472 6166  ``..        traf
-00010d00: 6669 635f 736f 7572 6365 2028 676f 6f67  fic_source (goog
-00010d10: 6c65 2e73 686f 7070 696e 672e 6d65 7263  le.shopping.merc
-00010d20: 6861 6e74 5f72 6570 6f72 7473 5f76 3162  hant_reports_v1b
-00010d30: 6574 612e 7479 7065 732e 5472 6166 6669  eta.types.Traffi
-00010d40: 6353 6f75 7263 652e 5472 6166 6669 6353  cSource.TrafficS
-00010d50: 6f75 7263 6545 6e75 6d29 3a0a 2020 2020  ourceEnum):.    
-00010d60: 2020 2020 2020 2020 5472 6166 6669 6320          Traffic 
-00010d70: 736f 7572 6365 206f 6620 696d 7072 6573  source of impres
-00010d80: 7369 6f6e 732e 0a0a 2020 2020 2020 2020  sions...        
-00010d90: 2020 2020 5265 7175 6972 6564 2069 6e20      Required in 
-00010da0: 7468 6520 6060 5345 4c45 4354 6060 2063  the ``SELECT`` c
-00010db0: 6c61 7573 652e 0a0a 2020 2020 2020 2020  lause...        
-00010dc0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
-00010dd0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
-00010de0: 6e65 6f66 605f 2060 605f 7472 6166 6669  neof`_ ``_traffi
-00010df0: 635f 736f 7572 6365 6060 2e0a 2020 2020  c_source``..    
-00010e00: 2020 2020 7261 6e6b 2028 696e 7429 3a0a      rank (int):.
-00010e10: 2020 2020 2020 2020 2020 2020 506f 7369              Posi
-00010e20: 7469 6f6e 206f 6620 7468 6520 646f 6d61  tion of the doma
-00010e30: 696e 2069 6e20 7468 6520 7369 6d69 6c61  in in the simila
-00010e40: 7220 6275 7369 6e65 7373 6573 2072 616e  r businesses ran
-00010e50: 6b69 6e67 2066 6f72 0a20 2020 2020 2020  king for.       
-00010e60: 2020 2020 2074 6865 2073 656c 6563 7465       the selecte
-00010e70: 6420 6b65 7973 2028 6060 6461 7465 6060  d keys (``date``
-00010e80: 2c20 6060 7265 706f 7274 5f63 6174 6567  , ``report_categ
-00010e90: 6f72 795f 6964 6060 2c0a 2020 2020 2020  ory_id``,.      
-00010ea0: 2020 2020 2020 6060 7265 706f 7274 5f63        ``report_c
-00010eb0: 6f75 6e74 7279 5f63 6f64 6560 602c 2060  ountry_code``, `
-00010ec0: 6074 7261 6666 6963 5f73 6f75 7263 6560  `traffic_source`
-00010ed0: 6029 2062 6173 6564 206f 6e0a 2020 2020  `) based on.    
-00010ee0: 2020 2020 2020 2020 696d 7072 6573 7369          impressi
-00010ef0: 6f6e 732e 2031 2069 7320 7468 6520 6869  ons. 1 is the hi
-00010f00: 6768 6573 742e 0a0a 2020 2020 2020 2020  ghest...        
-00010f10: 2020 2020 4361 6e6e 6f74 2062 6520 6669      Cannot be fi
-00010f20: 6c74 6572 6564 206f 6e20 696e 2074 6865  ltered on in the
-00010f30: 2027 5748 4552 4527 2063 6c61 7573 652e   'WHERE' clause.
-00010f40: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00010f50: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-00010f60: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-00010f70: 2060 605f 7261 6e6b 6060 2e0a 2020 2020   ``_rank``..    
-00010f80: 2020 2020 6164 735f 6f72 6761 6e69 635f      ads_organic_
-00010f90: 7261 7469 6f20 2866 6c6f 6174 293a 0a20  ratio (float):. 
-00010fa0: 2020 2020 2020 2020 2020 205b 4164 7320             [Ads 
-00010fb0: 2f20 6f72 6761 6e69 6320 7261 7469 6f5d  / organic ratio]
-00010fc0: 0a20 2020 2020 2020 2020 2020 2028 6874  .            (ht
-00010fd0: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
-00010fe0: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
-00010ff0: 7473 2f61 6e73 7765 722f 3131 3336 3634  ts/answer/113664
-00011000: 3432 237a 6970 7079 3d25 3243 6164 732d  42#zippy=%2Cads-
-00011010: 6672 6565 2d72 6174 696f 290a 2020 2020  free-ratio).    
-00011020: 2020 2020 2020 2020 7368 6f77 7320 686f          shows ho
-00011030: 7720 6f66 7465 6e20 7468 6520 646f 6d61  w often the doma
-00011040: 696e 2072 6563 6569 7665 7320 696d 7072  in receives impr
-00011050: 6573 7369 6f6e 7320 6672 6f6d 0a20 2020  essions from.   
-00011060: 2020 2020 2020 2020 2053 686f 7070 696e           Shoppin
-00011070: 6720 6164 7320 636f 6d70 6172 6564 2074  g ads compared t
-00011080: 6f20 6f72 6761 6e69 6320 7472 6166 6669  o organic traffi
-00011090: 632e 2054 6865 206e 756d 6265 7220 6973  c. The number is
-000110a0: 0a20 2020 2020 2020 2020 2020 2072 6f75  .            rou
-000110b0: 6e64 6564 2061 6e64 2062 7563 6b65 7465  nded and buckete
-000110c0: 642e 0a0a 2020 2020 2020 2020 2020 2020  d...            
-000110d0: 4361 6e6e 6f74 2062 6520 6669 6c74 6572  Cannot be filter
-000110e0: 6564 206f 6e20 696e 2074 6865 2027 5748  ed on in the 'WH
-000110f0: 4552 4527 2063 6c61 7573 652e 0a0a 2020  ERE' clause...  
-00011100: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00011110: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-00011120: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-00011130: 6164 735f 6f72 6761 6e69 635f 7261 7469  ads_organic_rati
-00011140: 6f60 602e 0a20 2020 2020 2020 2070 6167  o``..        pag
-00011150: 655f 6f76 6572 6c61 705f 7261 7465 2028  e_overlap_rate (
-00011160: 666c 6f61 7429 3a0a 2020 2020 2020 2020  float):.        
-00011170: 2020 2020 5b50 6167 6520 6f76 6572 6c61      [Page overla
-00011180: 7020 7261 7465 5d0a 2020 2020 2020 2020  p rate].        
-00011190: 2020 2020 2868 7474 7073 3a2f 2f73 7570      (https://sup
-000111a0: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-000111b0: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-000111c0: 2f31 3133 3636 3434 3223 7a69 7070 793d  /11366442#zippy=
-000111d0: 2532 4370 6167 652d 6f76 6572 6c61 702d  %2Cpage-overlap-
-000111e0: 7261 7465 290a 2020 2020 2020 2020 2020  rate).          
-000111f0: 2020 7368 6f77 7320 686f 7720 6672 6571    shows how freq
-00011200: 7565 6e74 6c79 2063 6f6d 7065 7469 6e67  uently competing
-00011210: 2072 6574 6169 6c65 7273 e280 9920 6f66   retailers... of
-00011220: 6665 7273 2061 7265 2073 686f 776e 0a20  fers are shown. 
-00011230: 2020 2020 2020 2020 2020 2074 6f67 6574             toget
-00011240: 6865 7220 7769 7468 2079 6f75 7220 6f66  her with your of
-00011250: 6665 7273 206f 6e20 7468 6520 7361 6d65  fers on the same
-00011260: 2070 6167 652e 0a0a 2020 2020 2020 2020   page...        
-00011270: 2020 2020 4361 6e6e 6f74 2062 6520 6669      Cannot be fi
-00011280: 6c74 6572 6564 206f 6e20 696e 2074 6865  ltered on in the
-00011290: 2027 5748 4552 4527 2063 6c61 7573 652e   'WHERE' clause.
-000112a0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-000112b0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
-000112c0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
-000112d0: 2060 605f 7061 6765 5f6f 7665 726c 6170   ``_page_overlap
-000112e0: 5f72 6174 6560 602e 0a20 2020 2020 2020  _rate``..       
-000112f0: 2068 6967 6865 725f 706f 7369 7469 6f6e   higher_position
-00011300: 5f72 6174 6520 2866 6c6f 6174 293a 0a20  _rate (float):. 
-00011310: 2020 2020 2020 2020 2020 205b 4869 6768             [High
-00011320: 6572 2070 6f73 6974 696f 6e20 7261 7465  er position rate
-00011330: 5d0a 2020 2020 2020 2020 2020 2020 2868  ].            (h
-00011340: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
-00011350: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
-00011360: 6e74 732f 616e 7377 6572 2f31 3133 3636  nts/answer/11366
-00011370: 3434 3223 7a69 7070 793d 2532 4368 6967  442#zippy=%2Chig
-00011380: 6865 722d 706f 7369 7469 6f6e 2d72 6174  her-position-rat
-00011390: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-000113a0: 686f 7773 2068 6f77 206f 6674 656e 2061  hows how often a
-000113b0: 2063 6f6d 7065 7469 746f 72e2 8099 7320   competitor...s 
-000113c0: 6f66 6665 7220 676f 7420 706c 6163 6564  offer got placed
-000113d0: 2069 6e20 6120 6869 6768 6572 0a20 2020   in a higher.   
-000113e0: 2020 2020 2020 2020 2070 6f73 6974 696f           positio
-000113f0: 6e20 6f6e 2074 6865 2070 6167 6520 7468  n on the page th
-00011400: 616e 2079 6f75 7220 6f66 6665 722e 0a0a  an your offer...
-00011410: 2020 2020 2020 2020 2020 2020 4361 6e6e              Cann
-00011420: 6f74 2062 6520 6669 6c74 6572 6564 206f  ot be filtered o
-00011430: 6e20 696e 2074 6865 2027 5748 4552 4527  n in the 'WHERE'
-00011440: 2063 6c61 7573 652e 0a0a 2020 2020 2020   clause...      
-00011450: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-00011460: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-00011470: 606f 6e65 6f66 605f 2060 605f 6869 6768  `oneof`_ ``_high
-00011480: 6572 5f70 6f73 6974 696f 6e5f 7261 7465  er_position_rate
-00011490: 6060 2e0a 2020 2020 2020 2020 7265 6c61  ``..        rela
-000114a0: 7469 7665 5f76 6973 6962 696c 6974 7920  tive_visibility 
-000114b0: 2866 6c6f 6174 293a 0a20 2020 2020 2020  (float):.       
-000114c0: 2020 2020 205b 5265 6c61 7469 7665 2076       [Relative v
-000114d0: 6973 6962 696c 6974 795d 0a20 2020 2020  isibility].     
-000114e0: 2020 2020 2020 2028 6874 7470 733a 2f2f         (https://
-000114f0: 7375 7070 6f72 742e 676f 6f67 6c65 2e63  support.google.c
-00011500: 6f6d 2f6d 6572 6368 616e 7473 2f61 6e73  om/merchants/ans
-00011510: 7765 722f 3131 3336 3634 3432 237a 6970  wer/11366442#zip
-00011520: 7079 3d25 3243 7265 6c61 7469 7665 2d76  py=%2Crelative-v
-00011530: 6973 6962 696c 6974 7929 0a20 2020 2020  isibility).     
-00011540: 2020 2020 2020 2073 686f 7773 2068 6f77         shows how
-00011550: 206f 6674 656e 2079 6f75 7220 636f 6d70   often your comp
-00011560: 6574 6974 6f72 73e2 8099 206f 6666 6572  etitors... offer
-00011570: 7320 6172 6520 7368 6f77 6e20 636f 6d70  s are shown comp
-00011580: 6172 6564 0a20 2020 2020 2020 2020 2020  ared.           
-00011590: 2074 6f20 796f 7572 206f 6666 6572 732e   to your offers.
-000115a0: 2049 6e20 6f74 6865 7220 776f 7264 732c   In other words,
-000115b0: 2074 6869 7320 6973 2074 6865 206e 756d   this is the num
-000115c0: 6265 7220 6f66 0a20 2020 2020 2020 2020  ber of.         
-000115d0: 2020 2064 6973 706c 6179 6564 2069 6d70     displayed imp
-000115e0: 7265 7373 696f 6e73 206f 6620 6120 636f  ressions of a co
-000115f0: 6d70 6574 6974 6f72 2072 6574 6169 6c65  mpetitor retaile
-00011600: 7220 6469 7669 6465 6420 6279 0a20 2020  r divided by.   
-00011610: 2020 2020 2020 2020 2074 6865 206e 756d           the num
-00011620: 6265 7220 6f66 2079 6f75 7220 6469 7370  ber of your disp
-00011630: 6c61 7965 6420 696d 7072 6573 7369 6f6e  layed impression
-00011640: 7320 6475 7269 6e67 2061 2073 656c 6563  s during a selec
-00011650: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
-00011660: 7469 6d65 2072 616e 6765 2066 6f72 2061  time range for a
-00011670: 2073 656c 6563 7465 6420 7072 6f64 7563   selected produc
-00011680: 7420 6361 7465 676f 7279 2061 6e64 2063  t category and c
-00011690: 6f75 6e74 7279 2e0a 0a20 2020 2020 2020  ountry...       
-000116a0: 2020 2020 2043 616e 6e6f 7420 6265 2066       Cannot be f
-000116b0: 696c 7465 7265 6420 6f6e 2069 6e20 7468  iltered on in th
-000116c0: 6520 2757 4845 5245 2720 636c 6175 7365  e 'WHERE' clause
-000116d0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-000116e0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
-000116f0: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
-00011700: 5f20 6060 5f72 656c 6174 6976 655f 7669  _ ``_relative_vi
-00011710: 7369 6269 6c69 7479 6060 2e0a 2020 2020  sibility``..    
-00011720: 2222 220a 0a20 2020 2064 6174 653a 2064  """..    date: d
-00011730: 6174 655f 7062 322e 4461 7465 203d 2070  ate_pb2.Date = p
-00011740: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
-00011750: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
-00011760: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
-00011770: 723d 312c 0a20 2020 2020 2020 206d 6573  r=1,.        mes
-00011780: 7361 6765 3d64 6174 655f 7062 322e 4461  sage=date_pb2.Da
-00011790: 7465 2c0a 2020 2020 290a 2020 2020 646f  te,.    ).    do
-000117a0: 6d61 696e 3a20 7374 7220 3d20 7072 6f74  main: str = prot
-000117b0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-000117c0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-000117d0: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
-000117e0: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-000117f0: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-00011800: 2020 6973 5f79 6f75 725f 646f 6d61 696e    is_your_domain
-00011810: 3a20 626f 6f6c 203d 2070 726f 746f 2e46  : bool = proto.F
-00011820: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
-00011830: 6f74 6f2e 424f 4f4c 2c0a 2020 2020 2020  oto.BOOL,.      
-00011840: 2020 6e75 6d62 6572 3d33 2c0a 2020 2020    number=3,.    
-00011850: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-00011860: 652c 0a20 2020 2029 0a20 2020 2072 6570  e,.    ).    rep
-00011870: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
-00011880: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
-00011890: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-000118a0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
-000118b0: 2020 206e 756d 6265 723d 342c 0a20 2020     number=4,.   
-000118c0: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
-000118d0: 7565 2c0a 2020 2020 290a 2020 2020 7265  ue,.    ).    re
-000118e0: 706f 7274 5f63 6174 6567 6f72 795f 6964  port_category_id
-000118f0: 3a20 696e 7420 3d20 7072 6f74 6f2e 4669  : int = proto.Fi
-00011900: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
-00011910: 746f 2e49 4e54 3634 2c0a 2020 2020 2020  to.INT64,.      
-00011920: 2020 6e75 6d62 6572 3d35 2c0a 2020 2020    number=5,.    
-00011930: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-00011940: 652c 0a20 2020 2029 0a20 2020 2074 7261  e,.    ).    tra
-00011950: 6666 6963 5f73 6f75 7263 653a 2022 5472  ffic_source: "Tr
-00011960: 6166 6669 6353 6f75 7263 652e 5472 6166  afficSource.Traf
-00011970: 6669 6353 6f75 7263 6545 6e75 6d22 203d  ficSourceEnum" =
-00011980: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-00011990: 2020 2020 2020 7072 6f74 6f2e 454e 554d        proto.ENUM
-000119a0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
-000119b0: 3d36 2c0a 2020 2020 2020 2020 6f70 7469  =6,.        opti
-000119c0: 6f6e 616c 3d54 7275 652c 0a20 2020 2020  onal=True,.     
-000119d0: 2020 2065 6e75 6d3d 2254 7261 6666 6963     enum="Traffic
-000119e0: 536f 7572 6365 2e54 7261 6666 6963 536f  Source.TrafficSo
-000119f0: 7572 6365 456e 756d 222c 0a20 2020 2029  urceEnum",.    )
-00011a00: 0a20 2020 2072 616e 6b3a 2069 6e74 203d  .    rank: int =
-00011a10: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-00011a20: 2020 2020 2020 7072 6f74 6f2e 494e 5436        proto.INT6
-00011a30: 342c 0a20 2020 2020 2020 206e 756d 6265  4,.        numbe
-00011a40: 723d 372c 0a20 2020 2020 2020 206f 7074  r=7,.        opt
-00011a50: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-00011a60: 290a 2020 2020 6164 735f 6f72 6761 6e69  ).    ads_organi
-00011a70: 635f 7261 7469 6f3a 2066 6c6f 6174 203d  c_ratio: float =
-00011a80: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
-00011a90: 2020 2020 2020 7072 6f74 6f2e 444f 5542        proto.DOUB
-00011aa0: 4c45 2c0a 2020 2020 2020 2020 6e75 6d62  LE,.        numb
-00011ab0: 6572 3d38 2c0a 2020 2020 2020 2020 6f70  er=8,.        op
-00011ac0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
-00011ad0: 2029 0a20 2020 2070 6167 655f 6f76 6572   ).    page_over
-00011ae0: 6c61 705f 7261 7465 3a20 666c 6f61 7420  lap_rate: float 
-00011af0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
-00011b00: 2020 2020 2020 2070 726f 746f 2e44 4f55         proto.DOU
-00011b10: 424c 452c 0a20 2020 2020 2020 206e 756d  BLE,.        num
-00011b20: 6265 723d 392c 0a20 2020 2020 2020 206f  ber=9,.        o
-00011b30: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
-00011b40: 2020 290a 2020 2020 6869 6768 6572 5f70    ).    higher_p
-00011b50: 6f73 6974 696f 6e5f 7261 7465 3a20 666c  osition_rate: fl
-00011b60: 6f61 7420 3d20 7072 6f74 6f2e 4669 656c  oat = proto.Fiel
-00011b70: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-00011b80: 2e44 4f55 424c 452c 0a20 2020 2020 2020  .DOUBLE,.       
-00011b90: 206e 756d 6265 723d 3130 2c0a 2020 2020   number=10,.    
-00011ba0: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-00011bb0: 652c 0a20 2020 2029 0a20 2020 2072 656c  e,.    ).    rel
-00011bc0: 6174 6976 655f 7669 7369 6269 6c69 7479  ative_visibility
-00011bd0: 3a20 666c 6f61 7420 3d20 7072 6f74 6f2e  : float = proto.
-00011be0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00011bf0: 726f 746f 2e44 4f55 424c 452c 0a20 2020  roto.DOUBLE,.   
-00011c00: 2020 2020 206e 756d 6265 723d 3131 2c0a       number=11,.
-00011c10: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-00011c20: 3d54 7275 652c 0a20 2020 2029 0a0a 0a63  =True,.    )...c
-00011c30: 6c61 7373 2043 6f6d 7065 7469 7469 7665  lass Competitive
-00011c40: 5669 7369 6269 6c69 7479 546f 704d 6572  VisibilityTopMer
-00011c50: 6368 616e 7456 6965 7728 7072 6f74 6f2e  chantView(proto.
-00011c60: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
-00011c70: 2222 4669 656c 6473 2061 7661 696c 6162  ""Fields availab
-00011c80: 6c65 2066 6f72 2071 7565 7279 2069 6e0a  le for query in.
-00011c90: 2020 2020 6060 636f 6d70 6574 6974 6976      ``competitiv
-00011ca0: 655f 7669 7369 6269 6c69 7479 5f74 6f70  e_visibility_top
-00011cb0: 5f6d 6572 6368 616e 745f 7669 6577 6060  _merchant_view``
-00011cc0: 2074 6162 6c65 2e0a 0a20 2020 2060 436f   table...    `Co
-00011cd0: 6d70 6574 6974 6976 650a 2020 2020 7669  mpetitive.    vi
-00011ce0: 7369 6269 6c69 7479 203c 6874 7470 733a  sibility <https:
-00011cf0: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
-00011d00: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
-00011d10: 6e73 7765 722f 3131 3336 3634 3432 3e60  nswer/11366442>`
-00011d20: 5f5f 0a20 2020 2072 6570 6f72 7420 7769  __.    report wi
-00011d30: 7468 2062 7573 696e 6573 7320 7769 7468  th business with
-00011d40: 2068 6967 6865 7374 2076 6973 6962 696c   highest visibil
-00011d50: 6974 792e 0a0a 2020 2020 5661 6c75 6573  ity...    Values
-00011d60: 2061 7265 206f 6e6c 7920 7365 7420 666f   are only set fo
-00011d70: 7220 6669 656c 6473 2072 6571 7565 7374  r fields request
-00011d80: 6564 2065 7870 6c69 6369 746c 7920 696e  ed explicitly in
-00011d90: 2074 6865 2072 6571 7565 7374 2773 0a20   the request's. 
-00011da0: 2020 2073 6561 7263 6820 7175 6572 792e     search query.
-00011db0: 0a0a 0a20 2020 202e 2e20 5f6f 6e65 6f66  ...    .. _oneof
-00011dc0: 3a20 6874 7470 733a 2f2f 7072 6f74 6f2d  : https://proto-
-00011dd0: 706c 7573 2d70 7974 686f 6e2e 7265 6164  plus-python.read
-00011de0: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
-00011df0: 6162 6c65 2f66 6965 6c64 732e 6874 6d6c  able/fields.html
-00011e00: 236f 6e65 6f66 732d 6d75 7475 616c 6c79  #oneofs-mutually
-00011e10: 2d65 7863 6c75 7369 7665 2d66 6965 6c64  -exclusive-field
-00011e20: 730a 0a20 2020 2041 7474 7269 6275 7465  s..    Attribute
-00011e30: 733a 0a20 2020 2020 2020 2064 6174 6520  s:.        date 
-00011e40: 2867 6f6f 676c 652e 7479 7065 2e64 6174  (google.type.dat
-00011e50: 655f 7062 322e 4461 7465 293a 0a20 2020  e_pb2.Date):.   
-00011e60: 2020 2020 2020 2020 2044 6174 6520 6f66           Date of
-00011e70: 2074 6869 7320 726f 772e 0a0a 2020 2020   this row...    
-00011e80: 2020 2020 2020 2020 4361 6e6e 6f74 2062          Cannot b
-00011e90: 6520 7365 6c65 6374 6564 2069 6e20 7468  e selected in th
-00011ea0: 6520 6060 5345 4c45 4354 6060 2063 6c61  e ``SELECT`` cla
-00011eb0: 7573 652e 2041 2063 6f6e 6469 7469 6f6e  use. A condition
-00011ec0: 206f 6e0a 2020 2020 2020 2020 2020 2020   on.            
-00011ed0: 6060 6461 7465 6060 2069 7320 7265 7175  ``date`` is requ
-00011ee0: 6972 6564 2069 6e20 7468 6520 6060 5748  ired in the ``WH
-00011ef0: 4552 4560 6020 636c 6175 7365 2e0a 2020  ERE`` clause..  
-00011f00: 2020 2020 2020 646f 6d61 696e 2028 7374        domain (st
-00011f10: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00011f20: 446f 6d61 696e 206f 6620 796f 7572 2063  Domain of your c
-00011f30: 6f6d 7065 7469 746f 7220 6f72 2079 6f75  ompetitor or you
-00011f40: 7220 646f 6d61 696e 2c20 6966 0a20 2020  r domain, if.   
-00011f50: 2020 2020 2020 2020 2027 6973 5f79 6f75           'is_you
-00011f60: 725f 646f 6d61 696e 2720 6973 2074 7275  r_domain' is tru
-00011f70: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
-00011f80: 5265 7175 6972 6564 2069 6e20 7468 6520  Required in the 
-00011f90: 6060 5345 4c45 4354 6060 2063 6c61 7573  ``SELECT`` claus
-00011fa0: 652e 2043 616e 6e6f 7420 6265 2066 696c  e. Cannot be fil
-00011fb0: 7465 7265 6420 6f6e 2069 6e0a 2020 2020  tered on in.    
-00011fc0: 2020 2020 2020 2020 7468 6520 2757 4845          the 'WHE
-00011fd0: 5245 2720 636c 6175 7365 2e0a 0a20 2020  RE' clause...   
-00011fe0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-00011ff0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-00012000: 6f66 2060 6f6e 656f 6660 5f20 6060 5f64  of `oneof`_ ``_d
-00012010: 6f6d 6169 6e60 602e 0a20 2020 2020 2020  omain``..       
-00012020: 2069 735f 796f 7572 5f64 6f6d 6169 6e20   is_your_domain 
-00012030: 2862 6f6f 6c29 3a0a 2020 2020 2020 2020  (bool):.        
-00012040: 2020 2020 5472 7565 2069 6620 7468 6973      True if this
-00012050: 2072 6f77 2063 6f6e 7461 696e 7320 6461   row contains da
-00012060: 7461 2066 6f72 2079 6f75 720a 2020 2020  ta for your.    
-00012070: 2020 2020 2020 2020 646f 6d61 696e 2e0a          domain..
-00012080: 2020 2020 2020 2020 2020 2020 4361 6e6e              Cann
-00012090: 6f74 2062 6520 6669 6c74 6572 6564 206f  ot be filtered o
-000120a0: 6e20 696e 2074 6865 2027 5748 4552 4527  n in the 'WHERE'
-000120b0: 2063 6c61 7573 652e 0a0a 2020 2020 2020   clause...      
-000120c0: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-000120d0: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-000120e0: 606f 6e65 6f66 605f 2060 605f 6973 5f79  `oneof`_ ``_is_y
-000120f0: 6f75 725f 646f 6d61 696e 6060 2e0a 2020  our_domain``..  
-00012100: 2020 2020 2020 7265 706f 7274 5f63 6f75        report_cou
-00012110: 6e74 7279 5f63 6f64 6520 2873 7472 293a  ntry_code (str):
-00012120: 0a20 2020 2020 2020 2020 2020 2043 6f75  .            Cou
-00012130: 6e74 7279 2077 6865 7265 2069 6d70 7265  ntry where impre
-00012140: 7373 696f 6e73 2061 7070 6561 7265 642e  ssions appeared.
-00012150: 0a0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
-00012160: 7175 6972 6564 2069 6e20 7468 6520 6060  quired in the ``
-00012170: 5345 4c45 4354 6060 2063 6c61 7573 652e  SELECT`` clause.
-00012180: 2041 2063 6f6e 6469 7469 6f6e 206f 6e0a   A condition on.
-00012190: 2020 2020 2020 2020 2020 2020 6060 7265              ``re
-000121a0: 706f 7274 5f63 6f75 6e74 7279 5f63 6f64  port_country_cod
-000121b0: 6560 6020 6973 2072 6571 7569 7265 6420  e`` is required 
-000121c0: 696e 2074 6865 2060 6057 4845 5245 6060  in the ``WHERE``
-000121d0: 2063 6c61 7573 652e 0a0a 2020 2020 2020   clause...      
-000121e0: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-000121f0: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-00012200: 606f 6e65 6f66 605f 2060 605f 7265 706f  `oneof`_ ``_repo
-00012210: 7274 5f63 6f75 6e74 7279 5f63 6f64 6560  rt_country_code`
-00012220: 602e 0a20 2020 2020 2020 2072 6570 6f72  `..        repor
-00012230: 745f 6361 7465 676f 7279 5f69 6420 2869  t_category_id (i
-00012240: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-00012250: 2047 6f6f 676c 6520 7072 6f64 7563 7420   Google product 
-00012260: 6361 7465 676f 7279 2049 4420 746f 2063  category ID to c
-00012270: 616c 6375 6c61 7465 2074 6865 2072 6570  alculate the rep
-00012280: 6f72 7420 666f 722c 0a20 2020 2020 2020  ort for,.       
-00012290: 2020 2020 2072 6570 7265 7365 6e74 6564       represented
-000122a0: 2069 6e20 6047 6f6f 676c 6527 7320 7072   in `Google's pr
-000122b0: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
-000122c0: 2020 7461 786f 6e6f 6d79 203c 6874 7470    taxonomy <http
-000122d0: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
-000122e0: 6c65 2e63 6f6d 2f6d 6572 6368 616e 7473  le.com/merchants
-000122f0: 2f61 6e73 7765 722f 3633 3234 3433 363e  /answer/6324436>
-00012300: 605f 5f2e 0a0a 2020 2020 2020 2020 2020  `__...          
-00012310: 2020 5265 7175 6972 6564 2069 6e20 7468    Required in th
-00012320: 6520 6060 5345 4c45 4354 6060 2063 6c61  e ``SELECT`` cla
-00012330: 7573 652e 2041 2063 6f6e 6469 7469 6f6e  use. A condition
-00012340: 206f 6e0a 2020 2020 2020 2020 2020 2020   on.            
-00012350: 6060 7265 706f 7274 5f63 6174 6567 6f72  ``report_categor
-00012360: 795f 6964 6060 2069 7320 7265 7175 6972  y_id`` is requir
-00012370: 6564 2069 6e20 7468 6520 6060 5748 4552  ed in the ``WHER
-00012380: 4560 6020 636c 6175 7365 2e0a 0a20 2020  E`` clause...   
-00012390: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
-000123a0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
-000123b0: 6f66 2060 6f6e 656f 6660 5f20 6060 5f72  of `oneof`_ ``_r
-000123c0: 6570 6f72 745f 6361 7465 676f 7279 5f69  eport_category_i
-000123d0: 6460 602e 0a20 2020 2020 2020 2074 7261  d``..        tra
-000123e0: 6666 6963 5f73 6f75 7263 6520 2867 6f6f  ffic_source (goo
-000123f0: 676c 652e 7368 6f70 7069 6e67 2e6d 6572  gle.shopping.mer
-00012400: 6368 616e 745f 7265 706f 7274 735f 7631  chant_reports_v1
-00012410: 6265 7461 2e74 7970 6573 2e54 7261 6666  beta.types.Traff
-00012420: 6963 536f 7572 6365 2e54 7261 6666 6963  icSource.Traffic
-00012430: 536f 7572 6365 456e 756d 293a 0a20 2020  SourceEnum):.   
-00012440: 2020 2020 2020 2020 2054 7261 6666 6963           Traffic
-00012450: 2073 6f75 7263 6520 6f66 2069 6d70 7265   source of impre
-00012460: 7373 696f 6e73 2e0a 0a20 2020 2020 2020  ssions...       
-00012470: 2020 2020 2052 6571 7569 7265 6420 696e       Required in
-00012480: 2074 6865 2060 6053 454c 4543 5460 6020   the ``SELECT`` 
-00012490: 636c 6175 7365 2e0a 0a20 2020 2020 2020  clause...       
-000124a0: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
-000124b0: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
-000124c0: 6f6e 656f 6660 5f20 6060 5f74 7261 6666  oneof`_ ``_traff
-000124d0: 6963 5f73 6f75 7263 6560 602e 0a20 2020  ic_source``..   
-000124e0: 2020 2020 2072 616e 6b20 2869 6e74 293a       rank (int):
-000124f0: 0a20 2020 2020 2020 2020 2020 2050 6f73  .            Pos
-00012500: 6974 696f 6e20 6f66 2074 6865 2064 6f6d  ition of the dom
-00012510: 6169 6e20 696e 2074 6865 2074 6f70 206d  ain in the top m
-00012520: 6572 6368 616e 7473 2072 616e 6b69 6e67  erchants ranking
-00012530: 2066 6f72 2074 6865 0a20 2020 2020 2020   for the.       
-00012540: 2020 2020 2073 656c 6563 7465 6420 6b65       selected ke
-00012550: 7973 2028 6060 6461 7465 6060 2c20 6060  ys (``date``, ``
-00012560: 7265 706f 7274 5f63 6174 6567 6f72 795f  report_category_
-00012570: 6964 6060 2c0a 2020 2020 2020 2020 2020  id``,.          
-00012580: 2020 6060 7265 706f 7274 5f63 6f75 6e74    ``report_count
-00012590: 7279 5f63 6f64 6560 602c 2060 6074 7261  ry_code``, ``tra
-000125a0: 6666 6963 5f73 6f75 7263 6560 6029 2062  ffic_source``) b
-000125b0: 6173 6564 206f 6e0a 2020 2020 2020 2020  ased on.        
-000125c0: 2020 2020 696d 7072 6573 7369 6f6e 732e      impressions.
-000125d0: 2031 2069 7320 7468 6520 6869 6768 6573   1 is the highes
-000125e0: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
-000125f0: 4361 6e6e 6f74 2062 6520 6669 6c74 6572  Cannot be filter
-00012600: 6564 206f 6e20 696e 2074 6865 2027 5748  ed on in the 'WH
-00012610: 4552 4527 2063 6c61 7573 652e 0a0a 2020  ERE' clause...  
-00012620: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00012630: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-00012640: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-00012650: 7261 6e6b 6060 2e0a 2020 2020 2020 2020  rank``..        
-00012660: 6164 735f 6f72 6761 6e69 635f 7261 7469  ads_organic_rati
-00012670: 6f20 2866 6c6f 6174 293a 0a20 2020 2020  o (float):.     
-00012680: 2020 2020 2020 205b 4164 7320 2f20 6f72         [Ads / or
-00012690: 6761 6e69 6320 7261 7469 6f5d 0a20 2020  ganic ratio].   
-000126a0: 2020 2020 2020 2020 2028 6874 7470 733a           (https:
-000126b0: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
-000126c0: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
-000126d0: 6e73 7765 722f 3131 3336 3634 3432 237a  nswer/11366442#z
-000126e0: 6970 7079 3d25 3243 6164 732d 6672 6565  ippy=%2Cads-free
-000126f0: 2d72 6174 696f 290a 2020 2020 2020 2020  -ratio).        
-00012700: 2020 2020 7368 6f77 7320 686f 7720 6f66      shows how of
-00012710: 7465 6e20 7468 6520 646f 6d61 696e 2072  ten the domain r
-00012720: 6563 6569 7665 7320 696d 7072 6573 7369  eceives impressi
-00012730: 6f6e 7320 6672 6f6d 0a20 2020 2020 2020  ons from.       
-00012740: 2020 2020 2053 686f 7070 696e 6720 6164       Shopping ad
-00012750: 7320 636f 6d70 6172 6564 2074 6f20 6f72  s compared to or
-00012760: 6761 6e69 6320 7472 6166 6669 632e 2054  ganic traffic. T
-00012770: 6865 206e 756d 6265 7220 6973 0a20 2020  he number is.   
-00012780: 2020 2020 2020 2020 2072 6f75 6e64 6564           rounded
-00012790: 2061 6e64 2062 7563 6b65 7465 642e 0a0a   and bucketed...
-000127a0: 2020 2020 2020 2020 2020 2020 4361 6e6e              Cann
-000127b0: 6f74 2062 6520 6669 6c74 6572 6564 206f  ot be filtered o
-000127c0: 6e20 696e 2074 6865 2027 5748 4552 4527  n in the 'WHERE'
-000127d0: 2063 6c61 7573 652e 0a0a 2020 2020 2020   clause...      
-000127e0: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
-000127f0: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
-00012800: 606f 6e65 6f66 605f 2060 605f 6164 735f  `oneof`_ ``_ads_
-00012810: 6f72 6761 6e69 635f 7261 7469 6f60 602e  organic_ratio``.
-00012820: 0a20 2020 2020 2020 2070 6167 655f 6f76  .        page_ov
-00012830: 6572 6c61 705f 7261 7465 2028 666c 6f61  erlap_rate (floa
-00012840: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00012850: 5b50 6167 6520 6f76 6572 6c61 7020 7261  [Page overlap ra
-00012860: 7465 5d0a 2020 2020 2020 2020 2020 2020  te].            
-00012870: 2868 7474 7073 3a2f 2f73 7570 706f 7274  (https://support
-00012880: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
-00012890: 6861 6e74 732f 616e 7377 6572 2f31 3133  hants/answer/113
-000128a0: 3636 3434 3223 7a69 7070 793d 2532 4370  66442#zippy=%2Cp
-000128b0: 6167 652d 6f76 6572 6c61 702d 7261 7465  age-overlap-rate
-000128c0: 290a 2020 2020 2020 2020 2020 2020 7368  ).            sh
-000128d0: 6f77 7320 686f 7720 6672 6571 7565 6e74  ows how frequent
-000128e0: 6c79 2063 6f6d 7065 7469 6e67 2072 6574  ly competing ret
-000128f0: 6169 6c65 7273 e280 9920 6f66 6665 7273  ailers... offers
-00012900: 2061 7265 2073 686f 776e 0a20 2020 2020   are shown.     
-00012910: 2020 2020 2020 2074 6f67 6574 6865 7220         together 
-00012920: 7769 7468 2079 6f75 7220 6f66 6665 7273  with your offers
-00012930: 206f 6e20 7468 6520 7361 6d65 2070 6167   on the same pag
-00012940: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
-00012950: 4361 6e6e 6f74 2062 6520 6669 6c74 6572  Cannot be filter
-00012960: 6564 206f 6e20 696e 2074 6865 2027 5748  ed on in the 'WH
-00012970: 4552 4527 2063 6c61 7573 652e 0a0a 2020  ERE' clause...  
-00012980: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00012990: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-000129a0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-000129b0: 7061 6765 5f6f 7665 726c 6170 5f72 6174  page_overlap_rat
-000129c0: 6560 602e 0a20 2020 2020 2020 2068 6967  e``..        hig
-000129d0: 6865 725f 706f 7369 7469 6f6e 5f72 6174  her_position_rat
-000129e0: 6520 2866 6c6f 6174 293a 0a20 2020 2020  e (float):.     
-000129f0: 2020 2020 2020 205b 4869 6768 6572 2070         [Higher p
-00012a00: 6f73 6974 696f 6e20 7261 7465 5d0a 2020  osition rate].  
-00012a10: 2020 2020 2020 2020 2020 2868 7474 7073            (https
-00012a20: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
-00012a30: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
-00012a40: 616e 7377 6572 2f31 3133 3636 3434 3223  answer/11366442#
-00012a50: 7a69 7070 793d 2532 4368 6967 6865 722d  zippy=%2Chigher-
-00012a60: 706f 7369 7469 6f6e 2d72 6174 6529 0a20  position-rate). 
-00012a70: 2020 2020 2020 2020 2020 2073 686f 7773             shows
-00012a80: 2068 6f77 206f 6674 656e 2061 2063 6f6d   how often a com
-00012a90: 7065 7469 746f 72e2 8099 7320 6f66 6665  petitor...s offe
-00012aa0: 7220 676f 7420 706c 6163 6564 2069 6e20  r got placed in 
-00012ab0: 6120 6869 6768 6572 0a20 2020 2020 2020  a higher.       
-00012ac0: 2020 2020 2070 6f73 6974 696f 6e20 6f6e       position on
-00012ad0: 2074 6865 2070 6167 6520 7468 616e 2079   the page than y
-00012ae0: 6f75 7220 6f66 6665 722e 0a0a 2020 2020  our offer...    
-00012af0: 2020 2020 2020 2020 4361 6e6e 6f74 2062          Cannot b
-00012b00: 6520 6669 6c74 6572 6564 206f 6e20 696e  e filtered on in
-00012b10: 2074 6865 2027 5748 4552 4527 2063 6c61   the 'WHERE' cla
-00012b20: 7573 652e 0a0a 2020 2020 2020 2020 2020  use...          
-00012b30: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-00012b40: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00012b50: 6f66 605f 2060 605f 6869 6768 6572 5f70  of`_ ``_higher_p
-00012b60: 6f73 6974 696f 6e5f 7261 7465 6060 2e0a  osition_rate``..
-00012b70: 2020 2020 2222 220a 0a20 2020 2064 6174      """..    dat
-00012b80: 653a 2064 6174 655f 7062 322e 4461 7465  e: date_pb2.Date
-00012b90: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
-00012ba0: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
-00012bb0: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
-00012bc0: 756d 6265 723d 312c 0a20 2020 2020 2020  umber=1,.       
-00012bd0: 206d 6573 7361 6765 3d64 6174 655f 7062   message=date_pb
-00012be0: 322e 4461 7465 2c0a 2020 2020 290a 2020  2.Date,.    ).  
-00012bf0: 2020 646f 6d61 696e 3a20 7374 7220 3d20    domain: str = 
-00012c00: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
-00012c10: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
-00012c20: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
-00012c30: 723d 322c 0a20 2020 2020 2020 206f 7074  r=2,.        opt
-00012c40: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
-00012c50: 290a 2020 2020 6973 5f79 6f75 725f 646f  ).    is_your_do
-00012c60: 6d61 696e 3a20 626f 6f6c 203d 2070 726f  main: bool = pro
-00012c70: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-00012c80: 2020 7072 6f74 6f2e 424f 4f4c 2c0a 2020    proto.BOOL,.  
-00012c90: 2020 2020 2020 6e75 6d62 6572 3d33 2c0a        number=3,.
-00012ca0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-00012cb0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-00012cc0: 2072 6570 6f72 745f 636f 756e 7472 795f   report_country_
-00012cd0: 636f 6465 3a20 7374 7220 3d20 7072 6f74  code: str = prot
-00012ce0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00012cf0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
-00012d00: 2020 2020 2020 206e 756d 6265 723d 342c         number=4,
-00012d10: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
-00012d20: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
-00012d30: 2020 7265 706f 7274 5f63 6174 6567 6f72    report_categor
-00012d40: 795f 6964 3a20 696e 7420 3d20 7072 6f74  y_id: int = prot
-00012d50: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
-00012d60: 2070 726f 746f 2e49 4e54 3634 2c0a 2020   proto.INT64,.  
-00012d70: 2020 2020 2020 6e75 6d62 6572 3d35 2c0a        number=5,.
-00012d80: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-00012d90: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
-00012da0: 2074 7261 6666 6963 5f73 6f75 7263 653a   traffic_source:
-00012db0: 2022 5472 6166 6669 6353 6f75 7263 652e   "TrafficSource.
-00012dc0: 5472 6166 6669 6353 6f75 7263 6545 6e75  TrafficSourceEnu
-00012dd0: 6d22 203d 2070 726f 746f 2e46 6965 6c64  m" = proto.Field
-00012de0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-00012df0: 454e 554d 2c0a 2020 2020 2020 2020 6e75  ENUM,.        nu
-00012e00: 6d62 6572 3d36 2c0a 2020 2020 2020 2020  mber=6,.        
-00012e10: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
-00012e20: 2020 2020 2020 2065 6e75 6d3d 2254 7261         enum="Tra
-00012e30: 6666 6963 536f 7572 6365 2e54 7261 6666  fficSource.Traff
-00012e40: 6963 536f 7572 6365 456e 756d 222c 0a20  icSourceEnum",. 
-00012e50: 2020 2029 0a20 2020 2072 616e 6b3a 2069     ).    rank: i
-00012e60: 6e74 203d 2070 726f 746f 2e46 6965 6c64  nt = proto.Field
-00012e70: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-00012e80: 494e 5436 342c 0a20 2020 2020 2020 206e  INT64,.        n
-00012e90: 756d 6265 723d 372c 0a20 2020 2020 2020  umber=7,.       
-00012ea0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-00012eb0: 2020 2020 290a 2020 2020 6164 735f 6f72      ).    ads_or
-00012ec0: 6761 6e69 635f 7261 7469 6f3a 2066 6c6f  ganic_ratio: flo
-00012ed0: 6174 203d 2070 726f 746f 2e46 6965 6c64  at = proto.Field
-00012ee0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
-00012ef0: 444f 5542 4c45 2c0a 2020 2020 2020 2020  DOUBLE,.        
-00012f00: 6e75 6d62 6572 3d38 2c0a 2020 2020 2020  number=8,.      
-00012f10: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
-00012f20: 0a20 2020 2029 0a20 2020 2070 6167 655f  .    ).    page_
-00012f30: 6f76 6572 6c61 705f 7261 7465 3a20 666c  overlap_rate: fl
-00012f40: 6f61 7420 3d20 7072 6f74 6f2e 4669 656c  oat = proto.Fiel
-00012f50: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
-00012f60: 2e44 4f55 424c 452c 0a20 2020 2020 2020  .DOUBLE,.       
-00012f70: 206e 756d 6265 723d 392c 0a20 2020 2020   number=9,.     
-00012f80: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
-00012f90: 2c0a 2020 2020 290a 2020 2020 6869 6768  ,.    ).    high
-00012fa0: 6572 5f70 6f73 6974 696f 6e5f 7261 7465  er_position_rate
-00012fb0: 3a20 666c 6f61 7420 3d20 7072 6f74 6f2e  : float = proto.
-00012fc0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00012fd0: 726f 746f 2e44 4f55 424c 452c 0a20 2020  roto.DOUBLE,.   
-00012fe0: 2020 2020 206e 756d 6265 723d 3130 2c0a       number=10,.
-00012ff0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-00013000: 3d54 7275 652c 0a20 2020 2029 0a0a 0a63  =True,.    )...c
-00013010: 6c61 7373 2043 6f6d 7065 7469 7469 7665  lass Competitive
-00013020: 5669 7369 6269 6c69 7479 4265 6e63 686d  VisibilityBenchm
-00013030: 6172 6b56 6965 7728 7072 6f74 6f2e 4d65  arkView(proto.Me
-00013040: 7373 6167 6529 3a0a 2020 2020 7222 2222  ssage):.    r"""
-00013050: 4669 656c 6473 2061 7661 696c 6162 6c65  Fields available
-00013060: 2066 6f72 2071 7565 7279 2069 6e0a 2020   for query in.  
-00013070: 2020 6060 636f 6d70 6574 6974 6976 655f    ``competitive_
-00013080: 7669 7369 6269 6c69 7479 5f62 656e 6368  visibility_bench
-00013090: 6d61 726b 5f76 6965 7760 6020 7461 626c  mark_view`` tabl
-000130a0: 652e 0a0a 2020 2020 6043 6f6d 7065 7469  e...    `Competi
-000130b0: 7469 7665 0a20 2020 2076 6973 6962 696c  tive.    visibil
-000130c0: 6974 7920 3c68 7474 7073 3a2f 2f73 7570  ity <https://sup
-000130d0: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
-000130e0: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
-000130f0: 2f31 3133 3636 3434 323e 605f 5f0a 2020  /11366442>`__.  
-00013100: 2020 7265 706f 7274 2077 6974 6820 7468    report with th
-00013110: 6520 6361 7465 676f 7279 2062 656e 6368  e category bench
-00013120: 6d61 726b 2e0a 0a20 2020 2056 616c 7565  mark...    Value
-00013130: 7320 6172 6520 6f6e 6c79 2073 6574 2066  s are only set f
-00013140: 6f72 2066 6965 6c64 7320 7265 7175 6573  or fields reques
-00013150: 7465 6420 6578 706c 6963 6974 6c79 2069  ted explicitly i
-00013160: 6e20 7468 6520 7265 7175 6573 7427 730a  n the request's.
-00013170: 2020 2020 7365 6172 6368 2071 7565 7279      search query
-00013180: 2e0a 0a0a 2020 2020 2e2e 205f 6f6e 656f  ....    .. _oneo
-00013190: 663a 2068 7474 7073 3a2f 2f70 726f 746f  f: https://proto
-000131a0: 2d70 6c75 732d 7079 7468 6f6e 2e72 6561  -plus-python.rea
-000131b0: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
-000131c0: 7461 626c 652f 6669 656c 6473 2e68 746d  table/fields.htm
-000131d0: 6c23 6f6e 656f 6673 2d6d 7574 7561 6c6c  l#oneofs-mutuall
-000131e0: 792d 6578 636c 7573 6976 652d 6669 656c  y-exclusive-fiel
-000131f0: 6473 0a0a 2020 2020 4174 7472 6962 7574  ds..    Attribut
-00013200: 6573 3a0a 2020 2020 2020 2020 6461 7465  es:.        date
-00013210: 2028 676f 6f67 6c65 2e74 7970 652e 6461   (google.type.da
-00013220: 7465 5f70 6232 2e44 6174 6529 3a0a 2020  te_pb2.Date):.  
-00013230: 2020 2020 2020 2020 2020 4461 7465 206f            Date o
-00013240: 6620 7468 6973 2072 6f77 2e0a 0a20 2020  f this row...   
-00013250: 2020 2020 2020 2020 2052 6571 7569 7265           Require
-00013260: 6420 696e 2074 6865 2060 6053 454c 4543  d in the ``SELEC
-00013270: 5460 6020 636c 6175 7365 2e20 4120 636f  T`` clause. A co
-00013280: 6e64 6974 696f 6e20 6f6e 2060 6064 6174  ndition on ``dat
-00013290: 6560 600a 2020 2020 2020 2020 2020 2020  e``.            
-000132a0: 6973 2072 6571 7569 7265 6420 696e 2074  is required in t
-000132b0: 6865 2060 6057 4845 5245 6060 2063 6c61  he ``WHERE`` cla
-000132c0: 7573 652e 0a20 2020 2020 2020 2072 6570  use..        rep
-000132d0: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
-000132e0: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
-000132f0: 2020 2020 436f 756e 7472 7920 7768 6572      Country wher
-00013300: 6520 696d 7072 6573 7369 6f6e 7320 6170  e impressions ap
-00013310: 7065 6172 6564 2e0a 0a20 2020 2020 2020  peared...       
-00013320: 2020 2020 2052 6571 7569 7265 6420 696e       Required in
-00013330: 2074 6865 2060 6053 454c 4543 5460 6020   the ``SELECT`` 
-00013340: 636c 6175 7365 2e20 4120 636f 6e64 6974  clause. A condit
-00013350: 696f 6e20 6f6e 0a20 2020 2020 2020 2020  ion on.         
-00013360: 2020 2060 6072 6570 6f72 745f 636f 756e     ``report_coun
-00013370: 7472 795f 636f 6465 6060 2069 7320 7265  try_code`` is re
-00013380: 7175 6972 6564 2069 6e20 7468 6520 6060  quired in the ``
-00013390: 5748 4552 4560 6020 636c 6175 7365 2e0a  WHERE`` clause..
-000133a0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-000133b0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
-000133c0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
-000133d0: 6060 5f72 6570 6f72 745f 636f 756e 7472  ``_report_countr
-000133e0: 795f 636f 6465 6060 2e0a 2020 2020 2020  y_code``..      
-000133f0: 2020 7265 706f 7274 5f63 6174 6567 6f72    report_categor
-00013400: 795f 6964 2028 696e 7429 3a0a 2020 2020  y_id (int):.    
-00013410: 2020 2020 2020 2020 476f 6f67 6c65 2070          Google p
-00013420: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
-00013430: 4944 2074 6f20 6361 6c63 756c 6174 6520  ID to calculate 
-00013440: 7468 6520 7265 706f 7274 2066 6f72 2c0a  the report for,.
-00013450: 2020 2020 2020 2020 2020 2020 7265 7072              repr
-00013460: 6573 656e 7465 6420 696e 2060 476f 6f67  esented in `Goog
-00013470: 6c65 2773 2070 726f 6475 6374 0a20 2020  le's product.   
-00013480: 2020 2020 2020 2020 2074 6178 6f6e 6f6d           taxonom
-00013490: 7920 3c68 7474 7073 3a2f 2f73 7570 706f  y <https://suppo
-000134a0: 7274 2e67 6f6f 676c 652e 636f 6d2f 6d65  rt.google.com/me
-000134b0: 7263 6861 6e74 732f 616e 7377 6572 2f36  rchants/answer/6
-000134c0: 3332 3434 3336 3e60 5f5f 2e0a 0a20 2020  324436>`__...   
-000134d0: 2020 2020 2020 2020 2052 6571 7569 7265           Require
-000134e0: 6420 696e 2074 6865 2060 6053 454c 4543  d in the ``SELEC
-000134f0: 5460 6020 636c 6175 7365 2e20 4120 636f  T`` clause. A co
-00013500: 6e64 6974 696f 6e20 6f6e 0a20 2020 2020  ndition on.     
-00013510: 2020 2020 2020 2060 6072 6570 6f72 745f         ``report_
-00013520: 6361 7465 676f 7279 5f69 6460 6020 6973  category_id`` is
-00013530: 2072 6571 7569 7265 6420 696e 2074 6865   required in the
-00013540: 2060 6057 4845 5245 6060 2063 6c61 7573   ``WHERE`` claus
-00013550: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
-00013560: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
-00013570: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
-00013580: 605f 2060 605f 7265 706f 7274 5f63 6174  `_ ``_report_cat
-00013590: 6567 6f72 795f 6964 6060 2e0a 2020 2020  egory_id``..    
-000135a0: 2020 2020 7472 6166 6669 635f 736f 7572      traffic_sour
-000135b0: 6365 2028 676f 6f67 6c65 2e73 686f 7070  ce (google.shopp
-000135c0: 696e 672e 6d65 7263 6861 6e74 5f72 6570  ing.merchant_rep
-000135d0: 6f72 7473 5f76 3162 6574 612e 7479 7065  orts_v1beta.type
-000135e0: 732e 5472 6166 6669 6353 6f75 7263 652e  s.TrafficSource.
-000135f0: 5472 6166 6669 6353 6f75 7263 6545 6e75  TrafficSourceEnu
-00013600: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
-00013610: 5472 6166 6669 6320 736f 7572 6365 206f  Traffic source o
-00013620: 6620 696d 7072 6573 7369 6f6e 732e 0a0a  f impressions...
-00013630: 2020 2020 2020 2020 2020 2020 5265 7175              Requ
-00013640: 6972 6564 2069 6e20 7468 6520 6060 5345  ired in the ``SE
-00013650: 4c45 4354 6060 2063 6c61 7573 652e 0a0a  LECT`` clause...
-00013660: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00013670: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
-00013680: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
-00013690: 605f 7472 6166 6669 635f 736f 7572 6365  `_traffic_source
-000136a0: 6060 2e0a 2020 2020 2020 2020 796f 7572  ``..        your
-000136b0: 5f64 6f6d 6169 6e5f 7669 7369 6269 6c69  _domain_visibili
-000136c0: 7479 5f74 7265 6e64 2028 666c 6f61 7429  ty_trend (float)
-000136d0: 3a0a 2020 2020 2020 2020 2020 2020 4368  :.            Ch
-000136e0: 616e 6765 2069 6e20 7669 7369 6269 6c69  ange in visibili
-000136f0: 7479 2062 6173 6564 206f 6e20 696d 7072  ty based on impr
-00013700: 6573 7369 6f6e 7320 666f 720a 2020 2020  essions for.    
-00013710: 2020 2020 2020 2020 796f 7572 2064 6f6d          your dom
-00013720: 6169 6e20 7769 7468 2072 6573 7065 6374  ain with respect
-00013730: 2074 6f20 7468 6520 7374 6172 7420 6f66   to the start of
-00013740: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-00013750: 2073 656c 6563 7465 6420 7469 6d65 2072   selected time r
-00013760: 616e 6765 2028 6f72 2066 6972 7374 2064  ange (or first d
-00013770: 6179 2077 6974 6820 6e6f 6e2d 7a65 726f  ay with non-zero
-00013780: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
-00013790: 7265 7373 696f 6e73 292e 0a0a 2020 2020  ressions)...    
-000137a0: 2020 2020 2020 2020 4361 6e6e 6f74 2062          Cannot b
-000137b0: 6520 6669 6c74 6572 6564 206f 6e20 696e  e filtered on in
-000137c0: 2074 6865 2027 5748 4552 4527 2063 6c61   the 'WHERE' cla
-000137d0: 7573 652e 0a0a 2020 2020 2020 2020 2020  use...          
-000137e0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
-000137f0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
-00013800: 6f66 605f 2060 605f 796f 7572 5f64 6f6d  of`_ ``_your_dom
-00013810: 6169 6e5f 7669 7369 6269 6c69 7479 5f74  ain_visibility_t
-00013820: 7265 6e64 6060 2e0a 2020 2020 2020 2020  rend``..        
-00013830: 6361 7465 676f 7279 5f62 656e 6368 6d61  category_benchma
-00013840: 726b 5f76 6973 6962 696c 6974 795f 7472  rk_visibility_tr
-00013850: 656e 6420 2866 6c6f 6174 293a 0a20 2020  end (float):.   
-00013860: 2020 2020 2020 2020 2043 6861 6e67 6520           Change 
-00013870: 696e 2076 6973 6962 696c 6974 7920 6261  in visibility ba
-00013880: 7365 6420 6f6e 2069 6d70 7265 7373 696f  sed on impressio
-00013890: 6e73 0a20 2020 2020 2020 2020 2020 2077  ns.            w
-000138a0: 6974 6820 7265 7370 6563 7420 746f 2074  ith respect to t
-000138b0: 6865 2073 7461 7274 206f 6620 7468 6520  he start of the 
-000138c0: 7365 6c65 6374 6564 2074 696d 650a 2020  selected time.  
-000138d0: 2020 2020 2020 2020 2020 7261 6e67 6520            range 
-000138e0: 286f 7220 6669 7273 7420 6461 7920 7769  (or first day wi
-000138f0: 7468 206e 6f6e 2d7a 6572 6f20 696d 7072  th non-zero impr
-00013900: 6573 7369 6f6e 7329 0a20 2020 2020 2020  essions).       
-00013910: 2020 2020 2066 6f72 2061 2063 6f6d 6269       for a combi
-00013920: 6e65 6420 7365 7420 6f66 206d 6572 6368  ned set of merch
-00013930: 616e 7473 2077 6974 6820 6869 6768 6573  ants with highes
-00013940: 740a 2020 2020 2020 2020 2020 2020 7669  t.            vi
-00013950: 7369 6269 6c69 7479 2061 7070 726f 7869  sibility approxi
-00013960: 6d61 7469 6e67 2074 6865 206d 6172 6b65  mating the marke
-00013970: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
-00013980: 4361 6e6e 6f74 2062 6520 6669 6c74 6572  Cannot be filter
-00013990: 6564 206f 6e20 696e 2074 6865 2027 5748  ed on in the 'WH
-000139a0: 4552 4527 2063 6c61 7573 652e 0a0a 2020  ERE' clause...  
-000139b0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-000139c0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
-000139d0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
-000139e0: 6361 7465 676f 7279 5f62 656e 6368 6d61  category_benchma
-000139f0: 726b 5f76 6973 6962 696c 6974 795f 7472  rk_visibility_tr
-00013a00: 656e 6460 602e 0a20 2020 2022 2222 0a0a  end``..    """..
-00013a10: 2020 2020 6461 7465 3a20 6461 7465 5f70      date: date_p
-00013a20: 6232 2e44 6174 6520 3d20 7072 6f74 6f2e  b2.Date = proto.
-00013a30: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00013a40: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
-00013a50: 2020 2020 2020 6e75 6d62 6572 3d31 2c0a        number=1,.
-00013a60: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
-00013a70: 6461 7465 5f70 6232 2e44 6174 652c 0a20  date_pb2.Date,. 
-00013a80: 2020 2029 0a20 2020 2072 6570 6f72 745f     ).    report_
-00013a90: 636f 756e 7472 795f 636f 6465 3a20 7374  country_code: st
-00013aa0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
-00013ab0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
-00013ac0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
-00013ad0: 756d 6265 723d 322c 0a20 2020 2020 2020  umber=2,.       
-00013ae0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
-00013af0: 2020 2020 290a 2020 2020 7265 706f 7274      ).    report
-00013b00: 5f63 6174 6567 6f72 795f 6964 3a20 696e  _category_id: in
-00013b10: 7420 3d20 7072 6f74 6f2e 4669 656c 6428  t = proto.Field(
-00013b20: 0a20 2020 2020 2020 2070 726f 746f 2e49  .        proto.I
-00013b30: 4e54 3634 2c0a 2020 2020 2020 2020 6e75  NT64,.        nu
-00013b40: 6d62 6572 3d33 2c0a 2020 2020 2020 2020  mber=3,.        
-00013b50: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
-00013b60: 2020 2029 0a20 2020 2074 7261 6666 6963     ).    traffic
-00013b70: 5f73 6f75 7263 653a 2022 5472 6166 6669  _source: "Traffi
-00013b80: 6353 6f75 7263 652e 5472 6166 6669 6353  cSource.TrafficS
-00013b90: 6f75 7263 6545 6e75 6d22 203d 2070 726f  ourceEnum" = pro
-00013ba0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
-00013bb0: 2020 7072 6f74 6f2e 454e 554d 2c0a 2020    proto.ENUM,.  
-00013bc0: 2020 2020 2020 6e75 6d62 6572 3d34 2c0a        number=4,.
-00013bd0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
-00013be0: 3d54 7275 652c 0a20 2020 2020 2020 2065  =True,.        e
-00013bf0: 6e75 6d3d 2254 7261 6666 6963 536f 7572  num="TrafficSour
-00013c00: 6365 2e54 7261 6666 6963 536f 7572 6365  ce.TrafficSource
-00013c10: 456e 756d 222c 0a20 2020 2029 0a20 2020  Enum",.    ).   
-00013c20: 2079 6f75 725f 646f 6d61 696e 5f76 6973   your_domain_vis
-00013c30: 6962 696c 6974 795f 7472 656e 643a 2066  ibility_trend: f
-00013c40: 6c6f 6174 203d 2070 726f 746f 2e46 6965  loat = proto.Fie
-00013c50: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
-00013c60: 6f2e 444f 5542 4c45 2c0a 2020 2020 2020  o.DOUBLE,.      
-00013c70: 2020 6e75 6d62 6572 3d35 2c0a 2020 2020    number=5,.    
-00013c80: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
-00013c90: 652c 0a20 2020 2029 0a20 2020 2063 6174  e,.    ).    cat
-00013ca0: 6567 6f72 795f 6265 6e63 686d 6172 6b5f  egory_benchmark_
-00013cb0: 7669 7369 6269 6c69 7479 5f74 7265 6e64  visibility_trend
-00013cc0: 3a20 666c 6f61 7420 3d20 7072 6f74 6f2e  : float = proto.
-00013cd0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
-00013ce0: 726f 746f 2e44 4f55 424c 452c 0a20 2020  roto.DOUBLE,.   
-00013cf0: 2020 2020 206e 756d 6265 723d 362c 0a20       number=6,. 
-00013d00: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
-00013d10: 5472 7565 2c0a 2020 2020 290a 0a0a 636c  True,.    )...cl
-00013d20: 6173 7320 4d61 726b 6574 696e 674d 6574  ass MarketingMet
-00013d30: 686f 6428 7072 6f74 6f2e 4d65 7373 6167  hod(proto.Messag
-00013d40: 6529 3a0a 2020 2020 7222 2222 4d61 726b  e):.    r"""Mark
-00013d50: 6574 696e 6720 6d65 7468 6f64 2075 7365  eting method use
-00013d60: 6420 746f 2070 726f 6d6f 7465 2079 6f75  d to promote you
-00013d70: 7220 7072 6f64 7563 7473 206f 6e20 476f  r products on Go
-00013d80: 6f67 6c65 0a20 2020 2028 6f72 6761 6e69  ogle.    (organi
-00013d90: 6320 7665 7273 7573 2061 6473 292e 0a0a  c versus ads)...
-00013da0: 2020 2020 2222 220a 0a20 2020 2063 6c61      """..    cla
-00013db0: 7373 204d 6172 6b65 7469 6e67 4d65 7468  ss MarketingMeth
-00013dc0: 6f64 456e 756d 2870 726f 746f 2e45 6e75  odEnum(proto.Enu
-00013dd0: 6d29 3a0a 2020 2020 2020 2020 7222 2222  m):.        r"""
-00013de0: 4d61 726b 6574 696e 6720 6d65 7468 6f64  Marketing method
-00013df0: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
-00013e00: 2020 5661 6c75 6573 3a0a 2020 2020 2020    Values:.      
-00013e10: 2020 2020 2020 4d41 524b 4554 494e 475f        MARKETING_
-00013e20: 4d45 5448 4f44 5f45 4e55 4d5f 554e 5350  METHOD_ENUM_UNSP
-00013e30: 4543 4946 4945 4420 2830 293a 0a20 2020  ECIFIED (0):.   
-00013e40: 2020 2020 2020 2020 2020 2020 204e 6f74               Not
-00013e50: 2073 7065 6369 6669 6564 2e0a 2020 2020   specified..    
-00013e60: 2020 2020 2020 2020 4f52 4741 4e49 4320          ORGANIC 
-00013e70: 2831 293a 0a20 2020 2020 2020 2020 2020  (1):.           
-00013e80: 2020 2020 204f 7267 616e 6963 206d 6172       Organic mar
-00013e90: 6b65 7469 6e67 2e0a 2020 2020 2020 2020  keting..        
-00013ea0: 2020 2020 4144 5320 2832 293a 0a20 2020      ADS (2):.   
-00013eb0: 2020 2020 2020 2020 2020 2020 2041 6473               Ads
-00013ec0: 2d62 6173 6564 206d 6172 6b65 7469 6e67  -based marketing
-00013ed0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00013ee0: 2020 2020 2020 4d41 524b 4554 494e 475f        MARKETING_
-00013ef0: 4d45 5448 4f44 5f45 4e55 4d5f 554e 5350  METHOD_ENUM_UNSP
-00013f00: 4543 4946 4945 4420 3d20 300a 2020 2020  ECIFIED = 0.    
-00013f10: 2020 2020 4f52 4741 4e49 4320 3d20 310a      ORGANIC = 1.
-00013f20: 2020 2020 2020 2020 4144 5320 3d20 320a          ADS = 2.
-00013f30: 0a0a 636c 6173 7320 5265 706f 7274 4772  ..class ReportGr
-00013f40: 616e 756c 6172 6974 7928 7072 6f74 6f2e  anularity(proto.
-00013f50: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
-00013f60: 2222 4772 616e 756c 6172 6974 7920 6f66  ""Granularity of
-00013f70: 2074 6865 2042 6573 7420 7365 6c6c 6572   the Best seller
-00013f80: 7320 7265 706f 7274 2e20 4265 7374 2073  s report. Best s
-00013f90: 656c 6c65 7273 2072 6570 6f72 7473 0a20  ellers reports. 
-00013fa0: 2020 2061 7265 2063 6f6d 7075 7465 6420     are computed 
-00013fb0: 6f76 6572 2061 2077 6565 6b20 616e 6420  over a week and 
-00013fc0: 6120 6d6f 6e74 6820 7469 6d65 6672 616d  a month timefram
-00013fd0: 652e 0a0a 2020 2020 2222 220a 0a20 2020  e...    """..   
-00013fe0: 2063 6c61 7373 2052 6570 6f72 7447 7261   class ReportGra
-00013ff0: 6e75 6c61 7269 7479 456e 756d 2870 726f  nularityEnum(pro
-00014000: 746f 2e45 6e75 6d29 3a0a 2020 2020 2020  to.Enum):.      
-00014010: 2020 7222 2222 5265 706f 7274 2067 7261    r"""Report gra
-00014020: 6e75 6c61 7269 7479 2076 616c 7565 732e  nularity values.
-00014030: 0a0a 2020 2020 2020 2020 5661 6c75 6573  ..        Values
-00014040: 3a0a 2020 2020 2020 2020 2020 2020 5245  :.            RE
-00014050: 504f 5254 5f47 5241 4e55 4c41 5249 5459  PORT_GRANULARITY
-00014060: 5f45 4e55 4d5f 554e 5350 4543 4946 4945  _ENUM_UNSPECIFIE
-00014070: 4420 2830 293a 0a20 2020 2020 2020 2020  D (0):.         
-00014080: 2020 2020 2020 204e 6f74 2073 7065 6369         Not speci
-00014090: 6669 6564 2e0a 2020 2020 2020 2020 2020  fied..          
-000140a0: 2020 5745 454b 4c59 2028 3129 3a0a 2020    WEEKLY (1):.  
-000140b0: 2020 2020 2020 2020 2020 2020 2020 5265                Re
-000140c0: 706f 7274 2069 7320 636f 6d70 7574 6564  port is computed
-000140d0: 206f 7665 7220 6120 7765 656b 2074 696d   over a week tim
-000140e0: 6566 7261 6d65 2e0a 2020 2020 2020 2020  eframe..        
-000140f0: 2020 2020 4d4f 4e54 484c 5920 2832 293a      MONTHLY (2):
-00014100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014110: 2052 6570 6f72 7420 6973 2063 6f6d 7075   Report is compu
-00014120: 7465 6420 6f76 6572 2061 206d 6f6e 7468  ted over a month
-00014130: 2074 696d 6566 7261 6d65 2e0a 2020 2020   timeframe..    
-00014140: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00014150: 5245 504f 5254 5f47 5241 4e55 4c41 5249  REPORT_GRANULARI
-00014160: 5459 5f45 4e55 4d5f 554e 5350 4543 4946  TY_ENUM_UNSPECIF
-00014170: 4945 4420 3d20 300a 2020 2020 2020 2020  IED = 0.        
-00014180: 5745 454b 4c59 203d 2031 0a20 2020 2020  WEEKLY = 1.     
-00014190: 2020 204d 4f4e 5448 4c59 203d 2032 0a0a     MONTHLY = 2..
-000141a0: 0a63 6c61 7373 2052 656c 6174 6976 6544  .class RelativeD
-000141b0: 656d 616e 6428 7072 6f74 6f2e 4d65 7373  emand(proto.Mess
-000141c0: 6167 6529 3a0a 2020 2020 7222 2222 5265  age):.    r"""Re
-000141d0: 6c61 7469 7665 2064 656d 616e 6420 6f66  lative demand of
-000141e0: 2061 2070 726f 6475 6374 2063 6c75 7374   a product clust
-000141f0: 6572 206f 7220 6272 616e 6420 696e 2074  er or brand in t
-00014200: 6865 2042 6573 740a 2020 2020 7365 6c6c  he Best.    sell
-00014210: 6572 7320 7265 706f 7274 2e0a 0a20 2020  ers report...   
-00014220: 2022 2222 0a0a 2020 2020 636c 6173 7320   """..    class 
-00014230: 5265 6c61 7469 7665 4465 6d61 6e64 456e  RelativeDemandEn
-00014240: 756d 2870 726f 746f 2e45 6e75 6d29 3a0a  um(proto.Enum):.
-00014250: 2020 2020 2020 2020 7222 2222 5265 6c61          r"""Rela
-00014260: 7469 7665 2064 656d 616e 6420 7661 6c75  tive demand valu
-00014270: 6573 2e0a 0a20 2020 2020 2020 2056 616c  es...        Val
-00014280: 7565 733a 0a20 2020 2020 2020 2020 2020  ues:.           
-00014290: 2052 454c 4154 4956 455f 4445 4d41 4e44   RELATIVE_DEMAND
-000142a0: 5f45 4e55 4d5f 554e 5350 4543 4946 4945  _ENUM_UNSPECIFIE
-000142b0: 4420 2830 293a 0a20 2020 2020 2020 2020  D (0):.         
-000142c0: 2020 2020 2020 204e 6f74 2073 7065 6369         Not speci
-000142d0: 6669 6564 2e0a 2020 2020 2020 2020 2020  fied..          
-000142e0: 2020 5645 5259 5f4c 4f57 2028 3130 293a    VERY_LOW (10):
-000142f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014300: 2044 656d 616e 6420 6973 2030 2d35 2520   Demand is 0-5% 
-00014310: 6f66 2074 6865 2064 656d 616e 6420 6f66  of the demand of
-00014320: 2074 6865 2068 6967 6865 7374 0a20 2020   the highest.   
-00014330: 2020 2020 2020 2020 2020 2020 2072 616e               ran
-00014340: 6b65 6420 7072 6f64 7563 7420 636c 7573  ked product clus
-00014350: 7465 7220 6f72 2062 7261 6e64 2e0a 2020  ter or brand..  
-00014360: 2020 2020 2020 2020 2020 4c4f 5720 2832            LOW (2
-00014370: 3029 3a0a 2020 2020 2020 2020 2020 2020  0):.            
-00014380: 2020 2020 4465 6d61 6e64 2069 7320 362d      Demand is 6-
-00014390: 3130 2520 6f66 2074 6865 2064 656d 616e  10% of the deman
-000143a0: 6420 6f66 2074 6865 2068 6967 6865 7374  d of the highest
-000143b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000143c0: 2072 616e 6b65 6420 7072 6f64 7563 7420   ranked product 
-000143d0: 636c 7573 7465 7220 6f72 2062 7261 6e64  cluster or brand
-000143e0: 2e0a 2020 2020 2020 2020 2020 2020 4d45  ..            ME
-000143f0: 4449 554d 2028 3330 293a 0a20 2020 2020  DIUM (30):.     
-00014400: 2020 2020 2020 2020 2020 2044 656d 616e             Deman
-00014410: 6420 6973 2031 312d 3230 2520 6f66 2074  d is 11-20% of t
-00014420: 6865 2064 656d 616e 6420 6f66 2074 6865  he demand of the
-00014430: 2068 6967 6865 7374 0a20 2020 2020 2020   highest.       
-00014440: 2020 2020 2020 2020 2072 616e 6b65 6420           ranked 
-00014450: 7072 6f64 7563 7420 636c 7573 7465 7220  product cluster 
-00014460: 6f72 2062 7261 6e64 2e0a 2020 2020 2020  or brand..      
-00014470: 2020 2020 2020 4849 4748 2028 3430 293a        HIGH (40):
-00014480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014490: 2044 656d 616e 6420 6973 2032 312d 3530   Demand is 21-50
-000144a0: 2520 6f66 2074 6865 2064 656d 616e 6420  % of the demand 
-000144b0: 6f66 2074 6865 2068 6967 6865 7374 0a20  of the highest. 
-000144c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000144d0: 616e 6b65 6420 7072 6f64 7563 7420 636c  anked product cl
-000144e0: 7573 7465 7220 6f72 2062 7261 6e64 2e0a  uster or brand..
-000144f0: 2020 2020 2020 2020 2020 2020 5645 5259              VERY
-00014500: 5f48 4947 4820 2835 3029 3a0a 2020 2020  _HIGH (50):.    
-00014510: 2020 2020 2020 2020 2020 2020 4465 6d61              Dema
-00014520: 6e64 2069 7320 3531 2d31 3030 2520 6f66  nd is 51-100% of
-00014530: 2074 6865 2064 656d 616e 6420 6f66 2074   the demand of t
-00014540: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
-00014550: 2020 2068 6967 6865 7374 2072 616e 6b65     highest ranke
-00014560: 6420 7072 6f64 7563 7420 636c 7573 7465  d product cluste
-00014570: 7220 6f72 2062 7261 6e64 2e0a 2020 2020  r or brand..    
-00014580: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00014590: 5245 4c41 5449 5645 5f44 454d 414e 445f  RELATIVE_DEMAND_
-000145a0: 454e 554d 5f55 4e53 5045 4349 4649 4544  ENUM_UNSPECIFIED
-000145b0: 203d 2030 0a20 2020 2020 2020 2056 4552   = 0.        VER
-000145c0: 595f 4c4f 5720 3d20 3130 0a20 2020 2020  Y_LOW = 10.     
-000145d0: 2020 204c 4f57 203d 2032 300a 2020 2020     LOW = 20.    
-000145e0: 2020 2020 4d45 4449 554d 203d 2033 300a      MEDIUM = 30.
-000145f0: 2020 2020 2020 2020 4849 4748 203d 2034          HIGH = 4
-00014600: 300a 2020 2020 2020 2020 5645 5259 5f48  0.        VERY_H
-00014610: 4947 4820 3d20 3530 0a0a 0a63 6c61 7373  IGH = 50...class
-00014620: 2052 656c 6174 6976 6544 656d 616e 6443   RelativeDemandC
-00014630: 6861 6e67 6554 7970 6528 7072 6f74 6f2e  hangeType(proto.
-00014640: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
-00014650: 2222 5265 6c61 7469 7665 2064 656d 616e  ""Relative deman
-00014660: 6420 6f66 2061 2070 726f 6475 6374 2063  d of a product c
-00014670: 6c75 7374 6572 206f 7220 6272 616e 6420  luster or brand 
-00014680: 696e 2074 6865 2042 6573 740a 2020 2020  in the Best.    
-00014690: 7365 6c6c 6572 7320 7265 706f 7274 2063  sellers report c
-000146a0: 6f6d 7061 7265 6420 746f 2074 6865 2070  ompared to the p
-000146b0: 7265 7669 6f75 7320 7469 6d65 2070 6572  revious time per
-000146c0: 696f 642e 0a0a 2020 2020 2222 220a 0a20  iod...    """.. 
-000146d0: 2020 2063 6c61 7373 2052 656c 6174 6976     class Relativ
-000146e0: 6544 656d 616e 6443 6861 6e67 6554 7970  eDemandChangeTyp
-000146f0: 6545 6e75 6d28 7072 6f74 6f2e 456e 756d  eEnum(proto.Enum
-00014700: 293a 0a20 2020 2020 2020 2072 2222 2252  ):.        r"""R
-00014710: 656c 6174 6976 6520 6465 6d61 6e64 2063  elative demand c
-00014720: 6861 6e67 6520 7479 7065 2076 616c 7565  hange type value
-00014730: 732e 0a0a 2020 2020 2020 2020 5661 6c75  s...        Valu
-00014740: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00014750: 5245 4c41 5449 5645 5f44 454d 414e 445f  RELATIVE_DEMAND_
-00014760: 4348 414e 4745 5f54 5950 455f 454e 554d  CHANGE_TYPE_ENUM
-00014770: 5f55 4e53 5045 4349 4649 4544 2028 3029  _UNSPECIFIED (0)
-00014780: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014790: 2020 4e6f 7420 7370 6563 6966 6965 642e    Not specified.
-000147a0: 0a20 2020 2020 2020 2020 2020 2053 494e  .            SIN
-000147b0: 4b45 5220 2831 293a 0a20 2020 2020 2020  KER (1):.       
-000147c0: 2020 2020 2020 2020 2052 656c 6174 6976           Relativ
-000147d0: 6520 6465 6d61 6e64 2069 7320 6c6f 7765  e demand is lowe
-000147e0: 7220 7468 616e 2074 6865 2070 7265 7669  r than the previ
-000147f0: 6f75 730a 2020 2020 2020 2020 2020 2020  ous.            
-00014800: 2020 2020 7469 6d65 2070 6572 696f 642e      time period.
-00014810: 0a20 2020 2020 2020 2020 2020 2046 4c41  .            FLA
-00014820: 5420 2832 293a 0a20 2020 2020 2020 2020  T (2):.         
-00014830: 2020 2020 2020 2052 656c 6174 6976 6520         Relative 
-00014840: 6465 6d61 6e64 2069 7320 6571 7561 6c20  demand is equal 
-00014850: 746f 2074 6865 2070 7265 7669 6f75 7320  to the previous 
-00014860: 7469 6d65 0a20 2020 2020 2020 2020 2020  time.           
-00014870: 2020 2020 2070 6572 696f 642e 0a20 2020       period..   
-00014880: 2020 2020 2020 2020 2052 4953 4552 2028           RISER (
-00014890: 3329 3a0a 2020 2020 2020 2020 2020 2020  3):.            
-000148a0: 2020 2020 5265 6c61 7469 7665 2064 656d      Relative dem
-000148b0: 616e 6420 6973 2068 6967 6865 7220 7468  and is higher th
-000148c0: 616e 2074 6865 2070 7265 7669 6f75 730a  an the previous.
-000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148e0: 7469 6d65 2070 6572 696f 642e 0a20 2020  time period..   
-000148f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00014900: 2052 454c 4154 4956 455f 4445 4d41 4e44   RELATIVE_DEMAND
-00014910: 5f43 4841 4e47 455f 5459 5045 5f45 4e55  _CHANGE_TYPE_ENU
-00014920: 4d5f 554e 5350 4543 4946 4945 4420 3d20  M_UNSPECIFIED = 
-00014930: 300a 2020 2020 2020 2020 5349 4e4b 4552  0.        SINKER
-00014940: 203d 2031 0a20 2020 2020 2020 2046 4c41   = 1.        FLA
-00014950: 5420 3d20 320a 2020 2020 2020 2020 5249  T = 2.        RI
-00014960: 5345 5220 3d20 330a 0a0a 636c 6173 7320  SER = 3...class 
-00014970: 5472 6166 6669 6353 6f75 7263 6528 7072  TrafficSource(pr
-00014980: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
-00014990: 2020 7222 2222 5472 6166 6669 6320 736f    r"""Traffic so
-000149a0: 7572 6365 206f 6620 696d 7072 6573 7369  urce of impressi
-000149b0: 6f6e 7320 696e 2074 6865 2043 6f6d 7065  ons in the Compe
-000149c0: 7469 7469 7665 2076 6973 6962 696c 6974  titive visibilit
-000149d0: 790a 2020 2020 7265 706f 7274 2e0a 0a20  y.    report... 
-000149e0: 2020 2022 2222 0a0a 2020 2020 636c 6173     """..    clas
-000149f0: 7320 5472 6166 6669 6353 6f75 7263 6545  s TrafficSourceE
-00014a00: 6e75 6d28 7072 6f74 6f2e 456e 756d 293a  num(proto.Enum):
-00014a10: 0a20 2020 2020 2020 2072 2222 2254 7261  .        r"""Tra
-00014a20: 6666 6963 2073 6f75 7263 6520 7661 6c75  ffic source valu
-00014a30: 6573 2e0a 0a20 2020 2020 2020 2056 616c  es...        Val
-00014a40: 7565 733a 0a20 2020 2020 2020 2020 2020  ues:.           
-00014a50: 2054 5241 4646 4943 5f53 4f55 5243 455f   TRAFFIC_SOURCE_
-00014a60: 454e 554d 5f55 4e53 5045 4349 4649 4544  ENUM_UNSPECIFIED
-00014a70: 2028 3029 3a0a 2020 2020 2020 2020 2020   (0):.          
-00014a80: 2020 2020 2020 4e6f 7420 7370 6563 6966        Not specif
-00014a90: 6965 642e 0a20 2020 2020 2020 2020 2020  ied..           
-00014aa0: 204f 5247 414e 4943 2028 3129 3a0a 2020   ORGANIC (1):.  
-00014ab0: 2020 2020 2020 2020 2020 2020 2020 4f72                Or
-00014ac0: 6761 6e69 6320 7472 6166 6669 632e 0a20  ganic traffic.. 
-00014ad0: 2020 2020 2020 2020 2020 2041 4453 2028             ADS (
-00014ae0: 3229 3a0a 2020 2020 2020 2020 2020 2020  2):.            
-00014af0: 2020 2020 5472 6166 6669 6320 6672 6f6d      Traffic from
-00014b00: 2061 6473 2e0a 2020 2020 2020 2020 2020   ads..          
-00014b10: 2020 414c 4c20 2833 293a 0a20 2020 2020    ALL (3):.     
-00014b20: 2020 2020 2020 2020 2020 204f 7267 616e             Organ
-00014b30: 6963 2061 6e64 2061 6473 2074 7261 6666  ic and ads traff
-00014b40: 6963 2e0a 2020 2020 2020 2020 2222 220a  ic..        """.
-00014b50: 2020 2020 2020 2020 5452 4146 4649 435f          TRAFFIC_
-00014b60: 534f 5552 4345 5f45 4e55 4d5f 554e 5350  SOURCE_ENUM_UNSP
-00014b70: 4543 4946 4945 4420 3d20 300a 2020 2020  ECIFIED = 0.    
-00014b80: 2020 2020 4f52 4741 4e49 4320 3d20 310a      ORGANIC = 1.
-00014b90: 2020 2020 2020 2020 4144 5320 3d20 320a          ADS = 2.
-00014ba0: 2020 2020 2020 2020 414c 4c20 3d20 330a          ALL = 3.
-00014bb0: 0a0a 5f5f 616c 6c5f 5f20 3d20 7475 706c  ..__all__ = tupl
-00014bc0: 6528 736f 7274 6564 285f 5f70 726f 746f  e(sorted(__proto
-00014bd0: 6275 665f 5f2e 6d61 6e69 6665 7374 2929  buf__.manifest))
-00014be0: 0a                                       .
+000004e0: 2c0a 2020 2020 2020 2020 224e 6f6e 5072  ,.        "NonPr
+000004f0: 6f64 7563 7450 6572 666f 726d 616e 6365  oductPerformance
+00000500: 5669 6577 222c 0a20 2020 2020 2020 2022  View",.        "
+00000510: 436f 6d70 6574 6974 6976 6556 6973 6962  CompetitiveVisib
+00000520: 696c 6974 7943 6f6d 7065 7469 746f 7256  ilityCompetitorV
+00000530: 6965 7722 2c0a 2020 2020 2020 2020 2243  iew",.        "C
+00000540: 6f6d 7065 7469 7469 7665 5669 7369 6269  ompetitiveVisibi
+00000550: 6c69 7479 546f 704d 6572 6368 616e 7456  lityTopMerchantV
+00000560: 6965 7722 2c0a 2020 2020 2020 2020 2243  iew",.        "C
+00000570: 6f6d 7065 7469 7469 7665 5669 7369 6269  ompetitiveVisibi
+00000580: 6c69 7479 4265 6e63 686d 6172 6b56 6965  lityBenchmarkVie
+00000590: 7722 2c0a 2020 2020 2020 2020 224d 6172  w",.        "Mar
+000005a0: 6b65 7469 6e67 4d65 7468 6f64 222c 0a20  ketingMethod",. 
+000005b0: 2020 2020 2020 2022 5265 706f 7274 4772         "ReportGr
+000005c0: 616e 756c 6172 6974 7922 2c0a 2020 2020  anularity",.    
+000005d0: 2020 2020 2252 656c 6174 6976 6544 656d      "RelativeDem
+000005e0: 616e 6422 2c0a 2020 2020 2020 2020 2252  and",.        "R
+000005f0: 656c 6174 6976 6544 656d 616e 6443 6861  elativeDemandCha
+00000600: 6e67 6554 7970 6522 2c0a 2020 2020 2020  ngeType",.      
+00000610: 2020 2254 7261 6666 6963 536f 7572 6365    "TrafficSource
+00000620: 222c 0a20 2020 207d 2c0a 290a 0a0a 636c  ",.    },.)...cl
+00000630: 6173 7320 5365 6172 6368 5265 7175 6573  ass SearchReques
+00000640: 7428 7072 6f74 6f2e 4d65 7373 6167 6529  t(proto.Message)
+00000650: 3a0a 2020 2020 7222 2222 5265 7175 6573  :.    r"""Reques
+00000660: 7420 6d65 7373 6167 6520 666f 7220 7468  t message for th
+00000670: 6520 6060 5265 706f 7274 5365 7276 6963  e ``ReportServic
+00000680: 652e 5365 6172 6368 6060 206d 6574 686f  e.Search`` metho
+00000690: 642e 0a0a 2020 2020 4174 7472 6962 7574  d...    Attribut
+000006a0: 6573 3a0a 2020 2020 2020 2020 7061 7265  es:.        pare
+000006b0: 6e74 2028 7374 7229 3a0a 2020 2020 2020  nt (str):.      
+000006c0: 2020 2020 2020 5265 7175 6972 6564 2e20        Required. 
+000006d0: 4964 206f 6620 7468 6520 6163 636f 756e  Id of the accoun
+000006e0: 7420 6d61 6b69 6e67 2074 6865 2063 616c  t making the cal
+000006f0: 6c2e 0a20 2020 2020 2020 2020 2020 204d  l..            M
+00000700: 7573 7420 6265 2061 2073 7461 6e64 616c  ust be a standal
+00000710: 6f6e 6520 6163 636f 756e 7420 6f72 2061  one account or a
+00000720: 6e20 4d43 410a 2020 2020 2020 2020 2020  n MCA.          
+00000730: 2020 7375 6261 6363 6f75 6e74 2e20 466f    subaccount. Fo
+00000740: 726d 6174 3a20 6163 636f 756e 7473 2f7b  rmat: accounts/{
+00000750: 6163 636f 756e 747d 0a20 2020 2020 2020  account}.       
+00000760: 2071 7565 7279 2028 7374 7229 3a0a 2020   query (str):.  
+00000770: 2020 2020 2020 2020 2020 5265 7175 6972            Requir
+00000780: 6564 2e20 5175 6572 7920 7468 6174 2064  ed. Query that d
+00000790: 6566 696e 6573 2061 2072 6570 6f72 7420  efines a report 
+000007a0: 746f 2062 650a 2020 2020 2020 2020 2020  to be.          
+000007b0: 2020 7265 7472 6965 7665 642e 0a20 2020    retrieved..   
+000007c0: 2020 2020 2020 2020 2046 6f72 2064 6574           For det
+000007d0: 6169 6c73 206f 6e20 686f 7720 746f 2063  ails on how to c
+000007e0: 6f6e 7374 7275 6374 2079 6f75 7220 7175  onstruct your qu
+000007f0: 6572 792c 2073 6565 0a20 2020 2020 2020  ery, see.       
+00000800: 2020 2020 2074 6865 2051 7565 7279 204c       the Query L
+00000810: 616e 6775 6167 6520 6775 6964 652e 2046  anguage guide. F
+00000820: 6f72 2074 6865 2066 756c 6c20 6c69 7374  or the full list
+00000830: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
+00000840: 6176 6169 6c61 626c 6520 7461 626c 6573  available tables
+00000850: 2061 6e64 2066 6965 6c64 732c 2073 6565   and fields, see
+00000860: 2074 6865 2041 7661 696c 6162 6c65 0a20   the Available. 
+00000870: 2020 2020 2020 2020 2020 2066 6965 6c64             field
+00000880: 732e 0a20 2020 2020 2020 2070 6167 655f  s..        page_
+00000890: 7369 7a65 2028 696e 7429 3a0a 2020 2020  size (int):.    
+000008a0: 2020 2020 2020 2020 4f70 7469 6f6e 616c          Optional
+000008b0: 2e20 4e75 6d62 6572 206f 6620 6060 5265  . Number of ``Re
+000008c0: 706f 7274 526f 7773 6060 2074 6f20 7265  portRows`` to re
+000008d0: 7472 6965 7665 2069 6e20 6120 7369 6e67  trieve in a sing
+000008e0: 6c65 0a20 2020 2020 2020 2020 2020 2070  le.            p
+000008f0: 6167 652e 2044 6566 6175 6c74 7320 746f  age. Defaults to
+00000900: 2031 3030 302e 2056 616c 7565 7320 6162   1000. Values ab
+00000910: 6f76 6520 3530 3030 2061 7265 2063 6f65  ove 5000 are coe
+00000920: 7263 6564 2074 6f0a 2020 2020 2020 2020  rced to.        
+00000930: 2020 2020 3530 3030 2e0a 2020 2020 2020      5000..      
+00000940: 2020 7061 6765 5f74 6f6b 656e 2028 7374    page_token (st
+00000950: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00000960: 4f70 7469 6f6e 616c 2e20 546f 6b65 6e20  Optional. Token 
+00000970: 6f66 2074 6865 2070 6167 6520 746f 2072  of the page to r
+00000980: 6574 7269 6576 652e 2049 6620 6e6f 7420  etrieve. If not 
+00000990: 7370 6563 6966 6965 642c 0a20 2020 2020  specified,.     
+000009a0: 2020 2020 2020 2074 6865 2066 6972 7374         the first
+000009b0: 2070 6167 6520 6f66 2072 6573 756c 7473   page of results
+000009c0: 2069 7320 7265 7475 726e 6564 2e20 496e   is returned. In
+000009d0: 206f 7264 6572 2074 6f20 7265 7175 6573   order to reques
+000009e0: 740a 2020 2020 2020 2020 2020 2020 7468  t.            th
+000009f0: 6520 6e65 7874 2070 6167 6520 6f66 2072  e next page of r
+00000a00: 6573 756c 7473 2c20 7468 6520 7661 6c75  esults, the valu
+00000a10: 6520 6f62 7461 696e 6564 2066 726f 6d0a  e obtained from.
+00000a20: 2020 2020 2020 2020 2020 2020 6060 6e65              ``ne
+00000a30: 7874 5f70 6167 655f 746f 6b65 6e60 6020  xt_page_token`` 
+00000a40: 696e 2074 6865 2070 7265 7669 6f75 7320  in the previous 
+00000a50: 7265 7370 6f6e 7365 2073 686f 756c 6420  response should 
+00000a60: 6265 2075 7365 642e 0a20 2020 2022 2222  be used..    """
+00000a70: 0a0a 2020 2020 7061 7265 6e74 3a20 7374  ..    parent: st
+00000a80: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00000a90: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+00000aa0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+00000ab0: 756d 6265 723d 312c 0a20 2020 2029 0a20  umber=1,.    ). 
+00000ac0: 2020 2071 7565 7279 3a20 7374 7220 3d20     query: str = 
+00000ad0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00000ae0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+00000af0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+00000b00: 723d 322c 0a20 2020 2029 0a20 2020 2070  r=2,.    ).    p
+00000b10: 6167 655f 7369 7a65 3a20 696e 7420 3d20  age_size: int = 
+00000b20: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00000b30: 2020 2020 2070 726f 746f 2e49 4e54 3332       proto.INT32
+00000b40: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00000b50: 3d33 2c0a 2020 2020 290a 2020 2020 7061  =3,.    ).    pa
+00000b60: 6765 5f74 6f6b 656e 3a20 7374 7220 3d20  ge_token: str = 
+00000b70: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00000b80: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+00000b90: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+00000ba0: 723d 342c 0a20 2020 2029 0a0a 0a63 6c61  r=4,.    )...cla
+00000bb0: 7373 2053 6561 7263 6852 6573 706f 6e73  ss SearchRespons
+00000bc0: 6528 7072 6f74 6f2e 4d65 7373 6167 6529  e(proto.Message)
+00000bd0: 3a0a 2020 2020 7222 2222 5265 7370 6f6e  :.    r"""Respon
+00000be0: 7365 206d 6573 7361 6765 2066 6f72 2074  se message for t
+00000bf0: 6865 2060 6052 6570 6f72 7453 6572 7669  he ``ReportServi
+00000c00: 6365 2e53 6561 7263 6860 6020 6d65 7468  ce.Search`` meth
+00000c10: 6f64 2e0a 0a20 2020 2041 7474 7269 6275  od...    Attribu
+00000c20: 7465 733a 0a20 2020 2020 2020 2072 6573  tes:.        res
+00000c30: 756c 7473 2028 4d75 7461 626c 6553 6571  ults (MutableSeq
+00000c40: 7565 6e63 655b 676f 6f67 6c65 2e73 686f  uence[google.sho
+00000c50: 7070 696e 672e 6d65 7263 6861 6e74 5f72  pping.merchant_r
+00000c60: 6570 6f72 7473 5f76 3162 6574 612e 7479  eports_v1beta.ty
+00000c70: 7065 732e 5265 706f 7274 526f 775d 293a  pes.ReportRow]):
+00000c80: 0a20 2020 2020 2020 2020 2020 2052 6f77  .            Row
+00000c90: 7320 7468 6174 206d 6174 6368 6564 2074  s that matched t
+00000ca0: 6865 2073 6561 7263 6820 7175 6572 792e  he search query.
+00000cb0: 0a20 2020 2020 2020 206e 6578 745f 7061  .        next_pa
+00000cc0: 6765 5f74 6f6b 656e 2028 7374 7229 3a0a  ge_token (str):.
+00000cd0: 2020 2020 2020 2020 2020 2020 546f 6b65              Toke
+00000ce0: 6e20 7768 6963 6820 6361 6e20 6265 2073  n which can be s
+00000cf0: 656e 7420 6173 2060 6070 6167 655f 746f  ent as ``page_to
+00000d00: 6b65 6e60 6020 746f 2072 6574 7269 6576  ken`` to retriev
+00000d10: 6520 7468 650a 2020 2020 2020 2020 2020  e the.          
+00000d20: 2020 6e65 7874 2070 6167 652e 2049 6620    next page. If 
+00000d30: 6f6d 6974 7465 642c 2074 6865 7265 2061  omitted, there a
+00000d40: 7265 206e 6f20 7375 6273 6571 7565 6e74  re no subsequent
+00000d50: 2070 6167 6573 2e0a 2020 2020 2222 220a   pages..    """.
+00000d60: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00000d70: 2020 2064 6566 2072 6177 5f70 6167 6528     def raw_page(
+00000d80: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+00000d90: 6574 7572 6e20 7365 6c66 0a0a 2020 2020  eturn self..    
+00000da0: 7265 7375 6c74 733a 204d 7574 6162 6c65  results: Mutable
+00000db0: 5365 7175 656e 6365 5b22 5265 706f 7274  Sequence["Report
+00000dc0: 526f 7722 5d20 3d20 7072 6f74 6f2e 5265  Row"] = proto.Re
+00000dd0: 7065 6174 6564 4669 656c 6428 0a20 2020  peatedField(.   
+00000de0: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
+00000df0: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
+00000e00: 6572 3d31 2c0a 2020 2020 2020 2020 6d65  er=1,.        me
+00000e10: 7373 6167 653d 2252 6570 6f72 7452 6f77  ssage="ReportRow
+00000e20: 222c 0a20 2020 2029 0a20 2020 206e 6578  ",.    ).    nex
+00000e30: 745f 7061 6765 5f74 6f6b 656e 3a20 7374  t_page_token: st
+00000e40: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00000e50: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+00000e60: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+00000e70: 756d 6265 723d 322c 0a20 2020 2029 0a0a  umber=2,.    )..
+00000e80: 0a63 6c61 7373 2052 6570 6f72 7452 6f77  .class ReportRow
+00000e90: 2870 726f 746f 2e4d 6573 7361 6765 293a  (proto.Message):
+00000ea0: 0a20 2020 2072 2222 2252 6573 756c 7420  .    r"""Result 
+00000eb0: 726f 7720 7265 7475 726e 6564 2066 726f  row returned fro
+00000ec0: 6d20 7468 6520 7365 6172 6368 2071 7565  m the search que
+00000ed0: 7279 2e0a 0a20 2020 204f 6e6c 7920 7468  ry...    Only th
+00000ee0: 6520 6d65 7373 6167 6520 636f 7272 6573  e message corres
+00000ef0: 706f 6e64 696e 6720 746f 2074 6865 2071  ponding to the q
+00000f00: 7565 7269 6564 2074 6162 6c65 2069 7320  ueried table is 
+00000f10: 706f 7075 6c61 7465 640a 2020 2020 696e  populated.    in
+00000f20: 2074 6865 2072 6573 706f 6e73 652e 2057   the response. W
+00000f30: 6974 6869 6e20 7468 6520 706f 7075 6c61  ithin the popula
+00000f40: 7465 6420 6d65 7373 6167 652c 206f 6e6c  ted message, onl
+00000f50: 7920 7468 6520 6669 656c 6473 0a20 2020  y the fields.   
+00000f60: 2072 6571 7565 7374 6564 2065 7870 6c69   requested expli
+00000f70: 6369 746c 7920 696e 2074 6865 2071 7565  citly in the que
+00000f80: 7279 2061 7265 2070 6f70 756c 6174 6564  ry are populated
+00000f90: 2e0a 0a20 2020 2041 7474 7269 6275 7465  ...    Attribute
+00000fa0: 733a 0a20 2020 2020 2020 2070 726f 6475  s:.        produ
+00000fb0: 6374 5f70 6572 666f 726d 616e 6365 5f76  ct_performance_v
+00000fc0: 6965 7720 2867 6f6f 676c 652e 7368 6f70  iew (google.shop
+00000fd0: 7069 6e67 2e6d 6572 6368 616e 745f 7265  ping.merchant_re
+00000fe0: 706f 7274 735f 7631 6265 7461 2e74 7970  ports_v1beta.typ
+00000ff0: 6573 2e50 726f 6475 6374 5065 7266 6f72  es.ProductPerfor
+00001000: 6d61 6e63 6556 6965 7729 3a0a 2020 2020  manceView):.    
+00001010: 2020 2020 2020 2020 4669 656c 6473 2061          Fields a
+00001020: 7661 696c 6162 6c65 2066 6f72 2071 7565  vailable for que
+00001030: 7279 2069 6e20 6060 7072 6f64 7563 745f  ry in ``product_
+00001040: 7065 7266 6f72 6d61 6e63 655f 7669 6577  performance_view
+00001050: 6060 0a20 2020 2020 2020 2020 2020 2074  ``.            t
+00001060: 6162 6c65 2e0a 2020 2020 2020 2020 6e6f  able..        no
+00001070: 6e5f 7072 6f64 7563 745f 7065 7266 6f72  n_product_perfor
+00001080: 6d61 6e63 655f 7669 6577 2028 676f 6f67  mance_view (goog
+00001090: 6c65 2e73 686f 7070 696e 672e 6d65 7263  le.shopping.merc
+000010a0: 6861 6e74 5f72 6570 6f72 7473 5f76 3162  hant_reports_v1b
+000010b0: 6574 612e 7479 7065 732e 4e6f 6e50 726f  eta.types.NonPro
+000010c0: 6475 6374 5065 7266 6f72 6d61 6e63 6556  ductPerformanceV
+000010d0: 6965 7729 3a0a 2020 2020 2020 2020 2020  iew):.          
+000010e0: 2020 4669 656c 6473 2061 7661 696c 6162    Fields availab
+000010f0: 6c65 2066 6f72 2071 7565 7279 2069 6e0a  le for query in.
+00001100: 2020 2020 2020 2020 2020 2020 6060 6e6f              ``no
+00001110: 6e5f 7072 6f64 7563 745f 7065 7266 6f72  n_product_perfor
+00001120: 6d61 6e63 655f 7669 6577 6060 2074 6162  mance_view`` tab
+00001130: 6c65 2e0a 2020 2020 2020 2020 7072 6f64  le..        prod
+00001140: 7563 745f 7669 6577 2028 676f 6f67 6c65  uct_view (google
+00001150: 2e73 686f 7070 696e 672e 6d65 7263 6861  .shopping.mercha
+00001160: 6e74 5f72 6570 6f72 7473 5f76 3162 6574  nt_reports_v1bet
+00001170: 612e 7479 7065 732e 5072 6f64 7563 7456  a.types.ProductV
+00001180: 6965 7729 3a0a 2020 2020 2020 2020 2020  iew):.          
+00001190: 2020 4669 656c 6473 2061 7661 696c 6162    Fields availab
+000011a0: 6c65 2066 6f72 2071 7565 7279 2069 6e20  le for query in 
+000011b0: 6060 7072 6f64 7563 745f 7669 6577 6060  ``product_view``
+000011c0: 2074 6162 6c65 2e0a 2020 2020 2020 2020   table..        
+000011d0: 7072 6963 655f 636f 6d70 6574 6974 6976  price_competitiv
+000011e0: 656e 6573 735f 7072 6f64 7563 745f 7669  eness_product_vi
+000011f0: 6577 2028 676f 6f67 6c65 2e73 686f 7070  ew (google.shopp
+00001200: 696e 672e 6d65 7263 6861 6e74 5f72 6570  ing.merchant_rep
+00001210: 6f72 7473 5f76 3162 6574 612e 7479 7065  orts_v1beta.type
+00001220: 732e 5072 6963 6543 6f6d 7065 7469 7469  s.PriceCompetiti
+00001230: 7665 6e65 7373 5072 6f64 7563 7456 6965  venessProductVie
+00001240: 7729 3a0a 2020 2020 2020 2020 2020 2020  w):.            
+00001250: 4669 656c 6473 2061 7661 696c 6162 6c65  Fields available
+00001260: 2066 6f72 2071 7565 7279 2069 6e0a 2020   for query in.  
+00001270: 2020 2020 2020 2020 2020 6060 7072 6963            ``pric
+00001280: 655f 636f 6d70 6574 6974 6976 656e 6573  e_competitivenes
+00001290: 735f 7072 6f64 7563 745f 7669 6577 6060  s_product_view``
+000012a0: 2074 6162 6c65 2e0a 2020 2020 2020 2020   table..        
+000012b0: 7072 6963 655f 696e 7369 6768 7473 5f70  price_insights_p
+000012c0: 726f 6475 6374 5f76 6965 7720 2867 6f6f  roduct_view (goo
+000012d0: 676c 652e 7368 6f70 7069 6e67 2e6d 6572  gle.shopping.mer
+000012e0: 6368 616e 745f 7265 706f 7274 735f 7631  chant_reports_v1
+000012f0: 6265 7461 2e74 7970 6573 2e50 7269 6365  beta.types.Price
+00001300: 496e 7369 6768 7473 5072 6f64 7563 7456  InsightsProductV
+00001310: 6965 7729 3a0a 2020 2020 2020 2020 2020  iew):.          
+00001320: 2020 4669 656c 6473 2061 7661 696c 6162    Fields availab
+00001330: 6c65 2066 6f72 2071 7565 7279 2069 6e0a  le for query in.
+00001340: 2020 2020 2020 2020 2020 2020 6060 7072              ``pr
+00001350: 6963 655f 696e 7369 6768 7473 5f70 726f  ice_insights_pro
+00001360: 6475 6374 5f76 6965 7760 6020 7461 626c  duct_view`` tabl
+00001370: 652e 0a20 2020 2020 2020 2062 6573 745f  e..        best_
+00001380: 7365 6c6c 6572 735f 7072 6f64 7563 745f  sellers_product_
+00001390: 636c 7573 7465 725f 7669 6577 2028 676f  cluster_view (go
+000013a0: 6f67 6c65 2e73 686f 7070 696e 672e 6d65  ogle.shopping.me
+000013b0: 7263 6861 6e74 5f72 6570 6f72 7473 5f76  rchant_reports_v
+000013c0: 3162 6574 612e 7479 7065 732e 4265 7374  1beta.types.Best
+000013d0: 5365 6c6c 6572 7350 726f 6475 6374 436c  SellersProductCl
+000013e0: 7573 7465 7256 6965 7729 3a0a 2020 2020  usterView):.    
+000013f0: 2020 2020 2020 2020 4669 656c 6473 2061          Fields a
+00001400: 7661 696c 6162 6c65 2066 6f72 2071 7565  vailable for que
+00001410: 7279 2069 6e0a 2020 2020 2020 2020 2020  ry in.          
+00001420: 2020 6060 6265 7374 5f73 656c 6c65 7273    ``best_sellers
+00001430: 5f70 726f 6475 6374 5f63 6c75 7374 6572  _product_cluster
+00001440: 5f76 6965 7760 6020 7461 626c 652e 0a20  _view`` table.. 
+00001450: 2020 2020 2020 2062 6573 745f 7365 6c6c         best_sell
+00001460: 6572 735f 6272 616e 645f 7669 6577 2028  ers_brand_view (
+00001470: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
+00001480: 6d65 7263 6861 6e74 5f72 6570 6f72 7473  merchant_reports
+00001490: 5f76 3162 6574 612e 7479 7065 732e 4265  _v1beta.types.Be
+000014a0: 7374 5365 6c6c 6572 7342 7261 6e64 5669  stSellersBrandVi
+000014b0: 6577 293a 0a20 2020 2020 2020 2020 2020  ew):.           
+000014c0: 2046 6965 6c64 7320 6176 6169 6c61 626c   Fields availabl
+000014d0: 6520 666f 7220 7175 6572 7920 696e 2060  e for query in `
+000014e0: 6062 6573 745f 7365 6c6c 6572 735f 6272  `best_sellers_br
+000014f0: 616e 645f 7669 6577 6060 0a20 2020 2020  and_view``.     
+00001500: 2020 2020 2020 2074 6162 6c65 2e0a 2020         table..  
+00001510: 2020 2020 2020 636f 6d70 6574 6974 6976        competitiv
+00001520: 655f 7669 7369 6269 6c69 7479 5f63 6f6d  e_visibility_com
+00001530: 7065 7469 746f 725f 7669 6577 2028 676f  petitor_view (go
+00001540: 6f67 6c65 2e73 686f 7070 696e 672e 6d65  ogle.shopping.me
+00001550: 7263 6861 6e74 5f72 6570 6f72 7473 5f76  rchant_reports_v
+00001560: 3162 6574 612e 7479 7065 732e 436f 6d70  1beta.types.Comp
+00001570: 6574 6974 6976 6556 6973 6962 696c 6974  etitiveVisibilit
+00001580: 7943 6f6d 7065 7469 746f 7256 6965 7729  yCompetitorView)
+00001590: 3a0a 2020 2020 2020 2020 2020 2020 4669  :.            Fi
+000015a0: 656c 6473 2061 7661 696c 6162 6c65 2066  elds available f
+000015b0: 6f72 2071 7565 7279 2069 6e0a 2020 2020  or query in.    
+000015c0: 2020 2020 2020 2020 6060 636f 6d70 6574          ``compet
+000015d0: 6974 6976 655f 7669 7369 6269 6c69 7479  itive_visibility
+000015e0: 5f63 6f6d 7065 7469 746f 725f 7669 6577  _competitor_view
+000015f0: 6060 2074 6162 6c65 2e0a 2020 2020 2020  `` table..      
+00001600: 2020 636f 6d70 6574 6974 6976 655f 7669    competitive_vi
+00001610: 7369 6269 6c69 7479 5f74 6f70 5f6d 6572  sibility_top_mer
+00001620: 6368 616e 745f 7669 6577 2028 676f 6f67  chant_view (goog
+00001630: 6c65 2e73 686f 7070 696e 672e 6d65 7263  le.shopping.merc
+00001640: 6861 6e74 5f72 6570 6f72 7473 5f76 3162  hant_reports_v1b
+00001650: 6574 612e 7479 7065 732e 436f 6d70 6574  eta.types.Compet
+00001660: 6974 6976 6556 6973 6962 696c 6974 7954  itiveVisibilityT
+00001670: 6f70 4d65 7263 6861 6e74 5669 6577 293a  opMerchantView):
+00001680: 0a20 2020 2020 2020 2020 2020 2046 6965  .            Fie
+00001690: 6c64 7320 6176 6169 6c61 626c 6520 666f  lds available fo
+000016a0: 7220 7175 6572 7920 696e 0a20 2020 2020  r query in.     
+000016b0: 2020 2020 2020 2060 6063 6f6d 7065 7469         ``competi
+000016c0: 7469 7665 5f76 6973 6962 696c 6974 795f  tive_visibility_
+000016d0: 746f 705f 6d65 7263 6861 6e74 5f76 6965  top_merchant_vie
+000016e0: 7760 6020 7461 626c 652e 0a20 2020 2020  w`` table..     
+000016f0: 2020 2063 6f6d 7065 7469 7469 7665 5f76     competitive_v
+00001700: 6973 6962 696c 6974 795f 6265 6e63 686d  isibility_benchm
+00001710: 6172 6b5f 7669 6577 2028 676f 6f67 6c65  ark_view (google
+00001720: 2e73 686f 7070 696e 672e 6d65 7263 6861  .shopping.mercha
+00001730: 6e74 5f72 6570 6f72 7473 5f76 3162 6574  nt_reports_v1bet
+00001740: 612e 7479 7065 732e 436f 6d70 6574 6974  a.types.Competit
+00001750: 6976 6556 6973 6962 696c 6974 7942 656e  iveVisibilityBen
+00001760: 6368 6d61 726b 5669 6577 293a 0a20 2020  chmarkView):.   
+00001770: 2020 2020 2020 2020 2046 6965 6c64 7320           Fields 
+00001780: 6176 6169 6c61 626c 6520 666f 7220 7175  available for qu
+00001790: 6572 7920 696e 0a20 2020 2020 2020 2020  ery in.         
+000017a0: 2020 2060 6063 6f6d 7065 7469 7469 7665     ``competitive
+000017b0: 5f76 6973 6962 696c 6974 795f 6265 6e63  _visibility_benc
+000017c0: 686d 6172 6b5f 7669 6577 6060 2074 6162  hmark_view`` tab
+000017d0: 6c65 2e0a 2020 2020 2222 220a 0a20 2020  le..    """..   
+000017e0: 2070 726f 6475 6374 5f70 6572 666f 726d   product_perform
+000017f0: 616e 6365 5f76 6965 773a 2022 5072 6f64  ance_view: "Prod
+00001800: 7563 7450 6572 666f 726d 616e 6365 5669  uctPerformanceVi
+00001810: 6577 2220 3d20 7072 6f74 6f2e 4669 656c  ew" = proto.Fiel
+00001820: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+00001830: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
+00001840: 2020 6e75 6d62 6572 3d31 2c0a 2020 2020    number=1,.    
+00001850: 2020 2020 6d65 7373 6167 653d 2250 726f      message="Pro
+00001860: 6475 6374 5065 7266 6f72 6d61 6e63 6556  ductPerformanceV
+00001870: 6965 7722 2c0a 2020 2020 290a 2020 2020  iew",.    ).    
+00001880: 6e6f 6e5f 7072 6f64 7563 745f 7065 7266  non_product_perf
+00001890: 6f72 6d61 6e63 655f 7669 6577 3a20 224e  ormance_view: "N
+000018a0: 6f6e 5072 6f64 7563 7450 6572 666f 726d  onProductPerform
+000018b0: 616e 6365 5669 6577 2220 3d20 7072 6f74  anceView" = prot
+000018c0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+000018d0: 2070 726f 746f 2e4d 4553 5341 4745 2c0a   proto.MESSAGE,.
+000018e0: 2020 2020 2020 2020 6e75 6d62 6572 3d37          number=7
+000018f0: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
+00001900: 653d 224e 6f6e 5072 6f64 7563 7450 6572  e="NonProductPer
+00001910: 666f 726d 616e 6365 5669 6577 222c 0a20  formanceView",. 
+00001920: 2020 2029 0a20 2020 2070 726f 6475 6374     ).    product
+00001930: 5f76 6965 773a 2022 5072 6f64 7563 7456  _view: "ProductV
+00001940: 6965 7722 203d 2070 726f 746f 2e46 6965  iew" = proto.Fie
+00001950: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00001960: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
+00001970: 2020 206e 756d 6265 723d 322c 0a20 2020     number=2,.   
+00001980: 2020 2020 206d 6573 7361 6765 3d22 5072       message="Pr
+00001990: 6f64 7563 7456 6965 7722 2c0a 2020 2020  oductView",.    
+000019a0: 290a 2020 2020 7072 6963 655f 636f 6d70  ).    price_comp
+000019b0: 6574 6974 6976 656e 6573 735f 7072 6f64  etitiveness_prod
+000019c0: 7563 745f 7669 6577 3a20 2250 7269 6365  uct_view: "Price
+000019d0: 436f 6d70 6574 6974 6976 656e 6573 7350  CompetitivenessP
+000019e0: 726f 6475 6374 5669 6577 2220 3d20 7072  roductView" = pr
+000019f0: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+00001a00: 2020 2070 726f 746f 2e4d 4553 5341 4745     proto.MESSAGE
+00001a10: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00001a20: 3d33 2c0a 2020 2020 2020 2020 6d65 7373  =3,.        mess
+00001a30: 6167 653d 2250 7269 6365 436f 6d70 6574  age="PriceCompet
+00001a40: 6974 6976 656e 6573 7350 726f 6475 6374  itivenessProduct
+00001a50: 5669 6577 222c 0a20 2020 2029 0a20 2020  View",.    ).   
+00001a60: 2070 7269 6365 5f69 6e73 6967 6874 735f   price_insights_
+00001a70: 7072 6f64 7563 745f 7669 6577 3a20 2250  product_view: "P
+00001a80: 7269 6365 496e 7369 6768 7473 5072 6f64  riceInsightsProd
+00001a90: 7563 7456 6965 7722 203d 2070 726f 746f  uctView" = proto
+00001aa0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00001ab0: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+00001ac0: 2020 2020 2020 206e 756d 6265 723d 342c         number=4,
+00001ad0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+00001ae0: 3d22 5072 6963 6549 6e73 6967 6874 7350  ="PriceInsightsP
+00001af0: 726f 6475 6374 5669 6577 222c 0a20 2020  roductView",.   
+00001b00: 2029 0a20 2020 2062 6573 745f 7365 6c6c   ).    best_sell
+00001b10: 6572 735f 7072 6f64 7563 745f 636c 7573  ers_product_clus
+00001b20: 7465 725f 7669 6577 3a20 2242 6573 7453  ter_view: "BestS
+00001b30: 656c 6c65 7273 5072 6f64 7563 7443 6c75  ellersProductClu
+00001b40: 7374 6572 5669 6577 2220 3d20 7072 6f74  sterView" = prot
+00001b50: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00001b60: 2070 726f 746f 2e4d 4553 5341 4745 2c0a   proto.MESSAGE,.
+00001b70: 2020 2020 2020 2020 6e75 6d62 6572 3d35          number=5
+00001b80: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
+00001b90: 653d 2242 6573 7453 656c 6c65 7273 5072  e="BestSellersPr
+00001ba0: 6f64 7563 7443 6c75 7374 6572 5669 6577  oductClusterView
+00001bb0: 222c 0a20 2020 2029 0a20 2020 2062 6573  ",.    ).    bes
+00001bc0: 745f 7365 6c6c 6572 735f 6272 616e 645f  t_sellers_brand_
+00001bd0: 7669 6577 3a20 2242 6573 7453 656c 6c65  view: "BestSelle
+00001be0: 7273 4272 616e 6456 6965 7722 203d 2070  rsBrandView" = p
+00001bf0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00001c00: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
+00001c10: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
+00001c20: 723d 362c 0a20 2020 2020 2020 206d 6573  r=6,.        mes
+00001c30: 7361 6765 3d22 4265 7374 5365 6c6c 6572  sage="BestSeller
+00001c40: 7342 7261 6e64 5669 6577 222c 0a20 2020  sBrandView",.   
+00001c50: 2029 0a20 2020 2063 6f6d 7065 7469 7469   ).    competiti
+00001c60: 7665 5f76 6973 6962 696c 6974 795f 636f  ve_visibility_co
+00001c70: 6d70 6574 6974 6f72 5f76 6965 773a 2022  mpetitor_view: "
+00001c80: 436f 6d70 6574 6974 6976 6556 6973 6962  CompetitiveVisib
+00001c90: 696c 6974 7943 6f6d 7065 7469 746f 7256  ilityCompetitorV
+00001ca0: 6965 7722 203d 2028 0a20 2020 2020 2020  iew" = (.       
+00001cb0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00001cc0: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
+00001cd0: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
+00001ce0: 2020 2020 206e 756d 6265 723d 382c 0a20       number=8,. 
+00001cf0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00001d00: 6765 3d22 436f 6d70 6574 6974 6976 6556  ge="CompetitiveV
+00001d10: 6973 6962 696c 6974 7943 6f6d 7065 7469  isibilityCompeti
+00001d20: 746f 7256 6965 7722 2c0a 2020 2020 2020  torView",.      
+00001d30: 2020 290a 2020 2020 290a 2020 2020 636f    ).    ).    co
+00001d40: 6d70 6574 6974 6976 655f 7669 7369 6269  mpetitive_visibi
+00001d50: 6c69 7479 5f74 6f70 5f6d 6572 6368 616e  lity_top_merchan
+00001d60: 745f 7669 6577 3a20 2243 6f6d 7065 7469  t_view: "Competi
+00001d70: 7469 7665 5669 7369 6269 6c69 7479 546f  tiveVisibilityTo
+00001d80: 704d 6572 6368 616e 7456 6965 7722 203d  pMerchantView" =
+00001d90: 2028 0a20 2020 2020 2020 2070 726f 746f   (.        proto
+00001da0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00001db0: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
+00001dc0: 452c 0a20 2020 2020 2020 2020 2020 206e  E,.            n
+00001dd0: 756d 6265 723d 392c 0a20 2020 2020 2020  umber=9,.       
+00001de0: 2020 2020 206d 6573 7361 6765 3d22 436f       message="Co
+00001df0: 6d70 6574 6974 6976 6556 6973 6962 696c  mpetitiveVisibil
+00001e00: 6974 7954 6f70 4d65 7263 6861 6e74 5669  ityTopMerchantVi
+00001e10: 6577 222c 0a20 2020 2020 2020 2029 0a20  ew",.        ). 
+00001e20: 2020 2029 0a20 2020 2063 6f6d 7065 7469     ).    competi
+00001e30: 7469 7665 5f76 6973 6962 696c 6974 795f  tive_visibility_
+00001e40: 6265 6e63 686d 6172 6b5f 7669 6577 3a20  benchmark_view: 
+00001e50: 2243 6f6d 7065 7469 7469 7665 5669 7369  "CompetitiveVisi
+00001e60: 6269 6c69 7479 4265 6e63 686d 6172 6b56  bilityBenchmarkV
+00001e70: 6965 7722 203d 2028 0a20 2020 2020 2020  iew" = (.       
+00001e80: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00001e90: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
+00001ea0: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
+00001eb0: 2020 2020 206e 756d 6265 723d 3130 2c0a       number=10,.
+00001ec0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
+00001ed0: 6167 653d 2243 6f6d 7065 7469 7469 7665  age="Competitive
+00001ee0: 5669 7369 6269 6c69 7479 4265 6e63 686d  VisibilityBenchm
+00001ef0: 6172 6b56 6965 7722 2c0a 2020 2020 2020  arkView",.      
+00001f00: 2020 290a 2020 2020 290a 0a0a 636c 6173    ).    )...clas
+00001f10: 7320 5072 6f64 7563 7450 6572 666f 726d  s ProductPerform
+00001f20: 616e 6365 5669 6577 2870 726f 746f 2e4d  anceView(proto.M
+00001f30: 6573 7361 6765 293a 0a20 2020 2072 2222  essage):.    r""
+00001f40: 2246 6965 6c64 7320 6176 6169 6c61 626c  "Fields availabl
+00001f50: 6520 666f 7220 7175 6572 7920 696e 2060  e for query in `
+00001f60: 6070 726f 6475 6374 5f70 6572 666f 726d  `product_perform
+00001f70: 616e 6365 5f76 6965 7760 6020 7461 626c  ance_view`` tabl
+00001f80: 652e 0a0a 2020 2020 5072 6f64 7563 7420  e...    Product 
+00001f90: 7065 7266 6f72 6d61 6e63 6520 6461 7461  performance data
+00001fa0: 2066 6f72 2079 6f75 7220 6163 636f 756e   for your accoun
+00001fb0: 742c 2069 6e63 6c75 6469 6e67 2070 6572  t, including per
+00001fc0: 666f 726d 616e 6365 0a20 2020 206d 6574  formance.    met
+00001fd0: 7269 6373 2028 666f 7220 6578 616d 706c  rics (for exampl
+00001fe0: 652c 2060 6063 6c69 636b 7360 6029 2061  e, ``clicks``) a
+00001ff0: 6e64 2064 696d 656e 7369 6f6e 7320 6163  nd dimensions ac
+00002000: 636f 7264 696e 6720 746f 2077 6869 6368  cording to which
+00002010: 0a20 2020 2070 6572 666f 726d 616e 6365  .    performance
+00002020: 206d 6574 7269 6373 2061 7265 2073 6567   metrics are seg
+00002030: 6d65 6e74 6564 2028 666f 7220 6578 616d  mented (for exam
+00002040: 706c 652c 2060 606f 6666 6572 5f69 6460  ple, ``offer_id`
+00002050: 6029 2e0a 2020 2020 5661 6c75 6573 206f  `)..    Values o
+00002060: 6620 7072 6f64 7563 7420 6469 6d65 6e73  f product dimens
+00002070: 696f 6e73 2c20 7375 6368 2061 7320 6060  ions, such as ``
+00002080: 6f66 6665 725f 6964 6060 2c20 7265 666c  offer_id``, refl
+00002090: 6563 7420 7468 650a 2020 2020 7374 6174  ect the.    stat
+000020a0: 6520 6f66 2061 2070 726f 6475 6374 2061  e of a product a
+000020b0: 7420 7468 6520 7469 6d65 206f 6620 7468  t the time of th
+000020c0: 6520 696d 7072 6573 7369 6f6e 2e0a 0a20  e impression... 
+000020d0: 2020 2053 6567 6d65 6e74 2066 6965 6c64     Segment field
+000020e0: 7320 6361 6e6e 6f74 2062 6520 7365 6c65  s cannot be sele
+000020f0: 6374 6564 2069 6e20 7175 6572 6965 7320  cted in queries 
+00002100: 7769 7468 6f75 7420 616c 736f 2073 656c  without also sel
+00002110: 6563 7469 6e67 0a20 2020 2061 7420 6c65  ecting.    at le
+00002120: 6173 7420 6f6e 6520 6d65 7472 6963 2066  ast one metric f
+00002130: 6965 6c64 2e0a 0a20 2020 2056 616c 7565  ield...    Value
+00002140: 7320 6172 6520 6f6e 6c79 2073 6574 2066  s are only set f
+00002150: 6f72 2066 6965 6c64 7320 7265 7175 6573  or fields reques
+00002160: 7465 6420 6578 706c 6963 6974 6c79 2069  ted explicitly i
+00002170: 6e20 7468 6520 7265 7175 6573 7427 730a  n the request's.
+00002180: 2020 2020 7365 6172 6368 2071 7565 7279      search query
+00002190: 2e0a 0a0a 2020 2020 2e2e 205f 6f6e 656f  ....    .. _oneo
+000021a0: 663a 2068 7474 7073 3a2f 2f70 726f 746f  f: https://proto
+000021b0: 2d70 6c75 732d 7079 7468 6f6e 2e72 6561  -plus-python.rea
+000021c0: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
+000021d0: 7461 626c 652f 6669 656c 6473 2e68 746d  table/fields.htm
+000021e0: 6c23 6f6e 656f 6673 2d6d 7574 7561 6c6c  l#oneofs-mutuall
+000021f0: 792d 6578 636c 7573 6976 652d 6669 656c  y-exclusive-fiel
+00002200: 6473 0a0a 2020 2020 4174 7472 6962 7574  ds..    Attribut
+00002210: 6573 3a0a 2020 2020 2020 2020 6d61 726b  es:.        mark
+00002220: 6574 696e 675f 6d65 7468 6f64 2028 676f  eting_method (go
+00002230: 6f67 6c65 2e73 686f 7070 696e 672e 6d65  ogle.shopping.me
+00002240: 7263 6861 6e74 5f72 6570 6f72 7473 5f76  rchant_reports_v
+00002250: 3162 6574 612e 7479 7065 732e 4d61 726b  1beta.types.Mark
+00002260: 6574 696e 674d 6574 686f 642e 4d61 726b  etingMethod.Mark
+00002270: 6574 696e 674d 6574 686f 6445 6e75 6d29  etingMethodEnum)
+00002280: 3a0a 2020 2020 2020 2020 2020 2020 4d61  :.            Ma
+00002290: 726b 6574 696e 6720 6d65 7468 6f64 2074  rketing method t
+000022a0: 6f20 7768 6963 6820 6d65 7472 6963 7320  o which metrics 
+000022b0: 6170 706c 792e 0a20 2020 2020 2020 2020  apply..         
+000022c0: 2020 2053 6567 6d65 6e74 2e0a 0a20 2020     Segment...   
+000022d0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
+000022e0: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
+000022f0: 6f66 2060 6f6e 656f 6660 5f20 6060 5f6d  of `oneof`_ ``_m
+00002300: 6172 6b65 7469 6e67 5f6d 6574 686f 6460  arketing_method`
+00002310: 602e 0a20 2020 2020 2020 2064 6174 6520  `..        date 
+00002320: 2867 6f6f 676c 652e 7479 7065 2e64 6174  (google.type.dat
+00002330: 655f 7062 322e 4461 7465 293a 0a20 2020  e_pb2.Date):.   
+00002340: 2020 2020 2020 2020 2044 6174 6520 696e           Date in
+00002350: 2074 6865 206d 6572 6368 616e 7420 7469   the merchant ti
+00002360: 6d65 7a6f 6e65 2074 6f20 7768 6963 6820  mezone to which 
+00002370: 6d65 7472 6963 7320 6170 706c 792e 0a20  metrics apply.. 
+00002380: 2020 2020 2020 2020 2020 2053 6567 6d65             Segme
+00002390: 6e74 2e0a 0a20 2020 2020 2020 2020 2020  nt...           
+000023a0: 2043 6f6e 6469 7469 6f6e 206f 6e20 6060   Condition on ``
+000023b0: 6461 7465 6060 2069 7320 7265 7175 6972  date`` is requir
+000023c0: 6564 2069 6e20 7468 6520 6060 5748 4552  ed in the ``WHER
+000023d0: 4560 6020 636c 6175 7365 2e0a 2020 2020  E`` clause..    
+000023e0: 2020 2020 7765 656b 2028 676f 6f67 6c65      week (google
+000023f0: 2e74 7970 652e 6461 7465 5f70 6232 2e44  .type.date_pb2.D
+00002400: 6174 6529 3a0a 2020 2020 2020 2020 2020  ate):.          
+00002410: 2020 4669 7273 7420 6461 7920 6f66 2074    First day of t
+00002420: 6865 2077 6565 6b20 284d 6f6e 6461 7929  he week (Monday)
+00002430: 206f 6620 7468 6520 6d65 7472 6963 730a   of the metrics.
+00002440: 2020 2020 2020 2020 2020 2020 6461 7465              date
+00002450: 2069 6e20 7468 6520 6d65 7263 6861 6e74   in the merchant
+00002460: 2074 696d 657a 6f6e 652e 2053 6567 6d65   timezone. Segme
+00002470: 6e74 2e0a 2020 2020 2020 2020 6375 7374  nt..        cust
+00002480: 6f6d 6572 5f63 6f75 6e74 7279 5f63 6f64  omer_country_cod
+00002490: 6520 2873 7472 293a 0a20 2020 2020 2020  e (str):.       
+000024a0: 2020 2020 2043 6f64 6520 6f66 2074 6865       Code of the
+000024b0: 2063 6f75 6e74 7279 2077 6865 7265 2074   country where t
+000024c0: 6865 2063 7573 746f 6d65 7220 6973 0a20  he customer is. 
+000024d0: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
+000024e0: 6564 2061 7420 7468 6520 7469 6d65 206f  ed at the time o
+000024f0: 6620 7468 6520 6576 656e 742e 2052 6570  f the event. Rep
+00002500: 7265 7365 6e74 6564 2069 6e0a 2020 2020  resented in.    
+00002510: 2020 2020 2020 2020 7468 6520 4953 4f20          the ISO 
+00002520: 3331 3636 2066 6f72 6d61 742e 2053 6567  3166 format. Seg
+00002530: 6d65 6e74 2e0a 0a20 2020 2020 2020 2020  ment...         
+00002540: 2020 2049 6620 7468 6520 6375 7374 6f6d     If the custom
+00002550: 6572 2063 6f75 6e74 7279 2063 616e 6e6f  er country canno
+00002560: 7420 6265 2064 6574 6572 6d69 6e65 642c  t be determined,
+00002570: 2061 0a20 2020 2020 2020 2020 2020 2073   a.            s
+00002580: 7065 6369 616c 2027 5a5a 2720 636f 6465  pecial 'ZZ' code
+00002590: 2069 7320 7265 7475 726e 6564 2e0a 0a20   is returned... 
+000025a0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+000025b0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+000025c0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+000025d0: 5f63 7573 746f 6d65 725f 636f 756e 7472  _customer_countr
+000025e0: 795f 636f 6465 6060 2e0a 2020 2020 2020  y_code``..      
+000025f0: 2020 6f66 6665 725f 6964 2028 7374 7229    offer_id (str)
+00002600: 3a0a 2020 2020 2020 2020 2020 2020 4d65  :.            Me
+00002610: 7263 6861 6e74 2d70 726f 7669 6465 6420  rchant-provided 
+00002620: 6964 206f 6620 7468 6520 7072 6f64 7563  id of the produc
+00002630: 742e 2053 6567 6d65 6e74 2e0a 0a20 2020  t. Segment...   
+00002640: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
+00002650: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
+00002660: 6f66 2060 6f6e 656f 6660 5f20 6060 5f6f  of `oneof`_ ``_o
+00002670: 6666 6572 5f69 6460 602e 0a20 2020 2020  ffer_id``..     
+00002680: 2020 2074 6974 6c65 2028 7374 7229 3a0a     title (str):.
+00002690: 2020 2020 2020 2020 2020 2020 5469 746c              Titl
+000026a0: 6520 6f66 2074 6865 2070 726f 6475 6374  e of the product
+000026b0: 2e20 5365 676d 656e 742e 0a0a 2020 2020  . Segment...    
+000026c0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+000026d0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+000026e0: 6620 606f 6e65 6f66 605f 2060 605f 7469  f `oneof`_ ``_ti
+000026f0: 746c 6560 602e 0a20 2020 2020 2020 2062  tle``..        b
+00002700: 7261 6e64 2028 7374 7229 3a0a 2020 2020  rand (str):.    
+00002710: 2020 2020 2020 2020 4272 616e 6420 6f66          Brand of
+00002720: 2074 6865 2070 726f 6475 6374 2e20 5365   the product. Se
+00002730: 676d 656e 742e 0a0a 2020 2020 2020 2020  gment...        
+00002740: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+00002750: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+00002760: 6e65 6f66 605f 2060 605f 6272 616e 6460  neof`_ ``_brand`
+00002770: 602e 0a20 2020 2020 2020 2063 6174 6567  `..        categ
+00002780: 6f72 795f 6c31 2028 7374 7229 3a0a 2020  ory_l1 (str):.  
+00002790: 2020 2020 2020 2020 2020 6050 726f 6475            `Produ
+000027a0: 6374 2063 6174 6567 6f72 7920 2831 7374  ct category (1st
+000027b0: 0a20 2020 2020 2020 2020 2020 206c 6576  .            lev
+000027c0: 656c 2920 3c68 7474 7073 3a2f 2f64 6576  el) <https://dev
+000027d0: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+000027e0: 6f6d 2f73 686f 7070 696e 672d 636f 6e74  om/shopping-cont
+000027f0: 656e 742f 6775 6964 6573 2f72 6570 6f72  ent/guides/repor
+00002800: 7473 2f73 6567 6d65 6e74 6174 696f 6e23  ts/segmentation#
+00002810: 6361 7465 676f 7279 5f61 6e64 5f70 726f  category_and_pro
+00002820: 6475 6374 5f74 7970 653e 605f 5f0a 2020  duct_type>`__.  
+00002830: 2020 2020 2020 2020 2020 696e 2047 6f6f            in Goo
+00002840: 676c 6527 7320 7072 6f64 7563 7420 7461  gle's product ta
+00002850: 786f 6e6f 6d79 2e20 5365 676d 656e 742e  xonomy. Segment.
+00002860: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00002870: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+00002880: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+00002890: 2060 605f 6361 7465 676f 7279 5f6c 3160   ``_category_l1`
+000028a0: 602e 0a20 2020 2020 2020 2063 6174 6567  `..        categ
+000028b0: 6f72 795f 6c32 2028 7374 7229 3a0a 2020  ory_l2 (str):.  
+000028c0: 2020 2020 2020 2020 2020 6050 726f 6475            `Produ
+000028d0: 6374 2063 6174 6567 6f72 7920 2832 6e64  ct category (2nd
+000028e0: 0a20 2020 2020 2020 2020 2020 206c 6576  .            lev
+000028f0: 656c 2920 3c68 7474 7073 3a2f 2f64 6576  el) <https://dev
+00002900: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00002910: 6f6d 2f73 686f 7070 696e 672d 636f 6e74  om/shopping-cont
+00002920: 656e 742f 6775 6964 6573 2f72 6570 6f72  ent/guides/repor
+00002930: 7473 2f73 6567 6d65 6e74 6174 696f 6e23  ts/segmentation#
+00002940: 6361 7465 676f 7279 5f61 6e64 5f70 726f  category_and_pro
+00002950: 6475 6374 5f74 7970 653e 605f 5f0a 2020  duct_type>`__.  
+00002960: 2020 2020 2020 2020 2020 696e 2047 6f6f            in Goo
+00002970: 676c 6527 7320 7072 6f64 7563 7420 7461  gle's product ta
+00002980: 786f 6e6f 6d79 2e20 5365 676d 656e 742e  xonomy. Segment.
+00002990: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+000029a0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+000029b0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+000029c0: 2060 605f 6361 7465 676f 7279 5f6c 3260   ``_category_l2`
+000029d0: 602e 0a20 2020 2020 2020 2063 6174 6567  `..        categ
+000029e0: 6f72 795f 6c33 2028 7374 7229 3a0a 2020  ory_l3 (str):.  
+000029f0: 2020 2020 2020 2020 2020 6050 726f 6475            `Produ
+00002a00: 6374 2063 6174 6567 6f72 7920 2833 7264  ct category (3rd
+00002a10: 0a20 2020 2020 2020 2020 2020 206c 6576  .            lev
+00002a20: 656c 2920 3c68 7474 7073 3a2f 2f64 6576  el) <https://dev
+00002a30: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00002a40: 6f6d 2f73 686f 7070 696e 672d 636f 6e74  om/shopping-cont
+00002a50: 656e 742f 6775 6964 6573 2f72 6570 6f72  ent/guides/repor
+00002a60: 7473 2f73 6567 6d65 6e74 6174 696f 6e23  ts/segmentation#
+00002a70: 6361 7465 676f 7279 5f61 6e64 5f70 726f  category_and_pro
+00002a80: 6475 6374 5f74 7970 653e 605f 5f0a 2020  duct_type>`__.  
+00002a90: 2020 2020 2020 2020 2020 696e 2047 6f6f            in Goo
+00002aa0: 676c 6527 7320 7072 6f64 7563 7420 7461  gle's product ta
+00002ab0: 786f 6e6f 6d79 2e20 5365 676d 656e 742e  xonomy. Segment.
+00002ac0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00002ad0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+00002ae0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+00002af0: 2060 605f 6361 7465 676f 7279 5f6c 3360   ``_category_l3`
+00002b00: 602e 0a20 2020 2020 2020 2063 6174 6567  `..        categ
+00002b10: 6f72 795f 6c34 2028 7374 7229 3a0a 2020  ory_l4 (str):.  
+00002b20: 2020 2020 2020 2020 2020 6050 726f 6475            `Produ
+00002b30: 6374 2063 6174 6567 6f72 7920 2834 7468  ct category (4th
+00002b40: 0a20 2020 2020 2020 2020 2020 206c 6576  .            lev
+00002b50: 656c 2920 3c68 7474 7073 3a2f 2f64 6576  el) <https://dev
+00002b60: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00002b70: 6f6d 2f73 686f 7070 696e 672d 636f 6e74  om/shopping-cont
+00002b80: 656e 742f 6775 6964 6573 2f72 6570 6f72  ent/guides/repor
+00002b90: 7473 2f73 6567 6d65 6e74 6174 696f 6e23  ts/segmentation#
+00002ba0: 6361 7465 676f 7279 5f61 6e64 5f70 726f  category_and_pro
+00002bb0: 6475 6374 5f74 7970 653e 605f 5f0a 2020  duct_type>`__.  
+00002bc0: 2020 2020 2020 2020 2020 696e 2047 6f6f            in Goo
+00002bd0: 676c 6527 7320 7072 6f64 7563 7420 7461  gle's product ta
+00002be0: 786f 6e6f 6d79 2e20 5365 676d 656e 742e  xonomy. Segment.
+00002bf0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00002c00: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+00002c10: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+00002c20: 2060 605f 6361 7465 676f 7279 5f6c 3460   ``_category_l4`
+00002c30: 602e 0a20 2020 2020 2020 2063 6174 6567  `..        categ
+00002c40: 6f72 795f 6c35 2028 7374 7229 3a0a 2020  ory_l5 (str):.  
+00002c50: 2020 2020 2020 2020 2020 6050 726f 6475            `Produ
+00002c60: 6374 2063 6174 6567 6f72 7920 2835 7468  ct category (5th
+00002c70: 0a20 2020 2020 2020 2020 2020 206c 6576  .            lev
+00002c80: 656c 2920 3c68 7474 7073 3a2f 2f64 6576  el) <https://dev
+00002c90: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00002ca0: 6f6d 2f73 686f 7070 696e 672d 636f 6e74  om/shopping-cont
+00002cb0: 656e 742f 6775 6964 6573 2f72 6570 6f72  ent/guides/repor
+00002cc0: 7473 2f73 6567 6d65 6e74 6174 696f 6e23  ts/segmentation#
+00002cd0: 6361 7465 676f 7279 5f61 6e64 5f70 726f  category_and_pro
+00002ce0: 6475 6374 5f74 7970 653e 605f 5f0a 2020  duct_type>`__.  
+00002cf0: 2020 2020 2020 2020 2020 696e 2047 6f6f            in Goo
+00002d00: 676c 6527 7320 7072 6f64 7563 7420 7461  gle's product ta
+00002d10: 786f 6e6f 6d79 2e20 5365 676d 656e 742e  xonomy. Segment.
+00002d20: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00002d30: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+00002d40: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+00002d50: 2060 605f 6361 7465 676f 7279 5f6c 3560   ``_category_l5`
+00002d60: 602e 0a20 2020 2020 2020 2070 726f 6475  `..        produ
+00002d70: 6374 5f74 7970 655f 6c31 2028 7374 7229  ct_type_l1 (str)
+00002d80: 3a0a 2020 2020 2020 2020 2020 2020 6050  :.            `P
+00002d90: 726f 6475 6374 2074 7970 6520 2831 7374  roduct type (1st
+00002da0: 0a20 2020 2020 2020 2020 2020 206c 6576  .            lev
+00002db0: 656c 2920 3c68 7474 7073 3a2f 2f64 6576  el) <https://dev
+00002dc0: 656c 6f70 6572 732e 676f 6f67 6c65 2e63  elopers.google.c
+00002dd0: 6f6d 2f73 686f 7070 696e 672d 636f 6e74  om/shopping-cont
+00002de0: 656e 742f 6775 6964 6573 2f72 6570 6f72  ent/guides/repor
+00002df0: 7473 2f73 6567 6d65 6e74 6174 696f 6e23  ts/segmentation#
+00002e00: 6361 7465 676f 7279 5f61 6e64 5f70 726f  category_and_pro
+00002e10: 6475 6374 5f74 7970 653e 605f 5f0a 2020  duct_type>`__.  
+00002e20: 2020 2020 2020 2020 2020 696e 206d 6572            in mer
+00002e30: 6368 616e 7427 7320 6f77 6e20 7072 6f64  chant's own prod
+00002e40: 7563 7420 7461 786f 6e6f 6d79 2e20 5365  uct taxonomy. Se
+00002e50: 676d 656e 742e 0a0a 2020 2020 2020 2020  gment...        
+00002e60: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+00002e70: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+00002e80: 6e65 6f66 605f 2060 605f 7072 6f64 7563  neof`_ ``_produc
+00002e90: 745f 7479 7065 5f6c 3160 602e 0a20 2020  t_type_l1``..   
+00002ea0: 2020 2020 2070 726f 6475 6374 5f74 7970       product_typ
+00002eb0: 655f 6c32 2028 7374 7229 3a0a 2020 2020  e_l2 (str):.    
+00002ec0: 2020 2020 2020 2020 6050 726f 6475 6374          `Product
+00002ed0: 2074 7970 6520 2832 6e64 0a20 2020 2020   type (2nd.     
+00002ee0: 2020 2020 2020 206c 6576 656c 2920 3c68         level) <h
+00002ef0: 7474 7073 3a2f 2f64 6576 656c 6f70 6572  ttps://developer
+00002f00: 732e 676f 6f67 6c65 2e63 6f6d 2f73 686f  s.google.com/sho
+00002f10: 7070 696e 672d 636f 6e74 656e 742f 6775  pping-content/gu
+00002f20: 6964 6573 2f72 6570 6f72 7473 2f73 6567  ides/reports/seg
+00002f30: 6d65 6e74 6174 696f 6e23 6361 7465 676f  mentation#catego
+00002f40: 7279 5f61 6e64 5f70 726f 6475 6374 5f74  ry_and_product_t
+00002f50: 7970 653e 605f 5f0a 2020 2020 2020 2020  ype>`__.        
+00002f60: 2020 2020 696e 206d 6572 6368 616e 7427      in merchant'
+00002f70: 7320 6f77 6e20 7072 6f64 7563 7420 7461  s own product ta
+00002f80: 786f 6e6f 6d79 2e20 5365 676d 656e 742e  xonomy. Segment.
+00002f90: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00002fa0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+00002fb0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+00002fc0: 2060 605f 7072 6f64 7563 745f 7479 7065   ``_product_type
+00002fd0: 5f6c 3260 602e 0a20 2020 2020 2020 2070  _l2``..        p
+00002fe0: 726f 6475 6374 5f74 7970 655f 6c33 2028  roduct_type_l3 (
+00002ff0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00003000: 2020 6050 726f 6475 6374 2074 7970 6520    `Product type 
+00003010: 2833 7264 0a20 2020 2020 2020 2020 2020  (3rd.           
+00003020: 206c 6576 656c 2920 3c68 7474 7073 3a2f   level) <https:/
+00003030: 2f64 6576 656c 6f70 6572 732e 676f 6f67  /developers.goog
+00003040: 6c65 2e63 6f6d 2f73 686f 7070 696e 672d  le.com/shopping-
+00003050: 636f 6e74 656e 742f 6775 6964 6573 2f72  content/guides/r
+00003060: 6570 6f72 7473 2f73 6567 6d65 6e74 6174  eports/segmentat
+00003070: 696f 6e23 6361 7465 676f 7279 5f61 6e64  ion#category_and
+00003080: 5f70 726f 6475 6374 5f74 7970 653e 605f  _product_type>`_
+00003090: 5f0a 2020 2020 2020 2020 2020 2020 696e  _.            in
+000030a0: 206d 6572 6368 616e 7427 7320 6f77 6e20   merchant's own 
+000030b0: 7072 6f64 7563 7420 7461 786f 6e6f 6d79  product taxonomy
+000030c0: 2e20 5365 676d 656e 742e 0a0a 2020 2020  . Segment...    
+000030d0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+000030e0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+000030f0: 6620 606f 6e65 6f66 605f 2060 605f 7072  f `oneof`_ ``_pr
+00003100: 6f64 7563 745f 7479 7065 5f6c 3360 602e  oduct_type_l3``.
+00003110: 0a20 2020 2020 2020 2070 726f 6475 6374  .        product
+00003120: 5f74 7970 655f 6c34 2028 7374 7229 3a0a  _type_l4 (str):.
+00003130: 2020 2020 2020 2020 2020 2020 6050 726f              `Pro
+00003140: 6475 6374 2074 7970 6520 2834 7468 0a20  duct type (4th. 
+00003150: 2020 2020 2020 2020 2020 206c 6576 656c             level
+00003160: 2920 3c68 7474 7073 3a2f 2f64 6576 656c  ) <https://devel
+00003170: 6f70 6572 732e 676f 6f67 6c65 2e63 6f6d  opers.google.com
+00003180: 2f73 686f 7070 696e 672d 636f 6e74 656e  /shopping-conten
+00003190: 742f 6775 6964 6573 2f72 6570 6f72 7473  t/guides/reports
+000031a0: 2f73 6567 6d65 6e74 6174 696f 6e23 6361  /segmentation#ca
+000031b0: 7465 676f 7279 5f61 6e64 5f70 726f 6475  tegory_and_produ
+000031c0: 6374 5f74 7970 653e 605f 5f0a 2020 2020  ct_type>`__.    
+000031d0: 2020 2020 2020 2020 696e 206d 6572 6368          in merch
+000031e0: 616e 7427 7320 6f77 6e20 7072 6f64 7563  ant's own produc
+000031f0: 7420 7461 786f 6e6f 6d79 2e20 5365 676d  t taxonomy. Segm
+00003200: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
+00003210: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00003220: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00003230: 6f66 605f 2060 605f 7072 6f64 7563 745f  of`_ ``_product_
+00003240: 7479 7065 5f6c 3460 602e 0a20 2020 2020  type_l4``..     
+00003250: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
+00003260: 6c35 2028 7374 7229 3a0a 2020 2020 2020  l5 (str):.      
+00003270: 2020 2020 2020 6050 726f 6475 6374 2074        `Product t
+00003280: 7970 6520 2835 7468 0a20 2020 2020 2020  ype (5th.       
+00003290: 2020 2020 206c 6576 656c 2920 3c68 7474       level) <htt
+000032a0: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
+000032b0: 676f 6f67 6c65 2e63 6f6d 2f73 686f 7070  google.com/shopp
+000032c0: 696e 672d 636f 6e74 656e 742f 6775 6964  ing-content/guid
+000032d0: 6573 2f72 6570 6f72 7473 2f73 6567 6d65  es/reports/segme
+000032e0: 6e74 6174 696f 6e23 6361 7465 676f 7279  ntation#category
+000032f0: 5f61 6e64 5f70 726f 6475 6374 5f74 7970  _and_product_typ
+00003300: 653e 605f 5f0a 2020 2020 2020 2020 2020  e>`__.          
+00003310: 2020 696e 206d 6572 6368 616e 7427 7320    in merchant's 
+00003320: 6f77 6e20 7072 6f64 7563 7420 7461 786f  own product taxo
+00003330: 6e6f 6d79 2e20 5365 676d 656e 742e 0a0a  nomy. Segment...
+00003340: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00003350: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00003360: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+00003370: 605f 7072 6f64 7563 745f 7479 7065 5f6c  `_product_type_l
+00003380: 3560 602e 0a20 2020 2020 2020 2063 7573  5``..        cus
+00003390: 746f 6d5f 6c61 6265 6c30 2028 7374 7229  tom_label0 (str)
+000033a0: 3a0a 2020 2020 2020 2020 2020 2020 4375  :.            Cu
+000033b0: 7374 6f6d 206c 6162 656c 2030 2066 6f72  stom label 0 for
+000033c0: 2063 7573 746f 6d20 6772 6f75 7069 6e67   custom grouping
+000033d0: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
+000033e0: 7072 6f64 7563 7473 2e20 5365 676d 656e  products. Segmen
+000033f0: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
+00003400: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+00003410: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+00003420: 605f 2060 605f 6375 7374 6f6d 5f6c 6162  `_ ``_custom_lab
+00003430: 656c 3060 602e 0a20 2020 2020 2020 2063  el0``..        c
+00003440: 7573 746f 6d5f 6c61 6265 6c31 2028 7374  ustom_label1 (st
+00003450: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00003460: 4375 7374 6f6d 206c 6162 656c 2031 2066  Custom label 1 f
+00003470: 6f72 2063 7573 746f 6d20 6772 6f75 7069  or custom groupi
+00003480: 6e67 206f 660a 2020 2020 2020 2020 2020  ng of.          
+00003490: 2020 7072 6f64 7563 7473 2e20 5365 676d    products. Segm
+000034a0: 656e 742e 0a0a 2020 2020 2020 2020 2020  ent...          
+000034b0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+000034c0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+000034d0: 6f66 605f 2060 605f 6375 7374 6f6d 5f6c  of`_ ``_custom_l
+000034e0: 6162 656c 3160 602e 0a20 2020 2020 2020  abel1``..       
+000034f0: 2063 7573 746f 6d5f 6c61 6265 6c32 2028   custom_label2 (
+00003500: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00003510: 2020 4375 7374 6f6d 206c 6162 656c 2032    Custom label 2
+00003520: 2066 6f72 2063 7573 746f 6d20 6772 6f75   for custom grou
+00003530: 7069 6e67 206f 660a 2020 2020 2020 2020  ping of.        
+00003540: 2020 2020 7072 6f64 7563 7473 2e20 5365      products. Se
+00003550: 676d 656e 742e 0a0a 2020 2020 2020 2020  gment...        
+00003560: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+00003570: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+00003580: 6e65 6f66 605f 2060 605f 6375 7374 6f6d  neof`_ ``_custom
+00003590: 5f6c 6162 656c 3260 602e 0a20 2020 2020  _label2``..     
+000035a0: 2020 2063 7573 746f 6d5f 6c61 6265 6c33     custom_label3
+000035b0: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+000035c0: 2020 2020 4375 7374 6f6d 206c 6162 656c      Custom label
+000035d0: 2033 2066 6f72 2063 7573 746f 6d20 6772   3 for custom gr
+000035e0: 6f75 7069 6e67 206f 660a 2020 2020 2020  ouping of.      
+000035f0: 2020 2020 2020 7072 6f64 7563 7473 2e20        products. 
+00003600: 5365 676d 656e 742e 0a0a 2020 2020 2020  Segment...      
+00003610: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+00003620: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+00003630: 606f 6e65 6f66 605f 2060 605f 6375 7374  `oneof`_ ``_cust
+00003640: 6f6d 5f6c 6162 656c 3360 602e 0a20 2020  om_label3``..   
+00003650: 2020 2020 2063 7573 746f 6d5f 6c61 6265       custom_labe
+00003660: 6c34 2028 7374 7229 3a0a 2020 2020 2020  l4 (str):.      
+00003670: 2020 2020 2020 4375 7374 6f6d 206c 6162        Custom lab
+00003680: 656c 2034 2066 6f72 2063 7573 746f 6d20  el 4 for custom 
+00003690: 6772 6f75 7069 6e67 206f 660a 2020 2020  grouping of.    
+000036a0: 2020 2020 2020 2020 7072 6f64 7563 7473          products
+000036b0: 2e20 5365 676d 656e 742e 0a0a 2020 2020  . Segment...    
+000036c0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+000036d0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+000036e0: 6620 606f 6e65 6f66 605f 2060 605f 6375  f `oneof`_ ``_cu
+000036f0: 7374 6f6d 5f6c 6162 656c 3460 602e 0a20  stom_label4``.. 
+00003700: 2020 2020 2020 2063 6c69 636b 7320 2869         clicks (i
+00003710: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+00003720: 204e 756d 6265 7220 6f66 2063 6c69 636b   Number of click
+00003730: 732e 204d 6574 7269 632e 0a0a 2020 2020  s. Metric...    
+00003740: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+00003750: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+00003760: 6620 606f 6e65 6f66 605f 2060 605f 636c  f `oneof`_ ``_cl
+00003770: 6963 6b73 6060 2e0a 2020 2020 2020 2020  icks``..        
+00003780: 696d 7072 6573 7369 6f6e 7320 2869 6e74  impressions (int
+00003790: 293a 0a20 2020 2020 2020 2020 2020 204e  ):.            N
+000037a0: 756d 6265 7220 6f66 2074 696d 6573 206d  umber of times m
+000037b0: 6572 6368 616e 7427 7320 7072 6f64 7563  erchant's produc
+000037c0: 7473 2061 7265 0a20 2020 2020 2020 2020  ts are.         
+000037d0: 2020 2073 686f 776e 2e20 4d65 7472 6963     shown. Metric
+000037e0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
+000037f0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
+00003800: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
+00003810: 5f20 6060 5f69 6d70 7265 7373 696f 6e73  _ ``_impressions
+00003820: 6060 2e0a 2020 2020 2020 2020 636c 6963  ``..        clic
+00003830: 6b5f 7468 726f 7567 685f 7261 7465 2028  k_through_rate (
+00003840: 666c 6f61 7429 3a0a 2020 2020 2020 2020  float):.        
+00003850: 2020 2020 436c 6963 6b2d 7468 726f 7567      Click-throug
+00003860: 6820 7261 7465 202d 2074 6865 206e 756d  h rate - the num
+00003870: 6265 7220 6f66 2063 6c69 636b 730a 2020  ber of clicks.  
+00003880: 2020 2020 2020 2020 2020 6d65 7263 6861            mercha
+00003890: 6e74 2773 2070 726f 6475 6374 7320 7265  nt's products re
+000038a0: 6365 6976 6520 2863 6c69 636b 7329 2064  ceive (clicks) d
+000038b0: 6976 6964 6564 2062 790a 2020 2020 2020  ivided by.      
+000038c0: 2020 2020 2020 7468 6520 6e75 6d62 6572        the number
+000038d0: 206f 6620 7469 6d65 7320 7468 6520 7072   of times the pr
+000038e0: 6f64 7563 7473 2061 7265 2073 686f 776e  oducts are shown
+000038f0: 0a20 2020 2020 2020 2020 2020 2028 696d  .            (im
+00003900: 7072 6573 7369 6f6e 7329 2e20 4d65 7472  pressions). Metr
+00003910: 6963 2e0a 0a20 2020 2020 2020 2020 2020  ic...           
+00003920: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+00003930: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+00003940: 6660 5f20 6060 5f63 6c69 636b 5f74 6872  f`_ ``_click_thr
+00003950: 6f75 6768 5f72 6174 6560 602e 0a20 2020  ough_rate``..   
+00003960: 2020 2020 2063 6f6e 7665 7273 696f 6e73       conversions
+00003970: 2028 666c 6f61 7429 3a0a 2020 2020 2020   (float):.      
+00003980: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
+00003990: 636f 6e76 6572 7369 6f6e 7320 6174 7472  conversions attr
+000039a0: 6962 7574 6564 2074 6f20 7468 6520 7072  ibuted to the pr
+000039b0: 6f64 7563 742c 2072 6570 6f72 7465 6420  oduct, reported 
+000039c0: 6f6e 0a20 2020 2020 2020 2020 2020 2074  on.            t
+000039d0: 6865 2063 6f6e 7665 7273 696f 6e20 6461  he conversion da
+000039e0: 7465 2e20 4465 7065 6e64 696e 6720 6f6e  te. Depending on
+000039f0: 2074 6865 2061 7474 7269 6275 7469 6f6e   the attribution
+00003a00: 206d 6f64 656c 2c20 610a 2020 2020 2020   model, a.      
+00003a10: 2020 2020 2020 636f 6e76 6572 7369 6f6e        conversion
+00003a20: 206d 6967 6874 2062 6520 6469 7374 7269   might be distri
+00003a30: 6275 7465 6420 6163 726f 7373 206d 756c  buted across mul
+00003a40: 7469 706c 6520 636c 6963 6b73 2c0a 2020  tiple clicks,.  
+00003a50: 2020 2020 2020 2020 2020 7768 6572 6520            where 
+00003a60: 6561 6368 2063 6c69 636b 2067 6574 7320  each click gets 
+00003a70: 6974 7320 6f77 6e20 6372 6564 6974 2061  its own credit a
+00003a80: 7373 6967 6e65 642e 2054 6869 7320 6d65  ssigned. This me
+00003a90: 7472 6963 0a20 2020 2020 2020 2020 2020  tric.           
+00003aa0: 2069 7320 6120 7375 6d20 6f66 2061 6c6c   is a sum of all
+00003ab0: 2073 7563 6820 6372 6564 6974 732e 204d   such credits. M
+00003ac0: 6574 7269 632e 0a0a 2020 2020 2020 2020  etric...        
+00003ad0: 2020 2020 4176 6169 6c61 626c 6520 6f6e      Available on
+00003ae0: 6c79 2066 6f72 2074 6865 2060 6046 5245  ly for the ``FRE
+00003af0: 4560 6020 7472 6166 6669 6320 736f 7572  E`` traffic sour
+00003b00: 6365 2e0a 0a20 2020 2020 2020 2020 2020  ce...           
+00003b10: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+00003b20: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+00003b30: 6660 5f20 6060 5f63 6f6e 7665 7273 696f  f`_ ``_conversio
+00003b40: 6e73 6060 2e0a 2020 2020 2020 2020 636f  ns``..        co
+00003b50: 6e76 6572 7369 6f6e 5f76 616c 7565 2028  nversion_value (
+00003b60: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
+00003b70: 7479 7065 2e74 7970 6573 2e50 7269 6365  type.types.Price
+00003b80: 293a 0a20 2020 2020 2020 2020 2020 2056  ):.            V
+00003b90: 616c 7565 206f 6620 636f 6e76 6572 7369  alue of conversi
+00003ba0: 6f6e 7320 6174 7472 6962 7574 6564 2074  ons attributed t
+00003bb0: 6f20 7468 6520 7072 6f64 7563 742c 2072  o the product, r
+00003bc0: 6570 6f72 7465 6420 6f6e 0a20 2020 2020  eported on.     
+00003bd0: 2020 2020 2020 2074 6865 2063 6f6e 7665         the conve
+00003be0: 7273 696f 6e20 6461 7465 2e20 4d65 7472  rsion date. Metr
+00003bf0: 6963 2e0a 0a20 2020 2020 2020 2020 2020  ic...           
+00003c00: 2041 7661 696c 6162 6c65 206f 6e6c 7920   Available only 
+00003c10: 666f 7220 7468 6520 6060 4652 4545 6060  for the ``FREE``
+00003c20: 2074 7261 6666 6963 2073 6f75 7263 652e   traffic source.
+00003c30: 0a20 2020 2020 2020 2063 6f6e 7665 7273  .        convers
+00003c40: 696f 6e5f 7261 7465 2028 666c 6f61 7429  ion_rate (float)
+00003c50: 3a0a 2020 2020 2020 2020 2020 2020 4e75  :.            Nu
+00003c60: 6d62 6572 206f 6620 636f 6e76 6572 7369  mber of conversi
+00003c70: 6f6e 7320 6469 7669 6465 6420 6279 2074  ons divided by t
+00003c80: 6865 206e 756d 6265 7220 6f66 2063 6c69  he number of cli
+00003c90: 636b 732c 0a20 2020 2020 2020 2020 2020  cks,.           
+00003ca0: 2072 6570 6f72 7465 6420 6f6e 2074 6865   reported on the
+00003cb0: 2069 6d70 7265 7373 696f 6e20 6461 7465   impression date
+00003cc0: 2e20 4d65 7472 6963 2e0a 0a20 2020 2020  . Metric...     
+00003cd0: 2020 2020 2020 2041 7661 696c 6162 6c65         Available
+00003ce0: 206f 6e6c 7920 666f 7220 7468 6520 6060   only for the ``
+00003cf0: 4652 4545 6060 2074 7261 6666 6963 2073  FREE`` traffic s
+00003d00: 6f75 7263 652e 0a0a 2020 2020 2020 2020  ource...        
+00003d10: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+00003d20: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+00003d30: 6e65 6f66 605f 2060 605f 636f 6e76 6572  neof`_ ``_conver
+00003d40: 7369 6f6e 5f72 6174 6560 602e 0a20 2020  sion_rate``..   
+00003d50: 2022 2222 0a0a 2020 2020 6d61 726b 6574   """..    market
+00003d60: 696e 675f 6d65 7468 6f64 3a20 224d 6172  ing_method: "Mar
+00003d70: 6b65 7469 6e67 4d65 7468 6f64 2e4d 6172  ketingMethod.Mar
+00003d80: 6b65 7469 6e67 4d65 7468 6f64 456e 756d  ketingMethodEnum
+00003d90: 2220 3d20 7072 6f74 6f2e 4669 656c 6428  " = proto.Field(
+00003da0: 0a20 2020 2020 2020 2070 726f 746f 2e45  .        proto.E
+00003db0: 4e55 4d2c 0a20 2020 2020 2020 206e 756d  NUM,.        num
+00003dc0: 6265 723d 312c 0a20 2020 2020 2020 206f  ber=1,.        o
+00003dd0: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+00003de0: 2020 2020 2020 656e 756d 3d22 4d61 726b        enum="Mark
+00003df0: 6574 696e 674d 6574 686f 642e 4d61 726b  etingMethod.Mark
+00003e00: 6574 696e 674d 6574 686f 6445 6e75 6d22  etingMethodEnum"
+00003e10: 2c0a 2020 2020 290a 2020 2020 6461 7465  ,.    ).    date
+00003e20: 3a20 6461 7465 5f70 6232 2e44 6174 6520  : date_pb2.Date 
+00003e30: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00003e40: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
+00003e50: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
+00003e60: 6d62 6572 3d32 2c0a 2020 2020 2020 2020  mber=2,.        
+00003e70: 6d65 7373 6167 653d 6461 7465 5f70 6232  message=date_pb2
+00003e80: 2e44 6174 652c 0a20 2020 2029 0a20 2020  .Date,.    ).   
+00003e90: 2077 6565 6b3a 2064 6174 655f 7062 322e   week: date_pb2.
+00003ea0: 4461 7465 203d 2070 726f 746f 2e46 6965  Date = proto.Fie
+00003eb0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00003ec0: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
+00003ed0: 2020 206e 756d 6265 723d 332c 0a20 2020     number=3,.   
+00003ee0: 2020 2020 206d 6573 7361 6765 3d64 6174       message=dat
+00003ef0: 655f 7062 322e 4461 7465 2c0a 2020 2020  e_pb2.Date,.    
+00003f00: 290a 2020 2020 6375 7374 6f6d 6572 5f63  ).    customer_c
+00003f10: 6f75 6e74 7279 5f63 6f64 653a 2073 7472  ountry_code: str
+00003f20: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00003f30: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+00003f40: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+00003f50: 6d62 6572 3d34 2c0a 2020 2020 2020 2020  mber=4,.        
+00003f60: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00003f70: 2020 2029 0a20 2020 206f 6666 6572 5f69     ).    offer_i
+00003f80: 643a 2073 7472 203d 2070 726f 746f 2e46  d: str = proto.F
+00003f90: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00003fa0: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+00003fb0: 2020 2020 6e75 6d62 6572 3d35 2c0a 2020      number=5,.  
+00003fc0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+00003fd0: 7275 652c 0a20 2020 2029 0a20 2020 2074  rue,.    ).    t
+00003fe0: 6974 6c65 3a20 7374 7220 3d20 7072 6f74  itle: str = prot
+00003ff0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00004000: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+00004010: 2020 2020 2020 206e 756d 6265 723d 362c         number=6,
+00004020: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+00004030: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+00004040: 2020 6272 616e 643a 2073 7472 203d 2070    brand: str = p
+00004050: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00004060: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+00004070: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00004080: 3d37 2c0a 2020 2020 2020 2020 6f70 7469  =7,.        opti
+00004090: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+000040a0: 0a20 2020 2063 6174 6567 6f72 795f 6c31  .    category_l1
+000040b0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+000040c0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+000040d0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+000040e0: 2020 206e 756d 6265 723d 382c 0a20 2020     number=8,.   
+000040f0: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+00004100: 7565 2c0a 2020 2020 290a 2020 2020 6361  ue,.    ).    ca
+00004110: 7465 676f 7279 5f6c 323a 2073 7472 203d  tegory_l2: str =
+00004120: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00004130: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+00004140: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
+00004150: 6572 3d39 2c0a 2020 2020 2020 2020 6f70  er=9,.        op
+00004160: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+00004170: 2029 0a20 2020 2063 6174 6567 6f72 795f   ).    category_
+00004180: 6c33 3a20 7374 7220 3d20 7072 6f74 6f2e  l3: str = proto.
+00004190: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+000041a0: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+000041b0: 2020 2020 206e 756d 6265 723d 3130 2c0a       number=10,.
+000041c0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+000041d0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+000041e0: 2063 6174 6567 6f72 795f 6c34 3a20 7374   category_l4: st
+000041f0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00004200: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+00004210: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+00004220: 756d 6265 723d 3131 2c0a 2020 2020 2020  umber=11,.      
+00004230: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+00004240: 0a20 2020 2029 0a20 2020 2063 6174 6567  .    ).    categ
+00004250: 6f72 795f 6c35 3a20 7374 7220 3d20 7072  ory_l5: str = pr
+00004260: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+00004270: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
+00004280: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+00004290: 3132 2c0a 2020 2020 2020 2020 6f70 7469  12,.        opti
+000042a0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+000042b0: 0a20 2020 2070 726f 6475 6374 5f74 7970  .    product_typ
+000042c0: 655f 6c31 3a20 7374 7220 3d20 7072 6f74  e_l1: str = prot
+000042d0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+000042e0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+000042f0: 2020 2020 2020 206e 756d 6265 723d 3133         number=13
+00004300: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+00004310: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+00004320: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
+00004330: 6c32 3a20 7374 7220 3d20 7072 6f74 6f2e  l2: str = proto.
+00004340: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00004350: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+00004360: 2020 2020 206e 756d 6265 723d 3134 2c0a       number=14,.
+00004370: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00004380: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+00004390: 2070 726f 6475 6374 5f74 7970 655f 6c33   product_type_l3
+000043a0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+000043b0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+000043c0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+000043d0: 2020 206e 756d 6265 723d 3135 2c0a 2020     number=15,.  
+000043e0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+000043f0: 7275 652c 0a20 2020 2029 0a20 2020 2070  rue,.    ).    p
+00004400: 726f 6475 6374 5f74 7970 655f 6c34 3a20  roduct_type_l4: 
+00004410: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
+00004420: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+00004430: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
+00004440: 206e 756d 6265 723d 3136 2c0a 2020 2020   number=16,.    
+00004450: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+00004460: 652c 0a20 2020 2029 0a20 2020 2070 726f  e,.    ).    pro
+00004470: 6475 6374 5f74 7970 655f 6c35 3a20 7374  duct_type_l5: st
+00004480: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00004490: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+000044a0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+000044b0: 756d 6265 723d 3137 2c0a 2020 2020 2020  umber=17,.      
+000044c0: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+000044d0: 0a20 2020 2029 0a20 2020 2063 7573 746f  .    ).    custo
+000044e0: 6d5f 6c61 6265 6c30 3a20 7374 7220 3d20  m_label0: str = 
+000044f0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00004500: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+00004510: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+00004520: 723d 3138 2c0a 2020 2020 2020 2020 6f70  r=18,.        op
+00004530: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+00004540: 2029 0a20 2020 2063 7573 746f 6d5f 6c61   ).    custom_la
+00004550: 6265 6c31 3a20 7374 7220 3d20 7072 6f74  bel1: str = prot
+00004560: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00004570: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+00004580: 2020 2020 2020 206e 756d 6265 723d 3139         number=19
+00004590: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+000045a0: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+000045b0: 2020 2063 7573 746f 6d5f 6c61 6265 6c32     custom_label2
+000045c0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+000045d0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+000045e0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+000045f0: 2020 206e 756d 6265 723d 3230 2c0a 2020     number=20,.  
+00004600: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+00004610: 7275 652c 0a20 2020 2029 0a20 2020 2063  rue,.    ).    c
+00004620: 7573 746f 6d5f 6c61 6265 6c33 3a20 7374  ustom_label3: st
+00004630: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00004640: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+00004650: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+00004660: 756d 6265 723d 3231 2c0a 2020 2020 2020  umber=21,.      
+00004670: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+00004680: 0a20 2020 2029 0a20 2020 2063 7573 746f  .    ).    custo
+00004690: 6d5f 6c61 6265 6c34 3a20 7374 7220 3d20  m_label4: str = 
+000046a0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+000046b0: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+000046c0: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+000046d0: 723d 3232 2c0a 2020 2020 2020 2020 6f70  r=22,.        op
+000046e0: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+000046f0: 2029 0a20 2020 2063 6c69 636b 733a 2069   ).    clicks: i
+00004700: 6e74 203d 2070 726f 746f 2e46 6965 6c64  nt = proto.Field
+00004710: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00004720: 494e 5436 342c 0a20 2020 2020 2020 206e  INT64,.        n
+00004730: 756d 6265 723d 3233 2c0a 2020 2020 2020  umber=23,.      
+00004740: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+00004750: 0a20 2020 2029 0a20 2020 2069 6d70 7265  .    ).    impre
+00004760: 7373 696f 6e73 3a20 696e 7420 3d20 7072  ssions: int = pr
+00004770: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+00004780: 2020 2070 726f 746f 2e49 4e54 3634 2c0a     proto.INT64,.
+00004790: 2020 2020 2020 2020 6e75 6d62 6572 3d32          number=2
+000047a0: 342c 0a20 2020 2020 2020 206f 7074 696f  4,.        optio
+000047b0: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
+000047c0: 2020 2020 636c 6963 6b5f 7468 726f 7567      click_throug
+000047d0: 685f 7261 7465 3a20 666c 6f61 7420 3d20  h_rate: float = 
+000047e0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+000047f0: 2020 2020 2070 726f 746f 2e44 4f55 424c       proto.DOUBL
+00004800: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
+00004810: 723d 3235 2c0a 2020 2020 2020 2020 6f70  r=25,.        op
+00004820: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+00004830: 2029 0a20 2020 2063 6f6e 7665 7273 696f   ).    conversio
+00004840: 6e73 3a20 666c 6f61 7420 3d20 7072 6f74  ns: float = prot
+00004850: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00004860: 2070 726f 746f 2e44 4f55 424c 452c 0a20   proto.DOUBLE,. 
+00004870: 2020 2020 2020 206e 756d 6265 723d 3236         number=26
+00004880: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+00004890: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+000048a0: 2020 2063 6f6e 7665 7273 696f 6e5f 7661     conversion_va
+000048b0: 6c75 653a 2074 7970 6573 2e50 7269 6365  lue: types.Price
+000048c0: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+000048d0: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+000048e0: 5353 4147 452c 0a20 2020 2020 2020 206e  SSAGE,.        n
+000048f0: 756d 6265 723d 3237 2c0a 2020 2020 2020  umber=27,.      
+00004900: 2020 6d65 7373 6167 653d 7479 7065 732e    message=types.
+00004910: 5072 6963 652c 0a20 2020 2029 0a20 2020  Price,.    ).   
+00004920: 2063 6f6e 7665 7273 696f 6e5f 7261 7465   conversion_rate
+00004930: 3a20 666c 6f61 7420 3d20 7072 6f74 6f2e  : float = proto.
+00004940: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00004950: 726f 746f 2e44 4f55 424c 452c 0a20 2020  roto.DOUBLE,.   
+00004960: 2020 2020 206e 756d 6265 723d 3238 2c0a       number=28,.
+00004970: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00004980: 3d54 7275 652c 0a20 2020 2029 0a0a 0a63  =True,.    )...c
+00004990: 6c61 7373 2050 726f 6475 6374 5669 6577  lass ProductView
+000049a0: 2870 726f 746f 2e4d 6573 7361 6765 293a  (proto.Message):
+000049b0: 0a20 2020 2072 2222 2246 6965 6c64 7320  .    r"""Fields 
+000049c0: 6176 6169 6c61 626c 6520 666f 7220 7175  available for qu
+000049d0: 6572 7920 696e 2060 6070 726f 6475 6374  ery in ``product
+000049e0: 5f76 6965 7760 6020 7461 626c 652e 0a0a  _view`` table...
+000049f0: 2020 2020 5072 6f64 7563 7473 2069 6e20      Products in 
+00004a00: 7468 6520 6375 7272 656e 7420 696e 7665  the current inve
+00004a10: 6e74 6f72 792e 2050 726f 6475 6374 7320  ntory. Products 
+00004a20: 696e 2074 6869 7320 7461 626c 6520 6172  in this table ar
+00004a30: 6520 7468 650a 2020 2020 7361 6d65 2061  e the.    same a
+00004a40: 7320 696e 2050 726f 6475 6374 7320 7375  s in Products su
+00004a50: 622d 4150 4920 6275 7420 6e6f 7420 616c  b-API but not al
+00004a60: 6c20 7072 6f64 7563 7420 6174 7472 6962  l product attrib
+00004a70: 7574 6573 2066 726f 6d0a 2020 2020 5072  utes from.    Pr
+00004a80: 6f64 7563 7473 2073 7562 2d41 5049 2061  oducts sub-API a
+00004a90: 7265 2061 7661 696c 6162 6c65 2066 6f72  re available for
+00004aa0: 2071 7565 7279 2069 6e20 7468 6973 2074   query in this t
+00004ab0: 6162 6c65 2e20 496e 2063 6f6e 7472 6173  able. In contras
+00004ac0: 740a 2020 2020 746f 2050 726f 6475 6374  t.    to Product
+00004ad0: 7320 7375 622d 4150 492c 2074 6869 7320  s sub-API, this 
+00004ae0: 7461 626c 6520 616c 6c6f 7773 2074 6f20  table allows to 
+00004af0: 6669 6c74 6572 2074 6865 2072 6574 7572  filter the retur
+00004b00: 6e65 6420 6c69 7374 0a20 2020 206f 6620  ned list.    of 
+00004b10: 7072 6f64 7563 7473 2062 7920 7072 6f64  products by prod
+00004b20: 7563 7420 6174 7472 6962 7574 6573 2e20  uct attributes. 
+00004b30: 546f 2072 6574 7269 6576 6520 6120 7369  To retrieve a si
+00004b40: 6e67 6c65 2070 726f 6475 6374 2062 790a  ngle product by.
+00004b50: 2020 2020 6060 6964 6060 206f 7220 6c69      ``id`` or li
+00004b60: 7374 2061 6c6c 2070 726f 6475 6374 732c  st all products,
+00004b70: 2050 726f 6475 6374 7320 7375 622d 4150   Products sub-AP
+00004b80: 4920 7368 6f75 6c64 2062 6520 7573 6564  I should be used
+00004b90: 2e0a 0a20 2020 2056 616c 7565 7320 6172  ...    Values ar
+00004ba0: 6520 6f6e 6c79 2073 6574 2066 6f72 2066  e only set for f
+00004bb0: 6965 6c64 7320 7265 7175 6573 7465 6420  ields requested 
+00004bc0: 6578 706c 6963 6974 6c79 2069 6e20 7468  explicitly in th
+00004bd0: 6520 7265 7175 6573 7427 730a 2020 2020  e request's.    
+00004be0: 7365 6172 6368 2071 7565 7279 2e0a 0a0a  search query....
+00004bf0: 2020 2020 2e2e 205f 6f6e 656f 663a 2068      .. _oneof: h
+00004c00: 7474 7073 3a2f 2f70 726f 746f 2d70 6c75  ttps://proto-plu
+00004c10: 732d 7079 7468 6f6e 2e72 6561 6474 6865  s-python.readthe
+00004c20: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+00004c30: 652f 6669 656c 6473 2e68 746d 6c23 6f6e  e/fields.html#on
+00004c40: 656f 6673 2d6d 7574 7561 6c6c 792d 6578  eofs-mutually-ex
+00004c50: 636c 7573 6976 652d 6669 656c 6473 0a0a  clusive-fields..
+00004c60: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
+00004c70: 2020 2020 2020 2020 6964 2028 7374 7229          id (str)
+00004c80: 3a0a 2020 2020 2020 2020 2020 2020 5245  :.            RE
+00004c90: 5354 2049 4420 6f66 2074 6865 2070 726f  ST ID of the pro
+00004ca0: 6475 6374 2c20 696e 2074 6865 2066 6f72  duct, in the for
+00004cb0: 6d20 6f66 0a20 2020 2020 2020 2020 2020  m of.           
+00004cc0: 2060 6063 6861 6e6e 656c 7e6c 616e 6775   ``channel~langu
+00004cd0: 6167 6543 6f64 657e 6665 6564 4c61 6265  ageCode~feedLabe
+00004ce0: 6c7e 6f66 6665 7249 6460 602e 204d 6572  l~offerId``. Mer
+00004cf0: 6368 616e 7420 4150 490a 2020 2020 2020  chant API.      
+00004d00: 2020 2020 2020 6d65 7468 6f64 7320 7468        methods th
+00004d10: 6174 206f 7065 7261 7465 206f 6e20 7072  at operate on pr
+00004d20: 6f64 7563 7473 2074 616b 6520 7468 6973  oducts take this
+00004d30: 2061 7320 7468 6569 7220 6060 6e61 6d65   as their ``name
+00004d40: 6060 0a20 2020 2020 2020 2020 2020 2070  ``.            p
+00004d50: 6172 616d 6574 6572 2e0a 0a20 2020 2020  arameter...     
+00004d60: 2020 2020 2020 2052 6571 7569 7265 6420         Required 
+00004d70: 696e 2074 6865 2060 6053 454c 4543 5460  in the ``SELECT`
+00004d80: 6020 636c 6175 7365 2e0a 0a20 2020 2020  ` clause...     
+00004d90: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
+00004da0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
+00004db0: 2060 6f6e 656f 6660 5f20 6060 5f69 6460   `oneof`_ ``_id`
+00004dc0: 602e 0a20 2020 2020 2020 2063 6861 6e6e  `..        chann
+00004dd0: 656c 2028 676f 6f67 6c65 2e73 686f 7070  el (google.shopp
+00004de0: 696e 672e 7479 7065 2e74 7970 6573 2e43  ing.type.types.C
+00004df0: 6861 6e6e 656c 2e43 6861 6e6e 656c 456e  hannel.ChannelEn
+00004e00: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
+00004e10: 2043 6861 6e6e 656c 206f 6620 7468 6520   Channel of the 
+00004e20: 7072 6f64 7563 742e 2043 616e 2062 6520  product. Can be 
+00004e30: 6060 4f4e 4c49 4e45 6060 206f 7220 6060  ``ONLINE`` or ``
+00004e40: 4c4f 4341 4c60 602e 0a0a 2020 2020 2020  LOCAL``...      
+00004e50: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+00004e60: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+00004e70: 606f 6e65 6f66 605f 2060 605f 6368 616e  `oneof`_ ``_chan
+00004e80: 6e65 6c60 602e 0a20 2020 2020 2020 206c  nel``..        l
+00004e90: 616e 6775 6167 655f 636f 6465 2028 7374  anguage_code (st
+00004ea0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00004eb0: 4c61 6e67 7561 6765 2063 6f64 6520 6f66  Language code of
+00004ec0: 2074 6865 2070 726f 6475 6374 2069 6e20   the product in 
+00004ed0: 4243 5020 3437 0a20 2020 2020 2020 2020  BCP 47.         
+00004ee0: 2020 2066 6f72 6d61 742e 0a0a 2020 2020     format...    
+00004ef0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+00004f00: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+00004f10: 6620 606f 6e65 6f66 605f 2060 605f 6c61  f `oneof`_ ``_la
+00004f20: 6e67 7561 6765 5f63 6f64 6560 602e 0a20  nguage_code``.. 
+00004f30: 2020 2020 2020 2066 6565 645f 6c61 6265         feed_labe
+00004f40: 6c20 2873 7472 293a 0a20 2020 2020 2020  l (str):.       
+00004f50: 2020 2020 2046 6565 6420 6c61 6265 6c20       Feed label 
+00004f60: 6f66 2074 6865 2070 726f 6475 6374 2e0a  of the product..
+00004f70: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00004f80: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+00004f90: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+00004fa0: 6060 5f66 6565 645f 6c61 6265 6c60 602e  ``_feed_label``.
+00004fb0: 0a20 2020 2020 2020 206f 6666 6572 5f69  .        offer_i
+00004fc0: 6420 2873 7472 293a 0a20 2020 2020 2020  d (str):.       
+00004fd0: 2020 2020 204d 6572 6368 616e 742d 7072       Merchant-pr
+00004fe0: 6f76 6964 6564 2069 6420 6f66 2074 6865  ovided id of the
+00004ff0: 2070 726f 6475 6374 2e0a 0a20 2020 2020   product...     
+00005000: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
+00005010: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
+00005020: 2060 6f6e 656f 6660 5f20 6060 5f6f 6666   `oneof`_ ``_off
+00005030: 6572 5f69 6460 602e 0a20 2020 2020 2020  er_id``..       
+00005040: 2074 6974 6c65 2028 7374 7229 3a0a 2020   title (str):.  
+00005050: 2020 2020 2020 2020 2020 5469 746c 6520            Title 
+00005060: 6f66 2074 6865 2070 726f 6475 6374 2e0a  of the product..
+00005070: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00005080: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+00005090: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+000050a0: 6060 5f74 6974 6c65 6060 2e0a 2020 2020  ``_title``..    
+000050b0: 2020 2020 6272 616e 6420 2873 7472 293a      brand (str):
+000050c0: 0a20 2020 2020 2020 2020 2020 2042 7261  .            Bra
+000050d0: 6e64 206f 6620 7468 6520 7072 6f64 7563  nd of the produc
+000050e0: 742e 0a0a 2020 2020 2020 2020 2020 2020  t...            
+000050f0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+00005100: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+00005110: 605f 2060 605f 6272 616e 6460 602e 0a20  `_ ``_brand``.. 
+00005120: 2020 2020 2020 2063 6174 6567 6f72 795f         category_
+00005130: 6c31 2028 7374 7229 3a0a 2020 2020 2020  l1 (str):.      
+00005140: 2020 2020 2020 5072 6f64 7563 7420 6361        Product ca
+00005150: 7465 676f 7279 2028 3173 7420 6c65 7665  tegory (1st leve
+00005160: 6c29 2069 6e20 6047 6f6f 676c 6527 7320  l) in `Google's 
+00005170: 7072 6f64 7563 740a 2020 2020 2020 2020  product.        
+00005180: 2020 2020 7461 786f 6e6f 6d79 203c 6874      taxonomy <ht
+00005190: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
+000051a0: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
+000051b0: 7473 2f61 6e73 7765 722f 3633 3234 3433  ts/answer/632443
+000051c0: 363e 605f 5f2e 0a0a 2020 2020 2020 2020  6>`__...        
+000051d0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+000051e0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+000051f0: 6e65 6f66 605f 2060 605f 6361 7465 676f  neof`_ ``_catego
+00005200: 7279 5f6c 3160 602e 0a20 2020 2020 2020  ry_l1``..       
+00005210: 2063 6174 6567 6f72 795f 6c32 2028 7374   category_l2 (st
+00005220: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00005230: 5072 6f64 7563 7420 6361 7465 676f 7279  Product category
+00005240: 2028 326e 6420 6c65 7665 6c29 2069 6e20   (2nd level) in 
+00005250: 6047 6f6f 676c 6527 7320 7072 6f64 7563  `Google's produc
+00005260: 740a 2020 2020 2020 2020 2020 2020 7461  t.            ta
+00005270: 786f 6e6f 6d79 203c 6874 7470 733a 2f2f  xonomy <https://
+00005280: 7375 7070 6f72 742e 676f 6f67 6c65 2e63  support.google.c
+00005290: 6f6d 2f6d 6572 6368 616e 7473 2f61 6e73  om/merchants/ans
+000052a0: 7765 722f 3633 3234 3433 363e 605f 5f2e  wer/6324436>`__.
+000052b0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+000052c0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+000052d0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+000052e0: 2060 605f 6361 7465 676f 7279 5f6c 3260   ``_category_l2`
+000052f0: 602e 0a20 2020 2020 2020 2063 6174 6567  `..        categ
+00005300: 6f72 795f 6c33 2028 7374 7229 3a0a 2020  ory_l3 (str):.  
+00005310: 2020 2020 2020 2020 2020 5072 6f64 7563            Produc
+00005320: 7420 6361 7465 676f 7279 2028 3372 6420  t category (3rd 
+00005330: 6c65 7665 6c29 2069 6e20 6047 6f6f 676c  level) in `Googl
+00005340: 6527 7320 7072 6f64 7563 740a 2020 2020  e's product.    
+00005350: 2020 2020 2020 2020 7461 786f 6e6f 6d79          taxonomy
+00005360: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
+00005370: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
+00005380: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
+00005390: 3234 3433 363e 605f 5f2e 0a0a 2020 2020  24436>`__...    
+000053a0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+000053b0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+000053c0: 6620 606f 6e65 6f66 605f 2060 605f 6361  f `oneof`_ ``_ca
+000053d0: 7465 676f 7279 5f6c 3360 602e 0a20 2020  tegory_l3``..   
+000053e0: 2020 2020 2063 6174 6567 6f72 795f 6c34       category_l4
+000053f0: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+00005400: 2020 2020 5072 6f64 7563 7420 6361 7465      Product cate
+00005410: 676f 7279 2028 3474 6820 6c65 7665 6c29  gory (4th level)
+00005420: 2069 6e20 6047 6f6f 676c 6527 7320 7072   in `Google's pr
+00005430: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
+00005440: 2020 7461 786f 6e6f 6d79 203c 6874 7470    taxonomy <http
+00005450: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
+00005460: 6c65 2e63 6f6d 2f6d 6572 6368 616e 7473  le.com/merchants
+00005470: 2f61 6e73 7765 722f 3633 3234 3433 363e  /answer/6324436>
+00005480: 605f 5f2e 0a0a 2020 2020 2020 2020 2020  `__...          
+00005490: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+000054a0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+000054b0: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
+000054c0: 5f6c 3460 602e 0a20 2020 2020 2020 2063  _l4``..        c
+000054d0: 6174 6567 6f72 795f 6c35 2028 7374 7229  ategory_l5 (str)
+000054e0: 3a0a 2020 2020 2020 2020 2020 2020 5072  :.            Pr
+000054f0: 6f64 7563 7420 6361 7465 676f 7279 2028  oduct category (
+00005500: 3574 6820 6c65 7665 6c29 2069 6e20 6047  5th level) in `G
+00005510: 6f6f 676c 6527 7320 7072 6f64 7563 740a  oogle's product.
+00005520: 2020 2020 2020 2020 2020 2020 7461 786f              taxo
+00005530: 6e6f 6d79 203c 6874 7470 733a 2f2f 7375  nomy <https://su
+00005540: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
+00005550: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
+00005560: 722f 3633 3234 3433 363e 605f 5f2e 0a0a  r/6324436>`__...
+00005570: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00005580: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00005590: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+000055a0: 605f 6361 7465 676f 7279 5f6c 3560 602e  `_category_l5``.
+000055b0: 0a20 2020 2020 2020 2070 726f 6475 6374  .        product
+000055c0: 5f74 7970 655f 6c31 2028 7374 7229 3a0a  _type_l1 (str):.
+000055d0: 2020 2020 2020 2020 2020 2020 5072 6f64              Prod
+000055e0: 7563 7420 7479 7065 2028 3173 7420 6c65  uct type (1st le
+000055f0: 7665 6c29 2069 6e20 6d65 7263 6861 6e74  vel) in merchant
+00005600: 2773 206f 776e 2060 7072 6f64 7563 740a  's own `product.
+00005610: 2020 2020 2020 2020 2020 2020 7461 786f              taxo
+00005620: 6e6f 6d79 203c 6874 7470 733a 2f2f 7375  nomy <https://su
+00005630: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
+00005640: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
+00005650: 722f 3633 3234 3430 363e 605f 5f2e 0a0a  r/6324406>`__...
+00005660: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00005670: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00005680: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+00005690: 605f 7072 6f64 7563 745f 7479 7065 5f6c  `_product_type_l
+000056a0: 3160 602e 0a20 2020 2020 2020 2070 726f  1``..        pro
+000056b0: 6475 6374 5f74 7970 655f 6c32 2028 7374  duct_type_l2 (st
+000056c0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000056d0: 5072 6f64 7563 7420 7479 7065 2028 326e  Product type (2n
+000056e0: 6420 6c65 7665 6c29 2069 6e20 6d65 7263  d level) in merc
+000056f0: 6861 6e74 2773 206f 776e 2060 7072 6f64  hant's own `prod
+00005700: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
+00005710: 7461 786f 6e6f 6d79 203c 6874 7470 733a  taxonomy <https:
+00005720: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
+00005730: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
+00005740: 6e73 7765 722f 3633 3234 3430 363e 605f  nswer/6324406>`_
+00005750: 5f2e 0a0a 2020 2020 2020 2020 2020 2020  _...            
+00005760: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+00005770: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+00005780: 605f 2060 605f 7072 6f64 7563 745f 7479  `_ ``_product_ty
+00005790: 7065 5f6c 3260 602e 0a20 2020 2020 2020  pe_l2``..       
+000057a0: 2070 726f 6475 6374 5f74 7970 655f 6c33   product_type_l3
+000057b0: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+000057c0: 2020 2020 5072 6f64 7563 7420 7479 7065      Product type
+000057d0: 2028 3372 6420 6c65 7665 6c29 2069 6e20   (3rd level) in 
+000057e0: 6d65 7263 6861 6e74 2773 206f 776e 2060  merchant's own `
+000057f0: 7072 6f64 7563 740a 2020 2020 2020 2020  product.        
+00005800: 2020 2020 7461 786f 6e6f 6d79 203c 6874      taxonomy <ht
+00005810: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
+00005820: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
+00005830: 7473 2f61 6e73 7765 722f 3633 3234 3430  ts/answer/632440
+00005840: 363e 605f 5f2e 0a0a 2020 2020 2020 2020  6>`__...        
+00005850: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+00005860: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+00005870: 6e65 6f66 605f 2060 605f 7072 6f64 7563  neof`_ ``_produc
+00005880: 745f 7479 7065 5f6c 3360 602e 0a20 2020  t_type_l3``..   
+00005890: 2020 2020 2070 726f 6475 6374 5f74 7970       product_typ
+000058a0: 655f 6c34 2028 7374 7229 3a0a 2020 2020  e_l4 (str):.    
+000058b0: 2020 2020 2020 2020 5072 6f64 7563 7420          Product 
+000058c0: 7479 7065 2028 3474 6820 6c65 7665 6c29  type (4th level)
+000058d0: 2069 6e20 6d65 7263 6861 6e74 2773 206f   in merchant's o
+000058e0: 776e 2060 7072 6f64 7563 740a 2020 2020  wn `product.    
+000058f0: 2020 2020 2020 2020 7461 786f 6e6f 6d79          taxonomy
+00005900: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
+00005910: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
+00005920: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
+00005930: 3234 3430 363e 605f 5f2e 0a0a 2020 2020  24406>`__...    
+00005940: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+00005950: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+00005960: 6620 606f 6e65 6f66 605f 2060 605f 7072  f `oneof`_ ``_pr
+00005970: 6f64 7563 745f 7479 7065 5f6c 3460 602e  oduct_type_l4``.
+00005980: 0a20 2020 2020 2020 2070 726f 6475 6374  .        product
+00005990: 5f74 7970 655f 6c35 2028 7374 7229 3a0a  _type_l5 (str):.
+000059a0: 2020 2020 2020 2020 2020 2020 5072 6f64              Prod
+000059b0: 7563 7420 7479 7065 2028 3574 6820 6c65  uct type (5th le
+000059c0: 7665 6c29 2069 6e20 6d65 7263 6861 6e74  vel) in merchant
+000059d0: 2773 206f 776e 2060 7072 6f64 7563 740a  's own `product.
+000059e0: 2020 2020 2020 2020 2020 2020 7461 786f              taxo
+000059f0: 6e6f 6d79 203c 6874 7470 733a 2f2f 7375  nomy <https://su
+00005a00: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
+00005a10: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
+00005a20: 722f 3633 3234 3430 363e 605f 5f2e 0a0a  r/6324406>`__...
+00005a30: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00005a40: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00005a50: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+00005a60: 605f 7072 6f64 7563 745f 7479 7065 5f6c  `_product_type_l
+00005a70: 3560 602e 0a20 2020 2020 2020 2070 7269  5``..        pri
+00005a80: 6365 2028 676f 6f67 6c65 2e73 686f 7070  ce (google.shopp
+00005a90: 696e 672e 7479 7065 2e74 7970 6573 2e50  ing.type.types.P
+00005aa0: 7269 6365 293a 0a20 2020 2020 2020 2020  rice):.         
+00005ab0: 2020 2050 726f 6475 6374 2070 7269 6365     Product price
+00005ac0: 2e20 4162 7365 6e74 2069 6620 7468 6520  . Absent if the 
+00005ad0: 696e 666f 726d 6174 696f 6e0a 2020 2020  information.    
+00005ae0: 2020 2020 2020 2020 6162 6f75 7420 7468          about th
+00005af0: 6520 7072 6963 6520 6f66 2074 6865 2070  e price of the p
+00005b00: 726f 6475 6374 2069 7320 6e6f 7420 6176  roduct is not av
+00005b10: 6169 6c61 626c 652e 0a20 2020 2020 2020  ailable..       
+00005b20: 2063 6f6e 6469 7469 6f6e 2028 7374 7229   condition (str)
+00005b30: 3a0a 2020 2020 2020 2020 2020 2020 6043  :.            `C
+00005b40: 6f6e 6469 7469 6f6e 203c 6874 7470 733a  ondition <https:
+00005b50: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
+00005b60: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
+00005b70: 6e73 7765 722f 3633 3234 3436 393e 605f  nswer/6324469>`_
+00005b80: 5f0a 2020 2020 2020 2020 2020 2020 6f66  _.            of
+00005b90: 2074 6865 2070 726f 6475 6374 2e0a 0a20   the product... 
+00005ba0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+00005bb0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+00005bc0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+00005bd0: 5f63 6f6e 6469 7469 6f6e 6060 2e0a 2020  _condition``..  
+00005be0: 2020 2020 2020 6176 6169 6c61 6269 6c69        availabili
+00005bf0: 7479 2028 7374 7229 3a0a 2020 2020 2020  ty (str):.      
+00005c00: 2020 2020 2020 6041 7661 696c 6162 696c        `Availabil
+00005c10: 6974 7920 3c68 7474 7073 3a2f 2f73 7570  ity <https://sup
+00005c20: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
+00005c30: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
+00005c40: 2f36 3332 3434 3438 3e60 5f5f 0a20 2020  /6324448>`__.   
+00005c50: 2020 2020 2020 2020 206f 6620 7468 6520           of the 
+00005c60: 7072 6f64 7563 742e 0a0a 2020 2020 2020  product...      
+00005c70: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+00005c80: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+00005c90: 606f 6e65 6f66 605f 2060 605f 6176 6169  `oneof`_ ``_avai
+00005ca0: 6c61 6269 6c69 7479 6060 2e0a 2020 2020  lability``..    
+00005cb0: 2020 2020 7368 6970 7069 6e67 5f6c 6162      shipping_lab
+00005cc0: 656c 2028 7374 7229 3a0a 2020 2020 2020  el (str):.      
+00005cd0: 2020 2020 2020 4e6f 726d 616c 697a 6564        Normalized
+00005ce0: 2060 7368 6970 7069 6e67 0a20 2020 2020   `shipping.     
+00005cf0: 2020 2020 2020 206c 6162 656c 203c 6874         label <ht
+00005d00: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
+00005d10: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
+00005d20: 7473 2f61 6e73 7765 722f 3633 3234 3530  ts/answer/632450
+00005d30: 343e 605f 5f0a 2020 2020 2020 2020 2020  4>`__.          
+00005d40: 2020 7370 6563 6966 6965 6420 696e 2074    specified in t
+00005d50: 6865 2064 6174 6120 736f 7572 6365 2e0a  he data source..
+00005d60: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00005d70: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+00005d80: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+00005d90: 6060 5f73 6869 7070 696e 675f 6c61 6265  ``_shipping_labe
+00005da0: 6c60 602e 0a20 2020 2020 2020 2067 7469  l``..        gti
+00005db0: 6e20 284d 7574 6162 6c65 5365 7175 656e  n (MutableSequen
+00005dc0: 6365 5b73 7472 5d29 3a0a 2020 2020 2020  ce[str]):.      
+00005dd0: 2020 2020 2020 4c69 7374 206f 6620 476c        List of Gl
+00005de0: 6f62 616c 2054 7261 6465 2049 7465 6d20  obal Trade Item 
+00005df0: 4e75 6d62 6572 7320 2847 5449 4e73 2920  Numbers (GTINs) 
+00005e00: 6f66 0a20 2020 2020 2020 2020 2020 2074  of.            t
+00005e10: 6865 2070 726f 6475 6374 2e0a 2020 2020  he product..    
+00005e20: 2020 2020 6974 656d 5f67 726f 7570 5f69      item_group_i
+00005e30: 6420 2873 7472 293a 0a20 2020 2020 2020  d (str):.       
+00005e40: 2020 2020 2049 7465 6d20 6772 6f75 7020       Item group 
+00005e50: 6964 2070 726f 7669 6465 6420 6279 2074  id provided by t
+00005e60: 6865 206d 6572 6368 616e 7420 666f 720a  he merchant for.
+00005e70: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
+00005e80: 7069 6e67 2076 6172 6961 6e74 7320 746f  ping variants to
+00005e90: 6765 7468 6572 2e0a 0a20 2020 2020 2020  gether...       
+00005ea0: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+00005eb0: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+00005ec0: 6f6e 656f 6660 5f20 6060 5f69 7465 6d5f  oneof`_ ``_item_
+00005ed0: 6772 6f75 705f 6964 6060 2e0a 2020 2020  group_id``..    
+00005ee0: 2020 2020 7468 756d 626e 6169 6c5f 6c69      thumbnail_li
+00005ef0: 6e6b 2028 7374 7229 3a0a 2020 2020 2020  nk (str):.      
+00005f00: 2020 2020 2020 4c69 6e6b 2074 6f20 7468        Link to th
+00005f10: 6520 7072 6f63 6573 7365 6420 696d 6167  e processed imag
+00005f20: 6520 6f66 2074 6865 2070 726f 6475 6374  e of the product
+00005f30: 2c0a 2020 2020 2020 2020 2020 2020 686f  ,.            ho
+00005f40: 7374 6564 206f 6e20 7468 6520 476f 6f67  sted on the Goog
+00005f50: 6c65 2069 6e66 7261 7374 7275 6374 7572  le infrastructur
+00005f60: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
+00005f70: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+00005f80: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+00005f90: 605f 2060 605f 7468 756d 626e 6169 6c5f  `_ ``_thumbnail_
+00005fa0: 6c69 6e6b 6060 2e0a 2020 2020 2020 2020  link``..        
+00005fb0: 6372 6561 7469 6f6e 5f74 696d 6520 2867  creation_time (g
+00005fc0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e74  oogle.protobuf.t
+00005fd0: 696d 6573 7461 6d70 5f70 6232 2e54 696d  imestamp_pb2.Tim
+00005fe0: 6573 7461 6d70 293a 0a20 2020 2020 2020  estamp):.       
+00005ff0: 2020 2020 2054 6865 2074 696d 6520 7468       The time th
+00006000: 6520 6d65 7263 6861 6e74 2063 7265 6174  e merchant creat
+00006010: 6564 2074 6865 2070 726f 6475 6374 2069  ed the product i
+00006020: 6e0a 2020 2020 2020 2020 2020 2020 7469  n.            ti
+00006030: 6d65 7374 616d 7020 7365 636f 6e64 732e  mestamp seconds.
+00006040: 0a20 2020 2020 2020 2065 7870 6972 6174  .        expirat
+00006050: 696f 6e5f 6461 7465 2028 676f 6f67 6c65  ion_date (google
+00006060: 2e74 7970 652e 6461 7465 5f70 6232 2e44  .type.date_pb2.D
+00006070: 6174 6529 3a0a 2020 2020 2020 2020 2020  ate):.          
+00006080: 2020 4578 7069 7261 7469 6f6e 2064 6174    Expiration dat
+00006090: 6520 666f 7220 7468 6520 7072 6f64 7563  e for the produc
+000060a0: 742c 2073 7065 6369 6669 6564 206f 6e0a  t, specified on.
+000060b0: 2020 2020 2020 2020 2020 2020 696e 7365              inse
+000060c0: 7274 696f 6e2e 0a20 2020 2020 2020 2061  rtion..        a
+000060d0: 6767 7265 6761 7465 645f 7265 706f 7274  ggregated_report
+000060e0: 696e 675f 636f 6e74 6578 745f 7374 6174  ing_context_stat
+000060f0: 7573 2028 676f 6f67 6c65 2e73 686f 7070  us (google.shopp
+00006100: 696e 672e 6d65 7263 6861 6e74 5f72 6570  ing.merchant_rep
+00006110: 6f72 7473 5f76 3162 6574 612e 7479 7065  orts_v1beta.type
+00006120: 732e 5072 6f64 7563 7456 6965 772e 4167  s.ProductView.Ag
+00006130: 6772 6567 6174 6564 5265 706f 7274 696e  gregatedReportin
+00006140: 6743 6f6e 7465 7874 5374 6174 7573 293a  gContextStatus):
+00006150: 0a20 2020 2020 2020 2020 2020 2041 6767  .            Agg
+00006160: 7265 6761 7465 6420 7374 6174 7573 2e0a  regated status..
+00006170: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00006180: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+00006190: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+000061a0: 6060 5f61 6767 7265 6761 7465 645f 7265  ``_aggregated_re
+000061b0: 706f 7274 696e 675f 636f 6e74 6578 745f  porting_context_
+000061c0: 7374 6174 7573 6060 2e0a 2020 2020 2020  status``..      
+000061d0: 2020 6974 656d 5f69 7373 7565 7320 284d    item_issues (M
+000061e0: 7574 6162 6c65 5365 7175 656e 6365 5b67  utableSequence[g
+000061f0: 6f6f 676c 652e 7368 6f70 7069 6e67 2e6d  oogle.shopping.m
+00006200: 6572 6368 616e 745f 7265 706f 7274 735f  erchant_reports_
+00006210: 7631 6265 7461 2e74 7970 6573 2e50 726f  v1beta.types.Pro
+00006220: 6475 6374 5669 6577 2e49 7465 6d49 7373  ductView.ItemIss
+00006230: 7565 5d29 3a0a 2020 2020 2020 2020 2020  ue]):.          
+00006240: 2020 4c69 7374 206f 6620 6974 656d 2069    List of item i
+00006250: 7373 7565 7320 666f 7220 7468 6520 7072  ssues for the pr
+00006260: 6f64 7563 742e 0a0a 2020 2020 2020 2020  oduct...        
+00006270: 2020 2020 2a2a 5468 6973 2066 6965 6c64      **This field
+00006280: 2063 616e 6e6f 7420 6265 2075 7365 6420   cannot be used 
+00006290: 666f 7220 736f 7274 696e 6720 7468 6520  for sorting the 
+000062a0: 7265 7375 6c74 732e 2a2a 0a0a 2020 2020  results.**..    
+000062b0: 2020 2020 2020 2020 2a2a 4f6e 6c79 2073          **Only s
+000062c0: 656c 6563 7465 6420 6174 7472 6962 7574  elected attribut
+000062d0: 6573 206f 6620 7468 6973 2066 6965 6c64  es of this field
+000062e0: 2028 666f 7220 6578 616d 706c 652c 0a20   (for example,. 
+000062f0: 2020 2020 2020 2020 2020 2060 6069 7465             ``ite
+00006300: 6d5f 6973 7375 6573 2e73 6576 6572 6974  m_issues.severit
+00006310: 792e 6167 6772 6567 6174 6564 5f73 6576  y.aggregated_sev
+00006320: 6572 6974 7960 6029 2063 616e 2062 6520  erity``) can be 
+00006330: 7573 6564 0a20 2020 2020 2020 2020 2020  used.           
+00006340: 2066 6f72 2066 696c 7465 7269 6e67 2074   for filtering t
+00006350: 6865 2072 6573 756c 7473 2e2a 2a0a 2020  he results.**.  
+00006360: 2020 2020 2020 636c 6963 6b5f 706f 7465        click_pote
+00006370: 6e74 6961 6c20 2867 6f6f 676c 652e 7368  ntial (google.sh
+00006380: 6f70 7069 6e67 2e6d 6572 6368 616e 745f  opping.merchant_
+00006390: 7265 706f 7274 735f 7631 6265 7461 2e74  reports_v1beta.t
+000063a0: 7970 6573 2e50 726f 6475 6374 5669 6577  ypes.ProductView
+000063b0: 2e43 6c69 636b 506f 7465 6e74 6961 6c29  .ClickPotential)
+000063c0: 3a0a 2020 2020 2020 2020 2020 2020 4573  :.            Es
+000063d0: 7469 6d61 7465 6420 7065 7266 6f72 6d61  timated performa
+000063e0: 6e63 6520 706f 7465 6e74 6961 6c20 636f  nce potential co
+000063f0: 6d70 6172 6564 2074 6f0a 2020 2020 2020  mpared to.      
+00006400: 2020 2020 2020 6869 6768 6573 7420 7065        highest pe
+00006410: 7266 6f72 6d69 6e67 2070 726f 6475 6374  rforming product
+00006420: 7320 6f66 2074 6865 206d 6572 6368 616e  s of the merchan
+00006430: 742e 0a20 2020 2020 2020 2063 6c69 636b  t..        click
+00006440: 5f70 6f74 656e 7469 616c 5f72 616e 6b20  _potential_rank 
+00006450: 2869 6e74 293a 0a20 2020 2020 2020 2020  (int):.         
+00006460: 2020 2052 616e 6b20 6f66 2074 6865 2070     Rank of the p
+00006470: 726f 6475 6374 2062 6173 6564 206f 6e20  roduct based on 
+00006480: 6974 7320 636c 6963 6b20 706f 7465 6e74  its click potent
+00006490: 6961 6c2e 2041 2070 726f 6475 6374 0a20  ial. A product. 
+000064a0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+000064b0: 6060 636c 6963 6b5f 706f 7465 6e74 6961  ``click_potentia
+000064c0: 6c5f 7261 6e6b 6060 2031 2068 6173 2074  l_rank`` 1 has t
+000064d0: 6865 2068 6967 6865 7374 2063 6c69 636b  he highest click
+000064e0: 0a20 2020 2020 2020 2020 2020 2070 6f74  .            pot
+000064f0: 656e 7469 616c 2061 6d6f 6e67 2074 6865  ential among the
+00006500: 206d 6572 6368 616e 7427 7320 7072 6f64   merchant's prod
+00006510: 7563 7473 2074 6861 7420 6675 6c66 696c  ucts that fulfil
+00006520: 6c20 7468 650a 2020 2020 2020 2020 2020  l the.          
+00006530: 2020 7365 6172 6368 2071 7565 7279 2063    search query c
+00006540: 6f6e 6469 7469 6f6e 732e 0a0a 2020 2020  onditions...    
+00006550: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+00006560: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+00006570: 6620 606f 6e65 6f66 605f 2060 605f 636c  f `oneof`_ ``_cl
+00006580: 6963 6b5f 706f 7465 6e74 6961 6c5f 7261  ick_potential_ra
+00006590: 6e6b 6060 2e0a 2020 2020 2222 220a 0a20  nk``..    """.. 
+000065a0: 2020 2063 6c61 7373 2041 6767 7265 6761     class Aggrega
+000065b0: 7465 6452 6570 6f72 7469 6e67 436f 6e74  tedReportingCont
+000065c0: 6578 7453 7461 7475 7328 7072 6f74 6f2e  extStatus(proto.
+000065d0: 456e 756d 293a 0a20 2020 2020 2020 2072  Enum):.        r
+000065e0: 2222 2253 7461 7475 7320 6f66 2074 6865  """Status of the
+000065f0: 2070 726f 6475 6374 2061 6767 7265 6761   product aggrega
+00006600: 7465 6420 666f 7220 616c 6c20 7265 706f  ted for all repo
+00006610: 7274 696e 6720 636f 6e74 6578 7473 2e0a  rting contexts..
+00006620: 0a20 2020 2020 2020 2048 6572 6527 7320  .        Here's 
+00006630: 616e 2065 7861 6d70 6c65 206f 6620 686f  an example of ho
+00006640: 7720 7468 6520 6167 6772 6567 6174 6564  w the aggregated
+00006650: 2073 7461 7475 7320 6973 2063 6f6d 7075   status is compu
+00006660: 7465 643a 0a0a 2020 2020 2020 2020 6060  ted:..        ``
+00006670: 600a 2020 2020 2020 2020 4672 6565 206c  `.        Free l
+00006680: 6973 7469 6e67 7320 5c7c 2053 686f 7070  istings \| Shopp
+00006690: 696e 6720 6164 7320 5c7c 2053 7461 7475  ing ads \| Statu
+000066a0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+000066b0: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
+000066c0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
+000066d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000066e0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2041  ------.        A
+000066f0: 7070 726f 7665 6420 5c7c 2041 7070 726f  pproved \| Appro
+00006700: 7665 6420 5c7c 2045 4c49 4749 424c 4520  ved \| ELIGIBLE 
+00006710: 4170 7072 6f76 6564 205c 7c20 5065 6e64  Approved \| Pend
+00006720: 696e 6720 5c7c 2045 4c49 4749 424c 450a  ing \| ELIGIBLE.
+00006730: 2020 2020 2020 2020 4170 7072 6f76 6564          Approved
+00006740: 205c 7c20 4469 7361 7070 726f 7665 6420   \| Disapproved 
+00006750: 5c7c 2045 4c49 4749 424c 455f 4c49 4d49  \| ELIGIBLE_LIMI
+00006760: 5445 4420 5065 6e64 696e 6720 5c7c 2050  TED Pending \| P
+00006770: 656e 6469 6e67 205c 7c0a 2020 2020 2020  ending \|.      
+00006780: 2020 5045 4e44 494e 4720 4469 7361 7070    PENDING Disapp
+00006790: 726f 7665 6420 5c7c 2044 6973 6170 7072  roved \| Disappr
+000067a0: 6f76 6564 205c 7c20 4e4f 545f 454c 4947  oved \| NOT_ELIG
+000067b0: 4942 4c45 5f4f 525f 4449 5341 5050 524f  IBLE_OR_DISAPPRO
+000067c0: 5645 440a 2020 2020 2020 2020 6060 600a  VED.        ```.
+000067d0: 0a20 2020 2020 2020 2056 616c 7565 733a  .        Values:
+000067e0: 0a20 2020 2020 2020 2020 2020 2041 4747  .            AGG
+000067f0: 5245 4741 5445 445f 5245 504f 5254 494e  REGATED_REPORTIN
+00006800: 475f 434f 4e54 4558 545f 5354 4154 5553  G_CONTEXT_STATUS
+00006810: 5f55 4e53 5045 4349 4649 4544 2028 3029  _UNSPECIFIED (0)
+00006820: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006830: 2020 4e6f 7420 7370 6563 6966 6965 642e    Not specified.
+00006840: 0a20 2020 2020 2020 2020 2020 204e 4f54  .            NOT
+00006850: 5f45 4c49 4749 424c 455f 4f52 5f44 4953  _ELIGIBLE_OR_DIS
+00006860: 4150 5052 4f56 4544 2028 3129 3a0a 2020  APPROVED (1):.  
+00006870: 2020 2020 2020 2020 2020 2020 2020 5072                Pr
+00006880: 6f64 7563 7420 6973 206e 6f74 2065 6c69  oduct is not eli
+00006890: 6769 626c 6520 6f72 2069 7320 6469 7361  gible or is disa
+000068a0: 7070 726f 7665 6420 666f 720a 2020 2020  pproved for.    
+000068b0: 2020 2020 2020 2020 2020 2020 616c 6c20              all 
+000068c0: 7265 706f 7274 696e 6720 636f 6e74 6578  reporting contex
+000068d0: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
+000068e0: 5045 4e44 494e 4720 2832 293a 0a20 2020  PENDING (2):.   
+000068f0: 2020 2020 2020 2020 2020 2020 2050 726f               Pro
+00006900: 6475 6374 2773 2073 7461 7475 7320 6973  duct's status is
+00006910: 2070 656e 6469 6e67 2069 6e20 616c 6c20   pending in all 
+00006920: 7265 706f 7274 696e 670a 2020 2020 2020  reporting.      
+00006930: 2020 2020 2020 2020 2020 636f 6e74 6578            contex
+00006940: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
+00006950: 454c 4947 4942 4c45 5f4c 494d 4954 4544  ELIGIBLE_LIMITED
+00006960: 2028 3329 3a0a 2020 2020 2020 2020 2020   (3):.          
+00006970: 2020 2020 2020 5072 6f64 7563 7420 6973        Product is
+00006980: 2065 6c69 6769 626c 6520 666f 7220 736f   eligible for so
+00006990: 6d65 2028 6275 7420 6e6f 7420 616c 6c29  me (but not all)
+000069a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000069b0: 2072 6570 6f72 7469 6e67 2063 6f6e 7465   reporting conte
+000069c0: 7874 732e 0a20 2020 2020 2020 2020 2020  xts..           
+000069d0: 2045 4c49 4749 424c 4520 2834 293a 0a20   ELIGIBLE (4):. 
+000069e0: 2020 2020 2020 2020 2020 2020 2020 2050                 P
+000069f0: 726f 6475 6374 2069 7320 656c 6967 6962  roduct is eligib
+00006a00: 6c65 2066 6f72 2061 6c6c 2072 6570 6f72  le for all repor
+00006a10: 7469 6e67 0a20 2020 2020 2020 2020 2020  ting.           
+00006a20: 2020 2020 2063 6f6e 7465 7874 732e 0a20       contexts.. 
+00006a30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006a40: 2020 2041 4747 5245 4741 5445 445f 5245     AGGREGATED_RE
+00006a50: 504f 5254 494e 475f 434f 4e54 4558 545f  PORTING_CONTEXT_
+00006a60: 5354 4154 5553 5f55 4e53 5045 4349 4649  STATUS_UNSPECIFI
+00006a70: 4544 203d 2030 0a20 2020 2020 2020 204e  ED = 0.        N
+00006a80: 4f54 5f45 4c49 4749 424c 455f 4f52 5f44  OT_ELIGIBLE_OR_D
+00006a90: 4953 4150 5052 4f56 4544 203d 2031 0a20  ISAPPROVED = 1. 
+00006aa0: 2020 2020 2020 2050 454e 4449 4e47 203d         PENDING =
+00006ab0: 2032 0a20 2020 2020 2020 2045 4c49 4749   2.        ELIGI
+00006ac0: 424c 455f 4c49 4d49 5445 4420 3d20 330a  BLE_LIMITED = 3.
+00006ad0: 2020 2020 2020 2020 454c 4947 4942 4c45          ELIGIBLE
+00006ae0: 203d 2034 0a0a 2020 2020 636c 6173 7320   = 4..    class 
+00006af0: 436c 6963 6b50 6f74 656e 7469 616c 2870  ClickPotential(p
+00006b00: 726f 746f 2e45 6e75 6d29 3a0a 2020 2020  roto.Enum):.    
+00006b10: 2020 2020 7222 2222 4120 7072 6f64 7563      r"""A produc
+00006b20: 7427 7320 6063 6c69 636b 0a20 2020 2020  t's `click.     
+00006b30: 2020 2070 6f74 656e 7469 616c 203c 6874     potential <ht
+00006b40: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
+00006b50: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
+00006b60: 7473 2f61 6e73 7765 722f 3138 3834 3838  ts/answer/188488
+00006b70: 3e60 5f5f 0a20 2020 2020 2020 2065 7374  >`__.        est
+00006b80: 696d 6174 6573 2069 7473 2070 6572 666f  imates its perfo
+00006b90: 726d 616e 6365 2070 6f74 656e 7469 616c  rmance potential
+00006ba0: 2063 6f6d 7061 7265 6420 746f 2068 6967   compared to hig
+00006bb0: 6865 7374 2070 6572 666f 726d 696e 670a  hest performing.
+00006bc0: 2020 2020 2020 2020 7072 6f64 7563 7473          products
+00006bd0: 206f 6620 7468 6520 6d65 7263 6861 6e74   of the merchant
+00006be0: 2e20 436c 6963 6b20 706f 7465 6e74 6961  . Click potentia
+00006bf0: 6c20 6f66 2061 2070 726f 6475 6374 2068  l of a product h
+00006c00: 656c 7073 0a20 2020 2020 2020 206d 6572  elps.        mer
+00006c10: 6368 616e 7473 2074 6f20 7072 696f 7269  chants to priori
+00006c20: 7469 7a65 2077 6869 6368 2070 726f 6475  tize which produ
+00006c30: 6374 7320 746f 2066 6978 2061 6e64 2068  cts to fix and h
+00006c40: 656c 7073 2074 6865 6d0a 2020 2020 2020  elps them.      
+00006c50: 2020 756e 6465 7273 7461 6e64 2068 6f77    understand how
+00006c60: 2070 726f 6475 6374 7320 6172 6520 7065   products are pe
+00006c70: 7266 6f72 6d69 6e67 2061 6761 696e 7374  rforming against
+00006c80: 2074 6865 6972 2070 6f74 656e 7469 616c   their potential
+00006c90: 2e0a 0a20 2020 2020 2020 2056 616c 7565  ...        Value
+00006ca0: 733a 0a20 2020 2020 2020 2020 2020 2043  s:.            C
+00006cb0: 4c49 434b 5f50 4f54 454e 5449 414c 5f55  LICK_POTENTIAL_U
+00006cc0: 4e53 5045 4349 4649 4544 2028 3029 3a0a  NSPECIFIED (0):.
+00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ce0: 556e 6b6e 6f77 6e20 7072 6564 6963 7465  Unknown predicte
+00006cf0: 6420 636c 6963 6b73 2069 6d70 6163 742e  d clicks impact.
+00006d00: 0a20 2020 2020 2020 2020 2020 204c 4f57  .            LOW
+00006d10: 2028 3129 3a0a 2020 2020 2020 2020 2020   (1):.          
+00006d20: 2020 2020 2020 506f 7465 6e74 6961 6c20        Potential 
+00006d30: 746f 2072 6563 6569 7665 2061 206c 6f77  to receive a low
+00006d40: 206e 756d 6265 7220 6f66 2063 6c69 636b   number of click
+00006d50: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00006d60: 2020 636f 6d70 6172 6564 2074 6f20 7468    compared to th
+00006d70: 6520 6869 6768 6573 7420 7065 7266 6f72  e highest perfor
+00006d80: 6d69 6e67 2070 726f 6475 6374 7320 6f66  ming products of
+00006d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006da0: 2074 6865 206d 6572 6368 616e 742e 0a20   the merchant.. 
+00006db0: 2020 2020 2020 2020 2020 204d 4544 4955             MEDIU
+00006dc0: 4d20 2832 293a 0a20 2020 2020 2020 2020  M (2):.         
+00006dd0: 2020 2020 2020 2050 6f74 656e 7469 616c         Potential
+00006de0: 2074 6f20 7265 6365 6976 6520 6120 6d6f   to receive a mo
+00006df0: 6465 7261 7465 206e 756d 6265 7220 6f66  derate number of
+00006e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006e10: 2063 6c69 636b 7320 636f 6d70 6172 6564   clicks compared
+00006e20: 2074 6f20 7468 6520 6869 6768 6573 7420   to the highest 
+00006e30: 7065 7266 6f72 6d69 6e67 0a20 2020 2020  performing.     
+00006e40: 2020 2020 2020 2020 2020 2070 726f 6475             produ
+00006e50: 6374 7320 6f66 2074 6865 206d 6572 6368  cts of the merch
+00006e60: 616e 742e 0a20 2020 2020 2020 2020 2020  ant..           
+00006e70: 2048 4947 4820 2833 293a 0a20 2020 2020   HIGH (3):.     
+00006e80: 2020 2020 2020 2020 2020 2050 6f74 656e             Poten
+00006e90: 7469 616c 2074 6f20 7265 6365 6976 6520  tial to receive 
+00006ea0: 6120 7369 6d69 6c61 7220 6e75 6d62 6572  a similar number
+00006eb0: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
+00006ec0: 2020 2020 636c 6963 6b73 2061 7320 7468      clicks as th
+00006ed0: 6520 6869 6768 6573 7420 7065 7266 6f72  e highest perfor
+00006ee0: 6d69 6e67 2070 726f 6475 6374 7320 6f66  ming products of
+00006ef0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00006f00: 2020 2020 206d 6572 6368 616e 742e 0a20       merchant.. 
+00006f10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006f20: 2020 2043 4c49 434b 5f50 4f54 454e 5449     CLICK_POTENTI
+00006f30: 414c 5f55 4e53 5045 4349 4649 4544 203d  AL_UNSPECIFIED =
+00006f40: 2030 0a20 2020 2020 2020 204c 4f57 203d   0.        LOW =
+00006f50: 2031 0a20 2020 2020 2020 204d 4544 4955   1.        MEDIU
+00006f60: 4d20 3d20 320a 2020 2020 2020 2020 4849  M = 2.        HI
+00006f70: 4748 203d 2033 0a0a 2020 2020 636c 6173  GH = 3..    clas
+00006f80: 7320 4974 656d 4973 7375 6528 7072 6f74  s ItemIssue(prot
+00006f90: 6f2e 4d65 7373 6167 6529 3a0a 2020 2020  o.Message):.    
+00006fa0: 2020 2020 7222 2222 4974 656d 2069 7373      r"""Item iss
+00006fb0: 7565 2061 7373 6f63 6961 7465 6420 7769  ue associated wi
+00006fc0: 7468 2074 6865 2070 726f 6475 6374 2e0a  th the product..
+00006fd0: 0a20 2020 2020 2020 202e 2e20 5f6f 6e65  .        .. _one
+00006fe0: 6f66 3a20 6874 7470 733a 2f2f 7072 6f74  of: https://prot
+00006ff0: 6f2d 706c 7573 2d70 7974 686f 6e2e 7265  o-plus-python.re
+00007000: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00007010: 7374 6162 6c65 2f66 6965 6c64 732e 6874  stable/fields.ht
+00007020: 6d6c 236f 6e65 6f66 732d 6d75 7475 616c  ml#oneofs-mutual
+00007030: 6c79 2d65 7863 6c75 7369 7665 2d66 6965  ly-exclusive-fie
+00007040: 6c64 730a 0a20 2020 2020 2020 2041 7474  lds..        Att
+00007050: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
+00007060: 2020 2020 2074 7970 655f 2028 676f 6f67       type_ (goog
+00007070: 6c65 2e73 686f 7070 696e 672e 6d65 7263  le.shopping.merc
+00007080: 6861 6e74 5f72 6570 6f72 7473 5f76 3162  hant_reports_v1b
+00007090: 6574 612e 7479 7065 732e 5072 6f64 7563  eta.types.Produc
+000070a0: 7456 6965 772e 4974 656d 4973 7375 652e  tView.ItemIssue.
+000070b0: 4974 656d 4973 7375 6554 7970 6529 3a0a  ItemIssueType):.
+000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070d0: 4974 656d 2069 7373 7565 2074 7970 652e  Item issue type.
+000070e0: 0a20 2020 2020 2020 2020 2020 2073 6576  .            sev
+000070f0: 6572 6974 7920 2867 6f6f 676c 652e 7368  erity (google.sh
+00007100: 6f70 7069 6e67 2e6d 6572 6368 616e 745f  opping.merchant_
+00007110: 7265 706f 7274 735f 7631 6265 7461 2e74  reports_v1beta.t
+00007120: 7970 6573 2e50 726f 6475 6374 5669 6577  ypes.ProductView
+00007130: 2e49 7465 6d49 7373 7565 2e49 7465 6d49  .ItemIssue.ItemI
+00007140: 7373 7565 5365 7665 7269 7479 293a 0a20  ssueSeverity):. 
+00007150: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+00007160: 7465 6d20 6973 7375 6520 7365 7665 7269  tem issue severi
+00007170: 7479 2e0a 2020 2020 2020 2020 2020 2020  ty..            
+00007180: 7265 736f 6c75 7469 6f6e 2028 676f 6f67  resolution (goog
+00007190: 6c65 2e73 686f 7070 696e 672e 6d65 7263  le.shopping.merc
+000071a0: 6861 6e74 5f72 6570 6f72 7473 5f76 3162  hant_reports_v1b
+000071b0: 6574 612e 7479 7065 732e 5072 6f64 7563  eta.types.Produc
+000071c0: 7456 6965 772e 4974 656d 4973 7375 652e  tView.ItemIssue.
+000071d0: 4974 656d 4973 7375 6552 6573 6f6c 7574  ItemIssueResolut
+000071e0: 696f 6e29 3a0a 2020 2020 2020 2020 2020  ion):.          
+000071f0: 2020 2020 2020 4974 656d 2069 7373 7565        Item issue
+00007200: 2072 6573 6f6c 7574 696f 6e2e 0a0a 2020   resolution...  
+00007210: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+00007220: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+00007230: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+00007240: 2060 605f 7265 736f 6c75 7469 6f6e 6060   ``_resolution``
+00007250: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+00007260: 2020 2020 2020 2063 6c61 7373 2049 7465         class Ite
+00007270: 6d49 7373 7565 5265 736f 6c75 7469 6f6e  mIssueResolution
+00007280: 2870 726f 746f 2e45 6e75 6d29 3a0a 2020  (proto.Enum):.  
+00007290: 2020 2020 2020 2020 2020 7222 2222 486f            r"""Ho
+000072a0: 7720 746f 2072 6573 6f6c 7665 2074 6865  w to resolve the
+000072b0: 2069 7373 7565 2e0a 0a20 2020 2020 2020   issue...       
+000072c0: 2020 2020 2056 616c 7565 733a 0a20 2020       Values:.   
+000072d0: 2020 2020 2020 2020 2020 2020 2049 5445               ITE
+000072e0: 4d5f 4953 5355 455f 5245 534f 4c55 5449  M_ISSUE_RESOLUTI
+000072f0: 4f4e 5f55 4e53 5045 4349 4649 4544 2028  ON_UNSPECIFIED (
+00007300: 3029 3a0a 2020 2020 2020 2020 2020 2020  0):.            
+00007310: 2020 2020 2020 2020 4e6f 7420 7370 6563          Not spec
+00007320: 6966 6965 642e 0a20 2020 2020 2020 2020  ified..         
+00007330: 2020 2020 2020 204d 4552 4348 414e 545f         MERCHANT_
+00007340: 4143 5449 4f4e 2028 3129 3a0a 2020 2020  ACTION (1):.    
+00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007360: 5468 6520 6d65 7263 6861 6e74 2068 6173  The merchant has
+00007370: 2074 6f20 6669 7820 7468 6520 6973 7375   to fix the issu
+00007380: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
+00007390: 2020 2050 454e 4449 4e47 5f50 524f 4345     PENDING_PROCE
+000073a0: 5353 494e 4720 2832 293a 0a20 2020 2020  SSING (2):.     
+000073b0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+000073c0: 6865 2069 7373 7565 2077 696c 6c20 6265  he issue will be
+000073d0: 2072 6573 6f6c 7665 6420 6175 746f 6d61   resolved automa
+000073e0: 7469 6361 6c6c 7920 2866 6f72 0a20 2020  tically (for.   
+000073f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007400: 2065 7861 6d70 6c65 2c20 696d 6167 6520   example, image 
+00007410: 6372 6177 6c29 206f 7220 7468 726f 7567  crawl) or throug
+00007420: 6820 6120 476f 6f67 6c65 0a20 2020 2020  h a Google.     
+00007430: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00007440: 6576 6965 772e 204e 6f20 6d65 7263 6861  eview. No mercha
+00007450: 6e74 2061 6374 696f 6e20 6973 2072 6571  nt action is req
+00007460: 7569 7265 6420 6e6f 772e 0a20 2020 2020  uired now..     
+00007470: 2020 2020 2020 2020 2020 2020 2020 2052                 R
+00007480: 6573 6f6c 7574 696f 6e20 6d69 6768 7420  esolution might 
+00007490: 6c65 6164 2074 6f20 616e 6f74 6865 7220  lead to another 
+000074a0: 6973 7375 6520 2866 6f72 0a20 2020 2020  issue (for.     
+000074b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000074c0: 7861 6d70 6c65 2c20 6966 2063 7261 776c  xample, if crawl
+000074d0: 2066 6169 6c73 292e 0a20 2020 2020 2020   fails)..       
+000074e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000074f0: 2020 2020 2049 5445 4d5f 4953 5355 455f       ITEM_ISSUE_
+00007500: 5245 534f 4c55 5449 4f4e 5f55 4e53 5045  RESOLUTION_UNSPE
+00007510: 4349 4649 4544 203d 2030 0a20 2020 2020  CIFIED = 0.     
+00007520: 2020 2020 2020 204d 4552 4348 414e 545f         MERCHANT_
+00007530: 4143 5449 4f4e 203d 2031 0a20 2020 2020  ACTION = 1.     
+00007540: 2020 2020 2020 2050 454e 4449 4e47 5f50         PENDING_P
+00007550: 524f 4345 5353 494e 4720 3d20 320a 0a20  ROCESSING = 2.. 
+00007560: 2020 2020 2020 2063 6c61 7373 2049 7465         class Ite
+00007570: 6d49 7373 7565 5479 7065 2870 726f 746f  mIssueType(proto
+00007580: 2e4d 6573 7361 6765 293a 0a20 2020 2020  .Message):.     
+00007590: 2020 2020 2020 2072 2222 2249 7373 7565         r"""Issue
+000075a0: 2074 7970 652e 0a0a 2020 2020 2020 2020   type...        
+000075b0: 2020 2020 2e2e 205f 6f6e 656f 663a 2068      .. _oneof: h
+000075c0: 7474 7073 3a2f 2f70 726f 746f 2d70 6c75  ttps://proto-plu
+000075d0: 732d 7079 7468 6f6e 2e72 6561 6474 6865  s-python.readthe
+000075e0: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+000075f0: 652f 6669 656c 6473 2e68 746d 6c23 6f6e  e/fields.html#on
+00007600: 656f 6673 2d6d 7574 7561 6c6c 792d 6578  eofs-mutually-ex
+00007610: 636c 7573 6976 652d 6669 656c 6473 0a0a  clusive-fields..
+00007620: 2020 2020 2020 2020 2020 2020 4174 7472              Attr
+00007630: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
+00007640: 2020 2020 2020 2020 636f 6465 2028 7374          code (st
+00007650: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00007660: 2020 2020 2020 2020 4572 726f 7220 636f          Error co
+00007670: 6465 206f 6620 7468 6520 6973 7375 652c  de of the issue,
+00007680: 2065 7175 6976 616c 656e 7420 746f 2074   equivalent to t
+00007690: 6865 2060 6063 6f64 6560 6020 6f66 0a20  he ``code`` of. 
+000076a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076b0: 2020 2060 5072 6f64 7563 740a 2020 2020     `Product.    
+000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076d0: 6973 7375 6573 203c 6874 7470 733a 2f2f  issues <https://
+000076e0: 6465 7665 6c6f 7065 7273 2e67 6f6f 676c  developers.googl
+000076f0: 652e 636f 6d2f 7368 6f70 7069 6e67 2d63  e.com/shopping-c
+00007700: 6f6e 7465 6e74 2f67 7569 6465 732f 7072  ontent/guides/pr
+00007710: 6f64 7563 742d 6973 7375 6573 3e60 5f5f  oduct-issues>`__
+00007720: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
+00007730: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
+00007740: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
+00007750: 2060 6f6e 656f 6660 5f20 6060 5f63 6f64   `oneof`_ ``_cod
+00007760: 6560 602e 0a20 2020 2020 2020 2020 2020  e``..           
+00007770: 2020 2020 2063 616e 6f6e 6963 616c 5f61       canonical_a
+00007780: 7474 7269 6275 7465 2028 7374 7229 3a0a  ttribute (str):.
+00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077a0: 2020 2020 4361 6e6f 6e69 6361 6c20 6174      Canonical at
+000077b0: 7472 6962 7574 6520 6e61 6d65 2066 6f72  tribute name for
+000077c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000077d0: 2020 2020 2061 7474 7269 6275 7465 2d73       attribute-s
+000077e0: 7065 6369 6669 6320 6973 7375 6573 2e0a  pecific issues..
+000077f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007800: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+00007810: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+00007820: 6f6e 656f 6660 5f20 6060 5f63 616e 6f6e  oneof`_ ``_canon
+00007830: 6963 616c 5f61 7474 7269 6275 7465 6060  ical_attribute``
+00007840: 2e0a 2020 2020 2020 2020 2020 2020 2222  ..            ""
+00007850: 220a 0a20 2020 2020 2020 2020 2020 2063  "..            c
+00007860: 6f64 653a 2073 7472 203d 2070 726f 746f  ode: str = proto
+00007870: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00007880: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+00007890: 5249 4e47 2c0a 2020 2020 2020 2020 2020  RING,.          
+000078a0: 2020 2020 2020 6e75 6d62 6572 3d31 2c0a        number=1,.
+000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078c0: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+000078d0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000078e0: 2020 2020 2020 2020 2063 616e 6f6e 6963           canonic
+000078f0: 616c 5f61 7474 7269 6275 7465 3a20 7374  al_attribute: st
+00007900: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00007910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007920: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+00007930: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00007940: 756d 6265 723d 322c 0a20 2020 2020 2020  umber=2,.       
+00007950: 2020 2020 2020 2020 206f 7074 696f 6e61           optiona
+00007960: 6c3d 5472 7565 2c0a 2020 2020 2020 2020  l=True,.        
+00007970: 2020 2020 290a 0a20 2020 2020 2020 2063      )..        c
+00007980: 6c61 7373 2049 7465 6d49 7373 7565 5365  lass ItemIssueSe
+00007990: 7665 7269 7479 2870 726f 746f 2e4d 6573  verity(proto.Mes
+000079a0: 7361 6765 293a 0a20 2020 2020 2020 2020  sage):.         
+000079b0: 2020 2072 2222 2248 6f77 2074 6865 2069     r"""How the i
+000079c0: 7373 7565 2061 6666 6563 7473 2074 6865  ssue affects the
+000079d0: 2073 6572 7669 6e67 206f 6620 7468 6520   serving of the 
+000079e0: 7072 6f64 7563 742e 0a0a 2020 2020 2020  product...      
+000079f0: 2020 2020 2020 2e2e 205f 6f6e 656f 663a        .. _oneof:
+00007a00: 2068 7474 7073 3a2f 2f70 726f 746f 2d70   https://proto-p
+00007a10: 6c75 732d 7079 7468 6f6e 2e72 6561 6474  lus-python.readt
+00007a20: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
+00007a30: 626c 652f 6669 656c 6473 2e68 746d 6c23  ble/fields.html#
+00007a40: 6f6e 656f 6673 2d6d 7574 7561 6c6c 792d  oneofs-mutually-
+00007a50: 6578 636c 7573 6976 652d 6669 656c 6473  exclusive-fields
+00007a60: 0a0a 2020 2020 2020 2020 2020 2020 4174  ..            At
+00007a70: 7472 6962 7574 6573 3a0a 2020 2020 2020  tributes:.      
+00007a80: 2020 2020 2020 2020 2020 7365 7665 7269            severi
+00007a90: 7479 5f70 6572 5f72 6570 6f72 7469 6e67  ty_per_reporting
+00007aa0: 5f63 6f6e 7465 7874 2028 4d75 7461 626c  _context (Mutabl
+00007ab0: 6553 6571 7565 6e63 655b 676f 6f67 6c65  eSequence[google
+00007ac0: 2e73 686f 7070 696e 672e 6d65 7263 6861  .shopping.mercha
+00007ad0: 6e74 5f72 6570 6f72 7473 5f76 3162 6574  nt_reports_v1bet
+00007ae0: 612e 7479 7065 732e 5072 6f64 7563 7456  a.types.ProductV
+00007af0: 6965 772e 4974 656d 4973 7375 652e 4974  iew.ItemIssue.It
+00007b00: 656d 4973 7375 6553 6576 6572 6974 792e  emIssueSeverity.
+00007b10: 4973 7375 6553 6576 6572 6974 7950 6572  IssueSeverityPer
+00007b20: 5265 706f 7274 696e 6743 6f6e 7465 7874  ReportingContext
+00007b30: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+00007b40: 2020 2020 2020 2020 4973 7375 6520 7365          Issue se
+00007b50: 7665 7269 7479 2070 6572 2072 6570 6f72  verity per repor
+00007b60: 7469 6e67 2063 6f6e 7465 7874 2e0a 2020  ting context..  
+00007b70: 2020 2020 2020 2020 2020 2020 2020 6167                ag
+00007b80: 6772 6567 6174 6564 5f73 6576 6572 6974  gregated_severit
+00007b90: 7920 2867 6f6f 676c 652e 7368 6f70 7069  y (google.shoppi
+00007ba0: 6e67 2e6d 6572 6368 616e 745f 7265 706f  ng.merchant_repo
+00007bb0: 7274 735f 7631 6265 7461 2e74 7970 6573  rts_v1beta.types
+00007bc0: 2e50 726f 6475 6374 5669 6577 2e49 7465  .ProductView.Ite
+00007bd0: 6d49 7373 7565 2e49 7465 6d49 7373 7565  mIssue.ItemIssue
+00007be0: 5365 7665 7269 7479 2e41 6767 7265 6761  Severity.Aggrega
+00007bf0: 7465 6449 7373 7565 5365 7665 7269 7479  tedIssueSeverity
+00007c00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00007c10: 2020 2020 2020 2041 6767 7265 6761 7465         Aggregate
+00007c20: 6420 7365 7665 7269 7479 206f 6620 7468  d severity of th
+00007c30: 6520 6973 7375 6520 666f 7220 616c 6c20  e issue for all 
+00007c40: 7265 706f 7274 696e 6720 636f 6e74 6578  reporting contex
+00007c50: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
+00007c60: 2020 2020 2020 2069 7420 6166 6665 6374         it affect
+00007c70: 732e 0a0a 2020 2020 2020 2020 2020 2020  s...            
+00007c80: 2020 2020 2020 2020 2a2a 5468 6973 2066          **This f
+00007c90: 6965 6c64 2063 616e 2062 6520 7573 6564  ield can be used
+00007ca0: 2066 6f72 2066 696c 7465 7269 6e67 2074   for filtering t
+00007cb0: 6865 2072 6573 756c 7473 2e2a 2a0a 0a20  he results.**.. 
+00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cd0: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+00007ce0: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+00007cf0: 656f 6660 5f20 6060 5f61 6767 7265 6761  eof`_ ``_aggrega
+00007d00: 7465 645f 7365 7665 7269 7479 6060 2e0a  ted_severity``..
+00007d10: 2020 2020 2020 2020 2020 2020 2222 220a              """.
+00007d20: 0a20 2020 2020 2020 2020 2020 2063 6c61  .            cla
+00007d30: 7373 2041 6767 7265 6761 7465 6449 7373  ss AggregatedIss
+00007d40: 7565 5365 7665 7269 7479 2870 726f 746f  ueSeverity(proto
+00007d50: 2e45 6e75 6d29 3a0a 2020 2020 2020 2020  .Enum):.        
+00007d60: 2020 2020 2020 2020 7222 2222 4973 7375          r"""Issu
+00007d70: 6520 7365 7665 7269 7479 2061 6767 7265  e severity aggre
+00007d80: 6761 7465 6420 666f 7220 616c 6c20 7265  gated for all re
+00007d90: 706f 7274 696e 6720 636f 6e74 6578 7473  porting contexts
+00007da0: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
+00007db0: 2020 2056 616c 7565 733a 0a20 2020 2020     Values:.     
+00007dc0: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+00007dd0: 4747 5245 4741 5445 445f 4953 5355 455f  GGREGATED_ISSUE_
+00007de0: 5345 5645 5249 5459 5f55 4e53 5045 4349  SEVERITY_UNSPECI
+00007df0: 4649 4544 2028 3029 3a0a 2020 2020 2020  FIED (0):.      
+00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e10: 2020 4e6f 7420 7370 6563 6966 6965 642e    Not specified.
+00007e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007e30: 2020 2020 2044 4953 4150 5052 4f56 4544       DISAPPROVED
+00007e40: 2028 3129 3a0a 2020 2020 2020 2020 2020   (1):.          
+00007e50: 2020 2020 2020 2020 2020 2020 2020 4973                Is
+00007e60: 7375 6520 6469 7361 7070 726f 7665 7320  sue disapproves 
+00007e70: 7468 6520 7072 6f64 7563 7420 696e 2061  the product in a
+00007e80: 7420 6c65 6173 7420 6f6e 650a 2020 2020  t least one.    
+00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ea0: 2020 2020 7265 706f 7274 696e 6720 636f      reporting co
+00007eb0: 6e74 6578 742e 0a20 2020 2020 2020 2020  ntext..         
+00007ec0: 2020 2020 2020 2020 2020 2044 454d 4f54             DEMOT
+00007ed0: 4544 2028 3229 3a0a 2020 2020 2020 2020  ED (2):.        
+00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ef0: 4973 7375 6520 6465 6d6f 7465 7320 7468  Issue demotes th
+00007f00: 6520 7072 6f64 7563 7420 696e 2061 6c6c  e product in all
+00007f10: 2072 6570 6f72 7469 6e67 0a20 2020 2020   reporting.     
+00007f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f30: 2020 2063 6f6e 7465 7874 7320 6974 2061     contexts it a
+00007f40: 6666 6563 7473 2e0a 2020 2020 2020 2020  ffects..        
+00007f50: 2020 2020 2020 2020 2020 2020 5045 4e44              PEND
+00007f60: 494e 4720 2833 293a 0a20 2020 2020 2020  ING (3):.       
+00007f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f80: 2049 7373 7565 2072 6573 6f6c 7574 696f   Issue resolutio
+00007f90: 6e20 6973 2060 6050 454e 4449 4e47 5f50  n is ``PENDING_P
+00007fa0: 524f 4345 5353 494e 4760 602e 0a20 2020  ROCESSING``..   
+00007fb0: 2020 2020 2020 2020 2020 2020 2022 2222               """
+00007fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007fd0: 2041 4747 5245 4741 5445 445f 4953 5355   AGGREGATED_ISSU
+00007fe0: 455f 5345 5645 5249 5459 5f55 4e53 5045  E_SEVERITY_UNSPE
+00007ff0: 4349 4649 4544 203d 2030 0a20 2020 2020  CIFIED = 0.     
+00008000: 2020 2020 2020 2020 2020 2044 4953 4150             DISAP
+00008010: 5052 4f56 4544 203d 2031 0a20 2020 2020  PROVED = 1.     
+00008020: 2020 2020 2020 2020 2020 2044 454d 4f54             DEMOT
+00008030: 4544 203d 2032 0a20 2020 2020 2020 2020  ED = 2.         
+00008040: 2020 2020 2020 2050 454e 4449 4e47 203d         PENDING =
+00008050: 2033 0a0a 2020 2020 2020 2020 2020 2020   3..            
+00008060: 636c 6173 7320 4973 7375 6553 6576 6572  class IssueSever
+00008070: 6974 7950 6572 5265 706f 7274 696e 6743  ityPerReportingC
+00008080: 6f6e 7465 7874 2870 726f 746f 2e4d 6573  ontext(proto.Mes
+00008090: 7361 6765 293a 0a20 2020 2020 2020 2020  sage):.         
+000080a0: 2020 2020 2020 2072 2222 2249 7373 7565         r"""Issue
+000080b0: 2073 6576 6572 6974 7920 7065 7220 7265   severity per re
+000080c0: 706f 7274 696e 6720 636f 6e74 6578 742e  porting context.
+000080d0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000080e0: 2020 2e2e 205f 6f6e 656f 663a 2068 7474    .. _oneof: htt
+000080f0: 7073 3a2f 2f70 726f 746f 2d70 6c75 732d  ps://proto-plus-
+00008100: 7079 7468 6f6e 2e72 6561 6474 6865 646f  python.readthedo
+00008110: 6373 2e69 6f2f 656e 2f73 7461 626c 652f  cs.io/en/stable/
+00008120: 6669 656c 6473 2e68 746d 6c23 6f6e 656f  fields.html#oneo
+00008130: 6673 2d6d 7574 7561 6c6c 792d 6578 636c  fs-mutually-excl
+00008140: 7573 6976 652d 6669 656c 6473 0a0a 2020  usive-fields..  
+00008150: 2020 2020 2020 2020 2020 2020 2020 4174                At
+00008160: 7472 6962 7574 6573 3a0a 2020 2020 2020  tributes:.      
+00008170: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00008180: 706f 7274 696e 675f 636f 6e74 6578 7420  porting_context 
+00008190: 2867 6f6f 676c 652e 7368 6f70 7069 6e67  (google.shopping
+000081a0: 2e74 7970 652e 7479 7065 732e 5265 706f  .type.types.Repo
+000081b0: 7274 696e 6743 6f6e 7465 7874 2e52 6570  rtingContext.Rep
+000081c0: 6f72 7469 6e67 436f 6e74 6578 7445 6e75  ortingContextEnu
+000081d0: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
+000081e0: 2020 2020 2020 2020 2020 2020 5265 706f              Repo
+000081f0: 7274 696e 6720 636f 6e74 6578 7420 7468  rting context th
+00008200: 6520 6973 7375 6520 6170 706c 6965 7320  e issue applies 
+00008210: 746f 2e0a 0a20 2020 2020 2020 2020 2020  to...           
+00008220: 2020 2020 2020 2020 2020 2020 2054 6869               Thi
+00008230: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+00008240: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+00008250: 6060 5f72 6570 6f72 7469 6e67 5f63 6f6e  ``_reporting_con
+00008260: 7465 7874 6060 2e0a 2020 2020 2020 2020  text``..        
+00008270: 2020 2020 2020 2020 2020 2020 6469 7361              disa
+00008280: 7070 726f 7665 645f 636f 756e 7472 6965  pproved_countrie
+00008290: 7320 284d 7574 6162 6c65 5365 7175 656e  s (MutableSequen
+000082a0: 6365 5b73 7472 5d29 3a0a 2020 2020 2020  ce[str]):.      
+000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082c0: 2020 4c69 7374 206f 6620 6469 7361 7070    List of disapp
+000082d0: 726f 7665 6420 636f 756e 7472 6965 7320  roved countries 
+000082e0: 696e 2074 6865 0a20 2020 2020 2020 2020  in the.         
+000082f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00008300: 6570 6f72 7469 6e67 2063 6f6e 7465 7874  eporting context
+00008310: 2c20 7265 7072 6573 656e 7465 6420 696e  , represented in
+00008320: 2049 534f 2033 3136 360a 2020 2020 2020   ISO 3166.      
+00008330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008340: 2020 666f 726d 6174 2e0a 2020 2020 2020    format..      
+00008350: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00008360: 6d6f 7465 645f 636f 756e 7472 6965 7320  moted_countries 
+00008370: 284d 7574 6162 6c65 5365 7175 656e 6365  (MutableSequence
+00008380: 5b73 7472 5d29 3a0a 2020 2020 2020 2020  [str]):.        
+00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083a0: 4c69 7374 206f 6620 6465 6d6f 7465 6420  List of demoted 
+000083b0: 636f 756e 7472 6965 7320 696e 2074 6865  countries in the
+000083c0: 2072 6570 6f72 7469 6e67 0a20 2020 2020   reporting.     
+000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083e0: 2020 2063 6f6e 7465 7874 2c20 7265 7072     context, repr
+000083f0: 6573 656e 7465 6420 696e 2049 534f 2033  esented in ISO 3
+00008400: 3136 3620 666f 726d 6174 2e0a 2020 2020  166 format..    
+00008410: 2020 2020 2020 2020 2020 2020 2222 220a              """.
+00008420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008430: 2072 6570 6f72 7469 6e67 5f63 6f6e 7465   reporting_conte
+00008440: 7874 3a20 7479 7065 732e 5265 706f 7274  xt: types.Report
+00008450: 696e 6743 6f6e 7465 7874 2e52 6570 6f72  ingContext.Repor
+00008460: 7469 6e67 436f 6e74 6578 7445 6e75 6d20  tingContextEnum 
+00008470: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00008480: 2020 2020 2020 2020 7072 6f74 6f2e 4669          proto.Fi
+00008490: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
+000084a0: 2020 2020 2020 2020 2020 2020 2070 726f               pro
+000084b0: 746f 2e45 4e55 4d2c 0a20 2020 2020 2020  to.ENUM,.       
+000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084d0: 206e 756d 6265 723d 312c 0a20 2020 2020   number=1,.     
+000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084f0: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+00008500: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008510: 2020 2020 2020 2020 2020 656e 756d 3d74            enum=t
+00008520: 7970 6573 2e52 6570 6f72 7469 6e67 436f  ypes.ReportingCo
+00008530: 6e74 6578 742e 5265 706f 7274 696e 6743  ntext.ReportingC
+00008540: 6f6e 7465 7874 456e 756d 2c0a 2020 2020  ontextEnum,.    
+00008550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008560: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008570: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00008580: 2020 2020 6469 7361 7070 726f 7665 645f      disapproved_
+00008590: 636f 756e 7472 6965 733a 204d 7574 6162  countries: Mutab
+000085a0: 6c65 5365 7175 656e 6365 5b73 7472 5d20  leSequence[str] 
+000085b0: 3d20 7072 6f74 6f2e 5265 7065 6174 6564  = proto.Repeated
+000085c0: 4669 656c 6428 0a20 2020 2020 2020 2020  Field(.         
+000085d0: 2020 2020 2020 2020 2020 2070 726f 746f             proto
+000085e0: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
+000085f0: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00008600: 6265 723d 322c 0a20 2020 2020 2020 2020  ber=2,.         
+00008610: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00008620: 2020 2020 2020 2020 2064 656d 6f74 6564           demoted
+00008630: 5f63 6f75 6e74 7269 6573 3a20 4d75 7461  _countries: Muta
+00008640: 626c 6553 6571 7565 6e63 655b 7374 725d  bleSequence[str]
+00008650: 203d 2070 726f 746f 2e52 6570 6561 7465   = proto.Repeate
+00008660: 6446 6965 6c64 280a 2020 2020 2020 2020  dField(.        
+00008670: 2020 2020 2020 2020 2020 2020 7072 6f74              prot
+00008680: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
+00008690: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+000086a0: 6d62 6572 3d33 2c0a 2020 2020 2020 2020  mber=3,.        
+000086b0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000086c0: 2020 2020 2020 2073 6576 6572 6974 795f         severity_
+000086d0: 7065 725f 7265 706f 7274 696e 675f 636f  per_reporting_co
+000086e0: 6e74 6578 743a 204d 7574 6162 6c65 5365  ntext: MutableSe
+000086f0: 7175 656e 6365 5b0a 2020 2020 2020 2020  quence[.        
+00008700: 2020 2020 2020 2020 2250 726f 6475 6374          "Product
+00008710: 5669 6577 2e49 7465 6d49 7373 7565 2e49  View.ItemIssue.I
+00008720: 7465 6d49 7373 7565 5365 7665 7269 7479  temIssueSeverity
+00008730: 2e49 7373 7565 5365 7665 7269 7479 5065  .IssueSeverityPe
+00008740: 7252 6570 6f72 7469 6e67 436f 6e74 6578  rReportingContex
+00008750: 7422 0a20 2020 2020 2020 2020 2020 205d  t".            ]
+00008760: 203d 2070 726f 746f 2e52 6570 6561 7465   = proto.Repeate
+00008770: 6446 6965 6c64 280a 2020 2020 2020 2020  dField(.        
+00008780: 2020 2020 2020 2020 7072 6f74 6f2e 4d45          proto.ME
+00008790: 5353 4147 452c 0a20 2020 2020 2020 2020  SSAGE,.         
+000087a0: 2020 2020 2020 206e 756d 6265 723d 312c         number=1,
+000087b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000087c0: 206d 6573 7361 6765 3d22 5072 6f64 7563   message="Produc
+000087d0: 7456 6965 772e 4974 656d 4973 7375 652e  tView.ItemIssue.
+000087e0: 4974 656d 4973 7375 6553 6576 6572 6974  ItemIssueSeverit
+000087f0: 792e 4973 7375 6553 6576 6572 6974 7950  y.IssueSeverityP
+00008800: 6572 5265 706f 7274 696e 6743 6f6e 7465  erReportingConte
+00008810: 7874 222c 0a20 2020 2020 2020 2020 2020  xt",.           
+00008820: 2029 0a20 2020 2020 2020 2020 2020 2061   ).            a
+00008830: 6767 7265 6761 7465 645f 7365 7665 7269  ggregated_severi
+00008840: 7479 3a20 2250 726f 6475 6374 5669 6577  ty: "ProductView
+00008850: 2e49 7465 6d49 7373 7565 2e49 7465 6d49  .ItemIssue.ItemI
+00008860: 7373 7565 5365 7665 7269 7479 2e41 6767  ssueSeverity.Agg
+00008870: 7265 6761 7465 6449 7373 7565 5365 7665  regatedIssueSeve
+00008880: 7269 7479 2220 3d20 7072 6f74 6f2e 4669  rity" = proto.Fi
+00008890: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
+000088a0: 2020 2020 2070 726f 746f 2e45 4e55 4d2c       proto.ENUM,
+000088b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000088c0: 206e 756d 6265 723d 322c 0a20 2020 2020   number=2,.     
+000088d0: 2020 2020 2020 2020 2020 206f 7074 696f             optio
+000088e0: 6e61 6c3d 5472 7565 2c0a 2020 2020 2020  nal=True,.      
+000088f0: 2020 2020 2020 2020 2020 656e 756d 3d22            enum="
+00008900: 5072 6f64 7563 7456 6965 772e 4974 656d  ProductView.Item
+00008910: 4973 7375 652e 4974 656d 4973 7375 6553  Issue.ItemIssueS
+00008920: 6576 6572 6974 792e 4167 6772 6567 6174  everity.Aggregat
+00008930: 6564 4973 7375 6553 6576 6572 6974 7922  edIssueSeverity"
+00008940: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00008950: 0a20 2020 2020 2020 2074 7970 655f 3a20  .        type_: 
+00008960: 2250 726f 6475 6374 5669 6577 2e49 7465  "ProductView.Ite
+00008970: 6d49 7373 7565 2e49 7465 6d49 7373 7565  mIssue.ItemIssue
+00008980: 5479 7065 2220 3d20 7072 6f74 6f2e 4669  Type" = proto.Fi
+00008990: 656c 6428 0a20 2020 2020 2020 2020 2020  eld(.           
+000089a0: 2070 726f 746f 2e4d 4553 5341 4745 2c0a   proto.MESSAGE,.
+000089b0: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
+000089c0: 6572 3d31 2c0a 2020 2020 2020 2020 2020  er=1,.          
+000089d0: 2020 6d65 7373 6167 653d 2250 726f 6475    message="Produ
+000089e0: 6374 5669 6577 2e49 7465 6d49 7373 7565  ctView.ItemIssue
+000089f0: 2e49 7465 6d49 7373 7565 5479 7065 222c  .ItemIssueType",
+00008a00: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00008a10: 2020 2073 6576 6572 6974 793a 2022 5072     severity: "Pr
+00008a20: 6f64 7563 7456 6965 772e 4974 656d 4973  oductView.ItemIs
+00008a30: 7375 652e 4974 656d 4973 7375 6553 6576  sue.ItemIssueSev
+00008a40: 6572 6974 7922 203d 2070 726f 746f 2e46  erity" = proto.F
+00008a50: 6965 6c64 280a 2020 2020 2020 2020 2020  ield(.          
+00008a60: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
+00008a70: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+00008a80: 6265 723d 322c 0a20 2020 2020 2020 2020  ber=2,.         
+00008a90: 2020 206d 6573 7361 6765 3d22 5072 6f64     message="Prod
+00008aa0: 7563 7456 6965 772e 4974 656d 4973 7375  uctView.ItemIssu
+00008ab0: 652e 4974 656d 4973 7375 6553 6576 6572  e.ItemIssueSever
+00008ac0: 6974 7922 2c0a 2020 2020 2020 2020 290a  ity",.        ).
+00008ad0: 2020 2020 2020 2020 7265 736f 6c75 7469          resoluti
+00008ae0: 6f6e 3a20 2250 726f 6475 6374 5669 6577  on: "ProductView
+00008af0: 2e49 7465 6d49 7373 7565 2e49 7465 6d49  .ItemIssue.ItemI
+00008b00: 7373 7565 5265 736f 6c75 7469 6f6e 2220  ssueResolution" 
+00008b10: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00008b20: 2020 2020 2020 2020 2020 2070 726f 746f             proto
+00008b30: 2e45 4e55 4d2c 0a20 2020 2020 2020 2020  .ENUM,.         
+00008b40: 2020 206e 756d 6265 723d 332c 0a20 2020     number=3,.   
+00008b50: 2020 2020 2020 2020 206f 7074 696f 6e61           optiona
+00008b60: 6c3d 5472 7565 2c0a 2020 2020 2020 2020  l=True,.        
+00008b70: 2020 2020 656e 756d 3d22 5072 6f64 7563      enum="Produc
+00008b80: 7456 6965 772e 4974 656d 4973 7375 652e  tView.ItemIssue.
+00008b90: 4974 656d 4973 7375 6552 6573 6f6c 7574  ItemIssueResolut
+00008ba0: 696f 6e22 2c0a 2020 2020 2020 2020 290a  ion",.        ).
+00008bb0: 0a20 2020 2069 643a 2073 7472 203d 2070  .    id: str = p
+00008bc0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00008bd0: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+00008be0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00008bf0: 3d31 2c0a 2020 2020 2020 2020 6f70 7469  =1,.        opti
+00008c00: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+00008c10: 0a20 2020 2063 6861 6e6e 656c 3a20 7479  .    channel: ty
+00008c20: 7065 732e 4368 616e 6e65 6c2e 4368 616e  pes.Channel.Chan
+00008c30: 6e65 6c45 6e75 6d20 3d20 7072 6f74 6f2e  nelEnum = proto.
+00008c40: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00008c50: 726f 746f 2e45 4e55 4d2c 0a20 2020 2020  roto.ENUM,.     
+00008c60: 2020 206e 756d 6265 723d 3238 2c0a 2020     number=28,.  
+00008c70: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+00008c80: 7275 652c 0a20 2020 2020 2020 2065 6e75  rue,.        enu
+00008c90: 6d3d 7479 7065 732e 4368 616e 6e65 6c2e  m=types.Channel.
+00008ca0: 4368 616e 6e65 6c45 6e75 6d2c 0a20 2020  ChannelEnum,.   
+00008cb0: 2029 0a20 2020 206c 616e 6775 6167 655f   ).    language_
+00008cc0: 636f 6465 3a20 7374 7220 3d20 7072 6f74  code: str = prot
+00008cd0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00008ce0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+00008cf0: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
+00008d00: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+00008d10: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+00008d20: 2020 6665 6564 5f6c 6162 656c 3a20 7374    feed_label: st
+00008d30: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00008d40: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+00008d50: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+00008d60: 756d 6265 723d 332c 0a20 2020 2020 2020  umber=3,.       
+00008d70: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+00008d80: 2020 2020 290a 2020 2020 6f66 6665 725f      ).    offer_
+00008d90: 6964 3a20 7374 7220 3d20 7072 6f74 6f2e  id: str = proto.
+00008da0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00008db0: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+00008dc0: 2020 2020 206e 756d 6265 723d 342c 0a20       number=4,. 
+00008dd0: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+00008de0: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+00008df0: 7469 746c 653a 2073 7472 203d 2070 726f  title: str = pro
+00008e00: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+00008e10: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
+00008e20: 2020 2020 2020 2020 6e75 6d62 6572 3d35          number=5
+00008e30: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+00008e40: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+00008e50: 2020 2062 7261 6e64 3a20 7374 7220 3d20     brand: str = 
+00008e60: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00008e70: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+00008e80: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+00008e90: 723d 362c 0a20 2020 2020 2020 206f 7074  r=6,.        opt
+00008ea0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+00008eb0: 290a 2020 2020 6361 7465 676f 7279 5f6c  ).    category_l
+00008ec0: 313a 2073 7472 203d 2070 726f 746f 2e46  1: str = proto.F
+00008ed0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00008ee0: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+00008ef0: 2020 2020 6e75 6d62 6572 3d37 2c0a 2020      number=7,.  
+00008f00: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+00008f10: 7275 652c 0a20 2020 2029 0a20 2020 2063  rue,.    ).    c
+00008f20: 6174 6567 6f72 795f 6c32 3a20 7374 7220  ategory_l2: str 
+00008f30: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00008f40: 2020 2020 2020 2070 726f 746f 2e53 5452         proto.STR
+00008f50: 494e 472c 0a20 2020 2020 2020 206e 756d  ING,.        num
+00008f60: 6265 723d 382c 0a20 2020 2020 2020 206f  ber=8,.        o
+00008f70: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+00008f80: 2020 290a 2020 2020 6361 7465 676f 7279    ).    category
+00008f90: 5f6c 333a 2073 7472 203d 2070 726f 746f  _l3: str = proto
+00008fa0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00008fb0: 7072 6f74 6f2e 5354 5249 4e47 2c0a 2020  proto.STRING,.  
+00008fc0: 2020 2020 2020 6e75 6d62 6572 3d39 2c0a        number=9,.
+00008fd0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00008fe0: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+00008ff0: 2063 6174 6567 6f72 795f 6c34 3a20 7374   category_l4: st
+00009000: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00009010: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+00009020: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+00009030: 756d 6265 723d 3130 2c0a 2020 2020 2020  umber=10,.      
+00009040: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+00009050: 0a20 2020 2029 0a20 2020 2063 6174 6567  .    ).    categ
+00009060: 6f72 795f 6c35 3a20 7374 7220 3d20 7072  ory_l5: str = pr
+00009070: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+00009080: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
+00009090: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+000090a0: 3131 2c0a 2020 2020 2020 2020 6f70 7469  11,.        opti
+000090b0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+000090c0: 0a20 2020 2070 726f 6475 6374 5f74 7970  .    product_typ
+000090d0: 655f 6c31 3a20 7374 7220 3d20 7072 6f74  e_l1: str = prot
+000090e0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+000090f0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+00009100: 2020 2020 2020 206e 756d 6265 723d 3132         number=12
+00009110: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+00009120: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+00009130: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
+00009140: 6c32 3a20 7374 7220 3d20 7072 6f74 6f2e  l2: str = proto.
+00009150: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00009160: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+00009170: 2020 2020 206e 756d 6265 723d 3133 2c0a       number=13,.
+00009180: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00009190: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+000091a0: 2070 726f 6475 6374 5f74 7970 655f 6c33   product_type_l3
+000091b0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+000091c0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+000091d0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+000091e0: 2020 206e 756d 6265 723d 3134 2c0a 2020     number=14,.  
+000091f0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+00009200: 7275 652c 0a20 2020 2029 0a20 2020 2070  rue,.    ).    p
+00009210: 726f 6475 6374 5f74 7970 655f 6c34 3a20  roduct_type_l4: 
+00009220: 7374 7220 3d20 7072 6f74 6f2e 4669 656c  str = proto.Fiel
+00009230: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+00009240: 2e53 5452 494e 472c 0a20 2020 2020 2020  .STRING,.       
+00009250: 206e 756d 6265 723d 3135 2c0a 2020 2020   number=15,.    
+00009260: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+00009270: 652c 0a20 2020 2029 0a20 2020 2070 726f  e,.    ).    pro
+00009280: 6475 6374 5f74 7970 655f 6c35 3a20 7374  duct_type_l5: st
+00009290: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+000092a0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+000092b0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+000092c0: 756d 6265 723d 3136 2c0a 2020 2020 2020  umber=16,.      
+000092d0: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+000092e0: 0a20 2020 2029 0a20 2020 2070 7269 6365  .    ).    price
+000092f0: 3a20 7479 7065 732e 5072 6963 6520 3d20  : types.Price = 
+00009300: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00009310: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
+00009320: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
+00009330: 6572 3d31 372c 0a20 2020 2020 2020 206d  er=17,.        m
+00009340: 6573 7361 6765 3d74 7970 6573 2e50 7269  essage=types.Pri
+00009350: 6365 2c0a 2020 2020 290a 2020 2020 636f  ce,.    ).    co
+00009360: 6e64 6974 696f 6e3a 2073 7472 203d 2070  ndition: str = p
+00009370: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00009380: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+00009390: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+000093a0: 3d31 382c 0a20 2020 2020 2020 206f 7074  =18,.        opt
+000093b0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+000093c0: 290a 2020 2020 6176 6169 6c61 6269 6c69  ).    availabili
+000093d0: 7479 3a20 7374 7220 3d20 7072 6f74 6f2e  ty: str = proto.
+000093e0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+000093f0: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+00009400: 2020 2020 206e 756d 6265 723d 3139 2c0a       number=19,.
+00009410: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00009420: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+00009430: 2073 6869 7070 696e 675f 6c61 6265 6c3a   shipping_label:
+00009440: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
+00009450: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00009460: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
+00009470: 2020 6e75 6d62 6572 3d32 302c 0a20 2020    number=20,.   
+00009480: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+00009490: 7565 2c0a 2020 2020 290a 2020 2020 6774  ue,.    ).    gt
+000094a0: 696e 3a20 4d75 7461 626c 6553 6571 7565  in: MutableSeque
+000094b0: 6e63 655b 7374 725d 203d 2070 726f 746f  nce[str] = proto
+000094c0: 2e52 6570 6561 7465 6446 6965 6c64 280a  .RepeatedField(.
+000094d0: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+000094e0: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+000094f0: 6d62 6572 3d32 312c 0a20 2020 2029 0a20  mber=21,.    ). 
+00009500: 2020 2069 7465 6d5f 6772 6f75 705f 6964     item_group_id
+00009510: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+00009520: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+00009530: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+00009540: 2020 206e 756d 6265 723d 3232 2c0a 2020     number=22,.  
+00009550: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+00009560: 7275 652c 0a20 2020 2029 0a20 2020 2074  rue,.    ).    t
+00009570: 6875 6d62 6e61 696c 5f6c 696e 6b3a 2073  humbnail_link: s
+00009580: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+00009590: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+000095a0: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+000095b0: 6e75 6d62 6572 3d32 332c 0a20 2020 2020  number=23,.     
+000095c0: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+000095d0: 2c0a 2020 2020 290a 2020 2020 6372 6561  ,.    ).    crea
+000095e0: 7469 6f6e 5f74 696d 653a 2074 696d 6573  tion_time: times
+000095f0: 7461 6d70 5f70 6232 2e54 696d 6573 7461  tamp_pb2.Timesta
+00009600: 6d70 203d 2070 726f 746f 2e46 6965 6c64  mp = proto.Field
+00009610: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00009620: 4d45 5353 4147 452c 0a20 2020 2020 2020  MESSAGE,.       
+00009630: 206e 756d 6265 723d 3234 2c0a 2020 2020   number=24,.    
+00009640: 2020 2020 6d65 7373 6167 653d 7469 6d65      message=time
+00009650: 7374 616d 705f 7062 322e 5469 6d65 7374  stamp_pb2.Timest
+00009660: 616d 702c 0a20 2020 2029 0a20 2020 2065  amp,.    ).    e
+00009670: 7870 6972 6174 696f 6e5f 6461 7465 3a20  xpiration_date: 
+00009680: 6461 7465 5f70 6232 2e44 6174 6520 3d20  date_pb2.Date = 
+00009690: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+000096a0: 2020 2020 2070 726f 746f 2e4d 4553 5341       proto.MESSA
+000096b0: 4745 2c0a 2020 2020 2020 2020 6e75 6d62  GE,.        numb
+000096c0: 6572 3d32 352c 0a20 2020 2020 2020 206d  er=25,.        m
+000096d0: 6573 7361 6765 3d64 6174 655f 7062 322e  essage=date_pb2.
+000096e0: 4461 7465 2c0a 2020 2020 290a 2020 2020  Date,.    ).    
+000096f0: 6167 6772 6567 6174 6564 5f72 6570 6f72  aggregated_repor
+00009700: 7469 6e67 5f63 6f6e 7465 7874 5f73 7461  ting_context_sta
+00009710: 7475 733a 2041 6767 7265 6761 7465 6452  tus: AggregatedR
+00009720: 6570 6f72 7469 6e67 436f 6e74 6578 7453  eportingContextS
+00009730: 7461 7475 7320 3d20 7072 6f74 6f2e 4669  tatus = proto.Fi
+00009740: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+00009750: 746f 2e45 4e55 4d2c 0a20 2020 2020 2020  to.ENUM,.       
+00009760: 206e 756d 6265 723d 3236 2c0a 2020 2020   number=26,.    
+00009770: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+00009780: 652c 0a20 2020 2020 2020 2065 6e75 6d3d  e,.        enum=
+00009790: 4167 6772 6567 6174 6564 5265 706f 7274  AggregatedReport
+000097a0: 696e 6743 6f6e 7465 7874 5374 6174 7573  ingContextStatus
+000097b0: 2c0a 2020 2020 290a 2020 2020 6974 656d  ,.    ).    item
+000097c0: 5f69 7373 7565 733a 204d 7574 6162 6c65  _issues: Mutable
+000097d0: 5365 7175 656e 6365 5b49 7465 6d49 7373  Sequence[ItemIss
+000097e0: 7565 5d20 3d20 7072 6f74 6f2e 5265 7065  ue] = proto.Repe
+000097f0: 6174 6564 4669 656c 6428 0a20 2020 2020  atedField(.     
+00009800: 2020 2070 726f 746f 2e4d 4553 5341 4745     proto.MESSAGE
+00009810: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00009820: 3d32 372c 0a20 2020 2020 2020 206d 6573  =27,.        mes
+00009830: 7361 6765 3d49 7465 6d49 7373 7565 2c0a  sage=ItemIssue,.
+00009840: 2020 2020 290a 2020 2020 636c 6963 6b5f      ).    click_
+00009850: 706f 7465 6e74 6961 6c3a 2043 6c69 636b  potential: Click
+00009860: 506f 7465 6e74 6961 6c20 3d20 7072 6f74  Potential = prot
+00009870: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00009880: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
+00009890: 2020 2020 206e 756d 6265 723d 3239 2c0a       number=29,.
+000098a0: 2020 2020 2020 2020 656e 756d 3d43 6c69          enum=Cli
+000098b0: 636b 506f 7465 6e74 6961 6c2c 0a20 2020  ckPotential,.   
+000098c0: 2029 0a20 2020 2063 6c69 636b 5f70 6f74   ).    click_pot
+000098d0: 656e 7469 616c 5f72 616e 6b3a 2069 6e74  ential_rank: int
+000098e0: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+000098f0: 2020 2020 2020 2020 7072 6f74 6f2e 494e          proto.IN
+00009900: 5436 342c 0a20 2020 2020 2020 206e 756d  T64,.        num
+00009910: 6265 723d 3330 2c0a 2020 2020 2020 2020  ber=30,.        
+00009920: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00009930: 2020 2029 0a0a 0a63 6c61 7373 2050 7269     )...class Pri
+00009940: 6365 436f 6d70 6574 6974 6976 656e 6573  ceCompetitivenes
+00009950: 7350 726f 6475 6374 5669 6577 2870 726f  sProductView(pro
+00009960: 746f 2e4d 6573 7361 6765 293a 0a20 2020  to.Message):.   
+00009970: 2072 2222 2246 6965 6c64 7320 6176 6169   r"""Fields avai
+00009980: 6c61 626c 6520 666f 7220 7175 6572 7920  lable for query 
+00009990: 696e 2060 6070 7269 6365 5f63 6f6d 7065  in ``price_compe
+000099a0: 7469 7469 7665 6e65 7373 5f70 726f 6475  titiveness_produ
+000099b0: 6374 5f76 6965 7760 600a 2020 2020 7461  ct_view``.    ta
+000099c0: 626c 652e 0a0a 2020 2020 6050 7269 6365  ble...    `Price
+000099d0: 0a20 2020 2063 6f6d 7065 7469 7469 7665  .    competitive
+000099e0: 6e65 7373 203c 6874 7470 733a 2f2f 7375  ness <https://su
+000099f0: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
+00009a00: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
+00009a10: 722f 3936 3236 3930 333e 605f 5f0a 2020  r/9626903>`__.  
+00009a20: 2020 7265 706f 7274 2e0a 0a20 2020 2056    report...    V
+00009a30: 616c 7565 7320 6172 6520 6f6e 6c79 2073  alues are only s
+00009a40: 6574 2066 6f72 2066 6965 6c64 7320 7265  et for fields re
+00009a50: 7175 6573 7465 6420 6578 706c 6963 6974  quested explicit
+00009a60: 6c79 2069 6e20 7468 6520 7265 7175 6573  ly in the reques
+00009a70: 7427 730a 2020 2020 7365 6172 6368 2071  t's.    search q
+00009a80: 7565 7279 2e0a 0a0a 2020 2020 2e2e 205f  uery....    .. _
+00009a90: 6f6e 656f 663a 2068 7474 7073 3a2f 2f70  oneof: https://p
+00009aa0: 726f 746f 2d70 6c75 732d 7079 7468 6f6e  roto-plus-python
+00009ab0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00009ac0: 656e 2f73 7461 626c 652f 6669 656c 6473  en/stable/fields
+00009ad0: 2e68 746d 6c23 6f6e 656f 6673 2d6d 7574  .html#oneofs-mut
+00009ae0: 7561 6c6c 792d 6578 636c 7573 6976 652d  ually-exclusive-
+00009af0: 6669 656c 6473 0a0a 2020 2020 4174 7472  fields..    Attr
+00009b00: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
+00009b10: 7265 706f 7274 5f63 6f75 6e74 7279 5f63  report_country_c
+00009b20: 6f64 6520 2873 7472 293a 0a20 2020 2020  ode (str):.     
+00009b30: 2020 2020 2020 2043 6f75 6e74 7279 206f         Country o
+00009b40: 6620 7468 6520 7072 6963 6520 6265 6e63  f the price benc
+00009b50: 686d 6172 6b2e 2052 6570 7265 7365 6e74  hmark. Represent
+00009b60: 6564 2069 6e20 7468 6520 4953 4f20 3331  ed in the ISO 31
+00009b70: 3636 0a20 2020 2020 2020 2020 2020 2066  66.            f
+00009b80: 6f72 6d61 742e 0a0a 2020 2020 2020 2020  ormat...        
+00009b90: 2020 2020 5265 7175 6972 6564 2069 6e20      Required in 
+00009ba0: 7468 6520 6060 5345 4c45 4354 6060 2063  the ``SELECT`` c
+00009bb0: 6c61 7573 652e 0a0a 2020 2020 2020 2020  lause...        
+00009bc0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+00009bd0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+00009be0: 6e65 6f66 605f 2060 605f 7265 706f 7274  neof`_ ``_report
+00009bf0: 5f63 6f75 6e74 7279 5f63 6f64 6560 602e  _country_code``.
+00009c00: 0a20 2020 2020 2020 2069 6420 2873 7472  .        id (str
+00009c10: 293a 0a20 2020 2020 2020 2020 2020 2052  ):.            R
+00009c20: 4553 5420 4944 206f 6620 7468 6520 7072  EST ID of the pr
+00009c30: 6f64 7563 742c 2069 6e20 7468 6520 666f  oduct, in the fo
+00009c40: 726d 206f 660a 2020 2020 2020 2020 2020  rm of.          
+00009c50: 2020 6060 6368 616e 6e65 6c7e 6c61 6e67    ``channel~lang
+00009c60: 7561 6765 436f 6465 7e66 6565 644c 6162  uageCode~feedLab
+00009c70: 656c 7e6f 6666 6572 4964 6060 2e20 4361  el~offerId``. Ca
+00009c80: 6e20 6265 2075 7365 6420 746f 0a20 2020  n be used to.   
+00009c90: 2020 2020 2020 2020 206a 6f69 6e20 6461           join da
+00009ca0: 7461 2077 6974 6820 7468 6520 6060 7072  ta with the ``pr
+00009cb0: 6f64 7563 745f 7669 6577 6060 2074 6162  oduct_view`` tab
+00009cc0: 6c65 2e0a 0a20 2020 2020 2020 2020 2020  le...           
+00009cd0: 2052 6571 7569 7265 6420 696e 2074 6865   Required in the
+00009ce0: 2060 6053 454c 4543 5460 6020 636c 6175   ``SELECT`` clau
+00009cf0: 7365 2e0a 0a20 2020 2020 2020 2020 2020  se...           
+00009d00: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+00009d10: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+00009d20: 6660 5f20 6060 5f69 6460 602e 0a20 2020  f`_ ``_id``..   
+00009d30: 2020 2020 206f 6666 6572 5f69 6420 2873       offer_id (s
+00009d40: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+00009d50: 204d 6572 6368 616e 742d 7072 6f76 6964   Merchant-provid
+00009d60: 6564 2069 6420 6f66 2074 6865 2070 726f  ed id of the pro
+00009d70: 6475 6374 2e0a 0a20 2020 2020 2020 2020  duct...         
+00009d80: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+00009d90: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+00009da0: 656f 6660 5f20 6060 5f6f 6666 6572 5f69  eof`_ ``_offer_i
+00009db0: 6460 602e 0a20 2020 2020 2020 2074 6974  d``..        tit
+00009dc0: 6c65 2028 7374 7229 3a0a 2020 2020 2020  le (str):.      
+00009dd0: 2020 2020 2020 5469 746c 6520 6f66 2074        Title of t
+00009de0: 6865 2070 726f 6475 6374 2e0a 0a20 2020  he product...   
+00009df0: 2020 2020 2020 2020 2054 6869 7320 6669           This fi
+00009e00: 656c 6420 6973 2061 206d 656d 6265 7220  eld is a member 
+00009e10: 6f66 2060 6f6e 656f 6660 5f20 6060 5f74  of `oneof`_ ``_t
+00009e20: 6974 6c65 6060 2e0a 2020 2020 2020 2020  itle``..        
+00009e30: 6272 616e 6420 2873 7472 293a 0a20 2020  brand (str):.   
+00009e40: 2020 2020 2020 2020 2042 7261 6e64 206f           Brand o
+00009e50: 6620 7468 6520 7072 6f64 7563 742e 0a0a  f the product...
+00009e60: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00009e70: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00009e80: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+00009e90: 605f 6272 616e 6460 602e 0a20 2020 2020  `_brand``..     
+00009ea0: 2020 2063 6174 6567 6f72 795f 6c31 2028     category_l1 (
+00009eb0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00009ec0: 2020 5072 6f64 7563 7420 6361 7465 676f    Product catego
+00009ed0: 7279 2028 3173 7420 6c65 7665 6c29 2069  ry (1st level) i
+00009ee0: 6e20 6047 6f6f 676c 6527 7320 7072 6f64  n `Google's prod
+00009ef0: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
+00009f00: 7461 786f 6e6f 6d79 203c 6874 7470 733a  taxonomy <https:
+00009f10: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
+00009f20: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
+00009f30: 6e73 7765 722f 3633 3234 3433 363e 605f  nswer/6324436>`_
+00009f40: 5f2e 0a0a 2020 2020 2020 2020 2020 2020  _...            
+00009f50: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+00009f60: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+00009f70: 605f 2060 605f 6361 7465 676f 7279 5f6c  `_ ``_category_l
+00009f80: 3160 602e 0a20 2020 2020 2020 2063 6174  1``..        cat
+00009f90: 6567 6f72 795f 6c32 2028 7374 7229 3a0a  egory_l2 (str):.
+00009fa0: 2020 2020 2020 2020 2020 2020 5072 6f64              Prod
+00009fb0: 7563 7420 6361 7465 676f 7279 2028 326e  uct category (2n
+00009fc0: 6420 6c65 7665 6c29 2069 6e20 6047 6f6f  d level) in `Goo
+00009fd0: 676c 6527 7320 7072 6f64 7563 740a 2020  gle's product.  
+00009fe0: 2020 2020 2020 2020 2020 7461 786f 6e6f            taxono
+00009ff0: 6d79 203c 6874 7470 733a 2f2f 7375 7070  my <https://supp
+0000a000: 6f72 742e 676f 6f67 6c65 2e63 6f6d 2f6d  ort.google.com/m
+0000a010: 6572 6368 616e 7473 2f61 6e73 7765 722f  erchants/answer/
+0000a020: 3633 3234 3433 363e 605f 5f2e 0a0a 2020  6324436>`__...  
+0000a030: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+0000a040: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+0000a050: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+0000a060: 6361 7465 676f 7279 5f6c 3260 602e 0a20  category_l2``.. 
+0000a070: 2020 2020 2020 2063 6174 6567 6f72 795f         category_
+0000a080: 6c33 2028 7374 7229 3a0a 2020 2020 2020  l3 (str):.      
+0000a090: 2020 2020 2020 5072 6f64 7563 7420 6361        Product ca
+0000a0a0: 7465 676f 7279 2028 3372 6420 6c65 7665  tegory (3rd leve
+0000a0b0: 6c29 2069 6e20 6047 6f6f 676c 6527 7320  l) in `Google's 
+0000a0c0: 7072 6f64 7563 740a 2020 2020 2020 2020  product.        
+0000a0d0: 2020 2020 7461 786f 6e6f 6d79 203c 6874      taxonomy <ht
+0000a0e0: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
+0000a0f0: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
+0000a100: 7473 2f61 6e73 7765 722f 3633 3234 3433  ts/answer/632443
+0000a110: 363e 605f 5f2e 0a0a 2020 2020 2020 2020  6>`__...        
+0000a120: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+0000a130: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+0000a140: 6e65 6f66 605f 2060 605f 6361 7465 676f  neof`_ ``_catego
+0000a150: 7279 5f6c 3360 602e 0a20 2020 2020 2020  ry_l3``..       
+0000a160: 2063 6174 6567 6f72 795f 6c34 2028 7374   category_l4 (st
+0000a170: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0000a180: 5072 6f64 7563 7420 6361 7465 676f 7279  Product category
+0000a190: 2028 3474 6820 6c65 7665 6c29 2069 6e20   (4th level) in 
+0000a1a0: 6047 6f6f 676c 6527 7320 7072 6f64 7563  `Google's produc
+0000a1b0: 740a 2020 2020 2020 2020 2020 2020 7461  t.            ta
+0000a1c0: 786f 6e6f 6d79 203c 6874 7470 733a 2f2f  xonomy <https://
+0000a1d0: 7375 7070 6f72 742e 676f 6f67 6c65 2e63  support.google.c
+0000a1e0: 6f6d 2f6d 6572 6368 616e 7473 2f61 6e73  om/merchants/ans
+0000a1f0: 7765 722f 3633 3234 3433 363e 605f 5f2e  wer/6324436>`__.
+0000a200: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+0000a210: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+0000a220: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+0000a230: 2060 605f 6361 7465 676f 7279 5f6c 3460   ``_category_l4`
+0000a240: 602e 0a20 2020 2020 2020 2063 6174 6567  `..        categ
+0000a250: 6f72 795f 6c35 2028 7374 7229 3a0a 2020  ory_l5 (str):.  
+0000a260: 2020 2020 2020 2020 2020 5072 6f64 7563            Produc
+0000a270: 7420 6361 7465 676f 7279 2028 3574 6820  t category (5th 
+0000a280: 6c65 7665 6c29 2069 6e20 6047 6f6f 676c  level) in `Googl
+0000a290: 6527 7320 7072 6f64 7563 740a 2020 2020  e's product.    
+0000a2a0: 2020 2020 2020 2020 7461 786f 6e6f 6d79          taxonomy
+0000a2b0: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
+0000a2c0: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
+0000a2d0: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
+0000a2e0: 3234 3433 363e 605f 5f2e 0a0a 2020 2020  24436>`__...    
+0000a2f0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+0000a300: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+0000a310: 6620 606f 6e65 6f66 605f 2060 605f 6361  f `oneof`_ ``_ca
+0000a320: 7465 676f 7279 5f6c 3560 602e 0a20 2020  tegory_l5``..   
+0000a330: 2020 2020 2070 726f 6475 6374 5f74 7970       product_typ
+0000a340: 655f 6c31 2028 7374 7229 3a0a 2020 2020  e_l1 (str):.    
+0000a350: 2020 2020 2020 2020 5072 6f64 7563 7420          Product 
+0000a360: 7479 7065 2028 3173 7420 6c65 7665 6c29  type (1st level)
+0000a370: 2069 6e20 6d65 7263 6861 6e74 2773 206f   in merchant's o
+0000a380: 776e 2060 7072 6f64 7563 740a 2020 2020  wn `product.    
+0000a390: 2020 2020 2020 2020 7461 786f 6e6f 6d79          taxonomy
+0000a3a0: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
+0000a3b0: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
+0000a3c0: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
+0000a3d0: 3234 3430 363e 605f 5f2e 0a0a 2020 2020  24406>`__...    
+0000a3e0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+0000a3f0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+0000a400: 6620 606f 6e65 6f66 605f 2060 605f 7072  f `oneof`_ ``_pr
+0000a410: 6f64 7563 745f 7479 7065 5f6c 3160 602e  oduct_type_l1``.
+0000a420: 0a20 2020 2020 2020 2070 726f 6475 6374  .        product
+0000a430: 5f74 7970 655f 6c32 2028 7374 7229 3a0a  _type_l2 (str):.
+0000a440: 2020 2020 2020 2020 2020 2020 5072 6f64              Prod
+0000a450: 7563 7420 7479 7065 2028 326e 6420 6c65  uct type (2nd le
+0000a460: 7665 6c29 2069 6e20 6d65 7263 6861 6e74  vel) in merchant
+0000a470: 2773 206f 776e 2060 7072 6f64 7563 740a  's own `product.
+0000a480: 2020 2020 2020 2020 2020 2020 7461 786f              taxo
+0000a490: 6e6f 6d79 203c 6874 7470 733a 2f2f 7375  nomy <https://su
+0000a4a0: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
+0000a4b0: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
+0000a4c0: 722f 3633 3234 3430 363e 605f 5f2e 0a0a  r/6324406>`__...
+0000a4d0: 2020 2020 2020 2020 2020 2020 5468 6973              This
+0000a4e0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+0000a4f0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+0000a500: 605f 7072 6f64 7563 745f 7479 7065 5f6c  `_product_type_l
+0000a510: 3260 602e 0a20 2020 2020 2020 2070 726f  2``..        pro
+0000a520: 6475 6374 5f74 7970 655f 6c33 2028 7374  duct_type_l3 (st
+0000a530: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0000a540: 5072 6f64 7563 7420 7479 7065 2028 3372  Product type (3r
+0000a550: 6420 6c65 7665 6c29 2069 6e20 6d65 7263  d level) in merc
+0000a560: 6861 6e74 2773 206f 776e 2060 7072 6f64  hant's own `prod
+0000a570: 7563 740a 2020 2020 2020 2020 2020 2020  uct.            
+0000a580: 7461 786f 6e6f 6d79 203c 6874 7470 733a  taxonomy <https:
+0000a590: 2f2f 7375 7070 6f72 742e 676f 6f67 6c65  //support.google
+0000a5a0: 2e63 6f6d 2f6d 6572 6368 616e 7473 2f61  .com/merchants/a
+0000a5b0: 6e73 7765 722f 3633 3234 3430 363e 605f  nswer/6324406>`_
+0000a5c0: 5f2e 0a0a 2020 2020 2020 2020 2020 2020  _...            
+0000a5d0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+0000a5e0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+0000a5f0: 605f 2060 605f 7072 6f64 7563 745f 7479  `_ ``_product_ty
+0000a600: 7065 5f6c 3360 602e 0a20 2020 2020 2020  pe_l3``..       
+0000a610: 2070 726f 6475 6374 5f74 7970 655f 6c34   product_type_l4
+0000a620: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+0000a630: 2020 2020 5072 6f64 7563 7420 7479 7065      Product type
+0000a640: 2028 3474 6820 6c65 7665 6c29 2069 6e20   (4th level) in 
+0000a650: 6d65 7263 6861 6e74 2773 206f 776e 2060  merchant's own `
+0000a660: 7072 6f64 7563 740a 2020 2020 2020 2020  product.        
+0000a670: 2020 2020 7461 786f 6e6f 6d79 203c 6874      taxonomy <ht
+0000a680: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
+0000a690: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
+0000a6a0: 7473 2f61 6e73 7765 722f 3633 3234 3430  ts/answer/632440
+0000a6b0: 363e 605f 5f2e 0a0a 2020 2020 2020 2020  6>`__...        
+0000a6c0: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+0000a6d0: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+0000a6e0: 6e65 6f66 605f 2060 605f 7072 6f64 7563  neof`_ ``_produc
+0000a6f0: 745f 7479 7065 5f6c 3460 602e 0a20 2020  t_type_l4``..   
+0000a700: 2020 2020 2070 726f 6475 6374 5f74 7970       product_typ
+0000a710: 655f 6c35 2028 7374 7229 3a0a 2020 2020  e_l5 (str):.    
+0000a720: 2020 2020 2020 2020 5072 6f64 7563 7420          Product 
+0000a730: 7479 7065 2028 3574 6820 6c65 7665 6c29  type (5th level)
+0000a740: 2069 6e20 6d65 7263 6861 6e74 2773 206f   in merchant's o
+0000a750: 776e 2060 7072 6f64 7563 740a 2020 2020  wn `product.    
+0000a760: 2020 2020 2020 2020 7461 786f 6e6f 6d79          taxonomy
+0000a770: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
+0000a780: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
+0000a790: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
+0000a7a0: 3234 3430 363e 605f 5f2e 0a0a 2020 2020  24406>`__...    
+0000a7b0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+0000a7c0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+0000a7d0: 6620 606f 6e65 6f66 605f 2060 605f 7072  f `oneof`_ ``_pr
+0000a7e0: 6f64 7563 745f 7479 7065 5f6c 3560 602e  oduct_type_l5``.
+0000a7f0: 0a20 2020 2020 2020 2070 7269 6365 2028  .        price (
+0000a800: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
+0000a810: 7479 7065 2e74 7970 6573 2e50 7269 6365  type.types.Price
+0000a820: 293a 0a20 2020 2020 2020 2020 2020 2043  ):.            C
+0000a830: 7572 7265 6e74 2070 7269 6365 206f 6620  urrent price of 
+0000a840: 7468 6520 7072 6f64 7563 742e 0a20 2020  the product..   
+0000a850: 2020 2020 2062 656e 6368 6d61 726b 5f70       benchmark_p
+0000a860: 7269 6365 2028 676f 6f67 6c65 2e73 686f  rice (google.sho
+0000a870: 7070 696e 672e 7479 7065 2e74 7970 6573  pping.type.types
+0000a880: 2e50 7269 6365 293a 0a20 2020 2020 2020  .Price):.       
+0000a890: 2020 2020 204c 6174 6573 7420 6176 6169       Latest avai
+0000a8a0: 6c61 626c 6520 7072 6963 6520 6265 6e63  lable price benc
+0000a8b0: 686d 6172 6b20 666f 7220 7468 650a 2020  hmark for the.  
+0000a8c0: 2020 2020 2020 2020 2020 7072 6f64 7563            produc
+0000a8d0: 7427 7320 6361 7461 6c6f 6720 696e 2074  t's catalog in t
+0000a8e0: 6865 2062 656e 6368 6d61 726b 2063 6f75  he benchmark cou
+0000a8f0: 6e74 7279 2e0a 2020 2020 2222 220a 0a20  ntry..    """.. 
+0000a900: 2020 2072 6570 6f72 745f 636f 756e 7472     report_countr
+0000a910: 795f 636f 6465 3a20 7374 7220 3d20 7072  y_code: str = pr
+0000a920: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+0000a930: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
+0000a940: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+0000a950: 312c 0a20 2020 2020 2020 206f 7074 696f  1,.        optio
+0000a960: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
+0000a970: 2020 2020 6964 3a20 7374 7220 3d20 7072      id: str = pr
+0000a980: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+0000a990: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
+0000a9a0: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+0000a9b0: 322c 0a20 2020 2020 2020 206f 7074 696f  2,.        optio
+0000a9c0: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
+0000a9d0: 2020 2020 6f66 6665 725f 6964 3a20 7374      offer_id: st
+0000a9e0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+0000a9f0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+0000aa00: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+0000aa10: 756d 6265 723d 332c 0a20 2020 2020 2020  umber=3,.       
+0000aa20: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+0000aa30: 2020 2020 290a 2020 2020 7469 746c 653a      ).    title:
+0000aa40: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
+0000aa50: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+0000aa60: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
+0000aa70: 2020 6e75 6d62 6572 3d34 2c0a 2020 2020    number=4,.    
+0000aa80: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+0000aa90: 652c 0a20 2020 2029 0a20 2020 2062 7261  e,.    ).    bra
+0000aaa0: 6e64 3a20 7374 7220 3d20 7072 6f74 6f2e  nd: str = proto.
+0000aab0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+0000aac0: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+0000aad0: 2020 2020 206e 756d 6265 723d 352c 0a20       number=5,. 
+0000aae0: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+0000aaf0: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+0000ab00: 6361 7465 676f 7279 5f6c 313a 2073 7472  category_l1: str
+0000ab10: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000ab20: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+0000ab30: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+0000ab40: 6d62 6572 3d36 2c0a 2020 2020 2020 2020  mber=6,.        
+0000ab50: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+0000ab60: 2020 2029 0a20 2020 2063 6174 6567 6f72     ).    categor
+0000ab70: 795f 6c32 3a20 7374 7220 3d20 7072 6f74  y_l2: str = prot
+0000ab80: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+0000ab90: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+0000aba0: 2020 2020 2020 206e 756d 6265 723d 372c         number=7,
+0000abb0: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+0000abc0: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+0000abd0: 2020 6361 7465 676f 7279 5f6c 333a 2073    category_l3: s
+0000abe0: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+0000abf0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+0000ac00: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+0000ac10: 6e75 6d62 6572 3d38 2c0a 2020 2020 2020  number=8,.      
+0000ac20: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+0000ac30: 0a20 2020 2029 0a20 2020 2063 6174 6567  .    ).    categ
+0000ac40: 6f72 795f 6c34 3a20 7374 7220 3d20 7072  ory_l4: str = pr
+0000ac50: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+0000ac60: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
+0000ac70: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+0000ac80: 392c 0a20 2020 2020 2020 206f 7074 696f  9,.        optio
+0000ac90: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
+0000aca0: 2020 2020 6361 7465 676f 7279 5f6c 353a      category_l5:
+0000acb0: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
+0000acc0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+0000acd0: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
+0000ace0: 2020 6e75 6d62 6572 3d31 302c 0a20 2020    number=10,.   
+0000acf0: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+0000ad00: 7565 2c0a 2020 2020 290a 2020 2020 7072  ue,.    ).    pr
+0000ad10: 6f64 7563 745f 7479 7065 5f6c 313a 2073  oduct_type_l1: s
+0000ad20: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+0000ad30: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+0000ad40: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+0000ad50: 6e75 6d62 6572 3d31 312c 0a20 2020 2020  number=11,.     
+0000ad60: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+0000ad70: 2c0a 2020 2020 290a 2020 2020 7072 6f64  ,.    ).    prod
+0000ad80: 7563 745f 7479 7065 5f6c 323a 2073 7472  uct_type_l2: str
+0000ad90: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000ada0: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+0000adb0: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+0000adc0: 6d62 6572 3d31 322c 0a20 2020 2020 2020  mber=12,.       
+0000add0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+0000ade0: 2020 2020 290a 2020 2020 7072 6f64 7563      ).    produc
+0000adf0: 745f 7479 7065 5f6c 333a 2073 7472 203d  t_type_l3: str =
+0000ae00: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+0000ae10: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+0000ae20: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
+0000ae30: 6572 3d31 332c 0a20 2020 2020 2020 206f  er=13,.        o
+0000ae40: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+0000ae50: 2020 290a 2020 2020 7072 6f64 7563 745f    ).    product_
+0000ae60: 7479 7065 5f6c 343a 2073 7472 203d 2070  type_l4: str = p
+0000ae70: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000ae80: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+0000ae90: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+0000aea0: 3d31 342c 0a20 2020 2020 2020 206f 7074  =14,.        opt
+0000aeb0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+0000aec0: 290a 2020 2020 7072 6f64 7563 745f 7479  ).    product_ty
+0000aed0: 7065 5f6c 353a 2073 7472 203d 2070 726f  pe_l5: str = pro
+0000aee0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+0000aef0: 2020 7072 6f74 6f2e 5354 5249 4e47 2c0a    proto.STRING,.
+0000af00: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
+0000af10: 352c 0a20 2020 2020 2020 206f 7074 696f  5,.        optio
+0000af20: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
+0000af30: 2020 2020 7072 6963 653a 2074 7970 6573      price: types
+0000af40: 2e50 7269 6365 203d 2070 726f 746f 2e46  .Price = proto.F
+0000af50: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+0000af60: 6f74 6f2e 4d45 5353 4147 452c 0a20 2020  oto.MESSAGE,.   
+0000af70: 2020 2020 206e 756d 6265 723d 3136 2c0a       number=16,.
+0000af80: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
+0000af90: 7479 7065 732e 5072 6963 652c 0a20 2020  types.Price,.   
+0000afa0: 2029 0a20 2020 2062 656e 6368 6d61 726b   ).    benchmark
+0000afb0: 5f70 7269 6365 3a20 7479 7065 732e 5072  _price: types.Pr
+0000afc0: 6963 6520 3d20 7072 6f74 6f2e 4669 656c  ice = proto.Fiel
+0000afd0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+0000afe0: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
+0000aff0: 2020 6e75 6d62 6572 3d31 372c 0a20 2020    number=17,.   
+0000b000: 2020 2020 206d 6573 7361 6765 3d74 7970       message=typ
+0000b010: 6573 2e50 7269 6365 2c0a 2020 2020 290a  es.Price,.    ).
+0000b020: 0a0a 636c 6173 7320 5072 6963 6549 6e73  ..class PriceIns
+0000b030: 6967 6874 7350 726f 6475 6374 5669 6577  ightsProductView
+0000b040: 2870 726f 746f 2e4d 6573 7361 6765 293a  (proto.Message):
+0000b050: 0a20 2020 2072 2222 2246 6965 6c64 7320  .    r"""Fields 
+0000b060: 6176 6169 6c61 626c 6520 666f 7220 7175  available for qu
+0000b070: 6572 7920 696e 2060 6070 7269 6365 5f69  ery in ``price_i
+0000b080: 6e73 6967 6874 735f 7072 6f64 7563 745f  nsights_product_
+0000b090: 7669 6577 6060 2074 6162 6c65 2e0a 0a20  view`` table... 
+0000b0a0: 2020 2060 5072 6963 650a 2020 2020 696e     `Price.    in
+0000b0b0: 7369 6768 7473 203c 6874 7470 733a 2f2f  sights <https://
+0000b0c0: 7375 7070 6f72 742e 676f 6f67 6c65 2e63  support.google.c
+0000b0d0: 6f6d 2f6d 6572 6368 616e 7473 2f61 6e73  om/merchants/ans
+0000b0e0: 7765 722f 3131 3931 3639 3236 3e60 5f5f  wer/11916926>`__
+0000b0f0: 0a20 2020 2072 6570 6f72 742e 0a0a 2020  .    report...  
+0000b100: 2020 5661 6c75 6573 2061 7265 206f 6e6c    Values are onl
+0000b110: 7920 7365 7420 666f 7220 6669 656c 6473  y set for fields
+0000b120: 2072 6571 7565 7374 6564 2065 7870 6c69   requested expli
+0000b130: 6369 746c 7920 696e 2074 6865 2072 6571  citly in the req
+0000b140: 7565 7374 2773 0a20 2020 2073 6561 7263  uest's.    searc
+0000b150: 6820 7175 6572 792e 0a0a 0a20 2020 202e  h query....    .
+0000b160: 2e20 5f6f 6e65 6f66 3a20 6874 7470 733a  . _oneof: https:
+0000b170: 2f2f 7072 6f74 6f2d 706c 7573 2d70 7974  //proto-plus-pyt
+0000b180: 686f 6e2e 7265 6164 7468 6564 6f63 732e  hon.readthedocs.
+0000b190: 696f 2f65 6e2f 7374 6162 6c65 2f66 6965  io/en/stable/fie
+0000b1a0: 6c64 732e 6874 6d6c 236f 6e65 6f66 732d  lds.html#oneofs-
+0000b1b0: 6d75 7475 616c 6c79 2d65 7863 6c75 7369  mutually-exclusi
+0000b1c0: 7665 2d66 6965 6c64 730a 0a20 2020 2041  ve-fields..    A
+0000b1d0: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
+0000b1e0: 2020 2069 6420 2873 7472 293a 0a20 2020     id (str):.   
+0000b1f0: 2020 2020 2020 2020 2052 4553 5420 4944           REST ID
+0000b200: 206f 6620 7468 6520 7072 6f64 7563 742c   of the product,
+0000b210: 2069 6e20 7468 6520 666f 726d 206f 660a   in the form of.
+0000b220: 2020 2020 2020 2020 2020 2020 6060 6368              ``ch
+0000b230: 616e 6e65 6c7e 6c61 6e67 7561 6765 436f  annel~languageCo
+0000b240: 6465 7e66 6565 644c 6162 656c 7e6f 6666  de~feedLabel~off
+0000b250: 6572 4964 6060 2e20 4361 6e20 6265 2075  erId``. Can be u
+0000b260: 7365 6420 746f 0a20 2020 2020 2020 2020  sed to.         
+0000b270: 2020 206a 6f69 6e20 6461 7461 2077 6974     join data wit
+0000b280: 6820 7468 6520 6060 7072 6f64 7563 745f  h the ``product_
+0000b290: 7669 6577 6060 2074 6162 6c65 2e0a 0a20  view`` table... 
+0000b2a0: 2020 2020 2020 2020 2020 2052 6571 7569             Requi
+0000b2b0: 7265 6420 696e 2074 6865 2060 6053 454c  red in the ``SEL
+0000b2c0: 4543 5460 6020 636c 6175 7365 2e0a 0a20  ECT`` clause... 
+0000b2d0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+0000b2e0: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+0000b2f0: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+0000b300: 5f69 6460 602e 0a20 2020 2020 2020 206f  _id``..        o
+0000b310: 6666 6572 5f69 6420 2873 7472 293a 0a20  ffer_id (str):. 
+0000b320: 2020 2020 2020 2020 2020 204d 6572 6368             Merch
+0000b330: 616e 742d 7072 6f76 6964 6564 2069 6420  ant-provided id 
+0000b340: 6f66 2074 6865 2070 726f 6475 6374 2e0a  of the product..
+0000b350: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+0000b360: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+0000b370: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+0000b380: 6060 5f6f 6666 6572 5f69 6460 602e 0a20  ``_offer_id``.. 
+0000b390: 2020 2020 2020 2074 6974 6c65 2028 7374         title (st
+0000b3a0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0000b3b0: 5469 746c 6520 6f66 2074 6865 2070 726f  Title of the pro
+0000b3c0: 6475 6374 2e0a 0a20 2020 2020 2020 2020  duct...         
+0000b3d0: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+0000b3e0: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+0000b3f0: 656f 6660 5f20 6060 5f74 6974 6c65 6060  eof`_ ``_title``
+0000b400: 2e0a 2020 2020 2020 2020 6272 616e 6420  ..        brand 
+0000b410: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+0000b420: 2020 2042 7261 6e64 206f 6620 7468 6520     Brand of the 
+0000b430: 7072 6f64 7563 742e 0a0a 2020 2020 2020  product...      
+0000b440: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+0000b450: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+0000b460: 606f 6e65 6f66 605f 2060 605f 6272 616e  `oneof`_ ``_bran
+0000b470: 6460 602e 0a20 2020 2020 2020 2063 6174  d``..        cat
+0000b480: 6567 6f72 795f 6c31 2028 7374 7229 3a0a  egory_l1 (str):.
+0000b490: 2020 2020 2020 2020 2020 2020 5072 6f64              Prod
+0000b4a0: 7563 7420 6361 7465 676f 7279 2028 3173  uct category (1s
+0000b4b0: 7420 6c65 7665 6c29 2069 6e20 6047 6f6f  t level) in `Goo
+0000b4c0: 676c 6527 7320 7072 6f64 7563 740a 2020  gle's product.  
+0000b4d0: 2020 2020 2020 2020 2020 7461 786f 6e6f            taxono
+0000b4e0: 6d79 203c 6874 7470 733a 2f2f 7375 7070  my <https://supp
+0000b4f0: 6f72 742e 676f 6f67 6c65 2e63 6f6d 2f6d  ort.google.com/m
+0000b500: 6572 6368 616e 7473 2f61 6e73 7765 722f  erchants/answer/
+0000b510: 3633 3234 3433 363e 605f 5f2e 0a0a 2020  6324436>`__...  
+0000b520: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+0000b530: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+0000b540: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+0000b550: 6361 7465 676f 7279 5f6c 3160 602e 0a20  category_l1``.. 
+0000b560: 2020 2020 2020 2063 6174 6567 6f72 795f         category_
+0000b570: 6c32 2028 7374 7229 3a0a 2020 2020 2020  l2 (str):.      
+0000b580: 2020 2020 2020 5072 6f64 7563 7420 6361        Product ca
+0000b590: 7465 676f 7279 2028 326e 6420 6c65 7665  tegory (2nd leve
+0000b5a0: 6c29 2069 6e20 6047 6f6f 676c 6527 7320  l) in `Google's 
+0000b5b0: 7072 6f64 7563 740a 2020 2020 2020 2020  product.        
+0000b5c0: 2020 2020 7461 786f 6e6f 6d79 203c 6874      taxonomy <ht
+0000b5d0: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
+0000b5e0: 6f67 6c65 2e63 6f6d 2f6d 6572 6368 616e  ogle.com/merchan
+0000b5f0: 7473 2f61 6e73 7765 722f 3633 3234 3433  ts/answer/632443
+0000b600: 363e 605f 5f2e 0a0a 2020 2020 2020 2020  6>`__...        
+0000b610: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+0000b620: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+0000b630: 6e65 6f66 605f 2060 605f 6361 7465 676f  neof`_ ``_catego
+0000b640: 7279 5f6c 3260 602e 0a20 2020 2020 2020  ry_l2``..       
+0000b650: 2063 6174 6567 6f72 795f 6c33 2028 7374   category_l3 (st
+0000b660: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0000b670: 5072 6f64 7563 7420 6361 7465 676f 7279  Product category
+0000b680: 2028 3372 6420 6c65 7665 6c29 2069 6e20   (3rd level) in 
+0000b690: 6047 6f6f 676c 6527 7320 7072 6f64 7563  `Google's produc
+0000b6a0: 740a 2020 2020 2020 2020 2020 2020 7461  t.            ta
+0000b6b0: 786f 6e6f 6d79 203c 6874 7470 733a 2f2f  xonomy <https://
+0000b6c0: 7375 7070 6f72 742e 676f 6f67 6c65 2e63  support.google.c
+0000b6d0: 6f6d 2f6d 6572 6368 616e 7473 2f61 6e73  om/merchants/ans
+0000b6e0: 7765 722f 3633 3234 3433 363e 605f 5f2e  wer/6324436>`__.
+0000b6f0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+0000b700: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+0000b710: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+0000b720: 2060 605f 6361 7465 676f 7279 5f6c 3360   ``_category_l3`
+0000b730: 602e 0a20 2020 2020 2020 2063 6174 6567  `..        categ
+0000b740: 6f72 795f 6c34 2028 7374 7229 3a0a 2020  ory_l4 (str):.  
+0000b750: 2020 2020 2020 2020 2020 5072 6f64 7563            Produc
+0000b760: 7420 6361 7465 676f 7279 2028 3474 6820  t category (4th 
+0000b770: 6c65 7665 6c29 2069 6e20 6047 6f6f 676c  level) in `Googl
+0000b780: 6527 7320 7072 6f64 7563 740a 2020 2020  e's product.    
+0000b790: 2020 2020 2020 2020 7461 786f 6e6f 6d79          taxonomy
+0000b7a0: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
+0000b7b0: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
+0000b7c0: 6368 616e 7473 2f61 6e73 7765 722f 3633  chants/answer/63
+0000b7d0: 3234 3433 363e 605f 5f2e 0a0a 2020 2020  24436>`__...    
+0000b7e0: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+0000b7f0: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+0000b800: 6620 606f 6e65 6f66 605f 2060 605f 6361  f `oneof`_ ``_ca
+0000b810: 7465 676f 7279 5f6c 3460 602e 0a20 2020  tegory_l4``..   
+0000b820: 2020 2020 2063 6174 6567 6f72 795f 6c35       category_l5
+0000b830: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+0000b840: 2020 2020 5072 6f64 7563 7420 6361 7465      Product cate
+0000b850: 676f 7279 2028 3574 6820 6c65 7665 6c29  gory (5th level)
+0000b860: 2069 6e20 6047 6f6f 676c 6527 7320 7072   in `Google's pr
+0000b870: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
+0000b880: 2020 7461 786f 6e6f 6d79 203c 6874 7470    taxonomy <http
+0000b890: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
+0000b8a0: 6c65 2e63 6f6d 2f6d 6572 6368 616e 7473  le.com/merchants
+0000b8b0: 2f61 6e73 7765 722f 3633 3234 3433 363e  /answer/6324436>
+0000b8c0: 605f 5f2e 0a0a 2020 2020 2020 2020 2020  `__...          
+0000b8d0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+0000b8e0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+0000b8f0: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
+0000b900: 5f6c 3560 602e 0a20 2020 2020 2020 2070  _l5``..        p
+0000b910: 726f 6475 6374 5f74 7970 655f 6c31 2028  roduct_type_l1 (
+0000b920: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+0000b930: 2020 5072 6f64 7563 7420 7479 7065 2028    Product type (
+0000b940: 3173 7420 6c65 7665 6c29 2069 6e20 6d65  1st level) in me
+0000b950: 7263 6861 6e74 2773 206f 776e 2060 7072  rchant's own `pr
+0000b960: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
+0000b970: 2020 7461 786f 6e6f 6d79 203c 6874 7470    taxonomy <http
+0000b980: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
+0000b990: 6c65 2e63 6f6d 2f6d 6572 6368 616e 7473  le.com/merchants
+0000b9a0: 2f61 6e73 7765 722f 3633 3234 3430 363e  /answer/6324406>
+0000b9b0: 605f 5f2e 0a0a 2020 2020 2020 2020 2020  `__...          
+0000b9c0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+0000b9d0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+0000b9e0: 6f66 605f 2060 605f 7072 6f64 7563 745f  of`_ ``_product_
+0000b9f0: 7479 7065 5f6c 3160 602e 0a20 2020 2020  type_l1``..     
+0000ba00: 2020 2070 726f 6475 6374 5f74 7970 655f     product_type_
+0000ba10: 6c32 2028 7374 7229 3a0a 2020 2020 2020  l2 (str):.      
+0000ba20: 2020 2020 2020 5072 6f64 7563 7420 7479        Product ty
+0000ba30: 7065 2028 326e 6420 6c65 7665 6c29 2069  pe (2nd level) i
+0000ba40: 6e20 6d65 7263 6861 6e74 2773 206f 776e  n merchant's own
+0000ba50: 2060 7072 6f64 7563 740a 2020 2020 2020   `product.      
+0000ba60: 2020 2020 2020 7461 786f 6e6f 6d79 203c        taxonomy <
+0000ba70: 6874 7470 733a 2f2f 7375 7070 6f72 742e  https://support.
+0000ba80: 676f 6f67 6c65 2e63 6f6d 2f6d 6572 6368  google.com/merch
+0000ba90: 616e 7473 2f61 6e73 7765 722f 3633 3234  ants/answer/6324
+0000baa0: 3430 363e 605f 5f2e 0a0a 2020 2020 2020  406>`__...      
+0000bab0: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+0000bac0: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+0000bad0: 606f 6e65 6f66 605f 2060 605f 7072 6f64  `oneof`_ ``_prod
+0000bae0: 7563 745f 7479 7065 5f6c 3260 602e 0a20  uct_type_l2``.. 
+0000baf0: 2020 2020 2020 2070 726f 6475 6374 5f74         product_t
+0000bb00: 7970 655f 6c33 2028 7374 7229 3a0a 2020  ype_l3 (str):.  
+0000bb10: 2020 2020 2020 2020 2020 5072 6f64 7563            Produc
+0000bb20: 7420 7479 7065 2028 3372 6420 6c65 7665  t type (3rd leve
+0000bb30: 6c29 2069 6e20 6d65 7263 6861 6e74 2773  l) in merchant's
+0000bb40: 206f 776e 2060 7072 6f64 7563 740a 2020   own `product.  
+0000bb50: 2020 2020 2020 2020 2020 7461 786f 6e6f            taxono
+0000bb60: 6d79 203c 6874 7470 733a 2f2f 7375 7070  my <https://supp
+0000bb70: 6f72 742e 676f 6f67 6c65 2e63 6f6d 2f6d  ort.google.com/m
+0000bb80: 6572 6368 616e 7473 2f61 6e73 7765 722f  erchants/answer/
+0000bb90: 3633 3234 3430 363e 605f 5f2e 0a0a 2020  6324406>`__...  
+0000bba0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+0000bbb0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+0000bbc0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+0000bbd0: 7072 6f64 7563 745f 7479 7065 5f6c 3360  product_type_l3`
+0000bbe0: 602e 0a20 2020 2020 2020 2070 726f 6475  `..        produ
+0000bbf0: 6374 5f74 7970 655f 6c34 2028 7374 7229  ct_type_l4 (str)
+0000bc00: 3a0a 2020 2020 2020 2020 2020 2020 5072  :.            Pr
+0000bc10: 6f64 7563 7420 7479 7065 2028 3474 6820  oduct type (4th 
+0000bc20: 6c65 7665 6c29 2069 6e20 6d65 7263 6861  level) in mercha
+0000bc30: 6e74 2773 206f 776e 2060 7072 6f64 7563  nt's own `produc
+0000bc40: 740a 2020 2020 2020 2020 2020 2020 7461  t.            ta
+0000bc50: 786f 6e6f 6d79 203c 6874 7470 733a 2f2f  xonomy <https://
+0000bc60: 7375 7070 6f72 742e 676f 6f67 6c65 2e63  support.google.c
+0000bc70: 6f6d 2f6d 6572 6368 616e 7473 2f61 6e73  om/merchants/ans
+0000bc80: 7765 722f 3633 3234 3430 363e 605f 5f2e  wer/6324406>`__.
+0000bc90: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+0000bca0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+0000bcb0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+0000bcc0: 2060 605f 7072 6f64 7563 745f 7479 7065   ``_product_type
+0000bcd0: 5f6c 3460 602e 0a20 2020 2020 2020 2070  _l4``..        p
+0000bce0: 726f 6475 6374 5f74 7970 655f 6c35 2028  roduct_type_l5 (
+0000bcf0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+0000bd00: 2020 5072 6f64 7563 7420 7479 7065 2028    Product type (
+0000bd10: 3574 6820 6c65 7665 6c29 2069 6e20 6d65  5th level) in me
+0000bd20: 7263 6861 6e74 2773 206f 776e 2060 7072  rchant's own `pr
+0000bd30: 6f64 7563 740a 2020 2020 2020 2020 2020  oduct.          
+0000bd40: 2020 7461 786f 6e6f 6d79 203c 6874 7470    taxonomy <http
+0000bd50: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
+0000bd60: 6c65 2e63 6f6d 2f6d 6572 6368 616e 7473  le.com/merchants
+0000bd70: 2f61 6e73 7765 722f 3633 3234 3430 363e  /answer/6324406>
+0000bd80: 605f 5f2e 0a0a 2020 2020 2020 2020 2020  `__...          
+0000bd90: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+0000bda0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+0000bdb0: 6f66 605f 2060 605f 7072 6f64 7563 745f  of`_ ``_product_
+0000bdc0: 7479 7065 5f6c 3560 602e 0a20 2020 2020  type_l5``..     
+0000bdd0: 2020 2070 7269 6365 2028 676f 6f67 6c65     price (google
+0000bde0: 2e73 686f 7070 696e 672e 7479 7065 2e74  .shopping.type.t
+0000bdf0: 7970 6573 2e50 7269 6365 293a 0a20 2020  ypes.Price):.   
+0000be00: 2020 2020 2020 2020 2043 7572 7265 6e74           Current
+0000be10: 2070 7269 6365 206f 6620 7468 6520 7072   price of the pr
+0000be20: 6f64 7563 742e 0a20 2020 2020 2020 2073  oduct..        s
+0000be30: 7567 6765 7374 6564 5f70 7269 6365 2028  uggested_price (
+0000be40: 676f 6f67 6c65 2e73 686f 7070 696e 672e  google.shopping.
+0000be50: 7479 7065 2e74 7970 6573 2e50 7269 6365  type.types.Price
+0000be60: 293a 0a20 2020 2020 2020 2020 2020 204c  ):.            L
+0000be70: 6174 6573 7420 7375 6767 6573 7465 6420  atest suggested 
+0000be80: 7072 6963 6520 666f 7220 7468 6520 7072  price for the pr
+0000be90: 6f64 7563 742e 0a20 2020 2020 2020 2070  oduct..        p
+0000bea0: 7265 6469 6374 6564 5f69 6d70 7265 7373  redicted_impress
+0000beb0: 696f 6e73 5f63 6861 6e67 655f 6672 6163  ions_change_frac
+0000bec0: 7469 6f6e 2028 666c 6f61 7429 3a0a 2020  tion (float):.  
+0000bed0: 2020 2020 2020 2020 2020 5072 6564 6963            Predic
+0000bee0: 7465 6420 6368 616e 6765 2069 6e20 696d  ted change in im
+0000bef0: 7072 6573 7369 6f6e 7320 6173 2061 2066  pressions as a f
+0000bf00: 7261 6374 696f 6e0a 2020 2020 2020 2020  raction.        
+0000bf10: 2020 2020 6166 7465 7220 696e 7472 6f64      after introd
+0000bf20: 7563 696e 6720 7468 6520 7375 6767 6573  ucing the sugges
+0000bf30: 7465 6420 7072 6963 6520 636f 6d70 6172  ted price compar
+0000bf40: 6564 0a20 2020 2020 2020 2020 2020 2074  ed.            t
+0000bf50: 6f20 6375 7272 656e 7420 6163 7469 7665  o current active
+0000bf60: 2070 7269 6365 2e20 466f 7220 6578 616d   price. For exam
+0000bf70: 706c 652c 2030 2e30 3520 6973 2061 0a20  ple, 0.05 is a. 
+0000bf80: 2020 2020 2020 2020 2020 2035 2520 7072             5% pr
+0000bf90: 6564 6963 7465 6420 696e 6372 6561 7365  edicted increase
+0000bfa0: 2069 6e20 696d 7072 6573 7369 6f6e 732e   in impressions.
+0000bfb0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+0000bfc0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+0000bfd0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+0000bfe0: 2060 605f 7072 6564 6963 7465 645f 696d   ``_predicted_im
+0000bff0: 7072 6573 7369 6f6e 735f 6368 616e 6765  pressions_change
+0000c000: 5f66 7261 6374 696f 6e60 602e 0a20 2020  _fraction``..   
+0000c010: 2020 2020 2070 7265 6469 6374 6564 5f63       predicted_c
+0000c020: 6c69 636b 735f 6368 616e 6765 5f66 7261  licks_change_fra
+0000c030: 6374 696f 6e20 2866 6c6f 6174 293a 0a20  ction (float):. 
+0000c040: 2020 2020 2020 2020 2020 2050 7265 6469             Predi
+0000c050: 6374 6564 2063 6861 6e67 6520 696e 2063  cted change in c
+0000c060: 6c69 636b 7320 6173 2061 2066 7261 6374  licks as a fract
+0000c070: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+0000c080: 6166 7465 7220 696e 7472 6f64 7563 696e  after introducin
+0000c090: 6720 7468 6520 7375 6767 6573 7465 6420  g the suggested 
+0000c0a0: 7072 6963 6520 636f 6d70 6172 6564 0a20  price compared. 
+0000c0b0: 2020 2020 2020 2020 2020 2074 6f20 6375             to cu
+0000c0c0: 7272 656e 7420 6163 7469 7665 2070 7269  rrent active pri
+0000c0d0: 6365 2e20 466f 7220 6578 616d 706c 652c  ce. For example,
+0000c0e0: 2030 2e30 3520 6973 2061 0a20 2020 2020   0.05 is a.     
+0000c0f0: 2020 2020 2020 2035 2520 7072 6564 6963         5% predic
+0000c100: 7465 6420 696e 6372 6561 7365 2069 6e20  ted increase in 
+0000c110: 636c 6963 6b73 2e0a 0a20 2020 2020 2020  clicks...       
+0000c120: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+0000c130: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+0000c140: 6f6e 656f 6660 5f20 6060 5f70 7265 6469  oneof`_ ``_predi
+0000c150: 6374 6564 5f63 6c69 636b 735f 6368 616e  cted_clicks_chan
+0000c160: 6765 5f66 7261 6374 696f 6e60 602e 0a20  ge_fraction``.. 
+0000c170: 2020 2020 2020 2070 7265 6469 6374 6564         predicted
+0000c180: 5f63 6f6e 7665 7273 696f 6e73 5f63 6861  _conversions_cha
+0000c190: 6e67 655f 6672 6163 7469 6f6e 2028 666c  nge_fraction (fl
+0000c1a0: 6f61 7429 3a0a 2020 2020 2020 2020 2020  oat):.          
+0000c1b0: 2020 5072 6564 6963 7465 6420 6368 616e    Predicted chan
+0000c1c0: 6765 2069 6e20 636f 6e76 6572 7369 6f6e  ge in conversion
+0000c1d0: 7320 6173 2061 2066 7261 6374 696f 6e0a  s as a fraction.
+0000c1e0: 2020 2020 2020 2020 2020 2020 6166 7465              afte
+0000c1f0: 7220 696e 7472 6f64 7563 696e 6720 7468  r introducing th
+0000c200: 6520 7375 6767 6573 7465 6420 7072 6963  e suggested pric
+0000c210: 6520 636f 6d70 6172 6564 0a20 2020 2020  e compared.     
+0000c220: 2020 2020 2020 2074 6f20 6375 7272 656e         to curren
+0000c230: 7420 6163 7469 7665 2070 7269 6365 2e20  t active price. 
+0000c240: 466f 7220 6578 616d 706c 652c 2030 2e30  For example, 0.0
+0000c250: 3520 6973 2061 0a20 2020 2020 2020 2020  5 is a.         
+0000c260: 2020 2035 2520 7072 6564 6963 7465 6420     5% predicted 
+0000c270: 696e 6372 6561 7365 2069 6e20 636f 6e76  increase in conv
+0000c280: 6572 7369 6f6e 7329 2e0a 0a20 2020 2020  ersions)...     
+0000c290: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
+0000c2a0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
+0000c2b0: 2060 6f6e 656f 6660 5f20 6060 5f70 7265   `oneof`_ ``_pre
+0000c2c0: 6469 6374 6564 5f63 6f6e 7665 7273 696f  dicted_conversio
+0000c2d0: 6e73 5f63 6861 6e67 655f 6672 6163 7469  ns_change_fracti
+0000c2e0: 6f6e 6060 2e0a 2020 2020 2020 2020 6566  on``..        ef
+0000c2f0: 6665 6374 6976 656e 6573 7320 2867 6f6f  fectiveness (goo
+0000c300: 676c 652e 7368 6f70 7069 6e67 2e6d 6572  gle.shopping.mer
+0000c310: 6368 616e 745f 7265 706f 7274 735f 7631  chant_reports_v1
+0000c320: 6265 7461 2e74 7970 6573 2e50 7269 6365  beta.types.Price
+0000c330: 496e 7369 6768 7473 5072 6f64 7563 7456  InsightsProductV
+0000c340: 6965 772e 4566 6665 6374 6976 656e 6573  iew.Effectivenes
+0000c350: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0000c360: 5468 6520 7072 6564 6963 7465 6420 6566  The predicted ef
+0000c370: 6665 6374 6976 656e 6573 7320 6f66 2061  fectiveness of a
+0000c380: 7070 6c79 696e 6720 7468 650a 2020 2020  pplying the.    
+0000c390: 2020 2020 2020 2020 7072 6963 6520 7375          price su
+0000c3a0: 6767 6573 7469 6f6e 2c20 6275 636b 6574  ggestion, bucket
+0000c3b0: 6564 2e0a 2020 2020 2222 220a 0a20 2020  ed..    """..   
+0000c3c0: 2063 6c61 7373 2045 6666 6563 7469 7665   class Effective
+0000c3d0: 6e65 7373 2870 726f 746f 2e45 6e75 6d29  ness(proto.Enum)
+0000c3e0: 3a0a 2020 2020 2020 2020 7222 2222 5072  :.        r"""Pr
+0000c3f0: 6564 6963 7465 6420 6566 6665 6374 6976  edicted effectiv
+0000c400: 656e 6573 7320 6275 636b 6574 2e0a 0a20  eness bucket... 
+0000c410: 2020 2020 2020 2045 6666 6563 7469 7665         Effective
+0000c420: 6e65 7373 2069 6e64 6963 6174 6573 2077  ness indicates w
+0000c430: 6869 6368 2070 726f 6475 6374 7320 776f  hich products wo
+0000c440: 756c 6420 6265 6e65 6669 7420 6d6f 7374  uld benefit most
+0000c450: 2066 726f 6d20 7072 6963 650a 2020 2020   from price.    
+0000c460: 2020 2020 6368 616e 6765 732e 2054 6869      changes. Thi
+0000c470: 7320 7261 7469 6e67 2074 616b 6573 2069  s rating takes i
+0000c480: 6e74 6f20 636f 6e73 6964 6572 6174 696f  nto consideratio
+0000c490: 6e20 7468 6520 7065 7266 6f72 6d61 6e63  n the performanc
+0000c4a0: 6520 626f 6f73 740a 2020 2020 2020 2020  e boost.        
+0000c4b0: 7072 6564 6963 7465 6420 6279 2061 646a  predicted by adj
+0000c4c0: 7573 7469 6e67 2074 6865 2073 616c 6520  usting the sale 
+0000c4d0: 7072 6963 6520 616e 6420 7468 6520 6469  price and the di
+0000c4e0: 6666 6572 656e 6365 2062 6574 7765 656e  fference between
+0000c4f0: 0a20 2020 2020 2020 2079 6f75 7220 6375  .        your cu
+0000c500: 7272 656e 7420 7072 6963 6520 616e 6420  rrent price and 
+0000c510: 7468 6520 7375 6767 6573 7465 6420 7072  the suggested pr
+0000c520: 6963 652e 2050 7269 6365 2073 7567 6765  ice. Price sugge
+0000c530: 7374 696f 6e73 2077 6974 680a 2020 2020  stions with.    
+0000c540: 2020 2020 6060 4849 4748 6060 2065 6666      ``HIGH`` eff
+0000c550: 6563 7469 7665 6e65 7373 2061 7265 2070  ectiveness are p
+0000c560: 7265 6469 6374 6564 2074 6f20 6472 6976  redicted to driv
+0000c570: 6520 7468 6520 6c61 7267 6573 7420 696e  e the largest in
+0000c580: 6372 6561 7365 0a20 2020 2020 2020 2069  crease.        i
+0000c590: 6e20 7065 7266 6f72 6d61 6e63 652e 0a0a  n performance...
+0000c5a0: 2020 2020 2020 2020 5661 6c75 6573 3a0a          Values:.
+0000c5b0: 2020 2020 2020 2020 2020 2020 4546 4645              EFFE
+0000c5c0: 4354 4956 454e 4553 535f 554e 5350 4543  CTIVENESS_UNSPEC
+0000c5d0: 4946 4945 4420 2830 293a 0a20 2020 2020  IFIED (0):.     
+0000c5e0: 2020 2020 2020 2020 2020 2045 6666 6563             Effec
+0000c5f0: 7469 7665 6e65 7373 2069 7320 756e 6b6e  tiveness is unkn
+0000c600: 6f77 6e2e 0a20 2020 2020 2020 2020 2020  own..           
+0000c610: 204c 4f57 2028 3129 3a0a 2020 2020 2020   LOW (1):.      
+0000c620: 2020 2020 2020 2020 2020 4566 6665 6374            Effect
+0000c630: 6976 656e 6573 7320 6973 206c 6f77 2e0a  iveness is low..
+0000c640: 2020 2020 2020 2020 2020 2020 4d45 4449              MEDI
+0000c650: 554d 2028 3229 3a0a 2020 2020 2020 2020  UM (2):.        
+0000c660: 2020 2020 2020 2020 4566 6665 6374 6976          Effectiv
+0000c670: 656e 6573 7320 6973 206d 6564 6975 6d2e  eness is medium.
+0000c680: 0a20 2020 2020 2020 2020 2020 2048 4947  .            HIG
+0000c690: 4820 2833 293a 0a20 2020 2020 2020 2020  H (3):.         
+0000c6a0: 2020 2020 2020 2045 6666 6563 7469 7665         Effective
+0000c6b0: 6e65 7373 2069 7320 6869 6768 2e0a 2020  ness is high..  
+0000c6c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000c6d0: 2020 4546 4645 4354 4956 454e 4553 535f    EFFECTIVENESS_
+0000c6e0: 554e 5350 4543 4946 4945 4420 3d20 300a  UNSPECIFIED = 0.
+0000c6f0: 2020 2020 2020 2020 4c4f 5720 3d20 310a          LOW = 1.
+0000c700: 2020 2020 2020 2020 4d45 4449 554d 203d          MEDIUM =
+0000c710: 2032 0a20 2020 2020 2020 2048 4947 4820   2.        HIGH 
+0000c720: 3d20 330a 0a20 2020 2069 643a 2073 7472  = 3..    id: str
+0000c730: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000c740: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+0000c750: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+0000c760: 6d62 6572 3d31 2c0a 2020 2020 2020 2020  mber=1,.        
+0000c770: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+0000c780: 2020 2029 0a20 2020 206f 6666 6572 5f69     ).    offer_i
+0000c790: 643a 2073 7472 203d 2070 726f 746f 2e46  d: str = proto.F
+0000c7a0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+0000c7b0: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+0000c7c0: 2020 2020 6e75 6d62 6572 3d32 2c0a 2020      number=2,.  
+0000c7d0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+0000c7e0: 7275 652c 0a20 2020 2029 0a20 2020 2074  rue,.    ).    t
+0000c7f0: 6974 6c65 3a20 7374 7220 3d20 7072 6f74  itle: str = prot
+0000c800: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+0000c810: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+0000c820: 2020 2020 2020 206e 756d 6265 723d 332c         number=3,
+0000c830: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+0000c840: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+0000c850: 2020 6272 616e 643a 2073 7472 203d 2070    brand: str = p
+0000c860: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000c870: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+0000c880: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+0000c890: 3d34 2c0a 2020 2020 2020 2020 6f70 7469  =4,.        opti
+0000c8a0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+0000c8b0: 0a20 2020 2063 6174 6567 6f72 795f 6c31  .    category_l1
+0000c8c0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+0000c8d0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+0000c8e0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+0000c8f0: 2020 206e 756d 6265 723d 352c 0a20 2020     number=5,.   
+0000c900: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+0000c910: 7565 2c0a 2020 2020 290a 2020 2020 6361  ue,.    ).    ca
+0000c920: 7465 676f 7279 5f6c 323a 2073 7472 203d  tegory_l2: str =
+0000c930: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+0000c940: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+0000c950: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
+0000c960: 6572 3d36 2c0a 2020 2020 2020 2020 6f70  er=6,.        op
+0000c970: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+0000c980: 2029 0a20 2020 2063 6174 6567 6f72 795f   ).    category_
+0000c990: 6c33 3a20 7374 7220 3d20 7072 6f74 6f2e  l3: str = proto.
+0000c9a0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+0000c9b0: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+0000c9c0: 2020 2020 206e 756d 6265 723d 372c 0a20       number=7,. 
+0000c9d0: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+0000c9e0: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+0000c9f0: 6361 7465 676f 7279 5f6c 343a 2073 7472  category_l4: str
+0000ca00: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000ca10: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+0000ca20: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+0000ca30: 6d62 6572 3d38 2c0a 2020 2020 2020 2020  mber=8,.        
+0000ca40: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+0000ca50: 2020 2029 0a20 2020 2063 6174 6567 6f72     ).    categor
+0000ca60: 795f 6c35 3a20 7374 7220 3d20 7072 6f74  y_l5: str = prot
+0000ca70: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+0000ca80: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+0000ca90: 2020 2020 2020 206e 756d 6265 723d 392c         number=9,
+0000caa0: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+0000cab0: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+0000cac0: 2020 7072 6f64 7563 745f 7479 7065 5f6c    product_type_l
+0000cad0: 313a 2073 7472 203d 2070 726f 746f 2e46  1: str = proto.F
+0000cae0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+0000caf0: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+0000cb00: 2020 2020 6e75 6d62 6572 3d31 302c 0a20      number=10,. 
+0000cb10: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+0000cb20: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+0000cb30: 7072 6f64 7563 745f 7479 7065 5f6c 323a  product_type_l2:
+0000cb40: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
+0000cb50: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+0000cb60: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
+0000cb70: 2020 6e75 6d62 6572 3d31 312c 0a20 2020    number=11,.   
+0000cb80: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+0000cb90: 7565 2c0a 2020 2020 290a 2020 2020 7072  ue,.    ).    pr
+0000cba0: 6f64 7563 745f 7479 7065 5f6c 333a 2073  oduct_type_l3: s
+0000cbb0: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+0000cbc0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+0000cbd0: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+0000cbe0: 6e75 6d62 6572 3d31 322c 0a20 2020 2020  number=12,.     
+0000cbf0: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+0000cc00: 2c0a 2020 2020 290a 2020 2020 7072 6f64  ,.    ).    prod
+0000cc10: 7563 745f 7479 7065 5f6c 343a 2073 7472  uct_type_l4: str
+0000cc20: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000cc30: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+0000cc40: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+0000cc50: 6d62 6572 3d31 332c 0a20 2020 2020 2020  mber=13,.       
+0000cc60: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+0000cc70: 2020 2020 290a 2020 2020 7072 6f64 7563      ).    produc
+0000cc80: 745f 7479 7065 5f6c 353a 2073 7472 203d  t_type_l5: str =
+0000cc90: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+0000cca0: 2020 2020 2020 7072 6f74 6f2e 5354 5249        proto.STRI
+0000ccb0: 4e47 2c0a 2020 2020 2020 2020 6e75 6d62  NG,.        numb
+0000ccc0: 6572 3d31 342c 0a20 2020 2020 2020 206f  er=14,.        o
+0000ccd0: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+0000cce0: 2020 290a 2020 2020 7072 6963 653a 2074    ).    price: t
+0000ccf0: 7970 6573 2e50 7269 6365 203d 2070 726f  ypes.Price = pro
+0000cd00: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+0000cd10: 2020 7072 6f74 6f2e 4d45 5353 4147 452c    proto.MESSAGE,
+0000cd20: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+0000cd30: 3135 2c0a 2020 2020 2020 2020 6d65 7373  15,.        mess
+0000cd40: 6167 653d 7479 7065 732e 5072 6963 652c  age=types.Price,
+0000cd50: 0a20 2020 2029 0a20 2020 2073 7567 6765  .    ).    sugge
+0000cd60: 7374 6564 5f70 7269 6365 3a20 7479 7065  sted_price: type
+0000cd70: 732e 5072 6963 6520 3d20 7072 6f74 6f2e  s.Price = proto.
+0000cd80: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+0000cd90: 726f 746f 2e4d 4553 5341 4745 2c0a 2020  roto.MESSAGE,.  
+0000cda0: 2020 2020 2020 6e75 6d62 6572 3d31 362c        number=16,
+0000cdb0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+0000cdc0: 3d74 7970 6573 2e50 7269 6365 2c0a 2020  =types.Price,.  
+0000cdd0: 2020 290a 2020 2020 7072 6564 6963 7465    ).    predicte
+0000cde0: 645f 696d 7072 6573 7369 6f6e 735f 6368  d_impressions_ch
+0000cdf0: 616e 6765 5f66 7261 6374 696f 6e3a 2066  ange_fraction: f
+0000ce00: 6c6f 6174 203d 2070 726f 746f 2e46 6965  loat = proto.Fie
+0000ce10: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+0000ce20: 6f2e 444f 5542 4c45 2c0a 2020 2020 2020  o.DOUBLE,.      
+0000ce30: 2020 6e75 6d62 6572 3d31 372c 0a20 2020    number=17,.   
+0000ce40: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+0000ce50: 7565 2c0a 2020 2020 290a 2020 2020 7072  ue,.    ).    pr
+0000ce60: 6564 6963 7465 645f 636c 6963 6b73 5f63  edicted_clicks_c
+0000ce70: 6861 6e67 655f 6672 6163 7469 6f6e 3a20  hange_fraction: 
+0000ce80: 666c 6f61 7420 3d20 7072 6f74 6f2e 4669  float = proto.Fi
+0000ce90: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+0000cea0: 746f 2e44 4f55 424c 452c 0a20 2020 2020  to.DOUBLE,.     
+0000ceb0: 2020 206e 756d 6265 723d 3138 2c0a 2020     number=18,.  
+0000cec0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+0000ced0: 7275 652c 0a20 2020 2029 0a20 2020 2070  rue,.    ).    p
+0000cee0: 7265 6469 6374 6564 5f63 6f6e 7665 7273  redicted_convers
+0000cef0: 696f 6e73 5f63 6861 6e67 655f 6672 6163  ions_change_frac
+0000cf00: 7469 6f6e 3a20 666c 6f61 7420 3d20 7072  tion: float = pr
+0000cf10: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+0000cf20: 2020 2070 726f 746f 2e44 4f55 424c 452c     proto.DOUBLE,
+0000cf30: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+0000cf40: 3139 2c0a 2020 2020 2020 2020 6f70 7469  19,.        opti
+0000cf50: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+0000cf60: 0a20 2020 2065 6666 6563 7469 7665 6e65  .    effectivene
+0000cf70: 7373 3a20 4566 6665 6374 6976 656e 6573  ss: Effectivenes
+0000cf80: 7320 3d20 7072 6f74 6f2e 4669 656c 6428  s = proto.Field(
+0000cf90: 0a20 2020 2020 2020 2070 726f 746f 2e45  .        proto.E
+0000cfa0: 4e55 4d2c 0a20 2020 2020 2020 206e 756d  NUM,.        num
+0000cfb0: 6265 723d 3232 2c0a 2020 2020 2020 2020  ber=22,.        
+0000cfc0: 656e 756d 3d45 6666 6563 7469 7665 6e65  enum=Effectivene
+0000cfd0: 7373 2c0a 2020 2020 290a 0a0a 636c 6173  ss,.    )...clas
+0000cfe0: 7320 4265 7374 5365 6c6c 6572 7350 726f  s BestSellersPro
+0000cff0: 6475 6374 436c 7573 7465 7256 6965 7728  ductClusterView(
+0000d000: 7072 6f74 6f2e 4d65 7373 6167 6529 3a0a  proto.Message):.
+0000d010: 2020 2020 7222 2222 4669 656c 6473 2061      r"""Fields a
+0000d020: 7661 696c 6162 6c65 2066 6f72 2071 7565  vailable for que
+0000d030: 7279 2069 6e20 6060 6265 7374 5f73 656c  ry in ``best_sel
+0000d040: 6c65 7273 5f70 726f 6475 6374 5f63 6c75  lers_product_clu
+0000d050: 7374 6572 5f76 6965 7760 600a 2020 2020  ster_view``.    
+0000d060: 7461 626c 652e 0a0a 2020 2020 6042 6573  table...    `Bes
+0000d070: 740a 2020 2020 7365 6c6c 6572 7320 3c68  t.    sellers <h
+0000d080: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
+0000d090: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
+0000d0a0: 6e74 732f 616e 7377 6572 2f39 3438 3836  nts/answer/94886
+0000d0b0: 3739 3e60 5f5f 0a20 2020 2072 6570 6f72  79>`__.    repor
+0000d0c0: 7420 7769 7468 2074 6f70 2070 726f 6475  t with top produ
+0000d0d0: 6374 2063 6c75 7374 6572 732e 2041 2070  ct clusters. A p
+0000d0e0: 726f 6475 6374 2063 6c75 7374 6572 2069  roduct cluster i
+0000d0f0: 7320 6120 6772 6f75 7069 6e67 0a20 2020  s a grouping.   
+0000d100: 2066 6f72 2064 6966 6665 7265 6e74 206f   for different o
+0000d110: 6666 6572 7320 616e 6420 7661 7269 616e  ffers and varian
+0000d120: 7473 2074 6861 7420 7265 7072 6573 656e  ts that represen
+0000d130: 7420 7468 6520 7361 6d65 2070 726f 6475  t the same produ
+0000d140: 6374 2c0a 2020 2020 666f 7220 6578 616d  ct,.    for exam
+0000d150: 706c 652c 2047 6f6f 676c 6520 5069 7865  ple, Google Pixe
+0000d160: 6c20 372e 0a0a 2020 2020 5661 6c75 6573  l 7...    Values
+0000d170: 2061 7265 206f 6e6c 7920 7365 7420 666f   are only set fo
+0000d180: 7220 6669 656c 6473 2072 6571 7565 7374  r fields request
+0000d190: 6564 2065 7870 6c69 6369 746c 7920 696e  ed explicitly in
+0000d1a0: 2074 6865 2072 6571 7565 7374 2773 0a20   the request's. 
+0000d1b0: 2020 2073 6561 7263 6820 7175 6572 792e     search query.
+0000d1c0: 0a0a 0a20 2020 202e 2e20 5f6f 6e65 6f66  ...    .. _oneof
+0000d1d0: 3a20 6874 7470 733a 2f2f 7072 6f74 6f2d  : https://proto-
+0000d1e0: 706c 7573 2d70 7974 686f 6e2e 7265 6164  plus-python.read
+0000d1f0: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
+0000d200: 6162 6c65 2f66 6965 6c64 732e 6874 6d6c  able/fields.html
+0000d210: 236f 6e65 6f66 732d 6d75 7475 616c 6c79  #oneofs-mutually
+0000d220: 2d65 7863 6c75 7369 7665 2d66 6965 6c64  -exclusive-field
+0000d230: 730a 0a20 2020 2041 7474 7269 6275 7465  s..    Attribute
+0000d240: 733a 0a20 2020 2020 2020 2072 6570 6f72  s:.        repor
+0000d250: 745f 6461 7465 2028 676f 6f67 6c65 2e74  t_date (google.t
+0000d260: 7970 652e 6461 7465 5f70 6232 2e44 6174  ype.date_pb2.Dat
+0000d270: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+0000d280: 5265 706f 7274 2064 6174 652e 2054 6865  Report date. The
+0000d290: 2076 616c 7565 206f 6620 7468 6973 2066   value of this f
+0000d2a0: 6965 6c64 2063 616e 206f 6e6c 7920 6265  ield can only be
+0000d2b0: 206f 6e65 206f 6620 7468 650a 2020 2020   one of the.    
+0000d2c0: 2020 2020 2020 2020 666f 6c6c 6f77 696e          followin
+0000d2d0: 673a 0a0a 2020 2020 2020 2020 2020 2020  g:..            
+0000d2e0: 2d20 2054 6865 2066 6972 7374 2064 6179  -  The first day
+0000d2f0: 206f 6620 7468 6520 7765 656b 2028 4d6f   of the week (Mo
+0000d300: 6e64 6179 2920 666f 7220 7765 656b 6c79  nday) for weekly
+0000d310: 2072 6570 6f72 7473 2c0a 2020 2020 2020   reports,.      
+0000d320: 2020 2020 2020 2d20 2054 6865 2066 6972        -  The fir
+0000d330: 7374 2064 6179 206f 6620 7468 6520 6d6f  st day of the mo
+0000d340: 6e74 6820 666f 7220 6d6f 6e74 686c 7920  nth for monthly 
+0000d350: 7265 706f 7274 732e 0a0a 2020 2020 2020  reports...      
+0000d360: 2020 2020 2020 5265 7175 6972 6564 2069        Required i
+0000d370: 6e20 7468 6520 6060 5345 4c45 4354 6060  n the ``SELECT``
+0000d380: 2063 6c61 7573 652e 2049 6620 6120 6060   clause. If a ``
+0000d390: 5748 4552 4560 6020 636f 6e64 6974 696f  WHERE`` conditio
+0000d3a0: 6e0a 2020 2020 2020 2020 2020 2020 6f6e  n.            on
+0000d3b0: 2060 6072 6570 6f72 745f 6461 7465 6060   ``report_date``
+0000d3c0: 2069 7320 6e6f 7420 7370 6563 6966 6965   is not specifie
+0000d3d0: 6420 696e 2074 6865 2071 7565 7279 2c20  d in the query, 
+0000d3e0: 7468 6520 6c61 7465 7374 0a20 2020 2020  the latest.     
+0000d3f0: 2020 2020 2020 2061 7661 696c 6162 6c65         available
+0000d400: 2077 6565 6b6c 7920 6f72 206d 6f6e 7468   weekly or month
+0000d410: 6c79 2072 6570 6f72 7420 6973 2072 6574  ly report is ret
+0000d420: 7572 6e65 642e 0a20 2020 2020 2020 2072  urned..        r
+0000d430: 6570 6f72 745f 6772 616e 756c 6172 6974  eport_granularit
+0000d440: 7920 2867 6f6f 676c 652e 7368 6f70 7069  y (google.shoppi
+0000d450: 6e67 2e6d 6572 6368 616e 745f 7265 706f  ng.merchant_repo
+0000d460: 7274 735f 7631 6265 7461 2e74 7970 6573  rts_v1beta.types
+0000d470: 2e52 6570 6f72 7447 7261 6e75 6c61 7269  .ReportGranulari
+0000d480: 7479 2e52 6570 6f72 7447 7261 6e75 6c61  ty.ReportGranula
+0000d490: 7269 7479 456e 756d 293a 0a20 2020 2020  rityEnum):.     
+0000d4a0: 2020 2020 2020 2047 7261 6e75 6c61 7269         Granulari
+0000d4b0: 7479 206f 6620 7468 6520 7265 706f 7274  ty of the report
+0000d4c0: 2e20 5468 6520 7261 6e6b 696e 6720 6361  . The ranking ca
+0000d4d0: 6e20 6265 2064 6f6e 6520 6f76 6572 2061  n be done over a
+0000d4e0: 0a20 2020 2020 2020 2020 2020 2077 6565  .            wee
+0000d4f0: 6b20 6f72 2061 206d 6f6e 7468 2074 696d  k or a month tim
+0000d500: 6566 7261 6d65 2e0a 0a20 2020 2020 2020  eframe...       
+0000d510: 2020 2020 2052 6571 7569 7265 6420 696e       Required in
+0000d520: 2074 6865 2060 6053 454c 4543 5460 6020   the ``SELECT`` 
+0000d530: 636c 6175 7365 2e20 436f 6e64 6974 696f  clause. Conditio
+0000d540: 6e20 6f6e 0a20 2020 2020 2020 2020 2020  n on.           
+0000d550: 2060 6072 6570 6f72 745f 6772 616e 756c   ``report_granul
+0000d560: 6172 6974 7960 6020 6973 2072 6571 7569  arity`` is requi
+0000d570: 7265 6420 696e 2074 6865 2060 6057 4845  red in the ``WHE
+0000d580: 5245 6060 2063 6c61 7573 652e 0a0a 2020  RE`` clause...  
+0000d590: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+0000d5a0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+0000d5b0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+0000d5c0: 7265 706f 7274 5f67 7261 6e75 6c61 7269  report_granulari
+0000d5d0: 7479 6060 2e0a 2020 2020 2020 2020 7265  ty``..        re
+0000d5e0: 706f 7274 5f63 6f75 6e74 7279 5f63 6f64  port_country_cod
+0000d5f0: 6520 2873 7472 293a 0a20 2020 2020 2020  e (str):.       
+0000d600: 2020 2020 2043 6f75 6e74 7279 2077 6865       Country whe
+0000d610: 7265 2074 6865 2072 616e 6b69 6e67 2069  re the ranking i
+0000d620: 7320 6361 6c63 756c 6174 6564 2e20 5265  s calculated. Re
+0000d630: 7072 6573 656e 7465 6420 696e 2074 6865  presented in the
+0000d640: 0a20 2020 2020 2020 2020 2020 2049 534f  .            ISO
+0000d650: 2033 3136 3620 666f 726d 6174 2e0a 0a20   3166 format... 
+0000d660: 2020 2020 2020 2020 2020 2052 6571 7569             Requi
+0000d670: 7265 6420 696e 2074 6865 2060 6053 454c  red in the ``SEL
+0000d680: 4543 5460 6020 636c 6175 7365 2e20 436f  ECT`` clause. Co
+0000d690: 6e64 6974 696f 6e20 6f6e 0a20 2020 2020  ndition on.     
+0000d6a0: 2020 2020 2020 2060 6072 6570 6f72 745f         ``report_
+0000d6b0: 636f 756e 7472 795f 636f 6465 6060 2069  country_code`` i
+0000d6c0: 7320 7265 7175 6972 6564 2069 6e20 7468  s required in th
+0000d6d0: 6520 6060 5748 4552 4560 6020 636c 6175  e ``WHERE`` clau
+0000d6e0: 7365 2e0a 0a20 2020 2020 2020 2020 2020  se...           
+0000d6f0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+0000d700: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+0000d710: 6660 5f20 6060 5f72 6570 6f72 745f 636f  f`_ ``_report_co
+0000d720: 756e 7472 795f 636f 6465 6060 2e0a 2020  untry_code``..  
+0000d730: 2020 2020 2020 7265 706f 7274 5f63 6174        report_cat
+0000d740: 6567 6f72 795f 6964 2028 696e 7429 3a0a  egory_id (int):.
+0000d750: 2020 2020 2020 2020 2020 2020 476f 6f67              Goog
+0000d760: 6c65 2070 726f 6475 6374 2063 6174 6567  le product categ
+0000d770: 6f72 7920 4944 2074 6f20 6361 6c63 756c  ory ID to calcul
+0000d780: 6174 6520 7468 6520 7261 6e6b 696e 6720  ate the ranking 
+0000d790: 666f 722c 0a20 2020 2020 2020 2020 2020  for,.           
+0000d7a0: 2072 6570 7265 7365 6e74 6564 2069 6e20   represented in 
+0000d7b0: 6047 6f6f 676c 6527 7320 7072 6f64 7563  `Google's produc
+0000d7c0: 740a 2020 2020 2020 2020 2020 2020 7461  t.            ta
+0000d7d0: 786f 6e6f 6d79 203c 6874 7470 733a 2f2f  xonomy <https://
+0000d7e0: 7375 7070 6f72 742e 676f 6f67 6c65 2e63  support.google.c
+0000d7f0: 6f6d 2f6d 6572 6368 616e 7473 2f61 6e73  om/merchants/ans
+0000d800: 7765 722f 3633 3234 3433 363e 605f 5f2e  wer/6324436>`__.
+0000d810: 0a0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
+0000d820: 7175 6972 6564 2069 6e20 7468 6520 6060  quired in the ``
+0000d830: 5345 4c45 4354 6060 2063 6c61 7573 652e  SELECT`` clause.
+0000d840: 2049 6620 6120 6060 5748 4552 4560 6020   If a ``WHERE`` 
+0000d850: 636f 6e64 6974 696f 6e0a 2020 2020 2020  condition.      
+0000d860: 2020 2020 2020 6f6e 2060 6072 6570 6f72        on ``repor
+0000d870: 745f 6361 7465 676f 7279 5f69 6460 6020  t_category_id`` 
+0000d880: 6973 206e 6f74 2073 7065 6369 6669 6564  is not specified
+0000d890: 2069 6e20 7468 6520 7175 6572 792c 0a20   in the query,. 
+0000d8a0: 2020 2020 2020 2020 2020 2072 616e 6b69             ranki
+0000d8b0: 6e67 7320 666f 7220 616c 6c20 746f 702d  ngs for all top-
+0000d8c0: 6c65 7665 6c20 6361 7465 676f 7269 6573  level categories
+0000d8d0: 2061 7265 2072 6574 7572 6e65 642e 0a0a   are returned...
+0000d8e0: 2020 2020 2020 2020 2020 2020 5468 6973              This
+0000d8f0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+0000d900: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+0000d910: 605f 7265 706f 7274 5f63 6174 6567 6f72  `_report_categor
+0000d920: 795f 6964 6060 2e0a 2020 2020 2020 2020  y_id``..        
+0000d930: 7469 746c 6520 2873 7472 293a 0a20 2020  title (str):.   
+0000d940: 2020 2020 2020 2020 2054 6974 6c65 206f           Title o
+0000d950: 6620 7468 6520 7072 6f64 7563 7420 636c  f the product cl
+0000d960: 7573 7465 722e 0a0a 2020 2020 2020 2020  uster...        
+0000d970: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+0000d980: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+0000d990: 6e65 6f66 605f 2060 605f 7469 746c 6560  neof`_ ``_title`
+0000d9a0: 602e 0a20 2020 2020 2020 2062 7261 6e64  `..        brand
+0000d9b0: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+0000d9c0: 2020 2020 4272 616e 6420 6f66 2074 6865      Brand of the
+0000d9d0: 2070 726f 6475 6374 2063 6c75 7374 6572   product cluster
+0000d9e0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
+0000d9f0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
+0000da00: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
+0000da10: 5f20 6060 5f62 7261 6e64 6060 2e0a 2020  _ ``_brand``..  
+0000da20: 2020 2020 2020 6361 7465 676f 7279 5f6c        category_l
+0000da30: 3120 2873 7472 293a 0a20 2020 2020 2020  1 (str):.       
+0000da40: 2020 2020 2050 726f 6475 6374 2063 6174       Product cat
+0000da50: 6567 6f72 7920 2831 7374 206c 6576 656c  egory (1st level
+0000da60: 2920 6f66 2074 6865 2070 726f 6475 6374  ) of the product
+0000da70: 2063 6c75 7374 6572 2c0a 2020 2020 2020   cluster,.      
+0000da80: 2020 2020 2020 7265 7072 6573 656e 7465        represente
+0000da90: 6420 696e 2060 476f 6f67 6c65 2773 2070  d in `Google's p
+0000daa0: 726f 6475 6374 0a20 2020 2020 2020 2020  roduct.         
+0000dab0: 2020 2074 6178 6f6e 6f6d 7920 3c68 7474     taxonomy <htt
+0000dac0: 7073 3a2f 2f73 7570 706f 7274 2e67 6f6f  ps://support.goo
+0000dad0: 676c 652e 636f 6d2f 6d65 7263 6861 6e74  gle.com/merchant
+0000dae0: 732f 616e 7377 6572 2f36 3332 3434 3336  s/answer/6324436
+0000daf0: 3e60 5f5f 2e0a 0a20 2020 2020 2020 2020  >`__...         
+0000db00: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+0000db10: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+0000db20: 656f 6660 5f20 6060 5f63 6174 6567 6f72  eof`_ ``_categor
+0000db30: 795f 6c31 6060 2e0a 2020 2020 2020 2020  y_l1``..        
+0000db40: 6361 7465 676f 7279 5f6c 3220 2873 7472  category_l2 (str
+0000db50: 293a 0a20 2020 2020 2020 2020 2020 2050  ):.            P
+0000db60: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
+0000db70: 2832 6e64 206c 6576 656c 2920 6f66 2074  (2nd level) of t
+0000db80: 6865 2070 726f 6475 6374 2063 6c75 7374  he product clust
+0000db90: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+0000dba0: 7265 7072 6573 656e 7465 6420 696e 2060  represented in `
+0000dbb0: 476f 6f67 6c65 2773 2070 726f 6475 6374  Google's product
+0000dbc0: 0a20 2020 2020 2020 2020 2020 2074 6178  .            tax
+0000dbd0: 6f6e 6f6d 7920 3c68 7474 7073 3a2f 2f73  onomy <https://s
+0000dbe0: 7570 706f 7274 2e67 6f6f 676c 652e 636f  upport.google.co
+0000dbf0: 6d2f 6d65 7263 6861 6e74 732f 616e 7377  m/merchants/answ
+0000dc00: 6572 2f36 3332 3434 3336 3e60 5f5f 2e0a  er/6324436>`__..
+0000dc10: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+0000dc20: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+0000dc30: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+0000dc40: 6060 5f63 6174 6567 6f72 795f 6c32 6060  ``_category_l2``
+0000dc50: 2e0a 2020 2020 2020 2020 6361 7465 676f  ..        catego
+0000dc60: 7279 5f6c 3320 2873 7472 293a 0a20 2020  ry_l3 (str):.   
+0000dc70: 2020 2020 2020 2020 2050 726f 6475 6374           Product
+0000dc80: 2063 6174 6567 6f72 7920 2833 7264 206c   category (3rd l
+0000dc90: 6576 656c 2920 6f66 2074 6865 2070 726f  evel) of the pro
+0000dca0: 6475 6374 2063 6c75 7374 6572 2c0a 2020  duct cluster,.  
+0000dcb0: 2020 2020 2020 2020 2020 7265 7072 6573            repres
+0000dcc0: 656e 7465 6420 696e 2060 476f 6f67 6c65  ented in `Google
+0000dcd0: 2773 2070 726f 6475 6374 0a20 2020 2020  's product.     
+0000dce0: 2020 2020 2020 2074 6178 6f6e 6f6d 7920         taxonomy 
+0000dcf0: 3c68 7474 7073 3a2f 2f73 7570 706f 7274  <https://support
+0000dd00: 2e67 6f6f 676c 652e 636f 6d2f 6d65 7263  .google.com/merc
+0000dd10: 6861 6e74 732f 616e 7377 6572 2f36 3332  hants/answer/632
+0000dd20: 3434 3336 3e60 5f5f 2e0a 0a20 2020 2020  4436>`__...     
+0000dd30: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
+0000dd40: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
+0000dd50: 2060 6f6e 656f 6660 5f20 6060 5f63 6174   `oneof`_ ``_cat
+0000dd60: 6567 6f72 795f 6c33 6060 2e0a 2020 2020  egory_l3``..    
+0000dd70: 2020 2020 6361 7465 676f 7279 5f6c 3420      category_l4 
+0000dd80: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+0000dd90: 2020 2050 726f 6475 6374 2063 6174 6567     Product categ
+0000dda0: 6f72 7920 2834 7468 206c 6576 656c 2920  ory (4th level) 
+0000ddb0: 6f66 2074 6865 2070 726f 6475 6374 2063  of the product c
+0000ddc0: 6c75 7374 6572 2c0a 2020 2020 2020 2020  luster,.        
+0000ddd0: 2020 2020 7265 7072 6573 656e 7465 6420      represented 
+0000dde0: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
+0000ddf0: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
+0000de00: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
+0000de10: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
+0000de20: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
+0000de30: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
+0000de40: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
+0000de50: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+0000de60: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+0000de70: 6660 5f20 6060 5f63 6174 6567 6f72 795f  f`_ ``_category_
+0000de80: 6c34 6060 2e0a 2020 2020 2020 2020 6361  l4``..        ca
+0000de90: 7465 676f 7279 5f6c 3520 2873 7472 293a  tegory_l5 (str):
+0000dea0: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
+0000deb0: 6475 6374 2063 6174 6567 6f72 7920 2835  duct category (5
+0000dec0: 7468 206c 6576 656c 2920 6f66 2074 6865  th level) of the
+0000ded0: 2070 726f 6475 6374 2063 6c75 7374 6572   product cluster
+0000dee0: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
+0000def0: 7072 6573 656e 7465 6420 696e 2060 476f  presented in `Go
+0000df00: 6f67 6c65 2773 2070 726f 6475 6374 0a20  ogle's product. 
+0000df10: 2020 2020 2020 2020 2020 2074 6178 6f6e             taxon
+0000df20: 6f6d 7920 3c68 7474 7073 3a2f 2f73 7570  omy <https://sup
+0000df30: 706f 7274 2e67 6f6f 676c 652e 636f 6d2f  port.google.com/
+0000df40: 6d65 7263 6861 6e74 732f 616e 7377 6572  merchants/answer
+0000df50: 2f36 3332 3434 3336 3e60 5f5f 2e0a 0a20  /6324436>`__... 
+0000df60: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+0000df70: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+0000df80: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+0000df90: 5f63 6174 6567 6f72 795f 6c35 6060 2e0a  _category_l5``..
+0000dfa0: 2020 2020 2020 2020 7661 7269 616e 745f          variant_
+0000dfb0: 6774 696e 7320 284d 7574 6162 6c65 5365  gtins (MutableSe
+0000dfc0: 7175 656e 6365 5b73 7472 5d29 3a0a 2020  quence[str]):.  
+0000dfd0: 2020 2020 2020 2020 2020 4754 494e 7320            GTINs 
+0000dfe0: 6f66 2065 7861 6d70 6c65 2076 6172 6961  of example varia
+0000dff0: 6e74 7320 6f66 2074 6865 2070 726f 6475  nts of the produ
+0000e000: 6374 0a20 2020 2020 2020 2020 2020 2063  ct.            c
+0000e010: 6c75 7374 6572 2e0a 2020 2020 2020 2020  luster..        
+0000e020: 696e 7665 6e74 6f72 795f 7374 6174 7573  inventory_status
+0000e030: 2028 676f 6f67 6c65 2e73 686f 7070 696e   (google.shoppin
+0000e040: 672e 6d65 7263 6861 6e74 5f72 6570 6f72  g.merchant_repor
+0000e050: 7473 5f76 3162 6574 612e 7479 7065 732e  ts_v1beta.types.
+0000e060: 4265 7374 5365 6c6c 6572 7350 726f 6475  BestSellersProdu
+0000e070: 6374 436c 7573 7465 7256 6965 772e 496e  ctClusterView.In
+0000e080: 7665 6e74 6f72 7953 7461 7475 7329 3a0a  ventoryStatus):.
+0000e090: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+0000e0a0: 6865 7220 7468 6520 7072 6f64 7563 7420  her the product 
+0000e0b0: 636c 7573 7465 7220 6973 2060 6049 4e5f  cluster is ``IN_
+0000e0c0: 5354 4f43 4b60 6020 696e 2079 6f75 7220  STOCK`` in your 
+0000e0d0: 7072 6f64 7563 740a 2020 2020 2020 2020  product.        
+0000e0e0: 2020 2020 6461 7461 2073 6f75 7263 6520      data source 
+0000e0f0: 696e 2061 7420 6c65 6173 7420 6f6e 6520  in at least one 
+0000e100: 6f66 2074 6865 2063 6f75 6e74 7269 6573  of the countries
+0000e110: 2c0a 2020 2020 2020 2020 2020 2020 6060  ,.            ``
+0000e120: 4f55 545f 4f46 5f53 544f 434b 6060 2069  OUT_OF_STOCK`` i
+0000e130: 6e20 796f 7572 2070 726f 6475 6374 2064  n your product d
+0000e140: 6174 6120 736f 7572 6365 2069 6e20 616c  ata source in al
+0000e150: 6c0a 2020 2020 2020 2020 2020 2020 636f  l.            co
+0000e160: 756e 7472 6965 732c 206f 7220 6060 4e4f  untries, or ``NO
+0000e170: 545f 494e 5f49 4e56 454e 544f 5259 6060  T_IN_INVENTORY``
+0000e180: 2061 7420 616c 6c2e 0a0a 2020 2020 2020   at all...      
+0000e190: 2020 2020 2020 5468 6520 6669 656c 6420        The field 
+0000e1a0: 646f 6573 6e27 7420 7461 6b65 2074 6865  doesn't take the
+0000e1b0: 2042 6573 7420 7365 6c6c 6572 7320 7265   Best sellers re
+0000e1c0: 706f 7274 2063 6f75 6e74 7279 0a20 2020  port country.   
+0000e1d0: 2020 2020 2020 2020 2066 696c 7465 7220           filter 
+0000e1e0: 696e 746f 2061 6363 6f75 6e74 2e0a 0a20  into account... 
+0000e1f0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+0000e200: 6669 656c 6420 6973 2061 206d 656d 6265  field is a membe
+0000e210: 7220 6f66 2060 6f6e 656f 6660 5f20 6060  r of `oneof`_ ``
+0000e220: 5f69 6e76 656e 746f 7279 5f73 7461 7475  _inventory_statu
+0000e230: 7360 602e 0a20 2020 2020 2020 2062 7261  s``..        bra
+0000e240: 6e64 5f69 6e76 656e 746f 7279 5f73 7461  nd_inventory_sta
+0000e250: 7475 7320 2867 6f6f 676c 652e 7368 6f70  tus (google.shop
+0000e260: 7069 6e67 2e6d 6572 6368 616e 745f 7265  ping.merchant_re
+0000e270: 706f 7274 735f 7631 6265 7461 2e74 7970  ports_v1beta.typ
+0000e280: 6573 2e42 6573 7453 656c 6c65 7273 5072  es.BestSellersPr
+0000e290: 6f64 7563 7443 6c75 7374 6572 5669 6577  oductClusterView
+0000e2a0: 2e49 6e76 656e 746f 7279 5374 6174 7573  .InventoryStatus
+0000e2b0: 293a 0a20 2020 2020 2020 2020 2020 2057  ):.            W
+0000e2c0: 6865 7468 6572 2074 6865 7265 2069 7320  hether there is 
+0000e2d0: 6174 206c 6561 7374 206f 6e65 2070 726f  at least one pro
+0000e2e0: 6475 6374 206f 6620 7468 6520 6272 616e  duct of the bran
+0000e2f0: 6420 6375 7272 656e 746c 790a 2020 2020  d currently.    
+0000e300: 2020 2020 2020 2020 6060 494e 5f53 544f          ``IN_STO
+0000e310: 434b 6060 2069 6e20 796f 7572 2070 726f  CK`` in your pro
+0000e320: 6475 6374 2064 6174 6120 736f 7572 6365  duct data source
+0000e330: 2069 6e20 6174 206c 6561 7374 206f 6e65   in at least one
+0000e340: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
+0000e350: 7468 6520 636f 756e 7472 6965 732c 2061  the countries, a
+0000e360: 6c6c 2070 726f 6475 6374 7320 6172 6520  ll products are 
+0000e370: 6060 4f55 545f 4f46 5f53 544f 434b 6060  ``OUT_OF_STOCK``
+0000e380: 2069 6e20 796f 7572 0a20 2020 2020 2020   in your.       
+0000e390: 2020 2020 2070 726f 6475 6374 2064 6174       product dat
+0000e3a0: 6120 736f 7572 6365 2069 6e20 616c 6c20  a source in all 
+0000e3b0: 636f 756e 7472 6965 732c 206f 720a 2020  countries, or.  
+0000e3c0: 2020 2020 2020 2020 2020 6060 4e4f 545f            ``NOT_
+0000e3d0: 494e 5f49 4e56 454e 544f 5259 6060 2e0a  IN_INVENTORY``..
+0000e3e0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+0000e3f0: 2066 6965 6c64 2064 6f65 736e 2774 2074   field doesn't t
+0000e400: 616b 6520 7468 6520 4265 7374 2073 656c  ake the Best sel
+0000e410: 6c65 7273 2072 6570 6f72 7420 636f 756e  lers report coun
+0000e420: 7472 790a 2020 2020 2020 2020 2020 2020  try.            
+0000e430: 6669 6c74 6572 2069 6e74 6f20 6163 636f  filter into acco
+0000e440: 756e 742e 0a0a 2020 2020 2020 2020 2020  unt...          
+0000e450: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+0000e460: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+0000e470: 6f66 605f 2060 605f 6272 616e 645f 696e  of`_ ``_brand_in
+0000e480: 7665 6e74 6f72 795f 7374 6174 7573 6060  ventory_status``
+0000e490: 2e0a 2020 2020 2020 2020 7261 6e6b 2028  ..        rank (
+0000e4a0: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+0000e4b0: 2020 506f 7075 6c61 7269 7479 206f 6620    Popularity of 
+0000e4c0: 7468 6520 7072 6f64 7563 7420 636c 7573  the product clus
+0000e4d0: 7465 7220 6f6e 2041 6473 2061 6e64 0a20  ter on Ads and. 
+0000e4e0: 2020 2020 2020 2020 2020 206f 7267 616e             organ
+0000e4f0: 6963 2073 7572 6661 6365 732c 2069 6e20  ic surfaces, in 
+0000e500: 7468 6520 7365 6c65 6374 6564 2063 6174  the selected cat
+0000e510: 6567 6f72 7920 616e 640a 2020 2020 2020  egory and.      
+0000e520: 2020 2020 2020 636f 756e 7472 792c 2062        country, b
+0000e530: 6173 6564 206f 6e20 7468 6520 6573 7469  ased on the esti
+0000e540: 6d61 7465 6420 6e75 6d62 6572 206f 6620  mated number of 
+0000e550: 756e 6974 730a 2020 2020 2020 2020 2020  units.          
+0000e560: 2020 736f 6c64 2e0a 0a20 2020 2020 2020    sold...       
+0000e570: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+0000e580: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+0000e590: 6f6e 656f 6660 5f20 6060 5f72 616e 6b60  oneof`_ ``_rank`
+0000e5a0: 602e 0a20 2020 2020 2020 2070 7265 7669  `..        previ
+0000e5b0: 6f75 735f 7261 6e6b 2028 696e 7429 3a0a  ous_rank (int):.
+0000e5c0: 2020 2020 2020 2020 2020 2020 506f 7075              Popu
+0000e5d0: 6c61 7269 7479 2072 616e 6b20 696e 2074  larity rank in t
+0000e5e0: 6865 2070 7265 7669 6f75 7320 7765 656b  he previous week
+0000e5f0: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
+0000e600: 6d6f 6e74 682e 0a0a 2020 2020 2020 2020  month...        
+0000e610: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+0000e620: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+0000e630: 6e65 6f66 605f 2060 605f 7072 6576 696f  neof`_ ``_previo
+0000e640: 7573 5f72 616e 6b60 602e 0a20 2020 2020  us_rank``..     
+0000e650: 2020 2072 656c 6174 6976 655f 6465 6d61     relative_dema
+0000e660: 6e64 2028 676f 6f67 6c65 2e73 686f 7070  nd (google.shopp
+0000e670: 696e 672e 6d65 7263 6861 6e74 5f72 6570  ing.merchant_rep
+0000e680: 6f72 7473 5f76 3162 6574 612e 7479 7065  orts_v1beta.type
+0000e690: 732e 5265 6c61 7469 7665 4465 6d61 6e64  s.RelativeDemand
+0000e6a0: 2e52 656c 6174 6976 6544 656d 616e 6445  .RelativeDemandE
+0000e6b0: 6e75 6d29 3a0a 2020 2020 2020 2020 2020  num):.          
+0000e6c0: 2020 4573 7469 6d61 7465 6420 6465 6d61    Estimated dema
+0000e6d0: 6e64 2069 6e20 7265 6c61 7469 6f6e 2074  nd in relation t
+0000e6e0: 6f20 7468 6520 7072 6f64 7563 740a 2020  o the product.  
+0000e6f0: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
+0000e700: 7220 7769 7468 2074 6865 2068 6967 6865  r with the highe
+0000e710: 7374 2070 6f70 756c 6172 6974 7920 7261  st popularity ra
+0000e720: 6e6b 2069 6e20 7468 650a 2020 2020 2020  nk in the.      
+0000e730: 2020 2020 2020 7361 6d65 2063 6174 6567        same categ
+0000e740: 6f72 7920 616e 6420 636f 756e 7472 792e  ory and country.
+0000e750: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+0000e760: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+0000e770: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+0000e780: 2060 605f 7265 6c61 7469 7665 5f64 656d   ``_relative_dem
+0000e790: 616e 6460 602e 0a20 2020 2020 2020 2070  and``..        p
+0000e7a0: 7265 7669 6f75 735f 7265 6c61 7469 7665  revious_relative
+0000e7b0: 5f64 656d 616e 6420 2867 6f6f 676c 652e  _demand (google.
+0000e7c0: 7368 6f70 7069 6e67 2e6d 6572 6368 616e  shopping.merchan
+0000e7d0: 745f 7265 706f 7274 735f 7631 6265 7461  t_reports_v1beta
+0000e7e0: 2e74 7970 6573 2e52 656c 6174 6976 6544  .types.RelativeD
+0000e7f0: 656d 616e 642e 5265 6c61 7469 7665 4465  emand.RelativeDe
+0000e800: 6d61 6e64 456e 756d 293a 0a20 2020 2020  mandEnum):.     
+0000e810: 2020 2020 2020 2045 7374 696d 6174 6564         Estimated
+0000e820: 2064 656d 616e 6420 696e 2072 656c 6174   demand in relat
+0000e830: 696f 6e20 746f 2074 6865 2070 726f 6475  ion to the produ
+0000e840: 6374 0a20 2020 2020 2020 2020 2020 2063  ct.            c
+0000e850: 6c75 7374 6572 2077 6974 6820 7468 6520  luster with the 
+0000e860: 6869 6768 6573 7420 706f 7075 6c61 7269  highest populari
+0000e870: 7479 2072 616e 6b20 696e 2074 6865 0a20  ty rank in the. 
+0000e880: 2020 2020 2020 2020 2020 2073 616d 6520             same 
+0000e890: 6361 7465 676f 7279 2061 6e64 2063 6f75  category and cou
+0000e8a0: 6e74 7279 2069 6e20 7468 6520 7072 6576  ntry in the prev
+0000e8b0: 696f 7573 2077 6565 6b0a 2020 2020 2020  ious week.      
+0000e8c0: 2020 2020 2020 6f72 206d 6f6e 7468 2e0a        or month..
+0000e8d0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+0000e8e0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+0000e8f0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+0000e900: 6060 5f70 7265 7669 6f75 735f 7265 6c61  ``_previous_rela
+0000e910: 7469 7665 5f64 656d 616e 6460 602e 0a20  tive_demand``.. 
+0000e920: 2020 2020 2020 2072 656c 6174 6976 655f         relative_
+0000e930: 6465 6d61 6e64 5f63 6861 6e67 6520 2867  demand_change (g
+0000e940: 6f6f 676c 652e 7368 6f70 7069 6e67 2e6d  oogle.shopping.m
+0000e950: 6572 6368 616e 745f 7265 706f 7274 735f  erchant_reports_
+0000e960: 7631 6265 7461 2e74 7970 6573 2e52 656c  v1beta.types.Rel
+0000e970: 6174 6976 6544 656d 616e 6443 6861 6e67  ativeDemandChang
+0000e980: 6554 7970 652e 5265 6c61 7469 7665 4465  eType.RelativeDe
+0000e990: 6d61 6e64 4368 616e 6765 5479 7065 456e  mandChangeTypeEn
+0000e9a0: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
+0000e9b0: 2043 6861 6e67 6520 696e 2074 6865 2065   Change in the e
+0000e9c0: 7374 696d 6174 6564 2064 656d 616e 642e  stimated demand.
+0000e9d0: 2057 6865 7468 6572 2069 740a 2020 2020   Whether it.    
+0000e9e0: 2020 2020 2020 2020 726f 7365 2c20 7361          rose, sa
+0000e9f0: 6e6b 206f 7220 7265 6d61 696e 6564 2066  nk or remained f
+0000ea00: 6c61 742e 0a0a 2020 2020 2020 2020 2020  lat...          
+0000ea10: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+0000ea20: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+0000ea30: 6f66 605f 2060 605f 7265 6c61 7469 7665  of`_ ``_relative
+0000ea40: 5f64 656d 616e 645f 6368 616e 6765 6060  _demand_change``
+0000ea50: 2e0a 2020 2020 2222 220a 0a20 2020 2063  ..    """..    c
+0000ea60: 6c61 7373 2049 6e76 656e 746f 7279 5374  lass InventorySt
+0000ea70: 6174 7573 2870 726f 746f 2e45 6e75 6d29  atus(proto.Enum)
+0000ea80: 3a0a 2020 2020 2020 2020 7222 2222 5374  :.        r"""St
+0000ea90: 6174 7573 206f 6620 7468 6520 7072 6f64  atus of the prod
+0000eaa0: 7563 7420 636c 7573 7465 7220 6f72 2062  uct cluster or b
+0000eab0: 7261 6e64 2069 6e20 796f 7572 2069 6e76  rand in your inv
+0000eac0: 656e 746f 7279 2e0a 0a20 2020 2020 2020  entory...       
+0000ead0: 2056 616c 7565 733a 0a20 2020 2020 2020   Values:.       
+0000eae0: 2020 2020 2049 4e56 454e 544f 5259 5f53       INVENTORY_S
+0000eaf0: 5441 5455 535f 554e 5350 4543 4946 4945  TATUS_UNSPECIFIE
+0000eb00: 4420 2830 293a 0a20 2020 2020 2020 2020  D (0):.         
+0000eb10: 2020 2020 2020 204e 6f74 2073 7065 6369         Not speci
+0000eb20: 6669 6564 2e0a 2020 2020 2020 2020 2020  fied..          
+0000eb30: 2020 494e 5f53 544f 434b 2028 3129 3a0a    IN_STOCK (1):.
+0000eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb50: 596f 7520 6861 7665 2061 2070 726f 6475  You have a produ
+0000eb60: 6374 2066 6f72 2074 6869 7320 7072 6f64  ct for this prod
+0000eb70: 7563 7420 636c 7573 7465 720a 2020 2020  uct cluster.    
+0000eb80: 2020 2020 2020 2020 2020 2020 6f72 2062              or b
+0000eb90: 7261 6e64 2069 6e20 7374 6f63 6b2e 0a20  rand in stock.. 
+0000eba0: 2020 2020 2020 2020 2020 204f 5554 5f4f             OUT_O
+0000ebb0: 465f 5354 4f43 4b20 2832 293a 0a20 2020  F_STOCK (2):.   
+0000ebc0: 2020 2020 2020 2020 2020 2020 2059 6f75               You
+0000ebd0: 2068 6176 6520 6120 7072 6f64 7563 7420   have a product 
+0000ebe0: 666f 7220 7468 6973 2070 726f 6475 6374  for this product
+0000ebf0: 2063 6c75 7374 6572 0a20 2020 2020 2020   cluster.       
+0000ec00: 2020 2020 2020 2020 206f 7220 6272 616e           or bran
+0000ec10: 6420 696e 2069 6e76 656e 746f 7279 2062  d in inventory b
+0000ec20: 7574 2069 7420 6973 2063 7572 7265 6e74  ut it is current
+0000ec30: 6c79 206f 7574 206f 660a 2020 2020 2020  ly out of.      
+0000ec40: 2020 2020 2020 2020 2020 7374 6f63 6b2e            stock.
+0000ec50: 0a20 2020 2020 2020 2020 2020 204e 4f54  .            NOT
+0000ec60: 5f49 4e5f 494e 5645 4e54 4f52 5920 2833  _IN_INVENTORY (3
+0000ec70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000ec80: 2020 2059 6f75 2064 6f20 6e6f 7420 6861     You do not ha
+0000ec90: 7665 2061 2070 726f 6475 6374 2066 6f72  ve a product for
+0000eca0: 2074 6869 7320 7072 6f64 7563 740a 2020   this product.  
+0000ecb0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+0000ecc0: 7573 7465 7220 6f72 2062 7261 6e64 2069  uster or brand i
+0000ecd0: 6e20 696e 7665 6e74 6f72 792e 0a20 2020  n inventory..   
+0000ece0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000ecf0: 2049 4e56 454e 544f 5259 5f53 5441 5455   INVENTORY_STATU
+0000ed00: 535f 554e 5350 4543 4946 4945 4420 3d20  S_UNSPECIFIED = 
+0000ed10: 300a 2020 2020 2020 2020 494e 5f53 544f  0.        IN_STO
+0000ed20: 434b 203d 2031 0a20 2020 2020 2020 204f  CK = 1.        O
+0000ed30: 5554 5f4f 465f 5354 4f43 4b20 3d20 320a  UT_OF_STOCK = 2.
+0000ed40: 2020 2020 2020 2020 4e4f 545f 494e 5f49          NOT_IN_I
+0000ed50: 4e56 454e 544f 5259 203d 2033 0a0a 2020  NVENTORY = 3..  
+0000ed60: 2020 7265 706f 7274 5f64 6174 653a 2064    report_date: d
+0000ed70: 6174 655f 7062 322e 4461 7465 203d 2070  ate_pb2.Date = p
+0000ed80: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000ed90: 2020 2020 7072 6f74 6f2e 4d45 5353 4147      proto.MESSAG
+0000eda0: 452c 0a20 2020 2020 2020 206e 756d 6265  E,.        numbe
+0000edb0: 723d 312c 0a20 2020 2020 2020 206d 6573  r=1,.        mes
+0000edc0: 7361 6765 3d64 6174 655f 7062 322e 4461  sage=date_pb2.Da
+0000edd0: 7465 2c0a 2020 2020 290a 2020 2020 7265  te,.    ).    re
+0000ede0: 706f 7274 5f67 7261 6e75 6c61 7269 7479  port_granularity
+0000edf0: 3a20 2252 6570 6f72 7447 7261 6e75 6c61  : "ReportGranula
+0000ee00: 7269 7479 2e52 6570 6f72 7447 7261 6e75  rity.ReportGranu
+0000ee10: 6c61 7269 7479 456e 756d 2220 3d20 7072  larityEnum" = pr
+0000ee20: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+0000ee30: 2020 2070 726f 746f 2e45 4e55 4d2c 0a20     proto.ENUM,. 
+0000ee40: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
+0000ee50: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+0000ee60: 6c3d 5472 7565 2c0a 2020 2020 2020 2020  l=True,.        
+0000ee70: 656e 756d 3d22 5265 706f 7274 4772 616e  enum="ReportGran
+0000ee80: 756c 6172 6974 792e 5265 706f 7274 4772  ularity.ReportGr
+0000ee90: 616e 756c 6172 6974 7945 6e75 6d22 2c0a  anularityEnum",.
+0000eea0: 2020 2020 290a 2020 2020 7265 706f 7274      ).    report
+0000eeb0: 5f63 6f75 6e74 7279 5f63 6f64 653a 2073  _country_code: s
+0000eec0: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+0000eed0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+0000eee0: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+0000eef0: 6e75 6d62 6572 3d33 2c0a 2020 2020 2020  number=3,.      
+0000ef00: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+0000ef10: 0a20 2020 2029 0a20 2020 2072 6570 6f72  .    ).    repor
+0000ef20: 745f 6361 7465 676f 7279 5f69 643a 2069  t_category_id: i
+0000ef30: 6e74 203d 2070 726f 746f 2e46 6965 6c64  nt = proto.Field
+0000ef40: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+0000ef50: 494e 5436 342c 0a20 2020 2020 2020 206e  INT64,.        n
+0000ef60: 756d 6265 723d 342c 0a20 2020 2020 2020  umber=4,.       
+0000ef70: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+0000ef80: 2020 2020 290a 2020 2020 7469 746c 653a      ).    title:
+0000ef90: 2073 7472 203d 2070 726f 746f 2e46 6965   str = proto.Fie
+0000efa0: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+0000efb0: 6f2e 5354 5249 4e47 2c0a 2020 2020 2020  o.STRING,.      
+0000efc0: 2020 6e75 6d62 6572 3d36 2c0a 2020 2020    number=6,.    
+0000efd0: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+0000efe0: 652c 0a20 2020 2029 0a20 2020 2062 7261  e,.    ).    bra
+0000eff0: 6e64 3a20 7374 7220 3d20 7072 6f74 6f2e  nd: str = proto.
+0000f000: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+0000f010: 726f 746f 2e53 5452 494e 472c 0a20 2020  roto.STRING,.   
+0000f020: 2020 2020 206e 756d 6265 723d 372c 0a20       number=7,. 
+0000f030: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+0000f040: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+0000f050: 6361 7465 676f 7279 5f6c 313a 2073 7472  category_l1: str
+0000f060: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+0000f070: 2020 2020 2020 2020 7072 6f74 6f2e 5354          proto.ST
+0000f080: 5249 4e47 2c0a 2020 2020 2020 2020 6e75  RING,.        nu
+0000f090: 6d62 6572 3d38 2c0a 2020 2020 2020 2020  mber=8,.        
+0000f0a0: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+0000f0b0: 2020 2029 0a20 2020 2063 6174 6567 6f72     ).    categor
+0000f0c0: 795f 6c32 3a20 7374 7220 3d20 7072 6f74  y_l2: str = prot
+0000f0d0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+0000f0e0: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+0000f0f0: 2020 2020 2020 206e 756d 6265 723d 392c         number=9,
+0000f100: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+0000f110: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+0000f120: 2020 6361 7465 676f 7279 5f6c 333a 2073    category_l3: s
+0000f130: 7472 203d 2070 726f 746f 2e46 6965 6c64  tr = proto.Field
+0000f140: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+0000f150: 5354 5249 4e47 2c0a 2020 2020 2020 2020  STRING,.        
+0000f160: 6e75 6d62 6572 3d31 302c 0a20 2020 2020  number=10,.     
+0000f170: 2020 206f 7074 696f 6e61 6c3d 5472 7565     optional=True
+0000f180: 2c0a 2020 2020 290a 2020 2020 6361 7465  ,.    ).    cate
+0000f190: 676f 7279 5f6c 343a 2073 7472 203d 2070  gory_l4: str = p
+0000f1a0: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000f1b0: 2020 2020 7072 6f74 6f2e 5354 5249 4e47      proto.STRING
+0000f1c0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+0000f1d0: 3d31 312c 0a20 2020 2020 2020 206f 7074  =11,.        opt
+0000f1e0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+0000f1f0: 290a 2020 2020 6361 7465 676f 7279 5f6c  ).    category_l
+0000f200: 353a 2073 7472 203d 2070 726f 746f 2e46  5: str = proto.F
+0000f210: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+0000f220: 6f74 6f2e 5354 5249 4e47 2c0a 2020 2020  oto.STRING,.    
+0000f230: 2020 2020 6e75 6d62 6572 3d31 322c 0a20      number=12,. 
+0000f240: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+0000f250: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+0000f260: 7661 7269 616e 745f 6774 696e 733a 204d  variant_gtins: M
+0000f270: 7574 6162 6c65 5365 7175 656e 6365 5b73  utableSequence[s
+0000f280: 7472 5d20 3d20 7072 6f74 6f2e 5265 7065  tr] = proto.Repe
+0000f290: 6174 6564 4669 656c 6428 0a20 2020 2020  atedField(.     
+0000f2a0: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
+0000f2b0: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+0000f2c0: 3133 2c0a 2020 2020 290a 2020 2020 696e  13,.    ).    in
+0000f2d0: 7665 6e74 6f72 795f 7374 6174 7573 3a20  ventory_status: 
+0000f2e0: 496e 7665 6e74 6f72 7953 7461 7475 7320  InventoryStatus 
+0000f2f0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+0000f300: 2020 2020 2020 2070 726f 746f 2e45 4e55         proto.ENU
+0000f310: 4d2c 0a20 2020 2020 2020 206e 756d 6265  M,.        numbe
+0000f320: 723d 3134 2c0a 2020 2020 2020 2020 6f70  r=14,.        op
+0000f330: 7469 6f6e 616c 3d54 7275 652c 0a20 2020  tional=True,.   
+0000f340: 2020 2020 2065 6e75 6d3d 496e 7665 6e74       enum=Invent
+0000f350: 6f72 7953 7461 7475 732c 0a20 2020 2029  oryStatus,.    )
+0000f360: 0a20 2020 2062 7261 6e64 5f69 6e76 656e  .    brand_inven
+0000f370: 746f 7279 5f73 7461 7475 733a 2049 6e76  tory_status: Inv
+0000f380: 656e 746f 7279 5374 6174 7573 203d 2070  entoryStatus = p
+0000f390: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+0000f3a0: 2020 2020 7072 6f74 6f2e 454e 554d 2c0a      proto.ENUM,.
+0000f3b0: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
+0000f3c0: 352c 0a20 2020 2020 2020 206f 7074 696f  5,.        optio
+0000f3d0: 6e61 6c3d 5472 7565 2c0a 2020 2020 2020  nal=True,.      
+0000f3e0: 2020 656e 756d 3d49 6e76 656e 746f 7279    enum=Inventory
+0000f3f0: 5374 6174 7573 2c0a 2020 2020 290a 2020  Status,.    ).  
+0000f400: 2020 7261 6e6b 3a20 696e 7420 3d20 7072    rank: int = pr
+0000f410: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+0000f420: 2020 2070 726f 746f 2e49 4e54 3634 2c0a     proto.INT64,.
+0000f430: 2020 2020 2020 2020 6e75 6d62 6572 3d31          number=1
+0000f440: 362c 0a20 2020 2020 2020 206f 7074 696f  6,.        optio
+0000f450: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
+0000f460: 2020 2020 7072 6576 696f 7573 5f72 616e      previous_ran
+0000f470: 6b3a 2069 6e74 203d 2070 726f 746f 2e46  k: int = proto.F
+0000f480: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+0000f490: 6f74 6f2e 494e 5436 342c 0a20 2020 2020  oto.INT64,.     
+0000f4a0: 2020 206e 756d 6265 723d 3137 2c0a 2020     number=17,.  
+0000f4b0: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+0000f4c0: 7275 652c 0a20 2020 2029 0a20 2020 2072  rue,.    ).    r
+0000f4d0: 656c 6174 6976 655f 6465 6d61 6e64 3a20  elative_demand: 
+0000f4e0: 2252 656c 6174 6976 6544 656d 616e 642e  "RelativeDemand.
+0000f4f0: 5265 6c61 7469 7665 4465 6d61 6e64 456e  RelativeDemandEn
+0000f500: 756d 2220 3d20 7072 6f74 6f2e 4669 656c  um" = proto.Fiel
+0000f510: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+0000f520: 2e45 4e55 4d2c 0a20 2020 2020 2020 206e  .ENUM,.        n
+0000f530: 756d 6265 723d 3138 2c0a 2020 2020 2020  umber=18,.      
+0000f540: 2020 6f70 7469 6f6e 616c 3d54 7275 652c    optional=True,
+0000f550: 0a20 2020 2020 2020 2065 6e75 6d3d 2252  .        enum="R
+0000f560: 656c 6174 6976 6544 656d 616e 642e 5265  elativeDemand.Re
+0000f570: 6c61 7469 7665 4465 6d61 6e64 456e 756d  lativeDemandEnum
+0000f580: 222c 0a20 2020 2029 0a20 2020 2070 7265  ",.    ).    pre
+0000f590: 7669 6f75 735f 7265 6c61 7469 7665 5f64  vious_relative_d
+0000f5a0: 656d 616e 643a 2022 5265 6c61 7469 7665  emand: "Relative
+0000f5b0: 4465 6d61 6e64 2e52 656c 6174 6976 6544  Demand.RelativeD
+0000f5c0: 656d 616e 6445 6e75 6d22 203d 2070 726f  emandEnum" = pro
+0000f5d0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+0000f5e0: 2020 7072 6f74 6f2e 454e 554d 2c0a 2020    proto.ENUM,.  
+0000f5f0: 2020 2020 2020 6e75 6d62 6572 3d31 392c        number=19,
+0000f600: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+0000f610: 6c3d 5472 7565 2c0a 2020 2020 2020 2020  l=True,.        
+0000f620: 656e 756d 3d22 5265 6c61 7469 7665 4465  enum="RelativeDe
+0000f630: 6d61 6e64 2e52 656c 6174 6976 6544 656d  mand.RelativeDem
+0000f640: 616e 6445 6e75 6d22 2c0a 2020 2020 290a  andEnum",.    ).
+0000f650: 2020 2020 7265 6c61 7469 7665 5f64 656d      relative_dem
+0000f660: 616e 645f 6368 616e 6765 3a20 2252 656c  and_change: "Rel
+0000f670: 6174 6976 6544 656d 616e 6443 6861 6e67  ativeDemandChang
+0000f680: 6554 7970 652e 5265 6c61 7469 7665 4465  eType.RelativeDe
+0000f690: 6d61 6e64 4368 616e 6765 5479 7065 456e  mandChangeTypeEn
+0000f6a0: 756d 2220 3d20 280a 2020 2020 2020 2020  um" = (.        
+0000f6b0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+0000f6c0: 2020 2020 2020 2020 2070 726f 746f 2e45           proto.E
+0000f6d0: 4e55 4d2c 0a20 2020 2020 2020 2020 2020  NUM,.           
+0000f6e0: 206e 756d 6265 723d 3230 2c0a 2020 2020   number=20,.    
+0000f6f0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+0000f700: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+0000f710: 2020 2065 6e75 6d3d 2252 656c 6174 6976     enum="Relativ
+0000f720: 6544 656d 616e 6443 6861 6e67 6554 7970  eDemandChangeTyp
+0000f730: 652e 5265 6c61 7469 7665 4465 6d61 6e64  e.RelativeDemand
+0000f740: 4368 616e 6765 5479 7065 456e 756d 222c  ChangeTypeEnum",
+0000f750: 0a20 2020 2020 2020 2029 0a20 2020 2029  .        ).    )
+0000f760: 0a0a 0a63 6c61 7373 2042 6573 7453 656c  ...class BestSel
+0000f770: 6c65 7273 4272 616e 6456 6965 7728 7072  lersBrandView(pr
+0000f780: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
+0000f790: 2020 7222 2222 4669 656c 6473 2061 7661    r"""Fields ava
+0000f7a0: 696c 6162 6c65 2066 6f72 2071 7565 7279  ilable for query
+0000f7b0: 2069 6e20 6060 6265 7374 5f73 656c 6c65   in ``best_selle
+0000f7c0: 7273 5f62 7261 6e64 5f76 6965 7760 6020  rs_brand_view`` 
+0000f7d0: 7461 626c 652e 0a0a 2020 2020 6042 6573  table...    `Bes
+0000f7e0: 740a 2020 2020 7365 6c6c 6572 7320 3c68  t.    sellers <h
+0000f7f0: 7474 7073 3a2f 2f73 7570 706f 7274 2e67  ttps://support.g
+0000f800: 6f6f 676c 652e 636f 6d2f 6d65 7263 6861  oogle.com/mercha
+0000f810: 6e74 732f 616e 7377 6572 2f39 3438 3836  nts/answer/94886
+0000f820: 3739 3e60 5f5f 0a20 2020 2072 6570 6f72  79>`__.    repor
+0000f830: 7420 7769 7468 2074 6f70 2062 7261 6e64  t with top brand
+0000f840: 732e 0a0a 2020 2020 5661 6c75 6573 2061  s...    Values a
+0000f850: 7265 206f 6e6c 7920 7365 7420 666f 7220  re only set for 
+0000f860: 6669 656c 6473 2072 6571 7565 7374 6564  fields requested
+0000f870: 2065 7870 6c69 6369 746c 7920 696e 2074   explicitly in t
+0000f880: 6865 2072 6571 7565 7374 2773 0a20 2020  he request's.   
+0000f890: 2073 6561 7263 6820 7175 6572 792e 0a0a   search query...
+0000f8a0: 0a20 2020 202e 2e20 5f6f 6e65 6f66 3a20  .    .. _oneof: 
+0000f8b0: 6874 7470 733a 2f2f 7072 6f74 6f2d 706c  https://proto-pl
+0000f8c0: 7573 2d70 7974 686f 6e2e 7265 6164 7468  us-python.readth
+0000f8d0: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+0000f8e0: 6c65 2f66 6965 6c64 732e 6874 6d6c 236f  le/fields.html#o
+0000f8f0: 6e65 6f66 732d 6d75 7475 616c 6c79 2d65  neofs-mutually-e
+0000f900: 7863 6c75 7369 7665 2d66 6965 6c64 730a  xclusive-fields.
+0000f910: 0a20 2020 2041 7474 7269 6275 7465 733a  .    Attributes:
+0000f920: 0a20 2020 2020 2020 2072 6570 6f72 745f  .        report_
+0000f930: 6461 7465 2028 676f 6f67 6c65 2e74 7970  date (google.typ
+0000f940: 652e 6461 7465 5f70 6232 2e44 6174 6529  e.date_pb2.Date)
+0000f950: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
+0000f960: 706f 7274 2064 6174 652e 2054 6865 2076  port date. The v
+0000f970: 616c 7565 206f 6620 7468 6973 2066 6965  alue of this fie
+0000f980: 6c64 2063 616e 206f 6e6c 7920 6265 206f  ld can only be o
+0000f990: 6e65 206f 6620 7468 650a 2020 2020 2020  ne of the.      
+0000f9a0: 2020 2020 2020 666f 6c6c 6f77 696e 673a        following:
+0000f9b0: 0a0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
+0000f9c0: 2054 6865 2066 6972 7374 2064 6179 206f   The first day o
+0000f9d0: 6620 7468 6520 7765 656b 2028 4d6f 6e64  f the week (Mond
+0000f9e0: 6179 2920 666f 7220 7765 656b 6c79 2072  ay) for weekly r
+0000f9f0: 6570 6f72 7473 2c0a 2020 2020 2020 2020  eports,.        
+0000fa00: 2020 2020 2d20 2054 6865 2066 6972 7374      -  The first
+0000fa10: 2064 6179 206f 6620 7468 6520 6d6f 6e74   day of the mont
+0000fa20: 6820 666f 7220 6d6f 6e74 686c 7920 7265  h for monthly re
+0000fa30: 706f 7274 732e 0a0a 2020 2020 2020 2020  ports...        
+0000fa40: 2020 2020 5265 7175 6972 6564 2069 6e20      Required in 
+0000fa50: 7468 6520 6060 5345 4c45 4354 6060 2063  the ``SELECT`` c
+0000fa60: 6c61 7573 652e 2049 6620 6120 6060 5748  lause. If a ``WH
+0000fa70: 4552 4560 6020 636f 6e64 6974 696f 6e0a  ERE`` condition.
+0000fa80: 2020 2020 2020 2020 2020 2020 6f6e 2060              on `
+0000fa90: 6072 6570 6f72 745f 6461 7465 6060 2069  `report_date`` i
+0000faa0: 7320 6e6f 7420 7370 6563 6966 6965 6420  s not specified 
+0000fab0: 696e 2074 6865 2071 7565 7279 2c20 7468  in the query, th
+0000fac0: 6520 6c61 7465 7374 0a20 2020 2020 2020  e latest.       
+0000fad0: 2020 2020 2061 7661 696c 6162 6c65 2077       available w
+0000fae0: 6565 6b6c 7920 6f72 206d 6f6e 7468 6c79  eekly or monthly
+0000faf0: 2072 6570 6f72 7420 6973 2072 6574 7572   report is retur
+0000fb00: 6e65 642e 0a20 2020 2020 2020 2072 6570  ned..        rep
+0000fb10: 6f72 745f 6772 616e 756c 6172 6974 7920  ort_granularity 
+0000fb20: 2867 6f6f 676c 652e 7368 6f70 7069 6e67  (google.shopping
+0000fb30: 2e6d 6572 6368 616e 745f 7265 706f 7274  .merchant_report
+0000fb40: 735f 7631 6265 7461 2e74 7970 6573 2e52  s_v1beta.types.R
+0000fb50: 6570 6f72 7447 7261 6e75 6c61 7269 7479  eportGranularity
+0000fb60: 2e52 6570 6f72 7447 7261 6e75 6c61 7269  .ReportGranulari
+0000fb70: 7479 456e 756d 293a 0a20 2020 2020 2020  tyEnum):.       
+0000fb80: 2020 2020 2047 7261 6e75 6c61 7269 7479       Granularity
+0000fb90: 206f 6620 7468 6520 7265 706f 7274 2e20   of the report. 
+0000fba0: 5468 6520 7261 6e6b 696e 6720 6361 6e20  The ranking can 
+0000fbb0: 6265 2064 6f6e 6520 6f76 6572 2061 0a20  be done over a. 
+0000fbc0: 2020 2020 2020 2020 2020 2077 6565 6b20             week 
+0000fbd0: 6f72 2061 206d 6f6e 7468 2074 696d 6566  or a month timef
+0000fbe0: 7261 6d65 2e0a 0a20 2020 2020 2020 2020  rame...         
+0000fbf0: 2020 2052 6571 7569 7265 6420 696e 2074     Required in t
+0000fc00: 6865 2060 6053 454c 4543 5460 6020 636c  he ``SELECT`` cl
+0000fc10: 6175 7365 2e20 436f 6e64 6974 696f 6e20  ause. Condition 
+0000fc20: 6f6e 0a20 2020 2020 2020 2020 2020 2060  on.            `
+0000fc30: 6072 6570 6f72 745f 6772 616e 756c 6172  `report_granular
+0000fc40: 6974 7960 6020 6973 2072 6571 7569 7265  ity`` is require
+0000fc50: 6420 696e 2074 6865 2060 6057 4845 5245  d in the ``WHERE
+0000fc60: 6060 2063 6c61 7573 652e 0a0a 2020 2020  `` clause...    
+0000fc70: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+0000fc80: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+0000fc90: 6620 606f 6e65 6f66 605f 2060 605f 7265  f `oneof`_ ``_re
+0000fca0: 706f 7274 5f67 7261 6e75 6c61 7269 7479  port_granularity
+0000fcb0: 6060 2e0a 2020 2020 2020 2020 7265 706f  ``..        repo
+0000fcc0: 7274 5f63 6f75 6e74 7279 5f63 6f64 6520  rt_country_code 
+0000fcd0: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+0000fce0: 2020 2043 6f75 6e74 7279 2077 6865 7265     Country where
+0000fcf0: 2074 6865 2072 616e 6b69 6e67 2069 7320   the ranking is 
+0000fd00: 6361 6c63 756c 6174 6564 2e20 5265 7072  calculated. Repr
+0000fd10: 6573 656e 7465 6420 696e 2074 6865 0a20  esented in the. 
+0000fd20: 2020 2020 2020 2020 2020 2049 534f 2033             ISO 3
+0000fd30: 3136 3620 666f 726d 6174 2e0a 0a20 2020  166 format...   
+0000fd40: 2020 2020 2020 2020 2052 6571 7569 7265           Require
+0000fd50: 6420 696e 2074 6865 2060 6053 454c 4543  d in the ``SELEC
+0000fd60: 5460 6020 636c 6175 7365 2e20 436f 6e64  T`` clause. Cond
+0000fd70: 6974 696f 6e20 6f6e 0a20 2020 2020 2020  ition on.       
+0000fd80: 2020 2020 2060 6072 6570 6f72 745f 636f       ``report_co
+0000fd90: 756e 7472 795f 636f 6465 6060 2069 7320  untry_code`` is 
+0000fda0: 7265 7175 6972 6564 2069 6e20 7468 6520  required in the 
+0000fdb0: 6060 5748 4552 4560 6020 636c 6175 7365  ``WHERE`` clause
+0000fdc0: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
+0000fdd0: 6869 7320 6669 656c 6420 6973 2061 206d  his field is a m
+0000fde0: 656d 6265 7220 6f66 2060 6f6e 656f 6660  ember of `oneof`
+0000fdf0: 5f20 6060 5f72 6570 6f72 745f 636f 756e  _ ``_report_coun
+0000fe00: 7472 795f 636f 6465 6060 2e0a 2020 2020  try_code``..    
+0000fe10: 2020 2020 7265 706f 7274 5f63 6174 6567      report_categ
+0000fe20: 6f72 795f 6964 2028 696e 7429 3a0a 2020  ory_id (int):.  
+0000fe30: 2020 2020 2020 2020 2020 476f 6f67 6c65            Google
+0000fe40: 2070 726f 6475 6374 2063 6174 6567 6f72   product categor
+0000fe50: 7920 4944 2074 6f20 6361 6c63 756c 6174  y ID to calculat
+0000fe60: 6520 7468 6520 7261 6e6b 696e 6720 666f  e the ranking fo
+0000fe70: 722c 0a20 2020 2020 2020 2020 2020 2072  r,.            r
+0000fe80: 6570 7265 7365 6e74 6564 2069 6e20 6047  epresented in `G
+0000fe90: 6f6f 676c 6527 7320 7072 6f64 7563 740a  oogle's product.
+0000fea0: 2020 2020 2020 2020 2020 2020 7461 786f              taxo
+0000feb0: 6e6f 6d79 203c 6874 7470 733a 2f2f 7375  nomy <https://su
+0000fec0: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
+0000fed0: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
+0000fee0: 722f 3633 3234 3433 363e 605f 5f2e 0a0a  r/6324436>`__...
+0000fef0: 2020 2020 2020 2020 2020 2020 5265 7175              Requ
+0000ff00: 6972 6564 2069 6e20 7468 6520 6060 5345  ired in the ``SE
+0000ff10: 4c45 4354 6060 2063 6c61 7573 652e 2049  LECT`` clause. I
+0000ff20: 6620 6120 6060 5748 4552 4560 6020 636f  f a ``WHERE`` co
+0000ff30: 6e64 6974 696f 6e0a 2020 2020 2020 2020  ndition.        
+0000ff40: 2020 2020 6f6e 2060 6072 6570 6f72 745f      on ``report_
+0000ff50: 6361 7465 676f 7279 5f69 6460 6020 6973  category_id`` is
+0000ff60: 206e 6f74 2073 7065 6369 6669 6564 2069   not specified i
+0000ff70: 6e20 7468 6520 7175 6572 792c 0a20 2020  n the query,.   
+0000ff80: 2020 2020 2020 2020 2072 616e 6b69 6e67           ranking
+0000ff90: 7320 666f 7220 616c 6c20 746f 702d 6c65  s for all top-le
+0000ffa0: 7665 6c20 6361 7465 676f 7269 6573 2061  vel categories a
+0000ffb0: 7265 2072 6574 7572 6e65 642e 0a0a 2020  re returned...  
+0000ffc0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+0000ffd0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+0000ffe0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+0000fff0: 7265 706f 7274 5f63 6174 6567 6f72 795f  report_category_
+00010000: 6964 6060 2e0a 2020 2020 2020 2020 6272  id``..        br
+00010010: 616e 6420 2873 7472 293a 0a20 2020 2020  and (str):.     
+00010020: 2020 2020 2020 204e 616d 6520 6f66 2074         Name of t
+00010030: 6865 2062 7261 6e64 2e0a 0a20 2020 2020  he brand...     
+00010040: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
+00010050: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
+00010060: 2060 6f6e 656f 6660 5f20 6060 5f62 7261   `oneof`_ ``_bra
+00010070: 6e64 6060 2e0a 2020 2020 2020 2020 7261  nd``..        ra
+00010080: 6e6b 2028 696e 7429 3a0a 2020 2020 2020  nk (int):.      
+00010090: 2020 2020 2020 506f 7075 6c61 7269 7479        Popularity
+000100a0: 206f 6620 7468 6520 6272 616e 6420 6f6e   of the brand on
+000100b0: 2041 6473 2061 6e64 206f 7267 616e 6963   Ads and organic
+000100c0: 0a20 2020 2020 2020 2020 2020 2073 7572  .            sur
+000100d0: 6661 6365 732c 2069 6e20 7468 6520 7365  faces, in the se
+000100e0: 6c65 6374 6564 2063 6174 6567 6f72 7920  lected category 
+000100f0: 616e 6420 636f 756e 7472 792c 0a20 2020  and country,.   
+00010100: 2020 2020 2020 2020 2062 6173 6564 206f           based o
+00010110: 6e20 7468 6520 6573 7469 6d61 7465 6420  n the estimated 
+00010120: 6e75 6d62 6572 206f 6620 756e 6974 7320  number of units 
+00010130: 736f 6c64 2e0a 0a20 2020 2020 2020 2020  sold...         
+00010140: 2020 2054 6869 7320 6669 656c 6420 6973     This field is
+00010150: 2061 206d 656d 6265 7220 6f66 2060 6f6e   a member of `on
+00010160: 656f 6660 5f20 6060 5f72 616e 6b60 602e  eof`_ ``_rank``.
+00010170: 0a20 2020 2020 2020 2070 7265 7669 6f75  .        previou
+00010180: 735f 7261 6e6b 2028 696e 7429 3a0a 2020  s_rank (int):.  
+00010190: 2020 2020 2020 2020 2020 506f 7075 6c61            Popula
+000101a0: 7269 7479 2072 616e 6b20 696e 2074 6865  rity rank in the
+000101b0: 2070 7265 7669 6f75 7320 7765 656b 206f   previous week o
+000101c0: 720a 2020 2020 2020 2020 2020 2020 6d6f  r.            mo
+000101d0: 6e74 682e 0a0a 2020 2020 2020 2020 2020  nth...          
+000101e0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+000101f0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00010200: 6f66 605f 2060 605f 7072 6576 696f 7573  of`_ ``_previous
+00010210: 5f72 616e 6b60 602e 0a20 2020 2020 2020  _rank``..       
+00010220: 2072 656c 6174 6976 655f 6465 6d61 6e64   relative_demand
+00010230: 2028 676f 6f67 6c65 2e73 686f 7070 696e   (google.shoppin
+00010240: 672e 6d65 7263 6861 6e74 5f72 6570 6f72  g.merchant_repor
+00010250: 7473 5f76 3162 6574 612e 7479 7065 732e  ts_v1beta.types.
+00010260: 5265 6c61 7469 7665 4465 6d61 6e64 2e52  RelativeDemand.R
+00010270: 656c 6174 6976 6544 656d 616e 6445 6e75  elativeDemandEnu
+00010280: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
+00010290: 4573 7469 6d61 7465 6420 6465 6d61 6e64  Estimated demand
+000102a0: 2069 6e20 7265 6c61 7469 6f6e 2074 6f20   in relation to 
+000102b0: 7468 6520 6272 616e 640a 2020 2020 2020  the brand.      
+000102c0: 2020 2020 2020 7769 7468 2074 6865 2068        with the h
+000102d0: 6967 6865 7374 2070 6f70 756c 6172 6974  ighest popularit
+000102e0: 7920 7261 6e6b 2069 6e20 7468 6520 7361  y rank in the sa
+000102f0: 6d65 0a20 2020 2020 2020 2020 2020 2063  me.            c
+00010300: 6174 6567 6f72 7920 616e 6420 636f 756e  ategory and coun
+00010310: 7472 792e 0a0a 2020 2020 2020 2020 2020  try...          
+00010320: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00010330: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00010340: 6f66 605f 2060 605f 7265 6c61 7469 7665  of`_ ``_relative
+00010350: 5f64 656d 616e 6460 602e 0a20 2020 2020  _demand``..     
+00010360: 2020 2070 7265 7669 6f75 735f 7265 6c61     previous_rela
+00010370: 7469 7665 5f64 656d 616e 6420 2867 6f6f  tive_demand (goo
+00010380: 676c 652e 7368 6f70 7069 6e67 2e6d 6572  gle.shopping.mer
+00010390: 6368 616e 745f 7265 706f 7274 735f 7631  chant_reports_v1
+000103a0: 6265 7461 2e74 7970 6573 2e52 656c 6174  beta.types.Relat
+000103b0: 6976 6544 656d 616e 642e 5265 6c61 7469  iveDemand.Relati
+000103c0: 7665 4465 6d61 6e64 456e 756d 293a 0a20  veDemandEnum):. 
+000103d0: 2020 2020 2020 2020 2020 2045 7374 696d             Estim
+000103e0: 6174 6564 2064 656d 616e 6420 696e 2072  ated demand in r
+000103f0: 656c 6174 696f 6e20 746f 2074 6865 2062  elation to the b
+00010400: 7261 6e64 0a20 2020 2020 2020 2020 2020  rand.           
+00010410: 2077 6974 6820 7468 6520 6869 6768 6573   with the highes
+00010420: 7420 706f 7075 6c61 7269 7479 2072 616e  t popularity ran
+00010430: 6b20 696e 2074 6865 2073 616d 650a 2020  k in the same.  
+00010440: 2020 2020 2020 2020 2020 6361 7465 676f            catego
+00010450: 7279 2061 6e64 2063 6f75 6e74 7279 2069  ry and country i
+00010460: 6e20 7468 6520 7072 6576 696f 7573 2077  n the previous w
+00010470: 6565 6b20 6f72 0a20 2020 2020 2020 2020  eek or.         
+00010480: 2020 206d 6f6e 7468 2e0a 0a20 2020 2020     month...     
+00010490: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
+000104a0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
+000104b0: 2060 6f6e 656f 6660 5f20 6060 5f70 7265   `oneof`_ ``_pre
+000104c0: 7669 6f75 735f 7265 6c61 7469 7665 5f64  vious_relative_d
+000104d0: 656d 616e 6460 602e 0a20 2020 2020 2020  emand``..       
+000104e0: 2072 656c 6174 6976 655f 6465 6d61 6e64   relative_demand
+000104f0: 5f63 6861 6e67 6520 2867 6f6f 676c 652e  _change (google.
+00010500: 7368 6f70 7069 6e67 2e6d 6572 6368 616e  shopping.merchan
+00010510: 745f 7265 706f 7274 735f 7631 6265 7461  t_reports_v1beta
+00010520: 2e74 7970 6573 2e52 656c 6174 6976 6544  .types.RelativeD
+00010530: 656d 616e 6443 6861 6e67 6554 7970 652e  emandChangeType.
+00010540: 5265 6c61 7469 7665 4465 6d61 6e64 4368  RelativeDemandCh
+00010550: 616e 6765 5479 7065 456e 756d 293a 0a20  angeTypeEnum):. 
+00010560: 2020 2020 2020 2020 2020 2043 6861 6e67             Chang
+00010570: 6520 696e 2074 6865 2065 7374 696d 6174  e in the estimat
+00010580: 6564 2064 656d 616e 642e 2057 6865 7468  ed demand. Wheth
+00010590: 6572 2069 740a 2020 2020 2020 2020 2020  er it.          
+000105a0: 2020 726f 7365 2c20 7361 6e6b 206f 7220    rose, sank or 
+000105b0: 7265 6d61 696e 6564 2066 6c61 742e 0a0a  remained flat...
+000105c0: 2020 2020 2020 2020 2020 2020 5468 6973              This
+000105d0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+000105e0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+000105f0: 605f 7265 6c61 7469 7665 5f64 656d 616e  `_relative_deman
+00010600: 645f 6368 616e 6765 6060 2e0a 2020 2020  d_change``..    
+00010610: 2222 220a 0a20 2020 2072 6570 6f72 745f  """..    report_
+00010620: 6461 7465 3a20 6461 7465 5f70 6232 2e44  date: date_pb2.D
+00010630: 6174 6520 3d20 7072 6f74 6f2e 4669 656c  ate = proto.Fiel
+00010640: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+00010650: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
+00010660: 2020 6e75 6d62 6572 3d31 2c0a 2020 2020    number=1,.    
+00010670: 2020 2020 6d65 7373 6167 653d 6461 7465      message=date
+00010680: 5f70 6232 2e44 6174 652c 0a20 2020 2029  _pb2.Date,.    )
+00010690: 0a20 2020 2072 6570 6f72 745f 6772 616e  .    report_gran
+000106a0: 756c 6172 6974 793a 2022 5265 706f 7274  ularity: "Report
+000106b0: 4772 616e 756c 6172 6974 792e 5265 706f  Granularity.Repo
+000106c0: 7274 4772 616e 756c 6172 6974 7945 6e75  rtGranularityEnu
+000106d0: 6d22 203d 2070 726f 746f 2e46 6965 6c64  m" = proto.Field
+000106e0: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+000106f0: 454e 554d 2c0a 2020 2020 2020 2020 6e75  ENUM,.        nu
+00010700: 6d62 6572 3d32 2c0a 2020 2020 2020 2020  mber=2,.        
+00010710: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00010720: 2020 2020 2020 2065 6e75 6d3d 2252 6570         enum="Rep
+00010730: 6f72 7447 7261 6e75 6c61 7269 7479 2e52  ortGranularity.R
+00010740: 6570 6f72 7447 7261 6e75 6c61 7269 7479  eportGranularity
+00010750: 456e 756d 222c 0a20 2020 2029 0a20 2020  Enum",.    ).   
+00010760: 2072 6570 6f72 745f 636f 756e 7472 795f   report_country_
+00010770: 636f 6465 3a20 7374 7220 3d20 7072 6f74  code: str = prot
+00010780: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00010790: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+000107a0: 2020 2020 2020 206e 756d 6265 723d 332c         number=3,
+000107b0: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+000107c0: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+000107d0: 2020 7265 706f 7274 5f63 6174 6567 6f72    report_categor
+000107e0: 795f 6964 3a20 696e 7420 3d20 7072 6f74  y_id: int = prot
+000107f0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00010800: 2070 726f 746f 2e49 4e54 3634 2c0a 2020   proto.INT64,.  
+00010810: 2020 2020 2020 6e75 6d62 6572 3d34 2c0a        number=4,.
+00010820: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00010830: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+00010840: 2062 7261 6e64 3a20 7374 7220 3d20 7072   brand: str = pr
+00010850: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+00010860: 2020 2070 726f 746f 2e53 5452 494e 472c     proto.STRING,
+00010870: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+00010880: 362c 0a20 2020 2020 2020 206f 7074 696f  6,.        optio
+00010890: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
+000108a0: 2020 2020 7261 6e6b 3a20 696e 7420 3d20      rank: int = 
+000108b0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+000108c0: 2020 2020 2070 726f 746f 2e49 4e54 3634       proto.INT64
+000108d0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+000108e0: 3d37 2c0a 2020 2020 2020 2020 6f70 7469  =7,.        opti
+000108f0: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+00010900: 0a20 2020 2070 7265 7669 6f75 735f 7261  .    previous_ra
+00010910: 6e6b 3a20 696e 7420 3d20 7072 6f74 6f2e  nk: int = proto.
+00010920: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00010930: 726f 746f 2e49 4e54 3634 2c0a 2020 2020  roto.INT64,.    
+00010940: 2020 2020 6e75 6d62 6572 3d38 2c0a 2020      number=8,.  
+00010950: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+00010960: 7275 652c 0a20 2020 2029 0a20 2020 2072  rue,.    ).    r
+00010970: 656c 6174 6976 655f 6465 6d61 6e64 3a20  elative_demand: 
+00010980: 2252 656c 6174 6976 6544 656d 616e 642e  "RelativeDemand.
+00010990: 5265 6c61 7469 7665 4465 6d61 6e64 456e  RelativeDemandEn
+000109a0: 756d 2220 3d20 7072 6f74 6f2e 4669 656c  um" = proto.Fiel
+000109b0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+000109c0: 2e45 4e55 4d2c 0a20 2020 2020 2020 206e  .ENUM,.        n
+000109d0: 756d 6265 723d 392c 0a20 2020 2020 2020  umber=9,.       
+000109e0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+000109f0: 2020 2020 2020 2020 656e 756d 3d22 5265          enum="Re
+00010a00: 6c61 7469 7665 4465 6d61 6e64 2e52 656c  lativeDemand.Rel
+00010a10: 6174 6976 6544 656d 616e 6445 6e75 6d22  ativeDemandEnum"
+00010a20: 2c0a 2020 2020 290a 2020 2020 7072 6576  ,.    ).    prev
+00010a30: 696f 7573 5f72 656c 6174 6976 655f 6465  ious_relative_de
+00010a40: 6d61 6e64 3a20 2252 656c 6174 6976 6544  mand: "RelativeD
+00010a50: 656d 616e 642e 5265 6c61 7469 7665 4465  emand.RelativeDe
+00010a60: 6d61 6e64 456e 756d 2220 3d20 7072 6f74  mandEnum" = prot
+00010a70: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00010a80: 2070 726f 746f 2e45 4e55 4d2c 0a20 2020   proto.ENUM,.   
+00010a90: 2020 2020 206e 756d 6265 723d 3130 2c0a       number=10,.
+00010aa0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00010ab0: 3d54 7275 652c 0a20 2020 2020 2020 2065  =True,.        e
+00010ac0: 6e75 6d3d 2252 656c 6174 6976 6544 656d  num="RelativeDem
+00010ad0: 616e 642e 5265 6c61 7469 7665 4465 6d61  and.RelativeDema
+00010ae0: 6e64 456e 756d 222c 0a20 2020 2029 0a20  ndEnum",.    ). 
+00010af0: 2020 2072 656c 6174 6976 655f 6465 6d61     relative_dema
+00010b00: 6e64 5f63 6861 6e67 653a 2022 5265 6c61  nd_change: "Rela
+00010b10: 7469 7665 4465 6d61 6e64 4368 616e 6765  tiveDemandChange
+00010b20: 5479 7065 2e52 656c 6174 6976 6544 656d  Type.RelativeDem
+00010b30: 616e 6443 6861 6e67 6554 7970 6545 6e75  andChangeTypeEnu
+00010b40: 6d22 203d 2028 0a20 2020 2020 2020 2070  m" = (.        p
+00010b50: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00010b60: 2020 2020 2020 2020 7072 6f74 6f2e 454e          proto.EN
+00010b70: 554d 2c0a 2020 2020 2020 2020 2020 2020  UM,.            
+00010b80: 6e75 6d62 6572 3d31 312c 0a20 2020 2020  number=11,.     
+00010b90: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+00010ba0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00010bb0: 2020 656e 756d 3d22 5265 6c61 7469 7665    enum="Relative
+00010bc0: 4465 6d61 6e64 4368 616e 6765 5479 7065  DemandChangeType
+00010bd0: 2e52 656c 6174 6976 6544 656d 616e 6443  .RelativeDemandC
+00010be0: 6861 6e67 6554 7970 6545 6e75 6d22 2c0a  hangeTypeEnum",.
+00010bf0: 2020 2020 2020 2020 290a 2020 2020 290a          ).    ).
+00010c00: 0a0a 636c 6173 7320 4e6f 6e50 726f 6475  ..class NonProdu
+00010c10: 6374 5065 7266 6f72 6d61 6e63 6556 6965  ctPerformanceVie
+00010c20: 7728 7072 6f74 6f2e 4d65 7373 6167 6529  w(proto.Message)
+00010c30: 3a0a 2020 2020 7222 2222 4669 656c 6473  :.    r"""Fields
+00010c40: 2061 7661 696c 6162 6c65 2066 6f72 2071   available for q
+00010c50: 7565 7279 2069 6e20 6060 6e6f 6e5f 7072  uery in ``non_pr
+00010c60: 6f64 7563 745f 7065 7266 6f72 6d61 6e63  oduct_performanc
+00010c70: 655f 7669 6577 6060 0a20 2020 2074 6162  e_view``.    tab
+00010c80: 6c65 2e0a 0a20 2020 2050 6572 666f 726d  le...    Perform
+00010c90: 616e 6365 2064 6174 6120 6f6e 2069 6d61  ance data on ima
+00010ca0: 6765 7320 616e 6420 6f6e 6c69 6e65 2073  ges and online s
+00010cb0: 746f 7265 206c 696e 6b73 206c 6561 6469  tore links leadi
+00010cc0: 6e67 2074 6f20 796f 7572 0a20 2020 206e  ng to your.    n
+00010cd0: 6f6e 2d70 726f 6475 6374 2070 6167 6573  on-product pages
+00010ce0: 2e20 5468 6973 2069 6e63 6c75 6465 7320  . This includes 
+00010cf0: 7065 7266 6f72 6d61 6e63 6520 6d65 7472  performance metr
+00010d00: 6963 7320 2866 6f72 2065 7861 6d70 6c65  ics (for example
+00010d10: 2c0a 2020 2020 6060 636c 6963 6b73 6060  ,.    ``clicks``
+00010d20: 2920 616e 6420 6469 6d65 6e73 696f 6e73  ) and dimensions
+00010d30: 2061 6363 6f72 6469 6e67 2074 6f20 7768   according to wh
+00010d40: 6963 6820 7065 7266 6f72 6d61 6e63 6520  ich performance 
+00010d50: 6d65 7472 6963 730a 2020 2020 6172 6520  metrics.    are 
+00010d60: 7365 676d 656e 7465 6420 2866 6f72 2065  segmented (for e
+00010d70: 7861 6d70 6c65 2c20 6060 6461 7465 6060  xample, ``date``
+00010d80: 292e 0a0a 2020 2020 5365 676d 656e 7420  )...    Segment 
+00010d90: 6669 656c 6473 2063 616e 6e6f 7420 6265  fields cannot be
+00010da0: 2073 656c 6563 7465 6420 696e 2071 7565   selected in que
+00010db0: 7269 6573 2077 6974 686f 7574 2061 6c73  ries without als
+00010dc0: 6f20 7365 6c65 6374 696e 670a 2020 2020  o selecting.    
+00010dd0: 6174 206c 6561 7374 206f 6e65 206d 6574  at least one met
+00010de0: 7269 6320 6669 656c 642e 0a0a 2020 2020  ric field...    
+00010df0: 5661 6c75 6573 2061 7265 206f 6e6c 7920  Values are only 
+00010e00: 7365 7420 666f 7220 6669 656c 6473 2072  set for fields r
+00010e10: 6571 7565 7374 6564 2065 7870 6c69 6369  equested explici
+00010e20: 746c 7920 696e 2074 6865 2072 6571 7565  tly in the reque
+00010e30: 7374 2773 0a20 2020 2073 6561 7263 6820  st's.    search 
+00010e40: 7175 6572 792e 0a0a 0a20 2020 202e 2e20  query....    .. 
+00010e50: 5f6f 6e65 6f66 3a20 6874 7470 733a 2f2f  _oneof: https://
+00010e60: 7072 6f74 6f2d 706c 7573 2d70 7974 686f  proto-plus-pytho
+00010e70: 6e2e 7265 6164 7468 6564 6f63 732e 696f  n.readthedocs.io
+00010e80: 2f65 6e2f 7374 6162 6c65 2f66 6965 6c64  /en/stable/field
+00010e90: 732e 6874 6d6c 236f 6e65 6f66 732d 6d75  s.html#oneofs-mu
+00010ea0: 7475 616c 6c79 2d65 7863 6c75 7369 7665  tually-exclusive
+00010eb0: 2d66 6965 6c64 730a 0a20 2020 2041 7474  -fields..    Att
+00010ec0: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
+00010ed0: 2064 6174 6520 2867 6f6f 676c 652e 7479   date (google.ty
+00010ee0: 7065 2e64 6174 655f 7062 322e 4461 7465  pe.date_pb2.Date
+00010ef0: 293a 0a20 2020 2020 2020 2020 2020 2044  ):.            D
+00010f00: 6174 6520 696e 2074 6865 206d 6572 6368  ate in the merch
+00010f10: 616e 7420 7469 6d65 7a6f 6e65 2074 6f20  ant timezone to 
+00010f20: 7768 6963 6820 6d65 7472 6963 7320 6170  which metrics ap
+00010f30: 706c 792e 0a20 2020 2020 2020 2020 2020  ply..           
+00010f40: 2053 6567 6d65 6e74 2e0a 0a20 2020 2020   Segment...     
+00010f50: 2020 2020 2020 2043 6f6e 6469 7469 6f6e         Condition
+00010f60: 206f 6e20 6060 6461 7465 6060 2069 7320   on ``date`` is 
+00010f70: 7265 7175 6972 6564 2069 6e20 7468 6520  required in the 
+00010f80: 6060 5748 4552 4560 6020 636c 6175 7365  ``WHERE`` clause
+00010f90: 2e0a 2020 2020 2020 2020 7765 656b 2028  ..        week (
+00010fa0: 676f 6f67 6c65 2e74 7970 652e 6461 7465  google.type.date
+00010fb0: 5f70 6232 2e44 6174 6529 3a0a 2020 2020  _pb2.Date):.    
+00010fc0: 2020 2020 2020 2020 4669 7273 7420 6461          First da
+00010fd0: 7920 6f66 2074 6865 2077 6565 6b20 284d  y of the week (M
+00010fe0: 6f6e 6461 7929 206f 6620 7468 6520 6d65  onday) of the me
+00010ff0: 7472 6963 730a 2020 2020 2020 2020 2020  trics.          
+00011000: 2020 6461 7465 2069 6e20 7468 6520 6d65    date in the me
+00011010: 7263 6861 6e74 2074 696d 657a 6f6e 652e  rchant timezone.
+00011020: 2053 6567 6d65 6e74 2e0a 2020 2020 2020   Segment..      
+00011030: 2020 636c 6963 6b73 2028 696e 7429 3a0a    clicks (int):.
+00011040: 2020 2020 2020 2020 2020 2020 4e75 6d62              Numb
+00011050: 6572 206f 6620 636c 6963 6b73 206f 6e20  er of clicks on 
+00011060: 696d 6167 6573 2061 6e64 206f 6e6c 696e  images and onlin
+00011070: 6520 7374 6f72 650a 2020 2020 2020 2020  e store.        
+00011080: 2020 2020 6c69 6e6b 7320 6c65 6164 696e      links leadin
+00011090: 6720 746f 2079 6f75 7220 6e6f 6e2d 7072  g to your non-pr
+000110a0: 6f64 7563 7420 7061 6765 732e 204d 6574  oduct pages. Met
+000110b0: 7269 632e 0a0a 2020 2020 2020 2020 2020  ric...          
+000110c0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+000110d0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+000110e0: 6f66 605f 2060 605f 636c 6963 6b73 6060  of`_ ``_clicks``
+000110f0: 2e0a 2020 2020 2020 2020 696d 7072 6573  ..        impres
+00011100: 7369 6f6e 7320 2869 6e74 293a 0a20 2020  sions (int):.   
+00011110: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
+00011120: 6f66 2074 696d 6573 2069 6d61 6765 7320  of times images 
+00011130: 616e 6420 6f6e 6c69 6e65 2073 746f 7265  and online store
+00011140: 206c 696e 6b73 0a20 2020 2020 2020 2020   links.         
+00011150: 2020 206c 6561 6469 6e67 2074 6f20 796f     leading to yo
+00011160: 7572 206e 6f6e 2d70 726f 6475 6374 2070  ur non-product p
+00011170: 6167 6573 2077 6572 6520 7368 6f77 6e2e  ages were shown.
+00011180: 0a20 2020 2020 2020 2020 2020 204d 6574  .            Met
+00011190: 7269 632e 0a0a 2020 2020 2020 2020 2020  ric...          
+000111a0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+000111b0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+000111c0: 6f66 605f 2060 605f 696d 7072 6573 7369  of`_ ``_impressi
+000111d0: 6f6e 7360 602e 0a20 2020 2020 2020 2063  ons``..        c
+000111e0: 6c69 636b 5f74 6872 6f75 6768 5f72 6174  lick_through_rat
+000111f0: 6520 2866 6c6f 6174 293a 0a20 2020 2020  e (float):.     
+00011200: 2020 2020 2020 2043 6c69 636b 2d74 6872         Click-thr
+00011210: 6f75 6768 2072 6174 6520 2d20 7468 6520  ough rate - the 
+00011220: 6e75 6d62 6572 206f 6620 636c 6963 6b73  number of clicks
+00011230: 2028 6060 636c 6963 6b73 6060 290a 2020   (``clicks``).  
+00011240: 2020 2020 2020 2020 2020 6469 7669 6465            divide
+00011250: 6420 6279 2074 6865 206e 756d 6265 7220  d by the number 
+00011260: 6f66 2069 6d70 7265 7373 696f 6e73 2028  of impressions (
+00011270: 6060 696d 7072 6573 7369 6f6e 7360 6029  ``impressions``)
+00011280: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
+00011290: 696d 6167 6573 2061 6e64 206f 6e6c 696e  images and onlin
+000112a0: 6520 7374 6f72 6520 6c69 6e6b 7320 6c65  e store links le
+000112b0: 6164 696e 6720 746f 2079 6f75 7220 6e6f  ading to your no
+000112c0: 6e2d 7072 6f64 7563 740a 2020 2020 2020  n-product.      
+000112d0: 2020 2020 2020 7061 6765 732e 204d 6574        pages. Met
+000112e0: 7269 632e 0a0a 2020 2020 2020 2020 2020  ric...          
+000112f0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00011300: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00011310: 6f66 605f 2060 605f 636c 6963 6b5f 7468  of`_ ``_click_th
+00011320: 726f 7567 685f 7261 7465 6060 2e0a 2020  rough_rate``..  
+00011330: 2020 2222 220a 0a20 2020 2064 6174 653a    """..    date:
+00011340: 2064 6174 655f 7062 322e 4461 7465 203d   date_pb2.Date =
+00011350: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00011360: 2020 2020 2020 7072 6f74 6f2e 4d45 5353        proto.MESS
+00011370: 4147 452c 0a20 2020 2020 2020 206e 756d  AGE,.        num
+00011380: 6265 723d 312c 0a20 2020 2020 2020 206d  ber=1,.        m
+00011390: 6573 7361 6765 3d64 6174 655f 7062 322e  essage=date_pb2.
+000113a0: 4461 7465 2c0a 2020 2020 290a 2020 2020  Date,.    ).    
+000113b0: 7765 656b 3a20 6461 7465 5f70 6232 2e44  week: date_pb2.D
+000113c0: 6174 6520 3d20 7072 6f74 6f2e 4669 656c  ate = proto.Fiel
+000113d0: 6428 0a20 2020 2020 2020 2070 726f 746f  d(.        proto
+000113e0: 2e4d 4553 5341 4745 2c0a 2020 2020 2020  .MESSAGE,.      
+000113f0: 2020 6e75 6d62 6572 3d32 2c0a 2020 2020    number=2,.    
+00011400: 2020 2020 6d65 7373 6167 653d 6461 7465      message=date
+00011410: 5f70 6232 2e44 6174 652c 0a20 2020 2029  _pb2.Date,.    )
+00011420: 0a20 2020 2063 6c69 636b 733a 2069 6e74  .    clicks: int
+00011430: 203d 2070 726f 746f 2e46 6965 6c64 280a   = proto.Field(.
+00011440: 2020 2020 2020 2020 7072 6f74 6f2e 494e          proto.IN
+00011450: 5436 342c 0a20 2020 2020 2020 206e 756d  T64,.        num
+00011460: 6265 723d 332c 0a20 2020 2020 2020 206f  ber=3,.        o
+00011470: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+00011480: 2020 290a 2020 2020 696d 7072 6573 7369    ).    impressi
+00011490: 6f6e 733a 2069 6e74 203d 2070 726f 746f  ons: int = proto
+000114a0: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+000114b0: 7072 6f74 6f2e 494e 5436 342c 0a20 2020  proto.INT64,.   
+000114c0: 2020 2020 206e 756d 6265 723d 342c 0a20       number=4,. 
+000114d0: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+000114e0: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+000114f0: 636c 6963 6b5f 7468 726f 7567 685f 7261  click_through_ra
+00011500: 7465 3a20 666c 6f61 7420 3d20 7072 6f74  te: float = prot
+00011510: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00011520: 2070 726f 746f 2e44 4f55 424c 452c 0a20   proto.DOUBLE,. 
+00011530: 2020 2020 2020 206e 756d 6265 723d 352c         number=5,
+00011540: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+00011550: 6c3d 5472 7565 2c0a 2020 2020 290a 0a0a  l=True,.    )...
+00011560: 636c 6173 7320 436f 6d70 6574 6974 6976  class Competitiv
+00011570: 6556 6973 6962 696c 6974 7943 6f6d 7065  eVisibilityCompe
+00011580: 7469 746f 7256 6965 7728 7072 6f74 6f2e  titorView(proto.
+00011590: 4d65 7373 6167 6529 3a0a 2020 2020 7222  Message):.    r"
+000115a0: 2222 4669 656c 6473 2061 7661 696c 6162  ""Fields availab
+000115b0: 6c65 2066 6f72 2071 7565 7279 2069 6e0a  le for query in.
+000115c0: 2020 2020 6060 636f 6d70 6574 6974 6976      ``competitiv
+000115d0: 655f 7669 7369 6269 6c69 7479 5f63 6f6d  e_visibility_com
+000115e0: 7065 7469 746f 725f 7669 6577 6060 2074  petitor_view`` t
+000115f0: 6162 6c65 2e0a 0a20 2020 2060 436f 6d70  able...    `Comp
+00011600: 6574 6974 6976 650a 2020 2020 7669 7369  etitive.    visi
+00011610: 6269 6c69 7479 203c 6874 7470 733a 2f2f  bility <https://
+00011620: 7375 7070 6f72 742e 676f 6f67 6c65 2e63  support.google.c
+00011630: 6f6d 2f6d 6572 6368 616e 7473 2f61 6e73  om/merchants/ans
+00011640: 7765 722f 3131 3336 3634 3432 3e60 5f5f  wer/11366442>`__
+00011650: 0a20 2020 2072 6570 6f72 7420 7769 7468  .    report with
+00011660: 2062 7573 696e 6573 7365 7320 7769 7468   businesses with
+00011670: 2073 696d 696c 6172 2076 6973 6962 696c   similar visibil
+00011680: 6974 792e 0a0a 2020 2020 5661 6c75 6573  ity...    Values
+00011690: 2061 7265 206f 6e6c 7920 7365 7420 666f   are only set fo
+000116a0: 7220 6669 656c 6473 2072 6571 7565 7374  r fields request
+000116b0: 6564 2065 7870 6c69 6369 746c 7920 696e  ed explicitly in
+000116c0: 2074 6865 2072 6571 7565 7374 2773 0a20   the request's. 
+000116d0: 2020 2073 6561 7263 6820 7175 6572 792e     search query.
+000116e0: 0a0a 0a20 2020 202e 2e20 5f6f 6e65 6f66  ...    .. _oneof
+000116f0: 3a20 6874 7470 733a 2f2f 7072 6f74 6f2d  : https://proto-
+00011700: 706c 7573 2d70 7974 686f 6e2e 7265 6164  plus-python.read
+00011710: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
+00011720: 6162 6c65 2f66 6965 6c64 732e 6874 6d6c  able/fields.html
+00011730: 236f 6e65 6f66 732d 6d75 7475 616c 6c79  #oneofs-mutually
+00011740: 2d65 7863 6c75 7369 7665 2d66 6965 6c64  -exclusive-field
+00011750: 730a 0a20 2020 2041 7474 7269 6275 7465  s..    Attribute
+00011760: 733a 0a20 2020 2020 2020 2064 6174 6520  s:.        date 
+00011770: 2867 6f6f 676c 652e 7479 7065 2e64 6174  (google.type.dat
+00011780: 655f 7062 322e 4461 7465 293a 0a20 2020  e_pb2.Date):.   
+00011790: 2020 2020 2020 2020 2044 6174 6520 6f66           Date of
+000117a0: 2074 6869 7320 726f 772e 0a0a 2020 2020   this row...    
+000117b0: 2020 2020 2020 2020 4120 636f 6e64 6974          A condit
+000117c0: 696f 6e20 6f6e 2060 6064 6174 6560 6020  ion on ``date`` 
+000117d0: 6973 2072 6571 7569 7265 6420 696e 2074  is required in t
+000117e0: 6865 2060 6057 4845 5245 6060 2063 6c61  he ``WHERE`` cla
+000117f0: 7573 652e 0a20 2020 2020 2020 2064 6f6d  use..        dom
+00011800: 6169 6e20 2873 7472 293a 0a20 2020 2020  ain (str):.     
+00011810: 2020 2020 2020 2044 6f6d 6169 6e20 6f66         Domain of
+00011820: 2079 6f75 7220 636f 6d70 6574 6974 6f72   your competitor
+00011830: 206f 7220 796f 7572 2064 6f6d 6169 6e2c   or your domain,
+00011840: 2069 660a 2020 2020 2020 2020 2020 2020   if.            
+00011850: 2769 735f 796f 7572 5f64 6f6d 6169 6e27  'is_your_domain'
+00011860: 2069 7320 7472 7565 2e0a 0a20 2020 2020   is true...     
+00011870: 2020 2020 2020 2052 6571 7569 7265 6420         Required 
+00011880: 696e 2074 6865 2060 6053 454c 4543 5460  in the ``SELECT`
+00011890: 6020 636c 6175 7365 2e20 4361 6e6e 6f74  ` clause. Cannot
+000118a0: 2062 6520 6669 6c74 6572 6564 206f 6e20   be filtered on 
+000118b0: 696e 0a20 2020 2020 2020 2020 2020 2074  in.            t
+000118c0: 6865 2027 5748 4552 4527 2063 6c61 7573  he 'WHERE' claus
+000118d0: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
+000118e0: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+000118f0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+00011900: 605f 2060 605f 646f 6d61 696e 6060 2e0a  `_ ``_domain``..
+00011910: 2020 2020 2020 2020 6973 5f79 6f75 725f          is_your_
+00011920: 646f 6d61 696e 2028 626f 6f6c 293a 0a20  domain (bool):. 
+00011930: 2020 2020 2020 2020 2020 2054 7275 6520             True 
+00011940: 6966 2074 6869 7320 726f 7720 636f 6e74  if this row cont
+00011950: 6169 6e73 2064 6174 6120 666f 7220 796f  ains data for yo
+00011960: 7572 0a20 2020 2020 2020 2020 2020 2064  ur.            d
+00011970: 6f6d 6169 6e2e 0a20 2020 2020 2020 2020  omain..         
+00011980: 2020 2043 616e 6e6f 7420 6265 2066 696c     Cannot be fil
+00011990: 7465 7265 6420 6f6e 2069 6e20 7468 6520  tered on in the 
+000119a0: 2757 4845 5245 2720 636c 6175 7365 2e0a  'WHERE' clause..
+000119b0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+000119c0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+000119d0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+000119e0: 6060 5f69 735f 796f 7572 5f64 6f6d 6169  ``_is_your_domai
+000119f0: 6e60 602e 0a20 2020 2020 2020 2072 6570  n``..        rep
+00011a00: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
+00011a10: 2028 7374 7229 3a0a 2020 2020 2020 2020   (str):.        
+00011a20: 2020 2020 436f 756e 7472 7920 7768 6572      Country wher
+00011a30: 6520 696d 7072 6573 7369 6f6e 7320 6170  e impressions ap
+00011a40: 7065 6172 6564 2e0a 0a20 2020 2020 2020  peared...       
+00011a50: 2020 2020 2052 6571 7569 7265 6420 696e       Required in
+00011a60: 2074 6865 2060 6053 454c 4543 5460 6020   the ``SELECT`` 
+00011a70: 636c 6175 7365 2e20 4120 636f 6e64 6974  clause. A condit
+00011a80: 696f 6e20 6f6e 0a20 2020 2020 2020 2020  ion on.         
+00011a90: 2020 2060 6072 6570 6f72 745f 636f 756e     ``report_coun
+00011aa0: 7472 795f 636f 6465 6060 2069 7320 7265  try_code`` is re
+00011ab0: 7175 6972 6564 2069 6e20 7468 6520 6060  quired in the ``
+00011ac0: 5748 4552 4560 6020 636c 6175 7365 2e0a  WHERE`` clause..
+00011ad0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00011ae0: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+00011af0: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+00011b00: 6060 5f72 6570 6f72 745f 636f 756e 7472  ``_report_countr
+00011b10: 795f 636f 6465 6060 2e0a 2020 2020 2020  y_code``..      
+00011b20: 2020 7265 706f 7274 5f63 6174 6567 6f72    report_categor
+00011b30: 795f 6964 2028 696e 7429 3a0a 2020 2020  y_id (int):.    
+00011b40: 2020 2020 2020 2020 476f 6f67 6c65 2070          Google p
+00011b50: 726f 6475 6374 2063 6174 6567 6f72 7920  roduct category 
+00011b60: 4944 2074 6f20 6361 6c63 756c 6174 6520  ID to calculate 
+00011b70: 7468 6520 7265 706f 7274 2066 6f72 2c0a  the report for,.
+00011b80: 2020 2020 2020 2020 2020 2020 7265 7072              repr
+00011b90: 6573 656e 7465 6420 696e 2060 476f 6f67  esented in `Goog
+00011ba0: 6c65 2773 2070 726f 6475 6374 0a20 2020  le's product.   
+00011bb0: 2020 2020 2020 2020 2074 6178 6f6e 6f6d           taxonom
+00011bc0: 7920 3c68 7474 7073 3a2f 2f73 7570 706f  y <https://suppo
+00011bd0: 7274 2e67 6f6f 676c 652e 636f 6d2f 6d65  rt.google.com/me
+00011be0: 7263 6861 6e74 732f 616e 7377 6572 2f36  rchants/answer/6
+00011bf0: 3332 3434 3336 3e60 5f5f 2e0a 0a20 2020  324436>`__...   
+00011c00: 2020 2020 2020 2020 2052 6571 7569 7265           Require
+00011c10: 6420 696e 2074 6865 2060 6053 454c 4543  d in the ``SELEC
+00011c20: 5460 6020 636c 6175 7365 2e20 4120 636f  T`` clause. A co
+00011c30: 6e64 6974 696f 6e20 6f6e 0a20 2020 2020  ndition on.     
+00011c40: 2020 2020 2020 2060 6072 6570 6f72 745f         ``report_
+00011c50: 6361 7465 676f 7279 5f69 6460 6020 6973  category_id`` is
+00011c60: 2072 6571 7569 7265 6420 696e 2074 6865   required in the
+00011c70: 2060 6057 4845 5245 6060 2063 6c61 7573   ``WHERE`` claus
+00011c80: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
+00011c90: 5468 6973 2066 6965 6c64 2069 7320 6120  This field is a 
+00011ca0: 6d65 6d62 6572 206f 6620 606f 6e65 6f66  member of `oneof
+00011cb0: 605f 2060 605f 7265 706f 7274 5f63 6174  `_ ``_report_cat
+00011cc0: 6567 6f72 795f 6964 6060 2e0a 2020 2020  egory_id``..    
+00011cd0: 2020 2020 7472 6166 6669 635f 736f 7572      traffic_sour
+00011ce0: 6365 2028 676f 6f67 6c65 2e73 686f 7070  ce (google.shopp
+00011cf0: 696e 672e 6d65 7263 6861 6e74 5f72 6570  ing.merchant_rep
+00011d00: 6f72 7473 5f76 3162 6574 612e 7479 7065  orts_v1beta.type
+00011d10: 732e 5472 6166 6669 6353 6f75 7263 652e  s.TrafficSource.
+00011d20: 5472 6166 6669 6353 6f75 7263 6545 6e75  TrafficSourceEnu
+00011d30: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
+00011d40: 5472 6166 6669 6320 736f 7572 6365 206f  Traffic source o
+00011d50: 6620 696d 7072 6573 7369 6f6e 732e 0a0a  f impressions...
+00011d60: 2020 2020 2020 2020 2020 2020 5265 7175              Requ
+00011d70: 6972 6564 2069 6e20 7468 6520 6060 5345  ired in the ``SE
+00011d80: 4c45 4354 6060 2063 6c61 7573 652e 0a0a  LECT`` clause...
+00011d90: 2020 2020 2020 2020 2020 2020 5468 6973              This
+00011da0: 2066 6965 6c64 2069 7320 6120 6d65 6d62   field is a memb
+00011db0: 6572 206f 6620 606f 6e65 6f66 605f 2060  er of `oneof`_ `
+00011dc0: 605f 7472 6166 6669 635f 736f 7572 6365  `_traffic_source
+00011dd0: 6060 2e0a 2020 2020 2020 2020 7261 6e6b  ``..        rank
+00011de0: 2028 696e 7429 3a0a 2020 2020 2020 2020   (int):.        
+00011df0: 2020 2020 506f 7369 7469 6f6e 206f 6620      Position of 
+00011e00: 7468 6520 646f 6d61 696e 2069 6e20 7468  the domain in th
+00011e10: 6520 7369 6d69 6c61 7220 6275 7369 6e65  e similar busine
+00011e20: 7373 6573 2072 616e 6b69 6e67 2066 6f72  sses ranking for
+00011e30: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+00011e40: 2073 656c 6563 7465 6420 6b65 7973 2028   selected keys (
+00011e50: 6060 6461 7465 6060 2c20 6060 7265 706f  ``date``, ``repo
+00011e60: 7274 5f63 6174 6567 6f72 795f 6964 6060  rt_category_id``
+00011e70: 2c0a 2020 2020 2020 2020 2020 2020 6060  ,.            ``
+00011e80: 7265 706f 7274 5f63 6f75 6e74 7279 5f63  report_country_c
+00011e90: 6f64 6560 602c 2060 6074 7261 6666 6963  ode``, ``traffic
+00011ea0: 5f73 6f75 7263 6560 6029 2062 6173 6564  _source``) based
+00011eb0: 206f 6e0a 2020 2020 2020 2020 2020 2020   on.            
+00011ec0: 696d 7072 6573 7369 6f6e 732e 2031 2069  impressions. 1 i
+00011ed0: 7320 7468 6520 6869 6768 6573 742e 0a0a  s the highest...
+00011ee0: 2020 2020 2020 2020 2020 2020 4361 6e6e              Cann
+00011ef0: 6f74 2062 6520 6669 6c74 6572 6564 206f  ot be filtered o
+00011f00: 6e20 696e 2074 6865 2027 5748 4552 4527  n in the 'WHERE'
+00011f10: 2063 6c61 7573 652e 0a0a 2020 2020 2020   clause...      
+00011f20: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+00011f30: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+00011f40: 606f 6e65 6f66 605f 2060 605f 7261 6e6b  `oneof`_ ``_rank
+00011f50: 6060 2e0a 2020 2020 2020 2020 6164 735f  ``..        ads_
+00011f60: 6f72 6761 6e69 635f 7261 7469 6f20 2866  organic_ratio (f
+00011f70: 6c6f 6174 293a 0a20 2020 2020 2020 2020  loat):.         
+00011f80: 2020 205b 4164 7320 2f20 6f72 6761 6e69     [Ads / organi
+00011f90: 6320 7261 7469 6f5d 0a20 2020 2020 2020  c ratio].       
+00011fa0: 2020 2020 2028 6874 7470 733a 2f2f 7375       (https://su
+00011fb0: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
+00011fc0: 2f6d 6572 6368 616e 7473 2f61 6e73 7765  /merchants/answe
+00011fd0: 722f 3131 3336 3634 3432 237a 6970 7079  r/11366442#zippy
+00011fe0: 3d25 3243 6164 732d 6672 6565 2d72 6174  =%2Cads-free-rat
+00011ff0: 696f 290a 2020 2020 2020 2020 2020 2020  io).            
+00012000: 7368 6f77 7320 686f 7720 6f66 7465 6e20  shows how often 
+00012010: 7468 6520 646f 6d61 696e 2072 6563 6569  the domain recei
+00012020: 7665 7320 696d 7072 6573 7369 6f6e 7320  ves impressions 
+00012030: 6672 6f6d 0a20 2020 2020 2020 2020 2020  from.           
+00012040: 2053 686f 7070 696e 6720 6164 7320 636f   Shopping ads co
+00012050: 6d70 6172 6564 2074 6f20 6f72 6761 6e69  mpared to organi
+00012060: 6320 7472 6166 6669 632e 2054 6865 206e  c traffic. The n
+00012070: 756d 6265 7220 6973 0a20 2020 2020 2020  umber is.       
+00012080: 2020 2020 2072 6f75 6e64 6564 2061 6e64       rounded and
+00012090: 2062 7563 6b65 7465 642e 0a0a 2020 2020   bucketed...    
+000120a0: 2020 2020 2020 2020 4361 6e6e 6f74 2062          Cannot b
+000120b0: 6520 6669 6c74 6572 6564 206f 6e20 696e  e filtered on in
+000120c0: 2074 6865 2027 5748 4552 4527 2063 6c61   the 'WHERE' cla
+000120d0: 7573 652e 0a0a 2020 2020 2020 2020 2020  use...          
+000120e0: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+000120f0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00012100: 6f66 605f 2060 605f 6164 735f 6f72 6761  of`_ ``_ads_orga
+00012110: 6e69 635f 7261 7469 6f60 602e 0a20 2020  nic_ratio``..   
+00012120: 2020 2020 2070 6167 655f 6f76 6572 6c61       page_overla
+00012130: 705f 7261 7465 2028 666c 6f61 7429 3a0a  p_rate (float):.
+00012140: 2020 2020 2020 2020 2020 2020 5b50 6167              [Pag
+00012150: 6520 6f76 6572 6c61 7020 7261 7465 5d0a  e overlap rate].
+00012160: 2020 2020 2020 2020 2020 2020 2868 7474              (htt
+00012170: 7073 3a2f 2f73 7570 706f 7274 2e67 6f6f  ps://support.goo
+00012180: 676c 652e 636f 6d2f 6d65 7263 6861 6e74  gle.com/merchant
+00012190: 732f 616e 7377 6572 2f31 3133 3636 3434  s/answer/1136644
+000121a0: 3223 7a69 7070 793d 2532 4370 6167 652d  2#zippy=%2Cpage-
+000121b0: 6f76 6572 6c61 702d 7261 7465 290a 2020  overlap-rate).  
+000121c0: 2020 2020 2020 2020 2020 7368 6f77 7320            shows 
+000121d0: 686f 7720 6672 6571 7565 6e74 6c79 2063  how frequently c
+000121e0: 6f6d 7065 7469 6e67 2072 6574 6169 6c65  ompeting retaile
+000121f0: 7273 e280 9920 6f66 6665 7273 2061 7265  rs... offers are
+00012200: 2073 686f 776e 0a20 2020 2020 2020 2020   shown.         
+00012210: 2020 2074 6f67 6574 6865 7220 7769 7468     together with
+00012220: 2079 6f75 7220 6f66 6665 7273 206f 6e20   your offers on 
+00012230: 7468 6520 7361 6d65 2070 6167 652e 0a0a  the same page...
+00012240: 2020 2020 2020 2020 2020 2020 4361 6e6e              Cann
+00012250: 6f74 2062 6520 6669 6c74 6572 6564 206f  ot be filtered o
+00012260: 6e20 696e 2074 6865 2027 5748 4552 4527  n in the 'WHERE'
+00012270: 2063 6c61 7573 652e 0a0a 2020 2020 2020   clause...      
+00012280: 2020 2020 2020 5468 6973 2066 6965 6c64        This field
+00012290: 2069 7320 6120 6d65 6d62 6572 206f 6620   is a member of 
+000122a0: 606f 6e65 6f66 605f 2060 605f 7061 6765  `oneof`_ ``_page
+000122b0: 5f6f 7665 726c 6170 5f72 6174 6560 602e  _overlap_rate``.
+000122c0: 0a20 2020 2020 2020 2068 6967 6865 725f  .        higher_
+000122d0: 706f 7369 7469 6f6e 5f72 6174 6520 2866  position_rate (f
+000122e0: 6c6f 6174 293a 0a20 2020 2020 2020 2020  loat):.         
+000122f0: 2020 205b 4869 6768 6572 2070 6f73 6974     [Higher posit
+00012300: 696f 6e20 7261 7465 5d0a 2020 2020 2020  ion rate].      
+00012310: 2020 2020 2020 2868 7474 7073 3a2f 2f73        (https://s
+00012320: 7570 706f 7274 2e67 6f6f 676c 652e 636f  upport.google.co
+00012330: 6d2f 6d65 7263 6861 6e74 732f 616e 7377  m/merchants/answ
+00012340: 6572 2f31 3133 3636 3434 3223 7a69 7070  er/11366442#zipp
+00012350: 793d 2532 4368 6967 6865 722d 706f 7369  y=%2Chigher-posi
+00012360: 7469 6f6e 2d72 6174 6529 0a20 2020 2020  tion-rate).     
+00012370: 2020 2020 2020 2073 686f 7773 2068 6f77         shows how
+00012380: 206f 6674 656e 2061 2063 6f6d 7065 7469   often a competi
+00012390: 746f 72e2 8099 7320 6f66 6665 7220 676f  tor...s offer go
+000123a0: 7420 706c 6163 6564 2069 6e20 6120 6869  t placed in a hi
+000123b0: 6768 6572 0a20 2020 2020 2020 2020 2020  gher.           
+000123c0: 2070 6f73 6974 696f 6e20 6f6e 2074 6865   position on the
+000123d0: 2070 6167 6520 7468 616e 2079 6f75 7220   page than your 
+000123e0: 6f66 6665 722e 0a0a 2020 2020 2020 2020  offer...        
+000123f0: 2020 2020 4361 6e6e 6f74 2062 6520 6669      Cannot be fi
+00012400: 6c74 6572 6564 206f 6e20 696e 2074 6865  ltered on in the
+00012410: 2027 5748 4552 4527 2063 6c61 7573 652e   'WHERE' clause.
+00012420: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00012430: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+00012440: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+00012450: 2060 605f 6869 6768 6572 5f70 6f73 6974   ``_higher_posit
+00012460: 696f 6e5f 7261 7465 6060 2e0a 2020 2020  ion_rate``..    
+00012470: 2020 2020 7265 6c61 7469 7665 5f76 6973      relative_vis
+00012480: 6962 696c 6974 7920 2866 6c6f 6174 293a  ibility (float):
+00012490: 0a20 2020 2020 2020 2020 2020 205b 5265  .            [Re
+000124a0: 6c61 7469 7665 2076 6973 6962 696c 6974  lative visibilit
+000124b0: 795d 0a20 2020 2020 2020 2020 2020 2028  y].            (
+000124c0: 6874 7470 733a 2f2f 7375 7070 6f72 742e  https://support.
+000124d0: 676f 6f67 6c65 2e63 6f6d 2f6d 6572 6368  google.com/merch
+000124e0: 616e 7473 2f61 6e73 7765 722f 3131 3336  ants/answer/1136
+000124f0: 3634 3432 237a 6970 7079 3d25 3243 7265  6442#zippy=%2Cre
+00012500: 6c61 7469 7665 2d76 6973 6962 696c 6974  lative-visibilit
+00012510: 7929 0a20 2020 2020 2020 2020 2020 2073  y).            s
+00012520: 686f 7773 2068 6f77 206f 6674 656e 2079  hows how often y
+00012530: 6f75 7220 636f 6d70 6574 6974 6f72 73e2  our competitors.
+00012540: 8099 206f 6666 6572 7320 6172 6520 7368  .. offers are sh
+00012550: 6f77 6e20 636f 6d70 6172 6564 0a20 2020  own compared.   
+00012560: 2020 2020 2020 2020 2074 6f20 796f 7572           to your
+00012570: 206f 6666 6572 732e 2049 6e20 6f74 6865   offers. In othe
+00012580: 7220 776f 7264 732c 2074 6869 7320 6973  r words, this is
+00012590: 2074 6865 206e 756d 6265 7220 6f66 0a20   the number of. 
+000125a0: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+000125b0: 6179 6564 2069 6d70 7265 7373 696f 6e73  ayed impressions
+000125c0: 206f 6620 6120 636f 6d70 6574 6974 6f72   of a competitor
+000125d0: 2072 6574 6169 6c65 7220 6469 7669 6465   retailer divide
+000125e0: 6420 6279 0a20 2020 2020 2020 2020 2020  d by.           
+000125f0: 2074 6865 206e 756d 6265 7220 6f66 2079   the number of y
+00012600: 6f75 7220 6469 7370 6c61 7965 6420 696d  our displayed im
+00012610: 7072 6573 7369 6f6e 7320 6475 7269 6e67  pressions during
+00012620: 2061 2073 656c 6563 7465 640a 2020 2020   a selected.    
+00012630: 2020 2020 2020 2020 7469 6d65 2072 616e          time ran
+00012640: 6765 2066 6f72 2061 2073 656c 6563 7465  ge for a selecte
+00012650: 6420 7072 6f64 7563 7420 6361 7465 676f  d product catego
+00012660: 7279 2061 6e64 2063 6f75 6e74 7279 2e0a  ry and country..
+00012670: 0a20 2020 2020 2020 2020 2020 2043 616e  .            Can
+00012680: 6e6f 7420 6265 2066 696c 7465 7265 6420  not be filtered 
+00012690: 6f6e 2069 6e20 7468 6520 2757 4845 5245  on in the 'WHERE
+000126a0: 2720 636c 6175 7365 2e0a 0a20 2020 2020  ' clause...     
+000126b0: 2020 2020 2020 2054 6869 7320 6669 656c         This fiel
+000126c0: 6420 6973 2061 206d 656d 6265 7220 6f66  d is a member of
+000126d0: 2060 6f6e 656f 6660 5f20 6060 5f72 656c   `oneof`_ ``_rel
+000126e0: 6174 6976 655f 7669 7369 6269 6c69 7479  ative_visibility
+000126f0: 6060 2e0a 2020 2020 2222 220a 0a20 2020  ``..    """..   
+00012700: 2064 6174 653a 2064 6174 655f 7062 322e   date: date_pb2.
+00012710: 4461 7465 203d 2070 726f 746f 2e46 6965  Date = proto.Fie
+00012720: 6c64 280a 2020 2020 2020 2020 7072 6f74  ld(.        prot
+00012730: 6f2e 4d45 5353 4147 452c 0a20 2020 2020  o.MESSAGE,.     
+00012740: 2020 206e 756d 6265 723d 312c 0a20 2020     number=1,.   
+00012750: 2020 2020 206d 6573 7361 6765 3d64 6174       message=dat
+00012760: 655f 7062 322e 4461 7465 2c0a 2020 2020  e_pb2.Date,.    
+00012770: 290a 2020 2020 646f 6d61 696e 3a20 7374  ).    domain: st
+00012780: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00012790: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+000127a0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+000127b0: 756d 6265 723d 322c 0a20 2020 2020 2020  umber=2,.       
+000127c0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+000127d0: 2020 2020 290a 2020 2020 6973 5f79 6f75      ).    is_you
+000127e0: 725f 646f 6d61 696e 3a20 626f 6f6c 203d  r_domain: bool =
+000127f0: 2070 726f 746f 2e46 6965 6c64 280a 2020   proto.Field(.  
+00012800: 2020 2020 2020 7072 6f74 6f2e 424f 4f4c        proto.BOOL
+00012810: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00012820: 3d33 2c0a 2020 2020 2020 2020 6f70 7469  =3,.        opti
+00012830: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+00012840: 0a20 2020 2072 6570 6f72 745f 636f 756e  .    report_coun
+00012850: 7472 795f 636f 6465 3a20 7374 7220 3d20  try_code: str = 
+00012860: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+00012870: 2020 2020 2070 726f 746f 2e53 5452 494e       proto.STRIN
+00012880: 472c 0a20 2020 2020 2020 206e 756d 6265  G,.        numbe
+00012890: 723d 342c 0a20 2020 2020 2020 206f 7074  r=4,.        opt
+000128a0: 696f 6e61 6c3d 5472 7565 2c0a 2020 2020  ional=True,.    
+000128b0: 290a 2020 2020 7265 706f 7274 5f63 6174  ).    report_cat
+000128c0: 6567 6f72 795f 6964 3a20 696e 7420 3d20  egory_id: int = 
+000128d0: 7072 6f74 6f2e 4669 656c 6428 0a20 2020  proto.Field(.   
+000128e0: 2020 2020 2070 726f 746f 2e49 4e54 3634       proto.INT64
+000128f0: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00012900: 3d35 2c0a 2020 2020 2020 2020 6f70 7469  =5,.        opti
+00012910: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+00012920: 0a20 2020 2074 7261 6666 6963 5f73 6f75  .    traffic_sou
+00012930: 7263 653a 2022 5472 6166 6669 6353 6f75  rce: "TrafficSou
+00012940: 7263 652e 5472 6166 6669 6353 6f75 7263  rce.TrafficSourc
+00012950: 6545 6e75 6d22 203d 2070 726f 746f 2e46  eEnum" = proto.F
+00012960: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00012970: 6f74 6f2e 454e 554d 2c0a 2020 2020 2020  oto.ENUM,.      
+00012980: 2020 6e75 6d62 6572 3d36 2c0a 2020 2020    number=6,.    
+00012990: 2020 2020 6f70 7469 6f6e 616c 3d54 7275      optional=Tru
+000129a0: 652c 0a20 2020 2020 2020 2065 6e75 6d3d  e,.        enum=
+000129b0: 2254 7261 6666 6963 536f 7572 6365 2e54  "TrafficSource.T
+000129c0: 7261 6666 6963 536f 7572 6365 456e 756d  rafficSourceEnum
+000129d0: 222c 0a20 2020 2029 0a20 2020 2072 616e  ",.    ).    ran
+000129e0: 6b3a 2069 6e74 203d 2070 726f 746f 2e46  k: int = proto.F
+000129f0: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00012a00: 6f74 6f2e 494e 5436 342c 0a20 2020 2020  oto.INT64,.     
+00012a10: 2020 206e 756d 6265 723d 372c 0a20 2020     number=7,.   
+00012a20: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+00012a30: 7565 2c0a 2020 2020 290a 2020 2020 6164  ue,.    ).    ad
+00012a40: 735f 6f72 6761 6e69 635f 7261 7469 6f3a  s_organic_ratio:
+00012a50: 2066 6c6f 6174 203d 2070 726f 746f 2e46   float = proto.F
+00012a60: 6965 6c64 280a 2020 2020 2020 2020 7072  ield(.        pr
+00012a70: 6f74 6f2e 444f 5542 4c45 2c0a 2020 2020  oto.DOUBLE,.    
+00012a80: 2020 2020 6e75 6d62 6572 3d38 2c0a 2020      number=8,.  
+00012a90: 2020 2020 2020 6f70 7469 6f6e 616c 3d54        optional=T
+00012aa0: 7275 652c 0a20 2020 2029 0a20 2020 2070  rue,.    ).    p
+00012ab0: 6167 655f 6f76 6572 6c61 705f 7261 7465  age_overlap_rate
+00012ac0: 3a20 666c 6f61 7420 3d20 7072 6f74 6f2e  : float = proto.
+00012ad0: 4669 656c 6428 0a20 2020 2020 2020 2070  Field(.        p
+00012ae0: 726f 746f 2e44 4f55 424c 452c 0a20 2020  roto.DOUBLE,.   
+00012af0: 2020 2020 206e 756d 6265 723d 392c 0a20       number=9,. 
+00012b00: 2020 2020 2020 206f 7074 696f 6e61 6c3d         optional=
+00012b10: 5472 7565 2c0a 2020 2020 290a 2020 2020  True,.    ).    
+00012b20: 6869 6768 6572 5f70 6f73 6974 696f 6e5f  higher_position_
+00012b30: 7261 7465 3a20 666c 6f61 7420 3d20 7072  rate: float = pr
+00012b40: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+00012b50: 2020 2070 726f 746f 2e44 4f55 424c 452c     proto.DOUBLE,
+00012b60: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+00012b70: 3130 2c0a 2020 2020 2020 2020 6f70 7469  10,.        opti
+00012b80: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+00012b90: 0a20 2020 2072 656c 6174 6976 655f 7669  .    relative_vi
+00012ba0: 7369 6269 6c69 7479 3a20 666c 6f61 7420  sibility: float 
+00012bb0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00012bc0: 2020 2020 2020 2070 726f 746f 2e44 4f55         proto.DOU
+00012bd0: 424c 452c 0a20 2020 2020 2020 206e 756d  BLE,.        num
+00012be0: 6265 723d 3131 2c0a 2020 2020 2020 2020  ber=11,.        
+00012bf0: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00012c00: 2020 2029 0a0a 0a63 6c61 7373 2043 6f6d     )...class Com
+00012c10: 7065 7469 7469 7665 5669 7369 6269 6c69  petitiveVisibili
+00012c20: 7479 546f 704d 6572 6368 616e 7456 6965  tyTopMerchantVie
+00012c30: 7728 7072 6f74 6f2e 4d65 7373 6167 6529  w(proto.Message)
+00012c40: 3a0a 2020 2020 7222 2222 4669 656c 6473  :.    r"""Fields
+00012c50: 2061 7661 696c 6162 6c65 2066 6f72 2071   available for q
+00012c60: 7565 7279 2069 6e0a 2020 2020 6060 636f  uery in.    ``co
+00012c70: 6d70 6574 6974 6976 655f 7669 7369 6269  mpetitive_visibi
+00012c80: 6c69 7479 5f74 6f70 5f6d 6572 6368 616e  lity_top_merchan
+00012c90: 745f 7669 6577 6060 2074 6162 6c65 2e0a  t_view`` table..
+00012ca0: 0a20 2020 2060 436f 6d70 6574 6974 6976  .    `Competitiv
+00012cb0: 650a 2020 2020 7669 7369 6269 6c69 7479  e.    visibility
+00012cc0: 203c 6874 7470 733a 2f2f 7375 7070 6f72   <https://suppor
+00012cd0: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
+00012ce0: 6368 616e 7473 2f61 6e73 7765 722f 3131  chants/answer/11
+00012cf0: 3336 3634 3432 3e60 5f5f 0a20 2020 2072  366442>`__.    r
+00012d00: 6570 6f72 7420 7769 7468 2062 7573 696e  eport with busin
+00012d10: 6573 7320 7769 7468 2068 6967 6865 7374  ess with highest
+00012d20: 2076 6973 6962 696c 6974 792e 0a0a 2020   visibility...  
+00012d30: 2020 5661 6c75 6573 2061 7265 206f 6e6c    Values are onl
+00012d40: 7920 7365 7420 666f 7220 6669 656c 6473  y set for fields
+00012d50: 2072 6571 7565 7374 6564 2065 7870 6c69   requested expli
+00012d60: 6369 746c 7920 696e 2074 6865 2072 6571  citly in the req
+00012d70: 7565 7374 2773 0a20 2020 2073 6561 7263  uest's.    searc
+00012d80: 6820 7175 6572 792e 0a0a 0a20 2020 202e  h query....    .
+00012d90: 2e20 5f6f 6e65 6f66 3a20 6874 7470 733a  . _oneof: https:
+00012da0: 2f2f 7072 6f74 6f2d 706c 7573 2d70 7974  //proto-plus-pyt
+00012db0: 686f 6e2e 7265 6164 7468 6564 6f63 732e  hon.readthedocs.
+00012dc0: 696f 2f65 6e2f 7374 6162 6c65 2f66 6965  io/en/stable/fie
+00012dd0: 6c64 732e 6874 6d6c 236f 6e65 6f66 732d  lds.html#oneofs-
+00012de0: 6d75 7475 616c 6c79 2d65 7863 6c75 7369  mutually-exclusi
+00012df0: 7665 2d66 6965 6c64 730a 0a20 2020 2041  ve-fields..    A
+00012e00: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
+00012e10: 2020 2064 6174 6520 2867 6f6f 676c 652e     date (google.
+00012e20: 7479 7065 2e64 6174 655f 7062 322e 4461  type.date_pb2.Da
+00012e30: 7465 293a 0a20 2020 2020 2020 2020 2020  te):.           
+00012e40: 2044 6174 6520 6f66 2074 6869 7320 726f   Date of this ro
+00012e50: 772e 0a0a 2020 2020 2020 2020 2020 2020  w...            
+00012e60: 4361 6e6e 6f74 2062 6520 7365 6c65 6374  Cannot be select
+00012e70: 6564 2069 6e20 7468 6520 6060 5345 4c45  ed in the ``SELE
+00012e80: 4354 6060 2063 6c61 7573 652e 2041 2063  CT`` clause. A c
+00012e90: 6f6e 6469 7469 6f6e 206f 6e0a 2020 2020  ondition on.    
+00012ea0: 2020 2020 2020 2020 6060 6461 7465 6060          ``date``
+00012eb0: 2069 7320 7265 7175 6972 6564 2069 6e20   is required in 
+00012ec0: 7468 6520 6060 5748 4552 4560 6020 636c  the ``WHERE`` cl
+00012ed0: 6175 7365 2e0a 2020 2020 2020 2020 646f  ause..        do
+00012ee0: 6d61 696e 2028 7374 7229 3a0a 2020 2020  main (str):.    
+00012ef0: 2020 2020 2020 2020 446f 6d61 696e 206f          Domain o
+00012f00: 6620 796f 7572 2063 6f6d 7065 7469 746f  f your competito
+00012f10: 7220 6f72 2079 6f75 7220 646f 6d61 696e  r or your domain
+00012f20: 2c20 6966 0a20 2020 2020 2020 2020 2020  , if.           
+00012f30: 2027 6973 5f79 6f75 725f 646f 6d61 696e   'is_your_domain
+00012f40: 2720 6973 2074 7275 652e 0a0a 2020 2020  ' is true...    
+00012f50: 2020 2020 2020 2020 5265 7175 6972 6564          Required
+00012f60: 2069 6e20 7468 6520 6060 5345 4c45 4354   in the ``SELECT
+00012f70: 6060 2063 6c61 7573 652e 2043 616e 6e6f  `` clause. Canno
+00012f80: 7420 6265 2066 696c 7465 7265 6420 6f6e  t be filtered on
+00012f90: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
+00012fa0: 7468 6520 2757 4845 5245 2720 636c 6175  the 'WHERE' clau
+00012fb0: 7365 2e0a 0a20 2020 2020 2020 2020 2020  se...           
+00012fc0: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+00012fd0: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+00012fe0: 6660 5f20 6060 5f64 6f6d 6169 6e60 602e  f`_ ``_domain``.
+00012ff0: 0a20 2020 2020 2020 2069 735f 796f 7572  .        is_your
+00013000: 5f64 6f6d 6169 6e20 2862 6f6f 6c29 3a0a  _domain (bool):.
+00013010: 2020 2020 2020 2020 2020 2020 5472 7565              True
+00013020: 2069 6620 7468 6973 2072 6f77 2063 6f6e   if this row con
+00013030: 7461 696e 7320 6461 7461 2066 6f72 2079  tains data for y
+00013040: 6f75 720a 2020 2020 2020 2020 2020 2020  our.            
+00013050: 646f 6d61 696e 2e0a 2020 2020 2020 2020  domain..        
+00013060: 2020 2020 4361 6e6e 6f74 2062 6520 6669      Cannot be fi
+00013070: 6c74 6572 6564 206f 6e20 696e 2074 6865  ltered on in the
+00013080: 2027 5748 4552 4527 2063 6c61 7573 652e   'WHERE' clause.
+00013090: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+000130a0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+000130b0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+000130c0: 2060 605f 6973 5f79 6f75 725f 646f 6d61   ``_is_your_doma
+000130d0: 696e 6060 2e0a 2020 2020 2020 2020 7265  in``..        re
+000130e0: 706f 7274 5f63 6f75 6e74 7279 5f63 6f64  port_country_cod
+000130f0: 6520 2873 7472 293a 0a20 2020 2020 2020  e (str):.       
+00013100: 2020 2020 2043 6f75 6e74 7279 2077 6865       Country whe
+00013110: 7265 2069 6d70 7265 7373 696f 6e73 2061  re impressions a
+00013120: 7070 6561 7265 642e 0a0a 2020 2020 2020  ppeared...      
+00013130: 2020 2020 2020 5265 7175 6972 6564 2069        Required i
+00013140: 6e20 7468 6520 6060 5345 4c45 4354 6060  n the ``SELECT``
+00013150: 2063 6c61 7573 652e 2041 2063 6f6e 6469   clause. A condi
+00013160: 7469 6f6e 206f 6e0a 2020 2020 2020 2020  tion on.        
+00013170: 2020 2020 6060 7265 706f 7274 5f63 6f75      ``report_cou
+00013180: 6e74 7279 5f63 6f64 6560 6020 6973 2072  ntry_code`` is r
+00013190: 6571 7569 7265 6420 696e 2074 6865 2060  equired in the `
+000131a0: 6057 4845 5245 6060 2063 6c61 7573 652e  `WHERE`` clause.
+000131b0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+000131c0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+000131d0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+000131e0: 2060 605f 7265 706f 7274 5f63 6f75 6e74   ``_report_count
+000131f0: 7279 5f63 6f64 6560 602e 0a20 2020 2020  ry_code``..     
+00013200: 2020 2072 6570 6f72 745f 6361 7465 676f     report_catego
+00013210: 7279 5f69 6420 2869 6e74 293a 0a20 2020  ry_id (int):.   
+00013220: 2020 2020 2020 2020 2047 6f6f 676c 6520           Google 
+00013230: 7072 6f64 7563 7420 6361 7465 676f 7279  product category
+00013240: 2049 4420 746f 2063 616c 6375 6c61 7465   ID to calculate
+00013250: 2074 6865 2072 6570 6f72 7420 666f 722c   the report for,
+00013260: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
+00013270: 7265 7365 6e74 6564 2069 6e20 6047 6f6f  resented in `Goo
+00013280: 676c 6527 7320 7072 6f64 7563 740a 2020  gle's product.  
+00013290: 2020 2020 2020 2020 2020 7461 786f 6e6f            taxono
+000132a0: 6d79 203c 6874 7470 733a 2f2f 7375 7070  my <https://supp
+000132b0: 6f72 742e 676f 6f67 6c65 2e63 6f6d 2f6d  ort.google.com/m
+000132c0: 6572 6368 616e 7473 2f61 6e73 7765 722f  erchants/answer/
+000132d0: 3633 3234 3433 363e 605f 5f2e 0a0a 2020  6324436>`__...  
+000132e0: 2020 2020 2020 2020 2020 5265 7175 6972            Requir
+000132f0: 6564 2069 6e20 7468 6520 6060 5345 4c45  ed in the ``SELE
+00013300: 4354 6060 2063 6c61 7573 652e 2041 2063  CT`` clause. A c
+00013310: 6f6e 6469 7469 6f6e 206f 6e0a 2020 2020  ondition on.    
+00013320: 2020 2020 2020 2020 6060 7265 706f 7274          ``report
+00013330: 5f63 6174 6567 6f72 795f 6964 6060 2069  _category_id`` i
+00013340: 7320 7265 7175 6972 6564 2069 6e20 7468  s required in th
+00013350: 6520 6060 5748 4552 4560 6020 636c 6175  e ``WHERE`` clau
+00013360: 7365 2e0a 0a20 2020 2020 2020 2020 2020  se...           
+00013370: 2054 6869 7320 6669 656c 6420 6973 2061   This field is a
+00013380: 206d 656d 6265 7220 6f66 2060 6f6e 656f   member of `oneo
+00013390: 6660 5f20 6060 5f72 6570 6f72 745f 6361  f`_ ``_report_ca
+000133a0: 7465 676f 7279 5f69 6460 602e 0a20 2020  tegory_id``..   
+000133b0: 2020 2020 2074 7261 6666 6963 5f73 6f75       traffic_sou
+000133c0: 7263 6520 2867 6f6f 676c 652e 7368 6f70  rce (google.shop
+000133d0: 7069 6e67 2e6d 6572 6368 616e 745f 7265  ping.merchant_re
+000133e0: 706f 7274 735f 7631 6265 7461 2e74 7970  ports_v1beta.typ
+000133f0: 6573 2e54 7261 6666 6963 536f 7572 6365  es.TrafficSource
+00013400: 2e54 7261 6666 6963 536f 7572 6365 456e  .TrafficSourceEn
+00013410: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
+00013420: 2054 7261 6666 6963 2073 6f75 7263 6520   Traffic source 
+00013430: 6f66 2069 6d70 7265 7373 696f 6e73 2e0a  of impressions..
+00013440: 0a20 2020 2020 2020 2020 2020 2052 6571  .            Req
+00013450: 7569 7265 6420 696e 2074 6865 2060 6053  uired in the ``S
+00013460: 454c 4543 5460 6020 636c 6175 7365 2e0a  ELECT`` clause..
+00013470: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00013480: 7320 6669 656c 6420 6973 2061 206d 656d  s field is a mem
+00013490: 6265 7220 6f66 2060 6f6e 656f 6660 5f20  ber of `oneof`_ 
+000134a0: 6060 5f74 7261 6666 6963 5f73 6f75 7263  ``_traffic_sourc
+000134b0: 6560 602e 0a20 2020 2020 2020 2072 616e  e``..        ran
+000134c0: 6b20 2869 6e74 293a 0a20 2020 2020 2020  k (int):.       
+000134d0: 2020 2020 2050 6f73 6974 696f 6e20 6f66       Position of
+000134e0: 2074 6865 2064 6f6d 6169 6e20 696e 2074   the domain in t
+000134f0: 6865 2074 6f70 206d 6572 6368 616e 7473  he top merchants
+00013500: 2072 616e 6b69 6e67 2066 6f72 2074 6865   ranking for the
+00013510: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00013520: 6563 7465 6420 6b65 7973 2028 6060 6461  ected keys (``da
+00013530: 7465 6060 2c20 6060 7265 706f 7274 5f63  te``, ``report_c
+00013540: 6174 6567 6f72 795f 6964 6060 2c0a 2020  ategory_id``,.  
+00013550: 2020 2020 2020 2020 2020 6060 7265 706f            ``repo
+00013560: 7274 5f63 6f75 6e74 7279 5f63 6f64 6560  rt_country_code`
+00013570: 602c 2060 6074 7261 6666 6963 5f73 6f75  `, ``traffic_sou
+00013580: 7263 6560 6029 2062 6173 6564 206f 6e0a  rce``) based on.
+00013590: 2020 2020 2020 2020 2020 2020 696d 7072              impr
+000135a0: 6573 7369 6f6e 732e 2031 2069 7320 7468  essions. 1 is th
+000135b0: 6520 6869 6768 6573 742e 0a0a 2020 2020  e highest...    
+000135c0: 2020 2020 2020 2020 4361 6e6e 6f74 2062          Cannot b
+000135d0: 6520 6669 6c74 6572 6564 206f 6e20 696e  e filtered on in
+000135e0: 2074 6865 2027 5748 4552 4527 2063 6c61   the 'WHERE' cla
+000135f0: 7573 652e 0a0a 2020 2020 2020 2020 2020  use...          
+00013600: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00013610: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00013620: 6f66 605f 2060 605f 7261 6e6b 6060 2e0a  of`_ ``_rank``..
+00013630: 2020 2020 2020 2020 6164 735f 6f72 6761          ads_orga
+00013640: 6e69 635f 7261 7469 6f20 2866 6c6f 6174  nic_ratio (float
+00013650: 293a 0a20 2020 2020 2020 2020 2020 205b  ):.            [
+00013660: 4164 7320 2f20 6f72 6761 6e69 6320 7261  Ads / organic ra
+00013670: 7469 6f5d 0a20 2020 2020 2020 2020 2020  tio].           
+00013680: 2028 6874 7470 733a 2f2f 7375 7070 6f72   (https://suppor
+00013690: 742e 676f 6f67 6c65 2e63 6f6d 2f6d 6572  t.google.com/mer
+000136a0: 6368 616e 7473 2f61 6e73 7765 722f 3131  chants/answer/11
+000136b0: 3336 3634 3432 237a 6970 7079 3d25 3243  366442#zippy=%2C
+000136c0: 6164 732d 6672 6565 2d72 6174 696f 290a  ads-free-ratio).
+000136d0: 2020 2020 2020 2020 2020 2020 7368 6f77              show
+000136e0: 7320 686f 7720 6f66 7465 6e20 7468 6520  s how often the 
+000136f0: 646f 6d61 696e 2072 6563 6569 7665 7320  domain receives 
+00013700: 696d 7072 6573 7369 6f6e 7320 6672 6f6d  impressions from
+00013710: 0a20 2020 2020 2020 2020 2020 2053 686f  .            Sho
+00013720: 7070 696e 6720 6164 7320 636f 6d70 6172  pping ads compar
+00013730: 6564 2074 6f20 6f72 6761 6e69 6320 7472  ed to organic tr
+00013740: 6166 6669 632e 2054 6865 206e 756d 6265  affic. The numbe
+00013750: 7220 6973 0a20 2020 2020 2020 2020 2020  r is.           
+00013760: 2072 6f75 6e64 6564 2061 6e64 2062 7563   rounded and buc
+00013770: 6b65 7465 642e 0a0a 2020 2020 2020 2020  keted...        
+00013780: 2020 2020 4361 6e6e 6f74 2062 6520 6669      Cannot be fi
+00013790: 6c74 6572 6564 206f 6e20 696e 2074 6865  ltered on in the
+000137a0: 2027 5748 4552 4527 2063 6c61 7573 652e   'WHERE' clause.
+000137b0: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+000137c0: 6973 2066 6965 6c64 2069 7320 6120 6d65  is field is a me
+000137d0: 6d62 6572 206f 6620 606f 6e65 6f66 605f  mber of `oneof`_
+000137e0: 2060 605f 6164 735f 6f72 6761 6e69 635f   ``_ads_organic_
+000137f0: 7261 7469 6f60 602e 0a20 2020 2020 2020  ratio``..       
+00013800: 2070 6167 655f 6f76 6572 6c61 705f 7261   page_overlap_ra
+00013810: 7465 2028 666c 6f61 7429 3a0a 2020 2020  te (float):.    
+00013820: 2020 2020 2020 2020 5b50 6167 6520 6f76          [Page ov
+00013830: 6572 6c61 7020 7261 7465 5d0a 2020 2020  erlap rate].    
+00013840: 2020 2020 2020 2020 2868 7474 7073 3a2f          (https:/
+00013850: 2f73 7570 706f 7274 2e67 6f6f 676c 652e  /support.google.
+00013860: 636f 6d2f 6d65 7263 6861 6e74 732f 616e  com/merchants/an
+00013870: 7377 6572 2f31 3133 3636 3434 3223 7a69  swer/11366442#zi
+00013880: 7070 793d 2532 4370 6167 652d 6f76 6572  ppy=%2Cpage-over
+00013890: 6c61 702d 7261 7465 290a 2020 2020 2020  lap-rate).      
+000138a0: 2020 2020 2020 7368 6f77 7320 686f 7720        shows how 
+000138b0: 6672 6571 7565 6e74 6c79 2063 6f6d 7065  frequently compe
+000138c0: 7469 6e67 2072 6574 6169 6c65 7273 e280  ting retailers..
+000138d0: 9920 6f66 6665 7273 2061 7265 2073 686f  . offers are sho
+000138e0: 776e 0a20 2020 2020 2020 2020 2020 2074  wn.            t
+000138f0: 6f67 6574 6865 7220 7769 7468 2079 6f75  ogether with you
+00013900: 7220 6f66 6665 7273 206f 6e20 7468 6520  r offers on the 
+00013910: 7361 6d65 2070 6167 652e 0a0a 2020 2020  same page...    
+00013920: 2020 2020 2020 2020 4361 6e6e 6f74 2062          Cannot b
+00013930: 6520 6669 6c74 6572 6564 206f 6e20 696e  e filtered on in
+00013940: 2074 6865 2027 5748 4552 4527 2063 6c61   the 'WHERE' cla
+00013950: 7573 652e 0a0a 2020 2020 2020 2020 2020  use...          
+00013960: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+00013970: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+00013980: 6f66 605f 2060 605f 7061 6765 5f6f 7665  of`_ ``_page_ove
+00013990: 726c 6170 5f72 6174 6560 602e 0a20 2020  rlap_rate``..   
+000139a0: 2020 2020 2068 6967 6865 725f 706f 7369       higher_posi
+000139b0: 7469 6f6e 5f72 6174 6520 2866 6c6f 6174  tion_rate (float
+000139c0: 293a 0a20 2020 2020 2020 2020 2020 205b  ):.            [
+000139d0: 4869 6768 6572 2070 6f73 6974 696f 6e20  Higher position 
+000139e0: 7261 7465 5d0a 2020 2020 2020 2020 2020  rate].          
+000139f0: 2020 2868 7474 7073 3a2f 2f73 7570 706f    (https://suppo
+00013a00: 7274 2e67 6f6f 676c 652e 636f 6d2f 6d65  rt.google.com/me
+00013a10: 7263 6861 6e74 732f 616e 7377 6572 2f31  rchants/answer/1
+00013a20: 3133 3636 3434 3223 7a69 7070 793d 2532  1366442#zippy=%2
+00013a30: 4368 6967 6865 722d 706f 7369 7469 6f6e  Chigher-position
+00013a40: 2d72 6174 6529 0a20 2020 2020 2020 2020  -rate).         
+00013a50: 2020 2073 686f 7773 2068 6f77 206f 6674     shows how oft
+00013a60: 656e 2061 2063 6f6d 7065 7469 746f 72e2  en a competitor.
+00013a70: 8099 7320 6f66 6665 7220 676f 7420 706c  ..s offer got pl
+00013a80: 6163 6564 2069 6e20 6120 6869 6768 6572  aced in a higher
+00013a90: 0a20 2020 2020 2020 2020 2020 2070 6f73  .            pos
+00013aa0: 6974 696f 6e20 6f6e 2074 6865 2070 6167  ition on the pag
+00013ab0: 6520 7468 616e 2079 6f75 7220 6f66 6665  e than your offe
+00013ac0: 722e 0a0a 2020 2020 2020 2020 2020 2020  r...            
+00013ad0: 4361 6e6e 6f74 2062 6520 6669 6c74 6572  Cannot be filter
+00013ae0: 6564 206f 6e20 696e 2074 6865 2027 5748  ed on in the 'WH
+00013af0: 4552 4527 2063 6c61 7573 652e 0a0a 2020  ERE' clause...  
+00013b00: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+00013b10: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+00013b20: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+00013b30: 6869 6768 6572 5f70 6f73 6974 696f 6e5f  higher_position_
+00013b40: 7261 7465 6060 2e0a 2020 2020 2222 220a  rate``..    """.
+00013b50: 0a20 2020 2064 6174 653a 2064 6174 655f  .    date: date_
+00013b60: 7062 322e 4461 7465 203d 2070 726f 746f  pb2.Date = proto
+00013b70: 2e46 6965 6c64 280a 2020 2020 2020 2020  .Field(.        
+00013b80: 7072 6f74 6f2e 4d45 5353 4147 452c 0a20  proto.MESSAGE,. 
+00013b90: 2020 2020 2020 206e 756d 6265 723d 312c         number=1,
+00013ba0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+00013bb0: 3d64 6174 655f 7062 322e 4461 7465 2c0a  =date_pb2.Date,.
+00013bc0: 2020 2020 290a 2020 2020 646f 6d61 696e      ).    domain
+00013bd0: 3a20 7374 7220 3d20 7072 6f74 6f2e 4669  : str = proto.Fi
+00013be0: 656c 6428 0a20 2020 2020 2020 2070 726f  eld(.        pro
+00013bf0: 746f 2e53 5452 494e 472c 0a20 2020 2020  to.STRING,.     
+00013c00: 2020 206e 756d 6265 723d 322c 0a20 2020     number=2,.   
+00013c10: 2020 2020 206f 7074 696f 6e61 6c3d 5472       optional=Tr
+00013c20: 7565 2c0a 2020 2020 290a 2020 2020 6973  ue,.    ).    is
+00013c30: 5f79 6f75 725f 646f 6d61 696e 3a20 626f  _your_domain: bo
+00013c40: 6f6c 203d 2070 726f 746f 2e46 6965 6c64  ol = proto.Field
+00013c50: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00013c60: 424f 4f4c 2c0a 2020 2020 2020 2020 6e75  BOOL,.        nu
+00013c70: 6d62 6572 3d33 2c0a 2020 2020 2020 2020  mber=3,.        
+00013c80: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00013c90: 2020 2029 0a20 2020 2072 6570 6f72 745f     ).    report_
+00013ca0: 636f 756e 7472 795f 636f 6465 3a20 7374  country_code: st
+00013cb0: 7220 3d20 7072 6f74 6f2e 4669 656c 6428  r = proto.Field(
+00013cc0: 0a20 2020 2020 2020 2070 726f 746f 2e53  .        proto.S
+00013cd0: 5452 494e 472c 0a20 2020 2020 2020 206e  TRING,.        n
+00013ce0: 756d 6265 723d 342c 0a20 2020 2020 2020  umber=4,.       
+00013cf0: 206f 7074 696f 6e61 6c3d 5472 7565 2c0a   optional=True,.
+00013d00: 2020 2020 290a 2020 2020 7265 706f 7274      ).    report
+00013d10: 5f63 6174 6567 6f72 795f 6964 3a20 696e  _category_id: in
+00013d20: 7420 3d20 7072 6f74 6f2e 4669 656c 6428  t = proto.Field(
+00013d30: 0a20 2020 2020 2020 2070 726f 746f 2e49  .        proto.I
+00013d40: 4e54 3634 2c0a 2020 2020 2020 2020 6e75  NT64,.        nu
+00013d50: 6d62 6572 3d35 2c0a 2020 2020 2020 2020  mber=5,.        
+00013d60: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00013d70: 2020 2029 0a20 2020 2074 7261 6666 6963     ).    traffic
+00013d80: 5f73 6f75 7263 653a 2022 5472 6166 6669  _source: "Traffi
+00013d90: 6353 6f75 7263 652e 5472 6166 6669 6353  cSource.TrafficS
+00013da0: 6f75 7263 6545 6e75 6d22 203d 2070 726f  ourceEnum" = pro
+00013db0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+00013dc0: 2020 7072 6f74 6f2e 454e 554d 2c0a 2020    proto.ENUM,.  
+00013dd0: 2020 2020 2020 6e75 6d62 6572 3d36 2c0a        number=6,.
+00013de0: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00013df0: 3d54 7275 652c 0a20 2020 2020 2020 2065  =True,.        e
+00013e00: 6e75 6d3d 2254 7261 6666 6963 536f 7572  num="TrafficSour
+00013e10: 6365 2e54 7261 6666 6963 536f 7572 6365  ce.TrafficSource
+00013e20: 456e 756d 222c 0a20 2020 2029 0a20 2020  Enum",.    ).   
+00013e30: 2072 616e 6b3a 2069 6e74 203d 2070 726f   rank: int = pro
+00013e40: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+00013e50: 2020 7072 6f74 6f2e 494e 5436 342c 0a20    proto.INT64,. 
+00013e60: 2020 2020 2020 206e 756d 6265 723d 372c         number=7,
+00013e70: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+00013e80: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+00013e90: 2020 6164 735f 6f72 6761 6e69 635f 7261    ads_organic_ra
+00013ea0: 7469 6f3a 2066 6c6f 6174 203d 2070 726f  tio: float = pro
+00013eb0: 746f 2e46 6965 6c64 280a 2020 2020 2020  to.Field(.      
+00013ec0: 2020 7072 6f74 6f2e 444f 5542 4c45 2c0a    proto.DOUBLE,.
+00013ed0: 2020 2020 2020 2020 6e75 6d62 6572 3d38          number=8
+00013ee0: 2c0a 2020 2020 2020 2020 6f70 7469 6f6e  ,.        option
+00013ef0: 616c 3d54 7275 652c 0a20 2020 2029 0a20  al=True,.    ). 
+00013f00: 2020 2070 6167 655f 6f76 6572 6c61 705f     page_overlap_
+00013f10: 7261 7465 3a20 666c 6f61 7420 3d20 7072  rate: float = pr
+00013f20: 6f74 6f2e 4669 656c 6428 0a20 2020 2020  oto.Field(.     
+00013f30: 2020 2070 726f 746f 2e44 4f55 424c 452c     proto.DOUBLE,
+00013f40: 0a20 2020 2020 2020 206e 756d 6265 723d  .        number=
+00013f50: 392c 0a20 2020 2020 2020 206f 7074 696f  9,.        optio
+00013f60: 6e61 6c3d 5472 7565 2c0a 2020 2020 290a  nal=True,.    ).
+00013f70: 2020 2020 6869 6768 6572 5f70 6f73 6974      higher_posit
+00013f80: 696f 6e5f 7261 7465 3a20 666c 6f61 7420  ion_rate: float 
+00013f90: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00013fa0: 2020 2020 2020 2070 726f 746f 2e44 4f55         proto.DOU
+00013fb0: 424c 452c 0a20 2020 2020 2020 206e 756d  BLE,.        num
+00013fc0: 6265 723d 3130 2c0a 2020 2020 2020 2020  ber=10,.        
+00013fd0: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00013fe0: 2020 2029 0a0a 0a63 6c61 7373 2043 6f6d     )...class Com
+00013ff0: 7065 7469 7469 7665 5669 7369 6269 6c69  petitiveVisibili
+00014000: 7479 4265 6e63 686d 6172 6b56 6965 7728  tyBenchmarkView(
+00014010: 7072 6f74 6f2e 4d65 7373 6167 6529 3a0a  proto.Message):.
+00014020: 2020 2020 7222 2222 4669 656c 6473 2061      r"""Fields a
+00014030: 7661 696c 6162 6c65 2066 6f72 2071 7565  vailable for que
+00014040: 7279 2069 6e0a 2020 2020 6060 636f 6d70  ry in.    ``comp
+00014050: 6574 6974 6976 655f 7669 7369 6269 6c69  etitive_visibili
+00014060: 7479 5f62 656e 6368 6d61 726b 5f76 6965  ty_benchmark_vie
+00014070: 7760 6020 7461 626c 652e 0a0a 2020 2020  w`` table...    
+00014080: 6043 6f6d 7065 7469 7469 7665 0a20 2020  `Competitive.   
+00014090: 2076 6973 6962 696c 6974 7920 3c68 7474   visibility <htt
+000140a0: 7073 3a2f 2f73 7570 706f 7274 2e67 6f6f  ps://support.goo
+000140b0: 676c 652e 636f 6d2f 6d65 7263 6861 6e74  gle.com/merchant
+000140c0: 732f 616e 7377 6572 2f31 3133 3636 3434  s/answer/1136644
+000140d0: 323e 605f 5f0a 2020 2020 7265 706f 7274  2>`__.    report
+000140e0: 2077 6974 6820 7468 6520 6361 7465 676f   with the catego
+000140f0: 7279 2062 656e 6368 6d61 726b 2e0a 0a20  ry benchmark... 
+00014100: 2020 2056 616c 7565 7320 6172 6520 6f6e     Values are on
+00014110: 6c79 2073 6574 2066 6f72 2066 6965 6c64  ly set for field
+00014120: 7320 7265 7175 6573 7465 6420 6578 706c  s requested expl
+00014130: 6963 6974 6c79 2069 6e20 7468 6520 7265  icitly in the re
+00014140: 7175 6573 7427 730a 2020 2020 7365 6172  quest's.    sear
+00014150: 6368 2071 7565 7279 2e0a 0a0a 2020 2020  ch query....    
+00014160: 2e2e 205f 6f6e 656f 663a 2068 7474 7073  .. _oneof: https
+00014170: 3a2f 2f70 726f 746f 2d70 6c75 732d 7079  ://proto-plus-py
+00014180: 7468 6f6e 2e72 6561 6474 6865 646f 6373  thon.readthedocs
+00014190: 2e69 6f2f 656e 2f73 7461 626c 652f 6669  .io/en/stable/fi
+000141a0: 656c 6473 2e68 746d 6c23 6f6e 656f 6673  elds.html#oneofs
+000141b0: 2d6d 7574 7561 6c6c 792d 6578 636c 7573  -mutually-exclus
+000141c0: 6976 652d 6669 656c 6473 0a0a 2020 2020  ive-fields..    
+000141d0: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
+000141e0: 2020 2020 6461 7465 2028 676f 6f67 6c65      date (google
+000141f0: 2e74 7970 652e 6461 7465 5f70 6232 2e44  .type.date_pb2.D
+00014200: 6174 6529 3a0a 2020 2020 2020 2020 2020  ate):.          
+00014210: 2020 4461 7465 206f 6620 7468 6973 2072    Date of this r
+00014220: 6f77 2e0a 0a20 2020 2020 2020 2020 2020  ow...           
+00014230: 2052 6571 7569 7265 6420 696e 2074 6865   Required in the
+00014240: 2060 6053 454c 4543 5460 6020 636c 6175   ``SELECT`` clau
+00014250: 7365 2e20 4120 636f 6e64 6974 696f 6e20  se. A condition 
+00014260: 6f6e 2060 6064 6174 6560 600a 2020 2020  on ``date``.    
+00014270: 2020 2020 2020 2020 6973 2072 6571 7569          is requi
+00014280: 7265 6420 696e 2074 6865 2060 6057 4845  red in the ``WHE
+00014290: 5245 6060 2063 6c61 7573 652e 0a20 2020  RE`` clause..   
+000142a0: 2020 2020 2072 6570 6f72 745f 636f 756e       report_coun
+000142b0: 7472 795f 636f 6465 2028 7374 7229 3a0a  try_code (str):.
+000142c0: 2020 2020 2020 2020 2020 2020 436f 756e              Coun
+000142d0: 7472 7920 7768 6572 6520 696d 7072 6573  try where impres
+000142e0: 7369 6f6e 7320 6170 7065 6172 6564 2e0a  sions appeared..
+000142f0: 0a20 2020 2020 2020 2020 2020 2052 6571  .            Req
+00014300: 7569 7265 6420 696e 2074 6865 2060 6053  uired in the ``S
+00014310: 454c 4543 5460 6020 636c 6175 7365 2e20  ELECT`` clause. 
+00014320: 4120 636f 6e64 6974 696f 6e20 6f6e 0a20  A condition on. 
+00014330: 2020 2020 2020 2020 2020 2060 6072 6570             ``rep
+00014340: 6f72 745f 636f 756e 7472 795f 636f 6465  ort_country_code
+00014350: 6060 2069 7320 7265 7175 6972 6564 2069  `` is required i
+00014360: 6e20 7468 6520 6060 5748 4552 4560 6020  n the ``WHERE`` 
+00014370: 636c 6175 7365 2e0a 0a20 2020 2020 2020  clause...       
+00014380: 2020 2020 2054 6869 7320 6669 656c 6420       This field 
+00014390: 6973 2061 206d 656d 6265 7220 6f66 2060  is a member of `
+000143a0: 6f6e 656f 6660 5f20 6060 5f72 6570 6f72  oneof`_ ``_repor
+000143b0: 745f 636f 756e 7472 795f 636f 6465 6060  t_country_code``
+000143c0: 2e0a 2020 2020 2020 2020 7265 706f 7274  ..        report
+000143d0: 5f63 6174 6567 6f72 795f 6964 2028 696e  _category_id (in
+000143e0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+000143f0: 476f 6f67 6c65 2070 726f 6475 6374 2063  Google product c
+00014400: 6174 6567 6f72 7920 4944 2074 6f20 6361  ategory ID to ca
+00014410: 6c63 756c 6174 6520 7468 6520 7265 706f  lculate the repo
+00014420: 7274 2066 6f72 2c0a 2020 2020 2020 2020  rt for,.        
+00014430: 2020 2020 7265 7072 6573 656e 7465 6420      represented 
+00014440: 696e 2060 476f 6f67 6c65 2773 2070 726f  in `Google's pro
+00014450: 6475 6374 0a20 2020 2020 2020 2020 2020  duct.           
+00014460: 2074 6178 6f6e 6f6d 7920 3c68 7474 7073   taxonomy <https
+00014470: 3a2f 2f73 7570 706f 7274 2e67 6f6f 676c  ://support.googl
+00014480: 652e 636f 6d2f 6d65 7263 6861 6e74 732f  e.com/merchants/
+00014490: 616e 7377 6572 2f36 3332 3434 3336 3e60  answer/6324436>`
+000144a0: 5f5f 2e0a 0a20 2020 2020 2020 2020 2020  __...           
+000144b0: 2052 6571 7569 7265 6420 696e 2074 6865   Required in the
+000144c0: 2060 6053 454c 4543 5460 6020 636c 6175   ``SELECT`` clau
+000144d0: 7365 2e20 4120 636f 6e64 6974 696f 6e20  se. A condition 
+000144e0: 6f6e 0a20 2020 2020 2020 2020 2020 2060  on.            `
+000144f0: 6072 6570 6f72 745f 6361 7465 676f 7279  `report_category
+00014500: 5f69 6460 6020 6973 2072 6571 7569 7265  _id`` is require
+00014510: 6420 696e 2074 6865 2060 6057 4845 5245  d in the ``WHERE
+00014520: 6060 2063 6c61 7573 652e 0a0a 2020 2020  `` clause...    
+00014530: 2020 2020 2020 2020 5468 6973 2066 6965          This fie
+00014540: 6c64 2069 7320 6120 6d65 6d62 6572 206f  ld is a member o
+00014550: 6620 606f 6e65 6f66 605f 2060 605f 7265  f `oneof`_ ``_re
+00014560: 706f 7274 5f63 6174 6567 6f72 795f 6964  port_category_id
+00014570: 6060 2e0a 2020 2020 2020 2020 7472 6166  ``..        traf
+00014580: 6669 635f 736f 7572 6365 2028 676f 6f67  fic_source (goog
+00014590: 6c65 2e73 686f 7070 696e 672e 6d65 7263  le.shopping.merc
+000145a0: 6861 6e74 5f72 6570 6f72 7473 5f76 3162  hant_reports_v1b
+000145b0: 6574 612e 7479 7065 732e 5472 6166 6669  eta.types.Traffi
+000145c0: 6353 6f75 7263 652e 5472 6166 6669 6353  cSource.TrafficS
+000145d0: 6f75 7263 6545 6e75 6d29 3a0a 2020 2020  ourceEnum):.    
+000145e0: 2020 2020 2020 2020 5472 6166 6669 6320          Traffic 
+000145f0: 736f 7572 6365 206f 6620 696d 7072 6573  source of impres
+00014600: 7369 6f6e 732e 0a0a 2020 2020 2020 2020  sions...        
+00014610: 2020 2020 5265 7175 6972 6564 2069 6e20      Required in 
+00014620: 7468 6520 6060 5345 4c45 4354 6060 2063  the ``SELECT`` c
+00014630: 6c61 7573 652e 0a0a 2020 2020 2020 2020  lause...        
+00014640: 2020 2020 5468 6973 2066 6965 6c64 2069      This field i
+00014650: 7320 6120 6d65 6d62 6572 206f 6620 606f  s a member of `o
+00014660: 6e65 6f66 605f 2060 605f 7472 6166 6669  neof`_ ``_traffi
+00014670: 635f 736f 7572 6365 6060 2e0a 2020 2020  c_source``..    
+00014680: 2020 2020 796f 7572 5f64 6f6d 6169 6e5f      your_domain_
+00014690: 7669 7369 6269 6c69 7479 5f74 7265 6e64  visibility_trend
+000146a0: 2028 666c 6f61 7429 3a0a 2020 2020 2020   (float):.      
+000146b0: 2020 2020 2020 4368 616e 6765 2069 6e20        Change in 
+000146c0: 7669 7369 6269 6c69 7479 2062 6173 6564  visibility based
+000146d0: 206f 6e20 696d 7072 6573 7369 6f6e 7320   on impressions 
+000146e0: 666f 720a 2020 2020 2020 2020 2020 2020  for.            
+000146f0: 796f 7572 2064 6f6d 6169 6e20 7769 7468  your domain with
+00014700: 2072 6573 7065 6374 2074 6f20 7468 6520   respect to the 
+00014710: 7374 6172 7420 6f66 2074 6865 0a20 2020  start of the.   
+00014720: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
+00014730: 6420 7469 6d65 2072 616e 6765 2028 6f72  d time range (or
+00014740: 2066 6972 7374 2064 6179 2077 6974 6820   first day with 
+00014750: 6e6f 6e2d 7a65 726f 0a20 2020 2020 2020  non-zero.       
+00014760: 2020 2020 2069 6d70 7265 7373 696f 6e73       impressions
+00014770: 292e 0a0a 2020 2020 2020 2020 2020 2020  )...            
+00014780: 4361 6e6e 6f74 2062 6520 6669 6c74 6572  Cannot be filter
+00014790: 6564 206f 6e20 696e 2074 6865 2027 5748  ed on in the 'WH
+000147a0: 4552 4527 2063 6c61 7573 652e 0a0a 2020  ERE' clause...  
+000147b0: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+000147c0: 6965 6c64 2069 7320 6120 6d65 6d62 6572  ield is a member
+000147d0: 206f 6620 606f 6e65 6f66 605f 2060 605f   of `oneof`_ ``_
+000147e0: 796f 7572 5f64 6f6d 6169 6e5f 7669 7369  your_domain_visi
+000147f0: 6269 6c69 7479 5f74 7265 6e64 6060 2e0a  bility_trend``..
+00014800: 2020 2020 2020 2020 6361 7465 676f 7279          category
+00014810: 5f62 656e 6368 6d61 726b 5f76 6973 6962  _benchmark_visib
+00014820: 696c 6974 795f 7472 656e 6420 2866 6c6f  ility_trend (flo
+00014830: 6174 293a 0a20 2020 2020 2020 2020 2020  at):.           
+00014840: 2043 6861 6e67 6520 696e 2076 6973 6962   Change in visib
+00014850: 696c 6974 7920 6261 7365 6420 6f6e 2069  ility based on i
+00014860: 6d70 7265 7373 696f 6e73 0a20 2020 2020  mpressions.     
+00014870: 2020 2020 2020 2077 6974 6820 7265 7370         with resp
+00014880: 6563 7420 746f 2074 6865 2073 7461 7274  ect to the start
+00014890: 206f 6620 7468 6520 7365 6c65 6374 6564   of the selected
+000148a0: 2074 696d 650a 2020 2020 2020 2020 2020   time.          
+000148b0: 2020 7261 6e67 6520 286f 7220 6669 7273    range (or firs
+000148c0: 7420 6461 7920 7769 7468 206e 6f6e 2d7a  t day with non-z
+000148d0: 6572 6f20 696d 7072 6573 7369 6f6e 7329  ero impressions)
+000148e0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000148f0: 2061 2063 6f6d 6269 6e65 6420 7365 7420   a combined set 
+00014900: 6f66 206d 6572 6368 616e 7473 2077 6974  of merchants wit
+00014910: 6820 6869 6768 6573 740a 2020 2020 2020  h highest.      
+00014920: 2020 2020 2020 7669 7369 6269 6c69 7479        visibility
+00014930: 2061 7070 726f 7869 6d61 7469 6e67 2074   approximating t
+00014940: 6865 206d 6172 6b65 742e 0a0a 2020 2020  he market...    
+00014950: 2020 2020 2020 2020 4361 6e6e 6f74 2062          Cannot b
+00014960: 6520 6669 6c74 6572 6564 206f 6e20 696e  e filtered on in
+00014970: 2074 6865 2027 5748 4552 4527 2063 6c61   the 'WHERE' cla
+00014980: 7573 652e 0a0a 2020 2020 2020 2020 2020  use...          
+00014990: 2020 5468 6973 2066 6965 6c64 2069 7320    This field is 
+000149a0: 6120 6d65 6d62 6572 206f 6620 606f 6e65  a member of `one
+000149b0: 6f66 605f 2060 605f 6361 7465 676f 7279  of`_ ``_category
+000149c0: 5f62 656e 6368 6d61 726b 5f76 6973 6962  _benchmark_visib
+000149d0: 696c 6974 795f 7472 656e 6460 602e 0a20  ility_trend``.. 
+000149e0: 2020 2022 2222 0a0a 2020 2020 6461 7465     """..    date
+000149f0: 3a20 6461 7465 5f70 6232 2e44 6174 6520  : date_pb2.Date 
+00014a00: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00014a10: 2020 2020 2020 2070 726f 746f 2e4d 4553         proto.MES
+00014a20: 5341 4745 2c0a 2020 2020 2020 2020 6e75  SAGE,.        nu
+00014a30: 6d62 6572 3d31 2c0a 2020 2020 2020 2020  mber=1,.        
+00014a40: 6d65 7373 6167 653d 6461 7465 5f70 6232  message=date_pb2
+00014a50: 2e44 6174 652c 0a20 2020 2029 0a20 2020  .Date,.    ).   
+00014a60: 2072 6570 6f72 745f 636f 756e 7472 795f   report_country_
+00014a70: 636f 6465 3a20 7374 7220 3d20 7072 6f74  code: str = prot
+00014a80: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00014a90: 2070 726f 746f 2e53 5452 494e 472c 0a20   proto.STRING,. 
+00014aa0: 2020 2020 2020 206e 756d 6265 723d 322c         number=2,
+00014ab0: 0a20 2020 2020 2020 206f 7074 696f 6e61  .        optiona
+00014ac0: 6c3d 5472 7565 2c0a 2020 2020 290a 2020  l=True,.    ).  
+00014ad0: 2020 7265 706f 7274 5f63 6174 6567 6f72    report_categor
+00014ae0: 795f 6964 3a20 696e 7420 3d20 7072 6f74  y_id: int = prot
+00014af0: 6f2e 4669 656c 6428 0a20 2020 2020 2020  o.Field(.       
+00014b00: 2070 726f 746f 2e49 4e54 3634 2c0a 2020   proto.INT64,.  
+00014b10: 2020 2020 2020 6e75 6d62 6572 3d33 2c0a        number=3,.
+00014b20: 2020 2020 2020 2020 6f70 7469 6f6e 616c          optional
+00014b30: 3d54 7275 652c 0a20 2020 2029 0a20 2020  =True,.    ).   
+00014b40: 2074 7261 6666 6963 5f73 6f75 7263 653a   traffic_source:
+00014b50: 2022 5472 6166 6669 6353 6f75 7263 652e   "TrafficSource.
+00014b60: 5472 6166 6669 6353 6f75 7263 6545 6e75  TrafficSourceEnu
+00014b70: 6d22 203d 2070 726f 746f 2e46 6965 6c64  m" = proto.Field
+00014b80: 280a 2020 2020 2020 2020 7072 6f74 6f2e  (.        proto.
+00014b90: 454e 554d 2c0a 2020 2020 2020 2020 6e75  ENUM,.        nu
+00014ba0: 6d62 6572 3d34 2c0a 2020 2020 2020 2020  mber=4,.        
+00014bb0: 6f70 7469 6f6e 616c 3d54 7275 652c 0a20  optional=True,. 
+00014bc0: 2020 2020 2020 2065 6e75 6d3d 2254 7261         enum="Tra
+00014bd0: 6666 6963 536f 7572 6365 2e54 7261 6666  fficSource.Traff
+00014be0: 6963 536f 7572 6365 456e 756d 222c 0a20  icSourceEnum",. 
+00014bf0: 2020 2029 0a20 2020 2079 6f75 725f 646f     ).    your_do
+00014c00: 6d61 696e 5f76 6973 6962 696c 6974 795f  main_visibility_
+00014c10: 7472 656e 643a 2066 6c6f 6174 203d 2070  trend: float = p
+00014c20: 726f 746f 2e46 6965 6c64 280a 2020 2020  roto.Field(.    
+00014c30: 2020 2020 7072 6f74 6f2e 444f 5542 4c45      proto.DOUBLE
+00014c40: 2c0a 2020 2020 2020 2020 6e75 6d62 6572  ,.        number
+00014c50: 3d35 2c0a 2020 2020 2020 2020 6f70 7469  =5,.        opti
+00014c60: 6f6e 616c 3d54 7275 652c 0a20 2020 2029  onal=True,.    )
+00014c70: 0a20 2020 2063 6174 6567 6f72 795f 6265  .    category_be
+00014c80: 6e63 686d 6172 6b5f 7669 7369 6269 6c69  nchmark_visibili
+00014c90: 7479 5f74 7265 6e64 3a20 666c 6f61 7420  ty_trend: float 
+00014ca0: 3d20 7072 6f74 6f2e 4669 656c 6428 0a20  = proto.Field(. 
+00014cb0: 2020 2020 2020 2070 726f 746f 2e44 4f55         proto.DOU
+00014cc0: 424c 452c 0a20 2020 2020 2020 206e 756d  BLE,.        num
+00014cd0: 6265 723d 362c 0a20 2020 2020 2020 206f  ber=6,.        o
+00014ce0: 7074 696f 6e61 6c3d 5472 7565 2c0a 2020  ptional=True,.  
+00014cf0: 2020 290a 0a0a 636c 6173 7320 4d61 726b    )...class Mark
+00014d00: 6574 696e 674d 6574 686f 6428 7072 6f74  etingMethod(prot
+00014d10: 6f2e 4d65 7373 6167 6529 3a0a 2020 2020  o.Message):.    
+00014d20: 7222 2222 4d61 726b 6574 696e 6720 6d65  r"""Marketing me
+00014d30: 7468 6f64 2075 7365 6420 746f 2070 726f  thod used to pro
+00014d40: 6d6f 7465 2079 6f75 7220 7072 6f64 7563  mote your produc
+00014d50: 7473 206f 6e20 476f 6f67 6c65 0a20 2020  ts on Google.   
+00014d60: 2028 6f72 6761 6e69 6320 7665 7273 7573   (organic versus
+00014d70: 2061 6473 292e 0a0a 2020 2020 2222 220a   ads)...    """.
+00014d80: 0a20 2020 2063 6c61 7373 204d 6172 6b65  .    class Marke
+00014d90: 7469 6e67 4d65 7468 6f64 456e 756d 2870  tingMethodEnum(p
+00014da0: 726f 746f 2e45 6e75 6d29 3a0a 2020 2020  roto.Enum):.    
+00014db0: 2020 2020 7222 2222 4d61 726b 6574 696e      r"""Marketin
+00014dc0: 6720 6d65 7468 6f64 2076 616c 7565 732e  g method values.
+00014dd0: 0a0a 2020 2020 2020 2020 5661 6c75 6573  ..        Values
+00014de0: 3a0a 2020 2020 2020 2020 2020 2020 4d41  :.            MA
+00014df0: 524b 4554 494e 475f 4d45 5448 4f44 5f45  RKETING_METHOD_E
+00014e00: 4e55 4d5f 554e 5350 4543 4946 4945 4420  NUM_UNSPECIFIED 
+00014e10: 2830 293a 0a20 2020 2020 2020 2020 2020  (0):.           
+00014e20: 2020 2020 204e 6f74 2073 7065 6369 6669       Not specifi
+00014e30: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00014e40: 4f52 4741 4e49 4320 2831 293a 0a20 2020  ORGANIC (1):.   
+00014e50: 2020 2020 2020 2020 2020 2020 204f 7267               Org
+00014e60: 616e 6963 206d 6172 6b65 7469 6e67 2e0a  anic marketing..
+00014e70: 2020 2020 2020 2020 2020 2020 4144 5320              ADS 
+00014e80: 2832 293a 0a20 2020 2020 2020 2020 2020  (2):.           
+00014e90: 2020 2020 2041 6473 2d62 6173 6564 206d       Ads-based m
+00014ea0: 6172 6b65 7469 6e67 2e0a 2020 2020 2020  arketing..      
+00014eb0: 2020 2222 220a 2020 2020 2020 2020 4d41    """.        MA
+00014ec0: 524b 4554 494e 475f 4d45 5448 4f44 5f45  RKETING_METHOD_E
+00014ed0: 4e55 4d5f 554e 5350 4543 4946 4945 4420  NUM_UNSPECIFIED 
+00014ee0: 3d20 300a 2020 2020 2020 2020 4f52 4741  = 0.        ORGA
+00014ef0: 4e49 4320 3d20 310a 2020 2020 2020 2020  NIC = 1.        
+00014f00: 4144 5320 3d20 320a 0a0a 636c 6173 7320  ADS = 2...class 
+00014f10: 5265 706f 7274 4772 616e 756c 6172 6974  ReportGranularit
+00014f20: 7928 7072 6f74 6f2e 4d65 7373 6167 6529  y(proto.Message)
+00014f30: 3a0a 2020 2020 7222 2222 4772 616e 756c  :.    r"""Granul
+00014f40: 6172 6974 7920 6f66 2074 6865 2042 6573  arity of the Bes
+00014f50: 7420 7365 6c6c 6572 7320 7265 706f 7274  t sellers report
+00014f60: 2e20 4265 7374 2073 656c 6c65 7273 2072  . Best sellers r
+00014f70: 6570 6f72 7473 0a20 2020 2061 7265 2063  eports.    are c
+00014f80: 6f6d 7075 7465 6420 6f76 6572 2061 2077  omputed over a w
+00014f90: 6565 6b20 616e 6420 6120 6d6f 6e74 6820  eek and a month 
+00014fa0: 7469 6d65 6672 616d 652e 0a0a 2020 2020  timeframe...    
+00014fb0: 2222 220a 0a20 2020 2063 6c61 7373 2052  """..    class R
+00014fc0: 6570 6f72 7447 7261 6e75 6c61 7269 7479  eportGranularity
+00014fd0: 456e 756d 2870 726f 746f 2e45 6e75 6d29  Enum(proto.Enum)
+00014fe0: 3a0a 2020 2020 2020 2020 7222 2222 5265  :.        r"""Re
+00014ff0: 706f 7274 2067 7261 6e75 6c61 7269 7479  port granularity
+00015000: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
+00015010: 2020 5661 6c75 6573 3a0a 2020 2020 2020    Values:.      
+00015020: 2020 2020 2020 5245 504f 5254 5f47 5241        REPORT_GRA
+00015030: 4e55 4c41 5249 5459 5f45 4e55 4d5f 554e  NULARITY_ENUM_UN
+00015040: 5350 4543 4946 4945 4420 2830 293a 0a20  SPECIFIED (0):. 
+00015050: 2020 2020 2020 2020 2020 2020 2020 204e                 N
+00015060: 6f74 2073 7065 6369 6669 6564 2e0a 2020  ot specified..  
+00015070: 2020 2020 2020 2020 2020 5745 454b 4c59            WEEKLY
+00015080: 2028 3129 3a0a 2020 2020 2020 2020 2020   (1):.          
+00015090: 2020 2020 2020 5265 706f 7274 2069 7320        Report is 
+000150a0: 636f 6d70 7574 6564 206f 7665 7220 6120  computed over a 
+000150b0: 7765 656b 2074 696d 6566 7261 6d65 2e0a  week timeframe..
+000150c0: 2020 2020 2020 2020 2020 2020 4d4f 4e54              MONT
+000150d0: 484c 5920 2832 293a 0a20 2020 2020 2020  HLY (2):.       
+000150e0: 2020 2020 2020 2020 2052 6570 6f72 7420           Report 
+000150f0: 6973 2063 6f6d 7075 7465 6420 6f76 6572  is computed over
+00015100: 2061 206d 6f6e 7468 2074 696d 6566 7261   a month timefra
+00015110: 6d65 2e0a 2020 2020 2020 2020 2222 220a  me..        """.
+00015120: 2020 2020 2020 2020 5245 504f 5254 5f47          REPORT_G
+00015130: 5241 4e55 4c41 5249 5459 5f45 4e55 4d5f  RANULARITY_ENUM_
+00015140: 554e 5350 4543 4946 4945 4420 3d20 300a  UNSPECIFIED = 0.
+00015150: 2020 2020 2020 2020 5745 454b 4c59 203d          WEEKLY =
+00015160: 2031 0a20 2020 2020 2020 204d 4f4e 5448   1.        MONTH
+00015170: 4c59 203d 2032 0a0a 0a63 6c61 7373 2052  LY = 2...class R
+00015180: 656c 6174 6976 6544 656d 616e 6428 7072  elativeDemand(pr
+00015190: 6f74 6f2e 4d65 7373 6167 6529 3a0a 2020  oto.Message):.  
+000151a0: 2020 7222 2222 5265 6c61 7469 7665 2064    r"""Relative d
+000151b0: 656d 616e 6420 6f66 2061 2070 726f 6475  emand of a produ
+000151c0: 6374 2063 6c75 7374 6572 206f 7220 6272  ct cluster or br
+000151d0: 616e 6420 696e 2074 6865 2042 6573 740a  and in the Best.
+000151e0: 2020 2020 7365 6c6c 6572 7320 7265 706f      sellers repo
+000151f0: 7274 2e0a 0a20 2020 2022 2222 0a0a 2020  rt...    """..  
+00015200: 2020 636c 6173 7320 5265 6c61 7469 7665    class Relative
+00015210: 4465 6d61 6e64 456e 756d 2870 726f 746f  DemandEnum(proto
+00015220: 2e45 6e75 6d29 3a0a 2020 2020 2020 2020  .Enum):.        
+00015230: 7222 2222 5265 6c61 7469 7665 2064 656d  r"""Relative dem
+00015240: 616e 6420 7661 6c75 6573 2e0a 0a20 2020  and values...   
+00015250: 2020 2020 2056 616c 7565 733a 0a20 2020       Values:.   
+00015260: 2020 2020 2020 2020 2052 454c 4154 4956           RELATIV
+00015270: 455f 4445 4d41 4e44 5f45 4e55 4d5f 554e  E_DEMAND_ENUM_UN
+00015280: 5350 4543 4946 4945 4420 2830 293a 0a20  SPECIFIED (0):. 
+00015290: 2020 2020 2020 2020 2020 2020 2020 204e                 N
+000152a0: 6f74 2073 7065 6369 6669 6564 2e0a 2020  ot specified..  
+000152b0: 2020 2020 2020 2020 2020 5645 5259 5f4c            VERY_L
+000152c0: 4f57 2028 3130 293a 0a20 2020 2020 2020  OW (10):.       
+000152d0: 2020 2020 2020 2020 2044 656d 616e 6420           Demand 
+000152e0: 6973 2030 2d35 2520 6f66 2074 6865 2064  is 0-5% of the d
+000152f0: 656d 616e 6420 6f66 2074 6865 2068 6967  emand of the hig
+00015300: 6865 7374 0a20 2020 2020 2020 2020 2020  hest.           
+00015310: 2020 2020 2072 616e 6b65 6420 7072 6f64       ranked prod
+00015320: 7563 7420 636c 7573 7465 7220 6f72 2062  uct cluster or b
+00015330: 7261 6e64 2e0a 2020 2020 2020 2020 2020  rand..          
+00015340: 2020 4c4f 5720 2832 3029 3a0a 2020 2020    LOW (20):.    
+00015350: 2020 2020 2020 2020 2020 2020 4465 6d61              Dema
+00015360: 6e64 2069 7320 362d 3130 2520 6f66 2074  nd is 6-10% of t
+00015370: 6865 2064 656d 616e 6420 6f66 2074 6865  he demand of the
+00015380: 2068 6967 6865 7374 0a20 2020 2020 2020   highest.       
+00015390: 2020 2020 2020 2020 2072 616e 6b65 6420           ranked 
+000153a0: 7072 6f64 7563 7420 636c 7573 7465 7220  product cluster 
+000153b0: 6f72 2062 7261 6e64 2e0a 2020 2020 2020  or brand..      
+000153c0: 2020 2020 2020 4d45 4449 554d 2028 3330        MEDIUM (30
+000153d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000153e0: 2020 2044 656d 616e 6420 6973 2031 312d     Demand is 11-
+000153f0: 3230 2520 6f66 2074 6865 2064 656d 616e  20% of the deman
+00015400: 6420 6f66 2074 6865 2068 6967 6865 7374  d of the highest
+00015410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015420: 2072 616e 6b65 6420 7072 6f64 7563 7420   ranked product 
+00015430: 636c 7573 7465 7220 6f72 2062 7261 6e64  cluster or brand
+00015440: 2e0a 2020 2020 2020 2020 2020 2020 4849  ..            HI
+00015450: 4748 2028 3430 293a 0a20 2020 2020 2020  GH (40):.       
+00015460: 2020 2020 2020 2020 2044 656d 616e 6420           Demand 
+00015470: 6973 2032 312d 3530 2520 6f66 2074 6865  is 21-50% of the
+00015480: 2064 656d 616e 6420 6f66 2074 6865 2068   demand of the h
+00015490: 6967 6865 7374 0a20 2020 2020 2020 2020  ighest.         
+000154a0: 2020 2020 2020 2072 616e 6b65 6420 7072         ranked pr
+000154b0: 6f64 7563 7420 636c 7573 7465 7220 6f72  oduct cluster or
+000154c0: 2062 7261 6e64 2e0a 2020 2020 2020 2020   brand..        
+000154d0: 2020 2020 5645 5259 5f48 4947 4820 2835      VERY_HIGH (5
+000154e0: 3029 3a0a 2020 2020 2020 2020 2020 2020  0):.            
+000154f0: 2020 2020 4465 6d61 6e64 2069 7320 3531      Demand is 51
+00015500: 2d31 3030 2520 6f66 2074 6865 2064 656d  -100% of the dem
+00015510: 616e 6420 6f66 2074 6865 0a20 2020 2020  and of the.     
+00015520: 2020 2020 2020 2020 2020 2068 6967 6865             highe
+00015530: 7374 2072 616e 6b65 6420 7072 6f64 7563  st ranked produc
+00015540: 7420 636c 7573 7465 7220 6f72 2062 7261  t cluster or bra
+00015550: 6e64 2e0a 2020 2020 2020 2020 2222 220a  nd..        """.
+00015560: 2020 2020 2020 2020 5245 4c41 5449 5645          RELATIVE
+00015570: 5f44 454d 414e 445f 454e 554d 5f55 4e53  _DEMAND_ENUM_UNS
+00015580: 5045 4349 4649 4544 203d 2030 0a20 2020  PECIFIED = 0.   
+00015590: 2020 2020 2056 4552 595f 4c4f 5720 3d20       VERY_LOW = 
+000155a0: 3130 0a20 2020 2020 2020 204c 4f57 203d  10.        LOW =
+000155b0: 2032 300a 2020 2020 2020 2020 4d45 4449   20.        MEDI
+000155c0: 554d 203d 2033 300a 2020 2020 2020 2020  UM = 30.        
+000155d0: 4849 4748 203d 2034 300a 2020 2020 2020  HIGH = 40.      
+000155e0: 2020 5645 5259 5f48 4947 4820 3d20 3530    VERY_HIGH = 50
+000155f0: 0a0a 0a63 6c61 7373 2052 656c 6174 6976  ...class Relativ
+00015600: 6544 656d 616e 6443 6861 6e67 6554 7970  eDemandChangeTyp
+00015610: 6528 7072 6f74 6f2e 4d65 7373 6167 6529  e(proto.Message)
+00015620: 3a0a 2020 2020 7222 2222 5265 6c61 7469  :.    r"""Relati
+00015630: 7665 2064 656d 616e 6420 6f66 2061 2070  ve demand of a p
+00015640: 726f 6475 6374 2063 6c75 7374 6572 206f  roduct cluster o
+00015650: 7220 6272 616e 6420 696e 2074 6865 2042  r brand in the B
+00015660: 6573 740a 2020 2020 7365 6c6c 6572 7320  est.    sellers 
+00015670: 7265 706f 7274 2063 6f6d 7061 7265 6420  report compared 
+00015680: 746f 2074 6865 2070 7265 7669 6f75 7320  to the previous 
+00015690: 7469 6d65 2070 6572 696f 642e 0a0a 2020  time period...  
+000156a0: 2020 2222 220a 0a20 2020 2063 6c61 7373    """..    class
+000156b0: 2052 656c 6174 6976 6544 656d 616e 6443   RelativeDemandC
+000156c0: 6861 6e67 6554 7970 6545 6e75 6d28 7072  hangeTypeEnum(pr
+000156d0: 6f74 6f2e 456e 756d 293a 0a20 2020 2020  oto.Enum):.     
+000156e0: 2020 2072 2222 2252 656c 6174 6976 6520     r"""Relative 
+000156f0: 6465 6d61 6e64 2063 6861 6e67 6520 7479  demand change ty
+00015700: 7065 2076 616c 7565 732e 0a0a 2020 2020  pe values...    
+00015710: 2020 2020 5661 6c75 6573 3a0a 2020 2020      Values:.    
+00015720: 2020 2020 2020 2020 5245 4c41 5449 5645          RELATIVE
+00015730: 5f44 454d 414e 445f 4348 414e 4745 5f54  _DEMAND_CHANGE_T
+00015740: 5950 455f 454e 554d 5f55 4e53 5045 4349  YPE_ENUM_UNSPECI
+00015750: 4649 4544 2028 3029 3a0a 2020 2020 2020  FIED (0):.      
+00015760: 2020 2020 2020 2020 2020 4e6f 7420 7370            Not sp
+00015770: 6563 6966 6965 642e 0a20 2020 2020 2020  ecified..       
+00015780: 2020 2020 2053 494e 4b45 5220 2831 293a       SINKER (1):
+00015790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000157a0: 2052 656c 6174 6976 6520 6465 6d61 6e64   Relative demand
+000157b0: 2069 7320 6c6f 7765 7220 7468 616e 2074   is lower than t
+000157c0: 6865 2070 7265 7669 6f75 730a 2020 2020  he previous.    
+000157d0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+000157e0: 2070 6572 696f 642e 0a20 2020 2020 2020   period..       
+000157f0: 2020 2020 2046 4c41 5420 2832 293a 0a20       FLAT (2):. 
+00015800: 2020 2020 2020 2020 2020 2020 2020 2052                 R
+00015810: 656c 6174 6976 6520 6465 6d61 6e64 2069  elative demand i
+00015820: 7320 6571 7561 6c20 746f 2074 6865 2070  s equal to the p
+00015830: 7265 7669 6f75 7320 7469 6d65 0a20 2020  revious time.   
+00015840: 2020 2020 2020 2020 2020 2020 2070 6572               per
+00015850: 696f 642e 0a20 2020 2020 2020 2020 2020  iod..           
+00015860: 2052 4953 4552 2028 3329 3a0a 2020 2020   RISER (3):.    
+00015870: 2020 2020 2020 2020 2020 2020 5265 6c61              Rela
+00015880: 7469 7665 2064 656d 616e 6420 6973 2068  tive demand is h
+00015890: 6967 6865 7220 7468 616e 2074 6865 2070  igher than the p
+000158a0: 7265 7669 6f75 730a 2020 2020 2020 2020  revious.        
+000158b0: 2020 2020 2020 2020 7469 6d65 2070 6572          time per
+000158c0: 696f 642e 0a20 2020 2020 2020 2022 2222  iod..        """
+000158d0: 0a20 2020 2020 2020 2052 454c 4154 4956  .        RELATIV
+000158e0: 455f 4445 4d41 4e44 5f43 4841 4e47 455f  E_DEMAND_CHANGE_
+000158f0: 5459 5045 5f45 4e55 4d5f 554e 5350 4543  TYPE_ENUM_UNSPEC
+00015900: 4946 4945 4420 3d20 300a 2020 2020 2020  IFIED = 0.      
+00015910: 2020 5349 4e4b 4552 203d 2031 0a20 2020    SINKER = 1.   
+00015920: 2020 2020 2046 4c41 5420 3d20 320a 2020       FLAT = 2.  
+00015930: 2020 2020 2020 5249 5345 5220 3d20 330a        RISER = 3.
+00015940: 0a0a 636c 6173 7320 5472 6166 6669 6353  ..class TrafficS
+00015950: 6f75 7263 6528 7072 6f74 6f2e 4d65 7373  ource(proto.Mess
+00015960: 6167 6529 3a0a 2020 2020 7222 2222 5472  age):.    r"""Tr
+00015970: 6166 6669 6320 736f 7572 6365 206f 6620  affic source of 
+00015980: 696d 7072 6573 7369 6f6e 7320 696e 2074  impressions in t
+00015990: 6865 2043 6f6d 7065 7469 7469 7665 2076  he Competitive v
+000159a0: 6973 6962 696c 6974 790a 2020 2020 7265  isibility.    re
+000159b0: 706f 7274 2e0a 0a20 2020 2022 2222 0a0a  port...    """..
+000159c0: 2020 2020 636c 6173 7320 5472 6166 6669      class Traffi
+000159d0: 6353 6f75 7263 6545 6e75 6d28 7072 6f74  cSourceEnum(prot
+000159e0: 6f2e 456e 756d 293a 0a20 2020 2020 2020  o.Enum):.       
+000159f0: 2072 2222 2254 7261 6666 6963 2073 6f75   r"""Traffic sou
+00015a00: 7263 6520 7661 6c75 6573 2e0a 0a20 2020  rce values...   
+00015a10: 2020 2020 2056 616c 7565 733a 0a20 2020       Values:.   
+00015a20: 2020 2020 2020 2020 2054 5241 4646 4943           TRAFFIC
+00015a30: 5f53 4f55 5243 455f 454e 554d 5f55 4e53  _SOURCE_ENUM_UNS
+00015a40: 5045 4349 4649 4544 2028 3029 3a0a 2020  PECIFIED (0):.  
+00015a50: 2020 2020 2020 2020 2020 2020 2020 4e6f                No
+00015a60: 7420 7370 6563 6966 6965 642e 0a20 2020  t specified..   
+00015a70: 2020 2020 2020 2020 204f 5247 414e 4943           ORGANIC
+00015a80: 2028 3129 3a0a 2020 2020 2020 2020 2020   (1):.          
+00015a90: 2020 2020 2020 4f72 6761 6e69 6320 7472        Organic tr
+00015aa0: 6166 6669 632e 0a20 2020 2020 2020 2020  affic..         
+00015ab0: 2020 2041 4453 2028 3229 3a0a 2020 2020     ADS (2):.    
+00015ac0: 2020 2020 2020 2020 2020 2020 5472 6166              Traf
+00015ad0: 6669 6320 6672 6f6d 2061 6473 2e0a 2020  fic from ads..  
+00015ae0: 2020 2020 2020 2020 2020 414c 4c20 2833            ALL (3
+00015af0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00015b00: 2020 204f 7267 616e 6963 2061 6e64 2061     Organic and a
+00015b10: 6473 2074 7261 6666 6963 2e0a 2020 2020  ds traffic..    
+00015b20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00015b30: 5452 4146 4649 435f 534f 5552 4345 5f45  TRAFFIC_SOURCE_E
+00015b40: 4e55 4d5f 554e 5350 4543 4946 4945 4420  NUM_UNSPECIFIED 
+00015b50: 3d20 300a 2020 2020 2020 2020 4f52 4741  = 0.        ORGA
+00015b60: 4e49 4320 3d20 310a 2020 2020 2020 2020  NIC = 1.        
+00015b70: 4144 5320 3d20 320a 2020 2020 2020 2020  ADS = 2.        
+00015b80: 414c 4c20 3d20 330a 0a0a 5f5f 616c 6c5f  ALL = 3...__all_
+00015b90: 5f20 3d20 7475 706c 6528 736f 7274 6564  _ = tuple(sorted
+00015ba0: 285f 5f70 726f 746f 6275 665f 5f2e 6d61  (__protobuf__.ma
+00015bb0: 6e69 6665 7374 2929 0a                   nifest)).
```

### Comparing `google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/PKG-INFO` & `google-shopping-merchant-reports-0.1.7/google_shopping_merchant_reports.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-merchant-reports
-Version: 0.1.6
+Version: 0.1.7
 Summary: Google Shopping Merchant Reports API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-reports
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-merchant-reports-0.1.6/google_shopping_merchant_reports.egg-info/SOURCES.txt` & `google-shopping-merchant-reports-0.1.7/google_shopping_merchant_reports.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/setup.py` & `google-shopping-merchant-reports-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/tests/__init__.py` & `google-shopping-merchant-reports-0.1.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/tests/unit/__init__.py` & `google-shopping-merchant-reports-0.1.7/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/tests/unit/gapic/__init__.py` & `google-shopping-merchant-reports-0.1.7/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/tests/unit/gapic/merchant_reports_v1beta/__init__.py` & `google-shopping-merchant-reports-0.1.7/tests/unit/gapic/merchant_reports_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-reports-0.1.6/tests/unit/gapic/merchant_reports_v1beta/test_report_service.py` & `google-shopping-merchant-reports-0.1.7/tests/unit/gapic/merchant_reports_v1beta/test_report_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1154,14 +1154,17 @@
     client = ReportServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.search), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.search()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == reports.SearchRequest()
 
 
 def test_search_non_empty_request_with_auto_populated_field():
@@ -1179,24 +1182,62 @@
         parent="parent_value",
         query="query_value",
         page_token="page_token_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.search), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.search(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == reports.SearchRequest(
             parent="parent_value",
             query="query_value",
             page_token="page_token_value",
         )
 
 
+def test_search_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ReportServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.search in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.search] = mock_rpc
+        request = {}
+        client.search(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.search(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_search_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ReportServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1213,14 +1254,58 @@
         response = await client.search()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == reports.SearchRequest()
 
 
 @pytest.mark.asyncio
+async def test_search_async_use_cached_wrapped_rpc(transport: str = "grpc_asyncio"):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = ReportServiceAsyncClient(
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
+            client._client._transport.search
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
+            client._client._transport.search
+        ] = mock_object
+
+        request = {}
+        await client.search(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.search(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_search_async(
     transport: str = "grpc_asyncio", request_type=reports.SearchRequest
 ):
     client = ReportServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -1622,14 +1707,50 @@
         response = client.search(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.SearchPager)
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_search_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = ReportServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.search in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.search] = mock_rpc
+
+        request = {}
+        client.search(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.search(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_search_rest_required_fields(request_type=reports.SearchRequest):
     transport_class = transports.ReportServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
     request_init["query"] = ""
     request = request_type(**request_init)
```

