# Comparing `tmp/ipywidgets-8.1.2.tar.gz` & `tmp/ipywidgets-8.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipywidgets-8.1.2.tar", last modified: Thu Feb  8 15:31:05 2024, max compression
+gzip compressed data, was "ipywidgets-8.1.3.tar", last modified: Tue May 28 09:32:06 2024, max compression
```

## Comparing `ipywidgets-8.1.2.tar` & `ipywidgets-8.1.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2024-02-08 15:31:05.314294 ipywidgets-8.1.2/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     1513 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/LICENSE
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      459 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/MANIFEST.in
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2347 2024-02-08 15:31:05.314198 ipywidgets-8.1.2/PKG-INFO
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      880 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/README.md
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2024-02-08 15:31:05.301898 ipywidgets-8.1.2/ipywidgets/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     1728 2024-02-08 14:25:01.000000 ipywidgets-8.1.2/ipywidgets/__init__.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      610 2024-02-08 15:30:16.000000 ipywidgets-8.1.2/ipywidgets/_version.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      764 2024-02-08 14:25:01.000000 ipywidgets-8.1.2/ipywidgets/comm.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    11287 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/embed.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2883 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/state.schema.json
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2024-02-08 15:31:05.303001 ipywidgets-8.1.2/ipywidgets/tests/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)        0 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/tests/__init__.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     6729 2024-02-08 14:25:01.000000 ipywidgets-8.1.2/ipywidgets/tests/test_embed.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      595 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/view.schema.json
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2024-02-08 15:31:05.307502 ipywidgets-8.1.2/ipywidgets/widgets/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     1709 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/__init__.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      639 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/docutils.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2290 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/domwidget.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    20414 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/interaction.py
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2024-02-08 15:31:05.312550 ipywidgets-8.1.2/ipywidgets/widgets/tests/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)        0 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/__init__.py
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2024-02-08 15:31:05.312963 ipywidgets-8.1.2/ipywidgets/widgets/tests/data/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    36297 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/data/jupyter-logo-transparent.png
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2111 2024-02-08 14:25:01.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_datetime_serializers.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      673 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_docutils.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    17123 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_interaction.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     1005 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_link.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     5619 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_selectioncontainer.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      732 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_send_state.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    11017 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_set_state.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     8361 2024-02-08 14:25:01.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_traits.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2478 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_utils.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2811 2024-02-08 14:25:01.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      995 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_box.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      369 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_button.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     4147 2024-02-08 14:25:01.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_datetime.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      606 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_float.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     4422 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_image.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2633 2024-02-08 14:25:01.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_naive_datetime.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     7466 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_output.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     3372 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_selection.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     1796 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_string.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    28435 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_templates.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2447 2024-02-08 14:25:01.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_time.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     4164 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_upload.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2407 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/tests/utils.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    16270 2024-02-08 14:25:01.000000 ipywidgets-8.1.2/ipywidgets/widgets/trait_types.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2608 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/utils.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      817 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/valuewidget.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    35131 2024-02-08 14:25:01.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     4328 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_bool.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     3731 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_box.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     4204 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_button.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      807 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_color.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2320 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_controller.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      622 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_core.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2597 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_date.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     4134 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_datetime.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2278 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_description.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    15028 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_float.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    12125 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_int.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     7067 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_layout.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     3708 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_link.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     7783 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_media.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     6823 2023-03-28 15:07:35.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_output.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    24457 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_selection.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     4198 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_selectioncontainer.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     6869 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_string.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      559 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_style.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     3498 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_tagsinput.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    15507 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_templates.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2779 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_time.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     4637 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/ipywidgets/widgets/widget_upload.py
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2024-02-08 15:31:05.313399 ipywidgets-8.1.2/ipywidgets.egg-info/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2347 2024-02-08 15:31:05.000000 ipywidgets-8.1.2/ipywidgets.egg-info/PKG-INFO
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2700 2024-02-08 15:31:05.000000 ipywidgets-8.1.2/ipywidgets.egg-info/SOURCES.txt
--rw-r--r--   0 maartenbreddels   (501) staff       (20)        1 2024-02-08 15:31:05.000000 ipywidgets-8.1.2/ipywidgets.egg-info/dependency_links.txt
--rw-r--r--   0 maartenbreddels   (501) staff       (20)        1 2024-02-08 15:31:05.000000 ipywidgets-8.1.2/ipywidgets.egg-info/not-zip-safe
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      157 2024-02-08 15:31:05.000000 ipywidgets-8.1.2/ipywidgets.egg-info/requires.txt
--rw-r--r--   0 maartenbreddels   (501) staff       (20)       11 2024-02-08 15:31:05.000000 ipywidgets-8.1.2/ipywidgets.egg-info/top_level.txt
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      229 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/pyproject.toml
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     1429 2024-02-08 15:31:05.314678 ipywidgets-8.1.2/setup.cfg
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      235 2023-03-28 15:07:31.000000 ipywidgets-8.1.2/setup.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-28 09:32:06.282020 ipywidgets-8.1.3/
+-rw-r--r--   0 martin    (1000) martin    (1000)     1513 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/LICENSE
+-rw-r--r--   0 martin    (1000) martin    (1000)      459 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)     2347 2024-05-28 09:32:06.282020 ipywidgets-8.1.3/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      880 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/README.md
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-28 09:32:06.278020 ipywidgets-8.1.3/ipywidgets/
+-rw-r--r--   0 martin    (1000) martin    (1000)     1728 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      610 2024-05-28 09:31:27.000000 ipywidgets-8.1.3/ipywidgets/_version.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      764 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/comm.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    11287 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/embed.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2883 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/state.schema.json
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-28 09:32:06.279020 ipywidgets-8.1.3/ipywidgets/tests/
+-rw-r--r--   0 martin    (1000) martin    (1000)        0 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/tests/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     6729 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/tests/test_embed.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      595 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/view.schema.json
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-28 09:32:06.280020 ipywidgets-8.1.3/ipywidgets/widgets/
+-rw-r--r--   0 martin    (1000) martin    (1000)     1709 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      639 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/docutils.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2290 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/domwidget.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    20414 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/interaction.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-28 09:32:06.281020 ipywidgets-8.1.3/ipywidgets/widgets/tests/
+-rw-r--r--   0 martin    (1000) martin    (1000)        0 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/__init__.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-28 09:32:06.281020 ipywidgets-8.1.3/ipywidgets/widgets/tests/data/
+-rw-r--r--   0 martin    (1000) martin    (1000)    36297 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/data/jupyter-logo-transparent.png
+-rw-r--r--   0 martin    (1000) martin    (1000)     2111 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_datetime_serializers.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      673 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_docutils.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    17123 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_interaction.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1005 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_link.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     5619 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_selectioncontainer.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      732 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_send_state.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    11017 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_set_state.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     8361 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_traits.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2478 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_utils.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2811 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      995 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_box.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      369 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_button.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     4147 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_datetime.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      606 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_float.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     4422 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_image.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2633 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_naive_datetime.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     7466 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_output.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     3372 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_selection.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1796 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_string.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    28435 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_templates.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2447 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_time.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     4164 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_upload.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2407 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/tests/utils.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    16270 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/trait_types.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2608 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/utils.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      817 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/valuewidget.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    35131 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     4328 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_bool.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     3731 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_box.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     4204 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_button.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      807 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_color.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2320 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_controller.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      622 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_core.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2597 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_date.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     4134 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_datetime.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2278 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_description.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    15028 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_float.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    12125 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_int.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     7067 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_layout.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     3708 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_link.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     7783 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_media.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     6823 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_output.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    24457 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_selection.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     4198 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_selectioncontainer.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     6869 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_string.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      559 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_style.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     3498 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_tagsinput.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    15507 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_templates.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     2779 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_time.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     4637 2024-05-23 10:50:20.000000 ipywidgets-8.1.3/ipywidgets/widgets/widget_upload.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-28 09:32:06.281020 ipywidgets-8.1.3/ipywidgets.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     2347 2024-05-28 09:32:06.000000 ipywidgets-8.1.3/ipywidgets.egg-info/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)     2700 2024-05-28 09:32:06.000000 ipywidgets-8.1.3/ipywidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        1 2024-05-28 09:32:06.000000 ipywidgets-8.1.3/ipywidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        1 2024-05-28 09:32:06.000000 ipywidgets-8.1.3/ipywidgets.egg-info/not-zip-safe
+-rw-r--r--   0 martin    (1000) martin    (1000)      157 2024-05-28 09:32:06.000000 ipywidgets-8.1.3/ipywidgets.egg-info/requires.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       11 2024-05-28 09:32:06.000000 ipywidgets-8.1.3/ipywidgets.egg-info/top_level.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)      229 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/pyproject.toml
+-rw-r--r--   0 martin    (1000) martin    (1000)     1429 2024-05-28 09:32:06.282020 ipywidgets-8.1.3/setup.cfg
+-rw-r--r--   0 martin    (1000) martin    (1000)      235 2024-01-31 13:17:14.000000 ipywidgets-8.1.3/setup.py
```

### Comparing `ipywidgets-8.1.2/LICENSE` & `ipywidgets-8.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/PKG-INFO` & `ipywidgets-8.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets
-Version: 8.1.2
+Version: 8.1.3
 Summary: Jupyter interactive widgets
 Home-page: http://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD 3-Clause License
 Keywords: Interactive,Interpreter,Shell,Web,ipython,widgets,Jupyter
 Platform: Linux
