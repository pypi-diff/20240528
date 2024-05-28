# Comparing `tmp/pytbai-1.5.6.tar.gz` & `tmp/pytbai-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.5.6.tar", last modified: Wed May 22 14:46:15 2024, max compression
+gzip compressed data, was "pytbai-1.5.7.tar", last modified: Tue May 28 15:26:52 2024, max compression
```

## Comparing `pytbai-1.5.6.tar` & `pytbai-1.5.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:15.404923 pytbai-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-22 14:46:11.000000 pytbai-1.5.6/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-22 14:46:11.000000 pytbai-1.5.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-22 14:46:11.000000 pytbai-1.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 14:46:11.000000 pytbai-1.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 14:46:11.000000 pytbai-1.5.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-22 14:46:15.404923 pytbai-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-22 14:46:11.000000 pytbai-1.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:15.400923 pytbai-1.5.6/pytbai/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 14:46:11.000000 pytbai-1.5.6/pytbai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-05-22 14:46:11.000000 pytbai-1.5.6/pytbai/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-22 14:46:11.000000 pytbai-1.5.6/pytbai/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:15.404923 pytbai-1.5.6/pytbai/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:15.404923 pytbai-1.5.6/pytbai/templates/XML/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:11.000000 pytbai-1.5.6/pytbai/templates/XML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-22 14:46:11.000000 pytbai-1.5.6/pytbai/templates/XML/tbai_structure.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:15.404923 pytbai-1.5.6/pytbai/templates/XSD/
--rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-05-22 14:46:11.000000 pytbai-1.5.6/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:11.000000 pytbai-1.5.6/pytbai/templates/XSD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-22 14:46:11.000000 pytbai-1.5.6/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:11.000000 pytbai-1.5.6/pytbai/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:15.404923 pytbai-1.5.6/pytbai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:11.000000 pytbai-1.5.6/pytbai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-22 14:46:11.000000 pytbai-1.5.6/pytbai/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-22 14:46:11.000000 pytbai-1.5.6/pytbai/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:15.404923 pytbai-1.5.6/pytbai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-22 14:46:15.000000 pytbai-1.5.6/pytbai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-22 14:46:15.000000 pytbai-1.5.6/pytbai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:46:15.000000 pytbai-1.5.6/pytbai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 14:46:15.000000 pytbai-1.5.6/pytbai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 14:46:15.000000 pytbai-1.5.6/pytbai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:46:15.404923 pytbai-1.5.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-05-22 14:46:11.000000 pytbai-1.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:15.404923 pytbai-1.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:11.000000 pytbai-1.5.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:15.404923 pytbai-1.5.6/tests/certs/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-22 14:46:11.000000 pytbai-1.5.6/tests/certs/cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-22 14:46:11.000000 pytbai-1.5.6/tests/certs/cert_for_tests.p12
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-22 14:46:11.000000 pytbai-1.5.6/tests/certs/key.pem
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 14:46:11.000000 pytbai-1.5.6/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:15.404923 pytbai-1.5.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 14:46:11.000000 pytbai-1.5.6/tests/data/tbai_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-22 14:46:11.000000 pytbai-1.5.6/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.546223 pytbai-1.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-28 15:26:47.000000 pytbai-1.5.7/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:26:47.000000 pytbai-1.5.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-28 15:26:47.000000 pytbai-1.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 15:26:47.000000 pytbai-1.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 15:26:47.000000 pytbai-1.5.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-28 15:26:52.546223 pytbai-1.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-28 15:26:47.000000 pytbai-1.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.542223 pytbai-1.5.7/pytbai/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.542223 pytbai-1.5.7/pytbai/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.542223 pytbai-1.5.7/pytbai/templates/XML/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/templates/XML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/templates/XML/tbai_structure.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.542223 pytbai-1.5.7/pytbai/templates/XSD/
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/templates/XSD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.546223 pytbai-1.5.7/pytbai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.546223 pytbai-1.5.7/pytbai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-28 15:26:52.000000 pytbai-1.5.7/pytbai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-28 15:26:52.000000 pytbai-1.5.7/pytbai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:26:52.000000 pytbai-1.5.7/pytbai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 15:26:52.000000 pytbai-1.5.7/pytbai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 15:26:52.000000 pytbai-1.5.7/pytbai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:26:52.546223 pytbai-1.5.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-05-28 15:26:47.000000 pytbai-1.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.546223 pytbai-1.5.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.546223 pytbai-1.5.7/tests/certs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/certs/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/certs/cert_for_tests.p12
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/certs/key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.546223 pytbai-1.5.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/data/tbai_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/test_basic.py
```

### Comparing `pytbai-1.5.6/CHANGELOG.txt` & `pytbai-1.5.7/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.6/LICENSE` & `pytbai-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.6/PKG-INFO` & `pytbai-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.5.6
+Version: 1.5.7
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.5.6/README.md` & `pytbai-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.6/pytbai/core.py` & `pytbai-1.5.7/pytbai/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,60 +72,60 @@
 
 
 class InvoiceLine:
     def __init__(
         self,
         description,
         quantity=Decimal("0"),
-        unit_amount=Decimal("0"),
+        amount=Decimal("0"),
         discount=Decimal("0"),
         vat_rate=DEFAULT_VAT_RATE,
         vat_type=None,
+        vat_included=None,
     ):
         self.description = description
         self.quantity = quantity
