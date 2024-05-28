# Comparing `tmp/flet-box-gui-0.1.2.tar.gz` & `tmp/flet-box-gui-0.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-box-gui-0.1.2.tar", last modified: Tue May 28 03:07:38 2024, max compression
+gzip compressed data, was "flet-box-gui-0.1.2.1.tar", last modified: Tue May 28 14:44:11 2024, max compression
```

## Comparing `flet-box-gui-0.1.2.tar` & `flet-box-gui-0.1.2.1.tar`

### file list

```diff
@@ -1,95 +1,97 @@
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.212126 flet-box-gui-0.1.2/
--rw-r--r--   0 mjay      (1000) mjay      (1000)       59 2024-05-26 13:58:32.000000 flet-box-gui-0.1.2/MANIFEST.in
--rw-r--r--   0 mjay      (1000) mjay      (1000)    18379 2024-05-28 03:07:38.212126 flet-box-gui-0.1.2/PKG-INFO
--rw-r--r--   0 mjay      (1000) mjay      (1000)    14507 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2/README.md
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.176126 flet-box-gui-0.1.2/flet_box/
--rw-r--r--   0 mjay      (1000) mjay      (1000)       29 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/__init__.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.196126 flet-box-gui-0.1.2/flet_box/assets/
--rw-r--r--   0 mjay      (1000) mjay      (1000)    13575 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/assets/avatar.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)    22379 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/assets/avatar.png
--rw-r--r--   0 mjay      (1000) mjay      (1000)    97142 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/assets/dragg_container.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)    51971 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/assets/dragg_container3.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)   195620 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/assets/image.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)   141033 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/assets/img.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)    82936 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/assets/logo.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)   135590 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/assets/logo_mark.png
--rw-r--r--   0 mjay      (1000) mjay      (1000)   226793 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/assets/my_avatar.png
--rw-r--r--   0 mjay      (1000) mjay      (1000)    11864 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/assets/no_imagen.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)   204659 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/assets/splash.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)    27549 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/assets/wallpaper.jpg
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.196126 flet-box-gui-0.1.2/flet_box/extra_utils/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/__init__.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.196126 flet-box-gui-0.1.2/flet_box/extra_utils/about/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/about/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    18687 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/about/about.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.196126 flet-box-gui-0.1.2/flet_box/extra_utils/alert/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/alert/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     1711 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/alert/alert_selected.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.200126 flet-box-gui-0.1.2/flet_box/extra_utils/chat_gpt_browser/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/chat_gpt_browser/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    14328 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/chat_gpt_browser/gpt_browser.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     6033 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/chat_gpt_browser/library_chatgpt.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.200126 flet-box-gui-0.1.2/flet_box/extra_utils/color_browser/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/color_browser/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    11954 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2/flet_box/extra_utils/color_browser/color_browser.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.200126 flet-box-gui-0.1.2/flet_box/extra_utils/config_container/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/config_container/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    16681 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2/flet_box/extra_utils/config_container/blur_color_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    11564 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/config_container/bool_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    13019 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2/flet_box/extra_utils/config_container/color_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    12624 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/config_container/double_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    16368 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/config_container/four_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    30959 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2/flet_box/extra_utils/config_container/gradient_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    18393 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/config_container/selection_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    13712 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/config_container/single_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    41661 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2/flet_box/extra_utils/config_container/widget_editor.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.204126 flet-box-gui-0.1.2/flet_box/extra_utils/drag_container/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/drag_container/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     8947 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/drag_container/dragg_widget.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    27864 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/drag_container/infinity_box_layer_one.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    25298 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/drag_container/widget_drag_editor.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.204126 flet-box-gui-0.1.2/flet_box/extra_utils/icon_browser/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/icon_browser/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    11552 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/icon_browser/icon_browser.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.204126 flet-box-gui-0.1.2/flet_box/extra_utils/lite_menu_bar_down_phone/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/lite_menu_bar_down_phone/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     8164 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/lite_menu_bar_down_phone/footer_bar_menu_phone.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     2374 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/lite_menu_bar_down_phone/selected_widget.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.204126 flet-box-gui-0.1.2/flet_box/extra_utils/lite_menu_bar_right_phone/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/lite_menu_bar_right_phone/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    22984 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/lite_menu_bar_right_phone/right_bar_menu_phone.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.204126 flet-box-gui-0.1.2/flet_box/extra_utils/menu_tab_left_phone/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/menu_tab_left_phone/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    11184 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/menu_tab_left_phone/widget_menu_left_editor.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.204126 flet-box-gui-0.1.2/flet_box/extra_utils/menu_tab_up_phone/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/menu_tab_up_phone/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     7973 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/menu_tab_up_phone/basic_menu_tab_up.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     1762 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/menu_tab_up_phone/skeleton_class_screens.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    19563 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/menu_tab_up_phone/widget_menu_tab_editor.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.204126 flet-box-gui-0.1.2/flet_box/extra_utils/phone_container/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/phone_container/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     7335 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2/flet_box/extra_utils/phone_container/widget_phone_editor.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.208126 flet-box-gui-0.1.2/flet_box/extra_utils/screen_manager/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/screen_manager/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    30641 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2/flet_box/extra_utils/screen_manager/screen_manager.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     2336 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/screen_manager/settings_screens.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)      636 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/screen_manager/write_file_proyect.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.208126 flet-box-gui-0.1.2/flet_box/extra_utils/settings_var/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/settings_var/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    53915 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2/flet_box/extra_utils/settings_var/save_export.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     3986 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2/flet_box/extra_utils/settings_var/settings_widget.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.208126 flet-box-gui-0.1.2/flet_box/extra_utils/tree_view/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/tree_view/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    10218 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/tree_view/color_hight_light_editor.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     3305 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/tree_view/tree_view.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    17067 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2/flet_box/extra_utils/tree_view/tree_view_text_editor.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    15513 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2/flet_box/flet_box.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 03:07:38.208126 flet-box-gui-0.1.2/flet_box_gui.egg-info/
--rw-r--r--   0 mjay      (1000) mjay      (1000)    18379 2024-05-28 03:07:37.000000 flet-box-gui-0.1.2/flet_box_gui.egg-info/PKG-INFO
--rw-r--r--   0 mjay      (1000) mjay      (1000)     3308 2024-05-28 03:07:38.000000 flet-box-gui-0.1.2/flet_box_gui.egg-info/SOURCES.txt
--rw-r--r--   0 mjay      (1000) mjay      (1000)        1 2024-05-28 03:07:37.000000 flet-box-gui-0.1.2/flet_box_gui.egg-info/dependency_links.txt
--rw-r--r--   0 mjay      (1000) mjay      (1000)       47 2024-05-28 03:07:37.000000 flet-box-gui-0.1.2/flet_box_gui.egg-info/entry_points.txt
--rw-r--r--   0 mjay      (1000) mjay      (1000)       42 2024-05-28 03:07:37.000000 flet-box-gui-0.1.2/flet_box_gui.egg-info/requires.txt
--rw-r--r--   0 mjay      (1000) mjay      (1000)        9 2024-05-28 03:07:37.000000 flet-box-gui-0.1.2/flet_box_gui.egg-info/top_level.txt
--rw-r--r--   0 mjay      (1000) mjay      (1000)       38 2024-05-28 03:07:38.212126 flet-box-gui-0.1.2/setup.cfg
--rw-r--r--   0 mjay      (1000) mjay      (1000)     4462 2024-05-28 03:06:37.000000 flet-box-gui-0.1.2/setup.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.601719 flet-box-gui-0.1.2.1/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     3189 2024-05-28 14:43:54.000000 flet-box-gui-0.1.2.1/CHANGELOG.md
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11340 2024-03-27 02:45:35.000000 flet-box-gui-0.1.2.1/LICENSE
+-rw-r--r--   0 mjay      (1000) mjay      (1000)       81 2024-05-28 03:22:40.000000 flet-box-gui-0.1.2.1/MANIFEST.in
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    23643 2024-05-28 14:44:11.601719 flet-box-gui-0.1.2.1/PKG-INFO
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    14602 2024-05-28 14:10:23.000000 flet-box-gui-0.1.2.1/README.md
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.577719 flet-box-gui-0.1.2.1/flet_box/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)       29 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/__init__.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.585719 flet-box-gui-0.1.2.1/flet_box/assets/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    13575 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/avatar.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    22379 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/avatar.png
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    97142 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/dragg_container.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    51971 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/dragg_container3.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)   195620 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/image.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)   141033 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/img.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    82936 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/logo.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)   135590 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/logo_mark.png
+-rw-r--r--   0 mjay      (1000) mjay      (1000)   226793 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/my_avatar.png
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11864 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/no_imagen.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)   204659 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/splash.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    27549 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/wallpaper.jpg
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.585719 flet-box-gui-0.1.2.1/flet_box/extra_utils/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/__init__.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.585719 flet-box-gui-0.1.2.1/flet_box/extra_utils/about/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/about/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    18687 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/about/about.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.585719 flet-box-gui-0.1.2.1/flet_box/extra_utils/alert/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/alert/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     1711 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/alert/alert_selected.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.585719 flet-box-gui-0.1.2.1/flet_box/extra_utils/chat_gpt_browser/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/chat_gpt_browser/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    14328 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/chat_gpt_browser/gpt_browser.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     6033 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/chat_gpt_browser/library_chatgpt.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.585719 flet-box-gui-0.1.2.1/flet_box/extra_utils/color_browser/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/color_browser/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11954 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/color_browser/color_browser.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.589719 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    16681 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/blur_color_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11564 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/bool_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    13019 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/color_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    12624 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/double_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    16368 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/four_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    30959 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/gradient_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    18393 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/selection_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    13712 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/single_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    41661 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/widget_editor.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.589719 flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     8947 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/dragg_widget.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    27864 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/infinity_box_layer_one.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    25298 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/widget_drag_editor.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.589719 flet-box-gui-0.1.2.1/flet_box/extra_utils/icon_browser/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/icon_browser/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11552 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/icon_browser/icon_browser.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.593719 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_down_phone/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_down_phone/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     8164 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_down_phone/footer_bar_menu_phone.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     2374 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_down_phone/selected_widget.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.593719 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_right_phone/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_right_phone/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    22984 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_right_phone/right_bar_menu_phone.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.593719 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_left_phone/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_left_phone/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11184 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_left_phone/widget_menu_left_editor.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.593719 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     7973 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/basic_menu_tab_up.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     1762 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/skeleton_class_screens.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    19563 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/widget_menu_tab_editor.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.593719 flet-box-gui-0.1.2.1/flet_box/extra_utils/phone_container/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/phone_container/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     7335 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/phone_container/widget_phone_editor.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.597719 flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    30641 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/screen_manager.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     2336 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/settings_screens.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)      636 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/write_file_proyect.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.597719 flet-box-gui-0.1.2.1/flet_box/extra_utils/settings_var/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/settings_var/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    53915 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/settings_var/save_export.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     3986 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/settings_var/settings_widget.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.597719 flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    10218 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/color_hight_light_editor.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     3305 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/tree_view.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    17067 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/tree_view_text_editor.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    15513 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2.1/flet_box/flet_box.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.601719 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    23643 2024-05-28 14:44:11.000000 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/PKG-INFO
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     3329 2024-05-28 14:44:11.000000 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        1 2024-05-28 14:44:11.000000 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 mjay      (1000) mjay      (1000)       47 2024-05-28 14:44:11.000000 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/entry_points.txt
+-rw-r--r--   0 mjay      (1000) mjay      (1000)       42 2024-05-28 14:44:11.000000 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/requires.txt
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        9 2024-05-28 14:44:11.000000 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/top_level.txt
+-rw-r--r--   0 mjay      (1000) mjay      (1000)       38 2024-05-28 14:44:11.601719 flet-box-gui-0.1.2.1/setup.cfg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     4780 2024-05-28 14:41:09.000000 flet-box-gui-0.1.2.1/setup.py
```

### Comparing `flet-box-gui-0.1.2/PKG-INFO` & `flet-box-gui-0.1.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,341 +1,312 @@
-Metadata-Version: 2.1
-Name: flet-box-gui
-Version: 0.1.2
-Summary: flet-box-gui it's a GUI Dragg and drop BUILDER.
-Home-page: https://github.com/xavier53348/Flet-Box
-Author: xavier53348
-Author-email: xavier53348@gmail.com
-Maintainer: xavier53348
-Maintainer-email: xavier53348@gmail.com
-License: UNKNOWN
-Project-URL: Documentation, https://github.com/xavier53348/Flet-Box/blob/main/docs/WIDGET.md
-Project-URL: GitHub, https://github.com/xavier53348/Flet-Box
-Project-URL: Changelog, https://github.com/xavier53348/Flet-Box/blob/main/docs/CHANGELOG.md
-Project-URL: Roadmap, https://github.com/xavier53348/Flet-Box/blob/main/docs/Roadmap.md
-Description: <!-- <img src="docs/gallery/full_screen.png" alt="Imagen Flet-Box"> -->
-        <!-- markdownserver http://localhost:8009/README.md -->
-        <!-- http://localhost:8080/Desktop/git_hub/flet_box/docs/Roadmap#flet-box-framework-roadmap -->
-        
-        
-        ## Flet-Box:
-        ### It's a Python GUI Framework for Multi-Platform Apps
-        
-        [![Gallery Preview FLET-BOX](docs/gallery/youtube.png)](https://www.youtube.com/watch?v=15DDAACb0Hw)
-        
-        <details>
-            <summary>Gallery Preview FLET-BOX</summary>
-            <img src="docs/gallery/full_screen.png"         alt="Imagen Flet-Box">
-            <img src="docs/gallery/icons.png"               alt="Icons Flet-Box">
-            <img src="docs/gallery/colors.png"              alt="Colors Flet-Box">
-            <img src="docs/gallery/pc_mode.png"             alt="Colors Flet-Box">
-            <img src="docs/gallery/pc_mode_config.png"      alt="Colors Flet-Box">
-        </details>
-        
-        
-        [More info documentation](https://github.com/xavier53348/Flet-Box/blob/main/docs/WIDGET.md)
-        
-        [Our goals and Roadmap](https://github.com/xavier53348/Flet-Box/blob/main/docs/Roadmap.md)
-        
-        **Certainly!** Let's create a documentation for **Flet-Box**, a GUI framework that simplifies building multi-platform apps using drag-and-drop widgets in the Python language.
-        
-        ## Instalation Flet-Box
-        ```bash
-        
-        >>> mkdir My_app
-        >>> cd My_app
-        
-        ```
-        ## Run one time
-        ```bash
-        
-        >>> python3 -m venv .venv
-        
-        ```
-        ## Activate virtual env
-        ```bash
-        
-        >>> source .venv/bin/activate
-        >>> pip install flet
-        >>> pip install -r requirements.txt
-        
-        ```
-        ## Install manually
-        
-        ```
-        >>> git clone https://github.com/xavier53348/Flet-Box.git
-        
-        ```
-        ## By pypi repo
-        
-        ```
-        >>> pip install flet-box-gui
-        
-        ```
-        ## Easy run Flet-Box
-        ```bash
-        
-        >>> flet flet_box/flet_box.py
-        
-        ```
-        ## Easy way run a save APP
-        
-        ```
-        >>> flet test/proyect_name/proyect_name/main.py
-        
-        ```
-        ### Introduction
-        **Flet-Box** is a powerful framework that enables developers to create interactive multi-user web, desktop, and mobile applications. Whether you're a seasoned developer or just starting out, **Flet-Box** makes frontend development accessible without prior experience. Here are the key features:
-        
-        1. **Cross-Platform**: Build apps that run seamlessly on web browsers, desktop environments (like macOS and Windows), and mobile devices.
-        
-        2. **Drag-and-Drop Widgets**: Easily design your app's user interface by dragging and dropping widgets.
-        
-        3. **Based on Flutter**: **Flet-Box** is a fork of **Flet Framework** leverages the power of Flutter by Google, but it doesn't stop there. It adds its own opinion by combining smaller widgets, implementing UI best practices, and applying reasonable defaults to ensure your apps look professional without extra effort.
-        
-        ### Getting Started with Flet-Box in Python
-        To get started, you don't need to be a front-end guru, but basic knowledge of Python and object-oriented programming is recommended. Let's dive into the basics:
-        
-        ### Learn More
-        Ready to build real-world apps? Check out the [official Flet documentation](https://flet.dev/docs/) and explore tutorials for your preferred language, including Python3. Happy coding! 🚀
-        
-        ### Widgets aviables with Flet-Box Now on building
-        
-        Certainly! In **Flet-Box**, you can create drag-and-drop interactions using the **LongPressDraggable** widget. Let's break down how to achieve this:
-        
-        1. **LongPressDraggable**: This widget recognizes when a user performs a long press (sometimes called touch & hold) on a widget. It then displays a new widget near the user's finger. As the user drags, the widget follows their finger. You have full control over the widget that the user drags.
-        
-        - Wrap your UI element (widget) with a **LongPressDraggable**. For example, if you have a list of menu items, each displayed using a custom **MenuListItem** widget, you can wrap it like this:
-        
-        ## Widgets will be Updating ...
-        #### You mey use now the currents widgets that are marked
-        
-        | **SPACE LAYOUTS**        |   | **IMAGE WIDGET**         |   | **ALERTS STATUS**        |   |
-        |--------------------------|---|--------------------------|---|--------------------------|---|
-        | ft.divider               | ✔ | ft.image                 | ✔ | ft.snackbar              | ✘ |
-        | ft.verticaldivider       | + | ft.circleavatar          | + | ft.tooltip               | ✔ |
-        |                          |   | ft.icon                  | ✔ | ft.cupertinoalertdialog  | ✘ |
-        |                          |   |                          |   | ft.cupertinodialogaction | ✘ |
-        |                          |   |                          |   |                          |   |
-        | **CONTAINERS LAYOUTS**   |   | **CHARTS LAYOUTS**       |   | **TEXT WIDGET**          |   |
-        | ft.stack                 | ✔ | ft.barchart              | ✘ | ft.text                  | ✔ |
-        | ft.row                   | ✔ | ft.charts                | ✘ | ft.textfield             | ✔ |
-        | ft.gridview              | ✔ | ft.linechart             | ✘ | ft.listview              | ✘ |
-        | ft.column                | ✔ | ft.matplotlibchart       | ✘ | ft.datatable             | ✘ |
-        | ft.container             | ✔ | ft.piechart              | ✘ |                          |   |
-        | ft.card                  | ✘ | ft.plotlychart           | ✘ |                          |   |
-        | ft.responsiverow         | ✘ |                          |   |                          |   |
-        | ft.transparentpointer    | ✘ |                          |   |                          |   |
-        |                          |   |                          |   |                          |   |
-        | **BUTTONS WIDGET**       |   | **SELECTIONS WIDGET**    |   | **ESPECIAL WIDGET**      |   |
-        | ft.textbutton            | ✔ | ft.switch                | ✘ | ft.tabs                  | ✘ |
-        | ft.filledbutton          | ✔ | ft.checkbox              | ✔ | ft.navigationbar         | ✘ |
-        | ft.filledtonalbutton     | ✔ | ft.cupertinocheckbox     | ✔ | ft.cupertinoappbar       | ✘ |
-        | ft.iconbutton            | ✔ | ft.cupertinoradio        | ✔ | ft.navigationdrawer      | ✘ |
-        | ft.elevatedbutton        | ✔ | ft.cupertinoslider       | ✔ | ft.navigationrail        | ✘ |
-        | ft.chip                  | ✔ | ft.cupertinoswitch       | ✔ | ft.menubar               | ✘ |
-        | ft.outlinedbutton        | ✔ | ft.submenubutton         | ✘ | ft.appbar                | ✘ |
-        | ft.bottomappbar          | ✘ | ft.dropdown              | ✘ | ft.cupertinonavigationbar| ✘ |
-        | ft.bottomsheet           | ✘ | ft.datepicker            | ✘ | ft.searchbar             | ✘ |
-        | ft.segmentedbutton       | ✘ | ft.timepicker            | ✘ |
-        | ft.floatingactionbutton  | ✘ | ft.filepicker            | ✘ |
-        |                          |   | ft.radio                 | ✘ |
-        | **WIDGETS STATUS**       |   |
-        | ft.slider                | ✘ |
-        | ft.progressbar           | ✘ |
-        | ft.progressring          | ✘ |
-        | ft.alertdialog           | ✘ |
-        | ft.rangeslider           | ✘ |
-        
-        <!-- make tree -->
-         <!-- tree -I '__pycache__|__init__.py|test|drag_drop_proyect|flet_box.egg-info|docs|.|build|dist|LICENSE|MANIFEST.in|requeriments.txt|README.md|pyproject.toml|setup.py' > full_path.txt -->
-        
-        ### Path Flet-Box Modules
-        ```bash
-        .
-        ├── full_path.txt
-        ├── src
-        │   ├── assets
-        │   │   ├── avatar.jpg
-        │   │   ├── avatar.png
-        │   │   ├── dragg_container3.jpg
-        │   │   ├── dragg_container.jpg
-        │   │   ├── image.jpg
-        │   │   ├── img.jpg
-        │   │   ├── iphone.png
-        │   │   ├── logo.jpg
-        │   │   ├── logo_mark.png
-        │   │   ├── my_avatar.png
-        │   │   ├── no_imagen.jpg
-        │   │   └── splash.jpg
-        │   ├── bump-version.sh
-        │   ├── CHANGELOG.md
-        │   ├── extra_utils
-        │   │   ├── about
-        │   │   │   └── about.py
-        │   │   ├── alert
-        │   │   │   └── alert_selected.py
-        │   │   ├── chat_gpt_browser
-        │   │   │   ├── gpt_browser.py
-        │   │   │   └── library_chatgpt.py
-        │   │   ├── color_browser
-        │   │   │   └── color_browser.py
-        │   │   ├── config_container
-        │   │   │   ├── bool_entry.py
-        │   │   │   ├── color_entry.py
-        │   │   │   ├── double_entry.py
-        │   │   │   ├── four_entry.py
-        │   │   │   ├── gradient_entry.py
-        │   │   │   ├── selection_entry.py
-        │   │   │   ├── single_entry.py
-        │   │   │   └── widget_editor.py
-        │   │   ├── drag_container
-        │   │   │   ├── dragg_widget.py
-        │   │   │   ├── drag_handler_container.py
-        │   │   │   ├── infinity_box_layer_one.py
-        │   │   │   └── widget_drag_editor.py
-        │   │   ├── icon_browser
-        │   │   │   └── icon_browser.py
-        │   │   ├── lite_menu_bar_down_phone
-        │   │   │   ├── footer_bar_menu_phone.py
-        │   │   │   └── selected_widget.py
-        │   │   ├── lite_menu_bar_up_phone
-        │   │   │   └── head_bar_menu_phone.py
-        │   │   ├── menu_tab_left_phone
-        │   │   │   └── widget_menu_left_editor.py
-        │   │   ├── menu_tab_up_phone
-        │   │   │   ├── basic_menu_tab_up.py
-        │   │   │   └── widget_menu_tab_editor.py
-        │   │   ├── phone_container
-        │   │   │   └── widget_phone_editor.py
-        │   │   ├── settings_var
-        │   │   │   ├── save_export.py
-        │   │   │   └── settings_widget.py
-        │   │   └── tree_view
-        │   │       ├── tree_view.py
-        │   │       └── tree_view_text_editor.py
-        │   ├── flet_box.py
-        │   ├── __main__.py
-        │   └── VERSION
-        └── workflows
-        
-        18 directories, 47 files
-        
-        ```
-        
-        ### Certainly!
-        
-        If you're passionate about shaping the future of frameworks and contributing to their development, I invite you to join our collaborative efforts. Here's how you can get involved:
-        
-        1. **Documentation and Modules**:
-        
-           - **Documentation**: We're actively working on creating comprehensive documentation for our Flet-Box framework. Your contributions can help make it more accessible, accurate, and user-friendly. Whether you're an expert or a beginner, your insights matter!
-        
-           - **Modules**: Our framework consists of various modules that handle different aspects of Flet activities. If you have expertise in any specific area (such as Documentation, Modules, or consensus algorithms ), consider contributing by improving existing modules or proposing new ones.
-        
-        2. **Financial Considerations**:
-        
-            - If you're passionate about supporting open-source projects and want to contribute to the **Flet-box Framework**, here's a simple invitation for you:
-        
-            **You may contribute Donating tokens to give suppor to the proyect in  MATIC , BINANCE or TRX Tokens**
-        
-            - **Low Fees**: In transactions have extremely low fees, making it ideal for micro-donations.
-            - Invite me a **COFFE** or a **BEER** ..
-        
-            **How to Donate Tokens:**
-            - **Get Token**: Purchase MATIC , BINANCE or TRX on platforms like Binance, Coinbase, or Uniswap.
-            - **Donate**: Visit the Flet-box page and contribute directly. **Every donation counts!**
-        
-            **MATIC WALLET**
-        
-        | **SPACE LAYOUTS**                                                                         |    **ADDRESS**                                            |
-        |-------------------------------------------------------------------------------------------|-----------------------------------------------------------|
-        | <img src="docs/assets/matics_wallet.jpeg" style="width:60px" align="Center">              | 0x6d437bB66af8d2c44670eA18F059BE1417Dcd7bA                |
-        | <img src="docs/assets/trx_wallet.jpeg" style="width:60px" align="Center">                 | THi2UTY8SrUYNrzqKek8U3pvLuEF5y4fDQ                        |
-        | <img src="docs/assets/bnb_wallet.jpeg" style="width:60px" align="Center">                 | bnb1vhe8q5zf2fr6s0ga8dnm5nzaz9uapky6w2xcnr                |
-        
-            - **Learn More**: Explore Flet-box's mission, roadmap, and community initiatives on their official website.
-        
-        3. **Collaboration and Feedback**:
-           - We value diverse perspectives. Engage in discussions, attend working groups, and provide feedback during public consultations.
-        
-        ###  How to Get Started:
-        
-        * Reach out to our team via the provided contact details if you have specific questions or want to contribute directly.
-        * Remember, every contribution counts! Let's build a robust and forward-looking framework that fosters innovation while safeguarding financial stability.
-        
-        ##  How contribute to build Widget dragg in flet-Box
-        
-        1.  Build left take dragg selection widgets.
-        
-        **Exemple:**
-        
-        ```python
-        
-        self.RowDragg  = DraggWidget( widget='Row' ,color='BLUE' ,icons= ft.icons.BURST_MODE_ROUNDED)
-        
-        ```
-            **Properties:**
-        
-                * widget <== 'Widget name'
-                * color  <== 'Color of the box Dragg'
-                * icons  <== 'icons of the box Dragg'
-        
-            * **we create a Object named self.RowDragg that we will add inside drag_container_to_phone object.**
-        
-            #### After we need add manual inside [ drag_container_to_phone ]
-        
-        2.  Exemple build left take dragg selection widgets inside drag_container_to_phone.
-        
-        ```python
-        
-        ft.Container(
-                content=ft.GridView(
-                                    runs_count=3,
-                                    run_spacing=8,
-                                    padding=4,
-                                    spacing=8,
-                                    expand=1,
-                                controls=[
-                                            self.RowDragg, # <============= add inside
-                                         ],
-        
-        ```
-        
-        3.  Go to infinity_box_layer_one.py and add Manually.
-        
-        **Location:**
-        
-        - ***'extra_utils/drag_container/infinity_box_layer_one.py'***
-        
-        - we need build the Container that will have the drop Widget inside
-        
-        **Exemple how will be**
-        
-        ```python
-        
-        "Row": [
-                    ft.Container(bgcolor='blue',alignment=ft.alignment.center,padding=ft.padding.all(4),border=ft.border.all(0.8, ft.colors.BLACK),tooltip='Row',
-                on_hover=lambda _:self.resetClick(),
-                on_click=lambda _:self.touchWidgetIndex(self.infinityDropWidget),
-                content=ft.Row( scroll="ALWAYS",
-                    controls= [
-                                   ],),),
-          ],
-        
-        ```
-        
-Keywords: flet-box-gui,flet,flet-gui,flet-builder,flet-sdk
-Platform: Multy platforms
-Classifier: Development Status :: 1 - Planning
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Description-Content-Type: text/markdown
+<!-- <img src="docs/gallery/full_screen.png" alt="Imagen Flet-Box"> -->
+<!-- markdownserver http://localhost:8009/README.md -->
+<!-- http://localhost:8080/Desktop/git_hub/flet_box/docs/Roadmap#flet-box-framework-roadmap -->
+
+
+## Flet-Box:
+### It's a Python GUI Framework for Multi-Platform Apps
+
+[![Gallery Preview FLET-BOX](docs/gallery/youtube.png)](https://www.youtube.com/watch?v=15DDAACb0Hw)
+
+<details>
+    <summary>Gallery Preview FLET-BOX</summary>
+    <img src="docs/gallery/full_screen.png"         alt="Imagen Flet-Box">
+    <img src="docs/gallery/icons.png"               alt="Icons Flet-Box">
+    <img src="docs/gallery/colors.png"              alt="Colors Flet-Box">
+    <img src="docs/gallery/pc_mode.png"             alt="Colors Flet-Box">
+    <img src="docs/gallery/pc_mode_config.png"      alt="Colors Flet-Box">
+</details>
+
+
+[More info documentation](https://github.com/xavier53348/Flet-Box/blob/main/docs/WIDGET.md)
+
+[Our goals and Roadmap](https://github.com/xavier53348/Flet-Box/blob/main/docs/Roadmap.md)
+
+**Certainly!** Let's create a documentation for **Flet-Box**, a GUI framework that simplifies building multi-platform apps using drag-and-drop widgets in the Python language.
+
+## Instalation Flet-Box
+```bash
+
+>>> mkdir My_app
+>>> cd My_app
+
+```
+## Run one time
+```bash
+
+>>> python3 -m venv .venv
+
+```
+## Activate virtual env
+```bash
+
+>>> source .venv/bin/activate
+>>> pip install flet
+>>> pip install -r requirements.txt
+
+```
+## Install manually
+
+```
+>>> git clone https://github.com/xavier53348/Flet-Box.git
+
+```
+## By pypi repo
+
+```
+>>> pip install flet-box-gui
+
+```
+## Easy run Flet-Box
+```bash
+
+>>> flet flet_box/flet_box.py
+
+```
+## Easy way run a save APP
+
+```
+>>> flet test/proyect_name/proyect_name/main.py
+
+```
+### Introduction
+**Flet-Box** is a powerful framework that enables developers to create interactive multi-user web, desktop, and mobile applications. Whether you're a seasoned developer or just starting out, **Flet-Box** makes frontend development accessible without prior experience. Here are the key features:
+
+1. **Cross-Platform**: Build apps that run seamlessly on web browsers, desktop environments (like macOS and Windows), and mobile devices.
+
+2. **Drag-and-Drop Widgets**: Easily design your app's user interface by dragging and dropping widgets.
+
+3. **Based on Flutter**: **Flet-Box** is a fork of **Flet Framework** leverages the power of Flutter by Google, but it doesn't stop there. It adds its own opinion by combining smaller widgets, implementing UI best practices, and applying reasonable defaults to ensure your apps look professional without extra effort.
+
+### Getting Started with Flet-Box in Python
+To get started, you don't need to be a front-end guru, but basic knowledge of Python and object-oriented programming is recommended. Let's dive into the basics:
+
+### Learn More
+Ready to build real-world apps? Check out the [official Flet documentation](https://flet.dev/docs/) and explore tutorials for your preferred language, including Python3. Happy coding! 🚀
+
+### Widgets aviables with Flet-Box Now on building
+
+Certainly! In **Flet-Box**, you can create drag-and-drop interactions using the **LongPressDraggable** widget. Let's break down how to achieve this:
+
+1. **LongPressDraggable**: This widget recognizes when a user performs a long press (sometimes called touch & hold) on a widget. It then displays a new widget near the user's finger. As the user drags, the widget follows their finger. You have full control over the widget that the user drags.
+
+- Wrap your UI element (widget) with a **LongPressDraggable**. For example, if you have a list of menu items, each displayed using a custom **MenuListItem** widget, you can wrap it like this:
+
+## Widgets will be Updating ...
+#### You mey use now the currents widgets that are marked
+
+| **SPACE LAYOUTS**        |   | **IMAGE WIDGET**         |   | **ALERTS STATUS**        |   |
+|--------------------------|---|--------------------------|---|--------------------------|---|
+| ft.divider               | ✔ | ft.image                 | ✔ | ft.snackbar              | ✘ |
+| ft.verticaldivider       | + | ft.circleavatar          | + | ft.tooltip               | ✔ |
+|                          |   | ft.icon                  | ✔ | ft.cupertinoalertdialog  | ✘ |
+|                          |   |                          |   | ft.cupertinodialogaction | ✘ |
+|                          |   |                          |   |                          |   |
+| **CONTAINERS LAYOUTS**   |   | **CHARTS LAYOUTS**       |   | **TEXT WIDGET**          |   |
+| ft.stack                 | ✔ | ft.barchart              | ✘ | ft.text                  | ✔ |
+| ft.row                   | ✔ | ft.charts                | ✘ | ft.textfield             | ✔ |
+| ft.gridview              | ✔ | ft.linechart             | ✘ | ft.listview              | ✘ |
+| ft.column                | ✔ | ft.matplotlibchart       | ✘ | ft.datatable             | ✘ |
+| ft.container             | ✔ | ft.piechart              | ✘ |                          |   |
+| ft.card                  | ✘ | ft.plotlychart           | ✘ |                          |   |
+| ft.responsiverow         | ✘ |                          |   |                          |   |
+| ft.transparentpointer    | ✘ |                          |   |                          |   |
+|                          |   |                          |   |                          |   |
+| **BUTTONS WIDGET**       |   | **SELECTIONS WIDGET**    |   | **ESPECIAL WIDGET**      |   |
+| ft.textbutton            | ✔ | ft.switch                | ✘ | ft.tabs                  | ✘ |
+| ft.filledbutton          | ✔ | ft.checkbox              | ✔ | ft.navigationbar         | ✘ |
+| ft.filledtonalbutton     | ✔ | ft.cupertinocheckbox     | ✔ | ft.cupertinoappbar       | ✘ |
+| ft.iconbutton            | ✔ | ft.cupertinoradio        | ✔ | ft.navigationdrawer      | ✘ |
+| ft.elevatedbutton        | ✔ | ft.cupertinoslider       | ✔ | ft.navigationrail        | ✘ |
+| ft.chip                  | ✔ | ft.cupertinoswitch       | ✔ | ft.menubar               | ✘ |
+| ft.outlinedbutton        | ✔ | ft.submenubutton         | ✘ | ft.appbar                | ✘ |
+| ft.bottomappbar          | ✘ | ft.dropdown              | ✘ | ft.cupertinonavigationbar| ✘ |
+| ft.bottomsheet           | ✘ | ft.datepicker            | ✘ | ft.searchbar             | ✘ |
+| ft.segmentedbutton       | ✘ | ft.timepicker            | ✘ |
+| ft.floatingactionbutton  | ✘ | ft.filepicker            | ✘ |
+|                          |   | ft.radio                 | ✘ |
+|                          |   |                          |   |                          |   |
+| **WIDGETS STATUS**       |   |
+| ft.slider                | ✘ |
+| ft.progressbar           | ✘ |
+| ft.progressring          | ✘ |
+| ft.alertdialog           | ✘ |
+| ft.rangeslider           | ✘ |
+
+<!-- make tree -->
+ <!-- tree -I '__pycache__|__init__.py|test|drag_drop_proyect|flet_box.egg-info|docs|.|build|dist|LICENSE|MANIFEST.in|requeriments.txt|README.md|pyproject.toml|setup.py' > full_path.txt -->
+
+### Path Flet-Box Modules
+```bash
+.
+├── full_path.txt
+├── src
+│   ├── assets
+│   │   ├── avatar.jpg
+│   │   ├── avatar.png
+│   │   ├── dragg_container3.jpg
+│   │   ├── dragg_container.jpg
+│   │   ├── image.jpg
+│   │   ├── img.jpg
+│   │   ├── iphone.png
+│   │   ├── logo.jpg
+│   │   ├── logo_mark.png
+│   │   ├── my_avatar.png
+│   │   ├── no_imagen.jpg
+│   │   └── splash.jpg
+│   ├── bump-version.sh
+│   ├── CHANGELOG.md
+│   ├── extra_utils
+│   │   ├── about
+│   │   │   └── about.py
+│   │   ├── alert
+│   │   │   └── alert_selected.py
+│   │   ├── chat_gpt_browser
+│   │   │   ├── gpt_browser.py
+│   │   │   └── library_chatgpt.py
+│   │   ├── color_browser
+│   │   │   └── color_browser.py
+│   │   ├── config_container
+│   │   │   ├── bool_entry.py
+│   │   │   ├── color_entry.py
+│   │   │   ├── double_entry.py
+│   │   │   ├── four_entry.py
+│   │   │   ├── gradient_entry.py
+│   │   │   ├── selection_entry.py
+│   │   │   ├── single_entry.py
+│   │   │   └── widget_editor.py
+│   │   ├── drag_container
+│   │   │   ├── dragg_widget.py
+│   │   │   ├── drag_handler_container.py
+│   │   │   ├── infinity_box_layer_one.py
+│   │   │   └── widget_drag_editor.py
+│   │   ├── icon_browser
+│   │   │   └── icon_browser.py
+│   │   ├── lite_menu_bar_down_phone
+│   │   │   ├── footer_bar_menu_phone.py
+│   │   │   └── selected_widget.py
+│   │   ├── lite_menu_bar_up_phone
+│   │   │   └── head_bar_menu_phone.py
+│   │   ├── menu_tab_left_phone
+│   │   │   └── widget_menu_left_editor.py
+│   │   ├── menu_tab_up_phone
+│   │   │   ├── basic_menu_tab_up.py
+│   │   │   └── widget_menu_tab_editor.py
+│   │   ├── phone_container
+│   │   │   └── widget_phone_editor.py
+│   │   ├── settings_var
+│   │   │   ├── save_export.py
+│   │   │   └── settings_widget.py
+│   │   └── tree_view
+│   │       ├── tree_view.py
+│   │       └── tree_view_text_editor.py
+│   ├── flet_box.py
+│   ├── __main__.py
+│   └── VERSION
+└── workflows
+
+18 directories, 47 files
+
+```
+
+### Certainly!
+
+If you're passionate about shaping the future of frameworks and contributing to their development, I invite you to join our collaborative efforts. Here's how you can get involved:
+
+1. **Documentation and Modules**:
+
+   - **Documentation**: We're actively working on creating comprehensive documentation for our Flet-Box framework. Your contributions can help make it more accessible, accurate, and user-friendly. Whether you're an expert or a beginner, your insights matter!
+
+   - **Modules**: Our framework consists of various modules that handle different aspects of Flet activities. If you have expertise in any specific area (such as Documentation, Modules, or consensus algorithms ), consider contributing by improving existing modules or proposing new ones.
+
+2. **Financial Considerations**:
+
+    - If you're passionate about supporting open-source projects and want to contribute to the **Flet-box Framework**, here's a simple invitation for you:
+
+    **You may contribute Donating tokens to give suppor to the proyect in  MATIC , BINANCE or TRX Tokens**
+
+    - **Low Fees**: In transactions have extremely low fees, making it ideal for micro-donations.
+    - Invite me a **COFFE** or a **BEER** ..
+
+    **How to Donate Tokens:**
+    - **Get Token**: Purchase MATIC , BINANCE or TRX on platforms like Binance, Coinbase, or Uniswap.
+    - **Donate**: Visit the Flet-box page and contribute directly. **Every donation counts!**
+
+    **MATIC WALLET**
+
+| **SPACE LAYOUTS**                                                                         |    **ADDRESS**                                            |
+|-------------------------------------------------------------------------------------------|-----------------------------------------------------------|
+| <img src="docs/assets/matics_wallet.jpeg" style="width:60px" align="Center">              | 0x6d437bB66af8d2c44670eA18F059BE1417Dcd7bA                |
+| <img src="docs/assets/trx_wallet.jpeg" style="width:60px" align="Center">                 | THi2UTY8SrUYNrzqKek8U3pvLuEF5y4fDQ                        |
+| <img src="docs/assets/bnb_wallet.jpeg" style="width:60px" align="Center">                 | bnb1vhe8q5zf2fr6s0ga8dnm5nzaz9uapky6w2xcnr                |
+
+    - **Learn More**: Explore Flet-box's mission, roadmap, and community initiatives on their official website.
+
+3. **Collaboration and Feedback**:
+   - We value diverse perspectives. Engage in discussions, attend working groups, and provide feedback during public consultations.
+
+###  How to Get Started:
+
+* Reach out to our team via the provided contact details if you have specific questions or want to contribute directly.
+* Remember, every contribution counts! Let's build a robust and forward-looking framework that fosters innovation while safeguarding financial stability.
+
+##  How contribute to build Widget dragg in flet-Box
+
+1.  Build left take dragg selection widgets.
+
+**Exemple:**
+
+```python
+
+self.RowDragg  = DraggWidget( widget='Row' ,color='BLUE' ,icons= ft.icons.BURST_MODE_ROUNDED)
+
+```
+    **Properties:**
+
+        * widget <== 'Widget name'
+        * color  <== 'Color of the box Dragg'
+        * icons  <== 'icons of the box Dragg'
+
+    * **we create a Object named self.RowDragg that we will add inside drag_container_to_phone object.**
+
+    #### After we need add manual inside [ drag_container_to_phone ]
+
+2.  Exemple build left take dragg selection widgets inside drag_container_to_phone.
+
+```python
+
+ft.Container(
+        content=ft.GridView(
+                            runs_count=3,
+                            run_spacing=8,
+                            padding=4,
+                            spacing=8,
+                            expand=1,
+                        controls=[
+                                    self.RowDragg, # <============= add inside
+                                 ],
+
+```
+
+3.  Go to infinity_box_layer_one.py and add Manually.
+
+**Location:**
+
+- ***'extra_utils/drag_container/infinity_box_layer_one.py'***
+
+- we need build the Container that will have the drop Widget inside
+
+**Exemple how will be**
+
+```python
+
+"Row": [
+            ft.Container(bgcolor='blue',alignment=ft.alignment.center,padding=ft.padding.all(4),border=ft.border.all(0.8, ft.colors.BLACK),tooltip='Row',
+        on_hover=lambda _:self.resetClick(),
+        on_click=lambda _:self.touchWidgetIndex(self.infinityDropWidget),
+        content=ft.Row( scroll="ALWAYS",
+            controls= [
+                           ],),),
+  ],
+
+```
```

### Comparing `flet-box-gui-0.1.2/flet_box/assets/avatar.jpg` & `flet-box-gui-0.1.2.1/flet_box/assets/avatar.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/assets/avatar.png` & `flet-box-gui-0.1.2.1/flet_box/assets/avatar.png`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/assets/dragg_container.jpg` & `flet-box-gui-0.1.2.1/flet_box/assets/dragg_container.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/assets/dragg_container3.jpg` & `flet-box-gui-0.1.2.1/flet_box/assets/dragg_container3.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/assets/image.jpg` & `flet-box-gui-0.1.2.1/flet_box/assets/image.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/assets/img.jpg` & `flet-box-gui-0.1.2.1/flet_box/assets/img.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/assets/logo.jpg` & `flet-box-gui-0.1.2.1/flet_box/assets/logo.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/assets/logo_mark.png` & `flet-box-gui-0.1.2.1/flet_box/assets/logo_mark.png`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/assets/my_avatar.png` & `flet-box-gui-0.1.2.1/flet_box/assets/my_avatar.png`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/assets/no_imagen.jpg` & `flet-box-gui-0.1.2.1/flet_box/assets/no_imagen.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/assets/splash.jpg` & `flet-box-gui-0.1.2.1/flet_box/assets/splash.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/assets/wallpaper.jpg` & `flet-box-gui-0.1.2.1/flet_box/assets/wallpaper.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/about/about.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/about/about.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/alert/alert_selected.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/alert/alert_selected.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/chat_gpt_browser/gpt_browser.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/chat_gpt_browser/gpt_browser.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/chat_gpt_browser/library_chatgpt.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/chat_gpt_browser/library_chatgpt.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/color_browser/color_browser.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/color_browser/color_browser.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/config_container/blur_color_entry.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/blur_color_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/config_container/bool_entry.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/bool_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/config_container/color_entry.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/color_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/config_container/double_entry.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/double_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/config_container/four_entry.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/four_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/config_container/gradient_entry.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/gradient_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/config_container/selection_entry.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/selection_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/config_container/single_entry.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/single_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/config_container/widget_editor.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/widget_editor.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/drag_container/dragg_widget.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/dragg_widget.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/drag_container/infinity_box_layer_one.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/infinity_box_layer_one.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/drag_container/widget_drag_editor.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/widget_drag_editor.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/icon_browser/icon_browser.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/icon_browser/icon_browser.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/lite_menu_bar_down_phone/footer_bar_menu_phone.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_down_phone/footer_bar_menu_phone.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/lite_menu_bar_down_phone/selected_widget.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_down_phone/selected_widget.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/lite_menu_bar_right_phone/right_bar_menu_phone.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_right_phone/right_bar_menu_phone.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/menu_tab_left_phone/widget_menu_left_editor.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_left_phone/widget_menu_left_editor.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/menu_tab_up_phone/basic_menu_tab_up.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/basic_menu_tab_up.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/menu_tab_up_phone/skeleton_class_screens.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/skeleton_class_screens.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/menu_tab_up_phone/widget_menu_tab_editor.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/widget_menu_tab_editor.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/phone_container/widget_phone_editor.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/phone_container/widget_phone_editor.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/screen_manager/screen_manager.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/screen_manager.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/screen_manager/settings_screens.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/settings_screens.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/screen_manager/write_file_proyect.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/write_file_proyect.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/settings_var/save_export.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/settings_var/save_export.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/settings_var/settings_widget.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/settings_var/settings_widget.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/tree_view/color_hight_light_editor.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/color_hight_light_editor.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/tree_view/tree_view.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/tree_view.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/extra_utils/tree_view/tree_view_text_editor.py` & `flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/tree_view_text_editor.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box/flet_box.py` & `flet-box-gui-0.1.2.1/flet_box/flet_box.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2/flet_box_gui.egg-info/SOURCES.txt` & `flet-box-gui-0.1.2.1/flet_box_gui.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+CHANGELOG.md
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 flet_box/__init__.py
 flet_box/flet_box.py
 flet_box/assets/avatar.jpg
 flet_box/assets/avatar.png
```

### Comparing `flet-box-gui-0.1.2/setup.py` & `flet-box-gui-0.1.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 from setuptools import setup , find_packages
 import os
 import pypandoc
+import sys
 
 #: MAKE A SETUP INSTALL
 # python3 setup.py sdist bdist_wheel
 # python3 setup.py bdist_wheel
 # python3 setup.py register -r pypi
 # python3 setup.py sdist upload -r pypi
 
+# $ python setup.py sdist
+# $ twine upload dist/* -r pypi
+# $ twine upload dist/* -r flet_box_gui
+
+# $ python setup.py sdist bdist_wheel --universal
+# $ twine upload dist/* -r pypi
+
 # pip install twine ,pypandoc
 # twine upload dist/*
 # PACKAGE META-DATA
 
+# python3 -m pip install --upgrade pip
+# pip install pypandoc
+# pip install pypandoc_binary
+
+# errors pip
+# sudo apt install libgpgme-dev swig
+# pip install --upgrade gpg
+
 NAME            = 'flet-box-gui'
 DESCRIPTION     = "flet-box-gui it's a GUI Dragg and drop BUILDER."
 PLATAFORM       = 'Multy platforms'
 REQUIRES_PYTHON = '>=3.8'
 
 AUTHOR          = 'xavier53348'
 EMAIL           = 'xavier53348@gmail.com'
@@ -39,28 +55,20 @@
 ],
 }
 
 PYPY_KEYWORDS_TO_FIND = ["flet-box-gui", "flet",'flet-gui','flet-builder','flet-sdk']
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-#: MANAGE README
 try:
-    # with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-    with open('README.md', "r") as f:
-        long_description = '\n' + f.read()
-        print(long_description)
-
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# try:
-#     long_description = pypandoc.convert_file('README.md', 'rst')
-# except(IOError, ImportError):
-#     long_description = open('README.md').read()
+    long_description = pypandoc.convert_file('README.md', 'rst')
+except(IOError, ImportError):
+    long_description = open('README.md').read()
+    data = "\n\tpip install pypandoc\n\tpip install pypandoc_binary"
+    print(f'Please install {data}')
 
 #: MANAGE VERSION
 try:
     with open(os.path.join(here, 'VERSION'), encoding='utf-8') as f:
         VERSION = f.read()
 
 except FileNotFoundError:
@@ -72,26 +80,26 @@
     "Changelog": CHANGE_LOG ,
     "Roadmap":ROADMAP,
 
 }
 
 setup(
     #: PERSONAL DATA
-    name                 = NAME,
-    author               = AUTHOR,
-    author_email         = EMAIL,
-    maintainer           = MANTAINER,
-    maintainer_email     = MANTAINER_EMAIL,
+    name                          = NAME,
+    author                        = AUTHOR,
+    author_email                  = EMAIL,
+    maintainer                    = MANTAINER,
+    maintainer_email              = MANTAINER_EMAIL,
 
     #: PROJECT DESCRIOPTION
-    description          = DESCRIPTION,
-    long_description=open("README.md", 'r').read(),
-    long_description_content_type='text/markdown',
-    url                  = URL,
-    project_urls         = PROJECT_DOCUMENTATION,
+    description                   =  DESCRIPTION,
+    long_description              = long_description,
+    long_description_content_type = 'text/markdown',
+    url                           = URL,
+    project_urls                  = PROJECT_DOCUMENTATION,
 
     #: DISTRIBUTION
     platforms            = PLATAFORM,
     version              = VERSION,
     packages             = find_packages(),
 
     #: EXTRA FILES INCLUID
@@ -120,14 +128,15 @@
 
         'Development Status :: 1 - Planning',
         "Topic :: Software Development :: Build Tools",
         'Intended Audience :: Developers',
         'Natural Language :: English',
         # 'License :: OSI Approved :: Apache License',
 
+        "License :: OSI Approved :: MIT License",
         # "License :: OSI Approved :: GNU General Public License (GPL)"
         # "License :: OSI Approved :: GNU General Public License v2 (GPLv2)"
         # "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)"
         # "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
         # "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
```

