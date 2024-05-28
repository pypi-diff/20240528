# Comparing `tmp/django-streamfield-2.2.0.tar.gz` & `tmp/django-streamfield-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-streamfield-2.2.0.tar", last modified: Tue May  7 13:40:35 2024, max compression
+gzip compressed data, was "django-streamfield-2.2.1.tar", last modified: Tue May 28 13:37:06 2024, max compression
```

## Comparing `django-streamfield-2.2.0.tar` & `django-streamfield-2.2.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.278529 django-streamfield-2.2.0/
--rw-r--r--   0 raagin     (501) staff       (20)     1309 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/LICENSE
--rw-r--r--   0 raagin     (501) staff       (20)      153 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/MANIFEST.in
--rw-r--r--   0 raagin     (501) staff       (20)    17393 2024-05-07 13:40:35.278316 django-streamfield-2.2.0/PKG-INFO
--rw-r--r--   0 raagin     (501) staff       (20)    16485 2024-05-06 18:59:33.000000 django-streamfield-2.2.0/README.md
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.271672 django-streamfield-2.2.0/django_streamfield.egg-info/
--rw-r--r--   0 raagin     (501) staff       (20)    17393 2024-05-07 13:40:35.000000 django-streamfield-2.2.0/django_streamfield.egg-info/PKG-INFO
--rw-r--r--   0 raagin     (501) staff       (20)     1731 2024-05-07 13:40:35.000000 django-streamfield-2.2.0/django_streamfield.egg-info/SOURCES.txt
--rw-r--r--   0 raagin     (501) staff       (20)        1 2024-05-07 13:40:35.000000 django-streamfield-2.2.0/django_streamfield.egg-info/dependency_links.txt
--rw-r--r--   0 raagin     (501) staff       (20)        1 2024-05-07 13:40:35.000000 django-streamfield-2.2.0/django_streamfield.egg-info/not-zip-safe
--rw-r--r--   0 raagin     (501) staff       (20)       12 2024-05-07 13:40:35.000000 django-streamfield-2.2.0/django_streamfield.egg-info/top_level.txt
--rw-r--r--   0 raagin     (501) staff       (20)       38 2024-05-07 13:40:35.278565 django-streamfield-2.2.0/setup.cfg
--rw-r--r--   0 raagin     (501) staff       (20)     1200 2024-05-06 18:59:40.000000 django-streamfield-2.2.0/setup.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.273431 django-streamfield-2.2.0/streamfield/
--rw-r--r--   0 raagin     (501) staff       (20)       38 2024-05-06 18:59:20.000000 django-streamfield-2.2.0/streamfield/__init__.py
--rw-r--r--   0 raagin     (501) staff       (20)     2917 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/admin.py
--rw-r--r--   0 raagin     (501) staff       (20)       95 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/apps.py
--rw-r--r--   0 raagin     (501) staff       (20)     9366 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/base.py
--rw-r--r--   0 raagin     (501) staff       (20)     3753 2023-11-08 08:04:34.000000 django-streamfield-2.2.0/streamfield/fields.py
--rw-r--r--   0 raagin     (501) staff       (20)      280 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/forms.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.270028 django-streamfield-2.2.0/streamfield/locale/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.269885 django-streamfield-2.2.0/streamfield/locale/en/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.273681 django-streamfield-2.2.0/streamfield/locale/en/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)      380 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     2618 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.269975 django-streamfield-2.2.0/streamfield/locale/it/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.273940 django-streamfield-2.2.0/streamfield/locale/it/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)     1855 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     3337 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.270062 django-streamfield-2.2.0/streamfield/locale/ru/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.274200 django-streamfield-2.2.0/streamfield/locale/ru/LC_MESSAGES/
--rw-r--r--   0 raagin     (501) staff       (20)     2398 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 raagin     (501) staff       (20)     4940 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 raagin     (501) staff       (20)       57 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/models.py
--rw-r--r--   0 raagin     (501) staff       (20)      706 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/settings.py
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.274347 django-streamfield-2.2.0/streamfield/static/
--rw-r--r--   0 raagin     (501) staff       (20)     6148 2024-05-07 09:37:08.000000 django-streamfield-2.2.0/streamfield/static/.DS_Store
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.275464 django-streamfield-2.2.0/streamfield/static/streamfield/
--rw-r--r--   0 raagin     (501) staff       (20)      267 2024-05-07 13:25:26.000000 django-streamfield-2.2.0/streamfield/static/streamfield/admin_popup_response.js
--rw-r--r--   0 raagin     (501) staff       (20)    10343 2024-05-07 13:25:26.000000 django-streamfield-2.2.0/streamfield/static/streamfield/streamfield_widget.css
--rw-r--r--   0 raagin     (501) staff       (20)   304296 2024-05-07 13:25:26.000000 django-streamfield-2.2.0/streamfield/static/streamfield/streamfield_widget.js
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.270291 django-streamfield-2.2.0/streamfield/templates/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.276578 django-streamfield-2.2.0/streamfield/templates/streamfield/
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.277221 django-streamfield-2.2.0/streamfield/templates/streamfield/admin/
--rw-r--r--   0 raagin     (501) staff       (20)        6 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/templates/streamfield/admin/abstract_block_template.html
--rw-r--r--   0 raagin     (501) staff       (20)     2306 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/templates/streamfield/admin/change_form.html
--rw-r--r--   0 raagin     (501) staff       (20)      371 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/templates/streamfield/admin/change_form_render_template.html
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.277779 django-streamfield-2.2.0/streamfield/templates/streamfield/admin/fields/
--rw-r--r--   0 raagin     (501) staff       (20)       33 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/templates/streamfield/admin/fields/default.html
--rw-r--r--   0 raagin     (501) staff       (20)     1022 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/templates/streamfield/admin/fields/file_browse_widget.html
--rw-r--r--   0 raagin     (501) staff       (20)       15 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/templates/streamfield/admin/fields/select.html
--rw-r--r--   0 raagin     (501) staff       (20)       71 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/templates/streamfield/admin/fields/stream_field_widget.html
--rw-r--r--   0 raagin     (501) staff       (20)      367 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/templates/streamfield/admin/streamfield_popup_response.html
--rw-r--r--   0 raagin     (501) staff       (20)      341 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/templates/streamfield/default_block_tmpl.html
--rw-r--r--   0 raagin     (501) staff       (20)      444 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/templates/streamfield/streamfield_admin_help.html
--rw-r--r--   0 raagin     (501) staff       (20)      978 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/templates/streamfield/streamfield_widget.html
-drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-07 13:40:35.278012 django-streamfield-2.2.0/streamfield/templatetags/
--rw-r--r--   0 raagin     (501) staff       (20)        0 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/templatetags/__init__.py
--rw-r--r--   0 raagin     (501) staff       (20)     1314 2024-03-19 08:42:15.000000 django-streamfield-2.2.0/streamfield/templatetags/streamfield_tags.py
--rw-r--r--   0 raagin     (501) staff       (20)       60 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/tests.py
--rw-r--r--   0 raagin     (501) staff       (20)      996 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/urls.py
--rw-r--r--   0 raagin     (501) staff       (20)     1977 2023-08-31 09:56:16.000000 django-streamfield-2.2.0/streamfield/views.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.741713 django-streamfield-2.2.1/
+-rw-r--r--   0 raagin     (501) staff       (20)     1309 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/LICENSE
+-rw-r--r--   0 raagin     (501) staff       (20)      153 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/MANIFEST.in
+-rw-r--r--   0 raagin     (501) staff       (20)    17393 2024-05-28 13:37:06.741397 django-streamfield-2.2.1/PKG-INFO
+-rw-r--r--   0 raagin     (501) staff       (20)    16485 2024-05-28 13:30:34.000000 django-streamfield-2.2.1/README.md
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.734679 django-streamfield-2.2.1/django_streamfield.egg-info/
+-rw-r--r--   0 raagin     (501) staff       (20)    17393 2024-05-28 13:37:06.000000 django-streamfield-2.2.1/django_streamfield.egg-info/PKG-INFO
+-rw-r--r--   0 raagin     (501) staff       (20)     1731 2024-05-28 13:37:06.000000 django-streamfield-2.2.1/django_streamfield.egg-info/SOURCES.txt
+-rw-r--r--   0 raagin     (501) staff       (20)        1 2024-05-28 13:37:06.000000 django-streamfield-2.2.1/django_streamfield.egg-info/dependency_links.txt
+-rw-r--r--   0 raagin     (501) staff       (20)        1 2024-05-07 13:40:35.000000 django-streamfield-2.2.1/django_streamfield.egg-info/not-zip-safe
+-rw-r--r--   0 raagin     (501) staff       (20)       12 2024-05-28 13:37:06.000000 django-streamfield-2.2.1/django_streamfield.egg-info/top_level.txt
+-rw-r--r--   0 raagin     (501) staff       (20)       38 2024-05-28 13:37:06.741749 django-streamfield-2.2.1/setup.cfg
+-rw-r--r--   0 raagin     (501) staff       (20)     1200 2024-05-28 13:30:31.000000 django-streamfield-2.2.1/setup.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.736564 django-streamfield-2.2.1/streamfield/
+-rw-r--r--   0 raagin     (501) staff       (20)       38 2024-05-28 13:30:16.000000 django-streamfield-2.2.1/streamfield/__init__.py
+-rw-r--r--   0 raagin     (501) staff       (20)     2917 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/admin.py
+-rw-r--r--   0 raagin     (501) staff       (20)       95 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/apps.py
+-rw-r--r--   0 raagin     (501) staff       (20)     9366 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/base.py
+-rw-r--r--   0 raagin     (501) staff       (20)     3753 2023-11-08 08:04:34.000000 django-streamfield-2.2.1/streamfield/fields.py
+-rw-r--r--   0 raagin     (501) staff       (20)      280 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/forms.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.732817 django-streamfield-2.2.1/streamfield/locale/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.732651 django-streamfield-2.2.1/streamfield/locale/en/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.736903 django-streamfield-2.2.1/streamfield/locale/en/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)      380 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     2618 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.732739 django-streamfield-2.2.1/streamfield/locale/it/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.737143 django-streamfield-2.2.1/streamfield/locale/it/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)     1855 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     3337 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.732856 django-streamfield-2.2.1/streamfield/locale/ru/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.737371 django-streamfield-2.2.1/streamfield/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 raagin     (501) staff       (20)     2398 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 raagin     (501) staff       (20)     4940 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 raagin     (501) staff       (20)       57 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/models.py
+-rw-r--r--   0 raagin     (501) staff       (20)      706 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/settings.py
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.737491 django-streamfield-2.2.1/streamfield/static/
+-rw-r--r--   0 raagin     (501) staff       (20)     6148 2024-05-07 09:37:08.000000 django-streamfield-2.2.1/streamfield/static/.DS_Store
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.738828 django-streamfield-2.2.1/streamfield/static/streamfield/
+-rw-r--r--   0 raagin     (501) staff       (20)      267 2024-05-07 13:25:26.000000 django-streamfield-2.2.1/streamfield/static/streamfield/admin_popup_response.js
+-rw-r--r--   0 raagin     (501) staff       (20)    10343 2024-05-07 13:25:26.000000 django-streamfield-2.2.1/streamfield/static/streamfield/streamfield_widget.css
+-rw-r--r--   0 raagin     (501) staff       (20)   304296 2024-05-07 13:25:26.000000 django-streamfield-2.2.1/streamfield/static/streamfield/streamfield_widget.js
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.733036 django-streamfield-2.2.1/streamfield/templates/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.739884 django-streamfield-2.2.1/streamfield/templates/streamfield/
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.740388 django-streamfield-2.2.1/streamfield/templates/streamfield/admin/
+-rw-r--r--   0 raagin     (501) staff       (20)        6 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/templates/streamfield/admin/abstract_block_template.html
+-rw-r--r--   0 raagin     (501) staff       (20)     2306 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/templates/streamfield/admin/change_form.html
+-rw-r--r--   0 raagin     (501) staff       (20)      371 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/templates/streamfield/admin/change_form_render_template.html
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.740896 django-streamfield-2.2.1/streamfield/templates/streamfield/admin/fields/
+-rw-r--r--   0 raagin     (501) staff       (20)       33 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/templates/streamfield/admin/fields/default.html
+-rw-r--r--   0 raagin     (501) staff       (20)     1022 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/templates/streamfield/admin/fields/file_browse_widget.html
+-rw-r--r--   0 raagin     (501) staff       (20)       15 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/templates/streamfield/admin/fields/select.html
+-rw-r--r--   0 raagin     (501) staff       (20)       71 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/templates/streamfield/admin/fields/stream_field_widget.html
+-rw-r--r--   0 raagin     (501) staff       (20)      367 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/templates/streamfield/admin/streamfield_popup_response.html
+-rw-r--r--   0 raagin     (501) staff       (20)      341 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/templates/streamfield/default_block_tmpl.html
+-rw-r--r--   0 raagin     (501) staff       (20)      444 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/templates/streamfield/streamfield_admin_help.html
+-rw-r--r--   0 raagin     (501) staff       (20)      978 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/templates/streamfield/streamfield_widget.html
+drwxr-xr-x   0 raagin     (501) staff       (20)        0 2024-05-28 13:37:06.741093 django-streamfield-2.2.1/streamfield/templatetags/
+-rw-r--r--   0 raagin     (501) staff       (20)        0 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/templatetags/__init__.py
+-rw-r--r--   0 raagin     (501) staff       (20)     1314 2024-03-19 08:42:15.000000 django-streamfield-2.2.1/streamfield/templatetags/streamfield_tags.py
+-rw-r--r--   0 raagin     (501) staff       (20)       60 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/tests.py
+-rw-r--r--   0 raagin     (501) staff       (20)      996 2023-08-31 09:56:16.000000 django-streamfield-2.2.1/streamfield/urls.py
+-rw-r--r--   0 raagin     (501) staff       (20)     1996 2024-05-28 13:28:00.000000 django-streamfield-2.2.1/streamfield/views.py
```

### Comparing `django-streamfield-2.2.0/LICENSE` & `django-streamfield-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/PKG-INFO` & `django-streamfield-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-streamfield
-Version: 2.2.0
+Version: 2.2.1
 Summary: StreamField for native Django Admin or with Grappelli
 Home-page: https://github.com/raagin/django-streamfield
 Author: Yury Lapshinov
 Author-email: y.raagin@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.2.0
