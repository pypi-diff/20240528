# Comparing `tmp/ms_salesforce_api-2.5.0.tar.gz` & `tmp/ms_salesforce_api-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-2.5.0.tar", max compression
+gzip compressed data, was "ms_salesforce_api-2.6.0.tar", max compression
```

## Comparing `ms_salesforce_api-2.5.0.tar` & `ms_salesforce_api-2.6.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35149 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/LICENSE
--rw-r--r--   0        0        0     8326 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/README.md
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0     1244 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2926 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2205 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/__init__.py
--rw-r--r--   0        0        0     1532 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/__init__.py
--rw-r--r--   0        0        0     1517 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/constants.py
--rw-r--r--   0        0        0    14378 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/dto/AccountDTO.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/dto/__init__.py
--rw-r--r--   0        0        0     4077 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/export_data/Bigquery.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/export_data/__init__.py
--rw-r--r--   0        0        0     1620 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/__init__.py
--rw-r--r--   0        0        0     4975 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/constants.py
--rw-r--r--   0        0        0    15701 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/dto/__init__.py
--rw-r--r--   0        0        0     5381 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py
--rw-r--r--   0        0        0     6011 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    10789 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0      303 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/helpers.py
--rw-r--r--   0        0        0     3788 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/__tests__/__init__.py
--rw-r--r--   0        0        0    24839 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py
--rw-r--r--   0        0        0    10921 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/constants.py
--rw-r--r--   0        0        0     3967 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0    35689 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2485 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/__init__.py
--rw-r--r--   0        0        0     9829 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py
--rw-r--r--   0        0        0    12640 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    13717 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/helpers/__init__.py
--rw-r--r--   0        0        0      303 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/helpers/string.py
--rw-r--r--   0        0        0     1055 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     9153 1970-01-01 00:00:00.000000 ms_salesforce_api-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-28 09:06:43.612287 ms_salesforce_api-2.6.0/LICENSE
+-rw-r--r--   0        0        0     8326 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0     1244 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2926 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2205 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/__init__.py
+-rw-r--r--   0        0        0     1532 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/account/__init__.py
+-rw-r--r--   0        0        0     1517 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/account/constants.py
+-rw-r--r--   0        0        0    14378 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/account/dto/AccountDTO.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/account/dto/__init__.py
+-rw-r--r--   0        0        0     4077 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/account/export_data/Bigquery.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/account/export_data/__init__.py
+-rw-r--r--   0        0        0     1620 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/__init__.py
+-rw-r--r--   0        0        0     5005 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/constants.py
+-rw-r--r--   0        0        0    16144 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/dto/__init__.py
+-rw-r--r--   0        0        0     5460 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py
+-rw-r--r--   0        0        0     6011 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    10789 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0      303 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/helpers.py
+-rw-r--r--   0        0        0     3788 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    24839 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0    10921 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/constants.py
+-rw-r--r--   0        0        0     3967 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    35689 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2485 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/dto/__init__.py
+-rw-r--r--   0        0        0     9829 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0    12640 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    13717 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/helpers/__init__.py
+-rw-r--r--   0        0        0      303 2024-05-28 09:06:43.616287 ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/helpers/string.py
+-rw-r--r--   0        0        0     1055 2024-05-28 09:06:43.620287 ms_salesforce_api-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9153 1970-01-01 00:00:00.000000 ms_salesforce_api-2.6.0/PKG-INFO
```

### Comparing `ms_salesforce_api-2.5.0/LICENSE` & `ms_salesforce_api-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/README.md` & `ms_salesforce_api-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/__init__.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/account/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/constants.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/account/constants.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/dto/AccountDTO.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/account/dto/AccountDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/export_data/Bigquery.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/account/export_data/Bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/__init__.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/constants.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
     Servicios_Asociados__c,
     StageName,
     Start_Date__c,
     Tier_Short__c,
     TotalOpportunityQuantity,
     Year_Created__c,
     LKP_Project__c,
