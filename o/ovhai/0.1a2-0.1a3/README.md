# Comparing `tmp/ovhai-0.1a2.tar.gz` & `tmp/ovhai-0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovhai-0.1a2.tar", last modified: Tue May 28 09:04:27 2024, max compression
+gzip compressed data, was "ovhai-0.1a3.tar", last modified: Tue May 28 13:41:14 2024, max compression
```

## Comparing `ovhai-0.1a2.tar` & `ovhai-0.1a3.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.476898 ovhai-0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-28 09:04:18.000000 ovhai-0.1a2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-28 09:04:18.000000 ovhai-0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 09:04:27.476898 ovhai-0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-28 09:04:18.000000 ovhai-0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.440898 ovhai-0.1a2/ovhai/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.444898 ovhai-0.1a2/ovhai/api/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.444898 ovhai-0.1a2/ovhai/api/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/app_cli_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/app_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/app_edit_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/app_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/app_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/app_stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/app_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/app_update_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/delete_v1_app_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/get_v1_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/get_v1_app_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/post_v1_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/app/post_v1_app_app_id_datasync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.448898 ovhai-0.1a2/ovhai/api/capabilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_app_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_flavor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_flavor_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_job_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_notebook_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_notebook_editor_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_notebook_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_notebook_framework_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_preset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_preset_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_quota.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.448898 ovhai-0.1a2/ovhai/api/deprecated_capabilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/deprecated_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_editor_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_framework_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.448898 ovhai-0.1a2/ovhai/api/framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/framework/delete_v1_framework_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/framework/get_v1_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/framework/get_v1_framework_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/framework/patch_v1_framework_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/framework/post_v1_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.452898 ovhai-0.1a2/ovhai/api/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/image/delete_v1_image_image_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/image/delete_v1_image_image_id_version_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/image/get_v1_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/image/get_v1_image_image_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/image/get_v1_image_image_id_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/image/get_v1_image_image_id_version_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/image/patch_v1_image_image_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/image/patch_v1_image_image_id_version_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/image/post_v1_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/image/post_v1_image_image_id_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/image/post_v1_image_image_id_version_tag_mirror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.452898 ovhai-0.1a2/ovhai/api/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/job_cli_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/job_data_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/job_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/job_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/job_edit_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/job_exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/job_get.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/job_get_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/job_kill.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/job_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/job_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/job/job_start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.452898 ovhai-0.1a2/ovhai/api/me/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/me/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/me/me.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.456898 ovhai-0.1a2/ovhai/api/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_cli_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_create_from_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_data_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_edit_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_get.py
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_get_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_get_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_list_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/notebook/notebook_stop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.456898 ovhai-0.1a2/ovhai/api/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/registry/registry_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/registry/registry_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/registry/registry_get_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/registry/registry_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/registry/registry_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.456898 ovhai-0.1a2/ovhai/api/token/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/token/token_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/token/token_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/token/token_get_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/token/token_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/token/token_renew.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.456898 ovhai-0.1a2/ovhai/api/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/volume/delete_v1_volume_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/volume/get_v1_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/volume/get_v1_volume_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/api/volume/post_v1_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.476898 ovhai-0.1a2/ovhai/models/
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/app_deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/app_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/app_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/app_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/app_spec_labels_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/app_state_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/app_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/app_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/app_update_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/app_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/automatic_scaling_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/capability_notebook_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/capability_notebook_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/cli_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/contract_terms_of_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/create_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/create_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/create_image_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/create_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/data_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/data_store_volume_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/data_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/data_sync_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/data_sync_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/data_sync_spec_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/data_sync_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/doc_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/fixed_scaling_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/flavor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/framework_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/get_v1_data_auth_alias_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/git_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/gpu_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/https_basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/image_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/image_mirror_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/image_mirror_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/image_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/image_version_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/info_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/job_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/job_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/job_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/job_spec_labels_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/job_spec_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/job_state_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    18324 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/label_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/licensing_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/me.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/me_token_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook_backup_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook_spec_labels_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook_spec_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook_spec_update_labels_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/notebook_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/partner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/preset_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/preset_partner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/preset_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/preset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/private_swift_volume_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/probe.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/product_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/project_quotas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/project_quotas_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/public_git_volume_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/public_swift_volume_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/registry_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/registry_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/resources_per_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/s3_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/scaling_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/scaling_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/ssh_key_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/standalone_volume_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/store_owner.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/store_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/terms_of_service_locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/token_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/token_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/token_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/update_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/update_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/update_image_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/user_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/volume_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/models/volume_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/ovhai_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-28 09:04:18.000000 ovhai-0.1a2/ovhai/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:04:27.444898 ovhai-0.1a2/ovhai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 09:04:27.000000 ovhai-0.1a2/ovhai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-28 09:04:27.000000 ovhai-0.1a2/ovhai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:04:27.000000 ovhai-0.1a2/ovhai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:04:27.000000 ovhai-0.1a2/ovhai.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 09:04:27.000000 ovhai-0.1a2/ovhai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 09:04:27.000000 ovhai-0.1a2/ovhai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-28 09:04:18.000000 ovhai-0.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:04:27.476898 ovhai-0.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.890796 ovhai-0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-28 13:41:03.000000 ovhai-0.1a3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-28 13:41:03.000000 ovhai-0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 13:41:14.890796 ovhai-0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-28 13:41:03.000000 ovhai-0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.854795 ovhai-0.1a3/ovhai/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.854795 ovhai-0.1a3/ovhai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.858795 ovhai-0.1a3/ovhai/api/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/app_cli_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/app_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/app_edit_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/app_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/app_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/app_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/app_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/app_update_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/delete_v1_app_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/get_v1_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/get_v1_app_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/post_v1_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/app/post_v1_app_app_id_datasync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.858795 ovhai-0.1a3/ovhai/api/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_app_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_flavor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_flavor_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_job_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_notebook_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_notebook_editor_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_notebook_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_notebook_framework_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_preset_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_quota.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.858795 ovhai-0.1a3/ovhai/api/deprecated_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/deprecated_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_editor_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_framework_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.862795 ovhai-0.1a3/ovhai/api/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/framework/delete_v1_framework_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/framework/get_v1_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/framework/get_v1_framework_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/framework/patch_v1_framework_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/framework/post_v1_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.862795 ovhai-0.1a3/ovhai/api/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/image/delete_v1_image_image_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/image/delete_v1_image_image_id_version_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/image/get_v1_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/image/get_v1_image_image_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/image/get_v1_image_image_id_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/image/get_v1_image_image_id_version_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/image/patch_v1_image_image_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/image/patch_v1_image_image_id_version_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/image/post_v1_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/image/post_v1_image_image_id_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/image/post_v1_image_image_id_version_tag_mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.866795 ovhai-0.1a3/ovhai/api/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/job_cli_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/job_data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/job_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/job_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/job_edit_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/job_exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/job_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/job_get_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/job_kill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/job_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/job_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/job/job_start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.866795 ovhai-0.1a3/ovhai/api/me/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/me/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/me/me.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.866795 ovhai-0.1a3/ovhai/api/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_cli_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_create_from_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_edit_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_get_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_get_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_list_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/notebook/notebook_stop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.870795 ovhai-0.1a3/ovhai/api/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/registry/registry_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/registry/registry_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/registry/registry_get_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/registry/registry_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/registry/registry_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.870795 ovhai-0.1a3/ovhai/api/token/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/token/token_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/token/token_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/token/token_get_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/token/token_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/token/token_renew.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.870795 ovhai-0.1a3/ovhai/api/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/volume/delete_v1_volume_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/volume/get_v1_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/volume/get_v1_volume_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/api/volume/post_v1_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.886796 ovhai-0.1a3/ovhai/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/app_deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/app_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/app_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/app_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/app_spec_labels_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/app_state_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/app_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/app_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/app_update_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/app_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/automatic_scaling_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/capability_notebook_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/capability_notebook_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/cli_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/contract_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/create_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/create_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/create_image_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/create_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/data_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/data_store_volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/data_sync_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/data_sync_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/data_sync_spec_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/data_sync_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/doc_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/fixed_scaling_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/flavor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/framework_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/get_v1_data_auth_alias_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/git_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/gpu_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/https_basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/image_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/image_mirror_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/image_mirror_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/image_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/image_version_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/info_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/job_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/job_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/job_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/job_spec_labels_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/job_spec_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/job_state_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18324 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/label_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/licensing_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/me.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/me_token_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook_backup_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook_spec_labels_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook_spec_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook_spec_update_labels_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/notebook_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/preset_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/preset_partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/preset_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/preset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/private_swift_volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/project_quotas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/project_quotas_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/public_git_volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/public_swift_volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/registry_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/registry_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/resources_per_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/s3_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/scaling_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/scaling_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/ssh_key_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/standalone_volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/store_owner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/store_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/terms_of_service_locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/token_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/token_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/token_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/update_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/update_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/update_image_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/user_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/volume_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/models/volume_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/ovhai_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-28 13:41:03.000000 ovhai-0.1a3/ovhai/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:41:14.854795 ovhai-0.1a3/ovhai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 13:41:14.000000 ovhai-0.1a3/ovhai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-28 13:41:14.000000 ovhai-0.1a3/ovhai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:41:14.000000 ovhai-0.1a3/ovhai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:41:14.000000 ovhai-0.1a3/ovhai.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 13:41:14.000000 ovhai-0.1a3/ovhai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 13:41:14.000000 ovhai-0.1a3/ovhai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-28 13:41:03.000000 ovhai-0.1a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:41:14.890796 ovhai-0.1a3/setup.cfg
```

### Comparing `ovhai-0.1a2/AUTHORS` & `ovhai-0.1a3/AUTHORS`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/LICENSE` & `ovhai-0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/README.md` & `ovhai-0.1a3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -32,43 +32,49 @@
 
 The token used to create the client can be created via the OVHcloud Control Panel (UI), from the AI Dashboard.
 
 Once your client is defined, you can call an endpoint:
 
 ```python
 from ovhai.models import Me