@@ -25,16 +25,16 @@
 Classifier: Framework :: Jupyter
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: comm>=0.1.3
 Requires-Dist: ipython>=6.1.0
 Requires-Dist: traitlets>=4.3.1
-Requires-Dist: widgetsnbextension~=4.0.10
-Requires-Dist: jupyterlab_widgets~=3.0.10
+Requires-Dist: widgetsnbextension~=4.0.11
+Requires-Dist: jupyterlab_widgets~=3.0.11
 Provides-Extra: test
 Requires-Dist: jsonschema; extra == "test"
 Requires-Dist: ipykernel; extra == "test"
 Requires-Dist: pytest>=3.6.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytz; extra == "test"
```

### Comparing `ipywidgets-8.1.2/README.md` & `ipywidgets-8.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/__init__.py` & `ipywidgets-8.1.3/ipywidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/_version.py` & `ipywidgets-8.1.3/ipywidgets/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
-__version__ = '8.1.2'
+__version__ = '8.1.3'
 
 __protocol_version__ = '2.1.0'
 __control_protocol_version__ = '1.0.0'
 
 # These are *protocol* versions for each package, *not* npm versions. To check, look at each package's src/version.ts file for the protocol version the package implements.
 __jupyter_widgets_base_version__ = '2.0.0'
 __jupyter_widgets_output_version__ = '1.0.0'
