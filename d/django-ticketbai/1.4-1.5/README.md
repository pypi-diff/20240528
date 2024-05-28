# Comparing `tmp/django_ticketbai-1.4.tar.gz` & `tmp/django_ticketbai-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ticketbai-1.4.tar", last modified: Wed May 22 14:22:25 2024, max compression
+gzip compressed data, was "django_ticketbai-1.5.tar", last modified: Tue May 28 09:55:11 2024, max compression
```

## Comparing `django_ticketbai-1.4.tar` & `django_ticketbai-1.5.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:25.610762 django_ticketbai-1.4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:14.000000 django_ticketbai-1.4/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-22 14:22:14.000000 django_ticketbai-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 14:22:14.000000 django_ticketbai-1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-22 14:22:25.610762 django_ticketbai-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-22 14:22:14.000000 django_ticketbai-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:25.602762 django_ticketbai-1.4/django_ticketbai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:25.606762 django_ticketbai-1.4/django_ticketbai/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0006_config_is_active.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0007_invoice_errorxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0010_alter_invoice_signature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0011_alter_invoice_signature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:25.602762 django_ticketbai-1.4/django_ticketbai/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:25.606762 django_ticketbai-1.4/django_ticketbai/templates/PDF/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/templates/PDF/ticketbai.css
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/templates/PDF/ticketbai.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:25.602762 django_ticketbai-1.4/django_ticketbai/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:25.610762 django_ticketbai-1.4/django_ticketbai/templates/admin/django_ticketbai/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/templates/admin/django_ticketbai/app_index.html
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:25.610762 django_ticketbai-1.4/django_ticketbai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/utils/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/utils/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-22 14:22:14.000000 django_ticketbai-1.4/django_ticketbai/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:22:25.610762 django_ticketbai-1.4/django_ticketbai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-22 14:22:25.000000 django_ticketbai-1.4/django_ticketbai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-22 14:22:25.000000 django_ticketbai-1.4/django_ticketbai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:22:25.000000 django_ticketbai-1.4/django_ticketbai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 14:22:25.000000 django_ticketbai-1.4/django_ticketbai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 14:22:25.000000 django_ticketbai-1.4/django_ticketbai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:22:25.610762 django_ticketbai-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-22 14:22:14.000000 django_ticketbai-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.404110 django_ticketbai-1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:04.000000 django_ticketbai-1.5/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-28 09:55:04.000000 django_ticketbai-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 09:55:04.000000 django_ticketbai-1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-28 09:55:11.404110 django_ticketbai-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 09:55:04.000000 django_ticketbai-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.396110 django_ticketbai-1.5/django_ticketbai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.400110 django_ticketbai-1.5/django_ticketbai/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0006_config_is_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0007_invoice_errorxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0010_alter_invoice_signature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0011_alter_invoice_signature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0015_invoice_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.392110 django_ticketbai-1.5/django_ticketbai/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.400110 django_ticketbai-1.5/django_ticketbai/templates/PDF/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/templates/PDF/ticketbai.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/templates/PDF/ticketbai.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.392110 django_ticketbai-1.5/django_ticketbai/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.400110 django_ticketbai-1.5/django_ticketbai/templates/admin/django_ticketbai/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/templates/admin/django_ticketbai/app_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.400110 django_ticketbai-1.5/django_ticketbai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/utils/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/utils/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.404110 django_ticketbai-1.5/django_ticketbai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-28 09:55:11.000000 django_ticketbai-1.5/django_ticketbai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-28 09:55:11.000000 django_ticketbai-1.5/django_ticketbai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:55:11.000000 django_ticketbai-1.5/django_ticketbai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 09:55:11.000000 django_ticketbai-1.5/django_ticketbai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 09:55:11.000000 django_ticketbai-1.5/django_ticketbai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:55:11.404110 django_ticketbai-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-28 09:55:04.000000 django_ticketbai-1.5/setup.py
```

### Comparing `django_ticketbai-1.4/LICENSE` & `django_ticketbai-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/PKG-INFO` & `django_ticketbai-1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ticketbai
-Version: 1.4
+Version: 1.5
 Summary: django-ticketbai allows to create, manage, store and send TicketBai invoices to the Basque tax authorities.
 Home-page: https://github.com/codesyntax/django-ticketbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `django_ticketbai-1.4/django_ticketbai/admin.py` & `django_ticketbai-1.5/django_ticketbai/admin.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/migrations/0001_initial.py` & `django_ticketbai-1.5/django_ticketbai/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py` & `django_ticketbai-1.5/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py` & `django_ticketbai-1.5/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py` & `django_ticketbai-1.5/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py` & `django_ticketbai-1.5/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py` & `django_ticketbai-1.5/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py` & `django_ticketbai-1.5/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/migrations/0010_alter_invoice_signature_value.py` & `django_ticketbai-1.5/django_ticketbai/migrations/0010_alter_invoice_signature_value.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py` & `django_ticketbai-1.5/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py` & `django_ticketbai-1.5/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py` & `django_ticketbai-1.5/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/models.py` & `django_ticketbai-1.5/django_ticketbai/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from django.utils.translation import gettext as _
 from .validators import validate_pdf_extension, validate_pks_extension
 from django.conf import settings
 
 
 User = settings.AUTH_USER_MODEL
 VAT_TYPE_CHOICES = ((row, row) for row in L11)