-        self.unit_amount = unit_amount
         self.discount = discount
         self.vat_rate = vat_rate
-        self.vat_fee = None
+        self.vat_fee = Decimal("0")
         if not vat_type:
             self.vat_type = S1
         elif vat_type in L11:
             self.vat_type = vat_type
         else:
             raise ValueError(
                 "Value not found in L11 options, see documentation: %s"
                 % DOCUMENTATION_URL
             )
 
-        self.set_base()
-        self.set_vat_fee()
-        self.set_total()
-
-    def get_line_base(self):
-        line_base = self.quantity * self.unit_amount
-        return line_base.quantize(Decimal("0.00"))
-
-    def get_discount_qty(self, line_base):
-        discount_qty = line_base * (self.discount / 100)
-        return discount_qty.quantize(Decimal("0.00"))
-
-    def set_base(self):
-        line_base = self.get_line_base()
-        if self.discount:
+        if not vat_included:
+            self.unit_amount = amount
+            line_base = self.quantity * self.unit_amount
             self.vat_base = line_base - self.get_discount_qty(line_base)
+            vat_fee = self.vat_base * (self.vat_rate / 100)
+            self.vat_fee = vat_fee.quantize(Decimal("0.00"))
+            self.total = self.vat_base + self.vat_fee
         else:
-            self.vat_base = line_base
+            self.total = amount
+            line_base = (self.total - self.get_discount_qty(self.total)) / self.quantity
+            self.unit_amount = (line_base / (1 + (self.vat_rate / 100))).quantize(
+                Decimal("0.00")
+            )
+            self.vat_fee = line_base.quantize(Decimal("0.00")) - self.unit_amount
+            vat_base = self.vat_fee / (self.vat_rate / 100)
+            self.vat_base = vat_base.quantize(Decimal("0.00"))
 
-    def set_vat_fee(self):
-        vat_fee = self.vat_base * (self.vat_rate / 100)
-        self.vat_fee = vat_fee.quantize(Decimal("0.00"))
+    def get_line_base(self):
+        return self.quantity * self.unit_amount
 
-    def set_total(self):
-        self.total = self.vat_base + self.vat_fee
+    def get_discount_qty(self, amount):
+        discount_qty = Decimal("0")
+        if self.discount:
+            discount_qty = amount * (self.discount / 100)
+        return discount_qty.quantize(Decimal("0.00"))
 
     def get_dict(self):
         return copy.deepcopy(self.__dict__)
 
 
 class Invoice:
     def __init__(
```

### Comparing `pytbai-1.5.6/pytbai/definitions.py` & `pytbai-1.5.7/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.6/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.5.7/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.6/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.5.7/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.6/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.5.7/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.6/pytbai/utils/xml.py` & `pytbai-1.5.7/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.6/pytbai.egg-info/PKG-INFO` & `pytbai-1.5.7/pytbai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.5.6
+Version: 1.5.7
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.5.6/pytbai.egg-info/SOURCES.txt` & `pytbai-1.5.7/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.6/setup.py` & `pytbai-1.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.5.6",
+    version="1.5.7",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.5.6/tests/certs/cert.pem` & `pytbai-1.5.7/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.6/tests/certs/cert_for_tests.p12` & `pytbai-1.5.7/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.6/tests/certs/key.pem` & `pytbai-1.5.7/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.6/tests/data/tbai_json.py` & `pytbai-1.5.7/tests/data/tbai_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         "expedition_date": "2023-07-05",
         "expedition_time": "12:58:17",
         "transaction_date": "2023-07-05",
         "simplified": "N",
         "substitution": "N",
         "vat_regime": "01",
         "lines": [],
-        "total_amount": 0,
+        "total_amount": 0.0,
         "vat_breakdown": [],
     },
     "software": {
         "license": "TBAIGIPRE00000000501",
         "dev_entity": "P2000000F",
         "soft_name": "FAKTURABAI",
         "soft_version": "1.0",
@@ -70,32 +70,32 @@
         "transaction_date": "2023-07-05",
         "simplified": "N",
         "substitution": "N",
         "vat_regime": "01",
         "lines": [
             {
                 "description": "Primer producto",
-                "quantity": 1,
-                "unit_amount": 200,
-                "discount": 20,
-                "vat_rate": 21,
+                "quantity": 1.0,
+                "discount": 20.0,
+                "vat_rate": 21.0,
                 "vat_fee": 33.6,
                 "vat_type": "S1",
+                "unit_amount": 200.0,
                 "vat_base": 160.0,
                 "total": 193.6,
             },
             {
                 "description": "Segundo producto",
-                "quantity": 2,
-                "unit_amount": 350,
-                "discount": 0,
-                "vat_rate": 21,
+                "quantity": 2.0,
+                "discount": 0.0,
+                "vat_rate": 21.0,
                 "vat_fee": 147.0,
                 "vat_type": "S1",
-                "vat_base": 700,
+                "unit_amount": 350.0,
+                "vat_base": 700.0,
                 "total": 847.0,
             },
         ],
         "total_amount": 1040.6,
         "vat_breakdown": [
             {"type": "S1", "rates": {"21": {"base": 860.0, "fee": 180.6}}}
         ],
```

### Comparing `pytbai-1.5.6/tests/test_basic.py` & `pytbai-1.5.7/tests/test_basic.py`

 * *Files identical despite different names*