+Stable version: 2.2.1
 Django <= 5.0
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.2.0/README.md` & `django-streamfield-2.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.2.0
+Stable version: 2.2.1
 Django <= 5.0
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.2.0/django_streamfield.egg-info/PKG-INFO` & `django-streamfield-2.2.1/django_streamfield.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-streamfield
-Version: 2.2.0
+Version: 2.2.1
 Summary: StreamField for native Django Admin or with Grappelli
 Home-page: https://github.com/raagin/django-streamfield
 Author: Yury Lapshinov
 Author-email: y.raagin@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django StreamField
 
 This is a simple realisation of StreamField's idea of Wagtail CMS for plain Django admin or with Grappelli skin.
-Stable version: 2.2.0
+Stable version: 2.2.1
 Django <= 5.0
 
 [Major changes (1.4.5 > 2)](changes2.0.md)
 
 ## Highlights
 You can build your page with different kind of blocks. 
 Sort them and sort the lists inside the blocks.
```

### Comparing `django-streamfield-2.2.0/django_streamfield.egg-info/SOURCES.txt` & `django-streamfield-2.2.1/django_streamfield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/setup.py` & `django-streamfield-2.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-streamfield",
-    version="2.2.0",
+    version="2.2.1",
     author="Yury Lapshinov",
     author_email="y.raagin@gmail.com",
     description="StreamField for native Django Admin or with Grappelli",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raagin/django-streamfield",
     packages=setuptools.find_packages(exclude=['test_project', 'frontend']),