+LANGUAGE_CODE = getattr(settings, "LANGUAGE_CODE", "en")
 
 
 class Config(models.Model):
     logo = models.CharField(max_length=150, null=True, blank=True, verbose_name=_("Logo"), help_text=_("Relative path to the logo"))
     prefix = models.CharField(max_length=5, verbose_name=_("Prefix"))
     suffix = models.CharField(
         max_length=5, null=True, blank=True, verbose_name=_("Suffix")
@@ -99,14 +100,15 @@
     pre_invoice = models.ForeignKey(
         "self",
         null=True,
         blank=True,
         verbose_name=_("Previous invoice"),
         on_delete=models.SET_NULL,
     )
+    lang = models.CharField(max_length=3, default=LANGUAGE_CODE)
 
     def get_name(self):
         return "{}/{}".format(self.serial_code, self.num)
 
     get_name.short_description = _("Serie")
 
     def get_pdf_name(self):
```

### Comparing `django_ticketbai-1.4/django_ticketbai/templates/PDF/ticketbai.html` & `django_ticketbai-1.5/django_ticketbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/utils/invoice.py` & `django_ticketbai-1.5/django_ticketbai/utils/invoice.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from django_ticketbai.models import Config, Invoice, InvoiceLine
 from django_ticketbai.utils.pdf import build_pdf
 from django.utils.translation import gettext_lazy as _
 from django.core.mail import send_mail
 from pytbai import TBai
 from decimal import Decimal
 
+LANGUAGE_CODE = getattr(settings, "LANGUAGE_CODE", "en")
+
 
 def calculate_serial_code():
     config = Config.objects.filter(is_active=True).first()
     year = timezone.now().year
     suffix = config.suffix
     if suffix:
         suffix = "-{}".format(suffix)
@@ -58,20 +60,21 @@
     )
     hash = crc8.crc8()
     hash.update(tbai_code.encode("utf-8"))
     tbai_code += "{}".format(str(int(hash.hexdigest(), 16)).rjust(3, "0"))
     return tbai_code
 
 
-def store_invoice(tbai, tbai_invoice, prev_invoice=None, email=None):
+def store_invoice(tbai, tbai_invoice, lang, prev_invoice=None, email=None):
     tbai_json = json.loads(tbai.get_json(tbai_invoice))
     invoice_json = tbai_json["invoice"]
     subject_json = tbai_json["subject"]
     lines = invoice_json.pop("lines")
     invoice = Invoice(**invoice_json)
+    invoice.lang = lang
     if email:
         invoice.email = email
     invoice.vat_breakdown = json.dumps(invoice_json["vat_breakdown"])
     invoice.save()
     for line in lines:
         invoiceline = InvoiceLine(**line)
         invoiceline.invoice = invoice