+    Owner.name,
+    NextStep,
     (
         SELECT
             Id,
             Product2.Id,
             Product2.LKP_ProfitCenter__r.Name,
             toLabel(Product2.LKP_ProfitCenter__r.PCK_Country__c),
             FRM_ProductName__c,
```

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,16 @@
         total_opportunity_quantity,
         year_created,
         opportunity_line_items,
         lkp_project,
         created_date,
         proposal_delivery_date,
         record_type,
+        owner_name,
+        next_step,
     ):
         self.opportunity_id = opportunity_id
         self.account_billing_country = account_billing_country
         self.account_owner = account_owner
         self.account_id = account_id
         self.amount = amount
         self.amount_eur = amount_eur
@@ -187,14 +189,16 @@
         self.total_opportunity_quantity = total_opportunity_quantity
         self.year_created = year_created
         self.opportunity_line_items = opportunity_line_items
         self.lkp_project = lkp_project
         self.created_date = created_date
         self.proposal_delivery_date = proposal_delivery_date
         self.record_type = record_type
+        self.owner_name = owner_name
+        self.next_step = next_step
 
     @staticmethod
     def from_salesforce_record(record):
         def _get_year_created(key: str):
             try:
                 year = int(record[key])
                 # We set allways the January first date because they want
@@ -218,14 +222,20 @@
 
         def _get_record_type():
             try:
                 return record["RecordType"]["Name"]
             except (KeyError, TypeError):
                 return ""
 
+        def _get_owner_name():
+            try:
+                return record["Owner"]["Name"]
+            except (KeyError, TypeError):
+                return ""
+
         opportunity_line_items = record.get("OpportunityLineItems", {})
         if opportunity_line_items and isinstance(opportunity_line_items, dict):
             line_items_records = record.get("OpportunityLineItems", {}).get(
                 "records", []
             )
             opportunity_line_items = [
                 OpportunityLineItemDTO.from_salesforce_record(
@@ -327,14 +337,16 @@
             ),
             year_created=_get_year_created("Year_Created__c"),
             opportunity_line_items=opportunity_line_items,
             lkp_project=normalize_value(record.get("LKP_Project__c", "")),
             created_date=record["CreatedDate"],
             proposal_delivery_date=record["Proposal_Delivery_Date__c"],
             record_type=_get_record_type(),
+            owner_name=_get_owner_name(),
+            next_step=record["NextStep"],
         )
 
     def to_dict(self):
         return {
             "opportunity_id": self.opportunity_id,
             "account_billing_country": self.account_billing_country,
             "account_owner": self.account_owner,
@@ -388,8 +400,10 @@
             "total_opportunity_quantity": self.total_opportunity_quantity,
             "year_created": self.year_created,
             "opportunity_line_items": self.opportunity_line_items,
             "lkp_project": self.lkp_project,
             "created_date": self.created_date,
             "proposal_delivery_date": self.proposal_delivery_date,
             "record_type": self.record_type,
+            "owner_name": self.owner_name,
+            "next_step": self.next_step,
         }
```

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
                 "total_opportunity_quantity": "FLOAT",
                 "start_date": "DATE",
                 "year_created": "DATE",
                 "lkp_project": "STRING",
                 "created_date": "TIMESTAMP",
                 "proposal_delivery_date": "TIMESTAMP",
                 "record_type": "STRING",
+                "owner_name": "STRING",
+                "next_step": "STRING",
             },
             "opportunity_line_item": {
                 "opportunity_id": "STRING",
                 "product_id": "STRING",
                 "profit_center_name": "STRING",
                 "country": "STRING",
                 "product_name": "STRING",
```

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/__init__.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/constants.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/constants.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-2.6.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.5.0/pyproject.toml` & `ms_salesforce_api-2.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "2.5.0"
+version = "2.6.0"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-2.5.0/PKG-INFO` & `ms_salesforce_api-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 2.5.0
+Version: 2.6.0
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