+from ovhai.api.me import me
 from ovhai.ovhai_types import Response
 
 with client as client:
     res: Me = me.sync(client=client)
-
+    print(res)
+    
     # or if you need more info (e.g. status_code)
-    response: Response[Me] = me.sync_detailed(client=client)
+    #response: Response[Me] = me.sync_detailed(client=client)
+    #print(response)
 ```
 
 Or do the same thing with an async version:
 
 ```python
 import asyncio
 from ovhai.models import Me
+from ovhai.api.me import me
 from ovhai.ovhai_types import Response
 
 async def main(client):
     res: Me = await me.asyncio(client=client)
-    response: Response[Me] = await me.asyncio_detailed(client=client)
-    print("res:", res)
-    print("response:", response)
+    print(res)
+    
+    # or if you need more info (e.g. status_code)
+    #response: Response[Me] = await me.asyncio_detailed(client=client)
+    #print(response)
     
 # Run the main function asynchronously
 asyncio.run(main(client=client))
 ```
 
-In the `ovhai/api` [folder](https://github.com/ovh/ovhai-python-sdk/tree/main/ovhai/api), you will find all the endpoints you can call up. They are grouped by folder according to their purpose (`notebook`, `job`, `app`). 
+In the `ovhai/api` [folder](https://github.com/ovh/ovhai-python-sdk/tree/main/ovhai/api), you will find all the endpoints you can call up. They are grouped by folder according to their purpose (`notebook`, `job`, `app`, `...`). 
 
-For example, to launch a notebook, you need to import the `notebook_new` file, located at `/ovhai/api/notebook`. You will also need to import the objects linked to this endpoint, since you will manipulate them (`Notebook` and `NotebookSpec` here). This will allow you to launch your first notebook using the `ovhai` python library, based on your specifications:
+For example, to launch a notebook, you need to import the [`notebook_new` file](https://github.com/ovh/ovhai-python-sdk/blob/master/ovhai/api/notebook/notebook_new.py), located at `/ovhai/api/notebook`. You will also need to import the objects linked to this endpoint (those mentioned in the python file), since you will manipulate them (`Notebook` and `NotebookSpec` here, in addition to the classic `AuthenticatedClient` and `Response`). This will allow you to launch your first notebook using the `ovhai` python library, based on your specifications:
 
 ```python
 from ovhai import AuthenticatedClient
 from ovhai.api.notebook import notebook_new
 from ovhai.models import NotebookSpec, Notebook
 from ovhai.ovhai_types import Response
 
