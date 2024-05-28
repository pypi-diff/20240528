# Comparing `tmp/google-cloud-securitycentermanagement-0.1.8.tar.gz` & `tmp/google-cloud-securitycentermanagement-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-securitycentermanagement-0.1.8.tar", last modified: Fri Mar 22 12:20:01 2024, max compression
+gzip compressed data, was "google-cloud-securitycentermanagement-0.1.9.tar", last modified: Tue May 28 08:23:51 2024, max compression
```

## Comparing `google-cloud-securitycentermanagement-0.1.8.tar` & `google-cloud-securitycentermanagement-0.1.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.471060 google-cloud-securitycentermanagement-0.1.8/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5502 2024-03-22 12:20:01.471060 google-cloud-securitycentermanagement-0.1.8/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4035 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.455059 google-cloud-securitycentermanagement-0.1.8/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.459059 google-cloud-securitycentermanagement-0.1.8/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.459059 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement/
--rw-rw-r--   0 root         (0)     1003     4595 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       98 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.463059 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/
--rw-rw-r--   0 root         (0)     1003     4405 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10666 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       98 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.463059 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.463059 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/
--rw-rw-r--   0 root         (0)     1003      809 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/__init__.py
--rw-rw-r--   0 root         (0)     1003   123047 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/async_client.py
--rw-rw-r--   0 root         (0)     1003   143301 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/client.py
--rw-rw-r--   0 root         (0)     1003    40238 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.463059 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/
--rw-rw-r--   0 root         (0)     1003     1561 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    24003 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/base.py
--rw-rw-r--   0 root         (0)     1003    44818 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    45605 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   138159 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.467060 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/types/
--rw-rw-r--   0 root         (0)     1003     4057 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    65759 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/types/security_center_management.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.467060 google-cloud-securitycentermanagement-0.1.8/google_cloud_securitycentermanagement.egg-info/
--rw-r--r--   0 root         (0)     1003     5502 2024-03-22 12:20:01.000000 google-cloud-securitycentermanagement-0.1.8/google_cloud_securitycentermanagement.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2030 2024-03-22 12:20:01.000000 google-cloud-securitycentermanagement-0.1.8/google_cloud_securitycentermanagement.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-22 12:20:01.000000 google-cloud-securitycentermanagement-0.1.8/google_cloud_securitycentermanagement.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-22 12:20:01.000000 google-cloud-securitycentermanagement-0.1.8/google_cloud_securitycentermanagement.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      342 2024-03-22 12:20:01.000000 google-cloud-securitycentermanagement-0.1.8/google_cloud_securitycentermanagement.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-22 12:20:01.000000 google-cloud-securitycentermanagement-0.1.8/google_cloud_securitycentermanagement.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-22 12:20:01.471060 google-cloud-securitycentermanagement-0.1.8/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3284 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.467060 google-cloud-securitycentermanagement-0.1.8/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.467060 google-cloud-securitycentermanagement-0.1.8/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.467060 google-cloud-securitycentermanagement-0.1.8/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:20:01.467060 google-cloud-securitycentermanagement-0.1.8/tests/unit/gapic/securitycentermanagement_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/tests/unit/gapic/securitycentermanagement_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   602811 2024-03-22 12:15:16.000000 google-cloud-securitycentermanagement-0.1.8/tests/unit/gapic/securitycentermanagement_v1/test_security_center_management.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.657056 google-cloud-securitycentermanagement-0.1.9/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5502 2024-05-28 08:23:51.657056 google-cloud-securitycentermanagement-0.1.9/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4035 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.645053 google-cloud-securitycentermanagement-0.1.9/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.645053 google-cloud-securitycentermanagement-0.1.9/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.649054 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement/
+-rw-rw-r--   0 root         (0)     1003     4971 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       98 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.649054 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/
+-rw-rw-r--   0 root         (0)     1003     4781 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12010 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       98 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.649054 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.653055 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/
+-rw-rw-r--   0 root         (0)     1003      809 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/__init__.py
+-rw-rw-r--   0 root         (0)     1003   140820 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/async_client.py
+-rw-rw-r--   0 root         (0)     1003   159771 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/client.py
+-rw-rw-r--   0 root         (0)     1003    46098 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.653055 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/
+-rw-rw-r--   0 root         (0)     1003     1561 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25783 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    49669 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    61067 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   157660 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.653055 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4433 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    76044 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/types/security_center_management.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.657056 google-cloud-securitycentermanagement-0.1.9/google_cloud_securitycentermanagement.egg-info/
+-rw-r--r--   0 root         (0)     1003     5502 2024-05-28 08:23:51.000000 google-cloud-securitycentermanagement-0.1.9/google_cloud_securitycentermanagement.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2030 2024-05-28 08:23:51.000000 google-cloud-securitycentermanagement-0.1.9/google_cloud_securitycentermanagement.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-28 08:23:51.000000 google-cloud-securitycentermanagement-0.1.9/google_cloud_securitycentermanagement.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-28 08:23:51.000000 google-cloud-securitycentermanagement-0.1.9/google_cloud_securitycentermanagement.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      342 2024-05-28 08:23:51.000000 google-cloud-securitycentermanagement-0.1.9/google_cloud_securitycentermanagement.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-28 08:23:51.000000 google-cloud-securitycentermanagement-0.1.9/google_cloud_securitycentermanagement.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-28 08:23:51.657056 google-cloud-securitycentermanagement-0.1.9/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3284 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.657056 google-cloud-securitycentermanagement-0.1.9/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.657056 google-cloud-securitycentermanagement-0.1.9/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.657056 google-cloud-securitycentermanagement-0.1.9/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:51.657056 google-cloud-securitycentermanagement-0.1.9/tests/unit/gapic/securitycentermanagement_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/tests/unit/gapic/securitycentermanagement_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   844453 2024-05-28 08:20:20.000000 google-cloud-securitycentermanagement-0.1.9/tests/unit/gapic/securitycentermanagement_v1/test_security_center_management.py
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/LICENSE` & `google-cloud-securitycentermanagement-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycentermanagement-0.1.8/MANIFEST.in` & `google-cloud-securitycentermanagement-0.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycentermanagement-0.1.8/PKG-INFO` & `google-cloud-securitycentermanagement-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-securitycentermanagement
-Version: 0.1.8
+Version: 0.1.9
 Summary: Google Cloud Securitycentermanagement API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-securitycentermanagement
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/README.rst` & `google-cloud-securitycentermanagement-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement/__init__.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,89 +9,86 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.securitycentermanagement import gapic_version as package_version
-
-__version__ = package_version.__version__
-
-
-from google.cloud.securitycentermanagement_v1.services.security_center_management.async_client import (
-    SecurityCenterManagementAsyncClient,
-)
-from google.cloud.securitycentermanagement_v1.services.security_center_management.client import (
-    SecurityCenterManagementClient,
-)
-from google.cloud.securitycentermanagement_v1.types.security_center_management import (
+from .security_center_management import (
     CreateEventThreatDetectionCustomModuleRequest,
     CreateSecurityHealthAnalyticsCustomModuleRequest,
     CustomConfig,
     DeleteEventThreatDetectionCustomModuleRequest,
     DeleteSecurityHealthAnalyticsCustomModuleRequest,
     EffectiveEventThreatDetectionCustomModule,
     EffectiveSecurityHealthAnalyticsCustomModule,
     EventThreatDetectionCustomModule,
     GetEffectiveEventThreatDetectionCustomModuleRequest,
     GetEffectiveSecurityHealthAnalyticsCustomModuleRequest,
     GetEventThreatDetectionCustomModuleRequest,
+    GetSecurityCenterServiceRequest,
     GetSecurityHealthAnalyticsCustomModuleRequest,
     ListDescendantEventThreatDetectionCustomModulesRequest,
     ListDescendantEventThreatDetectionCustomModulesResponse,
     ListDescendantSecurityHealthAnalyticsCustomModulesRequest,
     ListDescendantSecurityHealthAnalyticsCustomModulesResponse,
     ListEffectiveEventThreatDetectionCustomModulesRequest,
     ListEffectiveEventThreatDetectionCustomModulesResponse,
     ListEffectiveSecurityHealthAnalyticsCustomModulesRequest,
     ListEffectiveSecurityHealthAnalyticsCustomModulesResponse,
     ListEventThreatDetectionCustomModulesRequest,
     ListEventThreatDetectionCustomModulesResponse,
+    ListSecurityCenterServicesRequest,
+    ListSecurityCenterServicesResponse,
     ListSecurityHealthAnalyticsCustomModulesRequest,
     ListSecurityHealthAnalyticsCustomModulesResponse,
+    SecurityCenterService,
     SecurityHealthAnalyticsCustomModule,
     SimulatedFinding,
     SimulateSecurityHealthAnalyticsCustomModuleRequest,
     SimulateSecurityHealthAnalyticsCustomModuleResponse,
     UpdateEventThreatDetectionCustomModuleRequest,
+    UpdateSecurityCenterServiceRequest,
     UpdateSecurityHealthAnalyticsCustomModuleRequest,
     ValidateEventThreatDetectionCustomModuleRequest,
     ValidateEventThreatDetectionCustomModuleResponse,
 )
 
 __all__ = (
-    "SecurityCenterManagementClient",
-    "SecurityCenterManagementAsyncClient",
     "CreateEventThreatDetectionCustomModuleRequest",
     "CreateSecurityHealthAnalyticsCustomModuleRequest",
     "CustomConfig",
     "DeleteEventThreatDetectionCustomModuleRequest",
     "DeleteSecurityHealthAnalyticsCustomModuleRequest",
     "EffectiveEventThreatDetectionCustomModule",
     "EffectiveSecurityHealthAnalyticsCustomModule",
     "EventThreatDetectionCustomModule",
     "GetEffectiveEventThreatDetectionCustomModuleRequest",
     "GetEffectiveSecurityHealthAnalyticsCustomModuleRequest",
     "GetEventThreatDetectionCustomModuleRequest",
+    "GetSecurityCenterServiceRequest",
     "GetSecurityHealthAnalyticsCustomModuleRequest",
     "ListDescendantEventThreatDetectionCustomModulesRequest",
     "ListDescendantEventThreatDetectionCustomModulesResponse",
     "ListDescendantSecurityHealthAnalyticsCustomModulesRequest",
     "ListDescendantSecurityHealthAnalyticsCustomModulesResponse",
     "ListEffectiveEventThreatDetectionCustomModulesRequest",
     "ListEffectiveEventThreatDetectionCustomModulesResponse",
     "ListEffectiveSecurityHealthAnalyticsCustomModulesRequest",
     "ListEffectiveSecurityHealthAnalyticsCustomModulesResponse",
     "ListEventThreatDetectionCustomModulesRequest",
     "ListEventThreatDetectionCustomModulesResponse",
+    "ListSecurityCenterServicesRequest",
+    "ListSecurityCenterServicesResponse",
     "ListSecurityHealthAnalyticsCustomModulesRequest",
     "ListSecurityHealthAnalyticsCustomModulesResponse",
+    "SecurityCenterService",
     "SecurityHealthAnalyticsCustomModule",
     "SimulatedFinding",
     "SimulateSecurityHealthAnalyticsCustomModuleRequest",
     "SimulateSecurityHealthAnalyticsCustomModuleResponse",
     "UpdateEventThreatDetectionCustomModuleRequest",
+    "UpdateSecurityCenterServiceRequest",
     "UpdateSecurityHealthAnalyticsCustomModuleRequest",
     "ValidateEventThreatDetectionCustomModuleRequest",
     "ValidateEventThreatDetectionCustomModuleResponse",
 )
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement/gapic_version.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.8"  # {x-release-please-version}
+__version__ = "0.1.9"  # {x-release-please-version}
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/__init__.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,32 +30,37 @@
     DeleteSecurityHealthAnalyticsCustomModuleRequest,
     EffectiveEventThreatDetectionCustomModule,
     EffectiveSecurityHealthAnalyticsCustomModule,
     EventThreatDetectionCustomModule,
     GetEffectiveEventThreatDetectionCustomModuleRequest,
     GetEffectiveSecurityHealthAnalyticsCustomModuleRequest,
     GetEventThreatDetectionCustomModuleRequest,
+    GetSecurityCenterServiceRequest,
     GetSecurityHealthAnalyticsCustomModuleRequest,
     ListDescendantEventThreatDetectionCustomModulesRequest,
     ListDescendantEventThreatDetectionCustomModulesResponse,
     ListDescendantSecurityHealthAnalyticsCustomModulesRequest,
     ListDescendantSecurityHealthAnalyticsCustomModulesResponse,
     ListEffectiveEventThreatDetectionCustomModulesRequest,
     ListEffectiveEventThreatDetectionCustomModulesResponse,
     ListEffectiveSecurityHealthAnalyticsCustomModulesRequest,
     ListEffectiveSecurityHealthAnalyticsCustomModulesResponse,
     ListEventThreatDetectionCustomModulesRequest,
     ListEventThreatDetectionCustomModulesResponse,
+    ListSecurityCenterServicesRequest,
+    ListSecurityCenterServicesResponse,
     ListSecurityHealthAnalyticsCustomModulesRequest,
     ListSecurityHealthAnalyticsCustomModulesResponse,
+    SecurityCenterService,
     SecurityHealthAnalyticsCustomModule,
     SimulatedFinding,
     SimulateSecurityHealthAnalyticsCustomModuleRequest,
     SimulateSecurityHealthAnalyticsCustomModuleResponse,
     UpdateEventThreatDetectionCustomModuleRequest,
+    UpdateSecurityCenterServiceRequest,
     UpdateSecurityHealthAnalyticsCustomModuleRequest,
     ValidateEventThreatDetectionCustomModuleRequest,
     ValidateEventThreatDetectionCustomModuleResponse,
 )
 
 __all__ = (
     "SecurityCenterManagementAsyncClient",
@@ -66,30 +71,35 @@
     "DeleteSecurityHealthAnalyticsCustomModuleRequest",
     "EffectiveEventThreatDetectionCustomModule",
     "EffectiveSecurityHealthAnalyticsCustomModule",
     "EventThreatDetectionCustomModule",
     "GetEffectiveEventThreatDetectionCustomModuleRequest",
     "GetEffectiveSecurityHealthAnalyticsCustomModuleRequest",
     "GetEventThreatDetectionCustomModuleRequest",
+    "GetSecurityCenterServiceRequest",
     "GetSecurityHealthAnalyticsCustomModuleRequest",
     "ListDescendantEventThreatDetectionCustomModulesRequest",
     "ListDescendantEventThreatDetectionCustomModulesResponse",
     "ListDescendantSecurityHealthAnalyticsCustomModulesRequest",
     "ListDescendantSecurityHealthAnalyticsCustomModulesResponse",
     "ListEffectiveEventThreatDetectionCustomModulesRequest",
     "ListEffectiveEventThreatDetectionCustomModulesResponse",
     "ListEffectiveSecurityHealthAnalyticsCustomModulesRequest",
     "ListEffectiveSecurityHealthAnalyticsCustomModulesResponse",
     "ListEventThreatDetectionCustomModulesRequest",
     "ListEventThreatDetectionCustomModulesResponse",
+    "ListSecurityCenterServicesRequest",
+    "ListSecurityCenterServicesResponse",
     "ListSecurityHealthAnalyticsCustomModulesRequest",
     "ListSecurityHealthAnalyticsCustomModulesResponse",
     "SecurityCenterManagementClient",
+    "SecurityCenterService",
     "SecurityHealthAnalyticsCustomModule",
     "SimulateSecurityHealthAnalyticsCustomModuleRequest",
     "SimulateSecurityHealthAnalyticsCustomModuleResponse",
     "SimulatedFinding",
     "UpdateEventThreatDetectionCustomModuleRequest",
+    "UpdateSecurityCenterServiceRequest",
     "UpdateSecurityHealthAnalyticsCustomModuleRequest",
     "ValidateEventThreatDetectionCustomModuleRequest",
     "ValidateEventThreatDetectionCustomModuleResponse",
 )
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/gapic_metadata.json` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/gapic_metadata.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996279761904763%*

 * *Differences: {"'services'": "{'SecurityCenterManagement': {'clients': {'grpc': {'rpcs': "*

 * *               "{'GetSecurityCenterService': OrderedDict([('methods', "*

 * *               "['get_security_center_service'])]), 'ListSecurityCenterServices': "*

 * *               "OrderedDict([('methods', ['list_security_center_services'])]), "*

 * *               "'UpdateSecurityCenterService': OrderedDict([('methods', "*

 * *               "['update_security_center_service'])])}}, 'grpc-async': {'rpcs': "*

 * *               "{'GetSecurityCenterService […]*

```diff
@@ -41,14 +41,19 @@
                             ]
                         },
                         "GetEventThreatDetectionCustomModule": {
                             "methods": [
                                 "get_event_threat_detection_custom_module"
                             ]
                         },
+                        "GetSecurityCenterService": {
+                            "methods": [
+                                "get_security_center_service"
+                            ]
+                        },
                         "GetSecurityHealthAnalyticsCustomModule": {
                             "methods": [
                                 "get_security_health_analytics_custom_module"
                             ]
                         },
                         "ListDescendantEventThreatDetectionCustomModules": {
                             "methods": [
@@ -71,14 +76,19 @@
                             ]
                         },
                         "ListEventThreatDetectionCustomModules": {
                             "methods": [
                                 "list_event_threat_detection_custom_modules"
                             ]
                         },
+                        "ListSecurityCenterServices": {
+                            "methods": [
+                                "list_security_center_services"
+                            ]
+                        },
                         "ListSecurityHealthAnalyticsCustomModules": {
                             "methods": [
                                 "list_security_health_analytics_custom_modules"
                             ]
                         },
                         "SimulateSecurityHealthAnalyticsCustomModule": {
                             "methods": [
@@ -86,14 +96,19 @@
                             ]
                         },
                         "UpdateEventThreatDetectionCustomModule": {
                             "methods": [
                                 "update_event_threat_detection_custom_module"
                             ]
                         },
+                        "UpdateSecurityCenterService": {
+                            "methods": [
+                                "update_security_center_service"
+                            ]
+                        },
                         "UpdateSecurityHealthAnalyticsCustomModule": {
                             "methods": [
                                 "update_security_health_analytics_custom_module"
                             ]
                         },
                         "ValidateEventThreatDetectionCustomModule": {
                             "methods": [
@@ -136,14 +151,19 @@
                             ]
                         },
                         "GetEventThreatDetectionCustomModule": {
                             "methods": [
                                 "get_event_threat_detection_custom_module"
                             ]
                         },
+                        "GetSecurityCenterService": {
+                            "methods": [
+                                "get_security_center_service"
+                            ]
+                        },
                         "GetSecurityHealthAnalyticsCustomModule": {
                             "methods": [
                                 "get_security_health_analytics_custom_module"
                             ]
                         },
                         "ListDescendantEventThreatDetectionCustomModules": {
                             "methods": [
@@ -166,14 +186,19 @@
                             ]
                         },
                         "ListEventThreatDetectionCustomModules": {
                             "methods": [
                                 "list_event_threat_detection_custom_modules"
                             ]
                         },
+                        "ListSecurityCenterServices": {
+                            "methods": [
+                                "list_security_center_services"
+                            ]
+                        },
                         "ListSecurityHealthAnalyticsCustomModules": {
                             "methods": [
                                 "list_security_health_analytics_custom_modules"
                             ]
                         },
                         "SimulateSecurityHealthAnalyticsCustomModule": {
                             "methods": [
@@ -181,14 +206,19 @@
                             ]
                         },
                         "UpdateEventThreatDetectionCustomModule": {
                             "methods": [
                                 "update_event_threat_detection_custom_module"
                             ]
                         },
+                        "UpdateSecurityCenterService": {
+                            "methods": [
+                                "update_security_center_service"
+                            ]
+                        },
                         "UpdateSecurityHealthAnalyticsCustomModule": {
                             "methods": [
                                 "update_security_health_analytics_custom_module"
                             ]
                         },
                         "ValidateEventThreatDetectionCustomModule": {
                             "methods": [
@@ -231,14 +261,19 @@
                             ]
                         },
                         "GetEventThreatDetectionCustomModule": {
                             "methods": [
                                 "get_event_threat_detection_custom_module"
                             ]
                         },
+                        "GetSecurityCenterService": {
+                            "methods": [
+                                "get_security_center_service"
+                            ]
+                        },
                         "GetSecurityHealthAnalyticsCustomModule": {
                             "methods": [
                                 "get_security_health_analytics_custom_module"
                             ]
                         },
                         "ListDescendantEventThreatDetectionCustomModules": {
                             "methods": [
@@ -261,14 +296,19 @@
                             ]
                         },
                         "ListEventThreatDetectionCustomModules": {
                             "methods": [
                                 "list_event_threat_detection_custom_modules"
                             ]
                         },
+                        "ListSecurityCenterServices": {
+                            "methods": [
+                                "list_security_center_services"
+                            ]
+                        },
                         "ListSecurityHealthAnalyticsCustomModules": {
                             "methods": [
                                 "list_security_health_analytics_custom_modules"
                             ]
                         },
                         "SimulateSecurityHealthAnalyticsCustomModule": {
                             "methods": [
@@ -276,14 +316,19 @@
                             ]
                         },
                         "UpdateEventThreatDetectionCustomModule": {
                             "methods": [
                                 "update_event_threat_detection_custom_module"
                             ]
                         },
