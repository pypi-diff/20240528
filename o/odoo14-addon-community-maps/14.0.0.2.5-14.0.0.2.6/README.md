# Comparing `tmp/odoo14-addon-community_maps-14.0.0.2.5.tar.gz` & `tmp/odoo14-addon-community_maps-14.0.0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-community_maps-14.0.0.2.5.tar", last modified: Tue May 21 09:54:27 2024, max compression
+gzip compressed data, was "odoo14-addon-community_maps-14.0.0.2.6.tar", last modified: Tue May 28 15:05:40 2024, max compression
```

## Comparing `odoo14-addon-community_maps-14.0.0.2.5.tar` & `odoo14-addon-community_maps-14.0.0.2.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.154233 odoo14-addon-community_maps-14.0.0.2.5/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      386 2024-05-21 09:54:27.154233 odoo14-addon-community_maps-14.0.0.2.5/PKG-INFO
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.147567 odoo14-addon-community_maps-14.0.0.2.5/odoo/
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.147567 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.147567 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      116 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/__init__.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1336 2024-05-21 09:51:45.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/__manifest__.py
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.147567 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/controllers/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       80 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/controllers/__init__.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      481 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/controllers/cm_map_controller.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1304 2024-04-09 14:37:18.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/controllers/cm_submission_transfer_controller.py
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.147567 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/data/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1960 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/data/collect_place_submission_email_template.xml
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.150900 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      736 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/__init__.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1055 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_button_color_config.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      357 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_crowdfunding_notification.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1056 2024-03-04 08:15:19.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_crowdfunding_notification_request.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      466 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_external_id_mixin.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1902 2024-05-10 09:42:52.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_filter.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1328 2024-05-10 09:30:04.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_filter_group.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2913 2023-11-24 11:04:01.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_form_model.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6944 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_form_submission.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      351 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_form_submission_metadata.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4426 2024-04-09 14:16:53.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_form_submission_transfer_request.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    22223 2024-05-10 09:28:35.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_map.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1560 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_map_colorschema.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5850 2024-01-30 10:24:48.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_map_social_item.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      272 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_partner.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    36502 2024-05-10 09:58:19.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_place.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2918 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_place_category.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4141 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_place_child.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      981 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_place_external_link.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      371 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_place_presenter_metadata.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      846 2024-01-23 16:39:43.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_presenter_model.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1831 2024-04-25 12:21:08.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_slug_id_mixin.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      663 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_utils.py
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.150900 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/security/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1610 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/security/ir.model.access.csv
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3467 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/security/rules.xml
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.150900 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/services/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       64 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/services/__init__.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5156 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/services/cm_map_forms_service.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6174 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/services/cm_map_service.py
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.147567 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/static/
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.147567 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/static/src/
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.150900 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/static/src/img/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    21929 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/static/src/img/community_maps_odoo_icon.png
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.154233 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2130 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_button_color_config_id.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2593 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_filter_group.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3062 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_form_model.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5900 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_form_submission.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2374 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_form_submission_transfer_request.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     9856 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_map.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2189 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_map_colorschema.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      171 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_menu_root.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      135 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_menu_root_config.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    12868 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_place.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2197 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_place_category.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      770 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_place_presenter_metadata.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1933 2023-12-22 15:00:06.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_presenter_model.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      759 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_submission_transfer_page_template.xml
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      556 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/ir_cron_views.xml
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.154233 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/wizards/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       43 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/wizards/__init__.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3307 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.py
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1540 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.xml
-drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-21 09:54:27.154233 odoo14-addon-community_maps-14.0.0.2.5/odoo14_addon_community_maps.egg-info/
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      386 2024-05-21 09:54:27.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo14_addon_community_maps.egg-info/PKG-INFO
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3311 2024-05-21 09:54:27.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo14_addon_community_maps.egg-info/SOURCES.txt
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2024-05-21 09:54:27.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo14_addon_community_maps.egg-info/dependency_links.txt
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2023-12-05 08:53:35.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo14_addon_community_maps.egg-info/not-zip-safe
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      127 2024-05-21 09:54:27.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo14_addon_community_maps.egg-info/requires.txt
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        5 2024-05-21 09:54:27.000000 odoo14-addon-community_maps-14.0.0.2.5/odoo14_addon_community_maps.egg-info/top_level.txt
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       38 2024-05-21 09:54:27.154233 odoo14-addon-community_maps-14.0.0.2.5/setup.cfg
--rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      256 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.5/setup.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.833605 odoo14-addon-community_maps-14.0.0.2.6/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      386 2024-05-28 15:05:40.833605 odoo14-addon-community_maps-14.0.0.2.6/PKG-INFO
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      116 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1336 2024-05-28 15:02:51.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/__manifest__.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/controllers/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       80 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/controllers/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      481 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/controllers/cm_map_controller.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1304 2024-04-09 14:37:18.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/controllers/cm_submission_transfer_controller.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/data/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1960 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/data/collect_place_submission_email_template.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      736 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1055 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_button_color_config.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      357 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_crowdfunding_notification.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1056 2024-03-04 08:15:19.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_crowdfunding_notification_request.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      466 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_external_id_mixin.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1934 2024-05-28 14:46:11.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_filter.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1328 2024-05-28 14:45:45.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_filter_group.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2913 2023-11-24 11:04:01.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_form_model.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6944 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_form_submission.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      351 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_form_submission_metadata.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4426 2024-04-09 14:16:53.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_form_submission_transfer_request.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    22223 2024-05-28 14:45:45.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_map.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1560 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_map_colorschema.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5850 2024-01-30 10:24:48.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_map_social_item.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      272 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_partner.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    36502 2024-05-10 09:58:19.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_place.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2918 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_place_category.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     4141 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_place_child.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      981 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_place_external_link.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      371 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_place_presenter_metadata.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      846 2024-01-23 16:39:43.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_presenter_model.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1831 2024-05-28 14:42:15.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_slug_id_mixin.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      663 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_utils.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/security/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1610 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/security/ir.model.access.csv
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3467 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/security/rules.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/services/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       64 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/services/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5156 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/services/cm_map_forms_service.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     6174 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/services/cm_map_service.py
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/static/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/static/src/
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/static/src/img/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    21929 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/static/src/img/community_maps_odoo_icon.png
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2130 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_button_color_config_id.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2593 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_filter_group.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3062 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_form_model.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     5900 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_form_submission.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2374 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_form_submission_transfer_request.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     9856 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_map.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2189 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_map_colorschema.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      171 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_menu_root.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      135 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_menu_root_config.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)    12868 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_place.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     2197 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_place_category.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      770 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_place_presenter_metadata.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1933 2023-12-22 15:00:06.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_presenter_model.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      759 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_submission_transfer_page_template.xml
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      556 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/ir_cron_views.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.830272 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/wizards/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       43 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/wizards/__init__.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3307 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.py
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     1540 2024-03-08 17:00:07.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.xml
+drwxr-xr-x   0 daniquilez  (1000) daniquilez  (1000)        0 2024-05-28 15:05:40.833605 odoo14-addon-community_maps-14.0.0.2.6/odoo14_addon_community_maps.egg-info/
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      386 2024-05-28 15:05:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo14_addon_community_maps.egg-info/PKG-INFO
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)     3311 2024-05-28 15:05:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo14_addon_community_maps.egg-info/SOURCES.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2024-05-28 15:05:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo14_addon_community_maps.egg-info/dependency_links.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        1 2023-12-05 08:53:35.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo14_addon_community_maps.egg-info/not-zip-safe
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      127 2024-05-28 15:05:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo14_addon_community_maps.egg-info/requires.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)        5 2024-05-28 15:05:40.000000 odoo14-addon-community_maps-14.0.0.2.6/odoo14_addon_community_maps.egg-info/top_level.txt
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)       38 2024-05-28 15:05:40.833605 odoo14-addon-community_maps-14.0.0.2.6/setup.cfg
+-rw-r--r--   0 daniquilez  (1000) daniquilez  (1000)      256 2023-11-02 09:59:40.000000 odoo14-addon-community_maps-14.0.0.2.6/setup.py
```

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/__manifest__.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/__manifest__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     'summary': """
     Module to create and manage your map visualizations into a  website""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "https://gitlab.com/coopdevs/community-maps-builder-backend",
 
     'category': 'community-maps',
-    'version': '14.0.0.2.5',
+    'version': '14.0.0.2.6',
 
     'depends': [
         'base',
         'base_rest',
         'base_rest_base_structure',
         'sale',
         'crm',
```

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/controllers/cm_submission_transfer_controller.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/controllers/cm_submission_transfer_controller.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/data/collect_place_submission_email_template.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/data/collect_place_submission_email_template.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/__init__.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_button_color_config.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_button_color_config.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_crowdfunding_notification_request.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_crowdfunding_notification_request.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_filter.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from odoo import models, api, fields
 from odoo.tools.translate import _
 
 
 class CmFilter(models.Model):
     _name = "cm.filter"