@@ -128,27 +131,28 @@
     invoice_description,
     email,
     line_description,
     unit,
     price,
     discount=0,
     vat=21,
+    lang=LANGUAGE_CODE,
 ):
     config = Config.objects.filter(is_active=True).first()
     prev_invoice = get_prev_invoice()
     serial_code = calculate_serial_code()
     num = calculate_num(serial_code, None, prev_invoice)
 
     tbai = TBai(TICKETBAI_CONF)
     tbai_invoice = tbai.create_invoice(
         serial_code, num, invoice_description, simplified="S"
     )
     tbai_invoice.create_line(
         line_description, Decimal(unit), Decimal(price), Decimal(discount), Decimal(vat)
     )
 
-    invoice = store_invoice(tbai, tbai_invoice, prev_invoice, email)
+    invoice = store_invoice(tbai, tbai_invoice, lang, prev_invoice, email)
     invoice = sign_invoice(tbai, invoice, prev_invoice, tbai_invoice, config)
     invoice = store_pdf(tbai, invoice, tbai_invoice, config)
     invoice = send_invoice(tbai, invoice, config)
 
     return invoice
```

### Comparing `django_ticketbai-1.4/django_ticketbai/utils/pdf.py` & `django_ticketbai-1.5/django_ticketbai/utils/pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import io
 import qrcode
 import base64
 import crc8
 from io import BytesIO
 from django import template
+from django.utils import translation
 from requests.models import PreparedRequest
 from django.conf import settings
 from weasyprint import HTML, CSS
 from PIL import Image
 
 
 def get_crc8_url(url):
@@ -60,15 +61,17 @@
             width, height = image_file.size
             new_height = int(200 * height / width)
             image_file = image_file.resize((200, new_height), Image.LANCZOS)
             img_bytes = io.BytesIO()
             image_file.save(img_bytes, format='PNG')
             encoded_logo = base64.b64encode(img_bytes.getvalue()).decode("utf-8")
             context.update({"logo": encoded_logo})
+    translation.activate(invoice.lang)
     html = t.render(context)
+    translation.deactivate()
     return html
 
 
 def build_pdf(invoice, subject, config):
     css = CSS(string=get_css_string())
     html = HTML(string=get_html_string(invoice, subject, config.logo))
     return html.write_pdf(stylesheets=[css])
```

### Comparing `django_ticketbai-1.4/django_ticketbai/validators.py` & `django_ticketbai-1.5/django_ticketbai/validators.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai/views.py` & `django_ticketbai-1.5/django_ticketbai/views.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.4/django_ticketbai.egg-info/PKG-INFO` & `django_ticketbai-1.5/django_ticketbai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ticketbai
-Version: 1.4
+Version: 1.5
 Summary: django-ticketbai allows to create, manage, store and send TicketBai invoices to the Basque tax authorities.
 Home-page: https://github.com/codesyntax/django-ticketbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `django_ticketbai-1.4/django_ticketbai.egg-info/SOURCES.txt` & `django_ticketbai-1.5/django_ticketbai.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py
 django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py
 django_ticketbai/migrations/0010_alter_invoice_signature_value.py
 django_ticketbai/migrations/0011_alter_invoice_signature_value.py
 django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py
 django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py
 django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py
+django_ticketbai/migrations/0015_invoice_lang.py
 django_ticketbai/migrations/__init__.py
 django_ticketbai/templates/PDF/ticketbai.css
 django_ticketbai/templates/PDF/ticketbai.html
 django_ticketbai/templates/admin/django_ticketbai/app_index.html
 django_ticketbai/utils/__init__.py
 django_ticketbai/utils/invoice.py
 django_ticketbai/utils/pdf.py
```

### Comparing `django_ticketbai-1.4/setup.py` & `django_ticketbai-1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("LICENSE") as f:
     license = f.read()
 
 
 setup(
     name="django-ticketbai",
-    version="1.4",
+    version="1.5",
     description=(
         "django-ticketbai allows to create, manage, store and send TicketBai"
         " invoices to the Basque tax authorities."
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords="",
```

