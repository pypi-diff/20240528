# Comparing `tmp/oda_wd_client-0.2.0.tar.gz` & `tmp/oda_wd_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oda_wd_client-0.2.0.tar", max compression
+gzip compressed data, was "oda_wd_client-0.2.1.tar", max compression
```

## Comparing `oda_wd_client-0.2.0.tar` & `oda_wd_client-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0        0 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/__init__.py
--rw-r--r--   0        0        0      368 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/api.py
--rw-r--r--   0        0        0        0 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/base/__init__.py
--rw-r--r--   0        0        0     7281 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/base/api.py
--rw-r--r--   0        0        0      623 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/base/logging.py
--rw-r--r--   0        0        0      741 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/base/tools.py
--rw-r--r--   0        0        0     5242 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/base/types.py
--rw-r--r--   0        0        0     2894 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/base/utils.py
--rw-r--r--   0        0        0        0 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/service/__init__.py
--rw-r--r--   0        0        0       19 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/service/financial_management/__init__.py
--rw-r--r--   0        0        0     5543 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/service/financial_management/api.py
--rw-r--r--   0        0        0     6989 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/service/financial_management/types.py
--rw-r--r--   0        0        0    10331 2024-03-04 15:10:00.790419 oda_wd_client-0.2.0/oda_wd_client/service/financial_management/utils.py
--rw-r--r--   0        0        0        0 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/human_resources/__init__.py
--rw-r--r--   0        0        0     4857 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/human_resources/api.py
--rw-r--r--   0        0        0     1708 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/human_resources/types.py
--rw-r--r--   0        0        0     6367 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/human_resources/utils.py
--rw-r--r--   0        0        0        0 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/resource_management/__init__.py
--rw-r--r--   0        0        0     3560 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/resource_management/api.py
--rw-r--r--   0        0        0       40 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/resource_management/exceptions.py
--rw-r--r--   0        0        0     8934 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/resource_management/types.py
--rw-r--r--   0        0        0    13987 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/resource_management/utils.py
--rw-r--r--   0        0        0        0 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/staffing/__init__.py
--rw-r--r--   0        0        0     1407 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/staffing/api.py
--rw-r--r--   0        0        0     3618 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/staffing/types.py
--rw-r--r--   0        0        0      983 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/service/staffing/utils.py
--rw-r--r--   0        0        0      350 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/types/__init__.py
--rw-r--r--   0        0        0      584 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/types/financial_management.py
--rw-r--r--   0        0        0       85 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/types/human_resources.py
--rw-r--r--   0        0        0      649 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/types/resource_management.py
--rw-r--r--   0        0        0       82 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/oda_wd_client/types/staffing.py
--rw-r--r--   0        0        0      986 2024-03-04 15:10:00.794420 oda_wd_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 oda_wd_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/__init__.py
+-rw-r--r--   0        0        0      368 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/api.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/base/__init__.py
+-rw-r--r--   0        0        0     7281 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/base/api.py
+-rw-r--r--   0        0        0      623 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/base/logging.py
+-rw-r--r--   0        0        0      741 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/base/tools.py
+-rw-r--r--   0        0        0     5242 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/base/types.py
+-rw-r--r--   0        0        0     2894 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/base/utils.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/__init__.py
+-rw-r--r--   0        0        0       19 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/financial_management/__init__.py
+-rw-r--r--   0        0        0     5543 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/financial_management/api.py
+-rw-r--r--   0        0        0     6989 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/financial_management/types.py
+-rw-r--r--   0        0        0    10331 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/financial_management/utils.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/human_resources/__init__.py
+-rw-r--r--   0        0        0     4857 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/human_resources/api.py
+-rw-r--r--   0        0        0     1708 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/human_resources/types.py
+-rw-r--r--   0        0        0     6367 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/human_resources/utils.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/resource_management/__init__.py
+-rw-r--r--   0        0        0     3560 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/resource_management/api.py
+-rw-r--r--   0        0        0       40 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/resource_management/exceptions.py
+-rw-r--r--   0        0        0     9368 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/resource_management/types.py
+-rw-r--r--   0        0        0    14315 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/resource_management/utils.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/staffing/__init__.py
+-rw-r--r--   0        0        0     1407 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/staffing/api.py
+-rw-r--r--   0        0        0     3618 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/staffing/types.py
+-rw-r--r--   0        0        0      983 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/service/staffing/utils.py
+-rw-r--r--   0        0        0      350 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/types/__init__.py
+-rw-r--r--   0        0        0      584 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/types/financial_management.py
+-rw-r--r--   0        0        0       85 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/types/human_resources.py
+-rw-r--r--   0        0        0      649 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/types/resource_management.py
+-rw-r--r--   0        0        0       82 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/oda_wd_client/types/staffing.py
+-rw-r--r--   0        0        0      986 2024-05-28 13:38:46.466027 oda_wd_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 oda_wd_client-0.2.1/PKG-INFO
```

### Comparing `oda_wd_client-0.2.0/oda_wd_client/base/api.py` & `oda_wd_client-0.2.1/oda_wd_client/base/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/base/logging.py` & `oda_wd_client-0.2.1/oda_wd_client/base/logging.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/base/tools.py` & `oda_wd_client-0.2.1/oda_wd_client/base/tools.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/base/types.py` & `oda_wd_client-0.2.1/oda_wd_client/base/types.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/base/utils.py` & `oda_wd_client-0.2.1/oda_wd_client/base/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/service/financial_management/api.py` & `oda_wd_client-0.2.1/oda_wd_client/service/financial_management/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/service/financial_management/types.py` & `oda_wd_client-0.2.1/oda_wd_client/service/financial_management/types.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/service/financial_management/utils.py` & `oda_wd_client-0.2.1/oda_wd_client/service/financial_management/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/service/human_resources/api.py` & `oda_wd_client-0.2.1/oda_wd_client/service/human_resources/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/service/human_resources/types.py` & `oda_wd_client-0.2.1/oda_wd_client/service/human_resources/types.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/service/human_resources/utils.py` & `oda_wd_client-0.2.1/oda_wd_client/service/human_resources/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/service/resource_management/api.py` & `oda_wd_client-0.2.1/oda_wd_client/service/resource_management/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/service/resource_management/types.py` & `oda_wd_client-0.2.1/oda_wd_client/service/resource_management/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,24 @@
     _class_name = "Business_Entity_Status_ValueObject"
     workday_id: WorkdayID
     workday_id_type: Literal[
         "Business_Entity_Status_Value_ID"
     ] = "Business_Entity_Status_Value_ID"
 
 
