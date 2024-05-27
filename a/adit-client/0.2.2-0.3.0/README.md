# Comparing `tmp/adit_client-0.2.2.tar.gz` & `tmp/adit_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adit_client-0.2.2.tar", max compression
+gzip compressed data, was "adit_client-0.3.0.tar", max compression
```

## Comparing `adit_client-0.2.2.tar` & `adit_client-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      740 2023-09-03 09:56:17.000000 adit_client-0.2.2/README.md
--rw-r--r--   0        0        0       57 2023-09-03 09:56:17.000000 adit_client-0.2.2/adit_client/__init__.py
--rw-r--r--   0        0        0     2484 2023-09-03 09:56:17.000000 adit_client-0.2.2/adit_client/client.py
--rw-r--r--   0        0        0      438 2023-11-05 13:22:47.171551 adit_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 adit_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35122 2024-05-27 22:34:48.182611 adit_client-0.3.0/LICENSE
+-rw-r--r--   0        0        0      859 2024-05-27 22:34:48.182611 adit_client-0.3.0/README.md
+-rw-r--r--   0        0        0       57 2024-05-27 22:34:48.182611 adit_client-0.3.0/adit_client/__init__.py
+-rw-r--r--   0        0        0     2488 2024-05-27 23:24:15.289869 adit_client-0.3.0/adit_client/client.py
+-rw-r--r--   0        0        0     1701 2024-05-27 23:47:42.803608 adit_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1453 1970-01-01 00:00:00.000000 adit_client-0.3.0/PKG-INFO
```

### Comparing `adit_client-0.2.2/adit_client/client.py` & `adit_client-0.3.0/adit_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,13 +49,13 @@
 
     def store_instances(self, ae_title: str, instances: list[Dataset]) -> None:
         """Store some instances on an ADIT server."""
         self._create_dicom_web_client(ae_title).store_instances(instances)
 
     def _create_dicom_web_client(self, ae_title: str) -> DICOMwebClient:
         return DICOMwebClient(
-            url=f"{self.server_url}/dicom-web/{ae_title}",
+            url=f"{self.server_url}/api/dicom-web/{ae_title}",
             qido_url_prefix="qidors",
             wado_url_prefix="wadors",
             stow_url_prefix="stowrs",
             headers={"Authorization": f"Token {self.auth_token}"},
         )
```

### Comparing `adit_client-0.2.2/PKG-INFO` & `adit_client-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: adit-client
-Version: 0.2.2
+Version: 0.3.0
 Summary: ADIT Client library to connect to an ADIT server.
 License: GPL-3.0-or-later
 Author: Kai Schlamp
 Author-email: kai.schlamp@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dicomweb-client (>=0.59.1,<0.60.0)
 Requires-Dist: pydicom (>=2.4.3,<3.0.0)
 Description-Content-Type: text/markdown
 
-# Adit Client
+# ADIT Client
 
 ## About
 
-Adit Client is the official Python client of [ADIT (Automated DICOM Transfer)](https://github.com/radexperts/adit).
+ADIT Client is the official Python client of [ADIT (Automated DICOM Transfer)](https://github.com/openradx/adit).
 
 ## Usage
 
 ### Prerequisites
 
 - Generate an API token in your ADIT profile.
-- Make sure to have the permissions to access the ADIT API.
+- Make sure you have the permissions to access the ADIT API.
 - Also make sure you have access to the DICOM nodes you want query.
 
 ### Code
 
 ```python
-adit_url = "https://adit" # The host URL of adit
-adit_token = "my_token" # The generated auth token
-client = AditClient(server_url=adit_url, auth_token=adit_token)
+server_url = "https://adit" # The host URL of the ADIT server
+auth_token = "my_token" # The authentication token generated in your profile
+client = AditClient(server_url=server_url, auth_token=auth_token)
 
-# Search for studies
+# Search for studies. The first parameter is the AE title of the DICOM server
+# you want to query.
 studies = client.search_for_studies("ORTHANC1", {"PatientName": "Doe, John"})
 
-# The client returns pydicom datasets
+# The client returns pydicom datasets.
 study_descriptions = [study.StudyDescription for study in studies]
 ```
```

