# Comparing `tmp/labelme-ytu-5.4.1.tar.gz` & `tmp/labelme-ytu-5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelme-ytu-5.4.1.tar", last modified: Wed Apr 24 08:57:08 2024, max compression
+gzip compressed data, was "labelme-ytu-5.5.1.tar", last modified: Tue May 28 13:51:50 2024, max compression
```

## Comparing `labelme-ytu-5.4.1.tar` & `labelme-ytu-5.5.1.tar`

### file list

```diff
@@ -1,101 +1,104 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:08.096854 labelme-ytu-5.4.1/
--rw-rw-rw-   0        0        0      702 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/LICENSE
--rw-rw-rw-   0        0        0       19 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11650 2024-04-24 08:57:08.095854 labelme-ytu-5.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     9239 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:07.616337 labelme-ytu-5.4.1/labelme/
--rw-rw-rw-   0        0        0      700 2024-04-22 20:59:35.000000 labelme-ytu-5.4.1/labelme/__init__.py
--rw-rw-rw-   0        0        0     6176 2024-04-24 07:02:44.000000 labelme-ytu-5.4.1/labelme/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:07.667097 labelme-ytu-5.4.1/labelme/ai/
--rw-rw-rw-   0        0        0     3692 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/ai/__init__.py
--rw-rw-rw-   0        0        0     1379 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/ai/_utils.py
--rw-rw-rw-   0        0        0     3537 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/ai/efficient_sam.py
--rw-rw-rw-   0        0        0     5395 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/ai/segment_anything_model.py
--rw-rw-rw-   0        0        0     1130 2024-04-24 05:53:34.000000 labelme-ytu-5.4.1/labelme/ai/yolo.py
--rw-rw-rw-   0        0        0    83586 2024-04-24 05:58:55.000000 labelme-ytu-5.4.1/labelme/app.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:07.742727 labelme-ytu-5.4.1/labelme/cli/
--rw-rw-rw-   0        0        0      125 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/cli/__init__.py
--rw-rw-rw-   0        0        0     1382 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/cli/draw_json.py
--rw-rw-rw-   0        0        0     2342 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/cli/draw_label_png.py
--rw-rw-rw-   0        0        0     2188 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/cli/export_json.py
--rw-rw-rw-   0        0        0     2574 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/cli/json_to_dataset.py
--rw-rw-rw-   0        0        0     2851 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/cli/on_docker.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:07.768087 labelme-ytu-5.4.1/labelme/config/
--rw-rw-rw-   0        0        0     2660 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/config/__init__.py
--rw-rw-rw-   0        0        0     2492 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/config/default_config.yaml
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:07.906549 labelme-ytu-5.4.1/labelme/icons/
--rw-rw-rw-   0        0        0    14797 2024-04-22 12:00:13.000000 labelme-ytu-5.4.1/labelme/icons/ai.png
--rw-rw-rw-   0        0        0     2136 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/cancel.png
--rw-rw-rw-   0        0        0     3111 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/close.png
--rw-rw-rw-   0        0        0     2368 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/color-line.png
--rw-rw-rw-   0        0        0     2760 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/color.png
--rw-rw-rw-   0        0        0     1210 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/copy.png
--rw-rw-rw-   0        0        0     2879 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/delete.png
--rw-rw-rw-   0        0        0     2198 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/done.png
--rw-rw-rw-   0        0        0    22632 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/done.svg
--rw-rw-rw-   0        0        0     2144 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/edit.png
--rw-rw-rw-   0        0        0     7718 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/expert.png
--rw-rw-rw-   0        0        0     1264 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/eye.png
--rw-rw-rw-   0        0        0     8059 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/feBlend-icon.png
--rw-rw-rw-   0        0        0      765 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/file.png
--rw-rw-rw-   0        0        0     2743 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/fit-width.png
--rw-rw-rw-   0        0        0     1474 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/fit-window.png
--rw-rw-rw-   0        0        0     2262 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/fit.png
--rw-rw-rw-   0        0        0     1587 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/help.png
--rw-rw-rw-   0        0        0  1128131 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/icon.icns
--rw-rw-rw-   0        0        0   183198 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/icon.ico
--rw-rw-rw-   0        0        0    44771 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/icon.png
--rw-rw-rw-   0        0        0     2381 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/labels.png
--rw-rw-rw-   0        0        0    37512 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/labels.svg
--rw-rw-rw-   0        0        0      977 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/new.png
--rw-rw-rw-   0        0        0     2139 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/next.png
--rw-rw-rw-   0        0        0     3205 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/objects.png
--rw-rw-rw-   0        0        0     2073 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/open.png
--rw-rw-rw-   0        0        0    18773 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/open.svg
--rw-rw-rw-   0        0        0     2115 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/prev.png
--rw-rw-rw-   0        0        0     1915 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/quit.png
--rw-rw-rw-   0        0        0     2811 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/save-as.png
--rw-rw-rw-   0        0        0    65363 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/save-as.svg
--rw-rw-rw-   0        0        0     1187 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/save.png
--rw-rw-rw-   0        0        0    31292 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/save.svg
--rw-rw-rw-   0        0        0     2004 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/undo-cross.png
--rw-rw-rw-   0        0        0     2231 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/undo.png
--rw-rw-rw-   0        0        0     1099 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/zoom-in.png
--rw-rw-rw-   0        0        0     1074 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/zoom-out.png
--rw-rw-rw-   0        0        0     1139 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/icons/zoom.png
--rw-rw-rw-   0        0        0     7425 2024-04-24 06:10:13.000000 labelme-ytu-5.4.1/labelme/label_file.py
--rw-rw-rw-   0        0        0     1742 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/logger.py
--rw-rw-rw-   0        0        0    13043 2024-04-08 23:45:14.000000 labelme-ytu-5.4.1/labelme/shape.py
--rw-rw-rw-   0        0        0      884 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/testing.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:07.938581 labelme-ytu-5.4.1/labelme/translate/
--rw-rw-rw-   0        0        0    23225 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/translate/empty.ts
--rw-rw-rw-   0        0        0     9420 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/translate/zh_CN.qm
--rw-rw-rw-   0        0        0    24011 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/translate/zh_CN.ts
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:07.987787 labelme-ytu-5.4.1/labelme/utils/
--rw-rw-rw-   0        0        0      819 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/utils/__init__.py
--rw-rw-rw-   0        0        0      745 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/utils/_io.py
--rw-rw-rw-   0        0        0     2705 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/utils/image.py
--rw-rw-rw-   0        0        0     2510 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/utils/qt.py
--rw-rw-rw-   0        0        0     3759 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/utils/shape.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:08.059158 labelme-ytu-5.4.1/labelme/widgets/
--rw-rw-rw-   0        0        0      570 2024-04-22 12:35:06.000000 labelme-ytu-5.4.1/labelme/widgets/__init__.py
--rw-rw-rw-   0        0        0     1513 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/widgets/brightness_contrast_dialog.py
--rw-rw-rw-   0        0        0    40884 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/widgets/canvas.py
--rw-rw-rw-   0        0        0     1231 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/widgets/color_dialog.py
--rw-rw-rw-   0        0        0      243 2024-04-22 13:59:28.000000 labelme-ytu-5.4.1/labelme/widgets/error_dialog.py
--rw-rw-rw-   0        0        0      290 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/widgets/escapable_qlist_widget.py
--rw-rw-rw-   0        0        0     2471 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/widgets/file_dialog_preview.py
--rw-rw-rw-   0        0        0     8889 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/widgets/label_dialog.py
--rw-rw-rw-   0        0        0     5885 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/widgets/label_list_widget.py
--rw-rw-rw-   0        0        0      966 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/widgets/tool_bar.py
--rw-rw-rw-   0        0        0     1389 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/widgets/unique_label_qlist_widget.py
--rw-rw-rw-   0        0        0      733 2024-04-08 16:26:09.000000 labelme-ytu-5.4.1/labelme/widgets/zoom_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:57:08.093896 labelme-ytu-5.4.1/labelme_ytu.egg-info/
--rw-rw-rw-   0        0        0    11650 2024-04-24 08:57:07.000000 labelme-ytu-5.4.1/labelme_ytu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2297 2024-04-24 08:57:07.000000 labelme-ytu-5.4.1/labelme_ytu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 08:57:07.000000 labelme-ytu-5.4.1/labelme_ytu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      315 2024-04-24 08:57:07.000000 labelme-ytu-5.4.1/labelme_ytu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      157 2024-04-24 08:57:07.000000 labelme-ytu-5.4.1/labelme_ytu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 08:57:07.000000 labelme-ytu-5.4.1/labelme_ytu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 08:57:08.096854 labelme-ytu-5.4.1/setup.cfg
--rw-rw-rw-   0        0        0     4868 2024-04-24 08:48:38.000000 labelme-ytu-5.4.1/setup.py
+drwxrwxrwx   0 ismail    (1000) ismail    (1000)        0 2024-05-28 13:51:50.821074 labelme-ytu-5.5.1/
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      702 2024-04-24 17:22:41.000000 labelme-ytu-5.5.1/LICENSE
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)       19 2024-04-24 17:22:41.000000 labelme-ytu-5.5.1/MANIFEST.in
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    10270 2024-05-28 13:51:50.812415 labelme-ytu-5.5.1/PKG-INFO
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     9243 2024-04-24 17:47:16.000000 labelme-ytu-5.5.1/README.md
+drwxrwxrwx   0 ismail    (1000) ismail    (1000)        0 2024-05-28 13:51:48.814738 labelme-ytu-5.5.1/labelme/
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      700 2024-05-28 13:51:42.000000 labelme-ytu-5.5.1/labelme/__init__.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     5952 2024-05-19 20:30:14.000000 labelme-ytu-5.5.1/labelme/__main__.py
+drwxrwxrwx   0 ismail    (1000) ismail    (1000)        0 2024-05-28 13:51:48.918892 labelme-ytu-5.5.1/labelme/ai/
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     3692 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/ai/__init__.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1379 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/ai/_utils.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     3537 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/ai/efficient_sam.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     5395 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/ai/segment_anything_model.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1484 2024-05-19 20:29:47.000000 labelme-ytu-5.5.1/labelme/ai/yolo.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    92728 2024-05-28 12:43:00.000000 labelme-ytu-5.5.1/labelme/app.py
+drwxrwxrwx   0 ismail    (1000) ismail    (1000)        0 2024-05-28 13:51:49.062049 labelme-ytu-5.5.1/labelme/cli/
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      125 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/cli/__init__.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1382 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/cli/draw_json.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2342 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/cli/draw_label_png.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2188 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/cli/export_json.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2574 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/cli/json_to_dataset.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2851 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/cli/on_docker.py
+drwxrwxrwx   0 ismail    (1000) ismail    (1000)        0 2024-05-28 13:51:49.113603 labelme-ytu-5.5.1/labelme/config/
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2660 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/config/__init__.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2520 2024-05-19 19:30:22.000000 labelme-ytu-5.5.1/labelme/config/default_config.yaml
+drwxrwxrwx   0 ismail    (1000) ismail    (1000)        0 2024-05-28 13:51:50.162804 labelme-ytu-5.5.1/labelme/icons/
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    14797 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/icons/ai.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2136 2024-04-24 17:22:43.000000 labelme-ytu-5.5.1/labelme/icons/cancel.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     3111 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/close.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2368 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/color-line.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2760 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/color.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1210 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/copy.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2879 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/delete.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2198 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/done.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    22632 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/done.svg
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2144 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/edit.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     7718 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/expert.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1264 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/eye.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     8059 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/feBlend-icon.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      765 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/file.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2743 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/fit-width.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1474 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/fit-window.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2262 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/fit.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1587 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/help.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)   258048 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/icon.icns
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)   266302 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/icon.ico
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    76778 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/icon.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2381 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/labels.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    37512 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/labels.svg
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      977 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/new.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2139 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/next.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     3205 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/objects.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2073 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/open.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    18773 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/open.svg
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2115 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/prev.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1915 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/quit.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2811 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/save-as.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    65363 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/save-as.svg
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1187 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/save.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    31292 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/save.svg
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2004 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/undo-cross.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2231 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/undo.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    47450 2024-05-19 21:16:06.000000 labelme-ytu-5.5.1/labelme/icons/yildiz.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1099 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/zoom-in.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1074 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/zoom-out.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1139 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/icons/zoom.png
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     7425 2024-04-25 11:25:05.000000 labelme-ytu-5.5.1/labelme/label_file.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1742 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/logger.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    13043 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/shape.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      884 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/testing.py
+drwxrwxrwx   0 ismail    (1000) ismail    (1000)        0 2024-05-28 13:51:50.232816 labelme-ytu-5.5.1/labelme/translate/
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    23225 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/translate/empty.ts
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     9420 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/translate/zh_CN.qm
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    24011 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/translate/zh_CN.ts
+drwxrwxrwx   0 ismail    (1000) ismail    (1000)        0 2024-05-28 13:51:50.354845 labelme-ytu-5.5.1/labelme/utils/
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      819 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/utils/__init__.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      745 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/utils/_io.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2705 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/utils/image.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2510 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/utils/qt.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     3759 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/utils/shape.py
+drwxrwxrwx   0 ismail    (1000) ismail    (1000)        0 2024-05-28 13:51:50.682014 labelme-ytu-5.5.1/labelme/widgets/
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      621 2024-05-04 12:17:47.000000 labelme-ytu-5.5.1/labelme/widgets/__init__.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1513 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/widgets/brightness_contrast_dialog.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    41027 2024-05-24 16:53:21.000000 labelme-ytu-5.5.1/labelme/widgets/canvas.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1231 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/widgets/color_dialog.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      933 2024-05-04 12:17:47.000000 labelme-ytu-5.5.1/labelme/widgets/directory_selector.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      303 2024-04-25 11:25:05.000000 labelme-ytu-5.5.1/labelme/widgets/error_dialog.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      290 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/widgets/escapable_qlist_widget.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2471 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/widgets/file_dialog_preview.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      741 2024-05-04 12:17:47.000000 labelme-ytu-5.5.1/labelme/widgets/file_selector.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     8889 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/widgets/label_dialog.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     5885 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/widgets/label_list_widget.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      966 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/widgets/tool_bar.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     1389 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/widgets/unique_label_qlist_widget.py
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      733 2024-04-24 17:22:44.000000 labelme-ytu-5.5.1/labelme/widgets/zoom_widget.py
+drwxrwxrwx   0 ismail    (1000) ismail    (1000)        0 2024-05-28 13:51:50.792559 labelme-ytu-5.5.1/labelme_ytu.egg-info/
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)    10270 2024-05-28 13:51:47.000000 labelme-ytu-5.5.1/labelme_ytu.egg-info/PKG-INFO
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     2393 2024-05-28 13:51:48.000000 labelme-ytu-5.5.1/labelme_ytu.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)        1 2024-05-28 13:51:47.000000 labelme-ytu-5.5.1/labelme_ytu.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      315 2024-05-28 13:51:47.000000 labelme-ytu-5.5.1/labelme_ytu.egg-info/entry_points.txt
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)      148 2024-05-28 13:51:47.000000 labelme-ytu-5.5.1/labelme_ytu.egg-info/requires.txt
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)        8 2024-05-28 13:51:47.000000 labelme-ytu-5.5.1/labelme_ytu.egg-info/top_level.txt
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)       38 2024-05-28 13:51:50.822469 labelme-ytu-5.5.1/setup.cfg
+-rwxrwxrwx   0 ismail    (1000) ismail    (1000)     4872 2024-05-28 12:43:50.000000 labelme-ytu-5.5.1/setup.py
```

### Comparing `labelme-ytu-5.4.1/LICENSE` & `labelme-ytu-5.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/PKG-INFO` & `labelme-ytu-5.5.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,101 +1,77 @@
-Metadata-Version: 2.1
-Name: labelme-ytu
-Version: 5.4.1
-Summary: Image Polygonal Annotation with Python
-Home-page: https://github.com/wkentaro/labelme
-Author: Kentaro Wada
-Author-email: www.kentaro.wada@gmail.com
-License: GPLv3
-Keywords: Image Annotation,Machine Learning
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">
-  <img src="https://github.com/wkentaro/labelme/blob/main/labelme/icons/icon.png?raw=true"><br/>labelme
+  <img src="labelme/icons/icon.png"><br/>labelme-ytu
 </h1>
 
 <h4 align="center">
   Image Polygonal Annotation with Python
 </h4>
 
 <div align="center">
   <a href="https://pypi.python.org/pypi/labelme"><img src="https://img.shields.io/pypi/v/labelme.svg"></a>
   <a href="https://pypi.org/project/labelme"><img src="https://img.shields.io/pypi/pyversions/labelme.svg"></a>
   <a href="https://github.com/wkentaro/labelme/actions"><img src="https://github.com/wkentaro/labelme/workflows/ci/badge.svg?branch=main&event=push"></a>
 </div>
 
 <div align="center">