+                        "UpdateSecurityCenterService": {
+                            "methods": [
+                                "update_security_center_service"
+                            ]
+                        },
                         "UpdateSecurityHealthAnalyticsCustomModule": {
                             "methods": [
                                 "update_security_health_analytics_custom_module"
                             ]
                         },
                         "ValidateEventThreatDetectionCustomModule": {
                             "methods": [
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/gapic_version.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.8"  # {x-release-please-version}
+__version__ = "0.1.9"  # {x-release-please-version}
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/__init__.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/__init__.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/async_client.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/async_client.py`

 * *Files 7% similar despite different names*

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
@@ -87,14 +88,20 @@
         SecurityCenterManagementClient.event_threat_detection_custom_module_path
     )
     parse_event_threat_detection_custom_module_path = staticmethod(
         SecurityCenterManagementClient.parse_event_threat_detection_custom_module_path
     )
     finding_path = staticmethod(SecurityCenterManagementClient.finding_path)
     parse_finding_path = staticmethod(SecurityCenterManagementClient.parse_finding_path)
+    security_center_service_path = staticmethod(
+        SecurityCenterManagementClient.security_center_service_path
+    )
+    parse_security_center_service_path = staticmethod(
+        SecurityCenterManagementClient.parse_security_center_service_path
+    )
     security_health_analytics_custom_module_path = staticmethod(
         SecurityCenterManagementClient.security_health_analytics_custom_module_path
     )
     parse_security_health_analytics_custom_module_path = staticmethod(
         SecurityCenterManagementClient.parse_security_health_analytics_custom_module_path
     )
     common_billing_account_path = staticmethod(
@@ -228,29 +235,37 @@
         type(SecurityCenterManagementClient),
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, SecurityCenterManagementTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[
+                str,
+                SecurityCenterManagementTransport,
+                Callable[..., SecurityCenterManagementTransport],
+            ]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the security center management async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.SecurityCenterManagementTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,SecurityCenterManagementTransport,Callable[..., SecurityCenterManagementTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the SecurityCenterManagementTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -339,20 +354,20 @@
 
         Args:
             request (Optional[Union[google.cloud.securitycentermanagement_v1.types.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest, dict]]):
                 The request object. Request message for listing effective
                 Security Health Analytics custom
                 modules.
             parent (:class:`str`):
-                Required. Name of parent to list
-                effective custom modules. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of parent to list effective custom
+                modules. specified in one of the following formats:
+
+                -  ``organizations/{organization}/locations/{location}``
+                -  ``folders/{folder}/locations/{location}`` or
+                   ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -367,49 +382,43 @@
 
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
 
-        request = security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest(
-            request
-        )
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest,
+        ):
+            request = security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest(
+                request
+            )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_effective_security_health_analytics_custom_modules,
-            default_retry=retries.AsyncRetry(
-                initial=0.1,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_effective_security_health_analytics_custom_modules
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -480,21 +489,20 @@
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.securitycentermanagement_v1.types.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest, dict]]):
                 The request object. Message for getting a
                 EffectiveSecurityHealthAnalyticsCustomModule
             name (:class:`str`):
-                Required. The resource name of the SHA custom module.
-
-                Its format is:
+                Required. The full resource name of the custom module,
+                specified in one of the following formats:
 
-                -  "organizations/{organization}/locations/{location}/effectiveSecurityHealthAnalyticsCustomModules/{module_id}".
-                -  "folders/{folder}/locations/{location}/effectiveSecurityHealthAnalyticsCustomModules/{module_id}".
-                -  "projects/{project}/locations/{location}/effectiveSecurityHealthAnalyticsCustomModules/{module_id}".
+                -  ``organizations/organization/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}``
+                -  ``folders/folder/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}``
+                -  ``projects/project/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}``
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -516,49 +524,43 @@
                    enablement_state for the module in all child folders
                    or projects is also enabled.
                    EffectiveSecurityHealthAnalyticsCustomModule is
                    read-only.
 
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
 
-        request = security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest(
-            request
-        )
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest,
+        ):
+            request = security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest(
+                request
+            )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_effective_security_health_analytics_custom_module,
-            default_retry=retries.AsyncRetry(
-                initial=0.1,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_effective_security_health_analytics_custom_module
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -624,20 +626,21 @@
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.securitycentermanagement_v1.types.ListSecurityHealthAnalyticsCustomModulesRequest, dict]]):
                 The request object. Request message for listing Security
                 Health Analytics custom modules.
             parent (:class:`str`):
-                Required. Name of parent to list
-                custom modules. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of parent organization, folder, or
+                project in which to list custom modules, specified in
+                one of the following formats:
+
+                -  ``organizations/{organization}/locations/{location}``
+                -  ``folders/{folder}/locations/{location}``
+                -  ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -650,51 +653,43 @@
                 Health Analytics custom modules.
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
 
-        request = (
-            security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest(
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest,
+        ):
+            request = security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest(
                 request
             )
-        )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_security_health_analytics_custom_modules,
-            default_retry=retries.AsyncRetry(
-                initial=0.1,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_security_health_analytics_custom_modules
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -768,20 +763,21 @@
 
         Args:
             request (Optional[Union[google.cloud.securitycentermanagement_v1.types.ListDescendantSecurityHealthAnalyticsCustomModulesRequest, dict]]):
                 The request object. Request message for listing
                 descendant Security Health Analytics
                 custom modules.
             parent (:class:`str`):
-                Required. Name of parent to list
-                custom modules. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of the parent organization, folder, or
+                project in which to list custom modules, specified in
+                one of the following formats:
+
+                -  ``organizations/{organization}/locations/{location}``
+                -  ``folders/{folder}/locations/{location}``
+                -  ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -796,49 +792,43 @@
 
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
 
-        request = security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest(
-            request
-        )
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest,
+        ):
+            request = security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest(
+                request
+            )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_descendant_security_health_analytics_custom_modules,
-            default_retry=retries.AsyncRetry(
-                initial=0.1,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_descendant_security_health_analytics_custom_modules
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -933,51 +923,43 @@
                 level. Custom modules that you create at
                 the organization or folder level are
                 inherited by the child folders and
                 projects.
 
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
 
-        request = (
-            security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest(
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest,
+        ):
+            request = security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest(
                 request
             )
-        )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_security_health_analytics_custom_module,
-            default_retry=retries.AsyncRetry(
-                initial=0.1,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_security_health_analytics_custom_module
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -1046,20 +1028,21 @@
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.securitycentermanagement_v1.types.CreateSecurityHealthAnalyticsCustomModuleRequest, dict]]):
                 The request object. Message for creating a
                 SecurityHealthAnalyticsCustomModule
             parent (:class:`str`):
-                Required. Name of the parent for the
-                module. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of the parent organization, folder, or
+                project of the module, specified in one of the following
+                formats:
+
+                -  ``organizations/{organization}/locations/{location}``
+                -  ``folders/{folder}/locations/{location}``
+                -  ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             security_health_analytics_custom_module (:class:`google.cloud.securitycentermanagement_v1.types.SecurityHealthAnalyticsCustomModule`):
                 Required. The resource being created
                 This corresponds to the ``security_health_analytics_custom_module`` field
@@ -1082,45 +1065,47 @@
                 level. Custom modules that you create at
                 the organization or folder level are
                 inherited by the child folders and
                 projects.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, security_health_analytics_custom_module])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = (
-            security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest(
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest,
+        ):
+            request = security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest(
                 request
             )
-        )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if security_health_analytics_custom_module is not None:
             request.security_health_analytics_custom_module = (
                 security_health_analytics_custom_module
             )
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_security_health_analytics_custom_module,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_security_health_analytics_custom_module
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -1224,47 +1209,49 @@
                 level. Custom modules that you create at
                 the organization or folder level are
                 inherited by the child folders and
                 projects.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any(
             [security_health_analytics_custom_module, update_mask]
         )
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = (
-            security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest(
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest,
+        ):
+            request = security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest(
                 request
             )
-        )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if security_health_analytics_custom_module is not None:
             request.security_health_analytics_custom_module = (
                 security_health_analytics_custom_module
             )
         if update_mask is not None:
             request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_security_health_analytics_custom_module,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_security_health_analytics_custom_module
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (
                     (
@@ -1336,55 +1323,57 @@
                 The request object. Message for deleting a
                 SecurityHealthAnalyticsCustomModule
             name (:class:`str`):
                 Required. The resource name of the SHA custom module.
 
                 Its format is:
 
-                -  "organizations/{organization}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}".
-                -  "folders/{folder}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}".
-                -  "projects/{project}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}".
+                -  ``organizations/{organization}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}``.
+                -  ``folders/{folder}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}``.
+                -  ``projects/{project}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
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
 
-        request = (
-            security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest(
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest,
+        ):
+            request = security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest(
                 request
             )
-        )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_security_health_analytics_custom_module,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_security_health_analytics_custom_module
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -1489,53 +1478,47 @@
         Returns:
             google.cloud.securitycentermanagement_v1.types.SimulateSecurityHealthAnalyticsCustomModuleResponse:
                 Response message for simulating a SecurityHealthAnalyticsCustomModule
                    against a given resource.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, custom_config, resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest(
-            request
-        )
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest,
+        ):
+            request = security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest(
+                request
+            )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if custom_config is not None:
             request.custom_config = custom_config
         if resource is not None:
             request.resource = resource
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.simulate_security_health_analytics_custom_module,
-            default_retry=retries.AsyncRetry(
-                initial=0.1,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.simulate_security_health_analytics_custom_module
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -1600,20 +1583,19 @@
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.securitycentermanagement_v1.types.ListEffectiveEventThreatDetectionCustomModulesRequest, dict]]):
                 The request object. Request message for listing effective
                 Event Threat Detection custom modules.
             parent (:class:`str`):
-                Required. Name of parent to list
-                effective custom modules. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of parent to list effective custom
+                modules. Its format is
+                ``organizations/{organization}/locations/{location}``,
+                ``folders/{folder}/locations/{location}``, or
+                ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1628,49 +1610,43 @@
 
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
 
-        request = security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest(
-            request
-        )
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest,
+        ):
+            request = security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest(
+                request
+            )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_effective_event_threat_detection_custom_modules,
-            default_retry=retries.AsyncRetry(
-                initial=0.1,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_effective_event_threat_detection_custom_modules
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -1751,17 +1727,17 @@
                 The request object. Message for getting a
                 EffectiveEventThreatDetectionCustomModule
             name (:class:`str`):
                 Required. The resource name of the ETD custom module.
 
                 Its format is:
 
-                -  "organizations/{organization}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}".
-                -  "folders/{folder}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}".
-                -  "projects/{project}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}".
+                -  ``organizations/{organization}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}``.
+                -  ``folders/{folder}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}``.
+                -  ``projects/{project}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1780,49 +1756,43 @@
                    effective module's config will contain the ancestor's
                    config details.
                    EffectiveEventThreatDetectionCustomModule is
                    read-only.
 
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
 
-        request = security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest(
-            request
-        )
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest,
+        ):
+            request = security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest(
+                request
+            )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_effective_event_threat_detection_custom_module,
-            default_retry=retries.AsyncRetry(
-                initial=0.1,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_effective_event_threat_detection_custom_module
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -1887,20 +1857,19 @@
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.securitycentermanagement_v1.types.ListEventThreatDetectionCustomModulesRequest, dict]]):
                 The request object. Request message for listing Event
                 Threat Detection custom modules.
             parent (:class:`str`):
-                Required. Name of parent to list
-                custom modules. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of parent to list custom modules. Its
+                format is
+                ``organizations/{organization}/locations/{location}``,
+                ``folders/{folder}/locations/{location}``, or
+                ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1913,51 +1882,45 @@
                 Threat Detection custom modules.
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
 
-        request = (
-            security_center_management.ListEventThreatDetectionCustomModulesRequest(
-                request
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.ListEventThreatDetectionCustomModulesRequest,
+        ):
+            request = (
+                security_center_management.ListEventThreatDetectionCustomModulesRequest(
+                    request
+                )
             )
-        )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_event_threat_detection_custom_modules,
-            default_retry=retries.AsyncRetry(
-                initial=0.1,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_event_threat_detection_custom_modules
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -2031,20 +1994,19 @@
 
         Args:
             request (Optional[Union[google.cloud.securitycentermanagement_v1.types.ListDescendantEventThreatDetectionCustomModulesRequest, dict]]):
                 The request object. Request message for listing
                 descendant Event Threat Detection custom
                 modules.
             parent (:class:`str`):
-                Required. Name of parent to list
-                custom modules. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of parent to list custom modules. Its
+                format is
+                ``organizations/{organization}/locations/{location}``,
+                ``folders/{folder}/locations/{location}``, or
+                ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -2059,49 +2021,43 @@
 
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
 
-        request = security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest(
-            request
-        )
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest,
+        ):
+            request = security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest(
+                request
+            )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_descendant_event_threat_detection_custom_modules,
-            default_retry=retries.AsyncRetry(
-                initial=0.1,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_descendant_event_threat_detection_custom_modules
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -2175,17 +2131,17 @@
                 The request object. Message for getting a
                 EventThreatDetectionCustomModule
             name (:class:`str`):
                 Required. The resource name of the ETD custom module.
 
                 Its format is:
 
-                -  "organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-                -  "folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-                -  "projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
+                -  ``organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+                -  ``folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+                -  ``projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -2199,49 +2155,45 @@
                 contains the configuration and
                 enablement state of a custom module,
                 which enables ETD to write certain
                 findings to Cloud SCC.
 
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
 
-        request = security_center_management.GetEventThreatDetectionCustomModuleRequest(
-            request
-        )
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.GetEventThreatDetectionCustomModuleRequest,
+        ):
+            request = (
+                security_center_management.GetEventThreatDetectionCustomModuleRequest(
+                    request
+                )
+            )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_event_threat_detection_custom_module,
-            default_retry=retries.AsyncRetry(
-                initial=0.1,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_event_threat_detection_custom_module
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -2309,20 +2261,18 @@
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.securitycentermanagement_v1.types.CreateEventThreatDetectionCustomModuleRequest, dict]]):
                 The request object. Message for creating a
                 EventThreatDetectionCustomModule
             parent (:class:`str`):
-                Required. Name of parent for the
-                module. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of parent for the module. Its format is
+                ``organizations/{organization}/locations/{location}``,
+                ``folders/{folder}/locations/{location}``, or
+                ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             event_threat_detection_custom_module (:class:`google.cloud.securitycentermanagement_v1.types.EventThreatDetectionCustomModule`):
                 Required. The module to create. The
                 event_threat_detection_custom_module.name will be
@@ -2344,45 +2294,47 @@
                 contains the configuration and
                 enablement state of a custom module,
                 which enables ETD to write certain
                 findings to Cloud SCC.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, event_threat_detection_custom_module])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = (
-            security_center_management.CreateEventThreatDetectionCustomModuleRequest(
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.CreateEventThreatDetectionCustomModuleRequest,
+        ):
+            request = security_center_management.CreateEventThreatDetectionCustomModuleRequest(
                 request
             )
-        )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if event_threat_detection_custom_module is not None:
             request.event_threat_detection_custom_module = (
                 event_threat_detection_custom_module
             )
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_event_threat_detection_custom_module,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_event_threat_detection_custom_module
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -2485,45 +2437,47 @@
                 contains the configuration and
                 enablement state of a custom module,
                 which enables ETD to write certain
                 findings to Cloud SCC.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([event_threat_detection_custom_module, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = (
-            security_center_management.UpdateEventThreatDetectionCustomModuleRequest(
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.UpdateEventThreatDetectionCustomModuleRequest,
+        ):
+            request = security_center_management.UpdateEventThreatDetectionCustomModuleRequest(
                 request
             )
-        )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if event_threat_detection_custom_module is not None:
             request.event_threat_detection_custom_module = (
                 event_threat_detection_custom_module
             )
         if update_mask is not None:
             request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_event_threat_detection_custom_module,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_event_threat_detection_custom_module
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (
                     (
@@ -2595,55 +2549,57 @@
                 The request object. Message for deleting a
                 EventThreatDetectionCustomModule
             name (:class:`str`):
                 Required. The resource name of the ETD custom module.
 
                 Its format is:
 
-                -  "organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-                -  "folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-                -  "projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
+                -  ``organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+                -  ``folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+                -  ``projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
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
 
-        request = (
-            security_center_management.DeleteEventThreatDetectionCustomModuleRequest(
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.DeleteEventThreatDetectionCustomModuleRequest,
+        ):
+            request = security_center_management.DeleteEventThreatDetectionCustomModuleRequest(
                 request
             )
-        )
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_event_threat_detection_custom_module,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_event_threat_detection_custom_module
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -2715,49 +2671,448 @@
         Returns:
             google.cloud.securitycentermanagement_v1.types.ValidateEventThreatDetectionCustomModuleResponse:
                 Response to validating an Event
                 Threat Detection custom module.
 
         """
         # Create or coerce a protobuf request object.
-        request = (
-            security_center_management.ValidateEventThreatDetectionCustomModuleRequest(
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request,
+            security_center_management.ValidateEventThreatDetectionCustomModuleRequest,
+        ):
+            request = security_center_management.ValidateEventThreatDetectionCustomModuleRequest(
                 request
             )
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.validate_event_threat_detection_custom_module
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Validate the universe domain.
+        self._client._validate_universe_domain()
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
+        # Done; return the response.
+        return response
+
+    async def get_security_center_service(
+        self,
+        request: Optional[
+            Union[security_center_management.GetSecurityCenterServiceRequest, dict]
+        ] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> security_center_management.SecurityCenterService:
+        r"""Gets service settings for the specified Security
+        Command Center service.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import securitycentermanagement_v1
+
+            async def sample_get_security_center_service():
+                # Create a client
+                client = securitycentermanagement_v1.SecurityCenterManagementAsyncClient()
+
+                # Initialize request argument(s)
+                request = securitycentermanagement_v1.GetSecurityCenterServiceRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = await client.get_security_center_service(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.securitycentermanagement_v1.types.GetSecurityCenterServiceRequest, dict]]):
+                The request object. Request message for getting a
+                Security Command Center service.
+            name (:class:`str`):
+                Required. The Security Command Center service to
+                retrieve.
+
+                Formats:
+
+                -  organizations/{organization}/locations/{location}/securityCenterServices/{service}
+                -  folders/{folder}/locations/{location}/securityCenterServices/{service}
+                -  projects/{project}/locations/{location}/securityCenterServices/{service}
+
+                The possible values for id {service} are:
+
+                -  container-threat-detection
+                -  event-threat-detection
+                -  security-health-analytics
+                -  vm-threat-detection
+                -  web-security-scanner
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.securitycentermanagement_v1.types.SecurityCenterService:
+                Represents a particular Security
+                Command Center service. This includes
+                settings information such as top-level
+                enablement in addition to individual
+                module settings. Service settings can be
+                configured at the organization, folder,
+                or project level. Service settings at
+                the organization or folder level are
+                inherited by those in child folders and
+                projects.
+
+        """
+        # Create or coerce a protobuf request object.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request, security_center_management.GetSecurityCenterServiceRequest
+        ):
+            request = security_center_management.GetSecurityCenterServiceRequest(
+                request
+            )
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if name is not None:
+            request.name = name
+
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.validate_event_threat_detection_custom_module,
-            default_retry=retries.AsyncRetry(
-                initial=0.1,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.DeadlineExceeded,
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_security_center_service
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Validate the universe domain.
+        self._client._validate_universe_domain()
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
+        # Done; return the response.
+        return response
+
+    async def list_security_center_services(
+        self,
+        request: Optional[
+            Union[security_center_management.ListSecurityCenterServicesRequest, dict]
+        ] = None,
+        *,
+        parent: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> pagers.ListSecurityCenterServicesAsyncPager:
+        r"""Returns a list of all Security Command Center
+        services for the given parent.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import securitycentermanagement_v1
+
+            async def sample_list_security_center_services():
+                # Create a client
+                client = securitycentermanagement_v1.SecurityCenterManagementAsyncClient()
+
+                # Initialize request argument(s)
+                request = securitycentermanagement_v1.ListSecurityCenterServicesRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_security_center_services(request=request)
+
+                # Handle the response
+                async for response in page_result:
+                    print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.securitycentermanagement_v1.types.ListSecurityCenterServicesRequest, dict]]):
+                The request object. Request message for listing Security
+                Command Center services.
+            parent (:class:`str`):
+                Required. The name of the parent to list Security
+                Command Center services.
+
+                Formats:
+
+                -  organizations/{organization}/locations/{location}
+                -  folders/{folder}/locations/{location}
+                -  projects/{project}/locations/{location}
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.securitycentermanagement_v1.services.security_center_management.pagers.ListSecurityCenterServicesAsyncPager:
+                Response message for listing Security
+                Command Center services.
+                Iterating over this object will yield
+                results and resolve additional pages
+                automatically.
+
+        """
+        # Create or coerce a protobuf request object.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request, security_center_management.ListSecurityCenterServicesRequest
+        ):
+            request = security_center_management.ListSecurityCenterServicesRequest(
+                request
+            )
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if parent is not None:
+            request.parent = parent
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_security_center_services
+        ]
+
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Validate the universe domain.
         self._client._validate_universe_domain()
 
         # Send the request.
         response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # This method is paged; wrap the response in a pager, which provides
+        # an `__aiter__` convenience method.
+        response = pagers.ListSecurityCenterServicesAsyncPager(
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def update_security_center_service(
+        self,
+        request: Optional[
+            Union[security_center_management.UpdateSecurityCenterServiceRequest, dict]
+        ] = None,
+        *,
+        security_center_service: Optional[
+            security_center_management.SecurityCenterService
+        ] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> security_center_management.SecurityCenterService:
+        r"""Updates a Security Command Center service using the
+        given update mask.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import securitycentermanagement_v1
+
+            async def sample_update_security_center_service():
+                # Create a client
+                client = securitycentermanagement_v1.SecurityCenterManagementAsyncClient()
+
+                # Initialize request argument(s)
+                request = securitycentermanagement_v1.UpdateSecurityCenterServiceRequest(
+                )
+
+                # Make the request
+                response = await client.update_security_center_service(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.securitycentermanagement_v1.types.UpdateSecurityCenterServiceRequest, dict]]):
+                The request object. Request message for updating a
+                Security Command Center service.
+            security_center_service (:class:`google.cloud.securitycentermanagement_v1.types.SecurityCenterService`):
+                Required. The updated service.
+                This corresponds to the ``security_center_service`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
+                Required. The list of fields to be updated. Possible
+                values:
+
+                -  "intended_enablement_state"
+                -  "modules"
+
+                This corresponds to the ``update_mask`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.securitycentermanagement_v1.types.SecurityCenterService:
+                Represents a particular Security
+                Command Center service. This includes
+                settings information such as top-level
+                enablement in addition to individual
+                module settings. Service settings can be
+                configured at the organization, folder,
+                or project level. Service settings at
+                the organization or folder level are
+                inherited by those in child folders and
+                projects.
+
+        """
+        # Create or coerce a protobuf request object.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
+        has_flattened_params = any([security_center_service, update_mask])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request, security_center_management.UpdateSecurityCenterServiceRequest
+        ):
+            request = security_center_management.UpdateSecurityCenterServiceRequest(
+                request
+            )
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if security_center_service is not None:
+            request.security_center_service = security_center_service
+        if update_mask is not None:
+            request.update_mask = update_mask
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_security_center_service
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (
+                    (
+                        "security_center_service.name",
+                        request.security_center_service.name,
+                    ),
+                )
+            ),
+        )
+
+        # Validate the universe domain.
+        self._client._validate_universe_domain()
+
+        # Send the request.
+        response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/client.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/client.py`

 * *Files 7% similar despite different names*

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
@@ -280,14 +281,36 @@
         m = re.match(
             r"^organizations/(?P<organization>.+?)/sources/(?P<source>.+?)/findings/(?P<finding>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
+    def security_center_service_path(
+        project: str,
+        location: str,
+        service: str,
+    ) -> str:
+        """Returns a fully-qualified security_center_service string."""
+        return "projects/{project}/locations/{location}/securityCenterServices/{service}".format(
+            project=project,
+            location=location,
+            service=service,
+        )
+
+    @staticmethod
+    def parse_security_center_service_path(path: str) -> Dict[str, str]:
+        """Parses a security_center_service path into its component segments."""
+        m = re.match(
+            r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)/securityCenterServices/(?P<service>.+?)$",
+            path,
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
     def security_health_analytics_custom_module_path(
         organization: str,
         location: str,
         security_health_analytics_custom_module: str,
     ) -> str:
         """Returns a fully-qualified security_health_analytics_custom_module string."""
         return "organizations/{organization}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}".format(
@@ -628,29 +651,37 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, SecurityCenterManagementTransport]] = None,
+        transport: Optional[
+            Union[
+                str,
+                SecurityCenterManagementTransport,
+                Callable[..., SecurityCenterManagementTransport],
+            ]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the security center management client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, SecurityCenterManagementTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,SecurityCenterManagementTransport,Callable[..., SecurityCenterManagementTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the SecurityCenterManagementTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -753,16 +784,24 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[SecurityCenterManagementTransport],
+                Callable[..., SecurityCenterManagementTransport],
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., SecurityCenterManagementTransport], transport)
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
@@ -819,20 +858,20 @@
 
         Args:
             request (Union[google.cloud.securitycentermanagement_v1.types.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest, dict]):
                 The request object. Request message for listing effective
                 Security Health Analytics custom
                 modules.
             parent (str):
-                Required. Name of parent to list
-                effective custom modules. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of parent to list effective custom
+                modules. specified in one of the following formats:
+
+                -  ``organizations/{organization}/locations/{location}``
+                -  ``folders/{folder}/locations/{location}`` or
+                   ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -847,27 +886,25 @@
 
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
-        # in a security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest,
         ):
             request = security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest(
                 request
             )
@@ -955,21 +992,20 @@
                 print(response)
 
         Args:
             request (Union[google.cloud.securitycentermanagement_v1.types.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest, dict]):
                 The request object. Message for getting a
                 EffectiveSecurityHealthAnalyticsCustomModule
             name (str):
-                Required. The resource name of the SHA custom module.
-
-                Its format is:
+                Required. The full resource name of the custom module,
+                specified in one of the following formats:
 
-                -  "organizations/{organization}/locations/{location}/effectiveSecurityHealthAnalyticsCustomModules/{module_id}".
-                -  "folders/{folder}/locations/{location}/effectiveSecurityHealthAnalyticsCustomModules/{module_id}".
-                -  "projects/{project}/locations/{location}/effectiveSecurityHealthAnalyticsCustomModules/{module_id}".
+                -  ``organizations/organization/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}``
+                -  ``folders/folder/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}``
+                -  ``projects/project/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}``
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -991,27 +1027,25 @@
                    enablement_state for the module in all child folders
                    or projects is also enabled.
                    EffectiveSecurityHealthAnalyticsCustomModule is
                    read-only.
 
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
-        # in a security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest,
         ):
             request = security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest(
                 request
             )
@@ -1094,20 +1128,21 @@
                     print(response)
 
         Args:
             request (Union[google.cloud.securitycentermanagement_v1.types.ListSecurityHealthAnalyticsCustomModulesRequest, dict]):
                 The request object. Request message for listing Security
                 Health Analytics custom modules.
             parent (str):
-                Required. Name of parent to list
-                custom modules. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of parent organization, folder, or
+                project in which to list custom modules, specified in
+                one of the following formats:
+
+                -  ``organizations/{organization}/locations/{location}``
+                -  ``folders/{folder}/locations/{location}``
+                -  ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1120,27 +1155,25 @@
                 Health Analytics custom modules.
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
-        # in a security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest,
         ):
             request = security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest(
                 request
             )
@@ -1231,20 +1264,21 @@
 
         Args:
             request (Union[google.cloud.securitycentermanagement_v1.types.ListDescendantSecurityHealthAnalyticsCustomModulesRequest, dict]):
                 The request object. Request message for listing
                 descendant Security Health Analytics
                 custom modules.
             parent (str):
-                Required. Name of parent to list
-                custom modules. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of the parent organization, folder, or
+                project in which to list custom modules, specified in
+                one of the following formats:
+
+                -  ``organizations/{organization}/locations/{location}``
+                -  ``folders/{folder}/locations/{location}``
+                -  ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1259,27 +1293,25 @@
 
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
-        # in a security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest,
         ):
             request = security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest(
                 request
             )
@@ -1391,27 +1423,25 @@
                 level. Custom modules that you create at
                 the organization or folder level are
                 inherited by the child folders and
                 projects.
 
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
-        # in a security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest,
         ):
             request = security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest(
                 request
             )
@@ -1497,20 +1527,21 @@
                 print(response)
 
         Args:
             request (Union[google.cloud.securitycentermanagement_v1.types.CreateSecurityHealthAnalyticsCustomModuleRequest, dict]):
                 The request object. Message for creating a
                 SecurityHealthAnalyticsCustomModule
             parent (str):