+class Organization(WorkdayReferenceBaseModel):
+    """
+    Reference: https://community.workday.com/sites/default/files/file-hosting/productionapi/Resource_Management/v42.1/Get_Suppliers.html#OrganizationObjectType  # noqa
+    """
+
+    _class_name = "OrganizationObject"
+    workday_id: str
+    workday_id_type: Literal["Organization_Reference_ID"] = "Organization_Reference_ID"
+
+
 class Supplier(WorkdayReferenceBaseModel):
     """
     Reference: https://community.workday.com/sites/default/files/file-hosting/productionapi/Resource_Management/v40.2/Get_Suppliers.html#SupplierType  # noqa
     """
 
     _class_name = "SupplierObject"
     workday_id: str
@@ -90,14 +100,15 @@
     email: str | None = None
     url: str | None = None
     currency: str | None = None
     bank_account: str | None = None
     iban: str | None = None
     primary_tax_id: str | None = None
     worktag_only: bool = False
+    restricted_to_companies: list[Organization] = []
 
 
 class TaxRate(WorkdayReferenceBaseModel):
     """
     Reference: https://community.workday.com/sites/default/files/file-hosting/productionapi/Resource_Management/v40.2/Submit_Supplier_Invoice.html#Tax_RateObjectType  # noqa
     """
```

### Comparing `oda_wd_client-0.2.0/oda_wd_client/service/resource_management/utils.py` & `oda_wd_client-0.2.1/oda_wd_client/service/resource_management/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     Company,
     CostCenterWorktag,
     Currency,
     SpendCategory,
 )
 from oda_wd_client.service.resource_management.exceptions import NoSupplierID
 from oda_wd_client.service.resource_management.types import (
+    Organization,
     PrepaidAmortizationType,
     Supplier,
     SupplierInvoice,
     SupplierInvoiceAdjustment,
     SupplierInvoiceLine,
     SupplierStatus,
     TaxApplicability,
@@ -102,25 +103,31 @@
     currency_ref = sup_data.get("Currency_Reference", None)
     status_ref = None
     for status_line in sup_data.get("Supplier_Status_Data", []):
         _ref = SupplierStatus.from_id_list(status_line["Status_Reference"]["ID"])
         if _ref:
             status_ref = _ref
 
+    restrict_org_refs = sup_data.get("Restricted_To_Companies_Reference", list())
+    _orgs = [Organization.from_id_list(item["ID"]) for item in restrict_org_refs]
+    # Type narrowing to remove falsy values
+    restricted_orgs = [org for org in _orgs if org]
+
     return Supplier(
         workday_id=sup_id,
         reference_id=sup_data.get("Supplier_Reference_ID", None),
         name=sup_data["Supplier_Name"],
         status=status_ref,
         payment_terms=get_id_from_list(
             sup_data.get("Payment_Terms_Reference", {}).get("ID", []),
             "Payment_Terms_ID",
         ),
         primary_tax_id=primary_tax_id,
         worktag_only=sup_data["Worktag_Only"],
+        restricted_to_companies=restricted_orgs,
         # Currency_ID _should_ be in accordance with ISO 4217
         currency=get_id_from_list(currency_ref["ID"], "Currency_ID")
         if currency_ref
         else None,
         **contact_data,
         **account_data,
     )
```

### Comparing `oda_wd_client-0.2.0/oda_wd_client/service/staffing/api.py` & `oda_wd_client-0.2.1/oda_wd_client/service/staffing/api.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/service/staffing/types.py` & `oda_wd_client-0.2.1/oda_wd_client/service/staffing/types.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/service/staffing/utils.py` & `oda_wd_client-0.2.1/oda_wd_client/service/staffing/utils.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/types/financial_management.py` & `oda_wd_client-0.2.1/oda_wd_client/types/financial_management.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/oda_wd_client/types/resource_management.py` & `oda_wd_client-0.2.1/oda_wd_client/types/resource_management.py`

 * *Files identical despite different names*

### Comparing `oda_wd_client-0.2.0/pyproject.toml` & `oda_wd_client-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oda-wd-client"
-version = "0.2.0"
+version = "0.2.1"
 description = "A library for interacting with Workday from Python"
 authors = [
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `oda_wd_client-0.2.0/PKG-INFO` & `oda_wd_client-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oda-wd-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library for interacting with Workday from Python
 Author: Karl Fredrik Haugland
 Author-email: karlfredrik.haugland@oda.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
```