```

### Comparing `ipywidgets-8.1.2/ipywidgets/comm.py` & `ipywidgets-8.1.3/ipywidgets/comm.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/embed.py` & `ipywidgets-8.1.3/ipywidgets/embed.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/state.schema.json` & `ipywidgets-8.1.3/ipywidgets/state.schema.json`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/tests/test_embed.py` & `ipywidgets-8.1.3/ipywidgets/tests/test_embed.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/view.schema.json` & `ipywidgets-8.1.3/ipywidgets/view.schema.json`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/__init__.py` & `ipywidgets-8.1.3/ipywidgets/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/docutils.py` & `ipywidgets-8.1.3/ipywidgets/widgets/docutils.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/domwidget.py` & `ipywidgets-8.1.3/ipywidgets/widgets/domwidget.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/interaction.py` & `ipywidgets-8.1.3/ipywidgets/widgets/interaction.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/data/jupyter-logo-transparent.png` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/data/jupyter-logo-transparent.png`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_datetime_serializers.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_datetime_serializers.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_docutils.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_docutils.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_interaction.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_interaction.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_link.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_selectioncontainer.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_selectioncontainer.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_send_state.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_send_state.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_set_state.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_set_state.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_traits.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_traits.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_utils.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_box.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_box.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_datetime.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_datetime.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_float.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_float.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_image.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_image.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_naive_datetime.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_naive_datetime.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_output.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_output.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_selection.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_selection.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_string.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_string.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_templates.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_templates.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_time.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_time.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/test_widget_upload.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/test_widget_upload.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/tests/utils.py` & `ipywidgets-8.1.3/ipywidgets/widgets/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/trait_types.py` & `ipywidgets-8.1.3/ipywidgets/widgets/trait_types.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/utils.py` & `ipywidgets-8.1.3/ipywidgets/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/valuewidget.py` & `ipywidgets-8.1.3/ipywidgets/widgets/valuewidget.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_bool.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_bool.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_box.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_box.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_button.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_button.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_color.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_color.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_controller.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_controller.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_core.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_core.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_date.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_date.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_datetime.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_datetime.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_description.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_description.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_float.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_float.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_int.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_int.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_layout.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_layout.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_link.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_link.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_media.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_media.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_output.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_output.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_selection.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_selection.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_selectioncontainer.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_selectioncontainer.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_string.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_string.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_style.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_style.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_tagsinput.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_tagsinput.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_templates.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_templates.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_time.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_time.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets/widgets/widget_upload.py` & `ipywidgets-8.1.3/ipywidgets/widgets/widget_upload.py`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/ipywidgets.egg-info/PKG-INFO` & `ipywidgets-8.1.3/ipywidgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets
-Version: 8.1.2
+Version: 8.1.3
 Summary: Jupyter interactive widgets
 Home-page: http://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD 3-Clause License
 Keywords: Interactive,Interpreter,Shell,Web,ipython,widgets,Jupyter
 Platform: Linux
@@ -25,16 +25,16 @@
 Classifier: Framework :: Jupyter
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: comm>=0.1.3
 Requires-Dist: ipython>=6.1.0
 Requires-Dist: traitlets>=4.3.1
-Requires-Dist: widgetsnbextension~=4.0.10
-Requires-Dist: jupyterlab_widgets~=3.0.10
+Requires-Dist: widgetsnbextension~=4.0.11
+Requires-Dist: jupyterlab_widgets~=3.0.11
 Provides-Extra: test
 Requires-Dist: jsonschema; extra == "test"
 Requires-Dist: ipykernel; extra == "test"
 Requires-Dist: pytest>=3.6.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytz; extra == "test"
```

### Comparing `ipywidgets-8.1.2/ipywidgets.egg-info/SOURCES.txt` & `ipywidgets-8.1.3/ipywidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipywidgets-8.1.2/setup.cfg` & `ipywidgets-8.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 python_requires = >=3.7
 zip_safe = False
 packages = find:
 install_requires = 
 	comm>=0.1.3
 	ipython>=6.1.0
 	traitlets>=4.3.1
-	widgetsnbextension~=4.0.10
-	jupyterlab_widgets~=3.0.10
+	widgetsnbextension~=4.0.11
+	jupyterlab_widgets~=3.0.11
 
 [options.extras_require]
 test = 
 	jsonschema
 	ipykernel
 	pytest>=3.6.0
 	pytest-cov
```