-                Required. Name of the parent for the
-                module. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of the parent organization, folder, or
+                project of the module, specified in one of the following
+                formats:
+
+                -  ``organizations/{organization}/locations/{location}``
+                -  ``folders/{folder}/locations/{location}``
+                -  ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             security_health_analytics_custom_module (google.cloud.securitycentermanagement_v1.types.SecurityHealthAnalyticsCustomModule):
                 Required. The resource being created
                 This corresponds to the ``security_health_analytics_custom_module`` field
@@ -1533,27 +1564,25 @@
                 level. Custom modules that you create at
                 the organization or folder level are
                 inherited by the child folders and
                 projects.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, security_health_analytics_custom_module])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest,
         ):
             request = security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest(
                 request
             )
@@ -1678,29 +1707,27 @@
                 level. Custom modules that you create at
                 the organization or folder level are
                 inherited by the child folders and
                 projects.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any(
             [security_health_analytics_custom_module, update_mask]
         )
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest,
         ):
             request = security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest(
                 request
             )
@@ -1793,41 +1820,39 @@
                 The request object. Message for deleting a
                 SecurityHealthAnalyticsCustomModule
             name (str):
                 Required. The resource name of the SHA custom module.
 
                 Its format is:
 
-                -  "organizations/{organization}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}".
-                -  "folders/{folder}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}".
-                -  "projects/{project}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}".
+                -  ``organizations/{organization}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}``.
+                -  ``folders/{folder}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}``.
+                -  ``projects/{project}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
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
-        # in a security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest,
         ):
             request = security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest(
                 request
             )
@@ -1949,27 +1974,25 @@
         Returns:
             google.cloud.securitycentermanagement_v1.types.SimulateSecurityHealthAnalyticsCustomModuleResponse:
                 Response message for simulating a SecurityHealthAnalyticsCustomModule
                    against a given resource.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, custom_config, resource])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest,
         ):
             request = security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest(
                 request
             )
@@ -2055,20 +2078,19 @@
                     print(response)
 
         Args:
             request (Union[google.cloud.securitycentermanagement_v1.types.ListEffectiveEventThreatDetectionCustomModulesRequest, dict]):
                 The request object. Request message for listing effective
                 Event Threat Detection custom modules.
             parent (str):
-                Required. Name of parent to list
-                effective custom modules. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of parent to list effective custom
+                modules. Its format is
+                ``organizations/{organization}/locations/{location}``,
+                ``folders/{folder}/locations/{location}``, or
+                ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -2083,27 +2105,25 @@
 
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
-        # in a security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest,
         ):
             request = security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest(
                 request
             )
@@ -2201,17 +2221,17 @@
                 The request object. Message for getting a
                 EffectiveEventThreatDetectionCustomModule
             name (str):
                 Required. The resource name of the ETD custom module.
 
                 Its format is:
 
-                -  "organizations/{organization}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}".
-                -  "folders/{folder}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}".
-                -  "projects/{project}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}".
+                -  ``organizations/{organization}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}``.
+                -  ``folders/{folder}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}``.
+                -  ``projects/{project}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -2230,27 +2250,25 @@
                    effective module's config will contain the ancestor's
                    config details.
                    EffectiveEventThreatDetectionCustomModule is
                    read-only.
 
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
-        # in a security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest,
         ):
             request = security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest(
                 request
             )
@@ -2332,20 +2350,19 @@
                     print(response)
 
         Args:
             request (Union[google.cloud.securitycentermanagement_v1.types.ListEventThreatDetectionCustomModulesRequest, dict]):
                 The request object. Request message for listing Event
                 Threat Detection custom modules.
             parent (str):
-                Required. Name of parent to list
-                custom modules. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of parent to list custom modules. Its
+                format is
+                ``organizations/{organization}/locations/{location}``,
+                ``folders/{folder}/locations/{location}``, or
+                ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -2358,27 +2375,25 @@
                 Threat Detection custom modules.
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
-        # in a security_center_management.ListEventThreatDetectionCustomModulesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.ListEventThreatDetectionCustomModulesRequest,
         ):
             request = (
                 security_center_management.ListEventThreatDetectionCustomModulesRequest(
                     request
@@ -2471,20 +2486,19 @@
 
         Args:
             request (Union[google.cloud.securitycentermanagement_v1.types.ListDescendantEventThreatDetectionCustomModulesRequest, dict]):
                 The request object. Request message for listing
                 descendant Event Threat Detection custom
                 modules.
             parent (str):
-                Required. Name of parent to list
-                custom modules. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of parent to list custom modules. Its
+                format is
+                ``organizations/{organization}/locations/{location}``,
+                ``folders/{folder}/locations/{location}``, or
+                ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -2499,27 +2513,25 @@
 
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
-        # in a security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest,
         ):
             request = security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest(
                 request
             )
@@ -2610,17 +2622,17 @@
                 The request object. Message for getting a
                 EventThreatDetectionCustomModule
             name (str):
                 Required. The resource name of the ETD custom module.
 
                 Its format is:
 
-                -  "organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-                -  "folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-                -  "projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
+                -  ``organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+                -  ``folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+                -  ``projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -2634,27 +2646,25 @@
                 contains the configuration and
                 enablement state of a custom module,
                 which enables ETD to write certain
                 findings to Cloud SCC.
 
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
-        # in a security_center_management.GetEventThreatDetectionCustomModuleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.GetEventThreatDetectionCustomModuleRequest,
         ):
             request = (
                 security_center_management.GetEventThreatDetectionCustomModuleRequest(
                     request
@@ -2741,20 +2751,18 @@
                 print(response)
 
         Args:
             request (Union[google.cloud.securitycentermanagement_v1.types.CreateEventThreatDetectionCustomModuleRequest, dict]):
                 The request object. Message for creating a
                 EventThreatDetectionCustomModule
             parent (str):
-                Required. Name of parent for the
-                module. Its format is
-                "organizations/{organization}/locations/{location}",
-                "folders/{folder}/locations/{location}",
-                or
-                "projects/{project}/locations/{location}"
+                Required. Name of parent for the module. Its format is
+                ``organizations/{organization}/locations/{location}``,
+                ``folders/{folder}/locations/{location}``, or
+                ``projects/{project}/locations/{location}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             event_threat_detection_custom_module (google.cloud.securitycentermanagement_v1.types.EventThreatDetectionCustomModule):
                 Required. The module to create. The
                 event_threat_detection_custom_module.name will be
@@ -2776,27 +2784,25 @@
                 contains the configuration and
                 enablement state of a custom module,
                 which enables ETD to write certain
                 findings to Cloud SCC.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, event_threat_detection_custom_module])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a security_center_management.CreateEventThreatDetectionCustomModuleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.CreateEventThreatDetectionCustomModuleRequest,
         ):
             request = security_center_management.CreateEventThreatDetectionCustomModuleRequest(
                 request
             )
@@ -2920,27 +2926,25 @@
                 contains the configuration and
                 enablement state of a custom module,
                 which enables ETD to write certain
                 findings to Cloud SCC.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([event_threat_detection_custom_module, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a security_center_management.UpdateEventThreatDetectionCustomModuleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.UpdateEventThreatDetectionCustomModuleRequest,
         ):
             request = security_center_management.UpdateEventThreatDetectionCustomModuleRequest(
                 request
             )
@@ -3033,41 +3037,39 @@
                 The request object. Message for deleting a
                 EventThreatDetectionCustomModule
             name (str):
                 Required. The resource name of the ETD custom module.
 
                 Its format is:
 
-                -  "organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-                -  "folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-                -  "projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
+                -  ``organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+                -  ``folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+                -  ``projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
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
-        # in a security_center_management.DeleteEventThreatDetectionCustomModuleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.DeleteEventThreatDetectionCustomModuleRequest,
         ):
             request = security_center_management.DeleteEventThreatDetectionCustomModuleRequest(
                 request
             )
@@ -3156,18 +3158,16 @@
         Returns:
             google.cloud.securitycentermanagement_v1.types.ValidateEventThreatDetectionCustomModuleResponse:
                 Response to validating an Event
                 Threat Detection custom module.
 
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a security_center_management.ValidateEventThreatDetectionCustomModuleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(
             request,
             security_center_management.ValidateEventThreatDetectionCustomModuleRequest,
         ):
             request = security_center_management.ValidateEventThreatDetectionCustomModuleRequest(
                 request
             )
@@ -3185,14 +3185,418 @@
         )
 
         # Validate the universe domain.
         self._validate_universe_domain()
 
         # Send the request.
         response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def get_security_center_service(
+        self,
+        request: Optional[
+            Union[security_center_management.GetSecurityCenterServiceRequest, dict]
+        ] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> security_center_management.SecurityCenterService:
+        r"""Gets service settings for the specified Security
+        Command Center service.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import securitycentermanagement_v1
+
+            def sample_get_security_center_service():
+                # Create a client
+                client = securitycentermanagement_v1.SecurityCenterManagementClient()
+
+                # Initialize request argument(s)
+                request = securitycentermanagement_v1.GetSecurityCenterServiceRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_security_center_service(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.securitycentermanagement_v1.types.GetSecurityCenterServiceRequest, dict]):
+                The request object. Request message for getting a
+                Security Command Center service.
+            name (str):
+                Required. The Security Command Center service to
+                retrieve.
+
+                Formats:
+
+                -  organizations/{organization}/locations/{location}/securityCenterServices/{service}
+                -  folders/{folder}/locations/{location}/securityCenterServices/{service}
+                -  projects/{project}/locations/{location}/securityCenterServices/{service}
+
+                The possible values for id {service} are:
+
+                -  container-threat-detection
+                -  event-threat-detection
+                -  security-health-analytics
+                -  vm-threat-detection
+                -  web-security-scanner
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.securitycentermanagement_v1.types.SecurityCenterService:
+                Represents a particular Security
+                Command Center service. This includes
+                settings information such as top-level
+                enablement in addition to individual
+                module settings. Service settings can be
+                configured at the organization, folder,
+                or project level. Service settings at
+                the organization or folder level are
+                inherited by those in child folders and
+                projects.
+
+        """
+        # Create or coerce a protobuf request object.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request, security_center_management.GetSecurityCenterServiceRequest
+        ):
+            request = security_center_management.GetSecurityCenterServiceRequest(
+                request
+            )
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[
+            self._transport.get_security_center_service
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Validate the universe domain.
+        self._validate_universe_domain()
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def list_security_center_services(
+        self,
+        request: Optional[
+            Union[security_center_management.ListSecurityCenterServicesRequest, dict]
+        ] = None,
+        *,
+        parent: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> pagers.ListSecurityCenterServicesPager:
+        r"""Returns a list of all Security Command Center
+        services for the given parent.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import securitycentermanagement_v1
+
+            def sample_list_security_center_services():
+                # Create a client
+                client = securitycentermanagement_v1.SecurityCenterManagementClient()
+
+                # Initialize request argument(s)
+                request = securitycentermanagement_v1.ListSecurityCenterServicesRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_security_center_services(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
+        Args:
+            request (Union[google.cloud.securitycentermanagement_v1.types.ListSecurityCenterServicesRequest, dict]):
+                The request object. Request message for listing Security
+                Command Center services.
+            parent (str):
+                Required. The name of the parent to list Security
+                Command Center services.
+
+                Formats:
+
+                -  organizations/{organization}/locations/{location}
+                -  folders/{folder}/locations/{location}
+                -  projects/{project}/locations/{location}
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.securitycentermanagement_v1.services.security_center_management.pagers.ListSecurityCenterServicesPager:
+                Response message for listing Security
+                Command Center services.
+                Iterating over this object will yield
+                results and resolve additional pages
+                automatically.
+
+        """
+        # Create or coerce a protobuf request object.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request, security_center_management.ListSecurityCenterServicesRequest
+        ):
+            request = security_center_management.ListSecurityCenterServicesRequest(
+                request
+            )
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[
+            self._transport.list_security_center_services
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Validate the universe domain.
+        self._validate_universe_domain()
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # This method is paged; wrap the response in a pager, which provides
+        # an `__iter__` convenience method.
+        response = pagers.ListSecurityCenterServicesPager(
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def update_security_center_service(
+        self,
+        request: Optional[
+            Union[security_center_management.UpdateSecurityCenterServiceRequest, dict]
+        ] = None,
+        *,
+        security_center_service: Optional[
+            security_center_management.SecurityCenterService
+        ] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> security_center_management.SecurityCenterService:
+        r"""Updates a Security Command Center service using the
+        given update mask.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import securitycentermanagement_v1
+
+            def sample_update_security_center_service():
+                # Create a client
+                client = securitycentermanagement_v1.SecurityCenterManagementClient()
+
+                # Initialize request argument(s)
+                request = securitycentermanagement_v1.UpdateSecurityCenterServiceRequest(
+                )
+
+                # Make the request
+                response = client.update_security_center_service(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.securitycentermanagement_v1.types.UpdateSecurityCenterServiceRequest, dict]):
+                The request object. Request message for updating a
+                Security Command Center service.
+            security_center_service (google.cloud.securitycentermanagement_v1.types.SecurityCenterService):
+                Required. The updated service.
+                This corresponds to the ``security_center_service`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            update_mask (google.protobuf.field_mask_pb2.FieldMask):
+                Required. The list of fields to be updated. Possible
+                values:
+
+                -  "intended_enablement_state"
+                -  "modules"
+
+                This corresponds to the ``update_mask`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.securitycentermanagement_v1.types.SecurityCenterService:
+                Represents a particular Security
+                Command Center service. This includes
+                settings information such as top-level
+                enablement in addition to individual
+                module settings. Service settings can be
+                configured at the organization, folder,
+                or project level. Service settings at
+                the organization or folder level are
+                inherited by those in child folders and
+                projects.
+
+        """
+        # Create or coerce a protobuf request object.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
+        has_flattened_params = any([security_center_service, update_mask])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(
+            request, security_center_management.UpdateSecurityCenterServiceRequest
+        ):
+            request = security_center_management.UpdateSecurityCenterServiceRequest(
+                request
+            )
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if security_center_service is not None:
+                request.security_center_service = security_center_service
+            if update_mask is not None:
+                request.update_mask = update_mask
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[
+            self._transport.update_security_center_service
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (
+                    (
+                        "security_center_service.name",
+                        request.security_center_service.name,
+                    ),
+                )
+            ),
+        )
+
+        # Validate the universe domain.
+        self._validate_universe_domain()
+
+        # Send the request.
+        response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/pagers.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/pagers.py`

 * *Files 9% similar despite different names*

```diff
@@ -947,7 +947,150 @@
                 for response in page.event_threat_detection_custom_modules:
                     yield response
 
         return async_generator()
 
     def __repr__(self) -> str:
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
+
+
+class ListSecurityCenterServicesPager:
+    """A pager for iterating through ``list_security_center_services`` requests.
+
+    This class thinly wraps an initial
+    :class:`google.cloud.securitycentermanagement_v1.types.ListSecurityCenterServicesResponse` object, and
+    provides an ``__iter__`` method to iterate through its
+    ``security_center_services`` field.
+
+    If there are more pages, the ``__iter__`` method will make additional
+    ``ListSecurityCenterServices`` requests and continue to iterate
+    through the ``security_center_services`` field on the
+    corresponding responses.
+
+    All the usual :class:`google.cloud.securitycentermanagement_v1.types.ListSecurityCenterServicesResponse`
+    attributes are available on the pager. If multiple requests are made, only
+    the most recent response is retained, and thus used for attribute lookup.
+    """
+
+    def __init__(
+        self,
+        method: Callable[
+            ..., security_center_management.ListSecurityCenterServicesResponse
+        ],
+        request: security_center_management.ListSecurityCenterServicesRequest,
+        response: security_center_management.ListSecurityCenterServicesResponse,
+        *,
+        metadata: Sequence[Tuple[str, str]] = ()
+    ):
+        """Instantiate the pager.
+
+        Args:
+            method (Callable): The method that was originally called, and
+                which instantiated this pager.
+            request (google.cloud.securitycentermanagement_v1.types.ListSecurityCenterServicesRequest):
+                The initial request object.
+            response (google.cloud.securitycentermanagement_v1.types.ListSecurityCenterServicesResponse):
+                The initial response object.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        """
+        self._method = method
+        self._request = security_center_management.ListSecurityCenterServicesRequest(
+            request
+        )
+        self._response = response
+        self._metadata = metadata
+
+    def __getattr__(self, name: str) -> Any:
+        return getattr(self._response, name)
+
+    @property
+    def pages(
+        self,
+    ) -> Iterator[security_center_management.ListSecurityCenterServicesResponse]:
+        yield self._response
+        while self._response.next_page_token:
+            self._request.page_token = self._response.next_page_token
+            self._response = self._method(self._request, metadata=self._metadata)
+            yield self._response
+
+    def __iter__(self) -> Iterator[security_center_management.SecurityCenterService]:
+        for page in self.pages:
+            yield from page.security_center_services
+
+    def __repr__(self) -> str:
+        return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
+
+
+class ListSecurityCenterServicesAsyncPager:
+    """A pager for iterating through ``list_security_center_services`` requests.
+
+    This class thinly wraps an initial
+    :class:`google.cloud.securitycentermanagement_v1.types.ListSecurityCenterServicesResponse` object, and
+    provides an ``__aiter__`` method to iterate through its
+    ``security_center_services`` field.
+
+    If there are more pages, the ``__aiter__`` method will make additional
+    ``ListSecurityCenterServices`` requests and continue to iterate
+    through the ``security_center_services`` field on the
+    corresponding responses.
+
+    All the usual :class:`google.cloud.securitycentermanagement_v1.types.ListSecurityCenterServicesResponse`
+    attributes are available on the pager. If multiple requests are made, only
+    the most recent response is retained, and thus used for attribute lookup.
+    """
+
+    def __init__(
+        self,
+        method: Callable[
+            ...,
+            Awaitable[security_center_management.ListSecurityCenterServicesResponse],
+        ],
+        request: security_center_management.ListSecurityCenterServicesRequest,
+        response: security_center_management.ListSecurityCenterServicesResponse,
+        *,
+        metadata: Sequence[Tuple[str, str]] = ()
+    ):
+        """Instantiates the pager.
+
+        Args:
+            method (Callable): The method that was originally called, and
+                which instantiated this pager.
+            request (google.cloud.securitycentermanagement_v1.types.ListSecurityCenterServicesRequest):
+                The initial request object.
+            response (google.cloud.securitycentermanagement_v1.types.ListSecurityCenterServicesResponse):
+                The initial response object.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        """
+        self._method = method
+        self._request = security_center_management.ListSecurityCenterServicesRequest(
+            request
+        )
+        self._response = response
+        self._metadata = metadata
+
+    def __getattr__(self, name: str) -> Any:
+        return getattr(self._response, name)
+
+    @property
+    async def pages(
+        self,
+    ) -> AsyncIterator[security_center_management.ListSecurityCenterServicesResponse]:
+        yield self._response
+        while self._response.next_page_token:
+            self._request.page_token = self._response.next_page_token
+            self._response = await self._method(self._request, metadata=self._metadata)
+            yield self._response
+
+    def __aiter__(
+        self,
+    ) -> AsyncIterator[security_center_management.SecurityCenterService]:
+        async def async_generator():
+            async for page in self.pages:
+                for response in page.security_center_services:
+                    yield response
+
+        return async_generator()
+
+    def __repr__(self) -> str:
+        return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/__init__.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/base.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -334,14 +334,29 @@
                         core_exceptions.ServiceUnavailable,
                     ),
                     deadline=60.0,
                 ),
                 default_timeout=60.0,
                 client_info=client_info,
             ),
+            self.get_security_center_service: gapic_v1.method.wrap_method(
+                self.get_security_center_service,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.list_security_center_services: gapic_v1.method.wrap_method(
+                self.list_security_center_services,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.update_security_center_service: gapic_v1.method.wrap_method(
+                self.update_security_center_service,
+                default_timeout=None,
+                client_info=client_info,
+            ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
         .. warning::
              Only call this method if the transport is NOT shared
@@ -588,14 +603,50 @@
                 security_center_management.ValidateEventThreatDetectionCustomModuleResponse
             ],
         ],
     ]:
         raise NotImplementedError()
 
     @property
