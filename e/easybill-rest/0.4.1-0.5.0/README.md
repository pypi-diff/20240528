# Comparing `tmp/easybill_rest-0.4.1.tar.gz` & `tmp/easybill_rest-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybill_rest-0.4.1.tar", last modified: Tue Oct 17 12:31:14 2023, max compression
+gzip compressed data, was "easybill_rest-0.5.0.tar", last modified: Tue May 28 19:56:37 2024, max compression
```

## Comparing `easybill_rest-0.4.1.tar` & `easybill_rest-0.5.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 jannohles   (502) staff       (20)        0 2023-10-17 12:31:14.312020 easybill_rest-0.4.1/
--rw-r--r--   0 jannohles   (502) staff       (20)       94 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/MANIFEST.in
--rw-r--r--   0 jannohles   (502) staff       (20)     1434 2023-10-17 12:31:14.311881 easybill_rest-0.4.1/PKG-INFO
--rw-r--r--   0 jannohles   (502) staff       (20)      676 2023-10-17 12:03:00.000000 easybill_rest-0.4.1/changelog.md
-drwxr-xr-x   0 jannohles   (502) staff       (20)        0 2023-10-17 12:31:14.306761 easybill_rest-0.4.1/easybill_rest/
--rw-r--r--   0 jannohles   (502) staff       (20)     9547 2023-10-17 12:03:00.000000 easybill_rest-0.4.1/easybill_rest/__init__.py
--rw-r--r--   0 jannohles   (502) staff       (20)      431 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/helper.py
-drwxr-xr-x   0 jannohles   (502) staff       (20)        0 2023-10-17 12:31:14.311646 easybill_rest-0.4.1/easybill_rest/resources/
--rw-r--r--   0 jannohles   (502) staff       (20)      470 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_abstract.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2839 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_attachments.py
--rw-r--r--   0 jannohles   (502) staff       (20)     3201 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_contacts.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2635 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_customer_groups.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2390 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_customers.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2860 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_discount_position_groups.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2697 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_discount_positions.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2131 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_document_payments.py
--rw-r--r--   0 jannohles   (502) staff       (20)     4312 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_documents.py
--rw-r--r--   0 jannohles   (502) staff       (20)     1131 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_logins.py
--rw-r--r--   0 jannohles   (502) staff       (20)      854 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_pdf_templates.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2634 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_position_groups.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2390 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_positions.py
--rw-r--r--   0 jannohles   (502) staff       (20)     1547 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_post_boxes.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2366 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_projects.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2518 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_sepa_payments.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2076 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_serial_numbers.py
--rw-r--r--   0 jannohles   (502) staff       (20)     1508 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_stocks.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2213 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_tasks.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2602 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_text_templates.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2509 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_time_trackings.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2366 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/easybill_rest/resources/resource_webhooks.py
-drwxr-xr-x   0 jannohles   (502) staff       (20)        0 2023-10-17 12:31:14.307521 easybill_rest-0.4.1/easybill_rest.egg-info/
--rw-r--r--   0 jannohles   (502) staff       (20)     1434 2023-10-17 12:31:14.000000 easybill_rest-0.4.1/easybill_rest.egg-info/PKG-INFO
--rw-r--r--   0 jannohles   (502) staff       (20)     1356 2023-10-17 12:31:14.000000 easybill_rest-0.4.1/easybill_rest.egg-info/SOURCES.txt
--rw-r--r--   0 jannohles   (502) staff       (20)        1 2023-10-17 12:31:14.000000 easybill_rest-0.4.1/easybill_rest.egg-info/dependency_links.txt
--rw-r--r--   0 jannohles   (502) staff       (20)       42 2023-10-17 12:31:14.000000 easybill_rest-0.4.1/easybill_rest.egg-info/requires.txt
--rw-r--r--   0 jannohles   (502) staff       (20)       14 2023-10-17 12:31:14.000000 easybill_rest-0.4.1/easybill_rest.egg-info/top_level.txt
--rw-r--r--   0 jannohles   (502) staff       (20)     1036 2023-02-28 11:38:49.000000 easybill_rest-0.4.1/license.md
--rw-r--r--   0 jannohles   (502) staff       (20)      975 2023-10-17 12:03:00.000000 easybill_rest-0.4.1/readme.md
--rw-r--r--   0 jannohles   (502) staff       (20)       38 2023-10-17 12:31:14.312060 easybill_rest-0.4.1/setup.cfg
--rw-r--r--   0 jannohles   (502) staff       (20)      905 2023-10-17 12:03:00.000000 easybill_rest-0.4.1/setup.py
+drwxr-xr-x   0 jannohles   (502) staff       (20)        0 2024-05-28 19:56:37.336291 easybill_rest-0.5.0/
+-rw-r--r--   0 jannohles   (502) staff       (20)       94 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/MANIFEST.in
+-rw-r--r--   0 jannohles   (502) staff       (20)     1577 2024-05-28 19:56:37.336066 easybill_rest-0.5.0/PKG-INFO
+-rw-r--r--   0 jannohles   (502) staff       (20)      924 2024-05-28 19:41:52.000000 easybill_rest-0.5.0/changelog.md
+drwxr-xr-x   0 jannohles   (502) staff       (20)        0 2024-05-28 19:56:37.331133 easybill_rest-0.5.0/easybill_rest/
+-rw-r--r--   0 jannohles   (502) staff       (20)     9868 2024-05-28 19:41:52.000000 easybill_rest-0.5.0/easybill_rest/__init__.py
+-rw-r--r--   0 jannohles   (502) staff       (20)      431 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/helper.py
+drwxr-xr-x   0 jannohles   (502) staff       (20)        0 2024-05-28 19:56:37.335384 easybill_rest-0.5.0/easybill_rest/resources/
+-rw-r--r--   0 jannohles   (502) staff       (20)      470 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_abstract.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2795 2024-05-28 19:41:52.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_attachments.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     3217 2024-05-28 19:41:52.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_contacts.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2635 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_customer_groups.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2390 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_customers.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2860 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_discount_position_groups.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2697 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_discount_positions.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2131 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_document_payments.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2374 2024-05-28 19:41:52.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_document_versions.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     4781 2024-05-28 19:41:52.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_documents.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     1131 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_logins.py
+-rw-r--r--   0 jannohles   (502) staff       (20)      854 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_pdf_templates.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2634 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_position_groups.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2390 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_positions.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     1547 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_post_boxes.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2366 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_projects.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2518 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_sepa_payments.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2076 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_serial_numbers.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     1508 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_stocks.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2213 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_tasks.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2602 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_text_templates.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2509 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_time_trackings.py
+-rw-r--r--   0 jannohles   (502) staff       (20)     2366 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/easybill_rest/resources/resource_webhooks.py
+drwxr-xr-x   0 jannohles   (502) staff       (20)        0 2024-05-28 19:56:37.335587 easybill_rest-0.5.0/easybill_rest.egg-info/
+-rw-r--r--   0 jannohles   (502) staff       (20)     1577 2024-05-28 19:56:37.000000 easybill_rest-0.5.0/easybill_rest.egg-info/PKG-INFO
+-rw-r--r--   0 jannohles   (502) staff       (20)     1410 2024-05-28 19:56:37.000000 easybill_rest-0.5.0/easybill_rest.egg-info/SOURCES.txt
+-rw-r--r--   0 jannohles   (502) staff       (20)        1 2024-05-28 19:56:37.000000 easybill_rest-0.5.0/easybill_rest.egg-info/dependency_links.txt
+-rw-r--r--   0 jannohles   (502) staff       (20)       42 2024-05-28 19:56:37.000000 easybill_rest-0.5.0/easybill_rest.egg-info/requires.txt
+-rw-r--r--   0 jannohles   (502) staff       (20)       14 2024-05-28 19:56:37.000000 easybill_rest-0.5.0/easybill_rest.egg-info/top_level.txt
+-rw-r--r--   0 jannohles   (502) staff       (20)     1036 2023-02-28 11:38:49.000000 easybill_rest-0.5.0/license.md
+-rw-r--r--   0 jannohles   (502) staff       (20)      975 2024-05-28 19:41:52.000000 easybill_rest-0.5.0/readme.md
+-rw-r--r--   0 jannohles   (502) staff       (20)       38 2024-05-28 19:56:37.336331 easybill_rest-0.5.0/setup.cfg
+-rw-r--r--   0 jannohles   (502) staff       (20)      905 2024-05-28 19:41:52.000000 easybill_rest-0.5.0/setup.py
```

### Comparing `easybill_rest-0.4.1/PKG-INFO` & `easybill_rest-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: easybill_rest
-Version: 0.4.1
+Version: 0.5.0
 Summary: easybill_rest is a library to work with the easybill REST API (https://www.easybill.de/api/)
 Home-page: https://github.com/BolZer/py-ebrest
 Author: Jan Noehles (bolZer)
 Author-email: noehles@easybill.de
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
+Requires-Dist: requests
 Provides-Extra: dev
+Requires-Dist: coverage<5; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+Requires-Dist: pytest<8; extra == "dev"
 
 # easybill_rest (py-ebrest)
-[![Generic badge](https://img.shields.io/badge/Version-0.4.1-important.svg)]()
+[![Generic badge](https://img.shields.io/badge/Version-0.5.0-important.svg)]()
 [![Generic badge](https://img.shields.io/badge/coverage-97%25-success.svg)]()
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/easybill_rest.svg)
 [![Generic badge](https://img.shields.io/badge/License-MIT-blue.svg)]()
 [![Build Status](https://travis-ci.com/BolZer/py-ebrest.svg?branch=master)](https://travis-ci.com/BolZer/py-ebrest)
 
 `easybill_rest` is a library to work with the easybill REST API (https://www.easybill.de/api/) written in Python.
```

### Comparing `easybill_rest-0.4.1/changelog.md` & `easybill_rest-0.5.0/changelog.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 CHANGELOG
 =========
+* 0.5.0 (2024-05-28) 
+    * Update dependencies
+    * Fix attachment download method
+    * Add new resource document versions
+    * Add new method to download the document as jpeg
+    * Rename method to download document as pdf to be more precise
+
 * 0.4.1 (2023-10-17) 
     * Update urllib3 to v. 1.26.17
 
 * 0.4.0 (2023-07-26)
     * Change Python Version requirement to 3.11
     * Switch from nose to pytest
     * Bump dependencies with security issues
```

### Comparing `easybill_rest-0.4.1/easybill_rest/__init__.py` & `easybill_rest-0.5.0/easybill_rest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 from easybill_rest.resources.resource_sepa_payments import ResourceSepaPayments
 from easybill_rest.resources.resource_serial_numbers import ResourceSerialNumbers
 from easybill_rest.resources.resource_stocks import ResourceStocks
 from easybill_rest.resources.resource_tasks import ResourceTasks
 from easybill_rest.resources.resource_text_templates import ResourceTextTemplates
 from easybill_rest.resources.resource_time_trackings import ResourceTimeTrackings
 from easybill_rest.resources.resource_webhooks import ResourceWebhooks
+from easybill_rest.resources.resource_document_versions import ResourceDocumentVersions
 
 
 class Client:
-    _version: str = "0.4.1"
+    _version: str = "0.5.0"
     _base_url: str = "https://api.easybill.de"
     _requests = requests
 
     api_key: str = ""
     timeout: int
 
     def __init__(self, api_key: str, timeout: int = 10) -> None:
@@ -173,14 +174,20 @@
         return ResourceDiscountPositionGroups(self)
 
     def attachments(self) -> ResourceAttachments:
         """attachments returns the attachments resource which exposes the attachment resource."""
 
         return ResourceAttachments(self)
 
+    def document_versions(self) -> ResourceDocumentVersions:
+        """document_versions returns the document versions resource which exposes the document
+        version resource."""
+
+        return ResourceDocumentVersions(self)
+
     def call(
             self,
             method: str,
             request_url: str,
             headers: dict,
             passed_payload: dict = None) -> dict:
         """
```

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_attachments.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_attachments.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,16 @@
         return self.__client.upload(
             Helper.create_request_url_from_params(self.__endpoint),
             self.__client.get_basic_headers(),
             payload
         )
 
     def update_attachment(self, attachment_id: str, payload: dict) -> dict:
-        """update_attachment updates the reference (id) attachment with the given payload. Returns a part of the updated attachment model"""
+        """update_attachment updates the reference (id) attachment with the given payload. Returns a part of the
+        updated attachment model"""
 
         return self.__client.call(
             "PUT",
             Helper.create_request_url_from_params(
                 self.__endpoint +
                 "/" +
                 attachment_id),
@@ -66,14 +67,14 @@
             "DELETE",
             Helper.create_request_url_from_params(
                 self.__endpoint +
                 "/" +
                 attachment_id),
             self.__client.get_basic_headers())
 
-    def get_content(self, attachment_id: str, headers: dict = None) -> bytes:
-        """get_content returns None on success and raises an exception if the attachment couldn't be deleted"""
+    def get_content(self, attachment_id: str) -> bytes:
+        """get_content returns the attachment as bytes on success"""
 
         return self.__client.download(
             Helper.create_request_url_from_params(
-                self.__endpoint + "/" + attachment_id),
+                self.__endpoint + "/" + attachment_id + "/content"),
             self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_contacts.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_contacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,16 @@
                 "/" +
                 "contacts" +
                 "/" +
                 contact_id),
             self.__client.get_basic_headers_for_json())
 
     def create_contact(self, customer_id: str, payload: dict) -> dict:
-        """create_contact returns the contact model as dict on success with the data from the passed payload for the referenced customer"""
+        """create_contact returns the contact model as dict on success with the data from the passed payload for the
+        referenced customer"""
 
         return self.__client.call(
             "POST",
             Helper.create_request_url_from_params(
                 self.__endpoint +
                 "/" +
                 customer_id +
@@ -64,15 +65,16 @@
             payload)
 
     def update_contact(
             self,
             customer_id: str,
             contact_id: str,
             payload: dict) -> dict:
-        """update_contact updates the reference (id) contact with the given payload. Returns the updated contact model"""
+        """update_contact updates the reference (id) contact with the given payload. Returns the updated contact
+        model"""
 
         return self.__client.call(
             "PUT",
             Helper.create_request_url_from_params(
                 self.__endpoint +
                 "/" +
                 customer_id +
```

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_customer_groups.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_customer_groups.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_customers.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_customers.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_discount_position_groups.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_discount_position_groups.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_discount_positions.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_discount_positions.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_document_payments.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_document_payments.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_documents.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_documents.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,18 +116,30 @@
                 "/" +
                 document_id +
                 "/send/" +
                 str(send_method)),
             self.__client.get_basic_headers_for_json(),
             payload)
 
-    def download_document(self, document_id: str) -> bytes:
-        """download_document returns the document as bytes on success"""
+    def download_document_as_pdf(self, document_id: str) -> bytes:
+        """download_document_as_pdf returns the document pdf as bytes on success"""
 
         return self.__client.download(
             Helper.create_request_url_from_params(
                 self.__endpoint +
                 "/" +
                 document_id +
                 "/pdf"),
             self.__client.get_basic_headers_for_pdf(),
         )
+
+    def download_document_as_jpeg(self, document_id: str, params: dict = None) -> bytes:
+        """download_document_as_jpeg returns the document jpeg as bytes on success"""
+
+        return self.__client.download(
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                document_id +
+                "/jpg", params),
+            self.__client.get_basic_headers_for_pdf(),
+        )
```

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_logins.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_logins.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_pdf_templates.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_pdf_templates.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_position_groups.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_position_groups.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_positions.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_positions.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_post_boxes.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_post_boxes.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_projects.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_projects.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_sepa_payments.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_sepa_payments.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_serial_numbers.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_serial_numbers.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_stocks.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_stocks.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_tasks.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_tasks.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_text_templates.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_text_templates.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_time_trackings.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_time_trackings.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest/resources/resource_webhooks.py` & `easybill_rest-0.5.0/easybill_rest/resources/resource_webhooks.py`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/easybill_rest.egg-info/PKG-INFO` & `easybill_rest-0.5.0/easybill_rest.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
-Name: easybill-rest
-Version: 0.4.1
+Name: easybill_rest
+Version: 0.5.0
 Summary: easybill_rest is a library to work with the easybill REST API (https://www.easybill.de/api/)
 Home-page: https://github.com/BolZer/py-ebrest
 Author: Jan Noehles (bolZer)
 Author-email: noehles@easybill.de
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
+Requires-Dist: requests
 Provides-Extra: dev
+Requires-Dist: coverage<5; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+Requires-Dist: pytest<8; extra == "dev"
 
 # easybill_rest (py-ebrest)
-[![Generic badge](https://img.shields.io/badge/Version-0.4.1-important.svg)]()
+[![Generic badge](https://img.shields.io/badge/Version-0.5.0-important.svg)]()
 [![Generic badge](https://img.shields.io/badge/coverage-97%25-success.svg)]()
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/easybill_rest.svg)
 [![Generic badge](https://img.shields.io/badge/License-MIT-blue.svg)]()
 [![Build Status](https://travis-ci.com/BolZer/py-ebrest.svg?branch=master)](https://travis-ci.com/BolZer/py-ebrest)
 
 `easybill_rest` is a library to work with the easybill REST API (https://www.easybill.de/api/) written in Python.
```

### Comparing `easybill_rest-0.4.1/easybill_rest.egg-info/SOURCES.txt` & `easybill_rest-0.5.0/easybill_rest.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 easybill_rest/resources/resource_attachments.py
 easybill_rest/resources/resource_contacts.py
 easybill_rest/resources/resource_customer_groups.py
 easybill_rest/resources/resource_customers.py
 easybill_rest/resources/resource_discount_position_groups.py
 easybill_rest/resources/resource_discount_positions.py
 easybill_rest/resources/resource_document_payments.py
+easybill_rest/resources/resource_document_versions.py
 easybill_rest/resources/resource_documents.py
 easybill_rest/resources/resource_logins.py
 easybill_rest/resources/resource_pdf_templates.py
 easybill_rest/resources/resource_position_groups.py
 easybill_rest/resources/resource_positions.py
 easybill_rest/resources/resource_post_boxes.py
 easybill_rest/resources/resource_projects.py
```

### Comparing `easybill_rest-0.4.1/license.md` & `easybill_rest-0.5.0/license.md`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.4.1/readme.md` & `easybill_rest-0.5.0/readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # easybill_rest (py-ebrest)
-[![Generic badge](https://img.shields.io/badge/Version-0.4.1-important.svg)]()
+[![Generic badge](https://img.shields.io/badge/Version-0.5.0-important.svg)]()
 [![Generic badge](https://img.shields.io/badge/coverage-97%25-success.svg)]()
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/easybill_rest.svg)
 [![Generic badge](https://img.shields.io/badge/License-MIT-blue.svg)]()
 [![Build Status](https://travis-ci.com/BolZer/py-ebrest.svg?branch=master)](https://travis-ci.com/BolZer/py-ebrest)
 
 `easybill_rest` is a library to work with the easybill REST API (https://www.easybill.de/api/) written in Python.
```

### Comparing `easybill_rest-0.4.1/setup.py` & `easybill_rest-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     url="https://github.com/BolZer/py-ebrest",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     python_requires='>=3.11.0',
-    version="0.4.1",
+    version="0.5.0",
     install_requires=[
             "requests",
     ],
     extras_require={
         'dev': [
             "coverage<5",
             "wheel",
```

