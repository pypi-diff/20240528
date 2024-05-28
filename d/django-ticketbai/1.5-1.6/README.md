# Comparing `tmp/django_ticketbai-1.5.tar.gz` & `tmp/django_ticketbai-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ticketbai-1.5.tar", last modified: Tue May 28 09:55:11 2024, max compression
+gzip compressed data, was "django_ticketbai-1.6.tar", last modified: Tue May 28 11:42:38 2024, max compression
```

## Comparing `django_ticketbai-1.5.tar` & `django_ticketbai-1.6.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.404110 django_ticketbai-1.5/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:04.000000 django_ticketbai-1.5/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-28 09:55:04.000000 django_ticketbai-1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 09:55:04.000000 django_ticketbai-1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-28 09:55:11.404110 django_ticketbai-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 09:55:04.000000 django_ticketbai-1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.396110 django_ticketbai-1.5/django_ticketbai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.400110 django_ticketbai-1.5/django_ticketbai/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0006_config_is_active.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0007_invoice_errorxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0010_alter_invoice_signature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0011_alter_invoice_signature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/0015_invoice_lang.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.392110 django_ticketbai-1.5/django_ticketbai/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.400110 django_ticketbai-1.5/django_ticketbai/templates/PDF/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/templates/PDF/ticketbai.css
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/templates/PDF/ticketbai.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.392110 django_ticketbai-1.5/django_ticketbai/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.400110 django_ticketbai-1.5/django_ticketbai/templates/admin/django_ticketbai/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/templates/admin/django_ticketbai/app_index.html
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.400110 django_ticketbai-1.5/django_ticketbai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/utils/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/utils/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-28 09:55:04.000000 django_ticketbai-1.5/django_ticketbai/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:55:11.404110 django_ticketbai-1.5/django_ticketbai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-28 09:55:11.000000 django_ticketbai-1.5/django_ticketbai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-28 09:55:11.000000 django_ticketbai-1.5/django_ticketbai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:55:11.000000 django_ticketbai-1.5/django_ticketbai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 09:55:11.000000 django_ticketbai-1.5/django_ticketbai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 09:55:11.000000 django_ticketbai-1.5/django_ticketbai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:55:11.404110 django_ticketbai-1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-28 09:55:04.000000 django_ticketbai-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:38.015027 django_ticketbai-1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:26.000000 django_ticketbai-1.6/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-28 11:42:26.000000 django_ticketbai-1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-28 11:42:26.000000 django_ticketbai-1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-28 11:42:38.015027 django_ticketbai-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 11:42:26.000000 django_ticketbai-1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:38.007027 django_ticketbai-1.6/django_ticketbai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:38.007027 django_ticketbai-1.6/django_ticketbai/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:38.007027 django_ticketbai-1.6/django_ticketbai/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:38.011027 django_ticketbai-1.6/django_ticketbai/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:38.011027 django_ticketbai-1.6/django_ticketbai/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0006_config_is_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0007_invoice_errorxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0010_alter_invoice_signature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0011_alter_invoice_signature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/0015_invoice_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:38.007027 django_ticketbai-1.6/django_ticketbai/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:38.011027 django_ticketbai-1.6/django_ticketbai/templates/PDF/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/templates/PDF/ticketbai.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/templates/PDF/ticketbai.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:38.007027 django_ticketbai-1.6/django_ticketbai/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:38.011027 django_ticketbai-1.6/django_ticketbai/templates/admin/django_ticketbai/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/templates/admin/django_ticketbai/app_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:38.015027 django_ticketbai-1.6/django_ticketbai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/utils/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/utils/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-28 11:42:26.000000 django_ticketbai-1.6/django_ticketbai/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:38.015027 django_ticketbai-1.6/django_ticketbai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-28 11:42:37.000000 django_ticketbai-1.6/django_ticketbai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-28 11:42:38.000000 django_ticketbai-1.6/django_ticketbai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:42:37.000000 django_ticketbai-1.6/django_ticketbai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 11:42:37.000000 django_ticketbai-1.6/django_ticketbai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 11:42:37.000000 django_ticketbai-1.6/django_ticketbai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:42:38.015027 django_ticketbai-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-28 11:42:26.000000 django_ticketbai-1.6/setup.py
```

### Comparing `django_ticketbai-1.5/LICENSE` & `django_ticketbai-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/PKG-INFO` & `django_ticketbai-1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ticketbai
-Version: 1.5
+Version: 1.6
 Summary: django-ticketbai allows to create, manage, store and send TicketBai invoices to the Basque tax authorities.
 Home-page: https://github.com/codesyntax/django-ticketbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `django_ticketbai-1.5/django_ticketbai/admin.py` & `django_ticketbai-1.6/django_ticketbai/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
                 "fields": (
                     "serial_code",
                     "num",
                     "description",
                     "total_amount",
                     "vat_breakdown",
                     "email",
+                    "lang",
                 )
             },
         ),
         (
             _("Dates"),
             {
                 "fields": (
```

### Comparing `django_ticketbai-1.5/django_ticketbai/migrations/0001_initial.py` & `django_ticketbai-1.6/django_ticketbai/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py` & `django_ticketbai-1.6/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py` & `django_ticketbai-1.6/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py` & `django_ticketbai-1.6/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py` & `django_ticketbai-1.6/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py` & `django_ticketbai-1.6/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py` & `django_ticketbai-1.6/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/migrations/0010_alter_invoice_signature_value.py` & `django_ticketbai-1.6/django_ticketbai/migrations/0010_alter_invoice_signature_value.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py` & `django_ticketbai-1.6/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py` & `django_ticketbai-1.6/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py` & `django_ticketbai-1.6/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/models.py` & `django_ticketbai-1.6/django_ticketbai/models.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/templates/PDF/ticketbai.html` & `django_ticketbai-1.6/django_ticketbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/utils/invoice.py` & `django_ticketbai-1.6/django_ticketbai/utils/invoice.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/utils/pdf.py` & `django_ticketbai-1.6/django_ticketbai/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/validators.py` & `django_ticketbai-1.6/django_ticketbai/validators.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai/views.py` & `django_ticketbai-1.6/django_ticketbai/views.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.5/django_ticketbai.egg-info/PKG-INFO` & `django_ticketbai-1.6/django_ticketbai.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ticketbai
-Version: 1.5
+Version: 1.6
 Summary: django-ticketbai allows to create, manage, store and send TicketBai invoices to the Basque tax authorities.
 Home-page: https://github.com/codesyntax/django-ticketbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `django_ticketbai-1.5/django_ticketbai.egg-info/SOURCES.txt` & `django_ticketbai-1.6/django_ticketbai.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 django_ticketbai/validators.py
 django_ticketbai/views.py
 django_ticketbai.egg-info/PKG-INFO
 django_ticketbai.egg-info/SOURCES.txt
 django_ticketbai.egg-info/dependency_links.txt
 django_ticketbai.egg-info/requires.txt
 django_ticketbai.egg-info/top_level.txt
+django_ticketbai/locale/eu/LC_MESSAGES/django.mo
+django_ticketbai/locale/eu/LC_MESSAGES/django.po
 django_ticketbai/migrations/0001_initial.py
 django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py
 django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py
 django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py
 django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py
 django_ticketbai/migrations/0006_config_is_active.py
 django_ticketbai/migrations/0007_invoice_errorxml.py
```

### Comparing `django_ticketbai-1.5/setup.py` & `django_ticketbai-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("LICENSE") as f:
     license = f.read()
 
 
 setup(
     name="django-ticketbai",
-    version="1.5",
+    version="1.6",
     description=(
         "django-ticketbai allows to create, manage, store and send TicketBai"
         " invoices to the Basque tax authorities."
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords="",
```

