# Comparing `tmp/pytbai-1.5.7.tar.gz` & `tmp/pytbai-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.5.7.tar", last modified: Tue May 28 15:26:52 2024, max compression
+gzip compressed data, was "pytbai-1.5.8.tar", last modified: Tue May 28 16:10:35 2024, max compression
```

## Comparing `pytbai-1.5.7.tar` & `pytbai-1.5.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.546223 pytbai-1.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-28 15:26:47.000000 pytbai-1.5.7/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:26:47.000000 pytbai-1.5.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-28 15:26:47.000000 pytbai-1.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 15:26:47.000000 pytbai-1.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 15:26:47.000000 pytbai-1.5.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-28 15:26:52.546223 pytbai-1.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-28 15:26:47.000000 pytbai-1.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.542223 pytbai-1.5.7/pytbai/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.542223 pytbai-1.5.7/pytbai/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.542223 pytbai-1.5.7/pytbai/templates/XML/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/templates/XML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/templates/XML/tbai_structure.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.542223 pytbai-1.5.7/pytbai/templates/XSD/
--rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/templates/XSD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.546223 pytbai-1.5.7/pytbai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-28 15:26:47.000000 pytbai-1.5.7/pytbai/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.546223 pytbai-1.5.7/pytbai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-28 15:26:52.000000 pytbai-1.5.7/pytbai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-28 15:26:52.000000 pytbai-1.5.7/pytbai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:26:52.000000 pytbai-1.5.7/pytbai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 15:26:52.000000 pytbai-1.5.7/pytbai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 15:26:52.000000 pytbai-1.5.7/pytbai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:26:52.546223 pytbai-1.5.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-05-28 15:26:47.000000 pytbai-1.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.546223 pytbai-1.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.546223 pytbai-1.5.7/tests/certs/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/certs/cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/certs/cert_for_tests.p12
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/certs/key.pem
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:26:52.546223 pytbai-1.5.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/data/tbai_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-28 15:26:47.000000 pytbai-1.5.7/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:35.505087 pytbai-1.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-28 16:10:31.000000 pytbai-1.5.8/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 16:10:31.000000 pytbai-1.5.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-28 16:10:31.000000 pytbai-1.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 16:10:31.000000 pytbai-1.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 16:10:31.000000 pytbai-1.5.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-28 16:10:35.505087 pytbai-1.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-28 16:10:31.000000 pytbai-1.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:35.501087 pytbai-1.5.8/pytbai/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 16:10:31.000000 pytbai-1.5.8/pytbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-05-28 16:10:31.000000 pytbai-1.5.8/pytbai/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-28 16:10:31.000000 pytbai-1.5.8/pytbai/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:35.501087 pytbai-1.5.8/pytbai/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:35.505087 pytbai-1.5.8/pytbai/templates/XML/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:31.000000 pytbai-1.5.8/pytbai/templates/XML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-28 16:10:31.000000 pytbai-1.5.8/pytbai/templates/XML/tbai_structure.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:35.505087 pytbai-1.5.8/pytbai/templates/XSD/
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-05-28 16:10:31.000000 pytbai-1.5.8/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:31.000000 pytbai-1.5.8/pytbai/templates/XSD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-28 16:10:31.000000 pytbai-1.5.8/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:31.000000 pytbai-1.5.8/pytbai/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:35.505087 pytbai-1.5.8/pytbai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:31.000000 pytbai-1.5.8/pytbai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 16:10:31.000000 pytbai-1.5.8/pytbai/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-28 16:10:31.000000 pytbai-1.5.8/pytbai/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:35.505087 pytbai-1.5.8/pytbai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-28 16:10:35.000000 pytbai-1.5.8/pytbai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-28 16:10:35.000000 pytbai-1.5.8/pytbai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:10:35.000000 pytbai-1.5.8/pytbai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 16:10:35.000000 pytbai-1.5.8/pytbai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 16:10:35.000000 pytbai-1.5.8/pytbai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:10:35.505087 pytbai-1.5.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-05-28 16:10:31.000000 pytbai-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:35.505087 pytbai-1.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:31.000000 pytbai-1.5.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:35.505087 pytbai-1.5.8/tests/certs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-28 16:10:31.000000 pytbai-1.5.8/tests/certs/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-28 16:10:31.000000 pytbai-1.5.8/tests/certs/cert_for_tests.p12
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-28 16:10:31.000000 pytbai-1.5.8/tests/certs/key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 16:10:31.000000 pytbai-1.5.8/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:10:35.505087 pytbai-1.5.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-28 16:10:31.000000 pytbai-1.5.8/tests/data/tbai_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-28 16:10:31.000000 pytbai-1.5.8/tests/test_basic.py
```

### Comparing `pytbai-1.5.7/CHANGELOG.txt` & `pytbai-1.5.8/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/LICENSE` & `pytbai-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/PKG-INFO` & `pytbai-1.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.5.7
+Version: 1.5.8
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.5.7/README.md` & `pytbai-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/pytbai/core.py` & `pytbai-1.5.8/pytbai/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         self,
         description,
         quantity=Decimal("0"),
         amount=Decimal("0"),
         discount=Decimal("0"),
         vat_rate=DEFAULT_VAT_RATE,
         vat_type=None,
-        vat_included=None,
+        vat_included=False,
     ):
         self.description = description
         self.quantity = quantity
         self.discount = discount
         self.vat_rate = vat_rate
         self.vat_fee = Decimal("0")
         if not vat_type:
@@ -216,26 +216,28 @@
                 breakdown.append(line_types)
         return breakdown
 
     def create_line(
         self,
         description,
         quantity=Decimal("0"),
-        unit_import=Decimal("0"),
+        amount=Decimal("0"),
         discount=Decimal("0"),
         vat_rate=DEFAULT_VAT_RATE,
         vat_type=S1,
+        vat_included=False,
     ):
         line = InvoiceLine(
             description,
             quantity,
-            unit_import,
+            amount,
             discount,
             vat_rate,
             vat_type,
+            vat_included,
         )
         self.lines.append(line)
 
     def delete_lines(self, lines):
         curr_lines = self.lines
         for line in lines:
             curr_lines.remove(line)
```

### Comparing `pytbai-1.5.7/pytbai/definitions.py` & `pytbai-1.5.8/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.5.8/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.5.8/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.5.8/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/pytbai/utils/xml.py` & `pytbai-1.5.8/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/pytbai.egg-info/PKG-INFO` & `pytbai-1.5.8/pytbai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.5.7
+Version: 1.5.8
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.5.7/pytbai.egg-info/SOURCES.txt` & `pytbai-1.5.8/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/setup.py` & `pytbai-1.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.5.7",
+    version="1.5.8",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.5.7/tests/certs/cert.pem` & `pytbai-1.5.8/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/tests/certs/cert_for_tests.p12` & `pytbai-1.5.8/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/tests/certs/key.pem` & `pytbai-1.5.8/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/tests/data/tbai_json.py` & `pytbai-1.5.8/tests/data/tbai_json.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.7/tests/test_basic.py` & `pytbai-1.5.8/tests/test_basic.py`

 * *Files identical despite different names*