-  <a href="https://github.com/wkentaro/labelme/blob/main/#starter-guide"><b>Starter Guide</b></a>
-  | <a href="https://github.com/wkentaro/labelme/blob/main/#installation?raw=true"><b>Installation</b></a>
-  | <a href="https://github.com/wkentaro/labelme/blob/main/#usage"><b>Usage</b></a>
-  | <a href="https://github.com/wkentaro/labelme/blob/main/#examples"><b>Examples</b></a>
+  <a href="#starter-guide"><b>Starter Guide</b></a>
+  | <a href="#installation"><b>Installation</b></a>
+  | <a href="#usage"><b>Usage</b></a>
+  | <a href="#examples"><b>Examples</b></a>
   | <a href="https://x.com/labelmeai"><b>X/Twitter</b></a>
   <!-- | <a href="https://github.com/wkentaro/labelme/discussions"><b>Community</b></a> -->
   <!-- | <a href="https://www.youtube.com/playlist?list=PLI6LvFw0iflh3o33YYnVIfOpaO0hc5Dzw"><b>Youtube FAQ</b></a> -->
 </div>
 
 <br/>
 
 <div align="center">
-  <img src="https://github.com/wkentaro/labelme/blob/main/examples/instance_segmentation/.readme/annotation.jpg?raw=true" width="70%">
+  <img src="examples/instance_segmentation/.readme/annotation.jpg" width="70%">
 </div>
 
 ## Description
 
 Labelme is a graphical image annotation tool inspired by <http://labelme.csail.mit.edu>.  
 It is written in Python and uses Qt for its graphical interface.
 
-<img src="https://github.com/wkentaro/labelme/blob/main/examples/instance_segmentation/data_dataset_voc/JPEGImages/2011_000006.jpg?raw=true" width="19%" /> <img src="examples/instance_segmentation/data_dataset_voc/SegmentationClass/2011_000006.png" width="19%" /> <img src="examples/instance_segmentation/data_dataset_voc/SegmentationClassVisualization/2011_000006.jpg" width="19%" /> <img src="examples/instance_segmentation/data_dataset_voc/SegmentationObject/2011_000006.png" width="19%" /> <img src="examples/instance_segmentation/data_dataset_voc/SegmentationObjectVisualization/2011_000006.jpg" width="19%" />  
+<img src="examples/instance_segmentation/data_dataset_voc/JPEGImages/2011_000006.jpg" width="19%" /> <img src="examples/instance_segmentation/data_dataset_voc/SegmentationClass/2011_000006.png" width="19%" /> <img src="examples/instance_segmentation/data_dataset_voc/SegmentationClassVisualization/2011_000006.jpg" width="19%" /> <img src="examples/instance_segmentation/data_dataset_voc/SegmentationObject/2011_000006.png" width="19%" /> <img src="examples/instance_segmentation/data_dataset_voc/SegmentationObjectVisualization/2011_000006.jpg" width="19%" />  
 <i>VOC dataset example of instance segmentation.</i>
 
-<img src="https://github.com/wkentaro/labelme/blob/main/examples/semantic_segmentation/.readme/annotation.jpg?raw=true" width="30%" /> <img src="examples/bbox_detection/.readme/annotation.jpg" width="30%" /> <img src="examples/classification/.readme/annotation_cat.jpg" width="35%" />  
+<img src="examples/semantic_segmentation/.readme/annotation.jpg" width="30%" /> <img src="examples/bbox_detection/.readme/annotation.jpg" width="30%" /> <img src="examples/classification/.readme/annotation_cat.jpg" width="35%" />  
 <i>Other examples (semantic segmentation, bbox detection, and classification).</i>
 
 <img src="https://user-images.githubusercontent.com/4310419/47907116-85667800-de82-11e8-83d0-b9f4eb33268f.gif" width="30%" /> <img src="https://user-images.githubusercontent.com/4310419/47922172-57972880-deae-11e8-84f8-e4324a7c856a.gif" width="30%" /> <img src="https://user-images.githubusercontent.com/14256482/46932075-92145f00-d080-11e8-8d09-2162070ae57c.png" width="32%" />  
 <i>Various primitives (polygon, rectangle, circle, line, and point).</i>
 
 
 ## Features
 