```

### Comparing `django-streamfield-2.2.0/streamfield/admin.py` & `django-streamfield-2.2.1/streamfield/admin.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/base.py` & `django-streamfield-2.2.1/streamfield/base.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/fields.py` & `django-streamfield-2.2.1/streamfield/fields.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/locale/en/LC_MESSAGES/django.po` & `django-streamfield-2.2.1/streamfield/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/locale/it/LC_MESSAGES/django.mo` & `django-streamfield-2.2.1/streamfield/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/locale/it/LC_MESSAGES/django.po` & `django-streamfield-2.2.1/streamfield/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/locale/ru/LC_MESSAGES/django.mo` & `django-streamfield-2.2.1/streamfield/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/locale/ru/LC_MESSAGES/django.po` & `django-streamfield-2.2.1/streamfield/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/settings.py` & `django-streamfield-2.2.1/streamfield/settings.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/static/.DS_Store` & `django-streamfield-2.2.1/streamfield/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/static/streamfield/streamfield_widget.css` & `django-streamfield-2.2.1/streamfield/static/streamfield/streamfield_widget.css`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/static/streamfield/streamfield_widget.js` & `django-streamfield-2.2.1/streamfield/static/streamfield/streamfield_widget.js`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/templates/streamfield/admin/change_form.html` & `django-streamfield-2.2.1/streamfield/templates/streamfield/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/templates/streamfield/admin/fields/file_browse_widget.html` & `django-streamfield-2.2.1/streamfield/templates/streamfield/admin/fields/file_browse_widget.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/templates/streamfield/streamfield_widget.html` & `django-streamfield-2.2.1/streamfield/templates/streamfield/streamfield_widget.html`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/templatetags/streamfield_tags.py` & `django-streamfield-2.2.1/streamfield/templatetags/streamfield_tags.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/urls.py` & `django-streamfield-2.2.1/streamfield/urls.py`

 * *Files identical despite different names*

### Comparing `django-streamfield-2.2.0/streamfield/views.py` & `django-streamfield-2.2.1/streamfield/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,14 @@
         )
 
     return type(str(model.__name__ + 'TemplateView'), (base, ), attrs )
 
 
 def delete_instance(request, model_name, pk):
     model_class = apps.get_model(app_label='streamblocks', model_name=model_name)
-    obj = model_class.objects.get(pk=pk)
-    if request.method == 'DELETE':
+    obj = model_class.objects.filter(pk=pk).first()
+    if request.method == 'DELETE' and obj:
         obj.delete()
         resp = {'success': True}
     else:
         resp = {'success': False}
     return JsonResponse(resp)
```

