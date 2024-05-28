# Comparing `tmp/PDFFiller-0.2.3.tar.gz` & `tmp/pdffiller-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDFFiller-0.2.3.tar", last modified: Thu Mar 14 07:17:21 2024, max compression
+gzip compressed data, was "pdffiller-0.2.4.tar", last modified: Tue May 28 09:10:48 2024, max compression
```

## Comparing `PDFFiller-0.2.3.tar` & `pdffiller-0.2.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.752183 PDFFiller-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.740183 PDFFiller-0.2.3/PDFFiller/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.740183 PDFFiller-0.2.3/PDFFiller/attributes/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/attributes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/attributes/color.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/attributes/dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/attributes/font.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/attributes/position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.744183 PDFFiller-0.2.3/PDFFiller/components/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.744183 PDFFiller-0.2.3/PDFFiller/components/check_mark/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/check_mark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/check_mark/check_mark.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/check_mark/check_mark_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/check_mark/check_mark_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.744183 PDFFiller-0.2.3/PDFFiller/components/debug_box/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/debug_box/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/debug_box/debug_box.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/debug_box/debug_box_theme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.744183 PDFFiller-0.2.3/PDFFiller/components/image_box/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/image_box/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/image_box/image_box.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/image_box/image_box_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/image_box/image_box_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.744183 PDFFiller-0.2.3/PDFFiller/components/signing_area/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/signing_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/signing_area/signing_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/signing_area/signing_area_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/signing_area/signing_area_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.744183 PDFFiller-0.2.3/PDFFiller/components/text_field/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/text_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/text_field/text_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/text_field/text_field_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/components/text_field/text_field_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.748183 PDFFiller-0.2.3/PDFFiller/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/constants/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/constants/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.748183 PDFFiller-0.2.3/PDFFiller/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.748183 PDFFiller-0.2.3/PDFFiller/core/build_service/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/build_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/build_service/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.748183 PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/build_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/check_mark_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/debug_box_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/image_box_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/signing_area_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/text_field_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.748183 PDFFiller-0.2.3/PDFFiller/core/export_service/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/export_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/export_service/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.748183 PDFFiller-0.2.3/PDFFiller/core/export_service/fitz_export_service/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/export_service/fitz_export_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/export_service/fitz_export_service/export_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/pdf_filler.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.748183 PDFFiller-0.2.3/PDFFiller/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/helpers/fitz_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/helpers/load_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/helpers/load_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/helpers/performance_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.748183 PDFFiller-0.2.3/PDFFiller/theme/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/PDFFiller/theme/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.748183 PDFFiller-0.2.3/PDFFiller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-03-14 07:17:21.000000 PDFFiller-0.2.3/PDFFiller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-03-14 07:17:21.000000 PDFFiller-0.2.3/PDFFiller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 07:17:21.000000 PDFFiller-0.2.3/PDFFiller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-14 07:17:21.000000 PDFFiller-0.2.3/PDFFiller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-14 07:17:21.000000 PDFFiller-0.2.3/PDFFiller.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-03-14 07:17:21.752183 PDFFiller-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.740183 PDFFiller-0.2.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:21.748183 PDFFiller-0.2.3/examples/build/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/examples/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 07:17:21.752183 PDFFiller-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-14 07:17:13.000000 PDFFiller-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.053069 pdffiller-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-28 09:10:39.000000 pdffiller-0.2.4/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.041069 pdffiller-0.2.4/PDFFiller/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.045069 pdffiller-0.2.4/PDFFiller/attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/attributes/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/attributes/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/attributes/font.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/attributes/position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.045069 pdffiller-0.2.4/PDFFiller/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.045069 pdffiller-0.2.4/PDFFiller/components/check_mark/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/check_mark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/check_mark/check_mark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/check_mark/check_mark_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/check_mark/check_mark_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.045069 pdffiller-0.2.4/PDFFiller/components/debug_box/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/debug_box/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/debug_box/debug_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/debug_box/debug_box_theme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.045069 pdffiller-0.2.4/PDFFiller/components/image_box/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/image_box/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/image_box/image_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/image_box/image_box_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/image_box/image_box_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.045069 pdffiller-0.2.4/PDFFiller/components/signing_area/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/signing_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/signing_area/signing_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/signing_area/signing_area_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/signing_area/signing_area_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.049070 pdffiller-0.2.4/PDFFiller/components/text_field/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/text_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/text_field/text_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/text_field/text_field_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/components/text_field/text_field_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.049070 pdffiller-0.2.4/PDFFiller/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/constants/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/constants/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.049070 pdffiller-0.2.4/PDFFiller/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.049070 pdffiller-0.2.4/PDFFiller/core/build_service/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/build_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/build_service/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.049070 pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/build_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/check_mark_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/debug_box_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/image_box_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/signing_area_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/text_field_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.049070 pdffiller-0.2.4/PDFFiller/core/export_service/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/export_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/export_service/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.053069 pdffiller-0.2.4/PDFFiller/core/export_service/fitz_export_service/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/export_service/fitz_export_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/export_service/fitz_export_service/export_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/pdf_filler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.053069 pdffiller-0.2.4/PDFFiller/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/helpers/fitz_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/helpers/load_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/helpers/load_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/helpers/performance_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.053069 pdffiller-0.2.4/PDFFiller/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-28 09:10:39.000000 pdffiller-0.2.4/PDFFiller/theme/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.053069 pdffiller-0.2.4/PDFFiller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-28 09:10:48.000000 pdffiller-0.2.4/PDFFiller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-28 09:10:48.000000 pdffiller-0.2.4/PDFFiller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:10:48.000000 pdffiller-0.2.4/PDFFiller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 09:10:48.000000 pdffiller-0.2.4/PDFFiller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 09:10:48.000000 pdffiller-0.2.4/PDFFiller.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-28 09:10:48.053069 pdffiller-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-05-28 09:10:39.000000 pdffiller-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.041069 pdffiller-0.2.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:48.053069 pdffiller-0.2.4/examples/build/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:10:39.000000 pdffiller-0.2.4/examples/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:10:48.053069 pdffiller-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-28 09:10:39.000000 pdffiller-0.2.4/setup.py
```

### Comparing `PDFFiller-0.2.3/LICENSE.md` & `pdffiller-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/build_service.py` & `pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/build_service.py`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/check_mark_builder.py` & `pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/check_mark_builder.py`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/debug_box_builder.py` & `pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/debug_box_builder.py`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/image_box_builder.py` & `pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/image_box_builder.py`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/signing_area_builder.py` & `pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/signing_area_builder.py`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PDFFiller/core/build_service/fitz_build_service/text_field_builder.py` & `pdffiller-0.2.4/PDFFiller/core/build_service/fitz_build_service/text_field_builder.py`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PDFFiller/core/export_service/fitz_export_service/export_service.py` & `pdffiller-0.2.4/PDFFiller/core/export_service/fitz_export_service/export_service.py`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PDFFiller/core/pdf_filler.py` & `pdffiller-0.2.4/PDFFiller/core/pdf_filler.py`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PDFFiller/helpers/fitz_helper.py` & `pdffiller-0.2.4/PDFFiller/helpers/fitz_helper.py`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PDFFiller/helpers/load_fields.py` & `pdffiller-0.2.4/PDFFiller/helpers/load_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     with open(path, 'r') as stream:
         data_loaded = yaml.safe_load(stream)
         for text_field in data_loaded.get("text_fields", []):
             dimension = text_field.get("dimension")
             font = text_field.get("font")
             field = TextField(
                 key=text_field.get("key"),
+                tag=text_field.get("tag"),
                 value=text_field.get("value"),
                 position=Position(**text_field.get("position"))
             )
             if dimension:
                 field.dimension = Dimension(**dimension)
             if font:
                 field.font = Font(
```