-- [x] Image annotation for polygon, rectangle, circle, line and point. ([tutorial](https://github.com/wkentaro/labelme/blob/main/examples/tutorial))
+- [x] Image annotation for polygon, rectangle, circle, line and point. ([tutorial](examples/tutorial))
 - [x] Image flag annotation for classification and cleaning. ([#166](https://github.com/wkentaro/labelme/pull/166))
-- [x] Video annotation. ([video annotation](https://github.com/wkentaro/labelme/blob/main/examples/video_annotation?raw=true))
+- [x] Video annotation. ([video annotation](examples/video_annotation))
 - [x] GUI customization (predefined labels / flags, auto-saving, label validation, etc). ([#144](https://github.com/wkentaro/labelme/pull/144))
-- [x] Exporting VOC-format dataset for semantic/instance segmentation. ([semantic segmentation](https://github.com/wkentaro/labelme/blob/main/examples/semantic_segmentation?raw=true), [instance segmentation](https://github.com/wkentaro/labelme/blob/main/examples/instance_segmentation?raw=true))
-- [x] Exporting COCO-format dataset for instance segmentation. ([instance segmentation](https://github.com/wkentaro/labelme/blob/main/examples/instance_segmentation?raw=true))
+- [x] Exporting VOC-format dataset for semantic/instance segmentation. ([semantic segmentation](examples/semantic_segmentation), [instance segmentation](examples/instance_segmentation))
+- [x] Exporting COCO-format dataset for instance segmentation. ([instance segmentation](examples/instance_segmentation))
 
 
 ## Starter Guide
 
 If you're new to Labelme, you can get started with [Labelme Starter Guide](https://labelme.gumroad.com/l/starter-guide) (FREE), which contains:
 
-- **Installation guides** for all platforms: Windows, macOS, and Linux ğŸ’»
-- **Step-by-step tutorials**: first annotation to editing, exporting, and integrating with other programs ğŸ“•
-- **A compilation of valuable resources** for further exploration ğŸ”—.
+- **Installation guides** for all platforms: Windows, macOS, and Linux 💻
+- **Step-by-step tutorials**: first annotation to editing, exporting, and integrating with other programs 📕
+- **A compilation of valuable resources** for further exploration 🔗.
 
 
 ## Installation
 
 There are options:
 
-- Platform agnostic installation: [Anaconda](https://github.com/wkentaro/labelme/blob/main/#anaconda)
-- Platform specific installation: [Ubuntu](https://github.com/wkentaro/labelme/blob/main/#ubuntu), [macOS](https://github.com/wkentaro/labelme/blob/main/#macos), [Windows](https://github.com/wkentaro/labelme/blob/main/#windows)
+- Platform agnostic installation: [Anaconda](#anaconda)
+- Platform specific installation: [Ubuntu](#ubuntu), [macOS](#macos), [Windows](#windows)
 - Pre-build binaries from [the release section](https://github.com/wkentaro/labelme/releases)
 
 ### Anaconda
 
 You need install [Anaconda](https://www.continuum.io/downloads), then run below:
 
 ```bash
@@ -172,32 +148,32 @@
 labelme data_annotated/ --labels labels.txt  # specify label list with a file
 ```
 
 ### Command Line Arguments
 - `--output` specifies the location that annotations will be written to. If the location ends with .json, a single annotation will be written to this file. Only one image can be annotated if a location is specified with .json. If the location does not end with .json, the program will assume it is a directory. Annotations will be stored in this directory with a name that corresponds to the image that the annotation was made on.
 - The first time you run labelme, it will create a config file in `~/.labelmerc`. You can edit this file and the changes will be applied the next time that you launch labelme. If you would prefer to use a config file from another location, you can specify this file with the `--config` flag.
 - Without the `--nosortlabels` flag, the program will list labels in alphabetical order. When the program is run with this flag, it will display labels in the order that they are provided.
-- Flags are assigned to an entire image. [Example](https://github.com/wkentaro/labelme/blob/main/examples/classification?raw=true)
-- Labels are assigned to a single polygon. [Example](https://github.com/wkentaro/labelme/blob/main/examples/bbox_detection?raw=true)
+- Flags are assigned to an entire image. [Example](examples/classification)
+- Labels are assigned to a single polygon. [Example](examples/bbox_detection)
 
 ### FAQ
 
-- **How to convert JSON file to numpy array?** See [examples/tutorial](https://github.com/wkentaro/labelme/blob/main/examples/tutorial#convert-to-dataset).
-- **How to load label PNG file?** See [examples/tutorial](https://github.com/wkentaro/labelme/blob/main/examples/tutorial#how-to-load-label-png-file).
-- **How to get annotations for semantic segmentation?** See [examples/semantic_segmentation](https://github.com/wkentaro/labelme/blob/main/examples/semantic_segmentation?raw=true).
-- **How to get annotations for instance segmentation?** See [examples/instance_segmentation](https://github.com/wkentaro/labelme/blob/main/examples/instance_segmentation?raw=true).
+- **How to convert JSON file to numpy array?** See [examples/tutorial](examples/tutorial#convert-to-dataset).
+- **How to load label PNG file?** See [examples/tutorial](examples/tutorial#how-to-load-label-png-file).
+- **How to get annotations for semantic segmentation?** See [examples/semantic_segmentation](examples/semantic_segmentation).
+- **How to get annotations for instance segmentation?** See [examples/instance_segmentation](examples/instance_segmentation).
 
 
 ## Examples
 
-* [Image Classification](https://github.com/wkentaro/labelme/blob/main/examples/classification?raw=true)
-* [Bounding Box Detection](https://github.com/wkentaro/labelme/blob/main/examples/bbox_detection?raw=true)
-* [Semantic Segmentation](https://github.com/wkentaro/labelme/blob/main/examples/semantic_segmentation?raw=true)
-* [Instance Segmentation](https://github.com/wkentaro/labelme/blob/main/examples/instance_segmentation?raw=true)
-* [Video Annotation](https://github.com/wkentaro/labelme/blob/main/examples/video_annotation?raw=true)
+* [Image Classification](examples/classification)
+* [Bounding Box Detection](examples/bbox_detection)
+* [Semantic Segmentation](examples/semantic_segmentation)
+* [Instance Segmentation](examples/instance_segmentation)
+* [Video Annotation](examples/video_annotation)
 
 ## How to develop
 
 ```bash
 git clone https://github.com/wkentaro/labelme.git
 cd labelme
```

#### html2text {}

```diff
@@ -1,97 +1,75 @@
-Metadata-Version: 2.1 Name: labelme-ytu Version: 5.4.1 Summary: Image Polygonal
-Annotation with Python Home-page: https://github.com/wkentaro/labelme Author:
-Kentaro Wada Author-email: www.kentaro.wada@gmail.com License: GPLv3 Keywords:
-Image Annotation,Machine Learning Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Science/Research Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 3.5 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3 :: Only Description-Content-Type: text/markdown License-File:
-LICENSE
-     ************ [[hhttttppss::////ggiitthhuubb..ccoomm//wwkkeennttaarroo//llaabbeellmmee//bblloobb//mmaaiinn//llaabbeellmmee//iiccoonnss//
-                              iiccoonn..ppnngg??rraaww==ttrruuee]]
-                                llaabbeellmmee ************
+                        ************ [[llaabbeellmmee//iiccoonnss//iiccoonn..ppnngg]]
+                              llaabbeellmmee--yyttuu ************
                 ****** IImmaaggee PPoollyyggoonnaall AAnnnnoottaattiioonn wwiitthh PPyytthhoonn ******
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_l_a_b_e_l_m_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/
    _p_y_v_e_r_s_i_o_n_s_/_l_a_b_e_l_m_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_w_k_e_n_t_a_r_o_/_l_a_b_e_l_m_e_/_w_o_r_k_f_l_o_w_s_/_c_i_/
                        _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_&_e_v_e_n_t_=_p_u_s_h_]
           _SS_tt_aa_rr_tt_ee_rr_ _GG_uu_ii_dd_ee | _II_nn_ss_tt_aa_ll_ll_aa_tt_ii_oo_nn | _UU_ss_aa_gg_ee | _EE_xx_aa_mm_pp_ll_ee_ss | _XX_//_TT_ww_ii_tt_tt_ee_rr
 
-           [https://github.com/wkentaro/labelme/blob/main/examples/
-            instance_segmentation/.readme/annotation.jpg?raw=true]
+            [examples/instance_segmentation/.readme/annotation.jpg]
 ## Description Labelme is a graphical image annotation tool inspired by
 labelme.csail.mit.edu>. It is written in Python and uses Qt for its graphical
-interface. [https://github.com/wkentaro/labelme/blob/main/examples/
-instance_segmentation/data_dataset_voc/JPEGImages/2011_000006.jpg?raw=true]
-[examples/instance_segmentation/data_dataset_voc/SegmentationClass/
-2011_000006.png][examples/instance_segmentation/data_dataset_voc/
-SegmentationClassVisualization/2011_000006.jpg][examples/instance_segmentation/
-data_dataset_voc/SegmentationObject/2011_000006.png][examples/
-instance_segmentation/data_dataset_voc/SegmentationObjectVisualization/
-2011_000006.jpg]VOC dataset example of instance segmentation. [https://
-github.com/wkentaro/labelme/blob/main/examples/semantic_segmentation/.readme/
-annotation.jpg?raw=true][examples/bbox_detection/.readme/annotation.jpg]
-[examples/classification/.readme/annotation_cat.jpg]Other examples (semantic
-segmentation, bbox detection, and classification). [https://user-
-images.githubusercontent.com/4310419/47907116-85667800-de82-11e8-83d0-
-b9f4eb33268f.gif][https://user-images.githubusercontent.com/4310419/47922172-
-57972880-deae-11e8-84f8-e4324a7c856a.gif][https://user-
-images.githubusercontent.com/14256482/46932075-92145f00-d080-11e8-8d09-
-2162070ae57c.png]Various primitives (polygon, rectangle, circle, line, and
-point). ## Features - [x] Image annotation for polygon, rectangle, circle, line
-and point. ([tutorial](https://github.com/wkentaro/labelme/blob/main/examples/
-tutorial)) - [x] Image flag annotation for classification and cleaning. ([#166]
-(https://github.com/wkentaro/labelme/pull/166)) - [x] Video annotation. ([video
-annotation](https://github.com/wkentaro/labelme/blob/main/examples/
-video_annotation?raw=true)) - [x] GUI customization (predefined labels / flags,
-auto-saving, label validation, etc). ([#144](https://github.com/wkentaro/
-labelme/pull/144)) - [x] Exporting VOC-format dataset for semantic/instance
-segmentation. ([semantic segmentation](https://github.com/wkentaro/labelme/
-blob/main/examples/semantic_segmentation?raw=true), [instance segmentation]
-(https://github.com/wkentaro/labelme/blob/main/examples/
-instance_segmentation?raw=true)) - [x] Exporting COCO-format dataset for
-instance segmentation. ([instance segmentation](https://github.com/wkentaro/
-labelme/blob/main/examples/instance_segmentation?raw=true)) ## Starter Guide If
-you're new to Labelme, you can get started with [Labelme Starter Guide](https:/
-/labelme.gumroad.com/l/starter-guide) (FREE), which contains: - **Installation
-guides** for all platforms: Windows, macOS, and Linux ÄÅ¸âÂ» - **Step-by-
-step tutorials**: first annotation to editing, exporting, and integrating with
-other programs ÄÅ¸ââ¢ - **A compilation of valuable resources** for further
-exploration ÄÅ¸ââ. ## Installation There are options: - Platform agnostic
-installation: [Anaconda](https://github.com/wkentaro/labelme/blob/main/
-#anaconda) - Platform specific installation: [Ubuntu](https://github.com/
-wkentaro/labelme/blob/main/#ubuntu), [macOS](https://github.com/wkentaro/
-labelme/blob/main/#macos), [Windows](https://github.com/wkentaro/labelme/blob/
-main/#windows) - Pre-build binaries from [the release section](https://
-github.com/wkentaro/labelme/releases) ### Anaconda You need install [Anaconda]
-(https://www.continuum.io/downloads), then run below: ```bash # python3 conda
-create --name=labelme python=3 source activate labelme # conda install -
-c conda-forge pyside2 # conda install pyqt # pip install pyqt5 # pyqt5 can be
-installed via pip on python3 pip install labelme # or you can install
-everything by conda command # conda install labelme -c conda-forge ``` ###
-Ubuntu ```bash sudo apt-get install labelme # or sudo pip3 install labelme # or
-install standalone executable from: # https://github.com/wkentaro/labelme/
-releases ``` ### macOS ```bash brew install pyqt # maybe pyqt5 pip install
-labelme # or brew install wkentaro/labelme/labelme # command line interface #
-brew install --cask wkentaro/labelme/labelme # app # or install standalone
-executable/app from: # https://github.com/wkentaro/labelme/releases ``` ###
-Windows Install [Anaconda](https://www.continuum.io/downloads), then in an
-Anaconda Prompt run: ```bash conda create --name=labelme python=3 conda
-activate labelme pip install labelme # or install standalone executable/app
-from: # https://github.com/wkentaro/labelme/releases ``` ## Usage Run `labelme
---help` for detail. The annotations are saved as a [JSON](http://www.json.org/
-) file. ```bash labelme # just open gui # tutorial (single image example) cd
-examples/tutorial labelme apc2016_obj3.jpg # specify image file labelme
-apc2016_obj3.jpg -O apc2016_obj3.json # close window after the save labelme
-apc2016_obj3.jpg --nodata # not include image data but relative image path in
-JSON file labelme apc2016_obj3.jpg \ --labels
+interface. [examples/instance_segmentation/data_dataset_voc/JPEGImages/
+2011_000006.jpg][examples/instance_segmentation/data_dataset_voc/
+SegmentationClass/2011_000006.png][examples/instance_segmentation/
+data_dataset_voc/SegmentationClassVisualization/2011_000006.jpg][examples/
+instance_segmentation/data_dataset_voc/SegmentationObject/2011_000006.png]
+[examples/instance_segmentation/data_dataset_voc/
+SegmentationObjectVisualization/2011_000006.jpg]VOC dataset example of instance
+segmentation. [examples/semantic_segmentation/.readme/annotation.jpg][examples/
+bbox_detection/.readme/annotation.jpg][examples/classification/.readme/
+annotation_cat.jpg]Other examples (semantic segmentation, bbox detection, and
+classification). [https://user-images.githubusercontent.com/4310419/47907116-
+85667800-de82-11e8-83d0-b9f4eb33268f.gif][https://user-
+images.githubusercontent.com/4310419/47922172-57972880-deae-11e8-84f8-
+e4324a7c856a.gif][https://user-images.githubusercontent.com/14256482/46932075-
+92145f00-d080-11e8-8d09-2162070ae57c.png]Various primitives (polygon,
+rectangle, circle, line, and point). ## Features - [x] Image annotation for
+polygon, rectangle, circle, line and point. ([tutorial](examples/tutorial)) -
+[x] Image flag annotation for classification and cleaning. ([#166](https://
+github.com/wkentaro/labelme/pull/166)) - [x] Video annotation. ([video
+annotation](examples/video_annotation)) - [x] GUI customization (predefined
+labels / flags, auto-saving, label validation, etc). ([#144](https://
+github.com/wkentaro/labelme/pull/144)) - [x] Exporting VOC-format dataset for
+semantic/instance segmentation. ([semantic segmentation](examples/
+semantic_segmentation), [instance segmentation](examples/
+instance_segmentation)) - [x] Exporting COCO-format dataset for instance
+segmentation. ([instance segmentation](examples/instance_segmentation)) ##
+Starter Guide If you're new to Labelme, you can get started with [Labelme
+Starter Guide](https://labelme.gumroad.com/l/starter-guide) (FREE), which
+contains: - **Installation guides** for all platforms: Windows, macOS, and
+Linux ð» - **Step-by-step tutorials**: first annotation to editing,
+exporting, and integrating with other programs ð - **A compilation of
+valuable resources** for further exploration ð. ## Installation There are
+options: - Platform agnostic installation: [Anaconda](#anaconda) - Platform
+specific installation: [Ubuntu](#ubuntu), [macOS](#macos), [Windows](#windows)
+- Pre-build binaries from [the release section](https://github.com/wkentaro/
+labelme/releases) ### Anaconda You need install [Anaconda](https://
+www.continuum.io/downloads), then run below: ```bash # python3 conda create --
+name=labelme python=3 source activate labelme # conda install -c conda-forge
+pyside2 # conda install pyqt # pip install pyqt5 # pyqt5 can be installed via
+pip on python3 pip install labelme # or you can install everything by conda
+command # conda install labelme -c conda-forge ``` ### Ubuntu ```bash sudo apt-
+get install labelme # or sudo pip3 install labelme # or install standalone
+executable from: # https://github.com/wkentaro/labelme/releases ``` ### macOS
+```bash brew install pyqt # maybe pyqt5 pip install labelme # or brew install
+wkentaro/labelme/labelme # command line interface # brew install --cask
+wkentaro/labelme/labelme # app # or install standalone executable/app from: #
+https://github.com/wkentaro/labelme/releases ``` ### Windows Install [Anaconda]
+(https://www.continuum.io/downloads), then in an Anaconda Prompt run: ```bash
+conda create --name=labelme python=3 conda activate labelme pip install labelme
+# or install standalone executable/app from: # https://github.com/wkentaro/
+labelme/releases ``` ## Usage Run `labelme --help` for detail. The annotations
+are saved as a [JSON](http://www.json.org/) file. ```bash labelme # just open
+gui # tutorial (single image example) cd examples/tutorial labelme
+apc2016_obj3.jpg # specify image file labelme apc2016_obj3.jpg -
+O apc2016_obj3.json # close window after the save labelme apc2016_obj3.jpg --
+nodata # not include image data but relative image path in JSON file labelme
+apc2016_obj3.jpg \ --labels
 highland_6539_self_stick_notes,mead_index_cards,kong_air_dog_squeakair_tennis_ball
 # specify label list # semantic segmentation example cd examples/
 semantic_segmentation labelme data_annotated/ # Open directory to annotate all
 images in it labelme data_annotated/ --labels labels.txt # specify label list
 with a file ``` ### Command Line Arguments - `--output` specifies the location
 that annotations will be written to. If the location ends with .json, a single
 annotation will be written to this file. Only one image can be annotated if a
@@ -101,40 +79,32 @@
 made on. - The first time you run labelme, it will create a config file in
 `~/.labelmerc`. You can edit this file and the changes will be applied the next
 time that you launch labelme. If you would prefer to use a config file from
 another location, you can specify this file with the `--config` flag. - Without
 the `--nosortlabels` flag, the program will list labels in alphabetical order.
 When the program is run with this flag, it will display labels in the order
 that they are provided. - Flags are assigned to an entire image. [Example]
-(https://github.com/wkentaro/labelme/blob/main/examples/
-classification?raw=true) - Labels are assigned to a single polygon. [Example]
-(https://github.com/wkentaro/labelme/blob/main/examples/
-bbox_detection?raw=true) ### FAQ - **How to convert JSON file to numpy array?**
-See [examples/tutorial](https://github.com/wkentaro/labelme/blob/main/examples/
-tutorial#convert-to-dataset). - **How to load label PNG file?** See [examples/
-tutorial](https://github.com/wkentaro/labelme/blob/main/examples/tutorial#how-
-to-load-label-png-file). - **How to get annotations for semantic
-segmentation?** See [examples/semantic_segmentation](https://github.com/
-wkentaro/labelme/blob/main/examples/semantic_segmentation?raw=true). - **How to
-get annotations for instance segmentation?** See [examples/
-instance_segmentation](https://github.com/wkentaro/labelme/blob/main/examples/
-instance_segmentation?raw=true). ## Examples * [Image Classification](https://
-github.com/wkentaro/labelme/blob/main/examples/classification?raw=true) *
-[Bounding Box Detection](https://github.com/wkentaro/labelme/blob/main/
-examples/bbox_detection?raw=true) * [Semantic Segmentation](https://github.com/
-wkentaro/labelme/blob/main/examples/semantic_segmentation?raw=true) * [Instance
-Segmentation](https://github.com/wkentaro/labelme/blob/main/examples/
-instance_segmentation?raw=true) * [Video Annotation](https://github.com/
-wkentaro/labelme/blob/main/examples/video_annotation?raw=true) ## How to
-develop ```bash git clone https://github.com/wkentaro/labelme.git cd labelme #
-Install anaconda3 and labelme curl -L https://github.com/wkentaro/dotfiles/raw/
-main/local/bin/install_anaconda3.sh | bash -s . source .anaconda3/bin/activate
-pip install -e . ``` ### How to build standalone executable Below shows how to
-build the standalone executable on macOS, Linux and Windows. ```bash # Setup
-conda conda create --name labelme python=3.9 conda activate labelme # Build the
-standalone executable pip install . pip install 'matplotlib<3.3' pip install
-pyinstaller pyinstaller labelme.spec dist/labelme --version ``` ### How to
-contribute Make sure below test passes on your environment. See `.github/
-workflows/ci.yml` for more detail. ```bash pip install -r requirements-dev.txt
-ruff format --check # `ruff format` to auto-fix ruff check # `ruff check --fix`
-to auto-fix MPLBACKEND='agg' pytest -vsx tests/ ``` ## Acknowledgement This
-repo is the fork of [mpitid/pylabelme](https://github.com/mpitid/pylabelme).
+(examples/classification) - Labels are assigned to a single polygon. [Example]
+(examples/bbox_detection) ### FAQ - **How to convert JSON file to numpy
+array?** See [examples/tutorial](examples/tutorial#convert-to-dataset). - **How
+to load label PNG file?** See [examples/tutorial](examples/tutorial#how-to-
+load-label-png-file). - **How to get annotations for semantic segmentation?**
+See [examples/semantic_segmentation](examples/semantic_segmentation). - **How
+to get annotations for instance segmentation?** See [examples/
+instance_segmentation](examples/instance_segmentation). ## Examples * [Image
+Classification](examples/classification) * [Bounding Box Detection](examples/
+bbox_detection) * [Semantic Segmentation](examples/semantic_segmentation) *
+[Instance Segmentation](examples/instance_segmentation) * [Video Annotation]
+(examples/video_annotation) ## How to develop ```bash git clone https://
+github.com/wkentaro/labelme.git cd labelme # Install anaconda3 and labelme curl
+-L https://github.com/wkentaro/dotfiles/raw/main/local/bin/install_anaconda3.sh
+| bash -s . source .anaconda3/bin/activate pip install -e . ``` ### How to
+build standalone executable Below shows how to build the standalone executable
+on macOS, Linux and Windows. ```bash # Setup conda conda create --name labelme
+python=3.9 conda activate labelme # Build the standalone executable pip install
+. pip install 'matplotlib<3.3' pip install pyinstaller pyinstaller labelme.spec
+dist/labelme --version ``` ### How to contribute Make sure below test passes on
+your environment. See `.github/workflows/ci.yml` for more detail. ```bash pip
+install -r requirements-dev.txt ruff format --check # `ruff format` to auto-fix
+ruff check # `ruff check --fix` to auto-fix MPLBACKEND='agg' pytest -vsx tests/
+``` ## Acknowledgement This repo is the fork of [mpitid/pylabelme](https://
+github.com/mpitid/pylabelme).
```

### Comparing `labelme-ytu-5.4.1/labelme/__init__.py` & `labelme-ytu-5.5.1/labelme/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __appname__ = "labelme-ytu"
 
 # Semantic Versioning 2.0.0: https://semver.org/
 # 1. MAJOR version when you make incompatible API changes;
 # 2. MINOR version when you add functionality in a backwards-compatible manner;
 # 3. PATCH version when you make backwards-compatible bug fixes.
 # e.g., 1.0.0a0, 1.0.0a1, 1.0.0b0, 1.0.0rc0, 1.0.0, 1.0.0.post0
-__version__ = "5.4.1"
+__version__ = "5.5.1"
 
 QT4 = QT_VERSION[0] == "4"
 QT5 = QT_VERSION[0] == "5"
 del QT_VERSION
 
 PY2 = sys.version[0] == "2"
 PY3 = sys.version[0] == "3"
```

### Comparing `labelme-ytu-5.4.1/labelme/__main__.py` & `labelme-ytu-5.5.1/labelme/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,26 @@
-print("Main starting point.")
-
 import argparse
 import codecs
 import logging
 import os
 import os.path as osp
 import sys
-import time
-
-print("Python packages loaded in main. Duration = Unknown")
-begin = time.time()
 
 import yaml
 from qtpy import QtCore
 from qtpy import QtWidgets
 
-print("Qt Packages loaded in main. Duration = %f", time.time() - begin)
-begin = time.time()
-
 from labelme import __appname__
 from labelme import __version__
 from labelme.app import MainWindow
 from labelme.config import get_config
 from labelme.logger import logger
 from labelme.utils import newIcon
 
+
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("--version", "-V", action="store_true", help="show version")
     parser.add_argument("--reset-config", action="store_true", help="reset qt config")
     parser.add_argument(
         "--logger-level",
         default="debug",
```

### Comparing `labelme-ytu-5.4.1/labelme/ai/__init__.py` & `labelme-ytu-5.5.1/labelme/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/ai/_utils.py` & `labelme-ytu-5.5.1/labelme/ai/_utils.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/ai/efficient_sam.py` & `labelme-ytu-5.5.1/labelme/ai/efficient_sam.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/ai/segment_anything_model.py` & `labelme-ytu-5.5.1/labelme/ai/segment_anything_model.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/ai/yolo.py` & `labelme-ytu-5.5.1/labelme/ai/yolo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import os
 from os.path import exists
 from urllib.parse import urlparse
 
 from labelme.widgets import ErrorDialog
 
-import sys 
+import sys
 
 #ultralytics gives error if stdout is None
-if(sys.stdout is None):
+if sys.stdout is None:
     f = open(os.devnull, 'w')
     sys.stdout = f
 
-from ultralytics import YOLO
-
 class Yolo:
     model_path = ""
 
     def __init__(self, model_path):
         self.model_path = model_path
 
     @staticmethod
@@ -29,19 +27,28 @@
     def getFileName(path):
         return os.path.basename(path)
 
     def setModel(self, path):
         self.model_path = path
 
     def getResults(self, image_paths):
-        
-        if(not self.model_path.lower().endswith(".pt")):
+        if not self.model_path.lower().endswith(".pt"):
             msgBox = ErrorDialog("Could not run the model.\nCheck model path in AI -> Object Detection Model.")
             msgBox.show()
             return None
         
-        model = YOLO(self.model_path)
-        return model(image_paths)
+        # Lazy load YOLO only when this method is called
+        try:
+            import importlib
+            ultralytics = importlib.import_module('ultralytics')
+            YOLO = getattr(ultralytics, 'YOLO')
+            model = YOLO(self.model_path)
+            return model(image_paths)
+        except (ImportError, AttributeError) as e:
+            msgBox = ErrorDialog(f"Error loading YOLO model: {e}")
+            msgBox.show()
+            return None
+
```

### Comparing `labelme-ytu-5.4.1/labelme/app.py` & `labelme-ytu-5.5.1/labelme/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,47 @@
 # -*- coding: utf-8 -*-
-print("App start point")
 
 import functools
 import html
 import math
 import os
 import os.path as osp
 import re
 import webbrowser
 import time
 
-print("Python packages loaded. Duration = Unknown")
-begin = time.time()
-
+import cv2
 import imgviz
 import natsort
 from qtpy import QtCore
 from qtpy import QtGui
 from qtpy import QtWidgets
 from qtpy.QtCore import Qt
 
-print("Qt Packages loaded. Duration = %f", time.time() - begin)
-begin = time.time()
-
 from labelme import PY2
 from labelme import __appname__
-
-print("Basic labelme packages loaded. Duration = %f", time.time() - begin)
-begin = time.time()
-
+from labelme.ai import MODELS
+from labelme.ai.yolo import Yolo
 from labelme.config import get_config
 from labelme.label_file import LabelFile
 from labelme.label_file import LabelFileError
 from labelme.logger import logger
 from labelme.shape import Shape
 from labelme.widgets import BrightnessContrastDialog
 from labelme.widgets import Canvas
 from labelme.widgets import FileDialogPreview
 from labelme.widgets import LabelDialog
 from labelme.widgets import ErrorDialog
+from labelme.widgets import DirectorySelector
 from labelme.widgets import LabelListWidget
 from labelme.widgets import LabelListWidgetItem
 from labelme.widgets import ToolBar
 from labelme.widgets import UniqueLabelQListWidget
 from labelme.widgets import ZoomWidget
 
-print("Other labelme packages loaded. Duration = %f", time.time() - begin)
-begin = time.time()
-
 from . import utils
 
 # FIXME
 # - [medium] Set max zoom value to something big enough for FitWidth/Window
 
 # TODO(unknown):
 # - Zoom is too "steppy".
@@ -158,14 +148,16 @@
         self.label_dock.setWidget(self.uniqLabelList)
 
         self.fileSearch = QtWidgets.QLineEdit()
         self.fileSearch.setPlaceholderText(self.tr("Search Filename"))
         self.fileSearch.textChanged.connect(self.fileSearchChanged)
         self.fileListWidget = QtWidgets.QListWidget()
         self.fileListWidget.itemSelectionChanged.connect(self.fileSelectionChanged)
+        self.fileListWidget.model().rowsInserted.connect(lambda: self.fileListChanged())
+        self.fileListWidget.model().rowsRemoved.connect(lambda: self.fileListChanged())
         fileListLayout = QtWidgets.QVBoxLayout()
         fileListLayout.setContentsMargins(0, 0, 0, 0)
         fileListLayout.setSpacing(0)
         fileListLayout.addWidget(self.fileSearch)
         fileListLayout.addWidget(self.fileListWidget)
         self.file_dock = QtWidgets.QDockWidget(self.tr("File List"), self)
         self.file_dock.setObjectName("Files")
@@ -183,14 +175,15 @@
             crosshair=self._config["canvas"]["crosshair"],
         )
         self.canvas.zoomRequest.connect(self.zoomRequest)
 
         scrollArea = QtWidgets.QScrollArea()
         scrollArea.setWidget(self.canvas)
         scrollArea.setWidgetResizable(True)
+        scrollArea.setStyleSheet("background-image: url(./labelme/icons/yildiz.png);background-repeat: no-repeat; background-position: center;")
         self.scrollBars = {
             Qt.Vertical: scrollArea.verticalScrollBar(),
             Qt.Horizontal: scrollArea.horizontalScrollBar(),
         }
         self.canvas.scrollRequest.connect(self.scrollRequest)
 
         self.canvas.newShape.connect(self.newShape)
@@ -237,28 +230,34 @@
         opendir = action(
             self.tr("Open Dir"),
             self.openDirDialog,
             shortcuts["open_dir"],
             "open",
             self.tr("Open Dir"),
         )
+        extractFrames = action(
+            self.tr("Extract Frames"),
+            self.extractFramesDialog,
+            "open",
+            self.tr("Extract frames of a video to a directory"),
+        )
         openNextImg = action(
             self.tr("&Next Image"),
             self.openNextImg,
             shortcuts["open_next"],
             "next",
-            self.tr("Open next (hold Ctl+Shift to copy labels)"),
+            self.tr("Open next (hold Shift to copy labels)"),
             enabled=False,
         )
         openPrevImg = action(
             self.tr("&Prev Image"),
             self.openPrevImg,
             shortcuts["open_prev"],
             "prev",
-            self.tr("Open prev (hold Ctl+Shift to copy labels)"),
+            self.tr("Open prev (hold Shift to copy labels)"),
             enabled=False,
         )
         save = action(
             self.tr("&Save\n"),
             self.saveFile,
             shortcuts["save"],
             "save",
@@ -418,14 +417,22 @@
             self.tr("Delete Polygons"),
             self.deleteSelectedShape,
             shortcuts["delete_polygon"],
             "cancel",
             self.tr("Delete the selected polygons"),
             enabled=False,
         )
+        deleteAll = action(
+            self.tr("Delete All Polygons"),
+            self.deleteAllShapes,
+            shortcuts["delete_all"],
+            "delete",
+            self.tr("Delete all polygons in image (Shift+Delete)"),
+            enabled=False
+        )
         duplicate = action(
             self.tr("Duplicate Polygons"),
             self.duplicateSelectedShape,
             shortcuts["duplicate_polygon"],
             "copy",
             self.tr("Create a duplicate of the selected polygons"),
             enabled=False,
@@ -507,14 +514,21 @@
         objectDetectionModel = action(
             self.tr("&Object Detection Model"),
             self.selectObjModel,
             icon="ai",
             tip=self.tr("Select a model for object detection"),
         )
 
+        fillGapVideo = action(
+            self.tr("&Fill Video Gaps"),
+            self.fillGapVideo,
+            tip=self.tr("Fill gaps in video between two non-empty frames(only for labels with same ID numbers)"),
+            enabled=False,
+        )
+
         zoom = QtWidgets.QWidgetAction(self)
         zoomBoxLayout = QtWidgets.QVBoxLayout()
         zoomLabel = QtWidgets.QLabel("Zoom")
         zoomLabel.setAlignment(Qt.AlignCenter)
         zoomBoxLayout.addWidget(zoomLabel)
         zoomBoxLayout.addWidget(self.zoomWidget)
         zoom.setDefaultWidget(QtWidgets.QWidget())
@@ -645,14 +659,15 @@
             save=save,
             saveAs=saveAs,
             open=open_,
             close=close,
             deleteFile=deleteFile,
             toggleKeepPrevMode=toggle_keep_prev_mode,
             delete=delete,
+            deleteAll=deleteAll,
             edit=edit,
             duplicate=duplicate,
             copy=copy,
             paste=paste,
             undoLastPoint=undoLastPoint,
             undo=undo,
             removePoint=removePoint,
@@ -672,29 +687,33 @@
             keepPrevScale=keepPrevScale,
             fitWindow=fitWindow,
             fitWidth=fitWidth,
             brightnessContrast=brightnessContrast,
             zoomActions=zoomActions,
             openNextImg=openNextImg,
             openPrevImg=openPrevImg,
-            fileMenuActions=(open_, opendir, save, saveAs, close, quit),
+            fillGapVideo=fillGapVideo,
+            fileMenuActions=(open_, opendir, extractFrames, save, saveAs, close, quit),
             tool=(),
             # XXX: need to add some actions here to activate the shortcut
             editMenu=(
                 edit,
                 duplicate,
                 copy,
                 paste,
                 delete,
+                deleteAll,
                 None,
                 undo,
                 undoLastPoint,
                 None,
                 removePoint,
                 None,
+                fillGapVideo,
+                None,
                 toggle_keep_prev_mode,
             ),
             # menu shown at right click
             menu=(
                 createMode,
                 createRectangleMode,
                 createCircleMode,
@@ -722,15 +741,16 @@
                 createPointMode,
                 createLineStripMode,
                 createAiPolygonMode,
                 createAiMaskMode,
                 editMode,
                 brightnessContrast,
             ),
-            onShapesPresent=(saveAs, hideAll, showAll, toggleAll),
+            onShapesPresent=(saveAs, hideAll, showAll, toggleAll, deleteAll),
+            onVideoOpened=(fillGapVideo,),
         )
 
         self.canvas.vertexSelected.connect(self.actions.removePoint.setEnabled)
 
         self.menus = utils.struct(
             file=self.menu(self.tr("&File")),
             edit=self.menu(self.tr("&Edit")),
@@ -744,14 +764,15 @@
         utils.addActions(
             self.menus.file,
             (
                 open_,
                 openNextImg,
                 openPrevImg,
                 opendir,
+                extractFrames,
                 self.menus.recentFiles,
                 save,
                 saveAs,
                 saveAuto,
                 changeOutputDir,
                 saveWithImageData,
                 close,
@@ -837,14 +858,18 @@
             ),
         )
 
         runYolo = QtWidgets.QWidgetAction(self)
         runYolo.setDefaultWidget(QtWidgets.QWidget())
         runYolo.defaultWidget().setLayout(QtWidgets.QVBoxLayout())
         #
+        _warningLabel = QtWidgets.QLabel(self.tr("Warning: These methods will overwrite the existing labels!"))
+        _warningLabel.setAlignment(QtCore.Qt.AlignCenter)
+        runYolo.defaultWidget().layout().addWidget(_warningLabel)
+
         modelName = "No Model"
         if(self.model_path):
            modelName = Yolo.getFileName(self.model_path) 
         self.runYoloLabel = QtWidgets.QLabel(modelName)
         self.runYoloLabel.setAlignment(QtCore.Qt.AlignCenter)
         runYolo.defaultWidget().layout().addWidget(self.runYoloLabel)
 
@@ -861,18 +886,19 @@
             open_,
             opendir,
             openPrevImg,
             openNextImg,
             save,
             deleteFile,
             None,
-            createMode,
+            createRectangleMode,
             editMode,
             duplicate,
             delete,
+            deleteAll,
             undo,
             brightnessContrast,
             None,
             fitWindow,
             zoom,
             None,
             runYolo,
@@ -948,15 +974,18 @@
     def menu(self, title, actions=None):
         menu = self.menuBar().addMenu(title)
         if actions:
             utils.addActions(menu, actions)
         return menu
 
     def runYolo(self):
-        if(self.imagePath is None or not self.imagePath.lower().endswith((".png", ".jpg", "jpeg"))):
+        if(self.imagePath is None or not self.imagePath.lower().endswith(tuple([
+                ".{}".format(fmt.data().decode())
+                for fmt in QtGui.QImageReader.supportedImageFormats()
+            ]))):
             self.errorDialogue.setText("No Image found!")
             self.errorDialogue.show()
             return
 
         model = Yolo(self.model_path)
 
         results = model.getResults(self.imagePath)
@@ -979,29 +1008,43 @@
                     shape_type="rectangle",
                     description=None,
                     ))
 
                     pred_shapes[-1].addPoint(qpoint_list[0])
                     pred_shapes[-1].addPoint(qpoint_list[1])
                     i += 1
-                
-                self.loadShapes(pred_shapes,replace=False)
-    
+
+                self.loadShapes(pred_shapes,replace=True)
+
     def runYoloVid(self):
+        # the real code is above
+        if not (self.model_path and self.model_path.split(".")[-1] == "pt"):
+            self.errorDialogue.setText(self.tr("Model cannot found!"))
+            self.errorDialogue.show()
+            return
+
+        if(self.fileListWidget.count() <= 0):
+            self.errorDialogue.setText(self.tr("No frame found!"))
+            self.errorDialogue.show()
+            return
+
         progress = QtWidgets.QProgressDialog("Running Model on Video", "Cancel", 0, self.fileListWidget.count(), self)
         progress.setWindowModality(Qt.WindowModal)
 
         for i in range(self.fileListWidget.count()):
             progress.setValue(i)
 
             if progress.wasCanceled():
                 break
 
-            self.runYoloJson(self.fileListWidget.item(i).text())
-    
+            self.loadFile(self.fileListWidget.item(i).text())
+            self.runYolo()
+            self.saveFileAuto()
+            time.sleep(2)
+
         progress.setValue(self.fileListWidget.count())
 
     def runYoloJson(self,path):
 
         def format_shape(s):
             data = s.other_data.copy()
             data.update(
@@ -1012,15 +1055,15 @@
                     description=s.description,
                     shape_type=s.shape_type,
                     flags=s.flags,
                     mask=None if s.mask is None else utils.img_arr_to_b64(s.mask),
                 )
             )
             return data
-        
+
         model = Yolo(self.model_path)
 
         results = model.getResults(path)
         if results is None:
             return
         for result in results:
             if len(result.boxes.xyxy) > 0:
@@ -1039,20 +1082,20 @@
                     shape_type="rectangle",
                     description=None,
                     ))
 
                     pred_shapes[-1].addPoint(qpoint_list[0])
                     pred_shapes[-1].addPoint(qpoint_list[1])
                     i += 1
-                
+
                 lf = LabelFile()
 
                 imagefile = QtGui.QImage(path)
                 jsonfile = os.path.splitext(path)[0] + ".json"
-                
+
                 lf.change_and_save(
                     filename=jsonfile,
                     shapes=[format_shape(shape) for shape in pred_shapes],
                     imagePath=path,
                     imageHeight=imagefile.height(),
                     imageWidth=imagefile.width(),
                 )
@@ -1173,25 +1216,78 @@
     def undoShapeEdit(self):
         self.canvas.restoreShape()
         self.labelList.clear()
         self.loadShapes(self.canvas.shapes)
         self.actions.undo.setEnabled(self.canvas.isShapeRestorable)
 
     def tutorial(self):
-        url = "https://github.com/wkentaro/labelme/tree/main/examples/tutorial"  # NOQA
+   
         webbrowser.open(url)
 
+    def fillGapVideo(self):
+        if len(self.labelList) == 0:
+            self.errorDialogue.setText(self.tr("No annotation found in current image!"))
+            self.errorDialogue.show()
+            return
+        if self.fileListWidget.currentRow() - 1 < 0:
+            self.errorDialogue.setText(self.tr("No previous frame found!"))
+            self.errorDialogue.show()
+            return
+        
+        all_shapes = []
+        images = []
+        is_last = False
+        start_file = self.fileListWidget.currentItem().text()
+
+        all_shapes.append(self.canvas.shapes)
+        im = self.fileListWidget.item(self.fileListWidget.currentRow() - 1)
+        while im is not None:
+            self.loadFile(im.text())
+            if len(self.labelList) > 0:
+                all_shapes.append(self.canvas.shapes)
+                is_last = True
+                break
+            images.append(im)
+            im = self.fileListWidget.item(self.fileListWidget.currentRow() - 1)
+
+        if not is_last:
+            self.errorDialogue.setText(self.tr("No previous annotated frame found!"))
+            self.errorDialogue.show()
+            return
+        
+        for i in reversed(range(len(images))):
+            self.loadFile(images[i].text())
+            new_shapes = []
+            for shape1 in all_shapes[0]:
+                for shape2 in all_shapes[1]:
+                    if shape1.group_id == shape2.group_id:
+                        new_shape = shape1.copy()
+                        
+                        x_p0 = shape1.points[0].x() - (shape1.points[0].x() - shape2.points[0].x())*(i + 1)/(len(images) + 1)
+                        y_p0 = shape1.points[0].y() - (shape1.points[0].y() - shape2.points[0].y())*(i + 1)/(len(images) + 1)
+                        x_p1 = shape1.points[1].x() - (shape1.points[1].x() - shape2.points[1].x())*(i + 1)/(len(images) + 1)
+                        y_p1 = shape1.points[1].y() - (shape1.points[1].y() - shape2.points[1].y())*(i + 1)/(len(images) + 1)
+                        first_point = QtCore.QPointF(x_p0, y_p0)
+                        second_point = QtCore.QPointF(x_p1, y_p1)
+                        print(first_point, second_point)
+
+                        new_shape.points = [first_point, second_point]
+                        new_shapes.append(new_shape)
+            self.loadShapes(new_shapes, replace=True)
+            self.saveFileAuto()
+            self.loadFile(start_file)
+
     def selectObjModel(self):
         model_path = QtWidgets.QFileDialog.getOpenFileName(self,
                                                            self.tr("Open File"),
                                                            ".",
                                                            self.tr("Model Files (*.pt)"))
         self.model_path = model_path[0]
         self.runYoloLabel.setText(Yolo.getUniqueName(model_path[0]))
-        
+
 
 
     def toggleDrawingSensitive(self, drawing=True):
         """Toggle drawing sensitive.
 
         In the middle of drawing, toggling between modes should be disabled.
         """
@@ -1311,28 +1407,36 @@
         self.importDirImages(
             self.lastOpenDir,
             pattern=self.fileSearch.text(),
             load=False,
         )
 
     def fileSelectionChanged(self):
+        if self.filename and not self.image.isNull():
+            self.saveFile()
+
         items = self.fileListWidget.selectedItems()
         if not items:
             return
         item = items[0]
 
-        if not self.mayContinue():
-            return
-
         currIndex = self.imageList.index(str(item.text()))
         if currIndex < len(self.imageList):
             filename = self.imageList[currIndex]
             if filename:
                 self.loadFile(filename)
 
+    def fileListChanged(self):
+        if self.fileListWidget.count() == 0:
+            for action in self.actions.onVideoOpened:
+                action.setEnabled(False)
+        else:
+            for action in self.actions.onVideoOpened:
+                action.setEnabled(True)
+
     # React to canvas signals.
     def shapeSelectionChanged(self, selected_shapes):
         self._noSelectionSlot = True
         for shape in self.canvas.selectedShapes:
             shape.selected = False
         self.labelList.clearSelection()
         self.canvas.selectedShapes = selected_shapes
@@ -1891,48 +1995,48 @@
     def loadRecent(self, filename):
         if self.mayContinue():
             self.loadFile(filename)
 
     def openPrevImg(self, _value=False):
         keep_prev = self._config["keep_prev"]
         if QtWidgets.QApplication.keyboardModifiers() == (
-            Qt.ControlModifier | Qt.ShiftModifier
+            Qt.ShiftModifier
         ):
             self._config["keep_prev"] = True
 
-        if not self.mayContinue():
-            return
-
         if len(self.imageList) <= 0:
             return
 
+        if self.filename and self.dirty:
+            self._saveFile(self.filename.split(".")[0] + ".json")
+
         if self.filename is None:
             return
 
         currIndex = self.imageList.index(self.filename)
         if currIndex - 1 >= 0:
             filename = self.imageList[currIndex - 1]
             if filename:
                 self.loadFile(filename)
 
         self._config["keep_prev"] = keep_prev
 
     def openNextImg(self, _value=False, load=True):
         keep_prev = self._config["keep_prev"]
         if QtWidgets.QApplication.keyboardModifiers() == (
-            Qt.ControlModifier | Qt.ShiftModifier
+            Qt.ShiftModifier
         ):
             self._config["keep_prev"] = True
 
-        if not self.mayContinue():
-            return
-
         if len(self.imageList) <= 0:
             return
 
+        if self.filename and self.dirty :
+            self._saveFile(self.filename.split(".")[0] + ".json")
+
         filename = None
         if self.filename is None:
             filename = self.imageList[0]
         else:
             currIndex = self.imageList.index(self.filename)
             if currIndex + 1 < len(self.imageList):
                 filename = self.imageList[currIndex + 1]
@@ -1942,16 +2046,14 @@
 
         if self.filename and load:
             self.loadFile(self.filename)
 
         self._config["keep_prev"] = keep_prev
 
     def openFile(self, _value=False):
-        if not self.mayContinue():
-            return
         path = osp.dirname(str(self.filename)) if self.filename else "."
         formats = [
             "*.{}".format(fmt.data().decode())
             for fmt in QtGui.QImageReader.supportedImageFormats()
         ]
         filters = self.tr("Image & Label files (%s)") % " ".join(
             formats + ["*%s" % LabelFile.suffix]
@@ -2002,22 +2104,33 @@
         if current_filename in self.imageList:
             # retain currently selected file
             self.fileListWidget.setCurrentRow(self.imageList.index(current_filename))
             self.fileListWidget.repaint()
 
     def saveFile(self, _value=False):
         assert not self.image.isNull(), "cannot save empty image"
+        print(self.labelFile)
         if self.labelFile:
             # DL20180323 - overwrite when in directory
             self._saveFile(self.labelFile.filename)
         elif self.output_file:
             self._saveFile(self.output_file)
             self.close()
         else:
-            self._saveFile(self.saveFileDialog())
+            self._saveFile(self.filename.split(".")[0] + ".json")
+
+    def saveFileAuto(self, _value=False):
+        assert not self.image.isNull(), "cannot save empty image"
+        if self.labelFile:
+            self._saveFile(self.labelFile.filename)
+        elif self.output_file:
+            self._saveFile(self.output_file)
+            self.close()
+        else:
+            self._saveFile(self.filename.split(".")[0] + ".json")
 
     def saveFileAs(self, _value=False):
         assert not self.image.isNull(), "cannot save empty image"
         self._saveFile(self.saveFileDialog())
 
     def saveFileDialog(self):
         caption = self.tr("%s - Choose File") % __appname__
@@ -2060,14 +2173,16 @@
         self.resetState()
         self.setClean()
         self.toggleActions(False)
         self.canvas.setEnabled(False)
         self.actions.saveAs.setEnabled(False)
 
     def getLabelFile(self):
+        if self.filename is None:
+            return None
         if self.filename.lower().endswith(".json"):
             label_file = self.filename
         else:
             label_file = osp.splitext(self.filename)[0] + ".json"
 
         return label_file
 
@@ -2159,14 +2274,28 @@
         ):
             self.remLabels(self.canvas.deleteSelected())
             self.setDirty()
             if self.noShapes():
                 for action in self.actions.onShapesPresent:
                     action.setEnabled(False)
 
+    def deleteAllShapes(self):
+        yes, no = QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No
+        msg = self.tr(
+            "You are about to permanently delete polygons, " "proceed anyway?"
+        )
+        if yes == QtWidgets.QMessageBox.warning(
+            self, self.tr("Attention"), msg, yes | no, yes
+        ):
+            self.remLabels(self.canvas.deleteAllShapes())
+            self.setDirty()
+            if self.noShapes():
+                for action in self.actions.onShapesPresent:
+                    action.setEnabled(False)
+
     def copyShape(self):
         self.canvas.endMove(copy=True)
         for shape in self.canvas.selectedShapes:
             self.addLabel(shape)
         self.labelList.clearSelection()
         self.setDirty()
 
@@ -2191,14 +2320,104 @@
                 defaultOpenDirPath,
                 QtWidgets.QFileDialog.ShowDirsOnly
                 | QtWidgets.QFileDialog.DontResolveSymlinks,
             )
         )
         self.importDirImages(targetDirPath)
 
+    @QtCore.Slot()
+    def extractVideo(self, videopath, dirpath, framerate):
+        if not os.path.exists(dirpath):
+            os.makedirs(dirpath)
+
+        cap = cv2.VideoCapture(videopath)
+        if not cap.isOpened():
+            print("Error: Could not open video file.")
+            return
+
+        fps = cap.get(cv2.CAP_PROP_FPS)
+
+        # Calculate frame interval based on desired framerate
+        frame_interval = int(round(fps / framerate))
+
+        total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+        frame_count = 0
+        frame_num = 0
+
+        progress = QtWidgets.QProgressDialog("Extracting Video", "Cancel", 0, (int)(total_frames/frame_interval),self)
+        progress.setWindowModality(Qt.WindowModal)
+
+        # Read and save frames
+        while True:
+            ret, frame = cap.read()
+            if not ret:
+                break
+
+            if progress.wasCanceled():
+                break
+
+            # Save frame if it's within the desired frame interval
+            if frame_num % frame_interval == 0:
+                frame_filename = os.path.join(dirpath, f"frame_{frame_count}.jpg")
+                cv2.imwrite(frame_filename, frame)
+                frame_count += 1
+                progress.setValue(frame_count)
+
+            frame_num += 1
+
+        progress.setValue(int(total_frames/frame_interval))
+        cap.release()
+        msgbox = QtWidgets.QMessageBox()
+        msgbox.setText("Frames saved succesfully to %s" % dirpath)
+        msgbox.exec()
+
+    def extractFramesDialog(self):
+        path = osp.dirname(str(self.filename)) if self.filename else "."
+        formats = [
+            "*.mp4",
+            "*.mkv",
+            "*.avi",
+        ]
+        filters = self.tr("Video files (%s)") % " ".join(
+            formats
+        )
+        fileDialog = FileDialogPreview(self)
+        fileDialog.setFileMode(FileDialogPreview.ExistingFile)
+        fileDialog.setNameFilter(filters)
+        fileDialog.setWindowTitle(
+            self.tr("%s - Choose Video Files") % __appname__,
+        )
+        fileDialog.setWindowFilePath(path)
+        fileDialog.setViewMode(FileDialogPreview.Detail)
+        if fileDialog.exec_():
+            fileName = fileDialog.selectedFiles()[0]
+            if fileName:
+                videoDialog = QtWidgets.QDialog(self)
+                videoDialog.setModal(True)
+                layout = QtWidgets.QVBoxLayout(videoDialog)
+                dirpathlabel = QtWidgets.QLabel("Select output directory: ")
+                dirsel = DirectorySelector()
+                dirsel.setPath(fileName.split(".")[0])
+                frratelayout = QtWidgets.QHBoxLayout()
+                frameratelabel = QtWidgets.QLabel(self.tr("Select FPS : "))
+                frameratepicker = QtWidgets.QSpinBox()
+                frameratepicker.setRange(1,100)
+                frameratepicker.setSingleStep(1)
+                frameratepicker.setValue(5)
+                frratelayout.addWidget(frameratelabel)
+                frratelayout.addWidget(frameratepicker)
+                layout.addWidget(dirpathlabel)
+                layout.addWidget(dirsel)
+                layout.addLayout(frratelayout)
+                extbutton = QtWidgets.QPushButton("Extract")
+                extbutton.clicked.connect(lambda: self.extractVideo(fileName,dirsel.getPath(),frameratepicker.value()))
+                extbutton.clicked.connect(videoDialog.close)
+                layout.addWidget(extbutton, alignment = Qt.AlignRight)
+                videoDialog.exec()
+
     @property
     def imageList(self):
         lst = []
         for i in range(self.fileListWidget.count()):
             item = self.fileListWidget.item(i)
             lst.append(item.text())
         return lst
@@ -2272,12 +2491,7 @@
         for root, dirs, files in os.walk(folderPath):
             for file in files:
                 if file.lower().endswith(tuple(extensions)):
                     relativePath = os.path.normpath(osp.join(root, file))
                     images.append(relativePath)
         images = natsort.os_sorted(images)
         return images
-
-from labelme.ai import MODELS
-from labelme.ai.yolo import Yolo
-
-print("Labelme AI packages loaded. Duration = %f", time.time() - begin)
```

### Comparing `labelme-ytu-5.4.1/labelme/cli/draw_json.py` & `labelme-ytu-5.5.1/labelme/cli/draw_json.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/cli/draw_label_png.py` & `labelme-ytu-5.5.1/labelme/cli/draw_label_png.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/cli/export_json.py` & `labelme-ytu-5.5.1/labelme/cli/export_json.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/cli/json_to_dataset.py` & `labelme-ytu-5.5.1/labelme/cli/json_to_dataset.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/cli/on_docker.py` & `labelme-ytu-5.5.1/labelme/cli/on_docker.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/config/__init__.py` & `labelme-ytu-5.5.1/labelme/config/__init__.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/config/default_config.yaml` & `labelme-ytu-5.5.1/labelme/config/default_config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
   create_rectangle: Ctrl+R
   create_circle: null
   create_line: null
   create_point: null
   create_linestrip: null
   edit_polygon: Ctrl+J
   delete_polygon: Delete
+  delete_all: Shift+Delete
   duplicate_polygon: Ctrl+D
   copy_polygon: Ctrl+C
   paste_polygon: Ctrl+V
   undo: Ctrl+Z
   undo_last_point: Ctrl+Z
   add_point_to_edge: Ctrl+Shift+P
   edit_label: Ctrl+E
```

### Comparing `labelme-ytu-5.4.1/labelme/icons/ai.png` & `labelme-ytu-5.5.1/labelme/icons/ai.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/cancel.png` & `labelme-ytu-5.5.1/labelme/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/close.png` & `labelme-ytu-5.5.1/labelme/icons/close.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/color-line.png` & `labelme-ytu-5.5.1/labelme/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/color.png` & `labelme-ytu-5.5.1/labelme/icons/color.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/copy.png` & `labelme-ytu-5.5.1/labelme/icons/copy.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/delete.png` & `labelme-ytu-5.5.1/labelme/icons/delete.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/done.png` & `labelme-ytu-5.5.1/labelme/icons/done.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/done.svg` & `labelme-ytu-5.5.1/labelme/icons/done.svg`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/edit.png` & `labelme-ytu-5.5.1/labelme/icons/edit.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/expert.png` & `labelme-ytu-5.5.1/labelme/icons/expert.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/eye.png` & `labelme-ytu-5.5.1/labelme/icons/eye.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/feBlend-icon.png` & `labelme-ytu-5.5.1/labelme/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/file.png` & `labelme-ytu-5.5.1/labelme/icons/file.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/fit-width.png` & `labelme-ytu-5.5.1/labelme/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/fit-window.png` & `labelme-ytu-5.5.1/labelme/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/fit.png` & `labelme-ytu-5.5.1/labelme/icons/fit.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/help.png` & `labelme-ytu-5.5.1/labelme/icons/help.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/labels.png` & `labelme-ytu-5.5.1/labelme/icons/labels.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/labels.svg` & `labelme-ytu-5.5.1/labelme/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/new.png` & `labelme-ytu-5.5.1/labelme/icons/new.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/next.png` & `labelme-ytu-5.5.1/labelme/icons/next.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/objects.png` & `labelme-ytu-5.5.1/labelme/icons/objects.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/open.png` & `labelme-ytu-5.5.1/labelme/icons/open.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/open.svg` & `labelme-ytu-5.5.1/labelme/icons/open.svg`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/prev.png` & `labelme-ytu-5.5.1/labelme/icons/prev.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/quit.png` & `labelme-ytu-5.5.1/labelme/icons/quit.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/save-as.png` & `labelme-ytu-5.5.1/labelme/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/save-as.svg` & `labelme-ytu-5.5.1/labelme/icons/save-as.svg`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/save.png` & `labelme-ytu-5.5.1/labelme/icons/save.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/save.svg` & `labelme-ytu-5.5.1/labelme/icons/save.svg`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/undo-cross.png` & `labelme-ytu-5.5.1/labelme/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/undo.png` & `labelme-ytu-5.5.1/labelme/icons/undo.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/zoom-in.png` & `labelme-ytu-5.5.1/labelme/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/zoom-out.png` & `labelme-ytu-5.5.1/labelme/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/icons/zoom.png` & `labelme-ytu-5.5.1/labelme/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/label_file.py` & `labelme-ytu-5.5.1/labelme/label_file.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/logger.py` & `labelme-ytu-5.5.1/labelme/logger.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/shape.py` & `labelme-ytu-5.5.1/labelme/shape.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/testing.py` & `labelme-ytu-5.5.1/labelme/testing.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/translate/empty.ts` & `labelme-ytu-5.5.1/labelme/translate/empty.ts`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/translate/zh_CN.qm` & `labelme-ytu-5.5.1/labelme/translate/zh_CN.qm`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/translate/zh_CN.ts` & `labelme-ytu-5.5.1/labelme/translate/zh_CN.ts`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/utils/__init__.py` & `labelme-ytu-5.5.1/labelme/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/utils/_io.py` & `labelme-ytu-5.5.1/labelme/utils/_io.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/utils/image.py` & `labelme-ytu-5.5.1/labelme/utils/image.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/utils/qt.py` & `labelme-ytu-5.5.1/labelme/utils/qt.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/utils/shape.py` & `labelme-ytu-5.5.1/labelme/utils/shape.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/widgets/brightness_contrast_dialog.py` & `labelme-ytu-5.5.1/labelme/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/widgets/canvas.py` & `labelme-ytu-5.5.1/labelme/widgets/canvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,14 +636,15 @@
             self.setHiding(False)
             self.selectionChanged.emit([])
             self.hShapeIsSelected = False
             self.update()
 
     def deleteSelected(self):
         deleted_shapes = []
+
         if self.selectedShapes:
             for shape in self.selectedShapes:
                 self.shapes.remove(shape)
                 deleted_shapes.append(shape)
             self.storeShapes()
             self.selectedShapes = []
             self.update()
@@ -653,14 +654,19 @@
         if shape in self.selectedShapes:
             self.selectedShapes.remove(shape)
         if shape in self.shapes:
             self.shapes.remove(shape)
         self.storeShapes()
         self.update()
 
+    def deleteAllShapes(self):
+        if self.shapes:
+            self.selectShapes(self.shapes)
+        return self.deleteSelected()
+
     def duplicateSelectedShapes(self):
         if self.selectedShapes:
             self.selectedShapesCopy = [s.copy() for s in self.selectedShapes]
             self.boundedShiftShapes(self.selectedShapesCopy)
             self.endMove(copy=True)
         return self.selectedShapes
```

### Comparing `labelme-ytu-5.4.1/labelme/widgets/color_dialog.py` & `labelme-ytu-5.5.1/labelme/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/widgets/file_dialog_preview.py` & `labelme-ytu-5.5.1/labelme/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/widgets/label_dialog.py` & `labelme-ytu-5.5.1/labelme/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/widgets/label_list_widget.py` & `labelme-ytu-5.5.1/labelme/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/widgets/tool_bar.py` & `labelme-ytu-5.5.1/labelme/widgets/tool_bar.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/widgets/unique_label_qlist_widget.py` & `labelme-ytu-5.5.1/labelme/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme/widgets/zoom_widget.py` & `labelme-ytu-5.5.1/labelme/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `labelme-ytu-5.4.1/labelme_ytu.egg-info/SOURCES.txt` & `labelme-ytu-5.5.1/labelme_ytu.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 labelme/icons/quit.png
 labelme/icons/save-as.png
 labelme/icons/save-as.svg
 labelme/icons/save.png
 labelme/icons/save.svg
 labelme/icons/undo-cross.png
 labelme/icons/undo.png
+labelme/icons/yildiz.png
 labelme/icons/zoom-in.png
 labelme/icons/zoom-out.png
 labelme/icons/zoom.png
 labelme/translate/empty.ts
 labelme/translate/zh_CN.qm
 labelme/translate/zh_CN.ts
 labelme/utils/__init__.py
@@ -69,17 +70,19 @@
 labelme/utils/image.py
 labelme/utils/qt.py
 labelme/utils/shape.py
 labelme/widgets/__init__.py
 labelme/widgets/brightness_contrast_dialog.py
 labelme/widgets/canvas.py
 labelme/widgets/color_dialog.py
+labelme/widgets/directory_selector.py
 labelme/widgets/error_dialog.py
 labelme/widgets/escapable_qlist_widget.py
 labelme/widgets/file_dialog_preview.py
+labelme/widgets/file_selector.py
 labelme/widgets/label_dialog.py
 labelme/widgets/label_list_widget.py
 labelme/widgets/tool_bar.py
 labelme/widgets/unique_label_qlist_widget.py
 labelme/widgets/zoom_widget.py
 labelme_ytu.egg-info/PKG-INFO
 labelme_ytu.egg-info/SOURCES.txt
```

### Comparing `labelme-ytu-5.4.1/setup.py` & `labelme-ytu-5.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             sys.exit(1)
 
         commands = [
             "git push origin main",
             "git tag v{:s}".format(version),
             "git push origin --tags",
             "python setup.py sdist",
-            "twine upload dist/labelme-{:s}.tar.gz".format(version),
+            "twine upload dist/labelme-ytu-{:s}.tar.gz".format(version),
         ]
         for cmd in commands:
             print("+ {:s}".format(cmd))
             subprocess.check_call(shlex.split(cmd))
         sys.exit(0)
 
     setup(
```

