# Comparing `tmp/djangocms_oidc-4.1.0.tar.gz` & `tmp/djangocms_oidc-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms_oidc-4.1.0.tar", last modified: Mon May 27 12:55:53 2024, max compression
+gzip compressed data, was "djangocms_oidc-4.1.1.tar", last modified: Mon May 27 13:19:51 2024, max compression
```

## Comparing `djangocms_oidc-4.1.0.tar` & `djangocms_oidc-4.1.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.487322 djangocms_oidc-4.1.0/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    35147 2020-09-17 12:54:57.000000 djangocms_oidc-4.1.0/LICENSE
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      151 2020-09-17 12:54:57.000000 djangocms_oidc-4.1.0/MANIFEST.in
--rw-r--r--   0 zbohm     (1000) zbohm     (1000)     7342 2024-05-27 12:55:53.487322 djangocms_oidc-4.1.0/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5913 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/README.rst
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.479323 djangocms_oidc-4.1.0/djangocms_oidc/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/__init__.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc/admin/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      373 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/admin/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      638 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/admin/forms.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      413 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/admin/options.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    13210 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/auth.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4584 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.0/djangocms_oidc/cms_plugins.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      114 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/constants.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      701 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.0/djangocms_oidc/forms.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2637 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/helpers.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.479323 djangocms_oidc-4.1.0/djangocms_oidc/locale/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.479323 djangocms_oidc-4.1.0/djangocms_oidc/locale/cs/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    12113 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/locale/cs/LC_MESSAGES/django.po
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3511 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/middleware.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc/migrations/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9263 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/migrations/0001_initial.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2225 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/migrations/0002_30274_button_label.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/migrations/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    12191 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.0/djangocms_oidc/models.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.479323 djangocms_oidc-4.1.0/djangocms_oidc/templates/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/change_form/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3006 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/change_form/consumer.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      290 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/change_form/display_dedicated_content.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      386 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/change_form/list_identifiers.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      274 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/display_dedicated_content.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3515 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/handover_data.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      985 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/list_identifiers.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5291 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/login.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      128 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/show_attribute.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      236 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/show_attribute_country.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc/tests/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2455 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/settings.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2072 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_admin_forms.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      538 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_admin_options.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    27955 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_auth.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    32505 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_cms_plugins.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      878 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_forms.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5665 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_helpers.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    18721 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_middleware.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11065 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3726 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_utils.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    20601 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_views.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1126 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_widgets.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      698 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/urls.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      432 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/views.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1250 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/urls.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1525 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/utils.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8560 2024-04-24 10:59:39.000000 djangocms_oidc-4.1.0/djangocms_oidc/views.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      482 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.0/djangocms_oidc/widgets.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/
--rw-r--r--   0 zbohm     (1000) zbohm     (1000)     7342 2024-05-27 12:55:53.000000 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1992 2024-05-27 12:55:53.000000 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/SOURCES.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2024-05-27 12:55:53.000000 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/dependency_links.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2022-02-14 14:49:42.000000 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/not-zip-safe
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      144 2024-05-27 12:55:53.000000 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/requires.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       15 2024-05-27 12:55:53.000000 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/top_level.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      380 2024-05-27 12:55:53.487322 djangocms_oidc-4.1.0/setup.cfg
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1791 2024-05-27 12:55:31.000000 djangocms_oidc-4.1.0/setup.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 13:19:51.033290 djangocms_oidc-4.1.1/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    35147 2020-09-17 12:54:57.000000 djangocms_oidc-4.1.1/LICENSE
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      151 2020-09-17 12:54:57.000000 djangocms_oidc-4.1.1/MANIFEST.in
+-rw-r--r--   0 zbohm     (1000) zbohm     (1000)     7342 2024-05-27 13:19:51.033290 djangocms_oidc-4.1.1/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5913 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/README.rst
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 13:19:51.025289 djangocms_oidc-4.1.1/djangocms_oidc/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/__init__.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 13:19:51.029289 djangocms_oidc-4.1.1/djangocms_oidc/admin/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      373 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/admin/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      638 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/admin/forms.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      413 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/admin/options.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    13210 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/auth.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4584 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.1/djangocms_oidc/cms_plugins.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      114 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/constants.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      701 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.1/djangocms_oidc/forms.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2637 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/helpers.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 13:19:51.025289 djangocms_oidc-4.1.1/djangocms_oidc/locale/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 13:19:51.025289 djangocms_oidc-4.1.1/djangocms_oidc/locale/cs/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 13:19:51.029289 djangocms_oidc-4.1.1/djangocms_oidc/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    12113 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/locale/cs/LC_MESSAGES/django.po
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3511 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/middleware.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 13:19:51.029289 djangocms_oidc-4.1.1/djangocms_oidc/migrations/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9263 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/migrations/0001_initial.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2225 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/migrations/0002_30274_button_label.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/migrations/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    12327 2024-05-27 13:17:41.000000 djangocms_oidc-4.1.1/djangocms_oidc/models.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 13:19:51.025289 djangocms_oidc-4.1.1/djangocms_oidc/templates/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 13:19:51.029289 djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 13:19:51.029289 djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/change_form/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3006 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/change_form/consumer.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      290 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/change_form/display_dedicated_content.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      386 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/change_form/list_identifiers.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      274 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/display_dedicated_content.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3515 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/handover_data.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      985 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/list_identifiers.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5291 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/login.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      128 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/show_attribute.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      236 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/show_attribute_country.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 13:19:51.029289 djangocms_oidc-4.1.1/djangocms_oidc/tests/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2455 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/settings.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2072 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/test_admin_forms.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      538 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/test_admin_options.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    27955 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/test_auth.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    32505 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/test_cms_plugins.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      878 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/test_forms.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5665 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/test_helpers.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    18721 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/test_middleware.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11065 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/test_models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3726 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/test_utils.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    20601 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/test_views.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1126 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/test_widgets.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      698 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/urls.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      432 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.1/djangocms_oidc/tests/views.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1250 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/urls.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1525 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.1/djangocms_oidc/utils.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8560 2024-04-24 10:59:39.000000 djangocms_oidc-4.1.1/djangocms_oidc/views.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      482 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.1/djangocms_oidc/widgets.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 13:19:51.029289 djangocms_oidc-4.1.1/djangocms_oidc.egg-info/
+-rw-r--r--   0 zbohm     (1000) zbohm     (1000)     7342 2024-05-27 13:19:50.000000 djangocms_oidc-4.1.1/djangocms_oidc.egg-info/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1992 2024-05-27 13:19:51.000000 djangocms_oidc-4.1.1/djangocms_oidc.egg-info/SOURCES.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2024-05-27 13:19:50.000000 djangocms_oidc-4.1.1/djangocms_oidc.egg-info/dependency_links.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2022-02-14 14:49:42.000000 djangocms_oidc-4.1.1/djangocms_oidc.egg-info/not-zip-safe
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      144 2024-05-27 13:19:50.000000 djangocms_oidc-4.1.1/djangocms_oidc.egg-info/requires.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       15 2024-05-27 13:19:50.000000 djangocms_oidc-4.1.1/djangocms_oidc.egg-info/top_level.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      380 2024-05-27 13:19:51.033290 djangocms_oidc-4.1.1/setup.cfg
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1791 2024-05-27 13:19:26.000000 djangocms_oidc-4.1.1/setup.py
```

### Comparing `djangocms_oidc-4.1.0/LICENSE` & `djangocms_oidc-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/PKG-INFO` & `djangocms_oidc-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-oidc
-Version: 4.1.0
+Version: 4.1.1
 Summary: Plugin OIDC (OpenID Connect) into Django CMS.
 Home-page: https://github.com/CZ-NIC/djangocms-oidc
 Author: Zdeněk Böhm
 Author-email: zdenek.bohm@nic.cz
 License: GPL GNU License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `djangocms_oidc-4.1.0/README.rst` & `djangocms_oidc-4.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/admin/forms.py` & `djangocms_oidc-4.1.1/djangocms_oidc/admin/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/auth.py` & `djangocms_oidc-4.1.1/djangocms_oidc/auth.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/cms_plugins.py` & `djangocms_oidc-4.1.1/djangocms_oidc/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/forms.py` & `djangocms_oidc-4.1.1/djangocms_oidc/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/helpers.py` & `djangocms_oidc-4.1.1/djangocms_oidc/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/locale/cs/LC_MESSAGES/django.po` & `djangocms_oidc-4.1.1/djangocms_oidc/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/middleware.py` & `djangocms_oidc-4.1.1/djangocms_oidc/middleware.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/migrations/0001_initial.py` & `djangocms_oidc-4.1.1/djangocms_oidc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/migrations/0002_30274_button_label.py` & `djangocms_oidc-4.1.1/djangocms_oidc/migrations/0002_30274_button_label.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/models.py` & `djangocms_oidc-4.1.1/djangocms_oidc/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,19 @@
             if not isinstance(datadict["essential"], bool):
                 raise ValidationError(
                     _('The value of "essential" must be a boolean type": "%(key)s": {"essential": true},'),
                     params={'key': key}
                 )
 
 
+def get_default_claim() -> dict[str, str]:
+    """Get default claim."""
+    return {"userinfo": {"openid2_id": {"essential": True}}}
+
+
 class OIDCHandoverDataBase(CMSPlugin):
 
     consumer_type = HANDOVER_DATA
     AUTHORIZATION_PROMPT = (
         ('none', _('No interaction')),
         ('login', _('Force login')),
         ('consent', _('Force consent with handovered data')),
@@ -206,15 +211,15 @@
 
     provider = models.ForeignKey(OIDCProvider, on_delete=models.CASCADE)
     button_label = models.CharField(
         verbose_name=_('Button label'), max_length=80, null=True, blank=True,
         help_text=_("Button text for unlogged in user."))
     claims = models.JSONField(
         verbose_name=_("Claims"), validators=[validate_claims], help_text=_("Claims attributes for data handover."),
-        default={"userinfo": {}})
+        default=get_default_claim)
     insist_on_required_claims = models.BooleanField(
         verbose_name=_("Insist on required claims"), default=False,
         help_text=_("Consider the data invalid if not all the required data has been handovered."))
     verified_by = models.CharField(
         verbose_name=_('Verified by names'), max_length=255, null=True, blank=True,
         help_text=_("Verified by names (separated by space)."))
     redirect_page = PageField(verbose_name=_('CMS Page'), blank=True, null=True, on_delete=models.SET_NULL,
```

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/change_form/consumer.html` & `djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/change_form/consumer.html`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/handover_data.html` & `djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/handover_data.html`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/list_identifiers.html` & `djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/list_identifiers.html`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/login.html` & `djangocms_oidc-4.1.1/djangocms_oidc/templates/djangocms_oidc/login.html`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/settings.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_admin_forms.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/test_admin_forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_admin_options.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/test_admin_options.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_auth.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_cms_plugins.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/test_cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_forms.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_helpers.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_middleware.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_models.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_utils.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_views.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_widgets.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/tests/urls.py` & `djangocms_oidc-4.1.1/djangocms_oidc/tests/urls.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/urls.py` & `djangocms_oidc-4.1.1/djangocms_oidc/urls.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/utils.py` & `djangocms_oidc-4.1.1/djangocms_oidc/utils.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc/views.py` & `djangocms_oidc-4.1.1/djangocms_oidc/views.py`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc.egg-info/PKG-INFO` & `djangocms_oidc-4.1.1/djangocms_oidc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-oidc
-Version: 4.1.0
+Version: 4.1.1
 Summary: Plugin OIDC (OpenID Connect) into Django CMS.
 Home-page: https://github.com/CZ-NIC/djangocms-oidc
 Author: Zdeněk Böhm
 Author-email: zdenek.bohm@nic.cz
 License: GPL GNU License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `djangocms_oidc-4.1.0/djangocms_oidc.egg-info/SOURCES.txt` & `djangocms_oidc-4.1.1/djangocms_oidc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms_oidc-4.1.0/setup.py` & `djangocms_oidc-4.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     sub_commands = [("compile_catalog", lambda x: True)] + build.sub_commands
 
 
 setup(
     author='Zdeněk Böhm',
     author_email='zdenek.bohm@nic.cz',
     name='djangocms-oidc',
-    version='4.1.0',
+    version='4.1.1',
     description='Plugin OIDC (OpenID Connect) into Django CMS.',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     url='https://github.com/CZ-NIC/djangocms-oidc',
     license='GPL GNU License',
     platforms=['OS Independent'],
     classifiers=(
```