### Comparing `PDFFiller-0.2.3/PDFFiller/helpers/load_theme.py` & `pdffiller-0.2.4/PDFFiller/helpers/load_theme.py`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PDFFiller/theme/theme.py` & `pdffiller-0.2.4/PDFFiller/theme/theme.py`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PDFFiller.egg-info/PKG-INFO` & `pdffiller-0.2.4/PDFFiller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDFFiller
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple library to fill PDF documents
 Home-page: https://github.com/Moussawi7/pdf-filler
 Author: Ali Moussawi
 Author-email: moussawidev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PDFFiller-0.2.3/PDFFiller.egg-info/SOURCES.txt` & `pdffiller-0.2.4/PDFFiller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/PKG-INFO` & `pdffiller-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDFFiller
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple library to fill PDF documents
 Home-page: https://github.com/Moussawi7/pdf-filler
 Author: Ali Moussawi
 Author-email: moussawidev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PDFFiller-0.2.3/README.md` & `pdffiller-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `PDFFiller-0.2.3/setup.py` & `pdffiller-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = [
     'PyMuPDF>=1.23.7'
 ]
 
 setup(
     name='PDFFiller',
     packages=find_packages(exclude=['examples']),
-    version='0.2.3',
+    version='0.2.4',
     install_requires=install_requires,
     description='Simple library to fill PDF documents',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Ali Moussawi',
     author_email="moussawidev@gmail.com",
     classifiers=[
```