-
     _inherit = ["cm.slug.id.mixin"]
+    _slug_models = ["cm.filter"]
 
     name = fields.Char(string=_("Name"), translate=True)
     icon = fields.Char(string=_("Icon"))
     color = fields.Char(string=_("Color"))
     marker_color = fields.Char(string=_("Marker main color (hex)"))
     marker_text_color = fields.Char(string=_("Marker text color (hex)"))
     marker_bg_color = fields.Char(string=_("Marker background color (hex)"))
```

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_filter_group.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_filter_group.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_form_model.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_form_model.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_form_submission.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_form_submission.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_form_submission_transfer_request.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_form_submission_transfer_request.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_map.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_map.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_map_colorschema.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_map_colorschema.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_map_social_item.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_map_social_item.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_place.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_place.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_place_category.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_place_category.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_place_child.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_place_child.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_place_external_link.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_place_external_link.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_presenter_model.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_presenter_model.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_slug_id_mixin.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_slug_id_mixin.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/models/cm_utils.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/models/cm_utils.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/security/ir.model.access.csv` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/security/rules.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/security/rules.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/services/cm_map_forms_service.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/services/cm_map_forms_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/services/cm_map_service.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/services/cm_map_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/static/src/img/community_maps_odoo_icon.png` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/static/src/img/community_maps_odoo_icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_button_color_config_id.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_button_color_config_id.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_filter_group.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_filter_group.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_form_model.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_form_model.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_form_submission.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_form_submission.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_form_submission_transfer_request.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_form_submission_transfer_request.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_map.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_map.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_map_colorschema.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_map_colorschema.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_place.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_place.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_place_category.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_place_category.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_place_presenter_metadata.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_place_presenter_metadata.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_presenter_model.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_presenter_model.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/cm_submission_transfer_page_template.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/cm_submission_transfer_page_template.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/views/ir_cron_views.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/views/ir_cron_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.py` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.xml` & `odoo14-addon-community_maps-14.0.0.2.6/odoo/addons/community_maps/wizards/cm_collectchildplaces_wizard.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-community_maps-14.0.0.2.5/odoo14_addon_community_maps.egg-info/SOURCES.txt` & `odoo14-addon-community_maps-14.0.0.2.6/odoo14_addon_community_maps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