+    def get_security_center_service(
+        self,
+    ) -> Callable[
+        [security_center_management.GetSecurityCenterServiceRequest],
+        Union[
+            security_center_management.SecurityCenterService,
+            Awaitable[security_center_management.SecurityCenterService],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def list_security_center_services(
+        self,
+    ) -> Callable[
+        [security_center_management.ListSecurityCenterServicesRequest],
+        Union[
+            security_center_management.ListSecurityCenterServicesResponse,
+            Awaitable[security_center_management.ListSecurityCenterServicesResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def update_security_center_service(
+        self,
+    ) -> Callable[
+        [security_center_management.UpdateSecurityCenterServiceRequest],
+        Union[
+            security_center_management.SecurityCenterService,
+            Awaitable[security_center_management.SecurityCenterService],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def get_location(
         self,
     ) -> Callable[
         [locations_pb2.GetLocationRequest],
         Union[locations_pb2.Location, Awaitable[locations_pb2.Location]],
     ]:
         raise NotImplementedError()
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/grpc.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def __init__(
         self,
         *,
         host: str = "securitycentermanagement.googleapis.com",
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
                  The hostname to connect to (default: 'securitycentermanagement.googleapis.com').
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
@@ -873,14 +878,108 @@
             ] = self.grpc_channel.unary_unary(
                 "/google.cloud.securitycentermanagement.v1.SecurityCenterManagement/ValidateEventThreatDetectionCustomModule",
                 request_serializer=security_center_management.ValidateEventThreatDetectionCustomModuleRequest.serialize,
                 response_deserializer=security_center_management.ValidateEventThreatDetectionCustomModuleResponse.deserialize,
             )
         return self._stubs["validate_event_threat_detection_custom_module"]
 
+    @property
+    def get_security_center_service(
+        self,
+    ) -> Callable[
+        [security_center_management.GetSecurityCenterServiceRequest],
+        security_center_management.SecurityCenterService,
+    ]:
+        r"""Return a callable for the get security center service method over gRPC.
+
+        Gets service settings for the specified Security
+        Command Center service.
+
+        Returns:
+            Callable[[~.GetSecurityCenterServiceRequest],
+                    ~.SecurityCenterService]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_security_center_service" not in self._stubs:
+            self._stubs["get_security_center_service"] = self.grpc_channel.unary_unary(
+                "/google.cloud.securitycentermanagement.v1.SecurityCenterManagement/GetSecurityCenterService",
+                request_serializer=security_center_management.GetSecurityCenterServiceRequest.serialize,
+                response_deserializer=security_center_management.SecurityCenterService.deserialize,
+            )
+        return self._stubs["get_security_center_service"]
+
+    @property
+    def list_security_center_services(
+        self,
+    ) -> Callable[
+        [security_center_management.ListSecurityCenterServicesRequest],
+        security_center_management.ListSecurityCenterServicesResponse,
+    ]:
+        r"""Return a callable for the list security center services method over gRPC.
+
+        Returns a list of all Security Command Center
+        services for the given parent.
+
+        Returns:
+            Callable[[~.ListSecurityCenterServicesRequest],
+                    ~.ListSecurityCenterServicesResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_security_center_services" not in self._stubs:
+            self._stubs[
+                "list_security_center_services"
+            ] = self.grpc_channel.unary_unary(
+                "/google.cloud.securitycentermanagement.v1.SecurityCenterManagement/ListSecurityCenterServices",
+                request_serializer=security_center_management.ListSecurityCenterServicesRequest.serialize,
+                response_deserializer=security_center_management.ListSecurityCenterServicesResponse.deserialize,
+            )
+        return self._stubs["list_security_center_services"]
+
+    @property
+    def update_security_center_service(
+        self,
+    ) -> Callable[
+        [security_center_management.UpdateSecurityCenterServiceRequest],
+        security_center_management.SecurityCenterService,
+    ]:
+        r"""Return a callable for the update security center service method over gRPC.
+
+        Updates a Security Command Center service using the
+        given update mask.
+
+        Returns:
+            Callable[[~.UpdateSecurityCenterServiceRequest],
+                    ~.SecurityCenterService]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "update_security_center_service" not in self._stubs:
+            self._stubs[
+                "update_security_center_service"
+            ] = self.grpc_channel.unary_unary(
+                "/google.cloud.securitycentermanagement.v1.SecurityCenterManagement/UpdateSecurityCenterService",
+                request_serializer=security_center_management.UpdateSecurityCenterServiceRequest.serialize,
+                response_deserializer=security_center_management.SecurityCenterService.deserialize,
+            )
+        return self._stubs["update_security_center_service"]
+
     def close(self):
         self.grpc_channel.close()
 
     @property
     def list_locations(
         self,
     ) -> Callable[
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/grpc_asyncio.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/grpc_asyncio.py`

 * *Files 14% similar despite different names*

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
 from google.cloud.location import locations_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
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
         host: str = "securitycentermanagement.googleapis.com",
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
                  The hostname to connect to (default: 'securitycentermanagement.googleapis.com').
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
@@ -894,14 +900,338 @@
             ] = self.grpc_channel.unary_unary(
                 "/google.cloud.securitycentermanagement.v1.SecurityCenterManagement/ValidateEventThreatDetectionCustomModule",
                 request_serializer=security_center_management.ValidateEventThreatDetectionCustomModuleRequest.serialize,
                 response_deserializer=security_center_management.ValidateEventThreatDetectionCustomModuleResponse.deserialize,
             )
         return self._stubs["validate_event_threat_detection_custom_module"]
 
+    @property
+    def get_security_center_service(
+        self,
+    ) -> Callable[
+        [security_center_management.GetSecurityCenterServiceRequest],
+        Awaitable[security_center_management.SecurityCenterService],
+    ]:
+        r"""Return a callable for the get security center service method over gRPC.
+
+        Gets service settings for the specified Security
+        Command Center service.
+
+        Returns:
+            Callable[[~.GetSecurityCenterServiceRequest],
+                    Awaitable[~.SecurityCenterService]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_security_center_service" not in self._stubs:
+            self._stubs["get_security_center_service"] = self.grpc_channel.unary_unary(
+                "/google.cloud.securitycentermanagement.v1.SecurityCenterManagement/GetSecurityCenterService",
+                request_serializer=security_center_management.GetSecurityCenterServiceRequest.serialize,
+                response_deserializer=security_center_management.SecurityCenterService.deserialize,
+            )
+        return self._stubs["get_security_center_service"]
+
+    @property
+    def list_security_center_services(
+        self,
+    ) -> Callable[
+        [security_center_management.ListSecurityCenterServicesRequest],
+        Awaitable[security_center_management.ListSecurityCenterServicesResponse],
+    ]:
+        r"""Return a callable for the list security center services method over gRPC.
+
+        Returns a list of all Security Command Center
+        services for the given parent.
+
+        Returns:
+            Callable[[~.ListSecurityCenterServicesRequest],
+                    Awaitable[~.ListSecurityCenterServicesResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_security_center_services" not in self._stubs:
+            self._stubs[
+                "list_security_center_services"
+            ] = self.grpc_channel.unary_unary(
+                "/google.cloud.securitycentermanagement.v1.SecurityCenterManagement/ListSecurityCenterServices",
+                request_serializer=security_center_management.ListSecurityCenterServicesRequest.serialize,
+                response_deserializer=security_center_management.ListSecurityCenterServicesResponse.deserialize,
+            )
+        return self._stubs["list_security_center_services"]
+
+    @property
+    def update_security_center_service(
+        self,
+    ) -> Callable[
+        [security_center_management.UpdateSecurityCenterServiceRequest],
+        Awaitable[security_center_management.SecurityCenterService],
+    ]:
+        r"""Return a callable for the update security center service method over gRPC.
+
+        Updates a Security Command Center service using the
+        given update mask.
+
+        Returns:
+            Callable[[~.UpdateSecurityCenterServiceRequest],
+                    Awaitable[~.SecurityCenterService]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "update_security_center_service" not in self._stubs:
+            self._stubs[
+                "update_security_center_service"
+            ] = self.grpc_channel.unary_unary(
+                "/google.cloud.securitycentermanagement.v1.SecurityCenterManagement/UpdateSecurityCenterService",
+                request_serializer=security_center_management.UpdateSecurityCenterServiceRequest.serialize,
+                response_deserializer=security_center_management.SecurityCenterService.deserialize,
+            )
+        return self._stubs["update_security_center_service"]
+
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.list_effective_security_health_analytics_custom_modules: gapic_v1.method_async.wrap_method(
+                self.list_effective_security_health_analytics_custom_modules,
+                default_retry=retries.AsyncRetry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_effective_security_health_analytics_custom_module: gapic_v1.method_async.wrap_method(
+                self.get_effective_security_health_analytics_custom_module,
+                default_retry=retries.AsyncRetry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.list_security_health_analytics_custom_modules: gapic_v1.method_async.wrap_method(
+                self.list_security_health_analytics_custom_modules,
+                default_retry=retries.AsyncRetry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.list_descendant_security_health_analytics_custom_modules: gapic_v1.method_async.wrap_method(
+                self.list_descendant_security_health_analytics_custom_modules,
+                default_retry=retries.AsyncRetry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_security_health_analytics_custom_module: gapic_v1.method_async.wrap_method(
+                self.get_security_health_analytics_custom_module,
+                default_retry=retries.AsyncRetry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.create_security_health_analytics_custom_module: gapic_v1.method_async.wrap_method(
+                self.create_security_health_analytics_custom_module,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.update_security_health_analytics_custom_module: gapic_v1.method_async.wrap_method(
+                self.update_security_health_analytics_custom_module,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.delete_security_health_analytics_custom_module: gapic_v1.method_async.wrap_method(
+                self.delete_security_health_analytics_custom_module,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.simulate_security_health_analytics_custom_module: gapic_v1.method_async.wrap_method(
+                self.simulate_security_health_analytics_custom_module,
+                default_retry=retries.AsyncRetry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.list_effective_event_threat_detection_custom_modules: gapic_v1.method_async.wrap_method(
+                self.list_effective_event_threat_detection_custom_modules,
+                default_retry=retries.AsyncRetry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_effective_event_threat_detection_custom_module: gapic_v1.method_async.wrap_method(
+                self.get_effective_event_threat_detection_custom_module,
+                default_retry=retries.AsyncRetry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.list_event_threat_detection_custom_modules: gapic_v1.method_async.wrap_method(
+                self.list_event_threat_detection_custom_modules,
+                default_retry=retries.AsyncRetry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.list_descendant_event_threat_detection_custom_modules: gapic_v1.method_async.wrap_method(
+                self.list_descendant_event_threat_detection_custom_modules,
+                default_retry=retries.AsyncRetry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_event_threat_detection_custom_module: gapic_v1.method_async.wrap_method(
+                self.get_event_threat_detection_custom_module,
+                default_retry=retries.AsyncRetry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.create_event_threat_detection_custom_module: gapic_v1.method_async.wrap_method(
+                self.create_event_threat_detection_custom_module,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.update_event_threat_detection_custom_module: gapic_v1.method_async.wrap_method(
+                self.update_event_threat_detection_custom_module,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.delete_event_threat_detection_custom_module: gapic_v1.method_async.wrap_method(
+                self.delete_event_threat_detection_custom_module,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.validate_event_threat_detection_custom_module: gapic_v1.method_async.wrap_method(
+                self.validate_event_threat_detection_custom_module,
+                default_retry=retries.AsyncRetry(
+                    initial=0.1,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_security_center_service: gapic_v1.method_async.wrap_method(
+                self.get_security_center_service,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.list_security_center_services: gapic_v1.method_async.wrap_method(
+                self.list_security_center_services,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.update_security_center_service: gapic_v1.method_async.wrap_method(
+                self.update_security_center_service,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
     @property
     def list_locations(
         self,
     ) -> Callable[
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/rest.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/services/security_center_management/transports/rest.py`

 * *Files 9% similar despite different names*

```diff
@@ -110,14 +110,22 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_get_event_threat_detection_custom_module(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_get_security_center_service(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_get_security_center_service(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_get_security_health_analytics_custom_module(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_get_security_health_analytics_custom_module(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -158,14 +166,22 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_list_event_threat_detection_custom_modules(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_list_security_center_services(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_list_security_center_services(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_list_security_health_analytics_custom_modules(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_list_security_health_analytics_custom_modules(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -182,14 +198,22 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_update_event_threat_detection_custom_module(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_update_security_center_service(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_update_security_center_service(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_update_security_health_analytics_custom_module(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_update_security_health_analytics_custom_module(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -366,14 +390,40 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the SecurityCenterManagement server but before
         it is returned to user code.
         """
         return response
 
+    def pre_get_security_center_service(
+        self,
+        request: security_center_management.GetSecurityCenterServiceRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[
+        security_center_management.GetSecurityCenterServiceRequest,
+        Sequence[Tuple[str, str]],
+    ]:
+        """Pre-rpc interceptor for get_security_center_service
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the SecurityCenterManagement server.
+        """
+        return request, metadata
+
+    def post_get_security_center_service(
+        self, response: security_center_management.SecurityCenterService
+    ) -> security_center_management.SecurityCenterService:
+        """Post-rpc interceptor for get_security_center_service
+
+        Override in a subclass to manipulate the response
+        after it is returned by the SecurityCenterManagement server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_get_security_health_analytics_custom_module(
         self,
         request: security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[
         security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest,
         Sequence[Tuple[str, str]],
@@ -535,14 +585,40 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the SecurityCenterManagement server but before
         it is returned to user code.
         """
         return response
 
+    def pre_list_security_center_services(
+        self,
+        request: security_center_management.ListSecurityCenterServicesRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[
+        security_center_management.ListSecurityCenterServicesRequest,
+        Sequence[Tuple[str, str]],
+    ]:
+        """Pre-rpc interceptor for list_security_center_services
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the SecurityCenterManagement server.
+        """
+        return request, metadata
+
+    def post_list_security_center_services(
+        self, response: security_center_management.ListSecurityCenterServicesResponse
+    ) -> security_center_management.ListSecurityCenterServicesResponse:
+        """Post-rpc interceptor for list_security_center_services
+
+        Override in a subclass to manipulate the response
+        after it is returned by the SecurityCenterManagement server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_list_security_health_analytics_custom_modules(
         self,
         request: security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[
         security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest,
         Sequence[Tuple[str, str]],
@@ -615,14 +691,40 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the SecurityCenterManagement server but before
         it is returned to user code.
         """
         return response
 
+    def pre_update_security_center_service(
+        self,
+        request: security_center_management.UpdateSecurityCenterServiceRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[
+        security_center_management.UpdateSecurityCenterServiceRequest,
+        Sequence[Tuple[str, str]],
+    ]:
+        """Pre-rpc interceptor for update_security_center_service
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the SecurityCenterManagement server.
+        """
+        return request, metadata
+
+    def post_update_security_center_service(
+        self, response: security_center_management.SecurityCenterService
+    ) -> security_center_management.SecurityCenterService:
+        """Post-rpc interceptor for update_security_center_service
+
+        Override in a subclass to manipulate the response
+        after it is returned by the SecurityCenterManagement server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_update_security_health_analytics_custom_module(
         self,
         request: security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[
         security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest,
         Sequence[Tuple[str, str]],
@@ -1595,14 +1697,123 @@
                 resp
             )
 
             json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_get_event_threat_detection_custom_module(resp)
             return resp
 
+    class _GetSecurityCenterService(SecurityCenterManagementRestStub):
+        def __hash__(self):
+            return hash("GetSecurityCenterService")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: security_center_management.GetSecurityCenterServiceRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> security_center_management.SecurityCenterService:
+            r"""Call the get security center
+            service method over HTTP.
+
+                Args:
+                    request (~.security_center_management.GetSecurityCenterServiceRequest):
+                        The request object. Request message for getting a
+                    Security Command Center service.
+                    retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                        should be retried.
+                    timeout (float): The timeout for this request.
+                    metadata (Sequence[Tuple[str, str]]): Strings which should be
+                        sent along with the request as metadata.
+
+                Returns:
+                    ~.security_center_management.SecurityCenterService:
+                        Represents a particular Security
+                    Command Center service. This includes
+                    settings information such as top-level
+                    enablement in addition to individual
+                    module settings. Service settings can be
+                    configured at the organization, folder,
+                    or project level. Service settings at
+                    the organization or folder level are
+                    inherited by those in child folders and
+                    projects.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=projects/*/locations/*/securityCenterServices/*}",
+                },
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=folders/*/locations/*/securityCenterServices/*}",
+                },
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=organizations/*/locations/*/securityCenterServices/*}",
+                },
+            ]
+            request, metadata = self._interceptor.pre_get_security_center_service(
+                request, metadata
+            )
+            pb_request = security_center_management.GetSecurityCenterServiceRequest.pb(
+                request
+            )
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = security_center_management.SecurityCenterService()
+            pb_resp = security_center_management.SecurityCenterService.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_get_security_center_service(resp)
+            return resp
+
     class _GetSecurityHealthAnalyticsCustomModule(SecurityCenterManagementRestStub):
         def __hash__(self):
             return hash("GetSecurityHealthAnalyticsCustomModule")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
@@ -2284,14 +2495,117 @@
 
             json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_list_event_threat_detection_custom_modules(
                 resp
             )
             return resp
 
+    class _ListSecurityCenterServices(SecurityCenterManagementRestStub):
+        def __hash__(self):
+            return hash("ListSecurityCenterServices")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: security_center_management.ListSecurityCenterServicesRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> security_center_management.ListSecurityCenterServicesResponse:
+            r"""Call the list security center
+            services method over HTTP.
+
+                Args:
+                    request (~.security_center_management.ListSecurityCenterServicesRequest):
+                        The request object. Request message for listing Security
+                    Command Center services.
+                    retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                        should be retried.
+                    timeout (float): The timeout for this request.
+                    metadata (Sequence[Tuple[str, str]]): Strings which should be
+                        sent along with the request as metadata.
+
+                Returns:
+                    ~.security_center_management.ListSecurityCenterServicesResponse:
+                        Response message for listing Security
+                    Command Center services.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{parent=projects/*/locations/*}/securityCenterServices",
+                },
+                {
+                    "method": "get",
+                    "uri": "/v1/{parent=folders/*/locations/*}/securityCenterServices",
+                },
+                {
+                    "method": "get",
+                    "uri": "/v1/{parent=organizations/*/locations/*}/securityCenterServices",
+                },
+            ]
+            request, metadata = self._interceptor.pre_list_security_center_services(
+                request, metadata
+            )
+            pb_request = (
+                security_center_management.ListSecurityCenterServicesRequest.pb(request)
+            )
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = security_center_management.ListSecurityCenterServicesResponse()
+            pb_resp = security_center_management.ListSecurityCenterServicesResponse.pb(
+                resp
+            )
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_list_security_center_services(resp)
+            return resp
+
     class _ListSecurityHealthAnalyticsCustomModules(SecurityCenterManagementRestStub):
         def __hash__(self):
             return hash("ListSecurityHealthAnalyticsCustomModules")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
@@ -2647,14 +2961,136 @@
 
             json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_update_event_threat_detection_custom_module(
                 resp
             )
             return resp
 
+    class _UpdateSecurityCenterService(SecurityCenterManagementRestStub):
+        def __hash__(self):
+            return hash("UpdateSecurityCenterService")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
+            "updateMask": {},
+        }
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: security_center_management.UpdateSecurityCenterServiceRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> security_center_management.SecurityCenterService:
+            r"""Call the update security center
+            service method over HTTP.
+
+                Args:
+                    request (~.security_center_management.UpdateSecurityCenterServiceRequest):
+                        The request object. Request message for updating a
+                    Security Command Center service.
+                    retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                        should be retried.
+                    timeout (float): The timeout for this request.
+                    metadata (Sequence[Tuple[str, str]]): Strings which should be
+                        sent along with the request as metadata.
+
+                Returns:
+                    ~.security_center_management.SecurityCenterService:
+                        Represents a particular Security
+                    Command Center service. This includes
+                    settings information such as top-level
+                    enablement in addition to individual
+                    module settings. Service settings can be
+                    configured at the organization, folder,
+                    or project level. Service settings at
+                    the organization or folder level are
+                    inherited by those in child folders and
+                    projects.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "patch",
+                    "uri": "/v1/{security_center_service.name=projects/*/locations/*/securityCenterServices/*}",
+                    "body": "security_center_service",
+                },
+                {
+                    "method": "patch",
+                    "uri": "/v1/{security_center_service.name=folders/*/locations/*/securityCenterServices/*}",
+                    "body": "security_center_service",
+                },
+                {
+                    "method": "patch",
+                    "uri": "/v1/{security_center_service.name=organizations/*/locations/*/securityCenterServices/*}",
+                    "body": "security_center_service",
+                },
+            ]
+            request, metadata = self._interceptor.pre_update_security_center_service(
+                request, metadata
+            )
+            pb_request = (
+                security_center_management.UpdateSecurityCenterServiceRequest.pb(
+                    request
+                )
+            )
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"], use_integers_for_enums=True
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = security_center_management.SecurityCenterService()
+            pb_resp = security_center_management.SecurityCenterService.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_update_security_center_service(resp)
+            return resp
+
     class _UpdateSecurityHealthAnalyticsCustomModule(SecurityCenterManagementRestStub):
         def __hash__(self):
             return hash("UpdateSecurityHealthAnalyticsCustomModule")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
             "updateMask": {},
         }
@@ -2979,14 +3415,25 @@
         security_center_management.EventThreatDetectionCustomModule,
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._GetEventThreatDetectionCustomModule(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def get_security_center_service(
+        self,
+    ) -> Callable[
+        [security_center_management.GetSecurityCenterServiceRequest],
+        security_center_management.SecurityCenterService,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._GetSecurityCenterService(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def get_security_health_analytics_custom_module(
         self,
     ) -> Callable[
         [security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest],
         security_center_management.SecurityHealthAnalyticsCustomModule,
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
@@ -3053,14 +3500,25 @@
         security_center_management.ListEventThreatDetectionCustomModulesResponse,
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._ListEventThreatDetectionCustomModules(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def list_security_center_services(
+        self,
+    ) -> Callable[
+        [security_center_management.ListSecurityCenterServicesRequest],
+        security_center_management.ListSecurityCenterServicesResponse,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._ListSecurityCenterServices(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def list_security_health_analytics_custom_modules(
         self,
     ) -> Callable[
         [security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest],
         security_center_management.ListSecurityHealthAnalyticsCustomModulesResponse,
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
@@ -3086,14 +3544,25 @@
         security_center_management.EventThreatDetectionCustomModule,
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._UpdateEventThreatDetectionCustomModule(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def update_security_center_service(
+        self,
+    ) -> Callable[
+        [security_center_management.UpdateSecurityCenterServiceRequest],
+        security_center_management.SecurityCenterService,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._UpdateSecurityCenterService(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def update_security_health_analytics_custom_module(
         self,
     ) -> Callable[
         [security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest],
         security_center_management.SecurityHealthAnalyticsCustomModule,
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google/cloud/securitycentermanagement_v1/types/security_center_management.py` & `google-cloud-securitycentermanagement-0.1.9/google/cloud/securitycentermanagement_v1/types/security_center_management.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from google.rpc import status_pb2  # type: ignore
 from google.type import expr_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.securitycentermanagement.v1",
     manifest={
+        "SecurityCenterService",
         "EffectiveSecurityHealthAnalyticsCustomModule",
         "ListEffectiveSecurityHealthAnalyticsCustomModulesRequest",
         "ListEffectiveSecurityHealthAnalyticsCustomModulesResponse",
         "GetEffectiveSecurityHealthAnalyticsCustomModuleRequest",
         "SecurityHealthAnalyticsCustomModule",
         "CustomConfig",
         "ListSecurityHealthAnalyticsCustomModulesRequest",
@@ -57,18 +58,163 @@
         "ListDescendantEventThreatDetectionCustomModulesResponse",
         "GetEventThreatDetectionCustomModuleRequest",
         "CreateEventThreatDetectionCustomModuleRequest",
         "UpdateEventThreatDetectionCustomModuleRequest",
         "DeleteEventThreatDetectionCustomModuleRequest",
         "ValidateEventThreatDetectionCustomModuleRequest",
         "ValidateEventThreatDetectionCustomModuleResponse",
+        "GetSecurityCenterServiceRequest",
+        "ListSecurityCenterServicesRequest",
+        "ListSecurityCenterServicesResponse",
+        "UpdateSecurityCenterServiceRequest",
     },
 )
 
 
+class SecurityCenterService(proto.Message):
+    r"""Represents a particular Security Command Center service. This
+    includes settings information such as top-level enablement in
+    addition to individual module settings. Service settings can be
+    configured at the organization, folder, or project level.
+    Service settings at the organization or folder level are
+    inherited by those in child folders and projects.
+
+    Attributes:
+        name (str):
+            Identifier. The name of the service.
+
+            Its format is:
+
+            -  organizations/{organization}/locations/{location}/securityCenterServices/{service}
+            -  folders/{folder}/locations/{location}/securityCenterServices/{service}
+            -  projects/{project}/locations/{location}/securityCenterServices/{service}
+
+            The possible values for id {service} are:
+
+            -  container-threat-detection
+            -  event-threat-detection
+            -  security-health-analytics
+            -  vm-threat-detection
+            -  web-security-scanner
+        intended_enablement_state (google.cloud.securitycentermanagement_v1.types.SecurityCenterService.EnablementState):
+            Optional. The intended state of enablement for the service
+            at its level of the resource hierarchy. A DISABLED state
+            will override all module enablement_states to DISABLED.
+        effective_enablement_state (google.cloud.securitycentermanagement_v1.types.SecurityCenterService.EnablementState):
+            Output only. The effective enablement state
+            for the service at its level of the resource
+            hierarchy. If the intended state is set to
+            INHERITED, the effective state will be inherited
+            from the enablement state of an ancestor. This
+            state may differ from the intended enablement
+            state due to billing eligibility or onboarding
+            status.
+        modules (MutableMapping[str, google.cloud.securitycentermanagement_v1.types.SecurityCenterService.ModuleSettings]):
+            Optional. The configurations including the
+            state of enablement for the service's different
+            modules. The absence of a module in the map
+            implies its configuration is inherited from its
+            parents.
+        update_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. The time the service was last
+            updated. This could be due to an explicit user
+            update or due to a side effect of another system
+            change such as billing subscription expiry.
+        service_config (google.protobuf.struct_pb2.Struct):
+            Optional. Additional service specific
+            configuration. Not all services will utilize
+            this field.
+    """
+
+    class EnablementState(proto.Enum):
+        r"""Represents the possible intended states of enablement for a
+        service or module.
+
+        Values:
+            ENABLEMENT_STATE_UNSPECIFIED (0):
+                Default value. This value is unused.
+            INHERITED (1):
+                State is inherited from the parent resource.
+                Not a valid effective enablement state.
+            ENABLED (2):
+                State is enabled.
+            DISABLED (3):
+                State is disabled.
+        """
+        ENABLEMENT_STATE_UNSPECIFIED = 0
+        INHERITED = 1
+        ENABLED = 2
+        DISABLED = 3
+
+    class ModuleSettings(proto.Message):
+        r"""The settings for individual modules.
+
+        Attributes:
+            intended_enablement_state (google.cloud.securitycentermanagement_v1.types.SecurityCenterService.EnablementState):
+                Optional. The intended state of enablement
+                for the module at its level of the resource
+                hierarchy.
+            effective_enablement_state (google.cloud.securitycentermanagement_v1.types.SecurityCenterService.EnablementState):
+                Output only. The effective enablement state
+                for the module at its level of the resource
+                hierarchy. If the intended state is set to
+                INHERITED, the effective state will be inherited
+                from the enablement state of an ancestor. This
+                state may
+                differ from the intended enablement state due to
+                billing eligibility or onboarding status.
+        """
+
+        intended_enablement_state: "SecurityCenterService.EnablementState" = (
+            proto.Field(
+                proto.ENUM,
+                number=1,
+                enum="SecurityCenterService.EnablementState",
+            )
+        )
+        effective_enablement_state: "SecurityCenterService.EnablementState" = (
+            proto.Field(
+                proto.ENUM,
+                number=2,
+                enum="SecurityCenterService.EnablementState",
+            )
+        )
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    intended_enablement_state: EnablementState = proto.Field(
+        proto.ENUM,
+        number=2,
+        enum=EnablementState,
+    )
+    effective_enablement_state: EnablementState = proto.Field(
+        proto.ENUM,
+        number=3,
+        enum=EnablementState,
+    )
+    modules: MutableMapping[str, ModuleSettings] = proto.MapField(
+        proto.STRING,
+        proto.MESSAGE,
+        number=4,
+        message=ModuleSettings,
+    )
+    update_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=5,
+        message=timestamp_pb2.Timestamp,
+    )
+    service_config: struct_pb2.Struct = proto.Field(
+        proto.MESSAGE,
+        number=6,
+        message=struct_pb2.Struct,
+    )
+
+
 class EffectiveSecurityHealthAnalyticsCustomModule(proto.Message):
     r"""An EffectiveSecurityHealthAnalyticsCustomModule is the
     representation of a Security Health Analytics custom module at a
     specified level of the resource hierarchy: organization, folder, or
     project. If a custom module is inherited from a parent organization
     or folder, the value of the ``enablementState`` property in
     EffectiveSecurityHealthAnalyticsCustomModule is set to the value
@@ -76,21 +222,20 @@
     example, if the module is enabled in a parent organization or
     folder, the effective enablement_state for the module in all child
     folders or projects is also ``enabled``.
     EffectiveSecurityHealthAnalyticsCustomModule is read-only.
 
     Attributes:
         name (str):
-            Identifier. The resource name of the custom module. Its
-            format is
-            "organizations/{organization}/locations/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}",
-            or
-            "folders/{folder}/locations/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}",
-            or
-            "projects/{project}/locations/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}".
+            Identifier. The full resource name of the custom module,
+            specified in one of the following formats:
+
+            -  ``organizations/organization/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}``
+            -  ``folders/folder/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}``
+            -  ``projects/project/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}``
         custom_config (google.cloud.securitycentermanagement_v1.types.CustomConfig):
             Output only. The user-specified configuration
             for the module.
         enablement_state (google.cloud.securitycentermanagement_v1.types.EffectiveSecurityHealthAnalyticsCustomModule.EnablementState):
             Output only. The effective state of
             enablement for the module at the given level of
             the hierarchy.
@@ -139,20 +284,20 @@
 
 class ListEffectiveSecurityHealthAnalyticsCustomModulesRequest(proto.Message):
     r"""Request message for listing effective Security Health
     Analytics custom modules.
 
     Attributes:
         parent (str):
-            Required. Name of parent to list effective
-            custom modules. Its format is
-            "organizations/{organization}/locations/{location}",
-            "folders/{folder}/locations/{location}",
-            or
-            "projects/{project}/locations/{location}".
+            Required. Name of parent to list effective custom modules.
+            specified in one of the following formats:
+
+            -  ``organizations/{organization}/locations/{location}``
+            -  ``folders/{folder}/locations/{location}`` or
+               ``projects/{project}/locations/{location}``
         page_size (int):
             Optional. The maximum number of results to
             return in a single response. Default is 10,
             minimum is 1, maximum is 1000.
         page_token (str):
             Optional. The value returned by the last call
             indicating a continuation.
@@ -204,21 +349,20 @@
 
 class GetEffectiveSecurityHealthAnalyticsCustomModuleRequest(proto.Message):
     r"""Message for getting a
     EffectiveSecurityHealthAnalyticsCustomModule
 
     Attributes:
         name (str):
-            Required. The resource name of the SHA custom module.
-
-            Its format is:
+            Required. The full resource name of the custom module,
+            specified in one of the following formats:
 
-            -  "organizations/{organization}/locations/{location}/effectiveSecurityHealthAnalyticsCustomModules/{module_id}".
-            -  "folders/{folder}/locations/{location}/effectiveSecurityHealthAnalyticsCustomModules/{module_id}".
-            -  "projects/{project}/locations/{location}/effectiveSecurityHealthAnalyticsCustomModules/{module_id}".
+            -  ``organizations/organization/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}``
+            -  ``folders/folder/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}``
+            -  ``projects/project/{location}/effectiveSecurityHealthAnalyticsCustomModules/{effective_security_health_analytics_custom_module}``
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
@@ -229,24 +373,20 @@
     state, and last updated time. You can create a custom module at
     the organization, folder, or project level. Custom modules that
     you create at the organization or folder level are inherited by
     the child folders and projects.
 
     Attributes:
         name (str):
-            Identifier. The resource name of the custom module. Its
-            format is
-            "organizations/{organization}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}",
-            or
-            "folders/{folder}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}",
-            or
-            "projects/{project}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}"
+            Identifier. The full resource name of the custom module,
+            specified in one of the following formats:
 
-            The id {customModule} is server-generated and is not user
-            settable. It will be a numeric id containing 1-20 digits.
+            -  ``organizations/{organization}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}``
+            -  ``folders/{folder}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}``
+            -  ``projects/{project}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}``
         display_name (str):
             Optional. The display name of the Security
             Health Analytics custom module. This display
             name becomes the finding category for all
             findings that are returned by this custom
             module. The display name must be between 1 and
             128 characters, start with a lowercase letter,
@@ -481,20 +621,21 @@
 
 class ListSecurityHealthAnalyticsCustomModulesRequest(proto.Message):
     r"""Request message for listing Security Health Analytics custom
     modules.
 
     Attributes:
         parent (str):
-            Required. Name of parent to list custom
-            modules. Its format is
-            "organizations/{organization}/locations/{location}",
-            "folders/{folder}/locations/{location}",
-            or
-            "projects/{project}/locations/{location}".
+            Required. Name of parent organization, folder, or project in
+            which to list custom modules, specified in one of the
+            following formats:
+
+            -  ``organizations/{organization}/locations/{location}``
+            -  ``folders/{folder}/locations/{location}``
+            -  ``projects/{project}/locations/{location}``
         page_size (int):
             Optional. The maximum number of results to
             return in a single response. Default is 10,
             minimum is 1, maximum is 1000.
         page_token (str):
             Optional. A token identifying a page of
             results the server should return.
@@ -546,20 +687,21 @@
 
 class ListDescendantSecurityHealthAnalyticsCustomModulesRequest(proto.Message):
     r"""Request message for listing descendant Security Health
     Analytics custom modules.
 
     Attributes:
         parent (str):
-            Required. Name of parent to list custom
-            modules. Its format is
-            "organizations/{organization}/locations/{location}",
-            "folders/{folder}/locations/{location}",
-            or
-            "projects/{project}/locations/{location}".
+            Required. Name of the parent organization, folder, or
+            project in which to list custom modules, specified in one of
+            the following formats:
+
+            -  ``organizations/{organization}/locations/{location}``
+            -  ``folders/{folder}/locations/{location}``
+            -  ``projects/{project}/locations/{location}``
         page_size (int):
             Optional. The maximum number of results to
             return in a single response. Default is 10,
             minimum is 1, maximum is 1000.
         page_token (str):
             Optional. A token identifying a page of
             results the server should return.
@@ -624,20 +766,21 @@
 
 
 class CreateSecurityHealthAnalyticsCustomModuleRequest(proto.Message):
     r"""Message for creating a SecurityHealthAnalyticsCustomModule
 
     Attributes:
         parent (str):
-            Required. Name of the parent for the module.
-            Its format is
-            "organizations/{organization}/locations/{location}",
-            "folders/{folder}/locations/{location}",
-            or
-            "projects/{project}/locations/{location}".
+            Required. Name of the parent organization, folder, or
+            project of the module, specified in one of the following
+            formats:
+
+            -  ``organizations/{organization}/locations/{location}``
+            -  ``folders/{folder}/locations/{location}``
+            -  ``projects/{project}/locations/{location}``
         security_health_analytics_custom_module (google.cloud.securitycentermanagement_v1.types.SecurityHealthAnalyticsCustomModule):
             Required. The resource being created
         validate_only (bool):
             Optional. When set to true, only validations
             (including IAM checks) will done for the request
             (no module will be created). An OK response
             indicates the request is valid while an error
@@ -715,17 +858,17 @@
 
     Attributes:
         name (str):
             Required. The resource name of the SHA custom module.
 
             Its format is:
 
-            -  "organizations/{organization}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}".
-            -  "folders/{folder}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}".
-            -  "projects/{project}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}".
+            -  ``organizations/{organization}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}``.
+            -  ``folders/{folder}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}``.
+            -  ``projects/{project}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}``.
         validate_only (bool):
             Optional. When set to true, only validations
             (including IAM checks) will done for the request
             (module will not be deleted). An OK response
             indicates the request is valid while an error
             response indicates the request is invalid. Note
             that a subsequent request to actually delete the
@@ -818,23 +961,23 @@
     finding from a SHA custom module.
 
     Attributes:
         name (str):
             Identifier. The `relative resource
             name <https://cloud.google.com/apis/design/resource_names#relative_resource_name>`__
             of the finding. Example:
-            "organizations/{organization_id}/sources/{source_id}/findings/{finding_id}",
-            "folders/{folder_id}/sources/{source_id}/findings/{finding_id}",
-            "projects/{project_id}/sources/{source_id}/findings/{finding_id}".
+            ``organizations/{organization_id}/sources/{source_id}/findings/{finding_id}``,
+            ``folders/{folder_id}/sources/{source_id}/findings/{finding_id}``,
+            ``projects/{project_id}/sources/{source_id}/findings/{finding_id}``.
         parent (str):
             The relative resource name of the source the finding belongs
             to. See:
             https://cloud.google.com/apis/design/resource_names#relative_resource_name
             This field is immutable after creation time. For example:
-            "organizations/{organization_id}/sources/{source_id}".
+            ``organizations/{organization_id}/sources/{source_id}``
         resource_name (str):
             For findings on Google Cloud resources, the full resource
             name of the Google Cloud resource this finding is for. See:
             https://cloud.google.com/apis/design/resource_names#full_resource_name
             When the finding is for a non-Google Cloud resource, the
             resourceName can be a customer or partner defined string.
             This field is immutable after creation time.
@@ -1127,17 +1270,17 @@
 
     Attributes:
         name (str):
             Identifier. The resource name of the ETD custom module.
 
             Its format is:
 
-            -  "organizations/{organization}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}".
-            -  "folders/{folder}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}".
-            -  "projects/{project}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}".
+            -  ``organizations/{organization}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}``.
+            -  ``folders/{folder}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}``.
+            -  ``projects/{project}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}``.
         config (google.protobuf.struct_pb2.Struct):
             Output only. Config for the effective module.
         enablement_state (google.cloud.securitycentermanagement_v1.types.EffectiveEventThreatDetectionCustomModule.EnablementState):
             Output only. The effective state of
             enablement for the module at the given level of
             the hierarchy.
         type_ (str):
@@ -1194,20 +1337,19 @@
 
 class ListEffectiveEventThreatDetectionCustomModulesRequest(proto.Message):
     r"""Request message for listing effective Event Threat Detection
     custom modules.
 
     Attributes:
         parent (str):
-            Required. Name of parent to list effective
-            custom modules. Its format is
-            "organizations/{organization}/locations/{location}",
-            "folders/{folder}/locations/{location}",
-            or
-            "projects/{project}/locations/{location}".
+            Required. Name of parent to list effective custom modules.
+            Its format is
+            ``organizations/{organization}/locations/{location}``,
+            ``folders/{folder}/locations/{location}``, or
+            ``projects/{project}/locations/{location}``
         page_size (int):
             Optional. The maximum number of results to
             return in a single response. Default is 10,
             minimum is 1, maximum is 1000.
         page_token (str):
             Optional. The value returned by the last call
             indicating a continuation
@@ -1263,17 +1405,17 @@
 
     Attributes:
         name (str):
             Required. The resource name of the ETD custom module.
 
             Its format is:
 
-            -  "organizations/{organization}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}".
-            -  "folders/{folder}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}".
-            -  "projects/{project}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}".
+            -  ``organizations/{organization}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}``.
+            -  ``folders/{folder}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}``.
+            -  ``projects/{project}/locations/{location}/effectiveEventThreatDetectionCustomModules/{effective_event_threat_detection_custom_module}``.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
@@ -1286,17 +1428,17 @@
 
     Attributes:
         name (str):
             Identifier. The resource name of the ETD custom module.
 
             Its format is:
 
-            -  "organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-            -  "folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-            -  "projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
+            -  ``organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+            -  ``folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+            -  ``projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
         config (google.protobuf.struct_pb2.Struct):
             Optional. Config for the module. For the
             resident module, its config value is defined at
             this level. For the inherited module, its config
             value is inherited from the ancestor module.
         ancestor_module (str):
             Output only. The closest ancestor module that
@@ -1391,20 +1533,18 @@
 
 class ListEventThreatDetectionCustomModulesRequest(proto.Message):
     r"""Request message for listing Event Threat Detection custom
     modules.
 
     Attributes:
         parent (str):
-            Required. Name of parent to list custom
-            modules. Its format is
-            "organizations/{organization}/locations/{location}",
-            "folders/{folder}/locations/{location}",
-            or
-            "projects/{project}/locations/{location}".
+            Required. Name of parent to list custom modules. Its format
+            is ``organizations/{organization}/locations/{location}``,
+            ``folders/{folder}/locations/{location}``, or
+            ``projects/{project}/locations/{location}``
         page_size (int):
             Optional. The maximum number of modules to
             return. The service may return fewer than this
             value. If unspecified, at most 10 configs will
             be returned. The maximum value is 1000; values
             above 1000 will be coerced to 1000.
         page_token (str):
@@ -1462,20 +1602,18 @@
 
 class ListDescendantEventThreatDetectionCustomModulesRequest(proto.Message):
     r"""Request message for listing descendant Event Threat Detection
     custom modules.
 
     Attributes:
         parent (str):
-            Required. Name of parent to list custom
-            modules. Its format is
-            "organizations/{organization}/locations/{location}",
-            "folders/{folder}/locations/{location}",
-            or
-            "projects/{project}/locations/{location}".
+            Required. Name of parent to list custom modules. Its format
+            is ``organizations/{organization}/locations/{location}``,
+            ``folders/{folder}/locations/{location}``, or
+            ``projects/{project}/locations/{location}``
         page_size (int):
             Optional. The maximum number of modules to
             return. The service may return fewer than this
             value. If unspecified, at most 10 configs will
             be returned. The maximum value is 1000; values
             above 1000 will be coerced to 1000.
         page_token (str):
@@ -1531,36 +1669,34 @@
 
     Attributes:
         name (str):
             Required. The resource name of the ETD custom module.
 
             Its format is:
 
-            -  "organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-            -  "folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-            -  "projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
+            -  ``organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+            -  ``folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+            -  ``projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class CreateEventThreatDetectionCustomModuleRequest(proto.Message):
     r"""Message for creating a EventThreatDetectionCustomModule
 
     Attributes:
         parent (str):
-            Required. Name of parent for the module. Its
-            format is
-            "organizations/{organization}/locations/{location}",
-            "folders/{folder}/locations/{location}",
-            or
-            "projects/{project}/locations/{location}".
+            Required. Name of parent for the module. Its format is
+            ``organizations/{organization}/locations/{location}``,
+            ``folders/{folder}/locations/{location}``, or
+            ``projects/{project}/locations/{location}``
         event_threat_detection_custom_module (google.cloud.securitycentermanagement_v1.types.EventThreatDetectionCustomModule):
             Required. The module to create. The
             event_threat_detection_custom_module.name will be ignored
             and server generated.
         validate_only (bool):
             Optional. When set to true, only validations
             (including IAM checks) will done for the request
@@ -1638,17 +1774,17 @@
 
     Attributes:
         name (str):
             Required. The resource name of the ETD custom module.
 
             Its format is:
 
-            -  "organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-            -  "folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
-            -  "projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}".
+            -  ``organizations/{organization}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+            -  ``folders/{folder}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
+            -  ``projects/{project}/locations/{location}/eventThreatDetectionCustomModules/{event_threat_detection_custom_module}``.
         validate_only (bool):
             Optional. When set to true, only validations
             (including IAM checks) will done for the request
             (module will not be deleted). An OK response
             indicates the request is valid while an error
             response indicates the request is invalid. Note
             that a subsequent request to actually delete the
@@ -1673,15 +1809,15 @@
     Attributes:
         parent (str):
             Required. Resource name of the parent to validate the Custom
             Module under.
 
             Its format is:
 
-            -  "organizations/{organization}/locations/{location}".
+            -  ``organizations/{organization}/locations/{location}``.
         raw_text (str):
             Required. The raw text of the module's
             contents. Used to generate error messages.
         type_ (str):
             Required. The type of the module (e.g. CONFIGURABLE_BAD_IP).
     """
 
@@ -1785,8 +1921,144 @@
     errors: MutableSequence[CustomModuleValidationError] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=CustomModuleValidationError,
     )
 
 
+class GetSecurityCenterServiceRequest(proto.Message):
+    r"""Request message for getting a Security Command Center
+    service.
+
+    Attributes:
+        name (str):
+            Required. The Security Command Center service to retrieve.
+
+            Formats:
+
+            -  organizations/{organization}/locations/{location}/securityCenterServices/{service}
+            -  folders/{folder}/locations/{location}/securityCenterServices/{service}
+            -  projects/{project}/locations/{location}/securityCenterServices/{service}
+
+            The possible values for id {service} are:
+
+            -  container-threat-detection
+            -  event-threat-detection
+            -  security-health-analytics
+            -  vm-threat-detection
+            -  web-security-scanner
+    """
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
+class ListSecurityCenterServicesRequest(proto.Message):
+    r"""Request message for listing Security Command Center services.
+
+    Attributes:
+        parent (str):
+            Required. The name of the parent to list Security Command
+            Center services.
+
+            Formats:
+
+            -  organizations/{organization}/locations/{location}
+            -  folders/{folder}/locations/{location}
+            -  projects/{project}/locations/{location}
+        page_size (int):
+            Optional. The maximum number of results to
+            return in a single response. Default is 10,
+            minimum is 1, maximum is 1000.
+        page_token (str):
+            Optional. The value returned by the last call
+            indicating a continuation.
+    """
+
+    parent: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    page_size: int = proto.Field(
+        proto.INT32,
+        number=2,
+    )
+    page_token: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+
+
+class ListSecurityCenterServicesResponse(proto.Message):
+    r"""Response message for listing Security Command Center
+    services.
+
+    Attributes:
+        security_center_services (MutableSequence[google.cloud.securitycentermanagement_v1.types.SecurityCenterService]):
+            The list of services.
+        next_page_token (str):
+            A token identifying a page of results the
+            server should return.
+    """
+
+    @property
+    def raw_page(self):
+        return self
+
+    security_center_services: MutableSequence[
+        "SecurityCenterService"
+    ] = proto.RepeatedField(
+        proto.MESSAGE,
+        number=1,
+        message="SecurityCenterService",
+    )
+    next_page_token: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+
+
+class UpdateSecurityCenterServiceRequest(proto.Message):
+    r"""Request message for updating a Security Command Center
+    service.
+
+    Attributes:
+        security_center_service (google.cloud.securitycentermanagement_v1.types.SecurityCenterService):
+            Required. The updated service.
+        update_mask (google.protobuf.field_mask_pb2.FieldMask):
+            Required. The list of fields to be updated. Possible values:
+
+            -  "intended_enablement_state"
+            -  "modules".
+        validate_only (bool):
+            Optional. When set to true, only validations
+            (including IAM checks) will done for the request
+            (service will not be updated). An OK response
+            indicates the request is valid while an error
+            response indicates the request is invalid. Note
+            that a subsequent request to actually update the
+            service could still fail because:
+
+            1. The state could have changed (e.g. IAM permission lost) or
+            2. A failure occurred while trying to delete the
+               module.
+    """
+
+    security_center_service: "SecurityCenterService" = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message="SecurityCenterService",
+    )
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=field_mask_pb2.FieldMask,
+    )
+    validate_only: bool = proto.Field(
+        proto.BOOL,
+        number=3,
+    )
+
+
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google_cloud_securitycentermanagement.egg-info/PKG-INFO` & `google-cloud-securitycentermanagement-0.1.9/google_cloud_securitycentermanagement.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-securitycentermanagement
-Version: 0.1.8
+Version: 0.1.9
 Summary: Google Cloud Securitycentermanagement API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-securitycentermanagement
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-securitycentermanagement-0.1.8/google_cloud_securitycentermanagement.egg-info/SOURCES.txt` & `google-cloud-securitycentermanagement-0.1.9/google_cloud_securitycentermanagement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycentermanagement-0.1.8/setup.py` & `google-cloud-securitycentermanagement-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycentermanagement-0.1.8/tests/__init__.py` & `google-cloud-securitycentermanagement-0.1.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycentermanagement-0.1.8/tests/unit/__init__.py` & `google-cloud-securitycentermanagement-0.1.9/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycentermanagement-0.1.8/tests/unit/gapic/__init__.py` & `google-cloud-securitycentermanagement-0.1.9/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycentermanagement-0.1.8/tests/unit/gapic/securitycentermanagement_v1/__init__.py` & `google-cloud-securitycentermanagement-0.1.9/tests/unit/gapic/securitycentermanagement_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-securitycentermanagement-0.1.8/tests/unit/gapic/securitycentermanagement_v1/test_security_center_management.py` & `google-cloud-securitycentermanagement-0.1.9/tests/unit/gapic/securitycentermanagement_v1/test_security_center_management.py`

 * *Files 21% similar despite different names*

```diff
@@ -1231,18 +1231,18 @@
         response = client.list_effective_security_health_analytics_custom_modules(
             request
         )
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest()
+        request = (
+            security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListEffectiveSecurityHealthAnalyticsCustomModulesPager
     )
     assert response.next_page_token == "next_page_token_value"
 
@@ -1256,23 +1256,178 @@
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_effective_security_health_analytics_custom_modules),
         "__call__",
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_effective_security_health_analytics_custom_modules()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest()
         )
 
 
+def test_list_effective_security_health_analytics_custom_modules_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_effective_security_health_analytics_custom_modules),
+        "__call__",
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.list_effective_security_health_analytics_custom_modules(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+        )
+
+
+def test_list_effective_security_health_analytics_custom_modules_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_effective_security_health_analytics_custom_modules
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_effective_security_health_analytics_custom_modules
+        ] = mock_rpc
+        request = {}
+        client.list_effective_security_health_analytics_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_effective_security_health_analytics_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_list_effective_security_health_analytics_custom_modules_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_effective_security_health_analytics_custom_modules),
+        "__call__",
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = (
+            await client.list_effective_security_health_analytics_custom_modules()
+        )
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_effective_security_health_analytics_custom_modules_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.list_effective_security_health_analytics_custom_modules
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
+            client._client._transport.list_effective_security_health_analytics_custom_modules
+        ] = mock_object
+
+        request = {}
+        await client.list_effective_security_health_analytics_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_effective_security_health_analytics_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_effective_security_health_analytics_custom_modules_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1297,18 +1452,18 @@
         response = await client.list_effective_security_health_analytics_custom_modules(
             request
         )
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest()
+        request = (
+            security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListEffectiveSecurityHealthAnalyticsCustomModulesAsyncPager
     )
     assert response.next_page_token == "next_page_token_value"
 
@@ -1742,18 +1897,18 @@
             display_name="display_name_value",
         )
         response = client.get_effective_security_health_analytics_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest()
+        request = (
+            security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response,
         security_center_management.EffectiveSecurityHealthAnalyticsCustomModule,
     )
     assert response.name == "name_value"
@@ -1773,23 +1928,176 @@
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_effective_security_health_analytics_custom_module),
         "__call__",
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_effective_security_health_analytics_custom_module()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest()
         )
 
 
+def test_get_effective_security_health_analytics_custom_module_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_effective_security_health_analytics_custom_module),
+        "__call__",
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.get_effective_security_health_analytics_custom_module(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest(
+            name="name_value",
+        )
+
+
+def test_get_effective_security_health_analytics_custom_module_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.get_effective_security_health_analytics_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_effective_security_health_analytics_custom_module
+        ] = mock_rpc
+        request = {}
+        client.get_effective_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_effective_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_get_effective_security_health_analytics_custom_module_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_effective_security_health_analytics_custom_module),
+        "__call__",
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.EffectiveSecurityHealthAnalyticsCustomModule(
+                name="name_value",
+                enablement_state=security_center_management.EffectiveSecurityHealthAnalyticsCustomModule.EnablementState.ENABLED,
+                display_name="display_name_value",
+            )
+        )
+        response = await client.get_effective_security_health_analytics_custom_module()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_effective_security_health_analytics_custom_module_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.get_effective_security_health_analytics_custom_module
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
+            client._client._transport.get_effective_security_health_analytics_custom_module
+        ] = mock_object
+
+        request = {}
+        await client.get_effective_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_effective_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_effective_security_health_analytics_custom_module_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1816,18 +2124,18 @@
         response = await client.get_effective_security_health_analytics_custom_module(
             request
         )
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest()
+        request = (
+            security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response,
         security_center_management.EffectiveSecurityHealthAnalyticsCustomModule,
     )
     assert response.name == "name_value"
@@ -2040,18 +2348,18 @@
             )
         )
         response = client.list_security_health_analytics_custom_modules(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest()
+        request = (
+            security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListSecurityHealthAnalyticsCustomModulesPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_list_security_health_analytics_custom_modules_empty_call():
@@ -2062,23 +2370,176 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_security_health_analytics_custom_modules), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_security_health_analytics_custom_modules()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest()
         )
 
 
+def test_list_security_health_analytics_custom_modules_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = (
+        security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+        )
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_health_analytics_custom_modules), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.list_security_health_analytics_custom_modules(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+        )
+
+
+def test_list_security_health_analytics_custom_modules_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_security_health_analytics_custom_modules
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_security_health_analytics_custom_modules
+        ] = mock_rpc
+        request = {}
+        client.list_security_health_analytics_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_security_health_analytics_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_list_security_health_analytics_custom_modules_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_health_analytics_custom_modules), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.ListSecurityHealthAnalyticsCustomModulesResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.list_security_health_analytics_custom_modules()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_security_health_analytics_custom_modules_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.list_security_health_analytics_custom_modules
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
+            client._client._transport.list_security_health_analytics_custom_modules
+        ] = mock_object
+
+        request = {}
+        await client.list_security_health_analytics_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_security_health_analytics_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_security_health_analytics_custom_modules_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2100,18 +2561,18 @@
             )
         )
         response = await client.list_security_health_analytics_custom_modules(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest()
+        request = (
+            security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListSecurityHealthAnalyticsCustomModulesAsyncPager
     )
     assert response.next_page_token == "next_page_token_value"
 
@@ -2527,18 +2988,18 @@
         response = client.list_descendant_security_health_analytics_custom_modules(
             request
         )
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest()
+        request = (
+            security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListDescendantSecurityHealthAnalyticsCustomModulesPager
     )
     assert response.next_page_token == "next_page_token_value"
 
@@ -2552,23 +3013,178 @@
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_descendant_security_health_analytics_custom_modules),
         "__call__",
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_descendant_security_health_analytics_custom_modules()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest()
         )
 
 
+def test_list_descendant_security_health_analytics_custom_modules_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_descendant_security_health_analytics_custom_modules),
+        "__call__",
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.list_descendant_security_health_analytics_custom_modules(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+        )
+
+
+def test_list_descendant_security_health_analytics_custom_modules_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_descendant_security_health_analytics_custom_modules
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_descendant_security_health_analytics_custom_modules
+        ] = mock_rpc
+        request = {}
+        client.list_descendant_security_health_analytics_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_descendant_security_health_analytics_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_list_descendant_security_health_analytics_custom_modules_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_descendant_security_health_analytics_custom_modules),
+        "__call__",
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = (
+            await client.list_descendant_security_health_analytics_custom_modules()
+        )
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_descendant_security_health_analytics_custom_modules_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.list_descendant_security_health_analytics_custom_modules
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
+            client._client._transport.list_descendant_security_health_analytics_custom_modules
+        ] = mock_object
+
+        request = {}
+        await client.list_descendant_security_health_analytics_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_descendant_security_health_analytics_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_descendant_security_health_analytics_custom_modules_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2595,18 +3211,18 @@
                 request
             )
         )
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest()
+        request = (
+            security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListDescendantSecurityHealthAnalyticsCustomModulesAsyncPager
     )
     assert response.next_page_token == "next_page_token_value"
 
@@ -3041,18 +3657,18 @@
             ancestor_module="ancestor_module_value",
         )
         response = client.get_security_health_analytics_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest()
+        request = (
+            security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.SecurityHealthAnalyticsCustomModule
     )
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
@@ -3072,23 +3688,176 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_security_health_analytics_custom_module), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_security_health_analytics_custom_module()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest()
         )
 
 
+def test_get_security_health_analytics_custom_module_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_security_health_analytics_custom_module), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.get_security_health_analytics_custom_module(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest(
+            name="name_value",
+        )
+
+
+def test_get_security_health_analytics_custom_module_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.get_security_health_analytics_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_security_health_analytics_custom_module
+        ] = mock_rpc
+        request = {}
+        client.get_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_get_security_health_analytics_custom_module_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_security_health_analytics_custom_module), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.SecurityHealthAnalyticsCustomModule(
+                name="name_value",
+                display_name="display_name_value",
+                enablement_state=security_center_management.SecurityHealthAnalyticsCustomModule.EnablementState.ENABLED,
+                last_editor="last_editor_value",
+                ancestor_module="ancestor_module_value",
+            )
+        )
+        response = await client.get_security_health_analytics_custom_module()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_security_health_analytics_custom_module_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.get_security_health_analytics_custom_module
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
+            client._client._transport.get_security_health_analytics_custom_module
+        ] = mock_object
+
+        request = {}
+        await client.get_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_security_health_analytics_custom_module_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3114,18 +3883,18 @@
             )
         )
         response = await client.get_security_health_analytics_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest()
+        request = (
+            security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.SecurityHealthAnalyticsCustomModule
     )
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
@@ -3332,18 +4101,18 @@
             ancestor_module="ancestor_module_value",
         )
         response = client.create_security_health_analytics_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest()
+        request = (
+            security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.SecurityHealthAnalyticsCustomModule
     )
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
@@ -3364,23 +4133,180 @@
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_security_health_analytics_custom_module),
         "__call__",
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_security_health_analytics_custom_module()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest()
         )
 
 
+def test_create_security_health_analytics_custom_module_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = (
+        security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest(
+            parent="parent_value",
+        )
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_security_health_analytics_custom_module),
+        "__call__",
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.create_security_health_analytics_custom_module(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest(
+            parent="parent_value",
+        )
+
+
+def test_create_security_health_analytics_custom_module_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.create_security_health_analytics_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_security_health_analytics_custom_module
+        ] = mock_rpc
+        request = {}
+        client.create_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_create_security_health_analytics_custom_module_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_security_health_analytics_custom_module),
+        "__call__",
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.SecurityHealthAnalyticsCustomModule(
+                name="name_value",
+                display_name="display_name_value",
+                enablement_state=security_center_management.SecurityHealthAnalyticsCustomModule.EnablementState.ENABLED,
+                last_editor="last_editor_value",
+                ancestor_module="ancestor_module_value",
+            )
+        )
+        response = await client.create_security_health_analytics_custom_module()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_create_security_health_analytics_custom_module_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.create_security_health_analytics_custom_module
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
+            client._client._transport.create_security_health_analytics_custom_module
+        ] = mock_object
+
+        request = {}
+        await client.create_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.create_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_security_health_analytics_custom_module_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3407,18 +4333,18 @@
             )
         )
         response = await client.create_security_health_analytics_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest()
+        request = (
+            security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.SecurityHealthAnalyticsCustomModule
     )
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
@@ -3655,18 +4581,18 @@
             ancestor_module="ancestor_module_value",
         )
         response = client.update_security_health_analytics_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest()
+        request = (
+            security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.SecurityHealthAnalyticsCustomModule
     )
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
@@ -3687,23 +4613,177 @@
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_security_health_analytics_custom_module),
         "__call__",
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_security_health_analytics_custom_module()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest()
         )
 
 
+def test_update_security_health_analytics_custom_module_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = (
+        security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest()
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_security_health_analytics_custom_module),
+        "__call__",
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.update_security_health_analytics_custom_module(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest()
+        )
+
+
+def test_update_security_health_analytics_custom_module_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.update_security_health_analytics_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_security_health_analytics_custom_module
+        ] = mock_rpc
+        request = {}
+        client.update_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_update_security_health_analytics_custom_module_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_security_health_analytics_custom_module),
+        "__call__",
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.SecurityHealthAnalyticsCustomModule(
+                name="name_value",
+                display_name="display_name_value",
+                enablement_state=security_center_management.SecurityHealthAnalyticsCustomModule.EnablementState.ENABLED,
+                last_editor="last_editor_value",
+                ancestor_module="ancestor_module_value",
+            )
+        )
+        response = await client.update_security_health_analytics_custom_module()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_update_security_health_analytics_custom_module_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.update_security_health_analytics_custom_module
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
+            client._client._transport.update_security_health_analytics_custom_module
+        ] = mock_object
+
+        request = {}
+        await client.update_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.update_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_security_health_analytics_custom_module_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3730,18 +4810,18 @@
             )
         )
         response = await client.update_security_health_analytics_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest()
+        request = (
+            security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.SecurityHealthAnalyticsCustomModule
     )
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
@@ -3972,18 +5052,18 @@
         # Designate an appropriate return value for the call.
         call.return_value = None
         response = client.delete_security_health_analytics_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest()
+        request = (
+            security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 def test_delete_security_health_analytics_custom_module_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -3994,23 +5074,172 @@
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_security_health_analytics_custom_module),
         "__call__",
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_security_health_analytics_custom_module()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest()
         )
 
 
+def test_delete_security_health_analytics_custom_module_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = (
+        security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest(
+            name="name_value",
+        )
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_security_health_analytics_custom_module),
+        "__call__",
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.delete_security_health_analytics_custom_module(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest(
+            name="name_value",
+        )
+
+
+def test_delete_security_health_analytics_custom_module_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.delete_security_health_analytics_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_security_health_analytics_custom_module
+        ] = mock_rpc
+        request = {}
+        client.delete_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_delete_security_health_analytics_custom_module_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_security_health_analytics_custom_module),
+        "__call__",
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.delete_security_health_analytics_custom_module()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_delete_security_health_analytics_custom_module_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.delete_security_health_analytics_custom_module
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
+            client._client._transport.delete_security_health_analytics_custom_module
+        ] = mock_object
+
+        request = {}
+        await client.delete_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.delete_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_security_health_analytics_custom_module_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -4029,18 +5258,18 @@
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         response = await client.delete_security_health_analytics_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest()
+        request = (
+            security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
 async def test_delete_security_health_analytics_custom_module_async_from_dict():
@@ -4231,18 +5460,18 @@
             security_center_management.SimulateSecurityHealthAnalyticsCustomModuleResponse()
         )
         response = client.simulate_security_health_analytics_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest()
+        request = (
+            security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response,
         security_center_management.SimulateSecurityHealthAnalyticsCustomModuleResponse,
     )
 
@@ -4256,23 +5485,174 @@
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.simulate_security_health_analytics_custom_module),
         "__call__",
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.simulate_security_health_analytics_custom_module()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest()
         )
 
 
+def test_simulate_security_health_analytics_custom_module_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = (
+        security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest(
+            parent="parent_value",
+        )
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.simulate_security_health_analytics_custom_module),
+        "__call__",
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.simulate_security_health_analytics_custom_module(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest(
+            parent="parent_value",
+        )
+
+
+def test_simulate_security_health_analytics_custom_module_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.simulate_security_health_analytics_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.simulate_security_health_analytics_custom_module
+        ] = mock_rpc
+        request = {}
+        client.simulate_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.simulate_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_simulate_security_health_analytics_custom_module_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.simulate_security_health_analytics_custom_module),
+        "__call__",
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.SimulateSecurityHealthAnalyticsCustomModuleResponse()
+        )
+        response = await client.simulate_security_health_analytics_custom_module()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_simulate_security_health_analytics_custom_module_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.simulate_security_health_analytics_custom_module
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
+            client._client._transport.simulate_security_health_analytics_custom_module
+        ] = mock_object
+
+        request = {}
+        await client.simulate_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.simulate_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_simulate_security_health_analytics_custom_module_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -4295,18 +5675,18 @@
         response = await client.simulate_security_health_analytics_custom_module(
             request
         )
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest()
+        request = (
+            security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response,
         security_center_management.SimulateSecurityHealthAnalyticsCustomModuleResponse,
     )
 
@@ -4554,18 +5934,18 @@
             next_page_token="next_page_token_value",
         )
         response = client.list_effective_event_threat_detection_custom_modules(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest()
+        request = (
+            security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListEffectiveEventThreatDetectionCustomModulesPager
     )
     assert response.next_page_token == "next_page_token_value"
 
@@ -4579,23 +5959,176 @@
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_effective_event_threat_detection_custom_modules),
         "__call__",
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_effective_event_threat_detection_custom_modules()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest()
         )
 
 
+def test_list_effective_event_threat_detection_custom_modules_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_effective_event_threat_detection_custom_modules),
+        "__call__",
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.list_effective_event_threat_detection_custom_modules(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+        )
+
+
+def test_list_effective_event_threat_detection_custom_modules_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_effective_event_threat_detection_custom_modules
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_effective_event_threat_detection_custom_modules
+        ] = mock_rpc
+        request = {}
+        client.list_effective_event_threat_detection_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_effective_event_threat_detection_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_list_effective_event_threat_detection_custom_modules_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_effective_event_threat_detection_custom_modules),
+        "__call__",
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.ListEffectiveEventThreatDetectionCustomModulesResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.list_effective_event_threat_detection_custom_modules()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_effective_event_threat_detection_custom_modules_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.list_effective_event_threat_detection_custom_modules
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
+            client._client._transport.list_effective_event_threat_detection_custom_modules
+        ] = mock_object
+
+        request = {}
+        await client.list_effective_event_threat_detection_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_effective_event_threat_detection_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_effective_event_threat_detection_custom_modules_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -4620,18 +6153,18 @@
         response = await client.list_effective_event_threat_detection_custom_modules(
             request
         )
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest()
+        request = (
+            security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListEffectiveEventThreatDetectionCustomModulesAsyncPager
     )
     assert response.next_page_token == "next_page_token_value"
 
@@ -5061,18 +6594,18 @@
             description="description_value",
         )
         response = client.get_effective_event_threat_detection_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest()
+        request = (
+            security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.EffectiveEventThreatDetectionCustomModule
     )
     assert response.name == "name_value"
     assert (
@@ -5093,23 +6626,180 @@
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_effective_event_threat_detection_custom_module),
         "__call__",
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_effective_event_threat_detection_custom_module()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest()
         )
 
 
+def test_get_effective_event_threat_detection_custom_module_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = (
+        security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest(
+            name="name_value",
+        )
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_effective_event_threat_detection_custom_module),
+        "__call__",
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.get_effective_event_threat_detection_custom_module(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest(
+            name="name_value",
+        )
+
+
+def test_get_effective_event_threat_detection_custom_module_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.get_effective_event_threat_detection_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_effective_event_threat_detection_custom_module
+        ] = mock_rpc
+        request = {}
+        client.get_effective_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_effective_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_get_effective_event_threat_detection_custom_module_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_effective_event_threat_detection_custom_module),
+        "__call__",
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.EffectiveEventThreatDetectionCustomModule(
+                name="name_value",
+                enablement_state=security_center_management.EffectiveEventThreatDetectionCustomModule.EnablementState.ENABLED,
+                type_="type__value",
+                display_name="display_name_value",
+                description="description_value",
+            )
+        )
+        response = await client.get_effective_event_threat_detection_custom_module()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_effective_event_threat_detection_custom_module_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.get_effective_event_threat_detection_custom_module
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
+            client._client._transport.get_effective_event_threat_detection_custom_module
+        ] = mock_object
+
+        request = {}
+        await client.get_effective_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_effective_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_effective_event_threat_detection_custom_module_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -5138,18 +6828,18 @@
         response = await client.get_effective_event_threat_detection_custom_module(
             request
         )
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest()
+        request = (
+            security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.EffectiveEventThreatDetectionCustomModule
     )
     assert response.name == "name_value"
     assert (
@@ -5363,18 +7053,18 @@
             )
         )
         response = client.list_event_threat_detection_custom_modules(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ListEventThreatDetectionCustomModulesRequest()
+        request = (
+            security_center_management.ListEventThreatDetectionCustomModulesRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListEventThreatDetectionCustomModulesPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_list_event_threat_detection_custom_modules_empty_call():
@@ -5385,23 +7075,174 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_event_threat_detection_custom_modules), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_event_threat_detection_custom_modules()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.ListEventThreatDetectionCustomModulesRequest()
         )
 
 
+def test_list_event_threat_detection_custom_modules_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.ListEventThreatDetectionCustomModulesRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_event_threat_detection_custom_modules), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.list_event_threat_detection_custom_modules(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.ListEventThreatDetectionCustomModulesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+        )
+
+
+def test_list_event_threat_detection_custom_modules_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_event_threat_detection_custom_modules
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_event_threat_detection_custom_modules
+        ] = mock_rpc
+        request = {}
+        client.list_event_threat_detection_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_event_threat_detection_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_list_event_threat_detection_custom_modules_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_event_threat_detection_custom_modules), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.ListEventThreatDetectionCustomModulesResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.list_event_threat_detection_custom_modules()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.ListEventThreatDetectionCustomModulesRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_event_threat_detection_custom_modules_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.list_event_threat_detection_custom_modules
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
+            client._client._transport.list_event_threat_detection_custom_modules
+        ] = mock_object
+
+        request = {}
+        await client.list_event_threat_detection_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_event_threat_detection_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_event_threat_detection_custom_modules_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.ListEventThreatDetectionCustomModulesRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -5423,18 +7264,18 @@
             )
         )
         response = await client.list_event_threat_detection_custom_modules(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ListEventThreatDetectionCustomModulesRequest()
+        request = (
+            security_center_management.ListEventThreatDetectionCustomModulesRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListEventThreatDetectionCustomModulesAsyncPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 @pytest.mark.asyncio
@@ -5834,18 +7675,18 @@
             next_page_token="next_page_token_value",
         )
         response = client.list_descendant_event_threat_detection_custom_modules(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest()
+        request = (
+            security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListDescendantEventThreatDetectionCustomModulesPager
     )
     assert response.next_page_token == "next_page_token_value"
 
@@ -5859,23 +7700,176 @@
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_descendant_event_threat_detection_custom_modules),
         "__call__",
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_descendant_event_threat_detection_custom_modules()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest()
         )
 
 
+def test_list_descendant_event_threat_detection_custom_modules_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_descendant_event_threat_detection_custom_modules),
+        "__call__",
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.list_descendant_event_threat_detection_custom_modules(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+        )
+
+
+def test_list_descendant_event_threat_detection_custom_modules_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_descendant_event_threat_detection_custom_modules
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_descendant_event_threat_detection_custom_modules
+        ] = mock_rpc
+        request = {}
+        client.list_descendant_event_threat_detection_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_descendant_event_threat_detection_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_list_descendant_event_threat_detection_custom_modules_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_descendant_event_threat_detection_custom_modules),
+        "__call__",
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.ListDescendantEventThreatDetectionCustomModulesResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.list_descendant_event_threat_detection_custom_modules()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_descendant_event_threat_detection_custom_modules_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.list_descendant_event_threat_detection_custom_modules
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
+            client._client._transport.list_descendant_event_threat_detection_custom_modules
+        ] = mock_object
+
+        request = {}
+        await client.list_descendant_event_threat_detection_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_descendant_event_threat_detection_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_descendant_event_threat_detection_custom_modules_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -5900,18 +7894,18 @@
         response = await client.list_descendant_event_threat_detection_custom_modules(
             request
         )
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest()
+        request = (
+            security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListDescendantEventThreatDetectionCustomModulesAsyncPager
     )
     assert response.next_page_token == "next_page_token_value"
 
@@ -6340,18 +8334,18 @@
             last_editor="last_editor_value",
         )
         response = client.get_event_threat_detection_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.GetEventThreatDetectionCustomModuleRequest()
+        request = (
+            security_center_management.GetEventThreatDetectionCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.EventThreatDetectionCustomModule
     )
     assert response.name == "name_value"
     assert response.ancestor_module == "ancestor_module_value"
@@ -6373,23 +8367,178 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_event_threat_detection_custom_module), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_event_threat_detection_custom_module()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.GetEventThreatDetectionCustomModuleRequest()
         )
 
 
+def test_get_event_threat_detection_custom_module_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.GetEventThreatDetectionCustomModuleRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_event_threat_detection_custom_module), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.get_event_threat_detection_custom_module(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.GetEventThreatDetectionCustomModuleRequest(
+            name="name_value",
+        )
+
+
+def test_get_event_threat_detection_custom_module_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.get_event_threat_detection_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_event_threat_detection_custom_module
+        ] = mock_rpc
+        request = {}
+        client.get_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_get_event_threat_detection_custom_module_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_event_threat_detection_custom_module), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.EventThreatDetectionCustomModule(
+                name="name_value",
+                ancestor_module="ancestor_module_value",
+                enablement_state=security_center_management.EventThreatDetectionCustomModule.EnablementState.ENABLED,
+                type_="type__value",
+                display_name="display_name_value",
+                description="description_value",
+                last_editor="last_editor_value",
+            )
+        )
+        response = await client.get_event_threat_detection_custom_module()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.GetEventThreatDetectionCustomModuleRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_event_threat_detection_custom_module_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.get_event_threat_detection_custom_module
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
+            client._client._transport.get_event_threat_detection_custom_module
+        ] = mock_object
+
+        request = {}
+        await client.get_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_event_threat_detection_custom_module_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.GetEventThreatDetectionCustomModuleRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -6417,18 +8566,18 @@
             )
         )
         response = await client.get_event_threat_detection_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.GetEventThreatDetectionCustomModuleRequest()
+        request = (
+            security_center_management.GetEventThreatDetectionCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.EventThreatDetectionCustomModule
     )
     assert response.name == "name_value"
     assert response.ancestor_module == "ancestor_module_value"
@@ -6638,18 +8787,18 @@
             last_editor="last_editor_value",
         )
         response = client.create_event_threat_detection_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.CreateEventThreatDetectionCustomModuleRequest()
+        request = (
+            security_center_management.CreateEventThreatDetectionCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.EventThreatDetectionCustomModule
     )
     assert response.name == "name_value"
     assert response.ancestor_module == "ancestor_module_value"
@@ -6671,23 +8820,178 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_event_threat_detection_custom_module), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_event_threat_detection_custom_module()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.CreateEventThreatDetectionCustomModuleRequest()
         )
 
 
+def test_create_event_threat_detection_custom_module_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.CreateEventThreatDetectionCustomModuleRequest(
+        parent="parent_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_event_threat_detection_custom_module), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.create_event_threat_detection_custom_module(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.CreateEventThreatDetectionCustomModuleRequest(
+            parent="parent_value",
+        )
+
+
+def test_create_event_threat_detection_custom_module_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.create_event_threat_detection_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_event_threat_detection_custom_module
+        ] = mock_rpc
+        request = {}
+        client.create_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_create_event_threat_detection_custom_module_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_event_threat_detection_custom_module), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.EventThreatDetectionCustomModule(
+                name="name_value",
+                ancestor_module="ancestor_module_value",
+                enablement_state=security_center_management.EventThreatDetectionCustomModule.EnablementState.ENABLED,
+                type_="type__value",
+                display_name="display_name_value",
+                description="description_value",
+                last_editor="last_editor_value",
+            )
+        )
+        response = await client.create_event_threat_detection_custom_module()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.CreateEventThreatDetectionCustomModuleRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_create_event_threat_detection_custom_module_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.create_event_threat_detection_custom_module
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
+            client._client._transport.create_event_threat_detection_custom_module
+        ] = mock_object
+
+        request = {}
+        await client.create_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.create_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_event_threat_detection_custom_module_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.CreateEventThreatDetectionCustomModuleRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -6715,18 +9019,18 @@
             )
         )
         response = await client.create_event_threat_detection_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.CreateEventThreatDetectionCustomModuleRequest()
+        request = (
+            security_center_management.CreateEventThreatDetectionCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.EventThreatDetectionCustomModule
     )
     assert response.name == "name_value"
     assert response.ancestor_module == "ancestor_module_value"
@@ -6958,18 +9262,18 @@
             last_editor="last_editor_value",
         )
         response = client.update_event_threat_detection_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.UpdateEventThreatDetectionCustomModuleRequest()
+        request = (
+            security_center_management.UpdateEventThreatDetectionCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.EventThreatDetectionCustomModule
     )
     assert response.name == "name_value"
     assert response.ancestor_module == "ancestor_module_value"
@@ -6991,23 +9295,175 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_event_threat_detection_custom_module), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_event_threat_detection_custom_module()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.UpdateEventThreatDetectionCustomModuleRequest()
         )
 
 
+def test_update_event_threat_detection_custom_module_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.UpdateEventThreatDetectionCustomModuleRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_event_threat_detection_custom_module), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.update_event_threat_detection_custom_module(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.UpdateEventThreatDetectionCustomModuleRequest()
+        )
+
+
+def test_update_event_threat_detection_custom_module_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.update_event_threat_detection_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_event_threat_detection_custom_module
+        ] = mock_rpc
+        request = {}
+        client.update_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_update_event_threat_detection_custom_module_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_event_threat_detection_custom_module), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.EventThreatDetectionCustomModule(
+                name="name_value",
+                ancestor_module="ancestor_module_value",
+                enablement_state=security_center_management.EventThreatDetectionCustomModule.EnablementState.ENABLED,
+                type_="type__value",
+                display_name="display_name_value",
+                description="description_value",
+                last_editor="last_editor_value",
+            )
+        )
+        response = await client.update_event_threat_detection_custom_module()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.UpdateEventThreatDetectionCustomModuleRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_update_event_threat_detection_custom_module_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.update_event_threat_detection_custom_module
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
+            client._client._transport.update_event_threat_detection_custom_module
+        ] = mock_object
+
+        request = {}
+        await client.update_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.update_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_event_threat_detection_custom_module_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.UpdateEventThreatDetectionCustomModuleRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -7035,18 +9491,18 @@
             )
         )
         response = await client.update_event_threat_detection_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.UpdateEventThreatDetectionCustomModuleRequest()
+        request = (
+            security_center_management.UpdateEventThreatDetectionCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, security_center_management.EventThreatDetectionCustomModule
     )
     assert response.name == "name_value"
     assert response.ancestor_module == "ancestor_module_value"
@@ -7270,18 +9726,18 @@
         # Designate an appropriate return value for the call.
         call.return_value = None
         response = client.delete_event_threat_detection_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.DeleteEventThreatDetectionCustomModuleRequest()
+        request = (
+            security_center_management.DeleteEventThreatDetectionCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 def test_delete_event_threat_detection_custom_module_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -7291,23 +9747,168 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_event_threat_detection_custom_module), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_event_threat_detection_custom_module()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.DeleteEventThreatDetectionCustomModuleRequest()
         )
 
 
+def test_delete_event_threat_detection_custom_module_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.DeleteEventThreatDetectionCustomModuleRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_event_threat_detection_custom_module), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.delete_event_threat_detection_custom_module(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.DeleteEventThreatDetectionCustomModuleRequest(
+            name="name_value",
+        )
+
+
+def test_delete_event_threat_detection_custom_module_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.delete_event_threat_detection_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_event_threat_detection_custom_module
+        ] = mock_rpc
+        request = {}
+        client.delete_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_delete_event_threat_detection_custom_module_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_event_threat_detection_custom_module), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.delete_event_threat_detection_custom_module()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.DeleteEventThreatDetectionCustomModuleRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_delete_event_threat_detection_custom_module_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.delete_event_threat_detection_custom_module
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
+            client._client._transport.delete_event_threat_detection_custom_module
+        ] = mock_object
+
+        request = {}
+        await client.delete_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.delete_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_event_threat_detection_custom_module_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.DeleteEventThreatDetectionCustomModuleRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -7325,18 +9926,18 @@
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         response = await client.delete_event_threat_detection_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.DeleteEventThreatDetectionCustomModuleRequest()
+        request = (
+            security_center_management.DeleteEventThreatDetectionCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
 async def test_delete_event_threat_detection_custom_module_async_from_dict():
@@ -7518,18 +10119,18 @@
             security_center_management.ValidateEventThreatDetectionCustomModuleResponse()
         )
         response = client.validate_event_threat_detection_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ValidateEventThreatDetectionCustomModuleRequest()
+        request = (
+            security_center_management.ValidateEventThreatDetectionCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response,
         security_center_management.ValidateEventThreatDetectionCustomModuleResponse,
     )
 
@@ -7542,23 +10143,176 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.validate_event_threat_detection_custom_module), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.validate_event_threat_detection_custom_module()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert (
             args[0]
             == security_center_management.ValidateEventThreatDetectionCustomModuleRequest()
         )
 
 
+def test_validate_event_threat_detection_custom_module_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = (
+        security_center_management.ValidateEventThreatDetectionCustomModuleRequest(
+            parent="parent_value",
+            raw_text="raw_text_value",
+            type_="type__value",
+        )
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.validate_event_threat_detection_custom_module), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.validate_event_threat_detection_custom_module(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[
+            0
+        ] == security_center_management.ValidateEventThreatDetectionCustomModuleRequest(
+            parent="parent_value",
+            raw_text="raw_text_value",
+            type_="type__value",
+        )
+
+
+def test_validate_event_threat_detection_custom_module_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.validate_event_threat_detection_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.validate_event_threat_detection_custom_module
+        ] = mock_rpc
+        request = {}
+        client.validate_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.validate_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_validate_event_threat_detection_custom_module_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.validate_event_threat_detection_custom_module), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.ValidateEventThreatDetectionCustomModuleResponse()
+        )
+        response = await client.validate_event_threat_detection_custom_module()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0]
+            == security_center_management.ValidateEventThreatDetectionCustomModuleRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_validate_event_threat_detection_custom_module_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.validate_event_threat_detection_custom_module
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
+            client._client._transport.validate_event_threat_detection_custom_module
+        ] = mock_object
+
+        request = {}
+        await client.validate_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.validate_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_validate_event_threat_detection_custom_module_async(
     transport: str = "grpc_asyncio",
     request_type=security_center_management.ValidateEventThreatDetectionCustomModuleRequest,
 ):
     client = SecurityCenterManagementAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -7578,18 +10332,18 @@
             security_center_management.ValidateEventThreatDetectionCustomModuleResponse()
         )
         response = await client.validate_event_threat_detection_custom_module(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert (
-            args[0]
-            == security_center_management.ValidateEventThreatDetectionCustomModuleRequest()
+        request = (
+            security_center_management.ValidateEventThreatDetectionCustomModuleRequest()
         )
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(
         response,
         security_center_management.ValidateEventThreatDetectionCustomModuleResponse,
     )
 
@@ -7669,14 +10423,1471 @@
         "parent=parent_value",
     ) in kw["metadata"]
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        security_center_management.GetSecurityCenterServiceRequest,
+        dict,
+    ],
+)
+def test_get_security_center_service(request_type, transport: str = "grpc"):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_security_center_service), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = security_center_management.SecurityCenterService(
+            name="name_value",
+            intended_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+            effective_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+        )
+        response = client.get_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        request = security_center_management.GetSecurityCenterServiceRequest()
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, security_center_management.SecurityCenterService)
+    assert response.name == "name_value"
+    assert (
+        response.intended_enablement_state
+        == security_center_management.SecurityCenterService.EnablementState.INHERITED
+    )
+    assert (
+        response.effective_enablement_state
+        == security_center_management.SecurityCenterService.EnablementState.INHERITED
+    )
+
+
+def test_get_security_center_service_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_security_center_service), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.get_security_center_service()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == security_center_management.GetSecurityCenterServiceRequest()
+
+
+def test_get_security_center_service_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.GetSecurityCenterServiceRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_security_center_service), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.get_security_center_service(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == security_center_management.GetSecurityCenterServiceRequest(
+            name="name_value",
+        )
+
+
+def test_get_security_center_service_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.get_security_center_service
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_security_center_service
+        ] = mock_rpc
+        request = {}
+        client.get_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_security_center_service(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_get_security_center_service_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_security_center_service), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.SecurityCenterService(
+                name="name_value",
+                intended_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+                effective_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+            )
+        )
+        response = await client.get_security_center_service()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == security_center_management.GetSecurityCenterServiceRequest()
+
+
+@pytest.mark.asyncio
+async def test_get_security_center_service_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.get_security_center_service
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
+            client._client._transport.get_security_center_service
+        ] = mock_object
+
+        request = {}
+        await client.get_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_security_center_service(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_get_security_center_service_async(
+    transport: str = "grpc_asyncio",
+    request_type=security_center_management.GetSecurityCenterServiceRequest,
+):
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_security_center_service), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.SecurityCenterService(
+                name="name_value",
+                intended_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+                effective_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+            )
+        )
+        response = await client.get_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        request = security_center_management.GetSecurityCenterServiceRequest()
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, security_center_management.SecurityCenterService)
+    assert response.name == "name_value"
+    assert (
+        response.intended_enablement_state
+        == security_center_management.SecurityCenterService.EnablementState.INHERITED
+    )
+    assert (
+        response.effective_enablement_state
+        == security_center_management.SecurityCenterService.EnablementState.INHERITED
+    )
+
+
+@pytest.mark.asyncio
+async def test_get_security_center_service_async_from_dict():
+    await test_get_security_center_service_async(request_type=dict)
+
+
+def test_get_security_center_service_field_headers():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = security_center_management.GetSecurityCenterServiceRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_security_center_service), "__call__"
+    ) as call:
+        call.return_value = security_center_management.SecurityCenterService()
+        client.get_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_security_center_service_field_headers_async():
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = security_center_management.GetSecurityCenterServiceRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_security_center_service), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.SecurityCenterService()
+        )
+        await client.get_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+def test_get_security_center_service_flattened():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_security_center_service), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = security_center_management.SecurityCenterService()
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.get_security_center_service(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+def test_get_security_center_service_flattened_error():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.get_security_center_service(
+            security_center_management.GetSecurityCenterServiceRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_security_center_service_flattened_async():
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_security_center_service), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = security_center_management.SecurityCenterService()
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.SecurityCenterService()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.get_security_center_service(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_get_security_center_service_flattened_error_async():
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.get_security_center_service(
+            security_center_management.GetSecurityCenterServiceRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        security_center_management.ListSecurityCenterServicesRequest,
+        dict,
+    ],
+)
+def test_list_security_center_services(request_type, transport: str = "grpc"):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = (
+            security_center_management.ListSecurityCenterServicesResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = client.list_security_center_services(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        request = security_center_management.ListSecurityCenterServicesRequest()
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, pagers.ListSecurityCenterServicesPager)
+    assert response.next_page_token == "next_page_token_value"
+
+
+def test_list_security_center_services_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.list_security_center_services()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == security_center_management.ListSecurityCenterServicesRequest()
+
+
+def test_list_security_center_services_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.ListSecurityCenterServicesRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.list_security_center_services(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == security_center_management.ListSecurityCenterServicesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+        )
+
+
+def test_list_security_center_services_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_security_center_services
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_security_center_services
+        ] = mock_rpc
+        request = {}
+        client.list_security_center_services(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_security_center_services(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_list_security_center_services_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.ListSecurityCenterServicesResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.list_security_center_services()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == security_center_management.ListSecurityCenterServicesRequest()
+
+
+@pytest.mark.asyncio
+async def test_list_security_center_services_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.list_security_center_services
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
+            client._client._transport.list_security_center_services
+        ] = mock_object
+
+        request = {}
+        await client.list_security_center_services(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_security_center_services(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_list_security_center_services_async(
+    transport: str = "grpc_asyncio",
+    request_type=security_center_management.ListSecurityCenterServicesRequest,
+):
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.ListSecurityCenterServicesResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.list_security_center_services(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        request = security_center_management.ListSecurityCenterServicesRequest()
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, pagers.ListSecurityCenterServicesAsyncPager)
+    assert response.next_page_token == "next_page_token_value"
+
+
+@pytest.mark.asyncio
+async def test_list_security_center_services_async_from_dict():
+    await test_list_security_center_services_async(request_type=dict)
+
+
+def test_list_security_center_services_field_headers():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = security_center_management.ListSecurityCenterServicesRequest()
+
+    request.parent = "parent_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services), "__call__"
+    ) as call:
+        call.return_value = (
+            security_center_management.ListSecurityCenterServicesResponse()
+        )
+        client.list_security_center_services(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_list_security_center_services_field_headers_async():
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = security_center_management.ListSecurityCenterServicesRequest()
+
+    request.parent = "parent_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.ListSecurityCenterServicesResponse()
+        )
+        await client.list_security_center_services(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
+
+
+def test_list_security_center_services_flattened():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = (
+            security_center_management.ListSecurityCenterServicesResponse()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.list_security_center_services(
+            parent="parent_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+
+
+def test_list_security_center_services_flattened_error():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.list_security_center_services(
+            security_center_management.ListSecurityCenterServicesRequest(),
+            parent="parent_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_security_center_services_flattened_async():
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = (
+            security_center_management.ListSecurityCenterServicesResponse()
+        )
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.ListSecurityCenterServicesResponse()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.list_security_center_services(
+            parent="parent_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_list_security_center_services_flattened_error_async():
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.list_security_center_services(
+            security_center_management.ListSecurityCenterServicesRequest(),
+            parent="parent_value",
+        )
+
+
+def test_list_security_center_services_pager(transport_name: str = "grpc"):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport_name,
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services), "__call__"
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                ],
+                next_page_token="abc",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[],
+                next_page_token="def",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                ],
+                next_page_token="ghi",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                ],
+            ),
+            RuntimeError,
+        )
+
+        metadata = ()
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", ""),)),
+        )
+        pager = client.list_security_center_services(request={})
+
+        assert pager._metadata == metadata
+
+        results = list(pager)
+        assert len(results) == 6
+        assert all(
+            isinstance(i, security_center_management.SecurityCenterService)
+            for i in results
+        )
+
+
+def test_list_security_center_services_pages(transport_name: str = "grpc"):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport_name,
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services), "__call__"
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                ],
+                next_page_token="abc",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[],
+                next_page_token="def",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                ],
+                next_page_token="ghi",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                ],
+            ),
+            RuntimeError,
+        )
+        pages = list(client.list_security_center_services(request={}).pages)
+        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
+            assert page_.raw_page.next_page_token == token
+
+
+@pytest.mark.asyncio
+async def test_list_security_center_services_async_pager():
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services),
+        "__call__",
+        new_callable=mock.AsyncMock,
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                ],
+                next_page_token="abc",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[],
+                next_page_token="def",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                ],
+                next_page_token="ghi",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                ],
+            ),
+            RuntimeError,
+        )
+        async_pager = await client.list_security_center_services(
+            request={},
+        )
+        assert async_pager.next_page_token == "abc"
+        responses = []
+        async for response in async_pager:  # pragma: no branch
+            responses.append(response)
+
+        assert len(responses) == 6
+        assert all(
+            isinstance(i, security_center_management.SecurityCenterService)
+            for i in responses
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_security_center_services_async_pages():
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_security_center_services),
+        "__call__",
+        new_callable=mock.AsyncMock,
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                ],
+                next_page_token="abc",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[],
+                next_page_token="def",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                ],
+                next_page_token="ghi",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                ],
+            ),
+            RuntimeError,
+        )
+        pages = []
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
+            await client.list_security_center_services(request={})
+        ).pages:
+            pages.append(page_)
+        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
+            assert page_.raw_page.next_page_token == token
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        security_center_management.UpdateSecurityCenterServiceRequest,
+        dict,
+    ],
+)
+def test_update_security_center_service(request_type, transport: str = "grpc"):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_security_center_service), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = security_center_management.SecurityCenterService(
+            name="name_value",
+            intended_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+            effective_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+        )
+        response = client.update_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        request = security_center_management.UpdateSecurityCenterServiceRequest()
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, security_center_management.SecurityCenterService)
+    assert response.name == "name_value"
+    assert (
+        response.intended_enablement_state
+        == security_center_management.SecurityCenterService.EnablementState.INHERITED
+    )
+    assert (
+        response.effective_enablement_state
+        == security_center_management.SecurityCenterService.EnablementState.INHERITED
+    )
+
+
+def test_update_security_center_service_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_security_center_service), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.update_security_center_service()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0] == security_center_management.UpdateSecurityCenterServiceRequest()
+        )
+
+
+def test_update_security_center_service_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = security_center_management.UpdateSecurityCenterServiceRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_security_center_service), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.update_security_center_service(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0] == security_center_management.UpdateSecurityCenterServiceRequest()
+        )
+
+
+def test_update_security_center_service_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.update_security_center_service
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_security_center_service
+        ] = mock_rpc
+        request = {}
+        client.update_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_security_center_service(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_update_security_center_service_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_security_center_service), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.SecurityCenterService(
+                name="name_value",
+                intended_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+                effective_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+            )
+        )
+        response = await client.update_security_center_service()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert (
+            args[0] == security_center_management.UpdateSecurityCenterServiceRequest()
+        )
+
+
+@pytest.mark.asyncio
+async def test_update_security_center_service_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementAsyncClient(
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
+            client._client._transport.update_security_center_service
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
+            client._client._transport.update_security_center_service
+        ] = mock_object
+
+        request = {}
+        await client.update_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.update_security_center_service(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_update_security_center_service_async(
+    transport: str = "grpc_asyncio",
+    request_type=security_center_management.UpdateSecurityCenterServiceRequest,
+):
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_security_center_service), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.SecurityCenterService(
+                name="name_value",
+                intended_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+                effective_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+            )
+        )
+        response = await client.update_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        request = security_center_management.UpdateSecurityCenterServiceRequest()
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, security_center_management.SecurityCenterService)
+    assert response.name == "name_value"
+    assert (
+        response.intended_enablement_state
+        == security_center_management.SecurityCenterService.EnablementState.INHERITED
+    )
+    assert (
+        response.effective_enablement_state
+        == security_center_management.SecurityCenterService.EnablementState.INHERITED
+    )
+
+
+@pytest.mark.asyncio
+async def test_update_security_center_service_async_from_dict():
+    await test_update_security_center_service_async(request_type=dict)
+
+
+def test_update_security_center_service_field_headers():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = security_center_management.UpdateSecurityCenterServiceRequest()
+
+    request.security_center_service.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_security_center_service), "__call__"
+    ) as call:
+        call.return_value = security_center_management.SecurityCenterService()
+        client.update_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "security_center_service.name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_update_security_center_service_field_headers_async():
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = security_center_management.UpdateSecurityCenterServiceRequest()
+
+    request.security_center_service.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_security_center_service), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.SecurityCenterService()
+        )
+        await client.update_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "security_center_service.name=name_value",
+    ) in kw["metadata"]
+
+
+def test_update_security_center_service_flattened():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_security_center_service), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = security_center_management.SecurityCenterService()
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.update_security_center_service(
+            security_center_service=security_center_management.SecurityCenterService(
+                name="name_value"
+            ),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].security_center_service
+        mock_val = security_center_management.SecurityCenterService(name="name_value")
+        assert arg == mock_val
+        arg = args[0].update_mask
+        mock_val = field_mask_pb2.FieldMask(paths=["paths_value"])
+        assert arg == mock_val
+
+
+def test_update_security_center_service_flattened_error():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.update_security_center_service(
+            security_center_management.UpdateSecurityCenterServiceRequest(),
+            security_center_service=security_center_management.SecurityCenterService(
+                name="name_value"
+            ),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+
+@pytest.mark.asyncio
+async def test_update_security_center_service_flattened_async():
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_security_center_service), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = security_center_management.SecurityCenterService()
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            security_center_management.SecurityCenterService()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.update_security_center_service(
+            security_center_service=security_center_management.SecurityCenterService(
+                name="name_value"
+            ),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].security_center_service
+        mock_val = security_center_management.SecurityCenterService(name="name_value")
+        assert arg == mock_val
+        arg = args[0].update_mask
+        mock_val = field_mask_pb2.FieldMask(paths=["paths_value"])
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_update_security_center_service_flattened_error_async():
+    client = SecurityCenterManagementAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.update_security_center_service(
+            security_center_management.UpdateSecurityCenterServiceRequest(),
+            security_center_service=security_center_management.SecurityCenterService(
+                name="name_value"
+            ),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest,
         dict,
     ],
 )
 def test_list_effective_security_health_analytics_custom_modules_rest(request_type):
     client = SecurityCenterManagementClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -7712,14 +11923,55 @@
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListEffectiveSecurityHealthAnalyticsCustomModulesPager
     )
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_effective_security_health_analytics_custom_modules_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_effective_security_health_analytics_custom_modules
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_effective_security_health_analytics_custom_modules
+        ] = mock_rpc
+
+        request = {}
+        client.list_effective_security_health_analytics_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_effective_security_health_analytics_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_effective_security_health_analytics_custom_modules_rest_required_fields(
     request_type=security_center_management.ListEffectiveSecurityHealthAnalyticsCustomModulesRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -8111,14 +12363,55 @@
     assert (
         response.enablement_state
         == security_center_management.EffectiveSecurityHealthAnalyticsCustomModule.EnablementState.ENABLED
     )
     assert response.display_name == "display_name_value"
 
 
+def test_get_effective_security_health_analytics_custom_module_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.get_effective_security_health_analytics_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_effective_security_health_analytics_custom_module
+        ] = mock_rpc
+
+        request = {}
+        client.get_effective_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_effective_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_effective_security_health_analytics_custom_module_rest_required_fields(
     request_type=security_center_management.GetEffectiveSecurityHealthAnalyticsCustomModuleRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -8415,14 +12708,55 @@
         response = client.list_security_health_analytics_custom_modules(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListSecurityHealthAnalyticsCustomModulesPager)
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_security_health_analytics_custom_modules_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_security_health_analytics_custom_modules
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_security_health_analytics_custom_modules
+        ] = mock_rpc
+
+        request = {}
+        client.list_security_health_analytics_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_security_health_analytics_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_security_health_analytics_custom_modules_rest_required_fields(
     request_type=security_center_management.ListSecurityHealthAnalyticsCustomModulesRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -8801,14 +13135,55 @@
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListDescendantSecurityHealthAnalyticsCustomModulesPager
     )
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_descendant_security_health_analytics_custom_modules_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_descendant_security_health_analytics_custom_modules
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_descendant_security_health_analytics_custom_modules
+        ] = mock_rpc
+
+        request = {}
+        client.list_descendant_security_health_analytics_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_descendant_security_health_analytics_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_descendant_security_health_analytics_custom_modules_rest_required_fields(
     request_type=security_center_management.ListDescendantSecurityHealthAnalyticsCustomModulesRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -9202,14 +13577,55 @@
         response.enablement_state
         == security_center_management.SecurityHealthAnalyticsCustomModule.EnablementState.ENABLED
     )
     assert response.last_editor == "last_editor_value"
     assert response.ancestor_module == "ancestor_module_value"
 
 
+def test_get_security_health_analytics_custom_module_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.get_security_health_analytics_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_security_health_analytics_custom_module
+        ] = mock_rpc
+
+        request = {}
+        client.get_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_security_health_analytics_custom_module_rest_required_fields(
     request_type=security_center_management.GetSecurityHealthAnalyticsCustomModuleRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -9620,14 +14036,55 @@
         response.enablement_state
         == security_center_management.SecurityHealthAnalyticsCustomModule.EnablementState.ENABLED
     )
     assert response.last_editor == "last_editor_value"
     assert response.ancestor_module == "ancestor_module_value"
 
 
+def test_create_security_health_analytics_custom_module_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.create_security_health_analytics_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_security_health_analytics_custom_module
+        ] = mock_rpc
+
+        request = {}
+        client.create_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_create_security_health_analytics_custom_module_rest_required_fields(
     request_type=security_center_management.CreateSecurityHealthAnalyticsCustomModuleRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -10055,14 +14512,55 @@
         response.enablement_state
         == security_center_management.SecurityHealthAnalyticsCustomModule.EnablementState.ENABLED
     )
     assert response.last_editor == "last_editor_value"
     assert response.ancestor_module == "ancestor_module_value"
 
 
+def test_update_security_health_analytics_custom_module_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.update_security_health_analytics_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_security_health_analytics_custom_module
+        ] = mock_rpc
+
+        request = {}
+        client.update_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_update_security_health_analytics_custom_module_rest_required_fields(
     request_type=security_center_management.UpdateSecurityHealthAnalyticsCustomModuleRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request = request_type(**request_init)
@@ -10376,14 +14874,55 @@
         req.return_value = response_value
         response = client.delete_security_health_analytics_custom_module(request)
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
+def test_delete_security_health_analytics_custom_module_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.delete_security_health_analytics_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_security_health_analytics_custom_module
+        ] = mock_rpc
+
+        request = {}
+        client.delete_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_delete_security_health_analytics_custom_module_rest_required_fields(
     request_type=security_center_management.DeleteSecurityHealthAnalyticsCustomModuleRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -10654,14 +15193,55 @@
     # Establish that the response is the type that we expect.
     assert isinstance(
         response,
         security_center_management.SimulateSecurityHealthAnalyticsCustomModuleResponse,
     )
 
 
+def test_simulate_security_health_analytics_custom_module_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.simulate_security_health_analytics_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.simulate_security_health_analytics_custom_module
+        ] = mock_rpc
+
+        request = {}
+        client.simulate_security_health_analytics_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.simulate_security_health_analytics_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_simulate_security_health_analytics_custom_module_rest_required_fields(
     request_type=security_center_management.SimulateSecurityHealthAnalyticsCustomModuleRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -10972,14 +15552,55 @@
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListEffectiveEventThreatDetectionCustomModulesPager
     )
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_effective_event_threat_detection_custom_modules_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_effective_event_threat_detection_custom_modules
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_effective_event_threat_detection_custom_modules
+        ] = mock_rpc
+
+        request = {}
+        client.list_effective_event_threat_detection_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_effective_event_threat_detection_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_effective_event_threat_detection_custom_modules_rest_required_fields(
     request_type=security_center_management.ListEffectiveEventThreatDetectionCustomModulesRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -11373,14 +15994,55 @@
         == security_center_management.EffectiveEventThreatDetectionCustomModule.EnablementState.ENABLED
     )
     assert response.type_ == "type__value"
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
 
 
+def test_get_effective_event_threat_detection_custom_module_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.get_effective_event_threat_detection_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_effective_event_threat_detection_custom_module
+        ] = mock_rpc
+
+        request = {}
+        client.get_effective_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_effective_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_effective_event_threat_detection_custom_module_rest_required_fields(
     request_type=security_center_management.GetEffectiveEventThreatDetectionCustomModuleRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -11681,14 +16343,55 @@
         response = client.list_event_threat_detection_custom_modules(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListEventThreatDetectionCustomModulesPager)
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_event_threat_detection_custom_modules_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_event_threat_detection_custom_modules
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_event_threat_detection_custom_modules
+        ] = mock_rpc
+
+        request = {}
+        client.list_event_threat_detection_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_event_threat_detection_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_event_threat_detection_custom_modules_rest_required_fields(
     request_type=security_center_management.ListEventThreatDetectionCustomModulesRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -12063,14 +16766,55 @@
     # Establish that the response is the type that we expect.
     assert isinstance(
         response, pagers.ListDescendantEventThreatDetectionCustomModulesPager
     )
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_descendant_event_threat_detection_custom_modules_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_descendant_event_threat_detection_custom_modules
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_descendant_event_threat_detection_custom_modules
+        ] = mock_rpc
+
+        request = {}
+        client.list_descendant_event_threat_detection_custom_modules(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_descendant_event_threat_detection_custom_modules(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_descendant_event_threat_detection_custom_modules_rest_required_fields(
     request_type=security_center_management.ListDescendantEventThreatDetectionCustomModulesRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -12464,14 +17208,55 @@
     )
     assert response.type_ == "type__value"
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
     assert response.last_editor == "last_editor_value"
 
 
+def test_get_event_threat_detection_custom_module_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.get_event_threat_detection_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_event_threat_detection_custom_module
+        ] = mock_rpc
+
+        request = {}
+        client.get_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_event_threat_detection_custom_module_rest_required_fields(
     request_type=security_center_management.GetEventThreatDetectionCustomModuleRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -12869,14 +17654,55 @@
     )
     assert response.type_ == "type__value"
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
     assert response.last_editor == "last_editor_value"
 
 
+def test_create_event_threat_detection_custom_module_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.create_event_threat_detection_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_event_threat_detection_custom_module
+        ] = mock_rpc
+
+        request = {}
+        client.create_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_create_event_threat_detection_custom_module_rest_required_fields(
     request_type=security_center_management.CreateEventThreatDetectionCustomModuleRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -13289,14 +18115,55 @@
     )
     assert response.type_ == "type__value"
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
     assert response.last_editor == "last_editor_value"
 
 
+def test_update_event_threat_detection_custom_module_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.update_event_threat_detection_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_event_threat_detection_custom_module
+        ] = mock_rpc
+
+        request = {}
+        client.update_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_update_event_threat_detection_custom_module_rest_required_fields(
     request_type=security_center_management.UpdateEventThreatDetectionCustomModuleRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request = request_type(**request_init)
@@ -13608,14 +18475,55 @@
         req.return_value = response_value
         response = client.delete_event_threat_detection_custom_module(request)
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
+def test_delete_event_threat_detection_custom_module_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.delete_event_threat_detection_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_event_threat_detection_custom_module
+        ] = mock_rpc
+
+        request = {}
+        client.delete_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_delete_event_threat_detection_custom_module_rest_required_fields(
     request_type=security_center_management.DeleteEventThreatDetectionCustomModuleRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -13886,14 +18794,55 @@
     # Establish that the response is the type that we expect.
     assert isinstance(
         response,
         security_center_management.ValidateEventThreatDetectionCustomModuleResponse,
     )
 
 
+def test_validate_event_threat_detection_custom_module_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.validate_event_threat_detection_custom_module
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.validate_event_threat_detection_custom_module
+        ] = mock_rpc
+
+        request = {}
+        client.validate_event_threat_detection_custom_module(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.validate_event_threat_detection_custom_module(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_validate_event_threat_detection_custom_module_rest_required_fields(
     request_type=security_center_management.ValidateEventThreatDetectionCustomModuleRequest,
 ):
     transport_class = transports.SecurityCenterManagementRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -14093,14 +19042,1188 @@
 
 def test_validate_event_threat_detection_custom_module_rest_error():
     client = SecurityCenterManagementClient(
         credentials=ga_credentials.AnonymousCredentials(), transport="rest"
     )
 
 
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        security_center_management.GetSecurityCenterServiceRequest,
+        dict,
+    ],
+)
+def test_get_security_center_service_rest(request_type):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "name": "projects/sample1/locations/sample2/securityCenterServices/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = security_center_management.SecurityCenterService(
+            name="name_value",
+            intended_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+            effective_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        # Convert return value to protobuf type
+        return_value = security_center_management.SecurityCenterService.pb(return_value)
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.get_security_center_service(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, security_center_management.SecurityCenterService)
+    assert response.name == "name_value"
+    assert (
+        response.intended_enablement_state
+        == security_center_management.SecurityCenterService.EnablementState.INHERITED
+    )
+    assert (
+        response.effective_enablement_state
+        == security_center_management.SecurityCenterService.EnablementState.INHERITED
+    )
+
+
+def test_get_security_center_service_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.get_security_center_service
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_security_center_service
+        ] = mock_rpc
+
+        request = {}
+        client.get_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_security_center_service(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+def test_get_security_center_service_rest_required_fields(
+    request_type=security_center_management.GetSecurityCenterServiceRequest,
+):
+    transport_class = transports.SecurityCenterManagementRestTransport
+
+    request_init = {}
+    request_init["name"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(pb_request, use_integers_for_enums=False)
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).get_security_center_service._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["name"] = "name_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).get_security_center_service._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "name" in jsonified_request
+    assert jsonified_request["name"] == "name_value"
+
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = security_center_management.SecurityCenterService()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "get",
+                "query_params": pb_request,
+            }
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            # Convert return value to protobuf type
+            return_value = security_center_management.SecurityCenterService.pb(
+                return_value
+            )
+            json_return_value = json_format.MessageToJson(return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.get_security_center_service(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_get_security_center_service_rest_unset_required_fields():
+    transport = transports.SecurityCenterManagementRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.get_security_center_service._get_unset_required_fields({})
+    assert set(unset_fields) == (set(()) & set(("name",)))
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_get_security_center_service_rest_interceptors(null_interceptor):
+    transport = transports.SecurityCenterManagementRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.SecurityCenterManagementRestInterceptor(),
+    )
+    client = SecurityCenterManagementClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.SecurityCenterManagementRestInterceptor,
+        "post_get_security_center_service",
+    ) as post, mock.patch.object(
+        transports.SecurityCenterManagementRestInterceptor,
+        "pre_get_security_center_service",
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = security_center_management.GetSecurityCenterServiceRequest.pb(
+            security_center_management.GetSecurityCenterServiceRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = (
+            security_center_management.SecurityCenterService.to_json(
+                security_center_management.SecurityCenterService()
+            )
+        )
+
+        request = security_center_management.GetSecurityCenterServiceRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = security_center_management.SecurityCenterService()
+
+        client.get_security_center_service(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_get_security_center_service_rest_bad_request(
+    transport: str = "rest",
+    request_type=security_center_management.GetSecurityCenterServiceRequest,
+):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "name": "projects/sample1/locations/sample2/securityCenterServices/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.get_security_center_service(request)
+
+
+def test_get_security_center_service_rest_flattened():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = security_center_management.SecurityCenterService()
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {
+            "name": "projects/sample1/locations/sample2/securityCenterServices/sample3"
+        }
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            name="name_value",
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        # Convert return value to protobuf type
+        return_value = security_center_management.SecurityCenterService.pb(return_value)
+        json_return_value = json_format.MessageToJson(return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.get_security_center_service(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v1/{name=projects/*/locations/*/securityCenterServices/*}"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_get_security_center_service_rest_flattened_error(transport: str = "rest"):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.get_security_center_service(
+            security_center_management.GetSecurityCenterServiceRequest(),
+            name="name_value",
+        )
+
+
+def test_get_security_center_service_rest_error():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        security_center_management.ListSecurityCenterServicesRequest,
+        dict,
+    ],
+)
+def test_list_security_center_services_rest(request_type):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"parent": "projects/sample1/locations/sample2"}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = security_center_management.ListSecurityCenterServicesResponse(
+            next_page_token="next_page_token_value",
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        # Convert return value to protobuf type
+        return_value = security_center_management.ListSecurityCenterServicesResponse.pb(
+            return_value
+        )
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.list_security_center_services(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, pagers.ListSecurityCenterServicesPager)
+    assert response.next_page_token == "next_page_token_value"
+
+
+def test_list_security_center_services_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.list_security_center_services
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_security_center_services
+        ] = mock_rpc
+
+        request = {}
+        client.list_security_center_services(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_security_center_services(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+def test_list_security_center_services_rest_required_fields(
+    request_type=security_center_management.ListSecurityCenterServicesRequest,
+):
+    transport_class = transports.SecurityCenterManagementRestTransport
+
+    request_init = {}
+    request_init["parent"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(pb_request, use_integers_for_enums=False)
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).list_security_center_services._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["parent"] = "parent_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).list_security_center_services._get_unset_required_fields(jsonified_request)
+    # Check that path parameters and body parameters are not mixing in.
+    assert not set(unset_fields) - set(
+        (
+            "page_size",
+            "page_token",
+        )
+    )
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "parent" in jsonified_request
+    assert jsonified_request["parent"] == "parent_value"
+
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = security_center_management.ListSecurityCenterServicesResponse()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "get",
+                "query_params": pb_request,
+            }
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            # Convert return value to protobuf type
+            return_value = (
+                security_center_management.ListSecurityCenterServicesResponse.pb(
+                    return_value
+                )
+            )
+            json_return_value = json_format.MessageToJson(return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.list_security_center_services(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_list_security_center_services_rest_unset_required_fields():
+    transport = transports.SecurityCenterManagementRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.list_security_center_services._get_unset_required_fields(
+        {}
+    )
+    assert set(unset_fields) == (
+        set(
+            (
+                "pageSize",
+                "pageToken",
+            )
+        )
+        & set(("parent",))
+    )
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_list_security_center_services_rest_interceptors(null_interceptor):
+    transport = transports.SecurityCenterManagementRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.SecurityCenterManagementRestInterceptor(),
+    )
+    client = SecurityCenterManagementClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.SecurityCenterManagementRestInterceptor,
+        "post_list_security_center_services",
+    ) as post, mock.patch.object(
+        transports.SecurityCenterManagementRestInterceptor,
+        "pre_list_security_center_services",
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = security_center_management.ListSecurityCenterServicesRequest.pb(
+            security_center_management.ListSecurityCenterServicesRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = (
+            security_center_management.ListSecurityCenterServicesResponse.to_json(
+                security_center_management.ListSecurityCenterServicesResponse()
+            )
+        )
+
+        request = security_center_management.ListSecurityCenterServicesRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = (
+            security_center_management.ListSecurityCenterServicesResponse()
+        )
+
+        client.list_security_center_services(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_list_security_center_services_rest_bad_request(
+    transport: str = "rest",
+    request_type=security_center_management.ListSecurityCenterServicesRequest,
+):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"parent": "projects/sample1/locations/sample2"}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.list_security_center_services(request)
+
+
+def test_list_security_center_services_rest_flattened():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = security_center_management.ListSecurityCenterServicesResponse()
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {"parent": "projects/sample1/locations/sample2"}
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            parent="parent_value",
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        # Convert return value to protobuf type
+        return_value = security_center_management.ListSecurityCenterServicesResponse.pb(
+            return_value
+        )
+        json_return_value = json_format.MessageToJson(return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.list_security_center_services(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v1/{parent=projects/*/locations/*}/securityCenterServices"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_list_security_center_services_rest_flattened_error(transport: str = "rest"):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.list_security_center_services(
+            security_center_management.ListSecurityCenterServicesRequest(),
+            parent="parent_value",
+        )
+
+
+def test_list_security_center_services_rest_pager(transport: str = "rest"):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # TODO(kbandes): remove this mock unless there's a good reason for it.
+        # with mock.patch.object(path_template, 'transcode') as transcode:
+        # Set the response as a series of pages
+        response = (
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                ],
+                next_page_token="abc",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[],
+                next_page_token="def",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                ],
+                next_page_token="ghi",
+            ),
+            security_center_management.ListSecurityCenterServicesResponse(
+                security_center_services=[
+                    security_center_management.SecurityCenterService(),
+                    security_center_management.SecurityCenterService(),
+                ],
+            ),
+        )
+        # Two responses for two calls
+        response = response + response
+
+        # Wrap the values into proper Response objs
+        response = tuple(
+            security_center_management.ListSecurityCenterServicesResponse.to_json(x)
+            for x in response
+        )
+        return_values = tuple(Response() for i in response)
+        for return_val, response_val in zip(return_values, response):
+            return_val._content = response_val.encode("UTF-8")
+            return_val.status_code = 200
+        req.side_effect = return_values
+
+        sample_request = {"parent": "projects/sample1/locations/sample2"}
+
+        pager = client.list_security_center_services(request=sample_request)
+
+        results = list(pager)
+        assert len(results) == 6
+        assert all(
+            isinstance(i, security_center_management.SecurityCenterService)
+            for i in results
+        )
+
+        pages = list(client.list_security_center_services(request=sample_request).pages)
+        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
+            assert page_.raw_page.next_page_token == token
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        security_center_management.UpdateSecurityCenterServiceRequest,
+        dict,
+    ],
+)
+def test_update_security_center_service_rest(request_type):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "security_center_service": {
+            "name": "projects/sample1/locations/sample2/securityCenterServices/sample3"
+        }
+    }
+    request_init["security_center_service"] = {
+        "name": "projects/sample1/locations/sample2/securityCenterServices/sample3",
+        "intended_enablement_state": 1,
+        "effective_enablement_state": 1,
+        "modules": {},
+        "update_time": {"seconds": 751, "nanos": 543},
+        "service_config": {"fields": {}},
+    }
+    # The version of a generated dependency at test runtime may differ from the version used during generation.
+    # Delete any fields which are not present in the current runtime dependency
+    # See https://github.com/googleapis/gapic-generator-python/issues/1748
+
+    # Determine if the message type is proto-plus or protobuf
+    test_field = (
+        security_center_management.UpdateSecurityCenterServiceRequest.meta.fields[
+            "security_center_service"
+        ]
+    )
+
+    def get_message_fields(field):
+        # Given a field which is a message (composite type), return a list with
+        # all the fields of the message.
+        # If the field is not a composite type, return an empty list.
+        message_fields = []
+
+        if hasattr(field, "message") and field.message:
+            is_field_type_proto_plus_type = not hasattr(field.message, "DESCRIPTOR")
+
+            if is_field_type_proto_plus_type:
+                message_fields = field.message.meta.fields.values()
+            # Add `# pragma: NO COVER` because there may not be any `*_pb2` field types
+            else:  # pragma: NO COVER
+                message_fields = field.message.DESCRIPTOR.fields
+        return message_fields
+
+    runtime_nested_fields = [
+        (field.name, nested_field.name)
+        for field in get_message_fields(test_field)
+        for nested_field in get_message_fields(field)
+    ]
+
+    subfields_not_in_runtime = []
+
+    # For each item in the sample request, create a list of sub fields which are not present at runtime
+    # Add `# pragma: NO COVER` because this test code will not run if all subfields are present at runtime
+    for field, value in request_init[
+        "security_center_service"
+    ].items():  # pragma: NO COVER
+        result = None
+        is_repeated = False
+        # For repeated fields
+        if isinstance(value, list) and len(value):
+            is_repeated = True
+            result = value[0]
+        # For fields where the type is another message
+        if isinstance(value, dict):
+            result = value
+
+        if result and hasattr(result, "keys"):
+            for subfield in result.keys():
+                if (field, subfield) not in runtime_nested_fields:
+                    subfields_not_in_runtime.append(
+                        {
+                            "field": field,
+                            "subfield": subfield,
+                            "is_repeated": is_repeated,
+                        }
+                    )
+
+    # Remove fields from the sample request which are not present in the runtime version of the dependency
+    # Add `# pragma: NO COVER` because this test code will not run if all subfields are present at runtime
+    for subfield_to_delete in subfields_not_in_runtime:  # pragma: NO COVER
+        field = subfield_to_delete.get("field")
+        field_repeated = subfield_to_delete.get("is_repeated")
+        subfield = subfield_to_delete.get("subfield")
+        if subfield:
+            if field_repeated:
+                for i in range(0, len(request_init["security_center_service"][field])):
+                    del request_init["security_center_service"][field][i][subfield]
+            else:
+                del request_init["security_center_service"][field][subfield]
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = security_center_management.SecurityCenterService(
+            name="name_value",
+            intended_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+            effective_enablement_state=security_center_management.SecurityCenterService.EnablementState.INHERITED,
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        # Convert return value to protobuf type
+        return_value = security_center_management.SecurityCenterService.pb(return_value)
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.update_security_center_service(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, security_center_management.SecurityCenterService)
+    assert response.name == "name_value"
+    assert (
+        response.intended_enablement_state
+        == security_center_management.SecurityCenterService.EnablementState.INHERITED
+    )
+    assert (
+        response.effective_enablement_state
+        == security_center_management.SecurityCenterService.EnablementState.INHERITED
+    )
+
+
+def test_update_security_center_service_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = SecurityCenterManagementClient(
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
+            client._transport.update_security_center_service
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_security_center_service
+        ] = mock_rpc
+
+        request = {}
+        client.update_security_center_service(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_security_center_service(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+def test_update_security_center_service_rest_required_fields(
+    request_type=security_center_management.UpdateSecurityCenterServiceRequest,
+):
+    transport_class = transports.SecurityCenterManagementRestTransport
+
+    request_init = {}
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(pb_request, use_integers_for_enums=False)
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).update_security_center_service._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).update_security_center_service._get_unset_required_fields(jsonified_request)
+    # Check that path parameters and body parameters are not mixing in.
+    assert not set(unset_fields) - set(
+        (
+            "update_mask",
+            "validate_only",
+        )
+    )
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = security_center_management.SecurityCenterService()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "patch",
+                "query_params": pb_request,
+            }
+            transcode_result["body"] = pb_request
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            # Convert return value to protobuf type
+            return_value = security_center_management.SecurityCenterService.pb(
+                return_value
+            )
+            json_return_value = json_format.MessageToJson(return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.update_security_center_service(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_update_security_center_service_rest_unset_required_fields():
+    transport = transports.SecurityCenterManagementRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.update_security_center_service._get_unset_required_fields(
+        {}
+    )
+    assert set(unset_fields) == (
+        set(
+            (
+                "updateMask",
+                "validateOnly",
+            )
+        )
+        & set(
+            (
+                "securityCenterService",
+                "updateMask",
+            )
+        )
+    )
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_update_security_center_service_rest_interceptors(null_interceptor):
+    transport = transports.SecurityCenterManagementRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.SecurityCenterManagementRestInterceptor(),
+    )
+    client = SecurityCenterManagementClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.SecurityCenterManagementRestInterceptor,
+        "post_update_security_center_service",
+    ) as post, mock.patch.object(
+        transports.SecurityCenterManagementRestInterceptor,
+        "pre_update_security_center_service",
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = security_center_management.UpdateSecurityCenterServiceRequest.pb(
+            security_center_management.UpdateSecurityCenterServiceRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = (
+            security_center_management.SecurityCenterService.to_json(
+                security_center_management.SecurityCenterService()
+            )
+        )
+
+        request = security_center_management.UpdateSecurityCenterServiceRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = security_center_management.SecurityCenterService()
+
+        client.update_security_center_service(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_update_security_center_service_rest_bad_request(
+    transport: str = "rest",
+    request_type=security_center_management.UpdateSecurityCenterServiceRequest,
+):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "security_center_service": {
+            "name": "projects/sample1/locations/sample2/securityCenterServices/sample3"
+        }
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.update_security_center_service(request)
+
+
+def test_update_security_center_service_rest_flattened():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = security_center_management.SecurityCenterService()
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {
+            "security_center_service": {
+                "name": "projects/sample1/locations/sample2/securityCenterServices/sample3"
+            }
+        }
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            security_center_service=security_center_management.SecurityCenterService(
+                name="name_value"
+            ),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        # Convert return value to protobuf type
+        return_value = security_center_management.SecurityCenterService.pb(return_value)
+        json_return_value = json_format.MessageToJson(return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.update_security_center_service(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v1/{security_center_service.name=projects/*/locations/*/securityCenterServices/*}"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_update_security_center_service_rest_flattened_error(transport: str = "rest"):
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.update_security_center_service(
+            security_center_management.UpdateSecurityCenterServiceRequest(),
+            security_center_service=security_center_management.SecurityCenterService(
+                name="name_value"
+            ),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+
+def test_update_security_center_service_rest_error():
+    client = SecurityCenterManagementClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.SecurityCenterManagementGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = SecurityCenterManagementClient(
@@ -14250,14 +20373,17 @@
         "list_event_threat_detection_custom_modules",
         "list_descendant_event_threat_detection_custom_modules",
         "get_event_threat_detection_custom_module",
         "create_event_threat_detection_custom_module",
         "update_event_threat_detection_custom_module",
         "delete_event_threat_detection_custom_module",
         "validate_event_threat_detection_custom_module",
+        "get_security_center_service",
+        "list_security_center_services",
+        "update_security_center_service",
         "get_location",
         "list_locations",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
@@ -14596,14 +20722,23 @@
     assert session1 != session2
     session1 = client1.transport.delete_event_threat_detection_custom_module._session
     session2 = client2.transport.delete_event_threat_detection_custom_module._session
     assert session1 != session2
     session1 = client1.transport.validate_event_threat_detection_custom_module._session
     session2 = client2.transport.validate_event_threat_detection_custom_module._session
     assert session1 != session2
+    session1 = client1.transport.get_security_center_service._session
+    session2 = client2.transport.get_security_center_service._session
+    assert session1 != session2
+    session1 = client1.transport.list_security_center_services._session
+    session2 = client2.transport.list_security_center_services._session
+    assert session1 != session2
+    session1 = client1.transport.update_security_center_service._session
+    session2 = client2.transport.update_security_center_service._session
+    assert session1 != session2
 
 
 def test_security_center_management_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.SecurityCenterManagementGrpcTransport(
@@ -14850,18 +20985,46 @@
     path = SecurityCenterManagementClient.finding_path(**expected)
 
     # Check that the path construction is reversible.
     actual = SecurityCenterManagementClient.parse_finding_path(path)
     assert expected == actual
 
 
-def test_security_health_analytics_custom_module_path():
-    organization = "squid"
+def test_security_center_service_path():
+    project = "squid"
     location = "clam"
-    security_health_analytics_custom_module = "whelk"
+    service = "whelk"
+    expected = "projects/{project}/locations/{location}/securityCenterServices/{service}".format(
+        project=project,
+        location=location,
+        service=service,
+    )
+    actual = SecurityCenterManagementClient.security_center_service_path(
+        project, location, service
+    )
+    assert expected == actual
+
+
+def test_parse_security_center_service_path():
+    expected = {
+        "project": "octopus",
+        "location": "oyster",
+        "service": "nudibranch",
+    }
+    path = SecurityCenterManagementClient.security_center_service_path(**expected)
+
+    # Check that the path construction is reversible.
+    actual = SecurityCenterManagementClient.parse_security_center_service_path(path)
+    assert expected == actual
+
+
+def test_security_health_analytics_custom_module_path():
+    organization = "cuttlefish"
+    location = "mussel"
+    security_health_analytics_custom_module = "winkle"
     expected = "organizations/{organization}/locations/{location}/securityHealthAnalyticsCustomModules/{security_health_analytics_custom_module}".format(
         organization=organization,
         location=location,
         security_health_analytics_custom_module=security_health_analytics_custom_module,
     )
     actual = (
         SecurityCenterManagementClient.security_health_analytics_custom_module_path(
@@ -14869,124 +21032,124 @@
         )
     )
     assert expected == actual
 
 
 def test_parse_security_health_analytics_custom_module_path():
     expected = {
-        "organization": "octopus",
-        "location": "oyster",
-        "security_health_analytics_custom_module": "nudibranch",
+        "organization": "nautilus",
+        "location": "scallop",
+        "security_health_analytics_custom_module": "abalone",
     }
     path = SecurityCenterManagementClient.security_health_analytics_custom_module_path(
         **expected
     )
 
     # Check that the path construction is reversible.
     actual = SecurityCenterManagementClient.parse_security_health_analytics_custom_module_path(
         path
     )
     assert expected == actual
 
 
 def test_common_billing_account_path():
-    billing_account = "cuttlefish"
+    billing_account = "squid"
     expected = "billingAccounts/{billing_account}".format(
         billing_account=billing_account,
     )
     actual = SecurityCenterManagementClient.common_billing_account_path(billing_account)
     assert expected == actual
 
 
 def test_parse_common_billing_account_path():
     expected = {
-        "billing_account": "mussel",
+        "billing_account": "clam",
     }
     path = SecurityCenterManagementClient.common_billing_account_path(**expected)
 
     # Check that the path construction is reversible.
     actual = SecurityCenterManagementClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
-    folder = "winkle"
+    folder = "whelk"
     expected = "folders/{folder}".format(
         folder=folder,
     )
     actual = SecurityCenterManagementClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
-        "folder": "nautilus",
+        "folder": "octopus",
     }
     path = SecurityCenterManagementClient.common_folder_path(**expected)
 
     # Check that the path construction is reversible.
     actual = SecurityCenterManagementClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
-    organization = "scallop"
+    organization = "oyster"
     expected = "organizations/{organization}".format(
         organization=organization,
     )
     actual = SecurityCenterManagementClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
-        "organization": "abalone",
+        "organization": "nudibranch",
     }
     path = SecurityCenterManagementClient.common_organization_path(**expected)
 
     # Check that the path construction is reversible.
     actual = SecurityCenterManagementClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
-    project = "squid"
+    project = "cuttlefish"
     expected = "projects/{project}".format(
         project=project,
     )
     actual = SecurityCenterManagementClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
-        "project": "clam",
+        "project": "mussel",
     }
     path = SecurityCenterManagementClient.common_project_path(**expected)
 
     # Check that the path construction is reversible.
     actual = SecurityCenterManagementClient.parse_common_project_path(path)
     assert expected == actual
 
 
 def test_common_location_path():
-    project = "whelk"
-    location = "octopus"
+    project = "winkle"
+    location = "nautilus"
     expected = "projects/{project}/locations/{location}".format(
         project=project,
         location=location,
     )
     actual = SecurityCenterManagementClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
-        "project": "oyster",
-        "location": "nudibranch",
+        "project": "scallop",
+        "location": "abalone",
     }
     path = SecurityCenterManagementClient.common_location_path(**expected)
 
     # Check that the path construction is reversible.
     actual = SecurityCenterManagementClient.parse_common_location_path(path)
     assert expected == actual
```

