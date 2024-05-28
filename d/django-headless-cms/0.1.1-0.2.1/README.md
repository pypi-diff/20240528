# Comparing `tmp/django_headless_cms-0.1.1.tar.gz` & `tmp/django_headless_cms-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_headless_cms-0.1.1.tar", max compression
+gzip compressed data, was "django_headless_cms-0.2.1.tar", max compression
```

## Comparing `django_headless_cms-0.1.1.tar` & `django_headless_cms-0.2.1.tar`

### file list

```diff
@@ -1,75 +1,78 @@
--rw-r--r--   0        0        0     1521 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/LICENSE
--rw-r--r--   0        0        0      925 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/__init__.py
--rw-r--r--   0        0        0    14062 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/admin.py
--rw-r--r--   0        0        0       71 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/auto_translate/__init__.py
--rw-r--r--   0        0        0     4029 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/auto_translate/base_translate.py
--rw-r--r--   0        0        0     3617 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/auto_translate/openai_translate.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_metadata/__init__.py
--rw-r--r--   0        0        0      376 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_metadata/admin.py
--rw-r--r--   0        0        0     9496 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_metadata/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_metadata/migrations/__init__.py
--rw-r--r--   0        0        0     2695 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_metadata/models.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/__init__.py
--rw-r--r--   0        0        0      365 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/admin.py
--rw-r--r--   0        0        0    11108 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0001_initial.py
--rw-r--r--   0        0        0    12374 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0002_initial.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/__init__.py
--rw-r--r--   0        0        0     6212 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/models.py
--rw-r--r--   0        0        0     1327 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/views.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/__init__.py
--rw-r--r--   0        0        0      277 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/admin.py
--rw-r--r--   0        0        0    10936 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/migrations/__init__.py
--rw-r--r--   0        0        0     2413 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/models.py
--rw-r--r--   0        0        0      638 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/serializers.py
--rw-r--r--   0        0        0      369 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/urls.py
--rw-r--r--   0        0        0     2093 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/views.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/__init__.py
--rw-r--r--   0        0        0     1859 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/admin.py
--rw-r--r--   0        0        0    75728 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/migrations/__init__.py
--rw-r--r--   0        0        0    15115 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/models.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/shared/__init__.py
--rw-r--r--   0        0        0      226 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/shared/serializers.py
--rw-r--r--   0        0        0      736 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/urls.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/core/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/core/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/core/management/commands/__init__.py
--rw-r--r--   0        0        0     2558 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/core/management/commands/clean_outdated_drafts.py
--rw-r--r--   0        0        0     3912 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/core/management/commands/export_cms_data.py
--rw-r--r--   0        0        0     5165 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/core/management/commands/import_cms_data.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/__init__.py
--rw-r--r--   0        0        0     3003 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/static/localized_fields/localized-fields-admin.js
--rw-r--r--   0        0        0     1633 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/templates/admin/change_form.html
--rw-r--r--   0        0        0       67 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/templates/adminsortable2/edit_inline/stacked-django-5.0.html
--rw-r--r--   0        0        0       67 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/templates/adminsortable2/edit_inline/tabular-django-5.0.html
--rw-r--r--   0        0        0      689 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/templates/custom_localized_fields/admin/widget.html
--rw-r--r--   0        0        0     2115 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/templates/reversion/object_history.html
--rw-r--r--   0        0        0     1245 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/templates/reversion/revision_form.html
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/fields/__init__.py
--rw-r--r--   0        0        0     1352 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/fields/boolean_field.py
--rw-r--r--   0        0        0      559 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/fields/martor_field.py
--rw-r--r--   0        0        0      753 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/fields/slug_field.py
--rw-r--r--   0        0        0       89 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/fields/url_field.py
--rw-r--r--   0        0        0      452 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/forms.py
--rw-r--r--   0        0        0      302 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/mixins.py
--rw-r--r--   0        0        0     7213 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/models.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/schema/__init__.py
--rw-r--r--   0        0        0      490 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/schema/auto_schema.py
--rw-r--r--   0        0        0      314 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/schema/preprocessing_hooks.py
--rw-r--r--   0        0        0      831 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/schema/urls.py
--rw-r--r--   0        0        0      285 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/schema/views.py
--rw-r--r--   0        0        0      883 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/serializer_fields.py
--rw-r--r--   0        0        0     5802 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/serializers.py
--rw-r--r--   0        0        0     1028 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/settings.py
--rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/utils/__init__.py
--rw-r--r--   0        0        0     1954 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/utils/custom_import_export.py
--rw-r--r--   0        0        0     1003 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/utils/markdown.py
--rw-r--r--   0        0        0     2033 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/utils/martor_custom_upload.py
--rw-r--r--   0        0        0     2449 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/utils/relations.py
--rw-r--r--   0        0        0     5424 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/widgets.py
--rw-r--r--   0        0        0     3909 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4673 1970-01-01 00:00:00.000000 django_headless_cms-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1521 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/LICENSE
+-rw-r--r--   0        0        0      925 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/__init__.py
+-rw-r--r--   0        0        0    14062 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/admin.py
+-rw-r--r--   0        0        0       71 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/auto_translate/__init__.py
+-rw-r--r--   0        0        0     4029 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/auto_translate/base_translate.py
+-rw-r--r--   0        0        0     3617 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/auto_translate/openai_translate.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/__init__.py
+-rw-r--r--   0        0        0      376 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/admin.py
+-rw-r--r--   0        0        0     9496 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/migrations/__init__.py
+-rw-r--r--   0        0        0     2695 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/models.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/__init__.py
+-rw-r--r--   0        0        0      365 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/admin.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/management/commands/__init__.py
+-rw-r--r--   0        0        0     1115 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/management/commands/populate_aw_data.py
+-rw-r--r--   0        0        0    11108 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0001_initial.py
+-rw-r--r--   0        0        0    12374 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0002_initial.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/__init__.py
+-rw-r--r--   0        0        0     6212 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/models.py
+-rw-r--r--   0        0        0     1327 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/views.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/admin.py
+-rw-r--r--   0        0        0    10936 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/migrations/__init__.py
+-rw-r--r--   0        0        0     2413 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/models.py
+-rw-r--r--   0        0        0      638 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/serializers.py
+-rw-r--r--   0        0        0      369 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/urls.py
+-rw-r--r--   0        0        0     2093 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/views.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/__init__.py
+-rw-r--r--   0        0        0     1859 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/admin.py
+-rw-r--r--   0        0        0    75728 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/migrations/__init__.py
+-rw-r--r--   0        0        0    15115 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/models.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/shared/__init__.py
+-rw-r--r--   0        0        0      226 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/shared/serializers.py
+-rw-r--r--   0        0        0      736 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/contrib/astrowind/urls.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     2558 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/core/management/commands/clean_outdated_drafts.py
+-rw-r--r--   0        0        0     3912 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/core/management/commands/export_cms_data.py
+-rw-r--r--   0        0        0     5165 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/core/management/commands/import_cms_data.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/__init__.py
+-rw-r--r--   0        0        0     3003 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/static/localized_fields/localized-fields-admin.js
+-rw-r--r--   0        0        0     1633 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/templates/admin/change_form.html
+-rw-r--r--   0        0        0       67 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/templates/adminsortable2/edit_inline/stacked-django-5.0.html
+-rw-r--r--   0        0        0       67 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/templates/adminsortable2/edit_inline/tabular-django-5.0.html
+-rw-r--r--   0        0        0      689 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/templates/custom_localized_fields/admin/widget.html
+-rw-r--r--   0        0        0     2115 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/templates/reversion/object_history.html
+-rw-r--r--   0        0        0     1245 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/enhances/templates/reversion/revision_form.html
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/fields/__init__.py
+-rw-r--r--   0        0        0     1352 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/fields/boolean_field.py
+-rw-r--r--   0        0        0      559 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/fields/martor_field.py
+-rw-r--r--   0        0        0      753 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/fields/slug_field.py
+-rw-r--r--   0        0        0       89 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/fields/url_field.py
+-rw-r--r--   0        0        0      452 2024-05-28 15:13:45.693369 django_headless_cms-0.2.1/headless_cms/forms.py
+-rw-r--r--   0        0        0      302 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/mixins.py
+-rw-r--r--   0        0        0     7213 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/models.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/schema/__init__.py
+-rw-r--r--   0        0        0      490 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/schema/auto_schema.py
+-rw-r--r--   0        0        0      314 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/schema/preprocessing_hooks.py
+-rw-r--r--   0        0        0      831 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/schema/urls.py
+-rw-r--r--   0        0        0      285 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/schema/views.py
+-rw-r--r--   0        0        0      883 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/serializer_fields.py
+-rw-r--r--   0        0        0     5802 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/serializers.py
+-rw-r--r--   0        0        0     1028 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/settings.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/utils/__init__.py
+-rw-r--r--   0        0        0     1954 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/utils/custom_import_export.py
+-rw-r--r--   0        0        0     1003 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/utils/markdown.py
+-rw-r--r--   0        0        0     2033 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/utils/martor_custom_upload.py
+-rw-r--r--   0        0        0     2449 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/utils/relations.py
+-rw-r--r--   0        0        0     5424 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/headless_cms/widgets.py
+-rw-r--r--   0        0        0     3909 2024-05-28 15:13:45.697369 django_headless_cms-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4673 1970-01-01 00:00:00.000000 django_headless_cms-0.2.1/PKG-INFO
```

### Comparing `django_headless_cms-0.1.1/LICENSE` & `django_headless_cms-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/README.md` & `django_headless_cms-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/admin.py` & `django_headless_cms-0.2.1/headless_cms/admin.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/auto_translate/base_translate.py` & `django_headless_cms-0.2.1/headless_cms/auto_translate/base_translate.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/auto_translate/openai_translate.py` & `django_headless_cms-0.2.1/headless_cms/auto_translate/openai_translate.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_metadata/migrations/0001_initial.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_metadata/models.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_metadata/models.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0001_initial.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0002_initial.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/models.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/models.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/views.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_pages/views.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/migrations/0001_initial.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/models.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/models.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/serializers.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/serializers.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/views.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_posts/views.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/admin.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/admin.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/migrations/0001_initial.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/models.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/astrowind_widgets/models.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/contrib/astrowind/urls.py` & `django_headless_cms-0.2.1/headless_cms/contrib/astrowind/urls.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/core/management/commands/clean_outdated_drafts.py` & `django_headless_cms-0.2.1/headless_cms/core/management/commands/clean_outdated_drafts.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/core/management/commands/export_cms_data.py` & `django_headless_cms-0.2.1/headless_cms/core/management/commands/export_cms_data.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/core/management/commands/import_cms_data.py` & `django_headless_cms-0.2.1/headless_cms/core/management/commands/import_cms_data.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/enhances/static/localized_fields/localized-fields-admin.js` & `django_headless_cms-0.2.1/headless_cms/enhances/static/localized_fields/localized-fields-admin.js`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/enhances/templates/admin/change_form.html` & `django_headless_cms-0.2.1/headless_cms/enhances/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/enhances/templates/custom_localized_fields/admin/widget.html` & `django_headless_cms-0.2.1/headless_cms/enhances/templates/custom_localized_fields/admin/widget.html`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/enhances/templates/reversion/object_history.html` & `django_headless_cms-0.2.1/headless_cms/enhances/templates/reversion/object_history.html`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/enhances/templates/reversion/revision_form.html` & `django_headless_cms-0.2.1/headless_cms/enhances/templates/reversion/revision_form.html`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/fields/boolean_field.py` & `django_headless_cms-0.2.1/headless_cms/fields/boolean_field.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/fields/martor_field.py` & `django_headless_cms-0.2.1/headless_cms/fields/martor_field.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/fields/slug_field.py` & `django_headless_cms-0.2.1/headless_cms/fields/slug_field.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/models.py` & `django_headless_cms-0.2.1/headless_cms/models.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/schema/urls.py` & `django_headless_cms-0.2.1/headless_cms/schema/urls.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/serializer_fields.py` & `django_headless_cms-0.2.1/headless_cms/serializer_fields.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/serializers.py` & `django_headless_cms-0.2.1/headless_cms/serializers.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/settings.py` & `django_headless_cms-0.2.1/headless_cms/settings.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/utils/custom_import_export.py` & `django_headless_cms-0.2.1/headless_cms/utils/custom_import_export.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/utils/markdown.py` & `django_headless_cms-0.2.1/headless_cms/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/utils/martor_custom_upload.py` & `django_headless_cms-0.2.1/headless_cms/utils/martor_custom_upload.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/utils/relations.py` & `django_headless_cms-0.2.1/headless_cms/utils/relations.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/headless_cms/widgets.py` & `django_headless_cms-0.2.1/headless_cms/widgets.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.1.1/pyproject.toml` & `django_headless_cms-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 ]
 
 [tool.poetry]
 name = 'headless_cms'
 packages = [
   {include = "headless_cms"}
 ]
-version = "0.1.1"
+version = "0.2.1"
 
 [tool.poetry.group.dev.dependencies]
 commitizen = "^3.27.0"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = ">=7.0.0,<8"
 sphinx_rtd_theme = "*"
```

### Comparing `django_headless_cms-0.1.1/PKG-INFO` & `django_headless_cms-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-headless-cms
-Version: 0.1.1
+Version: 0.2.1
 Summary: A simple django-based headless CMS.
 Home-page: https://github.com/huynguyengl99/django-headless-cms
 License: Copyright © 2024-present, Huy Nguyen <danghuy1999@gmail.com>.
          
          All rights reserved.
          
          Redistribution and use in source and binary forms, with or without
```