@@ -102,43 +108,35 @@
 
 Every [OVHcloud's AI API](https://gra.training.ai.cloud.ovh.net/#/) endpoint has its dedicated Python module that comes with four functions:
 1. `sync`: Blocking request that returns parsed data (if successful) or `None`
 2. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.
 3. `asyncio`: Like `sync` but async instead of blocking
 4. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking
 
+To implement the call you want, find the folder and then the file corresponding to your needs in the [api folder](https://github.com/ovh/ovhai-python-sdk/tree/master/ovhai/api). Then choose the method that suits you best from the four mentioned above. Then import the objects you need to use this method.
 
 ## Advanced customizations
 
-There are more settings on the generated `Client` class which let you control more runtime behavior, check out the docstring on that class for more info. You can also customize the underlying `httpx.Client` or `httpx.AsyncClient` (depending on your use-case):
+There are more settings on the generated `AuthenticatedClient` class which let you control more runtime behavior, check out the [docstring on that class](https://github.com/ovh/ovhai-python-sdk/blob/master/ovhai/client.py) for more info. You can also customize the underlying `httpx.Client` or `httpx.AsyncClient` (depending on your use-case):
 
 ```python
-from ovhai import Client
+from ovhai import AuthenticatedClient
 
 def log_request(request):
     print(f"Request event hook: {request.method} {request.url} - Waiting for response")
 
 def log_response(response):
     request = response.request
     print(f"Response event hook: {request.method} {request.url} - Status {response.status_code}")
 
-client = Client(
+client = AuthenticatedClient(
     base_url="https://gra.training.ai.cloud.ovh.net",
     token="YOUR_AI_TOKEN",
     httpx_args={"event_hooks": {"request": [log_request], "response": [log_response]}},
 )
 
 # Or get the underlying httpx client to modify directly with client.get_httpx_client() or client.get_async_httpx_client()
 ```
 
-You can even set the httpx client directly, but beware that this will override any existing settings (e.g., base_url):
+For example, the previous code snippet shows how to define a custom request and response event hook using the `httpx_args` parameter of the `AuthenticatedClient` class. The `httpx_args` parameter is used to pass additional arguments to the underlying `httpx.Client` or `httpx.AsyncClient`. In this case, the `event_hooks` argument is used to specify custom functions that will be called before and after each HTTP request and response.
 
-```python
-import httpx
-from ovhai import Client
-
-client = Client(
-    base_url="https://gra.training.ai.cloud.ovh.net",
-)
-# Note that base_url needs to be re-set, as would any shared cookies, headers, etc.
-client.set_httpx_client(httpx.Client(base_url="https://gra.training.ai.cloud.ovh.net", proxies="http://localhost:8030"))
-```
+You can even set the httpx client directly, but beware that this will override any existing settings (e.g., `base_url`).
```

### Comparing `ovhai-0.1a2/ovhai/api/app/app_cli_command.py` & `ovhai-0.1a3/ovhai/api/app/app_cli_command.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/app/app_edit.py` & `ovhai-0.1a3/ovhai/api/app/app_edit.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/app/app_edit_label.py` & `ovhai-0.1a3/ovhai/api/app/app_edit_label.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/app/app_log.py` & `ovhai-0.1a3/ovhai/api/app/app_log.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/app/app_start.py` & `ovhai-0.1a3/ovhai/api/app/app_start.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/app/app_stop.py` & `ovhai-0.1a3/ovhai/api/app/app_stop.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/app/app_update.py` & `ovhai-0.1a3/ovhai/api/app/app_update.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/app/app_update_image.py` & `ovhai-0.1a3/ovhai/api/app/app_update_image.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/app/delete_v1_app_id.py` & `ovhai-0.1a3/ovhai/api/app/delete_v1_app_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/app/get_v1_app.py` & `ovhai-0.1a3/ovhai/api/app/get_v1_app.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/app/get_v1_app_id.py` & `ovhai-0.1a3/ovhai/api/app/get_v1_app_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/app/post_v1_app.py` & `ovhai-0.1a3/ovhai/api/app/post_v1_app.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/app/post_v1_app_app_id_datasync.py` & `ovhai-0.1a3/ovhai/api/app/post_v1_app_app_id_datasync.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_app_image.py` & `ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_app_image.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_flavor.py` & `ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_flavor.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_flavor_id.py` & `ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_flavor_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_job_image.py` & `ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_job_image.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_notebook_editor.py` & `ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_notebook_editor.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_notebook_editor_id.py` & `ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_notebook_editor_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_notebook_framework.py` & `ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_notebook_framework.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_notebook_framework_id.py` & `ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_notebook_framework_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_preset.py` & `ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_preset.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_preset_id.py` & `ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_preset_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/capabilities/get_v1_capabilities_quota.py` & `ovhai-0.1a3/ovhai/api/capabilities/get_v1_capabilities_quota.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_editor.py` & `ovhai-0.1a3/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_editor.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_editor_id.py` & `ovhai-0.1a3/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_editor_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_framework.py` & `ovhai-0.1a3/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_framework.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_framework_id.py` & `ovhai-0.1a3/ovhai/api/deprecated_capabilities/get_v1_notebook_capabilities_framework_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/framework/delete_v1_framework_id.py` & `ovhai-0.1a3/ovhai/api/framework/delete_v1_framework_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/framework/get_v1_framework.py` & `ovhai-0.1a3/ovhai/api/framework/get_v1_framework.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/framework/get_v1_framework_id.py` & `ovhai-0.1a3/ovhai/api/framework/get_v1_framework_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/framework/patch_v1_framework_id.py` & `ovhai-0.1a3/ovhai/api/framework/patch_v1_framework_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/framework/post_v1_framework.py` & `ovhai-0.1a3/ovhai/api/framework/post_v1_framework.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/image/delete_v1_image_image_id.py` & `ovhai-0.1a3/ovhai/api/image/delete_v1_image_image_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/image/delete_v1_image_image_id_version_tag.py` & `ovhai-0.1a3/ovhai/api/image/delete_v1_image_image_id_version_tag.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/image/get_v1_image.py` & `ovhai-0.1a3/ovhai/api/image/get_v1_image.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/image/get_v1_image_image_id.py` & `ovhai-0.1a3/ovhai/api/image/get_v1_image_image_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/image/get_v1_image_image_id_version.py` & `ovhai-0.1a3/ovhai/api/image/get_v1_image_image_id_version.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/image/get_v1_image_image_id_version_tag.py` & `ovhai-0.1a3/ovhai/api/image/get_v1_image_image_id_version_tag.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/image/patch_v1_image_image_id.py` & `ovhai-0.1a3/ovhai/api/image/patch_v1_image_image_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/image/patch_v1_image_image_id_version_tag.py` & `ovhai-0.1a3/ovhai/api/image/patch_v1_image_image_id_version_tag.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/image/post_v1_image.py` & `ovhai-0.1a3/ovhai/api/image/post_v1_image.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/image/post_v1_image_image_id_version.py` & `ovhai-0.1a3/ovhai/api/image/post_v1_image_image_id_version.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/image/post_v1_image_image_id_version_tag_mirror.py` & `ovhai-0.1a3/ovhai/api/image/post_v1_image_image_id_version_tag_mirror.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/job/job_cli_command.py` & `ovhai-0.1a3/ovhai/api/job/job_cli_command.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/job/job_data_sync.py` & `ovhai-0.1a3/ovhai/api/job/job_data_sync.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/job/job_delete.py` & `ovhai-0.1a3/ovhai/api/job/job_delete.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/job/job_edit.py` & `ovhai-0.1a3/ovhai/api/job/job_edit.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/job/job_edit_label.py` & `ovhai-0.1a3/ovhai/api/job/job_edit_label.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/job/job_exec.py` & `ovhai-0.1a3/ovhai/api/job/job_exec.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/job/job_get.py` & `ovhai-0.1a3/ovhai/api/job/job_get.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/job/job_get_all.py` & `ovhai-0.1a3/ovhai/api/job/job_get_all.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/job/job_kill.py` & `ovhai-0.1a3/ovhai/api/job/job_kill.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/job/job_log.py` & `ovhai-0.1a3/ovhai/api/job/job_log.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/job/job_new.py` & `ovhai-0.1a3/ovhai/api/job/job_new.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/job/job_start.py` & `ovhai-0.1a3/ovhai/api/job/job_start.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/me/me.py` & `ovhai-0.1a3/ovhai/api/me/me.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_cli_command.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_cli_command.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_create_from_backup.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_create_from_backup.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_data_sync.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_data_sync.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_delete.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_delete.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_edit.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_edit.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_edit_label.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_edit_label.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_exec.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_exec.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_get.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_get.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_get_all.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_get_all.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_get_backup.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_get_backup.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_list_backup.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_list_backup.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_new.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_new.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_start.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_start.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/notebook/notebook_stop.py` & `ovhai-0.1a3/ovhai/api/notebook/notebook_stop.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/registry/registry_delete.py` & `ovhai-0.1a3/ovhai/api/registry/registry_delete.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/registry/registry_get.py` & `ovhai-0.1a3/ovhai/api/registry/registry_get.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/registry/registry_get_all.py` & `ovhai-0.1a3/ovhai/api/registry/registry_get_all.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/registry/registry_new.py` & `ovhai-0.1a3/ovhai/api/registry/registry_new.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/registry/registry_update.py` & `ovhai-0.1a3/ovhai/api/registry/registry_update.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/token/token_delete.py` & `ovhai-0.1a3/ovhai/api/token/token_delete.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/token/token_get.py` & `ovhai-0.1a3/ovhai/api/token/token_get.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/token/token_get_all.py` & `ovhai-0.1a3/ovhai/api/token/token_get_all.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/token/token_new.py` & `ovhai-0.1a3/ovhai/api/token/token_new.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/token/token_renew.py` & `ovhai-0.1a3/ovhai/api/token/token_renew.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/volume/delete_v1_volume_id.py` & `ovhai-0.1a3/ovhai/api/volume/delete_v1_volume_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/volume/get_v1_volume.py` & `ovhai-0.1a3/ovhai/api/volume/get_v1_volume.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/volume/get_v1_volume_id.py` & `ovhai-0.1a3/ovhai/api/volume/get_v1_volume_id.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/api/volume/post_v1_volume.py` & `ovhai-0.1a3/ovhai/api/volume/post_v1_volume.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/client.py` & `ovhai-0.1a3/ovhai/client.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/errors.py` & `ovhai-0.1a3/ovhai/errors.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/__init__.py` & `ovhai-0.1a3/ovhai/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/app.py` & `ovhai-0.1a3/ovhai/models/app.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/app_deployment_strategy.py` & `ovhai-0.1a3/ovhai/models/app_deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/app_image.py` & `ovhai-0.1a3/ovhai/models/app_image.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/app_list.py` & `ovhai-0.1a3/ovhai/models/app_list.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/app_spec.py` & `ovhai-0.1a3/ovhai/models/app_spec.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/app_spec_labels_type_0.py` & `ovhai-0.1a3/ovhai/models/app_spec_labels_type_0.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/app_state_history.py` & `ovhai-0.1a3/ovhai/models/app_state_history.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/app_status.py` & `ovhai-0.1a3/ovhai/models/app_status.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/app_update.py` & `ovhai-0.1a3/ovhai/models/app_update.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/app_update_image.py` & `ovhai-0.1a3/ovhai/models/app_update_image.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/app_update_request.py` & `ovhai-0.1a3/ovhai/models/app_update_request.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/automatic_scaling_strategy.py` & `ovhai-0.1a3/ovhai/models/automatic_scaling_strategy.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/capability_notebook_editor.py` & `ovhai-0.1a3/ovhai/models/capability_notebook_editor.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/capability_notebook_framework.py` & `ovhai-0.1a3/ovhai/models/capability_notebook_framework.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/cli_command.py` & `ovhai-0.1a3/ovhai/models/cli_command.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/contract.py` & `ovhai-0.1a3/ovhai/models/contract.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/contract_terms_of_service.py` & `ovhai-0.1a3/ovhai/models/contract_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/create_framework.py` & `ovhai-0.1a3/ovhai/models/create_framework.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/create_image.py` & `ovhai-0.1a3/ovhai/models/create_image.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/create_image_version.py` & `ovhai-0.1a3/ovhai/models/create_image_version.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/create_volume.py` & `ovhai-0.1a3/ovhai/models/create_volume.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/credentials.py` & `ovhai-0.1a3/ovhai/models/credentials.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/data_store.py` & `ovhai-0.1a3/ovhai/models/data_store.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/data_store_volume_source.py` & `ovhai-0.1a3/ovhai/models/data_store_volume_source.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/data_sync.py` & `ovhai-0.1a3/ovhai/models/data_sync.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/data_sync_progress.py` & `ovhai-0.1a3/ovhai/models/data_sync_progress.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/data_sync_spec.py` & `ovhai-0.1a3/ovhai/models/data_sync_spec.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/data_sync_status.py` & `ovhai-0.1a3/ovhai/models/data_sync_status.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/doc_url.py` & `ovhai-0.1a3/ovhai/models/doc_url.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/env.py` & `ovhai-0.1a3/ovhai/models/env.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/error.py` & `ovhai-0.1a3/ovhai/models/error.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/fixed_scaling_strategy.py` & `ovhai-0.1a3/ovhai/models/fixed_scaling_strategy.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/flavor.py` & `ovhai-0.1a3/ovhai/models/flavor.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/framework.py` & `ovhai-0.1a3/ovhai/models/framework.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/framework_list.py` & `ovhai-0.1a3/ovhai/models/framework_list.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/get_v1_data_auth_alias_response_200.py` & `ovhai-0.1a3/ovhai/models/get_v1_data_auth_alias_response_200.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/git_credentials.py` & `ovhai-0.1a3/ovhai/models/git_credentials.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/gpu_information.py` & `ovhai-0.1a3/ovhai/models/gpu_information.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/https_basic_auth.py` & `ovhai-0.1a3/ovhai/models/https_basic_auth.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/image.py` & `ovhai-0.1a3/ovhai/models/image.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/image_list.py` & `ovhai-0.1a3/ovhai/models/image_list.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/image_mirror_status.py` & `ovhai-0.1a3/ovhai/models/image_mirror_status.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/image_version.py` & `ovhai-0.1a3/ovhai/models/image_version.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/image_version_list.py` & `ovhai-0.1a3/ovhai/models/image_version_list.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/info.py` & `ovhai-0.1a3/ovhai/models/info.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/info_arguments.py` & `ovhai-0.1a3/ovhai/models/info_arguments.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/job.py` & `ovhai-0.1a3/ovhai/models/job.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/job_image.py` & `ovhai-0.1a3/ovhai/models/job_image.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/job_list.py` & `ovhai-0.1a3/ovhai/models/job_list.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/job_spec.py` & `ovhai-0.1a3/ovhai/models/job_spec.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/job_spec_labels_type_0.py` & `ovhai-0.1a3/ovhai/models/job_spec_labels_type_0.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/job_spec_update.py` & `ovhai-0.1a3/ovhai/models/job_spec_update.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/job_state_history.py` & `ovhai-0.1a3/ovhai/models/job_state_history.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/job_status.py` & `ovhai-0.1a3/ovhai/models/job_status.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/label_update.py` & `ovhai-0.1a3/ovhai/models/label_update.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/links.py` & `ovhai-0.1a3/ovhai/models/links.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/me.py` & `ovhai-0.1a3/ovhai/models/me.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/metadata.py` & `ovhai-0.1a3/ovhai/models/metadata.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook.py` & `ovhai-0.1a3/ovhai/models/notebook.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook_backup.py` & `ovhai-0.1a3/ovhai/models/notebook_backup.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook_backup_list.py` & `ovhai-0.1a3/ovhai/models/notebook_backup_list.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook_editor.py` & `ovhai-0.1a3/ovhai/models/notebook_editor.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook_env.py` & `ovhai-0.1a3/ovhai/models/notebook_env.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook_framework.py` & `ovhai-0.1a3/ovhai/models/notebook_framework.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook_list.py` & `ovhai-0.1a3/ovhai/models/notebook_list.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook_spec.py` & `ovhai-0.1a3/ovhai/models/notebook_spec.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook_spec_labels_type_0.py` & `ovhai-0.1a3/ovhai/models/notebook_spec_labels_type_0.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook_spec_update.py` & `ovhai-0.1a3/ovhai/models/notebook_spec_update.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook_spec_update_labels_type_0.py` & `ovhai-0.1a3/ovhai/models/notebook_spec_update_labels_type_0.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook_status.py` & `ovhai-0.1a3/ovhai/models/notebook_status.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/notebook_workspace.py` & `ovhai-0.1a3/ovhai/models/notebook_workspace.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/partner.py` & `ovhai-0.1a3/ovhai/models/partner.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/preset.py` & `ovhai-0.1a3/ovhai/models/preset.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/preset_capabilities.py` & `ovhai-0.1a3/ovhai/models/preset_capabilities.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/preset_partner.py` & `ovhai-0.1a3/ovhai/models/preset_partner.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/preset_resources.py` & `ovhai-0.1a3/ovhai/models/preset_resources.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/private_swift_volume_source.py` & `ovhai-0.1a3/ovhai/models/private_swift_volume_source.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/probe.py` & `ovhai-0.1a3/ovhai/models/probe.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/project_quotas.py` & `ovhai-0.1a3/ovhai/models/project_quotas.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/project_quotas_resources.py` & `ovhai-0.1a3/ovhai/models/project_quotas_resources.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/public_git_volume_source.py` & `ovhai-0.1a3/ovhai/models/public_git_volume_source.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/public_swift_volume_source.py` & `ovhai-0.1a3/ovhai/models/public_swift_volume_source.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/registry.py` & `ovhai-0.1a3/ovhai/models/registry.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/registry_list.py` & `ovhai-0.1a3/ovhai/models/registry_list.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/registry_update.py` & `ovhai-0.1a3/ovhai/models/registry_update.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/resources.py` & `ovhai-0.1a3/ovhai/models/resources.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/resources_per_unit.py` & `ovhai-0.1a3/ovhai/models/resources_per_unit.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/s3_credentials.py` & `ovhai-0.1a3/ovhai/models/s3_credentials.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/scaling_strategy.py` & `ovhai-0.1a3/ovhai/models/scaling_strategy.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/ssh_key_pair.py` & `ovhai-0.1a3/ovhai/models/ssh_key_pair.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/standalone_volume_source.py` & `ovhai-0.1a3/ovhai/models/standalone_volume_source.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/terms_of_service_locale.py` & `ovhai-0.1a3/ovhai/models/terms_of_service_locale.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/token.py` & `ovhai-0.1a3/ovhai/models/token.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/token_list.py` & `ovhai-0.1a3/ovhai/models/token_list.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/token_spec.py` & `ovhai-0.1a3/ovhai/models/token_spec.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/token_status.py` & `ovhai-0.1a3/ovhai/models/token_status.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/update_framework.py` & `ovhai-0.1a3/ovhai/models/update_framework.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/update_image.py` & `ovhai-0.1a3/ovhai/models/update_image.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/update_image_version.py` & `ovhai-0.1a3/ovhai/models/update_image_version.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/user_volume.py` & `ovhai-0.1a3/ovhai/models/user_volume.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/volume.py` & `ovhai-0.1a3/ovhai/models/volume.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/volume_list.py` & `ovhai-0.1a3/ovhai/models/volume_list.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/models/volume_status.py` & `ovhai-0.1a3/ovhai/models/volume_status.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/ovhai_types.py` & `ovhai-0.1a3/ovhai/ovhai_types.py`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/ovhai/setup.py` & `ovhai-0.1a3/ovhai/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
 
 def readme():
     try:
-        with open('../README.md', encoding='utf-8') as f:
+        with open('../../README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "ovhai Package - Development Version"
 
 
 setup(
     name="ovhai",
-    version="0.1a2",
+    version="0.1a3",
     description="A client library for accessing OVHcloud's AI Solutions",
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords='ovhai ovh AI',
     project_urls={
           'Repository': 'https://github.com/ovh/ovhai-python-sdk'
       },
```

### Comparing `ovhai-0.1a2/ovhai.egg-info/SOURCES.txt` & `ovhai-0.1a3/ovhai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovhai-0.1a2/pyproject.toml` & `ovhai-0.1a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ovhai"
-version = "0.1a2"
+version = "0.1a3"
 description = "A client library for accessing OVHcloud's AI Solutions"
 authors = ["Mathieu Busquet <mathieu.busquet@ovhcloud.com>"]
 readme = "README.md"
 packages = [
     {include = "ovhai"},
 ]
 include = ["CHANGELOG.md", "ovhai/py.typed"]
```

